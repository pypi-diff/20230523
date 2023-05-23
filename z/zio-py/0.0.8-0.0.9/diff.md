# Comparing `tmp/zio_py-0.0.8.tar.gz` & `tmp/zio_py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zio_py-0.0.8.tar", last modified: Fri Feb 10 16:48:41 2023, max compression
+gzip compressed data, was "dist/zio_py-0.0.9.tar", last modified: Tue Feb 14 16:51:53 2023, max compression
```

## Comparing `zio_py-0.0.8.tar` & `zio_py-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 harveywi  (1000) harveywi  (1000)        0 2023-02-10 16:48:41.000000 zio_py-0.0.8/
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)    15680 2023-02-10 16:48:41.000000 zio_py-0.0.8/PKG-INFO
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)    13249 2023-02-10 16:37:20.000000 zio_py-0.0.8/README.md
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)       38 2023-02-10 16:48:41.000000 zio_py-0.0.8/setup.cfg
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)      851 2022-08-25 08:41:52.000000 zio_py-0.0.8/setup.py
-drwxr-xr-x   0 harveywi  (1000) harveywi  (1000)        0 2023-02-10 16:48:41.000000 zio_py-0.0.8/zio_py.egg-info/
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)    15680 2023-02-10 16:48:41.000000 zio_py-0.0.8/zio_py.egg-info/PKG-INFO
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)      474 2023-02-10 16:48:41.000000 zio_py-0.0.8/zio_py.egg-info/SOURCES.txt
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)        1 2023-02-10 16:48:41.000000 zio_py-0.0.8/zio_py.egg-info/dependency_links.txt
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)       64 2023-02-10 16:48:41.000000 zio_py-0.0.8/zio_py.egg-info/requires.txt
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)        6 2023-02-10 16:48:41.000000 zio_py-0.0.8/zio_py.egg-info/top_level.txt
-drwxr-xr-x   0 harveywi  (1000) harveywi  (1000)        0 2023-02-10 16:48:41.000000 zio_py-0.0.8/ziopy/
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)        6 2023-02-10 16:24:59.000000 zio_py-0.0.8/ziopy/VERSION
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)        0 2022-08-25 08:41:52.000000 zio_py-0.0.8/ziopy/__init__.py
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)    10393 2023-02-10 16:39:59.000000 zio_py-0.0.8/ziopy/either.py
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)      379 2022-08-25 08:41:52.000000 zio_py-0.0.8/ziopy/environments.py
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)        0 2022-08-25 08:41:52.000000 zio_py-0.0.8/ziopy/py.typed
-drwxr-xr-x   0 harveywi  (1000) harveywi  (1000)        0 2023-02-10 16:48:41.000000 zio_py-0.0.8/ziopy/services/
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)        0 2022-08-25 08:41:52.000000 zio_py-0.0.8/ziopy/services/__init__.py
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)     5074 2022-08-25 08:41:52.000000 zio_py-0.0.8/ziopy/services/console.py
-drwxr-xr-x   0 harveywi  (1000) harveywi  (1000)        0 2023-02-10 16:48:41.000000 zio_py-0.0.8/ziopy/services/mock_effects/
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)        0 2022-08-25 08:41:52.000000 zio_py-0.0.8/ziopy/services/mock_effects/__init__.py
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)      244 2022-08-25 08:41:52.000000 zio_py-0.0.8/ziopy/services/mock_effects/console.py
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)      129 2022-08-25 08:41:52.000000 zio_py-0.0.8/ziopy/services/mock_effects/system.py
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)     1289 2022-08-25 08:41:52.000000 zio_py-0.0.8/ziopy/services/system.py
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)      259 2023-02-10 16:35:20.000000 zio_py-0.0.8/ziopy/util.py
--rw-r--r--   0 harveywi  (1000) harveywi  (1000)    11996 2023-02-10 16:36:57.000000 zio_py-0.0.8/ziopy/zio.py
+drwxr-xr-x   0 harveywi  (1000) harveywi  (1000)        0 2023-02-14 16:51:53.000000 zio_py-0.0.9/
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)    15680 2023-02-14 16:51:53.000000 zio_py-0.0.9/PKG-INFO
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)    13249 2023-02-10 18:19:27.000000 zio_py-0.0.9/README.md
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)       38 2023-02-14 16:51:53.000000 zio_py-0.0.9/setup.cfg
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)      851 2022-08-25 08:41:52.000000 zio_py-0.0.9/setup.py
+drwxr-xr-x   0 harveywi  (1000) harveywi  (1000)        0 2023-02-14 16:51:53.000000 zio_py-0.0.9/zio_py.egg-info/
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)    15680 2023-02-14 16:51:53.000000 zio_py-0.0.9/zio_py.egg-info/PKG-INFO
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)      474 2023-02-14 16:51:53.000000 zio_py-0.0.9/zio_py.egg-info/SOURCES.txt
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)        1 2023-02-14 16:51:53.000000 zio_py-0.0.9/zio_py.egg-info/dependency_links.txt
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)       64 2023-02-14 16:51:53.000000 zio_py-0.0.9/zio_py.egg-info/requires.txt
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)        6 2023-02-14 16:51:53.000000 zio_py-0.0.9/zio_py.egg-info/top_level.txt
+drwxr-xr-x   0 harveywi  (1000) harveywi  (1000)        0 2023-02-14 16:51:53.000000 zio_py-0.0.9/ziopy/
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)        6 2023-02-14 16:49:22.000000 zio_py-0.0.9/ziopy/VERSION
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)        0 2022-08-25 08:41:52.000000 zio_py-0.0.9/ziopy/__init__.py
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)    10938 2023-02-14 16:48:44.000000 zio_py-0.0.9/ziopy/either.py
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)      379 2022-08-25 08:41:52.000000 zio_py-0.0.9/ziopy/environments.py
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)        0 2022-08-25 08:41:52.000000 zio_py-0.0.9/ziopy/py.typed
+drwxr-xr-x   0 harveywi  (1000) harveywi  (1000)        0 2023-02-14 16:51:53.000000 zio_py-0.0.9/ziopy/services/
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)        0 2022-08-25 08:41:52.000000 zio_py-0.0.9/ziopy/services/__init__.py
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)     5074 2022-08-25 08:41:52.000000 zio_py-0.0.9/ziopy/services/console.py
+drwxr-xr-x   0 harveywi  (1000) harveywi  (1000)        0 2023-02-14 16:51:53.000000 zio_py-0.0.9/ziopy/services/mock_effects/
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)        0 2022-08-25 08:41:52.000000 zio_py-0.0.9/ziopy/services/mock_effects/__init__.py
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)      244 2022-08-25 08:41:52.000000 zio_py-0.0.9/ziopy/services/mock_effects/console.py
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)      129 2022-08-25 08:41:52.000000 zio_py-0.0.9/ziopy/services/mock_effects/system.py
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)     1289 2022-08-25 08:41:52.000000 zio_py-0.0.9/ziopy/services/system.py
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)      259 2023-02-10 18:19:27.000000 zio_py-0.0.9/ziopy/util.py
+-rw-r--r--   0 harveywi  (1000) harveywi  (1000)    11996 2023-02-10 18:19:27.000000 zio_py-0.0.9/ziopy/zio.py
```

### Comparing `zio_py-0.0.8/PKG-INFO` & `zio_py-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zio_py
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python port of Scala ZIO for pure functional programming
 Home-page: https://github.com/miiohio/ziopy
 Author: William Harvey
 Author-email: drwjharvey@gmail.com
 License: MIT License
 Description: ZIO-py
         ======
