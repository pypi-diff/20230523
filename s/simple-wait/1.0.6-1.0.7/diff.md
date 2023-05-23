# Comparing `tmp/simple-wait-1.0.6.tar.gz` & `tmp/simple-wait-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-wait-1.0.6.tar", last modified: Tue May 23 10:50:25 2023, max compression
+gzip compressed data, was "simple-wait-1.0.7.tar", last modified: Tue May 23 11:05:40 2023, max compression
```

## Comparing `simple-wait-1.0.6.tar` & `simple-wait-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:50:25.519823 simple-wait-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-23 10:50:14.000000 simple-wait-1.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-23 10:50:25.519823 simple-wait-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-23 10:50:14.000000 simple-wait-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-23 10:50:14.000000 simple-wait-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 10:50:25.519823 simple-wait-1.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:50:25.515823 simple-wait-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:50:25.515823 simple-wait-1.0.6/src/simple_wait/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-23 10:50:14.000000 simple-wait-1.0.6/src/simple_wait/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:50:25.519823 simple-wait-1.0.6/src/simple_wait.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-23 10:50:25.000000 simple-wait-1.0.6/src/simple_wait.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-23 10:50:25.000000 simple-wait-1.0.6/src/simple_wait.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 10:50:25.000000 simple-wait-1.0.6/src/simple_wait.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 10:50:25.000000 simple-wait-1.0.6/src/simple_wait.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:50:25.519823 simple-wait-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-23 10:50:14.000000 simple-wait-1.0.6/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:05:40.900806 simple-wait-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-23 11:05:29.000000 simple-wait-1.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-23 11:05:40.900806 simple-wait-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-23 11:05:29.000000 simple-wait-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-23 11:05:29.000000 simple-wait-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 11:05:40.900806 simple-wait-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:05:40.900806 simple-wait-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:05:40.900806 simple-wait-1.0.7/src/simple_wait/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-23 11:05:29.000000 simple-wait-1.0.7/src/simple_wait/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:05:40.900806 simple-wait-1.0.7/src/simple_wait.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-23 11:05:40.000000 simple-wait-1.0.7/src/simple_wait.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-23 11:05:40.000000 simple-wait-1.0.7/src/simple_wait.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 11:05:40.000000 simple-wait-1.0.7/src/simple_wait.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 11:05:40.000000 simple-wait-1.0.7/src/simple_wait.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:05:40.900806 simple-wait-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-23 11:05:29.000000 simple-wait-1.0.7/tests/tests.py
```

### Comparing `simple-wait-1.0.6/LICENSE.txt` & `simple-wait-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple-wait-1.0.6/PKG-INFO` & `simple-wait-1.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-wait
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simple wait
 Author-email: Ilya Petrash <ilya.petrash@inbox.ru>
 License: MIT License
         
         Copyright (c) 2023 Ilya Petrash
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,24 +28,29 @@
 Project-URL: Homepage, https://github.com/gil9red/simple-wait
 Project-URL: Bug Tracker, https://github.com/gil9red/simple-wait/issues
 Keywords: wait
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # simple-wait
 Simple wait
 
