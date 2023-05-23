# Comparing `tmp/asgiref-3.5.2.tar.gz` & `tmp/asgiref-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgiref-3.5.2.tar", last modified: Mon May 16 20:39:02 2022, max compression
+gzip compressed data, was "asgiref-3.6.0.tar", last modified: Tue Dec 20 09:06:25 2022, max compression
```

## Comparing `asgiref-3.5.2.tar` & `asgiref-3.6.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2022-05-16 20:39:02.462978 asgiref-3.5.2/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1552 2021-03-24 16:04:48.000000 asgiref-3.5.2/LICENSE
--rw-r--r--   0 andrew    (1000) andrew    (1000)       70 2021-04-05 16:48:44.000000 asgiref-3.5.2/MANIFEST.in
--rw-r--r--   0 andrew    (1000) andrew    (1000)     8946 2022-05-16 20:39:02.462978 asgiref-3.5.2/PKG-INFO
--rw-r--r--   0 andrew    (1000) andrew    (1000)     7756 2022-01-22 16:43:01.000000 asgiref-3.5.2/README.rst
-drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2022-05-16 20:39:02.462978 asgiref-3.5.2/asgiref/
--rw-r--r--   0 andrew    (1000) andrew    (1000)       22 2022-05-16 20:29:01.000000 asgiref-3.5.2/asgiref/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1598 2022-01-22 16:43:01.000000 asgiref-3.5.2/asgiref/compatibility.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2801 2021-04-05 16:48:44.000000 asgiref-3.5.2/asgiref/current_thread_executor.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     4854 2021-08-18 14:20:12.000000 asgiref-3.5.2/asgiref/local.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)        0 2021-04-05 16:48:44.000000 asgiref-3.5.2/asgiref/py.typed
--rw-r--r--   0 andrew    (1000) andrew    (1000)     6005 2021-11-22 17:42:08.000000 asgiref-3.5.2/asgiref/server.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)    20185 2022-05-16 20:28:11.000000 asgiref-3.5.2/asgiref/sync.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     3119 2021-03-24 16:04:48.000000 asgiref-3.5.2/asgiref/testing.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     3440 2022-01-22 16:43:01.000000 asgiref-3.5.2/asgiref/timeout.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     5603 2022-01-22 16:53:53.000000 asgiref-3.5.2/asgiref/typing.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     6575 2021-03-24 16:04:48.000000 asgiref-3.5.2/asgiref/wsgi.py
-drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2022-05-16 20:39:02.462978 asgiref-3.5.2/asgiref.egg-info/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     8946 2022-05-16 20:39:02.000000 asgiref-3.5.2/asgiref.egg-info/PKG-INFO
--rw-r--r--   0 andrew    (1000) andrew    (1000)      613 2022-05-16 20:39:02.000000 asgiref-3.5.2/asgiref.egg-info/SOURCES.txt
--rw-r--r--   0 andrew    (1000) andrew    (1000)        1 2022-05-16 20:39:02.000000 asgiref-3.5.2/asgiref.egg-info/dependency_links.txt
--rw-r--r--   0 andrew    (1000) andrew    (1000)        1 2022-05-16 20:39:01.000000 asgiref-3.5.2/asgiref.egg-info/not-zip-safe
--rw-r--r--   0 andrew    (1000) andrew    (1000)       88 2022-05-16 20:39:02.000000 asgiref-3.5.2/asgiref.egg-info/requires.txt
--rw-r--r--   0 andrew    (1000) andrew    (1000)        8 2022-05-16 20:39:02.000000 asgiref-3.5.2/asgiref.egg-info/top_level.txt
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2688 2022-05-16 20:39:02.462978 asgiref-3.5.2/setup.cfg
--rw-r--r--   0 andrew    (1000) andrew    (1000)       62 2021-04-05 16:48:44.000000 asgiref-3.5.2/setup.py
-drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2022-05-16 20:39:02.462978 asgiref-3.5.2/tests/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2329 2021-04-05 16:47:44.000000 asgiref-3.5.2/tests/test_compatibility.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     8031 2021-04-05 16:47:44.000000 asgiref-3.5.2/tests/test_local.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     4851 2022-05-16 20:28:11.000000 asgiref-3.5.2/tests/test_server.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)    20785 2022-05-16 20:28:11.000000 asgiref-3.5.2/tests/test_sync.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2121 2022-01-22 16:43:01.000000 asgiref-3.5.2/tests/test_sync_contextvars.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1396 2021-03-24 16:04:48.000000 asgiref-3.5.2/tests/test_testing.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     8718 2021-06-27 20:11:39.000000 asgiref-3.5.2/tests/test_wsgi.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2022-12-20 09:06:25.459062 asgiref-3.6.0/
+-rw-r--r--   0 carlton    (501) staff       (20)     1552 2022-04-19 07:47:42.000000 asgiref-3.6.0/LICENSE
+-rw-r--r--   0 carlton    (501) staff       (20)       70 2022-04-19 07:47:42.000000 asgiref-3.6.0/MANIFEST.in
+-rw-r--r--   0 carlton    (501) staff       (20)     9006 2022-12-20 09:06:25.459167 asgiref-3.6.0/PKG-INFO
+-rw-r--r--   0 carlton    (501) staff       (20)     7756 2022-07-06 14:22:11.000000 asgiref-3.6.0/README.rst
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2022-12-20 09:06:25.456699 asgiref-3.6.0/asgiref/
+-rw-r--r--   0 carlton    (501) staff       (20)       22 2022-12-20 08:57:26.000000 asgiref-3.6.0/asgiref/__init__.py
+-rw-r--r--   0 carlton    (501) staff       (20)     1606 2022-12-15 09:04:51.000000 asgiref-3.6.0/asgiref/compatibility.py
+-rw-r--r--   0 carlton    (501) staff       (20)     2801 2022-04-19 07:47:42.000000 asgiref-3.6.0/asgiref/current_thread_executor.py
+-rw-r--r--   0 carlton    (501) staff       (20)     4854 2022-04-19 07:47:42.000000 asgiref-3.6.0/asgiref/local.py
+-rw-r--r--   0 carlton    (501) staff       (20)        0 2022-04-19 07:47:42.000000 asgiref-3.6.0/asgiref/py.typed
+-rw-r--r--   0 carlton    (501) staff       (20)     6005 2022-08-08 06:48:57.000000 asgiref-3.6.0/asgiref/server.py
+-rw-r--r--   0 carlton    (501) staff       (20)    20664 2022-12-15 09:04:51.000000 asgiref-3.6.0/asgiref/sync.py
+-rw-r--r--   0 carlton    (501) staff       (20)     3119 2022-04-19 07:47:42.000000 asgiref-3.6.0/asgiref/testing.py
+-rw-r--r--   0 carlton    (501) staff       (20)     3627 2022-12-15 18:33:28.000000 asgiref-3.6.0/asgiref/timeout.py
+-rw-r--r--   0 carlton    (501) staff       (20)     5843 2022-12-15 09:04:51.000000 asgiref-3.6.0/asgiref/typing.py
+-rw-r--r--   0 carlton    (501) staff       (20)     6575 2022-04-19 07:47:42.000000 asgiref-3.6.0/asgiref/wsgi.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2022-12-20 09:06:25.457631 asgiref-3.6.0/asgiref.egg-info/
+-rw-r--r--   0 carlton    (501) staff       (20)     9006 2022-12-20 09:06:25.000000 asgiref-3.6.0/asgiref.egg-info/PKG-INFO
+-rw-r--r--   0 carlton    (501) staff       (20)      613 2022-12-20 09:06:25.000000 asgiref-3.6.0/asgiref.egg-info/SOURCES.txt
+-rw-r--r--   0 carlton    (501) staff       (20)        1 2022-12-20 09:06:25.000000 asgiref-3.6.0/asgiref.egg-info/dependency_links.txt
+-rw-r--r--   0 carlton    (501) staff       (20)        1 2022-07-06 08:14:22.000000 asgiref-3.6.0/asgiref.egg-info/not-zip-safe
+-rw-r--r--   0 carlton    (501) staff       (20)       88 2022-12-20 09:06:25.000000 asgiref-3.6.0/asgiref.egg-info/requires.txt
+-rw-r--r--   0 carlton    (501) staff       (20)        8 2022-12-20 09:06:25.000000 asgiref-3.6.0/asgiref.egg-info/top_level.txt
+-rw-r--r--   0 carlton    (501) staff       (20)     2737 2022-12-20 09:06:25.459771 asgiref-3.6.0/setup.cfg
+-rw-r--r--   0 carlton    (501) staff       (20)       62 2022-04-19 07:47:42.000000 asgiref-3.6.0/setup.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2022-12-20 09:06:25.458884 asgiref-3.6.0/tests/
+-rw-r--r--   0 carlton    (501) staff       (20)     2329 2022-04-19 07:47:42.000000 asgiref-3.6.0/tests/test_compatibility.py
+-rw-r--r--   0 carlton    (501) staff       (20)     8031 2022-04-19 07:47:42.000000 asgiref-3.6.0/tests/test_local.py
+-rw-r--r--   0 carlton    (501) staff       (20)     4837 2022-12-15 09:04:51.000000 asgiref-3.6.0/tests/test_server.py
+-rw-r--r--   0 carlton    (501) staff       (20)    20811 2022-12-15 09:04:51.000000 asgiref-3.6.0/tests/test_sync.py
+-rw-r--r--   0 carlton    (501) staff       (20)     2121 2022-07-06 14:22:11.000000 asgiref-3.6.0/tests/test_sync_contextvars.py
+-rw-r--r--   0 carlton    (501) staff       (20)     1396 2022-04-19 07:47:42.000000 asgiref-3.6.0/tests/test_testing.py
+-rw-r--r--   0 carlton    (501) staff       (20)     8718 2022-04-19 07:47:42.000000 asgiref-3.6.0/tests/test_wsgi.py
```

### Comparing `asgiref-3.5.2/LICENSE` & `asgiref-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asgiref-3.5.2/PKG-INFO` & `asgiref-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: asgiref
-Version: 3.5.2
+Version: 3.6.0
 Summary: ASGI specs, helper code, and adapters
 Home-page: https://github.com/django/asgiref/
 Author: Django Software Foundation
 Author-email: foundation@djangoproject.com
