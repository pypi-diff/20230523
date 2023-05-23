# Comparing `tmp/stigg_api_client-0.442.0.tar.gz` & `tmp/stigg_api_client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client-0.442.0.tar", max compression
+gzip compressed data, was "stigg_api_client-0.5.0.tar", max compression
```

## Comparing `stigg_api_client-0.442.0.tar` & `stigg_api_client-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0     2479 2023-05-22 17:29:07.741472 stigg_api_client-0.442.0/README.md
--rw-r--r--   0        0        0      398 2023-05-22 17:29:42.897951 stigg_api_client-0.442.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-22 17:29:07.741472 stigg_api_client-0.442.0/stigg/__init__.py
--rw-r--r--   0        0        0     1141 2023-05-22 17:29:07.741472 stigg_api_client-0.442.0/stigg/client.py
--rw-r--r--   0        0        0     3161 1970-01-01 00:00:00.000000 stigg_api_client-0.442.0/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-03-05 12:25:06.526402 stigg_api_client-0.5.0/README.md
+-rw-r--r--   0        0        0      396 2023-04-24 14:47:14.271119 stigg_api_client-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-04-23 10:33:15.442973 stigg_api_client-0.5.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1141 2023-04-24 07:23:15.920589 stigg_api_client-0.5.0/stigg/client.py
+-rw-r--r--   0        0        0        0 2023-03-05 12:25:06.527730 stigg_api_client-0.5.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0    44689 2023-04-24 14:46:41.477637 stigg_api_client-0.5.0/stigg/generated/operations.py
+-rw-r--r--   0        0        0   443944 2023-04-24 14:46:41.312733 stigg_api_client-0.5.0/stigg/generated/schema.py
+-rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 stigg_api_client-0.5.0/PKG-INFO
```

### Comparing `stigg_api_client-0.442.0/README.md` & `stigg_api_client-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.442.0/stigg/client.py` & `stigg_api_client-0.5.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.442.0/PKG-INFO` & `stigg_api_client-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client
-Version: 0.442.0
+Version: 0.5.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

