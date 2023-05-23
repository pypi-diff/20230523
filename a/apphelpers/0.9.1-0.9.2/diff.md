# Comparing `tmp/apphelpers-0.9.1.tar.gz` & `tmp/apphelpers-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apphelpers-0.9.1.tar", last modified: Mon May 20 05:30:59 2019, max compression
+gzip compressed data, was "dist/apphelpers-0.9.2.tar", last modified: Mon May 20 09:21:48 2019, max compression
```

## Comparing `apphelpers-0.9.1.tar` & `apphelpers-0.9.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 shon      (1000) shon      (1000)        0 2019-05-20 05:30:59.000000 apphelpers-0.9.1/
--rw-r--r--   0 shon      (1000) shon      (1000)      151 2019-03-25 09:15:25.000000 apphelpers-0.9.1/AUTHORS.rst
--rw-r--r--   0 shon      (1000) shon      (1000)     3624 2019-03-25 09:15:25.000000 apphelpers-0.9.1/CONTRIBUTING.rst
--rw-r--r--   0 shon      (1000) shon      (1000)       89 2019-03-25 09:15:25.000000 apphelpers-0.9.1/HISTORY.rst
--rw-r--r--   0 shon      (1000) shon      (1000)     1070 2019-03-25 09:15:25.000000 apphelpers-0.9.1/LICENSE
--rw-r--r--   0 shon      (1000) shon      (1000)      262 2019-03-25 09:15:25.000000 apphelpers-0.9.1/MANIFEST.in
--rw-r--r--   0 shon      (1000) shon      (1000)     2195 2019-05-20 05:30:59.000000 apphelpers-0.9.1/PKG-INFO
--rw-r--r--   0 shon      (1000) shon      (1000)     1135 2019-03-25 09:15:25.000000 apphelpers-0.9.1/README.rst
-drwxr-xr-x   0 shon      (1000) shon      (1000)        0 2019-05-20 05:30:59.000000 apphelpers-0.9.1/apphelpers/
--rw-r--r--   0 shon      (1000) shon      (1000)      177 2019-05-20 05:30:40.000000 apphelpers-0.9.1/apphelpers/__init__.py
--rw-r--r--   0 shon      (1000) shon      (1000)      157 2019-04-16 06:39:29.000000 apphelpers-0.9.1/apphelpers/context.py
-drwxr-xr-x   0 shon      (1000) shon      (1000)        0 2019-05-20 05:30:59.000000 apphelpers-0.9.1/apphelpers/db/
--rw-r--r--   0 shon      (1000) shon      (1000)        0 2019-04-02 10:55:29.000000 apphelpers-0.9.1/apphelpers/db/__init__.py
--rw-r--r--   0 shon      (1000) shon      (1000)     2874 2019-04-05 10:35:55.000000 apphelpers-0.9.1/apphelpers/db/peewee.py
--rw-r--r--   0 shon      (1000) shon      (1000)      667 2019-04-16 06:39:29.000000 apphelpers-0.9.1/apphelpers/errors.py
-drwxr-xr-x   0 shon      (1000) shon      (1000)        0 2019-05-20 05:30:59.000000 apphelpers-0.9.1/apphelpers/rest/
--rw-r--r--   0 shon      (1000) shon      (1000)        0 2019-03-30 04:39:03.000000 apphelpers-0.9.1/apphelpers/rest/__init__.py
--rw-r--r--   0 shon      (1000) shon      (1000)       94 2019-03-29 05:37:16.000000 apphelpers-0.9.1/apphelpers/rest/fastapi.py
--rw-r--r--   0 shon      (1000) shon      (1000)     8305 2019-04-02 08:36:36.000000 apphelpers-0.9.1/apphelpers/rest/flask.py
--rw-r--r--   0 shon      (1000) shon      (1000)     3023 2019-04-02 08:34:51.000000 apphelpers-0.9.1/apphelpers/rest/flaskutils.py
--rw-r--r--   0 shon      (1000) shon      (1000)     6146 2019-05-20 05:29:39.000000 apphelpers-0.9.1/apphelpers/rest/hug.py
--rw-r--r--   0 shon      (1000) shon      (1000)      261 2019-03-30 04:49:03.000000 apphelpers-0.9.1/apphelpers/rest/starlette.py
--rw-r--r--   0 shon      (1000) shon      (1000)     3488 2019-04-25 10:17:08.000000 apphelpers-0.9.1/apphelpers/sessions.py
-drwxr-xr-x   0 shon      (1000) shon      (1000)        0 2019-05-20 05:30:59.000000 apphelpers-0.9.1/apphelpers.egg-info/
--rw-r--r--   0 shon      (1000) shon      (1000)     2195 2019-05-20 05:30:59.000000 apphelpers-0.9.1/apphelpers.egg-info/PKG-INFO
--rw-r--r--   0 shon      (1000) shon      (1000)      886 2019-05-20 05:30:59.000000 apphelpers-0.9.1/apphelpers.egg-info/SOURCES.txt
--rw-r--r--   0 shon      (1000) shon      (1000)        1 2019-05-20 05:30:59.000000 apphelpers-0.9.1/apphelpers.egg-info/dependency_links.txt
--rw-r--r--   0 shon      (1000) shon      (1000)        1 2019-05-20 05:30:59.000000 apphelpers-0.9.1/apphelpers.egg-info/not-zip-safe
--rw-r--r--   0 shon      (1000) shon      (1000)       17 2019-05-20 05:30:59.000000 apphelpers-0.9.1/apphelpers.egg-info/top_level.txt
-drwxr-xr-x   0 shon      (1000) shon      (1000)        0 2019-05-20 05:30:59.000000 apphelpers-0.9.1/docs/
--rw-r--r--   0 shon      (1000) shon      (1000)      611 2019-03-25 09:15:25.000000 apphelpers-0.9.1/docs/Makefile
--rw-r--r--   0 shon      (1000) shon      (1000)       28 2019-03-25 09:15:25.000000 apphelpers-0.9.1/docs/authors.rst
--rwxr-xr-x   0 shon      (1000) shon      (1000)     4961 2019-03-25 09:15:25.000000 apphelpers-0.9.1/docs/conf.py
--rw-r--r--   0 shon      (1000) shon      (1000)       33 2019-03-25 09:15:25.000000 apphelpers-0.9.1/docs/contributing.rst
--rw-r--r--   0 shon      (1000) shon      (1000)       28 2019-03-25 09:15:25.000000 apphelpers-0.9.1/docs/history.rst
--rw-r--r--   0 shon      (1000) shon      (1000)      336 2019-03-25 09:15:25.000000 apphelpers-0.9.1/docs/index.rst
--rw-r--r--   0 shon      (1000) shon      (1000)     1233 2019-03-25 09:15:25.000000 apphelpers-0.9.1/docs/installation.rst
--rw-r--r--   0 shon      (1000) shon      (1000)      772 2019-03-25 09:15:25.000000 apphelpers-0.9.1/docs/make.bat
--rw-r--r--   0 shon      (1000) shon      (1000)       27 2019-03-25 09:15:25.000000 apphelpers-0.9.1/docs/readme.rst
--rw-r--r--   0 shon      (1000) shon      (1000)      104 2019-03-25 09:15:25.000000 apphelpers-0.9.1/docs/usage.rst
--rw-r--r--   0 shon      (1000) shon      (1000)      393 2019-05-20 05:30:59.000000 apphelpers-0.9.1/setup.cfg
--rw-r--r--   0 shon      (1000) shon      (1000)     1200 2019-05-20 05:30:40.000000 apphelpers-0.9.1/setup.py
-drwxr-xr-x   0 shon      (1000) shon      (1000)        0 2019-05-20 05:30:59.000000 apphelpers-0.9.1/tests/
--rw-r--r--   0 shon      (1000) shon      (1000)       65 2019-03-25 09:15:25.000000 apphelpers-0.9.1/tests/__init__.py
-drwxr-xr-x   0 shon      (1000) shon      (1000)        0 2019-05-20 05:30:59.000000 apphelpers-0.9.1/tests/app/
--rw-r--r--   0 shon      (1000) shon      (1000)        0 2019-04-16 17:03:14.000000 apphelpers-0.9.1/tests/app/__init__.py
--rw-r--r--   0 shon      (1000) shon      (1000)     1059 2019-05-19 16:55:10.000000 apphelpers-0.9.1/tests/app/endpoints.py
-drwxr-xr-x   0 shon      (1000) shon      (1000)        0 2019-05-20 05:30:59.000000 apphelpers-0.9.1/tests/run/
--rw-r--r--   0 shon      (1000) shon      (1000)        5 2019-04-20 06:26:26.000000 apphelpers-0.9.1/tests/run/app.pid
--rw-r--r--   0 shon      (1000) shon      (1000)      586 2019-05-07 19:09:36.000000 apphelpers-0.9.1/tests/service.py
--rw-r--r--   0 shon      (1000) shon      (1000)     1124 2019-04-16 17:03:14.000000 apphelpers-0.9.1/tests/test_peewee.py
--rw-r--r--   0 shon      (1000) shon      (1000)     3280 2019-05-19 17:02:00.000000 apphelpers-0.9.1/tests/test_rest.py
--rw-r--r--   0 shon      (1000) shon      (1000)     1787 2019-04-21 17:28:09.000000 apphelpers-0.9.1/tests/test_sessions.py
+drwxr-xr-x   0 shon      (1000) shon      (1000)        0 2019-05-20 09:21:48.000000 apphelpers-0.9.2/
+-rw-r--r--   0 shon      (1000) shon      (1000)      151 2019-03-25 09:15:25.000000 apphelpers-0.9.2/AUTHORS.rst
+-rw-r--r--   0 shon      (1000) shon      (1000)     3624 2019-03-25 09:15:25.000000 apphelpers-0.9.2/CONTRIBUTING.rst
+-rw-r--r--   0 shon      (1000) shon      (1000)      205 2019-05-20 09:18:50.000000 apphelpers-0.9.2/HISTORY.rst
+-rw-r--r--   0 shon      (1000) shon      (1000)     1070 2019-03-25 09:15:25.000000 apphelpers-0.9.2/LICENSE
+-rw-r--r--   0 shon      (1000) shon      (1000)      262 2019-03-25 09:15:25.000000 apphelpers-0.9.2/MANIFEST.in
+-rw-r--r--   0 shon      (1000) shon      (1000)     2351 2019-05-20 09:21:48.000000 apphelpers-0.9.2/PKG-INFO
+-rw-r--r--   0 shon      (1000) shon      (1000)     1135 2019-03-25 09:15:25.000000 apphelpers-0.9.2/README.rst
+drwxr-xr-x   0 shon      (1000) shon      (1000)        0 2019-05-20 09:21:48.000000 apphelpers-0.9.2/apphelpers/
+-rw-r--r--   0 shon      (1000) shon      (1000)      177 2019-05-20 09:21:35.000000 apphelpers-0.9.2/apphelpers/__init__.py
+-rw-r--r--   0 shon      (1000) shon      (1000)      157 2019-04-16 06:39:29.000000 apphelpers-0.9.2/apphelpers/context.py
+drwxr-xr-x   0 shon      (1000) shon      (1000)        0 2019-05-20 09:21:48.000000 apphelpers-0.9.2/apphelpers/db/
+-rw-r--r--   0 shon      (1000) shon      (1000)        0 2019-04-02 10:55:29.000000 apphelpers-0.9.2/apphelpers/db/__init__.py
+-rw-r--r--   0 shon      (1000) shon      (1000)     2874 2019-04-05 10:35:55.000000 apphelpers-0.9.2/apphelpers/db/peewee.py
+-rw-r--r--   0 shon      (1000) shon      (1000)      667 2019-04-16 06:39:29.000000 apphelpers-0.9.2/apphelpers/errors.py
+drwxr-xr-x   0 shon      (1000) shon      (1000)        0 2019-05-20 09:21:48.000000 apphelpers-0.9.2/apphelpers/rest/
+-rw-r--r--   0 shon      (1000) shon      (1000)        0 2019-03-30 04:39:03.000000 apphelpers-0.9.2/apphelpers/rest/__init__.py
+-rw-r--r--   0 shon      (1000) shon      (1000)       94 2019-03-29 05:37:16.000000 apphelpers-0.9.2/apphelpers/rest/fastapi.py
+-rw-r--r--   0 shon      (1000) shon      (1000)     8305 2019-04-02 08:36:36.000000 apphelpers-0.9.2/apphelpers/rest/flask.py
+-rw-r--r--   0 shon      (1000) shon      (1000)     3023 2019-04-02 08:34:51.000000 apphelpers-0.9.2/apphelpers/rest/flaskutils.py
+-rw-r--r--   0 shon      (1000) shon      (1000)     6156 2019-05-20 09:04:39.000000 apphelpers-0.9.2/apphelpers/rest/hug.py
+-rw-r--r--   0 shon      (1000) shon      (1000)      261 2019-03-30 04:49:03.000000 apphelpers-0.9.2/apphelpers/rest/starlette.py
+-rw-r--r--   0 shon      (1000) shon      (1000)     3488 2019-04-25 10:17:08.000000 apphelpers-0.9.2/apphelpers/sessions.py
+drwxr-xr-x   0 shon      (1000) shon      (1000)        0 2019-05-20 09:21:48.000000 apphelpers-0.9.2/apphelpers.egg-info/
+-rw-r--r--   0 shon      (1000) shon      (1000)     2351 2019-05-20 09:21:47.000000 apphelpers-0.9.2/apphelpers.egg-info/PKG-INFO
+-rw-r--r--   0 shon      (1000) shon      (1000)      886 2019-05-20 09:21:48.000000 apphelpers-0.9.2/apphelpers.egg-info/SOURCES.txt
+-rw-r--r--   0 shon      (1000) shon      (1000)        1 2019-05-20 09:21:47.000000 apphelpers-0.9.2/apphelpers.egg-info/dependency_links.txt
+-rw-r--r--   0 shon      (1000) shon      (1000)        1 2019-05-20 09:21:47.000000 apphelpers-0.9.2/apphelpers.egg-info/not-zip-safe
+-rw-r--r--   0 shon      (1000) shon      (1000)       17 2019-05-20 09:21:47.000000 apphelpers-0.9.2/apphelpers.egg-info/top_level.txt
+drwxr-xr-x   0 shon      (1000) shon      (1000)        0 2019-05-20 09:21:48.000000 apphelpers-0.9.2/docs/
+-rw-r--r--   0 shon      (1000) shon      (1000)      611 2019-03-25 09:15:25.000000 apphelpers-0.9.2/docs/Makefile
+-rw-r--r--   0 shon      (1000) shon      (1000)       28 2019-03-25 09:15:25.000000 apphelpers-0.9.2/docs/authors.rst
+-rwxr-xr-x   0 shon      (1000) shon      (1000)     4961 2019-03-25 09:15:25.000000 apphelpers-0.9.2/docs/conf.py
+-rw-r--r--   0 shon      (1000) shon      (1000)       33 2019-03-25 09:15:25.000000 apphelpers-0.9.2/docs/contributing.rst
+-rw-r--r--   0 shon      (1000) shon      (1000)       28 2019-03-25 09:15:25.000000 apphelpers-0.9.2/docs/history.rst
+-rw-r--r--   0 shon      (1000) shon      (1000)      336 2019-03-25 09:15:25.000000 apphelpers-0.9.2/docs/index.rst
+-rw-r--r--   0 shon      (1000) shon      (1000)     1233 2019-03-25 09:15:25.000000 apphelpers-0.9.2/docs/installation.rst
+-rw-r--r--   0 shon      (1000) shon      (1000)      772 2019-03-25 09:15:25.000000 apphelpers-0.9.2/docs/make.bat
+-rw-r--r--   0 shon      (1000) shon      (1000)       27 2019-03-25 09:15:25.000000 apphelpers-0.9.2/docs/readme.rst
+-rw-r--r--   0 shon      (1000) shon      (1000)      104 2019-03-25 09:15:25.000000 apphelpers-0.9.2/docs/usage.rst
+-rw-r--r--   0 shon      (1000) shon      (1000)      393 2019-05-20 09:21:48.000000 apphelpers-0.9.2/setup.cfg
+-rw-r--r--   0 shon      (1000) shon      (1000)     1200 2019-05-20 09:21:35.000000 apphelpers-0.9.2/setup.py
+drwxr-xr-x   0 shon      (1000) shon      (1000)        0 2019-05-20 09:21:48.000000 apphelpers-0.9.2/tests/
+-rw-r--r--   0 shon      (1000) shon      (1000)       65 2019-03-25 09:15:25.000000 apphelpers-0.9.2/tests/__init__.py
+drwxr-xr-x   0 shon      (1000) shon      (1000)        0 2019-05-20 09:21:48.000000 apphelpers-0.9.2/tests/app/
+-rw-r--r--   0 shon      (1000) shon      (1000)        0 2019-04-16 17:03:14.000000 apphelpers-0.9.2/tests/app/__init__.py
+-rw-r--r--   0 shon      (1000) shon      (1000)     1059 2019-05-19 16:55:10.000000 apphelpers-0.9.2/tests/app/endpoints.py
+drwxr-xr-x   0 shon      (1000) shon      (1000)        0 2019-05-20 09:21:48.000000 apphelpers-0.9.2/tests/run/
+-rw-r--r--   0 shon      (1000) shon      (1000)        5 2019-04-20 06:26:26.000000 apphelpers-0.9.2/tests/run/app.pid
+-rw-r--r--   0 shon      (1000) shon      (1000)      586 2019-05-07 19:09:36.000000 apphelpers-0.9.2/tests/service.py
+-rw-r--r--   0 shon      (1000) shon      (1000)     1124 2019-04-16 17:03:14.000000 apphelpers-0.9.2/tests/test_peewee.py
+-rw-r--r--   0 shon      (1000) shon      (1000)     3280 2019-05-19 17:02:00.000000 apphelpers-0.9.2/tests/test_rest.py
+-rw-r--r--   0 shon      (1000) shon      (1000)     1787 2019-04-21 17:28:09.000000 apphelpers-0.9.2/tests/test_sessions.py
```

### Comparing `apphelpers-0.9.1/CONTRIBUTING.rst` & `apphelpers-0.9.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `apphelpers-0.9.1/LICENSE` & `apphelpers-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apphelpers-0.9.1/PKG-INFO` & `apphelpers-0.9.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: apphelpers
-Version: 0.9.1
+Version: 0.9.2
 Summary: Common helper libraries for Python Apps
 Home-page: https://github.com/scrolltech/apphelpers
 Author: Scroll Tech
 Author-email: tech@scroll.in
 License: MIT license
 Description: =======================================
         Common helper libraries for Python Apps
@@ -49,14 +49,19 @@
         .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
         
         
         =======
         History
         =======
         
+        0.9.2 (2019-05-20)
+        ------------------
+        
+        * New options `groups_forbidden` and `groups_required` to secure API access
+        
         0.1.0 (2019-03-24)
         ------------------
         
         * First release on PyPI.
         
 Keywords: apphelpers
 Platform: UNKNOWN
```

