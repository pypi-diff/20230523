# Comparing `tmp/tremolo-0.0.97.tar.gz` & `tmp/tremolo-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tremolo-0.0.97.tar", last modified: Sun May 21 09:14:48 2023, max compression
+gzip compressed data, was "dist/tremolo-0.0.98.tar", last modified: Tue May 23 02:00:57 2023, max compression
```

## Comparing `tremolo-0.0.97.tar` & `tremolo-0.0.98.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-21 09:14:48.000000 tremolo-0.0.97/
--rw-r--r--   0 tux       (1000) users      (100)     1063 2023-05-08 03:43:30.000000 tremolo-0.0.97/LICENSE.txt
--rw-r--r--   0 tux       (1000) users      (100)     4619 2023-05-21 09:14:48.000000 tremolo-0.0.97/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)     4019 2023-05-15 04:15:11.000000 tremolo-0.0.97/README.md
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-21 09:14:48.000000 tremolo-0.0.97/setup.cfg
--rwxr-xr-x   0 tux       (1000) users      (100)      975 2023-05-21 09:08:50.000000 tremolo-0.0.97/setup.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-21 09:14:48.000000 tremolo-0.0.97/tremolo/
--rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)     4465 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/__main__.py
--rw-r--r--   0 tux       (1000) users      (100)     2278 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/asgi_lifespan.py
--rw-r--r--   0 tux       (1000) users      (100)     5666 2023-05-19 13:26:48.000000 tremolo-0.0.97/tremolo/asgi_server.py
--rw-r--r--   0 tux       (1000) users      (100)      542 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/contexts.py
--rw-r--r--   0 tux       (1000) users      (100)      586 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/exceptions.py
--rw-r--r--   0 tux       (1000) users      (100)    10617 2023-05-19 14:03:18.000000 tremolo-0.0.97/tremolo/http_server.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-21 09:14:48.000000 tremolo-0.0.97/tremolo/lib/
--rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/lib/__init__.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-21 09:14:48.000000 tremolo-0.0.97/tremolo/lib/h1parser/
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/lib/h1parser/__init__.py
--rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/lib/h1parser/parse_header.py
--rw-r--r--   0 tux       (1000) users      (100)     1798 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/lib/http_exception.py
--rwxr-xr-x   0 tux       (1000) users      (100)    13962 2023-05-21 09:10:36.000000 tremolo-0.0.97/tremolo/lib/http_protocol.py
--rwxr-xr-x   0 tux       (1000) users      (100)     9281 2023-05-19 23:50:26.000000 tremolo-0.0.97/tremolo/lib/http_request.py
--rwxr-xr-x   0 tux       (1000) users      (100)    11322 2023-05-20 00:56:10.000000 tremolo-0.0.97/tremolo/lib/http_response.py
--rw-r--r--   0 tux       (1000) users      (100)      772 2023-05-19 07:52:08.000000 tremolo-0.0.97/tremolo/lib/object_pool.py
--rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-05-19 02:59:43.000000 tremolo-0.0.97/tremolo/lib/request.py
--rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/lib/response.py
--rwxr-xr-x   0 tux       (1000) users      (100)    15287 2023-05-08 03:43:30.000000 tremolo-0.0.97/tremolo/tremolo.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-21 09:14:48.000000 tremolo-0.0.97/tremolo.egg-info/
--rw-r--r--   0 tux       (1000) users      (100)     4619 2023-05-21 09:14:48.000000 tremolo-0.0.97/tremolo.egg-info/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)      610 2023-05-21 09:14:48.000000 tremolo-0.0.97/tremolo.egg-info/SOURCES.txt
--rw-r--r--   0 tux       (1000) users      (100)        1 2023-05-21 09:14:48.000000 tremolo-0.0.97/tremolo.egg-info/dependency_links.txt
--rw-r--r--   0 tux       (1000) users      (100)        8 2023-05-21 09:14:48.000000 tremolo-0.0.97/tremolo.egg-info/top_level.txt
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-23 02:00:57.000000 tremolo-0.0.98/
+-rw-r--r--   0 tux       (1000) users      (100)     1063 2023-05-08 03:43:30.000000 tremolo-0.0.98/LICENSE.txt
+-rw-r--r--   0 tux       (1000) users      (100)     4619 2023-05-23 02:00:57.000000 tremolo-0.0.98/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)     4019 2023-05-23 01:20:31.000000 tremolo-0.0.98/README.md
+-rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-23 02:00:57.000000 tremolo-0.0.98/setup.cfg
+-rwxr-xr-x   0 tux       (1000) users      (100)      975 2023-05-23 01:14:02.000000 tremolo-0.0.98/setup.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-23 02:00:57.000000 tremolo-0.0.98/tremolo/
+-rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-05-08 03:43:30.000000 tremolo-0.0.98/tremolo/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)     4465 2023-05-08 03:43:30.000000 tremolo-0.0.98/tremolo/__main__.py
+-rw-r--r--   0 tux       (1000) users      (100)     2278 2023-05-08 03:43:30.000000 tremolo-0.0.98/tremolo/asgi_lifespan.py
+-rw-r--r--   0 tux       (1000) users      (100)     5666 2023-05-19 13:26:48.000000 tremolo-0.0.98/tremolo/asgi_server.py
+-rw-r--r--   0 tux       (1000) users      (100)      542 2023-05-08 03:43:30.000000 tremolo-0.0.98/tremolo/contexts.py
+-rw-r--r--   0 tux       (1000) users      (100)      586 2023-05-08 03:43:30.000000 tremolo-0.0.98/tremolo/exceptions.py
+-rw-r--r--   0 tux       (1000) users      (100)    10617 2023-05-19 14:03:18.000000 tremolo-0.0.98/tremolo/http_server.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-23 02:00:57.000000 tremolo-0.0.98/tremolo/lib/
+-rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-08 03:43:30.000000 tremolo-0.0.98/tremolo/lib/__init__.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-23 02:00:57.000000 tremolo-0.0.98/tremolo/lib/h1parser/
+-rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-08 03:43:30.000000 tremolo-0.0.98/tremolo/lib/h1parser/__init__.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-05-08 03:43:30.000000 tremolo-0.0.98/tremolo/lib/h1parser/parse_header.py
+-rw-r--r--   0 tux       (1000) users      (100)     1798 2023-05-08 03:43:30.000000 tremolo-0.0.98/tremolo/lib/http_exception.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    14220 2023-05-23 01:43:26.000000 tremolo-0.0.98/tremolo/lib/http_protocol.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     9281 2023-05-19 23:50:26.000000 tremolo-0.0.98/tremolo/lib/http_request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    11322 2023-05-20 00:56:10.000000 tremolo-0.0.98/tremolo/lib/http_response.py
+-rw-r--r--   0 tux       (1000) users      (100)      772 2023-05-19 07:52:08.000000 tremolo-0.0.98/tremolo/lib/object_pool.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-05-19 02:59:43.000000 tremolo-0.0.98/tremolo/lib/request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-05-08 03:43:30.000000 tremolo-0.0.98/tremolo/lib/response.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    15287 2023-05-23 01:38:51.000000 tremolo-0.0.98/tremolo/tremolo.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-23 02:00:57.000000 tremolo-0.0.98/tremolo.egg-info/
+-rw-r--r--   0 tux       (1000) users      (100)     4619 2023-05-23 02:00:57.000000 tremolo-0.0.98/tremolo.egg-info/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)      610 2023-05-23 02:00:57.000000 tremolo-0.0.98/tremolo.egg-info/SOURCES.txt
+-rw-r--r--   0 tux       (1000) users      (100)        1 2023-05-23 02:00:57.000000 tremolo-0.0.98/tremolo.egg-info/dependency_links.txt
+-rw-r--r--   0 tux       (1000) users      (100)        8 2023-05-23 02:00:57.000000 tremolo-0.0.98/tremolo.egg-info/top_level.txt
```

### Comparing `tremolo-0.0.97/LICENSE.txt` & `tremolo-0.0.98/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.97/PKG-INFO` & `tremolo-0.0.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.97
+Version: 0.0.98
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -79,15 +79,15 @@
 async def app(scope, receive, send):
     assert scope['type'] == 'http'
 
     await send({
         'type': 'http.response.start',
         'status': 200,
         'headers': [
-            (b'content-type', b'text/plain'),
+            (b'content-type', b'text/plain')
         ]
     })
 
     await send({
         'type': 'http.response.body',
         'body': b'Hello world!'
     })
