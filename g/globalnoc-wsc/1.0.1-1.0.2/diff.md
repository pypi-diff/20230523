# Comparing `tmp/globalnoc_wsc-1.0.1.tar.gz` & `tmp/globalnoc_wsc-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globalnoc_wsc-1.0.1.tar", max compression
+gzip compressed data, was "globalnoc_wsc-1.0.2.tar", max compression
```

## Comparing `globalnoc_wsc-1.0.1.tar` & `globalnoc_wsc-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-04-01 18:18:42.189664 globalnoc_wsc-1.0.1/LICENSE
--rw-r--r--   0        0        0     3885 2023-04-01 16:27:29.824525 globalnoc_wsc-1.0.1/README.md
--rw-r--r--   0        0        0      612 2023-04-01 19:25:17.378510 globalnoc_wsc-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    13200 2023-04-01 19:25:17.383510 globalnoc_wsc-1.0.1/src/globalnoc/wsc/__init__.py
--rw-r--r--   0        0        0     3263 2023-04-01 19:25:17.388511 globalnoc_wsc-1.0.1/src/globalnoc/wsc/__main__.py
--rw-r--r--   0        0        0     4514 1970-01-01 00:00:00.000000 globalnoc_wsc-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-02 14:38:20.317346 globalnoc_wsc-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3885 2023-04-01 16:27:29.824525 globalnoc_wsc-1.0.2/README.md
+-rw-r--r--   0        0        0      933 2023-05-23 13:34:13.304831 globalnoc_wsc-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    13200 2023-04-02 14:38:20.435350 globalnoc_wsc-1.0.2/src/globalnoc/wsc/__init__.py
+-rw-r--r--   0        0        0     3263 2023-04-02 14:38:20.451350 globalnoc_wsc-1.0.2/src/globalnoc/wsc/__main__.py
+-rw-r--r--   0        0        0     4639 1970-01-01 00:00:00.000000 globalnoc_wsc-1.0.2/PKG-INFO
```

### Comparing `globalnoc_wsc-1.0.1/LICENSE` & `globalnoc_wsc-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `globalnoc_wsc-1.0.1/README.md` & `globalnoc_wsc-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `globalnoc_wsc-1.0.1/src/globalnoc/wsc/__init__.py` & `globalnoc_wsc-1.0.2/src/globalnoc/wsc/__init__.py`

 * *Files identical despite different names*

### Comparing `globalnoc_wsc-1.0.1/src/globalnoc/wsc/__main__.py` & `globalnoc_wsc-1.0.2/src/globalnoc/wsc/__main__.py`

 * *Files identical despite different names*

### Comparing `globalnoc_wsc-1.0.1/PKG-INFO` & `globalnoc_wsc-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: globalnoc-wsc
-Version: 1.0.1
+Version: 1.0.2
 Summary: GlobalNOC Web Service Client with SAML2 and basic auth support
 License: Apache-2.0
 Author: GlobalNOC SysEng
 Author-email: syseng@globalnoc.iu.edu
 Requires-Python: >=3.8.11,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: urllib3 (<2.0.0) ; python_version < "3.10"
+Requires-Dist: urllib3 (>=2.0.2,<3.0.0) ; python_version >= "3.10"
 Description-Content-Type: text/markdown
 
 # GlobalNOC WSC
 
 WSC is a client implementation of the GlobalNOC Web Service calling convention.
 
 You can use this library to interface with GlobalNOC Web Services.
```

