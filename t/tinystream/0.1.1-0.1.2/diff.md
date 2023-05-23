# Comparing `tmp/tinystream-0.1.1.tar.gz` & `tmp/tinystream-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinystream-0.1.1.tar", last modified: Wed May 17 10:32:41 2023, max compression
+gzip compressed data, was "tinystream-0.1.2.tar", last modified: Tue May 23 06:37:48 2023, max compression
```

## Comparing `tinystream-0.1.1.tar` & `tinystream-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-17 10:32:41.782634 tinystream-0.1.1/
--rw-r--r--   0 mikereiche   (502) staff       (20)     1068 2022-11-24 09:19:16.000000 tinystream-0.1.1/LICENSE
--rw-r--r--   0 mikereiche   (502) staff       (20)     4303 2023-05-17 10:32:41.782483 tinystream-0.1.1/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)     4069 2023-05-17 10:25:29.000000 tinystream-0.1.1/README.md
--rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-05-17 10:32:41.782682 tinystream-0.1.1/setup.cfg
--rw-r--r--   0 mikereiche   (502) staff       (20)      490 2023-05-17 10:32:07.000000 tinystream-0.1.1/setup.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-17 10:32:41.782200 tinystream-0.1.1/tinystream.egg-info/
--rw-r--r--   0 mikereiche   (502) staff       (20)     4303 2023-05-17 10:32:41.000000 tinystream-0.1.1/tinystream.egg-info/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)      176 2023-05-17 10:32:41.000000 tinystream-0.1.1/tinystream.egg-info/SOURCES.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-05-17 10:32:41.000000 tinystream-0.1.1/tinystream.egg-info/dependency_links.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       11 2023-05-17 10:32:41.000000 tinystream-0.1.1/tinystream.egg-info/top_level.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)     6713 2023-05-17 10:15:16.000000 tinystream-0.1.1/tinystream.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-23 06:37:48.942941 tinystream-0.1.2/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1068 2022-11-24 09:19:16.000000 tinystream-0.1.2/LICENSE
+-rw-r--r--   0 mikereiche   (502) staff       (20)     4303 2023-05-23 06:37:48.942816 tinystream-0.1.2/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)     4069 2023-05-17 10:25:29.000000 tinystream-0.1.2/README.md
+-rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-05-23 06:37:48.942976 tinystream-0.1.2/setup.cfg
+-rw-r--r--   0 mikereiche   (502) staff       (20)      490 2023-05-23 06:37:15.000000 tinystream-0.1.2/setup.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-23 06:37:48.942648 tinystream-0.1.2/tinystream.egg-info/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     4303 2023-05-23 06:37:48.000000 tinystream-0.1.2/tinystream.egg-info/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)      176 2023-05-23 06:37:48.000000 tinystream-0.1.2/tinystream.egg-info/SOURCES.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-05-23 06:37:48.000000 tinystream-0.1.2/tinystream.egg-info/dependency_links.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       11 2023-05-23 06:37:48.000000 tinystream-0.1.2/tinystream.egg-info/top_level.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)     6826 2023-05-23 06:34:37.000000 tinystream-0.1.2/tinystream.py
```

### Comparing `tinystream-0.1.1/LICENSE` & `tinystream-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tinystream-0.1.1/PKG-INFO` & `tinystream-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinystream
-Version: 0.1.1
+Version: 0.1.2
 Summary: Yet another python streams library
 Home-page: https://github.com/mreiche/python-streams
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Tests Status](https://github.com/mreiche/python-streams/actions/workflows/tests.yml/badge.svg)
```

### Comparing `tinystream-0.1.1/README.md` & `tinystream-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tinystream-0.1.1/tinystream.egg-info/PKG-INFO` & `tinystream-0.1.2/tinystream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinystream
-Version: 0.1.1
+Version: 0.1.2
 Summary: Yet another python streams library
 Home-page: https://github.com/mreiche/python-streams
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Tests Status](https://github.com/mreiche/python-streams/actions/workflows/tests.yml/badge.svg)
```

### Comparing `tinystream-0.1.1/tinystream.py` & `tinystream-0.1.2/tinystream.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,20 @@
             return self
         else:
             return Opt(None)
 
     def map(self, mapper: Mapper[T, R]):
         return Opt[R](mapper(self.__val))
 
-    def if_empty(self, supplier: Supplier[R]):
+    def if_empty(self, supplier: any|Supplier[R]):
         if self.empty:
-            return Opt[R](supplier())
+            if isinstance(supplier, Callable):
+                return Opt[R](supplier())
+            else:
+                return Opt[R](supplier)
         else:
             return self
 
     def type(self, typehint: Type[R]) -> "Opt[R]":
         return self
 
     def filter_type(self, typehint: Type[R]) -> "Opt[R]":
```

