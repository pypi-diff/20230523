# Comparing `tmp/ragas-0.0.1a7.tar.gz` & `tmp/ragas-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragas-0.0.1a7.tar", last modified: Sun May 14 22:03:46 2023, max compression
+gzip compressed data, was "ragas-0.0.2.tar", last modified: Tue May 23 06:41:03 2023, max compression
```

## Comparing `ragas-0.0.1a7.tar` & `ragas-0.0.2.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.796328 ragas-0.0.1a7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.788328 ragas-0.0.1a7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.788328 ragas-0.0.1a7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-14 22:03:31.000000 ragas-0.0.1a7/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-14 22:03:31.000000 ragas-0.0.1a7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-14 22:03:31.000000 ragas-0.0.1a7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 22:03:31.000000 ragas-0.0.1a7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-14 22:03:31.000000 ragas-0.0.1a7/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-14 22:03:46.792328 ragas-0.0.1a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-14 22:03:31.000000 ragas-0.0.1a7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-14 22:03:31.000000 ragas-0.0.1a7/citations.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.788328 ragas-0.0.1a7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.788328 ragas-0.0.1a7/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    33956 2023-05-14 22:03:31.000000 ragas-0.0.1a7/docs/assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.788328 ragas-0.0.1a7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-14 22:03:31.000000 ragas-0.0.1a7/examples/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (123)    25111 2023-05-14 22:03:31.000000 ragas-0.0.1a7/examples/quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-14 22:03:31.000000 ragas-0.0.1a7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.792328 ragas-0.0.1a7/ragas/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-14 22:03:31.000000 ragas-0.0.1a7/ragas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-14 22:03:46.000000 ragas-0.0.1a7/ragas/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-14 22:03:31.000000 ragas-0.0.1a7/ragas/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.792328 ragas-0.0.1a7/ragas/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-14 22:03:31.000000 ragas-0.0.1a7/ragas/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-14 22:03:31.000000 ragas-0.0.1a7/ragas/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-05-14 22:03:31.000000 ragas-0.0.1a7/ragas/metrics/factual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-14 22:03:31.000000 ragas-0.0.1a7/ragas/metrics/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-14 22:03:31.000000 ragas-0.0.1a7/ragas/metrics/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-14 22:03:31.000000 ragas-0.0.1a7/ragas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.792328 ragas-0.0.1a7/ragas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-14 22:03:46.000000 ragas-0.0.1a7/ragas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-14 22:03:46.000000 ragas-0.0.1a7/ragas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 22:03:46.000000 ragas-0.0.1a7/ragas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-14 22:03:46.000000 ragas-0.0.1a7/ragas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 22:03:46.000000 ragas-0.0.1a7/ragas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.792328 ragas-0.0.1a7/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-14 22:03:31.000000 ragas-0.0.1a7/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-14 22:03:31.000000 ragas-0.0.1a7/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 22:03:46.796328 ragas-0.0.1a7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.788328 ragas-0.0.1a7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.792328 ragas-0.0.1a7/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-14 22:03:31.000000 ragas-0.0.1a7/tests/benchmarks/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-14 22:03:31.000000 ragas-0.0.1a7/tests/benchmarks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.792328 ragas-0.0.1a7/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-14 22:03:31.000000 ragas-0.0.1a7/tests/unit/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.800064 ragas-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.792065 ragas-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.792065 ragas-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-23 06:40:47.000000 ragas-0.0.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-23 06:40:47.000000 ragas-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-23 06:40:47.000000 ragas-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 06:40:47.000000 ragas-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-23 06:40:47.000000 ragas-0.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-05-23 06:41:03.796064 ragas-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-23 06:40:47.000000 ragas-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.792065 ragas-0.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.792065 ragas-0.0.2/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    33956 2023-05-23 06:40:47.000000 ragas-0.0.2/docs/assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.796064 ragas-0.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-23 06:40:47.000000 ragas-0.0.2/examples/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-05-23 06:40:47.000000 ragas-0.0.2/examples/quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-23 06:40:47.000000 ragas-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.796064 ragas-0.0.2/ragas/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-23 06:40:47.000000 ragas-0.0.2/ragas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 06:41:03.000000 ragas-0.0.2/ragas/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-23 06:40:47.000000 ragas-0.0.2/ragas/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.796064 ragas-0.0.2/ragas/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-23 06:40:47.000000 ragas-0.0.2/ragas/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-23 06:40:47.000000 ragas-0.0.2/ragas/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-05-23 06:40:47.000000 ragas-0.0.2/ragas/metrics/factual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-23 06:40:47.000000 ragas-0.0.2/ragas/metrics/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-23 06:40:47.000000 ragas-0.0.2/ragas/metrics/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-23 06:40:47.000000 ragas-0.0.2/ragas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.796064 ragas-0.0.2/ragas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-05-23 06:41:03.000000 ragas-0.0.2/ragas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-23 06:41:03.000000 ragas-0.0.2/ragas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:41:03.000000 ragas-0.0.2/ragas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-23 06:41:03.000000 ragas-0.0.2/ragas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 06:41:03.000000 ragas-0.0.2/ragas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-23 06:40:47.000000 ragas-0.0.2/references.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.796064 ragas-0.0.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-23 06:40:47.000000 ragas-0.0.2/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-23 06:40:47.000000 ragas-0.0.2/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 06:41:03.800064 ragas-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.792065 ragas-0.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.796064 ragas-0.0.2/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-23 06:40:47.000000 ragas-0.0.2/tests/benchmarks/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-23 06:40:47.000000 ragas-0.0.2/tests/benchmarks/benchmark_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-23 06:40:47.000000 ragas-0.0.2/tests/benchmarks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.796064 ragas-0.0.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 06:40:47.000000 ragas-0.0.2/tests/unit/test_simple.py
```

### Comparing `ragas-0.0.1a7/.github/workflows/ci.yaml` & `ragas-0.0.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a7/.github/workflows/python-publish.yml` & `ragas-0.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a7/.gitignore` & `ragas-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a7/LICENSE` & `ragas-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a7/Makefile` & `ragas-0.0.2/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	@echo "(ruff) Running fix only..."
 	@ruff check ragas examples tests --fix-only
 lint: ## Running lint checker: ruff
 	@echo "(ruff) Linting development project..."
 	@ruff check ragas examples tests
 type: ## Running type checker: pyright
 	@echo "(pyright) Typechecking codebase..."
-	@pyright -p ragas
+	@pyright ragas
 clean: ## Clean all generated files
 	@echo "Cleaning all generated files..."
 	@cd $(GIT_ROOT)/docs && make clean
 	@cd $(GIT_ROOT) || exit 1
 	@find . -type f -name '*.py[co]' -delete -o -type d -name __pycache__ -delete
 run-ci: format lint type ## Running all CI checks
 run-benchmarks: ## Run benchmarks
```

### Comparing `ragas-0.0.1a7/PKG-INFO` & `ragas-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,64 @@
 Metadata-Version: 2.1
 Name: ragas
-Version: 0.0.1a7
+Version: 0.0.2
 Description-Content-Type: text/plain
 License-File: LICENSE
 
 <h1 align="center">
   <img style="vertical-align:middle" height="200"
   src="./docs/assets/logo.png">
 </h1>
 <p align="center">
   <i>SOTA metrics for evaluating Retrieval Augmented Generation (RAG)</i>
 </p>
 
 <p align="center">
