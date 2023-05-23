# Comparing `tmp/path_version-0.1.49.tar.gz` & `tmp/path_version-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "path_version-0.1.49.tar", max compression
+gzip compressed data, was "path_version-0.1.6.tar", max compression
```

## Comparing `path_version-0.1.49.tar` & `path_version-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      298 2022-04-25 15:07:36.180587 path_version-0.1.49/README.md
--rw-r--r--   0        0        0      162 2022-04-25 15:10:34.418894 path_version-0.1.49/path_version.py
--rw-r--r--   0        0        0      889 2023-05-23 10:03:29.699908 path_version-0.1.49/pyproject.toml
--rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 path_version-0.1.49/setup.py
--rw-r--r--   0        0        0      831 1970-01-01 00:00:00.000000 path_version-0.1.49/PKG-INFO
+-rw-r--r--   0        0        0      298 2022-04-25 15:02:54.783266 path_version-0.1.6/README.md
+-rw-r--r--   0        0        0      162 2022-04-25 15:10:35.182886 path_version-0.1.6/path_version.py
+-rw-r--r--   0        0        0     1082 2022-06-16 17:56:06.705917 path_version-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      781 2022-06-16 17:56:07.017396 path_version-0.1.6/setup.py
+-rw-r--r--   0        0        0      678 2022-06-16 17:56:07.017820 path_version-0.1.6/PKG-INFO
```

### Comparing `path_version-0.1.49/pyproject.toml` & `path_version-0.1.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [tool.poetry]
 name = "path_version"
-version = "0.1.49"
+version = "0.1.6"
 description = "Get the last changed has of a dir as a python function"
 readme = "README.md"
 authors = ["Oxford Ionics"]
 license = "Proprietary"
 
 [[tool.poetry.source]]
 name = "oxionics"
 url = "http://pypi.oxionics.com:3141/oiuser/oxionics/+simple/"
 default = true
 
 [tool.poetry.dependencies]
-python = "^3.8"
+# We are using a slightly old PyQt5 (specified by artiq) which limits what
+# Python versions have wheels available. If we upgrade the Qt version we can
+# probably relax this Python requirement.
+python = "~3.8"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^4.0.1"
 pytest = "^6.2.5"
 black = "22.3.0"
 pre-commit = "^2.17.0"
```

### Comparing `path_version-0.1.49/setup.py` & `path_version-0.1.6/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
 ['path_version']
 setup_kwargs = {
     'name': 'path-version',
-    'version': '0.1.49',
+    'version': '0.1.6',
     'description': 'Get the last changed has of a dir as a python function',
     'long_description': '# Path Version\n\nHelper to get the git hash of the last change to a particular sub-directory\nin a repository.\n\nNeeds to be a separate package so that we can install it in the same virtualenv\nas poetry and poetry-dynamic-versioning at least until we have poetry 1.2 and\nproper poetry plugin support.\n',
     'author': 'Oxford Ionics',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
+    'author_email': None,
+    'maintainer': None,
+    'maintainer_email': None,
+    'url': None,
     'py_modules': modules,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.8,<3.9',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `path_version-0.1.49/PKG-INFO` & `path_version-0.1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: path-version
-Version: 0.1.49
+Version: 0.1.6
 Summary: Get the last changed has of a dir as a python function
 License: Proprietary
 Author: Oxford Ionics
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8,<3.9
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Path Version
 
 Helper to get the git hash of the last change to a particular sub-directory
 in a repository.
```

