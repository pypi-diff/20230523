# Comparing `tmp/PyOpenGL-accelerate-3.1.6.tar.gz` & `tmp/PyOpenGL-accelerate-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyOpenGL-accelerate-3.1.6.tar", last modified: Fri Jan  6 04:55:42 2023, max compression
+gzip compressed data, was "PyOpenGL-accelerate-3.1.7.tar", last modified: Tue May 23 03:12:10 2023, max compression
```

## Comparing `PyOpenGL-accelerate-3.1.6.tar` & `PyOpenGL-accelerate-3.1.7.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxr-xr-x   0 mcfletch  (1000) mcfletch  (1000)        0 2023-01-06 04:55:42.684654 PyOpenGL-accelerate-3.1.6/
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)       86 2020-01-04 02:07:10.000000 PyOpenGL-accelerate-3.1.6/MANIFEST.in
-drwxr-xr-x   0 mcfletch  (1000) mcfletch  (1000)        0 2023-01-06 04:55:42.680654 PyOpenGL-accelerate-3.1.6/OpenGL_accelerate/
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)      379 2023-01-06 04:55:32.000000 PyOpenGL-accelerate-3.1.6/OpenGL_accelerate/__init__.py
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)      589 2019-11-25 02:18:31.000000 PyOpenGL-accelerate-3.1.6/OpenGL_accelerate/formathandler.pxd
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)      459 2019-11-25 02:18:31.000000 PyOpenGL-accelerate-3.1.6/OpenGL_accelerate/wrapper.pxd
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)      932 2023-01-06 04:55:42.684654 PyOpenGL-accelerate-3.1.6/PKG-INFO
-drwxr-xr-x   0 mcfletch  (1000) mcfletch  (1000)        0 2023-01-06 04:55:42.680654 PyOpenGL-accelerate-3.1.6/PyOpenGL_accelerate.egg-info/
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)      932 2023-01-06 04:55:42.000000 PyOpenGL-accelerate-3.1.6/PyOpenGL_accelerate.egg-info/PKG-INFO
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)      685 2023-01-06 04:55:42.000000 PyOpenGL-accelerate-3.1.6/PyOpenGL_accelerate.egg-info/SOURCES.txt
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)        1 2023-01-06 04:55:42.000000 PyOpenGL-accelerate-3.1.6/PyOpenGL_accelerate.egg-info/dependency_links.txt
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)       18 2023-01-06 04:55:42.000000 PyOpenGL-accelerate-3.1.6/PyOpenGL_accelerate.egg-info/top_level.txt
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)      141 2019-11-25 02:18:31.000000 PyOpenGL-accelerate-3.1.6/README.txt
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)     1711 2019-11-25 02:18:31.000000 PyOpenGL-accelerate-3.1.6/license.txt
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)       38 2023-01-06 04:55:42.684654 PyOpenGL-accelerate-3.1.6/setup.cfg
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)     4792 2023-01-06 04:52:54.000000 PyOpenGL-accelerate-3.1.6/setup.py
-drwxr-xr-x   0 mcfletch  (1000) mcfletch  (1000)        0 2023-01-06 04:55:42.684654 PyOpenGL-accelerate-3.1.6/src/
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)  1097244 2023-01-06 04:55:32.000000 PyOpenGL-accelerate-3.1.6/src/arraydatatype.c
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)    17886 2022-02-19 22:44:47.000000 PyOpenGL-accelerate-3.1.6/src/arraydatatype.pyx
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)   314406 2023-01-06 04:55:32.000000 PyOpenGL-accelerate-3.1.6/src/buffers_formathandler.c
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)     5906 2019-11-25 02:18:31.000000 PyOpenGL-accelerate-3.1.6/src/buffers_formathandler.pyx
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)   275445 2023-01-06 04:55:32.000000 PyOpenGL-accelerate-3.1.6/src/errorchecker.c
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)     2818 2020-01-04 02:07:10.000000 PyOpenGL-accelerate-3.1.6/src/errorchecker.pyx
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)   299931 2023-01-06 04:55:32.000000 PyOpenGL-accelerate-3.1.6/src/formathandler.c
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)     4318 2019-11-25 02:18:31.000000 PyOpenGL-accelerate-3.1.6/src/formathandler.pyx
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)   265077 2023-01-06 04:55:32.000000 PyOpenGL-accelerate-3.1.6/src/latebind.c
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)     1977 2020-01-04 02:07:10.000000 PyOpenGL-accelerate-3.1.6/src/latebind.pyx
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)   212216 2023-01-06 04:55:32.000000 PyOpenGL-accelerate-3.1.6/src/nones_formathandler.c
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)      946 2019-11-25 02:18:31.000000 PyOpenGL-accelerate-3.1.6/src/nones_formathandler.pyx
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)   450086 2023-01-06 04:55:32.000000 PyOpenGL-accelerate-3.1.6/src/numpy_formathandler.c
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)     9185 2023-01-06 04:10:12.000000 PyOpenGL-accelerate-3.1.6/src/numpy_formathandler.pyx
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)   700322 2023-01-06 04:55:32.000000 PyOpenGL-accelerate-3.1.6/src/vbo.c
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)    15776 2019-11-25 02:18:31.000000 PyOpenGL-accelerate-3.1.6/src/vbo.pyx
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)  1299358 2023-01-06 04:55:32.000000 PyOpenGL-accelerate-3.1.6/src/wrapper.c
--rw-r--r--   0 mcfletch  (1000) mcfletch  (1000)    15715 2022-02-19 22:44:47.000000 PyOpenGL-accelerate-3.1.6/src/wrapper.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:10.619218 PyOpenGL-accelerate-3.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:10.603218 PyOpenGL-accelerate-3.1.7/OpenGL_accelerate/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/OpenGL_accelerate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/OpenGL_accelerate/formathandler.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/OpenGL_accelerate/wrapper.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-23 03:12:10.619218 PyOpenGL-accelerate-3.1.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:10.607218 PyOpenGL-accelerate-3.1.7/PyOpenGL_accelerate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-23 03:12:10.000000 PyOpenGL-accelerate-3.1.7/PyOpenGL_accelerate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-23 03:12:10.000000 PyOpenGL-accelerate-3.1.7/PyOpenGL_accelerate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 03:12:10.000000 PyOpenGL-accelerate-3.1.7/PyOpenGL_accelerate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 03:12:10.000000 PyOpenGL-accelerate-3.1.7/PyOpenGL_accelerate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-23 03:12:10.619218 PyOpenGL-accelerate-3.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:10.619218 PyOpenGL-accelerate-3.1.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)  1112039 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/src/arraydatatype.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17886 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/src/arraydatatype.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   320127 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/src/buffers_formathandler.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/src/buffers_formathandler.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   281180 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/src/errorchecker.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/src/errorchecker.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   305611 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/src/formathandler.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/src/formathandler.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   271955 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/src/latebind.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/src/latebind.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   217894 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/src/nones_formathandler.c
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/src/nones_formathandler.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   459173 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/src/numpy_formathandler.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/src/numpy_formathandler.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   708055 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/src/vbo.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15776 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/src/vbo.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1320708 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/src/wrapper.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15715 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/src/wrapper.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:10.619218 PyOpenGL-accelerate-3.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/tests/test_arraydatatypeaccel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-23 03:11:41.000000 PyOpenGL-accelerate-3.1.7/tests/test_numpyaccel.py
```

### Comparing `PyOpenGL-accelerate-3.1.6/OpenGL_accelerate/formathandler.pxd` & `PyOpenGL-accelerate-3.1.7/OpenGL_accelerate/formathandler.pxd`

 * *Files identical despite different names*

### Comparing `PyOpenGL-accelerate-3.1.6/PKG-INFO` & `PyOpenGL-accelerate-3.1.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 Metadata-Version: 2.1
 Name: PyOpenGL-accelerate
-Version: 3.1.6
+Version: 3.1.7
 Summary: Acceleration code for PyOpenGL
 Home-page: http://pyopengl.sourceforge.net
+Download-URL: http://sourceforge.net/project/showfiles.php?group_id=5988
 Author: Mike C. Fletcher
 Author-email: mcfletch@vrplumber.com
 License: BSD
-Download-URL: http://sourceforge.net/project/showfiles.php?group_id=5988
 Keywords: PyOpenGL,accelerate,Cython
 Platform: Win32
 Platform: Linux
 Platform: OS-X
 Platform: Posix
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Multimedia :: Graphics :: 3D Rendering
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/plain
-
-Acceleration code for PyOpenGL
-
-This set of C (Cython) extensions provides acceleration of common operations
-for slow points in PyOpenGL 3.x
-
-
```

### Comparing `PyOpenGL-accelerate-3.1.6/PyOpenGL_accelerate.egg-info/PKG-INFO` & `PyOpenGL-accelerate-3.1.7/PyOpenGL_accelerate.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 Metadata-Version: 2.1
 Name: PyOpenGL-accelerate
-Version: 3.1.6
+Version: 3.1.7
 Summary: Acceleration code for PyOpenGL
 Home-page: http://pyopengl.sourceforge.net
+Download-URL: http://sourceforge.net/project/showfiles.php?group_id=5988
 Author: Mike C. Fletcher
 Author-email: mcfletch@vrplumber.com
 License: BSD
-Download-URL: http://sourceforge.net/project/showfiles.php?group_id=5988
 Keywords: PyOpenGL,accelerate,Cython
 Platform: Win32
 Platform: Linux
 Platform: OS-X
 Platform: Posix
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Multimedia :: Graphics :: 3D Rendering
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/plain
-
-Acceleration code for PyOpenGL
-
-This set of C (Cython) extensions provides acceleration of common operations
-for slow points in PyOpenGL 3.x
-
-
```

### Comparing `PyOpenGL-accelerate-3.1.6/PyOpenGL_accelerate.egg-info/SOURCES.txt` & `PyOpenGL-accelerate-3.1.7/PyOpenGL_accelerate.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 MANIFEST.in
 README.txt
 license.txt
+pyproject.toml
+setup.cfg
 setup.py
 OpenGL_accelerate/__init__.py
 OpenGL_accelerate/formathandler.pxd
 OpenGL_accelerate/wrapper.pxd
 PyOpenGL_accelerate.egg-info/PKG-INFO
 PyOpenGL_accelerate.egg-info/SOURCES.txt
 PyOpenGL_accelerate.egg-info/dependency_links.txt
@@ -22,8 +24,10 @@
 src/nones_formathandler.c
 src/nones_formathandler.pyx
 src/numpy_formathandler.c
 src/numpy_formathandler.pyx
 src/vbo.c
 src/vbo.pyx
 src/wrapper.c
-src/wrapper.pyx
+src/wrapper.pyx
+tests/test_arraydatatypeaccel.py
+tests/test_numpyaccel.py
```

### Comparing `PyOpenGL-accelerate-3.1.6/license.txt` & `PyOpenGL-accelerate-3.1.7/license.txt`

 * *Files identical despite different names*

### Comparing `PyOpenGL-accelerate-3.1.6/src/arraydatatype.c` & `PyOpenGL-accelerate-3.1.7/src/arraydatatype.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.28 */
+/* Generated by Cython 0.29.32 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_28"
-#define CYTHON_HEX_VERSION 0x001D1CF0
+#define CYTHON_ABI "0_29_32"
+#define CYTHON_HEX_VERSION 0x001D20F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -45,14 +45,15 @@
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
@@ -81,18 +82,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
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
@@ -122,18 +127,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
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
@@ -175,15 +229,15 @@
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 0
   #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
@@ -192,14 +246,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
@@ -643,16 +700,18 @@
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
@@ -1536,14 +1595,20 @@
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
 #if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif // CYTHON_FAST_PYCALL
 #endif
@@ -1709,14 +1774,20 @@
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* ExtTypeTest.proto */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
 
+/* PySequenceContains.proto */
+static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
+    int result = PySequence_Contains(seq, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
 /* CallNextTpDealloc.proto */
 static void __Pyx_call_next_tp_dealloc(PyObject* obj, destructor current_tp_dealloc);
 
 /* CallNextTpTraverse.proto */
 static int __Pyx_call_next_tp_traverse(PyObject* obj, visitproc v, void *a, traverseproc current_tp_traverse);
 
 /* CallNextTpClear.proto */
@@ -1991,43 +2062,43 @@
 static const char __pyx_k_pyx_unpickle_AsArrayTypedSize[] = "__pyx_unpickle_AsArrayTypedSize";
 static const char __pyx_k_pyx_unpickle_AsArrayTypedSizeC[] = "__pyx_unpickle_AsArrayTypedSizeChecked";
 static const char __pyx_k_pyx_unpickle_SizedOutputOrInpu[] = "__pyx_unpickle_SizedOutputOrInput";
 static const char __pyx_k_Did_not_resolve_parameter_index[] = "\"Did not resolve parameter index for %r";
 static const char __pyx_k_OpenGL_accelerate_arraydatatype[] = "OpenGL_accelerate.arraydatatype";
 static const char __pyx_k_Cython_coded_Array_handling_acce[] = "Cython-coded Array-handling accelerator module";
 static const char __pyx_k_Expected_r_byte_array_got_r_byte[] = "Expected %r byte array, got %r byte array";
-static const char __pyx_k_Incompatible_checksums_s_vs_0x56[] = "Incompatible checksums (%s vs 0x5629caa = (arrayIndex, arrayName, arrayType))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0x59[] = "Incompatible checksums (%s vs 0x59d77d2 = (arrayIndex, arrayName, arrayType, typeIndex, typeName))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0x66[] = "Incompatible checksums (%s vs 0x6673075 = (all_output_handlers, match, output_handler, preferredOutput, registry))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0x6c[] = "Incompatible checksums (%s vs 0x6c00339 = (arrayType, name, outIndex, size))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xb4[] = "Incompatible checksums (%s vs 0xb479b8c = (arrayType, index, lookup, name, outIndex, size, specifier))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xb8[] = "Incompatible checksums (%s vs 0xb82c5d3 = (arrayIndex, arrayName, arrayType, size))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xe1[] = "Incompatible checksums (%s vs 0xe120466 = (baseType, handler, typeConstant))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x6673075, 0xb44d830, 0x758d679) = (all_output_handlers, match, output_handler, preferredOutput, registry))";
 static const char __pyx_k_No_array_type_handler_for_type_r[] = "No array-type handler for type %r (value: %s) registered";
 static const char __pyx_k_Unable_to_find_any_output_handle[] = "Unable to find any output handler at all (not even ctypes/numpy ones!)";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_2[] = "Incompatible checksums (0x%x vs (0xe120466, 0xd74a616, 0x8a2112b) = (baseType, handler, typeConstant))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_3[] = "Incompatible checksums (0x%x vs (0x6c00339, 0xf1fc4f9, 0x957c7fd) = (arrayType, name, outIndex, size))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_4[] = "Incompatible checksums (0x%x vs (0xb479b8c, 0xbf26656, 0x3afe09b) = (arrayType, index, lookup, name, outIndex, size, specifier))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_5[] = "Incompatible checksums (0x%x vs (0x59d77d2, 0xf9a536a, 0x88bfae3) = (arrayIndex, arrayName, arrayType, typeIndex, typeName))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_6[] = "Incompatible checksums (0x%x vs (0x5629caa, 0x865d52c, 0xd219003) = (arrayIndex, arrayName, arrayType))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_7[] = "Incompatible checksums (0x%x vs (0xb82c5d3, 0x58e470f, 0xab80fcd) = (arrayIndex, arrayName, arrayType, size))";
 static PyObject *__pyx_n_s_ArrayDatatype;
 static PyObject *__pyx_n_s_AsArrayOfType;
 static PyObject *__pyx_n_s_AsArrayTyped;
 static PyObject *__pyx_n_s_AsArrayTypedSize;
 static PyObject *__pyx_n_s_AsArrayTypedSizeChecked;
 static PyObject *__pyx_n_s_AttributeError;
 static PyObject *__pyx_n_s_DO_OUTPUT;
 static PyObject *__pyx_kp_s_Did_not_resolve_parameter_index;
 static PyObject *__pyx_kp_s_Expected_r_byte_array_got_r_byte;
 static PyObject *__pyx_n_s_FormatHandler;
 static PyObject *__pyx_n_s_GENERIC_OUTPUT_PREFERENCES;
 static PyObject *__pyx_n_s_HandlerRegistry;
 static PyObject *__pyx_n_s_ImportError;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x56;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x59;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x66;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x6c;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xb4;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xb8;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xe1;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_3;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_4;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_5;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_6;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_7;
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_n_s_KeyError;
 static PyObject *__pyx_n_s_NULL;
 static PyObject *__pyx_n_s_NULL_2;
 static PyObject *__pyx_kp_s_No_array_type_handler_for_type_r;
 static PyObject *__pyx_n_s_OpenGL;
 static PyObject *__pyx_n_s_OpenGL__null;
@@ -2227,44 +2298,65 @@
 static PyObject *__pyx_tp_new_17OpenGL_accelerate_13arraydatatype_AsArrayOfType(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_17OpenGL_accelerate_13arraydatatype_AsArrayTyped(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_17OpenGL_accelerate_13arraydatatype_AsArrayTypedSizeChecked(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_17OpenGL_accelerate_13arraydatatype_AsArrayTypedSize(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_get = {0, &__pyx_n_s_get, 0, 0, 0};
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_50;
+static PyObject *__pyx_int_61857947;
 static PyObject *__pyx_int_90348714;
+static PyObject *__pyx_int_93210383;
 static PyObject *__pyx_int_94205906;
 static PyObject *__pyx_int_107425909;
 static PyObject *__pyx_int_113247033;
+static PyObject *__pyx_int_123262585;
+static PyObject *__pyx_int_140891436;
+static PyObject *__pyx_int_143391459;
+static PyObject *__pyx_int_144838955;
+static PyObject *__pyx_int_156747773;
+static PyObject *__pyx_int_179834829;
+static PyObject *__pyx_int_189061168;
 static PyObject *__pyx_int_189242252;
 static PyObject *__pyx_int_193119699;
+static PyObject *__pyx_int_200435286;
+static PyObject *__pyx_int_220303363;
+static PyObject *__pyx_int_225748502;
 static PyObject *__pyx_int_236061798;
+static PyObject *__pyx_int_253740281;
+static PyObject *__pyx_int_261772138;
 static PyObject *__pyx_slice_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
+static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
+static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
+static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_tuple__10;
-static PyObject *__pyx_tuple__12;
-static PyObject *__pyx_tuple__14;
-static PyObject *__pyx_tuple__16;
-static PyObject *__pyx_tuple__18;
-static PyObject *__pyx_tuple__20;
-static PyObject *__pyx_tuple__22;
-static PyObject *__pyx_codeobj__5;
-static PyObject *__pyx_codeobj__7;
-static PyObject *__pyx_codeobj__9;
-static PyObject *__pyx_codeobj__11;
-static PyObject *__pyx_codeobj__13;
-static PyObject *__pyx_codeobj__15;
-static PyObject *__pyx_codeobj__17;
-static PyObject *__pyx_codeobj__19;
-static PyObject *__pyx_codeobj__21;
-static PyObject *__pyx_codeobj__23;
+static PyObject *__pyx_tuple__11;
+static PyObject *__pyx_tuple__13;
+static PyObject *__pyx_tuple__15;
+static PyObject *__pyx_tuple__17;
+static PyObject *__pyx_tuple__19;
+static PyObject *__pyx_tuple__21;
+static PyObject *__pyx_tuple__23;
+static PyObject *__pyx_tuple__25;
+static PyObject *__pyx_tuple__27;
+static PyObject *__pyx_tuple__29;
+static PyObject *__pyx_codeobj__12;
+static PyObject *__pyx_codeobj__14;
+static PyObject *__pyx_codeobj__16;
+static PyObject *__pyx_codeobj__18;
+static PyObject *__pyx_codeobj__20;
+static PyObject *__pyx_codeobj__22;
+static PyObject *__pyx_codeobj__24;
+static PyObject *__pyx_codeobj__26;
+static PyObject *__pyx_codeobj__28;
+static PyObject *__pyx_codeobj__30;
 /* Late includes */
 
 /* "src/arraydatatype.pyx":21
  *     GENERIC_OUTPUT_PREFERENCES = ['numpy','ctypesarrays']
  *     cdef object all_output_handlers
  *     def __init__( self, plugin_match ):             # <<<<<<<<<<<<<<
  *         self.registry = {}
@@ -4470,15 +4562,15 @@
  *         """Initialize, grabbing our handler registry"""
  *         self.typeConstant = typeConstant
  */
 
 /* Python wrapper */
 static int __pyx_pw_17OpenGL_accelerate_13arraydatatype_13ArrayDatatype_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_17OpenGL_accelerate_13arraydatatype_13ArrayDatatype___init__[] = "Initialize, grabbing our handler registry";
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_17OpenGL_accelerate_13arraydatatype_13ArrayDatatype___init__;
 #endif
 static int __pyx_pw_17OpenGL_accelerate_13arraydatatype_13ArrayDatatype_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_typeConstant = 0;
   PyObject *__pyx_v_baseType = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -4992,15 +5084,15 @@
  *         """We cannot simply reference from_param as under Python 2.7 that makes us non-callable"""
  *         return self.from_param( value )
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_17OpenGL_accelerate_13arraydatatype_13ArrayDatatype_9__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_17OpenGL_accelerate_13arraydatatype_13ArrayDatatype_8__call__[] = "We cannot simply reference from_param as under Python 2.7 that makes us non-callable";
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_17OpenGL_accelerate_13arraydatatype_13ArrayDatatype_8__call__;
 #endif
 static PyObject *__pyx_pw_17OpenGL_accelerate_13arraydatatype_13ArrayDatatype_9__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_value = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -14583,151 +14675,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_13arraydatatype___pyx_unpickle_HandlerRegistry(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_HandlerRegistry", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x6673075:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x6673075, 0xb44d830, 0x758d679):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6673075 = (all_output_handlers, match, output_handler, preferredOutput, registry))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6673075, 0xb44d830, 0x758d679) = (all_output_handlers, match, output_handler, preferredOutput, registry))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x6673075) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__4, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x6673075:
+ *     if __pyx_checksum not in (0x6673075, 0xb44d830, 0x758d679):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6673075 = (all_output_handlers, match, output_handler, preferredOutput, registry))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6673075, 0xb44d830, 0x758d679) = (all_output_handlers, match, output_handler, preferredOutput, registry))" % __pyx_checksum)
  *     __pyx_result = HandlerRegistry.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x6673075:
+ *     if __pyx_checksum not in (0x6673075, 0xb44d830, 0x758d679):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6673075 = (all_output_handlers, match, output_handler, preferredOutput, registry))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6673075, 0xb44d830, 0x758d679) = (all_output_handlers, match, output_handler, preferredOutput, registry))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = HandlerRegistry.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x66, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x6673075:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x6673075, 0xb44d830, 0x758d679):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6673075 = (all_output_handlers, match, output_handler, preferredOutput, registry))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6673075, 0xb44d830, 0x758d679) = (all_output_handlers, match, output_handler, preferredOutput, registry))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6673075 = (all_output_handlers, match, output_handler, preferredOutput, registry))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6673075, 0xb44d830, 0x758d679) = (all_output_handlers, match, output_handler, preferredOutput, registry))" % __pyx_checksum)
  *     __pyx_result = HandlerRegistry.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_HandlerRegistry__set_state(<HandlerRegistry> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13arraydatatype_HandlerRegistry), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13arraydatatype_HandlerRegistry), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6673075 = (all_output_handlers, match, output_handler, preferredOutput, registry))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6673075, 0xb44d830, 0x758d679) = (all_output_handlers, match, output_handler, preferredOutput, registry))" % __pyx_checksum)
  *     __pyx_result = HandlerRegistry.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_HandlerRegistry__set_state(<HandlerRegistry> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = HandlerRegistry.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_HandlerRegistry__set_state(<HandlerRegistry> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_HandlerRegistry__set_state(HandlerRegistry __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_13arraydatatype___pyx_unpickle_HandlerRegistry__set_state(((struct __pyx_obj_17OpenGL_accelerate_13arraydatatype_HandlerRegistry *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_13arraydatatype___pyx_unpickle_HandlerRegistry__set_state(((struct __pyx_obj_17OpenGL_accelerate_13arraydatatype_HandlerRegistry *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6673075 = (all_output_handlers, match, output_handler, preferredOutput, registry))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6673075, 0xb44d830, 0x758d679) = (all_output_handlers, match, output_handler, preferredOutput, registry))" % __pyx_checksum)
  *     __pyx_result = HandlerRegistry.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_HandlerRegistry__set_state(<HandlerRegistry> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -14747,18 +14843,18 @@
  * def __pyx_unpickle_HandlerRegistry(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.arraydatatype.__pyx_unpickle_HandlerRegistry", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -15025,151 +15121,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_13arraydatatype_2__pyx_unpickle_ArrayDatatype(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_ArrayDatatype", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe120466:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xe120466, 0xd74a616, 0x8a2112b):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe120466 = (baseType, handler, typeConstant))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe120466, 0xd74a616, 0x8a2112b) = (baseType, handler, typeConstant))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xe120466) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__5, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe120466:
+ *     if __pyx_checksum not in (0xe120466, 0xd74a616, 0x8a2112b):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe120466 = (baseType, handler, typeConstant))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe120466, 0xd74a616, 0x8a2112b) = (baseType, handler, typeConstant))" % __pyx_checksum)
  *     __pyx_result = ArrayDatatype.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xe120466:
+ *     if __pyx_checksum not in (0xe120466, 0xd74a616, 0x8a2112b):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe120466 = (baseType, handler, typeConstant))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe120466, 0xd74a616, 0x8a2112b) = (baseType, handler, typeConstant))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = ArrayDatatype.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xe1, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe120466:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xe120466, 0xd74a616, 0x8a2112b):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe120466 = (baseType, handler, typeConstant))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe120466, 0xd74a616, 0x8a2112b) = (baseType, handler, typeConstant))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe120466 = (baseType, handler, typeConstant))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe120466, 0xd74a616, 0x8a2112b) = (baseType, handler, typeConstant))" % __pyx_checksum)
  *     __pyx_result = ArrayDatatype.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_ArrayDatatype__set_state(<ArrayDatatype> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13arraydatatype_ArrayDatatype), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13arraydatatype_ArrayDatatype), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe120466 = (baseType, handler, typeConstant))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe120466, 0xd74a616, 0x8a2112b) = (baseType, handler, typeConstant))" % __pyx_checksum)
  *     __pyx_result = ArrayDatatype.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_ArrayDatatype__set_state(<ArrayDatatype> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = ArrayDatatype.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_ArrayDatatype__set_state(<ArrayDatatype> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_ArrayDatatype__set_state(ArrayDatatype __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_13arraydatatype___pyx_unpickle_ArrayDatatype__set_state(((struct __pyx_obj_17OpenGL_accelerate_13arraydatatype_ArrayDatatype *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_13arraydatatype___pyx_unpickle_ArrayDatatype__set_state(((struct __pyx_obj_17OpenGL_accelerate_13arraydatatype_ArrayDatatype *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe120466 = (baseType, handler, typeConstant))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe120466, 0xd74a616, 0x8a2112b) = (baseType, handler, typeConstant))" % __pyx_checksum)
  *     __pyx_result = ArrayDatatype.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_ArrayDatatype__set_state(<ArrayDatatype> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -15189,18 +15289,18 @@
  * def __pyx_unpickle_ArrayDatatype(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.arraydatatype.__pyx_unpickle_ArrayDatatype", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -15445,151 +15545,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_13arraydatatype_4__pyx_unpickle_Output(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_Output", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x6c00339:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x6c00339, 0xf1fc4f9, 0x957c7fd):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6c00339 = (arrayType, name, outIndex, size))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6c00339, 0xf1fc4f9, 0x957c7fd) = (arrayType, name, outIndex, size))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x6c00339) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__6, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x6c00339:
+ *     if __pyx_checksum not in (0x6c00339, 0xf1fc4f9, 0x957c7fd):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6c00339 = (arrayType, name, outIndex, size))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6c00339, 0xf1fc4f9, 0x957c7fd) = (arrayType, name, outIndex, size))" % __pyx_checksum)
  *     __pyx_result = Output.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x6c00339:
