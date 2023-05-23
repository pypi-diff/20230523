# Comparing `tmp/sdss_clu-2.0.1.tar.gz` & `tmp/sdss_clu-2.0.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_clu-2.0.1.tar", max compression
+gzip compressed data, was "sdss_clu-2.0.2b1.tar", max compression
```

## Comparing `sdss_clu-2.0.1.tar` & `sdss_clu-2.0.2b1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1504 2023-03-13 00:37:42.451189 sdss_clu-2.0.1/LICENSE.md
--rw-r--r--   0        0        0     5049 2023-03-13 00:37:42.451418 sdss_clu-2.0.1/README.rst
--rw-r--r--   0        0        0     2665 2023-03-13 00:37:42.463756 sdss_clu-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      889 2023-03-13 00:37:42.464143 sdss_clu-2.0.1/python/clu/__init__.py
--rwxr-xr-x   0        0        0     7260 2023-03-13 00:37:42.464395 sdss_clu-2.0.1/python/clu/__main__.py
--rw-r--r--   0        0        0    13555 2023-03-13 00:37:42.464654 sdss_clu-2.0.1/python/clu/actor.py
--rw-r--r--   0        0        0    19832 2023-03-13 00:37:42.464985 sdss_clu-2.0.1/python/clu/base.py
--rw-r--r--   0        0        0    14541 2023-03-13 00:37:42.465258 sdss_clu-2.0.1/python/clu/client.py
--rw-r--r--   0        0        0    20069 2023-03-13 00:37:42.465540 sdss_clu-2.0.1/python/clu/command.py
--rw-r--r--   0        0        0     4135 2023-03-13 00:37:42.465804 sdss_clu-2.0.1/python/clu/device.py
--rw-r--r--   0        0        0     1347 2023-03-13 00:37:42.466013 sdss_clu-2.0.1/python/clu/exceptions.py
--rw-r--r--   0        0        0       41 2023-03-13 00:37:42.466455 sdss_clu-2.0.1/python/clu/legacy/__init__.py
--rw-r--r--   0        0        0    17892 2023-03-13 00:37:42.466743 sdss_clu-2.0.1/python/clu/legacy/actor.py
--rw-r--r--   0        0        0    13538 2023-03-13 00:37:42.467004 sdss_clu-2.0.1/python/clu/legacy/tron.py
--rw-r--r--   0        0        0        0 2023-03-13 00:37:42.467202 sdss_clu-2.0.1/python/clu/legacy/types/__init__.py
--rw-r--r--   0        0        0    15014 2023-03-13 00:37:42.467430 sdss_clu-2.0.1/python/clu/legacy/types/html.py
--rw-r--r--   0        0        0    17888 2023-03-13 00:37:42.467740 sdss_clu-2.0.1/python/clu/legacy/types/keys.py
--rw-r--r--   0        0        0    17508 2023-03-13 00:37:42.468009 sdss_clu-2.0.1/python/clu/legacy/types/messages.py
--rw-r--r--   0        0        0     9489 2023-03-13 00:37:42.468265 sdss_clu-2.0.1/python/clu/legacy/types/parser.py
--rwxr-xr-x   0        0        0      104 2023-03-13 00:37:42.468634 sdss_clu-2.0.1/python/clu/legacy/types/ply/__init__.py
--rwxr-xr-x   0        0        0    38405 2023-03-13 00:37:42.468987 sdss_clu-2.0.1/python/clu/legacy/types/ply/cpp.py
--rwxr-xr-x   0        0        0     2877 2023-03-13 00:37:42.469221 sdss_clu-2.0.1/python/clu/legacy/types/ply/ctokens.py
--rwxr-xr-x   0        0        0    45219 2023-03-13 00:37:42.469625 sdss_clu-2.0.1/python/clu/legacy/types/ply/lex.py
--rwxr-xr-x   0        0        0   140885 2023-03-13 00:37:42.470322 sdss_clu-2.0.1/python/clu/legacy/types/ply/yacc.py
--rwxr-xr-x   0        0        0     2314 2023-03-13 00:37:42.470627 sdss_clu-2.0.1/python/clu/legacy/types/ply/ygen.py
--rw-r--r--   0        0        0     5487 2023-03-13 00:37:42.470825 sdss_clu-2.0.1/python/clu/legacy/types/pvt.py
--rw-r--r--   0        0        0    19685 2023-03-13 00:37:42.471064 sdss_clu-2.0.1/python/clu/legacy/types/types.py
--rw-r--r--   0        0        0    11758 2023-03-13 00:37:42.471313 sdss_clu-2.0.1/python/clu/model.py
--rw-r--r--   0        0        0      309 2023-03-13 00:37:42.471591 sdss_clu-2.0.1/python/clu/parsers/__init__.py
--rw-r--r--   0        0        0    20428 2023-03-13 00:37:42.473334 sdss_clu-2.0.1/python/clu/parsers/click.py
--rw-r--r--   0        0        0     2685 2023-03-13 00:37:42.473557 sdss_clu-2.0.1/python/clu/parsers/json.py
--rw-r--r--   0        0        0    19724 2023-03-13 00:37:42.473829 sdss_clu-2.0.1/python/clu/protocol.py
--rw-r--r--   0        0        0     2805 2023-03-13 00:37:42.474175 sdss_clu-2.0.1/python/clu/store.py
--rw-r--r--   0        0        0     7820 2023-03-13 00:37:42.474417 sdss_clu-2.0.1/python/clu/testing.py
--rw-r--r--   0        0        0    16901 2023-03-13 00:37:42.474709 sdss_clu-2.0.1/python/clu/tools.py
--rw-r--r--   0        0        0     6412 1970-01-01 00:00:00.000000 sdss_clu-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-05-23 18:42:10.362267 sdss_clu-2.0.2b1/LICENSE.md
+-rw-r--r--   0        0        0     5049 2023-05-23 18:42:10.362498 sdss_clu-2.0.2b1/README.rst
+-rw-r--r--   0        0        0     2644 2023-05-23 18:42:10.376156 sdss_clu-2.0.2b1/pyproject.toml
+-rw-r--r--   0        0        0      889 2023-05-23 18:42:10.376648 sdss_clu-2.0.2b1/python/clu/__init__.py
+-rwxr-xr-x   0        0        0     7260 2023-05-23 18:42:10.377014 sdss_clu-2.0.2b1/python/clu/__main__.py
+-rw-r--r--   0        0        0    13555 2023-05-23 18:42:10.377447 sdss_clu-2.0.2b1/python/clu/actor.py
+-rw-r--r--   0        0        0    19832 2023-05-23 18:42:10.377898 sdss_clu-2.0.2b1/python/clu/base.py
+-rw-r--r--   0        0        0    14596 2023-05-23 18:42:10.378353 sdss_clu-2.0.2b1/python/clu/client.py
+-rw-r--r--   0        0        0    20069 2023-05-23 18:42:10.378854 sdss_clu-2.0.2b1/python/clu/command.py
+-rw-r--r--   0        0        0     4135 2023-05-23 18:42:10.421280 sdss_clu-2.0.2b1/python/clu/device.py
+-rw-r--r--   0        0        0     1347 2023-05-23 18:42:10.502589 sdss_clu-2.0.2b1/python/clu/exceptions.py
+-rw-r--r--   0        0        0       41 2023-05-23 18:42:10.502970 sdss_clu-2.0.2b1/python/clu/legacy/__init__.py
+-rw-r--r--   0        0        0    17892 2023-05-23 18:42:10.503291 sdss_clu-2.0.2b1/python/clu/legacy/actor.py
+-rw-r--r--   0        0        0    13538 2023-05-23 18:42:10.503623 sdss_clu-2.0.2b1/python/clu/legacy/tron.py
+-rw-r--r--   0        0        0        0 2023-05-23 18:42:10.503839 sdss_clu-2.0.2b1/python/clu/legacy/types/__init__.py
+-rw-r--r--   0        0        0    15014 2023-05-23 18:42:10.504088 sdss_clu-2.0.2b1/python/clu/legacy/types/html.py
+-rw-r--r--   0        0        0    17888 2023-05-23 18:42:10.504395 sdss_clu-2.0.2b1/python/clu/legacy/types/keys.py
+-rw-r--r--   0        0        0    17508 2023-05-23 18:42:10.504711 sdss_clu-2.0.2b1/python/clu/legacy/types/messages.py
+-rw-r--r--   0        0        0     9489 2023-05-23 18:42:10.505080 sdss_clu-2.0.2b1/python/clu/legacy/types/parser.py
+-rwxr-xr-x   0        0        0      104 2023-05-23 18:42:10.505376 sdss_clu-2.0.2b1/python/clu/legacy/types/ply/__init__.py
+-rwxr-xr-x   0        0        0    38405 2023-05-23 18:42:10.505775 sdss_clu-2.0.2b1/python/clu/legacy/types/ply/cpp.py
+-rwxr-xr-x   0        0        0     2877 2023-05-23 18:42:10.506167 sdss_clu-2.0.2b1/python/clu/legacy/types/ply/ctokens.py
+-rwxr-xr-x   0        0        0    45219 2023-05-23 18:42:10.506647 sdss_clu-2.0.2b1/python/clu/legacy/types/ply/lex.py
+-rwxr-xr-x   0        0        0   140885 2023-05-23 18:42:10.507599 sdss_clu-2.0.2b1/python/clu/legacy/types/ply/yacc.py
+-rwxr-xr-x   0        0        0     2314 2023-05-23 18:42:10.508114 sdss_clu-2.0.2b1/python/clu/legacy/types/ply/ygen.py
+-rw-r--r--   0        0        0     5487 2023-05-23 18:42:10.508442 sdss_clu-2.0.2b1/python/clu/legacy/types/pvt.py
+-rw-r--r--   0        0        0    19685 2023-05-23 18:42:10.508900 sdss_clu-2.0.2b1/python/clu/legacy/types/types.py
+-rw-r--r--   0        0        0    11758 2023-05-23 18:42:10.509180 sdss_clu-2.0.2b1/python/clu/model.py
+-rw-r--r--   0        0        0      309 2023-05-23 18:42:10.509537 sdss_clu-2.0.2b1/python/clu/parsers/__init__.py
+-rw-r--r--   0        0        0    20428 2023-05-23 18:42:10.509825 sdss_clu-2.0.2b1/python/clu/parsers/click.py
+-rw-r--r--   0        0        0     2685 2023-05-23 18:42:10.510042 sdss_clu-2.0.2b1/python/clu/parsers/json.py
+-rw-r--r--   0        0        0    19724 2023-05-23 18:42:10.510306 sdss_clu-2.0.2b1/python/clu/protocol.py
+-rw-r--r--   0        0        0     2805 2023-05-23 18:42:10.510527 sdss_clu-2.0.2b1/python/clu/store.py
+-rw-r--r--   0        0        0     7820 2023-05-23 18:42:10.510746 sdss_clu-2.0.2b1/python/clu/testing.py
+-rw-r--r--   0        0        0    16901 2023-05-23 18:42:10.511034 sdss_clu-2.0.2b1/python/clu/tools.py
+-rw-r--r--   0        0        0     6369 1970-01-01 00:00:00.000000 sdss_clu-2.0.2b1/PKG-INFO
```

### Comparing `sdss_clu-2.0.1/LICENSE.md` & `sdss_clu-2.0.2b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/README.rst` & `sdss_clu-2.0.2b1/README.rst`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/pyproject.toml` & `sdss_clu-2.0.2b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-clu"
-version = "2.0.1"
+version = "2.0.2b1"
 description = "A new protocol for SDSS actors."
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.rst"
 homepage = "https://github.com/sdss/clu"
 repository = "https://github.com/sdss/clu"
 documentation = "https://clu.readthedocs.io/en/latest/"
@@ -31,15 +31,14 @@
 click = "^8.0"
 aio_pika = "^9.0.0"
 jsonschema = "^4.0.1"
 sdsstools = "^1.0.0"
 prompt_toolkit = "^3.0.6"
 aiormq = "^6.6.4"
 unclick = "^0.1.0b4"
-setuptools = "^67.6.0"
 
 [tool.poetry.dev-dependencies]
 ipython = ">=8.0.0"
 flake8 = ">=3.7.9"
 doc8 = ">=0.8.0"
 toml = ">=0.10.0"
 isort = ">=5.2.2"
```

