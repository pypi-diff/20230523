# Comparing `tmp/octocheese-0.5.0.tar.gz` & `tmp/octocheese-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octocheese-0.5.0.tar", last modified: Sat May 14 14:28:55 2022, max compression
+gzip compressed data, was "octocheese-0.6.0.tar", last modified: Tue May 23 12:54:16 2023, max compression
```

## Comparing `octocheese-0.5.0.tar` & `octocheese-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0 runner    (1001) docker     (121)     4634 2022-05-14 14:28:54.997926 octocheese-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     5069 2022-05-14 14:28:54.997926 octocheese-0.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6792 2022-05-14 14:28:54.997926 octocheese-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-05-14 14:28:54.997926 octocheese-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-05-14 14:28:54.989926 octocheese-0.5.0/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (121)     1480 2022-05-14 14:28:13.893354 octocheese-0.5.0/octocheese/action.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-14 14:28:13.893354 octocheese-0.5.0/octocheese/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2022-05-14 14:28:13.893354 octocheese-0.5.0/octocheese/colours.py
--rw-r--r--   0 runner    (1001) docker     (121)     4881 2022-05-14 14:28:13.893354 octocheese-0.5.0/octocheese/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-05-14 14:28:13.893354 octocheese-0.5.0/octocheese/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9135 2022-05-14 14:28:13.893354 octocheese-0.5.0/octocheese/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5071 2023-05-23 12:54:16.330223 octocheese-0.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-05-23 12:54:16.322223 octocheese-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      229 2023-05-23 12:54:16.330223 octocheese-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     6799 2023-05-23 12:54:16.330223 octocheese-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4639 2023-05-23 12:54:16.326223 octocheese-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-05-23 12:53:40.111646 octocheese-0.6.0/octocheese/colours.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 12:53:40.111646 octocheese-0.6.0/octocheese/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     9140 2023-05-23 12:53:40.111646 octocheese-0.6.0/octocheese/core.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1480 2023-05-23 12:53:40.111646 octocheese-0.6.0/octocheese/action.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4886 2023-05-23 12:53:40.111646 octocheese-0.6.0/octocheese/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-05-23 12:53:40.111646 octocheese-0.6.0/octocheese/__init__.py
```

### Comparing `octocheese-0.5.0/pyproject.toml` & `octocheese-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "octocheese"
-version = "0.5.0"
+version = "0.6.0"
 description = "🐙 🧀 – Copy PyPI Packages to GitHub Releases"
 readme = "README.rst"
 keywords = [ "github", "github-action", "pypi",]
 dynamic = []
 dependencies = [
-    "apeye>=0.3.0",
+    "apeye-core>=1.0.0",
     "click>=7.1.2",
     "consolekit>=0.8.2",
     "domdf-python-tools>=1.5.0",
     "dulwich!=0.20.7,!=0.20.8,>=0.20.5",
     "github3-py>=1.3.0",
     "github3-utils>=0.3.0",
     "packaging>=21.3",
```

### Comparing `octocheese-0.5.0/README.rst` & `octocheese-0.6.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,16 @@
 	:target: https://github.com/domdfcoding/octocheese/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/octocheese/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/octocheese/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/octocheese/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/octocheese/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/octocheese/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/octocheese/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/octocheese/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/octocheese?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/octocheese?logo=codefactor
@@ -88,23 +88,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/octocheese
 	:target: https://github.com/domdfcoding/octocheese/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/octocheese
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/octocheese/v0.5.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/octocheese/v0.6.0
 	:target: https://github.com/domdfcoding/octocheese/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/octocheese
 	:target: https://github.com/domdfcoding/octocheese/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/octocheese
 	:target: https://pypi.org/project/octocheese/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `octocheese-0.5.0/PKG-INFO` & `octocheese-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octocheese
-Version: 0.5.0
+Version: 0.6.0
 Summary: 🐙 🧀 – Copy PyPI Packages to GitHub Releases
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: LGPL-3.0-or-later
 Keywords: github,github-action,pypi
 Home-page: https://github.com/domdfcoding/octocheese
 Project-URL: Issue Tracker, https://github.com/domdfcoding/octocheese/issues
 Project-URL: Source Code, https://github.com/domdfcoding/octocheese
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
-Requires-Dist: apeye>=0.3.0
+Requires-Dist: apeye-core>=1.0.0
 Requires-Dist: click>=7.1.2
 Requires-Dist: consolekit>=0.8.2
 Requires-Dist: domdf-python-tools>=1.5.0
 Requires-Dist: dulwich!=0.20.7,!=0.20.8,>=0.20.5
 Requires-Dist: github3-py>=1.3.0
 Requires-Dist: github3-utils>=0.3.0
 Requires-Dist: packaging>=21.3
@@ -96,16 +96,16 @@
 	:target: https://github.com/domdfcoding/octocheese/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/octocheese/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/octocheese/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/octocheese/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/octocheese/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/octocheese/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/octocheese/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/octocheese/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/octocheese?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/octocheese?logo=codefactor
@@ -131,23 +131,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/octocheese
 	:target: https://github.com/domdfcoding/octocheese/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/octocheese
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/octocheese/v0.5.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/octocheese/v0.6.0
 	:target: https://github.com/domdfcoding/octocheese/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/octocheese
 	:target: https://github.com/domdfcoding/octocheese/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/octocheese
 	:target: https://pypi.org/project/octocheese/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `octocheese-0.5.0/LICENSE` & `octocheese-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `octocheese-0.5.0/octocheese/action.py` & `octocheese-0.6.0/octocheese/action.py`

 * *Files identical despite different names*

### Comparing `octocheese-0.5.0/octocheese/colours.py` & `octocheese-0.6.0/octocheese/colours.py`

 * *Files identical despite different names*

### Comparing `octocheese-0.5.0/octocheese/__main__.py` & `octocheese-0.6.0/octocheese/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 # stdlib
 import sys
 from typing import Union
 
 # 3rd party
 import click
-from apeye import URL
+from apeye_core import URL
 from click import Context, Option
 from consolekit import click_command
 from consolekit.options import auto_default_option, flag_option, version_option
 from domdf_python_tools.secrets import Secret
 from github3_utils.click import token_option
 
 __all__ = ["main", "run", "token_var"]
```

### Comparing `octocheese-0.5.0/octocheese/__init__.py` & `octocheese-0.6.0/octocheese/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,11 +26,11 @@
 
 # this package
 from octocheese.core import copy_pypi_2_github, update_github_release
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020-2021 Dominic Davis-Foster"
 __license__: str = "GNU Lesser General Public License v3 or later (LGPLv3+)"
-__version__: str = "0.5.0"
+__version__: str = "0.6.0"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["copy_pypi_2_github", "update_github_release"]
```

### Comparing `octocheese-0.5.0/octocheese/core.py` & `octocheese-0.6.0/octocheese/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import functools
 from contextlib import suppress
 from functools import partial
 from typing import Iterable, Optional, Union
 
 # 3rd party
 import click
-from apeye import URL
+from apeye_core import URL
 from domdf_python_tools.paths import PathPlus, TemporaryPathPlus
 from domdf_python_tools.stringlist import StringList
 from github3 import GitHub
 from github3.exceptions import NotFoundError
 from github3.repos import Repository
 from github3.repos.release import Release
 from github3_utils.apps import make_footer_links
```

