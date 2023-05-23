# Comparing `tmp/aish-0.1.1.tar.gz` & `tmp/aish-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aish-0.1.1.tar", last modified: Tue May 23 15:05:39 2023, max compression
+gzip compressed data, was "aish-0.1.3.tar", last modified: Tue May 23 16:52:19 2023, max compression
```

## Comparing `aish-0.1.1.tar` & `aish-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-23 15:05:39.268332 aish-0.1.1/
--rw-r--r--   0 toni       (501) staff       (20)     1054 2023-05-19 19:01:29.000000 aish-0.1.1/LICENCE
--rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-23 15:05:39.268065 aish-0.1.1/PKG-INFO
--rw-r--r--   0 toni       (501) staff       (20)     1532 2023-05-22 15:47:59.000000 aish-0.1.1/README.md
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-23 15:05:39.265483 aish-0.1.1/aish/
--rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:02.000000 aish-0.1.1/aish/__init__.py
--rw-r--r--   0 toni       (501) staff       (20)     7270 2023-05-23 14:59:52.000000 aish-0.1.1/aish/aish.py
--rw-r--r--   0 toni       (501) staff       (20)     2395 2023-05-22 11:56:07.000000 aish-0.1.1/aish/proxy.py
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-23 15:05:39.267513 aish-0.1.1/aish.egg-info/
--rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-23 15:05:39.000000 aish-0.1.1/aish.egg-info/PKG-INFO
--rw-r--r--   0 toni       (501) staff       (20)      258 2023-05-23 15:05:39.000000 aish-0.1.1/aish.egg-info/SOURCES.txt
--rw-r--r--   0 toni       (501) staff       (20)        1 2023-05-23 15:05:39.000000 aish-0.1.1/aish.egg-info/dependency_links.txt
--rw-r--r--   0 toni       (501) staff       (20)       40 2023-05-23 15:05:39.000000 aish-0.1.1/aish.egg-info/entry_points.txt
--rw-r--r--   0 toni       (501) staff       (20)       29 2023-05-23 15:05:39.000000 aish-0.1.1/aish.egg-info/requires.txt
--rw-r--r--   0 toni       (501) staff       (20)       11 2023-05-23 15:05:39.000000 aish-0.1.1/aish.egg-info/top_level.txt
--rw-r--r--   0 toni       (501) staff       (20)       38 2023-05-23 15:05:39.268408 aish-0.1.1/setup.cfg
--rw-r--r--   0 toni       (501) staff       (20)      571 2023-05-23 15:05:31.000000 aish-0.1.1/setup.py
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-23 15:05:39.267777 aish-0.1.1/tests/
--rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:28.000000 aish-0.1.1/tests/__init__.py
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-23 16:52:19.813260 aish-0.1.3/
+-rw-r--r--   0 toni       (501) staff       (20)     1054 2023-05-19 19:01:29.000000 aish-0.1.3/LICENCE
+-rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-23 16:52:19.812837 aish-0.1.3/PKG-INFO
+-rw-r--r--   0 toni       (501) staff       (20)     1532 2023-05-22 15:47:59.000000 aish-0.1.3/README.md
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-23 16:52:19.809708 aish-0.1.3/aish/
+-rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:02.000000 aish-0.1.3/aish/__init__.py
+-rw-r--r--   0 toni       (501) staff       (20)     8387 2023-05-23 16:49:03.000000 aish-0.1.3/aish/aish.py
+-rw-r--r--   0 toni       (501) staff       (20)     2395 2023-05-22 11:56:07.000000 aish-0.1.3/aish/proxy.py
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-23 16:52:19.811857 aish-0.1.3/aish.egg-info/
+-rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-23 16:52:19.000000 aish-0.1.3/aish.egg-info/PKG-INFO
+-rw-r--r--   0 toni       (501) staff       (20)      258 2023-05-23 16:52:19.000000 aish-0.1.3/aish.egg-info/SOURCES.txt
+-rw-r--r--   0 toni       (501) staff       (20)        1 2023-05-23 16:52:19.000000 aish-0.1.3/aish.egg-info/dependency_links.txt
+-rw-r--r--   0 toni       (501) staff       (20)       40 2023-05-23 16:52:19.000000 aish-0.1.3/aish.egg-info/entry_points.txt
+-rw-r--r--   0 toni       (501) staff       (20)       36 2023-05-23 16:52:19.000000 aish-0.1.3/aish.egg-info/requires.txt
+-rw-r--r--   0 toni       (501) staff       (20)       11 2023-05-23 16:52:19.000000 aish-0.1.3/aish.egg-info/top_level.txt
+-rw-r--r--   0 toni       (501) staff       (20)       38 2023-05-23 16:52:19.813362 aish-0.1.3/setup.cfg
+-rw-r--r--   0 toni       (501) staff       (20)      590 2023-05-23 16:52:00.000000 aish-0.1.3/setup.py
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-23 16:52:19.812209 aish-0.1.3/tests/
+-rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:28.000000 aish-0.1.3/tests/__init__.py
```

### Comparing `aish-0.1.1/LICENCE` & `aish-0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `aish-0.1.1/PKG-INFO` & `aish-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aish
-Version: 0.1.1
+Version: 0.1.3
 Summary: A command-line application that interacts with the OpenAI ChatGPT API.
 Author: Toni Leino
 Author-email: toni@leino.net
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # Aish - ChatGPT CLI
```

### Comparing `aish-0.1.1/README.md` & `aish-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `aish-0.1.1/aish/aish.py` & `aish-0.1.3/aish/aish.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import argparse
 import json
 import os
