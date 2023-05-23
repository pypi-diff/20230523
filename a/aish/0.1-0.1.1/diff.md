# Comparing `tmp/aish-0.1.tar.gz` & `tmp/aish-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aish-0.1.tar", last modified: Mon May 22 15:46:10 2023, max compression
+gzip compressed data, was "aish-0.1.1.tar", last modified: Tue May 23 15:05:39 2023, max compression
```

## Comparing `aish-0.1.tar` & `aish-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-22 15:46:10.114516 aish-0.1/
--rw-r--r--   0 toni       (501) staff       (20)     1054 2023-05-19 19:01:29.000000 aish-0.1/LICENCE
--rw-r--r--   0 toni       (501) staff       (20)     1806 2023-05-22 15:46:10.114202 aish-0.1/PKG-INFO
--rw-r--r--   0 toni       (501) staff       (20)     1568 2023-05-21 17:16:49.000000 aish-0.1/README.md
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-22 15:46:10.111029 aish-0.1/aish/
--rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:02.000000 aish-0.1/aish/__init__.py
--rw-r--r--   0 toni       (501) staff       (20)     9060 2023-05-22 15:29:47.000000 aish-0.1/aish/aish.py
--rw-r--r--   0 toni       (501) staff       (20)     2395 2023-05-22 11:56:07.000000 aish-0.1/aish/proxy.py
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-22 15:46:10.113503 aish-0.1/aish.egg-info/
--rw-r--r--   0 toni       (501) staff       (20)     1806 2023-05-22 15:46:10.000000 aish-0.1/aish.egg-info/PKG-INFO
--rw-r--r--   0 toni       (501) staff       (20)      258 2023-05-22 15:46:10.000000 aish-0.1/aish.egg-info/SOURCES.txt
--rw-r--r--   0 toni       (501) staff       (20)        1 2023-05-22 15:46:10.000000 aish-0.1/aish.egg-info/dependency_links.txt
--rw-r--r--   0 toni       (501) staff       (20)       40 2023-05-22 15:46:10.000000 aish-0.1/aish.egg-info/entry_points.txt
--rw-r--r--   0 toni       (501) staff       (20)       29 2023-05-22 15:46:10.000000 aish-0.1/aish.egg-info/requires.txt
--rw-r--r--   0 toni       (501) staff       (20)       11 2023-05-22 15:46:10.000000 aish-0.1/aish.egg-info/top_level.txt
--rw-r--r--   0 toni       (501) staff       (20)       38 2023-05-22 15:46:10.114614 aish-0.1/setup.cfg
--rw-r--r--   0 toni       (501) staff       (20)      569 2023-05-22 12:02:57.000000 aish-0.1/setup.py
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-22 15:46:10.113837 aish-0.1/tests/
--rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:28.000000 aish-0.1/tests/__init__.py
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-23 15:05:39.268332 aish-0.1.1/
+-rw-r--r--   0 toni       (501) staff       (20)     1054 2023-05-19 19:01:29.000000 aish-0.1.1/LICENCE
+-rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-23 15:05:39.268065 aish-0.1.1/PKG-INFO
+-rw-r--r--   0 toni       (501) staff       (20)     1532 2023-05-22 15:47:59.000000 aish-0.1.1/README.md
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-23 15:05:39.265483 aish-0.1.1/aish/
+-rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:02.000000 aish-0.1.1/aish/__init__.py
+-rw-r--r--   0 toni       (501) staff       (20)     7270 2023-05-23 14:59:52.000000 aish-0.1.1/aish/aish.py
+-rw-r--r--   0 toni       (501) staff       (20)     2395 2023-05-22 11:56:07.000000 aish-0.1.1/aish/proxy.py
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-23 15:05:39.267513 aish-0.1.1/aish.egg-info/
+-rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-23 15:05:39.000000 aish-0.1.1/aish.egg-info/PKG-INFO
+-rw-r--r--   0 toni       (501) staff       (20)      258 2023-05-23 15:05:39.000000 aish-0.1.1/aish.egg-info/SOURCES.txt
+-rw-r--r--   0 toni       (501) staff       (20)        1 2023-05-23 15:05:39.000000 aish-0.1.1/aish.egg-info/dependency_links.txt
+-rw-r--r--   0 toni       (501) staff       (20)       40 2023-05-23 15:05:39.000000 aish-0.1.1/aish.egg-info/entry_points.txt
+-rw-r--r--   0 toni       (501) staff       (20)       29 2023-05-23 15:05:39.000000 aish-0.1.1/aish.egg-info/requires.txt
+-rw-r--r--   0 toni       (501) staff       (20)       11 2023-05-23 15:05:39.000000 aish-0.1.1/aish.egg-info/top_level.txt
+-rw-r--r--   0 toni       (501) staff       (20)       38 2023-05-23 15:05:39.268408 aish-0.1.1/setup.cfg
+-rw-r--r--   0 toni       (501) staff       (20)      571 2023-05-23 15:05:31.000000 aish-0.1.1/setup.py
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-23 15:05:39.267777 aish-0.1.1/tests/
+-rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:28.000000 aish-0.1.1/tests/__init__.py
```

### Comparing `aish-0.1/LICENCE` & `aish-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `aish-0.1/PKG-INFO` & `aish-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aish
-Version: 0.1
+Version: 0.1.1
 Summary: A command-line application that interacts with the OpenAI ChatGPT API.
 Author: Toni Leino
 Author-email: toni@leino.net
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # Aish - ChatGPT CLI
@@ -12,15 +12,15 @@
 This command-line interface (CLI) application is used to interact with the OpenAI through the OpenAI API. The chatbot takes an input prompt and returns a response from the selected model.
 
 ## Installation
 
 Ensure you have Python 3.7+ installed. To install the required libraries, use:
 
 ```bash
