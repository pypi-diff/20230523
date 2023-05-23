# Comparing `tmp/docker-composer-0.8.5.tar.gz` & `tmp/docker_composer-2.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-composer-0.8.5.tar", last modified: Mon Nov 30 11:31:14 2020, max compression
+gzip compressed data, was "docker_composer-2.17.0.tar", max compression
```

## Comparing `docker-composer-0.8.5.tar` & `docker_composer-2.17.0.tar`

### file list

```diff
@@ -1,41 +1,37 @@
--rw-r--r--   0        0        0    11358 2020-11-30 09:54:14.384682 docker-composer-0.8.5/LICENSE.txt
--rw-r--r--   0        0        0     1326 2020-11-30 11:29:59.131581 docker-composer-0.8.5/pyproject.toml
--rw-r--r--   0        0        0     1978 2020-11-30 09:54:14.389742 docker-composer-0.8.5/README.md
--rw-r--r--   0        0        0       60 2020-11-30 09:54:14.392743 docker-composer-0.8.5/src/docker_composer/__init__.py
--rw-r--r--   0        0        0        0 2020-11-30 09:54:14.393939 docker-composer-0.8.5/src/docker_composer/_utils/__init__.py
--rw-r--r--   0        0        0     4480 2020-11-30 09:57:33.910164 docker-composer-0.8.5/src/docker_composer/_utils/argument.py
--rw-r--r--   0        0        0     7221 2020-11-30 09:58:05.806712 docker-composer-0.8.5/src/docker_composer/_utils/generate_class.py
--rw-r--r--   0        0        0     3238 2020-11-30 11:27:39.134164 docker-composer-0.8.5/src/docker_composer/base.py
--rw-r--r--   0        0        0      506 2020-11-30 10:02:41.554941 docker-composer-0.8.5/src/docker_composer/docker-composer.iml
--rw-r--r--   0        0        0        0 2020-11-30 09:54:14.397638 docker-composer-0.8.5/src/docker_composer/py.typed
--rw-r--r--   0        0        0        0 2020-11-30 09:54:14.398701 docker-composer-0.8.5/src/docker_composer/runner/__init__.py
--rw-r--r--   0        0        0        0 2020-11-30 09:54:14.400672 docker-composer-0.8.5/src/docker_composer/runner/cmd/__init__.py
--rw-r--r--   0        0        0     1800 2020-11-30 09:54:14.401638 docker-composer-0.8.5/src/docker_composer/runner/cmd/build.py
--rw-r--r--   0        0        0     1122 2020-11-30 09:54:14.402638 docker-composer-0.8.5/src/docker_composer/runner/cmd/bundle.py
--rw-r--r--   0        0        0     1221 2020-11-30 09:54:14.403638 docker-composer-0.8.5/src/docker_composer/runner/cmd/config.py
--rw-r--r--   0        0        0     1107 2020-11-30 09:54:14.404714 docker-composer-0.8.5/src/docker_composer/runner/cmd/create.py
--rw-r--r--   0        0        0     1457 2020-11-30 09:54:14.405638 docker-composer-0.8.5/src/docker_composer/runner/cmd/down.py
--rw-r--r--   0        0        0      566 2020-11-30 09:54:14.406913 docker-composer-0.8.5/src/docker_composer/runner/cmd/events.py
--rw-r--r--   0        0        0     1206 2020-11-30 09:54:14.407758 docker-composer-0.8.5/src/docker_composer/runner/cmd/exec.py
--rw-r--r--   0        0        0      423 2020-11-30 09:54:14.408638 docker-composer-0.8.5/src/docker_composer/runner/cmd/help.py
--rw-r--r--   0        0        0      544 2020-11-30 09:54:14.409638 docker-composer-0.8.5/src/docker_composer/runner/cmd/images.py
--rw-r--r--   0        0        0      549 2020-11-30 09:54:14.410638 docker-composer-0.8.5/src/docker_composer/runner/cmd/kill.py
--rw-r--r--   0        0        0      825 2020-11-30 09:54:14.412659 docker-composer-0.8.5/src/docker_composer/runner/cmd/logs.py
--rw-r--r--   0        0        0      422 2020-11-30 09:54:14.413663 docker-composer-0.8.5/src/docker_composer/runner/cmd/pause.py
--rw-r--r--   0        0        0      664 2020-11-30 09:54:14.414647 docker-composer-0.8.5/src/docker_composer/runner/cmd/port.py
--rw-r--r--   0        0        0      792 2020-11-30 09:54:14.415634 docker-composer-0.8.5/src/docker_composer/runner/cmd/ps.py
--rw-r--r--   0        0        0     1104 2020-11-30 09:54:14.415634 docker-composer-0.8.5/src/docker_composer/runner/cmd/pull.py
--rw-r--r--   0        0        0      592 2020-11-30 09:54:14.417634 docker-composer-0.8.5/src/docker_composer/runner/cmd/push.py
--rw-r--r--   0        0        0      554 2020-11-30 09:54:14.417634 docker-composer-0.8.5/src/docker_composer/runner/cmd/restart.py
--rw-r--r--   0        0        0     1043 2020-11-30 09:54:14.418844 docker-composer-0.8.5/src/docker_composer/runner/cmd/rm.py
--rw-r--r--   0        0        0     2284 2020-11-30 09:54:14.419648 docker-composer-0.8.5/src/docker_composer/runner/cmd/run.py
--rw-r--r--   0        0        0      791 2020-11-30 09:54:14.420634 docker-composer-0.8.5/src/docker_composer/runner/cmd/scale.py
--rw-r--r--   0        0        0      433 2020-11-30 09:54:14.421634 docker-composer-0.8.5/src/docker_composer/runner/cmd/start.py
--rw-r--r--   0        0        0      624 2020-11-30 09:54:14.422634 docker-composer-0.8.5/src/docker_composer/runner/cmd/stop.py
--rw-r--r--   0        0        0      430 2020-11-30 09:54:14.423634 docker-composer-0.8.5/src/docker_composer/runner/cmd/top.py
--rw-r--r--   0        0        0      430 2020-11-30 09:54:14.425222 docker-composer-0.8.5/src/docker_composer/runner/cmd/unpause.py
--rw-r--r--   0        0        0     3559 2020-11-30 09:54:14.425910 docker-composer-0.8.5/src/docker_composer/runner/cmd/up.py
--rw-r--r--   0        0        0      536 2020-11-30 09:54:14.426840 docker-composer-0.8.5/src/docker_composer/runner/cmd/version.py
--rw-r--r--   0        0        0    28007 2020-11-30 09:54:14.427634 docker-composer-0.8.5/src/docker_composer/runner/root.py
--rw-r--r--   0        0        0     2872 2020-11-30 11:31:15.346048 docker-composer-0.8.5/setup.py
--rw-r--r--   0        0        0     3061 2020-11-30 11:31:15.346904 docker-composer-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-22 17:40:30.205463 docker_composer-2.17.0/LICENSE.txt
+-rw-r--r--   0        0        0     1978 2023-05-22 17:40:30.205594 docker_composer-2.17.0/README.md
+-rw-r--r--   0        0        0     1332 2023-05-22 20:35:25.787694 docker_composer-2.17.0/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-05-22 19:40:35.299994 docker_composer-2.17.0/src/docker_composer/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 17:40:30.206343 docker_composer-2.17.0/src/docker_composer/_utils/__init__.py
+-rw-r--r--   0        0        0     4557 2023-05-22 20:35:25.788589 docker_composer-2.17.0/src/docker_composer/_utils/argument.py
+-rw-r--r--   0        0        0     7241 2023-05-22 20:35:25.789294 docker_composer-2.17.0/src/docker_composer/_utils/generate_class.py
+-rw-r--r--   0        0        0     3238 2023-05-22 17:40:30.206770 docker_composer-2.17.0/src/docker_composer/base.py
+-rw-r--r--   0        0        0        0 2023-05-22 17:40:30.206821 docker_composer-2.17.0/src/docker_composer/py.typed
+-rw-r--r--   0        0        0        0 2023-05-22 17:40:30.206931 docker_composer-2.17.0/src/docker_composer/runner/__init__.py
+-rw-r--r--   0        0        0     1227 2023-05-22 20:35:25.790242 docker_composer-2.17.0/src/docker_composer/runner/cmd/build.py
+-rw-r--r--   0        0        0     1811 2023-05-22 20:35:25.790760 docker_composer-2.17.0/src/docker_composer/runner/cmd/config.py
+-rw-r--r--   0        0        0      937 2023-05-22 20:35:25.791110 docker_composer-2.17.0/src/docker_composer/runner/cmd/cp.py
+-rw-r--r--   0        0        0     1414 2023-05-22 20:35:25.791824 docker_composer-2.17.0/src/docker_composer/runner/cmd/create.py
+-rw-r--r--   0        0        0     1029 2023-05-22 20:35:25.792441 docker_composer-2.17.0/src/docker_composer/runner/cmd/down.py
+-rw-r--r--   0        0        0      608 2023-05-22 20:35:25.792940 docker_composer-2.17.0/src/docker_composer/runner/cmd/events.py
+-rw-r--r--   0        0        0     1234 2023-05-22 20:35:25.793552 docker_composer-2.17.0/src/docker_composer/runner/cmd/exec.py
+-rw-r--r--   0        0        0      690 2023-05-22 20:35:25.794073 docker_composer-2.17.0/src/docker_composer/runner/cmd/images.py
+-rw-r--r--   0        0        0      729 2023-05-22 20:35:25.794481 docker_composer-2.17.0/src/docker_composer/runner/cmd/kill.py
+-rw-r--r--   0        0        0     1250 2023-05-22 20:35:25.795147 docker_composer-2.17.0/src/docker_composer/runner/cmd/logs.py
+-rw-r--r--   0        0        0      830 2023-05-22 20:35:25.795508 docker_composer-2.17.0/src/docker_composer/runner/cmd/ls.py
+-rw-r--r--   0        0        0      463 2023-05-22 20:35:25.795972 docker_composer-2.17.0/src/docker_composer/runner/cmd/pause.py
+-rw-r--r--   0        0        0      687 2023-05-22 20:35:25.796437 docker_composer-2.17.0/src/docker_composer/runner/cmd/port.py
+-rw-r--r--   0        0        0     1112 2023-05-22 20:35:25.797054 docker_composer-2.17.0/src/docker_composer/runner/cmd/ps.py
+-rw-r--r--   0        0        0      964 2023-05-22 20:35:25.797590 docker_composer-2.17.0/src/docker_composer/runner/cmd/pull.py
+-rw-r--r--   0        0        0      856 2023-05-22 20:35:25.798080 docker_composer-2.17.0/src/docker_composer/runner/cmd/push.py
+-rw-r--r--   0        0        0      689 2023-05-22 20:35:25.798685 docker_composer-2.17.0/src/docker_composer/runner/cmd/restart.py
+-rw-r--r--   0        0        0     1012 2023-05-22 20:35:25.799207 docker_composer-2.17.0/src/docker_composer/runner/cmd/rm.py
+-rw-r--r--   0        0        0     2329 2023-05-22 20:35:25.799746 docker_composer-2.17.0/src/docker_composer/runner/cmd/run.py
+-rw-r--r--   0        0        0      463 2023-05-22 20:35:25.800293 docker_composer-2.17.0/src/docker_composer/runner/cmd/start.py
+-rw-r--r--   0        0        0      564 2023-05-22 20:35:25.800735 docker_composer-2.17.0/src/docker_composer/runner/cmd/stop.py
+-rw-r--r--   0        0        0      473 2023-05-22 20:35:25.801329 docker_composer-2.17.0/src/docker_composer/runner/cmd/top.py
+-rw-r--r--   0        0        0      471 2023-05-22 20:35:25.801939 docker_composer-2.17.0/src/docker_composer/runner/cmd/unpause.py
+-rw-r--r--   0        0        0     3410 2023-05-22 20:35:25.802415 docker_composer-2.17.0/src/docker_composer/runner/cmd/up.py
+-rw-r--r--   0        0        0      702 2023-05-22 20:35:25.802883 docker_composer-2.17.0/src/docker_composer/runner/cmd/version.py
+-rw-r--r--   0        0        0    27397 2023-05-22 20:35:25.803600 docker_composer-2.17.0/src/docker_composer/runner/root.py
+-rw-r--r--   0        0        0     3147 1970-01-01 00:00:00.000000 docker_composer-2.17.0/PKG-INFO
```

### Comparing `docker-composer-0.8.5/LICENSE.txt` & `docker_composer-2.17.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `docker-composer-0.8.5/pyproject.toml` & `docker_composer-2.17.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docker-composer"
-version = "0.8.5"
+version = "2.17.0"
 description = "Use docker-compose from within Python"
 authors = ["Micha <schollm-git@gmx.com>"]
 readme = "README.md"
 homepage = "https://github.com/schollm/docker-composer"
 repository = "https://github.com/schollm/docker-composer"
 license = "Apache-2.0"
 packages = [
@@ -19,22 +19,22 @@
   "Topic :: Software Development :: Libraries :: Application Frameworks",
   "Operating System :: OS Independent",
   "Development Status :: 4 - Beta"
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.6"
-attrs = "^20.3.0"
-loguru = "^0.5.3"
+python = "^3.7"
+attrs = ">=20.3.0"
+loguru = ">=0.5.3"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.1.2"
-black = "^20.8b1"
-isort = "^5.6.4"
+pytest = ">=6.1.2"
+black = ">=20.8b1"
+isort = ">=5.6.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest]
 addopts = "-ra --black"
```

