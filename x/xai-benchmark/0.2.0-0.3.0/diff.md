# Comparing `tmp/xai-benchmark-0.2.0.tar.gz` & `tmp/xai-benchmark-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xai-benchmark-0.2.0.tar", last modified: Sun Apr  2 10:53:11 2023, max compression
+gzip compressed data, was "xai-benchmark-0.3.0.tar", last modified: Tue May 23 14:26:18 2023, max compression
```

## Comparing `xai-benchmark-0.2.0.tar` & `xai-benchmark-0.3.0.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-02 10:53:11.566394 xai-benchmark-0.2.0/
--rw-r--r--   0 ilia      (1000) ilia      (1000)     1080 2023-01-23 18:56:22.000000 xai-benchmark-0.2.0/LICENSE
--rw-rw-r--   0 ilia      (1000) ilia      (1000)    14563 2023-04-02 10:53:11.566394 xai-benchmark-0.2.0/PKG-INFO
--rw-r--r--   0 ilia      (1000) ilia      (1000)    14155 2023-03-26 14:25:58.000000 xai-benchmark-0.2.0/README.md
--rw-r--r--   0 ilia      (1000) ilia      (1000)       87 2023-01-23 18:56:22.000000 xai-benchmark-0.2.0/pyproject.toml
--rw-r--r--   0 ilia      (1000) ilia      (1000)      219 2023-04-02 10:53:11.566394 xai-benchmark-0.2.0/setup.cfg
--rw-r--r--   0 ilia      (1000) ilia      (1000)      766 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/setup.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-02 10:53:11.566394 xai-benchmark-0.2.0/xai_benchmark.egg-info/
--rw-rw-r--   0 ilia      (1000) ilia      (1000)    14563 2023-04-02 10:53:11.000000 xai-benchmark-0.2.0/xai_benchmark.egg-info/PKG-INFO
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     3092 2023-04-02 10:53:11.000000 xai-benchmark-0.2.0/xai_benchmark.egg-info/SOURCES.txt
--rw-rw-r--   0 ilia      (1000) ilia      (1000)        1 2023-04-02 10:53:11.000000 xai-benchmark-0.2.0/xai_benchmark.egg-info/dependency_links.txt
--rw-rw-r--   0 ilia      (1000) ilia      (1000)       46 2023-04-02 10:53:11.000000 xai-benchmark-0.2.0/xai_benchmark.egg-info/requires.txt
--rw-rw-r--   0 ilia      (1000) ilia      (1000)        5 2023-04-02 10:53:11.000000 xai-benchmark-0.2.0/xai_benchmark.egg-info/top_level.txt
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-02 10:53:11.562394 xai-benchmark-0.2.0/xaib/
--rw-r--r--   0 ilia      (1000) ilia      (1000)      165 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/__init__.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-02 10:53:11.562394 xai-benchmark-0.2.0/xaib/base/
--rw-r--r--   0 ilia      (1000) ilia      (1000)       67 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/base/__init__.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     4715 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/base/base.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-02 10:53:11.562394 xai-benchmark-0.2.0/xaib/cases/
--rw-rw-r--   0 ilia      (1000) ilia      (1000)        0 2023-03-12 11:08:35.000000 xai-benchmark-0.2.0/xaib/cases/__init__.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-02 10:53:11.562394 xai-benchmark-0.2.0/xaib/cases/example_selection/
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      203 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/cases/example_selection/__init__.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      443 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/cases/example_selection/continuity_case.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)      454 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/cases/example_selection/contrastivity_case.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)      507 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/cases/example_selection/correctness_case.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)      430 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/cases/example_selection/covariate_complexity_case.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-02 10:53:11.562394 xai-benchmark-0.2.0/xaib/cases/feature_importance/
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      291 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/cases/feature_importance/__init__.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      404 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/cases/feature_importance/coherence_case.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      380 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/cases/feature_importance/compactness_case.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      444 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/cases/feature_importance/continuity_case.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      406 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/cases/feature_importance/contrastivity_case.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      508 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/cases/feature_importance/correctness_case.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      431 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/cases/feature_importance/covariate_complexity_case.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-02 10:53:11.562394 xai-benchmark-0.2.0/xaib/datasets/
--rw-rw-r--   0 ilia      (1000) ilia      (1000)        0 2023-03-26 14:23:50.000000 xai-benchmark-0.2.0/xaib/datasets/__init__.py
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      944 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/datasets/synthetic_dataset.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-02 10:53:11.562394 xai-benchmark-0.2.0/xaib/evaluation/
--rw-r--r--   0 ilia      (1000) ilia      (1000)       84 2023-03-14 08:33:29.000000 xai-benchmark-0.2.0/xaib/evaluation/__init__.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     1078 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/evaluation/dataset_factory.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-02 10:53:11.562394 xai-benchmark-0.2.0/xaib/evaluation/example_selection/
--rw-r--r--   0 ilia      (1000) ilia      (1000)      136 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/evaluation/example_selection/__init__.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     1043 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/evaluation/example_selection/case_factory.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     1408 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/evaluation/example_selection/example_selection.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     1234 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/evaluation/example_selection/experiment_factory.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)      657 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/evaluation/example_selection/explainer_factory.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-02 10:53:11.562394 xai-benchmark-0.2.0/xaib/evaluation/feature_importance/
--rw-r--r--   0 ilia      (1000) ilia      (1000)      136 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/evaluation/feature_importance/__init__.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     1223 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/evaluation/feature_importance/case_factory.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     1759 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/evaluation/feature_importance/experiment_factory.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)      811 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/evaluation/feature_importance/explainer_factory.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     1190 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/evaluation/feature_importance/feature_importance.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     1670 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/evaluation/model_factory.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     6759 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/evaluation/utils.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-02 10:53:11.562394 xai-benchmark-0.2.0/xaib/explainers/
--rw-r--r--   0 ilia      (1000) ilia      (1000)        0 2023-01-23 18:56:22.000000 xai-benchmark-0.2.0/xaib/explainers/__init__.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-02 10:53:11.562394 xai-benchmark-0.2.0/xaib/explainers/example_selection/
--rw-r--r--   0 ilia      (1000) ilia      (1000)        0 2023-01-23 18:56:22.000000 xai-benchmark-0.2.0/xaib/explainers/example_selection/__init__.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)      316 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/explainers/example_selection/constant_explainer.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)      370 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/explainers/example_selection/knn_explainer.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)      431 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/explainers/example_selection/random_explainer.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-02 10:53:11.562394 xai-benchmark-0.2.0/xaib/explainers/feature_importance/
--rw-r--r--   0 ilia      (1000) ilia      (1000)        0 2023-01-23 18:56:22.000000 xai-benchmark-0.2.0/xaib/explainers/feature_importance/__init__.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)      393 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/explainers/feature_importance/constant_explainer.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     1110 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/explainers/feature_importance/lime_explainer.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)      334 2023-04-02 08:20:11.000000 xai-benchmark-0.2.0/xaib/explainers/feature_importance/linear_regression_explainer.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)      432 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/explainers/feature_importance/random_explainer.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)      500 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/explainers/feature_importance/shap_explainer.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-02 10:53:11.562394 xai-benchmark-0.2.0/xaib/metrics/
--rw-r--r--   0 ilia      (1000) ilia      (1000)        0 2023-03-14 08:33:29.000000 xai-benchmark-0.2.0/xaib/metrics/__init__.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-02 10:53:11.566394 xai-benchmark-0.2.0/xaib/metrics/example_selection/
--rw-r--r--   0 ilia      (1000) ilia      (1000)      236 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/metrics/example_selection/__init__.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     2568 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/metrics/example_selection/covariate_regularity.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     2457 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/metrics/example_selection/parameter_randomization_check.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     2169 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/metrics/example_selection/small_noise_check.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     1777 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/metrics/example_selection/target_discriminativeness.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-02 10:53:11.566394 xai-benchmark-0.2.0/xaib/metrics/feature_importance/
--rw-r--r--   0 ilia      (1000) ilia      (1000)      299 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/metrics/feature_importance/__init__.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     1752 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/metrics/feature_importance/covariate_regularity.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     2789 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/metrics/feature_importance/label_difference.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     1818 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/metrics/feature_importance/other_disagreement.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     2616 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/metrics/feature_importance/parameter_randomization_check.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     1848 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/metrics/feature_importance/small_noise_check.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     1608 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/metrics/feature_importance/sparsity.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-02 10:53:11.566394 xai-benchmark-0.2.0/xaib/models/
--rw-rw-r--   0 ilia      (1000) ilia      (1000)        0 2023-03-16 08:30:10.000000 xai-benchmark-0.2.0/xaib/models/__init__.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-02 10:53:11.566394 xai-benchmark-0.2.0/xaib/tests/
--rw-r--r--   0 ilia      (1000) ilia      (1000)       66 2023-01-23 18:56:22.000000 xai-benchmark-0.2.0/xaib/tests/__init__.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     1098 2023-01-23 18:56:22.000000 xai-benchmark-0.2.0/xaib/tests/conftest.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-02 10:53:11.566394 xai-benchmark-0.2.0/xaib/utils/
--rw-r--r--   0 ilia      (1000) ilia      (1000)      163 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/utils/__init__.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)     2569 2023-04-02 10:43:39.000000 xai-benchmark-0.2.0/xaib/utils/utils.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-05-23 14:26:18.283939 xai-benchmark-0.3.0/
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     1080 2023-01-23 18:56:22.000000 xai-benchmark-0.3.0/LICENSE
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)    14563 2023-05-23 14:26:18.283939 xai-benchmark-0.3.0/PKG-INFO
+-rw-r--r--   0 ilia      (1000) ilia      (1000)    14155 2023-05-23 14:25:44.000000 xai-benchmark-0.3.0/README.md
+-rw-r--r--   0 ilia      (1000) ilia      (1000)       87 2023-01-23 18:56:22.000000 xai-benchmark-0.3.0/pyproject.toml
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      219 2023-05-23 14:26:18.283939 xai-benchmark-0.3.0/setup.cfg
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      759 2023-05-04 14:19:21.000000 xai-benchmark-0.3.0/setup.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-05-23 14:26:18.283939 xai-benchmark-0.3.0/xai_benchmark.egg-info/
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)    14563 2023-05-23 14:26:18.000000 xai-benchmark-0.3.0/xai_benchmark.egg-info/PKG-INFO
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     3122 2023-05-23 14:26:18.000000 xai-benchmark-0.3.0/xai_benchmark.egg-info/SOURCES.txt
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)        1 2023-05-23 14:26:18.000000 xai-benchmark-0.3.0/xai_benchmark.egg-info/dependency_links.txt
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)       39 2023-05-23 14:26:18.000000 xai-benchmark-0.3.0/xai_benchmark.egg-info/requires.txt
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)        5 2023-05-23 14:26:18.000000 xai-benchmark-0.3.0/xai_benchmark.egg-info/top_level.txt
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-05-23 14:26:18.275939 xai-benchmark-0.3.0/xaib/
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      165 2023-05-04 14:19:28.000000 xai-benchmark-0.3.0/xaib/__init__.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-05-23 14:26:18.275939 xai-benchmark-0.3.0/xaib/base/
+-rw-r--r--   0 ilia      (1000) ilia      (1000)       67 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/base/__init__.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     5143 2023-05-01 16:19:03.000000 xai-benchmark-0.3.0/xaib/base/base.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-05-23 14:26:18.275939 xai-benchmark-0.3.0/xaib/cases/
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)        0 2023-03-12 11:08:35.000000 xai-benchmark-0.3.0/xaib/cases/__init__.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-05-23 14:26:18.279939 xai-benchmark-0.3.0/xaib/cases/example_selection/
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)      203 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/cases/example_selection/__init__.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)      443 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/cases/example_selection/continuity_case.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      454 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/cases/example_selection/contrastivity_case.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      507 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/cases/example_selection/correctness_case.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      430 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/cases/example_selection/covariate_complexity_case.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-05-23 14:26:18.279939 xai-benchmark-0.3.0/xaib/cases/feature_importance/
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)      291 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/cases/feature_importance/__init__.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)      404 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/cases/feature_importance/coherence_case.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)      380 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/cases/feature_importance/compactness_case.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)      444 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/cases/feature_importance/continuity_case.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)      406 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/cases/feature_importance/contrastivity_case.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)      508 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/cases/feature_importance/correctness_case.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)      431 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/cases/feature_importance/covariate_complexity_case.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-05-23 14:26:18.279939 xai-benchmark-0.3.0/xaib/datasets/
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)        0 2023-03-26 14:23:50.000000 xai-benchmark-0.3.0/xaib/datasets/__init__.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     1630 2023-05-01 16:17:03.000000 xai-benchmark-0.3.0/xaib/datasets/sk_dataset.py
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     1167 2023-05-01 16:16:56.000000 xai-benchmark-0.3.0/xaib/datasets/synthetic_dataset.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-05-23 14:26:18.279939 xai-benchmark-0.3.0/xaib/evaluation/
+-rw-r--r--   0 ilia      (1000) ilia      (1000)       84 2023-03-14 08:33:29.000000 xai-benchmark-0.3.0/xaib/evaluation/__init__.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     1605 2023-05-04 10:37:00.000000 xai-benchmark-0.3.0/xaib/evaluation/dataset_factory.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-05-23 14:26:18.279939 xai-benchmark-0.3.0/xaib/evaluation/example_selection/
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      136 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/evaluation/example_selection/__init__.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     1057 2023-05-01 16:19:03.000000 xai-benchmark-0.3.0/xaib/evaluation/example_selection/case_factory.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     1499 2023-05-23 14:24:55.000000 xai-benchmark-0.3.0/xaib/evaluation/example_selection/example_selection.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     1273 2023-05-01 16:19:03.000000 xai-benchmark-0.3.0/xaib/evaluation/example_selection/experiment_factory.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      671 2023-05-01 16:19:03.000000 xai-benchmark-0.3.0/xaib/evaluation/example_selection/explainer_factory.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-05-23 14:26:18.279939 xai-benchmark-0.3.0/xaib/evaluation/feature_importance/
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      136 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/evaluation/feature_importance/__init__.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     1316 2023-05-01 16:19:03.000000 xai-benchmark-0.3.0/xaib/evaluation/feature_importance/case_factory.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     1868 2023-05-01 16:19:03.000000 xai-benchmark-0.3.0/xaib/evaluation/feature_importance/experiment_factory.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      837 2023-05-01 16:19:03.000000 xai-benchmark-0.3.0/xaib/evaluation/feature_importance/explainer_factory.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     1695 2023-05-23 14:24:55.000000 xai-benchmark-0.3.0/xaib/evaluation/feature_importance/feature_importance.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     2436 2023-05-01 16:19:03.000000 xai-benchmark-0.3.0/xaib/evaluation/model_factory.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     9895 2023-05-01 16:19:03.000000 xai-benchmark-0.3.0/xaib/evaluation/utils.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-05-23 14:26:18.279939 xai-benchmark-0.3.0/xaib/explainers/
+-rw-r--r--   0 ilia      (1000) ilia      (1000)        0 2023-01-23 18:56:22.000000 xai-benchmark-0.3.0/xaib/explainers/__init__.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-05-23 14:26:18.279939 xai-benchmark-0.3.0/xaib/explainers/example_selection/
+-rw-r--r--   0 ilia      (1000) ilia      (1000)        0 2023-01-23 18:56:22.000000 xai-benchmark-0.3.0/xaib/explainers/example_selection/__init__.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      316 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/explainers/example_selection/constant_explainer.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      370 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/explainers/example_selection/knn_explainer.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      431 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/explainers/example_selection/random_explainer.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-05-23 14:26:18.279939 xai-benchmark-0.3.0/xaib/explainers/feature_importance/
+-rw-r--r--   0 ilia      (1000) ilia      (1000)        0 2023-01-23 18:56:22.000000 xai-benchmark-0.3.0/xaib/explainers/feature_importance/__init__.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      393 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/explainers/feature_importance/constant_explainer.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     1215 2023-04-02 20:24:49.000000 xai-benchmark-0.3.0/xaib/explainers/feature_importance/lime_explainer.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      334 2023-04-02 08:20:11.000000 xai-benchmark-0.3.0/xaib/explainers/feature_importance/linear_regression_explainer.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      432 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/explainers/feature_importance/random_explainer.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      500 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/explainers/feature_importance/shap_explainer.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-05-23 14:26:18.279939 xai-benchmark-0.3.0/xaib/metrics/
+-rw-r--r--   0 ilia      (1000) ilia      (1000)        0 2023-03-14 08:33:29.000000 xai-benchmark-0.3.0/xaib/metrics/__init__.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-05-23 14:26:18.279939 xai-benchmark-0.3.0/xaib/metrics/example_selection/
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      236 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/metrics/example_selection/__init__.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     2568 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/metrics/example_selection/covariate_regularity.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     2457 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/metrics/example_selection/parameter_randomization_check.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     2169 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/metrics/example_selection/small_noise_check.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     1777 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/metrics/example_selection/target_discriminativeness.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-05-23 14:26:18.283939 xai-benchmark-0.3.0/xaib/metrics/feature_importance/
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      299 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/metrics/feature_importance/__init__.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     1752 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/metrics/feature_importance/covariate_regularity.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     2789 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/metrics/feature_importance/label_difference.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     1818 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/metrics/feature_importance/other_disagreement.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     2614 2023-04-30 14:02:27.000000 xai-benchmark-0.3.0/xaib/metrics/feature_importance/parameter_randomization_check.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     1848 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/metrics/feature_importance/small_noise_check.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     1608 2023-05-07 17:04:06.000000 xai-benchmark-0.3.0/xaib/metrics/feature_importance/sparsity.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-05-23 14:26:18.283939 xai-benchmark-0.3.0/xaib/models/
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)        0 2023-03-16 08:30:10.000000 xai-benchmark-0.3.0/xaib/models/__init__.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-05-23 14:26:18.283939 xai-benchmark-0.3.0/xaib/tests/
+-rw-r--r--   0 ilia      (1000) ilia      (1000)       66 2023-01-23 18:56:22.000000 xai-benchmark-0.3.0/xaib/tests/__init__.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     1098 2023-01-23 18:56:22.000000 xai-benchmark-0.3.0/xaib/tests/conftest.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-05-23 14:26:18.283939 xai-benchmark-0.3.0/xaib/utils/
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      163 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/utils/__init__.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     2569 2023-04-02 10:43:39.000000 xai-benchmark-0.3.0/xaib/utils/utils.py
```

### Comparing `xai-benchmark-0.2.0/LICENSE` & `xai-benchmark-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xai-benchmark-0.2.0/PKG-INFO` & `xai-benchmark-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xai-benchmark
-Version: 0.2.0
+Version: 0.3.0
 Summary: Benchmark for Explainable AI methods
 Home-page: https://github.com/oxid15/xai-benchmark
 Author: Ilia Moiseev
 Author-email: ilia.moiseev.5@yandex.ru
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `xai-benchmark-0.2.0/README.md` & `xai-benchmark-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `xai-benchmark-0.2.0/setup.py` & `xai-benchmark-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="xai-benchmark",
-    version="0.2.0",
+    version="0.3.0",
     author="Ilia Moiseev",
     author_email="ilia.moiseev.5@yandex.ru",
     license="MIT",
     description="Benchmark for Explainable AI methods",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/oxid15/xai-benchmark",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     package_dir={"xaib": "./xaib"},
     packages=setuptools.find_packages(),
     python_requires=">=3.8",
