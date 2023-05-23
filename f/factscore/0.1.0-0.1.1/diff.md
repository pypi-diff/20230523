# Comparing `tmp/factscore-0.1.0.tar.gz` & `tmp/factscore-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factscore-0.1.0.tar", max compression
+gzip compressed data, was "factscore-0.1.1.tar", max compression
```

## Comparing `factscore-0.1.0.tar` & `factscore-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3001 2023-05-23 14:50:25.973238 factscore-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-23 14:51:37.783672 factscore-0.1.0/factscore/__init__.py
--rw-r--r--   0        0        0    16718 2023-05-23 14:51:37.783672 factscore-0.1.0/factscore/atomic_facts.py
--rw-r--r--   0        0        0     2967 2023-05-23 14:51:37.783672 factscore-0.1.0/factscore/clm.py
--rw-r--r--   0        0        0     2069 2023-05-23 14:51:37.783672 factscore-0.1.0/factscore/download_data.py
--rw-r--r--   0        0        0    10302 2023-05-23 14:51:37.783672 factscore-0.1.0/factscore/factscorer.py
--rw-r--r--   0        0        0     1762 2023-05-23 14:51:37.783672 factscore-0.1.0/factscore/lm.py
--rw-r--r--   0        0        0     7133 2023-05-23 14:51:37.783672 factscore-0.1.0/factscore/npm.py
--rw-r--r--   0        0        0     3953 2023-05-23 14:51:37.783672 factscore-0.1.0/factscore/openai_lm.py
--rw-r--r--   0        0        0     7536 2023-05-23 14:51:37.783672 factscore-0.1.0/factscore/retrieval.py
--rw-r--r--   0        0        0     4774 2023-05-23 14:51:37.783672 factscore-0.1.0/factscore/utils.py
--rw-r--r--   0        0        0      790 2023-05-23 15:04:26.086923 factscore-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4125 1970-01-01 00:00:00.000000 factscore-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3010 2023-05-23 15:12:19.496601 factscore-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 14:51:37.783672 factscore-0.1.1/factscore/__init__.py
+-rw-r--r--   0        0        0    16718 2023-05-23 14:51:37.783672 factscore-0.1.1/factscore/atomic_facts.py
+-rw-r--r--   0        0        0     2967 2023-05-23 14:51:37.783672 factscore-0.1.1/factscore/clm.py
+-rw-r--r--   0        0        0     2069 2023-05-23 14:51:37.783672 factscore-0.1.1/factscore/download_data.py
+-rw-r--r--   0        0        0    10160 2023-05-23 15:44:47.262172 factscore-0.1.1/factscore/factscorer.py
+-rw-r--r--   0        0        0     1762 2023-05-23 14:51:37.783672 factscore-0.1.1/factscore/lm.py
+-rw-r--r--   0        0        0     7133 2023-05-23 14:51:37.783672 factscore-0.1.1/factscore/npm.py
+-rw-r--r--   0        0        0     3953 2023-05-23 14:51:37.783672 factscore-0.1.1/factscore/openai_lm.py
+-rw-r--r--   0        0        0     7536 2023-05-23 14:51:37.783672 factscore-0.1.1/factscore/retrieval.py
+-rw-r--r--   0        0        0     4774 2023-05-23 14:51:37.783672 factscore-0.1.1/factscore/utils.py
+-rw-r--r--   0        0        0      798 2023-05-23 15:45:04.165804 factscore-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4094 1970-01-01 00:00:00.000000 factscore-0.1.1/PKG-INFO
```

### Comparing `factscore-0.1.0/README.md` & `factscore-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,29 +9,30 @@
 ## Install
 <!-- ```
 conda create -n fs-env python=3.9
 conda activate fs-env
 pip install -r requirements.txt
 ``` -->
 
