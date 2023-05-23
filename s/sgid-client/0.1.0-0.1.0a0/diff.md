# Comparing `tmp/sgid_client-0.1.0.tar.gz` & `tmp/sgid_client-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgid_client-0.1.0.tar", max compression
+gzip compressed data, was "sgid_client-0.1.0a0.tar", max compression
```

## Comparing `sgid_client-0.1.0.tar` & `sgid_client-0.1.0a0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1081 2023-05-23 07:14:42.153098 sgid_client-0.1.0/LICENSE
--rw-r--r--   0        0        0     4926 2023-05-23 07:14:42.153098 sgid_client-0.1.0/README.md
--rw-r--r--   0        0        0      657 2023-05-23 07:14:42.153098 sgid_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1127 2023-05-23 07:14:42.153098 sgid_client-0.1.0/sgid_client/IdTokenVerifier.py
--rw-r--r--   0        0        0     8502 2023-05-23 07:14:42.153098 sgid_client-0.1.0/sgid_client/SgidClient.py
--rw-r--r--   0        0        0      179 2023-05-23 07:14:42.153098 sgid_client-0.1.0/sgid_client/__init__.py
--rw-r--r--   0        0        0     1184 2023-05-23 07:14:42.153098 sgid_client-0.1.0/sgid_client/decrypt_data.py
--rw-r--r--   0        0        0     4332 2023-05-23 07:14:42.153098 sgid_client-0.1.0/sgid_client/error.py
--rw-r--r--   0        0        0     2094 2023-05-23 07:14:42.153098 sgid_client-0.1.0/sgid_client/generators.py
--rw-r--r--   0        0        0      577 2023-05-23 07:14:42.153098 sgid_client-0.1.0/sgid_client/util.py
--rw-r--r--   0        0        0     4482 2023-05-23 07:14:42.153098 sgid_client-0.1.0/sgid_client/validation.py
--rw-r--r--   0        0        0     5547 1970-01-01 00:00:00.000000 sgid_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-23 06:27:13.508435 sgid_client-0.1.0a0/LICENSE
+-rw-r--r--   0        0        0     4926 2023-05-23 06:27:13.508435 sgid_client-0.1.0a0/README.md
+-rw-r--r--   0        0        0      665 2023-05-23 06:27:13.508435 sgid_client-0.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0     1127 2023-05-23 06:27:13.508435 sgid_client-0.1.0a0/sgid_client/IdTokenVerifier.py
+-rw-r--r--   0        0        0     8502 2023-05-23 06:27:13.508435 sgid_client-0.1.0a0/sgid_client/SgidClient.py
+-rw-r--r--   0        0        0      179 2023-05-23 06:27:13.508435 sgid_client-0.1.0a0/sgid_client/__init__.py
+-rw-r--r--   0        0        0     1184 2023-05-23 06:27:13.508435 sgid_client-0.1.0a0/sgid_client/decrypt_data.py
+-rw-r--r--   0        0        0     4332 2023-05-23 06:27:13.508435 sgid_client-0.1.0a0/sgid_client/error.py
+-rw-r--r--   0        0        0     2094 2023-05-23 06:27:13.508435 sgid_client-0.1.0a0/sgid_client/generators.py
+-rw-r--r--   0        0        0      577 2023-05-23 06:27:13.508435 sgid_client-0.1.0a0/sgid_client/util.py
+-rw-r--r--   0        0        0     4482 2023-05-23 06:27:13.508435 sgid_client-0.1.0a0/sgid_client/validation.py
+-rw-r--r--   0        0        0     5549 1970-01-01 00:00:00.000000 sgid_client-0.1.0a0/PKG-INFO
```

### Comparing `sgid_client-0.1.0/LICENSE` & `sgid_client-0.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `sgid_client-0.1.0/README.md` & `sgid_client-0.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `sgid_client-0.1.0/pyproject.toml` & `sgid_client-0.1.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sgid-client"
-version = "0.1.0"
+version = "0.1.0-alpha.0"
 description = "The official Python SDK for sgID"
 authors = ["Open Government Products"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "sgid_client"}]
 repository = "https://github.com/opengovsg/sgid-client-python"
```

### Comparing `sgid_client-0.1.0/sgid_client/IdTokenVerifier.py` & `sgid_client-0.1.0a0/sgid_client/IdTokenVerifier.py`

 * *Files identical despite different names*

### Comparing `sgid_client-0.1.0/sgid_client/SgidClient.py` & `sgid_client-0.1.0a0/sgid_client/SgidClient.py`

 * *Files identical despite different names*

### Comparing `sgid_client-0.1.0/sgid_client/decrypt_data.py` & `sgid_client-0.1.0a0/sgid_client/decrypt_data.py`

 * *Files identical despite different names*

### Comparing `sgid_client-0.1.0/sgid_client/error.py` & `sgid_client-0.1.0a0/sgid_client/error.py`

 * *Files identical despite different names*

### Comparing `sgid_client-0.1.0/sgid_client/generators.py` & `sgid_client-0.1.0a0/sgid_client/generators.py`

 * *Files identical despite different names*

### Comparing `sgid_client-0.1.0/sgid_client/util.py` & `sgid_client-0.1.0a0/sgid_client/util.py`

 * *Files identical despite different names*

### Comparing `sgid_client-0.1.0/sgid_client/validation.py` & `sgid_client-0.1.0a0/sgid_client/validation.py`

 * *Files identical despite different names*

### Comparing `sgid_client-0.1.0/PKG-INFO` & `sgid_client-0.1.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgid-client
-Version: 0.1.0
+Version: 0.1.0a0
 Summary: The official Python SDK for sgID
 Home-page: https://github.com/opengovsg/sgid-client-python
 License: MIT
 Author: Open Government Products
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

