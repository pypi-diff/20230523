# Comparing `tmp/assets2036py-0.0.15.tar.gz` & `tmp/assets2036py-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assets2036py-0.0.15.tar", last modified: Mon May 22 12:07:10 2023, max compression
+gzip compressed data, was "assets2036py-0.0.16.tar", last modified: Mon May 22 15:03:13 2023, max compression
```

## Comparing `assets2036py-0.0.15.tar` & `assets2036py-0.0.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:07:10.121992 assets2036py-0.0.15/
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-22 12:06:59.000000 assets2036py-0.0.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-22 12:06:59.000000 assets2036py-0.0.15/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-22 12:07:10.121992 assets2036py-0.0.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-22 12:06:59.000000 assets2036py-0.0.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:07:10.121992 assets2036py-0.0.15/assets2036py/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-22 12:06:59.000000 assets2036py-0.0.15/assets2036py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-05-22 12:06:59.000000 assets2036py-0.0.15/assets2036py/assetmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-05-22 12:06:59.000000 assets2036py-0.0.15/assets2036py/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-05-22 12:06:59.000000 assets2036py-0.0.15/assets2036py/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-22 12:06:59.000000 assets2036py-0.0.15/assets2036py/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:07:10.121992 assets2036py-0.0.15/assets2036py/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-22 12:06:59.000000 assets2036py-0.0.15/assets2036py/resources/_endpoint.json
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-22 12:06:59.000000 assets2036py-0.0.15/assets2036py/resources/submodel_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-22 12:06:59.000000 assets2036py-0.0.15/assets2036py/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:07:10.121992 assets2036py-0.0.15/assets2036py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-22 12:07:10.000000 assets2036py-0.0.15/assets2036py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-22 12:07:10.000000 assets2036py-0.0.15/assets2036py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 12:07:10.000000 assets2036py-0.0.15/assets2036py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 12:07:10.000000 assets2036py-0.0.15/assets2036py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 12:07:10.000000 assets2036py-0.0.15/assets2036py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 12:07:10.121992 assets2036py-0.0.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-22 12:06:59.000000 assets2036py-0.0.15/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:07:10.121992 assets2036py-0.0.15/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    27893 2023-05-22 12:06:59.000000 assets2036py-0.0.15/tests/test_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-05-22 12:06:59.000000 assets2036py-0.0.15/tests/test_assetmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-22 12:06:59.000000 assets2036py-0.0.15/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:13.675880 assets2036py-0.0.16/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-22 15:03:02.000000 assets2036py-0.0.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-22 15:03:02.000000 assets2036py-0.0.16/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-22 15:03:13.675880 assets2036py-0.0.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-22 15:03:02.000000 assets2036py-0.0.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:13.675880 assets2036py-0.0.16/assets2036py/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-22 15:03:02.000000 assets2036py-0.0.16/assets2036py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-05-22 15:03:02.000000 assets2036py-0.0.16/assets2036py/assetmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-05-22 15:03:02.000000 assets2036py-0.0.16/assets2036py/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-05-22 15:03:02.000000 assets2036py-0.0.16/assets2036py/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-22 15:03:02.000000 assets2036py-0.0.16/assets2036py/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:13.675880 assets2036py-0.0.16/assets2036py/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-22 15:03:02.000000 assets2036py-0.0.16/assets2036py/resources/_endpoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-22 15:03:02.000000 assets2036py-0.0.16/assets2036py/resources/submodel_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-22 15:03:02.000000 assets2036py-0.0.16/assets2036py/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:13.675880 assets2036py-0.0.16/assets2036py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-22 15:03:13.000000 assets2036py-0.0.16/assets2036py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-22 15:03:13.000000 assets2036py-0.0.16/assets2036py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:03:13.000000 assets2036py-0.0.16/assets2036py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 15:03:13.000000 assets2036py-0.0.16/assets2036py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 15:03:13.000000 assets2036py-0.0.16/assets2036py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 15:03:13.675880 assets2036py-0.0.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-22 15:03:02.000000 assets2036py-0.0.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:13.675880 assets2036py-0.0.16/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    28458 2023-05-22 15:03:02.000000 assets2036py-0.0.16/tests/test_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-05-22 15:03:02.000000 assets2036py-0.0.16/tests/test_assetmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-22 15:03:02.000000 assets2036py-0.0.16/tests/test_utils.py
```

### Comparing `assets2036py-0.0.15/LICENSE` & `assets2036py-0.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.15/NOTICE` & `assets2036py-0.0.16/NOTICE`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.15/assets2036py/__init__.py` & `assets2036py-0.0.16/assets2036py/__init__.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.15/assets2036py/assetmanager.py` & `assets2036py-0.0.16/assets2036py/assetmanager.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.15/assets2036py/assets.py` & `assets2036py-0.0.16/assets2036py/assets.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
+import time
 from enum import Enum
 from os import path
 import json
 import ssl
 import traceback
 from json import JSONDecodeError
 from urllib.request import urlopen
@@ -291,14 +292,29 @@
             if "properties" in submodel_definition:
                 self._create_readonly_properties(submodel_definition)
             if "operations" in submodel_definition:
                 self._create_callable_operations(submodel_definition)
             if "events" in submodel_definition:
                 self._create_subscribable_events(submodel_definition)
 
+    def is_online(self):
+        num_tries = 0
+        if self.name == "_endpoint":
+            online_prop = self.online
+        else:
+            online_prop = self.endpoint_asset._endpoint.online
+        while num_tries < 3:
+            online_state = online_prop.value
+            if online_state == None:
+                num_tries += 1
+                time.sleep(0.5)
+            else:
+                return online_state
+        return False
+
     def _raise_offline_exception(self, online):
         logger.debug("CALLBACK GOT %s", online)
         if not online and self._disconnect_callback != None:
             logger.debug("SEND DISCONNECT FOR %s", self.name)
             self._disconnect_callback(self.name)
 
     def on_disconnect(self, callback):
@@ -435,13 +451,21 @@
             sm_def = meta_info["submodel_definition"]
             submodel_defs.append(sm_def)
             sources[sm_def["name"]] = meta_info["source"]
 
         super().__init__(name, namespace, *submodel_defs, mode=mode,
                          communication_client=communication_client, endpoint_name=endpoint_name)
         for name, source in sources.items():
-            getattr(self, name).register_source(source)
-            # this is some hacky shit, we need some nicer refactoring here
+            if name != "_endpoint":
+                getattr(self, name).register_source(source)
+                # this is some hacky shit, we need some nicer refactoring here
+
+    @property
+    def is_online(self):
+        for submodel in self.sub_model_names:
+            if not getattr(self, submodel).is_online():
+                return False
+        return True
 
     def on_disconnect(self, callback):
         for submodel in self.sub_model_names:
             getattr(self, submodel).on_disconnect(callback)
```

