# Comparing `tmp/duty-0.8.0.tar.gz` & `tmp/duty-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duty-0.8.0.tar", last modified: Sat Feb 18 17:15:04 2023, max compression
+gzip compressed data, was "duty-0.9.0.tar", last modified: Tue Mar  7 19:39:11 2023, max compression
```

## Comparing `duty-0.8.0.tar` & `duty-0.9.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0      754 2023-02-10 13:44:22.417580 duty-0.8.0/LICENSE
--rw-r--r--   0        0        0     1218 2023-02-10 13:44:22.544245 duty-0.8.0/README.md
--rw-r--r--   0        0        0     2340 2023-02-18 16:32:20.386549 duty-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      144 2023-02-17 18:11:48.491654 duty-0.8.0/src/duty/__init__.py
--rw-r--r--   0        0        0      333 2023-02-17 18:11:53.968235 duty-0.8.0/src/duty/__main__.py
--rw-r--r--   0        0        0     2285 2023-02-18 16:25:12.282914 duty-0.8.0/src/duty/callables/__init__.py
--rw-r--r--   0        0        0      367 2023-02-17 17:16:47.840819 duty-0.8.0/src/duty/callables/_io.py
--rw-r--r--   0        0        0     4699 2023-02-18 16:09:01.647898 duty-0.8.0/src/duty/callables/autoflake.py
--rw-r--r--   0        0        0     7148 2023-02-18 16:14:20.452821 duty-0.8.0/src/duty/callables/black.py
--rw-r--r--   0        0        0     3199 2023-02-18 16:30:23.551614 duty-0.8.0/src/duty/callables/blacken_docs.py
--rw-r--r--   0        0        0    23941 2023-02-18 16:19:55.114352 duty-0.8.0/src/duty/callables/coverage.py
--rw-r--r--   0        0        0     8608 2023-02-18 16:14:20.452821 duty-0.8.0/src/duty/callables/flake8.py
--rw-r--r--   0        0        0    26580 2023-02-18 16:14:20.456154 duty-0.8.0/src/duty/callables/isort.py
--rw-r--r--   0        0        0     7882 2023-02-18 16:14:20.456154 duty-0.8.0/src/duty/callables/mkdocs.py
--rw-r--r--   0        0        0    19925 2023-02-18 16:14:20.452821 duty-0.8.0/src/duty/callables/mypy.py
--rw-r--r--   0        0        0    18523 2023-02-18 16:14:20.452821 duty-0.8.0/src/duty/callables/pytest.py
--rw-r--r--   0        0        0    10053 2023-02-18 16:14:20.456154 duty-0.8.0/src/duty/callables/ruff.py
--rw-r--r--   0        0        0     2217 2023-02-18 15:32:33.711095 duty-0.8.0/src/duty/callables/safety.py
--rw-r--r--   0        0        0     7966 2023-02-17 17:06:32.914465 duty-0.8.0/src/duty/cli.py
--rw-r--r--   0        0        0     6512 2023-02-17 18:11:29.418617 duty-0.8.0/src/duty/collection.py
--rw-r--r--   0        0        0     2984 2023-02-17 18:11:30.915261 duty-0.8.0/src/duty/context.py
--rw-r--r--   0        0        0     3021 2023-02-17 18:10:17.209735 duty-0.8.0/src/duty/decorator.py
--rw-r--r--   0        0        0      358 2023-02-17 18:11:31.715248 duty-0.8.0/src/duty/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-10 13:44:22.317582 duty-0.8.0/src/duty/py.typed
--rw-r--r--   0        0        0     6288 2023-02-17 18:11:43.025072 duty-0.8.0/src/duty/validation.py
--rw-r--r--   0        0        0      157 2023-02-10 13:44:22.314249 duty-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0       47 2023-02-10 13:44:22.314249 duty-0.8.0/tests/conftest.py
--rw-r--r--   0        0        0      130 2021-06-18 16:29:00.138929 duty-0.8.0/tests/fixtures/arguments.py
--rw-r--r--   0        0        0       55 2021-06-18 16:29:00.155592 duty-0.8.0/tests/fixtures/basic.py
--rw-r--r--   0        0        0      105 2021-06-18 16:29:00.155592 duty-0.8.0/tests/fixtures/booleans.py
--rw-r--r--   0        0        0       82 2021-06-18 16:29:00.172255 duty-0.8.0/tests/fixtures/code.py
--rw-r--r--   0        0        0      102 2021-06-18 16:29:00.172255 duty-0.8.0/tests/fixtures/list.py
--rw-r--r--   0        0        0      180 2021-06-18 16:29:00.182252 duty-0.8.0/tests/fixtures/multiple.py
--rw-r--r--   0        0        0      121 2021-06-18 16:29:00.182252 duty-0.8.0/tests/fixtures/precedence.py
--rw-r--r--   0        0        0      538 2021-07-19 11:03:47.419786 duty-0.8.0/tests/fixtures/validation.py
--rw-r--r--   0        0        0      335 2023-02-10 14:56:32.165244 duty-0.8.0/tests/fixtures/validation_38.py
--rw-r--r--   0        0        0     6115 2023-02-18 16:46:57.022899 duty-0.8.0/tests/test_cli.py
--rw-r--r--   0        0        0     1918 2023-02-18 16:46:57.019566 duty-0.8.0/tests/test_collection.py
--rw-r--r--   0        0        0     3181 2023-02-18 16:46:57.022899 duty-0.8.0/tests/test_context.py
--rw-r--r--   0        0        0      682 2023-02-18 16:46:57.019566 duty-0.8.0/tests/test_decorator.py
--rw-r--r--   0        0        0     3022 2023-02-18 16:46:57.036232 duty-0.8.0/tests/test_running.py
--rw-r--r--   0        0        0     5386 2023-02-18 16:46:57.019566 duty-0.8.0/tests/test_validation.py
--rw-r--r--   0        0        0     2576 1970-01-01 00:00:00.000000 duty-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-02-18 18:32:06.812496 duty-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1218 2023-02-18 18:32:07.099158 duty-0.9.0/README.md
+-rw-r--r--   0        0        0     2338 2023-02-18 18:32:07.099158 duty-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      144 2023-02-18 18:32:07.099158 duty-0.9.0/src/duty/__init__.py
+-rw-r--r--   0        0        0      333 2023-02-18 18:32:05.312520 duty-0.9.0/src/duty/__main__.py
+-rw-r--r--   0        0        0     2285 2023-02-18 16:25:12.282914 duty-0.9.0/src/duty/callables/__init__.py
+-rw-r--r--   0        0        0      367 2023-02-17 17:16:47.840819 duty-0.9.0/src/duty/callables/_io.py
+-rw-r--r--   0        0        0     4699 2023-02-18 16:09:01.647898 duty-0.9.0/src/duty/callables/autoflake.py
+-rw-r--r--   0        0        0     7148 2023-02-18 16:14:20.452821 duty-0.9.0/src/duty/callables/black.py
+-rw-r--r--   0        0        0     3216 2023-03-07 19:38:39.771702 duty-0.9.0/src/duty/callables/blacken_docs.py
+-rw-r--r--   0        0        0    23941 2023-02-18 16:19:55.114352 duty-0.9.0/src/duty/callables/coverage.py
+-rw-r--r--   0        0        0     8608 2023-02-18 16:14:20.452821 duty-0.9.0/src/duty/callables/flake8.py
+-rw-r--r--   0        0        0     5203 2023-03-03 14:18:24.951319 duty-0.9.0/src/duty/callables/interrogate.py
+-rw-r--r--   0        0        0    26580 2023-02-18 16:14:20.456154 duty-0.9.0/src/duty/callables/isort.py
+-rw-r--r--   0        0        0     7882 2023-02-18 16:14:20.456154 duty-0.9.0/src/duty/callables/mkdocs.py
+-rw-r--r--   0        0        0    19925 2023-02-18 16:14:20.452821 duty-0.9.0/src/duty/callables/mypy.py
+-rw-r--r--   0        0        0    18523 2023-02-18 16:14:20.452821 duty-0.9.0/src/duty/callables/pytest.py
+-rw-r--r--   0        0        0    10053 2023-02-18 16:14:20.456154 duty-0.9.0/src/duty/callables/ruff.py
+-rw-r--r--   0        0        0     2217 2023-02-18 15:32:33.711095 duty-0.9.0/src/duty/callables/safety.py
+-rw-r--r--   0        0        0     7966 2023-02-18 18:32:07.099158 duty-0.9.0/src/duty/cli.py
+-rw-r--r--   0        0        0     6512 2023-02-17 18:11:29.418617 duty-0.9.0/src/duty/collection.py
+-rw-r--r--   0        0        0     2984 2023-02-17 18:11:30.915261 duty-0.9.0/src/duty/context.py
+-rw-r--r--   0        0        0     3021 2023-02-17 18:10:17.209735 duty-0.9.0/src/duty/decorator.py
+-rw-r--r--   0        0        0      358 2023-02-17 18:11:31.715248 duty-0.9.0/src/duty/exceptions.py
+-rw-r--r--   0        0        0        0 2023-02-18 18:32:04.939193 duty-0.9.0/src/duty/py.typed
+-rw-r--r--   0        0        0     6288 2023-02-17 18:11:43.025072 duty-0.9.0/src/duty/validation.py
+-rw-r--r--   0        0        0      157 2023-02-18 18:32:04.925860 duty-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0       47 2023-02-18 18:32:04.919193 duty-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0      130 2021-06-18 16:29:00.138929 duty-0.9.0/tests/fixtures/arguments.py
+-rw-r--r--   0        0        0       55 2021-06-18 16:29:00.155592 duty-0.9.0/tests/fixtures/basic.py
+-rw-r--r--   0        0        0      105 2021-06-18 16:29:00.155592 duty-0.9.0/tests/fixtures/booleans.py
+-rw-r--r--   0        0        0       82 2021-06-18 16:29:00.172255 duty-0.9.0/tests/fixtures/code.py
+-rw-r--r--   0        0        0      102 2021-06-18 16:29:00.172255 duty-0.9.0/tests/fixtures/list.py
+-rw-r--r--   0        0        0      180 2021-06-18 16:29:00.182252 duty-0.9.0/tests/fixtures/multiple.py
+-rw-r--r--   0        0        0      121 2021-06-18 16:29:00.182252 duty-0.9.0/tests/fixtures/precedence.py
+-rw-r--r--   0        0        0      538 2021-07-19 11:03:47.419786 duty-0.9.0/tests/fixtures/validation.py
+-rw-r--r--   0        0        0      335 2023-02-10 14:56:32.165244 duty-0.9.0/tests/fixtures/validation_38.py
+-rw-r--r--   0        0        0     6115 2023-02-18 18:32:07.099158 duty-0.9.0/tests/test_cli.py
+-rw-r--r--   0        0        0     1918 2023-02-18 16:46:57.019566 duty-0.9.0/tests/test_collection.py
+-rw-r--r--   0        0        0     3181 2023-02-18 16:46:57.022899 duty-0.9.0/tests/test_context.py
+-rw-r--r--   0        0        0      682 2023-02-18 16:46:57.019566 duty-0.9.0/tests/test_decorator.py
+-rw-r--r--   0        0        0     3022 2023-02-18 16:46:57.036232 duty-0.9.0/tests/test_running.py
+-rw-r--r--   0        0        0     5386 2023-02-18 16:46:57.019566 duty-0.9.0/tests/test_validation.py
+-rw-r--r--   0        0        0     2576 1970-01-01 00:00:00.000000 duty-0.9.0/PKG-INFO
```

### Comparing `duty-0.8.0/LICENSE` & `duty-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/README.md` & `duty-0.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Duty
+# duty
 
 [![ci](https://github.com/pawamoy/duty/workflows/ci/badge.svg)](https://github.com/pawamoy/duty/actions?query=workflow%3Aci)
 [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://pawamoy.github.io/duty/)
 [![pypi version](https://img.shields.io/pypi/v/duty.svg)](https://pypi.org/project/duty/)
 [![gitpod](https://img.shields.io/badge/gitpod-workspace-blue.svg?style=flat)](https://gitpod.io/#https://github.com/pawamoy/duty)
 [![gitter](https://badges.gitter.im/join%20chat.svg)](https://gitter.im/duty/community)
```

### Comparing `duty-0.8.0/pyproject.toml` & `duty-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "Typing :: Typed",
 ]
 dependencies = [
     "failprint>=0.10",
     "cached-property>=1.5; python_version < '3.8'",
     "typing-extensions>=4.5; python_version < '3.8'",
 ]
-version = "0.8.0"
+version = "0.9.0"
 
 [project.urls]
 Homepage = "https://pawamoy.github.io/duty"
 Documentation = "https://pawamoy.github.io/duty"
 Changelog = "https://pawamoy.github.io/duty/changelog"
 Repository = "https://github.com/pawamoy/duty"
 Issues = "https://github.com/pawamoy/duty/issues"
@@ -74,15 +74,15 @@
     "mkdocstrings[python]>=0.18",
     "markdown-callouts>=0.2",
     "markdown-exec>=0.5",
     "toml>=0.10",
 ]
 maintain = [
     "black>=23.1",
-    "blacken-docs>=1.13.0",
+    "blacken-docs>=1.13",
     "git-changelog>=1.0",
 ]
 quality = [
     "ruff>=0.0.246",
 ]
 tests = [
     "pytest>=6.2",
```

### Comparing `duty-0.8.0/src/duty/callables/__init__.py` & `duty-0.9.0/src/duty/callables/__init__.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/src/duty/callables/autoflake.py` & `duty-0.9.0/src/duty/callables/autoflake.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/src/duty/callables/black.py` & `duty-0.9.0/src/duty/callables/black.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/src/duty/callables/blacken_docs.py` & `duty-0.9.0/src/duty/callables/blacken_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     from blacken_docs import format_file
 
     exts = ("md", "py") if exts is None else tuple(ext.lstrip(".") for ext in exts)
     if exclude:
         exclude = tuple(re.compile(regex, re.I) if isinstance(regex, str) else regex for regex in exclude)
     filepaths = set()
     for path in paths:
-        path = Path(path)
+        path = Path(path)  # noqa: PLW2901
         if path.is_file():
             filepaths.add(path.as_posix())
         else:
             for ext in exts:
                 filepaths |= {filepath.as_posix() for filepath in path.rglob(f"*.{ext}")}
 
     black_mode = black.Mode(
```

### Comparing `duty-0.8.0/src/duty/callables/coverage.py` & `duty-0.9.0/src/duty/callables/coverage.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/src/duty/callables/flake8.py` & `duty-0.9.0/src/duty/callables/flake8.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/src/duty/callables/isort.py` & `duty-0.9.0/src/duty/callables/isort.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/src/duty/callables/mkdocs.py` & `duty-0.9.0/src/duty/callables/mkdocs.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/src/duty/callables/mypy.py` & `duty-0.9.0/src/duty/callables/mypy.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/src/duty/callables/pytest.py` & `duty-0.9.0/src/duty/callables/pytest.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/src/duty/callables/ruff.py` & `duty-0.9.0/src/duty/callables/ruff.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/src/duty/callables/safety.py` & `duty-0.9.0/src/duty/callables/safety.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/src/duty/cli.py` & `duty-0.9.0/src/duty/cli.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/src/duty/collection.py` & `duty-0.9.0/src/duty/collection.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/src/duty/context.py` & `duty-0.9.0/src/duty/context.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/src/duty/decorator.py` & `duty-0.9.0/src/duty/decorator.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/src/duty/validation.py` & `duty-0.9.0/src/duty/validation.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/tests/fixtures/validation.py` & `duty-0.9.0/tests/fixtures/validation.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/tests/test_cli.py` & `duty-0.9.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/tests/test_collection.py` & `duty-0.9.0/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/tests/test_context.py` & `duty-0.9.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/tests/test_decorator.py` & `duty-0.9.0/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/tests/test_running.py` & `duty-0.9.0/tests/test_running.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/tests/test_validation.py` & `duty-0.9.0/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `duty-0.8.0/PKG-INFO` & `duty-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duty
-Version: 0.8.0
+Version: 0.9.0
 Summary: A simple task runner.
 License: ISC
 Keywords: task-runner,task,runner,cross-platform
 Author-email: Timothée Mazzucotelli <pawamoy@pm.me>
 Requires-Python: >=3.7
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -26,15 +26,15 @@
 Project-URL: Funding, https://github.com/sponsors/pawamoy
 Project-URL: Gitter, https://gitter.im/duty/community
 Project-URL: Homepage, https://pawamoy.github.io/duty
 Project-URL: Issues, https://github.com/pawamoy/duty/issues
 Project-URL: Repository, https://github.com/pawamoy/duty
 Description-Content-Type: text/markdown
 
-# Duty
+# duty
 
 [![ci](https://github.com/pawamoy/duty/workflows/ci/badge.svg)](https://github.com/pawamoy/duty/actions?query=workflow%3Aci)
 [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://pawamoy.github.io/duty/)
 [![pypi version](https://img.shields.io/pypi/v/duty.svg)](https://pypi.org/project/duty/)
 [![gitpod](https://img.shields.io/badge/gitpod-workspace-blue.svg?style=flat)](https://gitpod.io/#https://github.com/pawamoy/duty)
 [![gitter](https://badges.gitter.im/join%20chat.svg)](https://gitter.im/duty/community)
```

