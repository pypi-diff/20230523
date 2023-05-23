# Comparing `tmp/openai-tools-0.0.0.1.dev0.tar.gz` & `tmp/openai-tools-0.0.0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-tools-0.0.0.1.dev0.tar", last modified: Thu May  4 03:40:48 2023, max compression
+gzip compressed data, was "openai-tools-0.0.0.1.dev1.tar", last modified: Tue May 23 01:25:46 2023, max compression
```

## Comparing `openai-tools-0.0.0.1.dev0.tar` & `openai-tools-0.0.0.1.dev1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-04 03:40:48.641141 openai-tools-0.0.0.1.dev0/
--rw-r--r--   0 avsolatorio   (501) staff       (20)     3093 2023-05-03 19:41:46.000000 openai-tools-0.0.0.1.dev0/.gitignore
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1075 2023-05-03 19:36:38.000000 openai-tools-0.0.0.1.dev0/LICENSE
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1342 2023-05-04 02:56:41.000000 openai-tools-0.0.0.1.dev0/Makefile
--rw-r--r--   0 avsolatorio   (501) staff       (20)     2187 2023-05-04 03:40:48.640966 openai-tools-0.0.0.1.dev0/PKG-INFO
--rw-r--r--   0 avsolatorio   (501) staff       (20)      236 2023-05-04 02:57:55.000000 openai-tools-0.0.0.1.dev0/Pipfile
--rw-r--r--   0 avsolatorio   (501) staff       (20)       11 2023-05-03 19:36:38.000000 openai-tools-0.0.0.1.dev0/README.md
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1258 2023-05-04 02:59:03.000000 openai-tools-0.0.0.1.dev0/pyproject.toml
--rw-r--r--   0 avsolatorio   (501) staff       (20)       38 2023-05-04 03:40:48.641192 openai-tools-0.0.0.1.dev0/setup.cfg
--rw-r--r--   0 avsolatorio   (501) staff       (20)      128 2023-05-04 02:57:19.000000 openai-tools-0.0.0.1.dev0/setup.py
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-04 03:40:48.638136 openai-tools-0.0.0.1.dev0/src/
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-04 03:40:48.639854 openai-tools-0.0.0.1.dev0/src/openai_tools/
--rw-r--r--   0 avsolatorio   (501) staff       (20)       29 2023-05-04 03:40:07.000000 openai-tools-0.0.0.1.dev0/src/openai_tools/__init__.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)     7162 2023-05-04 03:38:30.000000 openai-tools-0.0.0.1.dev0/src/openai_tools/prompt.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)     2788 2023-05-04 03:26:59.000000 openai-tools-0.0.0.1.dev0/src/openai_tools/utils.py
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-04 03:40:48.640686 openai-tools-0.0.0.1.dev0/src/openai_tools.egg-info/
--rw-r--r--   0 avsolatorio   (501) staff       (20)     2187 2023-05-04 03:40:48.000000 openai-tools-0.0.0.1.dev0/src/openai_tools.egg-info/PKG-INFO
--rw-r--r--   0 avsolatorio   (501) staff       (20)      350 2023-05-04 03:40:48.000000 openai-tools-0.0.0.1.dev0/src/openai_tools.egg-info/SOURCES.txt
--rw-r--r--   0 avsolatorio   (501) staff       (20)        1 2023-05-04 03:40:48.000000 openai-tools-0.0.0.1.dev0/src/openai_tools.egg-info/dependency_links.txt
--rw-r--r--   0 avsolatorio   (501) staff       (20)       72 2023-05-04 03:40:48.000000 openai-tools-0.0.0.1.dev0/src/openai_tools.egg-info/requires.txt
--rw-r--r--   0 avsolatorio   (501) staff       (20)       23 2023-05-04 03:40:48.000000 openai-tools-0.0.0.1.dev0/src/openai_tools.egg-info/top_level.txt
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-23 01:25:46.976559 openai-tools-0.0.0.1.dev1/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     3093 2023-05-03 19:41:46.000000 openai-tools-0.0.0.1.dev1/.gitignore
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1075 2023-05-03 19:36:38.000000 openai-tools-0.0.0.1.dev1/LICENSE
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1342 2023-05-04 02:56:41.000000 openai-tools-0.0.0.1.dev1/Makefile
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     2187 2023-05-23 01:25:46.976365 openai-tools-0.0.0.1.dev1/PKG-INFO
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      236 2023-05-04 02:57:55.000000 openai-tools-0.0.0.1.dev1/Pipfile
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       11 2023-05-03 19:36:38.000000 openai-tools-0.0.0.1.dev1/README.md
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1258 2023-05-04 02:59:03.000000 openai-tools-0.0.0.1.dev1/pyproject.toml
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       38 2023-05-23 01:25:46.976622 openai-tools-0.0.0.1.dev1/setup.cfg
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      128 2023-05-04 02:57:19.000000 openai-tools-0.0.0.1.dev1/setup.py
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-23 01:25:46.972672 openai-tools-0.0.0.1.dev1/src/
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-23 01:25:46.975160 openai-tools-0.0.0.1.dev1/src/openai_tools/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       29 2023-05-23 01:25:23.000000 openai-tools-0.0.0.1.dev1/src/openai_tools/__init__.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      778 2023-05-23 01:24:37.000000 openai-tools-0.0.0.1.dev1/src/openai_tools/parser.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     7162 2023-05-04 03:38:30.000000 openai-tools-0.0.0.1.dev1/src/openai_tools/prompt.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     2788 2023-05-04 03:26:59.000000 openai-tools-0.0.0.1.dev1/src/openai_tools/utils.py
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-23 01:25:46.976089 openai-tools-0.0.0.1.dev1/src/openai_tools.egg-info/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     2187 2023-05-23 01:25:46.000000 openai-tools-0.0.0.1.dev1/src/openai_tools.egg-info/PKG-INFO
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      377 2023-05-23 01:25:46.000000 openai-tools-0.0.0.1.dev1/src/openai_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 avsolatorio   (501) staff       (20)        1 2023-05-23 01:25:46.000000 openai-tools-0.0.0.1.dev1/src/openai_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       72 2023-05-23 01:25:46.000000 openai-tools-0.0.0.1.dev1/src/openai_tools.egg-info/requires.txt
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       23 2023-05-23 01:25:46.000000 openai-tools-0.0.0.1.dev1/src/openai_tools.egg-info/top_level.txt
```

### Comparing `openai-tools-0.0.0.1.dev0/.gitignore` & `openai-tools-0.0.0.1.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `openai-tools-0.0.0.1.dev0/LICENSE` & `openai-tools-0.0.0.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai-tools-0.0.0.1.dev0/Makefile` & `openai-tools-0.0.0.1.dev1/Makefile`

 * *Files identical despite different names*