-    install_requires=["cascade-ml>=0.7.2", "scikit-learn", "plotly", "kaleido"],
+    install_requires=["cascade-ml", "scikit-learn", "plotly", "kaleido"],
 )
```

### Comparing `xai-benchmark-0.2.0/xai_benchmark.egg-info/PKG-INFO` & `xai-benchmark-0.3.0/xai_benchmark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xai-benchmark
-Version: 0.2.0
+Version: 0.3.0
 Summary: Benchmark for Explainable AI methods
 Home-page: https://github.com/oxid15/xai-benchmark
 Author: Ilia Moiseev
 Author-email: ilia.moiseev.5@yandex.ru
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `xai-benchmark-0.2.0/xai_benchmark.egg-info/SOURCES.txt` & `xai-benchmark-0.3.0/xai_benchmark.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 ./xaib/cases/feature_importance/coherence_case.py
 ./xaib/cases/feature_importance/compactness_case.py
 ./xaib/cases/feature_importance/continuity_case.py
 ./xaib/cases/feature_importance/contrastivity_case.py
 ./xaib/cases/feature_importance/correctness_case.py
 ./xaib/cases/feature_importance/covariate_complexity_case.py
 ./xaib/datasets/__init__.py
+./xaib/datasets/sk_dataset.py
 ./xaib/datasets/synthetic_dataset.py
 ./xaib/evaluation/__init__.py
 ./xaib/evaluation/dataset_factory.py
 ./xaib/evaluation/model_factory.py
 ./xaib/evaluation/utils.py
 ./xaib/evaluation/example_selection/__init__.py
 ./xaib/evaluation/example_selection/case_factory.py
```

