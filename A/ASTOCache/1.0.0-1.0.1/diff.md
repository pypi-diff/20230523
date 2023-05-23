# Comparing `tmp/ASTOCache-1.0.0.tar.gz` & `tmp/ASTOCache-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASTOCache-1.0.0.tar", last modified: Tue May 23 06:03:52 2023, max compression
+gzip compressed data, was "ASTOCache-1.0.1.tar", last modified: Tue May 23 06:19:35 2023, max compression
```

## Comparing `ASTOCache-1.0.0.tar` & `ASTOCache-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-05-23 06:03:52.702997 ASTOCache-1.0.0/
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-05-23 06:03:52.702997 ASTOCache-1.0.0/ASTOCache/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     5590 2023-05-23 05:09:56.000000 ASTOCache-1.0.0/ASTOCache/__init__.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1270 2023-05-23 05:06:02.000000 ASTOCache-1.0.0/ASTOCache/logger.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-05-23 06:03:52.702997 ASTOCache-1.0.0/ASTOCache.egg-info/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      610 2023-05-23 06:03:52.000000 ASTOCache-1.0.0/ASTOCache.egg-info/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      263 2023-05-23 06:03:52.000000 ASTOCache-1.0.0/ASTOCache.egg-info/SOURCES.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2023-05-23 06:03:52.000000 ASTOCache-1.0.0/ASTOCache.egg-info/dependency_links.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       43 2023-05-23 06:03:52.000000 ASTOCache-1.0.0/ASTOCache.egg-info/requires.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       10 2023-05-23 06:03:52.000000 ASTOCache-1.0.0/ASTOCache.egg-info/top_level.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       78 2023-05-22 13:09:12.000000 ASTOCache-1.0.0/CHANGELOG.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1070 2023-05-22 13:12:22.000000 ASTOCache-1.0.0/LICENCE.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       25 2023-05-22 13:10:04.000000 ASTOCache-1.0.0/MANIFEST.in
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      610 2023-05-23 06:03:52.702997 ASTOCache-1.0.0/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      115 2023-05-22 13:06:57.000000 ASTOCache-1.0.0/README.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       38 2023-05-23 06:03:52.702997 ASTOCache-1.0.0/setup.cfg
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      632 2023-05-23 06:03:38.000000 ASTOCache-1.0.0/setup.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-05-23 06:19:35.534864 ASTOCache-1.0.1/
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-05-23 06:19:35.534864 ASTOCache-1.0.1/ASTOCache/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     5600 2023-05-23 06:12:00.000000 ASTOCache-1.0.1/ASTOCache/__init__.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1270 2023-05-23 05:06:02.000000 ASTOCache-1.0.1/ASTOCache/logger.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2023-05-23 06:19:35.534864 ASTOCache-1.0.1/ASTOCache.egg-info/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      610 2023-05-23 06:19:35.000000 ASTOCache-1.0.1/ASTOCache.egg-info/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      263 2023-05-23 06:19:35.000000 ASTOCache-1.0.1/ASTOCache.egg-info/SOURCES.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2023-05-23 06:19:35.000000 ASTOCache-1.0.1/ASTOCache.egg-info/dependency_links.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       43 2023-05-23 06:19:35.000000 ASTOCache-1.0.1/ASTOCache.egg-info/requires.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       10 2023-05-23 06:19:35.000000 ASTOCache-1.0.1/ASTOCache.egg-info/top_level.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       78 2023-05-22 13:09:12.000000 ASTOCache-1.0.1/CHANGELOG.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1070 2023-05-22 13:12:22.000000 ASTOCache-1.0.1/LICENCE.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       25 2023-05-22 13:10:04.000000 ASTOCache-1.0.1/MANIFEST.in
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      610 2023-05-23 06:19:35.534864 ASTOCache-1.0.1/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      115 2023-05-22 13:06:57.000000 ASTOCache-1.0.1/README.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       38 2023-05-23 06:19:35.534864 ASTOCache-1.0.1/setup.cfg
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      632 2023-05-23 06:19:20.000000 ASTOCache-1.0.1/setup.py
```

### Comparing `ASTOCache-1.0.0/ASTOCache/__init__.py` & `ASTOCache-1.0.1/ASTOCache/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import hashlib
 import os
 import redis
 import time
 import copy
-from logger import log_emmiter
+from ASTOCache.logger import log_emmiter
 import requests
 import sys
 import traceback
 
 def sort_json_recursively(d):
     if isinstance(d, dict):
         new_dict = {}
```

### Comparing `ASTOCache-1.0.0/ASTOCache/logger.py` & `ASTOCache-1.0.1/ASTOCache/logger.py`

 * *Files identical despite different names*

### Comparing `ASTOCache-1.0.0/ASTOCache.egg-info/PKG-INFO` & `ASTOCache-1.0.1/ASTOCache.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASTOCache
-Version: 1.0.0
+Version: 1.0.1
 Summary: Caching the JSON request payload and the value in RedisQ
 Home-page: UNKNOWN
 Author: Aditya Kumar Singh
 Author-email: aditya.singh@netcorecloud.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `ASTOCache-1.0.0/LICENCE.txt` & `ASTOCache-1.0.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `ASTOCache-1.0.0/PKG-INFO` & `ASTOCache-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASTOCache
-Version: 1.0.0
+Version: 1.0.1
 Summary: Caching the JSON request payload and the value in RedisQ
 Home-page: UNKNOWN
 Author: Aditya Kumar Singh
 Author-email: aditya.singh@netcorecloud.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `ASTOCache-1.0.0/setup.py` & `ASTOCache-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   'Operating System :: OS Independent',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='ASTOCache',
-  version='1.0.0',
+  version='1.0.1',
   description='Caching the JSON request payload and the value in RedisQ',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Aditya Kumar Singh',
   author_email='aditya.singh@netcorecloud.com',
   license='MIT', 
   classifiers=classifiers,
```

