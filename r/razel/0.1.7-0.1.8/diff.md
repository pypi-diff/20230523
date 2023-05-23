# Comparing `tmp/razel-0.1.7.tar.gz` & `tmp/razel-0.1.8.tar.gz`

## Comparing `razel-0.1.7.tar` & `razel-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 razel-0.1.7/version.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 razel-0.1.7/src/razel/__init__.py
--rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 razel-0.1.7/src/razel/razel.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 razel-0.1.7/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 razel-0.1.7/LICENSE.md
--rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 razel-0.1.7/README.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 razel-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 razel-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 razel-0.1.8/version.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 razel-0.1.8/src/razel/__init__.py
+-rw-r--r--   0        0        0    15328 2020-02-02 00:00:00.000000 razel-0.1.8/src/razel/razel.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 razel-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 razel-0.1.8/LICENSE.md
+-rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 razel-0.1.8/README.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 razel-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 razel-0.1.8/PKG-INFO
```

### Comparing `razel-0.1.7/src/razel/razel.py` & `razel-0.1.8/src/razel/razel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # allows annotations with types that are not yet defined
 from __future__ import annotations
 
 import abc
 import json
 import os
+import subprocess
+import sys
 from enum import Enum
-from typing import ClassVar, Optional, Any, TypeVar
+from typing import ClassVar, Optional, Any, Tuple, TypeVar
 from collections.abc import Mapping, Sequence
 
 
 class Razel:
-    version: ClassVar[str] = "0.1.7"
+    version: ClassVar[str] = "0.1.8"
     _instance: ClassVar[Optional[Razel]] = None
 
     class Tag(str, Enum):
         QUIET = 'razel:quiet'
         VERBOSE = 'razel:verbose'
 
     def __init__(self, workspace_dir: str) -> None:
         self._workspace_dir = workspace_dir
+        self.razel_file = os.path.join(self._workspace_dir, "razel.jsonl")
         self._commands: list[Command] = []
 
     @staticmethod
     def init(workspace_dir: str) -> Razel:
         assert Razel._instance is None
         Razel._instance = Razel(workspace_dir)
         return Razel._instance
@@ -72,28 +75,51 @@
                 self.ensure_equal(arg1.outputs[i], arg2.outputs[i])
         else:
             file1 = _map_arg_to_output_file(arg1)
             file2 = _map_arg_to_output_file(arg2)
             name = f"{file1.basename}##shouldNotEqual##{file2.basename}"
             self._add(Task(name, "ensure-not-equal", [file1, file2]))
 
+    def run(self, args: list[str] = ["exec"]):
+        """Run the native razel binary to execute the commands.
+
+        Commands are written to `<workspace_dir>/razel.jsonl`. That file is processed with `razel exec`.
+        If the native razel binary is not available, it will be downloaded.
+
+        Output files are created in `<cwd>/razel-out`.
+        """
+        self.write_razel_file()
+        razel_binary_path = find_or_download_razel_binary(Razel.version)
+        cmd = [razel_binary_path]
+        if len(args) > 0 and args[0] == "exec":
+            razel_file_rel = os.path.relpath(self.razel_file, os.curdir)
+            cmd.extend([args[0]] + ['-f', razel_file_rel] + args[1:])
+        else:
+            cmd.extend(args)
+        print(" ".join(cmd))
+        status = subprocess.run(cmd).returncode
+        if status != 0:
+            sys.exit(status)
+
     def write_razel_file(self) -> None:
-        with open(os.path.join(self._workspace_dir, "razel.jsonl"), "w", encoding="utf-8") as file:
+        with open(self.razel_file, "w", encoding="utf-8") as file:
             for command in self._commands:
                 json.dump(command.json(), file, separators=(',', ':'))
                 file.write("\n")
 
     # Generic type used to ensure that _add() takes and returns the same type.
     _Command = TypeVar("_Command", bound="Command")
 
     def _add(self, command: _Command) -> _Command:
         for existing in self._commands:
             if existing.name == command.name:
-                assert command.json() == existing.json(), \
-                    f"conflicting actions: {command.name}:\nexisting: {existing.json()}\nto add: {command.json()}"
+                existing_json = existing.json_for_comparing_to_existing_command()
+                command_son = command.json_for_comparing_to_existing_command()
+                assert command_son == existing_json, \
+                    f"conflicting command: {command.name}:\nexisting: {existing_json}\nto add:   {command_son}"
                 assert isinstance(existing, type(command))
                 return existing
 
         self._commands.append(command)
         return command
 
     @staticmethod
