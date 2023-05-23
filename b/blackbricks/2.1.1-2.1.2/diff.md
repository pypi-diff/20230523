# Comparing `tmp/blackbricks-2.1.1.tar.gz` & `tmp/blackbricks-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackbricks-2.1.1.tar", max compression
+gzip compressed data, was "blackbricks-2.1.2.tar", max compression
```

## Comparing `blackbricks-2.1.1.tar` & `blackbricks-2.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1086 2023-04-26 10:42:31.846279 blackbricks-2.1.1/LICENSE
--rw-r--r--   0        0        0    11881 2023-04-26 10:42:31.846279 blackbricks-2.1.1/README.md
--rw-r--r--   0        0        0       22 2023-04-26 10:42:31.846279 blackbricks-2.1.1/blackbricks/__init__.py
--rw-r--r--   0        0        0     4561 2023-04-26 10:42:31.846279 blackbricks-2.1.1/blackbricks/blackbricks.py
--rw-r--r--   0        0        0     6512 2023-04-26 10:42:31.846279 blackbricks-2.1.1/blackbricks/cli.py
--rw-r--r--   0        0        0     5430 2023-04-26 10:42:31.846279 blackbricks-2.1.1/blackbricks/databricks_sync.py
--rw-r--r--   0        0        0     4355 2023-04-26 10:42:31.846279 blackbricks-2.1.1/blackbricks/files.py
--rw-r--r--   0        0        0     1585 2023-04-26 10:42:31.846279 blackbricks-2.1.1/pyproject.toml
--rw-r--r--   0        0        0    13265 1970-01-01 00:00:00.000000 blackbricks-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-05-23 12:01:08.318061 blackbricks-2.1.2/LICENSE
+-rw-r--r--   0        0        0    11881 2023-05-23 12:01:08.318061 blackbricks-2.1.2/README.md
+-rw-r--r--   0        0        0       22 2023-05-23 12:01:08.318061 blackbricks-2.1.2/blackbricks/__init__.py
+-rw-r--r--   0        0        0     4561 2023-05-23 12:01:08.318061 blackbricks-2.1.2/blackbricks/blackbricks.py
+-rw-r--r--   0        0        0     6512 2023-05-23 12:01:08.318061 blackbricks-2.1.2/blackbricks/cli.py
+-rw-r--r--   0        0        0     5430 2023-05-23 12:01:08.318061 blackbricks-2.1.2/blackbricks/databricks_sync.py
+-rw-r--r--   0        0        0     4355 2023-05-23 12:01:08.318061 blackbricks-2.1.2/blackbricks/files.py
+-rw-r--r--   0        0        0     1585 2023-05-23 12:01:08.318061 blackbricks-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0    13114 1970-01-01 00:00:00.000000 blackbricks-2.1.2/PKG-INFO
```

### Comparing `blackbricks-2.1.1/LICENSE` & `blackbricks-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `blackbricks-2.1.1/README.md` & `blackbricks-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `blackbricks-2.1.1/blackbricks/blackbricks.py` & `blackbricks-2.1.2/blackbricks/blackbricks.py`

 * *Files identical despite different names*

### Comparing `blackbricks-2.1.1/blackbricks/cli.py` & `blackbricks-2.1.2/blackbricks/cli.py`

 * *Files identical despite different names*

### Comparing `blackbricks-2.1.1/blackbricks/databricks_sync.py` & `blackbricks-2.1.2/blackbricks/databricks_sync.py`

 * *Files identical despite different names*

### Comparing `blackbricks-2.1.1/blackbricks/files.py` & `blackbricks-2.1.2/blackbricks/files.py`

 * *Files identical despite different names*

### Comparing `blackbricks-2.1.1/pyproject.toml` & `blackbricks-2.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blackbricks"
-version = "2.1.1"
+version = "2.1.2"
 description = "Black for Databricks notebooks"
 authors = ["Bendik Samseth <bendik.samseth@inspera.no>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/inspera/blackbricks"
 keywords = [
     "automation",
@@ -47,15 +47,15 @@
 flake8 = "^3.9.2"
 commitizen = "^2.32.2"
 mypy = "^0.971"
 
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "2.1.1"
+version = "2.1.2"
 tag_format = "$version"
 version_files = ["blackbricks/__init__.py:version", "pyproject.toml:version"]
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
```

### Comparing `blackbricks-2.1.1/PKG-INFO` & `blackbricks-2.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackbricks
-Version: 2.1.1
+Version: 2.1.2
 Summary: Black for Databricks notebooks
 Home-page: https://github.com/inspera/blackbricks
 License: MIT
 Keywords: automation,formatter,black,sql,yapf,autopep8,pyfmt,gofmt,rustfmt
 Author: Bendik Samseth
 Author-email: bendik.samseth@inspera.no
 Requires-Python: >=3.8,<4.0
@@ -16,17 +16,14 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Dist: black (>=23.1.0,<24.0.0)
 Requires-Dist: databricks-cli (>=0.17.3,<0.18.0)
 Requires-Dist: sqlparse (>=0.4.2,<0.5.0)
 Requires-Dist: typer[all] (>=0.6.1,<0.8)
 Project-URL: Repository, https://github.com/inspera/blackbricks
 Description-Content-Type: text/markdown
```

