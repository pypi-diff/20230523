# Comparing `tmp/async_websocket_pool-0.1.1.tar.gz` & `tmp/async_websocket_pool-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_websocket_pool-0.1.1.tar", max compression
+gzip compressed data, was "async_websocket_pool-0.1.3.tar", max compression
```

## Comparing `async_websocket_pool-0.1.1.tar` & `async_websocket_pool-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-05-15 14:53:33.451094 async_websocket_pool-0.1.1/LICENSE
--rw-r--r--   0        0        0     1483 2023-05-15 14:53:33.455094 async_websocket_pool-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-15 14:53:33.455094 async_websocket_pool-0.1.1/async_websocket_pool/__init__.py
--rw-r--r--   0        0        0     3960 2023-05-15 14:53:33.455094 async_websocket_pool-0.1.1/async_websocket_pool/websocket.py
--rw-r--r--   0        0        0      573 2023-05-15 14:53:33.455094 async_websocket_pool-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 async_websocket_pool-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-23 16:19:04.143596 async_websocket_pool-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1483 2023-05-23 16:19:04.143596 async_websocket_pool-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 16:19:04.143596 async_websocket_pool-0.1.3/async_websocket_pool/__init__.py
+-rw-r--r--   0        0        0     4240 2023-05-23 16:19:04.143596 async_websocket_pool-0.1.3/async_websocket_pool/websocket.py
+-rw-r--r--   0        0        0      573 2023-05-23 16:19:04.143596 async_websocket_pool-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 async_websocket_pool-0.1.3/PKG-INFO
```

### Comparing `async_websocket_pool-0.1.1/LICENSE` & `async_websocket_pool-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `async_websocket_pool-0.1.1/README.md` & `async_websocket_pool-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `async_websocket_pool-0.1.1/async_websocket_pool/websocket.py` & `async_websocket_pool-0.1.3/async_websocket_pool/websocket.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import asyncio
 import logging
 import sys
 from typing import Any, Optional, Callable, List
 
 import websockets
+from websockets import WebSocketClientProtocol
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 logger.addHandler(logging.StreamHandler(sys.stdout))
 
 
 async def connect(
         url: str,
-        message_handler: Callable[[Any], None],
+        on_message: Callable[[Any], None],
+        on_connect: Optional[Callable[[WebSocketClientProtocol], None]],
         timeout: Optional[int | float] = None,
         **kwargs
 ) -> None:
     """
     Asynchronously establishes a WebSocket connection to a given endpoint and continuously listens
     for incoming messages until a timeout or a disconnection occurs.
 
@@ -29,33 +31,37 @@
     for a message. If a timeout duration is specified, the function will wait for that period before
     timing out and attempting to reconnect.
 
     All exceptions, except for asyncio.TimeoutError and websockets.ConnectionClosed, are logged and
     propagated up the call stack.
 
     :param url: The WebSocket URL to establish the connection.
-    :param message_handler: A callback function to handle incoming messages. This function should
+    :param on_message: A callback function to handle incoming messages. This function should
                             accept a single argument which will be the received message.
+    :param on_connect: A callback function that is executed every time successful connection is established.
     :param timeout: Optional; The maximum wait time for a message, in seconds. If set to None,
                     the function will wait indefinitely for a message.
     :param kwargs: Optional; Additional keyword arguments for the websockets.connect function to
                    further customize the WebSocket connection.
     :return: None
 
     :raises: This function propagates all exceptions except for asyncio.TimeoutError and
              websockets.ConnectionClosed, which are handled internally.
     """
     async for websocket in websockets.connect(url, **kwargs):
         try:
             logger.info(f'Connected to {url}')
 
+            if on_connect:
+                on_connect(websocket)
+
             while True:
                 try:
                     message: Any = await asyncio.wait_for(websocket.recv(), timeout=timeout)
-                    message_handler(message)
+                    on_message(message)
                 except asyncio.TimeoutError:
                     logger.warning(f'Timeout detected for {url}')
                     break
         except websockets.ConnectionClosed:
             logger.warning(f'Disconnected from {url}')
         except Exception as e:
             logger.exception(e)
```

### Comparing `async_websocket_pool-0.1.1/pyproject.toml` & `async_websocket_pool-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-websocket-pool"
-version = "0.1.1"
+version = "0.1.3"
 description = "async-websocket-pool is a Python library that enables efficient creation and management of a pool of asynchronous WebSocket clients."
 authors = ["mpol1t"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "async_websocket_pool"}]
 
 [tool.poetry.dependencies]
```

### Comparing `async_websocket_pool-0.1.1/PKG-INFO` & `async_websocket_pool-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-websocket-pool
-Version: 0.1.1
+Version: 0.1.3
 Summary: async-websocket-pool is a Python library that enables efficient creation and management of a pool of asynchronous WebSocket clients.
 License: MIT
 Author: mpol1t
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

