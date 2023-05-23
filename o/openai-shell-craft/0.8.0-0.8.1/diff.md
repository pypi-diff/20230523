# Comparing `tmp/openai_shell_craft-0.8.0.tar.gz` & `tmp/openai_shell_craft-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_shell_craft-0.8.0.tar", last modified: Tue May 16 01:40:00 2023, max compression
+gzip compressed data, was "openai_shell_craft-0.8.1.tar", last modified: Tue May 23 16:54:22 2023, max compression
```

## Comparing `openai_shell_craft-0.8.0.tar` & `openai_shell_craft-0.8.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:40:00.428236 openai_shell_craft-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-05-16 01:40:00.428236 openai_shell_craft-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:40:00.424236 openai_shell_craft-0.8.0/openai_shell_craft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-05-16 01:40:00.000000 openai_shell_craft-0.8.0/openai_shell_craft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-16 01:40:00.000000 openai_shell_craft-0.8.0/openai_shell_craft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 01:40:00.000000 openai_shell_craft-0.8.0/openai_shell_craft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 01:40:00.000000 openai_shell_craft-0.8.0/openai_shell_craft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 01:40:00.000000 openai_shell_craft-0.8.0/openai_shell_craft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 01:40:00.000000 openai_shell_craft-0.8.0/openai_shell_craft.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 01:40:00.428236 openai_shell_craft-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:40:00.424236 openai_shell_craft-0.8.0/shell_craft/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:40:00.428236 openai_shell_craft-0.8.0/shell_craft/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/help.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:40:00.428236 openai_shell_craft-0.8.0/shell_craft/factories/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/factories/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:40:00.428236 openai_shell_craft-0.8.0/shell_craft/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/prompts/languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/prompts/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/prompts/templates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3388 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:40:00.428236 openai_shell_craft-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/tests/test_factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:54:22.930449 openai_shell_craft-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-05-23 16:54:22.930449 openai_shell_craft-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:54:22.922449 openai_shell_craft-0.8.1/openai_shell_craft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-05-23 16:54:22.000000 openai_shell_craft-0.8.1/openai_shell_craft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-23 16:54:22.000000 openai_shell_craft-0.8.1/openai_shell_craft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:54:22.000000 openai_shell_craft-0.8.1/openai_shell_craft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-23 16:54:22.000000 openai_shell_craft-0.8.1/openai_shell_craft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 16:54:22.000000 openai_shell_craft-0.8.1/openai_shell_craft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 16:54:22.000000 openai_shell_craft-0.8.1/openai_shell_craft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 16:54:22.930449 openai_shell_craft-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:54:22.922449 openai_shell_craft-0.8.1/shell_craft/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/shell_craft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/shell_craft/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:54:22.926449 openai_shell_craft-0.8.1/shell_craft/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/shell_craft/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/shell_craft/cli/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/shell_craft/cli/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/shell_craft/cli/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/shell_craft/cli/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/shell_craft/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/shell_craft/cli/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/shell_craft/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/shell_craft/cli/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/shell_craft/cli/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/shell_craft/cli/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:54:22.926449 openai_shell_craft-0.8.1/shell_craft/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/shell_craft/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/shell_craft/factories/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:54:22.930449 openai_shell_craft-0.8.1/shell_craft/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/shell_craft/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/shell_craft/prompts/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/shell_craft/prompts/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/shell_craft/prompts/templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3388 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/shell_craft/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:54:22.930449 openai_shell_craft-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-23 16:54:11.000000 openai_shell_craft-0.8.1/tests/test_factories.py
```

### Comparing `openai_shell_craft-0.8.0/LICENSE` & `openai_shell_craft-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/PKG-INFO` & `openai_shell_craft-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_shell_craft
-Version: 0.8.0
+Version: 0.8.1
 Summary: Generating shell commands and code using natural language models (OpenAI ChatGPT).
 Author-email: Johnathan Irvin <irvinjohnathan@gmail.com>
 Project-URL: Homepage, https://github.com/JohnnyIrvin/shell-craft
 Project-URL: Bug Tracker, https://github.com/JohnnyIrvin/shell-craft/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai_shell_craft-0.8.0/README.md` & `openai_shell_craft-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/openai_shell_craft.egg-info/PKG-INFO` & `openai_shell_craft-0.8.1/openai_shell_craft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-shell-craft
