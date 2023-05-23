# Comparing `tmp/cfg-argparser-1.1.4.post1.tar.gz` & `tmp/cfg-argparser-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfg-argparser-1.1.4.post1.tar", last modified: Thu May 18 20:28:52 2023, max compression
+gzip compressed data, was "cfg-argparser-1.1.5.tar", last modified: Tue May 23 20:56:34 2023, max compression
```

## Comparing `cfg-argparser-1.1.4.post1.tar` & `cfg-argparser-1.1.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-18 20:28:52.761670 cfg-argparser-1.1.4.post1/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1071 2023-04-12 20:40:08.000000 cfg-argparser-1.1.4.post1/LICENSE
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2126 2023-05-18 20:28:52.761670 cfg-argparser-1.1.4.post1/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1287 2023-05-18 20:28:23.000000 cfg-argparser-1.1.4.post1/README.md
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      876 2023-05-18 20:28:27.000000 cfg-argparser-1.1.4.post1/pyproject.toml
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       38 2023-05-18 20:28:52.761670 cfg-argparser-1.1.4.post1/setup.cfg
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-18 20:28:52.761670 cfg-argparser-1.1.4.post1/src/
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-18 20:28:52.761670 cfg-argparser-1.1.4.post1/src/cfg_argparser/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      104 2023-04-12 21:18:54.000000 cfg-argparser-1.1.4.post1/src/cfg_argparser/__init__.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)    12446 2023-05-18 20:25:57.000000 cfg-argparser-1.1.4.post1/src/cfg_argparser/config_arg_parser.py
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-18 20:28:52.761670 cfg-argparser-1.1.4.post1/src/cfg_argparser.egg-info/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2126 2023-05-18 20:28:52.000000 cfg-argparser-1.1.4.post1/src/cfg_argparser.egg-info/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      265 2023-05-18 20:28:52.000000 cfg-argparser-1.1.4.post1/src/cfg_argparser.egg-info/SOURCES.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)        1 2023-05-18 20:28:52.000000 cfg-argparser-1.1.4.post1/src/cfg_argparser.egg-info/dependency_links.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       14 2023-05-18 20:28:52.000000 cfg-argparser-1.1.4.post1/src/cfg_argparser.egg-info/top_level.txt
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-23 20:56:34.949829 cfg-argparser-1.1.5/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1071 2023-04-12 20:40:08.000000 cfg-argparser-1.1.5/LICENSE
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2118 2023-05-23 20:56:34.949829 cfg-argparser-1.1.5/PKG-INFO
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1285 2023-05-23 20:53:17.000000 cfg-argparser-1.1.5/README.md
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      874 2023-05-23 20:51:42.000000 cfg-argparser-1.1.5/pyproject.toml
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       38 2023-05-23 20:56:34.949829 cfg-argparser-1.1.5/setup.cfg
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-23 20:56:34.946496 cfg-argparser-1.1.5/src/
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-23 20:56:34.949829 cfg-argparser-1.1.5/src/cfg_argparser/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      125 2023-05-18 23:35:00.000000 cfg-argparser-1.1.5/src/cfg_argparser/__init__.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2395 2023-05-18 23:40:33.000000 cfg-argparser-1.1.5/src/cfg_argparser/cfg_dict.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)    10048 2023-05-18 23:34:21.000000 cfg-argparser-1.1.5/src/cfg_argparser/config_arg_parser.py
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-23 20:56:34.949829 cfg-argparser-1.1.5/src/cfg_argparser.egg-info/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2118 2023-05-23 20:56:34.000000 cfg-argparser-1.1.5/src/cfg_argparser.egg-info/PKG-INFO
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      295 2023-05-23 20:56:34.000000 cfg-argparser-1.1.5/src/cfg_argparser.egg-info/SOURCES.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)        1 2023-05-23 20:56:34.000000 cfg-argparser-1.1.5/src/cfg_argparser.egg-info/dependency_links.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       14 2023-05-23 20:56:34.000000 cfg-argparser-1.1.5/src/cfg_argparser.egg-info/top_level.txt
```

### Comparing `cfg-argparser-1.1.4.post1/LICENSE` & `cfg-argparser-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cfg-argparser-1.1.4.post1/PKG-INFO` & `cfg-argparser-1.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfg-argparser
-Version: 1.1.4.post1
+Version: 1.1.5
 Summary: A package designed to simplify configurable defaults from argparse.
 Author-email: Zeptofine <zeptofine@gmail.com>
 Project-URL: Homepage, https://github.com/zeptofine/cfg-argparser
 Project-URL: Bug Tracker, https://github.com/zeptofine/cfg-argparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# cfg_argparser 1.1.4-1
+# cfg_argparser 1.1.5
 
 a config wrapper I made to be easily applied to argparse objects.
 
 ## Installation
 
 ```bash
 # from pypi:
```

### Comparing `cfg-argparser-1.1.4.post1/README.md` & `cfg-argparser-1.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# cfg_argparser 1.1.4-1
+# cfg_argparser 1.1.5
 
 a config wrapper I made to be easily applied to argparse objects.
 
 ## Installation
 
 ```bash
 # from pypi:
```

### Comparing `cfg-argparser-1.1.4.post1/pyproject.toml` & `cfg-argparser-1.1.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cfg-argparser"
-version = "1.1.4-1"
+version = "1.1.5"
 authors = [{ name = "Zeptofine", email = "zeptofine@gmail.com" }]
 description = "A package designed to simplify configurable defaults from argparse."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
```

### Comparing `cfg-argparser-1.1.4.post1/src/cfg_argparser.egg-info/PKG-INFO` & `cfg-argparser-1.1.5/src/cfg_argparser.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfg-argparser
-Version: 1.1.4.post1
+Version: 1.1.5
 Summary: A package designed to simplify configurable defaults from argparse.
 Author-email: Zeptofine <zeptofine@gmail.com>
 Project-URL: Homepage, https://github.com/zeptofine/cfg-argparser
 Project-URL: Bug Tracker, https://github.com/zeptofine/cfg-argparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# cfg_argparser 1.1.4-1
+# cfg_argparser 1.1.5
 
 a config wrapper I made to be easily applied to argparse objects.
 
 ## Installation
 
 ```bash
 # from pypi:
```

