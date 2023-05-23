# Comparing `tmp/flake2lint-0.4.2.tar.gz` & `tmp/flake2lint-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake2lint-0.4.2.tar", last modified: Mon Aug  1 09:04:43 2022, max compression
+gzip compressed data, was "flake2lint-0.4.3.tar", last modified: Tue May 23 14:21:21 2023, max compression
```

## Comparing `flake2lint-0.4.2.tar` & `flake2lint-0.4.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0 runner    (1001) docker     (121)     4534 2022-08-01 09:04:43.138494 flake2lint-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     5946 2022-08-01 09:04:43.138494 flake2lint-0.4.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7484 2022-08-01 09:04:43.138494 flake2lint-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-08-01 09:04:43.130494 flake2lint-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-01 09:04:43.138494 flake2lint-0.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-01 09:04:09.330007 flake2lint-0.4.2/flake2lint/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     4432 2022-08-01 09:04:09.330007 flake2lint-0.4.2/flake2lint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2504 2022-08-01 09:04:09.330007 flake2lint-0.4.2/flake2lint/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5948 2023-05-23 14:21:21.168412 flake2lint-0.4.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-05-23 14:21:21.160412 flake2lint-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-23 14:21:21.168412 flake2lint-0.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7537 2023-05-23 14:21:21.168412 flake2lint-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4588 2023-05-23 14:21:21.168412 flake2lint-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 14:20:49.952651 flake2lint-0.4.3/flake2lint/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-05-23 14:20:49.952651 flake2lint-0.4.3/flake2lint/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4432 2023-05-23 14:20:49.952651 flake2lint-0.4.3/flake2lint/__init__.py
```

### Comparing `flake2lint-0.4.2/pyproject.toml` & `flake2lint-0.4.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "flake2lint"
-version = "0.4.2"
+version = "0.4.3"
 description = "Tool and pre-commit hook to augment Flake8 noqa comments with PyLint comments."
 readme = "README.rst"
 keywords = [ "flake8", "pre-commit", "pylint",]
 dynamic = []
 dependencies = [ "click>=7.1.2", "consolekit>=1.0.1", "domdf-python-tools>=2.1.0", "flake8>=3.8.4",]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -16,14 +16,15 @@
     "Framework :: Flake8",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Typing :: Typed",
@@ -51,15 +52,15 @@
 base-classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Framework :: Flake8",
     "Intended Audience :: Developers",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 
 [tool.sphinx-pyproject]
 github_username = "domdfcoding"
 github_repository = "flake2lint"
@@ -140,15 +141,15 @@
     "__new__",
     "__getnewargs__",
     "__abstractmethods__",
     "__hash__",
 ]
 
 [tool.mypy]
-python_version = "3.6"
+python_version = "3.8"
 namespace_packages = true
 check_untyped_defs = true
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
 [tool.snippet-fmt]
```

### Comparing `flake2lint-0.4.2/README.rst` & `flake2lint-0.4.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 	:target: https://github.com/domdfcoding/flake2lint/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/flake2lint/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/flake2lint/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/flake2lint/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/flake2lint/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/flake2lint/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/flake2lint/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/flake2lint/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/flake2lint?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/flake2lint?logo=codefactor
@@ -87,23 +87,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/flake2lint
 	:target: https://github.com/domdfcoding/flake2lint/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/flake2lint
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/flake2lint/v0.4.2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/flake2lint/v0.4.3
 	:target: https://github.com/domdfcoding/flake2lint/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/flake2lint
 	:target: https://github.com/domdfcoding/flake2lint/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/flake2lint
 	:target: https://pypi.org/project/flake2lint/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `flake2lint-0.4.2/PKG-INFO` & `flake2lint-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake2lint
-Version: 0.4.2
+Version: 0.4.3
 Summary: Tool and pre-commit hook to augment Flake8 noqa comments with PyLint comments.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: flake8,pre-commit,pylint
 Home-page: https://github.com/domdfcoding/flake2lint
 Project-URL: Issue Tracker, https://github.com/domdfcoding/flake2lint/issues
 Project-URL: Source Code, https://github.com/domdfcoding/flake2lint
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Requires-Dist: click>=7.1.2
 Requires-Dist: consolekit>=1.0.1
 Requires-Dist: domdf-python-tools>=2.1.0
@@ -90,16 +91,16 @@
 	:target: https://github.com/domdfcoding/flake2lint/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/flake2lint/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/flake2lint/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/flake2lint/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/flake2lint/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/flake2lint/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/flake2lint/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/flake2lint/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/flake2lint?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/flake2lint?logo=codefactor
@@ -125,23 +126,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/flake2lint
 	:target: https://github.com/domdfcoding/flake2lint/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/flake2lint
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/flake2lint/v0.4.2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/flake2lint/v0.4.3
 	:target: https://github.com/domdfcoding/flake2lint/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/flake2lint
 	:target: https://github.com/domdfcoding/flake2lint/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/flake2lint
 	:target: https://pypi.org/project/flake2lint/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `flake2lint-0.4.2/LICENSE` & `flake2lint-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flake2lint-0.4.2/flake2lint/__init__.py` & `flake2lint-0.4.3/flake2lint/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from domdf_python_tools.stringlist import DelimitedList
 from domdf_python_tools.typing import PathLike
 from flake8 import defaults  # type: ignore[import]
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.4.2"
+__version__: str = "0.4.3"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["find_pylint_disable", "process_file", "find_noqa"]
 
 code_mapping = {
 		"A001": "redefined-builtin",
 		"A002": "redefined-builtin",
```

### Comparing `flake2lint-0.4.2/flake2lint/__main__.py` & `flake2lint-0.4.3/flake2lint/__main__.py`

 * *Files identical despite different names*

