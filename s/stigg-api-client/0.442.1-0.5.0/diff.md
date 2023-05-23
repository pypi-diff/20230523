# Comparing `tmp/stigg_api_client-0.442.1.tar.gz` & `tmp/stigg_api_client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client-0.442.1.tar", max compression
+gzip compressed data, was "stigg_api_client-0.5.0.tar", max compression
```

## Comparing `stigg_api_client-0.442.1.tar` & `stigg_api_client-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0     2479 2023-05-23 08:06:03.257883 stigg_api_client-0.442.1/README.md
--rw-r--r--   0        0        0      391 2023-05-23 08:06:43.654465 stigg_api_client-0.442.1/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-23 08:06:03.257883 stigg_api_client-0.442.1/stigg/__init__.py
--rw-r--r--   0        0        0     1141 2023-05-23 08:06:03.257883 stigg_api_client-0.442.1/stigg/client.py
--rw-r--r--   0        0        0     3152 1970-01-01 00:00:00.000000 stigg_api_client-0.442.1/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-03-05 12:25:06.526402 stigg_api_client-0.5.0/README.md
+-rw-r--r--   0        0        0      396 2023-04-24 14:47:14.271119 stigg_api_client-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-04-23 10:33:15.442973 stigg_api_client-0.5.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1141 2023-04-24 07:23:15.920589 stigg_api_client-0.5.0/stigg/client.py
+-rw-r--r--   0        0        0        0 2023-03-05 12:25:06.527730 stigg_api_client-0.5.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0    44689 2023-04-24 14:46:41.477637 stigg_api_client-0.5.0/stigg/generated/operations.py
+-rw-r--r--   0        0        0   443944 2023-04-24 14:46:41.312733 stigg_api_client-0.5.0/stigg/generated/schema.py
+-rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 stigg_api_client-0.5.0/PKG-INFO
```

### Comparing `stigg_api_client-0.442.1/README.md` & `stigg_api_client-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.442.1/stigg/client.py` & `stigg_api_client-0.5.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.442.1/PKG-INFO` & `stigg_api_client-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: stigg-api-client
-Version: 0.442.1
+Version: 0.5.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: black (>=22.8,<23.0)
-Requires-Dist: flake8 (>=5.0,<6.0)
-Requires-Dist: graphql-core (>=3.1,<4.0)
-Requires-Dist: requests (>=2.28,<3.0)
+Requires-Dist: black (>=22.8.0,<23.0.0)
+Requires-Dist: flake8 (>=5.0.4,<6.0.0)
+Requires-Dist: graphql-core (==3.1.6)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: sgqlc (>=16.0,<17.0)
 Description-Content-Type: text/markdown
 
 # stigg-api-client
 
 This library provides a Python wrapper to [Stigg's GraphQL API](https://docs.stigg.io/docs/graphql-api) based on 
 the operations that are in use by the [Stigg's Node.js SDK](https://docs.stigg.io/docs/nodejs-sdk).
```

