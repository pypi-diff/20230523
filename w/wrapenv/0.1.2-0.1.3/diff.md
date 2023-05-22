# Comparing `tmp/wrapenv-0.1.2.tar.gz` & `tmp/wrapenv-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrapenv-0.1.2.tar", max compression
+gzip compressed data, was "wrapenv-0.1.3.tar", max compression
```

## Comparing `wrapenv-0.1.2.tar` & `wrapenv-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      400 2023-05-22 16:45:18.299351 wrapenv-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      373 2023-05-22 16:18:32.987463 wrapenv-0.1.2/README.md
--rw-r--r--   0        0        0      771 2023-05-22 16:45:31.001561 wrapenv-0.1.2/wrapenv/__init__.py
--rw-r--r--   0        0        0    14995 2023-05-22 14:48:59.630931 wrapenv-0.1.2/wrapenv/wrapenv.py
--rw-r--r--   0        0        0     1020 1970-01-01 00:00:00.000000 wrapenv-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      523 2023-05-22 22:48:17.954191 wrapenv-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      828 2023-05-22 22:51:13.479436 wrapenv-0.1.3/README.md
+-rw-r--r--   0        0        0      771 2023-05-22 22:48:26.904357 wrapenv-0.1.3/wrapenv/__init__.py
+-rw-r--r--   0        0        0    14995 2023-05-22 14:48:59.630931 wrapenv-0.1.3/wrapenv/wrapenv.py
+-rw-r--r--   0        0        0     1598 1970-01-01 00:00:00.000000 wrapenv-0.1.3/PKG-INFO
```

### Comparing `wrapenv-0.1.2/wrapenv/__init__.py` & `wrapenv-0.1.3/wrapenv/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 # Copyright:   (c) Anton G. Mueckl (amueckl@chartup.de) 2023
 # Licence:     MIT
 # -------------------------------------------------------------------------------
 
 from .wrapenv import environment, ENVIRONMENT, Function
 __all__ = (environment, ENVIRONMENT, Function)
 
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 __author__ = 'Anton G. Mueckl'
 __license__ = 'MIT'
 __email__ = 'AMueckl@users.noreply.github.com'
```

### Comparing `wrapenv-0.1.2/wrapenv/wrapenv.py` & `wrapenv-0.1.3/wrapenv/wrapenv.py`

 * *Files identical despite different names*

### Comparing `wrapenv-0.1.2/PKG-INFO` & `wrapenv-0.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: wrapenv
-Version: 0.1.2
-Summary: 
+Version: 0.1.3
+Summary: A wrapper for callable functions with environments to register pre- and post-processing functions checks and modifications.
 Home-page: https://github.com/AMueckl/WrapEnv
 Keywords: wrapper,preprocessing,postprocessing
 Author: AMueckl
 Author-email: AMueckl@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -26,7 +26,16 @@
 
 As usual, you can install the package using pip:
 
 ```bash
 pip install wrapenv
 ```
 
+## Usage
+
+The package provides an instance of the class `ENVIRONMENT` that can be used as a decorator for functions that
+are to be wrapped. As the instance is a global variable, it can be used from anywhere in the code (even in other modules).
+
+The example in the [EXAMPLES](examples/README.md) folder demonstrates how to use the `ENVIRONMENT` instance to wrap a 
+function that is to be called in a different environment than the one it was defined in.
+
+
```

