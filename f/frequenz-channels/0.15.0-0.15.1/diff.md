# Comparing `tmp/frequenz-channels-0.15.0.tar.gz` & `tmp/frequenz-channels-0.15.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-channels-0.15.0.tar", last modified: Tue May 16 09:51:44 2023, max compression
+gzip compressed data, was "frequenz-channels-0.15.1.tar", last modified: Tue May 23 14:19:20 2023, max compression
```

## Comparing `frequenz-channels-0.15.0.tar` & `frequenz-channels-0.15.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:51:44.800384 frequenz-channels-0.15.0/
--rw-r--r--   0 runner    (1001) docker     (122)     3497 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-05-16 09:51:44.800384 frequenz-channels-0.15.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:51:44.796384 frequenz-channels-0.15.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/docs/SUMMARY.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:51:44.796384 frequenz-channels-0.15.0/docs/css/
--rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/docs/css/mkdocstrings.css
--rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/docs/css/style.css
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/docs/mkdocstrings_autoapi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:51:44.796384 frequenz-channels-0.15.0/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (122)     2589 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2401 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-16 09:51:44.800384 frequenz-channels-0.15.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:51:44.796384 frequenz-channels-0.15.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:51:44.792384 frequenz-channels-0.15.0/src/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:51:44.796384 frequenz-channels-0.15.0/src/frequenz/channels/
--rw-r--r--   0 runner    (1001) docker     (122)     2771 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7095 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/_anycast.py
--rw-r--r--   0 runner    (1001) docker     (122)     6348 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/_base_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     5710 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/_bidirectional.py
--rw-r--r--   0 runner    (1001) docker     (122)    12090 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/_broadcast.py
--rw-r--r--   0 runner    (1001) docker     (122)     3193 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:51:44.796384 frequenz-channels-0.15.0/src/frequenz/channels/util/
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4259 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/util/_file_watcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     4011 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/util/_merge.py
--rw-r--r--   0 runner    (1001) docker     (122)     3694 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/util/_merge_named.py
--rw-r--r--   0 runner    (1001) docker     (122)     6686 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/util/_select.py
--rw-r--r--   0 runner    (1001) docker     (122)    24885 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/util/_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:51:44.800384 frequenz-channels-0.15.0/src/frequenz_channels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-05-16 09:51:44.000000 frequenz-channels-0.15.0/src/frequenz_channels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      965 2023-05-16 09:51:44.000000 frequenz-channels-0.15.0/src/frequenz_channels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 09:51:44.000000 frequenz-channels-0.15.0/src/frequenz_channels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      205 2023-05-16 09:51:44.000000 frequenz-channels-0.15.0/src/frequenz_channels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-16 09:51:44.000000 frequenz-channels-0.15.0/src/frequenz_channels.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 14:19:20.245454 frequenz-channels-0.15.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     3497 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-05-23 14:19:20.245454 frequenz-channels-0.15.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      539 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 14:19:20.241454 frequenz-channels-0.15.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 14:19:20.241454 frequenz-channels-0.15.1/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/docs/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/docs/mkdocstrings_autoapi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 14:19:20.241454 frequenz-channels-0.15.1/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2589 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2345 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 14:19:20.245454 frequenz-channels-0.15.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 14:19:20.241454 frequenz-channels-0.15.1/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 14:19:20.241454 frequenz-channels-0.15.1/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 14:19:20.245454 frequenz-channels-0.15.1/src/frequenz/channels/
+-rw-r--r--   0 runner    (1001) docker     (122)     2771 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7095 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/_anycast.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6348 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/_base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5710 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/_bidirectional.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12090 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/_broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3193 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 14:19:20.245454 frequenz-channels-0.15.1/src/frequenz/channels/util/
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4251 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/util/_file_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4249 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/util/_merge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3694 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/util/_merge_named.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6924 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/util/_select.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25535 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/util/_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 14:19:20.245454 frequenz-channels-0.15.1/src/frequenz_channels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-05-23 14:19:20.000000 frequenz-channels-0.15.1/src/frequenz_channels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-05-23 14:19:20.000000 frequenz-channels-0.15.1/src/frequenz_channels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 14:19:20.000000 frequenz-channels-0.15.1/src/frequenz_channels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-05-23 14:19:20.000000 frequenz-channels-0.15.1/src/frequenz_channels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-23 14:19:20.000000 frequenz-channels-0.15.1/src/frequenz_channels.egg-info/top_level.txt
```

### Comparing `frequenz-channels-0.15.0/CONTRIBUTING.md` & `frequenz-channels-0.15.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.0/LICENSE` & `frequenz-channels-0.15.1/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.0/PKG-INFO` & `frequenz-channels-0.15.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-channels
-Version: 0.15.0
+Version: 0.15.1
 Summary: Channel implementations for Python
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-channels-python/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-channels-python
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-channels-python/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-channels-python/discussions/categories/support
```

### Comparing `frequenz-channels-0.15.0/README.md` & `frequenz-channels-0.15.1/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.0/docs/css/mkdocstrings.css` & `frequenz-channels-0.15.1/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.0/docs/css/style.css` & `frequenz-channels-0.15.1/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.0/docs/logo.png` & `frequenz-channels-0.15.1/docs/logo.png`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.0/docs/mkdocstrings_autoapi.py` & `frequenz-channels-0.15.1/docs/mkdocstrings_autoapi.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.0/mkdocs.yml` & `frequenz-channels-0.15.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.0/pyproject.toml` & `frequenz-channels-0.15.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 [build-system]
-requires = [
-  "setuptools >= 65.3.0, < 66",
-  "setuptools_scm[toml] >= 7.0.5, < 8",
-  "wheel",
-]
+requires = ["setuptools == 65.3.0", "setuptools_scm[toml] == 7.0.5", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "frequenz-channels"
 description = "Channel implementations for Python"
 readme = "README.md"
@@ -21,29 +17,29 @@
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Topic :: Software Development :: Libraries",
 ]
 requires-python = ">= 3.8, < 4"
-dependencies = ["watchfiles >= 0.15.0"]
+dependencies = ["watchfiles >= 0.15.0, < 0.20.0"]
 dynamic = ["version"]
 
 [[project.authors]]
 name = "Frequenz Energy-as-a-Service GmbH"
 email = "floss@frequenz.com"
 
 [project.optional-dependencies]
 docs = [
-  "mike >= 1.1.2, < 2",
-  "mkdocs-gen-files >= 0.4.0, < 0.5.0",
-  "mkdocs-literate-nav >= 0.4.0, < 0.5.0",
-  "mkdocs-material >= 8.5.7, < 9",
-  "mkdocs-section-index >= 0.3.4, < 0.4.0",
-  "mkdocstrings[python] >= 0.19.0, < 0.20.0",
+  "mike == 1.1.2",
+  "mkdocs-gen-files == 0.5.0",
+  "mkdocs-literate-nav == 0.6.0",
+  "mkdocs-material == 9.1.14",
+  "mkdocs-section-index == 0.3.5",
+  "mkdocstrings[python] == 0.21.2",
 ]
 
 [project.urls]
 Changelog = "https://github.com/frequenz-floss/frequenz-channels-python/releases"
 Repository = "https://github.com/frequenz-floss/frequenz-channels-python"
 Issues = "https://github.com/frequenz-floss/frequenz-channels-python/issues"
 Support = "https://github.com/frequenz-floss/frequenz-channels-python/discussions/categories/support"
```

