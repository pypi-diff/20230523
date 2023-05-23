# Comparing `tmp/aioairzone-cloud-0.1.1.tar.gz` & `tmp/aioairzone-cloud-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-cloud-0.1.1.tar", last modified: Mon May 22 17:53:03 2023, max compression
+gzip compressed data, was "aioairzone-cloud-0.1.2.tar", last modified: Tue May 23 16:28:14 2023, max compression
```

## Comparing `aioairzone-cloud-0.1.1.tar` & `aioairzone-cloud-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-22 17:53:03.136175 aioairzone-cloud-0.1.1/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.1/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.1/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-22 17:53:03.136175 aioairzone-cloud-0.1.1/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2023-05-22 17:43:05.000000 aioairzone-cloud-0.1.1/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-22 17:53:03.132175 aioairzone-cloud-0.1.1/aioairzone_cloud/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    16731 2023-05-22 17:50:13.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/cloudapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2022-04-06 15:45:16.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     6167 2023-05-22 13:41:38.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3040 2023-05-21 08:34:57.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/device.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-21 08:34:57.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1184 2023-05-19 11:19:38.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/installation.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-05-22 07:54:27.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/py.typed
--rw-r--r--   0 noltari   (1000) noltari   (1000)      401 2022-04-06 19:37:08.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/system.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3791 2023-05-19 11:19:38.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/webserver.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    18130 2023-05-21 08:34:57.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/zone.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-22 17:53:03.136175 aioairzone-cloud-0.1.1/aioairzone_cloud.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-22 17:53:03.000000 aioairzone-cloud-0.1.1/aioairzone_cloud.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      619 2023-05-22 17:53:03.000000 aioairzone-cloud-0.1.1/aioairzone_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-22 17:53:03.000000 aioairzone-cloud-0.1.1/aioairzone_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-22 17:53:02.000000 aioairzone-cloud-0.1.1/aioairzone_cloud.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-22 17:53:03.000000 aioairzone-cloud-0.1.1/aioairzone_cloud.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-22 17:53:03.000000 aioairzone-cloud-0.1.1/aioairzone_cloud.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1029 2023-05-22 17:51:42.000000 aioairzone-cloud-0.1.1/pyproject.toml
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.1/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-22 17:53:03.136175 aioairzone-cloud-0.1.1/setup.cfg
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-23 16:28:14.963386 aioairzone-cloud-0.1.2/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.2/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.2/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-23 16:28:14.963386 aioairzone-cloud-0.1.2/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2023-05-22 17:43:05.000000 aioairzone-cloud-0.1.2/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-23 16:28:14.963386 aioairzone-cloud-0.1.2/aioairzone_cloud/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    16766 2023-05-23 16:26:50.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/cloudapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1527 2023-05-23 16:19:08.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     6167 2023-05-23 06:40:31.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3040 2023-05-23 16:26:50.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/device.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-21 08:34:57.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1184 2023-05-19 11:19:38.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/installation.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-05-22 07:54:27.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/py.typed
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      401 2023-05-23 16:26:50.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/system.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3791 2023-05-19 11:19:38.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/webserver.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    18130 2023-05-23 16:26:50.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/zone.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-23 16:28:14.963386 aioairzone-cloud-0.1.2/aioairzone_cloud.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-23 16:28:14.000000 aioairzone-cloud-0.1.2/aioairzone_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      619 2023-05-23 16:28:14.000000 aioairzone-cloud-0.1.2/aioairzone_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-23 16:28:14.000000 aioairzone-cloud-0.1.2/aioairzone_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-23 16:28:14.000000 aioairzone-cloud-0.1.2/aioairzone_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-23 16:28:14.000000 aioairzone-cloud-0.1.2/aioairzone_cloud.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-23 16:28:14.000000 aioairzone-cloud-0.1.2/aioairzone_cloud.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1029 2023-05-23 16:27:25.000000 aioairzone-cloud-0.1.2/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.2/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-23 16:28:14.963386 aioairzone-cloud-0.1.2/setup.cfg
```

### Comparing `aioairzone-cloud-0.1.1/LICENSE` & `aioairzone-cloud-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.1/PKG-INFO` & `aioairzone-cloud-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.1.1/README.md` & `aioairzone-cloud-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.1/aioairzone_cloud/cloudapi.py` & `aioairzone-cloud-0.1.2/aioairzone_cloud/cloudapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,29 +108,29 @@
                 f"{API_URL}/{path}",
                 headers=headers,
                 json=json,
                 raise_for_status=True,
                 timeout=HTTP_CALL_TIMEOUT,
             )
         except ClientConnectorError as err:
-            raise AirzoneCloudError from err
+            raise AirzoneCloudError(err) from err
         except ClientResponseError as err:
             if path.endswith(API_AUTH_LOGIN):
-                raise LoginError from err
+                raise LoginError(err) from err
             if path.endswith(API_AUTH_REFRESH_TOKEN):
-                raise TokenRefreshError from err
+                raise TokenRefreshError(err) from err
 
             if err.status == 400:
-                raise APIError from err
+                raise APIError(err) from err
             if err.status == 401:
-                raise AuthError from err
+                raise AuthError(err) from err
             if err.status == 429:
-                raise TooManyRequests from err
+                raise TooManyRequests(err) from err
 
-            raise AirzoneCloudError from err
+            raise AirzoneCloudError(err) from err
 
         resp_json = await resp.json(content_type=None)
         _LOGGER.debug("aiohttp response: %s", resp_json)
 
         return cast(dict[str, Any], resp_json)
 
     async def api_get_device_config(self, device: Device) -> dict[str, Any]:
```

### Comparing `aioairzone-cloud-0.1.1/aioairzone_cloud/common.py` & `aioairzone-cloud-0.1.2/aioairzone_cloud/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Airzone Cloud API common code."""
 from __future__ import annotations
 
 from dataclasses import dataclass
-from enum import Enum
+from enum import IntEnum
 
 
 @dataclass
 class ConnectionOptions:
     """Airzone Cloud options for connection."""
 
     username: str
     password: str
 
 
-class OperationMode(int, Enum):
+class OperationMode(IntEnum):
     """Airzone Cloud operation modes."""
 
     STOP = 0
     AUTO = 1
     COOLING = 2
     HEATING = 3
     VENTILATION = 4
@@ -58,12 +58,12 @@
         return self.value in [self.STOP]
 
     def is_vent(self) -> bool:
         """Return if mode is Ventilation."""
         return self.value in [self.VENTILATION]
 
 
-class TemperatureUnit(int, Enum):
+class TemperatureUnit(IntEnum):
     """Airzone Cloud temperature units."""
 
     CELSIUS = 0
     FAHRENHEIT = 1
```

### Comparing `aioairzone-cloud-0.1.1/aioairzone_cloud/const.py` & `aioairzone-cloud-0.1.2/aioairzone_cloud/const.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.1/aioairzone_cloud/device.py` & `aioairzone-cloud-0.1.2/aioairzone_cloud/device.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.1/aioairzone_cloud/exceptions.py` & `aioairzone-cloud-0.1.2/aioairzone_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.1/aioairzone_cloud/installation.py` & `aioairzone-cloud-0.1.2/aioairzone_cloud/installation.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.1/aioairzone_cloud/webserver.py` & `aioairzone-cloud-0.1.2/aioairzone_cloud/webserver.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.1/aioairzone_cloud/zone.py` & `aioairzone-cloud-0.1.2/aioairzone_cloud/zone.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.1/aioairzone_cloud.egg-info/PKG-INFO` & `aioairzone-cloud-0.1.2/aioairzone_cloud.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.1.1/aioairzone_cloud.egg-info/SOURCES.txt` & `aioairzone-cloud-0.1.2/aioairzone_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.1/pyproject.toml` & `aioairzone-cloud-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aioairzone-cloud"
-version = "0.1.1"
+version = "0.1.2"
 description = "Library to control Airzone Cloud devices"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "Apache-2.0"}
 keywords = ["airzone", "cloud", "hvac", "home"] 
 authors = [
   {name = "Álvaro Fernández Rojas", email = "noltari@gmail.com" }
```

