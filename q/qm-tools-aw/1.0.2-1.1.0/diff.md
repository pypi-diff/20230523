# Comparing `tmp/qm_tools_aw-1.0.2.tar.gz` & `tmp/qm_tools_aw-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qm_tools_aw-1.0.2.tar", last modified: Mon May 15 17:14:28 2023, max compression
+gzip compressed data, was "qm_tools_aw-1.1.0.tar", last modified: Tue May 23 15:44:46 2023, max compression
```

## Comparing `qm_tools_aw-1.0.2.tar` & `qm_tools_aw-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-15 17:14:28.272624 qm_tools_aw-1.0.2/
--rw-r--r--   0 austinwallace   (501) staff       (20)     1074 2023-03-27 20:06:41.000000 qm_tools_aw-1.0.2/LICENSE
--rw-r--r--   0 austinwallace   (501) staff       (20)      689 2023-05-15 17:14:28.272745 qm_tools_aw-1.0.2/PKG-INFO
--rw-r--r--   0 austinwallace   (501) staff       (20)      107 2023-03-27 20:06:41.000000 qm_tools_aw-1.0.2/README.md
--rw-r--r--   0 austinwallace   (501) staff       (20)      649 2023-05-15 17:14:23.000000 qm_tools_aw-1.0.2/pyproject.toml
--rw-r--r--   0 austinwallace   (501) staff       (20)      202 2023-05-15 17:14:28.273233 qm_tools_aw-1.0.2/setup.cfg
-drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-15 17:14:28.268759 qm_tools_aw-1.0.2/src/
-drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-15 17:14:28.270557 qm_tools_aw-1.0.2/src/qm_tools_aw/
--rw-r--r--   0 austinwallace   (501) staff       (20)       20 2023-03-27 20:06:41.000000 qm_tools_aw-1.0.2/src/qm_tools_aw/__init__.py
--rw-r--r--   0 austinwallace   (501) staff       (20)     7725 2023-05-15 17:13:26.000000 qm_tools_aw-1.0.2/src/qm_tools_aw/tools.py
-drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-15 17:14:28.272369 qm_tools_aw-1.0.2/src/qm_tools_aw.egg-info/
--rw-r--r--   0 austinwallace   (501) staff       (20)      689 2023-05-15 17:14:28.000000 qm_tools_aw-1.0.2/src/qm_tools_aw.egg-info/PKG-INFO
--rw-r--r--   0 austinwallace   (501) staff       (20)      323 2023-05-15 17:14:28.000000 qm_tools_aw-1.0.2/src/qm_tools_aw.egg-info/SOURCES.txt
--rw-r--r--   0 austinwallace   (501) staff       (20)        1 2023-05-15 17:14:28.000000 qm_tools_aw-1.0.2/src/qm_tools_aw.egg-info/dependency_links.txt
--rw-r--r--   0 austinwallace   (501) staff       (20)       32 2023-05-15 17:14:28.000000 qm_tools_aw-1.0.2/src/qm_tools_aw.egg-info/requires.txt
--rw-r--r--   0 austinwallace   (501) staff       (20)       12 2023-05-15 17:14:28.000000 qm_tools_aw-1.0.2/src/qm_tools_aw.egg-info/top_level.txt
--rw-r--r--   0 austinwallace   (501) staff       (20)        1 2023-03-27 20:27:35.000000 qm_tools_aw-1.0.2/src/qm_tools_aw.egg-info/zip-safe
+drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-05-23 15:44:46.506312 qm_tools_aw-1.1.0/
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)     1074 2023-01-17 19:48:33.000000 qm_tools_aw-1.1.0/LICENSE
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      689 2023-05-23 15:44:46.506312 qm_tools_aw-1.1.0/PKG-INFO
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      107 2023-01-17 19:48:33.000000 qm_tools_aw-1.1.0/README.md
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      649 2023-05-23 15:44:05.000000 qm_tools_aw-1.1.0/pyproject.toml
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      202 2023-05-23 15:44:46.508312 qm_tools_aw-1.1.0/setup.cfg
+drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-05-23 15:44:46.470312 qm_tools_aw-1.1.0/src/
+drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-05-23 15:44:46.487312 qm_tools_aw-1.1.0/src/qm_tools_aw/
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)       20 2023-03-10 20:29:53.000000 qm_tools_aw-1.1.0/src/qm_tools_aw/__init__.py
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)     7927 2023-05-16 20:39:29.000000 qm_tools_aw-1.1.0/src/qm_tools_aw/tools.py
+drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-05-23 15:44:46.499312 qm_tools_aw-1.1.0/src/qm_tools_aw.egg-info/
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      689 2023-05-23 15:44:46.000000 qm_tools_aw-1.1.0/src/qm_tools_aw.egg-info/PKG-INFO
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      323 2023-05-23 15:44:46.000000 qm_tools_aw-1.1.0/src/qm_tools_aw.egg-info/SOURCES.txt
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)        1 2023-05-23 15:44:46.000000 qm_tools_aw-1.1.0/src/qm_tools_aw.egg-info/dependency_links.txt
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)       32 2023-05-23 15:44:46.000000 qm_tools_aw-1.1.0/src/qm_tools_aw.egg-info/requires.txt
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)       12 2023-05-23 15:44:46.000000 qm_tools_aw-1.1.0/src/qm_tools_aw.egg-info/top_level.txt
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)        1 2023-01-18 18:58:47.000000 qm_tools_aw-1.1.0/src/qm_tools_aw.egg-info/zip-safe
```

### Comparing `qm_tools_aw-1.0.2/LICENSE` & `qm_tools_aw-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qm_tools_aw-1.0.2/PKG-INFO` & `qm_tools_aw-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qm_tools_aw
-Version: 1.0.2
+Version: 1.1.0
 Summary: Provides some functions that I have found value in reusing for quantum chemistry related tasks.
 Author-email: "Austin M. Wallace" <awallace43@gatech.edu>
 Project-URL: Homepage, https://github.com/Awallace3/qm_tools
 Project-URL: Bug Tracker, https://github.com/Awallace3/qm_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qm_tools_aw-1.0.2/pyproject.toml` & `qm_tools_aw-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qm_tools_aw"
