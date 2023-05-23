# Comparing `tmp/qm_tools_aw-1.1.0.tar.gz` & `tmp/qm_tools_aw-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qm_tools_aw-1.1.0.tar", last modified: Tue May 23 15:44:46 2023, max compression
+gzip compressed data, was "qm_tools_aw-1.1.1.tar", last modified: Tue May 23 17:01:28 2023, max compression
```

## Comparing `qm_tools_aw-1.1.0.tar` & `qm_tools_aw-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-05-23 15:44:46.506312 qm_tools_aw-1.1.0/
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)     1074 2023-01-17 19:48:33.000000 qm_tools_aw-1.1.0/LICENSE
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      689 2023-05-23 15:44:46.506312 qm_tools_aw-1.1.0/PKG-INFO
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      107 2023-01-17 19:48:33.000000 qm_tools_aw-1.1.0/README.md
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      649 2023-05-23 15:44:05.000000 qm_tools_aw-1.1.0/pyproject.toml
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      202 2023-05-23 15:44:46.508312 qm_tools_aw-1.1.0/setup.cfg
-drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-05-23 15:44:46.470312 qm_tools_aw-1.1.0/src/
-drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-05-23 15:44:46.487312 qm_tools_aw-1.1.0/src/qm_tools_aw/
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)       20 2023-03-10 20:29:53.000000 qm_tools_aw-1.1.0/src/qm_tools_aw/__init__.py
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)     7927 2023-05-16 20:39:29.000000 qm_tools_aw-1.1.0/src/qm_tools_aw/tools.py
-drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-05-23 15:44:46.499312 qm_tools_aw-1.1.0/src/qm_tools_aw.egg-info/
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      689 2023-05-23 15:44:46.000000 qm_tools_aw-1.1.0/src/qm_tools_aw.egg-info/PKG-INFO
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      323 2023-05-23 15:44:46.000000 qm_tools_aw-1.1.0/src/qm_tools_aw.egg-info/SOURCES.txt
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)        1 2023-05-23 15:44:46.000000 qm_tools_aw-1.1.0/src/qm_tools_aw.egg-info/dependency_links.txt
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)       32 2023-05-23 15:44:46.000000 qm_tools_aw-1.1.0/src/qm_tools_aw.egg-info/requires.txt
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)       12 2023-05-23 15:44:46.000000 qm_tools_aw-1.1.0/src/qm_tools_aw.egg-info/top_level.txt
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)        1 2023-01-18 18:58:47.000000 qm_tools_aw-1.1.0/src/qm_tools_aw.egg-info/zip-safe
+drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-05-23 17:01:28.774217 qm_tools_aw-1.1.1/
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)     1074 2023-01-17 19:48:33.000000 qm_tools_aw-1.1.1/LICENSE
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      689 2023-05-23 17:01:28.775217 qm_tools_aw-1.1.1/PKG-INFO
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      107 2023-01-17 19:48:33.000000 qm_tools_aw-1.1.1/README.md
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      649 2023-05-23 17:00:42.000000 qm_tools_aw-1.1.1/pyproject.toml
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      202 2023-05-23 17:01:28.779217 qm_tools_aw-1.1.1/setup.cfg
+drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-05-23 17:01:28.660216 qm_tools_aw-1.1.1/src/
+drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-05-23 17:01:28.699216 qm_tools_aw-1.1.1/src/qm_tools_aw/
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)       20 2023-03-10 20:29:53.000000 qm_tools_aw-1.1.1/src/qm_tools_aw/__init__.py
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)     8488 2023-05-23 16:52:09.000000 qm_tools_aw-1.1.1/src/qm_tools_aw/tools.py
+drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-05-23 17:01:28.772217 qm_tools_aw-1.1.1/src/qm_tools_aw.egg-info/
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      689 2023-05-23 17:01:28.000000 qm_tools_aw-1.1.1/src/qm_tools_aw.egg-info/PKG-INFO
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      323 2023-05-23 17:01:28.000000 qm_tools_aw-1.1.1/src/qm_tools_aw.egg-info/SOURCES.txt
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)        1 2023-05-23 17:01:28.000000 qm_tools_aw-1.1.1/src/qm_tools_aw.egg-info/dependency_links.txt
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)       32 2023-05-23 17:01:28.000000 qm_tools_aw-1.1.1/src/qm_tools_aw.egg-info/requires.txt
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)       12 2023-05-23 17:01:28.000000 qm_tools_aw-1.1.1/src/qm_tools_aw.egg-info/top_level.txt
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)        1 2023-01-18 18:58:47.000000 qm_tools_aw-1.1.1/src/qm_tools_aw.egg-info/zip-safe
```

### Comparing `qm_tools_aw-1.1.0/LICENSE` & `qm_tools_aw-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qm_tools_aw-1.1.0/PKG-INFO` & `qm_tools_aw-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qm_tools_aw
-Version: 1.1.0
+Version: 1.1.1
 Summary: Provides some functions that I have found value in reusing for quantum chemistry related tasks.
 Author-email: "Austin M. Wallace" <awallace43@gatech.edu>
 Project-URL: Homepage, https://github.com/Awallace3/qm_tools
 Project-URL: Bug Tracker, https://github.com/Awallace3/qm_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qm_tools_aw-1.1.0/pyproject.toml` & `qm_tools_aw-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qm_tools_aw"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Austin M. Wallace", email="awallace43@gatech.edu" },
 ]
 description = "Provides some functions that I have found value in reusing for quantum chemistry related tasks."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `qm_tools_aw-1.1.0/src/qm_tools_aw/tools.py` & `qm_tools_aw-1.1.1/src/qm_tools_aw/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,13 @@
 import pickle
 import numpy as np
 from periodictable import elements
 import qcelemental as qcel
 import pandas as pd
 
-def save_pkl(file_name, obj):
-    with open(file_name, "wb") as fobj:
-        pickle.dump(obj, fobj)
-
-
-def load_pkl(file_name):
-    with open(file_name, "rb") as fobj:
-        return pickle.load(fobj)
-
 
 def create_pt_dict():
     """
     create_pt_dict creates dictionary for string elements to atomic number.
     """
     el_dc = {}
     for el in elements:
@@ -43,20 +34,20 @@
     return w
 
 
 def convert_schr_row_to_mol(r) -> qcel.models.Molecule:
     """
     convert_schr_row_to_mol
     """
-    ma, mb = r['monAs'], r['monBs']
-    g1, g2 = r['Geometry'][ma], r['Geometry'][mb]
+    ma, mb = r["monAs"], r["monBs"]
+    g1, g2 = r["Geometry"][ma], r["Geometry"][mb]
     m1 = f"{r['charges'][1][0]} {r['charges'][1][1]}\n"
-    m1 += print_cartesians_pos_carts(g1[:,0], g1[:,1:], only_results=True)
+    m1 += print_cartesians_pos_carts(g1[:, 0], g1[:, 1:], only_results=True)
     m2 = f"{r['charges'][2][0]} {r['charges'][2][1]}\n"
-    m2 += print_cartesians_pos_carts(g2[:,0], g2[:,1:], only_results=True)
+    m2 += print_cartesians_pos_carts(g2[:, 0], g2[:, 1:], only_results=True)
     mol = qcel.models.Molecule.from_data(m1 + "--\n" + m2)
     return mol
 
 
 def string_carts_to_np(geom):
     geom = geom.split("\n")
     if geom[0] == "":
@@ -142,45 +133,79 @@
     print_cartesians(m1)
     print(f"--")
     print(*c2)
     print_cartesians(m2)
     return
 
 
-def print_cartesians_pos_carts(pos: np.array, carts: np.array, only_results=False):
+def print_cartesians_pos_carts(
+    pos: np.array, carts: np.array, only_results=False, el_attach=None
+):
     """
     prints a 2-D numpy array in a nicer format
     """
     if not only_results:
         print()
     lines = ""
     for n, r in enumerate(carts):
         x, y, z = r
-        line = "{}\t{:.10f}\t{:.10f}\t{:.10f}".format(int(pos[n]), x, y, z)
+        el = str(int(pos[n]))
+        if el_attach is not None:
+            el += el_attach
+        line = "{}\t{:.10f}\t{:.10f}\t{:.10f}".format(el, x, y, z)
         lines += line + "\n"
         if not only_results:
             print(line)
     if not only_results:
         print()
     return lines
 
+
+def print_cartesians_pos_carts_symbols(
+    pos: np.array,
+    carts: np.array,
+    only_results=False,
+    el_attach=None,
+    el_dc=create_el_num_to_symbol(),
+):
+    """
+    prints a 2-D numpy array in a nicer format
+    """
+    if not only_results:
+        print()
+    lines = ""
+    for n, r in enumerate(carts):
+        x, y, z = r
+        el = el_dc[int(pos[n])]
+        if el_attach is not None:
+            el += el_attach
+        line = "{}\t{:.10f}\t{:.10f}\t{:.10f}".format(el, x, y, z)
+        lines += line + "\n"
+        if not only_results:
+            print(line)
+    if not only_results:
+        print()
+    return lines
+
+
 # def return_cartesians_pos_carts(pos: np.array, carts: np.array):
 #     """
 #     prints a 2-D numpy array in a nicer format
 #     """
 #     print()
 #     lines = ""
 #     for n, r in enumerate(carts):
 #         x, y, z = r
 #         line = "{}\t{:.10f}\t{:.10f}\t{:.10f}".format(int(pos[n]), x, y, z)
 #         lines += line + "\n"
 #         print(line)
 #     print()
 #     return lines
 
+
 def carts_to_xyz(pos: np.array, carts: np.array, el_dc=create_el_num_to_symbol()):
     """
     creates xyz file from pos and carts
     """
     out = ""
     start = f"{len(pos)}\n\n"
     out += start
@@ -215,15 +240,17 @@
 
 
 def read_pickle(fname="data.pickle"):
     with open(fname, "rb") as handle:
         return pickle.load(handle)
 
 
-def read_xyz_to_pos_carts(xyz_path="mol.xyz",) -> (np.array, np.array):
+def read_xyz_to_pos_carts(
+    xyz_path="mol.xyz",
+) -> (np.array, np.array):
     """
     read_xyz_to_pos_carts reads xyz file and returns pos and carts
     """
     el_dc = create_pt_dict()
     with open(xyz_path, "r") as f:
         d = f.readlines()[2:]
 
@@ -236,15 +263,17 @@
             el = el_dc[l[0]]
         x, y, z = float(l[1]), float(l[2]), float(l[3])
         pos.append(el)
         carts.append([x, y, z])
     return np.array(pos), np.array(carts)
 
 
-def convert_geom_str_to_dimer_splits(geom, units_angstroms=True) -> [np.array, np.array, np.array, np.array]:
+def convert_geom_str_to_dimer_splits(
+    geom, units_angstroms=True
+) -> [np.array, np.array, np.array, np.array]:
 
     """
     convert_str_to_dimer_splits takes in geom as a STRING as a list or single string
     and makes Molecule objects
 
     returning order [ZA, ZB, RA, RB]
     """
```

### Comparing `qm_tools_aw-1.1.0/src/qm_tools_aw.egg-info/PKG-INFO` & `qm_tools_aw-1.1.1/src/qm_tools_aw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qm-tools-aw
-Version: 1.1.0
+Version: 1.1.1
 Summary: Provides some functions that I have found value in reusing for quantum chemistry related tasks.
 Author-email: "Austin M. Wallace" <awallace43@gatech.edu>
 Project-URL: Homepage, https://github.com/Awallace3/qm_tools
 Project-URL: Bug Tracker, https://github.com/Awallace3/qm_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