+ *     if __pyx_checksum not in (0x6c00339, 0xf1fc4f9, 0x957c7fd):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6c00339 = (arrayType, name, outIndex, size))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6c00339, 0xf1fc4f9, 0x957c7fd) = (arrayType, name, outIndex, size))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = Output.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x6c, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x6c00339:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x6c00339, 0xf1fc4f9, 0x957c7fd):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6c00339 = (arrayType, name, outIndex, size))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6c00339, 0xf1fc4f9, 0x957c7fd) = (arrayType, name, outIndex, size))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6c00339 = (arrayType, name, outIndex, size))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6c00339, 0xf1fc4f9, 0x957c7fd) = (arrayType, name, outIndex, size))" % __pyx_checksum)
  *     __pyx_result = Output.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Output__set_state(<Output> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13arraydatatype_Output), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13arraydatatype_Output), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6c00339 = (arrayType, name, outIndex, size))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6c00339, 0xf1fc4f9, 0x957c7fd) = (arrayType, name, outIndex, size))" % __pyx_checksum)
  *     __pyx_result = Output.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Output__set_state(<Output> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = Output.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Output__set_state(<Output> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Output__set_state(Output __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_13arraydatatype___pyx_unpickle_Output__set_state(((struct __pyx_obj_17OpenGL_accelerate_13arraydatatype_Output *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_13arraydatatype___pyx_unpickle_Output__set_state(((struct __pyx_obj_17OpenGL_accelerate_13arraydatatype_Output *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6c00339 = (arrayType, name, outIndex, size))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6c00339, 0xf1fc4f9, 0x957c7fd) = (arrayType, name, outIndex, size))" % __pyx_checksum)
  *     __pyx_result = Output.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Output__set_state(<Output> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -15609,18 +15713,18 @@
  * def __pyx_unpickle_Output(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.arraydatatype.__pyx_unpickle_Output", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -15877,151 +15981,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_13arraydatatype_6__pyx_unpickle_OutputOrInput(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_OutputOrInput", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x6c00339:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x6c00339, 0xf1fc4f9, 0x957c7fd):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6c00339 = (arrayType, name, outIndex, size))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6c00339, 0xf1fc4f9, 0x957c7fd) = (arrayType, name, outIndex, size))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x6c00339) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__6, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x6c00339:
+ *     if __pyx_checksum not in (0x6c00339, 0xf1fc4f9, 0x957c7fd):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6c00339 = (arrayType, name, outIndex, size))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6c00339, 0xf1fc4f9, 0x957c7fd) = (arrayType, name, outIndex, size))" % __pyx_checksum)
  *     __pyx_result = OutputOrInput.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x6c00339:
+ *     if __pyx_checksum not in (0x6c00339, 0xf1fc4f9, 0x957c7fd):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6c00339 = (arrayType, name, outIndex, size))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6c00339, 0xf1fc4f9, 0x957c7fd) = (arrayType, name, outIndex, size))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = OutputOrInput.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x6c, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x6c00339:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x6c00339, 0xf1fc4f9, 0x957c7fd):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6c00339 = (arrayType, name, outIndex, size))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6c00339, 0xf1fc4f9, 0x957c7fd) = (arrayType, name, outIndex, size))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6c00339 = (arrayType, name, outIndex, size))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6c00339, 0xf1fc4f9, 0x957c7fd) = (arrayType, name, outIndex, size))" % __pyx_checksum)
  *     __pyx_result = OutputOrInput.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_OutputOrInput__set_state(<OutputOrInput> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13arraydatatype_OutputOrInput), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13arraydatatype_OutputOrInput), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6c00339 = (arrayType, name, outIndex, size))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6c00339, 0xf1fc4f9, 0x957c7fd) = (arrayType, name, outIndex, size))" % __pyx_checksum)
  *     __pyx_result = OutputOrInput.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_OutputOrInput__set_state(<OutputOrInput> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = OutputOrInput.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_OutputOrInput__set_state(<OutputOrInput> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_OutputOrInput__set_state(OutputOrInput __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_13arraydatatype___pyx_unpickle_OutputOrInput__set_state(((struct __pyx_obj_17OpenGL_accelerate_13arraydatatype_OutputOrInput *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_13arraydatatype___pyx_unpickle_OutputOrInput__set_state(((struct __pyx_obj_17OpenGL_accelerate_13arraydatatype_OutputOrInput *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6c00339 = (arrayType, name, outIndex, size))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6c00339, 0xf1fc4f9, 0x957c7fd) = (arrayType, name, outIndex, size))" % __pyx_checksum)
  *     __pyx_result = OutputOrInput.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_OutputOrInput__set_state(<OutputOrInput> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -16041,18 +16149,18 @@
  * def __pyx_unpickle_OutputOrInput(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.arraydatatype.__pyx_unpickle_OutputOrInput", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -16309,151 +16417,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_13arraydatatype_8__pyx_unpickle_SizedOutput(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_SizedOutput", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xb479b8c:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xb479b8c, 0xbf26656, 0x3afe09b):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb479b8c = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb479b8c, 0xbf26656, 0x3afe09b) = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xb479b8c) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__7, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xb479b8c:
+ *     if __pyx_checksum not in (0xb479b8c, 0xbf26656, 0x3afe09b):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb479b8c = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb479b8c, 0xbf26656, 0x3afe09b) = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
  *     __pyx_result = SizedOutput.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xb479b8c:
+ *     if __pyx_checksum not in (0xb479b8c, 0xbf26656, 0x3afe09b):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb479b8c = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb479b8c, 0xbf26656, 0x3afe09b) = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = SizedOutput.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xb4, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_4, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xb479b8c:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xb479b8c, 0xbf26656, 0x3afe09b):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb479b8c = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb479b8c, 0xbf26656, 0x3afe09b) = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb479b8c = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb479b8c, 0xbf26656, 0x3afe09b) = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
  *     __pyx_result = SizedOutput.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_SizedOutput__set_state(<SizedOutput> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13arraydatatype_SizedOutput), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13arraydatatype_SizedOutput), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb479b8c = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb479b8c, 0xbf26656, 0x3afe09b) = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
  *     __pyx_result = SizedOutput.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_SizedOutput__set_state(<SizedOutput> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = SizedOutput.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_SizedOutput__set_state(<SizedOutput> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_SizedOutput__set_state(SizedOutput __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_13arraydatatype___pyx_unpickle_SizedOutput__set_state(((struct __pyx_obj_17OpenGL_accelerate_13arraydatatype_SizedOutput *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_13arraydatatype___pyx_unpickle_SizedOutput__set_state(((struct __pyx_obj_17OpenGL_accelerate_13arraydatatype_SizedOutput *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb479b8c = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb479b8c, 0xbf26656, 0x3afe09b) = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
  *     __pyx_result = SizedOutput.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_SizedOutput__set_state(<SizedOutput> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -16473,18 +16585,18 @@
  * def __pyx_unpickle_SizedOutput(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.arraydatatype.__pyx_unpickle_SizedOutput", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -16773,151 +16885,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_13arraydatatype_10__pyx_unpickle_SizedOutputOrInput(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_SizedOutputOrInput", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xb479b8c:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xb479b8c, 0xbf26656, 0x3afe09b):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb479b8c = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb479b8c, 0xbf26656, 0x3afe09b) = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xb479b8c) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__7, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xb479b8c:
+ *     if __pyx_checksum not in (0xb479b8c, 0xbf26656, 0x3afe09b):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb479b8c = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb479b8c, 0xbf26656, 0x3afe09b) = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
  *     __pyx_result = SizedOutputOrInput.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xb479b8c:
+ *     if __pyx_checksum not in (0xb479b8c, 0xbf26656, 0x3afe09b):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb479b8c = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb479b8c, 0xbf26656, 0x3afe09b) = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = SizedOutputOrInput.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xb4, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_4, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xb479b8c:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xb479b8c, 0xbf26656, 0x3afe09b):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb479b8c = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb479b8c, 0xbf26656, 0x3afe09b) = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb479b8c = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb479b8c, 0xbf26656, 0x3afe09b) = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
  *     __pyx_result = SizedOutputOrInput.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_SizedOutputOrInput__set_state(<SizedOutputOrInput> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13arraydatatype_SizedOutputOrInput), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13arraydatatype_SizedOutputOrInput), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb479b8c = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb479b8c, 0xbf26656, 0x3afe09b) = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
  *     __pyx_result = SizedOutputOrInput.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_SizedOutputOrInput__set_state(<SizedOutputOrInput> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = SizedOutputOrInput.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_SizedOutputOrInput__set_state(<SizedOutputOrInput> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_SizedOutputOrInput__set_state(SizedOutputOrInput __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_13arraydatatype___pyx_unpickle_SizedOutputOrInput__set_state(((struct __pyx_obj_17OpenGL_accelerate_13arraydatatype_SizedOutputOrInput *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_13arraydatatype___pyx_unpickle_SizedOutputOrInput__set_state(((struct __pyx_obj_17OpenGL_accelerate_13arraydatatype_SizedOutputOrInput *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb479b8c = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb479b8c, 0xbf26656, 0x3afe09b) = (arrayType, index, lookup, name, outIndex, size, specifier))" % __pyx_checksum)
  *     __pyx_result = SizedOutputOrInput.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_SizedOutputOrInput__set_state(<SizedOutputOrInput> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -16937,18 +17053,18 @@
  * def __pyx_unpickle_SizedOutputOrInput(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.arraydatatype.__pyx_unpickle_SizedOutputOrInput", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -17237,151 +17353,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_13arraydatatype_12__pyx_unpickle_AsArrayOfType(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_AsArrayOfType", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x59d77d2:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x59d77d2, 0xf9a536a, 0x88bfae3):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x59d77d2 = (arrayIndex, arrayName, arrayType, typeIndex, typeName))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x59d77d2, 0xf9a536a, 0x88bfae3) = (arrayIndex, arrayName, arrayType, typeIndex, typeName))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x59d77d2) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__8, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x59d77d2:
+ *     if __pyx_checksum not in (0x59d77d2, 0xf9a536a, 0x88bfae3):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x59d77d2 = (arrayIndex, arrayName, arrayType, typeIndex, typeName))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x59d77d2, 0xf9a536a, 0x88bfae3) = (arrayIndex, arrayName, arrayType, typeIndex, typeName))" % __pyx_checksum)
  *     __pyx_result = AsArrayOfType.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x59d77d2:
+ *     if __pyx_checksum not in (0x59d77d2, 0xf9a536a, 0x88bfae3):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x59d77d2 = (arrayIndex, arrayName, arrayType, typeIndex, typeName))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x59d77d2, 0xf9a536a, 0x88bfae3) = (arrayIndex, arrayName, arrayType, typeIndex, typeName))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = AsArrayOfType.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x59, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_5, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x59d77d2:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x59d77d2, 0xf9a536a, 0x88bfae3):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x59d77d2 = (arrayIndex, arrayName, arrayType, typeIndex, typeName))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x59d77d2, 0xf9a536a, 0x88bfae3) = (arrayIndex, arrayName, arrayType, typeIndex, typeName))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x59d77d2 = (arrayIndex, arrayName, arrayType, typeIndex, typeName))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x59d77d2, 0xf9a536a, 0x88bfae3) = (arrayIndex, arrayName, arrayType, typeIndex, typeName))" % __pyx_checksum)
  *     __pyx_result = AsArrayOfType.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_AsArrayOfType__set_state(<AsArrayOfType> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13arraydatatype_AsArrayOfType), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13arraydatatype_AsArrayOfType), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x59d77d2 = (arrayIndex, arrayName, arrayType, typeIndex, typeName))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x59d77d2, 0xf9a536a, 0x88bfae3) = (arrayIndex, arrayName, arrayType, typeIndex, typeName))" % __pyx_checksum)
  *     __pyx_result = AsArrayOfType.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_AsArrayOfType__set_state(<AsArrayOfType> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = AsArrayOfType.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_AsArrayOfType__set_state(<AsArrayOfType> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_AsArrayOfType__set_state(AsArrayOfType __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_13arraydatatype___pyx_unpickle_AsArrayOfType__set_state(((struct __pyx_obj_17OpenGL_accelerate_13arraydatatype_AsArrayOfType *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_13arraydatatype___pyx_unpickle_AsArrayOfType__set_state(((struct __pyx_obj_17OpenGL_accelerate_13arraydatatype_AsArrayOfType *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x59d77d2 = (arrayIndex, arrayName, arrayType, typeIndex, typeName))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x59d77d2, 0xf9a536a, 0x88bfae3) = (arrayIndex, arrayName, arrayType, typeIndex, typeName))" % __pyx_checksum)
  *     __pyx_result = AsArrayOfType.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_AsArrayOfType__set_state(<AsArrayOfType> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -17401,18 +17521,18 @@
  * def __pyx_unpickle_AsArrayOfType(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.arraydatatype.__pyx_unpickle_AsArrayOfType", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -17678,151 +17798,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_13arraydatatype_14__pyx_unpickle_AsArrayTyped(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_AsArrayTyped", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x5629caa:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x5629caa, 0x865d52c, 0xd219003):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x5629caa = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x5629caa, 0x865d52c, 0xd219003) = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x5629caa) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__9, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x5629caa:
+ *     if __pyx_checksum not in (0x5629caa, 0x865d52c, 0xd219003):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x5629caa = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x5629caa, 0x865d52c, 0xd219003) = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
  *     __pyx_result = AsArrayTyped.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x5629caa:
+ *     if __pyx_checksum not in (0x5629caa, 0x865d52c, 0xd219003):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x5629caa = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x5629caa, 0x865d52c, 0xd219003) = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = AsArrayTyped.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x56, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_6, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x5629caa:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x5629caa, 0x865d52c, 0xd219003):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x5629caa = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x5629caa, 0x865d52c, 0xd219003) = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x5629caa = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x5629caa, 0x865d52c, 0xd219003) = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
  *     __pyx_result = AsArrayTyped.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_AsArrayTyped__set_state(<AsArrayTyped> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13arraydatatype_AsArrayTyped), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13arraydatatype_AsArrayTyped), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x5629caa = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x5629caa, 0x865d52c, 0xd219003) = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
  *     __pyx_result = AsArrayTyped.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_AsArrayTyped__set_state(<AsArrayTyped> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = AsArrayTyped.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_AsArrayTyped__set_state(<AsArrayTyped> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_AsArrayTyped__set_state(AsArrayTyped __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_13arraydatatype___pyx_unpickle_AsArrayTyped__set_state(((struct __pyx_obj_17OpenGL_accelerate_13arraydatatype_AsArrayTyped *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_13arraydatatype___pyx_unpickle_AsArrayTyped__set_state(((struct __pyx_obj_17OpenGL_accelerate_13arraydatatype_AsArrayTyped *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x5629caa = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x5629caa, 0x865d52c, 0xd219003) = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
  *     __pyx_result = AsArrayTyped.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_AsArrayTyped__set_state(<AsArrayTyped> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -17842,18 +17966,18 @@
  * def __pyx_unpickle_AsArrayTyped(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.arraydatatype.__pyx_unpickle_AsArrayTyped", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -18098,151 +18222,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_13arraydatatype_16__pyx_unpickle_AsArrayTypedSizeChecked(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_AsArrayTypedSizeChecked", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xb82c5d3:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xb82c5d3, 0x58e470f, 0xab80fcd):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb82c5d3 = (arrayIndex, arrayName, arrayType, size))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb82c5d3, 0x58e470f, 0xab80fcd) = (arrayIndex, arrayName, arrayType, size))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xb82c5d3) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__10, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xb82c5d3:
+ *     if __pyx_checksum not in (0xb82c5d3, 0x58e470f, 0xab80fcd):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb82c5d3 = (arrayIndex, arrayName, arrayType, size))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb82c5d3, 0x58e470f, 0xab80fcd) = (arrayIndex, arrayName, arrayType, size))" % __pyx_checksum)
  *     __pyx_result = AsArrayTypedSizeChecked.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xb82c5d3:
+ *     if __pyx_checksum not in (0xb82c5d3, 0x58e470f, 0xab80fcd):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb82c5d3 = (arrayIndex, arrayName, arrayType, size))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb82c5d3, 0x58e470f, 0xab80fcd) = (arrayIndex, arrayName, arrayType, size))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = AsArrayTypedSizeChecked.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xb8, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_7, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xb82c5d3:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xb82c5d3, 0x58e470f, 0xab80fcd):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb82c5d3 = (arrayIndex, arrayName, arrayType, size))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb82c5d3, 0x58e470f, 0xab80fcd) = (arrayIndex, arrayName, arrayType, size))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb82c5d3 = (arrayIndex, arrayName, arrayType, size))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb82c5d3, 0x58e470f, 0xab80fcd) = (arrayIndex, arrayName, arrayType, size))" % __pyx_checksum)
  *     __pyx_result = AsArrayTypedSizeChecked.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_AsArrayTypedSizeChecked__set_state(<AsArrayTypedSizeChecked> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13arraydatatype_AsArrayTypedSizeChecked), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13arraydatatype_AsArrayTypedSizeChecked), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb82c5d3 = (arrayIndex, arrayName, arrayType, size))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb82c5d3, 0x58e470f, 0xab80fcd) = (arrayIndex, arrayName, arrayType, size))" % __pyx_checksum)
  *     __pyx_result = AsArrayTypedSizeChecked.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_AsArrayTypedSizeChecked__set_state(<AsArrayTypedSizeChecked> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = AsArrayTypedSizeChecked.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_AsArrayTypedSizeChecked__set_state(<AsArrayTypedSizeChecked> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_AsArrayTypedSizeChecked__set_state(AsArrayTypedSizeChecked __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_13arraydatatype___pyx_unpickle_AsArrayTypedSizeChecked__set_state(((struct __pyx_obj_17OpenGL_accelerate_13arraydatatype_AsArrayTypedSizeChecked *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_13arraydatatype___pyx_unpickle_AsArrayTypedSizeChecked__set_state(((struct __pyx_obj_17OpenGL_accelerate_13arraydatatype_AsArrayTypedSizeChecked *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb82c5d3 = (arrayIndex, arrayName, arrayType, size))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb82c5d3, 0x58e470f, 0xab80fcd) = (arrayIndex, arrayName, arrayType, size))" % __pyx_checksum)
  *     __pyx_result = AsArrayTypedSizeChecked.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_AsArrayTypedSizeChecked__set_state(<AsArrayTypedSizeChecked> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -18262,18 +18390,18 @@
  * def __pyx_unpickle_AsArrayTypedSizeChecked(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.arraydatatype.__pyx_unpickle_AsArrayTypedSizeChecked", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -18527,151 +18655,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_13arraydatatype_18__pyx_unpickle_AsArrayTypedSize(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_AsArrayTypedSize", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x5629caa:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x5629caa, 0x865d52c, 0xd219003):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x5629caa = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x5629caa, 0x865d52c, 0xd219003) = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x5629caa) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__9, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x5629caa:
+ *     if __pyx_checksum not in (0x5629caa, 0x865d52c, 0xd219003):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x5629caa = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x5629caa, 0x865d52c, 0xd219003) = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
  *     __pyx_result = AsArrayTypedSize.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x5629caa:
+ *     if __pyx_checksum not in (0x5629caa, 0x865d52c, 0xd219003):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x5629caa = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x5629caa, 0x865d52c, 0xd219003) = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = AsArrayTypedSize.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x56, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_6, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x5629caa:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x5629caa, 0x865d52c, 0xd219003):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x5629caa = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x5629caa, 0x865d52c, 0xd219003) = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x5629caa = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x5629caa, 0x865d52c, 0xd219003) = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
  *     __pyx_result = AsArrayTypedSize.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_AsArrayTypedSize__set_state(<AsArrayTypedSize> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13arraydatatype_AsArrayTypedSize), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13arraydatatype_AsArrayTypedSize), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x5629caa = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x5629caa, 0x865d52c, 0xd219003) = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
  *     __pyx_result = AsArrayTypedSize.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_AsArrayTypedSize__set_state(<AsArrayTypedSize> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = AsArrayTypedSize.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_AsArrayTypedSize__set_state(<AsArrayTypedSize> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_AsArrayTypedSize__set_state(AsArrayTypedSize __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_13arraydatatype___pyx_unpickle_AsArrayTypedSize__set_state(((struct __pyx_obj_17OpenGL_accelerate_13arraydatatype_AsArrayTypedSize *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_13arraydatatype___pyx_unpickle_AsArrayTypedSize__set_state(((struct __pyx_obj_17OpenGL_accelerate_13arraydatatype_AsArrayTypedSize *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x5629caa = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x5629caa, 0x865d52c, 0xd219003) = (arrayIndex, arrayName, arrayType))" % __pyx_checksum)
  *     __pyx_result = AsArrayTypedSize.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_AsArrayTypedSize__set_state(<AsArrayTypedSize> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -18691,18 +18823,18 @@
  * def __pyx_unpickle_AsArrayTypedSize(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.arraydatatype.__pyx_unpickle_AsArrayTypedSize", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -20310,21 +20442,21 @@
   {&__pyx_n_s_DO_OUTPUT, __pyx_k_DO_OUTPUT, sizeof(__pyx_k_DO_OUTPUT), 0, 0, 1, 1},
   {&__pyx_kp_s_Did_not_resolve_parameter_index, __pyx_k_Did_not_resolve_parameter_index, sizeof(__pyx_k_Did_not_resolve_parameter_index), 0, 0, 1, 0},
   {&__pyx_kp_s_Expected_r_byte_array_got_r_byte, __pyx_k_Expected_r_byte_array_got_r_byte, sizeof(__pyx_k_Expected_r_byte_array_got_r_byte), 0, 0, 1, 0},
   {&__pyx_n_s_FormatHandler, __pyx_k_FormatHandler, sizeof(__pyx_k_FormatHandler), 0, 0, 1, 1},
   {&__pyx_n_s_GENERIC_OUTPUT_PREFERENCES, __pyx_k_GENERIC_OUTPUT_PREFERENCES, sizeof(__pyx_k_GENERIC_OUTPUT_PREFERENCES), 0, 0, 1, 1},
   {&__pyx_n_s_HandlerRegistry, __pyx_k_HandlerRegistry, sizeof(__pyx_k_HandlerRegistry), 0, 0, 1, 1},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x56, __pyx_k_Incompatible_checksums_s_vs_0x56, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x56), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x59, __pyx_k_Incompatible_checksums_s_vs_0x59, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x59), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x66, __pyx_k_Incompatible_checksums_s_vs_0x66, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x66), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x6c, __pyx_k_Incompatible_checksums_s_vs_0x6c, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x6c), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xb4, __pyx_k_Incompatible_checksums_s_vs_0xb4, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xb4), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xb8, __pyx_k_Incompatible_checksums_s_vs_0xb8, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xb8), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xe1, __pyx_k_Incompatible_checksums_s_vs_0xe1, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xe1), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2, __pyx_k_Incompatible_checksums_0x_x_vs_0_2, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_2), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_3, __pyx_k_Incompatible_checksums_0x_x_vs_0_3, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_3), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_4, __pyx_k_Incompatible_checksums_0x_x_vs_0_4, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_4), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_5, __pyx_k_Incompatible_checksums_0x_x_vs_0_5, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_5), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_6, __pyx_k_Incompatible_checksums_0x_x_vs_0_6, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_6), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_7, __pyx_k_Incompatible_checksums_0x_x_vs_0_7, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_7), 0, 0, 1, 0},
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_n_s_KeyError, __pyx_k_KeyError, sizeof(__pyx_k_KeyError), 0, 0, 1, 1},
   {&__pyx_n_s_NULL, __pyx_k_NULL, sizeof(__pyx_k_NULL), 0, 0, 1, 1},
   {&__pyx_n_s_NULL_2, __pyx_k_NULL_2, sizeof(__pyx_k_NULL_2), 0, 0, 1, 1},
   {&__pyx_kp_s_No_array_type_handler_for_type_r, __pyx_k_No_array_type_handler_for_type_r, sizeof(__pyx_k_No_array_type_handler_for_type_r), 0, 0, 1, 0},
   {&__pyx_n_s_OpenGL, __pyx_k_OpenGL, sizeof(__pyx_k_OpenGL), 0, 0, 1, 1},
   {&__pyx_n_s_OpenGL__null, __pyx_k_OpenGL__null, sizeof(__pyx_k_OpenGL__null), 0, 0, 1, 1},
@@ -20474,78 +20606,121 @@
  *             try:
  *                 return result[0]
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_int_1); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "(tree fragment)":1
- * def __pyx_unpickle_HandlerRegistry(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+  /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0x6673075, 0xb44d830, 0x758d679):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6673075, 0xb44d830, 0x758d679) = (all_output_handlers, match, output_handler, preferredOutput, registry))" % __pyx_checksum)
  */
-  __pyx_tuple__4 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(3, __pyx_int_107425909, __pyx_int_189061168, __pyx_int_123262585); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_HandlerRegistry, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__6 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(3, __pyx_int_236061798, __pyx_int_225748502, __pyx_int_144838955); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_tuple__6 = PyTuple_Pack(3, __pyx_int_113247033, __pyx_int_253740281, __pyx_int_156747773); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_ArrayDatatype, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__8 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(3, __pyx_int_189242252, __pyx_int_200435286, __pyx_int_61857947); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_94205906, __pyx_int_261772138, __pyx_int_143391459); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Output, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__10 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(3, __pyx_int_90348714, __pyx_int_140891436, __pyx_int_220303363); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_tuple__10 = PyTuple_Pack(3, __pyx_int_193119699, __pyx_int_93210383, __pyx_int_179834829); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_OutputOrInput, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__12 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_SizedOutput, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__14 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_SizedOutputOrInpu, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__16 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_AsArrayOfType, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__18 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_AsArrayTyped, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__20 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_AsArrayTypedSizeC, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__22 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_AsArrayTypedSize, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(1, 1, __pyx_L1_error)
+
+  /* "(tree fragment)":1
+ * def __pyx_unpickle_HandlerRegistry(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
+  __pyx_tuple__11 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_HandlerRegistry, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_ArrayDatatype, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Output, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_OutputOrInput, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_SizedOutput, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_SizedOutputOrInpu, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_AsArrayOfType, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_AsArrayTyped, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_AsArrayTypedSizeC, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__29 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__29);
+  __Pyx_GIVEREF(__pyx_tuple__29);
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_AsArrayTypedSize, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   __pyx_umethod_PyDict_Type_get.type = (PyObject*)&PyDict_Type;
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_50 = PyInt_FromLong(50); if (unlikely(!__pyx_int_50)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_61857947 = PyInt_FromLong(61857947L); if (unlikely(!__pyx_int_61857947)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_90348714 = PyInt_FromLong(90348714L); if (unlikely(!__pyx_int_90348714)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_93210383 = PyInt_FromLong(93210383L); if (unlikely(!__pyx_int_93210383)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_94205906 = PyInt_FromLong(94205906L); if (unlikely(!__pyx_int_94205906)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_107425909 = PyInt_FromLong(107425909L); if (unlikely(!__pyx_int_107425909)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_113247033 = PyInt_FromLong(113247033L); if (unlikely(!__pyx_int_113247033)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_123262585 = PyInt_FromLong(123262585L); if (unlikely(!__pyx_int_123262585)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_140891436 = PyInt_FromLong(140891436L); if (unlikely(!__pyx_int_140891436)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_143391459 = PyInt_FromLong(143391459L); if (unlikely(!__pyx_int_143391459)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_144838955 = PyInt_FromLong(144838955L); if (unlikely(!__pyx_int_144838955)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_156747773 = PyInt_FromLong(156747773L); if (unlikely(!__pyx_int_156747773)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_179834829 = PyInt_FromLong(179834829L); if (unlikely(!__pyx_int_179834829)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_189061168 = PyInt_FromLong(189061168L); if (unlikely(!__pyx_int_189061168)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_189242252 = PyInt_FromLong(189242252L); if (unlikely(!__pyx_int_189242252)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_193119699 = PyInt_FromLong(193119699L); if (unlikely(!__pyx_int_193119699)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_200435286 = PyInt_FromLong(200435286L); if (unlikely(!__pyx_int_200435286)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_220303363 = PyInt_FromLong(220303363L); if (unlikely(!__pyx_int_220303363)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_225748502 = PyInt_FromLong(225748502L); if (unlikely(!__pyx_int_225748502)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_236061798 = PyInt_FromLong(236061798L); if (unlikely(!__pyx_int_236061798)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_253740281 = PyInt_FromLong(253740281L); if (unlikely(!__pyx_int_253740281)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_261772138 = PyInt_FromLong(261772138L); if (unlikely(!__pyx_int_261772138)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -20608,25 +20783,25 @@
   if (PyType_Ready(&__pyx_type_17OpenGL_accelerate_13arraydatatype_ArrayDatatype) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_17OpenGL_accelerate_13arraydatatype_ArrayDatatype.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_17OpenGL_accelerate_13arraydatatype_ArrayDatatype.tp_dictoffset && __pyx_type_17OpenGL_accelerate_13arraydatatype_ArrayDatatype.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_17OpenGL_accelerate_13arraydatatype_ArrayDatatype.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_17OpenGL_accelerate_13arraydatatype_ArrayDatatype, "__init__"); if (unlikely(!wrapper)) __PYX_ERR(0, 106, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_17OpenGL_accelerate_13arraydatatype_13ArrayDatatype___init__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_17OpenGL_accelerate_13arraydatatype_13ArrayDatatype___init__.doc = __pyx_doc_17OpenGL_accelerate_13arraydatatype_13ArrayDatatype___init__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_17OpenGL_accelerate_13arraydatatype_13ArrayDatatype___init__;
     }
   }
   #endif
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_17OpenGL_accelerate_13arraydatatype_ArrayDatatype, "__call__"); if (unlikely(!wrapper)) __PYX_ERR(0, 106, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_17OpenGL_accelerate_13arraydatatype_13ArrayDatatype_8__call__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_17OpenGL_accelerate_13arraydatatype_13ArrayDatatype_8__call__.doc = __pyx_doc_17OpenGL_accelerate_13arraydatatype_13ArrayDatatype_8__call__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_17OpenGL_accelerate_13arraydatatype_13ArrayDatatype_8__call__;
     }
@@ -22932,25 +23107,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
 #endif
+    if (getstate) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+#else
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
+#endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -22987,14 +23180,16 @@
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
@@ -23203,14 +23398,20 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
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
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -23266,22 +23467,32 @@
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
@@ -23882,19 +24093,41 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
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
```

### Comparing `PyOpenGL-accelerate-3.1.6/src/arraydatatype.pyx` & `PyOpenGL-accelerate-3.1.7/src/arraydatatype.pyx`

 * *Files identical despite different names*

### Comparing `PyOpenGL-accelerate-3.1.6/src/buffers_formathandler.c` & `PyOpenGL-accelerate-3.1.7/src/buffers_formathandler.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.28 */
+/* Generated by Cython 0.29.32 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_28"
-#define CYTHON_HEX_VERSION 0x001D1CF0
+#define CYTHON_ABI "0_29_32"
+#define CYTHON_HEX_VERSION 0x001D20F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -45,14 +45,15 @@
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
@@ -81,18 +82,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
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
@@ -122,18 +127,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
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
@@ -175,15 +229,15 @@
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 0
   #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
@@ -192,14 +246,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
@@ -643,16 +700,18 @@
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
@@ -1201,14 +1260,20 @@
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
 #if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif // CYTHON_FAST_PYCALL
 #endif
@@ -1324,14 +1389,20 @@
 
 /* GetAttr.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
 
 /* GetAttr3.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
 
+/* PySequenceContains.proto */
+static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
+    int result = PySequence_Contains(seq, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
                __Pyx_GetItemInt_Generic(o, to_py_func(i))))
 #define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
