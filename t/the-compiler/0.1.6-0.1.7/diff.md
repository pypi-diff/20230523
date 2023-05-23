# Comparing `tmp/the-compiler-0.1.6.tar.gz` & `tmp/the-compiler-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "the-compiler-0.1.6.tar", last modified: Tue May 23 01:17:28 2023, max compression
+gzip compressed data, was "the-compiler-0.1.7.tar", last modified: Tue May 23 05:05:22 2023, max compression
```

## Comparing `the-compiler-0.1.6.tar` & `the-compiler-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:17:28.273873 the-compiler-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 01:17:11.000000 the-compiler-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-23 01:17:28.273873 the-compiler-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-05-23 01:17:11.000000 the-compiler-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 01:17:28.273873 the-compiler-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-23 01:17:11.000000 the-compiler-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:17:28.269873 the-compiler-0.1.6/the_compiler/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-23 01:17:11.000000 the-compiler-0.1.6/the_compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-23 01:17:11.000000 the-compiler-0.1.6/the_compiler/the_compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:17:28.273873 the-compiler-0.1.6/the_compiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-23 01:17:28.000000 the-compiler-0.1.6/the_compiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-23 01:17:28.000000 the-compiler-0.1.6/the_compiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 01:17:28.000000 the-compiler-0.1.6/the_compiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 01:17:28.000000 the-compiler-0.1.6/the_compiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 01:17:28.000000 the-compiler-0.1.6/the_compiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:05:22.168552 the-compiler-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 05:05:11.000000 the-compiler-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-23 05:05:22.168552 the-compiler-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-05-23 05:05:11.000000 the-compiler-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 05:05:22.168552 the-compiler-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-23 05:05:11.000000 the-compiler-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:05:22.168552 the-compiler-0.1.7/the_compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-23 05:05:11.000000 the-compiler-0.1.7/the_compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-23 05:05:11.000000 the-compiler-0.1.7/the_compiler/the_compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:05:22.168552 the-compiler-0.1.7/the_compiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-23 05:05:22.000000 the-compiler-0.1.7/the_compiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-23 05:05:22.000000 the-compiler-0.1.7/the_compiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 05:05:22.000000 the-compiler-0.1.7/the_compiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 05:05:22.000000 the-compiler-0.1.7/the_compiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 05:05:22.000000 the-compiler-0.1.7/the_compiler.egg-info/top_level.txt
```

### Comparing `the-compiler-0.1.6/LICENSE` & `the-compiler-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `the-compiler-0.1.6/PKG-INFO` & `the-compiler-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: the-compiler
-Version: 0.1.6
+Version: 0.1.7
 Summary: The Compiler 
 Home-page: https://github.com/kyegomez/the-compiler
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `the-compiler-0.1.6/setup.py` & `the-compiler-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'the-compiler',
   packages = find_packages(exclude=[]),
-  version = '0.1.6',
+  version = '0.1.7',
   license='MIT',
   description = 'The Compiler ',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/the-compiler',
   keywords = [
```

### Comparing `the-compiler-0.1.6/the_compiler/the_compiler.py` & `the-compiler-0.1.7/the_compiler/the_compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#autonmous agent load balancing add more agents to spec interpreter, add more agents to spec generate or unit tester, default is 3 1 for each, use your own llms, starcoder, reinforcement backed individual agent learning, particle swarm tree of thoughts -> run tree of thoughts on the space of all thoughts ran by agents as trees of an networked swarm system, use autogpt config and env with embedding retriveal search, map all thoughts to an embedding database, while now tester is not done keep running in a while loop, agentgpt with autoforestgpt
+#autonmous agent load balancing add more agents to spec interpreter, add more agents to spec generate or unit tester, default is 3 1 for each, use your own llms, starcoder, reinforcement backed individual agent learning, particle swarm tree of thoughts -> run tree of thoughts on the space of all thoughts ran by agents as trees of an networked swarm system, use autogpt config and env with embedding retriveal search, map all thoughts to an embedding database, while now tester is not done keep running in a while loop, agentgpt with autoforestgpt, program optimizer agent works in unison with the generator to optimize code. Create 5 optimizations for this code: {code}
 #inital implementation of the compiler
 from tree_of_thoughts import OptimizedTreeofThoughts, OptimizedOpenAILanguageModel
 import subprocess
 import json
 import re
 
 class TerminalExecutor:
```

### Comparing `the-compiler-0.1.6/the_compiler.egg-info/PKG-INFO` & `the-compiler-0.1.7/the_compiler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: the-compiler
-Version: 0.1.6
+Version: 0.1.7
 Summary: The Compiler 
 Home-page: https://github.com/kyegomez/the-compiler
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

