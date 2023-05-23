# Comparing `tmp/pysecuritytxt-1.1.0.tar.gz` & `tmp/pysecuritytxt-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysecuritytxt-1.1.0.tar", max compression
+gzip compressed data, was "pysecuritytxt-1.1.1.tar", max compression
```

## Comparing `pysecuritytxt-1.1.0.tar` & `pysecuritytxt-1.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1516 2022-08-30 12:22:20.250018 pysecuritytxt-1.1.0/LICENSE
--rw-r--r--   0        0        0      628 2022-09-01 12:24:36.102749 pysecuritytxt-1.1.0/README.md
--rw-r--r--   0        0        0     1386 2023-03-20 09:13:45.957430 pysecuritytxt-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      522 2023-02-14 11:30:56.801475 pysecuritytxt-1.1.0/pysecuritytxt/__init__.py
--rw-r--r--   0        0        0     6722 2023-03-20 09:02:25.117314 pysecuritytxt-1.1.0/pysecuritytxt/api.py
--rw-r--r--   0        0        0        0 2022-08-30 12:22:20.250018 pysecuritytxt-1.1.0/pysecuritytxt/py.typed
--rw-r--r--   0        0        0     2103 1970-01-01 00:00:00.000000 pysecuritytxt-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1516 2022-08-30 12:22:20.250018 pysecuritytxt-1.1.1/LICENSE
+-rw-r--r--   0        0        0      628 2022-09-01 12:24:36.102749 pysecuritytxt-1.1.1/README.md
+-rw-r--r--   0        0        0     1512 2023-05-23 12:59:39.054189 pysecuritytxt-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      522 2023-02-14 11:30:56.801475 pysecuritytxt-1.1.1/pysecuritytxt/__init__.py
+-rw-r--r--   0        0        0     6722 2023-03-20 09:16:34.074434 pysecuritytxt-1.1.1/pysecuritytxt/api.py
+-rw-r--r--   0        0        0        0 2022-08-30 12:22:20.250018 pysecuritytxt-1.1.1/pysecuritytxt/py.typed
+-rw-r--r--   0        0        0     2154 1970-01-01 00:00:00.000000 pysecuritytxt-1.1.1/PKG-INFO
```

### Comparing `pysecuritytxt-1.1.0/LICENSE` & `pysecuritytxt-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysecuritytxt-1.1.0/README.md` & `pysecuritytxt-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pysecuritytxt-1.1.0/pyproject.toml` & `pysecuritytxt-1.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysecuritytxt"
-version = "1.1.0"
+version = "1.1.1"
 description = "Python CLI and module for querying security.txt files on domains."
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/pysecuritytxt"
 documentation = "https://pysecuritytxt.readthedocs.io/en/latest/index.html"
 
 readme = "README.md"
@@ -17,33 +17,37 @@
     'Intended Audience :: Science/Research',
     'Intended Audience :: Telecommunications Industry',
     'Intended Audience :: Information Technology',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Security',
     'Topic :: Internet',
 ]
 
 include = ['README.md']
 
 [tool.poetry.scripts]
 pysecuritytxt = 'pysecuritytxt:main'
 
 [tool.poetry.dependencies]
 python = "^3.8"
-requests = "^2.28.2"
-Sphinx = { version = "^6.1.3", optional = true }
+requests = "^2.31.0"
+Sphinx = { version = "^7.0.1", optional = true }
 
 [tool.poetry.dev-dependencies]
-mypy = "^1.1.1"
-types-requests = "^2.28.11.15"
-ipython = "^8.11.0"
-pytest = "^7.2.2"
+mypy = "^1.3.0"
+types-requests = "^2.31.0.0"
+ipython = [
+    {version = "<8.13.0", python = "<3.9"},
+    {version = "^8.13.0", python = ">=3.9"}
+]
+pytest = "^7.3.1"
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
 
 [build-system]
 requires = ["poetry_core>=1.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pysecuritytxt-1.1.0/pysecuritytxt/__init__.py` & `pysecuritytxt-1.1.1/pysecuritytxt/__init__.py`

 * *Files identical despite different names*

### Comparing `pysecuritytxt-1.1.0/pysecuritytxt/api.py` & `pysecuritytxt-1.1.1/pysecuritytxt/api.py`

 * *Files identical despite different names*

### Comparing `pysecuritytxt-1.1.0/PKG-INFO` & `pysecuritytxt-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysecuritytxt
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python CLI and module for querying security.txt files on domains.
 Home-page: https://github.com/Lookyloo/pysecuritytxt
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,21 +17,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: docs
-Requires-Dist: Sphinx (>=6.1.3,<7.0.0) ; extra == "docs"
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: Sphinx (>=7.0.1,<8.0.0) ; extra == "docs"
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Documentation, https://pysecuritytxt.readthedocs.io/en/latest/index.html
 Project-URL: Repository, https://github.com/Lookyloo/pysecuritytxt
 Description-Content-Type: text/markdown
 
 # Python client and module for querying .well-known/security.txt files
 
 Give it a domain, it tries to fetch the security.txt file
```

