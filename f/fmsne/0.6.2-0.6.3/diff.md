# Comparing `tmp/fmsne-0.6.2.tar.gz` & `tmp/fmsne-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmsne-0.6.2.tar", last modified: Sun May 21 14:59:38 2023, max compression
+gzip compressed data, was "fmsne-0.6.3.tar", last modified: Tue May 23 07:59:04 2023, max compression
```

## Comparing `fmsne-0.6.2.tar` & `fmsne-0.6.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 lgatto    (1001) lgatto    (1001)        0 2023-05-21 14:59:38.329306 fmsne-0.6.2/
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     1195 2023-05-17 17:30:25.000000 fmsne-0.6.2/LICENCE.md
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       67 2023-05-17 17:30:25.000000 fmsne-0.6.2/MANIFEST.in
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8788 2023-05-21 14:59:38.329306 fmsne-0.6.2/PKG-INFO
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8200 2023-05-17 17:30:25.000000 fmsne-0.6.2/README.md
-drwxrwxr-x   0 lgatto    (1001) lgatto    (1001)        0 2023-05-21 14:59:38.329306 fmsne-0.6.2/fmsne/
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       44 2023-05-21 14:59:28.000000 fmsne-0.6.2/fmsne/__init__.py
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     3380 2023-05-17 17:30:25.000000 fmsne-0.6.2/fmsne/arithmetic_ansi.h
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8830 2023-05-17 17:30:25.000000 fmsne-0.6.2/fmsne/arithmetic_sse_double.h
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     9070 2023-05-17 17:30:25.000000 fmsne-0.6.2/fmsne/arithmetic_sse_float.h
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    41058 2023-05-21 14:59:28.000000 fmsne-0.6.2/fmsne/fmsne.py
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)  2008886 2023-05-21 12:37:39.000000 fmsne-0.6.2/fmsne/fmsne_implem.cpp
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)   171438 2023-05-17 17:30:25.000000 fmsne-0.6.2/fmsne/fmsne_implem.pyx
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    41095 2023-05-17 17:30:25.000000 fmsne-0.6.2/fmsne/lbfgs.c
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    32648 2023-05-17 17:30:25.000000 fmsne-0.6.2/fmsne/lbfgs.h
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    19367 2023-05-17 17:30:25.000000 fmsne-0.6.2/fmsne/vptree.h
-drwxrwxr-x   0 lgatto    (1001) lgatto    (1001)        0 2023-05-21 14:59:38.329306 fmsne-0.6.2/fmsne.egg-info/
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8788 2023-05-21 14:59:38.000000 fmsne-0.6.2/fmsne.egg-info/PKG-INFO
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)      400 2023-05-21 14:59:38.000000 fmsne-0.6.2/fmsne.egg-info/SOURCES.txt
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)        1 2023-05-21 14:59:38.000000 fmsne-0.6.2/fmsne.egg-info/dependency_links.txt
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       49 2023-05-21 14:59:38.000000 fmsne-0.6.2/fmsne.egg-info/requires.txt
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       19 2023-05-21 14:59:38.000000 fmsne-0.6.2/fmsne.egg-info/top_level.txt
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)      579 2023-05-21 14:59:38.329306 fmsne-0.6.2/setup.cfg
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     1017 2023-05-21 13:08:54.000000 fmsne-0.6.2/setup.py
+drwxrwxr-x   0 lgatto    (1001) lgatto    (1001)        0 2023-05-23 07:59:04.079030 fmsne-0.6.3/
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     1195 2023-05-17 17:30:25.000000 fmsne-0.6.3/LICENCE.md
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       67 2023-05-17 17:30:25.000000 fmsne-0.6.3/MANIFEST.in
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8788 2023-05-23 07:59:04.079030 fmsne-0.6.3/PKG-INFO
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8200 2023-05-17 17:30:25.000000 fmsne-0.6.3/README.md
+drwxrwxr-x   0 lgatto    (1001) lgatto    (1001)        0 2023-05-23 07:59:04.079030 fmsne-0.6.3/fmsne/
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       44 2023-05-23 07:42:20.000000 fmsne-0.6.3/fmsne/__init__.py
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     3380 2023-05-17 17:30:25.000000 fmsne-0.6.3/fmsne/arithmetic_ansi.h
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8830 2023-05-17 17:30:25.000000 fmsne-0.6.3/fmsne/arithmetic_sse_double.h
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     9070 2023-05-17 17:30:25.000000 fmsne-0.6.3/fmsne/arithmetic_sse_float.h
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    40938 2023-05-23 07:28:55.000000 fmsne-0.6.3/fmsne/fmsne.py
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)  2008886 2023-05-21 12:37:39.000000 fmsne-0.6.3/fmsne/fmsne_implem.cpp
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)   171438 2023-05-17 17:30:25.000000 fmsne-0.6.3/fmsne/fmsne_implem.pyx
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    41095 2023-05-17 17:30:25.000000 fmsne-0.6.3/fmsne/lbfgs.c
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    32648 2023-05-17 17:30:25.000000 fmsne-0.6.3/fmsne/lbfgs.h
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    19367 2023-05-17 17:30:25.000000 fmsne-0.6.3/fmsne/vptree.h
+drwxrwxr-x   0 lgatto    (1001) lgatto    (1001)        0 2023-05-23 07:59:04.079030 fmsne-0.6.3/fmsne.egg-info/
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8788 2023-05-23 07:59:03.000000 fmsne-0.6.3/fmsne.egg-info/PKG-INFO
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)      400 2023-05-23 07:59:03.000000 fmsne-0.6.3/fmsne.egg-info/SOURCES.txt
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)        1 2023-05-23 07:59:03.000000 fmsne-0.6.3/fmsne.egg-info/dependency_links.txt
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       49 2023-05-23 07:59:03.000000 fmsne-0.6.3/fmsne.egg-info/requires.txt
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       19 2023-05-23 07:59:03.000000 fmsne-0.6.3/fmsne.egg-info/top_level.txt
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)      579 2023-05-23 07:59:04.079030 fmsne-0.6.3/setup.cfg
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     1017 2023-05-21 13:08:54.000000 fmsne-0.6.3/setup.py
```

### Comparing `fmsne-0.6.2/LICENCE.md` & `fmsne-0.6.3/LICENCE.md`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.2/PKG-INFO` & `fmsne-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmsne
-Version: 0.6.2
+Version: 0.6.3
 Summary: Fast Multi-Scale Neighbour Embedding
 Home-page: https://github.com/cdebodt/Fast_Multi-scale_NE
 Author: Cyril de Bodt
 Author-email: cyril.debodt@uclouvain.be
 Maintainer: Laurent Gatto
 Maintainer-email: laurent.gatto@uclouvain.be
 License: MIT
```

