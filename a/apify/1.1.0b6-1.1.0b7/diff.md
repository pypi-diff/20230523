# Comparing `tmp/apify-1.1.0b6.tar.gz` & `tmp/apify-1.1.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify-1.1.0b6.tar", last modified: Tue May 23 06:51:16 2023, max compression
+gzip compressed data, was "apify-1.1.0b7.tar", last modified: Tue May 23 14:12:14 2023, max compression
```

## Comparing `apify-1.1.0b6.tar` & `apify-1.1.0b7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:16.455531 apify-1.1.0b6/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-23 06:50:59.000000 apify-1.1.0b6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-23 06:51:16.451531 apify-1.1.0b6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-23 06:50:59.000000 apify-1.1.0b6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 06:51:16.455531 apify-1.1.0b6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-23 06:50:59.000000 apify-1.1.0b6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:16.443531 apify-1.1.0b6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:16.447531 apify-1.1.0b6/src/apify/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:16.451531 apify-1.1.0b6/src/apify/_memory_storage/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/file_storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/memory_storage_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:16.451531 apify-1.1.0b6/src/apify/_memory_storage/resource_clients/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/resource_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/resource_clients/base_resource_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19664 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/resource_clients/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/resource_clients/dataset_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19736 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/resource_clients/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19050 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/resource_clients/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/resource_clients/request_queue_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 06:51:15.000000 apify-1.1.0b6/src/apify/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    58019 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/proxy_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:16.451531 apify-1.1.0b6/src/apify/storages/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/storages/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    23398 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/storages/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/storages/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    25879 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/storages/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/storages/storage_client_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:16.451531 apify-1.1.0b6/src/apify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-23 06:51:16.000000 apify-1.1.0b6/src/apify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-23 06:51:16.000000 apify-1.1.0b6/src/apify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:51:16.000000 apify-1.1.0b6/src/apify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-23 06:51:16.000000 apify-1.1.0b6/src/apify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 06:51:16.000000 apify-1.1.0b6/src/apify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:12:14.602346 apify-1.1.0b7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-23 14:12:00.000000 apify-1.1.0b7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-23 14:12:14.602346 apify-1.1.0b7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-23 14:12:00.000000 apify-1.1.0b7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:12:14.602346 apify-1.1.0b7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-23 14:12:00.000000 apify-1.1.0b7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:12:14.590346 apify-1.1.0b7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:12:14.598346 apify-1.1.0b7/src/apify/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:12:14.602346 apify-1.1.0b7/src/apify/_memory_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/file_storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/memory_storage_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:12:14.602346 apify-1.1.0b7/src/apify/_memory_storage/resource_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/resource_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/resource_clients/base_resource_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19664 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/resource_clients/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/resource_clients/dataset_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19736 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/resource_clients/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19050 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/resource_clients/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/resource_clients/request_queue_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 14:12:14.000000 apify-1.1.0b7/src/apify/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58928 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/proxy_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:12:14.602346 apify-1.1.0b7/src/apify/storages/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/storages/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23398 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/storages/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/storages/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25879 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/storages/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/storages/storage_client_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:12:14.598346 apify-1.1.0b7/src/apify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-23 14:12:14.000000 apify-1.1.0b7/src/apify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-23 14:12:14.000000 apify-1.1.0b7/src/apify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:12:14.000000 apify-1.1.0b7/src/apify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-23 14:12:14.000000 apify-1.1.0b7/src/apify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 14:12:14.000000 apify-1.1.0b7/src/apify.egg-info/top_level.txt
```

### Comparing `apify-1.1.0b6/LICENSE` & `apify-1.1.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/PKG-INFO` & `apify-1.1.0b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.1.0b6
+Version: 1.1.0b7
 Summary: Apify SDK for Python
 Home-page: https://github.com/apify/apify-sdk-python
 Author: Apify Technologies s.r.o.
 Author-email: support@apify.com
 License: Apache Software License
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
```

### Comparing `apify-1.1.0b6/README.md` & `apify-1.1.0b7/README.md`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/setup.py` & `apify-1.1.0b7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     package_data={'apify': ['py.typed']},
     python_requires='>=3.8',
     install_requires=[
         'aiofiles ~= 22.1.0',
         'aioshutil ~= 1.2',
-        'apify-client ~= 1.0.0',
+        'apify-client ~= 1.1',
         'colorama ~= 0.4.6',
         'cryptography ~= 39.0.1',
         'httpx ~= 0.23.0',
         'psutil ~= 5.9.4',
         'pyee ~= 9.0.4',
         'sortedcollections ~= 2.1.0',
         'typing-extensions ~= 4.4.0',
```

