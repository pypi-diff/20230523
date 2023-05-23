# Comparing `tmp/PyMT64-1.9.tar.gz` & `tmp/PyMT64-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyMT64-1.9.tar", last modified: Mon May 11 10:54:52 2020, max compression
+gzip compressed data, was "PyMT64-2.0.tar", last modified: Tue May 23 09:09:31 2023, max compression
```

## Comparing `PyMT64-1.9.tar` & `PyMT64-2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 reza      (1001) reza      (1001)        0 2020-05-11 10:54:52.000000 PyMT64-1.9/
--rw-r--r--   0 reza      (1001) reza      (1001)     6363 2020-05-11 10:48:26.000000 PyMT64-1.9/pymt64.pyx
--rw-r--r--   0 reza      (1001) reza      (1001)   389690 2020-05-11 10:48:35.000000 PyMT64-1.9/pymt64.c
--rw-r--r--   0 reza      (1001) reza      (1001)     2388 2020-05-11 10:39:42.000000 PyMT64-1.9/README.txt
--rw-r--r--   0 reza      (1001) reza      (1001)      871 2019-12-20 15:06:16.000000 PyMT64-1.9/pymt64_test_mp.py
--rw-r--r--   0 reza      (1001) reza      (1001)      767 2020-05-11 10:39:16.000000 PyMT64-1.9/setup.py
--rw-r--r--   0 reza      (1001) reza      (1001)     3435 2019-12-20 15:03:20.000000 PyMT64-1.9/mt64mp.h
--rw-r--r--   0 reza      (1001) reza      (1001)      336 2019-12-20 15:49:07.000000 PyMT64-1.9/pymt64lib.h
--rw-r--r--   0 reza      (1001) reza      (1001)     3129 2020-05-11 10:54:52.000000 PyMT64-1.9/PKG-INFO
--rw-r--r--   0 reza      (1001) reza      (1001)       38 2020-05-11 10:54:52.000000 PyMT64-1.9/setup.cfg
-drwxr-xr-x   0 reza      (1001) reza      (1001)        0 2020-05-11 10:54:52.000000 PyMT64-1.9/PyMT64.egg-info/
--rw-r--r--   0 reza      (1001) reza      (1001)        7 2020-05-11 10:54:52.000000 PyMT64-1.9/PyMT64.egg-info/top_level.txt
--rw-r--r--   0 reza      (1001) reza      (1001)        1 2020-05-11 10:54:52.000000 PyMT64-1.9/PyMT64.egg-info/dependency_links.txt
--rw-r--r--   0 reza      (1001) reza      (1001)     3129 2020-05-11 10:54:52.000000 PyMT64-1.9/PyMT64.egg-info/PKG-INFO
--rw-r--r--   0 reza      (1001) reza      (1001)      261 2020-05-11 10:54:52.000000 PyMT64-1.9/PyMT64.egg-info/SOURCES.txt
--rw-r--r--   0 reza      (1001) reza      (1001)     6812 2019-12-20 15:03:13.000000 PyMT64-1.9/mt19937-64mp.c
--rw-r--r--   0 reza      (1001) reza      (1001)      984 2019-12-20 15:06:13.000000 PyMT64-1.9/pymt64_test.py
--rw-r--r--   0 reza      (1001) reza      (1001)      152 2020-01-10 10:36:09.000000 PyMT64-1.9/Makefile
--rw-r--r--   0 reza      (1001) reza      (1001)     4537 2019-12-20 15:18:56.000000 PyMT64-1.9/pymt64lib.c
--rw-r--r--   0 reza      (1001) reza      (1001)      122 2020-01-10 11:01:14.000000 PyMT64-1.9/MANIFEST.in
+drwxrwxr-x   0 reza      (1001) reza      (1001)        0 2023-05-23 09:09:31.053198 PyMT64-2.0/
+-rw-r--r--   0 reza      (1001) reza      (1001)      122 2020-01-10 11:01:14.000000 PyMT64-2.0/MANIFEST.in
+-rw-r--r--   0 reza      (1001) reza      (1001)      152 2020-01-10 10:36:09.000000 PyMT64-2.0/Makefile
+-rw-rw-r--   0 reza      (1001) reza      (1001)     2832 2023-05-23 09:09:31.053198 PyMT64-2.0/PKG-INFO
+drwxrwxr-x   0 reza      (1001) reza      (1001)        0 2023-05-23 09:09:31.053198 PyMT64-2.0/PyMT64.egg-info/
+-rw-r--r--   0 reza      (1001) reza      (1001)     2832 2023-05-23 09:09:31.000000 PyMT64-2.0/PyMT64.egg-info/PKG-INFO
+-rw-r--r--   0 reza      (1001) reza      (1001)      261 2023-05-23 09:09:31.000000 PyMT64-2.0/PyMT64.egg-info/SOURCES.txt
+-rw-r--r--   0 reza      (1001) reza      (1001)        1 2023-05-23 09:09:31.000000 PyMT64-2.0/PyMT64.egg-info/dependency_links.txt
+-rw-r--r--   0 reza      (1001) reza      (1001)        7 2023-05-23 09:09:31.000000 PyMT64-2.0/PyMT64.egg-info/top_level.txt
+-rw-r--r--   0 reza      (1001) reza      (1001)     2534 2023-05-23 09:08:54.000000 PyMT64-2.0/README.txt
+-rw-r--r--   0 reza      (1001) reza      (1001)     6812 2019-12-20 15:03:13.000000 PyMT64-2.0/mt19937-64mp.c
+-rw-r--r--   0 reza      (1001) reza      (1001)     3435 2019-12-20 15:03:20.000000 PyMT64-2.0/mt64mp.h
+-rw-rw-r--   0 reza      (1001) reza      (1001)   317054 2023-05-23 08:40:13.000000 PyMT64-2.0/pymt64.c
+-rw-r--r--   0 reza      (1001) reza      (1001)     6366 2023-05-23 08:40:05.000000 PyMT64-2.0/pymt64.pyx
+-rw-r--r--   0 reza      (1001) reza      (1001)      984 2019-12-20 15:06:13.000000 PyMT64-2.0/pymt64_test.py
+-rw-r--r--   0 reza      (1001) reza      (1001)      871 2019-12-20 15:06:16.000000 PyMT64-2.0/pymt64_test_mp.py
+-rw-r--r--   0 reza      (1001) reza      (1001)     4537 2019-12-20 15:18:56.000000 PyMT64-2.0/pymt64lib.c
+-rw-r--r--   0 reza      (1001) reza      (1001)      336 2019-12-20 15:49:07.000000 PyMT64-2.0/pymt64lib.h
+-rw-rw-r--   0 reza      (1001) reza      (1001)       38 2023-05-23 09:09:31.053198 PyMT64-2.0/setup.cfg
+-rw-r--r--   0 reza      (1001) reza      (1001)      767 2023-05-23 08:27:04.000000 PyMT64-2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PyMT64-1.9/pymt64.pyx` & `PyMT64-2.0/pymt64.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -56,21 +56,21 @@
 # about the numpy module (this is stored in a file numpy.pxd which is
 # currently part of the Cython distribution).
 cimport numpy as np
 # We now need to fix a datatype for our arrays. I've used the variable
 # DTYPE for this, which is assigned to the usual NumPy runtime
 # type info object.
 DTYPE = np.double
-ITYPE = np.int
+#DTYPE = np.int
 U64TYPE = np.uint64
 # "ctypedef" assigns a corresponding compile-time type to DTYPE_t. For
 # every type in the numpy module there's a corresponding compile-time
 # type with a _t-suffix.
 ctypedef np.double_t DTYPE_t
-ctypedef np.int_t ITYPE_t
+#ctypedef np.int_t ITYPE_t
 ctypedef np.uint64_t U64TYPE_t
 # "def" can type its arguments but not have a return type. The type of the
 # arguments for a "def" function is checked at run-time when entering the
 # function.
 
 cimport cython
 cdef int MTSIZE = 312
@@ -80,14 +80,15 @@
 
 cdef extern from "pymt64lib.h":
     cdef void uniformn(UL64 * mt , int * mti, double * x , long n ) ;
     cdef void poissonn(UL64 * mt , int * mti , double xm, double * x , long n ) ;
     cdef void normaln(UL64 * mt, int * mti , double * x , double * y, long n ) ;
     cdef void poissonn_multlam( UL64 * mt , int * mti , double * xm, double * x , long n )
 
+
 def init(unsigned long long  seed ): 
     '''
     Function used to initialise the state vector mt used by the pseudorandom number generator.
     
     mt = init(seed)
     
     '''
