# Comparing `tmp/codapy-0.3.7.tar.gz` & `tmp/codapy-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/codapy-0.3.7.tar", last modified: Thu Mar 21 19:41:01 2019, max compression
+gzip compressed data, was "dist/codapy-0.3.8.tar", last modified: Thu May  2 08:17:08 2019, max compression
```

## Comparing `codapy-0.3.7.tar` & `codapy-0.3.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-03-21 19:41:01.000000 codapy-0.3.7/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4740 2019-03-21 19:41:01.000000 codapy-0.3.7/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3572 2019-03-21 19:40:51.000000 codapy-0.3.7/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-03-21 19:41:01.000000 codapy-0.3.7/codapy.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4740 2019-03-21 19:41:01.000000 codapy-0.3.7/codapy.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      285 2019-03-21 19:41:01.000000 codapy-0.3.7/codapy.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2019-03-21 19:41:01.000000 codapy-0.3.7/codapy.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2019-03-21 19:41:01.000000 codapy-0.3.7/codapy.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2019-03-21 19:41:01.000000 codapy-0.3.7/codapy.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2019-03-21 19:41:01.000000 codapy-0.3.7/codapy.egg-info/zip-safe
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-03-21 19:41:01.000000 codapy-0.3.7/pycoda/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       63 2019-03-21 19:40:51.000000 codapy-0.3.7/pycoda/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1743 2019-03-21 19:40:51.000000 codapy-0.3.7/pycoda/codafile.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5711 2019-03-21 19:40:51.000000 codapy-0.3.7/pycoda/factories.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6711 2019-03-21 19:40:51.000000 codapy-0.3.7/pycoda/fields.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22168 2019-03-21 19:40:51.000000 codapy-0.3.7/pycoda/records.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2019-03-21 19:41:01.000000 codapy-0.3.7/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1505 2019-03-21 19:40:51.000000 codapy-0.3.7/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-05-02 08:17:08.000000 codapy-0.3.8/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4740 2019-05-02 08:17:08.000000 codapy-0.3.8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3572 2019-05-02 08:16:54.000000 codapy-0.3.8/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-05-02 08:17:08.000000 codapy-0.3.8/codapy.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4740 2019-05-02 08:17:08.000000 codapy-0.3.8/codapy.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      285 2019-05-02 08:17:08.000000 codapy-0.3.8/codapy.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2019-05-02 08:17:08.000000 codapy-0.3.8/codapy.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2019-05-02 08:17:08.000000 codapy-0.3.8/codapy.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2019-05-02 08:17:08.000000 codapy-0.3.8/codapy.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2019-05-02 08:17:08.000000 codapy-0.3.8/codapy.egg-info/zip-safe
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-05-02 08:17:08.000000 codapy-0.3.8/pycoda/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       63 2019-05-02 08:16:54.000000 codapy-0.3.8/pycoda/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1743 2019-05-02 08:16:54.000000 codapy-0.3.8/pycoda/codafile.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5711 2019-05-02 08:16:54.000000 codapy-0.3.8/pycoda/factories.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6711 2019-05-02 08:16:54.000000 codapy-0.3.8/pycoda/fields.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22168 2019-05-02 08:16:54.000000 codapy-0.3.8/pycoda/records.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2019-05-02 08:17:08.000000 codapy-0.3.8/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1505 2019-05-02 08:16:54.000000 codapy-0.3.8/setup.py
```

### Comparing `codapy-0.3.7/PKG-INFO` & `codapy-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codapy
-Version: 0.3.7
+Version: 0.3.8
 Summary: Coded statement of Account (CODA) python API
 Home-page: https://github.com/mhemeryck/pycoda
 Author: Martijn Hemeryck
 Author-email: martijn.hemeryck@gmail.com
 License: MIT
 Description: # pycoda
```

### Comparing `codapy-0.3.7/README.md` & `codapy-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `codapy-0.3.7/codapy.egg-info/PKG-INFO` & `codapy-0.3.8/codapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codapy
-Version: 0.3.7
+Version: 0.3.8
 Summary: Coded statement of Account (CODA) python API
 Home-page: https://github.com/mhemeryck/pycoda
 Author: Martijn Hemeryck
 Author-email: martijn.hemeryck@gmail.com
 License: MIT
 Description: # pycoda
```

### Comparing `codapy-0.3.7/pycoda/codafile.py` & `codapy-0.3.8/pycoda/codafile.py`

 * *Files identical despite different names*

### Comparing `codapy-0.3.7/pycoda/factories.py` & `codapy-0.3.8/pycoda/factories.py`

 * *Files identical despite different names*

### Comparing `codapy-0.3.7/pycoda/fields.py` & `codapy-0.3.8/pycoda/fields.py`

 * *Files identical despite different names*

### Comparing `codapy-0.3.7/pycoda/records.py` & `codapy-0.3.8/pycoda/records.py`

 * *Files identical despite different names*

### Comparing `codapy-0.3.7/setup.py` & `codapy-0.3.8/setup.py`

 * *Files identical despite different names*