### Comparing `apify-1.1.0b6/src/apify/_crypto.py` & `apify-1.1.0b7/src/apify/_crypto.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/_memory_storage/file_storage_utils.py` & `apify-1.1.0b7/src/apify/_memory_storage/file_storage_utils.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/_memory_storage/memory_storage_client.py` & `apify-1.1.0b7/src/apify/_memory_storage/memory_storage_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/_memory_storage/resource_clients/__init__.py` & `apify-1.1.0b7/src/apify/_memory_storage/resource_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/_memory_storage/resource_clients/base_resource_client.py` & `apify-1.1.0b7/src/apify/_memory_storage/resource_clients/base_resource_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py` & `apify-1.1.0b7/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/_memory_storage/resource_clients/dataset.py` & `apify-1.1.0b7/src/apify/_memory_storage/resource_clients/dataset.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/_memory_storage/resource_clients/dataset_collection.py` & `apify-1.1.0b7/src/apify/_memory_storage/resource_clients/dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/_memory_storage/resource_clients/key_value_store.py` & `apify-1.1.0b7/src/apify/_memory_storage/resource_clients/key_value_store.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/_memory_storage/resource_clients/key_value_store_collection.py` & `apify-1.1.0b7/src/apify/_memory_storage/resource_clients/key_value_store_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/_memory_storage/resource_clients/request_queue.py` & `apify-1.1.0b7/src/apify/_memory_storage/resource_clients/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/_memory_storage/resource_clients/request_queue_collection.py` & `apify-1.1.0b7/src/apify/_memory_storage/resource_clients/request_queue_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/_utils.py` & `apify-1.1.0b7/src/apify/_utils.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/actor.py` & `apify-1.1.0b7/src/apify/actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,37 +297,41 @@
 
     @classmethod
     async def exit(
         cls,
         *,
         exit_code: int = 0,
         event_listeners_timeout_secs: Optional[float] = EVENT_LISTENERS_TIMEOUT_SECS,
+        status_message: Optional[str] = None,
     ) -> None:
         """Exit the actor instance.
 
         This stops the Actor instance.
         It cancels all the intervals for regularly sending `PERSIST_STATE` events,
         sends a final `PERSIST_STATE` event,
         waits for all the event listeners to finish,
         and stops the event manager.
 
         Args:
             exit_code (int, optional): The exit code with which the actor should fail (defaults to `0`).
-            event_listeners_timeout_secs (float, optional): How long should the actor wait for actor event listeners to finish before exiting
+            event_listeners_timeout_secs (float, optional): How long should the actor wait for actor event listeners to finish before exiting.
+            status_message (str, optional): The final status message that the actor should display.
         """
         return await cls._get_default_instance().exit(
             exit_code=exit_code,
             event_listeners_timeout_secs=event_listeners_timeout_secs,
+            status_message=status_message,
         )
 
     async def _exit_internal(
         self,
         *,
         exit_code: int = 0,
         event_listeners_timeout_secs: Optional[float] = EVENT_LISTENERS_TIMEOUT_SECS,
+        status_message: Optional[str] = None,
     ) -> None:
         self._raise_if_not_initialized()
 
         self._is_exiting = True
 
         exit_code = _maybe_extract_enum_member_value(exit_code)
 
@@ -336,14 +340,17 @@
         await self._cancel_event_emitting_intervals()
 
         # Send final persist state event
         if not self._was_final_persist_state_emitted:
             self._event_manager.emit(ActorEventTypes.PERSIST_STATE, {'isMigrating': False})
             self._was_final_persist_state_emitted = True
 
+        if status_message is not None:
+            await self.set_status_message(status_message, is_terminal=True)
+
         # Sleep for a bit so that the listeners have a chance to trigger
         await asyncio.sleep(0.1)
 
         await self._event_manager.close(event_listeners_timeout_secs=event_listeners_timeout_secs)
 
         self._is_initialized = False
 
@@ -358,43 +365,47 @@
 
     @classmethod
     async def fail(
         cls,
         *,
         exit_code: int = 1,
         exception: Optional[BaseException] = None,
+        status_message: Optional[str] = None,
     ) -> None:
         """Fail the actor instance.
 
         This performs all the same steps as Actor.exit(),
         but it additionally sets the exit code to `1` (by default).
 
         Args:
             exit_code (int, optional): The exit code with which the actor should fail (defaults to `1`).
             exception (BaseException, optional): The exception with which the actor failed.
+            status_message (str, optional): The final status message that the actor should display.
         """
         return await cls._get_default_instance().fail(
             exit_code=exit_code,
             exception=exception,
+            status_message=status_message,
         )
 
     async def _fail_internal(
         self,
         *,
         exit_code: int = 1,
         exception: Optional[BaseException] = None,
+        status_message: Optional[str] = None,
     ) -> None:
         self._raise_if_not_initialized()
 
         # In IPython, we don't run `sys.exit()` during actor exits,
         # so the exception traceback will be printed on its own
         if exception and not _is_running_in_ipython():
             self.log.exception('Actor failed with an exception', exc_info=exception)
 
