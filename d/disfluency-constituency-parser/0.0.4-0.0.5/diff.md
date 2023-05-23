# Comparing `tmp/disfluency-constituency-parser-0.0.4.tar.gz` & `tmp/disfluency-constituency-parser-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disfluency-constituency-parser-0.0.4.tar", last modified: Wed May 17 03:08:20 2023, max compression
+gzip compressed data, was "disfluency-constituency-parser-0.0.5.tar", last modified: Tue May 23 18:00:07 2023, max compression
```

## Comparing `disfluency-constituency-parser-0.0.4.tar` & `disfluency-constituency-parser-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:08:20.675900 disfluency-constituency-parser-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-17 03:08:00.000000 disfluency-constituency-parser-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-17 03:08:20.675900 disfluency-constituency-parser-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-17 03:08:00.000000 disfluency-constituency-parser-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:08:20.675900 disfluency-constituency-parser-0.0.4/dc_parser/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-17 03:08:00.000000 disfluency-constituency-parser-0.0.4/dc_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-17 03:08:00.000000 disfluency-constituency-parser-0.0.4/dc_parser/chart_helper.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-17 03:08:00.000000 disfluency-constituency-parser-0.0.4/dc_parser/nkutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-17 03:08:00.000000 disfluency-constituency-parser-0.0.4/dc_parser/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    50393 2023-05-17 03:08:00.000000 disfluency-constituency-parser-0.0.4/dc_parser/parse_nk.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-05-17 03:08:00.000000 disfluency-constituency-parser-0.0.4/dc_parser/trees.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-17 03:08:00.000000 disfluency-constituency-parser-0.0.4/dc_parser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-17 03:08:00.000000 disfluency-constituency-parser-0.0.4/dc_parser/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:08:20.675900 disfluency-constituency-parser-0.0.4/disfluency_constituency_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-17 03:08:20.000000 disfluency-constituency-parser-0.0.4/disfluency_constituency_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-17 03:08:20.000000 disfluency-constituency-parser-0.0.4/disfluency_constituency_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 03:08:20.000000 disfluency-constituency-parser-0.0.4/disfluency_constituency_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-17 03:08:20.000000 disfluency-constituency-parser-0.0.4/disfluency_constituency_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 03:08:20.000000 disfluency-constituency-parser-0.0.4/disfluency_constituency_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 03:08:20.675900 disfluency-constituency-parser-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-17 03:08:00.000000 disfluency-constituency-parser-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:07.908176 disfluency-constituency-parser-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-23 17:59:49.000000 disfluency-constituency-parser-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-23 18:00:07.908176 disfluency-constituency-parser-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-23 17:59:49.000000 disfluency-constituency-parser-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:07.908176 disfluency-constituency-parser-0.0.5/dc_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-23 17:59:49.000000 disfluency-constituency-parser-0.0.5/dc_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-23 17:59:49.000000 disfluency-constituency-parser-0.0.5/dc_parser/chart_helper.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-23 17:59:49.000000 disfluency-constituency-parser-0.0.5/dc_parser/nkutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-23 17:59:49.000000 disfluency-constituency-parser-0.0.5/dc_parser/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50393 2023-05-23 17:59:49.000000 disfluency-constituency-parser-0.0.5/dc_parser/parse_nk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-05-23 17:59:49.000000 disfluency-constituency-parser-0.0.5/dc_parser/trees.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-23 17:59:49.000000 disfluency-constituency-parser-0.0.5/dc_parser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-23 17:59:49.000000 disfluency-constituency-parser-0.0.5/dc_parser/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:07.908176 disfluency-constituency-parser-0.0.5/disfluency_constituency_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-23 18:00:07.000000 disfluency-constituency-parser-0.0.5/disfluency_constituency_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-23 18:00:07.000000 disfluency-constituency-parser-0.0.5/disfluency_constituency_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:00:07.000000 disfluency-constituency-parser-0.0.5/disfluency_constituency_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 18:00:07.000000 disfluency-constituency-parser-0.0.5/disfluency_constituency_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 18:00:07.000000 disfluency-constituency-parser-0.0.5/disfluency_constituency_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 18:00:07.908176 disfluency-constituency-parser-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-23 17:59:49.000000 disfluency-constituency-parser-0.0.5/setup.py
```

### Comparing `disfluency-constituency-parser-0.0.4/LICENSE` & `disfluency-constituency-parser-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `disfluency-constituency-parser-0.0.4/PKG-INFO` & `disfluency-constituency-parser-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disfluency-constituency-parser
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/liwangd/disfluency-constituency-parser
 Author: Li Wang
 Author-email: li@liwang.info
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `disfluency-constituency-parser-0.0.4/README.md` & `disfluency-constituency-parser-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `disfluency-constituency-parser-0.0.4/dc_parser/chart_helper.pyx` & `disfluency-constituency-parser-0.0.5/dc_parser/chart_helper.pyx`

 * *Files identical despite different names*

### Comparing `disfluency-constituency-parser-0.0.4/dc_parser/nkutil.py` & `disfluency-constituency-parser-0.0.5/dc_parser/nkutil.py`

 * *Files identical despite different names*

### Comparing `disfluency-constituency-parser-0.0.4/dc_parser/parse.py` & `disfluency-constituency-parser-0.0.5/dc_parser/parse.py`

 * *Files identical despite different names*

### Comparing `disfluency-constituency-parser-0.0.4/dc_parser/parse_nk.py` & `disfluency-constituency-parser-0.0.5/dc_parser/parse_nk.py`

 * *Files identical despite different names*

### Comparing `disfluency-constituency-parser-0.0.4/dc_parser/trees.py` & `disfluency-constituency-parser-0.0.5/dc_parser/trees.py`

 * *Files identical despite different names*

### Comparing `disfluency-constituency-parser-0.0.4/dc_parser/utils.py` & `disfluency-constituency-parser-0.0.5/dc_parser/utils.py`

 * *Files identical despite different names*

### Comparing `disfluency-constituency-parser-0.0.4/dc_parser/vocabulary.py` & `disfluency-constituency-parser-0.0.5/dc_parser/vocabulary.py`

 * *Files identical despite different names*

### Comparing `disfluency-constituency-parser-0.0.4/disfluency_constituency_parser.egg-info/PKG-INFO` & `disfluency-constituency-parser-0.0.5/disfluency_constituency_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disfluency-constituency-parser
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/liwangd/disfluency-constituency-parser
 Author: Li Wang
 Author-email: li@liwang.info
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `disfluency-constituency-parser-0.0.4/setup.py` & `disfluency-constituency-parser-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="disfluency-constituency-parser",
-    version="0.0.4",
+    version="0.0.5",
     author="Li Wang",
     author_email="li@liwang.info",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liwangd/disfluency-constituency-parser",
     packages=setuptools.find_packages(),
     package_data={'': ['*.pyx']},
```