-    <a href="https://github.com/beir-cellar/beir/releases">
-        <img alt="GitHub release" src="https://img.shields.io/github/release/beir-cellar/beir.svg">
+    <a href="https://github.com/explodinggradients/ragas/releases">
+        <img alt="GitHub release" src="https://img.shields.io/github/release/explodinggradients/ragas.svg">
     </a>
     <a href="https://www.python.org/">
             <img alt="Build" src="https://img.shields.io/badge/Made%20with-Python-1f425f.svg?color=purple">
     </a>
-    <a href="https://github.com/beir-cellar/beir/blob/master/LICENSE">
-        <img alt="License" src="https://img.shields.io/github/license/beir-cellar/beir.svg?color=green">
+    <a href="https://github.com/explodinggradients/ragas/blob/master/LICENSE">
+        <img alt="License" src="https://img.shields.io/github/license/explodinggradients/ragas.svg?color=green">
     </a>
     <a href="https://colab.research.google.com/drive/1HfutiEhHMJLXiWGT8pcipxT5L2TpYEdt?usp=sharing">
         <img alt="Open In Colab" src="https://colab.research.google.com/assets/colab-badge.svg">
     </a>
-    <a href="https://github.com/beir-cellar/beir/">
+    <a href="https://github.com/explodinggradients/ragas/">
         <img alt="Downloads" src="https://badges.frapsoft.com/os/v1/open-source.svg?v=103">
     </a>
 </p>
 
 <h4 align="center">
     <p>
-        <a href="#beers-installation">Installation</a> |
-        <a href="#beers-quick-example">Quick Example</a> |
-        <a href="https://huggingface.co/BeIR">Hugging Face</a>
+        <a href="#shield-installation">Installation</a> |
+        <a href="#fire-quickstart">Quickstart</a> |
+        <a href="#luggage-metrics">Metrics</a> |
+        <a href="https://huggingface.co/explodinggradients">Hugging Face</a>
     <p>
 </h4>
 
 ragas is a framework that helps you evaluate your Retrieval Augmented Generation (RAG) pipelines. RAG denotes a class of LLM applications that use external data to augment the LLM’s context. There are existing tools and frameworks that help you build these pipelines but evaluating it and quantifying your pipeline performance can be hard.. This is were ragas (RAG Assessment) comes in
 
 ragas provides you with the tools based on the latest research for evaluating LLM generated text  to give you insights about your RAG pipeline. ragas can be integrated with your CI/CD to provide continuous check to ensure performance.
 
-## Installation 🛡
+## :shield: Installation
 
 ```bash
 pip install ragas
 ```
 if you want to install from source 
 ```bash
 git clone https://github.com/explodinggradients/ragas && cd ragas
 pip install -e .
 ```
 
-## Quickstart 🔥
+## :fire: Quickstart 
 
 This is a small example program you can run to see ragas in action!
 ```python
 from datasets import load_dataset
 from ragas.metrics import (
     Evaluation,
     rouge1,
@@ -77,34 +78,34 @@
 )
 
 # run the evaluation
 results = e.eval(ds["ground_truth"], ds["generated_text"])
 print(results)
 ```
 If you want a more in-depth explanation of core components, check out our quick-start notebook
-## 🧰 Metrics
+## :luggage: Metrics
 
-### ✏️ Character based 
+### :3rd_place_medal: Character based 
 
 - **Levenshtein distance** the number of single character edits (additional, insertion, deletion) required to change your generated text to ground truth text.
 - **Levenshtein** **ratio** is obtained by dividing the Levenshtein distance by sum of number of characters in generated text and ground truth. This type of metrics is suitable where one works with short and precise texts.
 
-### 🖊 N-Gram based
+### :2nd_place_medal: N-Gram based
 
 N-gram based metrics as name indicates uses n-grams for comparing generated answer with ground truth. It is suitable to extractive and abstractive tasks but has its limitations in long free form answers due to the word based comparison.
 
 - **ROGUE** (Recall-Oriented Understudy for Gisting Evaluation):
     - **ROUGE-N** measures the number of matching ‘n-grams’ between generated text and ground truth. These matches do not consider the ordering of words.
     - **ROUGE-L** measures the longest common subsequence (LCS) between generated text and ground truth. This means is that we count the longest sequence of tokens that is shared between both
 
 - **BLEU** (BiLingual Evaluation Understudy)
 
-It measures precision by comparing  clipped n-grams in generated text to ground truth text. These matches do not consider the ordering of words.
+    It measures precision by comparing  clipped n-grams in generated text to ground truth text. These matches do not consider the ordering of words.
 
-### 🪄 Model Based
+### :1st_place_medal: Model Based
 
 Model based methods uses language models combined with NLP techniques to compare generated text with ground truth.  It is well suited for free form long or short answer types. 
 
 - **BertScore**
     
     Bert Score measures the similarity between ground truth text answers and generated text using SBERT vector embeddings. The common choice of similarity measure is cosine similarity for which values range between 0 to 1. It shows good correlation with human judgement.
     
@@ -112,11 +113,11 @@
 - **EntailmentScore**
     
     Textual entailment to measure factual consistency in generated text given ground truth. Score can range from 0 to 1 with latter indicating perfect factual entailment for all samples. Entailment score is highly correlated with human judgement.
     
 
 - **$Q^2$**
     
-    Best used to measure factual consistencies between ground truth and generated text. Scores can range from 0 to 1. Higher score indicates better factual consistency between ground truth and generated answer. Employs QA-QG paradigm followed by NLI to compare ground truth and generated answer. Q2Score score is highly correlated with human judgement.
+    Best used to measure factual consistencies between ground truth and generated text. Scores can range from 0 to 1. Higher score indicates better factual consistency between ground truth and generated answer. Employs QA-QG paradigm followed by NLI to compare ground truth and generated answer. $Q^2$ score is highly correlated with human judgement. :warning: time and resource hungry metrics. 
 
-📜 Checkout [citations](./citations.md) for related publications.
+📜 Checkout [citations](./references.md) for related publications.
```

#### html2text {}

```diff
@@ -1,59 +1,60 @@
-Metadata-Version: 2.1 Name: ragas Version: 0.0.1a7 Description-Content-Type:
+Metadata-Version: 2.1 Name: ragas Version: 0.0.2 Description-Content-Type:
 text/plain License-File: LICENSE
                     ****** [./docs/assets/logo.png] ******
        SOTA metrics for evaluating Retrieval Augmented Generation (RAG)
         [GitHub_release] [Build] [License] [Open_In_Colab] [Downloads]
-              *** Installation | Quick_Example | Hugging_Face ***
+          *** Installation | Quickstart | Metrics | Hugging_Face ***
 ragas is a framework that helps you evaluate your Retrieval Augmented
 Generation (RAG) pipelines. RAG denotes a class of LLM applications that use
 external data to augment the LLMâs context. There are existing tools and
 frameworks that help you build these pipelines but evaluating it and
 quantifying your pipeline performance can be hard.. This is were ragas (RAG
 Assessment) comes in ragas provides you with the tools based on the latest
 research for evaluating LLM generated text to give you insights about your RAG
 pipeline. ragas can be integrated with your CI/CD to provide continuous check
