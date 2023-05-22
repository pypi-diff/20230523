# Comparing `tmp/llmo-0.1.6.tar.gz` & `tmp/llmo-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmo-0.1.6.tar", last modified: Mon May 22 21:37:44 2023, max compression
+gzip compressed data, was "llmo-0.1.7.tar", last modified: Mon May 22 22:05:31 2023, max compression
```

## Comparing `llmo-0.1.6.tar` & `llmo-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,11 @@
--rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.1.6/LICENSE
--rw-r--r--   0        0        0     2134 2023-05-22 08:06:19.890271 llmo-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.1.6/llmo/__init__.py
--rw-r--r--   0        0        0    18574 2023-05-22 21:37:00.363982 llmo-0.1.6/llmo/chat.py
--rw-r--r--   0        0        0      353 2023-05-21 18:43:49.180818 llmo-0.1.6/llmo/layout.css
--rw-r--r--   0        0        0      680 2023-05-22 21:37:44.394393 llmo-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2479 1970-01-01 00:00:00.000000 llmo-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2134 2023-05-22 08:06:19.890271 llmo-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.1.7/llmo/__init__.py
+-rw-r--r--   0        0        0     2901 2023-05-22 22:03:31.776068 llmo-0.1.7/llmo/cli.py
+-rw-r--r--   0        0        0      122 2023-05-22 21:51:03.475865 llmo-0.1.7/llmo/constants.py
+-rw-r--r--   0        0        0     9088 2023-05-22 22:03:50.349449 llmo-0.1.7/llmo/gui.py
+-rw-r--r--   0        0        0      353 2023-05-21 18:43:49.180818 llmo-0.1.7/llmo/layout.css
+-rw-r--r--   0        0        0     5878 2023-05-22 21:51:03.478418 llmo-0.1.7/llmo/llms.py
+-rw-r--r--   0        0        0     1045 2023-05-22 22:03:50.352845 llmo-0.1.7/llmo/shell_mode.py
+-rw-r--r--   0        0        0      678 2023-05-22 22:05:31.495671 llmo-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2479 1970-01-01 00:00:00.000000 llmo-0.1.7/PKG-INFO
```

### Comparing `llmo-0.1.6/LICENSE` & `llmo-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `llmo-0.1.6/README.md` & `llmo-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `llmo-0.1.6/pyproject.toml` & `llmo-0.1.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llmo"
-version = "0.1.6"
+version = "0.1.7"
 description = "AI pair programmer"
 authors = [
     { name = "Stephan Fitzpatrick", email = "stephan@knowsuchagency.com" },
 ]
 dependencies = [
     "textual>=0.26.0",
     "openai>=0.27.6",
@@ -15,16 +15,16 @@
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 Source = "https://github.com/knowsuchagency/llmo"
 
 [project.scripts]
-llmo = "llmo.chat:main"
-lm = "llmo.chat:main"
+llmo = "llmo.cli:main"
+lm = "llmo.cli:main"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `llmo-0.1.6/PKG-INFO` & `llmo-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmo
-Version: 0.1.6
+Version: 0.1.7
 Summary: AI pair programmer
 Author-Email: Stephan Fitzpatrick <stephan@knowsuchagency.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/knowsuchagency/llmo
 Requires-Python: >=3.10
 Requires-Dist: textual>=0.26.0
 Requires-Dist: openai>=0.27.6
```

