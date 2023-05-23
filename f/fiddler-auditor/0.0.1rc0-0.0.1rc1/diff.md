# Comparing `tmp/fiddler-auditor-0.0.1rc0.tar.gz` & `tmp/fiddler-auditor-0.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiddler-auditor-0.0.1rc0.tar", last modified: Mon May 22 06:58:27 2023, max compression
+gzip compressed data, was "fiddler-auditor-0.0.1rc1.tar", last modified: Mon May 22 08:17:37 2023, max compression
```

## Comparing `fiddler-auditor-0.0.1rc0.tar` & `fiddler-auditor-0.0.1rc1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:58:27.676056 fiddler-auditor-0.0.1rc0/
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-22 06:58:27.676056 fiddler-auditor-0.0.1rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:58:27.668055 fiddler-auditor-0.0.1rc0/auditor/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:58:27.664055 fiddler-auditor-0.0.1rc0/auditor/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:58:27.668055 fiddler-auditor-0.0.1rc0/auditor/assets/data/
--rw-r--r--   0 runner    (1001) docker     (123)    43309 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/assets/data/snips_dataset_dev.csv
--rw-r--r--   0 runner    (1001) docker     (123)    43115 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/assets/data/snips_dataset_test.csv
--rw-r--r--   0 runner    (1001) docker     (123)   798933 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/assets/data/snips_dataset_train.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:58:27.672056 fiddler-auditor-0.0.1rc0/auditor/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/evaluation/discriminative.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/evaluation/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/evaluation/expected_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)    10198 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/evaluation/generative.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:58:27.672056 fiddler-auditor-0.0.1rc0/auditor/generations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/generations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/generations/paraphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:58:27.672056 fiddler-auditor-0.0.1rc0/auditor/perturbations/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/perturbations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/perturbations/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/perturbations/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:58:27.672056 fiddler-auditor-0.0.1rc0/auditor/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/reporting/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:58:27.672056 fiddler-auditor-0.0.1rc0/auditor/reporting/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/reporting/templates/report_template.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:58:27.672056 fiddler-auditor-0.0.1rc0/auditor/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/auditor/utils/similarity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:58:27.676056 fiddler-auditor-0.0.1rc0/fiddler_auditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-22 06:58:27.000000 fiddler-auditor-0.0.1rc0/fiddler_auditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-22 06:58:27.000000 fiddler-auditor-0.0.1rc0/fiddler_auditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 06:58:27.000000 fiddler-auditor-0.0.1rc0/fiddler_auditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-22 06:58:27.000000 fiddler-auditor-0.0.1rc0/fiddler_auditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 06:58:27.000000 fiddler-auditor-0.0.1rc0/fiddler_auditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 06:58:27.676056 fiddler-auditor-0.0.1rc0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:58:27.676056 fiddler-auditor-0.0.1rc0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/tests/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/tests/test_llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-22 06:54:49.000000 fiddler-auditor-0.0.1rc0/tests/test_perturbations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:37.969350 fiddler-auditor-0.0.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-22 08:17:37.969350 fiddler-auditor-0.0.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:37.961350 fiddler-auditor-0.0.1rc1/auditor/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:37.961350 fiddler-auditor-0.0.1rc1/auditor/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:37.961350 fiddler-auditor-0.0.1rc1/auditor/assets/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    43309 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/assets/data/snips_dataset_dev.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    43115 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/assets/data/snips_dataset_test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   798933 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/assets/data/snips_dataset_train.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:37.965350 fiddler-auditor-0.0.1rc1/auditor/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/evaluation/discriminative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/evaluation/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/evaluation/expected_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/evaluation/generative.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:37.965350 fiddler-auditor-0.0.1rc1/auditor/generations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/generations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/generations/paraphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:37.965350 fiddler-auditor-0.0.1rc1/auditor/perturbations/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/perturbations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/perturbations/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/perturbations/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:37.965350 fiddler-auditor-0.0.1rc1/auditor/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/reporting/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:37.965350 fiddler-auditor-0.0.1rc1/auditor/reporting/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/reporting/templates/report_template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:37.965350 fiddler-auditor-0.0.1rc1/auditor/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/auditor/utils/similarity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:37.965350 fiddler-auditor-0.0.1rc1/fiddler_auditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-22 08:17:37.000000 fiddler-auditor-0.0.1rc1/fiddler_auditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-22 08:17:37.000000 fiddler-auditor-0.0.1rc1/fiddler_auditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:17:37.000000 fiddler-auditor-0.0.1rc1/fiddler_auditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-22 08:17:37.000000 fiddler-auditor-0.0.1rc1/fiddler_auditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 08:17:37.000000 fiddler-auditor-0.0.1rc1/fiddler_auditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 08:17:37.969350 fiddler-auditor-0.0.1rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:37.965350 fiddler-auditor-0.0.1rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/tests/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/tests/test_llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-22 08:13:48.000000 fiddler-auditor-0.0.1rc1/tests/test_perturbations.py
```

### Comparing `fiddler-auditor-0.0.1rc0/LICENSE` & `fiddler-auditor-0.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc0/PKG-INFO` & `fiddler-auditor-0.0.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: fiddler-auditor
-Version: 0.0.1rc0
+Version: 0.0.1rc1
 Summary: Auditing large language models made easy.
 Author-email: Fiddler Labs <support@fiddler.ai>
 License: Elastic License 2.0 (ELv2)
 Project-URL: repository, https://github.com/fiddler-labs/fiddler-auditor
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: <4.0,>=3.7.12
+Requires-Python: <4.0,>=3.8.1
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # ![alt text](https://global-uploads.webflow.com/5e067beb4c88a64e31622d4b/6030124ca93f9ce13a57aa79_favicon.png "Fiddler Auditor") Fiddler Auditor 
 Auditing Large Language Models made easy! 🍰
