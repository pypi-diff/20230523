# Comparing `tmp/python-ascendex-0.1.3.tar.gz` & `tmp/python_ascendex-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-ascendex-0.1.3.tar", max compression
+gzip compressed data, was "python_ascendex-0.2.0.tar", max compression
```

## Comparing `python-ascendex-0.1.3.tar` & `python_ascendex-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2021-07-16 20:32:58.763222 python-ascendex-0.1.3/LICENSE
--rw-r--r--   0        0        0      174 2021-07-17 19:23:04.971639 python-ascendex-0.1.3/ascendex/__init__.py
--rw-r--r--   0        0        0      457 2021-10-11 18:14:59.487690 python-ascendex-0.1.3/ascendex/exceptions.py
--rw-r--r--   0        0        0     4454 2021-11-12 18:39:39.036710 python-ascendex-0.1.3/ascendex/reconnecting_websocket.py
--rw-r--r--   0        0        0     6899 2021-10-11 18:37:32.355721 python-ascendex-0.1.3/ascendex/rest_client.py
--rw-r--r--   0        0        0     1433 2021-07-17 21:26:38.052905 python-ascendex-0.1.3/ascendex/util.py
--rw-r--r--   0        0        0    11794 2021-11-12 14:10:20.362549 python-ascendex-0.1.3/ascendex/web_socket_client.py
--rw-r--r--   0        0        0      487 2021-11-12 18:45:39.556945 python-ascendex-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      688 2021-11-12 18:45:55.474802 python-ascendex-0.1.3/setup.py
--rw-r--r--   0        0        0      541 2021-11-12 18:45:55.475000 python-ascendex-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-10-11 12:20:21.310147 python_ascendex-0.2.0/LICENSE
+-rw-r--r--   0        0        0      174 2022-10-11 12:20:21.310147 python_ascendex-0.2.0/ascendex/__init__.py
+-rw-r--r--   0        0        0      457 2022-10-11 12:20:21.310147 python_ascendex-0.2.0/ascendex/exceptions.py
+-rw-r--r--   0        0        0     4454 2022-10-11 12:20:21.310147 python_ascendex-0.2.0/ascendex/reconnecting_websocket.py
+-rw-r--r--   0        0        0     7190 2022-10-11 12:20:21.310147 python_ascendex-0.2.0/ascendex/rest_client.py
+-rw-r--r--   0        0        0     1433 2022-10-11 12:20:21.310147 python_ascendex-0.2.0/ascendex/util.py
+-rw-r--r--   0        0        0    11876 2022-10-11 12:25:43.398075 python_ascendex-0.2.0/ascendex/web_socket_client.py
+-rw-r--r--   0        0        0      511 2023-05-23 15:12:57.634323 python_ascendex-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 python_ascendex-0.2.0/setup.py
+-rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 python_ascendex-0.2.0/PKG-INFO
```

### Comparing `python-ascendex-0.1.3/LICENSE` & `python_ascendex-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-ascendex-0.1.3/ascendex/reconnecting_websocket.py` & `python_ascendex-0.2.0/ascendex/reconnecting_websocket.py`

 * *Files identical despite different names*

### Comparing `python-ascendex-0.1.3/ascendex/rest_client.py` & `python_ascendex-0.2.0/ascendex/rest_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional
 import asyncio
 import aiosonic
 import ujson
 import time
 import logging
 
 from ascendex.util import *
@@ -16,27 +17,27 @@
         self.group_id = group_id
         self.api_key = api_key
         self.api_secret = api_secret
         self.last_response_headers = {}
         self._timeouts = aiosonic.Timeouts(request_timeout = request_timeout)
         self.session = self._init_session()
 
-    def _init_session(self):
+    def _init_session(self) -> aiosonic.HTTPClient:
         session = aiosonic.HTTPClient(
             connector=aiosonic.TCPConnector(
                 pool_size=self.POOL_SIZE,
                 timeouts=self._timeouts,
             ),
         )
         return session
 
     async def close(self):
         await self.session.shutdown()
 
