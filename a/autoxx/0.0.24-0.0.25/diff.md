# Comparing `tmp/autoxx-0.0.24.tar.gz` & `tmp/autoxx-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.24.tar", max compression
+gzip compressed data, was "autoxx-0.0.25.tar", max compression
```

## Comparing `autoxx-0.0.24.tar` & `autoxx-0.0.25.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.24/README.md
--rw-r--r--   0        0        0     7194 2023-05-23 06:11:19.762151 autoxx-0.0.24/autoxx/agent/babyagi/agi.py
--rw-r--r--   0        0        0     1109 2023-05-22 11:10:29.311248 autoxx-0.0.24/autoxx/agent/babyagi/task_manager.py
--rw-r--r--   0        0        0    10193 2023-05-22 08:58:57.762888 autoxx-0.0.24/autoxx/agent/react/agent.py
--rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.24/autoxx/requirements.txt
--rw-r--r--   0        0        0      801 2023-05-23 08:04:17.676812 autoxx-0.0.24/autoxx/setup.py
--rw-r--r--   0        0        0     5352 2023-05-22 11:51:39.068804 autoxx-0.0.24/autoxx/tools/knowledge_base/utils.py
--rw-r--r--   0        0        0      929 2023-05-22 06:15:52.199109 autoxx-0.0.24/autoxx/tools/llm/utils.py
--rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.24/autoxx/tools/web_search/js/overlay.js
--rw-r--r--   0        0        0     6481 2023-05-23 07:37:32.730417 autoxx-0.0.24/autoxx/tools/web_search/search.py
--rw-r--r--   0        0        0      664 2023-05-23 08:04:20.304710 autoxx-0.0.24/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 autoxx-0.0.24/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.25/README.md
+-rw-r--r--   0        0        0     7344 2023-05-23 10:04:32.651102 autoxx-0.0.25/autoxx/agent/babyagi/agi.py
+-rw-r--r--   0        0        0     1109 2023-05-22 11:10:29.311248 autoxx-0.0.25/autoxx/agent/babyagi/task_manager.py
+-rw-r--r--   0        0        0    10193 2023-05-22 08:58:57.762888 autoxx-0.0.25/autoxx/agent/react/agent.py
+-rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.25/autoxx/requirements.txt
+-rw-r--r--   0        0        0      801 2023-05-23 08:04:17.676812 autoxx-0.0.25/autoxx/setup.py
+-rw-r--r--   0        0        0     5352 2023-05-22 11:51:39.068804 autoxx-0.0.25/autoxx/tools/knowledge_base/utils.py
+-rw-r--r--   0        0        0      929 2023-05-22 06:15:52.199109 autoxx-0.0.25/autoxx/tools/llm/utils.py
+-rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.25/autoxx/tools/web_search/js/overlay.js
+-rw-r--r--   0        0        0     6473 2023-05-23 10:03:19.637350 autoxx-0.0.25/autoxx/tools/web_search/search.py
+-rw-r--r--   0        0        0      664 2023-05-23 10:05:40.511480 autoxx-0.0.25/pyproject.toml
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 autoxx-0.0.25/PKG-INFO
```

### Comparing `autoxx-0.0.24/autoxx/agent/babyagi/agi.py` & `autoxx-0.0.25/autoxx/agent/babyagi/agi.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
             f"Your task: decelop a task list .\n"
             f"The current tool option is [web-search, text-completion] only. What each tool does is as follows:\n"
             f"web-search: It supports searching for information from the Internet. Interaction with web pages is not supported. For tasks using [web-search], provide the search query, and only the search query to use (eg. not 'research waterproof shoes, but 'waterproof shoes').\n"
             f"text-completion: It can be used for text extraction, summarization, copywrite, translation, etc., and it can also be used for LLM-based QA.\n"
             f"Make sure all task IDs are in chronological order.\n"
             f"For efficiency, let's think step by step and create the tasks (up to 5 tasks) that are most critical to objective. "
             f"The last step is always to provide a final summary report including tasks executed and summary of knowledge acquired.\n"
+            f"Do not create any summarizing steps outside of the last step. And provide useful link in the summary report.\n"
             f"The task list output format is as follows: "
             "[{\"id\": 1, \"task\": \"Untapped Capital\", \"tool\": \"web-search\", \"dependent_task_ids\": [], \"status\": \"incomplete\", \"result\": null, \"result_summary\": null}, {\"id\": 2, \"task\": \"Consider additional insights that can be reasoned from the results of...\", \"tool\": \"text-completion\", \"dependent_task_ids\": [1], \"status\": \"incomplete\", \"result\": null, \"result_summary\": null}].\n"
             f"Ensure the output can be parsed by Python json.loads.\n task list="
         )
 
         messages = create_message(prompt)
         response = create_chat_completion(
@@ -75,17 +76,19 @@
                 if dependent_task and dependent_task["status"] != "completed":
                     return
                 elif dependent_task:
                     dependent_task_prompt += f"\ntask ({dependent_task['id']}. {dependent_task['task']}) result: {dependent_task['result']}"
 
         # Execute task
         
-        task_prompt = f"Complete your assigned task based on the objective: {self.objective}. Your task: {task['task']}"
+        task_prompt = (
+            f"Complete your assigned task based on the objective: {self.objective}. Your task: {task['task']}\n"
+        )
         if dependent_task_prompt != "":
-            task_prompt += f"\nThe previous tasks: {dependent_task_prompt}"
+            task_prompt += f"The previous tasks: {dependent_task_prompt}"
 
         task_prompt += "\nResponse:"
         if task["tool"] == "text-completion":
             result = llm_uils().text_completion(task_prompt)
             summary_result_prompt = f"Please summarize the following text:\n{result}\nSummary:"
             task["result_summary"] = llm_uils().text_completion(summary_result_prompt)
         elif task["tool"] == "web-search":
```

### Comparing `autoxx-0.0.24/autoxx/agent/babyagi/task_manager.py` & `autoxx-0.0.25/autoxx/agent/babyagi/task_manager.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.24/autoxx/agent/react/agent.py` & `autoxx-0.0.25/autoxx/agent/react/agent.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.24/autoxx/setup.py` & `autoxx-0.0.25/autoxx/setup.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.24/autoxx/tools/knowledge_base/utils.py` & `autoxx-0.0.25/autoxx/tools/knowledge_base/utils.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.24/autoxx/tools/llm/utils.py` & `autoxx-0.0.25/autoxx/tools/llm/utils.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.24/autoxx/tools/web_search/js/overlay.js` & `autoxx-0.0.25/autoxx/tools/web_search/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.24/autoxx/tools/web_search/search.py` & `autoxx-0.0.25/autoxx/tools/web_search/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,10 +199,10 @@
             raise f"Error: {e}"
 
     # Return the list of search result URLs
     for search_result in search_results:
         search_summaries.append({
             "relevant_content": search_result['snippet'],
             "title": search_result['title'],
-            "url": search_result['formattedUrl']
+            "url": search_result['link']
         })
     return search_summaries
```

### Comparing `autoxx-0.0.24/pyproject.toml` & `autoxx-0.0.25/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.24"
+version = "0.0.25"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `autoxx-0.0.24/PKG-INFO` & `autoxx-0.0.25/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.24
+Version: 0.0.25
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

