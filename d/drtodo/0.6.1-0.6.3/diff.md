# Comparing `tmp/drtodo-0.6.1.tar.gz` & `tmp/drtodo-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drtodo-0.6.1.tar", max compression
+gzip compressed data, was "drtodo-0.6.3.tar", max compression
```

## Comparing `drtodo-0.6.1.tar` & `drtodo-0.6.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1064 2023-05-22 16:06:20.808229 drtodo-0.6.1/LICENSE
--rw-r--r--   0        0        0     9777 2023-05-22 16:06:20.808229 drtodo-0.6.1/drtodo/README.md
--rw-r--r--   0        0        0      224 2023-05-22 16:06:20.808229 drtodo-0.6.1/drtodo/__init__.py
--rw-r--r--   0        0        0       44 2023-05-22 16:06:20.808229 drtodo-0.6.1/drtodo/__main__.py
--rw-r--r--   0        0        0    11816 2023-05-22 16:06:20.808229 drtodo-0.6.1/drtodo/main.py
--rw-r--r--   0        0        0     4681 2023-05-22 16:06:20.808229 drtodo-0.6.1/drtodo/man_command.py
--rw-r--r--   0        0        0     4718 2023-05-22 16:06:20.808229 drtodo-0.6.1/drtodo/mdparser.py
--rw-r--r--   0        0        0     1406 2023-05-22 16:06:20.808229 drtodo-0.6.1/drtodo/mistuneplugin.py
--rw-r--r--   0        0        0      618 2023-05-22 16:06:20.808229 drtodo-0.6.1/drtodo/rich_display.py
--rw-r--r--   0        0        0     7052 2023-05-22 16:06:20.808229 drtodo-0.6.1/drtodo/settings.py
--rw-r--r--   0        0        0       11 2023-05-22 16:06:20.808229 drtodo-0.6.1/drtodo/util.py
--rw-r--r--   0        0        0      807 2023-05-22 16:06:34.996262 drtodo-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    10671 1970-01-01 00:00:00.000000 drtodo-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-23 02:51:22.787598 drtodo-0.6.3/LICENSE
+-rw-r--r--   0        0        0     9777 2023-05-23 02:51:22.787598 drtodo-0.6.3/drtodo/README.md
+-rw-r--r--   0        0        0      224 2023-05-23 02:51:22.791598 drtodo-0.6.3/drtodo/__init__.py
+-rw-r--r--   0        0        0       44 2023-05-23 02:51:22.791598 drtodo-0.6.3/drtodo/__main__.py
+-rw-r--r--   0        0        0    11844 2023-05-23 02:51:22.791598 drtodo-0.6.3/drtodo/main.py
+-rw-r--r--   0        0        0     4703 2023-05-23 02:51:22.791598 drtodo-0.6.3/drtodo/man_command.py
+-rw-r--r--   0        0        0     4784 2023-05-23 02:51:22.791598 drtodo-0.6.3/drtodo/mdparser.py
+-rw-r--r--   0        0        0     1406 2023-05-23 02:51:22.791598 drtodo-0.6.3/drtodo/mistuneplugin.py
+-rw-r--r--   0        0        0      618 2023-05-23 02:51:22.791598 drtodo-0.6.3/drtodo/rich_display.py
+-rw-r--r--   0        0        0     7052 2023-05-23 02:51:22.791598 drtodo-0.6.3/drtodo/settings.py
+-rw-r--r--   0        0        0       11 2023-05-23 02:51:22.791598 drtodo-0.6.3/drtodo/util.py
+-rw-r--r--   0        0        0      807 2023-05-23 02:51:34.295809 drtodo-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0    10671 1970-01-01 00:00:00.000000 drtodo-0.6.3/PKG-INFO
```

### Comparing `drtodo-0.6.1/LICENSE` & `drtodo-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.1/drtodo/README.md` & `drtodo-0.6.3/drtodo/README.md`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.1/drtodo/main.py` & `drtodo-0.6.3/drtodo/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .mdparser import TaskListTraverser, TodoListParser
 from .rich_display import console
 from .settings import constants, globals, settings
 
 app = typer.Typer(
     no_args_is_help=True,
     rich_markup_mode="markdown",
-    help="**{constants.appname}, MD**: *a straightforward todo list manager for markdown files in git repos.*",
+    help=f"**{constants.appname}, MD**: *a straightforward todo list manager for markdown files in git repos.*",
     epilog=f"DrTodo can manage items in a global todo list ({globals.global_todofile_pretty})"
     f" and in a local todo list ({globals.local_todofile_pretty or 'if the current folder is under a git repo'})."
     f" Settings are read from config files and env variables (see *todo man config*).",
     rich_help_panel="Integration")
 
 
 def version_string() -> str:
@@ -95,18 +95,18 @@
 
 
 @app.command()
 def debug():
     """
     List configuration, settings, version and other debug info.
     """
-    console().print(f"{version_string()}")
+    console().print(f"{version_string()}", highlight=False)
 
     d = constants.__dict__ | dict(settings) | globals.__dict__
-    console.print(d)
+    console().print(d)
 
 
 def _add_item(todo_item: dict, todofile_path: Path):
     if todofile_path and todofile_path.exists():
         todo = TodoListParser()
         todo.parse(todofile_path)
         # TODO: need to append in the MD file in the right place (once we support sections, etc.)
@@ -129,15 +129,15 @@
 ):
     """
     Add a new todo item to the list
     """
     duestr = f" due:{due}" if due else ""
     ownerstr = f" @{owner}" if owner else ""
     prioritystr = f" P{priority}" if priority else ""
-    itemstr = f"{prioritystr}{ownerstr}{duestr} {description}"
+    itemstr = f"{prioritystr}{ownerstr}{duestr} {description}".strip()
     todo_item = TaskListTraverser.create_item(itemstr, index=0, checked=done)
     if not global_todo and globals.local_todofile and globals.local_todofile.exists():
         console().print(f"[header]{globals.local_todofile_pretty}[text]")
         _add_item(todo_item, globals.local_todofile)
     else:
         console().print(f"[header]{globals.global_todofile_pretty}[text]")
         _add_item(todo_item, globals.global_todofile)
```