-License: BSD
+License: BSD-3-Clause
 Project-URL: Documentation, https://asgi.readthedocs.io/
 Project-URL: Further Documentation, https://docs.djangoproject.com/en/stable/topics/async/#async-adapter-functions
 Project-URL: Changelog, https://github.com/django/asgiref/blob/master/CHANGELOG.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.7
 Provides-Extra: tests
 License-File: LICENSE
 
 asgiref
 =======
```

### Comparing `asgiref-3.5.2/README.rst` & `asgiref-3.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `asgiref-3.5.2/asgiref/compatibility.py` & `asgiref-3.6.0/asgiref/compatibility.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import asyncio
 import inspect
 
+from .sync import iscoroutinefunction
+
 
 def is_double_callable(application):
     """
     Tests to see if an application is a legacy-style (double-callable) application.
     """
     # Look for a hint on the object first
     if getattr(application, "_asgi_single_callable", False):
@@ -14,18 +15,18 @@
     # Uninstanted classes are double-callable
     if inspect.isclass(application):
         return True
     # Instanted classes depend on their __call__
     if hasattr(application, "__call__"):
         # We only check to see if its __call__ is a coroutine function -
         # if it's not, it still might be a coroutine function itself.
-        if asyncio.iscoroutinefunction(application.__call__):
+        if iscoroutinefunction(application.__call__):
             return False
     # Non-classes we just check directly
-    return not asyncio.iscoroutinefunction(application)
+    return not iscoroutinefunction(application)
 
 
 def double_to_single_callable(application):
     """
     Transforms a double-callable ASGI application into a single-callable one.
     """
```