### Comparing `frequenz-channels-0.15.0/src/frequenz/channels/__init__.py` & `frequenz-channels-0.15.1/src/frequenz/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.0/src/frequenz/channels/_anycast.py` & `frequenz-channels-0.15.1/src/frequenz/channels/_anycast.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.0/src/frequenz/channels/_base_classes.py` & `frequenz-channels-0.15.1/src/frequenz/channels/_base_classes.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.0/src/frequenz/channels/_bidirectional.py` & `frequenz-channels-0.15.1/src/frequenz/channels/_bidirectional.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.0/src/frequenz/channels/_broadcast.py` & `frequenz-channels-0.15.1/src/frequenz/channels/_broadcast.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.0/src/frequenz/channels/_exceptions.py` & `frequenz-channels-0.15.1/src/frequenz/channels/_exceptions.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.0/src/frequenz/channels/util/__init__.py` & `frequenz-channels-0.15.1/src/frequenz/channels/util/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.0/src/frequenz/channels/util/_file_watcher.py` & `frequenz-channels-0.15.1/src/frequenz/channels/util/_file_watcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 """A Channel receiver for watching for new (or modified) files."""
 
 from __future__ import annotations
 
 import asyncio
 import pathlib
+from collections import abc
 from dataclasses import dataclass
 from enum import Enum
 
 from watchfiles import Change, awatch
 from watchfiles.main import FileChange
 
 from .._base_classes import Receiver
