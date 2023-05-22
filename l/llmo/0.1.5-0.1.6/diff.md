# Comparing `tmp/llmo-0.1.5.tar.gz` & `tmp/llmo-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmo-0.1.5.tar", last modified: Mon May 22 08:20:47 2023, max compression
+gzip compressed data, was "llmo-0.1.6.tar", last modified: Mon May 22 21:37:44 2023, max compression
```

## Comparing `llmo-0.1.5.tar` & `llmo-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.1.5/LICENSE
--rw-r--r--   0        0        0     2134 2023-05-22 08:06:19.890271 llmo-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.1.5/llmo/__init__.py
--rw-r--r--   0        0        0    18412 2023-05-22 08:18:40.772359 llmo-0.1.5/llmo/chat.py
--rw-r--r--   0        0        0      353 2023-05-21 18:43:49.180818 llmo-0.1.5/llmo/layout.css
--rw-r--r--   0        0        0      680 2023-05-22 08:20:47.621318 llmo-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2479 1970-01-01 00:00:00.000000 llmo-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2134 2023-05-22 08:06:19.890271 llmo-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.1.6/llmo/__init__.py
+-rw-r--r--   0        0        0    18574 2023-05-22 21:37:00.363982 llmo-0.1.6/llmo/chat.py
+-rw-r--r--   0        0        0      353 2023-05-21 18:43:49.180818 llmo-0.1.6/llmo/layout.css
+-rw-r--r--   0        0        0      680 2023-05-22 21:37:44.394393 llmo-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2479 1970-01-01 00:00:00.000000 llmo-0.1.6/PKG-INFO
```

### Comparing `llmo-0.1.5/LICENSE` & `llmo-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `llmo-0.1.5/README.md` & `llmo-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `llmo-0.1.5/llmo/chat.py` & `llmo-0.1.6/llmo/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,28 +432,32 @@
 
     @work
     async def handle_initial_submission(self):
         """This runs after the app is mounted, if a prompt was passed from the CLI."""
         await self.handle_submission()
 
 
-def run_shell_mode(openai_client: OpenAI, prompt=None, files=None):
+def run_shell_mode(
+    openai_client: OpenAI,
+    prompt=None,
+    files=None,
+    rich_text_mode=False,
+):
     console = Console()
 
     async def display_content():
         response = ""
         num_lines_to_clear = 0
 
         async for content in openai_client.asubmit(prompt=prompt, files=files):
             response += content
             console.print(content, soft_wrap=True, end="")
             num_lines_to_clear += content.count("\n")
 
-        if num_lines_to_clear > 0:
-            # Clear the previously printed lines
+        if rich_text_mode and num_lines_to_clear > 0:
             for _ in range(num_lines_to_clear):
                 print("\033[F\033[K", end="")
 
             md = rich.markdown.Markdown(response)
             console.print(md)
         else:
             console.print()
@@ -471,16 +475,16 @@
     parser = argparse.ArgumentParser(
         description="chat and pair-programming from the command-line"
     )
 
     parser.add_argument(
         "prompt",
         type=str,
-        nargs="?",
-        default="",
+        nargs=argparse.REMAINDER,
+        default=[],
         help="initial LLM prompt (optional)",
     )
     parser.add_argument(
         "-f",
         "--files",
         type=str,
         action="append",
@@ -534,14 +538,16 @@
         disable_personality_env_var.lower().startswith("t")
         or disable_personality_env_var == "1"
     ):
         parser.set_defaults(personality=False)
 
     args = parser.parse_args()
 
+    args.prompt = " ".join(args.prompt)
+
     staged_files = [Path(f) for f in args.files] if args.files else []
 
     for f in staged_files:
         assert f.exists(), f"File {f} does not exist"
 
     openai_client = OpenAI(
         model=args.model,
@@ -549,15 +555,20 @@
         max_tokens=args.max_tokens,
     )
 
     if args.personality:
         openai_client.add_personality()
 
     if args.shell_mode:
-        run_shell_mode(openai_client, prompt=args.prompt, files=args.files)
+        run_shell_mode(
+            openai_client,
+            prompt=args.prompt,
+            files=args.files,
+            rich_text_mode=args.rich_text_mode,
+        )
     else:
         app = LLMO(
             prompt=args.prompt,
             staged_files=staged_files,
             openai_client=openai_client,
             rich_text_mode=args.rich_text_mode,
         )
```

### Comparing `llmo-0.1.5/pyproject.toml` & `llmo-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llmo"
-version = "0.1.5"
+version = "0.1.6"
 description = "AI pair programmer"
 authors = [
     { name = "Stephan Fitzpatrick", email = "stephan@knowsuchagency.com" },
 ]
 dependencies = [
     "textual>=0.26.0",
     "openai>=0.27.6",
```

### Comparing `llmo-0.1.5/PKG-INFO` & `llmo-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmo
-Version: 0.1.5
+Version: 0.1.6
 Summary: AI pair programmer
 Author-Email: Stephan Fitzpatrick <stephan@knowsuchagency.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/knowsuchagency/llmo
 Requires-Python: >=3.10
 Requires-Dist: textual>=0.26.0
 Requires-Dist: openai>=0.27.6
```

