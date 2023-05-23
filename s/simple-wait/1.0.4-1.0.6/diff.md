# Comparing `tmp/simple-wait-1.0.4.tar.gz` & `tmp/simple-wait-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-wait-1.0.4.tar", last modified: Tue May 23 06:58:45 2023, max compression
+gzip compressed data, was "simple-wait-1.0.6.tar", last modified: Tue May 23 10:50:25 2023, max compression
```

## Comparing `simple-wait-1.0.4.tar` & `simple-wait-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:58:45.497998 simple-wait-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-23 06:58:34.000000 simple-wait-1.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-23 06:58:45.497998 simple-wait-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-23 06:58:34.000000 simple-wait-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-23 06:58:34.000000 simple-wait-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 06:58:45.497998 simple-wait-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:58:45.497998 simple-wait-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:58:45.497998 simple-wait-1.0.4/src/simple_wait/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-23 06:58:34.000000 simple-wait-1.0.4/src/simple_wait/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:58:45.497998 simple-wait-1.0.4/src/simple_wait.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-23 06:58:45.000000 simple-wait-1.0.4/src/simple_wait.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-23 06:58:45.000000 simple-wait-1.0.4/src/simple_wait.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:58:45.000000 simple-wait-1.0.4/src/simple_wait.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 06:58:45.000000 simple-wait-1.0.4/src/simple_wait.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:58:45.497998 simple-wait-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-23 06:58:34.000000 simple-wait-1.0.4/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:50:25.519823 simple-wait-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-23 10:50:14.000000 simple-wait-1.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-23 10:50:25.519823 simple-wait-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-23 10:50:14.000000 simple-wait-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-23 10:50:14.000000 simple-wait-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 10:50:25.519823 simple-wait-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:50:25.515823 simple-wait-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:50:25.515823 simple-wait-1.0.6/src/simple_wait/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-23 10:50:14.000000 simple-wait-1.0.6/src/simple_wait/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:50:25.519823 simple-wait-1.0.6/src/simple_wait.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-23 10:50:25.000000 simple-wait-1.0.6/src/simple_wait.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-23 10:50:25.000000 simple-wait-1.0.6/src/simple_wait.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 10:50:25.000000 simple-wait-1.0.6/src/simple_wait.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 10:50:25.000000 simple-wait-1.0.6/src/simple_wait.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:50:25.519823 simple-wait-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-23 10:50:14.000000 simple-wait-1.0.6/tests/tests.py
```

### Comparing `simple-wait-1.0.4/LICENSE.txt` & `simple-wait-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple-wait-1.0.4/PKG-INFO` & `simple-wait-1.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-wait
-Version: 1.0.4
+Version: 1.0.6
 Summary: Simple wait
 Author-email: Ilya Petrash <ilya.petrash@inbox.ru>
 License: MIT License
         
         Copyright (c) 2023 Ilya Petrash
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,16 +35,20 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # simple-wait
 Simple wait
 
+[![Run tests](https://github.com/gil9red/simple-wait/actions/workflows/run-tests.yml/badge.svg)](https://github.com/gil9red/simple-wait/actions/workflows/run-tests.yml)
+[![Upload Python Package](https://github.com/gil9red/simple-wait/actions/workflows/python-publish.yml/badge.svg)](https://github.com/gil9red/simple-wait/actions/workflows/python-publish.yml)
+
 ```python
 from datetime import datetime
+from simple_wait import wait
 
 print("Start wait")
 wait(seconds=5)
 print("Finish wait")
 
 while True:
     print()
```

### Comparing `simple-wait-1.0.4/pyproject.toml` & `simple-wait-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simple-wait-1.0.4/src/simple_wait/__init__.py` & `simple-wait-1.0.6/src/simple_wait/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 __author__ = "ipetrash"
-__version__ = "1.0.4"
+__version__ = "1.0.6"
 
 
 import sys
 import time
 
 from datetime import datetime, timedelta
 from itertools import cycle
```

### Comparing `simple-wait-1.0.4/src/simple_wait.egg-info/PKG-INFO` & `simple-wait-1.0.6/src/simple_wait.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-wait
-Version: 1.0.4
+Version: 1.0.6
 Summary: Simple wait
 Author-email: Ilya Petrash <ilya.petrash@inbox.ru>
 License: MIT License
         
         Copyright (c) 2023 Ilya Petrash
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,16 +35,20 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # simple-wait
 Simple wait
 
+[![Run tests](https://github.com/gil9red/simple-wait/actions/workflows/run-tests.yml/badge.svg)](https://github.com/gil9red/simple-wait/actions/workflows/run-tests.yml)
+[![Upload Python Package](https://github.com/gil9red/simple-wait/actions/workflows/python-publish.yml/badge.svg)](https://github.com/gil9red/simple-wait/actions/workflows/python-publish.yml)
+
 ```python
 from datetime import datetime
+from simple_wait import wait
 
 print("Start wait")
 wait(seconds=5)
 print("Finish wait")
 
 while True:
     print()
```

### Comparing `simple-wait-1.0.4/tests/tests.py` & `simple-wait-1.0.6/tests/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,20 +45,17 @@
                     str_timedelta(timedelta(**actual)),
                 )
 
     def test_get_timeout_date(self):
         with self.subTest("None"):
             now = datetime.today()
 
-            self.assertEqual(get_timeout_date(now), get_timeout_date())
-            self.assertEqual(now, get_timeout_date())
-            self.assertEqual(
-                now,
-                get_timeout_date(now),
-            )
+            self.assertTrue(get_timeout_date())
+            self.assertTrue(get_timeout_date(now))
+            self.assertEqual(now, get_timeout_date(now))
 
         with self.subTest("Simple"):
             now = datetime.today()
             self.assertEqual(
                 now + timedelta(hours=2, minutes=10, seconds=20),
                 get_timeout_date(now, hours=2, minutes=10, seconds=20),
             )
```

