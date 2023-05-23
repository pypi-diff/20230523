# Comparing `tmp/serverless-sdk-0.4.8.tar.gz` & `tmp/serverless-sdk-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-ukj8y1ml/serverless-sdk-0.4.8.tar", last modified: Mon May 15 13:10:42 2023, max compression
+gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-s5iy1w2o/serverless-sdk-0.4.9.tar", last modified: Thu May 18 09:11:23 2023, max compression
```

## Comparing `serverless-sdk-0.4.8.tar` & `serverless-sdk-0.4.9.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/serverless_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/serverless_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/serverless_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/serverless_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/serverless_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/serverless_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/serverless_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/serverless_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/sls_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/sls_sdk/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/error_captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/notice.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/stack_trace_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/lib/warning_captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/sls_sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:42.000000 serverless-sdk-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/tests/test_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/tests/test_sdk_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-05-15 13:10:18.000000 serverless-sdk-0.4.8/tests/test_thread_safety.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/serverless_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/serverless_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/serverless_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/serverless_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/serverless_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/serverless_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/serverless_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/serverless_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/sls_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/sls_sdk/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/error_captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/notice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/stack_trace_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/lib/warning_captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/sls_sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:23.000000 serverless-sdk-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/tests/test_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/tests/test_sdk_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-05-18 09:11:05.000000 serverless-sdk-0.4.9/tests/test_thread_safety.py
```

### Comparing `serverless-sdk-0.4.8/PKG-INFO` & `serverless-sdk-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.4.8
+Version: 0.4.9
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `serverless-sdk-0.4.8/README.md` & `serverless-sdk-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.8/pyproject.toml` & `serverless-sdk-0.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.8/serverless_sdk.egg-info/PKG-INFO` & `serverless-sdk-0.4.9/serverless_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.4.8
+Version: 0.4.9
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `serverless-sdk-0.4.8/serverless_sdk.egg-info/SOURCES.txt` & `serverless-sdk-0.4.9/serverless_sdk.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 sls_sdk/py.typed
 sls_sdk/lib/__init__.py
 sls_sdk/lib/captured_event.py
 sls_sdk/lib/emitter.py
 sls_sdk/lib/error.py
 sls_sdk/lib/error_captured_event.py
 sls_sdk/lib/id.py
+sls_sdk/lib/imports.py
 sls_sdk/lib/name.py
 sls_sdk/lib/notice.py
 sls_sdk/lib/stack_trace_string.py
 sls_sdk/lib/tags.py
 sls_sdk/lib/timing.py
 sls_sdk/lib/trace.py
 sls_sdk/lib/warning.py
```

### Comparing `serverless-sdk-0.4.8/sls_sdk/__init__.py` & `serverless-sdk-0.4.9/sls_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.8/sls_sdk/base.py` & `serverless-sdk-0.4.9/sls_sdk/base.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.8/sls_sdk/exceptions.py` & `serverless-sdk-0.4.9/sls_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.8/sls_sdk/lib/captured_event.py` & `serverless-sdk-0.4.9/sls_sdk/lib/captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.8/sls_sdk/lib/emitter.py` & `serverless-sdk-0.4.9/sls_sdk/lib/emitter.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.8/sls_sdk/lib/error.py` & `serverless-sdk-0.4.9/sls_sdk/lib/error.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.8/sls_sdk/lib/error_captured_event.py` & `serverless-sdk-0.4.9/sls_sdk/lib/error_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/flask.py` & `serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/flask.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/http.py` & `serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/http.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/import_hook.py` & `serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/import_hook.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/logging.py` & `serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/logging.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.8/sls_sdk/lib/instrumentation/wrapper.py` & `serverless-sdk-0.4.9/sls_sdk/lib/instrumentation/wrapper.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.8/sls_sdk/lib/name.py` & `serverless-sdk-0.4.9/sls_sdk/lib/name.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
-
 from re import Pattern
+from .imports import internally_imported
 
-from js_regex import compile
-from typing_extensions import Final
+with internally_imported("js_regex"):
+    from js_regex import compile
 
+from typing_extensions import Final
 from ..exceptions import InvalidTraceSpanName
 
 
 # from https://github.com/serverless/console/blob/main/node/packages/sdk/lib/get-ensure-resource-name.js#L7
 RE: Final[str] = (
     r"^[a-z][a-z0-9]*"
     r"(?:_[a-z][a-z0-9]*)*"
```

### Comparing `serverless-sdk-0.4.8/sls_sdk/lib/stack_trace_string.py` & `serverless-sdk-0.4.9/sls_sdk/lib/stack_trace_string.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.8/sls_sdk/lib/tags.py` & `serverless-sdk-0.4.9/sls_sdk/lib/tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from __future__ import annotations
 import re
 from datetime import datetime
 from math import inf, nan
 from re import Pattern
 from typing import Dict, List, Mapping, Tuple, Optional, Any
-from js_regex import compile
+from .imports import internally_imported
+
+with internally_imported("js_regex"):
+    from js_regex import compile
+
 from typing_extensions import Final, get_args
 from threading import Lock
 from .error import report as report_error
 from ..base import TagType, ValidTags
 from ..exceptions import (
     DuplicateTraceSpanName,
     InvalidTraceSpanTagName,
```

### Comparing `serverless-sdk-0.4.8/sls_sdk/lib/trace.py` & `serverless-sdk-0.4.9/sls_sdk/lib/trace.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.8/sls_sdk/lib/warning.py` & `serverless-sdk-0.4.9/sls_sdk/lib/warning.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.8/sls_sdk/lib/warning_captured_event.py` & `serverless-sdk-0.4.9/sls_sdk/lib/warning_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.8/tests/test_sdk.py` & `serverless-sdk-0.4.9/tests/test_sdk.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.8/tests/test_thread_safety.py` & `serverless-sdk-0.4.9/tests/test_thread_safety.py`

 * *Files identical despite different names*

