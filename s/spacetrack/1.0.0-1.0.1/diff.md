# Comparing `tmp/spacetrack-1.0.0.tar.gz` & `tmp/spacetrack-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetrack-1.0.0.tar", last modified: Mon May 22 16:46:43 2023, max compression
+gzip compressed data, was "spacetrack-1.0.1.tar", last modified: Tue May 23 13:47:04 2023, max compression
```

## Comparing `spacetrack-1.0.0.tar` & `spacetrack-1.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:46:43.165195 spacetrack-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-22 16:46:23.000000 spacetrack-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-22 16:46:23.000000 spacetrack-1.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-22 16:46:23.000000 spacetrack-1.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-22 16:46:23.000000 spacetrack-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-22 16:46:23.000000 spacetrack-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-22 16:46:43.165195 spacetrack-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-22 16:46:23.000000 spacetrack-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-22 16:46:23.000000 spacetrack-1.0.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:46:43.157195 spacetrack-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-05-22 16:46:23.000000 spacetrack-1.0.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-22 16:46:23.000000 spacetrack-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-22 16:46:23.000000 spacetrack-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-22 16:46:23.000000 spacetrack-1.0.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-22 16:46:23.000000 spacetrack-1.0.0/docs/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:46:43.161195 spacetrack-1.0.0/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-22 16:46:23.000000 spacetrack-1.0.0/docs/modules/aio.rst
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-22 16:46:23.000000 spacetrack-1.0.0/docs/modules/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-22 16:46:23.000000 spacetrack-1.0.0/docs/modules/operators.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-05-22 16:46:23.000000 spacetrack-1.0.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-22 16:46:23.000000 spacetrack-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-22 16:46:43.165195 spacetrack-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:46:43.153195 spacetrack-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:46:43.161195 spacetrack-1.0.0/src/spacetrack/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-22 16:46:23.000000 spacetrack-1.0.0/src/spacetrack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-22 16:46:23.000000 spacetrack-1.0.0/src/spacetrack/aio.py
--rw-r--r--   0 runner    (1001) docker     (123)    28440 2023-05-22 16:46:23.000000 spacetrack-1.0.0/src/spacetrack/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-22 16:46:23.000000 spacetrack-1.0.0/src/spacetrack/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:46:43.161195 spacetrack-1.0.0/src/spacetrack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-22 16:46:43.000000 spacetrack-1.0.0/src/spacetrack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-22 16:46:43.000000 spacetrack-1.0.0/src/spacetrack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:46:43.000000 spacetrack-1.0.0/src/spacetrack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-22 16:46:43.000000 spacetrack-1.0.0/src/spacetrack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-22 16:46:43.000000 spacetrack-1.0.0/src/spacetrack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:46:43.165195 spacetrack-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:46:23.000000 spacetrack-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-22 16:46:23.000000 spacetrack-1.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-22 16:46:23.000000 spacetrack-1.0.0/tests/test_aio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-22 16:46:23.000000 spacetrack-1.0.0/tests/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    16870 2023-05-22 16:46:23.000000 spacetrack-1.0.0/tests/test_spacetrack.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-22 16:46:23.000000 spacetrack-1.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:47:04.236090 spacetrack-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-23 13:46:48.000000 spacetrack-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-23 13:46:48.000000 spacetrack-1.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-23 13:46:48.000000 spacetrack-1.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-23 13:46:48.000000 spacetrack-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-23 13:46:48.000000 spacetrack-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-23 13:47:04.236090 spacetrack-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-23 13:46:48.000000 spacetrack-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-23 13:46:48.000000 spacetrack-1.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:47:04.232090 spacetrack-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-05-23 13:46:48.000000 spacetrack-1.0.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-23 13:46:48.000000 spacetrack-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-23 13:46:48.000000 spacetrack-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-23 13:46:48.000000 spacetrack-1.0.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-23 13:46:48.000000 spacetrack-1.0.1/docs/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:47:04.232090 spacetrack-1.0.1/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-23 13:46:48.000000 spacetrack-1.0.1/docs/modules/aio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 13:46:48.000000 spacetrack-1.0.1/docs/modules/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-23 13:46:48.000000 spacetrack-1.0.1/docs/modules/operators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-05-23 13:46:48.000000 spacetrack-1.0.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-23 13:46:48.000000 spacetrack-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-23 13:47:04.236090 spacetrack-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:47:04.232090 spacetrack-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:47:04.236090 spacetrack-1.0.1/src/spacetrack/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-23 13:46:48.000000 spacetrack-1.0.1/src/spacetrack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-05-23 13:46:48.000000 spacetrack-1.0.1/src/spacetrack/aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28651 2023-05-23 13:46:48.000000 spacetrack-1.0.1/src/spacetrack/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-23 13:46:48.000000 spacetrack-1.0.1/src/spacetrack/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:47:04.236090 spacetrack-1.0.1/src/spacetrack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-23 13:47:04.000000 spacetrack-1.0.1/src/spacetrack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-23 13:47:04.000000 spacetrack-1.0.1/src/spacetrack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:47:04.000000 spacetrack-1.0.1/src/spacetrack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-23 13:47:04.000000 spacetrack-1.0.1/src/spacetrack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 13:47:04.000000 spacetrack-1.0.1/src/spacetrack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:47:04.236090 spacetrack-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:46:48.000000 spacetrack-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-23 13:46:48.000000 spacetrack-1.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-23 13:46:48.000000 spacetrack-1.0.1/tests/test_aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-23 13:46:48.000000 spacetrack-1.0.1/tests/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16870 2023-05-23 13:46:48.000000 spacetrack-1.0.1/tests/test_spacetrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-23 13:46:48.000000 spacetrack-1.0.1/tox.ini
```

### Comparing `spacetrack-1.0.0/.pre-commit-config.yaml` & `spacetrack-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spacetrack-1.0.0/LICENSE.txt` & `spacetrack-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spacetrack-1.0.0/PKG-INFO` & `spacetrack-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacetrack
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python client for space-track.org
 Author-email: Frazer McLean <frazer@frazermclean.co.uk>
 License: MIT
 Project-URL: Repository, https://github.com/python-astrodynamics/spacetrack
 Project-URL: Documentation, https://spacetrack.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `spacetrack-1.0.0/README.rst` & `spacetrack-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `spacetrack-1.0.0/docs/changelog.rst` & `spacetrack-1.0.1/docs/changelog.rst`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,26 @@
 ==========
 
 Unreleased_
 -----------
 
 N/A
 