### Comparing `asgiref-3.5.2/asgiref/current_thread_executor.py` & `asgiref-3.6.0/asgiref/current_thread_executor.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.5.2/asgiref/local.py` & `asgiref-3.6.0/asgiref/local.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.5.2/asgiref/server.py` & `asgiref-3.6.0/asgiref/server.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.5.2/asgiref/sync.py` & `asgiref-3.6.0/asgiref/sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,27 +22,49 @@
         try:
             if cvar.get() != context.get(cvar):
                 cvar.set(context.get(cvar))
         except LookupError:
             cvar.set(context.get(cvar))
 
 
+# Python 3.12 deprecates asyncio.iscoroutinefunction() as an alias for
+# inspect.iscoroutinefunction(), whilst also removing the _is_coroutine marker.
+# The latter is replaced with the inspect.markcoroutinefunction decorator.
+# Until 3.12 is the minimum supported Python version, provide a shim.
+# Django 4.0 only supports 3.8+, so don't concern with the _or_partial backport.
+
+# Type hint: should be generic: whatever T it takes it returns. (Same id)
+def markcoroutinefunction(func: Any) -> Any:
+    if hasattr(inspect, "markcoroutinefunction"):
+        return inspect.markcoroutinefunction(func)
+    else:
+        func._is_coroutine = asyncio.coroutines._is_coroutine  # type: ignore
+        return func
+
+
+def iscoroutinefunction(func: Any) -> bool:
+    if hasattr(inspect, "markcoroutinefunction"):
+        return inspect.iscoroutinefunction(func)
+    else:
+        return asyncio.iscoroutinefunction(func)
+
+
 def _iscoroutinefunction_or_partial(func: Any) -> bool:
     # Python < 3.8 does not correctly determine partially wrapped
     # coroutine functions are coroutine functions, hence the need for
     # this to exist. Code taken from CPython.
     if sys.version_info >= (3, 8):