@@ -1535,24 +1606,24 @@
 static const char __pyx_k_NotImplementedError[] = "NotImplementedError";
 static const char __pyx_k_ARRAY_TO_GL_TYPE_MAPPING[] = "ARRAY_TO_GL_TYPE_MAPPING";
 static const char __pyx_k_OpenGL_arrays__arrayconstants[] = "OpenGL.arrays._arrayconstants";
 static const char __pyx_k_Unable_to_load_array_constants[] = "Unable to load array constants";
 static const char __pyx_k_pyx_unpickle_MemoryviewHandler[] = "__pyx_unpickle_MemoryviewHandler";
 static const char __pyx_k_Don_t_know_GL_type_for_array_of[] = "Don't know GL type for array of type %r, known types: %s\nvalue:%s";
 static const char __pyx_k_Cython_memoryview_implementation[] = "Cython memoryview implementation of buffer-api format handler";
-static const char __pyx_k_Incompatible_checksums_s_vs_0x40[] = "Incompatible checksums (%s vs 0x4048af0 = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x4048af0, 0xf213594, 0xb577e6f) = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))";
 static const char __pyx_k_Need_a_MemoryView_instance_in_fr[] = "Need a MemoryView instance in from_param (call asArray first)";
 static const char __pyx_k_Need_to_use_a_subclass_to_get_ze[] = "Need to use a subclass to get zeros support";
 static const char __pyx_k_OpenGL_accelerate_buffers_format[] = "OpenGL_accelerate.buffers_formathandler";
 static PyObject *__pyx_n_s_ARRAY_TO_GL_TYPE_MAPPING;
 static PyObject *__pyx_n_s_CopyError;
 static PyObject *__pyx_kp_s_Don_t_know_GL_type_for_array_of;
 static PyObject *__pyx_n_s_ERROR_ON_COPY;
 static PyObject *__pyx_n_s_ImportError;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x40;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
 static PyObject *__pyx_n_s_MemoryviewHandler;
 static PyObject *__pyx_kp_s_Need_a_MemoryView_instance_in_fr;
 static PyObject *__pyx_kp_s_Need_to_use_a_subclass_to_get_ze;
 static PyObject *__pyx_n_s_NotImplementedError;
 static PyObject *__pyx_n_s_OpenGL;
 static PyObject *__pyx_n_s_OpenGL__bytes;
 static PyObject *__pyx_n_s_OpenGL_accelerate_buffers_format;
@@ -1608,19 +1679,22 @@
 static PyObject *__pyx_pf_17OpenGL_accelerate_21buffers_formathandler_17MemoryviewHandler_4__setstate_cython__(struct __pyx_obj_17OpenGL_accelerate_21buffers_formathandler_MemoryviewHandler *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_17OpenGL_accelerate_21buffers_formathandler___pyx_unpickle_MemoryviewHandler(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_17OpenGL_accelerate_21buffers_formathandler_MemoryviewHandler(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_get = {0, &__pyx_n_s_get, 0, 0, 0};
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_keys = {0, &__pyx_n_s_keys, 0, 0, 0};
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_67406576;
+static PyObject *__pyx_int_190283375;
+static PyObject *__pyx_int_253834644;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
-static PyObject *__pyx_codeobj__5;
+static PyObject *__pyx_tuple__5;
+static PyObject *__pyx_codeobj__6;
 /* Late includes */
 
 /* "src/buffers_formathandler.pyx":55
  *     isOutput = True
  * 
  *     def __init__( self, ERROR_ON_COPY=None, a_to_gl=None ):             # <<<<<<<<<<<<<<
  *         if ERROR_ON_COPY is None:
@@ -3514,151 +3588,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_21buffers_formathandler___pyx_unpickle_MemoryviewHandler(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_MemoryviewHandler", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x4048af0:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x4048af0, 0xf213594, 0xb577e6f):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x4048af0 = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x4048af0, 0xf213594, 0xb577e6f) = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x4048af0) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__4, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x4048af0:
+ *     if __pyx_checksum not in (0x4048af0, 0xf213594, 0xb577e6f):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x4048af0 = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x4048af0, 0xf213594, 0xb577e6f) = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
  *     __pyx_result = MemoryviewHandler.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x4048af0:
+ *     if __pyx_checksum not in (0x4048af0, 0xf213594, 0xb577e6f):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x4048af0 = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x4048af0, 0xf213594, 0xb577e6f) = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = MemoryviewHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x40, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x4048af0:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x4048af0, 0xf213594, 0xb577e6f):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x4048af0 = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x4048af0, 0xf213594, 0xb577e6f) = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x4048af0 = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x4048af0, 0xf213594, 0xb577e6f) = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
  *     __pyx_result = MemoryviewHandler.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_MemoryviewHandler__set_state(<MemoryviewHandler> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_21buffers_formathandler_MemoryviewHandler), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_21buffers_formathandler_MemoryviewHandler), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x4048af0 = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x4048af0, 0xf213594, 0xb577e6f) = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
  *     __pyx_result = MemoryviewHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_MemoryviewHandler__set_state(<MemoryviewHandler> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = MemoryviewHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_MemoryviewHandler__set_state(<MemoryviewHandler> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_MemoryviewHandler__set_state(MemoryviewHandler __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_21buffers_formathandler___pyx_unpickle_MemoryviewHandler__set_state(((struct __pyx_obj_17OpenGL_accelerate_21buffers_formathandler_MemoryviewHandler *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_21buffers_formathandler___pyx_unpickle_MemoryviewHandler__set_state(((struct __pyx_obj_17OpenGL_accelerate_21buffers_formathandler_MemoryviewHandler *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x4048af0 = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x4048af0, 0xf213594, 0xb577e6f) = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
  *     __pyx_result = MemoryviewHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_MemoryviewHandler__set_state(<MemoryviewHandler> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -3678,18 +3756,18 @@
  * def __pyx_unpickle_MemoryviewHandler(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.buffers_formathandler.__pyx_unpickle_MemoryviewHandler", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -4063,15 +4141,15 @@
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_n_s_ARRAY_TO_GL_TYPE_MAPPING, __pyx_k_ARRAY_TO_GL_TYPE_MAPPING, sizeof(__pyx_k_ARRAY_TO_GL_TYPE_MAPPING), 0, 0, 1, 1},
   {&__pyx_n_s_CopyError, __pyx_k_CopyError, sizeof(__pyx_k_CopyError), 0, 0, 1, 1},
   {&__pyx_kp_s_Don_t_know_GL_type_for_array_of, __pyx_k_Don_t_know_GL_type_for_array_of, sizeof(__pyx_k_Don_t_know_GL_type_for_array_of), 0, 0, 1, 0},
   {&__pyx_n_s_ERROR_ON_COPY, __pyx_k_ERROR_ON_COPY, sizeof(__pyx_k_ERROR_ON_COPY), 0, 0, 1, 1},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x40, __pyx_k_Incompatible_checksums_s_vs_0x40, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x40), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
   {&__pyx_n_s_MemoryviewHandler, __pyx_k_MemoryviewHandler, sizeof(__pyx_k_MemoryviewHandler), 0, 0, 1, 1},
   {&__pyx_kp_s_Need_a_MemoryView_instance_in_fr, __pyx_k_Need_a_MemoryView_instance_in_fr, sizeof(__pyx_k_Need_a_MemoryView_instance_in_fr), 0, 0, 1, 0},
   {&__pyx_kp_s_Need_to_use_a_subclass_to_get_ze, __pyx_k_Need_to_use_a_subclass_to_get_ze, sizeof(__pyx_k_Need_to_use_a_subclass_to_get_ze), 0, 0, 1, 0},
   {&__pyx_n_s_NotImplementedError, __pyx_k_NotImplementedError, sizeof(__pyx_k_NotImplementedError), 0, 0, 1, 1},
   {&__pyx_n_s_OpenGL, __pyx_k_OpenGL, sizeof(__pyx_k_OpenGL), 0, 0, 1, 1},
   {&__pyx_n_s_OpenGL__bytes, __pyx_k_OpenGL__bytes, sizeof(__pyx_k_OpenGL__bytes), 0, 0, 1, 1},
   {&__pyx_n_s_OpenGL_accelerate_buffers_format, __pyx_k_OpenGL_accelerate_buffers_format, sizeof(__pyx_k_OpenGL_accelerate_buffers_format), 0, 0, 1, 1},
@@ -4162,36 +4240,49 @@
  *     cdef c_arraySize( self, object instance, object typeCode ):
  *         """Retrieve array size reference"""
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_Need_to_use_a_subclass_to_get_ze); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "(tree fragment)":1
- * def __pyx_unpickle_MemoryviewHandler(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+  /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0x4048af0, 0xf213594, 0xb577e6f):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x4048af0, 0xf213594, 0xb577e6f) = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
  */
-  __pyx_tuple__4 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(3, __pyx_int_67406576, __pyx_int_253834644, __pyx_int_190283375); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_MemoryviewHandler, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(1, 1, __pyx_L1_error)
+
+  /* "(tree fragment)":1
+ * def __pyx_unpickle_MemoryviewHandler(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
+  __pyx_tuple__5 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_MemoryviewHandler, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   __pyx_umethod_PyDict_Type_get.type = (PyObject*)&PyDict_Type;
   __pyx_umethod_PyDict_Type_keys.type = (PyObject*)&PyDict_Type;
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_67406576 = PyInt_FromLong(67406576L); if (unlikely(!__pyx_int_67406576)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_190283375 = PyInt_FromLong(190283375L); if (unlikely(!__pyx_int_190283375)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_253834644 = PyInt_FromLong(253834644L); if (unlikely(!__pyx_int_253834644)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -6133,25 +6224,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
 #endif
+    if (getstate) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+#else
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
+#endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -6188,14 +6297,16 @@
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
@@ -6323,14 +6434,20 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
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
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -6386,22 +6503,32 @@
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
@@ -7002,19 +7129,41 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
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
```

### Comparing `PyOpenGL-accelerate-3.1.6/src/buffers_formathandler.pyx` & `PyOpenGL-accelerate-3.1.7/src/buffers_formathandler.pyx`

 * *Files identical despite different names*

### Comparing `PyOpenGL-accelerate-3.1.6/src/errorchecker.c` & `PyOpenGL-accelerate-3.1.7/src/errorchecker.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.28 */
+/* Generated by Cython 0.29.32 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_28"
-#define CYTHON_HEX_VERSION 0x001D1CF0
+#define CYTHON_ABI "0_29_32"
+#define CYTHON_HEX_VERSION 0x001D20F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -45,14 +45,15 @@
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
@@ -81,18 +82,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
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
@@ -122,18 +127,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
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
@@ -175,15 +229,15 @@
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 0
   #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
@@ -192,14 +246,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
@@ -643,16 +700,18 @@
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
@@ -1062,14 +1121,20 @@
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
 #if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif // CYTHON_FAST_PYCALL
 #endif
@@ -1158,14 +1223,20 @@
 
 /* GetAttr.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
 
 /* GetAttr3.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
 
+/* PySequenceContains.proto */
+static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
+    int result = PySequence_Contains(seq, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
@@ -1318,21 +1389,21 @@
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_CONTEXT_CHECKING[] = "CONTEXT_CHECKING";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_CurrentContextIsValid[] = "CurrentContextIsValid";
 static const char __pyx_k_pyx_unpickle__ErrorChecker[] = "__pyx_unpickle__ErrorChecker";
 static const char __pyx_k_OpenGL_accelerate_errorchecker[] = "OpenGL_accelerate.errorchecker";
 static const char __pyx_k_Cython_coded_GL_error_check_modu[] = "Cython-coded GL-error-check module";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xc5[] = "Incompatible checksums (%s vs 0xc56610f = (_errorClass, _getErrors, _isValid, _noErrorResult, checkContext, doChecks))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xc56610f, 0x21f4614, 0xf220d93) = (_errorClass, _getErrors, _isValid, _noErrorResult, checkContext, doChecks))";
 static PyObject *__pyx_n_s_CONTEXT_CHECKING;
 static PyObject *__pyx_n_s_CurrentContextIsValid;
 static PyObject *__pyx_n_s_ERROR_CHECKING;
 static PyObject *__pyx_n_s_ErrorChecker;
 static PyObject *__pyx_n_s_GLError;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xc5;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
 static PyObject *__pyx_n_s_OpenGL;
 static PyObject *__pyx_n_s_OpenGL_accelerate_errorchecker;
 static PyObject *__pyx_n_s_OpenGL_error;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_baseOperation;
 static PyObject *__pyx_n_s_cArguments;
 static PyObject *__pyx_n_s_cline_in_traceback;
@@ -1385,31 +1456,34 @@
 static PyObject *__pyx_pf_17OpenGL_accelerate_12errorchecker_13_ErrorChecker_14_noErrorResult___get__(struct __pyx_obj_17OpenGL_accelerate_12errorchecker__ErrorChecker *__pyx_v_self); /* proto */
 static int __pyx_pf_17OpenGL_accelerate_12errorchecker_13_ErrorChecker_14_noErrorResult_2__set__(struct __pyx_obj_17OpenGL_accelerate_12errorchecker__ErrorChecker *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_17OpenGL_accelerate_12errorchecker_13_ErrorChecker_10__reduce_cython__(struct __pyx_obj_17OpenGL_accelerate_12errorchecker__ErrorChecker *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_17OpenGL_accelerate_12errorchecker_13_ErrorChecker_12__setstate_cython__(struct __pyx_obj_17OpenGL_accelerate_12errorchecker__ErrorChecker *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_17OpenGL_accelerate_12errorchecker___pyx_unpickle__ErrorChecker(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_17OpenGL_accelerate_12errorchecker__ErrorChecker(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_0;
+static PyObject *__pyx_int_35603988;
 static PyObject *__pyx_int_206987535;
+static PyObject *__pyx_int_253889939;
 static PyObject *__pyx_tuple_;
-static PyObject *__pyx_codeobj__2;
+static PyObject *__pyx_tuple__2;
+static PyObject *__pyx_codeobj__3;
 /* Late includes */
 
 /* "src/errorchecker.pyx":18
  *     cdef public int _noErrorResult
  * 
  *     def __init__( self, platform, baseOperation, noErrorResult=0, errorClass=None ):             # <<<<<<<<<<<<<<
  *         """Initialize from a platform module/reference"""
  *         self._isValid = platform.CurrentContextIsValid
  */
 
 /* Python wrapper */
 static int __pyx_pw_17OpenGL_accelerate_12errorchecker_13_ErrorChecker_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_17OpenGL_accelerate_12errorchecker_13_ErrorChecker___init__[] = "Initialize from a platform module/reference";
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_17OpenGL_accelerate_12errorchecker_13_ErrorChecker___init__;
 #endif
 static int __pyx_pw_17OpenGL_accelerate_12errorchecker_13_ErrorChecker_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_platform = 0;
   PyObject *__pyx_v_baseOperation = 0;
   PyObject *__pyx_v_noErrorResult = 0;
   PyObject *__pyx_v_errorClass = 0;
@@ -3326,151 +3400,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_12errorchecker___pyx_unpickle__ErrorChecker(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle__ErrorChecker", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xc56610f:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xc56610f, 0x21f4614, 0xf220d93):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xc56610f = (_errorClass, _getErrors, _isValid, _noErrorResult, checkContext, doChecks))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc56610f, 0x21f4614, 0xf220d93) = (_errorClass, _getErrors, _isValid, _noErrorResult, checkContext, doChecks))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xc56610f) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple_, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xc56610f:
+ *     if __pyx_checksum not in (0xc56610f, 0x21f4614, 0xf220d93):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xc56610f = (_errorClass, _getErrors, _isValid, _noErrorResult, checkContext, doChecks))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc56610f, 0x21f4614, 0xf220d93) = (_errorClass, _getErrors, _isValid, _noErrorResult, checkContext, doChecks))" % __pyx_checksum)
  *     __pyx_result = _ErrorChecker.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xc56610f:
+ *     if __pyx_checksum not in (0xc56610f, 0x21f4614, 0xf220d93):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xc56610f = (_errorClass, _getErrors, _isValid, _noErrorResult, checkContext, doChecks))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc56610f, 0x21f4614, 0xf220d93) = (_errorClass, _getErrors, _isValid, _noErrorResult, checkContext, doChecks))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = _ErrorChecker.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xc5, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xc56610f:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xc56610f, 0x21f4614, 0xf220d93):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xc56610f = (_errorClass, _getErrors, _isValid, _noErrorResult, checkContext, doChecks))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc56610f, 0x21f4614, 0xf220d93) = (_errorClass, _getErrors, _isValid, _noErrorResult, checkContext, doChecks))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xc56610f = (_errorClass, _getErrors, _isValid, _noErrorResult, checkContext, doChecks))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc56610f, 0x21f4614, 0xf220d93) = (_errorClass, _getErrors, _isValid, _noErrorResult, checkContext, doChecks))" % __pyx_checksum)
  *     __pyx_result = _ErrorChecker.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle__ErrorChecker__set_state(<_ErrorChecker> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_12errorchecker__ErrorChecker), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_12errorchecker__ErrorChecker), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xc56610f = (_errorClass, _getErrors, _isValid, _noErrorResult, checkContext, doChecks))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc56610f, 0x21f4614, 0xf220d93) = (_errorClass, _getErrors, _isValid, _noErrorResult, checkContext, doChecks))" % __pyx_checksum)
  *     __pyx_result = _ErrorChecker.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle__ErrorChecker__set_state(<_ErrorChecker> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = _ErrorChecker.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle__ErrorChecker__set_state(<_ErrorChecker> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle__ErrorChecker__set_state(_ErrorChecker __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_12errorchecker___pyx_unpickle__ErrorChecker__set_state(((struct __pyx_obj_17OpenGL_accelerate_12errorchecker__ErrorChecker *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_12errorchecker___pyx_unpickle__ErrorChecker__set_state(((struct __pyx_obj_17OpenGL_accelerate_12errorchecker__ErrorChecker *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xc56610f = (_errorClass, _getErrors, _isValid, _noErrorResult, checkContext, doChecks))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc56610f, 0x21f4614, 0xf220d93) = (_errorClass, _getErrors, _isValid, _noErrorResult, checkContext, doChecks))" % __pyx_checksum)
  *     __pyx_result = _ErrorChecker.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle__ErrorChecker__set_state(<_ErrorChecker> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -3490,18 +3568,18 @@
  * def __pyx_unpickle__ErrorChecker(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.errorchecker.__pyx_unpickle__ErrorChecker", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -3970,15 +4048,15 @@
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_n_s_CONTEXT_CHECKING, __pyx_k_CONTEXT_CHECKING, sizeof(__pyx_k_CONTEXT_CHECKING), 0, 0, 1, 1},
   {&__pyx_n_s_CurrentContextIsValid, __pyx_k_CurrentContextIsValid, sizeof(__pyx_k_CurrentContextIsValid), 0, 0, 1, 1},
   {&__pyx_n_s_ERROR_CHECKING, __pyx_k_ERROR_CHECKING, sizeof(__pyx_k_ERROR_CHECKING), 0, 0, 1, 1},
   {&__pyx_n_s_ErrorChecker, __pyx_k_ErrorChecker, sizeof(__pyx_k_ErrorChecker), 0, 0, 1, 1},
   {&__pyx_n_s_GLError, __pyx_k_GLError, sizeof(__pyx_k_GLError), 0, 0, 1, 1},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xc5, __pyx_k_Incompatible_checksums_s_vs_0xc5, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xc5), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
   {&__pyx_n_s_OpenGL, __pyx_k_OpenGL, sizeof(__pyx_k_OpenGL), 0, 0, 1, 1},
   {&__pyx_n_s_OpenGL_accelerate_errorchecker, __pyx_k_OpenGL_accelerate_errorchecker, sizeof(__pyx_k_OpenGL_accelerate_errorchecker), 0, 0, 1, 1},
   {&__pyx_n_s_OpenGL_error, __pyx_k_OpenGL_error, sizeof(__pyx_k_OpenGL_error), 0, 0, 1, 1},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_baseOperation, __pyx_k_baseOperation, sizeof(__pyx_k_baseOperation), 0, 0, 1, 1},
   {&__pyx_n_s_cArguments, __pyx_k_cArguments, sizeof(__pyx_k_cArguments), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
@@ -4016,34 +4094,47 @@
   return 0;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "(tree fragment)":1
- * def __pyx_unpickle__ErrorChecker(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+  /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0xc56610f, 0x21f4614, 0xf220d93):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc56610f, 0x21f4614, 0xf220d93) = (_errorClass, _getErrors, _isValid, _noErrorResult, checkContext, doChecks))" % __pyx_checksum)
  */
-  __pyx_tuple_ = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(3, __pyx_int_206987535, __pyx_int_35603988, __pyx_int_253889939); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
-  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple_, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle__ErrorChecker, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(1, 1, __pyx_L1_error)
+
+  /* "(tree fragment)":1
+ * def __pyx_unpickle__ErrorChecker(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
+  __pyx_tuple__2 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
+  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle__ErrorChecker, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_35603988 = PyInt_FromLong(35603988L); if (unlikely(!__pyx_int_35603988)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_206987535 = PyInt_FromLong(206987535L); if (unlikely(!__pyx_int_206987535)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_253889939 = PyInt_FromLong(253889939L); if (unlikely(!__pyx_int_253889939)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -4087,15 +4178,15 @@
   if (PyType_Ready(&__pyx_type_17OpenGL_accelerate_12errorchecker__ErrorChecker) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_17OpenGL_accelerate_12errorchecker__ErrorChecker.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_17OpenGL_accelerate_12errorchecker__ErrorChecker.tp_dictoffset && __pyx_type_17OpenGL_accelerate_12errorchecker__ErrorChecker.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_17OpenGL_accelerate_12errorchecker__ErrorChecker.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_17OpenGL_accelerate_12errorchecker__ErrorChecker, "__init__"); if (unlikely(!wrapper)) __PYX_ERR(0, 4, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_17OpenGL_accelerate_12errorchecker_13_ErrorChecker___init__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_17OpenGL_accelerate_12errorchecker_13_ErrorChecker___init__.doc = __pyx_doc_17OpenGL_accelerate_12errorchecker_13_ErrorChecker___init__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_17OpenGL_accelerate_12errorchecker_13_ErrorChecker___init__;
     }
@@ -5431,25 +5522,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
+#endif
+    if (getstate) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+#else
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
 #endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -5486,14 +5595,16 @@
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
@@ -5621,14 +5732,20 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
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
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -5684,22 +5801,32 @@
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
@@ -6300,19 +6427,41 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
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
```

### Comparing `PyOpenGL-accelerate-3.1.6/src/errorchecker.pyx` & `PyOpenGL-accelerate-3.1.7/src/errorchecker.pyx`

 * *Files identical despite different names*

### Comparing `PyOpenGL-accelerate-3.1.6/src/formathandler.c` & `PyOpenGL-accelerate-3.1.7/src/formathandler.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.28 */
+/* Generated by Cython 0.29.32 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_28"
-#define CYTHON_HEX_VERSION 0x001D1CF0
+#define CYTHON_ABI "0_29_32"
+#define CYTHON_HEX_VERSION 0x001D20F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -45,14 +45,15 @@
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
@@ -81,18 +82,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
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
@@ -122,18 +127,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
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
@@ -175,15 +229,15 @@
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 0
   #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
@@ -192,14 +246,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
@@ -643,16 +700,18 @@
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
@@ -1043,14 +1102,20 @@
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
 #if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif // CYTHON_FAST_PYCALL
 #endif
@@ -1183,14 +1248,20 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
+/* PySequenceContains.proto */
+static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
+    int result = PySequence_Contains(seq, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
                __Pyx_GetItemInt_Generic(o, to_py_func(i))))
 #define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
@@ -1363,19 +1434,19 @@
 static const char __pyx_k_s_does_not_define_arraySize_met[] = "%s does not define arraySize method";
 static const char __pyx_k_s_does_not_define_arrayToGLType[] = "%s does not define arrayToGLType method";
 static const char __pyx_k_s_does_not_define_asArray_metho[] = "%s does not define asArray method";
 static const char __pyx_k_s_does_not_define_dataPointer_m[] = "%s does not define dataPointer method";
 static const char __pyx_k_s_does_not_define_dimensions_me[] = "%s does not define dimensions method";
 static const char __pyx_k_s_does_not_define_from_param_me[] = "%s does not define from_param method";
 static const char __pyx_k_s_does_not_define_unitSize_meth[] = "%s does not define unitSize method";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xf7[] = "Incompatible checksums (%s vs 0xf703739 = (ERROR_ON_COPY))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xf703739, 0xdc45998, 0x7a908a8) = (ERROR_ON_COPY))";
 static PyObject *__pyx_n_s_ArrayDatatype;
 static PyObject *__pyx_n_s_FormatHandler;
 static PyObject *__pyx_n_s_HANDLED_TYPES;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xf7;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
 static PyObject *__pyx_n_s_NotImplementedError;
 static PyObject *__pyx_n_s_OpenGL_accelerate_formathandler;
 static PyObject *__pyx_n_s_OpenGL_arrays_arraydatatype;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_dict;
@@ -1434,31 +1505,34 @@
 static PyObject *__pyx_pf_17OpenGL_accelerate_13formathandler_13FormatHandler_24dimensions(struct __pyx_obj_17OpenGL_accelerate_13formathandler_FormatHandler *__pyx_v_self, PyObject *__pyx_v_instance); /* proto */
 static PyObject *__pyx_pf_17OpenGL_accelerate_13formathandler_13FormatHandler_13ERROR_ON_COPY___get__(struct __pyx_obj_17OpenGL_accelerate_13formathandler_FormatHandler *__pyx_v_self); /* proto */
 static int __pyx_pf_17OpenGL_accelerate_13formathandler_13FormatHandler_13ERROR_ON_COPY_2__set__(struct __pyx_obj_17OpenGL_accelerate_13formathandler_FormatHandler *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_17OpenGL_accelerate_13formathandler_13FormatHandler_26__reduce_cython__(struct __pyx_obj_17OpenGL_accelerate_13formathandler_FormatHandler *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_17OpenGL_accelerate_13formathandler_13FormatHandler_28__setstate_cython__(struct __pyx_obj_17OpenGL_accelerate_13formathandler_FormatHandler *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_17OpenGL_accelerate_13formathandler___pyx_unpickle_FormatHandler(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_17OpenGL_accelerate_13formathandler_FormatHandler(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_int_128518312;
+static PyObject *__pyx_int_230971800;
 static PyObject *__pyx_int_259012409;
 static PyObject *__pyx_tuple_;
-static PyObject *__pyx_codeobj__2;
+static PyObject *__pyx_tuple__2;
+static PyObject *__pyx_codeobj__3;
 /* Late includes */
 
 /* "src/formathandler.pyx":22
  * 	HANDLED_TYPES = ()
  * 
  * 	def __init__( self):             # <<<<<<<<<<<<<<
  * 		"""Initialize the format handler"""
  * 	def register( self, types=None ):
  */
 
 /* Python wrapper */
 static int __pyx_pw_17OpenGL_accelerate_13formathandler_13FormatHandler_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_17OpenGL_accelerate_13formathandler_13FormatHandler___init__[] = "Initialize the format handler";
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_17OpenGL_accelerate_13formathandler_13FormatHandler___init__;
 #endif
 static int __pyx_pw_17OpenGL_accelerate_13formathandler_13FormatHandler_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   if (unlikely(PyTuple_GET_SIZE(__pyx_args) > 0)) {
@@ -3736,151 +3810,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_13formathandler___pyx_unpickle_FormatHandler(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_FormatHandler", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xf703739:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xf703739, 0xdc45998, 0x7a908a8):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf703739 = (ERROR_ON_COPY))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf703739, 0xdc45998, 0x7a908a8) = (ERROR_ON_COPY))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xf703739) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple_, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xf703739:
+ *     if __pyx_checksum not in (0xf703739, 0xdc45998, 0x7a908a8):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf703739 = (ERROR_ON_COPY))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf703739, 0xdc45998, 0x7a908a8) = (ERROR_ON_COPY))" % __pyx_checksum)
  *     __pyx_result = FormatHandler.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xf703739:
+ *     if __pyx_checksum not in (0xf703739, 0xdc45998, 0x7a908a8):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf703739 = (ERROR_ON_COPY))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf703739, 0xdc45998, 0x7a908a8) = (ERROR_ON_COPY))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = FormatHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xf7, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xf703739:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xf703739, 0xdc45998, 0x7a908a8):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf703739 = (ERROR_ON_COPY))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf703739, 0xdc45998, 0x7a908a8) = (ERROR_ON_COPY))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf703739 = (ERROR_ON_COPY))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf703739, 0xdc45998, 0x7a908a8) = (ERROR_ON_COPY))" % __pyx_checksum)
  *     __pyx_result = FormatHandler.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_FormatHandler__set_state(<FormatHandler> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13formathandler_FormatHandler), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_13formathandler_FormatHandler), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf703739 = (ERROR_ON_COPY))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf703739, 0xdc45998, 0x7a908a8) = (ERROR_ON_COPY))" % __pyx_checksum)
  *     __pyx_result = FormatHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_FormatHandler__set_state(<FormatHandler> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = FormatHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_FormatHandler__set_state(<FormatHandler> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_FormatHandler__set_state(FormatHandler __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_13formathandler___pyx_unpickle_FormatHandler__set_state(((struct __pyx_obj_17OpenGL_accelerate_13formathandler_FormatHandler *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_13formathandler___pyx_unpickle_FormatHandler__set_state(((struct __pyx_obj_17OpenGL_accelerate_13formathandler_FormatHandler *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf703739 = (ERROR_ON_COPY))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf703739, 0xdc45998, 0x7a908a8) = (ERROR_ON_COPY))" % __pyx_checksum)
  *     __pyx_result = FormatHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_FormatHandler__set_state(<FormatHandler> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -3900,18 +3978,18 @@
  * def __pyx_unpickle_FormatHandler(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.formathandler.__pyx_unpickle_FormatHandler", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -4227,15 +4305,15 @@
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_n_s_ArrayDatatype, __pyx_k_ArrayDatatype, sizeof(__pyx_k_ArrayDatatype), 0, 0, 1, 1},
   {&__pyx_n_s_FormatHandler, __pyx_k_FormatHandler, sizeof(__pyx_k_FormatHandler), 0, 0, 1, 1},
   {&__pyx_n_s_HANDLED_TYPES, __pyx_k_HANDLED_TYPES, sizeof(__pyx_k_HANDLED_TYPES), 0, 0, 1, 1},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xf7, __pyx_k_Incompatible_checksums_s_vs_0xf7, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xf7), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
   {&__pyx_n_s_NotImplementedError, __pyx_k_NotImplementedError, sizeof(__pyx_k_NotImplementedError), 0, 0, 1, 1},
   {&__pyx_n_s_OpenGL_accelerate_formathandler, __pyx_k_OpenGL_accelerate_formathandler, sizeof(__pyx_k_OpenGL_accelerate_formathandler), 0, 0, 1, 1},
   {&__pyx_n_s_OpenGL_arrays_arraydatatype, __pyx_k_OpenGL_arrays_arraydatatype, sizeof(__pyx_k_OpenGL_arrays_arraydatatype), 0, 0, 1, 1},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
@@ -4288,32 +4366,45 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "(tree fragment)":1
- * def __pyx_unpickle_FormatHandler(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+  /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0xf703739, 0xdc45998, 0x7a908a8):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf703739, 0xdc45998, 0x7a908a8) = (ERROR_ON_COPY))" % __pyx_checksum)
  */
-  __pyx_tuple_ = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple_)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(3, __pyx_int_259012409, __pyx_int_230971800, __pyx_int_128518312); if (unlikely(!__pyx_tuple_)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
-  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple_, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_FormatHandler, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(2, 1, __pyx_L1_error)
+
+  /* "(tree fragment)":1
+ * def __pyx_unpickle_FormatHandler(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
+  __pyx_tuple__2 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
+  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_FormatHandler, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  __pyx_int_128518312 = PyInt_FromLong(128518312L); if (unlikely(!__pyx_int_128518312)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_230971800 = PyInt_FromLong(230971800L); if (unlikely(!__pyx_int_230971800)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_259012409 = PyInt_FromLong(259012409L); if (unlikely(!__pyx_int_259012409)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
@@ -4368,15 +4459,15 @@
   if (PyType_Ready(&__pyx_type_17OpenGL_accelerate_13formathandler_FormatHandler) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_17OpenGL_accelerate_13formathandler_FormatHandler.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_17OpenGL_accelerate_13formathandler_FormatHandler.tp_dictoffset && __pyx_type_17OpenGL_accelerate_13formathandler_FormatHandler.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_17OpenGL_accelerate_13formathandler_FormatHandler.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_17OpenGL_accelerate_13formathandler_FormatHandler, "__init__"); if (unlikely(!wrapper)) __PYX_ERR(0, 3, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_17OpenGL_accelerate_13formathandler_13FormatHandler___init__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_17OpenGL_accelerate_13formathandler_13FormatHandler___init__.doc = __pyx_doc_17OpenGL_accelerate_13formathandler_13FormatHandler___init__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_17OpenGL_accelerate_13formathandler_13FormatHandler___init__;
     }
@@ -5779,25 +5870,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
 #endif
+    if (getstate) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+#else
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
+#endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -5834,14 +5943,16 @@
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
@@ -5969,14 +6080,20 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
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
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -6032,22 +6149,32 @@
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
@@ -6648,19 +6775,41 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
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
```

### Comparing `PyOpenGL-accelerate-3.1.6/src/formathandler.pyx` & `PyOpenGL-accelerate-3.1.7/src/formathandler.pyx`

 * *Files identical despite different names*

### Comparing `PyOpenGL-accelerate-3.1.6/src/latebind.c` & `PyOpenGL-accelerate-3.1.7/src/latebind.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.28 */
+/* Generated by Cython 0.29.32 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_28"
-#define CYTHON_HEX_VERSION 0x001D1CF0
+#define CYTHON_ABI "0_29_32"
+#define CYTHON_HEX_VERSION 0x001D20F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -45,14 +45,15 @@
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
@@ -81,18 +82,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
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
@@ -122,18 +127,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
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
@@ -175,15 +229,15 @@
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 0
   #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
@@ -192,14 +246,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
@@ -643,16 +700,18 @@
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
@@ -1010,14 +1069,20 @@
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
 #if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif // CYTHON_FAST_PYCALL
 #endif
@@ -1162,14 +1227,20 @@
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
 /* ParseKeywords.proto */
 static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
     const char* function_name);
 
+/* PySequenceContains.proto */
+static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
+    int result = PySequence_Contains(seq, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* PyObjectCall2Args.proto */
@@ -1321,19 +1392,19 @@
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_wrapperFunction[] = "wrapperFunction";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_pyx_unpickle_Curry[] = "__pyx_unpickle_Curry";
 static const char __pyx_k_pyx_unpickle_LateBind[] = "__pyx_unpickle_LateBind";
 static const char __pyx_k_OpenGL_accelerate_latebind[] = "OpenGL_accelerate.latebind";
 static const char __pyx_k_General_pattern_which_does_late[] = "General pattern which does late-bound calls";
-static const char __pyx_k_Incompatible_checksums_s_vs_0x55[] = "Incompatible checksums (%s vs 0x558a770 = (baseFunction, wrapperFunction))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xe3[] = "Incompatible checksums (%s vs 0xe3df702 = (_finalCall))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xe3df702, 0x518e26c, 0xf22f0ad) = (_finalCall))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_2[] = "Incompatible checksums (0x%x vs (0x558a770, 0xf1a6081, 0x1677659) = (baseFunction, wrapperFunction))";
 static PyObject *__pyx_n_s_Curry;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x55;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xe3;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2;
 static PyObject *__pyx_n_s_LateBind;
 static PyObject *__pyx_n_s_OpenGL_accelerate_latebind;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_baseFunction;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_finalise;
@@ -1372,20 +1443,26 @@
 static PyObject *__pyx_pf_17OpenGL_accelerate_8latebind_5Curry_2__call__(struct __pyx_obj_17OpenGL_accelerate_8latebind_Curry *__pyx_v_self, PyObject *__pyx_v_args, PyObject *__pyx_v_named); /* proto */
 static PyObject *__pyx_pf_17OpenGL_accelerate_8latebind_5Curry_4__reduce_cython__(struct __pyx_obj_17OpenGL_accelerate_8latebind_Curry *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_17OpenGL_accelerate_8latebind_5Curry_6__setstate_cython__(struct __pyx_obj_17OpenGL_accelerate_8latebind_Curry *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_17OpenGL_accelerate_8latebind___pyx_unpickle_LateBind(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_17OpenGL_accelerate_8latebind_2__pyx_unpickle_Curry(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_17OpenGL_accelerate_8latebind_LateBind(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_17OpenGL_accelerate_8latebind_Curry(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_int_23557721;
+static PyObject *__pyx_int_85516908;
 static PyObject *__pyx_int_89696112;
 static PyObject *__pyx_int_238941954;
+static PyObject *__pyx_int_253386881;
+static PyObject *__pyx_int_253948077;
 static PyObject *__pyx_tuple_;
+static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
-static PyObject *__pyx_codeobj__2;
+static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_codeobj__4;
+static PyObject *__pyx_codeobj__6;
 /* Late includes */
 
 /* "src/latebind.pyx":10
  *     """
  *     cdef object _finalCall
  *     def setFinalCall( self, object finalCall ):             # <<<<<<<<<<<<<<
  *         """Set our finalCall to the callable object given"""
@@ -1762,15 +1839,15 @@
  *         """Call self._finalCall, calling finalise() first if not already called
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_17OpenGL_accelerate_8latebind_8LateBind_11__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_17OpenGL_accelerate_8latebind_8LateBind_10__call__[] = "Call self._finalCall, calling finalise() first if not already called\n\n        There's actually *no* reason to unpack and repack the arguments,\n        but unfortunately I don't know of a Cython syntax to specify\n        that.\n        ";
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_17OpenGL_accelerate_8latebind_8LateBind_10__call__;
 #endif
 static PyObject *__pyx_pw_17OpenGL_accelerate_8latebind_8LateBind_11__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_args = 0;
   PyObject *__pyx_v_named = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -2190,15 +2267,15 @@
  *         """Stores self.wrapperFunction and self.baseFunction"""
  *         self.baseFunction = baseFunction
  */
 
 /* Python wrapper */
 static int __pyx_pw_17OpenGL_accelerate_8latebind_5Curry_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_17OpenGL_accelerate_8latebind_5Curry___init__[] = "Stores self.wrapperFunction and self.baseFunction";
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_17OpenGL_accelerate_8latebind_5Curry___init__;
 #endif
 static int __pyx_pw_17OpenGL_accelerate_8latebind_5Curry_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_wrapperFunction = 0;
   PyObject *__pyx_v_baseFunction = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -2311,15 +2388,15 @@
  *         """returns self.wrapperFunction( self.baseFunction, *args, **named )"""
  *         return self.wrapperFunction( self.baseFunction, *args, **named )
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_17OpenGL_accelerate_8latebind_5Curry_3__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_17OpenGL_accelerate_8latebind_5Curry_2__call__[] = "returns self.wrapperFunction( self.baseFunction, *args, **named )";
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_17OpenGL_accelerate_8latebind_5Curry_2__call__;
 #endif
 static PyObject *__pyx_pw_17OpenGL_accelerate_8latebind_5Curry_3__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_args = 0;
   PyObject *__pyx_v_named = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -2784,151 +2861,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_8latebind___pyx_unpickle_LateBind(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_LateBind", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe3df702:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xe3df702, 0x518e26c, 0xf22f0ad):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe3df702 = (_finalCall))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe3df702, 0x518e26c, 0xf22f0ad) = (_finalCall))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xe3df702) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple_, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe3df702:
+ *     if __pyx_checksum not in (0xe3df702, 0x518e26c, 0xf22f0ad):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe3df702 = (_finalCall))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe3df702, 0x518e26c, 0xf22f0ad) = (_finalCall))" % __pyx_checksum)
  *     __pyx_result = LateBind.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xe3df702:
+ *     if __pyx_checksum not in (0xe3df702, 0x518e26c, 0xf22f0ad):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe3df702 = (_finalCall))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe3df702, 0x518e26c, 0xf22f0ad) = (_finalCall))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = LateBind.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xe3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe3df702:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xe3df702, 0x518e26c, 0xf22f0ad):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe3df702 = (_finalCall))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe3df702, 0x518e26c, 0xf22f0ad) = (_finalCall))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe3df702 = (_finalCall))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe3df702, 0x518e26c, 0xf22f0ad) = (_finalCall))" % __pyx_checksum)
  *     __pyx_result = LateBind.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_LateBind__set_state(<LateBind> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_8latebind_LateBind), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_8latebind_LateBind), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe3df702 = (_finalCall))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe3df702, 0x518e26c, 0xf22f0ad) = (_finalCall))" % __pyx_checksum)
  *     __pyx_result = LateBind.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_LateBind__set_state(<LateBind> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = LateBind.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_LateBind__set_state(<LateBind> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_LateBind__set_state(LateBind __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_8latebind___pyx_unpickle_LateBind__set_state(((struct __pyx_obj_17OpenGL_accelerate_8latebind_LateBind *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_8latebind___pyx_unpickle_LateBind__set_state(((struct __pyx_obj_17OpenGL_accelerate_8latebind_LateBind *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe3df702 = (_finalCall))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe3df702, 0x518e26c, 0xf22f0ad) = (_finalCall))" % __pyx_checksum)
  *     __pyx_result = LateBind.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_LateBind__set_state(<LateBind> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -2948,18 +3029,18 @@
  * def __pyx_unpickle_LateBind(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.latebind.__pyx_unpickle_LateBind", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -3181,151 +3262,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_8latebind_2__pyx_unpickle_Curry(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_Curry", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x558a770:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x558a770, 0xf1a6081, 0x1677659):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x558a770 = (baseFunction, wrapperFunction))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x558a770, 0xf1a6081, 0x1677659) = (baseFunction, wrapperFunction))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x558a770) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__2, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x558a770:
+ *     if __pyx_checksum not in (0x558a770, 0xf1a6081, 0x1677659):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x558a770 = (baseFunction, wrapperFunction))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x558a770, 0xf1a6081, 0x1677659) = (baseFunction, wrapperFunction))" % __pyx_checksum)
  *     __pyx_result = Curry.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x558a770:
