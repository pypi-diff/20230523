# Comparing `tmp/langchain_wenxin-0.0.1.tar.gz` & `tmp/langchain_wenxin-0.1.0.tar.gz`

## Comparing `langchain_wenxin-0.0.1.tar` & `langchain_wenxin-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 langchain_wenxin-0.0.1/src/langchain_wenxin/__about__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.0.1/src/langchain_wenxin/__init__.py
--rw-r--r--   0        0        0    13473 2020-02-02 00:00:00.000000 langchain_wenxin-0.0.1/src/langchain_wenxin/llms.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 langchain_wenxin-0.0.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 langchain_wenxin-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 langchain_wenxin-0.0.1/README.md
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 langchain_wenxin-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 langchain_wenxin-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 langchain_wenxin-0.1.0/src/langchain_wenxin/__about__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.1.0/src/langchain_wenxin/__init__.py
+-rw-r--r--   0        0        0    13473 2020-02-02 00:00:00.000000 langchain_wenxin-0.1.0/src/langchain_wenxin/llms.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 langchain_wenxin-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 langchain_wenxin-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 langchain_wenxin-0.1.0/README.md
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 langchain_wenxin-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 langchain_wenxin-0.1.0/PKG-INFO
```

### Comparing `langchain_wenxin-0.0.1/src/langchain_wenxin/llms.py` & `langchain_wenxin-0.1.0/src/langchain_wenxin/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.0.1/.gitignore` & `langchain_wenxin-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.0.1/LICENSE.txt` & `langchain_wenxin-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.0.1/README.md` & `langchain_wenxin-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.0.1/pyproject.toml` & `langchain_wenxin-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,31 +20,32 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = []
+dependencies = [
+  "langchain>=0.0.175",
+  "requests",
+  "sseclient",
+]
 
 [project.urls]
 Documentation = "https://github.com/unknown/langchain-wenxin#readme"
 Issues = "https://github.com/unknown/langchain-wenxin/issues"
 Source = "https://github.com/unknown/langchain-wenxin"
 
 [tool.hatch.version]
 path = "src/langchain_wenxin/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
-  "langchain>=0.0.175",
-  "requests",
-  "sseclient",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
```

### Comparing `langchain_wenxin-0.0.1/PKG-INFO` & `langchain_wenxin-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-wenxin
-Version: 0.0.1
+Version: 0.1.0
 Project-URL: Documentation, https://github.com/unknown/langchain-wenxin#readme
 Project-URL: Issues, https://github.com/unknown/langchain-wenxin/issues
 Project-URL: Source, https://github.com/unknown/langchain-wenxin
 Author-email: Tao Yang <swulling@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -13,14 +13,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+Requires-Dist: langchain>=0.0.175
+Requires-Dist: requests
+Requires-Dist: sseclient
 Description-Content-Type: text/markdown
 
 # langchain-wenxin - Langchain Baidu WENXINWORKSHOP wrapper
 
 [![PyPI - Version](https://img.shields.io/pypi/v/langchain-wenxin.svg)](https://pypi.org/project/langchain-wenxin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/langchain-wenxin.svg)](https://pypi.org/project/langchain-wenxin)
```