### Comparing `xai-benchmark-0.2.0/xaib/base/base.py` & `xai-benchmark-0.3.0/xaib/base/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .. import __version__ as version
 from typing import Union, List, Dict, Any, Callable
 from cascade import data as cdd
 from cascade import models as cdm
 
 
 class Dataset(cdd.Dataset):
     """
@@ -68,47 +69,50 @@
 
     def evaluate(
         self,
         name: str,
         expl: Explainer,
         batch_size: int = 1,
         expl_kwargs: Union[Dict[Any, Any], None] = None,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None:
         if expl_kwargs is None:
             expl_kwargs = {}
         value = self.compute(expl, batch_size=batch_size, **expl_kwargs, **kwargs)
 
         self.params["name"] = name
         self.params["direction"] = self.direction
         self.params["dataset"] = self._ds.name
         self.params["model"] = self._model.name
+        self.params["model_params"] = self._model.params
+        self.params["model_metrics"] = self._model.metrics
         self.metrics[self.name] = value
 
 
 class Case(cdm.Model):
     """
     Case is a collection of Metrics which represent some
     high-level property of an Explainer
     """
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.name = None
         self._metric_objs = dict()
+        self._meta_prefix.update({"xaib_version": version})
 
     def add_metric(self, name: str, metric: Metric) -> None:
         self._metric_objs[name] = metric
 
     def evaluate(
         self,
         name: str,
         expl: Explainer,
         metrics_kwargs: Union[Dict[str, Dict[Any, Any]], None] = None,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None:
         if metrics_kwargs is None:
             metrics_kwargs = {name: {} for _ in self._metric_objs}
 
         self.params["metric_params"] = dict()
         for m_name in self._metric_objs:
             mkwargs = {}
@@ -142,19 +146,25 @@
         else:
             kwargs = self._constructors_kwargs[name]
 
         constructor = self._constructors[name]
         return constructor(**kwargs)
 
     def get(self, name: str) -> Union[Dict[str, Any], Any]:
-        if name == "all":
-            return self._get_all()
-        return self._get(name)
+        try:
+            if name == "all":
+                return self._get_all()
+            return self._get(name)
+        except Exception as e:
+            raise RuntimeError(f"Failed to create object {name} in {self}") from e
 
     def add(
         self,
         name: str,
         constructor: Callable[[Any], Any],
         constr_kwargs: Union[Any, None] = None,
     ) -> None:
         self._constructors[name] = constructor
         self._constructors_kwargs[name] = constr_kwargs
+
+    def get_names(self):
+        return list(self._constructors.keys())
```

### Comparing `xai-benchmark-0.2.0/xaib/datasets/synthetic_dataset.py` & `xai-benchmark-0.3.0/xaib/datasets/synthetic_dataset.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,29 +2,37 @@
 
 from cascade import data as cdd
 from sklearn.datasets import make_classification
 from sklearn.model_selection import train_test_split
 
 
 class SyntheticDataset(cdd.SizedDataset):
-    def __init__(self, split, name=None, frac=0.8, *args, **kwargs) -> None:
+    def __init__(
+        self, split, name=None, frac=0.8, *args, n_classes=2, **kwargs
+    ) -> None:
         super().__init__(**kwargs)
         # Useful for different synthetic datasets
         if name is not None:
             self.name = name
         else:
             self.name = "synthetic"
 
-        x, y = make_classification(*args, **kwargs)
+        x, y = make_classification(*args, n_classes=n_classes, **kwargs)
+        self.labels = [i for i in range(n_classes)]
 
         train_x, test_x, train_y, test_y = train_test_split(x, y, train_size=frac)
 
         if split == "train":
             self.x, self.y = train_x, train_y
         elif split == "test":
             self.x, self.y = test_x, test_y
 
     def __len__(self) -> int:
         return len(self.x)
 
     def __getitem__(self, index: int) -> Dict[str, Any]:
         return {"item": self.x[index], "label": self.y[index]}
+
+    def get_meta(self):
+        meta = super().get_meta()
+        meta[0]["dataset_name"] = self.name
+        return meta
```

### Comparing `xai-benchmark-0.2.0/xaib/evaluation/dataset_factory.py` & `xai-benchmark-0.3.0/xaib/evaluation/dataset_factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,51 @@
 from ..base import Factory
 from ..datasets.synthetic_dataset import SyntheticDataset
+from ..datasets.sk_dataset import SkDataset
 
 
-def generate_dataset(name=None, frac: float = 0.9, **kwargs):
+def generate_dataset(ds_cls, *args, **kwargs):
     train_ds, test_ds = (
-        SyntheticDataset("train", name=name, frac=frac, **kwargs),
-        SyntheticDataset("test", name=name, frac=frac, **kwargs),
+        ds_cls(split="train", *args, **kwargs),
+        ds_cls(split="test", *args, **kwargs),
     )
     return train_ds, test_ds
 
 
 class DatasetFactory(Factory):
     def __init__(self) -> None:
         super().__init__()
         self._constructors["synthetic"] = lambda: generate_dataset(
-            n_samples=100,
+            SyntheticDataset,
+            n_samples=1000,
             n_features=14,
             random_state=0,
             n_informative=14,
             n_redundant=0,
             n_repeated=0,
             n_clusters_per_class=1,
             frac=0.8,
         )
         self._constructors["synthetic_noisy"] = lambda: generate_dataset(
+            SyntheticDataset,
             name="synthetic_noisy",
-            n_samples=100,
+            n_samples=1000,
             n_features=14,
             random_state=0,
             n_informative=7,
             n_redundant=5,
             n_repeated=2,
             n_clusters_per_class=2,
             frac=0.8,
         )
+        self._constructors["iris"] = lambda: generate_dataset(
+            SkDataset, "iris", frac=0.8
+        )
+        self._constructors["wine"] = lambda: generate_dataset(
+            SkDataset, "wine", frac=0.8
+        )
+        self._constructors["digits"] = lambda: generate_dataset(
+            SkDataset, "digits", frac=0.8
+        )
+        self._constructors["breast_cancer"] = lambda: generate_dataset(
+            SkDataset, "breast_cancer", frac=0.8
+        )
```

### Comparing `xai-benchmark-0.2.0/xaib/evaluation/example_selection/case_factory.py` & `xai-benchmark-0.3.0/xaib/evaluation/example_selection/case_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 def correctness(test_ds, model):
     noisy_model = RandomNeighborsBaseline(len(test_ds))
 
     return CorrectnessCase(test_ds, model, noisy_model)
 
 
 class CaseFactory(Factory):
-    def __init__(self, test_ds: Dataset, model: Model) -> None:
+    def __init__(self, test_ds: Dataset = None, model: Model = None) -> None:
         super().__init__()
         self._constructors["continuity"] = lambda: continuity(test_ds, model)
         self._constructors["contrastivity"] = lambda: ContrastivityCase(test_ds, model)
         self._constructors["covariate_complexity"] = lambda: CovariateComplexityCase(
             test_ds, model
         )
         self._constructors["correctness"] = lambda: correctness(test_ds, model)
```

### Comparing `xai-benchmark-0.2.0/xaib/evaluation/example_selection/example_selection.py` & `xai-benchmark-0.3.0/xaib/evaluation/example_selection/example_selection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 import os
 import sys
 
-from cascade import data as cdd
 from cascade.models import ModelRepo
 from cascade.utils.sk_model import SkModel
 from xaib.evaluation import DatasetFactory, ModelFactory
-from xaib.evaluation.example_selection import ExperimentFactory, ExplainerFactory
+from xaib.evaluation.example_selection import (
+    ExperimentFactory,
+    ExplainerFactory,
+    CaseFactory,
+)
 
 SCRIPT_DIR = os.path.dirname(__file__)
 # xaib/results/...
 REPO_PATH = os.path.join(
     os.path.dirname(os.path.dirname(SCRIPT_DIR)), "results", "example_selection"
 )
 
 sys.path.append(os.path.abspath(os.path.dirname(SCRIPT_DIR)))
-from utils import WrapperModel, visualize_results
-
+from utils import Setup, visualize_results
 
-class SkWrapper(SkModel):
-    def __init__(self, *args, blocks=None, name=None, **kwargs) -> None:
-        super().__init__(*args, blocks=blocks, **kwargs)
-        self.name = name
 
-
-BS = 5
+BS = 100
 
 # Overwrite previous run
 ModelRepo(REPO_PATH, overwrite=True)
 
-for dataset in ["synthetic_noisy", "synthetic"]:
-    for model in ["knn"]:
-        train_ds, test_ds = DatasetFactory().get(dataset)
-        print(train_ds.get_meta())
-
-        model = ModelFactory(train_ds, test_ds).get(model)
-        print(model.get_meta())
-
-        explainers = ExplainerFactory(train_ds, model).get("all")
-        experiment_factory = ExperimentFactory(
-            REPO_PATH, explainers, test_ds, model, BS
-        )
-
-        experiments = experiment_factory.get("all")
-        for name in experiments:
-            experiments[name]()
+factories = (DatasetFactory(), ModelFactory(), ExplainerFactory(), CaseFactory())
+setups = [Setup(*factories, models=["knn"])]
+
+for setup in setups:
+    for dataset in setup.datasets:
+        for model in setup.models:
+            train_ds, test_ds = DatasetFactory().get(dataset)
+            print(train_ds.get_meta())
+
+            model = ModelFactory(train_ds, test_ds).get(model)
+            print(model.get_meta())
+
+            explainers = {
+                explainer: ExplainerFactory(train_ds, model).get(explainer)
+                for explainer in setup.explainers
+            }
+
+            experiment_factory = ExperimentFactory(
+                REPO_PATH, explainers, test_ds, model, BS
+            )
+
+            for case in setup.cases:
+                experiment = experiment_factory.get(case)
+                experiment()
 
 visualize_results(REPO_PATH, REPO_PATH)
```

### Comparing `xai-benchmark-0.2.0/xaib/evaluation/example_selection/experiment_factory.py` & `xai-benchmark-0.3.0/xaib/evaluation/example_selection/experiment_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from xaib import Factory
 from xaib.evaluation.example_selection import CaseFactory
 
 from ..utils import experiment
 
 
 class ExperimentFactory(Factory):
-    def __init__(self, repo_path, explainers, test_ds, model, batch_size) -> None:
+    def __init__(
+        self, repo_path=None, explainers=None, test_ds=None, model=None, batch_size=None
+    ) -> None:
         super().__init__()
 
         case_factory = CaseFactory(test_ds, model)
 
         @experiment(repo_path, explainers=explainers, batch_size=batch_size)
         def continuity():
             return case_factory.get("continuity")
```

### Comparing `xai-benchmark-0.2.0/xaib/evaluation/example_selection/explainer_factory.py` & `xai-benchmark-0.3.0/xaib/evaluation/feature_importance/explainer_factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from ...base import Dataset, Factory, Model
-from ...explainers.example_selection.constant_explainer import ConstantExplainer
-from ...explainers.example_selection.knn_explainer import KNNExplainer
-from ...explainers.example_selection.random_explainer import RandomExplainer
+from ...explainers.feature_importance.constant_explainer import ConstantExplainer
+from ...explainers.feature_importance.lime_explainer import LimeExplainer
+from ...explainers.feature_importance.random_explainer import RandomExplainer
+from ...explainers.feature_importance.shap_explainer import ShapExplainer
 
 
 class ExplainerFactory(Factory):
-    def __init__(self, train_ds: Dataset, model: Model) -> None:
+    def __init__(
+        self, train_ds: Dataset = None, model: Model = None, labels=None
+    ) -> None:
         super().__init__()
-        self._constructors["const"] = lambda: ConstantExplainer(
-            train_ds, train_ds[0]["item"]
-        )
-        self._constructors["random"] = lambda: RandomExplainer(train_ds)
-        self._constructors["knn"] = lambda: KNNExplainer(train_ds)
+        self._constructors["const"] = lambda: ConstantExplainer(constant=1)
+        self._constructors["random"] = lambda: RandomExplainer(shift=-15, magnitude=10)
+        self._constructors["shap"] = lambda: ShapExplainer(train_ds)
+        self._constructors["lime"] = lambda: LimeExplainer(train_ds, labels=labels)
```

### Comparing `xai-benchmark-0.2.0/xaib/evaluation/feature_importance/case_factory.py` & `xai-benchmark-0.3.0/xaib/evaluation/feature_importance/case_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,31 +3,35 @@
     CoherenceCase,
     CompactnessCase,
     ContinuityCase,
     ContrastivityCase,
     CorrectnessCase,
     CovariateComplexityCase,
 )
-from ..utils import NoiseApplier, RandomBinBaseline
+from ..utils import NoiseApplier, RandomBaseline
 
 
-def correctness(test_ds, model):
-    noisy_model = RandomBinBaseline()
+def correctness(test_ds, model, labels):
+    noisy_model = RandomBaseline(labels=labels)
     return CorrectnessCase(test_ds, model, noisy_model)
 
 
 def continuity(test_ds, model):
     test_ds_noisy = NoiseApplier(test_ds, multiplier=0.01)
     return ContinuityCase(test_ds, test_ds_noisy, model, multiplier=0.01)
 
 
 class CaseFactory(Factory):
-    def __init__(self, test_ds: Dataset, model: Model) -> None:
+    def __init__(
+        self, test_ds: Dataset = None, model: Model = None, labels=None
+    ) -> None:
         super().__init__()
-        self._constructors["correctness"] = lambda: correctness(test_ds, model)
+        self._constructors["correctness"] = lambda: correctness(
+            test_ds, model, labels=labels
+        )
         self._constructors["continuity"] = lambda: continuity(test_ds, model)
         self._constructors["contrastivity"] = lambda: ContrastivityCase(test_ds, model)
         self._constructors["coherence"] = lambda: CoherenceCase(test_ds, model)
         self._constructors["compactness"] = lambda: CompactnessCase(test_ds, model)
         self._constructors["covariate_complexity"] = lambda: CovariateComplexityCase(
             test_ds, model
         )
```

### Comparing `xai-benchmark-0.2.0/xaib/evaluation/feature_importance/experiment_factory.py` & `xai-benchmark-0.3.0/xaib/evaluation/feature_importance/experiment_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 from xaib import Factory
 from xaib.evaluation.feature_importance import CaseFactory
 
 from ..utils import experiment
 
 
 class ExperimentFactory(Factory):
-    def __init__(self, repo_path, explainers, test_ds, model, batch_size) -> None:
+    def __init__(
+        self,
+        repo_path=None,
+        explainers=None,
+        test_ds=None,
+        model=None,
+        labels=None,
+        batch_size=None,
+    ) -> None:
         super().__init__()
 
-        case_factory = CaseFactory(test_ds, model)
+        case_factory = CaseFactory(test_ds, model, labels)
 
         @experiment(repo_path, explainers=explainers, batch_size=batch_size)
         def correctness():
             return case_factory.get("correctness")
 
         @experiment(repo_path, explainers=explainers, batch_size=batch_size)
         def continuity():
```

### Comparing `xai-benchmark-0.2.0/xaib/evaluation/feature_importance/feature_importance.py` & `xai-benchmark-0.3.0/xaib/evaluation/feature_importance/feature_importance.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,61 @@
+import matplotlib
+
+matplotlib.use("TkAgg")
+
 import os
 import sys
 
 from cascade.models import ModelRepo
 from xaib.evaluation import DatasetFactory, ModelFactory
-from xaib.evaluation.feature_importance import ExperimentFactory, ExplainerFactory
+from xaib.evaluation.feature_importance import (
+    ExperimentFactory,
+    ExplainerFactory,
+    CaseFactory,
+)
 
 SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
 BASE_DIR = os.path.dirname(SCRIPT_DIR)
 PROJECT_DIR = os.path.dirname(os.path.dirname(BASE_DIR))
 sys.path.append(PROJECT_DIR)
 
-from xaib.evaluation.utils import visualize_results
+from xaib.evaluation.utils import visualize_results, Setup
 
-REPO_PATH = os.path.join(os.path.dirname(BASE_DIR), "results", "feature_importance")
-BS = 5
 
+REPO_PATH = os.path.join(os.path.dirname(BASE_DIR), "results", "feature_importance")
+BS = 100
 
 # Overwrite previous run
 ModelRepo(REPO_PATH, overwrite=True)
 
-for dataset in ["synthetic_noisy", "synthetic"]:
-    for model in ["svm"]:
-        train_ds, test_ds = DatasetFactory().get(dataset)
-        print(train_ds.get_meta())
-
-        model = ModelFactory(train_ds, test_ds).get(model)
-        print(model.get_meta())
-
-        explainers = ExplainerFactory(train_ds, model).get("all")
-        experiment_factory = ExperimentFactory(
-            REPO_PATH, explainers, test_ds, model, BS
-        )
-
-        experiments = experiment_factory.get("all")
-        for name in experiments:
-            experiments[name]()
+factories = (DatasetFactory(), ModelFactory(), ExplainerFactory(), CaseFactory())
+setups = [Setup(*factories, models_except=["knn"])]
+
+for setup in setups:
+    for dataset in setup.datasets:
+        for model in setup.models:
+            print(dataset, model)
+
+            train_ds, test_ds = DatasetFactory().get(dataset)
+            print(train_ds.get_meta())
+
+            labels = train_ds.labels
+
+            model = ModelFactory(train_ds, test_ds).get(model)
+            print(model.get_meta())
+
+            explainers = {
+                explainer: ExplainerFactory(train_ds, model, labels=labels).get(
+                    explainer
+                )
+                for explainer in setup.explainers
+            }
+
+            experiment_factory = ExperimentFactory(
+                REPO_PATH, explainers, test_ds, model, labels, BS
+            )
+
+            for case in setup.cases:
+                experiment = experiment_factory.get(case)
+                experiment()
 
 visualize_results(REPO_PATH, REPO_PATH)
```

### Comparing `xai-benchmark-0.2.0/xaib/evaluation/model_factory.py` & `xai-benchmark-0.3.0/xaib/evaluation/model_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,68 @@
 import numpy as np
 from cascade.utils.sk_model import SkModel
 from sklearn.metrics import f1_score
 from sklearn.neighbors import KNeighborsClassifier
+from sklearn.neural_network import MLPClassifier
 from sklearn.svm import SVC
 
 from ..base import Factory
 
 
 class SkWrapper(SkModel):
     def __init__(self, *args, blocks=None, name=None, **kwargs) -> None:
         super().__init__(*args, blocks=blocks, **kwargs)
         self.name = name
 
 
+# TODO: merge code repetition
 def svm(train_ds, test_ds):
     X_train, Y_train = [x["item"] for x in train_ds], [x["label"] for x in train_ds]
     X_test, Y_test = [x["item"] for x in test_ds], [x["label"] for x in test_ds]
 
     X_train = np.array(X_train)
     Y_train = np.array(Y_train, dtype=int)
     X_test = np.array(X_test)
     Y_test = np.array(Y_test, dtype=int)
 
     model = SkWrapper(blocks=[SVC(probability=True)], name="svm")
     model.fit(X_train, Y_train)
-    model.evaluate(X_test, Y_test, {"f1": f1_score})
+    model.evaluate(X_test, Y_test, {"f1": lambda x, y: f1_score(x, y, average="macro")})
     return model
 
 
 def knn(train_ds, test_ds):
     X_train, Y_train = [x["item"] for x in train_ds], [x["label"] for x in train_ds]
     X_test, Y_test = [x["item"] for x in test_ds], [x["label"] for x in test_ds]
 
     X_train = np.array(X_train)
     Y_train = np.array(Y_train, dtype=int)
     X_test = np.array(X_test)
     Y_test = np.array(Y_test, dtype=int)
 
-    model = SkWrapper(blocks=[KNeighborsClassifier(n_neighbors=3)], name="svm")
+    model = SkWrapper(blocks=[KNeighborsClassifier(n_neighbors=3)], name="knn")
     model.fit(X_train, Y_train)
-    model.evaluate(X_test, Y_test, {"f1": f1_score})
+    model.evaluate(X_test, Y_test, {"f1": lambda x, y: f1_score(x, y, average="macro")})
+    return model
+
+
+def nn(train_ds, test_ds):
+    X_train, Y_train = [x["item"] for x in train_ds], [x["label"] for x in train_ds]
+    X_test, Y_test = [x["item"] for x in test_ds], [x["label"] for x in test_ds]
+
+    X_train = np.array(X_train)
+    Y_train = np.array(Y_train, dtype=int)
+    X_test = np.array(X_test)
+    Y_test = np.array(Y_test, dtype=int)
+
+    model = SkWrapper(blocks=[MLPClassifier()], name="nn")
+    model.fit(X_train, Y_train)
+    model.evaluate(X_test, Y_test, {"f1": lambda x, y: f1_score(x, y, average="macro")})
     return model
 
 
 class ModelFactory(Factory):
-    def __init__(self, train_ds, test_ds) -> None:
+    def __init__(self, train_ds=None, test_ds=None) -> None:
         super().__init__()
         self._constructors["svm"] = lambda: svm(train_ds, test_ds)
         self._constructors["knn"] = lambda: knn(train_ds, test_ds)
+        self._constructors["nn"] = lambda: nn(train_ds, test_ds)
```

### Comparing `xai-benchmark-0.2.0/xaib/explainers/feature_importance/lime_explainer.py` & `xai-benchmark-0.3.0/xaib/explainers/feature_importance/lime_explainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,26 +6,29 @@
 
 class LimeExplainer(Explainer):
     def __init__(self, train_ds, labels, *args, meta_prefix=None, **kwargs) -> None:
         super().__init__(*args, meta_prefix=meta_prefix, **kwargs)
 
         data = np.array([item["item"] for item in train_ds])
         self._explainer = lime_tabular.LimeTabularExplainer(
-            data, feature_selection="none"
+            data, feature_selection="none", training_labels=labels
         )
         self._labels = labels
 
     def predict(self, x, model):
         if not hasattr(model, "predict_proba"):
             raise ValueError("The model should have `predict_proba` method")
 
         explanations = []
         for item in x:
             ex = self._explainer.explain_instance(
-                item, model.predict_proba, labels=self._labels
+                item,
+                model.predict_proba,
+                labels=self._labels,
+                num_features=len(self._labels),
             )
             predicted_label = np.argmax(ex.predict_proba)
             ex = ex.as_map()[predicted_label]
             # Sorts by the feature order
             importance_scores = [item[1] for item in sorted(ex)]
             explanations.append(importance_scores)
         return np.asarray(explanations)
```

### Comparing `xai-benchmark-0.2.0/xaib/metrics/example_selection/covariate_regularity.py` & `xai-benchmark-0.3.0/xaib/metrics/example_selection/covariate_regularity.py`

 * *Files identical despite different names*

### Comparing `xai-benchmark-0.2.0/xaib/metrics/example_selection/parameter_randomization_check.py` & `xai-benchmark-0.3.0/xaib/metrics/example_selection/parameter_randomization_check.py`

 * *Files identical despite different names*

### Comparing `xai-benchmark-0.2.0/xaib/metrics/example_selection/small_noise_check.py` & `xai-benchmark-0.3.0/xaib/metrics/example_selection/small_noise_check.py`

 * *Files identical despite different names*

### Comparing `xai-benchmark-0.2.0/xaib/metrics/example_selection/target_discriminativeness.py` & `xai-benchmark-0.3.0/xaib/metrics/example_selection/target_discriminativeness.py`

 * *Files identical despite different names*

### Comparing `xai-benchmark-0.2.0/xaib/metrics/feature_importance/covariate_regularity.py` & `xai-benchmark-0.3.0/xaib/metrics/feature_importance/covariate_regularity.py`

 * *Files identical despite different names*

### Comparing `xai-benchmark-0.2.0/xaib/metrics/feature_importance/label_difference.py` & `xai-benchmark-0.3.0/xaib/metrics/feature_importance/label_difference.py`

 * *Files identical despite different names*

### Comparing `xai-benchmark-0.2.0/xaib/metrics/feature_importance/other_disagreement.py` & `xai-benchmark-0.3.0/xaib/metrics/feature_importance/other_disagreement.py`

 * *Files identical despite different names*

### Comparing `xai-benchmark-0.2.0/xaib/metrics/feature_importance/parameter_randomization_check.py` & `xai-benchmark-0.3.0/xaib/metrics/feature_importance/parameter_randomization_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     def __init__(
         self, ds: Dataset, model: Model, noisy_model: Model, **kwargs: Any
     ) -> None:
         super().__init__(ds, model, **kwargs)
         self._noisy_model = noisy_model
         self.name = "parameter_randomization_check"
-        self.direction = "down"
+        self.direction = "up"
 
     def compute(
         self,
         expl: Explainer,
         batch_size: int = 1,
         expl_kwargs: Union[Dict[Any, Any], None] = None,
         expl_noisy_kwargs: Union[Dict[Any, Any], None] = None,
```

### Comparing `xai-benchmark-0.2.0/xaib/metrics/feature_importance/small_noise_check.py` & `xai-benchmark-0.3.0/xaib/metrics/feature_importance/small_noise_check.py`

 * *Files identical despite different names*

### Comparing `xai-benchmark-0.2.0/xaib/metrics/feature_importance/sparsity.py` & `xai-benchmark-0.3.0/xaib/metrics/feature_importance/sparsity.py`

 * *Files identical despite different names*

### Comparing `xai-benchmark-0.2.0/xaib/tests/conftest.py` & `xai-benchmark-0.3.0/xaib/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xai-benchmark-0.2.0/xaib/utils/utils.py` & `xai-benchmark-0.3.0/xaib/utils/utils.py`

 * *Files identical despite different names*