```

### Comparing `PyMT64-1.9/pymt64.c` & `PyMT64-2.0/pymt64.c`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-/* Generated by Cython 0.28.5 */
+/* Generated by Cython 0.29.32 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/home/reza/anaconda2/envs/py3.5/lib/python3.5/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/home/reza/anaconda2/envs/py3.5/lib/python3.5/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/home/reza/venv/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/home/reza/venv/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/home/reza/venv/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/home/reza/venv/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/home/reza/venv/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "mt64mp.h",
             "pymt64lib.h"
         ],
         "include_dirs": [
-            "/home/reza/anaconda2/envs/py3.5/lib/python3.5/site-packages/numpy/core/include"
+            "/home/reza/venv/lib/python3.10/site-packages/numpy/core/include"
         ],
         "libraries": [
             "m"
         ],
         "name": "pymt64",
         "sources": [
             "pymt64.pyx",
@@ -22,22 +25,25 @@
             "mt19937-64mp.c"
         ]
     },
     "module_name": "pymt64"
 }
 END: Cython Metadata */
 
+#ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
+#endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_28_5"
+#define CYTHON_ABI "0_29_32"
+#define CYTHON_HEX_VERSION 0x001D20F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -68,14 +74,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -100,18 +107,26 @@
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
   #undef CYTHON_PEP489_MULTI_PHASE_INIT
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -137,18 +152,71 @@
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
   #undef CYTHON_PEP489_MULTI_PHASE_INIT
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -168,50 +236,70 @@
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0
+  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL 1
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT (0 && PY_VERSION_HEX >= 0x03050000)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
+  #ifndef CYTHON_USE_DICT_VERSIONS
+    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+  #endif
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
+    #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
+  #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #include "longintrepr.h"
+  #if PY_MAJOR_VERSION < 3
+    #include "longintrepr.h"
+  #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
+  #ifdef SIZEOF_VOID_P
+    enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
+  #endif
 #endif
 #ifndef __has_attribute
   #define __has_attribute(x) 0
 #endif
 #ifndef __has_cpp_attribute
   #define __has_cpp_attribute(x) 0
 #endif
@@ -314,52 +402,124 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject* co=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
+        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
+        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
+        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
+        if (!(nlocals=PyLong_FromLong(l))) goto end;
+        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
+        if (!(stacksize=PyLong_FromLong(s))) goto end;
+        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
+        if (!(flags=PyLong_FromLong(f))) goto end;
+        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
+        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
+        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
+        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
+        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
+        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
+        Py_XDECREF((PyObject*)co);
+        co = (PyCodeObject*)call_result;
+        call_result = NULL;
+        if (0) {
+            cleanup_code_too:
+            Py_XDECREF((PyObject*)co);
+            co = NULL;
+        }
+        end:
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(call_result);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return co;
+    }
+#else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+#endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
   #define Py_TPFLAGS_HAVE_NEWBUFFER 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_FINALIZE
   #define Py_TPFLAGS_HAVE_FINALIZE 0
 #endif
+#ifndef METH_STACKLESS
+  #define METH_STACKLESS 0
+#endif
 #if PY_VERSION_HEX <= 0x030700A3 || !defined(METH_FASTCALL)
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
   #define __Pyx_PyCFunctionFast _PyCFunctionFast
   #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
 #endif
 #if CYTHON_FAST_PYCCALL
 #define __Pyx_PyFastCFunction_Check(func)\
-    ((PyCFunction_Check(func) && (METH_FASTCALL == (PyCFunction_GET_FLAGS(func) & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS)))))
+    ((PyCFunction_Check(func) && (METH_FASTCALL == (PyCFunction_GET_FLAGS(func) & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)))))
 #else
 #define __Pyx_PyFastCFunction_Check(func) 0
 #endif
 #if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Malloc)
   #define PyObject_Malloc(s)   PyMem_Malloc(s)
   #define PyObject_Free(p)     PyMem_Free(p)
   #define PyObject_Realloc(p)  PyMem_Realloc(p)
 #endif
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030400A1
+  #define PyMem_RawMalloc(n)           PyMem_Malloc(n)
+  #define PyMem_RawRealloc(p, n)       PyMem_Realloc(p, n)
+  #define PyMem_RawFree(p)             PyMem_Free(p)
+#endif
 #if CYTHON_COMPILING_IN_PYSTON
   #define __Pyx_PyCode_HasFreeVars(co)  PyCode_HasFreeVars(co)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno) PyFrame_SetLineNumber(frame, lineno)
 #else
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
@@ -374,15 +534,15 @@
 #endif
 #if PY_VERSION_HEX < 0x030700A2 && !defined(PyThread_tss_create) && !defined(Py_tss_NEEDS_INIT)
 #include "pythread.h"
 #define Py_tss_NEEDS_INIT 0
 typedef int Py_tss_t;
 static CYTHON_INLINE int PyThread_tss_create(Py_tss_t *key) {
   *key = PyThread_create_key();
-  return 0; // PyThread_create_key reports success always
+  return 0;
 }
 static CYTHON_INLINE Py_tss_t * PyThread_tss_alloc(void) {
   Py_tss_t *key = (Py_tss_t *)PyObject_Malloc(sizeof(Py_tss_t));
   *key = Py_tss_NEEDS_INIT;
   return key;
 }
 static CYTHON_INLINE void PyThread_tss_free(Py_tss_t *key) {
@@ -397,15 +557,15 @@
 }
 static CYTHON_INLINE int PyThread_tss_set(Py_tss_t *key, void *value) {
   return PyThread_set_key_value(*key, value);
 }
 static CYTHON_INLINE void * PyThread_tss_get(Py_tss_t *key) {
   return PyThread_get_key_value(*key);
 }
-#endif // TSS (Thread Specific Storage) API
+#endif
 #if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
@@ -417,24 +577,36 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
+  #if defined(PyUnicode_IS_READY)
   #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
                                               0 : _PyUnicode_Ready((PyObject *)(op)))
+  #else
+  #define __Pyx_PyUnicode_READY(op)       (0)
+  #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
+  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
+  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #else
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #endif
+  #else
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+  #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
@@ -459,42 +631,51 @@
 #endif
 #if CYTHON_COMPILING_IN_PYPY && !defined(PyByteArray_Check)
   #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
 #endif
 #if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Format)
   #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
 #endif
-#define __Pyx_PyString_FormatSafe(a, b)   ((unlikely((a) == Py_None)) ? PyNumber_Remainder(a, b) : __Pyx_PyString_Format(a, b))
-#define __Pyx_PyUnicode_FormatSafe(a, b)  ((unlikely((a) == Py_None)) ? PyNumber_Remainder(a, b) : PyUnicode_Format(a, b))
+#define __Pyx_PyString_FormatSafe(a, b)   ((unlikely((a) == Py_None || (PyString_Check(b) && !PyString_CheckExact(b)))) ? PyNumber_Remainder(a, b) : __Pyx_PyString_Format(a, b))
+#define __Pyx_PyUnicode_FormatSafe(a, b)  ((unlikely((a) == Py_None || (PyUnicode_Check(b) && !PyUnicode_CheckExact(b)))) ? PyNumber_Remainder(a, b) : PyUnicode_Format(a, b))
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyString_Format(a, b)  PyUnicode_Format(a, b)
 #else
   #define __Pyx_PyString_Format(a, b)  PyString_Format(a, b)
 #endif
 #if PY_MAJOR_VERSION < 3 && !defined(PyObject_ASCII)
   #define PyObject_ASCII(o)            PyObject_Repr(o)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBaseString_Type            PyUnicode_Type
   #define PyStringObject               PyUnicodeObject
   #define PyString_Type                PyUnicode_Type
   #define PyString_Check               PyUnicode_Check
   #define PyString_CheckExact          PyUnicode_CheckExact
+#ifndef PyObject_Unicode
   #define PyObject_Unicode             PyObject_Str
 #endif
+#endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
 #ifndef PySet_CheckExact
   #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
 #endif
+#if PY_VERSION_HEX >= 0x030900A4
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
+#else
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
+#endif
 #if CYTHON_ASSUME_SAFE_MACROS
   #define __Pyx_PySequence_SIZE(seq)  Py_SIZE(seq)
 #else
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
@@ -520,21 +701,21 @@
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? PyMethod_New(func, self) : (Py_INCREF(func), func))
+  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
@@ -548,16 +729,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -567,19 +750,18 @@
 #endif
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
-
+#define __PYX_MARK_ERR_POS(f_index, lineno) \
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
-{ \
-  __pyx_filename = __pyx_f[f_index]; __pyx_lineno = lineno; __pyx_clineno = __LINE__; goto Ln_error; \
-}
+    { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifndef __PYX_EXTERN_C
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
@@ -587,30 +769,37 @@
 
 #define __PYX_HAVE__pymt64
 #define __PYX_HAVE_API__pymt64
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
+#include "numpy/ndarrayobject.h"
+#include "numpy/ndarraytypes.h"
+#include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
+
+    /* NumPy API declarations from "numpy/__init__.pxd" */
+    
 #include "mt64mp.h"
 #include "pymt64lib.h"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
 #endif
 
 typedef struct {PyObject **p; const char *s; const Py_ssize_t n; const char* encoding;
                 const char is_unicode; const char is_str; const char intern; } __Pyx_StringTabEntry;
 
 #define __PYX_DEFAULT_STRING_ENCODING_IS_ASCII 0
-#define __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT 0
+#define __PYX_DEFAULT_STRING_ENCODING_IS_UTF8 0
+#define __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT (PY_MAJOR_VERSION >= 3 && __PYX_DEFAULT_STRING_ENCODING_IS_UTF8)
 #define __PYX_DEFAULT_STRING_ENCODING ""
 #define __Pyx_PyObject_FromString __Pyx_PyBytes_FromString
 #define __Pyx_PyObject_FromStringAndSize __Pyx_PyBytes_FromStringAndSize
 #define __Pyx_uchar_cast(c) ((unsigned char)c)
 #define __Pyx_long_cast(x) ((long)x)
 #define __Pyx_fits_Py_ssize_t(v, type, is_signed)  (\
     (sizeof(type) < sizeof(Py_ssize_t))  ||\
@@ -618,14 +807,17 @@
           likely(v < (type)PY_SSIZE_T_MAX ||\
                  v == (type)PY_SSIZE_T_MAX)  &&\
           (!is_signed || likely(v > (type)PY_SSIZE_T_MIN ||\
                                 v == (type)PY_SSIZE_T_MIN)))  ||\
     (sizeof(type) == sizeof(Py_ssize_t) &&\
           (is_signed || likely(v < (type)PY_SSIZE_T_MAX ||\
                                v == (type)PY_SSIZE_T_MAX)))  )
+static CYTHON_INLINE int __Pyx_is_valid_index(Py_ssize_t i, Py_ssize_t limit) {
+    return (size_t) i < (size_t) limit;
+}
 #if defined (__cplusplus) && __cplusplus >= 201103L
     #include <cstdlib>
     #define __Pyx_sst_abs(value) std::abs(value)
 #elif SIZEOF_INT >= SIZEOF_SIZE_T
     #define __Pyx_sst_abs(value) abs(value)
 #elif SIZEOF_LONG >= SIZEOF_SIZE_T
     #define __Pyx_sst_abs(value) labs(value)
@@ -676,19 +868,21 @@
 #define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
 #define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
+static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
@@ -756,15 +950,15 @@
     sys = PyImport_ImportModule("sys");
     if (!sys) goto bad;
     default_encoding = PyObject_CallMethod(sys, (char*) (const char*) "getdefaultencoding", NULL);
     Py_DECREF(sys);
     if (!default_encoding) goto bad;
     default_encoding_c = PyBytes_AsString(default_encoding);
     if (!default_encoding_c) goto bad;
-    __PYX_DEFAULT_STRING_ENCODING = (char*) malloc(strlen(default_encoding_c));
+    __PYX_DEFAULT_STRING_ENCODING = (char*) malloc(strlen(default_encoding_c) + 1);
     if (!__PYX_DEFAULT_STRING_ENCODING) goto bad;
     strcpy(__PYX_DEFAULT_STRING_ENCODING, default_encoding_c);
     Py_DECREF(default_encoding);
     return 0;
 bad:
     Py_XDECREF(default_encoding);
     return -1;
@@ -856,224 +1050,215 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":730
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":731
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":732
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":733
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":737
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":738
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":739
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":740
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":744
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":745
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":754
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":755
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":756
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":758
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":759
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":760
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":762
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":763
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":765
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":766
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":767
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
 
 /* "pymt64.pyx":68
  * # every type in the numpy module there's a corresponding compile-time
  * # type with a _t-suffix.
  * ctypedef np.double_t DTYPE_t             # <<<<<<<<<<<<<<
- * ctypedef np.int_t ITYPE_t
+ * #ctypedef np.int_t ITYPE_t
  * ctypedef np.uint64_t U64TYPE_t
  */
 typedef __pyx_t_5numpy_double_t __pyx_t_6pymt64_DTYPE_t;
 
-/* "pymt64.pyx":69
- * # type with a _t-suffix.
- * ctypedef np.double_t DTYPE_t
- * ctypedef np.int_t ITYPE_t             # <<<<<<<<<<<<<<
- * ctypedef np.uint64_t U64TYPE_t
- * # "def" can type its arguments but not have a return type. The type of the
- */
-typedef __pyx_t_5numpy_int_t __pyx_t_6pymt64_ITYPE_t;
-
 /* "pymt64.pyx":70
  * ctypedef np.double_t DTYPE_t
- * ctypedef np.int_t ITYPE_t
+ * #ctypedef np.int_t ITYPE_t
  * ctypedef np.uint64_t U64TYPE_t             # <<<<<<<<<<<<<<
  * # "def" can type its arguments but not have a return type. The type of the
  * # arguments for a "def" function is checked at run-time when entering the
  */
 typedef __pyx_t_5numpy_uint64_t __pyx_t_6pymt64_U64TYPE_t;
 /* Declarations.proto */
 #if CYTHON_CCOMPLEX
@@ -1098,42 +1283,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":769
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":770
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":771
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":773
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1208,16 +1393,60 @@
 #else
 #define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
 #endif
 
 /* GetBuiltinName.proto */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name);
 
+/* PyDictVersioning.proto */
+#if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
+#define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
+#define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
+#define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
+    (version_var) = __PYX_GET_DICT_VERSION(dict);\
+    (cache_var) = (value);
+#define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP) {\
+    static PY_UINT64_T __pyx_dict_version = 0;\
+    static PyObject *__pyx_dict_cached_value = NULL;\
+    if (likely(__PYX_GET_DICT_VERSION(DICT) == __pyx_dict_version)) {\
+        (VAR) = __pyx_dict_cached_value;\
+    } else {\
+        (VAR) = __pyx_dict_cached_value = (LOOKUP);\
+        __pyx_dict_version = __PYX_GET_DICT_VERSION(DICT);\
+    }\
+}
+static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj);
+static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj);
+static CYTHON_INLINE int __Pyx_object_dict_version_matches(PyObject* obj, PY_UINT64_T tp_dict_version, PY_UINT64_T obj_dict_version);
+#else
+#define __PYX_GET_DICT_VERSION(dict)  (0)
+#define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
+#define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
+#endif
+
 /* GetModuleGlobalName.proto */
-static CYTHON_INLINE PyObject *__Pyx_GetModuleGlobalName(PyObject *name);
+#if CYTHON_USE_DICT_VERSIONS
+#define __Pyx_GetModuleGlobalName(var, name)  {\
+    static PY_UINT64_T __pyx_dict_version = 0;\
+    static PyObject *__pyx_dict_cached_value = NULL;\
+    (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
+        (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
+        __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
+}
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+    PY_UINT64_T __pyx_dict_version;\
+    PyObject *__pyx_dict_cached_value;\
+    (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
+}
+static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
+#else
+#define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
+static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
+#endif
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
 #endif
@@ -1300,63 +1529,19 @@
 
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
     ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
-/* RaiseException.proto */
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
-
-/* PyCFunctionFastCall.proto */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
-#else
-#define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
+/* GetTopmostException.proto */
+#if CYTHON_USE_EXC_INFO_STACK
+static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
-/* PyFunctionFastCall.proto */
-#if CYTHON_FAST_PYCALL
-#define __Pyx_PyFunction_FastCall(func, args, nargs)\
-    __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
-#if 1 || PY_VERSION_HEX < 0x030600B1
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, int nargs, PyObject *kwargs);
-#else
-#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
-#endif
-#endif
-
-/* PyObjectCallMethO.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
-#endif
-
-/* PyObjectCallOneArg.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
-
-/* DictGetItem.proto */
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
-#define __Pyx_PyObject_Dict_GetItem(obj, name)\
-    (likely(PyDict_CheckExact(obj)) ?\
-     __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
-#else
-#define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
-#define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
-#endif
-
-/* RaiseTooManyValuesToUnpack.proto */
-static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected);
-
-/* RaiseNeedMoreValuesToUnpack.proto */
-static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index);
-
-/* RaiseNoneIterError.proto */
-static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void);
-
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
 #else
@@ -1376,14 +1561,28 @@
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+
+/* TypeImport.proto */
+#ifndef __PYX_HAVE_RT_ImportType_proto
+#define __PYX_HAVE_RT_ImportType_proto
+enum __Pyx_ImportType_CheckSize {
+   __Pyx_ImportType_CheckSize_Error = 0,
+   __Pyx_ImportType_CheckSize_Warn = 1,
+   __Pyx_ImportType_CheckSize_Ignore = 2
+};
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+#endif
+
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
@@ -1428,19 +1627,18 @@
     static void __Pyx_ReleaseBuffer(Py_buffer *view);
 #else
     #define __Pyx_GetBuffer PyObject_GetBuffer
     #define __Pyx_ReleaseBuffer PyBuffer_Release
 #endif
 
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
-
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+/* GCCDiagnostics.proto */
+#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#define __Pyx_HAS_GCC_DIAGNOSTIC
+#endif
 
 /* RealImag.proto */
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     #define __Pyx_CREAL(z) ((z).real())
     #define __Pyx_CIMAG(z) ((z).imag())
   #else
@@ -1532,23 +1730,26 @@
     static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_conj_double(__pyx_t_double_complex);
     #if 1
         static CYTHON_INLINE double __Pyx_c_abs_double(__pyx_t_double_complex);
         static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_pow_double(__pyx_t_double_complex, __pyx_t_double_complex);
     #endif
 #endif
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value);
-
 /* CIntFromPy.proto */
 static CYTHON_INLINE unsigned PY_LONG_LONG __Pyx_PyInt_As_unsigned_PY_LONG_LONG(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
@@ -1560,29 +1761,14 @@
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
-/* PyIdentifierFromString.proto */
-#if !defined(__Pyx_PyIdentifier_FromString)
-#if PY_MAJOR_VERSION < 3
-  #define __Pyx_PyIdentifier_FromString(s) PyString_FromString(s)
-#else
-  #define __Pyx_PyIdentifier_FromString(s) PyUnicode_FromString(s)
-#endif
-#endif
-
-/* ModuleImport.proto */
-static PyObject *__Pyx_ImportModule(const char *name);
-
-/* TypeImport.proto */
-static PyTypeObject *__Pyx_ImportType(const char *module_name, const char *class_name, size_t size, int strict);
-
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
 /* Module declarations from 'cpython.buffer' */
 
 /* Module declarations from 'libc.string' */
@@ -1605,164 +1791,144 @@
 /* Module declarations from 'numpy' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
+static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
+static PyTypeObject *__pyx_ptype_5numpy_number = 0;
+static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
+static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
+static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
+static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
-static CYTHON_INLINE char *__pyx_f_5numpy__util_dtypestring(PyArray_Descr *, char *, char *, int *); /*proto*/
 
 /* Module declarations from 'cython' */
 
 /* Module declarations from 'pymt64' */
 static int __pyx_v_6pymt64_MTSIZE;
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_6pymt64_U64TYPE_t = { "U64TYPE_t", NULL, sizeof(__pyx_t_6pymt64_U64TYPE_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_6pymt64_U64TYPE_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_6pymt64_U64TYPE_t), 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_6pymt64_DTYPE_t = { "DTYPE_t", NULL, sizeof(__pyx_t_6pymt64_DTYPE_t), { 0 }, 0, 'R', 0, 0 };
 #define __Pyx_MODULE_NAME "pymt64"
 extern int __pyx_module_is_main_pymt64;
 int __pyx_module_is_main_pymt64 = 0;
 
 /* Implementation of 'pymt64' */
-static PyObject *__pyx_builtin_ValueError;
-static PyObject *__pyx_builtin_range;
-static PyObject *__pyx_builtin_RuntimeError;
 static PyObject *__pyx_builtin_ImportError;
 static const char __pyx_k_n[] = "n";
 static const char __pyx_k_mt[] = "mt";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_xm[] = "xm";
-static const char __pyx_k_int[] = "int";
 static const char __pyx_k_init[] = "init";
 static const char __pyx_k_main[] = "__main__";
+static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_seed[] = "seed";
 static const char __pyx_k_size[] = "size";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_DTYPE[] = "DTYPE";
-static const char __pyx_k_ITYPE[] = "ITYPE";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_numpy[] = "numpy";
-static const char __pyx_k_range[] = "range";
 static const char __pyx_k_zeros[] = "zeros";
 static const char __pyx_k_double[] = "double";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_normal[] = "normal";
 static const char __pyx_k_pymt64[] = "pymt64";
 static const char __pyx_k_series[] = "series";
 static const char __pyx_k_uint64[] = "uint64";
 static const char __pyx_k_U64TYPE[] = "U64TYPE";
 static const char __pyx_k_counter[] = "counter";
 static const char __pyx_k_poisson[] = "poisson";
 static const char __pyx_k_series1[] = "series1";
 static const char __pyx_k_series2[] = "series2";
 static const char __pyx_k_uniform[] = "uniform";
-static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_pymt64_pyx[] = "pymt64.pyx";
 static const char __pyx_k_ImportError[] = "ImportError";
-static const char __pyx_k_RuntimeError[] = "RuntimeError";
 static const char __pyx_k_poisson_multlam[] = "poisson_multlam";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
-static const char __pyx_k_ndarray_is_not_C_contiguous[] = "ndarray is not C contiguous";
 static const char __pyx_k_PyMT64_PyMT64_is_a_Python_versi[] = "\n                     PyMT64\n                     \nPyMT64 is a Python version of the Mersenne Twister (MT) 64-bit pseudorandom number generator by Takuji Nishimura and Makoto Matsumoto (see http://www.math.sci.hiroshima-u.ac.jp/~m-mat/MT/emt64.html and the references below).\n\nThis customised version is thread safe and was interfaced from C to Python (see pymt64.c)\n\nThis module provides the following methods:\n- init : initialization of the state vector (mt) used by the pseudorandom number generator (PNG)\n- uniform : generation of an uniform distribution\n- normal : generation of two Normal distributions\n- poisson : generation of a Poisson distribution\n\nThe period of the PNG is 2**19937-1.\n\nExample:\n    import pymt64\n    seed = 143439545 seed # the initial seed\n    mt = pymt64.init(seed) # initialisation of the state vector of MT\n    u = pymt64.uniform(mt,10) # generation of an uniform distribution\n    print (u)\n   [0.12444525 0.22084376 0.31059967 0.45578589 0.84743752 0.28825306\n    0.83320389 0.05085032 0.48682253 0.17667076]\n\nFor a complete example, see pymt64_test.py\n\nNote: the state vector 'mt' returned by pymt64.init has 313 elements instead of the 312 elements of the original C code. This is because the 313th element store the associated counter (mti).\n\nChange history:\n1.9 : correct bug associated with the normal distribution\n1.8 : include a missing file\n1.7 : corrected data package contain\n1.6 : correct wrong size of the state vector \n1.5 : module interface is now based on Cython, module now compatibily with python 3\n1.4 : link problem fixed\n1.3 : fixe a compilation problem regading the Numpy include directory\n1.2 : the previous implementation of the poisson distribution was not thread safe\n1.1 : fix a problem with the initialization of the seed  (in the previous version the seed set by init() was not taken into account such that the results were not reproductible)\n1.0 : initial version\n\n\nR. Samadi (LESIA, Observatoire ""de Paris), 22 Dec. 2012        \n\nReferences:\n   T. Nishimura, ``Tables of 64-bit Mersenne Twisters''\n     ACM Transactions on Modeling and \n     Computer Simulation 10. (2000) 348--357.\n   M. Matsumoto and T. Nishimura,\n     ``Mersenne Twister: a 623-dimensionally equidistributed\n       uniform pseudorandom number generator''\n     ACM Transactions on Modeling and \n     Computer Simulation 8. (Jan. 1998) 3--30.\n";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
-static const char __pyx_k_unknown_dtype_code_in_numpy_pxd[] = "unknown dtype code in numpy.pxd (%d)";
-static const char __pyx_k_Format_string_allocated_too_shor[] = "Format string allocated too short, see comment in numpy.pxd";
-static const char __pyx_k_Non_native_byte_order_not_suppor[] = "Non-native byte order not supported";
-static const char __pyx_k_ndarray_is_not_Fortran_contiguou[] = "ndarray is not Fortran contiguous";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
-static const char __pyx_k_Format_string_allocated_too_shor_2[] = "Format string allocated too short.";
 static PyObject *__pyx_n_s_DTYPE;
-static PyObject *__pyx_kp_u_Format_string_allocated_too_shor;
-static PyObject *__pyx_kp_u_Format_string_allocated_too_shor_2;
-static PyObject *__pyx_n_s_ITYPE;
 static PyObject *__pyx_n_s_ImportError;
-static PyObject *__pyx_kp_u_Non_native_byte_order_not_suppor;
-static PyObject *__pyx_n_s_RuntimeError;
 static PyObject *__pyx_n_s_U64TYPE;
-static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_counter;
 static PyObject *__pyx_n_s_double;
 static PyObject *__pyx_n_s_dtype;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_init;
-static PyObject *__pyx_n_s_int;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_mt;
 static PyObject *__pyx_n_s_n;
-static PyObject *__pyx_kp_u_ndarray_is_not_C_contiguous;
-static PyObject *__pyx_kp_u_ndarray_is_not_Fortran_contiguou;
+static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_normal;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_kp_s_numpy_core_multiarray_failed_to;
 static PyObject *__pyx_kp_s_numpy_core_umath_failed_to_impor;
 static PyObject *__pyx_n_s_poisson;
 static PyObject *__pyx_n_s_poisson_multlam;
 static PyObject *__pyx_n_s_pymt64;
 static PyObject *__pyx_kp_s_pymt64_pyx;
-static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_seed;
 static PyObject *__pyx_n_s_series;
 static PyObject *__pyx_n_s_series1;
 static PyObject *__pyx_n_s_series2;
 static PyObject *__pyx_n_s_size;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_uint64;
 static PyObject *__pyx_n_s_uniform;
-static PyObject *__pyx_kp_u_unknown_dtype_code_in_numpy_pxd;
 static PyObject *__pyx_n_s_xm;
 static PyObject *__pyx_n_s_zeros;
 static PyObject *__pyx_pf_6pymt64_init(CYTHON_UNUSED PyObject *__pyx_self, unsigned PY_LONG_LONG __pyx_v_seed); /* proto */
 static PyObject *__pyx_pf_6pymt64_2uniform(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_mt, int __pyx_v_n); /* proto */
 static PyObject *__pyx_pf_6pymt64_4poisson(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_mt, double __pyx_v_xm, int __pyx_v_n); /* proto */
 static PyObject *__pyx_pf_6pymt64_6normal(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_mt, int __pyx_v_n); /* proto */
 static PyObject *__pyx_pf_6pymt64_8poisson_multlam(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_mt, PyArrayObject *__pyx_v_xm); /* proto */
-static int __pyx_pf_5numpy_7ndarray___getbuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
-static void __pyx_pf_5numpy_7ndarray_2__releasebuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info); /* proto */
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
-static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
-static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__7;
-static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__9;
-static PyObject *__pyx_tuple__10;
-static PyObject *__pyx_tuple__12;
-static PyObject *__pyx_tuple__14;
-static PyObject *__pyx_tuple__16;
-static PyObject *__pyx_tuple__18;
-static PyObject *__pyx_codeobj__11;
-static PyObject *__pyx_codeobj__13;
-static PyObject *__pyx_codeobj__15;
-static PyObject *__pyx_codeobj__17;
-static PyObject *__pyx_codeobj__19;
+static PyObject *__pyx_tuple__11;
+static PyObject *__pyx_codeobj__4;
+static PyObject *__pyx_codeobj__6;
+static PyObject *__pyx_codeobj__8;
+static PyObject *__pyx_codeobj__10;
+static PyObject *__pyx_codeobj__12;
 /* Late includes */
 
-/* "pymt64.pyx":87
- *     cdef void poissonn_multlam( UL64 * mt , int * mti , double * xm, double * x , long n )
+/* "pymt64.pyx":88
+ * 
  * 
  * def init(unsigned long long  seed ):             # <<<<<<<<<<<<<<
  *     '''
  *     Function used to initialise the state vector mt used by the pseudorandom number generator.
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6pymt64_1init(PyObject *__pyx_self, PyObject *__pyx_arg_seed); /*proto*/
 static char __pyx_doc_6pymt64_init[] = "\n    Function used to initialise the state vector mt used by the pseudorandom number generator.\n    \n    mt = init(seed)\n    \n    ";
 static PyMethodDef __pyx_mdef_6pymt64_1init = {"init", (PyCFunction)__pyx_pw_6pymt64_1init, METH_O, __pyx_doc_6pymt64_init};
 static PyObject *__pyx_pw_6pymt64_1init(PyObject *__pyx_self, PyObject *__pyx_arg_seed) {
   unsigned PY_LONG_LONG __pyx_v_seed;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("init (wrapper)", 0);
   assert(__pyx_arg_seed); {
-    __pyx_v_seed = __Pyx_PyInt_As_unsigned_PY_LONG_LONG(__pyx_arg_seed); if (unlikely((__pyx_v_seed == (unsigned PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 87, __pyx_L3_error)
+    __pyx_v_seed = __Pyx_PyInt_As_unsigned_PY_LONG_LONG(__pyx_arg_seed); if (unlikely((__pyx_v_seed == (unsigned PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("pymt64.init", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -1783,142 +1949,143 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyArrayObject *__pyx_t_5 = NULL;
   Py_ssize_t __pyx_t_6;
   int __pyx_t_7;
-  Py_ssize_t __pyx_t_8;
-  Py_ssize_t __pyx_t_9;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("init", 0);
   __pyx_pybuffer_mt.pybuffer.buf = NULL;
   __pyx_pybuffer_mt.refcount = 0;
   __pyx_pybuffernd_mt.data = NULL;
   __pyx_pybuffernd_mt.rcbuffer = &__pyx_pybuffer_mt;
 
-  /* "pymt64.pyx":94
+  /* "pymt64.pyx":95
  * 
  *     '''
  *     cdef np.ndarray [U64TYPE_t,ndim=1, mode='c'] mt = np.zeros([MTSIZE+1], dtype=U64TYPE)             # <<<<<<<<<<<<<<
  *     cdef int counter = mt[MTSIZE]
  *     #      the state vector 'mt'  has MTSIZE+1  elements
  */
-  __pyx_t_1 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_long((__pyx_v_6pymt64_MTSIZE + 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_long((__pyx_v_6pymt64_MTSIZE + 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_GetModuleGlobalName(__pyx_n_s_U64TYPE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_U64TYPE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 94, __pyx_L1_error)
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 95, __pyx_L1_error)
   __pyx_t_5 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_mt.rcbuffer->pybuffer, (PyObject*)__pyx_t_5, &__Pyx_TypeInfo_nn___pyx_t_6pymt64_U64TYPE_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_mt = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 94, __pyx_L1_error)
+      __PYX_ERR(0, 95, __pyx_L1_error)
     } else {__pyx_pybuffernd_mt.diminfo[0].strides = __pyx_pybuffernd_mt.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_mt.diminfo[0].shape = __pyx_pybuffernd_mt.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_5 = 0;
   __pyx_v_mt = ((PyArrayObject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "pymt64.pyx":95
+  /* "pymt64.pyx":96
  *     '''
  *     cdef np.ndarray [U64TYPE_t,ndim=1, mode='c'] mt = np.zeros([MTSIZE+1], dtype=U64TYPE)
  *     cdef int counter = mt[MTSIZE]             # <<<<<<<<<<<<<<
  *     #      the state vector 'mt'  has MTSIZE+1  elements
  *     # instead of the MTSIZE  elements of the original C code.
  */
   __pyx_t_6 = __pyx_v_6pymt64_MTSIZE;
   __pyx_t_7 = -1;
   if (__pyx_t_6 < 0) {
     __pyx_t_6 += __pyx_pybuffernd_mt.diminfo[0].shape;
     if (unlikely(__pyx_t_6 < 0)) __pyx_t_7 = 0;
   } else if (unlikely(__pyx_t_6 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_7 = 0;
   if (unlikely(__pyx_t_7 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_7);
-    __PYX_ERR(0, 95, __pyx_L1_error)
+    __PYX_ERR(0, 96, __pyx_L1_error)
   }
   __pyx_v_counter = (*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_6, __pyx_pybuffernd_mt.diminfo[0].strides));
 
-  /* "pymt64.pyx":100
+  /* "pymt64.pyx":101
  *     # This is because the last element stores the associated counter (mti).
  * 
  *     init_genrand64(seed , &mt[0] , &counter )             # <<<<<<<<<<<<<<
  *     mt[MTSIZE] = counter
  * 
  */
-  __pyx_t_8 = 0;
+  __pyx_t_6 = 0;
   __pyx_t_7 = -1;
-  if (__pyx_t_8 < 0) {
-    __pyx_t_8 += __pyx_pybuffernd_mt.diminfo[0].shape;
-    if (unlikely(__pyx_t_8 < 0)) __pyx_t_7 = 0;
-  } else if (unlikely(__pyx_t_8 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_7 = 0;
+  if (__pyx_t_6 < 0) {
+    __pyx_t_6 += __pyx_pybuffernd_mt.diminfo[0].shape;
+    if (unlikely(__pyx_t_6 < 0)) __pyx_t_7 = 0;
+  } else if (unlikely(__pyx_t_6 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_7 = 0;
   if (unlikely(__pyx_t_7 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_7);
-    __PYX_ERR(0, 100, __pyx_L1_error)
+    __PYX_ERR(0, 101, __pyx_L1_error)
   }
-  init_genrand64(__pyx_v_seed, (&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_mt.diminfo[0].strides))), (&__pyx_v_counter));
+  init_genrand64(__pyx_v_seed, (&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_6, __pyx_pybuffernd_mt.diminfo[0].strides))), (&__pyx_v_counter));
 
-  /* "pymt64.pyx":101
+  /* "pymt64.pyx":102
  * 
  *     init_genrand64(seed , &mt[0] , &counter )
  *     mt[MTSIZE] = counter             # <<<<<<<<<<<<<<
  * 
  *     return mt
  */
-  __pyx_t_9 = __pyx_v_6pymt64_MTSIZE;
+  __pyx_t_6 = __pyx_v_6pymt64_MTSIZE;
   __pyx_t_7 = -1;
-  if (__pyx_t_9 < 0) {
-    __pyx_t_9 += __pyx_pybuffernd_mt.diminfo[0].shape;
-    if (unlikely(__pyx_t_9 < 0)) __pyx_t_7 = 0;
-  } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_7 = 0;
+  if (__pyx_t_6 < 0) {
+    __pyx_t_6 += __pyx_pybuffernd_mt.diminfo[0].shape;
+    if (unlikely(__pyx_t_6 < 0)) __pyx_t_7 = 0;
+  } else if (unlikely(__pyx_t_6 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_7 = 0;
   if (unlikely(__pyx_t_7 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_7);
-    __PYX_ERR(0, 101, __pyx_L1_error)
+    __PYX_ERR(0, 102, __pyx_L1_error)
   }
-  *__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_mt.diminfo[0].strides) = __pyx_v_counter;
+  *__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_6, __pyx_pybuffernd_mt.diminfo[0].strides) = __pyx_v_counter;
 
-  /* "pymt64.pyx":103
+  /* "pymt64.pyx":104
  *     mt[MTSIZE] = counter
  * 
  *     return mt             # <<<<<<<<<<<<<<
  * 
  * def uniform(np.ndarray [U64TYPE_t,ndim=1, mode='c'] mt , int n):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_mt));
   __pyx_r = ((PyObject *)__pyx_v_mt);
   goto __pyx_L0;
 
-  /* "pymt64.pyx":87
- *     cdef void poissonn_multlam( UL64 * mt , int * mti , double * xm, double * x , long n )
+  /* "pymt64.pyx":88
+ * 
  * 
  * def init(unsigned long long  seed ):             # <<<<<<<<<<<<<<
  *     '''
  *     Function used to initialise the state vector mt used by the pseudorandom number generator.
  */
 
   /* function exit code */
@@ -1941,29 +2108,32 @@
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_mt);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pymt64.pyx":105
+/* "pymt64.pyx":106
  *     return mt
  * 
  * def uniform(np.ndarray [U64TYPE_t,ndim=1, mode='c'] mt , int n):             # <<<<<<<<<<<<<<
  *     '''
  *     Generates n random numbers on [0,1]-real-interval
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6pymt64_3uniform(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_6pymt64_2uniform[] = "\n    Generates n random numbers on [0,1]-real-interval\n    \n    x = uniform(mt,n)\n    \n    ";
-static PyMethodDef __pyx_mdef_6pymt64_3uniform = {"uniform", (PyCFunction)__pyx_pw_6pymt64_3uniform, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6pymt64_2uniform};
+static PyMethodDef __pyx_mdef_6pymt64_3uniform = {"uniform", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6pymt64_3uniform, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6pymt64_2uniform};
 static PyObject *__pyx_pw_6pymt64_3uniform(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyArrayObject *__pyx_v_mt = 0;
   int __pyx_v_n;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("uniform (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_mt,&__pyx_n_s_n,0};
     PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
@@ -1982,38 +2152,38 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mt)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_n)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("uniform", 1, 2, 2, 1); __PYX_ERR(0, 105, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("uniform", 1, 2, 2, 1); __PYX_ERR(0, 106, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "uniform") < 0)) __PYX_ERR(0, 105, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "uniform") < 0)) __PYX_ERR(0, 106, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_mt = ((PyArrayObject *)values[0]);
-    __pyx_v_n = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_n == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
+    __pyx_v_n = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_n == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 106, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("uniform", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 105, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("uniform", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 106, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pymt64.uniform", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_mt), __pyx_ptype_5numpy_ndarray, 1, "mt", 0))) __PYX_ERR(0, 105, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_mt), __pyx_ptype_5numpy_ndarray, 1, "mt", 0))) __PYX_ERR(0, 106, __pyx_L1_error)
   __pyx_r = __pyx_pf_6pymt64_2uniform(__pyx_self, __pyx_v_mt, __pyx_v_n);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -2034,155 +2204,156 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyArrayObject *__pyx_t_5 = NULL;
   Py_ssize_t __pyx_t_6;
   int __pyx_t_7;
   Py_ssize_t __pyx_t_8;
-  Py_ssize_t __pyx_t_9;
-  Py_ssize_t __pyx_t_10;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("uniform", 0);
   __pyx_pybuffer_series.pybuffer.buf = NULL;
   __pyx_pybuffer_series.refcount = 0;
   __pyx_pybuffernd_series.data = NULL;
   __pyx_pybuffernd_series.rcbuffer = &__pyx_pybuffer_series;
   __pyx_pybuffer_mt.pybuffer.buf = NULL;
   __pyx_pybuffer_mt.refcount = 0;
   __pyx_pybuffernd_mt.data = NULL;
   __pyx_pybuffernd_mt.rcbuffer = &__pyx_pybuffer_mt;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_mt.rcbuffer->pybuffer, (PyObject*)__pyx_v_mt, &__Pyx_TypeInfo_nn___pyx_t_6pymt64_U64TYPE_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 105, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_mt.rcbuffer->pybuffer, (PyObject*)__pyx_v_mt, &__Pyx_TypeInfo_nn___pyx_t_6pymt64_U64TYPE_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 106, __pyx_L1_error)
   }
   __pyx_pybuffernd_mt.diminfo[0].strides = __pyx_pybuffernd_mt.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_mt.diminfo[0].shape = __pyx_pybuffernd_mt.rcbuffer->pybuffer.shape[0];
 
-  /* "pymt64.pyx":113
+  /* "pymt64.pyx":114
  *     '''
  * 
  *     cdef np.ndarray [DTYPE_t,ndim=1, mode='c'] series = np.zeros(n, dtype=DTYPE)             # <<<<<<<<<<<<<<
  *     cdef int counter = mt[MTSIZE]
  * 
  */
-  __pyx_t_1 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_GetModuleGlobalName(__pyx_n_s_DTYPE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 113, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 113, __pyx_L1_error)
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 114, __pyx_L1_error)
   __pyx_t_5 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_series.rcbuffer->pybuffer, (PyObject*)__pyx_t_5, &__Pyx_TypeInfo_nn___pyx_t_6pymt64_DTYPE_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_series = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_series.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 113, __pyx_L1_error)
+      __PYX_ERR(0, 114, __pyx_L1_error)
     } else {__pyx_pybuffernd_series.diminfo[0].strides = __pyx_pybuffernd_series.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_series.diminfo[0].shape = __pyx_pybuffernd_series.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_5 = 0;
   __pyx_v_series = ((PyArrayObject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "pymt64.pyx":114
+  /* "pymt64.pyx":115
  * 
  *     cdef np.ndarray [DTYPE_t,ndim=1, mode='c'] series = np.zeros(n, dtype=DTYPE)
  *     cdef int counter = mt[MTSIZE]             # <<<<<<<<<<<<<<
  * 
  *     uniformn( &mt[0]  , &counter , &series[0], n)
  */
   __pyx_t_6 = __pyx_v_6pymt64_MTSIZE;
   __pyx_t_7 = -1;
   if (__pyx_t_6 < 0) {
     __pyx_t_6 += __pyx_pybuffernd_mt.diminfo[0].shape;
     if (unlikely(__pyx_t_6 < 0)) __pyx_t_7 = 0;
   } else if (unlikely(__pyx_t_6 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_7 = 0;
   if (unlikely(__pyx_t_7 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_7);
-    __PYX_ERR(0, 114, __pyx_L1_error)
+    __PYX_ERR(0, 115, __pyx_L1_error)
   }
   __pyx_v_counter = (*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_6, __pyx_pybuffernd_mt.diminfo[0].strides));
 
-  /* "pymt64.pyx":116
+  /* "pymt64.pyx":117
  *     cdef int counter = mt[MTSIZE]
  * 
  *     uniformn( &mt[0]  , &counter , &series[0], n)             # <<<<<<<<<<<<<<
  *     mt[MTSIZE] = counter
  * 
  */
-  __pyx_t_8 = 0;
+  __pyx_t_6 = 0;
   __pyx_t_7 = -1;
-  if (__pyx_t_8 < 0) {
-    __pyx_t_8 += __pyx_pybuffernd_mt.diminfo[0].shape;
-    if (unlikely(__pyx_t_8 < 0)) __pyx_t_7 = 0;
-  } else if (unlikely(__pyx_t_8 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_7 = 0;
+  if (__pyx_t_6 < 0) {
+    __pyx_t_6 += __pyx_pybuffernd_mt.diminfo[0].shape;
+    if (unlikely(__pyx_t_6 < 0)) __pyx_t_7 = 0;
+  } else if (unlikely(__pyx_t_6 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_7 = 0;
   if (unlikely(__pyx_t_7 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_7);
-    __PYX_ERR(0, 116, __pyx_L1_error)
+    __PYX_ERR(0, 117, __pyx_L1_error)
   }
-  __pyx_t_9 = 0;
+  __pyx_t_8 = 0;
   __pyx_t_7 = -1;
-  if (__pyx_t_9 < 0) {
-    __pyx_t_9 += __pyx_pybuffernd_series.diminfo[0].shape;
-    if (unlikely(__pyx_t_9 < 0)) __pyx_t_7 = 0;
-  } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_series.diminfo[0].shape)) __pyx_t_7 = 0;
+  if (__pyx_t_8 < 0) {
+    __pyx_t_8 += __pyx_pybuffernd_series.diminfo[0].shape;
+    if (unlikely(__pyx_t_8 < 0)) __pyx_t_7 = 0;
+  } else if (unlikely(__pyx_t_8 >= __pyx_pybuffernd_series.diminfo[0].shape)) __pyx_t_7 = 0;
   if (unlikely(__pyx_t_7 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_7);
-    __PYX_ERR(0, 116, __pyx_L1_error)
+    __PYX_ERR(0, 117, __pyx_L1_error)
   }
-  uniformn((&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_mt.diminfo[0].strides))), (&__pyx_v_counter), (&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_DTYPE_t *, __pyx_pybuffernd_series.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_series.diminfo[0].strides))), __pyx_v_n);
+  uniformn((&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_6, __pyx_pybuffernd_mt.diminfo[0].strides))), (&__pyx_v_counter), (&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_DTYPE_t *, __pyx_pybuffernd_series.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_series.diminfo[0].strides))), __pyx_v_n);
 
-  /* "pymt64.pyx":117
+  /* "pymt64.pyx":118
  * 
  *     uniformn( &mt[0]  , &counter , &series[0], n)
  *     mt[MTSIZE] = counter             # <<<<<<<<<<<<<<
  * 
  *     return series
  */
-  __pyx_t_10 = __pyx_v_6pymt64_MTSIZE;
+  __pyx_t_8 = __pyx_v_6pymt64_MTSIZE;
   __pyx_t_7 = -1;
-  if (__pyx_t_10 < 0) {
-    __pyx_t_10 += __pyx_pybuffernd_mt.diminfo[0].shape;
-    if (unlikely(__pyx_t_10 < 0)) __pyx_t_7 = 0;
-  } else if (unlikely(__pyx_t_10 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_7 = 0;
+  if (__pyx_t_8 < 0) {
+    __pyx_t_8 += __pyx_pybuffernd_mt.diminfo[0].shape;
+    if (unlikely(__pyx_t_8 < 0)) __pyx_t_7 = 0;
+  } else if (unlikely(__pyx_t_8 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_7 = 0;
   if (unlikely(__pyx_t_7 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_7);
-    __PYX_ERR(0, 117, __pyx_L1_error)
+    __PYX_ERR(0, 118, __pyx_L1_error)
   }
-  *__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_mt.diminfo[0].strides) = __pyx_v_counter;
+  *__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_mt.diminfo[0].strides) = __pyx_v_counter;
 
-  /* "pymt64.pyx":119
+  /* "pymt64.pyx":120
  *     mt[MTSIZE] = counter
  * 
  *     return series             # <<<<<<<<<<<<<<
  * 
  * def poisson(np.ndarray [U64TYPE_t,ndim=1, mode='c'] mt , double xm , int n):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_series));
   __pyx_r = ((PyObject *)__pyx_v_series);
   goto __pyx_L0;
 
-  /* "pymt64.pyx":105
+  /* "pymt64.pyx":106
  *     return mt
  * 
  * def uniform(np.ndarray [U64TYPE_t,ndim=1, mode='c'] mt , int n):             # <<<<<<<<<<<<<<
  *     '''
  *     Generates n random numbers on [0,1]-real-interval
  */
 
@@ -2208,30 +2379,33 @@
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_series);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pymt64.pyx":121
+/* "pymt64.pyx":122
  *     return series
  * 
  * def poisson(np.ndarray [U64TYPE_t,ndim=1, mode='c'] mt , double xm , int n):             # <<<<<<<<<<<<<<
  *     '''
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6pymt64_5poisson(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_6pymt64_4poisson[] = "\n    \n    Generates a Poisson distribution of mean mu.\n\n    x = poisson(mt,mu,n)\n  \n    ";
-static PyMethodDef __pyx_mdef_6pymt64_5poisson = {"poisson", (PyCFunction)__pyx_pw_6pymt64_5poisson, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6pymt64_4poisson};
+static PyMethodDef __pyx_mdef_6pymt64_5poisson = {"poisson", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6pymt64_5poisson, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6pymt64_4poisson};
 static PyObject *__pyx_pw_6pymt64_5poisson(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyArrayObject *__pyx_v_mt = 0;
   double __pyx_v_xm;
   int __pyx_v_n;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("poisson (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_mt,&__pyx_n_s_xm,&__pyx_n_s_n,0};
     PyObject* values[3] = {0,0,0};
     if (unlikely(__pyx_kwds)) {
@@ -2252,46 +2426,46 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mt)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_xm)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("poisson", 1, 3, 3, 1); __PYX_ERR(0, 121, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("poisson", 1, 3, 3, 1); __PYX_ERR(0, 122, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_n)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("poisson", 1, 3, 3, 2); __PYX_ERR(0, 121, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("poisson", 1, 3, 3, 2); __PYX_ERR(0, 122, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "poisson") < 0)) __PYX_ERR(0, 121, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "poisson") < 0)) __PYX_ERR(0, 122, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_mt = ((PyArrayObject *)values[0]);
-    __pyx_v_xm = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_xm == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 121, __pyx_L3_error)
-    __pyx_v_n = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_n == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 121, __pyx_L3_error)
+    __pyx_v_xm = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_xm == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 122, __pyx_L3_error)
+    __pyx_v_n = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_n == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 122, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("poisson", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 121, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("poisson", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 122, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pymt64.poisson", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_mt), __pyx_ptype_5numpy_ndarray, 1, "mt", 0))) __PYX_ERR(0, 121, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_mt), __pyx_ptype_5numpy_ndarray, 1, "mt", 0))) __PYX_ERR(0, 122, __pyx_L1_error)
   __pyx_r = __pyx_pf_6pymt64_4poisson(__pyx_self, __pyx_v_mt, __pyx_v_xm, __pyx_v_n);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -2312,155 +2486,156 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyArrayObject *__pyx_t_5 = NULL;
   Py_ssize_t __pyx_t_6;
   int __pyx_t_7;
   Py_ssize_t __pyx_t_8;
-  Py_ssize_t __pyx_t_9;
-  Py_ssize_t __pyx_t_10;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("poisson", 0);
   __pyx_pybuffer_series.pybuffer.buf = NULL;
   __pyx_pybuffer_series.refcount = 0;
   __pyx_pybuffernd_series.data = NULL;
   __pyx_pybuffernd_series.rcbuffer = &__pyx_pybuffer_series;
   __pyx_pybuffer_mt.pybuffer.buf = NULL;
   __pyx_pybuffer_mt.refcount = 0;
   __pyx_pybuffernd_mt.data = NULL;
   __pyx_pybuffernd_mt.rcbuffer = &__pyx_pybuffer_mt;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_mt.rcbuffer->pybuffer, (PyObject*)__pyx_v_mt, &__Pyx_TypeInfo_nn___pyx_t_6pymt64_U64TYPE_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 121, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_mt.rcbuffer->pybuffer, (PyObject*)__pyx_v_mt, &__Pyx_TypeInfo_nn___pyx_t_6pymt64_U64TYPE_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 122, __pyx_L1_error)
   }
   __pyx_pybuffernd_mt.diminfo[0].strides = __pyx_pybuffernd_mt.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_mt.diminfo[0].shape = __pyx_pybuffernd_mt.rcbuffer->pybuffer.shape[0];
 
-  /* "pymt64.pyx":130
+  /* "pymt64.pyx":131
  *     '''
  * 
  *     cdef np.ndarray [DTYPE_t,ndim=1, mode='c'] series = np.zeros(n, dtype=DTYPE)             # <<<<<<<<<<<<<<
  *     cdef int counter = mt[MTSIZE]
  * 
  */
-  __pyx_t_1 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_GetModuleGlobalName(__pyx_n_s_DTYPE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 130, __pyx_L1_error)
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 131, __pyx_L1_error)
   __pyx_t_5 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_series.rcbuffer->pybuffer, (PyObject*)__pyx_t_5, &__Pyx_TypeInfo_nn___pyx_t_6pymt64_DTYPE_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_series = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_series.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 130, __pyx_L1_error)
+      __PYX_ERR(0, 131, __pyx_L1_error)
     } else {__pyx_pybuffernd_series.diminfo[0].strides = __pyx_pybuffernd_series.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_series.diminfo[0].shape = __pyx_pybuffernd_series.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_5 = 0;
   __pyx_v_series = ((PyArrayObject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "pymt64.pyx":131
+  /* "pymt64.pyx":132
  * 
  *     cdef np.ndarray [DTYPE_t,ndim=1, mode='c'] series = np.zeros(n, dtype=DTYPE)
  *     cdef int counter = mt[MTSIZE]             # <<<<<<<<<<<<<<
  * 
  *     poissonn( &mt[0] , &counter ,xm, &series[0], n)
  */
   __pyx_t_6 = __pyx_v_6pymt64_MTSIZE;
   __pyx_t_7 = -1;
   if (__pyx_t_6 < 0) {
     __pyx_t_6 += __pyx_pybuffernd_mt.diminfo[0].shape;
     if (unlikely(__pyx_t_6 < 0)) __pyx_t_7 = 0;
   } else if (unlikely(__pyx_t_6 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_7 = 0;
   if (unlikely(__pyx_t_7 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_7);
-    __PYX_ERR(0, 131, __pyx_L1_error)
+    __PYX_ERR(0, 132, __pyx_L1_error)
   }
   __pyx_v_counter = (*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_6, __pyx_pybuffernd_mt.diminfo[0].strides));
 
-  /* "pymt64.pyx":133
+  /* "pymt64.pyx":134
  *     cdef int counter = mt[MTSIZE]
  * 
  *     poissonn( &mt[0] , &counter ,xm, &series[0], n)             # <<<<<<<<<<<<<<
  *     mt[MTSIZE] = counter
  * 
  */
-  __pyx_t_8 = 0;
+  __pyx_t_6 = 0;
   __pyx_t_7 = -1;
-  if (__pyx_t_8 < 0) {
-    __pyx_t_8 += __pyx_pybuffernd_mt.diminfo[0].shape;
-    if (unlikely(__pyx_t_8 < 0)) __pyx_t_7 = 0;
-  } else if (unlikely(__pyx_t_8 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_7 = 0;
+  if (__pyx_t_6 < 0) {
+    __pyx_t_6 += __pyx_pybuffernd_mt.diminfo[0].shape;
+    if (unlikely(__pyx_t_6 < 0)) __pyx_t_7 = 0;
+  } else if (unlikely(__pyx_t_6 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_7 = 0;
   if (unlikely(__pyx_t_7 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_7);
-    __PYX_ERR(0, 133, __pyx_L1_error)
+    __PYX_ERR(0, 134, __pyx_L1_error)
   }
-  __pyx_t_9 = 0;
+  __pyx_t_8 = 0;
   __pyx_t_7 = -1;
-  if (__pyx_t_9 < 0) {
-    __pyx_t_9 += __pyx_pybuffernd_series.diminfo[0].shape;
-    if (unlikely(__pyx_t_9 < 0)) __pyx_t_7 = 0;
-  } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_series.diminfo[0].shape)) __pyx_t_7 = 0;
+  if (__pyx_t_8 < 0) {
+    __pyx_t_8 += __pyx_pybuffernd_series.diminfo[0].shape;
+    if (unlikely(__pyx_t_8 < 0)) __pyx_t_7 = 0;
+  } else if (unlikely(__pyx_t_8 >= __pyx_pybuffernd_series.diminfo[0].shape)) __pyx_t_7 = 0;
   if (unlikely(__pyx_t_7 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_7);
-    __PYX_ERR(0, 133, __pyx_L1_error)
+    __PYX_ERR(0, 134, __pyx_L1_error)
   }
-  poissonn((&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_mt.diminfo[0].strides))), (&__pyx_v_counter), __pyx_v_xm, (&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_DTYPE_t *, __pyx_pybuffernd_series.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_series.diminfo[0].strides))), __pyx_v_n);
+  poissonn((&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_6, __pyx_pybuffernd_mt.diminfo[0].strides))), (&__pyx_v_counter), __pyx_v_xm, (&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_DTYPE_t *, __pyx_pybuffernd_series.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_series.diminfo[0].strides))), __pyx_v_n);
 
-  /* "pymt64.pyx":134
+  /* "pymt64.pyx":135
  * 
  *     poissonn( &mt[0] , &counter ,xm, &series[0], n)
  *     mt[MTSIZE] = counter             # <<<<<<<<<<<<<<
  * 
  *     return series
  */
-  __pyx_t_10 = __pyx_v_6pymt64_MTSIZE;
+  __pyx_t_8 = __pyx_v_6pymt64_MTSIZE;
   __pyx_t_7 = -1;
-  if (__pyx_t_10 < 0) {
-    __pyx_t_10 += __pyx_pybuffernd_mt.diminfo[0].shape;
-    if (unlikely(__pyx_t_10 < 0)) __pyx_t_7 = 0;
-  } else if (unlikely(__pyx_t_10 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_7 = 0;
+  if (__pyx_t_8 < 0) {
+    __pyx_t_8 += __pyx_pybuffernd_mt.diminfo[0].shape;
+    if (unlikely(__pyx_t_8 < 0)) __pyx_t_7 = 0;
+  } else if (unlikely(__pyx_t_8 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_7 = 0;
   if (unlikely(__pyx_t_7 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_7);
-    __PYX_ERR(0, 134, __pyx_L1_error)
+    __PYX_ERR(0, 135, __pyx_L1_error)
   }
-  *__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_mt.diminfo[0].strides) = __pyx_v_counter;
+  *__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_mt.diminfo[0].strides) = __pyx_v_counter;
 
-  /* "pymt64.pyx":136
+  /* "pymt64.pyx":137
  *     mt[MTSIZE] = counter
  * 
  *     return series             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_series));
   __pyx_r = ((PyObject *)__pyx_v_series);
   goto __pyx_L0;
 
-  /* "pymt64.pyx":121
+  /* "pymt64.pyx":122
  *     return series
  * 
  * def poisson(np.ndarray [U64TYPE_t,ndim=1, mode='c'] mt , double xm , int n):             # <<<<<<<<<<<<<<
  *     '''
  * 
  */
 
@@ -2486,29 +2661,32 @@
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_series);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pymt64.pyx":139
+/* "pymt64.pyx":140
  * 
  * 
  * def normal(np.ndarray [U64TYPE_t,ndim=1, mode='c'] mt ,  int n):             # <<<<<<<<<<<<<<
  * 
  *     '''
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6pymt64_7normal(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_6pymt64_6normal[] = "\n    Generates two random series of size n Normally distributed with zero mean and variance one.\n    \n    (x,y) = normal(mt,n)\n    \n    ";
-static PyMethodDef __pyx_mdef_6pymt64_7normal = {"normal", (PyCFunction)__pyx_pw_6pymt64_7normal, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6pymt64_6normal};
+static PyMethodDef __pyx_mdef_6pymt64_7normal = {"normal", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6pymt64_7normal, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6pymt64_6normal};
 static PyObject *__pyx_pw_6pymt64_7normal(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyArrayObject *__pyx_v_mt = 0;
   int __pyx_v_n;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("normal (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_mt,&__pyx_n_s_n,0};
     PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
@@ -2527,38 +2705,38 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mt)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_n)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("normal", 1, 2, 2, 1); __PYX_ERR(0, 139, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("normal", 1, 2, 2, 1); __PYX_ERR(0, 140, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "normal") < 0)) __PYX_ERR(0, 139, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "normal") < 0)) __PYX_ERR(0, 140, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_mt = ((PyArrayObject *)values[0]);
-    __pyx_v_n = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_n == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
+    __pyx_v_n = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_n == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 140, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("normal", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 139, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("normal", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 140, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pymt64.normal", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_mt), __pyx_ptype_5numpy_ndarray, 1, "mt", 0))) __PYX_ERR(0, 139, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_mt), __pyx_ptype_5numpy_ndarray, 1, "mt", 0))) __PYX_ERR(0, 140, __pyx_L1_error)
   __pyx_r = __pyx_pf_6pymt64_6normal(__pyx_self, __pyx_v_mt, __pyx_v_n);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -2584,16 +2762,17 @@
   PyObject *__pyx_t_4 = NULL;
   PyArrayObject *__pyx_t_5 = NULL;
   PyArrayObject *__pyx_t_6 = NULL;
   Py_ssize_t __pyx_t_7;
   int __pyx_t_8;
   Py_ssize_t __pyx_t_9;
   Py_ssize_t __pyx_t_10;
-  Py_ssize_t __pyx_t_11;
-  Py_ssize_t __pyx_t_12;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("normal", 0);
   __pyx_pybuffer_series1.pybuffer.buf = NULL;
   __pyx_pybuffer_series1.refcount = 0;
   __pyx_pybuffernd_series1.data = NULL;
   __pyx_pybuffernd_series1.rcbuffer = &__pyx_pybuffer_series1;
   __pyx_pybuffer_series2.pybuffer.buf = NULL;
   __pyx_pybuffer_series2.refcount = 0;
@@ -2601,204 +2780,204 @@
   __pyx_pybuffernd_series2.rcbuffer = &__pyx_pybuffer_series2;
   __pyx_pybuffer_mt.pybuffer.buf = NULL;
   __pyx_pybuffer_mt.refcount = 0;
   __pyx_pybuffernd_mt.data = NULL;
   __pyx_pybuffernd_mt.rcbuffer = &__pyx_pybuffer_mt;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_mt.rcbuffer->pybuffer, (PyObject*)__pyx_v_mt, &__Pyx_TypeInfo_nn___pyx_t_6pymt64_U64TYPE_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 139, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_mt.rcbuffer->pybuffer, (PyObject*)__pyx_v_mt, &__Pyx_TypeInfo_nn___pyx_t_6pymt64_U64TYPE_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 140, __pyx_L1_error)
   }
   __pyx_pybuffernd_mt.diminfo[0].strides = __pyx_pybuffernd_mt.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_mt.diminfo[0].shape = __pyx_pybuffernd_mt.rcbuffer->pybuffer.shape[0];
 
-  /* "pymt64.pyx":148
+  /* "pymt64.pyx":149
  *     '''
  * 
  *     cdef np.ndarray [DTYPE_t,ndim=1, mode='c'] series1 = np.zeros(n, dtype=DTYPE)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray [DTYPE_t,ndim=1, mode='c'] series2 = np.zeros(n, dtype=DTYPE)
  *     cdef int counter = mt[MTSIZE]
  */
-  __pyx_t_1 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_GetModuleGlobalName(__pyx_n_s_DTYPE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 148, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 148, __pyx_L1_error)
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 149, __pyx_L1_error)
   __pyx_t_5 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_series1.rcbuffer->pybuffer, (PyObject*)__pyx_t_5, &__Pyx_TypeInfo_nn___pyx_t_6pymt64_DTYPE_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_series1 = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_series1.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 148, __pyx_L1_error)
+      __PYX_ERR(0, 149, __pyx_L1_error)
     } else {__pyx_pybuffernd_series1.diminfo[0].strides = __pyx_pybuffernd_series1.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_series1.diminfo[0].shape = __pyx_pybuffernd_series1.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_5 = 0;
   __pyx_v_series1 = ((PyArrayObject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "pymt64.pyx":149
+  /* "pymt64.pyx":150
  * 
  *     cdef np.ndarray [DTYPE_t,ndim=1, mode='c'] series1 = np.zeros(n, dtype=DTYPE)
  *     cdef np.ndarray [DTYPE_t,ndim=1, mode='c'] series2 = np.zeros(n, dtype=DTYPE)             # <<<<<<<<<<<<<<
  *     cdef int counter = mt[MTSIZE]
  * 
  */
-  __pyx_t_4 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = __Pyx_GetModuleGlobalName(__pyx_n_s_DTYPE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 149, __pyx_L1_error)
+  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 150, __pyx_L1_error)
   __pyx_t_6 = ((PyArrayObject *)__pyx_t_2);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_series2.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_6pymt64_DTYPE_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_series2 = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_series2.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 149, __pyx_L1_error)
+      __PYX_ERR(0, 150, __pyx_L1_error)
     } else {__pyx_pybuffernd_series2.diminfo[0].strides = __pyx_pybuffernd_series2.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_series2.diminfo[0].shape = __pyx_pybuffernd_series2.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_6 = 0;
   __pyx_v_series2 = ((PyArrayObject *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "pymt64.pyx":150
+  /* "pymt64.pyx":151
  *     cdef np.ndarray [DTYPE_t,ndim=1, mode='c'] series1 = np.zeros(n, dtype=DTYPE)
  *     cdef np.ndarray [DTYPE_t,ndim=1, mode='c'] series2 = np.zeros(n, dtype=DTYPE)
  *     cdef int counter = mt[MTSIZE]             # <<<<<<<<<<<<<<
  * 
  *     normaln( &mt[0] , &counter , &series1[0], &series2[0], n)
  */
   __pyx_t_7 = __pyx_v_6pymt64_MTSIZE;
   __pyx_t_8 = -1;
   if (__pyx_t_7 < 0) {
     __pyx_t_7 += __pyx_pybuffernd_mt.diminfo[0].shape;
     if (unlikely(__pyx_t_7 < 0)) __pyx_t_8 = 0;
   } else if (unlikely(__pyx_t_7 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_8 = 0;
   if (unlikely(__pyx_t_8 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_8);
-    __PYX_ERR(0, 150, __pyx_L1_error)
+    __PYX_ERR(0, 151, __pyx_L1_error)
   }
   __pyx_v_counter = (*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_7, __pyx_pybuffernd_mt.diminfo[0].strides));
 
-  /* "pymt64.pyx":152
+  /* "pymt64.pyx":153
  *     cdef int counter = mt[MTSIZE]
  * 
  *     normaln( &mt[0] , &counter , &series1[0], &series2[0], n)             # <<<<<<<<<<<<<<
  *     mt[MTSIZE] = counter
  *     return series1,series2
  */
+  __pyx_t_7 = 0;
+  __pyx_t_8 = -1;
+  if (__pyx_t_7 < 0) {
+    __pyx_t_7 += __pyx_pybuffernd_mt.diminfo[0].shape;
+    if (unlikely(__pyx_t_7 < 0)) __pyx_t_8 = 0;
+  } else if (unlikely(__pyx_t_7 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_8 = 0;
+  if (unlikely(__pyx_t_8 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_8);
+    __PYX_ERR(0, 153, __pyx_L1_error)
+  }
   __pyx_t_9 = 0;
   __pyx_t_8 = -1;
   if (__pyx_t_9 < 0) {
-    __pyx_t_9 += __pyx_pybuffernd_mt.diminfo[0].shape;
+    __pyx_t_9 += __pyx_pybuffernd_series1.diminfo[0].shape;
     if (unlikely(__pyx_t_9 < 0)) __pyx_t_8 = 0;
-  } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_8 = 0;
+  } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_series1.diminfo[0].shape)) __pyx_t_8 = 0;
   if (unlikely(__pyx_t_8 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_8);
-    __PYX_ERR(0, 152, __pyx_L1_error)
+    __PYX_ERR(0, 153, __pyx_L1_error)
   }
   __pyx_t_10 = 0;
   __pyx_t_8 = -1;
   if (__pyx_t_10 < 0) {
-    __pyx_t_10 += __pyx_pybuffernd_series1.diminfo[0].shape;
+    __pyx_t_10 += __pyx_pybuffernd_series2.diminfo[0].shape;
     if (unlikely(__pyx_t_10 < 0)) __pyx_t_8 = 0;
-  } else if (unlikely(__pyx_t_10 >= __pyx_pybuffernd_series1.diminfo[0].shape)) __pyx_t_8 = 0;
-  if (unlikely(__pyx_t_8 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_8);
-    __PYX_ERR(0, 152, __pyx_L1_error)
-  }
-  __pyx_t_11 = 0;
-  __pyx_t_8 = -1;
-  if (__pyx_t_11 < 0) {
-    __pyx_t_11 += __pyx_pybuffernd_series2.diminfo[0].shape;
-    if (unlikely(__pyx_t_11 < 0)) __pyx_t_8 = 0;
-  } else if (unlikely(__pyx_t_11 >= __pyx_pybuffernd_series2.diminfo[0].shape)) __pyx_t_8 = 0;
+  } else if (unlikely(__pyx_t_10 >= __pyx_pybuffernd_series2.diminfo[0].shape)) __pyx_t_8 = 0;
   if (unlikely(__pyx_t_8 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_8);
-    __PYX_ERR(0, 152, __pyx_L1_error)
+    __PYX_ERR(0, 153, __pyx_L1_error)
   }
-  normaln((&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_mt.diminfo[0].strides))), (&__pyx_v_counter), (&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_DTYPE_t *, __pyx_pybuffernd_series1.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_series1.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_DTYPE_t *, __pyx_pybuffernd_series2.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_series2.diminfo[0].strides))), __pyx_v_n);
+  normaln((&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_7, __pyx_pybuffernd_mt.diminfo[0].strides))), (&__pyx_v_counter), (&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_DTYPE_t *, __pyx_pybuffernd_series1.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_series1.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_DTYPE_t *, __pyx_pybuffernd_series2.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_series2.diminfo[0].strides))), __pyx_v_n);
 
-  /* "pymt64.pyx":153
+  /* "pymt64.pyx":154
  * 
  *     normaln( &mt[0] , &counter , &series1[0], &series2[0], n)
  *     mt[MTSIZE] = counter             # <<<<<<<<<<<<<<
  *     return series1,series2
  * 
  */
-  __pyx_t_12 = __pyx_v_6pymt64_MTSIZE;
+  __pyx_t_10 = __pyx_v_6pymt64_MTSIZE;
   __pyx_t_8 = -1;
-  if (__pyx_t_12 < 0) {
-    __pyx_t_12 += __pyx_pybuffernd_mt.diminfo[0].shape;
-    if (unlikely(__pyx_t_12 < 0)) __pyx_t_8 = 0;
-  } else if (unlikely(__pyx_t_12 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_8 = 0;
+  if (__pyx_t_10 < 0) {
+    __pyx_t_10 += __pyx_pybuffernd_mt.diminfo[0].shape;
+    if (unlikely(__pyx_t_10 < 0)) __pyx_t_8 = 0;
+  } else if (unlikely(__pyx_t_10 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_8 = 0;
   if (unlikely(__pyx_t_8 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_8);
-    __PYX_ERR(0, 153, __pyx_L1_error)
+    __PYX_ERR(0, 154, __pyx_L1_error)
   }
-  *__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_mt.diminfo[0].strides) = __pyx_v_counter;
+  *__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_mt.diminfo[0].strides) = __pyx_v_counter;
 
-  /* "pymt64.pyx":154
+  /* "pymt64.pyx":155
  *     normaln( &mt[0] , &counter , &series1[0], &series2[0], n)
  *     mt[MTSIZE] = counter
  *     return series1,series2             # <<<<<<<<<<<<<<
  * 
  * def  poisson_multlam(np.ndarray [U64TYPE_t,ndim=1, mode='c'] mt , np.ndarray [DTYPE_t,ndim=1, mode='c'] xm):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(((PyObject *)__pyx_v_series1));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_series1));
   PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)__pyx_v_series1));
   __Pyx_INCREF(((PyObject *)__pyx_v_series2));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_series2));
   PyTuple_SET_ITEM(__pyx_t_2, 1, ((PyObject *)__pyx_v_series2));
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "pymt64.pyx":139
+  /* "pymt64.pyx":140
  * 
  * 
  * def normal(np.ndarray [U64TYPE_t,ndim=1, mode='c'] mt ,  int n):             # <<<<<<<<<<<<<<
  * 
  *     '''
  */
 
@@ -2827,29 +3006,32 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_series1);
   __Pyx_XDECREF((PyObject *)__pyx_v_series2);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pymt64.pyx":156
+/* "pymt64.pyx":157
  *     return series1,series2
  * 
  * def  poisson_multlam(np.ndarray [U64TYPE_t,ndim=1, mode='c'] mt , np.ndarray [DTYPE_t,ndim=1, mode='c'] xm):             # <<<<<<<<<<<<<<
  * 
  *     '''
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6pymt64_9poisson_multlam(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_6pymt64_8poisson_multlam[] = "\n    Generates a Poisson distribution. \n    While poisson() works with a single value of 'lambda', this functions considers multiple values of lambda. i.e one for each generated random number. lambda must have as many elements as the number of random values desired.\n    \n    x = poisson_multlamb(mt,lambda)    \n    ";
-static PyMethodDef __pyx_mdef_6pymt64_9poisson_multlam = {"poisson_multlam", (PyCFunction)__pyx_pw_6pymt64_9poisson_multlam, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6pymt64_8poisson_multlam};
+static PyMethodDef __pyx_mdef_6pymt64_9poisson_multlam = {"poisson_multlam", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6pymt64_9poisson_multlam, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6pymt64_8poisson_multlam};
 static PyObject *__pyx_pw_6pymt64_9poisson_multlam(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyArrayObject *__pyx_v_mt = 0;
   PyArrayObject *__pyx_v_xm = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("poisson_multlam (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_mt,&__pyx_n_s_xm,0};
     PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
@@ -2868,39 +3050,39 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mt)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_xm)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("poisson_multlam", 1, 2, 2, 1); __PYX_ERR(0, 156, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("poisson_multlam", 1, 2, 2, 1); __PYX_ERR(0, 157, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "poisson_multlam") < 0)) __PYX_ERR(0, 156, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "poisson_multlam") < 0)) __PYX_ERR(0, 157, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_mt = ((PyArrayObject *)values[0]);
     __pyx_v_xm = ((PyArrayObject *)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("poisson_multlam", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 156, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("poisson_multlam", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 157, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pymt64.poisson_multlam", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_mt), __pyx_ptype_5numpy_ndarray, 1, "mt", 0))) __PYX_ERR(0, 156, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_xm), __pyx_ptype_5numpy_ndarray, 1, "xm", 0))) __PYX_ERR(0, 156, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_mt), __pyx_ptype_5numpy_ndarray, 1, "mt", 0))) __PYX_ERR(0, 157, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_xm), __pyx_ptype_5numpy_ndarray, 1, "xm", 0))) __PYX_ERR(0, 157, __pyx_L1_error)
   __pyx_r = __pyx_pf_6pymt64_8poisson_multlam(__pyx_self, __pyx_v_mt, __pyx_v_xm);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -2924,17 +3106,18 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyArrayObject *__pyx_t_5 = NULL;
   Py_ssize_t __pyx_t_6;
   int __pyx_t_7;
   Py_ssize_t __pyx_t_8;
   Py_ssize_t __pyx_t_9;
-  Py_ssize_t __pyx_t_10;
-  long __pyx_t_11;
-  Py_ssize_t __pyx_t_12;
+  long __pyx_t_10;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("poisson_multlam", 0);
   __pyx_pybuffer_series.pybuffer.buf = NULL;
   __pyx_pybuffer_series.refcount = 0;
   __pyx_pybuffernd_series.data = NULL;
   __pyx_pybuffernd_series.rcbuffer = &__pyx_pybuffer_series;
   __pyx_pybuffer_mt.pybuffer.buf = NULL;
   __pyx_pybuffer_mt.refcount = 0;
@@ -2942,159 +3125,159 @@
   __pyx_pybuffernd_mt.rcbuffer = &__pyx_pybuffer_mt;
   __pyx_pybuffer_xm.pybuffer.buf = NULL;
   __pyx_pybuffer_xm.refcount = 0;
   __pyx_pybuffernd_xm.data = NULL;
   __pyx_pybuffernd_xm.rcbuffer = &__pyx_pybuffer_xm;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_mt.rcbuffer->pybuffer, (PyObject*)__pyx_v_mt, &__Pyx_TypeInfo_nn___pyx_t_6pymt64_U64TYPE_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 156, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_mt.rcbuffer->pybuffer, (PyObject*)__pyx_v_mt, &__Pyx_TypeInfo_nn___pyx_t_6pymt64_U64TYPE_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 157, __pyx_L1_error)
   }
   __pyx_pybuffernd_mt.diminfo[0].strides = __pyx_pybuffernd_mt.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_mt.diminfo[0].shape = __pyx_pybuffernd_mt.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_xm.rcbuffer->pybuffer, (PyObject*)__pyx_v_xm, &__Pyx_TypeInfo_nn___pyx_t_6pymt64_DTYPE_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 156, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_xm.rcbuffer->pybuffer, (PyObject*)__pyx_v_xm, &__Pyx_TypeInfo_nn___pyx_t_6pymt64_DTYPE_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 157, __pyx_L1_error)
   }
   __pyx_pybuffernd_xm.diminfo[0].strides = __pyx_pybuffernd_xm.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_xm.diminfo[0].shape = __pyx_pybuffernd_xm.rcbuffer->pybuffer.shape[0];
 
-  /* "pymt64.pyx":165
+  /* "pymt64.pyx":166
  *     '''
  * 
  *     cdef np.ndarray [DTYPE_t,ndim=1, mode='c'] series = np.zeros(xm.size, dtype=DTYPE)             # <<<<<<<<<<<<<<
  *     cdef int counter = mt[MTSIZE]
  * 
  */
-  __pyx_t_1 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_xm), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_xm), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_GetModuleGlobalName(__pyx_n_s_DTYPE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 165, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 165, __pyx_L1_error)
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 166, __pyx_L1_error)
   __pyx_t_5 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_series.rcbuffer->pybuffer, (PyObject*)__pyx_t_5, &__Pyx_TypeInfo_nn___pyx_t_6pymt64_DTYPE_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_series = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_series.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 165, __pyx_L1_error)
+      __PYX_ERR(0, 166, __pyx_L1_error)
     } else {__pyx_pybuffernd_series.diminfo[0].strides = __pyx_pybuffernd_series.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_series.diminfo[0].shape = __pyx_pybuffernd_series.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_5 = 0;
   __pyx_v_series = ((PyArrayObject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "pymt64.pyx":166
+  /* "pymt64.pyx":167
  * 
  *     cdef np.ndarray [DTYPE_t,ndim=1, mode='c'] series = np.zeros(xm.size, dtype=DTYPE)
  *     cdef int counter = mt[MTSIZE]             # <<<<<<<<<<<<<<
  * 
  *     poissonn_multlam( &mt[0] , &counter , &xm[0], &series[0], xm.size )
  */
   __pyx_t_6 = __pyx_v_6pymt64_MTSIZE;
   __pyx_t_7 = -1;
   if (__pyx_t_6 < 0) {
     __pyx_t_6 += __pyx_pybuffernd_mt.diminfo[0].shape;
     if (unlikely(__pyx_t_6 < 0)) __pyx_t_7 = 0;
   } else if (unlikely(__pyx_t_6 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_7 = 0;
   if (unlikely(__pyx_t_7 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_7);
-    __PYX_ERR(0, 166, __pyx_L1_error)
+    __PYX_ERR(0, 167, __pyx_L1_error)
   }
   __pyx_v_counter = (*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_6, __pyx_pybuffernd_mt.diminfo[0].strides));
 
-  /* "pymt64.pyx":168
+  /* "pymt64.pyx":169
  *     cdef int counter = mt[MTSIZE]
  * 
  *     poissonn_multlam( &mt[0] , &counter , &xm[0], &series[0], xm.size )             # <<<<<<<<<<<<<<
  *     mt[MTSIZE] = counter
  * 
  */
+  __pyx_t_6 = 0;
+  __pyx_t_7 = -1;
+  if (__pyx_t_6 < 0) {
+    __pyx_t_6 += __pyx_pybuffernd_mt.diminfo[0].shape;
+    if (unlikely(__pyx_t_6 < 0)) __pyx_t_7 = 0;
+  } else if (unlikely(__pyx_t_6 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_7 = 0;
+  if (unlikely(__pyx_t_7 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_7);
+    __PYX_ERR(0, 169, __pyx_L1_error)
+  }
   __pyx_t_8 = 0;
   __pyx_t_7 = -1;
   if (__pyx_t_8 < 0) {
-    __pyx_t_8 += __pyx_pybuffernd_mt.diminfo[0].shape;
+    __pyx_t_8 += __pyx_pybuffernd_xm.diminfo[0].shape;
     if (unlikely(__pyx_t_8 < 0)) __pyx_t_7 = 0;
-  } else if (unlikely(__pyx_t_8 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_7 = 0;
+  } else if (unlikely(__pyx_t_8 >= __pyx_pybuffernd_xm.diminfo[0].shape)) __pyx_t_7 = 0;
   if (unlikely(__pyx_t_7 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_7);
-    __PYX_ERR(0, 168, __pyx_L1_error)
+    __PYX_ERR(0, 169, __pyx_L1_error)
   }
   __pyx_t_9 = 0;
   __pyx_t_7 = -1;
   if (__pyx_t_9 < 0) {
-    __pyx_t_9 += __pyx_pybuffernd_xm.diminfo[0].shape;
+    __pyx_t_9 += __pyx_pybuffernd_series.diminfo[0].shape;
     if (unlikely(__pyx_t_9 < 0)) __pyx_t_7 = 0;
-  } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_xm.diminfo[0].shape)) __pyx_t_7 = 0;
-  if (unlikely(__pyx_t_7 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_7);
-    __PYX_ERR(0, 168, __pyx_L1_error)
-  }
-  __pyx_t_10 = 0;
-  __pyx_t_7 = -1;
-  if (__pyx_t_10 < 0) {
-    __pyx_t_10 += __pyx_pybuffernd_series.diminfo[0].shape;
-    if (unlikely(__pyx_t_10 < 0)) __pyx_t_7 = 0;
-  } else if (unlikely(__pyx_t_10 >= __pyx_pybuffernd_series.diminfo[0].shape)) __pyx_t_7 = 0;
+  } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_series.diminfo[0].shape)) __pyx_t_7 = 0;
   if (unlikely(__pyx_t_7 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_7);
-    __PYX_ERR(0, 168, __pyx_L1_error)
+    __PYX_ERR(0, 169, __pyx_L1_error)
   }
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_xm), __pyx_n_s_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_xm), __pyx_n_s_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 169, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_t_4); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 168, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_As_long(__pyx_t_4); if (unlikely((__pyx_t_10 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 169, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  poissonn_multlam((&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_mt.diminfo[0].strides))), (&__pyx_v_counter), (&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_DTYPE_t *, __pyx_pybuffernd_xm.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_xm.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_DTYPE_t *, __pyx_pybuffernd_series.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_series.diminfo[0].strides))), __pyx_t_11);
+  poissonn_multlam((&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_6, __pyx_pybuffernd_mt.diminfo[0].strides))), (&__pyx_v_counter), (&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_DTYPE_t *, __pyx_pybuffernd_xm.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_xm.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_DTYPE_t *, __pyx_pybuffernd_series.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_series.diminfo[0].strides))), __pyx_t_10);
 
-  /* "pymt64.pyx":169
+  /* "pymt64.pyx":170
  * 
  *     poissonn_multlam( &mt[0] , &counter , &xm[0], &series[0], xm.size )
  *     mt[MTSIZE] = counter             # <<<<<<<<<<<<<<
  * 
  *     return series
  */
-  __pyx_t_12 = __pyx_v_6pymt64_MTSIZE;
+  __pyx_t_9 = __pyx_v_6pymt64_MTSIZE;
   __pyx_t_7 = -1;
-  if (__pyx_t_12 < 0) {
-    __pyx_t_12 += __pyx_pybuffernd_mt.diminfo[0].shape;
-    if (unlikely(__pyx_t_12 < 0)) __pyx_t_7 = 0;
-  } else if (unlikely(__pyx_t_12 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_7 = 0;
+  if (__pyx_t_9 < 0) {
+    __pyx_t_9 += __pyx_pybuffernd_mt.diminfo[0].shape;
+    if (unlikely(__pyx_t_9 < 0)) __pyx_t_7 = 0;
+  } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_mt.diminfo[0].shape)) __pyx_t_7 = 0;
   if (unlikely(__pyx_t_7 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_7);
-    __PYX_ERR(0, 169, __pyx_L1_error)
+    __PYX_ERR(0, 170, __pyx_L1_error)
   }
-  *__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_mt.diminfo[0].strides) = __pyx_v_counter;
+  *__Pyx_BufPtrCContig1d(__pyx_t_6pymt64_U64TYPE_t *, __pyx_pybuffernd_mt.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_mt.diminfo[0].strides) = __pyx_v_counter;
 
-  /* "pymt64.pyx":171
+  /* "pymt64.pyx":172
  *     mt[MTSIZE] = counter
  * 
  *     return series             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_series));
   __pyx_r = ((PyObject *)__pyx_v_series);
   goto __pyx_L0;
 
-  /* "pymt64.pyx":156
+  /* "pymt64.pyx":157
  *     return series1,series2
  * 
  * def  poisson_multlam(np.ndarray [U64TYPE_t,ndim=1, mode='c'] mt , np.ndarray [DTYPE_t,ndim=1, mode='c'] xm):             # <<<<<<<<<<<<<<
  * 
  *     '''
  */
 
@@ -3122,897 +3305,46 @@
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_series);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":215
- *         # experimental exception made for __getbuffer__ and __releasebuffer__
- *         # -- the details of this may change.
- *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
- *             # This implementation of getbuffer is geared towards Cython
- *             # requirements, and does not yet fulfill the PEP.
- */
-
-/* Python wrapper */
-static CYTHON_UNUSED int __pyx_pw_5numpy_7ndarray_1__getbuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /*proto*/
-static CYTHON_UNUSED int __pyx_pw_5numpy_7ndarray_1__getbuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__getbuffer__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_5numpy_7ndarray___getbuffer__(((PyArrayObject *)__pyx_v_self), ((Py_buffer *)__pyx_v_info), ((int)__pyx_v_flags));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_5numpy_7ndarray___getbuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags) {
-  int __pyx_v_i;
-  int __pyx_v_ndim;
-  int __pyx_v_endian_detector;
-  int __pyx_v_little_endian;
-  int __pyx_v_t;
-  char *__pyx_v_f;
-  PyArray_Descr *__pyx_v_descr = 0;
-  int __pyx_v_offset;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  int __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  int __pyx_t_5;
-  int __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
-  char *__pyx_t_8;
-  if (__pyx_v_info == NULL) {
-    PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
-    return -1;
-  }
-  __Pyx_RefNannySetupContext("__getbuffer__", 0);
-  __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
-  __Pyx_GIVEREF(__pyx_v_info->obj);
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":222
- * 
- *             cdef int i, ndim
- *             cdef int endian_detector = 1             # <<<<<<<<<<<<<<
- *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
- * 
- */
-  __pyx_v_endian_detector = 1;
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":223
- *             cdef int i, ndim
- *             cdef int endian_detector = 1
- *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
- * 
- *             ndim = PyArray_NDIM(self)
- */
-  __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":225
- *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
- * 
- *             ndim = PyArray_NDIM(self)             # <<<<<<<<<<<<<<
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- */
-  __pyx_v_ndim = PyArray_NDIM(__pyx_v_self);
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":227
- *             ndim = PyArray_NDIM(self)
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")
- */
-  __pyx_t_2 = (((__pyx_v_flags & PyBUF_C_CONTIGUOUS) == PyBUF_C_CONTIGUOUS) != 0);
-  if (__pyx_t_2) {
-  } else {
-    __pyx_t_1 = __pyx_t_2;
-    goto __pyx_L4_bool_binop_done;
-  }
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":228
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_C_CONTIGUOUS)):             # <<<<<<<<<<<<<<
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- */
-  __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_C_CONTIGUOUS) != 0)) != 0);
-  __pyx_t_1 = __pyx_t_2;
-  __pyx_L4_bool_binop_done:;
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":227
- *             ndim = PyArray_NDIM(self)
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")
- */
-  if (unlikely(__pyx_t_1)) {
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":229
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 229, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 229, __pyx_L1_error)
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":227
- *             ndim = PyArray_NDIM(self)
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")
- */
-  }
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":231
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- */
-  __pyx_t_2 = (((__pyx_v_flags & PyBUF_F_CONTIGUOUS) == PyBUF_F_CONTIGUOUS) != 0);
-  if (__pyx_t_2) {
-  } else {
-    __pyx_t_1 = __pyx_t_2;
-    goto __pyx_L7_bool_binop_done;
-  }
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":232
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_F_CONTIGUOUS)):             # <<<<<<<<<<<<<<
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- * 
- */
-  __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_F_CONTIGUOUS) != 0)) != 0);
-  __pyx_t_1 = __pyx_t_2;
-  __pyx_L7_bool_binop_done:;
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":231
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- */
-  if (unlikely(__pyx_t_1)) {
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":233
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
- * 
- *             info.buf = PyArray_DATA(self)
- */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 233, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 233, __pyx_L1_error)
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":231
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- */
-  }
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":235
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- * 
- *             info.buf = PyArray_DATA(self)             # <<<<<<<<<<<<<<
- *             info.ndim = ndim
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- */
-  __pyx_v_info->buf = PyArray_DATA(__pyx_v_self);
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":236
- * 
- *             info.buf = PyArray_DATA(self)
- *             info.ndim = ndim             # <<<<<<<<<<<<<<
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 # Allocate new buffer for strides and shape info.
- */
-  __pyx_v_info->ndim = __pyx_v_ndim;
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":237
- *             info.buf = PyArray_DATA(self)
- *             info.ndim = ndim
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 # Allocate new buffer for strides and shape info.
- *                 # This is allocated as one block, strides first.
- */
-  __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":240
- *                 # Allocate new buffer for strides and shape info.
- *                 # This is allocated as one block, strides first.
- *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)             # <<<<<<<<<<<<<<
- *                 info.shape = info.strides + ndim
- *                 for i in range(ndim):
- */
-    __pyx_v_info->strides = ((Py_ssize_t *)PyObject_Malloc((((sizeof(Py_ssize_t)) * 2) * ((size_t)__pyx_v_ndim))));
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":241
- *                 # This is allocated as one block, strides first.
- *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
- *                 info.shape = info.strides + ndim             # <<<<<<<<<<<<<<
- *                 for i in range(ndim):
- *                     info.strides[i] = PyArray_STRIDES(self)[i]
- */
-    __pyx_v_info->shape = (__pyx_v_info->strides + __pyx_v_ndim);
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":242
- *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
- *                 info.shape = info.strides + ndim
- *                 for i in range(ndim):             # <<<<<<<<<<<<<<
- *                     info.strides[i] = PyArray_STRIDES(self)[i]
- *                     info.shape[i] = PyArray_DIMS(self)[i]
- */
-    __pyx_t_4 = __pyx_v_ndim;
-    __pyx_t_5 = __pyx_t_4;
-    for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
-      __pyx_v_i = __pyx_t_6;
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":243
- *                 info.shape = info.strides + ndim
- *                 for i in range(ndim):
- *                     info.strides[i] = PyArray_STRIDES(self)[i]             # <<<<<<<<<<<<<<
- *                     info.shape[i] = PyArray_DIMS(self)[i]
- *             else:
- */
-      (__pyx_v_info->strides[__pyx_v_i]) = (PyArray_STRIDES(__pyx_v_self)[__pyx_v_i]);
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":244
- *                 for i in range(ndim):
- *                     info.strides[i] = PyArray_STRIDES(self)[i]
- *                     info.shape[i] = PyArray_DIMS(self)[i]             # <<<<<<<<<<<<<<
- *             else:
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
- */
-      (__pyx_v_info->shape[__pyx_v_i]) = (PyArray_DIMS(__pyx_v_self)[__pyx_v_i]);
-    }
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":237
- *             info.buf = PyArray_DATA(self)
- *             info.ndim = ndim
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 # Allocate new buffer for strides and shape info.
- *                 # This is allocated as one block, strides first.
- */
-    goto __pyx_L9;
-  }
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":246
- *                     info.shape[i] = PyArray_DIMS(self)[i]
- *             else:
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
- *             info.suboffsets = NULL
- */
-  /*else*/ {
-    __pyx_v_info->strides = ((Py_ssize_t *)PyArray_STRIDES(__pyx_v_self));
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":247
- *             else:
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)             # <<<<<<<<<<<<<<
- *             info.suboffsets = NULL
- *             info.itemsize = PyArray_ITEMSIZE(self)
- */
-    __pyx_v_info->shape = ((Py_ssize_t *)PyArray_DIMS(__pyx_v_self));
-  }
-  __pyx_L9:;
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":248
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
- *             info.suboffsets = NULL             # <<<<<<<<<<<<<<
- *             info.itemsize = PyArray_ITEMSIZE(self)
- *             info.readonly = not PyArray_ISWRITEABLE(self)
- */
-  __pyx_v_info->suboffsets = NULL;
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":249
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
- *             info.suboffsets = NULL
- *             info.itemsize = PyArray_ITEMSIZE(self)             # <<<<<<<<<<<<<<
- *             info.readonly = not PyArray_ISWRITEABLE(self)
- * 
- */
-  __pyx_v_info->itemsize = PyArray_ITEMSIZE(__pyx_v_self);
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":250
- *             info.suboffsets = NULL
- *             info.itemsize = PyArray_ITEMSIZE(self)
- *             info.readonly = not PyArray_ISWRITEABLE(self)             # <<<<<<<<<<<<<<
- * 
- *             cdef int t
- */
-  __pyx_v_info->readonly = (!(PyArray_ISWRITEABLE(__pyx_v_self) != 0));
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":253
- * 
- *             cdef int t
- *             cdef char* f = NULL             # <<<<<<<<<<<<<<
- *             cdef dtype descr = self.descr
- *             cdef int offset
- */
-  __pyx_v_f = NULL;
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":254
- *             cdef int t
- *             cdef char* f = NULL
- *             cdef dtype descr = self.descr             # <<<<<<<<<<<<<<
- *             cdef int offset
- * 
- */
-  __pyx_t_3 = ((PyObject *)__pyx_v_self->descr);
-  __Pyx_INCREF(__pyx_t_3);
-  __pyx_v_descr = ((PyArray_Descr *)__pyx_t_3);
-  __pyx_t_3 = 0;
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":257
- *             cdef int offset
- * 
- *             info.obj = self             # <<<<<<<<<<<<<<
- * 
- *             if not PyDataType_HASFIELDS(descr):
- */
-  __Pyx_INCREF(((PyObject *)__pyx_v_self));
-  __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
-  __Pyx_GOTREF(__pyx_v_info->obj);
-  __Pyx_DECREF(__pyx_v_info->obj);
-  __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":259
- *             info.obj = self
- * 
- *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or
- */
-  __pyx_t_1 = ((!(PyDataType_HASFIELDS(__pyx_v_descr) != 0)) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":260
- * 
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num             # <<<<<<<<<<<<<<
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):
- */
-    __pyx_t_4 = __pyx_v_descr->type_num;
-    __pyx_v_t = __pyx_t_4;
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":261
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- */
-    __pyx_t_2 = ((__pyx_v_descr->byteorder == '>') != 0);
-    if (!__pyx_t_2) {
-      goto __pyx_L15_next_or;
-    } else {
-    }
-    __pyx_t_2 = (__pyx_v_little_endian != 0);
-    if (!__pyx_t_2) {
-    } else {
-      __pyx_t_1 = __pyx_t_2;
-      goto __pyx_L14_bool_binop_done;
-    }
-    __pyx_L15_next_or:;
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":262
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
- *                     raise ValueError(u"Non-native byte order not supported")
- *                 if   t == NPY_BYTE:        f = "b"
- */
-    __pyx_t_2 = ((__pyx_v_descr->byteorder == '<') != 0);
-    if (__pyx_t_2) {
-    } else {
-      __pyx_t_1 = __pyx_t_2;
-      goto __pyx_L14_bool_binop_done;
-    }
-    __pyx_t_2 = ((!(__pyx_v_little_endian != 0)) != 0);
-    __pyx_t_1 = __pyx_t_2;
-    __pyx_L14_bool_binop_done:;
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":261
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- */
-    if (unlikely(__pyx_t_1)) {
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":263
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"
- */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 263, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 263, __pyx_L1_error)
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":261
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- */
-    }
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":264
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- *                 if   t == NPY_BYTE:        f = "b"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_UBYTE:       f = "B"
- *                 elif t == NPY_SHORT:       f = "h"
- */
-    switch (__pyx_v_t) {
-      case NPY_BYTE:
-      __pyx_v_f = ((char *)"b");
-      break;
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":265
- *                     raise ValueError(u"Non-native byte order not supported")
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_SHORT:       f = "h"
- *                 elif t == NPY_USHORT:      f = "H"
- */
-      case NPY_UBYTE:
-      __pyx_v_f = ((char *)"B");
-      break;
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":266
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"
- *                 elif t == NPY_SHORT:       f = "h"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_USHORT:      f = "H"
- *                 elif t == NPY_INT:         f = "i"
- */
-      case NPY_SHORT:
-      __pyx_v_f = ((char *)"h");
-      break;
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":267
- *                 elif t == NPY_UBYTE:       f = "B"
- *                 elif t == NPY_SHORT:       f = "h"
- *                 elif t == NPY_USHORT:      f = "H"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_INT:         f = "i"
- *                 elif t == NPY_UINT:        f = "I"
- */
-      case NPY_USHORT:
-      __pyx_v_f = ((char *)"H");
-      break;
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":268
- *                 elif t == NPY_SHORT:       f = "h"
- *                 elif t == NPY_USHORT:      f = "H"
- *                 elif t == NPY_INT:         f = "i"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_UINT:        f = "I"
- *                 elif t == NPY_LONG:        f = "l"
- */
-      case NPY_INT:
-      __pyx_v_f = ((char *)"i");
-      break;
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":269
- *                 elif t == NPY_USHORT:      f = "H"
- *                 elif t == NPY_INT:         f = "i"
- *                 elif t == NPY_UINT:        f = "I"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_LONG:        f = "l"
- *                 elif t == NPY_ULONG:       f = "L"
- */
-      case NPY_UINT:
-      __pyx_v_f = ((char *)"I");
-      break;
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":270
- *                 elif t == NPY_INT:         f = "i"
- *                 elif t == NPY_UINT:        f = "I"
- *                 elif t == NPY_LONG:        f = "l"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_ULONG:       f = "L"
- *                 elif t == NPY_LONGLONG:    f = "q"
- */
-      case NPY_LONG:
-      __pyx_v_f = ((char *)"l");
-      break;
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":271
- *                 elif t == NPY_UINT:        f = "I"
- *                 elif t == NPY_LONG:        f = "l"
- *                 elif t == NPY_ULONG:       f = "L"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_LONGLONG:    f = "q"
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- */
-      case NPY_ULONG:
-      __pyx_v_f = ((char *)"L");
-      break;
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":272
- *                 elif t == NPY_LONG:        f = "l"
- *                 elif t == NPY_ULONG:       f = "L"
- *                 elif t == NPY_LONGLONG:    f = "q"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- *                 elif t == NPY_FLOAT:       f = "f"
- */
-      case NPY_LONGLONG:
-      __pyx_v_f = ((char *)"q");
-      break;
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":273
- *                 elif t == NPY_ULONG:       f = "L"
- *                 elif t == NPY_LONGLONG:    f = "q"
- *                 elif t == NPY_ULONGLONG:   f = "Q"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_FLOAT:       f = "f"
- *                 elif t == NPY_DOUBLE:      f = "d"
- */
-      case NPY_ULONGLONG:
-      __pyx_v_f = ((char *)"Q");
-      break;
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":274
- *                 elif t == NPY_LONGLONG:    f = "q"
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- *                 elif t == NPY_FLOAT:       f = "f"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_DOUBLE:      f = "d"
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- */
-      case NPY_FLOAT:
-      __pyx_v_f = ((char *)"f");
-      break;
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":275
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- *                 elif t == NPY_FLOAT:       f = "f"
- *                 elif t == NPY_DOUBLE:      f = "d"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- */
-      case NPY_DOUBLE:
-      __pyx_v_f = ((char *)"d");
-      break;
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":276
- *                 elif t == NPY_FLOAT:       f = "f"
- *                 elif t == NPY_DOUBLE:      f = "d"
- *                 elif t == NPY_LONGDOUBLE:  f = "g"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- */
-      case NPY_LONGDOUBLE:
-      __pyx_v_f = ((char *)"g");
-      break;
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":277
- *                 elif t == NPY_DOUBLE:      f = "d"
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- *                 elif t == NPY_CFLOAT:      f = "Zf"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
- */
-      case NPY_CFLOAT:
-      __pyx_v_f = ((char *)"Zf");
-      break;
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":278
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- *                 elif t == NPY_CDOUBLE:     f = "Zd"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
- *                 elif t == NPY_OBJECT:      f = "O"
- */
-      case NPY_CDOUBLE:
-      __pyx_v_f = ((char *)"Zd");
-      break;
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":279
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_OBJECT:      f = "O"
- *                 else:
- */
-      case NPY_CLONGDOUBLE:
-      __pyx_v_f = ((char *)"Zg");
-      break;
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":280
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
- *                 elif t == NPY_OBJECT:      f = "O"             # <<<<<<<<<<<<<<
- *                 else:
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- */
-      case NPY_OBJECT:
-      __pyx_v_f = ((char *)"O");
-      break;
-      default:
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":282
- *                 elif t == NPY_OBJECT:      f = "O"
- *                 else:
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
- *                 info.format = f
- *                 return
- */
-      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 282, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_7 = PyUnicode_Format(__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 282, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 282, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 282, __pyx_L1_error)
-      break;
-    }
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":283
- *                 else:
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- *                 info.format = f             # <<<<<<<<<<<<<<
- *                 return
- *             else:
- */
-    __pyx_v_info->format = __pyx_v_f;
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":284
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- *                 info.format = f
- *                 return             # <<<<<<<<<<<<<<
- *             else:
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
- */
-    __pyx_r = 0;
-    goto __pyx_L0;
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":259
- *             info.obj = self
- * 
- *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or
- */
-  }
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":286
- *                 return
- *             else:
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)             # <<<<<<<<<<<<<<
- *                 info.format[0] = c'^' # Native data types, manual alignment
- *                 offset = 0
- */
-  /*else*/ {
-    __pyx_v_info->format = ((char *)PyObject_Malloc(0xFF));
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":287
- *             else:
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
- *                 info.format[0] = c'^' # Native data types, manual alignment             # <<<<<<<<<<<<<<
- *                 offset = 0
- *                 f = _util_dtypestring(descr, info.format + 1,
- */
-    (__pyx_v_info->format[0]) = '^';
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":288
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
- *                 info.format[0] = c'^' # Native data types, manual alignment
- *                 offset = 0             # <<<<<<<<<<<<<<
- *                 f = _util_dtypestring(descr, info.format + 1,
- *                                       info.format + _buffer_format_string_len,
- */
-    __pyx_v_offset = 0;
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":289
- *                 info.format[0] = c'^' # Native data types, manual alignment
- *                 offset = 0
- *                 f = _util_dtypestring(descr, info.format + 1,             # <<<<<<<<<<<<<<
- *                                       info.format + _buffer_format_string_len,
- *                                       &offset)
- */
-    __pyx_t_8 = __pyx_f_5numpy__util_dtypestring(__pyx_v_descr, (__pyx_v_info->format + 1), (__pyx_v_info->format + 0xFF), (&__pyx_v_offset)); if (unlikely(__pyx_t_8 == ((char *)NULL))) __PYX_ERR(1, 289, __pyx_L1_error)
-    __pyx_v_f = __pyx_t_8;
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":292
- *                                       info.format + _buffer_format_string_len,
- *                                       &offset)
- *                 f[0] = c'\0' # Terminate format string             # <<<<<<<<<<<<<<
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- */
-    (__pyx_v_f[0]) = '\x00';
-  }
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":215
- *         # experimental exception made for __getbuffer__ and __releasebuffer__
- *         # -- the details of this may change.
- *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
- *             # This implementation of getbuffer is geared towards Cython
- *             # requirements, and does not yet fulfill the PEP.
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("numpy.ndarray.__getbuffer__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  if (__pyx_v_info->obj != NULL) {
-    __Pyx_GOTREF(__pyx_v_info->obj);
-    __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
-  }
-  goto __pyx_L2;
-  __pyx_L0:;
-  if (__pyx_v_info->obj == Py_None) {
-    __Pyx_GOTREF(__pyx_v_info->obj);
-    __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
-  }
-  __pyx_L2:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_descr);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":294
- *                 f[0] = c'\0' # Terminate format string
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- */
-
-/* Python wrapper */
-static CYTHON_UNUSED void __pyx_pw_5numpy_7ndarray_3__releasebuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info); /*proto*/
-static CYTHON_UNUSED void __pyx_pw_5numpy_7ndarray_3__releasebuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__releasebuffer__ (wrapper)", 0);
-  __pyx_pf_5numpy_7ndarray_2__releasebuffer__(((PyArrayObject *)__pyx_v_self), ((Py_buffer *)__pyx_v_info));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-}
-
-static void __pyx_pf_5numpy_7ndarray_2__releasebuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  __Pyx_RefNannySetupContext("__releasebuffer__", 0);
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":295
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- */
-  __pyx_t_1 = (PyArray_HASFIELDS(__pyx_v_self) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":296
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)             # <<<<<<<<<<<<<<
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 PyObject_Free(info.strides)
- */
-    PyObject_Free(__pyx_v_info->format);
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":295
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- */
-  }
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":297
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.strides)
- *                 # info.shape was stored after info.strides in the same block
- */
-  __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":298
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 PyObject_Free(info.strides)             # <<<<<<<<<<<<<<
- *                 # info.shape was stored after info.strides in the same block
- * 
- */
-    PyObject_Free(__pyx_v_info->strides);
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":297
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.strides)
- *                 # info.shape was stored after info.strides in the same block
- */
-  }
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":294
- *                 f[0] = c'\0' # Terminate format string
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- */
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-}
-
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":775
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":776
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 776, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":775
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4023,43 +3355,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":778
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew2(PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":779
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 779, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":778
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4070,43 +3405,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":781
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew3(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":782
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 782, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":781
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4117,43 +3455,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":784
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew4(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":785
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 785, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":784
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4164,43 +3505,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":787
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew5(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d, PyObject *__pyx_v_e) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":788
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 788, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":787
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4211,1115 +3555,326 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":790
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":791
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":792
+    /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":791
+    /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":794
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:
+ * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":790
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":796
- *         return ()
- * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
- *     # Recursive utility function used in __getbuffer__ to get format
- *     # string. The new location in the format string is returned.
- */
-
-static CYTHON_INLINE char *__pyx_f_5numpy__util_dtypestring(PyArray_Descr *__pyx_v_descr, char *__pyx_v_f, char *__pyx_v_end, int *__pyx_v_offset) {
-  PyArray_Descr *__pyx_v_child = 0;
-  int __pyx_v_endian_detector;
-  int __pyx_v_little_endian;
-  PyObject *__pyx_v_fields = 0;
-  PyObject *__pyx_v_childname = NULL;
-  PyObject *__pyx_v_new_offset = NULL;
-  PyObject *__pyx_v_t = NULL;
-  char *__pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
-  int __pyx_t_6;
-  int __pyx_t_7;
-  long __pyx_t_8;
-  char *__pyx_t_9;
-  __Pyx_RefNannySetupContext("_util_dtypestring", 0);
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":801
- * 
- *     cdef dtype child
- *     cdef int endian_detector = 1             # <<<<<<<<<<<<<<
- *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
- *     cdef tuple fields
- */
-  __pyx_v_endian_detector = 1;
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":802
- *     cdef dtype child
- *     cdef int endian_detector = 1
- *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
- *     cdef tuple fields
- * 
- */
-  __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":805
- *     cdef tuple fields
- * 
- *     for childname in descr.names:             # <<<<<<<<<<<<<<
- *         fields = descr.fields[childname]
- *         child, new_offset = fields
- */
-  if (unlikely(__pyx_v_descr->names == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(1, 805, __pyx_L1_error)
-  }
-  __pyx_t_1 = __pyx_v_descr->names; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
-  for (;;) {
-    if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
-    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_3); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 805, __pyx_L1_error)
-    #else
-    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 805, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    #endif
-    __Pyx_XDECREF_SET(__pyx_v_childname, __pyx_t_3);
-    __pyx_t_3 = 0;
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":806
- * 
- *     for childname in descr.names:
- *         fields = descr.fields[childname]             # <<<<<<<<<<<<<<
- *         child, new_offset = fields
- * 
- */
-    if (unlikely(__pyx_v_descr->fields == Py_None)) {
-      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 806, __pyx_L1_error)
-    }
-    __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_descr->fields, __pyx_v_childname); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 806, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    if (!(likely(PyTuple_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(1, 806, __pyx_L1_error)
-    __Pyx_XDECREF_SET(__pyx_v_fields, ((PyObject*)__pyx_t_3));
-    __pyx_t_3 = 0;
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":807
- *     for childname in descr.names:
- *         fields = descr.fields[childname]
- *         child, new_offset = fields             # <<<<<<<<<<<<<<
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:
- */
-    if (likely(__pyx_v_fields != Py_None)) {
-      PyObject* sequence = __pyx_v_fields;
-      Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
-      if (unlikely(size != 2)) {
-        if (size > 2) __Pyx_RaiseTooManyValuesError(2);
-        else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(1, 807, __pyx_L1_error)
-      }
-      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
-      __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_4);
-      #else
-      __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 807, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 807, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      #endif
-    } else {
-      __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 807, __pyx_L1_error)
-    }
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_dtype))))) __PYX_ERR(1, 807, __pyx_L1_error)
-    __Pyx_XDECREF_SET(__pyx_v_child, ((PyArray_Descr *)__pyx_t_3));
-    __pyx_t_3 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_new_offset, __pyx_t_4);
-    __pyx_t_4 = 0;
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":809
- *         child, new_offset = fields
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- */
-    __pyx_t_4 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 809, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = PyNumber_Subtract(__pyx_v_new_offset, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 809, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 809, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_6 = ((((__pyx_v_end - __pyx_v_f) - ((int)__pyx_t_5)) < 15) != 0);
-    if (unlikely(__pyx_t_6)) {
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":810
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
- * 
- *         if ((child.byteorder == c'>' and little_endian) or
- */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 810, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 810, __pyx_L1_error)
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":809
- *         child, new_offset = fields
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- */
-    }
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":812
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")
- */
-    __pyx_t_7 = ((__pyx_v_child->byteorder == '>') != 0);
-    if (!__pyx_t_7) {
-      goto __pyx_L8_next_or;
-    } else {
-    }
-    __pyx_t_7 = (__pyx_v_little_endian != 0);
-    if (!__pyx_t_7) {
-    } else {
-      __pyx_t_6 = __pyx_t_7;
-      goto __pyx_L7_bool_binop_done;
-    }
-    __pyx_L8_next_or:;
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":813
- * 
- *         if ((child.byteorder == c'>' and little_endian) or
- *             (child.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
- *             raise ValueError(u"Non-native byte order not supported")
- *             # One could encode it in the format string and have Cython
- */
-    __pyx_t_7 = ((__pyx_v_child->byteorder == '<') != 0);
-    if (__pyx_t_7) {
-    } else {
-      __pyx_t_6 = __pyx_t_7;
-      goto __pyx_L7_bool_binop_done;
-    }
-    __pyx_t_7 = ((!(__pyx_v_little_endian != 0)) != 0);
-    __pyx_t_6 = __pyx_t_7;
-    __pyx_L7_bool_binop_done:;
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":812
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")
- */
-    if (unlikely(__pyx_t_6)) {
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":814
- *         if ((child.byteorder == c'>' and little_endian) or
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *             # One could encode it in the format string and have Cython
- *             # complain instead, BUT: < and > in format strings also imply
- */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 814, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 814, __pyx_L1_error)
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":812
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")
- */
-    }
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":824
- * 
- *         # Output padding bytes
- *         while offset[0] < new_offset:             # <<<<<<<<<<<<<<
- *             f[0] = 120 # "x"; pad byte
- *             f += 1
- */
-    while (1) {
-      __pyx_t_3 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 824, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_v_new_offset, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 824, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 824, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (!__pyx_t_6) break;
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":825
- *         # Output padding bytes
- *         while offset[0] < new_offset:
- *             f[0] = 120 # "x"; pad byte             # <<<<<<<<<<<<<<
- *             f += 1
- *             offset[0] += 1
- */
-      (__pyx_v_f[0]) = 0x78;
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":826
- *         while offset[0] < new_offset:
- *             f[0] = 120 # "x"; pad byte
- *             f += 1             # <<<<<<<<<<<<<<
- *             offset[0] += 1
- * 
- */
-      __pyx_v_f = (__pyx_v_f + 1);
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":827
- *             f[0] = 120 # "x"; pad byte
- *             f += 1
- *             offset[0] += 1             # <<<<<<<<<<<<<<
- * 
- *         offset[0] += child.itemsize
- */
-      __pyx_t_8 = 0;
-      (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + 1);
-    }
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":829
- *             offset[0] += 1
- * 
- *         offset[0] += child.itemsize             # <<<<<<<<<<<<<<
- * 
- *         if not PyDataType_HASFIELDS(child):
- */
-    __pyx_t_8 = 0;
-    (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + __pyx_v_child->elsize);
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":831
- *         offset[0] += child.itemsize
- * 
- *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
- *             t = child.type_num
- *             if end - f < 5:
- */
-    __pyx_t_6 = ((!(PyDataType_HASFIELDS(__pyx_v_child) != 0)) != 0);
-    if (__pyx_t_6) {
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":832
- * 
- *         if not PyDataType_HASFIELDS(child):
- *             t = child.type_num             # <<<<<<<<<<<<<<
- *             if end - f < 5:
- *                 raise RuntimeError(u"Format string allocated too short.")
- */
-      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_child->type_num); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 832, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_XDECREF_SET(__pyx_v_t, __pyx_t_4);
-      __pyx_t_4 = 0;
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":833
- *         if not PyDataType_HASFIELDS(child):
- *             t = child.type_num
- *             if end - f < 5:             # <<<<<<<<<<<<<<
- *                 raise RuntimeError(u"Format string allocated too short.")
- * 
- */
-      __pyx_t_6 = (((__pyx_v_end - __pyx_v_f) < 5) != 0);
-      if (unlikely(__pyx_t_6)) {
-
-        /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":834
- *             t = child.type_num
- *             if end - f < 5:
- *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
- * 
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- */
-        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 834, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_Raise(__pyx_t_4, 0, 0, 0);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __PYX_ERR(1, 834, __pyx_L1_error)
-
-        /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":833
- *         if not PyDataType_HASFIELDS(child):
- *             t = child.type_num
- *             if end - f < 5:             # <<<<<<<<<<<<<<
- *                 raise RuntimeError(u"Format string allocated too short.")
- * 
- */
-      }
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":837
- * 
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- *             if   t == NPY_BYTE:        f[0] =  98 #"b"             # <<<<<<<<<<<<<<
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_BYTE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 837, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 837, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 837, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 98;
-        goto __pyx_L15;
-      }
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":838
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- *             if   t == NPY_BYTE:        f[0] =  98 #"b"
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"             # <<<<<<<<<<<<<<
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UBYTE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 838, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 838, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 838, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 66;
-        goto __pyx_L15;
-      }
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":839
- *             if   t == NPY_BYTE:        f[0] =  98 #"b"
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"             # <<<<<<<<<<<<<<
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_SHORT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 839, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 839, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 839, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x68;
-        goto __pyx_L15;
-      }
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":840
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"             # <<<<<<<<<<<<<<
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_USHORT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 840, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 840, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 840, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 72;
-        goto __pyx_L15;
-      }
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":841
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- *             elif t == NPY_INT:         f[0] = 105 #"i"             # <<<<<<<<<<<<<<
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_INT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 841, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 841, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 841, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x69;
-        goto __pyx_L15;
-      }
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":842
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- *             elif t == NPY_UINT:        f[0] =  73 #"I"             # <<<<<<<<<<<<<<
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UINT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 842, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 842, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 842, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 73;
-        goto __pyx_L15;
-      }
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":843
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- *             elif t == NPY_LONG:        f[0] = 108 #"l"             # <<<<<<<<<<<<<<
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 843, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 843, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 843, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x6C;
-        goto __pyx_L15;
-      }
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":844
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"             # <<<<<<<<<<<<<<
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 844, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 844, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 844, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 76;
-        goto __pyx_L15;
-      }
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":845
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"             # <<<<<<<<<<<<<<
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGLONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 845, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 845, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 845, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x71;
-        goto __pyx_L15;
-      }
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":846
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"             # <<<<<<<<<<<<<<
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONGLONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 846, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 846, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 846, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 81;
-        goto __pyx_L15;
-      }
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":847
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"             # <<<<<<<<<<<<<<
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_FLOAT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 847, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 847, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 847, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x66;
-        goto __pyx_L15;
-      }
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":848
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"             # <<<<<<<<<<<<<<
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_DOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 848, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 848, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 848, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x64;
-        goto __pyx_L15;
-      }
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":849
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"             # <<<<<<<<<<<<<<
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 849, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 849, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 849, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x67;
-        goto __pyx_L15;
-      }
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":850
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf             # <<<<<<<<<<<<<<
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CFLOAT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 850, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 850, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 850, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 90;
-        (__pyx_v_f[1]) = 0x66;
-        __pyx_v_f = (__pyx_v_f + 1);
-        goto __pyx_L15;
-      }
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":851
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd             # <<<<<<<<<<<<<<
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 851, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 851, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 851, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 90;
-        (__pyx_v_f[1]) = 0x64;
-        __pyx_v_f = (__pyx_v_f + 1);
-        goto __pyx_L15;
-      }
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":852
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg             # <<<<<<<<<<<<<<
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
- *             else:
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CLONGDOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 852, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 852, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 852, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 90;
-        (__pyx_v_f[1]) = 0x67;
-        __pyx_v_f = (__pyx_v_f + 1);
-        goto __pyx_L15;
-      }
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":853
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"             # <<<<<<<<<<<<<<
- *             else:
- *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_OBJECT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 853, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 853, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 853, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (likely(__pyx_t_6)) {
-        (__pyx_v_f[0]) = 79;
-        goto __pyx_L15;
-      }
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":855
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
- *             else:
- *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
- *             f += 1
- *         else:
- */
-      /*else*/ {
-        __pyx_t_3 = PyUnicode_Format(__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 855, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 855, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __Pyx_Raise(__pyx_t_4, 0, 0, 0);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __PYX_ERR(1, 855, __pyx_L1_error)
-      }
-      __pyx_L15:;
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":856
- *             else:
- *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- *             f += 1             # <<<<<<<<<<<<<<
- *         else:
- *             # Cython ignores struct boundary information ("T{...}"),
- */
-      __pyx_v_f = (__pyx_v_f + 1);
-
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":831
- *         offset[0] += child.itemsize
- * 
- *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
- *             t = child.type_num
- *             if end - f < 5:
- */
-      goto __pyx_L13;
-    }
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":860
- *             # Cython ignores struct boundary information ("T{...}"),
- *             # so don't output it
- *             f = _util_dtypestring(child, f, end, offset)             # <<<<<<<<<<<<<<
- *     return f
- * 
- */
-    /*else*/ {
-      __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_child, __pyx_v_f, __pyx_v_end, __pyx_v_offset); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(1, 860, __pyx_L1_error)
-      __pyx_v_f = __pyx_t_9;
-    }
-    __pyx_L13:;
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":805
- *     cdef tuple fields
- * 
- *     for childname in descr.names:             # <<<<<<<<<<<<<<
- *         fields = descr.fields[childname]
- *         child, new_offset = fields
- */
-  }
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":861
- *             # so don't output it
- *             f = _util_dtypestring(child, f, end, offset)
- *     return f             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = __pyx_v_f;
-  goto __pyx_L0;
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":796
- *         return ()
- * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
- *     # Recursive utility function used in __getbuffer__ to get format
- *     # string. The new location in the format string is returned.
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("numpy._util_dtypestring", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_child);
-  __Pyx_XDECREF(__pyx_v_fields);
-  __Pyx_XDECREF(__pyx_v_childname);
-  __Pyx_XDECREF(__pyx_v_new_offset);
-  __Pyx_XDECREF(__pyx_v_t);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":977
- * 
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":929
+ *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
- *      cdef PyObject* baseptr
- *      if base is None:
+ *     Py_INCREF(base) # important to do this before stealing the reference below!
+ *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
-  PyObject *__pyx_v_baseptr;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  int __pyx_t_2;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":979
- * cdef inline void set_array_base(ndarray arr, object base):
- *      cdef PyObject* baseptr
- *      if base is None:             # <<<<<<<<<<<<<<
- *          baseptr = NULL
- *      else:
- */
-  __pyx_t_1 = (__pyx_v_base == Py_None);
-  __pyx_t_2 = (__pyx_t_1 != 0);
-  if (__pyx_t_2) {
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":980
- *      cdef PyObject* baseptr
- *      if base is None:
- *          baseptr = NULL             # <<<<<<<<<<<<<<
- *      else:
- *          Py_INCREF(base) # important to do this before decref below!
- */
-    __pyx_v_baseptr = NULL;
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":979
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":930
+ * 
  * cdef inline void set_array_base(ndarray arr, object base):
- *      cdef PyObject* baseptr
- *      if base is None:             # <<<<<<<<<<<<<<
- *          baseptr = NULL
- *      else:
- */
-    goto __pyx_L3;
-  }
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":982
- *          baseptr = NULL
- *      else:
- *          Py_INCREF(base) # important to do this before decref below!             # <<<<<<<<<<<<<<
- *          baseptr = <PyObject*>base
- *      Py_XDECREF(arr.base)
- */
-  /*else*/ {
-    Py_INCREF(__pyx_v_base);
-
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":983
- *      else:
- *          Py_INCREF(base) # important to do this before decref below!
- *          baseptr = <PyObject*>base             # <<<<<<<<<<<<<<
- *      Py_XDECREF(arr.base)
- *      arr.base = baseptr
- */
-    __pyx_v_baseptr = ((PyObject *)__pyx_v_base);
-  }
-  __pyx_L3:;
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":984
- *          Py_INCREF(base) # important to do this before decref below!
- *          baseptr = <PyObject*>base
- *      Py_XDECREF(arr.base)             # <<<<<<<<<<<<<<
- *      arr.base = baseptr
+ *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
+ *     PyArray_SetBaseObject(arr, base)
  * 
  */
-  Py_XDECREF(__pyx_v_arr->base);
+  Py_INCREF(__pyx_v_base);
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":985
- *          baseptr = <PyObject*>base
- *      Py_XDECREF(arr.base)
- *      arr.base = baseptr             # <<<<<<<<<<<<<<
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":931
+ * cdef inline void set_array_base(ndarray arr, object base):
+ *     Py_INCREF(base) # important to do this before stealing the reference below!
+ *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  __pyx_v_arr->base = __pyx_v_baseptr;
+  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":977
- * 
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":929
+ *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
- *      cdef PyObject* baseptr
- *      if base is None:
+ *     Py_INCREF(base) # important to do this before stealing the reference below!
+ *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":987
- *      arr.base = baseptr
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":933
+ *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
- *     if arr.base is NULL:
- *         return None
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
+  PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":988
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
- *     if arr.base is NULL:             # <<<<<<<<<<<<<<
+ *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
+ *     if base is NULL:
  *         return None
- *     else:
  */
-  __pyx_t_1 = ((__pyx_v_arr->base == NULL) != 0);
-  if (__pyx_t_1) {
+  __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":989
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
- *     if arr.base is NULL:
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:             # <<<<<<<<<<<<<<
+ *         return None
+ *     return <object>base
+ */
+  __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
+  if (__pyx_t_1) {
+
+    /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":936
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
- *     else:
- *         return <object>arr.base
+ *     return <object>base
+ * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":988
- * 
+    /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
- *     if arr.base is NULL:             # <<<<<<<<<<<<<<
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
- *     else:
+ *     return <object>base
  */
   }
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":991
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":937
+ *     if base is NULL:
  *         return None
- *     else:
- *         return <object>arr.base             # <<<<<<<<<<<<<<
- * 
+ *     return <object>base             # <<<<<<<<<<<<<<
  * 
+ * # Versions of the import_* functions which are more suitable for
  */
-  /*else*/ {
-    __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(((PyObject *)__pyx_v_arr->base));
-    __pyx_r = ((PyObject *)__pyx_v_arr->base);
-    goto __pyx_L0;
-  }
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(((PyObject *)__pyx_v_base));
+  __pyx_r = ((PyObject *)__pyx_v_base);
+  goto __pyx_L0;
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":987
- *      arr.base = baseptr
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":933
+ *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
- *     if arr.base is NULL:
- *         return None
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":996
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
- *         _import_array()
+ *         __pyx_import_array()
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_import_array(void) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":997
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:
  */
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":998
+      /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
- *         _import_array()             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 998, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":997
+      /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":999
+    /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *     try:
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 999, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":1000
- *         _import_array()
+      /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":945
+ *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1000, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 1000, __pyx_L5_except_error)
+      __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":997
+    /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":996
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
- *         _import_array()
+ *         __pyx_import_array()
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_5);
@@ -5329,15 +3884,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":1002
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5348,17 +3903,20 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":1003
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5366,84 +3924,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":1004
+      /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1004, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":1003
+      /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":1005
+    /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1005, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":1006
+      /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1006, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 1006, __pyx_L5_except_error)
+      __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":1003
+    /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":1002
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5458,15 +4016,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":1008
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5477,17 +4035,20 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":1009
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5495,81 +4056,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":1010
+      /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1010, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":1009
+      /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":1011
+    /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
+ * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1011, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":1012
+      /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1012, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 1012, __pyx_L5_except_error)
+      __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":1009
+    /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":1008
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5584,14 +4148,188 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
+
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":979
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
+
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":994
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
+  npy_datetime __pyx_r;
+
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+ *     also needed.  That can be found using `get_datetime64_unit`.
+ *     """
+ *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
+  npy_timedelta __pyx_r;
+
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ *     """
+ *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
+  NPY_DATETIMEUNIT __pyx_r;
+
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":1018
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ *     """
+ *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ */
+  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
+  goto __pyx_L0;
+
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
@@ -5619,251 +4357,172 @@
     NULL, /* m_reload */
   #endif
     NULL, /* m_traverse */
     NULL, /* m_clear */
     NULL /* m_free */
 };
 #endif
+#ifndef CYTHON_SMALL_CODE
+#if defined(__clang__)
+    #define CYTHON_SMALL_CODE
+#elif defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 3))
+    #define CYTHON_SMALL_CODE __attribute__((cold))
+#else
+    #define CYTHON_SMALL_CODE
+#endif
+#endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_n_s_DTYPE, __pyx_k_DTYPE, sizeof(__pyx_k_DTYPE), 0, 0, 1, 1},
-  {&__pyx_kp_u_Format_string_allocated_too_shor, __pyx_k_Format_string_allocated_too_shor, sizeof(__pyx_k_Format_string_allocated_too_shor), 0, 1, 0, 0},
-  {&__pyx_kp_u_Format_string_allocated_too_shor_2, __pyx_k_Format_string_allocated_too_shor_2, sizeof(__pyx_k_Format_string_allocated_too_shor_2), 0, 1, 0, 0},
-  {&__pyx_n_s_ITYPE, __pyx_k_ITYPE, sizeof(__pyx_k_ITYPE), 0, 0, 1, 1},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
-  {&__pyx_kp_u_Non_native_byte_order_not_suppor, __pyx_k_Non_native_byte_order_not_suppor, sizeof(__pyx_k_Non_native_byte_order_not_suppor), 0, 1, 0, 0},
-  {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
   {&__pyx_n_s_U64TYPE, __pyx_k_U64TYPE, sizeof(__pyx_k_U64TYPE), 0, 0, 1, 1},
-  {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_counter, __pyx_k_counter, sizeof(__pyx_k_counter), 0, 0, 1, 1},
   {&__pyx_n_s_double, __pyx_k_double, sizeof(__pyx_k_double), 0, 0, 1, 1},
   {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
-  {&__pyx_n_s_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_mt, __pyx_k_mt, sizeof(__pyx_k_mt), 0, 0, 1, 1},
   {&__pyx_n_s_n, __pyx_k_n, sizeof(__pyx_k_n), 0, 0, 1, 1},
-  {&__pyx_kp_u_ndarray_is_not_C_contiguous, __pyx_k_ndarray_is_not_C_contiguous, sizeof(__pyx_k_ndarray_is_not_C_contiguous), 0, 1, 0, 0},
-  {&__pyx_kp_u_ndarray_is_not_Fortran_contiguou, __pyx_k_ndarray_is_not_Fortran_contiguou, sizeof(__pyx_k_ndarray_is_not_Fortran_contiguou), 0, 1, 0, 0},
+  {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_normal, __pyx_k_normal, sizeof(__pyx_k_normal), 0, 0, 1, 1},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_kp_s_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 0, 1, 0},
   {&__pyx_kp_s_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 0, 1, 0},
   {&__pyx_n_s_poisson, __pyx_k_poisson, sizeof(__pyx_k_poisson), 0, 0, 1, 1},
   {&__pyx_n_s_poisson_multlam, __pyx_k_poisson_multlam, sizeof(__pyx_k_poisson_multlam), 0, 0, 1, 1},
   {&__pyx_n_s_pymt64, __pyx_k_pymt64, sizeof(__pyx_k_pymt64), 0, 0, 1, 1},
   {&__pyx_kp_s_pymt64_pyx, __pyx_k_pymt64_pyx, sizeof(__pyx_k_pymt64_pyx), 0, 0, 1, 0},
-  {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_seed, __pyx_k_seed, sizeof(__pyx_k_seed), 0, 0, 1, 1},
   {&__pyx_n_s_series, __pyx_k_series, sizeof(__pyx_k_series), 0, 0, 1, 1},
   {&__pyx_n_s_series1, __pyx_k_series1, sizeof(__pyx_k_series1), 0, 0, 1, 1},
   {&__pyx_n_s_series2, __pyx_k_series2, sizeof(__pyx_k_series2), 0, 0, 1, 1},
   {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_uint64, __pyx_k_uint64, sizeof(__pyx_k_uint64), 0, 0, 1, 1},
   {&__pyx_n_s_uniform, __pyx_k_uniform, sizeof(__pyx_k_uniform), 0, 0, 1, 1},
-  {&__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_k_unknown_dtype_code_in_numpy_pxd, sizeof(__pyx_k_unknown_dtype_code_in_numpy_pxd), 0, 1, 0, 0},
   {&__pyx_n_s_xm, __pyx_k_xm, sizeof(__pyx_k_xm), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
-static int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 229, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(1, 242, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(1, 810, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 1000, __pyx_L1_error)
+static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
-static int __Pyx_InitCachedConstants(void) {
+static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":229
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_C_contiguous); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 229, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple_);
-  __Pyx_GIVEREF(__pyx_tuple_);
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":233
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
- * 
- *             info.buf = PyArray_DATA(self)
- */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_Fortran_contiguou); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 233, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":263
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"
- */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_Non_native_byte_order_not_suppor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 263, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":810
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
- * 
- *         if ((child.byteorder == c'>' and little_endian) or
- */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 810, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":814
- *         if ((child.byteorder == c'>' and little_endian) or
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *             # One could encode it in the format string and have Cython
- *             # complain instead, BUT: < and > in format strings also imply
- */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_Non_native_byte_order_not_suppor); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 814, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":834
- *             t = child.type_num
- *             if end - f < 5:
- *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
- * 
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor_2); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 834, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":1000
- *         _import_array()
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":945
+ *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 1000, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 945, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple_);
+  __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":1006
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 1006, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
-
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":1012
- *         _import_umath()
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
- */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 1012, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 951, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "pymt64.pyx":87
- *     cdef void poissonn_multlam( UL64 * mt , int * mti , double * xm, double * x , long n )
+  /* "pymt64.pyx":88
+ * 
  * 
  * def init(unsigned long long  seed ):             # <<<<<<<<<<<<<<
  *     '''
  *     Function used to initialise the state vector mt used by the pseudorandom number generator.
  */
-  __pyx_tuple__10 = PyTuple_Pack(4, __pyx_n_s_seed, __pyx_n_s_seed, __pyx_n_s_mt, __pyx_n_s_counter); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 87, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pymt64_pyx, __pyx_n_s_init, 87, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(4, __pyx_n_s_seed, __pyx_n_s_seed, __pyx_n_s_mt, __pyx_n_s_counter); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pymt64_pyx, __pyx_n_s_init, 88, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 88, __pyx_L1_error)
 
-  /* "pymt64.pyx":105
+  /* "pymt64.pyx":106
  *     return mt
  * 
  * def uniform(np.ndarray [U64TYPE_t,ndim=1, mode='c'] mt , int n):             # <<<<<<<<<<<<<<
  *     '''
  *     Generates n random numbers on [0,1]-real-interval
  */
-  __pyx_tuple__12 = PyTuple_Pack(4, __pyx_n_s_mt, __pyx_n_s_n, __pyx_n_s_series, __pyx_n_s_counter); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 105, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pymt64_pyx, __pyx_n_s_uniform, 105, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(4, __pyx_n_s_mt, __pyx_n_s_n, __pyx_n_s_series, __pyx_n_s_counter); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pymt64_pyx, __pyx_n_s_uniform, 106, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 106, __pyx_L1_error)
 
-  /* "pymt64.pyx":121
+  /* "pymt64.pyx":122
  *     return series
  * 
  * def poisson(np.ndarray [U64TYPE_t,ndim=1, mode='c'] mt , double xm , int n):             # <<<<<<<<<<<<<<
  *     '''
  * 
  */
-  __pyx_tuple__14 = PyTuple_Pack(5, __pyx_n_s_mt, __pyx_n_s_xm, __pyx_n_s_n, __pyx_n_s_series, __pyx_n_s_counter); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 121, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pymt64_pyx, __pyx_n_s_poisson, 121, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 121, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(5, __pyx_n_s_mt, __pyx_n_s_xm, __pyx_n_s_n, __pyx_n_s_series, __pyx_n_s_counter); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 122, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pymt64_pyx, __pyx_n_s_poisson, 122, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 122, __pyx_L1_error)
 
-  /* "pymt64.pyx":139
+  /* "pymt64.pyx":140
  * 
  * 
  * def normal(np.ndarray [U64TYPE_t,ndim=1, mode='c'] mt ,  int n):             # <<<<<<<<<<<<<<
  * 
  *     '''
  */
-  __pyx_tuple__16 = PyTuple_Pack(5, __pyx_n_s_mt, __pyx_n_s_n, __pyx_n_s_series1, __pyx_n_s_series2, __pyx_n_s_counter); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 139, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pymt64_pyx, __pyx_n_s_normal, 139, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 139, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(5, __pyx_n_s_mt, __pyx_n_s_n, __pyx_n_s_series1, __pyx_n_s_series2, __pyx_n_s_counter); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 140, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pymt64_pyx, __pyx_n_s_normal, 140, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 140, __pyx_L1_error)
 
-  /* "pymt64.pyx":156
+  /* "pymt64.pyx":157
  *     return series1,series2
  * 
  * def  poisson_multlam(np.ndarray [U64TYPE_t,ndim=1, mode='c'] mt , np.ndarray [DTYPE_t,ndim=1, mode='c'] xm):             # <<<<<<<<<<<<<<
  * 
  *     '''
  */
-  __pyx_tuple__18 = PyTuple_Pack(4, __pyx_n_s_mt, __pyx_n_s_xm, __pyx_n_s_series, __pyx_n_s_counter); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 156, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pymt64_pyx, __pyx_n_s_poisson_multlam, 156, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(4, __pyx_n_s_mt, __pyx_n_s_xm, __pyx_n_s_series, __pyx_n_s_counter); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 157, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pymt64_pyx, __pyx_n_s_poisson_multlam, 157, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 157, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
-static int __Pyx_InitGlobals(void) {
+static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
-static int __Pyx_modinit_global_init_code(void); /*proto*/
-static int __Pyx_modinit_variable_export_code(void); /*proto*/
-static int __Pyx_modinit_function_export_code(void); /*proto*/
-static int __Pyx_modinit_type_init_code(void); /*proto*/
-static int __Pyx_modinit_type_import_code(void); /*proto*/
-static int __Pyx_modinit_variable_import_code(void); /*proto*/
-static int __Pyx_modinit_function_import_code(void); /*proto*/
+static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
+static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
+static CYTHON_SMALL_CODE int __Pyx_modinit_function_export_code(void); /*proto*/
+static CYTHON_SMALL_CODE int __Pyx_modinit_type_init_code(void); /*proto*/
+static CYTHON_SMALL_CODE int __Pyx_modinit_type_import_code(void); /*proto*/
+static CYTHON_SMALL_CODE int __Pyx_modinit_variable_import_code(void); /*proto*/
+static CYTHON_SMALL_CODE int __Pyx_modinit_function_import_code(void); /*proto*/
 
 static int __Pyx_modinit_global_init_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_global_init_code", 0);
   /*--- Global init code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
@@ -5891,31 +4550,68 @@
   /*--- Type init code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static int __Pyx_modinit_type_import_code(void) {
   __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
-  0); if (unlikely(!__pyx_ptype_7cpython_4type_type)) __PYX_ERR(2, 9, __pyx_L1_error)
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType("numpy", "dtype", sizeof(PyArray_Descr), 0); if (unlikely(!__pyx_ptype_5numpy_dtype)) __PYX_ERR(1, 164, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType("numpy", "flatiter", sizeof(PyArrayIterObject), 0); if (unlikely(!__pyx_ptype_5numpy_flatiter)) __PYX_ERR(1, 186, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType("numpy", "broadcast", sizeof(PyArrayMultiIterObject), 0); if (unlikely(!__pyx_ptype_5numpy_broadcast)) __PYX_ERR(1, 190, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType("numpy", "ndarray", sizeof(PyArrayObject), 0); if (unlikely(!__pyx_ptype_5numpy_ndarray)) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType("numpy", "ufunc", sizeof(PyUFuncObject), 0); if (unlikely(!__pyx_ptype_5numpy_ufunc)) __PYX_ERR(1, 872, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static int __Pyx_modinit_variable_import_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_variable_import_code", 0);
@@ -5929,106 +4625,136 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
-#if PY_MAJOR_VERSION < 3
-#ifdef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC void
-#else
+#ifndef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
-#endif
-#else
-#ifdef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC PyObject *
+#elif PY_MAJOR_VERSION < 3
+#ifdef __cplusplus
+#define __Pyx_PyMODINIT_FUNC extern "C" void
 #else
-#define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
-#endif
+#define __Pyx_PyMODINIT_FUNC void
 #endif
-#ifndef CYTHON_SMALL_CODE
-#if defined(__clang__)
-    #define CYTHON_SMALL_CODE
-#elif defined(__GNUC__) && (!(defined(__cplusplus)) || (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ > 4)))
-    #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
-    #define CYTHON_SMALL_CODE
+#ifdef __cplusplus
+#define __Pyx_PyMODINIT_FUNC extern "C" PyObject *
+#else
+#define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
 __Pyx_PyMODINIT_FUNC initpymt64(void) CYTHON_SMALL_CODE; /*proto*/
 __Pyx_PyMODINIT_FUNC initpymt64(void)
 #else
 __Pyx_PyMODINIT_FUNC PyInit_pymt64(void) CYTHON_SMALL_CODE; /*proto*/
 __Pyx_PyMODINIT_FUNC PyInit_pymt64(void)
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 {
   return PyModuleDef_Init(&__pyx_moduledef);
 }
-static int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name) {
+static CYTHON_SMALL_CODE int __Pyx_check_single_interpreter(void) {
+    #if PY_VERSION_HEX >= 0x030700A1
+    static PY_INT64_T main_interpreter_id = -1;
+    PY_INT64_T current_id = PyInterpreterState_GetID(PyThreadState_Get()->interp);
+    if (main_interpreter_id == -1) {
+        main_interpreter_id = current_id;
+        return (unlikely(current_id == -1)) ? -1 : 0;
+    } else if (unlikely(main_interpreter_id != current_id))
+    #else
+    static PyInterpreterState *main_interpreter = NULL;
+    PyInterpreterState *current_interpreter = PyThreadState_Get()->interp;
+    if (!main_interpreter) {
+        main_interpreter = current_interpreter;
+    } else if (unlikely(main_interpreter != current_interpreter))
+    #endif
+    {
+        PyErr_SetString(
+            PyExc_ImportError,
+            "Interpreter change detected - this module can only be loaded into one interpreter per process.");
+        return -1;
+    }
+    return 0;
+}
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none) {
     PyObject *value = PyObject_GetAttrString(spec, from_name);
     int result = 0;
     if (likely(value)) {
-        result = PyDict_SetItemString(moddict, to_name, value);
+        if (allow_none || value != Py_None) {
+            result = PyDict_SetItemString(moddict, to_name, value);
+        }
         Py_DECREF(value);
     } else if (PyErr_ExceptionMatches(PyExc_AttributeError)) {
         PyErr_Clear();
     } else {
         result = -1;
     }
     return result;
 }
-static PyObject* __pyx_pymod_create(PyObject *spec, CYTHON_UNUSED PyModuleDef *def) {
+static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, CYTHON_UNUSED PyModuleDef *def) {
     PyObject *module = NULL, *moddict, *modname;
+    if (__Pyx_check_single_interpreter())
+        return NULL;
     if (__pyx_m)
         return __Pyx_NewRef(__pyx_m);
     modname = PyObject_GetAttrString(spec, "name");
     if (unlikely(!modname)) goto bad;
     module = PyModule_NewObject(modname);
     Py_DECREF(modname);
     if (unlikely(!module)) goto bad;
     moddict = PyModule_GetDict(module);
     if (unlikely(!moddict)) goto bad;
-    if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "loader", "__loader__") < 0)) goto bad;
-    if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "origin", "__file__") < 0)) goto bad;
-    if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "parent", "__package__") < 0)) goto bad;
-    if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "submodule_search_locations", "__path__") < 0)) goto bad;
+    if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "loader", "__loader__", 1) < 0)) goto bad;
+    if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "origin", "__file__", 1) < 0)) goto bad;
+    if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "parent", "__package__", 1) < 0)) goto bad;
+    if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "submodule_search_locations", "__path__", 0) < 0)) goto bad;
     return module;
 bad:
     Py_XDECREF(module);
     return NULL;
 }
 
 
-static int __pyx_pymod_exec_pymt64(PyObject *__pyx_pyinit_module)
+static CYTHON_SMALL_CODE int __pyx_pymod_exec_pymt64(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
-  if (__pyx_m && __pyx_m == __pyx_pyinit_module) return 0;
+  if (__pyx_m) {
+    if (__pyx_m == __pyx_pyinit_module) return 0;
+    PyErr_SetString(PyExc_RuntimeError, "Module 'pymt64' has already been imported. Re-initialisation is not supported.");
+    return -1;
+  }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
   __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_pymt64(void)", 0);
   if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  #ifdef __Pxy_PyFrame_Initialize_Offsets
+  __Pxy_PyFrame_Initialize_Offsets();
+  #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
   if (__pyx_CyFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_FusedFunction_USED
@@ -6044,19 +4770,17 @@
   if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
   if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
-  #ifdef WITH_THREAD /* Python build with threading support? */
+  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
-  #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("pymt64", __pyx_methods, __pyx_k_PyMT64_PyMT64_is_a_Python_versi, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
@@ -6064,26 +4788,25 @@
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   #endif
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  #if CYTHON_COMPILING_IN_PYPY
   Py_INCREF(__pyx_b);
-  #endif
+  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_cython_runtime);
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_pymt64) {
-    if (PyObject_SetAttrString(__pyx_m, "__name__", __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "pymt64")) {
       if (unlikely(PyDict_SetItemString(modules, "pymt64", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
@@ -6094,15 +4817,15 @@
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
   (void)__Pyx_modinit_type_init_code();
-  if (unlikely(__Pyx_modinit_type_import_code() != 0)) goto __pyx_L1_error;
+  if (unlikely(__Pyx_modinit_type_import_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
@@ -6118,153 +4841,138 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pymt64.pyx":62
  * # DTYPE for this, which is assigned to the usual NumPy runtime
  * # type info object.
  * DTYPE = np.double             # <<<<<<<<<<<<<<
- * ITYPE = np.int
+ * #DTYPE = np.int
  * U64TYPE = np.uint64
  */
-  __pyx_t_1 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_double); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_DTYPE, __pyx_t_2) < 0) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pymt64.pyx":63
- * # type info object.
- * DTYPE = np.double
- * ITYPE = np.int             # <<<<<<<<<<<<<<
- * U64TYPE = np.uint64
- * # "ctypedef" assigns a corresponding compile-time type to DTYPE_t. For
- */
-  __pyx_t_2 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ITYPE, __pyx_t_1) < 0) __PYX_ERR(0, 63, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
   /* "pymt64.pyx":64
  * DTYPE = np.double
- * ITYPE = np.int
+ * #DTYPE = np.int
  * U64TYPE = np.uint64             # <<<<<<<<<<<<<<
  * # "ctypedef" assigns a corresponding compile-time type to DTYPE_t. For
  * # every type in the numpy module there's a corresponding compile-time
  */
-  __pyx_t_1 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_uint64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_U64TYPE, __pyx_t_2) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_U64TYPE, __pyx_t_1) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pymt64.pyx":76
  * 
  * cimport cython
  * cdef int MTSIZE = 312             # <<<<<<<<<<<<<<
  * cdef extern from "mt64mp.h":
  *     ctypedef unsigned long long UL64
  */
   __pyx_v_6pymt64_MTSIZE = 0x138;
 
-  /* "pymt64.pyx":87
- *     cdef void poissonn_multlam( UL64 * mt , int * mti , double * xm, double * x , long n )
+  /* "pymt64.pyx":88
+ * 
  * 
  * def init(unsigned long long  seed ):             # <<<<<<<<<<<<<<
  *     '''
  *     Function used to initialise the state vector mt used by the pseudorandom number generator.
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_6pymt64_1init, NULL, __pyx_n_s_pymt64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_init, __pyx_t_2) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6pymt64_1init, NULL, __pyx_n_s_pymt64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_init, __pyx_t_1) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pymt64.pyx":105
+  /* "pymt64.pyx":106
  *     return mt
  * 
  * def uniform(np.ndarray [U64TYPE_t,ndim=1, mode='c'] mt , int n):             # <<<<<<<<<<<<<<
  *     '''
  *     Generates n random numbers on [0,1]-real-interval
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_6pymt64_3uniform, NULL, __pyx_n_s_pymt64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 105, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_uniform, __pyx_t_2) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6pymt64_3uniform, NULL, __pyx_n_s_pymt64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_uniform, __pyx_t_1) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pymt64.pyx":121
+  /* "pymt64.pyx":122
  *     return series
  * 
  * def poisson(np.ndarray [U64TYPE_t,ndim=1, mode='c'] mt , double xm , int n):             # <<<<<<<<<<<<<<
  *     '''
  * 
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_6pymt64_5poisson, NULL, __pyx_n_s_pymt64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 121, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_poisson, __pyx_t_2) < 0) __PYX_ERR(0, 121, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6pymt64_5poisson, NULL, __pyx_n_s_pymt64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_poisson, __pyx_t_1) < 0) __PYX_ERR(0, 122, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pymt64.pyx":139
+  /* "pymt64.pyx":140
  * 
  * 
  * def normal(np.ndarray [U64TYPE_t,ndim=1, mode='c'] mt ,  int n):             # <<<<<<<<<<<<<<
  * 
  *     '''
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_6pymt64_7normal, NULL, __pyx_n_s_pymt64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_normal, __pyx_t_2) < 0) __PYX_ERR(0, 139, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6pymt64_7normal, NULL, __pyx_n_s_pymt64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 140, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_normal, __pyx_t_1) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pymt64.pyx":156
+  /* "pymt64.pyx":157
  *     return series1,series2
  * 
  * def  poisson_multlam(np.ndarray [U64TYPE_t,ndim=1, mode='c'] mt , np.ndarray [DTYPE_t,ndim=1, mode='c'] xm):             # <<<<<<<<<<<<<<
  * 
  *     '''
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_6pymt64_9poisson_multlam, NULL, __pyx_n_s_pymt64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_poisson_multlam, __pyx_t_2) < 0) __PYX_ERR(0, 156, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6pymt64_9poisson_multlam, NULL, __pyx_n_s_pymt64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_poisson_multlam, __pyx_t_1) < 0) __PYX_ERR(0, 157, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pymt64.pyx":1
  * '''             # <<<<<<<<<<<<<<
  *                      PyMT64
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../anaconda2/envs/py3.5/lib/python3.5/site-packages/Cython/Includes/numpy/__init__.pxd":1008
- *         raise ImportError("numpy.core.umath failed to import")
+  /* "../../../venv/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
- * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   if (__pyx_m) {
     if (__pyx_d) {
-      __Pyx_AddTraceback("init pymt64", 0, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init pymt64", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
-    Py_DECREF(__pyx_m); __pyx_m = 0;
+    Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init pymt64");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
@@ -6277,17 +4985,17 @@
 
 /* --- Runtime support code --- */
 /* Refnanny */
 #if CYTHON_REFNANNY
 static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname) {
     PyObject *m = NULL, *p = NULL;
     void *r = NULL;
-    m = PyImport_ImportModule((char *)modname);
+    m = PyImport_ImportModule(modname);
     if (!m) goto end;
-    p = PyObject_GetAttrString(m, (char *)"RefNannyAPI");
+    p = PyObject_GetAttrString(m, "RefNannyAPI");
     if (!p) goto end;
     r = PyLong_AsVoidPtr(p);
 end:
     Py_XDECREF(p);
     Py_XDECREF(m);
     return (__Pyx_RefNannyAPIStruct *)r;
 }
@@ -6317,46 +5025,80 @@
 #else
             "name '%.200s' is not defined", PyString_AS_STRING(name));
 #endif
     }
     return result;
 }
 
+/* PyDictVersioning */
+#if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
+    PyObject *dict = Py_TYPE(obj)->tp_dict;
+    return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
+}
+static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
+    PyObject **dictptr = NULL;
+    Py_ssize_t offset = Py_TYPE(obj)->tp_dictoffset;
+    if (offset) {
+#if CYTHON_COMPILING_IN_CPYTHON
+        dictptr = (likely(offset > 0)) ? (PyObject **) ((char *)obj + offset) : _PyObject_GetDictPtr(obj);
+#else
+        dictptr = _PyObject_GetDictPtr(obj);
+#endif
+    }
+    return (dictptr && *dictptr) ? __PYX_GET_DICT_VERSION(*dictptr) : 0;
+}
+static CYTHON_INLINE int __Pyx_object_dict_version_matches(PyObject* obj, PY_UINT64_T tp_dict_version, PY_UINT64_T obj_dict_version) {
+    PyObject *dict = Py_TYPE(obj)->tp_dict;
+    if (unlikely(!dict) || unlikely(tp_dict_version != __PYX_GET_DICT_VERSION(dict)))
+        return 0;
+    return obj_dict_version == __Pyx_get_object_dict_version(obj);
+}
+#endif
+
 /* GetModuleGlobalName */
-static CYTHON_INLINE PyObject *__Pyx_GetModuleGlobalName(PyObject *name) {
+#if CYTHON_USE_DICT_VERSIONS
+static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value)
+#else
+static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name)
+#endif
+{
     PyObject *result;
 #if !CYTHON_AVOID_BORROWED_REFS
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
     result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
+    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
-        Py_INCREF(result);
+        return __Pyx_NewRef(result);
     } else if (unlikely(PyErr_Occurred())) {
-        result = NULL;
-    } else {
+        return NULL;
+    }
 #else
     result = PyDict_GetItem(__pyx_d, name);
+    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
-        Py_INCREF(result);
-    } else {
+        return __Pyx_NewRef(result);
+    }
 #endif
 #else
     result = PyObject_GetItem(__pyx_d, name);
-    if (!result) {
-        PyErr_Clear();
-#endif
-        result = __Pyx_GetBuiltinName(name);
+    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
+    if (likely(result)) {
+        return __Pyx_NewRef(result);
     }
-    return result;
+    PyErr_Clear();
+#endif
+    return __Pyx_GetBuiltinName(name);
 }
 
 /* PyObjectCall */
-    #if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
-    ternaryfunc call = func->ob_type->tp_call;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
@@ -6365,39 +5107,39 @@
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
 /* ExtTypeTest */
-    static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
+static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
     if (likely(__Pyx_TypeCheck(obj, type)))
         return 1;
     PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
                  Py_TYPE(obj)->tp_name, type->tp_name);
     return 0;
 }
 
 /* IsLittleEndian */
-    static CYTHON_INLINE int __Pyx_Is_Little_Endian(void)
+static CYTHON_INLINE int __Pyx_Is_Little_Endian(void)
 {
   union {
     uint32_t u32;
     uint8_t u8[4];
   } S;
   S.u32 = 0x01020304;
   return S.u8[0] == 4;
 }
 
 /* BufferFormatCheck */
-    static void __Pyx_BufFmt_Init(__Pyx_BufFmt_Context* ctx,
+static void __Pyx_BufFmt_Init(__Pyx_BufFmt_Context* ctx,
                               __Pyx_BufFmt_StackElem* stack,
                               __Pyx_TypeInfo* type) {
   stack[0].field = &ctx->root;
   stack[0].parent_offset = 0;
   ctx->root.type = type;
   ctx->root.name = "buffer dtype";
   ctx->root.offset = 0;
@@ -6423,15 +5165,15 @@
 static int __Pyx_BufFmt_ParseNumber(const char** ts) {
     int count;
     const char* t = *ts;
     if (*t < '0' || *t > '9') {
       return -1;
     } else {
         count = *t++ - '0';
-        while (*t >= '0' && *t < '9') {
+        while (*t >= '0' && *t <= '9') {
             count *= 10;
             count += *t++ - '0';
         }
     }
     *ts = t;
     return count;
 }
@@ -6444,14 +5186,15 @@
 }
 static void __Pyx_BufFmt_RaiseUnexpectedChar(char ch) {
   PyErr_Format(PyExc_ValueError,
                "Unexpected format string character: '%c'", ch);
 }
 static const char* __Pyx_BufFmt_DescribeTypeChar(char ch, int is_complex) {
   switch (ch) {
+    case '?': return "'bool'";
     case 'c': return "'char'";
     case 'b': return "'signed char'";
     case 'B': return "'unsigned char'";
     case 'h': return "'short'";
     case 'H': return "'unsigned short'";
     case 'i': return "'int'";
     case 'I': return "'unsigned int'";
@@ -6486,15 +5229,15 @@
     default:
       __Pyx_BufFmt_RaiseUnexpectedChar(ch);
       return 0;
     }
 }
 static size_t __Pyx_BufFmt_TypeCharToNativeSize(char ch, int is_complex) {
   switch (ch) {
-    case 'c': case 'b': case 'B': case 's': case 'p': return 1;
+    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
     case 'h': case 'H': return sizeof(short);
     case 'i': case 'I': return sizeof(int);
     case 'l': case 'L': return sizeof(long);
     #ifdef HAVE_LONG_LONG
     case 'q': case 'Q': return sizeof(PY_LONG_LONG);
     #endif
     case 'f': return sizeof(float) * (is_complex ? 2 : 1);
@@ -6570,15 +5313,15 @@
 static char __Pyx_BufFmt_TypeCharToGroup(char ch, int is_complex) {
   switch (ch) {
     case 'c':
         return 'H';
     case 'b': case 'h': case 'i':
     case 'l': case 'q': case 's': case 'p':
         return 'I';
-    case 'B': case 'H': case 'I': case 'L': case 'Q':
+    case '?': case 'B': case 'H': case 'I': case 'L': case 'Q':
         return 'U';
     case 'f': case 'd': case 'g':
         return (is_complex ? 'C' : 'R');
     case 'O':
         return 'O';
     case 'P':
         return 'P';
@@ -6714,24 +5457,23 @@
   ctx->is_complex = 0;
   return 0;
 }
 static PyObject *
 __pyx_buffmt_parse_array(__Pyx_BufFmt_Context* ctx, const char** tsp)
 {
     const char *ts = *tsp;
-    int i = 0, number;
-    int ndim = ctx->head->field->type->ndim;
-;
+    int i = 0, number, ndim;
     ++ts;
     if (ctx->new_count != 1) {
         PyErr_SetString(PyExc_ValueError,
                         "Cannot handle repeated arrays in format string");
         return NULL;
     }
     if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+    ndim = ctx->head->field->type->ndim;
     while (*ts && *ts != ')') {
         switch (*ts) {
             case ' ': case '\f': case '\r': case '\n': case '\t': case '\v':  continue;
             default:  break;
         }
         number = __Pyx_BufFmt_ExpectNumber(&ts);
         if (number == -1) return NULL;
@@ -6849,20 +5591,20 @@
         got_Z = 1;
         ++ts;
         if (*ts != 'f' && *ts != 'd' && *ts != 'g') {
           __Pyx_BufFmt_RaiseUnexpectedChar('Z');
           return NULL;
         }
         CYTHON_FALLTHROUGH;
-      case 'c': case 'b': case 'B': case 'h': case 'H': case 'i': case 'I':
+      case '?': case 'c': case 'b': case 'B': case 'h': case 'H': case 'i': case 'I':
       case 'l': case 'L': case 'q': case 'Q':
       case 'f': case 'd': case 'g':
       case 'O': case 'p':
-        if (ctx->enc_type == *ts && got_Z == ctx->is_complex &&
-            ctx->enc_packmode == ctx->new_packmode) {
+        if ((ctx->enc_type == *ts) && (got_Z == ctx->is_complex) &&
+            (ctx->enc_packmode == ctx->new_packmode) && (!ctx->is_valid_array)) {
           ctx->enc_count += ctx->new_count;
           ctx->new_count = 1;
           got_Z = 0;
           ++ts;
           break;
         }
         CYTHON_FALLTHROUGH;
@@ -6891,15 +5633,15 @@
           ctx->new_count = (size_t)number;
         }
     }
   }
 }
 
 /* BufferGetAndValidate */
-      static CYTHON_INLINE void __Pyx_SafeReleaseBuffer(Py_buffer* info) {
+  static CYTHON_INLINE void __Pyx_SafeReleaseBuffer(Py_buffer* info) {
   if (unlikely(info->buf == NULL)) return;
   if (info->suboffsets == __Pyx_minusones) info->suboffsets = NULL;
   __Pyx_ReleaseBuffer(info);
 }
 static void __Pyx_ZeroBuffer(Py_buffer* buf) {
   buf->buf = NULL;
   buf->obj = NULL;
@@ -6923,36 +5665,36 @@
     goto fail;
   }
   if (!cast) {
     __Pyx_BufFmt_Context ctx;
     __Pyx_BufFmt_Init(&ctx, stack, dtype);
     if (!__Pyx_BufFmt_CheckString(&ctx, buf->format)) goto fail;
   }
-  if (unlikely((unsigned)buf->itemsize != dtype->size)) {
+  if (unlikely((size_t)buf->itemsize != dtype->size)) {
     PyErr_Format(PyExc_ValueError,
       "Item size of buffer (%" CYTHON_FORMAT_SSIZE_T "d byte%s) does not match size of '%s' (%" CYTHON_FORMAT_SSIZE_T "d byte%s)",
       buf->itemsize, (buf->itemsize > 1) ? "s" : "",
       dtype->name, (Py_ssize_t)dtype->size, (dtype->size > 1) ? "s" : "");
     goto fail;
   }
   if (buf->suboffsets == NULL) buf->suboffsets = __Pyx_minusones;
   return 0;
 fail:;
   __Pyx_SafeReleaseBuffer(buf);
   return -1;
 }
 
 /* BufferIndexError */
-      static void __Pyx_RaiseBufferIndexError(int axis) {
+  static void __Pyx_RaiseBufferIndexError(int axis) {
   PyErr_Format(PyExc_IndexError,
      "Out of bounds on buffer access (axis %d)", axis);
 }
 
 /* PyErrFetchRestore */
-      #if CYTHON_FAST_THREAD_STATE
+  #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
     tstate->curexc_type = type;
     tstate->curexc_value = value;
@@ -6968,15 +5710,15 @@
     tstate->curexc_type = 0;
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
 }
 #endif
 
 /* RaiseArgTupleInvalid */
-      static void __Pyx_RaiseArgtupleInvalid(
+  static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
     Py_ssize_t num_found)
 {
     Py_ssize_t num_expected;
@@ -6994,29 +5736,29 @@
     PyErr_Format(PyExc_TypeError,
                  "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
                  func_name, more_or_less, num_expected,
                  (num_expected == 1) ? "" : "s", num_found);
 }
 
 /* RaiseDoubleKeywords */
-      static void __Pyx_RaiseDoubleKeywordsError(
+  static void __Pyx_RaiseDoubleKeywordsError(
     const char* func_name,
     PyObject* kw_name)
 {
     PyErr_Format(PyExc_TypeError,
         #if PY_MAJOR_VERSION >= 3
         "%s() got multiple values for keyword argument '%U'", func_name, kw_name);
         #else
         "%s() got multiple values for keyword argument '%s'", func_name,
         PyString_AsString(kw_name));
         #endif
 }
 
 /* ParseKeywords */
-      static int __Pyx_ParseOptionalKeywords(
+  static int __Pyx_ParseOptionalKeywords(
     PyObject *kwds,
     PyObject **argnames[],
     PyObject *kwds2,
     PyObject *values[],
     Py_ssize_t num_pos_args,
     const char* function_name)
 {
@@ -7029,15 +5771,15 @@
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
             continue;
         }
         name = first_kw_arg;
         #if PY_MAJOR_VERSION < 3
-        if (likely(PyString_CheckExact(key)) || likely(PyString_Check(key))) {
+        if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
                     break;
                 }
                 name++;
@@ -7056,15 +5798,15 @@
             }
         } else
         #endif
         if (likely(PyUnicode_Check(key))) {
             while (*name) {
                 int cmp = (**name == key) ? 0 :
                 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                    (PyUnicode_GET_SIZE(**name) != PyUnicode_GET_SIZE(key)) ? 1 :
+                    (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
                     PyUnicode_Compare(**name, key);
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
                     break;
                 }
@@ -7072,15 +5814,15 @@
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
                 while (argname != first_kw_arg) {
                     int cmp = (**argname == key) ? 0 :
                     #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                        (PyUnicode_GET_SIZE(**argname) != PyUnicode_GET_SIZE(key)) ? 1 :
+                        (__Pyx_PyUnicode_GET_LENGTH(**argname) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                     #endif
                         PyUnicode_Compare(**argname, key);
                     if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                     if (cmp == 0) goto arg_passed_twice;
                     argname++;
                 }
             }
@@ -7110,15 +5852,15 @@
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
 /* ArgTypeTest */
-      static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
+  static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
 {
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
     else if (exact) {
         #if PY_MAJOR_VERSION == 2
@@ -7130,16 +5872,171 @@
     }
     PyErr_Format(PyExc_TypeError,
         "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
         name, type->tp_name, Py_TYPE(obj)->tp_name);
     return 0;
 }
 
+/* GetTopmostException */
+  #if CYTHON_USE_EXC_INFO_STACK
+static _PyErr_StackItem *
+__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
+{
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
+           exc_info->previous_item != NULL)
+    {
+        exc_info = exc_info->previous_item;
+    }
+    return exc_info;
+}
+#endif
+
+/* SaveResetException */
+  #if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    *type = exc_info->exc_type;
+    *value = exc_info->exc_value;
+    *tb = exc_info->exc_traceback;
+    #else
+    *type = tstate->exc_type;
+    *value = tstate->exc_value;
+    *tb = tstate->exc_traceback;
+    #endif
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+}
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_type = exc_info->exc_type;
+    tmp_value = exc_info->exc_value;
+    tmp_tb = exc_info->exc_traceback;
+    exc_info->exc_type = type;
+    exc_info->exc_value = value;
+    exc_info->exc_traceback = tb;
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = type;
+    tstate->exc_value = value;
+    tstate->exc_traceback = tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+}
+#endif
+
+/* PyErrExceptionMatches */
+  #if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+    }
+#endif
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    }
+    return 0;
+}
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    PyObject *exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
+    if (unlikely(PyTuple_Check(err)))
+        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+}
+#endif
+
+/* GetException */
+  #if CYTHON_FAST_THREAD_STATE
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+#endif
+{
+    PyObject *local_type, *local_value, *local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    local_type = tstate->curexc_type;
+    local_value = tstate->curexc_value;
+    local_tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+#else
+    PyErr_Fetch(&local_type, &local_value, &local_tb);
+#endif
+    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
+#if CYTHON_FAST_THREAD_STATE
+    if (unlikely(tstate->curexc_type))
+#else
+    if (unlikely(PyErr_Occurred()))
+#endif
+        goto bad;
+    #if PY_MAJOR_VERSION >= 3
+    if (local_tb) {
+        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
+            goto bad;
+    }
+    #endif
+    Py_XINCREF(local_tb);
+    Py_XINCREF(local_type);
+    Py_XINCREF(local_value);
+    *type = local_type;
+    *value = local_value;
+    *tb = local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    #if CYTHON_USE_EXC_INFO_STACK
+    {
+        _PyErr_StackItem *exc_info = tstate->exc_info;
+        tmp_type = exc_info->exc_type;
+        tmp_value = exc_info->exc_value;
+        tmp_tb = exc_info->exc_traceback;
+        exc_info->exc_type = local_type;
+        exc_info->exc_value = local_value;
+        exc_info->exc_traceback = local_tb;
+    }
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = local_type;
+    tstate->exc_value = local_value;
+    tstate->exc_traceback = local_tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#else
+    PyErr_SetExcInfo(local_type, local_value, local_tb);
+#endif
+    return 0;
+bad:
+    *type = 0;
+    *value = 0;
+    *tb = 0;
+    Py_XDECREF(local_type);
+    Py_XDECREF(local_value);
+    Py_XDECREF(local_tb);
+    return -1;
+}
+
 /* RaiseException */
-      #if PY_MAJOR_VERSION < 3
+  #if PY_MAJOR_VERSION < 3
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
                         CYTHON_UNUSED PyObject *cause) {
     __Pyx_PyThreadState_declare
     Py_XINCREF(type);
     if (!value || value == Py_None)
         value = NULL;
     else
@@ -7289,390 +6186,77 @@
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
-/* PyCFunctionFastCall */
-      #if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
-    PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
-    PyCFunction meth = PyCFunction_GET_FUNCTION(func);
-    PyObject *self = PyCFunction_GET_SELF(func);
-    int flags = PyCFunction_GET_FLAGS(func);
-    assert(PyCFunction_Check(func));
-    assert(METH_FASTCALL == (flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS)));
-    assert(nargs >= 0);
-    assert(nargs == 0 || args != NULL);
-    /* _PyCFunction_FastCallDict() must not be called with an exception set,
-       because it may clear it (directly or indirectly) and so the
-       caller loses its exception */
-    assert(!PyErr_Occurred());
-    if ((PY_VERSION_HEX < 0x030700A0) || unlikely(flags & METH_KEYWORDS)) {
-        return (*((__Pyx_PyCFunctionFastWithKeywords)meth)) (self, args, nargs, NULL);
-    } else {
-        return (*((__Pyx_PyCFunctionFast)meth)) (self, args, nargs);
-    }
-}
-#endif
-
-/* PyFunctionFastCall */
-      #if CYTHON_FAST_PYCALL
-#include "frameobject.h"
-static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
-                                               PyObject *globals) {
-    PyFrameObject *f;
-    PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject **fastlocals;
-    Py_ssize_t i;
-    PyObject *result;
-    assert(globals != NULL);
-    /* XXX Perhaps we should create a specialized
-       PyFrame_New() that doesn't take locals, but does
-       take builtins without sanity checking them.
-       */
-    assert(tstate != NULL);
-    f = PyFrame_New(tstate, co, globals, NULL);
-    if (f == NULL) {
-        return NULL;
-    }
-    fastlocals = f->f_localsplus;
-    for (i = 0; i < na; i++) {
-        Py_INCREF(*args);
-        fastlocals[i] = *args++;
-    }
-    result = PyEval_EvalFrameEx(f,0);
-    ++tstate->recursion_depth;
-    Py_DECREF(f);
-    --tstate->recursion_depth;
-    return result;
-}
-#if 1 || PY_VERSION_HEX < 0x030600B1
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, int nargs, PyObject *kwargs) {
-    PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
-    PyObject *globals = PyFunction_GET_GLOBALS(func);
-    PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
-    PyObject *closure;
-#if PY_MAJOR_VERSION >= 3
-    PyObject *kwdefs;
-#endif
-    PyObject *kwtuple, **k;
-    PyObject **d;
-    Py_ssize_t nd;
-    Py_ssize_t nk;
-    PyObject *result;
-    assert(kwargs == NULL || PyDict_Check(kwargs));
-    nk = kwargs ? PyDict_Size(kwargs) : 0;
-    if (Py_EnterRecursiveCall((char*)" while calling a Python object")) {
-        return NULL;
-    }
-    if (
-#if PY_MAJOR_VERSION >= 3
-            co->co_kwonlyargcount == 0 &&
-#endif
-            likely(kwargs == NULL || nk == 0) &&
-            co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
-        if (argdefs == NULL && co->co_argcount == nargs) {
-            result = __Pyx_PyFunction_FastCallNoKw(co, args, nargs, globals);
-            goto done;
-        }
-        else if (nargs == 0 && argdefs != NULL
-                 && co->co_argcount == Py_SIZE(argdefs)) {
-            /* function called with no arguments, but all parameters have
-               a default value: use default values as arguments .*/
-            args = &PyTuple_GET_ITEM(argdefs, 0);
-            result =__Pyx_PyFunction_FastCallNoKw(co, args, Py_SIZE(argdefs), globals);
-            goto done;
-        }
-    }
-    if (kwargs != NULL) {
-        Py_ssize_t pos, i;
-        kwtuple = PyTuple_New(2 * nk);
-        if (kwtuple == NULL) {
-            result = NULL;
-            goto done;
-        }
-        k = &PyTuple_GET_ITEM(kwtuple, 0);
-        pos = i = 0;
-        while (PyDict_Next(kwargs, &pos, &k[i], &k[i+1])) {
-            Py_INCREF(k[i]);
-            Py_INCREF(k[i+1]);
-            i += 2;
-        }
-        nk = i / 2;
-    }
-    else {
-        kwtuple = NULL;
-        k = NULL;
-    }
-    closure = PyFunction_GET_CLOSURE(func);
-#if PY_MAJOR_VERSION >= 3
-    kwdefs = PyFunction_GET_KW_DEFAULTS(func);
-#endif
-    if (argdefs != NULL) {
-        d = &PyTuple_GET_ITEM(argdefs, 0);
-        nd = Py_SIZE(argdefs);
-    }
-    else {
-        d = NULL;
-        nd = 0;
-    }
-#if PY_MAJOR_VERSION >= 3
-    result = PyEval_EvalCodeEx((PyObject*)co, globals, (PyObject *)NULL,
-                               args, nargs,
-                               k, (int)nk,
-                               d, (int)nd, kwdefs, closure);
-#else
-    result = PyEval_EvalCodeEx(co, globals, (PyObject *)NULL,
-                               args, nargs,
-                               k, (int)nk,
-                               d, (int)nd, closure);
-#endif
-    Py_XDECREF(kwtuple);
-done:
-    Py_LeaveRecursiveCall();
-    return result;
-}
-#endif
-#endif
-
-/* PyObjectCallMethO */
-      #if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
-    PyObject *self, *result;
-    PyCFunction cfunc;
-    cfunc = PyCFunction_GET_FUNCTION(func);
-    self = PyCFunction_GET_SELF(func);
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
-        return NULL;
-    result = cfunc(self, arg);
-    Py_LeaveRecursiveCall();
-    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
-        PyErr_SetString(
-            PyExc_SystemError,
-            "NULL result without error in PyObject_Call");
-    }
-    return result;
-}
-#endif
-
-/* PyObjectCallOneArg */
-      #if CYTHON_COMPILING_IN_CPYTHON
-static PyObject* __Pyx__PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *result;
-    PyObject *args = PyTuple_New(1);
-    if (unlikely(!args)) return NULL;
-    Py_INCREF(arg);
-    PyTuple_SET_ITEM(args, 0, arg);
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
-    return result;
-}
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, &arg, 1);
-    }
-#endif
-    if (likely(PyCFunction_Check(func))) {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-            return __Pyx_PyObject_CallMethO(func, arg);
-#if CYTHON_FAST_PYCCALL
-        } else if (PyCFunction_GET_FLAGS(func) & METH_FASTCALL) {
-            return __Pyx_PyCFunction_FastCall(func, &arg, 1);
+/* TypeImport */
+  #ifndef __PYX_HAVE_RT_ImportType
+#define __PYX_HAVE_RT_ImportType
+static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+{
+    PyObject *result = 0;
+    char warning[200];
+    Py_ssize_t basicsize;
+#ifdef Py_LIMITED_API
+    PyObject *py_basicsize;
 #endif
-        }
+    result = PyObject_GetAttrString(module, class_name);
+    if (!result)
+        goto bad;
+    if (!PyType_Check(result)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s.%.200s is not a type object",
+            module_name, class_name);
+        goto bad;
     }
-    return __Pyx__PyObject_CallOneArg(func, arg);
-}
+#ifndef Py_LIMITED_API
+    basicsize = ((PyTypeObject *)result)->tp_basicsize;
 #else
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *result;
-    PyObject *args = PyTuple_Pack(1, arg);
-    if (unlikely(!args)) return NULL;
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
-    return result;
-}
-#endif
-
-/* DictGetItem */
-      #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
-    PyObject *value;
-    value = PyDict_GetItemWithError(d, key);
-    if (unlikely(!value)) {
-        if (!PyErr_Occurred()) {
-            PyObject* args = PyTuple_Pack(1, key);
-            if (likely(args))
-                PyErr_SetObject(PyExc_KeyError, args);
-            Py_XDECREF(args);
-        }
-        return NULL;
-    }
-    Py_INCREF(value);
-    return value;
-}
-#endif
-
-/* RaiseTooManyValuesToUnpack */
-      static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
-    PyErr_Format(PyExc_ValueError,
-                 "too many values to unpack (expected %" CYTHON_FORMAT_SSIZE_T "d)", expected);
-}
-
-/* RaiseNeedMoreValuesToUnpack */
-      static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index) {
-    PyErr_Format(PyExc_ValueError,
-                 "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
-                 index, (index == 1) ? "" : "s");
-}
-
-/* RaiseNoneIterError */
-      static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-}
-
-/* SaveResetException */
-      #if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    #if PY_VERSION_HEX >= 0x030700A3
-    *type = tstate->exc_state.exc_type;
-    *value = tstate->exc_state.exc_value;
-    *tb = tstate->exc_state.exc_traceback;
-    #else
-    *type = tstate->exc_type;
-    *value = tstate->exc_value;
-    *tb = tstate->exc_traceback;
-    #endif
-    Py_XINCREF(*type);
-    Py_XINCREF(*value);
-    Py_XINCREF(*tb);
-}
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if PY_VERSION_HEX >= 0x030700A3
-    tmp_type = tstate->exc_state.exc_type;
-    tmp_value = tstate->exc_state.exc_value;
-    tmp_tb = tstate->exc_state.exc_traceback;
-    tstate->exc_state.exc_type = type;
-    tstate->exc_state.exc_value = value;
-    tstate->exc_state.exc_traceback = tb;
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = type;
-    tstate->exc_value = value;
-    tstate->exc_traceback = tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-#endif
-
-/* PyErrExceptionMatches */
-      #if CYTHON_FAST_THREAD_STATE
-static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
-    Py_ssize_t i, n;
-    n = PyTuple_GET_SIZE(tuple);
-#if PY_MAJOR_VERSION >= 3
-    for (i=0; i<n; i++) {
-        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
-    }
+    py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
+    if (!py_basicsize)
+        goto bad;
+    basicsize = PyLong_AsSsize_t(py_basicsize);
+    Py_DECREF(py_basicsize);
+    py_basicsize = 0;
+    if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    for (i=0; i<n; i++) {
-        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    if ((size_t)basicsize < size) {
+        PyErr_Format(PyExc_ValueError,
+            "%.200s.%.200s size changed, may indicate binary incompatibility. "
+            "Expected %zd from C header, got %zd from PyObject",
+            module_name, class_name, size, basicsize);
+        goto bad;
     }
-    return 0;
-}
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
-    PyObject *exc_type = tstate->curexc_type;
-    if (exc_type == err) return 1;
-    if (unlikely(!exc_type)) return 0;
-    if (unlikely(PyTuple_Check(err)))
-        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
-    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
-}
-#endif
-
-/* GetException */
-      #if CYTHON_FAST_THREAD_STATE
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb) {
-#endif
-    PyObject *local_type, *local_value, *local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    local_type = tstate->curexc_type;
-    local_value = tstate->curexc_value;
-    local_tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-#else
-    PyErr_Fetch(&local_type, &local_value, &local_tb);
-#endif
-    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
-#if CYTHON_FAST_THREAD_STATE
-    if (unlikely(tstate->curexc_type))
-#else
-    if (unlikely(PyErr_Occurred()))
-#endif
+    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+        PyErr_Format(PyExc_ValueError,
+            "%.200s.%.200s size changed, may indicate binary incompatibility. "
+            "Expected %zd from C header, got %zd from PyObject",
+            module_name, class_name, size, basicsize);
         goto bad;
-    #if PY_MAJOR_VERSION >= 3
-    if (local_tb) {
-        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
-            goto bad;
     }
-    #endif
-    Py_XINCREF(local_tb);
-    Py_XINCREF(local_type);
-    Py_XINCREF(local_value);
-    *type = local_type;
-    *value = local_value;
-    *tb = local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    #if PY_VERSION_HEX >= 0x030700A3
-    tmp_type = tstate->exc_state.exc_type;
-    tmp_value = tstate->exc_state.exc_value;
-    tmp_tb = tstate->exc_state.exc_traceback;
-    tstate->exc_state.exc_type = local_type;
-    tstate->exc_state.exc_value = local_value;
-    tstate->exc_state.exc_traceback = local_tb;
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = local_type;
-    tstate->exc_value = local_value;
-    tstate->exc_traceback = local_tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-#else
-    PyErr_SetExcInfo(local_type, local_value, local_tb);
-#endif
-    return 0;
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+        PyOS_snprintf(warning, sizeof(warning),
+            "%s.%s size changed, may indicate binary incompatibility. "
+            "Expected %zd from C header, got %zd from PyObject",
+            module_name, class_name, size, basicsize);
+        if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
+    }
+    return (PyTypeObject *)result;
 bad:
-    *type = 0;
-    *value = 0;
-    *tb = 0;
-    Py_XDECREF(local_type);
-    Py_XDECREF(local_value);
-    Py_XDECREF(local_tb);
-    return -1;
+    Py_XDECREF(result);
+    return NULL;
 }
+#endif
 
 /* Import */
-        static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
+  static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
     PyObject *empty_list = 0;
     PyObject *module = 0;
     PyObject *global_dict = 0;
     PyObject *empty_dict = 0;
     PyObject *list;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_import;
@@ -7693,15 +6277,15 @@
         goto bad;
     empty_dict = PyDict_New();
     if (!empty_dict)
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
-            if (strchr(__Pyx_MODULE_NAME, '.')) {
+            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
                 module = PyImport_ImportModuleLevelObject(
                     name, global_dict, empty_dict, list, 1);
                 if (!module) {
                     if (!PyErr_ExceptionMatches(PyExc_ImportError))
                         goto bad;
                     PyErr_Clear();
                 }
@@ -7711,15 +6295,15 @@
         #endif
         if (!module) {
             #if PY_MAJOR_VERSION < 3
             PyObject *py_level = PyInt_FromLong(level);
             if (!py_level)
                 goto bad;
             module = PyObject_CallFunctionObjArgs(py_import,
-                name, global_dict, empty_dict, list, py_level, NULL);
+                name, global_dict, empty_dict, list, py_level, (PyObject *)NULL);
             Py_DECREF(py_level);
             #else
             module = PyImport_ImportModuleLevelObject(
                 name, global_dict, empty_dict, list, level);
             #endif
         }
     }
@@ -7729,55 +6313,57 @@
     #endif
     Py_XDECREF(empty_list);
     Py_XDECREF(empty_dict);
     return module;
 }
 
 /* CLineInTraceback */
-        #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
+  #ifndef CYTHON_CLINE_IN_TRACEBACK
+static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
     }
     __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
 #if CYTHON_COMPILING_IN_CPYTHON
     cython_runtime_dict = _PyObject_GetDictPtr(__pyx_cython_runtime);
     if (likely(cython_runtime_dict)) {
-      use_cline = __Pyx_PyDict_GetItemStr(*cython_runtime_dict, __pyx_n_s_cline_in_traceback);
+        __PYX_PY_DICT_LOOKUP_IF_MODIFIED(
+            use_cline, *cython_runtime_dict,
+            __Pyx_PyDict_GetItemStr(*cython_runtime_dict, __pyx_n_s_cline_in_traceback))
     } else
 #endif
     {
       PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
       if (use_cline_obj) {
         use_cline = PyObject_Not(use_cline_obj) ? Py_False : Py_True;
         Py_DECREF(use_cline_obj);
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
-    else if (PyObject_Not(use_cline) != 0) {
+    else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
 #endif
 
 /* CodeObjectCache */
-        static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
+  static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
     int start = 0, mid = 0, end = count - 1;
     if (end >= 0 && code_line > entries[end].code_line) {
         return count;
     }
     while (start < end) {
         mid = start + (end - start) / 2;
         if (code_line < entries[mid].code_line) {
@@ -7832,15 +6418,15 @@
         entries[pos].code_object = code_object;
         Py_DECREF(tmp);
         return;
     }
     if (__pyx_code_cache.count == __pyx_code_cache.max_count) {
         int new_max = __pyx_code_cache.max_count + 64;
         entries = (__Pyx_CodeObjectCacheEntry*)PyMem_Realloc(
-            __pyx_code_cache.entries, (size_t)new_max*sizeof(__Pyx_CodeObjectCacheEntry));
+            __pyx_code_cache.entries, ((size_t)new_max) * sizeof(__Pyx_CodeObjectCacheEntry));
         if (unlikely(!entries)) {
             return;
         }
         __pyx_code_cache.entries = entries;
         __pyx_code_cache.max_count = new_max;
     }
     for (i=__pyx_code_cache.count; i>pos; i--) {
@@ -7849,44 +6435,51 @@
     entries[pos].code_line = code_line;
     entries[pos].code_object = code_object;
     __pyx_code_cache.count++;
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
-        #include "compile.h"
+  #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = 0;
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
+    PyCodeObject *py_code = NULL;
+    PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
+    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    #else
-    py_srcfile = PyUnicode_FromString(filename);
-    #endif
     if (!py_srcfile) goto bad;
+    #endif
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
+        funcname = PyUnicode_AsUTF8(py_funcname);
+        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        #else
-        py_funcname = PyUnicode_FromString(funcname);
+        if (!py_funcname) goto bad;
         #endif
     }
-    if (!py_funcname) goto bad;
+    #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -7897,34 +6490,49 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    Py_DECREF(py_funcname);
+    #else
+    py_code = PyCode_NewEmpty(filename, funcname, py_line);
+    #endif
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
-    Py_XDECREF(py_srcfile);
     Py_XDECREF(py_funcname);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_srcfile);
+    #endif
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -7936,35 +6544,33 @@
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 
 #if PY_MAJOR_VERSION < 3
 static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags) {
     if (PyObject_CheckBuffer(obj)) return PyObject_GetBuffer(obj, view, flags);
-        if (__Pyx_TypeCheck(obj, __pyx_ptype_5numpy_ndarray)) return __pyx_pw_5numpy_7ndarray_1__getbuffer__(obj, view, flags);
     PyErr_Format(PyExc_TypeError, "'%.200s' does not have the buffer interface", Py_TYPE(obj)->tp_name);
     return -1;
 }
 static void __Pyx_ReleaseBuffer(Py_buffer *view) {
     PyObject *obj = view->obj;
     if (!obj) return;
     if (PyObject_CheckBuffer(obj)) {
         PyBuffer_Release(view);
         return;
     }
     if ((0)) {}
-        else if (__Pyx_TypeCheck(obj, __pyx_ptype_5numpy_ndarray)) __pyx_pw_5numpy_7ndarray_3__releasebuffer__(obj, view);
     view->obj = NULL;
     Py_DECREF(obj);
 }
 #endif
 
 
-        /* CIntFromPyVerify */
-        #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
+  /* CIntFromPyVerify */
+  #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
 #define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
 #define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
     {\
         func_type value = func_value;\
         if (sizeof(target_type) < sizeof(func_type)) {\
@@ -7977,78 +6583,16 @@
                 else\
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
-/* CIntToPy */
-        static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-    const long neg_one = (long) -1, const_zero = (long) 0;
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(long) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(long),
-                                     little, !is_unsigned);
-    }
-}
-
-/* CIntToPy */
-        static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-    const int neg_one = (int) -1, const_zero = (int) 0;
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(int) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
-                                     little, !is_unsigned);
-    }
-}
-
 /* Declarations */
-        #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return ::std::complex< float >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return x + y*(__pyx_t_float_complex)_Complex_I;
@@ -8060,15 +6604,15 @@
       z.real = x;
       z.imag = y;
       return z;
     }
 #endif
 
 /* Arithmetic */
-        #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX
 #else
     static CYTHON_INLINE int __Pyx_c_eq_float(__pyx_t_float_complex a, __pyx_t_float_complex b) {
        return (a.real == b.real) && (a.imag == b.imag);
     }
     static CYTHON_INLINE __pyx_t_float_complex __Pyx_c_sum_float(__pyx_t_float_complex a, __pyx_t_float_complex b) {
         __pyx_t_float_complex z;
         z.real = a.real + b.real;
@@ -8092,21 +6636,21 @@
         if (b.imag == 0) {
             return __pyx_t_float_complex_from_parts(a.real / b.real, a.imag / b.real);
         } else if (fabsf(b.real) >= fabsf(b.imag)) {
             if (b.real == 0 && b.imag == 0) {
                 return __pyx_t_float_complex_from_parts(a.real / b.real, a.imag / b.imag);
             } else {
                 float r = b.imag / b.real;
-                float s = 1.0 / (b.real + b.imag * r);
+                float s = (float)(1.0) / (b.real + b.imag * r);
                 return __pyx_t_float_complex_from_parts(
                     (a.real + a.imag * r) * s, (a.imag - a.real * r) * s);
             }
         } else {
             float r = b.real / b.imag;
-            float s = 1.0 / (b.imag + b.real * r);
+            float s = (float)(1.0) / (b.imag + b.real * r);
             return __pyx_t_float_complex_from_parts(
                 (a.real * r + a.imag) * s, (a.imag * r - a.real) * s);
         }
     }
     #else
     static CYTHON_INLINE __pyx_t_float_complex __Pyx_c_quot_float(__pyx_t_float_complex a, __pyx_t_float_complex b) {
         if (b.imag == 0) {
@@ -8156,15 +6700,14 @@
                     case 0:
                         z.real = 1;
                         z.imag = 0;
                         return z;
                     case 1:
                         return a;
                     case 2:
-                        z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(a, a);
                     case 3:
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, a);
                     case 4:
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
@@ -8178,15 +6721,15 @@
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
                     r = -a.real;
-                    theta = atan2f(0, -1);
+                    theta = atan2f(0.0, -1.0);
                 }
             } else {
                 r = __Pyx_c_abs_float(a);
                 theta = atan2f(a.imag, a.real);
             }
             lnr = logf(r);
             z_r = expf(lnr * b.real - theta * b.imag);
@@ -8195,15 +6738,15 @@
             z.imag = z_r * sinf(z_theta);
             return z;
         }
     #endif
 #endif
 
 /* Declarations */
-        #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double x, double y) {
       return ::std::complex< double >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double x, double y) {
       return x + y*(__pyx_t_double_complex)_Complex_I;
@@ -8215,15 +6758,15 @@
       z.real = x;
       z.imag = y;
       return z;
     }
 #endif
 
 /* Arithmetic */
-        #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX
 #else
     static CYTHON_INLINE int __Pyx_c_eq_double(__pyx_t_double_complex a, __pyx_t_double_complex b) {
        return (a.real == b.real) && (a.imag == b.imag);
     }
     static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_sum_double(__pyx_t_double_complex a, __pyx_t_double_complex b) {
         __pyx_t_double_complex z;
         z.real = a.real + b.real;
@@ -8247,21 +6790,21 @@
         if (b.imag == 0) {
             return __pyx_t_double_complex_from_parts(a.real / b.real, a.imag / b.real);
         } else if (fabs(b.real) >= fabs(b.imag)) {
             if (b.real == 0 && b.imag == 0) {
                 return __pyx_t_double_complex_from_parts(a.real / b.real, a.imag / b.imag);
             } else {
                 double r = b.imag / b.real;
-                double s = 1.0 / (b.real + b.imag * r);
+                double s = (double)(1.0) / (b.real + b.imag * r);
                 return __pyx_t_double_complex_from_parts(
                     (a.real + a.imag * r) * s, (a.imag - a.real * r) * s);
             }
         } else {
             double r = b.real / b.imag;
-            double s = 1.0 / (b.imag + b.real * r);
+            double s = (double)(1.0) / (b.imag + b.real * r);
             return __pyx_t_double_complex_from_parts(
                 (a.real * r + a.imag) * s, (a.imag * r - a.real) * s);
         }
     }
     #else
     static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_quot_double(__pyx_t_double_complex a, __pyx_t_double_complex b) {
         if (b.imag == 0) {
@@ -8311,15 +6854,14 @@
                     case 0:
                         z.real = 1;
                         z.imag = 0;
                         return z;
                     case 1:
                         return a;
                     case 2:
-                        z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(a, a);
                     case 3:
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, a);
                     case 4:
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
@@ -8333,15 +6875,15 @@
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
                     r = -a.real;
-                    theta = atan2(0, -1);
+                    theta = atan2(0.0, -1.0);
                 }
             } else {
                 r = __Pyx_c_abs_double(a);
                 theta = atan2(a.imag, a.real);
             }
             lnr = log(r);
             z_r = exp(lnr * b.real - theta * b.imag);
@@ -8349,48 +6891,24 @@
             z.real = z_r * cos(z_theta);
             z.imag = z_r * sin(z_theta);
             return z;
         }
     #endif
 #endif
 
-/* CIntToPy */
-        static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value) {
-    const enum NPY_TYPES neg_one = (enum NPY_TYPES) -1, const_zero = (enum NPY_TYPES) 0;
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(enum NPY_TYPES) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(enum NPY_TYPES) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(enum NPY_TYPES),
-                                     little, !is_unsigned);
-    }
-}
-
 /* CIntFromPy */
-        static CYTHON_INLINE unsigned PY_LONG_LONG __Pyx_PyInt_As_unsigned_PY_LONG_LONG(PyObject *x) {
+  static CYTHON_INLINE unsigned PY_LONG_LONG __Pyx_PyInt_As_unsigned_PY_LONG_LONG(PyObject *x) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
     const unsigned PY_LONG_LONG neg_one = (unsigned PY_LONG_LONG) -1, const_zero = (unsigned PY_LONG_LONG) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(unsigned PY_LONG_LONG) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(unsigned PY_LONG_LONG, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -8570,16 +7088,23 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to unsigned PY_LONG_LONG");
     return (unsigned PY_LONG_LONG) -1;
 }
 
 /* CIntFromPy */
-        static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
+  static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
     const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(int) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -8758,17 +7283,100 @@
     return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
+/* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(long) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(long) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(long),
+                                     little, !is_unsigned);
+    }
+}
+
+/* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+    }
+}
+
 /* CIntFromPy */
-        static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
+  static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
     const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(long) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -8948,15 +7556,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
 /* FastTypeChecks */
-        #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
         a = a->tp_base;
         if (a == b)
             return 1;
     }
     return b == &PyBaseObject_Type;
@@ -9048,114 +7656,53 @@
         return __Pyx_inner_PyErr_GivenExceptionMatches2(err, exc_type1, exc_type2);
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
-        static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+  static int __Pyx_check_binary_version(void) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
-/* ModuleImport */
-        #ifndef __PYX_HAVE_RT_ImportModule
-#define __PYX_HAVE_RT_ImportModule
-static PyObject *__Pyx_ImportModule(const char *name) {
-    PyObject *py_name = 0;
-    PyObject *py_module = 0;
-    py_name = __Pyx_PyIdentifier_FromString(name);
-    if (!py_name)
-        goto bad;
-    py_module = PyImport_Import(py_name);
-    Py_DECREF(py_name);
-    return py_module;
-bad:
-    Py_XDECREF(py_name);
-    return 0;
-}
-#endif
-
-/* TypeImport */
-        #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(const char *module_name, const char *class_name,
-    size_t size, int strict)
-{
-    PyObject *py_module = 0;
-    PyObject *result = 0;
-    PyObject *py_name = 0;
-    char warning[200];
-    Py_ssize_t basicsize;
-#ifdef Py_LIMITED_API
-    PyObject *py_basicsize;
-#endif
-    py_module = __Pyx_ImportModule(module_name);
-    if (!py_module)
-        goto bad;
-    py_name = __Pyx_PyIdentifier_FromString(class_name);
-    if (!py_name)
-        goto bad;
-    result = PyObject_GetAttr(py_module, py_name);
-    Py_DECREF(py_name);
-    py_name = 0;
-    Py_DECREF(py_module);
-    py_module = 0;
-    if (!result)
-        goto bad;
-    if (!PyType_Check(result)) {
-        PyErr_Format(PyExc_TypeError,
-            "%.200s.%.200s is not a type object",
-            module_name, class_name);
-        goto bad;
-    }
-#ifndef Py_LIMITED_API
-    basicsize = ((PyTypeObject *)result)->tp_basicsize;
-#else
-    py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
-    if (!py_basicsize)
-        goto bad;
-    basicsize = PyLong_AsSsize_t(py_basicsize);
-    Py_DECREF(py_basicsize);
-    py_basicsize = 0;
-    if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
-        goto bad;
-#endif
-    if (!strict && (size_t)basicsize > size) {
-        PyOS_snprintf(warning, sizeof(warning),
-            "%s.%s size changed, may indicate binary incompatibility. Expected %zd, got %zd",
-            module_name, class_name, basicsize, size);
-        if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
-    }
-    else if ((size_t)basicsize != size) {
-        PyErr_Format(PyExc_ValueError,
-            "%.200s.%.200s has the wrong size, try recompiling. Expected %zd, got %zd",
-            module_name, class_name, basicsize, size);
-        goto bad;
-    }
-    return (PyTypeObject *)result;
-bad:
-    Py_XDECREF(py_module);
-    Py_XDECREF(result);
-    return NULL;
-}
-#endif
-
 /* InitStrings */
-        static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
+  static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
         #if PY_MAJOR_VERSION < 3
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
         } else if (t->intern) {
             *t->p = PyString_InternFromString(t->s);
         } else {
@@ -9256,14 +7803,21 @@
     }
 }
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject* x) {
    int is_true = x == Py_True;
    if (is_true | (x == Py_False) | (x == Py_None)) return is_true;
    else return PyObject_IsTrue(x);
 }
+static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject* x) {
+    int retval;
+    if (unlikely(!x)) return -1;
+    retval = __Pyx_PyObject_IsTrue(x);
+    Py_DECREF(x);
+    return retval;
+}
 static PyObject* __Pyx_PyNumber_IntOrLongWrongResultType(PyObject* result, const char* type_name) {
 #if PY_MAJOR_VERSION >= 3
     if (PyLong_Check(result)) {
         if (PyErr_WarnFormat(PyExc_DeprecationWarning, 1,
                 "__int__ returned non-int (type %.200s).  "
                 "The ability to return an instance of a strict subclass of int "
                 "is deprecated, and may be removed in a future version of Python.",
@@ -9333,15 +7887,15 @@
   Py_ssize_t ival;
   PyObject *x;
 #if PY_MAJOR_VERSION < 3
   if (likely(PyInt_CheckExact(b))) {
     if (sizeof(Py_ssize_t) >= sizeof(long))
         return PyInt_AS_LONG(b);
     else
-        return PyInt_AsSsize_t(x);
+        return PyInt_AsSsize_t(b);
   }
 #endif
   if (likely(PyLong_CheckExact(b))) {
     #if CYTHON_USE_PYLONG_INTERNALS
     const digit* digits = ((PyLongObject*)b)->ob_digit;
     const Py_ssize_t size = Py_SIZE(b);
     if (likely(__Pyx_sst_abs(size) <= 1)) {
@@ -9387,14 +7941,31 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
+  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
+    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
+#if PY_MAJOR_VERSION < 3
+  } else if (likely(PyInt_CheckExact(o))) {
+    return PyInt_AS_LONG(o);
+#endif
+  } else {
+    Py_ssize_t ival;
+    PyObject *x;
+    x = PyNumber_Index(o);
+    if (!x) return -1;
+    ival = PyInt_AsLong(x);
+    Py_DECREF(x);
+    return ival;
+  }
+}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
```