### Comparing `fmsne-0.6.2/README.md` & `fmsne-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.2/fmsne/arithmetic_ansi.h` & `fmsne-0.6.3/fmsne/arithmetic_ansi.h`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.2/fmsne/arithmetic_sse_double.h` & `fmsne-0.6.3/fmsne/arithmetic_sse_double.h`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.2/fmsne/arithmetic_sse_float.h` & `fmsne-0.6.3/fmsne/arithmetic_sse_float.h`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.2/fmsne/fmsne.py` & `fmsne-0.6.3/fmsne/fmsne.py`

 * *Files 2% similar despite different names*

```diff
@@ -913,15 +913,14 @@
     """
     return eval_dr_quality(d_hd = eucl_dist_matr(X),
                            d_ld = eucl_dist_matr(Y))
 
 
 def eval_red_rnx_auc_from_data(X, Y, Kup = 10000):
     """
-    Computes the pairwise Euclidean distances of HD and LD
-    embeddings X and Y and then computes the reduced DR quality
-    assessment criteria R_{NX}(K) and AUC. See `red_rnx_auc` and
-    `eval_dr_quality` functions for details.
+    Computes the reduced DR quality assessment criteria R_{NX}(K)
+    and AUC. See `red_rnx_auc` and `eval_dr_quality` functions for
+    details.
     """
-    return red_rnx_auc(X_hds = eucl_dist_matr(X),
-                       X_lds = eucl_dist_matr(Y),
+    return red_rnx_auc(X_hds = X,
+                       X_lds = Y,
                        Kup = Kup)
```

### Comparing `fmsne-0.6.2/fmsne/fmsne_implem.cpp` & `fmsne-0.6.3/fmsne/fmsne_implem.cpp`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.2/fmsne/fmsne_implem.pyx` & `fmsne-0.6.3/fmsne/fmsne_implem.pyx`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.2/fmsne/lbfgs.c` & `fmsne-0.6.3/fmsne/lbfgs.c`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.2/fmsne/lbfgs.h` & `fmsne-0.6.3/fmsne/lbfgs.h`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.2/fmsne/vptree.h` & `fmsne-0.6.3/fmsne/vptree.h`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.2/fmsne.egg-info/PKG-INFO` & `fmsne-0.6.3/fmsne.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmsne
-Version: 0.6.2
+Version: 0.6.3
 Summary: Fast Multi-Scale Neighbour Embedding
 Home-page: https://github.com/cdebodt/Fast_Multi-scale_NE
 Author: Cyril de Bodt
 Author-email: cyril.debodt@uclouvain.be
 Maintainer: Laurent Gatto
 Maintainer-email: laurent.gatto@uclouvain.be
 License: MIT
```

### Comparing `fmsne-0.6.2/setup.cfg` & `fmsne-0.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.2/setup.py` & `fmsne-0.6.3/setup.py`

 * *Files identical despite different names*

