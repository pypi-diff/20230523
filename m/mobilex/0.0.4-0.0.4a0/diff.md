# Comparing `tmp/mobilex-0.0.4.tar.gz` & `tmp/mobilex-0.0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobilex-0.0.4.tar", max compression
+gzip compressed data, was "mobilex-0.0.4a0.tar", max compression
```

## Comparing `mobilex-0.0.4.tar` & `mobilex-0.0.4a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1067 2023-05-23 05:42:56.800529 mobilex-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     1361 2023-05-23 05:43:12.312545 mobilex-0.0.4/README.md
--rw-r--r--   0        0        0      342 2023-05-23 05:42:56.800529 mobilex-0.0.4/mobilex/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 05:42:56.800529 mobilex-0.0.4/mobilex/cache/__init__.py
--rw-r--r--   0        0        0     3594 2023-05-23 05:42:56.800529 mobilex-0.0.4/mobilex/cache/base.py
--rw-r--r--   0        0        0     1880 2023-05-23 05:42:56.800529 mobilex-0.0.4/mobilex/cache/dict.py
--rw-r--r--   0        0        0     1765 2023-05-23 05:42:56.800529 mobilex-0.0.4/mobilex/cache/redis.py
--rw-r--r--   0        0        0      327 2023-05-23 05:42:56.800529 mobilex-0.0.4/mobilex/const.py
--rw-r--r--   0        0        0     4935 2023-05-23 05:42:56.800529 mobilex-0.0.4/mobilex/core.py
--rw-r--r--   0        0        0     1022 2023-05-23 05:42:56.800529 mobilex-0.0.4/mobilex/exc.py
--rw-r--r--   0        0        0     2516 2023-05-23 05:42:56.800529 mobilex-0.0.4/mobilex/response.py
--rw-r--r--   0        0        0     6057 2023-05-23 05:42:56.800529 mobilex-0.0.4/mobilex/router.py
--rw-r--r--   0        0        0      267 2023-05-23 05:42:56.800529 mobilex-0.0.4/mobilex/screens/__init__.py
--rw-r--r--   0        0        0    11671 2023-05-23 05:42:56.800529 mobilex-0.0.4/mobilex/screens/base.py
--rw-r--r--   0        0        0     6932 2023-05-23 05:42:56.800529 mobilex-0.0.4/mobilex/sessions.py
--rw-r--r--   0        0        0     1807 2023-05-23 05:42:56.800529 mobilex-0.0.4/mobilex/utils/__init__.py
--rw-r--r--   0        0        0     1881 2023-05-23 05:42:56.800529 mobilex-0.0.4/mobilex/utils/types.py
--rw-r--r--   0        0        0     1826 2023-05-23 05:42:56.800529 mobilex-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2161 1970-01-01 00:00:00.000000 mobilex-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/LICENSE.txt
+-rw-r--r--   0        0        0     1365 2023-05-23 05:26:31.482713 mobilex-0.0.4a0/README.md
+-rw-r--r--   0        0        0      342 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/cache/__init__.py
+-rw-r--r--   0        0        0     3594 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/cache/base.py
+-rw-r--r--   0        0        0     1880 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/cache/dict.py
+-rw-r--r--   0        0        0     1765 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/cache/redis.py
+-rw-r--r--   0        0        0      327 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/const.py
+-rw-r--r--   0        0        0     4935 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/core.py
+-rw-r--r--   0        0        0     1022 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/exc.py
+-rw-r--r--   0        0        0     2516 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/response.py
+-rw-r--r--   0        0        0     6057 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/router.py
+-rw-r--r--   0        0        0      267 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/screens/__init__.py
+-rw-r--r--   0        0        0    11671 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/screens/base.py
+-rw-r--r--   0        0        0     6932 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/sessions.py
+-rw-r--r--   0        0        0     1807 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/utils/__init__.py
+-rw-r--r--   0        0        0     1881 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/utils/types.py
+-rw-r--r--   0        0        0     1828 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/pyproject.toml
+-rw-r--r--   0        0        0     2167 1970-01-01 00:00:00.000000 mobilex-0.0.4a0/PKG-INFO
```

### Comparing `mobilex-0.0.4/LICENSE.txt` & `mobilex-0.0.4a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mobilex-0.0.4/README.md` & `mobilex-0.0.4a0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -38,8 +38,8 @@
 [pyversions-link]: https://pypi.python.org/pypi/mobilex
 [ci-image]: https://github.com/davidkyalo/python-mobilex/actions/workflows/workflow.yaml/badge.svg?event=push&branch=main
 [ci-link]: https://github.com/davidkyalo/python-mobilex/actions?query=workflow%3ACI%2FCD+event%3Apush+branch%3Amaster
 [codecov-image]: https://codecov.io/gh/davidkyalo/python-mobilex/branch/main/graph/badge.svg
 [codecov-link]: https://codecov.io/gh/davidkyalo/python-mobilex
 
 
