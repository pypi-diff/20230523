# Comparing `tmp/agixt-1.1.67b0.tar.gz` & `tmp/agixt-1.1.68b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.67b0.tar", last modified: Tue May 23 00:49:32 2023, max compression
+gzip compressed data, was "agixt-1.1.68b0.tar", last modified: Tue May 23 21:03:06 2023, max compression
```

## Comparing `agixt-1.1.67b0.tar` & `agixt-1.1.68b0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:49:32.870091 agixt-1.1.67b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-23 00:49:17.000000 agixt-1.1.67b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-23 00:49:17.000000 agixt-1.1.67b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-23 00:49:32.870091 agixt-1.1.67b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:49:32.866091 agixt-1.1.67b0/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/AGiXT.py
--rw-r--r--   0 runner    (1001) docker     (123)    14049 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/Commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/CustomPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/Main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/Tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:49:32.870091 agixt-1.1.67b0/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:49:32.870091 agixt-1.1.67b0/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-23 00:49:32.000000 agixt-1.1.67b0/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-23 00:49:32.000000 agixt-1.1.67b0/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 00:49:32.000000 agixt-1.1.67b0/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-23 00:49:32.000000 agixt-1.1.67b0/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 00:49:32.000000 agixt-1.1.67b0/agixt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:49:32.870091 agixt-1.1.67b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-23 00:49:17.000000 agixt-1.1.67b0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-23 00:49:17.000000 agixt-1.1.67b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 00:49:32.870091 agixt-1.1.67b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-23 00:49:17.000000 agixt-1.1.67b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:03:06.919393 agixt-1.1.68b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-23 21:02:55.000000 agixt-1.1.68b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-23 21:02:55.000000 agixt-1.1.68b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-23 21:03:06.919393 agixt-1.1.68b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:03:06.919393 agixt-1.1.68b0/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    16622 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/AGiXT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14049 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/Commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/CustomPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/Main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/Tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:03:06.919393 agixt-1.1.68b0/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/provider/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/provider/llamacppapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 21:02:55.000000 agixt-1.1.68b0/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:03:06.919393 agixt-1.1.68b0/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-23 21:03:06.000000 agixt-1.1.68b0/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-23 21:03:06.000000 agixt-1.1.68b0/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:03:06.000000 agixt-1.1.68b0/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-23 21:03:06.000000 agixt-1.1.68b0/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 21:03:06.000000 agixt-1.1.68b0/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:03:06.919393 agixt-1.1.68b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-23 21:02:55.000000 agixt-1.1.68b0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-23 21:02:55.000000 agixt-1.1.68b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 21:03:06.919393 agixt-1.1.68b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-23 21:02:55.000000 agixt-1.1.68b0/setup.py
```

### Comparing `agixt-1.1.67b0/LICENSE` & `agixt-1.1.68b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/PKG-INFO` & `agixt-1.1.68b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.67b0
+Version: 1.1.68b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.67b0/agixt/AGiXT.py` & `agixt-1.1.68b0/agixt/AGiXT.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import re
 import asyncio
 import regex
 import json
+import time
 from datetime import datetime
 from Agent import Agent
 from CustomPrompt import CustomPrompt
 from duckduckgo_search import ddg
 from urllib.parse import urlparse
 
 
 class AGiXT:
     def __init__(self, agent_name: str = "AGiXT"):
         self.agent_name = agent_name
         self.agent = Agent(self.agent_name)
         self.stop_running_event = None
         self.browsed_links = []
+        self.failures = 0
 
     def custom_format(self, string, **kwargs):
         if isinstance(string, list):
             string = "".join(str(x) for x in string)
 
         def replace(match):
             key = match.group(1)
@@ -95,19 +97,27 @@
                 loop.run_until_complete(
                     self.websearch_agent(task=task, depth=websearch_depth)
                 )
             else:
                 self.websearch_agent(task=task, depth=websearch_depth)
         try:
             self.response = self.agent.instruct(formatted_prompt, tokens=tokens)
-        except:
+        except Exception as e:
+            print(f"Error: {e}")
+            print(f"PROMPT CONTENT: {formatted_prompt}")
+            print(f"TOKENS: {tokens}")
+            self.failures += 1
+            if self.failures == 5:
+                self.failures == 0
+                print("Failed to get a response 5 times in a row.")
+                return None
+            print(f"Retrying in 10 seconds...")
+            time.sleep(10)
             if context_results > 0:
                 context_results = context_results - 1
