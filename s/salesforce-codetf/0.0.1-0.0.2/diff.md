# Comparing `tmp/salesforce-codetf-0.0.1.tar.gz` & `tmp/salesforce-codetf-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesforce-codetf-0.0.1.tar", last modified: Mon May 22 21:32:45 2023, max compression
+gzip compressed data, was "salesforce-codetf-0.0.2.tar", last modified: Tue May 23 19:01:45 2023, max compression
```

## Comparing `salesforce-codetf-0.0.1.tar` & `salesforce-codetf-0.0.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-22 21:32:45.770820 salesforce-codetf-0.0.1/
--rw-r--r--   0 nghi.bui   (503) staff       (20)    19491 2023-05-22 21:32:45.771116 salesforce-codetf-0.0.1/PKG-INFO
--rw-r--r--   0 nghi.bui   (503) staff       (20)    16625 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.1/README.md
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-22 21:32:45.750292 salesforce-codetf-0.0.1/codetf/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      620 2023-03-20 20:11:15.000000 salesforce-codetf-0.0.1/codetf/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-22 21:32:45.751848 salesforce-codetf-0.0.1/codetf/code_utility/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.1/codetf/code_utility/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-22 21:32:45.752407 salesforce-codetf-0.0.1/codetf/code_utility/apex/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.1/codetf/code_utility/apex/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     5146 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.1/codetf/code_utility/apex/apex_code_utility.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     5116 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.1/codetf/code_utility/ast_parser.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      846 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.1/codetf/code_utility/base_utility.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-22 21:32:45.753075 salesforce-codetf-0.0.1/codetf/code_utility/java/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.1/codetf/code_utility/java/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2480 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.1/codetf/code_utility/java/java_code_utility.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      221 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.1/codetf/code_utility/language_specific_utility.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-22 21:32:45.753617 salesforce-codetf-0.0.1/codetf/code_utility/python/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.1/codetf/code_utility/python/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2450 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.1/codetf/code_utility/python/python_code_utility.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-22 21:32:45.754238 salesforce-codetf-0.0.1/codetf/common/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     6365 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.1/codetf/common/registry.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)    14084 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.1/codetf/common/utils.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-22 21:32:45.756735 salesforce-codetf-0.0.1/codetf/data_utility/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.1/codetf/data_utility/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1123 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.1/codetf/data_utility/apps_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1347 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.1/codetf/data_utility/base_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     4292 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.1/codetf/data_utility/codexglue_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1149 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.1/codetf/data_utility/human_eval_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1114 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.1/codetf/data_utility/mpp_dataset.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1851 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.1/codetf/data_utility/util.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-22 21:32:45.757922 salesforce-codetf-0.0.1/codetf/models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3204 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.1/codetf/models/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2262 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.1/codetf/models/base_model.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-22 21:32:45.758396 salesforce-codetf-0.0.1/codetf/models/bert_models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2773 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.1/codetf/models/bert_models/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-22 21:32:45.758762 salesforce-codetf-0.0.1/codetf/models/causal_lm_models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3062 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.1/codetf/models/causal_lm_models/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-22 21:32:45.759183 salesforce-codetf-0.0.1/codetf/models/codet5_models/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     3096 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.1/codetf/models/codet5_models/__init__.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-22 21:32:45.760511 salesforce-codetf-0.0.1/codetf/performance/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.1/codetf/performance/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2674 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.1/codetf/performance/evaluation_metric.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     4443 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.1/codetf/performance/model_evaluator.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-22 21:32:45.761924 salesforce-codetf-0.0.1/codetf/trainer/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     6263 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.1/codetf/trainer/base_trainer.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1303 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.1/codetf/trainer/causal_lm_trainer.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2048 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.1/codetf/trainer/codet5_trainer.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-22 21:32:45.764247 salesforce-codetf-0.0.1/salesforce_codetf.egg-info/
--rw-r--r--   0 nghi.bui   (503) staff       (20)    19491 2023-05-22 21:32:45.000000 salesforce-codetf-0.0.1/salesforce_codetf.egg-info/PKG-INFO
--rw-r--r--   0 nghi.bui   (503) staff       (20)     2043 2023-05-22 21:32:45.000000 salesforce-codetf-0.0.1/salesforce_codetf.egg-info/SOURCES.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)        1 2023-05-22 21:32:45.000000 salesforce-codetf-0.0.1/salesforce_codetf.egg-info/dependency_links.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)        1 2023-05-22 21:32:45.000000 salesforce-codetf-0.0.1/salesforce_codetf.egg-info/not-zip-safe
--rw-r--r--   0 nghi.bui   (503) staff       (20)      375 2023-05-22 21:32:45.000000 salesforce-codetf-0.0.1/salesforce_codetf.egg-info/requires.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)       91 2023-05-22 21:32:45.000000 salesforce-codetf-0.0.1/salesforce_codetf.egg-info/top_level.txt
--rw-r--r--   0 nghi.bui   (503) staff       (20)       79 2023-05-22 21:32:45.771837 salesforce-codetf-0.0.1/setup.cfg
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1030 2023-05-22 21:32:12.000000 salesforce-codetf-0.0.1/setup.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-22 21:32:45.766157 salesforce-codetf-0.0.1/test_code_utilities/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.1/test_code_utilities/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1063 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.1/test_code_utilities/test_extract_code_attributre.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      528 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.1/test_code_utilities/test_parse_code.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1369 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.1/test_code_utilities/test_remove_comments.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1066 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.1/test_code_utilities/test_variable_renaming.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-22 21:32:45.766497 salesforce-codetf-0.0.1/test_dataset/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      791 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.1/test_dataset/test_load_codexgluedataset.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-22 21:32:45.767190 salesforce-codetf-0.0.1/test_evaluation/
--rw-r--r--   0 nghi.bui   (503) staff       (20)      901 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.1/test_evaluation/test_evaluate_human_eval_codegen.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1378 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.1/test_evaluation/test_evaluate_human_eval_codet5.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-22 21:32:45.769128 salesforce-codetf-0.0.1/test_inference/
--rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.1/test_inference/__init__.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      482 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.1/test_inference/test_codebert_embedding.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      468 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.1/test_inference/test_codegen_nl2code.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1129 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.1/test_inference/test_codet5_multitask.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      452 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.1/test_inference/test_starcoder_nl2code.py
-drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-22 21:32:45.770384 salesforce-codetf-0.0.1/test_trainer/
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1347 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.1/test_trainer/test_causal_lm_trainer_codegen.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)     1373 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.1/test_trainer/test_codet5_trainer.py
--rw-r--r--   0 nghi.bui   (503) staff       (20)      714 2023-05-08 01:21:19.000000 salesforce-codetf-0.0.1/test_trainer/test_t5_trainer.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:01:45.737625 salesforce-codetf-0.0.2/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    19491 2023-05-23 19:01:45.737841 salesforce-codetf-0.0.2/PKG-INFO
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    16625 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.2/README.md
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:01:45.723482 salesforce-codetf-0.0.2/codetf/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      620 2023-03-20 20:11:15.000000 salesforce-codetf-0.0.2/codetf/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:01:45.724529 salesforce-codetf-0.0.2/codetf/code_utility/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.2/codetf/code_utility/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:01:45.725020 salesforce-codetf-0.0.2/codetf/code_utility/apex/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.2/codetf/code_utility/apex/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     5146 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.2/codetf/code_utility/apex/apex_code_utility.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     5116 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.2/codetf/code_utility/ast_parser.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      846 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.2/codetf/code_utility/base_utility.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:01:45.725506 salesforce-codetf-0.0.2/codetf/code_utility/java/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.2/codetf/code_utility/java/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2480 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.2/codetf/code_utility/java/java_code_utility.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      221 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.2/codetf/code_utility/language_specific_utility.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:01:45.725993 salesforce-codetf-0.0.2/codetf/code_utility/python/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-08 00:25:11.000000 salesforce-codetf-0.0.2/codetf/code_utility/python/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2450 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.2/codetf/code_utility/python/python_code_utility.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:01:45.726531 salesforce-codetf-0.0.2/codetf/common/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     5677 2023-05-22 22:50:41.000000 salesforce-codetf-0.0.2/codetf/common/registry.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    14084 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.2/codetf/common/utils.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:01:45.728615 salesforce-codetf-0.0.2/codetf/data_utility/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.2/codetf/data_utility/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1123 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.2/codetf/data_utility/apps_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1347 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.2/codetf/data_utility/base_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     4292 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.2/codetf/data_utility/codexglue_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1149 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.2/codetf/data_utility/human_eval_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1114 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.2/codetf/data_utility/mpp_dataset.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1851 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.2/codetf/data_utility/util.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:01:45.729166 salesforce-codetf-0.0.2/codetf/models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3204 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.2/codetf/models/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2262 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.2/codetf/models/base_model.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:01:45.729448 salesforce-codetf-0.0.2/codetf/models/bert_models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2773 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.2/codetf/models/bert_models/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:01:45.729752 salesforce-codetf-0.0.2/codetf/models/causal_lm_models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3062 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.2/codetf/models/causal_lm_models/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:01:45.730034 salesforce-codetf-0.0.2/codetf/models/codet5_models/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     3096 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.2/codetf/models/codet5_models/__init__.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:01:45.730801 salesforce-codetf-0.0.2/codetf/performance/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.2/codetf/performance/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2674 2023-05-22 01:18:29.000000 salesforce-codetf-0.0.2/codetf/performance/evaluation_metric.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     4443 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.2/codetf/performance/model_evaluator.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:01:45.731630 salesforce-codetf-0.0.2/codetf/trainer/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     6263 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.2/codetf/trainer/base_trainer.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1303 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.2/codetf/trainer/causal_lm_trainer.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2048 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.2/codetf/trainer/codet5_trainer.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:01:45.733339 salesforce-codetf-0.0.2/salesforce_codetf.egg-info/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)    19491 2023-05-23 19:01:45.000000 salesforce-codetf-0.0.2/salesforce_codetf.egg-info/PKG-INFO
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     2043 2023-05-23 19:01:45.000000 salesforce-codetf-0.0.2/salesforce_codetf.egg-info/SOURCES.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        1 2023-05-23 19:01:45.000000 salesforce-codetf-0.0.2/salesforce_codetf.egg-info/dependency_links.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        1 2023-05-22 21:32:45.000000 salesforce-codetf-0.0.2/salesforce_codetf.egg-info/not-zip-safe
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      350 2023-05-23 19:01:45.000000 salesforce-codetf-0.0.2/salesforce_codetf.egg-info/requires.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      101 2023-05-23 19:01:45.000000 salesforce-codetf-0.0.2/salesforce_codetf.egg-info/top_level.txt
+-rw-r--r--   0 nghi.bui   (503) staff       (20)       79 2023-05-23 19:01:45.738289 salesforce-codetf-0.0.2/setup.cfg
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1030 2023-05-23 19:01:40.000000 salesforce-codetf-0.0.2/setup.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:01:45.734629 salesforce-codetf-0.0.2/test_code_utilities/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.2/test_code_utilities/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1063 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.2/test_code_utilities/test_extract_code_attributre.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      528 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.2/test_code_utilities/test_parse_code.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1369 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.2/test_code_utilities/test_remove_comments.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1066 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.2/test_code_utilities/test_variable_renaming.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:01:45.734889 salesforce-codetf-0.0.2/test_dataset/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      791 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.2/test_dataset/test_load_codexgluedataset.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:01:45.735411 salesforce-codetf-0.0.2/test_evaluation/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      901 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.2/test_evaluation/test_evaluate_human_eval_codegen.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1378 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.2/test_evaluation/test_evaluate_human_eval_codet5.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:01:45.736641 salesforce-codetf-0.0.2/test_inference/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)        0 2022-11-08 10:16:02.000000 salesforce-codetf-0.0.2/test_inference/__init__.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      482 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.2/test_inference/test_codebert_embedding.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      468 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.2/test_inference/test_codegen_nl2code.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1129 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.2/test_inference/test_codet5_multitask.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      452 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.2/test_inference/test_starcoder_nl2code.py
+drwxr-xr-x   0 nghi.bui   (503) staff       (20)        0 2023-05-23 19:01:45.737407 salesforce-codetf-0.0.2/test_trainer/
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1347 2023-05-22 20:33:30.000000 salesforce-codetf-0.0.2/test_trainer/test_causal_lm_trainer_codegen.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)     1373 2023-05-22 05:27:28.000000 salesforce-codetf-0.0.2/test_trainer/test_codet5_trainer.py
+-rw-r--r--   0 nghi.bui   (503) staff       (20)      714 2023-05-08 01:21:19.000000 salesforce-codetf-0.0.2/test_trainer/test_t5_trainer.py
```

### Comparing `salesforce-codetf-0.0.1/PKG-INFO` & `salesforce-codetf-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesforce-codetf
-Version: 0.0.1
+Version: 0.0.2
 Summary: CodeTF: A Transformer-based Library for Code Intelligence
 Home-page: https://github.com/Salesforce/CodeTF
 Author: Nghi D. Q. Bui
 License: 3-Clause BSD
 Description: 
             
         <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: salesforce-codetf Version: 0.0.1 Summary: CodeTF: A
