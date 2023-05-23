# Comparing `tmp/deprecation-alias-0.3.1.tar.gz` & `tmp/deprecation-alias-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deprecation-alias-0.3.1.tar", last modified: Mon Feb  7 10:28:24 2022, max compression
+gzip compressed data, was "deprecation-alias-0.3.2.tar", last modified: Tue May 23 15:55:02 2023, max compression
```

## Comparing `deprecation-alias-0.3.1.tar` & `deprecation-alias-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 10:28:24.904339 deprecation-alias-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)    10898 2022-02-07 10:27:49.000000 deprecation-alias-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-02-07 10:27:49.000000 deprecation-alias-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6468 2022-02-07 10:28:24.904339 deprecation-alias-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5055 2022-02-07 10:27:49.000000 deprecation-alias-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 10:28:24.904339 deprecation-alias-0.3.1/deprecation_alias/
--rw-r--r--   0 runner    (1001) docker     (121)     7753 2022-02-07 10:27:49.000000 deprecation-alias-0.3.1/deprecation_alias/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 10:27:49.000000 deprecation-alias-0.3.1/deprecation_alias/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 10:28:24.904339 deprecation-alias-0.3.1/deprecation_alias.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6468 2022-02-07 10:28:24.000000 deprecation-alias-0.3.1/deprecation_alias.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-02-07 10:28:24.000000 deprecation-alias-0.3.1/deprecation_alias.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-07 10:28:24.000000 deprecation-alias-0.3.1/deprecation_alias.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-07 10:28:24.000000 deprecation-alias-0.3.1/deprecation_alias.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-02-07 10:28:24.000000 deprecation-alias-0.3.1/deprecation_alias.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-02-07 10:28:24.000000 deprecation-alias-0.3.1/deprecation_alias.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1781 2022-02-07 10:27:49.000000 deprecation-alias-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-02-07 10:27:49.000000 deprecation-alias-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2022-02-07 10:28:24.908339 deprecation-alias-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      639 2022-02-07 10:27:49.000000 deprecation-alias-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 15:55:02.863628 deprecation-alias-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    10898 2023-05-23 15:54:35.000000 deprecation-alias-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-05-23 15:54:35.000000 deprecation-alias-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    19145 2023-05-23 15:55:02.863628 deprecation-alias-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5057 2023-05-23 15:54:35.000000 deprecation-alias-0.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 15:55:02.863628 deprecation-alias-0.3.2/deprecation_alias/
+-rw-r--r--   0 runner    (1001) docker     (122)     7753 2023-05-23 15:54:35.000000 deprecation-alias-0.3.2/deprecation_alias/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 15:54:35.000000 deprecation-alias-0.3.2/deprecation_alias/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 15:55:02.863628 deprecation-alias-0.3.2/deprecation_alias.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    19145 2023-05-23 15:55:02.000000 deprecation-alias-0.3.2/deprecation_alias.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      408 2023-05-23 15:55:02.000000 deprecation-alias-0.3.2/deprecation_alias.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 15:55:02.000000 deprecation-alias-0.3.2/deprecation_alias.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 15:55:02.000000 deprecation-alias-0.3.2/deprecation_alias.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-23 15:55:02.000000 deprecation-alias-0.3.2/deprecation_alias.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-23 15:55:02.000000 deprecation-alias-0.3.2/deprecation_alias.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-05-23 15:54:35.000000 deprecation-alias-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-23 15:54:35.000000 deprecation-alias-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-05-23 15:55:02.863628 deprecation-alias-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2023-05-23 15:54:35.000000 deprecation-alias-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 15:55:02.863628 deprecation-alias-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4961 2023-05-23 15:54:35.000000 deprecation-alias-0.3.2/tests/test_deprecation.py
```

### Comparing `deprecation-alias-0.3.1/LICENSE` & `deprecation-alias-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deprecation-alias-0.3.1/README.rst` & `deprecation-alias-0.3.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 	:target: https://github.com/domdfcoding/deprecation-alias/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/deprecation-alias/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/deprecation-alias/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/deprecation-alias/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/deprecation-alias/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/deprecation-alias/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/deprecation-alias/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/deprecation-alias/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/deprecation-alias?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/deprecation-alias?logo=codefactor
@@ -87,23 +87,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/deprecation-alias
 	:target: https://github.com/domdfcoding/deprecation-alias/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/deprecation-alias
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/deprecation-alias/v0.3.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/deprecation-alias/v0.3.2
 	:target: https://github.com/domdfcoding/deprecation-alias/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/deprecation-alias
 	:target: https://github.com/domdfcoding/deprecation-alias/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/deprecation-alias
 	:target: https://pypi.org/project/deprecation-alias/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `deprecation-alias-0.3.1/deprecation_alias/__init__.py` & `deprecation-alias-0.3.2/deprecation_alias/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # 3rd party
 import deprecation  # type: ignore
 from packaging import version
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "Apache Software License"
-__version__: str = "0.3.1"
+__version__: str = "0.3.2"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["deprecated"]
 
 
 def deprecated(
 		deprecated_in: Optional[str] = None,
```

### Comparing `deprecation-alias-0.3.1/setup.cfg` & `deprecation-alias-0.3.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = deprecation-alias
-version = 0.3.1
+version = 0.3.2
 author = Dominic Davis-Foster
 author_email = dominic@davis-foster.co.uk
 license = Apache Software License
 keywords = deprecation
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 platforms = Windows, macOS, Linux
@@ -20,14 +20,15 @@
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Software Development :: Libraries :: Python Modules
 	Typing :: Typed
 
 [options]
 python_requires = >=3.6.1
```

### Comparing `deprecation-alias-0.3.1/setup.py` & `deprecation-alias-0.3.2/setup.py`

 * *Files identical despite different names*