### Comparing `docker-composer-0.8.5/README.md` & `docker_composer-2.17.0/README.md`

 * *Files identical despite different names*

### Comparing `docker-composer-0.8.5/src/docker_composer/_utils/argument.py` & `docker_composer-2.17.0/src/docker_composer/_utils/argument.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,17 @@
     "TLS_KEY_PATH": str,
     "USER": str,
     "type": str,
     "string": str,
     "int": int,
     "list": list,
     "str": str,
+    "stringArray": list[str],
+    "volumes": list[str],
+    "docker": bool,
 }
 
 
 @attr.s(auto_attribs=True, frozen=True)
 class Argument:
     arg: str
     type_desc: str
@@ -68,15 +71,15 @@
         return Argument(arg, type_desc, type_, desc, default_str)
 
 
 def _collect_arguments(arguments: Iterable[str]) -> Iterator[str]:
     """Combine argument lines to obtain one line per argument"""
     res = ""
     for arg in arguments:
-        if res and arg[:6].strip().startswith("-"):
+        if res and arg[:12].strip().startswith("-"):
             yield res.strip()
             res = ""
         res += f"\n   {arg.strip()}"
     if res:
         yield res.strip()
```

### Comparing `docker-composer-0.8.5/src/docker_composer/_utils/generate_class.py` & `docker_composer-2.17.0/src/docker_composer/_utils/generate_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import os
 import subprocess
 from collections import defaultdict
 from functools import lru_cache, reduce
 from operator import add
 from pathlib import Path
-from typing import Iterable, Iterator, List, Mapping, Optional, Set, Tuple, Union
+from typing import Iterable, Iterator, List, Mapping, Set, Tuple, Union
 
 import black
 import isort
 from isort.exceptions import ISortError
 from loguru import logger
 
 from docker_composer._utils.argument import Argument, parse_dc_argument
@@ -34,28 +33,33 @@
 
 @lru_cache()
 def get_help_message(subcommand: str = "") -> str:
     """Obtain the help message for subcommand from docker-compose."""
     args = [arg for arg in ["docker-compose", subcommand, "--help"] if arg]
     process = subprocess.run(args, capture_output=True, text=True)
     if process.returncode:
-        logger.error(process.returncode)
+        logger.error(
+            "docker-compose {} --help exited with {}:", subcommand, process.returncode
+        )
         logger.error(process.stderr)
+
     return process.stdout
 
 
 def collect_help_lines(msg: str) -> Mapping[str, List[str]]:
     """Collect help messages into sections.
     :param msg: Output from docker-compose <cmd> --help
     :returns Mapping from section header to lines as lists. First (unnamed) section gets name "general"
     """
     parts: Mapping[str, List[str]] = defaultdict(list)
     part = "general"
     for line in msg.split("\n"):
-        if line and line[0] != " " and line.endswith(":") and " " not in line:
+        if not line:
+            part = "general"
+        elif " " not in line and line.endswith(":"):
             part = line[:-1].lower()
         else:
             parts[part].append(line)
     return parts
 
 
 def parse_help(msg: str) -> Tuple[Mapping[str, List[str]], List[Argument]]:
