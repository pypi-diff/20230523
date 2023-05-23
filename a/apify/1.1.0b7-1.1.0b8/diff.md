# Comparing `tmp/apify-1.1.0b7.tar.gz` & `tmp/apify-1.1.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify-1.1.0b7.tar", last modified: Tue May 23 14:12:14 2023, max compression
+gzip compressed data, was "apify-1.1.0b8.tar", last modified: Tue May 23 15:25:34 2023, max compression
```

## Comparing `apify-1.1.0b7.tar` & `apify-1.1.0b8.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:12:14.602346 apify-1.1.0b7/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-23 14:12:00.000000 apify-1.1.0b7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-23 14:12:14.602346 apify-1.1.0b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-23 14:12:00.000000 apify-1.1.0b7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:12:14.602346 apify-1.1.0b7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-23 14:12:00.000000 apify-1.1.0b7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:12:14.590346 apify-1.1.0b7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:12:14.598346 apify-1.1.0b7/src/apify/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:12:14.602346 apify-1.1.0b7/src/apify/_memory_storage/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/file_storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/memory_storage_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:12:14.602346 apify-1.1.0b7/src/apify/_memory_storage/resource_clients/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/resource_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/resource_clients/base_resource_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19664 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/resource_clients/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/resource_clients/dataset_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19736 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/resource_clients/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19050 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/resource_clients/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_memory_storage/resource_clients/request_queue_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 14:12:14.000000 apify-1.1.0b7/src/apify/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    58928 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/proxy_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:12:14.602346 apify-1.1.0b7/src/apify/storages/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/storages/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    23398 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/storages/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/storages/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    25879 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/storages/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-23 14:12:00.000000 apify-1.1.0b7/src/apify/storages/storage_client_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:12:14.598346 apify-1.1.0b7/src/apify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-23 14:12:14.000000 apify-1.1.0b7/src/apify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-23 14:12:14.000000 apify-1.1.0b7/src/apify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:12:14.000000 apify-1.1.0b7/src/apify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-23 14:12:14.000000 apify-1.1.0b7/src/apify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 14:12:14.000000 apify-1.1.0b7/src/apify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:25:34.456034 apify-1.1.0b8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-23 15:24:54.000000 apify-1.1.0b8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-23 15:25:34.456034 apify-1.1.0b8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-23 15:24:54.000000 apify-1.1.0b8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-23 15:25:30.000000 apify-1.1.0b8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 15:25:34.456034 apify-1.1.0b8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:25:34.452034 apify-1.1.0b8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:25:34.456034 apify-1.1.0b8/src/apify/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:25:34.456034 apify-1.1.0b8/src/apify/_memory_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/file_storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/memory_storage_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:25:34.456034 apify-1.1.0b8/src/apify/_memory_storage/resource_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/resource_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/resource_clients/base_resource_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19664 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/resource_clients/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/resource_clients/dataset_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19736 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/resource_clients/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19050 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/resource_clients/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_memory_storage/resource_clients/request_queue_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58928 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/proxy_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:25:34.456034 apify-1.1.0b8/src/apify/storages/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/storages/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23398 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/storages/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/storages/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25879 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/storages/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-23 15:24:54.000000 apify-1.1.0b8/src/apify/storages/storage_client_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:25:34.456034 apify-1.1.0b8/src/apify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-23 15:25:34.000000 apify-1.1.0b8/src/apify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-23 15:25:34.000000 apify-1.1.0b8/src/apify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:25:34.000000 apify-1.1.0b8/src/apify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-23 15:25:34.000000 apify-1.1.0b8/src/apify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 15:25:34.000000 apify-1.1.0b8/src/apify.egg-info/top_level.txt
```

### Comparing `apify-1.1.0b7/LICENSE` & `apify-1.1.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/PKG-INFO` & `apify-1.1.0b8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.1.0b7
+Version: 1.1.0b8
 Summary: Apify SDK for Python
-Home-page: https://github.com/apify/apify-sdk-python
-Author: Apify Technologies s.r.o.
-Author-email: support@apify.com
+Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
+Project-URL: Homepage, https://docs.apify.com/sdk/python/
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
 Project-URL: Issue tracker, https://github.com/apify/apify-sdk-python/issues