```

### Comparing `fiddler-auditor-0.0.1rc0/README.md` & `fiddler-auditor-0.0.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc0/auditor/assets/data/snips_dataset_dev.csv` & `fiddler-auditor-0.0.1rc1/auditor/assets/data/snips_dataset_dev.csv`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc0/auditor/assets/data/snips_dataset_test.csv` & `fiddler-auditor-0.0.1rc1/auditor/assets/data/snips_dataset_test.csv`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc0/auditor/assets/data/snips_dataset_train.csv` & `fiddler-auditor-0.0.1rc1/auditor/assets/data/snips_dataset_train.csv`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc0/auditor/evaluation/discriminative.py` & `fiddler-auditor-0.0.1rc1/auditor/evaluation/discriminative.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc0/auditor/evaluation/expected_behavior.py` & `fiddler-auditor-0.0.1rc1/auditor/evaluation/expected_behavior.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc0/auditor/evaluation/generative.py` & `fiddler-auditor-0.0.1rc1/auditor/evaluation/generative.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional, Literal
+from typing import List, Optional, Literal, Dict
 
 from langchain.llms.base import BaseLLM
 
 from auditor.utils.data import (
     LLMEvalResult,
     LLMEvalType,
 )
@@ -180,15 +180,15 @@
         # TODO: Add perturbation types
         perturbed_dataset = perturber.paraphrase(temperature=temperature)
         if return_original:
             return perturbed_dataset.data[0]
         else:
             return perturbed_dataset.data[0][1:]
 
-    def _get_generation_details(self) -> dict[str, str]:
+    def _get_generation_details(self) -> Dict[str, str]:
         """Returns generation related details"""
         details = {}
         if hasattr(self.llm, '_llm_type'):
             details['Provider'] = self.llm._llm_type
         if hasattr(self.llm, 'temperature'):
             details['Temperature'] = self.llm.temperature
         if hasattr(self.llm, 'model_name'):
```

