# Comparing `tmp/agixt-1.1.66b0.tar.gz` & `tmp/agixt-1.1.67b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.66b0.tar", last modified: Mon May 22 18:55:52 2023, max compression
+gzip compressed data, was "agixt-1.1.67b0.tar", last modified: Tue May 23 00:49:32 2023, max compression
```

## Comparing `agixt-1.1.66b0.tar` & `agixt-1.1.67b0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:55:52.801069 agixt-1.1.66b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-22 18:55:40.000000 agixt-1.1.66b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-22 18:55:40.000000 agixt-1.1.66b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-22 18:55:52.801069 agixt-1.1.66b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:55:52.797068 agixt-1.1.66b0/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/AGiXT.py
--rw-r--r--   0 runner    (1001) docker     (123)    13536 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/Commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/CustomPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/Main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/Tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:55:52.801069 agixt-1.1.66b0/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/provider/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 18:55:40.000000 agixt-1.1.66b0/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:55:52.797068 agixt-1.1.66b0/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-22 18:55:52.000000 agixt-1.1.66b0/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-22 18:55:52.000000 agixt-1.1.66b0/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 18:55:52.000000 agixt-1.1.66b0/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-22 18:55:52.000000 agixt-1.1.66b0/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 18:55:52.000000 agixt-1.1.66b0/agixt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:55:52.801069 agixt-1.1.66b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-22 18:55:40.000000 agixt-1.1.66b0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-22 18:55:40.000000 agixt-1.1.66b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 18:55:52.801069 agixt-1.1.66b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-22 18:55:40.000000 agixt-1.1.66b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:49:32.870091 agixt-1.1.67b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-23 00:49:17.000000 agixt-1.1.67b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-23 00:49:17.000000 agixt-1.1.67b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-23 00:49:32.870091 agixt-1.1.67b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:49:32.866091 agixt-1.1.67b0/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/AGiXT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14049 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/Commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/CustomPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/Main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/Tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:49:32.870091 agixt-1.1.67b0/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 00:49:17.000000 agixt-1.1.67b0/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:49:32.870091 agixt-1.1.67b0/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-23 00:49:32.000000 agixt-1.1.67b0/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-23 00:49:32.000000 agixt-1.1.67b0/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 00:49:32.000000 agixt-1.1.67b0/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-23 00:49:32.000000 agixt-1.1.67b0/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 00:49:32.000000 agixt-1.1.67b0/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:49:32.870091 agixt-1.1.67b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-23 00:49:17.000000 agixt-1.1.67b0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-23 00:49:17.000000 agixt-1.1.67b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 00:49:32.870091 agixt-1.1.67b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-23 00:49:17.000000 agixt-1.1.67b0/setup.py
```

### Comparing `agixt-1.1.66b0/LICENSE` & `agixt-1.1.67b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/PKG-INFO` & `agixt-1.1.67b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.66b0
+Version: 1.1.67b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.66b0/agixt/AGiXT.py` & `agixt-1.1.67b0/agixt/AGiXT.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/Agent.py` & `agixt-1.1.67b0/agixt/Agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import os
-import re
 import json
 import glob
-import uuid
 import shutil
 import importlib
 import yaml
 from pathlib import Path
 from inspect import signature, Parameter
 from provider import Provider
 from Memories import Memories
@@ -15,15 +13,17 @@
 
 class Agent:
     def __init__(self, agent_name=None):
         # General Configuration
         self.agent_name = agent_name if agent_name is not None else "AGiXT"
         # Need to get the following from the agent config file:
         self.AGENT_CONFIG = self.get_agent_config()
+        self.commands = self.load_commands()
         self.available_commands = Commands(self.AGENT_CONFIG).get_available_commands()
+        self.clean_agent_config_commands()
         self.execute = Commands(self.AGENT_CONFIG).execute_command
         # AI Configuration
         if "settings" in self.AGENT_CONFIG:
             self.PROVIDER_SETTINGS = self.AGENT_CONFIG["settings"]
             if "provider" in self.PROVIDER_SETTINGS:
                 self.AI_PROVIDER = self.PROVIDER_SETTINGS["provider"]
                 self.PROVIDER = Provider(self.AI_PROVIDER, **self.PROVIDER_SETTINGS)
@@ -61,14 +61,25 @@
             if key in self.AGENT_CONFIG:
                 setattr(self, key, self.AGENT_CONFIG[key])
 
     def _create_parent_directories(self, file_path):
         path = Path(file_path)
         path.parent.mkdir(parents=True, exist_ok=True)
 
+    def clean_agent_config_commands(self):
+        for command in self.commands:
+            friendly_name = command[0]
+            if friendly_name not in self.AGENT_CONFIG["commands"]:
+                self.AGENT_CONFIG["commands"][friendly_name] = False
+        for command in list(self.AGENT_CONFIG["commands"]):
+            if command not in [cmd[0] for cmd in self.commands]:
+                del self.AGENT_CONFIG["commands"][command]
+        with open(f"agents/{self.agent_name}/config.json", "w") as f:
+            json.dump(self.AGENT_CONFIG, f)
+
     def get_commands_string(self):
         if len(self.available_commands) == 0:
             return "No commands."
 
         enabled_commands = filter(
             lambda command: command.get("enabled", True), self.available_commands
         )
