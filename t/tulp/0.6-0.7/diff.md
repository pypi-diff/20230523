# Comparing `tmp/tulp-0.6.tar.gz` & `tmp/tulp-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulp-0.6.tar", last modified: Fri May 12 03:02:28 2023, max compression
+gzip compressed data, was "tulp-0.7.tar", last modified: Tue May 23 19:58:07 2023, max compression
```

## Comparing `tulp-0.6.tar` & `tulp-0.7.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-05-12 03:02:28.830553 tulp-0.6/
--rw-rw-r--   0 fede      (1000) fede      (1000)      684 2023-04-20 22:33:28.000000 tulp-0.6/LICENSE
--rw-rw-r--   0 fede      (1000) fede      (1000)     7906 2023-05-12 03:02:28.830553 tulp-0.6/PKG-INFO
--rw-rw-r--   0 fede      (1000) fede      (1000)     7313 2023-05-12 03:01:09.000000 tulp-0.6/README.md
--rw-rw-r--   0 fede      (1000) fede      (1000)      900 2023-05-12 03:02:28.830553 tulp-0.6/setup.cfg
--rw-rw-r--   0 fede      (1000) fede      (1000)       39 2023-04-20 22:33:28.000000 tulp-0.6/setup.py
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-05-12 03:02:28.810553 tulp-0.6/test/
--rw-rw-r--   0 fede      (1000) fede      (1000)     2680 2023-04-21 01:24:55.000000 tulp-0.6/test/test_filterMode_advanced.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     3621 2023-04-21 01:24:55.000000 tulp-0.6/test/test_filterMode_basic.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1342 2023-04-21 01:24:55.000000 tulp-0.6/test/test_requestMode.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1066 2023-04-21 01:24:55.000000 tulp-0.6/test/test_slowtest.py
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-05-12 03:02:28.822553 tulp-0.6/tulp/
--rw-rw-r--   0 fede      (1000) fede      (1000)      111 2023-04-20 22:33:28.000000 tulp-0.6/tulp/__init__.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     4940 2023-05-03 18:35:41.000000 tulp-0.6/tulp/filteringPrompt.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     4481 2023-04-24 02:39:45.000000 tulp-0.6/tulp/filteringPrompt.roto.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1230 2023-05-06 16:28:30.000000 tulp-0.6/tulp/newMain.2.py
--rw-rw-r--   0 fede      (1000) fede      (1000)      921 2023-05-06 19:31:01.000000 tulp-0.6/tulp/newMain.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     3841 2023-05-12 02:22:46.000000 tulp-0.6/tulp/programPrompt.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     3841 2023-05-12 02:22:14.000000 tulp-0.6/tulp/requestPrompt.py
--rw-rw-r--   0 fede      (1000) fede      (1000)    15468 2023-05-03 22:20:43.000000 tulp-0.6/tulp/text_splitter.py
--rw-rw-r--   0 fede      (1000) fede      (1000)    15468 2023-05-03 22:26:14.000000 tulp-0.6/tulp/text_splitter_org.py
--rwxrwxr-x   0 fede      (1000) fede      (1000)     9022 2023-05-12 02:42:29.000000 tulp-0.6/tulp/tulp.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1017 2023-05-06 20:21:58.000000 tulp-0.6/tulp/tulpargs.2.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1688 2023-05-12 02:40:01.000000 tulp-0.6/tulp/tulpargs.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1052 2023-05-06 20:28:06.000000 tulp-0.6/tulp/tulpconfig.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1722 2023-04-23 20:36:49.000000 tulp-0.6/tulp/tulplogger.py
--rw-rw-r--   0 fede      (1000) fede      (1000)       16 2023-05-12 02:07:52.000000 tulp-0.6/tulp/version.py
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-05-12 03:02:28.830553 tulp-0.6/tulp.egg-info/
--rw-rw-r--   0 fede      (1000) fede      (1000)     7906 2023-05-12 03:02:28.000000 tulp-0.6/tulp.egg-info/PKG-INFO
--rw-rw-r--   0 fede      (1000) fede      (1000)      638 2023-05-12 03:02:28.000000 tulp-0.6/tulp.egg-info/SOURCES.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)        1 2023-05-12 03:02:28.000000 tulp-0.6/tulp.egg-info/dependency_links.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)       39 2023-05-12 03:02:28.000000 tulp-0.6/tulp.egg-info/entry_points.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)       15 2023-05-12 03:02:28.000000 tulp-0.6/tulp.egg-info/requires.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)        5 2023-05-12 03:02:28.000000 tulp-0.6/tulp.egg-info/top_level.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)        1 2023-04-21 01:25:36.000000 tulp-0.6/tulp.egg-info/zip-safe
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-05-23 19:58:07.877287 tulp-0.7/
+-rw-rw-r--   0 fede      (1000) fede      (1000)      684 2023-04-20 22:33:28.000000 tulp-0.7/LICENSE
+-rw-rw-r--   0 fede      (1000) fede      (1000)     7906 2023-05-23 19:58:07.877287 tulp-0.7/PKG-INFO
+-rw-rw-r--   0 fede      (1000) fede      (1000)     7313 2023-05-12 03:01:09.000000 tulp-0.7/README.md
+-rw-rw-r--   0 fede      (1000) fede      (1000)      900 2023-05-23 19:58:07.877287 tulp-0.7/setup.cfg
+-rw-rw-r--   0 fede      (1000) fede      (1000)       39 2023-04-20 22:33:28.000000 tulp-0.7/setup.py
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-05-23 19:58:07.861287 tulp-0.7/test/
+-rw-rw-r--   0 fede      (1000) fede      (1000)     2680 2023-04-21 01:24:55.000000 tulp-0.7/test/test_filterMode_advanced.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3621 2023-04-21 01:24:55.000000 tulp-0.7/test/test_filterMode_basic.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1342 2023-04-21 01:24:55.000000 tulp-0.7/test/test_requestMode.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1066 2023-04-21 01:24:55.000000 tulp-0.7/test/test_slowtest.py
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-05-23 19:58:07.873287 tulp-0.7/tulp/
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1218 2023-05-12 18:00:03.000000 tulp-0.7/tulp/TulpOutputFileWriter.old.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1378 2023-05-23 19:57:51.000000 tulp-0.7/tulp/TulpOutputFileWriter.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)      111 2023-04-20 22:33:28.000000 tulp-0.7/tulp/__init__.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1864 2023-05-23 19:57:51.000000 tulp-0.7/tulp/createFilteringProgramPrompt.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1443 2023-05-23 19:57:51.000000 tulp-0.7/tulp/createProgramPrompt.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)      389 2023-05-23 19:57:51.000000 tulp-0.7/tulp/executePython.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     4940 2023-05-03 18:35:41.000000 tulp-0.7/tulp/filteringPrompt.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     4481 2023-04-24 02:39:45.000000 tulp-0.7/tulp/filteringPrompt.roto.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1230 2023-05-06 16:28:30.000000 tulp-0.7/tulp/newMain.2.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)      921 2023-05-06 19:31:01.000000 tulp-0.7/tulp/newMain.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3841 2023-05-12 02:22:14.000000 tulp-0.7/tulp/requestPrompt.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)    15468 2023-05-03 22:20:43.000000 tulp-0.7/tulp/text_splitter.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)    15468 2023-05-03 22:26:14.000000 tulp-0.7/tulp/text_splitter_org.py
+-rwxrwxr-x   0 fede      (1000) fede      (1000)    12315 2023-05-23 19:57:51.000000 tulp-0.7/tulp/tulp.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1017 2023-05-06 20:21:58.000000 tulp-0.7/tulp/tulpargs.2.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1786 2023-05-23 19:57:51.000000 tulp-0.7/tulp/tulpargs.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1052 2023-05-06 20:28:06.000000 tulp-0.7/tulp/tulpconfig.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1722 2023-04-23 20:36:49.000000 tulp-0.7/tulp/tulplogger.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     2588 2023-05-12 15:19:39.000000 tulp-0.7/tulp/tulpparser.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)       16 2023-05-23 19:57:51.000000 tulp-0.7/tulp/version.py
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-05-23 19:58:07.877287 tulp-0.7/tulp.egg-info/
+-rw-rw-r--   0 fede      (1000) fede      (1000)     7906 2023-05-23 19:58:07.000000 tulp-0.7/tulp.egg-info/PKG-INFO
+-rw-rw-r--   0 fede      (1000) fede      (1000)      784 2023-05-23 19:58:07.000000 tulp-0.7/tulp.egg-info/SOURCES.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)        1 2023-05-23 19:58:07.000000 tulp-0.7/tulp.egg-info/dependency_links.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)       39 2023-05-23 19:58:07.000000 tulp-0.7/tulp.egg-info/entry_points.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)       15 2023-05-23 19:58:07.000000 tulp-0.7/tulp.egg-info/requires.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)        5 2023-05-23 19:58:07.000000 tulp-0.7/tulp.egg-info/top_level.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)        1 2023-04-21 01:25:36.000000 tulp-0.7/tulp.egg-info/zip-safe
```

### Comparing `tulp-0.6/LICENSE` & `tulp-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tulp-0.6/PKG-INFO` & `tulp-0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulp
-Version: 0.6
+Version: 0.7
 Summary: TULP: A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world.
 Home-page: https://github.com/fedenunez/tulp
 Author: Federico Nuñez
 Author-email: fedenunez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

