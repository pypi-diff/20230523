# Comparing `tmp/pysparse-array-1.0.6.tar.gz` & `tmp/pysparse-array-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparse-array-1.0.6.tar", last modified: Tue May 23 14:27:45 2023, max compression
+gzip compressed data, was "pysparse-array-1.0.7.tar", last modified: Tue May 23 16:53:52 2023, max compression
```

## Comparing `pysparse-array-1.0.6.tar` & `pysparse-array-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-23 14:27:45.886987 pysparse-array-1.0.6/
--rw-r--r--   0 thomasfrost   (502) staff       (20)     3152 2023-05-23 14:26:45.000000 pysparse-array-1.0.6/HISTORY.md
--rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-1.0.6/LICENSE.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       19 2023-05-16 11:11:47.000000 pysparse-array-1.0.6/MANIFEST.in
--rw-r--r--   0 thomasfrost   (502) staff       (20)     5399 2023-05-23 14:27:45.882730 pysparse-array-1.0.6/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)     4694 2023-05-20 21:17:03.000000 pysparse-array-1.0.6/README.md
--rw-r--r--   0 thomasfrost   (502) staff       (20)      763 2023-05-23 14:23:31.000000 pysparse-array-1.0.6/pyproject.toml
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-23 14:27:45.791412 pysparse-array-1.0.6/pysparse_array.egg-info/
--rw-r--r--   0 thomasfrost   (502) staff       (20)     5399 2023-05-23 14:27:45.000000 pysparse-array-1.0.6/pysparse_array.egg-info/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)      311 2023-05-23 14:27:45.000000 pysparse-array-1.0.6/pysparse_array.egg-info/SOURCES.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-23 14:27:45.000000 pysparse-array-1.0.6/pysparse_array.egg-info/dependency_links.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       34 2023-05-23 14:27:45.000000 pysparse-array-1.0.6/pysparse_array.egg-info/requires.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        7 2023-05-23 14:27:45.000000 pysparse-array-1.0.6/pysparse_array.egg-info/top_level.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-05-23 14:27:45.887169 pysparse-array-1.0.6/setup.cfg
--rw-r--r--   0 thomasfrost   (502) staff       (20)      708 2023-05-23 14:23:36.000000 pysparse-array-1.0.6/setup.py
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-23 14:27:45.880024 pysparse-array-1.0.6/sparse/
--rw-r--r--   0 thomasfrost   (502) staff       (20)      113 2023-05-16 11:47:08.000000 pysparse-array-1.0.6/sparse/__init__.py
--rw-r--r--   0 thomasfrost   (502) staff       (20)     8942 2023-05-22 13:07:48.000000 pysparse-array-1.0.6/sparse/array_api.py
--rw-r--r--   0 thomasfrost   (502) staff       (20)     7531 2023-05-23 14:25:40.000000 pysparse-array-1.0.6/sparse/core.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-23 16:53:52.310155 pysparse-array-1.0.7/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     3228 2023-05-23 16:52:28.000000 pysparse-array-1.0.7/HISTORY.md
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-1.0.7/LICENSE.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       19 2023-05-16 11:11:47.000000 pysparse-array-1.0.7/MANIFEST.in
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     5399 2023-05-23 16:53:52.302293 pysparse-array-1.0.7/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     4694 2023-05-20 21:17:03.000000 pysparse-array-1.0.7/README.md
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      763 2023-05-23 16:52:42.000000 pysparse-array-1.0.7/pyproject.toml
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-23 16:53:52.262639 pysparse-array-1.0.7/pysparse_array.egg-info/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     5399 2023-05-23 16:53:52.000000 pysparse-array-1.0.7/pysparse_array.egg-info/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      311 2023-05-23 16:53:52.000000 pysparse-array-1.0.7/pysparse_array.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-23 16:53:52.000000 pysparse-array-1.0.7/pysparse_array.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       34 2023-05-23 16:53:52.000000 pysparse-array-1.0.7/pysparse_array.egg-info/requires.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        7 2023-05-23 16:53:52.000000 pysparse-array-1.0.7/pysparse_array.egg-info/top_level.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-05-23 16:53:52.310404 pysparse-array-1.0.7/setup.cfg
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      708 2023-05-23 16:52:47.000000 pysparse-array-1.0.7/setup.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-23 16:53:52.299824 pysparse-array-1.0.7/sparse/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      113 2023-05-16 11:47:08.000000 pysparse-array-1.0.7/sparse/__init__.py
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     8949 2023-05-23 16:51:47.000000 pysparse-array-1.0.7/sparse/array_api.py
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     7531 2023-05-23 14:25:40.000000 pysparse-array-1.0.7/sparse/core.py
```

### Comparing `pysparse-array-1.0.6/HISTORY.md` & `pysparse-array-1.0.7/HISTORY.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 #Changelog
 
 All notable changes to the `PySparse` package will be documented in this file.
 
 ## [Unreleased]
 
