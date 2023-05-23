# Comparing `tmp/numpy_dataframe-0.1.6.tar.gz` & `tmp/numpy_dataframe-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpy_dataframe-0.1.6.tar", last modified: Tue Mar  7 12:33:32 2023, max compression
+gzip compressed data, was "numpy_dataframe-0.1.7.tar", last modified: Tue May 23 12:44:59 2023, max compression
```

## Comparing `numpy_dataframe-0.1.6.tar` & `numpy_dataframe-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-03-07 12:33:32.492146 numpy_dataframe-0.1.6/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1094 2022-10-30 20:08:54.000000 numpy_dataframe-0.1.6/LICENSE
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      729 2023-03-07 12:33:32.492146 numpy_dataframe-0.1.6/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      440 2022-10-30 20:14:15.000000 numpy_dataframe-0.1.6/README.md
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-03-07 12:33:32.488146 numpy_dataframe-0.1.6/numpy_dataframe/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      155 2023-03-07 12:30:31.000000 numpy_dataframe-0.1.6/numpy_dataframe/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    17466 2022-12-01 13:53:37.000000 numpy_dataframe-0.1.6/numpy_dataframe/numpy_dataframe.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-03-07 12:33:32.492146 numpy_dataframe-0.1.6/numpy_dataframe.egg-info/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      729 2023-03-07 12:33:32.000000 numpy_dataframe-0.1.6/numpy_dataframe.egg-info/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      283 2023-03-07 12:33:32.000000 numpy_dataframe-0.1.6/numpy_dataframe.egg-info/SOURCES.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-03-07 12:33:32.000000 numpy_dataframe-0.1.6/numpy_dataframe.egg-info/dependency_links.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2022-10-30 20:16:12.000000 numpy_dataframe-0.1.6/numpy_dataframe.egg-info/not-zip-safe
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       16 2023-03-07 12:33:32.000000 numpy_dataframe-0.1.6/numpy_dataframe.egg-info/top_level.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-03-07 12:33:32.492146 numpy_dataframe-0.1.6/setup.cfg
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      450 2023-03-07 12:30:40.000000 numpy_dataframe-0.1.6/setup.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-23 12:44:59.801394 numpy_dataframe-0.1.7/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1094 2022-10-30 20:08:54.000000 numpy_dataframe-0.1.7/LICENSE
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      729 2023-05-23 12:44:59.801394 numpy_dataframe-0.1.7/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      440 2022-10-30 20:14:15.000000 numpy_dataframe-0.1.7/README.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-23 12:44:59.797394 numpy_dataframe-0.1.7/numpy_dataframe/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      155 2023-05-23 12:43:55.000000 numpy_dataframe-0.1.7/numpy_dataframe/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    18603 2023-05-23 12:43:42.000000 numpy_dataframe-0.1.7/numpy_dataframe/numpy_dataframe.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    17512 2023-05-18 09:27:23.000000 numpy_dataframe-0.1.7/numpy_dataframe/numpy_dataframe_unknown_mod.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-23 12:44:59.801394 numpy_dataframe-0.1.7/numpy_dataframe.egg-info/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      729 2023-05-23 12:44:59.000000 numpy_dataframe-0.1.7/numpy_dataframe.egg-info/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      330 2023-05-23 12:44:59.000000 numpy_dataframe-0.1.7/numpy_dataframe.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-23 12:44:59.000000 numpy_dataframe-0.1.7/numpy_dataframe.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2022-10-30 20:16:12.000000 numpy_dataframe-0.1.7/numpy_dataframe.egg-info/not-zip-safe
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       16 2023-05-23 12:44:59.000000 numpy_dataframe-0.1.7/numpy_dataframe.egg-info/top_level.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-23 12:44:59.801394 numpy_dataframe-0.1.7/setup.cfg
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      450 2023-05-23 12:43:50.000000 numpy_dataframe-0.1.7/setup.py
```

### Comparing `numpy_dataframe-0.1.6/LICENSE` & `numpy_dataframe-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `numpy_dataframe-0.1.6/PKG-INFO` & `numpy_dataframe-0.1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numpy_dataframe
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple dataframe implementation using numpy as its basic element
 Home-page: UNKNOWN
 Author: Carlos Molinero
 Author-email: 
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `numpy_dataframe-0.1.6/numpy_dataframe/numpy_dataframe.py` & `numpy_dataframe-0.1.7/numpy_dataframe/numpy_dataframe_unknown_mod.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import numpy as np
 import pandas as pd
 from copy import deepcopy
 import numpy_groupies as npg
 import time
 from collections import defaultdict
-import numba as nb
+# import numba as nb
 # import numpy_helper as nph
 
-int_array = nb.types.int64[:]
-int_list = nb.types.ListType(nb.types.int64)
+# int_array = nb.types.int64[:]
+# int_list = nb.types.ListType(nb.types.int64)
 
-@nb.jit(nopython=True)
-def ordered_clusters_group_by(l,current_type):
-    indices = nb.typed.Dict.empty(
-        key_type=current_type,
-        value_type=int_list
-    )
-
-    for i in np.arange(l.shape[0]):
-        try:
-            indices[l[i]].append(i)
-        except:
-            indices[l[i]] = nb.typed.List([i])
-
-    indices_list = np.empty_like(l,np.int64)
-    i = 0
-    ks = np.empty(len(indices.keys()))
-    for k in indices.keys():
-        ks[i] = k
-        for h in indices[k]:
-            indices_list[h] = i
-        i += 1
-    return ks,indices_list
+# @nb.jit(nopython=True)
+# def ordered_clusters_group_by(l,current_type):
+#     indices = nb.typed.Dict.empty(
+#         key_type=current_type,
+#         value_type=int_list
+#     )
+
+#     for i in np.arange(l.shape[0]):
+#         try:
+#             indices[l[i]].append(i)
+#         except:
+#             indices[l[i]] = nb.typed.List([i])
+
+#     indices_list = np.empty_like(l,np.int64)
+#     i = 0
+#     ks = np.empty(len(indices.keys()))
+#     for k in indices.keys():
+#         ks[i] = k
+#         for h in indices[k]:
+#             indices_list[h] = i
+#         i += 1
+#     return ks,indices_list
 
 
 class DataFrame:
     def __new__(cls, *args, **kwargs):
         return super().__new__(cls)
     def __init__(self):
         super(DataFrame, self).__setattr__('__d__', {})
```

### Comparing `numpy_dataframe-0.1.6/numpy_dataframe.egg-info/PKG-INFO` & `numpy_dataframe-0.1.7/numpy_dataframe.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numpy-dataframe
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple dataframe implementation using numpy as its basic element
 Home-page: UNKNOWN
 Author: Carlos Molinero
 Author-email: 
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