### Comparing `tulp-0.6/README.md` & `tulp-0.7/README.md`

 * *Files identical despite different names*

### Comparing `tulp-0.6/setup.cfg` & `tulp-0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `tulp-0.6/test/test_filterMode_advanced.py` & `tulp-0.7/test/test_filterMode_advanced.py`

 * *Files identical despite different names*

### Comparing `tulp-0.6/test/test_filterMode_basic.py` & `tulp-0.7/test/test_filterMode_basic.py`

 * *Files identical despite different names*

### Comparing `tulp-0.6/test/test_requestMode.py` & `tulp-0.7/test/test_requestMode.py`

 * *Files identical despite different names*

### Comparing `tulp-0.6/test/test_slowtest.py` & `tulp-0.7/test/test_slowtest.py`

 * *Files identical despite different names*

### Comparing `tulp-0.6/tulp/filteringPrompt.py` & `tulp-0.7/tulp/filteringPrompt.py`

 * *Files identical despite different names*

### Comparing `tulp-0.6/tulp/filteringPrompt.roto.py` & `tulp-0.7/tulp/filteringPrompt.roto.py`

 * *Files identical despite different names*

### Comparing `tulp-0.6/tulp/newMain.2.py` & `tulp-0.7/tulp/newMain.2.py`

 * *Files identical despite different names*