-## [1.0.6] - ?????
+## [1.0.7] - 2023-05-23
+
+### Fixed
+- Fixed ongoing multi-index issues
+
+## [1.0.6] - 2023-05-23
 
 ### Fixed
 - Accidentally left njit commented out!
 
 ### Changed
 - Progress bar fixed to always finish with 100%
 
-## [1.0.5] - 2023-05-20
+## [1.0.5] - 2023-05-22
 
 ### Fixed
 - Fixed single-index bug at axis=0
 
 ## [1.0.4] - 2023-05-22
 
 ### Fixed
```

### Comparing `pysparse-array-1.0.6/LICENSE.txt` & `pysparse-array-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysparse-array-1.0.6/PKG-INFO` & `pysparse-array-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparse-array
-Version: 1.0.6
+Version: 1.0.7
 Summary: A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries.
 Home-page: https://github.com/tdgfrost/PySparse
 Download-URL: https://pypi.org/project/pysparse-array/
 Author: Thomas Frost
 Author-email: Thomas Frost <tdgfrost@gmail.com>
 Project-URL: Homepage, https://github.com/tdgfrost/PySparse
 Project-URL: Bug Tracker, https://github.com/tdgfrost/PySparse/issues
```

### Comparing `pysparse-array-1.0.6/README.md` & `pysparse-array-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pysparse-array-1.0.6/pyproject.toml` & `pysparse-array-1.0.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pysparse-array"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
 	{ name="Thomas Frost", email="tdgfrost@gmail.com" },
 ]
 description = "A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries."
 readme = "README.md"
 requires-python = ">=3.8.0"
 classifiers = [
```

### Comparing `pysparse-array-1.0.6/pysparse_array.egg-info/PKG-INFO` & `pysparse-array-1.0.7/pysparse_array.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparse-array
-Version: 1.0.6
+Version: 1.0.7
 Summary: A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries.
 Home-page: https://github.com/tdgfrost/PySparse
 Download-URL: https://pypi.org/project/pysparse-array/
 Author: Thomas Frost
 Author-email: Thomas Frost <tdgfrost@gmail.com>
 Project-URL: Homepage, https://github.com/tdgfrost/PySparse
 Project-URL: Bug Tracker, https://github.com/tdgfrost/PySparse/issues
```

### Comparing `pysparse-array-1.0.6/setup.py` & `pysparse-array-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='pysparse-array',
-    version='1.0.6',
+    version='1.0.7',
     description='Package to encode and decode large OOM numpy arrays as Sparse binaries',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     packages=find_packages(),
     author='Thomas Frost',
     author_email='tdgfrost@gmail.com',
     url='https://github.com/tdgfrost/PySparse',
```

### Comparing `pysparse-array-1.0.6/sparse/array_api.py` & `pysparse-array-1.0.7/sparse/array_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,19 +121,19 @@
 
         # Assuming the row indices have non-zero data...
         if coords_present:
             # Locate the coordinates of the non-zero data in the original dense array
             target_coords = self.coords[find_coords]
 
             # Some slightly complex indexing to identify the non-zero cells of the (indexed) target array
-            nonzero_row_indices_unique = np.where(np.isin(row_idx, np.unique(target_coords[:, 0])))[0]
-            nonzero_row_indices_unique_idx = np.where(np.isin(np.unique(target_coords[:, 0]), row_idx))[0]
+            nonzero_idxs_in_row_idx = np.where(np.isin(row_idx, np.unique(target_coords[:, 0])))[0]
+            location_of_each_new_idx_in_target_coords = np.unique(target_coords[:, 0], return_index=True)[1]
 
             target_coords[:, 0] = 0
-            target_coords[nonzero_row_indices_unique_idx, 0] = nonzero_row_indices_unique
+            target_coords[location_of_each_new_idx_in_target_coords, 0] = nonzero_idxs_in_row_idx
 
             target_coords[:, 0] = np.maximum.accumulate(target_coords[:, 0], axis=0)
 
             # Re-create the dense array (of the shape requested) with all zeros
             target_data = np.zeros((1,) + self.dense_shape[1:], dtype=self.data_dtype) if isinstance(row_idx, int) else np.zeros(
                 (len(row_idx),) + self.dense_shape[1:], dtype=self.data_dtype)
```

### Comparing `pysparse-array-1.0.6/sparse/core.py` & `pysparse-array-1.0.7/sparse/core.py`

 * *Files identical despite different names*

