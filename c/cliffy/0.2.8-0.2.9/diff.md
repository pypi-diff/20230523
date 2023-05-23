# Comparing `tmp/cliffy-0.2.8.tar.gz` & `tmp/cliffy-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliffy-0.2.8.tar", max compression
+gzip compressed data, was "cliffy-0.2.9.tar", max compression
```

## Comparing `cliffy-0.2.8.tar` & `cliffy-0.2.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1060 2023-05-21 17:30:19.035557 cliffy-0.2.8/LICENSE
--rw-r--r--   0        0        0     6575 2023-05-21 17:30:19.035557 cliffy-0.2.8/README.md
--rw-r--r--   0        0        0        0 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/__init__.py
--rw-r--r--   0        0        0       97 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/__main__.py
--rw-r--r--   0        0        0     1657 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/builder.py
--rw-r--r--   0        0        0     6741 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/cli.py
--rw-r--r--   0        0        0        0 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/clis/__init__.py
--rw-r--r--   0        0        0     4072 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/commander.py
--rw-r--r--   0        0        0        0 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/commanders/__init__.py
--rw-r--r--   0        0        0      981 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/commanders/click.py
--rw-r--r--   0        0        0     1939 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/commanders/typer.py
--rw-r--r--   0        0        0     2775 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/helper.py
--rw-r--r--   0        0        0     3030 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/homer.py
--rw-r--r--   0        0        0     1366 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/loader.py
--rw-r--r--   0        0        0      297 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/manifests/__init__.py
--rw-r--r--   0        0        0     7504 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/manifests/v1.py
--rw-r--r--   0        0        0      137 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/merger.py
--rw-r--r--   0        0        0     4959 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/parser.py
--rw-r--r--   0        0        0      860 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/rich.py
--rw-r--r--   0        0        0       47 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/run.py
--rw-r--r--   0        0        0     3515 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/transformer.py
--rw-r--r--   0        0        0     1092 2023-05-21 17:30:19.039557 cliffy-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     7536 1970-01-01 00:00:00.000000 cliffy-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-05-23 01:00:11.848763 cliffy-0.2.9/LICENSE
+-rw-r--r--   0        0        0     6575 2023-05-23 01:00:11.848763 cliffy-0.2.9/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/__init__.py
+-rw-r--r--   0        0        0       97 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/__main__.py
+-rw-r--r--   0        0        0     1657 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/builder.py
+-rw-r--r--   0        0        0     6705 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/cli.py
+-rw-r--r--   0        0        0        0 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/clis/__init__.py
+-rw-r--r--   0        0        0     4074 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/commander.py
+-rw-r--r--   0        0        0        0 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/commanders/__init__.py
+-rw-r--r--   0        0        0      981 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/commanders/click.py
+-rw-r--r--   0        0        0     1939 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/commanders/typer.py
+-rw-r--r--   0        0        0     2877 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/helper.py
+-rw-r--r--   0        0        0     3030 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/homer.py
+-rw-r--r--   0        0        0     1392 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/loader.py
+-rw-r--r--   0        0        0      297 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/manifests/__init__.py
+-rw-r--r--   0        0        0     7504 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/manifests/v1.py
+-rw-r--r--   0        0        0      137 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/merger.py
+-rw-r--r--   0        0        0     4971 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/parser.py
+-rw-r--r--   0        0        0      905 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/rich.py
+-rw-r--r--   0        0        0       47 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/run.py
+-rw-r--r--   0        0        0     4271 2023-05-23 01:00:11.848763 cliffy-0.2.9/cliffy/transformer.py
+-rw-r--r--   0        0        0     1092 2023-05-23 01:00:11.852763 cliffy-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     7536 1970-01-01 00:00:00.000000 cliffy-0.2.9/PKG-INFO
```

### Comparing `cliffy-0.2.8/LICENSE` & `cliffy-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.8/README.md` & `cliffy-0.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 4. Run loaded CLIs straight from the terminal
 5. When ready to share, run `build` or `bundle` to generate portable zipapps built with [Shiv](https://github.com/linkedin/shiv)
 
 ## Usage
 `cli <command>`
 * `init <cli name>`: Generate a template CLI manifest for a new CLI
 * `load <manifest>`: Add a new CLI based on the manifest
-* `render <manifest>`: Render the CLI manifest into python code
+* `render <manifest>`: View generated CLI script for a manifest
 * `list` or `ls`: Output a list of loaded CLIs 
 * `update <cli name>`: Reload a loaded CLI
 * `remove <cli name>` or `rm <cli name>`: Remove a loaded CLI
 * `run <manifest> -- <args>`: Runs a CLI manifest as a one-time operation
 * `build <manifest>`: Build a CLI manifest into a self-contained zipapp
 * `bundle <cli name>`: Bundle a loaded CLI into a self-contained zipapp
```

### Comparing `cliffy-0.2.8/cliffy/builder.py` & `cliffy-0.2.9/cliffy/builder.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.8/cliffy/cli.py` & `cliffy-0.2.9/cliffy/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ## CLI to generate CLIs
 import contextlib
 from tempfile import NamedTemporaryFile
 from typing import TextIO
 
 try:
     import rich_click as click  # type: ignore
-    from rich.console import Console
+    from rich.console import Console  # type: ignore
     from rich_click.rich_group import RichGroup as AliasGroup  # type: ignore
 except ImportError:
     import click
     from .rich import Console
     from click import Group as AliasGroup
 
 from .builder import build_cli, run_cli
-from .helper import CLIFFY_CLI_DIR, print_rich_table, write_to_file
+from .helper import CLIFFY_CLI_DIR, out, out_err, print_rich_table, write_to_file
 from .homer import get_clis, get_metadata, get_metadata_path, remove_metadata, save_metadata
 from .loader import Loader
 from .manifests import Manifest, set_manifest_version
 from .transformer import Transformer
 
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
@@ -39,43 +39,43 @@
 @click.argument('manifests', type=click.File('rb'), nargs=-1)
 def load(manifests: list[TextIO]) -> None:
     """Load CLI for given manifest(s)"""
     for manifest in manifests:
         T = Transformer(manifest)
         Loader.load_from_cli(T.cli)
         save_metadata(manifest.name, T.cli)
-        click.secho(f"~ Generated {T.cli.name} CLI v{T.cli.version} ~", fg="green")
-        click.secho(click.style("$", fg="magenta"), nl=False)
-        click.echo(f" {T.cli.name} -h")
+        out(f"✨ Generated {T.cli.name} CLI v{T.cli.version} ✨", fg="green")
+        out("$", fg="magenta", nl=False)
+        out(f" {T.cli.name} -h")
 
 
 @cli.command()
 @click.argument('cli_names', type=str, nargs=-1)
 def update(cli_names: list[str]) -> None:
     """Reloads CLI by name"""
     for cli_name in cli_names:
         if cli_metadata := get_metadata(cli_name):
             T = Transformer(open(cli_metadata.runner_path, "r"))
             Loader.load_from_cli(T.cli)
             save_metadata(cli_metadata.runner_path, T.cli)
-            click.secho(f"~ Reloaded {T.cli.name} CLI v{T.cli.version} ~", fg="green")
-            click.secho(click.style("$", fg="magenta"), nl=False)
-            click.echo(f" {T.cli.name} -h")
+            out(f"✨ Reloaded {T.cli.name} CLI v{T.cli.version} ✨", fg="green")
+            out("$", fg="magenta", nl=False)
+            out(f" {T.cli.name} -h")
         else:
-            click.secho(f"~ {cli_name} not found", fg="red")
+            out_err(f"~ {cli_name} not found")
 
 
 @cli.command()
 @click.argument('manifest', type=click.File('rb'))
 def render(manifest: TextIO) -> None:
     """Render the CLI manifest generation as code"""
     T = Transformer(manifest)
     console = Console()
     console.print(T.cli.code, overflow="fold", emoji=False, markup=False)
-    click.secho(f"# Rendered {T.cli.name} CLI v{T.cli.version} ~", fg="green")
+    out(f"# Rendered {T.cli.name} CLI v{T.cli.version} ~", fg="green")
 
 
 @cli.command("run")
 @click.argument('manifest', type=click.File('rb'))
 @click.argument('cli_args', type=str, nargs=-1)
 def cliffy_run(manifest: TextIO, cli_args: tuple[str]) -> None:
     """Run CLI for a manifest"""
@@ -100,16 +100,20 @@
     set_manifest_version(version)
     template = Manifest.get_raw_template(cli_name) if raw else Manifest.get_template(cli_name)
 
     if render:
         console = Console()
         console.print(template, overflow="fold", emoji=False, markup=False)
     else:
-        write_to_file(f'{cli_name}.yaml', text=template)
-        click.secho(f"+ {cli_name}.yaml", fg="green")
+        try:
+            write_to_file(f'{cli_name}.yaml', text=template)
+        except Exception as e:
+            out_err(f"~ error writing to file: {e}")
+            raise SystemExit(1)
+        out(f"+ {cli_name}.yaml", fg="green")
 
 
 @cli.command("list")
 def cliffy_list() -> None:
     "List all CLIs loaded"
     cols = ["Name", "Version", "Manifest"]
     rows = [[metadata.cli_name, metadata.version, metadata.runner_path] for metadata in get_clis()]
@@ -120,42 +124,42 @@
 @click.argument('cli_names', type=str, nargs=-1)
 def remove(cli_names: list[str]) -> None:
     "Remove a loaded CLI by name"
     for cli_name in cli_names:
         if get_metadata_path(cli_name):
             remove_metadata(cli_name)
             Loader.unload_cli(cli_name)
-            click.secho(f"~ {cli_name} unloaded", fg="green")
+            out(f"~ {cli_name} removed 💥", fg="green")
         else:
-            click.secho(f"~ {cli_name} not loaded", fg="red")
+            out_err(f"~ {cli_name} not loaded")
 
 
 @cli.command()
 @click.argument('cli_names', type=str, nargs=-1)
 @click.option('--debug', is_flag=True, show_default=True, default=False, help="Display build output")
 @click.option('--output-dir', '-o', type=click.Path(file_okay=False, dir_okay=True, writable=True), help="Output dir")
 def bundle(cli_names: list[str], debug: bool, output_dir: str) -> None:
     "Bundle a loaded CLI into a zipapp"
     for cli_name in cli_names:
         if not (metadata := get_metadata(cli_name)):
-            click.secho(f"~ {cli_name} not loaded", fg="red")
+            out_err(f"~ {cli_name} not loaded")
             continue
 
         result = build_cli(
             cli_name, script_path=f'{CLIFFY_CLI_DIR}/{cli_name}.py', deps=metadata.requires, output_dir=output_dir
         )
 
         if result.exit_code != 0:
-            click.secho(result.stdout)
-            click.secho(f"~ {cli_name} bundle failed", fg="red", error=True)
+            out(result.stdout)
+            out_err(f"~ {cli_name} bundle failed")
             continue
 
         if debug:
-            click.secho(result.stdout)
-        click.secho(f"+ {cli_name} bundled", fg="green")
+            out(result.stdout)
+        out(f"+ {cli_name} bundled 📦", fg="green")
 
 
 @cli.command()
 @click.argument('manifests', type=click.File('rb'), nargs=-1)
 @click.option('--debug', is_flag=True, show_default=True, default=False, help="Display build output")
 @click.option('--output-dir', '-o', type=click.Path(file_okay=False, dir_okay=True, writable=True), help="Output dir")
 def build(manifests: list[TextIO], debug: bool, output_dir: str) -> None:
@@ -164,20 +168,21 @@
         T = Transformer(manifest, validate_requires=False)
         with NamedTemporaryFile(mode='w', prefix=f'{T.cli.name}_', suffix='.py', delete=True) as script:
             script.write(T.cli.code)
             script.flush()
             result = build_cli(T.cli.name, script_path=script.name, deps=T.cli.requires, output_dir=output_dir)
 
         if result.exit_code != 0:
-            click.secho(result.stdout)
-            click.secho(f"~ {T.cli.name} build failed", fg="red", error=True)
+            out(result.stdout)
+            out_err(f"~ {T.cli.name} build failed")
             continue
 
         if debug:
-            click.secho(result.stdout)
-        click.secho(f"+ {T.cli.name} built", fg="green")
+            out(result.stdout)
+        out(f"+ {T.cli.name} built 📦", fg="green")
 
 
 ALIASES = {
+    "add": load,
     "rm": remove,
     "ls": cliffy_list,
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cliffy-0.2.8/cliffy/commander.py` & `cliffy-0.2.9/cliffy/commander.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         elif isinstance(self.manifest.imports, list):
             for _import in self.manifest.imports:
                 self.cli += _import + "\n"
 
     def add_functions(self) -> None:
         self.cli += "\n"
         for func in self.manifest.functions:
-            self.cli += f"{func}"
+            self.cli += f"{func}\n"
         self.cli += "\n"
 
     def add_greedy_commands(self) -> None:
         """Greedy commands get lazy-loaded. Only supported for group-commands currently"""
         for greedy_command in self.greedy:
             if greedy_command.name.startswith('(*)'):
                 for group in self.groups:
```

### Comparing `cliffy-0.2.8/cliffy/commanders/click.py` & `cliffy-0.2.9/cliffy/commanders/click.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.8/cliffy/commanders/typer.py` & `cliffy-0.2.9/cliffy/commanders/typer.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.8/cliffy/helper.py` & `cliffy-0.2.9/cliffy/helper.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import operator
 import os
 import platform
 import subprocess
 import sys
 from importlib.resources import files
 from pathlib import Path
-from typing import Optional
+from typing import Any, Optional
 
+from click import secho
 from packaging import version
 from pydantic import BaseModel
 
 try:
-    from rich.console import Console
-    from rich.table import Table
+    from rich.console import Console  # type: ignore
+    from rich.table import Table  # type: ignore
 except ImportError:
     from .rich import Console, Table
 
 HOME_PATH = str(Path.home())
 PYTHON_BIN = f"{sys.exec_prefix}/Scripts" if platform.system() == "Windows" else f"{sys.exec_prefix}/bin"
 PYTHON_EXECUTABLE = sys.executable
 CLIFFY_CLI_DIR = files('cliffy.clis')
@@ -33,28 +34,22 @@
 
 class RequirementSpec(BaseModel):
     name: str
     operator: Optional[str]
     version: Optional[str]
 
 
-def write_to_file(path: str, text: str, executable: bool = False) -> bool:
-    try:
-        output_file = Path(path)
-        output_file.parent.mkdir(exist_ok=True, parents=True)
-        output_file.write_text(text)
-    except Exception as e:
-        print("write_to_file", e)
-        return False
+def write_to_file(path: str, text: str, executable: bool = False) -> None:
+    output_file = Path(path)
+    output_file.parent.mkdir(exist_ok=True, parents=True)
+    output_file.write_text(text)
 
     if executable:
         make_executable(path)
 
-    return True
-
 
 def make_executable(path: str) -> None:
     mode = os.stat(path).st_mode
     mode |= (mode & 0o444) >> 2
     os.chmod(path, mode)
 
 
@@ -100,7 +95,15 @@
     return RequirementSpec(name=requirement.strip(), operator=None, version=None)
 
 
 def compare_versions(version1: str, version2: str, op: str) -> bool:
     v1 = version.parse(version1)
     v2 = version.parse(version2)
     return OPERATOR_MAP[op](v1, v2)
+
+
+def out(text: str, **echo_kwargs: Any) -> None:
+    secho(text, **echo_kwargs)
+
+
+def out_err(text: str) -> None:
+    secho(f"{text} 💔", fg='red', err=True)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cliffy-0.2.8/cliffy/homer.py` & `cliffy-0.2.9/cliffy/homer.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.8/cliffy/loader.py` & `cliffy-0.2.9/cliffy/loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import os
 
 from .commander import CLI
 from .helper import CLIFFY_CLI_DIR, PYTHON_BIN, PYTHON_EXECUTABLE, write_to_file
 
 
 class Loader:
+    __slots__ = ('cli',)
+
     def __init__(self, cli: CLI) -> None:
         self.cli = cli
 
     def deploy_cli(self) -> str:
         cli_path = Loader.get_cli_path(self.cli.name)
         write_to_file(cli_path, self.cli.code)
         return cli_path
```

### Comparing `cliffy-0.2.8/cliffy/manifests/v1.py` & `cliffy-0.2.9/cliffy/manifests/v1.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.8/cliffy/parser.py` & `cliffy-0.2.9/cliffy/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 
 from pybash.transformer import transform as transform_bash
 
 from .manifests import Manifest
 
 
 class Parser:
+
+    __slots__ = ('manifest',)
+
     def __init__(self, manifest: Manifest) -> None:
         self.manifest = manifest
 
     def is_param_required(self, param_type: str) -> bool:
         return (
             param_type.strip().endswith('!')
             if '=' not in param_type
@@ -30,18 +33,17 @@
         base_param_name = param_name.split('|')[0].replace('-', '')
         aliases = param_name.split('|')[1:]
 
         return base_param_name, aliases
 
     def parse_command_block(self, script: str):
         ## Bash commands start with $
-        if script.startswith('$'):
-            script = script.replace('$ ', '$', 1)
-            script = f'>{script[1:]}'
-            return " " * 4 + transform_bash(script)
+        if script.strip().startswith('$'):
+            pybash_script = f'>{script[1:].strip()}'
+            return " " * 4 + transform_bash(pybash_script)
 
         return "".join(" " * 4 + line + "\n" for line in script.split('\n'))
 
     def parse_command(self, block: Union[str, list[Union[str, dict[Literal['help'], str]]]]) -> str:
         if isinstance(block, list):
             script_block = []
             help_text = ""
```

### Comparing `cliffy-0.2.8/cliffy/rich.py` & `cliffy-0.2.9/cliffy/rich.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 ## Mimic rich API methods for rich-less support
-from typing import Union
+from typing import Any, Union
 
 import click
 
 
 class Console:
     def __init__(self) -> None:
         pass
 
-    def print(self, text, **kwargs) -> None:
+    def print(self, text: Any, **kwargs) -> None:
         if isinstance(text, Table):
             click.echo(text)
         else:
             print(text)
 
 
 class Table:
+
+    __slots__ = ('cols', 'rows')
+
     def __init__(self) -> None:
         self.cols: list[str] = []
         self.rows: list[list[str]] = []
 
     def add_column(self, col: str, style: Union[str, None] = None) -> None:
         self.cols.append(col)
```

### Comparing `cliffy-0.2.8/cliffy/transformer.py` & `cliffy-0.2.9/cliffy/transformer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,79 @@
 import os
 from typing import Any, TextIO
 
 import yaml
 from jinja2 import BaseLoader, Environment, FileSystemLoader
+from pydantic import ValidationError
 from typing_extensions import Self
 
 from .commander import build_cli
 from .commanders.typer import TyperCommander
-from .helper import compare_versions, get_installed_pip_packages, parse_requirement
+from .helper import compare_versions, get_installed_pip_packages, out, out_err, parse_requirement
 from .manifests import IncludeManifest, Manifest, set_manifest_version
 from .merger import cliffy_merger
 
 
 class Transformer:
     """Loads command manifest and transforms it into a CLI"""
 
-    def __init__(self, manifest_io: TextIO, as_include: bool = False, validate_requires: bool = True) -> None:
+    __slots__ = ('manifest_io', 'command_config', 'manifest_version', 'includes_config', 'manifest', 'cli')
+
+    def __init__(self, manifest_io: TextIO, *, as_include: bool = False, validate_requires: bool = True) -> None:
         self.manifest_io = manifest_io
         self.command_config = self.load_manifest(manifest_io)
         self.manifest_version = self.command_config.pop('manifestVersion', 'v1')
-
         if self.command_config.get("includes"):
             self.includes_config = self.resolve_includes()
             cliffy_merger.merge(self.command_config, self.includes_config)
 
         set_manifest_version(self.manifest_version)
         if as_include:
-            self.manifest = IncludeManifest(**self.command_config)
+            try:
+                self.manifest = IncludeManifest(**self.command_config)
+            except ValidationError as e:
+                out_err(f"~ error validating {manifest_io.name}")
+                out(f"{e}")
+                raise SystemExit(1)
         else:
-            self.manifest = Manifest(**self.command_config)
+            try:
+                self.manifest = Manifest(**self.command_config)
+            except ValidationError as e:
+                out_err(f"~ error validating {manifest_io.name}")
+                out(f"{e}")
+                raise SystemExit(1)
             if validate_requires:
                 self.validate_cli_requires()
             self.cli = build_cli(self.manifest, commander_cls=TyperCommander)
 
     def validate_cli_requires(self) -> None:
         if not self.manifest.requires:
             return
 
         installed_pip_packages = get_installed_pip_packages()
         for dep in self.manifest.requires:
             dep_spec = parse_requirement(dep)
             if dep_spec.name not in installed_pip_packages:
-                raise SystemExit(f"MissingRequirement: CLI requires `{dep}`, please install it")
+                out_err(f"~ missing requirement: `{self.manifest_io.name}` requires `{dep}` to be installed")
+                raise SystemExit(1)
 
             if (
                 dep_spec.version
                 and dep_spec.operator
                 and not compare_versions(
                     installed_pip_packages[dep_spec.name],
                     dep_spec.version,
                     dep_spec.operator,
                 )
             ):
-                raise SystemExit(
-                    f"MissingRequirement: CLI requires `{dep}`, "
-                    f"found version {installed_pip_packages[dep_spec.name]}"
+                out_err(
+                    f"~ missing requirement: `{self.manifest_io.name}` requires `{dep}` to be installed"
+                    f"    found version `{installed_pip_packages[dep_spec.name]}`"
                 )
+                raise SystemExit(1)
 
     def resolve_includes(self) -> dict:
         include_transforms = map(self.resolve_include_by_path, set(self.command_config['includes']))
         merged_config: dict[str, Any] = {}
         for transformed_include in include_transforms:
             cliffy_merger.merge(merged_config, transformed_include.command_config)
 
@@ -71,17 +85,19 @@
             return cls(m, as_include=True)
 
     @staticmethod
     def load_manifest(manifest_io: TextIO) -> dict[str, Any]:
         try:
             manifest_path = os.path.realpath(manifest_io.name)
             all_vars = yaml.safe_load(open(manifest_path, "r")).get('vars', {})
+            all_vars['env'] = os.environ
             var_env = Environment(loader=BaseLoader())
             interpolated_vars = {
                 var_env.from_string(str(k)).render(all_vars): var_env.from_string(str(v)).render(all_vars)
                 for k, v in all_vars.items()
             }
             manifest_env = Environment(loader=FileSystemLoader(manifest_path)).get_template("")
             return yaml.safe_load(manifest_env.render(interpolated_vars))
         except yaml.YAMLError as e:
-            print("load_manifest", e)
-            raise
+            out_err("~ error loading manifest")
+            out(f"{e}")
+            raise SystemExit(1)
```

### Comparing `cliffy-0.2.8/pyproject.toml` & `cliffy-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cliffy"
-version = "0.2.8"
+version = "0.2.9"
 description = "$ cli load from.yaml"
 authors = ["Jay <jay.github0@gmail.com>"]
 repository = "https://github.com/jaykv/cliffy"
 readme = "README.md"
 packages = [{include = "cliffy"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cliffy-0.2.8/PKG-INFO` & `cliffy-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliffy
-Version: 0.2.8
+Version: 0.2.9
 Summary: $ cli load from.yaml
 Home-page: https://github.com/jaykv/cliffy
 Author: Jay
 Author-email: jay.github0@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -52,15 +52,15 @@
 4. Run loaded CLIs straight from the terminal
 5. When ready to share, run `build` or `bundle` to generate portable zipapps built with [Shiv](https://github.com/linkedin/shiv)
 
 ## Usage
 `cli <command>`
 * `init <cli name>`: Generate a template CLI manifest for a new CLI
 * `load <manifest>`: Add a new CLI based on the manifest
-* `render <manifest>`: Render the CLI manifest into python code
+* `render <manifest>`: View generated CLI script for a manifest
 * `list` or `ls`: Output a list of loaded CLIs 
 * `update <cli name>`: Reload a loaded CLI
 * `remove <cli name>` or `rm <cli name>`: Remove a loaded CLI
 * `run <manifest> -- <args>`: Runs a CLI manifest as a one-time operation
 * `build <manifest>`: Build a CLI manifest into a self-contained zipapp
 * `bundle <cli name>`: Bundle a loaded CLI into a self-contained zipapp
```

