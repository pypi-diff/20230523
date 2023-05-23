# Comparing `tmp/rhods_model_registry_poc-0.1.7.tar.gz` & `tmp/rhods_model_registry_poc-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhods_model_registry_poc-0.1.7.tar", max compression
+gzip compressed data, was "rhods_model_registry_poc-0.1.8.tar", max compression
```

## Comparing `rhods_model_registry_poc-0.1.7.tar` & `rhods_model_registry_poc-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      114 2023-05-17 16:42:56.567694 rhods_model_registry_poc-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-05-17 12:00:46.265494 rhods_model_registry_poc-0.1.7/model_registry_python_sdk/__init__.py
--rw-r--r--   0        0        0     2076 2023-05-19 14:26:16.238842 rhods_model_registry_poc-0.1.7/model_registry_python_sdk/client.py
--rw-r--r--   0        0        0      568 2023-05-19 14:26:59.515695 rhods_model_registry_poc-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 rhods_model_registry_poc-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      114 2023-05-17 16:42:56.567694 rhods_model_registry_poc-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 12:00:46.265494 rhods_model_registry_poc-0.1.8/model_registry_python_sdk/__init__.py
+-rw-r--r--   0        0        0     2152 2023-05-22 17:41:05.420550 rhods_model_registry_poc-0.1.8/model_registry_python_sdk/client.py
+-rw-r--r--   0        0        0      568 2023-05-22 17:45:03.130827 rhods_model_registry_poc-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 rhods_model_registry_poc-0.1.8/PKG-INFO
```

### Comparing `rhods_model_registry_poc-0.1.7/model_registry_python_sdk/client.py` & `rhods_model_registry_poc-0.1.8/model_registry_python_sdk/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         access_key=access_key,
         secret_key=secret_key,
         secure=False,
     )
   
   async def register_model(self, name, file_name) -> bool:
     result=self.s3_client.fput_object(BUCKET, name, file_name)
+    result=self.s3_client.fput_object(BUCKET, result.version_id, file_name)
     # print("created {0} object; etag: {1}, version-id: {2}".format(result.object_name, result.etag, result.version_id))
     
     payload = ArtifactContent()
     payload.content = json.dumps({
         "bucket": result.bucket_name,
         "object_name": result.object_name,
         "version": result.version_id,
```

### Comparing `rhods_model_registry_poc-0.1.7/pyproject.toml` & `rhods_model_registry_poc-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rhods-model-registry-poc"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["Andrea Peruffo <andrea.peruffo1982@gmail.com>"]
 readme = "README.md"
 packages = [{include = "model_registry_python_sdk"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `rhods_model_registry_poc-0.1.7/PKG-INFO` & `rhods_model_registry_poc-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhods-model-registry-poc
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: Andrea Peruffo
 Author-email: andrea.peruffo1982@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

