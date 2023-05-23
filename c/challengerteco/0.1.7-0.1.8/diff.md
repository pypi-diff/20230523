# Comparing `tmp/challengerteco-0.1.7.tar.gz` & `tmp/challengerteco-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "challengerteco-0.1.7.tar", max compression
+gzip compressed data, was "challengerteco-0.1.8.tar", max compression
```

## Comparing `challengerteco-0.1.7.tar` & `challengerteco-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-04-18 13:26:24.967751 challengerteco-0.1.7/README.md
--rw-r--r--   0        0        0    83013 2023-05-23 15:03:49.708078 challengerteco-0.1.7/challengerteco/Challenger.py
--rw-r--r--   0        0        0       86 2023-04-20 16:51:54.029080 challengerteco-0.1.7/challengerteco/__init__.py
--rw-r--r--   0        0        0      339 2023-05-23 15:04:29.091329 challengerteco-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 challengerteco-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-18 13:26:24.967751 challengerteco-0.1.8/README.md
+-rw-r--r--   0        0        0    83013 2023-05-23 15:03:49.708078 challengerteco-0.1.8/challengerteco/Challenger.py
+-rw-r--r--   0        0        0       86 2023-04-20 16:51:54.029080 challengerteco-0.1.8/challengerteco/__init__.py
+-rw-r--r--   0        0        0      357 2023-05-23 15:05:14.517929 challengerteco-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 challengerteco-0.1.8/PKG-INFO
```

### Comparing `challengerteco-0.1.7/challengerteco/Challenger.py` & `challengerteco-0.1.8/challengerteco/Challenger.py`

 * *Files identical despite different names*

### Comparing `challengerteco-0.1.7/PKG-INFO` & `challengerteco-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: challengerteco
-Version: 0.1.7
-Summary: Fix en manejo de deciles
+Version: 0.1.8
+Summary: Clase para manejo de challenger en la nube
 Author: Eduardo Pagnone
 Author-email: mlopsaa@teco.com.ar
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

