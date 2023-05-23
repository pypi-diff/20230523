# Comparing `tmp/formenergy-observability-0.2.0.tar.gz` & `tmp/formenergy-observability-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formenergy-observability-0.2.0.tar", last modified: Tue Apr 11 14:30:17 2023, max compression
+gzip compressed data, was "formenergy-observability-0.3.0.tar", last modified: Tue May 23 15:56:12 2023, max compression
```

## Comparing `formenergy-observability-0.2.0.tar` & `formenergy-observability-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0      186 2023-01-04 16:50:38.583078 formenergy-observability-0.2.0/.gitignore
--rw-r--r--   0        0        0     2038 2023-01-04 16:51:23.731215 formenergy-observability-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      112 2023-01-04 16:51:23.731215 formenergy-observability-0.2.0/.pypirc
--rw-r--r--   0        0        0     1068 2023-01-04 16:09:14.490252 formenergy-observability-0.2.0/LICENSE
--rw-r--r--   0        0        0     3438 2023-04-11 14:24:18.896172 formenergy-observability-0.2.0/README.md
--rw-r--r--   0        0        0   177939 2023-01-04 16:31:04.090964 formenergy-observability-0.2.0/examples/basics-trace.png
--rwxr-xr-x   0        0        0     2570 2023-01-05 18:19:19.918044 formenergy-observability-0.2.0/examples/basics.py
--rw-r--r--   0        0        0   156173 2023-01-04 16:31:04.090964 formenergy-observability-0.2.0/examples/dagster_job.png
--rw-r--r--   0        0        0     2621 2023-01-05 18:20:20.389334 formenergy-observability-0.2.0/examples/dagster_job.py
--rwxr-xr-x   0        0        0     2040 2023-01-05 18:21:06.057762 formenergy-observability-0.2.0/examples/multithread.py
--rw-r--r--   0        0        0      602 2023-04-11 14:24:25.424182 formenergy-observability-0.2.0/form_observability/__init__.py
--rw-r--r--   0        0        0       61 2023-01-05 16:42:09.235771 formenergy-observability-0.2.0/form_observability/conftest.py
--rw-r--r--   0        0        0     8130 2023-01-05 18:33:53.414215 formenergy-observability-0.2.0/form_observability/context_aware.py
--rw-r--r--   0        0        0      299 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/dagster_otel/__init__.py
--rw-r--r--   0        0        0     8827 2023-04-11 14:25:49.316307 formenergy-observability-0.2.0/form_observability/dagster_otel/otel_ops.py
--rw-r--r--   0        0        0     2352 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/dagster_otel/test_otel_op.py
--rw-r--r--   0        0        0      955 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/dagster_otel/test_timing.py
--rw-r--r--   0        0        0      734 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/dagster_otel/testing.py
--rw-r--r--   0        0        0     1291 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/dagster_otel/timing.py
--rw-r--r--   0        0        0      582 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/dagster_otel/util.py
--rw-r--r--   0        0        0     3701 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/log.py
--rw-r--r--   0        0        0     1422 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/otel_value.py
--rw-r--r--   0        0        0     3239 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/pipeline_setup.py
--rw-r--r--   0        0        0     1572 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/test_context_aware.py
--rw-r--r--   0        0        0      941 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/testing.py
--rw-r--r--   0        0        0     1754 2023-04-11 14:23:41.900116 formenergy-observability-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4503 1970-01-01 00:00:00.000000 formenergy-observability-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-23 15:55:45.341077 formenergy-observability-0.3.0/.gitignore
+-rw-r--r--   0        0        0     2038 2023-01-04 16:51:23.731215 formenergy-observability-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      112 2023-01-04 16:51:23.731215 formenergy-observability-0.3.0/.pypirc
+-rw-r--r--   0        0        0     1068 2023-01-04 16:09:14.490252 formenergy-observability-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3497 2023-05-23 15:52:50.668752 formenergy-observability-0.3.0/README.md
+-rw-r--r--   0        0        0   177939 2023-01-04 16:31:04.090964 formenergy-observability-0.3.0/examples/basics-trace.png
+-rwxr-xr-x   0        0        0     2570 2023-05-09 15:42:12.623237 formenergy-observability-0.3.0/examples/basics.py
+-rw-r--r--   0        0        0   156173 2023-01-04 16:31:04.090964 formenergy-observability-0.3.0/examples/dagster_job.png
+-rw-r--r--   0        0        0     2621 2023-05-17 18:05:51.312379 formenergy-observability-0.3.0/examples/dagster_job.py
+-rwxr-xr-x   0        0        0     1793 2023-05-23 15:52:50.668752 formenergy-observability-0.3.0/examples/linked_traces.py
+-rwxr-xr-x   0        0        0     2040 2023-01-05 18:21:06.057762 formenergy-observability-0.3.0/examples/multithread.py
+-rw-r--r--   0        0        0      602 2023-05-23 15:52:50.668752 formenergy-observability-0.3.0/form_observability/__init__.py
+-rw-r--r--   0        0        0       61 2023-01-05 16:42:09.235771 formenergy-observability-0.3.0/form_observability/conftest.py
+-rw-r--r--   0        0        0     9394 2023-05-23 15:54:38.244987 formenergy-observability-0.3.0/form_observability/context_aware.py
+-rw-r--r--   0        0        0      299 2023-01-05 16:42:09.239771 formenergy-observability-0.3.0/form_observability/dagster_otel/__init__.py
+-rw-r--r--   0        0        0     8827 2023-04-11 14:25:49.316307 formenergy-observability-0.3.0/form_observability/dagster_otel/otel_ops.py
+-rw-r--r--   0        0        0     2344 2023-05-23 15:52:50.668752 formenergy-observability-0.3.0/form_observability/dagster_otel/test_otel_op.py
+-rw-r--r--   0        0        0      955 2023-01-05 16:42:09.239771 formenergy-observability-0.3.0/form_observability/dagster_otel/test_timing.py
+-rw-r--r--   0        0        0      734 2023-01-05 16:42:09.239771 formenergy-observability-0.3.0/form_observability/dagster_otel/testing.py
+-rw-r--r--   0        0        0     1291 2023-01-05 16:42:09.239771 formenergy-observability-0.3.0/form_observability/dagster_otel/timing.py
+-rw-r--r--   0        0        0      582 2023-01-05 16:42:09.239771 formenergy-observability-0.3.0/form_observability/dagster_otel/util.py
+-rw-r--r--   0        0        0     3701 2023-01-05 16:42:09.239771 formenergy-observability-0.3.0/form_observability/log.py
+-rw-r--r--   0        0        0     1422 2023-01-05 16:42:09.239771 formenergy-observability-0.3.0/form_observability/otel_value.py
+-rw-r--r--   0        0        0     3239 2023-01-05 16:42:09.239771 formenergy-observability-0.3.0/form_observability/pipeline_setup.py
+-rw-r--r--   0        0        0     1572 2023-01-05 16:42:09.239771 formenergy-observability-0.3.0/form_observability/test_context_aware.py
+-rw-r--r--   0        0        0      941 2023-01-05 16:42:09.239771 formenergy-observability-0.3.0/form_observability/testing.py
+-rw-r--r--   0        0        0     1754 2023-04-11 14:23:41.900116 formenergy-observability-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4562 1970-01-01 00:00:00.000000 formenergy-observability-0.3.0/PKG-INFO
```

### Comparing `formenergy-observability-0.2.0/.pre-commit-config.yaml` & `formenergy-observability-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.2.0/LICENSE` & `formenergy-observability-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.2.0/README.md` & `formenergy-observability-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 
 ## License
 
 This library is provided under the MIT license, see [LICENSE](LICENSE).
 
 ## Release Notes
 
