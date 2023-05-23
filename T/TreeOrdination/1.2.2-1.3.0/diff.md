# Comparing `tmp/treeordination-1.2.2.tar.gz` & `tmp/treeordination-1.3.0.tar.gz`

## Comparing `treeordination-1.2.2.tar` & `treeordination-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 treeordination-1.2.2/environment.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 treeordination-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 treeordination-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 treeordination-1.2.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 treeordination-1.2.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    13285 2020-02-02 00:00:00.000000 treeordination-1.2.2/TreeOrdination/TreeOrdination.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 treeordination-1.2.2/TreeOrdination/__init__.py
--rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 treeordination-1.2.2/TreeOrdination/feature_importance_treeord.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 treeordination-1.2.2/TreeOrdination/transformers_treeord.py
--rw-r--r--   0        0        0    10961 2020-02-02 00:00:00.000000 treeordination-1.2.2/docs/API.md
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 treeordination-1.2.2/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treeordination-1.2.2/notebooks/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treeordination-1.2.2/tests/__init__.py
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 treeordination-1.2.2/tests/test_treeord.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 treeordination-1.2.2/.gitignore
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 treeordination-1.2.2/LICENSE
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 treeordination-1.2.2/README.md
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 treeordination-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 treeordination-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 treeordination-1.3.0/environment.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 treeordination-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 treeordination-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 treeordination-1.3.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 treeordination-1.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 treeordination-1.3.0/TreeOrdination/TreeOrdination.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 treeordination-1.3.0/TreeOrdination/__init__.py
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 treeordination-1.3.0/TreeOrdination/feature_importance_treeord.py
+-rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 treeordination-1.3.0/TreeOrdination/transformers_treeord.py
+-rw-r--r--   0        0        0     9119 2020-02-02 00:00:00.000000 treeordination-1.3.0/docs/API.md
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 treeordination-1.3.0/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treeordination-1.3.0/notebooks/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treeordination-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 treeordination-1.3.0/tests/test_treeord.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 treeordination-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 treeordination-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 treeordination-1.3.0/README.md
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 treeordination-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 treeordination-1.3.0/PKG-INFO
```

### Comparing `treeordination-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md` & `treeordination-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `treeordination-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md` & `treeordination-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `treeordination-1.2.2/.github/workflows/ci.yml` & `treeordination-1.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `treeordination-1.2.2/.github/workflows/python-publish.yml` & `treeordination-1.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `treeordination-1.2.2/TreeOrdination/feature_importance_treeord.py` & `treeordination-1.3.0/TreeOrdination/feature_importance_treeord.py`

 * *Files identical despite different names*

### Comparing `treeordination-1.2.2/docs/API.md` & `treeordination-1.3.0/docs/API.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,48 +2,45 @@
 
 This section provides an overview of the `TreeOrdination` and the different parameters
 of the `TreeOrdination` class and its methods.
 
 ## Class
 
     class TreeOrdination.TreeOrdination(feature_names, resampler =  NoResample(),  metric  = "hamming", supervised_clf =  ExtraTreesClassifier(1024),
-                                        proxy_model = ExtraTreesRegressor(1024), n_iter_unsup = 5, unsup_n_estim = 160, max_samples_tree = 100, transformer =  NoTransform(),
+                                        proxy_model = ExtraTreesRegressor(1024), n_iter_unsup = 5, unsup_n_estim = 160, transformer =  NoTransform(),
                                         exclude_col = [False, 0],  n_neighbors = 8, n_components  = 2, min_dist = 0.001, n_jobs = 4)
 
 ### Parameters
 
     feature_names: list-like, required
         A list of feature names.
 
     resampler: default = NoResample
         The re-sampling  method to be used. Should follow the format
-        used by 'imbalaced-learn'
+        used by 'imbalaced-learn'. Use this to control how many samples
+        are passed to LANDMark.
     
     metric: str, default = "hamming"
         The metric used by UMAP to calculate the dissimilarity between 
         LANDMark embeddings.
         
     supervised_clf: default = ExtraTreesClassifier(1024)
         The classification model used to predict the class of each sample
         using the unsupervised projections.
         
     proxy_model: default = ExtraTreesClassifier(1024)
         The regression model used to predict the location of each sample
         in the projected space.
 
+    landmark_model: default = LANDMarkClassifier(160, use_nnet = False, n_jobs = 8)
+
     n_iter_unsup: int, default = 5
         The number of LANDMark embeddings which will be used to construct
         the final embedding.
-        
-    unsup_n_estim: int, default = 160
-        The number of decision trees in each LANDMark classifier.
-
-    max_samples_tree: int, default = 100
-        Specifies how many samples will be used to train each LANDMark tree.
-        
+                
     transformer: default = NoTransform()
         The pre-processing method used to transform data. Should follow
         the 'scikit-learn' format.
         
     exclude_col: list-like, default = [False, [0]]
         Specifies which columns should be excluded for scaling and/or
         transformation. If the first entry in the list is true the columns
