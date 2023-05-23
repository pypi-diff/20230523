# Comparing `tmp/laff-0.7.1.tar.gz` & `tmp/laff-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laff-0.7.1.tar", max compression
+gzip compressed data, was "laff-0.7.2.tar", max compression
```

## Comparing `laff-0.7.1.tar` & `laff-0.7.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2642 2023-04-10 13:43:40.172834 laff-0.7.1/README.md
--rw-r--r--   0        0        0       60 2023-05-22 15:56:53.693817 laff-0.7.1/laff/__init__.py
--rw-r--r--   0        0        0     2299 2023-05-23 12:21:34.231551 laff-0.7.1/laff/laff.py
--rw-r--r--   0        0        0     1501 2023-05-23 12:25:19.049472 laff-0.7.1/laff/lcimport.py
--rw-r--r--   0        0        0     6955 2023-05-22 15:52:07.771697 laff-0.7.1/laff/methods.py
--rw-r--r--   0        0        0      410 2023-05-23 12:25:28.012544 laff-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 laff-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     2642 2023-04-10 13:43:40.172834 laff-0.7.2/README.md
+-rw-r--r--   0        0        0       60 2023-05-22 15:56:53.693817 laff-0.7.2/laff/__init__.py
+-rw-r--r--   0        0        0     2299 2023-05-23 12:21:34.231551 laff-0.7.2/laff/laff.py
+-rw-r--r--   0        0        0     1474 2023-05-23 12:38:27.291735 laff-0.7.2/laff/lcimport.py
+-rw-r--r--   0        0        0     6922 2023-05-23 12:40:41.468513 laff-0.7.2/laff/methods.py
+-rw-r--r--   0        0        0      410 2023-05-23 12:40:52.290062 laff-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 laff-0.7.2/PKG-INFO
```

### Comparing `laff-0.7.1/README.md` & `laff-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `laff-0.7.1/laff/laff.py` & `laff-0.7.2/laff/laff.py`

 * *Files identical despite different names*

### Comparing `laff-0.7.1/laff/lcimport.py` & `laff-0.7.2/laff/lcimport.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,10 +45,8 @@
 
     # Prepare data to pandas frame.
     data = vstack(qdptable).to_pandas()
     data = data.sort_values(by=['col1'])
     data = data.reset_index(drop=True)
     data.columns = ['time', 'time_perr', 'time_nerr', 'flux', 'flux_perr', 'flux_nerr']
 
-    data['flare'] = False
-
     return data
```

### Comparing `laff-0.7.1/laff/methods.py` & `laff-0.7.2/laff/methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
 
 def _find_deviations(data):
-
-    data = np.array(data.flux[:-10])
+    
     deviations = []
 
     for index in data.index[:10]:
 
         flux = np.array(data.flux)
 
         # Just return false if next point is lower.
```

### Comparing `laff-0.7.1/PKG-INFO` & `laff-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laff
-Version: 0.7.1
+Version: 0.7.2
 Summary: GRB lightcurve flare and continuum fitter.
 Author: Adam Hennessy
 Author-email: ah724@leicester.ac.uk
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