@@ -35,27 +36,24 @@
         """The type of change that was observed."""
         path: pathlib.Path
         """The path where the change was observed."""
 
     def __init__(
         self,
         paths: list[pathlib.Path | str],
-        event_types: set[EventType] | None = None,
+        event_types: abc.Iterable[EventType] = frozenset(EventType),
     ) -> None:
         """Create a `FileWatcher` instance.
 
         Args:
             paths: Paths to watch for changes.
-            event_types: Types of events to watch for or `None` to watch for
+            event_types: Types of events to watch for. Defaults to watch for
                 all event types.
         """
-        if event_types is None:
-            event_types = set(FileWatcher.EventType)  # all types
-
-        self.event_types = event_types
+        self.event_types: frozenset[FileWatcher.EventType] = frozenset(event_types)
         self._stop_event = asyncio.Event()
         self._paths = [
             path if isinstance(path, pathlib.Path) else pathlib.Path(path)
             for path in paths
         ]
         self._awatch = awatch(
             *self._paths, stop_event=self._stop_event, watch_filter=self._filter_events
```

### Comparing `frequenz-channels-0.15.0/src/frequenz/channels/util/_merge.py` & `frequenz-channels-0.15.1/src/frequenz/channels/util/_merge.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,21 @@
 
     Example:
         For example, if there are two channel receivers with the same type,
         they can be awaited together, and their results merged into a single
         stream, by using `Merge` like this:
 
         ```python
+        from frequenz.channels import Broadcast
+
+        channel1 = Broadcast[int]("input-chan-1")
+        channel2 = Broadcast[int]("input-chan-2")
+        receiver1 = channel1.new_receiver()
+        receiver2 = channel2.new_receiver()
+
         merge = Merge(receiver1, receiver2)
         while msg := await merge.receive():
             # do something with msg
             pass
         ```
 
         When `merge` is no longer needed, then it should be stopped using
```

### Comparing `frequenz-channels-0.15.0/src/frequenz/channels/util/_merge_named.py` & `frequenz-channels-0.15.1/src/frequenz/channels/util/_merge_named.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.0/src/frequenz/channels/util/_select.py` & `frequenz-channels-0.15.1/src/frequenz/channels/util/_select.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,14 +68,21 @@
     `self.stop()` method. This would cleanup any internal pending async tasks.
 
     Example:
         For example, if there are two receivers that you want to
         simultaneously wait on, this can be done with:
 
         ```python
+        from frequenz.channels import Broadcast
+
+        channel1 = Broadcast[int]("input-chan-1")
+        channel2 = Broadcast[int]("input-chan-2")
+        receiver1 = channel1.new_receiver()
+        receiver2 = channel2.new_receiver()
+
         select = Select(name1 = receiver1, name2 = receiver2)
         while await select.ready():
             if msg := select.name1:
                 if val := msg.inner:
                     # do something with `val`
                     pass
                 else:
```

### Comparing `frequenz-channels-0.15.0/src/frequenz/channels/util/_timer.py` & `frequenz-channels-0.15.1/src/frequenz/channels/util/_timer.py`

 * *Files 6% similar despite different names*

```diff
@@ -283,51 +283,69 @@
             print(f"The timer has triggered {drift=}")
         ```
 
         But you can also use [`Select`][frequenz.channels.util.Select] to combine it
         with other receivers, and even start it (semi) manually:
 
         ```python
+        import logging
+        from frequenz.channels.util import Select
+        from frequenz.channels import Broadcast
+
+        timer = Timer.timeout(timedelta(seconds=1.0), auto_start=False)
+        chan = Broadcast[int]("input-chan")
+        receiver1 = chan.new_receiver()
+
         timer = Timer.timeout(timedelta(seconds=1.0), auto_start=False)
         # Do some other initialization, the timer will start automatically if
         # a message is awaited (or manually via `reset()`).
         select = Select(bat_1=receiver1, timer=timer)
         while await select.ready():
             if msg := select.bat_1:
                 if val := msg.inner:
-                    process_data(val)
+                    battery_soc = val
                 else:
-                    logging.warn("battery channel closed")
+                    logging.warning("battery channel closed")
             elif drift := select.timer:
                 # Print some regular battery data
-                print(f"Battery is charged at {battery.soc}%")
-                if stop_logging:
-                    timer.stop()
-                elif start_logging:
-                    timer.reset()
+                print(f"Battery is charged at {battery_soc}%")
         ```
 
     Example: Timeout example
         ```python
+        import logging
+        from frequenz.channels.util import Select
+        from frequenz.channels import Broadcast
+
+        def process_data(data: int):
+            logging.info("Processing data: %d", data)
+
+        def do_heavy_processing(data: int):
+            logging.info("Heavy processing data: %d", data)
+
         timer = Timer.timeout(timedelta(seconds=1.0), auto_start=False)
+        chan1 = Broadcast[int]("input-chan-1")
+        chan2 = Broadcast[int]("input-chan-2")
+        receiver1 = chan1.new_receiver()
+        receiver2 = chan2.new_receiver()
         select = Select(bat_1=receiver1, heavy_process=receiver2, timeout=timer)
         while await select.ready():
             if msg := select.bat_1:
                 if val := msg.inner:
                     process_data(val)
                     timer.reset()
                 else:
-                    logging.warn("battery channel closed")
+                    logging.warning("battery channel closed")
             if msg := select.heavy_process:
                 if val := msg.inner:
                     do_heavy_processing(val)
                 else:
-                    logging.warn("processing channel closed")
+                    logging.warning("processing channel closed")
             elif drift := select.timeout:
-                logging.warn("No data received in time")
+                logging.warning("No data received in time")
         ```
 
         In this case `do_heavy_processing` might take 2 seconds, and we don't
         want our timeout timer to trigger for the missed ticks, and want the
         next tick to be relative to the time timer was last triggered.
     """
```

### Comparing `frequenz-channels-0.15.0/src/frequenz_channels.egg-info/PKG-INFO` & `frequenz-channels-0.15.1/src/frequenz_channels.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-channels
-Version: 0.15.0
+Version: 0.15.1
 Summary: Channel implementations for Python
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-channels-python/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-channels-python
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-channels-python/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-channels-python/discussions/categories/support
```

### Comparing `frequenz-channels-0.15.0/src/frequenz_channels.egg-info/SOURCES.txt` & `frequenz-channels-0.15.1/src/frequenz_channels.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 docs/SUMMARY.md
 docs/index.md
 docs/logo.png
 docs/mkdocstrings_autoapi.py
 docs/css/mkdocstrings.css
 docs/css/style.css
 docs/overrides/main.html
+src/conftest.py
 src/frequenz/channels/__init__.py
 src/frequenz/channels/_anycast.py
 src/frequenz/channels/_base_classes.py
 src/frequenz/channels/_bidirectional.py
 src/frequenz/channels/_broadcast.py
 src/frequenz/channels/_exceptions.py
 src/frequenz/channels/py.typed
```

