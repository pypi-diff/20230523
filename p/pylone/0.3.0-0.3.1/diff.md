# Comparing `tmp/pylone-0.3.0.tar.gz` & `tmp/pylone-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylone-0.3.0.tar", last modified: Thu Jun 16 13:34:23 2022, max compression
+gzip compressed data, was "pylone-0.3.1.tar", last modified: Tue May 23 09:32:15 2023, max compression
```

## Comparing `pylone-0.3.0.tar` & `pylone-0.3.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 13:34:23.300139 pylone-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2413 2022-06-16 13:34:23.300139 pylone-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1675 2022-06-16 13:34:21.000000 pylone-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 13:34:23.296139 pylone-0.3.0/pylone/
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2163 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/apis.py
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)      687 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 13:34:23.300139 pylone-0.3.0/pylone/providers/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 13:34:23.300139 pylone-0.3.0/pylone/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4291 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/providers/aws/function.py
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/providers/aws/iam.py
--rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/providers/aws/layer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/providers/aws/s3.py
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/providers/aws/shared.py
--rw-r--r--   0 runner    (1001) docker     (121)     3186 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/pylone.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 13:34:23.300139 pylone-0.3.0/pylone/questions/
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/questions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/questions/create_function.py
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/questions/create_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/questions/credentials.py
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/questions/global_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 13:34:23.300139 pylone-0.3.0/pylone/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/utils/changes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1016 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/utils/checksum.py
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/utils/constructors.py
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/utils/dirs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/utils/doppler.py
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/utils/gitignore.py
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/utils/scripts.py
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-06-16 13:34:21.000000 pylone-0.3.0/pylone/utils/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 13:34:23.300139 pylone-0.3.0/pylone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2413 2022-06-16 13:34:22.000000 pylone-0.3.0/pylone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-06-16 13:34:23.000000 pylone-0.3.0/pylone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-16 13:34:22.000000 pylone-0.3.0/pylone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-06-16 13:34:22.000000 pylone-0.3.0/pylone.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-06-16 13:34:23.000000 pylone-0.3.0/pylone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-06-16 13:34:23.000000 pylone-0.3.0/pylone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-16 13:34:23.300139 pylone-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-06-16 13:34:21.000000 pylone-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 09:32:15.888428 pylone-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-05-23 09:32:15.888428 pylone-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1852 2023-05-23 09:32:15.000000 pylone-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 09:32:15.884428 pylone-0.3.1/pylone/
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      292 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/apis.py
+-rw-r--r--   0 runner    (1001) docker     (122)      637 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1104 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 09:32:15.884428 pylone-0.3.1/pylone/providers/
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 09:32:15.884428 pylone-0.3.1/pylone/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (122)      747 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4291 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/providers/aws/function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      348 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/providers/aws/iam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1458 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/providers/aws/layer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1693 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/providers/aws/s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/providers/aws/shared.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3186 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/pylone.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 09:32:15.884428 pylone-0.3.1/pylone/questions/
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/questions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/questions/create_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/questions/create_layer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/questions/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/questions/global_config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 09:32:15.888428 pylone-0.3.1/pylone/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/utils/changes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/utils/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/utils/constructors.py
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/utils/dirs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1036 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/utils/doppler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/utils/gitignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/utils/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone/utils/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 09:32:15.884428 pylone-0.3.1/pylone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      942 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-23 09:32:15.000000 pylone-0.3.1/pylone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 09:32:15.888428 pylone-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1285 2023-05-23 09:32:15.000000 pylone-0.3.1/setup.py
```

### Comparing `pylone-0.3.0/PKG-INFO` & `pylone-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylone
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python Serverless framework
 Home-page: https://github.com/mathix420/pylone
 Author: Arnaud Gissinger
 Author-email: agissing@student.42.fr
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -14,26 +14,35 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-<img src="https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/120/google/223/tokyo-tower_1f5fc.png" width="100" height="100" align="right" alt="Pylone icon">
+<img src="https://em-content.zobj.net/thumbs/160/google/350/tokyo-tower_1f5fc.png" width="100" height="100" align="right" alt="Pylone icon">
 
 # PYLONE
 
 **Python CD framework**
 
 [![Pypi](https://badgen.net/pypi/v/pylone)](https://pypi.org/project/pylone/)
 [![Docker Pulls](https://badgen.net/docker/pulls/plsr/pylone?icon=docker&label=pulls)](https://hub.docker.com/r/plsr/pylone/)
 
 [![wakatime](https://wakatime.com/badge/github/mathix420/pylone.svg)](https://wakatime.com/badge/github/mathix420/pylone)
 [![Maintainability](https://api.codeclimate.com/v1/badges/fc078176e896556db324/maintainability)](https://codeclimate.com/github/mathix420/pylone/maintainability)
 
+# Features
+
+- Publish, update and delete Lambdas
+- Publish, update and delete Layers
+- [Doppler](https://doppler.com) integration
+- Simple and light wieght
+- Multi stages lambdas
+- Before/after deploy hooks
+
 # Usage
 
 ## Pylone usage
 
 ```bash
 pylone -h
 ```
```

### Comparing `pylone-0.3.0/README.md` & `pylone-0.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,28 @@
-<img src="https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/120/google/223/tokyo-tower_1f5fc.png" width="100" height="100" align="right" alt="Pylone icon">
+<img src="https://em-content.zobj.net/thumbs/160/google/350/tokyo-tower_1f5fc.png" width="100" height="100" align="right" alt="Pylone icon">
 
 # PYLONE
 
 **Python CD framework**
 
 [![Pypi](https://badgen.net/pypi/v/pylone)](https://pypi.org/project/pylone/)
 [![Docker Pulls](https://badgen.net/docker/pulls/plsr/pylone?icon=docker&label=pulls)](https://hub.docker.com/r/plsr/pylone/)
 
 [![wakatime](https://wakatime.com/badge/github/mathix420/pylone.svg)](https://wakatime.com/badge/github/mathix420/pylone)
 [![Maintainability](https://api.codeclimate.com/v1/badges/fc078176e896556db324/maintainability)](https://codeclimate.com/github/mathix420/pylone/maintainability)
 
+# Features
+
+- Publish, update and delete Lambdas
+- Publish, update and delete Layers
+- [Doppler](https://doppler.com) integration
+- Simple and light wieght
+- Multi stages lambdas
+- Before/after deploy hooks
+
 # Usage
 
 ## Pylone usage
 
 ```bash
 pylone -h
 ```
```

### Comparing `pylone-0.3.0/pylone/__main__.py` & `pylone-0.3.1/pylone/__main__.py`

 * *Files identical despite different names*

### Comparing `pylone-0.3.0/pylone/config.py` & `pylone-0.3.1/pylone/config.py`

 * *Files identical despite different names*

### Comparing `pylone-0.3.0/pylone/functions.py` & `pylone-0.3.1/pylone/functions.py`

 * *Files identical despite different names*

### Comparing `pylone-0.3.0/pylone/handlers.py` & `pylone-0.3.1/pylone/handlers.py`

 * *Files identical despite different names*

### Comparing `pylone-0.3.0/pylone/layers.py` & `pylone-0.3.1/pylone/layers.py`

 * *Files identical despite different names*

### Comparing `pylone-0.3.0/pylone/providers/aws/__init__.py` & `pylone-0.3.1/pylone/providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `pylone-0.3.0/pylone/providers/aws/function.py` & `pylone-0.3.1/pylone/providers/aws/function.py`

 * *Files identical despite different names*

### Comparing `pylone-0.3.0/pylone/providers/aws/layer.py` & `pylone-0.3.1/pylone/providers/aws/layer.py`

 * *Files identical despite different names*

### Comparing `pylone-0.3.0/pylone/providers/aws/s3.py` & `pylone-0.3.1/pylone/providers/aws/s3.py`

 * *Files identical despite different names*

### Comparing `pylone-0.3.0/pylone/providers/aws/shared.py` & `pylone-0.3.1/pylone/providers/aws/shared.py`

 * *Files identical despite different names*

### Comparing `pylone-0.3.0/pylone/pylone.py` & `pylone-0.3.1/pylone/pylone.py`

 * *Files identical despite different names*

### Comparing `pylone-0.3.0/pylone/questions/__init__.py` & `pylone-0.3.1/pylone/questions/__init__.py`

 * *Files identical despite different names*

### Comparing `pylone-0.3.0/pylone/questions/create_function.py` & `pylone-0.3.1/pylone/questions/create_function.py`

 * *Files identical despite different names*

### Comparing `pylone-0.3.0/pylone/questions/create_layer.py` & `pylone-0.3.1/pylone/questions/create_layer.py`

 * *Files identical despite different names*

### Comparing `pylone-0.3.0/pylone/questions/global_config.py` & `pylone-0.3.1/pylone/questions/global_config.py`

 * *Files identical despite different names*

### Comparing `pylone-0.3.0/pylone/utils/changes.py` & `pylone-0.3.1/pylone/utils/changes.py`

 * *Files identical despite different names*

### Comparing `pylone-0.3.0/pylone/utils/checksum.py` & `pylone-0.3.1/pylone/utils/checksum.py`

 * *Files identical despite different names*

### Comparing `pylone-0.3.0/pylone/utils/doppler.py` & `pylone-0.3.1/pylone/utils/doppler.py`

 * *Files identical despite different names*

### Comparing `pylone-0.3.0/pylone.egg-info/PKG-INFO` & `pylone-0.3.1/pylone.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylone
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python Serverless framework
 Home-page: https://github.com/mathix420/pylone
 Author: Arnaud Gissinger
 Author-email: agissing@student.42.fr
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -14,26 +14,35 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-<img src="https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/120/google/223/tokyo-tower_1f5fc.png" width="100" height="100" align="right" alt="Pylone icon">
+<img src="https://em-content.zobj.net/thumbs/160/google/350/tokyo-tower_1f5fc.png" width="100" height="100" align="right" alt="Pylone icon">
 
 # PYLONE
 
 **Python CD framework**
 
 [![Pypi](https://badgen.net/pypi/v/pylone)](https://pypi.org/project/pylone/)
 [![Docker Pulls](https://badgen.net/docker/pulls/plsr/pylone?icon=docker&label=pulls)](https://hub.docker.com/r/plsr/pylone/)
 
 [![wakatime](https://wakatime.com/badge/github/mathix420/pylone.svg)](https://wakatime.com/badge/github/mathix420/pylone)
 [![Maintainability](https://api.codeclimate.com/v1/badges/fc078176e896556db324/maintainability)](https://codeclimate.com/github/mathix420/pylone/maintainability)
 
+# Features
+
+- Publish, update and delete Lambdas
+- Publish, update and delete Layers
+- [Doppler](https://doppler.com) integration
+- Simple and light wieght
+- Multi stages lambdas
+- Before/after deploy hooks
+
 # Usage
 
 ## Pylone usage
 
 ```bash
 pylone -h
 ```
```

### Comparing `pylone-0.3.0/pylone.egg-info/SOURCES.txt` & `pylone-0.3.1/pylone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylone-0.3.0/setup.py` & `pylone-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='pylone',
-    version='0.3.0',
+    version='0.3.1',
     description='A Python Serverless framework',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/mathix420/pylone',
     author='Arnaud Gissinger',
     author_email='agissing@student.42.fr',
     license='MIT',
@@ -24,14 +24,14 @@
                 'Programming Language :: Python :: 3.7',
                 'Programming Language :: Python :: 3.8',
                 'Programming Language :: Python :: 3.9',
     ],
     install_requires=[
         'python-dotenv>=0.10.5',
         'PyInquirer>=1.0.3',
-        'requests==2.27.1',
+        'requests==2.31.0',
         'boto3>=1.10.24',
         'PyYAML>=3.13',
     ],
     packages=find_namespace_packages(include=["pylone", "pylone.*"]),
     entry_points={'console_scripts': ['pylone=pylone.__main__:main']},
 )
```

