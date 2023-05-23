# Comparing `tmp/sidetrek-0.0.81.tar.gz` & `tmp/sidetrek-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sidetrek-0.0.81.tar", max compression
+gzip compressed data, was "sidetrek-0.0.9.tar", max compression
```

## Comparing `sidetrek-0.0.81.tar` & `sidetrek-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,18 @@
--rw-r--r--   0        0        0       27 2023-03-09 16:33:17.090578 sidetrek-0.0.81/README.md
--rw-r--r--   0        0        0      776 2023-05-23 01:53:01.764782 sidetrek-0.0.81/pyproject.toml
--rw-r--r--   0        0        0      604 2023-05-21 17:56:16.028060 sidetrek-0.0.81/sidetrek/__init__.py
--rw-r--r--   0        0        0     1609 2023-05-23 01:24:18.459454 sidetrek-0.0.81/sidetrek/cli.py
--rw-r--r--   0        0        0        0 2023-03-13 16:42:41.918418 sidetrek-0.0.81/sidetrek/cli_commands/__init__.py
--rw-r--r--   0        0        0      174 2023-03-14 03:00:43.940526 sidetrek-0.0.81/sidetrek/cli_commands/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      388 2023-03-30 16:36:26.685225 sidetrek-0.0.81/sidetrek/cli_commands/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0     8815 2023-04-06 20:18:36.881239 sidetrek-0.0.81/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc
--rw-r--r--   0        0        0     2395 2023-04-06 20:18:55.453228 sidetrek-0.0.81/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0      161 2023-05-21 20:54:49.328467 sidetrek-0.0.81/sidetrek/cli_commands/constants.py
--rw-r--r--   0        0        0    10668 2023-05-21 21:04:05.995911 sidetrek-0.0.81/sidetrek/cli_commands/helpers.py
--rw-r--r--   0        0        0     3471 2023-05-23 01:52:59.164219 sidetrek-0.0.81/sidetrek/cli_commands/workflow.py
--rw-r--r--   0        0        0       37 2023-04-02 20:04:34.987724 sidetrek-0.0.81/sidetrek/constants.py
--rw-r--r--   0        0        0     1114 2023-05-03 16:51:33.053983 sidetrek-0.0.81/sidetrek/datapipes.py
--rw-r--r--   0        0        0     4317 2023-05-22 17:35:27.418133 sidetrek-0.0.81/sidetrek/dataset.py
--rw-r--r--   0        0        0       15 2023-05-03 16:06:32.112969 sidetrek-0.0.81/sidetrek/flyte/__init__.py
--rw-r--r--   0        0        0      874 2023-05-09 03:56:32.928519 sidetrek-0.0.81/sidetrek/global_fns.py
--rw-r--r--   0        0        0      661 2023-04-09 00:09:05.853814 sidetrek-0.0.81/sidetrek/loggers.py
--rw-r--r--   0        0        0        0 2023-05-07 17:03:01.499766 sidetrek-0.0.81/sidetrek/types/__init__.py
--rw-r--r--   0        0        0      642 2023-05-22 15:17:38.985798 sidetrek-0.0.81/sidetrek/types/dataset.py
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 sidetrek-0.0.81/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-03-09 16:33:17.090578 sidetrek-0.0.9/README.md
+-rw-r--r--   0        0        0      689 2023-04-09 00:09:19.420892 sidetrek-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      558 2023-04-08 23:51:45.364985 sidetrek-0.0.9/sidetrek/__init__.py
+-rw-r--r--   0        0        0     1607 2023-03-30 15:37:18.710028 sidetrek-0.0.9/sidetrek/cli.py
+-rw-r--r--   0        0        0        0 2023-03-13 16:42:41.918418 sidetrek-0.0.9/sidetrek/cli_commands/__init__.py
+-rw-r--r--   0        0        0      174 2023-03-14 03:00:43.940526 sidetrek-0.0.9/sidetrek/cli_commands/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      388 2023-03-30 16:36:26.685225 sidetrek-0.0.9/sidetrek/cli_commands/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0     8815 2023-04-06 20:18:36.881239 sidetrek-0.0.9/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc
+-rw-r--r--   0        0        0     2395 2023-04-06 20:18:55.453228 sidetrek-0.0.9/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0      244 2023-03-30 16:14:08.795493 sidetrek-0.0.9/sidetrek/cli_commands/constants.py
+-rw-r--r--   0        0        0     9970 2023-04-06 20:18:33.249911 sidetrek-0.0.9/sidetrek/cli_commands/helpers.py
+-rw-r--r--   0        0        0     3115 2023-04-06 20:19:34.857751 sidetrek-0.0.9/sidetrek/cli_commands/workflow.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:08:56.569055 sidetrek-0.0.9/sidetrek/core/__init__.py
+-rw-r--r--   0        0        0       37 2023-04-02 20:04:34.987724 sidetrek-0.0.9/sidetrek/core/constants.py
+-rw-r--r--   0        0        0      491 2023-04-08 23:51:25.980013 sidetrek-0.0.9/sidetrek/core/global_fns.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:09:01.575253 sidetrek-0.0.9/sidetrek/loggers/__init__.py
+-rw-r--r--   0        0        0      661 2023-04-09 00:09:05.853814 sidetrek-0.0.9/sidetrek/loggers/loggers.py
+-rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 sidetrek-0.0.9/PKG-INFO
```

### Comparing `sidetrek-0.0.81/pyproject.toml` & `sidetrek-0.0.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 [tool.poetry]
 name = "sidetrek"
