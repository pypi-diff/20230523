# Comparing `tmp/hyperfast_python_template-0.5.0.tar.gz` & `tmp/hyperfast_python_template-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfast_python_template-0.5.0.tar", max compression
+gzip compressed data, was "hyperfast_python_template-0.5.1.tar", max compression
```

## Comparing `hyperfast_python_template-0.5.0.tar` & `hyperfast_python_template-0.5.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-05-19 20:33:18.861937 hyperfast_python_template-0.5.0/LICENSE
--rw-r--r--   0        0        0     5490 2023-05-19 20:33:18.861937 hyperfast_python_template-0.5.0/README.md
--rw-r--r--   0        0        0     2991 2023-05-19 20:33:39.062720 hyperfast_python_template-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      323 2023-05-19 20:33:18.861937 hyperfast_python_template-0.5.0/src/hyperfastpy/__cli__.py
--rw-r--r--   0        0        0      135 2023-05-19 20:33:18.861937 hyperfast_python_template-0.5.0/src/hyperfastpy/__init__.py
--rw-r--r--   0        0        0       22 2023-05-19 20:33:39.002717 hyperfast_python_template-0.5.0/src/hyperfastpy/_version.py
--rw-r--r--   0        0        0      272 2023-05-19 20:33:39.002717 hyperfast_python_template-0.5.0/src/hyperfastpy/conf/about/__init__.yaml
--rw-r--r--   0        0        0      243 2023-05-19 20:33:18.861937 hyperfast_python_template-0.5.0/src/hyperfastpy/project.toml
--rw-r--r--   0        0        0        0 2023-05-19 20:33:18.861937 hyperfast_python_template-0.5.0/src/hyperfastpy/py.typed
--rw-r--r--   0        0        0      242 2023-05-19 20:33:18.865937 hyperfast_python_template-0.5.0/src/hyperfastpy/pyproject.toml
--rw-r--r--   0        0        0     6156 1970-01-01 00:00:00.000000 hyperfast_python_template-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-23 05:19:15.994269 hyperfast_python_template-0.5.1/LICENSE
+-rw-r--r--   0        0        0     5490 2023-05-23 05:19:15.994269 hyperfast_python_template-0.5.1/README.md
+-rw-r--r--   0        0        0     2991 2023-05-23 05:19:32.834516 hyperfast_python_template-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      323 2023-05-23 05:19:15.998269 hyperfast_python_template-0.5.1/src/hyperfastpy/__cli__.py
+-rw-r--r--   0        0        0      135 2023-05-23 05:19:15.998269 hyperfast_python_template-0.5.1/src/hyperfastpy/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-23 05:19:32.778514 hyperfast_python_template-0.5.1/src/hyperfastpy/_version.py
+-rw-r--r--   0        0        0      272 2023-05-23 05:19:32.778514 hyperfast_python_template-0.5.1/src/hyperfastpy/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      243 2023-05-23 05:19:15.998269 hyperfast_python_template-0.5.1/src/hyperfastpy/project.toml
+-rw-r--r--   0        0        0        0 2023-05-23 05:19:15.998269 hyperfast_python_template-0.5.1/src/hyperfastpy/py.typed
+-rw-r--r--   0        0        0      242 2023-05-23 05:19:15.998269 hyperfast_python_template-0.5.1/src/hyperfastpy/pyproject.toml
+-rw-r--r--   0        0        0     6156 1970-01-01 00:00:00.000000 hyperfast_python_template-0.5.1/PKG-INFO
```

### Comparing `hyperfast_python_template-0.5.0/LICENSE` & `hyperfast_python_template-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.5.0/README.md` & `hyperfast_python_template-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.5.0/pyproject.toml` & `hyperfast_python_template-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperfast-python-template"
-version = "0.5.0"
+version = "0.5.1"
 description = "A python template that helps you jump start your project"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyperfast-python.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyperfast-python-template"
 readme = "README.md"
 packages = [{ include = "hyperfastpy", from = "src" }]
```

### Comparing `hyperfast_python_template-0.5.0/PKG-INFO` & `hyperfast_python_template-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperfast-python-template
-Version: 0.5.0
+Version: 0.5.1
 Summary: A python template that helps you jump start your project
 Home-page: https://hyperfast-python.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

