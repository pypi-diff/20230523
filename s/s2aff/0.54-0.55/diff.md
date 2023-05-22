# Comparing `tmp/s2aff-0.54.tar.gz` & `tmp/s2aff-0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.54.tar", last modified: Mon May 22 13:37:54 2023, max compression
+gzip compressed data, was "s2aff-0.55.tar", last modified: Mon May 22 19:56:16 2023, max compression
```

## Comparing `s2aff-0.54.tar` & `s2aff-0.55.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-22 13:37:54.811339 s2aff-0.54/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.54/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-22 13:37:54.811207 s2aff-0.54/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.54/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-22 13:37:54.803893 s2aff-0.54/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.54/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.54/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.54/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-22 13:37:54.804164 s2aff-0.54/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.54/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-22 13:37:54.807690 s2aff-0.54/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11348 2023-05-22 13:29:36.000000 s2aff-0.54/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-16 14:48:02.000000 s2aff-0.54/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.54/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.54/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.54/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.54/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13721 2023-05-19 17:29:02.000000 s2aff-0.54/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    36032 2023-05-22 13:35:44.000000 s2aff-0.54/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.54/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-22 13:37:54.808967 s2aff-0.54/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.54/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.54/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.54/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-22 13:37:54.808511 s2aff-0.54/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-22 13:37:54.000000 s2aff-0.54/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-22 13:37:54.000000 s2aff-0.54/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-22 13:37:54.000000 s2aff-0.54/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-22 13:37:54.000000 s2aff-0.54/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-22 13:37:54.000000 s2aff-0.54/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-22 13:37:54.810939 s2aff-0.54/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.54/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.54/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.54/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.54/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.54/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.54/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.54/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-22 13:37:54.811385 s2aff-0.54/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-22 13:35:44.000000 s2aff-0.54/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-22 19:56:16.803909 s2aff-0.55/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.55/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-22 19:56:16.803775 s2aff-0.55/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.55/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-22 19:56:16.796527 s2aff-0.55/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.55/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.55/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.55/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-22 19:56:16.796816 s2aff-0.55/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.55/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-22 19:56:16.800369 s2aff-0.55/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11348 2023-05-22 13:29:36.000000 s2aff-0.55/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-16 14:48:02.000000 s2aff-0.55/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.55/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.55/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.55/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.55/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13725 2023-05-22 17:08:00.000000 s2aff-0.55/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    36032 2023-05-22 13:35:44.000000 s2aff-0.55/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.55/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-22 19:56:16.801564 s2aff-0.55/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.55/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.55/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.55/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-22 19:56:16.801137 s2aff-0.55/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-22 19:56:16.000000 s2aff-0.55/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-22 19:56:16.000000 s2aff-0.55/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-22 19:56:16.000000 s2aff-0.55/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-22 19:56:16.000000 s2aff-0.55/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-22 19:56:16.000000 s2aff-0.55/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-22 19:56:16.803502 s2aff-0.55/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.55/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.55/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.55/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.55/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.55/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.55/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.55/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-22 19:56:16.803960 s2aff-0.55/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-22 17:08:11.000000 s2aff-0.55/setup.py
```

### Comparing `s2aff-0.54/LICENSE` & `s2aff-0.55/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.54/README.md` & `s2aff-0.55/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.54/data/combine_gold.py` & `s2aff-0.55/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.54/data/download_latest_ror.py` & `s2aff-0.55/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.54/s2aff/__init__.py` & `s2aff-0.55/s2aff/__init__.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.54/s2aff/consts.py` & `s2aff-0.55/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.54/s2aff/data.py` & `s2aff-0.55/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.54/s2aff/features.py` & `s2aff-0.55/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.54/s2aff/file_cache.py` & `s2aff-0.55/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.54/s2aff/lightgbm_helpers.py` & `s2aff-0.55/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.54/s2aff/model.py` & `s2aff-0.55/s2aff/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     """Named Entity Recognition for affiliation strings.
     Uses SimpleTransformers under the hood.
     """
 
     def __init__(self, model_path=PATHS["ner_model"], model_type="roberta", use_cuda=True):
         self.model_path = model_path
         self.model_type = model_type
-        self.use_cuda = True
+        self.use_cuda = use_cuda
         if self.model_path is not None:
             self.load_model(self.model_path, self.model_type)
 
     def load_model(self, model_path=PATHS["ner_model"], model_type="roberta"):
         """Load a model from disk.
 
         model_path (str, optional): Location of the saved NER model.
```

### Comparing `s2aff-0.54/s2aff/ror.py` & `s2aff-0.55/s2aff/ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.54/s2aff/text.py` & `s2aff-0.55/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.54/s2aff/timo/integration_test.py` & `s2aff-0.55/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.54/s2aff/timo/interface.py` & `s2aff-0.55/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.54/s2aff.egg-info/SOURCES.txt` & `s2aff-0.55/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.54/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.55/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.54/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.55/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.54/scripts/generate_lightgbm_training_data.py` & `s2aff-0.55/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.54/scripts/train_lightgbm_reranker.py` & `s2aff-0.55/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.54/scripts/train_ner_model.py` & `s2aff-0.55/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.54/scripts/update_openalex_works_counts.py` & `s2aff-0.55/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.54/setup.py` & `s2aff-0.55/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.54",
+    version="0.55",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

