# Comparing `tmp/jtbl-1.5.1.tar.gz` & `tmp/jtbl-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jtbl-1.5.1.tar", last modified: Wed Mar  1 00:42:53 2023, max compression
+gzip compressed data, was "jtbl-1.5.2.tar", last modified: Mon May 22 23:49:37 2023, max compression
```

## Comparing `jtbl-1.5.1.tar` & `jtbl-1.5.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kelly      (501) staff       (20)        0 2023-03-01 00:42:53.099064 jtbl-1.5.1/
--rw-r--r--   0 kelly      (501) staff       (20)     2284 2023-03-01 00:31:50.000000 jtbl-1.5.1/CHANGELOG
--rw-r--r--   0 kelly      (501) staff       (20)     1069 2023-01-12 03:28:22.000000 jtbl-1.5.1/LICENSE
--rw-r--r--   0 kelly      (501) staff       (20)       36 2023-01-12 03:28:22.000000 jtbl-1.5.1/MANIFEST.in
--rw-r--r--   0 kelly      (501) staff       (20)    15959 2023-03-01 00:42:53.099305 jtbl-1.5.1/PKG-INFO
--rw-r--r--   0 kelly      (501) staff       (20)    15435 2023-01-12 03:28:22.000000 jtbl-1.5.1/README.md
-drwxr-xr-x   0 kelly      (501) staff       (20)        0 2023-03-01 00:42:53.094217 jtbl-1.5.1/jtbl/
--rw-r--r--   0 kelly      (501) staff       (20)        0 2023-01-12 03:28:22.000000 jtbl-1.5.1/jtbl/__init__.py
--rw-r--r--   0 kelly      (501) staff       (20)       33 2023-01-12 03:28:22.000000 jtbl-1.5.1/jtbl/__main__.py
--rw-r--r--   0 kelly      (501) staff       (20)    10669 2023-03-01 00:32:02.000000 jtbl-1.5.1/jtbl/cli.py
-drwxr-xr-x   0 kelly      (501) staff       (20)        0 2023-03-01 00:42:53.097321 jtbl-1.5.1/jtbl.egg-info/
--rw-r--r--   0 kelly      (501) staff       (20)    15959 2023-03-01 00:42:52.000000 jtbl-1.5.1/jtbl.egg-info/PKG-INFO
--rw-r--r--   0 kelly      (501) staff       (20)      285 2023-03-01 00:42:52.000000 jtbl-1.5.1/jtbl.egg-info/SOURCES.txt
--rw-r--r--   0 kelly      (501) staff       (20)        1 2023-03-01 00:42:52.000000 jtbl-1.5.1/jtbl.egg-info/dependency_links.txt
--rw-r--r--   0 kelly      (501) staff       (20)       39 2023-03-01 00:42:52.000000 jtbl-1.5.1/jtbl.egg-info/entry_points.txt
--rw-r--r--   0 kelly      (501) staff       (20)       16 2023-03-01 00:42:52.000000 jtbl-1.5.1/jtbl.egg-info/requires.txt
--rw-r--r--   0 kelly      (501) staff       (20)        5 2023-03-01 00:42:52.000000 jtbl-1.5.1/jtbl.egg-info/top_level.txt
-drwxr-xr-x   0 kelly      (501) staff       (20)        0 2023-03-01 00:42:53.098467 jtbl-1.5.1/man/
--rw-r--r--   0 kelly      (501) staff       (20)     1343 2023-03-01 00:33:36.000000 jtbl-1.5.1/man/jtbl.1
--rw-r--r--   0 kelly      (501) staff       (20)       73 2023-03-01 00:42:53.100994 jtbl-1.5.1/setup.cfg
--rwxr-xr-x   0 kelly      (501) staff       (20)      946 2023-03-01 00:32:21.000000 jtbl-1.5.1/setup.py
+drwxr-xr-x   0 kelly      (501) staff       (20)        0 2023-05-22 23:49:37.420615 jtbl-1.5.2/
+-rw-r--r--   0 kelly      (501) staff       (20)     2330 2023-05-22 23:44:51.000000 jtbl-1.5.2/CHANGELOG
+-rw-r--r--   0 kelly      (501) staff       (20)     1069 2023-01-12 03:28:22.000000 jtbl-1.5.2/LICENSE
+-rw-r--r--   0 kelly      (501) staff       (20)       36 2023-01-12 03:28:22.000000 jtbl-1.5.2/MANIFEST.in
+-rw-r--r--   0 kelly      (501) staff       (20)    15959 2023-05-22 23:49:37.421123 jtbl-1.5.2/PKG-INFO
+-rw-r--r--   0 kelly      (501) staff       (20)    15435 2023-01-12 03:28:22.000000 jtbl-1.5.2/README.md
+drwxr-xr-x   0 kelly      (501) staff       (20)        0 2023-05-22 23:49:37.416513 jtbl-1.5.2/jtbl/
+-rw-r--r--   0 kelly      (501) staff       (20)        0 2023-01-12 03:28:22.000000 jtbl-1.5.2/jtbl/__init__.py
+-rw-r--r--   0 kelly      (501) staff       (20)       33 2023-01-12 03:28:22.000000 jtbl-1.5.2/jtbl/__main__.py
+-rw-r--r--   0 kelly      (501) staff       (20)    10740 2023-05-22 23:37:49.000000 jtbl-1.5.2/jtbl/cli.py
+drwxr-xr-x   0 kelly      (501) staff       (20)        0 2023-05-22 23:49:37.419325 jtbl-1.5.2/jtbl.egg-info/
+-rw-r--r--   0 kelly      (501) staff       (20)    15959 2023-05-22 23:49:37.000000 jtbl-1.5.2/jtbl.egg-info/PKG-INFO
+-rw-r--r--   0 kelly      (501) staff       (20)      285 2023-05-22 23:49:37.000000 jtbl-1.5.2/jtbl.egg-info/SOURCES.txt
+-rw-r--r--   0 kelly      (501) staff       (20)        1 2023-05-22 23:49:37.000000 jtbl-1.5.2/jtbl.egg-info/dependency_links.txt
+-rw-r--r--   0 kelly      (501) staff       (20)       39 2023-05-22 23:49:37.000000 jtbl-1.5.2/jtbl.egg-info/entry_points.txt
+-rw-r--r--   0 kelly      (501) staff       (20)       16 2023-05-22 23:49:37.000000 jtbl-1.5.2/jtbl.egg-info/requires.txt
+-rw-r--r--   0 kelly      (501) staff       (20)        5 2023-05-22 23:49:37.000000 jtbl-1.5.2/jtbl.egg-info/top_level.txt
+drwxr-xr-x   0 kelly      (501) staff       (20)        0 2023-05-22 23:49:37.419847 jtbl-1.5.2/man/
+-rw-r--r--   0 kelly      (501) staff       (20)     1343 2023-03-01 00:33:36.000000 jtbl-1.5.2/man/jtbl.1
+-rw-r--r--   0 kelly      (501) staff       (20)       73 2023-05-22 23:49:37.422327 jtbl-1.5.2/setup.cfg
+-rwxr-xr-x   0 kelly      (501) staff       (20)      946 2023-05-22 23:45:18.000000 jtbl-1.5.2/setup.py
```

### Comparing `jtbl-1.5.1/CHANGELOG` & `jtbl-1.5.2/CHANGELOG`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 jtbl changelog
 
+20230522 v1.5.2
+- Fix output for empty array
+
 20230228 v1.5.1
 - Preserve long float formatting
 
 20230114 v1.5.0
 - Be more tolerant of loading JSON Lines with blank lines and whitespace
 
 20221006 v1.4.0
```