-version = "0.0.81"
+version = "0.0.9"
 description = ""
 authors = ["Seungchan Lee <seunggs@gmail.com>"]
 readme = "README.md"
 exclude = ["sidetrek/test/**"]
 
 [tool.poetry.scripts]
 sidetrek = "sidetrek.cli:app"
 
 [tool.poetry.dependencies]
-python = "^3.8,<3.12"
+python = "^3.10,<3.11"
 typer = {extras = ["all"], version = "^0.7.0"}
 numba = "^0.56.4" # Required for mlflow: mlflow depends on old version of numba which won't install via poetry, so we had to manually include it here
-mlflow = "^2.0"
-flytekit = "^1.2.10,<=1.4.2"
+mlflow = "^2.2.1"
+flytekit = "<=1.4.2"
 requests = "^2.28.2"
 pylint = "^2.17.0"
-torchdata = "^0.6.0"
-fsspec = "^2023.4.0"
-s3fs = "^2023.4.0"
-bentoml = "^1.0.20"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `sidetrek-0.0.81/sidetrek/__init__.py` & `sidetrek-0.0.9/sidetrek/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-from sidetrek.loggers import logger
-from sidetrek.global_fns import *
-
-
-__all__ = ["dataset", "types", "flyte", "cli_commands"]
-
+from sidetrek.loggers.loggers import logger
+from sidetrek.core.global_fns import *
 
 __doc__ = """
 sidetrek
 ================
 
 Description
 -----------
```

### Comparing `sidetrek-0.0.81/sidetrek/cli.py` & `sidetrek-0.0.9/sidetrek/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import json
 from pathlib import Path
 import pickle
 import requests
 import typer
 from rich import print
-from sidetrek.cli_commands import workflow
-from sidetrek.cli_commands.constants import APP_NAME
-from sidetrek.cli_commands.helpers import get_node_env, get_auth_api_base_url
+from cli_commands import workflow
+from cli_commands.constants import NODE_ENV, APP_NAME
+from cli_commands.helpers import get_auth_api_base_url
 
 app = typer.Typer()
 
 app.add_typer(workflow.app, name="workflow")
 
-if get_node_env() != "production":
-    print(f"Environment: {get_node_env()}\n")
+# if NODE_ENV == 'development':
+#     print(f"Environment: {NODE_ENV}\n")
+print(f"Environment: {NODE_ENV}\n")
 
 
 @app.command()
 def login(email: str = typer.Option(..., prompt=True), password: str = typer.Option(..., prompt=True, hide_input=True)):
     # Login and get refresh/access tokens
     try:
         auth_api_base_url = get_auth_api_base_url()
