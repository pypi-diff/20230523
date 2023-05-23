# Comparing `tmp/muffin-0.97.2.tar.gz` & `tmp/muffin-0.98.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin-0.97.2.tar", max compression
+gzip compressed data, was "muffin-0.98.0.tar", max compression
```

## Comparing `muffin-0.97.2.tar` & `muffin-0.98.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     9874 2023-04-11 12:30:09.537730 muffin-0.97.2/README.rst
--rw-r--r--   0        0        0      982 2023-04-11 12:30:09.537730 muffin-0.97.2/muffin/__init__.py
--rw-r--r--   0        0        0     5130 2023-04-11 12:30:09.537730 muffin-0.97.2/muffin/app.py
--rw-r--r--   0        0        0       71 2023-04-11 12:30:09.537730 muffin-0.97.2/muffin/constants.py
--rw-r--r--   0        0        0      701 2023-04-11 12:30:09.537730 muffin-0.97.2/muffin/errors.py
--rw-r--r--   0        0        0     3754 2023-04-11 12:30:09.537730 muffin-0.97.2/muffin/handler.py
--rw-r--r--   0        0        0     8805 2023-04-11 12:30:09.537730 muffin-0.97.2/muffin/manage.py
--rw-r--r--   0        0        0     2857 2023-04-11 12:30:09.541730 muffin-0.97.2/muffin/plugins.py
--rw-r--r--   0        0        0        0 2023-04-11 12:30:09.541730 muffin-0.97.2/muffin/py.typed
--rw-r--r--   0        0        0     2705 2023-04-11 12:30:09.541730 muffin-0.97.2/muffin/pytest.py
--rw-r--r--   0        0        0      153 2023-04-11 12:30:09.541730 muffin-0.97.2/muffin/types.py
--rw-r--r--   0        0        0     2449 2023-04-11 12:30:09.541730 muffin-0.97.2/muffin/utils.py
--rw-r--r--   0        0        0     3038 2023-04-11 12:30:09.541730 muffin-0.97.2/pyproject.toml
--rw-r--r--   0        0        0    11614 1970-01-01 00:00:00.000000 muffin-0.97.2/PKG-INFO
+-rw-r--r--   0        0        0     9874 2023-05-23 08:03:28.922982 muffin-0.98.0/README.rst
+-rw-r--r--   0        0        0      982 2023-05-23 08:03:28.922982 muffin-0.98.0/muffin/__init__.py
+-rw-r--r--   0        0        0     5250 2023-05-23 08:03:28.922982 muffin-0.98.0/muffin/app.py
+-rw-r--r--   0        0        0       71 2023-05-23 08:03:28.922982 muffin-0.98.0/muffin/constants.py
+-rw-r--r--   0        0        0      701 2023-05-23 08:03:28.922982 muffin-0.98.0/muffin/errors.py
+-rw-r--r--   0        0        0     3754 2023-05-23 08:03:28.922982 muffin-0.98.0/muffin/handler.py
+-rw-r--r--   0        0        0     8805 2023-05-23 08:03:28.922982 muffin-0.98.0/muffin/manage.py
+-rw-r--r--   0        0        0     2857 2023-05-23 08:03:28.922982 muffin-0.98.0/muffin/plugins.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:03:28.922982 muffin-0.98.0/muffin/py.typed
+-rw-r--r--   0        0        0     2705 2023-05-23 08:03:28.926982 muffin-0.98.0/muffin/pytest.py
+-rw-r--r--   0        0        0      153 2023-05-23 08:03:28.926982 muffin-0.98.0/muffin/types.py
+-rw-r--r--   0        0        0     2584 2023-05-23 08:03:28.926982 muffin-0.98.0/muffin/utils.py
+-rw-r--r--   0        0        0     2990 2023-05-23 08:03:28.926982 muffin-0.98.0/pyproject.toml
+-rw-r--r--   0        0        0    11329 1970-01-01 00:00:00.000000 muffin-0.98.0/PKG-INFO
```

### Comparing `muffin-0.97.2/README.rst` & `muffin-0.98.0/README.rst`

 * *Files identical despite different names*

### Comparing `muffin-0.97.2/muffin/__init__.py` & `muffin-0.98.0/muffin/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin-0.97.2/muffin/app.py` & `muffin-0.98.0/muffin/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,31 +110,34 @@
         """Support background tasks."""
         await self.lifespan(scope, receive, send)
         bgtasks = BACKGROUND_TASK.get()
         if bgtasks is not None:
             await aio_wait(*bgtasks)
             BACKGROUND_TASK.set(None)
 
