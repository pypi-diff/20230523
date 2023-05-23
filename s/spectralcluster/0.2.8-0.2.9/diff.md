# Comparing `tmp/spectralcluster-0.2.8.tar.gz` & `tmp/spectralcluster-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectralcluster-0.2.8.tar", last modified: Fri Jun 10 20:51:39 2022, max compression
+gzip compressed data, was "spectralcluster-0.2.9.tar", last modified: Sun Jun 12 18:00:12 2022, max compression
```

## Comparing `spectralcluster-0.2.8.tar` & `spectralcluster-0.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 quanw    (353957) eng       (5000)        0 2022-06-10 20:51:39.405335 spectralcluster-0.2.8/
--rw-r--r--   0 quanw    (353957) eng       (5000)    11339 2019-01-19 02:20:33.000000 spectralcluster-0.2.8/LICENSE
--rw-r--r--   0 quanw    (353957) eng       (5000)    10354 2022-06-10 20:51:39.405147 spectralcluster-0.2.8/PKG-INFO
--rw-r--r--   0 quanw    (353957) eng       (5000)     9943 2022-06-10 16:38:03.000000 spectralcluster-0.2.8/README.md
--rw-r--r--   0 quanw    (353957) eng       (5000)       38 2022-06-10 20:51:39.405385 spectralcluster-0.2.8/setup.cfg
--rw-r--r--   0 quanw    (353957) eng       (5000)      695 2022-06-10 20:49:59.000000 spectralcluster-0.2.8/setup.py
-drwxr-xr-x   0 quanw    (353957) eng       (5000)        0 2022-06-10 20:51:39.404340 spectralcluster-0.2.8/spectralcluster/
--rw-r--r--   0 quanw    (353957) eng       (5000)      978 2022-06-10 16:00:23.000000 spectralcluster-0.2.8/spectralcluster/__init__.py
--rw-r--r--   0 quanw    (353957) eng       (5000)     4135 2022-05-31 14:11:00.000000 spectralcluster-0.2.8/spectralcluster/autotune.py
--rw-r--r--   0 quanw    (353957) eng       (5000)     2729 2021-09-27 00:23:32.000000 spectralcluster-0.2.8/spectralcluster/configs.py
--rw-r--r--   0 quanw    (353957) eng       (5000)     8145 2021-10-04 20:19:30.000000 spectralcluster-0.2.8/spectralcluster/constraint.py
--rw-r--r--   0 quanw    (353957) eng       (5000)     5404 2021-07-28 18:25:34.000000 spectralcluster-0.2.8/spectralcluster/custom_distance_kmeans.py
--rw-r--r--   0 quanw    (353957) eng       (5000)     2448 2022-06-10 19:25:20.000000 spectralcluster-0.2.8/spectralcluster/fallback_clusterer.py
--rw-r--r--   0 quanw    (353957) eng       (5000)     1738 2021-10-04 20:19:00.000000 spectralcluster-0.2.8/spectralcluster/laplacian.py
--rw-r--r--   0 quanw    (353957) eng       (5000)     9215 2021-10-04 20:18:41.000000 spectralcluster-0.2.8/spectralcluster/refinement.py
--rw-r--r--   0 quanw    (353957) eng       (5000)    11092 2022-06-10 20:49:13.000000 spectralcluster-0.2.8/spectralcluster/spectral_clusterer.py
--rw-r--r--   0 quanw    (353957) eng       (5000)     4897 2021-10-04 20:19:49.000000 spectralcluster-0.2.8/spectralcluster/utils.py
-drwxr-xr-x   0 quanw    (353957) eng       (5000)        0 2022-06-10 20:51:39.404960 spectralcluster-0.2.8/spectralcluster.egg-info/
--rw-r--r--   0 quanw    (353957) eng       (5000)    10354 2022-06-10 20:51:39.000000 spectralcluster-0.2.8/spectralcluster.egg-info/PKG-INFO
--rw-r--r--   0 quanw    (353957) eng       (5000)      497 2022-06-10 20:51:39.000000 spectralcluster-0.2.8/spectralcluster.egg-info/SOURCES.txt
--rw-r--r--   0 quanw    (353957) eng       (5000)        1 2022-06-10 20:51:39.000000 spectralcluster-0.2.8/spectralcluster.egg-info/dependency_links.txt
--rw-r--r--   0 quanw    (353957) eng       (5000)       16 2022-06-10 20:51:39.000000 spectralcluster-0.2.8/spectralcluster.egg-info/top_level.txt
+drwxr-xr-x   0 quanw    (353957) eng       (5000)        0 2022-06-12 18:00:12.865766 spectralcluster-0.2.9/
+-rw-r--r--   0 quanw    (353957) eng       (5000)    11339 2019-01-19 02:20:33.000000 spectralcluster-0.2.9/LICENSE
+-rw-r--r--   0 quanw    (353957) eng       (5000)    10395 2022-06-12 18:00:12.865498 spectralcluster-0.2.9/PKG-INFO
+-rw-r--r--   0 quanw    (353957) eng       (5000)     9984 2022-06-12 17:56:57.000000 spectralcluster-0.2.9/README.md
+-rw-r--r--   0 quanw    (353957) eng       (5000)       38 2022-06-12 18:00:12.865827 spectralcluster-0.2.9/setup.cfg
+-rw-r--r--   0 quanw    (353957) eng       (5000)      695 2022-06-12 17:54:52.000000 spectralcluster-0.2.9/setup.py
+drwxr-xr-x   0 quanw    (353957) eng       (5000)        0 2022-06-12 18:00:12.864630 spectralcluster-0.2.9/spectralcluster/
+-rw-r--r--   0 quanw    (353957) eng       (5000)      978 2022-06-10 16:00:23.000000 spectralcluster-0.2.9/spectralcluster/__init__.py
+-rw-r--r--   0 quanw    (353957) eng       (5000)     4135 2022-05-31 14:11:00.000000 spectralcluster-0.2.9/spectralcluster/autotune.py
+-rw-r--r--   0 quanw    (353957) eng       (5000)     2729 2021-09-27 00:23:32.000000 spectralcluster-0.2.9/spectralcluster/configs.py
+-rw-r--r--   0 quanw    (353957) eng       (5000)     8145 2021-10-04 20:19:30.000000 spectralcluster-0.2.9/spectralcluster/constraint.py
+-rw-r--r--   0 quanw    (353957) eng       (5000)     5404 2021-07-28 18:25:34.000000 spectralcluster-0.2.9/spectralcluster/custom_distance_kmeans.py
+-rw-r--r--   0 quanw    (353957) eng       (5000)     4644 2022-06-12 17:53:43.000000 spectralcluster-0.2.9/spectralcluster/fallback_clusterer.py
+-rw-r--r--   0 quanw    (353957) eng       (5000)     1738 2021-10-04 20:19:00.000000 spectralcluster-0.2.9/spectralcluster/laplacian.py
+-rw-r--r--   0 quanw    (353957) eng       (5000)     9215 2021-10-04 20:18:41.000000 spectralcluster-0.2.9/spectralcluster/refinement.py
+-rw-r--r--   0 quanw    (353957) eng       (5000)     9591 2022-06-12 16:27:57.000000 spectralcluster-0.2.9/spectralcluster/spectral_clusterer.py
+-rw-r--r--   0 quanw    (353957) eng       (5000)     4897 2021-10-04 20:19:49.000000 spectralcluster-0.2.9/spectralcluster/utils.py
+drwxr-xr-x   0 quanw    (353957) eng       (5000)        0 2022-06-12 18:00:12.865309 spectralcluster-0.2.9/spectralcluster.egg-info/
+-rw-r--r--   0 quanw    (353957) eng       (5000)    10395 2022-06-12 18:00:12.000000 spectralcluster-0.2.9/spectralcluster.egg-info/PKG-INFO
+-rw-r--r--   0 quanw    (353957) eng       (5000)      497 2022-06-12 18:00:12.000000 spectralcluster-0.2.9/spectralcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 quanw    (353957) eng       (5000)        1 2022-06-12 18:00:12.000000 spectralcluster-0.2.9/spectralcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 quanw    (353957) eng       (5000)       16 2022-06-12 18:00:12.000000 spectralcluster-0.2.9/spectralcluster.egg-info/top_level.txt
```

### Comparing `spectralcluster-0.2.8/LICENSE` & `spectralcluster-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spectralcluster-0.2.8/PKG-INFO` & `spectralcluster-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectralcluster
-Version: 0.2.8
+Version: 0.2.9
 Summary: Spectral Clustering
 Home-page: https://github.com/wq2012/SpectralCluster
 Author: Quan Wang
 Author-email: quanw@google.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -182,15 +182,15 @@
 
 Spectral clustering exploits the global structure of the data. But there are
 cases where spectral clustering does not work as well as some other simpler
 clustering methods, such as when the number of embeddings is too small.
 
 When initializing the `SpectralClusterer` object, you can pass in a `FallbackOptions` object to the `fallback_options` argument, to use a fallback clusterer under certain conditions.
 
