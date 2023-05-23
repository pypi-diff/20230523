# Comparing `tmp/curl_cffi-0.5.5.tar.gz` & `tmp/curl_cffi-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curl_cffi-0.5.5.tar", last modified: Sun Apr 16 03:39:40 2023, max compression
+gzip compressed data, was "curl_cffi-0.5.6.tar", last modified: Tue May 23 08:48:07 2023, max compression
```

## Comparing `curl_cffi-0.5.5.tar` & `curl_cffi-0.5.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:39:40.483289 curl_cffi-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-16 03:39:32.000000 curl_cffi-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-16 03:39:32.000000 curl_cffi-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-04-16 03:39:40.483289 curl_cffi-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-16 03:39:32.000000 curl_cffi-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:39:40.483289 curl_cffi-0.5.5/curl_cffi/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-16 03:39:32.000000 curl_cffi-0.5.5/curl_cffi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-16 03:39:32.000000 curl_cffi-0.5.5/curl_cffi/aio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-16 03:39:32.000000 curl_cffi-0.5.5/curl_cffi/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    12654 2023-04-16 03:39:32.000000 curl_cffi-0.5.5/curl_cffi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-16 03:39:32.000000 curl_cffi-0.5.5/curl_cffi/curl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:39:40.483289 curl_cffi-0.5.5/curl_cffi/ffi/
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-16 03:39:32.000000 curl_cffi-0.5.5/curl_cffi/ffi/cdef.c
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-16 03:39:32.000000 curl_cffi-0.5.5/curl_cffi/ffi/shim.c
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-16 03:39:32.000000 curl_cffi-0.5.5/curl_cffi/ffi/shim.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:39:40.483289 curl_cffi-0.5.5/curl_cffi/requests/
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-16 03:39:32.000000 curl_cffi-0.5.5/curl_cffi/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-04-16 03:39:32.000000 curl_cffi-0.5.5/curl_cffi/requests/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-16 03:39:32.000000 curl_cffi-0.5.5/curl_cffi/requests/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-04-16 03:39:32.000000 curl_cffi-0.5.5/curl_cffi/requests/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16996 2023-04-16 03:39:32.000000 curl_cffi-0.5.5/curl_cffi/requests/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:39:40.483289 curl_cffi-0.5.5/curl_cffi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-04-16 03:39:40.000000 curl_cffi-0.5.5/curl_cffi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-16 03:39:40.000000 curl_cffi-0.5.5/curl_cffi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 03:39:40.000000 curl_cffi-0.5.5/curl_cffi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-16 03:39:40.000000 curl_cffi-0.5.5/curl_cffi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-16 03:39:40.000000 curl_cffi-0.5.5/curl_cffi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-16 03:39:32.000000 curl_cffi-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 03:39:40.483289 curl_cffi-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-16 03:39:32.000000 curl_cffi-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:48:07.467091 curl_cffi-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-05-23 08:48:07.467091 curl_cffi-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:48:07.463091 curl_cffi-0.5.6/curl_cffi/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12654 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/curl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:48:07.467091 curl_cffi-0.5.6/curl_cffi/ffi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/ffi/cdef.c
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/ffi/shim.c
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/ffi/shim.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:48:07.467091 curl_cffi-0.5.6/curl_cffi/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/requests/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/requests/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/requests/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/curl_cffi/requests/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:48:07.467091 curl_cffi-0.5.6/curl_cffi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-05-23 08:48:07.000000 curl_cffi-0.5.6/curl_cffi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-23 08:48:07.000000 curl_cffi-0.5.6/curl_cffi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:48:07.000000 curl_cffi-0.5.6/curl_cffi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-23 08:48:07.000000 curl_cffi-0.5.6/curl_cffi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 08:48:07.000000 curl_cffi-0.5.6/curl_cffi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 08:48:07.467091 curl_cffi-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-23 08:47:59.000000 curl_cffi-0.5.6/setup.py
```

### Comparing `curl_cffi-0.5.5/LICENSE` & `curl_cffi-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.5/PKG-INFO` & `curl_cffi-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curl_cffi
-Version: 0.5.5
+Version: 0.5.6
 Summary: libcurl ffi bindings for Python, with impersonation support
 Author-email: Yifei Kong <kong@yifei.me>
 License: MIT License
         
         Copyright (c) 2018 multippt
         Copyright (c) 2022 Yifei Kong