@@ -133,21 +159,21 @@
         Razel.instance().ensure_equal(self, other)
 
     def ensure_not_equal(self, other: File | Command) -> None:
         Razel.instance().ensure_not_equal(self, other)
 
 
 class Command(abc.ABC):
-    def __init__(self, name: str, inputs: Sequence[File], outputs: Sequence[File]) -> None:
+    def __init__(self, name: str, inputs: list[File], outputs: list[File]) -> None:
         self._name = name
         self._inputs = inputs
         self._outputs = outputs
         self._stdout: File | None = None
         self._stderr: File | None = None
-        self._tags: Sequence[Razel.Tag | str] = []
+        self._tags: list[Razel.Tag | str] = []
         for out in self._outputs:
             out._created_by = self
 
     @property
     def name(self) -> str:
         return self._name
 
@@ -191,14 +217,18 @@
     def ensure_not_equal(self, other: File | Command) -> None:
         Razel.instance().ensure_not_equal(self, other)
 
     @abc.abstractmethod
     def json(self) -> Mapping[str, Any]:
         pass
 
+    @abc.abstractmethod
+    def json_for_comparing_to_existing_command(self) -> Mapping[str, Any]:
+        pass
+
 
 class CustomCommand(Command):
     def __init__(
         self, name: str, executable: str, args: Sequence[str | File], env: Optional[Mapping[str, str]] = None
     ) -> None:
         (inputs, outputs) = _split_args_in_inputs_and_outputs(args)
         super().__init__(name, inputs, outputs)
@@ -229,32 +259,32 @@
         for x in args:
             self.add_input_file(x)
         return self
 
     def add_output_file(self, arg: str | File) -> CustomCommand:
         """Add an output file which is not part of the command line."""
         file = arg if isinstance(arg, File) else Razel.instance().add_output_file(arg)
-        file._createdBy = self
+        file._created_by = self
         self._outputs.append(file)
         return self
 
-    def write_stdout_to_file(self, path: str = None) -> CustomCommand:
+    def write_stdout_to_file(self, path: Optional[str] = None) -> CustomCommand:
         self._stdout = Razel.instance().add_output_file(path if path else self._name)
         self._stdout._created_by = self
         self._outputs.append(self._stdout)
         return self
 
-    def write_stderr_to_file(self, path: str = None) -> CustomCommand:
+    def write_stderr_to_file(self, path: Optional[str] = None) -> CustomCommand:
         self._stderr = Razel.instance().add_output_file(path if path else self._name)
         self._stderr._created_by = self
         self._outputs.append(self._stderr)
         return self
 
     def json(self) -> Mapping[str, Any]:
-        j = {
+        j: Any = {
             "name": self.name,
             "executable": self.executable,
             "args": [x.file_name if isinstance(x, File) else x for x in self.args],
             "inputs": [x.file_name for x in self._inputs],
             "outputs": [x.file_name for x in self._outputs if x != self._stdout and x != self._stderr],
         }
         if self.env:
@@ -263,14 +293,25 @@
             j["stdout"] = self._stdout.file_name
         if self._stderr:
             j["stderr"] = self._stderr.file_name
         if self._tags:
             j["tags"] = self._tags
         return j
 
+    def json_for_comparing_to_existing_command(self) -> Mapping[str, Any]:
+        j: Any = {
+            "executable": self.executable,
+            "args": [x.file_name if isinstance(x, File) else x for x in self.args],
+            "inputs": [x.file_name for x in self._inputs],
+            "outputs": [x.file_name for x in self._outputs if x != self._stdout and x != self._stderr],
+        }
+        if self.env:
+            j["env"] = self.env
+        return j
+
 
 class Task(Command):
     @staticmethod
     def write_file(path: str, lines: Sequence[str]) -> File:
         file = Razel.instance().add_output_file(path)
         Razel.instance().add_task(path, "write-file", [file, *lines])
         return file
@@ -295,14 +336,20 @@
             "task": self.task,
             "args": [x.file_name if isinstance(x, File) else x for x in self.args],
         }
         if self._tags:
             j["tags"] = self._tags
         return j
 
+    def json_for_comparing_to_existing_command(self) -> Mapping[str, Any]:
+        return {
+            "task": self.task,
+            "args": [x.file_name if isinstance(x, File) else x for x in self.args],
+        }
+
 
 def _map_arg_to_output_path(arg: str | File | Command) -> str:
     if isinstance(arg, Command):
         return arg.output.file_name
     elif isinstance(arg, File):
         return arg.file_name
     return arg