+*   0.3.0 Add `ContextAwareTracer.start_new_linked_trace`.
 *   0.2.0 Switch to `context.op_handle` and `materialization.metadata` as dict for Dagster 1.2.
 *   0.1.0 Initial external release, including `ContextAwareTracer`, `ctx`, and `@otel_op`.
 
 ## Development
 
 If you contribute, please ensure you and your employer accept [the license](LICENSE) for any of your contributions.
```

### Comparing `formenergy-observability-0.2.0/examples/basics-trace.png` & `formenergy-observability-0.3.0/examples/basics-trace.png`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.2.0/examples/basics.py` & `formenergy-observability-0.3.0/examples/basics.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.2.0/examples/dagster_job.png` & `formenergy-observability-0.3.0/examples/dagster_job.png`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.2.0/examples/dagster_job.py` & `formenergy-observability-0.3.0/examples/dagster_job.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.2.0/examples/multithread.py` & `formenergy-observability-0.3.0/examples/multithread.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.2.0/form_observability/__init__.py` & `formenergy-observability-0.3.0/form_observability/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """OTel tracing/logging tools, emphasizing data pipeline use cases with Dagster."""
 
 #: Semantic versioning number. The three dotted numbers are:
 #: *   Major: breaking API changes, significant feature additions.
 #: *   Minor: standard feature additions and improvements. No breaking changes.
 #: *   Micro: small bug fixes.
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 # Make commonly used symbols importable from form_observability.
 from .context_aware import ContextAwareTracer, ctx
 from .log import OtelSpanEventHandler
 from .otel_value import EventAttrKey, EventAttrValue, SpanName
 from .pipeline_setup import configure
```

### Comparing `formenergy-observability-0.2.0/form_observability/context_aware.py` & `formenergy-observability-0.3.0/form_observability/context_aware.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from contextlib import contextmanager
 import functools
 import platform
 import threading
 from typing import Optional, Any, Dict
 
 import opentelemetry