+import re
 
 import requests
+from distro import name as distro_name
 from rich import print as pprint
 from rich.console import Console
 from rich.panel import Panel
 from rich.syntax import Syntax
 
 # Initializing console object for better user experience and output formatting
 console = Console()
 
+user_shell = os.environ["SHELL"].split("/")[-1]
+user_distro = distro_name(pretty=True)
+
 DEFAULT_CONFIG = {
     "roles": {
-        "default": "You are a command-line application designed to assist with coding and system management tasks. Your current task is to administer the Mac OS operating system using the zsh shell. Please only present simple, unformatted text in your responses. Avoid offering any advice or details about your functions.",
-        "shell": "Output only plain text zsh commands for Mac OS  without any description or explanation. If there is a lack of details, provide the most logical solution. Ensure that the output of your response is a valid shell command. If multiple steps are required, try to combine them together.",
+        "default": f"You are a command-line application designed to assist with coding and system management tasks. Your current task is to administer the {user_distro} operating system using the {user_shell} shell. Please only present simple, unformatted text in your responses. Avoid offering any advice or details about your functions.",
+        "shell": f"Output only plain text {user_shell} commands for {user_distro}  without any description or explanation. If there is a lack of details, provide the most logical solution. Ensure that the output of your response is a valid shell command. If multiple steps are required, try to combine them together.",
         "code": "Output only plain text code without any description or explanation. Do not ask for more details. If multiple steps are required, try to combine them together.",
     },
     "model": "gpt-3.5-turbo",
     "temperature": 0.5,
     "top_p": 0.5,
     "timeout": 60,
     "role": "default",
@@ -59,28 +64,35 @@
     ) as response:
         response.raise_for_status()
         answer = ""
         rline = ""
 
         in_code_block = False
         language = ""
-
+        lines_printed = 0
         for line in response.iter_lines():
             data = line.lstrip(b"data: ").decode("utf-8")
             if data == "[DONE]":
                 console.print("", end="\r")
 
                 if "```" in rline:
                     in_code_block = not in_code_block
                     rline = "   "
 
                 if in_code_block:
-                    console.print(Panel(rline), end="\n")
+                    syntax = Syntax(rline, language)
+                    console.print(syntax, end="\n")
                 else:
-                    console.print(rline, end="\n")
+                    if lines_printed == 0 and config["role"] == "shell":
+                        syntax = Syntax(rline, language)
+                        console.print(syntax, end="\n")
+                        if not re.search("this is not a .* command\.", rline):
+                            answer = f"```\n{rline}\n```"
+                    else:
+                        console.print(rline, end="\n")
 
                 rline = ""
                 break
 
             if not data:
                 continue
 
@@ -88,28 +100,29 @@
             delta = data["choices"][0]["delta"]
             if "content" not in delta:
                 continue
             answer += delta["content"]
             out = delta["content"]
 
             if "\n" in out:
+                lines_printed += 1
                 out = out.replace("\n", "")
                 rline += out
 
                 console.print("", end="\r")
 
                 if "```" in rline:
                     console.print("            ", end="\n")
                     in_code_block = not in_code_block
                     if in_code_block:
                         parts = rline.split("```")
                         if len(parts) > 1:
                             language = parts[1]
                         else:
-                            language = "zsh"
+                            language = user_shell
                     rline = ""
 
                 elif in_code_block:
                     syntax = Syntax(rline, language)
                     console.print(syntax, end="\n")
                 else:
                     console.print(rline, end="\n")
@@ -117,15 +130,14 @@
             else:
                 console.print(out, end="")
                 rline += out
 
         print()
 
         if config["role"] == "shell":
-            shell = os.environ.get("SHELL", "/bin/sh")
             code_blocks = []
             lines = answer.split("\n")
             in_code_block = False
 
             for line in lines:
                 if "```" in line:
                     in_code_block = not in_code_block
@@ -133,14 +145,16 @@
                     code_blocks.append(line.strip())
 
             execute_shell_commands(code_blocks, debug)
 
 
 def chat(prompt, config, debug=False, playback=False):
     prompt = " ".join(prompt)
+    if prompt == "":
+        prompt = input("How can I help you? ")
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {os.getenv('OPENAI_API_KEY')}",
     }
 
     messages = [
         {"role": "system", "content": config["roles"][config["role"]]},
@@ -221,12 +235,16 @@
         config["url"] = args.url
 
     if args.code:
         config["role"] = "code"
     elif args.shell:
         config["role"] = "shell"
 
-    chat(args.prompt, config, args.debug, args.playback)
+    try:                                                                                                                                                                                                                        
+        chat(args.prompt, config, args.debug, args.playback)
+    except KeyboardInterrupt:                                                                                                                                                                                                   
+        pass
+
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `aish-0.1.1/aish/proxy.py` & `aish-0.1.3/aish/proxy.py`

 * *Files identical despite different names*

### Comparing `aish-0.1.1/aish.egg-info/PKG-INFO` & `aish-0.1.3/aish.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aish
-Version: 0.1.1
+Version: 0.1.3
 Summary: A command-line application that interacts with the OpenAI ChatGPT API.
 Author: Toni Leino
 Author-email: toni@leino.net
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # Aish - ChatGPT CLI
```

### Comparing `aish-0.1.1/setup.py` & `aish-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aish',
-    version='0.1.1',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=[
         'rich',
         'flask',
         'requests',
-        'argparse'
+        'argparse',
+        'distro',
     ],
     entry_points={
         'console_scripts': [
             'aish=aish.aish:main'
        ],
     },
     author='Toni Leino',
```

