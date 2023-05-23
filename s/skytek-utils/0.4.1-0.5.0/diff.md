# Comparing `tmp/skytek-utils-0.4.1.tar.gz` & `tmp/skytek-utils-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skytek-utils-0.4.1.tar", last modified: Fri May 19 12:07:06 2023, max compression
+gzip compressed data, was "skytek-utils-0.5.0.tar", last modified: Tue May 23 20:15:25 2023, max compression
```

## Comparing `skytek-utils-0.4.1.tar` & `skytek-utils-0.5.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:07:06.772829 skytek-utils-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-19 12:07:06.768829 skytek-utils-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:07:06.768829 skytek-utils-0.4.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/requirements/lint.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 12:07:06.772829 skytek-utils-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:07:06.768829 skytek-utils-0.4.1/skytek_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 12:06:59.000000 skytek-utils-0.4.1/skytek_utils/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/skytek_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/skytek_utils/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/skytek_utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:07:06.768829 skytek-utils-0.4.1/skytek_utils/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/skytek_utils/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/skytek_utils/django/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/skytek_utils/django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/skytek_utils/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:07:06.768829 skytek-utils-0.4.1/skytek_utils/interconnect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/skytek_utils/interconnect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:07:06.768829 skytek-utils-0.4.1/skytek_utils/interconnect/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/skytek_utils/interconnect/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/skytek_utils/interconnect/api/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/skytek_utils/interconnect/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/skytek_utils/interconnect/api/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/skytek_utils/interconnect/api/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/skytek_utils/interconnect/api/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/skytek_utils/interconnect/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/skytek_utils/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/skytek_utils/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:07:06.768829 skytek-utils-0.4.1/skytek_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-19 12:07:06.000000 skytek-utils-0.4.1/skytek_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-19 12:07:06.000000 skytek-utils-0.4.1/skytek_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:07:06.000000 skytek-utils-0.4.1/skytek_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:07:06.000000 skytek-utils-0.4.1/skytek_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-19 12:07:06.000000 skytek-utils-0.4.1/skytek_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-19 12:07:06.000000 skytek-utils-0.4.1/skytek_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:07:06.768829 skytek-utils-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-19 12:06:57.000000 skytek-utils-0.4.1/tests/test_iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:15:25.258721 skytek-utils-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-23 20:15:25.258721 skytek-utils-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:15:25.254721 skytek-utils-0.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/requirements/lint.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 20:15:25.258721 skytek-utils-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:15:25.254721 skytek-utils-0.5.0/skytek_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 20:15:17.000000 skytek-utils-0.5.0/skytek_utils/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/skytek_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/skytek_utils/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/skytek_utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:15:25.258721 skytek-utils-0.5.0/skytek_utils/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/skytek_utils/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/skytek_utils/django/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/skytek_utils/django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/skytek_utils/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:15:25.258721 skytek-utils-0.5.0/skytek_utils/interconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/skytek_utils/interconnect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:15:25.258721 skytek-utils-0.5.0/skytek_utils/interconnect/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/skytek_utils/interconnect/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/skytek_utils/interconnect/api/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/skytek_utils/interconnect/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/skytek_utils/interconnect/api/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/skytek_utils/interconnect/api/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/skytek_utils/interconnect/api/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/skytek_utils/interconnect/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/skytek_utils/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/skytek_utils/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:15:25.258721 skytek-utils-0.5.0/skytek_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-23 20:15:25.000000 skytek-utils-0.5.0/skytek_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-23 20:15:25.000000 skytek-utils-0.5.0/skytek_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:15:25.000000 skytek-utils-0.5.0/skytek_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:15:25.000000 skytek-utils-0.5.0/skytek_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-23 20:15:25.000000 skytek-utils-0.5.0/skytek_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 20:15:25.000000 skytek-utils-0.5.0/skytek_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:15:25.258721 skytek-utils-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-23 20:15:14.000000 skytek-utils-0.5.0/tests/test_iter.py
```

### Comparing `skytek-utils-0.4.1/LICENSE` & `skytek-utils-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.4.1/PKG-INFO` & `skytek-utils-0.5.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytek-utils
-Version: 0.4.1
+Version: 0.5.0
 Summary: skytek-utils - a set of small util functions
 Home-page: http://github.com/Skytek/skytek-utils
 Author: Skytek Ltd.
 Author-email: wiktor.latanowicz@skytek.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `skytek-utils-0.4.1/setup.py` & `skytek-utils-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.4.1/skytek_utils/celery.py` & `skytek-utils-0.5.0/skytek_utils/celery.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.4.1/skytek_utils/datetime.py` & `skytek-utils-0.5.0/skytek_utils/datetime.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.4.1/skytek_utils/interconnect/api/authentication.py` & `skytek-utils-0.5.0/skytek_utils/interconnect/api/authentication.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.4.1/skytek_utils/interconnect/api/client.py` & `skytek-utils-0.5.0/skytek_utils/interconnect/api/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,17 +17,20 @@
         protocol = (
             "https" if getattr(settings, "INTERCONNECT_USE_SSL", True) else "http"
         )
         if not path.startswith("/"):
             path = f"/{path}"
         return f"{protocol}://{host}{path}"
 
-    def _call_api(self, method, path, *args, **kwargs):
-        method_function = getattr(requests, method)
+    def _call_api_by_path(self, method, path, *args, **kwargs):
         url = self._make_url(path)
+        return self._call_api(method, url, *args, **kwargs)
+
+    def _call_api(self, method, url, *args, **kwargs):
+        method_function = getattr(requests, method)
         headers = {
             **kwargs.pop("headers", {}),
             **self._make_headers(),
         }
         result = method_function(
             url,
             *args,
@@ -40,17 +43,30 @@
         jwt = generate_jwt()
         headers = {
             "Authorization": f"Bearer {jwt}",
         }
         return headers
 
     def get(self, path, *args, **kwargs):
-        return self._call_api("get", path, *args, **kwargs)
+        return self._call_api_by_path("get", path, *args, **kwargs)
 
     def post(self, path, *args, **kwargs):
-        return self._call_api("post", path, *args, **kwargs)
+        return self._call_api_by_path("post", path, *args, **kwargs)
 
     def patch(self, path, *args, **kwargs):
-        return self._call_api("patch", path, *args, **kwargs)
+        return self._call_api_by_path("patch", path, *args, **kwargs)
 
     def delete(self, path, *args, **kwargs):
-        return self._call_api("delete", path, *args, **kwargs)
+        return self._call_api_by_path("delete", path, *args, **kwargs)
+
+    def get_all(self, path, *args, **kwargs):
+        url = self._make_url(path)
+        while url:
+            result = self._call_api("get", *args, **kwargs)
+            result.raise_for_status()
+            response = result.json()
+
+            yield from response["result"]
+
+            url = response.get("next")
+            if "query" in kwargs:
+                del kwargs["query"]
```

### Comparing `skytek-utils-0.4.1/skytek_utils/interconnect/api/jwt.py` & `skytek-utils-0.5.0/skytek_utils/interconnect/api/jwt.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.4.1/skytek_utils/interconnect/api/mixins.py` & `skytek-utils-0.5.0/skytek_utils/interconnect/api/mixins.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.4.1/skytek_utils/interconnect/api/permissions.py` & `skytek-utils-0.5.0/skytek_utils/interconnect/api/permissions.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.4.1/skytek_utils/monitoring.py` & `skytek-utils-0.5.0/skytek_utils/monitoring.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.4.1/skytek_utils.egg-info/PKG-INFO` & `skytek-utils-0.5.0/skytek_utils.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytek-utils
-Version: 0.4.1
+Version: 0.5.0
 Summary: skytek-utils - a set of small util functions
 Home-page: http://github.com/Skytek/skytek-utils
 Author: Skytek Ltd.
 Author-email: wiktor.latanowicz@skytek.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `skytek-utils-0.4.1/skytek_utils.egg-info/SOURCES.txt` & `skytek-utils-0.5.0/skytek_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.4.1/tests/test_iter.py` & `skytek-utils-0.5.0/tests/test_iter.py`

 * *Files identical despite different names*