-See this release on GitHub: [v0.0.4](https://github.com/davidkyalo/python-mobilex/releases/tag/0.0.4)
+See this release on GitHub: [v0.0.4a0](https://github.com/davidkyalo/python-mobilex/releases/tag/0.0.4a0)
```

### Comparing `mobilex-0.0.4/mobilex/cache/base.py` & `mobilex-0.0.4a0/mobilex/cache/base.py`

 * *Files identical despite different names*

### Comparing `mobilex-0.0.4/mobilex/cache/dict.py` & `mobilex-0.0.4a0/mobilex/cache/dict.py`

 * *Files identical despite different names*

### Comparing `mobilex-0.0.4/mobilex/cache/redis.py` & `mobilex-0.0.4a0/mobilex/cache/redis.py`

 * *Files identical despite different names*

### Comparing `mobilex-0.0.4/mobilex/core.py` & `mobilex-0.0.4a0/mobilex/core.py`

 * *Files identical despite different names*

### Comparing `mobilex-0.0.4/mobilex/exc.py` & `mobilex-0.0.4a0/mobilex/exc.py`

 * *Files identical despite different names*

### Comparing `mobilex-0.0.4/mobilex/response.py` & `mobilex-0.0.4a0/mobilex/response.py`

 * *Files identical despite different names*

### Comparing `mobilex-0.0.4/mobilex/router.py` & `mobilex-0.0.4a0/mobilex/router.py`

 * *Files identical despite different names*

### Comparing `mobilex-0.0.4/mobilex/screens/base.py` & `mobilex-0.0.4a0/mobilex/screens/base.py`

 * *Files identical despite different names*

### Comparing `mobilex-0.0.4/mobilex/sessions.py` & `mobilex-0.0.4a0/mobilex/sessions.py`

 * *Files identical despite different names*

### Comparing `mobilex-0.0.4/mobilex/utils/__init__.py` & `mobilex-0.0.4a0/mobilex/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mobilex-0.0.4/mobilex/utils/types.py` & `mobilex-0.0.4a0/mobilex/utils/types.py`

 * *Files identical despite different names*

### Comparing `mobilex-0.0.4/pyproject.toml` & `mobilex-0.0.4a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mobilex"
-version = "0.0.4"
+version = "0.0.4a0"
 description = "USSD and SMS exchange framework"
 authors = ["David Kyalo <davidmkyalo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/davidkyalo/python-mobilex"
 documentation = "https://davidkyalo.github.io/python-mobilex"
 keywords = [
```

### Comparing `mobilex-0.0.4/PKG-INFO` & `mobilex-0.0.4a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobilex
-Version: 0.0.4
+Version: 0.0.4a0
 Summary: USSD and SMS exchange framework
 Home-page: https://github.com/davidkyalo/python-mobilex
 License: MIT
 Keywords: mobilex,mobile,USSD,SMS
 Author: David Kyalo
 Author-email: davidmkyalo@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -59,9 +59,9 @@
 [pyversions-link]: https://pypi.python.org/pypi/mobilex
 [ci-image]: https://github.com/davidkyalo/python-mobilex/actions/workflows/workflow.yaml/badge.svg?event=push&branch=main
 [ci-link]: https://github.com/davidkyalo/python-mobilex/actions?query=workflow%3ACI%2FCD+event%3Apush+branch%3Amaster
 [codecov-image]: https://codecov.io/gh/davidkyalo/python-mobilex/branch/main/graph/badge.svg
 [codecov-link]: https://codecov.io/gh/davidkyalo/python-mobilex
 
 
-See this release on GitHub: [v0.0.4](https://github.com/davidkyalo/python-mobilex/releases/tag/0.0.4)
+See this release on GitHub: [v0.0.4a0](https://github.com/davidkyalo/python-mobilex/releases/tag/0.0.4a0)
```

