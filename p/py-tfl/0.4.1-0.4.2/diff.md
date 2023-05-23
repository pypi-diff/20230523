# Comparing `tmp/py_tfl-0.4.1.tar.gz` & `tmp/py_tfl-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_tfl-0.4.1.tar", max compression
+gzip compressed data, was "py_tfl-0.4.2.tar", max compression
```

## Comparing `py_tfl-0.4.1.tar` & `py_tfl-0.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1068 2023-05-16 19:08:53.668645 py_tfl-0.4.1/LICENSE
--rw-r--r--   0        0        0     4409 2023-05-16 19:08:53.668645 py_tfl-0.4.1/README.md
--rw-r--r--   0        0        0     2347 2023-05-16 19:08:53.668645 py_tfl-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      128 2023-05-16 19:08:53.668645 py_tfl-0.4.1/tfl/__init__.py
--rw-r--r--   0        0        0       68 2023-05-16 19:08:53.668645 py_tfl-0.4.1/tfl/cli/__init__.py
--rw-r--r--   0        0        0     1345 2023-05-16 19:08:53.668645 py_tfl-0.4.1/tfl/cli/_async_typer.py
--rw-r--r--   0        0        0     2930 2023-05-16 19:08:53.668645 py_tfl-0.4.1/tfl/cli/main.py
--rw-r--r--   0        0        0        0 2023-05-16 19:08:53.668645 py_tfl-0.4.1/tfl/cli/py.typed
--rw-r--r--   0        0        0      415 2023-05-16 19:08:53.668645 py_tfl-0.4.1/tfl/clients/__init__.py
--rw-r--r--   0        0        0     4650 2023-05-16 19:08:53.668645 py_tfl-0.4.1/tfl/clients/_accident_stats_client.py
--rw-r--r--   0        0        0     4484 2023-05-16 19:08:53.668645 py_tfl-0.4.1/tfl/clients/_air_quality_client.py
--rw-r--r--   0        0        0     1696 2023-05-16 19:08:53.668645 py_tfl-0.4.1/tfl/clients/_auth.py
--rw-r--r--   0        0        0     5000 2023-05-16 19:08:53.668645 py_tfl-0.4.1/tfl/clients/_client.py
--rw-r--r--   0        0        0     4913 2023-05-16 19:08:53.668645 py_tfl-0.4.1/tfl/clients/_crowding_client.py
--rw-r--r--   0        0        0     4463 2023-05-16 19:08:53.668645 py_tfl-0.4.1/tfl/clients/_lift_disruptions_client.py
--rw-r--r--   0        0        0        0 2023-05-16 19:08:53.668645 py_tfl-0.4.1/tfl/clients/py.typed
--rw-r--r--   0        0        0      561 2023-05-16 19:08:53.668645 py_tfl-0.4.1/tfl/enums.py
--rw-r--r--   0        0        0        0 2023-05-16 19:08:53.668645 py_tfl-0.4.1/tfl/py.typed
--rw-r--r--   0        0        0     5583 1970-01-01 00:00:00.000000 py_tfl-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-23 19:26:28.035691 py_tfl-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4409 2023-05-23 19:26:28.035691 py_tfl-0.4.2/README.md
+-rw-r--r--   0        0        0     2347 2023-05-23 19:26:28.035691 py_tfl-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-05-23 19:26:28.039691 py_tfl-0.4.2/tfl/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-23 19:26:28.039691 py_tfl-0.4.2/tfl/cli/__init__.py
+-rw-r--r--   0        0        0     1345 2023-05-23 19:26:28.039691 py_tfl-0.4.2/tfl/cli/_async_typer.py
+-rw-r--r--   0        0        0     2930 2023-05-23 19:26:28.039691 py_tfl-0.4.2/tfl/cli/main.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:26:28.039691 py_tfl-0.4.2/tfl/cli/py.typed
+-rw-r--r--   0        0        0      415 2023-05-23 19:26:28.039691 py_tfl-0.4.2/tfl/clients/__init__.py
+-rw-r--r--   0        0        0     4650 2023-05-23 19:26:28.039691 py_tfl-0.4.2/tfl/clients/_accident_stats_client.py
+-rw-r--r--   0        0        0     4484 2023-05-23 19:26:28.039691 py_tfl-0.4.2/tfl/clients/_air_quality_client.py
+-rw-r--r--   0        0        0     1696 2023-05-23 19:26:28.039691 py_tfl-0.4.2/tfl/clients/_auth.py
+-rw-r--r--   0        0        0     5000 2023-05-23 19:26:28.039691 py_tfl-0.4.2/tfl/clients/_client.py
+-rw-r--r--   0        0        0     4913 2023-05-23 19:26:28.039691 py_tfl-0.4.2/tfl/clients/_crowding_client.py
+-rw-r--r--   0        0        0     4463 2023-05-23 19:26:28.039691 py_tfl-0.4.2/tfl/clients/_lift_disruptions_client.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:26:28.039691 py_tfl-0.4.2/tfl/clients/py.typed
+-rw-r--r--   0        0        0      561 2023-05-23 19:26:28.039691 py_tfl-0.4.2/tfl/enums.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:26:28.039691 py_tfl-0.4.2/tfl/py.typed
+-rw-r--r--   0        0        0     5381 1970-01-01 00:00:00.000000 py_tfl-0.4.2/PKG-INFO
```

### Comparing `py_tfl-0.4.1/LICENSE` & `py_tfl-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_tfl-0.4.1/README.md` & `py_tfl-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `py_tfl-0.4.1/pyproject.toml` & `py_tfl-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "py-tfl"
-version = "0.4.1"
+version = "0.4.2"
 description = "A Python package for the Transport for London (TFL) API."
 authors = ["Cellan Hall <hallcellan@gmail.com>"]
 readme = "README.md"
 packages = [
     {include = "tfl"},
 ]
 homepage = "https://ce11an.github.io/tfl/"
@@ -32,23 +32,23 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 httpx = "~=0.24.0"
 typer = {extras = ["all"], version = "~=0.9.0"}
 
 [tool.poetry.dev-dependencies]
-pre-commit = "~=3.3.1"
+pre-commit = "~=3.3.2"
 black = "~=23.3.0"
 ruff = "~=0.0.267"
 mypy = "~=1.3.0"
 pytest = "~=7.3.1"
 pytest-cov = "~=4.0.0"
 pytest-httpx = "~=0.22.0"
 pytest-asyncio = "~=0.21.0"
-mkdocs-material = "~=9.1.12"
+mkdocs-material = "~=9.1.14"
 mkdocstrings = {extras = ["python"], version = "~=0.21.2"}
 
 [tool.black]
 line-length = 120
 color = true
 
 exclude = '''
```

