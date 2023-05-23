# Comparing `tmp/autoxx-0.0.19.tar.gz` & `tmp/autoxx-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.19.tar", max compression
+gzip compressed data, was "autoxx-0.0.20.tar", max compression
```

## Comparing `autoxx-0.0.19.tar` & `autoxx-0.0.20.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.19/README.md
--rw-r--r--   0        0        0     7194 2023-05-23 03:43:48.025037 autoxx-0.0.19/autoxx/agent/babyagi/agi.py
--rw-r--r--   0        0        0     1109 2023-05-22 11:10:29.311248 autoxx-0.0.19/autoxx/agent/babyagi/task_manager.py
--rw-r--r--   0        0        0    10193 2023-05-22 08:58:57.762888 autoxx-0.0.19/autoxx/agent/react/agent.py
--rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.19/autoxx/requirements.txt
--rw-r--r--   0        0        0      619 2023-05-23 00:34:07.217327 autoxx-0.0.19/autoxx/setup.py
--rw-r--r--   0        0        0     5352 2023-05-22 11:51:39.068804 autoxx-0.0.19/autoxx/tools/knowledge_base/utils.py
--rw-r--r--   0        0        0      929 2023-05-22 06:15:52.199109 autoxx-0.0.19/autoxx/tools/llm/utils.py
--rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.19/autoxx/tools/web_search/js/overlay.js
--rw-r--r--   0        0        0     6224 2023-05-23 02:55:50.078287 autoxx-0.0.19/autoxx/tools/web_search/search.py
--rw-r--r--   0        0        0      664 2023-05-23 04:09:00.385202 autoxx-0.0.19/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 autoxx-0.0.19/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.20/README.md
+-rw-r--r--   0        0        0     7194 2023-05-23 03:43:48.025037 autoxx-0.0.20/autoxx/agent/babyagi/agi.py
+-rw-r--r--   0        0        0     1109 2023-05-22 11:10:29.311248 autoxx-0.0.20/autoxx/agent/babyagi/task_manager.py
+-rw-r--r--   0        0        0    10193 2023-05-22 08:58:57.762888 autoxx-0.0.20/autoxx/agent/react/agent.py
+-rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.20/autoxx/requirements.txt
+-rw-r--r--   0        0        0      619 2023-05-23 00:34:07.217327 autoxx-0.0.20/autoxx/setup.py
+-rw-r--r--   0        0        0     5352 2023-05-22 11:51:39.068804 autoxx-0.0.20/autoxx/tools/knowledge_base/utils.py
+-rw-r--r--   0        0        0      929 2023-05-22 06:15:52.199109 autoxx-0.0.20/autoxx/tools/llm/utils.py
+-rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.20/autoxx/tools/web_search/js/overlay.js
+-rw-r--r--   0        0        0     6247 2023-05-23 05:10:30.480843 autoxx-0.0.20/autoxx/tools/web_search/search.py
+-rw-r--r--   0        0        0      664 2023-05-23 05:10:40.050949 autoxx-0.0.20/pyproject.toml
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 autoxx-0.0.20/PKG-INFO
```

### Comparing `autoxx-0.0.19/autoxx/agent/babyagi/agi.py` & `autoxx-0.0.20/autoxx/agent/babyagi/agi.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.19/autoxx/agent/babyagi/task_manager.py` & `autoxx-0.0.20/autoxx/agent/babyagi/task_manager.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.19/autoxx/agent/react/agent.py` & `autoxx-0.0.20/autoxx/agent/react/agent.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.19/autoxx/setup.py` & `autoxx-0.0.20/autoxx/setup.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.19/autoxx/tools/knowledge_base/utils.py` & `autoxx-0.0.20/autoxx/tools/knowledge_base/utils.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.19/autoxx/tools/llm/utils.py` & `autoxx-0.0.20/autoxx/tools/llm/utils.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.19/autoxx/tools/web_search/js/overlay.js` & `autoxx-0.0.20/autoxx/tools/web_search/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.19/autoxx/tools/web_search/search.py` & `autoxx-0.0.20/autoxx/tools/web_search/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from autogpt.commands.web_selenium import scrape_text_with_selenium
 from selenium.webdriver.remote.webdriver import WebDriver
 from autogpt import token_counter
 from autogpt.llm_utils import create_chat_completion
 from autogpt.processing.text import split_text
 
 FILE_DIR = Path(__file__).parent
-CFG = Config()
 
 def create_message(chunk: str, question: str) -> Dict[str, str]:
     """Create a message for the chat completion
 
     Args:
         chunk (str): The chunk of text to summarize
         question (str): The question to answer
@@ -49,14 +48,15 @@
     Args:
         chunks (list[str]): The chunks to summarize
         question (str): The question to answer
 
     Returns:
         str: The summary of the chunks
     """
+    CFG = Config()
     model = CFG.fast_llm_model
     text_length = len(text)
     print(f"Text length: {text_length} characters")
 
     chunks = list(
         split_text(text=text, max_length=CFG.browse_chunk_max_length, question=question)
     )
@@ -153,14 +153,15 @@
     Returns:
         str: The results of the search.
     """
 
     from googleapiclient.discovery import build
     from googleapiclient.errors import HttpError
 
+    CFG = Config()
     search_summaries = []
     try:
         # Get the Google API key and Custom Search Engine ID from the config file
         api_key = CFG.google_api_key
         custom_search_engine_id = CFG.custom_search_engine_id
 
         # Initialize the Custom Search API service
```

### Comparing `autoxx-0.0.19/pyproject.toml` & `autoxx-0.0.20/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.19"
+version = "0.0.20"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `autoxx-0.0.19/PKG-INFO` & `autoxx-0.0.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.19
+Version: 0.0.20
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

