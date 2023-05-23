# Comparing `tmp/pysparse-array-1.0.5.tar.gz` & `tmp/pysparse-array-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparse-array-1.0.5.tar", last modified: Mon May 22 13:09:32 2023, max compression
+gzip compressed data, was "pysparse-array-1.0.6.tar", last modified: Tue May 23 14:27:45 2023, max compression
```

## Comparing `pysparse-array-1.0.5.tar` & `pysparse-array-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-22 13:09:32.147642 pysparse-array-1.0.5/
--rw-r--r--   0 thomasfrost   (502) staff       (20)     2968 2023-05-22 13:08:28.000000 pysparse-array-1.0.5/HISTORY.md
--rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-1.0.5/LICENSE.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       19 2023-05-16 11:11:47.000000 pysparse-array-1.0.5/MANIFEST.in
--rw-r--r--   0 thomasfrost   (502) staff       (20)     5399 2023-05-22 13:09:32.145696 pysparse-array-1.0.5/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)     4694 2023-05-20 21:17:03.000000 pysparse-array-1.0.5/README.md
--rw-r--r--   0 thomasfrost   (502) staff       (20)      763 2023-05-22 13:08:37.000000 pysparse-array-1.0.5/pyproject.toml
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-22 13:09:32.091781 pysparse-array-1.0.5/pysparse_array.egg-info/
--rw-r--r--   0 thomasfrost   (502) staff       (20)     5399 2023-05-22 13:09:31.000000 pysparse-array-1.0.5/pysparse_array.egg-info/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)      311 2023-05-22 13:09:31.000000 pysparse-array-1.0.5/pysparse_array.egg-info/SOURCES.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-22 13:09:31.000000 pysparse-array-1.0.5/pysparse_array.egg-info/dependency_links.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       34 2023-05-22 13:09:31.000000 pysparse-array-1.0.5/pysparse_array.egg-info/requires.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        7 2023-05-22 13:09:31.000000 pysparse-array-1.0.5/pysparse_array.egg-info/top_level.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-05-22 13:09:32.147883 pysparse-array-1.0.5/setup.cfg
--rw-r--r--   0 thomasfrost   (502) staff       (20)      708 2023-05-22 13:08:42.000000 pysparse-array-1.0.5/setup.py
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-22 13:09:32.124287 pysparse-array-1.0.5/sparse/
--rw-r--r--   0 thomasfrost   (502) staff       (20)      113 2023-05-16 11:47:08.000000 pysparse-array-1.0.5/sparse/__init__.py
--rw-r--r--   0 thomasfrost   (502) staff       (20)     8942 2023-05-22 13:07:48.000000 pysparse-array-1.0.5/sparse/array_api.py
--rw-r--r--   0 thomasfrost   (502) staff       (20)     7483 2023-05-21 09:30:56.000000 pysparse-array-1.0.5/sparse/core.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-23 14:27:45.886987 pysparse-array-1.0.6/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     3152 2023-05-23 14:26:45.000000 pysparse-array-1.0.6/HISTORY.md
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-1.0.6/LICENSE.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       19 2023-05-16 11:11:47.000000 pysparse-array-1.0.6/MANIFEST.in
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     5399 2023-05-23 14:27:45.882730 pysparse-array-1.0.6/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     4694 2023-05-20 21:17:03.000000 pysparse-array-1.0.6/README.md
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      763 2023-05-23 14:23:31.000000 pysparse-array-1.0.6/pyproject.toml
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-23 14:27:45.791412 pysparse-array-1.0.6/pysparse_array.egg-info/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     5399 2023-05-23 14:27:45.000000 pysparse-array-1.0.6/pysparse_array.egg-info/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      311 2023-05-23 14:27:45.000000 pysparse-array-1.0.6/pysparse_array.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-23 14:27:45.000000 pysparse-array-1.0.6/pysparse_array.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       34 2023-05-23 14:27:45.000000 pysparse-array-1.0.6/pysparse_array.egg-info/requires.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        7 2023-05-23 14:27:45.000000 pysparse-array-1.0.6/pysparse_array.egg-info/top_level.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-05-23 14:27:45.887169 pysparse-array-1.0.6/setup.cfg
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      708 2023-05-23 14:23:36.000000 pysparse-array-1.0.6/setup.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-23 14:27:45.880024 pysparse-array-1.0.6/sparse/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      113 2023-05-16 11:47:08.000000 pysparse-array-1.0.6/sparse/__init__.py
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     8942 2023-05-22 13:07:48.000000 pysparse-array-1.0.6/sparse/array_api.py
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     7531 2023-05-23 14:25:40.000000 pysparse-array-1.0.6/sparse/core.py
```

### Comparing `pysparse-array-1.0.5/HISTORY.md` & `pysparse-array-1.0.6/HISTORY.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 #Changelog
 
 All notable changes to the `PySparse` package will be documented in this file.
 
 ## [Unreleased]
 
-## [1.0.5]
+## [1.0.6] - ?????
+
+### Fixed
+- Accidentally left njit commented out!
+
+### Changed
+- Progress bar fixed to always finish with 100%
+
+## [1.0.5] - 2023-05-20
 
 ### Fixed
 - Fixed single-index bug at axis=0
 
-## [1.0.4]
+## [1.0.4] - 2023-05-22
 
 ### Fixed
 - Fixed multi-indexing bug
 
