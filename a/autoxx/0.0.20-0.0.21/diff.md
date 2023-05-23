# Comparing `tmp/autoxx-0.0.20.tar.gz` & `tmp/autoxx-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.20.tar", max compression
+gzip compressed data, was "autoxx-0.0.21.tar", max compression
```

## Comparing `autoxx-0.0.20.tar` & `autoxx-0.0.21.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.20/README.md
--rw-r--r--   0        0        0     7194 2023-05-23 03:43:48.025037 autoxx-0.0.20/autoxx/agent/babyagi/agi.py
--rw-r--r--   0        0        0     1109 2023-05-22 11:10:29.311248 autoxx-0.0.20/autoxx/agent/babyagi/task_manager.py
--rw-r--r--   0        0        0    10193 2023-05-22 08:58:57.762888 autoxx-0.0.20/autoxx/agent/react/agent.py
--rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.20/autoxx/requirements.txt
--rw-r--r--   0        0        0      619 2023-05-23 00:34:07.217327 autoxx-0.0.20/autoxx/setup.py
--rw-r--r--   0        0        0     5352 2023-05-22 11:51:39.068804 autoxx-0.0.20/autoxx/tools/knowledge_base/utils.py
--rw-r--r--   0        0        0      929 2023-05-22 06:15:52.199109 autoxx-0.0.20/autoxx/tools/llm/utils.py
--rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.20/autoxx/tools/web_search/js/overlay.js
--rw-r--r--   0        0        0     6247 2023-05-23 05:10:30.480843 autoxx-0.0.20/autoxx/tools/web_search/search.py
--rw-r--r--   0        0        0      664 2023-05-23 05:10:40.050949 autoxx-0.0.20/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 autoxx-0.0.20/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.21/README.md
+-rw-r--r--   0        0        0     7194 2023-05-23 03:43:48.025037 autoxx-0.0.21/autoxx/agent/babyagi/agi.py
+-rw-r--r--   0        0        0     1109 2023-05-22 11:10:29.311248 autoxx-0.0.21/autoxx/agent/babyagi/task_manager.py
+-rw-r--r--   0        0        0    10193 2023-05-22 08:58:57.762888 autoxx-0.0.21/autoxx/agent/react/agent.py
+-rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.21/autoxx/requirements.txt
+-rw-r--r--   0        0        0      800 2023-05-23 05:45:02.494638 autoxx-0.0.21/autoxx/setup.py
+-rw-r--r--   0        0        0     5352 2023-05-22 11:51:39.068804 autoxx-0.0.21/autoxx/tools/knowledge_base/utils.py
+-rw-r--r--   0        0        0      929 2023-05-22 06:15:52.199109 autoxx-0.0.21/autoxx/tools/llm/utils.py
+-rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.21/autoxx/tools/web_search/js/overlay.js
+-rw-r--r--   0        0        0     6247 2023-05-23 05:10:30.480843 autoxx-0.0.21/autoxx/tools/web_search/search.py
+-rw-r--r--   0        0        0      664 2023-05-23 05:45:08.540299 autoxx-0.0.21/pyproject.toml
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 autoxx-0.0.21/PKG-INFO
```

### Comparing `autoxx-0.0.20/autoxx/agent/babyagi/agi.py` & `autoxx-0.0.21/autoxx/agent/babyagi/agi.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.20/autoxx/agent/babyagi/task_manager.py` & `autoxx-0.0.21/autoxx/agent/babyagi/task_manager.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.20/autoxx/agent/react/agent.py` & `autoxx-0.0.21/autoxx/agent/react/agent.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.20/autoxx/setup.py` & `autoxx-0.0.21/autoxx/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,13 +10,16 @@
     CFG = Config()
     if azure_config_file != "":
         CFG.set_openai_api_key(os.getenv("AZURE_OPENAI_API_KEY", ""))
         CFG.use_azure=True
         CFG.load_azure_config(config_file=azure_config_file)
 
     CFG.set_debug_mode(debug)
+    if CFG.google_api_key is None:
+        CFG.set_google_api_key(os.getenv("GOOGLE_API_KEY", ""))
+        CFG.set_custom_search_engine_id(os.getenv("CUSTOM_SEARCH_ENGINE_ID", ""))
 
     openai.api_type = CFG.openai_api_type
     openai.api_base = CFG.openai_api_base
     openai.api_version = CFG.openai_api_version
     openai.api_key = CFG.openai_api_key
     return CFG
```

### Comparing `autoxx-0.0.20/autoxx/tools/knowledge_base/utils.py` & `autoxx-0.0.21/autoxx/tools/knowledge_base/utils.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.20/autoxx/tools/llm/utils.py` & `autoxx-0.0.21/autoxx/tools/llm/utils.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.20/autoxx/tools/web_search/js/overlay.js` & `autoxx-0.0.21/autoxx/tools/web_search/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.20/autoxx/tools/web_search/search.py` & `autoxx-0.0.21/autoxx/tools/web_search/search.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.20/pyproject.toml` & `autoxx-0.0.21/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.20"
+version = "0.0.21"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `autoxx-0.0.20/PKG-INFO` & `autoxx-0.0.21/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.20
+Version: 0.0.21
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