-    pip install git+https://github.com/Frodotus/aish.git
+    pip install aish
 ```
 
 ## Usage
 
 To use the application, you need to set the environment variable `OPENAI_API_KEY` with your OpenAI API key. Then, you can run the script from the terminal using the command:
 
 ```bash
```

### Comparing `aish-0.1/README.md` & `aish-0.1.1/aish.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,26 @@
+Metadata-Version: 2.1
+Name: aish
+Version: 0.1.1
+Summary: A command-line application that interacts with the OpenAI ChatGPT API.
+Author: Toni Leino
+Author-email: toni@leino.net
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
 # Aish - ChatGPT CLI
 
 This command-line interface (CLI) application is used to interact with the OpenAI through the OpenAI API. The chatbot takes an input prompt and returns a response from the selected model.
 
 ## Installation
 
 Ensure you have Python 3.7+ installed. To install the required libraries, use:
 
 ```bash
-    pip install git+https://github.com/Frodotus/aish.git
+    pip install aish
 ```
 
 ## Usage
 
 To use the application, you need to set the environment variable `OPENAI_API_KEY` with your OpenAI API key. Then, you can run the script from the terminal using the command:
 
 ```bash
@@ -35,8 +44,8 @@
 
 ## Help
 
 You can display the help message which provides details about the command usage and the different parameters by running:
 
 ```bash
     aish --help
-```
+```
```

### Comparing `aish-0.1/aish/aish.py` & `aish-0.1.1/aish/aish.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,245 +1,232 @@
-# Importing necessary libraries
 import argparse
 import json
 import os
 
 import requests
 from rich import print as pprint
 from rich.console import Console
-from rich.markdown import Markdown
 from rich.panel import Panel
 from rich.syntax import Syntax
 
 # Initializing console object for better user experience and output formatting
 console = Console()
 
