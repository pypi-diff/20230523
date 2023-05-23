# Comparing `tmp/troncos-3.3.0.tar.gz` & `tmp/troncos-4.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troncos-3.3.0.tar", max compression
+gzip compressed data, was "troncos-4.0.0b1.tar", max compression
```

## Comparing `troncos-3.3.0.tar` & `troncos-4.0.0b1.tar`

### file list

```diff
@@ -1,25 +1,30 @@
--rw-r--r--   0        0        0     1077 2023-05-10 13:08:14.285874 troncos-3.3.0/LICENSE
--rw-r--r--   0        0        0    15818 2023-05-10 13:08:14.285874 troncos-3.3.0/README.md
--rw-r--r--   0        0        0     2326 2023-05-10 13:08:14.289874 troncos-3.3.0/pyproject.toml
--rw-r--r--   0        0        0      291 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/__init__.py
--rw-r--r--   0        0        0     1214 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/_ddlazy/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/frameworks/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/frameworks/asgi/__init__.py
--rw-r--r--   0        0        0     3049 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/frameworks/asgi/middleware.py
--rw-r--r--   0        0        0     3367 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/frameworks/asgi/utils.py
--rw-r--r--   0        0        0      993 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/frameworks/gunicorn/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/frameworks/starlette/__init__.py
--rw-r--r--   0        0        0     4488 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/frameworks/starlette/uvicorn.py
--rw-r--r--   0        0        0        0 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/frameworks/structlog/__init__.py
--rw-r--r--   0        0        0     2222 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/frameworks/structlog/processors.py
--rw-r--r--   0        0        0     5589 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/frameworks/structlog/setup.py
--rw-r--r--   0        0        0     4922 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/logs/__init__.py
--rw-r--r--   0        0        0     3710 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/logs/filters.py
--rw-r--r--   0        0        0     9364 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/logs/formatters.py
--rw-r--r--   0        0        0     3090 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/profiling/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/py.typed
--rw-r--r--   0        0        0    10949 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/traces/__init__.py
--rw-r--r--   0        0        0     7563 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/traces/dd_shim.py
--rw-r--r--   0        0        0     8351 2023-05-10 13:08:14.293874 troncos-3.3.0/troncos/traces/decorate.py
--rw-r--r--   0        0        0     1459 2023-05-10 13:08:14.293874 troncos-3.3.0/troncos/traces/propagation.py
--rw-r--r--   0        0        0    16888 1970-01-01 00:00:00.000000 troncos-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-23 13:42:18.030371 troncos-4.0.0b1/LICENSE
+-rw-r--r--   0        0        0     6047 2023-05-23 13:42:18.030371 troncos-4.0.0b1/README.md
+-rw-r--r--   0        0        0     2195 2023-05-23 13:42:18.030371 troncos-4.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0      291 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/asgi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/asgi/logging/__init__.py
+-rw-r--r--   0        0        0     2606 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/asgi/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/asgi/profiling/__init__.py
+-rw-r--r--   0        0        0      576 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/asgi/profiling/app.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/django/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/django/profiling/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/django/profiling/views.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/starlette/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/starlette/profiling/__init__.py
+-rw-r--r--   0        0        0      291 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/starlette/profiling/views.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/structlog/__init__.py
+-rw-r--r--   0        0        0      705 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/contrib/structlog/processors.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/profiling/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/profiling/auto.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/profiling/bootstrap/__init__.py
+-rw-r--r--   0        0        0      439 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/profiling/bootstrap/profile.py
+-rw-r--r--   0        0        0      343 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/profiling/bootstrap/start.py
+-rw-r--r--   0        0        0     1814 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/profiling/profiler.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/py.typed
+-rw-r--r--   0        0        0      570 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/tracing/__init__.py
+-rw-r--r--   0        0        0     1298 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/tracing/_otel.py
+-rw-r--r--   0        0        0     4062 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/tracing/_span.py
+-rw-r--r--   0        0        0     1672 2023-05-23 13:42:18.034371 troncos-4.0.0b1/troncos/tracing/_writer.py
+-rw-r--r--   0        0        0     6887 1970-01-01 00:00:00.000000 troncos-4.0.0b1/PKG-INFO
```

### Comparing `troncos-3.3.0/LICENSE` & `troncos-4.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `troncos-3.3.0/pyproject.toml` & `troncos-4.0.0b1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [tool.poetry]
 name = "troncos"
-version = "3.3.0"
+version = "4.0.0b1"
 description = "Collection of Python logging, tracing and profiling tools"
 authors = [
     "Guðmundur Björn Birkisson <gudmundur.birkisson@oda.com>",
     "Karl Fredrik Haugland <karlfredrik.haugland@oda.com>",
+    "Eirik Martiniussen Sylliaas <eirik.sylliaas@oda.com>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kolonialno/troncos"
 repository = "https://github.com/kolonialno/troncos"
 documentation = "https://github.com/kolonialno/troncos"
 keywords = ["logs", "traces", "opentelemetry"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
-ddtrace = "1.13.0"
+ddtrace = "1.13.3"
 opentelemetry-sdk = "1.17.0"
-opentelemetry-exporter-otlp-proto-http = {version = "1.17.0", optional = true}
-opentelemetry-exporter-otlp-proto-grpc = {version = "1.17.0", optional = true}
-structlog = {version = ">=22.3,<24.0", optional = true}
+opentelemetry-exporter-otlp-proto-http = "1.17.0"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.1"
 pytest = "^7.2.1"
@@ -32,37 +31,38 @@
 requests = "^2.28.2"
 pytest-cov = "^4.0.0"
 types-requests = "^2.28.11.14"
 pytest-asyncio = ">=0.20.3,<0.22.0"
 django-environ = "^0.9.0"
 pytest-benchmark = "^4.0.0"
 snakeviz = "^2.2.0"
+django = "^4.2.1"
+starlette = "^0.27.0"
+structlog = "^23.1.0"
 
-[tool.poetry.extras]
-http = ["opentelemetry-exporter-otlp-proto-http"]
-grpc = ["opentelemetry-exporter-otlp-proto-grpc"]
-structlog = ["structlog"]
 
 [tool.black]
 target-version = ['py311']
 line-length = 88
 include = '\.pyi?$'
 safe = true
 
 [tool.isort]
 profile = "black"
 skip_gitignore = true
 combine_as_imports = true
 
 [tool.mypy]
 python_version = "3.11"
-strict = true
 files = ["./troncos", "./tests",]
 namespace_packages = true
 show_error_codes = true
+ignore_missing_imports = true
+follow_imports = "normal"
+strict = true
 
 [[tool.mypy.overrides]]
 module = [
     "opentelemetry.sdk.*",
     "opentelemetry.context.*",
 ]
 implicit_reexport = true
```

