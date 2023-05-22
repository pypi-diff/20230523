# Comparing `tmp/proconip-0.0.2.tar.gz` & `tmp/proconip-1.0.0.tar.gz`

## Comparing `proconip-0.0.2.tar` & `proconip-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 proconip-0.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 proconip-0.0.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 proconip-0.0.2/SECURITY.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 proconip-0.0.2/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 proconip-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 proconip-0.0.2/.github/workflows/unittest.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 proconip-0.0.2/src/requirements.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 proconip-0.0.2/src/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-0.0.2/src/proconip/__init__.py
--rw-r--r--   0        0        0     6006 2020-02-02 00:00:00.000000 proconip-0.0.2/src/proconip/api.py
--rw-r--r--   0        0        0    21899 2020-02-02 00:00:00.000000 proconip-0.0.2/src/proconip/definitions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 proconip-0.0.2/tests/helper.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 proconip-0.0.2/tests/requirements.txt
--rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 proconip-0.0.2/tests/test_definitions.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 proconip-0.0.2/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 proconip-0.0.2/LICENSE
--rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 proconip-0.0.2/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proconip-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 proconip-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 proconip-1.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 proconip-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 proconip-1.0.0/SECURITY.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 proconip-1.0.0/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 proconip-1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 proconip-1.0.0/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 proconip-1.0.0/src/requirements.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 proconip-1.0.0/src/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.0.0/src/proconip/__init__.py
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 proconip-1.0.0/src/proconip/api.py
+-rw-r--r--   0        0        0    21918 2020-02-02 00:00:00.000000 proconip-1.0.0/src/proconip/definitions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 proconip-1.0.0/tests/helper.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 proconip-1.0.0/tests/requirements.txt
+-rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 proconip-1.0.0/tests/test_definitions.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 proconip-1.0.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 proconip-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 proconip-1.0.0/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proconip-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 proconip-1.0.0/PKG-INFO
```

### Comparing `proconip-0.0.2/CODE_OF_CONDUCT.md` & `proconip-1.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `proconip-0.0.2/CONTRIBUTING.md` & `proconip-1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `proconip-0.0.2/.github/workflows/pylint.yml` & `proconip-1.0.0/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `proconip-0.0.2/.github/workflows/python-publish.yml` & `proconip-1.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `proconip-0.0.2/.github/workflows/unittest.yml` & `proconip-1.0.0/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `proconip-0.0.2/src/proconip/api.py` & `proconip-1.0.0/src/proconip/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     """Switch on a relay using the usrcfg.cgi interface."""
     bit_state = current_state.determine_overall_relay_bit_state()
     relay_bit_mask = relay.get_bit_mask()
     bit_state[0] |= relay_bit_mask
     bit_state[1] |= relay_bit_mask
     url = URL(config.base_url).with_path(API_PATH_USRCFG)
     result = await client_session.post(url,
-                                       data=f"ENA={bit_state}&MANUAL=1",
+                                       data=f"ENA={bit_state[0]},{bit_state[1]}&MANUAL=1",
                                        auth=BasicAuth(config.username,
                                                       password=config.password))
     if result.status != 200:
         raise BasStatusCodeException(f"Unexpected status code: {result.status}")
     if result.status in [401, 403]:
         raise BadCredentialsException
 
@@ -75,15 +75,15 @@
     """Switch on a relay using the usrcfg.cgi interface."""
     bit_state = current_state.determine_overall_relay_bit_state()
     relay_bit_mask = relay.get_bit_mask()
     bit_state[0] |= relay_bit_mask
     bit_state[1] &= ~relay_bit_mask
     url = URL(config.base_url).with_path(API_PATH_USRCFG)
     result = await client_session.post(url,
-                                       data=f"ENA={bit_state}&MANUAL=1",
+                                       data=f"ENA={bit_state[0]},{bit_state[1]}&MANUAL=1",
                                        auth=BasicAuth(config.username,
                                                       password=config.password))
     if result.status != 200:
         raise BasStatusCodeException(f"Unexpected status code: {result.status}")
     if result.status in [401, 403]:
         raise BadCredentialsException
 
@@ -96,15 +96,15 @@
     """Switch on a relay using the usrcfg.cgi interface."""
     bit_state = current_state.determine_overall_relay_bit_state()
     relay_bit_mask = relay.get_bit_mask()
     bit_state[0] &= ~relay_bit_mask
     bit_state[1] &= ~relay_bit_mask
     url = URL(config.base_url).with_path(API_PATH_USRCFG)
     result = await client_session.post(url,
-                                       data=f"ENA={bit_state}&MANUAL=1",
+                                       data=f"ENA={bit_state[0]},{bit_state[1]}&MANUAL=1",
                                        auth=BasicAuth(config.username,
                                                       password=config.password))
     if result.status != 200:
         raise BasStatusCodeException(f"Unexpected status code: {result.status}")
     if result.status in [401, 403]:
         raise BadCredentialsException
```

### Comparing `proconip-0.0.2/src/proconip/definitions.py` & `proconip-1.0.0/src/proconip/definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -594,12 +594,12 @@
         relays = self.relays()
         bit_state = [255, 0]
         if self.is_relay_extension_enabled():
             relays.extend(self.external_relays())
             bit_state[0] = 65535
         for relay in relays:
             relay_bit_mask = relay.get_bit_mask()