+Project-URL: Changelog, https://github.com/apify/apify-sdk-python/blob/master/CHANGELOG.md
 Project-URL: Apify Homepage, https://apify.com
 Keywords: apify,sdk,actor,scraping,automation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `apify-1.1.0b7/README.md` & `apify-1.1.0b8/README.md`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/_crypto.py` & `apify-1.1.0b8/src/apify/_crypto.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/_memory_storage/file_storage_utils.py` & `apify-1.1.0b8/src/apify/_memory_storage/file_storage_utils.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/_memory_storage/memory_storage_client.py` & `apify-1.1.0b8/src/apify/_memory_storage/memory_storage_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/_memory_storage/resource_clients/__init__.py` & `apify-1.1.0b8/src/apify/_memory_storage/resource_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/_memory_storage/resource_clients/base_resource_client.py` & `apify-1.1.0b8/src/apify/_memory_storage/resource_clients/base_resource_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py` & `apify-1.1.0b8/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/_memory_storage/resource_clients/dataset.py` & `apify-1.1.0b8/src/apify/_memory_storage/resource_clients/dataset.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/_memory_storage/resource_clients/dataset_collection.py` & `apify-1.1.0b8/src/apify/_memory_storage/resource_clients/dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/_memory_storage/resource_clients/key_value_store.py` & `apify-1.1.0b8/src/apify/_memory_storage/resource_clients/key_value_store.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/_memory_storage/resource_clients/key_value_store_collection.py` & `apify-1.1.0b8/src/apify/_memory_storage/resource_clients/key_value_store_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/_memory_storage/resource_clients/request_queue.py` & `apify-1.1.0b8/src/apify/_memory_storage/resource_clients/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/_memory_storage/resource_clients/request_queue_collection.py` & `apify-1.1.0b8/src/apify/_memory_storage/resource_clients/request_queue_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/_utils.py` & `apify-1.1.0b8/src/apify/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,26 +12,24 @@
 import re
 import sys
 import time
 from collections import OrderedDict
 from collections.abc import MutableMapping
 from datetime import datetime, timezone
 from enum import Enum
+from importlib import metadata
 from typing import Any, Callable, Dict, Generic, ItemsView, Iterator, List, NoReturn, Optional
 from typing import OrderedDict as OrderedDictType
 from typing import Tuple, Type, TypeVar, Union, ValuesView, cast, overload
 
 import aioshutil
 import psutil
 from aiofiles import ospath
 from aiofiles.os import remove, rename
 