-    async def _request(self, method, path, uri_account = None, include_group = False, version = 'v1', **kwargs):
+    async def _request(self, method, path, uri_account = None, include_group = False, version = 'v1', timeouts: Optional[aiosonic.Timeouts] = None, **kwargs):
         '''
         Perform REST api request
 
         :param method: http method such as 'get'
         :param path: last portion of the api uri path without ROUTE_PREFIX, account and leading slash
         :param uri_account: 'cash' | 'margin' | ...
         :param include_group: should group id be included in uri?
@@ -64,15 +65,15 @@
             path = f'{ROUTE_PREFIX}/{version}/{path}'
 
         uri = f'{self.API_URL}/{path}'
         # print(uri)
         # print(params)
         # print(data)
         response = await self.session.request(
-            uri, method, headers, params, data
+            url = uri, method = method, headers = headers, params = params, data = data, timeouts = timeouts
         )
         self.session.wait_requests
         return await self._handle_response(uri, params, response)
 
     async def _handle_response(self, uri: str, params: str, response: aiosonic.HttpResponse):
         """Internal helper for handling API responses from the Binance server.
         Raises the appropriate exceptions when necessary; otherwise, returns the
@@ -80,27 +81,26 @@
         """
         if not str(response.status_code).startswith("2"):
             raise AscendexAPIException(uri, params, response, await response.text())
         self.last_response_headers = response.headers
         try:
             content = ujson.loads(await response.content())
         except ValueError:
-            txt = await response.text()
-            raise AscendexAPIException(uri, params, "Invalid Response", txt)
+            raise AscendexAPIException(uri, params, response, await response.text())
         except AttributeError:
             # weird aiosonic bug:
             # File "/home/ec2-user/bot/env/lib/python3.8/site-packages/aiosonic/__init__.py", line 263, in read_chunks
             # chunk_size = int((await self.connection.reader.readline()).rstrip(), 16)
             # AttributeError: 'NoneType' object has no attribute 'reader'
             logging.warning('Reponse chunked=%s keep_alive=%s blocked=%s',
                 response.chunked,
                 response.connection.keep_alive if response.connection else None,
                 response.connection.blocked if response.connection else None
             )
-            raise AscendexAPIException(uri, params, 'Connection lost during _handle_response', response)
+            raise AscendexAPIException(uri, params, response, 'Connection lost during _handle_response')
 
         if 'message' in content and 'reason' in content:
             raise AscendexAPIException(uri, params, response, content['reason'] + ': ' + content['message'])
         return content
 
     # Exchange Endpoints
 
@@ -167,29 +167,31 @@
             "get",
             "order/hist",
             include_group = True,
             symbol=symbol,
             account = 'cash',
             version = 'v2',
             limit = limit,
+            timeouts = aiosonic.Timeouts(request_timeout = 10 + limit * 0.1),
             **kwargs,
         )
         return list(sorted(res["data"], key = lambda item: item['lastExecTime']))
 
     async def get_fills(self, symbol, limit, page = 0):
         res = await self._request(
             "get",
             "order/hist",
             include_group = True,
             symbol = symbol,
             category = 'CASH',
             version = 'v1',
             pageSize = limit,
             page = page,
-            status = 'WithFill'
+            status = 'WithFill',
+            timeouts = aiosonic.Timeouts(request_timeout = 10 + page * limit * 0.1),
         )
         if not 'data' in res or not 'data' in res['data']:
             return []
         return list(sorted(
             res['data']['data'],
             key = lambda item: item['lastExecTime']
         ))
```

### Comparing `python-ascendex-0.1.3/ascendex/util.py` & `python_ascendex-0.2.0/ascendex/util.py`

 * *Files identical despite different names*

### Comparing `python-ascendex-0.1.3/ascendex/web_socket_client.py` & `python_ascendex-0.2.0/ascendex/web_socket_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         self.loop = asyncio.get_event_loop()
         self._url = f"{self.WS_DOMAIN}/{group_id}/{ROUTE_PREFIX}/v1/stream"
         # TODO: the reconnection logic doesnt work properly, therefore we raise exception on reconnect
         self.ws = ReconnectingWebsocket(
             loop=self.loop,
             path=self._url,
             coro=self.on_message,
-            reconnect_auth_coro = self._raise_on_disconnect,
+            reconnect_auth_coro = self._on_reconnect,
         )
         self.subscribers = {}
         self.responses = collections.defaultdict(dict)
 
         self.key = api_key
         self.secret = api_secret
 
@@ -51,16 +51,20 @@
         id_ = self.get_uuid()[:6]
         msg = ujson.dumps(
             dict(op="auth", id=id_, t=ts, key=self.key, sig=sig)
         )
         await self.ws.send(msg)
         await self._wait_response('auth', id_)
 
-    async def _raise_on_disconnect(self) -> None:
-        raise websockets.exceptions.ConnectionClosedError(-1, 'Websocket connection lost')
+    async def _on_reconnect(self):
+        await self.authenticate()
+        # Resubscribe
+        for channel, ids in self.subscribers.items():
+            for id_ in ids:
+                await self._send_subscribe(id_, channel)
 
     @staticmethod
     def _get_subscribe_message(channel, symbols, unsubscribe=False):
         msg_type = "unsub" if unsubscribe else "sub"
         msg = {"op": msg_type, "ch": "{}:{}".format(channel, symbols)}
         return ujson.dumps(msg)
```

### Comparing `python-ascendex-0.1.3/setup.py` & `python_ascendex-0.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 packages = \
 ['ascendex']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['aiosonic>=0.12.0,<0.13.0',
+['aiosonic>=0.16.1,<0.17.0',
  'chardet>=4.0.0,<5.0.0',
- 'ujson>=4.0.2,<5.0.0',
- 'websockets>=9.1,<10.0']
+ 'ujson>=5.1.0,<6.0.0',
+ 'websockets>=11.0.2,<12']
 
 setup_kwargs = {
     'name': 'python-ascendex',
-    'version': '0.1.3',
+    'version': '0.2.0',
     'description': 'Python API for AscendEx',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'Jan Skoda',
     'author_email': 'skoda@jskoda.cz',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `python-ascendex-0.1.3/PKG-INFO` & `python_ascendex-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: python-ascendex
-Version: 0.1.3
+Version: 0.2.0
 Summary: Python API for AscendEx
 License: MIT
 Author: Jan Skoda
 Author-email: skoda@jskoda.cz
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: aiosonic (>=0.12.0,<0.13.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiosonic (>=0.16.1,<0.17.0)
 Requires-Dist: chardet (>=4.0.0,<5.0.0)
-Requires-Dist: ujson (>=4.0.2,<5.0.0)
-Requires-Dist: websockets (>=9.1,<10.0)
+Requires-Dist: ujson (>=5.1.0,<6.0.0)
+Requires-Dist: websockets (>=11.0.2,<12)
```

