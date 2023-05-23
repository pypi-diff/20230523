# Comparing `tmp/nicegpt-0.0.5.tar.gz` & `tmp/nicegpt-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nicegpt-0.0.5.tar", last modified: Tue May 23 03:15:14 2023, max compression
+gzip compressed data, was "nicegpt-0.0.6.tar", last modified: Tue May 23 03:19:07 2023, max compression
```

## Comparing `nicegpt-0.0.5.tar` & `nicegpt-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 03:15:14.788907 nicegpt-0.0.5/
--rw-rw-rw-   0        0        0     1091 2023-05-08 21:26:59.000000 nicegpt-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3497 2023-05-23 03:15:14.787908 nicegpt-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1594 2023-05-20 19:00:32.000000 nicegpt-0.0.5/README.md
--rw-rw-rw-   0        0        0      782 2023-05-23 03:14:56.000000 nicegpt-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 03:15:14.788907 nicegpt-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-23 03:15:14.731843 nicegpt-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 03:15:14.758850 nicegpt-0.0.5/src/nicegpt/
--rw-rw-rw-   0        0        0      141 2023-05-23 03:12:19.000000 nicegpt-0.0.5/src/nicegpt/__init__.py
--rw-rw-rw-   0        0        0     4347 2023-05-23 03:15:03.000000 nicegpt-0.0.5/src/nicegpt/nicegpt.py
-drwxrwxrwx   0        0        0        0 2023-05-23 03:15:14.786906 nicegpt-0.0.5/src/nicegpt.egg-info/
--rw-rw-rw-   0        0        0     3497 2023-05-23 03:15:14.000000 nicegpt-0.0.5/src/nicegpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-05-23 03:15:14.000000 nicegpt-0.0.5/src/nicegpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 03:15:14.000000 nicegpt-0.0.5/src/nicegpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-23 03:15:14.000000 nicegpt-0.0.5/src/nicegpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-23 03:15:14.000000 nicegpt-0.0.5/src/nicegpt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 03:19:07.191847 nicegpt-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2023-05-08 21:26:59.000000 nicegpt-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3497 2023-05-23 03:19:07.190847 nicegpt-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1594 2023-05-20 19:00:32.000000 nicegpt-0.0.6/README.md
+-rw-rw-rw-   0        0        0      782 2023-05-23 03:18:34.000000 nicegpt-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 03:19:07.191847 nicegpt-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 03:19:07.162906 nicegpt-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 03:19:07.168142 nicegpt-0.0.6/src/nicegpt/
+-rw-rw-rw-   0        0        0      141 2023-05-23 03:12:19.000000 nicegpt-0.0.6/src/nicegpt/__init__.py
+-rw-rw-rw-   0        0        0     4348 2023-05-23 03:17:14.000000 nicegpt-0.0.6/src/nicegpt/nicegpt.py
+-rw-rw-rw-   0        0        0      236 2023-05-23 03:17:52.000000 nicegpt-0.0.6/src/nicegpt/text.py
+drwxrwxrwx   0        0        0        0 2023-05-23 03:19:07.189865 nicegpt-0.0.6/src/nicegpt.egg-info/
+-rw-rw-rw-   0        0        0     3497 2023-05-23 03:19:07.000000 nicegpt-0.0.6/src/nicegpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-05-23 03:19:07.000000 nicegpt-0.0.6/src/nicegpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 03:19:07.000000 nicegpt-0.0.6/src/nicegpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-23 03:19:07.000000 nicegpt-0.0.6/src/nicegpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-23 03:19:07.000000 nicegpt-0.0.6/src/nicegpt.egg-info/top_level.txt
```

### Comparing `nicegpt-0.0.5/LICENSE` & `nicegpt-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nicegpt-0.0.5/PKG-INFO` & `nicegpt-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicegpt
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple package to make GPT API usage easier
 Author-email: Samuel Reeder <samuel.reeder@mail.utoronto.ca>
 License: MIT License
         
         Copyright (c) 2023 Samuel Reeder
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nicegpt-0.0.5/README.md` & `nicegpt-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nicegpt-0.0.5/pyproject.toml` & `nicegpt-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nicegpt"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Samuel Reeder", email="samuel.reeder@mail.utoronto.ca" },
 ]
 description = "A simple package to make GPT API usage easier"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
```

### Comparing `nicegpt-0.0.5/src/nicegpt/nicegpt.py` & `nicegpt-0.0.6/src/nicegpt/nicegpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     _system: str
     _cost: float
     messages: list[list]
     cost: str
     prompt_tokens: int
     completion_tokens: int
 
-    def __init__(self, model: Model = Model.GPT_3, system: str = None) -> None:
+    def __init__(self, model: Model = Model.GPT3_5, system: str = None) -> None:
         """
         Initiates an instance of a GPT model. Provide the GPT model you would like to use by accessing the <gpt.Model> enum and optionally provide a system prompt.
         """
         self.change_model(model)
         self._system = system
         self._cost = 0.0 
         self.messages = []
```

### Comparing `nicegpt-0.0.5/src/nicegpt.egg-info/PKG-INFO` & `nicegpt-0.0.6/src/nicegpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicegpt
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple package to make GPT API usage easier
 Author-email: Samuel Reeder <samuel.reeder@mail.utoronto.ca>
 License: MIT License
         
         Copyright (c) 2023 Samuel Reeder
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