-to ensure performance. ## Installation ð¡ ```bash pip install ragas ``` if
-you want to install from source ```bash git clone https://github.com/
-explodinggradients/ragas && cd ragas pip install -e . ``` ## Quickstart ð¥
+to ensure performance. ## :shield: Installation ```bash pip install ragas ```
+if you want to install from source ```bash git clone https://github.com/
+explodinggradients/ragas && cd ragas pip install -e . ``` ## :fire: Quickstart
 This is a small example program you can run to see ragas in action! ```python
 from datasets import load_dataset from ragas.metrics import ( Evaluation,
 rouge1, bert_score, entailment_score, ) # import the metrics you want to use #
 load the dataset ds = load_dataset("explodinggradients/eli5-test",
 split="test_eli5").select(range(100)) # init the evaluator, this takes in the
 metrics you want to use # and performs the evaluation e = Evaluation( metrics=
 [rouge1, bert_score, entailment_score,], batched=False, batch_size=30, ) # run
 the evaluation results = e.eval(ds["ground_truth"], ds["generated_text"]) print
 (results) ``` If you want a more in-depth explanation of core components, check
-out our quick-start notebook ## ð§° Metrics ### âï¸ Character based -
-**Levenshtein distance** the number of single character edits (additional,
-insertion, deletion) required to change your generated text to ground truth
-text. - **Levenshtein** **ratio** is obtained by dividing the Levenshtein
-distance by sum of number of characters in generated text and ground truth.
-This type of metrics is suitable where one works with short and precise texts.
-### ð N-Gram based N-gram based metrics as name indicates uses n-grams for
-comparing generated answer with ground truth. It is suitable to extractive and
-abstractive tasks but has its limitations in long free form answers due to the
-word based comparison. - **ROGUE** (Recall-Oriented Understudy for Gisting
-Evaluation): - **ROUGE-N** measures the number of matching ân-gramsâ
-between generated text and ground truth. These matches do not consider the
-ordering of words. - **ROUGE-L** measures the longest common subsequence (LCS)
-between generated text and ground truth. This means is that we count the
-longest sequence of tokens that is shared between both - **BLEU** (BiLingual
-Evaluation Understudy) It measures precision by comparingÂ  clipped n-grams in
-generated text to ground truth text. These matches do not consider the ordering
-of words. ### ðª Model Based Model based methods uses language models
-combined with NLP techniques to compare generated text with ground truth. It is
-well suited for free form long or short answer types. - **BertScore** Bert
-Score measures the similarity between ground truth text answers and generated
-text using SBERT vector embeddings. The common choice of similarity measure is
-cosine similarity for which values range between 0 to 1. It shows good
-correlation with human judgement. - **EntailmentScore** Textual entailment to
-measure factual consistency in generated text given ground truth. Score can
-range from 0 to 1 with latter indicating perfect factual entailment for all
-samples. Entailment score is highly correlated with human judgement. -
-**$Q^2$** Best used to measure factual consistencies between ground truth and
-generated text. Scores can range from 0 to 1. Higher score indicates better
-factual consistency between ground truth and generated answer. Employs QA-QG
-paradigm followed by NLI to compare ground truth and generated answer. Q2Score
-score is highly correlated with human judgement. ð Checkout [citations](./
-citations.md) for related publications.
+out our quick-start notebook ## :luggage: Metrics ### :3rd_place_medal:
+Character based - **Levenshtein distance** the number of single character edits
+(additional, insertion, deletion) required to change your generated text to
+ground truth text. - **Levenshtein** **ratio** is obtained by dividing the
+Levenshtein distance by sum of number of characters in generated text and
+ground truth. This type of metrics is suitable where one works with short and
+precise texts. ### :2nd_place_medal: N-Gram based N-gram based metrics as name
+indicates uses n-grams for comparing generated answer with ground truth. It is
+suitable to extractive and abstractive tasks but has its limitations in long
+free form answers due to the word based comparison. - **ROGUE** (Recall-
+Oriented Understudy for Gisting Evaluation): - **ROUGE-N** measures the number
+of matching ân-gramsâ between generated text and ground truth. These
+matches do not consider the ordering of words. - **ROUGE-L** measures the
+longest common subsequence (LCS) between generated text and ground truth. This
+means is that we count the longest sequence of tokens that is shared between
+both - **BLEU** (BiLingual Evaluation Understudy) It measures precision by
+comparingÂ  clipped n-grams in generated text to ground truth text. These
+matches do not consider the ordering of words. ### :1st_place_medal: Model
+Based Model based methods uses language models combined with NLP techniques to
+compare generated text with ground truth. It is well suited for free form long
+or short answer types. - **BertScore** Bert Score measures the similarity
+between ground truth text answers and generated text using SBERT vector
+embeddings. The common choice of similarity measure is cosine similarity for
+which values range between 0 to 1. It shows good correlation with human
+judgement. - **EntailmentScore** Textual entailment to measure factual
+consistency in generated text given ground truth. Score can range from 0 to 1
+with latter indicating perfect factual entailment for all samples. Entailment
+score is highly correlated with human judgement. - **$Q^2$** Best used to
+measure factual consistencies between ground truth and generated text. Scores
+can range from 0 to 1. Higher score indicates better factual consistency
+between ground truth and generated answer. Employs QA-QG paradigm followed by
+NLI to compare ground truth and generated answer. $Q^2$ score is highly
+correlated with human judgement. :warning: time and resource hungry metrics.
+ð Checkout [citations](./references.md) for related publications.
```

### Comparing `ragas-0.0.1a7/README.md` & `ragas-0.0.2/ragas.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,64 @@
+Metadata-Version: 2.1
+Name: ragas
+Version: 0.0.2
+Description-Content-Type: text/plain
+License-File: LICENSE
+
 <h1 align="center">
   <img style="vertical-align:middle" height="200"
   src="./docs/assets/logo.png">
 </h1>
 <p align="center">
   <i>SOTA metrics for evaluating Retrieval Augmented Generation (RAG)</i>
 </p>
 
 <p align="center">
-    <a href="https://github.com/beir-cellar/beir/releases">
-        <img alt="GitHub release" src="https://img.shields.io/github/release/beir-cellar/beir.svg">
+    <a href="https://github.com/explodinggradients/ragas/releases">
+        <img alt="GitHub release" src="https://img.shields.io/github/release/explodinggradients/ragas.svg">
     </a>
     <a href="https://www.python.org/">
             <img alt="Build" src="https://img.shields.io/badge/Made%20with-Python-1f425f.svg?color=purple">
     </a>
-    <a href="https://github.com/beir-cellar/beir/blob/master/LICENSE">
-        <img alt="License" src="https://img.shields.io/github/license/beir-cellar/beir.svg?color=green">
+    <a href="https://github.com/explodinggradients/ragas/blob/master/LICENSE">
+        <img alt="License" src="https://img.shields.io/github/license/explodinggradients/ragas.svg?color=green">
     </a>
     <a href="https://colab.research.google.com/drive/1HfutiEhHMJLXiWGT8pcipxT5L2TpYEdt?usp=sharing">
         <img alt="Open In Colab" src="https://colab.research.google.com/assets/colab-badge.svg">
     </a>
-    <a href="https://github.com/beir-cellar/beir/">
+    <a href="https://github.com/explodinggradients/ragas/">
         <img alt="Downloads" src="https://badges.frapsoft.com/os/v1/open-source.svg?v=103">
     </a>
 </p>
 
 <h4 align="center">
     <p>
