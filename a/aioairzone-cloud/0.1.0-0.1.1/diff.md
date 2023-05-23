# Comparing `tmp/aioairzone-cloud-0.1.0.tar.gz` & `tmp/aioairzone-cloud-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-cloud-0.1.0.tar", last modified: Mon May 22 17:29:23 2023, max compression
+gzip compressed data, was "aioairzone-cloud-0.1.1.tar", last modified: Mon May 22 17:53:03 2023, max compression
```

## Comparing `aioairzone-cloud-0.1.0.tar` & `aioairzone-cloud-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-22 17:29:23.858698 aioairzone-cloud-0.1.0/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.0/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.0/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1102 2023-05-22 17:29:23.858698 aioairzone-cloud-0.1.0/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      320 2023-05-18 08:06:51.000000 aioairzone-cloud-0.1.0/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-22 17:29:23.858698 aioairzone-cloud-0.1.0/aioairzone_cloud/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    16659 2023-05-22 17:23:29.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/cloudapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2022-04-06 15:45:16.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     6167 2023-05-22 13:41:38.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3040 2023-05-21 08:34:57.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/device.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-21 08:34:57.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1184 2023-05-19 11:19:38.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/installation.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-05-22 07:54:27.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/py.typed
--rw-r--r--   0 noltari   (1000) noltari   (1000)      401 2022-04-06 19:37:08.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/system.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3791 2023-05-19 11:19:38.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/webserver.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    18130 2023-05-21 08:34:57.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/zone.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-22 17:29:23.858698 aioairzone-cloud-0.1.0/aioairzone_cloud.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1102 2023-05-22 17:29:23.000000 aioairzone-cloud-0.1.0/aioairzone_cloud.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      619 2023-05-22 17:29:23.000000 aioairzone-cloud-0.1.0/aioairzone_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-22 17:29:23.000000 aioairzone-cloud-0.1.0/aioairzone_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-22 17:29:23.000000 aioairzone-cloud-0.1.0/aioairzone_cloud.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-22 17:29:23.000000 aioairzone-cloud-0.1.0/aioairzone_cloud.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-22 17:29:23.000000 aioairzone-cloud-0.1.0/aioairzone_cloud.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1029 2023-05-22 17:27:48.000000 aioairzone-cloud-0.1.0/pyproject.toml
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.0/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-22 17:29:23.858698 aioairzone-cloud-0.1.0/setup.cfg
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-22 17:53:03.136175 aioairzone-cloud-0.1.1/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.1/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.1/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-22 17:53:03.136175 aioairzone-cloud-0.1.1/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2023-05-22 17:43:05.000000 aioairzone-cloud-0.1.1/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-22 17:53:03.132175 aioairzone-cloud-0.1.1/aioairzone_cloud/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    16731 2023-05-22 17:50:13.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/cloudapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2022-04-06 15:45:16.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     6167 2023-05-22 13:41:38.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3040 2023-05-21 08:34:57.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/device.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-21 08:34:57.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1184 2023-05-19 11:19:38.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/installation.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-05-22 07:54:27.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/py.typed
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      401 2022-04-06 19:37:08.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/system.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3791 2023-05-19 11:19:38.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/webserver.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    18130 2023-05-21 08:34:57.000000 aioairzone-cloud-0.1.1/aioairzone_cloud/zone.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-22 17:53:03.136175 aioairzone-cloud-0.1.1/aioairzone_cloud.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-22 17:53:03.000000 aioairzone-cloud-0.1.1/aioairzone_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      619 2023-05-22 17:53:03.000000 aioairzone-cloud-0.1.1/aioairzone_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-22 17:53:03.000000 aioairzone-cloud-0.1.1/aioairzone_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-22 17:53:02.000000 aioairzone-cloud-0.1.1/aioairzone_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-22 17:53:03.000000 aioairzone-cloud-0.1.1/aioairzone_cloud.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-22 17:53:03.000000 aioairzone-cloud-0.1.1/aioairzone_cloud.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1029 2023-05-22 17:51:42.000000 aioairzone-cloud-0.1.1/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.1/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-22 17:53:03.136175 aioairzone-cloud-0.1.1/setup.cfg
```

### Comparing `aioairzone-cloud-0.1.0/LICENSE` & `aioairzone-cloud-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.0/aioairzone_cloud/cloudapi.py` & `aioairzone-cloud-0.1.1/aioairzone_cloud/cloudapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             RAW_DEVICES_STATUS: {},
             RAW_INSTALLATIONS: {},
             RAW_WEBSERVERS: {},
         }
         self.aiohttp_session = aiohttp_session
         self.installations: list[Installation] = []
         self.options = options
-        self.refresh_time: datetime
+        self.refresh_time: datetime | None = None
         self.refresh_token: str | None = None
         self.systems: list[System] = []
         self.token: str | None = None
         self.webservers: list[WebServer] = []
         self.zones: list[Zone] = []
 
     async def api_request(
@@ -482,15 +482,17 @@
         ]
 
         await asyncio.gather(*tasks)
 
     async def update(self) -> None:
         """Update all Airzone Cloud data."""
 
-        if (datetime.now() - self.refresh_time) > TOKEN_REFRESH_PERIOD:
+        if (self.refresh_time is not None) and (
+            datetime.now() - self.refresh_time
+        ) > TOKEN_REFRESH_PERIOD:
             try:
                 await self.token_refresh()
             except TokenRefreshError:
                 await self.login()
 
         try:
             await self._update()
```

### Comparing `aioairzone-cloud-0.1.0/aioairzone_cloud/common.py` & `aioairzone-cloud-0.1.1/aioairzone_cloud/common.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.0/aioairzone_cloud/const.py` & `aioairzone-cloud-0.1.1/aioairzone_cloud/const.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.0/aioairzone_cloud/device.py` & `aioairzone-cloud-0.1.1/aioairzone_cloud/device.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.0/aioairzone_cloud/exceptions.py` & `aioairzone-cloud-0.1.1/aioairzone_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.0/aioairzone_cloud/installation.py` & `aioairzone-cloud-0.1.1/aioairzone_cloud/installation.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.0/aioairzone_cloud/webserver.py` & `aioairzone-cloud-0.1.1/aioairzone_cloud/webserver.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.0/aioairzone_cloud/zone.py` & `aioairzone-cloud-0.1.1/aioairzone_cloud/zone.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.0/aioairzone_cloud.egg-info/SOURCES.txt` & `aioairzone-cloud-0.1.1/aioairzone_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.0/pyproject.toml` & `aioairzone-cloud-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aioairzone-cloud"
-version = "0.1.0"
+version = "0.1.1"
 description = "Library to control Airzone Cloud devices"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "Apache-2.0"}
 keywords = ["airzone", "cloud", "hvac", "home"] 
 authors = [
   {name = "Álvaro Fernández Rojas", email = "noltari@gmail.com" }
```

