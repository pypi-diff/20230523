# Comparing `tmp/addana-0.0.6.tar.gz` & `tmp/addana-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "addana-0.0.6.tar", last modified: Fri Mar  3 10:06:24 2023, max compression
+gzip compressed data, was "addana-0.0.9.tar", last modified: Fri Mar  3 10:14:07 2023, max compression
```

## Comparing `addana-0.0.6.tar` & `addana-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:06:24.362696 addana-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-03 10:06:10.000000 addana-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-03 10:06:10.000000 addana-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-03-03 10:06:24.362696 addana-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-03 10:06:10.000000 addana-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:06:24.362696 addana-0.0.6/addana/
--rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-03-03 10:06:10.000000 addana-0.0.6/addana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-03-03 10:06:10.000000 addana-0.0.6/addana/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-03-03 10:06:10.000000 addana-0.0.6/addana/drawer.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-03 10:06:10.000000 addana-0.0.6/addana/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)   269005 2023-03-03 10:06:10.000000 addana-0.0.6/addana/pca.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-03-03 10:06:10.000000 addana-0.0.6/addana/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:06:24.362696 addana-0.0.6/addana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-03-03 10:06:24.000000 addana-0.0.6/addana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-03 10:06:24.000000 addana-0.0.6/addana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-03 10:06:24.000000 addana-0.0.6/addana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 10:06:24.000000 addana-0.0.6/addana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-03 10:06:24.000000 addana-0.0.6/addana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-03 10:06:24.000000 addana-0.0.6/addana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-03 10:06:10.000000 addana-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-03 10:06:24.362696 addana-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-03-03 10:06:10.000000 addana-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:14:07.208684 addana-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-03 10:13:54.000000 addana-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-03 10:13:54.000000 addana-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-03-03 10:14:07.208684 addana-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-03 10:13:54.000000 addana-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:14:07.208684 addana-0.0.9/addana/
+-rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-03-03 10:13:54.000000 addana-0.0.9/addana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-03-03 10:13:54.000000 addana-0.0.9/addana/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-03-03 10:13:54.000000 addana-0.0.9/addana/drawer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-03 10:13:54.000000 addana-0.0.9/addana/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-03-03 10:13:54.000000 addana-0.0.9/addana/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:14:07.208684 addana-0.0.9/addana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-03-03 10:14:07.000000 addana-0.0.9/addana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-03 10:14:07.000000 addana-0.0.9/addana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-03 10:14:07.000000 addana-0.0.9/addana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 10:14:07.000000 addana-0.0.9/addana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-03 10:14:07.000000 addana-0.0.9/addana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-03 10:14:07.000000 addana-0.0.9/addana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-03 10:13:54.000000 addana-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-03 10:14:07.208684 addana-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-03-03 10:13:54.000000 addana-0.0.9/setup.py
```

### Comparing `addana-0.0.6/LICENSE` & `addana-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `addana-0.0.6/PKG-INFO` & `addana-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: addana
-Version: 0.0.6
+Version: 0.0.9
 Summary: address
 Home-page: https://github.com/advancehs/addana
 Author: advancehs
 Author-email: 1019753743@11.com
 License: MIT license
 Keywords: addana
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `addana-0.0.6/README.md` & `addana-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `addana-0.0.6/addana/__init__.py` & `addana-0.0.9/addana/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 except ImportError:
     from collections import Iterable
 import pandas as pd
 
 from .structures import AddrMap, Pca
 from .structures import P, C, A
 
-__version__ = '0.0.6'
+__version__ = '0.0.9'
 
 pwd_path = os.path.abspath(os.path.dirname(__file__))
 # 区划地址文件
 pca_path = os.path.join(pwd_path, 'data\pca.csv')
 
 if six.PY2:
     text_type = unicode
```

### Comparing `addana-0.0.6/addana/__main__.py` & `addana-0.0.9/addana/__main__.py`

 * *Files identical despite different names*

### Comparing `addana-0.0.6/addana/drawer.py` & `addana-0.0.9/addana/drawer.py`

 * *Files identical despite different names*

### Comparing `addana-0.0.6/addana/structures.py` & `addana-0.0.9/addana/structures.py`

 * *Files identical despite different names*

### Comparing `addana-0.0.6/addana.egg-info/PKG-INFO` & `addana-0.0.9/addana.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: addana
-Version: 0.0.6
+Version: 0.0.9
 Summary: address
 Home-page: https://github.com/advancehs/addana
 Author: advancehs
 Author-email: 1019753743@11.com
 License: MIT license
 Keywords: addana
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `addana-0.0.6/setup.py` & `addana-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,18 +44,21 @@
     dependency_links=dependency_links,
     license="MIT license",
     long_description=readme,
     long_description_content_type='text/markdown',
     include_package_data=True,
     keywords='addana',
     name='addana',
-    packages=find_packages(include=['addana', 'addana.*','addana.data']),
+    packages=find_packages(exclude=['tests']),
+    package_dir={'addana': 'addana'},
     package_data={
         'addana': ['*.*'],
+        'addana': ['*.*.*'],
+        'addana.data': ['*.*.*'], 
     },
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/advancehs/addana',
-    version='0.0.6',
+    version='0.0.9',
     zip_safe=False,
 )
```

