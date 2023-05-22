# Comparing `tmp/dicommeta-0.5.5.tar.gz` & `tmp/dicommeta-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicommeta-0.5.5.tar", max compression
+gzip compressed data, was "dicommeta-0.5.6.tar", max compression
```

## Comparing `dicommeta-0.5.5.tar` & `dicommeta-0.5.6.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    11356 2023-05-09 13:28:51.971341 dicommeta-0.5.5/LICENSE
--rw-r--r--   0        0        0     1880 2023-05-22 17:47:09.010671 dicommeta-0.5.5/README.md
--rw-r--r--   0        0        0      514 2023-05-22 19:40:54.248060 dicommeta-0.5.5/pyproject.toml
--rw-r--r--   0        0        0      153 2023-05-22 17:47:09.015177 dicommeta-0.5.5/src/dicommeta/Instance.py
--rw-r--r--   0        0        0      721 2023-05-22 17:47:09.004819 dicommeta-0.5.5/src/dicommeta/Series.py
--rw-r--r--   0        0        0     2608 2023-05-22 17:59:43.981254 dicommeta-0.5.5/src/dicommeta/Study.py
--rw-r--r--   0        0        0     2096 2023-05-22 17:47:09.016479 dicommeta-0.5.5/src/dicommeta/Utils.py
--rw-r--r--   0        0        0      139 2023-05-22 19:17:01.141051 dicommeta-0.5.5/src/dicommeta/__init__.py
--rw-r--r--   0        0        0     2340 1970-01-01 00:00:00.000000 dicommeta-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-05-09 13:28:51.971341 dicommeta-0.5.6/LICENSE
+-rw-r--r--   0        0        0     1901 2023-05-22 22:09:41.951820 dicommeta-0.5.6/README.md
+-rw-r--r--   0        0        0      514 2023-05-22 22:10:57.585318 dicommeta-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0        3 2023-05-22 22:09:41.954275 dicommeta-0.5.6/src/dicommeta/Instance.py
+-rw-r--r--   0        0        0        3 2023-05-22 22:09:41.950004 dicommeta-0.5.6/src/dicommeta/Series.py
+-rw-r--r--   0        0        0     3331 2023-05-22 22:09:41.953101 dicommeta-0.5.6/src/dicommeta/Structure.py
+-rw-r--r--   0        0        0        3 2023-05-22 22:09:41.948747 dicommeta-0.5.6/src/dicommeta/Study.py
+-rw-r--r--   0        0        0     2096 2023-05-22 17:47:09.016479 dicommeta-0.5.6/src/dicommeta/Utils.py
+-rw-r--r--   0        0        0        0 2023-05-22 22:10:29.709188 dicommeta-0.5.6/src/dicommeta/__init__.py
+-rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 dicommeta-0.5.6/PKG-INFO
```

### Comparing `dicommeta-0.5.5/LICENSE` & `dicommeta-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dicommeta-0.5.5/README.md` & `dicommeta-0.5.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 pip install dicommeta
 ```
 
 ## Usage
 
 ```python
 from pprint import pprint
-from src.dicommeta import (Series, Study, Instance)
+from src.dicommeta import (Series, Study)
+from dicommeta import Instance
 from dicommeta.Utils import Mode
 
 new_dicom_study = Study(
     StudyInstanceUID='1.3.6.1.4.1.14519.5.2.1.4334.1501.757929841898426427124434115918',
     SpecificCharacterSet='ISO_IR 100',
     StudyDate="20190701",
     StudyTime='023750',
```

### Comparing `dicommeta-0.5.5/pyproject.toml` & `dicommeta-0.5.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dicommeta"
-version = "0.5.5"
+version = "0.5.6"
 description = "Dicom Metadata structures"
 authors = ["Kevin Long <longke@pennmedicine.upenn.edu>"]
 readme = "README.md"
 packages = [
     { include = "dicommeta", from = "src" },
 ]
```

### Comparing `dicommeta-0.5.5/src/dicommeta/Utils.py` & `dicommeta-0.5.6/src/dicommeta/Utils.py`

 * *Files identical despite different names*

### Comparing `dicommeta-0.5.5/PKG-INFO` & `dicommeta-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicommeta
-Version: 0.5.5
+Version: 0.5.6
 Summary: Dicom Metadata structures
 Author: Kevin Long
 Author-email: longke@pennmedicine.upenn.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -24,15 +24,16 @@
 pip install dicommeta
 ```
 
 ## Usage
 
 ```python
 from pprint import pprint
-from src.dicommeta import (Series, Study, Instance)
+from src.dicommeta import (Series, Study)
+from dicommeta import Instance
 from dicommeta.Utils import Mode
 
 new_dicom_study = Study(
     StudyInstanceUID='1.3.6.1.4.1.14519.5.2.1.4334.1501.757929841898426427124434115918',
     SpecificCharacterSet='ISO_IR 100',
     StudyDate="20190701",
     StudyTime='023750',
```

