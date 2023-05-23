# Comparing `tmp/llm_cost_estimation-0.1.0.tar.gz` & `tmp/llm_cost_estimation-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_cost_estimation-0.1.0.tar", max compression
+gzip compressed data, was "llm_cost_estimation-0.1.1.tar", max compression
```

## Comparing `llm_cost_estimation-0.1.0.tar` & `llm_cost_estimation-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1103 2023-05-23 14:27:07.572982 llm_cost_estimation-0.1.0/LICENSE
--rw-r--r--   0        0        0      169 2023-05-23 14:13:32.567999 llm_cost_estimation-0.1.0/llm_cost_estimation/__init__.py
--rw-r--r--   0        0        0     2565 2023-05-23 14:28:21.073207 llm_cost_estimation-0.1.0/llm_cost_estimation/count_tokens.py
--rw-r--r--   0        0        0     4340 2023-05-23 14:13:45.642121 llm_cost_estimation-0.1.0/llm_cost_estimation/estimate_cost.py
--rw-r--r--   0        0        0     6207 2023-05-23 14:04:51.303595 llm_cost_estimation-0.1.0/llm_cost_estimation/models.py
--rw-r--r--   0        0        0      465 2023-05-23 14:08:39.816665 llm_cost_estimation-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8361 2023-05-23 15:07:32.078689 llm_cost_estimation-0.1.0/README.md
--rw-r--r--   0        0        0     8685 1970-01-01 00:00:00.000000 llm_cost_estimation-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1103 2023-05-23 14:27:07.572982 llm_cost_estimation-0.1.1/LICENSE
+-rw-r--r--   0        0        0      169 2023-05-23 14:13:32.567999 llm_cost_estimation-0.1.1/llm_cost_estimation/__init__.py
+-rw-r--r--   0        0        0     2565 2023-05-23 14:28:21.073207 llm_cost_estimation-0.1.1/llm_cost_estimation/count_tokens.py
+-rw-r--r--   0        0        0     4340 2023-05-23 14:13:45.642121 llm_cost_estimation-0.1.1/llm_cost_estimation/estimate_cost.py
+-rw-r--r--   0        0        0     6207 2023-05-23 14:04:51.303595 llm_cost_estimation-0.1.1/llm_cost_estimation/models.py
+-rw-r--r--   0        0        0      484 2023-05-23 15:18:25.807590 llm_cost_estimation-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8361 2023-05-23 15:07:32.078689 llm_cost_estimation-0.1.1/README.md
+-rw-r--r--   0        0        0     8685 1970-01-01 00:00:00.000000 llm_cost_estimation-0.1.1/PKG-INFO
```

### Comparing `llm_cost_estimation-0.1.0/LICENSE` & `llm_cost_estimation-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_cost_estimation-0.1.0/llm_cost_estimation/count_tokens.py` & `llm_cost_estimation-0.1.1/llm_cost_estimation/count_tokens.py`

 * *Files identical despite different names*

### Comparing `llm_cost_estimation-0.1.0/llm_cost_estimation/estimate_cost.py` & `llm_cost_estimation-0.1.1/llm_cost_estimation/estimate_cost.py`

 * *Files identical despite different names*

### Comparing `llm_cost_estimation-0.1.0/llm_cost_estimation/models.py` & `llm_cost_estimation-0.1.1/llm_cost_estimation/models.py`

 * *Files identical despite different names*

### Comparing `llm_cost_estimation-0.1.0/README.md` & `llm_cost_estimation-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `llm_cost_estimation-0.1.0/PKG-INFO` & `llm_cost_estimation-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-cost-estimation
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Christopher Carroll Smith
 Author-email: 75859865+chriscarrollsmith@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

