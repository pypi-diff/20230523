# Comparing `tmp/sqlinks-0.0.1.tar.gz` & `tmp/sqlinks-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlinks-0.0.1.tar", last modified: Fri May 19 11:19:29 2023, max compression
+gzip compressed data, was "sqlinks-0.0.2.tar", last modified: Tue May 23 14:53:10 2023, max compression
```

## Comparing `sqlinks-0.0.1.tar` & `sqlinks-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 dherriott   (502) staff       (20)        0 2023-05-19 11:19:29.883766 sqlinks-0.0.1/
--rw-r--r--   0 dherriott   (502) staff       (20)    35149 2023-05-18 14:11:11.000000 sqlinks-0.0.1/LICENSE
--rw-r--r--   0 dherriott   (502) staff       (20)     1003 2023-05-19 11:19:29.883607 sqlinks-0.0.1/PKG-INFO
--rw-r--r--   0 dherriott   (502) staff       (20)     1946 2023-05-19 11:07:41.000000 sqlinks-0.0.1/README.md
--rw-r--r--   0 dherriott   (502) staff       (20)       38 2023-05-19 11:19:29.883814 sqlinks-0.0.1/setup.cfg
--rw-r--r--   0 dherriott   (502) staff       (20)     1354 2023-05-19 11:08:47.000000 sqlinks-0.0.1/setup.py
-drwxr-xr-x   0 dherriott   (502) staff       (20)        0 2023-05-19 11:19:29.875298 sqlinks-0.0.1/sqlinks/
--rw-r--r--   0 dherriott   (502) staff       (20)       20 2023-05-19 11:12:12.000000 sqlinks-0.0.1/sqlinks/__init__.py
--rw-r--r--   0 dherriott   (502) staff       (20)     2727 2023-05-19 11:13:44.000000 sqlinks-0.0.1/sqlinks/__main__.py
-drwxr-xr-x   0 dherriott   (502) staff       (20)        0 2023-05-19 11:19:29.881154 sqlinks-0.0.1/sqlinks/app/
--rw-r--r--   0 dherriott   (502) staff       (20)    14287 2023-05-19 11:12:57.000000 sqlinks-0.0.1/sqlinks/app/Objects.py
--rw-r--r--   0 dherriott   (502) staff       (20)       20 2023-05-19 11:12:15.000000 sqlinks-0.0.1/sqlinks/app/__init__.py
--rw-r--r--   0 dherriott   (502) staff       (20)     1273 2023-05-18 16:46:52.000000 sqlinks-0.0.1/sqlinks/app/draw.py
--rw-r--r--   0 dherriott   (502) staff       (20)      501 2023-05-18 14:11:11.000000 sqlinks-0.0.1/sqlinks/app/helpers.py
--rw-r--r--   0 dherriott   (502) staff       (20)      272 2023-05-18 14:11:11.000000 sqlinks-0.0.1/sqlinks/app/open.py
--rw-r--r--   0 dherriott   (502) staff       (20)     7058 2023-05-19 11:13:31.000000 sqlinks-0.0.1/sqlinks/app/parse.py
--rw-r--r--   0 dherriott   (502) staff       (20)     7137 2023-05-18 14:11:11.000000 sqlinks-0.0.1/sqlinks/app/populate.py
--rw-r--r--   0 dherriott   (502) staff       (20)      621 2023-05-18 16:23:24.000000 sqlinks-0.0.1/sqlinks/app/scan.py
-drwxr-xr-x   0 dherriott   (502) staff       (20)        0 2023-05-19 11:19:29.881587 sqlinks-0.0.1/sqlinks/app/templates/
--rw-r--r--   0 dherriott   (502) staff       (20)     2862 2023-05-18 14:11:11.000000 sqlinks-0.0.1/sqlinks/app/templates/drawio_template.xml
-drwxr-xr-x   0 dherriott   (502) staff       (20)        0 2023-05-19 11:19:29.877377 sqlinks-0.0.1/sqlinks.egg-info/
--rw-r--r--   0 dherriott   (502) staff       (20)     1003 2023-05-19 11:19:29.000000 sqlinks-0.0.1/sqlinks.egg-info/PKG-INFO
--rw-r--r--   0 dherriott   (502) staff       (20)      536 2023-05-19 11:19:29.000000 sqlinks-0.0.1/sqlinks.egg-info/SOURCES.txt
--rw-r--r--   0 dherriott   (502) staff       (20)        1 2023-05-19 11:19:29.000000 sqlinks-0.0.1/sqlinks.egg-info/dependency_links.txt
--rw-r--r--   0 dherriott   (502) staff       (20)       29 2023-05-19 11:19:29.000000 sqlinks-0.0.1/sqlinks.egg-info/requires.txt
--rw-r--r--   0 dherriott   (502) staff       (20)       14 2023-05-19 11:19:29.000000 sqlinks-0.0.1/sqlinks.egg-info/top_level.txt
-drwxr-xr-x   0 dherriott   (502) staff       (20)        0 2023-05-19 11:19:29.883132 sqlinks-0.0.1/tests/
--rw-r--r--   0 dherriott   (502) staff       (20)        0 2022-09-24 20:01:55.000000 sqlinks-0.0.1/tests/__init__.py
--rw-r--r--   0 dherriott   (502) staff       (20)        0 2022-09-24 20:01:55.000000 sqlinks-0.0.1/tests/test_draw.py
--rw-r--r--   0 dherriott   (502) staff       (20)       39 2023-05-19 11:13:13.000000 sqlinks-0.0.1/tests/test_parse.py
--rw-r--r--   0 dherriott   (502) staff       (20)        0 2022-09-24 20:01:55.000000 sqlinks-0.0.1/tests/test_populate.py
--rw-r--r--   0 dherriott   (502) staff       (20)       98 2023-05-19 11:13:09.000000 sqlinks-0.0.1/tests/test_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:53:10.088570 sqlinks-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-23 14:53:00.000000 sqlinks-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-23 14:53:10.088570 sqlinks-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-23 14:53:00.000000 sqlinks-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:53:10.088570 sqlinks-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-23 14:53:00.000000 sqlinks-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:53:10.088570 sqlinks-0.0.2/sqlinks/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 14:53:00.000000 sqlinks-0.0.2/sqlinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-23 14:53:00.000000 sqlinks-0.0.2/sqlinks/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:53:10.088570 sqlinks-0.0.2/sqlinks/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-05-23 14:53:00.000000 sqlinks-0.0.2/sqlinks/app/Objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 14:53:00.000000 sqlinks-0.0.2/sqlinks/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-23 14:53:00.000000 sqlinks-0.0.2/sqlinks/app/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-23 14:53:00.000000 sqlinks-0.0.2/sqlinks/app/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-23 14:53:00.000000 sqlinks-0.0.2/sqlinks/app/open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-05-23 14:53:00.000000 sqlinks-0.0.2/sqlinks/app/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-05-23 14:53:00.000000 sqlinks-0.0.2/sqlinks/app/populate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-23 14:53:00.000000 sqlinks-0.0.2/sqlinks/app/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:53:10.088570 sqlinks-0.0.2/sqlinks/app/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-23 14:53:00.000000 sqlinks-0.0.2/sqlinks/app/templates/drawio_template.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:53:10.088570 sqlinks-0.0.2/sqlinks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-23 14:53:10.000000 sqlinks-0.0.2/sqlinks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-23 14:53:10.000000 sqlinks-0.0.2/sqlinks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:53:10.000000 sqlinks-0.0.2/sqlinks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-23 14:53:10.000000 sqlinks-0.0.2/sqlinks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 14:53:10.000000 sqlinks-0.0.2/sqlinks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:53:10.088570 sqlinks-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:53:00.000000 sqlinks-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:53:00.000000 sqlinks-0.0.2/tests/test_draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 14:53:00.000000 sqlinks-0.0.2/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:53:00.000000 sqlinks-0.0.2/tests/test_populate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 14:53:00.000000 sqlinks-0.0.2/tests/test_scan.py
```

### Comparing `sqlinks-0.0.1/LICENSE` & `sqlinks-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlinks-0.0.1/PKG-INFO` & `sqlinks-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlinks
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streaming video data via networks
 Author: Dominic Herriott
 Author-email: dominicherriott@outlook.com
 Keywords: python,documentation,sql
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqlinks-0.0.1/README.md` & `sqlinks-0.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 <h1 align="center">sqlinks</h1> <br>
 <p align="center">
   <a href="">