```

### Comparing `curl_cffi-0.5.5/README.md` & `curl_cffi-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.5/curl_cffi/aio.py` & `curl_cffi-0.5.6/curl_cffi/aio.py`

 * *Files 10% similar despite different names*

```diff
@@ -87,15 +87,16 @@
         self.setopt(CurlMOpt.SOCKETDATA, self._self_handle)
         self.setopt(CurlMOpt.TIMERDATA, self._self_handle)
 
     def close(self):
         self._checker.cancel()
         for curl, future in self._curl2future.items():
             lib.curl_multi_remove_handle(self._curlm, curl._curl)
-            future.set_result(None)
+            if not future.done() and not future.cancelled():
+                future.set_result(None)
         lib.curl_multi_cleanup(self._curlm)
         self._curlm = None
         for sockfd in  self._sockfds:
             self.loop.remove_reader(sockfd)
             self.loop.remove_writer(sockfd)
         for timer in self._timers:
             timer.cancel()
@@ -155,15 +156,17 @@
 
     def cancel_handle(self, curl: Curl):
         future = self._pop_future(curl)
         future.cancel()
 
     def set_result(self, curl: Curl):
         future = self._pop_future(curl)
-        future.set_result(None)
+        if not future.done() and not future.cancelled():
+            future.set_result(None)
 
     def set_exception(self, curl: Curl, exception):
         future = self._pop_future(curl)
-        future.set_exception(exception)
+        if not future.done() and not future.cancelled():
+            future.set_exception(exception)
 
     def setopt(self, option, value):
         return lib.curl_multi_setopt(self._curlm, option, value)
```

### Comparing `curl_cffi-0.5.5/curl_cffi/build.py` & `curl_cffi-0.5.6/curl_cffi/build.py`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.5/curl_cffi/const.py` & `curl_cffi-0.5.6/curl_cffi/const.py`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.5/curl_cffi/curl.py` & `curl_cffi-0.5.6/curl_cffi/curl.py`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.5/curl_cffi/ffi/cdef.c` & `curl_cffi-0.5.6/curl_cffi/ffi/cdef.c`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.5/curl_cffi/ffi/shim.c` & `curl_cffi-0.5.6/curl_cffi/ffi/shim.c`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.5/curl_cffi/requests/__init__.py` & `curl_cffi-0.5.6/curl_cffi/requests/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 from typing import Callable, Dict, Optional, Tuple, Union
 
 from .cookies import Cookies, CookieTypes, Response
 from .errors import RequestsError
 from .headers import Headers, HeaderTypes
 from .session import AsyncSession, BrowserType, Session
 
+# ThreadType = Literal["eventlet", "gevent", None]
+
 
 def request(
     method: str,
     url: str,
     params: Optional[dict] = None,
     data: Optional[Union[Dict[str, str], str, BytesIO, bytes]] = None,
     json: Optional[dict] = None,
@@ -34,16 +36,17 @@
     max_redirects: int = -1,
     proxies: Optional[dict] = None,
     verify: Optional[bool] = None,
     referer: Optional[str] = None,
     accept_encoding: Optional[str] = "gzip, deflate, br",
     content_callback: Optional[Callable] = None,
     impersonate: Optional[Union[str, BrowserType]] = None,
+    thread: Optional[str] = None,
 ) -> Response:
-    with Session() as s:
+    with Session(thread=thread) as s:
         return s.request(
             method,
             url,
             params,
             data,
             json,
             headers,
```

### Comparing `curl_cffi-0.5.5/curl_cffi/requests/cookies.py` & `curl_cffi-0.5.6/curl_cffi/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.5/curl_cffi/requests/headers.py` & `curl_cffi-0.5.6/curl_cffi/requests/headers.py`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.5/curl_cffi/requests/session.py` & `curl_cffi-0.5.6/curl_cffi/requests/session.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 import asyncio
 import re