+Make a new Python 3.7+ environment using `virtualenv` or `conda`.
+
 ```bash
-python3.7 -m virtualenv fs-venv
 pip install factscore
-python -m spacy download en_core_web_lg
+python -m spacy download en_core_web_sm
 ```
 
 ## Download the data
 
 ```bash
 python -m factscore.download_data
 ```
 
 Or, download it manually from this [Google Drive link](https://drive.google.com/drive/folders/1bLHGu_imkZVtX6O0mpZ-G0-4ofTLM1ZA?usp=sharing). Make a cache directory `.cache/factscore`, and place unzipped `demos` and `enwiki-20230401.db` in that directory.
 
-## Running the script with oracle atomic facts
+## Running FactScore
 
 ```bash
 python -m factscore.factscorer --data_path {data_path} --model_name {estimator_name} --cache_dir {cache_dir} --openai_key {openai_key}
 ```
 
 - `data_path` can be something like `data/src-light/bio_ChatGPT_v0.2.jsonl` which is in a format we have been using so far. TODO for simplying the format and allowing it to take any topics/generations.
 - `model_name`: `retrieval+llama`, `retrieval+llama+npm`, `retrieval+ChatGPT`, `retrieval+ChatGPT+npm`
```

### Comparing `factscore-0.1.0/factscore/atomic_facts.py` & `factscore-0.1.1/factscore/atomic_facts.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.0/factscore/clm.py` & `factscore-0.1.1/factscore/clm.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.0/factscore/download_data.py` & `factscore-0.1.1/factscore/download_data.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.0/factscore/factscorer.py` & `factscore-0.1.1/factscore/factscorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import argparse
 import string
 import json
 import numpy as np
 import os
-import subprocess
 
 from tqdm import tqdm
 from factscore.atomic_facts import AtomicFactGenerator
 from factscore.clm import CLM
 from factscore.npm import NPM
 from factscore.openai_lm import OpenAIModel
 from factscore.retrieval import DocDB, Retrieval
@@ -53,36 +52,36 @@
 
     def register_knowledge_source(self, name="enwiki-20230401", db_path=None, data_path=None):
         assert name not in self.retrieval, f"{name} already registered"
         if db_path is None:
             db_path = os.path.join(self.cache_dir, f"{name}.db")
         if data_path is None:
             data_path = os.path.join(self.cache_dir, f"{name}.jsonl")
-        
+
         cache_path = os.path.join(self.cache_dir, f"retrieval-{name}.json")
         embed_cache_path = os.path.join(self.cache_dir, f"retrieval-{name}.pkl")
-        
+
         self.db[name] = DocDB(db_path=db_path, data_path=data_path)
         self.retrieval[name] = Retrieval(self.db[name], cache_path, embed_cache_path, batch_size=self.batch_size)
         if "npm" in self.model_name:
             cache_path = os.path.join(self.cache_dir, f"bm25-{name}.json")
             embed_cache_path = os.path.join(self.cache_dir, f"bm25-{name}.pkl")
             self.npm[name] = NPM(Retrieval(self.db[name], cache_path, embed_cache_path, "bm25"),
                                  "npm-single",
                                  cache_file=os.path.join(self.cache_dir, f"npm-{name}.pkl"))
 
     def get_score(self,
                   topics,
                   generations,
+                  atomic_facts,
                   knowledge_source=None,
-                  atomic_facts=None,
                   return_atomic_facts=False,
                   return_individual_decisions=False,
                   verbose=False):
-        
+
         if knowledge_source is None:
             # use the default one (enwiki-20230401)
             knowledge_source = "enwiki-20230401"
             self.register_knowledge_source(knowledge_source)
         else:
             assert knowledge_source in self.retrieval, \
                 f"{knowledge_source} is not registered yet. Please use `register_knowledge_source()` function to register it with a database"
@@ -90,18 +89,15 @@
         if type(topics)==len(generations)==str:
             topics = [topics]
             generations = [generations]
         else:
             assert type(topics)==type(generations)==list, "`topics` and `generations` should be lists."
             assert len(topics)==len(generations), "`topics` and `generations` should have the same length"
 
-        if atomic_facts is not None:
-            assert len(topics)==len(atomic_facts), "`topics` and `atomic_facts` should have the same length"
-        else:
-            raise NotImplementedError()
+        assert len(topics)==len(atomic_facts), "`topics` and `atomic_facts` should have the same length"
 
         if verbose:
             topics = tqdm(topics)
 
         scores = []
         decisions = []
         for topic, generation, facts in zip(topics, generations, atomic_facts):
```

### Comparing `factscore-0.1.0/factscore/lm.py` & `factscore-0.1.1/factscore/lm.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.0/factscore/npm.py` & `factscore-0.1.1/factscore/npm.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.0/factscore/openai_lm.py` & `factscore-0.1.1/factscore/openai_lm.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.0/factscore/retrieval.py` & `factscore-0.1.1/factscore/retrieval.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.0/factscore/utils.py` & `factscore-0.1.1/factscore/utils.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.0/pyproject.toml` & `factscore-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "factscore"
-version = "0.1.0"
+version = "0.1.1"
 description = "FactScore is an automatic evaluation metric for factual precision in long-form text generation. It uses large language models and retrieval to break down generations into atomic facts and then measure the correctness with respect to a knowledge source (like Wikipedia)."
 authors = ["Sewon Min <sewon@cs.washington.edu>", "Kalpesh Krishna <kalpesh@cs.umass.edu>", "Xinxi Lyu <alrope@cs.washington.edu>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.7.1"
 torch = "^1.13.0"
 sentence-transformers = "^2.2.2"
 transformers = "^4.29.2"
-pysqlite3 = "^0.5.0"
 openai = "^0.27.7"
 rank-bm25 = "^0.2.2"
 spacy = "^3.5.3"
+pysqlite-binary = "^0.5.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `factscore-0.1.0/PKG-INFO` & `factscore-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: factscore
-Version: 0.1.0
+Version: 0.1.1
 Summary: FactScore is an automatic evaluation metric for factual precision in long-form text generation. It uses large language models and retrieval to break down generations into atomic facts and then measure the correctness with respect to a knowledge source (like Wikipedia).
 License: MIT
 Author: Sewon Min
 Author-email: sewon@cs.washington.edu
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.7,<0.28.0)
-Requires-Dist: pysqlite3 (>=0.5.0,<0.6.0)
+Requires-Dist: pysqlite-binary (>=0.5.0,<0.6.0)
 Requires-Dist: rank-bm25 (>=0.2.2,<0.3.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: spacy (>=3.5.3,<4.0.0)
 Requires-Dist: torch (>=1.13.0,<2.0.0)
 Requires-Dist: transformers (>=4.29.2,<5.0.0)
 Description-Content-Type: text/markdown
 
@@ -33,29 +32,30 @@
 ## Install
 <!-- ```
 conda create -n fs-env python=3.9
 conda activate fs-env
 pip install -r requirements.txt
 ``` -->
 
+Make a new Python 3.7+ environment using `virtualenv` or `conda`.
+
 ```bash
-python3.7 -m virtualenv fs-venv
 pip install factscore
-python -m spacy download en_core_web_lg
+python -m spacy download en_core_web_sm
 ```
 
 ## Download the data
 
 ```bash
 python -m factscore.download_data
 ```
 
 Or, download it manually from this [Google Drive link](https://drive.google.com/drive/folders/1bLHGu_imkZVtX6O0mpZ-G0-4ofTLM1ZA?usp=sharing). Make a cache directory `.cache/factscore`, and place unzipped `demos` and `enwiki-20230401.db` in that directory.
 
-## Running the script with oracle atomic facts
+## Running FactScore
 
 ```bash
 python -m factscore.factscorer --data_path {data_path} --model_name {estimator_name} --cache_dir {cache_dir} --openai_key {openai_key}
 ```
 
 - `data_path` can be something like `data/src-light/bio_ChatGPT_v0.2.jsonl` which is in a format we have been using so far. TODO for simplying the format and allowing it to take any topics/generations.
 - `model_name`: `retrieval+llama`, `retrieval+llama+npm`, `retrieval+ChatGPT`, `retrieval+ChatGPT+npm`
```

