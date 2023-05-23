# Comparing `tmp/tsaugmentation-0.5.8.tar.gz` & `tmp/tsaugmentation-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsaugmentation-0.5.8.tar", last modified: Wed Nov 30 10:54:22 2022, max compression
+gzip compressed data, was "tsaugmentation-0.5.9.tar", last modified: Wed Nov 30 12:43:53 2022, max compression
```

## Comparing `tsaugmentation-0.5.8.tar` & `tsaugmentation-0.5.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 10:54:22.340065 tsaugmentation-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (122)      655 2022-11-30 10:54:22.340065 tsaugmentation-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-30 10:54:22.340065 tsaugmentation-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1565 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 10:54:22.324065 tsaugmentation-0.5.8/tsaugmentation/
--rw-r--r--   0 runner    (1001) docker     (122)      392 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 10:54:22.328065 tsaugmentation-0.5.8/tsaugmentation/feature_engineering/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/feature_engineering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1590 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/feature_engineering/dynamic_features.py
--rw-r--r--   0 runner    (1001) docker     (122)     2173 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/feature_engineering/feature_transformations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1215 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/feature_engineering/get_data_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     2095 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/feature_engineering/static_features.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 10:54:22.328065 tsaugmentation-0.5.8/tsaugmentation/model/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1818 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/model/helper.py
--rw-r--r--   0 runner    (1001) docker     (122)     6490 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/model/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 10:54:22.332064 tsaugmentation-0.5.8/tsaugmentation/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (122)       32 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2036 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/postprocessing/generative_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 10:54:22.332064 tsaugmentation-0.5.8/tsaugmentation/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (122)       39 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10000 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/preprocessing/pre_processing_datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     5343 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/preprocessing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 10:54:22.336065 tsaugmentation-0.5.8/tsaugmentation/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2236 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/tests/test_building_distances_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)     2375 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/tests/test_compute_similarities.py
--rw-r--r--   0 runner    (1001) docker     (122)     4601 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/tests/test_create_transformed_dataset_files.py
--rw-r--r--   0 runner    (1001) docker     (122)     1268 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/tests/test_end2end_vae.py
--rw-r--r--   0 runner    (1001) docker     (122)     1283 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/tests/test_end2end_vae_prison.py
--rw-r--r--   0 runner    (1001) docker     (122)     3476 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/tests/test_evaluate_similarity_dataset_w_groups.py
--rw-r--r--   0 runner    (1001) docker     (122)     8088 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/tests/test_feature_engineering.py
--rw-r--r--   0 runner    (1001) docker     (122)      900 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/tests/test_import_datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/tests/test_manipulate_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3658 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     4504 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/tests/test_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (122)      810 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/tests/test_similarity_ts.py
--rw-r--r--   0 runner    (1001) docker     (122)      671 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/tests/test_visualize_transformed_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 10:54:22.340065 tsaugmentation-0.5.8/tsaugmentation/transformations/
--rw-r--r--   0 runner    (1001) docker     (122)      277 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2524 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/transformations/compute_distances.py
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/transformations/compute_similarities.py
--rw-r--r--   0 runner    (1001) docker     (122)     3143 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/transformations/compute_similarities_summary_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     7787 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/transformations/create_dataset_versions.py
--rw-r--r--   0 runner    (1001) docker     (122)    12598 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/transformations/create_dataset_versions_vae.py
--rw-r--r--   0 runner    (1001) docker     (122)     1983 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/transformations/manipulate_data.py
--rw-r--r--   0 runner    (1001) docker     (122)      328 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/transformations/similarity_model.py
--rw-r--r--   0 runner    (1001) docker     (122)      129 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/transformations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 10:54:22.340065 tsaugmentation-0.5.8/tsaugmentation/visualization/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2245 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/visualization/model_visualization.py
--rw-r--r--   0 runner    (1001) docker     (122)     3822 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/visualization/visualize_ridge_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     3402 2022-11-30 10:54:13.000000 tsaugmentation-0.5.8/tsaugmentation/visualization/visualize_transformed_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 10:54:22.328065 tsaugmentation-0.5.8/tsaugmentation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      655 2022-11-30 10:54:22.000000 tsaugmentation-0.5.8/tsaugmentation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2022-11-30 10:54:22.000000 tsaugmentation-0.5.8/tsaugmentation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 10:54:22.000000 tsaugmentation-0.5.8/tsaugmentation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      169 2022-11-30 10:54:22.000000 tsaugmentation-0.5.8/tsaugmentation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2022-11-30 10:54:22.000000 tsaugmentation-0.5.8/tsaugmentation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:43:53.123607 tsaugmentation-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (122)      655 2022-11-30 12:43:53.123607 tsaugmentation-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-30 12:43:53.123607 tsaugmentation-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1565 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:43:53.119607 tsaugmentation-0.5.9/tsaugmentation/
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:43:53.119607 tsaugmentation-0.5.9/tsaugmentation/feature_engineering/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/feature_engineering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1590 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/feature_engineering/dynamic_features.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2173 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/feature_engineering/feature_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1215 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/feature_engineering/get_data_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2095 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/feature_engineering/static_features.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:43:53.119607 tsaugmentation-0.5.9/tsaugmentation/model/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1818 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/model/helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6490 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/model/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:43:53.119607 tsaugmentation-0.5.9/tsaugmentation/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2036 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/postprocessing/generative_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:43:53.119607 tsaugmentation-0.5.9/tsaugmentation/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10000 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/preprocessing/pre_processing_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5343 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/preprocessing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:43:53.119607 tsaugmentation-0.5.9/tsaugmentation/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2236 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/tests/test_building_distances_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2375 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/tests/test_compute_similarities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4601 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/tests/test_create_transformed_dataset_files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1268 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/tests/test_end2end_vae.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1283 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/tests/test_end2end_vae_prison.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3476 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/tests/test_evaluate_similarity_dataset_w_groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8088 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/tests/test_feature_engineering.py
+-rw-r--r--   0 runner    (1001) docker     (122)      900 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/tests/test_import_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/tests/test_manipulate_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3658 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4504 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/tests/test_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/tests/test_similarity_ts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      671 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/tests/test_visualize_transformed_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:43:53.119607 tsaugmentation-0.5.9/tsaugmentation/transformations/
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2524 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/transformations/compute_distances.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/transformations/compute_similarities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3143 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/transformations/compute_similarities_summary_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7787 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/transformations/create_dataset_versions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12542 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/transformations/create_dataset_versions_vae.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1983 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/transformations/manipulate_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      328 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/transformations/similarity_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/transformations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:43:53.119607 tsaugmentation-0.5.9/tsaugmentation/visualization/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2245 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/visualization/model_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3822 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/visualization/visualize_ridge_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2022-11-30 12:43:38.000000 tsaugmentation-0.5.9/tsaugmentation/visualization/visualize_transformed_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:43:53.119607 tsaugmentation-0.5.9/tsaugmentation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      655 2022-11-30 12:43:53.000000 tsaugmentation-0.5.9/tsaugmentation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2022-11-30 12:43:53.000000 tsaugmentation-0.5.9/tsaugmentation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 12:43:53.000000 tsaugmentation-0.5.9/tsaugmentation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2022-11-30 12:43:53.000000 tsaugmentation-0.5.9/tsaugmentation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2022-11-30 12:43:53.000000 tsaugmentation-0.5.9/tsaugmentation.egg-info/top_level.txt
```

### Comparing `tsaugmentation-0.5.8/PKG-INFO` & `tsaugmentation-0.5.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsaugmentation
-Version: 0.5.8
+Version: 0.5.9
 Summary: Robust time series tsaugmentation for forecasting algorithms
 Author: Luis Roque
 Author-email: <roque0luis@gmail.com>
 Keywords: python,time series,hierarchical,forecasting,tsaugmentation,machine learning
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `tsaugmentation-0.5.8/setup.py` & `tsaugmentation-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/feature_engineering/dynamic_features.py` & `tsaugmentation-0.5.9/tsaugmentation/feature_engineering/dynamic_features.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/feature_engineering/feature_transformations.py` & `tsaugmentation-0.5.9/tsaugmentation/feature_engineering/feature_transformations.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/feature_engineering/get_data_distance.py` & `tsaugmentation-0.5.9/tsaugmentation/feature_engineering/get_data_distance.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/feature_engineering/static_features.py` & `tsaugmentation-0.5.9/tsaugmentation/feature_engineering/static_features.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/model/helper.py` & `tsaugmentation-0.5.9/tsaugmentation/model/helper.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/model/models.py` & `tsaugmentation-0.5.9/tsaugmentation/model/models.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/postprocessing/generative_helper.py` & `tsaugmentation-0.5.9/tsaugmentation/postprocessing/generative_helper.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/preprocessing/pre_processing_datasets.py` & `tsaugmentation-0.5.9/tsaugmentation/preprocessing/pre_processing_datasets.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/preprocessing/utils.py` & `tsaugmentation-0.5.9/tsaugmentation/preprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/tests/test_building_distances_plots.py` & `tsaugmentation-0.5.9/tsaugmentation/tests/test_building_distances_plots.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/tests/test_compute_similarities.py` & `tsaugmentation-0.5.9/tsaugmentation/tests/test_compute_similarities.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/tests/test_create_transformed_dataset_files.py` & `tsaugmentation-0.5.9/tsaugmentation/tests/test_create_transformed_dataset_files.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/tests/test_end2end_vae.py` & `tsaugmentation-0.5.9/tsaugmentation/tests/test_end2end_vae.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/tests/test_end2end_vae_prison.py` & `tsaugmentation-0.5.9/tsaugmentation/tests/test_end2end_vae_prison.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/tests/test_evaluate_similarity_dataset_w_groups.py` & `tsaugmentation-0.5.9/tsaugmentation/tests/test_evaluate_similarity_dataset_w_groups.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/tests/test_feature_engineering.py` & `tsaugmentation-0.5.9/tsaugmentation/tests/test_feature_engineering.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/tests/test_import_datasets.py` & `tsaugmentation-0.5.9/tsaugmentation/tests/test_import_datasets.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/tests/test_manipulate_data.py` & `tsaugmentation-0.5.9/tsaugmentation/tests/test_manipulate_data.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/tests/test_models.py` & `tsaugmentation-0.5.9/tsaugmentation/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/tests/test_postprocessing.py` & `tsaugmentation-0.5.9/tsaugmentation/tests/test_postprocessing.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/tests/test_similarity_ts.py` & `tsaugmentation-0.5.9/tsaugmentation/tests/test_similarity_ts.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/tests/test_visualize_transformed_datasets.py` & `tsaugmentation-0.5.9/tsaugmentation/tests/test_visualize_transformed_datasets.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/transformations/compute_distances.py` & `tsaugmentation-0.5.9/tsaugmentation/transformations/compute_distances.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/transformations/compute_similarities.py` & `tsaugmentation-0.5.9/tsaugmentation/transformations/compute_similarities.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/transformations/compute_similarities_summary_metrics.py` & `tsaugmentation-0.5.9/tsaugmentation/transformations/compute_similarities_summary_metrics.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/transformations/create_dataset_versions.py` & `tsaugmentation-0.5.9/tsaugmentation/transformations/create_dataset_versions.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/transformations/create_dataset_versions_vae.py` & `tsaugmentation-0.5.9/tsaugmentation/transformations/create_dataset_versions_vae.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,26 +57,26 @@
         self.df = pd.concat(
             [self.df, pd.DataFrame(self.dataset["dates"], columns=["Date"])], axis=1
         )[: self.n]
         self.df = self.df.set_index("Date")
         self.df.asfreq(self.freq)
 
         # Create dataset with window_size more dates in the past to be used
-        if self.freq == 'Q':
+        if self.freq == 'QS':
             start_date = self.df.index[0] - pd.DateOffset(months=10*3)
-        elif self.freq == 'M':
+        elif self.freq == 'MS':
             start_date = self.df.index[0] - pd.DateOffset(months=10)
         elif self.freq == 'W':
             start_date = self.df.index[0] - pd.DateOffset(weeks=10)
         elif self.freq == 'D':
             start_date = self.df.index[0] - pd.DateOffset(days=10)
         ix = pd.date_range(
             start=start_date,
             end=self.df.index[-1],
-            freq=self.freq + "S",  # S ensures that we are at the start of the period
+            freq=self.freq,
         )
         self.df_generate = self.df.copy()
         self.df_generate = self.df_generate.reindex(ix)
 
         self.features_input = (None, None, None)
         self._create_directories()
         self._save_original_file()
```

### Comparing `tsaugmentation-0.5.8/tsaugmentation/transformations/manipulate_data.py` & `tsaugmentation-0.5.9/tsaugmentation/transformations/manipulate_data.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/visualization/model_visualization.py` & `tsaugmentation-0.5.9/tsaugmentation/visualization/model_visualization.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/visualization/visualize_ridge_distance.py` & `tsaugmentation-0.5.9/tsaugmentation/visualization/visualize_ridge_distance.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation/visualization/visualize_transformed_datasets.py` & `tsaugmentation-0.5.9/tsaugmentation/visualization/visualize_transformed_datasets.py`

 * *Files identical despite different names*

### Comparing `tsaugmentation-0.5.8/tsaugmentation.egg-info/PKG-INFO` & `tsaugmentation-0.5.9/tsaugmentation.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsaugmentation
-Version: 0.5.8
+Version: 0.5.9
 Summary: Robust time series tsaugmentation for forecasting algorithms
 Author: Luis Roque
 Author-email: <roque0luis@gmail.com>
 Keywords: python,time series,hierarchical,forecasting,tsaugmentation,machine learning
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `tsaugmentation-0.5.8/tsaugmentation.egg-info/SOURCES.txt` & `tsaugmentation-0.5.9/tsaugmentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