-            if context_results == 0:
-                print("Warning: No context injected due to max tokens.")
             return self.run(
                 task=task,
                 prompt=prompt,
                 context_results=context_results,
                 async_exec=async_exec,
                 **kwargs,
             )
```

### Comparing `agixt-1.1.67b0/agixt/Agent.py` & `agixt-1.1.68b0/agixt/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/Chain.py` & `agixt-1.1.68b0/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/Commands.py` & `agixt-1.1.68b0/agixt/Commands.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/Config.py` & `agixt-1.1.68b0/agixt/Config.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/CustomPrompt.py` & `agixt-1.1.68b0/agixt/CustomPrompt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/Embedding.py` & `agixt-1.1.68b0/agixt/Embedding.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,29 @@
         ).json()
 
         if "predictions" in response:
             return response["predictions"]
         return {}
 
 
+class LlamacppEmbeddingFunction(EmbeddingFunction):
+    def __init__(self, api_host: str):
+        self._api_host = api_host
+        self._session = requests.Session()
+
+    def __call__(self, texts: Documents) -> Embeddings:
+        response = self._session.post(
+            self._api_url, json={"content": texts, "threads": 5}
+        ).json()
+        if "data" in response:
+            if "embedding" in response["data"]:
+                return response["data"]["embedding"]
+        return {}
+
+
 class AzureEmbeddingFunction(EmbeddingFunction):
     def __init__(
         self,
         api_key: str,
         model_name: str = "text-embedding-ada-002",
         deployment_id: str = "",
         AZURE_OPENAI_ENDPOINT: str = "https://api.openai.com",
@@ -164,14 +179,21 @@
     def cohere(self):
         chunk_size = 500
         embed = embedding_functions.CohereEmbeddingFunction(
             api_key=self.AGENT_CONFIG["settings"]["COHERE_API_KEY"],
         )
         return embed, chunk_size
 
+    def llamacpp(self):
+        chunk_size = 250
+        embed = embedding_functions.LlamaCppEmbeddingFunction(
+            model_name=self.AGENT_CONFIG["settings"]["EMBEDDING_URI"],
+        )
+        return embed, chunk_size
+
 
 def get_embedding_providers():
     return [
         func
         for func, _ in inspect.getmembers(Embedding, predicate=inspect.isfunction)
         if not func.startswith("__")
     ]
```

### Comparing `agixt-1.1.67b0/agixt/Main.py` & `agixt-1.1.68b0/agixt/Main.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/Memories.py` & `agixt-1.1.68b0/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/Tasks.py` & `agixt-1.1.68b0/agixt/Tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from AGiXT import AGiXT
 import re
 import os
 import json
 import uuid
 import yaml
+import time
 from pathlib import Path
 from Agent import Agent
 from collections import deque
 from typing import List, Dict
 
 
 class Tasks:
@@ -124,15 +125,17 @@
         response = AGiXT(self.agent_name).run(
             task=self.primary_objective,
             prompt="task",
             result=result,
             task_description=task_description,
             tasks=task_list,
         )
-
+        if response == None:
+            time.sleep(5)
+            return self.task_agent(result, task_description, task_list)
         lines = response.split("\n") if "\n" in response else [response]
         new_tasks = []
         for line in lines:
             match = re.match(r"(\d+)\.\s+(.*)", line)
             if match:
                 task_id, task_name = match.groups()
                 new_tasks.append(
```

### Comparing `agixt-1.1.67b0/agixt/app.py` & `agixt-1.1.68b0/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/provider/__init__.py` & `agixt-1.1.68b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/provider/azure.py` & `agixt-1.1.68b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/provider/bing.py` & `agixt-1.1.68b0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/provider/chatgpt.py` & `agixt-1.1.68b0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/provider/claude.py` & `agixt-1.1.68b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/provider/fastchat.py` & `agixt-1.1.68b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/provider/gpt4all.py` & `agixt-1.1.68b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/provider/gpt4free.py` & `agixt-1.1.68b0/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/provider/gpugpt4all.py` & `agixt-1.1.68b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/provider/huggingchat.py` & `agixt-1.1.68b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/provider/kobold.py` & `agixt-1.1.68b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/provider/llamacpp.py` & `agixt-1.1.68b0/agixt/provider/llamacpp.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,46 +15,49 @@
         MODEL_PATH: str = "",
         MAX_TOKENS: int = 2000,
         AI_TEMPERATURE: float = 0.7,
         AI_MODEL: str = "default",
         GPU_LAYERS: int = 0,
         BATCH_SIZE: int = 512,
         THREADS: int = 0,
-        STOP_SEQUENCE: str = "\n",
-        **kwargs
+        STOP_SEQUENCE: str = "</s>",
+        **kwargs,
     ):
         self.requirements = ["llama-cpp-python"]
         self.AI_TEMPERATURE = AI_TEMPERATURE
         self.MAX_TOKENS = MAX_TOKENS
         self.AI_MODEL = AI_MODEL
         self.GPU_LAYERS = GPU_LAYERS
         self.BATCH_SIZE = BATCH_SIZE
         self.THREADS = THREADS if THREADS != 0 else None
         self.STOP_SEQUENCE = STOP_SEQUENCE
-
-        if MODEL_PATH:
+        self.MODEL_PATH = MODEL_PATH
+        if self.MODEL_PATH:
             try:
                 self.MAX_TOKENS = int(self.MAX_TOKENS)
             except:
                 self.MAX_TOKENS = 2000
 
-        if os.path.isfile(MODEL_PATH):
+    def instruct(self, prompt, tokens: int = 0):
+        max_tokens = int(self.MAX_TOKENS) - tokens
+        if max_tokens < 1:
+            max_tokens = int(self.MAX_TOKENS)
+        if os.path.isfile(self.MODEL_PATH):
             self.model = Llama(
-                model_path=MODEL_PATH,
-                n_ctx=(int(self.MAX_TOKENS) * 2),
+                model_path=self.MODEL_PATH,
                 n_gpu_layers=int(self.GPU_LAYERS),
                 n_threads=int(self.THREADS),
+                n_ctx=max_tokens,
             )
         else:
             print("Unable to find model path.")
-
-    def instruct(self, prompt, tokens: int = 0):
-        max_tokens = int(self.MAX_TOKENS) - tokens
-        if max_tokens < 1:
-            max_tokens = int(self.MAX_TOKENS)
-
-        return self.model(
+            return None
+        response = self.model(
             prompt,
-            max_tokens=max_tokens,
             stop=[self.STOP_SEQUENCE],
             temperature=float(self.AI_TEMPERATURE),
-        )["choices"][0]["text"]
+            echo=True,
+        )
+        data = response["choices"][0]["text"]
+        data = data.replace(prompt, "")
+        data = data.lstrip("\n")
+        return data
```

### Comparing `agixt-1.1.67b0/agixt/provider/oobabooga.py` & `agixt-1.1.68b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/provider/openai.py` & `agixt-1.1.68b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/provider/palm.py` & `agixt-1.1.68b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/provider/transformer.py` & `agixt-1.1.68b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt/requirements.txt` & `agixt-1.1.68b0/agixt/requirements.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/agixt.egg-info/PKG-INFO` & `agixt-1.1.68b0/agixt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.67b0
+Version: 1.1.68b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.67b0/agixt.egg-info/SOURCES.txt` & `agixt-1.1.68b0/agixt.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -30,12 +30,13 @@
 agixt/provider/fastchat.py
 agixt/provider/gpt4all.py
 agixt/provider/gpt4free.py
 agixt/provider/gpugpt4all.py
 agixt/provider/huggingchat.py
 agixt/provider/kobold.py
 agixt/provider/llamacpp.py
+agixt/provider/llamacppapi.py
 agixt/provider/oobabooga.py
 agixt/provider/openai.py
 agixt/provider/palm.py
 agixt/provider/transformer.py
 docs/README.md
```

### Comparing `agixt-1.1.67b0/agixt.egg-info/requires.txt` & `agixt-1.1.68b0/agixt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/docs/README.md` & `agixt-1.1.68b0/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.1.67b0/setup.py` & `agixt-1.1.68b0/setup.py`

 * *Files identical despite different names*