+from opentelemetry.trace import Context, Link
 
 from form_observability.otel_value import (
     EventAttrKey,
     EventAttrValue,
     SpanName,
 )
 
@@ -238,7 +239,39 @@
         span_attrs.update(attributes)
         with ctx.set(attributes or {}), self._tracer.start_as_current_span(
             _convert_types(name),
             attributes=_filter_attributes(span_attrs),
             **kwargs,
         ) as span:
             yield span
+
+    @contextmanager
+    def start_new_linked_trace(
+        self,
+        name: str,
+        **kwargs,
+    ):
+        """Starts a new root span with start_as_current_span, linked to the current trace.
+
+        The new root span will have a link back to the previously active trace, but will
+        not appear as a child span. This helps avoid very large/complex traces.
+
+        This does not reset the _ObservabilityContext.
+
+        :return: The trace context of the new trace.
+        """
+        if "context" in kwargs:
+            raise ValueError("Cannot specify context when starting new trace.")
+        # Record the current context, to be added as a link.
+        orig_context = opentelemetry.trace.get_current_span().get_span_context()
+        # Include a link back to the old trace. Allow other links to be passed in too.
+        links = kwargs.get("links", [])
+        links.append(Link(orig_context))
+        kwargs["links"] = links
+        with self.start_as_current_span(
+            name,
+            # Start a fresh trace context.
+            context=Context(),
+            **kwargs,
+        ) as child_span:
+            child_context = child_span.get_span_context()
+            yield child_context
```

### Comparing `formenergy-observability-0.2.0/form_observability/dagster_otel/otel_ops.py` & `formenergy-observability-0.3.0/form_observability/dagster_otel/otel_ops.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.2.0/form_observability/dagster_otel/test_otel_op.py` & `formenergy-observability-0.3.0/form_observability/dagster_otel/test_otel_op.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,22 +17,22 @@
     _set_trace_context,
 )
 from form_observability.dagster_otel.testing import noop_resource
 
 
 def test_publish_trace_context_logs_asset(mock_get_current_span):
     mock_context = MagicMock(spec=OpExecutionContext)
-    mock_context.solid_handle.path = ["main_graph", "subgraph", "my_op"]
+    mock_context.op_handle.path = ["main_graph", "subgraph", "my_op"]
 
     publish_current_trace_context(mock_context)
 
     mock_context.log_event.assert_called_once()
     first_call = mock_context.log_event.call_args_list[0]
     materialization = first_call[0][0]  # first arg from the call's args list
-    assert "traceparent" in materialization.metadata_entries[0].entry_data.data
+    assert "traceparent" in materialization.metadata["trace_context"].data
     assert materialization.asset_key.path[0] == "main_graph.subgraph"
 
 
 def test_otel_op_finds_trace_context_and_catches_exception():
     @op
     def root_trace_context_op(context):
         publish_current_trace_context(context)
```

### Comparing `formenergy-observability-0.2.0/form_observability/dagster_otel/test_timing.py` & `formenergy-observability-0.3.0/form_observability/dagster_otel/test_timing.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.2.0/form_observability/dagster_otel/testing.py` & `formenergy-observability-0.3.0/form_observability/dagster_otel/testing.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.2.0/form_observability/dagster_otel/timing.py` & `formenergy-observability-0.3.0/form_observability/dagster_otel/timing.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.2.0/form_observability/dagster_otel/util.py` & `formenergy-observability-0.3.0/form_observability/dagster_otel/util.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.2.0/form_observability/log.py` & `formenergy-observability-0.3.0/form_observability/log.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.2.0/form_observability/otel_value.py` & `formenergy-observability-0.3.0/form_observability/otel_value.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.2.0/form_observability/pipeline_setup.py` & `formenergy-observability-0.3.0/form_observability/pipeline_setup.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.2.0/form_observability/test_context_aware.py` & `formenergy-observability-0.3.0/form_observability/test_context_aware.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.2.0/form_observability/testing.py` & `formenergy-observability-0.3.0/form_observability/testing.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.2.0/pyproject.toml` & `formenergy-observability-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.2.0/PKG-INFO` & `formenergy-observability-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formenergy-observability
-Version: 0.2.0
+Version: 0.3.0
 Summary: OTel tracing/logging tools, emphasizing data pipeline use cases with Dagster.
 Author-email: Form Energy Software <software@formenergy.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -91,14 +91,15 @@
 
 ## License
 
 This library is provided under the MIT license, see [LICENSE](LICENSE).
 
 ## Release Notes
 
+*   0.3.0 Add `ContextAwareTracer.start_new_linked_trace`.
 *   0.2.0 Switch to `context.op_handle` and `materialization.metadata` as dict for Dagster 1.2.
 *   0.1.0 Initial external release, including `ContextAwareTracer`, `ctx`, and `@otel_op`.
 
 ## Development
 
 If you contribute, please ensure you and your employer accept [the license](LICENSE) for any of your contributions.
```