-from apify_client import __version__ as client_version
-
-from ._version import __version__ as sdk_version
 from .consts import (
     _BOOL_ENV_VARS_TYPE,
     _DATETIME_ENV_VARS_TYPE,
     _FLOAT_ENV_VARS_TYPE,
     _INTEGER_ENV_VARS_TYPE,
     _STRING_ENV_VARS_TYPE,
     BOOL_ENV_VARS,
@@ -51,16 +49,16 @@
     return method
 
 
 def _get_system_info() -> Dict:
     python_version = '.'.join([str(x) for x in sys.version_info[:3]])
 
     system_info: Dict[str, Union[str, bool]] = {
-        'apify_sdk_version': sdk_version,
-        'apify_client_version': client_version,
+        'apify_sdk_version': metadata.version('apify'),
+        'apify_client_version': metadata.version('apify-client'),
         'python_version': python_version,
         'os': sys.platform,
     }
 
     if _is_running_in_ipython():
         system_info['is_running_in_ipython'] = True
```

### Comparing `apify-1.1.0b7/src/apify/actor.py` & `apify-1.1.0b8/src/apify/actor.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/config.py` & `apify-1.1.0b8/src/apify/config.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/consts.py` & `apify-1.1.0b8/src/apify/consts.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/event_manager.py` & `apify-1.1.0b8/src/apify/event_manager.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/log.py` & `apify-1.1.0b8/src/apify/log.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/proxy_configuration.py` & `apify-1.1.0b8/src/apify/proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/storages/base_storage.py` & `apify-1.1.0b8/src/apify/storages/base_storage.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/storages/dataset.py` & `apify-1.1.0b8/src/apify/storages/dataset.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/storages/key_value_store.py` & `apify-1.1.0b8/src/apify/storages/key_value_store.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/storages/request_queue.py` & `apify-1.1.0b8/src/apify/storages/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify/storages/storage_client_manager.py` & `apify-1.1.0b8/src/apify/storages/storage_client_manager.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b7/src/apify.egg-info/PKG-INFO` & `apify-1.1.0b8/src/apify.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.1.0b7
+Version: 1.1.0b8
 Summary: Apify SDK for Python
-Home-page: https://github.com/apify/apify-sdk-python
-Author: Apify Technologies s.r.o.
-Author-email: support@apify.com
+Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
+Project-URL: Homepage, https://docs.apify.com/sdk/python/
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
 Project-URL: Issue tracker, https://github.com/apify/apify-sdk-python/issues
+Project-URL: Changelog, https://github.com/apify/apify-sdk-python/blob/master/CHANGELOG.md
 Project-URL: Apify Homepage, https://apify.com
 Keywords: apify,sdk,actor,scraping,automation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `apify-1.1.0b7/src/apify.egg-info/SOURCES.txt` & `apify-1.1.0b8/src/apify.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 README.md
-setup.py
+pyproject.toml
 src/apify/__init__.py
 src/apify/_crypto.py
 src/apify/_types.py
 src/apify/_utils.py
-src/apify/_version.py
 src/apify/actor.py
 src/apify/config.py
 src/apify/consts.py
 src/apify/event_manager.py
 src/apify/log.py
 src/apify/proxy_configuration.py
 src/apify/py.typed
```

### Comparing `apify-1.1.0b7/src/apify.egg-info/requires.txt` & `apify-1.1.0b8/src/apify.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-aiofiles~=22.1.0
-aioshutil~=1.2
-apify-client~=1.1
+aiofiles~=23.1.0
+aioshutil~=1.3
+apify-client~=1.2.0
 colorama~=0.4.6
-cryptography~=39.0.1
-httpx~=0.23.0
-psutil~=5.9.4
-pyee~=9.0.4
+cryptography~=40.0.2
+httpx~=0.24.1
+psutil~=5.9.5
+pyee~=9.1.0
 sortedcollections~=2.1.0
-typing-extensions~=4.4.0
-websockets~=10.4
+typing-extensions~=4.6.0
+websockets~=11.0.3
 
 [dev]
-autopep8~=2.0.1
-filelock~=3.9.0
+autopep8~=2.0.2
+build~=0.10.0
+filelock~=3.12.0
 flake8~=6.0.0
-flake8-bugbear~=23.1.20
+flake8-bugbear~=23.5.9
 flake8-commas~=2.1.0
-flake8-comprehensions~=3.10.1
+flake8-comprehensions~=3.12.0
 flake8-datetimez~=20.10.0
 flake8-docstrings~=1.7.0
 flake8-encodings~=0.5.0
 flake8-isort~=6.0.0
-flake8-noqa~=1.3.0
+flake8-noqa~=1.3.1
 flake8-pytest-style~=1.7.2
-flake8-quotes~=3.3.1
+flake8-quotes~=3.3.2
 flake8-unused-arguments~=0.0.13
 isort~=5.12.0
-mypy~=1.0.0
-pep8-naming~=0.13.2
-pre-commit~=3.0.1
-pytest~=7.2.0
-pytest-asyncio~=0.20.3
+mypy~=1.3.0
+pep8-naming~=0.13.3
+pre-commit~=3.3.2
+pytest~=7.3.1
+pytest-asyncio~=0.21.0
 pytest-only~=2.0.0
 pytest-randomly~=3.12.0
 pytest-timeout~=2.1.0
-pytest-xdist~=3.2.0
+pytest-xdist~=3.3.1
 respx~=0.20.1
 sphinx~=6.1.3
 sphinx-autodoc-typehints~=1.22
 sphinx-markdown-builder==0.5.4
-types-aiofiles~=22.1.0.4
-types-colorama~=0.4.15.7
-types-psutil~=5.9.5.5
-types-setuptools
+twine~=4.0.2
+types-aiofiles~=23.1.0.3
+types-colorama~=0.4.15.11
+types-psutil~=5.9.5.12
```

