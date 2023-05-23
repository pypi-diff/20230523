# Comparing `tmp/vot-trax-4.0.0.tar.gz` & `tmp/vot-trax-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vot-trax-4.0.0.tar", last modified: Thu May  4 21:27:08 2023, max compression
+gzip compressed data, was "vot-trax-4.0.1.tar", last modified: Tue May 23 12:36:22 2023, max compression
```

## Comparing `vot-trax-4.0.0.tar` & `vot-trax-4.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-04 21:27:08.575316 vot-trax-4.0.0/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1053 2023-05-04 21:27:08.575316 vot-trax-4.0.0/PKG-INFO
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      544 2023-05-04 21:26:46.047421 vot-trax-4.0.0/README.rst
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        6 2023-05-04 21:26:06.363611 vot-trax-4.0.0/VERSION
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3126 2023-05-04 21:26:06.363611 vot-trax-4.0.0/setup.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-04 21:27:08.575316 vot-trax-4.0.0/trax/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9243 2023-05-04 21:26:46.063421 vot-trax-4.0.0/trax/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    54378 2023-05-04 21:26:46.067421 vot-trax-4.0.0/trax/_ctypes.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6953 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/base64.c
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      335 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/base64.h
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4548 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/buffer.h
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7944 2023-05-04 21:26:46.067421 vot-trax-4.0.0/trax/client.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1562 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/debug.c
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      971 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/debug.h
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8029 2023-05-04 21:26:46.067421 vot-trax-4.0.0/trax/image.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    23442 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/message.c
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1810 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/message.h
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    30473 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/region.c
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3364 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/region.h
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8687 2023-05-04 21:26:46.067421 vot-trax-4.0.0/trax/region.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5967 2023-05-04 21:26:46.067421 vot-trax-4.0.0/trax/server.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14754 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/strmap.c
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12968 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/strmap.h
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    58417 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/trax.c
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    36170 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/trax.h
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    24834 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/traxpp.cpp
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-23 12:36:22.460717 vot-trax-4.0.1/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1053 2023-05-23 12:36:22.460717 vot-trax-4.0.1/PKG-INFO
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      544 2023-05-04 21:26:46.047421 vot-trax-4.0.1/README.rst
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        6 2023-05-23 12:34:41.272537 vot-trax-4.0.1/VERSION
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3126 2023-05-04 21:26:06.363611 vot-trax-4.0.1/setup.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-23 12:36:22.460717 vot-trax-4.0.1/trax/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9243 2023-05-23 12:13:30.166442 vot-trax-4.0.1/trax/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    54378 2023-05-04 21:26:46.067421 vot-trax-4.0.1/trax/_ctypes.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6953 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/base64.c
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      335 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/base64.h
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4548 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/buffer.h
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7944 2023-05-23 12:13:16.466424 vot-trax-4.0.1/trax/client.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1562 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/debug.c
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      971 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/debug.h
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8029 2023-05-04 21:26:46.067421 vot-trax-4.0.1/trax/image.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    23442 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/message.c
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1810 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/message.h
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    30473 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/region.c
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3364 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/region.h
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8687 2023-05-04 21:26:46.067421 vot-trax-4.0.1/trax/region.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5967 2023-05-04 21:26:46.067421 vot-trax-4.0.1/trax/server.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14754 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/strmap.c
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12968 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/strmap.h
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    58455 2023-05-23 12:11:45.642304 vot-trax-4.0.1/trax/trax.c
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    36170 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/trax.h
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    24834 2023-05-04 21:26:46.083421 vot-trax-4.0.1/trax/traxpp.cpp
```

### Comparing `vot-trax-4.0.0/PKG-INFO` & `vot-trax-4.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: vot-trax
-Version: 4.0.0
+Version: 4.0.1
 Summary: TraX protocol reference implementation wrapper for Python
 Home-page: https://github.com/votchallenge/trax/
 Author: Luka Cehovin Zajc
 Author-email: luka.cehovin@gmail.com
 License: UNKNOWN
 Description: 
         `Visual Tracking eXchange protocol <http://prints.vicos.si/publications/311/>`_ is a simple protocol that enables easier evaluation of computer vision tracking algorithms. The basic idea is that a tracker communicates with the evaluation software using a set of text commands over the (standard) input/output streams or TCP sockets.
```

### Comparing `vot-trax-4.0.0/README.rst` & `vot-trax-4.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.0/setup.py` & `vot-trax-4.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.0/trax/__init__.py` & `vot-trax-4.0.1/trax/__init__.py`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.0/trax/_ctypes.py` & `vot-trax-4.0.1/trax/_ctypes.py`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.0/trax/base64.c` & `vot-trax-4.0.1/trax/base64.c`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.0/trax/buffer.h` & `vot-trax-4.0.1/trax/buffer.h`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.0/trax/client.py` & `vot-trax-4.0.1/trax/client.py`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.0/trax/debug.c` & `vot-trax-4.0.1/trax/debug.c`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.0/trax/debug.h` & `vot-trax-4.0.1/trax/debug.h`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.0/trax/image.py` & `vot-trax-4.0.1/trax/image.py`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.0/trax/message.c` & `vot-trax-4.0.1/trax/message.c`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.0/trax/message.h` & `vot-trax-4.0.1/trax/message.h`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.0/trax/region.c` & `vot-trax-4.0.1/trax/region.c`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.0/trax/region.h` & `vot-trax-4.0.1/trax/region.h`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.0/trax/region.py` & `vot-trax-4.0.1/trax/region.py`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.0/trax/server.py` & `vot-trax-4.0.1/trax/server.py`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.0/trax/strmap.c` & `vot-trax-4.0.1/trax/strmap.c`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.0/trax/strmap.h` & `vot-trax-4.0.1/trax/strmap.h`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.0/trax/trax.c` & `vot-trax-4.0.1/trax/trax.c`

 * *Files 0% similar despite different names*

```diff
@@ -807,14 +807,15 @@
                 trax_properties_release(&tmp_properties);
                 trax_object_list_release(objects);
                 result = TRAX_ERROR;
                 break;
             }
 
             trax_object_list_set((*objects), i, _region);
+            region_release(&_region);
             copy_properties(tmp_properties, trax_object_list_properties((*objects), i), COPY_ALL | COPY_OVERWRITE);
 
         } else if (result == TRAX_QUIT) {
 
             if (list_size(arguments) != 0) {
                 list_destroy(&arguments);
                 trax_properties_release(&tmp_properties);
```

### Comparing `vot-trax-4.0.0/trax/trax.h` & `vot-trax-4.0.1/trax/trax.h`

 * *Files identical despite different names*

### Comparing `vot-trax-4.0.0/trax/traxpp.cpp` & `vot-trax-4.0.1/trax/traxpp.cpp`

 * *Files identical despite different names*