-        return asyncio.iscoroutinefunction(func)
+        return iscoroutinefunction(func)
     else:
         while inspect.ismethod(func):
             func = func.__func__
         while isinstance(func, functools.partial):
             func = func.func
 
-        return asyncio.iscoroutinefunction(func)
+        return iscoroutinefunction(func)
 
 
 class ThreadSensitiveContext:
     """Async context manager to manage context for thread sensitive mode
 
     This context manager controls which thread pool executor is used when in
     thread sensitive mode. By default, a single thread pool executor is shared
@@ -310,23 +332,14 @@
     rather than just blocking.
 
     If executor is passed in, that will be used instead of the loop's default executor.
     In order to pass in an executor, thread_sensitive must be set to False, otherwise
     a TypeError will be raised.
     """
 
-    # If they've set ASGI_THREADS, update the default asyncio executor for now
-    if "ASGI_THREADS" in os.environ:
-        # We use get_event_loop here - not get_running_loop - as this will
-        # be run at import time, and we want to update the main thread's loop.
-        loop = asyncio.get_event_loop()
-        loop.set_default_executor(
-            ThreadPoolExecutor(max_workers=int(os.environ["ASGI_THREADS"]))
-        )
-
     # Maps launched threads to the coroutines that spawned them
     launch_map: "Dict[threading.Thread, asyncio.Task[object]]" = {}
 
     # Storage for main event loop references
     threadlocal = threading.local()
 
     # Single-thread executor for thread-sensitive code
@@ -361,15 +374,15 @@
             or _iscoroutinefunction_or_partial(func)
             or _iscoroutinefunction_or_partial(getattr(func, "__call__", func))
         ):
             raise TypeError("sync_to_async can only be applied to sync functions.")
         self.func = func
         functools.update_wrapper(self, func)
         self._thread_sensitive = thread_sensitive
-        self._is_coroutine = asyncio.coroutines._is_coroutine  # type: ignore
+        markcoroutinefunction(self)
         if thread_sensitive and executor is not None:
             raise TypeError("executor must not be set when thread_sensitive is True")
         self._executor = executor
         try:
             self.__self__ = func.__self__  # type: ignore
         except AttributeError:
             pass
@@ -441,15 +454,16 @@
 
         return ret
 
     def __get__(self, parent, objtype):
         """
         Include self for methods
         """