### Comparing `apphelpers-0.9.1/README.rst` & `apphelpers-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `apphelpers-0.9.1/apphelpers/db/peewee.py` & `apphelpers-0.9.2/apphelpers/db/peewee.py`

 * *Files identical despite different names*

### Comparing `apphelpers-0.9.1/apphelpers/errors.py` & `apphelpers-0.9.2/apphelpers/errors.py`

 * *Files identical despite different names*

### Comparing `apphelpers-0.9.1/apphelpers/rest/flask.py` & `apphelpers-0.9.2/apphelpers/rest/flask.py`

 * *Files identical despite different names*

### Comparing `apphelpers-0.9.1/apphelpers/rest/flaskutils.py` & `apphelpers-0.9.2/apphelpers/rest/flaskutils.py`

 * *Files identical despite different names*

### Comparing `apphelpers-0.9.1/apphelpers/rest/hug.py` & `apphelpers-0.9.2/apphelpers/rest/hug.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,35 +100,35 @@
         self.secure_router = self.router.http(requires=hug.authentication.token(set_context))
 
         def access_wrapper(f):
             """
             This is the authentication + authorization part
             """
             login_required = getattr(f, 'login_required', None)
-            roles_required = getattr(f, 'roles_required', None)
-            roles_forbidden = getattr(f, 'roles_forbidden', None)
+            groups_required = getattr(f, 'groups_required', None)
+            groups_forbidden = getattr(f, 'groups_forbidden', None)
 