@@ -177,44 +181,43 @@
     _cmd: str = "{cmd or ""}"
     _options: List[str] = [{options}]
 {indent(cmd_fns, level=nl)}
 ''',
         level=level,
     )
     try:
-        res = isort.code(res, config=isort.Config(settings_path=project_root()))
+        res = isort.code(
+            res, config=isort.Config(settings_path=project_root().as_posix())
+        )
     except ISortError as exc:
         logger.exception(exc)
     try:
         return black.format_str(res, mode=black.Mode())
     except Exception as exc:
         logger.exception(exc)
         return res
 
 
-def write_class(cmd: str, file_name: Optional[str] = None) -> None:
+def write_class(cmd: str) -> None:
     """
     Generate a class for `cmd` and write it to `file_name`
 
     :param cmd: docker-compose command to create or an empty string for root.
     :param file_name: Name of output file (empty/None for auto-generation)
     :return:
     """
-    if not file_name:
-        file_name = os.path.join(
-            os.path.dirname(__file__),
-            "..",
-            "runner",
-            "cmd" if cmd else "",
-            f"{cmd or 'root'}.py",
-        )
+    base_path = Path(__file__).parents[1] / "runner"
+    if cmd:
+        file_name = base_path / "cmd" / f"{cmd}.py"
+    else:
+        file_name = base_path / "root.py"
+
     class_str = generate_class(f"DockerCompose{(cmd or 'root').capitalize()}", cmd)
-    logger.info("Write {:<8s} -> {}", cmd or "root", file_name)
-    with open(file_name, "w") as f:
-        f.write(class_str)
+    logger.info("Write {:<8s} -> {}", cmd, file_name)
+    file_name.write_text(class_str, encoding="utf-8")
 
 
 def main() -> None:
     write_class("")
     docker_lines = get_help_message("")
     sections, _ = parse_help(docker_lines)
     for cmd_line in sections["commands"]:
```

### Comparing `docker-composer-0.8.5/src/docker_composer/base.py` & `docker_composer-2.17.0/src/docker_composer/base.py`

 * *Files identical despite different names*

### Comparing `docker-composer-0.8.5/src/docker_composer/runner/cmd/build.py` & `docker_composer-2.17.0/src/docker_composer/runner/cmd/ps.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,35 @@
-# DO NOT EDIT: Autogenerated by src/docker_composer/_utils/generate_class.py
-# for docker-compose version 1.25.0, build unknown
+# DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
+# for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
-class DockerComposeBuild(DockerBaseRunner):
+class DockerComposePs(DockerBaseRunner):
     """
-    Build or rebuild services.
-
-    Services are built once and then tagged as `project_service`,
-    e.g. `composetest_db`. If you change a service's `Dockerfile` or the
-    contents of its build directory, you can run `docker-compose build` to rebuild it.
-
-    Usage: build [options] [--build-arg key=val...] [SERVICE...]
-
+    Usage:  docker compose ps [OPTIONS] [SERVICE...]
+    List containers
     """
 
-    build_arg: Optional[dict] = None
-    """Set build-time variables for services."""
-    compress: Optional[bool] = None
-    """Compress the build context using gzip."""
-    force_rm: Optional[bool] = None
-    """Always remove intermediate containers."""
-    memory: Optional[int] = None
-    """Set memory limit for the build container."""
-    no_cache: Optional[bool] = None
-    """Do not use cache when building the image."""
-    no_rm: Optional[bool] = None
-    """Do not remove intermediate containers after a successful build."""
-    parallel: Optional[bool] = None
-    """Build images in parallel."""
-    progress: Optional[str] = None
-    """Set type of progress output (auto, plain, tty).
-       EXPERIMENTAL flag for native builder.
-       To enable, run with COMPOSE_DOCKER_CLI_BUILD=1)"""
-    pull: Optional[bool] = None
-    """Always attempt to pull a newer version of the image."""
+    all: Optional[bool] = None
+    """Show all stopped containers (including those created by the run command)"""
+    filter: Optional[str] = None
+    """Filter services by a property (supported filters: status)."""
+    format: Optional[str] = None
+    """Format the output. Values: [table | json] (default "table")"""
     quiet: Optional[bool] = None
-    """Don't print anything to STDOUT"""
-    _cmd: str = "build"
+    """Only display IDs"""
+    services: Optional[bool] = None
+    """Display services"""
+    status: Optional[list] = None
+    """Filter services by status. Values: [paused | restarting | removing | running | dead | created | exited]"""
+    _cmd: str = "ps"
     _options: List[str] = [
-        "compress",
-        "force_rm",
-        "no_cache",
-        "no_rm",
-        "parallel",
-        "pull",
+        "all",
         "quiet",
+        "services",
     ]
```

### Comparing `docker-composer-0.8.5/src/docker_composer/runner/cmd/config.py` & `docker_composer-2.17.0/src/docker_composer/runner/cmd/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,53 @@
-# DO NOT EDIT: Autogenerated by src/docker_composer/_utils/generate_class.py
-# for docker-compose version 1.25.0, build unknown
+# DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
+# for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeConfig(DockerBaseRunner):
     """
-    Validate and view the Compose file.
-
-    Usage: config [options]
-
+    Usage:  docker compose config [OPTIONS] [SERVICE...]
+    Parse, resolve and render compose file in canonical format
     """
 
-    resolve_image_digests: Optional[bool] = None
-    """Pin image tags to digests."""
+    format: Optional[str] = None
+    """Format the output. Values: [yaml | json] (default "yaml")"""
+    hash: Optional[str] = None
+    """Print the service config hash, one per line."""
+    images: Optional[bool] = None
+    """Print the image names, one per line."""
+    no_consistency: Optional[bool] = None
+    """Don't check model consistency - warning: may produce invalid Compose output"""
     no_interpolate: Optional[bool] = None
-    """Don't interpolate environment variables"""
+    """Don't interpolate environment variables."""
+    no_normalize: Optional[bool] = None
+    """Don't normalize compose model."""
+    output: Optional[str] = None
+    """Save to file (default to stdout)"""
+    profiles: Optional[bool] = None
+    """Print the profile names, one per line."""
     quiet: Optional[bool] = None
-    """Only validate the configuration, don't print
-       anything."""
+    """Only validate the configuration, don't print anything."""
+    resolve_image_digests: Optional[bool] = None
+    """Pin image tags to digests."""
     services: Optional[bool] = None
     """Print the service names, one per line."""
     volumes: Optional[bool] = None
     """Print the volume names, one per line."""
-    hash: Optional[str] = None
-    """Print the service config hash, one per line.
-       Set "service1,service2" for a list of specified services
-       or use the wildcard symbol to display all services"""
     _cmd: str = "config"
     _options: List[str] = [
-        "resolve_image_digests",
+        "images",
+        "no_consistency",
         "no_interpolate",
+        "no_normalize",
+        "profiles",
         "quiet",
+        "resolve_image_digests",
         "services",
         "volumes",
     ]
```

### Comparing `docker-composer-0.8.5/src/docker_composer/runner/cmd/create.py` & `docker_composer-2.17.0/src/docker_composer/runner/cmd/cp.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,29 @@
-# DO NOT EDIT: Autogenerated by src/docker_composer/_utils/generate_class.py
-# for docker-compose version 1.25.0, build unknown
+# DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
+# for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
-class DockerComposeCreate(DockerBaseRunner):
+class DockerComposeCp(DockerBaseRunner):
     """
-    Creates containers for a service.
-    This command is deprecated. Use the `up` command with `--no-start` instead.
-
-    Usage: create [options] [SERVICE...]
-
+    Usage:  docker compose cp [OPTIONS] SERVICE:SRC_PATH DEST_PATH|-
+        docker compose cp [OPTIONS] SRC_PATH|- SERVICE:DEST_PATH
+    Copy files/folders between a service container and the local filesystem
     """
 
-    force_recreate: Optional[bool] = None
-    """Recreate containers even if their configuration and
-       image haven't changed. Incompatible with --no-recreate."""
-    no_recreate: Optional[bool] = None
-    """If containers already exist, don't recreate them.
-       Incompatible with --force-recreate."""
-    no_build: Optional[bool] = None
-    """Don't build an image, even if it's missing."""
-    build: Optional[bool] = None
-    """Build images before creating containers."""
-    _cmd: str = "create"
+    archive: Optional[bool] = None
+    """Archive mode (copy all uid/gid information)"""
+    follow_link: Optional[bool] = None
+    """Always follow symbol link in SRC_PATH"""
+    index: Optional[int] = None
+    """Index of the container if there are multiple instances of a service ."""
+    _cmd: str = "cp"
     _options: List[str] = [
-        "force_recreate",
-        "no_recreate",
-        "no_build",
-        "build",
+        "archive",
+        "follow_link",
     ]
```

### Comparing `docker-composer-0.8.5/src/docker_composer/runner/cmd/events.py` & `docker_composer-2.17.0/src/docker_composer/runner/cmd/events.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-# DO NOT EDIT: Autogenerated by src/docker_composer/_utils/generate_class.py
-# for docker-compose version 1.25.0, build unknown
+# DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
+# for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeEvents(DockerBaseRunner):
     """
+    Usage:  docker compose events [OPTIONS] [SERVICE...]
     Receive real time events from containers.
-
-    Usage: events [options] [SERVICE...]
-
     """
 
     json: Optional[bool] = None
     """Output events as a stream of json objects"""
     _cmd: str = "events"
     _options: List[str] = [
         "json",
```

### Comparing `docker-composer-0.8.5/src/docker_composer/runner/cmd/exec.py` & `docker_composer-2.17.0/src/docker_composer/runner/cmd/exec.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,36 @@
-# DO NOT EDIT: Autogenerated by src/docker_composer/_utils/generate_class.py
-# for docker-compose version 1.25.0, build unknown
+# DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
+# for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeExec(DockerBaseRunner):
     """
-    Execute a command in a running container
-
-    Usage: exec [options] [-e KEY=VAL...] SERVICE COMMAND [ARGS...]
-
+    Usage:  docker compose exec [OPTIONS] SERVICE COMMAND [ARGS...]
+    Execute a command in a running container.
     """
 
     detach: Optional[bool] = None
     """Detached mode: Run command in the background."""
+    env: Optional[list] = None
+    """Set environment variables"""
+    index: Optional[int] = None
+    """index of the container if there are multiple instances of a service [default: 1]. (default 1)"""
+    no_TTY: Optional[bool] = None
+    """Disable pseudo-TTY allocation. By default docker compose exec allocates a TTY. (default true)"""
     privileged: Optional[bool] = None
     """Give extended privileges to the process."""
     user: Optional[str] = None
     """Run the command as this user."""
-    T: Optional[bool] = None
-    """Disable pseudo-tty allocation. By default `docker-compose exec`
-       allocates a TTY."""
-    index: Optional[int] = None
-    """index of the container if there are multiple
-       instances of a service [default: 1]"""
-    env: Optional[dict] = None
-    """not supported in API < 1.25)"""
     workdir: Optional[str] = None
     """Path to workdir directory for this command."""
     _cmd: str = "exec"
     _options: List[str] = [
         "detach",
         "privileged",
-        "T",
     ]
```

### Comparing `docker-composer-0.8.5/src/docker_composer/runner/cmd/images.py` & `docker_composer-2.17.0/src/docker_composer/runner/cmd/kill.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-# DO NOT EDIT: Autogenerated by src/docker_composer/_utils/generate_class.py
-# for docker-compose version 1.25.0, build unknown
+# DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
+# for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
-class DockerComposeImages(DockerBaseRunner):
+class DockerComposeKill(DockerBaseRunner):
     """
-    List images used by the created containers.
-    Usage: images [options] [SERVICE...]
-
+    Usage:  docker compose kill [OPTIONS] [SERVICE...]
+    Force stop service containers.
     """
 
-    quiet: Optional[bool] = None
-    """Only display IDs"""
-    _cmd: str = "images"
+    remove_orphans: Optional[bool] = None
+    """Remove containers for services not defined in the Compose file."""
+    signal: Optional[str] = None
+    """SIGNAL to send to the container. (default "SIGKILL")"""
+    _cmd: str = "kill"
     _options: List[str] = [
-        "quiet",
+        "remove_orphans",
     ]
```

### Comparing `docker-composer-0.8.5/src/docker_composer/runner/cmd/kill.py` & `docker_composer-2.17.0/src/docker_composer/runner/cmd/stop.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-# DO NOT EDIT: Autogenerated by src/docker_composer/_utils/generate_class.py
-# for docker-compose version 1.25.0, build unknown
+# DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
+# for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
-class DockerComposeKill(DockerBaseRunner):
+class DockerComposeStop(DockerBaseRunner):
     """
-    Force stop service containers.
-
-    Usage: kill [options] [SERVICE...]
-
+    Usage:  docker compose stop [OPTIONS] [SERVICE...]
+    Stop services
     """
 
-    s: Optional[int] = None
-    """SIGNAL to send to the container.
-       Default signal is SIGKILL."""
-    _cmd: str = "kill"
+    timeout: Optional[int] = None
+    """Specify a shutdown timeout in seconds (default 10)"""
+    _cmd: str = "stop"
     _options: List[str] = []
```

### Comparing `docker-composer-0.8.5/src/docker_composer/runner/cmd/logs.py` & `docker_composer-2.17.0/src/docker_composer/runner/cmd/logs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-# DO NOT EDIT: Autogenerated by src/docker_composer/_utils/generate_class.py
-# for docker-compose version 1.25.0, build unknown
+# DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
+# for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeLogs(DockerBaseRunner):
     """
-    View output from containers.
-
-    Usage: logs [options] [SERVICE...]
-
+    Usage:  docker compose logs [OPTIONS] [SERVICE...]
+    View output from containers
     """
 
-    no_color: Optional[bool] = None
-    """Produce monochrome output."""
     follow: Optional[bool] = None
     """Follow log output."""
+    no_color: Optional[bool] = None
+    """Produce monochrome output."""
+    no_log_prefix: Optional[bool] = None
+    """Don't print prefix in logs."""
+    since: Optional[str] = None
+    """Show logs since timestamp (e.g. 2013-01-02T13:23:37Z) or relative (e.g. 42m for 42 minutes)"""
+    tail: Optional[str] = None
+    """Number of lines to show from the end of the logs for each container. (default "all")"""
     timestamps: Optional[bool] = None
     """Show timestamps."""
-    tail: Optional[str] = None
-    """Number of lines to show from the end of the logs
-       for each container."""
+    until: Optional[str] = None
+    """Show logs before a timestamp (e.g. 2013-01-02T13:23:37Z) or relative (e.g. 42m for 42 minutes)"""
     _cmd: str = "logs"
     _options: List[str] = [
-        "no_color",
         "follow",
+        "no_color",
+        "no_log_prefix",
         "timestamps",
     ]
```

### Comparing `docker-composer-0.8.5/src/docker_composer/runner/cmd/port.py` & `docker_composer-2.17.0/src/docker_composer/runner/cmd/port.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-# DO NOT EDIT: Autogenerated by src/docker_composer/_utils/generate_class.py
-# for docker-compose version 1.25.0, build unknown
+# DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
+# for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposePort(DockerBaseRunner):
     """
+    Usage:  docker compose port [OPTIONS] SERVICE PRIVATE_PORT
     Print the public port for a port binding.
-
-    Usage: port [options] SERVICE PRIVATE_PORT
-
     """
 
-    protocol: Optional[str] = None
-    """tcp or udp [default: tcp]"""
     index: Optional[int] = None
-    """index of the container if there are multiple
-       instances of a service [default: 1]"""
+    """index of the container if service has multiple replicas (default 1)"""
+    protocol: Optional[str] = None
+    """tcp or udp (default "tcp")"""
     _cmd: str = "port"
     _options: List[str] = []
```

### Comparing `docker-composer-0.8.5/src/docker_composer/runner/cmd/ps.py` & `docker_composer-2.17.0/src/docker_composer/runner/cmd/restart.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,25 @@
-# DO NOT EDIT: Autogenerated by src/docker_composer/_utils/generate_class.py
-# for docker-compose version 1.25.0, build unknown
+# DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
+# for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
-class DockerComposePs(DockerBaseRunner):
+class DockerComposeRestart(DockerBaseRunner):
     """
-    List containers.
-
-    Usage: ps [options] [SERVICE...]
-
+    Usage:  docker compose restart [OPTIONS] [SERVICE...]
+    Restart service containers
     """
 
-    quiet: Optional[bool] = None
-    """Only display IDs"""
-    services: Optional[bool] = None
-    """Display services"""
-    filter: Optional[dict] = None
-    """Filter services by a property"""
-    all: Optional[bool] = None
-    """Show all stopped containers (including those created by the run command)"""
-    _cmd: str = "ps"
+    no_deps: Optional[bool] = None
+    """Don't restart dependent services."""
+    timeout: Optional[int] = None
+    """Specify a shutdown timeout in seconds (default 10)"""
+    _cmd: str = "restart"
     _options: List[str] = [
-        "quiet",
-        "services",
-        "all",
+        "no_deps",
     ]
```

### Comparing `docker-composer-0.8.5/src/docker_composer/runner/cmd/pull.py` & `docker_composer-2.17.0/src/docker_composer/runner/cmd/images.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,25 @@
-# DO NOT EDIT: Autogenerated by src/docker_composer/_utils/generate_class.py
-# for docker-compose version 1.25.0, build unknown
+# DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
+# for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
-class DockerComposePull(DockerBaseRunner):
+class DockerComposeImages(DockerBaseRunner):
     """
-    Pulls images for services defined in a Compose file, but does not start the containers.
-
-    Usage: pull [options] [SERVICE...]
-
+    Usage:  docker compose images [OPTIONS] [SERVICE...]
+    List images used by the created containers
     """
 
-    ignore_pull_failures: Optional[bool] = None
-    """Pull what it can and ignores images with pull failures."""
-    parallel: Optional[bool] = None
-    """Deprecated, pull multiple images in parallel (enabled by default)."""
-    no_parallel: Optional[bool] = None
-    """Disable parallel pulling."""
+    format: Optional[str] = None
+    """Format the output. Values: [table | json]. (default "table")"""
     quiet: Optional[bool] = None
-    """Pull without printing progress information"""
-    include_deps: Optional[bool] = None
-    """Also pull services declared as dependencies"""
-    _cmd: str = "pull"
+    """Only display IDs"""
+    _cmd: str = "images"
     _options: List[str] = [
-        "ignore_pull_failures",
-        "parallel",
-        "no_parallel",
         "quiet",
-        "include_deps",
     ]
```

### Comparing `docker-composer-0.8.5/src/docker_composer/runner/cmd/push.py` & `docker_composer-2.17.0/src/docker_composer/runner/cmd/version.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# DO NOT EDIT: Autogenerated by src/docker_composer/_utils/generate_class.py
-# for docker-compose version 1.25.0, build unknown
+# DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
+# for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
-class DockerComposePush(DockerBaseRunner):
+class DockerComposeVersion(DockerBaseRunner):
     """
-    Pushes images for services.
-
-    Usage: push [options] [SERVICE...]
-
+    Usage:  docker compose version [OPTIONS]
+    Show the Docker Compose version information
     """
 
-    ignore_push_failures: Optional[bool] = None
-    """Push what it can and ignores images with push failures."""
-    _cmd: str = "push"
+    format: Optional[str] = None
+    """Format the output. Values: [pretty | json]. (Default: pretty)"""
+    short: Optional[bool] = None
+    """Shows only Compose's version number."""
+    _cmd: str = "version"
     _options: List[str] = [
-        "ignore_push_failures",
+        "short",
     ]
```

### Comparing `docker-composer-0.8.5/src/docker_composer/runner/cmd/rm.py` & `docker_composer-2.17.0/src/docker_composer/runner/cmd/rm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,32 @@
-# DO NOT EDIT: Autogenerated by src/docker_composer/_utils/generate_class.py
-# for docker-compose version 1.25.0, build unknown
+# DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
+# for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeRm(DockerBaseRunner):
     """
-    Removes stopped service containers.
-
+    Usage:  docker compose rm [OPTIONS] [SERVICE...]
+    Removes stopped service containers
     By default, anonymous volumes attached to containers will not be removed. You
-    can override this with `-v`. To list all volumes, use `docker volume ls`.
-
+    can override this with -v. To list all volumes, use "docker volume ls".
     Any data which is not in a volume will be lost.
-
-    Usage: rm [options] [SERVICE...]
-
     """
 
     force: Optional[bool] = None
     """Don't ask to confirm removal"""
     stop: Optional[bool] = None
     """Stop the containers, if required, before removing"""
-    v: Optional[bool] = None
+    volumes: Optional[bool] = None
     """Remove any anonymous volumes attached to containers"""
-    all: Optional[bool] = None
-    """Deprecated - no effect."""
     _cmd: str = "rm"
     _options: List[str] = [
         "force",
         "stop",
-        "v",
-        "all",
+        "volumes",
     ]
```

### Comparing `docker-composer-0.8.5/src/docker_composer/runner/cmd/run.py` & `docker_composer-2.17.0/src/docker_composer/runner/cmd/run.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,66 @@
-# DO NOT EDIT: Autogenerated by src/docker_composer/_utils/generate_class.py
-# for docker-compose version 1.25.0, build unknown
+# DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
+# for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeRun(DockerBaseRunner):
     """
+    Usage:  docker compose run [OPTIONS] SERVICE [COMMAND] [ARGS...]
     Run a one-off command on a service.
-
-    For example:
-
-        $ docker-compose run web python manage.py shell
-
-    By default, linked services will be started, unless they are already
-    running. If you do not want to start linked services, use
-    `docker-compose run --no-deps SERVICE COMMAND [ARGS...]`.
-
-    Usage:
-        run [options] [-v VOLUME...] [-p PORT...] [-e KEY=VAL...] [-l KEY=VALUE...]
-            SERVICE [COMMAND] [ARGS...]
-
     """
 
+    build: Optional[bool] = None
+    """Build image before starting container."""
     detach: Optional[bool] = None
-    """Detached mode: Run container in the background, print
-       new container name."""
+    """Run container in background and print container ID"""
+    entrypoint: Optional[str] = None
+    """Override the entrypoint of the image"""
+    env: Optional[list] = None
+    """Set environment variables"""
+    interactive: Optional[bool] = None
+    """Keep STDIN open even if not attached. (default true)"""
+    label: Optional[list] = None
+    """Add or override a label"""
     name: Optional[str] = None
     """Assign a name to the container"""
-    entrypoint: Optional[str] = None
-    """Override the entrypoint of the image."""
-    e: Optional[dict] = None
-    """Set an environment variable (can be used multiple times)"""
-    label: Optional[dict] = None
-    """Add or override a label (can be used multiple times)"""
-    user: Optional[str] = None
-    """Run as specified username or uid"""
+    no_TTY: Optional[bool] = None
+    """Disable pseudo-TTY allocation (default: auto-detected). (default true)"""
     no_deps: Optional[bool] = None
     """Don't start linked services."""
-    rm: Optional[bool] = None
-    """Remove container after run. Ignored in detached mode."""
     publish: Optional[list] = None
-    """Publish a container's port(s) to the host"""
+    """Publish a container's port(s) to the host."""
+    quiet_pull: Optional[bool] = None
+    """Pull without printing progress information."""
+    remove_orphans: Optional[bool] = None
+    """Remove containers for services not defined in the Compose file."""
+    rm: Optional[bool] = None
+    """Automatically remove the container when it exits"""
     service_ports: Optional[bool] = None
-    """Run command with the service's ports enabled and mapped
-       to the host."""
+    """Run command with the service's ports enabled and mapped to the host."""
     use_aliases: Optional[bool] = None
-    """Use the service's network aliases in the network(s) the
-       container connects to."""
+    """Use the service's network useAliases in the network(s) the container connects to."""
+    user: Optional[str] = None
+    """Run as specified username or uid"""
     volume: Optional[list] = None
-    """Bind mount a volume (default [])"""
-    T: Optional[bool] = None
-    """Disable pseudo-tty allocation. By default `docker-compose run`
-       allocates a TTY."""
+    """Bind mount a volume."""
     workdir: Optional[str] = None
     """Working directory inside the container"""
     _cmd: str = "run"
     _options: List[str] = [
+        "build",
         "detach",
+        "interactive",
+        "no_TTY",
         "no_deps",
+        "quiet_pull",
+        "remove_orphans",
         "rm",
         "service_ports",
         "use_aliases",
-        "T",
     ]
```

### Comparing `docker-composer-0.8.5/src/docker_composer/runner/cmd/scale.py` & `docker_composer-2.17.0/src/docker_composer/runner/cmd/pull.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# DO NOT EDIT: Autogenerated by src/docker_composer/_utils/generate_class.py
-# for docker-compose version 1.25.0, build unknown
+# DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
+# for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
-class DockerComposeScale(DockerBaseRunner):
+class DockerComposePull(DockerBaseRunner):
     """
-    Set number of containers to run for a service.
-
-    Numbers are specified in the form `service=num` as arguments.
-    For example:
-
-        $ docker-compose scale web=2 worker=3
-
-    This command is deprecated. Use the up command with the `--scale` flag
-    instead.
-
-    Usage: scale [options] [SERVICE=NUM...]
-
+    Usage:  docker compose pull [OPTIONS] [SERVICE...]
+    Pull service images
     """
 
-    timeout: Optional[int] = None
-    """Specify a shutdown timeout in seconds.
-       (default: 10)"""
-    _cmd: str = "scale"
-    _options: List[str] = []
+    ignore_buildable: Optional[bool] = None
+    """Ignore images that can be built."""
+    ignore_pull_failures: Optional[bool] = None
+    """Pull what it can and ignores images with pull failures."""
+    include_deps: Optional[bool] = None
+    """Also pull services declared as dependencies."""
+    quiet: Optional[bool] = None
+    """Pull without printing progress information."""
+    _cmd: str = "pull"
+    _options: List[str] = [
+        "ignore_buildable",
+        "ignore_pull_failures",
+        "include_deps",
+        "quiet",
+    ]
```

### Comparing `docker-composer-0.8.5/src/docker_composer/runner/cmd/up.py` & `docker_composer-2.17.0/src/docker_composer/runner/cmd/up.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,85 @@
-# DO NOT EDIT: Autogenerated by src/docker_composer/_utils/generate_class.py
-# for docker-compose version 1.25.0, build unknown
+# DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
+# for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeUp(DockerBaseRunner):
     """
-    Builds, (re)creates, starts, and attaches to containers for a service.
-
-    Unless they are already running, this command also starts any linked services.
-
-    The `docker-compose up` command aggregates the output of each container. When
-    the command exits, all containers are stopped. Running `docker-compose up -d`
-    starts the containers in the background and leaves them running.
-
-    If there are existing containers for a service, and the service's configuration
-    or image was changed after the container's creation, `docker-compose up` picks
-    up the changes by stopping and recreating the containers (preserving mounted
-    volumes). To prevent Compose from picking up changes, use the `--no-recreate`
-    flag.
-
-    If you want to force Compose to stop and recreate all containers, use the
-    `--force-recreate` flag.
-
-    Usage: up [options] [--scale SERVICE=NUM...] [SERVICE...]
-
+    Usage:  docker compose up [OPTIONS] [SERVICE...]
+    Create and start containers
     """
 
+    abort_on_container_exit: Optional[bool] = None
+    """Stops all containers if any container was stopped. Incompatible with -d"""
+    always_recreate_deps: Optional[bool] = None
+    """Recreate dependent containers. Incompatible with --no-recreate."""
+    attach: Optional[list] = None
+    """Attach to service output."""
+    attach_dependencies: Optional[bool] = None
+    """Attach to dependent containers."""
+    build: Optional[bool] = None
+    """Build images before starting containers."""
     detach: Optional[bool] = None
-    """Detached mode: Run containers in the background,
-       print new container names. Incompatible with
-       --abort-on-container-exit."""
+    """Detached mode: Run containers in the background"""
+    exit_code_from: Optional[str] = None
+    """Return the exit code of the selected service container. Implies --abort-on-container-exit"""
+    force_recreate: Optional[bool] = None
+    """Recreate containers even if their configuration and image haven't changed."""
+    no_attach: Optional[list] = None
+    """Don't attach to specified service."""
+    no_build: Optional[bool] = None
+    """Don't build an image, even if it's missing."""
     no_color: Optional[bool] = None
     """Produce monochrome output."""
-    quiet_pull: Optional[bool] = None
-    """Pull without printing progress information"""
     no_deps: Optional[bool] = None
     """Don't start linked services."""
-    force_recreate: Optional[bool] = None
-    """Recreate containers even if their configuration
-       and image haven't changed."""
-    always_recreate_deps: Optional[bool] = None
-    """Recreate dependent containers.
-       Incompatible with --no-recreate."""
+    no_log_prefix: Optional[bool] = None
+    """Don't print prefix in logs."""
     no_recreate: Optional[bool] = None
-    """If containers already exist, don't recreate
-       them. Incompatible with --force-recreate and -V."""
-    no_build: Optional[bool] = None
-    """Don't build an image, even if it's missing."""
+    """If containers already exist, don't recreate them. Incompatible with --force-recreate."""
     no_start: Optional[bool] = None
     """Don't start the services after creating them."""
-    build: Optional[bool] = None
-    """Build images before starting containers."""
-    abort_on_container_exit: Optional[bool] = None
-    """Stops all containers if any container was
-       stopped. Incompatible with -d."""
-    timeout: Optional[int] = None
-    """Use this timeout in seconds for container
-       shutdown when attached or when containers are
-       already running. (default: 10)"""
-    renew_anon_volumes: Optional[bool] = None
-    """Recreate anonymous volumes instead of retrieving
-       data from the previous containers."""
+    pull: Optional[str] = None
+    """Pull image before running ("always"|"missing"|"never") (default "missing")"""
+    quiet_pull: Optional[bool] = None
+    """Pull without printing progress information."""
     remove_orphans: Optional[bool] = None
-    """Remove containers for services not defined
-       in the Compose file."""
-    exit_code_from: Optional[str] = None
-    """Return the exit code of the selected service
-       container. Implies --abort-on-container-exit."""
-    scale: Optional[dict] = None
-    """Scale SERVICE to NUM instances. Overrides the
-       `scale` setting in the Compose file if present."""
+    """Remove containers for services not defined in the Compose file."""
+    renew_anon_volumes: Optional[bool] = None
+    """Recreate anonymous volumes instead of retrieving data from the previous containers."""
+    scale: Optional[str] = None
+    """Scale SERVICE to NUM instances. Overrides the scale setting in the Compose file if present."""
+    timestamps: Optional[bool] = None
+    """Show timestamps."""
+    wait: Optional[bool] = None
+    """Wait for services to be running|healthy. Implies detached mode."""
+    wait_timeout: Optional[int] = None
+    """timeout waiting for application to be running|healthy."""
+    waitTimeout: Optional[int] = None
+    """Use this waitTimeout in seconds for container shutdown when attached or when containers are already running. (default 10)"""
     _cmd: str = "up"
     _options: List[str] = [
+        "abort_on_container_exit",
+        "always_recreate_deps",
+        "attach_dependencies",
+        "build",
         "detach",
+        "force_recreate",
+        "no_build",
         "no_color",
-        "quiet_pull",
         "no_deps",
-        "force_recreate",
-        "always_recreate_deps",
+        "no_log_prefix",
         "no_recreate",
-        "no_build",
         "no_start",
-        "build",
-        "abort_on_container_exit",
-        "renew_anon_volumes",
+        "quiet_pull",
         "remove_orphans",
+        "renew_anon_volumes",
+        "timestamps",
+        "wait",
     ]
```

### Comparing `docker-composer-0.8.5/src/docker_composer/runner/root.py` & `docker_composer-2.17.0/src/docker_composer/runner/root.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,777 +1,652 @@
-# DO NOT EDIT: Autogenerated by src/docker_composer/_utils/generate_class.py
-# for docker-compose version 1.25.0, build unknown
+# DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
+# for Docker Compose version v2.17.2
 
 from typing import List, Optional
 
 import attr
 
 import docker_composer.runner.cmd.build
-import docker_composer.runner.cmd.bundle
 import docker_composer.runner.cmd.config
+import docker_composer.runner.cmd.cp
 import docker_composer.runner.cmd.create
 import docker_composer.runner.cmd.down
 import docker_composer.runner.cmd.events
 import docker_composer.runner.cmd.exec
-import docker_composer.runner.cmd.help
 import docker_composer.runner.cmd.images
 import docker_composer.runner.cmd.kill
 import docker_composer.runner.cmd.logs
+import docker_composer.runner.cmd.ls
 import docker_composer.runner.cmd.pause
 import docker_composer.runner.cmd.port
 import docker_composer.runner.cmd.ps
 import docker_composer.runner.cmd.pull
 import docker_composer.runner.cmd.push
 import docker_composer.runner.cmd.restart
 import docker_composer.runner.cmd.rm
 import docker_composer.runner.cmd.run
-import docker_composer.runner.cmd.scale
 import docker_composer.runner.cmd.start
 import docker_composer.runner.cmd.stop
 import docker_composer.runner.cmd.top
 import docker_composer.runner.cmd.unpause
 import docker_composer.runner.cmd.up
 import docker_composer.runner.cmd.version
 from docker_composer.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
 class DockerComposeRoot(DockerBaseRunner):
     """
-    Define and run multi-container applications with Docker.
-
-    Usage:
-      docker-compose [-f <arg>...] [options] [COMMAND] [ARGS...]
-      docker-compose -h|--help
-
+    Usage:  docker compose [OPTIONS] COMMAND
+    Docker Compose
+    Run 'docker compose COMMAND --help' for more information on a command.
     """
 
-    file: Optional[str] = None
-    """Specify an alternate compose file
-       (default: docker-compose.yml)"""
-    project_name: Optional[str] = None
-    """Specify an alternate project name
-       (default: directory name)"""
-    verbose: Optional[bool] = None
-    """Show more output"""
-    log_level: Optional[int] = None
-    """Set log level (DEBUG, INFO, WARNING, ERROR, CRITICAL)"""
-    no_ansi: Optional[bool] = None
-    """Do not print ANSI control characters"""
-    host: Optional[str] = None
-    """Daemon socket to connect to"""
-    tls: Optional[bool] = None
-    """Use TLS; implied by --tlsverify"""
-    tlscacert: Optional[str] = None
-    """Trust certs signed only by this CA"""
-    tlscert: Optional[str] = None
-    """Path to TLS certificate file"""
-    tlskey: Optional[str] = None
-    """Path to TLS key file"""
-    tlsverify: Optional[bool] = None
-    """Use TLS and verify the remote"""
-    skip_hostname_check: Optional[bool] = None
-    """Don't check the daemon's hostname against the
-       name specified in the client certificate"""
+    ansi: Optional[str] = None
+    """Control when to print ANSI control characters ("never"|"always"|"auto") (default "auto")"""
+    compatibility: Optional[bool] = None
+    """Run compose in backward compatibility mode"""
+    env_file: Optional[list] = None
+    """Specify an alternate environment file."""
+    file: Optional[list] = None
+    """Compose configuration files"""
+    parallel: Optional[int] = None
+    """Control max parallelism, -1 for unlimited (default -1)"""
+    profile: Optional[list] = None
+    """Specify a profile to enable"""
     project_directory: Optional[str] = None
     """Specify an alternate working directory
-       (default: the path of the Compose file)"""
-    compatibility: Optional[bool] = None
-    """If set, Compose will attempt to convert keys
-       in v3 files to their non-Swarm equivalent"""
-    env_file: Optional[str] = None
-    """Specify an alternate environment file"""
+       (default: the path of the, first specified, Compose file)"""
+    project_name: Optional[str] = None
+    """Project name"""
     _cmd: str = ""
     _options: List[str] = [
-        "verbose",
-        "no_ansi",
-        "tls",
-        "tlsverify",
-        "skip_hostname_check",
         "compatibility",
     ]
 
     def build(
         self,
-        build_arg: Optional[dict] = None,
-        compress: Optional[bool] = None,
-        force_rm: Optional[bool] = None,
-        memory: Optional[int] = None,
+        build_arg: Optional[list] = None,
         no_cache: Optional[bool] = None,
-        no_rm: Optional[bool] = None,
-        parallel: Optional[bool] = None,
         progress: Optional[str] = None,
         pull: Optional[bool] = None,
+        push: Optional[bool] = None,
         quiet: Optional[bool] = None,
+        ssh: Optional[str] = None,
     ) -> docker_composer.runner.cmd.build.DockerComposeBuild:
         """
-        Build or rebuild services.
-
-        Services are built once and then tagged as `project_service`,
-        e.g. `composetest_db`. If you change a service's `Dockerfile` or the
-        contents of its build directory, you can run `docker-compose build` to rebuild it.
-
-        Usage: build [options] [--build-arg key=val...] [SERVICE...]
-
+        Usage:  docker compose build [OPTIONS] [SERVICE...]
+        Build or rebuild services
 
         :param build_arg: Set build-time variables for services.
-        :param compress: Compress the build context using gzip.
-        :param force_rm: Always remove intermediate containers.
-        :param memory: Set memory limit for the build container.
-        :param no_cache: Do not use cache when building the image.
-        :param no_rm: Do not remove intermediate containers after a successful build.
-        :param parallel: Build images in parallel.
-        :param progress: Set type of progress output (auto, plain, tty).
-           EXPERIMENTAL flag for native builder.
-           To enable, run with COMPOSE_DOCKER_CLI_BUILD=1)
+        :param no_cache: Do not use cache when building the image
+        :param progress: Set type of progress output (auto, tty, plain, quiet) (default "auto")
         :param pull: Always attempt to pull a newer version of the image.
+        :param push: Push service images.
         :param quiet: Don't print anything to STDOUT
+        :param ssh: Set SSH authentications used when building service images. (use 'default' for using your default SSH Agent)
         """
         runner = docker_composer.runner.cmd.build.DockerComposeBuild(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
-    def bundle(
-        self, push_images: Optional[bool] = None, output: Optional[str] = None
-    ) -> docker_composer.runner.cmd.bundle.DockerComposeBundle:
-        """
-        Generate a Distributed Application Bundle (DAB) from the Compose file.
-
-        Images must have digests stored, which requires interaction with a
-        Docker registry. If digests aren't stored for all images, you can fetch
-        them with `docker-compose pull` or `docker-compose push`. To push images
-        automatically when bundling, pass `--push-images`. Only services with
-        a `build` option specified will have their images pushed.
-
-        Usage: bundle [options]
-
-
-        :param push_images: Automatically push images for any services
-           which have a `build` option specified.
-        :param output: Path to write the bundle file to.
-           Defaults to "<project name>.dab".
-        """
-        runner = docker_composer.runner.cmd.bundle.DockerComposeBundle(
-            **{k: v for k, v in locals().items() if k != "self"}
-        )
-        runner._parent_cmd = self._call_cmd()
-        return runner
-
     def config(
         self,
-        resolve_image_digests: Optional[bool] = None,
+        format: Optional[str] = None,
+        hash: Optional[str] = None,
+        images: Optional[bool] = None,
+        no_consistency: Optional[bool] = None,
         no_interpolate: Optional[bool] = None,
+        no_normalize: Optional[bool] = None,
+        output: Optional[str] = None,
+        profiles: Optional[bool] = None,
         quiet: Optional[bool] = None,
+        resolve_image_digests: Optional[bool] = None,
         services: Optional[bool] = None,
         volumes: Optional[bool] = None,
-        hash: Optional[str] = None,
     ) -> docker_composer.runner.cmd.config.DockerComposeConfig:
         """
-        Validate and view the Compose file.
-
-        Usage: config [options]
-
+        Usage:  docker compose config [OPTIONS] [SERVICE...]
+        Parse, resolve and render compose file in canonical format
 
+        :param format: Format the output. Values: [yaml | json] (default "yaml")
+        :param hash: Print the service config hash, one per line.
+        :param images: Print the image names, one per line.
+        :param no_consistency: Don't check model consistency - warning: may produce invalid Compose output
+        :param no_interpolate: Don't interpolate environment variables.
+        :param no_normalize: Don't normalize compose model.
+        :param output: Save to file (default to stdout)
+        :param profiles: Print the profile names, one per line.
+        :param quiet: Only validate the configuration, don't print anything.
         :param resolve_image_digests: Pin image tags to digests.
-        :param no_interpolate: Don't interpolate environment variables
-        :param quiet: Only validate the configuration, don't print
-           anything.
         :param services: Print the service names, one per line.
         :param volumes: Print the volume names, one per line.
-        :param hash: Print the service config hash, one per line.
-           Set "service1,service2" for a list of specified services
-           or use the wildcard symbol to display all services
         """
         runner = docker_composer.runner.cmd.config.DockerComposeConfig(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
+    def cp(
+        self,
+        archive: Optional[bool] = None,
+        follow_link: Optional[bool] = None,
+        index: Optional[int] = None,
+    ) -> docker_composer.runner.cmd.cp.DockerComposeCp:
+        """
+        Usage:  docker compose cp [OPTIONS] SERVICE:SRC_PATH DEST_PATH|-
+                docker compose cp [OPTIONS] SRC_PATH|- SERVICE:DEST_PATH
+        Copy files/folders between a service container and the local filesystem
+
+        :param archive: Archive mode (copy all uid/gid information)
+        :param follow_link: Always follow symbol link in SRC_PATH
+        :param index: Index of the container if there are multiple instances of a service .
+        """
+        runner = docker_composer.runner.cmd.cp.DockerComposeCp(
+            **{k: v for k, v in locals().items() if k != "self"}
+        )
+        runner._parent_cmd = self._call_cmd()
+        return runner
+
     def create(
         self,
+        build: Optional[bool] = None,
         force_recreate: Optional[bool] = None,
-        no_recreate: Optional[bool] = None,
         no_build: Optional[bool] = None,
-        build: Optional[bool] = None,
+        no_recreate: Optional[bool] = None,
+        pull: Optional[str] = None,
+        remove_orphans: Optional[bool] = None,
+        scale: Optional[str] = None,
     ) -> docker_composer.runner.cmd.create.DockerComposeCreate:
         """
+        Usage:  docker compose create [OPTIONS] [SERVICE...]
         Creates containers for a service.
-        This command is deprecated. Use the `up` command with `--no-start` instead.
-
-        Usage: create [options] [SERVICE...]
-
 
-        :param force_recreate: Recreate containers even if their configuration and
-           image haven't changed. Incompatible with --no-recreate.
-        :param no_recreate: If containers already exist, don't recreate them.
-           Incompatible with --force-recreate.
+        :param build: Build images before starting containers.
+        :param force_recreate: Recreate containers even if their configuration and image haven't changed.
         :param no_build: Don't build an image, even if it's missing.
-        :param build: Build images before creating containers.
+        :param no_recreate: If containers already exist, don't recreate them. Incompatible with --force-recreate.
+        :param pull: Pull image before running ("always"|"missing"|"never") (default "missing")
+        :param remove_orphans: Remove containers for services not defined in the Compose file.
+        :param scale: Scale SERVICE to NUM instances. Overrides the scale setting in the Compose file if present.
         """
         runner = docker_composer.runner.cmd.create.DockerComposeCreate(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def down(
         self,
-        rmi: Optional[str] = None,
-        volumes: Optional[bool] = None,
         remove_orphans: Optional[bool] = None,
+        rmi: Optional[str] = None,
         timeout: Optional[int] = None,
+        volumes: Optional[list] = None,
     ) -> docker_composer.runner.cmd.down.DockerComposeDown:
         """
-        Stops containers and removes containers, networks, volumes, and images
-        created by `up`.
-
-        By default, the only things removed are:
+        Usage:  docker compose down [OPTIONS]
+        Stop and remove containers, networks
 
-        - Containers for services defined in the Compose file
-        - Networks defined in the `networks` section of the Compose file
-        - The default network, if one is used
-
-        Networks and volumes defined as `external` are never removed.
-
-        Usage: down [options]
-
-
-        :param rmi: Remove images. Type must be one of:
-           'all': Remove all images used by any service.
-           'local': Remove only images that don't have a
-           custom tag set by the `image` field.
-        :param volumes: Remove named volumes declared in the `volumes`
-           section of the Compose file and anonymous volumes
-           attached to containers.
-        :param remove_orphans: Remove containers for services not defined in the
-           Compose file
-        :param timeout: Specify a shutdown timeout in seconds.
-           (default: 10)
+        :param remove_orphans: Remove containers for services not defined in the Compose file.
+        :param rmi: Remove images used by services. "local" remove only images that don't have a custom tag ("local"|"all")
+        :param timeout: Specify a shutdown timeout in seconds (default 10)
+        :param volumes: Remove named volumes declared in the volumes section of the Compose file and anonymous volumes attached to containers.
         """
         runner = docker_composer.runner.cmd.down.DockerComposeDown(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def events(
         self, json: Optional[bool] = None
     ) -> docker_composer.runner.cmd.events.DockerComposeEvents:
         """
+        Usage:  docker compose events [OPTIONS] [SERVICE...]
         Receive real time events from containers.
 
-        Usage: events [options] [SERVICE...]
-
-
         :param json: Output events as a stream of json objects
         """
         runner = docker_composer.runner.cmd.events.DockerComposeEvents(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def exec(
         self,
         detach: Optional[bool] = None,
+        env: Optional[list] = None,
+        index: Optional[int] = None,
+        no_TTY: Optional[bool] = None,
         privileged: Optional[bool] = None,
         user: Optional[str] = None,
-        T: Optional[bool] = None,
-        index: Optional[int] = None,
-        env: Optional[dict] = None,
         workdir: Optional[str] = None,
     ) -> docker_composer.runner.cmd.exec.DockerComposeExec:
         """
-        Execute a command in a running container
-
-        Usage: exec [options] [-e KEY=VAL...] SERVICE COMMAND [ARGS...]
-
+        Usage:  docker compose exec [OPTIONS] SERVICE COMMAND [ARGS...]
+        Execute a command in a running container.
 
         :param detach: Detached mode: Run command in the background.
+        :param env: Set environment variables
+        :param index: index of the container if there are multiple instances of a service [default: 1]. (default 1)
+        :param no_TTY: Disable pseudo-TTY allocation. By default docker compose exec allocates a TTY. (default true)
         :param privileged: Give extended privileges to the process.
         :param user: Run the command as this user.
-        :param T: Disable pseudo-tty allocation. By default `docker-compose exec`
-           allocates a TTY.
-        :param index: index of the container if there are multiple
-           instances of a service [default: 1]
-        :param env: not supported in API < 1.25)
         :param workdir: Path to workdir directory for this command.
         """
         runner = docker_composer.runner.cmd.exec.DockerComposeExec(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
-    def help(
-        self,
-    ) -> docker_composer.runner.cmd.help.DockerComposeHelp:
-        """
-        Get help on a command.
-
-        Usage: help [COMMAND]
-
-
-
-        """
-        runner = docker_composer.runner.cmd.help.DockerComposeHelp(
-            **{k: v for k, v in locals().items() if k != "self"}
-        )
-        runner._parent_cmd = self._call_cmd()
-        return runner
-
     def images(
-        self, quiet: Optional[bool] = None
+        self, format: Optional[str] = None, quiet: Optional[bool] = None
     ) -> docker_composer.runner.cmd.images.DockerComposeImages:
         """
-        List images used by the created containers.
-        Usage: images [options] [SERVICE...]
-
+        Usage:  docker compose images [OPTIONS] [SERVICE...]
+        List images used by the created containers
 
+        :param format: Format the output. Values: [table | json]. (default "table")
         :param quiet: Only display IDs
         """
         runner = docker_composer.runner.cmd.images.DockerComposeImages(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def kill(
-        self, s: Optional[int] = None
+        self, remove_orphans: Optional[bool] = None, signal: Optional[str] = None
     ) -> docker_composer.runner.cmd.kill.DockerComposeKill:
         """
+        Usage:  docker compose kill [OPTIONS] [SERVICE...]
         Force stop service containers.
 
-        Usage: kill [options] [SERVICE...]
-
-
-        :param s: SIGNAL to send to the container.
-           Default signal is SIGKILL.
+        :param remove_orphans: Remove containers for services not defined in the Compose file.
+        :param signal: SIGNAL to send to the container. (default "SIGKILL")
         """
         runner = docker_composer.runner.cmd.kill.DockerComposeKill(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def logs(
         self,
-        no_color: Optional[bool] = None,
         follow: Optional[bool] = None,
-        timestamps: Optional[bool] = None,
+        no_color: Optional[bool] = None,
+        no_log_prefix: Optional[bool] = None,
+        since: Optional[str] = None,
         tail: Optional[str] = None,
+        timestamps: Optional[bool] = None,
+        until: Optional[str] = None,
     ) -> docker_composer.runner.cmd.logs.DockerComposeLogs:
         """
-        View output from containers.
-
-        Usage: logs [options] [SERVICE...]
-
+        Usage:  docker compose logs [OPTIONS] [SERVICE...]
+        View output from containers
 
-        :param no_color: Produce monochrome output.
         :param follow: Follow log output.
+        :param no_color: Produce monochrome output.
+        :param no_log_prefix: Don't print prefix in logs.
+        :param since: Show logs since timestamp (e.g. 2013-01-02T13:23:37Z) or relative (e.g. 42m for 42 minutes)
+        :param tail: Number of lines to show from the end of the logs for each container. (default "all")
         :param timestamps: Show timestamps.
-        :param tail: Number of lines to show from the end of the logs
-           for each container.
+        :param until: Show logs before a timestamp (e.g. 2013-01-02T13:23:37Z) or relative (e.g. 42m for 42 minutes)
         """
         runner = docker_composer.runner.cmd.logs.DockerComposeLogs(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
-    def pause(
+    def ls(
         self,
-    ) -> docker_composer.runner.cmd.pause.DockerComposePause:
+        all: Optional[bool] = None,
+        filter: Optional[str] = None,
+        format: Optional[str] = None,
+        quiet: Optional[bool] = None,
+    ) -> docker_composer.runner.cmd.ls.DockerComposeLs:
         """
-        Pause services.
+        Usage:  docker compose ls [OPTIONS]
+        List running compose projects
 
-        Usage: pause [SERVICE...]
+        :param all: Show all stopped Compose projects
+        :param filter: Filter output based on conditions provided.
+        :param format: Format the output. Values: [table | json]. (default "table")
+        :param quiet: Only display IDs.
+        """
+        runner = docker_composer.runner.cmd.ls.DockerComposeLs(
+            **{k: v for k, v in locals().items() if k != "self"}
+        )
+        runner._parent_cmd = self._call_cmd()
+        return runner
 
+    def pause(
+        self,
+    ) -> docker_composer.runner.cmd.pause.DockerComposePause:
+        """
+        Usage:  docker compose pause [SERVICE...]
+        Pause services
 
 
         """
         runner = docker_composer.runner.cmd.pause.DockerComposePause(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def port(
-        self, protocol: Optional[str] = None, index: Optional[int] = None
+        self, index: Optional[int] = None, protocol: Optional[str] = None
     ) -> docker_composer.runner.cmd.port.DockerComposePort:
         """
+        Usage:  docker compose port [OPTIONS] SERVICE PRIVATE_PORT
         Print the public port for a port binding.
 
-        Usage: port [options] SERVICE PRIVATE_PORT
-
-
-        :param protocol: tcp or udp [default: tcp]
-        :param index: index of the container if there are multiple
-           instances of a service [default: 1]
+        :param index: index of the container if service has multiple replicas (default 1)
+        :param protocol: tcp or udp (default "tcp")
         """
         runner = docker_composer.runner.cmd.port.DockerComposePort(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def ps(
         self,
+        all: Optional[bool] = None,
+        filter: Optional[str] = None,
+        format: Optional[str] = None,
         quiet: Optional[bool] = None,
         services: Optional[bool] = None,
-        filter: Optional[dict] = None,
-        all: Optional[bool] = None,
+        status: Optional[list] = None,
     ) -> docker_composer.runner.cmd.ps.DockerComposePs:
         """
-        List containers.
-
-        Usage: ps [options] [SERVICE...]
-
+        Usage:  docker compose ps [OPTIONS] [SERVICE...]
+        List containers
 
+        :param all: Show all stopped containers (including those created by the run command)
+        :param filter: Filter services by a property (supported filters: status).
+        :param format: Format the output. Values: [table | json] (default "table")
         :param quiet: Only display IDs
         :param services: Display services
-        :param filter: Filter services by a property
-        :param all: Show all stopped containers (including those created by the run command)
+        :param status: Filter services by status. Values: [paused | restarting | removing | running | dead | created | exited]
         """
         runner = docker_composer.runner.cmd.ps.DockerComposePs(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def pull(
         self,
+        ignore_buildable: Optional[bool] = None,
         ignore_pull_failures: Optional[bool] = None,
-        parallel: Optional[bool] = None,
-        no_parallel: Optional[bool] = None,
-        quiet: Optional[bool] = None,
         include_deps: Optional[bool] = None,
+        quiet: Optional[bool] = None,
     ) -> docker_composer.runner.cmd.pull.DockerComposePull:
         """
-        Pulls images for services defined in a Compose file, but does not start the containers.
-
-        Usage: pull [options] [SERVICE...]
-
+        Usage:  docker compose pull [OPTIONS] [SERVICE...]
+        Pull service images
 
+        :param ignore_buildable: Ignore images that can be built.
         :param ignore_pull_failures: Pull what it can and ignores images with pull failures.
-        :param parallel: Deprecated, pull multiple images in parallel (enabled by default).
-        :param no_parallel: Disable parallel pulling.
-        :param quiet: Pull without printing progress information
-        :param include_deps: Also pull services declared as dependencies
+        :param include_deps: Also pull services declared as dependencies.
+        :param quiet: Pull without printing progress information.
         """
         runner = docker_composer.runner.cmd.pull.DockerComposePull(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def push(
-        self, ignore_push_failures: Optional[bool] = None
+        self,
+        ignore_push_failures: Optional[bool] = None,
+        include_deps: Optional[bool] = None,
+        quiet: Optional[bool] = None,
     ) -> docker_composer.runner.cmd.push.DockerComposePush:
         """
-        Pushes images for services.
-
-        Usage: push [options] [SERVICE...]
-
+        Usage:  docker compose push [OPTIONS] [SERVICE...]
+        Push service images
 
-        :param ignore_push_failures: Push what it can and ignores images with push failures.
+        :param ignore_push_failures: Push what it can and ignores images with push failures
+        :param include_deps: Also push images of services declared as dependencies
+        :param quiet: Push without printing progress information
         """
         runner = docker_composer.runner.cmd.push.DockerComposePush(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def restart(
-        self, timeout: Optional[int] = None
+        self, no_deps: Optional[bool] = None, timeout: Optional[int] = None
     ) -> docker_composer.runner.cmd.restart.DockerComposeRestart:
         """
-        Restart running containers.
-
-        Usage: restart [options] [SERVICE...]
-
+        Usage:  docker compose restart [OPTIONS] [SERVICE...]
+        Restart service containers
 
-        :param timeout: Specify a shutdown timeout in seconds.
-           (default: 10)
+        :param no_deps: Don't restart dependent services.
+        :param timeout: Specify a shutdown timeout in seconds (default 10)
         """
         runner = docker_composer.runner.cmd.restart.DockerComposeRestart(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def rm(
         self,
         force: Optional[bool] = None,
         stop: Optional[bool] = None,
-        v: Optional[bool] = None,
-        all: Optional[bool] = None,
+        volumes: Optional[bool] = None,
     ) -> docker_composer.runner.cmd.rm.DockerComposeRm:
         """
-        Removes stopped service containers.
-
+        Usage:  docker compose rm [OPTIONS] [SERVICE...]
+        Removes stopped service containers
         By default, anonymous volumes attached to containers will not be removed. You
-        can override this with `-v`. To list all volumes, use `docker volume ls`.
-
+        can override this with -v. To list all volumes, use "docker volume ls".
         Any data which is not in a volume will be lost.
 
-        Usage: rm [options] [SERVICE...]
-
-
         :param force: Don't ask to confirm removal
         :param stop: Stop the containers, if required, before removing
-        :param v: Remove any anonymous volumes attached to containers
-        :param all: Deprecated - no effect.
+        :param volumes: Remove any anonymous volumes attached to containers
         """
         runner = docker_composer.runner.cmd.rm.DockerComposeRm(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def run(
         self,
+        build: Optional[bool] = None,
         detach: Optional[bool] = None,
-        name: Optional[str] = None,
         entrypoint: Optional[str] = None,
-        e: Optional[dict] = None,
-        label: Optional[dict] = None,
-        user: Optional[str] = None,
+        env: Optional[list] = None,
+        interactive: Optional[bool] = None,
+        label: Optional[list] = None,
+        name: Optional[str] = None,
+        no_TTY: Optional[bool] = None,
         no_deps: Optional[bool] = None,
-        rm: Optional[bool] = None,
         publish: Optional[list] = None,
+        quiet_pull: Optional[bool] = None,
+        remove_orphans: Optional[bool] = None,
+        rm: Optional[bool] = None,
         service_ports: Optional[bool] = None,
         use_aliases: Optional[bool] = None,
+        user: Optional[str] = None,
         volume: Optional[list] = None,
-        T: Optional[bool] = None,
         workdir: Optional[str] = None,
     ) -> docker_composer.runner.cmd.run.DockerComposeRun:
         """
+        Usage:  docker compose run [OPTIONS] SERVICE [COMMAND] [ARGS...]
         Run a one-off command on a service.
 
-        For example:
-
-            $ docker-compose run web python manage.py shell
-
-        By default, linked services will be started, unless they are already
-        running. If you do not want to start linked services, use
-        `docker-compose run --no-deps SERVICE COMMAND [ARGS...]`.
-
-            run [options] [-v VOLUME...] [-p PORT...] [-e KEY=VAL...] [-l KEY=VALUE...]
-                SERVICE [COMMAND] [ARGS...]
-
-        :param detach: Detached mode: Run container in the background, print
-           new container name.
+        :param build: Build image before starting container.
+        :param detach: Run container in background and print container ID
+        :param entrypoint: Override the entrypoint of the image
+        :param env: Set environment variables
+        :param interactive: Keep STDIN open even if not attached. (default true)
+        :param label: Add or override a label
         :param name: Assign a name to the container
-        :param entrypoint: Override the entrypoint of the image.
-        :param e: Set an environment variable (can be used multiple times)
-        :param label: Add or override a label (can be used multiple times)
-        :param user: Run as specified username or uid
+        :param no_TTY: Disable pseudo-TTY allocation (default: auto-detected). (default true)
         :param no_deps: Don't start linked services.
-        :param rm: Remove container after run. Ignored in detached mode.
-        :param publish: Publish a container's port(s) to the host
-        :param service_ports: Run command with the service's ports enabled and mapped
-           to the host.
-        :param use_aliases: Use the service's network aliases in the network(s) the
-           container connects to.
-        :param volume: Bind mount a volume (default [])
-        :param T: Disable pseudo-tty allocation. By default `docker-compose run`
-           allocates a TTY.
+        :param publish: Publish a container's port(s) to the host.
+        :param quiet_pull: Pull without printing progress information.
+        :param remove_orphans: Remove containers for services not defined in the Compose file.
+        :param rm: Automatically remove the container when it exits
+        :param service_ports: Run command with the service's ports enabled and mapped to the host.
+        :param use_aliases: Use the service's network useAliases in the network(s) the container connects to.
+        :param user: Run as specified username or uid
+        :param volume: Bind mount a volume.
         :param workdir: Working directory inside the container
         """
         runner = docker_composer.runner.cmd.run.DockerComposeRun(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
-    def scale(
-        self, timeout: Optional[int] = None
-    ) -> docker_composer.runner.cmd.scale.DockerComposeScale:
-        """
-        Set number of containers to run for a service.
-
-        Numbers are specified in the form `service=num` as arguments.
-        For example:
-
-            $ docker-compose scale web=2 worker=3
-
-        This command is deprecated. Use the up command with the `--scale` flag
-        instead.
-
-        Usage: scale [options] [SERVICE=NUM...]
-
-
-        :param timeout: Specify a shutdown timeout in seconds.
-           (default: 10)
-        """
-        runner = docker_composer.runner.cmd.scale.DockerComposeScale(
-            **{k: v for k, v in locals().items() if k != "self"}
-        )
-        runner._parent_cmd = self._call_cmd()
-        return runner
-
     def start(
         self,
     ) -> docker_composer.runner.cmd.start.DockerComposeStart:
         """
-        Start existing containers.
-
-        Usage: start [SERVICE...]
-
+        Usage:  docker compose start [SERVICE...]
+        Start services
 
 
         """
         runner = docker_composer.runner.cmd.start.DockerComposeStart(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def stop(
         self, timeout: Optional[int] = None
     ) -> docker_composer.runner.cmd.stop.DockerComposeStop:
         """
-        Stop running containers without removing them.
-
-        They can be started again with `docker-compose start`.
+        Usage:  docker compose stop [OPTIONS] [SERVICE...]
+        Stop services
 
-        Usage: stop [options] [SERVICE...]
-
-
-        :param timeout: Specify a shutdown timeout in seconds.
-           (default: 10)
+        :param timeout: Specify a shutdown timeout in seconds (default 10)
         """
         runner = docker_composer.runner.cmd.stop.DockerComposeStop(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def top(
         self,
     ) -> docker_composer.runner.cmd.top.DockerComposeTop:
         """
+        Usage:  docker compose top [SERVICES...]
         Display the running processes
 
-        Usage: top [SERVICE...]
-
-
 
         """
         runner = docker_composer.runner.cmd.top.DockerComposeTop(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def unpause(
         self,
     ) -> docker_composer.runner.cmd.unpause.DockerComposeUnpause:
         """
-        Unpause services.
-
-        Usage: unpause [SERVICE...]
-
+        Usage:  docker compose unpause [SERVICE...]
+        Unpause services
 
 
         """
         runner = docker_composer.runner.cmd.unpause.DockerComposeUnpause(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def up(
         self,
+        abort_on_container_exit: Optional[bool] = None,
+        always_recreate_deps: Optional[bool] = None,
+        attach: Optional[list] = None,
+        attach_dependencies: Optional[bool] = None,
+        build: Optional[bool] = None,
         detach: Optional[bool] = None,
+        exit_code_from: Optional[str] = None,
+        force_recreate: Optional[bool] = None,
+        no_attach: Optional[list] = None,
+        no_build: Optional[bool] = None,
         no_color: Optional[bool] = None,
-        quiet_pull: Optional[bool] = None,
         no_deps: Optional[bool] = None,
-        force_recreate: Optional[bool] = None,
-        always_recreate_deps: Optional[bool] = None,
+        no_log_prefix: Optional[bool] = None,
         no_recreate: Optional[bool] = None,
-        no_build: Optional[bool] = None,
         no_start: Optional[bool] = None,
-        build: Optional[bool] = None,
-        abort_on_container_exit: Optional[bool] = None,
-        timeout: Optional[int] = None,
-        renew_anon_volumes: Optional[bool] = None,
+        pull: Optional[str] = None,
+        quiet_pull: Optional[bool] = None,
         remove_orphans: Optional[bool] = None,
-        exit_code_from: Optional[str] = None,
-        scale: Optional[dict] = None,
+        renew_anon_volumes: Optional[bool] = None,
+        scale: Optional[str] = None,
+        timestamps: Optional[bool] = None,
+        wait: Optional[bool] = None,
+        wait_timeout: Optional[int] = None,
+        waitTimeout: Optional[int] = None,
     ) -> docker_composer.runner.cmd.up.DockerComposeUp:
         """
-        Builds, (re)creates, starts, and attaches to containers for a service.
-
-        Unless they are already running, this command also starts any linked services.
-
-        The `docker-compose up` command aggregates the output of each container. When
-        the command exits, all containers are stopped. Running `docker-compose up -d`
-        starts the containers in the background and leaves them running.
+        Usage:  docker compose up [OPTIONS] [SERVICE...]
+        Create and start containers
 
-        If there are existing containers for a service, and the service's configuration
-        or image was changed after the container's creation, `docker-compose up` picks
-        up the changes by stopping and recreating the containers (preserving mounted
-        volumes). To prevent Compose from picking up changes, use the `--no-recreate`
-        flag.
-
-        If you want to force Compose to stop and recreate all containers, use the
-        `--force-recreate` flag.
-
-        Usage: up [options] [--scale SERVICE=NUM...] [SERVICE...]
-
-
-        :param detach: Detached mode: Run containers in the background,
-           print new container names. Incompatible with
-           --abort-on-container-exit.
+        :param abort_on_container_exit: Stops all containers if any container was stopped. Incompatible with -d
+        :param always_recreate_deps: Recreate dependent containers. Incompatible with --no-recreate.
+        :param attach: Attach to service output.
+        :param attach_dependencies: Attach to dependent containers.
+        :param build: Build images before starting containers.
+        :param detach: Detached mode: Run containers in the background
+        :param exit_code_from: Return the exit code of the selected service container. Implies --abort-on-container-exit
+        :param force_recreate: Recreate containers even if their configuration and image haven't changed.
+        :param no_attach: Don't attach to specified service.
+        :param no_build: Don't build an image, even if it's missing.
         :param no_color: Produce monochrome output.
-        :param quiet_pull: Pull without printing progress information
         :param no_deps: Don't start linked services.
-        :param force_recreate: Recreate containers even if their configuration
-           and image haven't changed.
-        :param always_recreate_deps: Recreate dependent containers.
-           Incompatible with --no-recreate.
-        :param no_recreate: If containers already exist, don't recreate
-           them. Incompatible with --force-recreate and -V.
-        :param no_build: Don't build an image, even if it's missing.
+        :param no_log_prefix: Don't print prefix in logs.
+        :param no_recreate: If containers already exist, don't recreate them. Incompatible with --force-recreate.
         :param no_start: Don't start the services after creating them.
-        :param build: Build images before starting containers.
-        :param abort_on_container_exit: Stops all containers if any container was
-           stopped. Incompatible with -d.
-        :param timeout: Use this timeout in seconds for container
-           shutdown when attached or when containers are
-           already running. (default: 10)
-        :param renew_anon_volumes: Recreate anonymous volumes instead of retrieving
-           data from the previous containers.
-        :param remove_orphans: Remove containers for services not defined
-           in the Compose file.
-        :param exit_code_from: Return the exit code of the selected service
-           container. Implies --abort-on-container-exit.
-        :param scale: Scale SERVICE to NUM instances. Overrides the
-           `scale` setting in the Compose file if present.
+        :param pull: Pull image before running ("always"|"missing"|"never") (default "missing")
+        :param quiet_pull: Pull without printing progress information.
+        :param remove_orphans: Remove containers for services not defined in the Compose file.
+        :param renew_anon_volumes: Recreate anonymous volumes instead of retrieving data from the previous containers.
+        :param scale: Scale SERVICE to NUM instances. Overrides the scale setting in the Compose file if present.
+        :param timestamps: Show timestamps.
+        :param wait: Wait for services to be running|healthy. Implies detached mode.
+        :param wait_timeout: timeout waiting for application to be running|healthy.
+        :param waitTimeout: Use this waitTimeout in seconds for container shutdown when attached or when containers are already running. (default 10)
         """
         runner = docker_composer.runner.cmd.up.DockerComposeUp(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def version(
-        self, short: Optional[bool] = None
+        self, format: Optional[str] = None, short: Optional[bool] = None
     ) -> docker_composer.runner.cmd.version.DockerComposeVersion:
         """
-        Show version information
-
-        Usage: version [--short]
-
+        Usage:  docker compose version [OPTIONS]
+        Show the Docker Compose version information
 
+        :param format: Format the output. Values: [pretty | json]. (Default: pretty)
         :param short: Shows only Compose's version number.
         """
         runner = docker_composer.runner.cmd.version.DockerComposeVersion(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
```

### Comparing `docker-composer-0.8.5/setup.py` & `docker_composer-2.17.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,85 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: docker-composer
+Version: 2.17.0
+Summary: Use docker-compose from within Python
+Home-page: https://github.com/schollm/docker-composer
+License: Apache-2.0
+Author: Micha
+Author-email: schollm-git@gmx.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Requires-Dist: attrs (>=20.3.0)
+Requires-Dist: loguru (>=0.5.3)
+Project-URL: Repository, https://github.com/schollm/docker-composer
+Description-Content-Type: text/markdown
+
+# Docker Composer
+A library to interact with `docker-compose` from a python Program.
+All commands and parameters are exposed as python classes and attributes
+to allow for full auto-completion of its parameters with IDEs
+that support it.
+
+
+## Install
+```shell script
+pip install docker-composer
+```
+
+## Usage
+The main class is `docker_composer.DockerCompose`. Its parameters are
+all options from `docker-compose`.
+ 
+Each `docker-compose` command has a corresponding function, e.g. 
+`DockerCompose.run` or `DockerCompose.scale`. Their arguments again mirror 
+the options of the corresponding command.
+
+The resulting object has a `call` function. 
+It takes arbitrary strings as input, as well as all keyword arguments from 
+`subprocess.run`, and returns a `subprocess.CompletedProcess`
+
+```python
+from docker_composer import DockerCompose
+
+
+base = DockerCompose(file="docker-compose.yml", verbose=True)
+base.run(detach=True, workdir="/tmp").call("app")
+base.run(workdir="/tmp").call("app", "/bin/bash", "-l")
+
+# /tmp $ ls /.dockerenv
+# /.dockerenv
+# /tmp $ exit
+
+process = base.ps(all=True).call(capture_output=True)
+print(process.stdout.encode("UTF-8"))
+#          Name                      Command           State    Ports
+# -------------------------------------------------------------------
+# myapp_app_70fd8b786b76   myapp --start-server        Exit 0        
+# myapp_app_6ac3db4e1b55   myapp --client              Exit 0   
+```
+
+## Develop
+
+### Coding Standards
+
+| **Type**       | Package  | Comment                         |
+| -------------- | -------- | ------------------------------- |
+| **Linter**     | `black`  | Also for auto-formatted modules |
+| **Logging**    | `loguru` |                                 |
+| **Packaging**  | `poetry` |                                 |
+| **Tests**      | `pytest` |                                 |
+| **Typing**     | `mypy`   | Type all methods                |
+| **Imports**    | `isort`  |                                 |
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['docker_composer',
- 'docker_composer._utils',
- 'docker_composer.runner',
- 'docker_composer.runner.cmd']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['attrs>=20.3.0,<21.0.0', 'loguru>=0.5.3,<0.6.0']
-
-setup_kwargs = {
-    'name': 'docker-composer',
-    'version': '0.8.5',
-    'description': 'Use docker-compose from within Python',
-    'long_description': '# Docker Composer\nA library to interact with `docker-compose` from a python Program.\nAll commands and parameters are exposed as python classes and attributes\nto allow for full auto-completion of its parameters with IDEs\nthat support it.\n\n\n## Install\n```shell script\npip install docker-composer\n```\n\n## Usage\nThe main class is `docker_composer.DockerCompose`. Its parameters are\nall options from `docker-compose`.\n \nEach `docker-compose` command has a corresponding function, e.g. \n`DockerCompose.run` or `DockerCompose.scale`. Their arguments again mirror \nthe options of the corresponding command.\n\nThe resulting object has a `call` function. \nIt takes arbitrary strings as input, as well as all keyword arguments from \n`subprocess.run`, and returns a `subprocess.CompletedProcess`\n\n```python\nfrom docker_composer import DockerCompose\n\n\nbase = DockerCompose(file="docker-compose.yml", verbose=True)\nbase.run(detach=True, workdir="/tmp").call("app")\nbase.run(workdir="/tmp").call("app", "/bin/bash", "-l")\n\n# /tmp $ ls /.dockerenv\n# /.dockerenv\n# /tmp $ exit\n\nprocess = base.ps(all=True).call(capture_output=True)\nprint(process.stdout.encode("UTF-8"))\n#          Name                      Command           State    Ports\n# -------------------------------------------------------------------\n# myapp_app_70fd8b786b76   myapp --start-server        Exit 0        \n# myapp_app_6ac3db4e1b55   myapp --client              Exit 0   \n```\n\n## Develop\n\n### Coding Standards\n\n| **Type**       | Package  | Comment                         |\n| -------------- | -------- | ------------------------------- |\n| **Linter**     | `black`  | Also for auto-formatted modules |\n| **Logging**    | `loguru` |                                 |\n| **Packaging**  | `poetry` |                                 |\n| **Tests**      | `pytest` |                                 |\n| **Typing**     | `mypy`   | Type all methods                |\n| **Imports**    | `isort`  |                                 |\n',
-    'author': 'Micha',
-    'author_email': 'schollm-git@gmx.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/schollm/docker-composer',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

