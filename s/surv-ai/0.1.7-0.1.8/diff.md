# Comparing `tmp/surv_ai-0.1.7.tar.gz` & `tmp/surv_ai-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surv_ai-0.1.7.tar", max compression
+gzip compressed data, was "surv_ai-0.1.8.tar", max compression
```

## Comparing `surv_ai-0.1.7.tar` & `surv_ai-0.1.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1056 2023-05-19 03:25:36.438871 surv_ai-0.1.7/LICENSE
--rw-r--r--   0        0        0    21369 2023-05-23 13:32:11.427446 surv_ai-0.1.7/README.md
--rw-r--r--   0        0        0     1447 2023-05-23 13:32:23.220510 surv_ai-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1301 2023-05-22 19:00:12.464186 surv_ai-0.1.7/surv_ai/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 02:57:50.211881 surv_ai-0.1.7/surv_ai/core/__init__.py
--rw-r--r--   0        0        0     1667 2023-05-22 16:09:44.534005 surv_ai-0.1.7/surv_ai/core/agent.py
--rw-r--r--   0        0        0        0 2023-05-09 03:57:54.724106 surv_ai-0.1.7/surv_ai/core/agents/__init__.py
--rw-r--r--   0        0        0     1608 2023-05-22 15:04:42.549505 surv_ai-0.1.7/surv_ai/core/agents/binary.py
--rw-r--r--   0        0        0     6979 2023-05-22 15:18:19.376795 surv_ai-0.1.7/surv_ai/core/agents/reasoning.py
--rw-r--r--   0        0        0     1857 2023-05-22 19:00:12.464474 surv_ai-0.1.7/surv_ai/core/interfaces.py
--rw-r--r--   0        0        0     1279 2023-05-22 16:09:44.531688 surv_ai-0.1.7/surv_ai/core/model.py
--rw-r--r--   0        0        0     4723 2023-05-23 12:58:41.819687 surv_ai-0.1.7/surv_ai/core/survey.py
--rw-r--r--   0        0        0        0 2023-04-16 19:43:12.303158 surv_ai-0.1.7/surv_ai/lib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 03:24:33.757534 surv_ai-0.1.7/surv_ai/lib/conversation/__init__.py
--rw-r--r--   0        0        0     1065 2023-05-22 15:04:42.565319 surv_ai-0.1.7/surv_ai/lib/conversation/conversation.py
--rw-r--r--   0        0        0      409 2023-05-21 02:50:40.891526 surv_ai-0.1.7/surv_ai/lib/conversation/interfaces.py
--rw-r--r--   0        0        0       53 2023-05-08 03:25:52.022148 surv_ai-0.1.7/surv_ai/lib/knowledge_store/__init__.py
--rw-r--r--   0        0        0      693 2023-05-22 15:04:42.556450 surv_ai-0.1.7/surv_ai/lib/knowledge_store/interfaces.py
--rw-r--r--   0        0        0     1486 2023-05-22 15:04:42.581390 surv_ai-0.1.7/surv_ai/lib/knowledge_store/local.py
--rw-r--r--   0        0        0        0 2023-04-16 19:53:58.086455 surv_ai-0.1.7/surv_ai/lib/llm/__init__.py
--rw-r--r--   0        0        0     3755 2023-05-22 16:07:39.753305 surv_ai-0.1.7/surv_ai/lib/llm/anthropic.py
--rw-r--r--   0        0        0     4261 2023-05-22 16:07:57.537852 surv_ai-0.1.7/surv_ai/lib/llm/gpt.py
--rw-r--r--   0        0        0      432 2023-05-22 15:04:42.564655 surv_ai-0.1.7/surv_ai/lib/llm/interfaces.py
--rw-r--r--   0        0        0     2005 2023-05-23 04:29:11.574974 surv_ai-0.1.7/surv_ai/lib/log.py
--rw-r--r--   0        0        0        0 2023-04-16 23:16:14.406022 surv_ai-0.1.7/surv_ai/lib/tools/__init__.py
--rw-r--r--   0        0        0      656 2023-05-22 19:00:03.447356 surv_ai-0.1.7/surv_ai/lib/tools/interfaces.py
--rw-r--r--   0        0        0        0 2023-04-16 23:16:30.843990 surv_ai-0.1.7/surv_ai/lib/tools/query/__init__.py
--rw-r--r--   0        0        0     7047 2023-05-22 16:09:44.603986 surv_ai-0.1.7/surv_ai/lib/tools/query/google_custom_search.py
--rw-r--r--   0        0        0      219 2023-05-19 05:42:04.105413 surv_ai-0.1.7/surv_ai/lib/tools/query/interfaces.py
--rw-r--r--   0        0        0     5918 2023-05-22 16:09:44.606441 surv_ai-0.1.7/surv_ai/lib/tools/query/wikipedia.py
--rw-r--r--   0        0        0     2924 2023-05-22 19:00:12.464217 surv_ai-0.1.7/surv_ai/lib/tools/tool_belt.py
--rw-r--r--   0        0        0    22719 1970-01-01 00:00:00.000000 surv_ai-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-19 03:25:36.438871 surv_ai-0.1.8/LICENSE
+-rw-r--r--   0        0        0    21368 2023-05-23 14:20:46.224165 surv_ai-0.1.8/README.md
+-rw-r--r--   0        0        0     1447 2023-05-23 14:20:58.843859 surv_ai-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1301 2023-05-22 19:00:12.464186 surv_ai-0.1.8/surv_ai/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 02:57:50.211881 surv_ai-0.1.8/surv_ai/core/__init__.py
+-rw-r--r--   0        0        0     1667 2023-05-22 16:09:44.534005 surv_ai-0.1.8/surv_ai/core/agent.py
+-rw-r--r--   0        0        0        0 2023-05-09 03:57:54.724106 surv_ai-0.1.8/surv_ai/core/agents/__init__.py
+-rw-r--r--   0        0        0     1608 2023-05-22 15:04:42.549505 surv_ai-0.1.8/surv_ai/core/agents/binary.py
+-rw-r--r--   0        0        0     6979 2023-05-22 15:18:19.376795 surv_ai-0.1.8/surv_ai/core/agents/reasoning.py
+-rw-r--r--   0        0        0     1857 2023-05-22 19:00:12.464474 surv_ai-0.1.8/surv_ai/core/interfaces.py
+-rw-r--r--   0        0        0     1279 2023-05-22 16:09:44.531688 surv_ai-0.1.8/surv_ai/core/model.py
+-rw-r--r--   0        0        0     4722 2023-05-23 14:20:48.841757 surv_ai-0.1.8/surv_ai/core/survey.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:43:12.303158 surv_ai-0.1.8/surv_ai/lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 03:24:33.757534 surv_ai-0.1.8/surv_ai/lib/conversation/__init__.py
+-rw-r--r--   0        0        0     1065 2023-05-22 15:04:42.565319 surv_ai-0.1.8/surv_ai/lib/conversation/conversation.py
+-rw-r--r--   0        0        0      409 2023-05-21 02:50:40.891526 surv_ai-0.1.8/surv_ai/lib/conversation/interfaces.py
+-rw-r--r--   0        0        0       53 2023-05-08 03:25:52.022148 surv_ai-0.1.8/surv_ai/lib/knowledge_store/__init__.py
+-rw-r--r--   0        0        0      693 2023-05-22 15:04:42.556450 surv_ai-0.1.8/surv_ai/lib/knowledge_store/interfaces.py
+-rw-r--r--   0        0        0     1486 2023-05-22 15:04:42.581390 surv_ai-0.1.8/surv_ai/lib/knowledge_store/local.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:53:58.086455 surv_ai-0.1.8/surv_ai/lib/llm/__init__.py
+-rw-r--r--   0        0        0     3755 2023-05-22 16:07:39.753305 surv_ai-0.1.8/surv_ai/lib/llm/anthropic.py
+-rw-r--r--   0        0        0     4261 2023-05-22 16:07:57.537852 surv_ai-0.1.8/surv_ai/lib/llm/gpt.py
+-rw-r--r--   0        0        0      432 2023-05-22 15:04:42.564655 surv_ai-0.1.8/surv_ai/lib/llm/interfaces.py
+-rw-r--r--   0        0        0     2005 2023-05-23 04:29:11.574974 surv_ai-0.1.8/surv_ai/lib/log.py
+-rw-r--r--   0        0        0        0 2023-04-16 23:16:14.406022 surv_ai-0.1.8/surv_ai/lib/tools/__init__.py
+-rw-r--r--   0        0        0      656 2023-05-22 19:00:03.447356 surv_ai-0.1.8/surv_ai/lib/tools/interfaces.py
+-rw-r--r--   0        0        0        0 2023-04-16 23:16:30.843990 surv_ai-0.1.8/surv_ai/lib/tools/query/__init__.py
+-rw-r--r--   0        0        0     7047 2023-05-22 16:09:44.603986 surv_ai-0.1.8/surv_ai/lib/tools/query/google_custom_search.py
+-rw-r--r--   0        0        0      219 2023-05-19 05:42:04.105413 surv_ai-0.1.8/surv_ai/lib/tools/query/interfaces.py
+-rw-r--r--   0        0        0     5918 2023-05-22 16:09:44.606441 surv_ai-0.1.8/surv_ai/lib/tools/query/wikipedia.py
+-rw-r--r--   0        0        0     2924 2023-05-22 19:00:12.464217 surv_ai-0.1.8/surv_ai/lib/tools/tool_belt.py
+-rw-r--r--   0        0        0    22718 1970-01-01 00:00:00.000000 surv_ai-0.1.8/PKG-INFO
```

### Comparing `surv_ai-0.1.7/LICENSE` & `surv_ai-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.7/README.md` & `surv_ai-0.1.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 class Survey:
     def __init__(
         self,
         client: LargeLanguageModelClientInterface,
         tool_belt: ToolBeltInterface,
         n_agents=10,
         max_concurrency=10,
-        max_knowledge_per_agent=10,
+        max_knowledge_per_agent=3,
     ):
         ...
 
     async def conduct(self, hypothesis: str) -> SurveyResponse:
         ...
 ```
```