### Comparing `assets2036py-0.0.15/assets2036py/communication.py` & `assets2036py-0.0.16/assets2036py/communication.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.15/assets2036py/exceptions.py` & `assets2036py-0.0.16/assets2036py/exceptions.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.15/assets2036py/resources/_endpoint.json` & `assets2036py-0.0.16/assets2036py/resources/_endpoint.json`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.15/assets2036py/resources/submodel_schema.json` & `assets2036py-0.0.16/assets2036py/resources/submodel_schema.json`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.15/assets2036py/utilities.py` & `assets2036py-0.0.16/assets2036py/utilities.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.15/assets2036py.egg-info/SOURCES.txt` & `assets2036py-0.0.16/assets2036py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.15/setup.py` & `assets2036py-0.0.16/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='assets2036py',
-    version='0.0.15',
+    version='0.0.16',
     url='https://github.com/boschresearch/assets2036-submodels',
     license='BIOS',
     author='Daniel Ewert (CR/APA3 G6/BD-BBI)',
     author_email='Daniel.Ewert@de.bosch.com',
     description='helper library to easily implement assets2036',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `assets2036py-0.0.15/tests/test_asset.py` & `assets2036py-0.0.16/tests/test_asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -661,15 +661,15 @@
         owner.simple_operation.bind_addnumbers(do_addnumbers)
 
         time.sleep(1)
 
         res = sink.simple_operation.addnumbers(a=5, b=6)
         self.assertEqual(res, 11)
 
-    def test_asset_offline_exception(self):
+    def test_asset_disconnect_callback(self):
         mgr = AssetManager(HOST, PORT, "test_arena2036", "test_endpoint_1")
         mgr2 = AssetManager(HOST, PORT, "test_arena2036", "test_endpoint_2")
         asset = mgr.create_asset("test_asset", res_url + "simple_prop.json")
         callback_called = False
 
         def disconnect_callback(*args):
             nonlocal callback_called
@@ -690,7 +690,20 @@
         for _ in range(20):
             my_prop = asset_proxy.simple_prop_json.my_property.value
             if callback_called:
                 break
             time.sleep(0.5)
 
         self.assertTrue(callback_called)
+
+    def test_is_proxy_asset_online(self):
+        mgr = AssetManager(HOST, PORT, "test_arena2036", "test_endpoint_1")
+        mgr2 = AssetManager(HOST, PORT, "test_arena2036", "test_endpoint_2")
+        asset = mgr.create_asset("test_asset", res_url + "simple_prop.json")
+        asset.simple_prop_json.my_property.value = 42
+
+        asset_proxy = mgr2.create_asset_proxy(
+            "test_arena2036", "test_asset")
+        self.assertTrue(asset_proxy.is_online)
+        asset.disconnect()
+        time.sleep(1)
+        self.assertFalse(asset_proxy.is_online)
```

### Comparing `assets2036py-0.0.15/tests/test_assetmanager.py` & `assets2036py-0.0.16/tests/test_assetmanager.py`

 * *Files identical despite different names*

### Comparing `assets2036py-0.0.15/tests/test_utils.py` & `assets2036py-0.0.16/tests/test_utils.py`

 * *Files identical despite different names*