+            if relay.is_auto_mode():
+                bit_state[0] &= ~relay_bit_mask
             if relay.is_on():
                 bit_state[1] |= relay_bit_mask
-            else:
-                bit_state[0] &= ~relay_bit_mask
         return bit_state
```

### Comparing `proconip-0.0.2/tests/helper.py` & `proconip-1.0.0/tests/helper.py`

 * *Files identical despite different names*

### Comparing `proconip-0.0.2/tests/test_definitions.py` & `proconip-1.0.0/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `proconip-0.0.2/.gitignore` & `proconip-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `proconip-0.0.2/LICENSE` & `proconip-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proconip-0.0.2/README.md` & `proconip-1.0.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -48,25 +48,45 @@
 
 ## Usage
 
 ```python
 import asyncio
 import aiohttp
 from proconip.definitions import ConfigObject
-from proconip.api import GetState
+from proconip.api import GetState, RelaySwitch
 
 
 async def testrun():
     client_session = aiohttp.ClientSession()
     config = ConfigObject("http://192.168.2.3", "admin", "admin")
-    controller = GetState(client_session, config)
-    data = await controller.structured()
-    print(data.redox_electrode.display_value)
-    print(data.ph_electrode.display_value)
-    print(data.temperature_objects[0].display_value)
+    get_state = GetState(client_session, config)
+    data = await get_state.structured()
+    print(f"Redox (Chlor): {data.redox_electrode.display_value}")
+    print(f"pH: {data.ph_electrode.display_value}")
+    for relay in (relay for relay in data.relays() if relay.name != "n.a."):
+        print(f"{relay.name}: {relay.display_value}")
+    for temp in (temp for temp in data.temperature_objects if temp.name != "n.a."):
+        print(f"{temp.name}: {temp.display_value}")
+    
+    relay_switch = RelaySwitch(client_session, config)
+    print(f"Relay no. 2: {data.get_relay(1).display_value}")
+    print(f"Relay no. 3: {data.get_relay(2).display_value}")
+    await relay_switch.set_auto_mode(data, 1)
+    data = await get_state.structured()
+    print(f"Relay no. 2: {data.get_relay(1).display_value}")
+    await relay_switch.set_on(data, 2)
+    data = await get_state.structured()
+    print(f"Relay no. 3: {data.get_relay(2).display_value}")
+    await relay_switch.set_off(data, 1)
+    data = await get_state.structured()
+    print(f"Relay no. 2: {data.get_relay(1).display_value}")
+    await relay_switch.set_off(data, 2)
+    data = await get_state.structured()
+    print(f"Relay no. 3: {data.get_relay(2).display_value}")
+    
     await client_session.close()
 
 
 asyncio.run(testrun())
 
 ```
```

### Comparing `proconip-0.0.2/pyproject.toml` & `proconip-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "proconip"
-version = "0.0.2"
+version = "1.0.0"
 authors = [
   { name="Yannic Labonte", email="yannic.labonte@gmail.com" },
 ]
 description = "Library for basic interaction with the Procon.IP pool controller unit."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `proconip-0.0.2/PKG-INFO` & `proconip-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proconip
-Version: 0.0.2
+Version: 1.0.0
 Summary: Library for basic interaction with the Procon.IP pool controller unit.
 Project-URL: Homepage, https://github.com/ylabonte/proconip-pypi
 Project-URL: Bug Tracker, https://github.com/ylabonte/proconip-pypi/issues
 Author-email: Yannic Labonte <yannic.labonte@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -62,25 +62,45 @@
 
 ## Usage
 
 ```python
 import asyncio
 import aiohttp
 from proconip.definitions import ConfigObject
-from proconip.api import GetState
+from proconip.api import GetState, RelaySwitch
 
 
 async def testrun():
     client_session = aiohttp.ClientSession()
     config = ConfigObject("http://192.168.2.3", "admin", "admin")
-    controller = GetState(client_session, config)
-    data = await controller.structured()
-    print(data.redox_electrode.display_value)
-    print(data.ph_electrode.display_value)
-    print(data.temperature_objects[0].display_value)
+    get_state = GetState(client_session, config)
+    data = await get_state.structured()
+    print(f"Redox (Chlor): {data.redox_electrode.display_value}")
+    print(f"pH: {data.ph_electrode.display_value}")
+    for relay in (relay for relay in data.relays() if relay.name != "n.a."):
+        print(f"{relay.name}: {relay.display_value}")
+    for temp in (temp for temp in data.temperature_objects if temp.name != "n.a."):
+        print(f"{temp.name}: {temp.display_value}")
+    
+    relay_switch = RelaySwitch(client_session, config)
+    print(f"Relay no. 2: {data.get_relay(1).display_value}")
+    print(f"Relay no. 3: {data.get_relay(2).display_value}")
+    await relay_switch.set_auto_mode(data, 1)
+    data = await get_state.structured()
+    print(f"Relay no. 2: {data.get_relay(1).display_value}")
+    await relay_switch.set_on(data, 2)
+    data = await get_state.structured()
+    print(f"Relay no. 3: {data.get_relay(2).display_value}")
+    await relay_switch.set_off(data, 1)
+    data = await get_state.structured()
+    print(f"Relay no. 2: {data.get_relay(1).display_value}")
+    await relay_switch.set_off(data, 2)
+    data = await get_state.structured()
+    print(f"Relay no. 3: {data.get_relay(2).display_value}")
+    
     await client_session.close()
 
 
 asyncio.run(testrun())
 
 ```
```

