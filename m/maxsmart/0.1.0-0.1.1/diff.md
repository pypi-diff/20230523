# Comparing `tmp/maxsmart-0.1.0.tar.gz` & `tmp/maxsmart-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxsmart-0.1.0.tar", last modified: Sun May 21 18:08:13 2023, max compression
+gzip compressed data, was "maxsmart-0.1.1.tar", last modified: Tue May 23 18:09:50 2023, max compression
```

## Comparing `maxsmart-0.1.0.tar` & `maxsmart-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-05-21 18:08:13.560228 maxsmart-0.1.0/
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)     1070 2023-05-20 20:48:25.000000 maxsmart-0.1.0/LICENSE
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)      846 2023-05-21 18:08:13.560228 maxsmart-0.1.0/PKG-INFO
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)     4535 2023-05-21 18:07:02.000000 maxsmart-0.1.0/README.md
-drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-05-21 18:08:13.560228 maxsmart-0.1.0/maxsmart/
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)       31 2023-05-20 20:48:25.000000 maxsmart-0.1.0/maxsmart/__init__.py
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)     1970 2023-05-20 20:48:25.000000 maxsmart-0.1.0/maxsmart/maxsmart.py
-drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-05-21 18:08:13.560228 maxsmart-0.1.0/maxsmart.egg-info/
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)      846 2023-05-21 18:08:13.000000 maxsmart-0.1.0/maxsmart.egg-info/PKG-INFO
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)      268 2023-05-21 18:08:13.000000 maxsmart-0.1.0/maxsmart.egg-info/SOURCES.txt
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)        1 2023-05-21 18:08:13.000000 maxsmart-0.1.0/maxsmart.egg-info/dependency_links.txt
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)        9 2023-05-21 18:08:13.000000 maxsmart-0.1.0/maxsmart.egg-info/requires.txt
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)       15 2023-05-21 18:08:13.000000 maxsmart-0.1.0/maxsmart.egg-info/top_level.txt
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)       38 2023-05-21 18:08:13.560228 maxsmart-0.1.0/setup.cfg
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)     1014 2023-05-21 18:07:02.000000 maxsmart-0.1.0/setup.py
-drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-05-21 18:08:13.560228 maxsmart-0.1.0/tests/
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)        0 2023-05-20 20:48:25.000000 maxsmart-0.1.0/tests/__init__.py
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)     1550 2023-05-20 20:48:25.000000 maxsmart-0.1.0/tests/test_maxsmart.py
+drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-05-23 18:09:50.757565 maxsmart-0.1.1/
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)     1070 2023-05-20 20:48:25.000000 maxsmart-0.1.1/LICENSE
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)      846 2023-05-23 18:09:50.757565 maxsmart-0.1.1/PKG-INFO
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)     6934 2023-05-23 18:02:07.000000 maxsmart-0.1.1/README.md
+drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-05-23 18:09:50.757565 maxsmart-0.1.1/maxsmart/
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)       31 2023-05-20 20:48:25.000000 maxsmart-0.1.1/maxsmart/__init__.py
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)     3347 2023-05-23 18:02:12.000000 maxsmart-0.1.1/maxsmart/maxsmart.py
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)     2232 2023-05-23 18:02:16.000000 maxsmart-0.1.1/maxsmart/test_script.py
+drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-05-23 18:09:50.757565 maxsmart-0.1.1/maxsmart.egg-info/
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)      846 2023-05-23 18:09:50.000000 maxsmart-0.1.1/maxsmart.egg-info/PKG-INFO
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)      292 2023-05-23 18:09:50.000000 maxsmart-0.1.1/maxsmart.egg-info/SOURCES.txt
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)        1 2023-05-23 18:09:50.000000 maxsmart-0.1.1/maxsmart.egg-info/dependency_links.txt
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)        9 2023-05-23 18:09:50.000000 maxsmart-0.1.1/maxsmart.egg-info/requires.txt
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)       15 2023-05-23 18:09:50.000000 maxsmart-0.1.1/maxsmart.egg-info/top_level.txt
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)       38 2023-05-23 18:09:50.757565 maxsmart-0.1.1/setup.cfg
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)     1014 2023-05-23 18:03:35.000000 maxsmart-0.1.1/setup.py
+drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-05-23 18:09:50.757565 maxsmart-0.1.1/tests/
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)        0 2023-05-20 20:48:25.000000 maxsmart-0.1.1/tests/__init__.py
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)     1550 2023-05-23 18:02:14.000000 maxsmart-0.1.1/tests/test_maxsmart.py
```

### Comparing `maxsmart-0.1.0/LICENSE` & `maxsmart-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `maxsmart-0.1.0/PKG-INFO` & `maxsmart-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxsmart
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python module for operating network connected power strips
 Home-page: https://github.com/superkikim/maxsmart
 Author: Akim Sissaoui
 Author-email: superkikim@sissaoui.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `maxsmart-0.1.0/maxsmart.egg-info/PKG-INFO` & `maxsmart-0.1.1/maxsmart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxsmart
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python module for operating network connected power strips
 Home-page: https://github.com/superkikim/maxsmart
 Author: Akim Sissaoui
 Author-email: superkikim@sissaoui.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `maxsmart-0.1.0/setup.py` & `maxsmart-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='maxsmart',
-    version='0.1.0',
+    version='0.1.1',
     author='Akim Sissaoui',
     author_email='superkikim@sissaoui.com',
     description='A Python module for operating network connected power strips',
     long_description='''A Python module for operating network connected power strips.
                         It provides functionality to turn on/off sockets, check their state, and retrieve power consumption data.''',
     url='https://github.com/superkikim/maxsmart',
     packages=find_packages(),
```

### Comparing `maxsmart-0.1.0/tests/test_maxsmart.py` & `maxsmart-0.1.1/tests/test_maxsmart.py`

 * *Files identical despite different names*

