# Comparing `tmp/pelican-granular-signals-1.0.1.tar.gz` & `tmp/pelican_granular_signals-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican-granular-signals-1.0.1.tar", max compression
+gzip compressed data, was "pelican_granular_signals-1.1.0.tar", max compression
```

## Comparing `pelican-granular-signals-1.0.1.tar` & `pelican_granular_signals-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1098 2022-03-31 11:02:17.625828 pelican-granular-signals-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0      782 2022-03-31 11:04:07.201988 pelican-granular-signals-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2630 2022-03-31 11:02:17.625828 pelican-granular-signals-1.0.1/README.rst
--rw-r--r--   0        0        0     1423 2022-03-31 11:02:17.625828 pelican-granular-signals-1.0.1/src/pelican/plugins/granular_signals/__init__.py
--rw-r--r--   0        0        0     3374 2022-03-31 11:04:56.202712 pelican-granular-signals-1.0.1/setup.py
--rw-r--r--   0        0        0     3184 2022-03-31 11:04:56.202712 pelican-granular-signals-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-23 01:10:12.292984 pelican_granular_signals-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      941 2023-05-23 01:10:12.297370 pelican_granular_signals-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2638 2023-05-23 01:10:12.295119 pelican_granular_signals-1.1.0/README.rst
+-rw-r--r--   0        0        0     1465 2023-05-23 01:10:12.299437 pelican_granular_signals-1.1.0/src/pelican/plugins/granular_signals/__init__.py
+-rw-r--r--   0        0        0     3186 1970-01-01 00:00:00.000000 pelican_granular_signals-1.1.0/PKG-INFO
```

### Comparing `pelican-granular-signals-1.0.1/LICENSE.txt` & `pelican_granular_signals-1.1.0/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021-2022 Kurt McKee <contactme@kurtmckee.org>
+Copyright (c) 2021-2023 Kurt McKee <contactme@kurtmckee.org>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pelican-granular-signals-1.0.1/pyproject.toml` & `pelican_granular_signals-1.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,52 @@
 [tool.poetry]
 name = "pelican-granular-signals"
-version = "1.0.1"
+version = "1.1.0"
 description = "Add more granular signals to Pelican."
 authors = ["Kurt McKee <contactme@kurtmckee.org>"]
 license = "MIT"
 packages = [
     { include = "pelican", from = "src" }
 ]
 readme = "README.rst"
 
 [tool.poetry.dependencies]
-python = ">=3.6.2,<4.0"
+python = ">=3.8"
 
-[tool.poetry.dev-dependencies]
-black = "^22.3.0"
-isort = "^5.10.1"
-pre-commit = "^2.13.0"
-tox = "^3.24.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.coverage.run]
 branch = true
+parallel = true
+data_file = ".tox/.coverage-data-files/.coverage"
+source = [
+    "pelican.plugins.granular_signals",
+    "tests",
+]
 
 
 [tool.coverage.paths]
 source = [
     "src",
     "*/site-packages",
 ]
 
 
+[tool.coverage.report]
+fail_under = 100
+
+
 [tool.isort]
 profile = "black"
 known_third_party = "pelican"
 known_first_party = "pelican.plugins.granular_signals"
+
+
+[tool.pytest.ini_options]
+addopts = "--color=yes"
+filterwarnings = [
+    "error",
+]
```

### Comparing `pelican-granular-signals-1.0.1/README.rst` & `pelican_granular_signals-1.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ..  This file is part of the pelican-granular-signals plugin.
-..  Copyright 2021-2022 Kurt McKee <contactme@kurtmckee.org>
+..  Copyright 2021-2023 Kurt McKee <contactme@kurtmckee.org>
 ..  Released under the MIT license.
 
 pelican-granular-signals
 ************************
 
 *Ensure that your Pelican plugin is called at the right time, every time.*
 
@@ -84,8 +84,8 @@
 
 
 
 ..  Links
 ..  =====
 
 ..  _Pelican: https://getpelican.com/
-..  _blinker: https://github.com/jek/blinker
+..  _blinker: https://github.com/pallets-eco/blinker
```

### Comparing `pelican-granular-signals-1.0.1/src/pelican/plugins/granular_signals/__init__.py` & `pelican_granular_signals-1.1.0/src/pelican/plugins/granular_signals/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 # This file is part of the pelican-granular-signals plugin.
-# Copyright 2021-2022 Kurt McKee <contactme@kurtmckee.org>
+# Copyright 2021-2023 Kurt McKee <contactme@kurtmckee.org>
 # Released under the MIT license.
 
+from __future__ import annotations
+
 import functools
-from typing import Any, Callable, List, Tuple
+import typing
 
 import blinker
 import pelican
 
-signal_names: Tuple[str, ...] = (
+signal_names: tuple[str, ...] = (
     "sitemap",
     "optimize",
     "minify",
     "compress",
     "deploy",
 )
 
 
 REGISTERED: bool = False
 
 
-def register():
+def register() -> None:
     """Add additional signals to Pelican.
 
     To help ensure that site finalization plugins can be called in
     the correct order, the ``finalized`` signal is wrapped so that
     additional signals can be sent.
     """
 
     global REGISTERED
     if REGISTERED:
         return
 
     # Create new signals.
-    for signal_name in signal_names:
-        blinker.signal(signal_name)
+    for signal_name_ in signal_names:
+        blinker.signal(signal_name_)
 
     # Create a wrapper for the ``finalized`` signal.
-    def augment_finalized(original_send: Callable) -> Callable:
+    def augment_finalized(original_send: typing.Callable) -> typing.Callable:
         @functools.wraps(original_send)
         def wrapper(sender):
-            results: List[Tuple[Callable, Any]] = original_send(sender)
+            results: list[tuple[typing.Callable, typing.Any]] = original_send(sender)
             for signal_name in signal_names:
                 signal: blinker.base.NamedSignal = blinker.signal(signal_name)
                 results.extend(signal.send(sender))
             return results
 
         return wrapper
```

### Comparing `pelican-granular-signals-1.0.1/PKG-INFO` & `pelican_granular_signals-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pelican-granular-signals
-Version: 1.0.1
+Version: 1.1.0
 Summary: Add more granular signals to Pelican.
 License: MIT
 Author: Kurt McKee
 Author-email: contactme@kurtmckee.org
-Requires-Python: >=3.6.2,<4.0
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 
 ..  This file is part of the pelican-granular-signals plugin.
-..  Copyright 2021-2022 Kurt McKee <contactme@kurtmckee.org>
+..  Copyright 2021-2023 Kurt McKee <contactme@kurtmckee.org>
 ..  Released under the MIT license.
 
 pelican-granular-signals
 ************************
 
 *Ensure that your Pelican plugin is called at the right time, every time.*
 
@@ -100,9 +100,9 @@
 
 
 
 ..  Links
 ..  =====
 
 ..  _Pelican: https://getpelican.com/
-..  _blinker: https://github.com/jek/blinker
+..  _blinker: https://github.com/pallets-eco/blinker
```