### Comparing `tulp-0.6/tulp/newMain.py` & `tulp-0.7/tulp/newMain.py`

 * *Files identical despite different names*

### Comparing `tulp-0.6/tulp/programPrompt.py` & `tulp-0.7/tulp/requestPrompt.py`

 * *Files identical despite different names*

### Comparing `tulp-0.6/tulp/text_splitter.py` & `tulp-0.7/tulp/text_splitter.py`

 * *Files identical despite different names*

### Comparing `tulp-0.6/tulp/text_splitter_org.py` & `tulp-0.7/tulp/text_splitter_org.py`

 * *Files identical despite different names*

### Comparing `tulp-0.6/tulp/tulp.py` & `tulp-0.7/tulp/tulp.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import sys
 import os
 import math
 from . import tulpargs
 from . import tulplogger
 from . import tulpconfig
 from . import version
+from . import TulpOutputFileWriter
 
 log = tulplogger.Logger()
 config = tulpconfig.TulipConfig()
 args = tulpargs.TulpArgs().get()
 
 
 
@@ -28,15 +29,15 @@
 
 
 ## block_exists(blocks_dict, key):  test if a KEY exist and is not empty
 def block_exists(blocks_dict, key):
     return key in blocks_dict and len(blocks_dict[key]["content"].strip()) > 0
 
 ## VALID_BLOCKS: define the valid answer blocks  blocks