-    def import_submodules(self, *submodules: str):
+    def import_submodules(self, *submodules: str, silent: bool = False):
         """Automatically import submodules.
 
         .. code-block:: python
 
             # Somewhere in package "__init__.py" file
 
             # import all submodules
             app.import_submodules()
 
             # import only specific submodules (in specified order)
             app.import_submodules('submodule1', 'submodule2')
 
+            # ignore import errors
+            app.import_submodules(silent=True)
+
         """
         parent_frame = stack()[1][0]
         package_name = parent_frame.f_locals["__name__"]
-        return import_submodules(package_name, *submodules)
+        return import_submodules(package_name, *submodules, silent=silent)
 
     def run_after_response(self, *tasks: Awaitable):
         """Await the given awaitable after the response is completed.
 
         .. code-block:: python
 
             from muffin import Application
```

### Comparing `muffin-0.97.2/muffin/errors.py` & `muffin-0.98.0/muffin/errors.py`

 * *Files identical despite different names*

### Comparing `muffin-0.97.2/muffin/handler.py` & `muffin-0.98.0/muffin/handler.py`

 * *Files identical despite different names*

### Comparing `muffin-0.97.2/muffin/manage.py` & `muffin-0.98.0/muffin/manage.py`

 * *Files identical despite different names*

### Comparing `muffin-0.97.2/muffin/plugins.py` & `muffin-0.98.0/muffin/plugins.py`

 * *Files identical despite different names*

### Comparing `muffin-0.97.2/muffin/pytest.py` & `muffin-0.98.0/muffin/pytest.py`

 * *Files identical despite different names*

### Comparing `muffin-0.97.2/muffin/utils.py` & `muffin-0.98.0/muffin/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -68,23 +68,30 @@
     AIOLIB.current = aiolib = AIOLIB.current or aio_lib()
     if aiolib == "asyncio":
         return asyncio.run(corofn(*args, **kwargs))
 
     return AIOLIBS[aiolib].run(lambda: corofn(*args, **kwargs))
 
 
-def import_submodules(package_name: str, *module_names: str) -> Dict[str, ModuleType]:
-    """Import all submodules by package name."""
+def import_submodules(
+    package_name: str, *module_names: str, silent: bool = False
+) -> Dict[str, ModuleType]:
+    """Import all submodules by the given package name."""
     package = sys.modules[package_name]
-    return {
-        module_name: importlib.import_module(f"{package_name}.{module_name}")
-        for module_name in (
-            module_names or (name for _, name, _ in pkgutil.walk_packages(package.__path__))
-        )
-    }
+    res = {}
+    for module_name in module_names or (
+        name for _, name, _ in pkgutil.walk_packages(package.__path__)
+    ):
+        try:
+            res[module_name] = importlib.import_module(f"{package_name}.{module_name}")
+        except ImportError:
+            if not silent:
+                raise
+
+    return res
 
 
 def import_app(app_uri: str, *, reload: bool = False) -> Application:
     """Import application by the given string (python.path.to.module:app_name)."""
     mod_name, _, app_name = app_uri.partition(":")
     mod = importlib.import_module(mod_name)
     if reload:
```

### Comparing `muffin-0.97.2/pyproject.toml` & `muffin-0.98.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin"
-version = "0.97.2"
+version = "0.98.0"
 description = "Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)"
 readme = "README.rst"
 license = "MIT"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 keywords = ["asgi", "web", "web framework", "asyncio", "trio", "curio"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
@@ -20,71 +20,71 @@
   "Topic :: Internet :: WWW/HTTP",
   "Framework :: AsyncIO",
   "Framework :: Trio",
 ]
 homepage = "https://github.com/klen/muffin"
 repository = "https://github.com/klen/muffin"
 documentation = "https://klen.github.io/muffin"
-packages = [{include = "muffin"}]
+packages = [{ include = "muffin" }]
 
 [tool.poetry.urls]
 changelog = "https://raw.githubusercontent.com/klen/muffin/master/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-asgi-tools = "^0.73.2"
-modconfig = "^1.2.1"
-ujson = "^5.7.0"
+asgi-tools = "^0"
+modconfig = "^1"
+ujson = "*"
 
 # Optional
-gunicorn = {version = "^20.1.0", optional = true}
-uvicorn = {version = "^0.21.1", optional = true, extras = ["standard"]}
+gunicorn = { version = "^20.1.0", optional = true }
+uvicorn = { version = "^0.21.1", optional = true, extras = ["standard"] }
 
 [tool.poetry.scripts]
 muffin = "muffin.manage:cli"
 
 [tool.poetry.plugins]
 pytest11 = { muffin_pytest = "muffin.pytest" }
 
 [tool.poetry.extras]
 standard = ["gunicorn", "uvicorn"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-aiofile = "^3.8.5"
-pytest = "^7.2.2"
-pytest-mypy = "^0.10.3"
-ruff = "^0.0.258"
-pytest-aio = {extras = ["curio", "trio"], version = "^1.5.0"}
-pre-commit = "^3.2.0"
+aiofile = "*"
+pytest = "*"
+pytest-mypy = "*"
+ruff = "*"
+pytest-aio = { extras = ["curio", "trio"], version = "*" }
+pre-commit = "*"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^6.1.3"
-pydata-sphinx-theme = "^0.13.1"
-sphinx-copybutton = "^0.5.1"
+sphinx = "*"
+pydata-sphinx-theme = "*"
+sphinx-copybutton = "*"
 
 [tool.pytest.ini_options]
 addopts = "-xsvl"
 muffin_app = "tests:app"
 
 [tool.mypy]
 packages = ["muffin"]
 ignore_missing_imports = true
 
 [tool.ruff]
 line-length = 100
 target-version = "py38"
 exclude = [".venv", "docs", "example"]
 select = ["ALL"]
-ignore = ["D", "UP", "ANN", "DJ", "EM", "RSE", "SLF", "RET", "S101", "PLR2004", "N804"]
+ignore = ["D", "UP", "ANN", "DJ", "EM", "RSE", "SLF", "RET", "S101", "PLR2004", "N804", "COM"]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["ARG", "TRY", "F", "PGH", "PLR", "PLW", "PTH", "SIM", "RET504", "T20"]
 
 [tool.black]
 line-length = 100
 target-version = ["py38", "py39", "py310", "py311"]
```

### Comparing `muffin-0.97.2/PKG-INFO` & `muffin-0.98.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin
-Version: 0.97.2
+Version: 0.98.0
 Summary: Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)
 Home-page: https://github.com/klen/muffin
 License: MIT
 Keywords: asgi,web,web framework,asyncio,trio,curio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -15,26 +15,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP
 Provides-Extra: standard
-Requires-Dist: asgi-tools (>=0.73.2,<0.74.0)
+Requires-Dist: asgi-tools (>=0,<1)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0) ; extra == "standard"
-Requires-Dist: modconfig (>=1.2.1,<2.0.0)
-Requires-Dist: ujson (>=5.7.0,<6.0.0)
+Requires-Dist: modconfig (>=1,<2)
+Requires-Dist: ujson
 Requires-Dist: uvicorn[standard] (>=0.21.1,<0.22.0) ; extra == "standard"
 Project-URL: Documentation, https://klen.github.io/muffin
 Project-URL: Repository, https://github.com/klen/muffin
 Project-URL: changelog, https://raw.githubusercontent.com/klen/muffin/master/CHANGELOG.md
 Description-Content-Type: text/x-rst
 
 .. image:: https://raw.github.com/klen/muffin/develop/docs/static/logo-h200.png
```