+Metadata-Version: 2.1 Name: salesforce-codetf Version: 0.0.2 Summary: CodeTF: A
 Transformer-based Library for Code Intelligence Home-page: https://github.com/
 Salesforce/CodeTF Author: Nghi D. Q. Bui License: 3-Clause BSD Description:
 
                               [assets/logo.png]
  [license] [license] # CodeTF - A Comprehensive Transformer-based Library for
                          Code LLM & Code Intelligence
 ## Table of Contents - [Introduction](#introduction) - [Installation]
```

### Comparing `salesforce-codetf-0.0.1/README.md` & `salesforce-codetf-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/__init__.py` & `salesforce-codetf-0.0.2/codetf/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/code_utility/apex/apex_code_utility.py` & `salesforce-codetf-0.0.2/codetf/code_utility/apex/apex_code_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/code_utility/ast_parser.py` & `salesforce-codetf-0.0.2/codetf/code_utility/ast_parser.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/code_utility/base_utility.py` & `salesforce-codetf-0.0.2/codetf/code_utility/base_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/code_utility/java/java_code_utility.py` & `salesforce-codetf-0.0.2/codetf/code_utility/java/java_code_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/code_utility/python/python_code_utility.py` & `salesforce-codetf-0.0.2/codetf/code_utility/python/python_code_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/common/registry.py` & `salesforce-codetf-0.0.2/codetf/common/registry.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,33 +26,14 @@
                 )
             cls.mapping["model_name_mapping"][name] = model_cls
             return model_cls
 
         return wrap
 
     @classmethod
