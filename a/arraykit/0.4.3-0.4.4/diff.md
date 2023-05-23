# Comparing `tmp/arraykit-0.4.3.tar.gz` & `tmp/arraykit-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraykit-0.4.3.tar", last modified: Sun May 21 17:55:06 2023, max compression
+gzip compressed data, was "arraykit-0.4.4.tar", last modified: Mon May 22 23:19:03 2023, max compression
```

## Comparing `arraykit-0.4.3.tar` & `arraykit-0.4.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:55:06.077374 arraykit-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-21 17:54:59.000000 arraykit-0.4.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-21 17:54:59.000000 arraykit-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-21 17:55:06.077374 arraykit-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-21 17:54:59.000000 arraykit-0.4.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:55:06.077374 arraykit-0.4.3/arraykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-21 17:55:05.000000 arraykit-0.4.3/arraykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-21 17:55:06.000000 arraykit-0.4.3/arraykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 17:55:05.000000 arraykit-0.4.3/arraykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-21 17:55:05.000000 arraykit-0.4.3/arraykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 17:55:05.000000 arraykit-0.4.3/arraykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 17:55:06.077374 arraykit-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-21 17:54:59.000000 arraykit-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:55:06.077374 arraykit-0.4.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-21 17:54:59.000000 arraykit-0.4.3/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   188739 2023-05-21 17:54:59.000000 arraykit-0.4.3/src/_arraykit.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:55:06.077374 arraykit-0.4.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-21 17:54:59.000000 arraykit-0.4.3/test/test_array_go.py
--rw-r--r--   0 runner    (1001) docker     (123)    24496 2023-05-21 17:54:59.000000 arraykit-0.4.3/test/test_block_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    49054 2023-05-21 17:54:59.000000 arraykit-0.4.3/test/test_delimited_to_arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-21 17:54:59.000000 arraykit-0.4.3/test/test_delimited_to_arrays_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-21 17:54:59.000000 arraykit-0.4.3/test/test_delimited_to_arrays_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-21 17:54:59.000000 arraykit-0.4.3/test/test_pyi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-21 17:54:59.000000 arraykit-0.4.3/test/test_split_after_count.py
--rw-r--r--   0 runner    (1001) docker     (123)    28073 2023-05-21 17:54:59.000000 arraykit-0.4.3/test/test_type_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    27668 2023-05-21 17:54:59.000000 arraykit-0.4.3/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:19:03.500360 arraykit-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-22 23:18:54.000000 arraykit-0.4.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-22 23:18:54.000000 arraykit-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-22 23:19:03.496360 arraykit-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-22 23:18:54.000000 arraykit-0.4.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:19:03.496360 arraykit-0.4.4/arraykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-22 23:19:03.000000 arraykit-0.4.4/arraykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-22 23:19:03.000000 arraykit-0.4.4/arraykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 23:19:03.000000 arraykit-0.4.4/arraykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 23:19:03.000000 arraykit-0.4.4/arraykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 23:19:03.000000 arraykit-0.4.4/arraykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 23:19:03.500360 arraykit-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-22 23:18:54.000000 arraykit-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:19:03.496360 arraykit-0.4.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-22 23:18:54.000000 arraykit-0.4.4/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   189205 2023-05-22 23:18:54.000000 arraykit-0.4.4/src/_arraykit.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:19:03.496360 arraykit-0.4.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-22 23:18:54.000000 arraykit-0.4.4/test/test_array_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26033 2023-05-22 23:18:54.000000 arraykit-0.4.4/test/test_block_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49054 2023-05-22 23:18:54.000000 arraykit-0.4.4/test/test_delimited_to_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-22 23:18:54.000000 arraykit-0.4.4/test/test_delimited_to_arrays_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-22 23:18:54.000000 arraykit-0.4.4/test/test_delimited_to_arrays_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-22 23:18:54.000000 arraykit-0.4.4/test/test_pyi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-22 23:18:54.000000 arraykit-0.4.4/test/test_split_after_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28073 2023-05-22 23:18:54.000000 arraykit-0.4.4/test/test_type_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27668 2023-05-22 23:18:54.000000 arraykit-0.4.4/test/test_util.py
```

### Comparing `arraykit-0.4.3/LICENSE.txt` & `arraykit-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.3/PKG-INFO` & `arraykit-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arraykit
-Version: 0.4.3
+Version: 0.4.4
 Summary: Array utilities for StaticFrame
 Home-page: https://github.com/static-frame/arraykit
 Author: Christopher Ariza, Brandt Bucher, Charles Burkland
 License: MIT
 Description: The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
         
         Code: https://github.com/static-frame/arraykit