### Comparing `fiddler-auditor-0.0.1rc0/auditor/generations/paraphrase.py` & `fiddler-auditor-0.0.1rc1/auditor/generations/paraphrase.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc0/auditor/perturbations/text.py` & `fiddler-auditor-0.0.1rc1/auditor/perturbations/text.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc0/auditor/reporting/generate.py` & `fiddler-auditor-0.0.1rc1/auditor/reporting/generate.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc0/auditor/reporting/templates/report_template.html` & `fiddler-auditor-0.0.1rc1/auditor/reporting/templates/report_template.html`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc0/auditor/utils/data.py` & `fiddler-auditor-0.0.1rc1/auditor/utils/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         perturbed_prompts: List[str],
         perturbed_generations: List[str],
         result: List[int],
         metric: List[Dict[str, Any]],
         expected_behavior_desc: str,
         evaluation_type: Literal[LLMEvalType.robustness, LLMEvalType.correctness],  # noqa: E501
         reference_generation: Optional[str] = None,
-        generation_kwargs: Optional[dict[str, str]] = None,
+        generation_kwargs: Optional[Dict[str, str]] = None,
     ) -> None:
         self.original_prompt = original_prompt
         self.pre_context = pre_context
         self.post_context = post_context
         self.perturbed_prompts = perturbed_prompts
         self.perturbed_generations = perturbed_generations
         self.reference_generation = reference_generation
@@ -221,15 +221,15 @@
         post_context: str,
         reference_generation: str,
         evaluation_type: str,
         perturbed_prompts: List[str],
         perturbed_generations: List[str],
         test_result: List[int],
         metric: List[Dict[str, Any]],
-        generation_kwargs: Optional[dict[str, str]] = None,
+        generation_kwargs: Optional[Dict[str, str]] = None,
         expected_behavior_desc: Optional[str] = None,
     ) -> str:
         # report type
         report_type = f'{evaluation_type} report'
         # metric name
         metric_name = list(metric[0].keys())[0]
         metric_values = [i[metric_name] for i in metric]
```

### Comparing `fiddler-auditor-0.0.1rc0/auditor/utils/dataset.py` & `fiddler-auditor-0.0.1rc1/auditor/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc0/auditor/utils/logging.py` & `fiddler-auditor-0.0.1rc1/auditor/utils/logging.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc0/auditor/utils/similarity.py` & `fiddler-auditor-0.0.1rc1/auditor/utils/similarity.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc0/fiddler_auditor.egg-info/PKG-INFO` & `fiddler-auditor-0.0.1rc1/fiddler_auditor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: fiddler-auditor
-Version: 0.0.1rc0
+Version: 0.0.1rc1
 Summary: Auditing large language models made easy.
 Author-email: Fiddler Labs <support@fiddler.ai>
 License: Elastic License 2.0 (ELv2)
 Project-URL: repository, https://github.com/fiddler-labs/fiddler-auditor
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: <4.0,>=3.7.12
+Requires-Python: <4.0,>=3.8.1
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # ![alt text](https://global-uploads.webflow.com/5e067beb4c88a64e31622d4b/6030124ca93f9ce13a57aa79_favicon.png "Fiddler Auditor") Fiddler Auditor 
 Auditing Large Language Models made easy! 🍰
```

### Comparing `fiddler-auditor-0.0.1rc0/fiddler_auditor.egg-info/SOURCES.txt` & `fiddler-auditor-0.0.1rc1/fiddler_auditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc0/pyproject.toml` & `fiddler-auditor-0.0.1rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fiddler-auditor"
-version = "0.0.1.rc0"
+version = "0.0.1.rc1"
 authors = [
   { name="Fiddler Labs", email="support@fiddler.ai" },
 ]
 description = "Auditing large language models made easy."
 readme = "README.md"
-requires-python = ">=3.7.12,<4.0"
+requires-python = ">=3.8.1,<4.0"
 
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
```

### Comparing `fiddler-auditor-0.0.1rc0/tests/test_dataset.py` & `fiddler-auditor-0.0.1rc1/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc0/tests/test_evaluation.py` & `fiddler-auditor-0.0.1rc1/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc0/tests/test_llm.py` & `fiddler-auditor-0.0.1rc1/tests/test_llm.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc0/tests/test_perturbations.py` & `fiddler-auditor-0.0.1rc1/tests/test_perturbations.py`

 * *Files identical despite different names*