+import threading
+import warnings
 from enum import Enum
 from functools import partialmethod
 from io import BytesIO
 from json import dumps
 from typing import Callable, Dict, List, Optional, Tuple, Union, cast
 from urllib.parse import ParseResult, parse_qsl, unquote, urlencode, urlparse
 
 from .. import AsyncCurl, Curl, CurlError, CurlInfo, CurlOpt
 from .cookies import Cookies, CookieTypes, Request, Response
 from .errors import RequestsError
 from .headers import Headers, HeaderTypes
 
+try:
+    import gevent
+except ImportError:
+    pass
+
+try:
+    import eventlet.tpool
+except ImportError:
+    pass
+
 
 class BrowserType(str, Enum):
     edge99 = "edge99"
     edge101 = "edge101"
     chrome99 = "chrome99"
     chrome100 = "chrome100"
     chrome101 = "chrome101"
@@ -326,18 +338,36 @@
         rsp.elapsed = cast(float, c.getinfo(CurlInfo.TOTAL_TIME))
         rsp.redirect_count = cast(int, c.getinfo(CurlInfo.REDIRECT_COUNT))
         rsp.redirect_url = cast(bytes, c.getinfo(CurlInfo.REDIRECT_URL)).decode()
 
         return rsp
 
 
+# ThreadType = Literal["eventlet", "gevent", None]
+
+
 class Session(BaseSession):
-    def __init__(self, curl: Optional[Curl] = None, **kwargs):
+    def __init__(self, curl: Optional[Curl] = None, thread: Optional[str] = None, **kwargs):
         super().__init__(**kwargs)
-        self.curl = curl if curl is not None else Curl()
+        self._thread = thread
+        self._local = threading.local()
+        if curl:
+            self._is_customized_curl = True
+            self._local.curl = curl
+        else:
+            self._is_customized_curl = False
+            self._local.curl = Curl()
+
+    @property
+    def curl(self):
+        if self._is_customized_curl:
+            warnings.warn("Creating fresh curl in different thread.")
+        if not getattr(self._local, "curl", None):
+            self._local.curl = Curl()
+        return self._local.curl
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         self.close()
 
@@ -384,15 +414,22 @@
             verify,
             referer,
             accept_encoding,
             content_callback,
             impersonate,
         )
         try:
-            c.perform()
+            if self._thread == "eventlet":
+                # see: https://eventlet.net/doc/threading.html
+                eventlet.tpool.execute(c.perform)
+            elif self._thread == "gevent":
+                # see: https://www.gevent.org/api/gevent.threadpool.html
+                gevent.get_hub().threadpool.spawn(c.perform).get()
+            else:
+                c.perform()
         except CurlError as e:
             raise RequestsError(e)
 
         rsp = self._parse_response(c, req, buffer, header_buffer)
         self.curl.reset()
         return rsp
```

### Comparing `curl_cffi-0.5.5/curl_cffi.egg-info/PKG-INFO` & `curl_cffi-0.5.6/curl_cffi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curl-cffi
-Version: 0.5.5
+Version: 0.5.6
 Summary: libcurl ffi bindings for Python, with impersonation support
 Author-email: Yifei Kong <kong@yifei.me>
 License: MIT License
         
         Copyright (c) 2018 multippt
         Copyright (c) 2022 Yifei Kong
```

### Comparing `curl_cffi-0.5.5/curl_cffi.egg-info/SOURCES.txt` & `curl_cffi-0.5.6/curl_cffi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.5/curl_cffi.egg-info/requires.txt` & `curl_cffi-0.5.6/curl_cffi.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.5/pyproject.toml` & `curl_cffi-0.5.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "curl_cffi"
-version = "0.5.5"
+version = "0.5.6"
 authors = [{ name = "Yifei Kong", email = "kong@yifei.me" }]
 description = "libcurl ffi bindings for Python, with impersonation support"
 license = { file = "LICENSE" }
 dependencies = ["cffi>=1.12.0"]
 readme = "README.md"
 requires-python = ">=3.7"
 urls = { "repository" = "https://github.com/yifeikong/curl_cffi" }
```

### Comparing `curl_cffi-0.5.5/setup.py` & `curl_cffi-0.5.6/setup.py`

 * *Files identical despite different names*