+DEFAULT_CONFIG = {
+    "roles": {
+        "default": "You are a command-line application designed to assist with coding and system management tasks. Your current task is to administer the Mac OS operating system using the zsh shell. Please only present simple, unformatted text in your responses. Avoid offering any advice or details about your functions.",
+        "shell": "Output only plain text zsh commands for Mac OS  without any description or explanation. If there is a lack of details, provide the most logical solution. Ensure that the output of your response is a valid shell command. If multiple steps are required, try to combine them together.",
+        "code": "Output only plain text code without any description or explanation. Do not ask for more details. If multiple steps are required, try to combine them together.",
+    },
+    "model": "gpt-3.5-turbo",
+    "temperature": 0.5,
+    "top_p": 0.5,
+    "timeout": 60,
+    "role": "default",
+    "url": "https://api.openai.com/v1/chat/completions",
+}
 
-# Initializing the chat function with default parameters and/or custom configurations
-def chat(
-    prompt, model, temperature, top_p, timeout, role, url, debug=False, playback=False
-):
-    defaults = {
-        "roles": {
-            "default": "You are a command-line application designed to assist with coding and system management tasks. Your current task is to administer the Mac OS operating system using the zsh shell. Please only present simple, unformatted text in your responses. Avoid offering any advice or details about your functions.",
-            "shell": "Output only plain text zsh commands for Mac OS  without any description or explanation. If there is a lack of details, provide the most logical solution. Ensure that the output of your response is a valid shell command. If multiple steps are required, try to combine them together.",
-            "code": "Output only plain text code without any description or explanation. Do not ask for more details. If multiple steps are required, try to combine them together.",
-        },
-        "model": "gpt-3.5-turbo",
-        "temperature": 0.5,
-        "top_p": 0.5,
-        "timeout": 60,
-        "role": "default",
-        "url": "https://api.openai.com/v1/chat/completions",
-    }
 
-    # Reading the configuration from a config.json file, and overriding any attribute if provided by the user
+def load_config(defaults):
     try:
         with open("config.json") as f:
             config = json.load(f)
     except FileNotFoundError:
         config = defaults
     defaults.update(config)
-    model = model or defaults["model"]
-    temperature = temperature or defaults["temperature"]
-    top_p = top_p or defaults["top_p"]
-    timeout = timeout or defaults["timeout"]
-    role = role or defaults["role"]
-    url = url or defaults["url"]
-    prompt = prompt or []
-
-    # Role validation
-    if role not in defaults["roles"]:
-        print(
-            f"Error: '{role}' is not a valid role. Please choose from: {list(defaults['roles'].keys())}"
-        )
-        return
+    return defaults
 
-    # Formatting user input and preparing headers for requesting chat(Response formatting)
-    prompt = " ".join(prompt)
-    headers = {
-        "Content-Type": "application/json",
-        "Authorization": f"Bearer {os.getenv('OPENAI_API_KEY')}",
-    }
 
-    # Configuration setup for the request
-    messages = [
-        {"role": "system", "content": defaults["roles"][role]},
-        {"role": "user", "content": prompt},
-    ]
-    data = {
-        "messages": messages,
-        "model": model,
-        "temperature": temperature,
-        "top_p": top_p,
-        "stream": True,
-    }
+def execute_shell_commands(commands, debug=False):
+    shell = os.environ.get("SHELL", "/bin/sh")
+    if debug:
+        print("Commands: ", commands)
 
-    # Enabling playback feature if requested by user for the previous response
-    if playback:
-        data["playback"] = True
+    if len(commands) > 0:
+        for command in commands:
+            choice = input(f"Execute command '{command}'? (Y/n): ")
+
+            if choice.lower() == "y" or choice == "":
+                os.system(f"{shell} -c '{command}'")
 
-    # Debugging enabled to display the request and response details
-    if debug:
-        pprint("--- Request ---")
-        pprint(data)
-        pprint("--- Response ---")
 
-    # Making the API call to OpenAI GPT-3 Chat API
+def get_api_response(data, headers, config, debug=False):
     with requests.post(
-        url, headers=headers, data=json.dumps(data), timeout=timeout, stream=True
+        config["url"],
+        headers=headers,
+        data=json.dumps(data),
+        timeout=config["timeout"],
+        stream=True,
     ) as response:
         response.raise_for_status()
         answer = ""
         rline = ""
 
         in_code_block = False
         language = ""
 
-        # Iterating through the response received in chunks of lines
         for line in response.iter_lines():