+ *     if __pyx_checksum not in (0x558a770, 0xf1a6081, 0x1677659):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x558a770 = (baseFunction, wrapperFunction))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x558a770, 0xf1a6081, 0x1677659) = (baseFunction, wrapperFunction))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = Curry.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x55, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x558a770:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x558a770, 0xf1a6081, 0x1677659):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x558a770 = (baseFunction, wrapperFunction))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x558a770, 0xf1a6081, 0x1677659) = (baseFunction, wrapperFunction))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x558a770 = (baseFunction, wrapperFunction))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x558a770, 0xf1a6081, 0x1677659) = (baseFunction, wrapperFunction))" % __pyx_checksum)
  *     __pyx_result = Curry.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Curry__set_state(<Curry> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_8latebind_Curry), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_8latebind_Curry), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x558a770 = (baseFunction, wrapperFunction))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x558a770, 0xf1a6081, 0x1677659) = (baseFunction, wrapperFunction))" % __pyx_checksum)
  *     __pyx_result = Curry.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Curry__set_state(<Curry> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = Curry.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Curry__set_state(<Curry> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Curry__set_state(Curry __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_8latebind___pyx_unpickle_Curry__set_state(((struct __pyx_obj_17OpenGL_accelerate_8latebind_Curry *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_8latebind___pyx_unpickle_Curry__set_state(((struct __pyx_obj_17OpenGL_accelerate_8latebind_Curry *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x558a770 = (baseFunction, wrapperFunction))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x558a770, 0xf1a6081, 0x1677659) = (baseFunction, wrapperFunction))" % __pyx_checksum)
  *     __pyx_result = Curry.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Curry__set_state(<Curry> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -3345,18 +3430,18 @@
  * def __pyx_unpickle_Curry(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.latebind.__pyx_unpickle_Curry", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -3866,16 +3951,16 @@
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_n_s_Curry, __pyx_k_Curry, sizeof(__pyx_k_Curry), 0, 0, 1, 1},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x55, __pyx_k_Incompatible_checksums_s_vs_0x55, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x55), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xe3, __pyx_k_Incompatible_checksums_s_vs_0xe3, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xe3), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2, __pyx_k_Incompatible_checksums_0x_x_vs_0_2, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_2), 0, 0, 1, 0},
   {&__pyx_n_s_LateBind, __pyx_k_LateBind, sizeof(__pyx_k_LateBind), 0, 0, 1, 1},
   {&__pyx_n_s_OpenGL_accelerate_latebind, __pyx_k_OpenGL_accelerate_latebind, sizeof(__pyx_k_OpenGL_accelerate_latebind), 0, 0, 1, 1},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_baseFunction, __pyx_k_baseFunction, sizeof(__pyx_k_baseFunction), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_finalise, __pyx_k_finalise, sizeof(__pyx_k_finalise), 0, 0, 1, 1},
@@ -3908,38 +3993,56 @@
   return 0;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "(tree fragment)":1
- * def __pyx_unpickle_LateBind(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+  /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0xe3df702, 0x518e26c, 0xf22f0ad):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe3df702, 0x518e26c, 0xf22f0ad) = (_finalCall))" % __pyx_checksum)
  */
-  __pyx_tuple_ = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(3, __pyx_int_238941954, __pyx_int_85516908, __pyx_int_253948077); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
-  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple_, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_LateBind, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(3, __pyx_int_89696112, __pyx_int_253386881, __pyx_int_23557721); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
+
+  /* "(tree fragment)":1
+ * def __pyx_unpickle_LateBind(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
   __pyx_tuple__3 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Curry, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_LateBind, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Curry, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  __pyx_int_23557721 = PyInt_FromLong(23557721L); if (unlikely(!__pyx_int_23557721)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_85516908 = PyInt_FromLong(85516908L); if (unlikely(!__pyx_int_85516908)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_89696112 = PyInt_FromLong(89696112L); if (unlikely(!__pyx_int_89696112)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_238941954 = PyInt_FromLong(238941954L); if (unlikely(!__pyx_int_238941954)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_253386881 = PyInt_FromLong(253386881L); if (unlikely(!__pyx_int_253386881)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_253948077 = PyInt_FromLong(253948077L); if (unlikely(!__pyx_int_253948077)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -3983,15 +4086,15 @@
   if (PyType_Ready(&__pyx_type_17OpenGL_accelerate_8latebind_LateBind) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_17OpenGL_accelerate_8latebind_LateBind.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_17OpenGL_accelerate_8latebind_LateBind.tp_dictoffset && __pyx_type_17OpenGL_accelerate_8latebind_LateBind.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_17OpenGL_accelerate_8latebind_LateBind.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_17OpenGL_accelerate_8latebind_LateBind, "__call__"); if (unlikely(!wrapper)) __PYX_ERR(0, 3, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_17OpenGL_accelerate_8latebind_8LateBind_10__call__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_17OpenGL_accelerate_8latebind_8LateBind_10__call__.doc = __pyx_doc_17OpenGL_accelerate_8latebind_8LateBind_10__call__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_17OpenGL_accelerate_8latebind_8LateBind_10__call__;
     }
@@ -4003,25 +4106,25 @@
   if (PyType_Ready(&__pyx_type_17OpenGL_accelerate_8latebind_Curry) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_17OpenGL_accelerate_8latebind_Curry.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_17OpenGL_accelerate_8latebind_Curry.tp_dictoffset && __pyx_type_17OpenGL_accelerate_8latebind_Curry.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_17OpenGL_accelerate_8latebind_Curry.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_17OpenGL_accelerate_8latebind_Curry, "__init__"); if (unlikely(!wrapper)) __PYX_ERR(0, 41, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_17OpenGL_accelerate_8latebind_5Curry___init__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_17OpenGL_accelerate_8latebind_5Curry___init__.doc = __pyx_doc_17OpenGL_accelerate_8latebind_5Curry___init__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_17OpenGL_accelerate_8latebind_5Curry___init__;
     }
   }
   #endif
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_17OpenGL_accelerate_8latebind_Curry, "__call__"); if (unlikely(!wrapper)) __PYX_ERR(0, 41, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_17OpenGL_accelerate_8latebind_5Curry_2__call__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_17OpenGL_accelerate_8latebind_5Curry_2__call__.doc = __pyx_doc_17OpenGL_accelerate_8latebind_5Curry_2__call__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_17OpenGL_accelerate_8latebind_5Curry_2__call__;
     }
@@ -5387,25 +5490,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
 #endif
+    if (getstate) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+#else
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
+#endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -5442,14 +5563,16 @@
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
@@ -5577,14 +5700,20 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
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
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -5640,22 +5769,32 @@
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
@@ -6218,19 +6357,41 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
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
```

### Comparing `PyOpenGL-accelerate-3.1.6/src/latebind.pyx` & `PyOpenGL-accelerate-3.1.7/src/latebind.pyx`

 * *Files identical despite different names*

### Comparing `PyOpenGL-accelerate-3.1.6/src/nones_formathandler.c` & `PyOpenGL-accelerate-3.1.7/src/nones_formathandler.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.28 */
+/* Generated by Cython 0.29.32 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_28"
-#define CYTHON_HEX_VERSION 0x001D1CF0
+#define CYTHON_ABI "0_29_32"
+#define CYTHON_HEX_VERSION 0x001D20F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -45,14 +45,15 @@
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
@@ -81,18 +82,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
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
@@ -122,18 +127,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
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
@@ -175,15 +229,15 @@
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 0
   #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
@@ -192,14 +246,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
@@ -643,16 +700,18 @@
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
@@ -1140,14 +1199,20 @@
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
 /* ParseKeywords.proto */
 static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
     const char* function_name);
 
