# Comparing `tmp/connpy-3.2.6.tar.gz` & `tmp/connpy-3.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connpy-3.2.6.tar", last modified: Mon May 22 21:33:59 2023, max compression
+gzip compressed data, was "connpy-3.2.7.tar", last modified: Tue May 23 19:16:09 2023, max compression
```

## Comparing `connpy-3.2.6.tar` & `connpy-3.2.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:33:59.711212 connpy-3.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-22 21:33:47.000000 connpy-3.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-22 21:33:59.711212 connpy-3.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-05-22 21:33:47.000000 connpy-3.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:33:59.707212 connpy-3.2.6/connpy/
--rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-05-22 21:33:47.000000 connpy-3.2.6/connpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-22 21:33:47.000000 connpy-3.2.6/connpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-22 21:33:47.000000 connpy-3.2.6/connpy/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21366 2023-05-22 21:33:47.000000 connpy-3.2.6/connpy/ai.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5102 2023-05-22 21:33:47.000000 connpy-3.2.6/connpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-22 21:33:47.000000 connpy-3.2.6/connpy/completion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15540 2023-05-22 21:33:47.000000 connpy-3.2.6/connpy/configfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50300 2023-05-22 21:33:47.000000 connpy-3.2.6/connpy/connapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28719 2023-05-22 21:33:47.000000 connpy-3.2.6/connpy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:33:59.707212 connpy-3.2.6/connpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-22 21:33:59.000000 connpy-3.2.6/connpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-22 21:33:59.000000 connpy-3.2.6/connpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 21:33:59.000000 connpy-3.2.6/connpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-22 21:33:59.000000 connpy-3.2.6/connpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-22 21:33:59.000000 connpy-3.2.6/connpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 21:33:59.000000 connpy-3.2.6/connpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-22 21:33:59.711212 connpy-3.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-22 21:33:47.000000 connpy-3.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:16:09.755095 connpy-3.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-23 19:15:57.000000 connpy-3.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-23 19:16:09.755095 connpy-3.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-05-23 19:15:57.000000 connpy-3.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:16:09.755095 connpy-3.2.7/connpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-05-23 19:15:57.000000 connpy-3.2.7/connpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-23 19:15:57.000000 connpy-3.2.7/connpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 19:15:57.000000 connpy-3.2.7/connpy/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22109 2023-05-23 19:15:57.000000 connpy-3.2.7/connpy/ai.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5102 2023-05-23 19:15:57.000000 connpy-3.2.7/connpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-23 19:15:57.000000 connpy-3.2.7/connpy/completion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15540 2023-05-23 19:15:57.000000 connpy-3.2.7/connpy/configfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50300 2023-05-23 19:15:57.000000 connpy-3.2.7/connpy/connapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28719 2023-05-23 19:15:57.000000 connpy-3.2.7/connpy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:16:09.755095 connpy-3.2.7/connpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-23 19:16:09.000000 connpy-3.2.7/connpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-23 19:16:09.000000 connpy-3.2.7/connpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 19:16:09.000000 connpy-3.2.7/connpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-23 19:16:09.000000 connpy-3.2.7/connpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-23 19:16:09.000000 connpy-3.2.7/connpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 19:16:09.000000 connpy-3.2.7/connpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-23 19:16:09.755095 connpy-3.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-23 19:15:57.000000 connpy-3.2.7/setup.py
```

### Comparing `connpy-3.2.6/LICENSE` & `connpy-3.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `connpy-3.2.6/PKG-INFO` & `connpy-3.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.2.6
+Version: 3.2.7
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.2.6/README.md` & `connpy-3.2.7/README.md`

 * *Files identical despite different names*

### Comparing `connpy-3.2.6/connpy/__init__.py` & `connpy-3.2.7/connpy/__init__.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.6/connpy/ai.py` & `connpy-3.2.7/connpy/ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,24 @@
             If the input does not fit into either of these categories, kindly express that you didn't understand and request the user to rephrase their response.
             """
         self.__prompt["confirmation_user"] = "Yes go ahead!"
         self.__prompt["confirmation_assistant"] = "True"
         self.model = model
         self.temp = temp
 
+    def process_string(self, s):
+        if s.startswith('[') and s.endswith(']') and not (s.startswith("['") and s.endswith("']")) and not (s.startswith('["') and s.endswith('"]')):
+            # Extract the content inside square brackets and split by comma
+            content = s[1:-1].split(',')
+            # Add single quotes around each item and join them back together with commas
+            new_content = ', '.join(f"'{item.strip()}'" for item in content)
+            # Replace the old content with the new content
+            s = '[' + new_content + ']'
+        return s
+
     def _retry_function(self, function, max_retries, backoff_num, *args):
         #Retry openai requests
         retries = 0
         while retries < max_retries:
             try:
                 myfunction = function(*args)
                 break
@@ -172,14 +182,15 @@
                 if value.lower() == "true":
                     value = True
                 elif value.lower() == "false":
                     value = False
                 elif value.lower() == "none":
                     value = None
                 if key == "filter":
+                    value = self.process_string(value)
                     value = ast.literal_eval(value)
                 #store in dictionary
                 info_dict[key] = value
                 current_key = key
             else:
                 if current_key == "response":
                     if "response" in info_dict:
@@ -225,18 +236,18 @@
 
     def _get_commands(self, user_input, nodes):
         #Send the request for commands for each device to openAI GPT.
         output_list = []
         for key, value in nodes.items():
             tags = value.get('tags', {})
             try:
-                os_value = tags.get('os', '')
+                if os_value := tags.get('os'):
+                    output_list.append(f"{key}: {os_value}")
             except:
-                os_value = ""
-            output_list.append(f"{key}: {os_value}")
+                pass
         output_str = "\n".join(output_list)
         command_input = f"input: {user_input}\n\nDevices:\n{output_str}"
         message = []
         message.append({"role": "system", "content": dedent(self.__prompt["command_system"]).strip()})
         message.append({"role": "user", "content": dedent(self.__prompt["command_user"]).strip()})
         message.append({"role": "assistant", "content": dedent(self.__prompt["command_assistant"]).strip()})
         message.append({"role": "user", "content": command_input})
@@ -407,14 +418,15 @@
                 if not commands:
                     output["app_related"] = False
                     output["response"] = f"{self.model} api is not responding right now, please try again later."
                     return output
                 output["args"] = {}
                 output["args"]["commands"] = commands["response"]["commands"]
                 output["args"]["vars"] = commands["response"]["variables"]
+                output["nodes"] = [item for item in output["nodes"] if output["args"]["vars"].get(item)]
                 if original["response"].get("expected"):
                     output["args"]["expected"] = original["response"]["expected"]
                     output["action"] = "test"
                 else:
                     output["action"] = "run"
                 if dryrun:
                     output["task"] = []
```

### Comparing `connpy-3.2.6/connpy/api.py` & `connpy-3.2.7/connpy/api.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.6/connpy/completion.py` & `connpy-3.2.7/connpy/completion.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.6/connpy/configfile.py` & `connpy-3.2.7/connpy/configfile.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.6/connpy/connapp.py` & `connpy-3.2.7/connpy/connapp.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.6/connpy/core.py` & `connpy-3.2.7/connpy/core.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.6/connpy.egg-info/PKG-INFO` & `connpy-3.2.7/connpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.2.6
+Version: 3.2.7
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.2.6/setup.cfg` & `connpy-3.2.7/setup.cfg`

 * *Files identical despite different names*

