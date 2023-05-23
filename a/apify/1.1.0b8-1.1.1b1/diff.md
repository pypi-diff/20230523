# Comparing `tmp/apify-1.1.0b8.tar.gz` & `tmp/apify-1.1.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify-1.1.0b8.tar", last modified: Tue May 23 15:25:34 2023, max compression
+gzip compressed data, was "apify-1.1.1b1.tar", last modified: Tue May 23 17:08:47 2023, max compression
```

## Comparing `apify-1.1.0b8.tar` & `apify-1.1.1b1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:25:34.456034 apify-1.1.0b8/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-23 15:24:54.000000 apify-1.1.0b8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-23 15:25:34.456034 apify-1.1.0b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-23 15:24:54.000000 apify-1.1.0b8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-23 15:25:30.000000 apify-1.1.0b8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 15:25:34.456034 apify-1.1.0b8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:25:34.452034 apify-1.1.0b8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:25:34.456034 apify-1.1.0b8/src/apify/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:25:34.456034 apify-1.1.0b8/src/apify/_memory_storage/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/file_storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/memory_storage_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:25:34.456034 apify-1.1.0b8/src/apify/_memory_storage/resource_clients/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/resource_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/resource_clients/base_resource_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19664 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/resource_clients/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/resource_clients/dataset_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19736 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/resource_clients/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19050 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/resource_clients/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/resource_clients/request_queue_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    58928 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/proxy_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:25:34.456034 apify-1.1.0b8/src/apify/storages/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/storages/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    23398 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/storages/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/storages/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    25879 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/storages/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/storages/storage_client_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:25:34.456034 apify-1.1.0b8/src/apify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-23 15:25:34.000000 apify-1.1.0b8/src/apify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-23 15:25:34.000000 apify-1.1.0b8/src/apify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:25:34.000000 apify-1.1.0b8/src/apify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-23 15:25:34.000000 apify-1.1.0b8/src/apify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 15:25:34.000000 apify-1.1.0b8/src/apify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:47.826235 apify-1.1.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-23 17:07:59.000000 apify-1.1.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-23 17:08:47.826235 apify-1.1.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-23 17:07:59.000000 apify-1.1.1b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-23 17:08:42.000000 apify-1.1.1b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 17:08:47.826235 apify-1.1.1b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:47.818235 apify-1.1.1b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:47.822235 apify-1.1.1b1/src/apify/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:47.822235 apify-1.1.1b1/src/apify/_memory_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/file_storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/memory_storage_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:47.826235 apify-1.1.1b1/src/apify/_memory_storage/resource_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/resource_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/resource_clients/base_resource_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19664 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/resource_clients/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/resource_clients/dataset_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19736 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/resource_clients/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19050 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/resource_clients/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/resource_clients/request_queue_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58928 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/proxy_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:47.826235 apify-1.1.1b1/src/apify/storages/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/storages/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23398 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/storages/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/storages/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25879 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/storages/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/storages/storage_client_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:47.822235 apify-1.1.1b1/src/apify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-23 17:08:47.000000 apify-1.1.1b1/src/apify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-23 17:08:47.000000 apify-1.1.1b1/src/apify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:08:47.000000 apify-1.1.1b1/src/apify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-23 17:08:47.000000 apify-1.1.1b1/src/apify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 17:08:47.000000 apify-1.1.1b1/src/apify.egg-info/top_level.txt
```

### Comparing `apify-1.1.0b8/LICENSE` & `apify-1.1.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/PKG-INFO` & `apify-1.1.1b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.1.0b8
+Version: 1.1.1b1
 Summary: Apify SDK for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/sdk/python/
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
 Project-URL: Issue tracker, https://github.com/apify/apify-sdk-python/issues
```

### Comparing `apify-1.1.0b8/README.md` & `apify-1.1.1b1/README.md`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/pyproject.toml` & `apify-1.1.1b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 
 name = "apify"
 
-version = "1.1.0b8"
+version = "1.1.1b1"
 description = "Apify SDK for Python"
 
 readme = "README.md"
 
 license = {text = "Apache Software License"}
 
 authors = [
@@ -43,35 +43,35 @@
 
 
 
 requires-python = ">=3.8"
 
 dependencies = [
 
-    "aiofiles ~= 23.1.0",
+    "aiofiles >= 22.1.0",
 
-    "aioshutil ~= 1.3",
+    "aioshutil >= 1.0",
 
-    "apify-client ~= 1.2.0",
+    "apify-client >= 1.2.0",
 
-    "colorama ~= 0.4.6",
+    "colorama >= 0.4.6",
 
-    "cryptography ~= 40.0.2",
+    "cryptography >= 39.0.0",
 
-    "httpx ~= 0.24.1",
+    "httpx >= 0.24.1",
 
-    "psutil ~= 5.9.5",
+    "psutil >= 5.9.5",
 
-    "pyee ~= 9.1.0",
+    "pyee >= 9.0.0",
 
-    "sortedcollections ~= 2.1.0",
+    "sortedcollections >= 2.0.1",
 
-    "typing-extensions ~= 4.6.0",
+    "typing-extensions >= 4.1.0",
 
-    "websockets ~= 11.0.3",
+    "websockets >= 10.1",
 
 ]
 
 
 
 [project.optional-dependencies]
```

