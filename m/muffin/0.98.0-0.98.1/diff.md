# Comparing `tmp/muffin-0.98.0.tar.gz` & `tmp/muffin-0.98.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin-0.98.0.tar", max compression
+gzip compressed data, was "muffin-0.98.1.tar", max compression
```

## Comparing `muffin-0.98.0.tar` & `muffin-0.98.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     9874 2023-05-23 08:03:28.922982 muffin-0.98.0/README.rst
--rw-r--r--   0        0        0      982 2023-05-23 08:03:28.922982 muffin-0.98.0/muffin/__init__.py
--rw-r--r--   0        0        0     5250 2023-05-23 08:03:28.922982 muffin-0.98.0/muffin/app.py
--rw-r--r--   0        0        0       71 2023-05-23 08:03:28.922982 muffin-0.98.0/muffin/constants.py
--rw-r--r--   0        0        0      701 2023-05-23 08:03:28.922982 muffin-0.98.0/muffin/errors.py
--rw-r--r--   0        0        0     3754 2023-05-23 08:03:28.922982 muffin-0.98.0/muffin/handler.py
--rw-r--r--   0        0        0     8805 2023-05-23 08:03:28.922982 muffin-0.98.0/muffin/manage.py
--rw-r--r--   0        0        0     2857 2023-05-23 08:03:28.922982 muffin-0.98.0/muffin/plugins.py
--rw-r--r--   0        0        0        0 2023-05-23 08:03:28.922982 muffin-0.98.0/muffin/py.typed
--rw-r--r--   0        0        0     2705 2023-05-23 08:03:28.926982 muffin-0.98.0/muffin/pytest.py
--rw-r--r--   0        0        0      153 2023-05-23 08:03:28.926982 muffin-0.98.0/muffin/types.py
--rw-r--r--   0        0        0     2584 2023-05-23 08:03:28.926982 muffin-0.98.0/muffin/utils.py
--rw-r--r--   0        0        0     2990 2023-05-23 08:03:28.926982 muffin-0.98.0/pyproject.toml
--rw-r--r--   0        0        0    11329 1970-01-01 00:00:00.000000 muffin-0.98.0/PKG-INFO
+-rw-r--r--   0        0        0     9874 2023-05-23 08:19:08.565057 muffin-0.98.1/README.rst
+-rw-r--r--   0        0        0      982 2023-05-23 08:19:08.569057 muffin-0.98.1/muffin/__init__.py
+-rw-r--r--   0        0        0     5237 2023-05-23 08:19:08.569057 muffin-0.98.1/muffin/app.py
+-rw-r--r--   0        0        0       71 2023-05-23 08:19:08.569057 muffin-0.98.1/muffin/constants.py
+-rw-r--r--   0        0        0      701 2023-05-23 08:19:08.569057 muffin-0.98.1/muffin/errors.py
+-rw-r--r--   0        0        0     3754 2023-05-23 08:19:08.569057 muffin-0.98.1/muffin/handler.py
+-rw-r--r--   0        0        0     8805 2023-05-23 08:19:08.569057 muffin-0.98.1/muffin/manage.py
+-rw-r--r--   0        0        0     2857 2023-05-23 08:19:08.569057 muffin-0.98.1/muffin/plugins.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:19:08.569057 muffin-0.98.1/muffin/py.typed
+-rw-r--r--   0        0        0     2705 2023-05-23 08:19:08.569057 muffin-0.98.1/muffin/pytest.py
+-rw-r--r--   0        0        0      153 2023-05-23 08:19:08.569057 muffin-0.98.1/muffin/types.py
+-rw-r--r--   0        0        0     2743 2023-05-23 08:19:08.569057 muffin-0.98.1/muffin/utils.py
+-rw-r--r--   0        0        0     2990 2023-05-23 08:19:08.569057 muffin-0.98.1/pyproject.toml
+-rw-r--r--   0        0        0    11329 1970-01-01 00:00:00.000000 muffin-0.98.1/PKG-INFO
```

### Comparing `muffin-0.98.0/README.rst` & `muffin-0.98.1/README.rst`

 * *Files identical despite different names*

### Comparing `muffin-0.98.0/muffin/__init__.py` & `muffin-0.98.1/muffin/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.0/muffin/app.py` & `muffin-0.98.1/muffin/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import TYPE_CHECKING, Any, Dict, Final, Mapping, Union
 
 from asgi_tools import App as BaseApp
 from asgi_tools._compat import aio_wait
 from modconfig import Config
 
 from muffin.constants import CONFIG_ENV_VARIABLE
