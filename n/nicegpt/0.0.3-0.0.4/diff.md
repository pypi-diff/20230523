# Comparing `tmp/nicegpt-0.0.3.tar.gz` & `tmp/nicegpt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nicegpt-0.0.3.tar", last modified: Tue May 23 02:44:20 2023, max compression
+gzip compressed data, was "nicegpt-0.0.4.tar", last modified: Tue May 23 03:05:11 2023, max compression
```

## Comparing `nicegpt-0.0.3.tar` & `nicegpt-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 02:44:20.678429 nicegpt-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-05-08 21:26:59.000000 nicegpt-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     3497 2023-05-23 02:44:20.677429 nicegpt-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1594 2023-05-20 19:00:32.000000 nicegpt-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 02:44:20.651676 nicegpt-0.0.3/nicegpt/
--rw-rw-rw-   0        0        0       84 2023-05-09 21:32:02.000000 nicegpt-0.0.3/nicegpt/__init__.py
--rw-rw-rw-   0        0        0      700 2023-05-09 06:08:08.000000 nicegpt-0.0.3/nicegpt/helpers.py
--rw-rw-rw-   0        0        0     3725 2023-05-20 19:00:43.000000 nicegpt-0.0.3/nicegpt/nicegpt.py
-drwxrwxrwx   0        0        0        0 2023-05-23 02:44:20.676447 nicegpt-0.0.3/nicegpt.egg-info/
--rw-rw-rw-   0        0        0     3497 2023-05-23 02:44:20.000000 nicegpt-0.0.3/nicegpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-23 02:44:20.000000 nicegpt-0.0.3/nicegpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 02:44:20.000000 nicegpt-0.0.3/nicegpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-23 02:44:20.000000 nicegpt-0.0.3/nicegpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-23 02:44:20.000000 nicegpt-0.0.3/nicegpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      782 2023-05-20 18:59:16.000000 nicegpt-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 02:44:20.678429 nicegpt-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 03:05:11.020659 nicegpt-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-05-08 21:26:59.000000 nicegpt-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3497 2023-05-23 03:05:11.017208 nicegpt-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1594 2023-05-20 19:00:32.000000 nicegpt-0.0.4/README.md
+-rw-rw-rw-   0        0        0      782 2023-05-23 03:01:24.000000 nicegpt-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 03:05:11.020659 nicegpt-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 03:05:10.962240 nicegpt-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 03:05:10.984491 nicegpt-0.0.4/src/nicegpt/
+-rw-rw-rw-   0        0        0       80 2023-05-23 03:00:07.000000 nicegpt-0.0.4/src/nicegpt/__init__.py
+-rw-rw-rw-   0        0        0      700 2023-05-09 06:08:08.000000 nicegpt-0.0.4/src/nicegpt/helpers.py
+-rw-rw-rw-   0        0        0     3739 2023-05-23 03:00:47.000000 nicegpt-0.0.4/src/nicegpt/nicegpt.py
+drwxrwxrwx   0        0        0        0 2023-05-23 03:05:11.016208 nicegpt-0.0.4/src/nicegpt.egg-info/
+-rw-rw-rw-   0        0        0     3497 2023-05-23 03:05:10.000000 nicegpt-0.0.4/src/nicegpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-05-23 03:05:10.000000 nicegpt-0.0.4/src/nicegpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 03:05:10.000000 nicegpt-0.0.4/src/nicegpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-23 03:05:10.000000 nicegpt-0.0.4/src/nicegpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-23 03:05:10.000000 nicegpt-0.0.4/src/nicegpt.egg-info/top_level.txt
```

### Comparing `nicegpt-0.0.3/LICENSE` & `nicegpt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nicegpt-0.0.3/PKG-INFO` & `nicegpt-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicegpt
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple package to make GPT API usage easier
 Author-email: Samuel Reeder <samuel.reeder@mail.utoronto.ca>
 License: MIT License
         
         Copyright (c) 2023 Samuel Reeder
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nicegpt-0.0.3/README.md` & `nicegpt-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nicegpt-0.0.3/nicegpt/helpers.py` & `nicegpt-0.0.4/src/nicegpt/helpers.py`

 * *Files identical despite different names*

### Comparing `nicegpt-0.0.3/nicegpt/nicegpt.py` & `nicegpt-0.0.4/src/nicegpt/nicegpt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 GPT class file.
 """
 import openai
-import helpers
+from helpers import compile_messages
 from enum import Enum
 from typing import Any
 
 
 class Model(Enum):
     """
     This Enum class represents the available GPT models that can be used.
@@ -51,15 +51,15 @@
         self.completion_tokens = 0
 
     def response(self, prompt: str, just_reply=True, **kwargs: Any) -> str | dict:
         """
         Obtain a context-driven response from GPT given the specified prompt.
         """
         self.messages.append([prompt, None])
-        messages = helpers.compile_messages(self.messages, self._system)
+        messages = compile_messages(self.messages, self._system)
         response = openai.ChatCompletion.create(
             model=self._model,
             messages=messages,
             **kwargs,
         )
         if response is None:
             raise Exception(
```

### Comparing `nicegpt-0.0.3/nicegpt.egg-info/PKG-INFO` & `nicegpt-0.0.4/src/nicegpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicegpt
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple package to make GPT API usage easier
 Author-email: Samuel Reeder <samuel.reeder@mail.utoronto.ca>
 License: MIT License
         
         Copyright (c) 2023 Samuel Reeder
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nicegpt-0.0.3/pyproject.toml` & `nicegpt-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nicegpt"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Samuel Reeder", email="samuel.reeder@mail.utoronto.ca" },
 ]
 description = "A simple package to make GPT API usage easier"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
```