### Comparing `apify-1.1.0b8/src/apify/_crypto.py` & `apify-1.1.1b1/src/apify/_crypto.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/_memory_storage/file_storage_utils.py` & `apify-1.1.1b1/src/apify/_memory_storage/file_storage_utils.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/_memory_storage/memory_storage_client.py` & `apify-1.1.1b1/src/apify/_memory_storage/memory_storage_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/_memory_storage/resource_clients/__init__.py` & `apify-1.1.1b1/src/apify/_memory_storage/resource_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/_memory_storage/resource_clients/base_resource_client.py` & `apify-1.1.1b1/src/apify/_memory_storage/resource_clients/base_resource_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py` & `apify-1.1.1b1/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/_memory_storage/resource_clients/dataset.py` & `apify-1.1.1b1/src/apify/_memory_storage/resource_clients/dataset.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/_memory_storage/resource_clients/dataset_collection.py` & `apify-1.1.1b1/src/apify/_memory_storage/resource_clients/dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/_memory_storage/resource_clients/key_value_store.py` & `apify-1.1.1b1/src/apify/_memory_storage/resource_clients/key_value_store.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/_memory_storage/resource_clients/key_value_store_collection.py` & `apify-1.1.1b1/src/apify/_memory_storage/resource_clients/key_value_store_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/_memory_storage/resource_clients/request_queue.py` & `apify-1.1.1b1/src/apify/_memory_storage/resource_clients/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/_memory_storage/resource_clients/request_queue_collection.py` & `apify-1.1.1b1/src/apify/_memory_storage/resource_clients/request_queue_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/_utils.py` & `apify-1.1.1b1/src/apify/_utils.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/actor.py` & `apify-1.1.1b1/src/apify/actor.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/config.py` & `apify-1.1.1b1/src/apify/config.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/consts.py` & `apify-1.1.1b1/src/apify/consts.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/event_manager.py` & `apify-1.1.1b1/src/apify/event_manager.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/log.py` & `apify-1.1.1b1/src/apify/log.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/proxy_configuration.py` & `apify-1.1.1b1/src/apify/proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/storages/base_storage.py` & `apify-1.1.1b1/src/apify/storages/base_storage.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/storages/dataset.py` & `apify-1.1.1b1/src/apify/storages/dataset.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/storages/key_value_store.py` & `apify-1.1.1b1/src/apify/storages/key_value_store.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/storages/request_queue.py` & `apify-1.1.1b1/src/apify/storages/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify/storages/storage_client_manager.py` & `apify-1.1.1b1/src/apify/storages/storage_client_manager.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify.egg-info/PKG-INFO` & `apify-1.1.1b1/src/apify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.1.0b8
+Version: 1.1.1b1
 Summary: Apify SDK for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/sdk/python/
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
 Project-URL: Issue tracker, https://github.com/apify/apify-sdk-python/issues
```

### Comparing `apify-1.1.0b8/src/apify.egg-info/SOURCES.txt` & `apify-1.1.1b1/src/apify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b8/src/apify.egg-info/requires.txt` & `apify-1.1.1b1/src/apify.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-aiofiles~=23.1.0
-aioshutil~=1.3
-apify-client~=1.2.0
-colorama~=0.4.6
-cryptography~=40.0.2
-httpx~=0.24.1
-psutil~=5.9.5
-pyee~=9.1.0
-sortedcollections~=2.1.0
-typing-extensions~=4.6.0
-websockets~=11.0.3
+aiofiles>=22.1.0
+aioshutil>=1.0
+apify-client>=1.2.0
+colorama>=0.4.6
+cryptography>=39.0.0
+httpx>=0.24.1
+psutil>=5.9.5
+pyee>=9.0.0
+sortedcollections>=2.0.1
+typing-extensions>=4.1.0
+websockets>=10.1
 
 [dev]
 autopep8~=2.0.2
 build~=0.10.0
 filelock~=3.12.0
 flake8~=6.0.0
 flake8-bugbear~=23.5.9
```