### Comparing `PyMT64-1.9/README.txt` & `PyMT64-2.0/README.txt`

 * *Files 6% similar despite different names*

```diff
@@ -24,24 +24,25 @@
     0.83320389 0.05085032 0.48682253 0.17667076]
 
 For a complete example, see pymt64_test.py
 
 Note: the state vector 'mt' returned by pymt64.init has 313 elements instead of the 312 elements of the original C code. This is because the 313th element store the associated counter (mti).
 
 Change history:
-1.9 : correct bug associated with the normal distribution
-1.8 : include a missing file
-1.7 : corrected data package contain
-1.6 : correct wrong size of the state vector 
-1.5 : module interface is now based on Cython, module now compatible with python 3
-1.4 : link problem fixed
-1.3 : fixe a compilation problem regading the Numpy include directory
-1.2 : the previous implementation of the poisson distribution was not thread safe
-1.1 : fix a problem with the initialization of the seed  (in the previous version the seed set by init() was not taken into account such that the results were not reproductible)
-1.0 : initial version
+- 2.0 (23/05/2023):  suppress posible occurence of warning message or error due to the declaration of variable of type np.int
+- 1.9 : correct bug associated with the normal distribution
+- 1.8 : include a missing file
+- 1.7 : corrected data package contain
+- 1.6 : correct wrong size of the state vector 
+- 1.5 : module interface is now based on Cython, module now compatible with python 3
+- 1.4 : link problem fixed
+- 1.3 : fixe a compilation problem regading the Numpy include directory
+- 1.2 : the previous implementation of the poisson distribution was not thread safe
+- 1.1 : fix a problem with the initialization of the seed  (in the previous version the seed set by init() was not taken into account such that the results were not reproductible)
+- 1.0 : initial version
 
 
 R. Samadi (LESIA, Observatoire de Paris), 22 Dec. 2012	    
 
 References:
    T. Nishimura, ``Tables of 64-bit Mersenne Twisters''
      ACM Transactions on Modeling and
```