+1.0.1_ - 2023-05-23
+-------------------
+
+Fixed
+~~~~~
+
+- requests which should have been streamed (e.g. ``iter_content=True``) were
+  not.
+- requests which need to follow redirects work again.
+
 1.0.0_ - 2023-05-22
---------------------
+-------------------
 
 Added
 ~~~~~
 
 - :class:`~spacetrack.aio.AsyncSpaceTrackClient` supports Trio_ in addition to
   asyncio.
 
@@ -280,15 +290,16 @@
 -  ``Predicate`` class now has a ``default`` attribute.
 
 0.9.0_ - 2016-01-28
 -------------------
 
 First release.
 
-.. _Unreleased: https://github.com/python-astrodynamics/spacetrack/compare/1.0.0...HEAD
+.. _Unreleased: https://github.com/python-astrodynamics/spacetrack/compare/1.0.1...HEAD
+.. _1.0.1: https://github.com/python-astrodynamics/spacetrack/compare/1.0.0...1.0.1
 .. _1.0.0: https://github.com/python-astrodynamics/spacetrack/compare/0.16.0...1.0.0
 .. _0.16.0: https://github.com/python-astrodynamics/spacetrack/compare/0.15.0...0.16.0
 .. _0.15.0: https://github.com/python-astrodynamics/spacetrack/compare/0.14.0...0.15.0
 .. _0.14.0: https://github.com/python-astrodynamics/spacetrack/compare/0.13.7...0.14.0
 .. _0.13.7: https://github.com/python-astrodynamics/spacetrack/compare/0.13.6...0.13.7
 .. _0.13.6: https://github.com/python-astrodynamics/spacetrack/compare/0.13.5...0.13.6
 .. _0.13.5: https://github.com/python-astrodynamics/spacetrack/compare/0.13.4...0.13.5
```

### Comparing `spacetrack-1.0.0/docs/conf.py` & `spacetrack-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spacetrack-1.0.0/docs/usage.rst` & `spacetrack-1.0.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `spacetrack-1.0.0/pyproject.toml` & `spacetrack-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spacetrack"
-version = "1.0.0"
+version = "1.0.1"
 description = "Python client for space-track.org"
 readme = "README.rst"
 requires-python = ">=3.7"
 license = { text = "MIT" }
 authors = [
     { name = "Frazer McLean", email = "frazer@frazermclean.co.uk" },
 ]
```