-            if login_required or roles_required or roles_forbidden:
+            if login_required or groups_required or groups_forbidden:
 
                 @wraps(f)
                 def wrapper(request, *args, **kw):
 
                     user = request.context['user']
 
                     # this is authentication part
                     if not user.id:
                         raise HTTPUnauthorized('Invalid or expired session')
 
                     # this is authorization part
                     groups = set(user.groups)
 
-                    if roles_required and not groups.intersection(roles_required):
+                    if groups_required and not groups.intersection(groups_required):
                         raise HTTPForbidden('Unauthorized access')
 
-                    if roles_forbidden and groups.intersection(roles_forbidden):
+                    if groups_forbidden and groups.intersection(groups_forbidden):
                         raise HTTPForbidden('Unauthorized access')
 
                     return f(*args, **kw)
             else:
 
                 wrapper = f
```

### Comparing `apphelpers-0.9.1/apphelpers/sessions.py` & `apphelpers-0.9.2/apphelpers/sessions.py`

 * *Files identical despite different names*

### Comparing `apphelpers-0.9.1/apphelpers.egg-info/PKG-INFO` & `apphelpers-0.9.2/apphelpers.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: apphelpers
-Version: 0.9.1
+Version: 0.9.2
 Summary: Common helper libraries for Python Apps
 Home-page: https://github.com/scrolltech/apphelpers
 Author: Scroll Tech
 Author-email: tech@scroll.in
 License: MIT license
 Description: =======================================
         Common helper libraries for Python Apps
