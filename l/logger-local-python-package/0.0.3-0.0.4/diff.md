# Comparing `tmp/logger-local-python-package-0.0.3.tar.gz` & `tmp/logger-local-python-package-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger-local-python-package-0.0.3.tar", last modified: Fri May 19 10:17:52 2023, max compression
+gzip compressed data, was "logger-local-python-package-0.0.4.tar", last modified: Tue May 23 14:03:40 2023, max compression
```

## Comparing `logger-local-python-package-0.0.3.tar` & `logger-local-python-package-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:17:52.389367 logger-local-python-package-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-19 10:17:41.000000 logger-local-python-package-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-19 10:17:52.389367 logger-local-python-package-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-19 10:17:41.000000 logger-local-python-package-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:17:52.389367 logger-local-python-package-0.0.3/logger_local_python_package.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-19 10:17:52.000000 logger-local-python-package-0.0.3/logger_local_python_package.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-19 10:17:52.000000 logger-local-python-package-0.0.3/logger_local_python_package.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 10:17:52.000000 logger-local-python-package-0.0.3/logger_local_python_package.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-19 10:17:52.000000 logger-local-python-package-0.0.3/logger_local_python_package.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 10:17:52.389367 logger-local-python-package-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-19 10:17:41.000000 logger-local-python-package-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:17:52.389367 logger-local-python-package-0.0.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-19 10:17:41.000000 logger-local-python-package-0.0.3/src/LoggerService.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-19 10:17:41.000000 logger-local-python-package-0.0.3/src/LoggerServiceSingleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-19 10:17:41.000000 logger-local-python-package-0.0.3/src/MessageSeverity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-19 10:17:41.000000 logger-local-python-package-0.0.3/src/Writer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 10:17:41.000000 logger-local-python-package-0.0.3/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:17:52.389367 logger-local-python-package-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-19 10:17:41.000000 logger-local-python-package-0.0.3/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:03:40.087737 logger-local-python-package-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-23 14:03:22.000000 logger-local-python-package-0.0.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:03:40.083736 logger-local-python-package-0.0.4/LoggerLocalPythonPackage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-23 14:03:22.000000 logger-local-python-package-0.0.4/LoggerLocalPythonPackage/LoggerService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-23 14:03:22.000000 logger-local-python-package-0.0.4/LoggerLocalPythonPackage/LoggerServiceSingleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-23 14:03:22.000000 logger-local-python-package-0.0.4/LoggerLocalPythonPackage/MessageSeverity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-23 14:03:22.000000 logger-local-python-package-0.0.4/LoggerLocalPythonPackage/Writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:03:22.000000 logger-local-python-package-0.0.4/LoggerLocalPythonPackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-23 14:03:40.087737 logger-local-python-package-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-23 14:03:22.000000 logger-local-python-package-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:03:40.087737 logger-local-python-package-0.0.4/logger_local_python_package.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-23 14:03:40.000000 logger-local-python-package-0.0.4/logger_local_python_package.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-23 14:03:40.000000 logger-local-python-package-0.0.4/logger_local_python_package.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:03:40.000000 logger-local-python-package-0.0.4/logger_local_python_package.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-23 14:03:40.000000 logger-local-python-package-0.0.4/logger_local_python_package.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:03:40.087737 logger-local-python-package-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-23 14:03:22.000000 logger-local-python-package-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:03:40.087737 logger-local-python-package-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-23 14:03:22.000000 logger-local-python-package-0.0.4/tests/test_writer.py
```

### Comparing `logger-local-python-package-0.0.3/LICENSE` & `logger-local-python-package-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `logger-local-python-package-0.0.3/PKG-INFO` & `logger-local-python-package-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-local-python-package
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyPI Package for Circles Logger Python Local
 Home-page: https://github.com/circles-zone/logger-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `logger-local-python-package-0.0.3/logger_local_python_package.egg-info/PKG-INFO` & `logger-local-python-package-0.0.4/logger_local_python_package.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-local-python-package
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyPI Package for Circles Logger Python Local
 Home-page: https://github.com/circles-zone/logger-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `logger-local-python-package-0.0.3/setup.py` & `logger-local-python-package-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='logger-local-python-package',
-    version='0.0.3',
+    version='0.0.4',
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles Logger Python Local",
     long_description="This is a package for sharing common Logger function used in different repositories",
     long_description_content_type="text/markdown",
     url="https://github.com/circles-zone/logger-local-python-package",
     packages=setuptools.find_packages(),
```

### Comparing `logger-local-python-package-0.0.3/src/LoggerService.py` & `logger-local-python-package-0.0.4/LoggerLocalPythonPackage/LoggerService.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from src.MessageSeverity import MessageSeverity
-from src.Writer import Writer
+from LoggerLocalPythonPackage.MessageSeverity import MessageSeverity
+from LoggerLocalPythonPackage.Writer import Writer
 
 
 class LoggerService:
 
     def __init__(self):
         self._writer = Writer()
```

### Comparing `logger-local-python-package-0.0.3/src/Writer.py` & `logger-local-python-package-0.0.4/LoggerLocalPythonPackage/Writer.py`

 * *Files identical despite different names*

### Comparing `logger-local-python-package-0.0.3/tests/test_writer.py` & `logger-local-python-package-0.0.4/tests/test_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pymysql
 import os
-from src.MessageSeverity import MessageSeverity
-from src.LoggerServiceSingleton import locallgr
+from LoggerLocalPythonPackage.MessageSeverity import MessageSeverity
+from LoggerLocalPythonPackage.LoggerServiceSingleton import locallgr
 
 ID = 5000001
 # ID = 1
 
 def get_connection() -> pymysql.connections.Connection:
     return pymysql.connect(
         user=os.getenv('RDS_USERNAME'),
```