@@ -198,18 +209,14 @@
                                 "embedder": "default",
                             },
                         }
                     )
                 )
         return agent_config_data
 
-    def write_agent_config(self, agent_config, config_data):
-        with open(agent_config, "w") as f:
-            json.dump(config_data, f)
-
     def add_agent(self, agent_name, provider_settings):
         if not agent_name:
             return "Agent name cannot be empty."
         provider_settings = (
             {
                 "provider": "gpt4free",
                 "AI_MODEL": "gpt-3.5-turbo",
@@ -230,14 +237,15 @@
             agent_name, provider_settings, command_dict
         )
         with open(os.path.join("agents", f"{agent_name}.yaml"), "w") as f:
             f.write("")
         return {"agent_file": f"{agent_name}.yaml"}
 
     def rename_agent(self, agent_name, new_name):
+        self.agent_name = new_name
         agent_file = f"agents/{agent_name}.yaml"
         agent_folder = f"agents/{agent_name}/"
         agent_file = os.path.abspath(agent_file)
         agent_folder = os.path.abspath(agent_folder)
         if os.path.exists(agent_file):
             os.rename(agent_file, os.path.join("agents", f"{new_name}.yaml"))
         if os.path.exists(agent_folder):
```

### Comparing `agixt-1.1.66b0/agixt/Chain.py` & `agixt-1.1.67b0/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/Commands.py` & `agixt-1.1.67b0/agixt/Commands.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/Config.py` & `agixt-1.1.67b0/agixt/Config.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/CustomPrompt.py` & `agixt-1.1.67b0/agixt/CustomPrompt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/Embedding.py` & `agixt-1.1.67b0/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/Main.py` & `agixt-1.1.67b0/agixt/Main.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/Memories.py` & `agixt-1.1.67b0/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/Tasks.py` & `agixt-1.1.67b0/agixt/Tasks.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/app.py` & `agixt-1.1.67b0/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/provider/__init__.py` & `agixt-1.1.67b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/provider/azure.py` & `agixt-1.1.67b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/provider/bing.py` & `agixt-1.1.67b0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/provider/chatgpt.py` & `agixt-1.1.67b0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/provider/claude.py` & `agixt-1.1.67b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/provider/fastchat.py` & `agixt-1.1.67b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/provider/gpt4all.py` & `agixt-1.1.67b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/provider/gpt4free.py` & `agixt-1.1.67b0/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/provider/gpugpt4all.py` & `agixt-1.1.67b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/provider/huggingchat.py` & `agixt-1.1.67b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/provider/kobold.py` & `agixt-1.1.67b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/provider/llamacpp.py` & `agixt-1.1.67b0/agixt/provider/llamacpp.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,17 +37,16 @@
             except:
                 self.MAX_TOKENS = 2000
 
         if os.path.isfile(MODEL_PATH):
             self.model = Llama(
                 model_path=MODEL_PATH,
                 n_ctx=(int(self.MAX_TOKENS) * 2),
-                n_gpu_layers=self.GPU_LAYERS,
-                n_batch=self.BATCH_SIZE,
-                n_threads=self.THREADS,
+                n_gpu_layers=int(self.GPU_LAYERS),
+                n_threads=int(self.THREADS),
             )
         else:
             print("Unable to find model path.")
 
     def instruct(self, prompt, tokens: int = 0):
         max_tokens = int(self.MAX_TOKENS) - tokens
         if max_tokens < 1:
```

### Comparing `agixt-1.1.66b0/agixt/provider/oobabooga.py` & `agixt-1.1.67b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/provider/openai.py` & `agixt-1.1.67b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/provider/palm.py` & `agixt-1.1.67b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/provider/transformer.py` & `agixt-1.1.67b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/agixt/requirements.txt` & `agixt-1.1.67b0/agixt.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 chromadb
+sentence-transformers
+llama-cpp-python
+accelerate
+nomic
+chromadb
 argparse
 anthropic
 beautifulsoup4
 captcha-solver
 docker
 duckduckgo_search==2.9.5
 fastapi
@@ -27,21 +32,19 @@
 selenium
 sendgrid
 tiktoken
 tweepy
 webdriver_manager
 spacy
 discord
-git+https://github.com/xtekky/gpt4free
--r https://raw.githubusercontent.com/xtekky/gpt4free/main/requirements.txt
 EdgeGPT
 google-generativeai
 google-cloud-aiplatform
 streamlit
 docx2txt
 pdfplumber
 ffmpeg
 hugchat
 flask-bcrypt
 revChatGPT
 random-password-generator
-cryptography==38.0.4
+cryptography==38.0.4
```

### Comparing `agixt-1.1.66b0/agixt.egg-info/PKG-INFO` & `agixt-1.1.67b0/agixt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.66b0
+Version: 1.1.67b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.66b0/agixt.egg-info/SOURCES.txt` & `agixt-1.1.67b0/agixt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/docs/README.md` & `agixt-1.1.67b0/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.1.66b0/setup.py` & `agixt-1.1.67b0/setup.py`

 * *Files identical despite different names*