-Also, since spectral clustering and eigen-gap may not work well at making single-vs-multi cluster decisions, when `min_clusters=1`, we can also specify `FallbackOptions.single_cluster_affinity_threshold` to help determine single cluster cases by thresdholding the affinity matrix.
+Also, spectral clustering and eigen-gap may not work well at making single-vs-multi cluster decisions. When `min_clusters=1`, we can also specify `FallbackOptions.single_cluster_condition` and `FallbackOptions.single_cluster_affinity_threshold` to help determine single cluster cases by thresdholding the affinity matrix.
 
 For the complete list of parameters of `FallbackOptions`, see `spectralcluster/fallback_clusterer.py`.
 
 ### Constrained spectral clustering
 
 ![turn-to-diarize-diagram](https://raw.githubusercontent.com/wq2012/SpectralCluster/master/resources/turn-to-diarize.png)
```

### Comparing `spectralcluster-0.2.8/README.md` & `spectralcluster-0.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 
 Spectral clustering exploits the global structure of the data. But there are
 cases where spectral clustering does not work as well as some other simpler
 clustering methods, such as when the number of embeddings is too small.
 
 When initializing the `SpectralClusterer` object, you can pass in a `FallbackOptions` object to the `fallback_options` argument, to use a fallback clusterer under certain conditions.
 
-Also, since spectral clustering and eigen-gap may not work well at making single-vs-multi cluster decisions, when `min_clusters=1`, we can also specify `FallbackOptions.single_cluster_affinity_threshold` to help determine single cluster cases by thresdholding the affinity matrix.
+Also, spectral clustering and eigen-gap may not work well at making single-vs-multi cluster decisions. When `min_clusters=1`, we can also specify `FallbackOptions.single_cluster_condition` and `FallbackOptions.single_cluster_affinity_threshold` to help determine single cluster cases by thresdholding the affinity matrix.
 
 For the complete list of parameters of `FallbackOptions`, see `spectralcluster/fallback_clusterer.py`.
 
 ### Constrained spectral clustering
 
 ![turn-to-diarize-diagram](https://raw.githubusercontent.com/wq2012/SpectralCluster/master/resources/turn-to-diarize.png)
```

### Comparing `spectralcluster-0.2.8/setup.py` & `spectralcluster-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Setup script for the package."""
 
 import setuptools
 
-VERSION = "0.2.8"
+VERSION = "0.2.9"
 
 with open("README.md", "r") as file_object:
     LONG_DESCRIPTION = file_object.read()
 
 setuptools.setup(
     name="spectralcluster",
     version=VERSION,
```

### Comparing `spectralcluster-0.2.8/spectralcluster/__init__.py` & `spectralcluster-0.2.9/spectralcluster/__init__.py`

 * *Files identical despite different names*

### Comparing `spectralcluster-0.2.8/spectralcluster/autotune.py` & `spectralcluster-0.2.9/spectralcluster/autotune.py`

 * *Files identical despite different names*

### Comparing `spectralcluster-0.2.8/spectralcluster/configs.py` & `spectralcluster-0.2.9/spectralcluster/configs.py`

 * *Files identical despite different names*

### Comparing `spectralcluster-0.2.8/spectralcluster/constraint.py` & `spectralcluster-0.2.9/spectralcluster/constraint.py`

 * *Files identical despite different names*

### Comparing `spectralcluster-0.2.8/spectralcluster/custom_distance_kmeans.py` & `spectralcluster-0.2.9/spectralcluster/custom_distance_kmeans.py`

 * *Files identical despite different names*

### Comparing `spectralcluster-0.2.8/spectralcluster/laplacian.py` & `spectralcluster-0.2.9/spectralcluster/laplacian.py`

 * *Files identical despite different names*

### Comparing `spectralcluster-0.2.8/spectralcluster/refinement.py` & `spectralcluster-0.2.9/spectralcluster/refinement.py`

 * *Files identical despite different names*

### Comparing `spectralcluster-0.2.8/spectralcluster/spectral_clusterer.py` & `spectralcluster-0.2.9/spectralcluster/spectral_clusterer.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from spectralcluster import refinement
 from spectralcluster import utils
 
 RefinementName = refinement.RefinementName
 LaplacianType = laplacian.LaplacianType
 ConstraintName = constraint.ConstraintName
 EigenGapType = utils.EigenGapType
-SingleClusterCondition = fallback_clusterer.SingleClusterCondition
 
 
 class SpectralClusterer:
   """Spectral clustering class."""
 
   def __init__(self,
                min_clusters=None,
@@ -137,51 +136,14 @@
       n_clusters, max_delta_norm = utils.compute_number_of_clusters(
           eigenvalues,
           max_clusters=self.max_clusters,
           eigengap_type=self.eigengap_type,
           descend=False)
     return eigenvectors, n_clusters, max_delta_norm
 
-  def _check_single_cluster(self, embeddings, affinity):
-    """Check whether this is only a single cluster.
-
-    Args:
-      embeddings: numpy array of shape (n_samples, n_features)
-      affinity: the affinity matrix of shape (n_samples, (n_samples)
-
-    Returns:
-      a boolean, where True means there is only a single cluster
-    """
-    if (self.fallback_options.single_cluster_condition ==
-        SingleClusterCondition.AllAffinity):
-      if (affinity.min() >
-          self.fallback_options.single_cluster_affinity_threshold):
-        return True
-    elif (self.fallback_options.single_cluster_condition ==
-          SingleClusterCondition.NeighborAffinity):
-      neighbor_affinity = np.diag(affinity, k=1)
-      if (neighbor_affinity.min() >
-          self.fallback_options.single_cluster_affinity_threshold):
-        return True
-    elif (self.fallback_options.single_cluster_condition ==
-          SingleClusterCondition.AffinityStd):
-      if (np.std(affinity) <
-          self.fallback_options.single_cluster_affinity_threshold):
-        return True
-    elif (self.fallback_options.single_cluster_condition ==
-          SingleClusterCondition.FallbackClusterer):
-      temp_clusterer = fallback_clusterer.FallbackClusterer(
-          self.fallback_options)
-      temp_labels = temp_clusterer.predict(embeddings)
-      if np.unique(temp_labels).size == 1:
-        return True
-    else:
-      raise TypeError("Unsupported single_cluster_condition")
-    return False
-
   def predict(self, embeddings, constraint_matrix=None):
     """Perform spectral clustering on data embeddings.
 
     The spectral clustering is performed on an affinity matrix.
 
     Args:
       embeddings: numpy array of shape (n_samples, n_features)
@@ -210,15 +172,16 @@
       return temp_clusterer.predict(embeddings)
 
     # Compute affinity matrix.
     affinity = self.affinity_function(embeddings)
 
     # Make single-vs-multi cluster(s) decision.
     if self.min_clusters == 1:
-      if self._check_single_cluster(embeddings, affinity):
+      if fallback_clusterer.check_single_cluster(
+          self.fallback_options, embeddings, affinity):
         return np.array([0] * num_embeddings)
 
     # Apply constraint.
     if (self.constraint_options and
         self.constraint_options.apply_before_refinement):
       # Perform the constraint operation before refinement
       affinity = self.constraint_options.constraint_operator.adjust_affinity(
```

### Comparing `spectralcluster-0.2.8/spectralcluster/utils.py` & `spectralcluster-0.2.9/spectralcluster/utils.py`

 * *Files identical despite different names*

### Comparing `spectralcluster-0.2.8/spectralcluster.egg-info/PKG-INFO` & `spectralcluster-0.2.9/spectralcluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectralcluster
-Version: 0.2.8
+Version: 0.2.9
 Summary: Spectral Clustering
 Home-page: https://github.com/wq2012/SpectralCluster
 Author: Quan Wang
 Author-email: quanw@google.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -182,15 +182,15 @@
 
 Spectral clustering exploits the global structure of the data. But there are
 cases where spectral clustering does not work as well as some other simpler
 clustering methods, such as when the number of embeddings is too small.
 
 When initializing the `SpectralClusterer` object, you can pass in a `FallbackOptions` object to the `fallback_options` argument, to use a fallback clusterer under certain conditions.
 
-Also, since spectral clustering and eigen-gap may not work well at making single-vs-multi cluster decisions, when `min_clusters=1`, we can also specify `FallbackOptions.single_cluster_affinity_threshold` to help determine single cluster cases by thresdholding the affinity matrix.
+Also, spectral clustering and eigen-gap may not work well at making single-vs-multi cluster decisions. When `min_clusters=1`, we can also specify `FallbackOptions.single_cluster_condition` and `FallbackOptions.single_cluster_affinity_threshold` to help determine single cluster cases by thresdholding the affinity matrix.
 
 For the complete list of parameters of `FallbackOptions`, see `spectralcluster/fallback_clusterer.py`.
 
 ### Constrained spectral clustering
 
 ![turn-to-diarize-diagram](https://raw.githubusercontent.com/wq2012/SpectralCluster/master/resources/turn-to-diarize.png)
```

