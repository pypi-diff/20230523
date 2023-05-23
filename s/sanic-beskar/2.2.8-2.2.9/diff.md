# Comparing `tmp/sanic_beskar-2.2.8.tar.gz` & `tmp/sanic_beskar-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanic_beskar-2.2.8.tar", max compression
+gzip compressed data, was "sanic_beskar-2.2.9.tar", max compression
```

## Comparing `sanic_beskar-2.2.8.tar` & `sanic_beskar-2.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1083 2023-03-23 21:52:41.014886 sanic_beskar-2.2.8/LICENSE.rst
--rw-r--r--   0        0        0     4789 2023-03-23 21:52:41.014886 sanic_beskar-2.2.8/README.rst
--rw-r--r--   0        0        0     2172 2023-03-23 21:52:41.022886 sanic_beskar-2.2.8/pyproject.toml
--rw-r--r--   0        0        0      653 2023-03-23 21:52:41.022886 sanic_beskar-2.2.8/sanic_beskar/__init__.py
--rw-r--r--   0        0        0    75146 2023-03-23 21:52:41.022886 sanic_beskar-2.2.8/sanic_beskar/base.py
--rw-r--r--   0        0        0     2337 2023-03-23 21:52:41.022886 sanic_beskar-2.2.8/sanic_beskar/constants.py
--rw-r--r--   0        0        0     8952 2023-03-23 21:52:41.022886 sanic_beskar-2.2.8/sanic_beskar/decorators.py
--rw-r--r--   0        0        0     4011 2023-03-23 21:52:41.022886 sanic_beskar-2.2.8/sanic_beskar/exceptions.py
--rw-r--r--   0        0        0      744 2023-03-23 21:52:41.022886 sanic_beskar-2.2.8/sanic_beskar/orm/__init__.py
--rw-r--r--   0        0        0     3701 2023-03-23 21:52:41.022886 sanic_beskar-2.2.8/sanic_beskar/orm/beanie_user_mixins.py
--rw-r--r--   0        0        0     3643 2023-03-23 21:52:41.022886 sanic_beskar-2.2.8/sanic_beskar/orm/tortoise_user_mixins.py
--rw-r--r--   0        0        0     3964 2023-03-23 21:52:41.022886 sanic_beskar-2.2.8/sanic_beskar/orm/umongo_user_mixins.py
--rw-r--r--   0        0        0        0 2023-03-23 21:52:41.022886 sanic_beskar-2.2.8/sanic_beskar/py.typed
--rw-r--r--   0        0        0     6707 2023-03-23 21:52:41.022886 sanic_beskar-2.2.8/sanic_beskar/templates/registration_email.html
--rw-r--r--   0        0        0     6721 2023-03-23 21:52:41.022886 sanic_beskar-2.2.8/sanic_beskar/templates/reset_email.html
--rw-r--r--   0        0        0     9255 2023-03-23 21:52:41.022886 sanic_beskar-2.2.8/sanic_beskar/utilities.py
--rw-r--r--   0        0        0     5863 1970-01-01 00:00:00.000000 sanic_beskar-2.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-23 15:29:54.628131 sanic_beskar-2.2.9/LICENSE.rst
+-rw-r--r--   0        0        0     4789 2023-05-23 15:29:54.628131 sanic_beskar-2.2.9/README.rst
+-rw-r--r--   0        0        0     2185 2023-05-23 15:29:54.636131 sanic_beskar-2.2.9/pyproject.toml
+-rw-r--r--   0        0        0      653 2023-05-23 15:29:54.636131 sanic_beskar-2.2.9/sanic_beskar/__init__.py
+-rw-r--r--   0        0        0    75146 2023-05-23 15:29:54.636131 sanic_beskar-2.2.9/sanic_beskar/base.py
+-rw-r--r--   0        0        0     2337 2023-05-23 15:29:54.636131 sanic_beskar-2.2.9/sanic_beskar/constants.py
+-rw-r--r--   0        0        0     8952 2023-05-23 15:29:54.636131 sanic_beskar-2.2.9/sanic_beskar/decorators.py
+-rw-r--r--   0        0        0     4011 2023-05-23 15:29:54.636131 sanic_beskar-2.2.9/sanic_beskar/exceptions.py
+-rw-r--r--   0        0        0      744 2023-05-23 15:29:54.636131 sanic_beskar-2.2.9/sanic_beskar/orm/__init__.py
+-rw-r--r--   0        0        0     3701 2023-05-23 15:29:54.636131 sanic_beskar-2.2.9/sanic_beskar/orm/beanie_user_mixins.py
+-rw-r--r--   0        0        0     3643 2023-05-23 15:29:54.636131 sanic_beskar-2.2.9/sanic_beskar/orm/tortoise_user_mixins.py
+-rw-r--r--   0        0        0     3964 2023-05-23 15:29:54.636131 sanic_beskar-2.2.9/sanic_beskar/orm/umongo_user_mixins.py
+-rw-r--r--   0        0        0        0 2023-05-23 15:29:54.636131 sanic_beskar-2.2.9/sanic_beskar/py.typed
+-rw-r--r--   0        0        0     6707 2023-05-23 15:29:54.636131 sanic_beskar-2.2.9/sanic_beskar/templates/registration_email.html
+-rw-r--r--   0        0        0     6721 2023-05-23 15:29:54.636131 sanic_beskar-2.2.9/sanic_beskar/templates/reset_email.html
+-rw-r--r--   0        0        0     9255 2023-05-23 15:29:54.636131 sanic_beskar-2.2.9/sanic_beskar/utilities.py
+-rw-r--r--   0        0        0     5860 1970-01-01 00:00:00.000000 sanic_beskar-2.2.9/PKG-INFO
```

### Comparing `sanic_beskar-2.2.8/LICENSE.rst` & `sanic_beskar-2.2.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `sanic_beskar-2.2.8/README.rst` & `sanic_beskar-2.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `sanic_beskar-2.2.8/pyproject.toml` & `sanic_beskar-2.2.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sanic-beskar"
-version = "2.2.8"
+version = "2.2.9"
 description = "Strong, Simple, (now async!) and Precise security for Sanic APIs"
 authors = ["Rob Dailey <rob@suspected.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://sanic-beskar.readthedocs.io/en/latest/"
 documentation = "https://sanic-beskar.readthedocs.io/en/latest/"
 repository = "https://github.com/pahrohfit/sanic-beskar"
@@ -16,39 +16,39 @@
 types-passlib = "^1.7"
 mongo-types = "^0.15"
 mypy = "^1.1"
 
 [tool.poetry.group.dev.dependencies]
 bcrypt = "^4.0.1"
 plummet = {version = "^1.1", extras = ["time-machine"]}
-sanic-testing = "^22.6.0"
-pytest-asyncio = "^0.20.2"
+sanic-testing = "^23.3"
+pytest-asyncio = "^0.21"
 tortoise-orm = "^0.19.2"
 nest-asyncio = "^1.5.5"
 pytest-cov = "^4.0.0"
 umongo = "3.1.0"
 motor = "^3.1.0"
 pytest-profiling = "^1.7.0"
 fastpbkdf2 = "^0.2"
 segno = "^1.5.2"
 pytest = "^7.2.0"
-beanie = "^1.11.7"
-mongomock-motor = "^0.0.17"
+beanie = ">=1.11.7, <=2.0"
+mongomock-motor = "^0.0.19"
 mongomock = "^4.1.2"
 ipdb = "^0.13.9"
 bandit = "^1.7.4"
 flake8-async = "^22.11.6"
 safety = "^2.3.1"
 async-sender = "^2.0.0"
 pytest-xdist = "^3.0.2"
 
 [tool.poetry.group.docs.dependencies]
 toml = "^0.10.2"
-sphinx = "^6.0.0"
-sphinx-rtd-theme = "^1.1.1"
+sphinx = "^7.0.1"
+furo = "^2023.5.20"
 
 [tool.coverage.report]
 exclude_lines = [
     'pragma: no cover',
     'if TYPE_CHECKING:',
     'def __repr__',
 ]
@@ -63,18 +63,18 @@
 exclude = ["example", "docs", "tests"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pyjwt = "^2.6"
 pendulum = "^2.1"
 passlib = "^1.7"
-sanic = "^22.6.0"
+sanic = ">=22.6.0, <=23.4"
 pyseto = "^1.6.9"
 py-buzz = "^3.2.1"
-cryptography = "^39.0.2"
+cryptography = ">=39.0.2, <40.1"
 jinja2 = "^3.1.2"
 
 [build-system]
 requires = ["poetry-core>=1.2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
```

### Comparing `sanic_beskar-2.2.8/sanic_beskar/__init__.py` & `sanic_beskar-2.2.9/sanic_beskar/__init__.py`

 * *Files identical despite different names*

### Comparing `sanic_beskar-2.2.8/sanic_beskar/base.py` & `sanic_beskar-2.2.9/sanic_beskar/base.py`

 * *Files identical despite different names*

### Comparing `sanic_beskar-2.2.8/sanic_beskar/constants.py` & `sanic_beskar-2.2.9/sanic_beskar/constants.py`

 * *Files identical despite different names*

### Comparing `sanic_beskar-2.2.8/sanic_beskar/decorators.py` & `sanic_beskar-2.2.9/sanic_beskar/decorators.py`

 * *Files identical despite different names*

### Comparing `sanic_beskar-2.2.8/sanic_beskar/exceptions.py` & `sanic_beskar-2.2.9/sanic_beskar/exceptions.py`

 * *Files identical despite different names*

### Comparing `sanic_beskar-2.2.8/sanic_beskar/orm/__init__.py` & `sanic_beskar-2.2.9/sanic_beskar/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `sanic_beskar-2.2.8/sanic_beskar/orm/beanie_user_mixins.py` & `sanic_beskar-2.2.9/sanic_beskar/orm/beanie_user_mixins.py`

 * *Files identical despite different names*

### Comparing `sanic_beskar-2.2.8/sanic_beskar/orm/tortoise_user_mixins.py` & `sanic_beskar-2.2.9/sanic_beskar/orm/tortoise_user_mixins.py`

 * *Files identical despite different names*

### Comparing `sanic_beskar-2.2.8/sanic_beskar/orm/umongo_user_mixins.py` & `sanic_beskar-2.2.9/sanic_beskar/orm/umongo_user_mixins.py`

 * *Files identical despite different names*

### Comparing `sanic_beskar-2.2.8/sanic_beskar/templates/registration_email.html` & `sanic_beskar-2.2.9/sanic_beskar/templates/registration_email.html`

 * *Files identical despite different names*

### Comparing `sanic_beskar-2.2.8/sanic_beskar/templates/reset_email.html` & `sanic_beskar-2.2.9/sanic_beskar/templates/reset_email.html`

 * *Files identical despite different names*

### Comparing `sanic_beskar-2.2.8/sanic_beskar/utilities.py` & `sanic_beskar-2.2.9/sanic_beskar/utilities.py`

 * *Files identical despite different names*

### Comparing `sanic_beskar-2.2.8/PKG-INFO` & `sanic_beskar-2.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: sanic-beskar
-Version: 2.2.8
+Version: 2.2.9
 Summary: Strong, Simple, (now async!) and Precise security for Sanic APIs
 Home-page: https://sanic-beskar.readthedocs.io/en/latest/
 License: MIT
 Author: Rob Dailey
 Author-email: rob@suspected.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: cryptography (>=39.0.2,<40.0.0)
+Requires-Dist: cryptography (>=39.0.2,<40.1)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: passlib (>=1.7,<2.0)
 Requires-Dist: pendulum (>=2.1,<3.0)
 Requires-Dist: py-buzz (>=3.2.1,<4.0.0)
 Requires-Dist: pyjwt (>=2.6,<3.0)
 Requires-Dist: pyseto (>=1.6.9,<2.0.0)
-Requires-Dist: sanic (>=22.6.0,<23.0.0)
+Requires-Dist: sanic (>=22.6.0,<=23.4)
 Project-URL: Documentation, https://sanic-beskar.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/pahrohfit/sanic-beskar
 Description-Content-Type: text/x-rst
 
 .. image::  https://badge.fury.io/py/sanic-beskar.svg
    :target: https://badge.fury.io/py/sanic-beskar
    :alt:    Latest Published Version
```