@@ -312,11 +359,70 @@
     return arg.output if isinstance(arg, Command) else arg
 
 
 def _map_args_to_output_files(args: Sequence[str | File | Command]) -> Sequence[str | File]:
     return [x.output if isinstance(x, Command) else x for x in args]
 
 
-def _split_args_in_inputs_and_outputs(args: Sequence[str | File | Command]) -> (Sequence[File], Sequence[File]):
+def _split_args_in_inputs_and_outputs(args: Sequence[str | File | Command]) -> Tuple[list[File], list[File]]:
     inputs = [x for x in args if isinstance(x, File) and (x.is_data or x.created_by)]
     outputs = [x for x in args if isinstance(x, File) and not x.is_data and x.created_by is None]
     return inputs, outputs
+
+
+def find_or_download_razel_binary(version: str) -> str:
+    ext = ".exe" if sys.platform == "Windows" else ""
+    # try to use razel binary from PATH
+    path = f"razel{ext}"
+    if get_razel_version(path) == version:
+        return path
+    # try to use razel binary from .cache
+    if sys.platform == "Darwin":
+        cache_dir = f"{os.environ['HOME']}/Library/Caches/de.reu-dev.razel"
+    elif sys.platform == "Windows":
+        localAppData = os.environ["LOCALAPPDATA"].replace('\\', '/')
+        cache_dir = f"{localAppData}/reu-dev/razel"
+    else:
+        cache_dir = f"{os.environ['HOME']}/.cache/razel"
+    path = f"{cache_dir}/razel{ext}"
+    if get_razel_version(path) == version:
+        return path
+    # download razel binary to .cache
+    download_razel_binary(version, path)
+    return path
+
+
+def get_razel_version(path: str) -> Optional[str]:
+    try:
+        p = subprocess.run([path, "--version"], capture_output=True, text=True)
+        if p.returncode != 0:
+            return None
+        return p.stdout.strip().split(" ")[1]
+    except:
+        return None
+
+
+def download_razel_binary(version: Optional[str], path: str):
+    import gzip
+    import pathlib
+    import urllib.request
+    download_tag = f"download/v{version}" if version else "latest/download"
+    if sys.platform == "Darwin":
+        build_target = "x86_64-apple-Darwin"
+    elif sys.platform == "Windows":
+        build_target = "x86_64-pc-Windows-msvc"
+    else:
+        build_target = "x86_64-unknown-linux-gnu"
+    url = f"https://github.com/reu-dev/razel/releases/{download_tag}/razel-{build_target}.gz"
+    print('Download razel binary from', url)
+    with urllib.request.urlopen(url) as response:
+        with gzip.GzipFile(fileobj=response) as uncompressed:
+            file_content = uncompressed.read()
+    print(f"Extract razel binary to {path}")
+    pathlib.Path(path).parent.mkdir(parents=True, exist_ok=True)
+    with open(path, "wb") as f:
+        f.write(file_content)
+    if sys.platform != "Windows":
+        subprocess.check_call(["chmod", "+x", path])
+    actual_version = get_razel_version(path)
+    assert actual_version, "Failed to download razel binary. To build it from source, run: cargo install razel"
+    print(f"Downloaded razel {actual_version}")
```

### Comparing `razel-0.1.7/LICENSE.md` & `razel-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `razel-0.1.7/README.md` & `razel-0.1.8/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -17,59 +17,58 @@
 * Made for: data processing pipelines with executables working on files and many dependencies between those
 
 Razel is not the best choice for building software, especially there's no built-in support for compiler setup and header
 dependencies.
 
 ## Getting Started
 
-Use [rustup](https://rustup.rs/) to install Rust. Install `protobuf-compiler`. Clone and build Razel:
-
-```bash
-cargo install razel
-```
-
 The native input format for Razel is a `razel.jsonl` file, see the example [test/razel.jsonl](test/razel.jsonl).
-```
-razel exec -f test/razel.jsonl
-```
+It can be run with `razel exec -f test/razel.jsonl`.
+
+The preferred way is to use one of the high-level APIs. Both allow specifying the commands in an object-oriented style
+and provide a `run()` function which creates the `razel.jsonl` file, downloads the native `razel` binary
+and uses it to execute the commands.
 
-The preferred way to create a `razel.jsonl` file is using one of the high-level APIs.
+Output files are created in `<cwd>/razel-out`.
 
 ### TypeScript API
 
 Install [Deno](https://deno.land/) to use the [TypeScript API](include/deno/razel.ts).
-Run the [example Deno script](test/deno.ts) to create `test/razel.jsonl` and execute it with Razel:
+Run the [example Deno script](test/deno.ts):
 
 ```bash
