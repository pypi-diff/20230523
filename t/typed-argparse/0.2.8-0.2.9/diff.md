# Comparing `tmp/typed-argparse-0.2.8.tar.gz` & `tmp/typed-argparse-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typed-argparse-0.2.8.tar", last modified: Tue Dec 20 00:49:56 2022, max compression
+gzip compressed data, was "typed-argparse-0.2.9.tar", last modified: Sat Dec 24 13:50:20 2022, max compression
```

## Comparing `typed-argparse-0.2.8.tar` & `typed-argparse-0.2.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 00:49:56.469582 typed-argparse-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2022-12-20 00:49:52.000000 typed-argparse-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-20 00:49:52.000000 typed-argparse-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2022-12-20 00:49:56.469582 typed-argparse-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2022-12-20 00:49:52.000000 typed-argparse-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2022-12-20 00:49:52.000000 typed-argparse-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2022-12-20 00:49:56.469582 typed-argparse-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      297 2022-12-20 00:49:52.000000 typed-argparse-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 00:49:56.469582 typed-argparse-0.2.8/typed_argparse/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2022-12-20 00:49:52.000000 typed-argparse-0.2.8/typed_argparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2022-12-20 00:49:52.000000 typed-argparse-0.2.8/typed_argparse/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2022-12-20 00:49:52.000000 typed-argparse-0.2.8/typed_argparse/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2022-12-20 00:49:52.000000 typed-argparse-0.2.8/typed_argparse/dataclass_transform_backport.py
--rw-r--r--   0 runner    (1001) docker     (123)    20083 2022-12-20 00:49:52.000000 typed-argparse-0.2.8/typed_argparse/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 00:49:52.000000 typed-argparse-0.2.8/typed_argparse/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2022-12-20 00:49:52.000000 typed-argparse-0.2.8/typed_argparse/runtime_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12160 2022-12-20 00:49:52.000000 typed-argparse-0.2.8/typed_argparse/type_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2022-12-20 00:49:52.000000 typed-argparse-0.2.8/typed_argparse/typed_args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 00:49:56.469582 typed-argparse-0.2.8/typed_argparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2022-12-20 00:49:56.000000 typed-argparse-0.2.8/typed_argparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2022-12-20 00:49:56.000000 typed-argparse-0.2.8/typed_argparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 00:49:56.000000 typed-argparse-0.2.8/typed_argparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-20 00:49:56.000000 typed-argparse-0.2.8/typed_argparse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-20 00:49:56.000000 typed-argparse-0.2.8/typed_argparse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 13:50:20.834559 typed-argparse-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2022-12-24 13:50:16.000000 typed-argparse-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-24 13:50:16.000000 typed-argparse-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2022-12-24 13:50:20.834559 typed-argparse-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2022-12-24 13:50:16.000000 typed-argparse-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2022-12-24 13:50:16.000000 typed-argparse-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2022-12-24 13:50:20.834559 typed-argparse-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2022-12-24 13:50:16.000000 typed-argparse-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 13:50:20.834559 typed-argparse-0.2.9/typed_argparse/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2022-12-24 13:50:16.000000 typed-argparse-0.2.9/typed_argparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2022-12-24 13:50:16.000000 typed-argparse-0.2.9/typed_argparse/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2022-12-24 13:50:16.000000 typed-argparse-0.2.9/typed_argparse/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2022-12-24 13:50:16.000000 typed-argparse-0.2.9/typed_argparse/dataclass_transform_backport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20148 2022-12-24 13:50:16.000000 typed-argparse-0.2.9/typed_argparse/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-24 13:50:16.000000 typed-argparse-0.2.9/typed_argparse/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2022-12-24 13:50:16.000000 typed-argparse-0.2.9/typed_argparse/runtime_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12160 2022-12-24 13:50:16.000000 typed-argparse-0.2.9/typed_argparse/type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2022-12-24 13:50:16.000000 typed-argparse-0.2.9/typed_argparse/typed_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 13:50:20.834559 typed-argparse-0.2.9/typed_argparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2022-12-24 13:50:20.000000 typed-argparse-0.2.9/typed_argparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2022-12-24 13:50:20.000000 typed-argparse-0.2.9/typed_argparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-24 13:50:20.000000 typed-argparse-0.2.9/typed_argparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-24 13:50:20.000000 typed-argparse-0.2.9/typed_argparse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-24 13:50:20.000000 typed-argparse-0.2.9/typed_argparse.egg-info/top_level.txt
```

### Comparing `typed-argparse-0.2.8/LICENSE` & `typed-argparse-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `typed-argparse-0.2.8/PKG-INFO` & `typed-argparse-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typed-argparse
-Version: 0.2.8
+Version: 0.2.9
 Summary: Write type-safe and elegant CLIs with a clear separation of concerns.
 Home-page: https://typed-argparse.github.io/typed-argparse/
 License: MIT
 Project-URL: Source, https://github.com/typed-argparse/typed-argparse
 Description: # typed-argparse
         
         💡 write type-safe and elegant CLIs with a clear separation of concerns.
```

