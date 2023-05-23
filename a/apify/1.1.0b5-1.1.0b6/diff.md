# Comparing `tmp/apify-1.1.0b5.tar.gz` & `tmp/apify-1.1.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify-1.1.0b5.tar", last modified: Mon Apr 24 07:10:17 2023, max compression
+gzip compressed data, was "apify-1.1.0b6.tar", last modified: Tue May 23 06:51:16 2023, max compression
```

## Comparing `apify-1.1.0b5.tar` & `apify-1.1.0b6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:10:17.486343 apify-1.1.0b5/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-04-24 07:10:06.000000 apify-1.1.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-24 07:10:17.486343 apify-1.1.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-24 07:10:06.000000 apify-1.1.0b5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 07:10:17.486343 apify-1.1.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-04-24 07:10:06.000000 apify-1.1.0b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:10:17.482343 apify-1.1.0b5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:10:17.482343 apify-1.1.0b5/src/apify/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:10:17.486343 apify-1.1.0b5/src/apify/_memory_storage/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/file_storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/memory_storage_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:10:17.486343 apify-1.1.0b5/src/apify/_memory_storage/resource_clients/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/resource_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/resource_clients/base_resource_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19664 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/resource_clients/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/resource_clients/dataset_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/resource_clients/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19050 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/resource_clients/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/resource_clients/request_queue_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 07:10:17.000000 apify-1.1.0b5/src/apify/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    58019 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/proxy_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:10:17.486343 apify-1.1.0b5/src/apify/storages/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/storages/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    23398 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/storages/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/storages/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    25879 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/storages/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/storages/storage_client_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:10:17.486343 apify-1.1.0b5/src/apify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-24 07:10:17.000000 apify-1.1.0b5/src/apify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-24 07:10:17.000000 apify-1.1.0b5/src/apify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 07:10:17.000000 apify-1.1.0b5/src/apify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-24 07:10:17.000000 apify-1.1.0b5/src/apify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 07:10:17.000000 apify-1.1.0b5/src/apify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:16.455531 apify-1.1.0b6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-23 06:50:59.000000 apify-1.1.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-23 06:51:16.451531 apify-1.1.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-23 06:50:59.000000 apify-1.1.0b6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 06:51:16.455531 apify-1.1.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-23 06:50:59.000000 apify-1.1.0b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:16.443531 apify-1.1.0b6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:16.447531 apify-1.1.0b6/src/apify/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:16.451531 apify-1.1.0b6/src/apify/_memory_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/file_storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/memory_storage_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:16.451531 apify-1.1.0b6/src/apify/_memory_storage/resource_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/resource_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/resource_clients/base_resource_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19664 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/resource_clients/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/resource_clients/dataset_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19736 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/resource_clients/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19050 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/resource_clients/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_memory_storage/resource_clients/request_queue_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 06:51:15.000000 apify-1.1.0b6/src/apify/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58019 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/proxy_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:16.451531 apify-1.1.0b6/src/apify/storages/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/storages/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23398 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/storages/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/storages/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25879 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/storages/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-23 06:50:59.000000 apify-1.1.0b6/src/apify/storages/storage_client_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:16.451531 apify-1.1.0b6/src/apify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-23 06:51:16.000000 apify-1.1.0b6/src/apify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-23 06:51:16.000000 apify-1.1.0b6/src/apify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:51:16.000000 apify-1.1.0b6/src/apify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-23 06:51:16.000000 apify-1.1.0b6/src/apify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 06:51:16.000000 apify-1.1.0b6/src/apify.egg-info/top_level.txt
```

### Comparing `apify-1.1.0b5/LICENSE` & `apify-1.1.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/PKG-INFO` & `apify-1.1.0b6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.1.0b5
+Version: 1.1.0b6
 Summary: Apify SDK for Python
 Home-page: https://github.com/apify/apify-sdk-python
 Author: Apify Technologies s.r.o.
 Author-email: support@apify.com
 License: Apache Software License
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
```

### Comparing `apify-1.1.0b5/README.md` & `apify-1.1.0b6/README.md`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/setup.py` & `apify-1.1.0b6/setup.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/_crypto.py` & `apify-1.1.0b6/src/apify/_crypto.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/_memory_storage/file_storage_utils.py` & `apify-1.1.0b6/src/apify/_memory_storage/file_storage_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -37,53 +37,14 @@
     # Save all the new items to the disk
     for idx, item in data:
         file_path = os.path.join(entity_directory, f'{idx}.json')
         async with aiofiles.open(file_path, mode='wb') as f:
             await f.write(_json_dumps(item).encode('utf-8'))
 
 
-async def _set_or_delete_key_value_store_record(
-    *,
-    entity_directory: str,
-    persist_storage: bool,
-    record: Dict,
-    should_set: bool,
-    write_metadata: bool,
-) -> None:
-    # Skip writing files to the disk if the client has the option set to false
-    if not persist_storage:
-        return
-
-    # Ensure the directory for the entity exists
-    await makedirs(entity_directory, exist_ok=True)
-
-    # Create files for the record
-    record_path = os.path.join(entity_directory, f"""{record['key']}.{record['extension']}""")
-    record_metadata_path = os.path.join(entity_directory, f"""{record['key']}.__metadata__.json""")
-
-    await _force_remove(record_path)
-    await _force_remove(record_metadata_path)
-
-    if should_set:
-        if write_metadata:
-            async with aiofiles.open(record_metadata_path, mode='wb') as f:
-                await f.write(_json_dumps({
-                    'key': record['key'],
-                    'contentType': record.get('content_type') or 'unknown/no content type',
-                    'extension': record['extension'],
-                }).encode('utf-8'))
-
-        # Convert to bytes if string
-        if isinstance(record['value'], str):
-            record['value'] = record['value'].encode('utf-8')
-
-        async with aiofiles.open(record_path, mode='wb') as f:
-            await f.write(record['value'])
-
-
 async def _update_request_queue_item(
     *,
     request_id: str,
     request: Dict,
     entity_directory: str,
     persist_storage: bool,
 ) -> None:
```