-        await self.exit(exit_code=exit_code)
+        await self.exit(exit_code=exit_code, status_message=status_message)
 
     @classmethod
     async def main(cls, main_actor_function: Callable[[], MainReturnType]) -> Optional[MainReturnType]:
         """Initialize the actor, run the passed function and finish the actor cleanly.
 
         **The `Actor.main()` function is optional** and is provided merely for your convenience.
         It is mainly useful when you're running your code as an actor on the [Apify platform](https://apify.com/actors).
@@ -1206,36 +1217,38 @@
             payload_template=payload_template,
             ignore_ssl_errors=ignore_ssl_errors,
             do_not_retry=do_not_retry,
             idempotency_key=idempotency_key,
         )
 
     @classmethod
-    async def set_status_message(cls, status_message: str) -> Optional[Dict]:
+    async def set_status_message(cls, status_message: str, *, is_terminal: Optional[bool] = None) -> Optional[Dict]:
         """Set the status message for the current actor run.
 
         Args:
             status_message (str): The status message to set to the run.
+            is_terminal (bool, optional): Set this flag to True if this is the final status message of the Actor run.
 
         Returns:
             dict: The updated actor run object
         """
-        return await cls._get_default_instance().set_status_message(status_message=status_message)
+        return await cls._get_default_instance().set_status_message(status_message=status_message, is_terminal=is_terminal)
 
-    async def _set_status_message_internal(self, status_message: str) -> Optional[Dict]:
+    async def _set_status_message_internal(self, status_message: str, *, is_terminal: Optional[bool] = None) -> Optional[Dict]:
         self._raise_if_not_initialized()
 
         if not self.is_at_home():
-            self.log.error('Actor.set_status_message() is only supported when running on the Apify platform.')
+            title = 'Terminal status message' if is_terminal else 'Status message'
+            self.log.info(f'[{title}]: {status_message}')
             return None
 
         # If is_at_home() is True, config.actor_run_id is always set
         assert self._config.actor_run_id is not None
 
-        return await self._apify_client.run(self._config.actor_run_id).update(status_message=status_message)
+        return await self._apify_client.run(self._config.actor_run_id).update(status_message=status_message, is_status_message_terminal=is_terminal)
 
     @classmethod
     async def create_proxy_configuration(
         cls,
         *,
         actor_proxy_input: Optional[Dict] = None,  # this is the raw proxy input from the actor run input, it is not spread or snake_cased in here
         password: Optional[str] = None,
```

### Comparing `apify-1.1.0b6/src/apify/config.py` & `apify-1.1.0b7/src/apify/config.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/consts.py` & `apify-1.1.0b7/src/apify/consts.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/event_manager.py` & `apify-1.1.0b7/src/apify/event_manager.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/log.py` & `apify-1.1.0b7/src/apify/log.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/proxy_configuration.py` & `apify-1.1.0b7/src/apify/proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/storages/base_storage.py` & `apify-1.1.0b7/src/apify/storages/base_storage.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/storages/dataset.py` & `apify-1.1.0b7/src/apify/storages/dataset.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/storages/key_value_store.py` & `apify-1.1.0b7/src/apify/storages/key_value_store.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/storages/request_queue.py` & `apify-1.1.0b7/src/apify/storages/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify/storages/storage_client_manager.py` & `apify-1.1.0b7/src/apify/storages/storage_client_manager.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify.egg-info/PKG-INFO` & `apify-1.1.0b7/src/apify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.1.0b6
+Version: 1.1.0b7
 Summary: Apify SDK for Python
 Home-page: https://github.com/apify/apify-sdk-python
 Author: Apify Technologies s.r.o.
 Author-email: support@apify.com
 License: Apache Software License
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
```

### Comparing `apify-1.1.0b6/src/apify.egg-info/SOURCES.txt` & `apify-1.1.0b7/src/apify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b6/src/apify.egg-info/requires.txt` & `apify-1.1.0b7/src/apify.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 aiofiles~=22.1.0
 aioshutil~=1.2
-apify-client~=1.0.0
+apify-client~=1.1
 colorama~=0.4.6
 cryptography~=39.0.1
 httpx~=0.23.0
 psutil~=5.9.4
 pyee~=9.0.4
 sortedcollections~=2.1.0
 typing-extensions~=4.4.0
```