### Comparing `PyMT64-1.9/pymt64_test_mp.py` & `PyMT64-2.0/pymt64_test_mp.py`

 * *Files identical despite different names*

### Comparing `PyMT64-1.9/setup.py` & `PyMT64-2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
               depends  = ['mt64mp.h', 'pymt64lib.h'],
                sources   = ['pymt64.pyx','pymt64lib.c','mt19937-64mp.c'], 
                include_dirs=[numpy.get_include()] )
     ]
 
 
 setup(name = 'PyMT64',
-      version = '1.9',
+      version = '2.0',
       description = 'Python version of the Mersenne Twister 64-bit pseudorandom number generator',
       author = 'R. Samadi',
       author_email = 'reza.samadi@obspm.fr',
       url =  'http://lesia.obspm.fr/',
       long_description = open('README.txt').read(),
       long_description_content_type='text/markdown',
       ext_modules =  cythonize(ext_modules)
```

### Comparing `PyMT64-1.9/mt64mp.h` & `PyMT64-2.0/mt64mp.h`

 * *Files identical despite different names*

### Comparing `PyMT64-1.9/PKG-INFO` & `PyMT64-2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 Metadata-Version: 2.1
 Name: PyMT64
-Version: 1.9
+Version: 2.0
 Summary: Python version of the Mersenne Twister 64-bit pseudorandom number generator
 Home-page: http://lesia.obspm.fr/
 Author: R. Samadi
 Author-email: reza.samadi@obspm.fr
 License: UNKNOWN
-Description: # PyMT64 Package
-        
-                             PyMT64
-                             
-        PyMT64 is a Python version of the Mersenne Twister (MT) 64-bit pseudorandom number generator by Takuji Nishimura and Makoto Matsumoto (see http://www.math.sci.hiroshima-u.ac.jp/~m-mat/MT/emt64.html and the references below).
-        
-        This customised version is thread safe and was interfaced from C to Python (see pymt64.c)
-        
-        This module provides the following methods:
-        - init : initialization of the state vector (mt) used by the pseudorandom number generator (PNG)
-        - uniform : generation of an uniform distribution
-        - normal : generation of two Normal distributions
-        - poisson : generation of a Poisson distribution
-        
-        The period of the PNG is 2**19937-1.
-        
-        Example:
-            import pymt64
-            seed = 143439545 seed # the initial seed
-            mt = pymt64.init(seed) # initialisation of the state vector of MT
-            u = pymt64.uniform(mt,10) # generation of an uniform distribution
-            print (u)
-            [0.12444525 0.22084376 0.31059967 0.45578589 0.84743752 0.28825306
-            0.83320389 0.05085032 0.48682253 0.17667076]
-        
-        For a complete example, see pymt64_test.py
-        
-        Note: the state vector 'mt' returned by pymt64.init has 313 elements instead of the 312 elements of the original C code. This is because the 313th element store the associated counter (mti).
-        
-        Change history:
-        1.9 : correct bug associated with the normal distribution
-        1.8 : include a missing file
-        1.7 : corrected data package contain
-        1.6 : correct wrong size of the state vector 
-        1.5 : module interface is now based on Cython, module now compatible with python 3
-        1.4 : link problem fixed
-        1.3 : fixe a compilation problem regading the Numpy include directory
-        1.2 : the previous implementation of the poisson distribution was not thread safe
-        1.1 : fix a problem with the initialization of the seed  (in the previous version the seed set by init() was not taken into account such that the results were not reproductible)
-        1.0 : initial version
-        
-        
-        R. Samadi (LESIA, Observatoire de Paris), 22 Dec. 2012	    
-        
-        References:
-           T. Nishimura, ``Tables of 64-bit Mersenne Twisters''
-             ACM Transactions on Modeling and 
-             Computer Simulation 10. (2000) 348--357.
-           M. Matsumoto and T. Nishimura,
-             ``Mersenne Twister: a 623-dimensionally equidistributed
-               uniform pseudorandom number generator''
-             ACM Transactions on Modeling and 
-             Computer Simulation 8. (Jan. 1998) 3--30.
-        
-        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+# PyMT64 Package
+
+                     PyMT64
+                     
+PyMT64 is a Python version of the Mersenne Twister (MT) 64-bit pseudorandom number generator by Takuji Nishimura and Makoto Matsumoto (see http://www.math.sci.hiroshima-u.ac.jp/~m-mat/MT/emt64.html and the references below).
+
+This customised version is thread safe and was interfaced from C to Python (see pymt64.c)
+
+This module provides the following methods:
+- init : initialization of the state vector (mt) used by the pseudorandom number generator (PNG)
+- uniform : generation of an uniform distribution
+- normal : generation of two Normal distributions
+- poisson : generation of a Poisson distribution
+
+The period of the PNG is 2**19937-1.
+
+Example:
+    import pymt64
+    seed = 143439545 seed # the initial seed
+    mt = pymt64.init(seed) # initialisation of the state vector of MT
+    u = pymt64.uniform(mt,10) # generation of an uniform distribution
+    print (u)
+    [0.12444525 0.22084376 0.31059967 0.45578589 0.84743752 0.28825306
+    0.83320389 0.05085032 0.48682253 0.17667076]
+
+For a complete example, see pymt64_test.py
+
+Note: the state vector 'mt' returned by pymt64.init has 313 elements instead of the 312 elements of the original C code. This is because the 313th element store the associated counter (mti).
+
+Change history:
+- 2.0 (23/05/2023):  suppress posible occurence of warning message or error due to the declaration of variable of type np.int
+- 1.9 : correct bug associated with the normal distribution
+- 1.8 : include a missing file
+- 1.7 : corrected data package contain
+- 1.6 : correct wrong size of the state vector 
+- 1.5 : module interface is now based on Cython, module now compatible with python 3
+- 1.4 : link problem fixed
+- 1.3 : fixe a compilation problem regading the Numpy include directory
+- 1.2 : the previous implementation of the poisson distribution was not thread safe
+- 1.1 : fix a problem with the initialization of the seed  (in the previous version the seed set by init() was not taken into account such that the results were not reproductible)
+- 1.0 : initial version
+
+
+R. Samadi (LESIA, Observatoire de Paris), 22 Dec. 2012	    
+
+References:
+   T. Nishimura, ``Tables of 64-bit Mersenne Twisters''
+     ACM Transactions on Modeling and 
+     Computer Simulation 10. (2000) 348--357.
+   M. Matsumoto and T. Nishimura,
+     ``Mersenne Twister: a 623-dimensionally equidistributed
+       uniform pseudorandom number generator''
+     ACM Transactions on Modeling and 
+     Computer Simulation 8. (Jan. 1998) 3--30.
+
+
+
```

### Comparing `PyMT64-1.9/PyMT64.egg-info/PKG-INFO` & `PyMT64-2.0/PyMT64.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 Metadata-Version: 2.1
 Name: PyMT64
-Version: 1.9
+Version: 2.0
 Summary: Python version of the Mersenne Twister 64-bit pseudorandom number generator
 Home-page: http://lesia.obspm.fr/
 Author: R. Samadi
 Author-email: reza.samadi@obspm.fr
 License: UNKNOWN
-Description: # PyMT64 Package
-        
-                             PyMT64
-                             
-        PyMT64 is a Python version of the Mersenne Twister (MT) 64-bit pseudorandom number generator by Takuji Nishimura and Makoto Matsumoto (see http://www.math.sci.hiroshima-u.ac.jp/~m-mat/MT/emt64.html and the references below).
-        
-        This customised version is thread safe and was interfaced from C to Python (see pymt64.c)
-        
-        This module provides the following methods:
-        - init : initialization of the state vector (mt) used by the pseudorandom number generator (PNG)
-        - uniform : generation of an uniform distribution
-        - normal : generation of two Normal distributions
-        - poisson : generation of a Poisson distribution
-        
-        The period of the PNG is 2**19937-1.
-        
-        Example:
-            import pymt64
-            seed = 143439545 seed # the initial seed
-            mt = pymt64.init(seed) # initialisation of the state vector of MT
-            u = pymt64.uniform(mt,10) # generation of an uniform distribution
-            print (u)
-            [0.12444525 0.22084376 0.31059967 0.45578589 0.84743752 0.28825306
-            0.83320389 0.05085032 0.48682253 0.17667076]
-        
-        For a complete example, see pymt64_test.py
-        
-        Note: the state vector 'mt' returned by pymt64.init has 313 elements instead of the 312 elements of the original C code. This is because the 313th element store the associated counter (mti).
-        
-        Change history:
-        1.9 : correct bug associated with the normal distribution
-        1.8 : include a missing file
-        1.7 : corrected data package contain
-        1.6 : correct wrong size of the state vector 
-        1.5 : module interface is now based on Cython, module now compatible with python 3
-        1.4 : link problem fixed
-        1.3 : fixe a compilation problem regading the Numpy include directory
-        1.2 : the previous implementation of the poisson distribution was not thread safe
-        1.1 : fix a problem with the initialization of the seed  (in the previous version the seed set by init() was not taken into account such that the results were not reproductible)
-        1.0 : initial version
-        
-        
-        R. Samadi (LESIA, Observatoire de Paris), 22 Dec. 2012	    
-        
-        References:
-           T. Nishimura, ``Tables of 64-bit Mersenne Twisters''
-             ACM Transactions on Modeling and 
-             Computer Simulation 10. (2000) 348--357.
-           M. Matsumoto and T. Nishimura,
-             ``Mersenne Twister: a 623-dimensionally equidistributed
-               uniform pseudorandom number generator''
-             ACM Transactions on Modeling and 
-             Computer Simulation 8. (Jan. 1998) 3--30.
-        
-        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+# PyMT64 Package
+
+                     PyMT64
+                     
+PyMT64 is a Python version of the Mersenne Twister (MT) 64-bit pseudorandom number generator by Takuji Nishimura and Makoto Matsumoto (see http://www.math.sci.hiroshima-u.ac.jp/~m-mat/MT/emt64.html and the references below).
+
+This customised version is thread safe and was interfaced from C to Python (see pymt64.c)
+
+This module provides the following methods:
+- init : initialization of the state vector (mt) used by the pseudorandom number generator (PNG)
+- uniform : generation of an uniform distribution
+- normal : generation of two Normal distributions
+- poisson : generation of a Poisson distribution
+
+The period of the PNG is 2**19937-1.
+
+Example:
+    import pymt64
+    seed = 143439545 seed # the initial seed
+    mt = pymt64.init(seed) # initialisation of the state vector of MT
+    u = pymt64.uniform(mt,10) # generation of an uniform distribution
+    print (u)
+    [0.12444525 0.22084376 0.31059967 0.45578589 0.84743752 0.28825306
+    0.83320389 0.05085032 0.48682253 0.17667076]
+
+For a complete example, see pymt64_test.py
+
+Note: the state vector 'mt' returned by pymt64.init has 313 elements instead of the 312 elements of the original C code. This is because the 313th element store the associated counter (mti).
+
+Change history:
+- 2.0 (23/05/2023):  suppress posible occurence of warning message or error due to the declaration of variable of type np.int
+- 1.9 : correct bug associated with the normal distribution
+- 1.8 : include a missing file
+- 1.7 : corrected data package contain
+- 1.6 : correct wrong size of the state vector 
+- 1.5 : module interface is now based on Cython, module now compatible with python 3
+- 1.4 : link problem fixed
+- 1.3 : fixe a compilation problem regading the Numpy include directory
+- 1.2 : the previous implementation of the poisson distribution was not thread safe
+- 1.1 : fix a problem with the initialization of the seed  (in the previous version the seed set by init() was not taken into account such that the results were not reproductible)
+- 1.0 : initial version
+
+
+R. Samadi (LESIA, Observatoire de Paris), 22 Dec. 2012	    
+
+References:
+   T. Nishimura, ``Tables of 64-bit Mersenne Twisters''
+     ACM Transactions on Modeling and 
+     Computer Simulation 10. (2000) 348--357.
+   M. Matsumoto and T. Nishimura,
+     ``Mersenne Twister: a 623-dimensionally equidistributed
+       uniform pseudorandom number generator''
+     ACM Transactions on Modeling and 
+     Computer Simulation 8. (Jan. 1998) 3--30.
+
+
+
```

### Comparing `PyMT64-1.9/mt19937-64mp.c` & `PyMT64-2.0/mt19937-64mp.c`

 * *Files identical despite different names*

### Comparing `PyMT64-1.9/pymt64_test.py` & `PyMT64-2.0/pymt64_test.py`

 * *Files identical despite different names*

### Comparing `PyMT64-1.9/pymt64lib.c` & `PyMT64-2.0/pymt64lib.c`

 * *Files identical despite different names*

