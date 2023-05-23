# Comparing `tmp/autoxx-0.0.18.tar.gz` & `tmp/autoxx-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.18.tar", max compression
+gzip compressed data, was "autoxx-0.0.19.tar", max compression
```

## Comparing `autoxx-0.0.18.tar` & `autoxx-0.0.19.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.18/README.md
--rw-r--r--   0        0        0     7150 2023-05-23 01:56:40.555520 autoxx-0.0.18/autoxx/agent/babyagi/agi.py
--rw-r--r--   0        0        0     1109 2023-05-22 11:10:29.311248 autoxx-0.0.18/autoxx/agent/babyagi/task_manager.py
--rw-r--r--   0        0        0    10193 2023-05-22 08:58:57.762888 autoxx-0.0.18/autoxx/agent/react/agent.py
--rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.18/autoxx/requirements.txt
--rw-r--r--   0        0        0      619 2023-05-23 00:34:07.217327 autoxx-0.0.18/autoxx/setup.py
--rw-r--r--   0        0        0     5352 2023-05-22 11:51:39.068804 autoxx-0.0.18/autoxx/tools/knowledge_base/utils.py
--rw-r--r--   0        0        0      929 2023-05-22 06:15:52.199109 autoxx-0.0.18/autoxx/tools/llm/utils.py
--rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.18/autoxx/tools/web_search/js/overlay.js
--rw-r--r--   0        0        0     6326 2023-05-23 00:36:56.019874 autoxx-0.0.18/autoxx/tools/web_search/search.py
--rw-r--r--   0        0        0      664 2023-05-23 02:30:58.978735 autoxx-0.0.18/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 autoxx-0.0.18/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.19/README.md
+-rw-r--r--   0        0        0     7194 2023-05-23 03:43:48.025037 autoxx-0.0.19/autoxx/agent/babyagi/agi.py
+-rw-r--r--   0        0        0     1109 2023-05-22 11:10:29.311248 autoxx-0.0.19/autoxx/agent/babyagi/task_manager.py
+-rw-r--r--   0        0        0    10193 2023-05-22 08:58:57.762888 autoxx-0.0.19/autoxx/agent/react/agent.py
+-rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.19/autoxx/requirements.txt
+-rw-r--r--   0        0        0      619 2023-05-23 00:34:07.217327 autoxx-0.0.19/autoxx/setup.py
+-rw-r--r--   0        0        0     5352 2023-05-22 11:51:39.068804 autoxx-0.0.19/autoxx/tools/knowledge_base/utils.py
+-rw-r--r--   0        0        0      929 2023-05-22 06:15:52.199109 autoxx-0.0.19/autoxx/tools/llm/utils.py
+-rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.19/autoxx/tools/web_search/js/overlay.js
+-rw-r--r--   0        0        0     6224 2023-05-23 02:55:50.078287 autoxx-0.0.19/autoxx/tools/web_search/search.py
+-rw-r--r--   0        0        0      664 2023-05-23 04:09:00.385202 autoxx-0.0.19/pyproject.toml
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 autoxx-0.0.19/PKG-INFO
```

### Comparing `autoxx-0.0.18/autoxx/agent/babyagi/agi.py` & `autoxx-0.0.19/autoxx/agent/babyagi/agi.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             f"Create new tasks based on the following plan delimited by triple backtick if necessary for the objective. Limit tasks types to those that can be completed with the available tools listed below. Task description should be detailed. "
             f"Your task: decelop a task list .\n"
             f"The current tool option is [web-search, text-completion] only. What each tool does is as follows:\n"
             f"web-search: It supports searching for information from the Internet. Interaction with web pages is not supported. For tasks using [web-search], provide the search query, and only the search query to use (eg. not 'research waterproof shoes, but 'waterproof shoes').\n"
             f"text-completion: It can be used for text extraction, summarization, copywrite, translation, etc., and it can also be used for LLM-based QA.\n"
             f"Make sure all task IDs are in chronological order.\n"
             f"For efficiency, let's think step by step and create the tasks (up to 5 tasks) that are most critical to objective. "
