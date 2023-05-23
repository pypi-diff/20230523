# Comparing `tmp/python_opensky-0.0.6.tar.gz` & `tmp/python_opensky-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_opensky-0.0.6.tar", max compression
+gzip compressed data, was "python_opensky-0.0.7.tar", max compression
```

## Comparing `python_opensky-0.0.6.tar` & `python_opensky-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1077 2023-05-08 15:43:19.410883 python_opensky-0.0.6/LICENSE.md
--rw-r--r--   0        0        0     5328 2023-05-08 15:43:19.410883 python_opensky-0.0.6/README.md
--rw-r--r--   0        0        0     3659 2023-05-08 15:43:45.228431 python_opensky-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      444 2023-05-08 15:43:19.414884 python_opensky-0.0.6/src/python_opensky/__init__.py
--rw-r--r--   0        0        0      849 2023-05-08 15:43:19.414884 python_opensky-0.0.6/src/python_opensky/const.py
--rw-r--r--   0        0        0      384 2023-05-08 15:43:19.414884 python_opensky-0.0.6/src/python_opensky/exceptions.py
--rw-r--r--   0        0        0     3573 2023-05-08 15:43:19.414884 python_opensky-0.0.6/src/python_opensky/models.py
--rw-r--r--   0        0        0     7400 2023-05-08 15:43:19.414884 python_opensky-0.0.6/src/python_opensky/opensky.py
--rw-r--r--   0        0        0        0 2023-05-08 15:43:19.414884 python_opensky-0.0.6/src/python_opensky/py.typed
--rw-r--r--   0        0        0     6730 1970-01-01 00:00:00.000000 python_opensky-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-23 20:15:17.557045 python_opensky-0.0.7/LICENSE.md
+-rw-r--r--   0        0        0     5328 2023-05-23 20:15:17.557045 python_opensky-0.0.7/README.md
+-rw-r--r--   0        0        0     3659 2023-05-23 20:15:43.549260 python_opensky-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      444 2023-05-23 20:15:17.557045 python_opensky-0.0.7/src/python_opensky/__init__.py
+-rw-r--r--   0        0        0      849 2023-05-23 20:15:17.557045 python_opensky-0.0.7/src/python_opensky/const.py
+-rw-r--r--   0        0        0      384 2023-05-23 20:15:17.561045 python_opensky-0.0.7/src/python_opensky/exceptions.py
+-rw-r--r--   0        0        0     3573 2023-05-23 20:15:17.561045 python_opensky-0.0.7/src/python_opensky/models.py
+-rw-r--r--   0        0        0    12059 2023-05-23 20:15:17.561045 python_opensky-0.0.7/src/python_opensky/opensky.py
+-rw-r--r--   0        0        0        0 2023-05-23 20:15:17.561045 python_opensky-0.0.7/src/python_opensky/py.typed
+-rw-r--r--   0        0        0     6580 1970-01-01 00:00:00.000000 python_opensky-0.0.7/PKG-INFO
```

### Comparing `python_opensky-0.0.6/LICENSE.md` & `python_opensky-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python_opensky-0.0.6/README.md` & `python_opensky-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `python_opensky-0.0.6/pyproject.toml` & `python_opensky-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python_opensky"
-version = "0.0.6"
+version = "0.0.7"
 description = "Asynchronous Python client for Opensky API."
 authors = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 maintainers = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/joostlek/python-opensky"
 repository = "https://github.com/joostlek/python-opensky"
@@ -33,24 +33,24 @@
 [tool.poetry.group.dev.dependencies]
 aresponses = "2.1.6"
 black = "23.3.0"
 blacken-docs = "1.13.0"
 codespell = "2.2.4"
 covdefaults = "2.3.0"
 coverage = {version = "7.2.5", extras = ["toml"]}
-mypy = "1.2.0"
-pre-commit = "3.3.1"
+mypy = "1.3.0"
+pre-commit = "3.3.2"
 pre-commit-hooks = "4.4.0"
 pylint = "2.17.4"
 pytest = "7.3.1"
 pytest-asyncio = "0.21.0"
 pytest-cov = "4.0.0"
-ruff = "0.0.265"
+ruff = "0.0.269"
 safety = "2.4.0b1"
-yamllint = "1.31.0"
+yamllint = "1.32.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/joostlek/python-opensky/issues"
 Changelog = "https://github.com/joostlek/python-opensky/releases"
 
 [tool.coverage.report]
 show_missing = true
```

### Comparing `python_opensky-0.0.6/src/python_opensky/const.py` & `python_opensky-0.0.7/src/python_opensky/const.py`

 * *Files identical despite different names*

### Comparing `python_opensky-0.0.6/src/python_opensky/models.py` & `python_opensky-0.0.7/src/python_opensky/models.py`

 * *Files identical despite different names*

### Comparing `python_opensky-0.0.6/PKG-INFO` & `python_opensky-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-opensky
-Version: 0.0.6
+Version: 0.0.7
 Summary: Asynchronous Python client for Opensky API.
 Home-page: https://github.com/joostlek/python-opensky
 License: MIT
 Keywords: opensky,api,async,client
 Author: Joost Lekkerkerker
 Author-email: joostlek@outlook.com
 Maintainer: Joost Lekkerkerker
@@ -14,17 +14,14 @@
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.0.0)
 Requires-Dist: pydantic (==1.10.7)
 Requires-Dist: yarl (>=1.6.0)
 Project-URL: Bug Tracker, https://github.com/joostlek/python-opensky/issues
 Project-URL: Changelog, https://github.com/joostlek/python-opensky/releases
 Project-URL: Documentation, https://github.com/joostlek/python-opensky
```