### Comparing `apify-1.1.0b5/src/apify/_memory_storage/memory_storage_client.py` & `apify-1.1.0b6/src/apify/_memory_storage/memory_storage_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/_memory_storage/resource_clients/__init__.py` & `apify-1.1.0b6/src/apify/_memory_storage/resource_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/_memory_storage/resource_clients/base_resource_client.py` & `apify-1.1.0b6/src/apify/_memory_storage/resource_clients/base_resource_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py` & `apify-1.1.0b6/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/_memory_storage/resource_clients/dataset.py` & `apify-1.1.0b6/src/apify/_memory_storage/resource_clients/dataset.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/_memory_storage/resource_clients/dataset_collection.py` & `apify-1.1.0b6/src/apify/_memory_storage/resource_clients/dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/_memory_storage/resource_clients/key_value_store.py` & `apify-1.1.0b6/src/apify/_memory_storage/resource_clients/key_value_store.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,69 @@
 import asyncio
 import io
 import json
 import mimetypes
 import os
 import pathlib
-import warnings
 from datetime import datetime, timezone
 from operator import itemgetter
-from typing import TYPE_CHECKING, Any, AsyncIterator, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, AsyncIterator, Dict, List, Optional, TypedDict
 
+import aiofiles
 import aioshutil
+from aiofiles.os import makedirs
+from typing_extensions import NotRequired
 
 from ..._crypto import _crypto_random_object_id
 from ..._utils import (
+    _force_remove,
     _force_rename,
     _guess_file_extension,
     _is_file_or_bytes,
     _json_dumps,
     _maybe_parse_body,
     _raise_on_duplicate_storage,
     _raise_on_non_existing_storage,
     ignore_docs,
 )
 from ...consts import DEFAULT_API_PARAM_LIMIT, _StorageTypes
 from ...log import logger
-from ..file_storage_utils import _set_or_delete_key_value_store_record, _update_metadata
+from ..file_storage_utils import _update_metadata
 from .base_resource_client import BaseResourceClient
 
 if TYPE_CHECKING:
     from ..memory_storage_client import MemoryStorageClient
 