### Comparing `drtodo-0.6.1/drtodo/man_command.py` & `drtodo-0.6.3/drtodo/man_command.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typer
 import rich
 import rich.markdown
 from .rich_display import console
 from .settings import constants, get_default_config
 
 
-raw_man_output = False
+man_output = None
 manapp = typer.Typer()
 
 
 def md_mdfiles():
     return f"""
 # Markdown Files
 
@@ -133,36 +133,36 @@
 {get_default_config()}
 ```
 """
 
 
 @manapp.command()
 def mdfiles():
-    md = md_mdfiles()
-    if not raw_man_output:
-        md = rich.markdown.Markdown(md)
-    console().print(md)
+    assert man_output
+    man_output(md_mdfiles())
 
 
 @manapp.command()
 def config():
-    md = md_config()
-    if not raw_man_output:
-        md = rich.markdown.Markdown(md)
-    console().print(md)
+    assert man_output
+    man_output(md_config())
 
 
 @manapp.command()
 def all():
-    md = md_mdfiles() + "\n\n" + md_config()
-    if not raw_man_output:
-        md = rich.markdown.Markdown(md)
-    console().print(md)
+    assert man_output
+    man_output(md_mdfiles() + "\n\n" + md_config())
 
 
+def output_as_raw(mdstring: str):
+    console().print(mdstring, markup=False, highlight=False)
+
+def output_pretty(mdstring: str):
+    console().print(rich.markdown.Markdown(mdstring))
+
 # handle global options
 @manapp.callback()
 def main(
     raw: bool = typer.Option(False, "--raw", help="Print the raw markdown man content"),
 ):
-    global raw_man_output
-    raw_man_output = raw
+    global man_output
+    man_output = output_as_raw if raw else output_pretty
```

### Comparing `drtodo-0.6.1/drtodo/mdparser.py` & `drtodo-0.6.3/drtodo/mdparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     @staticmethod
     def create_item(text, *, index: int, checked: bool = False, token: dict = None) -> dict:
         """
         creates a dict to represent a task list item from text and an index.
         If token is given, it is used, otherwise a new one is created.
         """
-        id = TaskListTraverser.calc_git_hash(text)
+        id = TaskListTraverser.calc_git_hash(text.strip())  # always ignore leading and trailing whitespace for hash
         token = token or TaskListTraverser.create_item_token(checked, text)
         item = {'checked': checked, 'text': text, 'id': id, 'index': index, 'token': token}
         token['task_item'] = item
         return item
 
     @staticmethod
     def create_item_token(checked: bool, text: str) -> dict:
```

### Comparing `drtodo-0.6.1/drtodo/mistuneplugin.py` & `drtodo-0.6.3/drtodo/mistuneplugin.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.1/drtodo/rich_display.py` & `drtodo-0.6.3/drtodo/rich_display.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.1/drtodo/settings.py` & `drtodo-0.6.3/drtodo/settings.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.1/pyproject.toml` & `drtodo-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "DrTodo"
-version = "0.6.1"
+version = "0.6.3"
 description = "DrTodo, MD: todo list manager using markdown files and git"
 authors = ["exilium <info@exilium.com>"]
 readme = "drtodo/README.md"
 license = "MIT"
 repository = "https://github.com/exilium-com/DrTodo"
 keywords = ["utilities", "todo", "markdown"]
```

### Comparing `drtodo-0.6.1/PKG-INFO` & `drtodo-0.6.3/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drtodo
-Version: 0.6.1
+Version: 0.6.3
 Summary: DrTodo, MD: todo list manager using markdown files and git
 Home-page: https://github.com/exilium-com/DrTodo
 License: MIT
 Keywords: utilities,todo,markdown
 Author: exilium
 Author-email: info@exilium.com
 Requires-Python: >=3.9,<4.0
```