-    def register_processor(cls, name):
-        def wrap(processor_cls):
-            from lavis.processors import BaseProcessor
-
-            assert issubclass(
-                processor_cls, BaseProcessor
-            ), "All processors must inherit BaseProcessor class"
-            if name in cls.mapping["processor_name_mapping"]:
-                raise KeyError(
-                    "Name '{}' already registered for {}.".format(
-                        name, cls.mapping["processor_name_mapping"][name]
-                    )
-                )
-            cls.mapping["processor_name_mapping"][name] = processor_cls
-            return processor_cls
-
-        return wrap
-
-    @classmethod
     def register_lr_scheduler(cls, name):
         def wrap(lr_sched_cls):
             if name in cls.mapping["lr_scheduler_name_mapping"]:
                 raise KeyError(
                     "Name '{}' already registered for {}.".format(
                         name, cls.mapping["lr_scheduler_name_mapping"][name]
                     )
```

### Comparing `salesforce-codetf-0.0.1/codetf/common/utils.py` & `salesforce-codetf-0.0.2/codetf/common/utils.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/data_utility/apps_dataset.py` & `salesforce-codetf-0.0.2/codetf/data_utility/apps_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/data_utility/base_dataset.py` & `salesforce-codetf-0.0.2/codetf/data_utility/base_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/data_utility/codexglue_dataset.py` & `salesforce-codetf-0.0.2/codetf/data_utility/codexglue_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/data_utility/human_eval_dataset.py` & `salesforce-codetf-0.0.2/codetf/data_utility/human_eval_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/data_utility/mpp_dataset.py` & `salesforce-codetf-0.0.2/codetf/data_utility/mpp_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/data_utility/util.py` & `salesforce-codetf-0.0.2/codetf/data_utility/util.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/models/__init__.py` & `salesforce-codetf-0.0.2/codetf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/models/base_model.py` & `salesforce-codetf-0.0.2/codetf/models/base_model.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/models/bert_models/__init__.py` & `salesforce-codetf-0.0.2/codetf/models/bert_models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/models/causal_lm_models/__init__.py` & `salesforce-codetf-0.0.2/codetf/models/causal_lm_models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/models/codet5_models/__init__.py` & `salesforce-codetf-0.0.2/codetf/models/codet5_models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/performance/evaluation_metric.py` & `salesforce-codetf-0.0.2/codetf/performance/evaluation_metric.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/performance/model_evaluator.py` & `salesforce-codetf-0.0.2/codetf/performance/model_evaluator.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/trainer/base_trainer.py` & `salesforce-codetf-0.0.2/codetf/trainer/base_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/trainer/causal_lm_trainer.py` & `salesforce-codetf-0.0.2/codetf/trainer/causal_lm_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/codetf/trainer/codet5_trainer.py` & `salesforce-codetf-0.0.2/codetf/trainer/codet5_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/salesforce_codetf.egg-info/PKG-INFO` & `salesforce-codetf-0.0.2/salesforce_codetf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesforce-codetf
-Version: 0.0.1
+Version: 0.0.2
 Summary: CodeTF: A Transformer-based Library for Code Intelligence
 Home-page: https://github.com/Salesforce/CodeTF
 Author: Nghi D. Q. Bui
 License: 3-Clause BSD
 Description: 
             
         <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: salesforce-codetf Version: 0.0.1 Summary: CodeTF: A
+Metadata-Version: 2.1 Name: salesforce-codetf Version: 0.0.2 Summary: CodeTF: A
 Transformer-based Library for Code Intelligence Home-page: https://github.com/
 Salesforce/CodeTF Author: Nghi D. Q. Bui License: 3-Clause BSD Description:
 
                               [assets/logo.png]
  [license] [license] # CodeTF - A Comprehensive Transformer-based Library for
                          Code LLM & Code Intelligence
 ## Table of Contents - [Introduction](#introduction) - [Installation]
```

### Comparing `salesforce-codetf-0.0.1/salesforce_codetf.egg-info/SOURCES.txt` & `salesforce-codetf-0.0.2/salesforce_codetf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/setup.py` & `salesforce-codetf-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     
 def fetch_requirements(filename):
     with open(filename) as f:
         return [ln.strip() for ln in f.read().split("\n")]
 
 setup(
   name = 'salesforce-codetf',
-  version = "0.0.1",
+  version = "0.0.2",
   py_modules = ['codetf'],
   description = 'CodeTF: A Transformer-based Library for Code Intelligence',
   author = 'Nghi D. Q. Bui',
   long_description=open("README.md", "r", encoding="utf-8").read(),
   long_description_content_type="text/markdown",
   keywords="AI4Code, Code Intelligence, Generative AI, Deep Learning, Library, PyTorch, HuggingFace",
   license="3-Clause BSD",
```

### Comparing `salesforce-codetf-0.0.1/test_code_utilities/test_extract_code_attributre.py` & `salesforce-codetf-0.0.2/test_code_utilities/test_extract_code_attributre.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/test_code_utilities/test_parse_code.py` & `salesforce-codetf-0.0.2/test_code_utilities/test_parse_code.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/test_code_utilities/test_remove_comments.py` & `salesforce-codetf-0.0.2/test_code_utilities/test_remove_comments.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/test_code_utilities/test_variable_renaming.py` & `salesforce-codetf-0.0.2/test_code_utilities/test_variable_renaming.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/test_dataset/test_load_codexgluedataset.py` & `salesforce-codetf-0.0.2/test_dataset/test_load_codexgluedataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/test_evaluation/test_evaluate_human_eval_codegen.py` & `salesforce-codetf-0.0.2/test_evaluation/test_evaluate_human_eval_codegen.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/test_evaluation/test_evaluate_human_eval_codet5.py` & `salesforce-codetf-0.0.2/test_evaluation/test_evaluate_human_eval_codet5.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/test_inference/test_codet5_multitask.py` & `salesforce-codetf-0.0.2/test_inference/test_codet5_multitask.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/test_trainer/test_causal_lm_trainer_codegen.py` & `salesforce-codetf-0.0.2/test_trainer/test_causal_lm_trainer_codegen.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/test_trainer/test_codet5_trainer.py` & `salesforce-codetf-0.0.2/test_trainer/test_codet5_trainer.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-0.0.1/test_trainer/test_t5_trainer.py` & `salesforce-codetf-0.0.2/test_trainer/test_t5_trainer.py`

 * *Files identical despite different names*