### Comparing `troncos-3.3.0/troncos/frameworks/asgi/middleware.py` & `troncos-4.0.0b1/troncos/contrib/asgi/logging/middleware.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,42 @@
-import logging
 import time
 from typing import Any, Awaitable, Callable
 
-from troncos._ddlazy import ddlazy
-from troncos.frameworks.asgi.utils import guarantee_single_callable
+try:
+    from structlog import get_logger
+except ImportError:
+    raise RuntimeError(
+        "Structlog must be installed to use the asgi logging middleware."
+    )
 
 
 class AsgiLoggingMiddleware:
     """
     ASGI application middleware that logs requests.
     """
 
     def __init__(
         self,
         app: Any,
         logger_name: str | None = None,
     ) -> None:
-        self._app = guarantee_single_callable(app)
+        self._app = app
         ln = logger_name or "asgi"
-        self._access = logging.getLogger(f"{ln}.access")
-        self._error = logging.getLogger(f"{ln}.error")
+        self._access = get_logger(f"{ln}.access")
+        self._error = get_logger(f"{ln}.error")
 
     async def __call__(
         self,
         scope: dict[str, Any],
         receive: Callable[[Any], Any],
         send: Callable[[dict[str, Any]], Awaitable[Any]],
     ) -> Any:
         if scope["type"] != "http":
             return await self._app(scope, receive, send)
 
-        # Extract tracing context now, because it is not available
-        # when we create the log records!
-        dd_context = (
-            ddlazy.dd_tracer().current_trace_context()
-            if ddlazy.dd_initialized()
-            else None
-        )
-
         client_ip, client_port = scope.get("client", ("NO_IP", -1))
         method = scope.get("method")
         path = scope.get("path")
         http_version = scope.get("http_version")
         status = [0]
         start_time = time.time()
 
@@ -60,33 +55,29 @@
                     "http_client_addr": f"{client_ip}:{client_port}",
                     "http_method": method,
                     "http_path": path,
                     "http_version": http_version,
                     "http_status_code": status[0],
                     "duration": f"{time.time()-start_time:.6f}",
                 }
-                if dd_context:
-                    extra["dd_context"] = dd_context
                 self._access.info(
                     "",
-                    extra=extra,
+                    **extra,
                 )
 
         try:
             return await self._app(scope, receive, wrapped_send)
         except Exception as e:
             extra = {
                 "http_client_addr": f"{client_ip}:{client_port}",
                 "http_method": method,
                 "http_path": path,
                 "http_version": http_version,
                 "http_status_code": 500,
                 "duration": f"{time.time()-start_time:.6f}",
             }