### Comparing `jtbl-1.5.1/LICENSE` & `jtbl-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jtbl-1.5.1/PKG-INFO` & `jtbl-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jtbl
-Version: 1.5.1
+Version: 1.5.2
 Summary: A simple cli tool to print JSON and JSON Lines data as a table in the terminal.
 Home-page: https://github.com/kellyjonbrazil/jtbl
 Author: Kelly Brazil
 Author-email: kellyjonbrazil@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jtbl-1.5.1/README.md` & `jtbl-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `jtbl-1.5.1/jtbl/cli.py` & `jtbl-1.5.2/jtbl/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import signal
 import textwrap
 import csv
 import json
 import tabulate
 import shutil
 
-__version__ = '1.5.1'
+__version__ = '1.5.2'
 SUCCESS, ERROR = True, False
 
 
 def ctrlc(signum, frame):
     """exit with error on SIGINT"""
     sys.exit(1)
 
@@ -168,14 +168,19 @@
             return (ERROR, textwrap.dedent(f'''\
                 jtbl:  Cannot parse the data (Not JSON or JSON Lines data):
                        {str(data)[0:columns - 8]}
                        '''))
 
         return SUCCESS, data
 
+    if data == []:
+        return SUCCESS, ''
+
+    return ERROR, data
+
 
 def get_headers(data):
     """scan the data and return a dictionary of all of the headers in order"""
     headers = []
 
     if isinstance(data, dict):
         headers.append(data.keys())
```

### Comparing `jtbl-1.5.1/jtbl.egg-info/PKG-INFO` & `jtbl-1.5.2/jtbl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jtbl
-Version: 1.5.1
+Version: 1.5.2
 Summary: A simple cli tool to print JSON and JSON Lines data as a table in the terminal.
 Home-page: https://github.com/kellyjonbrazil/jtbl
 Author: Kelly Brazil
 Author-email: kellyjonbrazil@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jtbl-1.5.1/man/jtbl.1` & `jtbl-1.5.2/man/jtbl.1`

 * *Files identical despite different names*

### Comparing `jtbl-1.5.1/setup.py` & `jtbl-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='jtbl',
-    version='1.5.1',
+    version='1.5.2',
     author='Kelly Brazil',
     author_email='kellyjonbrazil@gmail.com',
     description='A simple cli tool to print JSON and JSON Lines data as a table in the terminal.',
     install_requires=[
         'tabulate>=0.8.6'
     ],
     license='MIT',
```