-        <a href="#beers-installation">Installation</a> |
-        <a href="#beers-quick-example">Quick Example</a> |
-        <a href="https://huggingface.co/BeIR">Hugging Face</a>
+        <a href="#shield-installation">Installation</a> |
+        <a href="#fire-quickstart">Quickstart</a> |
+        <a href="#luggage-metrics">Metrics</a> |
+        <a href="https://huggingface.co/explodinggradients">Hugging Face</a>
     <p>
 </h4>
 
 ragas is a framework that helps you evaluate your Retrieval Augmented Generation (RAG) pipelines. RAG denotes a class of LLM applications that use external data to augment the LLM’s context. There are existing tools and frameworks that help you build these pipelines but evaluating it and quantifying your pipeline performance can be hard.. This is were ragas (RAG Assessment) comes in
 
 ragas provides you with the tools based on the latest research for evaluating LLM generated text  to give you insights about your RAG pipeline. ragas can be integrated with your CI/CD to provide continuous check to ensure performance.
 
-## Installation 🛡
+## :shield: Installation
 
 ```bash
 pip install ragas
 ```
 if you want to install from source 
 ```bash
 git clone https://github.com/explodinggradients/ragas && cd ragas
 pip install -e .
 ```
 
-## Quickstart 🔥
+## :fire: Quickstart 
 
 This is a small example program you can run to see ragas in action!
 ```python
 from datasets import load_dataset
 from ragas.metrics import (
     Evaluation,
     rouge1,
@@ -71,34 +78,34 @@
 )
 
 # run the evaluation
 results = e.eval(ds["ground_truth"], ds["generated_text"])
 print(results)
 ```
 If you want a more in-depth explanation of core components, check out our quick-start notebook
-## 🧰 Metrics
+## :luggage: Metrics
 
-### ✏️ Character based 
+### :3rd_place_medal: Character based 
 
 - **Levenshtein distance** the number of single character edits (additional, insertion, deletion) required to change your generated text to ground truth text.
 - **Levenshtein** **ratio** is obtained by dividing the Levenshtein distance by sum of number of characters in generated text and ground truth. This type of metrics is suitable where one works with short and precise texts.
 
-### 🖊 N-Gram based
+### :2nd_place_medal: N-Gram based
 
 N-gram based metrics as name indicates uses n-grams for comparing generated answer with ground truth. It is suitable to extractive and abstractive tasks but has its limitations in long free form answers due to the word based comparison.
 
 - **ROGUE** (Recall-Oriented Understudy for Gisting Evaluation):
     - **ROUGE-N** measures the number of matching ‘n-grams’ between generated text and ground truth. These matches do not consider the ordering of words.
     - **ROUGE-L** measures the longest common subsequence (LCS) between generated text and ground truth. This means is that we count the longest sequence of tokens that is shared between both
 
 - **BLEU** (BiLingual Evaluation Understudy)
 
-It measures precision by comparing  clipped n-grams in generated text to ground truth text. These matches do not consider the ordering of words.
+    It measures precision by comparing  clipped n-grams in generated text to ground truth text. These matches do not consider the ordering of words.
 
-### 🪄 Model Based
+### :1st_place_medal: Model Based
 
 Model based methods uses language models combined with NLP techniques to compare generated text with ground truth.  It is well suited for free form long or short answer types. 
 
 - **BertScore**
     
     Bert Score measures the similarity between ground truth text answers and generated text using SBERT vector embeddings. The common choice of similarity measure is cosine similarity for which values range between 0 to 1. It shows good correlation with human judgement.
     
@@ -106,11 +113,11 @@
 - **EntailmentScore**
     
     Textual entailment to measure factual consistency in generated text given ground truth. Score can range from 0 to 1 with latter indicating perfect factual entailment for all samples. Entailment score is highly correlated with human judgement.
     
 
 - **$Q^2$**
     
-    Best used to measure factual consistencies between ground truth and generated text. Scores can range from 0 to 1. Higher score indicates better factual consistency between ground truth and generated answer. Employs QA-QG paradigm followed by NLI to compare ground truth and generated answer. Q2Score score is highly correlated with human judgement.
+    Best used to measure factual consistencies between ground truth and generated text. Scores can range from 0 to 1. Higher score indicates better factual consistency between ground truth and generated answer. Employs QA-QG paradigm followed by NLI to compare ground truth and generated answer. $Q^2$ score is highly correlated with human judgement. :warning: time and resource hungry metrics. 
 
-📜 Checkout [citations](./citations.md) for related publications.
+📜 Checkout [citations](./references.md) for related publications.
```

#### html2text {}

```diff
@@ -1,57 +1,60 @@
+Metadata-Version: 2.1 Name: ragas Version: 0.0.2 Description-Content-Type:
+text/plain License-File: LICENSE
                     ****** [./docs/assets/logo.png] ******
        SOTA metrics for evaluating Retrieval Augmented Generation (RAG)
         [GitHub_release] [Build] [License] [Open_In_Colab] [Downloads]
-              *** Installation | Quick_Example | Hugging_Face ***
+          *** Installation | Quickstart | Metrics | Hugging_Face ***
 ragas is a framework that helps you evaluate your Retrieval Augmented
 Generation (RAG) pipelines. RAG denotes a class of LLM applications that use
 external data to augment the LLMâs context. There are existing tools and
 frameworks that help you build these pipelines but evaluating it and
 quantifying your pipeline performance can be hard.. This is were ragas (RAG
 Assessment) comes in ragas provides you with the tools based on the latest
 research for evaluating LLM generated text to give you insights about your RAG
 pipeline. ragas can be integrated with your CI/CD to provide continuous check
-to ensure performance. ## Installation ð¡ ```bash pip install ragas ``` if
-you want to install from source ```bash git clone https://github.com/
-explodinggradients/ragas && cd ragas pip install -e . ``` ## Quickstart ð¥
+to ensure performance. ## :shield: Installation ```bash pip install ragas ```
+if you want to install from source ```bash git clone https://github.com/
+explodinggradients/ragas && cd ragas pip install -e . ``` ## :fire: Quickstart
 This is a small example program you can run to see ragas in action! ```python
 from datasets import load_dataset from ragas.metrics import ( Evaluation,
 rouge1, bert_score, entailment_score, ) # import the metrics you want to use #
 load the dataset ds = load_dataset("explodinggradients/eli5-test",
 split="test_eli5").select(range(100)) # init the evaluator, this takes in the
 metrics you want to use # and performs the evaluation e = Evaluation( metrics=
 [rouge1, bert_score, entailment_score,], batched=False, batch_size=30, ) # run
 the evaluation results = e.eval(ds["ground_truth"], ds["generated_text"]) print
 (results) ``` If you want a more in-depth explanation of core components, check
