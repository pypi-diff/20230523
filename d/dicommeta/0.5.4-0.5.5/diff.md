# Comparing `tmp/dicommeta-0.5.4.tar.gz` & `tmp/dicommeta-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicommeta-0.5.4.tar", max compression
+gzip compressed data, was "dicommeta-0.5.5.tar", max compression
```

## Comparing `dicommeta-0.5.4.tar` & `dicommeta-0.5.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11356 2023-05-09 13:28:51.971341 dicommeta-0.5.4/LICENSE
--rw-r--r--   0        0        0     1880 2023-05-22 17:47:09.010671 dicommeta-0.5.4/README.md
--rw-r--r--   0        0        0      507 2023-05-22 19:29:02.986506 dicommeta-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      153 2023-05-22 17:47:09.015177 dicommeta-0.5.4/src/dicommeta/Instance.py
--rw-r--r--   0        0        0      721 2023-05-22 17:47:09.004819 dicommeta-0.5.4/src/dicommeta/Series.py
--rw-r--r--   0        0        0     2608 2023-05-22 17:59:43.981254 dicommeta-0.5.4/src/dicommeta/Study.py
--rw-r--r--   0        0        0     2096 2023-05-22 17:47:09.016479 dicommeta-0.5.4/src/dicommeta/Utils.py
--rw-r--r--   0        0        0      139 2023-05-22 19:17:01.141051 dicommeta-0.5.4/src/dicommeta/__init__.py
--rw-r--r--   0        0        0     2333 1970-01-01 00:00:00.000000 dicommeta-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-05-09 13:28:51.971341 dicommeta-0.5.5/LICENSE
+-rw-r--r--   0        0        0     1880 2023-05-22 17:47:09.010671 dicommeta-0.5.5/README.md
+-rw-r--r--   0        0        0      514 2023-05-22 19:40:54.248060 dicommeta-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0      153 2023-05-22 17:47:09.015177 dicommeta-0.5.5/src/dicommeta/Instance.py
+-rw-r--r--   0        0        0      721 2023-05-22 17:47:09.004819 dicommeta-0.5.5/src/dicommeta/Series.py
+-rw-r--r--   0        0        0     2608 2023-05-22 17:59:43.981254 dicommeta-0.5.5/src/dicommeta/Study.py
+-rw-r--r--   0        0        0     2096 2023-05-22 17:47:09.016479 dicommeta-0.5.5/src/dicommeta/Utils.py
+-rw-r--r--   0        0        0      139 2023-05-22 19:17:01.141051 dicommeta-0.5.5/src/dicommeta/__init__.py
+-rw-r--r--   0        0        0     2340 1970-01-01 00:00:00.000000 dicommeta-0.5.5/PKG-INFO
```

### Comparing `dicommeta-0.5.4/LICENSE` & `dicommeta-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dicommeta-0.5.4/README.md` & `dicommeta-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `dicommeta-0.5.4/src/dicommeta/Series.py` & `dicommeta-0.5.5/src/dicommeta/Series.py`

 * *Files identical despite different names*

### Comparing `dicommeta-0.5.4/src/dicommeta/Study.py` & `dicommeta-0.5.5/src/dicommeta/Study.py`

 * *Files identical despite different names*

### Comparing `dicommeta-0.5.4/src/dicommeta/Utils.py` & `dicommeta-0.5.5/src/dicommeta/Utils.py`

 * *Files identical despite different names*

### Comparing `dicommeta-0.5.4/PKG-INFO` & `dicommeta-0.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: dicommeta
-Version: 0.5.4
+Version: 0.5.5
 Summary: Dicom Metadata structures
 Author: Kevin Long
 Author-email: longke@pennmedicine.upenn.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
-Requires-Dist: pendulum (>=2.1.2,<3.0.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # DicomMeta
 
 dicommeta is a Python library for efficiently storing large amounts of Dicom Metadata
 
 ## Installation
```

