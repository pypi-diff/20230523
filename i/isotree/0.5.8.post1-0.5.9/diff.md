# Comparing `tmp/isotree-0.5.8.post1.tar.gz` & `tmp/isotree-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/isotree-0.5.8.post1.tar", last modified: Fri Jan 14 21:58:40 2022, max compression
+gzip compressed data, was "dist/isotree-0.5.9.tar", last modified: Tue Jan 18 03:37:34 2022, max compression
```

## Comparing `isotree-0.5.8.post1.tar` & `isotree-0.5.9.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-01-14 21:58:40.000000 isotree-0.5.8.post1/
--rw-r--r--   0 david     (1000) david     (1000)      374 2021-11-19 21:54:05.000000 isotree-0.5.8.post1/.gitignore
--rw-r--r--   0 david     (1000) david     (1000)     1327 2022-01-03 05:51:31.000000 isotree-0.5.8.post1/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)     1005 2022-01-03 04:23:39.000000 isotree-0.5.8.post1/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)      355 2022-01-14 21:58:40.000000 isotree-0.5.8.post1/PKG-INFO
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-01-14 21:58:40.000000 isotree-0.5.8.post1/isotree/
--rw-r--r--   0 david     (1000) david     (1000)   187819 2022-01-14 21:58:17.000000 isotree-0.5.8.post1/isotree/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)    65258 2022-01-14 20:57:20.000000 isotree-0.5.8.post1/isotree/cpp_interface.pyx
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-01-14 21:58:40.000000 isotree-0.5.8.post1/isotree.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      355 2022-01-14 21:58:40.000000 isotree-0.5.8.post1/isotree.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      808 2022-01-14 21:58:40.000000 isotree-0.5.8.post1/isotree.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2022-01-14 21:58:40.000000 isotree-0.5.8.post1/isotree.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)        8 2022-01-14 21:58:40.000000 isotree-0.5.8.post1/isotree.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)       86 2021-11-19 21:54:05.000000 isotree-0.5.8.post1/pyproject.toml
--rw-r--r--   0 david     (1000) david     (1000)       40 2021-11-19 21:54:05.000000 isotree-0.5.8.post1/requirements.txt
--rw-r--r--   0 david     (1000) david     (1000)       38 2022-01-14 21:58:40.000000 isotree-0.5.8.post1/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)    10468 2022-01-14 21:52:27.000000 isotree-0.5.8.post1/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-01-14 21:58:40.000000 isotree-0.5.8.post1/src/
--rw-r--r--   0 david     (1000) david     (1000)   105524 2022-01-12 20:51:13.000000 isotree-0.5.8.post1/src/crit.hpp
--rw-r--r--   0 david     (1000) david     (1000)    67481 2022-01-13 20:00:59.000000 isotree-0.5.8.post1/src/dist.hpp
--rw-r--r--   0 david     (1000) david     (1000)    64346 2022-01-12 20:48:00.000000 isotree-0.5.8.post1/src/extended.hpp
--rw-r--r--   0 david     (1000) david     (1000)   111623 2022-01-14 21:23:46.000000 isotree-0.5.8.post1/src/fit_model.hpp
--rw-r--r--   0 david     (1000) david     (1000)     3857 2022-01-03 05:51:31.000000 isotree-0.5.8.post1/src/headers_joined.hpp
--rw-r--r--   0 david     (1000) david     (1000)    35365 2022-01-12 20:48:36.000000 isotree-0.5.8.post1/src/helpers_iforest.hpp
--rw-r--r--   0 david     (1000) david     (1000)    55115 2022-01-12 20:48:20.000000 isotree-0.5.8.post1/src/impute.hpp
--rw-r--r--   0 david     (1000) david     (1000)    20578 2022-01-12 00:41:41.000000 isotree-0.5.8.post1/src/indexer.cpp
--rw-r--r--   0 david     (1000) david     (1000)    11228 2022-01-10 23:51:13.000000 isotree-0.5.8.post1/src/instantiate_template_headers.hpp
--rw-r--r--   0 david     (1000) david     (1000)    78530 2022-01-12 20:48:59.000000 isotree-0.5.8.post1/src/isoforest.hpp
--rw-r--r--   0 david     (1000) david     (1000)    98807 2022-01-12 21:14:53.000000 isotree-0.5.8.post1/src/isotree.hpp
--rw-r--r--   0 david     (1000) david     (1000)    12175 2022-01-10 20:43:48.000000 isotree-0.5.8.post1/src/merge_models.cpp
--rw-r--r--   0 david     (1000) david     (1000)    47575 2022-01-12 20:51:39.000000 isotree-0.5.8.post1/src/mult.hpp
--rw-r--r--   0 david     (1000) david     (1000)     9527 2022-01-03 05:51:31.000000 isotree-0.5.8.post1/src/other_helpers.hpp
--rw-r--r--   0 david     (1000) david     (1000)    82459 2022-01-10 22:56:59.000000 isotree-0.5.8.post1/src/predict.hpp
--rw-r--r--   0 david     (1000) david     (1000)     4955 2022-01-10 00:15:23.000000 isotree-0.5.8.post1/src/python_helpers.hpp
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-01-14 21:58:40.000000 isotree-0.5.8.post1/src/robinmap/
--rw-r--r--   0 david     (1000) david     (1000)     1102 2021-07-16 23:59:38.000000 isotree-0.5.8.post1/src/robinmap/LICENSE
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-01-14 21:58:40.000000 isotree-0.5.8.post1/src/robinmap/include/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-01-14 21:58:40.000000 isotree-0.5.8.post1/src/robinmap/include/tsl/
--rw-r--r--   0 david     (1000) david     (1000)    11773 2021-07-16 23:59:38.000000 isotree-0.5.8.post1/src/robinmap/include/tsl/robin_growth_policy.h
--rw-r--r--   0 david     (1000) david     (1000)    53806 2021-07-16 23:59:38.000000 isotree-0.5.8.post1/src/robinmap/include/tsl/robin_hash.h
--rw-r--r--   0 david     (1000) david     (1000)    28412 2021-07-16 23:59:38.000000 isotree-0.5.8.post1/src/robinmap/include/tsl/robin_map.h
--rw-r--r--   0 david     (1000) david     (1000)    23593 2021-07-16 23:59:38.000000 isotree-0.5.8.post1/src/robinmap/include/tsl/robin_set.h
--rw-r--r--   0 david     (1000) david     (1000)   134414 2022-01-12 00:25:15.000000 isotree-0.5.8.post1/src/serialize.cpp
--rw-r--r--   0 david     (1000) david     (1000)    31437 2022-01-12 20:47:38.000000 isotree-0.5.8.post1/src/sql.cpp
--rw-r--r--   0 david     (1000) david     (1000)     9116 2022-01-09 22:15:16.000000 isotree-0.5.8.post1/src/subset_models.cpp
--rw-r--r--   0 david     (1000) david     (1000)   122388 2022-01-12 20:53:33.000000 isotree-0.5.8.post1/src/utils.hpp
--rw-r--r--   0 david     (1000) david     (1000)    14675 2022-01-10 19:17:58.000000 isotree-0.5.8.post1/src/xoshiro.hpp
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-01-18 03:37:34.000000 isotree-0.5.9/
+-rw-r--r--   0 david     (1000) david     (1000)      374 2021-11-19 21:54:05.000000 isotree-0.5.9/.gitignore
+-rw-r--r--   0 david     (1000) david     (1000)     1327 2022-01-03 05:51:31.000000 isotree-0.5.9/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)     1005 2022-01-03 04:23:39.000000 isotree-0.5.9/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)      349 2022-01-18 03:37:34.000000 isotree-0.5.9/PKG-INFO
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-01-18 03:37:34.000000 isotree-0.5.9/isotree/
+-rw-r--r--   0 david     (1000) david     (1000)   199759 2022-01-18 01:43:10.000000 isotree-0.5.9/isotree/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)    75287 2022-01-18 02:41:23.000000 isotree-0.5.9/isotree/cpp_interface.pyx
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-01-18 03:37:34.000000 isotree-0.5.9/isotree.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)      349 2022-01-18 03:37:33.000000 isotree-0.5.9/isotree.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      828 2022-01-18 03:37:34.000000 isotree-0.5.9/isotree.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2022-01-18 03:37:33.000000 isotree-0.5.9/isotree.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)        8 2022-01-18 03:37:33.000000 isotree-0.5.9/isotree.egg-info/top_level.txt
+-rw-r--r--   0 david     (1000) david     (1000)       86 2021-11-19 21:54:05.000000 isotree-0.5.9/pyproject.toml
+-rw-r--r--   0 david     (1000) david     (1000)       40 2021-11-19 21:54:05.000000 isotree-0.5.9/requirements.txt
+-rw-r--r--   0 david     (1000) david     (1000)       38 2022-01-18 03:37:34.000000 isotree-0.5.9/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)    10466 2022-01-18 03:04:38.000000 isotree-0.5.9/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-01-18 03:37:34.000000 isotree-0.5.9/src/
+-rw-r--r--   0 david     (1000) david     (1000)   106408 2022-01-16 19:15:38.000000 isotree-0.5.9/src/crit.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    85169 2022-01-18 03:19:04.000000 isotree-0.5.9/src/dist.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    64578 2022-01-15 21:22:12.000000 isotree-0.5.9/src/extended.hpp
+-rw-r--r--   0 david     (1000) david     (1000)   119198 2022-01-17 23:24:01.000000 isotree-0.5.9/src/fit_model.hpp
+-rw-r--r--   0 david     (1000) david     (1000)     4327 2022-01-17 02:22:39.000000 isotree-0.5.9/src/headers_joined.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    35597 2022-01-15 21:23:05.000000 isotree-0.5.9/src/helpers_iforest.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    55347 2022-01-15 21:23:11.000000 isotree-0.5.9/src/impute.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    18564 2022-01-17 20:46:56.000000 isotree-0.5.9/src/indexer.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    12924 2022-01-17 23:53:52.000000 isotree-0.5.9/src/instantiate_template_headers.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    78762 2022-01-15 21:23:35.000000 isotree-0.5.9/src/isoforest.hpp
+-rw-r--r--   0 david     (1000) david     (1000)   103040 2022-01-18 00:56:15.000000 isotree-0.5.9/src/isotree.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    14025 2022-01-17 17:56:51.000000 isotree-0.5.9/src/merge_models.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    47973 2022-01-16 19:47:04.000000 isotree-0.5.9/src/mult.hpp
+-rw-r--r--   0 david     (1000) david     (1000)     9759 2022-01-15 21:24:40.000000 isotree-0.5.9/src/other_helpers.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    83369 2022-01-17 00:18:00.000000 isotree-0.5.9/src/predict.hpp
+-rw-r--r--   0 david     (1000) david     (1000)     5187 2022-01-15 21:24:51.000000 isotree-0.5.9/src/python_helpers.hpp
+-rw-r--r--   0 david     (1000) david     (1000)     7870 2022-01-17 21:16:08.000000 isotree-0.5.9/src/ref_indexer.hpp
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-01-18 03:37:34.000000 isotree-0.5.9/src/robinmap/
+-rw-r--r--   0 david     (1000) david     (1000)     1102 2021-07-16 23:59:38.000000 isotree-0.5.9/src/robinmap/LICENSE
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-01-18 03:37:34.000000 isotree-0.5.9/src/robinmap/include/
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-01-18 03:37:34.000000 isotree-0.5.9/src/robinmap/include/tsl/
+-rw-r--r--   0 david     (1000) david     (1000)    11773 2021-07-16 23:59:38.000000 isotree-0.5.9/src/robinmap/include/tsl/robin_growth_policy.h
+-rw-r--r--   0 david     (1000) david     (1000)    53806 2021-07-16 23:59:38.000000 isotree-0.5.9/src/robinmap/include/tsl/robin_hash.h
+-rw-r--r--   0 david     (1000) david     (1000)    28412 2021-07-16 23:59:38.000000 isotree-0.5.9/src/robinmap/include/tsl/robin_map.h
+-rw-r--r--   0 david     (1000) david     (1000)    23593 2021-07-16 23:59:38.000000 isotree-0.5.9/src/robinmap/include/tsl/robin_set.h
+-rw-r--r--   0 david     (1000) david     (1000)   135564 2022-01-17 16:49:47.000000 isotree-0.5.9/src/serialize.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    31669 2022-01-15 21:25:09.000000 isotree-0.5.9/src/sql.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     9348 2022-01-15 21:25:14.000000 isotree-0.5.9/src/subset_models.cpp
+-rw-r--r--   0 david     (1000) david     (1000)   122639 2022-01-18 00:56:04.000000 isotree-0.5.9/src/utils.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    15289 2022-01-16 21:12:00.000000 isotree-0.5.9/src/xoshiro.hpp
```

### Comparing `isotree-0.5.8.post1/LICENSE` & `isotree-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `isotree-0.5.8.post1/MANIFEST.in` & `isotree-0.5.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `isotree-0.5.8.post1/isotree/__init__.py` & `isotree-0.5.9/isotree/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -789,14 +789,16 @@
     .. [10] https://math.stackexchange.com/questions/3333220/expected-average-depth-in-random-binary-tree-constructed-top-to-bottom
     .. [11] Cortes, David. "Revisiting randomized choices in isolation forests."
             arXiv preprint arXiv:2110.13402 (2021).
     .. [12] Guha, Sudipto, et al. "Robust random cut forest based anomaly detection on streams."
             International conference on machine learning. PMLR, 2016.
     .. [13] Cortes, David. "Isolation forests: looking beyond tree depth."
             arXiv preprint arXiv:2111.11639 (2021).
+    .. [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou. "Isolation kernel and its effect on SVM."
+            Proceedings of the 24th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining. 2018.
     """
     def __init__(self, sample_size = "auto", ntrees = 500, ndim = 3, ntry = 1,
                  categ_cols = None, max_depth = "auto", ncols_per_tree = None,
                  prob_pick_pooled_gain = 0.0, prob_pick_avg_gain = 0.0,
                  prob_pick_col_by_range = 0.0, prob_pick_col_by_var = 0.0,
                  prob_pick_col_by_kurt = 0.0,
                  min_gain = 0., missing_action = "auto", new_categ_action = "auto",
@@ -1146,18 +1148,21 @@
         if self.is_fitted_:
             msg += "Consisting of %d trees\n" % self._ntrees
             if self._ncols_numeric > 0:
                 msg += "Numeric columns: %d\n" % self._ncols_numeric
             if self._ncols_categ:
                 msg += "Categorical columns: %d\n" % self._ncols_categ
         if self.has_indexer_:
-            if self._cpp_obj.has_indexer_with_distances():
-                msg += "(Has node indexer with distances built-in)\n"
-            else:
-                msg += "(Has node indexer built-in)\n"
+            has_distances = self._cpp_obj.has_indexer_with_distances()
+            has_references = self._cpp_obj.has_reference_points()
+            msg += "(Has node indexer%s%s%s built-in)\n" & (
+                "  with distances" if has_distances else "",
+                " and" if (has_distances and has_references) else "",
+                " with reference points" if has_references else ""
+            )
         return msg
 
     def __repr__(self):
         return self.__str__()
 
     def _get_model_obj(self):
         return self._cpp_obj.get_cpp_obj(self._is_extended_)
@@ -2267,111 +2272,188 @@
         Returns
         -------
         score : array(n_samples,)
             Outlier scores for the rows in 'X' (the higher, the most anomalous).
         """
         return self.predict(X, output="score")
 
-    def predict_distance(self, X, output = "dist", square_mat = False, X_ref = None):
+    def predict_distance(self, X, output = "dist", square_mat = True, X_ref = None, use_reference_points = True):
         """
-        Predict approximate distances between points
+        Predict approximate distances or isolation kernels/proximities between points
 
-        Predict approximate pairwise distances between points or individual distances between
-        two sets of points based on how many
-        splits it takes to separate them. Can output either the average number of paths,
+        Predict approximate pairwise distances between points, or individual distances between
+        two sets of points based on how many splits it takes to separate them, or isolation
+        kernels (a.k.a. proximity matrix) from the model based on the number of trees in which
+        two observations end up in the same terminal node. Can output either the average number
+        of paths/steps it takes to separate two observations,
         or a standardized metric (in the same way as the outlier score) in which values closer
         to zero indicate nearer points, closer to one further away points, and closer to 0.5
-        average distance.
+        average distance, or a kernel/proximity metric, either standardized (values between zero and one)
+        or raw (values ranging from zero to the number of trees in the model).
 
         Note
         ----
         The more threads that are set for the model, the higher the memory requirement will be as each
-        thread will allocate an array with one entry per combination.
+        thread will allocate an array with one entry per combination (with an exception being
+        calculation of distances to reference points, which do not do this).
 
         Note
         ----
         Separation depths are very slow to calculate. By default, it will do it through a procedure
         that counts steps as observations are passed down the trees, which is especially slow and
         not recommended for more than a few thousand observations. If this function is going to be
         called repeatedly and/or it is going to be called for a large number of rows, it's highly
         recommended to build node distance indexes beforehand through ``build_indexer`` with
         option ``with_distances=True``, as then the computation will be done based on terminal node
-        indices instead, which is a much faster procedure.
+        indices instead, which is a much faster procedure. If the calculations are all going to be performed
+        with respect to a fixed set of points, it's highly recommended to set those points as references
+        through ``set_reference_points``.
 
         Note
         ----
         If using ``assume_full_distr=False`` (not recommended to use such option), predictions with
         and without an indexer will differ slightly due to differences in what they count towards
         "additional" observations in the calculation.
 
         Parameters
         ----------
         X : array or array-like (n_samples, n_features)
-            Observations for which to calculate approximate pairwise distances,
-            or first group for distances between sets of points. Can pass
+            Observations for which to calculate approximate pairwise distances or kernels,
+            or first group for distances/kernels between sets of points. Can pass
             a NumPy array, Pandas DataFrame, or SciPy sparse CSC matrix.
-        output : str, one of "dist", "avg_sep"
+        output : str, one of "dist", "avg_sep", "kernel", "kernel_raw"
             Type of output to produce. If passing "dist", will standardize the average separation
             depths. If passing "avg_sep", will output the average separation depth without standardizing it
             (note that lower separation depth means furthest distance).
+            If passing "kernel", will output the fraction of the trees in which two observations end up
+            in the same terminal node. If passing "kernel_raw", will output the number (not fraction) of
+            trees in which two observations end up in the same terminal node.
+
+            Note that for "kernel" and "kernel_raw", having an indexer without reference points will not
+            speed up calculations, and if such calculations are going to be done frequently, it is highly
+            recommended to set reference points in the model object.
         square_mat : bool
-            Whether to produce a full square matrix with the pairwise distances. If passing 'False', will output
+            Whether to produce a full square matrix with the pairwise distances or kernels.
+            If passing 'False', will output
             only the upper triangular part as a 1-d array in which entry (i,j) with 0 <= i < j < n is located at
             position p(i,j) = (i * (n - (i+1)/2) + j - i - 1).
-            Ignored when passing ``X_ref``.
+            
+            Ignored when passing ``X_ref`` or ``use_reference_points=True`` plus having reference points.
         X_ref : array or array-like (n_ref, n_features)
-            Second group of observations. If passing it, will calculate distances between each point in
+            Second group of observations. If passing it, will calculate distances/kernels between each point in
             ``X`` and each point in ``X_ref``. If passing ``None`` (the default), will calculate
-            pairwise distances between the points in ``X``.
+            pairwise distances/kernels between the points in ``X``.
             Must be of the same type as ``X`` (e.g. array, DataFrame, CSC).
 
+            Note that, if ``X_ref`` is passed and the model object has an indexer with reference points
+            added (through ``set_reference_points``), those reference points will be ignored for the
+            calculation.
+        use_reference_points : bool
+            When the model object has an indexer with reference points (which can be added through
+            ``set_reference_points``), whether to calculate the distances/kernels from ``X`` to those reference
+            points instead of the pairwise distances/kernels between points in ``X``.
+
+            This is ignored when passing ``X_ref`` or when the model object does not contain an indexer
+            or the indexer does not contain reference points.
+
         Returns
         -------
         dist : array(n_samples * (n_samples - 1) / 2,) or array(n_samples, n_samples) or array(n_samples, n_ref)
-            Approximate distances or average separation depth between points, according to
-            parameter 'output'. Shape and size depends on parameter ``square_mat``, or ``X_ref`` if passed.
+            Approximate distances or average separation depth or kernels/proximities between points,
+            according to parameter 'output'. Shape and size depends on parameters ``square_mat``,
+            ``use_reference_points``, and whether ``X_ref`` is passed.
         """
         assert self.is_fitted_
-        assert output in ["dist", "avg_sep"]
+        assert output in ["dist", "avg_sep", "kernel", "kernel_raw"]
         nthreads_use = _process_nthreads(self.nthreads)
 
-        if X_ref is None:
-            nobs_group1 = 0
-        else:
+        if X_ref is not None:
             if X.__class__ != X_ref.__class__:
                 raise ValueError("'X' and 'X_ref' must be of the same class.")
             nobs_group1 = X.shape[0]
             if X.__class__.__name__ == "DataFrame":
                 X = X.append(X_ref, ignore_index = True)
             elif issparse(X):
                 X = sp_vstack([X, X_ref])
             else:
                 X = np.vstack([X, X_ref])
+        else:
+            nobs_group1 = 0
+            use_reference_points = bool(use_reference_points)
+            if use_reference_points and self._cpp_obj.has_reference_points():
+                if (not output in ["kernel", "kernel_raw"]) and (not self._cpp_obj.has_indexer_with_distances()):
+                    raise ValueError("Model indexer was built without distances. Cannot calculate distances to reference points.")
+            
 
         can_take_row_major = self._cpp_obj.has_indexer() and self._cpp_obj.has_indexer_with_distances() and not issparse(X)
         X_num, X_cat, nrows = self._process_data_new(X, allow_csr = False, prefer_row_major = can_take_row_major, keep_new_cat_levels = False)
-        if nrows == 1:
+        if nrows == 1 and not (use_reference_points and self._cpp_obj.has_reference_points()):
             raise ValueError("Cannot calculate pairwise distances for only 1 row.")
 
         tmat, dmat, rmat = self._cpp_obj.dist(_get_num_dtype(X_num, None, None), _get_int_dtype(X_num),
                                               X_num, X_cat, self._is_extended_,
                                               ctypes.c_size_t(nrows).value,
                                               ctypes.c_int(nthreads_use).value,
                                               ctypes.c_bool(self.assume_full_distr).value,
-                                              ctypes.c_bool(output == "dist").value,
+                                              ctypes.c_bool(output in ["dist", "kernel"]).value,
                                               ctypes.c_bool(square_mat).value,
-                                              ctypes.c_size_t(nobs_group1).value)
+                                              ctypes.c_size_t(nobs_group1).value,
+                                              ctypes.c_bool(use_reference_points).value,
+                                              ctypes.c_bool(output in ["kernel", "kernel_raw"]).value)
         
-        if X_ref is not None:
+        if (X_ref is not None) or (use_reference_points and rmat.shape[1]):
             return rmat
         elif square_mat:
             return dmat
         else:
             return tmat
 
+    def predict_kernel(self, X, square_mat = True, X_ref = None, use_reference_points = True):
+        """
+        Predict isolation kernel between points
+
+        This is a shorthand for ``predict_distance`` with ``output="kernel"``.
+
+        Parameters
+        ----------
+        X : array or array-like (n_samples, n_features)
+            Observations for which to calculate approximate pairwise kernels/proximities,
+            or first group for kernels between sets of points. Can pass
+            a NumPy array, Pandas DataFrame, or SciPy sparse CSC matrix.
+        square_mat : bool
+            Whether to produce a full square matrix with the pairwise kernels. If passing 'False', will output
+            only the upper triangular part as a 1-d array in which entry (i,j) with 0 <= i < j < n is located at
+            position p(i,j) = (i * (n - (i+1)/2) + j - i - 1).
+            Ignored when passing ``X_ref``.
+        X_ref : array or array-like (n_ref, n_features)
+            Second group of observations. If passing it, will calculate kernels between each point in
+            ``X`` and each point in ``X_ref``. If passing ``None`` (the default), will calculate
+            pairwise kernels between the points in ``X``.
+            Must be of the same type as ``X`` (e.g. array, DataFrame, CSC).
+
+            Note that, if ``X_ref`` is passed and the model object has an indexer with reference points
+            added (through ``set_reference_points``), those reference points will be ignored for the
+            calculation.
+        use_reference_points : bool
+            When the model object has an indexer with reference points (which can be added through
+            ``set_reference_points``), whether to calculate the kernels from ``X`` to those reference
+            points instead of the pairwise kernels between points in ``X``.
+
+            This is ignored when passing ``X_ref`` or when the model object does not contain an indexer
+            or the indexer does not contain reference points.
+
+        Returns
+        -------
+        dist : array(n_samples * (n_samples - 1) / 2,) or array(n_samples, n_samples) or array(n_samples, n_ref)
+            Approximate kernels between points, according to
+            parameter 'output'. Shape and size depends on parameter ``square_mat``,
+            and whether ``X_ref`` is passed.
+        """
+        return self.predict_distance(X, output = "kernel", square_mat = square_mat, X_ref = X_ref, use_reference_points = use_reference_points)
+
     def transform(self, X):
         """
         Impute missing values in the data using isolation forest model
 
         Note
         ----
         In order to use this functionality, the model must have been built with imputation capabilities ('build_imputer' = 'True').
@@ -2463,15 +2545,15 @@
         if (self.sample_size is None) or (self.sample_size == "auto"):
             outp = self.fit_predict(X = X, column_weights = column_weights, output_imputed = True)
             return outp["imputed"]
         else:
             self.fit(X = X, column_weights = column_weights)
             return self.transform(X)
 
-    def partial_fit(self, X, sample_weights = None, column_weights = None):
+    def partial_fit(self, X, sample_weights = None, column_weights = None, X_ref = None):
         """
         Add additional (single) tree to isolation forest model
 
         Adds a single tree fit to the full (non-subsampled) data passed here. Must
         have the same columns as previously-fitted data.
 
         Note
@@ -2499,22 +2581,34 @@
              - Numeric, if their dtype is a subtype of NumPy's 'number' or 'datetime64'.
             
              - Categorical, if their dtype is 'object', 'Categorical', or 'bool'. Note that,
                if `Categorical` dtypes are ordered, the order will be ignored here.
                Categorical columns, if any, may have new categories.
             
             Other dtypes are not supported.
+
+            If passing an array and the array is not in column-major format, will be forcibly converted
+            to column-major, which implies an extra data copy.
         sample_weights : None or array(n_samples,)
             Sample observation weights for each row of 'X', with higher weights indicating
             distribution density (i.e. if the weight is two, it has the same effect of including the same data
             point twice). If not 'None', model must have been built with 'weights_as_sample_prob' = 'False'.
         column_weights : None or array(n_features,)
             Sampling weights for each column in 'X'. Ignored when picking columns by deterministic criterion.
             If passing None, each column will have a uniform weight. If used along with kurtosis weights, the
             effect is multiplicative.
+        X_ref : array or array-like (n_references, n_features)
+            Reference points for distance and/or kernel calculations, if these were previously added to
+            the model object through ``set_reference_points``. Must correspond to the same points that
+            were passed to the call to ``set_reference_points``.
+
+            Might be passed in either row-major (preferred) or column-major order. If sparse, only CSC
+            format is supported.
+
+            This is ignored if the model has no stored reference points.
 
         Returns
         -------
         self : obj
             This object.
         """
         if not self.is_fitted_:
@@ -2523,17 +2617,29 @@
             raise ValueError("Cannot use sampling weights with 'partial_fit'.")
 
         if not self.is_fitted_:
             trees_restore = self.ntrees
             try:
                 self.ntrees = 1
                 self.fit(X = X, sample_weights = sample_weights, column_weights = column_weights)
+                if X_ref is not None:
+                    self.set_reference_points(X_ref)
             finally:
                 self.ntrees = trees_restore
             return self
+
+        if self.is_fitted_:
+            if (X_ref is None) and (self.has_indexer_) and (self._cpp_obj.has_reference_points()):
+                msg  = "Must pass either pass 'X_ref' in order to maintain reference points in indexer,"
+                msg += " or drop reference points through 'drop_reference_points'."
+                raise ValueError(msg)
+            if (X_ref is not None) and (not self.has_indexer_ or not self._cpp_obj.has_reference_points()):
+                warnings.warn("Passed 'X_ref', but model object has no reference points. Will be ignored.")
+                X_ref = None
+
         
         X_num, X_cat, nrows = self._process_data_new(X, allow_csr = False, prefer_row_major = False, keep_new_cat_levels = True)
         if sample_weights is not None:
             sample_weights = np.array(sample_weights).reshape(-1)
             if (X_num is not None) and (X_num.dtype != sample_weights.dtype):
                 sample_weights = sample_weights.astype(X_num.dtype)
             if sample_weights.dtype not in [ctypes.c_double, ctypes.c_float]:
@@ -2582,14 +2688,35 @@
 
         if isinstance(self.random_state, np.random.RandomState):
             seed = self.random_state.randint(np.iinfo(np.int32).max)
         else:
             seed = self.random_seed
         seed += self._ntrees
 
+        if X_ref is None:
+            ref_X_num = None
+            ref_X_cat = None
+        else:
+            ref_X_num, ref_X_cat, ref_nrows = self._process_data_new(X_ref, allow_csr = False, prefer_row_major = True, keep_new_cat_levels = True)
+            expected_ref_nrows = self._cpp_obj.get_n_reference_points()
+            if ref_nrows != expected_ref_nrows:
+                raise ValueError("'X_ref' as %d rows, but previous reference data had %d rows."
+                                 % (ref_nrows, expected_ref_nrows))
+            if ref_X_num is not None:
+                matching_num_dtype = _get_num_dtype(X_num, sample_weights, column_weights)
+                if ref_X_num.data.dtype != matching_num_dtype.dtype:
+                    ref_X_num = ref_X_num.astype(matching_num_dtype.dtype)
+                if issparse(ref_X_num):
+                    matching_int_dtype = _get_int_dtype(X_num)
+                    if ref_X_num.indptr.dtype != matching_int_dtype.dtype:
+                        ref_X_num = ref_X_num.copy()
+                        ref_X_num.indices = ref_X_num.indices.astype(matching_int_dtype.dtype)
+                        ref_X_num.indptr = ref_X_num.indptr.astype(matching_int_dtype.dtype)
+
+
         self._cpp_obj.fit_tree(_get_num_dtype(X_num, sample_weights, column_weights),
                                _get_int_dtype(X_num),
                                X_num, X_cat, ncat, sample_weights, column_weights,
                                ctypes.c_size_t(nrows).value,
                                ctypes.c_size_t(self._ncols_numeric).value,
                                ctypes.c_size_t(self._ncols_categ).value,
                                ctypes.c_size_t(self.ndim_).value,
@@ -2612,14 +2739,16 @@
                                self.categ_split_type_,
                                self.new_categ_action_,
                                ctypes.c_bool(self.build_imputer).value,
                                ctypes.c_size_t(self.min_imp_obs).value,
                                self.depth_imp,
                                self.weigh_imp_rows,
                                ctypes.c_bool(self.all_perm).value,
+                               ref_X_num,
+                               ref_X_cat,
                                ctypes.c_int(seed).value)
         self._ntrees += 1
         return self
 
     def get_num_nodes(self):
         """
         Get number of nodes per tree
@@ -3175,22 +3304,40 @@
         """
         Drops the indexer sub-object from this model object
 
         Drops the indexer sub-object from this model object, if it was constructed.
         The indexer, if constructed, is likely to be a very heavy object which might
         not be needed for all purposes.
 
+        Note that reference points as added through ``set_reference_points`` are
+        associated with the indexer object and will also be dropped if any were added.
+
         Returns
         -------
         self : obj
             This object
         """
         self._cpp_obj.drop_indexer()
         return self
 
+    def drop_reference_points(self):
+        """
+        Drops reference points from this model
+
+        Drops any reference points used for distance and/or kernel calculations
+        from the model object, if any were set through ``set_reference_points``.
+
+        Returns
+        -------
+        self : obj
+            This object
+        """
+        self._cpp_obj.drop_reference_points()
+        return self
+
     def build_indexer(self, with_distances = False):
         """
         Build indexer for faster terminal node predictions and/or distance calculations
 
         Builds an index of terminal nodes for faster prediction of terminal node numbers
         (calling ``predict`` with ``output="tree_num"``).
 
@@ -3213,24 +3360,79 @@
         -------
         self : obj
             This object
         """
         assert self.is_fitted_
         if self.missing_action_ == "divide":
             raise ValueError("Cannot build tree indexer when using missing_action='divide'.")
-        if self.new_categ_action_ == "weighted":
+        if self.new_categ_action_ == "weighted" and self.categ_split_type_ != "single_categ":
             if self._ncols_categ or self.cols_categ_.shape[0]:
                 raise ValueError("Cannot build tree indexer when using new_categ_action='weighted'.")
         self._cpp_obj.build_tree_indices(self._is_extended_, bool(with_distances), _process_nthreads(self.nthreads))
         return self
 
     @property
     def has_indexer_(self):
         return self._cpp_obj.has_indexer()
-    
+
+    @property
+    def has_reference_points_(self):
+        return self._cpp_obj.has_reference_points()
+
+    def set_reference_points(self, X, with_distances=False):
+        """
+        Set reference points to calculate distances or kernels with
+
+        Sets some points as pre-defined landmarks with respect to which distances and/or
+        isolation kernel values will be calculated for arbitrary new points in calls to
+        ``predict_distance`` and/or ``predict_kernel``. If any points have already been set
+        as references in the model object, they will be overwritten with the new points passed here.
+
+        Be aware that adding reference points requires building a tree indexer.
+
+        Parameters
+        ----------
+        X : array or array-like (n_samples, n_features)
+            Observations to set as references for future distance and/or isolation kernel calculations.
+            Can pass a NumPy array, Pandas DataFrame, or SciPy sparse CSC matrix.
+        with_distances : bool
+            Whether to pre-calculate node distances (this is required to calculate distance
+            from arbitrary points to the reference points).
+
+            Note that reference points for distances can only be set when using `assume_full_distr=False`
+            (which is the default).
+
+        Returns
+        -------
+        self : obj
+            This object
+        """
+        assert self.is_fitted_
+        with_distances = bool(with_distances)
+
+        if with_distances and (not self.assume_full_distr):
+            raise ValueError("Cannot set reference points for distance when using 'assume_full_distr=False'.")
+
+        if self.missing_action_ == "divide":
+            raise ValueError("Cannot set reference points when using missing_action='divide'.")
+        if self.new_categ_action_ == "weighted" and self.categ_split_type_ != "single_categ":
+            if self._ncols_categ or self.cols_categ_.shape[0]:
+                raise ValueError("Cannot set reference points when using new_categ_action='weighted'.")
+
+        nthreads_use = _process_nthreads(self.nthreads)
+        X_num, X_cat, nrows = self._process_data_new(X, prefer_row_major = True, keep_new_cat_levels = True, allow_csr = False)
+        self._cpp_obj.set_reference_points(
+                            _get_num_dtype(X_num, None, None), _get_int_dtype(X_num),
+                            X_num, X_cat, self._is_extended_,
+                            ctypes.c_size_t(nrows).value,
+                            ctypes.c_int(nthreads_use).value,
+                            ctypes.c_bool(with_distances).value
+                    )
+        return self
+
 
     def subset_trees(self, trees_take):
         """
         Subset trees of a given model
 
         Creates a new model containing only selected trees of this
         model object.
@@ -3247,15 +3449,15 @@
             A new IsolationForest model object, containing only the subset of trees
             from this object that was specified under 'trees_take'.
         """
         assert self.is_fitted_
         trees_take = np.array(trees_take).reshape(-1).astype(ctypes.c_size_t)
         if not trees_take.shape[0]:
             raise ValueError("'trees_take' is empty.")
-        if trees_take.max() >= self.ntrees:
+        if trees_take.max() >= self._ntrees:
             raise ValueError("Attempting to take tree indices that the model does not have.")
         new_cpp_obj = self._cpp_obj.subset_model(trees_take, self._is_extended_, self.build_imputer)
         old_cpp_obj = self._cpp_obj
         try:
             self._cpp_obj = None
             new_obj = deepcopy(self)
             new_obj._cpp_obj = new_cpp_obj
```

### Comparing `isotree-0.5.8.post1/isotree/cpp_interface.pyx` & `isotree-0.5.9/isotree/cpp_interface.pyx`

 * *Files 9% similar despite different names*

```diff
@@ -22,24 +22,28 @@
 #     [7] Quinlan, J. Ross. C4. 5: programs for machine learning. Elsevier, 2014.
 #     [8] Cortes, David.
 #         "Distance approximation using Isolation Forests."
 #         arXiv preprint arXiv:1910.12362 (2019).
 #     [9] Cortes, David.
 #         "Imputing missing values with unsupervised random trees."
 #         arXiv preprint arXiv:1911.06646 (2019).
-#     [10] https://math.stackexchange.com/questions/3333220/expected-average-depth-in-random-binary-tree-constructed-top-to-bottom
+#     [10] https://math.stackexchange.com/questions/3333220/expected-average-depth-in-random-binary-tree-constructed-top-to-bottomF
 #     [11] Cortes, David.
 #          "Revisiting randomized choices in isolation forests."
 #          arXiv preprint arXiv:2110.13402 (2021).
 #     [12] Guha, Sudipto, et al.
 #          "Robust random cut forest based anomaly detection on streams."
 #          International conference on machine learning. PMLR, 2016.
 #     [13] Cortes, David.
 #          "Isolation forests: looking beyond tree depth."
 #          arXiv preprint arXiv:2111.11639 (2021).
+#     [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou.
+#          "Isolation kernel and its effect on SVM"
+#          Proceedings of the 24th ACM SIGKDD
+#          International Conference on Knowledge Discovery & Data Mining. 2018.
 # 
 #     BSD 2-Clause License
 #     Copyright (c) 2019-2022, David Cortes
 #     All rights reserved.
 #     Redistribution and use in source and binary forms, with or without
 #     modification, are permitted provided that the following conditions are met:
 #     * Redistributions of source code must retain the above copyright notice, this
@@ -203,15 +207,15 @@
         vector[size_t] reference_mapping
         size_t n_terminal
 
     ctypedef struct TreesIndexer:
         vector[SingleTreeIndex] indices
 
 
-    void tmat_to_dense(double *tmat, double *dmat, size_t n, bool_t diag_to_one, bool_t diag_to_inf)
+    void tmat_to_dense(double *tmat, double *dmat, size_t n, double fill_diag)
 
     void merge_models(IsoForest*     model,      IsoForest*     other,
                       ExtIsoForest*  ext_model,  ExtIsoForest*  ext_other,
                       Imputer*       imputer,    Imputer*       iother,
                       TreesIndexer*  indexer,    TreesIndexer*  ind_other) nogil except +
 
     void subset_model(IsoForest*     model,      IsoForest*     model_new,
@@ -339,17 +343,18 @@
     void get_num_nodes[sparse_ix_](IsoForest &model_outputs, sparse_ix_ *n_nodes, sparse_ix_ *n_terminal, int nthreads) except +
 
     void get_num_nodes[sparse_ix_](ExtIsoForest &model_outputs, sparse_ix_ *n_nodes, sparse_ix_ *n_terminal, int nthreads) except +
 
     void calc_similarity[real_t_, sparse_ix_](
                          real_t_ numeric_data[], int categ_data[],
                          real_t_ Xc[], sparse_ix_ Xc_ind[], sparse_ix_ Xc_indptr[],
-                         size_t nrows, int nthreads, bool_t assume_full_distr, bool_t standardize_dist,
+                         size_t nrows, int nthreads,
+                         bool_t assume_full_distr, bool_t standardize_dist, bool_t as_kernel,
                          IsoForest *model_outputs, ExtIsoForest *model_outputs_ext,
-                         double tmat[], double rmat[], size_t n_from,
+                         double tmat[], double rmat[], size_t n_from, bool_t use_indexed_references,
                          TreesIndexer *indexer, bool_t is_col_major, size_t ld_numeric, size_t ld_categ) nogil except +
 
     void impute_missing_values[real_t_, sparse_ix_](
                                real_t_ *numeric_data, int *categ_data, bool_t is_col_major,
                                real_t_ *Xr, sparse_ix_ *Xr_ind, sparse_ix_ *Xr_indptr,
                                size_t nrows, int nthreads,
                                IsoForest *model_outputs, ExtIsoForest *model_outputs_ext,
@@ -370,16 +375,28 @@
                  double prob_pick_col_by_range, double prob_pick_col_by_var,
                  double prob_pick_col_by_kurt,
                  double min_gain, MissingAction missing_action,
                  CategSplit cat_split_type, NewCategAction new_cat_action,
                  UseDepthImp depth_imp, WeighImpRows weigh_imp_rows,
                  bool_t  all_perm, Imputer *imputer, size_t min_imp_obs,
                  TreesIndexer *indexer,
+                 real_t_ ref_numeric_data[], int ref_categ_data[],
+                 bool_t ref_is_col_major, size_t ref_ld_numeric, size_t ref_ld_categ,
+                 real_t_ ref_Xc[], sparse_ix_ ref_Xc_ind[], sparse_ix_ ref_Xc_indptr[],
                  uint64_t random_seed) nogil except +
 
+    void set_reference_points[real_t_, sparse_ix_](
+                              IsoForest *model_outputs, ExtIsoForest *model_outputs_ext, TreesIndexer *indexer,
+                              const bool_t with_distances,
+                              real_t_ *numeric_data, int *categ_data,
+                              bool_t is_col_major, size_t ld_numeric, size_t ld_categ,
+                              real_t_ *Xc, sparse_ix_ *Xc_ind, sparse_ix_ *Xc_indptr,
+                              real_t_ *Xr, sparse_ix_ *Xr_ind, sparse_ix_ *Xr_indptr,
+                              size_t nrows, int nthreads) nogil except +
+
     void build_tree_indices(TreesIndexer &indexer, const IsoForest &model, int nthreads, const bool_t with_distances) nogil except +
 
     void build_tree_indices(TreesIndexer &indexer, const ExtIsoForest &model, int nthreads, const bool_t with_distances) nogil except +
 
 
 cdef extern from "python_helpers.hpp":
     model_t deepcopy_obj[model_t](model_t obj) except +
@@ -642,14 +659,24 @@
         dealloc_Imputer(self.imputer)
         self.imputer = get_Imputer()
 
     def drop_indexer(self):
         dealloc_Indexer(self.indexer)
         self.indexer = get_Indexer()
 
+    def drop_reference_points(self):
+        cdef size_t tree, ntrees
+        ntrees = self.indexer.indices.size()
+        if (ntrees > 0) and (self.indexer.indices.front().reference_points.empty()):
+            return None
+        for tree in range(ntrees):
+            self.indexer.indices[tree].reference_points.clear()
+            self.indexer.indices[tree].reference_indptr.clear()
+            self.indexer.indices[tree].reference_mapping.clear()
+
     def get_cpp_obj(self, is_extended):
         if is_extended:
             return self.ext_isoforest
         else:
             return self.isoforest
 
     def get_imputer(self):
@@ -783,15 +810,15 @@
         cdef double*  dmat_ptr    =  NULL
         cdef double*  depths_ptr  =  NULL
 
         if calc_dist:
             tmat      =  np.zeros(int((nrows * (nrows - <size_t>1)) / <size_t>2), dtype = ctypes.c_double)
             tmat_ptr  =  &tmat[0]
             if sq_dist:
-                dmat      =  np.zeros((nrows, nrows), dtype = ctypes.c_double, order = 'F')
+                dmat      =  np.zeros((nrows, nrows), dtype = ctypes.c_double)
                 dmat_ptr  =  &dmat[0, 0]
         if calc_depth:
             depths      =  np.zeros(nrows, dtype = ctypes.c_double)
             depths_ptr  =  &depths[0]
 
         cdef IsoForest*     model_ptr      =  NULL
         cdef ExtIsoForest*  ext_model_ptr  =  NULL
@@ -841,15 +868,15 @@
             cy_tick_off_interrupt_switch()
             raise InterruptedError("Error: procedure was interrupted.")
 
         if ret_val == return_EXIT_FAILURE():
             raise ValueError("Error: something went wrong. Procedure failed.")
 
         if (calc_dist) and (sq_dist):
-            tmat_to_dense(tmat_ptr, dmat_ptr, nrows, <bool_t>0, <bool_t>(not standardize_dist))
+            tmat_to_dense(tmat_ptr, dmat_ptr, nrows, 0. if standardize_dist else np.inf)
 
         return depths, tmat, dmat, X_num, X_cat
 
     def fit_tree(self,
                  np.ndarray[real_t, ndim=1] placeholder_real_t,
                  np.ndarray[sparse_ix, ndim=1] placeholder_sparse_ix,
                  X_num, X_cat, ncat, sample_weights, col_weights,
@@ -860,15 +887,17 @@
                  bool_t fast_bratio, bool_t weigh_by_kurt,
                  double prob_pick_by_gain_pl, double prob_pick_by_gain_avg,
                  double prob_pick_col_by_range, double prob_pick_col_by_var,
                  double prob_pick_col_by_kurt,
                  double min_gain, missing_action, cat_split_type, new_cat_action,
                  bool_t build_imputer, size_t min_imp_obs,
                  depth_imp, weigh_imp_rows,
-                 bool_t all_perm, uint64_t random_seed):
+                 bool_t all_perm,
+                 ref_X_num, ref_X_cat,
+                 uint64_t random_seed):
         cdef real_t*     numeric_data_ptr    =  NULL
         cdef int*        categ_data_ptr      =  NULL
         cdef int*        ncat_ptr            =  NULL
         cdef real_t*     Xc_ptr              =  NULL
         cdef sparse_ix*  Xc_ind_ptr          =  NULL
         cdef sparse_ix*  Xc_indptr_ptr       =  NULL
         cdef real_t*     sample_weights_ptr  =  NULL
@@ -918,14 +947,59 @@
             if real_t is float:
                 col_weights_ptr     =  get_ptr_float_vec(col_weights)
             else:
                 if col_weights.dtype != ctypes.c_double:
                     col_weights = col_weights.astype(ctypes.c_double)
                 col_weights_ptr =  get_ptr_dbl_vec(col_weights)
 
+
+        cdef real_t*     ref_numeric_data_ptr    =  NULL
+        cdef int*        ref_categ_data_ptr      =  NULL
+        cdef real_t*     ref_Xc_ptr              =  NULL
+        cdef sparse_ix*  ref_Xc_ind_ptr          =  NULL
+        cdef sparse_ix*  ref_Xc_indptr_ptr       =  NULL
+        cdef bool_t      ref_is_col_major    =  True
+        cdef size_t      ref_ncols_numeric   =  0
+        cdef size_t      ref_ncols_categ     =  0
+
+        if ref_X_num is not None:
+            if not issparse(ref_X_num):
+                if real_t is float:
+                    ref_numeric_data_ptr  =  get_ptr_float_mat(ref_X_num)
+                else:
+                    if ref_X_num.dtype != ctypes.c_double:
+                        ref_X_num = ref_X_num.astype(ctypes.c_double)
+                    ref_numeric_data_ptr  =  get_ptr_dbl_mat(ref_X_num)
+                ref_ncols_numeric      =  ref_X_num.shape[1]
+                ref_is_col_major       =  np.isfortran(ref_X_num)
+            else:
+                if real_t is float:
+                    ref_Xc_ptr         =  get_ptr_float_vec(ref_X_num.data)
+                else:
+                    if ref_X_num.data.dtype != ctypes.c_double:
+                        ref_X_num.data = ref_X_num.data.astype(ctypes.c_double)
+                    ref_Xc_ptr         =  get_ptr_dbl_vec(ref_X_num.data)
+                if sparse_ix is int:
+                    ref_Xc_ind_ptr     =  get_ptr_int_vec(ref_X_num.indices)
+                    ref_Xc_indptr_ptr  =  get_ptr_int_vec(ref_X_num.indptr)
+                elif sparse_ix is np.int64_t:
+                    ref_Xc_ind_ptr     =  get_ptr_int64_vec(ref_X_num.indices)
+                    ref_Xc_indptr_ptr  =  get_ptr_int64_vec(ref_X_num.indptr)
+                else:
+                    if ref_X_num.indices.dtype != ctypes.c_size_t:
+                        ref_X_num.indices = ref_X_num.indices.astype(ctypes.c_size_t)
+                    if ref_X_num.indptr.dtype != ctypes.c_size_t:
+                        ref_X_num.indptr = ref_X_num.indptr.astype(ctypes.c_size_t)
+                    ref_Xc_ind_ptr     =  get_ptr_szt_vec(ref_X_num.indices)
+                    ref_Xc_indptr_ptr  =  get_ptr_szt_vec(ref_X_num.indptr)
+        if ref_X_cat is not None:
+            ref_categ_data_ptr     =  get_ptr_int_mat(ref_X_cat)
+            ref_ncols_categ        =  ref_X_cat.shape[1]
+            ref_is_col_major       =  np.isfortran(ref_X_cat)
+
         cdef CoefType        coef_type_C       =  Normal
         cdef CategSplit      cat_split_type_C  =  SubSet
         cdef NewCategAction  new_cat_action_C  =  Weighted
         cdef MissingAction   missing_action_C  =  Divide
         cdef UseDepthImp     depth_imp_C       =  Same
         cdef WeighImpRows    weigh_imp_rows_C  =  Flat
         
@@ -979,15 +1053,19 @@
                      prob_pick_by_gain_pl, prob_pick_by_gain_avg,
                      prob_pick_col_by_range, prob_pick_col_by_var,
                      prob_pick_col_by_kurt,
                      min_gain, missing_action_C,
                      cat_split_type_C, new_cat_action_C,
                      depth_imp_C, weigh_imp_rows_C,
                      all_perm, imputer_ptr, min_imp_obs,
-                     indexer_ptr, random_seed)
+                     indexer_ptr,
+                     ref_numeric_data_ptr, ref_categ_data_ptr,
+                     ref_is_col_major, ref_ncols_numeric, ref_ncols_categ,
+                     ref_Xc_ptr, ref_Xc_ind_ptr, ref_Xc_indptr_ptr,
+                     random_seed)
 
     def predict(self,
                 np.ndarray[real_t, ndim=1] placeholder_real_t,
                 np.ndarray[sparse_ix, ndim=1] placeholder_sparse_ix,
                 X_num, X_cat, is_extended,
                 size_t nrows, int nthreads, bool_t standardize,
                 bool_t output_tree_num, bool_t output_per_tree_depths):
@@ -1116,28 +1194,42 @@
 
     def dist(self,
              np.ndarray[real_t, ndim=1] placeholder_real_t,
              np.ndarray[sparse_ix, ndim=1] placeholder_sparse_ix,
              X_num, X_cat, is_extended,
              size_t nrows, int nthreads, bool_t assume_full_distr,
              bool_t standardize_dist,    bool_t sq_dist,
-             size_t n_from):
+             size_t n_from, bool_t use_reference_points,
+             bool_t as_kernel):
 
         cdef real_t*     numeric_data_ptr  =  NULL
         cdef int*        categ_data_ptr    =  NULL
         cdef real_t*     Xc_ptr            =  NULL
         cdef sparse_ix*  Xc_ind_ptr        =  NULL
         cdef sparse_ix*  Xc_indptr_ptr     =  NULL
 
         cdef bool_t is_col_major    =  True
         cdef size_t ncols_numeric   =  0
         cdef size_t ncols_categ     =  0
 
+        cdef bool_t avoid_row_major = (
+            as_kernel and
+            (not use_reference_points or
+             self.indexer.indices.empty() or
+             self.indexer.indices.front().reference_points.empty())
+        )
+
         if X_num is not None:
             if not issparse(X_num):
+                if avoid_row_major and not np.isfortran(X_num):
+                    if real_t is float:
+                        X_num = np.asfortranarray(X_num, dtype=ctypes.c_float)
+                    else:
+                        X_num = np.asfortranarray(X_num, dtype=ctypes.c_double)
+
                 if real_t is float:
                     numeric_data_ptr  =  get_ptr_float_mat(X_num)
                 else:
                     if X_num.dtype != ctypes.c_double:
                         X_num = X_num.astype(ctypes.c_double)
                     numeric_data_ptr  =  get_ptr_dbl_mat(X_num)
                 ncols_numeric  =  X_num.shape[1]
@@ -1163,34 +1255,45 @@
                         if X_num.indices.dtype != ctypes.c_size_t:
                             X_num.indices = X_num.indices.astype(ctypes.c_size_t)
                         Xc_ind_ptr     =  get_ptr_szt_vec(X_num.indices)
                     if X_num.indptr.dtype != ctypes.c_size_t:
                         X_num.indptr = X_num.indptr.astype(ctypes.c_size_t)
                     Xc_indptr_ptr  =  get_ptr_szt_vec(X_num.indptr)
         if X_cat is not None:
+            if avoid_row_major and not np.isfortran(X_cat):
+                X_cat = np.asfortranarray(X_cat, dtype=ctypes.c_int)
+
             categ_data_ptr     =  get_ptr_int_mat(X_cat)
             ncols_categ        =  X_cat.shape[1]
             is_col_major       =  np.isfortran(X_cat)
 
         cdef np.ndarray[double, ndim = 1]  tmat    =  np.empty(0, dtype = ctypes.c_double)
         cdef np.ndarray[double, ndim = 2]  dmat    =  np.empty((0, 0), dtype = ctypes.c_double)
         cdef np.ndarray[double, ndim = 2]  rmat    =  np.empty((0, 0), dtype = ctypes.c_double)
         cdef double*  tmat_ptr    =  NULL
         cdef double*  dmat_ptr    =  NULL
         cdef double*  rmat_ptr    =  NULL
 
-        if n_from == 0:
+        if n_from != 0:
+            rmat = np.zeros((n_from, nrows - n_from), dtype = ctypes.c_double)
+            rmat_ptr = &rmat[0, 0]
+        elif (
+              use_reference_points and
+              not self.indexer.indices.empty() and
+              not self.indexer.indices.front().reference_points.empty() and
+              (as_kernel or not self.indexer.indices.front().node_distances.empty())
+        ):
+            rmat = np.zeros((nrows, self.indexer.indices.front().reference_points.size()), dtype = ctypes.c_double)
+            rmat_ptr = &rmat[0, 0]
+        else:
             tmat      =  np.zeros(int((nrows * (nrows - 1)) / 2), dtype = ctypes.c_double)
             tmat_ptr  =  &tmat[0]
             if sq_dist:
-                dmat      =  np.zeros((nrows, nrows), dtype = ctypes.c_double, order = 'F')
+                dmat      =  np.zeros((nrows, nrows), dtype = ctypes.c_double)
                 dmat_ptr  =  &dmat[0, 0]
-        else:
-            rmat = np.zeros((n_from, nrows - n_from), dtype = ctypes.c_double)
-            rmat_ptr = &rmat[0, 0]
 
         cdef IsoForest*     model_ptr      =  NULL
         cdef ExtIsoForest*  ext_model_ptr  =  NULL
         if not is_extended:
             model_ptr      =  &self.isoforest
         else:
             ext_model_ptr  =  &self.ext_isoforest
@@ -1198,25 +1301,38 @@
         cdef TreesIndexer*  indexer_ptr = NULL
         if not self.indexer.indices.empty():
             indexer_ptr = &self.indexer
         
         with nogil, boundscheck(False), nonecheck(False), wraparound(False):
             calc_similarity(numeric_data_ptr, categ_data_ptr,
                             Xc_ptr, Xc_ind_ptr, Xc_indptr_ptr,
-                            nrows, nthreads, assume_full_distr, standardize_dist,
+                            nrows, nthreads,
+                            assume_full_distr, standardize_dist, as_kernel,
                             model_ptr, ext_model_ptr,
-                            tmat_ptr, rmat_ptr, n_from,
+                            tmat_ptr, rmat_ptr, n_from, use_reference_points,
                             indexer_ptr, is_col_major, ncols_numeric, ncols_categ)
 
         if cy_check_interrupt_switch():
             cy_tick_off_interrupt_switch()
             raise InterruptedError("Error: procedure was interrupted.")
 
-        if (sq_dist) and (n_from == 0):
-            tmat_to_dense(tmat_ptr, dmat_ptr, nrows, <bool_t>0, <bool_t>(not standardize_dist))
+        cdef double diag_filler
+
+        if (sq_dist) and (n_from == 0) and (not rmat.shape[1]):
+            if as_kernel:
+                if standardize_dist:
+                    diag_filler = 1
+                else:
+                    diag_filler = max(self.isoforest.trees.size(), self.ext_isoforest.hplanes.size())
+            else:
+                if standardize_dist:
+                    diag_filler = 0
+                else:
+                    diag_filler = np.inf
+            tmat_to_dense(tmat_ptr, dmat_ptr, nrows, diag_filler)
 
         return tmat, dmat, rmat
 
     def impute(self,
                np.ndarray[real_t, ndim=1] placeholder_real_t,
                np.ndarray[sparse_ix, ndim=1] placeholder_sparse_ix,
                X_num, X_cat, bool_t is_extended, size_t nrows, int nthreads):
@@ -1501,7 +1617,98 @@
     def has_indexer(self):
         return not self.indexer.indices.empty()
 
     def has_indexer_with_distances(self):
         if not self.has_indexer():
             return False
         return not self.indexer.indices.front().node_distances.empty()
+
+    def set_reference_points(self,
+                             np.ndarray[real_t, ndim=1] placeholder_real_t,
+                             np.ndarray[sparse_ix, ndim=1] placeholder_sparse_ix,
+                             X_num, X_cat, is_extended,
+                             size_t nrows, int nthreads, bool_t with_distances):
+
+        cdef real_t*     numeric_data_ptr  =  NULL
+        cdef int*        categ_data_ptr    =  NULL
+        cdef real_t*     Xc_ptr            =  NULL
+        cdef sparse_ix*  Xc_ind_ptr        =  NULL
+        cdef sparse_ix*  Xc_indptr_ptr     =  NULL
+
+        cdef bool_t is_col_major    =  True
+        cdef size_t ncols_numeric   =  0
+        cdef size_t ncols_categ     =  0
+
+        if X_num is not None:
+            if not issparse(X_num):
+                if real_t is float:
+                    numeric_data_ptr  =  get_ptr_float_mat(X_num)
+                else:
+                    if X_num.dtype != ctypes.c_double:
+                        X_num = X_num.astype(ctypes.c_double)
+                    numeric_data_ptr  =  get_ptr_dbl_mat(X_num)
+                ncols_numeric  =  X_num.shape[1]
+                is_col_major   =  np.isfortran(X_num)
+            else:
+                if X_num.data.shape[0]:
+                    if real_t is float:
+                        Xc_ptr         =  get_ptr_float_vec(X_num.data)
+                    else:
+                        if X_num.data.dtype != ctypes.c_double:
+                            X_num.data = X_num.data.astype(ctypes.c_double)
+                        Xc_ptr         =  get_ptr_dbl_vec(X_num.data)
+                if sparse_ix is int:
+                    if X_num.indices.shape[0]:
+                        Xc_ind_ptr =  get_ptr_int_vec(X_num.indices)
+                    Xc_indptr_ptr  =  get_ptr_int_vec(X_num.indptr)
+                elif sparse_ix is np.int64_t:
+                    if X_num.indices.shape[0]:
+                        Xc_ind_ptr =  get_ptr_int64_vec(X_num.indices)
+                    Xc_indptr_ptr  =  get_ptr_int64_vec(X_num.indptr)
+                else:
+                    if X_num.indices.shape[0]:
+                        if X_num.indices.dtype != ctypes.c_size_t:
+                            X_num.indices = X_num.indices.astype(ctypes.c_size_t)
+                        Xc_ind_ptr     =  get_ptr_szt_vec(X_num.indices)
+                    if X_num.indptr.dtype != ctypes.c_size_t:
+                        X_num.indptr = X_num.indptr.astype(ctypes.c_size_t)
+                    Xc_indptr_ptr  =  get_ptr_szt_vec(X_num.indptr)
+        if X_cat is not None:
+            categ_data_ptr     =  get_ptr_int_mat(X_cat)
+            ncols_categ        =  X_cat.shape[1]
+            is_col_major       =  np.isfortran(X_cat)
+
+
+        cdef IsoForest*     model_ptr      =  NULL
+        cdef ExtIsoForest*  ext_model_ptr  =  NULL
+        if not is_extended:
+            model_ptr      =  &self.isoforest
+        else:
+            ext_model_ptr  =  &self.ext_isoforest
+        cdef TreesIndexer*  indexer_ptr = &self.indexer
+
+        with nogil, boundscheck(False), nonecheck(False), wraparound(False):
+            set_reference_points(model_ptr, ext_model_ptr, indexer_ptr,
+                                 with_distances,
+                                 numeric_data_ptr, categ_data_ptr,
+                                 is_col_major, ncols_numeric, ncols_categ,
+                                 Xc_ptr, Xc_ind_ptr, Xc_indptr_ptr,
+                                 <real_t*>NULL, <sparse_ix*>NULL, <sparse_ix*>NULL,
+                                 nrows, nthreads)
+
+        if cy_check_interrupt_switch():
+            cy_tick_off_interrupt_switch()
+            raise InterruptedError("Error: procedure was interrupted.")
+
+    def has_reference_points(self):
+        if self.indexer.indices.empty():
+            return False
+        if self.indexer.indices.front().reference_points.empty():
+            return False
+        else:
+            return True
+
+    def get_n_reference_points(self):
+        if self.indexer.indices.empty():
+            return 0
+        return self.indexer.indices.front().reference_points.size()
+
```

### Comparing `isotree-0.5.8.post1/isotree.egg-info/SOURCES.txt` & `isotree-0.5.9/isotree.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 src/isoforest.hpp
 src/isotree.hpp
 src/merge_models.cpp
 src/mult.hpp
 src/other_helpers.hpp
 src/predict.hpp
 src/python_helpers.hpp
+src/ref_indexer.hpp
 src/serialize.cpp
 src/sql.cpp
 src/subset_models.cpp
 src/utils.hpp
 src/xoshiro.hpp
 src/robinmap/LICENSE
 src/robinmap/include/tsl/robin_growth_policy.h
```

### Comparing `isotree-0.5.8.post1/setup.py` & `isotree-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
             for e in self.extensions:
                 e.define_macros += [("SUPPORTS_RESTRICT", "1")]
 
 
 setup(
     name  = "isotree",
     packages = ["isotree"],
-    version = '0.5.8-1',
+    version = '0.5.9',
     description = 'Isolation-Based Outlier Detection, Distance, and NA imputation',
     author = 'David Cortes',
     author_email = 'david.cortes.rivera@gmail.com',
     url = 'https://github.com/david-cortes/isotree',
     keywords = ['isolation-forest', 'anomaly', 'outlier'],
     cmdclass = {'build_ext': build_ext_subclass},
     ext_modules = [Extension(
```

### Comparing `isotree-0.5.8.post1/src/crit.hpp` & `isotree-0.5.9/src/crit.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 *          arXiv preprint arXiv:2110.13402 (2021).
 *     [12] Guha, Sudipto, et al.
 *          "Robust random cut forest based anomaly detection on streams."
 *          International conference on machine learning. PMLR, 2016.
 *     [13] Cortes, David.
 *          "Isolation forests: looking beyond tree depth."
 *          arXiv preprint arXiv:2111.11639 (2021).
+*     [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou.
+*          "Isolation kernel and its effect on SVM"
+*          Proceedings of the 24th ACM SIGKDD
+*          International Conference on Knowledge Discovery & Data Mining. 2018.
 * 
 *     BSD 2-Clause License
 *     Copyright (c) 2019-2022, David Cortes
 *     All rights reserved.
 *     Redistribution and use in source and binary forms, with or without
 *     modification, are permitted provided that the following conditions are met:
 *     * Redistributions of source code must retain the above copyright notice, this
@@ -95,30 +99,30 @@
 
             m   +=  delta_div;
             M4  +=  diff * delta_s * (n * n - 3 * n + 3) + 6 * delta_s * M2 - 4 * delta_div * M3;
             M3  +=  diff * delta_div * (n - 2) - 3 * delta_div * M2;
             M2  +=  diff;
         }
 
-        if (!is_na_or_inf(M2) && M2 <= 0)
+        if (unlikely(!is_na_or_inf(M2) && M2 <= 0))
         {
             if (!check_more_than_two_unique_values(ix_arr, st, end, x, missing_action))
                 return -HUGE_VAL;
         }
 
         out = ( M4 / M2 ) * ( (ldouble_safe)(end - st + 1) / M2 );
         return (!is_na_or_inf(out))? std::fmax((double)out, 0.) : (-HUGE_VAL);
     }
 
     else
     {
         size_t cnt = 0;
         for (size_t row = st; row <= end; row++)
         {
-            if (!is_na_or_inf(x[ix_arr[row]]))
+            if (likely(!is_na_or_inf(x[ix_arr[row]])))
             {
                 cnt++;
                 n = (ldouble_safe) cnt;
 
                 delta      =  x[ix_arr[row]] - m;
                 delta_div  =  delta / n;
                 delta_s    =  delta_div * delta_div;
@@ -127,16 +131,16 @@
                 m   +=  delta_div;
                 M4  +=  diff * delta_s * (n * n - 3 * n + 3) + 6 * delta_s * M2 - 4 * delta_div * M3;
                 M3  +=  diff * delta_div * (n - 2) - 3 * delta_div * M2;
                 M2  +=  diff;
             }
         }
 
-        if (cnt == 0) return -HUGE_VAL;
-        if (!is_na_or_inf(M2) && M2 <= 0)
+        if (unlikely(cnt == 0)) return -HUGE_VAL;
+        if (unlikely(!is_na_or_inf(M2) && M2 <= 0))
         {
             if (!check_more_than_two_unique_values(ix_arr, st, end, x, missing_action))
                 return -HUGE_VAL;
         }
 
         out = ( M4 / M2 ) * ( (ldouble_safe)cnt / M2 );
         return (!is_na_or_inf(out))? std::fmax((double)out, 0.) : (-HUGE_VAL);
@@ -174,15 +178,15 @@
     }
 
     else
     {
         size_t cnt = 0;
         for (size_t row = 0; row < n; row++)
         {
-            if (!is_na_or_inf(x[row]))
+            if (likely(!is_na_or_inf(x[row])))
             {
                 cnt++;
                 n_ = (ldouble_safe) cnt;
 
                 delta      =  x[row] - m;
                 delta_div  =  delta / n_;
                 delta_s    =  delta_div * delta_div;
@@ -191,15 +195,15 @@
                 m   +=  delta_div;
                 M4  +=  diff * delta_s * (n_ * n_ - 3 * n_ + 3) + 6 * delta_s * M2 - 4 * delta_div * M3;
                 M3  +=  diff * delta_div * (n_ - 2) - 3 * delta_div * M2;
                 M2  +=  diff;
             }
         }
 
-        if (cnt == 0) return -HUGE_VAL;
+        if (unlikely(cnt == 0)) return -HUGE_VAL;
 
         out = ( M4 / M2 ) * ( (ldouble_safe)cnt / M2 );
         return (!is_na_or_inf(out))? std::fmax((double)out, 0.) : (-HUGE_VAL);
     }
 }
 
 /* TODO: is this algorithm correct? */
@@ -214,15 +218,15 @@
     ldouble_safe n = 0;
     ldouble_safe out;
     ldouble_safe n_prev = 0.;
     ldouble_safe w_this;
 
     for (size_t row = st; row <= end; row++)
     {
-        if (!is_na_or_inf(x[ix_arr[row]]))
+        if (likely(!is_na_or_inf(x[ix_arr[row]])))
         {
             w_this = w[ix_arr[row]];
             n += w_this;
 
             delta      =  x[ix_arr[row]] - m;
             delta_div  =  delta / n;
             delta_s    =  delta_div * delta_div;
@@ -232,16 +236,16 @@
             m   +=  w_this * (delta_div);
             M4  +=  w_this * (diff * delta_s * (n * n - 3 * n + 3) + 6 * delta_s * M2 - 4 * delta_div * M3);
             M3  +=  w_this * (diff * delta_div * (n - 2) - 3 * delta_div * M2);
             M2  +=  w_this * (diff);
         }
     }
 
-    if (n <= 0) return -HUGE_VAL;
-    if (!is_na_or_inf(M2) && M2 <= std::numeric_limits<double>::epsilon())
+    if (unlikely(n <= 0)) return -HUGE_VAL;
+    if (unlikely(!is_na_or_inf(M2) && M2 <= std::numeric_limits<double>::epsilon()))
     {
         if (!check_more_than_two_unique_values(ix_arr, st, end, x, missing_action))
             return -HUGE_VAL;
     }
 
     out = ( M4 / M2 ) * ( n / M2 );
     return (!is_na_or_inf(out))? std::fmax((double)out, 0.) : (-HUGE_VAL);
@@ -257,15 +261,15 @@
     ldouble_safe n = 0;
     ldouble_safe out;
     ldouble_safe n_prev = 0.;
     ldouble_safe w_this;
 
     for (size_t row = 0; row < n_; row++)
     {
-        if (!is_na_or_inf(x[row]))
+        if (likely(!is_na_or_inf(x[row])))
         {
             w_this = w[row];
             n += w_this;
 
             delta      =  x[row] - m;
             delta_div  =  delta / n;
             delta_s    =  delta_div * delta_div;
@@ -275,15 +279,15 @@
             m   +=  w_this * (delta_div);
             M4  +=  w_this * (diff * delta_s * (n * n - 3 * n + 3) + 6 * delta_s * M2 - 4 * delta_div * M3);
             M3  +=  w_this * (diff * delta_div * (n - 2) - 3 * delta_div * M2);
             M2  +=  w_this * (diff);
         }
     }
 
-    if (n <= 0) return -HUGE_VAL;
+    if (unlikely(n <= 0)) return -HUGE_VAL;
 
     out = ( M4 / M2 ) * ( n / M2 );
     return (!is_na_or_inf(out))? std::fmax((double)out, 0.) : (-HUGE_VAL);
 }
 
 
 /* TODO: make these compensated sums */
@@ -301,15 +305,15 @@
     ldouble_safe s1 = 0;
     ldouble_safe s2 = 0;
     ldouble_safe s3 = 0;
     ldouble_safe s4 = 0;
     ldouble_safe x_sq;
     size_t cnt = end - st + 1;
 
-    if (cnt <= 1) return -HUGE_VAL;
+    if (unlikely(cnt <= 1)) return -HUGE_VAL;
     
     size_t st_col  = Xc_indptr[col_num];
     size_t end_col = Xc_indptr[col_num + 1] - 1;
     size_t curr_pos = st_col;
     size_t ind_end_col = Xc_ind[end_col];
     size_t *ptr_st = std::lower_bound(ix_arr + st, ix_arr + end + 1, Xc_ind[st_col]);
 
@@ -320,15 +324,15 @@
         for (size_t *row = ptr_st;
              row != ix_arr + end + 1 && curr_pos != end_col + 1 && ind_end_col >= *row;
             )
         {
             if (Xc_ind[curr_pos] == (sparse_ix)(*row))
             {
                 xval = Xc[curr_pos];
-                if (is_na_or_inf(xval))
+                if (unlikely(is_na_or_inf(xval)))
                 {
                     cnt--;
                 }
 
                 else
                 {
                     /* TODO: is it safe to use FMA here? some calculations rely on assuming that
@@ -354,15 +358,15 @@
                 if (Xc_ind[curr_pos] > (sparse_ix)(*row))
                     row = std::lower_bound(row + 1, ix_arr + end + 1, Xc_ind[curr_pos]);
                 else
                     curr_pos = std::lower_bound(Xc_ind + curr_pos + 1, Xc_ind + end_col + 1, *row) - Xc_ind;
             }
         }
 
-        if (cnt <= (end - st + 1) - (Xc_indptr[col_num+1] - Xc_indptr[col_num])) return -HUGE_VAL;
+        if (unlikely(cnt <= (end - st + 1) - (Xc_indptr[col_num+1] - Xc_indptr[col_num]))) return -HUGE_VAL;
     }
 
     else
     {
         for (size_t *row = ptr_st;
              row != ix_arr + end + 1 && curr_pos != end_col + 1 && ind_end_col >= *row;
             )
@@ -390,27 +394,27 @@
                     row = std::lower_bound(row + 1, ix_arr + end + 1, Xc_ind[curr_pos]);
                 else
                     curr_pos = std::lower_bound(Xc_ind + curr_pos + 1, Xc_ind + end_col + 1, *row) - Xc_ind;
             }
         }
     }
 
-    if (cnt <= 1 || s2 == 0 || s2 == pw2(s1)) return -HUGE_VAL;
+    if (unlikely(cnt <= 1 || s2 == 0 || s2 == pw2(s1))) return -HUGE_VAL;
     ldouble_safe cnt_l = (ldouble_safe) cnt;
     ldouble_safe sn = s1 / cnt_l;
     ldouble_safe v  = s2 / cnt_l - pw2(sn);
-    if (std::isnan(v)) return -HUGE_VAL;
+    if (unlikely(std::isnan(v))) return -HUGE_VAL;
     if (
         v <= std::numeric_limits<double>::epsilon() &&
         !check_more_than_two_unique_values(ix_arr, st, end, col_num,
                                            Xc_indptr, Xc_ind, Xc,
                                            missing_action)
     )
         return -HUGE_VAL;
-    if (v <= 0) return 0.;
+    if (unlikely(v <= 0)) return 0.;
     ldouble_safe out =  (s4 - 4 * s3 * sn + 6 * s2 * pw2(sn) - 4 * s1 * pw3(sn) + cnt_l * pw4(sn)) / (cnt_l * pw2(v));
     return (!is_na_or_inf(out))? std::fmax((double)out, 0.) : (-HUGE_VAL);
 }
 
 template <class real_t, class sparse_ix>
 double calc_kurtosis(size_t col_num, size_t nrows,
                      real_t Xc[], sparse_ix *restrict Xc_ind, sparse_ix *restrict Xc_indptr,
@@ -422,24 +426,24 @@
     ldouble_safe s1 = 0;
     ldouble_safe s2 = 0;
     ldouble_safe s3 = 0;
     ldouble_safe s4 = 0;
     ldouble_safe x_sq;
     size_t cnt = nrows;
 
-    if (cnt <= 1) return -HUGE_VAL;
+    if (unlikely(cnt <= 1)) return -HUGE_VAL;
 
     ldouble_safe xval;
 
     if (missing_action != Fail)
     {
         for (auto ix = Xc_indptr[col_num]; ix < Xc_indptr[col_num+1]; ix++)
         {
             xval = Xc[ix];
-            if (is_na_or_inf(xval))
+            if (unlikely(is_na_or_inf(xval)))
             {
                 cnt--;
             }
 
             else
             {
                 x_sq = square(xval);
@@ -470,27 +474,27 @@
             // s1 += pw1(xval);
             // s2 += pw2(xval);
             // s3 += pw3(xval);
             // s4 += pw4(xval);
         }
     }
 
-    if (cnt <= 1 || s2 == 0 || s2 == pw2(s1)) return -HUGE_VAL;
+    if (unlikely(cnt <= 1 || s2 == 0 || s2 == pw2(s1))) return -HUGE_VAL;
     ldouble_safe cnt_l = (ldouble_safe) cnt;
     ldouble_safe sn = s1 / cnt_l;
     ldouble_safe v  = s2 / cnt_l - pw2(sn);
-    if (std::isnan(v)) return -HUGE_VAL;
+    if (unlikely(std::isnan(v))) return -HUGE_VAL;
     if (
         v <= std::numeric_limits<double>::epsilon() &&
         !check_more_than_two_unique_values(nrows, col_num,
                                            Xc_indptr, Xc_ind, Xc,
                                            missing_action)
     )
         return -HUGE_VAL;
-    if (v <= 0) return 0.;
+    if (unlikely(v <= 0)) return 0.;
     ldouble_safe out =  (s4 - 4 * s3 * sn + 6 * s2 * pw2(sn) - 4 * s1 * pw3(sn) + cnt_l * pw4(sn)) / (cnt_l * pw2(v));
     return (!is_na_or_inf(out))? std::fmax((double)out, 0.) : (-HUGE_VAL);
 }
 
 
 template <class real_t, class sparse_ix, class mapping>
 double calc_kurtosis_weighted(size_t *restrict ix_arr, size_t st, size_t end, size_t col_num,
@@ -507,15 +511,15 @@
     ldouble_safe s4 = 0;
     ldouble_safe x_sq;
     ldouble_safe w_this;
     ldouble_safe cnt = 0;
     for (size_t row = st; row <= end; row++)
         cnt += w[ix_arr[row]];
 
-    if (cnt <= 0) return -HUGE_VAL;
+    if (unlikely(cnt <= 0)) return -HUGE_VAL;
     
     size_t st_col  = Xc_indptr[col_num];
     size_t end_col = Xc_indptr[col_num + 1] - 1;
     size_t curr_pos = st_col;
     size_t ind_end_col = Xc_ind[end_col];
     size_t *ptr_st = std::lower_bound(ix_arr + st, ix_arr + end + 1, Xc_ind[st_col]);
 
@@ -528,15 +532,15 @@
             )
         {
             if (Xc_ind[curr_pos] == (sparse_ix)(*row))
             {
                 w_this = w[*row];
                 xval = Xc[curr_pos];
 
-                if (is_na_or_inf(xval))
+                if (unlikely(is_na_or_inf(xval)))
                 {
                     cnt -= w_this;
                 }
 
                 else
                 {
                     x_sq = xval * xval;
@@ -559,15 +563,15 @@
                 if (Xc_ind[curr_pos] > (sparse_ix)(*row))
                     row = std::lower_bound(row + 1, ix_arr + end + 1, Xc_ind[curr_pos]);
                 else
                     curr_pos = std::lower_bound(Xc_ind + curr_pos + 1, Xc_ind + end_col + 1, *row) - Xc_ind;
             }
         }
 
-        if (cnt <= 0) return -HUGE_VAL;
+        if (unlikely(cnt <= 0)) return -HUGE_VAL;
     }
 
     else
     {
         for (size_t *row = ptr_st;
              row != ix_arr + end + 1 && curr_pos != end_col + 1 && ind_end_col >= *row;
             )
@@ -597,18 +601,18 @@
                     row = std::lower_bound(row + 1, ix_arr + end + 1, Xc_ind[curr_pos]);
                 else
                     curr_pos = std::lower_bound(Xc_ind + curr_pos + 1, Xc_ind + end_col + 1, *row) - Xc_ind;
             }
         }
     }
 
-    if (cnt <= 1 || s2 == 0 || s2 == pw2(s1)) return -HUGE_VAL;
+    if (unlikely(cnt <= 1 || s2 == 0 || s2 == pw2(s1))) return -HUGE_VAL;
     ldouble_safe sn = s1 / cnt;
     ldouble_safe v  = s2 / cnt - pw2(sn);
-    if (std::isnan(v)) return -HUGE_VAL;
+    if (unlikely(std::isnan(v))) return -HUGE_VAL;
     if (
         v <= std::numeric_limits<double>::epsilon() &&
         !check_more_than_two_unique_values(ix_arr, st, end, col_num,
                                            Xc_indptr, Xc_ind, Xc,
                                            missing_action)
     )
         return -HUGE_VAL;
@@ -631,26 +635,26 @@
     ldouble_safe s4 = 0;
     ldouble_safe x_sq;
     ldouble_safe w_this;
     ldouble_safe cnt = nrows - (Xc_indptr[col_num + 1] - Xc_indptr[col_num]);
     for (auto ix = Xc_indptr[col_num]; ix < Xc_indptr[col_num + 1]; ix++)
         cnt += w[Xc_ind[ix]];
 
-    if (cnt <= 0) return -HUGE_VAL;
+    if (unlikely(cnt <= 0)) return -HUGE_VAL;
     
     ldouble_safe xval;
 
     if (missing_action != Fail)
     {
         for (auto ix = Xc_indptr[col_num]; ix < Xc_indptr[col_num + 1]; ix++)
         {
             w_this = w[Xc_ind[ix]];
             xval = Xc[ix];
 
-            if (is_na_or_inf(xval))
+            if (unlikely(is_na_or_inf(xval)))
             {
                 cnt -= w_this;
             }
 
             else
             {
                 x_sq = xval * xval;
@@ -683,26 +687,26 @@
             // s1 += w_this * pw1(xval);
             // s2 += w_this * pw2(xval);
             // s3 += w_this * pw3(xval);
             // s4 += w_this * pw4(xval);
         }
     }
 
-    if (cnt <= 1 || s2 == 0 || s2 == pw2(s1)) return -HUGE_VAL;
+    if (unlikely(cnt <= 1 || s2 == 0 || s2 == pw2(s1))) return -HUGE_VAL;
     ldouble_safe sn = s1 / cnt;
     ldouble_safe v  = s2 / cnt - pw2(sn);
-    if (std::isnan(v)) return -HUGE_VAL;
+    if (unlikely(std::isnan(v))) return -HUGE_VAL;
     if (
         v <= std::numeric_limits<double>::epsilon() &&
         !check_more_than_two_unique_values(nrows, col_num,
                                            Xc_indptr, Xc_ind, Xc,
                                            missing_action)
     )
         return -HUGE_VAL;
-    if (v <= 0) return -HUGE_VAL;
+    if (unlikely(v <= 0)) return -HUGE_VAL;
     ldouble_safe out =  (s4 - 4 * s3 * sn + 6 * s2 * pw2(sn) - 4 * s1 * pw3(sn) + cnt * pw4(sn)) / (cnt * pw2(v));
     return (!is_na_or_inf(out))? std::fmax((double)out, 0.) : (-HUGE_VAL);
 }
 
 
 
 double calc_kurtosis_internal(size_t cnt, int x[], int ncat, size_t buffer_cnt[], double buffer_prob[],
@@ -755,17 +759,17 @@
                 }
                 temp_v = s2 - pw2(s1);
                 if (temp_v <= 0)
                     ntry--;
                 else
                     sum_kurt += (s4 - 4 * s3 * pw1(s1) + 6 * s2 * pw2(s1) - 4 * s1 * pw3(s1) + pw4(s1)) / pw2(temp_v);
             }
-            if (!ntry)
+            if (unlikely(!ntry))
                 return -HUGE_VAL;
-            else if (is_na_or_inf(sum_kurt))
+            else if (unlikely(is_na_or_inf(sum_kurt)))
                 return -HUGE_VAL;
             else
                 return std::fmax(sum_kurt, 0.) / (double)ntry;
         }
 
         case SingleCateg:
         {
@@ -777,15 +781,15 @@
                 if (p == 0)
                     ncat_present--;
                 else
                     sum_kurt += (p - 4 * p * pw1(p) + 6 * p * pw2(p) - 4 * p * pw3(p) + pw4(p)) / pw2(p - pw2(p));
             }
             if (ncat_present <= 1)
                 return -HUGE_VAL;
-            else if (is_na_or_inf(sum_kurt))
+            else if (unlikely(is_na_or_inf(sum_kurt)))
                 return -HUGE_VAL;
             else
                 return std::fmax(sum_kurt, 0.) / (double)ncat_present;
         }
     }
 
     return -1; /* this will never be reached, but CRAN complains otherwise */
@@ -812,15 +816,15 @@
             buffer_cnt[x[ix_arr[row]]]++;
     }
 
     else
     {
         for (size_t row = st; row <= end; row++)
         {
-            if (x[ix_arr[row]] >= 0)
+            if (likely(x[ix_arr[row]] >= 0))
                 buffer_cnt[x[ix_arr[row]]]++;
             else
                 buffer_cnt[ncat]++;
         }
     }
 
     return calc_kurtosis_internal(cnt, x, ncat, buffer_cnt, buffer_prob,
@@ -839,15 +843,15 @@
             buffer_cnt[x[row]]++;
     }
 
     else
     {
         for (size_t row = 0; row < nrows; row++)
         {
-            if (x[row] >= 0)
+            if (likely(x[row] >= 0))
                 buffer_cnt[x[row]]++;
             else
                 buffer_cnt[ncat]++;
         }
     }
 
     return calc_kurtosis_internal(cnt, x, ncat, buffer_cnt, buffer_prob,
@@ -862,15 +866,15 @@
                                        RNG_engine &rnd_generator, mapping &w)
 {
     double sum_kurt = 0;
 
     ldouble_safe cnt = std::accumulate(buffer_cnt.begin(), buffer_cnt.end(), (ldouble_safe)0);
 
     cnt -= buffer_cnt[ncat];
-    if (cnt <= 1) return -HUGE_VAL;
+    if (unlikely(cnt <= 1)) return -HUGE_VAL;
     for (int cat = 0; cat < ncat; cat++)
         buffer_prob[cat] = buffer_cnt[cat] / cnt;
 
     switch (cat_split_type)
     {
         case SubSet:
         {
@@ -894,22 +898,22 @@
                     s4 = std::fma(w_this, coef2*coef2, s4);
                     // s1 += buffer_prob[cat] * pw1(coef);
                     // s2 += buffer_prob[cat] * pw2(coef);
                     // s3 += buffer_prob[cat] * pw3(coef);
                     // s4 += buffer_prob[cat] * pw4(coef);
                 }
                 temp_v = s2 - pw2(s1);
-                if (temp_v <= 0)
+                if (unlikely(temp_v <= 0))
                     ntry--;
                 else
                     sum_kurt += (s4 - 4 * s3 * pw1(s1) + 6 * s2 * pw2(s1) - 4 * s1 * pw3(s1) + pw4(s1)) / pw2(temp_v);
             }
-            if (!ntry)
+            if (unlikely(!ntry))
                 return -HUGE_VAL;
-            else if (is_na_or_inf(sum_kurt))
+            else if (unlikely(is_na_or_inf(sum_kurt)))
                 return -HUGE_VAL;
             else
                 return std::fmax(sum_kurt, 0.) / (double)ntry;
         }
 
         case SingleCateg:
         {
@@ -921,15 +925,15 @@
                 if (p == 0)
                     ncat_present--;
                 else
                     sum_kurt += (p - 4 * p * pw1(p) + 6 * p * pw2(p) - 4 * p * pw3(p) + pw4(p)) / pw2(p - pw2(p));
             }
             if (ncat_present <= 1)
                 return -HUGE_VAL;
-            else if (is_na_or_inf(sum_kurt))
+            else if (unlikely(is_na_or_inf(sum_kurt)))
                 return -HUGE_VAL;
             else
                 return std::fmax(sum_kurt, 0.) / (double)ncat_present;
         }
     }
 
     return -1; /* this will never be reached, but CRAN complains otherwise */
@@ -941,15 +945,15 @@
 {
     std::vector<ldouble_safe> buffer_cnt(ncat+1, 0.);
     ldouble_safe w_this;
 
     for (size_t row = st; row <= end; row++)
     {
         w_this = w[ix_arr[row]];
-        if (x[ix_arr[row]] >= 0)
+        if (likely(x[ix_arr[row]] >= 0))
             buffer_cnt[x[ix_arr[row]]] += w_this;
         else
             buffer_cnt[ncat] += w_this;
     }
     
     return calc_kurtosis_weighted_internal(buffer_cnt, x, ncat,
                                            buffer_prob, missing_action, cat_split_type,
@@ -963,15 +967,15 @@
 {
     std::vector<ldouble_safe> buffer_cnt(ncat+1, 0.);
     ldouble_safe w_this;
 
     for (size_t row = 0; row < nrows; row++)
     {
         w_this = w[row];
-        if (x[row] >= 0)
+        if (likely(x[row] >= 0))
             buffer_cnt[x[row]] += w_this;
         else
             buffer_cnt[ncat] += w_this;
     }
     
     return calc_kurtosis_weighted_internal(buffer_cnt, x, ncat,
                                            buffer_prob, missing_action, cat_split_type,
@@ -1080,28 +1084,28 @@
 
     if (missing_action != Fail)
     {
         int xval;
         for (size_t row = st; row <= end; row++)
         {
             xval = x[ix_arr[row]];
-            if (xval < 0)
+            if (unlikely(xval < 0))
                 buffer_cnt[ncat]++;
             else
                 buffer_cnt[xval]++;
         }
         cnt -= buffer_cnt[ncat];
         if (cnt == 0) return 0;
     }
 
     else
     {
         for (size_t row = st; row <= end; row++)
         {
-            if (x[ix_arr[row]] >= 0) buffer_cnt[x[ix_arr[row]]]++;
+            if (likely(x[ix_arr[row]] >= 0)) buffer_cnt[x[ix_arr[row]]]++;
         }
     }
 
     return expected_sd_cat_internal(ncat, buffer_cnt, cnt, buffer_pos, buffer_prob);
 }
 
 template <class mapping>
@@ -1118,37 +1122,37 @@
         int xval;
         double w_this;
         for (size_t row = st; row <= end; row++)
         {
             xval = x[ix_arr[row]];
             w_this = w[ix_arr[row]];
 
-            if (xval < 0) {
+            if (unlikely(xval < 0)) {
                 buffer_cnt[ncat] += w_this;
             }
             else {
                 buffer_cnt[xval] += w_this;
                 cnt += w_this;
             }
         }
         if (cnt == 0) return 0;
     }
 
     else
     {
         for (size_t row = st; row <= end; row++)
         {
-            if (x[ix_arr[row]] >= 0)
+            if (likely(x[ix_arr[row]] >= 0))
             {
                 buffer_cnt[x[ix_arr[row]]] += w[ix_arr[row]];
             }
         }
         for (int cat = 0; cat < ncat; cat++)
             cnt += buffer_cnt[cat];
-        if (cnt == 0) return 0;
+        if (unlikely(cnt == 0)) return 0;
     }
 
     return expected_sd_cat_internal(ncat, buffer_cnt, cnt, buffer_pos, buffer_prob);
 }
 
 /* Note: this isn't exactly comparable to the pooled gain from numeric variables,
    but among all the possible options, this is what happens to end up in the most
@@ -1238,15 +1242,15 @@
     Maybe it should instead use sums of centered squares: sigma = sqrt((x-mean(x))^2/n)
     The sums of centered squares method is also likely to be more precise. */
 
 template <class real_t>
 double midpoint(real_t x, real_t y)
 {
     real_t m = x + (y-x)/(real_t)2;
-    if ((double)m < (double)y)
+    if (likely((double)m < (double)y))
         return m;
     else {
         m = std::nextafter(m, y);
         if (m > x && m < y)
             return m;
         else
             return x;
@@ -1671,15 +1675,15 @@
                         double &restrict split_point, double &restrict xmin, double &restrict xmax)
 {
     /* Note: the input 'x' is supposed to be a linear combination of standardized variables, so
        all numbers are assumed to be small and in the same scale */
     double gain;
 
     /* here it's assumed the 'x' vector matches exactly with 'ix_arr' + 'st' */
-    if (n == 2)
+    if (unlikely(n == 2))
     {
         if (x[0] == x[1]) return -HUGE_VAL;
         split_point = midpoint_with_reorder(x[0], x[1]);
         gain        = 1.;
         if (gain > min_gain)
             return gain;
         else
@@ -1705,15 +1709,15 @@
                                  double *restrict w, size_t *restrict buffer_indices)
 {
     /* Note: the input 'x' is supposed to be a linear combination of standardized variables, so
        all numbers are assumed to be small and in the same scale */
     double gain;
 
     /* here it's assumed the 'x' vector matches exactly with 'ix_arr' + 'st' */
-    if (n == 2)
+    if (unlikely(n == 2))
     {
         if (x[0] == x[1]) return -HUGE_VAL;
         split_point = midpoint_with_reorder(x[0], x[1]);
         gain        = 1.;
         if (gain > min_gain)
             return gain;
         else
@@ -1743,16 +1747,16 @@
     size_t st_orig = st;
     double gain;
 
     /* move NAs to the front if there's any, exclude them from calculations */
     if (missing_action != Fail)
         st = move_NAs_to_front(ix_arr, st, end, x);
 
-    if (st >= end) return -HUGE_VAL;
-    else if (st == (end-1))
+    if (unlikely(st >= end)) return -HUGE_VAL;
+    else if (unlikely(st == (end-1)))
     {
         if (x[ix_arr[st]] == x[ix_arr[end]])
             return -HUGE_VAL;
         split_point = midpoint_with_reorder(x[ix_arr[st]], x[ix_arr[end]]);
         split_ix    = st;
         gain        = 1.;
         if (gain > min_gain)
@@ -1812,16 +1816,16 @@
     size_t st_orig = st;
     double gain;
 
     /* move NAs to the front if there's any, exclude them from calculations */
     if (missing_action != Fail)
         st = move_NAs_to_front(ix_arr, st, end, x);
 
-    if (st >= end) return -HUGE_VAL;
-    else if (st == (end-1))
+    if (unlikely(st >= end)) return -HUGE_VAL;
+    else if (unlikely(st == (end-1)))
     {
         if (x[ix_arr[st]] == x[ix_arr[end]])
             return -HUGE_VAL;
         split_point = midpoint_with_reorder(x[ix_arr[st]], x[ix_arr[end]]);
         split_ix    = st;
         gain        = 1.;
         if (gain > min_gain)
@@ -1893,15 +1897,15 @@
     std::iota(buffer_pos, buffer_pos + tot, (size_t)0);
 
     if (missing_action == Impute)
     {
         missing_action = Fail;
         for (size_t ix = 0; ix < tot; ix++)
         {
-            if (is_na_or_inf(buffer_arr[ix]))
+            if (unlikely(is_na_or_inf(buffer_arr[ix])))
             {
                 goto fill_missing;
             }
         }
         goto no_nas;
 
         fill_missing:
@@ -1949,15 +1953,15 @@
 
 
     if (missing_action == Impute)
     {
         missing_action = Fail;
         for (size_t ix = 0; ix < tot; ix++)
         {
-            if (is_na_or_inf(buffer_arr[ix]))
+            if (unlikely(is_na_or_inf(buffer_arr[ix])))
             {
                 goto fill_missing;
             }
         }
         goto no_nas;
 
         fill_missing:
@@ -2029,36 +2033,36 @@
     }
 
     else if (missing_action == Impute)
     {
         for (size_t row = st; row <= end; row++)
         {
             xval = x[ix_arr[row]];
-            if (xval < 0)
+            if (unlikely(xval < 0))
                 n_nas++;
             else
                 buffer_cnt[xval]++;
         }
 
-        if (n_nas >= end-st) return -HUGE_VAL;
+        if (unlikely(n_nas >= end-st)) return -HUGE_VAL;
 
         if (n_nas)
         {
             auto idxmax = std::max_element(buffer_cnt, buffer_cnt + ncat);
             *idxmax += n_nas;
             *saved_cat_mode = (int)std::distance(buffer_cnt, idxmax);
         }
     }
 
     else
     {
         for (size_t row = st; row <= end; row++)
         {
             xval = x[ix_arr[row]];
-            if (xval >= 0) buffer_cnt[xval]++;
+            if (likely(xval >= 0)) buffer_cnt[xval]++;
         }
     }
 
     double this_gain = -HUGE_VAL;
     double best_gain = -HUGE_VAL;
     std::iota(buffer_pos, buffer_pos + ncat, (size_t)0);
     size_t st_pos = 0;
@@ -2351,25 +2355,26 @@
     /* TODO: allocate this buffer externally */
     std::vector<ldouble_safe> buffer_cnt(ncat, (ldouble_safe)0);
     if (missing_action == Fail)
     {
         for (size_t row = st; row <= end; row++)
         {
             ix_ = ix_arr[row];
+            if (unlikely(x[ix_]) < 0) continue;
             buffer_cnt[x[ix_]] += w[ix_];
         }
     }
 
     else if (missing_action == Impute)
     {
         for (size_t row = st; row <= end; row++)
         {
             ix_ = ix_arr[row];
             xval = x[ix_];
-            if (xval < 0)
+            if (unlikely(xval < 0))
                 w_missing += w[ix_];
             else
                 buffer_cnt[xval] += w[ix_];
         }
 
         if (w_missing)
         {
@@ -2381,15 +2386,15 @@
 
     else
     {
         for (size_t row = st; row <= end; row++)
         {
             ix_ = ix_arr[row];
             xval = x[ix_];
-            if (xval >= 0) buffer_cnt[xval] += w[ix_];
+            if (likely(xval >= 0)) buffer_cnt[xval] += w[ix_];
         }
     }
 
     ldouble_safe cnt = std::accumulate(buffer_cnt.begin(), buffer_cnt.end(), (ldouble_safe)0);
 
     double this_gain = -HUGE_VAL;
     double best_gain = -HUGE_VAL;
```

### Comparing `isotree-0.5.8.post1/src/dist.hpp` & `isotree-0.5.9/src/dist.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -30,14 +30,19 @@
 *          arXiv preprint arXiv:2110.13402 (2021).
 *     [12] Guha, Sudipto, et al.
 *          "Robust random cut forest based anomaly detection on streams."
 *          International conference on machine learning. PMLR, 2016.
 *     [13] Cortes, David.
 *          "Isolation forests: looking beyond tree depth."
 *          arXiv preprint arXiv:2111.11639 (2021).
+*     [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou.
+*          "Isolation kernel and its effect on SVM"
+*          Proceedings of the 24th ACM SIGKDD
+*          International Conference on Knowledge Discovery & Data Mining. 2018.
+* 
 *     BSD 2-Clause License
 *     Copyright (c) 2019-2022, David Cortes
 *     All rights reserved.
 *     Redistribution and use in source and binary forms, with or without
 *     modification, are permitted provided that the following conditions are met:
 *     * Redistributions of source code must retain the above copyright notice, this
 *       list of conditions and the following disclaimer.
@@ -54,24 +59,15 @@
 *     CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 *     OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 *     OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 */
 #include "isotree.hpp" 
 
 
-/* TODO: the method used here is quite slow. From a high level perspective, what the code
-   in this file does is to pass observations down a tree and add +1 for each pair at each
-   step, but this is not actually necessary, as it's also possible to precompute the
-   separation depths between each pair of terminal nodes and then make only one addition
-   per tree for each pair of observations. Should add a 'precompute_distances' method
-   here as a different object class, and perhaps add also the 'isolation kernel'
-   technique for comparison purposes. */
-
-
-/* Calculate distance or similarity between data points
+/* Calculate distance or similarity or kernel/proximity between data points
 * 
 * Parameters
 * ==========
 * - numeric_data[nrows * ncols_numeric]
 *       Pointer to numeric data for which to make calculations. If not using 'indexer', must be
 *       ordered by columns like Fortran, not ordered by rows like C (i.e. entries 1..n contain
 *       column 0, n+1..2n column 1, etc.), while if using 'indexer', may be passed in either
@@ -118,75 +114,98 @@
 *       Pass NULL if there are no sparse numeric columns in CSC or CSR format.
 *       If making calculations between two sets of observations/rows (see documentation for 'rmat'),
 *       the first group is assumed to be the earlier rows here.
 * - nrows
 *       Number of rows in 'numeric_data', 'Xc', 'categ_data'.
 * - nthreads
 *       Number of parallel threads to use. Note that, the more threads, the more memory will be
-*       allocated, even if the thread does not end up being used. Ignored when not building with
-*       OpenMP support.
+*       allocated, even if the thread does not end up being used (with one exception being kernel calculations
+*       with respect to reference points in an idexer). Ignored when not building with OpenMP support.
 * - assume_full_distr
 *       Whether to assume that the fitted model represents a full population distribution (will use a
 *       standardizing criterion assuming infinite sample, and the results of the similarity between two points
 *       at prediction time will not depend on the prescence of any third point that is similar to them, but will
 *       differ more compared to the pairwise distances between points from which the model was fit). If passing
 *       'false', will calculate pairwise distances as if the new observations at prediction time were added to
 *       the sample to which each tree was fit, which will make the distances between two points potentially vary
 *       according to other newly introduced points.
 *       This was added for experimentation purposes only and it's not recommended to pass 'false'.
 *       Note that when calculating distances using 'indexer', there
 *       might be slight discrepancies between the numbers produced with or without the indexer due to what
 *       are considered "additional" observations in this calculation.
+*       This is ignored when passing 'as_kernel=true'.
 * - standardize_dist
 *       Whether to standardize the resulting average separation depths between rows according
 *       to the expected average separation depth in a similar way as when predicting outlierness,
 *       in order to obtain a standardized distance. If passing 'false', will output the average
 *       separation depth instead.
+*       If passing 'as_kernel=true', this indicates whether to output a fraction (if 'true') or
+*       the raw number of matching trees (if 'false').
+* - as_kernel
+*       Whether to calculate the "similarities" as isolation kernel or proximity matrix, which counts
+*       the proportion of trees in which two observations end up in the same terminal node. This is
+*       typically much faster than separation-based distance, but is typically not as good quality.
+*       Note that, for kernel calculations, the indexer is only used if it has reference points stored on it.
 * - model_outputs
 *       Pointer to fitted single-variable model object from function 'fit_iforest'. Pass NULL
 *       if the calculations are to be made from an extended model. Can only pass one of
 *       'model_outputs' and 'model_outputs_ext'.
 * - model_outputs_ext
 *       Pointer to fitted extended model object from function 'fit_iforest'. Pass NULL
 *       if the calculations are to be made from a single-variable model. Can only pass one of
 *       'model_outputs' and 'model_outputs_ext'.
 * - tmat[nrows * (nrows - 1) / 2] (out)
-*       Pointer to array where the resulting pairwise distances or average separation depths will
+*       Pointer to array where the resulting pairwise distances or average separation depths or kernels will
 *       be written into. As the output is a symmetric matrix, this function will only fill in the
 *       upper-triangular part, in which entry 0 <= i < j < n will be located at position
 *           p(i,j) = (i * (n - (i+1)/2) + j - i - 1).
 *       Can be converted to a dense square matrix through function 'tmat_to_dense'.
 *       The array must already be initialized to zeros.
 *       If calculating distance/separation from a group of points to another group of points,
 *       pass NULL here and use 'rmat' instead.
 * - rmat[nrows1 * nrows2] (out)
-*       Pointer to array where to write the distances or separation depths between each row in
+*       Pointer to array where to write the distances or separation depths or kernels between each row in
 *       one set of observations and each row in a different set of observations. If doing these
 *       calculations for all pairs of observations/rows, pass 'tmat' instead.
 *       Will take the first group of observations as the rows in this matrix, and the second
 *       group as the columns. The groups are assumed to be in the same data arrays, with the
 *       first group corresponding to the earlier rows there.
-*       This matrix will be used in row-major order (i.e. entries 1..n_from contain the first row).
+*       This matrix will be used in row-major order (i.e. entries 1..nrows2 contain the first row from nrows1).
 *       Must be already initialized to zeros.
+*       If passing 'use_indexed_references=true' plus an indexer object with reference points, this
+*       array should have dimension [nrows, n_references].
 *       Ignored when 'tmat' is passed.
 * - n_from
 *       When calculating distances between two groups of points, this indicates the number of
 *       observations/rows belonging to the first group (the rows in 'rmat'), which will be
 *       assumed to be the first 'n_from' rows.
-*       Ignored when 'tmat' is passed.
+*       Ignored when 'tmat' is passed or when 'use_indexed_references=true' plus an indexer with
+*       references are passed.
+* - use_indexed_references
+*       Whether to calculate distances with respect to reference points stored in the indexer
+*       object, if it has any. This is only supported with 'assume_full_distr=true' or with 'as_kernel=true'.
+*       If passing 'use_indexed_references=true', then 'tmat' must be NULL, and 'rmat' must
+*       be of dimension [nrows, n_references].
 * - indexer
 *       Pointer to associated tree indexer for the model being used, if it was constructed,
 *       which can be used to speed up distance calculations, assuming that it was built with
 *       option 'with_distances=true'. If it does not contain node distances, it will not be used.
 *       Pass NULL if the indexer has not been constructed or was constructed with 'with_distances=false'.
+*       If it contains reference points and passing 'use_indexed_references=true', distances will be
+*       calculated between between the input data passed here and the reference points stored in this object.
+*       If passing 'as_kernel=true', the indexer can only be used for calculating kernels with respect to
+*       reference points in the indexer, otherwise it will not be used (which also means that the data must be
+*       passed in column-major order for all kernel calculations that are not with respect to reference points
+*       from an indexer).
 * - is_col_major
 *       Whether the data comes in column-major order. If using 'indexer', predictions are also possible
 *       (and are even faster for the case of dense-only data) if passing the data in row-major format.
-*       Without 'indexer', data may only be passed in column-major format.
-*       If there is sparse numeric data, it is highly suggested to pass it in CSR/column-major format.
+*       Without 'indexer' (and with 'as_kernel=true' but without reference points in the idnexer), data
+*       may only be passed in column-major format.
+*       If there is sparse numeric data, it is highly suggested to pass it in CSC/column-major format.
 * - ld_numeric
 *       If passing 'is_col_major=false', this indicates the leading dimension of the array 'numeric_data'.
 *       Typically, this corresponds to the number of columns, but may be larger (the array will
 *       be accessed assuming that row 'n' starts at 'numeric_data + n*ld_numeric'). If passing
 *       'numeric_data' in column-major order, this is ignored and will be assumed that the
 *       leading dimension corresponds to the number of rows. This is ignored when passing numeric
 *       data in sparse format.
@@ -198,54 +217,107 @@
 *       'categ_data' in column-major order, this is ignored and will be assumed that the
 *       leading dimension corresponds to the number of rows.
 *       Note that data in row-major order is only accepted when using 'indexer'.
 */
 template <class real_t, class sparse_ix>
 void calc_similarity(real_t numeric_data[], int categ_data[],
                      real_t Xc[], sparse_ix Xc_ind[], sparse_ix Xc_indptr[],
-                     size_t nrows, int nthreads, bool assume_full_distr, bool standardize_dist,
+                     size_t nrows, int nthreads,
+                     bool assume_full_distr, bool standardize_dist, bool as_kernel,
                      IsoForest *model_outputs, ExtIsoForest *model_outputs_ext,
-                     double tmat[], double rmat[], size_t n_from,
+                     double tmat[], double rmat[], size_t n_from, bool use_indexed_references,
                      TreesIndexer *indexer, bool is_col_major, size_t ld_numeric, size_t ld_categ)
 {
-    if (nrows < 2)
+    if (nrows < 2 && (!use_indexed_references || indexer == NULL || indexer->indices.empty() || indexer->indices.front().reference_points.empty()))
         throw std::runtime_error("Cannot calculate distances from less than 2 rows.\n");
+    if (as_kernel && (tmat != NULL || !use_indexed_references || (indexer != NULL && !indexer->indices.empty() && indexer->indices.front().reference_points.empty())))
+        indexer = NULL;
 
     if (indexer != NULL && model_outputs != NULL)
     {
-        if (model_outputs->missing_action == Divide)
+        if (model_outputs->missing_action == Divide) {
+            indexer = NULL;
+            if (use_indexed_references) throw std::runtime_error("Invalid indexer - cannot use references from it.\n");
+        }
+        if (model_outputs->new_cat_action == Weighted && model_outputs->cat_split_type == SubSet && categ_data != NULL) {
             indexer = NULL;
-        if (model_outputs->new_cat_action == Weighted && categ_data != NULL)
+            if (use_indexed_references) throw std::runtime_error("Invalid indexer - cannot use references from it.\n");
+        }
+    }
+    if (
+        !as_kernel &&
+        indexer != NULL &&
+        (indexer->indices.empty() || indexer->indices.front().node_distances.empty())
+    ) {
+        if (use_indexed_references && !indexer->indices.empty() && !indexer->indices.front().reference_points.empty())
+            throw std::runtime_error("Indexer was built without distances. Cannot use references from it.\n");
+        else {
             indexer = NULL;
+            fprintf(stderr, "Indexer has no pre-computed distances, will not be used for distance calculations.\n");
+        }
     }
-    if (indexer != NULL && (indexer->indices.empty() || indexer->indices.front().node_distances.empty()))
-        indexer = NULL;
     if (
         !is_col_major &&
         indexer == NULL &&
         (
             Xc_indptr != NULL
                 ||
             (nrows != 1 &&
              ((numeric_data != NULL && ld_numeric > 1) || (categ_data != NULL && ld_categ > 1)))
         )
     )
         throw std::runtime_error("Cannot calculate distances with row-major data without indexer.\n");
     if (indexer != NULL)
     {
-        calc_similarity_from_indexer(
-            numeric_data, categ_data,
-            Xc, Xc_ind, Xc_indptr,
-            nrows, nthreads, assume_full_distr, standardize_dist,
-            model_outputs, model_outputs_ext,
-            tmat, rmat, n_from,
-            indexer, is_col_major, ld_numeric, ld_categ
-        );
+        if (use_indexed_references && tmat == NULL && !indexer->indices.empty() && !indexer->indices.front().reference_points.empty())
+        {
+            if (unlikely(!assume_full_distr))
+                throw std::runtime_error("Cannot calculate distances to reference points in indexer with 'assume_full_distr=false'.\n");
+            
+            if (!as_kernel)
+            {
+                calc_similarity_from_indexer_with_references(
+                    numeric_data, categ_data,
+                    Xc, Xc_ind, Xc_indptr,
+                    nrows, nthreads, standardize_dist,
+                    model_outputs, model_outputs_ext,
+                    rmat,
+                    indexer, is_col_major, ld_numeric, ld_categ
+                );
+            }
+            
+            else
+            {
+                kernel_to_references(*indexer,
+                                     model_outputs, model_outputs_ext,
+                                     numeric_data, categ_data,
+                                     Xc, Xc_ind, Xc_indptr,
+                                     is_col_major, ld_numeric, ld_categ,
+                                     nrows, nthreads,
+                                     rmat,
+                                     standardize_dist);
+            }
+        }
+
+        else
+        {
+            if (as_kernel) goto skip_indexer_if_kernel;
+            calc_similarity_from_indexer(
+                numeric_data, categ_data,
+                Xc, Xc_ind, Xc_indptr,
+                nrows, nthreads, assume_full_distr, standardize_dist,
+                model_outputs, model_outputs_ext,
+                tmat, rmat, n_from,
+                indexer, is_col_major, ld_numeric, ld_categ
+            );
+        }
+
         return;
     }
+    skip_indexer_if_kernel:
 
     PredictionData<real_t, sparse_ix>
                    prediction_data = {numeric_data, categ_data, nrows,
                                       false, 0, 0,
                                       Xc, Xc_ind, Xc_indptr,
                                       NULL, NULL, NULL};
 
@@ -280,29 +352,42 @@
     #if defined(DONT_THROW_ON_INTERRUPT)
     if (interrupt_switch) return;
     #endif
     /* For handling exceptions */
     bool threw_exception = false;
     std::exception_ptr ex = NULL;
 
+    if (
+        tmat == NULL &&
+        use_indexed_references &&
+        indexer != NULL &&
+        !indexer->indices.empty() &&
+        !indexer->indices.front().reference_points.empty() &&
+        (as_kernel || !indexer->indices.front().node_distances.empty())
+    ) {
+        n_from = indexer->indices.front().reference_points.size();
+    }
+
     if (model_outputs != NULL)
     {
-        #pragma omp parallel for schedule(dynamic) num_threads(nthreads) shared(ntrees, worker_memory, prediction_data, model_outputs, ex, threw_exception)
+        #pragma omp parallel for schedule(dynamic) num_threads(nthreads) \
+                shared(ntrees, worker_memory, prediction_data, model_outputs, ex, threw_exception, n_from)
         for (size_t_for tree = 0; tree < (decltype(tree))ntrees; tree++)
         {
             if (threw_exception || interrupt_switch) continue;
             try
             {
                 initialize_worker_for_sim(worker_memory[omp_get_thread_num()], prediction_data,
                                           model_outputs, NULL, n_from, assume_full_distr);
                 traverse_tree_sim(worker_memory[omp_get_thread_num()],
                                   prediction_data,
                                   *model_outputs,
                                   model_outputs->trees[tree],
-                                  (size_t)0);
+                                  (size_t)0,
+                                  as_kernel);
             }
 
             catch (...)
             {
                 #pragma omp critical
                 {
                     if (!threw_exception)
@@ -313,27 +398,29 @@
                 }
             }
         }
     }
 
     else
     {
-        #pragma omp parallel for schedule(dynamic) num_threads(nthreads) shared(ntrees, worker_memory, prediction_data, model_outputs_ext, ex, threw_exception)
+        #pragma omp parallel for schedule(dynamic) num_threads(nthreads) \
+                shared(ntrees, worker_memory, prediction_data, model_outputs_ext, ex, threw_exception, n_from)
         for (size_t_for hplane = 0; hplane < (decltype(hplane))ntrees; hplane++)
         {
             if (threw_exception || interrupt_switch) continue;
             try
             {
                 initialize_worker_for_sim(worker_memory[omp_get_thread_num()], prediction_data,
                                           NULL, model_outputs_ext, n_from, assume_full_distr);
                 traverse_hplane_sim(worker_memory[omp_get_thread_num()],
                                     prediction_data,
                                     *model_outputs_ext,
                                     model_outputs_ext->hplanes[hplane],
-                                    (size_t)0);
+                                    (size_t)0,
+                                    as_kernel);
             }
 
             catch (...)
             {
                 #pragma omp critical
                 {
                     if (!threw_exception)
@@ -357,107 +444,197 @@
     /* gather and transform the results */
     gather_sim_result< PredictionData<real_t, sparse_ix>, InputData<real_t, sparse_ix>, WorkerMemory<ImputedData<sparse_ix>> >
                      (&worker_memory, NULL,
                       &prediction_data, NULL,
                       model_outputs, model_outputs_ext,
                       tmat, rmat, n_from,
                       ntrees, assume_full_distr,
-                      standardize_dist, nthreads);
+                      standardize_dist, as_kernel, nthreads);
 
     check_interrupt_switch(ss);
     #if defined(DONT_THROW_ON_INTERRUPT)
     if (interrupt_switch) return;
     #endif
 }
 
 template <class PredictionData>
 void traverse_tree_sim(WorkerForSimilarity   &workspace,
                        PredictionData        &prediction_data,
                        IsoForest             &model_outputs,
                        std::vector<IsoTree>  &trees,
-                       size_t                curr_tree)
+                       size_t                curr_tree,
+                       const bool            as_kernel)
 {
     if (interrupt_switch)
         return;
 
     if (workspace.st == workspace.end)
         return;
 
-    if (!workspace.tmat_sep.size())
+    if (workspace.tmat_sep.empty())
     {
         std::sort(workspace.ix_arr.begin() + workspace.st, workspace.ix_arr.begin() + workspace.end + 1);
         if (workspace.ix_arr[workspace.st] >= workspace.n_from)
             return;
         if (workspace.ix_arr[workspace.end] < workspace.n_from)
             return;
     }
 
     /* Note: the first separation step will not be added here, as it simply consists of adding +1
        to every combination regardless. It has to be added at the end in 'gather_sim_result' to
        obtain the average separation depth. */
     if (trees[curr_tree].tree_left == 0)
     {
         ldouble_safe rem = (ldouble_safe) trees[curr_tree].remainder;
-        if (!workspace.weights_arr.size())
+        if (workspace.weights_arr.empty())
         {
-            rem += (ldouble_safe)(workspace.end - workspace.st + 1);
-            if (workspace.tmat_sep.size())
-                increase_comb_counter(workspace.ix_arr.data(), workspace.st, workspace.end,
-                                      prediction_data.nrows, workspace.tmat_sep.data(),
-                                      workspace.assume_full_distr? 3. : expected_separation_depth(rem));
+            if (!as_kernel)
+            {
+                rem += (ldouble_safe)(workspace.end - workspace.st + 1);
+                if (!workspace.tmat_sep.empty())
+                    increase_comb_counter(workspace.ix_arr.data(), workspace.st, workspace.end,
+                                          prediction_data.nrows, workspace.tmat_sep.data(),
+                                          workspace.assume_full_distr? 3. : expected_separation_depth(rem));
+                else if (!workspace.rmat.empty())
+                    increase_comb_counter_in_groups(workspace.ix_arr.data(), workspace.st, workspace.end,
+                                                    workspace.n_from, prediction_data.nrows, workspace.rmat.data(),
+                                                    workspace.assume_full_distr? 3. : expected_separation_depth(rem));
+            }
+
             else
-                increase_comb_counter_in_groups(workspace.ix_arr.data(), workspace.st, workspace.end,
-                                                workspace.n_from, prediction_data.nrows, workspace.rmat.data(),
-                                                workspace.assume_full_distr? 3. : expected_separation_depth(rem));
+            {
+                if (!workspace.tmat_sep.empty())
+                {
+                    size_t i_, j_;
+                    for (size_t i = workspace.st; i < workspace.end; i++)
+                    {
+                        i_ = workspace.ix_arr[i];
+                        for (size_t j = i + 1; j <= workspace.end; j++)
+                        {
+                            j_ = workspace.ix_arr[j];
+                            workspace.tmat_sep[ix_comb(i_, j_, prediction_data.nrows, workspace.tmat_sep.size())]++;
+                        }
+                    }
+                }
+
+                else if (!workspace.rmat.empty())
+                {
+                    size_t n_group = std::distance(workspace.ix_arr.begin() + workspace.st,
+                                                   std::lower_bound(workspace.ix_arr.begin() + workspace.st,
+                                                                    workspace.ix_arr.begin() + workspace.end + 1,
+                                                                    workspace.n_from));
+                    double *restrict rmat_this;
+                    for (size_t i = workspace.st; i < workspace.st + n_group; i++)
+                    {
+                        rmat_this = workspace.rmat.data() + workspace.ix_arr[i]*workspace.n_from;
+                        for (size_t j = workspace.st + n_group; j <= workspace.end; j++)
+                        {
+                            rmat_this[workspace.ix_arr[j] - workspace.n_from]++;
+                        }
+                    }
+                }
+            }
         }
 
         else
         {
-            if (!workspace.assume_full_distr)
+            if (!as_kernel)
             {
-                rem += std::accumulate(workspace.ix_arr.begin() + workspace.st,
-                                       workspace.ix_arr.begin() + workspace.end,
-                                       (ldouble_safe) 0.,
-                                       [&workspace](ldouble_safe curr, size_t ix)
-                                                      {return curr + (ldouble_safe)workspace.weights_arr[ix];}
-                                      );
+                if (!workspace.assume_full_distr)
+                {
+                    rem += std::accumulate(workspace.ix_arr.begin() + workspace.st,
+                                           workspace.ix_arr.begin() + workspace.end,
+                                           (ldouble_safe) 0.,
+                                           [&workspace](ldouble_safe curr, size_t ix)
+                                           {return curr + (ldouble_safe)workspace.weights_arr[ix];}
+                                          );
+                }
+
+                if (!workspace.tmat_sep.empty())
+                    increase_comb_counter(workspace.ix_arr.data(), workspace.st, workspace.end,
+                                          prediction_data.nrows, workspace.tmat_sep.data(),
+                                          workspace.weights_arr.data(),
+                                          workspace.assume_full_distr? 3. : expected_separation_depth(rem));
+                else if (!workspace.rmat.empty())
+                    increase_comb_counter_in_groups(workspace.ix_arr.data(), workspace.st, workspace.end,
+                                                    workspace.n_from, prediction_data.nrows,
+                                                    workspace.rmat.data(), workspace.weights_arr.data(),
+                                                    workspace.assume_full_distr? 3. : expected_separation_depth(rem));
             }
 
-            if (workspace.tmat_sep.size())
-                increase_comb_counter(workspace.ix_arr.data(), workspace.st, workspace.end,
-                                      prediction_data.nrows, workspace.tmat_sep.data(),
-                                      workspace.weights_arr.data(),
-                                      workspace.assume_full_distr? 3. : expected_separation_depth(rem));
             else
-                increase_comb_counter_in_groups(workspace.ix_arr.data(), workspace.st, workspace.end,
-                                                workspace.n_from, prediction_data.nrows,
-                                                workspace.rmat.data(), workspace.weights_arr.data(),
-                                                workspace.assume_full_distr? 3. : expected_separation_depth(rem));
+            {
+                if (!workspace.tmat_sep.empty())
+                {
+                    size_t i_, j_;
+                    double w_this;
+                    for (size_t i = workspace.st; i < workspace.end; i++)
+                    {
+                        i_ = workspace.ix_arr[i];
+                        w_this = workspace.weights_arr[i_];
+                        for (size_t j = i + 1; j <= workspace.end; j++)
+                        {
+                            j_ = workspace.ix_arr[j];
+                            workspace.tmat_sep[ix_comb(i_, j_, prediction_data.nrows, workspace.tmat_sep.size())]
+                                +=
+                            w_this * workspace.weights_arr[j_];
+                        }
+                    }
+                }
+
+                else if (!workspace.rmat.empty())
+                {
+                    size_t n_group = std::distance(workspace.ix_arr.begin() + workspace.st,
+                                                   std::lower_bound(workspace.ix_arr.begin() + workspace.st,
+                                                                    workspace.ix_arr.begin() + workspace.end + 1,
+                                                                    workspace.n_from));
+                    double *restrict rmat_this;
+                    double w_this;
+                    size_t i_, j_;
+                    for (size_t i = workspace.st; i < workspace.st + n_group; i++)
+                    {
+                        i_ = workspace.ix_arr[i];
+                        rmat_this = workspace.rmat.data() + i_*workspace.n_from;
+                        w_this = workspace.weights_arr[i_];
+                        for (size_t j = workspace.st + n_group; j <= workspace.end; j++)
+                        {
+                            j_ = workspace.ix_arr[j];
+                            rmat_this[j_ - workspace.n_from]
+                                +=
+                            w_this * workspace.weights_arr[j_];
+                        }
+                    }
+                }
+            }
         }
         return;
     }
 
-    else if (curr_tree > 0)
+    else if (curr_tree > 0 && !as_kernel)
     {
-        if (workspace.tmat_sep.size())
-            if (!workspace.weights_arr.size())
+        if (!workspace.tmat_sep.empty())
+        {
+            if (workspace.weights_arr.empty())
                 increase_comb_counter(workspace.ix_arr.data(), workspace.st, workspace.end,
                                       prediction_data.nrows, workspace.tmat_sep.data(), -1.);
             else
                 increase_comb_counter(workspace.ix_arr.data(), workspace.st, workspace.end,
                                       prediction_data.nrows, workspace.tmat_sep.data(),
                                       workspace.weights_arr.data(), -1.);
-        else
-            if (!workspace.weights_arr.size())
+        }
+        else if (!workspace.rmat.empty())
+        {
+            if (workspace.weights_arr.empty())
                 increase_comb_counter_in_groups(workspace.ix_arr.data(), workspace.st, workspace.end,
                                                 workspace.n_from, prediction_data.nrows, workspace.rmat.data(), -1.);
             else
                 increase_comb_counter_in_groups(workspace.ix_arr.data(), workspace.st, workspace.end,
                                                 workspace.n_from, prediction_data.nrows,
                                                 workspace.rmat.data(), workspace.weights_arr.data(), -1.);
+        }
     }
 
 
     /* divide according to tree */
     if (prediction_data.Xc_indptr != NULL && !workspace.tmat_sep.empty())
         std::sort(workspace.ix_arr.begin() + workspace.st, workspace.ix_arr.begin() + workspace.end + 1);
     size_t st_NA, end_NA, split_ix;
@@ -518,15 +695,15 @@
             break;
         }
     }
 
 
     /* continue splitting recursively */
     size_t orig_end = workspace.end;
-    if (model_outputs.new_cat_action == Weighted && prediction_data.categ_data != NULL) {
+    if (model_outputs.new_cat_action == Weighted && model_outputs.cat_split_type == SubSet && prediction_data.categ_data != NULL) {
         if (model_outputs.missing_action == Fail && trees[curr_tree].col_type == Numeric) {
             st_NA = split_ix;
             end_NA = split_ix;
         }
         goto missing_action_divide;
     }
     switch (model_outputs.missing_action)
@@ -541,27 +718,29 @@
             if (split_ix > workspace.st)
             {
                 workspace.end = split_ix - 1;
                 traverse_tree_sim(workspace,
                                   prediction_data,
                                   model_outputs,
                                   trees,
-                                  trees[curr_tree].tree_left);
+                                  trees[curr_tree].tree_left,
+                                  as_kernel);
             }
 
 
             if (split_ix <= orig_end)
             {
                 workspace.st  = split_ix;
                 workspace.end = orig_end;
                 traverse_tree_sim(workspace,
                                   prediction_data,
                                   model_outputs,
                                   trees,
-                                  trees[curr_tree].tree_right);
+                                  trees[curr_tree].tree_right,
+                                  as_kernel);
             }
             break;
         }
 
         case Divide: /* new_cat_action = 'Weighted' will also fall here */
         {
             /* TODO: this one should also have a parameter 'changed_weoghts' like during fitting */
@@ -583,22 +762,23 @@
                 workspace.end = end_NA - 1;
                 for (size_t row = st_NA; row < end_NA; row++)
                     workspace.weights_arr[workspace.ix_arr[row]] *= trees[curr_tree].pct_tree_left;
                 traverse_tree_sim(workspace,
                                   prediction_data,
                                   model_outputs,
                                   trees,
-                                  trees[curr_tree].tree_left);
+                                  trees[curr_tree].tree_left,
+                                  as_kernel);
             }
 
             if (st_NA <= orig_end)
             {
                 workspace.st = st_NA;
                 workspace.end = orig_end;
-                if (weights_arr.size())
+                if (!weights_arr.empty())
                 {
                     std::copy(weights_arr.begin(),
                               weights_arr.end(),
                               workspace.weights_arr.begin());
                     std::copy(ix_arr.begin(),
                               ix_arr.end(),
                               workspace.ix_arr.begin());
@@ -610,71 +790,110 @@
 
                 for (size_t row = st_NA; row < end_NA; row++)
                     workspace.weights_arr[workspace.ix_arr[row]] *= (1. - trees[curr_tree].pct_tree_left);
                 traverse_tree_sim(workspace,
                                   prediction_data,
                                   model_outputs,
                                   trees,
-                                  trees[curr_tree].tree_right);
+                                  trees[curr_tree].tree_right,
+                                  as_kernel);
             }
             break;
         }
     }
 }
 
 template <class PredictionData>
 void traverse_hplane_sim(WorkerForSimilarity     &workspace,
                          PredictionData          &prediction_data,
                          ExtIsoForest            &model_outputs,
                          std::vector<IsoHPlane>  &hplanes,
-                         size_t                  curr_tree)
+                         size_t                  curr_tree,
+                         const bool              as_kernel)
 {
     if (interrupt_switch)
         return;
     
     if (workspace.st == workspace.end)
         return;
 
-    if (!workspace.tmat_sep.size())
+    if (workspace.tmat_sep.empty())
     {
         std::sort(workspace.ix_arr.begin() + workspace.st, workspace.ix_arr.begin() + workspace.end + 1);
         if (workspace.ix_arr[workspace.st] >= workspace.n_from)
             return;
         if (workspace.ix_arr[workspace.end] < workspace.n_from)
             return;
     }
 
     /* Note: the first separation step will not be added here, as it simply consists of adding +1
        to every combination regardless. It has to be added at the end in 'gather_sim_result' to
        obtain the average separation depth. */
     if (hplanes[curr_tree].hplane_left == 0)
     {
-        if (workspace.tmat_sep.size())
-            increase_comb_counter(workspace.ix_arr.data(), workspace.st, workspace.end,
-                                  prediction_data.nrows, workspace.tmat_sep.data(),
-                                  workspace.assume_full_distr? 3. : 
-                                  expected_separation_depth((ldouble_safe) hplanes[curr_tree].remainder
-                                                              + (ldouble_safe)(workspace.end - workspace.st + 1))
-                                  );
+        if (!as_kernel)
+        {
+            if (!workspace.tmat_sep.empty())
+                increase_comb_counter(workspace.ix_arr.data(), workspace.st, workspace.end,
+                                      prediction_data.nrows, workspace.tmat_sep.data(),
+                                      workspace.assume_full_distr? 3. : 
+                                      expected_separation_depth((ldouble_safe) hplanes[curr_tree].remainder
+                                                                  + (ldouble_safe)(workspace.end - workspace.st + 1))
+                                      );
+            else if (!workspace.rmat.empty())
+                increase_comb_counter_in_groups(workspace.ix_arr.data(), workspace.st, workspace.end, workspace.n_from,
+                                                prediction_data.nrows, workspace.rmat.data(),
+                                                workspace.assume_full_distr? 3. : 
+                                                expected_separation_depth((ldouble_safe) hplanes[curr_tree].remainder
+                                                                            + (ldouble_safe)(workspace.end - workspace.st + 1))
+                                                );
+        }
+
         else
-            increase_comb_counter_in_groups(workspace.ix_arr.data(), workspace.st, workspace.end, workspace.n_from,
-                                            prediction_data.nrows, workspace.rmat.data(),
-                                            workspace.assume_full_distr? 3. : 
-                                            expected_separation_depth((ldouble_safe) hplanes[curr_tree].remainder
-                                                                        + (ldouble_safe)(workspace.end - workspace.st + 1))
-                                            );
+        {
+            if (!workspace.tmat_sep.empty())
+            {
+                size_t i_, j_;
+                for (size_t i = workspace.st; i < workspace.end; i++)
+                {
+                    i_ = workspace.ix_arr[i];
+                    for (size_t j = i + 1; j <= workspace.end; j++)
+                    {
+                        j_ = workspace.ix_arr[j];
+                        workspace.tmat_sep[ix_comb(i_, j_, prediction_data.nrows, workspace.tmat_sep.size())]++;
+                    }
+                }
+            }
+
+            else if (!workspace.rmat.empty())
+            {
+                size_t n_group = std::distance(workspace.ix_arr.begin() + workspace.st,
+                                               std::lower_bound(workspace.ix_arr.begin() + workspace.st,
+                                                                workspace.ix_arr.begin() + workspace.end + 1,
+                                                                workspace.n_from));
+                double *restrict rmat_this;
+                for (size_t i = workspace.st; i < workspace.st + n_group; i++)
+                {
+                    rmat_this = workspace.rmat.data() + workspace.ix_arr[i]*workspace.n_from;
+                    for (size_t j = workspace.st + n_group; j <= workspace.end; j++)
+                    {
+                        rmat_this[workspace.ix_arr[j] - workspace.n_from]++;
+                    }
+                }
+            }
+        }
         return;
     }
 
-    else if (curr_tree > 0)
+    else if (curr_tree > 0 && !as_kernel)
     {
-        if (workspace.tmat_sep.size())
+        if (!workspace.tmat_sep.empty())
             increase_comb_counter(workspace.ix_arr.data(), workspace.st, workspace.end,
                                   prediction_data.nrows, workspace.tmat_sep.data(), -1.);
-        else
+        else if (!workspace.rmat.empty())
             increase_comb_counter_in_groups(workspace.ix_arr.data(), workspace.st, workspace.end, workspace.n_from,
                                             prediction_data.nrows, workspace.rmat.data(), -1.);
     }
 
     if (prediction_data.Xc_indptr != NULL && workspace.tmat_sep.size())
         std::sort(workspace.ix_arr.begin() + workspace.st, workspace.ix_arr.begin() + workspace.end + 1);
 
@@ -769,38 +988,40 @@
     if (split_ix > workspace.st)
     {
         workspace.end = split_ix - 1;
         traverse_hplane_sim(workspace,
                             prediction_data,
                             model_outputs,
                             hplanes,
-                            hplanes[curr_tree].hplane_left);
+                            hplanes[curr_tree].hplane_left,
+                            as_kernel);
     }
 
     if (split_ix <= orig_end)
     {
         workspace.st  = split_ix;
         workspace.end = orig_end;
         traverse_hplane_sim(workspace,
                             prediction_data,
                             model_outputs,
                             hplanes,
-                            hplanes[curr_tree].hplane_right);
+                            hplanes[curr_tree].hplane_right,
+                            as_kernel);
     }
 
 }
 
 template <class PredictionData, class InputData, class WorkerMemory>
 void gather_sim_result(std::vector<WorkerForSimilarity> *worker_memory,
                        std::vector<WorkerMemory> *worker_memory_m,
                        PredictionData *prediction_data, InputData *input_data,
                        IsoForest *model_outputs, ExtIsoForest *model_outputs_ext,
                        double *restrict tmat, double *restrict rmat, size_t n_from,
                        size_t ntrees, bool assume_full_distr,
-                       bool standardize_dist, int nthreads)
+                       bool standardize_dist, bool as_kernel, int nthreads)
 {
     if (interrupt_switch)
         return;
 
     size_t nrows = (prediction_data != NULL)? prediction_data->nrows : input_data->nrows;
     size_t ncomb = calc_ncomb(nrows);
     size_t n_to  = (prediction_data != NULL)? (prediction_data->nrows - n_from) : 0;
@@ -808,34 +1029,34 @@
     #ifdef _OPENMP
     if (nthreads > 1)
     {
         if (worker_memory != NULL)
         {
             for (WorkerForSimilarity &w : *worker_memory)
             {
-                if (w.tmat_sep.size())
+                if (!w.tmat_sep.empty())
                 {
                     #pragma omp parallel for schedule(static) num_threads(nthreads) shared(ncomb, tmat, w, worker_memory)
                     for (size_t_for ix = 0; ix < (decltype(ix))ncomb; ix++)
                         tmat[ix] += w.tmat_sep[ix];
                 }
-                else if (w.rmat.size())
+                else if (!w.rmat.empty())
                 {
                     #pragma omp parallel for schedule(static) num_threads(nthreads) shared(rmat, w, worker_memory)
                     for (size_t_for ix = 0; ix < (decltype(ix))w.rmat.size(); ix++)
                         rmat[ix] += w.rmat[ix];
                 }
             }
         }
 
         else
         {
             for (WorkerMemory &w : *worker_memory_m)
             {
-                if (w.tmat_sep.size())
+                if (!w.tmat_sep.empty())
                 {
                     #pragma omp parallel for schedule(static) num_threads(nthreads) shared(ncomb, tmat, w, worker_memory_m)
                     for (size_t_for ix = 0; ix < (decltype(ix))ncomb; ix++)
                         tmat[ix] += w.tmat_sep[ix];
                 }
             }
         }
@@ -857,14 +1078,26 @@
             std::copy((*worker_memory_m)[0].tmat_sep.begin(), (*worker_memory_m)[0].tmat_sep.end(), tmat);
         }
     }
 
     double ntrees_dbl = (double) ntrees;
     if (standardize_dist)
     {
+        if (as_kernel)
+        {
+            if (tmat != NULL)
+                for (size_t ix = 0; ix < ncomb; ix++)
+                    tmat[ix] /= ntrees_dbl;
+            else
+                for (size_t ix = 0; ix < (n_from * n_to); ix++)
+                    rmat[ix] /= ntrees_dbl;
+            return;
+        }
+
+
         /* Note: the separation distances up this point are missing the first hop, which is always
            a +1 to every combination. Thus, it needs to be added back for the average separation depth.
            For the standardized metric, it takes the expected divisor as 2(=3-1) instead of 3, given
            that every combination will always get a +1 at the beginning. Since what's obtained here
            is a sum across all trees, adding this +1 means adding the number of trees. */
         double div_trees = ntrees_dbl;
         if (assume_full_distr)
@@ -904,14 +1137,16 @@
             #endif
             for (size_t ix = 0; ix < (n_from * n_to); ix++)
                 rmat[ix] = std::exp2( - rmat[ix] / div_trees);
     }
     
     else
     {
+        if (as_kernel) return;
+
         if (tmat != NULL)
             #ifndef _WIN32
             #pragma omp simd
             #endif
             for (size_t ix = 0; ix < ncomb; ix++)
                 tmat[ix] = (tmat[ix] + ntrees) / ntrees_dbl;
         else
@@ -944,15 +1179,15 @@
             workspace.tmat_sep.resize(calc_ncomb(prediction_data.nrows), 0);
         else
             workspace.rmat.resize((prediction_data.nrows - n_from) * n_from, 0);
     }
 
     if (model_outputs != NULL &&
         (model_outputs->missing_action == Divide ||
-         (model_outputs->new_cat_action == Weighted && prediction_data.categ_data != NULL)))
+         (model_outputs->new_cat_action == Weighted && model_outputs->cat_split_type == SubSet && prediction_data.categ_data != NULL)))
     {
         if (workspace.weights_arr.empty())
             workspace.weights_arr.resize(prediction_data.nrows, 1.);
         else
             std::fill(workspace.weights_arr.begin(), workspace.weights_arr.end(), 1.);
     }
 
@@ -972,14 +1207,15 @@
     real_t *restrict Xc, sparse_ix *restrict Xc_ind, sparse_ix *restrict Xc_indptr,
     size_t nrows, int nthreads, bool assume_full_distr, bool standardize_dist,
     IsoForest *model_outputs, ExtIsoForest *model_outputs_ext,
     double *restrict tmat, double *restrict rmat, size_t n_from,
     TreesIndexer *indexer, bool is_col_major, size_t ld_numeric, size_t ld_categ
 )
 {
+    SignalSwitcher ss;
     size_t ntrees = (model_outputs != NULL)? model_outputs->trees.size() : model_outputs_ext->hplanes.size();
     std::vector<sparse_ix> terminal_indices(nrows * ntrees);
     std::unique_ptr<double[]> ignored(new double[nrows]);
     predict_iforest(numeric_data, categ_data,
                     is_col_major, ld_numeric, ld_categ,
                     is_col_major? Xc : nullptr, is_col_major? Xc_ind : nullptr, is_col_major? Xc_indptr : nullptr,
                     is_col_major? (real_t*)nullptr : Xc, is_col_major? (sparse_ix*)nullptr : Xc_ind, is_col_major? (sparse_ix*)nullptr : Xc_indptr,
@@ -990,15 +1226,15 @@
                     indexer);
     ignored.reset();
 
     #ifndef _OPENMP
     nthreads = 1;
     #endif
 
-    SignalSwitcher ss;
+    check_interrupt_switch(ss);
 
     if (n_from == 0)
     {
         size_t ncomb = calc_ncomb(nrows);
         std::fill_n(tmat, ncomb, 0.);
 
         std::vector<std::vector<double>> sum_separations(nthreads);
@@ -1019,15 +1255,15 @@
                 shared(model_outputs, model_outputs_ext, nthreads, indexer, nrows, ncomb, terminal_indices, \
                        sum_separations, thread_argsorted_nodes, thread_sorted_nodes, tmat, \
                        threw_exception, ex)
         for (size_t_for tree = 0; tree < (decltype(tree))ntrees; tree++)
         {
             if (interrupt_switch || threw_exception) continue;
 
-            if (indexer->indices[tree].n_terminal <= 1)
+            if (unlikely(indexer->indices[tree].n_terminal <= 1))
             {
                 for (auto &el : sum_separations[omp_get_thread_num()]) el += 1.;
                 continue;
             }
 
             double *restrict ptr_this_sep = sum_separations[omp_get_thread_num()].data();
             if (nthreads == 1) ptr_this_sep = tmat;
@@ -1045,15 +1281,15 @@
             {
                 for (size_t el1 = 0; el1 < nrows-1; el1++)
                 {
                     i = terminal_indices_this[el1];
                     for (size_t el2 = el1+1; el2 < nrows; el2++)
                     {
                         j = terminal_indices_this[el2];
-                        if (i == j)
+                        if (unlikely(i == j))
                             add_round = node_depths_this[i] + 3.;
                         else
                             add_round = node_dist_this[ix_comb(i, j, n_terminal_this, ncomb_this)];
                         ptr_this_sep[ix_comb(el1, el2, nrows, ncomb)] += add_round;
                     }
                 }
             }
@@ -1066,15 +1302,15 @@
                     nodes_w_repeated.reserve(n_terminal_this);
                     for (size_t el1 = 0; el1 < nrows-1; el1++)
                     {
                         i = terminal_indices_this[el1];
                         for (size_t el2 = el1+1; el2 < nrows; el2++)
                         {
                             j = terminal_indices_this[el2];
-                            if (i == j)
+                            if (unlikely(i == j))
                                 nodes_w_repeated.insert(i);
                             else
                                 ptr_this_sep[ix_comb(el1, el2, nrows, ncomb)]
                                     +=
                                 node_dist_this[ix_comb(i, j, n_terminal_this, ncomb_this)];
                         }
                     }
@@ -1088,15 +1324,15 @@
                         {
                             threw_exception = true;
                             ex = std::current_exception();
                         }
                     }
                 }
 
-                if (!nodes_w_repeated.empty())
+                if (likely(!nodes_w_repeated.empty()))
                 {
                     std::vector<size_t> *restrict argsorted_nodes = &thread_argsorted_nodes[omp_get_thread_num()];
                     std::iota(argsorted_nodes->begin(), argsorted_nodes->end(), (size_t)0);
                     std::sort(argsorted_nodes->begin(), argsorted_nodes->end(),
                               [&terminal_indices_this](const size_t a, const size_t b)
                               {return terminal_indices_this[a] < terminal_indices_this[b];});
                     std::vector<size_t>::iterator curr_begin = argsorted_nodes->begin();
@@ -1231,15 +1467,15 @@
                 shared(model_outputs, model_outputs_ext, nthreads, indexer, nrows, ncomb, terminal_indices, \
                        sum_separations, thread_argsorted_nodes, thread_sorted_nodes, thread_doubly_argsorted, rmat, n_to, n_from, \
                        threw_exception, ex)
         for (size_t_for tree = 0; tree < (decltype(tree))ntrees; tree++)
         {
             if (interrupt_switch || threw_exception) continue;
 
-            if (indexer->indices[tree].n_terminal <= 1)
+            if (unlikely(indexer->indices[tree].n_terminal <= 1))
             {
                 for (auto &el : sum_separations[omp_get_thread_num()]) el += 1.;
                 continue;
             }
 
             double *restrict ptr_this_sep = sum_separations[omp_get_thread_num()].data();
             if (nthreads == 1) ptr_this_sep = rmat;
@@ -1258,15 +1494,15 @@
                 for (size_t el1 = 0; el1 < n_from; el1++)
                 {
                     i = terminal_indices_this[el1];
                     double *ptr_this_sep_ = ptr_this_sep + el1*n_to;
                     for (size_t el2 = n_from; el2 < nrows; el2++)
                     {
                         j = terminal_indices_this[el2];
-                        if (i == j)
+                        if (unlikely(i == j))
                             add_round = node_depths_this[i] + 3.;
                         else
                             add_round = node_dist_this[ix_comb(i, j, n_terminal_this, ncomb_this)];
                         ptr_this_sep_[el2-n_from] += add_round;
                     }
                 }
             }
@@ -1280,24 +1516,24 @@
                     for (size_t el1 = 0; el1 < n_from; el1++)
                     {
                         i = terminal_indices_this[el1];
                         double *ptr_this_sep_ = ptr_this_sep + el1*n_to;
                         for (size_t el2 = n_from; el2 < nrows; el2++)
                         {
                             j = terminal_indices_this[el2];
-                            if (i == j)
+                            if (unlikely(i == j))
                                 nodes_w_repeated.insert(i);
                             else
                                 ptr_this_sep_[el2-n_from]
                                     +=
                                 node_dist_this[ix_comb(i, j, n_terminal_this, ncomb_this)];
                         }
                     }
 
-                    if (!nodes_w_repeated.empty())
+                    if (likely(!nodes_w_repeated.empty()))
                     {
                         std::vector<size_t> *restrict argsorted_nodes = &thread_argsorted_nodes[omp_get_thread_num()];
                         std::iota(argsorted_nodes->begin(), argsorted_nodes->end(), (size_t)0);
                         std::sort(argsorted_nodes->begin(), argsorted_nodes->end(),
                                   [&terminal_indices_this](const size_t a, const size_t b)
                                   {return terminal_indices_this[a] < terminal_indices_this[b];});
                         std::vector<size_t>::iterator curr_begin = argsorted_nodes->begin();
@@ -1313,15 +1549,15 @@
                                                           [&terminal_indices_this](const size_t &a, const size_t &b)
                                                           {return (size_t)terminal_indices_this[a] < b;});
                             new_begin =  std::upper_bound(curr_begin, argsorted_nodes->end(),
                                                           node_ix,
                                                           [&terminal_indices_this](const size_t &a, const size_t &b)
                                                           {return a < (size_t)terminal_indices_this[b];});
                             size_t n_this = std::distance(curr_begin, new_begin);
-                            if (!n_this) unexpected_error();
+                            if (unlikely(!n_this)) unexpected_error();
                             ldouble_safe sep_this
                                 =
                             n_this
                                 +
                             ((tree_this != NULL)?
                              (*tree_this)[node_ix].remainder
                                 :
@@ -1424,7 +1660,170 @@
             for (size_t ix = 0; ix < ncomb; ix++)
                 rmat[ix] /= divisor;
         }
 
         check_interrupt_switch(ss);
     }
 }
+
+template <class real_t, class sparse_ix>
+void calc_similarity_from_indexer_with_references
+(
+    real_t *restrict numeric_data, int *restrict categ_data,
+    real_t *restrict Xc, sparse_ix *restrict Xc_ind, sparse_ix *restrict Xc_indptr,
+    size_t nrows, int nthreads, bool standardize_dist,
+    IsoForest *model_outputs, ExtIsoForest *model_outputs_ext,
+    double *restrict rmat,
+    TreesIndexer *indexer, bool is_col_major, size_t ld_numeric, size_t ld_categ
+)
+{
+    size_t n_ref = get_number_of_reference_points(*indexer);
+    if (unlikely(!n_ref)) unexpected_error();
+
+    SignalSwitcher ss;
+
+    size_t ntrees = (model_outputs != NULL)? model_outputs->trees.size() : model_outputs_ext->hplanes.size();
+    std::vector<sparse_ix> terminal_indices(nrows * ntrees);
+    std::unique_ptr<double[]> ignored(new double[nrows]);
+    predict_iforest(numeric_data, categ_data,
+                    is_col_major, ld_numeric, ld_categ,
+                    is_col_major? Xc : nullptr, is_col_major? Xc_ind : nullptr, is_col_major? Xc_indptr : nullptr,
+                    is_col_major? (real_t*)nullptr : Xc, is_col_major? (sparse_ix*)nullptr : Xc_ind, is_col_major? (sparse_ix*)nullptr : Xc_indptr,
+                    nrows, nthreads, false,
+                    model_outputs, model_outputs_ext,
+                    ignored.get(), terminal_indices.data(),
+                    (double*)NULL,
+                    indexer);
+    ignored.reset();
+
+    #ifndef _OPENMP
+    nthreads = 1;
+    #endif
+
+    check_interrupt_switch(ss);
+
+    #pragma omp parallel for schedule(static) num_threads(nthreads) \
+            shared(rmat, terminal_indices, nrows, n_ref, indexer, ntrees)
+    for (size_t_for row = 0; row < nrows; row++)
+    {
+        if (interrupt_switch) continue;
+
+        size_t i, j;
+        size_t n_terminal_this;
+        size_t ncomb_this;
+        size_t *restrict ref_this;
+        sparse_ix *restrict ind_this;
+        double *restrict node_depths_this;
+        double *restrict node_dist_this;
+        double *rmat_this = rmat + row*n_ref;
+        memset(rmat_this, 0, n_ref*sizeof(double));
+        for (size_t tree = 0; tree < ntrees; tree++)
+        {
+            ref_this = indexer->indices[tree].reference_points.data();
+            ind_this = terminal_indices.data() + tree*nrows;
+            node_depths_this = indexer->indices[tree].node_depths.data();
+            n_terminal_this = indexer->indices[tree].n_terminal;
+            node_dist_this = indexer->indices[tree].node_distances.data();
+            ncomb_this = calc_ncomb(n_terminal_this);
+            for (size_t ref = 0; ref < n_ref; ref++)
+            {
+                i = ind_this[row];
+                j = ref_this[ref];
+
+                if (unlikely(i == j))
+                    rmat_this[ref] += node_depths_this[i] + 3.;
+                else
+                    rmat_this[ref] += node_dist_this[ix_comb(i, j, n_terminal_this, ncomb_this)];
+            }
+        }
+    }
+
+    check_interrupt_switch(ss);
+
+    size_t size_rmat = nrows * n_ref;
+    if (standardize_dist)
+    {
+        double ntrees_dbl = (double)ntrees;
+        double div_trees = (double)(mult2(ntrees));
+        #ifndef _WIN32
+        #pragma omp simd
+        #endif
+        for (size_t ix = 0; ix < size_rmat; ix++)
+            rmat[ix] = std::exp2( - (rmat[ix] - ntrees_dbl) / div_trees);
+    }
+
+    else
+    {
+        double div_trees = (double)ntrees;
+        for (size_t ix = 0; ix < size_rmat; ix++)
+            rmat[ix] /= div_trees;
+    }
+
+    check_interrupt_switch(ss);
+}
+
+template <class real_t, class sparse_ix>
+void kernel_to_references(TreesIndexer &indexer,
+                          IsoForest *model_outputs, ExtIsoForest *model_outputs_ext,
+                          real_t *restrict numeric_data, int *restrict categ_data,
+                          real_t *restrict Xc, sparse_ix *restrict Xc_ind, sparse_ix *restrict Xc_indptr,
+                          bool is_col_major, size_t ld_numeric, size_t ld_categ,
+                          size_t nrows, int nthreads,
+                          double *restrict rmat,
+                          bool standardize)
+{
+    size_t ntrees = indexer.indices.size();
+    size_t n_ref = indexer.indices.front().reference_points.size();
+
+    SignalSwitcher ss;
+
+    std::unique_ptr<sparse_ix[]> terminal_indices(new sparse_ix[nrows*ntrees]);
+    std::unique_ptr<double[]> ignored(new double[nrows]);
+    predict_iforest(numeric_data, categ_data,
+                    is_col_major, ld_numeric, ld_categ,
+                    is_col_major? Xc : nullptr, is_col_major? Xc_ind : nullptr, is_col_major? Xc_indptr : nullptr,
+                    is_col_major? (real_t*)nullptr : Xc, is_col_major? (sparse_ix*)nullptr : Xc_ind, is_col_major? (sparse_ix*)nullptr : Xc_indptr,
+                    nrows, nthreads, false,
+                    model_outputs, model_outputs_ext,
+                    ignored.get(), terminal_indices.get(),
+                    (double*)NULL,
+                    &indexer);
+    ignored.reset();
+
+    check_interrupt_switch(ss);
+
+    #pragma omp parallel for schedule(static) num_threads(nthreads) \
+            shared(indexer, terminal_indices, nrows, ntrees, n_ref, rmat)
+    for (size_t_for row = 0; row < nrows; row++)
+    {
+        if (interrupt_switch) continue;
+
+        SingleTreeIndex *restrict index_node;
+        size_t idx_this;
+        sparse_ix *restrict terminal_indices_this = terminal_indices.get() + row;
+        double *restrict rmat_this = rmat + row*n_ref;
+        memset(rmat_this, 0, n_ref*sizeof(double));
+
+        for (size_t tree = 0; tree < ntrees; tree++)
+        {
+            idx_this = terminal_indices_this[tree*nrows];
+            index_node = &indexer.indices[tree];
+            for (size_t ind = index_node->reference_indptr[idx_this];
+                 ind < index_node->reference_indptr[idx_this + 1];
+                 ind++)
+            {
+                rmat_this[index_node->reference_mapping[ind]]++;
+            }
+        }
+    }
+
+    check_interrupt_switch(ss);
+
+    if (standardize)
+    {
+        double ntrees_dbl = (double)ntrees;
+        for (size_t ix = 0; ix < nrows*n_ref; ix++)
+            rmat[ix] /= ntrees_dbl;
+    }
+
+    check_interrupt_switch(ss);
+}
```

### Comparing `isotree-0.5.8.post1/src/extended.hpp` & `isotree-0.5.9/src/extended.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 *          arXiv preprint arXiv:2110.13402 (2021).
 *     [12] Guha, Sudipto, et al.
 *          "Robust random cut forest based anomaly detection on streams."
 *          International conference on machine learning. PMLR, 2016.
 *     [13] Cortes, David.
 *          "Isolation forests: looking beyond tree depth."
 *          arXiv preprint arXiv:2111.11639 (2021).
+*     [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou.
+*          "Isolation kernel and its effect on SVM"
+*          Proceedings of the 24th ACM SIGKDD
+*          International Conference on Knowledge Discovery & Data Mining. 2018.
 * 
 *     BSD 2-Clause License
 *     Copyright (c) 2019-2022, David Cortes
 *     All rights reserved.
 *     Redistribution and use in source and binary forms, with or without
 *     modification, are permitted provided that the following conditions are met:
 *     * Redistributions of source code must retain the above copyright notice, this
```

### Comparing `isotree-0.5.8.post1/src/fit_model.hpp` & `isotree-0.5.9/src/fit_model.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 *          arXiv preprint arXiv:2110.13402 (2021).
 *     [12] Guha, Sudipto, et al.
 *          "Robust random cut forest based anomaly detection on streams."
 *          International conference on machine learning. PMLR, 2016.
 *     [13] Cortes, David.
 *          "Isolation forests: looking beyond tree depth."
 *          arXiv preprint arXiv:2111.11639 (2021).
+*     [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou.
+*          "Isolation kernel and its effect on SVM"
+*          Proceedings of the 24th ACM SIGKDD
+*          International Conference on Knowledge Discovery & Data Mining. 2018.
 * 
 *     BSD 2-Clause License
 *     Copyright (c) 2019-2022, David Cortes
 *     All rights reserved.
 *     Redistribution and use in source and binary forms, with or without
 *     modification, are permitted provided that the following conditions are met:
 *     * Redistributions of source code must retain the above copyright notice, this
@@ -947,15 +951,15 @@
     if (calc_dist)
         gather_sim_result< PredictionData<real_t, sparse_ix>, InputData<real_t, sparse_ix> >
                          (NULL, &worker_memory,
                           NULL, &input_data,
                           model_outputs, model_outputs_ext,
                           tmat, NULL, 0,
                           model_params.ntrees, false,
-                          standardize_dist, nthreads);
+                          standardize_dist, false, nthreads);
 
     check_interrupt_switch(ss);
     #if defined(DONT_THROW_ON_INTERRUPT)
     if (interrupt_switch) return EXIT_FAILURE;
     #endif
 
     /* same for depths */
@@ -1040,40 +1044,40 @@
 *       'model_outputs' and 'model_outputs_ext'. Note that this function is not thread-safe,
 *       so it cannot be run in parallel for the same model object.
 * - model_outputs_ext
 *       Pointer to fitted extended model object from function 'fit_iforest'. Pass NULL
 *       if the trees are are to be added to an single-variable model. Can only pass one of
 *       'model_outputs' and 'model_outputs_ext'. Note that this function is not thread-safe,
 *       so it cannot be run in parallel for the same model object.
-* - numeric_data
+* - numeric_data[nrows * ncols_numeric]
 *       Pointer to numeric data to which to fit this additional tree. Must be ordered by columns like Fortran,
 *       not ordered by rows like C (i.e. entries 1..n contain column 0, n+1..2n column 1, etc.).
 *       Pass NULL if there are no dense numeric columns.
 *       Can only pass one of 'numeric_data' or 'Xc' + 'Xc_ind' + 'Xc_indptr'.
 *       If the model from 'fit_iforest' was fit to numeric data, must pass numeric data with the same number
 *       of columns, either as dense or as sparse arrays.
 * - ncols_numeric
 *       Same parameter as for 'fit_iforest' (see the documentation in there for details). Cannot be changed from
 *       what was originally passed to 'fit_iforest'.
-* - categ_data
+* - categ_data[nrows * ncols_categ]
 *       Pointer to categorical data to which to fit this additional tree. Must be ordered by columns like Fortran,
 *       not ordered by rows like C (i.e. entries 1..n contain column 0, n+1..2n column 1, etc.).
 *       Pass NULL if there are no categorical columns. The encoding must be the same as was used
 *       in the data to which the model was fit.
 *       Each category should be represented as an integer, and these integers must start at zero and
 *       be in consecutive order - i.e. if category '3' is present, category '2' must have also been
 *       present when the model was fit (note that they are not treated as being ordinal, this is just
 *       an encoding). Missing values should be encoded as negative numbers such as (-1). The encoding
 *       must be the same as was used in the data to which the model was fit.
 *       If the model from 'fit_iforest' was fit to categorical data, must pass categorical data with the same number
 *       of columns and the same category encoding.
 * - ncols_categ
 *       Same parameter as for 'fit_iforest' (see the documentation in there for details). Cannot be changed from
 *       what was originally passed to 'fit_iforest'.
-* - ncat
+* - ncat[ncols_categ]
 *       Same parameter as for 'fit_iforest' (see the documentation in there for details). May contain new categories,
 *       but should keep the same encodings that were used for previous categories.
 * - Xc[nnz]
 *       Pointer to numeric data in sparse numeric matrix in CSC format (column-compressed).
 *       Pass NULL if there are no sparse numeric columns.
 *       Can only pass one of 'numeric_data' or 'Xc' + 'Xc_ind' + 'Xc_indptr'.
 * - Xc_ind[nnz]
@@ -1173,15 +1177,65 @@
 *       Pass NULL if the model was built without imputer.
 * - min_imp_obs
 *       Same parameter as for 'fit_iforest' (see the documentation in there for details). Can be changed from
 *       what was originally passed to 'fit_iforest'.
 * - indexer
 *       Indexer object associated to the model object ('model_outputs' or 'model_outputs_ext'), which will
 *       be updated with the new tree to add.
+*       If 'indexer' has reference points, these must be passed again here in order to index them.
 *       Pass NULL if the model has no associated indexer.
+* - ref_numeric_data[nref * ncols_numeric]
+*       Pointer to numeric data for reference points. May be ordered by rows
+*       (i.e. entries 1..n contain row 0, n+1..2n row 1, etc.) - a.k.a. row-major - or by
+*       columns (i.e. entries 1..n contain column 0, n+1..2n column 1, etc.) - a.k.a. column-major
+*       (see parameter 'ref_is_col_major').
+*       Pass NULL if there are no dense numeric columns or no reference points.
+*       Can only pass one of 'ref_numeric_data' or 'ref_Xc' + 'ref_Xc_ind' + 'ref_Xc_indptr'.
+*       If 'indexer' is passed, it has reference points, and the data to which the model was fit had
+*       numeric columns, then numeric data for reference points must be passed (in either dense or sparse format).
+* - ref_categ_data[nref * ncols_categ]
+*       Pointer to categorical data for reference points. May be ordered by rows
+*       (i.e. entries 1..n contain row 0, n+1..2n row 1, etc.) - a.k.a. row-major - or by
+*       columns (i.e. entries 1..n contain column 0, n+1..2n column 1, etc.) - a.k.a. column-major
+*       (see parameter 'ref_is_col_major').
+*       Pass NULL if there are no categorical columns or no reference points.
+*       If 'indexer' is passed, it has reference points, and the data to which the model was fit had
+*       categorical columns, then 'ref_categ_data' must be passed.
+* - ref_is_col_major
+*       Whether 'ref_numeric_data' and/or 'ref_categ_data' are in column-major order. If numeric data is
+*       passed in sparse format, categorical data must be passed in column-major format. If passing dense
+*       data, row-major format is preferred as it will be faster. If the data is passed in row-major format,
+*       must also pass 'ref_ld_numeric' and/or 'ref_ld_categ'.
+*       If both 'ref_numeric_data' and 'ref_categ_data' are passed, they must have the same orientation
+*       (row-major or column-major).
+* - ref_ld_numeric
+*       Leading dimension of the array 'ref_numeric_data', if it is passed in row-major format.
+*       Typically, this corresponds to the number of columns, but may be larger (the array will
+*       be accessed assuming that row 'n' starts at 'ref_numeric_data + n*ref_ld_numeric'). If passing
+*       'ref_numeric_data' in column-major order, this is ignored and will be assumed that the
+*       leading dimension corresponds to the number of rows. This is ignored when passing numeric
+*       data in sparse format.
+* - ref_ld_categ
+*       Leading dimension of the array 'ref_categ_data', if it is passed in row-major format.
+*       Typically, this corresponds to the number of columns, but may be larger (the array will
+*       be accessed assuming that row 'n' starts at 'ref_categ_data + n*ref_ld_categ'). If passing
+*       'ref_categ_data' in column-major order, this is ignored and will be assumed that the
+*       leading dimension corresponds to the number of rows.
+* - ref_Xc[ref_nnz]
+*       Pointer to numeric data for reference points in sparse numeric matrix in CSC format (column-compressed).
+*       Pass NULL if there are no sparse numeric columns for reference points or no reference points.
+*       Can only pass one of 'ref_numeric_data' or 'ref_Xc' + 'ref_Xc_ind' + 'ref_Xc_indptr'.
+* - ref_Xc_ind[ref_nnz]
+*       Pointer to row indices to which each non-zero entry in 'ref_Xc' corresponds.
+*       Must be in sorted order, otherwise results will be incorrect.
+*       Pass NULL if there are no sparse numeric columns in CSC format for reference points or no reference points.
+* - ref_Xc_indptr[ref_nnz]
+*       Pointer to column index pointers that tell at entry [col] where does column 'col'
+*       start and at entry [col + 1] where does column 'col' end.
+*       Pass NULL if there are no sparse numeric columns in CSC format for reference points or no reference points.
 * - random_seed
 *       Seed that will be used to generate random numbers used by the model.
 */
 template <class real_t, class sparse_ix>
 int add_tree(IsoForest *model_outputs, ExtIsoForest *model_outputs_ext,
              real_t numeric_data[],  size_t ncols_numeric,
              int    categ_data[],    size_t ncols_categ,    int ncat[],
@@ -1196,28 +1250,35 @@
              double prob_pick_col_by_range, double prob_pick_col_by_var,
              double prob_pick_col_by_kurt,
              double min_gain, MissingAction missing_action,
              CategSplit cat_split_type, NewCategAction new_cat_action,
              UseDepthImp depth_imp, WeighImpRows weigh_imp_rows,
              bool   all_perm, Imputer *imputer, size_t min_imp_obs,
              TreesIndexer *indexer,
+             real_t ref_numeric_data[], int ref_categ_data[],
+             bool ref_is_col_major, size_t ref_ld_numeric, size_t ref_ld_categ,
+             real_t ref_Xc[], sparse_ix ref_Xc_ind[], sparse_ix ref_Xc_indptr[],
              uint64_t random_seed)
 {
     if (
         prob_pick_by_gain_avg < 0 || prob_pick_by_gain_pl < 0 || prob_pick_col_by_range < 0 ||
         prob_pick_col_by_var < 0 || prob_pick_col_by_kurt < 0
     ) {
         throw std::runtime_error("Cannot pass negative probabilities.\n");
     }
     if (prob_pick_col_by_range && categ_data != NULL)
         throw std::runtime_error("'prob_pick_col_by_range' is not compatible with categorical data.\n");
     if (prob_pick_col_by_kurt && weigh_by_kurt)
         throw std::runtime_error("'weigh_by_kurt' and 'prob_pick_col_by_kurt' cannot be used together.\n");
     if (ndim == 0 && model_outputs == NULL)
         throw std::runtime_error("Must pass 'ndim>0' in the extended model.\n");
+    if (indexer != NULL && !indexer->indices.empty() && !indexer->indices.front().reference_points.empty()) {
+        if (ref_numeric_data == NULL && ref_categ_data == NULL && ref_Xc_indptr == NULL)
+            throw std::runtime_error("'indexer' has reference points. Those points must be passed to index them in the new tree to add.\n");
+    }
 
     std::vector<ImputeNode> *impute_nodes = NULL;
 
     int max_categ = 0;
     for (size_t col = 0; col < ncols_categ; col++)
         max_categ = (ncat[col] > max_categ)? ncat[col] : max_categ;
 
@@ -1343,14 +1404,64 @@
                         indexer->indices.back().n_terminal,
                         model_outputs_ext->hplanes.back()
                     );
                 }
             }
 
             check_interrupt_switch(ss);
+            if (!indexer->indices.front().reference_points.empty())
+            {
+                size_t n_ref = indexer->indices.front().reference_points.size();
+                std::vector<sparse_ix> terminal_indices(n_ref);
+                std::unique_ptr<double[]> ignored(new double[n_ref]);
+                if (model_outputs != NULL)
+                {
+                    IsoForest single_tree_model;
+                    single_tree_model.new_cat_action = model_outputs->new_cat_action;
+                    single_tree_model.cat_split_type = model_outputs->cat_split_type;
+                    single_tree_model.missing_action = model_outputs->missing_action;
+                    single_tree_model.trees.push_back(model_outputs->trees.back());
+
+                    predict_iforest(ref_numeric_data, ref_categ_data,
+                                    ref_is_col_major, ref_ld_numeric, ref_ld_categ,
+                                    ref_Xc, ref_Xc_ind, ref_Xc_indptr,
+                                    (real_t*)NULL, (sparse_ix*)NULL, (sparse_ix*)NULL,
+                                    n_ref, 1, false,
+                                    &single_tree_model, (ExtIsoForest*)NULL,
+                                    ignored.get(), terminal_indices.data(),
+                                    (double*)NULL,
+                                    indexer);
+                }
+
+                else
+                {
+                    ExtIsoForest single_tree_model;
+                    single_tree_model.new_cat_action = model_outputs_ext->new_cat_action;
+                    single_tree_model.cat_split_type = model_outputs_ext->cat_split_type;
+                    single_tree_model.missing_action = model_outputs_ext->missing_action;
+                    single_tree_model.hplanes.push_back(model_outputs_ext->hplanes.back());
+
+                    predict_iforest(ref_numeric_data, ref_categ_data,
+                                    ref_is_col_major, ref_ld_numeric, ref_ld_categ,
+                                    ref_Xc, ref_Xc_ind, ref_Xc_indptr,
+                                    (real_t*)NULL, (sparse_ix*)NULL, (sparse_ix*)NULL,
+                                    n_ref, 1, false,
+                                    (IsoForest*)NULL, &single_tree_model,
+                                    ignored.get(), terminal_indices.data(),
+                                    (double*)NULL,
+                                    indexer);
+                }
+
+                ignored.reset();
+                indexer->indices.back().reference_points.assign(terminal_indices.begin(), terminal_indices.end());
+                indexer->indices.back().reference_points.shrink_to_fit();
+                build_ref_node(indexer->indices.back());
+            }
+
+            check_interrupt_switch(ss);
         }
     }
 
     catch (...)
     {
         if (added_tree)
         {
```

### Comparing `isotree-0.5.8.post1/src/headers_joined.hpp` & `isotree-0.5.9/src/headers_joined.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 *          arXiv preprint arXiv:2110.13402 (2021).
 *     [12] Guha, Sudipto, et al.
 *          "Robust random cut forest based anomaly detection on streams."
 *          International conference on machine learning. PMLR, 2016.
 *     [13] Cortes, David.
 *          "Isolation forests: looking beyond tree depth."
 *          arXiv preprint arXiv:2111.11639 (2021).
+*     [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou.
+*          "Isolation kernel and its effect on SVM"
+*          Proceedings of the 24th ACM SIGKDD
+*          International Conference on Knowledge Discovery & Data Mining. 2018.
 * 
 *     BSD 2-Clause License
 *     Copyright (c) 2019-2022, David Cortes
 *     All rights reserved.
 *     Redistribution and use in source and binary forms, with or without
 *     modification, are permitted provided that the following conditions are met:
 *     * Redistributions of source code must retain the above copyright notice, this
@@ -63,8 +67,16 @@
 #include "extended.hpp"
 #include "fit_model.hpp"
 #include "helpers_iforest.hpp"
 #include "impute.hpp"
 #include "isoforest.hpp"
 #include "mult.hpp"
 #include "predict.hpp"
+#include "ref_indexer.hpp"
 #include "utils.hpp"
+
+/*  Note: Cython also defines these in its auto-generated code, and leads to
+    conflicts if they are not undefined and then included again.  */
+#ifdef _FOR_PYTHON
+    #undef likely
+    #undef unlikely
+#endif
```

### Comparing `isotree-0.5.8.post1/src/helpers_iforest.hpp` & `isotree-0.5.9/src/helpers_iforest.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 *          arXiv preprint arXiv:2110.13402 (2021).
 *     [12] Guha, Sudipto, et al.
 *          "Robust random cut forest based anomaly detection on streams."
 *          International conference on machine learning. PMLR, 2016.
 *     [13] Cortes, David.
 *          "Isolation forests: looking beyond tree depth."
 *          arXiv preprint arXiv:2111.11639 (2021).
+*     [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou.
+*          "Isolation kernel and its effect on SVM"
+*          Proceedings of the 24th ACM SIGKDD
+*          International Conference on Knowledge Discovery & Data Mining. 2018.
 * 
 *     BSD 2-Clause License
 *     Copyright (c) 2019-2022, David Cortes
 *     All rights reserved.
 *     Redistribution and use in source and binary forms, with or without
 *     modification, are permitted provided that the following conditions are met:
 *     * Redistributions of source code must retain the above copyright notice, this
```

### Comparing `isotree-0.5.8.post1/src/impute.hpp` & `isotree-0.5.9/src/impute.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 *          arXiv preprint arXiv:2110.13402 (2021).
 *     [12] Guha, Sudipto, et al.
 *          "Robust random cut forest based anomaly detection on streams."
 *          International conference on machine learning. PMLR, 2016.
 *     [13] Cortes, David.
 *          "Isolation forests: looking beyond tree depth."
 *          arXiv preprint arXiv:2111.11639 (2021).
+*     [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou.
+*          "Isolation kernel and its effect on SVM"
+*          Proceedings of the 24th ACM SIGKDD
+*          International Conference on Knowledge Discovery & Data Mining. 2018.
 * 
 *     BSD 2-Clause License
 *     Copyright (c) 2019-2022, David Cortes
 *     All rights reserved.
 *     Redistribution and use in source and binary forms, with or without
 *     modification, are permitted provided that the following conditions are met:
 *     * Redistributions of source code must retain the above copyright notice, this
```

### Comparing `isotree-0.5.8.post1/src/indexer.cpp` & `isotree-0.5.9/src/indexer.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 *          arXiv preprint arXiv:2110.13402 (2021).
 *     [12] Guha, Sudipto, et al.
 *          "Robust random cut forest based anomaly detection on streams."
 *          International conference on machine learning. PMLR, 2016.
 *     [13] Cortes, David.
 *          "Isolation forests: looking beyond tree depth."
 *          arXiv preprint arXiv:2111.11639 (2021).
+*     [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou.
+*          "Isolation kernel and its effect on SVM"
+*          Proceedings of the 24th ACM SIGKDD
+*          International Conference on Knowledge Discovery & Data Mining. 2018.
 * 
 *     BSD 2-Clause License
 *     Copyright (c) 2019-2022, David Cortes
 *     All rights reserved.
 *     Redistribution and use in source and binary forms, with or without
 *     modification, are permitted provided that the following conditions are met:
 *     * Redistributions of source code must retain the above copyright notice, this
@@ -190,15 +194,15 @@
                 temp = node_indices[frontier];
                 node_indices[frontier] = node_indices[ix];
                 node_indices[ix] = temp;
                 frontier++;
             }
         }
 
-        if (frontier == st) unexpected_error();
+        if (unlikely(frontier == st)) unexpected_error();
 
         curr_depth++;
         build_dindex_recursive<Node>(get_idx_tree_left(tree[curr_node]),
                                      n_terminal, ncomb,
                                      st, frontier-1,
                                      node_indices,
                                      node_mappings,
@@ -379,39 +383,49 @@
         {
             ind.reference_points.clear();
             ind.reference_indptr.clear();
             ind.reference_mapping.clear();
         }
     }
 
-    if (with_distances) {
-        build_distance_mappings(indexer, model, nthreads);
-    }
+    
+    try
+    {
+        if (with_distances) {
+            build_distance_mappings(indexer, model, nthreads);
+        }
 
-    else {
-        if (!indexer.indices.empty() && !indexer.indices.front().node_distances.empty())
-        {
-            for (auto &ind : indexer.indices)
+        else {
+            if (!indexer.indices.empty() && !indexer.indices.front().node_distances.empty())
             {
-                ind.node_distances.clear();
-                ind.node_depths.clear();
+                for (auto &ind : indexer.indices)
+                {
+                    ind.node_distances.clear();
+                    ind.node_depths.clear();
+                }
             }
+
+            build_terminal_node_mappings(indexer, model);
         }
+    }
 
-        build_terminal_node_mappings(indexer, model);
+    catch (...)
+    {
+        indexer.indices.clear();
+        throw;
     }
 }
 
 void build_tree_indices(TreesIndexer &indexer, const IsoForest &model, int nthreads, const bool with_distances)
 {
     if (model.trees.empty())
         throw std::runtime_error("Cannot build indexed for unfitted model.\n");
     if (model.missing_action == Divide)
         throw std::runtime_error("Cannot build tree indexer with 'missing_action=Divide'.\n");
-    if (model.new_cat_action == Weighted)
+    if (model.new_cat_action == Weighted && model.cat_split_type == SubSet)
     {
         for (const std::vector<IsoTree> &tree : model.trees)
         {
             for (const IsoTree &node : tree)
             {
                 if (!is_terminal_node(node) && node.col_type == Categorical)
                     throw std::runtime_error("Cannot build tree indexer with 'new_cat_action=Weighted'.\n");
@@ -457,85 +471,45 @@
 {
     if (model_outputs != NULL)
         build_tree_indices(*indexer, *model_outputs, nthreads, with_distances);
     else
         build_tree_indices(*indexer, *model_outputs_ext, nthreads, with_distances);
 }
 
-// template <class Model, class real_t, class sparse_ix>
-// void set_reference_points(TreesIndexer &indexer, Model &model, const bool with_distances, const bool with_kernel,
-//                           real_t *restrict numeric_data, int *restrict categ_data,
-//                           bool is_col_major, size_t ld_numeric, size_t ld_categ,
-//                           real_t *restrict Xc, sparse_ix *restrict Xc_ind, sparse_ix *restrict Xc_indptr,
-//                           real_t *restrict Xr, sparse_ix *restrict Xr_ind, sparse_ix *restrict Xr_indptr,
-//                           size_t nrows, int nthreads)
-// {
-//     if (indexer.indices.empty())
-//     {
-//         build_tree_indices(indexer, model, nthreads, with_distances);
-//     }
-
-//     size_t ntrees = get_ntrees(model);
-//     for (size_t tree = 0; tree < ntrees; tree++)
-//     {
-//         indexer.indices[tree].reference_points.resize(nrows);
-//         indexer.indices[tree].reference_points.shrink_to_fit();
-//     }
-
-//     std::vector<double> ignored(nrows);
-//     std::vector<sparse_ix> node_indices_predict(nrows * ntrees);
-//     void *model_ptr = (std::is_same<Model, IsoForest>::value)? &model : NULL;
-//     void *model_ext_ptr = (std::is_same<Model, ExtIsoForest>::value)? &model : NULL;
-//     predict_iforest(numeric_data, categ_data,
-//                     is_col_major, ld_numeric, ld_categ,
-//                     Xc, Xc_ind, Xc_indptr,
-//                     Xr, Xr_ind, Xr_indptr,
-//                     nrows, nthreads, false,
-//                     (IsoForest*)model_ptr, (ExtIsoForest*)model_ext_ptr,
-//                     ignored.data(), node_indices_predict.data(),
-//                     (double*)NULL);
-
-//     for (size_t tree = 0; tree < ntrees; tree++)
-//     {
-//         indexer.indices[tree].reference_points.assign(node_indices_predict.begin() + tree*nrows,
-//                                                       node_indices_predict.begin() + (tree+1)*nrows);
-//     }
-
-
-//     if (with_kernel)
-//     {
-//         std::vector<size_t> argsorted(nrows);
-//         for (size_t tree = 0; tree < ntrees; tree++)
-//         {
-//             std::iota(argsorted.begin(), argsorted.end(), (size_t)0);
-//             std::sort(argsorted.begin(), argsorted.end(),
-//                       [&indexer, &tree](const size_t a, const size_t b)
-//                       {indexer.indices[tree].reference_points[a] < indexer.indices[tree].reference_points[b];});
-//             indexer.indices[tree].reference_mapping.resize(nrows);
-//             indexer.indices[tree].reference_mapping.shrink_to_fit();
-//             for (size_t row = 0; row < nrows; row++)
-//                 indexer.indices[tree].reference_mapping[row] = argsorted[row];
-
-//             size_t n_terminal = *std::max_element(indexer.indices[tree].terminal_node_mappings.begin(),
-//                                                   indexer.indices[tree].terminal_node_mappings.end());
-//             indexer.indices[tree].reference_indptr.resize(n_terminal+1);
-//             indexer.indices[tree].reference_indptr.shrink_to_fit();
-//             indexer.indices[tree].reference_indptr[0] = 0;
-//             size_t curr_node = 0;
-//             std::vector<size_t>::iterator curr_begin = argsorted.begin();
-//             for (size_t node = 1; node < n_terminal; node++)
-//             {
-//                 curr_begin = std::lower_bound(curr_begin, argsorted.end(), node);
-//                 indexer.indices[tree].reference_indptr[node] = std::distance(argsorted.begin(), curr_begin);
-//                 if (curr_begin == argsorted.end() && node < n_terminal - 1)
-//                 {
-//                     std::fill(indexer.indices[tree].reference_indptr.begin() + node + 1,
-//                               indexer.indices[tree].reference_indptr.begin() + n_terminal,
-//                               indexer.indices[tree].reference_indptr[node]);
-//                     break;
-//                 }
-//             }
-//             for (size_t node = 1; node < n_terminal; node++)
-//                 indexer.indices[tree].reference_indptr[node+1] += indexer.indices[tree].reference_indptr[node];
-//         }
-//     }
-// }
+/* Gets the number of reference points stored in an indexer object */
+size_t get_number_of_reference_points(const TreesIndexer &indexer) noexcept
+{
+    if (indexer.indices.empty()) return 0;
+    return indexer.indices.front().reference_points.size();
+}
+
+/* This assumes it already has the indexer and 'reference_points' were just added.
+   It builds up 'reference_mapping' and 'reference_indptr' from it. */
+void build_ref_node(SingleTreeIndex &node)
+{
+    node.reference_mapping.resize(node.reference_points.size());
+    node.reference_mapping.shrink_to_fit();
+    std::iota(node.reference_mapping.begin(), node.reference_mapping.end(), (size_t)0);
+    std::sort(node.reference_mapping.begin(), node.reference_mapping.end(),
+              [&node](const size_t a, const size_t b)
+              {return node.reference_points[a] < node.reference_points[b];});
+
+    size_t n_terminal = node.n_terminal;
+    node.reference_indptr.assign(n_terminal+1, (size_t)0);
+    node.reference_indptr.shrink_to_fit();
+
+    std::vector<size_t>::iterator curr_begin = node.reference_mapping.begin();
+    std::vector<size_t>::iterator new_begin;
+    size_t curr_node;
+    while (curr_begin != node.reference_mapping.end())
+    {
+        curr_node = node.reference_points[*curr_begin];
+        new_begin = std::upper_bound(curr_begin, node.reference_mapping.end(), curr_node,
+                                     [&node](const size_t a, const size_t b)
+                                     {return a < node.reference_points[b];});
+        node.reference_indptr[curr_node+1] = std::distance(curr_begin, new_begin);
+        curr_begin = new_begin;
+    }
+
+    for (size_t ix = 1; ix < n_terminal; ix++)
+        node.reference_indptr[ix+1] += node.reference_indptr[ix];
+}
```

### Comparing `isotree-0.5.8.post1/src/instantiate_template_headers.hpp` & `isotree-0.5.9/src/instantiate_template_headers.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 *          arXiv preprint arXiv:2110.13402 (2021).
 *     [12] Guha, Sudipto, et al.
 *          "Robust random cut forest based anomaly detection on streams."
 *          International conference on machine learning. PMLR, 2016.
 *     [13] Cortes, David.
 *          "Isolation forests: looking beyond tree depth."
 *          arXiv preprint arXiv:2111.11639 (2021).
+*     [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou.
+*          "Isolation kernel and its effect on SVM"
+*          Proceedings of the 24th ACM SIGKDD
+*          International Conference on Knowledge Discovery & Data Mining. 2018.
 * 
 *     BSD 2-Clause License
 *     Copyright (c) 2019-2022, David Cortes
 *     All rights reserved.
 *     Redistribution and use in source and binary forms, with or without
 *     modification, are permitted provided that the following conditions are met:
 *     * Redistributions of source code must retain the above copyright notice, this
@@ -116,14 +120,17 @@
              double prob_pick_col_by_range, double prob_pick_col_by_var,
              double prob_pick_col_by_kurt,
              double min_gain, MissingAction missing_action,
              CategSplit cat_split_type, NewCategAction new_cat_action,
              UseDepthImp depth_imp, WeighImpRows weigh_imp_rows,
              bool   all_perm, Imputer *imputer, size_t min_imp_obs,
              TreesIndexer *indexer,
+             real_t ref_numeric_data[], int ref_categ_data[],
+             bool ref_is_col_major, size_t ref_ld_numeric, size_t ref_ld_categ,
+             real_t ref_Xc[], sparse_ix ref_Xc_ind[], sparse_ix ref_Xc_indptr[],
              uint64_t random_seed)
 {
     return add_tree<real_t, sparse_ix>
             (model_outputs, model_outputs_ext,
              numeric_data,  ncols_numeric,
              categ_data,    ncols_categ,    ncat,
              Xc, Xc_ind, Xc_indptr,
@@ -137,14 +144,17 @@
              prob_pick_col_by_range, prob_pick_col_by_var,
              prob_pick_col_by_kurt,
              min_gain, missing_action,
              cat_split_type, new_cat_action,
              depth_imp, weigh_imp_rows,
              all_perm, imputer, min_imp_obs,
              indexer,
+             ref_numeric_data, ref_categ_data,
+             ref_is_col_major, ref_ld_numeric, ref_ld_categ,
+             ref_Xc, ref_Xc_ind, ref_Xc_indptr,
              random_seed);
 }
 ISOTREE_EXPORTED void predict_iforest(real_t numeric_data[], int categ_data[],
                      bool is_col_major, size_t ncols_numeric, size_t ncols_categ,
                      real_t Xc[], sparse_ix Xc_ind[], sparse_ix Xc_indptr[],
                      real_t Xr[], sparse_ix Xr_ind[], sparse_ix Xr_indptr[],
                      size_t nrows, int nthreads, bool standardize,
@@ -162,25 +172,27 @@
                      model_outputs, model_outputs_ext,
                      output_depths,   tree_num,
                      per_tree_depths,
                      indexer);
 }
 ISOTREE_EXPORTED void calc_similarity(real_t numeric_data[], int categ_data[],
                      real_t Xc[], sparse_ix Xc_ind[], sparse_ix Xc_indptr[],
-                     size_t nrows, int nthreads, bool assume_full_distr, bool standardize_dist,
+                     size_t nrows, int nthreads,
+                     bool assume_full_distr, bool standardize_dist, bool as_kernel,
                      IsoForest *model_outputs, ExtIsoForest *model_outputs_ext,
-                     double tmat[], double rmat[], size_t n_from,
+                     double tmat[], double rmat[], size_t n_from, bool use_indexed_references,
                      TreesIndexer *indexer, bool is_col_major, size_t ld_numeric, size_t ld_categ)
 {
     calc_similarity<real_t, sparse_ix>
                     (numeric_data, categ_data,
                      Xc, Xc_ind, Xc_indptr,
-                     nrows, nthreads, assume_full_distr, standardize_dist,
+                     nrows, nthreads,
+                     assume_full_distr, standardize_dist, as_kernel,
                      model_outputs, model_outputs_ext,
-                     tmat, rmat, n_from,
+                     tmat, rmat, n_from, use_indexed_references,
                      indexer, is_col_major, ld_numeric, ld_categ);
 }
 ISOTREE_EXPORTED void impute_missing_values(real_t numeric_data[], int categ_data[], bool is_col_major,
                            real_t Xr[], sparse_ix Xr_ind[], sparse_ix Xr_indptr[],
                            size_t nrows, int nthreads,
                            IsoForest *model_outputs, ExtIsoForest *model_outputs_ext,
                            Imputer &imputer)
@@ -189,18 +201,36 @@
                           (numeric_data, categ_data, is_col_major,
                            Xr, Xr_ind, Xr_indptr,
                            nrows, nthreads,
                            model_outputs, model_outputs_ext,
                            imputer);
 }
 
+ISOTREE_EXPORTED void set_reference_points(IsoForest *model_outputs, ExtIsoForest *model_outputs_ext, TreesIndexer *indexer,
+                          const bool with_distances,
+                          real_t *numeric_data, int *categ_data,
+                          bool is_col_major, size_t ld_numeric, size_t ld_categ,
+                          real_t *Xc, sparse_ix *Xc_ind, sparse_ix *Xc_indptr,
+                          real_t *Xr, sparse_ix *Xr_ind, sparse_ix *Xr_indptr,
+                          size_t nrows, int nthreads)
+{
+    set_reference_points<real_t, sparse_ix>
+                        (model_outputs, model_outputs_ext, indexer,
+                         with_distances,
+                         numeric_data, categ_data,
+                         is_col_major, ld_numeric, ld_categ,
+                         Xc, Xc_ind, Xc_indptr,
+                         Xr, Xr_ind, Xr_indptr,
+                         nrows, nthreads);
+}
+
 #ifndef _NO_REAL_T
-ISOTREE_EXPORTED void get_num_nodes(IsoForest &model_outputs, sparse_ix *n_nodes, sparse_ix *n_terminal, int nthreads)
+ISOTREE_EXPORTED void get_num_nodes(IsoForest &model_outputs, sparse_ix *n_nodes, sparse_ix *n_terminal, int nthreads) noexcept
 {
     get_num_nodes<sparse_ix>(model_outputs, n_nodes, n_terminal, nthreads);
 }
-ISOTREE_EXPORTED void get_num_nodes(ExtIsoForest &model_outputs, sparse_ix *n_nodes, sparse_ix *n_terminal, int nthreads)
+ISOTREE_EXPORTED void get_num_nodes(ExtIsoForest &model_outputs, sparse_ix *n_nodes, sparse_ix *n_terminal, int nthreads) noexcept
 {
     get_num_nodes<sparse_ix>(model_outputs, n_nodes, n_terminal, nthreads);
 }
 #endif
```

### Comparing `isotree-0.5.8.post1/src/isoforest.hpp` & `isotree-0.5.9/src/isoforest.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 *          arXiv preprint arXiv:2110.13402 (2021).
 *     [12] Guha, Sudipto, et al.
 *          "Robust random cut forest based anomaly detection on streams."
 *          International conference on machine learning. PMLR, 2016.
 *     [13] Cortes, David.
 *          "Isolation forests: looking beyond tree depth."
 *          arXiv preprint arXiv:2111.11639 (2021).
+*     [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou.
+*          "Isolation kernel and its effect on SVM"
+*          Proceedings of the 24th ACM SIGKDD
+*          International Conference on Knowledge Discovery & Data Mining. 2018.
 * 
 *     BSD 2-Clause License
 *     Copyright (c) 2019-2022, David Cortes
 *     All rights reserved.
 *     Redistribution and use in source and binary forms, with or without
 *     modification, are permitted provided that the following conditions are met:
 *     * Redistributions of source code must retain the above copyright notice, this
```

### Comparing `isotree-0.5.8.post1/src/isotree.hpp` & `isotree-0.5.9/src/isotree.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 *          arXiv preprint arXiv:2110.13402 (2021).
 *     [12] Guha, Sudipto, et al.
 *          "Robust random cut forest based anomaly detection on streams."
 *          International conference on machine learning. PMLR, 2016.
 *     [13] Cortes, David.
 *          "Isolation forests: looking beyond tree depth."
 *          arXiv preprint arXiv:2111.11639 (2021).
+*     [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou.
+*          "Isolation kernel and its effect on SVM"
+*          Proceedings of the 24th ACM SIGKDD
+*          International Conference on Knowledge Discovery & Data Mining. 2018.
 * 
 *     BSD 2-Clause License
 *     Copyright (c) 2019-2022, David Cortes
 *     All rights reserved.
 *     Redistribution and use in source and binary forms, with or without
 *     modification, are permitted provided that the following conditions are met:
 *     * Redistributions of source code must retain the above copyright notice, this
@@ -134,14 +138,22 @@
     #ifdef AVOID_LONG_DOUBLE
         typedef double ldouble_safe;
     #else
         typedef long double ldouble_safe;
     #endif
 #endif
 
+#if defined(__GNUC__) || defined(__clang__)
+    #define likely(x) __builtin_expect((bool)(x), true)
+    #define unlikely(x) __builtin_expect((bool)(x), false)
+#else
+    #define likely(x) (x)
+    #define unlikely(x) (x)
+#endif
+
 #if defined(__GNUC__)  || defined(__clang__) || defined(_MSC_VER)
     #define unexpected_error() throw std::runtime_error(\
         std::string("Unexpected error in ") + \
         std::string(__FILE__) + \
         std::string(":") + \
         std::to_string(__LINE__) + \
         std::string(". Please open an issue in GitHub with this information, indicating the installed version of 'isotree'.\n"))
@@ -227,14 +239,16 @@
 /* https://stackoverflow.com/questions/2249731/how-do-i-get-bit-by-bit-data-from-an-integer-value-in-c */
 #define extract_bit(number, bit) (((number) >> (bit)) & 1)
 #ifndef _FOR_R
     #if defined(__GNUC__) && (__GNUC__ >= 5)
         #pragma GCC diagnostic pop
     #elif defined(__clang__)
         #pragma clang diagnostic pop
+        #pragma clang diagnostic push
+        #pragma clang diagnostic ignored "-Wunknown-attributes"
     #endif
 #endif
 using std::isinf;
 using std::isnan;
 #define is_na_or_inf(x) (isnan(x) || isinf(x))
 
 
@@ -252,22 +266,30 @@
     #else
         #define size_t_for size_t
     #endif
 #else
     #define size_t_for size_t
 #endif
 
-#if defined(_FOR_R) || defined(_FOR_PYTHON) || !defined(_WIN32)
+#if defined(_FOR_R) || defined(_FOR_PYTHON)
     #define ISOTREE_EXPORTED 
 #else
-    #ifdef ISOTREE_COMPILE_TIME
-        #define ISOTREE_EXPORTED __declspec(dllexport)
+    #if defined(_WIN32)
+        #ifdef ISOTREE_COMPILE_TIME
+            #define ISOTREE_EXPORTED __declspec(dllexport)
+        #else
+            #define ISOTREE_EXPORTED __declspec(dllimport)
+        #endif
     #else
-        #define ISOTREE_EXPORTED __declspec(dllimport)
-    #endif 
+        #if defined(EXPLICITLTY_EXPORT_SYMBOLS) && defined(ISOTREE_COMPILE_TIME)
+            #define ISOTREE_EXPORTED __attribute__((visibility ("default")))
+        #else
+            #define ISOTREE_EXPORTED 
+        #endif
+    #endif
 #endif
 
 
 /*   Apple at some point decided to drop OMP library and headers from its compiler distribution
 *    and to alias 'gcc' to 'clang', which work differently when given flags they cannot interpret,
 *    causing installation issues with pretty much all scientific software due to OMP headers that
 *    would normally do nothing. This piece of code is to allow compilation without OMP header. */
@@ -908,14 +930,17 @@
              double prob_pick_col_by_range, double prob_pick_col_by_var,
              double prob_pick_col_by_kurt,
              double min_gain, MissingAction missing_action,
              CategSplit cat_split_type, NewCategAction new_cat_action,
              UseDepthImp depth_imp, WeighImpRows weigh_imp_rows,
              bool   all_perm, Imputer *imputer, size_t min_imp_obs,
              TreesIndexer *indexer,
+             real_t ref_numeric_data[], int ref_categ_data[],
+             bool ref_is_col_major, size_t ref_ld_numeric, size_t ref_ld_categ,
+             real_t ref_Xc[], sparse_ix ref_Xc_ind[], sparse_ix ref_Xc_indptr[],
              uint64_t random_seed);
 template <class InputData, class WorkerMemory>
 void fit_itree(std::vector<IsoTree>    *tree_root,
                std::vector<IsoHPlane>  *hplane_root,
                WorkerMemory             &workspace,
                InputData                &input_data,
                ModelParams              &model_params,
@@ -965,47 +990,47 @@
 [[gnu::hot]]
 void traverse_itree_no_recurse(std::vector<IsoTree>  &tree,
                                IsoForest             &model_outputs,
                                PredictionData        &prediction_data,
                                double &restrict      output_depth,
                                sparse_ix *restrict   tree_num,
                                double *restrict      tree_depth,
-                               size_t                row);
+                               size_t                row) noexcept;
 template <class PredictionData, class sparse_ix, class ImputedData>
 [[gnu::hot]]
 double traverse_itree(std::vector<IsoTree>     &tree,
                       IsoForest                &model_outputs,
                       PredictionData           &prediction_data,
                       std::vector<ImputeNode> *impute_nodes,
                       ImputedData             *imputed_data,
                       double                   curr_weight,
                       size_t                   row,
                       sparse_ix *restrict      tree_num,
                       double *restrict         tree_depth,
-                      size_t                   curr_lev);
+                      size_t                   curr_lev) noexcept;
 template <class PredictionData, class sparse_ix>
 [[gnu::hot]]
 void traverse_hplane_fast(std::vector<IsoHPlane>  &hplane,
                           ExtIsoForest            &model_outputs,
                           PredictionData          &prediction_data,
                           double &restrict        output_depth,
                           sparse_ix *restrict     tree_num,
                           double *restrict        tree_depth,
-                          size_t                  row);
+                          size_t                  row) noexcept;
 template <class PredictionData, class sparse_ix, class ImputedData>
 [[gnu::hot]]
 void traverse_hplane(std::vector<IsoHPlane>   &hplane,
                      ExtIsoForest             &model_outputs,
                      PredictionData           &prediction_data,
                      double &restrict         output_depth,
                      std::vector<ImputeNode> *impute_nodes,
                      ImputedData             *imputed_data,
                      sparse_ix *restrict      tree_num,
                      double *restrict         tree_depth,
-                     size_t                   row);
+                     size_t                   row) noexcept;
 template <class real_t, class sparse_ix>
 void batched_csc_predict(PredictionData<real_t, sparse_ix> &prediction_data, int nthreads,
                          IsoForest *model_outputs, ExtIsoForest *model_outputs_ext,
                          double *restrict output_depths,   sparse_ix *restrict tree_num,
                          double *restrict per_tree_depths);
 template <class PredictionData, class sparse_ix>
 void traverse_itree_csc(WorkerForPredictCSC   &workspace,
@@ -1029,53 +1054,56 @@
 void add_csc_range_penalty(WorkerForPredictCSC  &workspace,
                            PredictionData       &prediction_data,
                            double *restrict     weights_arr,
                            size_t               col_num,
                            double               range_low,
                            double               range_high);
 template <class PredictionData>
-double extract_spC(PredictionData &prediction_data, size_t row, size_t col_num);
+double extract_spC(PredictionData &prediction_data, size_t row, size_t col_num) noexcept;
 template <class PredictionData, class sparse_ix>
-double extract_spR(PredictionData &prediction_data, sparse_ix *row_st, sparse_ix *row_end, size_t col_num);
+double extract_spR(PredictionData &prediction_data, sparse_ix *row_st, sparse_ix *row_end, size_t col_num) noexcept;
 template <class sparse_ix>
-void get_num_nodes(IsoForest &model_outputs, sparse_ix *restrict n_nodes, sparse_ix *restrict n_terminal, int nthreads);
+void get_num_nodes(IsoForest &model_outputs, sparse_ix *restrict n_nodes, sparse_ix *restrict n_terminal, int nthreads) noexcept;
 template <class sparse_ix>
-void get_num_nodes(ExtIsoForest &model_outputs, sparse_ix *restrict n_nodes, sparse_ix *restrict n_terminal, int nthreads);
+void get_num_nodes(ExtIsoForest &model_outputs, sparse_ix *restrict n_nodes, sparse_ix *restrict n_terminal, int nthreads) noexcept;
 
 /* dist.cpp */
 template <class real_t, class sparse_ix>
 void calc_similarity(real_t numeric_data[], int categ_data[],
                      real_t Xc[], sparse_ix Xc_ind[], sparse_ix Xc_indptr[],
-                     size_t nrows, int nthreads, bool assume_full_distr, bool standardize_dist,
+                     size_t nrows, int nthreads,
+                     bool assume_full_distr, bool standardize_dist, bool as_kernel,
                      IsoForest *model_outputs, ExtIsoForest *model_outputs_ext,
-                     double tmat[], double rmat[], size_t n_from,
+                     double tmat[], double rmat[], size_t n_from, bool use_indexed_references,
                      TreesIndexer *indexer, bool is_col_major, size_t ld_numeric, size_t ld_categ);
 template <class PredictionData>
 void traverse_tree_sim(WorkerForSimilarity   &workspace,
                        PredictionData        &prediction_data,
                        IsoForest             &model_outputs,
                        std::vector<IsoTree>  &trees,
-                       size_t                curr_tree);
+                       size_t                curr_tree,
+                       const bool            as_kernel);
 template <class PredictionData>
 void traverse_hplane_sim(WorkerForSimilarity     &workspace,
                          PredictionData          &prediction_data,
                          ExtIsoForest            &model_outputs,
                          std::vector<IsoHPlane>  &hplanes,
-                         size_t                  curr_tree);
+                         size_t                  curr_tree,
+                         const bool              as_kernel);
 template <class PredictionData, class InputData, class WorkerMemory>
 #ifndef _FOR_R
 [[gnu::optimize("no-trapping-math"), gnu::optimize("no-math-errno")]]
 #endif
 void gather_sim_result(std::vector<WorkerForSimilarity> *worker_memory,
                        std::vector<WorkerMemory> *worker_memory_m,
                        PredictionData *prediction_data, InputData *input_data,
                        IsoForest *model_outputs, ExtIsoForest *model_outputs_ext,
                        double *restrict tmat, double *restrict rmat, size_t n_from,
                        size_t ntrees, bool assume_full_distr,
-                       bool standardize_dist, int nthreads);
+                       bool standardize_dist, bool as_kernel, int nthreads);
 template <class PredictionData>
 void initialize_worker_for_sim(WorkerForSimilarity  &workspace,
                                PredictionData       &prediction_data,
                                IsoForest            *model_outputs,
                                ExtIsoForest         *model_outputs_ext,
                                size_t                n_from,
                                bool                  assume_full_distr);
@@ -1088,14 +1116,36 @@
     real_t *restrict numeric_data, int *restrict categ_data,
     real_t *restrict Xc, sparse_ix *restrict Xc_ind, sparse_ix *restrict Xc_indptr,
     size_t nrows, int nthreads, bool assume_full_distr, bool standardize_dist,
     IsoForest *model_outputs, ExtIsoForest *model_outputs_ext,
     double *restrict tmat, double *restrict rmat, size_t n_from,
     TreesIndexer *indexer, bool is_col_major, size_t ld_numeric, size_t ld_categ
 );
+template <class real_t, class sparse_ix>
+#ifndef _FOR_R
+[[gnu::optimize("no-trapping-math"), gnu::optimize("no-math-errno")]]
+#endif
+void calc_similarity_from_indexer_with_references
+(
+    real_t *restrict numeric_data, int *restrict categ_data,
+    real_t *restrict Xc, sparse_ix *restrict Xc_ind, sparse_ix *restrict Xc_indptr,
+    size_t nrows, int nthreads, bool standardize_dist,
+    IsoForest *model_outputs, ExtIsoForest *model_outputs_ext,
+    double *restrict rmat,
+    TreesIndexer *indexer, bool is_col_major, size_t ld_numeric, size_t ld_categ
+);
+template <class real_t, class sparse_ix>
+void kernel_to_references(TreesIndexer &indexer,
+                          IsoForest *model_outputs, ExtIsoForest *model_outputs_ext,
+                          real_t *restrict numeric_data, int *restrict categ_data,
+                          real_t *restrict Xc, sparse_ix *restrict Xc_ind, sparse_ix *restrict Xc_indptr,
+                          bool is_col_major, size_t ld_numeric, size_t ld_categ,
+                          size_t nrows, int nthreads,
+                          double *restrict rmat,
+                          bool standardize);
 
 /* impute.cpp */
 template <class real_t, class sparse_ix>
 void impute_missing_values(real_t numeric_data[], int categ_data[], bool is_col_major,
                            real_t Xr[], sparse_ix Xr_ind[], sparse_ix Xr_indptr[],
                            size_t nrows, int nthreads,
                            IsoForest *model_outputs, ExtIsoForest *model_outputs_ext,
@@ -1245,60 +1295,60 @@
                            double *restrict counter, double *restrict weights, double exp_remainder);
 void increase_comb_counter(size_t ix_arr[], size_t st, size_t end, size_t n,
                            double counter[], hashed_map<size_t, double> &weights, double exp_remainder);
 void increase_comb_counter_in_groups(size_t ix_arr[], size_t st, size_t end, size_t split_ix, size_t n,
                                      double counter[], double exp_remainder);
 void increase_comb_counter_in_groups(size_t ix_arr[], size_t st, size_t end, size_t split_ix, size_t n,
                                      double *restrict counter, double *restrict weights, double exp_remainder);
-void tmat_to_dense(double *restrict tmat, double *restrict dmat, size_t n, bool diag_to_one, bool diag_to_inf);
+void tmat_to_dense(double *restrict tmat, double *restrict dmat, size_t n, double fill_diag);
 template <class real_t=double>
 void build_btree_sampler(std::vector<double> &btree_weights, real_t *restrict sample_weights,
                          size_t nrows, size_t &restrict log2_n, size_t &restrict btree_offset);
 template <class real_t=double>
 void sample_random_rows(std::vector<size_t> &restrict ix_arr, size_t nrows, bool with_replacement,
                         RNG_engine &rnd_generator, std::vector<size_t> &restrict ix_all,
                         real_t *restrict sample_weights, std::vector<double> &restrict btree_weights,
                         size_t log2_n, size_t btree_offset, std::vector<bool> &is_repeated);
 template <class real_t=double>
 void weighted_shuffle(size_t *restrict outp, size_t n, real_t *restrict weights, double *restrict buffer_arr, RNG_engine &rnd_generator);
-double sample_random_uniform(double xmin, double xmax, RNG_engine &rng);
-size_t divide_subset_split(size_t ix_arr[], double x[], size_t st, size_t end, double split_point);
+double sample_random_uniform(double xmin, double xmax, RNG_engine &rng) noexcept;
+size_t divide_subset_split(size_t ix_arr[], double x[], size_t st, size_t end, double split_point) noexcept;
 template <class real_t=double>
 void divide_subset_split(size_t *restrict ix_arr, real_t x[], size_t st, size_t end, double split_point,
-                         MissingAction missing_action, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix);
+                         MissingAction missing_action, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix) noexcept;
 template <class real_t, class sparse_ix>
 void divide_subset_split(size_t *restrict ix_arr, size_t st, size_t end, size_t col_num,
                          real_t Xc[], sparse_ix *restrict Xc_ind, sparse_ix *restrict Xc_indptr, double split_point,
-                         MissingAction missing_action, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix);
+                         MissingAction missing_action, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix) noexcept;
 void divide_subset_split(size_t *restrict ix_arr, int x[], size_t st, size_t end, signed char split_categ[],
-                         MissingAction missing_action, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix);
+                         MissingAction missing_action, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix) noexcept;
 void divide_subset_split(size_t *restrict ix_arr, int x[], size_t st, size_t end, signed char split_categ[],
                          int ncat, MissingAction missing_action, NewCategAction new_cat_action,
-                         bool move_new_to_left, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix);
+                         bool move_new_to_left, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix) noexcept;
 void divide_subset_split(size_t *restrict ix_arr, int x[], size_t st, size_t end, int split_categ,
-                         MissingAction missing_action, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix);
+                         MissingAction missing_action, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix) noexcept;
 void divide_subset_split(size_t *restrict ix_arr, int x[], size_t st, size_t end,
                          MissingAction missing_action, NewCategAction new_cat_action,
-                         bool move_new_to_left, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix);
+                         bool move_new_to_left, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix) noexcept;
 template <class real_t=double>
 void get_range(size_t ix_arr[], real_t *restrict x, size_t st, size_t end,
-               MissingAction missing_action, double &restrict xmin, double &restrict xmax, bool &unsplittable);
+               MissingAction missing_action, double &restrict xmin, double &restrict xmax, bool &unsplittable) noexcept;
 template <class real_t>
 void get_range(real_t *restrict x, size_t n,
-               MissingAction missing_action, double &restrict xmin, double &restrict xmax, bool &unsplittable);
+               MissingAction missing_action, double &restrict xmin, double &restrict xmax, bool &unsplittable) noexcept;
 template <class real_t, class sparse_ix>
 void get_range(size_t *restrict ix_arr, size_t st, size_t end, size_t col_num,
                real_t *restrict Xc, sparse_ix *restrict Xc_ind, sparse_ix *restrict Xc_indptr,
-               MissingAction missing_action, double &restrict xmin_, double &restrict xmax_, bool &unsplittable);
+               MissingAction missing_action, double &restrict xmin_, double &restrict xmax_, bool &unsplittable) noexcept;
 template <class real_t, class sparse_ix>
 void get_range(size_t col_num, size_t nrows,
                real_t *restrict Xc, sparse_ix *restrict Xc_ind, sparse_ix *restrict Xc_indptr,
-               MissingAction missing_action, double &restrict xmin, double &restrict xmax, bool &unsplittable);
+               MissingAction missing_action, double &restrict xmin, double &restrict xmax, bool &unsplittable) noexcept;
 void get_categs(size_t *restrict ix_arr, int x[], size_t st, size_t end, int ncat,
-                MissingAction missing_action, signed char categs[], size_t &restrict npresent, bool &unsplittable);
+                MissingAction missing_action, signed char categs[], size_t &restrict npresent, bool &unsplittable) noexcept;
 template <class real_t>
 bool check_more_than_two_unique_values(size_t ix_arr[], size_t st, size_t end, real_t x[], MissingAction missing_action);
 bool check_more_than_two_unique_values(size_t ix_arr[], size_t st, size_t end, int x[], MissingAction missing_action);
 template <class real_t, class sparse_ix>
 bool check_more_than_two_unique_values(size_t *restrict ix_arr, size_t st, size_t end, size_t col,
                                        sparse_ix *restrict Xc_indptr, sparse_ix *restrict Xc_ind, real_t *restrict Xc,
                                        MissingAction missing_action);
@@ -1624,14 +1674,34 @@
 (
     TreesIndexer *indexer,
     const IsoForest *model_outputs,
     const ExtIsoForest *model_outputs_ext,
     int nthreads,
     const bool with_distances
 );
+ISOTREE_EXPORTED
+size_t get_number_of_reference_points(const TreesIndexer &indexer) noexcept;
+void build_ref_node(SingleTreeIndex &node);
+
+/* ref_indexer.hpp */
+template <class Model, class real_t, class sparse_ix>
+void set_reference_points(TreesIndexer &indexer, Model &model, const bool with_distances,
+                          real_t *restrict numeric_data, int *restrict categ_data,
+                          bool is_col_major, size_t ld_numeric, size_t ld_categ,
+                          real_t *restrict Xc, sparse_ix *restrict Xc_ind, sparse_ix *restrict Xc_indptr,
+                          real_t *restrict Xr, sparse_ix *restrict Xr_ind, sparse_ix *restrict Xr_indptr,
+                          size_t nrows, int nthreads);
+template <class real_t, class sparse_ix>
+void set_reference_points(IsoForest *model_outputs, ExtIsoForest *model_outputs_ext, TreesIndexer *indexer,
+                          const bool with_distances,
+                          real_t *restrict numeric_data, int *restrict categ_data,
+                          bool is_col_major, size_t ld_numeric, size_t ld_categ,
+                          real_t *restrict Xc, sparse_ix *restrict Xc_ind, sparse_ix *restrict Xc_indptr,
+                          real_t *restrict Xr, sparse_ix *restrict Xr_ind, sparse_ix *restrict Xr_indptr,
+                          size_t nrows, int nthreads);
 
 /* merge_models.cpp */
 ISOTREE_EXPORTED
 void merge_models(IsoForest*     model,      IsoForest*     other,
                   ExtIsoForest*  ext_model,  ExtIsoForest*  ext_other,
                   Imputer*       imputer,    Imputer*       iother,
                   TreesIndexer*  indexer,    TreesIndexer*  ind_other);
@@ -1641,16 +1711,19 @@
 void subset_model(IsoForest*     model,      IsoForest*     model_new,
                   ExtIsoForest*  ext_model,  ExtIsoForest*  ext_model_new,
                   Imputer*       imputer,    Imputer*       imputer_new,
                   TreesIndexer*  indexer,    TreesIndexer*  indexer_new,
                   size_t *trees_take, size_t ntrees_take);
 
 /* serialize.cpp */
+[[noreturn]]
 void throw_errno();
+[[noreturn]]
 void throw_ferror(FILE *file);
+[[noreturn]]
 void throw_feoferr();
 class FileHandle
 {
 public:
     FILE *handle = NULL;
     FileHandle(const char *fname, const char *mode)
     {
@@ -1690,23 +1763,23 @@
                     fprintf(stderr, "Error: could not close file.\n");
             }
             this->handle = NULL;
         }
     };
 #endif
 ISOTREE_EXPORTED
-bool has_wchar_t_file_serializers();
+bool has_wchar_t_file_serializers() noexcept;
 ISOTREE_EXPORTED
-size_t determine_serialized_size(const IsoForest &model);
+size_t determine_serialized_size(const IsoForest &model) noexcept;
 ISOTREE_EXPORTED
-size_t determine_serialized_size(const ExtIsoForest &model);
+size_t determine_serialized_size(const ExtIsoForest &model) noexcept;
 ISOTREE_EXPORTED
-size_t determine_serialized_size(const Imputer &model);
+size_t determine_serialized_size(const Imputer &model) noexcept;
 ISOTREE_EXPORTED
-size_t determine_serialized_size(const TreesIndexer &model);
+size_t determine_serialized_size(const TreesIndexer &model) noexcept;
 ISOTREE_EXPORTED
 void serialize_IsoForest(const IsoForest &model, char *out);
 ISOTREE_EXPORTED
 void serialize_IsoForest(const IsoForest &model, FILE *out);
 ISOTREE_EXPORTED
 void serialize_IsoForest(const IsoForest &model, std::ostream &out);
 ISOTREE_EXPORTED
@@ -1896,21 +1969,21 @@
 ISOTREE_EXPORTED
 bool check_can_undergo_incremental_serialization(const ExtIsoForest &model, const char *serialized_bytes);
 ISOTREE_EXPORTED
 bool check_can_undergo_incremental_serialization(const Imputer &model, const char *serialized_bytes);
 ISOTREE_EXPORTED
 bool check_can_undergo_incremental_serialization(const TreesIndexer &model, const char *serialized_bytes);
 ISOTREE_EXPORTED
-size_t determine_serialized_size_additional_trees(const IsoForest &model, size_t old_ntrees);
+size_t determine_serialized_size_additional_trees(const IsoForest &model, size_t old_ntrees) noexcept;
 ISOTREE_EXPORTED
-size_t determine_serialized_size_additional_trees(const ExtIsoForest &model, size_t old_ntrees);
+size_t determine_serialized_size_additional_trees(const ExtIsoForest &model, size_t old_ntrees) noexcept;
 ISOTREE_EXPORTED
-size_t determine_serialized_size_additional_trees(const Imputer &model, size_t old_ntrees);
+size_t determine_serialized_size_additional_trees(const Imputer &model, size_t old_ntrees) noexcept;
 ISOTREE_EXPORTED
-size_t determine_serialized_size_additional_trees(const TreesIndexer &model, size_t old_ntrees);
+size_t determine_serialized_size_additional_trees(const TreesIndexer &model, size_t old_ntrees) noexcept;
 ISOTREE_EXPORTED
 void incremental_serialize_IsoForest(const IsoForest &model, char *old_bytes_reallocated);
 ISOTREE_EXPORTED
 void incremental_serialize_ExtIsoForest(const ExtIsoForest &model, char *old_bytes_reallocated);
 ISOTREE_EXPORTED
 void incremental_serialize_Imputer(const Imputer &model, char *old_bytes_reallocated);
 ISOTREE_EXPORTED
@@ -1919,24 +1992,24 @@
 size_t determine_serialized_size_combined
 (
     const IsoForest *model,
     const ExtIsoForest *model_ext,
     const Imputer *imputer,
     const TreesIndexer *indexer,
     const size_t size_optional_metadata
-);
+) noexcept;
 ISOTREE_EXPORTED
 size_t determine_serialized_size_combined
 (
     const char *serialized_model,
     const char *serialized_model_ext,
     const char *serialized_imputer,
     const char *serialized_indexer,
     const size_t size_optional_metadata
-);
+) noexcept;
 ISOTREE_EXPORTED
 void serialize_combined
 (
     const IsoForest *model,
     const ExtIsoForest *model_ext,
     const Imputer *imputer,
     const TreesIndexer *indexer,
@@ -2044,20 +2117,20 @@
     const std::string &in,
     IsoForest *model,
     ExtIsoForest *model_ext,
     Imputer *imputer,
     TreesIndexer *indexer,
     char *optional_metadata
 );
-bool check_model_has_range_penalty(const IsoForest &model);
-bool check_model_has_range_penalty(const ExtIsoForest &model);
-void add_range_penalty(IsoForest &model);
-void add_range_penalty(ExtIsoForest &model);
-void add_range_penalty(Imputer &model);
-void add_range_penalty(TreesIndexer &model);
+bool check_model_has_range_penalty(const IsoForest &model) noexcept;
+bool check_model_has_range_penalty(const ExtIsoForest &model) noexcept;
+void add_range_penalty(IsoForest &model) noexcept;
+void add_range_penalty(ExtIsoForest &model) noexcept;
+void add_range_penalty(Imputer &model) noexcept;
+void add_range_penalty(TreesIndexer &model) noexcept;
 
 /* sql.cpp */
 ISOTREE_EXPORTED
 std::vector<std::string> generate_sql(IsoForest *model_outputs, ExtIsoForest *model_outputs_ext,
                                       std::vector<std::string> &numeric_colnames, std::vector<std::string> &categ_colnames,
                                       std::vector<std::vector<std::string>> &categ_levels,
                                       bool output_tree_num, bool index1, bool single_tree, size_t tree_num,
@@ -2076,8 +2149,14 @@
                           std::string &cond_left, std::string &cond_right,
                           std::vector<std::string> &numeric_colnames, std::vector<std::string> &categ_colnames,
                           std::vector<std::vector<std::string>> &categ_levels);
 void extract_cond_ext_isotree(ExtIsoForest &model, IsoHPlane &hplane,
                               std::string &cond_left, std::string &cond_right,
                               std::vector<std::string> &numeric_colnames, std::vector<std::string> &categ_colnames,
                               std::vector<std::vector<std::string>> &categ_levels);
+
+#ifndef _FOR_R
+    #if defined(__clang__)
+        #pragma clang diagnostic pop
+    #endif
+#endif
 #endif /* ISOTREE_H */
```

### Comparing `isotree-0.5.8.post1/src/merge_models.cpp` & `isotree-0.5.9/src/merge_models.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 *          arXiv preprint arXiv:2110.13402 (2021).
 *     [12] Guha, Sudipto, et al.
 *          "Robust random cut forest based anomaly detection on streams."
 *          International conference on machine learning. PMLR, 2016.
 *     [13] Cortes, David.
 *          "Isolation forests: looking beyond tree depth."
 *          arXiv preprint arXiv:2111.11639 (2021).
+*     [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou.
+*          "Isolation kernel and its effect on SVM"
+*          Proceedings of the 24th ACM SIGKDD
+*          International Conference on Knowledge Discovery & Data Mining. 2018.
 * 
 *     BSD 2-Clause License
 *     Copyright (c) 2019-2022, David Cortes
 *     All rights reserved.
 *     Redistribution and use in source and binary forms, with or without
 *     modification, are permitted provided that the following conditions are met:
 *     * Redistributions of source code must retain the above copyright notice, this
@@ -133,79 +137,122 @@
 
     if (imputer != NULL && iother == NULL)
         throw std::runtime_error("Model to append trees to has imputer, but model to take trees from doesn't.\n");
     if (indexer != NULL && ind_other == NULL)
         throw std::runtime_error("Model to append trees to has indexer, but model to take trees from doesn't.\n");
     if (indexer != NULL && ind_other != NULL)
     {
-        if (!indexer->indices.front().node_distances.empty() && ind_other->indices.front().node_distances.empty())
+        bool indexer_is_empty = indexer->indices.empty();
+        bool ind_other_is_empty = ind_other->indices.empty();
+        bool model_is_empty = (model != NULL && model->trees.empty()) || (ext_model != NULL && ext_model->hplanes.empty());
+        bool other_is_empty = (other != NULL && other->trees.empty()) || (ext_model != NULL && ext_other->hplanes.empty());
+
+        if (indexer_is_empty && !model_is_empty && ind_other_is_empty && !other_is_empty) {
+            indexer = NULL;
+            ind_other = NULL;
+            goto skip_indexers;
+        }
+
+        if (!model_is_empty && !indexer_is_empty && !other_is_empty && ind_other_is_empty)
+            throw std::runtime_error("Model to append trees to has indexer, but model to take trees from doesn't.\n");
+        if (!model_is_empty && indexer_is_empty && !other_is_empty && !ind_other_is_empty)
+            throw std::runtime_error("Model to take trees from has indexer, but model to append trees to doesn't.\n");
+
+        if (
+            !indexer_is_empty && !ind_other_is_empty &&
+            indexer->indices.front().reference_points.size() != ind_other->indices.front().reference_points.size()
+        ) {
+            throw std::runtime_error("Model to append trees to and model to take trees from have different number of reference points.\n");
+        }
+
+
+        if (
+            !indexer_is_empty &&
+            !ind_other_is_empty &&
+            !indexer->indices.front().node_distances.empty() &&
+            ind_other->indices.front().node_distances.empty()
+        ) {
             throw std::runtime_error("Model to append trees to has indexer with distances, but model to take trees from has indexer without distances.\n");
-        if (!indexer->indices.front().reference_points.empty() && ind_other->indices.front().reference_points.empty())
+        }
+        if (
+            !indexer_is_empty &&
+            !ind_other_is_empty &&
+            !indexer->indices.front().reference_points.empty() &&
+            ind_other->indices.front().reference_points.empty()
+        ) {
             throw std::runtime_error("Model to append trees to has indexer with reference points, but model to take trees from has indexer without reference points.\n");
-        if (!indexer->indices.front().reference_indptr.empty() && ind_other->indices.front().reference_indptr.empty())
+        }
+        if (
+            !indexer_is_empty &&
+            !ind_other_is_empty &&
+            !indexer->indices.front().reference_indptr.empty() &&
+            ind_other->indices.front().reference_indptr.empty()
+        ) {
             throw std::runtime_error("Model to append trees to has indexer with kernel reference points, but model to take trees from has indexer without kernel reference points.\n");
+        }
     }
+    skip_indexers:
 
     try
     {
         if (model != NULL && other != NULL)
         {
             if (model == other)
             {
                 auto other_copy = *other;
-                merge_models(model, &other_copy, ext_model, ext_other, imputer, iother, indexer, ind_other);
+                merge_models(model, &other_copy, NULL, NULL, NULL, NULL, NULL, NULL);
                 return;
             }
             model->trees.insert(model->trees.end(),
                                 other->trees.begin(),
                                 other->trees.end());
 
         }
 
         if (ext_model != NULL && ext_other != NULL)
         {
             if (ext_model == ext_other)
             {
                 auto other_copy = *ext_other;
-                merge_models(model, other, ext_model, &other_copy, imputer, iother, indexer, ind_other);
+                merge_models(NULL, NULL, ext_model, &other_copy, NULL, NULL, NULL, NULL);
                 return;
             }
             ext_model->hplanes.insert(ext_model->hplanes.end(),
                                       ext_other->hplanes.begin(),
                                       ext_other->hplanes.end());
         }
 
         if (imputer != NULL && iother != NULL)
         {
             if (imputer == iother)
             {
                 auto other_copy = *iother;
-                merge_models(model, other, ext_model, ext_other, imputer, &other_copy, indexer, ind_other);
+                merge_models(NULL, NULL, NULL, NULL, imputer, &other_copy, NULL, NULL);
                 return;
             }
             imputer->imputer_tree.insert(imputer->imputer_tree.end(),
                                          iother->imputer_tree.begin(),
                                          iother->imputer_tree.end());
         }
 
         if (indexer != NULL && ind_other != NULL)
         {
             if (indexer == ind_other)
             {
                 auto other_copy = *ind_other;
-                merge_models(model, other, ext_model, ext_other, imputer, iother, indexer, &other_copy);
+                merge_models(NULL, NULL, NULL, NULL, NULL, NULL, indexer, &other_copy);
                 return;
             }
             indexer->indices.insert(indexer->indices.end(),
                                     ind_other->indices.begin(),
                                     ind_other->indices.end());
         }
     }
 
-    catch(...)
+    catch (...)
     {
         if (model != NULL) model->trees.resize(curr_size_model);
         if (ext_model != NULL) ext_model->hplanes.resize(curr_size_model_ext);
         if (imputer != NULL) imputer->imputer_tree.resize(curr_size_imputer);
         if (indexer != NULL) indexer->indices.resize(curr_size_indexer);
         throw;
     }
```

### Comparing `isotree-0.5.8.post1/src/mult.hpp` & `isotree-0.5.9/src/mult.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 *          arXiv preprint arXiv:2110.13402 (2021).
 *     [12] Guha, Sudipto, et al.
 *          "Robust random cut forest based anomaly detection on streams."
 *          International conference on machine learning. PMLR, 2016.
 *     [13] Cortes, David.
 *          "Isolation forests: looking beyond tree depth."
 *          arXiv preprint arXiv:2111.11639 (2021).
+*     [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou.
+*          "Isolation kernel and its effect on SVM"
+*          Proceedings of the 24th ACM SIGKDD
+*          International Conference on Knowledge Discovery & Data Mining. 2018.
 * 
 *     BSD 2-Clause License
 *     Copyright (c) 2019-2022, David Cortes
 *     All rights reserved.
 *     Redistribution and use in source and binary forms, with or without
 *     modification, are permitted provided that the following conditions are met:
 *     * Redistributions of source code must retain the above copyright notice, this
@@ -95,15 +99,15 @@
         {
             m_prev = x[ix_arr[++st]];
         }
 
         for (size_t row = st; row <= end; row++)
         {
             xval = x[ix_arr[row]];
-            if (!is_na_or_inf(xval))
+            if (likely(!is_na_or_inf(xval)))
             {
                 cnt++;
                 m += (xval - m) / (real_t)cnt;
                 s  = std::fma(xval - m, xval - m_prev, s);
                 m_prev = m;
             }
         }
@@ -118,15 +122,15 @@
 {
     size_t cnt = 0;
     double m = 0;
     real_t_ xval;
     for (size_t row = st; row <= end; row++)
     {
         xval = x[ix_arr[row]];
-        if (!is_na_or_inf(xval))
+        if (likely(!is_na_or_inf(xval)))
         {
             cnt++;
             m += (xval - m) / (double)cnt;
         }
     }
 
     return m;
@@ -157,15 +161,15 @@
     {
         m_prev = x[ix_arr[++st]];
     }
 
     for (size_t row = st; row <= end; row++)
     {
         xval = x[ix_arr[row]];
-        if (!is_na_or_inf(xval))
+        if (likely(!is_na_or_inf(xval)))
         {
             w_this = w[ix_arr[row]];
             cnt += w_this;
             m = std::fma(w_this, (xval - m) / cnt, m);
             s = std::fma(w_this, (xval - m) * (xval - m_prev), s);
             m_prev = m;
         }
@@ -179,15 +183,15 @@
 double calc_mean_only_weighted(size_t ix_arr[], size_t st, size_t end, real_t_ *restrict x, mapping &w)
 {
     double cnt = 0;
     double w_this;
     double m = 0;
     for (size_t row = st; row <= end; row++)
     {
-        if (!is_na_or_inf(x[ix_arr[row]]))
+        if (likely(!is_na_or_inf(x[ix_arr[row]])))
         {
             w_this = w[ix_arr[row]];
             cnt += w_this;
             m = std::fma(w_this, (x[ix_arr[row]] - m) / cnt, m);
         }
     }
 
@@ -221,15 +225,15 @@
 
     for (size_t *row = ptr_st;
          row != ix_arr + end + 1 && curr_pos != end_col + 1 && ind_end_col >= *row;
         )
     {
         if (Xc_ind[curr_pos] == (sparse_ix)(*row))
         {
-            if (is_na_or_inf(Xc[curr_pos]))
+            if (unlikely(is_na_or_inf(Xc[curr_pos])))
             {
                 cnt--;
             }
 
             else
             {
                 if (added == 0) m_prev = Xc[curr_pos];
@@ -305,15 +309,15 @@
 
     for (size_t *row = ptr_st;
          row != ix_arr + end + 1 && curr_pos != end_col + 1 && ind_end_col >= *row;
         )
     {
         if (Xc_ind[curr_pos] == (sparse_ix)(*row))
         {
-            if (is_na_or_inf(Xc[curr_pos]))
+            if (unlikely(is_na_or_inf(Xc[curr_pos])))
                 cnt--;
             else
                 m += (Xc[curr_pos] - m) / (double)(++added);
 
             if (row == ix_arr + end || curr_pos == end_col) break;
             curr_pos = std::lower_bound(Xc_ind + curr_pos + 1, Xc_ind + end_col + 1, *(++row)) - Xc_ind;
         }
@@ -365,15 +369,15 @@
 
     for (size_t *row = ptr_st;
          row != ix_arr + end + 1 && curr_pos != end_col + 1 && ind_end_col >= *row;
         )
     {
         if (Xc_ind[curr_pos] == (sparse_ix)(*row))
         {
-            if (is_na_or_inf(Xc[curr_pos]))
+            if (unlikely(is_na_or_inf(Xc[curr_pos])))
             {
                 cnt -= w[*row];
             }
 
             else
             {
                 w_this = w[*row];
@@ -443,15 +447,15 @@
 
     for (size_t *row = ptr_st;
          row != ix_arr + end + 1 && curr_pos != end_col + 1 && ind_end_col >= *row;
         )
     {
         if (Xc_ind[curr_pos] == (sparse_ix)(*row))
         {
-            if (is_na_or_inf(Xc[curr_pos])) {
+            if (unlikely(is_na_or_inf(Xc[curr_pos]))) {
                 cnt -= w[*row];
             }
 
             else {
                 w_this = w[*row];
                 added += w_this;
                 m += w_this * (Xc[curr_pos] - m) / added;
@@ -507,15 +511,15 @@
 
     else
     {
         if (first_run)
         {
             for (size_t row = st; row <= end; row++)
             {
-                if (!is_na_or_inf(x[ix_arr[row]]))
+                if (likely(!is_na_or_inf(x[ix_arr[row]])))
                 {
                     res_write[row]     =  std::fma(x[ix_arr[row]] - x_mean, coef, res_write[row]);
                     buffer_arr[cnt++]  =  x[ix_arr[row]];
                 }
 
                 else
                 {
@@ -585,15 +589,15 @@
 
     else
     {
         if (first_run)
         {
             for (size_t row = st; row <= end; row++)
             {
-                if (!is_na_or_inf(x[ix_arr[row]]))
+                if (likely(!is_na_or_inf(x[ix_arr[row]])))
                 {
                     w_this = w[ix_arr[row]];
                     res_write[row]     = std::fma(x[ix_arr[row]] - x_mean, coef, res_write[row]);
                     obs_weight[cnt]    = w_this;
                     buffer_arr[cnt++]  =  x[ix_arr[row]];
                     cumw += w_this;
                 }
@@ -712,15 +716,15 @@
         {
             for (size_t *row = ptr_st;
                  row != ix_arr + end + 1 && curr_pos != end_col + 1 && ind_end_col >= *row;
                 )
             {
                 if (Xc_ind[curr_pos] == (sparse_ix)(*row))
                 {
-                    if (is_na_or_inf(Xc[curr_pos]))
+                    if (unlikely(is_na_or_inf(Xc[curr_pos])))
                     {
                         buffer_NAs[cnt_NA++] = row - ix_arr_plus_st;
                     }
 
                     else
                     {
                         buffer_arr[cnt_non_NA++]   = Xc[curr_pos];
@@ -883,15 +887,15 @@
         std::vector<double> obs_weight(end-st+1);
         for (size_t row = st; row <= end; row++)
             obs_weight[row - st] = w[ix_arr[row]];
 
         size_t end_new = end - st + 1;
         for (size_t ix = 0; ix < end-st+1; ix++)
         {
-            if (is_na_or_inf(denseX[ix]))
+            if (unlikely(is_na_or_inf(denseX[ix])))
             {
                 std::swap(denseX[ix], denseX[--end_new]);
                 std::swap(obs_weight[ix], obs_weight[end_new]);
             }
         }
 
         ldouble_safe cumw = std::accumulate(obs_weight.begin(), obs_weight.begin() + end_new, (ldouble_safe)0);
@@ -962,15 +966,15 @@
                     size_t cnt_NA = 0;
                     size_t cnt_this = 0;
                     size_t cnt = end - st + 1;
                     if (first_run)
                     {
                         for (size_t row = st; row <= end; row++)
                         {
-                            if (x[ix_arr[row]] < 0)
+                            if (unlikely(x[ix_arr[row]] < 0))
                             {
                                 cnt_NA++;
                             }
 
                             else if (x[ix_arr[row]] == chosen_cat)
                             {
                                 cnt_this++;
@@ -1102,15 +1106,15 @@
                     // cat = std::min(cat, ncat); /* in case it picks the last one */
                     fill_val = cat_coef[buffer_pos[cat]];
                     if (new_cat_action != Smallest)
                         fill_new = fill_val;
 
                     if (buffer_cnt[ncat] > 0 && fill_val) /* NAs */
                         for (size_t row = st; row <= end; row++)
-                            if (x[ix_arr[row]] < 0)
+                            if (unlikely(x[ix_arr[row]] < 0))
                                 res_write[row] += fill_val;
                 }
             }
 
             /* now fill unseen categories */
             if (new_cat_action != Random)
                 for (int cat = 0; cat < ncat; cat++)
@@ -1150,15 +1154,15 @@
                     bool has_NA = false;
                     ldouble_safe cnt_this = 0;
                     ldouble_safe cnt_other = 0;
                     if (first_run)
                     {
                         for (size_t row = st; row <= end; row++)
                         {
-                            if (x[ix_arr[row]] < 0)
+                            if (unlikely(x[ix_arr[row]] < 0))
                             {
                                 has_NA = true;
                             }
 
                             else if (x[ix_arr[row]] == chosen_cat)
                             {
                                 cnt_this += w[ix_arr[row]];
@@ -1179,15 +1183,15 @@
                         return;
                     }
 
                     fill_val = (cnt_this > cnt_other)? single_cat_coef : 0;
                     if (has_NA && fill_val)
                     {
                         for (size_t row = st; row <= end; row++)
-                            if (x[ix_arr[row]] < 0)
+                            if (unlikely(x[ix_arr[row]] < 0))
                                 res_write[row] += fill_val;
                     }
                     return;
                 }
 
                 default:
                 {
@@ -1241,15 +1245,15 @@
                     break;
                 }
 
                 default:
                 {
                     for (size_t row = st; row <= end; row++)
                     {
-                        if (x[ix_arr[row]] >= 0)
+                        if (likely(x[ix_arr[row]] >= 0))
                         {
                             buffer_cnt[x[ix_arr[row]]] += w[ix_arr[row]];
                             res_write[row] += cat_coef[x[ix_arr[row]]];
                         }
 
                         else
                         {
@@ -1296,15 +1300,15 @@
                     // cat = std::min(cat, ncat); /* in case it picks the last one */
                     fill_val = cat_coef[buffer_pos[cat]];
                     if (new_cat_action != Smallest)
                         fill_new = fill_val;
 
                     if (buffer_cnt[ncat] > 0 && fill_val) /* NAs */
                         for (size_t row = st; row <= end; row++)
-                            if (x[ix_arr[row]] < 0)
+                            if (unlikely(x[ix_arr[row]] < 0))
                                 res_write[row] += fill_val;
                 }
             }
 
             /* now fill unseen categories */
             if (new_cat_action != Random)
                 for (int cat = 0; cat < ncat; cat++)
```

### Comparing `isotree-0.5.8.post1/src/other_helpers.hpp` & `isotree-0.5.9/src/other_helpers.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 *          arXiv preprint arXiv:2110.13402 (2021).
 *     [12] Guha, Sudipto, et al.
 *          "Robust random cut forest based anomaly detection on streams."
 *          International conference on machine learning. PMLR, 2016.
 *     [13] Cortes, David.
 *          "Isolation forests: looking beyond tree depth."
 *          arXiv preprint arXiv:2111.11639 (2021).
+*     [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou.
+*          "Isolation kernel and its effect on SVM"
+*          Proceedings of the 24th ACM SIGKDD
+*          International Conference on Knowledge Discovery & Data Mining. 2018.
 * 
 *     BSD 2-Clause License
 *     Copyright (c) 2019-2022, David Cortes
 *     All rights reserved.
 *     Redistribution and use in source and binary forms, with or without
 *     modification, are permitted provided that the following conditions are met:
 *     * Redistributions of source code must retain the above copyright notice, this
```

### Comparing `isotree-0.5.8.post1/src/predict.hpp` & `isotree-0.5.9/src/predict.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 *          arXiv preprint arXiv:2110.13402 (2021).
 *     [12] Guha, Sudipto, et al.
 *          "Robust random cut forest based anomaly detection on streams."
 *          International conference on machine learning. PMLR, 2016.
 *     [13] Cortes, David.
 *          "Isolation forests: looking beyond tree depth."
 *          arXiv preprint arXiv:2111.11639 (2021).
+*     [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou.
+*          "Isolation kernel and its effect on SVM"
+*          Proceedings of the 24th ACM SIGKDD
+*          International Conference on Knowledge Discovery & Data Mining. 2018.
 * 
 *     BSD 2-Clause License
 *     Copyright (c) 2019-2022, David Cortes
 *     All rights reserved.
 *     Redistribution and use in source and binary forms, with or without
 *     modification, are permitted provided that the following conditions are met:
 *     * Redistributions of source code must retain the above copyright notice, this
@@ -191,14 +195,16 @@
                      real_t *restrict Xr, sparse_ix *restrict Xr_ind, sparse_ix *restrict Xr_indptr,
                      size_t nrows, int nthreads, bool standardize,
                      IsoForest *model_outputs, ExtIsoForest *model_outputs_ext,
                      double *restrict output_depths,   sparse_ix *restrict tree_num,
                      double *restrict per_tree_depths,
                      TreesIndexer *indexer)
 {
+    if (unlikely(!nrows)) return;
+
     /* put data in a struct for passing it in fewer lines */
     PredictionData<real_t, sparse_ix>
                    prediction_data = {numeric_data, categ_data, nrows,
                                       is_col_major, ld_numeric, ld_categ,
                                       Xc, Xc_ind, Xc_indptr,
                                       Xr, Xr_ind, Xr_indptr};
 
@@ -216,15 +222,15 @@
     }
 
     /* Regular case (no specialized CSC route) */
     else if (model_outputs != NULL)
     {
         if (
             model_outputs->missing_action == Fail &&
-            (model_outputs->new_cat_action != Weighted || prediction_data.categ_data == NULL) &&
+            (model_outputs->new_cat_action != Weighted || model_outputs->cat_split_type == SingleCateg || prediction_data.categ_data == NULL) &&
             prediction_data.Xc_indptr == NULL && prediction_data.Xr_indptr == NULL &&
             !model_outputs->has_range_penalty
             )
         {
             #pragma omp parallel for if(nrows > 1) schedule(static) num_threads(nthreads) \
                     shared(nrows, model_outputs, prediction_data, output_depths, tree_num, per_tree_depths)
             for (size_t_for row = 0; row < (decltype(row))nrows; row++)
@@ -431,15 +437,15 @@
         if (indexer != NULL && !indexer->indices.empty())
         {
             size_t ntrees = (model_outputs != NULL)? model_outputs->trees.size() : model_outputs_ext->hplanes.size();
             if (model_outputs != NULL)
             {
                 if (model_outputs->missing_action == Divide)
                     goto manual_remap;
-                if (model_outputs->new_cat_action == Weighted && categ_data != NULL)
+                if (model_outputs->new_cat_action == Weighted && model_outputs->cat_split_type == SubSet && categ_data != NULL)
                     goto manual_remap;
             }
 
             for (size_t tree = 0; tree < ntrees; tree++)
             {
                 size_t *restrict mapping = indexer->indices[tree].terminal_node_mappings.data();
                 for (size_t row = 0; row < nrows; row++)
@@ -461,28 +467,28 @@
 template <class PredictionData, class sparse_ix>
 void traverse_itree_no_recurse(std::vector<IsoTree>  &tree,
                                IsoForest             &model_outputs,
                                PredictionData        &prediction_data,
                                double &restrict      output_depth,
                                sparse_ix *restrict   tree_num,
                                double *restrict      tree_depth,
-                               size_t                row)
+                               size_t                row) noexcept
 {
     size_t curr_lev = 0;
     double xval;
     int    cval;
     while (true)
     {
         // if (tree[curr_lev].score > 0)
-        if (tree[curr_lev].tree_left == 0)
+        if (unlikely(tree[curr_lev].tree_left == 0))
         {
             output_depth += tree[curr_lev].score;
-            if (tree_num != NULL)
+            if (unlikely(tree_num != NULL))
                 tree_num[row] = curr_lev;
-            if (tree_depth != NULL)
+            if (unlikely(tree_depth != NULL))
                 *tree_depth = tree[curr_lev].score;
             break;
         }
 
         else
         {
             switch(tree[curr_lev].col_type)
@@ -539,15 +545,15 @@
                                         curr_lev = (tree[curr_lev].cat_split[cval])?
                                                     tree[curr_lev].tree_left : tree[curr_lev].tree_right;
                                         break;
                                     }
 
                                     case Smallest:
                                     {
-                                        if (cval >= (int)tree[curr_lev].cat_split.size())
+                                        if (unlikely(cval >= (int)tree[curr_lev].cat_split.size()))
                                         {
                                             curr_lev =  (tree[curr_lev].pct_tree_left < .5)? tree[curr_lev].tree_left : tree[curr_lev].tree_right;
                                         }
 
                                         else
                                         {
                                             curr_lev = (tree[curr_lev].cat_split[cval])?
@@ -594,15 +600,15 @@
                       PredictionData           &prediction_data,
                       std::vector<ImputeNode> *impute_nodes,     /* only when imputing missing */
                       ImputedData             *imputed_data,     /* only when imputing missing */
                       double                   curr_weight,      /* only when imputing missing */
                       size_t                   row,
                       sparse_ix *restrict      tree_num,
                       double *restrict         tree_depth,
-                      size_t                   curr_lev)
+                      size_t                   curr_lev) noexcept
 {
     double xval;
     int    cval;
     double range_penalty = 0;
 
     NumericConfig numeric_config;
     if (prediction_data.Xr_indptr != NULL)
@@ -620,21 +626,21 @@
         row_st  = prediction_data.Xr_ind + prediction_data.Xr_indptr[row];
         row_end = prediction_data.Xr_ind + prediction_data.Xr_indptr[row + 1];
     }
 
     while (true)
     {
         // if (tree[curr_lev].score >= 0.)
-        if (tree[curr_lev].tree_left == 0)
+        if (unlikely(tree[curr_lev].tree_left == 0))
         {
-            if (tree_num != NULL)
+            if (unlikely(tree_num != NULL))
                 tree_num[row] = curr_lev;
-            if (tree_depth != NULL)
+            if (unlikely(tree_depth != NULL))
                 *tree_depth = tree[curr_lev].score;
-            if (imputed_data != NULL)
+            if (unlikely(imputed_data != NULL))
                 add_from_impute_node((*impute_nodes)[curr_lev], *imputed_data, curr_weight);
 
             return tree[curr_lev].score - range_penalty;
         }
 
         else
         {
@@ -665,15 +671,15 @@
                         case SparseCSC:
                         {
                             xval = extract_spC(prediction_data, row, tree[curr_lev].col_num);
                             break;
                         }
                     }
 
-                    if (isnan(xval))
+                    if (unlikely(isnan(xval)))
                     {
                         switch(model_outputs.missing_action)
                         {
                             case Divide:
                             {
                                 return
                                     tree[curr_lev].pct_tree_left
@@ -714,15 +720,15 @@
                 {
                     cval =  prediction_data.categ_data[
                                 prediction_data.is_col_major?
                                 (row +  tree[curr_lev].col_num * prediction_data.nrows)
                                     :
                                 (tree[curr_lev].col_num + row * prediction_data.ncols_categ)
                             ];
-                    if (cval < 0)
+                    if (unlikely(cval < 0))
                     {
                         switch(model_outputs.missing_action)
                         {
                             case Divide:
                             {
                                 return
                                     tree[curr_lev].pct_tree_left
@@ -816,15 +822,15 @@
                                             curr_lev = (tree[curr_lev].cat_split[cval])?
                                                         tree[curr_lev].tree_left : tree[curr_lev].tree_right;
                                             break;
                                         }
 
                                         case Smallest:
                                         {
-                                            if (cval >= (int)tree[curr_lev].cat_split.size())
+                                            if (unlikely(cval >= (int)tree[curr_lev].cat_split.size()))
                                             {
                                                 curr_lev =  (tree[curr_lev].pct_tree_left < .5)? tree[curr_lev].tree_left : tree[curr_lev].tree_right;
                                             }
 
                                             else
                                             {
                                                 curr_lev = (tree[curr_lev].cat_split[cval])?
@@ -882,28 +888,28 @@
 template <class PredictionData, class sparse_ix>
 void traverse_hplane_fast(std::vector<IsoHPlane>  &hplane,
                           ExtIsoForest            &model_outputs,
                           PredictionData          &prediction_data,
                           double &restrict        output_depth,
                           sparse_ix *restrict     tree_num,
                           double *restrict        tree_depth,
-                          size_t                  row)
+                          size_t                  row) noexcept
 {
     size_t  curr_lev = 0;
     double  hval;
 
     while(true)
     {
         // if (hplane[curr_lev].score > 0)
-        if (hplane[curr_lev].hplane_left == 0)
+        if (unlikely(hplane[curr_lev].hplane_left == 0))
         {
             output_depth += hplane[curr_lev].score;
-            if (tree_num != NULL)
+            if (unlikely(tree_num != NULL))
                 tree_num[row] = curr_lev;
-            if (tree_depth != NULL)
+            if (unlikely(tree_depth != NULL))
                 *tree_depth = hplane[curr_lev].score;
             return;
         }
 
         else
         {
             hval = 0;
@@ -933,15 +939,15 @@
                      ExtIsoForest             &model_outputs,
                      PredictionData           &prediction_data,
                      double &restrict         output_depth,
                      std::vector<ImputeNode> *impute_nodes,     /* only when imputing missing */
                      ImputedData             *imputed_data,     /* only when imputing missing */
                      sparse_ix *restrict      tree_num,
                      double *restrict         tree_depth,
-                     size_t                   row)
+                     size_t                   row) noexcept
 {
     size_t  curr_lev = 0;
     double  xval;
     int     cval;
     double  hval;
 
     size_t ncols_numeric, ncols_categ;
@@ -962,22 +968,22 @@
         row_st  = prediction_data.Xr_ind + prediction_data.Xr_indptr[row];
         row_end = prediction_data.Xr_ind + prediction_data.Xr_indptr[row + 1];
     }
 
     while(true)
     {
         // if (hplane[curr_lev].score > 0)
-        if (hplane[curr_lev].hplane_left == 0)
+        if (unlikely(hplane[curr_lev].hplane_left == 0))
         {
             output_depth += hplane[curr_lev].score;
-            if (tree_num != NULL)
+            if (unlikely(tree_num != NULL))
                 tree_num[row] = curr_lev;
-            if (tree_depth != NULL)
+            if (unlikely(tree_depth != NULL))
                 *tree_depth = hplane[curr_lev].score;
-            if (imputed_data != NULL)
+            if (unlikely(imputed_data != NULL))
             {
                 add_from_impute_node((*impute_nodes)[curr_lev], *imputed_data, (double)1);
             }
             return;
         }
 
         else
@@ -1013,15 +1019,15 @@
                             case SparseCSC:
                             {
                                 xval = extract_spC(prediction_data, row, hplane[curr_lev].col_num[col]);
                                 break;
                             }
                         }
 
-                        if (is_na_or_inf(xval))
+                        if (unlikely(is_na_or_inf(xval)))
                         {
                             if (model_outputs.missing_action != Fail)
                             {
                                 hval += hplane[curr_lev].fill_val[col];
                             }
 
                             else
@@ -1044,15 +1050,15 @@
                     {
                         cval = prediction_data.categ_data[
                             prediction_data.is_col_major?
                             (row +  hplane[curr_lev].col_num[col] * prediction_data.nrows)
                                 :
                             (hplane[curr_lev].col_num[col] + row * prediction_data.ncols_categ)
                         ];
-                        if (cval < 0)
+                        if (unlikely(cval < 0))
                         {
                             if (model_outputs.missing_action != Fail)
                             {
                                 hval += hplane[curr_lev].fill_val[col];
                             }
                             
                             else
@@ -1070,15 +1076,15 @@
                                 {
                                     hval += (cval == hplane[curr_lev].chosen_cat[ncols_categ])? hplane[curr_lev].fill_new[ncols_categ] : 0;
                                     break;
                                 }
 
                                 case SubSet:
                                 {
-                                    if (cval >= (int)hplane[curr_lev].cat_coef[ncols_categ].size())
+                                    if (unlikely(cval >= (int)hplane[curr_lev].cat_coef[ncols_categ].size()))
                                     {
                                         if (model_outputs.new_cat_action == Random) {
                                             cval = cval % (int)hplane[curr_lev].cat_coef[ncols_categ].size();
                                             hval += hplane[curr_lev].cat_coef[ncols_categ][cval];
                                         }
 
                                         else {
@@ -1150,15 +1156,15 @@
                     ptr_worker->depths.resize(prediction_data.nrows);
                     ptr_worker->ix_arr.resize(prediction_data.nrows);
                     std::iota(ptr_worker->ix_arr.begin(),
                               ptr_worker->ix_arr.end(),
                               (size_t)0);
 
                     if (model_outputs->missing_action == Divide ||
-                        (model_outputs->new_cat_action == Weighted && prediction_data.categ_data != NULL)
+                        (model_outputs->new_cat_action == Weighted && model_outputs->cat_split_type == SubSet && prediction_data.categ_data != NULL)
                     ) {
                         ptr_worker->weights_arr.resize(prediction_data.nrows);
                     }
                 }
 
                 ptr_worker->st  = 0;
                 ptr_worker->end = prediction_data.nrows - 1;
@@ -1272,54 +1278,54 @@
                         PredictionData        &prediction_data,
                         sparse_ix *restrict   tree_num,
                         double *restrict      per_tree_depths,
                         size_t                curr_tree,
                         bool                  has_range_penalty)
 {
     // if (trees[curr_tree].score >= 0)
-    if (trees[curr_tree].tree_left == 0)
+    if (unlikely(trees[curr_tree].tree_left == 0))
     {
         if (model_outputs.missing_action != Divide)
             for (size_t row = workspace.st; row <= workspace.end; row++)
                 workspace.depths[workspace.ix_arr[row]] += trees[curr_tree].score;
         else
             for (size_t row = workspace.st; row <= workspace.end; row++)
                 workspace.depths[workspace.ix_arr[row]] += workspace.weights_arr[workspace.ix_arr[row]] * trees[curr_tree].score;
-        if (tree_num != NULL)
+        if (unlikely(tree_num != NULL))
             for (size_t row = workspace.st; row <= workspace.end; row++)
                 tree_num[workspace.ix_arr[row]] = curr_tree;
-        if (per_tree_depths != NULL)
+        if (unlikely(per_tree_depths != NULL))
             for (size_t row = workspace.st; row <= workspace.end; row++)
                 per_tree_depths[workspace.ix_arr[row]] = trees[curr_tree].score;
         return;
     }
 
     /* in this case, the indices are sorted in the csc penalty function */
     if (!(has_range_penalty && model_outputs.missing_action != Divide && curr_tree > 0) && trees[curr_tree].col_type == Numeric)
         std::sort(workspace.ix_arr.begin() + workspace.st, workspace.ix_arr.begin() + workspace.end + 1);
 
     /* TODO: should mix the splitting function with the range penalty */
     
     /* divide according to tree */
     size_t orig_end = workspace.end;
     size_t st_NA, end_NA, split_ix;
-    switch(trees[curr_tree].col_type)
+    switch (trees[curr_tree].col_type)
     {
         case Numeric:
         {
             divide_subset_split(workspace.ix_arr.data(), workspace.st, workspace.end, trees[curr_tree].col_num,
                                 prediction_data.Xc, prediction_data.Xc_ind, prediction_data.Xc_indptr,
                                 trees[curr_tree].num_split, model_outputs.missing_action,
                                 st_NA, end_NA, split_ix);
             break;
         }
 
         case Categorical:
         {
-            switch(model_outputs.cat_split_type)
+            switch (model_outputs.cat_split_type)
             {
                 case SingleCateg:
                 {
                     divide_subset_split(workspace.ix_arr.data(),
                                         prediction_data.categ_data + prediction_data.nrows * trees[curr_tree].col_num,
                                         workspace.st, workspace.end, trees[curr_tree].chosen_cat,
                                          model_outputs.missing_action, st_NA, end_NA, split_ix);
@@ -1351,17 +1357,17 @@
         {
             assert(0);
             break;
         }
     }
 
     /* continue splitting recursively */
-    if (model_outputs.new_cat_action == Weighted)
+    if (unlikely(model_outputs.new_cat_action == Weighted && model_outputs.cat_split_type == SubSet && prediction_data.categ_data != NULL))
         goto missing_action_divide;
-    switch(model_outputs.missing_action)
+    switch (model_outputs.missing_action)
     {
         case Impute:
         {
             split_ix = (trees[curr_tree].pct_tree_left >= .5)? end_NA : st_NA;
         }
 
         case Fail:
@@ -1517,32 +1523,32 @@
                          PredictionData           &prediction_data,
                          sparse_ix *restrict      tree_num,
                          double *restrict         per_tree_depths,
                          size_t                   curr_tree,
                          bool                     has_range_penalty)
 {
     // if (hplanes[curr_tree].score >= 0)
-    if (hplanes[curr_tree].hplane_left == 0)
+    if (unlikely(hplanes[curr_tree].hplane_left == 0))
     {
         for (size_t row = workspace.st; row <= workspace.end; row++)
             workspace.depths[workspace.ix_arr[row]] += hplanes[curr_tree].score;
-        if (tree_num != NULL)
+        if (unlikely(tree_num != NULL))
             for (size_t row = workspace.st; row <= workspace.end; row++)
                 tree_num[workspace.ix_arr[row]] = curr_tree;
-        if (per_tree_depths != NULL)
+        if (unlikely(per_tree_depths != NULL))
             for (size_t row = workspace.st; row <= workspace.end; row++)
                 per_tree_depths[workspace.ix_arr[row]] = hplanes[curr_tree].score;
         return;
     }
 
     std::sort(workspace.ix_arr.begin() + workspace.st, workspace.ix_arr.begin() + workspace.end + 1);
     std::fill(workspace.comb_val.begin(), workspace.comb_val.begin() + (workspace.end - workspace.st + 1), 0.);
     double unused;
 
-    if (prediction_data.categ_data == NULL)
+    if (likely(prediction_data.categ_data == NULL))
     {
         for (size_t col = 0; col < hplanes[curr_tree].col_num.size(); col++)
             add_linear_comb(workspace.ix_arr.data(), workspace.st, workspace.end,
                             hplanes[curr_tree].col_num[col], workspace.comb_val.data(),
                             prediction_data.Xc, prediction_data.Xc_ind, prediction_data.Xc_indptr,
                             hplanes[curr_tree].coef[col], (double)0, hplanes[curr_tree].mean[col],
                             (model_outputs.missing_action == Fail)?  unused : hplanes[curr_tree].fill_val[col],
@@ -1551,15 +1557,15 @@
 
     else
     {
         size_t ncols_numeric = 0;
         size_t ncols_categ = 0;
         for (size_t col = 0; col < hplanes[curr_tree].col_num.size(); col++)
         {
-            switch(hplanes[curr_tree].col_type[col])
+            switch (hplanes[curr_tree].col_type[col])
             {
                 case Numeric:
                 {
                     add_linear_comb(workspace.ix_arr.data(), workspace.st, workspace.end,
                                     hplanes[curr_tree].col_num[col], workspace.comb_val.data(),
                                     prediction_data.Xc, prediction_data.Xc_ind, prediction_data.Xc_indptr,
                                     hplanes[curr_tree].coef[ncols_numeric], (double)0, hplanes[curr_tree].mean[ncols_numeric],
@@ -1657,18 +1663,18 @@
     {
         for (size_t *row = ptr_st;
              row != workspace.ix_arr.data() + workspace.end + 1 && curr_pos != end_col + 1 && ind_end_col >= *row;
             )
         {
             if (prediction_data.Xc_ind[curr_pos] == (decltype(*prediction_data.Xc_ind))(*row))
             {
-                if (!isnan(prediction_data.Xc[curr_pos])
-                        &&
-                    (   prediction_data.Xc[curr_pos] < range_low    ||
-                        prediction_data.Xc[curr_pos] > range_high   ))
+                if (likely(!isnan(prediction_data.Xc[curr_pos])
+                               &&
+                           (   prediction_data.Xc[curr_pos] < range_low    ||
+                               prediction_data.Xc[curr_pos] > range_high   )))
                 {
                     workspace.depths[*row] -= (weights_arr == NULL)? 1. : weights_arr[*row];
                 }
                 
                 if (row == workspace.ix_arr.data() + workspace.end || curr_pos == end_col) break;
                 curr_pos = std::lower_bound(prediction_data.Xc_ind + curr_pos + 1,
                                             prediction_data.Xc_ind + end_col  + 1,
@@ -1689,32 +1695,32 @@
                                     - prediction_data.Xc_ind;
             }
         }
     }
 
     else
     {
-        if (weights_arr == NULL)
+        if (likely(weights_arr == NULL))
             for (size_t row = workspace.st; row <= workspace.end; row++)
                 workspace.depths[workspace.ix_arr[row]]--;
         else
             for (size_t row = workspace.st; row <= workspace.end; row++)
                 workspace.depths[workspace.ix_arr[row]] -= weights_arr[workspace.ix_arr[row]];
 
 
         for (size_t *row = ptr_st;
              row != workspace.ix_arr.data() + workspace.end + 1 && curr_pos != end_col + 1 && ind_end_col >= *row;
             )
         {
             if (prediction_data.Xc_ind[curr_pos] == (decltype(*prediction_data.Xc_ind))(*row))
             {
-                if (isnan(prediction_data.Xc[curr_pos])
-                        ||
-                    (   prediction_data.Xc[curr_pos] >= range_low    &&
-                        prediction_data.Xc[curr_pos] <= range_high   ))
+                if (likely(isnan(prediction_data.Xc[curr_pos])
+                               ||
+                           (   prediction_data.Xc[curr_pos] >= range_low    &&
+                               prediction_data.Xc[curr_pos] <= range_high   )))
                 {
                     workspace.depths[*row] += (weights_arr == NULL)? 1. : weights_arr[*row];
                 }
                 
                 if (row == workspace.ix_arr.data() + workspace.end || curr_pos == end_col) break;
                 curr_pos = std::lower_bound(prediction_data.Xc_ind + curr_pos + 1,
                                             prediction_data.Xc_ind + end_col  + 1,
@@ -1735,15 +1741,15 @@
                                     - prediction_data.Xc_ind;
             }
         }
     }
 }
 
 template <class PredictionData>
-double extract_spC(PredictionData &prediction_data, size_t row, size_t col_num)
+double extract_spC(PredictionData &prediction_data, size_t row, size_t col_num) noexcept
 {
     decltype(prediction_data.Xc_indptr)
                search_res = std::lower_bound(prediction_data.Xc_ind + prediction_data.Xc_indptr[col_num],
                                              prediction_data.Xc_ind + prediction_data.Xc_indptr[col_num + 1],
                                              row);
     if (
         search_res == (prediction_data.Xc_ind + prediction_data.Xc_indptr[col_num + 1])
@@ -1752,48 +1758,47 @@
         )
         return 0.;
     else
         return prediction_data.Xc[search_res - prediction_data.Xc_ind];
 }
 
 template <class PredictionData, class sparse_ix>
-double extract_spR(PredictionData &prediction_data, sparse_ix *row_st, sparse_ix *row_end, size_t col_num)
+double extract_spR(PredictionData &prediction_data, sparse_ix *row_st, sparse_ix *row_end, size_t col_num) noexcept
 {
     if (row_end == row_st)
         return 0.;
     sparse_ix *search_res = std::lower_bound(row_st, row_end, (sparse_ix) col_num);
     if (search_res == row_end || *search_res != (sparse_ix)col_num)
         return 0.;
     else
         return prediction_data.Xr[search_res - prediction_data.Xr_ind];
 }
 
 template <class sparse_ix>
-void get_num_nodes(IsoForest &model_outputs, sparse_ix *restrict n_nodes, sparse_ix *restrict n_terminal, int nthreads)
+void get_num_nodes(IsoForest &model_outputs, sparse_ix *restrict n_nodes, sparse_ix *restrict n_terminal, int nthreads) noexcept
 {
     std::fill(n_terminal, n_terminal + model_outputs.trees.size(), 0);
     #pragma omp parallel for schedule(static) num_threads(nthreads) shared(model_outputs, n_nodes, n_terminal)
     for (size_t_for tree = 0; tree < (decltype(tree))model_outputs.trees.size(); tree++)
     {
         n_nodes[tree] = model_outputs.trees[tree].size();
         for (IsoTree &node : model_outputs.trees[tree])
         {
             n_terminal[tree] += (node.tree_left == 0);
         }
     }
 }
 
 template <class sparse_ix>
-void get_num_nodes(ExtIsoForest &model_outputs, sparse_ix *restrict n_nodes, sparse_ix *restrict n_terminal, int nthreads)
+void get_num_nodes(ExtIsoForest &model_outputs, sparse_ix *restrict n_nodes, sparse_ix *restrict n_terminal, int nthreads) noexcept
 {
     std::fill(n_terminal, n_terminal + model_outputs.hplanes.size(), 0);
     #pragma omp parallel for schedule(static) num_threads(nthreads) shared(model_outputs, n_nodes, n_terminal)
     for (size_t_for hplane = 0; hplane <(decltype(hplane)) model_outputs.hplanes.size(); hplane++)
     {
         n_nodes[hplane] = model_outputs.hplanes[hplane].size();
         for (IsoHPlane &node : model_outputs.hplanes[hplane])
         {
             n_terminal[hplane] += (node.hplane_left == 0);
         }
     }
 }
-
```

### Comparing `isotree-0.5.8.post1/src/python_helpers.hpp` & `isotree-0.5.9/src/python_helpers.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 *          arXiv preprint arXiv:2110.13402 (2021).
 *     [12] Guha, Sudipto, et al.
 *          "Robust random cut forest based anomaly detection on streams."
 *          International conference on machine learning. PMLR, 2016.
 *     [13] Cortes, David.
 *          "Isolation forests: looking beyond tree depth."
 *          arXiv preprint arXiv:2111.11639 (2021).
+*     [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou.
+*          "Isolation kernel and its effect on SVM"
+*          Proceedings of the 24th ACM SIGKDD
+*          International Conference on Knowledge Discovery & Data Mining. 2018.
 * 
 *     BSD 2-Clause License
 *     Copyright (c) 2019-2022, David Cortes
 *     All rights reserved.
 *     Redistribution and use in source and binary forms, with or without
 *     modification, are permitted provided that the following conditions are met:
 *     * Redistributions of source code must retain the above copyright notice, this
```

### Comparing `isotree-0.5.8.post1/src/robinmap/LICENSE` & `isotree-0.5.9/src/robinmap/LICENSE`

 * *Files identical despite different names*

### Comparing `isotree-0.5.8.post1/src/robinmap/include/tsl/robin_growth_policy.h` & `isotree-0.5.9/src/robinmap/include/tsl/robin_growth_policy.h`

 * *Files identical despite different names*

### Comparing `isotree-0.5.8.post1/src/robinmap/include/tsl/robin_hash.h` & `isotree-0.5.9/src/robinmap/include/tsl/robin_hash.h`

 * *Files identical despite different names*

### Comparing `isotree-0.5.8.post1/src/robinmap/include/tsl/robin_map.h` & `isotree-0.5.9/src/robinmap/include/tsl/robin_map.h`

 * *Files identical despite different names*

### Comparing `isotree-0.5.8.post1/src/robinmap/include/tsl/robin_set.h` & `isotree-0.5.9/src/robinmap/include/tsl/robin_set.h`

 * *Files identical despite different names*

### Comparing `isotree-0.5.8.post1/src/serialize.cpp` & `isotree-0.5.9/src/serialize.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 *          arXiv preprint arXiv:2110.13402 (2021).
 *     [12] Guha, Sudipto, et al.
 *          "Robust random cut forest based anomaly detection on streams."
 *          International conference on machine learning. PMLR, 2016.
 *     [13] Cortes, David.
 *          "Isolation forests: looking beyond tree depth."
 *          arXiv preprint arXiv:2111.11639 (2021).
+*     [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou.
+*          "Isolation kernel and its effect on SVM"
+*          Proceedings of the 24th ACM SIGKDD
+*          International Conference on Knowledge Discovery & Data Mining. 2018.
 * 
 *     BSD 2-Clause License
 *     Copyright (c) 2019-2022, David Cortes
 *     All rights reserved.
 *     Redistribution and use in source and binary forms, with or without
 *     modification, are permitted provided that the following conditions are met:
 *     * Redistributions of source code must retain the above copyright notice, this
@@ -166,170 +170,170 @@
     HasExtModelPlusImputerPlusMetadataNext=9,
     HasExtModelPlusImputerPlusIndexerPlusMetadataNext=19,
     HasMoreTreesNext=10
 };
 
 #ifdef _MSC_VER
 #include <stdlib.h>
-void swap16b(char *bytes)
+void swap16b(char *bytes) noexcept
 {
     if (std::numeric_limits<unsigned short>::max() == UINT16_MAX) {
         unsigned short temp;
         memcpy(&temp, bytes, sizeof(unsigned short));
         temp = _byteswap_ushort(temp);
         memcpy(bytes, &temp, sizeof(unsigned short));
     }
     
     else {
         std::swap(bytes[0], bytes[1]);
     }
 }
-void swap32b(char *bytes)
+void swap32b(char *bytes) noexcept
 {
     if (std::numeric_limits<unsigned long>::max() == UINT32_MAX) {
         unsigned long temp;
         memcpy(&temp, bytes, sizeof(unsigned long));
         temp = _byteswap_ulong(temp);
         memcpy(bytes, &temp, sizeof(unsigned long));
     }
     
     else {
         std::swap(bytes[0], bytes[3]);
         std::swap(bytes[1], bytes[2]);
     }
 }
-void swap64b(char *bytes)
+void swap64b(char *bytes) noexcept
 {
     unsigned __int64 temp;
     memcpy(&temp, bytes, sizeof(unsigned __int64));
     temp = _byteswap_uint64(temp);
     memcpy(bytes, &temp, sizeof(unsigned __int64));
 }
 #elif defined(__GNUC__) && (__GNUC__ >= 5) && !defined(_WIN32)
-void swap16b(char *bytes)
+void swap16b(char *bytes) noexcept
 {
     uint16_t temp;
     memcpy(&temp, bytes, sizeof(uint16_t));
     temp = __builtin_bswap16(temp);
     memcpy(bytes, &temp, sizeof(uint16_t));
 }
-void swap32b(char *bytes)
+void swap32b(char *bytes) noexcept
 {
     uint32_t temp;
     memcpy(&temp, bytes, sizeof(uint32_t));
     temp = __builtin_bswap32(temp);
     memcpy(bytes, &temp, sizeof(uint32_t));
 }
-void swap64b(char *bytes)
+void swap64b(char *bytes) noexcept
 {
     uint64_t temp;
     memcpy(&temp, bytes, sizeof(uint64_t));
     temp = __builtin_bswap64(temp);
     memcpy(bytes, &temp, sizeof(uint64_t));
 }
 #else
-void swap16b(char *bytes)
+void swap16b(char *bytes) noexcept
 {
     std::swap(bytes[0], bytes[1]);
 }
-void swap32b(char *bytes)
+void swap32b(char *bytes) noexcept
 {
     std::swap(bytes[0], bytes[3]);
     std::swap(bytes[1], bytes[2]);
 }
-void swap64b(char *bytes)
+void swap64b(char *bytes) noexcept
 {
     std::swap(bytes[0], bytes[7]);
     std::swap(bytes[1], bytes[6]);
     std::swap(bytes[2], bytes[5]);
     std::swap(bytes[3], bytes[4]);
 }
 #endif
-void endian_swap(float &bytes)
+void endian_swap(float &bytes) noexcept
 {
     #ifdef HAS_IEEE_DOUBLE
     swap32b((char*)&bytes);
     #else
     std::reverse((char*)&bytes, (char*)&bytes + sizeof(float));
     #endif
 }
-void endian_swap(double &bytes)
+void endian_swap(double &bytes) noexcept
 {
     #ifdef HAS_IEEE_DOUBLE
     swap64b((char*)&bytes);
     #else
     std::reverse((char*)&bytes, (char*)&bytes + sizeof(double));
     #endif
 }
-void endian_swap(uint8_t &bytes)
+void endian_swap(uint8_t &bytes) noexcept
 {
     return;
 }
-void endian_swap(uint16_t &bytes)
+void endian_swap(uint16_t &bytes) noexcept
 {
     swap16b((char*)&bytes);
 }
-void endian_swap(uint32_t &bytes)
+void endian_swap(uint32_t &bytes) noexcept
 {
     swap32b((char*)&bytes);
 }
-void endian_swap(uint64_t &bytes)
+void endian_swap(uint64_t &bytes) noexcept
 {
     swap64b((char*)&bytes);
 }
-void endian_swap(int8_t &bytes)
+void endian_swap(int8_t &bytes) noexcept
 {
     return;
 }
-void endian_swap(int16_t &bytes)
+void endian_swap(int16_t &bytes) noexcept
 {
     swap16b((char*)&bytes);
 }
-void endian_swap(int32_t &bytes)
+void endian_swap(int32_t &bytes) noexcept
 {
     swap32b((char*)&bytes);
 }
-void endian_swap(int64_t &bytes)
+void endian_swap(int64_t &bytes) noexcept
 {
     swap64b((char*)&bytes);
 }
 /* Note: on macOS, some compilers will  take 'size_t' as different from 'uin64_t',
    hence it needs a separate one. However, in other compiler and platforms this
    leads to a a duplicated function definition, and thus needs this separation
    in names (otherwise, compilers such as GCC will not compile it). */
-void endian_swap_size_t(char *bytes)
+void endian_swap_size_t(char *bytes) noexcept
 {
     #if (SIZE_MAX == UINT32_MAX)
     swap32b(bytes);
     #elif (SIZE_MAX == UINT64_MAX)
     swap64b(bytes);
     #else
     std::reverse(bytes, bytes + sizeof(size_t));
     #endif
 }
-void endian_swap_int(char *bytes)
+void endian_swap_int(char *bytes) noexcept
 {
     #if (INT_MAX == INT16_MAX)
     swap16b(bytes);
     #elif (INT_MAX == INT32_MAX)
     swap32b(bytes);
     #elif (SIZE_MAX == INT64_MAX)
     swap64b(bytes);
     #else
     std::reverse(bytes, bytes + sizeof(int));
     #endif
 }
 template <class T>
-void endian_swap(T &bytes)
+void endian_swap(T &bytes) noexcept
 {
     std::reverse((char*)&bytes, (char*)&bytes + sizeof(T));
 }
 
 template <class dtype>
-void swap_endianness(dtype *ptr, size_t n_els)
+void swap_endianness(dtype *ptr, size_t n_els) noexcept
 {
     #ifndef __GNUC__
     if (std::is_same<dtype, size_t>::value)
     {
         for (size_t ix = 0; ix < n_els; ix++)
             endian_swap_size_t((char*)&ptr[ix]);
         return;
@@ -343,20 +347,20 @@
     }
     #endif
 
     for (size_t ix = 0; ix < n_els; ix++)
         endian_swap(ptr[ix]);
 }
 
-const char* set_return_position(const char *in)
+const char* set_return_position(const char *in) noexcept
 {
     return in;
 }
 
-char* set_return_position(char *in)
+char* set_return_position(char *in) noexcept
 {
     return in;
 }
 
 fpos_t_ set_return_position(FILE *in)
 {
     return ftell_(in);
@@ -370,20 +374,20 @@
 }
 
 pos_type_istream set_return_position(std::ostream &in)
 {
     return in.tellp();
 }
 
-void return_to_position(const char *&in, const char *saved_position)
+void return_to_position(const char *&in, const char *saved_position) noexcept
 {
     in = saved_position;
 }
 
-void return_to_position(char *&in, char *saved_position)
+void return_to_position(char *&in, char *saved_position) noexcept
 {
     in = saved_position;
 }
 
 void return_to_position(FILE *&in, fpos_t_ saved_position)
 {
     fseek_(in, saved_position, SEEK_SET);
@@ -396,15 +400,15 @@
 
 void return_to_position(std::ostream &in, pos_type_istream saved_position)
 {
     in.seekp(saved_position);
 }
 
 
-bool has_wchar_t_file_serializers()
+bool has_wchar_t_file_serializers()  noexcept
 {
     #ifdef WCHAR_T_FUNS
     return true;
     #else
     return false;
     #endif
 }
@@ -432,153 +436,153 @@
     saved_type *ptr_read = (saved_type*)buffer.data();
 
     if ((sizeof(dtype) <= sizeof(saved_type)) &&
         (saved_type)std::numeric_limits<dtype>::max() < std::numeric_limits<saved_type>::max())
     {
         const saved_type maxval = (saved_type) std::numeric_limits<dtype>::max();
         for (size_t el = 0; el < n_els; el++)
-            if (ptr_read[el] > maxval)
+            if (unlikely(ptr_read[el] > maxval))
                 throw std::runtime_error("Error: serialized model has values too large for the current machine's types.\n");
     }
 
     for (size_t el = 0; el < n_els; el++)
         ptr_write[el] = (dtype)ptr_read[el];
 }
 
 template <class dtype>
-void write_bytes(const void *ptr, const size_t n_els, char *&out)
+void write_bytes(const void *ptr, const size_t n_els, char *&out) noexcept
 {
     if (n_els == 0) return;
     memcpy(out, ptr, n_els * sizeof(dtype));
     out += n_els * sizeof(dtype);
 }
 
 template <class dtype>
 void write_bytes(const void *ptr, const size_t n_els, std::ostream &out)
 {
     if (n_els == 0) return;
     out.write((char*)ptr, n_els * sizeof(dtype));
-    if (out.bad()) throw_errno();
+    if (unlikely(out.bad())) throw_errno();
 }
 
 template <class dtype>
 void write_bytes(const void *ptr, const size_t n_els, FILE *&out)
 {
     if (n_els == 0) return;
     size_t n_written = fwrite(ptr, sizeof(dtype), n_els, out);
     if (n_written != n_els || ferror(out)) throw_ferror(out);
 }
 
 template <class dtype>
-void read_bytes(void *ptr, const size_t n_els, const char *&in)
+void read_bytes(void *ptr, const size_t n_els, const char *&in) noexcept
 {
     if (n_els == 0) return;
     memcpy(ptr, in, n_els * sizeof(dtype));
     in += n_els * sizeof(dtype);
 }
 
 template <class dtype, class saved_type>
 void read_bytes(void *ptr, const size_t n_els, const char *&in, std::vector<char> &buffer, const bool diff_endian)
 {
     if (std::is_same<dtype, saved_type>::value)
     {
         read_bytes<dtype>(ptr, n_els, in);
-        if (diff_endian) swap_endianness((dtype*)ptr, n_els);
+        if (unlikely(diff_endian)) swap_endianness((dtype*)ptr, n_els);
         return;
     }
     if (n_els == 0) return;
-    if (buffer.size() < n_els * sizeof(saved_type))
+    if (unlikely(buffer.size() < n_els * sizeof(saved_type)))
         buffer.resize((size_t)2 * n_els * sizeof(saved_type));
     memcpy(buffer.data(), in, n_els * sizeof(saved_type));
     in += n_els * sizeof(saved_type);
 
-    if (diff_endian) swap_endianness((saved_type*)buffer.data(), n_els);
+    if (unlikely(diff_endian)) swap_endianness((saved_type*)buffer.data(), n_els);
     convert_dtype<dtype, saved_type>(ptr, buffer, n_els);
 }
 
 template <class dtype>
-void read_bytes(void *ptr, const size_t n_els, char *&in)
+void read_bytes(void *ptr, const size_t n_els, char *&in) noexcept
 {
     if (n_els == 0) return;
     memcpy(ptr, in, n_els * sizeof(dtype));
     in += n_els * sizeof(dtype);
 }
 
 template <class dtype, class saved_type>
 void read_bytes(void *ptr, const size_t n_els, char *&in, std::vector<char> &buffer, const bool diff_endian)
 {
     if (std::is_same<dtype, saved_type>::value)
     {
         read_bytes<dtype>(ptr, n_els, in);
-        if (diff_endian) swap_endianness((dtype*)ptr, n_els);
+        if (unlikely(diff_endian)) swap_endianness((dtype*)ptr, n_els);
         return;
     }
     if (n_els == 0) return;
-    if (buffer.size() < n_els * sizeof(saved_type))
+    if (unlikely(buffer.size() < n_els * sizeof(saved_type)))
         buffer.resize((size_t)2 * n_els * sizeof(saved_type));
     memcpy(buffer.data(), in, n_els * sizeof(saved_type));
     in += n_els * sizeof(saved_type);
 
-    if (diff_endian) swap_endianness((saved_type*)buffer.data(), n_els);
+    if (unlikely(diff_endian)) swap_endianness((saved_type*)buffer.data(), n_els);
     convert_dtype<dtype, saved_type>(ptr, buffer, n_els);
 }
 
 template <class dtype>
 void read_bytes(void *ptr, const size_t n_els, std::istream &in)
 {
     if (n_els == 0) return;
     in.read((char*)ptr, n_els * sizeof(dtype));
-    if (in.bad()) throw_errno();
+    if (unlikely(in.bad())) throw_errno();
 }
 
 template <class dtype, class saved_type>
 void read_bytes(void *ptr, const size_t n_els, std::istream &in, std::vector<char> &buffer, const bool diff_endian)
 {
     if (std::is_same<dtype, saved_type>::value)
     {
         read_bytes<dtype>(ptr, n_els, in);
-        if (diff_endian) swap_endianness((dtype*)ptr, n_els);
+        if (unlikely(diff_endian)) swap_endianness((dtype*)ptr, n_els);
         return;
     }
     if (n_els == 0) return;
-    if (buffer.size() < n_els * sizeof(saved_type))
+    if (unlikely(buffer.size() < n_els * sizeof(saved_type)))
         buffer.resize((size_t)2 * n_els * sizeof(saved_type));
     in.read((char*)buffer.data(), n_els * sizeof(saved_type));
-    if (in.bad()) throw_errno();
+    if (unlikely(in.bad())) throw_errno();
 
-    if (diff_endian) swap_endianness((saved_type*)buffer.data(), n_els);
+    if (unlikely(diff_endian)) swap_endianness((saved_type*)buffer.data(), n_els);
     convert_dtype<dtype, saved_type>(ptr, buffer, n_els);
 }
 
 template <class dtype>
 void read_bytes(void *ptr, const size_t n_els, FILE *&in)
 {
     if (n_els == 0) return;
-    if (feof(in)) throw_feoferr();
+    if (unlikely(feof(in))) throw_feoferr();
     size_t n_read = fread(ptr, sizeof(dtype), n_els, in);
-    if (n_read != n_els || ferror(in)) throw_ferror(in);
+    if (unlikely(n_read != n_els || ferror(in))) throw_ferror(in);
 }
 
 template <class dtype, class saved_type>
 void read_bytes(void *ptr, const size_t n_els, FILE *&in, std::vector<char> &buffer, const bool diff_endian)
 {
     if (std::is_same<dtype, saved_type>::value)
     {
         read_bytes<dtype>(ptr, n_els, in);
-        if (diff_endian) swap_endianness((dtype*)ptr, n_els);
+        if (unlikely(diff_endian)) swap_endianness((dtype*)ptr, n_els);
         return;
     }
     if (n_els == 0) return;
-    if (feof(in)) throw_feoferr();
-    if (buffer.size() < n_els * sizeof(saved_type))
+    if (unlikely(feof(in))) throw_feoferr();
+    if (unlikely(buffer.size() < n_els * sizeof(saved_type)))
         buffer.resize((size_t)2 * n_els * sizeof(saved_type));
     size_t n_read = fread(buffer.data(), sizeof(saved_type), n_els, in);
-    if (n_read != n_els || ferror(in)) throw_ferror(in);
+    if (unlikely(n_read != n_els || ferror(in))) throw_ferror(in);
 
-    if (diff_endian) swap_endianness((saved_type*)buffer.data(), n_els);
+    if (unlikely(diff_endian)) swap_endianness((saved_type*)buffer.data(), n_els);
     convert_dtype<dtype, saved_type>(ptr, buffer, n_els);
 }
 
 template <class dtype>
 void read_bytes(std::vector<dtype> &vec, const size_t n_els, const char *&in)
 {
     if (n_els)
@@ -591,25 +595,25 @@
 
 template <class dtype, class saved_type>
 void read_bytes(std::vector<dtype> &vec, const size_t n_els, const char *&in, std::vector<char> &buffer, const bool diff_endian)
 {
     if (std::is_same<dtype, saved_type>::value)
     {
         read_bytes<dtype>(vec, n_els, in);
-        if (diff_endian) swap_endianness(vec.data(), n_els);
+        if (unlikely(diff_endian)) swap_endianness(vec.data(), n_els);
         return;
     }
     if (n_els) {
-        if (buffer.size() < n_els * sizeof(saved_type))
+        if (unlikely(buffer.size() < n_els * sizeof(saved_type)))
             buffer.resize((size_t)2 * n_els * sizeof(saved_type));
         read_bytes<saved_type>(buffer.data(), n_els, in);
         vec.resize(n_els);
         vec.shrink_to_fit();
         
-        if (diff_endian) swap_endianness((saved_type*)buffer.data(), n_els);
+        if (unlikely(diff_endian)) swap_endianness((saved_type*)buffer.data(), n_els);
         convert_dtype<dtype, saved_type>(vec.data(), buffer, n_els);
     }
     
     else {
         vec.clear();
         vec.shrink_to_fit();
     }
@@ -621,80 +625,80 @@
 void read_bytes(std::vector<dtype> &vec, const size_t n_els, std::istream &in)
 {
     vec.resize(n_els);
     vec.shrink_to_fit();
 
     if (n_els) {
         in.read((char*)vec.data(), n_els * sizeof(dtype));
-        if (in.bad()) throw_errno();
+        if (unlikely(in.bad())) throw_errno();
     }
 }
 
 template <class dtype, class saved_type>
 void read_bytes(std::vector<dtype> &vec, const size_t n_els, std::istream &in, std::vector<char> &buffer, const bool diff_endian)
 {
     if (std::is_same<dtype, saved_type>::value)
     {
         read_bytes<dtype>(vec, n_els, in);
-        if (diff_endian) swap_endianness(vec.data(), n_els);
+        if (unlikely(diff_endian)) swap_endianness(vec.data(), n_els);
         return;
     }
     vec.resize(n_els);
     vec.shrink_to_fit();
 
     if (n_els) {
-        if (buffer.size() < n_els * sizeof(saved_type))
+        if (unlikely(buffer.size() < n_els * sizeof(saved_type)))
             buffer.resize((size_t)2 * n_els * sizeof(saved_type));
         in.read(buffer.data(), n_els * sizeof(saved_type));
-        if (in.bad()) throw_errno();
+        if (unlikely(in.bad())) throw_errno();
 
-        if (diff_endian) swap_endianness((saved_type*)buffer.data(), n_els);
+        if (unlikely(diff_endian)) swap_endianness((saved_type*)buffer.data(), n_els);
         convert_dtype<dtype, saved_type>(vec.data(), buffer, n_els);
     }
 }
 
 template <class dtype>
 void read_bytes(std::vector<dtype> &vec, const size_t n_els, FILE *&in)
 {
     vec.resize(n_els);
     vec.shrink_to_fit();
     
     if (n_els) {
-        if (feof(in)) throw_feoferr();
+        if (unlikely(feof(in))) throw_feoferr();
         size_t n_read = fread(vec.data(), sizeof(dtype), n_els, in);
-        if (n_read != n_els || ferror(in)) throw_ferror(in);
+        if (unlikely(n_read != n_els || ferror(in))) throw_ferror(in);
     }
 }
 
 template <class dtype, class saved_type>
 void read_bytes(std::vector<dtype> &vec, const size_t n_els, FILE *&in, std::vector<char> &buffer, const bool diff_endian)
 {
     if (std::is_same<dtype, saved_type>::value)
     {
         read_bytes<dtype>(vec, n_els, in);
-        if (diff_endian) swap_endianness(vec.data(), n_els);
+        if (unlikely(diff_endian)) swap_endianness(vec.data(), n_els);
         return;
     }
     vec.resize(n_els);
     vec.shrink_to_fit();
 
     if (n_els) {
-        if (feof(in)) throw_feoferr();
-        if (buffer.size() < n_els * sizeof(saved_type))
+        if (unlikely(feof(in))) throw_feoferr();
+        if (unlikely(buffer.size() < n_els * sizeof(saved_type)))
             buffer.resize((size_t)2 * n_els * sizeof(saved_type));
 
         size_t n_read = fread(buffer.data(), sizeof(saved_type), n_els, in);
-        if (n_read != n_els || ferror(in)) throw_ferror(in);
+        if (unlikely(n_read != n_els || ferror(in))) throw_ferror(in);
 
-        if (diff_endian) swap_endianness((saved_type*)buffer.data(), n_els);
+        if (unlikely(diff_endian)) swap_endianness((saved_type*)buffer.data(), n_els);
         convert_dtype<dtype, saved_type>(vec.data(), buffer, n_els);
     }
 }
 
-size_t get_size_node(const IsoTree &node)
+size_t get_size_node(const IsoTree &node) noexcept
 {
     size_t n_bytes = 0;
     n_bytes += sizeof(uint8_t);
     n_bytes += sizeof(int);
     n_bytes += sizeof(double) * 6;
     n_bytes += sizeof(size_t) * 4;
     n_bytes += sizeof(signed char) * node.cat_split.size();
@@ -785,15 +789,15 @@
     read_bytes<size_t, saved_size_t>((void*)data_sizets, (size_t)4, in, buffer, diff_endian);
     node.col_num = data_sizets[0];
     node.tree_left = data_sizets[1];
     node.tree_right = data_sizets[2];
     read_bytes<signed char, signed char>(node.cat_split, data_sizets[3], in, buffer, diff_endian);
 }
 
-size_t get_size_node(const IsoHPlane &node)
+size_t get_size_node(const IsoHPlane &node) noexcept
 {
     size_t n_bytes = 0;
     n_bytes += sizeof(double) * 5;
     n_bytes += sizeof(size_t) * 10;
     n_bytes += sizeof(size_t) * node.col_num.size();
     if (node.col_type.size()) {
         n_bytes += sizeof(uint8_t)*node.col_type.size();
@@ -970,15 +974,15 @@
     read_bytes<int, saved_int_t>(node.chosen_cat, data_sizets[7], in, buffer2, diff_endian);
 
     read_bytes<double, double>(node.fill_val, data_sizets[8], in, buffer2, diff_endian);
 
     read_bytes<double, double>(node.fill_new, data_sizets[9], in, buffer2, diff_endian);
 }
 
-size_t get_size_node(const ImputeNode &node)
+size_t get_size_node(const ImputeNode &node) noexcept
 {
     size_t n_bytes = 0;
     n_bytes += sizeof(size_t) * 5;
     n_bytes += sizeof(double) * node.num_sum.size();
     n_bytes += sizeof(double) * node.num_weight.size();
     if (node.cat_sum.size()) {
         for (const auto &v : node.cat_sum) {
@@ -1068,15 +1072,15 @@
         }
     }
     node.cat_sum.shrink_to_fit();
 
     read_bytes<double, double>(node.cat_weight, data_sizets[4], in, buffer, diff_endian);
 }
 
-size_t get_size_node(const SingleTreeIndex &node)
+size_t get_size_node(const SingleTreeIndex &node) noexcept
 {
     size_t n_bytes = 0;
     n_bytes += sizeof(size_t);
     n_bytes += node.terminal_node_mappings.size() * sizeof(size_t);
     n_bytes += sizeof(size_t);
     n_bytes += node.node_distances.size() * sizeof(double);
     n_bytes += sizeof(size_t);
@@ -1180,15 +1184,15 @@
 
     read_bytes<size_t, saved_size_t>((void*)&vec_size, (size_t)1, in, buffer, diff_endian);
     read_bytes<size_t, saved_size_t>(node.reference_mapping, vec_size, in, buffer, diff_endian);
 
     read_bytes<size_t, saved_size_t>((void*)&node.n_terminal, (size_t)1, in, buffer, diff_endian);
 }
 
-size_t get_size_model(const IsoForest &model)
+size_t get_size_model(const IsoForest &model) noexcept
 {
     size_t n_bytes = 0;
     n_bytes += sizeof(uint8_t) * 5;
     n_bytes += sizeof(double) * 2;
     n_bytes += sizeof(size_t) * 2;
     for (const auto &tree : model.trees) {
         n_bytes += sizeof(size_t);
@@ -1334,26 +1338,26 @@
         veclen = model.trees[ix].size();
         write_bytes<size_t>((void*)&veclen, (size_t)1, out);
         for (const auto &node : model.trees[ix])
             serialize_node(node, out);
     }
 }
 
-size_t determine_serialized_size_additional_trees(const IsoForest &model, size_t old_ntrees)
+size_t determine_serialized_size_additional_trees(const IsoForest &model, size_t old_ntrees) noexcept
 {
     size_t n_bytes = 0;
     for (size_t ix = 0; ix < model.trees.size(); ix++) {
         n_bytes += sizeof(size_t);
         for (const auto &node : model.trees[ix])
             n_bytes += get_size_node(node);
     }
     return n_bytes;
 }
 
-size_t get_size_model(const ExtIsoForest &model)
+size_t get_size_model(const ExtIsoForest &model) noexcept
 {
     size_t n_bytes = 0;
     n_bytes += sizeof(uint8_t) * 5;
     n_bytes += sizeof(double) * 2;
     n_bytes += sizeof(size_t) * 2;
     for (const auto &tree : model.hplanes) {
         n_bytes += sizeof(size_t);
@@ -1505,26 +1509,26 @@
         veclen = model.hplanes[ix].size();
         write_bytes<size_t>((void*)&veclen, (size_t)1, out);
         for (const auto &node : model.hplanes[ix])
             serialize_node(node, out, buffer);
     }
 }
 
-size_t determine_serialized_size_additional_trees(const ExtIsoForest &model, size_t old_ntrees)
+size_t determine_serialized_size_additional_trees(const ExtIsoForest &model, size_t old_ntrees) noexcept
 {
     size_t n_bytes = 0;
     for (size_t ix = 0; ix < model.hplanes.size(); ix++) {
         n_bytes += sizeof(size_t);
         for (const auto &node : model.hplanes[ix])
             n_bytes += get_size_node(node);
     }
     return n_bytes;
 }
 
-size_t get_size_model(const Imputer &model)
+size_t get_size_model(const Imputer &model) noexcept
 {
     size_t n_bytes = 0;
     n_bytes += sizeof(size_t) * 6;
     n_bytes += sizeof(int) * model.ncat.size();
     n_bytes += sizeof(double) * model.col_means.size();
     n_bytes += sizeof(int) * model.col_modes.size();
     for (const auto &tree : model.imputer_tree) {
@@ -1645,26 +1649,26 @@
         veclen = model.imputer_tree[ix].size();
         write_bytes<size_t>((void*)&veclen, (size_t)1, out);
         for (const auto &node : model.imputer_tree[ix])
             serialize_node(node, out);
     }
 }
 
-size_t determine_serialized_size_additional_trees(const Imputer &model, size_t old_ntrees)
+size_t determine_serialized_size_additional_trees(const Imputer &model, size_t old_ntrees) noexcept
 {
     size_t n_bytes = 0;
     for (size_t ix = 0; ix < model.imputer_tree.size(); ix++) {
         n_bytes += sizeof(size_t);
         for (const auto &node : model.imputer_tree[ix])
             n_bytes += get_size_node(node);
     }
     return n_bytes;
 }
 
-size_t get_size_model(const TreesIndexer &model)
+size_t get_size_model(const TreesIndexer &model) noexcept
 {
     size_t n_bytes = 0;
     n_bytes += sizeof(size_t);
     for (const auto &node : model.indices)
         n_bytes += get_size_node(node);
     return n_bytes;
 }
@@ -1712,29 +1716,29 @@
 template <class otype>
 void serialize_additional_trees(const TreesIndexer &model, otype &out, size_t trees_prev)
 {
     for (size_t ix = trees_prev; ix < model.indices.size(); ix++)
         serialize_node(model.indices[ix], out);
 }
 
-size_t determine_serialized_size_additional_trees(const TreesIndexer &model, size_t old_ntrees)
+size_t determine_serialized_size_additional_trees(const TreesIndexer &model, size_t old_ntrees) noexcept
 {
     size_t n_bytes = 0;
     for (size_t ix = 0; ix < model.indices.size(); ix++)
         n_bytes += get_size_node(model.indices[ix]);
     return n_bytes;
 }
 
-bool get_is_little_endian()
+bool get_is_little_endian() noexcept
 {
     const int one = 1;
     return *((unsigned char*)&one) != 0;
 }
 
-size_t get_size_setup_info()
+size_t get_size_setup_info() noexcept
 {
     size_t n_bytes = 0;
     n_bytes += sizeof(unsigned char) * SIZE_WATERMARK;
     n_bytes += sizeof(uint8_t) * 9;
     return n_bytes;
 }
 
@@ -1997,50 +2001,50 @@
     }
     if (!has_same_double)
         throw std::runtime_error("Error: input model was saved in a machine with different 'double' type.\n");
     if (!is_deserializable)
         throw std::runtime_error("Error: input format is incompatible.\n");
 }
 
-size_t get_size_ending_metadata()
+size_t get_size_ending_metadata() noexcept
 {
     size_t n_bytes = 0;
     n_bytes += sizeof(uint8_t);
     n_bytes += sizeof(size_t);
     return n_bytes;
 }
 
 template <class Model>
-size_t determine_serialized_size(const Model &model)
+size_t determine_serialized_size(const Model &model) noexcept
 {
     size_t n_bytes = 0;
     n_bytes += get_size_setup_info();
     n_bytes += sizeof(uint8_t);
     n_bytes += sizeof(size_t);
     n_bytes += get_size_model(model);
     n_bytes += get_size_ending_metadata();
     return n_bytes;
 }
 
-uint8_t get_model_code(const IsoForest &model)
+uint8_t get_model_code(const IsoForest &model) noexcept
 {
     return IsoForestModel;
 }
 
-uint8_t get_model_code(const ExtIsoForest &model)
+uint8_t get_model_code(const ExtIsoForest &model) noexcept
 {
     return ExtIsoForestModel;
 }
 
-uint8_t get_model_code(const Imputer &model)
+uint8_t get_model_code(const Imputer &model) noexcept
 {
     return ImputerModel;
 }
 
-uint8_t get_model_code(const TreesIndexer &model)
+uint8_t get_model_code(const TreesIndexer &model) noexcept
 {
     return IndexerModel;
 }
 
 template <class Model, class otype>
 void serialization_pipeline(const Model &model, otype &out)
 {
@@ -2511,30 +2515,30 @@
 void serialization_pipeline_ToFile(const Model &model, const wchar_t *fname)
 {
     WFileHandle f(fname, L"wb");
     serialization_pipeline(model, f.handle);
 }
 #endif
 
-size_t determine_serialized_size(const IsoForest &model)
+size_t determine_serialized_size(const IsoForest &model) noexcept
 {
     return determine_serialized_size<IsoForest>(model);
 }
 
-size_t determine_serialized_size(const ExtIsoForest &model)
+size_t determine_serialized_size(const ExtIsoForest &model) noexcept
 {
     return determine_serialized_size<ExtIsoForest>(model);
 }
 
-size_t determine_serialized_size(const Imputer &model)
+size_t determine_serialized_size(const Imputer &model) noexcept
 {
     return determine_serialized_size<Imputer>(model);
 }
 
-size_t determine_serialized_size(const TreesIndexer &model)
+size_t determine_serialized_size(const TreesIndexer &model) noexcept
 {
     return determine_serialized_size<TreesIndexer>(model);
 }
 
 void serialize_IsoForest(const IsoForest &model, char *out)
 {
     serialization_pipeline(model, out);
@@ -3446,15 +3450,15 @@
 size_t determine_serialized_size_combined
 (
     const IsoForest *model,
     const ExtIsoForest *model_ext,
     const Imputer *imputer,
     const TreesIndexer *indexer,
     const size_t size_optional_metadata
-)
+) noexcept
 {
     size_t n_bytes = get_size_setup_info();
     n_bytes += 3 * sizeof(uint8_t);
     n_bytes += 5 * sizeof(size_t);
 
     if (model != NULL)
         n_bytes += get_size_model(*model);
@@ -3705,15 +3709,15 @@
 size_t determine_serialized_size_combined
 (
     const char *serialized_model,
     const char *serialized_model_ext,
     const char *serialized_imputer,
     const char *serialized_indexer,
     const size_t size_optional_metadata
-)
+) noexcept
 {
     size_t n_bytes = get_size_setup_info();
     n_bytes += 3 * sizeof(uint8_t);
     n_bytes += 5 * sizeof(size_t);
 
     size_t model_size;
 
@@ -4360,15 +4364,15 @@
         model_ext,
         imputer,
         indexer,
         optional_metadata
     );
 }
 
-bool check_model_has_range_penalty(const IsoForest &model)
+bool check_model_has_range_penalty(const IsoForest &model) noexcept
 {
     for (const auto &tree : model.trees)
     {
         for (const auto &node : tree)
         {
             if (node.score < 0 && node.col_type == Numeric)
             {
@@ -4377,15 +4381,15 @@
             }
         }
     }
 
     return false;
 }
 
-bool check_model_has_range_penalty(const ExtIsoForest &model)
+bool check_model_has_range_penalty(const ExtIsoForest &model) noexcept
 {
     for (const auto &tree : model.hplanes)
     {
         for (const auto &node : tree)
         {
             if (node.score < 0)
             {
@@ -4394,26 +4398,26 @@
             }
         }
     }
 
     return false;
 }
 
-void add_range_penalty(IsoForest &model)
+void add_range_penalty(IsoForest &model) noexcept
 {
     model.has_range_penalty = check_model_has_range_penalty(model);
 }
 
-void add_range_penalty(ExtIsoForest &model)
+void add_range_penalty(ExtIsoForest &model) noexcept
 {
     model.has_range_penalty = check_model_has_range_penalty(model);
 }
 
-void add_range_penalty(Imputer &model)
+void add_range_penalty(Imputer &model) noexcept
 {
     
 }
 
-void add_range_penalty(TreesIndexer &model)
+void add_range_penalty(TreesIndexer &model) noexcept
 {
     
 }
```

### Comparing `isotree-0.5.8.post1/src/sql.cpp` & `isotree-0.5.9/src/sql.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 *          arXiv preprint arXiv:2110.13402 (2021).
 *     [12] Guha, Sudipto, et al.
 *          "Robust random cut forest based anomaly detection on streams."
 *          International conference on machine learning. PMLR, 2016.
 *     [13] Cortes, David.
 *          "Isolation forests: looking beyond tree depth."
 *          arXiv preprint arXiv:2111.11639 (2021).
+*     [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou.
+*          "Isolation kernel and its effect on SVM"
+*          Proceedings of the 24th ACM SIGKDD
+*          International Conference on Knowledge Discovery & Data Mining. 2018.
 * 
 *     BSD 2-Clause License
 *     Copyright (c) 2019-2022, David Cortes
 *     All rights reserved.
 *     Redistribution and use in source and binary forms, with or without
 *     modification, are permitted provided that the following conditions are met:
 *     * Redistributions of source code must retain the above copyright notice, this
```

### Comparing `isotree-0.5.8.post1/src/subset_models.cpp` & `isotree-0.5.9/src/subset_models.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 *          arXiv preprint arXiv:2110.13402 (2021).
 *     [12] Guha, Sudipto, et al.
 *          "Robust random cut forest based anomaly detection on streams."
 *          International conference on machine learning. PMLR, 2016.
 *     [13] Cortes, David.
 *          "Isolation forests: looking beyond tree depth."
 *          arXiv preprint arXiv:2111.11639 (2021).
+*     [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou.
+*          "Isolation kernel and its effect on SVM"
+*          Proceedings of the 24th ACM SIGKDD
+*          International Conference on Knowledge Discovery & Data Mining. 2018.
 * 
 *     BSD 2-Clause License
 *     Copyright (c) 2019-2022, David Cortes
 *     All rights reserved.
 *     Redistribution and use in source and binary forms, with or without
 *     modification, are permitted provided that the following conditions are met:
 *     * Redistributions of source code must retain the above copyright notice, this
```

### Comparing `isotree-0.5.8.post1/src/utils.hpp` & `isotree-0.5.9/src/utils.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 *          arXiv preprint arXiv:2110.13402 (2021).
 *     [12] Guha, Sudipto, et al.
 *          "Robust random cut forest based anomaly detection on streams."
 *          International conference on machine learning. PMLR, 2016.
 *     [13] Cortes, David.
 *          "Isolation forests: looking beyond tree depth."
 *          arXiv preprint arXiv:2111.11639 (2021).
+*     [14] Ting, Kai Ming, Yue Zhu, and Zhi-Hua Zhou.
+*          "Isolation kernel and its effect on SVM"
+*          Proceedings of the 24th ACM SIGKDD
+*          International Conference on Knowledge Discovery & Data Mining. 2018.
 * 
 *     BSD 2-Clause License
 *     Copyright (c) 2019-2022, David Cortes
 *     All rights reserved.
 *     Redistribution and use in source and binary forms, with or without
 *     modification, are permitted provided that the following conditions are met:
 *     * Redistributions of source code must retain the above copyright notice, this
@@ -132,15 +136,15 @@
 {
     double y, z, z2;
 
     /* check for positive integer up to 10 */
     if( (x <= THRESHOLD_EXACT_H) && (x == std::floor(x)) )
         return harmonic(x - 1) - EULERS_GAMMA;
 
-    if( x < 1.0e17 )
+    if (likely(x < 1.0e17 ))
     {
         z = 1.0/(x * x);
         z2 = square(z);
         y = z * ( 8.33333333333333333333E-2
                  -8.33333333333333333333E-3*z
                  +3.96825396825396825397E-3*z2
                  -4.16666666666666666667E-3*z2*z
@@ -371,21 +375,16 @@
             }
         }
 }
 
 void increase_comb_counter_in_groups(size_t ix_arr[], size_t st, size_t end, size_t split_ix, size_t n,
                                      double counter[], double exp_remainder)
 {
-    size_t n_group = 0;
-    for (size_t ix = st; ix <= end; ix++)
-        if (ix_arr[ix] < split_ix)
-            n_group++;
-        else
-            break;
-
+    size_t *ptr_split_ix = std::lower_bound(ix_arr + st, ix_arr + end + 1, split_ix);
+    size_t n_group = std::distance(ix_arr + st, ptr_split_ix);
     n = n - split_ix;
 
     if (exp_remainder <= 1)
         for (size_t ix1 = st; ix1 < st + n_group; ix1++)
             for (size_t ix2 = st + n_group; ix2 <= end; ix2++)
                 counter[ix_arr[ix1] * n + ix_arr[ix2] - split_ix]++;
     else
@@ -393,21 +392,16 @@
             for (size_t ix2 = st + n_group; ix2 <= end; ix2++)
                 counter[ix_arr[ix1] * n + ix_arr[ix2] - split_ix] += exp_remainder;
 }
 
 void increase_comb_counter_in_groups(size_t ix_arr[], size_t st, size_t end, size_t split_ix, size_t n,
                                      double *restrict counter, double *restrict weights, double exp_remainder)
 {
-    size_t n_group = 0;
-    for (size_t ix = st; ix <= end; ix++)
-        if (ix_arr[ix] < split_ix)
-            n_group++;
-        else
-            break;
-
+    size_t *ptr_split_ix = std::lower_bound(ix_arr + st, ix_arr + end + 1, split_ix);
+    size_t n_group = std::distance(ix_arr + st, ptr_split_ix);
     n = n - split_ix;
 
     if (exp_remainder <= 1)
         for (size_t ix1 = st; ix1 < st + n_group; ix1++)
             for (size_t ix2 = st + n_group; ix2 <= end; ix2++)
                 counter[ix_arr[ix1] * n + ix_arr[ix2] - split_ix]
                     +=
@@ -416,37 +410,27 @@
         for (size_t ix1 = st; ix1 < st + n_group; ix1++)
             for (size_t ix2 = st + n_group; ix2 <= end; ix2++)
                 counter[ix_arr[ix1] * n + ix_arr[ix2] - split_ix]
                     +=
                 weights[ix_arr[ix1]] * weights[ix_arr[ix2]] * exp_remainder;
 }
 
-void tmat_to_dense(double *restrict tmat, double *restrict dmat, size_t n, bool diag_to_one, bool diag_to_inf)
+void tmat_to_dense(double *restrict tmat, double *restrict dmat, size_t n, double fill_diag)
 {
     size_t ncomb = calc_ncomb(n);
     for (size_t i = 0; i < (n-1); i++)
     {
         for (size_t j = i + 1; j < n; j++)
         {
             // dmat[i + j * n] = dmat[j + i * n] = tmat[i * (n - (i+1)/2) + j - i - 1];
             dmat[i + j * n] = dmat[j + i * n] = tmat[ix_comb(i, j, n, ncomb)];
         }
     }
-    if (diag_to_one) {
-        for (size_t i = 0; i < n; i++)
-            dmat[i + i * n] = 1;
-    }
-    else if (diag_to_inf) {
-        for (size_t i = 0; i < n; i++)
-            dmat[i + i * n] = std::numeric_limits<double>::infinity();
-    }
-    else {
-        for (size_t i = 0; i < n; i++)
-            dmat[i + i * n] = 0;
-    }
+    for (size_t i = 0; i < n; i++)
+        dmat[i + i * n] = fill_diag;
 }
 
 template <class real_t>
 void build_btree_sampler(std::vector<double> &btree_weights, real_t *restrict sample_weights,
                          size_t nrows, size_t &restrict log2_n, size_t &restrict btree_offset)
 {
     /* build a perfectly-balanced binary search tree in which each node will
@@ -699,22 +683,22 @@
             curr_ix = ix_parent(curr_ix);
             buffer_arr[curr_ix] =   buffer_arr[ix_child(curr_ix)]
                                   + buffer_arr[ix_child(curr_ix) + 1];
         }
     }
 }
 
-double sample_random_uniform(double xmin, double xmax, RNG_engine &rng)
+double sample_random_uniform(double xmin, double xmax, RNG_engine &rng) noexcept
 {
     double out;
     std::uniform_real_distribution<double> runif(xmin, xmax);
     for (int attempt = 0; attempt < 100; attempt++)
     {
         out = runif(rng);
-        if (out < xmax) return out;
+        if (likely(out < xmax)) return out;
     }
     return xmin;
 }
 
 /*  This one samples with replacement. When using weights, the algorithm is the
     same as for the row sampler, but keeping the weights after taking each iteration. */
 /*  TODO: this column sampler could use coroutines from C++20 once compilers implement them. */
@@ -735,15 +719,15 @@
     this->offset = pow2(this->tree_levels) - 1;
     for (size_t ix = 0; ix < this->n_cols; ix++)
         this->tree_weights[ix + this->offset] = std::fmax(0., weights[ix]);
     for (size_t ix = this->tree_weights.size() - 1; ix > 0; ix--)
         this->tree_weights[ix_parent(ix)] += this->tree_weights[ix];
 
     /* if the weights are invalid, make it an unweighted sampler */
-    if (isnan(this->tree_weights[0]) || this->tree_weights[0] <= 0)
+    if (unlikely(isnan(this->tree_weights[0]) || this->tree_weights[0] <= 0))
     {
         this->drop_weights();
     }
 
     this->n_dropped = 0;
 }
 
@@ -1208,15 +1192,15 @@
 
         /* due to the way this is calculated, there can be large roundoff errors and even negatives */
         if (this->cumw <= 0)
         {
             this->cumw = 0;
             for (size_t col = 0; col < this->curr_pos; col++)
                 this->cumw += this->weights_orig[this->col_indices[col]];
-            if (this->cumw <= 0)
+            if (unlikely(this->cumw <= 0))
                 unexpected_error();
         }
 
         /* if there are no infinites, choose a column according to weight */
         ldouble_safe chosen = std::uniform_real_distribution<ldouble_safe>((ldouble_safe)0, this->cumw)(rnd_generator);
         ldouble_safe cumw_ = 0;
         for (size_t col = 0; col < this->curr_pos; col++)
@@ -2168,15 +2152,15 @@
 {
     this->n_present = 0;
     for (int cat = 0; cat < ncat; cat++)
         this->n_present +=  cat_counts[cat] > 0;
 }
 
 /* For hyperplane intersections */
-size_t divide_subset_split(size_t ix_arr[], double x[], size_t st, size_t end, double split_point)
+size_t divide_subset_split(size_t ix_arr[], double x[], size_t st, size_t end, double split_point) noexcept
 {
     size_t temp;
     size_t st_orig = st;
     for (size_t row = st_orig; row <= end; row++)
     {
         if (x[row - st_orig] <= split_point)
         {
@@ -2188,15 +2172,15 @@
     }
     return st;
 }
 
 /* For numerical columns */
 template <class real_t>
 void divide_subset_split(size_t *restrict ix_arr, real_t x[], size_t st, size_t end, double split_point,
-                         MissingAction missing_action, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix)
+                         MissingAction missing_action, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix) noexcept
 {
     size_t temp;
 
     /* if NAs are not to be bothered with, just need to do a single pass */
     if (missing_action == Fail)
     {
         /* move to the left if it's l.e. split point */
@@ -2226,15 +2210,15 @@
                 st++;
             }
         }
         st_NA = st;
 
         for (size_t row = st; row <= end; row++)
         {
-            if (isnan(x[ix_arr[row]]))
+            if (unlikely(isnan(x[ix_arr[row]])))
             {
                 temp        = ix_arr[st];
                 ix_arr[st]  = ix_arr[row];
                 ix_arr[row] = temp;
                 st++;
             }
         }
@@ -2242,15 +2226,15 @@
     }
 }
 
 /* For sparse numeric columns */
 template <class real_t, class sparse_ix>
 void divide_subset_split(size_t *restrict ix_arr, size_t st, size_t end, size_t col_num,
                          real_t Xc[], sparse_ix *restrict Xc_ind, sparse_ix *restrict Xc_indptr, double split_point,
-                         MissingAction missing_action, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix)
+                         MissingAction missing_action, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix) noexcept
 {
     /* TODO: this is a mess, needs refactoring */
     /* TODO: when moving zeros, would be better to instead move by '>' (opposite as in here) */
     /* TODO: should create an extra version to go along with 'predict' that would
        add the range penalty right here to spare operations. */
     if (Xc_indptr[col_num] == Xc_indptr[col_num + 1])
     {
@@ -2392,15 +2376,15 @@
                         st++;
                     }
                     break;
                 }
 
                 if (Xc_ind[curr_pos] == (sparse_ix)(*row))
                 {
-                    if (isnan(Xc[curr_pos]))
+                    if (unlikely(isnan(Xc[curr_pos])))
                         has_NAs = true;
                     else if (Xc[curr_pos] <= split_point)
                     {
                         temp       = ix_arr[st];
                         ix_arr[st] = *row;
                         *row       = temp;
                         st++;
@@ -2442,15 +2426,15 @@
         {
             for (size_t *row = ptr_st;
                  row != ix_arr + end + 1 && curr_pos != end_col + 1 && ind_end_col >= *row;
                 )
             {
                 if (Xc_ind[curr_pos] == (sparse_ix)(*row))
                 {
-                    if (isnan(Xc[curr_pos])) has_NAs = true;
+                    if (unlikely(isnan(Xc[curr_pos]))) has_NAs = true;
                     if (!isnan(Xc[curr_pos]) && Xc[curr_pos] <= split_point)
                     {
                         temp       = ix_arr[st];
                         ix_arr[st] = *row;
                         *row       = temp;
                         st++;
                     }
@@ -2476,15 +2460,15 @@
             std::sort(ix_arr + st, ix_arr + end + 1);
             for (size_t *row = ix_arr + st;
                  row != ix_arr + end + 1 && curr_pos != end_col + 1 && ind_end_col >= *row;
                 )
             {
                 if (Xc_ind[curr_pos] == (sparse_ix)(*row))
                 {
-                    if (isnan(Xc[curr_pos]))
+                    if (unlikely(isnan(Xc[curr_pos])))
                     {
                         temp       = ix_arr[st];
                         ix_arr[st] = *row;
                         *row       = temp;
                         st++;
                     }
                     if (row == ix_arr + end || curr_pos == end_col) break;
@@ -2504,15 +2488,15 @@
 
     }
 
 }
 
 /* For categorical columns split by subset */
 void divide_subset_split(size_t *restrict ix_arr, int x[], size_t st, size_t end, signed char split_categ[],
-                         MissingAction missing_action, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix)
+                         MissingAction missing_action, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix) noexcept
 {
     size_t temp;
 
     /* if NAs are not to be bothered with, just need to do a single pass */
     if (missing_action == Fail)
     {
         /* move to the left if it's l.e. than the split point */
@@ -2557,15 +2541,15 @@
         end_NA = st;
     }
 }
 
 /* For categorical columns split by subset, used at prediction time (with similarity) */
 void divide_subset_split(size_t *restrict ix_arr, int x[], size_t st, size_t end, signed char split_categ[],
                          int ncat, MissingAction missing_action, NewCategAction new_cat_action,
-                         bool move_new_to_left, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix)
+                         bool move_new_to_left, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix) noexcept
 {
     size_t temp;
     int cval;
 
     /* if NAs are not to be bothered with, just need to do a single pass */
     if (missing_action == Fail && new_cat_action != Weighted)
     {
@@ -2658,15 +2642,15 @@
         }
         st_NA = st;
 
         if (!(missing_action == Impute && !move_new_to_left))
         {
             for (size_t row = st; row <= end; row++)
             {
-                if (x[ix_arr[row]] < 0)
+                if (unlikely(x[ix_arr[row]] < 0))
                 {
                     temp        = ix_arr[st];
                     ix_arr[st]  = ix_arr[row];
                     ix_arr[row] = temp;
                     st++;
                 }
             }
@@ -2758,15 +2742,15 @@
             }
         }
 
         else if (missing_action == Divide)
         {
             for (size_t row = st; row <= end; row++)
             {
-                if (x[ix_arr[row]] < 0)
+                if (unlikely(x[ix_arr[row]] < 0))
                 {
                     temp        = ix_arr[st];
                     ix_arr[st]  = ix_arr[row];
                     ix_arr[row] = temp;
                     st++;
                 }
             }
@@ -2774,15 +2758,15 @@
 
         end_NA = st;
     }
 }
 
 /* For categoricals split on a single category */
 void divide_subset_split(size_t *restrict ix_arr, int x[], size_t st, size_t end, int split_categ,
-                         MissingAction missing_action, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix)
+                         MissingAction missing_action, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix) noexcept
 {
     size_t temp;
 
     /* if NAs are not to be bothered with, just need to do a single pass */
     if (missing_action == Fail)
     {
         /* move to the left if it's equal to the chosen category */
@@ -2812,30 +2796,30 @@
                 st++;
             }
         }
         st_NA = st;
 
         for (size_t row = st; row <= end; row++)
         {
-            if (x[ix_arr[row]] < 0)
+            if (unlikely(x[ix_arr[row]] < 0))
             {
                 temp        = ix_arr[st];
                 ix_arr[st]  = ix_arr[row];
                 ix_arr[row] = temp;
                 st++;
             }
         }
         end_NA = st;
     }
 }
 
 /* For categoricals split on sub-set that turned out to have 2 categories only (prediction-time) */
 void divide_subset_split(size_t *restrict ix_arr, int x[], size_t st, size_t end,
                          MissingAction missing_action, NewCategAction new_cat_action,
-                         bool move_new_to_left, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix)
+                         bool move_new_to_left, size_t &restrict st_NA, size_t &restrict end_NA, size_t &restrict split_ix) noexcept
 {
     size_t temp;
 
     /* if NAs are not to be bothered with, just need to do a single pass */
     if (missing_action == Fail)
     {
         /* move to the left if it's l.e. than the split point */
@@ -2884,15 +2868,15 @@
                     st++;
                 }
             }
             st_NA = st;
 
             for (size_t row = st; row <= end; row++)
             {
-                if (x[ix_arr[row]] < 0)
+                if (unlikely(x[ix_arr[row]] < 0))
                 {
                     temp        = ix_arr[st];
                     ix_arr[st]  = ix_arr[row];
                     ix_arr[row] = temp;
                     st++;
                 }
             }
@@ -2911,15 +2895,15 @@
                     st++;
                 }
             }
             st_NA = st;
 
             for (size_t row = st; row <= end; row++)
             {
-                if (x[ix_arr[row]] < 0)
+                if (unlikely(x[ix_arr[row]] < 0))
                 {
                     temp        = ix_arr[st];
                     ix_arr[st]  = ix_arr[row];
                     ix_arr[row] = temp;
                     st++;
                 }
             }
@@ -2927,15 +2911,15 @@
         }
     }
 }
 
 /* for regular numeric columns */
 template <class real_t>
 void get_range(size_t ix_arr[], real_t *restrict x, size_t st, size_t end,
-               MissingAction missing_action, double &restrict xmin, double &restrict xmax, bool &unsplittable)
+               MissingAction missing_action, double &restrict xmin, double &restrict xmax, bool &unsplittable) noexcept
 {
     xmin =  HUGE_VAL;
     xmax = -HUGE_VAL;
     double xval;
 
     if (missing_action == Fail)
     {
@@ -2959,15 +2943,15 @@
     }
 
     unsplittable = (xmin == xmax) || (xmin == HUGE_VAL && xmax == -HUGE_VAL) || isnan(xmin) || isnan(xmax);
 }
 
 template <class real_t>
 void get_range(real_t *restrict x, size_t n,
-               MissingAction missing_action, double &restrict xmin, double &restrict xmax, bool &unsplittable)
+               MissingAction missing_action, double &restrict xmin, double &restrict xmax, bool &unsplittable) noexcept
 {
     xmin =  HUGE_VAL;
     xmax = -HUGE_VAL;
 
     if (missing_action == Fail)
     {
         for (size_t row = 0; row < n; row++)
@@ -2990,15 +2974,15 @@
     unsplittable = (xmin == xmax) || (xmin == HUGE_VAL && xmax == -HUGE_VAL) || isnan(xmin) || isnan(xmax);
 }
 
 /* for sparse inputs */
 template <class real_t, class sparse_ix>
 void get_range(size_t *restrict ix_arr, size_t st, size_t end, size_t col_num,
                real_t *restrict Xc, sparse_ix *restrict Xc_ind, sparse_ix *restrict Xc_indptr,
-               MissingAction missing_action, double &restrict xmin, double &restrict xmax, bool &unsplittable)
+               MissingAction missing_action, double &restrict xmin, double &restrict xmax, bool &unsplittable) noexcept
 {
     /* ix_arr must already be sorted beforehand */
     xmin =  HUGE_VAL;
     xmax = -HUGE_VAL;
 
     size_t st_col  = Xc_indptr[col_num];
     size_t end_col = Xc_indptr[col_num + 1];
@@ -3086,15 +3070,15 @@
 
     unsplittable = (xmin == xmax) || (xmin == HUGE_VAL && xmax == -HUGE_VAL) || isnan(xmin) || isnan(xmax);
 }
 
 template <class real_t, class sparse_ix>
 void get_range(size_t col_num, size_t nrows,
                real_t *restrict Xc, sparse_ix *restrict Xc_ind, sparse_ix *restrict Xc_indptr,
-               MissingAction missing_action, double &restrict xmin, double &restrict xmax, bool &unsplittable)
+               MissingAction missing_action, double &restrict xmin, double &restrict xmax, bool &unsplittable) noexcept
 {
     xmin =  HUGE_VAL;
     xmax = -HUGE_VAL;
 
     if ((size_t)(Xc_indptr[col_num+1] - Xc_indptr[col_num]) < nrows)
     {
         xmin = 0;
@@ -3110,31 +3094,31 @@
         }
     }
 
     else
     {
         for (auto ix = Xc_indptr[col_num]; ix < Xc_indptr[col_num+1]; ix++)
         {
-            if (std::isinf(Xc[ix])) continue;
+            if (unlikely(std::isinf(Xc[ix]))) continue;
             xmin = std::fmin(xmin, Xc[ix]);
             xmax = std::fmax(xmax, Xc[ix]);
         }
     }
 
     unsplittable = (xmin == xmax) || (xmin == HUGE_VAL && xmax == -HUGE_VAL) || isnan(xmin) || isnan(xmax);
 }
 
 
 void get_categs(size_t *restrict ix_arr, int x[], size_t st, size_t end, int ncat,
-                MissingAction missing_action, signed char categs[], size_t &restrict npresent, bool &unsplittable)
+                MissingAction missing_action, signed char categs[], size_t &restrict npresent, bool &unsplittable) noexcept
 {
     std::fill(categs, categs + ncat, -1);
     npresent = 0;
     for (size_t row = st; row <= end; row++)
-        if (x[ix_arr[row]] >= 0)
+        if (likely(x[ix_arr[row]] >= 0))
             categs[x[ix_arr[row]]] = 1;
 
     npresent = std::accumulate(categs,
                                categs + ncat,
                                (size_t)0,
                                [](const size_t a, const signed char b){return a + (b > 0);}
                                );
@@ -3158,15 +3142,15 @@
 
     else
     {
         real_t x0;
         size_t ix;
         for (ix = st; ix <= end; ix++)
         {
-            if (!is_na_or_inf(x[ix_arr[ix]]))
+            if (likely(!is_na_or_inf(x[ix_arr[ix]])))
             {
                 x0 = x[ix_arr[ix]];
                 ix++;
                 break;
             }
         }
 
@@ -3335,24 +3319,24 @@
     return false;
 }
 
 void count_categs(size_t *restrict ix_arr, size_t st, size_t end, int x[], int ncat, size_t *restrict counts)
 {
     std::fill(counts, counts + ncat, (size_t)0);
     for (size_t row = st; row <= end; row++)
-        if (x[ix_arr[row]] >= 0)
+        if (likely(x[ix_arr[row]] >= 0))
             counts[x[ix_arr[row]]]++;
 }
 
 int count_ncateg_in_col(const int x[], const size_t n, const int ncat, unsigned char buffer[])
 {
     memset(buffer, 0, ncat*sizeof(char));
     for (size_t ix = 0; ix < n; ix++)
     {
-        if (x[ix] >= 0) buffer[x[ix]] = true;
+        if (likely(x[ix] >= 0)) buffer[x[ix]] = true;
     }
 
     int ncat_present = 0;
     for (int cat = 0; cat < ncat; cat++)
         ncat_present += buffer[cat];
     return ncat_present;
 }
@@ -3378,15 +3362,15 @@
 size_t move_NAs_to_front(size_t ix_arr[], size_t st, size_t end, real_t x[])
 {
     size_t st_non_na = st;
     size_t temp;
 
     for (size_t row = st; row <= end; row++)
     {
-        if (is_na_or_inf(x[ix_arr[row]]))
+        if (unlikely(is_na_or_inf(x[ix_arr[row]])))
         {
             temp = ix_arr[st_non_na];
             ix_arr[st_non_na] = ix_arr[row];
             ix_arr[row] = temp;
             st_non_na++;
         }
     }
@@ -3409,15 +3393,15 @@
 
     for (size_t *row = ptr_st;
          row != ix_arr + end + 1 && curr_pos != end_col + 1 && ind_end_col >= *row;
         )
     {
         if (Xc_ind[curr_pos] == *row)
         {
-            if (is_na_or_inf(Xc[curr_pos]))
+            if (unlikely(is_na_or_inf(Xc[curr_pos])))
             {
                 temp = ix_arr[st_non_na];
                 ix_arr[st_non_na] = *row;
                 *row = temp;
                 st_non_na++;
             }
 
@@ -3440,15 +3424,15 @@
 size_t move_NAs_to_front(size_t ix_arr[], size_t st, size_t end, int x[])
 {
     size_t st_non_na = st;
     size_t temp;
 
     for (size_t row = st; row <= end; row++)
     {
-        if (x[ix_arr[row]] < 0)
+        if (unlikely(x[ix_arr[row]] < 0))
         {
             temp = ix_arr[st_non_na];
             ix_arr[st_non_na] = ix_arr[row];
             ix_arr[row] = temp;
             st_non_na++;
         }
     }
```

### Comparing `isotree-0.5.8.post1/src/xoshiro.hpp` & `isotree-0.5.9/src/xoshiro.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -14,68 +14,75 @@
 #if (__cplusplus  >= 202002L)
 #include <bit>
 #endif
 using std::uint32_t;
 using std::uint64_t;
 using std::memcpy;
 
+#ifndef _FOR_R
+    #if defined(__clang__)
+        #pragma clang diagnostic push
+        #pragma clang diagnostic ignored "-Wunknown-attributes"
+    #endif
+#endif
+
 namespace Xoshiro {
 
 #if (__cplusplus  >= 202002L)
 #define rotl64(x, k) std::rotl(x, k)
 #define rotl32(x, k) std::rotl(x, k)
 #else
-static inline uint64_t rotl64(const uint64_t x, const int k) {
+static inline uint64_t rotl64(const uint64_t x, const int k) noexcept {
     return (x << k) | (x >> (64 - k));
 }
-static inline uint32_t rotl32(const uint32_t x, const int k) {
+static inline uint32_t rotl32(const uint32_t x, const int k) noexcept {
     return (x << k) | (x >> (32 - k));
 }
 #endif
 
 /* these are in order to avoid gcc warnings about 'strict aliasing rules' */
-static inline uint32_t extract_32bits_from64_left(const uint64_t x)
+static inline uint32_t extract_32bits_from64_left(const uint64_t x) noexcept
 {
     uint32_t out;
     memcpy(reinterpret_cast<char*>(&out),
            reinterpret_cast<const char*>(&x),
            sizeof(uint32_t));
     return out;
 }
 
-static inline uint32_t extract_32bits_from64_right(const uint64_t x)
+static inline uint32_t extract_32bits_from64_right(const uint64_t x) noexcept
 {
     uint32_t out;
     memcpy(reinterpret_cast<char*>(&out),
            reinterpret_cast<const char*>(&x) + sizeof(uint32_t),
            sizeof(uint32_t));
     return out;
 }
 
-static inline void assign_32bits_to64_left(uint64_t &assign_to, const uint32_t take_from)
+static inline void assign_32bits_to64_left(uint64_t &assign_to, const uint32_t take_from) noexcept
 {
     memcpy(reinterpret_cast<char*>(&assign_to),
            reinterpret_cast<const char*>(&take_from),
            sizeof(uint32_t));
 }
 
-static inline void assign_32bits_to64_right(uint64_t &assign_to, const uint32_t take_from)
+static inline void assign_32bits_to64_right(uint64_t &assign_to, const uint32_t take_from) noexcept
 {
     memcpy(reinterpret_cast<char*>(&assign_to) + sizeof(uint32_t),
            reinterpret_cast<const char*>(&take_from),
            sizeof(uint32_t));
 }
 
 /* This is a fixed-increment version of Java 8's SplittableRandom generator
    See http://dx.doi.org/10.1145/2714064.2660195 and 
    http://docs.oracle.com/javase/8/docs/api/java/util/SplittableRandom.html
 
    It is a very fast generator passing BigCrush, and it can be useful if
    for some reason you absolutely want 64 bits of state. */
-static inline uint64_t splitmix64(const uint64_t seed)
+static inline uint64_t splitmix64(const uint64_t seed) noexcept
 {
     uint64_t z = (seed + 0x9e3779b97f4a7c15);
     z = (z ^ (z >> 30)) * 0xbf58476d1ce4e5b9;
     z = (z ^ (z >> 27)) * 0x94d049bb133111eb;
     return z ^ (z >> 31);
 }
 
@@ -91,52 +98,52 @@
    output to fill s. */
 class Xoshiro256PP
 {
 public:
     using result_type = uint64_t;
     uint64_t state[4];
 
-    constexpr static result_type min()
+    constexpr static result_type min() noexcept
     {
         return 0;
     }
 
-    constexpr static result_type max()
+    constexpr static result_type max() noexcept
     {
         return UINT64_MAX;
     }
 
-    Xoshiro256PP() = default;
+    Xoshiro256PP() noexcept = default;
 
-    inline void seed(const uint64_t seed)
+    inline void seed(const uint64_t seed) noexcept
     {
         this->state[0] = splitmix64(splitmix64(seed));
         this->state[1] = splitmix64(this->state[0]);
         this->state[2] = splitmix64(this->state[1]);
         this->state[3] = splitmix64(this->state[2]);
     }
 
     template <class integer>
-    inline void seed(const integer seed)
+    inline void seed(const integer seed) noexcept
     {
         this->seed((uint64_t)seed);
     }
 
-    Xoshiro256PP(const uint64_t seed)
+    Xoshiro256PP(const uint64_t seed) noexcept
     {
         this->seed(seed);
     }
 
     template <class integer>
-    Xoshiro256PP(const integer seed)
+    Xoshiro256PP(const integer seed) noexcept
     {
         this->seed((uint64_t)seed);
     }
 
-    inline result_type operator()()
+    inline result_type operator()() noexcept
     {
         const uint64_t result = rotl64(this->state[0] + this->state[3], 23) + this->state[0];
         const uint64_t t = this->state[1] << 17;
         this->state[2] ^= this->state[0];
         this->state[3] ^= this->state[1];
         this->state[1] ^= this->state[2];
         this->state[0] ^= this->state[3];
@@ -157,69 +164,69 @@
    The state must be seeded so that it is not everywhere zero. */
 class Xoshiro128PP
 {
 public:
     using result_type = uint32_t;
     uint32_t state[4];
 
-    constexpr static result_type min()
+    constexpr static result_type min() noexcept
     {
         return 0;
     }
 
-    constexpr static result_type max()
+    constexpr static result_type max() noexcept
     {
         return UINT32_MAX;
     }
 
-    Xoshiro128PP() = default;
+    Xoshiro128PP() noexcept = default;
 
 
-    inline void seed(const uint64_t seed)
+    inline void seed(const uint64_t seed) noexcept
     {
         const auto t1 = splitmix64(seed);
         const auto t2 = splitmix64(t1);
         this->state[0] = extract_32bits_from64_left(t1);
         this->state[1] = extract_32bits_from64_right(t1);
         this->state[2] = extract_32bits_from64_left(t2);
         this->state[3] = extract_32bits_from64_right(t2);
     }
 
-    inline void seed(const uint32_t seed)
+    inline void seed(const uint32_t seed) noexcept
     {
         uint64_t temp;
         assign_32bits_to64_left(temp, seed);
         assign_32bits_to64_right(temp, seed);
         this->seed(temp);
     }
 
 
     template <class integer>
-    inline void seed(const integer seed)
+    inline void seed(const integer seed) noexcept
     {
         this->seed((uint64_t)seed);
     }
 
-    Xoshiro128PP(const uint32_t seed)
+    Xoshiro128PP(const uint32_t seed) noexcept
     {
         this->seed(seed);
     }
 
-    Xoshiro128PP(const uint64_t seed)
+    Xoshiro128PP(const uint64_t seed) noexcept
     {
         this->seed(seed);
     }
 
     template <class integer>
-    Xoshiro128PP(const integer seed)
+    Xoshiro128PP(const integer seed) noexcept
     {
         this->seed((uint64_t)seed);
     }
 
-    inline result_type operator()()
+    inline result_type operator()() noexcept
     {
         const uint32_t result = rotl32(this->state[0] + this->state[3], 7) + this->state[0];
         const uint32_t t = this->state[1] << 9;
         this->state[2] ^= this->state[0];
         this->state[3] ^= this->state[1];
         this->state[1] ^= this->state[2];
         this->state[0] ^= this->state[3];
@@ -240,34 +247,34 @@
 constexpr static const uint32_t two22_i = (UINT32_C(1) << 22) - UINT32_C(1);
 constexpr static const uint32_t two21_i = (UINT32_C(1) << 21) - UINT32_C(1);
 constexpr static const uint32_t two20_i = (UINT32_C(1) << 20) - UINT32_C(1);
 constexpr static const double ui64_d = (double)UINT64_MAX;
 constexpr static const double i64_d = (double)INT64_MAX;
 constexpr static const double twoPI = 2. * M_PI;
 
-static inline uint64_t gen_bits(Xoshiro256PP &rng)
+static inline uint64_t gen_bits(Xoshiro256PP &rng) noexcept
 {
     return rng();
 }
 
-static inline uint64_t gen_bits(Xoshiro128PP &rng)
+static inline uint64_t gen_bits(Xoshiro128PP &rng) noexcept
 {
     uint64_t bits;
     assign_32bits_to64_left(bits, rng());
     assign_32bits_to64_right(bits, rng());
     return bits;
 }
 
 
 /* Note: the way in which endian-ness detection is handled here looks
    inefficient at a first glance. Nevertheless, do NOT try to optimize
    any further as GCC9 has a bug in which it optimizes away some 'if's'
    but with the *wrong* bit ending if done as ternary operators or if
    declaring pointer variables outside of the braces in what comes below. */
-static inline bool get_is_little_endian()
+static inline bool get_is_little_endian() noexcept
 {
     const uint32_t ONE = 1;
     return (*(reinterpret_cast<const unsigned char*>(&ONE)) != 0);
 }
 static const bool is_little_endian = get_is_little_endian();
 
 /* ~Uniform([0,1))
@@ -279,24 +286,24 @@
      that something will go wrong, but better not take it).
    (For example, GCC4 had bugs like those)
    Hence this replacement. It is not too much slower
    than what the compiler's header use. */
 class UniformUnitInterval
 {
 public:
-    UniformUnitInterval() = default;
+    UniformUnitInterval() noexcept = default;
 
     template <class A, class B>
-    UniformUnitInterval(A a, B b) {}
+    UniformUnitInterval(A a, B b) noexcept {}
     
     template <class XoshiroRNG>
     #ifndef _FOR_R
     [[gnu::optimize("no-trapping-math"), gnu::optimize("no-math-errno")]]
     #endif
-    double operator()(XoshiroRNG &rng)
+    double operator()(XoshiroRNG &rng) noexcept
     {
         #if SIZE_MAX >= UINT64_MAX
         #   if (__cplusplus >= 201703L) || (__cplusplus >= 201402L && (defined(__GNUC__) || defined(_MSC_VER)))
         return (double)(gen_bits(rng) & two53_i) * 0x1.0p-53;
         #   else
         return std::ldexp(gen_bits(rng) & two53_i, -53);
         #   endif
@@ -326,47 +333,47 @@
    interval. Nevertheless, since it'd be less than ideal to
    output zero from here (that is, it would mean not taking
    a column when creating a random hyperplane), it instead
    will transform exact zeros into exact ones. */
 class UniformMinusOneToOne
 {
 public:
-    UniformMinusOneToOne() = default;
+    UniformMinusOneToOne() noexcept = default;
 
     template <class A, class B>
-    UniformMinusOneToOne(A a, B b) {}
+    UniformMinusOneToOne(A a, B b) noexcept {}
 
     template <class XoshiroRNG>
     #ifndef _FOR_R
     [[gnu::optimize("no-trapping-math"), gnu::optimize("no-math-errno")]]
     #endif
-    double operator()(XoshiroRNG &rng)
+    double operator()(XoshiroRNG &rng) noexcept
     {
         #if SIZE_MAX >= UINT64_MAX
         #   if (__cplusplus >= 201703L) || (__cplusplus >= 201402L && (defined(__GNUC__) || defined(_MSC_VER)))
         double out = (double)((int64_t)(gen_bits(rng) & two54_i) - two53_ii) * 0x1.0p-53;
         #   else
         double out = std::ldexp((int64_t)(gen_bits(rng) & two54_i) - two53_ii, -53);
         #endif
-        if (out == 0) out = 1;
+        if (unlikely(out == 0)) out = 1;
         return out;
         #else
         uint64_t bits = gen_bits(rng);
         char *rbits_ = reinterpret_cast<char*>(&bits);
         if (is_little_endian) rbits_ += sizeof(uint32_t);
         uint32_t rbits;
         memcpy(&rbits, rbits_, sizeof(uint32_t));
         rbits = rbits & two22_i;
         memcpy(rbits_, &rbits, sizeof(uint32_t));
         #   if (__cplusplus >= 201703L) || (__cplusplus >= 201402L && (defined(__GNUC__) || defined(_MSC_VER)))
         double out = (double)((int64_t)bits - two53_ii) * 0x1.0p-53;
         #   else
         double out = std::ldexp((int64_t)bits - two53_ii, -53);
         #endif
-        if (out == 0) out = 1;
+        if (unlikely(out == 0)) out = 1;
         return out;
         #endif
     }
 };
 
 /* Normal distribution using Box-Muller transform in raw form.
    This usually gives better results than the polar form, but
@@ -381,24 +388,24 @@
    Which is how it reaches an unbiased open uniform distribution. */
 class StandardNormalDistr
 {
 public:
     double reserve;
     double has_reserve = false;
 
-    StandardNormalDistr() = default;
+    StandardNormalDistr() noexcept = default;
 
     template <class A, class B>
-    StandardNormalDistr(A a, B b) : has_reserve(false) {}
+    StandardNormalDistr(A a, B b) noexcept : has_reserve(false) {}
 
     template <class XoshiroRNG>
     #ifndef _FOR_R
     [[gnu::optimize("no-trapping-math"), gnu::optimize("no-math-errno")]]
     #endif
-    double operator()(XoshiroRNG &rng)
+    double operator()(XoshiroRNG &rng) noexcept
     {
         double res;
         if (has_reserve) {
             res = this->reserve;
         }
         
         else {
@@ -444,7 +451,13 @@
         this->has_reserve = !this->has_reserve;
         if (!res) return this->operator()(rng);
         return res;
     }
 };
 
 }
+
+#ifndef _FOR_R
+    #if defined(__clang__)
+        #pragma clang diagnostic pop
+    #endif
+#endif
```