@@ -57,17 +54,14 @@
      
     n_components: int, default = 2
         The number of components of the final unsupervised projection.
      
     min_dist: float, default = 0.001
         The 'min_dist' parameter of UMAP.
 
-    n_jobs: int, default = 4
-        The number of processes used by LANDMark to train each classifier.
-
 ### Attributes
 
     encoded_labels: LabelEncoder
         A label encoder used to transform class labels.
 
     X, y: np.ndarray
         A saved copy of the training data.
@@ -85,42 +79,33 @@
     l_model: 
         A regression model which maps training data to the output produced
         by R_PCA (see below).
 
     Rs: list
         A list of trained LANDMark models
 
-    R_final: list
+    LM_emb: np.ndarray
         A list of LANDMark proximities
 
-    features_scaled: list
-        A list of masks containing information about zero-variance features
-        which are removed prior to preprocessing
-
-    features_unscaled: list
-        A list of masks containing information about zero-variance features
-        which are to be removed. These are features to which a pre-processing
-        transformation is not to be applied.
-
     transformers: list
         A list of pre-processing transformers to be applied prior to fitting
         a LANDMark model or using a LANDMark model to calculate proximities.
 
-    tree_emb: UMAP
+    UMAP_trf: UMAP
         A 'UMAP' transformer trained using R_final.
 
-    R_PCA: PCA
+    UMAP_emb: np.ndarray
+        The UMAP transformed data..
+
+    PCA_trf: PCA
         A 'scikit-learn' PCA transformer fit using the output of the UMAP
         transformer.
 
-    R_PCA_emb: np.ndarray
-        The PCA transformed data produced by applying R_PCA.
-
-    self.feature_importance_explainer:
-        An 'alibi' TreeExplainer object.
+    PCA_emb: np.ndarray
+        The PCA transformed data.
 
 ### Methods
 
     fit(X, y, **fit_params)
         Fits a `TreeOrdination` model.
 
         Parameters:
@@ -229,66 +214,42 @@
         the number of features (taxa, OTUs, ASVs, etc).
 
         Returns:
 
         A np.ndarray of shape (m, p) where 'm' is the number of samples in X and
         'p' is the number of classes.
 
-    transform(X)
-        Transforms X into the high-dimensional LANDMark embedding.
-
-        Input:
-
-        X: NumPy array of shape (m, n) where 'm' is the number of samples and 'n'
-        the number of features (taxa, OTUs, ASVs, etc).
-
-        Returns:
-
-        X_transformed: NumPy array of shape (m, p) where 'm' is the number of samples and 'p'
-        the number of features (leaves of the LANDMark embedding)
-
-    emb_transform(X, y, **fit_params)
-        Transforms X into a lower dimensional embedding using LANDMark proximities.
+    emb_transform(X, y, trf_type)
+        Transforms X into a lower dimensional embedding.
 
         Parameters:
 
         X: NumPy array of shape (m, n) where 'm' is the number of samples and 'n'
         the number of features (taxa, OTUs, ASVs, etc).
 
-        Returns:
-
-        X_transformed: NumPy array of shape (m, p) where 'm' is the number of samples and 'p'
-        the number of components specified at the initialization of `TreeOrdination`.
-
-    approx_transform(X)
-        Transforms X into a lower dimensional embedding using the proxy model.
-
-        Parameters:
-
-        X: NumPy array of shape (m, n) where 'm' is the number of samples and 'n'
-        the number of features (taxa, OTUs, ASVs, etc).
+        trf_type: str, default = "PCA"
+        Transforms data using the specified transformer. Options are "approx", 
+        "LM", "UMAP", or "PCA".
 
         Returns:
 
         X_transformed: NumPy array of shape (m, p) where 'm' is the number of samples and 'p'
         the number of components specified at the initialization of `TreeOrdination`.
 
 ## Class
 
-    class TreeOrdination.NoTransform()
-    class TreeOrdination.NoResample()
     class TreeOrdination.CLRClosureTransform(do_clr = False, delta = None)
 
 ### Parameters (For CLRClosureTransform() Only)
 
     do_clr: bool, default = False
         Applies the CLR transformation if True. Otherwise only the closure
         operation is applied.
 
-### Methods (CLRClosureTransform/NoTransform)
+### Methods (CLRClosureTransform)
 
     fit_transform(X, y = None, **kwargs)
         Fits a CLRClosureTransform/NoTransform model and returns the transformed data.
         A NoTransform model will just return the original data.
 
         Parameters:
 
@@ -308,24 +269,8 @@
 
         X: NumPy array of shape (m, n) where 'm' is the number of samples and 'n'
         the number of features (taxa, OTUs, ASVs, etc).
 
         Returns:
 
         X_transformed: NumPy array of shape (m, n) where 'm' is the number of samples and 'n'