+/* PySequenceContains.proto */
+static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
+    int result = PySequence_Contains(seq, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* PyCFunctionFastCall.proto */
@@ -1170,14 +1235,20 @@
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
 #if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif // CYTHON_FAST_PYCALL
 #endif
@@ -1372,18 +1443,18 @@
 static const char __pyx_k_HANDLED_TYPES[] = "HANDLED_TYPES";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_pyx_unpickle_NoneHandler[] = "__pyx_unpickle_NoneHandler";
 static const char __pyx_k_Accelerator_for_None_as_an_array[] = "Accelerator for None-as-an-array format handler operations";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xf7[] = "Incompatible checksums (%s vs 0xf703739 = (ERROR_ON_COPY))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xf703739, 0xdc45998, 0x7a908a8) = (ERROR_ON_COPY))";
 static const char __pyx_k_OpenGL_accelerate_nones_formatha[] = "OpenGL_accelerate.nones_formathandler";
 static PyObject *__pyx_n_s_HANDLED_TYPES;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xf7;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
 static PyObject *__pyx_n_s_NoneHandler;
 static PyObject *__pyx_n_s_OpenGL_accelerate_nones_formatha;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_n_s_import;
@@ -1408,18 +1479,21 @@
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_pf_17OpenGL_accelerate_19nones_formathandler_11NoneHandler___reduce_cython__(struct __pyx_obj_17OpenGL_accelerate_19nones_formathandler_NoneHandler *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_17OpenGL_accelerate_19nones_formathandler_11NoneHandler_2__setstate_cython__(struct __pyx_obj_17OpenGL_accelerate_19nones_formathandler_NoneHandler *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_17OpenGL_accelerate_19nones_formathandler___pyx_unpickle_NoneHandler(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_17OpenGL_accelerate_19nones_formathandler_NoneHandler(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_0;
+static PyObject *__pyx_int_128518312;
+static PyObject *__pyx_int_230971800;
 static PyObject *__pyx_int_259012409;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_codeobj__3;
+static PyObject *__pyx_tuple__3;
+static PyObject *__pyx_codeobj__4;
 /* Late includes */
 
 /* "src/nones_formathandler.pyx":8
  * 	HANDLED_TYPES = (type(None),)
  * 
  * 	cdef c_from_param( self, object instance, object typeCode ):             # <<<<<<<<<<<<<<
  * 		"""simple function-based from_param"""
@@ -2030,151 +2104,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_19nones_formathandler___pyx_unpickle_NoneHandler(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_NoneHandler", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xf703739:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xf703739, 0xdc45998, 0x7a908a8):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf703739 = (ERROR_ON_COPY))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf703739, 0xdc45998, 0x7a908a8) = (ERROR_ON_COPY))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xf703739) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__2, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xf703739:
+ *     if __pyx_checksum not in (0xf703739, 0xdc45998, 0x7a908a8):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf703739 = (ERROR_ON_COPY))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf703739, 0xdc45998, 0x7a908a8) = (ERROR_ON_COPY))" % __pyx_checksum)
  *     __pyx_result = NoneHandler.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xf703739:
+ *     if __pyx_checksum not in (0xf703739, 0xdc45998, 0x7a908a8):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf703739 = (ERROR_ON_COPY))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf703739, 0xdc45998, 0x7a908a8) = (ERROR_ON_COPY))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = NoneHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xf7, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xf703739:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xf703739, 0xdc45998, 0x7a908a8):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf703739 = (ERROR_ON_COPY))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf703739, 0xdc45998, 0x7a908a8) = (ERROR_ON_COPY))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf703739 = (ERROR_ON_COPY))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf703739, 0xdc45998, 0x7a908a8) = (ERROR_ON_COPY))" % __pyx_checksum)
  *     __pyx_result = NoneHandler.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_NoneHandler__set_state(<NoneHandler> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_19nones_formathandler_NoneHandler), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_19nones_formathandler_NoneHandler), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf703739 = (ERROR_ON_COPY))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf703739, 0xdc45998, 0x7a908a8) = (ERROR_ON_COPY))" % __pyx_checksum)
  *     __pyx_result = NoneHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_NoneHandler__set_state(<NoneHandler> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = NoneHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_NoneHandler__set_state(<NoneHandler> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_NoneHandler__set_state(NoneHandler __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_19nones_formathandler___pyx_unpickle_NoneHandler__set_state(((struct __pyx_obj_17OpenGL_accelerate_19nones_formathandler_NoneHandler *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_19nones_formathandler___pyx_unpickle_NoneHandler__set_state(((struct __pyx_obj_17OpenGL_accelerate_19nones_formathandler_NoneHandler *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf703739 = (ERROR_ON_COPY))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf703739, 0xdc45998, 0x7a908a8) = (ERROR_ON_COPY))" % __pyx_checksum)
  *     __pyx_result = NoneHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_NoneHandler__set_state(<NoneHandler> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -2194,18 +2272,18 @@
  * def __pyx_unpickle_NoneHandler(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.nones_formathandler.__pyx_unpickle_NoneHandler", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -2483,15 +2561,15 @@
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_n_s_HANDLED_TYPES, __pyx_k_HANDLED_TYPES, sizeof(__pyx_k_HANDLED_TYPES), 0, 0, 1, 1},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xf7, __pyx_k_Incompatible_checksums_s_vs_0xf7, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xf7), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
   {&__pyx_n_s_NoneHandler, __pyx_k_NoneHandler, sizeof(__pyx_k_NoneHandler), 0, 0, 1, 1},
   {&__pyx_n_s_OpenGL_accelerate_nones_formatha, __pyx_k_OpenGL_accelerate_nones_formatha, sizeof(__pyx_k_OpenGL_accelerate_nones_formatha), 0, 0, 1, 1},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
@@ -2530,33 +2608,46 @@
  * 		"""Retrieve full set of dimensions for the array as tuple"""
  * 		return (0,)             # <<<<<<<<<<<<<<
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_int_0); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "(tree fragment)":1
- * def __pyx_unpickle_NoneHandler(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+  /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0xf703739, 0xdc45998, 0x7a908a8):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf703739, 0xdc45998, 0x7a908a8) = (ERROR_ON_COPY))" % __pyx_checksum)
  */
-  __pyx_tuple__2 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(3, __pyx_int_259012409, __pyx_int_230971800, __pyx_int_128518312); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_NoneHandler, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(1, 1, __pyx_L1_error)
+
+  /* "(tree fragment)":1
+ * def __pyx_unpickle_NoneHandler(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
+  __pyx_tuple__3 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_NoneHandler, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_128518312 = PyInt_FromLong(128518312L); if (unlikely(!__pyx_int_128518312)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_230971800 = PyInt_FromLong(230971800L); if (unlikely(!__pyx_int_230971800)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_259012409 = PyInt_FromLong(259012409L); if (unlikely(!__pyx_int_259012409)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
@@ -4045,25 +4136,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
 #endif
+    if (getstate) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+#else
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
+#endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -4100,14 +4209,16 @@
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
@@ -4235,14 +4346,20 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
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
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -4298,22 +4415,32 @@
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
@@ -4914,19 +5041,41 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
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
```

### Comparing `PyOpenGL-accelerate-3.1.6/src/nones_formathandler.pyx` & `PyOpenGL-accelerate-3.1.7/src/nones_formathandler.pyx`

 * *Files identical despite different names*

### Comparing `PyOpenGL-accelerate-3.1.6/src/numpy_formathandler.c` & `PyOpenGL-accelerate-3.1.7/src/numpy_formathandler.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.28 */
+/* Generated by Cython 0.29.32 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_28"
-#define CYTHON_HEX_VERSION 0x001D1CF0
+#define CYTHON_ABI "0_29_32"
+#define CYTHON_HEX_VERSION 0x001D20F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -45,14 +45,15 @@
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
@@ -81,18 +82,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
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
@@ -122,18 +127,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
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
@@ -175,15 +229,15 @@
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 0
   #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
@@ -192,14 +246,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
@@ -643,16 +700,18 @@
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
@@ -925,195 +984,195 @@
 static const char *__pyx_f[] = {
   "src/numpy_formathandler.pyx",
   "stringsource",
   "__init__.pxd",
   "type.pxd",
 };
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":693
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":700
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":705
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":720
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1142,42 +1201,42 @@
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 struct __pyx_obj_17OpenGL_accelerate_13formathandler_FormatHandler;
 struct __pyx_obj_17OpenGL_accelerate_19numpy_formathandler_NumpyHandler;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":733
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1361,14 +1420,20 @@
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
 #if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif // CYTHON_FAST_PYCALL
 #endif
@@ -1593,14 +1658,20 @@
 
 /* GetAttr.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
 
 /* GetAttr3.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
 
+/* PySequenceContains.proto */
+static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
+    int result = PySequence_Contains(seq, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
                __Pyx_GetItemInt_Generic(o, to_py_func(i))))
 #define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
@@ -1978,29 +2049,29 @@
 static const char __pyx_k_OpenGL_arrays_numpymodule[] = "OpenGL.arrays.numpymodule";
 static const char __pyx_k_pyx_unpickle_NumpyHandler[] = "__pyx_unpickle_NumpyHandler";
 static const char __pyx_k_Non_contiguous_array_passed[] = "Non-contiguous array passed";
 static const char __pyx_k_Array_of_type_r_passed_required[] = "Array of type %r passed, required array of type %r";
 static const char __pyx_k_Don_t_know_GL_type_for_array_of[] = "Don't know GL type for array of type %r, known types: %s\nvalue:%s";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_Accelerator_for_numpy_format_han[] = "Accelerator for numpy format handler operations";
-static const char __pyx_k_Incompatible_checksums_s_vs_0x40[] = "Incompatible checksums (%s vs 0x4048af0 = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x4048af0, 0xf213594, 0xb577e6f) = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))";
 static const char __pyx_k_Numpy_format_handler_passed_a_no[] = "Numpy format handler passed a non-numpy-array object %s (of type %s)";
 static const char __pyx_k_OpenGL_accelerate_numpy_formatha[] = "OpenGL_accelerate.numpy_formathandler";
 static const char __pyx_k_Unable_to_fill_new_array_with_va[] = "Unable to fill new array with value %r (%s)";
 static const char __pyx_k_from_param_received_a_non_contig[] = "from_param received a non-contiguous array! %s";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
 static PyObject *__pyx_n_s_ARRAY_TO_GL_TYPE_MAPPING;
 static PyObject *__pyx_kp_s_Array_of_type_r_passed_required;
 static PyObject *__pyx_n_s_CopyError;
 static PyObject *__pyx_kp_s_Don_t_know_GL_type_for_array_of;
 static PyObject *__pyx_n_s_ERROR_ON_COPY;
 static PyObject *__pyx_n_s_GL_TYPE_TO_ARRAY_MAPPING;
 static PyObject *__pyx_n_s_HANDLED_TYPES;
 static PyObject *__pyx_n_s_ImportError;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x40;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
 static PyObject *__pyx_kp_s_Non_contiguous_array_passed;
 static PyObject *__pyx_n_s_NumpyHandler;
 static PyObject *__pyx_kp_s_Numpy_format_handler_passed_a_no;
 static PyObject *__pyx_n_s_OpenGL;
 static PyObject *__pyx_n_s_OpenGL__bytes;
 static PyObject *__pyx_n_s_OpenGL_accelerate_numpy_formatha;
 static PyObject *__pyx_n_s_OpenGL_arrays_numpymodule;
@@ -2088,19 +2159,22 @@
 static PyObject *__pyx_pf_17OpenGL_accelerate_19numpy_formathandler_12NumpyHandler_4__setstate_cython__(struct __pyx_obj_17OpenGL_accelerate_19numpy_formathandler_NumpyHandler *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_17OpenGL_accelerate_19numpy_formathandler___pyx_unpickle_NumpyHandler(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_17OpenGL_accelerate_19numpy_formathandler_NumpyHandler(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_get = {0, &__pyx_n_s_get, 0, 0, 0};
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_keys = {0, &__pyx_n_s_keys, 0, 0, 0};
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_67406576;
+static PyObject *__pyx_int_190283375;
+static PyObject *__pyx_int_253834644;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
-static PyObject *__pyx_codeobj__5;
+static PyObject *__pyx_tuple__5;
+static PyObject *__pyx_codeobj__6;
 /* Late includes */
 
 /* "src/numpy_formathandler.pyx":33
  *     cdef np.npy_intp PyArray_SIZE( np.ndarray )
  * 
  * cdef np.dtype array_descr( np.ndarray array ):             # <<<<<<<<<<<<<<
  *     """Wrap PyArray_DESCR and incref to deal with the "borrowed" reference"""
@@ -5009,151 +5083,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_19numpy_formathandler___pyx_unpickle_NumpyHandler(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_NumpyHandler", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x4048af0:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x4048af0, 0xf213594, 0xb577e6f):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x4048af0 = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x4048af0, 0xf213594, 0xb577e6f) = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x4048af0) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__2, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x4048af0:
+ *     if __pyx_checksum not in (0x4048af0, 0xf213594, 0xb577e6f):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x4048af0 = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x4048af0, 0xf213594, 0xb577e6f) = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
  *     __pyx_result = NumpyHandler.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x4048af0:
+ *     if __pyx_checksum not in (0x4048af0, 0xf213594, 0xb577e6f):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x4048af0 = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x4048af0, 0xf213594, 0xb577e6f) = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = NumpyHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x40, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x4048af0:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x4048af0, 0xf213594, 0xb577e6f):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x4048af0 = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x4048af0, 0xf213594, 0xb577e6f) = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x4048af0 = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x4048af0, 0xf213594, 0xb577e6f) = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
  *     __pyx_result = NumpyHandler.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_NumpyHandler__set_state(<NumpyHandler> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_19numpy_formathandler_NumpyHandler), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_19numpy_formathandler_NumpyHandler), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x4048af0 = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x4048af0, 0xf213594, 0xb577e6f) = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
  *     __pyx_result = NumpyHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_NumpyHandler__set_state(<NumpyHandler> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = NumpyHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_NumpyHandler__set_state(<NumpyHandler> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_NumpyHandler__set_state(NumpyHandler __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_19numpy_formathandler___pyx_unpickle_NumpyHandler__set_state(((struct __pyx_obj_17OpenGL_accelerate_19numpy_formathandler_NumpyHandler *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_19numpy_formathandler___pyx_unpickle_NumpyHandler__set_state(((struct __pyx_obj_17OpenGL_accelerate_19numpy_formathandler_NumpyHandler *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x4048af0 = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x4048af0, 0xf213594, 0xb577e6f) = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
  *     __pyx_result = NumpyHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_NumpyHandler__set_state(<NumpyHandler> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -5173,18 +5251,18 @@
  * def __pyx_unpickle_NumpyHandler(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.numpy_formathandler.__pyx_unpickle_NumpyHandler", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -5342,15 +5420,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":735
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5359,29 +5437,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":736
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 736, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5392,15 +5470,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":738
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5409,29 +5487,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":739
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 739, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5442,15 +5520,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":741
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5459,29 +5537,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":742
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 742, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5492,15 +5570,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":744
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5509,29 +5587,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":745
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 745, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5542,15 +5620,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":747
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5559,29 +5637,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":748
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 748, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5592,212 +5670,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":750
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":749
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
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":751
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":752
+    /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":751
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
 
-    /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":754
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":749
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
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":929
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":933
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":935
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":936
+    /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":941
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5813,15 +5891,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -5829,84 +5907,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":943
+      /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 943, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 942, __pyx_L3_error)
 
-      /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 944, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 945, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 945, __pyx_L5_except_error)
+      __PYX_ERR(2, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":942
+    /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5921,15 +5999,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":947
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5945,15 +6023,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5961,84 +6039,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":949
+      /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 949, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 948, __pyx_L3_error)
 
-      /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":947
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
 
-    /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 950, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 951, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 951, __pyx_L5_except_error)
+      __PYX_ERR(2, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":948
+    /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":947
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
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6053,15 +6131,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":953
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6077,15 +6155,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":954
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6093,84 +6171,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":955
+      /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 955, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 954, __pyx_L3_error)
 
-      /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":953
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
 
-    /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":956
+    /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 956, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":957
+      /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 957, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 957, __pyx_L5_except_error)
+      __PYX_ERR(2, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":954
+    /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":953
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
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6185,176 +6263,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":967
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":967
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":982
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":982
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":997
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":997
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+/* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":1018
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -6578,15 +6656,15 @@
   {&__pyx_kp_s_Array_of_type_r_passed_required, __pyx_k_Array_of_type_r_passed_required, sizeof(__pyx_k_Array_of_type_r_passed_required), 0, 0, 1, 0},
   {&__pyx_n_s_CopyError, __pyx_k_CopyError, sizeof(__pyx_k_CopyError), 0, 0, 1, 1},
   {&__pyx_kp_s_Don_t_know_GL_type_for_array_of, __pyx_k_Don_t_know_GL_type_for_array_of, sizeof(__pyx_k_Don_t_know_GL_type_for_array_of), 0, 0, 1, 0},
   {&__pyx_n_s_ERROR_ON_COPY, __pyx_k_ERROR_ON_COPY, sizeof(__pyx_k_ERROR_ON_COPY), 0, 0, 1, 1},
   {&__pyx_n_s_GL_TYPE_TO_ARRAY_MAPPING, __pyx_k_GL_TYPE_TO_ARRAY_MAPPING, sizeof(__pyx_k_GL_TYPE_TO_ARRAY_MAPPING), 0, 0, 1, 1},
   {&__pyx_n_s_HANDLED_TYPES, __pyx_k_HANDLED_TYPES, sizeof(__pyx_k_HANDLED_TYPES), 0, 0, 1, 1},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x40, __pyx_k_Incompatible_checksums_s_vs_0x40, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x40), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
   {&__pyx_kp_s_Non_contiguous_array_passed, __pyx_k_Non_contiguous_array_passed, sizeof(__pyx_k_Non_contiguous_array_passed), 0, 0, 1, 0},
   {&__pyx_n_s_NumpyHandler, __pyx_k_NumpyHandler, sizeof(__pyx_k_NumpyHandler), 0, 0, 1, 1},
   {&__pyx_kp_s_Numpy_format_handler_passed_a_no, __pyx_k_Numpy_format_handler_passed_a_no, sizeof(__pyx_k_Numpy_format_handler_passed_a_no), 0, 0, 1, 0},
   {&__pyx_n_s_OpenGL, __pyx_k_OpenGL, sizeof(__pyx_k_OpenGL), 0, 0, 1, 1},
   {&__pyx_n_s_OpenGL__bytes, __pyx_k_OpenGL__bytes, sizeof(__pyx_k_OpenGL__bytes), 0, 0, 1, 1},
   {&__pyx_n_s_OpenGL_accelerate_numpy_formatha, __pyx_k_OpenGL_accelerate_numpy_formatha, sizeof(__pyx_k_OpenGL_accelerate_numpy_formatha), 0, 0, 1, 1},
   {&__pyx_n_s_OpenGL_arrays_numpymodule, __pyx_k_OpenGL_arrays_numpymodule, sizeof(__pyx_k_OpenGL_arrays_numpymodule), 0, 0, 1, 1},
@@ -6664,15 +6742,15 @@
   {&__pyx_n_s_void, __pyx_k_void, sizeof(__pyx_k_void), 0, 0, 1, 1},
   {&__pyx_n_s_weakref, __pyx_k_weakref, sizeof(__pyx_k_weakref), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 90, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 124, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 945, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 944, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -6685,58 +6763,71 @@
  *             res = PyArray_FillWithScalar(<object>working, instance)
  *             if res < -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_int_1); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "(tree fragment)":4
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0x4048af0, 0xf213594, 0xb577e6f):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x4048af0, 0xf213594, 0xb577e6f) = (ERROR_ON_COPY, array_to_gl_constant, gl_constant_to_array))" % __pyx_checksum)
+ */
+  __pyx_tuple__2 = PyTuple_Pack(3, __pyx_int_67406576, __pyx_int_253834644, __pyx_int_190283375); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
+
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(2, 945, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(2, 944, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(2, 951, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(2, 950, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_NumpyHandler(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__4 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_NumpyHandler, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_NumpyHandler, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   __pyx_umethod_PyDict_Type_get.type = (PyObject*)&PyDict_Type;
   __pyx_umethod_PyDict_Type_keys.type = (PyObject*)&PyDict_Type;
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_67406576 = PyInt_FromLong(67406576L); if (unlikely(!__pyx_int_67406576)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_190283375 = PyInt_FromLong(190283375L); if (unlikely(!__pyx_int_190283375)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_253834644 = PyInt_FromLong(253834644L); if (unlikely(!__pyx_int_253834644)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -6833,46 +6924,46 @@
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 200, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 200, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 223, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 227, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
   __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 771, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
   __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 773, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
   __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 775, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
   __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 777, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
   __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 779, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
   __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 781, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
   __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 783, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
   __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 785, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
   __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 787, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
   __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 789, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 827, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -7733,15 +7824,15 @@
  * import numpy as np
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/pip-build-env-mft82qvr/overlay/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -9285,25 +9376,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
 #endif
+    if (getstate) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+#else
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
+#endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -9340,14 +9449,16 @@
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
@@ -9495,14 +9606,20 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
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
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -9558,22 +9675,32 @@
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
@@ -10482,19 +10609,41 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
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
```

### Comparing `PyOpenGL-accelerate-3.1.6/src/numpy_formathandler.pyx` & `PyOpenGL-accelerate-3.1.7/src/numpy_formathandler.pyx`

 * *Files identical despite different names*

### Comparing `PyOpenGL-accelerate-3.1.6/src/vbo.c` & `PyOpenGL-accelerate-3.1.7/src/vbo.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.28 */
+/* Generated by Cython 0.29.32 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_28"
-#define CYTHON_HEX_VERSION 0x001D1CF0
+#define CYTHON_ABI "0_29_32"
+#define CYTHON_HEX_VERSION 0x001D20F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -45,14 +45,15 @@
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
@@ -81,18 +82,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
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
@@ -122,18 +127,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
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
@@ -175,15 +229,15 @@
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 0
   #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
@@ -192,14 +246,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
@@ -643,16 +700,18 @@
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
@@ -1171,14 +1230,20 @@
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
 #if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif // CYTHON_FAST_PYCALL
 #endif
@@ -1467,14 +1532,20 @@
 
 /* ExtTypeTest.proto */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
 
 /* KeywordStringCheck.proto */
 static int __Pyx_CheckKeywordStrings(PyObject *kwdict, const char* function_name, int kw_allowed);
 
+/* PySequenceContains.proto */
+static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
+    int result = PySequence_Contains(seq, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
 /* PyObject_GenericGetAttrNoDict.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
 #endif
 
@@ -1722,32 +1793,32 @@
 static const char __pyx_k_OpenGL_arrays_arraydatatype[] = "OpenGL.arrays.arraydatatype";
 static const char __pyx_k_pyx_unpickle_VBOOffsetHandler[] = "__pyx_unpickle_VBOOffsetHandler";
 static const char __pyx_k_Attempting_to_use_a_deleted_VBO[] = "Attempting to use a deleted VBO";
 static const char __pyx_k_Cython_coded_VBO_implementation[] = "Cython-coded VBO implementation";
 static const char __pyx_k_Should_do_create_buffers_before[] = "Should do create_buffers before copy_data";
 static const char __pyx_k_Attempting_to_use_offset_into_de[] = "Attempting to use offset into deleted VBO";
 static const char __pyx_k_Don_t_know_how_to_map_stepped_ar[] = "Don't know how to map stepped arrays yet";
-static const char __pyx_k_Incompatible_checksums_s_vs_0x0f[] = "Incompatible checksums (%s vs 0x0fed755 = (_I_, _copy_segments, arrayType, buffer, copied, created, data, resolved, size, target, target_spec, usage, usage_spec))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xad[] = "Incompatible checksums (%s vs 0xaddf131 = (ERROR_ON_COPY, arrayType, vp0))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xe0[] = "Incompatible checksums (%s vs 0xe0a0c83 = (ERROR_ON_COPY, arrayType))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x0fed755, 0xc23cd69, 0xd9c0226) = (_I_, _copy_segments, arrayType, buffer, copied, created, data, resolved, size, target, target_spec, usage, usage_spec))";
 static const char __pyx_k_Only_know_how_to_add_integer_lon[] = "Only know how to add integer/long offsets";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_2[] = "Incompatible checksums (0x%x vs (0xaddf131, 0x8b69ded, 0x7370e1d) = (ERROR_ON_COPY, arrayType, vp0))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_3[] = "Incompatible checksums (0x%x vs (0xe0a0c83, 0x3e55b0f, 0x0464fd9) = (ERROR_ON_COPY, arrayType))";
 static PyObject *__pyx_kp_s_Already_created_the_buffer;
 static PyObject *__pyx_n_s_ArrayDatatype;
 static PyObject *__pyx_kp_s_Attempting_to_use_a_deleted_VBO;
 static PyObject *__pyx_kp_s_Attempting_to_use_offset_into_de;
 static PyObject *__pyx_n_s_AttributeError;
 static PyObject *__pyx_n_s_DELETERS;
 static PyObject *__pyx_kp_s_Don_t_know_how_to_map_stepped_ar;
 static PyObject *__pyx_n_s_GL_ARRAY_BUFFER;
 static PyObject *__pyx_n_s_GL_DYNAMIC_DRAW;
 static PyObject *__pyx_n_s_I;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x0f;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xad;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xe0;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_3;
 static PyObject *__pyx_n_s_KeyError;
 static PyObject *__pyx_n_s_NULL;
 static PyObject *__pyx_kp_s_No_r_key_in_VBOOffset;
 static PyObject *__pyx_n_s_NotImplemented;
 static PyObject *__pyx_n_s_NullFunctionError;
 static PyObject *__pyx_kp_s_Only_know_how_to_add_integer_lon;
 static PyObject *__pyx_n_s_OpenGL;
@@ -1912,42 +1983,51 @@
 static PyObject *__pyx_pf_17OpenGL_accelerate_3vbo_4__pyx_unpickle_VBOOffsetHandler(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_17OpenGL_accelerate_3vbo_VBO(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_17OpenGL_accelerate_3vbo_VBOOffset(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_17OpenGL_accelerate_3vbo_VBOHandler(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_17OpenGL_accelerate_3vbo_VBOOffsetHandler(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
+static PyObject *__pyx_int_4607961;
 static PyObject *__pyx_int_16701269;
+static PyObject *__pyx_int_65362703;
+static PyObject *__pyx_int_121048605;
+static PyObject *__pyx_int_146185709;
 static PyObject *__pyx_int_182317361;
+static PyObject *__pyx_int_203672937;
+static PyObject *__pyx_int_228327974;
 static PyObject *__pyx_int_235539587;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
+static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_tuple__10;
-static PyObject *__pyx_codeobj__7;
-static PyObject *__pyx_codeobj__9;
-static PyObject *__pyx_codeobj__11;
+static PyObject *__pyx_tuple__9;
+static PyObject *__pyx_tuple__11;
+static PyObject *__pyx_tuple__13;
+static PyObject *__pyx_codeobj__10;
+static PyObject *__pyx_codeobj__12;
+static PyObject *__pyx_codeobj__14;
 /* Late includes */
 
 /* "src/vbo.pyx":49
  *     cdef public object arrayType
  *     _no_cache_ = True # do not cache in context data arrays
  *     def __init__(             # <<<<<<<<<<<<<<
  *         self, data, usage='GL_DYNAMIC_DRAW',
  *         target='GL_ARRAY_BUFFER',
  */
 
 /* Python wrapper */
 static int __pyx_pw_17OpenGL_accelerate_3vbo_3VBO_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_17OpenGL_accelerate_3vbo_3VBO___init__[] = "Initialize the VBO\n\n        data -- array-compatible data format object\n\n        usage -- string/GLenum constant specifying streaming usage\n            for the VBO, normal values:\n\n                GL_STREAM_DRAW -- updated every frame from client to card\n                GL_STREAM_COPY -- read and written from card each frame\n\n                GL_STATIC_DRAW -- just written from client (once)\n                GL_STATIC_READ -- just read from client\n                GL_STATIC_COPY -- read and written from client (once)\n\n                GL_DYNAMIC_DRAW -- updated from client every once in a while\n                GL_DYNAMIC_COPY -- read and written from client every once in a while\n                GL_DYNAMIC_READ -- read from the client every once in a while\n\n        target -- string/GLenum constant specifying the role for the buffer\n            normal values:\n\n                GL_ARRAY_BUFFER -- vertex attribute values\n                GL_ELEMENT_ARRAY_BUFFER -- vertex index values\n                GL_PIXEL_PACK_BUFFER/GL_PIXEL_UNPACK_BUFFER -- client-side\n                    image source/sink for image-manipulation operations.\n        ";
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_17OpenGL_accelerate_3vbo_3VBO___init__;
 #endif
 static int __pyx_pw_17OpenGL_accelerate_3vbo_3VBO_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_data = 0;
   PyObject *__pyx_v_usage = 0;
   PyObject *__pyx_v_target = 0;
   PyObject *__pyx_v_size = 0;
@@ -2920,15 +3000,15 @@
  *         """Set slice of data on the array and vbo (if copied already)
  * 
  */
 
 /* Python wrapper */
 static int __pyx_pw_17OpenGL_accelerate_3vbo_3VBO_7__setitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_slice, PyObject *__pyx_v_array); /*proto*/
 static char __pyx_doc_17OpenGL_accelerate_3vbo_3VBO_6__setitem__[] = "Set slice of data on the array and vbo (if copied already)\n\n        slice -- the Python slice object determining how the data should\n            be copied into the vbo/array\n        array -- something array-compatible that will be used as the\n            source of the data, note that the data-format will have to\n            be the same as the internal data-array to work properly, if\n            not, the amount of data copied will be wrong.\n\n        This is a reasonably complex operation, it has to have all sorts\n        of state-aware changes to correctly map the source into the low-level\n        OpenGL view of the buffer (which is just bytes as far as the GL\n        is concerned).\n        ";
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_17OpenGL_accelerate_3vbo_3VBO_6__setitem__;
 #endif
 static int __pyx_pw_17OpenGL_accelerate_3vbo_3VBO_7__setitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_slice, PyObject *__pyx_v_array) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setitem__ (wrapper)", 0);
   __pyx_r = __pyx_pf_17OpenGL_accelerate_3vbo_3VBO_6__setitem__(((struct __pyx_obj_17OpenGL_accelerate_3vbo_VBO *)__pyx_v_self), ((PyObject *)__pyx_v_slice), ((PyObject *)__pyx_v_array));
@@ -3681,15 +3761,15 @@
  *         """Get our VBO id"""
  *         if not self.buffer:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_17OpenGL_accelerate_3vbo_3VBO_13__int__(PyObject *__pyx_v_self); /*proto*/
 static char __pyx_doc_17OpenGL_accelerate_3vbo_3VBO_12__int__[] = "Get our VBO id";
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_17OpenGL_accelerate_3vbo_3VBO_12__int__;
 #endif
 static PyObject *__pyx_pw_17OpenGL_accelerate_3vbo_3VBO_13__int__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__int__ (wrapper)", 0);
   __pyx_r = __pyx_pf_17OpenGL_accelerate_3vbo_3VBO_12__int__(((struct __pyx_obj_17OpenGL_accelerate_3vbo_VBO *)__pyx_v_self));
@@ -5331,15 +5411,15 @@
  *         """Add an integer to this VBO (offset)"""
  *         if hasattr( other, 'offset' ):
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_17OpenGL_accelerate_3vbo_3VBO_25__add__(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
 static char __pyx_doc_17OpenGL_accelerate_3vbo_3VBO_24__add__[] = "Add an integer to this VBO (offset)";
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_17OpenGL_accelerate_3vbo_3VBO_24__add__;
 #endif
 static PyObject *__pyx_pw_17OpenGL_accelerate_3vbo_3VBO_25__add__(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__add__ (wrapper)", 0);
   __pyx_r = __pyx_pf_17OpenGL_accelerate_3vbo_3VBO_24__add__(((PyObject *)__pyx_v_self), ((PyObject *)__pyx_v_other));
@@ -10140,151 +10220,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_3vbo___pyx_unpickle_VBO(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_VBO", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x0fed755:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x0fed755, 0xc23cd69, 0xd9c0226):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x0fed755 = (_I_, _copy_segments, arrayType, buffer, copied, created, data, resolved, size, target, target_spec, usage, usage_spec))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x0fed755, 0xc23cd69, 0xd9c0226) = (_I_, _copy_segments, arrayType, buffer, copied, created, data, resolved, size, target, target_spec, usage, usage_spec))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x0fed755) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__6, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x0fed755:
+ *     if __pyx_checksum not in (0x0fed755, 0xc23cd69, 0xd9c0226):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x0fed755 = (_I_, _copy_segments, arrayType, buffer, copied, created, data, resolved, size, target, target_spec, usage, usage_spec))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x0fed755, 0xc23cd69, 0xd9c0226) = (_I_, _copy_segments, arrayType, buffer, copied, created, data, resolved, size, target, target_spec, usage, usage_spec))" % __pyx_checksum)
  *     __pyx_result = VBO.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x0fed755:
+ *     if __pyx_checksum not in (0x0fed755, 0xc23cd69, 0xd9c0226):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x0fed755 = (_I_, _copy_segments, arrayType, buffer, copied, created, data, resolved, size, target, target_spec, usage, usage_spec))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x0fed755, 0xc23cd69, 0xd9c0226) = (_I_, _copy_segments, arrayType, buffer, copied, created, data, resolved, size, target, target_spec, usage, usage_spec))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = VBO.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x0f, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x0fed755:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x0fed755, 0xc23cd69, 0xd9c0226):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x0fed755 = (_I_, _copy_segments, arrayType, buffer, copied, created, data, resolved, size, target, target_spec, usage, usage_spec))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x0fed755, 0xc23cd69, 0xd9c0226) = (_I_, _copy_segments, arrayType, buffer, copied, created, data, resolved, size, target, target_spec, usage, usage_spec))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x0fed755 = (_I_, _copy_segments, arrayType, buffer, copied, created, data, resolved, size, target, target_spec, usage, usage_spec))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x0fed755, 0xc23cd69, 0xd9c0226) = (_I_, _copy_segments, arrayType, buffer, copied, created, data, resolved, size, target, target_spec, usage, usage_spec))" % __pyx_checksum)
  *     __pyx_result = VBO.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_VBO__set_state(<VBO> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_3vbo_VBO), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_3vbo_VBO), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x0fed755 = (_I_, _copy_segments, arrayType, buffer, copied, created, data, resolved, size, target, target_spec, usage, usage_spec))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x0fed755, 0xc23cd69, 0xd9c0226) = (_I_, _copy_segments, arrayType, buffer, copied, created, data, resolved, size, target, target_spec, usage, usage_spec))" % __pyx_checksum)
  *     __pyx_result = VBO.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_VBO__set_state(<VBO> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = VBO.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_VBO__set_state(<VBO> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_VBO__set_state(VBO __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_3vbo___pyx_unpickle_VBO__set_state(((struct __pyx_obj_17OpenGL_accelerate_3vbo_VBO *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_3vbo___pyx_unpickle_VBO__set_state(((struct __pyx_obj_17OpenGL_accelerate_3vbo_VBO *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x0fed755 = (_I_, _copy_segments, arrayType, buffer, copied, created, data, resolved, size, target, target_spec, usage, usage_spec))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x0fed755, 0xc23cd69, 0xd9c0226) = (_I_, _copy_segments, arrayType, buffer, copied, created, data, resolved, size, target, target_spec, usage, usage_spec))" % __pyx_checksum)
  *     __pyx_result = VBO.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_VBO__set_state(<VBO> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -10304,18 +10388,18 @@
  * def __pyx_unpickle_VBO(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.vbo.__pyx_unpickle_VBO", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -10662,151 +10746,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_3vbo_2__pyx_unpickle_VBOHandler(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_VBOHandler", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xaddf131:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xaddf131, 0x8b69ded, 0x7370e1d):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xaddf131 = (ERROR_ON_COPY, arrayType, vp0))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xaddf131, 0x8b69ded, 0x7370e1d) = (ERROR_ON_COPY, arrayType, vp0))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xaddf131) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__7, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xaddf131:
+ *     if __pyx_checksum not in (0xaddf131, 0x8b69ded, 0x7370e1d):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xaddf131 = (ERROR_ON_COPY, arrayType, vp0))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xaddf131, 0x8b69ded, 0x7370e1d) = (ERROR_ON_COPY, arrayType, vp0))" % __pyx_checksum)
  *     __pyx_result = VBOHandler.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xaddf131:
+ *     if __pyx_checksum not in (0xaddf131, 0x8b69ded, 0x7370e1d):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xaddf131 = (ERROR_ON_COPY, arrayType, vp0))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xaddf131, 0x8b69ded, 0x7370e1d) = (ERROR_ON_COPY, arrayType, vp0))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = VBOHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xad, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xaddf131:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xaddf131, 0x8b69ded, 0x7370e1d):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xaddf131 = (ERROR_ON_COPY, arrayType, vp0))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xaddf131, 0x8b69ded, 0x7370e1d) = (ERROR_ON_COPY, arrayType, vp0))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xaddf131 = (ERROR_ON_COPY, arrayType, vp0))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xaddf131, 0x8b69ded, 0x7370e1d) = (ERROR_ON_COPY, arrayType, vp0))" % __pyx_checksum)
  *     __pyx_result = VBOHandler.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_VBOHandler__set_state(<VBOHandler> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_3vbo_VBOHandler), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_3vbo_VBOHandler), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xaddf131 = (ERROR_ON_COPY, arrayType, vp0))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xaddf131, 0x8b69ded, 0x7370e1d) = (ERROR_ON_COPY, arrayType, vp0))" % __pyx_checksum)
  *     __pyx_result = VBOHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_VBOHandler__set_state(<VBOHandler> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = VBOHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_VBOHandler__set_state(<VBOHandler> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_VBOHandler__set_state(VBOHandler __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_3vbo___pyx_unpickle_VBOHandler__set_state(((struct __pyx_obj_17OpenGL_accelerate_3vbo_VBOHandler *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_3vbo___pyx_unpickle_VBOHandler__set_state(((struct __pyx_obj_17OpenGL_accelerate_3vbo_VBOHandler *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xaddf131 = (ERROR_ON_COPY, arrayType, vp0))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xaddf131, 0x8b69ded, 0x7370e1d) = (ERROR_ON_COPY, arrayType, vp0))" % __pyx_checksum)
  *     __pyx_result = VBOHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_VBOHandler__set_state(<VBOHandler> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -10826,18 +10914,18 @@
  * def __pyx_unpickle_VBOHandler(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.vbo.__pyx_unpickle_VBOHandler", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -11080,151 +11168,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_3vbo_4__pyx_unpickle_VBOOffsetHandler(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_VBOOffsetHandler", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe0a0c83:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xe0a0c83, 0x3e55b0f, 0x0464fd9):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe0a0c83 = (ERROR_ON_COPY, arrayType))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe0a0c83, 0x3e55b0f, 0x0464fd9) = (ERROR_ON_COPY, arrayType))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xe0a0c83) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__8, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe0a0c83:
+ *     if __pyx_checksum not in (0xe0a0c83, 0x3e55b0f, 0x0464fd9):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe0a0c83 = (ERROR_ON_COPY, arrayType))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe0a0c83, 0x3e55b0f, 0x0464fd9) = (ERROR_ON_COPY, arrayType))" % __pyx_checksum)
  *     __pyx_result = VBOOffsetHandler.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xe0a0c83:
+ *     if __pyx_checksum not in (0xe0a0c83, 0x3e55b0f, 0x0464fd9):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe0a0c83 = (ERROR_ON_COPY, arrayType))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe0a0c83, 0x3e55b0f, 0x0464fd9) = (ERROR_ON_COPY, arrayType))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = VBOOffsetHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xe0, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe0a0c83:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xe0a0c83, 0x3e55b0f, 0x0464fd9):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe0a0c83 = (ERROR_ON_COPY, arrayType))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe0a0c83, 0x3e55b0f, 0x0464fd9) = (ERROR_ON_COPY, arrayType))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe0a0c83 = (ERROR_ON_COPY, arrayType))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe0a0c83, 0x3e55b0f, 0x0464fd9) = (ERROR_ON_COPY, arrayType))" % __pyx_checksum)
  *     __pyx_result = VBOOffsetHandler.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_VBOOffsetHandler__set_state(<VBOOffsetHandler> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_3vbo_VBOOffsetHandler), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_3vbo_VBOOffsetHandler), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe0a0c83 = (ERROR_ON_COPY, arrayType))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe0a0c83, 0x3e55b0f, 0x0464fd9) = (ERROR_ON_COPY, arrayType))" % __pyx_checksum)
  *     __pyx_result = VBOOffsetHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_VBOOffsetHandler__set_state(<VBOOffsetHandler> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = VBOOffsetHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_VBOOffsetHandler__set_state(<VBOOffsetHandler> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_VBOOffsetHandler__set_state(VBOOffsetHandler __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_3vbo___pyx_unpickle_VBOOffsetHandler__set_state(((struct __pyx_obj_17OpenGL_accelerate_3vbo_VBOOffsetHandler *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_3vbo___pyx_unpickle_VBOOffsetHandler__set_state(((struct __pyx_obj_17OpenGL_accelerate_3vbo_VBOOffsetHandler *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe0a0c83 = (ERROR_ON_COPY, arrayType))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe0a0c83, 0x3e55b0f, 0x0464fd9) = (ERROR_ON_COPY, arrayType))" % __pyx_checksum)
  *     __pyx_result = VBOOffsetHandler.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_VBOOffsetHandler__set_state(<VBOOffsetHandler> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -11244,18 +11336,18 @@
  * def __pyx_unpickle_VBOOffsetHandler(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.vbo.__pyx_unpickle_VBOOffsetHandler", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -12449,17 +12541,17 @@
   {&__pyx_kp_s_Attempting_to_use_offset_into_de, __pyx_k_Attempting_to_use_offset_into_de, sizeof(__pyx_k_Attempting_to_use_offset_into_de), 0, 0, 1, 0},
   {&__pyx_n_s_AttributeError, __pyx_k_AttributeError, sizeof(__pyx_k_AttributeError), 0, 0, 1, 1},
   {&__pyx_n_s_DELETERS, __pyx_k_DELETERS, sizeof(__pyx_k_DELETERS), 0, 0, 1, 1},
   {&__pyx_kp_s_Don_t_know_how_to_map_stepped_ar, __pyx_k_Don_t_know_how_to_map_stepped_ar, sizeof(__pyx_k_Don_t_know_how_to_map_stepped_ar), 0, 0, 1, 0},
   {&__pyx_n_s_GL_ARRAY_BUFFER, __pyx_k_GL_ARRAY_BUFFER, sizeof(__pyx_k_GL_ARRAY_BUFFER), 0, 0, 1, 1},
   {&__pyx_n_s_GL_DYNAMIC_DRAW, __pyx_k_GL_DYNAMIC_DRAW, sizeof(__pyx_k_GL_DYNAMIC_DRAW), 0, 0, 1, 1},
   {&__pyx_n_s_I, __pyx_k_I, sizeof(__pyx_k_I), 0, 0, 1, 1},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x0f, __pyx_k_Incompatible_checksums_s_vs_0x0f, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x0f), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xad, __pyx_k_Incompatible_checksums_s_vs_0xad, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xad), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xe0, __pyx_k_Incompatible_checksums_s_vs_0xe0, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xe0), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2, __pyx_k_Incompatible_checksums_0x_x_vs_0_2, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_2), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_3, __pyx_k_Incompatible_checksums_0x_x_vs_0_3, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_3), 0, 0, 1, 0},
   {&__pyx_n_s_KeyError, __pyx_k_KeyError, sizeof(__pyx_k_KeyError), 0, 0, 1, 1},
   {&__pyx_n_s_NULL, __pyx_k_NULL, sizeof(__pyx_k_NULL), 0, 0, 1, 1},
   {&__pyx_kp_s_No_r_key_in_VBOOffset, __pyx_k_No_r_key_in_VBOOffset, sizeof(__pyx_k_No_r_key_in_VBOOffset), 0, 0, 1, 0},
   {&__pyx_n_s_NotImplemented, __pyx_k_NotImplemented, sizeof(__pyx_k_NotImplemented), 0, 0, 1, 1},
   {&__pyx_n_s_NullFunctionError, __pyx_k_NullFunctionError, sizeof(__pyx_k_NullFunctionError), 0, 0, 1, 1},
   {&__pyx_kp_s_Only_know_how_to_add_integer_lon, __pyx_k_Only_know_how_to_add_integer_lon, sizeof(__pyx_k_Only_know_how_to_add_integer_lon), 0, 0, 1, 0},
   {&__pyx_n_s_OpenGL, __pyx_k_OpenGL, sizeof(__pyx_k_OpenGL), 0, 0, 1, 1},
@@ -12618,45 +12710,60 @@
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_tuple__6 = PyTuple_Pack(3, __pyx_int_16701269, __pyx_int_203672937, __pyx_int_228327974); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_tuple__7 = PyTuple_Pack(3, __pyx_int_182317361, __pyx_int_146185709, __pyx_int_121048605); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_235539587, __pyx_int_65362703, __pyx_int_4607961); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_VBO(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__6 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_VBO, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__8 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_VBOHandler, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__10 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_VBOOffsetHandler, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_VBO, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_VBOHandler, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_VBOOffsetHandler, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_4607961 = PyInt_FromLong(4607961L); if (unlikely(!__pyx_int_4607961)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_16701269 = PyInt_FromLong(16701269L); if (unlikely(!__pyx_int_16701269)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_65362703 = PyInt_FromLong(65362703L); if (unlikely(!__pyx_int_65362703)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_121048605 = PyInt_FromLong(121048605L); if (unlikely(!__pyx_int_121048605)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_146185709 = PyInt_FromLong(146185709L); if (unlikely(!__pyx_int_146185709)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_182317361 = PyInt_FromLong(182317361L); if (unlikely(!__pyx_int_182317361)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_203672937 = PyInt_FromLong(203672937L); if (unlikely(!__pyx_int_203672937)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_228327974 = PyInt_FromLong(228327974L); if (unlikely(!__pyx_int_228327974)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_235539587 = PyInt_FromLong(235539587L); if (unlikely(!__pyx_int_235539587)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
@@ -12704,45 +12811,45 @@
   __pyx_vtable_17OpenGL_accelerate_3vbo_VBO.c_resolve = (unsigned int (*)(struct __pyx_obj_17OpenGL_accelerate_3vbo_VBO *, PyObject *))__pyx_f_17OpenGL_accelerate_3vbo_3VBO_c_resolve;
   __pyx_vtable_17OpenGL_accelerate_3vbo_VBO.c_set_array = (PyObject *(*)(struct __pyx_obj_17OpenGL_accelerate_3vbo_VBO *, PyObject *, PyObject *))__pyx_f_17OpenGL_accelerate_3vbo_3VBO_c_set_array;
   __pyx_vtable_17OpenGL_accelerate_3vbo_VBO.check_live = (int (*)(struct __pyx_obj_17OpenGL_accelerate_3vbo_VBO *))__pyx_f_17OpenGL_accelerate_3vbo_3VBO_check_live;
   if (PyType_Ready(&__pyx_type_17OpenGL_accelerate_3vbo_VBO) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_17OpenGL_accelerate_3vbo_VBO.tp_print = 0;
   #endif
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_17OpenGL_accelerate_3vbo_VBO, "__init__"); if (unlikely(!wrapper)) __PYX_ERR(0, 13, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_17OpenGL_accelerate_3vbo_3VBO___init__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_17OpenGL_accelerate_3vbo_3VBO___init__.doc = __pyx_doc_17OpenGL_accelerate_3vbo_3VBO___init__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_17OpenGL_accelerate_3vbo_3VBO___init__;
     }
   }
   #endif
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_17OpenGL_accelerate_3vbo_VBO, "__setitem__"); if (unlikely(!wrapper)) __PYX_ERR(0, 13, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_17OpenGL_accelerate_3vbo_3VBO_6__setitem__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_17OpenGL_accelerate_3vbo_3VBO_6__setitem__.doc = __pyx_doc_17OpenGL_accelerate_3vbo_3VBO_6__setitem__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_17OpenGL_accelerate_3vbo_3VBO_6__setitem__;
     }
   }
   #endif
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_17OpenGL_accelerate_3vbo_VBO, "__int__"); if (unlikely(!wrapper)) __PYX_ERR(0, 13, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_17OpenGL_accelerate_3vbo_3VBO_12__int__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_17OpenGL_accelerate_3vbo_3VBO_12__int__.doc = __pyx_doc_17OpenGL_accelerate_3vbo_3VBO_12__int__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_17OpenGL_accelerate_3vbo_3VBO_12__int__;
     }
   }
   #endif
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_17OpenGL_accelerate_3vbo_VBO, "__add__"); if (unlikely(!wrapper)) __PYX_ERR(0, 13, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_17OpenGL_accelerate_3vbo_3VBO_24__add__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_17OpenGL_accelerate_3vbo_3VBO_24__add__.doc = __pyx_doc_17OpenGL_accelerate_3vbo_3VBO_24__add__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_17OpenGL_accelerate_3vbo_3VBO_24__add__;
     }
@@ -14241,15 +14348,15 @@
         ps2 = PyBytes_AS_STRING(s2);
         if (ps1[0] != ps2[0]) {
             return (equals == Py_NE);
         } else if (length == 1) {
             return (equals == Py_EQ);
         } else {
             int result;
-#if CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
             Py_hash_t hash1, hash2;
             hash1 = ((PyBytesObject*)s1)->ob_shash;
             hash2 = ((PyBytesObject*)s2)->ob_shash;
             if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
                 return (equals == Py_NE);
             }
 #endif
@@ -15085,25 +15192,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
+#if CYTHON_USE_PYTYPE_LOOKUP
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
+#else
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
+#endif
+    if (getstate) {
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
 #endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -15140,14 +15265,16 @@
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
@@ -15376,14 +15503,20 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
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
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -15439,22 +15572,32 @@
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
@@ -16189,19 +16332,41 @@
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
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
```

### Comparing `PyOpenGL-accelerate-3.1.6/src/vbo.pyx` & `PyOpenGL-accelerate-3.1.7/src/vbo.pyx`

 * *Files identical despite different names*

### Comparing `PyOpenGL-accelerate-3.1.6/src/wrapper.c` & `PyOpenGL-accelerate-3.1.7/src/wrapper.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.28 */
+/* Generated by Cython 0.29.32 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_28"
-#define CYTHON_HEX_VERSION 0x001D1CF0
+#define CYTHON_ABI "0_29_32"
+#define CYTHON_HEX_VERSION 0x001D20F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -45,14 +45,15 @@
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
@@ -81,18 +82,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
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
@@ -122,18 +127,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
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
@@ -175,15 +229,15 @@
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 0
   #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
@@ -192,14 +246,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
@@ -643,16 +700,18 @@
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
@@ -1583,14 +1642,20 @@
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
 #if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif // CYTHON_FAST_PYCALL
 #endif
@@ -1760,14 +1825,20 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
+/* PySequenceContains.proto */
+static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
+    int result = PySequence_Contains(seq, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* CallNextTpTraverse.proto */
@@ -2019,47 +2090,47 @@
 static const char __pyx_k_pyx_unpickle_PyArgCalculatorEl[] = "__pyx_unpickle_PyArgCalculatorElement";
 static const char __pyx_k_pyx_unpickle_cArgumentConverte[] = "__pyx_unpickle_cArgumentConverter";
 static const char __pyx_k_pyx_unpickle_returnPyArgumentI[] = "__pyx_unpickle_returnPyArgumentIndex";
 static const char __pyx_k_s_requires_r_arguments_s_receiv[] = "%s requires %r arguments (%s), received %s: %r";
 static const char __pyx_k_Cython_coded_implementation_of_w[] = "Cython-coded implementation of wrapper module";
 static const char __pyx_k_Expected_parameter_index_r_but_p[] = "Expected parameter index %r, but pyArgs only length %s";
 static const char __pyx_k_Expected_s_C_arguments_for_resol[] = "Expected %s C arguments for resolution, got %s";
-static const char __pyx_k_Incompatible_checksums_s_vs_0x08[] = "Incompatible checksums (%s vs 0x087f810 = (index, name))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0x26[] = "Incompatible checksums (%s vs 0x268184c = (children))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0x6a[] = "Incompatible checksums (%s vs 0x6a992d5 = (index))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0x92[] = "Incompatible checksums (%s vs 0x92e32ee = (length, mapping, wrapper))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0x93[] = "Incompatible checksums (%s vs 0x9388fec = (cResolvers, resolver_length))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xbd[] = "Incompatible checksums (%s vs 0xbdc49ed = (c_converter, converter, doCAPI, index, wrapper))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xc1[] = "Incompatible checksums (%s vs 0xc1c4252 = (function))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xd4[] = "Incompatible checksums (%s vs 0xd41d8cd = ())";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xd8[] = "Incompatible checksums (%s vs 0xd834048 = (c_converter, callable, converter, doCAPI, index, wrapper))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xe3[] = "Incompatible checksums (%s vs 0xe374ee2 = (c_returnValues, calculate_cArgs, calculate_cArguments, calculate_pyArgs, doCReturnAPI, doCargs, doCarguments, doPyargs, doReturnValues, doStoreValues, returnValues, storeValues, wrappedOperation))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xf8[] = "Incompatible checksums (%s vs 0xf84f4a6 = (mapping))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_2[] = "Incompatible checksums (0x%x vs (0xd834048, 0x5e58c5d, 0x3a61d67) = (c_converter, callable, converter, doCAPI, index, wrapper))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_3[] = "Incompatible checksums (0x%x vs (0xf84f4a6, 0xa6375ee, 0x821b7db) = (mapping))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_4[] = "Incompatible checksums (0x%x vs (0xbdc49ed, 0x502b02e, 0xbcf176e) = (c_converter, converter, doCAPI, index, wrapper))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_5[] = "Incompatible checksums (0x%x vs (0x92e32ee, 0x43c38b9, 0xef836e9) = (length, mapping, wrapper))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_6[] = "Incompatible checksums (0x%x vs (0x9388fec, 0x392503f, 0x9b5a664) = (cResolvers, resolver_length))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_7[] = "Incompatible checksums (0x%x vs (0xc1c4252, 0x78f9ac0, 0xc218e39) = (function))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_8[] = "Incompatible checksums (0x%x vs (0x6a992d5, 0x1bc04b5, 0xe540cdd) = (index))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_9[] = "Incompatible checksums (0x%x vs (0xe374ee2, 0x430b5a5, 0x3461dce) = (c_returnValues, calculate_cArgs, calculate_cArguments, calculate_pyArgs, doCReturnAPI, doCargs, doCarguments, doPyargs, doReturnValues, doStoreValues, returnValues, storeValues, wrappedOperation))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_10[] = "Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_11[] = "Incompatible checksums (0x%x vs (0x268184c, 0x1091008, 0x42685f1) = (children))";
 static PyObject *__pyx_kp_s_;
 static PyObject *__pyx_n_s_ArgumentError;
 static PyObject *__pyx_n_s_AttributeError;
 static PyObject *__pyx_n_s_CArgCalculator;
 static PyObject *__pyx_n_s_CArgCalculatorElement;
 static PyObject *__pyx_n_s_CArgumentCalculator;
 static PyObject *__pyx_n_s_CallFuncPyConverter;
 static PyObject *__pyx_n_s_DefaultCConverter;
 static PyObject *__pyx_kp_s_Expected_parameter_index_r_but_p;
 static PyObject *__pyx_kp_s_Expected_s_C_arguments_for_resol;
 static PyObject *__pyx_n_s_GLError;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x08;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x26;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x6a;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x92;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x93;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xbd;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xc1;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xd4;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xd8;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xe3;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xf8;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_10;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_11;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_3;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_4;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_5;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_6;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_7;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_8;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_9;
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_n_s_MultiReturn;
 static PyObject *__pyx_n_s_NULL;
 static PyObject *__pyx_n_s_NULL_2;
 static PyObject *__pyx_n_s_OpenGL;
 static PyObject *__pyx_n_s_OpenGL__null;
 static PyObject *__pyx_n_s_OpenGL_accelerate_wrapper;
@@ -2282,72 +2353,105 @@
 static PyObject *__pyx_tp_new_17OpenGL_accelerate_7wrapper_returnPyArgument(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_17OpenGL_accelerate_7wrapper_returnPyArgumentIndex(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_17OpenGL_accelerate_7wrapper_returnCArgument(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_17OpenGL_accelerate_7wrapper_MultiReturn(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_8910864;
+static PyObject *__pyx_int_17371144;
+static PyObject *__pyx_int_29099189;
 static PyObject *__pyx_int_40376396;
+static PyObject *__pyx_int_54926798;
+static PyObject *__pyx_int_59920447;
+static PyObject *__pyx_int_61218151;
+static PyObject *__pyx_int_69633521;
+static PyObject *__pyx_int_70301093;
+static PyObject *__pyx_int_71055545;
+static PyObject *__pyx_int_84062254;
+static PyObject *__pyx_int_98929757;
 static PyObject *__pyx_int_111776469;
+static PyObject *__pyx_int_126851776;
+static PyObject *__pyx_int_136427483;
 static PyObject *__pyx_int_154022638;
 static PyObject *__pyx_int_154701804;
+static PyObject *__pyx_int_160602753;
+static PyObject *__pyx_int_162899556;
+static PyObject *__pyx_int_174290414;
+static PyObject *__pyx_int_195155610;
+static PyObject *__pyx_int_198121326;
 static PyObject *__pyx_int_198986221;
 static PyObject *__pyx_int_203178578;
+static PyObject *__pyx_int_203525689;
 static PyObject *__pyx_int_222419149;
 static PyObject *__pyx_int_226705480;
+static PyObject *__pyx_int_228825662;
 static PyObject *__pyx_int_238505698;
+static PyObject *__pyx_int_238750788;
+static PyObject *__pyx_int_240389341;
+static PyObject *__pyx_int_251148009;
 static PyObject *__pyx_int_260371622;
 static PyObject *__pyx_tuple__2;
+static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
+static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
+static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
+static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_tuple__10;
+static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__12;
-static PyObject *__pyx_tuple__14;
-static PyObject *__pyx_tuple__16;
-static PyObject *__pyx_tuple__18;
-static PyObject *__pyx_tuple__20;
-static PyObject *__pyx_tuple__22;
-static PyObject *__pyx_tuple__24;
-static PyObject *__pyx_tuple__26;
-static PyObject *__pyx_tuple__28;
-static PyObject *__pyx_tuple__30;
-static PyObject *__pyx_tuple__32;
-static PyObject *__pyx_tuple__34;
-static PyObject *__pyx_codeobj__3;
-static PyObject *__pyx_codeobj__5;
-static PyObject *__pyx_codeobj__7;
-static PyObject *__pyx_codeobj__9;
-static PyObject *__pyx_codeobj__11;
-static PyObject *__pyx_codeobj__13;
-static PyObject *__pyx_codeobj__15;
-static PyObject *__pyx_codeobj__17;
-static PyObject *__pyx_codeobj__19;
-static PyObject *__pyx_codeobj__21;
-static PyObject *__pyx_codeobj__23;
-static PyObject *__pyx_codeobj__25;
-static PyObject *__pyx_codeobj__27;
-static PyObject *__pyx_codeobj__29;
-static PyObject *__pyx_codeobj__31;
-static PyObject *__pyx_codeobj__33;
-static PyObject *__pyx_codeobj__35;
+static PyObject *__pyx_tuple__13;
+static PyObject *__pyx_tuple__15;
+static PyObject *__pyx_tuple__17;
+static PyObject *__pyx_tuple__19;
+static PyObject *__pyx_tuple__21;
+static PyObject *__pyx_tuple__23;
+static PyObject *__pyx_tuple__25;
+static PyObject *__pyx_tuple__27;
+static PyObject *__pyx_tuple__29;
+static PyObject *__pyx_tuple__31;
+static PyObject *__pyx_tuple__33;
+static PyObject *__pyx_tuple__35;
+static PyObject *__pyx_tuple__37;
+static PyObject *__pyx_tuple__39;
+static PyObject *__pyx_tuple__41;
+static PyObject *__pyx_tuple__43;
+static PyObject *__pyx_tuple__45;
+static PyObject *__pyx_codeobj__14;
+static PyObject *__pyx_codeobj__16;
+static PyObject *__pyx_codeobj__18;
+static PyObject *__pyx_codeobj__20;
+static PyObject *__pyx_codeobj__22;
+static PyObject *__pyx_codeobj__24;
+static PyObject *__pyx_codeobj__26;
+static PyObject *__pyx_codeobj__28;
+static PyObject *__pyx_codeobj__30;
+static PyObject *__pyx_codeobj__32;
+static PyObject *__pyx_codeobj__34;
+static PyObject *__pyx_codeobj__36;
+static PyObject *__pyx_codeobj__38;
+static PyObject *__pyx_codeobj__40;
+static PyObject *__pyx_codeobj__42;
+static PyObject *__pyx_codeobj__44;
+static PyObject *__pyx_codeobj__46;
 /* Late includes */
 
 /* "src/wrapper.pyx":12
  * cdef class cArgConverter:
  *     """C-level API definition for cConverter objects"""
  *     def __call__( self, tuple pyArgs, int index, object wrapper ):             # <<<<<<<<<<<<<<
  *         """Return pyArgs[self.index] or raise a ValueError"""
  *         return self.c_call( pyArgs, index, wrapper )
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_17OpenGL_accelerate_7wrapper_13cArgConverter_1__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_17OpenGL_accelerate_7wrapper_13cArgConverter___call__[] = "Return pyArgs[self.index] or raise a ValueError";
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_13cArgConverter___call__;
 #endif
 static PyObject *__pyx_pw_17OpenGL_accelerate_7wrapper_13cArgConverter_1__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_pyArgs = 0;
   int __pyx_v_index;
   PyObject *__pyx_v_wrapper = 0;
   int __pyx_lineno = 0;
@@ -2780,15 +2884,15 @@
  *         """Call our function on incoming"""
  *         return self.c_call( incoming, function, arguments )
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_17OpenGL_accelerate_7wrapper_14pyArgConverter_1__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_17OpenGL_accelerate_7wrapper_14pyArgConverter___call__[] = "Call our function on incoming";
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_14pyArgConverter___call__;
 #endif
 static PyObject *__pyx_pw_17OpenGL_accelerate_7wrapper_14pyArgConverter_1__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_incoming = 0;
   PyObject *__pyx_v_function = 0;
   PyObject *__pyx_v_arguments = 0;
   int __pyx_lineno = 0;
@@ -3221,15 +3325,15 @@
  *         """Call our function on incoming"""
  *         return self.c_call( element )
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_17OpenGL_accelerate_7wrapper_18cArgumentConverter_1__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_17OpenGL_accelerate_7wrapper_18cArgumentConverter___call__[] = "Call our function on incoming";
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_18cArgumentConverter___call__;
 #endif
 static PyObject *__pyx_pw_17OpenGL_accelerate_7wrapper_18cArgumentConverter_1__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_element = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -3635,15 +3739,15 @@
  *         """Call our function on incoming"""
  *         return self.c_call( result, baseOperation, pyArgs, cArgs )
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_17OpenGL_accelerate_7wrapper_15returnConverter_1__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_17OpenGL_accelerate_7wrapper_15returnConverter___call__[] = "Call our function on incoming";
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_15returnConverter___call__;
 #endif
 static PyObject *__pyx_pw_17OpenGL_accelerate_7wrapper_15returnConverter_1__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_result = 0;
   PyObject *__pyx_v_baseOperation = 0;
   PyObject *__pyx_v_pyArgs = 0;
   PyObject *__pyx_v_cArgs = 0;
@@ -4316,15 +4420,15 @@
  *         """If callable, call converter( pyArgs, index, wrapper ), else return converter"""
  *         return self.c_call( pyArgs )
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_17OpenGL_accelerate_7wrapper_21CArgCalculatorElement_3__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_17OpenGL_accelerate_7wrapper_21CArgCalculatorElement_2__call__[] = "If callable, call converter( pyArgs, index, wrapper ), else return converter";
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_21CArgCalculatorElement_2__call__;
 #endif
 static PyObject *__pyx_pw_17OpenGL_accelerate_7wrapper_21CArgCalculatorElement_3__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_pyArgs = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -6007,15 +6111,15 @@
  *         """If converter is not None, call converter( pyArgs[self.index],  wrapper, pyArgs ), else return args[self.index]"""
  *         return self.c_call( args )
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_17OpenGL_accelerate_7wrapper_22PyArgCalculatorElement_3__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_17OpenGL_accelerate_7wrapper_22PyArgCalculatorElement_2__call__[] = "If converter is not None, call converter( pyArgs[self.index],  wrapper, pyArgs ), else return args[self.index]";
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_22PyArgCalculatorElement_2__call__;
 #endif
 static PyObject *__pyx_pw_17OpenGL_accelerate_7wrapper_22PyArgCalculatorElement_3__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_args = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -8854,15 +8958,15 @@
  *         """Store the function"""
  *         self.function = function
  */
 
 /* Python wrapper */
 static int __pyx_pw_17OpenGL_accelerate_7wrapper_19CallFuncPyConverter_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_17OpenGL_accelerate_7wrapper_19CallFuncPyConverter___init__[] = "Store the function";
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_19CallFuncPyConverter___init__;
 #endif
 static int __pyx_pw_17OpenGL_accelerate_7wrapper_19CallFuncPyConverter_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_function = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -9019,15 +9123,15 @@
  *         """Have a useful representation"""
  *         return '%s( %r )'%(
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_17OpenGL_accelerate_7wrapper_19CallFuncPyConverter_3__repr__(PyObject *__pyx_v_self); /*proto*/
 static char __pyx_doc_17OpenGL_accelerate_7wrapper_19CallFuncPyConverter_2__repr__[] = "Have a useful representation";
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_19CallFuncPyConverter_2__repr__;
 #endif
 static PyObject *__pyx_pw_17OpenGL_accelerate_7wrapper_19CallFuncPyConverter_3__repr__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__repr__ (wrapper)", 0);
   __pyx_r = __pyx_pf_17OpenGL_accelerate_7wrapper_19CallFuncPyConverter_2__repr__(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_CallFuncPyConverter *)__pyx_v_self));
@@ -9419,15 +9523,15 @@
  *         """Just store index for future access"""
  *         self.index = index
  */
 
 /* Python wrapper */
 static int __pyx_pw_17OpenGL_accelerate_7wrapper_17DefaultCConverter_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_17OpenGL_accelerate_7wrapper_17DefaultCConverter___init__[] = "Just store index for future access";
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_17DefaultCConverter___init__;
 #endif
 static int __pyx_pw_17OpenGL_accelerate_7wrapper_17DefaultCConverter_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_index = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -16217,151 +16321,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_7wrapper___pyx_unpickle_cArgConverter(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_cArgConverter", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd41d8cd:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xd41d8cd) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__2, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd41d8cd:
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = cArgConverter.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xd41d8cd:
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = cArgConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xd4, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd41d8cd:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = cArgConverter.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_cArgConverter__set_state(<cArgConverter> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_cArgConverter), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_cArgConverter), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = cArgConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_cArgConverter__set_state(<cArgConverter> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = cArgConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_cArgConverter__set_state(<cArgConverter> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_cArgConverter__set_state(cArgConverter __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_cArgConverter__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_cArgConverter *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_cArgConverter__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_cArgConverter *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = cArgConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_cArgConverter__set_state(<cArgConverter> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -16381,18 +16489,18 @@
  * def __pyx_unpickle_cArgConverter(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.wrapper.__pyx_unpickle_cArgConverter", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -16595,151 +16703,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_7wrapper_2__pyx_unpickle_pyArgConverter(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_pyArgConverter", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd41d8cd:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xd41d8cd) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__2, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd41d8cd:
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = pyArgConverter.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xd41d8cd:
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = pyArgConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xd4, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd41d8cd:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = pyArgConverter.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_pyArgConverter__set_state(<pyArgConverter> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_pyArgConverter), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_pyArgConverter), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = pyArgConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_pyArgConverter__set_state(<pyArgConverter> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = pyArgConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_pyArgConverter__set_state(<pyArgConverter> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_pyArgConverter__set_state(pyArgConverter __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_pyArgConverter__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_pyArgConverter *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_pyArgConverter__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_pyArgConverter *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = pyArgConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_pyArgConverter__set_state(<pyArgConverter> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -16759,18 +16871,18 @@
  * def __pyx_unpickle_pyArgConverter(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.wrapper.__pyx_unpickle_pyArgConverter", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -16973,151 +17085,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_7wrapper_4__pyx_unpickle_cArgumentConverter(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_cArgumentConverter", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd41d8cd:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xd41d8cd) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__2, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd41d8cd:
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = cArgumentConverter.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xd41d8cd:
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = cArgumentConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xd4, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd41d8cd:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = cArgumentConverter.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_cArgumentConverter__set_state(<cArgumentConverter> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_cArgumentConverter), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_cArgumentConverter), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = cArgumentConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_cArgumentConverter__set_state(<cArgumentConverter> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = cArgumentConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_cArgumentConverter__set_state(<cArgumentConverter> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_cArgumentConverter__set_state(cArgumentConverter __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_cArgumentConverter__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_cArgumentConverter *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_cArgumentConverter__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_cArgumentConverter *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = cArgumentConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_cArgumentConverter__set_state(<cArgumentConverter> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -17137,18 +17253,18 @@
  * def __pyx_unpickle_cArgumentConverter(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.wrapper.__pyx_unpickle_cArgumentConverter", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -17351,151 +17467,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_7wrapper_6__pyx_unpickle_returnConverter(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_returnConverter", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd41d8cd:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xd41d8cd) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__2, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd41d8cd:
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = returnConverter.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xd41d8cd:
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = returnConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xd4, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd41d8cd:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = returnConverter.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_returnConverter__set_state(<returnConverter> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_returnConverter), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_returnConverter), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = returnConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_returnConverter__set_state(<returnConverter> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = returnConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_returnConverter__set_state(<returnConverter> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_returnConverter__set_state(returnConverter __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_returnConverter__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_returnConverter *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_returnConverter__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_returnConverter *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = returnConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_returnConverter__set_state(<returnConverter> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -17515,18 +17635,18 @@
  * def __pyx_unpickle_returnConverter(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.wrapper.__pyx_unpickle_returnConverter", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -17729,151 +17849,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_7wrapper_8__pyx_unpickle_CArgCalculatorElement(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_CArgCalculatorElement", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd834048:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xd834048, 0x5e58c5d, 0x3a61d67):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd834048 = (c_converter, callable, converter, doCAPI, index, wrapper))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd834048, 0x5e58c5d, 0x3a61d67) = (c_converter, callable, converter, doCAPI, index, wrapper))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xd834048) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__3, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd834048:
+ *     if __pyx_checksum not in (0xd834048, 0x5e58c5d, 0x3a61d67):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd834048 = (c_converter, callable, converter, doCAPI, index, wrapper))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd834048, 0x5e58c5d, 0x3a61d67) = (c_converter, callable, converter, doCAPI, index, wrapper))" % __pyx_checksum)
  *     __pyx_result = CArgCalculatorElement.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xd834048:
+ *     if __pyx_checksum not in (0xd834048, 0x5e58c5d, 0x3a61d67):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd834048 = (c_converter, callable, converter, doCAPI, index, wrapper))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd834048, 0x5e58c5d, 0x3a61d67) = (c_converter, callable, converter, doCAPI, index, wrapper))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = CArgCalculatorElement.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xd8, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd834048:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xd834048, 0x5e58c5d, 0x3a61d67):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd834048 = (c_converter, callable, converter, doCAPI, index, wrapper))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd834048, 0x5e58c5d, 0x3a61d67) = (c_converter, callable, converter, doCAPI, index, wrapper))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd834048 = (c_converter, callable, converter, doCAPI, index, wrapper))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd834048, 0x5e58c5d, 0x3a61d67) = (c_converter, callable, converter, doCAPI, index, wrapper))" % __pyx_checksum)
  *     __pyx_result = CArgCalculatorElement.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_CArgCalculatorElement__set_state(<CArgCalculatorElement> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_CArgCalculatorElement), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_CArgCalculatorElement), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd834048 = (c_converter, callable, converter, doCAPI, index, wrapper))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd834048, 0x5e58c5d, 0x3a61d67) = (c_converter, callable, converter, doCAPI, index, wrapper))" % __pyx_checksum)
  *     __pyx_result = CArgCalculatorElement.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_CArgCalculatorElement__set_state(<CArgCalculatorElement> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = CArgCalculatorElement.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_CArgCalculatorElement__set_state(<CArgCalculatorElement> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_CArgCalculatorElement__set_state(CArgCalculatorElement __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_CArgCalculatorElement__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_CArgCalculatorElement *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_CArgCalculatorElement__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_CArgCalculatorElement *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd834048 = (c_converter, callable, converter, doCAPI, index, wrapper))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd834048, 0x5e58c5d, 0x3a61d67) = (c_converter, callable, converter, doCAPI, index, wrapper))" % __pyx_checksum)
  *     __pyx_result = CArgCalculatorElement.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_CArgCalculatorElement__set_state(<CArgCalculatorElement> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -17893,18 +18017,18 @@
  * def __pyx_unpickle_CArgCalculatorElement(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.wrapper.__pyx_unpickle_CArgCalculatorElement", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -18178,151 +18302,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_7wrapper_10__pyx_unpickle_CArgCalculator(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_CArgCalculator", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xf84f4a6:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xf84f4a6, 0xa6375ee, 0x821b7db):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf84f4a6 = (mapping))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf84f4a6, 0xa6375ee, 0x821b7db) = (mapping))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xf84f4a6) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__4, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xf84f4a6:
+ *     if __pyx_checksum not in (0xf84f4a6, 0xa6375ee, 0x821b7db):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf84f4a6 = (mapping))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf84f4a6, 0xa6375ee, 0x821b7db) = (mapping))" % __pyx_checksum)
  *     __pyx_result = CArgCalculator.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xf84f4a6:
+ *     if __pyx_checksum not in (0xf84f4a6, 0xa6375ee, 0x821b7db):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf84f4a6 = (mapping))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf84f4a6, 0xa6375ee, 0x821b7db) = (mapping))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = CArgCalculator.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xf8, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xf84f4a6:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xf84f4a6, 0xa6375ee, 0x821b7db):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf84f4a6 = (mapping))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf84f4a6, 0xa6375ee, 0x821b7db) = (mapping))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf84f4a6 = (mapping))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf84f4a6, 0xa6375ee, 0x821b7db) = (mapping))" % __pyx_checksum)
  *     __pyx_result = CArgCalculator.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_CArgCalculator__set_state(<CArgCalculator> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_CArgCalculator), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_CArgCalculator), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf84f4a6 = (mapping))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf84f4a6, 0xa6375ee, 0x821b7db) = (mapping))" % __pyx_checksum)
  *     __pyx_result = CArgCalculator.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_CArgCalculator__set_state(<CArgCalculator> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = CArgCalculator.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_CArgCalculator__set_state(<CArgCalculator> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_CArgCalculator__set_state(CArgCalculator __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_CArgCalculator__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_CArgCalculator *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_CArgCalculator__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_CArgCalculator *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf84f4a6 = (mapping))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf84f4a6, 0xa6375ee, 0x821b7db) = (mapping))" % __pyx_checksum)
  *     __pyx_result = CArgCalculator.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_CArgCalculator__set_state(<CArgCalculator> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -18342,18 +18470,18 @@
  * def __pyx_unpickle_CArgCalculator(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.wrapper.__pyx_unpickle_CArgCalculator", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -18576,151 +18704,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_7wrapper_12__pyx_unpickle_PyArgCalculatorElement(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_PyArgCalculatorElement", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xbdc49ed:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xbdc49ed, 0x502b02e, 0xbcf176e):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xbdc49ed = (c_converter, converter, doCAPI, index, wrapper))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xbdc49ed, 0x502b02e, 0xbcf176e) = (c_converter, converter, doCAPI, index, wrapper))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xbdc49ed) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__5, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xbdc49ed:
+ *     if __pyx_checksum not in (0xbdc49ed, 0x502b02e, 0xbcf176e):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xbdc49ed = (c_converter, converter, doCAPI, index, wrapper))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xbdc49ed, 0x502b02e, 0xbcf176e) = (c_converter, converter, doCAPI, index, wrapper))" % __pyx_checksum)
  *     __pyx_result = PyArgCalculatorElement.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xbdc49ed:
+ *     if __pyx_checksum not in (0xbdc49ed, 0x502b02e, 0xbcf176e):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xbdc49ed = (c_converter, converter, doCAPI, index, wrapper))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xbdc49ed, 0x502b02e, 0xbcf176e) = (c_converter, converter, doCAPI, index, wrapper))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = PyArgCalculatorElement.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xbd, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_4, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xbdc49ed:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xbdc49ed, 0x502b02e, 0xbcf176e):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xbdc49ed = (c_converter, converter, doCAPI, index, wrapper))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xbdc49ed, 0x502b02e, 0xbcf176e) = (c_converter, converter, doCAPI, index, wrapper))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xbdc49ed = (c_converter, converter, doCAPI, index, wrapper))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xbdc49ed, 0x502b02e, 0xbcf176e) = (c_converter, converter, doCAPI, index, wrapper))" % __pyx_checksum)
  *     __pyx_result = PyArgCalculatorElement.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_PyArgCalculatorElement__set_state(<PyArgCalculatorElement> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_PyArgCalculatorElement), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_PyArgCalculatorElement), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xbdc49ed = (c_converter, converter, doCAPI, index, wrapper))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xbdc49ed, 0x502b02e, 0xbcf176e) = (c_converter, converter, doCAPI, index, wrapper))" % __pyx_checksum)
  *     __pyx_result = PyArgCalculatorElement.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_PyArgCalculatorElement__set_state(<PyArgCalculatorElement> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = PyArgCalculatorElement.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_PyArgCalculatorElement__set_state(<PyArgCalculatorElement> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_PyArgCalculatorElement__set_state(PyArgCalculatorElement __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_PyArgCalculatorElement__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_PyArgCalculatorElement *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_PyArgCalculatorElement__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_PyArgCalculatorElement *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xbdc49ed = (c_converter, converter, doCAPI, index, wrapper))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xbdc49ed, 0x502b02e, 0xbcf176e) = (c_converter, converter, doCAPI, index, wrapper))" % __pyx_checksum)
  *     __pyx_result = PyArgCalculatorElement.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_PyArgCalculatorElement__set_state(<PyArgCalculatorElement> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -18740,18 +18872,18 @@
  * def __pyx_unpickle_PyArgCalculatorElement(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.wrapper.__pyx_unpickle_PyArgCalculatorElement", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -19016,151 +19148,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_7wrapper_14__pyx_unpickle_PyArgCalculator(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_PyArgCalculator", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x92e32ee:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x92e32ee, 0x43c38b9, 0xef836e9):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x92e32ee = (length, mapping, wrapper))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x92e32ee, 0x43c38b9, 0xef836e9) = (length, mapping, wrapper))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x92e32ee) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__6, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x92e32ee:
+ *     if __pyx_checksum not in (0x92e32ee, 0x43c38b9, 0xef836e9):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x92e32ee = (length, mapping, wrapper))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x92e32ee, 0x43c38b9, 0xef836e9) = (length, mapping, wrapper))" % __pyx_checksum)
  *     __pyx_result = PyArgCalculator.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x92e32ee:
+ *     if __pyx_checksum not in (0x92e32ee, 0x43c38b9, 0xef836e9):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x92e32ee = (length, mapping, wrapper))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x92e32ee, 0x43c38b9, 0xef836e9) = (length, mapping, wrapper))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = PyArgCalculator.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x92, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_5, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x92e32ee:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x92e32ee, 0x43c38b9, 0xef836e9):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x92e32ee = (length, mapping, wrapper))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x92e32ee, 0x43c38b9, 0xef836e9) = (length, mapping, wrapper))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x92e32ee = (length, mapping, wrapper))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x92e32ee, 0x43c38b9, 0xef836e9) = (length, mapping, wrapper))" % __pyx_checksum)
  *     __pyx_result = PyArgCalculator.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_PyArgCalculator__set_state(<PyArgCalculator> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_PyArgCalculator), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_PyArgCalculator), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x92e32ee = (length, mapping, wrapper))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x92e32ee, 0x43c38b9, 0xef836e9) = (length, mapping, wrapper))" % __pyx_checksum)
  *     __pyx_result = PyArgCalculator.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_PyArgCalculator__set_state(<PyArgCalculator> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = PyArgCalculator.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_PyArgCalculator__set_state(<PyArgCalculator> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_PyArgCalculator__set_state(PyArgCalculator __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_PyArgCalculator__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_PyArgCalculator *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_PyArgCalculator__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_PyArgCalculator *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x92e32ee = (length, mapping, wrapper))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x92e32ee, 0x43c38b9, 0xef836e9) = (length, mapping, wrapper))" % __pyx_checksum)
  *     __pyx_result = PyArgCalculator.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_PyArgCalculator__set_state(<PyArgCalculator> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -19180,18 +19316,18 @@
  * def __pyx_unpickle_PyArgCalculator(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.wrapper.__pyx_unpickle_PyArgCalculator", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -19435,151 +19571,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_7wrapper_16__pyx_unpickle_CArgumentCalculator(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_CArgumentCalculator", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x9388fec:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x9388fec, 0x392503f, 0x9b5a664):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x9388fec = (cResolvers, resolver_length))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x9388fec, 0x392503f, 0x9b5a664) = (cResolvers, resolver_length))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x9388fec) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__7, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x9388fec:
+ *     if __pyx_checksum not in (0x9388fec, 0x392503f, 0x9b5a664):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x9388fec = (cResolvers, resolver_length))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x9388fec, 0x392503f, 0x9b5a664) = (cResolvers, resolver_length))" % __pyx_checksum)
  *     __pyx_result = CArgumentCalculator.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x9388fec:
+ *     if __pyx_checksum not in (0x9388fec, 0x392503f, 0x9b5a664):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x9388fec = (cResolvers, resolver_length))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x9388fec, 0x392503f, 0x9b5a664) = (cResolvers, resolver_length))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = CArgumentCalculator.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x93, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_6, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x9388fec:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x9388fec, 0x392503f, 0x9b5a664):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x9388fec = (cResolvers, resolver_length))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x9388fec, 0x392503f, 0x9b5a664) = (cResolvers, resolver_length))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x9388fec = (cResolvers, resolver_length))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x9388fec, 0x392503f, 0x9b5a664) = (cResolvers, resolver_length))" % __pyx_checksum)
  *     __pyx_result = CArgumentCalculator.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_CArgumentCalculator__set_state(<CArgumentCalculator> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_CArgumentCalculator), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_CArgumentCalculator), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x9388fec = (cResolvers, resolver_length))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x9388fec, 0x392503f, 0x9b5a664) = (cResolvers, resolver_length))" % __pyx_checksum)
  *     __pyx_result = CArgumentCalculator.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_CArgumentCalculator__set_state(<CArgumentCalculator> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = CArgumentCalculator.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_CArgumentCalculator__set_state(<CArgumentCalculator> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_CArgumentCalculator__set_state(CArgumentCalculator __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_CArgumentCalculator__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_CArgumentCalculator *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_CArgumentCalculator__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_CArgumentCalculator *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x9388fec = (cResolvers, resolver_length))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x9388fec, 0x392503f, 0x9b5a664) = (cResolvers, resolver_length))" % __pyx_checksum)
  *     __pyx_result = CArgumentCalculator.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_CArgumentCalculator__set_state(<CArgumentCalculator> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -19599,18 +19739,18 @@
  * def __pyx_unpickle_CArgumentCalculator(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.wrapper.__pyx_unpickle_CArgumentCalculator", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -19843,151 +19983,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_7wrapper_18__pyx_unpickle_CallFuncPyConverter(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_CallFuncPyConverter", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xc1c4252:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xc1c4252, 0x78f9ac0, 0xc218e39):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xc1c4252 = (function))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc1c4252, 0x78f9ac0, 0xc218e39) = (function))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xc1c4252) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__8, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xc1c4252:
+ *     if __pyx_checksum not in (0xc1c4252, 0x78f9ac0, 0xc218e39):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xc1c4252 = (function))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc1c4252, 0x78f9ac0, 0xc218e39) = (function))" % __pyx_checksum)
  *     __pyx_result = CallFuncPyConverter.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xc1c4252:
+ *     if __pyx_checksum not in (0xc1c4252, 0x78f9ac0, 0xc218e39):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xc1c4252 = (function))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc1c4252, 0x78f9ac0, 0xc218e39) = (function))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = CallFuncPyConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xc1, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_7, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xc1c4252:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xc1c4252, 0x78f9ac0, 0xc218e39):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xc1c4252 = (function))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc1c4252, 0x78f9ac0, 0xc218e39) = (function))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xc1c4252 = (function))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc1c4252, 0x78f9ac0, 0xc218e39) = (function))" % __pyx_checksum)
  *     __pyx_result = CallFuncPyConverter.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_CallFuncPyConverter__set_state(<CallFuncPyConverter> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_CallFuncPyConverter), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_CallFuncPyConverter), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xc1c4252 = (function))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc1c4252, 0x78f9ac0, 0xc218e39) = (function))" % __pyx_checksum)
  *     __pyx_result = CallFuncPyConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_CallFuncPyConverter__set_state(<CallFuncPyConverter> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = CallFuncPyConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_CallFuncPyConverter__set_state(<CallFuncPyConverter> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_CallFuncPyConverter__set_state(CallFuncPyConverter __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_CallFuncPyConverter__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_CallFuncPyConverter *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_CallFuncPyConverter__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_CallFuncPyConverter *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xc1c4252 = (function))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc1c4252, 0x78f9ac0, 0xc218e39) = (function))" % __pyx_checksum)
  *     __pyx_result = CallFuncPyConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_CallFuncPyConverter__set_state(<CallFuncPyConverter> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -20007,18 +20151,18 @@
  * def __pyx_unpickle_CallFuncPyConverter(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.wrapper.__pyx_unpickle_CallFuncPyConverter", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -20240,151 +20384,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_7wrapper_20__pyx_unpickle_DefaultCConverter(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_DefaultCConverter", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x6a992d5:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x6a992d5, 0x1bc04b5, 0xe540cdd):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6a992d5 = (index))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6a992d5, 0x1bc04b5, 0xe540cdd) = (index))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x6a992d5) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__9, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x6a992d5:
+ *     if __pyx_checksum not in (0x6a992d5, 0x1bc04b5, 0xe540cdd):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6a992d5 = (index))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6a992d5, 0x1bc04b5, 0xe540cdd) = (index))" % __pyx_checksum)
  *     __pyx_result = DefaultCConverter.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x6a992d5:
+ *     if __pyx_checksum not in (0x6a992d5, 0x1bc04b5, 0xe540cdd):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6a992d5 = (index))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6a992d5, 0x1bc04b5, 0xe540cdd) = (index))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = DefaultCConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x6a, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_8, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x6a992d5:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x6a992d5, 0x1bc04b5, 0xe540cdd):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6a992d5 = (index))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6a992d5, 0x1bc04b5, 0xe540cdd) = (index))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6a992d5 = (index))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6a992d5, 0x1bc04b5, 0xe540cdd) = (index))" % __pyx_checksum)
  *     __pyx_result = DefaultCConverter.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_DefaultCConverter__set_state(<DefaultCConverter> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_DefaultCConverter), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_DefaultCConverter), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6a992d5 = (index))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6a992d5, 0x1bc04b5, 0xe540cdd) = (index))" % __pyx_checksum)
  *     __pyx_result = DefaultCConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_DefaultCConverter__set_state(<DefaultCConverter> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = DefaultCConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_DefaultCConverter__set_state(<DefaultCConverter> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_DefaultCConverter__set_state(DefaultCConverter __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_DefaultCConverter__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_DefaultCConverter *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_DefaultCConverter__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_DefaultCConverter *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6a992d5 = (index))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6a992d5, 0x1bc04b5, 0xe540cdd) = (index))" % __pyx_checksum)
  *     __pyx_result = DefaultCConverter.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_DefaultCConverter__set_state(<DefaultCConverter> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -20404,18 +20552,18 @@
  * def __pyx_unpickle_DefaultCConverter(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.wrapper.__pyx_unpickle_DefaultCConverter", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -20636,151 +20784,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_7wrapper_22__pyx_unpickle_Wrapper(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_Wrapper", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe374ee2:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xe374ee2, 0x430b5a5, 0x3461dce):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe374ee2 = (c_returnValues, calculate_cArgs, calculate_cArguments, calculate_pyArgs, doCReturnAPI, doCargs, doCarguments, doPyargs, doReturnValues, doStoreValues, returnValues, storeValues, wrappedOperation))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe374ee2, 0x430b5a5, 0x3461dce) = (c_returnValues, calculate_cArgs, calculate_cArguments, calculate_pyArgs, doCReturnAPI, doCargs, doCarguments, doPyargs, doReturnValues, doStoreValues, returnValues, storeValues, wrappedOperation))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xe374ee2) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__10, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe374ee2:
+ *     if __pyx_checksum not in (0xe374ee2, 0x430b5a5, 0x3461dce):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe374ee2 = (c_returnValues, calculate_cArgs, calculate_cArguments, calculate_pyArgs, doCReturnAPI, doCargs, doCarguments, doPyargs, doReturnValues, doStoreValues, returnValues, storeValues, wrappedOperation))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe374ee2, 0x430b5a5, 0x3461dce) = (c_returnValues, calculate_cArgs, calculate_cArguments, calculate_pyArgs, doCReturnAPI, doCargs, doCarguments, doPyargs, doReturnValues, doStoreValues, returnValues, storeValues, wrappedOperation))" % __pyx_checksum)
  *     __pyx_result = Wrapper.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xe374ee2:
+ *     if __pyx_checksum not in (0xe374ee2, 0x430b5a5, 0x3461dce):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe374ee2 = (c_returnValues, calculate_cArgs, calculate_cArguments, calculate_pyArgs, doCReturnAPI, doCargs, doCarguments, doPyargs, doReturnValues, doStoreValues, returnValues, storeValues, wrappedOperation))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe374ee2, 0x430b5a5, 0x3461dce) = (c_returnValues, calculate_cArgs, calculate_cArguments, calculate_pyArgs, doCReturnAPI, doCargs, doCarguments, doPyargs, doReturnValues, doStoreValues, returnValues, storeValues, wrappedOperation))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = Wrapper.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xe3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_9, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe374ee2:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xe374ee2, 0x430b5a5, 0x3461dce):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe374ee2 = (c_returnValues, calculate_cArgs, calculate_cArguments, calculate_pyArgs, doCReturnAPI, doCargs, doCarguments, doPyargs, doReturnValues, doStoreValues, returnValues, storeValues, wrappedOperation))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe374ee2, 0x430b5a5, 0x3461dce) = (c_returnValues, calculate_cArgs, calculate_cArguments, calculate_pyArgs, doCReturnAPI, doCargs, doCarguments, doPyargs, doReturnValues, doStoreValues, returnValues, storeValues, wrappedOperation))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe374ee2 = (c_returnValues, calculate_cArgs, calculate_cArguments, calculate_pyArgs, doCReturnAPI, doCargs, doCarguments, doPyargs, doReturnValues, doStoreValues, returnValues, storeValues, wrappedOperation))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe374ee2, 0x430b5a5, 0x3461dce) = (c_returnValues, calculate_cArgs, calculate_cArguments, calculate_pyArgs, doCReturnAPI, doCargs, doCarguments, doPyargs, doReturnValues, doStoreValues, returnValues, storeValues, wrappedOperation))" % __pyx_checksum)
  *     __pyx_result = Wrapper.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Wrapper__set_state(<Wrapper> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_Wrapper), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_Wrapper), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe374ee2 = (c_returnValues, calculate_cArgs, calculate_cArguments, calculate_pyArgs, doCReturnAPI, doCargs, doCarguments, doPyargs, doReturnValues, doStoreValues, returnValues, storeValues, wrappedOperation))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe374ee2, 0x430b5a5, 0x3461dce) = (c_returnValues, calculate_cArgs, calculate_cArguments, calculate_pyArgs, doCReturnAPI, doCargs, doCarguments, doPyargs, doReturnValues, doStoreValues, returnValues, storeValues, wrappedOperation))" % __pyx_checksum)
  *     __pyx_result = Wrapper.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Wrapper__set_state(<Wrapper> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = Wrapper.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Wrapper__set_state(<Wrapper> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Wrapper__set_state(Wrapper __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_Wrapper__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_Wrapper *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_Wrapper__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_Wrapper *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe374ee2 = (c_returnValues, calculate_cArgs, calculate_cArguments, calculate_pyArgs, doCReturnAPI, doCargs, doCarguments, doPyargs, doReturnValues, doStoreValues, returnValues, storeValues, wrappedOperation))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe374ee2, 0x430b5a5, 0x3461dce) = (c_returnValues, calculate_cArgs, calculate_cArguments, calculate_pyArgs, doCReturnAPI, doCargs, doCarguments, doPyargs, doReturnValues, doStoreValues, returnValues, storeValues, wrappedOperation))" % __pyx_checksum)
  *     __pyx_result = Wrapper.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Wrapper__set_state(<Wrapper> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -20800,18 +20952,18 @@
  * def __pyx_unpickle_Wrapper(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.wrapper.__pyx_unpickle_Wrapper", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -21158,151 +21310,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_7wrapper_24__pyx_unpickle_getPyArgsName(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_getPyArgsName", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x087f810:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x087f810, 0x9929a81, 0xba1d69a):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x087f810 = (index, name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x087f810) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__11, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x087f810:
+ *     if __pyx_checksum not in (0x087f810, 0x9929a81, 0xba1d69a):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x087f810 = (index, name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))" % __pyx_checksum)
  *     __pyx_result = getPyArgsName.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x087f810:
+ *     if __pyx_checksum not in (0x087f810, 0x9929a81, 0xba1d69a):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x087f810 = (index, name))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = getPyArgsName.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x08, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_10, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x087f810:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x087f810, 0x9929a81, 0xba1d69a):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x087f810 = (index, name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x087f810 = (index, name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))" % __pyx_checksum)
  *     __pyx_result = getPyArgsName.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_getPyArgsName__set_state(<getPyArgsName> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_getPyArgsName), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_getPyArgsName), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x087f810 = (index, name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))" % __pyx_checksum)
  *     __pyx_result = getPyArgsName.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_getPyArgsName__set_state(<getPyArgsName> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = getPyArgsName.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_getPyArgsName__set_state(<getPyArgsName> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_getPyArgsName__set_state(getPyArgsName __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_getPyArgsName__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_getPyArgsName *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_getPyArgsName__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_getPyArgsName *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x087f810 = (index, name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))" % __pyx_checksum)
  *     __pyx_result = getPyArgsName.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_getPyArgsName__set_state(<getPyArgsName> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -21322,18 +21478,18 @@
  * def __pyx_unpickle_getPyArgsName(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.wrapper.__pyx_unpickle_getPyArgsName", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -21566,151 +21722,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_7wrapper_26__pyx_unpickle_returnPyArgument(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_returnPyArgument", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x087f810:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x087f810, 0x9929a81, 0xba1d69a):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x087f810 = (index, name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x087f810) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__11, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x087f810:
+ *     if __pyx_checksum not in (0x087f810, 0x9929a81, 0xba1d69a):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x087f810 = (index, name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))" % __pyx_checksum)
  *     __pyx_result = returnPyArgument.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x087f810:
+ *     if __pyx_checksum not in (0x087f810, 0x9929a81, 0xba1d69a):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x087f810 = (index, name))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = returnPyArgument.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x08, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_10, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x087f810:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x087f810, 0x9929a81, 0xba1d69a):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x087f810 = (index, name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x087f810 = (index, name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))" % __pyx_checksum)
  *     __pyx_result = returnPyArgument.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_returnPyArgument__set_state(<returnPyArgument> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_returnPyArgument), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_returnPyArgument), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x087f810 = (index, name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))" % __pyx_checksum)
  *     __pyx_result = returnPyArgument.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_returnPyArgument__set_state(<returnPyArgument> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = returnPyArgument.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_returnPyArgument__set_state(<returnPyArgument> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_returnPyArgument__set_state(returnPyArgument __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_returnPyArgument__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_returnPyArgument *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_returnPyArgument__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_returnPyArgument *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x087f810 = (index, name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))" % __pyx_checksum)
  *     __pyx_result = returnPyArgument.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_returnPyArgument__set_state(<returnPyArgument> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -21730,18 +21890,18 @@
  * def __pyx_unpickle_returnPyArgument(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.wrapper.__pyx_unpickle_returnPyArgument", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -21974,151 +22134,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_7wrapper_28__pyx_unpickle_returnPyArgumentIndex(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_returnPyArgumentIndex", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x6a992d5:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x6a992d5, 0x1bc04b5, 0xe540cdd):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6a992d5 = (index))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6a992d5, 0x1bc04b5, 0xe540cdd) = (index))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x6a992d5) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__9, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x6a992d5:
+ *     if __pyx_checksum not in (0x6a992d5, 0x1bc04b5, 0xe540cdd):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6a992d5 = (index))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6a992d5, 0x1bc04b5, 0xe540cdd) = (index))" % __pyx_checksum)
  *     __pyx_result = returnPyArgumentIndex.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x6a992d5:
+ *     if __pyx_checksum not in (0x6a992d5, 0x1bc04b5, 0xe540cdd):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6a992d5 = (index))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6a992d5, 0x1bc04b5, 0xe540cdd) = (index))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = returnPyArgumentIndex.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x6a, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_8, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x6a992d5:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x6a992d5, 0x1bc04b5, 0xe540cdd):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6a992d5 = (index))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6a992d5, 0x1bc04b5, 0xe540cdd) = (index))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6a992d5 = (index))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6a992d5, 0x1bc04b5, 0xe540cdd) = (index))" % __pyx_checksum)
  *     __pyx_result = returnPyArgumentIndex.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_returnPyArgumentIndex__set_state(<returnPyArgumentIndex> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_returnPyArgumentIndex), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_returnPyArgumentIndex), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6a992d5 = (index))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6a992d5, 0x1bc04b5, 0xe540cdd) = (index))" % __pyx_checksum)
  *     __pyx_result = returnPyArgumentIndex.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_returnPyArgumentIndex__set_state(<returnPyArgumentIndex> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = returnPyArgumentIndex.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_returnPyArgumentIndex__set_state(<returnPyArgumentIndex> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_returnPyArgumentIndex__set_state(returnPyArgumentIndex __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_returnPyArgumentIndex__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_returnPyArgumentIndex *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_returnPyArgumentIndex__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_returnPyArgumentIndex *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x6a992d5 = (index))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x6a992d5, 0x1bc04b5, 0xe540cdd) = (index))" % __pyx_checksum)
  *     __pyx_result = returnPyArgumentIndex.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_returnPyArgumentIndex__set_state(<returnPyArgumentIndex> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -22138,18 +22302,18 @@
  * def __pyx_unpickle_returnPyArgumentIndex(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.wrapper.__pyx_unpickle_returnPyArgumentIndex", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -22370,151 +22534,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_7wrapper_30__pyx_unpickle_returnCArgument(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_returnCArgument", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x087f810:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x087f810, 0x9929a81, 0xba1d69a):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x087f810 = (index, name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x087f810) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__11, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x087f810:
+ *     if __pyx_checksum not in (0x087f810, 0x9929a81, 0xba1d69a):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x087f810 = (index, name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))" % __pyx_checksum)
  *     __pyx_result = returnCArgument.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x087f810:
+ *     if __pyx_checksum not in (0x087f810, 0x9929a81, 0xba1d69a):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x087f810 = (index, name))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = returnCArgument.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x08, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_10, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x087f810:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x087f810, 0x9929a81, 0xba1d69a):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x087f810 = (index, name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x087f810 = (index, name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))" % __pyx_checksum)
  *     __pyx_result = returnCArgument.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_returnCArgument__set_state(<returnCArgument> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_returnCArgument), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_returnCArgument), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x087f810 = (index, name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))" % __pyx_checksum)
  *     __pyx_result = returnCArgument.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_returnCArgument__set_state(<returnCArgument> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = returnCArgument.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_returnCArgument__set_state(<returnCArgument> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_returnCArgument__set_state(returnCArgument __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_returnCArgument__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_returnCArgument *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_returnCArgument__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_returnCArgument *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x087f810 = (index, name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x087f810, 0x9929a81, 0xba1d69a) = (index, name))" % __pyx_checksum)
  *     __pyx_result = returnCArgument.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_returnCArgument__set_state(<returnCArgument> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -22534,18 +22702,18 @@
  * def __pyx_unpickle_returnCArgument(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.wrapper.__pyx_unpickle_returnCArgument", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -22778,151 +22946,155 @@
 }
 
 static PyObject *__pyx_pf_17OpenGL_accelerate_7wrapper_32__pyx_unpickle_MultiReturn(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_MultiReturn", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x268184c:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x268184c, 0x1091008, 0x42685f1):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x268184c = (children))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x268184c, 0x1091008, 0x42685f1) = (children))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x268184c) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__12, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x268184c:
+ *     if __pyx_checksum not in (0x268184c, 0x1091008, 0x42685f1):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x268184c = (children))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x268184c, 0x1091008, 0x42685f1) = (children))" % __pyx_checksum)
  *     __pyx_result = MultiReturn.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x268184c:
+ *     if __pyx_checksum not in (0x268184c, 0x1091008, 0x42685f1):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x268184c = (children))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x268184c, 0x1091008, 0x42685f1) = (children))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = MultiReturn.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x26, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_11, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x268184c:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x268184c, 0x1091008, 0x42685f1):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x268184c = (children))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x268184c, 0x1091008, 0x42685f1) = (children))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x268184c = (children))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x268184c, 0x1091008, 0x42685f1) = (children))" % __pyx_checksum)
  *     __pyx_result = MultiReturn.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_MultiReturn__set_state(<MultiReturn> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_MultiReturn), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_17OpenGL_accelerate_7wrapper_MultiReturn), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x268184c = (children))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x268184c, 0x1091008, 0x42685f1) = (children))" % __pyx_checksum)
  *     __pyx_result = MultiReturn.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_MultiReturn__set_state(<MultiReturn> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = MultiReturn.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_MultiReturn__set_state(<MultiReturn> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_MultiReturn__set_state(MultiReturn __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_MultiReturn__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_MultiReturn *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __pyx_f_17OpenGL_accelerate_7wrapper___pyx_unpickle_MultiReturn__set_state(((struct __pyx_obj_17OpenGL_accelerate_7wrapper_MultiReturn *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x268184c = (children))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x268184c, 0x1091008, 0x42685f1) = (children))" % __pyx_checksum)
  *     __pyx_result = MultiReturn.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_MultiReturn__set_state(<MultiReturn> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -22942,18 +23114,18 @@
  * def __pyx_unpickle_MultiReturn(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("OpenGL_accelerate.wrapper.__pyx_unpickle_MultiReturn", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -25318,25 +25490,25 @@
   {&__pyx_n_s_CArgCalculatorElement, __pyx_k_CArgCalculatorElement, sizeof(__pyx_k_CArgCalculatorElement), 0, 0, 1, 1},
   {&__pyx_n_s_CArgumentCalculator, __pyx_k_CArgumentCalculator, sizeof(__pyx_k_CArgumentCalculator), 0, 0, 1, 1},
   {&__pyx_n_s_CallFuncPyConverter, __pyx_k_CallFuncPyConverter, sizeof(__pyx_k_CallFuncPyConverter), 0, 0, 1, 1},
   {&__pyx_n_s_DefaultCConverter, __pyx_k_DefaultCConverter, sizeof(__pyx_k_DefaultCConverter), 0, 0, 1, 1},
   {&__pyx_kp_s_Expected_parameter_index_r_but_p, __pyx_k_Expected_parameter_index_r_but_p, sizeof(__pyx_k_Expected_parameter_index_r_but_p), 0, 0, 1, 0},
   {&__pyx_kp_s_Expected_s_C_arguments_for_resol, __pyx_k_Expected_s_C_arguments_for_resol, sizeof(__pyx_k_Expected_s_C_arguments_for_resol), 0, 0, 1, 0},
   {&__pyx_n_s_GLError, __pyx_k_GLError, sizeof(__pyx_k_GLError), 0, 0, 1, 1},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x08, __pyx_k_Incompatible_checksums_s_vs_0x08, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x08), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x26, __pyx_k_Incompatible_checksums_s_vs_0x26, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x26), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x6a, __pyx_k_Incompatible_checksums_s_vs_0x6a, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x6a), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x92, __pyx_k_Incompatible_checksums_s_vs_0x92, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x92), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x93, __pyx_k_Incompatible_checksums_s_vs_0x93, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x93), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xbd, __pyx_k_Incompatible_checksums_s_vs_0xbd, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xbd), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xc1, __pyx_k_Incompatible_checksums_s_vs_0xc1, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xc1), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xd4, __pyx_k_Incompatible_checksums_s_vs_0xd4, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xd4), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xd8, __pyx_k_Incompatible_checksums_s_vs_0xd8, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xd8), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xe3, __pyx_k_Incompatible_checksums_s_vs_0xe3, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xe3), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xf8, __pyx_k_Incompatible_checksums_s_vs_0xf8, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xf8), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_10, __pyx_k_Incompatible_checksums_0x_x_vs_0_10, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_10), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_11, __pyx_k_Incompatible_checksums_0x_x_vs_0_11, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_11), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2, __pyx_k_Incompatible_checksums_0x_x_vs_0_2, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_2), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_3, __pyx_k_Incompatible_checksums_0x_x_vs_0_3, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_3), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_4, __pyx_k_Incompatible_checksums_0x_x_vs_0_4, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_4), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_5, __pyx_k_Incompatible_checksums_0x_x_vs_0_5, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_5), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_6, __pyx_k_Incompatible_checksums_0x_x_vs_0_6, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_6), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_7, __pyx_k_Incompatible_checksums_0x_x_vs_0_7, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_7), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_8, __pyx_k_Incompatible_checksums_0x_x_vs_0_8, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_8), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_9, __pyx_k_Incompatible_checksums_0x_x_vs_0_9, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_9), 0, 0, 1, 0},
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_n_s_MultiReturn, __pyx_k_MultiReturn, sizeof(__pyx_k_MultiReturn), 0, 0, 1, 1},
   {&__pyx_n_s_NULL, __pyx_k_NULL, sizeof(__pyx_k_NULL), 0, 0, 1, 1},
   {&__pyx_n_s_NULL_2, __pyx_k_NULL_2, sizeof(__pyx_k_NULL_2), 0, 0, 1, 1},
   {&__pyx_n_s_OpenGL, __pyx_k_OpenGL, sizeof(__pyx_k_OpenGL), 0, 0, 1, 1},
   {&__pyx_n_s_OpenGL__null, __pyx_k_OpenGL__null, sizeof(__pyx_k_OpenGL__null), 0, 0, 1, 1},
   {&__pyx_n_s_OpenGL_accelerate_wrapper, __pyx_k_OpenGL_accelerate_wrapper, sizeof(__pyx_k_OpenGL_accelerate_wrapper), 0, 0, 1, 1},
@@ -25442,108 +25614,171 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "(tree fragment)":1
- * def __pyx_unpickle_cArgConverter(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+  /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  */
-  __pyx_tuple__2 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(3, __pyx_int_222419149, __pyx_int_238750788, __pyx_int_228825662); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_cArgConverter, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__4 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(3, __pyx_int_226705480, __pyx_int_98929757, __pyx_int_61218151); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_tuple__4 = PyTuple_Pack(3, __pyx_int_260371622, __pyx_int_174290414, __pyx_int_136427483); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_pyArgConverter, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__6 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(3, __pyx_int_198986221, __pyx_int_84062254, __pyx_int_198121326); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_tuple__6 = PyTuple_Pack(3, __pyx_int_154022638, __pyx_int_71055545, __pyx_int_251148009); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_cArgumentConverte, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__8 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(3, __pyx_int_154701804, __pyx_int_59920447, __pyx_int_162899556); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_203178578, __pyx_int_126851776, __pyx_int_203525689); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_returnConverter, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__10 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(3, __pyx_int_111776469, __pyx_int_29099189, __pyx_int_240389341); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_tuple__10 = PyTuple_Pack(3, __pyx_int_238505698, __pyx_int_70301093, __pyx_int_54926798); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_CArgCalculatorEle, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__12 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(3, __pyx_int_8910864, __pyx_int_160602753, __pyx_int_195155610); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_tuple__12 = PyTuple_Pack(3, __pyx_int_40376396, __pyx_int_17371144, __pyx_int_69633521); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_CArgCalculator, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__14 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_PyArgCalculatorEl, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__16 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_PyArgCalculator, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__18 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_CArgumentCalculat, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__20 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_CallFuncPyConvert, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__22 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_DefaultCConverter, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__24 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Wrapper, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__26 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_getPyArgsName, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__28 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_returnPyArgument, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__30 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
-  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_returnPyArgumentI, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__32 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__32);
-  __Pyx_GIVEREF(__pyx_tuple__32);
-  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_returnCArgument, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__34 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__34);
-  __Pyx_GIVEREF(__pyx_tuple__34);
-  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_MultiReturn, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(1, 1, __pyx_L1_error)
+
+  /* "(tree fragment)":1
+ * def __pyx_unpickle_cArgConverter(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
+  __pyx_tuple__13 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_cArgConverter, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_pyArgConverter, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_cArgumentConverte, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_returnConverter, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_CArgCalculatorEle, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_CArgCalculator, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_PyArgCalculatorEl, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_PyArgCalculator, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__29 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__29);
+  __Pyx_GIVEREF(__pyx_tuple__29);
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_CArgumentCalculat, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__31 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__31);
+  __Pyx_GIVEREF(__pyx_tuple__31);
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_CallFuncPyConvert, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__33);
+  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_DefaultCConverter, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__35 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__35);
+  __Pyx_GIVEREF(__pyx_tuple__35);
+  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Wrapper, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__37 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__37);
+  __Pyx_GIVEREF(__pyx_tuple__37);
+  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_getPyArgsName, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__39 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__39);
+  __Pyx_GIVEREF(__pyx_tuple__39);
+  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_returnPyArgument, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__41 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__41);
+  __Pyx_GIVEREF(__pyx_tuple__41);
+  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_returnPyArgumentI, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__43 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__43);
+  __Pyx_GIVEREF(__pyx_tuple__43);
+  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_returnCArgument, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__45 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__45);
+  __Pyx_GIVEREF(__pyx_tuple__45);
+  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_MultiReturn, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_8910864 = PyInt_FromLong(8910864L); if (unlikely(!__pyx_int_8910864)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_17371144 = PyInt_FromLong(17371144L); if (unlikely(!__pyx_int_17371144)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_29099189 = PyInt_FromLong(29099189L); if (unlikely(!__pyx_int_29099189)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_40376396 = PyInt_FromLong(40376396L); if (unlikely(!__pyx_int_40376396)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_54926798 = PyInt_FromLong(54926798L); if (unlikely(!__pyx_int_54926798)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_59920447 = PyInt_FromLong(59920447L); if (unlikely(!__pyx_int_59920447)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_61218151 = PyInt_FromLong(61218151L); if (unlikely(!__pyx_int_61218151)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_69633521 = PyInt_FromLong(69633521L); if (unlikely(!__pyx_int_69633521)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_70301093 = PyInt_FromLong(70301093L); if (unlikely(!__pyx_int_70301093)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_71055545 = PyInt_FromLong(71055545L); if (unlikely(!__pyx_int_71055545)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_84062254 = PyInt_FromLong(84062254L); if (unlikely(!__pyx_int_84062254)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_98929757 = PyInt_FromLong(98929757L); if (unlikely(!__pyx_int_98929757)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_111776469 = PyInt_FromLong(111776469L); if (unlikely(!__pyx_int_111776469)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_126851776 = PyInt_FromLong(126851776L); if (unlikely(!__pyx_int_126851776)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_136427483 = PyInt_FromLong(136427483L); if (unlikely(!__pyx_int_136427483)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_154022638 = PyInt_FromLong(154022638L); if (unlikely(!__pyx_int_154022638)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_154701804 = PyInt_FromLong(154701804L); if (unlikely(!__pyx_int_154701804)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_160602753 = PyInt_FromLong(160602753L); if (unlikely(!__pyx_int_160602753)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_162899556 = PyInt_FromLong(162899556L); if (unlikely(!__pyx_int_162899556)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_174290414 = PyInt_FromLong(174290414L); if (unlikely(!__pyx_int_174290414)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_195155610 = PyInt_FromLong(195155610L); if (unlikely(!__pyx_int_195155610)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_198121326 = PyInt_FromLong(198121326L); if (unlikely(!__pyx_int_198121326)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_198986221 = PyInt_FromLong(198986221L); if (unlikely(!__pyx_int_198986221)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_203178578 = PyInt_FromLong(203178578L); if (unlikely(!__pyx_int_203178578)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_203525689 = PyInt_FromLong(203525689L); if (unlikely(!__pyx_int_203525689)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_222419149 = PyInt_FromLong(222419149L); if (unlikely(!__pyx_int_222419149)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_226705480 = PyInt_FromLong(226705480L); if (unlikely(!__pyx_int_226705480)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_228825662 = PyInt_FromLong(228825662L); if (unlikely(!__pyx_int_228825662)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_238505698 = PyInt_FromLong(238505698L); if (unlikely(!__pyx_int_238505698)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_238750788 = PyInt_FromLong(238750788L); if (unlikely(!__pyx_int_238750788)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_240389341 = PyInt_FromLong(240389341L); if (unlikely(!__pyx_int_240389341)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_251148009 = PyInt_FromLong(251148009L); if (unlikely(!__pyx_int_251148009)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_260371622 = PyInt_FromLong(260371622L); if (unlikely(!__pyx_int_260371622)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
@@ -25590,15 +25825,15 @@
   if (PyType_Ready(&__pyx_type_17OpenGL_accelerate_7wrapper_cArgConverter) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_17OpenGL_accelerate_7wrapper_cArgConverter.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_17OpenGL_accelerate_7wrapper_cArgConverter.tp_dictoffset && __pyx_type_17OpenGL_accelerate_7wrapper_cArgConverter.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_17OpenGL_accelerate_7wrapper_cArgConverter.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_17OpenGL_accelerate_7wrapper_cArgConverter, "__call__"); if (unlikely(!wrapper)) __PYX_ERR(0, 10, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_13cArgConverter___call__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_13cArgConverter___call__.doc = __pyx_doc_17OpenGL_accelerate_7wrapper_13cArgConverter___call__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_17OpenGL_accelerate_7wrapper_13cArgConverter___call__;
     }
@@ -25613,15 +25848,15 @@
   if (PyType_Ready(&__pyx_type_17OpenGL_accelerate_7wrapper_pyArgConverter) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_17OpenGL_accelerate_7wrapper_pyArgConverter.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_17OpenGL_accelerate_7wrapper_pyArgConverter.tp_dictoffset && __pyx_type_17OpenGL_accelerate_7wrapper_pyArgConverter.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_17OpenGL_accelerate_7wrapper_pyArgConverter.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_17OpenGL_accelerate_7wrapper_pyArgConverter, "__call__"); if (unlikely(!wrapper)) __PYX_ERR(0, 17, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_14pyArgConverter___call__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_14pyArgConverter___call__.doc = __pyx_doc_17OpenGL_accelerate_7wrapper_14pyArgConverter___call__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_17OpenGL_accelerate_7wrapper_14pyArgConverter___call__;
     }
@@ -25636,15 +25871,15 @@
   if (PyType_Ready(&__pyx_type_17OpenGL_accelerate_7wrapper_cArgumentConverter) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_17OpenGL_accelerate_7wrapper_cArgumentConverter.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_17OpenGL_accelerate_7wrapper_cArgumentConverter.tp_dictoffset && __pyx_type_17OpenGL_accelerate_7wrapper_cArgumentConverter.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_17OpenGL_accelerate_7wrapper_cArgumentConverter.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_17OpenGL_accelerate_7wrapper_cArgumentConverter, "__call__"); if (unlikely(!wrapper)) __PYX_ERR(0, 24, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_18cArgumentConverter___call__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_18cArgumentConverter___call__.doc = __pyx_doc_17OpenGL_accelerate_7wrapper_18cArgumentConverter___call__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_17OpenGL_accelerate_7wrapper_18cArgumentConverter___call__;
     }
@@ -25659,15 +25894,15 @@
   if (PyType_Ready(&__pyx_type_17OpenGL_accelerate_7wrapper_returnConverter) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_17OpenGL_accelerate_7wrapper_returnConverter.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_17OpenGL_accelerate_7wrapper_returnConverter.tp_dictoffset && __pyx_type_17OpenGL_accelerate_7wrapper_returnConverter.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_17OpenGL_accelerate_7wrapper_returnConverter.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_17OpenGL_accelerate_7wrapper_returnConverter, "__call__"); if (unlikely(!wrapper)) __PYX_ERR(0, 31, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_15returnConverter___call__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_15returnConverter___call__.doc = __pyx_doc_17OpenGL_accelerate_7wrapper_15returnConverter___call__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_17OpenGL_accelerate_7wrapper_15returnConverter___call__;
     }
@@ -25682,15 +25917,15 @@
   if (PyType_Ready(&__pyx_type_17OpenGL_accelerate_7wrapper_CArgCalculatorElement) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_17OpenGL_accelerate_7wrapper_CArgCalculatorElement.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_17OpenGL_accelerate_7wrapper_CArgCalculatorElement.tp_dictoffset && __pyx_type_17OpenGL_accelerate_7wrapper_CArgCalculatorElement.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_17OpenGL_accelerate_7wrapper_CArgCalculatorElement.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_17OpenGL_accelerate_7wrapper_CArgCalculatorElement, "__call__"); if (unlikely(!wrapper)) __PYX_ERR(0, 40, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_21CArgCalculatorElement_2__call__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_21CArgCalculatorElement_2__call__.doc = __pyx_doc_17OpenGL_accelerate_7wrapper_21CArgCalculatorElement_2__call__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_17OpenGL_accelerate_7wrapper_21CArgCalculatorElement_2__call__;
     }
@@ -25718,15 +25953,15 @@
   if (PyType_Ready(&__pyx_type_17OpenGL_accelerate_7wrapper_PyArgCalculatorElement) < 0) __PYX_ERR(0, 93, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_17OpenGL_accelerate_7wrapper_PyArgCalculatorElement.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_17OpenGL_accelerate_7wrapper_PyArgCalculatorElement.tp_dictoffset && __pyx_type_17OpenGL_accelerate_7wrapper_PyArgCalculatorElement.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_17OpenGL_accelerate_7wrapper_PyArgCalculatorElement.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_17OpenGL_accelerate_7wrapper_PyArgCalculatorElement, "__call__"); if (unlikely(!wrapper)) __PYX_ERR(0, 93, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_22PyArgCalculatorElement_2__call__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_22PyArgCalculatorElement_2__call__.doc = __pyx_doc_17OpenGL_accelerate_7wrapper_22PyArgCalculatorElement_2__call__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_17OpenGL_accelerate_7wrapper_22PyArgCalculatorElement_2__call__;
     }
@@ -25769,25 +26004,25 @@
   if (PyType_Ready(&__pyx_type_17OpenGL_accelerate_7wrapper_CallFuncPyConverter) < 0) __PYX_ERR(0, 204, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_17OpenGL_accelerate_7wrapper_CallFuncPyConverter.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_17OpenGL_accelerate_7wrapper_CallFuncPyConverter.tp_dictoffset && __pyx_type_17OpenGL_accelerate_7wrapper_CallFuncPyConverter.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_17OpenGL_accelerate_7wrapper_CallFuncPyConverter.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_17OpenGL_accelerate_7wrapper_CallFuncPyConverter, "__init__"); if (unlikely(!wrapper)) __PYX_ERR(0, 204, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_19CallFuncPyConverter___init__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_19CallFuncPyConverter___init__.doc = __pyx_doc_17OpenGL_accelerate_7wrapper_19CallFuncPyConverter___init__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_17OpenGL_accelerate_7wrapper_19CallFuncPyConverter___init__;
     }
   }
   #endif
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_17OpenGL_accelerate_7wrapper_CallFuncPyConverter, "__repr__"); if (unlikely(!wrapper)) __PYX_ERR(0, 204, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_19CallFuncPyConverter_2__repr__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_19CallFuncPyConverter_2__repr__.doc = __pyx_doc_17OpenGL_accelerate_7wrapper_19CallFuncPyConverter_2__repr__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_17OpenGL_accelerate_7wrapper_19CallFuncPyConverter_2__repr__;
     }
@@ -25804,15 +26039,15 @@
   if (PyType_Ready(&__pyx_type_17OpenGL_accelerate_7wrapper_DefaultCConverter) < 0) __PYX_ERR(0, 219, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_17OpenGL_accelerate_7wrapper_DefaultCConverter.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_17OpenGL_accelerate_7wrapper_DefaultCConverter.tp_dictoffset && __pyx_type_17OpenGL_accelerate_7wrapper_DefaultCConverter.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_17OpenGL_accelerate_7wrapper_DefaultCConverter.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_17OpenGL_accelerate_7wrapper_DefaultCConverter, "__init__"); if (unlikely(!wrapper)) __PYX_ERR(0, 219, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_17DefaultCConverter___init__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_17OpenGL_accelerate_7wrapper_17DefaultCConverter___init__.doc = __pyx_doc_17OpenGL_accelerate_7wrapper_17DefaultCConverter___init__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_17OpenGL_accelerate_7wrapper_17DefaultCConverter___init__;
     }
@@ -27955,25 +28190,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
 #endif
+    if (getstate) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+#else
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
+#endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -28010,14 +28263,16 @@
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
@@ -28145,14 +28400,20 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
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
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -28208,22 +28469,32 @@
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
@@ -28958,19 +29229,41 @@
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to unsigned int");
     return (unsigned int) -1;
 }
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
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
```

### Comparing `PyOpenGL-accelerate-3.1.6/src/wrapper.pyx` & `PyOpenGL-accelerate-3.1.7/src/wrapper.pyx`

 * *Files identical despite different names*