-        return functools.partial(self.__call__, parent)
+        func = functools.partial(self.__call__, parent)
+        return functools.update_wrapper(func, self.func)
 
     def thread_handler(self, loop, source_task, exc_info, func, *args, **kwargs):
         """
         Wraps the sync application with exception handling.
         """
         # Set the threadlocal for AsyncToSync
         self.threadlocal.main_event_loop = loop
```

### Comparing `asgiref-3.5.2/asgiref/testing.py` & `asgiref-3.6.0/asgiref/testing.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.5.2/asgiref/timeout.py` & `asgiref-3.6.0/asgiref/timeout.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 # https://github.com/aio-libs/async-timeout
 
 # It is vendored here to reduce chain-dependencies on this library, and
 # modified slightly to remove some features we don't use.
 
 
 import asyncio
+import warnings
 from types import TracebackType
-from typing import Any, Optional, Type
+from typing import Any  # noqa
+from typing import Optional, Type
 
 
 class timeout:
     """timeout context manager.
 
     Useful in cases when you want to apply timeout logic around block
     of code or in cases when asyncio.wait_for is not suitable. For example:
@@ -30,15 +32,19 @@
         self,
         timeout: Optional[float],
         *,
         loop: Optional[asyncio.AbstractEventLoop] = None,
     ) -> None:
         self._timeout = timeout
         if loop is None:
-            loop = asyncio.get_event_loop()
+            loop = asyncio.get_running_loop()
+        else:
+            warnings.warn(
+                """The loop argument to timeout() is deprecated.""", DeprecationWarning
+            )
         self._loop = loop
         self._task = None  # type: Optional[asyncio.Task[Any]]
         self._cancelled = False
         self._cancel_handler = None  # type: Optional[asyncio.Handle]
         self._cancel_at = None  # type: Optional[float]
 
     def __enter__(self) -> "timeout":
```

### Comparing `asgiref-3.5.2/asgiref/typing.py` & `asgiref-3.6.0/asgiref/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     "WebSocketScope",
     "LifespanScope",
     "WWWScope",
     "Scope",
     "HTTPRequestEvent",
     "HTTPResponseStartEvent",
     "HTTPResponseBodyEvent",
+    "HTTPResponseTrailersEvent",
     "HTTPServerPushEvent",
     "HTTPDisconnectEvent",
     "WebSocketConnectEvent",
     "WebSocketAcceptEvent",
     "WebSocketReceiveEvent",
     "WebSocketSendEvent",
     "WebSocketResponseStartEvent",
@@ -95,22 +96,29 @@
     more_body: bool
 
 
 class HTTPResponseStartEvent(TypedDict):
     type: Literal["http.response.start"]
     status: int
     headers: Iterable[Tuple[bytes, bytes]]
+    trailers: bool
 
 
 class HTTPResponseBodyEvent(TypedDict):
     type: Literal["http.response.body"]
     body: bytes
     more_body: bool
 
 
+class HTTPResponseTrailersEvent(TypedDict):
+    type: Literal["http.response.trailers"]
+    headers: Iterable[Tuple[bytes, bytes]]
+    more_trailers: bool
+
+
 class HTTPServerPushEvent(TypedDict):
     type: Literal["http.response.push"]
     path: str
     headers: Iterable[Tuple[bytes, bytes]]
 
 
 class HTTPDisconnectEvent(TypedDict):
@@ -198,14 +206,15 @@
     LifespanShutdownEvent,
 ]
 
 
 ASGISendEvent = Union[
     HTTPResponseStartEvent,
     HTTPResponseBodyEvent,
+    HTTPResponseTrailersEvent,
     HTTPServerPushEvent,
     HTTPDisconnectEvent,
     WebSocketAcceptEvent,
     WebSocketSendEvent,
     WebSocketResponseStartEvent,
     WebSocketResponseBodyEvent,
     WebSocketCloseEvent,
```

### Comparing `asgiref-3.5.2/asgiref/wsgi.py` & `asgiref-3.6.0/asgiref/wsgi.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.5.2/asgiref.egg-info/PKG-INFO` & `asgiref-3.6.0/asgiref.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: asgiref
-Version: 3.5.2
+Version: 3.6.0
 Summary: ASGI specs, helper code, and adapters
 Home-page: https://github.com/django/asgiref/
 Author: Django Software Foundation
 Author-email: foundation@djangoproject.com
-License: BSD
+License: BSD-3-Clause
 Project-URL: Documentation, https://asgi.readthedocs.io/
 Project-URL: Further Documentation, https://docs.djangoproject.com/en/stable/topics/async/#async-adapter-functions
 Project-URL: Changelog, https://github.com/django/asgiref/blob/master/CHANGELOG.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.7
 Provides-Extra: tests
 License-File: LICENSE
 
 asgiref
 =======
```

### Comparing `asgiref-3.5.2/asgiref.egg-info/SOURCES.txt` & `asgiref-3.6.0/asgiref.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asgiref-3.5.2/setup.cfg` & `asgiref-3.6.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 name = asgiref
 version = attr: asgiref.__version__
 url = https://github.com/django/asgiref/
 author = Django Software Foundation
 author_email = foundation@djangoproject.com
 description = ASGI specs, helper code, and adapters
 long_description = file: README.rst
-license = BSD
+license = BSD-3-Clause
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Internet :: WWW/HTTP
 project_urls = 
 	Documentation = https://asgi.readthedocs.io/
 	Further Documentation = https://docs.djangoproject.com/en/stable/topics/async/#async-adapter-functions
 	Changelog = https://github.com/django/asgiref/blob/master/CHANGELOG.txt
 
 [options]
```

### Comparing `asgiref-3.5.2/tests/test_compatibility.py` & `asgiref-3.6.0/tests/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.5.2/tests/test_local.py` & `asgiref-3.6.0/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.5.2/tests/test_server.py` & `asgiref-3.6.0/tests/test_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,18 +57,18 @@
     def __init__(self, name):
         self._sock = sock.socket(sock.AF_INET, sock.SOCK_DGRAM)
         self._sock.setblocking(False)
         self.name = name
 
     async def register(self, server_addr, name=None):
         name = name or self.name
-        self._sock.sendto(f"Register {name}".encode("utf-8"), server_addr)
+        self._sock.sendto(f"Register {name}".encode(), server_addr)
 
     async def send(self, server_addr, to, msg):
-        self._sock.sendto(f"To {to} {msg}".encode("utf-8"), server_addr)
+        self._sock.sendto(f"To {to} {msg}".encode(), server_addr)
 
     async def get_msg(self):
         msg, server_addr = await sock_recvfrom(self._sock, 4096)
         return msg, server_addr
 
     def close(self):
         self._sock.close()
```

### Comparing `asgiref-3.5.2/tests/test_sync.py` & `asgiref-3.6.0/tests/test_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 import warnings
 from concurrent.futures import ThreadPoolExecutor
 from functools import wraps
 from unittest import TestCase
 
 import pytest
 
-from asgiref.sync import ThreadSensitiveContext, async_to_sync, sync_to_async
+from asgiref.sync import (
+    ThreadSensitiveContext,
+    async_to_sync,
+    iscoroutinefunction,
+    sync_to_async,
+)
 from asgiref.timeout import timeout
 
 
 @pytest.mark.asyncio
 async def test_sync_to_async():
     """
     Tests we can call sync functions from an async thread
@@ -641,16 +646,16 @@
     """
     Tests that SyncToAsync functions are detected as coroutines.
     """
 
     def sync_func():
         return
 
-    assert not asyncio.iscoroutinefunction(sync_to_async)
-    assert asyncio.iscoroutinefunction(sync_to_async(sync_func))
+    assert not iscoroutinefunction(sync_to_async)
+    assert iscoroutinefunction(sync_to_async(sync_func))
 
 
 async def async_process(queue):
     queue.put(42)
 
 
 def sync_process(queue):
```

### Comparing `asgiref-3.5.2/tests/test_sync_contextvars.py` & `asgiref-3.6.0/tests/test_sync_contextvars.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.5.2/tests/test_testing.py` & `asgiref-3.6.0/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.5.2/tests/test_wsgi.py` & `asgiref-3.6.0/tests/test_wsgi.py`

 * *Files identical despite different names*