-out our quick-start notebook ## ð§° Metrics ### âï¸ Character based -
-**Levenshtein distance** the number of single character edits (additional,
-insertion, deletion) required to change your generated text to ground truth
-text. - **Levenshtein** **ratio** is obtained by dividing the Levenshtein
-distance by sum of number of characters in generated text and ground truth.
-This type of metrics is suitable where one works with short and precise texts.
-### ð N-Gram based N-gram based metrics as name indicates uses n-grams for
-comparing generated answer with ground truth. It is suitable to extractive and
-abstractive tasks but has its limitations in long free form answers due to the
-word based comparison. - **ROGUE** (Recall-Oriented Understudy for Gisting
-Evaluation): - **ROUGE-N** measures the number of matching ân-gramsâ
-between generated text and ground truth. These matches do not consider the
-ordering of words. - **ROUGE-L** measures the longest common subsequence (LCS)
-between generated text and ground truth. This means is that we count the
-longest sequence of tokens that is shared between both - **BLEU** (BiLingual
-Evaluation Understudy) It measures precision by comparingÂ  clipped n-grams in
-generated text to ground truth text. These matches do not consider the ordering
-of words. ### ðª Model Based Model based methods uses language models
-combined with NLP techniques to compare generated text with ground truth. It is
-well suited for free form long or short answer types. - **BertScore** Bert
-Score measures the similarity between ground truth text answers and generated
-text using SBERT vector embeddings. The common choice of similarity measure is
-cosine similarity for which values range between 0 to 1. It shows good
-correlation with human judgement. - **EntailmentScore** Textual entailment to
-measure factual consistency in generated text given ground truth. Score can
-range from 0 to 1 with latter indicating perfect factual entailment for all
-samples. Entailment score is highly correlated with human judgement. -
-**$Q^2$** Best used to measure factual consistencies between ground truth and
-generated text. Scores can range from 0 to 1. Higher score indicates better
-factual consistency between ground truth and generated answer. Employs QA-QG
-paradigm followed by NLI to compare ground truth and generated answer. Q2Score
-score is highly correlated with human judgement. ð Checkout [citations](./
-citations.md) for related publications.
+out our quick-start notebook ## :luggage: Metrics ### :3rd_place_medal:
+Character based - **Levenshtein distance** the number of single character edits
+(additional, insertion, deletion) required to change your generated text to
+ground truth text. - **Levenshtein** **ratio** is obtained by dividing the
+Levenshtein distance by sum of number of characters in generated text and
+ground truth. This type of metrics is suitable where one works with short and
+precise texts. ### :2nd_place_medal: N-Gram based N-gram based metrics as name
+indicates uses n-grams for comparing generated answer with ground truth. It is
+suitable to extractive and abstractive tasks but has its limitations in long
+free form answers due to the word based comparison. - **ROGUE** (Recall-
+Oriented Understudy for Gisting Evaluation): - **ROUGE-N** measures the number
+of matching ân-gramsâ between generated text and ground truth. These
+matches do not consider the ordering of words. - **ROUGE-L** measures the
+longest common subsequence (LCS) between generated text and ground truth. This
+means is that we count the longest sequence of tokens that is shared between
+both - **BLEU** (BiLingual Evaluation Understudy) It measures precision by
+comparingÂ  clipped n-grams in generated text to ground truth text. These
+matches do not consider the ordering of words. ### :1st_place_medal: Model
+Based Model based methods uses language models combined with NLP techniques to
+compare generated text with ground truth. It is well suited for free form long
+or short answer types. - **BertScore** Bert Score measures the similarity
+between ground truth text answers and generated text using SBERT vector
+embeddings. The common choice of similarity measure is cosine similarity for
+which values range between 0 to 1. It shows good correlation with human
+judgement. - **EntailmentScore** Textual entailment to measure factual
+consistency in generated text given ground truth. Score can range from 0 to 1
+with latter indicating perfect factual entailment for all samples. Entailment
+score is highly correlated with human judgement. - **$Q^2$** Best used to
+measure factual consistencies between ground truth and generated text. Scores
+can range from 0 to 1. Higher score indicates better factual consistency
+between ground truth and generated answer. Employs QA-QG paradigm followed by
+NLI to compare ground truth and generated answer. $Q^2$ score is highly
+correlated with human judgement. :warning: time and resource hungry metrics.
+ð Checkout [citations](./references.md) for related publications.
```

### Comparing `ragas-0.0.1a7/citations.md` & `ragas-0.0.2/references.md`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a7/docs/assets/logo.png` & `ragas-0.0.2/docs/assets/logo.png`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a7/examples/data_prep.py` & `ragas-0.0.2/examples/data_prep.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a7/ragas/metrics/base.py` & `ragas-0.0.2/ragas/metrics/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,38 +9,58 @@
 
 
 @dataclass
 class Metric(ABC):
     @property
     @abstractmethod
     def name(self: t.Self) -> str:
+        """
+        the metric name
+        """
         ...
 
     @property
     @abstractmethod
     def is_batchable(self: t.Self) -> bool:
+        """
+        Attribute to check if this metric is is_batchable
+        """
+        ...
+
+    @abstractmethod
+    def init_model():
+        """
+        This method will lazy initialize the model.
+        """
         ...
 
     @abstractmethod
     def score(
         self: t.Self, ground_truth: list[str], generated_text: list[str]
     ) -> list[float]:
+        """
+        Run the metric on the ground_truth and generated_text and return score.
+        """
         ...
 
 
 @dataclass
 class Evaluation:
     metrics: list[Metric]
     batched: bool = True
     batch_size: int = 1000
 
     def eval(self, ground_truth: list[list[str]], generated_text: list[str]) -> Result:
         ds = Dataset.from_dict(
             {"ground_truth": ground_truth, "generated_text": generated_text}
         )
+
+        # initialize all the models in the metrics
+        [m.init_model() for m in self.metrics]
+
         ds = ds.map(
             self._get_score,
             batched=self.batched,
             batch_size=self.batch_size,
             remove_columns=["ground_truth", "generated_text"],
         )
```

### Comparing `ragas-0.0.1a7/ragas/metrics/factual.py` & `ragas-0.0.2/ragas/metrics/factual.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 import json
 import re
 import string
 import typing as t
 from dataclasses import dataclass
+from warnings import warn
 
 import numpy as np
 import spacy
+import torch
 import transformers
+from spacy.cli.download import download as spacy_download
 from transformers import (
     AutoConfig,
     AutoModelForSequenceClassification,
     AutoTokenizer,
     PreTrainedModel,
 )
 
