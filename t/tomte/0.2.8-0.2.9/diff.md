# Comparing `tmp/tomte-0.2.8.tar.gz` & `tmp/tomte-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomte-0.2.8.tar", max compression
+gzip compressed data, was "tomte-0.2.9.tar", max compression
```

## Comparing `tomte-0.2.8.tar` & `tomte-0.2.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1063 2022-10-01 14:11:14.626018 tomte-0.2.8/LICENSE
--rw-r--r--   0        0        0     2856 2023-05-21 20:23:04.326638 tomte-0.2.8/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-21 20:23:10.250010 tomte-0.2.8/tomte/__init__.py
--rw-r--r--   0        0        0     2871 2023-05-21 20:21:36.335344 tomte-0.2.8/tomte/cli.py
--rw-r--r--   0        0        0      876 2022-09-11 16:56:11.417175 tomte-0.2.8/tomte/tools/__init__.py
--rwxr-xr-x   0        0        0    11139 2023-05-21 16:09:32.802247 tomte-0.2.8/tomte/tools/check_copyright.py
--rwxr-xr-x   0        0        0     6964 2023-05-21 16:10:52.628522 tomte-0.2.8/tomte/tools/check_doc_links.py
--rwxr-xr-x   0        0        0     1678 2023-05-21 10:59:04.565876 tomte-0.2.8/tomte/tools/check_readme.py
--rwxr-xr-x   0        0        0     1348 2023-05-21 15:29:26.914379 tomte-0.2.8/tomte/tools/freeze_dependencies.py
--rw-r--r--   0        0        0     1937 1970-01-01 00:00:00.000000 tomte-0.2.8/setup.py
--rw-r--r--   0        0        0     2806 1970-01-01 00:00:00.000000 tomte-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2022-10-01 14:11:14.626018 tomte-0.2.9/LICENSE
+-rw-r--r--   0        0        0     2856 2023-05-21 20:33:25.197298 tomte-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-21 20:33:30.263640 tomte-0.2.9/tomte/__init__.py
+-rw-r--r--   0        0        0     2871 2023-05-21 20:31:20.839953 tomte-0.2.9/tomte/cli.py
+-rw-r--r--   0        0        0      876 2022-09-11 16:56:11.417175 tomte-0.2.9/tomte/tools/__init__.py
+-rwxr-xr-x   0        0        0    11139 2023-05-21 16:09:32.802247 tomte-0.2.9/tomte/tools/check_copyright.py
+-rwxr-xr-x   0        0        0     6964 2023-05-21 16:10:52.628522 tomte-0.2.9/tomte/tools/check_doc_links.py
+-rwxr-xr-x   0        0        0     1678 2023-05-21 10:59:04.565876 tomte-0.2.9/tomte/tools/check_readme.py
+-rwxr-xr-x   0        0        0     1363 2023-05-21 20:31:41.182974 tomte-0.2.9/tomte/tools/freeze_dependencies.py
+-rw-r--r--   0        0        0     1937 1970-01-01 00:00:00.000000 tomte-0.2.9/setup.py
+-rw-r--r--   0        0        0     2806 1970-01-01 00:00:00.000000 tomte-0.2.9/PKG-INFO
```

### Comparing `tomte-0.2.8/LICENSE` & `tomte-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tomte-0.2.8/pyproject.toml` & `tomte-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tomte"
-version = "0.2.8"
+version = "0.2.9"
 description = "A library that wraps many useful tools (linters, analysers, etc) to keep Python code clean, secure, well-documented and optimised."
 authors = ["David Minarsch <david.minarsch@googlemail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 tox = {version = "==3.28.0", optional = true}
```

### Comparing `tomte-0.2.8/tomte/cli.py` & `tomte-0.2.9/tomte/cli.py`

 * *Files identical despite different names*

### Comparing `tomte-0.2.8/tomte/tools/__init__.py` & `tomte-0.2.9/tomte/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `tomte-0.2.8/tomte/tools/check_copyright.py` & `tomte-0.2.9/tomte/tools/check_copyright.py`

 * *Files identical despite different names*

### Comparing `tomte-0.2.8/tomte/tools/check_doc_links.py` & `tomte-0.2.9/tomte/tools/check_doc_links.py`

 * *Files identical despite different names*

### Comparing `tomte-0.2.8/tomte/tools/check_readme.py` & `tomte-0.2.9/tomte/tools/check_readme.py`

 * *Files identical despite different names*

### Comparing `tomte-0.2.8/tomte/tools/freeze_dependencies.py` & `tomte-0.2.9/tomte/tools/freeze_dependencies.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 
 """This CLI tool freezes the dependencies."""
 import subprocess  # nosec
 from pathlib import Path
 from typing import Optional
 
 
-def main(output: Optional[str]) -> None:
+def main(output_path: Optional[str]) -> None:
     pip_freeze_call = subprocess.Popen(  # nosec  # pylint: disable=consider-using-with
         ["pip", "freeze"], stdout=subprocess.PIPE
     )
     (stdout, stderr) = pip_freeze_call.communicate()
     requirements = stdout.decode("utf-8")
 
-    if output is None:
+    if output_path is None:
         print(requirements)
     else:
-        path = Path(output)
+        path = Path(output_path)
         path.write_text(requirements)
```

### Comparing `tomte-0.2.8/setup.py` & `tomte-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
  'vulture': ['vulture==2.7']}
 
 entry_points = \
 {'console_scripts': ['tomte = tomte.cli:cli']}
 
 setup_kwargs = {
     'name': 'tomte',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'A library that wraps many useful tools (linters, analysers, etc) to keep Python code clean, secure, well-documented and optimised.',
     'long_description': 'None',
     'author': 'David Minarsch',
     'author_email': 'david.minarsch@googlemail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tomte-0.2.8/PKG-INFO` & `tomte-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomte
-Version: 0.2.8
+Version: 0.2.9
 Summary: A library that wraps many useful tools (linters, analysers, etc) to keep Python code clean, secure, well-documented and optimised.
 License: MIT
 Author: David Minarsch
 Author-email: david.minarsch@googlemail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

