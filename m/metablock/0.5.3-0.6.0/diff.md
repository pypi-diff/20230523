# Comparing `tmp/metablock-0.5.3.tar.gz` & `tmp/metablock-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metablock-0.5.3.tar", max compression
+gzip compressed data, was "metablock-0.6.0.tar", max compression
```

## Comparing `metablock-0.5.3.tar` & `metablock-0.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1482 2023-05-20 10:27:45.002933 metablock-0.5.3/LICENSE
--rw-r--r--   0        0        0      502 2023-05-20 10:27:45.002933 metablock-0.5.3/metablock/__init__.py
--rw-r--r--   0        0        0     4119 2023-05-20 10:27:45.002933 metablock-0.5.3/metablock/client.py
--rw-r--r--   0        0        0     7937 2023-05-20 10:27:45.002933 metablock-0.5.3/metablock/components.py
--rw-r--r--   0        0        0      540 2023-05-20 10:27:45.002933 metablock-0.5.3/metablock/extensions.py
--rw-r--r--   0        0        0     1850 2023-05-20 10:27:45.002933 metablock-0.5.3/metablock/orgs.py
--rw-r--r--   0        0        0        0 2023-05-20 10:27:45.002933 metablock-0.5.3/metablock/py.typed
--rw-r--r--   0        0        0     3029 2023-05-20 10:27:45.006933 metablock-0.5.3/metablock/spaces.py
--rw-r--r--   0        0        0     1350 2023-05-20 10:27:45.006933 metablock-0.5.3/metablock/user.py
--rw-r--r--   0        0        0      531 2023-05-20 10:27:45.006933 metablock-0.5.3/metablock/utils.py
--rw-r--r--   0        0        0      564 2023-05-20 10:27:45.006933 metablock-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     1010 2023-05-20 10:27:45.006933 metablock-0.5.3/readme.md
--rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 metablock-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1482 2023-05-23 08:25:37.198904 metablock-0.6.0/LICENSE
+-rw-r--r--   0        0        0      502 2023-05-23 08:25:37.198904 metablock-0.6.0/metablock/__init__.py
+-rw-r--r--   0        0        0     4004 2023-05-23 08:25:37.198904 metablock-0.6.0/metablock/client.py
+-rw-r--r--   0        0        0     7937 2023-05-23 08:25:37.198904 metablock-0.6.0/metablock/components.py
+-rw-r--r--   0        0        0      540 2023-05-23 08:25:37.198904 metablock-0.6.0/metablock/extensions.py
+-rw-r--r--   0        0        0     1850 2023-05-23 08:25:37.198904 metablock-0.6.0/metablock/orgs.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:25:37.198904 metablock-0.6.0/metablock/py.typed
+-rw-r--r--   0        0        0     3029 2023-05-23 08:25:37.198904 metablock-0.6.0/metablock/spaces.py
+-rw-r--r--   0        0        0     1350 2023-05-23 08:25:37.198904 metablock-0.6.0/metablock/user.py
+-rw-r--r--   0        0        0      531 2023-05-23 08:25:37.198904 metablock-0.6.0/metablock/utils.py
+-rw-r--r--   0        0        0      564 2023-05-23 08:25:37.198904 metablock-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1010 2023-05-23 08:25:37.198904 metablock-0.6.0/readme.md
+-rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 metablock-0.6.0/PKG-INFO
```

### Comparing `metablock-0.5.3/LICENSE` & `metablock-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metablock-0.5.3/metablock/client.py` & `metablock-0.6.0/metablock/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -96,27 +96,28 @@
             except Exception:
                 data = await response.text()
             raise MetablockResponseError(response, data)
         response.raise_for_status()
         data = await response.json()
         return wrap(data) if wrap else data
 
-    async def get_user(self, callback: Callback | None = None) -> User:
-        return await self.get(f"{self.url}/user", callback=callback, wrap=self._user)
+    async def get_user(self, **kw: Any) -> User:
+        kw.setdefault("wrap", self._user)
+        return await self.get(f"{self.url}/user", **kw)
+
+    async def get_space(self, **kw: Any) -> Space:
+        kw.setdefault("wrap", self._space)
+        return await self.get(f"{self.url}/space", **kw)
+
+    async def update_user(self, **kw: Any) -> User:
+        kw.setdefault("wrap", self._user)
+        return await self.patch(f"{self.url}/user", **kw)
 
-    async def get_space(self, callback: Callback | None = None) -> Space:
-        return await self.get(f"{self.url}/space", callback=callback, wrap=self._space)
-
-    async def update_user(self, callback: Callback | None = None, **data: Any) -> User:
-        return await self.patch(
-            f"{self.url}/user", json=data, callback=callback, wrap=self._user
-        )
-
-    async def delete_user(self, callback: Callback | None = None) -> None:
-        return await self.delete(f"{self.url}/user", callback=callback)
+    async def delete_user(self, **kw: Any) -> None:
+        return await self.delete(f"{self.url}/user", **kw)
 
     def get_default_headers(self) -> dict[str, str]:
         headers = self.default_headers.copy()
         if self.auth_key:
             headers[self.auth_key_name] = self.auth_key
         return headers
```

### Comparing `metablock-0.5.3/metablock/components.py` & `metablock-0.6.0/metablock/components.py`

 * *Files identical despite different names*

### Comparing `metablock-0.5.3/metablock/extensions.py` & `metablock-0.6.0/metablock/extensions.py`

 * *Files identical despite different names*

### Comparing `metablock-0.5.3/metablock/orgs.py` & `metablock-0.6.0/metablock/orgs.py`

 * *Files identical despite different names*

### Comparing `metablock-0.5.3/metablock/spaces.py` & `metablock-0.6.0/metablock/spaces.py`

 * *Files identical despite different names*

### Comparing `metablock-0.5.3/metablock/user.py` & `metablock-0.6.0/metablock/user.py`

 * *Files identical despite different names*

### Comparing `metablock-0.5.3/metablock/utils.py` & `metablock-0.6.0/metablock/utils.py`

 * *Files identical despite different names*

### Comparing `metablock-0.5.3/pyproject.toml` & `metablock-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metablock"
-version = "0.5.3"
+version = "0.6.0"
 description = "Metablock cloud python client"
 authors = ["Luca <luca@quantmind.com>"]
 license = "BSD"
 readme = "readme.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `metablock-0.5.3/readme.md` & `metablock-0.6.0/readme.md`

 * *Files identical despite different names*

### Comparing `metablock-0.5.3/PKG-INFO` & `metablock-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metablock
-Version: 0.5.3
+Version: 0.6.0
 Summary: Metablock cloud python client
 License: BSD
 Author: Luca
 Author-email: luca@quantmind.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

