# Comparing `tmp/dicommeta-0.5.7.tar.gz` & `tmp/dicommeta-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicommeta-0.5.7.tar", max compression
+gzip compressed data, was "dicommeta-0.5.8.tar", max compression
```

## Comparing `dicommeta-0.5.7.tar` & `dicommeta-0.5.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11356 2023-05-09 13:28:51.971341 dicommeta-0.5.7/LICENSE
--rw-r--r--   0        0        0     1901 2023-05-22 22:09:41.951820 dicommeta-0.5.7/README.md
--rw-r--r--   0        0        0      514 2023-05-22 22:32:55.119142 dicommeta-0.5.7/pyproject.toml
--rw-r--r--   0        0        0        3 2023-05-22 22:09:41.954275 dicommeta-0.5.7/src/dicommeta/Instance.py
--rw-r--r--   0        0        0        3 2023-05-22 22:09:41.950004 dicommeta-0.5.7/src/dicommeta/Series.py
--rw-r--r--   0        0        0     3331 2023-05-22 22:09:41.953101 dicommeta-0.5.7/src/dicommeta/Structure.py
--rw-r--r--   0        0        0        3 2023-05-22 22:09:41.948747 dicommeta-0.5.7/src/dicommeta/Study.py
--rw-r--r--   0        0        0     2109 2023-05-22 22:29:37.095454 dicommeta-0.5.7/src/dicommeta/Utils.py
--rw-r--r--   0        0        0        0 2023-05-22 22:10:29.709188 dicommeta-0.5.7/src/dicommeta/__init__.py
--rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 dicommeta-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-05-09 13:28:51.971341 dicommeta-0.5.8/LICENSE
+-rw-r--r--   0        0        0     1901 2023-05-22 22:09:41.951820 dicommeta-0.5.8/README.md
+-rw-r--r--   0        0        0      514 2023-05-22 22:52:03.916813 dicommeta-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0        3 2023-05-22 22:09:41.954275 dicommeta-0.5.8/src/dicommeta/Instance.py
+-rw-r--r--   0        0        0        3 2023-05-22 22:09:41.950004 dicommeta-0.5.8/src/dicommeta/Series.py
+-rw-r--r--   0        0        0     3331 2023-05-22 22:09:41.953101 dicommeta-0.5.8/src/dicommeta/Struct.py
+-rw-r--r--   0        0        0        3 2023-05-22 22:09:41.948747 dicommeta-0.5.8/src/dicommeta/Study.py
+-rw-r--r--   0        0        0     2109 2023-05-22 22:29:37.095454 dicommeta-0.5.8/src/dicommeta/Utils.py
+-rw-r--r--   0        0        0        0 2023-05-22 22:10:29.709188 dicommeta-0.5.8/src/dicommeta/__init__.py
+-rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 dicommeta-0.5.8/PKG-INFO
```

### Comparing `dicommeta-0.5.7/LICENSE` & `dicommeta-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dicommeta-0.5.7/README.md` & `dicommeta-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `dicommeta-0.5.7/pyproject.toml` & `dicommeta-0.5.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dicommeta"
-version = "0.5.7"
+version = "0.5.8"
 description = "Dicom Metadata structures"
 authors = ["Kevin Long <longke@pennmedicine.upenn.edu>"]
 readme = "README.md"
 packages = [
     { include = "dicommeta", from = "src" },
 ]
```

### Comparing `dicommeta-0.5.7/src/dicommeta/Structure.py` & `dicommeta-0.5.8/src/dicommeta/Struct.py`

 * *Files identical despite different names*

### Comparing `dicommeta-0.5.7/src/dicommeta/Utils.py` & `dicommeta-0.5.8/src/dicommeta/Utils.py`

 * *Files identical despite different names*

### Comparing `dicommeta-0.5.7/PKG-INFO` & `dicommeta-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicommeta
-Version: 0.5.7
+Version: 0.5.8
 Summary: Dicom Metadata structures
 Author: Kevin Long
 Author-email: longke@pennmedicine.upenn.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

