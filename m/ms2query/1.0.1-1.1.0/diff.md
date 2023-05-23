# Comparing `tmp/ms2query-1.0.1.tar.gz` & `tmp/ms2query-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ms2query-1.0.1.tar", last modified: Thu May 18 09:30:10 2023, max compression
+gzip compressed data, was "dist/ms2query-1.1.0.tar", last modified: Tue May 23 10:14:09 2023, max compression
```

## Comparing `ms2query-1.0.1.tar` & `ms2query-1.1.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:30:10.000000 ms2query-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    24177 2023-05-18 09:30:10.000000 ms2query-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20873 2023-05-18 09:29:57.000000 ms2query-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:30:10.000000 ms2query-1.0.1/ms2query/
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:30:10.000000 ms2query-1.0.1/ms2query/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21282 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/benchmarking/collect_test_data_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/benchmarking/create_accuracy_vs_recall_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/benchmarking/k_fold_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/benchmarking/visualize_mass_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/benchmarking/visualize_tanimoto_score_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/clean_and_filter_spectra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:30:10.000000 ms2query-1.0.1/ms2query/create_new_library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/create_new_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/create_new_library/add_classifire_classifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/create_new_library/calculate_tanimoto_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/create_new_library/create_sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/create_new_library/library_files_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/create_new_library/split_data_for_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/create_new_library/train_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/create_new_library/train_ms2deepscore.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/create_new_library/train_ms2query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    25085 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/ms2library.py
--rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/old_query_from_sqlite_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/query_from_sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/results_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/run_ms2query.py
--rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-05-18 09:29:57.000000 ms2query-1.0.1/ms2query/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:30:10.000000 ms2query-1.0.1/ms2query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24177 2023-05-18 09:30:10.000000 ms2query-1.0.1/ms2query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-18 09:30:10.000000 ms2query-1.0.1/ms2query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 09:30:10.000000 ms2query-1.0.1/ms2query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-18 09:30:10.000000 ms2query-1.0.1/ms2query.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 09:30:10.000000 ms2query-1.0.1/ms2query.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-18 09:30:10.000000 ms2query-1.0.1/ms2query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-18 09:30:10.000000 ms2query-1.0.1/ms2query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-18 09:30:10.000000 ms2query-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-18 09:29:57.000000 ms2query-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:30:10.000000 ms2query-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:29:57.000000 ms2query-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-18 09:29:57.000000 ms2query-1.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-18 09:29:57.000000 ms2query-1.0.1/tests/test_add_classifier_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-18 09:29:57.000000 ms2query-1.0.1/tests/test_calculate_tanimoto_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-05-18 09:29:57.000000 ms2query-1.0.1/tests/test_clean_and_filter_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-18 09:29:57.000000 ms2query-1.0.1/tests/test_collect_test_data_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-18 09:29:57.000000 ms2query-1.0.1/tests/test_library_files_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-05-18 09:29:57.000000 ms2query-1.0.1/tests/test_ms2library.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-18 09:29:57.000000 ms2query-1.0.1/tests/test_results_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-18 09:29:57.000000 ms2query-1.0.1/tests/test_run_ms2query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-18 09:29:57.000000 ms2query-1.0.1/tests/test_split_data_for_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-05-18 09:29:57.000000 ms2query-1.0.1/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-18 09:29:57.000000 ms2query-1.0.1/tests/test_train_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-18 09:29:57.000000 ms2query-1.0.1/tests/test_train_ms2deepscore.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-18 09:29:57.000000 ms2query-1.0.1/tests/test_train_ms2query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-18 09:29:57.000000 ms2query-1.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:14:09.000000 ms2query-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    24177 2023-05-23 10:14:09.000000 ms2query-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20873 2023-05-23 10:13:58.000000 ms2query-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:14:09.000000 ms2query-1.1.0/ms2query/
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:14:09.000000 ms2query-1.1.0/ms2query/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21282 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/benchmarking/collect_test_data_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/benchmarking/create_accuracy_vs_recall_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/benchmarking/k_fold_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/benchmarking/visualize_mass_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/benchmarking/visualize_tanimoto_score_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/clean_and_filter_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:14:09.000000 ms2query-1.1.0/ms2query/create_new_library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/create_new_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/create_new_library/add_classifire_classifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/create_new_library/calculate_tanimoto_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/create_new_library/create_sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/create_new_library/library_files_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/create_new_library/split_data_for_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/create_new_library/train_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/create_new_library/train_ms2deepscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/create_new_library/train_ms2query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22515 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/ms2library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/old_query_from_sqlite_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/query_from_sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/results_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/run_ms2query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-05-23 10:13:58.000000 ms2query-1.1.0/ms2query/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:14:09.000000 ms2query-1.1.0/ms2query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24177 2023-05-23 10:14:09.000000 ms2query-1.1.0/ms2query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-23 10:14:09.000000 ms2query-1.1.0/ms2query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 10:14:09.000000 ms2query-1.1.0/ms2query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 10:14:09.000000 ms2query-1.1.0/ms2query.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 10:14:09.000000 ms2query-1.1.0/ms2query.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-23 10:14:09.000000 ms2query-1.1.0/ms2query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 10:14:09.000000 ms2query-1.1.0/ms2query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-23 10:14:09.000000 ms2query-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-23 10:13:59.000000 ms2query-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:14:09.000000 ms2query-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:13:59.000000 ms2query-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-23 10:13:59.000000 ms2query-1.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-23 10:13:59.000000 ms2query-1.1.0/tests/test_add_classifier_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-23 10:13:59.000000 ms2query-1.1.0/tests/test_calculate_tanimoto_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-05-23 10:13:59.000000 ms2query-1.1.0/tests/test_clean_and_filter_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-23 10:13:59.000000 ms2query-1.1.0/tests/test_collect_test_data_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-23 10:13:59.000000 ms2query-1.1.0/tests/test_library_files_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-23 10:13:59.000000 ms2query-1.1.0/tests/test_ms2library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-23 10:13:59.000000 ms2query-1.1.0/tests/test_results_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-23 10:13:59.000000 ms2query-1.1.0/tests/test_run_ms2query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-23 10:13:59.000000 ms2query-1.1.0/tests/test_split_data_for_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-05-23 10:13:59.000000 ms2query-1.1.0/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-23 10:13:59.000000 ms2query-1.1.0/tests/test_train_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-23 10:13:59.000000 ms2query-1.1.0/tests/test_train_ms2deepscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-23 10:13:59.000000 ms2query-1.1.0/tests/test_train_ms2query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-23 10:13:59.000000 ms2query-1.1.0/tests/test_utils.py
```

### Comparing `ms2query-1.0.1/PKG-INFO` & `ms2query-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms2query
-Version: 1.0.1
+Version: 1.1.0
 Summary: Tool to query MS/MS spectra against mass spectral library
 Home-page: https://github.com/iomega/ms2query
 Author: Netherlands eScience Center
 Author-email: 
 License: Apache Software License 2.0
 Description: [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/iomega/ms2query/CI_build.yml)](https://github.com/iomega/ms2query/actions/workflows/CI_build.yml)
         ![GitHub](https://img.shields.io/github/license/iomega/ms2query)
```

### Comparing `ms2query-1.0.1/README.md` & `ms2query-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/ms2query/__init__.py` & `ms2query-1.1.0/ms2query/__init__.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/ms2query/benchmarking/collect_test_data_results.py` & `ms2query-1.1.0/ms2query/benchmarking/collect_test_data_results.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/ms2query/benchmarking/create_accuracy_vs_recall_plot.py` & `ms2query-1.1.0/ms2query/benchmarking/create_accuracy_vs_recall_plot.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/ms2query/benchmarking/k_fold_cross_validation.py` & `ms2query-1.1.0/ms2query/benchmarking/k_fold_cross_validation.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/ms2query/benchmarking/visualize_mass_distribution.py` & `ms2query-1.1.0/ms2query/benchmarking/visualize_mass_distribution.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/ms2query/benchmarking/visualize_tanimoto_score_distribution.py` & `ms2query-1.1.0/ms2query/benchmarking/visualize_tanimoto_score_distribution.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/ms2query/clean_and_filter_spectra.py` & `ms2query-1.1.0/ms2query/clean_and_filter_spectra.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/ms2query/create_new_library/add_classifire_classifications.py` & `ms2query-1.1.0/ms2query/create_new_library/add_classifire_classifications.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/ms2query/create_new_library/calculate_tanimoto_scores.py` & `ms2query-1.1.0/ms2query/create_new_library/calculate_tanimoto_scores.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/ms2query/create_new_library/create_sqlite_database.py` & `ms2query-1.1.0/ms2query/create_new_library/create_sqlite_database.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/ms2query/create_new_library/library_files_creator.py` & `ms2query-1.1.0/ms2query/create_new_library/library_files_creator.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/ms2query/create_new_library/split_data_for_training.py` & `ms2query-1.1.0/ms2query/create_new_library/split_data_for_training.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/ms2query/create_new_library/train_models.py` & `ms2query-1.1.0/ms2query/create_new_library/train_models.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/ms2query/create_new_library/train_ms2deepscore.py` & `ms2query-1.1.0/ms2query/create_new_library/train_ms2deepscore.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/ms2query/create_new_library/train_ms2query_model.py` & `ms2query-1.1.0/ms2query/create_new_library/train_ms2query_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,16 +49,15 @@
         ------
         validation_query_spectra:
             List of Spectrum objects
         """
         all_tanimoto_scores = pd.DataFrame()
         info_of_matches_with_tanimoto = pd.DataFrame()
         for query_spectrum in tqdm(query_spectra,
-                                   desc="Get scores and tanimoto scores",
-                                   disable=not self.ms2library.settings["progress_bars"]):
+                                   desc="Get scores and tanimoto scores"):
             results_table = self.ms2library.calculate_features_single_spectrum(query_spectrum,
                                                                                self.preselection_cut_off)
 
             # Get tanimoto scores
             library_spectrum_ids = list(results_table.data.index)
             tanimoto_scores = calculate_tanimoto_scores_with_library(self.ms2library.sqlite_library, query_spectrum,
                                                                      library_spectrum_ids)
```

### Comparing `ms2query-1.0.1/ms2query/ms2library.py` & `ms2query-1.1.0/ms2query/ms2library.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os.path
-from typing import Dict, List, Set, Tuple, Union, Optional
+from typing import Dict, List, Set, Tuple, Union, Optional, Iterator
 import numpy as np
 import pandas as pd
 from gensim.models import Word2Vec
 from matchms.Spectrum import Spectrum
 from ms2deepscore import MS2DeepScore
 from ms2deepscore.models import load_model as load_ms2ds_model
 from spec2vec.vector_operations import calc_vector, cosine_similarity_matrix
@@ -12,15 +12,15 @@
 from ms2query.query_from_sqlite_database import SqliteLibrary
 from ms2query.results_table import ResultsTable
 from ms2query.clean_and_filter_spectra import (clean_metadata,
                                                create_spectrum_documents,
                                                normalize_and_filter_peaks)
 from ms2query.utils import (column_names_for_output, load_ms2query_model,
                             load_pickled_file, SettingsRunMS2Query, predict_onnx_model,
-                            select_files_in_directory)
+                            select_files_in_directory, return_non_existing_file_name)
 
 
 class MS2Library:
     """Calculates scores of spectra in library and selects best matches
 
     For example
 
@@ -38,16 +38,15 @@
     """
     def __init__(self,
                  sqlite_file_name: str,
                  s2v_model_file_name: str,
                  ms2ds_model_file_name: str,
                  pickled_s2v_embeddings_file_name: str,
                  pickled_ms2ds_embeddings_file_name: str,
-                 ms2query_model_file_name: Union[str, None],
-                 **settings):
+                 ms2query_model_file_name: Union[str, None]):
         """
         Parameters
         ----------
         sqlite_file_name:
             The location at which the sqlite_file_is_stored. The file is
             expected to have 3 tables: tanimoto_scores, inchikeys and
             spectra_data.
@@ -61,28 +60,17 @@
             File location of a pickled file with Spec2Vec embeddings in a
             pd.Dataframe with as index the spectrum id.
         pickled_ms2ds_embeddings_file_name:
             File location of a pickled file with ms2ds embeddings in a
             pd.Dataframe with as index the spectrum id.
         ms2query_model_file_name:
             File location of ms2query model with .hdf5 extension.
-
-        **settings:
-            As additional parameters predefined settings can be changed.
-        spectrum_id_column_name:
-            The name of the column or key in dictionaries under which the
-            spectrum id is stored. Default = "spectrumid"
-        progress_bars:
-            If True progress bars will be shown of all methods. Default = True
         """
         # pylint: disable=too-many-arguments
 
-        # Change default settings to values given in **settings
-        self.settings = self._set_settings(settings)
-
         # Load models and set file locations
         assert os.path.isfile(sqlite_file_name), f"The given sqlite file does not exist: {sqlite_file_name}"
         self.sqlite_library = SqliteLibrary(sqlite_file_name)
 
         if ms2query_model_file_name is not None:
             self.ms2query_model = load_ms2query_model(ms2query_model_file_name)
 
@@ -113,38 +101,14 @@
             self.sqlite_library.get_inchikey_information()
         self.inchikey14s_of_spectra = {}
         for inchikey, list_of_spectrum_ids in \
                 self.spectra_of_inchikey14s.items():
             for spectrum_id in list_of_spectrum_ids:
                 self.inchikey14s_of_spectra[spectrum_id] = inchikey
 
-    @staticmethod
-    def _set_settings(new_settings: Dict[str, Union[str, bool]],
-                      ) -> Dict[str, Union[str, float]]:
-        """Changes default settings to new_settings
-
-        Args:
-        ------
-        new_settings:
-            Dictionary with settings that should be changed. Only the
-            keys given in default_settings can be used and the type has to be
-            the same as the type of the values in default settings.
-        """
-        # Set default settings
-        default_settings = {"spectrum_id_column_name": "spectrumid",
-                            "progress_bars": True}
-        for attribute in new_settings:
-            assert attribute in default_settings, \
-                f"Invalid argument in constructor:{attribute}"
-            assert isinstance(new_settings[attribute],
-                              type(default_settings[attribute])), \
-                f"Different type is expected for argument: {attribute}"
-            default_settings[attribute] = new_settings[attribute]
-        return default_settings
-
     def calculate_features_single_spectrum(self,
                                            query_spectrum: Spectrum,
                                            preselection_cut_off: int = 2000,
                                            filter_on_ionmode: Optional[str] = None) -> Optional[ResultsTable]:
         """Calculates a results table for a single spectrum"""
         query_spectrum = clean_metadata(query_spectrum)
         query_spectrum = normalize_and_filter_peaks(query_spectrum)
@@ -159,111 +123,98 @@
                       f"Instead the spectrum is in {query_ionmode} ionization mode.")
                 return None
         if query_ionmode != "n/a" and self.ionization_mode is not None:
             assert query_ionmode == self.ionization_mode, \
                 f"The spectrum is in {query_ionmode} ionization mode, while the library is for {self.ionization_mode} ionization mode. " \
                 f"Check the readme to download a library in the {query_ionmode} ionization mode"
 
-
         ms2deepscore_scores = self._get_all_ms2ds_scores(query_spectrum)
         # Initialize result table
         results_table = ResultsTable(preselection_cut_off=preselection_cut_off, ms2deepscores=ms2deepscore_scores,
                                      query_spectrum=query_spectrum, sqlite_library=self.sqlite_library)
         results_table = \
             self._calculate_features_for_random_forest_model(results_table)
         return results_table
 
-    def analog_search_return_results_tables(self,
-                                            query_spectra: List[Spectrum],
-                                            preselection_cut_off: int = 2000,
-                                            store_ms2deepscore_scores: bool = False
-                                            ) -> List[ResultsTable]:
-        """Returns a list with a ResultTable for each query spectrum
+    def analog_search_yield_df(self,
+                               query_spectra: List[Spectrum],
+                               settings: Optional[SettingsRunMS2Query] = None,
+                               progress_bar: bool = True
+                               ) -> Iterator[pd.DataFrame]:
+        """Runs ms2query on the query_spectra
+
+        Returns a generator returning dfs containing the results
 
         Args
         ----
         query_spectra:
             List of query spectra for which the best matches should be found
-        preselection_cut_off:
-            The number of spectra with the highest ms2ds that should be
-            selected. Default = 2000
+        settings:
+            Settings for running MS2Query, see SettingsRunMS2Query for details.
+        progress_bar:
+            If true a progress bar is shown.
         """
+        if settings is None:
+            settings = SettingsRunMS2Query()
+        # Create csv file if it does not exist already
         assert self.ms2query_model is not None, \
             "MS2Query model should be given when creating ms2library object"
 
-        result_tables = []
-        for i, query_spectrum in tqdm(enumerate(query_spectra),
-                                      desc="collecting matches info",
-                                      disable=not self.settings["progress_bars"],
-                                      total=len(query_spectra)):
+        for i, query_spectrum in \
+                tqdm(enumerate(query_spectra),
+                     desc="Predicting matches for query spectra",
+                     disable=not progress_bar,
+                     total=len(query_spectra)):
             query_spectrum.set("spectrum_nr", i+1)
-            results_table = self.calculate_features_single_spectrum(query_spectrum, preselection_cut_off)
-            if results_table is not None:
-                results_table = get_ms2query_model_prediction_single_spectrum(results_table, self.ms2query_model)
-                # To reduce the memory footprint the ms2deepscore scores are removed.
-                if not store_ms2deepscore_scores:
-                    results_table.ms2deepscores = pd.DataFrame()
-                result_tables.append(results_table)
+            results_table = self.calculate_features_single_spectrum(query_spectrum, settings.preselection_cut_off,
+                                                                    settings.filter_on_ion_mode)
+            if results_table is None:
+                print(f"Spectrum nr {i} was not stored, since it did not pass all cleaning steps")
             else:
-                result_tables.append(None)
-        return result_tables
+                results_table = get_ms2query_model_prediction_single_spectrum(results_table, self.ms2query_model)
+                results_df = results_table.export_to_dataframe(
+                    settings.nr_of_top_analogs_to_save,
+                    settings.minimal_ms2query_metascore,
+                    additional_metadata_columns=settings.additional_metadata_columns,
+                    additional_ms2query_score_columns=settings.additional_ms2query_score_columns)
+                yield results_df
 
     def analog_search_store_in_csv(self,
                                    query_spectra: List[Spectrum],
                                    results_csv_file_location: str,
                                    settings: Optional[SettingsRunMS2Query] = None
                                    ) -> None:
         """Stores the results of an analog in csv files.
 
-        This method is less memory intensive than analog_search_return_results_table,
-        since the results tables do not have to be kept in memory, since they are directly
-        stored in a csv file.
+        The results will be stored directly when created.
 
         Args
         ----
         query_spectra:
             List of query spectra for which the best matches should be found
         results_csv_file_location:
             file location were a csv file is created that stores the results
         settings:
             Settings for running MS2Query, see SettingsRunMS2Query for details.
         """
         if settings is None:
             settings = SettingsRunMS2Query()
-        # Create csv file if it does not exist already
-        assert not os.path.exists(results_csv_file_location), "Csv file location for results already exists"
-        assert self.ms2query_model is not None, \
-            "MS2Query model should be given when creating ms2library object"
+        results_csv_file_location = return_non_existing_file_name(results_csv_file_location)
 
         with open(results_csv_file_location, "w", encoding="utf-8") as csv_file:
             # Check if sqlite file has class annotations stored
             add_class_annotations: bool = self.sqlite_library.contains_class_annotation()
-
             csv_file.write(",".join(
                 column_names_for_output(True, add_class_annotations, settings.additional_metadata_columns,
                                         settings.additional_ms2query_score_columns)) + "\n")
 
-        for i, query_spectrum in \
-                tqdm(enumerate(query_spectra),
-                     desc="Predicting matches for query spectra",
-                     disable=not self.settings["progress_bars"],
-                     total=len(query_spectra)):
-            query_spectrum.set("spectrum_nr", i+1)
-            results_table = self.calculate_features_single_spectrum(query_spectrum, settings.preselection_cut_off,
-                                                                    settings.filter_on_ion_mode)
-            if results_table is None:
-                print(f"Spectrum nr {i} was not stored, since it did not pass all cleaning steps")
-            else:
-                results_table = get_ms2query_model_prediction_single_spectrum(results_table, self.ms2query_model)
-                results_df = results_table.export_to_dataframe(
-                    settings.nr_of_top_analogs_to_save,
-                    settings.minimal_ms2query_metascore,
-                    additional_metadata_columns=settings.additional_metadata_columns,
-                    additional_ms2query_score_columns=settings.additional_ms2query_score_columns)
-                results_df.to_csv(results_csv_file_location, mode="a", header=False, float_format="%.4f", index=False)
+        results_df_generator = self.analog_search_yield_df(query_spectra, settings)
+
+        for results_df in results_df_generator:
+            results_df.to_csv(results_csv_file_location, mode="a", header=False, float_format="%.4f", index=False)
 
     def _calculate_features_for_random_forest_model(self,
                                                     results_table: ResultsTable
                                                     ) -> ResultsTable:
         """Calculate the features for random forest model for selected spectra
 
         Args:
```

### Comparing `ms2query-1.0.1/ms2query/old_query_from_sqlite_functions.py` & `ms2query-1.1.0/ms2query/old_query_from_sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/ms2query/query_from_sqlite_database.py` & `ms2query-1.1.0/ms2query/query_from_sqlite_database.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/ms2query/results_table.py` & `ms2query-1.1.0/ms2query/results_table.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/ms2query/run_ms2query.py` & `ms2query-1.1.0/ms2query/run_ms2query.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/ms2query/utils.py` & `ms2query-1.1.0/ms2query/utils.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/ms2query.egg-info/PKG-INFO` & `ms2query-1.1.0/ms2query.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms2query
-Version: 1.0.1
+Version: 1.1.0
 Summary: Tool to query MS/MS spectra against mass spectral library
 Home-page: https://github.com/iomega/ms2query
 Author: Netherlands eScience Center
 Author-email: 
 License: Apache Software License 2.0
 Description: [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/iomega/ms2query/CI_build.yml)](https://github.com/iomega/ms2query/actions/workflows/CI_build.yml)
         ![GitHub](https://img.shields.io/github/license/iomega/ms2query)
```

### Comparing `ms2query-1.0.1/ms2query.egg-info/SOURCES.txt` & `ms2query-1.1.0/ms2query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/ms2query.egg-info/requires.txt` & `ms2query-1.1.0/ms2query.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/setup.py` & `ms2query-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/tests/conftest.py` & `ms2query-1.1.0/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,20 +41,18 @@
         "general_test_files/100_test_spectra_s2v_embeddings.pickle")
     ms2ds_model_file_name = os.path.join(
         path_to_tests_dir,
         "general_test_files/ms2ds_siamese_210301_5000_500_400.hdf5")
     ms2ds_embeddings_file_name = os.path.join(
         path_to_tests_dir,
         "general_test_files/100_test_spectra_ms2ds_embeddings.pickle")
-    spectrum_id_column_name = "spectrumid"
     ms2q_model_file_name = os.path.join(path_to_tests_dir,
         "general_test_files", "test_ms2q_rf_model.onnx")
     ms2library = MS2Library(sqlite_file_loc, spec2vec_model_file_loc, ms2ds_model_file_name,
-                            s2v_pickled_embeddings_file, ms2ds_embeddings_file_name, ms2q_model_file_name,
-                            spectrum_id_column_name=spectrum_id_column_name)
+                            s2v_pickled_embeddings_file, ms2ds_embeddings_file_name, ms2q_model_file_name)
     return ms2library
 
 
 @pytest.fixture(scope="package")
 def test_spectra():
     """Returns a list with two spectra
```

### Comparing `ms2query-1.0.1/tests/test_add_classifier_annotations.py` & `ms2query-1.1.0/tests/test_add_classifier_annotations.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/tests/test_calculate_tanimoto_scores.py` & `ms2query-1.1.0/tests/test_calculate_tanimoto_scores.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/tests/test_clean_and_filter_spectra.py` & `ms2query-1.1.0/tests/test_clean_and_filter_spectra.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/tests/test_collect_test_data_results.py` & `ms2query-1.1.0/tests/test_collect_test_data_results.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/tests/test_library_files_creator.py` & `ms2query-1.1.0/tests/test_library_files_creator.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/tests/test_ms2library.py` & `ms2query-1.1.0/tests/test_ms2library.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,45 +2,26 @@
 import os
 import numpy as np
 import pandas as pd
 import pytest
 from pandas.testing import assert_series_equal
 from ms2query.ms2library import (MS2Library,
                                  create_library_object_from_one_dir)
-from ms2query.utils import load_pickled_file, SettingsRunMS2Query
+from ms2query.utils import load_pickled_file, SettingsRunMS2Query, column_names_for_output
 from tests.test_utils import check_correct_results_csv_file
 
 
 @pytest.fixture
 def expected_ms2deespcore_scores():
     ms2dscores:pd.DataFrame = load_pickled_file(os.path.join(
         os.path.split(os.path.dirname(__file__))[0],
         'tests/test_files/test_files_ms2library/expected_ms2ds_scores.pickle'))
     return ms2dscores
 
 
-def test_ms2library_set_settings(ms2library):
-    """Tests creating a ms2library object"""
-
-    assert ms2library.settings["spectrum_id_column_name"] == "spectrumid", \
-        "Different value for attribute was expected"
-    assert ms2library.settings["progress_bars"] == True, \
-        "Different value for attribute was expected"
-
-
-def test_analog_search_no_ms2ds(ms2library, test_spectra):
-    """Check if no ms2deepscores are stored."""
-    cutoff = 20
-    results_without_ms2deepscores = ms2library.analog_search_return_results_tables(
-        test_spectra, cutoff, store_ms2deepscore_scores=False)
-    for i in range(len(results_without_ms2deepscores)):
-        assert results_without_ms2deepscores[i].ms2deepscores.empty, \
-            "No ms2deepscores should be stored in the result table"
-
-
 def test_get_all_ms2ds_scores(ms2library, test_spectra, expected_ms2deespcore_scores):
     """Test get_all_ms2ds_scores method of ms2library"""
     result = ms2library._get_all_ms2ds_scores(test_spectra[0])
     assert_series_equal(result, expected_ms2deespcore_scores)
 
 
 def test_get_s2v_scores(ms2library, test_spectra):
@@ -106,9 +87,26 @@
     path_to_tests_dir = os.path.join(
         os.path.split(os.path.dirname(__file__))[0],
         'tests/test_files/general_test_files')
     library = create_library_object_from_one_dir(path_to_tests_dir)
     assert isinstance(library, MS2Library)
 
 
-if __name__ == "__main__":
-    pass
+def test_analog_yield_df(ms2library, test_spectra, tmp_path):
+    settings = SettingsRunMS2Query(additional_metadata_columns=("spectrumid", ),)
+    result = ms2library.analog_search_yield_df(test_spectra, settings)
+    expected_headers = \
+        ['query_spectrum_nr', "ms2query_model_prediction", "precursor_mz_difference", "precursor_mz_query_spectrum",
+         "precursor_mz_analog", "inchikey", "analog_compound_name", "smiles", "spectrumid"]
+    check_correct_results_csv_file(list(result)[0], expected_headers, nr_of_rows_to_check=1)
+
+
+def test_analog_yield_df_additional_columns(ms2library, test_spectra, tmp_path):
+    settings = SettingsRunMS2Query(additional_metadata_columns=("charge", ),
+                                   additional_ms2query_score_columns=("s2v_score", "ms2ds_score",),)
+    result = ms2library.analog_search_yield_df(test_spectra, settings)
+    result_first_spectrum = list(result)[0]
+    check_correct_results_csv_file(result_first_spectrum,
+                                   column_names_for_output(True, True, ("charge",),
+                                                           ("s2v_score", "ms2ds_score",)),
+                                   nr_of_rows_to_check=1)
+
```

### Comparing `ms2query-1.0.1/tests/test_run_ms2query.py` & `ms2query-1.1.0/tests/test_run_ms2query.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/tests/test_split_data_for_training.py` & `ms2query-1.1.0/tests/test_split_data_for_training.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/tests/test_sqlite.py` & `ms2query-1.1.0/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/tests/test_train_models.py` & `ms2query-1.1.0/tests/test_train_models.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/tests/test_train_ms2deepscore.py` & `ms2query-1.1.0/tests/test_train_ms2deepscore.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/tests/test_train_ms2query_model.py` & `ms2query-1.1.0/tests/test_train_ms2query_model.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.0.1/tests/test_utils.py` & `ms2query-1.1.0/tests/test_utils.py`

 * *Files identical despite different names*