-deno run --allow-write=. --check test/deno.ts
-razel exec -f test/razel.jsonl
+deno run -A --check test/deno.ts -- -v
 ```
 
 ### Python API
 
 The [Python API](include/python/razel.py) requires Python >= 3.8.
-Run the [example Python script](test/python.py) to create `test/razel.jsonl` and execute it with Razel:
+Install the package and run the [example Python script](test/python.py):
 
 ```bash
 pip install razel
-python3 test/python.py
-razel exec -f test/razel.jsonl
+python test/python.py -v
 ```
 
 ### Batch file
 
 In addition to `razel.jsonl`, Razel can directly execute a batch file containing commands.
 Input and output files need to be specified, which is WIP.
 
 Execute the example [test/batch.sh](test/batch.sh) with Razel:
 
 ```bash
 razel exec -f test/batch.sh
 ```
 
+### Building Razel from source
+
+Use [rustup](https://rustup.rs/) to install Rust. Install `protobuf-compiler`. Then run `cargo install razel`.
+
+
 ## Project Status
 
 Razel is in active development and **not** ready for production. CLI and format of `razel.jsonl` will likely change.
 
 | OS      | Status | Note                              |
 |---------|--------|-----------------------------------|
 | Linux   | ✓      | stable, main development platform |
```

### Comparing `razel-0.1.7/pyproject.toml` & `razel-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `razel-0.1.7/PKG-INFO` & `razel-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: razel
-Version: 0.1.7
+Version: 0.1.8
 Summary: a command executor with caching for data processing pipelines
 Project-URL: Homepage, https://github.com/reu-dev/razel
 Project-URL: Bug Tracker, https://github.com/reu-dev/razel/issues
 Author-email: Stefan Reuschl <stefan@reu-dev.de>, Kacper Sagnowski <ksagnowski@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,59 +31,58 @@
 * Made for: data processing pipelines with executables working on files and many dependencies between those
 
 Razel is not the best choice for building software, especially there's no built-in support for compiler setup and header
 dependencies.
 
 ## Getting Started
 
-Use [rustup](https://rustup.rs/) to install Rust. Install `protobuf-compiler`. Clone and build Razel:
-
-```bash
-cargo install razel
-```
-
 The native input format for Razel is a `razel.jsonl` file, see the example [test/razel.jsonl](test/razel.jsonl).
-```
-razel exec -f test/razel.jsonl
-```
+It can be run with `razel exec -f test/razel.jsonl`.
+
+The preferred way is to use one of the high-level APIs. Both allow specifying the commands in an object-oriented style
+and provide a `run()` function which creates the `razel.jsonl` file, downloads the native `razel` binary
+and uses it to execute the commands.
 
-The preferred way to create a `razel.jsonl` file is using one of the high-level APIs.
+Output files are created in `<cwd>/razel-out`.
 
 ### TypeScript API
 
 Install [Deno](https://deno.land/) to use the [TypeScript API](include/deno/razel.ts).
-Run the [example Deno script](test/deno.ts) to create `test/razel.jsonl` and execute it with Razel:
+Run the [example Deno script](test/deno.ts):
 
 ```bash
-deno run --allow-write=. --check test/deno.ts
-razel exec -f test/razel.jsonl
+deno run -A --check test/deno.ts -- -v
 ```
 
 ### Python API
 
 The [Python API](include/python/razel.py) requires Python >= 3.8.
-Run the [example Python script](test/python.py) to create `test/razel.jsonl` and execute it with Razel:
+Install the package and run the [example Python script](test/python.py):
 
 ```bash
 pip install razel
-python3 test/python.py
-razel exec -f test/razel.jsonl
+python test/python.py -v
 ```
 
 ### Batch file
 
 In addition to `razel.jsonl`, Razel can directly execute a batch file containing commands.
 Input and output files need to be specified, which is WIP.
 
 Execute the example [test/batch.sh](test/batch.sh) with Razel:
 
 ```bash
 razel exec -f test/batch.sh
 ```
 
+### Building Razel from source
+
+Use [rustup](https://rustup.rs/) to install Rust. Install `protobuf-compiler`. Then run `cargo install razel`.
+
+
 ## Project Status
 
 Razel is in active development and **not** ready for production. CLI and format of `razel.jsonl` will likely change.
 
 | OS      | Status | Note                              |
 |---------|--------|-----------------------------------|
 | Linux   | ✓      | stable, main development platform |
```