### Comparing `spacetrack-1.0.0/src/spacetrack/aio.py` & `spacetrack-1.0.1/src/spacetrack/aio.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,19 @@
             rush_store=rush_store,
             rush_key_prefix=rush_key_prefix,
             httpx_client=httpx_client,
         )
 
     async def _handle_event(self, event):
         if isinstance(event, NormalRequest):
-            return await self.client.send(event.request)
+            return await self.client.send(
+                event.request,
+                follow_redirects=event.follow_redirects,
+                stream=event.stream,
+            )
         elif isinstance(event, ReadResponse):
             return await event.response.aread()
         elif isinstance(event, IterLines):
             return _iter_lines_generator(event.response)
         elif isinstance(event, IterContent):
             return _iter_content_generator(event.response, event.decode)
         elif isinstance(event, RateLimitWait):
```

### Comparing `spacetrack-1.0.0/src/spacetrack/base.py` & `spacetrack-1.0.1/src/spacetrack/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     pass
 
 
 @attr.s(slots=True)
 class NormalRequest(Event):
     request = attr.ib()
     stream = attr.ib(default=False)
+    follow_redirects = attr.ib(default=False)
 
 
 @attr.s(slots=True)
 class ReadResponse(Event):
     response = attr.ib()
 
 
@@ -292,15 +293,19 @@
 
     @base_url.setter
     def base_url(self, url):
         self.client.base_url = url
 
     def _handle_event(self, event):
         if isinstance(event, NormalRequest):
-            return self.client.send(event.request)
+            return self.client.send(
+                event.request,
+                follow_redirects=event.follow_redirects,
+                stream=event.stream,
+            )
         elif isinstance(event, ReadResponse):
             return event.response.read()
         elif isinstance(event, IterLines):
             return _iter_lines_generator(event.response)
         elif isinstance(event, IterContent):
             return _iter_content_generator(event.response, event.decode)
         elif isinstance(event, RateLimitWait):
@@ -568,15 +573,16 @@
 
         if hour_limit.limited:
             sleep_time = max(sleep_time, hour_limit.retry_after.total_seconds())
 
         if sleep_time > 0:
             yield RateLimitWait(sleep_time)
 
-        resp = yield NormalRequest(request, stream=stream)
+        req_event = NormalRequest(request, stream=stream, follow_redirects=True)
+        resp = yield req_event
 
         # It's possible that Space-Track will return HTTP status 500 with a
         # query rate limit violation. This can happen if a script is cancelled
         # before it has finished sleeping to satisfy the rate limit and it is
         # started again.
         #
         # Let's catch this specific instance and retry once if it happens.
@@ -587,15 +593,15 @@
             if "violated your query rate limit" in resp.text:
                 # It seems that only the per-minute rate limit causes an HTTP
                 # 500 error. Breaking the per-hour limit seems to result in an
                 # email from Space-Track instead.
                 yield RateLimitWait(
                     self._per_minute_throttle.rate.period.total_seconds()
                 )
-                resp = yield NormalRequest(request)
+                resp = yield req_event
 
         return resp
 
     def _ratelimit_callback(self, until):
         duration = int(round(until - time.monotonic()))
         logger.info("Rate limit reached. Sleeping for {:d} seconds.", duration)
```

### Comparing `spacetrack-1.0.0/src/spacetrack/operators.py` & `spacetrack-1.0.1/src/spacetrack/operators.py`

 * *Files identical despite different names*

### Comparing `spacetrack-1.0.0/src/spacetrack.egg-info/PKG-INFO` & `spacetrack-1.0.1/src/spacetrack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacetrack
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python client for space-track.org
 Author-email: Frazer McLean <frazer@frazermclean.co.uk>
 License: MIT
 Project-URL: Repository, https://github.com/python-astrodynamics/spacetrack
 Project-URL: Documentation, https://spacetrack.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `spacetrack-1.0.0/src/spacetrack.egg-info/SOURCES.txt` & `spacetrack-1.0.1/src/spacetrack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spacetrack-1.0.0/tests/conftest.py` & `spacetrack-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spacetrack-1.0.0/tests/test_aio.py` & `spacetrack-1.0.1/tests/test_aio.py`

 * *Files identical despite different names*

### Comparing `spacetrack-1.0.0/tests/test_operators.py` & `spacetrack-1.0.1/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `spacetrack-1.0.0/tests/test_spacetrack.py` & `spacetrack-1.0.1/tests/test_spacetrack.py`

 * *Files identical despite different names*

### Comparing `spacetrack-1.0.0/tox.ini` & `spacetrack-1.0.1/tox.ini`

 * *Files identical despite different names*

