# Comparing `tmp/vasp_suite-0.3.4.tar.gz` & `tmp/vasp_suite-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vasp_suite-0.3.4.tar", last modified: Tue Jan 24 16:04:33 2023, max compression
+gzip compressed data, was "vasp_suite-1.0.0.tar", last modified: Tue May 23 15:01:05 2023, max compression
```

## Comparing `vasp_suite-0.3.4.tar` & `vasp_suite-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 16:04:33.395591 vasp_suite-0.3.4/
--rw-rw-rw-   0 root         (0) root         (0)    35079 2023-01-24 16:03:51.000000 vasp_suite-0.3.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3381 2023-01-24 16:04:33.394591 vasp_suite-0.3.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2933 2023-01-24 16:03:51.000000 vasp_suite-0.3.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-01-24 16:03:51.000000 vasp_suite-0.3.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-24 16:04:33.395591 vasp_suite-0.3.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1332 2023-01-24 16:04:29.000000 vasp_suite-0.3.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 16:04:33.389590 vasp_suite-0.3.4/vasp_suite/
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-01-24 16:03:51.000000 vasp_suite-0.3.4/vasp_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-01-24 16:04:29.000000 vasp_suite-0.3.4/vasp_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)     7355 2023-01-24 16:03:51.000000 vasp_suite-0.3.4/vasp_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     3521 2023-01-24 16:03:51.000000 vasp_suite-0.3.4/vasp_suite/config.py
--rw-rw-rw-   0 root         (0) root         (0)     9606 2023-01-24 16:03:51.000000 vasp_suite-0.3.4/vasp_suite/file_transform.py
--rw-rw-rw-   0 root         (0) root         (0)    11663 2023-01-24 16:03:51.000000 vasp_suite-0.3.4/vasp_suite/input.py
--rw-rw-rw-   0 root         (0) root         (0)     2902 2023-01-24 16:03:51.000000 vasp_suite-0.3.4/vasp_suite/plotter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 16:04:33.392591 vasp_suite-0.3.4/vasp_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3381 2023-01-24 16:04:33.000000 vasp_suite-0.3.4/vasp_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      406 2023-01-24 16:04:33.000000 vasp_suite-0.3.4/vasp_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-24 16:04:33.000000 vasp_suite-0.3.4/vasp_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-01-24 16:04:33.000000 vasp_suite-0.3.4/vasp_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-01-24 16:04:33.000000 vasp_suite-0.3.4/vasp_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-01-24 16:04:33.000000 vasp_suite-0.3.4/vasp_suite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:01:05.949262 vasp_suite-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35079 2023-05-23 15:00:48.000000 vasp_suite-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-05-23 15:01:05.949262 vasp_suite-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2933 2023-05-23 15:00:48.000000 vasp_suite-1.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-05-23 15:00:48.000000 vasp_suite-1.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 15:01:05.949262 vasp_suite-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2023-05-23 15:01:02.000000 vasp_suite-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:01:05.947262 vasp_suite-1.0.0/vasp_suite/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-05-23 15:00:48.000000 vasp_suite-1.0.0/vasp_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-05-23 15:01:02.000000 vasp_suite-1.0.0/vasp_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10476 2023-05-23 15:00:48.000000 vasp_suite-1.0.0/vasp_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     3362 2023-05-23 15:00:48.000000 vasp_suite-1.0.0/vasp_suite/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    16932 2023-05-23 15:00:48.000000 vasp_suite-1.0.0/vasp_suite/ewald.py
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2023-05-23 15:00:48.000000 vasp_suite-1.0.0/vasp_suite/input.py
+-rw-rw-rw-   0 root         (0) root         (0)    16803 2023-05-23 15:00:48.000000 vasp_suite-1.0.0/vasp_suite/structure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1711 2023-05-23 15:00:48.000000 vasp_suite-1.0.0/vasp_suite/submission.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:01:05.949262 vasp_suite-1.0.0/vasp_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-05-23 15:01:05.000000 vasp_suite-1.0.0/vasp_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      422 2023-05-23 15:01:05.000000 vasp_suite-1.0.0/vasp_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 15:01:05.000000 vasp_suite-1.0.0/vasp_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-05-23 15:01:05.000000 vasp_suite-1.0.0/vasp_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-23 15:01:05.000000 vasp_suite-1.0.0/vasp_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-23 15:01:05.000000 vasp_suite-1.0.0/vasp_suite.egg-info/top_level.txt
```

### Comparing `vasp_suite-0.3.4/LICENSE` & `vasp_suite-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vasp_suite-0.3.4/PKG-INFO` & `vasp_suite-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp_suite
-Version: 0.3.4
+Version: 1.0.0
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `vasp_suite-0.3.4/README.md` & `vasp_suite-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `vasp_suite-0.3.4/setup.py` & `vasp_suite-1.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 # pylint: disable=line-too-long,missing-module-docstring,exec-used
 import setuptools
 
 # DO NOT EDIT THIS NUMBER!
 # It is changed automatically by python-semantic-release
-__version__ = "0.3.4"
+__version__ = "1.0.0"
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name='vasp_suite',
     version=__version__,
@@ -29,14 +29,16 @@
         'Operating System :: OS Independent'
         ],
     packages=setuptools.find_packages(),
     python_requires='>=3.6',
     install_requires=[
         'numpy',
         'gemmi',
+        'matplotlib',
+        'scipy',
         ],
     entry_points={
         'console_scripts': [
             'vasp_suite = vasp_suite.cli:main'
             ]
         }
     )
```

### Comparing `vasp_suite-0.3.4/vasp_suite.egg-info/PKG-INFO` & `vasp_suite-1.0.0/vasp_suite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp-suite
-Version: 0.3.4
+Version: 1.0.0
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