### Comparing `sdss_clu-2.0.1/python/clu/__init__.py` & `sdss_clu-2.0.2b1/python/clu/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/__main__.py` & `sdss_clu-2.0.2b1/python/clu/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/actor.py` & `sdss_clu-2.0.2b1/python/clu/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/base.py` & `sdss_clu-2.0.2b1/python/clu/base.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/client.py` & `sdss_clu-2.0.2b1/python/clu/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import asyncio
 import json
 import logging
 import pathlib
 import uuid
 
-from typing import TYPE_CHECKING, Callable, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Awaitable, Callable, Dict, List, Optional, Union
 
 import aio_pika as apika
 
 from sdsstools.logger import SDSSLogger
 
 from .base import BaseClient, Reply
 from .command import Command
@@ -31,14 +31,15 @@
     from aio_pika.abc import HeadersType
 
 
 __all__ = ["AMQPClient", "AMQPReply"]
 
 
 PathLike = Union[str, pathlib.Path]
+ReplyCallbackType = Callable[["AMQPReply"], Union[None, Awaitable[None]]]
 
 
 class AMQPReply(object):
     """Wrapper for an `~aio_pika.IncomingMessage` that expands and decodes it.
 
     Parameters
     ----------
@@ -203,15 +204,15 @@
         )
 
         #: dict: External commands currently running.
         self.running_commands: Dict[str, Command] = {}
 
         self.models = ModelSet(self, actors=models, raise_exception=False)
 
-        self._callbacks: list[Callable[[AMQPReply], None]] = []
+        self._callbacks: list[ReplyCallbackType] = []
 
     def __repr__(self):
         if self.connection.connection is None:
             url = "disconnected"
         else:
             assert isinstance(self.connection.connection, apika.Connection)
             url = str(self.connection.connection.url)
@@ -441,20 +442,20 @@
             )
 
         if await_command:
             await command
 
         return command
 
-    def add_reply_callback(self, callback_func: Callable[[AMQPReply], None]):
+    def add_reply_callback(self, callback_func: ReplyCallbackType):
         """Adds a callback that is called when a new reply is received."""
 
         if callback_func not in self._callbacks:
             self._callbacks.append(callback_func)
 
-    def remove_reply_callback(self, callback_func: Callable[[AMQPReply], None]):
+    def remove_reply_callback(self, callback_func: ReplyCallbackType):
         """Removes a reply callback."""
 
         if callback_func not in self._callbacks:
             raise ValueError("Callback not registered.")
 
         self._callbacks.remove(callback_func)
```

### Comparing `sdss_clu-2.0.1/python/clu/command.py` & `sdss_clu-2.0.2b1/python/clu/command.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/device.py` & `sdss_clu-2.0.2b1/python/clu/device.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/exceptions.py` & `sdss_clu-2.0.2b1/python/clu/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/legacy/actor.py` & `sdss_clu-2.0.2b1/python/clu/legacy/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/legacy/tron.py` & `sdss_clu-2.0.2b1/python/clu/legacy/tron.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/legacy/types/html.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/html.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/legacy/types/keys.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/keys.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/legacy/types/messages.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/messages.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/legacy/types/parser.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/parser.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/legacy/types/ply/cpp.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/ply/cpp.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/legacy/types/ply/ctokens.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/ply/ctokens.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/legacy/types/ply/lex.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/ply/lex.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/legacy/types/ply/yacc.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/legacy/types/ply/ygen.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/ply/ygen.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/legacy/types/pvt.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/pvt.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/legacy/types/types.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/types.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/model.py` & `sdss_clu-2.0.2b1/python/clu/model.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/parsers/click.py` & `sdss_clu-2.0.2b1/python/clu/parsers/click.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/parsers/json.py` & `sdss_clu-2.0.2b1/python/clu/parsers/json.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/protocol.py` & `sdss_clu-2.0.2b1/python/clu/protocol.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/store.py` & `sdss_clu-2.0.2b1/python/clu/store.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/testing.py` & `sdss_clu-2.0.2b1/python/clu/testing.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/python/clu/tools.py` & `sdss_clu-2.0.2b1/python/clu/tools.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.1/PKG-INFO` & `sdss_clu-2.0.2b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-clu
-Version: 2.0.1
+Version: 2.0.2b1
 Summary: A new protocol for SDSS actors.
 Home-page: https://github.com/sdss/clu
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.8,<4.0
@@ -22,15 +22,14 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aio_pika (>=9.0.0,<10.0.0)
 Requires-Dist: aiormq (>=6.6.4,<7.0.0)
 Requires-Dist: click (>=8.0,<9.0)
 Requires-Dist: jsonschema (>=4.0.1,<5.0.0)
 Requires-Dist: prompt_toolkit (>=3.0.6,<4.0.0)
 Requires-Dist: sdsstools (>=1.0.0,<2.0.0)
-Requires-Dist: setuptools (>=67.6.0,<68.0.0)
 Requires-Dist: unclick (>=0.1.0b4,<0.2.0)
 Project-URL: Documentation, https://clu.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/sdss/clu
 Description-Content-Type: text/x-rst
 
 `CLU <https://tron.fandom.com/wiki/Clu>`__
 ==========================================
```

