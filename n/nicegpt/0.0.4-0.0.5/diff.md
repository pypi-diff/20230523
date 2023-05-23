# Comparing `tmp/nicegpt-0.0.4.tar.gz` & `tmp/nicegpt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nicegpt-0.0.4.tar", last modified: Tue May 23 03:05:11 2023, max compression
+gzip compressed data, was "nicegpt-0.0.5.tar", last modified: Tue May 23 03:15:14 2023, max compression
```

## Comparing `nicegpt-0.0.4.tar` & `nicegpt-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 03:05:11.020659 nicegpt-0.0.4/
--rw-rw-rw-   0        0        0     1091 2023-05-08 21:26:59.000000 nicegpt-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3497 2023-05-23 03:05:11.017208 nicegpt-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1594 2023-05-20 19:00:32.000000 nicegpt-0.0.4/README.md
--rw-rw-rw-   0        0        0      782 2023-05-23 03:01:24.000000 nicegpt-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 03:05:11.020659 nicegpt-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-23 03:05:10.962240 nicegpt-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 03:05:10.984491 nicegpt-0.0.4/src/nicegpt/
--rw-rw-rw-   0        0        0       80 2023-05-23 03:00:07.000000 nicegpt-0.0.4/src/nicegpt/__init__.py
--rw-rw-rw-   0        0        0      700 2023-05-09 06:08:08.000000 nicegpt-0.0.4/src/nicegpt/helpers.py
--rw-rw-rw-   0        0        0     3739 2023-05-23 03:00:47.000000 nicegpt-0.0.4/src/nicegpt/nicegpt.py
-drwxrwxrwx   0        0        0        0 2023-05-23 03:05:11.016208 nicegpt-0.0.4/src/nicegpt.egg-info/
--rw-rw-rw-   0        0        0     3497 2023-05-23 03:05:10.000000 nicegpt-0.0.4/src/nicegpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-05-23 03:05:10.000000 nicegpt-0.0.4/src/nicegpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 03:05:10.000000 nicegpt-0.0.4/src/nicegpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-23 03:05:10.000000 nicegpt-0.0.4/src/nicegpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-23 03:05:10.000000 nicegpt-0.0.4/src/nicegpt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 03:15:14.788907 nicegpt-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-05-08 21:26:59.000000 nicegpt-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3497 2023-05-23 03:15:14.787908 nicegpt-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1594 2023-05-20 19:00:32.000000 nicegpt-0.0.5/README.md
+-rw-rw-rw-   0        0        0      782 2023-05-23 03:14:56.000000 nicegpt-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 03:15:14.788907 nicegpt-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 03:15:14.731843 nicegpt-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 03:15:14.758850 nicegpt-0.0.5/src/nicegpt/
+-rw-rw-rw-   0        0        0      141 2023-05-23 03:12:19.000000 nicegpt-0.0.5/src/nicegpt/__init__.py
+-rw-rw-rw-   0        0        0     4347 2023-05-23 03:15:03.000000 nicegpt-0.0.5/src/nicegpt/nicegpt.py
+drwxrwxrwx   0        0        0        0 2023-05-23 03:15:14.786906 nicegpt-0.0.5/src/nicegpt.egg-info/
+-rw-rw-rw-   0        0        0     3497 2023-05-23 03:15:14.000000 nicegpt-0.0.5/src/nicegpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-05-23 03:15:14.000000 nicegpt-0.0.5/src/nicegpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 03:15:14.000000 nicegpt-0.0.5/src/nicegpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-23 03:15:14.000000 nicegpt-0.0.5/src/nicegpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-23 03:15:14.000000 nicegpt-0.0.5/src/nicegpt.egg-info/top_level.txt
```

### Comparing `nicegpt-0.0.4/LICENSE` & `nicegpt-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nicegpt-0.0.4/PKG-INFO` & `nicegpt-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicegpt
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple package to make GPT API usage easier
 Author-email: Samuel Reeder <samuel.reeder@mail.utoronto.ca>
 License: MIT License
         
         Copyright (c) 2023 Samuel Reeder
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nicegpt-0.0.4/README.md` & `nicegpt-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nicegpt-0.0.4/pyproject.toml` & `nicegpt-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nicegpt"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Samuel Reeder", email="samuel.reeder@mail.utoronto.ca" },
 ]
 description = "A simple package to make GPT API usage easier"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
```

### Comparing `nicegpt-0.0.4/src/nicegpt/nicegpt.py` & `nicegpt-0.0.5/src/nicegpt/nicegpt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,37 @@
 """
 GPT class file.
 """
 import openai
-from helpers import compile_messages
 from enum import Enum
 from typing import Any
 
 
+def config(key: str, organization: str = None) -> None:
+    """
+    Provide a valid OpenAI Api Key to provide to the openai package
+    """
+    openai.api_key = key
+    if organization is not None:
+        openai.organization = organization
+
+
+def compile_messages(messages: list[list[str, str | str, None]], system: str = None, ) -> list[dict]:
+    """
+    Compile a list of message dictionaries given a list of lists [user_prompt, gpt_response], and an optional system message.    
+    """
+    formatted_messages = messages.copy()
+    formatted_messages = [] if not system else [{"role": "system", "content": system}]
+    for exchange in messages:
+        formatted_messages.append({"role": "user", "content": exchange[0]})
+        if exchange[1] is not None:
+            formatted_messages.append({"role": "assistant", "content": exchange[1]})
+    return formatted_messages
+
+
 class Model(Enum):
     """
     This Enum class represents the available GPT models that can be used.
 
     Each model is represented by a tuple that contains the model's identifier string 
     and two rate values. The first rate value corresponds to the cost per 1000 tokens 
     for prompts, and the second rate value corresponds to the cost per 1000 tokens 
@@ -93,17 +114,8 @@
         """
         messages = []
         for exchange in self.messages:
             user_message, gpt_message = {
                 "user": exchange[0]}, {"assistant": exchange[1]}
             messages.extend([user_message, gpt_message])
 
-        return messages
-
-
-def config(key: str, organization: str = None) -> None:
-    """
-    Provide a valid OpenAI Api Key to provide to the openai package
-    """
-    openai.api_key = key
-    if organization is not None:
-        openai.organization = organization
+        return messages
```

### Comparing `nicegpt-0.0.4/src/nicegpt.egg-info/PKG-INFO` & `nicegpt-0.0.5/src/nicegpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicegpt
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple package to make GPT API usage easier
 Author-email: Samuel Reeder <samuel.reeder@mail.utoronto.ca>
 License: MIT License
         
         Copyright (c) 2023 Samuel Reeder
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

