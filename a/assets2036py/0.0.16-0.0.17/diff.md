# Comparing `tmp/assets2036py-0.0.16.tar.gz` & `tmp/assets2036py-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assets2036py-0.0.16.tar", last modified: Mon May 22 15:03:13 2023, max compression
+gzip compressed data, was "assets2036py-0.0.17.tar", last modified: Tue May 23 13:17:18 2023, max compression
```

## Comparing `assets2036py-0.0.16.tar` & `assets2036py-0.0.17.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:13.675880 assets2036py-0.0.16/
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-22 15:03:02.000000 assets2036py-0.0.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-22 15:03:02.000000 assets2036py-0.0.16/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-22 15:03:13.675880 assets2036py-0.0.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-22 15:03:02.000000 assets2036py-0.0.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:13.675880 assets2036py-0.0.16/assets2036py/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-22 15:03:02.000000 assets2036py-0.0.16/assets2036py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-05-22 15:03:02.000000 assets2036py-0.0.16/assets2036py/assetmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-05-22 15:03:02.000000 assets2036py-0.0.16/assets2036py/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-05-22 15:03:02.000000 assets2036py-0.0.16/assets2036py/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-22 15:03:02.000000 assets2036py-0.0.16/assets2036py/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:13.675880 assets2036py-0.0.16/assets2036py/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-22 15:03:02.000000 assets2036py-0.0.16/assets2036py/resources/_endpoint.json
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-22 15:03:02.000000 assets2036py-0.0.16/assets2036py/resources/submodel_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-22 15:03:02.000000 assets2036py-0.0.16/assets2036py/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:13.675880 assets2036py-0.0.16/assets2036py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-22 15:03:13.000000 assets2036py-0.0.16/assets2036py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-22 15:03:13.000000 assets2036py-0.0.16/assets2036py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:03:13.000000 assets2036py-0.0.16/assets2036py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 15:03:13.000000 assets2036py-0.0.16/assets2036py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 15:03:13.000000 assets2036py-0.0.16/assets2036py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 15:03:13.675880 assets2036py-0.0.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-22 15:03:02.000000 assets2036py-0.0.16/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:13.675880 assets2036py-0.0.16/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    28458 2023-05-22 15:03:02.000000 assets2036py-0.0.16/tests/test_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-05-22 15:03:02.000000 assets2036py-0.0.16/tests/test_assetmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-22 15:03:02.000000 assets2036py-0.0.16/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:17:18.594671 assets2036py-0.0.17/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-23 13:17:05.000000 assets2036py-0.0.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-23 13:17:05.000000 assets2036py-0.0.17/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-23 13:17:18.594671 assets2036py-0.0.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-23 13:17:05.000000 assets2036py-0.0.17/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:17:18.594671 assets2036py-0.0.17/assets2036py/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-23 13:17:05.000000 assets2036py-0.0.17/assets2036py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-05-23 13:17:05.000000 assets2036py-0.0.17/assets2036py/assetmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17414 2023-05-23 13:17:05.000000 assets2036py-0.0.17/assets2036py/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-05-23 13:17:05.000000 assets2036py-0.0.17/assets2036py/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-23 13:17:05.000000 assets2036py-0.0.17/assets2036py/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:17:18.594671 assets2036py-0.0.17/assets2036py/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-23 13:17:05.000000 assets2036py-0.0.17/assets2036py/resources/_endpoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-23 13:17:05.000000 assets2036py-0.0.17/assets2036py/resources/submodel_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-23 13:17:05.000000 assets2036py-0.0.17/assets2036py/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:17:18.594671 assets2036py-0.0.17/assets2036py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-23 13:17:18.000000 assets2036py-0.0.17/assets2036py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-23 13:17:18.000000 assets2036py-0.0.17/assets2036py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:17:18.000000 assets2036py-0.0.17/assets2036py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 13:17:18.000000 assets2036py-0.0.17/assets2036py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 13:17:18.000000 assets2036py-0.0.17/assets2036py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:17:18.594671 assets2036py-0.0.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-23 13:17:05.000000 assets2036py-0.0.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:17:18.594671 assets2036py-0.0.17/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    29160 2023-05-23 13:17:05.000000 assets2036py-0.0.17/tests/test_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-05-23 13:17:05.000000 assets2036py-0.0.17/tests/test_assetmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-23 13:17:05.000000 assets2036py-0.0.17/tests/test_utils.py
```

### Comparing `assets2036py-0.0.16/LICENSE` & `assets2036py-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.16/NOTICE` & `assets2036py-0.0.17/NOTICE`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.16/PKG-INFO` & `assets2036py-0.0.17/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: assets2036py
-Version: 0.0.16
+Version: 0.0.17
 Summary: helper library to easily implement assets2036
-Home-page: https://github.com/boschresearch/assets2036-submodels
+Home-page: https://github.com/boschresearch/assets2036spy
 Author: Daniel Ewert (CR/APA3 G6/BD-BBI)
 Author-email: Daniel.Ewert@de.bosch.com
 License: BIOS
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
```

