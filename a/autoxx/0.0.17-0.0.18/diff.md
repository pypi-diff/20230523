# Comparing `tmp/autoxx-0.0.17.tar.gz` & `tmp/autoxx-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.17.tar", max compression
+gzip compressed data, was "autoxx-0.0.18.tar", max compression
```

## Comparing `autoxx-0.0.17.tar` & `autoxx-0.0.18.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.17/README.md
--rw-r--r--   0        0        0    10410 2023-05-22 14:38:11.995184 autoxx-0.0.17/autoxx/agent/babyagi/agi.py
--rw-r--r--   0        0        0     1109 2023-05-22 11:10:29.311248 autoxx-0.0.17/autoxx/agent/babyagi/task_manager.py
--rw-r--r--   0        0        0    10193 2023-05-22 08:58:57.762888 autoxx-0.0.17/autoxx/agent/react/agent.py
--rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.17/autoxx/requirements.txt
--rw-r--r--   0        0        0      619 2023-05-23 00:34:07.217327 autoxx-0.0.17/autoxx/setup.py
--rw-r--r--   0        0        0     5352 2023-05-22 11:51:39.068804 autoxx-0.0.17/autoxx/tools/knowledge_base/utils.py
--rw-r--r--   0        0        0      929 2023-05-22 06:15:52.199109 autoxx-0.0.17/autoxx/tools/llm/utils.py
--rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.17/autoxx/tools/web_search/js/overlay.js
--rw-r--r--   0        0        0     6326 2023-05-23 00:36:56.019874 autoxx-0.0.17/autoxx/tools/web_search/search.py
--rw-r--r--   0        0        0      664 2023-05-23 00:32:35.825311 autoxx-0.0.17/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 autoxx-0.0.17/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.18/README.md
+-rw-r--r--   0        0        0     7150 2023-05-23 01:56:40.555520 autoxx-0.0.18/autoxx/agent/babyagi/agi.py
+-rw-r--r--   0        0        0     1109 2023-05-22 11:10:29.311248 autoxx-0.0.18/autoxx/agent/babyagi/task_manager.py
+-rw-r--r--   0        0        0    10193 2023-05-22 08:58:57.762888 autoxx-0.0.18/autoxx/agent/react/agent.py
+-rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.18/autoxx/requirements.txt
+-rw-r--r--   0        0        0      619 2023-05-23 00:34:07.217327 autoxx-0.0.18/autoxx/setup.py
+-rw-r--r--   0        0        0     5352 2023-05-22 11:51:39.068804 autoxx-0.0.18/autoxx/tools/knowledge_base/utils.py
+-rw-r--r--   0        0        0      929 2023-05-22 06:15:52.199109 autoxx-0.0.18/autoxx/tools/llm/utils.py
+-rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.18/autoxx/tools/web_search/js/overlay.js
+-rw-r--r--   0        0        0     6326 2023-05-23 00:36:56.019874 autoxx-0.0.18/autoxx/tools/web_search/search.py
+-rw-r--r--   0        0        0      664 2023-05-23 02:30:58.978735 autoxx-0.0.18/pyproject.toml
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 autoxx-0.0.18/PKG-INFO
```

### Comparing `autoxx-0.0.17/autoxx/agent/babyagi/agi.py` & `autoxx-0.0.18/autoxx/agent/babyagi/agi.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,15 +34,16 @@
             f"You are a task management AI tasked with creating tasks for the following objective: {objective}.\n"
             f"Create new tasks based on the following plan delimited by triple backtick if necessary for the objective. Limit tasks types to those that can be completed with the available tools listed below. Task description should be detailed. "
             f"Your task: decelop a task list .\n"
             f"The current tool option is [web-search, text-completion] only. What each tool does is as follows:\n"
             f"web-search: It supports searching for information from the Internet. Interaction with web pages is not supported. For tasks using [web-search], provide the search query, and only the search query to use (eg. not 'research waterproof shoes, but 'waterproof shoes').\n"
             f"text-completion: It can be used for text extraction, summarization, copywrite, translation, etc., and it can also be used for LLM-based QA.\n"
             f"Make sure all task IDs are in chronological order.\n"