-        the number of features.
-
-### Methods (NoResample)
-
-    fit_resample(X, y, **kwargs)
-
-        Parameters:
-
-        X: NumPy array of shape (m, n) where 'm' is the number of samples and 'n'
-        the number of features (taxa, OTUs, ASVs, etc).
-
-        y: NumPy array of shape (m,) where 'm' is the number of samples. Each entry
-        of 'y' should be a factor.
-
-        Returns:
-
-        X, y
+        the number of features.
```

### Comparing `treeordination-1.2.2/docs/CONTRIBUTING.md` & `treeordination-1.3.0/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `treeordination-1.2.2/tests/test_treeord.py` & `treeordination-1.3.0/tests/test_treeord.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from TreeOrdination import (
     TreeOrdination,
     CLRClosureTransformer,
-    NoTransform,
-    NoResample,
 )
 
 from sklearn.datasets import make_classification
 from sklearn.preprocessing import StandardScaler
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import balanced_accuracy_score, median_absolute_error
 
@@ -34,33 +32,25 @@
         shuffle=False,
         random_state=0,
     )
 
     # To prevent negative proportions
     X_non_neg = np.abs(X)
 
-    # Ensures that the NoScale transformer returns the input
-    R = pd.DataFrame(NoTransform().fit_transform(X))
-    X = pd.DataFrame(X)
-    pd.testing.assert_frame_equal(X, R, check_dtype=False)
-
     # Ensures that CLRTransformer returns the CLR Transform of X
     R = pd.DataFrame(CLRClosureTransformer(do_clr=True).fit_transform(X_non_neg))
 
     X_clr = pd.DataFrame(clr(multiplicative_replacement(closure(X_non_neg))))
     pd.testing.assert_frame_equal(X_clr, R, check_dtype=False)
 
     # Ensures that CLRTransformer returns the Closure of X
     R = pd.DataFrame(CLRClosureTransformer(do_clr=False).fit_transform(X_non_neg))
     X_closure = pd.DataFrame(closure(X_non_neg))
     pd.testing.assert_frame_equal(X_closure, R, check_dtype=False)
 
-    # Ensures that NoResample returns the input
-    R, R_y = NoResample().fit_resample(X, y)
-
     R = pd.DataFrame(R)
     pd.testing.assert_frame_equal(X, R, check_dtype=False)
 
     R_y = pd.Series(R_y)
     y = pd.Series(y)
     pd.testing.assert_series_equal(y, R_y, check_dtype=False)
```

### Comparing `treeordination-1.2.2/.gitignore` & `treeordination-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `treeordination-1.2.2/LICENSE` & `treeordination-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `treeordination-1.2.2/README.md` & `treeordination-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `treeordination-1.2.2/pyproject.toml` & `treeordination-1.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "TreeOrdination"
-version = "1.2.2"
+version = "1.3.0"
 authors = [
     {name = "Josip Rudar", email = "rudarj@uoguelph.ca"},
     {name = "G. Brian Golding"},
     {name = "Stefan C. Kremer"},
     {name = "Mehrdad Hajibabaei", email = "mhajibab@uoguelph.ca"}
 ]
 description = "Projection of High-Dimensional Data Using Multivariate Decision Trees and UMAP"
@@ -36,15 +36,15 @@
 dependencies = [
     "numpy == 1.23.5",
     "scikit-learn >= 1.1.2",
     "scikit-bio >= 0.5.8",
     "umap-learn >= 0.5.3",
     "seaborn",
     "shap >= 0.40.0",
-    "LANDMarkClassifier >= 2.0.2"
+    "LANDMarkClassifier >= 2.0.4"
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project.urls]
 "Homepage" = "https://github.com/jrudar/TreeOrdination"
@@ -61,11 +61,11 @@
 
 test = [
     "pytest",
     "pytest-cov"
 ]
 
 [tool.pytest.ini_options]
-addopts = "--cov --cov-report html --cov-report term-missing --cov-fail-under 70"
+addopts = "--cov --cov-report html --cov-report term-missing --cov-fail-under 30"
 
 [tool.coverage.run]
 source = ["TreeOrdination"]
```

### Comparing `treeordination-1.2.2/PKG-INFO` & `treeordination-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TreeOrdination
-Version: 1.2.2
+Version: 1.3.0
 Summary: Projection of High-Dimensional Data Using Multivariate Decision Trees and UMAP
 Project-URL: Homepage, https://github.com/jrudar/TreeOrdination
 Project-URL: Repository, https://github.com/jrudar/TreeOrdination.git
 Project-URL: Bug Tracker, https://github.com/jrudar/TreeOrdination/issues
 Author: G. Brian Golding, Stefan C. Kremer
 Author-email: Josip Rudar <rudarj@uoguelph.ca>, Mehrdad Hajibabaei <mhajibab@uoguelph.ca>
 License: MIT License
@@ -38,15 +38,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
-Requires-Dist: landmarkclassifier>=2.0.2
+Requires-Dist: landmarkclassifier>=2.0.4
 Requires-Dist: numpy==1.23.5
 Requires-Dist: scikit-bio>=0.5.8
 Requires-Dist: scikit-learn>=1.1.2
 Requires-Dist: seaborn
 Requires-Dist: shap>=0.40.0
 Requires-Dist: umap-learn>=0.5.3
 Provides-Extra: dev
```