-## [1.0.3]
+## [1.0.3] - 2023-05-21
 
 ### Fixed
 - Fixed further bug around multi-index slicing, and in doing so, tidied up some unnecessary Class code
 - Fixed bug whereby the first value was being lost when converting to_sparse
 - Fixed bug whereby certain values were being lost in to_sparse due to a dictionary error
 
-## [1.0.2]
+## [1.0.2] - 2023-05-20
 
 ### Added
 - Added .shape attribute alongside .dense_shape and .coords_shape
 
 ### Fixed
 - Fixed bug with indexing 1D data
 - README updated appropriately
```

### Comparing `pysparse-array-1.0.5/LICENSE.txt` & `pysparse-array-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysparse-array-1.0.5/PKG-INFO` & `pysparse-array-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparse-array
-Version: 1.0.5
+Version: 1.0.6
 Summary: A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries.
 Home-page: https://github.com/tdgfrost/PySparse
 Download-URL: https://pypi.org/project/pysparse-array/
 Author: Thomas Frost
 Author-email: Thomas Frost <tdgfrost@gmail.com>
 Project-URL: Homepage, https://github.com/tdgfrost/PySparse
 Project-URL: Bug Tracker, https://github.com/tdgfrost/PySparse/issues
```

### Comparing `pysparse-array-1.0.5/README.md` & `pysparse-array-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pysparse-array-1.0.5/pyproject.toml` & `pysparse-array-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pysparse-array"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
 	{ name="Thomas Frost", email="tdgfrost@gmail.com" },
 ]
 description = "A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries."
 readme = "README.md"
 requires-python = ">=3.8.0"
 classifiers = [
```

### Comparing `pysparse-array-1.0.5/pysparse_array.egg-info/PKG-INFO` & `pysparse-array-1.0.6/pysparse_array.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparse-array
-Version: 1.0.5
+Version: 1.0.6
 Summary: A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries.
 Home-page: https://github.com/tdgfrost/PySparse
 Download-URL: https://pypi.org/project/pysparse-array/
 Author: Thomas Frost
 Author-email: Thomas Frost <tdgfrost@gmail.com>
 Project-URL: Homepage, https://github.com/tdgfrost/PySparse
 Project-URL: Bug Tracker, https://github.com/tdgfrost/PySparse/issues
```

### Comparing `pysparse-array-1.0.5/setup.py` & `pysparse-array-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='pysparse-array',
-    version='1.0.5',
+    version='1.0.6',
     description='Package to encode and decode large OOM numpy arrays as Sparse binaries',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     packages=find_packages(),
     author='Thomas Frost',
     author_email='tdgfrost@gmail.com',
     url='https://github.com/tdgfrost/PySparse',
```

### Comparing `pysparse-array-1.0.5/sparse/array_api.py` & `pysparse-array-1.0.6/sparse/array_api.py`

 * *Files identical despite different names*

### Comparing `pysparse-array-1.0.5/sparse/core.py` & `pysparse-array-1.0.6/sparse/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,21 +54,21 @@
     shape = array.shape
 
     if (chunksize is None) or (type(array) is np.ndarray):
         data_shape = np.count_nonzero(array)
 
     else:
         for i in range(0, shape[0], chunksize):
-            progress_bar(i, shape[0]) if verbose else None
+            progress_bar(i, shape[0] // chunksize * chunksize) if verbose else None
             data_shape += np.count_nonzero(array[i:i + chunksize])
 
     return data_shape
 
 
-#@njit
+@njit
 def __convert_to_sparse_data(sparse_coords, sparse_values, iteration: int, chunksize, sparse_idx) -> (np.ndarray, np.ndarray):
     """
     Convert a chunk of a dense array to sparse data
     :param sparse_coords: sparse coordinates
     :param sparse_values: sparse values
     :param iteration: iteration number
     :param prev_sparse_coords_max: maximum idx of the previous sparse coordinates
@@ -82,15 +82,15 @@
     sparse_coords = sparse_coords_arr.T
     sparse_coords_dict = __create_sparse_coords_dictionary(sparse_coords, iteration, chunksize,
                                                            sparse_idx)
 
     return sparse_coords, sparse_values, sparse_coords_dict
 
 
-#@njit(parallel=True)
+@njit(parallel=True)
 def __create_sparse_coords_dictionary(sparse_coords, iteration, chunksize, sparse_idx):
     """
     Convert a chunk of a dense array to sparse data
     :param sparse_coords: sparse coordinates
     :return: dictionary mapping dense rows to sparse coordinates
     """
     min_value = sparse_coords[:, 0].min()
@@ -147,15 +147,15 @@
 
         memmap_sparse_coords[:] = sparse_coords
         memmap_sparse_data[:] = sparse_values
 
     else:
         sparse_coords_dict = {}
         for chunk_idx in range(0, dense_shape[0], chunksize):
-            progress_bar(chunk_idx, dense_shape[0]) if verbose else None
+            progress_bar(chunk_idx, dense_shape[0] // chunksize * chunksize) if verbose else None
             array_chunk = array[chunk_idx:chunk_idx + chunksize]
             # Use of the bool dtype accelerates this step
             sparse_coords = array_chunk.astype(bool).nonzero()
             sparse_values = array_chunk[sparse_coords]
             sparse_coords, sparse_values, sparse_coords_dict_temp = __convert_to_sparse_data(sparse_coords, sparse_values,
                                                                                              chunk_idx, chunksize,
                                                                                              sparse_index)
```

