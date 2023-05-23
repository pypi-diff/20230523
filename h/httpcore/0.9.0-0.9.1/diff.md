# Comparing `tmp/httpcore-0.9.0.tar.gz` & `tmp/httpcore-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/httpcore-0.9.0.tar", last modified: Thu May 21 11:34:03 2020, max compression
+gzip compressed data, was "dist/httpcore-0.9.1.tar", last modified: Wed May 27 14:57:28 2020, max compression
```

## Comparing `httpcore-0.9.0.tar` & `httpcore-0.9.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-21 11:34:03.000000 httpcore-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (116)     1331 2020-05-21 11:33:23.000000 httpcore-0.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (116)     1518 2020-05-21 11:33:23.000000 httpcore-0.9.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (116)       84 2020-05-21 11:33:23.000000 httpcore-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     5289 2020-05-21 11:34:03.000000 httpcore-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1990 2020-05-21 11:33:23.000000 httpcore-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-21 11:34:03.000000 httpcore-0.9.0/httpcore/
--rw-r--r--   0 runner    (1001) docker     (116)      986 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-21 11:34:03.000000 httpcore-0.9.0/httpcore/_async/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3849 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_async/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     4744 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_async/connection.py
--rw-r--r--   0 runner    (1001) docker     (116)    11305 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_async/connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (116)     6100 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_async/http11.py
--rw-r--r--   0 runner    (1001) docker     (116)    14247 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_async/http2.py
--rw-r--r--   0 runner    (1001) docker     (116)     8896 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_async/http_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-21 11:34:03.000000 httpcore-0.9.0/httpcore/_backends/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8639 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_backends/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (116)     1584 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_backends/auto.py
--rw-r--r--   0 runner    (1001) docker     (116)     2580 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_backends/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     4596 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_backends/sync.py
--rw-r--r--   0 runner    (1001) docker     (116)     5493 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_backends/trio.py
--rw-r--r--   0 runner    (1001) docker     (116)      945 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-21 11:34:03.000000 httpcore-0.9.0/httpcore/_sync/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3745 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_sync/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     4678 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_sync/connection.py
--rw-r--r--   0 runner    (1001) docker     (116)    11078 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_sync/connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (116)     5930 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_sync/http11.py
--rw-r--r--   0 runner    (1001) docker     (116)    13934 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_sync/http2.py
--rw-r--r--   0 runner    (1001) docker     (116)     8792 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_sync/http_proxy.py
--rw-r--r--   0 runner    (1001) docker     (116)      813 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_threadlock.py
--rw-r--r--   0 runner    (1001) docker     (116)      299 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_types.py
--rw-r--r--   0 runner    (1001) docker     (116)     1802 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-21 11:33:23.000000 httpcore-0.9.0/httpcore/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-21 11:34:03.000000 httpcore-0.9.0/httpcore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5289 2020-05-21 11:34:03.000000 httpcore-0.9.0/httpcore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      937 2020-05-21 11:34:03.000000 httpcore-0.9.0/httpcore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-21 11:34:03.000000 httpcore-0.9.0/httpcore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-21 11:34:01.000000 httpcore-0.9.0/httpcore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       36 2020-05-21 11:34:03.000000 httpcore-0.9.0/httpcore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       59 2020-05-21 11:34:03.000000 httpcore-0.9.0/httpcore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      728 2020-05-21 11:34:03.000000 httpcore-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2133 2020-05-21 11:33:23.000000 httpcore-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-27 14:57:28.000000 httpcore-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (116)     1520 2020-05-27 14:56:58.000000 httpcore-0.9.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1518 2020-05-27 14:56:58.000000 httpcore-0.9.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (116)       84 2020-05-27 14:56:58.000000 httpcore-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     5534 2020-05-27 14:57:28.000000 httpcore-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1990 2020-05-27 14:56:58.000000 httpcore-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-27 14:57:28.000000 httpcore-0.9.1/httpcore/
+-rw-r--r--   0 runner    (1001) docker     (116)      986 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-27 14:57:28.000000 httpcore-0.9.1/httpcore/_async/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3849 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_async/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4910 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_async/connection.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11305 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_async/connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6100 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_async/http11.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14247 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_async/http2.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8896 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_async/http_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-27 14:57:28.000000 httpcore-0.9.1/httpcore/_backends/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8639 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_backends/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1584 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_backends/auto.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2580 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4544 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_backends/sync.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5493 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_backends/trio.py
+-rw-r--r--   0 runner    (1001) docker     (116)      945 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-27 14:57:28.000000 httpcore-0.9.1/httpcore/_sync/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3745 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_sync/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4824 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_sync/connection.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11078 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_sync/connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5930 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_sync/http11.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13934 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_sync/http2.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8792 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_sync/http_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (116)      813 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_threadlock.py
+-rw-r--r--   0 runner    (1001) docker     (116)      299 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_types.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1803 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-27 14:56:58.000000 httpcore-0.9.1/httpcore/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-27 14:57:28.000000 httpcore-0.9.1/httpcore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     5534 2020-05-27 14:57:28.000000 httpcore-0.9.1/httpcore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      937 2020-05-27 14:57:28.000000 httpcore-0.9.1/httpcore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-27 14:57:28.000000 httpcore-0.9.1/httpcore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-27 14:57:26.000000 httpcore-0.9.1/httpcore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       36 2020-05-27 14:57:28.000000 httpcore-0.9.1/httpcore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       59 2020-05-27 14:57:28.000000 httpcore-0.9.1/httpcore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      728 2020-05-27 14:57:28.000000 httpcore-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     2133 2020-05-27 14:56:58.000000 httpcore-0.9.1/setup.py
```

### Comparing `httpcore-0.9.0/CHANGELOG.md` & `httpcore-0.9.1/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
+## 0.9.1 (May 27th, 2020)
+
+### Fixed
+
+- Proper host resolution for sync case, including IPv6 support. (Pull #97)
+- Close outstanding connections when connection pool is closed. (Pull #98)
+
 ## 0.9.0 (May 21th, 2020)
 
 ### Changed
 
 - URL port becomes an `Optional[int]` instead of `int`. (Pull #92)
 
 ### Fixed
```

### Comparing `httpcore-0.9.0/LICENSE.md` & `httpcore-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `httpcore-0.9.0/PKG-INFO` & `httpcore-0.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpcore
-Version: 0.9.0
+Version: 0.9.1
 Summary: A minimal low-level HTTP client.
 Home-page: https://github.com/encode/httpcore
 Author: Tom Christie
 Author-email: tom@tomchristie.com
 License: BSD
 Project-URL: Documentation, https://www.encode.io/httpcore
 Project-URL: Source, https://github.com/encode/httpcore
@@ -68,14 +68,21 @@
         
         # Changelog
         
         All notable changes to this project will be documented in this file.
         
         The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
         
+        ## 0.9.1 (May 27th, 2020)
+        
+        ### Fixed
+        
+        - Proper host resolution for sync case, including IPv6 support. (Pull #97)
+        - Close outstanding connections when connection pool is closed. (Pull #98)
+        
         ## 0.9.0 (May 21th, 2020)
         
         ### Changed
         
         - URL port becomes an `Optional[int]` instead of `int`. (Pull #92)
         
         ### Fixed
```

### Comparing `httpcore-0.9.0/README.md` & `httpcore-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `httpcore-0.9.0/httpcore/__init__.py` & `httpcore-0.9.1/httpcore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,8 +35,8 @@
     "WriteTimeout",
     "NetworkError",
     "ConnectError",
     "ReadError",
     "WriteError",
     "CloseError",
 ]
-__version__ = "0.9.0"
+__version__ = "0.9.1"
```

### Comparing `httpcore-0.9.0/httpcore/_async/base.py` & `httpcore-0.9.1/httpcore/_async/base.py`

 * *Files identical despite different names*

### Comparing `httpcore-0.9.0/httpcore/_async/connection.py` & `httpcore-0.9.1/httpcore/_async/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,7 +122,12 @@
 
     async def start_tls(self, hostname: bytes, timeout: TimeoutDict = None) -> None:
         if self.connection is not None:
             logger.trace("start_tls hostname=%r timeout=%r", hostname, timeout)
             await self.connection.start_tls(hostname, timeout)
             logger.trace("start_tls complete hostname=%r timeout=%r", hostname, timeout)
             self.socket = self.connection.socket
+
+    async def aclose(self) -> None:
+        async with self.request_lock:
+            if self.connection is not None:
+                await self.connection.aclose()
```

### Comparing `httpcore-0.9.0/httpcore/_async/connection_pool.py` & `httpcore-0.9.1/httpcore/_async/connection_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         self,
         method: bytes,
         url: URL,
         headers: Headers = None,
         stream: AsyncByteStream = None,
         timeout: TimeoutDict = None,
     ) -> Tuple[bytes, int, bytes, Headers, AsyncByteStream]:
-        assert url[0] in (b'http', b'https')
+        assert url[0] in (b"http", b"https")
         origin = url_to_origin(url)
 
         if self._keepalive_expiry is not None:
             await self._keepalive_sweep()
 
         connection: Optional[AsyncHTTPConnection] = None
         while connection is None:
```

### Comparing `httpcore-0.9.0/httpcore/_async/http11.py` & `httpcore-0.9.1/httpcore/_async/http11.py`

 * *Files identical despite different names*

### Comparing `httpcore-0.9.0/httpcore/_async/http2.py` & `httpcore-0.9.1/httpcore/_async/http2.py`

 * *Files identical despite different names*

### Comparing `httpcore-0.9.0/httpcore/_async/http_proxy.py` & `httpcore-0.9.1/httpcore/_async/http_proxy.py`

 * *Files identical despite different names*

### Comparing `httpcore-0.9.0/httpcore/_backends/asyncio.py` & `httpcore-0.9.1/httpcore/_backends/asyncio.py`

 * *Files identical despite different names*

### Comparing `httpcore-0.9.0/httpcore/_backends/auto.py` & `httpcore-0.9.1/httpcore/_backends/auto.py`

 * *Files identical despite different names*

### Comparing `httpcore-0.9.0/httpcore/_backends/base.py` & `httpcore-0.9.1/httpcore/_backends/base.py`

 * *Files identical despite different names*

### Comparing `httpcore-0.9.0/httpcore/_backends/sync.py` & `httpcore-0.9.1/httpcore/_backends/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,21 +122,20 @@
     def open_tcp_stream(
         self,
         hostname: bytes,
         port: int,
         ssl_context: Optional[SSLContext],
         timeout: TimeoutDict,
     ) -> SyncSocketStream:
+        address = (hostname.decode("ascii"), port)
         connect_timeout = timeout.get("connect")
         exc_map = {socket.timeout: ConnectTimeout, socket.error: ConnectError}
 
         with map_exceptions(exc_map):
-            sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-            sock.settimeout(connect_timeout)
-            sock.connect((hostname.decode("ascii"), port))
+            sock = socket.create_connection(address, connect_timeout)
             if ssl_context is not None:
                 sock = ssl_context.wrap_socket(
                     sock, server_hostname=hostname.decode("ascii")
                 )
             return SyncSocketStream(sock=sock)
 
     def create_lock(self) -> SyncLock:
```

### Comparing `httpcore-0.9.0/httpcore/_backends/trio.py` & `httpcore-0.9.1/httpcore/_backends/trio.py`

 * *Files identical despite different names*

### Comparing `httpcore-0.9.0/httpcore/_exceptions.py` & `httpcore-0.9.1/httpcore/_exceptions.py`

 * *Files identical despite different names*

### Comparing `httpcore-0.9.0/httpcore/_sync/base.py` & `httpcore-0.9.1/httpcore/_sync/base.py`

 * *Files identical despite different names*

### Comparing `httpcore-0.9.0/httpcore/_sync/connection.py` & `httpcore-0.9.1/httpcore/_sync/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,7 +122,12 @@
 
     def start_tls(self, hostname: bytes, timeout: TimeoutDict = None) -> None:
         if self.connection is not None:
             logger.trace("start_tls hostname=%r timeout=%r", hostname, timeout)
             self.connection.start_tls(hostname, timeout)
             logger.trace("start_tls complete hostname=%r timeout=%r", hostname, timeout)
             self.socket = self.connection.socket
+
+    def close(self) -> None:
+        with self.request_lock:
+            if self.connection is not None:
+                self.connection.close()
```

### Comparing `httpcore-0.9.0/httpcore/_sync/connection_pool.py` & `httpcore-0.9.1/httpcore/_sync/connection_pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         self,
         method: bytes,
         url: URL,
         headers: Headers = None,
         stream: SyncByteStream = None,
         timeout: TimeoutDict = None,
     ) -> Tuple[bytes, int, bytes, Headers, SyncByteStream]:
-        assert url[0] in (b'http', b'https')
+        assert url[0] in (b"http", b"https")
         origin = url_to_origin(url)
 
         if self._keepalive_expiry is not None:
             self._keepalive_sweep()
 
         connection: Optional[SyncHTTPConnection] = None
         while connection is None:
```

### Comparing `httpcore-0.9.0/httpcore/_sync/http11.py` & `httpcore-0.9.1/httpcore/_sync/http11.py`

 * *Files identical despite different names*

### Comparing `httpcore-0.9.0/httpcore/_sync/http2.py` & `httpcore-0.9.1/httpcore/_sync/http2.py`

 * *Files identical despite different names*

### Comparing `httpcore-0.9.0/httpcore/_sync/http_proxy.py` & `httpcore-0.9.1/httpcore/_sync/http_proxy.py`

 * *Files identical despite different names*

### Comparing `httpcore-0.9.0/httpcore/_threadlock.py` & `httpcore-0.9.1/httpcore/_threadlock.py`

 * *Files identical despite different names*

### Comparing `httpcore-0.9.0/httpcore/_utils.py` & `httpcore-0.9.1/httpcore/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import os
 import sys
 import typing
+
 from ._types import URL, Origin
 
 _LOGGER_INITIALIZED = False
 TRACE_LOG_LEVEL = 5
 
 
 class Logger(logging.Logger):
