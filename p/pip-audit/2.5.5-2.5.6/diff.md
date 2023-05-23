# Comparing `tmp/pip_audit-2.5.5.tar.gz` & `tmp/pip_audit-2.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_audit-2.5.5.tar", last modified: Thu May  4 16:28:45 2023, max compression
+gzip compressed data, was "pip_audit-2.5.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pip_audit-2.5.5.tar` & `pip_audit-2.5.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    10174 2023-05-04 16:28:36.653429 pip_audit-2.5.5/LICENSE
--rw-r--r--   0        0        0    20850 2023-05-04 16:28:36.653429 pip_audit-2.5.5/README.md
--rw-r--r--   0        0        0       53 2023-05-04 16:28:36.653429 pip_audit-2.5.5/pip_audit/__init__.py
--rw-r--r--   0        0        0      144 2023-05-04 16:28:36.653429 pip_audit-2.5.5/pip_audit/__main__.py
--rw-r--r--   0        0        0     3158 2023-05-04 16:28:36.653429 pip_audit-2.5.5/pip_audit/_audit.py
--rw-r--r--   0        0        0     6214 2023-05-04 16:28:36.653429 pip_audit-2.5.5/pip_audit/_cache.py
--rw-r--r--   0        0        0    19415 2023-05-04 16:28:36.653429 pip_audit-2.5.5/pip_audit/_cli.py
--rw-r--r--   0        0        0      490 2023-05-04 16:28:36.653429 pip_audit-2.5.5/pip_audit/_dependency_source/__init__.py
--rw-r--r--   0        0        0     1552 2023-05-04 16:28:36.653429 pip_audit-2.5.5/pip_audit/_dependency_source/interface.py
--rw-r--r--   0        0        0     6853 2023-05-04 16:28:36.653429 pip_audit-2.5.5/pip_audit/_dependency_source/pip.py
--rw-r--r--   0        0        0     5416 2023-05-04 16:28:36.653429 pip_audit-2.5.5/pip_audit/_dependency_source/pyproject.py
--rw-r--r--   0        0        0    10810 2023-05-04 16:28:36.653429 pip_audit-2.5.5/pip_audit/_dependency_source/requirement.py
--rw-r--r--   0        0        0     3683 2023-05-04 16:28:36.653429 pip_audit-2.5.5/pip_audit/_fix.py
--rw-r--r--   0        0        0      380 2023-05-04 16:28:36.653429 pip_audit-2.5.5/pip_audit/_format/__init__.py
--rw-r--r--   0        0        0     5318 2023-05-04 16:28:36.653429 pip_audit-2.5.5/pip_audit/_format/columns.py
--rw-r--r--   0        0        0     2957 2023-05-04 16:28:36.653429 pip_audit-2.5.5/pip_audit/_format/cyclonedx.py
--rw-r--r--   0        0        0     1119 2023-05-04 16:28:36.653429 pip_audit-2.5.5/pip_audit/_format/interface.py
--rw-r--r--   0        0        0     3160 2023-05-04 16:28:36.657429 pip_audit-2.5.5/pip_audit/_format/json.py
--rw-r--r--   0        0        0     4844 2023-05-04 16:28:36.657429 pip_audit-2.5.5/pip_audit/_format/markdown.py
--rw-r--r--   0        0        0      536 2023-05-04 16:28:36.657429 pip_audit-2.5.5/pip_audit/_service/__init__.py
--rw-r--r--   0        0        0     5265 2023-05-04 16:28:36.657429 pip_audit-2.5.5/pip_audit/_service/interface.py
--rw-r--r--   0        0        0     5898 2023-05-04 16:28:36.657429 pip_audit-2.5.5/pip_audit/_service/osv.py
--rw-r--r--   0        0        0     5047 2023-05-04 16:28:36.657429 pip_audit-2.5.5/pip_audit/_service/pypi.py
--rw-r--r--   0        0        0     8716 2023-05-04 16:28:36.657429 pip_audit-2.5.5/pip_audit/_state.py
--rw-r--r--   0        0        0     2332 2023-05-04 16:28:36.657429 pip_audit-2.5.5/pip_audit/_subprocess.py
--rw-r--r--   0        0        0      662 2023-05-04 16:28:36.657429 pip_audit-2.5.5/pip_audit/_util.py
--rw-r--r--   0        0        0     6326 2023-05-04 16:28:36.657429 pip_audit-2.5.5/pip_audit/_virtual_env.py
--rw-r--r--   0        0        0     3387 2023-05-04 16:28:36.657429 pip_audit-2.5.5/pyproject.toml
--rw-r--r--   0        0        0    23011 1970-01-01 00:00:00.000000 pip_audit-2.5.5/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-05-23 00:26:07.678217 pip_audit-2.5.6/LICENSE
+-rw-r--r--   0        0        0    20850 2023-05-23 00:26:07.682217 pip_audit-2.5.6/README.md
+-rw-r--r--   0        0        0       53 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/__main__.py
+-rw-r--r--   0        0        0     3158 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_audit.py
+-rw-r--r--   0        0        0     6214 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_cache.py
+-rw-r--r--   0        0        0    19415 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_cli.py
+-rw-r--r--   0        0        0      490 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_dependency_source/__init__.py
+-rw-r--r--   0        0        0     1552 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_dependency_source/interface.py
+-rw-r--r--   0        0        0     6853 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_dependency_source/pip.py
+-rw-r--r--   0        0        0     5416 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_dependency_source/pyproject.py
+-rw-r--r--   0        0        0    10810 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_dependency_source/requirement.py
+-rw-r--r--   0        0        0     3683 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_fix.py
+-rw-r--r--   0        0        0      380 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_format/__init__.py
+-rw-r--r--   0        0        0     5318 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_format/columns.py
+-rw-r--r--   0        0        0     2957 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_format/cyclonedx.py
+-rw-r--r--   0        0        0     1119 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_format/interface.py
+-rw-r--r--   0        0        0     3160 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_format/json.py
+-rw-r--r--   0        0        0     4844 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_format/markdown.py
+-rw-r--r--   0        0        0      536 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_service/__init__.py
+-rw-r--r--   0        0        0     5265 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_service/interface.py
+-rw-r--r--   0        0        0     5898 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_service/osv.py
+-rw-r--r--   0        0        0     5047 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_service/pypi.py
+-rw-r--r--   0        0        0     8716 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_state.py
+-rw-r--r--   0        0        0     2332 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_subprocess.py
+-rw-r--r--   0        0        0      662 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_util.py
+-rw-r--r--   0        0        0     6326 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_virtual_env.py
+-rw-r--r--   0        0        0     3400 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pyproject.toml
+-rw-r--r--   0        0        0    23048 1970-01-01 00:00:00.000000 pip_audit-2.5.6/PKG-INFO
```

### Comparing `pip_audit-2.5.5/LICENSE` & `pip_audit-2.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/README.md` & `pip_audit-2.5.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 `pip-audit` has [`pre-commit`](https://pre-commit.com/) support.
 
 For example, using `pip-audit` via `pre-commit` to audit a requirements file:
 
 ```yaml
   - repo: https://github.com/pypa/pip-audit
-    rev: v2.5.5
+    rev: v2.5.6
     hooks:
       -   id: pip-audit
           args: ["-r", "requirements.txt"]
 
 ci:
   # Leave pip-audit to only run locally and not in CI
   # pre-commit.ci does not allow network calls
```

### Comparing `pip_audit-2.5.5/pip_audit/_audit.py` & `pip_audit-2.5.6/pip_audit/_audit.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/pip_audit/_cache.py` & `pip_audit-2.5.6/pip_audit/_cache.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/pip_audit/_cli.py` & `pip_audit-2.5.6/pip_audit/_cli.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/pip_audit/_dependency_source/interface.py` & `pip_audit-2.5.6/pip_audit/_dependency_source/interface.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/pip_audit/_dependency_source/pip.py` & `pip_audit-2.5.6/pip_audit/_dependency_source/pip.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/pip_audit/_dependency_source/pyproject.py` & `pip_audit-2.5.6/pip_audit/_dependency_source/pyproject.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/pip_audit/_dependency_source/requirement.py` & `pip_audit-2.5.6/pip_audit/_dependency_source/requirement.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/pip_audit/_fix.py` & `pip_audit-2.5.6/pip_audit/_fix.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/pip_audit/_format/columns.py` & `pip_audit-2.5.6/pip_audit/_format/columns.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/pip_audit/_format/cyclonedx.py` & `pip_audit-2.5.6/pip_audit/_format/cyclonedx.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/pip_audit/_format/interface.py` & `pip_audit-2.5.6/pip_audit/_format/interface.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/pip_audit/_format/json.py` & `pip_audit-2.5.6/pip_audit/_format/json.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/pip_audit/_format/markdown.py` & `pip_audit-2.5.6/pip_audit/_format/markdown.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/pip_audit/_service/__init__.py` & `pip_audit-2.5.6/pip_audit/_service/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/pip_audit/_service/interface.py` & `pip_audit-2.5.6/pip_audit/_service/interface.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/pip_audit/_service/osv.py` & `pip_audit-2.5.6/pip_audit/_service/osv.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/pip_audit/_service/pypi.py` & `pip_audit-2.5.6/pip_audit/_service/pypi.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/pip_audit/_state.py` & `pip_audit-2.5.6/pip_audit/_state.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/pip_audit/_subprocess.py` & `pip_audit-2.5.6/pip_audit/_subprocess.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/pip_audit/_util.py` & `pip_audit-2.5.6/pip_audit/_util.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/pip_audit/_virtual_env.py` & `pip_audit-2.5.6/pip_audit/_virtual_env.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.5/pyproject.toml` & `pip_audit-2.5.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,38 +23,39 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Security",
 ]
 dependencies = [
-    "CacheControl[filecache]>=0.12.10",
+    "CacheControl[filecache] >= 0.12.0",
     # NOTE(ww): Release 2.5.0 is broken, subsequent 2.5.x releases fix it.
     # See: https://github.com/CycloneDX/cyclonedx-python-lib/issues/245
     "cyclonedx-python-lib ~= 2.0, != 2.5.0",
     "html5lib>=1.1",
     "packaging>=23.0.0",                     # https://github.com/pypa/pip-audit/issues/464
     "pip-api>=0.0.28",
     "pip-requirements-parser>=32.0.0",
-    # NOTE(ww): urllib3 2.0 and higher are incompatible with CacheControl;
-    # we prevent its use by using a version of requests that uses urllib3 < 2.0.
-    # See: https://github.com/psf/requests/issues/6437
-    "requests<2.30",
+    "requests >= 2.31.0",
+    # NOTE(ww): We constrain this subdepency because of CacheControl's incompatibility
+    # with urllib3 ~= 2.0 by way of requests.
+    # See: https://github.com/ionrock/cachecontrol/issues/292
+    "urllib3 ~= 1.26",
     "rich>=12.4",
     "toml>=0.10",
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 test = ["coverage[toml]", "pretend", "pytest", "pytest-cov"]
 lint = [
     "black>=22.3.0",
     # NOTE(ww): ruff is under active development, so we pin conservatively here
     # and let Dependabot periodically perform this update.
-    "ruff < 0.0.265",
+    "ruff < 0.0.270",
     "interrogate",
     "isort",
     "mypy",
     "types-html5lib",
     "types-requests",
     "types-toml",
 ]
```

### Comparing `pip_audit-2.5.5/PKG-INFO` & `pip_audit-2.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip_audit
-Version: 2.5.5
+Version: 2.5.6
 Summary: A tool for scanning Python environments for known vulnerabilities
 Author-email: Alex Cameron <alex.cameron@trailofbits.com>, Dustin Ingram <di@python.org>, William Woodruff <william@trailofbits.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,29 +12,30 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
-Requires-Dist: CacheControl[filecache]>=0.12.10
+Requires-Dist: CacheControl[filecache] >= 0.12.0
 Requires-Dist: cyclonedx-python-lib ~= 2.0, != 2.5.0
 Requires-Dist: html5lib>=1.1
 Requires-Dist: packaging>=23.0.0
 Requires-Dist: pip-api>=0.0.28
 Requires-Dist: pip-requirements-parser>=32.0.0
-Requires-Dist: requests<2.30
+Requires-Dist: requests >= 2.31.0
+Requires-Dist: urllib3 ~= 1.26
 Requires-Dist: rich>=12.4
 Requires-Dist: toml>=0.10
 Requires-Dist: build ; extra == "dev"
 Requires-Dist: bump>=1.3.2 ; extra == "dev"
 Requires-Dist: pip-audit[doc,test,lint] ; extra == "dev"
 Requires-Dist: pdoc ; extra == "doc"
 Requires-Dist: black>=22.3.0 ; extra == "lint"
-Requires-Dist: ruff < 0.0.265 ; extra == "lint"
+Requires-Dist: ruff < 0.0.270 ; extra == "lint"
 Requires-Dist: interrogate ; extra == "lint"
 Requires-Dist: isort ; extra == "lint"
 Requires-Dist: mypy ; extra == "lint"
 Requires-Dist: types-html5lib ; extra == "lint"
 Requires-Dist: types-requests ; extra == "lint"
 Requires-Dist: types-toml ; extra == "lint"
 Requires-Dist: coverage[toml] ; extra == "test"
@@ -153,15 +154,15 @@
 
 `pip-audit` has [`pre-commit`](https://pre-commit.com/) support.
 
 For example, using `pip-audit` via `pre-commit` to audit a requirements file:
 
 ```yaml
   - repo: https://github.com/pypa/pip-audit
-    rev: v2.5.5
+    rev: v2.5.6
     hooks:
       -   id: pip-audit
           args: ["-r", "requirements.txt"]
 
 ci:
   # Leave pip-audit to only run locally and not in CI
   # pre-commit.ci does not allow network calls
```