@@ -116,15 +116,15 @@
 ```
 uvicorn --loop asyncio --http h11 --log-level error example:app
 ```
 
 vs
 
 ```
-python -m tremolo --log-level ERROR example:app
+python3 -m tremolo --log-level ERROR example:app
 ```
 
 You will find that Tremolo is reasonably fast.
 
 What's interesting is that this may become different when [CPython becomes faster](https://devblogs.microsoft.com/python/python-311-faster-cpython-team/),
 or another faster Python implementation comes along.
```

### Comparing `tremolo-0.0.97/README.md` & `tremolo-0.0.98/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 async def app(scope, receive, send):
     assert scope['type'] == 'http'
 
     await send({
         'type': 'http.response.start',
         'status': 200,
         'headers': [
-            (b'content-type', b'text/plain'),
+            (b'content-type', b'text/plain')
         ]
     })
 
     await send({
         'type': 'http.response.body',
         'body': b'Hello world!'
     })
@@ -100,15 +100,15 @@
 ```
 uvicorn --loop asyncio --http h11 --log-level error example:app
 ```
 
 vs
 
 ```
-python -m tremolo --log-level ERROR example:app
+python3 -m tremolo --log-level ERROR example:app
 ```
 
 You will find that Tremolo is reasonably fast.
 
 What's interesting is that this may become different when [CPython becomes faster](https://devblogs.microsoft.com/python/python-311-faster-cpython-team/),
 or another faster Python implementation comes along.
