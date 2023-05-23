# Comparing `tmp/revproxy_auth-0.1.1.tar.gz` & `tmp/revproxy_auth-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revproxy_auth-0.1.1.tar", last modified: Mon May 22 06:15:09 2023, max compression
+gzip compressed data, was "revproxy_auth-0.1.3.tar", last modified: Tue May 23 14:55:12 2023, max compression
```

## Comparing `revproxy_auth-0.1.1.tar` & `revproxy_auth-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:09.403558 revproxy_auth-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-22 06:15:09.403558 revproxy_auth-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:09.399557 revproxy_auth-0.1.1/revproxy_auth/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/revproxy_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/revproxy_auth/config-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)    18545 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/revproxy_auth/revproxy_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:09.395557 revproxy_auth-0.1.1/revproxy_auth/revproxy_auth_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:09.399557 revproxy_auth-0.1.1/revproxy_auth/revproxy_auth_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/revproxy_auth/revproxy_auth_static/css/view.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:09.399557 revproxy_auth-0.1.1/revproxy_auth/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/revproxy_auth/templates/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:09.399557 revproxy_auth-0.1.1/revproxy_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-22 06:15:09.000000 revproxy_auth-0.1.1/revproxy_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-22 06:15:09.000000 revproxy_auth-0.1.1/revproxy_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 06:15:09.000000 revproxy_auth-0.1.1/revproxy_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-22 06:15:09.000000 revproxy_auth-0.1.1/revproxy_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 06:15:09.000000 revproxy_auth-0.1.1/revproxy_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 06:15:09.403558 revproxy_auth-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:09.403558 revproxy_auth-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:15:09.403558 revproxy_auth-0.1.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/tests/data/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/tests/test_000.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-22 06:14:59.000000 revproxy_auth-0.1.1/tests/test_001.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:55:12.557099 revproxy_auth-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-23 14:55:12.557099 revproxy_auth-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:55:12.553099 revproxy_auth-0.1.3/revproxy_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/revproxy_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/revproxy_auth/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/revproxy_auth/revproxy_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:55:12.553099 revproxy_auth-0.1.3/revproxy_auth/revproxy_auth_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:55:12.557099 revproxy_auth-0.1.3/revproxy_auth/revproxy_auth_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/revproxy_auth/revproxy_auth_static/css/view.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:55:12.557099 revproxy_auth-0.1.3/revproxy_auth/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/revproxy_auth/templates/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:55:12.557099 revproxy_auth-0.1.3/revproxy_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-23 14:55:12.000000 revproxy_auth-0.1.3/revproxy_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-23 14:55:12.000000 revproxy_auth-0.1.3/revproxy_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:55:12.000000 revproxy_auth-0.1.3/revproxy_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-23 14:55:12.000000 revproxy_auth-0.1.3/revproxy_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 14:55:12.000000 revproxy_auth-0.1.3/revproxy_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:55:12.557099 revproxy_auth-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:55:12.557099 revproxy_auth-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:55:12.557099 revproxy_auth-0.1.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/tests/data/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/tests/test_000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-23 14:55:01.000000 revproxy_auth-0.1.3/tests/test_001.py
```

### Comparing `revproxy_auth-0.1.1/PKG-INFO` & `revproxy_auth-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revproxy_auth
-Version: 0.1.1
+Version: 0.1.3
 Summary: Reverse proxy with synology authentication
 Home-page: https://github.com/Phornee/revproxy_auth
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # revproxy_auth
         This class implements a reverse proxy intended to work inside a Flask server, allows to use the synology auth credentials for all your services behind the synology service proxy.
```

### Comparing `revproxy_auth-0.1.1/README.md` & `revproxy_auth-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.1.1/revproxy_auth/revproxy_auth.py` & `revproxy_auth-0.1.3/revproxy_auth/revproxy_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,16 +244,17 @@
                              headers = headers,
                              timeout=10)
         return Response(resp.text, status=resp.status_code, content_type=resp.headers['content-type'])
 
     def _reask_credentials(self, req: Request, old_cookie_name: str = None) -> Response:
         new_cookie, new_cookie_name = self._build_auth_cookie(req)
         if not new_cookie: # Unable to build cookie for requested path: host unknown
-            return Response(req.host, status=HTTP_501_NOT_IMPLEMENTED, content_type='text/plain')
-            # return ApiRestResponse(request_dict['host'], status=501)
+            return Response(f'Host {req.host} not found on revproxy_auth config translation table',
+                            status=HTTP_501_NOT_IMPLEMENTED, 
+                            content_type='text/plain')
         print(f'Creating new auth cookie {new_cookie_name} and reasking to user...')
         self._write_cookie(new_cookie, self.auth_cookie_folder, new_cookie_name)
         response = self._build_auth_popup(new_cookie_name)
         if old_cookie_name:
             print(f'Deleting cookie in response: {old_cookie_name}')
             self._clear_local_cookie(self.auth_cookie_folder, old_cookie_name)
         return response
```

### Comparing `revproxy_auth-0.1.1/revproxy_auth/revproxy_auth_static/css/view.css` & `revproxy_auth-0.1.3/revproxy_auth/revproxy_auth_static/css/view.css`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.1.1/revproxy_auth/templates/form.html` & `revproxy_auth-0.1.3/revproxy_auth/templates/form.html`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.1.1/revproxy_auth.egg-info/PKG-INFO` & `revproxy_auth-0.1.3/revproxy_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revproxy-auth
-Version: 0.1.1
+Version: 0.1.3
 Summary: Reverse proxy with synology authentication
 Home-page: https://github.com/Phornee/revproxy_auth
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # revproxy_auth
         This class implements a reverse proxy intended to work inside a Flask server, allows to use the synology auth credentials for all your services behind the synology service proxy.
```

### Comparing `revproxy_auth-0.1.1/tests/test_000.py` & `revproxy_auth-0.1.3/tests/test_000.py`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.1.1/tests/test_001.py` & `revproxy_auth-0.1.3/tests/test_001.py`

 * *Files identical despite different names*

