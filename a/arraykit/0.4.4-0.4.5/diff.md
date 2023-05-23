# Comparing `tmp/arraykit-0.4.4.tar.gz` & `tmp/arraykit-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraykit-0.4.4.tar", last modified: Mon May 22 23:19:03 2023, max compression
+gzip compressed data, was "arraykit-0.4.5.tar", last modified: Tue May 23 13:04:19 2023, max compression
```

## Comparing `arraykit-0.4.4.tar` & `arraykit-0.4.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:19:03.500360 arraykit-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-22 23:18:54.000000 arraykit-0.4.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-22 23:18:54.000000 arraykit-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-22 23:19:03.496360 arraykit-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-22 23:18:54.000000 arraykit-0.4.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:19:03.496360 arraykit-0.4.4/arraykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-22 23:19:03.000000 arraykit-0.4.4/arraykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-22 23:19:03.000000 arraykit-0.4.4/arraykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 23:19:03.000000 arraykit-0.4.4/arraykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 23:19:03.000000 arraykit-0.4.4/arraykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 23:19:03.000000 arraykit-0.4.4/arraykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 23:19:03.500360 arraykit-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-22 23:18:54.000000 arraykit-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:19:03.496360 arraykit-0.4.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-22 23:18:54.000000 arraykit-0.4.4/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   189205 2023-05-22 23:18:54.000000 arraykit-0.4.4/src/_arraykit.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:19:03.496360 arraykit-0.4.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-22 23:18:54.000000 arraykit-0.4.4/test/test_array_go.py
--rw-r--r--   0 runner    (1001) docker     (123)    26033 2023-05-22 23:18:54.000000 arraykit-0.4.4/test/test_block_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    49054 2023-05-22 23:18:54.000000 arraykit-0.4.4/test/test_delimited_to_arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-22 23:18:54.000000 arraykit-0.4.4/test/test_delimited_to_arrays_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-22 23:18:54.000000 arraykit-0.4.4/test/test_delimited_to_arrays_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-22 23:18:54.000000 arraykit-0.4.4/test/test_pyi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-22 23:18:54.000000 arraykit-0.4.4/test/test_split_after_count.py
--rw-r--r--   0 runner    (1001) docker     (123)    28073 2023-05-22 23:18:54.000000 arraykit-0.4.4/test/test_type_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    27668 2023-05-22 23:18:54.000000 arraykit-0.4.4/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:04:19.330720 arraykit-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-23 13:04:12.000000 arraykit-0.4.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-23 13:04:12.000000 arraykit-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-23 13:04:19.330720 arraykit-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-23 13:04:12.000000 arraykit-0.4.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:04:19.326720 arraykit-0.4.5/arraykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-23 13:04:19.000000 arraykit-0.4.5/arraykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-23 13:04:19.000000 arraykit-0.4.5/arraykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:04:19.000000 arraykit-0.4.5/arraykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 13:04:19.000000 arraykit-0.4.5/arraykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 13:04:19.000000 arraykit-0.4.5/arraykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:04:19.330720 arraykit-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-23 13:04:12.000000 arraykit-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:04:19.330720 arraykit-0.4.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-23 13:04:12.000000 arraykit-0.4.5/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   189270 2023-05-23 13:04:12.000000 arraykit-0.4.5/src/_arraykit.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:04:19.330720 arraykit-0.4.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-23 13:04:12.000000 arraykit-0.4.5/test/test_array_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27208 2023-05-23 13:04:12.000000 arraykit-0.4.5/test/test_block_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49054 2023-05-23 13:04:12.000000 arraykit-0.4.5/test/test_delimited_to_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-23 13:04:12.000000 arraykit-0.4.5/test/test_delimited_to_arrays_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-23 13:04:12.000000 arraykit-0.4.5/test/test_delimited_to_arrays_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-23 13:04:12.000000 arraykit-0.4.5/test/test_pyi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-23 13:04:12.000000 arraykit-0.4.5/test/test_split_after_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28073 2023-05-23 13:04:12.000000 arraykit-0.4.5/test/test_type_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27668 2023-05-23 13:04:12.000000 arraykit-0.4.5/test/test_util.py
```

### Comparing `arraykit-0.4.4/LICENSE.txt` & `arraykit-0.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.4/PKG-INFO` & `arraykit-0.4.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arraykit
-Version: 0.4.4
+Version: 0.4.5
 Summary: Array utilities for StaticFrame
 Home-page: https://github.com/static-frame/arraykit
 Author: Christopher Ariza, Brandt Bucher, Charles Burkland
 License: MIT
 Description: The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
         
         Code: https://github.com/static-frame/arraykit
```

### Comparing `arraykit-0.4.4/README.rst` & `arraykit-0.4.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,20 @@
 - NumPy >= 1.18.5
 
 
 
 What is New in ArrayKit
 -------------------------
 
+0.4.5
+............
+
+Corrected handling of ``ascending`` in ``BlockIndex.iter_contiguous()`` with Boolean arrays.
+
+
 0.4.4
 ............
 
 Corrected deallocation routines in ``BlockIndex.iter_contiguous()``.
 
 
 0.4.3
```

### Comparing `arraykit-0.4.4/arraykit.egg-info/PKG-INFO` & `arraykit-0.4.5/arraykit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arraykit
-Version: 0.4.4
+Version: 0.4.5
 Summary: Array utilities for StaticFrame
 Home-page: https://github.com/static-frame/arraykit
 Author: Christopher Ariza, Brandt Bucher, Charles Burkland
 License: MIT
 Description: The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
         
         Code: https://github.com/static-frame/arraykit