### Comparing `assets2036py-0.0.16/assets2036py/__init__.py` & `assets2036py-0.0.17/assets2036py/__init__.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.16/assets2036py/assetmanager.py` & `assets2036py-0.0.17/assets2036py/assetmanager.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import ssl
 import json
 import os
 import logging
 from urllib.request import urlopen
 from threading import Thread, Event
 from assets2036py import Asset, Mode, ProxyAsset
-from assets2036py.exceptions import AssetNotFoundError, OperationTimeoutException
+from assets2036py.exceptions import AssetNotFoundError, OperationTimeoutException, AssetNotOnlineError
 from assets2036py.communication import CommunicationClient, MQTTClient
 from assets2036py.utilities import get_resource_path
 
 
 logger = logging.getLogger(__name__)
 
 # pylint: disable=line-too-long
@@ -195,33 +195,42 @@
 
         Returns:
             list: list of found asset names
         """
 
         return self.client.query_asset_names(namespace, *submodel_names)
 
-    def create_asset_proxy(self, namespace: str, name: str) -> ProxyAsset:
+    def create_asset_proxy(self, namespace: str, name: str, wait_seconds_until_online: int = -1) -> ProxyAsset:
         """Returns the asset with the given name if found, raises AssetNotFoundError otherwise
 
         Args:
             namespace (str): namespace to use
             name (str): name of asset to use
+            wait_seconds_until_online (int): seconds to wait for the asset to register as online.
+                -1 ignores online state and initiates asset (default: -1)
 
         Raises:
             AssetNotFoundError: raised if Asset cannot be found