-            if dd_context:
-                extra["dd_context"] = dd_context
-            self._error.error(
+
+            self._error.exception(
                 "",
-                exc_info=e,
-                extra=extra,
+                **extra,
             )
             raise e
```

### Comparing `troncos-3.3.0/troncos/profiling/__init__.py` & `troncos-4.0.0b1/troncos/profiling/profiler.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,83 +1,54 @@
-import logging
-import os
-from typing import Callable, Tuple
+from typing import Any
 
-from troncos._ddlazy import ddlazy
+from ddtrace.profiling import exporter
+from ddtrace.profiling.exporter import pprof  # type: ignore
+from ddtrace.profiling.profiler import (
+    Profiler as DDProfiler,
+    _ProfilerInstance as DDProfilerInstance,
+)
 
-logger = logging.getLogger(__name__)
 
+class _PprofExporter(pprof.PprofExporter):  # type: ignore[misc]
+    pprof = ""
 
-def init_profiling_basic() -> Callable[[], Tuple[str, dict[str, str]]]:
-    """
-    Sets up and enables the continuous profiler.
-
-    :return: A callable that returns the profile data and http headers that
-             phlare is happy with.
-    """
+    @staticmethod
+    def _map_frames(events):  # type: ignore[no-untyped-def]
+        """
+        This function takes the profiling events, and iterates over all the frames,
+        formatting the data for phlare.
+        """
 
-    if not ddlazy.dd_initialized():
-        logger.warning(
-            "If you are also tracing, YOU SHOULD CALL 'init_tracing_basic' "
-            "BEFORE YOU INITIALIZE THE PROFILER"
+        for _, e1 in events.items():
+            for e2 in e1:
+                e2.frames = list(e2.frames)
+                for i in range(len(e2.frames)):
+                    frame = e2.frames[i]
+                    file = frame[0].split("/lib/", 1)[-1]
+                    loc = f"{file}:{frame[1]}:{frame[2]}"
+                    e2.frames[i] = (frame[0], frame[1], loc, frame[3])
+
+    def export(self, events, start_time_ns, end_time_ns):  # type: ignore[no-untyped-def] # noqa: E501
+        self._map_frames(events)  # type: ignore[no-untyped-call]
+        pprof_profile, _ = super(_PprofExporter, self).export(
+            events, start_time_ns, end_time_ns
         )
 
-    # We import ddtrace here because we only want to import
-    # it when this function is called, not when it is imported.
-    import ddtrace
-    from ddtrace.profiling.exporter import pprof  # type: ignore[attr-defined]
-
-    # Define our custom exporter, again ve define this inside the function
-    # so ddtrace does not get imported until the function is called.
-    class _PprofExporter(pprof.PprofExporter):  # type: ignore[misc]
-        pprof = ""
-
-        @staticmethod
-        def _map_frames(events):  # type: ignore[no-untyped-def]
-            """
-            This function takes the profiling events, and iterates over all the frames,
-            formatting the data for phlare.
-            """
-
-            for _, e1 in events.items():
-                for e2 in e1:
-                    e2.frames = list(e2.frames)
-                    for i in range(len(e2.frames)):
-                        frame = e2.frames[i]
-                        file = frame[0].split("/lib/", 1)[-1]
-                        loc = f"{file}:{frame[1]}:{frame[2]}"
-                        e2.frames[i] = (frame[0], frame[1], loc, frame[3])
-
-        def export(self, events, start_time_ns, end_time_ns):  # type: ignore[no-untyped-def] # noqa: E501
-            self._map_frames(events)  # type: ignore[no-untyped-call]
-            pprof_profile, _ = super(_PprofExporter, self).export(
-                events, start_time_ns, end_time_ns
-            )
-            self.pprof = pprof_profile.SerializeToString()
-
-    _endpoint_exporter = _PprofExporter()
-
-    @staticmethod  # type: ignore[misc]
-    def _build_default_exporters():  # type: ignore[no-untyped-def]
-        return [_endpoint_exporter]
-
-    # Monkey patch default exporter func
-    ddtrace.profiling.profiler._ProfilerInstance._build_default_exporters = _build_default_exporters  # type: ignore[assignment] # noqa: 501
-
-    # Set params and enable continuous profiling
-    os.environ.setdefault("DD_PROFILING_UPLOAD_INTERVAL", "14")
-    import ddtrace.profiling.auto  # noqa: E402
+        self.pprof = pprof_profile.SerializeToString()
+
+
+class _ProfilerInstance(DDProfilerInstance):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        self.exporter = _PprofExporter()
+
+        super().__init__(*args, **kwargs)
+
+    def _build_default_exporters(self) -> list[exporter.Exporter]:
+        return [self.exporter]
 
-    # Create function to return
-    def python_pprof() -> Tuple[str, dict[str, str]]:
-        """
-        Returns the pprof content as a string and the headers that should be returned by
-        a http endpoint
-        """
 
-        return _endpoint_exporter.pprof, {
-            "Content-Type": "application/octet-stream",
-            "Content-Disposition": 'attachment; filename="python.pprof"',
-            "X-Content-Type-Options": "nosniff",
-        }
+class Profiler(DDProfiler):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        self._profiler = _ProfilerInstance(*args, **kwargs)
 
-    return python_pprof
+    def get_profile(self) -> str:
+        return self._profiler.exporter.pprof  # type: ignore
```