-DEFAULT_LOCAL_FILE_EXTENSION = 'bin'
+KeyValueStoreRecord = TypedDict('KeyValueStoreRecord', {'key': str, 'value': Any, 'contentType': Optional[str], 'filename': NotRequired[str]})
+
+
+def _filename_from_record(record: KeyValueStoreRecord) -> str:
+    if record.get('filename') is not None:
+        return record['filename']
+
+    content_type = record.get('contentType')
+    if not content_type or content_type == 'application/octet-stream':
+        return record['key']
+    else:
+        extension = _guess_file_extension(content_type)
+        if record['key'].endswith(f'.{extension}'):
+            return record['key']
+        else:
+            return f'{record["key"]}.{extension}'
 
 
 @ignore_docs
 class KeyValueStoreClient(BaseResourceClient):
     """Sub-client for manipulating a single key-value store."""
 
     _id: str
     _resource_directory: str
     _memory_storage_client: 'MemoryStorageClient'
     _name: Optional[str]
-    _key_value_entries: Dict[str, Dict]
+    _records: Dict[str, KeyValueStoreRecord]
     _created_at: datetime
     _accessed_at: datetime
     _modified_at: datetime
     _file_operation_lock: asyncio.Lock
 
     def __init__(
         self,
@@ -56,15 +74,15 @@
         name: Optional[str] = None,
     ) -> None:
         """Initialize the KeyValueStoreClient."""
         self._id = id or _crypto_random_object_id()
         self._resource_directory = os.path.join(base_storage_directory, name or self._id)
         self._memory_storage_client = memory_storage_client
         self._name = name
-        self._key_value_entries = {}
+        self._records = {}
         self._created_at = datetime.now(timezone.utc)
         self._accessed_at = datetime.now(timezone.utc)
         self._modified_at = datetime.now(timezone.utc)
         self._file_operation_lock = asyncio.Lock()
 
     async def get(self) -> Optional[Dict]:
         """Retrieve the key-value store.
@@ -127,15 +145,15 @@
     async def delete(self) -> None:
         """Delete the key-value store."""
         store = next((store for store in self._memory_storage_client._key_value_stores_handled if store._id == self._id), None)
 
         if store is not None:
             async with store._file_operation_lock:
                 self._memory_storage_client._key_value_stores_handled.remove(store)
-                store._key_value_entries.clear()
+                store._records.clear()
 
                 if os.path.exists(store._resource_directory):
                     await aioshutil.rmtree(store._resource_directory)
 
     async def list_keys(self, *, limit: int = DEFAULT_API_PARAM_LIMIT, exclusive_start_key: Optional[str] = None) -> Dict:
         """List the keys in the key-value store.
 
@@ -151,15 +169,15 @@
             memory_storage_client=self._memory_storage_client, id=self._id, name=self._name)
 
         if existing_store_by_id is None:
             _raise_on_non_existing_storage(_StorageTypes.KEY_VALUE_STORE, self._id)
 
         items = []
 
-        for record in existing_store_by_id._key_value_entries.values():
+        for record in existing_store_by_id._records.values():
             size = len(record['value'])
             items.append({
                 'key': record['key'],
                 'size': size,
             })
 
         if len(items) == 0:
@@ -204,24 +222,23 @@
         # Check by id
         existing_store_by_id = self._find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client, id=self._id, name=self._name)
 
         if existing_store_by_id is None:
             _raise_on_non_existing_storage(_StorageTypes.KEY_VALUE_STORE, self._id)
 
-        entry = existing_store_by_id._key_value_entries.get(key)
+        stored_record = existing_store_by_id._records.get(key)
 
-        if entry is None:
+        if stored_record is None:
             return None
 
         record = {
-            'key': entry['key'],
-            'value': entry['value'],
-            # To guess the type, we need a real file name, not just the extension. e.g. 'file.json' instead of 'json'
-            'contentType': entry.get('content_type') or mimetypes.guess_type(f"file.{entry['extension']}")[0],
+            'key': stored_record['key'],
+            'value': stored_record['value'],
+            'contentType': stored_record.get('contentType'),
         }
 
         if not as_bytes:
             try:
                 record['value'] = _maybe_parse_body(record['value'], record['contentType'])
             except ValueError:
                 logger.exception('Error parsing key-value store record')
@@ -278,64 +295,96 @@
             if _is_file_or_bytes(value):
                 content_type = 'application/octet-stream'
             elif isinstance(value, str):
                 content_type = 'text/plain; charset=utf-8'
             else:
                 content_type = 'application/json; charset=utf-8'
 
