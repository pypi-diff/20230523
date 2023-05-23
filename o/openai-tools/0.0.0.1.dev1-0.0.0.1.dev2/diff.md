# Comparing `tmp/openai-tools-0.0.0.1.dev1.tar.gz` & `tmp/openai-tools-0.0.0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-tools-0.0.0.1.dev1.tar", last modified: Tue May 23 01:25:46 2023, max compression
+gzip compressed data, was "openai-tools-0.0.0.1.dev2.tar", last modified: Tue May 23 01:53:09 2023, max compression
```

## Comparing `openai-tools-0.0.0.1.dev1.tar` & `openai-tools-0.0.0.1.dev2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-23 01:25:46.976559 openai-tools-0.0.0.1.dev1/
--rw-r--r--   0 avsolatorio   (501) staff       (20)     3093 2023-05-03 19:41:46.000000 openai-tools-0.0.0.1.dev1/.gitignore
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1075 2023-05-03 19:36:38.000000 openai-tools-0.0.0.1.dev1/LICENSE
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1342 2023-05-04 02:56:41.000000 openai-tools-0.0.0.1.dev1/Makefile
--rw-r--r--   0 avsolatorio   (501) staff       (20)     2187 2023-05-23 01:25:46.976365 openai-tools-0.0.0.1.dev1/PKG-INFO
--rw-r--r--   0 avsolatorio   (501) staff       (20)      236 2023-05-04 02:57:55.000000 openai-tools-0.0.0.1.dev1/Pipfile
--rw-r--r--   0 avsolatorio   (501) staff       (20)       11 2023-05-03 19:36:38.000000 openai-tools-0.0.0.1.dev1/README.md
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1258 2023-05-04 02:59:03.000000 openai-tools-0.0.0.1.dev1/pyproject.toml
--rw-r--r--   0 avsolatorio   (501) staff       (20)       38 2023-05-23 01:25:46.976622 openai-tools-0.0.0.1.dev1/setup.cfg
--rw-r--r--   0 avsolatorio   (501) staff       (20)      128 2023-05-04 02:57:19.000000 openai-tools-0.0.0.1.dev1/setup.py
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-23 01:25:46.972672 openai-tools-0.0.0.1.dev1/src/
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-23 01:25:46.975160 openai-tools-0.0.0.1.dev1/src/openai_tools/
--rw-r--r--   0 avsolatorio   (501) staff       (20)       29 2023-05-23 01:25:23.000000 openai-tools-0.0.0.1.dev1/src/openai_tools/__init__.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)      778 2023-05-23 01:24:37.000000 openai-tools-0.0.0.1.dev1/src/openai_tools/parser.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)     7162 2023-05-04 03:38:30.000000 openai-tools-0.0.0.1.dev1/src/openai_tools/prompt.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)     2788 2023-05-04 03:26:59.000000 openai-tools-0.0.0.1.dev1/src/openai_tools/utils.py
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-23 01:25:46.976089 openai-tools-0.0.0.1.dev1/src/openai_tools.egg-info/
--rw-r--r--   0 avsolatorio   (501) staff       (20)     2187 2023-05-23 01:25:46.000000 openai-tools-0.0.0.1.dev1/src/openai_tools.egg-info/PKG-INFO
--rw-r--r--   0 avsolatorio   (501) staff       (20)      377 2023-05-23 01:25:46.000000 openai-tools-0.0.0.1.dev1/src/openai_tools.egg-info/SOURCES.txt
--rw-r--r--   0 avsolatorio   (501) staff       (20)        1 2023-05-23 01:25:46.000000 openai-tools-0.0.0.1.dev1/src/openai_tools.egg-info/dependency_links.txt
--rw-r--r--   0 avsolatorio   (501) staff       (20)       72 2023-05-23 01:25:46.000000 openai-tools-0.0.0.1.dev1/src/openai_tools.egg-info/requires.txt
--rw-r--r--   0 avsolatorio   (501) staff       (20)       23 2023-05-23 01:25:46.000000 openai-tools-0.0.0.1.dev1/src/openai_tools.egg-info/top_level.txt
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-23 01:53:09.528922 openai-tools-0.0.0.1.dev2/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     3093 2023-05-03 19:41:46.000000 openai-tools-0.0.0.1.dev2/.gitignore
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1075 2023-05-03 19:36:38.000000 openai-tools-0.0.0.1.dev2/LICENSE
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1342 2023-05-04 02:56:41.000000 openai-tools-0.0.0.1.dev2/Makefile
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     2187 2023-05-23 01:53:09.528706 openai-tools-0.0.0.1.dev2/PKG-INFO
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      236 2023-05-04 02:57:55.000000 openai-tools-0.0.0.1.dev2/Pipfile
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       11 2023-05-03 19:36:38.000000 openai-tools-0.0.0.1.dev2/README.md
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1258 2023-05-04 02:59:03.000000 openai-tools-0.0.0.1.dev2/pyproject.toml
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       38 2023-05-23 01:53:09.528981 openai-tools-0.0.0.1.dev2/setup.cfg
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      128 2023-05-04 02:57:19.000000 openai-tools-0.0.0.1.dev2/setup.py
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-23 01:53:09.524870 openai-tools-0.0.0.1.dev2/src/
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-23 01:53:09.527495 openai-tools-0.0.0.1.dev2/src/openai_tools/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       29 2023-05-23 01:52:58.000000 openai-tools-0.0.0.1.dev2/src/openai_tools/__init__.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      850 2023-05-23 01:52:52.000000 openai-tools-0.0.0.1.dev2/src/openai_tools/parser.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     7162 2023-05-04 03:38:30.000000 openai-tools-0.0.0.1.dev2/src/openai_tools/prompt.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     2788 2023-05-04 03:26:59.000000 openai-tools-0.0.0.1.dev2/src/openai_tools/utils.py
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-23 01:53:09.528427 openai-tools-0.0.0.1.dev2/src/openai_tools.egg-info/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     2187 2023-05-23 01:53:09.000000 openai-tools-0.0.0.1.dev2/src/openai_tools.egg-info/PKG-INFO
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      377 2023-05-23 01:53:09.000000 openai-tools-0.0.0.1.dev2/src/openai_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 avsolatorio   (501) staff       (20)        1 2023-05-23 01:53:09.000000 openai-tools-0.0.0.1.dev2/src/openai_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       72 2023-05-23 01:53:09.000000 openai-tools-0.0.0.1.dev2/src/openai_tools.egg-info/requires.txt
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       23 2023-05-23 01:53:09.000000 openai-tools-0.0.0.1.dev2/src/openai_tools.egg-info/top_level.txt
```

### Comparing `openai-tools-0.0.0.1.dev1/.gitignore` & `openai-tools-0.0.0.1.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `openai-tools-0.0.0.1.dev1/LICENSE` & `openai-tools-0.0.0.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `openai-tools-0.0.0.1.dev1/Makefile` & `openai-tools-0.0.0.1.dev2/Makefile`

 * *Files identical despite different names*

### Comparing `openai-tools-0.0.0.1.dev1/PKG-INFO` & `openai-tools-0.0.0.1.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-tools
-Version: 0.0.0.1.dev1
+Version: 0.0.0.1.dev2
 Summary: A Python wrapper for managing OpenAI API.
 Author-email: "Aivin V. Solatorio" <avsolatorio@gmail.com>
 Maintainer-email: "Aivin V. Solatorio" <avsolatorio@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Aivin V. Solatorio
