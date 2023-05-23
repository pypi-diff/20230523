# Comparing `tmp/openai-tools-0.0.0.1.dev2.tar.gz` & `tmp/openai-tools-0.0.0.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-tools-0.0.0.1.dev2.tar", last modified: Tue May 23 01:53:09 2023, max compression
+gzip compressed data, was "openai-tools-0.0.0.1.dev3.tar", last modified: Tue May 23 02:17:27 2023, max compression
```

## Comparing `openai-tools-0.0.0.1.dev2.tar` & `openai-tools-0.0.0.1.dev3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-23 01:53:09.528922 openai-tools-0.0.0.1.dev2/
--rw-r--r--   0 avsolatorio   (501) staff       (20)     3093 2023-05-03 19:41:46.000000 openai-tools-0.0.0.1.dev2/.gitignore
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1075 2023-05-03 19:36:38.000000 openai-tools-0.0.0.1.dev2/LICENSE
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1342 2023-05-04 02:56:41.000000 openai-tools-0.0.0.1.dev2/Makefile
--rw-r--r--   0 avsolatorio   (501) staff       (20)     2187 2023-05-23 01:53:09.528706 openai-tools-0.0.0.1.dev2/PKG-INFO
--rw-r--r--   0 avsolatorio   (501) staff       (20)      236 2023-05-04 02:57:55.000000 openai-tools-0.0.0.1.dev2/Pipfile
--rw-r--r--   0 avsolatorio   (501) staff       (20)       11 2023-05-03 19:36:38.000000 openai-tools-0.0.0.1.dev2/README.md
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1258 2023-05-04 02:59:03.000000 openai-tools-0.0.0.1.dev2/pyproject.toml
--rw-r--r--   0 avsolatorio   (501) staff       (20)       38 2023-05-23 01:53:09.528981 openai-tools-0.0.0.1.dev2/setup.cfg
--rw-r--r--   0 avsolatorio   (501) staff       (20)      128 2023-05-04 02:57:19.000000 openai-tools-0.0.0.1.dev2/setup.py
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-23 01:53:09.524870 openai-tools-0.0.0.1.dev2/src/
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-23 01:53:09.527495 openai-tools-0.0.0.1.dev2/src/openai_tools/
--rw-r--r--   0 avsolatorio   (501) staff       (20)       29 2023-05-23 01:52:58.000000 openai-tools-0.0.0.1.dev2/src/openai_tools/__init__.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)      850 2023-05-23 01:52:52.000000 openai-tools-0.0.0.1.dev2/src/openai_tools/parser.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)     7162 2023-05-04 03:38:30.000000 openai-tools-0.0.0.1.dev2/src/openai_tools/prompt.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)     2788 2023-05-04 03:26:59.000000 openai-tools-0.0.0.1.dev2/src/openai_tools/utils.py
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-23 01:53:09.528427 openai-tools-0.0.0.1.dev2/src/openai_tools.egg-info/
--rw-r--r--   0 avsolatorio   (501) staff       (20)     2187 2023-05-23 01:53:09.000000 openai-tools-0.0.0.1.dev2/src/openai_tools.egg-info/PKG-INFO
--rw-r--r--   0 avsolatorio   (501) staff       (20)      377 2023-05-23 01:53:09.000000 openai-tools-0.0.0.1.dev2/src/openai_tools.egg-info/SOURCES.txt
--rw-r--r--   0 avsolatorio   (501) staff       (20)        1 2023-05-23 01:53:09.000000 openai-tools-0.0.0.1.dev2/src/openai_tools.egg-info/dependency_links.txt
--rw-r--r--   0 avsolatorio   (501) staff       (20)       72 2023-05-23 01:53:09.000000 openai-tools-0.0.0.1.dev2/src/openai_tools.egg-info/requires.txt
--rw-r--r--   0 avsolatorio   (501) staff       (20)       23 2023-05-23 01:53:09.000000 openai-tools-0.0.0.1.dev2/src/openai_tools.egg-info/top_level.txt
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-23 02:17:27.743876 openai-tools-0.0.0.1.dev3/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     3093 2023-05-03 19:41:46.000000 openai-tools-0.0.0.1.dev3/.gitignore
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1075 2023-05-03 19:36:38.000000 openai-tools-0.0.0.1.dev3/LICENSE
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1342 2023-05-04 02:56:41.000000 openai-tools-0.0.0.1.dev3/Makefile
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     2187 2023-05-23 02:17:27.743687 openai-tools-0.0.0.1.dev3/PKG-INFO
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      236 2023-05-04 02:57:55.000000 openai-tools-0.0.0.1.dev3/Pipfile
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       11 2023-05-03 19:36:38.000000 openai-tools-0.0.0.1.dev3/README.md
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1258 2023-05-04 02:59:03.000000 openai-tools-0.0.0.1.dev3/pyproject.toml
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       38 2023-05-23 02:17:27.743935 openai-tools-0.0.0.1.dev3/setup.cfg
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      128 2023-05-04 02:57:19.000000 openai-tools-0.0.0.1.dev3/setup.py
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-23 02:17:27.740072 openai-tools-0.0.0.1.dev3/src/
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-23 02:17:27.742504 openai-tools-0.0.0.1.dev3/src/openai_tools/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       29 2023-05-23 02:16:57.000000 openai-tools-0.0.0.1.dev3/src/openai_tools/__init__.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1212 2023-05-23 02:16:42.000000 openai-tools-0.0.0.1.dev3/src/openai_tools/parser.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     7162 2023-05-04 03:38:30.000000 openai-tools-0.0.0.1.dev3/src/openai_tools/prompt.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     2788 2023-05-04 03:26:59.000000 openai-tools-0.0.0.1.dev3/src/openai_tools/utils.py
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-23 02:17:27.743416 openai-tools-0.0.0.1.dev3/src/openai_tools.egg-info/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     2187 2023-05-23 02:17:27.000000 openai-tools-0.0.0.1.dev3/src/openai_tools.egg-info/PKG-INFO
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      377 2023-05-23 02:17:27.000000 openai-tools-0.0.0.1.dev3/src/openai_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 avsolatorio   (501) staff       (20)        1 2023-05-23 02:17:27.000000 openai-tools-0.0.0.1.dev3/src/openai_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       72 2023-05-23 02:17:27.000000 openai-tools-0.0.0.1.dev3/src/openai_tools.egg-info/requires.txt
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       23 2023-05-23 02:17:27.000000 openai-tools-0.0.0.1.dev3/src/openai_tools.egg-info/top_level.txt
```

### Comparing `openai-tools-0.0.0.1.dev2/.gitignore` & `openai-tools-0.0.0.1.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `openai-tools-0.0.0.1.dev2/LICENSE` & `openai-tools-0.0.0.1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `openai-tools-0.0.0.1.dev2/Makefile` & `openai-tools-0.0.0.1.dev3/Makefile`

 * *Files identical despite different names*

### Comparing `openai-tools-0.0.0.1.dev2/PKG-INFO` & `openai-tools-0.0.0.1.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-tools
-Version: 0.0.0.1.dev2
+Version: 0.0.0.1.dev3
 Summary: A Python wrapper for managing OpenAI API.
 Author-email: "Aivin V. Solatorio" <avsolatorio@gmail.com>
 Maintainer-email: "Aivin V. Solatorio" <avsolatorio@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Aivin V. Solatorio
```

### Comparing `openai-tools-0.0.0.1.dev2/pyproject.toml` & `openai-tools-0.0.0.1.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openai-tools-0.0.0.1.dev2/src/openai_tools/prompt.py` & `openai-tools-0.0.0.1.dev3/src/openai_tools/prompt.py`

 * *Files identical despite different names*

### Comparing `openai-tools-0.0.0.1.dev2/src/openai_tools/utils.py` & `openai-tools-0.0.0.1.dev3/src/openai_tools/utils.py`

 * *Files identical despite different names*

### Comparing `openai-tools-0.0.0.1.dev2/src/openai_tools.egg-info/PKG-INFO` & `openai-tools-0.0.0.1.dev3/src/openai_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-tools
-Version: 0.0.0.1.dev2
+Version: 0.0.0.1.dev3
 Summary: A Python wrapper for managing OpenAI API.
 Author-email: "Aivin V. Solatorio" <avsolatorio@gmail.com>
 Maintainer-email: "Aivin V. Solatorio" <avsolatorio@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Aivin V. Solatorio
```