-        extension = _guess_file_extension(content_type or '') or DEFAULT_LOCAL_FILE_EXTENSION
-
         if 'application/json' in content_type and not _is_file_or_bytes(value) and not isinstance(value, str):
             value = _json_dumps(value).encode('utf-8')
 
         async with existing_store_by_id._file_operation_lock:
-            record = {
-                'extension': extension,
+            await existing_store_by_id._update_timestamps(True)
+            record: KeyValueStoreRecord = {
                 'key': key,
                 'value': value,
-                'content_type': content_type,
+                'contentType': content_type,
             }
 
-            existing_store_by_id._key_value_entries[key] = record
+            old_record = existing_store_by_id._records.get(key)
+            existing_store_by_id._records[key] = record
 
-            await existing_store_by_id._update_timestamps(True)
-            await _set_or_delete_key_value_store_record(
-                entity_directory=existing_store_by_id._resource_directory,
-                persist_storage=self._memory_storage_client._persist_storage,
-                record=record,
-                should_set=True,
-                write_metadata=self._memory_storage_client._write_metadata,
-            )
+            if self._memory_storage_client._persist_storage:
+                if old_record is not None:
+                    if _filename_from_record(old_record) != _filename_from_record(record):
+                        await existing_store_by_id._delete_persisted_record(old_record)
+
+                await existing_store_by_id._persist_record(record)
+
+    async def _persist_record(self, record: KeyValueStoreRecord) -> None:
+        store_directory = self._resource_directory
+        record_filename = _filename_from_record(record)
+        record['filename'] = record_filename
+
+        # Ensure the directory for the entity exists
+        await makedirs(store_directory, exist_ok=True)
+
+        # Create files for the record
+        record_path = os.path.join(store_directory, record_filename)
+        record_metadata_path = os.path.join(store_directory, record_filename + '.__metadata__.json')
+
+        # Convert to bytes if string
+        if isinstance(record['value'], str):
+            record['value'] = record['value'].encode('utf-8')
+
+        async with aiofiles.open(record_path, mode='wb') as f:
+            await f.write(record['value'])
+
+        if self._memory_storage_client._write_metadata:
+            async with aiofiles.open(record_metadata_path, mode='wb') as f:
+                await f.write(_json_dumps({
+                    'key': record['key'],
+                    'contentType': record['contentType'],
+                }).encode('utf-8'))
 
     async def delete_record(self, key: str) -> None:
         """Delete the specified record from the key-value store.
 
         Args:
             key (str): The key of the record which to delete
         """
         # Check by id
         existing_store_by_id = self._find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client, id=self._id, name=self._name)
 
         if existing_store_by_id is None:
             _raise_on_non_existing_storage(_StorageTypes.KEY_VALUE_STORE, self._id)
 
-        entry = existing_store_by_id._key_value_entries.get(key)
+        record = existing_store_by_id._records.get(key)
 
-        if entry is not None:
+        if record is not None:
             async with existing_store_by_id._file_operation_lock:
-                del existing_store_by_id._key_value_entries[key]
+                del existing_store_by_id._records[key]
                 await existing_store_by_id._update_timestamps(True)
-                await _set_or_delete_key_value_store_record(
-                    entity_directory=existing_store_by_id._resource_directory,
-                    persist_storage=self._memory_storage_client._persist_storage,
-                    record=entry,
-                    should_set=False,
-                    write_metadata=self._memory_storage_client._write_metadata,
-                )
+                if self._memory_storage_client._persist_storage:
+                    await existing_store_by_id._delete_persisted_record(record)
+
+    async def _delete_persisted_record(self, record: KeyValueStoreRecord) -> None:
+        store_directory = self._resource_directory
+        record_filename = _filename_from_record(record)
+
+        # Ensure the directory for the entity exists
+        await makedirs(store_directory, exist_ok=True)
+
+        # Create files for the record
+        record_path = os.path.join(store_directory, record_filename)
+        record_metadata_path = os.path.join(store_directory, record_filename + '.__metadata__.json')
+
+        await _force_remove(record_path)
+        await _force_remove(record_metadata_path)
 
     def _to_resource_info(self) -> Dict:
         """Retrieve the key-value store info."""
         return {
             'id': self._id,
             'name': self._name,
             'accessedAt': self._accessed_at,
@@ -372,107 +421,85 @@
         memory_storage_client: 'MemoryStorageClient',
         id: Optional[str] = None,
         name: Optional[str] = None,
     ) -> 'KeyValueStoreClient':
         created_at = datetime.now(timezone.utc)
         accessed_at = datetime.now(timezone.utc)
         modified_at = datetime.now(timezone.utc)