-            # Converting the byte output to string and checking if response is completely received
             data = line.lstrip(b"data: ").decode("utf-8")
             if data == "[DONE]":
                 console.print("", end="\r")
-                if "```" in rline:  # This line is a delimiter
-                    in_code_block = not in_code_block  # Change the state
+
+                if "```" in rline:
+                    in_code_block = not in_code_block
                     rline = "   "
 
                 if in_code_block:
                     console.print(Panel(rline), end="\n")
                 else:
                     console.print(rline, end="\n")
-                    
+
                 rline = ""
                 break
 
-            # Checking if response is empty after decoding, useful for handling exceptions
             if not data:
                 continue
 
-            # Extracting the content to display from the JSON response
             data = json.loads(data)
             delta = data["choices"][0]["delta"]
             if "content" not in delta:
                 continue
             answer += delta["content"]
             out = delta["content"]
-            # Handling multiple lines of output formatting with Rich library
+
             if "\n" in out:
                 out = out.replace("\n", "")
                 rline += out
 
                 console.print("", end="\r")
-                    
-                if "```" in rline:  # This line is a delimiter
+
+                if "```" in rline:
+                    console.print("            ", end="\n")
                     in_code_block = not in_code_block
                     if in_code_block:
-                        # Split the line by "```"
                         parts = rline.split("```")
                         if len(parts) > 1:
-                            # The second part of the split contains the language
                             language = parts[1]
                         else:
-                            # No language specified
                             language = "zsh"
-                    rline = "   "
+                    rline = ""
 
-                if in_code_block:
+                elif in_code_block:
                     syntax = Syntax(rline, language)
-                    console.print(syntax, style="on bright_black", width=console.width, end="\n")
+                    console.print(syntax, end="\n")
                 else:
                     console.print(rline, end="\n")
                 rline = ""
             else:
                 console.print(out, end="")
                 rline += out
 
         print()
 
-        # Processing code blocks obtained from response for shell role
-        if role == "shell":
+        if config["role"] == "shell":
             shell = os.environ.get("SHELL", "/bin/sh")
             code_blocks = []
             lines = answer.split("\n")
             in_code_block = False
 
             for line in lines:
-                if "```" in line:  # This line is a delimiter
-                    in_code_block = not in_code_block  # Change the state
-                elif in_code_block:  # We're inside a code block
+                if "```" in line:
+                    in_code_block = not in_code_block
+                elif in_code_block:
                     code_blocks.append(line.strip())
 
-            # Printing the resulting lines
-            if debug:
-                print("Commands: ", code_blocks)
-
-            if len(code_blocks) > 0:
-                # Loop through each command in the list
-                for code_block in code_blocks:
-                    commands = code_block.split("\n")
-                    for command in commands:
-                        choice = input(f"Execute command '{command}'? (Y/n): ")
-
-                        # If the user selects yes, execute the current command
-                        if choice.lower() == "y" or choice == "":
-                            os.system(f"{shell} -c '{command}'")
+            execute_shell_commands(code_blocks, debug)
+
+
+def chat(prompt, config, debug=False, playback=False):
+    prompt = " ".join(prompt)
+    headers = {
+        "Content-Type": "application/json",
+        "Authorization": f"Bearer {os.getenv('OPENAI_API_KEY')}",
+    }
+
+    messages = [
+        {"role": "system", "content": config["roles"][config["role"]]},
+        {"role": "user", "content": prompt},
+    ]
+    data = {
+        "messages": messages,
+        "model": config["model"],
+        "temperature": config["temperature"],
+        "top_p": config["top_p"],
+        "stream": True,
+    }
+
+    if playback:
+        data["playback"] = True
+
+    if debug:
+        pprint("--- Request ---")
+        pprint(data)
+        pprint("--- Response ---")
+
+    get_api_response(data, headers, config, debug)
 
 
 def main():