-Version: 0.8.0
+Version: 0.8.1
 Summary: Generating shell commands and code using natural language models (OpenAI ChatGPT).
 Author-email: Johnathan Irvin <irvinjohnathan@gmail.com>
 Project-URL: Homepage, https://github.com/JohnnyIrvin/shell-craft
 Project-URL: Bug Tracker, https://github.com/JohnnyIrvin/shell-craft/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai_shell_craft-0.8.0/openai_shell_craft.egg-info/SOURCES.txt` & `openai_shell_craft-0.8.1/openai_shell_craft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/pyproject.toml` & `openai_shell_craft-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openai_shell_craft"
-version = "0.8.0"
+version = "0.8.1"
 authors = [
   { name="Johnathan Irvin", email="irvinjohnathan@gmail.com" },
 ]
 description = "Generating shell commands and code using natural language models (OpenAI ChatGPT)."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `openai_shell_craft-0.8.0/shell_craft/__init__.py` & `openai_shell_craft-0.8.1/shell_craft/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/shell_craft/__main__.py` & `openai_shell_craft-0.8.1/shell_craft/__main__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/shell_craft/cli/__init__.py` & `openai_shell_craft-0.8.1/shell_craft/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/shell_craft/cli/github.py` & `openai_shell_craft-0.8.1/shell_craft/cli/github.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/shell_craft/cli/help.py` & `openai_shell_craft-0.8.1/shell_craft/cli/help.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/shell_craft/cli/key.py` & `openai_shell_craft-0.8.1/shell_craft/cli/key.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/shell_craft/cli/language.py` & `openai_shell_craft-0.8.1/shell_craft/cli/language.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/shell_craft/cli/main.py` & `openai_shell_craft-0.8.1/shell_craft/cli/main.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/shell_craft/cli/models.py` & `openai_shell_craft-0.8.1/shell_craft/cli/models.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/shell_craft/cli/parser.py` & `openai_shell_craft-0.8.1/shell_craft/cli/parser.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/shell_craft/cli/prompt.py` & `openai_shell_craft-0.8.1/shell_craft/cli/prompt.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/shell_craft/cli/request.py` & `openai_shell_craft-0.8.1/shell_craft/cli/request.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/shell_craft/cli/results.py` & `openai_shell_craft-0.8.1/shell_craft/cli/results.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/shell_craft/factories/__init__.py` & `openai_shell_craft-0.8.1/shell_craft/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/shell_craft/factories/prompt.py` & `openai_shell_craft-0.8.1/shell_craft/factories/prompt.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/shell_craft/prompts/__init__.py` & `openai_shell_craft-0.8.1/shell_craft/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/shell_craft/prompts/languages.py` & `openai_shell_craft-0.8.1/shell_craft/prompts/languages.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/shell_craft/prompts/prompt.py` & `openai_shell_craft-0.8.1/shell_craft/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/shell_craft/prompts/templates.py` & `openai_shell_craft-0.8.1/shell_craft/prompts/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,8 +60,8 @@
 1. Go to '...'
 2. Click on '....'
 3. Scroll down to '....'
 4. See error
 
 **Expected behavior**
 A clear and concise description of what you expected to happen.
-""")
+```""")
```

### Comparing `openai_shell_craft-0.8.0/shell_craft/service.py` & `openai_shell_craft-0.8.1/shell_craft/service.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/tests/test_cli.py` & `openai_shell_craft-0.8.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.0/tests/test_factories.py` & `openai_shell_craft-0.8.1/tests/test_factories.py`

 * *Files identical despite different names*