```

### Comparing `arraykit-0.4.3/README.rst` & `arraykit-0.4.4/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,20 @@
 - NumPy >= 1.18.5
 
 
 
 What is New in ArrayKit
 -------------------------
 
+0.4.4
+............
+
+Corrected deallocation routines in ``BlockIndex.iter_contiguous()``.
+
+
 0.4.3
 ............
 
 Added ``BlockIndex.iter_contiguous()`` with options for ``ascending`` and ``reduce`` sequences.
 
 
 0.4.2
```

### Comparing `arraykit-0.4.3/arraykit.egg-info/PKG-INFO` & `arraykit-0.4.4/arraykit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arraykit
-Version: 0.4.3
+Version: 0.4.4
 Summary: Array utilities for StaticFrame
 Home-page: https://github.com/static-frame/arraykit
 Author: Christopher Ariza, Brandt Bucher, Charles Burkland
 License: MIT
 Description: The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
         
         Code: https://github.com/static-frame/arraykit
```

### Comparing `arraykit-0.4.3/setup.py` & `arraykit-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import site
 import os
 import typing as tp
 from setuptools import Extension  # type: ignore
 from setuptools import setup
 from pathlib import Path
 
-AK_VERSION = '0.4.3'
+AK_VERSION = '0.4.4'
 
 def get_long_description() -> str:
     return '''The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
 
 Code: https://github.com/static-frame/arraykit
 
 Packages: https://pypi.org/project/arraykit
```

### Comparing `arraykit-0.4.3/src/__init__.py` & `arraykit-0.4.4/src/__init__.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.3/src/_arraykit.c` & `arraykit-0.4.4/src/_arraykit.c`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,20 @@
 
 # define AK_DEBUG_MSG_OBJ(msg, obj)     \
     _AK_DEBUG_BEGIN();                  \
         fprintf(stderr, #msg " ");      \
         PyObject_Print(obj, stderr, 0); \
     _AK_DEBUG_END()
 
+# define AK_DEBUG_MSG_REFCNT(msg, obj)     \
+    _AK_DEBUG_BEGIN();                  \
+        fprintf(stderr, #msg " ref count: ");      \
+        PyObject_Print(PyLong_FromSsize_t(Py_REFCNT((PyObject*)obj)), stderr, 0); \
+    _AK_DEBUG_END()
+
 # define AK_DEBUG_OBJ(obj)              \
     _AK_DEBUG_BEGIN();                  \
         fprintf(stderr, #obj " = ");    \
         PyObject_Print(obj, stderr, 0); \
     _AK_DEBUG_END()
 
 # define AK_DEBUG(msg)          \
@@ -4240,41 +4246,41 @@
 //------------------------------------------------------------------------------
 // BI Iterator
 static PyTypeObject BIIterType;
 
 typedef struct BIIterObject {
     PyObject_VAR_HEAD
     BlockIndexObject *bi;
-    int8_t reversed;
+    bool reversed;
     Py_ssize_t pos; // current index state, mutated in-place
 } BIIterObject;
 
 static PyObject *
-BIIter_new(BlockIndexObject *bi, int8_t reversed) {
+BIIter_new(BlockIndexObject *bi, bool reversed) {
     BIIterObject *bii = PyObject_New(BIIterObject, &BIIterType);
     if (!bii) {
         return NULL;
     }
-    Py_INCREF(bi);
+    Py_INCREF((PyObject*)bi);
     bii->bi = bi;
     bii->reversed = reversed;
     bii->pos = 0;
     return (PyObject *)bii;
 }
 
 static void
 BIIter_dealloc(BIIterObject *self) {
-    Py_DECREF(self->bi);
-    Py_TYPE(self)->tp_free((PyObject *)self);
+    Py_DECREF((PyObject*)self->bi);
+    PyObject_Del((PyObject*)self);
 }
 
-static BIIterObject *
+static PyObject*
 BIIter_iter(BIIterObject *self) {
     Py_INCREF(self);
-    return self;
+    return (PyObject*)self;
 }
 
 static PyObject *
 BIIter_iternext(BIIterObject *self) {
     Py_ssize_t i;
     if (self->reversed) {
         i = self->bi->bir_count - ++self->pos;
@@ -4315,15 +4321,14 @@
     .tp_dealloc = (destructor) BIIter_dealloc,
     .tp_iter = (getiterfunc) BIIter_iter,
     .tp_iternext = (iternextfunc) BIIter_iternext,
     .tp_methods = BIIter_methods,
     .tp_name = "arraykit.BlockIndexIterator",
 };
 
-
 //------------------------------------------------------------------------------
 // BI Iterator sequence selection
 static PyTypeObject BIIterSeqType;
 static PyTypeObject BIIterSliceType;
 static PyTypeObject BIIterBoolType;
 
 
@@ -4334,45 +4339,45 @@
     BIIS_UNKNOWN
 } BIIterSelectorKind;
 
 
 static PyObject *
 BIIterSelector_new(BlockIndexObject *bi,
         PyObject* selector,
-        int8_t reversed,
+        bool reversed,
         BIIterSelectorKind kind,
-        int8_t ascending
+        bool ascending
         );
 
 typedef struct BIIterSeqObject {
     PyObject_VAR_HEAD
     BlockIndexObject *bi;
-    int8_t reversed;
+    bool reversed;
     PyObject* selector;
     Py_ssize_t pos; // current pos in sequence, mutated in-place
     Py_ssize_t len;
-    int8_t is_array;
+    bool is_array;
 } BIIterSeqObject;
 
 static void
 BIIterSeq_dealloc(BIIterSeqObject *self) {
-    Py_DECREF(self->bi);
+    Py_DECREF((PyObject*)self->bi);
     Py_DECREF(self->selector);
-    Py_TYPE(self)->tp_free((PyObject *)self);
+    PyObject_Del((PyObject*)self);
 }
 
-static BIIterSeqObject *
+static PyObject*
 BIIterSeq_iter(BIIterSeqObject *self) {
     Py_INCREF(self);
-    return self;
+    return (PyObject*)self;
 }
 
 // Returns -1 on end of sequence; return -1 with exception set on
 static inline Py_ssize_t
-BIIterSeq_iternext_core(BIIterSeqObject *self)
+BIIterSeq_iternext_index(BIIterSeqObject *self)
 {
     Py_ssize_t i;
     if (self->reversed) {
         i = self->len - ++self->pos;
         if (i < 0) {
             return -1;
         }
@@ -4435,28 +4440,30 @@
     return t;
 }
 
 
 static PyObject *
 BIIterSeq_iternext(BIIterSeqObject *self)
 {
-    Py_ssize_t i = BIIterSeq_iternext_core(self);
+    Py_ssize_t i = BIIterSeq_iternext_index(self);
     if (i == -1) {
         return NULL; // an error is set
     }
     return AK_BI_item(self->bi, i); // return new ref
 }
 
 static PyObject *
-BIIterSeq_reversed(BIIterSeqObject *self) {
+BIIterSeq_reversed(BIIterSeqObject *self)
+{
     return BIIterSelector_new(self->bi, self->selector, !self->reversed, BIIS_SEQ, 0);
 }
 
 static PyObject *
-BIIterSeq_length_hint(BIIterSeqObject *self) {
+BIIterSeq_length_hint(BIIterSeqObject *self)
+{
     // this works for reversed as we use self-> index to subtract from length
     Py_ssize_t len = Py_MAX(0, self->len - self->pos);
     return PyLong_FromSsize_t(len);
 }
 
 static PyMethodDef BIiterSeq_methods[] = {
     {"__length_hint__", (PyCFunction)BIIterSeq_length_hint, METH_NOARGS, NULL},
@@ -4476,66 +4483,69 @@
 
 //------------------------------------------------------------------------------
 // BI Iterator slice selection
 
 typedef struct BIIterSliceObject {
     PyObject_VAR_HEAD
     BlockIndexObject *bi;
-    int8_t reversed;
+    bool reversed;
     PyObject* selector; // slice
     Py_ssize_t count; // count of , mutated in-place
     // these are the normalized values truncated to the span of the bir_count; len is the realized length after extraction; step is always set to 1 if missing; len is 0 if no realized values
     Py_ssize_t pos;
     Py_ssize_t step;
     Py_ssize_t len;
 } BIIterSliceObject;
 
 static void
 BIIterSlice_dealloc(BIIterSliceObject *self) {
-    Py_DECREF(self->bi);
+    // AK_DEBUG_MSG_REFCNT("start dealloc", self);
+    Py_DECREF((PyObject*)self->bi);
     Py_DECREF(self->selector);
-    Py_TYPE(self)->tp_free((PyObject *)self);
+    PyObject_Del((PyObject*)self);
 }
 
-static BIIterSliceObject *
+static PyObject*
 BIIterSlice_iter(BIIterSliceObject *self) {
     Py_INCREF(self);
-    return self;
+    return (PyObject*)self;
 }
 
+// NOTE: this does not use `reversed`, as pos, step, and count are set in BIIterSelector_new
 static inline Py_ssize_t
-BIIterSlice_iternext_core(BIIterSliceObject *self)
+BIIterSlice_iternext_index(BIIterSliceObject *self)
 {
     if (self->len == 0 || self->count >= self->len) {
         return -1;
     }
     Py_ssize_t i = self->pos;
     self->pos += self->step;
     self->count++; // by counting index we we do not need to compare to stop
     // i will never be out of range
     return i;
 }
 
-// NOTE: this does not use `reversed`, as pos, step, and count are set in BIIterSelector_new
 static PyObject *
 BIIterSlice_iternext(BIIterSliceObject *self) {
-    Py_ssize_t i = BIIterSlice_iternext_core(self);
+    Py_ssize_t i = BIIterSlice_iternext_index(self);
     if (i == -1) {
         return NULL;
     }
     return AK_BI_item(self->bi, i); // return new ref
 }
 
 static PyObject *
-BIIterSlice_reversed(BIIterSliceObject *self) {
+BIIterSlice_reversed(BIIterSliceObject *self)
+{
     return BIIterSelector_new(self->bi, self->selector, !self->reversed, BIIS_SLICE, 0);
 }
 
 static PyObject *
-BIIterSlice_length_hint(BIIterSliceObject *self) {
+BIIterSlice_length_hint(BIIterSliceObject *self)
+{
     // this works for reversed as we use self-> index to subtract from length
     Py_ssize_t len = Py_MAX(0, self->len - self->count);
     return PyLong_FromSsize_t(len);
 }
 
 static PyMethodDef BIiterSlice_methods[] = {
     {"__length_hint__", (PyCFunction)BIIterSlice_length_hint, METH_NOARGS, NULL},
@@ -4555,35 +4565,36 @@
 
 //------------------------------------------------------------------------------
 // BI Iterator Boolean array selection
 
 typedef struct BIIterBooleanObject {
     PyObject_VAR_HEAD
     BlockIndexObject *bi;
-    int8_t reversed;
+    bool reversed;
     PyObject* selector;
     Py_ssize_t pos; // current index, mutated in-place
     Py_ssize_t len;
 } BIIterBooleanObject;
 
 static void
 BIIterBoolean_dealloc(BIIterBooleanObject *self) {
-    Py_DECREF(self->bi);
+    Py_DECREF((PyObject*)self->bi);
     Py_DECREF(self->selector);
-    Py_TYPE(self)->tp_free((PyObject *)self);
+    PyObject_Del((PyObject*)self);
 }
 
-static BIIterBooleanObject *
-BIIterBoolean_iter(BIIterBooleanObject *self) {
+static PyObject*
+BIIterBoolean_iter(BIIterBooleanObject *self)
+{
     Py_INCREF(self);
-    return self;
+    return (PyObject*)self;
 }
 
 static inline Py_ssize_t
-BIIterBoolean_iternext_core(BIIterBooleanObject *self)
+BIIterBoolean_iternext_index(BIIterBooleanObject *self)
 {
     npy_bool v = 0;
     Py_ssize_t i = -1;
     PyArrayObject* a = (PyArrayObject*) self->selector;
 
     if (!self->reversed) {
         while (self->pos < self->len) {
@@ -4611,23 +4622,24 @@
         return i;
     }
     return -1; // no True remain
 }
 
 static PyObject *
 BIIterBoolean_iternext(BIIterBooleanObject *self) {
-    Py_ssize_t i = BIIterBoolean_iternext_core(self);
+    Py_ssize_t i = BIIterBoolean_iternext_index(self);
     if (i == -1) {
         return NULL;
     }
     return AK_BI_item(self->bi, i); // return new ref
 }
 
 static PyObject *
-BIIterBoolean_reversed(BIIterBooleanObject *self) {
+BIIterBoolean_reversed(BIIterBooleanObject *self)
+{
     return BIIterSelector_new(self->bi, self->selector, !self->reversed, BIIS_BOOLEAN, 0);
 }
 
 // NOTE: no length hint given as we would have to traverse whole array and count True... not sure it is worht it.
 static PyMethodDef BIiterBoolean_methods[] = {
     {"__reversed__", (PyCFunction)BIIterBoolean_reversed, METH_NOARGS, NULL},
     {NULL},
@@ -4646,63 +4658,107 @@
 //------------------------------------------------------------------------------
 // BI Iterator Contigous
 static PyTypeObject BIIterContiguousType;
 
 typedef struct BIIterContiguousObject {
     PyObject_VAR_HEAD
     BlockIndexObject *bi;
-    PyObject* iter; // own refernce to core iterator
-    int8_t reversed;
+    PyObject* iter; // own reference to core iterator
+    bool reversed;
     Py_ssize_t last_block;
     Py_ssize_t last_column;
     Py_ssize_t next_block;
     Py_ssize_t next_column;
     bool reduce; // optionally reduce slices to integers
 } BIIterContiguousObject;
 
 static PyObject *
 BIIterContiguous_new(BlockIndexObject *bi,
-        int8_t reversed,
+        bool reversed,
         PyObject* iter,
         bool reduce)
 {
     BIIterContiguousObject *bii = PyObject_New(BIIterContiguousObject, &BIIterContiguousType);
     if (!bii) {
         return NULL;
     }
-    Py_INCREF(bi);
+    Py_INCREF((PyObject*)bi);
     bii->bi = bi;
+
     Py_INCREF(iter);
     bii->iter = iter;
+
     bii->reversed = reversed;
 
     bii->last_block = -1;
     bii->last_column = -1;
     bii->next_block = -1;
     bii->next_column = -1;
     bii->reduce = reduce;
 
     return (PyObject *)bii;
 }
 
 static void
-BIIterContiguous_dealloc(BIIterContiguousObject *self) {
-    Py_DECREF(self->bi);
+BIIterContiguous_dealloc(BIIterContiguousObject *self)
+{
+    Py_DECREF((PyObject*)self->bi);
     Py_DECREF(self->iter);
-    Py_TYPE(self)->tp_free((PyObject *)self);
+    PyObject_Del((PyObject*)self);
 }
 
-static BIIterContiguousObject *
-BIIterContiguous_iter(BIIterContiguousObject *self) {
+
+// Simply incref this object and return it.
+static PyObject*
+BIIterContiguous_iter(BIIterContiguousObject *self)
+{
     Py_INCREF(self);
-    return self;
+    return (PyObject*)self;
 }
 
+// Returns a new reference.
 static PyObject *
-BIIterContiguous_iternext(BIIterContiguousObject *self) {
+BIIterContiguous_reversed(BIIterContiguousObject *self)
+{
+    bool reversed = !self->reversed;
+
+    PyObject* selector = NULL;
+    PyTypeObject* type = Py_TYPE(self->iter);
+    if (type == &BIIterSeqType) {
+        selector = ((BIIterSeqObject*)self->iter)->selector;
+    }
+    else if (type == &BIIterSliceType) {
+        selector = ((BIIterSliceObject*)self->iter)->selector;
+    }
+    else if (type == &BIIterBoolType) {
+        selector = ((BIIterBooleanObject*)self->iter)->selector;
+    }
+    if (selector == NULL) {
+        return NULL;
+    }
+
+    PyObject* iter = BIIterSelector_new(self->bi,
+            selector,
+            reversed,
+            BIIS_UNKNOWN, // let type be determined by selector
+            0);
+    if (iter == NULL) {
+        return NULL;
+    }
+    PyObject* biiter = BIIterContiguous_new(self->bi,
+            reversed,
+            self->iter,
+            self->reduce);
+    Py_DECREF(iter);
+    return biiter;
+}
+
+static PyObject *
+BIIterContiguous_iternext(BIIterContiguousObject *self)
+{
     Py_ssize_t i = -1;
     PyObject* iter = self->iter;
     PyTypeObject* type = Py_TYPE(iter);
 
     Py_ssize_t slice_start = -1;
     Py_ssize_t block;
     Py_ssize_t column;
@@ -4714,35 +4770,35 @@
         if (self->next_block != -1) {
             // discontinuity found on last iteration, set new start
             self->last_block = self->next_block;
             self->last_column = slice_start = self->next_column;
             self->next_block = self->next_column = -1; // clear next state
         }
         if (type == &BIIterSeqType) {
-            i = BIIterSeq_iternext_core((BIIterSeqObject*)iter);
+            i = BIIterSeq_iternext_index((BIIterSeqObject*)iter);
         }
         else if (type == &BIIterSliceType) {
-            i = BIIterSlice_iternext_core((BIIterSliceObject*)iter);
+            i = BIIterSlice_iternext_index((BIIterSliceObject*)iter);
         }
         else if (type == &BIIterBoolType) {
-            i = BIIterBoolean_iternext_core((BIIterBooleanObject*)iter);
+            i = BIIterBoolean_iternext_index((BIIterBooleanObject*)iter);
         }
         if (i == -1) { // end of iteration or error
             if (PyErr_Occurred()) {
                 break;
             }
             // no more pairs, return previous slice_start, flag for end on next call
             self->next_block = -2;
             return Py_BuildValue("nN", // N steals ref
                     self->last_block,
                     AK_build_slice_inclusive(slice_start,
                             self->last_column,
                             self->reduce));
         }
-        // i is gauranteed to be within the range of self->bit_count at this point; the only source of arbitrary indices is in BIIterSeq_iternext_core, and that function validates the range
+        // i is gauranteed to be within the range of self->bit_count at this point; the only source of arbitrary indices is in BIIterSeq_iternext_index, and that function validates the range
         BlockIndexRecord* biri = &self->bi->bir[i];
         block = biri->block;
         column = biri->column;
 
         // inititialization
         if (self->last_block == -1) {
             self->last_block = block;
@@ -4762,47 +4818,14 @@
                 AK_build_slice_inclusive(slice_start,
                         self->last_column,
                         self->reduce));
     }
     return NULL;
 }
 
-static PyObject *
-BIIterContiguous_reversed(BIIterContiguousObject *self) {
-
-    PyObject* selector = NULL;
-    PyTypeObject* type = Py_TYPE(self->iter);
-    if (type == &BIIterSeqType) {
-        selector = ((BIIterSeqObject*)self->iter)->selector;
-    }
-    else if (type == &BIIterSliceType) {
-        selector = ((BIIterSliceObject*)self->iter)->selector;
-    }
-    else if (type == &BIIterBoolType) {
-        selector = ((BIIterBooleanObject*)self->iter)->selector;
-    }
-
-    if (selector == NULL) {
-        return NULL;
-    }
-
-    PyObject* iter = BIIterSelector_new(self->bi,
-            selector,
-            !self->reversed,
-            BIIS_UNKNOWN, // let type be determined by selector
-            0);
-    PyObject* biiter = BIIterContiguous_new(self->bi,
-            !self->reversed,
-            self->iter,
-            self->reduce);
-    Py_DECREF(iter);
-    return biiter;
-}
-
-
 // not implementing __length_hint__
 static PyMethodDef BIIterContiguous_methods[] = {
     {"__reversed__", (PyCFunction)BIIterContiguous_reversed, METH_NOARGS, NULL},
     {NULL},
 };
 
 
@@ -4812,40 +4835,39 @@
     .tp_dealloc = (destructor) BIIterContiguous_dealloc,
     .tp_iter = (getiterfunc) BIIterContiguous_iter,
     .tp_iternext = (iternextfunc) BIIterContiguous_iternext,
     .tp_methods = BIIterContiguous_methods,
     .tp_name = "arraykit.BlockIndexContiguousIterator",
 };
 
-
 //------------------------------------------------------------------------------
 
 // NOTE: this constructor returns one of three different PyObject types. We do this to consolidate error reporting and type checks.
 // The ascending argument is applied before consideration of a reverse iterator
 static PyObject *
 BIIterSelector_new(BlockIndexObject *bi,
         PyObject* selector,
-        int8_t reversed,
+        bool reversed,
         BIIterSelectorKind kind,
-        int8_t ascending) {
+        bool ascending) {
 
-    int8_t is_array = 0;
-    int8_t incref_selector = 1; // incref borrowed selector; but if a new ref is made, do not
+    bool is_array = false;
+    bool incref_selector = true; // incref borrowed selector; but if a new ref is made, do not
 
     Py_ssize_t len = -1;
     Py_ssize_t pos = 0;
     Py_ssize_t stop = 0;
     Py_ssize_t step = 0;
 
     if (PyArray_Check(selector)) {
         if (kind == BIIS_SLICE) {
             PyErr_SetString(PyExc_TypeError, "Arrays cannot be used as selectors for slice iterators");
             return NULL;
         }
-        is_array = 1;
+        is_array = true;
         PyArrayObject *a = (PyArrayObject *)selector;
         if (PyArray_NDIM(a) != 1) {
             PyErr_SetString(PyExc_TypeError, "Arrays must be 1-dimensional");
             return NULL;
         }
         len = PyArray_SIZE(a);
 
@@ -4877,32 +4899,31 @@
         if (ascending) {
             // NOTE: we can overwrite selector here as we have a borrowed refernce; sorting gives us a new reference, so we do not need to incref below
             selector = PyArray_NewCopy(a, NPY_CORDER);
             // sort in-place; can use a non-stable sort
             if (PyArray_Sort((PyArrayObject*)selector, 0, NPY_QUICKSORT)) {
                 return NULL; // returns -1 on error
             }; // new ref
-            incref_selector = 0;
+            incref_selector = false;
         }
     }
     else if (PySlice_Check(selector)) {
         if (kind == BIIS_UNKNOWN) {
             kind = BIIS_SLICE;
         }
         else if (kind != BIIS_SLICE) {
             PyErr_SetString(PyExc_TypeError, "Slices cannot be used as selectors for this type of iterator");
             return NULL;
         }
 
         if (ascending) {
             // NOTE: we are abandoning the borrowed reference
             selector = AK_slice_to_ascending_slice(selector, bi->bir_count); // new ref
-            incref_selector = 0;
+            incref_selector = false;
         }
-
         if (PySlice_Unpack(selector, &pos, &stop, &step)) {
             return NULL;
         }
         len = PySlice_AdjustIndices(bi->bir_count, &pos, &stop, step);
 
         if (reversed) {
             pos += (step * (len - 1));
@@ -4926,15 +4947,15 @@
                 return NULL;
             }
             PyObject* post = PyObject_CallMethod(selector, "sort", NULL); // new ref
             if (post == NULL) {
                 return NULL;
             }
             Py_DECREF(post); // just a None
-            incref_selector = 0;
+            incref_selector = false;
         }
     }
     else {
         PyErr_SetString(PyExc_TypeError, "Input type not supported");
         return NULL;
     }
 
@@ -4975,15 +4996,16 @@
             it->pos = reversed ? len - 1 : 0;
             bii = (PyObject*)it;
             break;
         }
         case BIIS_UNKNOWN:
             goto error; // should not get here!
     }
-    Py_INCREF(bi);
+    Py_INCREF((PyObject*)bi);
+
     if (incref_selector) {
         Py_INCREF(selector);
     }
     return bii;
 error: // nothing shold be increfed when we get here
     return NULL;
 }
@@ -5036,16 +5058,14 @@
     }
     return (PyObject *)self;
 }
 
 // Returns 0 on success, -1 on error.
 int
 BlockIndex_init(PyObject *self, PyObject *args, PyObject *kwargs) {
-    // PyTypeObject* cls = Py_TYPE(self); // borrowed ref
-    // const char *name = cls->tp_name;
     BlockIndexObject* bi = (BlockIndexObject*)self;
 
     Py_ssize_t block_count = 0;
     Py_ssize_t row_count = -1; // mark as unset
     Py_ssize_t bir_count = 0;
     Py_ssize_t bir_capacity = 8;
     PyObject* bir_bytes = NULL;
@@ -5144,15 +5164,14 @@
     }
 
     // if we are not adding columns, we are not adding types, so we are not changing the  dtype or shape
     if (increment == 0) {
         Py_RETURN_FALSE;
     }
 
-
     PyArray_Descr* dt = PyArray_DESCR(a); // borrowed ref
     self->shape_recache = true; // adjusting columns, must recache shape
 
     if (self->dtype == NULL) { // if not already set
         Py_INCREF((PyObject*)dt);
         self->dtype = dt;
     }
@@ -5272,15 +5291,15 @@
 static PyObject *
 BlockIndex_rows_getter(BlockIndexObject *self, void* Py_UNUSED(closure)){
     return PyLong_FromSsize_t(self->row_count);
 }
 
 static PyObject *
 BlockIndex_columns_getter(BlockIndexObject *self, void* Py_UNUSED(closure)){
-    return PyLong_FromSsize_t(self->bir_count );
+    return PyLong_FromSsize_t(self->bir_count);
 }
 
 // Return the resolved dtype for all registered blocks. If no block have been registered, this will return a float dtype.
 static PyObject *
 BlockIndex_dtype_getter(BlockIndexObject *self, void* Py_UNUSED(closure)){
     if (self->dtype != NULL) {
         Py_INCREF(self->dtype);
@@ -5424,17 +5443,19 @@
             &reduce
             )) {
         return NULL;
     }
 
     // might need to store enum type for branching
     PyObject* iter = BIIterSelector_new(self, selector, 0, BIIS_UNKNOWN, ascending);
-    PyObject* biiter = BIIterContiguous_new(self, 0, iter, reduce); // will incref iter
+    if (iter == NULL) {
+        return NULL; // exception set
+    }
+    PyObject* biiter = BIIterContiguous_new(self, 0, iter, reduce); // might be NULL, will incref iter
     Py_DECREF(iter);
-
     return biiter;
 }
 
 //------------------------------------------------------------------------------
 // slot / method def
 
 static PySequenceMethods BlockIndex_as_sequece = {
```

### Comparing `arraykit-0.4.3/test/test_array_go.py` & `arraykit-0.4.4/test/test_array_go.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.3/test/test_block_index.py` & `arraykit-0.4.4/test/test_block_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -561,14 +561,29 @@
         bi1.register(np.arange(4).reshape(2,2))
         bi1.register(np.arange(2))
         bi1.register(np.arange(10).reshape(2,5))
 
         with self.assertRaises(TypeError):
             _ = list(bi1.iter_select(['b', 'c']))
 
+
+
+    def test_block_index_iter_select_sequence_d(self) -> None:
+        bi1 = BlockIndex()
+        bi1.register(np.arange(10).reshape(2,5))
+
+        sel = [0, 3, 4]
+        it1 = iter(bi1.iter_select(sel))
+        it2 = iter(it1)
+        del sel
+        del bi1
+        del it1
+        self.assertEqual(list(it2), [(0, 0), (0, 3), (0, 4)])
+
+
     #---------------------------------------------------------------------------
 
     def test_block_index_iter_contiguous_a(self) -> None:
         bi1 = BlockIndex()
         bi1.register(np.arange(6).reshape(2,3))
         bi1.register(np.arange(2))
         bi1.register(np.arange(6).reshape(2,3))
@@ -701,7 +716,48 @@
             list(bi1.iter_contiguous(np.array([6, 0, 7]), reduce=True)),
             [(6, 0), (0, 0), (7, 0)]
             )
         self.assertEqual(
             list(bi1.iter_contiguous(np.array([6, 0, 7]), ascending=True, reduce=True)),
             [(0, 0), (6, 0), (7, 0)]
             )
+
+
+    def test_block_index_iter_contiguous_f1(self) -> None:
+        bi1 = BlockIndex()
+        bi1.register(np.arange(6).reshape(2,3))
+        bi1.register(np.arange(6).reshape(2,3))
+        bi1.register(np.arange(4).reshape(2,2))
+
+        key = np.array([2, 3, 5])
+
+        def gen1():
+            yield from bi1.iter_select(key)
+        post1 = list(gen1())
+        self.assertEqual(post1, [(0, 2), (1, 0), (1, 2)])
+
+
+
+    def test_block_index_iter_contiguous_f2(self) -> None:
+        bi1 = BlockIndex()
+        bi1.register(np.arange(6).reshape(2,3))
+        bi1.register(np.arange(6).reshape(2,3))
+        bi1.register(np.arange(4).reshape(2,2))
+        key = np.array([2, 3, 5])
+
+        def gen2():
+            yield from bi1.iter_contiguous(key)
+        post2 = list(gen2())
+
+        post1 = list(bi1.iter_contiguous(key))
+        self.assertEqual(post1, post2)
+
+
+
+    def test_block_index_iter_contiguous_g(self) -> None:
+        bi1 = BlockIndex()
+        bi1.register(np.arange(6).reshape(2,3))
+        bi1.register(np.arange(6).reshape(2,3))
+        bi1.register(np.arange(4).reshape(2,2))
+
+        with self.assertRaises(TypeError):
+            _ = list(bi1.iter_contiguous('a'))
```

### Comparing `arraykit-0.4.3/test/test_delimited_to_arrays.py` & `arraykit-0.4.4/test/test_delimited_to_arrays.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.3/test/test_delimited_to_arrays_integration.py` & `arraykit-0.4.4/test/test_delimited_to_arrays_integration.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.3/test/test_delimited_to_arrays_property.py` & `arraykit-0.4.4/test/test_delimited_to_arrays_property.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.3/test/test_pyi.py` & `arraykit-0.4.4/test/test_pyi.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.3/test/test_split_after_count.py` & `arraykit-0.4.4/test/test_split_after_count.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.3/test/test_type_discovery.py` & `arraykit-0.4.4/test/test_type_discovery.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.4.3/test/test_util.py` & `arraykit-0.4.4/test/test_util.py`

 * *Files identical despite different names*