-from muffin.utils import import_submodules
+from muffin.utils import import_submodules, logger
 
 if TYPE_CHECKING:
     from collections.abc import Awaitable
     from types import ModuleType
 
     from asgi_tools.types import TASGIReceive, TASGIScope, TASGISend
 
@@ -71,15 +71,15 @@
 
         # Setup CLI
         from muffin.manage import Manager
 
         self.manage = Manager(self)
 
         # Setup logging
-        self.logger = logging.getLogger("muffin")
+        self.logger = logger
         self.logger.setLevel(self.cfg.LOG_LEVEL)
         self.logger.propagate = False
         if not self.logger.handlers:
             ch = logging.StreamHandler()
             ch.setFormatter(
                 logging.Formatter(self.cfg.LOG_FORMAT, self.cfg.LOG_DATE_FORMAT),
             )
```

### Comparing `muffin-0.98.0/muffin/errors.py` & `muffin-0.98.1/muffin/errors.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.0/muffin/handler.py` & `muffin-0.98.1/muffin/handler.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.0/muffin/manage.py` & `muffin-0.98.1/muffin/manage.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.0/muffin/plugins.py` & `muffin-0.98.1/muffin/plugins.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.0/muffin/pytest.py` & `muffin-0.98.1/muffin/pytest.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.0/muffin/utils.py` & `muffin-0.98.1/muffin/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import sys
 import threading
 from collections import OrderedDict
 from contextlib import suppress
 from typing import TYPE_CHECKING, Callable, Coroutine, Dict, TypeVar
 
 from asgi_tools.utils import is_awaitable, to_awaitable
+from curio.task import logging
 from sniffio import current_async_library
 
 from muffin.errors import InvalidAppError
 
 if TYPE_CHECKING:
     from types import ModuleType
 
@@ -45,14 +46,16 @@
 
     AIOLIBS["trio"] = trio
 
 AIOLIBS["asyncio"] = asyncio
 
 TV = TypeVar("TV")
 
+logger = logging.getLogger("muffin")
+
 
 def aio_lib() -> str:
     """Return first available async library."""
     aiolib = os.environ.get("MUFFIN_AIOLIB", "asyncio")
     if aiolib:
         return aiolib
 
@@ -83,14 +86,16 @@
     ):
         try:
             res[module_name] = importlib.import_module(f"{package_name}.{module_name}")
         except ImportError:
             if not silent:
                 raise
 
+            logger.debug("Failed to import module: %s", f"{package_name}.{module_name}")
+
     return res
 
 
 def import_app(app_uri: str, *, reload: bool = False) -> Application:
     """Import application by the given string (python.path.to.module:app_name)."""
     mod_name, _, app_name = app_uri.partition(":")
     mod = importlib.import_module(mod_name)
```

### Comparing `muffin-0.98.0/pyproject.toml` & `muffin-0.98.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin"
-version = "0.98.0"
+version = "0.98.1"
 description = "Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)"
 readme = "README.rst"
 license = "MIT"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 keywords = ["asgi", "web", "web framework", "asyncio", "trio", "curio"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
```

### Comparing `muffin-0.98.0/PKG-INFO` & `muffin-0.98.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin
-Version: 0.98.0
+Version: 0.98.1
 Summary: Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)
 Home-page: https://github.com/klen/muffin
 License: MIT
 Keywords: asgi,web,web framework,asyncio,trio,curio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