-    # Initializing ArgumentParser object with description of chat function arguments
     parser = argparse.ArgumentParser(description="Get a response from the ChatGPT API.")
     parser.add_argument(
         "prompt", nargs="*", help="The initial text that you want the AI to respond to."
     )
     parser.add_argument(
-        "--model", type=str, help="The model version that you want to use."
+        "--model", "-m", type=str, help="The model version that you want to use."
     )
     parser.add_argument(
-        "--temperature", type=float, help="The randomness of the AI’s responses."
+        "--temperature", "-t", type=float, help="The randomness of the AI’s responses."
     )
     parser.add_argument(
-        "--top_p", type=float, help="A parameter for controlling randomness."
+        "--top_p", "-p", type=float, help="A parameter for controlling randomness."
     )
     parser.add_argument(
         "--timeout",
+        "-o",
         type=int,
         help="The maximum time in seconds that the request will wait for a response from the API.",
     )
-    parser.add_argument("--role", type=str, help="The role of the assistant.")
+    parser.add_argument("--role", "-r", type=str, help="The role of the assistant.")
     parser.add_argument(
         "--shell", "-s", action="store_true", help="Execute the command in the shell."
     )
     parser.add_argument("--code", "-c", action="store_true", help="Output only code.")
-    parser.add_argument("--url", type=str, help="The API endpoint to use.")
-    parser.add_argument("--debug", action="store_true")
+    parser.add_argument("--url", "-u", type=str, help="The API endpoint to use.")
+    parser.add_argument(
+        "--debug",
+        "-d",
+        action="store_true",
+        help="Print debug information to the console.",
+    )
     parser.add_argument(
         "--playback",
+        "-b",
         action="store_true",
-        help="Playback previous response. Works only when using proxy",
+        help="Replay the conversation from the beginning.",
     )
 
     args = parser.parse_args()
-    role = args.role or "default"
+    config = load_config(DEFAULT_CONFIG)
+
+    if args.model:
+        config["model"] = args.model
+    if args.temperature:
+        config["temperature"] = args.temperature
+    if args.top_p:
+        config["top_p"] = args.top_p
+    if args.timeout:
+        config["timeout"] = args.timeout
+    if args.role:
+        config["role"] = args.role
+    if args.url:
+        config["url"] = args.url
 
-    # Setting the role based on user parameters code or shell
     if args.code:
-        role = "code"
+        config["role"] = "code"
     elif args.shell:
-        role = "shell"
+        config["role"] = "shell"
 
-    # Calling the chat function with all the parameters
-    chat(
-        args.prompt,
-        args.model,
-        args.temperature,
-        args.top_p,
-        args.timeout,
-        role,
-        args.url,
-        debug=args.debug,
-        playback=args.playback,
-    )
+    chat(args.prompt, config, args.debug, args.playback)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `aish-0.1/aish/proxy.py` & `aish-0.1.1/aish/proxy.py`

 * *Files identical despite different names*

### Comparing `aish-0.1/aish.egg-info/PKG-INFO` & `aish-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,17 @@
-Metadata-Version: 2.1
-Name: aish
-Version: 0.1
-Summary: A command-line application that interacts with the OpenAI ChatGPT API.
-Author: Toni Leino
-Author-email: toni@leino.net
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
 # Aish - ChatGPT CLI
 
 This command-line interface (CLI) application is used to interact with the OpenAI through the OpenAI API. The chatbot takes an input prompt and returns a response from the selected model.
 
 ## Installation
 
 Ensure you have Python 3.7+ installed. To install the required libraries, use:
 
 ```bash
-    pip install git+https://github.com/Frodotus/aish.git
+    pip install aish
 ```
 
 ## Usage
 
 To use the application, you need to set the environment variable `OPENAI_API_KEY` with your OpenAI API key. Then, you can run the script from the terminal using the command:
 
 ```bash
@@ -44,8 +35,8 @@
 
 ## Help
 
 You can display the help message which provides details about the command usage and the different parameters by running:
 
 ```bash
     aish --help
-```
+```
```

### Comparing `aish-0.1/setup.py` & `aish-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aish',
-    version='0.1',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         'rich',
         'flask',
         'requests',
         'argparse'
     ],
```

