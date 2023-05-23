# Comparing `tmp/lacuscore-1.4.8.tar.gz` & `tmp/lacuscore-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacuscore-1.4.8.tar", max compression
+gzip compressed data, was "lacuscore-1.4.9.tar", max compression
```

## Comparing `lacuscore-1.4.8.tar` & `lacuscore-1.4.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.4.8/LICENSE
--rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.4.8/README.md
--rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.4.8/lacuscore/__init__.py
--rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.4.8/lacuscore/lacus_monitoring.py
--rw-r--r--   0        0        0    28070 2023-04-11 13:29:09.084489 lacuscore-1.4.8/lacuscore/lacuscore.py
--rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.4.8/lacuscore/py.typed
--rw-r--r--   0        0        0     1516 2023-04-12 11:36:31.465532 lacuscore-1.4.8/pyproject.toml
--rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 lacuscore-1.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.4.9/LICENSE
+-rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.4.9/README.md
+-rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.4.9/lacuscore/__init__.py
+-rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.4.9/lacuscore/lacus_monitoring.py
+-rw-r--r--   0        0        0    28455 2023-04-14 13:46:44.792327 lacuscore-1.4.9/lacuscore/lacuscore.py
+-rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.4.9/lacuscore/py.typed
+-rw-r--r--   0        0        0     1516 2023-04-14 13:47:44.812598 lacuscore-1.4.9/pyproject.toml
+-rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 lacuscore-1.4.9/PKG-INFO
```

### Comparing `lacuscore-1.4.8/LICENSE` & `lacuscore-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lacuscore-1.4.8/README.md` & `lacuscore-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `lacuscore-1.4.8/lacuscore/lacus_monitoring.py` & `lacuscore-1.4.9/lacuscore/lacus_monitoring.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.4.8/lacuscore/lacuscore.py` & `lacuscore-1.4.9/lacuscore/lacuscore.py`

 * *Files 2% similar despite different names*

```diff
@@ -507,25 +507,30 @@
                 else:
                     browser_engine = 'webkit'
 
             try:
                 logger.debug(f'Capturing {url}')
                 # NOTE: starting with python 3.11, we can use asyncio.timeout
                 # async with asyncio.timeout(self.max_capture_time):
+                general_timeout = to_capture.get('general_timeout_in_sec')
                 async with Capture(
                         browser=browser_engine,
                         device_name=to_capture.get('device_name'),
                         proxy=proxy,
-                        general_timeout_in_sec=to_capture.get('general_timeout_in_sec')) as capture:
+                        general_timeout_in_sec=general_timeout) as capture:
                     # required by Mypy: https://github.com/python/mypy/issues/3004
                     capture.headers = to_capture.get('headers')  # type: ignore
                     capture.cookies = to_capture.get('cookies')  # type: ignore
                     capture.viewport = to_capture.get('viewport')  # type: ignore
                     capture.user_agent = to_capture.get('user_agent')  # type: ignore
-                    await capture.initialize_context()
+                    try:
+                        await asyncio.wait_for(capture.initialize_context(), timeout=general_timeout)
+                    except (TimeoutError, asyncio.exceptions.TimeoutError):
+                        logger.warning(f'Initializing the context for {url} took longer than the allowed general timeout ({general_timeout}s)')
+                        raise RetryCapture
                     playwright_result = await asyncio.wait_for(
                         capture.capture_page(
                             url, referer=to_capture.get('referer'),
                             depth=to_capture.get('depth', 0),
                             rendered_hostname_only=to_capture.get('rendered_hostname_only', True),
                             max_depth_capture_time=self.max_capture_time),
                         timeout=self.max_capture_time)
```

### Comparing `lacuscore-1.4.8/pyproject.toml` & `lacuscore-1.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacuscore"
-version = "1.4.8"
+version = "1.4.9"
 description = "Core of Lacus, usable as a module"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ail-project/LacusCore"
 documentation = "https://lacuscore.readthedocs.io/en/latest/"
 
 readme = "README.md"
```

### Comparing `lacuscore-1.4.8/PKG-INFO` & `lacuscore-1.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lacuscore
-Version: 1.4.8
+Version: 1.4.9
 Summary: Core of Lacus, usable as a module
 Home-page: https://github.com/ail-project/LacusCore
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