```

### Comparing `openai-tools-0.0.0.1.dev1/pyproject.toml` & `openai-tools-0.0.0.1.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openai-tools-0.0.0.1.dev1/src/openai_tools/parser.py` & `openai-tools-0.0.0.1.dev2/src/openai_tools/parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any
 import json
 
 
-def parse_misparsed(text: str, open: str = None, close: str = None, normalize_newline: bool = True) -> Any:
+def parse_misparsed(text: str, open: str = None, close: str = None, normalize_newline: bool = True, to_json: bool = True) -> Any:
     """Parse misparsed JSON.
     Args:
         text (str): The text to parse.
         open (str, optional): The open character. Defaults to None.
         close (str, optional): The close character. Defaults to None.
     Returns:
         JSON: The parsed JSON.
@@ -22,8 +22,11 @@
         text = text[start:end]
     except ValueError:
         text = text
 
     if normalize_newline:
         text = text.replace('\\n', '\n').replace("\n", "\\n")
 
-    return json.loads(text)
+    if to_json:
+        return json.loads(text)
+    else:
+        return text
```

### Comparing `openai-tools-0.0.0.1.dev1/src/openai_tools/prompt.py` & `openai-tools-0.0.0.1.dev2/src/openai_tools/prompt.py`

 * *Files identical despite different names*

### Comparing `openai-tools-0.0.0.1.dev1/src/openai_tools/utils.py` & `openai-tools-0.0.0.1.dev2/src/openai_tools/utils.py`

 * *Files identical despite different names*

### Comparing `openai-tools-0.0.0.1.dev1/src/openai_tools.egg-info/PKG-INFO` & `openai-tools-0.0.0.1.dev2/src/openai_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-tools
-Version: 0.0.0.1.dev1
+Version: 0.0.0.1.dev2
 Summary: A Python wrapper for managing OpenAI API.
 Author-email: "Aivin V. Solatorio" <avsolatorio@gmail.com>
 Maintainer-email: "Aivin V. Solatorio" <avsolatorio@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Aivin V. Solatorio
```