-[![Run tests](https://github.com/gil9red/simple-wait/actions/workflows/run-tests.yml/badge.svg)](https://github.com/gil9red/simple-wait/actions/workflows/run-tests.yml)
-[![Upload Python Package](https://github.com/gil9red/simple-wait/actions/workflows/python-publish.yml/badge.svg)](https://github.com/gil9red/simple-wait/actions/workflows/python-publish.yml)
+[![tests](https://github.com/gil9red/simple-wait/actions/workflows/run-tests.yml/badge.svg)](https://github.com/gil9red/simple-wait/actions/workflows/run-tests.yml)
+[![upload to pypi](https://github.com/gil9red/simple-wait/actions/workflows/python-publish.yml/badge.svg)](https://github.com/gil9red/simple-wait/actions/workflows/python-publish.yml)
+[![pypi](https://img.shields.io/pypi/v/simple-wait.svg)](https://pypi.org/project/simple-wait/)
+![pypi python versions](https://img.shields.io/pypi/pyversions/simple-wait.svg)
+[![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://pypi.org/project/black/)
+[![License](https://img.shields.io/badge/license-MIT-black.svg)](https://opensource.org/licenses/MIT)
 
+Example:
 ```python
 from datetime import datetime
 from simple_wait import wait
 
 print("Start wait")
 wait(seconds=5)
 print("Finish wait")
```

### Comparing `simple-wait-1.0.6/pyproject.toml` & `simple-wait-1.0.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 dynamic = ["version"]
 authors = [
   { name="Ilya Petrash", email="ilya.petrash@inbox.ru" },
 ]
 description = "Simple wait"
 readme = "README.md"
 license = { file = "LICENSE.txt" }
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 keywords = ["wait"]
```

### Comparing `simple-wait-1.0.6/src/simple_wait/__init__.py` & `simple-wait-1.0.7/src/simple_wait/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 __author__ = "ipetrash"
-__version__ = "1.0.6"
+__version__ = "1.0.7"
 
 
 import sys
 import time
 
 from datetime import datetime, timedelta
 from itertools import cycle
```

### Comparing `simple-wait-1.0.6/src/simple_wait.egg-info/PKG-INFO` & `simple-wait-1.0.7/src/simple_wait.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-wait
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simple wait
 Author-email: Ilya Petrash <ilya.petrash@inbox.ru>
 License: MIT License
         
         Copyright (c) 2023 Ilya Petrash
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,24 +28,29 @@
 Project-URL: Homepage, https://github.com/gil9red/simple-wait
 Project-URL: Bug Tracker, https://github.com/gil9red/simple-wait/issues
 Keywords: wait
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # simple-wait
 Simple wait
 
-[![Run tests](https://github.com/gil9red/simple-wait/actions/workflows/run-tests.yml/badge.svg)](https://github.com/gil9red/simple-wait/actions/workflows/run-tests.yml)
-[![Upload Python Package](https://github.com/gil9red/simple-wait/actions/workflows/python-publish.yml/badge.svg)](https://github.com/gil9red/simple-wait/actions/workflows/python-publish.yml)
+[![tests](https://github.com/gil9red/simple-wait/actions/workflows/run-tests.yml/badge.svg)](https://github.com/gil9red/simple-wait/actions/workflows/run-tests.yml)
+[![upload to pypi](https://github.com/gil9red/simple-wait/actions/workflows/python-publish.yml/badge.svg)](https://github.com/gil9red/simple-wait/actions/workflows/python-publish.yml)
+[![pypi](https://img.shields.io/pypi/v/simple-wait.svg)](https://pypi.org/project/simple-wait/)
+![pypi python versions](https://img.shields.io/pypi/pyversions/simple-wait.svg)
+[![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://pypi.org/project/black/)
+[![License](https://img.shields.io/badge/license-MIT-black.svg)](https://opensource.org/licenses/MIT)
 
+Example:
 ```python
 from datetime import datetime
 from simple_wait import wait
 
 print("Start wait")
 wait(seconds=5)
 print("Finish wait")
```

### Comparing `simple-wait-1.0.6/tests/tests.py` & `simple-wait-1.0.7/tests/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 __author__ = "ipetrash"
 
 
-from datetime import timedelta, datetime
-
 import io
 import unittest
 
+from datetime import timedelta, datetime
+
 from src.simple_wait import str_timedelta, get_timeout_date, wait
 
 
 class TestCase(unittest.TestCase):
     timedelta_cases: list[dict[str, int]] = [
         ("00:00:10", dict(seconds=10)),
         ("00:00:10", dict(seconds=10, milliseconds=150)),
@@ -72,17 +72,15 @@
             buffer=io.BytesIO(),
             encoding="utf-8",
         )
         wait(seconds=3, log=log)
 
         log.seek(0)
         lines = [
-            line.strip()
-            for line in log.readlines()
-            if "Time left to wait" in line
+            line.strip() for line in log.readlines() if "Time left to wait" in line
         ]
         self.assertTrue(lines)
         self.assertTrue(len(lines) > 1)
 
 
 if __name__ == "__main__":
     unittest.main()
```