@@ -49,14 +49,19 @@
         .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
         
         
         =======
         History
         =======
         
+        0.9.2 (2019-05-20)
+        ------------------
+        
+        * New options `groups_forbidden` and `groups_required` to secure API access
+        
         0.1.0 (2019-03-24)
         ------------------
         
         * First release on PyPI.
         
 Keywords: apphelpers
 Platform: UNKNOWN
```

### Comparing `apphelpers-0.9.1/apphelpers.egg-info/SOURCES.txt` & `apphelpers-0.9.2/apphelpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apphelpers-0.9.1/docs/Makefile` & `apphelpers-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `apphelpers-0.9.1/docs/conf.py` & `apphelpers-0.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `apphelpers-0.9.1/docs/installation.rst` & `apphelpers-0.9.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `apphelpers-0.9.1/docs/make.bat` & `apphelpers-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `apphelpers-0.9.1/setup.py` & `apphelpers-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,10 +36,10 @@
     keywords='apphelpers',
     name='apphelpers',
     packages=find_packages(exclude=['tests']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/scrolltech/apphelpers',
-    version='0.9.1',
+    version='0.9.2',
     zip_safe=False,
 )
```

### Comparing `apphelpers-0.9.1/tests/app/endpoints.py` & `apphelpers-0.9.2/tests/app/endpoints.py`

 * *Files identical despite different names*

### Comparing `apphelpers-0.9.1/tests/service.py` & `apphelpers-0.9.2/tests/service.py`

 * *Files identical despite different names*

### Comparing `apphelpers-0.9.1/tests/test_peewee.py` & `apphelpers-0.9.2/tests/test_peewee.py`

 * *Files identical despite different names*

### Comparing `apphelpers-0.9.1/tests/test_rest.py` & `apphelpers-0.9.2/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `apphelpers-0.9.1/tests/test_sessions.py` & `apphelpers-0.9.2/tests/test_sessions.py`

 * *Files identical despite different names*