```

### Comparing `sidetrek-0.0.81/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc` & `sidetrek-0.0.9/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.81/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc` & `sidetrek-0.0.9/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.81/sidetrek/cli_commands/helpers.py` & `sidetrek-0.0.9/sidetrek/cli_commands/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,19 @@
-import os
 import json
 import time
 import threading
 from pathlib import Path
 import shutil
 import urllib.parse
 import io
 from zipfile import ZipFile
 import typer
 from rich import print
 import requests
-from sidetrek.cli_commands.constants import APP_NAME, GENERATED_LOCAL_SIDETREK_DIRNAME, GENERATED_PROJECT_DIRNAME
-
-
-def get_node_env():
-    if os.environ.get("NODE_ENV") == "development":
-        return "development"
-    elif os.environ.get("NODE_ENV") == "staging":
-        return "staging"
-    else:
-        return "production"
+from cli_commands.constants import NODE_ENV, APP_NAME, GENERATED_LOCAL_SIDETREK_DIRNAME, GENERATED_PROJECT_DIRNAME
 
 
 def print_timer(seconds: int = 1):
     start_time = time.time()
 
     def loop():
         while True:
@@ -32,41 +22,23 @@
             elapsed_time = current_time - start_time
             print(f"\r{elapsed_time} seconds...")
 
     threading.Thread(target=loop).start()
 
 
 def get_auth_api_base_url():
-    node_env = get_node_env()
-    if node_env == "development":
-        return f"http://localhost:4002/api/v1"
-    elif node_env == "staging":
-        return f"https://auth-staging.sidetrek.com/api/v1"
-    else:
-        return f"https://auth.sidetrek.com/api/v1"
+    return f"http://localhost:4002/api/v1" if NODE_ENV == "development" else f"https://auth.sidetrek.com/api/v1"
 
 
 def get_user_machine_node_api_base_url(user_id):
-    node_env = get_node_env()
-    if node_env == "development":
-        return f"http://localhost:4008/p/api/v1"
-    elif node_env == "staging":
-        return f"https://user-machines.sidetrek.com/{user_id}/node/p/api/v1"
-    else:
-        return f"https://user-machines.sidetrek.com/{user_id}/node/p/api/v1"
+    return f"http://localhost:4008/p/api/v1" if NODE_ENV == "development" else f"https://user-machines.sidetrek.com/{user_id}/node/p/api/v1"
 
 
 def get_webapp_api_base_url():
-    node_env = get_node_env()
-    if node_env == "development":
-        return f"http://localhost:4001/p/app/api/v1"
-    elif node_env == "staging":
-        return f"https://app-staging.sidetrek.com/p/app/api/v1"
-    else:
-        return f"https://app.sidetrek.com/p/app/api/v1"
+    return f"http://localhost:4001/p/app/api/v1" if NODE_ENV == "development" else f"https://app.sidetrek.com/p/app/api/v1"
 
 
 def get_generated_local_sidetrek_dir_path() -> Path:
     app_dir = typer.get_app_dir(APP_NAME)
     generated_local_sidetrek_dir_path = Path(app_dir) / GENERATED_LOCAL_SIDETREK_DIRNAME
     Path(generated_local_sidetrek_dir_path).mkdir(parents=True, exist_ok=True)
     return generated_local_sidetrek_dir_path
```

### Comparing `sidetrek-0.0.81/sidetrek/cli_commands/workflow.py` & `sidetrek-0.0.9/sidetrek/cli_commands/workflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import threading
 from pathlib import Path
 import typer
 import subprocess
 from time import sleep
 from rich import print
 from rich.progress import Progress, SpinnerColumn, TextColumn