### Comparing `py_tfl-0.4.1/tfl/cli/_async_typer.py` & `py_tfl-0.4.2/tfl/cli/_async_typer.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.4.1/tfl/cli/main.py` & `py_tfl-0.4.2/tfl/cli/main.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.4.1/tfl/clients/_accident_stats_client.py` & `py_tfl-0.4.2/tfl/clients/_accident_stats_client.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.4.1/tfl/clients/_air_quality_client.py` & `py_tfl-0.4.2/tfl/clients/_air_quality_client.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.4.1/tfl/clients/_auth.py` & `py_tfl-0.4.2/tfl/clients/_auth.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.4.1/tfl/clients/_client.py` & `py_tfl-0.4.2/tfl/clients/_client.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.4.1/tfl/clients/_crowding_client.py` & `py_tfl-0.4.2/tfl/clients/_crowding_client.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.4.1/tfl/clients/_lift_disruptions_client.py` & `py_tfl-0.4.2/tfl/clients/_lift_disruptions_client.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.4.1/tfl/enums.py` & `py_tfl-0.4.2/tfl/enums.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.4.1/PKG-INFO` & `py_tfl-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 Metadata-Version: 2.1
 Name: py-tfl
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Python package for the Transport for London (TFL) API.
 Home-page: https://ce11an.github.io/tfl/
 Author: Cellan Hall
 Author-email: hallcellan@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/Ce11an/tfl
 Description-Content-Type: text/markdown
```

