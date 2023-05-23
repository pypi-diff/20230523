# Comparing `tmp/giup-1.1.4.tar.gz` & `tmp/giup-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giup-1.1.4.tar", max compression
+gzip compressed data, was "giup-1.1.5.tar", max compression
```

## Comparing `giup-1.1.4.tar` & `giup-1.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0    11558 2021-01-31 22:52:26.563141 giup-1.1.4/LICENSE
--rwxr-xr-x   0        0        0     2655 2021-01-31 23:04:48.331614 giup-1.1.4/README.md
--rwxr-xr-x   0        0        0        0 2023-05-13 00:41:43.507705 giup-1.1.4/giup/__init__.py
--rwxr-xr-x   0        0        0     2805 2023-05-13 15:10:47.846943 giup-1.1.4/giup/cli.py
--rwxr-xr-x   0        0        0     5368 2023-05-13 12:00:22.923550 giup-1.1.4/giup/command.py
--rwxr-xr-x   0        0        0     1745 2023-05-13 01:02:56.311788 giup-1.1.4/giup/git.py
--rwxr-xr-x   0        0        0     6633 2023-05-13 15:11:32.223538 giup-1.1.4/giup/project.py
--rwxr-xr-x   0        0        0     2078 2023-05-13 10:45:22.366835 giup-1.1.4/giup/util.py
--rwxr-xr-x   0        0        0     1473 2023-05-13 15:12:32.568229 giup-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     3782 1970-01-01 00:00:00.000000 giup-1.1.4/PKG-INFO
+-rwxr-xr-x   0        0        0    11558 2021-01-31 22:52:26.563141 giup-1.1.5/LICENSE
+-rwxr-xr-x   0        0        0     2655 2021-01-31 23:04:48.331614 giup-1.1.5/README.md
+-rwxr-xr-x   0        0        0        0 2023-05-13 00:41:43.507705 giup-1.1.5/giup/__init__.py
+-rwxr-xr-x   0        0        0     3157 2023-05-23 16:55:20.839987 giup-1.1.5/giup/cli.py
+-rwxr-xr-x   0        0        0     5368 2023-05-13 12:00:22.923550 giup-1.1.5/giup/command.py
+-rwxr-xr-x   0        0        0     1886 2023-05-23 16:50:42.766135 giup-1.1.5/giup/git.py
+-rwxr-xr-x   0        0        0     6945 2023-05-23 16:53:16.891403 giup-1.1.5/giup/project.py
+-rwxr-xr-x   0        0        0     2078 2023-05-13 10:45:22.366835 giup-1.1.5/giup/util.py
+-rwxr-xr-x   0        0        0     1473 2023-05-23 16:56:52.308425 giup-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3782 1970-01-01 00:00:00.000000 giup-1.1.5/PKG-INFO
```

### Comparing `giup-1.1.4/LICENSE` & `giup-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `giup-1.1.4/README.md` & `giup-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `giup-1.1.4/giup/cli.py` & `giup-1.1.5/giup/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,14 +68,26 @@
     parser.add_argument(
         "--no-commands",
         action="store_true",
         default=False,
         help="Don't run any commands",
     )
     parser.add_argument(
+        "--no-return",
+        action="store_true",
+        default=False,
+        help="Don't return to the original branch after running",
+    )
+    parser.add_argument(
+        "-e", "--edit-commit-message",
+        action="store_true",
+        default=False,
+        help="Edit the commit message before committing",
+    )
+    parser.add_argument(
         "-v", "--version",
         action="version",
         version=importlib.metadata.version("giup"),
     )
 
     args = parser.parse_args()
```

### Comparing `giup-1.1.4/giup/command.py` & `giup-1.1.5/giup/command.py`

 * *Files identical despite different names*

### Comparing `giup-1.1.4/giup/git.py` & `giup-1.1.5/giup/git.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,10 +47,12 @@
 
 
 async def switch(branch_name: str):
     if await async_run_command_result("git switch --quiet " + shlex.quote(branch_name)):
         raise GitBranchError(branch_name)
 
 
-async def merge(branch_name: str):
-    if await async_run_command_result("git merge " + shlex.quote(branch_name)):
+async def merge(branch_name: str, edit_commit_message: bool = False):
+    merge_opts = "" if edit_commit_message else "--no-edit"
+    branch_name = shlex.quote(branch_name)
+    if await async_run_command_result(f"git merge {merge_opts} -- {branch_name}"):
         raise GitBranchError(branch_name)
```

### Comparing `giup-1.1.4/giup/project.py` & `giup-1.1.5/giup/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,17 @@
     def __init__(self):
         pass
 
     async def run_commands(self):
         for command in self._commands:
             await command.run(self.fail_on_error)
 
-    async def run(self):
+    async def run(self,
+                  return_to_original_branch: bool = True,
+                  edit_commit_message: bool = False):
         original_branch = await git.get_current_branch()
         i = 0
         for merge_path in self.merge_paths:
             cprint(f"> Following merge path #{i}: {' -> '.join(merge_path)}", color="blue")
             i += 1
             # noinspection PyBroadException
             try:
@@ -57,31 +59,35 @@
 
                 else:
                     last_branch = merge_path[0]
                     branches = merge_path[1::]
                     for branch in branches:
                         await Command(git.switch, branch, title="Switching to branch \"" + branch + "\"")\
                             .run(self.fail_on_error)
-                        await Command(git.merge, last_branch, title="Merging parent branch \"" + last_branch + "\"")\
+                        await Command(git.merge,
+                                      last_branch,
+                                      edit_commit_message=edit_commit_message,
+                                      title="Merging parent branch \"" + last_branch + "\"")\
                             .run(self.fail_on_error)
                         last_branch = branch
                         await self.run_commands()
 
             except util.GiupPathAbort:
                 cprint("Aborting current path!", attrs=["bold"], file=sys.stderr)
             except util.GiupStop:
                 cprint("Quitting giup (cancelling all further paths)", attrs=["bold"], file=sys.stderr)
                 break
             except BaseException:
                 cprint(f"Failed to follow merge path!\n{traceback.format_exc()}", color="red", file=sys.stderr)
                 if self.fail_on_error:
                     return
 
-        cprint("> Returning to original branch \"" + original_branch + "\"", color="blue")
-        await git.switch(original_branch)
+        if return_to_original_branch:
+            cprint("> Returning to original branch \"" + original_branch + "\"", color="blue")
+            await git.switch(original_branch)
 
     @staticmethod
     async def _read_merge_path(path_json: Any) -> Optional[List[str]]:
         if type(path_json) == list:
             branches = path_json
         elif type(path_json) == str:
             branches: List[str] = path_json.split("->")
```

### Comparing `giup-1.1.4/giup/util.py` & `giup-1.1.5/giup/util.py`

 * *Files identical despite different names*

### Comparing `giup-1.1.4/pyproject.toml` & `giup-1.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "GIUP"
-version = "1.1.4"
+version = "1.1.5"
 description = "Interactively and hierarchically perform git merges across branches and run commands in between."
 authors = ["Siphalor <info@siphalor.de>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/Siphalor/giup"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `giup-1.1.4/PKG-INFO` & `giup-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giup
-Version: 1.1.4
+Version: 1.1.5
 Summary: Interactively and hierarchically perform git merges across branches and run commands in between.
 Home-page: https://github.com/Siphalor/giup
 License: Apache-2.0
 Author: Siphalor
 Author-email: info@siphalor.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

