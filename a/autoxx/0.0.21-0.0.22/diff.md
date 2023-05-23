# Comparing `tmp/autoxx-0.0.21.tar.gz` & `tmp/autoxx-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.21.tar", max compression
+gzip compressed data, was "autoxx-0.0.22.tar", max compression
```

## Comparing `autoxx-0.0.21.tar` & `autoxx-0.0.22.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.21/README.md
--rw-r--r--   0        0        0     7194 2023-05-23 03:43:48.025037 autoxx-0.0.21/autoxx/agent/babyagi/agi.py
--rw-r--r--   0        0        0     1109 2023-05-22 11:10:29.311248 autoxx-0.0.21/autoxx/agent/babyagi/task_manager.py
--rw-r--r--   0        0        0    10193 2023-05-22 08:58:57.762888 autoxx-0.0.21/autoxx/agent/react/agent.py
--rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.21/autoxx/requirements.txt
--rw-r--r--   0        0        0      800 2023-05-23 05:45:02.494638 autoxx-0.0.21/autoxx/setup.py
--rw-r--r--   0        0        0     5352 2023-05-22 11:51:39.068804 autoxx-0.0.21/autoxx/tools/knowledge_base/utils.py
--rw-r--r--   0        0        0      929 2023-05-22 06:15:52.199109 autoxx-0.0.21/autoxx/tools/llm/utils.py
--rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.21/autoxx/tools/web_search/js/overlay.js
--rw-r--r--   0        0        0     6247 2023-05-23 05:10:30.480843 autoxx-0.0.21/autoxx/tools/web_search/search.py
--rw-r--r--   0        0        0      664 2023-05-23 05:45:08.540299 autoxx-0.0.21/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 autoxx-0.0.21/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.22/README.md
+-rw-r--r--   0        0        0     7194 2023-05-23 06:11:19.762151 autoxx-0.0.22/autoxx/agent/babyagi/agi.py
+-rw-r--r--   0        0        0     1109 2023-05-22 11:10:29.311248 autoxx-0.0.22/autoxx/agent/babyagi/task_manager.py
+-rw-r--r--   0        0        0    10193 2023-05-22 08:58:57.762888 autoxx-0.0.22/autoxx/agent/react/agent.py
+-rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.22/autoxx/requirements.txt
+-rw-r--r--   0        0        0      803 2023-05-23 07:38:57.371927 autoxx-0.0.22/autoxx/setup.py
+-rw-r--r--   0        0        0     5352 2023-05-22 11:51:39.068804 autoxx-0.0.22/autoxx/tools/knowledge_base/utils.py
+-rw-r--r--   0        0        0      929 2023-05-22 06:15:52.199109 autoxx-0.0.22/autoxx/tools/llm/utils.py
+-rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.22/autoxx/tools/web_search/js/overlay.js
+-rw-r--r--   0        0        0     6481 2023-05-23 07:37:32.730417 autoxx-0.0.22/autoxx/tools/web_search/search.py
+-rw-r--r--   0        0        0      664 2023-05-23 07:39:22.006297 autoxx-0.0.22/pyproject.toml
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 autoxx-0.0.22/PKG-INFO
```

### Comparing `autoxx-0.0.21/autoxx/agent/babyagi/agi.py` & `autoxx-0.0.22/autoxx/agent/babyagi/agi.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.21/autoxx/agent/babyagi/task_manager.py` & `autoxx-0.0.22/autoxx/agent/babyagi/task_manager.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.21/autoxx/agent/react/agent.py` & `autoxx-0.0.22/autoxx/agent/react/agent.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.21/autoxx/setup.py` & `autoxx-0.0.22/autoxx/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import openai
+
+\import openai
 import os
 from autogpt.config import Config
 from typing import Optional
 
 def setup_config(
         azure_config_file:Optional[str] = "",
         debug:bool = False,
@@ -18,8 +19,8 @@
         CFG.set_google_api_key(os.getenv("GOOGLE_API_KEY", ""))
         CFG.set_custom_search_engine_id(os.getenv("CUSTOM_SEARCH_ENGINE_ID", ""))
 
     openai.api_type = CFG.openai_api_type
     openai.api_base = CFG.openai_api_base
     openai.api_version = CFG.openai_api_version
     openai.api_key = CFG.openai_api_key
-    return CFG
+    return CFG
```

### Comparing `autoxx-0.0.21/autoxx/tools/knowledge_base/utils.py` & `autoxx-0.0.22/autoxx/tools/knowledge_base/utils.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.21/autoxx/tools/llm/utils.py` & `autoxx-0.0.22/autoxx/tools/llm/utils.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.21/autoxx/tools/web_search/js/overlay.js` & `autoxx-0.0.22/autoxx/tools/web_search/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.21/autoxx/tools/web_search/search.py` & `autoxx-0.0.22/autoxx/tools/web_search/search.py`

 * *Files 8% similar despite different names*

```diff
@@ -121,33 +121,41 @@
     """
     driver, text = scrape_text_with_selenium(url=url)
     add_header(driver)
     summaries = summarize_chunks(text=text, question=question, url=url, driver=driver)
     close_browser(driver)
     return '\n'.join(summaries)
 
-def web_search(question:str, search_num:Optional[int]=2) -> List[Dict]:
-    search_result = google_official_search(query=question, num_results=search_num)
+def web_search(question:str, search_num:Optional[int]=3) -> List[Dict]:
+    search_result = google_official_search(query=question, num_results=search_num+3)
     search_summaries = []
 
+    index = 0
     for res in search_result:
         print(f"{res['title']} x {res['url']}\n")
-        summary = browse_website(url=res['url'], question=question)
+        try:
+            summary = browse_website(url=res['url'], question=question)
+        except Exception as e:
+            print(f"Error browsing websit {res['title']} x {res['url']}: {e}")
+            continue
 
         search_summaries.append({
             "relevant_content": summary,
             "title": res['title'],
             "url": res['url']
         })
 
         print(f"{res['title']} x {res['url']} summary: {summary}\n")
+        index += 1
+        if index >= search_num:
+            break
 
     return search_summaries
 
-def google_official_search(query: str, num_results: int = 2) -> List[Dict]:
+def google_official_search(query: str, num_results: int = 8) -> List[Dict]:
     """Return the results of a Google search using the official Google API
 
     Args:
         query (str): The search query.
         num_results (int): The number of results to return.
 
     Returns:
@@ -193,8 +201,8 @@
     # Return the list of search result URLs
     for search_result in search_results:
         search_summaries.append({
             "relevant_content": search_result['snippet'],
             "title": search_result['title'],
             "url": search_result['formattedUrl']
         })
-    return search_summaries
+    return search_summaries
```

### Comparing `autoxx-0.0.21/pyproject.toml` & `autoxx-0.0.22/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.21"
+version = "0.0.22"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `autoxx-0.0.21/PKG-INFO` & `autoxx-0.0.22/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.21
+Version: 0.0.22
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

