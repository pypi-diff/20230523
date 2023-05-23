# Comparing `tmp/duckingit-0.0.8.tar.gz` & `tmp/duckingit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckingit-0.0.8.tar", last modified: Mon May 22 17:27:57 2023, max compression
+gzip compressed data, was "duckingit-0.0.9.tar", last modified: Mon May 22 17:41:46 2023, max compression
```

## Comparing `duckingit-0.0.8.tar` & `duckingit-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.059910 duckingit-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 17:27:37.000000 duckingit-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-22 17:27:57.059910 duckingit-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-22 17:27:37.000000 duckingit-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.059910 duckingit-0.0.8/duckingit/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-22 17:27:37.000000 duckingit-0.0.8/duckingit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10266 2023-05-22 17:27:37.000000 duckingit-0.0.8/duckingit/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-05-22 17:27:37.000000 duckingit-0.0.8/duckingit/_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-22 17:27:37.000000 duckingit-0.0.8/duckingit/_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-22 17:27:37.000000 duckingit-0.0.8/duckingit/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-22 17:27:37.000000 duckingit-0.0.8/duckingit/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-05-22 17:27:37.000000 duckingit-0.0.8/duckingit/_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-22 17:27:37.000000 duckingit-0.0.8/duckingit/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-05-22 17:27:37.000000 duckingit-0.0.8/duckingit/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.059910 duckingit-0.0.8/duckingit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-22 17:27:57.000000 duckingit-0.0.8/duckingit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-22 17:27:57.000000 duckingit-0.0.8/duckingit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:27:57.000000 duckingit-0.0.8/duckingit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-22 17:27:57.000000 duckingit-0.0.8/duckingit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 17:27:57.000000 duckingit-0.0.8/duckingit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-22 17:27:37.000000 duckingit-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:27:57.059910 duckingit-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:41:46.090362 duckingit-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 17:41:26.000000 duckingit-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-22 17:41:46.090362 duckingit-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-22 17:41:26.000000 duckingit-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:41:46.090362 duckingit-0.0.9/duckingit/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-22 17:41:26.000000 duckingit-0.0.9/duckingit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10266 2023-05-22 17:41:26.000000 duckingit-0.0.9/duckingit/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-05-22 17:41:26.000000 duckingit-0.0.9/duckingit/_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-22 17:41:26.000000 duckingit-0.0.9/duckingit/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-22 17:41:26.000000 duckingit-0.0.9/duckingit/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-22 17:41:26.000000 duckingit-0.0.9/duckingit/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-05-22 17:41:26.000000 duckingit-0.0.9/duckingit/_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-22 17:41:26.000000 duckingit-0.0.9/duckingit/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-05-22 17:41:26.000000 duckingit-0.0.9/duckingit/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:41:46.090362 duckingit-0.0.9/duckingit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-22 17:41:46.000000 duckingit-0.0.9/duckingit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-22 17:41:46.000000 duckingit-0.0.9/duckingit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:41:46.000000 duckingit-0.0.9/duckingit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 17:41:46.000000 duckingit-0.0.9/duckingit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 17:41:46.000000 duckingit-0.0.9/duckingit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-22 17:41:26.000000 duckingit-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:41:46.090362 duckingit-0.0.9/setup.cfg
```

### Comparing `duckingit-0.0.8/LICENSE` & `duckingit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `duckingit-0.0.8/PKG-INFO` & `duckingit-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckingit
-Version: 0.0.8
+Version: 0.0.9
 Summary: A framework to leverage clusters of serverless functions for analytics. Powered by DuckDB
 Author-email: Tobias Egelund <egelundtobias@gmail.com>
 Project-URL: Homepage, https://github.com/tobiasegelund/duckingit
 Project-URL: Bug Tracker, https://github.com/tobiasegelund/duckingit/issues
 Keywords: Serverless,DuckDB,Data Engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckingit-0.0.8/README.md` & `duckingit-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `duckingit-0.0.8/duckingit/_config.py` & `duckingit-0.0.9/duckingit/_config.py`

 * *Files identical despite different names*

### Comparing `duckingit-0.0.8/duckingit/_controller.py` & `duckingit-0.0.9/duckingit/_controller.py`

 * *Files identical despite different names*

### Comparing `duckingit-0.0.8/duckingit/_dataset.py` & `duckingit-0.0.9/duckingit/_dataset.py`

 * *Files identical despite different names*

### Comparing `duckingit-0.0.8/duckingit/_parser.py` & `duckingit-0.0.9/duckingit/_parser.py`

 * *Files identical despite different names*

### Comparing `duckingit-0.0.8/duckingit/_planner.py` & `duckingit-0.0.9/duckingit/_planner.py`

 * *Files identical despite different names*

### Comparing `duckingit-0.0.8/duckingit/_session.py` & `duckingit-0.0.9/duckingit/_session.py`

 * *Files identical despite different names*

### Comparing `duckingit-0.0.8/duckingit/_utils.py` & `duckingit-0.0.9/duckingit/_utils.py`

 * *Files identical despite different names*

### Comparing `duckingit-0.0.8/duckingit.egg-info/PKG-INFO` & `duckingit-0.0.9/duckingit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckingit
-Version: 0.0.8
+Version: 0.0.9
 Summary: A framework to leverage clusters of serverless functions for analytics. Powered by DuckDB
 Author-email: Tobias Egelund <egelundtobias@gmail.com>
 Project-URL: Homepage, https://github.com/tobiasegelund/duckingit
 Project-URL: Bug Tracker, https://github.com/tobiasegelund/duckingit/issues
 Keywords: Serverless,DuckDB,Data Engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckingit-0.0.8/pyproject.toml` & `duckingit-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "duckingit"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   {name="Tobias Egelund", email="egelundtobias@gmail.com" },
 ]
 description = "A framework to leverage clusters of serverless functions for analytics. Powered by DuckDB"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["Serverless", "DuckDB", "Data Engineering"]
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "boto3",
     "duckdb",
-    'sqlglot<=12.0',
+    'sqlglot<12.0',
     'pyarrow',
 ]
 
 [tool.setuptools]
 packages = ["duckingit"]
 
 [project.urls]
```