-            f"For efficiency, let's think step by step and create the tasks (up to 3 tasks) that are most critical to objective.\n"
+            f"For efficiency, let's think step by step and create the tasks (up to 5 tasks) that are most critical to objective. "
+            f"The last task is always to provide a final answer for customer.\n"
             f"The task list output format is as follows: "
             "[{\"id\": 1, \"task\": \"Untapped Capital\", \"tool\": \"web-search\", \"dependent_task_ids\": [], \"status\": \"incomplete\", \"result\": null, \"result_summary\": null}, {\"id\": 2, \"task\": \"Consider additional insights that can be reasoned from the results of...\", \"tool\": \"text-completion\", \"dependent_task_ids\": [1], \"status\": \"incomplete\", \"result\": null, \"result_summary\": null}].\n"
             f"Ensure the output can be parsed by Python json.loads.\n task list="
         )
 
         messages = create_message(prompt)
         response = create_chat_completion(
@@ -54,54 +55,14 @@
         task_list = []
         for new_task in new_tasks:
             task_id_counter += 1
             new_task.update({"id": task_id_counter})
             task_list.append(new_task)
         return task_list
 
-    def orchestrate_task(self, last_task: Dict) -> List[Dict]:
-        original_task_list = self.task_list.copy()
-        minified_task_list = [{k: v for k, v in task.items() if k != "result"} for task in self.task_list]
-        result = last_task['result'][0:4000] #come up with better solution later.
-        
-        prompt = (
-            f"You are a QA AI assistant tasked with cleaning the formatting of and reprioritizing the following tasks delimited by triple backtick:\n```{minified_task_list}```\n"
-            f"the last completed task (task id = {last_task['id']}, tool = {last_task['tool']}) has the following result delimited by triple backtick:\n```{last_task['result']}```\n\n"
-            f"Your task: Consider the ultimate objective of your team is to answer the question {self.objective} and reflect on the result of task that has been complted, re-create the task list (up to 5 tasks) to answer the question.\n" 
-            f"The current tool option is [web-search, text-completion] only. What each tool does is as follows:\n"
-            f"web-search: It supports searching for information from the Internet. Interaction with web pages is not supported. For tasks using [web-search], provide the search query, and only the search query to use (eg. not 'research waterproof shoes, but 'waterproof shoes').\n"
-            f"text-completion: It can be used for text extraction, summarization, copywrite, translation, etc., and it can also be used for LLM-based QA.\n"
-            f"dependent_task_ids should always be an empty array, or an array of numbers representing the task ID it should pull results from."
-            f"Make sure all task IDs are in chronological order.\n"
-            f"Do not remove the completed tasks.\n"
-            f"The last task is always to provide a final answer for customer.\n"
-            f"The task list output format is as follows: "
-            "[{\"id\": 1, \"task\": \"Untapped Capital\", \"tool\": \"web-search\", \"dependent_task_ids\": [], \"status\": \"incomplete\", \"result\": null, \"result_summary\": null}, {\"id\": 2, \"task\": \"Consider additional insights that can be reasoned from the results of...\", \"tool\": \"text-completion\", \"dependent_task_ids\": [1], \"status\": \"incomplete\", \"result\": null, \"result_summary\": null}].\n"
-            f"Ensure the output can be parsed by Python json.loads.\n task list="
-        )
-
-        messages = create_message(prompt)
-        result = create_chat_completion(
-            model=Config().smart_llm_model,
-            messages=messages,
-        )
-
-        try:
-            tmp_task_list = json.loads(result)
-        except Exception as error:
-            print(f"fail to decode ({error}): {result}")
-            return original_task_list
-        # Add the 'result' field back in
-
-        for updated_task, original_task in zip(tmp_task_list, original_task_list):
-            if "result" in original_task:
-                updated_task["result"] = original_task["result"]
-
-        return tmp_task_list
-
     ### Agent functions ##############################
     def execute_task(self, task: Dict) -> Dict:
         # Check if dependent_task_id is completed
         dependent_task_ids = []
         dependent_task_prompt = ""
         if task["dependent_task_ids"]:
             if isinstance(task["dependent_task_ids"], list):
@@ -163,16 +124,13 @@
                     completed_task = self.execute_task(task)
                     logging.info(f"\033[93m\033[1m TASK RESULT({self.objective}) \033[0m\033[0m {completed_task['result']}")
                 except Exception as e:  
                     logging.error(f"An error occurred while executing the task({self.objective}): {e.with_traceback()}")
                     self.status = "error"
                     self.error_message = str(e)  
                     return str(e)
-                if len(self.task_list) - len(incomplete_tasks) + 1 < self.max_tasks_count or len(incomplete_tasks) > 1:
-                    logging.info(f"\033[90m\033[3m" + "\nOrchestrate_task list({self.objective})...\n" + "\033[0m")
-                    self.task_list = self.orchestrate_task(completed_task)
 
             time.sleep(1)  # Sleep before checking the task list again
         self.status = "completed"
 
     def stat(self) -> Dict:
         return {"task_list": self.task_list, "status": self.status, "error_message": self.error_message}
```

### Comparing `autoxx-0.0.17/autoxx/agent/babyagi/task_manager.py` & `autoxx-0.0.18/autoxx/agent/babyagi/task_manager.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.17/autoxx/agent/react/agent.py` & `autoxx-0.0.18/autoxx/agent/react/agent.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.17/autoxx/setup.py` & `autoxx-0.0.18/autoxx/setup.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.17/autoxx/tools/knowledge_base/utils.py` & `autoxx-0.0.18/autoxx/tools/knowledge_base/utils.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.17/autoxx/tools/llm/utils.py` & `autoxx-0.0.18/autoxx/tools/llm/utils.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.17/autoxx/tools/web_search/js/overlay.js` & `autoxx-0.0.18/autoxx/tools/web_search/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.17/autoxx/tools/web_search/search.py` & `autoxx-0.0.18/autoxx/tools/web_search/search.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.17/PKG-INFO` & `autoxx-0.0.18/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.17
+Version: 0.0.18
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