```

### Comparing `arraykit-0.4.4/setup.py` & `arraykit-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import site
 import os
 import typing as tp
 from setuptools import Extension  # type: ignore
 from setuptools import setup
 from pathlib import Path
 
-AK_VERSION = '0.4.4'
+AK_VERSION = '0.4.5'
 
 def get_long_description() -> str:
     return '''The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
 
 Code: https://github.com/static-frame/arraykit
 
 Packages: https://pypi.org/project/arraykit
```

### Comparing `arraykit-0.4.4/src/__init__.py` & `arraykit-0.4.5/src/__init__.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.4/src/_arraykit.c` & `arraykit-0.4.5/src/_arraykit.c`

 * *Files 0% similar despite different names*

```diff
@@ -4881,26 +4881,29 @@
             }
             else {
                 PyErr_SetString(PyExc_TypeError, "Arrays kind not supported");
                 return NULL;
             }
         }
         else if (kind == BIIS_SEQ && k != 'i' && k != 'u') {
-            PyErr_SetString(PyExc_TypeError, "Arrays must integer kind");
+            PyErr_SetString(PyExc_TypeError, "Arrays must be integer kind");
             return NULL;
         }
         else if (kind == BIIS_BOOLEAN && k != 'b') {
-            PyErr_SetString(PyExc_TypeError, "Arrays must Boolean kind");
+            PyErr_SetString(PyExc_TypeError, "Arrays must be Boolean kind");
             return NULL;
         }
-        if (kind == BIIS_BOOLEAN && len != bi->bir_count) {
-            PyErr_SetString(PyExc_TypeError, "Boolean arrays must match BlockIndex size");
-            return NULL;
+
+        if (kind == BIIS_BOOLEAN) {
+            if (len != bi->bir_count) {
+                PyErr_SetString(PyExc_TypeError, "Boolean arrays must match BlockIndex size");
+                return NULL;
+            }
         }
-        if (ascending) {
+        else if (ascending) { // not Boolean
             // NOTE: we can overwrite selector here as we have a borrowed refernce; sorting gives us a new reference, so we do not need to incref below
             selector = PyArray_NewCopy(a, NPY_CORDER);
             // sort in-place; can use a non-stable sort
             if (PyArray_Sort((PyArrayObject*)selector, 0, NPY_QUICKSORT)) {
                 return NULL; // returns -1 on error
             }; // new ref
             incref_selector = false;
```

### Comparing `arraykit-0.4.4/test/test_array_go.py` & `arraykit-0.4.5/test/test_array_go.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.4/test/test_block_index.py` & `arraykit-0.4.5/test/test_block_index.py`

 * *Files 3% similar despite different names*

```diff
@@ -757,7 +757,40 @@
         bi1 = BlockIndex()
         bi1.register(np.arange(6).reshape(2,3))
         bi1.register(np.arange(6).reshape(2,3))
         bi1.register(np.arange(4).reshape(2,2))
 
         with self.assertRaises(TypeError):
             _ = list(bi1.iter_contiguous('a'))
+
+
+    def test_block_index_iter_contiguous_h1(self) -> None:
+        bi1 = BlockIndex()
+        bi1.register(np.arange(6).reshape(2,3))
+        bi1.register(np.arange(6).reshape(2,3))
+
+        sel = np.array([1, 1, 1, 0, 0, 0]).astype(bool)
+        post1 = list(bi1.iter_contiguous(sel))
+        post2 = list(bi1.iter_contiguous(sel, ascending=True))
+        self.assertEqual(post1, post2)
+        self.assertEqual(post1, [(0, slice(0, 3, None))])
+
+    def test_block_index_iter_contiguous_h2(self) -> None:
+        bi1 = BlockIndex()
+        bi1.register(np.arange(6).reshape(2,3))
+        bi1.register(np.arange(6).reshape(2,3))
+
+        sel = np.array([1, 0, 1, 0, 1, 0]).astype(bool)
+        post1 = list(bi1.iter_contiguous(sel))
+        post2 = list(bi1.iter_contiguous(sel, ascending=True))
+        self.assertEqual(post1, post2)
+        self.assertEqual(post1,
+                [(0, slice(0, 1, None)),
+                (0, slice(2, 3, None)),
+                (1, slice(1, 2, None))])
+
+        post3 = list(bi1.iter_contiguous(sel, ascending=True, reduce=True))
+        self.assertEqual(post3,
+                [(0, 0),
+                (0, 2),
+                (1, 1)])
+
```

### Comparing `arraykit-0.4.4/test/test_delimited_to_arrays.py` & `arraykit-0.4.5/test/test_delimited_to_arrays.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.4/test/test_delimited_to_arrays_integration.py` & `arraykit-0.4.5/test/test_delimited_to_arrays_integration.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.4/test/test_delimited_to_arrays_property.py` & `arraykit-0.4.5/test/test_delimited_to_arrays_property.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.4/test/test_pyi.py` & `arraykit-0.4.5/test/test_pyi.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.4/test/test_split_after_count.py` & `arraykit-0.4.5/test/test_split_after_count.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.4/test/test_type_discovery.py` & `arraykit-0.4.5/test/test_type_discovery.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.4/test/test_util.py` & `arraykit-0.4.5/test/test_util.py`

 * *Files identical despite different names*