-from sidetrek.cli_commands.helpers import (
+from cli_commands.helpers import (
     get_current_user,
     get_generated_local_sidetrek_dir_path,
     get_generated_workflow_name,
     download_generated_flyte_workflow,
     get_workflow_draft_version,
     print_timer,
 )
@@ -20,67 +20,60 @@
 
 
 @app.command()
 def run(workflow_id: int = typer.Option(...), workflow_args: str = "{}"):
     """
     Execute the workflow locally (e.g. for testing).
 
-    * You can retrieve the --workflow-id (e.g. 42) from Sidetrek app.
-    * Workflow version used it always `draft` for this command
-    * --workflow-args is a stringified JSON of your workflow arguments (e.g. '{"learning_rate"=0.1, "epochs"=5}').
+    You can retrieve the --workflow-id (e.g. 42) from Sidetrek app.
+    --workflow-args is a stringified JSON of your workflow arguments (e.g. '{"learning_rate"=0.1, "epochs"=5}').
     """
-    start_time = time.time()
 
     with Progress(
         SpinnerColumn(),
         TextColumn("[progress.description]{task.description}"),
         transient=True,
     ) as progress:
         print("generated_local_sidetrek_dir_path", get_generated_local_sidetrek_dir_path())
-
+        
         # # Add a timer
         # print_timer()
-
+        
         # Get current user
         auth_step = progress.add_task(description="Authenticating...", total=None)
         current_user = get_current_user()
         progress.remove_task(auth_step)
-        time_elapsed = round(time.time() - start_time, 2)
-        print(f"[green]✔️ [white]Authenticated [grey89]({time_elapsed}s)")
+        print(f"[green]✔️ [white]Authenticated")
 
         # Always use the draft version for testing
         wf_generation_step = progress.add_task(description="Generating the workflow...", total=None)
         workflow_version = get_workflow_draft_version(workflow_id=workflow_id)
         # print(f"workflow_version={workflow_version}")
 
         # Generate the workflow file
         wf_file_path = download_generated_flyte_workflow(user_id=current_user["id"], workflow_version=workflow_version)
         generated_wf_name = get_generated_workflow_name(workflow_id)
         progress.remove_task(wf_generation_step)
-        time_elapsed = round(time.time() - start_time, 2)
-        print(f"[green]✔️ [white]Workflow generated [grey89]({time_elapsed}s)")
-        print(f"Generated workflow file: {wf_file_path.as_posix()}")
+        print(f"[green]✔️ [white]Workflow generated")
 
         wf_execution_step = progress.add_task(description="Executing the workflow...", total=None)
-        # print(" ".join(["pyflyte", "run", wf_file_path.as_posix(), generated_wf_name, "--_wf_args", workflow_args]))
         with subprocess.Popen(
+            # ["pyflyte", "--pkgs", "project", "package", "--output", "flyte-workflow-package.tgz", "--image", "gcr.io/sidetrek/tylo-birch1-development/wf-22:0.0.39", "--force"],
             ["pyflyte", "run", wf_file_path, generated_wf_name, "--_wf_args", workflow_args],
             cwd=get_generated_local_sidetrek_dir_path(),
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
-            bufsize=1,
-            universal_newlines=True,
         ) as process:
-            for line in process.stdout:
-                print(line, end="")
-
-            _, error = process.communicate()
-
-            if process.returncode != 0:
-                time_elapsed = round(time.time() - start_time, 2)
-                print(f"[light_coral]{error}")
-                print(f"[red]✕ [white]Workflow execution failed [grey89]({time_elapsed}s)")
+            output, error = process.communicate()
+            
+            if process.returncode != 0: 
+                print(f"[light_coral]{error.decode('utf-8')}")
+                print(f"[red]✕ [white]Workflow execution failed")
                 raise typer.Exit()
-
+            
+            print(f"[green]{output.decode('utf-8')}")
+            
             progress.remove_task(wf_execution_step)
-            time_elapsed = round(time.time() - start_time, 2)
-            print(f"[green]✔️ [white]Workflow execution completed 🎉 [grey89]({time_elapsed}s)")
+            print(f"[green]✔️ [white]Workflow execution completed 🎉")
+            # while process.poll() == None:
+            #     print(f"{process.stdout.read1().decode('utf-8')}")
+
```

### Comparing `sidetrek-0.0.81/sidetrek/loggers.py` & `sidetrek-0.0.9/sidetrek/loggers/loggers.py`

 * *Files identical despite different names*