-VALID_BLOCKS=["(#output)","(#inner_message)","(#error)","(#context)","(#comment)","(#end)"]
+VALID_BLOCKS=["(#output)","(#thoughts)","(#inner_message)","(#error)","(#context)","(#comment)","(#end)"]
 ## parse_response)response_text): parse a gpt response, returning a dict with each response section 
 def parse_response(response_text):
     blocks_dict={}
     lines = response_text.splitlines()
     # (#end) is not specified by us, but sometimes gpt-3.5 wrote it so we just parse it so we can keep it out
 
     # parse blocks:
@@ -124,71 +125,89 @@
                     compressed_lines[compresed_index] += "\n"
 
     for line in compressed_lines:
         raw_input_chunks.append(line)
 
     return raw_input_chunks
 
-def run():
-    log.debug(f"Running tulp v{version.VERSION} using model: {config.model}")
-    openai_key = config.openai_api_key
-    if not openai_key:
-        log.error(f'OpenAI API key not found. Please set the TULP_OPENAI_API_KEY environment variable or add it to {tulpconfig.CONFIG_FILE}')
-        log.error(f"If you don't have one, please create one at: https://platform.openai.com/account/api-keys")
-        sys.exit(1)
-
-
-    openai.api_key = openai_key
-    prev_context=None
-
-
 
-    # If input is available on stdin, read it
-    input_text = ""
-    if not sys.stdin.isatty():
-        input_text = sys.stdin.read().strip()
-
-    user_request=None
-    if not args.request and not input_text:
-        user_request = input("Enter your request: ").strip()
-    elif args.request and not input_text:
-        user_request = args.request
-    elif not args.request and input_text:
-        user_request = "Summarize the input"
-    elif args.request and input_text:
-        user_request = args.request
-
-
-    getInstructionMessages=None
-    if input_text and user_request:
-        from . import filteringPrompt
-        getInstructionMessages=filteringPrompt.getMessages
+def processExecutionRequest(promptFactory, user_request, raw_input_chunks=None):
+    retries = 0
+    max_retries = 5
+    if (not raw_input_chunks):
+        raw_input_chunks = [""]
+    requestMessages = promptFactory.getMessages(user_request, raw_input_chunks[0], len(raw_input_chunks))
+    while retries < max_retries:
+        for req in requestMessages:
+            log.debug(f"REQ: {req}")
+        log.debug(f"Sending the request to OpenAI...")
+        response = openai.ChatCompletion.create(
+            model=config.model,
+            messages=requestMessages,
+            temperature=0
+        )
+        log.debug(f"ANS: {response}")
+        response_text = response.choices[0].message.content
+        finish_reason = response.choices[0].finish_reason
+        blocks_dict = parse_response(response_text)
+        if block_exists(blocks_dict,"(#comment)"):
+            log.info(blocks_dict["(#comment)"]["content"])
+        if block_exists(blocks_dict,"(#output)"):
+            oType = ""
+            generatedCode = cleanup_output(blocks_dict["(#output)"]["content"])
+            log.debug(f"The generated code:\n{generatedCode}")
+            from . import executePython
+            input_text="".join(raw_input_chunks)
+            if args.w:
+                ok, filename = TulpOutputFileWriter.TulpOutputFileWriter().write_to_file(args.w, generatedCode)
+                if ok: 
+                    log.info(f"Wrote created program at: {filename}")
+                else:
+                    log.error(f"Error while writing created code: {filename}")
+            log.info(f"Executing generated code...")
+            boutput, berror, ecode  = executePython.execute_python_code(generatedCode, input_text)
+            log.debug(f"Execution results: {boutput}, {berror}, {ecode}")
+            if (ecode != 0 and berror.find("Traceback") != -1 ):
+                retries += 1
+                log.warning(f"Error while executing the code, I will try to fix it!")
+                requestMessages = promptFactory.getMessages(user_request, raw_input_chunks[0], len(raw_input_chunks))
+                requestMessages.append(response.choices[0].message)
+                requestMessages.append({"role": "user","content": f"The execution of the program failed with error:\n{berror}\n\nPlease try to write a new (#output) that fixes the error"})
+            else:
+                break;
+    if retries == max_retries:
+        log.error("while executing generated code, max retries reached, giving up.")
     else:
-        from . import requestPrompt
-        getInstructionMessages=requestPrompt.getMessages
-
+        if (ecode != 0):
+            log.error(f"Error executing the program:\n{berror}")
+        else:
+            log.info("Code was executed correctly.")
 
-    raw_input_chunks = pre_process_raw_input(input_text)
+    print(boutput)
+    return ecode
 
+def processRequest(promptFactory,user_request, raw_input_chunks=None):
+    if not raw_input_chunks:
+        raw_input_chunks = [""] 
     for i in range(0,len(raw_input_chunks)):
         if (len(raw_input_chunks) > 1):
             log.info(f"Processing {i+1} of {len(raw_input_chunks)}...")
         else:
             log.info(f"Processing...")
         finish_reason = ""
         response_text = ""
         raw_input_chunk = raw_input_chunks[i]
         if user_request:
-            request = getInstructionMessages(user_request, raw_input_chunk , len(raw_input_chunks), i+1, prev_context)
-            for req in request:
+            requestMessages = promptFactory.getMessages(user_request, raw_input_chunk , len(raw_input_chunks), i+1)
+            for req in requestMessages:
                 log.debug(f"REQ: {req}")
             log.debug(f"Sending the request to OpenAI...")
             response = openai.ChatCompletion.create(
                 model=config.model,
-                messages=request,
+                messages=requestMessages,
                 temperature=0
             )
             log.debug(f"ANS: {response}")
             response_text += response.choices[0].message.content
             finish_reason = response.choices[0].finish_reason
 
 
@@ -233,9 +252,56 @@
 (currently ={config.max_chars}), using a different model or improving your
 instructions.
 """
 
             log.error(errorMsg)
             sys.exit(2)
 
+def run():
+    log.debug(f"Running tulp v{version.VERSION} using model: {config.model}")
+    openai_key = config.openai_api_key
+    if not openai_key:
+        log.error(f'OpenAI API key not found. Please set the TULP_OPENAI_API_KEY environment variable or add it to {tulpconfig.CONFIG_FILE}')
+        log.error(f"If you don't have one, please create one at: https://platform.openai.com/account/api-keys")
+        sys.exit(1)
+
+
+    openai.api_key = openai_key
+
+    # If input is available on stdin, read it
+    input_text = ""
+    if not sys.stdin.isatty():
+        input_text = sys.stdin.read().strip()
+
+    user_request=None
+    if not args.request and not input_text:
+        user_request = input("Enter your request: ").strip()
+    elif args.request and not input_text:
+        user_request = args.request
+    elif not args.request and input_text:
+        user_request = "Summarize the input"
+    elif args.request and input_text:
+        user_request = args.request
+
+    raw_input_chunks = pre_process_raw_input(input_text)
+
+    if input_text and user_request:
+        # A filtering request:
+        if (args.x):
+            from . import createFilteringProgramPrompt
+            sys.exit(processExecutionRequest(createFilteringProgramPrompt, user_request, raw_input_chunks))
+        else:
+            from . import filteringPrompt
+            sys.exit(processRequest(filteringPrompt, user_request, raw_input_chunks))
+    else:
+        # A request
+        if (args.x):
+            from . import createProgramPrompt
+            sys.exit(processExecutionRequest(createProgramPrompt, user_request))
+        else:
+            from . import requestPrompt
+            sys.exit(processRequest(requestPrompt, user_request))
+
+
+
 if __name__ == "__main__":
     run()
```

### Comparing `tulp-0.6/tulp/tulpargs.2.py` & `tulp-0.7/tulp/tulpargs.2.py`

 * *Files identical despite different names*

### Comparing `tulp-0.6/tulp/tulpconfig.py` & `tulp-0.7/tulp/tulpconfig.py`

 * *Files identical despite different names*

### Comparing `tulp-0.6/tulp/tulplogger.py` & `tulp-0.7/tulp/tulplogger.py`

 * *Files identical despite different names*

### Comparing `tulp-0.6/tulp.egg-info/PKG-INFO` & `tulp-0.7/tulp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulp
-Version: 0.6
+Version: 0.7
 Summary: TULP: A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world.
 Home-page: https://github.com/fedenunez/tulp
 Author: Federico Nuñez
 Author-email: fedenunez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