-        internal_records: Dict[str, Dict] = {}
-
-        # Access the key value store folder
-        for entry in os.scandir(storage_directory):
-            if entry.is_file():
-                if entry.name == '__metadata__.json':
-                    # We have found the store metadata file, build out information based on it
-                    with open(os.path.join(storage_directory, entry.name), encoding='utf-8') as f:
-                        metadata = json.load(f)
-                    id = metadata['id']
-                    name = metadata['name']
-                    created_at = datetime.fromisoformat(metadata['createdAt'])
-                    accessed_at = datetime.fromisoformat(metadata['accessedAt'])
-                    modified_at = datetime.fromisoformat(metadata['modifiedAt'])
-
-                    continue
-
-                if '.__metadata__.' in entry.name:
-                    # This is an entry's metadata file, we can use it to create/extend the record
-                    with open(os.path.join(storage_directory, entry.name), encoding='utf-8') as f:
-                        metadata = json.load(f)
-
-                    new_record = {
-                        **internal_records.get(metadata['key'], {}),
-                        **metadata,
-                    }
-
-                    internal_records[metadata['key']] = new_record
-
-                    continue
-
-                with open(os.path.join(storage_directory, entry.name), 'rb') as f:
-                    file_content = f.read()
-                file_extension = pathlib.Path(entry.name).suffix
-                content_type, _ = mimetypes.guess_type(entry.name)
-                if content_type is None:
-                    content_type = 'text/plain'
-                extension = _guess_file_extension(content_type)
 
-                if file_extension == '':
-                    # We need to override and then restore the warnings filter so that the warning gets printed out,
-                    # Otherwise it would be silently swallowed
-                    with warnings.catch_warnings():
-                        warnings.simplefilter('always')
-                        warnings.warn(
-                            f"""Key-value entry "{entry.name}" for store {name or id} does not have a file extension, assuming it as text.
-                            If you want to have correct interpretation of the file, you should add a file extension to the entry.""",
-                            Warning,
-                            stacklevel=2,
-                        )
-                elif 'application/json' in content_type:
-                    try:
-                        # Try parsing the JSON ahead of time (not ideal but solves invalid files being loaded into stores)
-                        json.loads(file_content.decode('utf-8'))
-                    except json.JSONDecodeError:
-                        # We need to override and then restore the warnings filter so that the warning gets printed out,
-                        # Otherwise it would be silently swallowed
-                        with warnings.catch_warnings():
-                            warnings.simplefilter('always')
-                            warnings.warn(
-                                (f'Key-value entry "{entry.name}" for store {name or id} has invalid JSON content'
-                                    'and will be ignored from the store.'),
-                                Warning,
-                                stacklevel=2,
-                            )
-                        continue
-
-                name_split = entry.name.split('.')
-
-                if file_extension != '':
-                    name_split.pop()
-
-                key = '.'.join(name_split)
-
-                new_record = {
-                    'key': key,
-                    'extension': extension,
-                    'value': file_content,
-                    'content_type': content_type,
-                    **internal_records.get(key, {}),
-                }
-
-                internal_records[key] = new_record
+        store_metadata_path = os.path.join(storage_directory, '__metadata__.json')
+        if os.path.exists(store_metadata_path):
+            with open(store_metadata_path, encoding='utf-8') as f:
+                metadata = json.load(f)
+            id = metadata['id']
+            name = metadata['name']
+            created_at = datetime.fromisoformat(metadata['createdAt'])
+            accessed_at = datetime.fromisoformat(metadata['accessedAt'])
+            modified_at = datetime.fromisoformat(metadata['modifiedAt'])
 
         new_client = KeyValueStoreClient(
             base_storage_directory=memory_storage_client._key_value_stores_directory,
             memory_storage_client=memory_storage_client,
             id=id,
             name=name,
         )
 