@@ -48,10 +49,10 @@
     logger.trace = trace  # type: ignore
 
     return typing.cast(Logger, logger)
 
 
 def url_to_origin(url: URL) -> Origin:
     scheme, host, explicit_port = url[:3]
-    default_port = {b'http': 80, b'https': 443}[scheme]
+    default_port = {b"http": 80, b"https": 443}[scheme]
     port = default_port if explicit_port is None else explicit_port
     return scheme, host, port
```

### Comparing `httpcore-0.9.0/httpcore.egg-info/PKG-INFO` & `httpcore-0.9.1/httpcore.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpcore
-Version: 0.9.0
+Version: 0.9.1
 Summary: A minimal low-level HTTP client.
 Home-page: https://github.com/encode/httpcore
 Author: Tom Christie
 Author-email: tom@tomchristie.com
 License: BSD
 Project-URL: Documentation, https://www.encode.io/httpcore
 Project-URL: Source, https://github.com/encode/httpcore
@@ -68,14 +68,21 @@
         
         # Changelog
         
         All notable changes to this project will be documented in this file.
         
         The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
         
+        ## 0.9.1 (May 27th, 2020)
+        
+        ### Fixed
+        
+        - Proper host resolution for sync case, including IPv6 support. (Pull #97)
+        - Close outstanding connections when connection pool is closed. (Pull #98)
+        
         ## 0.9.0 (May 21th, 2020)
         
         ### Changed
         
         - URL port becomes an `Optional[int]` instead of `int`. (Pull #92)
         
         ### Fixed
```

### Comparing `httpcore-0.9.0/httpcore.egg-info/SOURCES.txt` & `httpcore-0.9.1/httpcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `httpcore-0.9.0/setup.cfg` & `httpcore-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `httpcore-0.9.0/setup.py` & `httpcore-0.9.1/setup.py`

 * *Files identical despite different names*

