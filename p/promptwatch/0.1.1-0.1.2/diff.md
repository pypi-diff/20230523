# Comparing `tmp/promptwatch-0.1.1.tar.gz` & `tmp/promptwatch-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptwatch-0.1.1.tar", last modified: Fri May 19 13:00:54 2023, max compression
+gzip compressed data, was "promptwatch-0.1.2.tar", last modified: Tue May 23 20:28:37 2023, max compression
```

## Comparing `promptwatch-0.1.1.tar` & `promptwatch-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 13:00:54.453308 promptwatch-0.1.1/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-05-19 13:00:54.453150 promptwatch-0.1.1/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3584 2023-05-19 10:25:10.000000 promptwatch-0.1.1/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.1.1/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-05-19 13:00:54.453353 promptwatch-0.1.1/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-19 10:25:10.000000 promptwatch-0.1.1/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 13:00:54.448601 promptwatch-0.1.1/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 13:00:54.450230 promptwatch-0.1.1/src/promptwatch/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      317 2023-05-19 13:00:45.000000 promptwatch-0.1.1/src/promptwatch/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    11928 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5392 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/client.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/constants.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5469 2023-04-22 10:16:33.000000 promptwatch-0.1.1/src/promptwatch/data_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1605 2023-05-19 07:02:23.000000 promptwatch-0.1.1/src/promptwatch/decorators.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 13:00:54.452032 promptwatch-0.1.1/src/promptwatch/langchain/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      153 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/langchain/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    11067 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/langchain/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    25660 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/langchain/langchain_support.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4270 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/langchain/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    17876 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/promptwatch_context.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 13:00:54.452921 promptwatch-0.1.1/src/promptwatch/unit_tests/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/unit_tests/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13513 2023-05-19 12:57:26.000000 promptwatch-0.1.1/src/promptwatch/unit_tests/evaluation.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2261 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/unit_tests/schema.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13583 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/unit_tests/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1081 2023-05-02 21:26:09.000000 promptwatch-0.1.1/src/promptwatch/utils.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 13:00:54.451377 promptwatch-0.1.1/src/promptwatch.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-05-19 13:00:54.000000 promptwatch-0.1.1/src/promptwatch.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2023-05-19 13:00:54.000000 promptwatch-0.1.1/src/promptwatch.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-05-19 13:00:54.000000 promptwatch-0.1.1/src/promptwatch.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.1.1/src/promptwatch.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2023-05-19 13:00:54.000000 promptwatch-0.1.1/src/promptwatch.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-05-19 13:00:54.000000 promptwatch-0.1.1/src/promptwatch.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-23 20:28:37.686735 promptwatch-0.1.2/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-05-23 20:28:37.686568 promptwatch-0.1.2/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3584 2023-05-19 10:25:10.000000 promptwatch-0.1.2/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.1.2/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-05-23 20:28:37.686777 promptwatch-0.1.2/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-19 10:25:10.000000 promptwatch-0.1.2/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-23 20:28:37.677705 promptwatch-0.1.2/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-23 20:28:37.680992 promptwatch-0.1.2/src/promptwatch/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      317 2023-05-23 20:28:28.000000 promptwatch-0.1.2/src/promptwatch/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    11928 2023-05-19 10:25:10.000000 promptwatch-0.1.2/src/promptwatch/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5392 2023-05-19 10:25:10.000000 promptwatch-0.1.2/src/promptwatch/client.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-19 10:25:10.000000 promptwatch-0.1.2/src/promptwatch/constants.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5469 2023-04-22 10:16:33.000000 promptwatch-0.1.2/src/promptwatch/data_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1555 2023-05-23 20:20:02.000000 promptwatch-0.1.2/src/promptwatch/decorators.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-23 20:28:37.683983 promptwatch-0.1.2/src/promptwatch/langchain/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      153 2023-05-19 10:25:10.000000 promptwatch-0.1.2/src/promptwatch/langchain/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    11067 2023-05-19 10:25:10.000000 promptwatch-0.1.2/src/promptwatch/langchain/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    25666 2023-05-23 20:18:59.000000 promptwatch-0.1.2/src/promptwatch/langchain/langchain_support.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4270 2023-05-19 10:25:10.000000 promptwatch-0.1.2/src/promptwatch/langchain/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    17876 2023-05-19 10:25:10.000000 promptwatch-0.1.2/src/promptwatch/promptwatch_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-23 20:28:37.686353 promptwatch-0.1.2/src/promptwatch/unit_tests/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-19 10:25:10.000000 promptwatch-0.1.2/src/promptwatch/unit_tests/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13513 2023-05-20 12:19:55.000000 promptwatch-0.1.2/src/promptwatch/unit_tests/evaluation.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2261 2023-05-19 10:25:10.000000 promptwatch-0.1.2/src/promptwatch/unit_tests/schema.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13583 2023-05-19 10:25:10.000000 promptwatch-0.1.2/src/promptwatch/unit_tests/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1083 2023-05-23 19:47:43.000000 promptwatch-0.1.2/src/promptwatch/utils.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-23 20:28:37.682322 promptwatch-0.1.2/src/promptwatch.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-05-23 20:28:37.000000 promptwatch-0.1.2/src/promptwatch.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2023-05-23 20:28:37.000000 promptwatch-0.1.2/src/promptwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-05-23 20:28:37.000000 promptwatch-0.1.2/src/promptwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.1.2/src/promptwatch.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2023-05-23 20:28:37.000000 promptwatch-0.1.2/src/promptwatch.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-05-23 20:28:37.000000 promptwatch-0.1.2/src/promptwatch.egg-info/top_level.txt
```

### Comparing `promptwatch-0.1.1/PKG-INFO` & `promptwatch-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.1.1
+Version: 0.1.2
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.1.1/README.md` & `promptwatch-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.1/setup.py` & `promptwatch-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.1/src/promptwatch/caching.py` & `promptwatch-0.1.2/src/promptwatch/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.1/src/promptwatch/client.py` & `promptwatch-0.1.2/src/promptwatch/client.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.1/src/promptwatch/data_model.py` & `promptwatch-0.1.2/src/promptwatch/data_model.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.1/src/promptwatch/decorators.py` & `promptwatch-0.1.2/src/promptwatch/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             #skipping the first argument because it is self
             result = func(*args, **kwargs)
             pw = PromptWatch.get_active_instance()
             if pw is not None:
                 _self=args[0]
                 pw.add_context(FORMATTED_PROMPT_CONTEXT_KEY, result)
                 pw.add_context(TEMPLATE_NAME_CONTEXT_KEY, template_name)