-        # Overwrite properties
+        # Overwrite internal properties
         new_client._accessed_at = accessed_at
         new_client._created_at = created_at
         new_client._modified_at = modified_at
 
-        for key, record in internal_records.items():
-            new_client._key_value_entries[key] = record
+        # Scan the key value store folder, check each entry in there and parse it as a store record
+        for entry in os.scandir(storage_directory):
+            if not entry.is_file():
+                continue
+
+            # Ignore metadata files on their own
+            if entry.name.endswith('__metadata__.json'):
+                continue
+
+            with open(os.path.join(storage_directory, entry.name), 'rb') as f:
+                file_content = f.read()
+
+            # Try checking if this file has a metadata file associated with it
+            metadata = None
+            if (os.path.exists(os.path.join(storage_directory, entry.name + '.__metadata__.json'))):
+                with open(os.path.join(storage_directory, entry.name + '.__metadata__.json'), encoding='utf-8') as metadata_file:
+                    try:
+                        metadata = json.load(metadata_file)
+                        assert metadata.get('key') is not None
+                        assert metadata.get('contentType') is not None
+                    except Exception:
+                        logger.warning(
+                            f"""Metadata of key-value store entry "{entry.name}" for store {name or id} could not be parsed."""
+                            'The metadata file will be ignored.',
+                            exc_info=True,
+                        )
+
+            if not metadata:
+                content_type, _ = mimetypes.guess_type(entry.name)
+                if content_type is None:
+                    content_type = 'application/octet-stream'
+
+                metadata = {
+                    'key': pathlib.Path(entry.name).stem,
+                    'contentType': content_type,
+                }
+
+            try:
+                _maybe_parse_body(file_content, metadata['contentType'])
+            except Exception:
+                metadata['contentType'] = 'application/octet-stream'
+                logger.warning(
+                    f"""Key-value store entry "{metadata['key']}" for store {name or id} could not be parsed."""
+                    'The entry will be assumed as binary.',
+                    exc_info=True,
+                )
+
+            new_client._records[metadata['key']] = {
+                'key': metadata['key'],
+                'contentType': metadata['contentType'],
+                'filename': entry.name,
+                'value': file_content,
+            }
 
         return new_client
```

### Comparing `apify-1.1.0b5/src/apify/_memory_storage/resource_clients/key_value_store_collection.py` & `apify-1.1.0b6/src/apify/_memory_storage/resource_clients/key_value_store_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/_memory_storage/resource_clients/request_queue.py` & `apify-1.1.0b6/src/apify/_memory_storage/resource_clients/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/_memory_storage/resource_clients/request_queue_collection.py` & `apify-1.1.0b6/src/apify/_memory_storage/resource_clients/request_queue_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/_utils.py` & `apify-1.1.0b6/src/apify/_utils.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/actor.py` & `apify-1.1.0b6/src/apify/actor.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/config.py` & `apify-1.1.0b6/src/apify/config.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/consts.py` & `apify-1.1.0b6/src/apify/consts.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/event_manager.py` & `apify-1.1.0b6/src/apify/event_manager.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/log.py` & `apify-1.1.0b6/src/apify/log.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/proxy_configuration.py` & `apify-1.1.0b6/src/apify/proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/storages/base_storage.py` & `apify-1.1.0b6/src/apify/storages/base_storage.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/storages/dataset.py` & `apify-1.1.0b6/src/apify/storages/dataset.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/storages/key_value_store.py` & `apify-1.1.0b6/src/apify/storages/key_value_store.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/storages/request_queue.py` & `apify-1.1.0b6/src/apify/storages/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify/storages/storage_client_manager.py` & `apify-1.1.0b6/src/apify/storages/storage_client_manager.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify.egg-info/PKG-INFO` & `apify-1.1.0b6/src/apify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.1.0b5
+Version: 1.1.0b6
 Summary: Apify SDK for Python
 Home-page: https://github.com/apify/apify-sdk-python
 Author: Apify Technologies s.r.o.
 Author-email: support@apify.com
 License: Apache Software License
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
```

### Comparing `apify-1.1.0b5/src/apify.egg-info/SOURCES.txt` & `apify-1.1.0b6/src/apify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b5/src/apify.egg-info/requires.txt` & `apify-1.1.0b6/src/apify.egg-info/requires.txt`

 * *Files identical despite different names*