-version = "1.0.2"
+version = "1.1.0"
 authors = [
   { name="Austin M. Wallace", email="awallace43@gatech.edu" },
 ]
 description = "Provides some functions that I have found value in reusing for quantum chemistry related tasks."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `qm_tools_aw-1.0.2/src/qm_tools_aw/tools.py` & `qm_tools_aw-1.1.0/src/qm_tools_aw/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 import pickle
 import numpy as np
 from periodictable import elements
 import qcelemental as qcel
 import pandas as pd
 
+def save_pkl(file_name, obj):
+    with open(file_name, "wb") as fobj:
+        pickle.dump(obj, fobj)
+
+
+def load_pkl(file_name):
+    with open(file_name, "rb") as fobj:
+        return pickle.load(fobj)
+
 
 def create_pt_dict():
     """
     create_pt_dict creates dictionary for string elements to atomic number.
     """
     el_dc = {}
     for el in elements:
```

### Comparing `qm_tools_aw-1.0.2/src/qm_tools_aw.egg-info/PKG-INFO` & `qm_tools_aw-1.1.0/src/qm_tools_aw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qm-tools-aw
-Version: 1.0.2
+Version: 1.1.0
 Summary: Provides some functions that I have found value in reusing for quantum chemistry related tasks.
 Author-email: "Austin M. Wallace" <awallace43@gatech.edu>
 Project-URL: Homepage, https://github.com/Awallace3/qm_tools
 Project-URL: Bug Tracker, https://github.com/Awallace3/qm_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