+            AssetNotOnlineError: raised if Asset doesn't come online in set time
 
         Returns:
             Asset: returns Asset proxy to be used to communicate with remote asset
         """
         submodels = self.client.query_submodels_for_asset(namespace, name)
         if not submodels:
             raise AssetNotFoundError
         # verified_submodels = self._get_submodel_schemata(submodels)
-        return ProxyAsset(name, namespace, *submodels.values(), mode=Mode.CONSUMER, communication_client=self.client,
-                          endpoint_name=self.endpoint_name)
+
+        proxy_asset = ProxyAsset(name, namespace, *submodels.values(), mode=Mode.CONSUMER, communication_client=self.client,
+                                 endpoint_name=self.endpoint_name)
+        if wait_seconds_until_online >= 0:
+            online = proxy_asset.wait_for_online(wait_seconds_until_online)
+            if not online:
+                raise AssetNotOnlineError
+        return proxy_asset
 
     def _get_submodel_schemata(self, sub_models):
         # pylint: disable=protected-access,broad-except
         schemata = []
         for meta in sub_models.values():
             try:
                 url = meta["submodel_url"]
```

### Comparing `assets2036py-0.0.16/assets2036py/assets.py` & `assets2036py-0.0.17/assets2036py/assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,21 +292,21 @@
             if "properties" in submodel_definition:
                 self._create_readonly_properties(submodel_definition)
             if "operations" in submodel_definition:
                 self._create_callable_operations(submodel_definition)
             if "events" in submodel_definition:
                 self._create_subscribable_events(submodel_definition)
 
-    def is_online(self):
+    def is_online(self, seconds_to_wait):
         num_tries = 0
         if self.name == "_endpoint":
             online_prop = self.online
         else:
             online_prop = self.endpoint_asset._endpoint.online
-        while num_tries < 3:
+        while num_tries < seconds_to_wait * 2:
             online_state = online_prop.value
             if online_state == None:
                 num_tries += 1
                 time.sleep(0.5)
             else:
                 return online_state
         return False
@@ -457,15 +457,18 @@
         for name, source in sources.items():
             if name != "_endpoint":
                 getattr(self, name).register_source(source)
                 # this is some hacky shit, we need some nicer refactoring here
 
     @property
     def is_online(self):
+        return self.wait_for_online(3)
+
+    def wait_for_online(self, seconds_to_wait):
         for submodel in self.sub_model_names:
-            if not getattr(self, submodel).is_online():
+            if not getattr(self, submodel).is_online(seconds_to_wait):
                 return False
         return True
 
     def on_disconnect(self, callback):
         for submodel in self.sub_model_names:
             getattr(self, submodel).on_disconnect(callback)
```

### Comparing `assets2036py-0.0.16/assets2036py/communication.py` & `assets2036py-0.0.17/assets2036py/communication.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.16/assets2036py/exceptions.py` & `assets2036py-0.0.17/assets2036py/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,7 +31,11 @@
 
 class NotReadableError(Exception):
     pass
 
 
 class InvalidParameterException(Exception):
     pass
+
+
+class AssetNotOnlineError(Exception):
+    pass
```

### Comparing `assets2036py-0.0.16/assets2036py/resources/_endpoint.json` & `assets2036py-0.0.17/assets2036py/resources/_endpoint.json`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.16/assets2036py/resources/submodel_schema.json` & `assets2036py-0.0.17/assets2036py/resources/submodel_schema.json`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.16/assets2036py/utilities.py` & `assets2036py-0.0.17/assets2036py/utilities.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.16/assets2036py.egg-info/PKG-INFO` & `assets2036py-0.0.17/assets2036py.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: assets2036py
-Version: 0.0.16
+Version: 0.0.17
 Summary: helper library to easily implement assets2036
-Home-page: https://github.com/boschresearch/assets2036-submodels
+Home-page: https://github.com/boschresearch/assets2036spy
 Author: Daniel Ewert (CR/APA3 G6/BD-BBI)
 Author-email: Daniel.Ewert@de.bosch.com
 License: BIOS
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
```

### Comparing `assets2036py-0.0.16/assets2036py.egg-info/SOURCES.txt` & `assets2036py-0.0.17/assets2036py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.16/setup.py` & `assets2036py-0.0.17/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='assets2036py',
-    version='0.0.16',
-    url='https://github.com/boschresearch/assets2036-submodels',
+    version='0.0.17',
+    url='https://github.com/boschresearch/assets2036spy',
     license='BIOS',
     author='Daniel Ewert (CR/APA3 G6/BD-BBI)',
     author_email='Daniel.Ewert@de.bosch.com',
     description='helper library to easily implement assets2036',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(exclude=['contrib', 'docs', 'tests', 'examples']),
```

### Comparing `assets2036py-0.0.16/tests/test_asset.py` & `assets2036py-0.0.17/tests/test_asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from threading import Thread
 from multiprocessing import Pool
 from concurrent.futures import ThreadPoolExecutor
 
 from jsonschema import ValidationError
 from assets2036py import Asset, Mode, AssetManager
 from assets2036py.communication import MockClient
-from assets2036py.exceptions import NotWritableError
+from assets2036py.exceptions import NotWritableError, AssetNotOnlineError
 from .test_utils import get_msgs_for_n_secs, wipe_retained_msgs, res_url
 logger = logging.getLogger(__name__)
 
 HOST = os.getenv("MQTT_BROKER_URL", "localhost")
 PORT = int(os.getenv("MQTT_BROKER_PORT", "1883"))
 # HINT: Add an .env file to the root of your project to set the environment variables
 
@@ -703,7 +703,25 @@
 
         asset_proxy = mgr2.create_asset_proxy(
             "test_arena2036", "test_asset")
         self.assertTrue(asset_proxy.is_online)
         asset.disconnect()
         time.sleep(1)
         self.assertFalse(asset_proxy.is_online)
+
+    def test_proxy_not_online_exception(self):
+        mgr = AssetManager(HOST, PORT, "test_arena2036", "test_endpoint_1")
+        asset = mgr.create_asset("test_asset", res_url + "simple_prop.json")
+        asset.simple_prop_json.my_property.value = 42
+        time.sleep(1)
+
+        def create_proxy():
+            mgr2 = AssetManager(
+                HOST, PORT, "test_arena2036", "test_endpoint_2")
+            asset_proxy = mgr2.create_asset_proxy(
+                "test_arena2036", "test_asset", 3)
+            return True
+
+        self.assertTrue(create_proxy())
+        asset.disconnect()
+        time.sleep(1)
+        self.assertRaises(AssetNotOnlineError, create_proxy)
```

### Comparing `assets2036py-0.0.16/tests/test_assetmanager.py` & `assets2036py-0.0.17/tests/test_assetmanager.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.16/tests/test_utils.py` & `assets2036py-0.0.17/tests/test_utils.py`

 * *Files identical despite different names*