```

### Comparing `tremolo-0.0.97/setup.py` & `tremolo-0.0.98/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tremolo',
     packages=['tremolo'],
     package_data={'': ['lib/*', 'lib/h1parser/*']},
-    version='0.0.97',
+    version='0.0.98',
     license='MIT',
     author='nggit',
     author_email='contact@anggit.com',
     description='Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nggit/tremolo',
```

### Comparing `tremolo-0.0.97/tremolo/__main__.py` & `tremolo-0.0.98/tremolo/__main__.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.97/tremolo/asgi_lifespan.py` & `tremolo-0.0.98/tremolo/asgi_lifespan.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.97/tremolo/asgi_server.py` & `tremolo-0.0.98/tremolo/asgi_server.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.97/tremolo/contexts.py` & `tremolo-0.0.98/tremolo/contexts.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.97/tremolo/exceptions.py` & `tremolo-0.0.98/tremolo/exceptions.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.97/tremolo/http_server.py` & `tremolo-0.0.98/tremolo/http_server.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.97/tremolo/lib/h1parser/parse_header.py` & `tremolo-0.0.98/tremolo/lib/h1parser/parse_header.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.97/tremolo/lib/http_exception.py` & `tremolo-0.0.98/tremolo/lib/http_exception.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.97/tremolo/lib/http_protocol.py` & `tremolo-0.0.98/tremolo/lib/http_protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,18 +62,19 @@
         self._transport = transport
         self._pool = self._options['_pool'].get()
         self._queue = self._pool['queue']
 
         self._data = bytearray()
         self._waiters = {'request': self._loop.create_future()}
 