### Comparing `typed-argparse-0.2.8/README.md` & `typed-argparse-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `typed-argparse-0.2.8/setup.cfg` & `typed-argparse-0.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `typed-argparse-0.2.8/typed_argparse/__init__.py` & `typed-argparse-0.2.9/typed_argparse/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .arg import Arg, arg
 from .choices import Choices, get_choices_from, get_choices_from_class
 from .parser import Binding, Bindings, Parser, SubParser, SubParserGroup
 from .typed_args import TypedArgs, WithUnionType, validate_type_union
 
-VERSION = "0.2.8"
+VERSION = "0.2.9"
 
 __all__ = [
     "Choices",
     "TypedArgs",
     "WithUnionType",
     "get_choices_from",
     "get_choices_from_class",
```

### Comparing `typed-argparse-0.2.8/typed_argparse/arg.py` & `typed-argparse-0.2.9/typed_argparse/arg.py`

 * *Files identical despite different names*

### Comparing `typed-argparse-0.2.8/typed_argparse/choices.py` & `typed-argparse-0.2.9/typed_argparse/choices.py`

 * *Files identical despite different names*

### Comparing `typed-argparse-0.2.8/typed_argparse/dataclass_transform_backport.py` & `typed-argparse-0.2.9/typed_argparse/dataclass_transform_backport.py`

 * *Files identical despite different names*

### Comparing `typed-argparse-0.2.8/typed_argparse/parser.py` & `typed-argparse-0.2.9/typed_argparse/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 import argparse
 import sys
 from argparse import ArgumentParser as ArgparseParser
-from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Type, TypeVar, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Set,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+    get_type_hints,
+)
 
 from typing_extensions import assert_never
 
 from .arg import Arg
 from .arg import arg as make_arg
 from .choices import Choices
 from .type_utils import TypeAnnotation, collect_type_annotations
@@ -25,15 +37,15 @@
         self.func: Callable[[Any], None] = func
 
     @staticmethod
     def from_func(func: Callable[[Any], None]) -> "Binding":
         if not hasattr(func, "__annotations__"):
             raise ValueError(f"Function {func.__name__} misses type annotations.")
 
-        annotations = func.__annotations__
+        annotations = get_type_hints(func)
 
         if len(annotations) == 0:
             raise ValueError(f"Type annotations of {func.__name__} are empty.")
 
         first_type: object = next(iter(annotations.values()))
 
         if not isinstance(first_type, type):
```

### Comparing `typed-argparse-0.2.8/typed_argparse/runtime_generic.py` & `typed-argparse-0.2.9/typed_argparse/runtime_generic.py`

 * *Files identical despite different names*

### Comparing `typed-argparse-0.2.8/typed_argparse/type_utils.py` & `typed-argparse-0.2.9/typed_argparse/type_utils.py`

 * *Files identical despite different names*

### Comparing `typed-argparse-0.2.8/typed_argparse/typed_args.py` & `typed-argparse-0.2.9/typed_argparse/typed_args.py`

 * *Files identical despite different names*

### Comparing `typed-argparse-0.2.8/typed_argparse.egg-info/PKG-INFO` & `typed-argparse-0.2.9/typed_argparse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typed-argparse
-Version: 0.2.8
+Version: 0.2.9
 Summary: Write type-safe and elegant CLIs with a clear separation of concerns.
 Home-page: https://typed-argparse.github.io/typed-argparse/
 License: MIT
 Project-URL: Source, https://github.com/typed-argparse/typed-argparse
 Description: # typed-argparse
         
         💡 write type-safe and elegant CLIs with a clear separation of concerns.
```

### Comparing `typed-argparse-0.2.8/typed_argparse.egg-info/SOURCES.txt` & `typed-argparse-0.2.9/typed_argparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

