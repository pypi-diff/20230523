# Comparing `tmp/simple-wait-1.0.1.tar.gz` & `tmp/simple-wait-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-wait-1.0.1.tar", last modified: Mon May 22 23:48:21 2023, max compression
+gzip compressed data, was "simple-wait-1.0.3.tar", last modified: Tue May 23 06:35:25 2023, max compression
```

## Comparing `simple-wait-1.0.1.tar` & `simple-wait-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:48:21.192457 simple-wait-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-22 23:48:08.000000 simple-wait-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-22 23:48:21.192457 simple-wait-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-22 23:48:08.000000 simple-wait-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-22 23:48:08.000000 simple-wait-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 23:48:21.192457 simple-wait-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:48:21.188457 simple-wait-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:48:21.192457 simple-wait-1.0.1/src/simple_wait/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-22 23:48:08.000000 simple-wait-1.0.1/src/simple_wait/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:48:21.192457 simple-wait-1.0.1/src/simple_wait.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-22 23:48:21.000000 simple-wait-1.0.1/src/simple_wait.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-22 23:48:21.000000 simple-wait-1.0.1/src/simple_wait.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 23:48:21.000000 simple-wait-1.0.1/src/simple_wait.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 23:48:21.000000 simple-wait-1.0.1/src/simple_wait.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:48:21.192457 simple-wait-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-22 23:48:08.000000 simple-wait-1.0.1/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:35:25.343094 simple-wait-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-23 06:35:14.000000 simple-wait-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-23 06:35:25.343094 simple-wait-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-23 06:35:14.000000 simple-wait-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-23 06:35:14.000000 simple-wait-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 06:35:25.343094 simple-wait-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:35:25.343094 simple-wait-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:35:25.343094 simple-wait-1.0.3/src/simple_wait/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-23 06:35:14.000000 simple-wait-1.0.3/src/simple_wait/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:35:25.343094 simple-wait-1.0.3/src/simple_wait.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-23 06:35:25.000000 simple-wait-1.0.3/src/simple_wait.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-23 06:35:25.000000 simple-wait-1.0.3/src/simple_wait.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:35:25.000000 simple-wait-1.0.3/src/simple_wait.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 06:35:25.000000 simple-wait-1.0.3/src/simple_wait.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:35:25.343094 simple-wait-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-23 06:35:14.000000 simple-wait-1.0.3/tests/tests.py
```

### Comparing `simple-wait-1.0.1/LICENSE.txt` & `simple-wait-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple-wait-1.0.1/PKG-INFO` & `simple-wait-1.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-wait
-Version: 1.0.1
+Version: 1.0.3
 Summary: Simple wait
 Author-email: Ilya Petrash <ilya.petrash@inbox.ru>
 License: MIT License
         
         Copyright (c) 2023 Ilya Petrash
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,13 +27,14 @@
         
 Project-URL: Homepage, https://github.com/gil9red/simple-wait
 Project-URL: Bug Tracker, https://github.com/gil9red/simple-wait/issues
 Keywords: wait
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # simple-wait
 Simple wait
```

### Comparing `simple-wait-1.0.1/pyproject.toml` & `simple-wait-1.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 [project]
 name = "simple-wait"
-version = "1.0.1"
+dynamic = ["version"]
 authors = [
   { name="Ilya Petrash", email="ilya.petrash@inbox.ru" },
 ]
 description = "Simple wait"
 readme = "README.md"
 license = { file = "LICENSE.txt" }
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
+    "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 keywords = ["wait"]
 
 [project.urls]
 "Homepage" = "https://github.com/gil9red/simple-wait"
 "Bug Tracker" = "https://github.com/gil9red/simple-wait/issues"
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools.dynamic]
+version = { attr = "simple_wait.__version__" }
+
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `simple-wait-1.0.1/src/simple_wait/__init__.py` & `simple-wait-1.0.3/src/simple_wait/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 __author__ = "ipetrash"
-__version__ = "1.0.1"
+__version__ = "1.0.3"
 
 
 import sys
 import time
 
 from datetime import datetime, timedelta
 from itertools import cycle
```

### Comparing `simple-wait-1.0.1/src/simple_wait.egg-info/PKG-INFO` & `simple-wait-1.0.3/src/simple_wait.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-wait
-Version: 1.0.1
+Version: 1.0.3
 Summary: Simple wait
 Author-email: Ilya Petrash <ilya.petrash@inbox.ru>
 License: MIT License
         
         Copyright (c) 2023 Ilya Petrash
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,13 +27,14 @@
         
 Project-URL: Homepage, https://github.com/gil9red/simple-wait
 Project-URL: Bug Tracker, https://github.com/gil9red/simple-wait/issues
 Keywords: wait
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # simple-wait
 Simple wait
```

### Comparing `simple-wait-1.0.1/tests/tests.py` & `simple-wait-1.0.3/tests/tests.py`

 * *Files identical despite different names*

