# Comparing `tmp/laff-0.6.1.tar.gz` & `tmp/laff-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laff-0.6.1.tar", max compression
+gzip compressed data, was "laff-0.7.0.tar", max compression
```

## Comparing `laff-0.6.1.tar` & `laff-0.7.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     2642 2023-04-10 13:43:40.172834 laff-0.6.1/README.md
--rw-r--r--   0        0        0       31 2023-05-19 17:34:57.346443 laff-0.6.1/laff/__init__.py
--rw-r--r--   0        0        0      109 2023-05-22 12:37:51.258725 laff-0.6.1/laff/laff.py
--rw-r--r--   0        0        0     1482 2023-05-19 18:24:22.268766 laff-0.6.1/laff/lcimport.py
--rw-r--r--   0        0        0      410 2023-05-22 12:38:21.091044 laff-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 laff-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     2642 2023-04-10 13:43:40.172834 laff-0.7.0/README.md
+-rw-r--r--   0        0        0       60 2023-05-22 15:56:53.693817 laff-0.7.0/laff/__init__.py
+-rw-r--r--   0        0        0     2299 2023-05-23 12:21:34.231551 laff-0.7.0/laff/laff.py
+-rw-r--r--   0        0        0     1520 2023-05-22 12:49:45.564897 laff-0.7.0/laff/lcimport.py
+-rw-r--r--   0        0        0     6955 2023-05-22 15:52:07.771697 laff-0.7.0/laff/methods.py
+-rw-r--r--   0        0        0      410 2023-05-23 12:22:08.457213 laff-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 laff-0.7.0/PKG-INFO
```

### Comparing `laff-0.6.1/README.md` & `laff-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `laff-0.6.1/laff/lcimport.py` & `laff-0.7.0/laff/lcimport.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,17 @@
         data (pandas dataframe)
             Formatted pandas datatable.
     """
 
     if format == "swift":
         # data = _swift_online_archive(filepath)
         data = 1
+    
+    else:
+        return "error"
         
     return data
 
 
 def _swift_online_archive(data_filepath):
     qdptable = []
     i = 0
```

### Comparing `laff-0.6.1/PKG-INFO` & `laff-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laff
-Version: 0.6.1
+Version: 0.7.0
 Summary: GRB lightcurve flare and continuum fitter.
 Author: Adam Hennessy
 Author-email: ah724@leicester.ac.uk
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