-    <img alt="sqlinks" title="sqlinks" src="images/logo.png" width="250">
+    <img alt="sqlinks" title="sqlinks" src="images/link-logo.png" width="250">
   </a>
 </p>
 
 <p align="center">
   Diagram your data pipelines.
 </p>
 
 ## Table of Contents
 
 - [Table of Contents](#table-of-contents)
 - [Introduction](#introduction)
 - [Features](#features)
 - [Example](#example)
+- [Getting started](#getting-started)
 - [Feedback](#feedback)
 - [Acknowledgments](#acknowledgments)
 - [Dev](#dev)
 - [Deflation](#deflation)
   - [](#)
+  - [PyPI](#pypi)
 
 ## Introduction
 
 Documenting data pipelines is hard. Not only is it complex, but it's also time consuming. When working with big teams it becomes near impossible; documentation is out of date as soon as it's completed as there's continual change. **sqlinks** hopes to remedy this by allowing you to generate flow diagrams programatically. This allows for reproducable and clear diagrams that, by using [diagrams.net](diagrams.net), are also easily accessible by non-technical users.
 
 
 ## Features
@@ -36,14 +38,29 @@
 - ⏳ Customisation via config files
 
 
 ## Example
 
 Coming soon...
 
+## Getting started
+
+Install **sqlinks** using **pip**:
+
+```pip install sqlinks```
+
+
+When installed, run **sqlinks** against your current directory using the following:
+
+```python -m sqlinks```
+
+To view all available command line options use:
+
+```python -m sqlinks --help```
+
 
 ## Feedback
 
 Feel free to reach out on [LinkedIn](https://www.linkedin.com/in/dominic-herriott/) and please use [GitHub Issues](https://github.com/domherriott/sqlinks/issues) for feature requests! :grinning:
 
 ## Acknowledgments
 
@@ -63,7 +80,11 @@
 ###
 
 Build dist files
 `python setup.py sdist bdist_wheel`
 
 Push to PyPI
 `python -m twine upload --repository testpypi dist/*`
+
+
+### PyPI
+https://pypi.org/project/sqlinks/0.0.1/
```

#### html2text {}

```diff
@@ -1,27 +1,32 @@
                              ****** sqlinks ******
 
                                    [sqlinks]
                          Diagram your data pipelines.
 ## Table of Contents - [Table of Contents](#table-of-contents) - [Introduction]
-(#introduction) - [Features](#features) - [Example](#example) - [Feedback]
-(#feedback) - [Acknowledgments](#acknowledgments) - [Dev](#dev) - [Deflation]
-(#deflation) - [](#) ## Introduction Documenting data pipelines is hard. Not
-only is it complex, but it's also time consuming. When working with big teams
-it becomes near impossible; documentation is out of date as soon as it's
-completed as there's continual change. **sqlinks** hopes to remedy this by
-allowing you to generate flow diagrams programatically. This allows for
-reproducable and clear diagrams that, by using [diagrams.net](diagrams.net),
-are also easily accessible by non-technical users. ## Features - ð Generate
-flow diagrams from simple CTAS statements - ð Visualise interactions of
-schemas, tables & columns To come... - â³ Functionality for complex CTAS
-statements, CTEs, INSERT statements etc. - â³ Customisation via config files
-## Example Coming soon... ## Feedback Feel free to reach out on [LinkedIn]
-(https://www.linkedin.com/in/dominic-herriott/) and please use [GitHub Issues]
-(https://github.com/domherriott/sqlinks/issues) for feature requests! :
-grinning: ## Acknowledgments Thanks to all those who have contributed and
-helped build the packages this is built on. Special thanks to the developers at
-[diagrams.net](diagrams.net)! ## Dev run `pre-commit install` to set up the git
-hook scripts ## Deflation https://drawio-app.com/extracting-the-xml-from-
-mxfiles/ https://jgraph.github.io/drawio-tools/tools/convert.html ### Build
-dist files `python setup.py sdist bdist_wheel` Push to PyPI `python -m twine
-upload --repository testpypi dist/*`
+(#introduction) - [Features](#features) - [Example](#example) - [Getting
+started](#getting-started) - [Feedback](#feedback) - [Acknowledgments]
+(#acknowledgments) - [Dev](#dev) - [Deflation](#deflation) - [](#) - [PyPI]
+(#pypi) ## Introduction Documenting data pipelines is hard. Not only is it
+complex, but it's also time consuming. When working with big teams it becomes
+near impossible; documentation is out of date as soon as it's completed as
+there's continual change. **sqlinks** hopes to remedy this by allowing you to
+generate flow diagrams programatically. This allows for reproducable and clear
+diagrams that, by using [diagrams.net](diagrams.net), are also easily
+accessible by non-technical users. ## Features - ð Generate flow diagrams
+from simple CTAS statements - ð Visualise interactions of schemas, tables &
+columns To come... - â³ Functionality for complex CTAS statements, CTEs,
+INSERT statements etc. - â³ Customisation via config files ## Example Coming
+soon... ## Getting started Install **sqlinks** using **pip**: ```pip install
+sqlinks``` When installed, run **sqlinks** against your current directory using
+the following: ```python -m sqlinks``` To view all available command line
+options use: ```python -m sqlinks --help``` ## Feedback Feel free to reach out
+on [LinkedIn](https://www.linkedin.com/in/dominic-herriott/) and please use
+[GitHub Issues](https://github.com/domherriott/sqlinks/issues) for feature
+requests! :grinning: ## Acknowledgments Thanks to all those who have
+contributed and helped build the packages this is built on. Special thanks to
+the developers at [diagrams.net](diagrams.net)! ## Dev run `pre-commit install`
+to set up the git hook scripts ## Deflation https://drawio-app.com/extracting-
+the-xml-from-mxfiles/ https://jgraph.github.io/drawio-tools/tools/convert.html
+### Build dist files `python setup.py sdist bdist_wheel` Push to PyPI `python -
+m twine upload --repository testpypi dist/*` ### PyPI https://pypi.org/project/
+sqlinks/0.0.1/
```

### Comparing `sqlinks-0.0.1/setup.py` & `sqlinks-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 DESCRIPTION = "Streaming video data via networks"
 LONG_DESCRIPTION = "Documenting data pipelines is hard. Not only is it complex, but it's also time consuming. When working with big teams it becomes near impossible; documentation is out of date as soon as it's completed as there's continual change. **sqlinks** hopes to remedy this by allowing you to generate flow diagrams programatically. This allows for reproducable and clear diagrams that, by using [diagrams.net](diagrams.net), are also easily accessible by non-technical users."
 
 # Setting up
 setup(
     name="sqlinks",
     version=VERSION,
```

### Comparing `sqlinks-0.0.1/sqlinks/__main__.py` & `sqlinks-0.0.2/sqlinks/__main__.py`

 * *Files identical despite different names*

### Comparing `sqlinks-0.0.1/sqlinks/app/Objects.py` & `sqlinks-0.0.2/sqlinks/app/Objects.py`

 * *Files identical despite different names*

### Comparing `sqlinks-0.0.1/sqlinks/app/draw.py` & `sqlinks-0.0.2/sqlinks/app/draw.py`

 * *Files identical despite different names*

### Comparing `sqlinks-0.0.1/sqlinks/app/parse.py` & `sqlinks-0.0.2/sqlinks/app/parse.py`

 * *Files identical despite different names*

### Comparing `sqlinks-0.0.1/sqlinks/app/populate.py` & `sqlinks-0.0.2/sqlinks/app/populate.py`

 * *Files identical despite different names*

### Comparing `sqlinks-0.0.1/sqlinks/app/scan.py` & `sqlinks-0.0.2/sqlinks/app/scan.py`

 * *Files identical despite different names*

### Comparing `sqlinks-0.0.1/sqlinks/app/templates/drawio_template.xml` & `sqlinks-0.0.2/sqlinks/app/templates/drawio_template.xml`

 * *Files identical despite different names*

### Comparing `sqlinks-0.0.1/sqlinks.egg-info/PKG-INFO` & `sqlinks-0.0.2/sqlinks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlinks
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streaming video data via networks
 Author: Dominic Herriott
 Author-email: dominicherriott@outlook.com
 Keywords: python,documentation,sql
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqlinks-0.0.1/sqlinks.egg-info/SOURCES.txt` & `sqlinks-0.0.2/sqlinks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