-            f"The last task is always to provide a final answer for customer.\n"
+            f"The last step is always to provide a final summary report including tasks executed and summary of knowledge acquired.\n"
             f"The task list output format is as follows: "
             "[{\"id\": 1, \"task\": \"Untapped Capital\", \"tool\": \"web-search\", \"dependent_task_ids\": [], \"status\": \"incomplete\", \"result\": null, \"result_summary\": null}, {\"id\": 2, \"task\": \"Consider additional insights that can be reasoned from the results of...\", \"tool\": \"text-completion\", \"dependent_task_ids\": [1], \"status\": \"incomplete\", \"result\": null, \"result_summary\": null}].\n"
             f"Ensure the output can be parsed by Python json.loads.\n task list="
         )
 
         messages = create_message(prompt)
         response = create_chat_completion(
@@ -100,15 +100,15 @@
             result = "Unknown tool"
         
         # Update task status and result
         task["status"] = "completed"
         task["result"] = result
         return task
     
-    def execute(self) -> str:
+    def execute(self):
         self.status = "running"
         # Main loop
         while any(task["status"] == "incomplete" for task in self.task_list):
               # Filter out incomplete tasks
             incomplete_tasks = [task for task in self.task_list if task["status"] == "incomplete"]
             logging.info(f"\033[95m\033[1m INCOMPLETE TASK LIST({self.objective}) \033[0m\033[0m {[str(t['id'])+': '+t['task'] + '[' + t['tool'] + ']' for t in incomplete_tasks]}")
             if incomplete_tasks:
@@ -120,17 +120,17 @@
                 logging.info(f"\033[92m\033[1m NEXT TASK({self.objective}) \033[0m\033[0m {task['id']}:{task['task']}[{task['tool']}]")
 
                 # Execute task & call task manager from function
                 try:
                     completed_task = self.execute_task(task)
                     logging.info(f"\033[93m\033[1m TASK RESULT({self.objective}) \033[0m\033[0m {completed_task['result']}")
                 except Exception as e:  
-                    logging.error(f"An error occurred while executing the task({self.objective}): {e.with_traceback()}")
+                    logging.error(f"An error occurred while executing the task({self.objective}): {e.with_traceback(None)}")
                     self.status = "error"
                     self.error_message = str(e)  
-                    return str(e)
+                    return
 
             time.sleep(1)  # Sleep before checking the task list again
         self.status = "completed"
 
     def stat(self) -> Dict:
         return {"task_list": self.task_list, "status": self.status, "error_message": self.error_message}
```

### Comparing `autoxx-0.0.18/autoxx/agent/babyagi/task_manager.py` & `autoxx-0.0.19/autoxx/agent/babyagi/task_manager.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.18/autoxx/agent/react/agent.py` & `autoxx-0.0.19/autoxx/agent/react/agent.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.18/autoxx/setup.py` & `autoxx-0.0.19/autoxx/setup.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.18/autoxx/tools/knowledge_base/utils.py` & `autoxx-0.0.19/autoxx/tools/knowledge_base/utils.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.18/autoxx/tools/llm/utils.py` & `autoxx-0.0.19/autoxx/tools/llm/utils.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.18/autoxx/tools/web_search/js/overlay.js` & `autoxx-0.0.19/autoxx/tools/web_search/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.18/autoxx/tools/web_search/search.py` & `autoxx-0.0.19/autoxx/tools/web_search/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,17 +123,14 @@
     add_header(driver)
     summaries = summarize_chunks(text=text, question=question, url=url, driver=driver)
     close_browser(driver)
     return '\n'.join(summaries)
 
 def web_search(question:str, search_num:Optional[int]=2) -> List[Dict]:
     search_result = google_official_search(query=question, num_results=search_num)
-    if isinstance(search_result, str):
-        raise ValueError(f"google search error: {e}")
-
     search_summaries = []
 
     for res in search_result:
         print(f"{res['title']} x {res['url']}\n")
         summary = browse_website(url=res['url'], question=question)
 
         search_summaries.append({
@@ -142,15 +139,15 @@
             "url": res['url']
         })
 
         print(f"{res['title']} x {res['url']} summary: {summary}\n")
 
     return search_summaries
 
-def google_official_search(query: str, num_results: int = 2) -> str | List[Dict]:
+def google_official_search(query: str, num_results: int = 2) -> List[Dict]:
     """Return the results of a Google search using the official Google API
 
     Args:
         query (str): The search query.
         num_results (int): The number of results to return.
 
     Returns:
@@ -184,17 +181,17 @@
 
         # Check if the error is related to an invalid or missing API key
         if error_details.get("error", {}).get(
             "code"
         ) == 403 and "invalid API key" in error_details.get("error", {}).get(
             "message", ""
         ):
-            return "Error: The provided Google API key is invalid or missing."
+            raise "Error: The provided Google API key is invalid or missing."
         else:
-            return f"Error: {e}"
+            raise f"Error: {e}"
 
     # Return the list of search result URLs
     for search_result in search_results:
         search_summaries.append({
             "relevant_content": search_result['snippet'],
             "title": search_result['title'],
             "url": search_result['formattedUrl']
```

### Comparing `autoxx-0.0.18/pyproject.toml` & `autoxx-0.0.19/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.18"
+version = "0.0.19"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `autoxx-0.0.18/PKG-INFO` & `autoxx-0.0.19/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.18
+Version: 0.0.19
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