-        for task in (self._send_data(), self.set_timeout(self._waiters['request'],
-                                                         timeout=self._options['request_timeout'],
-                                                         timeout_cb=self.request_timeout)):
-            self.tasks.append(self._loop.create_task(task))
+        self.tasks.append(
+            self._loop.create_task(self.set_timeout(self._waiters['request'],
+                                                    timeout=self._options['request_timeout'],
+                                                    timeout_cb=self.request_timeout))
+        )
 
     async def request_timeout(self, timeout):
         self._options['logger'].info('request timeout after {:g}s'.format(timeout))
 
     async def keepalive_timeout(self, timeout):
         self._options['logger'].info('keepalive timeout after {:g}s'.format(timeout))
 
@@ -246,15 +247,19 @@
 
         if self._data is not None:
             self._data.extend(data)
             header_size = self._data.find(b'\r\n\r\n')
 
             if -1 < header_size <= 8192:
                 self._transport.pause_reading()
-                self.tasks.append(self._loop.create_task(self._handle_request_header(self._data, header_size)))
+                self.tasks.extend([
+                    self._loop.create_task(self._send_data()),
+                    self._loop.create_task(self._handle_request_header(self._data, header_size))
+                ])
+
                 self._data = None
             elif header_size > 8192:
                 self._options['logger'].info('request header too large')
                 self._transport.abort()
             elif not (header_size == -1 and len(self._data) <= 8192):
                 self._options['logger'].info('bad request')
                 self._transport.abort()
@@ -346,22 +351,27 @@
 
         if not self._request.http_continue:
             self._data = bytearray()
             self._request.clear_body()
 
         self._waiters['keepalive'] = self._loop.create_future()
 
-        self.tasks.append(self._loop.create_task(self.set_timeout(self._waiters['keepalive'],
-                                                                  timeout=self._options['keepalive_timeout'],
-                                                                  timeout_cb=self.keepalive_timeout)))
+        self.tasks.append(
+            self._loop.create_task(self.set_timeout(self._waiters['keepalive'],
+                                                    timeout=self._options['keepalive_timeout'],
+                                                    timeout_cb=self.keepalive_timeout))
+        )
         self._transport.resume_reading()
 
     def connection_lost(self, exc):
         for task in self.tasks:
             if callable(task):
+                # even if you put callable objects in self.tasks,
+                # they will be executed when the client is disconnected.
+                # this is useful for the cleanup mechanism.
                 task()
                 continue
 
             try:
                 exc = task.exception()
 
                 if exc:
```

### Comparing `tremolo-0.0.97/tremolo/lib/http_request.py` & `tremolo-0.0.98/tremolo/lib/http_request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.97/tremolo/lib/http_response.py` & `tremolo-0.0.98/tremolo/lib/http_response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.97/tremolo/lib/object_pool.py` & `tremolo-0.0.98/tremolo/lib/object_pool.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.97/tremolo/lib/request.py` & `tremolo-0.0.98/tremolo/lib/request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.97/tremolo/lib/response.py` & `tremolo-0.0.98/tremolo/lib/response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.97/tremolo/tremolo.py` & `tremolo-0.0.98/tremolo/tremolo.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.97/tremolo.egg-info/PKG-INFO` & `tremolo-0.0.98/tremolo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.97
+Version: 0.0.98
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -79,15 +79,15 @@
 async def app(scope, receive, send):
     assert scope['type'] == 'http'
 
     await send({
         'type': 'http.response.start',
         'status': 200,
         'headers': [
-            (b'content-type', b'text/plain'),
+            (b'content-type', b'text/plain')
         ]
     })
 
     await send({
         'type': 'http.response.body',
         'body': b'Hello world!'
     })
@@ -116,15 +116,15 @@
 ```
 uvicorn --loop asyncio --http h11 --log-level error example:app
 ```
 
 vs
 
 ```
-python -m tremolo --log-level ERROR example:app
+python3 -m tremolo --log-level ERROR example:app
 ```
 
 You will find that Tremolo is reasonably fast.
 
 What's interesting is that this may become different when [CPython becomes faster](https://devblogs.microsoft.com/python/python-311-faster-cpython-team/),
 or another faster Python implementation comes along.
```

### Comparing `tremolo-0.0.97/tremolo.egg-info/SOURCES.txt` & `tremolo-0.0.98/tremolo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

