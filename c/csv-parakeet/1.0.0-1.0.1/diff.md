# Comparing `tmp/csv_parakeet-1.0.0.tar.gz` & `tmp/csv_parakeet-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv_parakeet-1.0.0.tar", max compression
+gzip compressed data, was "csv_parakeet-1.0.1.tar", max compression
```

## Comparing `csv_parakeet-1.0.0.tar` & `csv_parakeet-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-05-19 15:48:24.538534 csv_parakeet-1.0.0/LICENSE
--rw-r--r--   0        0        0      675 2023-05-19 15:48:24.538534 csv_parakeet-1.0.0/README.md
--rw-r--r--   0        0        0     1033 2023-05-19 15:48:24.538534 csv_parakeet-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       72 2023-05-19 15:48:24.538534 csv_parakeet-1.0.0/src/csv_parakeet/__init__.py
--rw-r--r--   0        0        0     1043 2023-05-19 15:48:24.538534 csv_parakeet-1.0.0/src/csv_parakeet/console.py
--rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 csv_parakeet-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-23 11:00:52.631360 csv_parakeet-1.0.1/LICENSE
+-rw-r--r--   0        0        0      675 2023-05-23 11:00:52.631360 csv_parakeet-1.0.1/README.md
+-rw-r--r--   0        0        0     1033 2023-05-23 11:00:52.631360 csv_parakeet-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       72 2023-05-23 11:00:52.631360 csv_parakeet-1.0.1/src/csv_parakeet/__init__.py
+-rw-r--r--   0        0        0     1043 2023-05-23 11:00:52.631360 csv_parakeet-1.0.1/src/csv_parakeet/console.py
+-rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 csv_parakeet-1.0.1/PKG-INFO
```

### Comparing `csv_parakeet-1.0.0/LICENSE` & `csv_parakeet-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `csv_parakeet-1.0.0/README.md` & `csv_parakeet-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `csv_parakeet-1.0.0/pyproject.toml` & `csv_parakeet-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "csv-parakeet"
-version = "1.0.0"
+version = "1.0.1"
 description = "Parquet to CSV command line tool"
 authors = ["Alfie Bowman <alfiebowman@protonmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/A1fus/csv-parakeet"
 repository = "https://github.com/A1fus/csv-parakeet"
 
 [tool.poetry.dependencies]
```

### Comparing `csv_parakeet-1.0.0/src/csv_parakeet/console.py` & `csv_parakeet-1.0.1/src/csv_parakeet/console.py`

 * *Files identical despite different names*

### Comparing `csv_parakeet-1.0.0/PKG-INFO` & `csv_parakeet-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv-parakeet
-Version: 1.0.0
+Version: 1.0.1
 Summary: Parquet to CSV command line tool
 Home-page: https://github.com/A1fus/csv-parakeet
 Author: Alfie Bowman
 Author-email: alfiebowman@protonmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