-                if isinstance(pw.current_activity,ChainSequence) and pw.current_activity.sequence_type=="LLMChain":
+                if isinstance(pw.current_activity,ChainSequence):
                     llm_chain = find_the_caller_in_the_stack(type=LLMChain)
                     if llm_chain:
                         pw.add_context(LLM_CHAIN_CONTEXT_KEY, llm_chain)  
                         
 
                 
             return result
```

### Comparing `promptwatch-0.1.1/src/promptwatch/langchain/caching.py` & `promptwatch-0.1.2/src/promptwatch/langchain/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.1/src/promptwatch/langchain/langchain_support.py` & `promptwatch-0.1.2/src/promptwatch/langchain/langchain_support.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,26 +147,29 @@
         prompt_template = None
         prompt_input_values=None
         llm_info=None
         info_message=None
         formatted_prompt=None
 
         current_llm_chain:LLMChain= self.prompt_watch.get_context(LLM_CHAIN_CONTEXT_KEY)
+
+        template_name = self.prompt_watch.get_context(TEMPLATE_NAME_CONTEXT_KEY)
+        if template_name:
+            prompt_template = PromptWatch.prompt_template_register_cache.get(template_name)
+            
         # this should ensure that all the additional data is available in the context
         if current_llm_chain:
             if current_llm_chain.llm and current_llm_chain.llm.dict:
                 llm = current_llm_chain.llm
                 if hasattr(current_llm_chain.llm,"inner_llm"): # cachedLLM
                     llm = llm.inner_llm
                 llm_info = {k:v for k,v in llm.dict().items() if is_primitive_type(v)}
                 llm_info["stop"] = self.prompt_watch.current_activity.inputs.get("stop")
             # lets try to retrieve registered named template first... it's faster
-            template_name = self.prompt_watch.get_context(TEMPLATE_NAME_CONTEXT_KEY)
-            if template_name:
-                prompt_template = PromptWatch.prompt_template_register_cache.get(template_name)
+            
 
             if not prompt_template:
                 # lets create anonymous prompt template description
                 prompt_template = create_prompt_template_description(current_llm_chain.prompt)
 
             prompt_input_values = self.prompt_watch.current_activity.inputs
 
@@ -270,15 +273,15 @@
 
     
     def on_chain_start(
         self, serialized: Dict[str, Any], inputs: Dict[str, Any], **kwargs: Any
     ) -> Any:
         """Run when chain starts running."""
         
-        if serialized.get("name").startswith("LLM") :
+        if "LLM" in serialized.get("name") :
             current_llm_chain = find_the_caller_in_the_stack(serialized["name"])
             self.prompt_watch.add_context(LLM_CHAIN_CONTEXT_KEY,current_llm_chain)
 
         self.try_get_retrieved_documents(inputs)
```

### Comparing `promptwatch-0.1.1/src/promptwatch/langchain/unit_tests.py` & `promptwatch-0.1.2/src/promptwatch/langchain/unit_tests.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.1/src/promptwatch/promptwatch_context.py` & `promptwatch-0.1.2/src/promptwatch/promptwatch_context.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.1/src/promptwatch/unit_tests/evaluation.py` & `promptwatch-0.1.2/src/promptwatch/unit_tests/evaluation.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.1/src/promptwatch/unit_tests/schema.py` & `promptwatch-0.1.2/src/promptwatch/unit_tests/schema.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.1/src/promptwatch/unit_tests/unit_tests.py` & `promptwatch-0.1.2/src/promptwatch/unit_tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.1/src/promptwatch/utils.py` & `promptwatch-0.1.2/src/promptwatch/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import types
 def find_the_caller_in_the_stack(name:str=None, type:type = None):
         caller_frame = inspect.currentframe().f_back
         while caller_frame:
             caller_locals = caller_frame.f_locals
             caller_instance = caller_locals.get("self", None)
 
-            if name==caller_instance.__class__.__name__ or type==caller_instance.__class__:
+            if name==caller_instance.__class__.__name__ or isinstance(caller_instance, type):
                 return caller_instance
             caller_frame = caller_frame.f_back
 
 
 def is_primitive_type(val):
     return val.__class__.__module__=="builtins" and not type(val) is type and not type(val) is dict
```

### Comparing `promptwatch-0.1.1/src/promptwatch.egg-info/PKG-INFO` & `promptwatch-0.1.2/src/promptwatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.1.1
+Version: 0.1.2
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.1.1/src/promptwatch.egg-info/SOURCES.txt` & `promptwatch-0.1.2/src/promptwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

