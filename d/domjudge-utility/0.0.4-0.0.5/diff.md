# Comparing `tmp/domjudge_utility-0.0.4.tar.gz` & `tmp/domjudge_utility-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domjudge_utility-0.0.4.tar", max compression
+gzip compressed data, was "domjudge_utility-0.0.5.tar", max compression
```

## Comparing `domjudge_utility-0.0.4.tar` & `domjudge_utility-0.0.5.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0     1061 2023-05-19 03:14:02.985352 domjudge_utility-0.0.4/LICENSE
--rw-r--r--   0        0        0      636 2023-05-19 03:14:02.985352 domjudge_utility-0.0.4/README.md
--rw-r--r--   0        0        0       22 2023-05-19 03:14:02.989352 domjudge_utility-0.0.4/domjudge_utility/__init__.py
--rw-r--r--   0        0        0     1044 2023-05-19 03:14:02.989352 domjudge_utility-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1485 1970-01-01 00:00:00.000000 domjudge_utility-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-23 05:33:42.634489 domjudge_utility-0.0.5/LICENSE
+-rw-r--r--   0        0        0      636 2023-05-23 05:33:42.634489 domjudge_utility-0.0.5/README.md
+-rw-r--r--   0        0        0       43 2023-05-23 05:33:42.634489 domjudge_utility-0.0.5/domjudge_utility/__init__.py
+-rw-r--r--   0        0        0    24644 2023-05-23 05:33:42.634489 domjudge_utility-0.0.5/domjudge_utility/dump.py
+-rw-r--r--   0        0        0      394 2023-05-23 05:33:42.634489 domjudge_utility-0.0.5/domjudge_utility/utils.py
+-rw-r--r--   0        0        0     1162 2023-05-23 05:33:42.634489 domjudge_utility-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 domjudge_utility-0.0.5/PKG-INFO
```

### Comparing `domjudge_utility-0.0.4/LICENSE` & `domjudge_utility-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `domjudge_utility-0.0.4/README.md` & `domjudge_utility-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `domjudge_utility-0.0.4/pyproject.toml` & `domjudge_utility-0.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "domjudge-utility"
-version = "0.0.4"
+version = "0.0.5"
 description = "DOMjudge Utility"
 authors = ["Dup4 <lyuzhi.pan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -14,14 +14,20 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
+pyyaml = "^6.0"
+xlwt = "^1.3.0"
+requests = "^2.31.0"
+requests-toolbelt = "^1.0.0"
+grequests = "^0.6.0"
+bs4 = "^0.0.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 flake8 = "^6.0.0"
 pyright = "^1.1.305"
 autopep8 = "^2.0.2"
 pytest-snapshot = "^0.9.0"
```

### Comparing `domjudge_utility-0.0.4/PKG-INFO` & `domjudge_utility-0.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: domjudge-utility
-Version: 0.0.4
+Version: 0.0.5
 Summary: DOMjudge Utility
 License: MIT
 Author: Dup4
 Author-email: lyuzhi.pan@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: bs4 (>=0.0.1,<0.0.2)
+Requires-Dist: grequests (>=0.6.0,<0.7.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
+Requires-Dist: xlwt (>=1.3.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 <img align="right" width="96px" src="./assets/python3_logo.png">
 
 # DOMjudge-Utility
 
 [![Test][test-ci-badge]][test-ci]
```