### Comparing `surv_ai-0.1.7/pyproject.toml` & `surv_ai-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "surv_ai"
-version = "0.1.7"
+version = "0.1.8"
 description = "A framework for multi-agent modeling using large language models"
 authors = ["Daniel Balsam <daniel.balsam@survai.org>"]
 license = "MIT"
 readme = "README.md"
 keywords=[
     "ai",
     "artificial intelligence",
```

### Comparing `surv_ai-0.1.7/surv_ai/__init__.py` & `surv_ai-0.1.8/surv_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.7/surv_ai/core/agent.py` & `surv_ai-0.1.8/surv_ai/core/agent.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.7/surv_ai/core/agents/binary.py` & `surv_ai-0.1.8/surv_ai/core/agents/binary.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.7/surv_ai/core/agents/reasoning.py` & `surv_ai-0.1.8/surv_ai/core/agents/reasoning.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.7/surv_ai/core/interfaces.py` & `surv_ai-0.1.8/surv_ai/core/interfaces.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.7/surv_ai/core/model.py` & `surv_ai-0.1.8/surv_ai/core/model.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.7/surv_ai/core/survey.py` & `surv_ai-0.1.8/surv_ai/core/survey.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 class Survey(SurveyInterface):
     def __init__(
         self,
         client: LargeLanguageModelClientInterface,
         tool_belt: ToolBeltInterface,
         n_agents=10,
         max_concurrency=10,
-        max_knowledge_per_agent=10,
+        max_knowledge_per_agent=3,
         base_knowledge: Optional[list[Knowledge]] = None,
     ):
         self.client = client
         self.tool_belt = tool_belt
 
         self.n_agents = n_agents
         self.max_concurrency = max_concurrency
```

### Comparing `surv_ai-0.1.7/surv_ai/lib/conversation/conversation.py` & `surv_ai-0.1.8/surv_ai/lib/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.7/surv_ai/lib/knowledge_store/interfaces.py` & `surv_ai-0.1.8/surv_ai/lib/knowledge_store/interfaces.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.7/surv_ai/lib/knowledge_store/local.py` & `surv_ai-0.1.8/surv_ai/lib/knowledge_store/local.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.7/surv_ai/lib/llm/anthropic.py` & `surv_ai-0.1.8/surv_ai/lib/llm/anthropic.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.7/surv_ai/lib/llm/gpt.py` & `surv_ai-0.1.8/surv_ai/lib/llm/gpt.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.7/surv_ai/lib/log.py` & `surv_ai-0.1.8/surv_ai/lib/log.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.7/surv_ai/lib/tools/interfaces.py` & `surv_ai-0.1.8/surv_ai/lib/tools/interfaces.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.7/surv_ai/lib/tools/query/google_custom_search.py` & `surv_ai-0.1.8/surv_ai/lib/tools/query/google_custom_search.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.7/surv_ai/lib/tools/query/wikipedia.py` & `surv_ai-0.1.8/surv_ai/lib/tools/query/wikipedia.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.7/surv_ai/lib/tools/tool_belt.py` & `surv_ai-0.1.8/surv_ai/lib/tools/tool_belt.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.7/PKG-INFO` & `surv_ai-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surv-ai
-Version: 0.1.7
+Version: 0.1.8
 Summary: A framework for multi-agent modeling using large language models
 Home-page: https://github.com/DanielBalsam/surv_ai
 License: MIT
 Keywords: ai,artificial intelligence,data science,statistics,models,llm,agents,survai,surv_ai,survey,multi-agent,large language model,artificial intelligence,machine learning,natural language processing,nlp,sentiment analysis
 Author: Daniel Balsam
 Author-email: daniel.balsam@survai.org
 Requires-Python: >=3.9,<4.0
@@ -84,15 +84,15 @@
 class Survey:
     def __init__(
         self,
         client: LargeLanguageModelClientInterface,
         tool_belt: ToolBeltInterface,
         n_agents=10,
         max_concurrency=10,
-        max_knowledge_per_agent=10,
+        max_knowledge_per_agent=3,
     ):
         ...
 
     async def conduct(self, hypothesis: str) -> SurveyResponse:
         ...
 ```
```

