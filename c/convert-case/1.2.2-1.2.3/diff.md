# Comparing `tmp/convert-case-1.2.2.tar.gz` & `tmp/convert-case-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convert-case-1.2.2.tar", last modified: Tue May 23 19:26:59 2023, max compression
+gzip compressed data, was "convert-case-1.2.3.tar", last modified: Tue May 23 19:27:02 2023, max compression
```

## Comparing `convert-case-1.2.2.tar` & `convert-case-1.2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:26:59.886263 convert-case-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-23 19:26:36.000000 convert-case-1.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 19:26:36.000000 convert-case-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-05-23 19:26:59.886263 convert-case-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-05-23 19:26:36.000000 convert-case-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:26:59.886263 convert-case-1.2.2/convert_case.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-05-23 19:26:59.000000 convert-case-1.2.2/convert_case.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-23 19:26:59.000000 convert-case-1.2.2/convert_case.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 19:26:59.000000 convert-case-1.2.2/convert_case.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-23 19:26:59.000000 convert-case-1.2.2/convert_case.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 19:26:59.000000 convert-case-1.2.2/convert_case.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-23 19:26:59.886263 convert-case-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-23 19:26:36.000000 convert-case-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:26:59.886263 convert-case-1.2.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-23 19:26:36.000000 convert-case-1.2.2/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-23 19:26:36.000000 convert-case-1.2.2/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-23 19:26:36.000000 convert-case-1.2.2/src/camel.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-23 19:26:36.000000 convert-case-1.2.2/src/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-23 19:26:36.000000 convert-case-1.2.2/src/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-23 19:26:36.000000 convert-case-1.2.2/src/kebab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-23 19:26:36.000000 convert-case-1.2.2/src/lower.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-23 19:26:36.000000 convert-case-1.2.2/src/pascal.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 19:26:36.000000 convert-case-1.2.2/src/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-23 19:26:36.000000 convert-case-1.2.2/src/sentence.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-23 19:26:36.000000 convert-case-1.2.2/src/snake.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-23 19:26:36.000000 convert-case-1.2.2/src/title.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-23 19:26:36.000000 convert-case-1.2.2/src/upper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:27:02.635835 convert-case-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-23 19:26:37.000000 convert-case-1.2.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 19:26:37.000000 convert-case-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-05-23 19:27:02.635835 convert-case-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-05-23 19:26:37.000000 convert-case-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:27:02.635835 convert-case-1.2.3/convert_case.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-05-23 19:27:02.000000 convert-case-1.2.3/convert_case.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-23 19:27:02.000000 convert-case-1.2.3/convert_case.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 19:27:02.000000 convert-case-1.2.3/convert_case.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-23 19:27:02.000000 convert-case-1.2.3/convert_case.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 19:27:02.000000 convert-case-1.2.3/convert_case.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-23 19:27:02.635835 convert-case-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-23 19:26:37.000000 convert-case-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:27:02.635835 convert-case-1.2.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-23 19:26:37.000000 convert-case-1.2.3/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-23 19:26:37.000000 convert-case-1.2.3/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-23 19:26:37.000000 convert-case-1.2.3/src/camel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-23 19:26:37.000000 convert-case-1.2.3/src/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-23 19:26:37.000000 convert-case-1.2.3/src/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-23 19:26:37.000000 convert-case-1.2.3/src/kebab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-23 19:26:37.000000 convert-case-1.2.3/src/lower.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-23 19:26:37.000000 convert-case-1.2.3/src/pascal.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 19:26:37.000000 convert-case-1.2.3/src/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-23 19:26:37.000000 convert-case-1.2.3/src/sentence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-23 19:26:37.000000 convert-case-1.2.3/src/snake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-23 19:26:37.000000 convert-case-1.2.3/src/title.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-23 19:26:37.000000 convert-case-1.2.3/src/upper.py
```

### Comparing `convert-case-1.2.2/LICENSE.md` & `convert-case-1.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `convert-case-1.2.2/PKG-INFO` & `convert-case-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convert-case
-Version: 1.2.2
+Version: 1.2.3
 Summary: Convert between string cases with built-in case inference.
 Home-page: https://github.com/JoelLefkowitz/convert-case
 Author: joellefkowitz
 Author-email: joellefkowitz@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/JoelLefkowitz/convert-case/issues
 Project-URL: CI, https://github.com/JoelLefkowitz/convert-case/actions
```

### Comparing `convert-case-1.2.2/README.md` & `convert-case-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `convert-case-1.2.2/convert_case.egg-info/PKG-INFO` & `convert-case-1.2.3/convert_case.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convert-case
-Version: 1.2.2
+Version: 1.2.3
 Summary: Convert between string cases with built-in case inference.
 Home-page: https://github.com/JoelLefkowitz/convert-case
 Author: joellefkowitz
 Author-email: joellefkowitz@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/JoelLefkowitz/convert-case/issues
 Project-URL: CI, https://github.com/JoelLefkowitz/convert-case/actions
```

### Comparing `convert-case-1.2.2/setup.cfg` & `convert-case-1.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = convert-case
-version = 1.2.2
+version = 1.2.3
 description = Convert between string cases with built-in case inference.
 url = https://github.com/JoelLefkowitz/convert-case
 license_file = LICENSE.md
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = joellefkowitz
 author_email = joellefkowitz@hotmail.com
```

### Comparing `convert-case-1.2.2/setup.py` & `convert-case-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `convert-case-1.2.2/src/__main__.py` & `convert-case-1.2.3/src/__main__.py`

 * *Files identical despite different names*

### Comparing `convert-case-1.2.2/src/lower.py` & `convert-case-1.2.3/src/lower.py`

 * *Files identical despite different names*