-from ragas.exceptions import RagasException
 from ragas.metrics import Metric
 from ragas.utils import device_check
 
 if t.TYPE_CHECKING:
     from torch import device as Device
 
 from transformers.models.auto.modeling_auto import (
@@ -46,15 +48,15 @@
     """
 
     model_name: str = "typeform/distilbert-base-uncased-mnli"
     max_length: int = 512
     batch_size: int = 4
     device: t.Literal["cpu", "cuda"] | Device = "cpu"
 
-    def __post_init__(self):
+    def init_model(self):
         self.device = device_check(self.device)
         self.tokenizer = AutoTokenizer.from_pretrained(self.model_name)
         self.model = AutoModelForSequenceClassification.from_pretrained(self.model_name)
         self.model.eval()
         self.model.to(self.device)
 
         model_config = self.model.config.to_dict()
@@ -206,24 +208,30 @@
     max_answers: int = 10
     crosscheck_candidates: bool = True
     load_single = False
     batch_size: int = 4
     include_nouns: bool = True
     save_results: bool = False
 
-    def __post_init__(self):
+    def init_model(self):
         self.qa = QAGQ.from_pretrained(self.qa_model_name)
         self.qg = QAGQ.from_pretrained(self.qg_model_name)
+        self.nli = EntailmentScore()
+        self.nli.init_model()
         try:
             self.nlp = spacy.load(SPACY_MODEL)
         except OSError:
-            raise RagasException(
+            warn(
                 f"Spacy model [{SPACY_MODEL}] not found. Please run "
-                "`python -m spacy download {SPACY_MODEL}` to install it."
+                f"`python -m spacy download {SPACY_MODEL}` to install it."
             )
+            # logger.warning(f"Spacy models '{spacy_model_name}' not found."
+            # "  Downloading and installing.")
+            spacy_download(SPACY_MODEL)
+            self.nlp = spacy.load(SPACY_MODEL)
 
     @property
     def name(self):
         return "Qsquare"
 
     @property
     def is_batchable(self):
@@ -284,26 +292,25 @@
         text = text.strip().lower()
         text = text.translate(str.maketrans("", "", string.punctuation))
         text = re.sub(r"\b(a|an|the|in|our)\b", " ", text)
 
         return text
 
     def score_candidates(self, ques_ans_dict: dict):
-        nli = EntailmentScore()
         for qas in ques_ans_dict.values():
             for item in qas:
                 item["answer"] = self.clean_candidate(item["answer"])
                 item["predicted_answer"] = self.clean_candidate(
                     item["predicted_answer"]
                 )
                 if item["answer"] == item["predicted_answer"]:
                     item.update({"score": 1})
                 else:
                     qstn = item.get("question")
-                    score_dict = nli.infer(
+                    score_dict = self.nli.infer(
                         f'{qstn}{item.get("answer")}',
                         f'{qstn}{item.get("predicted_answer")}',
                     )
                     label = max(zip(score_dict.values(), score_dict.keys()))[1]
                     item.update({"score": LABEL2SCORE[label]})
 
         return ques_ans_dict
@@ -316,34 +323,35 @@
             gen_answers = self.generate_answers(questions, context)
             if self.crosscheck_candidates:
                 questions, candidates = self.filter_candidates(
                     questions, candidates, gen_answers
                 )
             gnd_qans[i] = [
                 {"question": qstn, "answer": ans}
-                for qstn, ans in zip(questions, candidates)
+                for qstn, ans in zip(questions, candidates)  # type: ignore
             ]
 
         for i, gen_text in enumerate(generated_text):
             questions = [item["question"] for item in gnd_qans[i]]
             gen_answers = self.generate_answers(questions, gen_text)
             _ = [
                 item.update({"predicted_answer": ans})
-                for item, ans in zip(gnd_qans[i], gen_answers)
+                for item, ans in zip(gnd_qans[i], gen_answers)  # type: ignore
             ]
 
-        del self.qa
-        del self.qg
+        # del self.qa
+        # del self.qg
 
         gnd_qans = self.score_candidates(gnd_qans)
 
         if self.save_results:
             with open("qa-qj-intermediate.json", "w") as file:
                 json.dump(gnd_qans, file, indent=4)
 
         scores = [[dic["score"] for dic in item] for item in gnd_qans.values()]
         scores = [sum(sublist) / (len(sublist) + EPS) for sublist in scores]
         return scores
 
 
-entailment_score = EntailmentScore()
-q_square = Qsquare()
+device = "cuda" if torch.cuda.is_available() else "cpu"
+entailment_score = EntailmentScore(device=device)
+q_square = Qsquare(device=device)
```

### Comparing `ragas-0.0.1a7/ragas/metrics/similarity.py` & `ragas-0.0.2/ragas/metrics/similarity.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 @dataclass
 class BERTScore(Metric):
     similarity_metric: t.Literal[BERT_METRIC] = "cosine"
     model_path: str = "all-MiniLM-L6-v2"
     batch_size: int = 1000
 
-    def __post_init__(self):
+    def init_model(self):
         self.model = SentenceTransformer(self.model_path)
 
     @property
     def name(
         self,
     ):
         return f"BERTScore_{self.similarity_metric}"
@@ -46,16 +46,16 @@
             gndtruth_emb, np.ndarray
         ), (
             f"Both gndtruth_emb[{type(gentext_emb)}], gentext_emb[{type(gentext_emb)}]"
             " should be numpy ndarray."
         )
 
         if self.similarity_metric == "cosine":
-            score = np.dot(gndtruth_emb, gentext_emb.T) / (
-                norm(gndtruth_emb) * norm(gentext_emb)
+            score = np.sum(gndtruth_emb * gentext_emb, axis=1) / (
+                norm(gndtruth_emb, axis=1) * norm(gentext_emb, axis=1)
             )
 
         elif self.similarity_metric == "euclidean":
             score = norm(gndtruth_emb - gentext_emb, ord=2)
 
         else:
             raise ValueError(f"Unkown metrics {self.similarity_metric}")
```

### Comparing `ragas-0.0.1a7/ragas/metrics/simple.py` & `ragas-0.0.2/ragas/metrics/simple.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,17 @@
     def name(self):
         return "BLEU"
 
     @property
     def is_batchable(self):
         return True
 
+    def init_model(self):
+        ...
+
     def score(self, ground_truth: t.List[str], generated_text: t.List[str]):
         ground_truth_ = [[word_tokenize(text)] for text in ground_truth]
         generated_text_ = [word_tokenize(text) for text in generated_text]
         return [
             sentence_bleu(
                 s1,
                 s2,
@@ -41,15 +44,15 @@
 
 
 @dataclass
 class ROUGE(Metric):
     type: t.Literal[ROUGE_TYPES]
     use_stemmer: bool = False
 
-    def __post_init__(self):
+    def init_model(self):
         self.scorer = rouge_scorer.RougeScorer(
             [self.type], use_stemmer=self.use_stemmer
         )
 
     @property
     def name(self):
         return self.type
@@ -76,14 +79,17 @@
     def name(self) -> str:
         return f"edit_{self.measure}"
 
     @property
     def is_batchable(self):
         return True
 
+    def init_model(self):
+        ...
+
     def score(self, ground_truth: t.List[str], generated_text: t.List[str]):
         if self.measure == "distance":
             score = [distance(s1, s2) for s1, s2 in zip(ground_truth, generated_text)]
         elif self.measure == "ratio":
             score = [ratio(s1, s2) for s1, s2 in zip(ground_truth, generated_text)]
         else:
             raise ValueError(f"Unkown measure {self.measure}")
```

### Comparing `ragas-0.0.1a7/ragas/utils.py` & `ragas-0.0.2/ragas/utils.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a7/ragas.egg-info/PKG-INFO` & `ragas-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,58 @@
-Metadata-Version: 2.1
-Name: ragas
-Version: 0.0.1a7
-Description-Content-Type: text/plain
-License-File: LICENSE
-
 <h1 align="center">
   <img style="vertical-align:middle" height="200"
   src="./docs/assets/logo.png">
 </h1>
 <p align="center">
   <i>SOTA metrics for evaluating Retrieval Augmented Generation (RAG)</i>
 </p>
 
 <p align="center">
-    <a href="https://github.com/beir-cellar/beir/releases">
-        <img alt="GitHub release" src="https://img.shields.io/github/release/beir-cellar/beir.svg">
+    <a href="https://github.com/explodinggradients/ragas/releases">
+        <img alt="GitHub release" src="https://img.shields.io/github/release/explodinggradients/ragas.svg">
     </a>
     <a href="https://www.python.org/">
             <img alt="Build" src="https://img.shields.io/badge/Made%20with-Python-1f425f.svg?color=purple">
     </a>
-    <a href="https://github.com/beir-cellar/beir/blob/master/LICENSE">
-        <img alt="License" src="https://img.shields.io/github/license/beir-cellar/beir.svg?color=green">
+    <a href="https://github.com/explodinggradients/ragas/blob/master/LICENSE">
+        <img alt="License" src="https://img.shields.io/github/license/explodinggradients/ragas.svg?color=green">
     </a>
     <a href="https://colab.research.google.com/drive/1HfutiEhHMJLXiWGT8pcipxT5L2TpYEdt?usp=sharing">
         <img alt="Open In Colab" src="https://colab.research.google.com/assets/colab-badge.svg">
     </a>
-    <a href="https://github.com/beir-cellar/beir/">
+    <a href="https://github.com/explodinggradients/ragas/">
         <img alt="Downloads" src="https://badges.frapsoft.com/os/v1/open-source.svg?v=103">
     </a>
 </p>
 
 <h4 align="center">
     <p>
-        <a href="#beers-installation">Installation</a> |
-        <a href="#beers-quick-example">Quick Example</a> |
-        <a href="https://huggingface.co/BeIR">Hugging Face</a>
+        <a href="#shield-installation">Installation</a> |
+        <a href="#fire-quickstart">Quickstart</a> |
+        <a href="#luggage-metrics">Metrics</a> |
+        <a href="https://huggingface.co/explodinggradients">Hugging Face</a>
     <p>
 </h4>
 
 ragas is a framework that helps you evaluate your Retrieval Augmented Generation (RAG) pipelines. RAG denotes a class of LLM applications that use external data to augment the LLM’s context. There are existing tools and frameworks that help you build these pipelines but evaluating it and quantifying your pipeline performance can be hard.. This is were ragas (RAG Assessment) comes in
 
 ragas provides you with the tools based on the latest research for evaluating LLM generated text  to give you insights about your RAG pipeline. ragas can be integrated with your CI/CD to provide continuous check to ensure performance.
 
-## Installation 🛡
+## :shield: Installation
 
 ```bash
 pip install ragas
 ```
 if you want to install from source 
 ```bash
 git clone https://github.com/explodinggradients/ragas && cd ragas
 pip install -e .
 ```
 
-## Quickstart 🔥
+## :fire: Quickstart 
 
 This is a small example program you can run to see ragas in action!
 ```python
 from datasets import load_dataset
 from ragas.metrics import (
     Evaluation,
     rouge1,
@@ -77,34 +72,34 @@
 )
 
 # run the evaluation
 results = e.eval(ds["ground_truth"], ds["generated_text"])
 print(results)
 ```
 If you want a more in-depth explanation of core components, check out our quick-start notebook
-## 🧰 Metrics
+## :luggage: Metrics
 
-### ✏️ Character based 
+### :3rd_place_medal: Character based 
 
 - **Levenshtein distance** the number of single character edits (additional, insertion, deletion) required to change your generated text to ground truth text.
 - **Levenshtein** **ratio** is obtained by dividing the Levenshtein distance by sum of number of characters in generated text and ground truth. This type of metrics is suitable where one works with short and precise texts.
 
-### 🖊 N-Gram based
+### :2nd_place_medal: N-Gram based
 
 N-gram based metrics as name indicates uses n-grams for comparing generated answer with ground truth. It is suitable to extractive and abstractive tasks but has its limitations in long free form answers due to the word based comparison.
 
 - **ROGUE** (Recall-Oriented Understudy for Gisting Evaluation):
     - **ROUGE-N** measures the number of matching ‘n-grams’ between generated text and ground truth. These matches do not consider the ordering of words.
     - **ROUGE-L** measures the longest common subsequence (LCS) between generated text and ground truth. This means is that we count the longest sequence of tokens that is shared between both
 
 - **BLEU** (BiLingual Evaluation Understudy)
 
-It measures precision by comparing  clipped n-grams in generated text to ground truth text. These matches do not consider the ordering of words.
+    It measures precision by comparing  clipped n-grams in generated text to ground truth text. These matches do not consider the ordering of words.
 
-### 🪄 Model Based
+### :1st_place_medal: Model Based
 
 Model based methods uses language models combined with NLP techniques to compare generated text with ground truth.  It is well suited for free form long or short answer types. 
 
 - **BertScore**
     
     Bert Score measures the similarity between ground truth text answers and generated text using SBERT vector embeddings. The common choice of similarity measure is cosine similarity for which values range between 0 to 1. It shows good correlation with human judgement.
     
@@ -112,11 +107,11 @@
 - **EntailmentScore**
     
     Textual entailment to measure factual consistency in generated text given ground truth. Score can range from 0 to 1 with latter indicating perfect factual entailment for all samples. Entailment score is highly correlated with human judgement.
     
 
 - **$Q^2$**
     
-    Best used to measure factual consistencies between ground truth and generated text. Scores can range from 0 to 1. Higher score indicates better factual consistency between ground truth and generated answer. Employs QA-QG paradigm followed by NLI to compare ground truth and generated answer. Q2Score score is highly correlated with human judgement.
+    Best used to measure factual consistencies between ground truth and generated text. Scores can range from 0 to 1. Higher score indicates better factual consistency between ground truth and generated answer. Employs QA-QG paradigm followed by NLI to compare ground truth and generated answer. $Q^2$ score is highly correlated with human judgement. :warning: time and resource hungry metrics. 
 
-📜 Checkout [citations](./citations.md) for related publications.
+📜 Checkout [citations](./references.md) for related publications.
```

#### html2text {}

```diff
@@ -1,59 +1,58 @@
-Metadata-Version: 2.1 Name: ragas Version: 0.0.1a7 Description-Content-Type:
-text/plain License-File: LICENSE
                     ****** [./docs/assets/logo.png] ******
        SOTA metrics for evaluating Retrieval Augmented Generation (RAG)
         [GitHub_release] [Build] [License] [Open_In_Colab] [Downloads]
-              *** Installation | Quick_Example | Hugging_Face ***
+          *** Installation | Quickstart | Metrics | Hugging_Face ***
 ragas is a framework that helps you evaluate your Retrieval Augmented
 Generation (RAG) pipelines. RAG denotes a class of LLM applications that use
 external data to augment the LLMâs context. There are existing tools and
 frameworks that help you build these pipelines but evaluating it and
 quantifying your pipeline performance can be hard.. This is were ragas (RAG
 Assessment) comes in ragas provides you with the tools based on the latest
 research for evaluating LLM generated text to give you insights about your RAG
 pipeline. ragas can be integrated with your CI/CD to provide continuous check
-to ensure performance. ## Installation ð¡ ```bash pip install ragas ``` if
-you want to install from source ```bash git clone https://github.com/
-explodinggradients/ragas && cd ragas pip install -e . ``` ## Quickstart ð¥
+to ensure performance. ## :shield: Installation ```bash pip install ragas ```
+if you want to install from source ```bash git clone https://github.com/
+explodinggradients/ragas && cd ragas pip install -e . ``` ## :fire: Quickstart
 This is a small example program you can run to see ragas in action! ```python
 from datasets import load_dataset from ragas.metrics import ( Evaluation,
 rouge1, bert_score, entailment_score, ) # import the metrics you want to use #
 load the dataset ds = load_dataset("explodinggradients/eli5-test",
 split="test_eli5").select(range(100)) # init the evaluator, this takes in the
 metrics you want to use # and performs the evaluation e = Evaluation( metrics=
 [rouge1, bert_score, entailment_score,], batched=False, batch_size=30, ) # run
 the evaluation results = e.eval(ds["ground_truth"], ds["generated_text"]) print
 (results) ``` If you want a more in-depth explanation of core components, check
-out our quick-start notebook ## ð§° Metrics ### âï¸ Character based -
-**Levenshtein distance** the number of single character edits (additional,
-insertion, deletion) required to change your generated text to ground truth
-text. - **Levenshtein** **ratio** is obtained by dividing the Levenshtein
-distance by sum of number of characters in generated text and ground truth.
-This type of metrics is suitable where one works with short and precise texts.
-### ð N-Gram based N-gram based metrics as name indicates uses n-grams for
-comparing generated answer with ground truth. It is suitable to extractive and
-abstractive tasks but has its limitations in long free form answers due to the
-word based comparison. - **ROGUE** (Recall-Oriented Understudy for Gisting
-Evaluation): - **ROUGE-N** measures the number of matching ân-gramsâ
-between generated text and ground truth. These matches do not consider the
-ordering of words. - **ROUGE-L** measures the longest common subsequence (LCS)
-between generated text and ground truth. This means is that we count the
-longest sequence of tokens that is shared between both - **BLEU** (BiLingual
-Evaluation Understudy) It measures precision by comparingÂ  clipped n-grams in
-generated text to ground truth text. These matches do not consider the ordering
-of words. ### ðª Model Based Model based methods uses language models
-combined with NLP techniques to compare generated text with ground truth. It is
-well suited for free form long or short answer types. - **BertScore** Bert
-Score measures the similarity between ground truth text answers and generated
-text using SBERT vector embeddings. The common choice of similarity measure is
-cosine similarity for which values range between 0 to 1. It shows good
-correlation with human judgement. - **EntailmentScore** Textual entailment to
-measure factual consistency in generated text given ground truth. Score can
-range from 0 to 1 with latter indicating perfect factual entailment for all
-samples. Entailment score is highly correlated with human judgement. -
-**$Q^2$** Best used to measure factual consistencies between ground truth and
-generated text. Scores can range from 0 to 1. Higher score indicates better
-factual consistency between ground truth and generated answer. Employs QA-QG
-paradigm followed by NLI to compare ground truth and generated answer. Q2Score
-score is highly correlated with human judgement. ð Checkout [citations](./
-citations.md) for related publications.
+out our quick-start notebook ## :luggage: Metrics ### :3rd_place_medal:
+Character based - **Levenshtein distance** the number of single character edits
+(additional, insertion, deletion) required to change your generated text to
+ground truth text. - **Levenshtein** **ratio** is obtained by dividing the
+Levenshtein distance by sum of number of characters in generated text and
+ground truth. This type of metrics is suitable where one works with short and
+precise texts. ### :2nd_place_medal: N-Gram based N-gram based metrics as name
+indicates uses n-grams for comparing generated answer with ground truth. It is
+suitable to extractive and abstractive tasks but has its limitations in long
+free form answers due to the word based comparison. - **ROGUE** (Recall-
+Oriented Understudy for Gisting Evaluation): - **ROUGE-N** measures the number
+of matching ân-gramsâ between generated text and ground truth. These
+matches do not consider the ordering of words. - **ROUGE-L** measures the
+longest common subsequence (LCS) between generated text and ground truth. This
+means is that we count the longest sequence of tokens that is shared between
+both - **BLEU** (BiLingual Evaluation Understudy) It measures precision by
+comparingÂ  clipped n-grams in generated text to ground truth text. These
+matches do not consider the ordering of words. ### :1st_place_medal: Model
+Based Model based methods uses language models combined with NLP techniques to
+compare generated text with ground truth. It is well suited for free form long
+or short answer types. - **BertScore** Bert Score measures the similarity
+between ground truth text answers and generated text using SBERT vector
+embeddings. The common choice of similarity measure is cosine similarity for
+which values range between 0 to 1. It shows good correlation with human
+judgement. - **EntailmentScore** Textual entailment to measure factual
+consistency in generated text given ground truth. Score can range from 0 to 1
+with latter indicating perfect factual entailment for all samples. Entailment
+score is highly correlated with human judgement. - **$Q^2$** Best used to
+measure factual consistencies between ground truth and generated text. Scores
+can range from 0 to 1. Higher score indicates better factual consistency
+between ground truth and generated answer. Employs QA-QG paradigm followed by
+NLI to compare ground truth and generated answer. $Q^2$ score is highly
+correlated with human judgement. :warning: time and resource hungry metrics.
+ð Checkout [citations](./references.md) for related publications.
```

### Comparing `ragas-0.0.1a7/ragas.egg-info/SOURCES.txt` & `ragas-0.0.2/ragas.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .gitignore
 LICENSE
 Makefile
 README.md
-citations.md
 pyproject.toml
+references.md
 .github/workflows/ci.yaml
 .github/workflows/python-publish.yml
 docs/assets/logo.png
 examples/data_prep.py
 examples/quickstart.ipynb
 ragas/__init__.py
 ragas/_version.py
@@ -22,9 +22,10 @@
 ragas/metrics/base.py
 ragas/metrics/factual.py
 ragas/metrics/similarity.py
 ragas/metrics/simple.py
 requirements/dev.txt
 requirements/test.txt
 tests/benchmarks/benchmark.py
+tests/benchmarks/benchmark_eval.py
 tests/benchmarks/utils.py
 tests/unit/test_simple.py
```

### Comparing `ragas-0.0.1a7/tests/benchmarks/benchmark.py` & `ragas-0.0.2/tests/benchmarks/benchmark.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import typing as t
 
 from datasets import Dataset, arrow_dataset, load_dataset
 from torch.cuda import is_available
 from tqdm import tqdm
 from utils import print_table, timeit
 
-from ragas.metrics import Evaluation, edit_distance, edit_ratio, rouge1, rouge2, rougeL
+from ragas.metrics import (
+    Evaluation,
+    bert_score,
+    edit_ratio,
+    rouge1,
+)
 
 DEVICE = "cuda" if is_available() else "cpu"
-BATCHES = [0, 1]
+BATCHES = [0, 1, 30, 60]
 
 METRICS = {
     "Rouge1": rouge1,
-    "Rouge2": rouge2,
-    "RougeL": rougeL,
+    # "Rouge2": rouge2,
+    # "RougeL": rougeL,
     "EditRatio": edit_ratio,
-    "EditDistance": edit_distance,
-    # "SBERTScore": sbert_score,
-    # "EntailmentScore": entail,
+    # "EditDistance": edit_distance,
+    "SBERTScore": bert_score,
+    # "EntailmentScore": entailment_score,
+    # "Qsquare": q_square,
 }
 DS = load_dataset("explodinggradients/eli5-test", split="test_eli5")
 assert isinstance(DS, arrow_dataset.Dataset), "Not an arrow_dataset"
 DS = DS.select(range(100))
 
 
 def setup() -> t.Iterator[tuple[str, Evaluation, Dataset]]:
```

### Comparing `ragas-0.0.1a7/tests/benchmarks/utils.py` & `ragas-0.0.2/tests/benchmarks/utils.py`

 * *Files identical despite different names*