### Comparing `openai-tools-0.0.0.1.dev0/PKG-INFO` & `openai-tools-0.0.0.1.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-tools
-Version: 0.0.0.1.dev0
+Version: 0.0.0.1.dev1
 Summary: A Python wrapper for managing OpenAI API.
 Author-email: "Aivin V. Solatorio" <avsolatorio@gmail.com>
 Maintainer-email: "Aivin V. Solatorio" <avsolatorio@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Aivin V. Solatorio
```

### Comparing `openai-tools-0.0.0.1.dev0/pyproject.toml` & `openai-tools-0.0.0.1.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openai-tools-0.0.0.1.dev0/src/openai_tools/prompt.py` & `openai-tools-0.0.0.1.dev1/src/openai_tools/prompt.py`

 * *Files identical despite different names*

### Comparing `openai-tools-0.0.0.1.dev0/src/openai_tools/utils.py` & `openai-tools-0.0.0.1.dev1/src/openai_tools/utils.py`

 * *Files identical despite different names*

### Comparing `openai-tools-0.0.0.1.dev0/src/openai_tools.egg-info/PKG-INFO` & `openai-tools-0.0.0.1.dev1/src/openai_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-tools
-Version: 0.0.0.1.dev0
+Version: 0.0.0.1.dev1
 Summary: A Python wrapper for managing OpenAI API.
 Author-email: "Aivin V. Solatorio" <avsolatorio@gmail.com>
 Maintainer-email: "Aivin V. Solatorio" <avsolatorio@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Aivin V. Solatorio
```

