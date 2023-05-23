# Comparing `tmp/llmo-0.2.1.tar.gz` & `tmp/llmo-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmo-0.2.1.tar", last modified: Tue May 23 04:45:58 2023, max compression
+gzip compressed data, was "llmo-0.2.2.tar", last modified: Tue May 23 04:56:57 2023, max compression
```

## Comparing `llmo-0.2.1.tar` & `llmo-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.2.1/LICENSE
--rw-r--r--   0        0        0     2134 2023-05-22 08:06:19.890271 llmo-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.2.1/llmo/__init__.py
--rw-r--r--   0        0        0     2898 2023-05-22 22:11:47.649149 llmo-0.2.1/llmo/cli.py
--rw-r--r--   0        0        0      122 2023-05-22 21:51:03.475865 llmo-0.2.1/llmo/constants.py
--rw-r--r--   0        0        0     9793 2023-05-23 03:53:39.625867 llmo-0.2.1/llmo/gui.py
--rw-r--r--   0        0        0      341 2023-05-23 03:17:45.469101 llmo-0.2.1/llmo/layout.css
--rw-r--r--   0        0        0     5982 2023-05-23 03:45:21.644631 llmo-0.2.1/llmo/llms.py
--rw-r--r--   0        0        0     1223 2023-05-23 04:45:14.948974 llmo-0.2.1/llmo/shell_mode.py
--rw-r--r--   0        0        0      699 2023-05-23 04:45:58.778013 llmo-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      838 2023-05-22 22:24:34.139710 llmo-0.2.1/tests/test_openai.py
--rw-r--r--   0        0        0     2479 1970-01-01 00:00:00.000000 llmo-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2134 2023-05-22 08:06:19.890271 llmo-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.2.2/llmo/__init__.py
+-rw-r--r--   0        0        0     2898 2023-05-22 22:11:47.649149 llmo-0.2.2/llmo/cli.py
+-rw-r--r--   0        0        0      122 2023-05-22 21:51:03.475865 llmo-0.2.2/llmo/constants.py
+-rw-r--r--   0        0        0     9793 2023-05-23 03:53:39.625867 llmo-0.2.2/llmo/gui.py
+-rw-r--r--   0        0        0      341 2023-05-23 03:17:45.469101 llmo-0.2.2/llmo/layout.css
+-rw-r--r--   0        0        0     5982 2023-05-23 03:45:21.644631 llmo-0.2.2/llmo/llms.py
+-rw-r--r--   0        0        0     1593 2023-05-23 04:53:16.585981 llmo-0.2.2/llmo/shell_mode.py
+-rw-r--r--   0        0        0      699 2023-05-23 04:56:57.394313 llmo-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      838 2023-05-22 22:24:34.139710 llmo-0.2.2/tests/test_openai.py
+-rw-r--r--   0        0        0     2479 1970-01-01 00:00:00.000000 llmo-0.2.2/PKG-INFO
```

### Comparing `llmo-0.2.1/LICENSE` & `llmo-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llmo-0.2.1/README.md` & `llmo-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `llmo-0.2.1/llmo/cli.py` & `llmo-0.2.2/llmo/cli.py`

 * *Files identical despite different names*

### Comparing `llmo-0.2.1/llmo/gui.py` & `llmo-0.2.2/llmo/gui.py`

 * *Files identical despite different names*

### Comparing `llmo-0.2.1/llmo/llms.py` & `llmo-0.2.2/llmo/llms.py`

 * *Files identical despite different names*

### Comparing `llmo-0.2.1/llmo/shell_mode.py` & `llmo-0.2.2/llmo/shell_mode.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import asyncio
+import signal
 
 from rich.console import Console
 from rich.markdown import Markdown
 from rich.prompt import Prompt
+from rich.text import Text
 
 from llmo.llms import OpenAI
 
 
 def run_shell_mode(
     openai_client: OpenAI,
     prompt=None,
@@ -17,31 +19,38 @@
 
     async def display_content():
         response = ""
         num_lines_to_clear = 0
 
         async for content in openai_client.asubmit(prompt=prompt, files=files):
             response += content
-            console.print(content, soft_wrap=True, end="")
+            content_text = Text(content, style="green")
+            console.print(content_text, soft_wrap=True, end="")
             num_lines_to_clear += content.count("\n")
 
         if rich_text_mode and num_lines_to_clear > 0:
             for _ in range(num_lines_to_clear):
-                print("\033[F\033[K", end="")
+                console.print(Text("\033[F\033[K", style="red"), end="")
 
             md = Markdown(response)
             console.print(md)
         else:
             console.print()
 
+    def handle_keyboard_interrupt(signal_number, frame):
+        console.print(Text("\nReceived keyboard interrupt. Exiting...", style="red"))
+        exit(0)
+
+    signal.signal(signal.SIGINT, handle_keyboard_interrupt)
+
     initial_prompt = True if prompt else False
 
     while True:
         if not initial_prompt:
-            prompt = Prompt.ask(">> ")
+            prompt = Prompt.ask(Text(">> ", style="bold"))
 
             if prompt in ["exit", "clear"]:
                 if prompt == "exit":
                     return
                 console.clear()
                 continue
```

### Comparing `llmo-0.2.1/pyproject.toml` & `llmo-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llmo"
-version = "0.2.1"
+version = "0.2.2"
 description = "AI pair programmer"
 authors = [
     { name = "Stephan Fitzpatrick", email = "stephan@knowsuchagency.com" },
 ]
 dependencies = [
     "textual>=0.26.0",
     "openai>=0.27.6",
```

### Comparing `llmo-0.2.1/tests/test_openai.py` & `llmo-0.2.2/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `llmo-0.2.1/PKG-INFO` & `llmo-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmo
-Version: 0.2.1
+Version: 0.2.2
 Summary: AI pair programmer
 Author-Email: Stephan Fitzpatrick <stephan@knowsuchagency.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/knowsuchagency/llmo
 Requires-Python: >=3.10
 Requires-Dist: textual>=0.26.0
 Requires-Dist: openai>=0.27.6
```