```

### Comparing `zio_py-0.0.8/README.md` & `zio_py-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `zio_py-0.0.8/setup.py` & `zio_py-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `zio_py-0.0.8/zio_py.egg-info/PKG-INFO` & `zio_py-0.0.9/zio_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zio-py
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python port of Scala ZIO for pure functional programming
 Home-page: https://github.com/miiohio/ziopy
 Author: William Harvey
 Author-email: drwjharvey@gmail.com
 License: MIT License
 Description: ZIO-py
         ======
```

### Comparing `zio_py-0.0.8/ziopy/either.py` & `zio_py-0.0.9/ziopy/either.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,14 +116,17 @@
 
     def flat_map(self, f: "Callable[[B], Either[AA, C]]") -> "Either[Union[A, AA], C]":
         return self.match(
             lambda left: left,
             lambda right: f(right.value)
         )
 
+    def __lshift__(self, f: "Callable[[B], Either[AA, C]]") -> "Either[Union[A, AA], C]":
+        return self.flat_map(f)
+
     def flatten(self: "Either[A1, Either[AA, BB]]") -> "Either[Union[A1, AA], BB]":
         return self.flat_map(lambda x: x)
 
     def require(
         self,
         predicate: Callable[[B], bool],
         to_error: Callable[[B], AA]
@@ -280,14 +283,17 @@
 
     def map_left(self, f: Callable[[A], C]) -> "EitherArrow[P, C, B]":
         return EitherArrow(lambda *args, **kwargs: self._f(*args, **kwargs).map_left(f))
 
     def flat_map(self, f: "Callable[[B], Either[AA, C]]") -> "EitherArrow[P, Union[A, AA], C]":
         return EitherArrow(lambda *args, **kwargs: self._f(*args, **kwargs).flat_map(f))
 
+    def __lshift__(self, f: "Callable[[B], Either[AA, C]]") -> "EitherArrow[P, Union[A, AA], C]":
+        return self.flat_map(f)
+
     def flatten(
         self: "EitherArrow[P, A1, Either[AA, BB]]"
     ) -> "EitherArrow[P, Union[A1, AA], BB]":
         return EitherArrow(lambda *args, **kwargs: self._f(*args, **kwargs).flatten())
 
     def require(
         self,
@@ -303,14 +309,22 @@
         predicate: Callable[[B], bool],
         to_error: Callable[[B], X]
     ) -> "EitherArrow[P, A, B]":
         return EitherArrow(
             lambda *args, **kwargs: self._f(*args, **kwargs).asserting(predicate, to_error)
         )
 
+    def or_else(self, other: "EitherArrow[P, AA, BB]") -> "EitherArrow[P, A | AA, B | BB]":
+        return EitherArrow(
+            lambda *args, **kwargs: self._f(*args, **kwargs).match(
+                lambda _: other(*args, **kwargs),
+                lambda a: a
+            )
+        )
+
     def raise_errors(self: "EitherArrow[P, AA, BB]") -> "EitherArrow[P, NoReturn, BB]":
         return EitherArrow(lambda *args, **kwargs: self._f(*args, **kwargs).raise_errors())
 
     def tap(self, op: "Callable[[Either[A, B]], Any]") -> "EitherArrow[P, A, B]":
         return EitherArrow(lambda *args, **kwargs: self._f(*args, **kwargs).tap(op))
 
     def display(self, description: Optional[str] = None) -> "EitherArrow[P, A, B]":
```

### Comparing `zio_py-0.0.8/ziopy/services/console.py` & `zio_py-0.0.9/ziopy/services/console.py`

 * *Files identical despite different names*

### Comparing `zio_py-0.0.8/ziopy/services/system.py` & `zio_py-0.0.9/ziopy/services/system.py`

 * *Files identical despite different names*

### Comparing `zio_py-0.0.8/ziopy/zio.py` & `zio_py-0.0.9/ziopy/zio.py`

 * *Files identical despite different names*

