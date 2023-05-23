# Comparing `tmp/toui-2.4.0.tar.gz` & `tmp/toui-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toui-2.4.0.tar", last modified: Mon May 22 17:36:06 2023, max compression
+gzip compressed data, was "toui-2.4.1.tar", last modified: Tue May 23 17:58:46 2023, max compression
```

## Comparing `toui-2.4.0.tar` & `toui-2.4.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 17:36:06.858692 toui-2.4.0/
--rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-2.4.0/LICENSE
--rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-2.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2994 2023-05-22 17:36:06.857692 toui-2.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2621 2023-05-15 13:27:02.000000 toui-2.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 17:36:06.709721 toui-2.4.0/examples/
--rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-2.4.0/examples/__init__.py
--rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-2.4.0/examples/advanced_example_1_toui_blueprint.py
--rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-2.4.0/examples/example_1_simple_website.py
--rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-2.4.0/examples/example_2_simple_desktop_app.py
--rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-2.4.0/examples/example_3_updating_page.py
--rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-2.4.0/examples/example_4_function_with_arg.py
--rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-2.4.0/examples/example_5_user_variables.py
--rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-2.4.0/examples/example_6_quick_website.py
--rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-2.4.0/examples/example_7_quick_desktop_app.py
-drwxrwxrwx   0        0        0        0 2023-05-22 17:36:06.713919 toui-2.4.0/images/
--rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-2.4.0/images/logo.png
--rw-rw-rw-   0        0        0       42 2023-05-22 17:36:06.859692 toui-2.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1635 2023-05-21 08:35:49.000000 toui-2.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 17:36:06.846500 toui-2.4.0/toui/
--rw-rw-rw-   0        0        0      266 2023-05-22 16:15:34.000000 toui-2.4.0/toui/__init__.py
--rw-rw-rw-   0        0        0      431 2023-05-04 15:56:54.000000 toui-2.4.0/toui/_defaults.py
--rw-rw-rw-   0        0        0     1272 2023-05-15 13:04:45.000000 toui-2.4.0/toui/_helpers.py
--rw-rw-rw-   0        0        0    10611 2023-05-22 17:16:43.000000 toui-2.4.0/toui/_javascript_templates.py
--rw-rw-rw-   0        0        0     6450 2023-05-15 13:04:45.000000 toui-2.4.0/toui/_signals.py
--rw-rw-rw-   0        0        0    29077 2023-05-22 16:49:37.000000 toui-2.4.0/toui/apps.py
--rw-rw-rw-   0        0        0    23003 2023-05-22 17:25:05.000000 toui-2.4.0/toui/elements.py
--rw-rw-rw-   0        0        0      316 2023-05-15 13:04:45.000000 toui-2.4.0/toui/exceptions.py
--rw-rw-rw-   0        0        0    18042 2023-05-22 17:32:38.000000 toui-2.4.0/toui/pages.py
--rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-2.4.0/toui/structure.py
-drwxrwxrwx   0        0        0        0 2023-05-22 17:36:06.856697 toui-2.4.0/toui.egg-info/
--rw-rw-rw-   0        0        0     2994 2023-05-22 17:36:06.000000 toui-2.4.0/toui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2023-05-22 17:36:06.000000 toui-2.4.0/toui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 17:36:06.000000 toui-2.4.0/toui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      196 2023-05-22 17:36:06.000000 toui-2.4.0/toui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-22 17:36:06.000000 toui-2.4.0/toui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 17:58:46.531751 toui-2.4.1/
+-rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-2.4.1/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-2.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2994 2023-05-23 17:58:46.531751 toui-2.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2621 2023-05-15 13:27:02.000000 toui-2.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 17:58:46.464317 toui-2.4.1/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-2.4.1/examples/__init__.py
+-rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-2.4.1/examples/advanced_example_1_toui_blueprint.py
+-rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-2.4.1/examples/example_1_simple_website.py
+-rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-2.4.1/examples/example_2_simple_desktop_app.py
+-rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-2.4.1/examples/example_3_updating_page.py
+-rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-2.4.1/examples/example_4_function_with_arg.py
+-rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-2.4.1/examples/example_5_user_variables.py
+-rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-2.4.1/examples/example_6_quick_website.py
+-rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-2.4.1/examples/example_7_quick_desktop_app.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:58:46.472786 toui-2.4.1/images/
+-rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-2.4.1/images/logo.png
+-rw-rw-rw-   0        0        0       42 2023-05-23 17:58:46.531751 toui-2.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1657 2023-05-23 17:57:05.000000 toui-2.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:58:46.514953 toui-2.4.1/toui/
+-rw-rw-rw-   0        0        0      266 2023-05-23 16:57:01.000000 toui-2.4.1/toui/__init__.py
+-rw-rw-rw-   0        0        0      431 2023-05-23 15:00:55.000000 toui-2.4.1/toui/_defaults.py
+-rw-rw-rw-   0        0        0     1272 2023-05-15 13:04:45.000000 toui-2.4.1/toui/_helpers.py
+-rw-rw-rw-   0        0        0    10611 2023-05-23 15:20:04.000000 toui-2.4.1/toui/_javascript_templates.py
+-rw-rw-rw-   0        0        0     6452 2023-05-23 15:20:31.000000 toui-2.4.1/toui/_signals.py
+-rw-rw-rw-   0        0        0    30744 2023-05-23 16:55:16.000000 toui-2.4.1/toui/apps.py
+-rw-rw-rw-   0        0        0    22886 2023-05-23 15:17:02.000000 toui-2.4.1/toui/elements.py
+-rw-rw-rw-   0        0        0      316 2023-05-15 13:04:45.000000 toui-2.4.1/toui/exceptions.py
+-rw-rw-rw-   0        0        0    18047 2023-05-23 16:30:18.000000 toui-2.4.1/toui/pages.py
+-rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-2.4.1/toui/structure.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:58:46.531751 toui-2.4.1/toui.egg-info/
+-rw-rw-rw-   0        0        0     2994 2023-05-23 17:58:46.000000 toui-2.4.1/toui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2023-05-23 17:58:46.000000 toui-2.4.1/toui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 17:58:46.000000 toui-2.4.1/toui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      220 2023-05-23 17:58:46.000000 toui-2.4.1/toui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-23 17:58:46.000000 toui-2.4.1/toui.egg-info/top_level.txt
```

### Comparing `toui-2.4.0/LICENSE` & `toui-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `toui-2.4.0/PKG-INFO` & `toui-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 2.4.0
+Version: 2.4.1
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `toui-2.4.0/README.md` & `toui-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `toui-2.4.0/examples/advanced_example_1_toui_blueprint.py` & `toui-2.4.1/examples/advanced_example_1_toui_blueprint.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.0/examples/example_1_simple_website.py` & `toui-2.4.1/examples/example_1_simple_website.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.0/examples/example_2_simple_desktop_app.py` & `toui-2.4.1/examples/example_2_simple_desktop_app.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.0/examples/example_3_updating_page.py` & `toui-2.4.1/examples/example_3_updating_page.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.0/examples/example_4_function_with_arg.py` & `toui-2.4.1/examples/example_4_function_with_arg.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.0/examples/example_5_user_variables.py` & `toui-2.4.1/examples/example_5_user_variables.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.0/images/logo.png` & `toui-2.4.1/images/logo.png`

 * *Files identical despite different names*

### Comparing `toui-2.4.0/setup.py` & `toui-2.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 requirements = []
 optional_requirements = ['flask-login', 'flask-sqlalchemy', 'flask-basicauth']
 
 reqs_txt = \
 """beautifulsoup4==4.12.2
 Flask==2.2.5
 Flask_BasicAuth==0.2.0
+Flask_Session==0.4.1
 Flask_Caching==2.0.2
 Flask_Login==0.6.2
 flask_sock==0.6.0
 flask_sqlalchemy==3.0.3
 pywebview==4.1
 tinycss==0.4"""
```

### Comparing `toui-2.4.0/toui/_helpers.py` & `toui-2.4.1/toui/_helpers.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.0/toui/_javascript_templates.py` & `toui-2.4.1/toui/_javascript_templates.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.0/toui/_signals.py` & `toui-2.4.1/toui/_signals.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,17 @@
             if func.__name__ in decorator.no_return_functions:
                 return
             if decorator.return_type == "js":
                 return real_output
             return value
         return new_func
 
-    def _call_method(self, func, **kwargs):
+    def _call_method(self, func_, **kwargs):
         for method_name, method in inspect.getmembers(self, inspect.isfunction):
-            if method_name == func.__name__ and (not method_name.startswith("_") or
+            if method_name == func_.__name__ and (not method_name.startswith("_") or
                                                  method_name in self.included_private_methods):
                 signal = method(**kwargs)
                 if signal:
                     return self._send(signal)
                 else:
                     return
```

### Comparing `toui-2.4.0/toui/apps.py` & `toui-2.4.1/toui/apps.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from abc import ABCMeta, abstractmethod
 from collections.abc import MutableMapping
 from functools import wraps
 from typing import Any
 from flask import Flask, session, request, send_file
 from flask_sock import Sock
 from flask_caching import Cache
+from flask_session import Session
 import webview
 from toui._helpers import warn, info, debug, error
 from toui.pages import Page
 from toui.exceptions import ToUIWrongPlaceException, ToUINotAddedError
 from toui._defaults import validate_ws, validate_data
 
 _imported_optional_reqs = {'flask-login':False,
@@ -88,26 +89,33 @@
             A dictionary that stores temporary data unique to each user. The data are stored in a `Cache` object from `flask-caching`
             package.
 
         pages: list
             A list of added `Page` objects.
 
 
+        Warning
+        -------
+        A folder called 'flask_session' will be created in the main directory when calling this class.
+
+
         .. admonition:: Behind The Scenes
             :class: tip
             
             ToUI uses `Flask` and its extenstions to create apps. When creating an instance of this class, the following
             extensions are used:
 
+            - `Session` class extension from `Flask-Session` package.
             - `Sock` class extension from `Flask-Sock` package.
-            - `Cache` class extension from `Flask-Cache` package.
+            - `Cache` class extension from `Flask-Caching` package.
 
             The following `Flask` configurations are also set:
 
             - `CACHE_TYPE = "SimpleCache"`
+            - `SESSION_TYPE = "filesystem"`
 
         """
         self._functions = {}
         if not name:
             if hasattr(__main__, "__file__"):
                 name = os.path.basename(__main__.__file__).split(".")[0]
             else:
@@ -119,14 +127,16 @@
             self.flask_app.secret_key = secret_key
         elif os.environ.get('SECRET_KEY') is not None:
             self.flask_app.secret_key = os.environ.get('SECRET_KEY')
         else:
             warn("No secret key was set. Generating a random secret key for Flask.")
             self.flask_app.secret_key = os.urandom(50)
         self.pages = []
+        self.flask_app.config['SESSION_TYPE'] = "filesystem"
+        Session(self.flask_app)
         self._add_communication_method()
         self._add_user_vars()
         self.flask_app.route("/toui-download-<path_id>", methods=['POST', 'GET'])(self._download)
         self.forbidden_urls = ['/toui-communicate', "/toui-download-<path_id>"]
         self._validate_ws = validate_ws
         self._validate_data = validate_data
         self._auth = None
@@ -231,17 +241,17 @@
             The path to the file (on the server).
 
         new: bool, default=True
             Opens new tab/window when downloading file.
 
         """
         path_id = 0
-        while self._cache.get(f'toui-download-{path_id}'):
+        while self._user_vars._get(f'toui-download-{path_id}'):
             path_id += 1
-        self._cache.set(f'toui-download-{path_id}', filepath)
+        self._user_vars._set(f'toui-download-{path_id}', filepath)
         self.open_new_page(f"/toui-download-{path_id}", new=new)
 
     @_ReqsChecker(['flask-sqlalchemy', 'flask-login'])
     def add_user_database(self, database_uri, other_columns=[], user_cls=None):
         """
         Creates a simple database that has data specific to each user.
 
@@ -396,15 +406,15 @@
             ``True`` if the user is signed in, and ``False`` if it is not signed in.
 
         """
         self._confirm_user_database_created()
         user = self._user_cls.query.filter_by(username=username, password=password, **other_info).first()
         if user:
             login_user(user)
-            self._cache.set("user-id", user.id)
+            self._user_vars._set("user-id", user.id)
             return True
         else:
             return False
         
     @_ReqsChecker(['flask-sqlalchemy', 'flask-login'])
     def signin_user_from_id(self, user_id, **other_info):
         """
@@ -423,26 +433,26 @@
             ``True`` if the user is signed in, and ``False`` if it is not signed in.
 
         """
         self._confirm_user_database_created()
         user = self._user_cls.query.filter_by(id=user_id, **other_info).first()
         if user:
             login_user(user)
-            self._cache.set("user-id", user_id)
+            self._user_vars._set("user-id", user_id)
             return True
         else:
             return False
 
     @_ReqsChecker(['flask-login'])
     def signout_user(self):
         """
         A method that signs out the current user.
         """
         logout_user()
-        self._cache.set('user-id', None)
+        self._user_vars._del('user-id')
 
     @_ReqsChecker(['flask-sqlalchemy'])
     def username_exists(self, username):
         """
         Checks if the username is exists in the database.
         
         Parameters
@@ -588,22 +598,22 @@
         try:
             session.keys()
         except RuntimeError as e:
             return False
         if not "user page" in session.keys():
             session['user page'] = None
         if not "_user_id" in session.keys():
-            user_id = self._cache.get('user-id')
+            user_id = self._user_vars._get('user-id')
             if user_id:
                 session['_user_id'] = user_id
         return True
     
     def _download(self, path_id):
         debug(f"PATH: {path_id}")
-        file_to_download = self._cache.get(f'toui-download-{path_id}')
+        file_to_download = self._user_vars._get(f'toui-download-{path_id}')
         debug(f"File to download: {file_to_download}")
         if file_to_download:
             return send_file(file_to_download, as_attachment=True)
 
     def _communicate(self, ws):
         """This is a private function."""
         validation = self._validate_ws(ws)
@@ -667,41 +677,84 @@
 
 
 class _UserVars(MutableMapping):
     """User-specific variables"""
 
     def __init__(self, cache) -> None:
         self._cache = cache
-        self._cache.set('toui-vars', {})
+        self._default_vars = {}
+
+    def _sid_check(self):
+        try:
+            session.keys()
+            session_exists = True
+        except:
+            session_exists = False
+        if session_exists:
+            user_dict = self._cache.get(session.sid)
+            if user_dict is None:
+                self._cache.set(session.sid, {"toui-vars": self._default_vars})
+            return session.sid
+
+    def _get_toui_vars(self):
+        sid = self._sid_check()
+        if sid:
+            return self._cache.get(sid)['toui-vars']
+        else:
+            return self._default_vars
+    
+    def _set_toui_vars(self, toui_vars):
+        sid = self._sid_check()
+        if sid:
+            self._cache.set(session.sid, {'toui-vars': toui_vars})
+        else:
+            self._default_vars = toui_vars
+
+    def _get(self, key):
+        self._sid_check()
+        return self._cache.get(session.sid).get(key)
+    
+    def _set(self, key, value):
+        """Avoid key='toui-vars'"""
+        self._sid_check()
+        sid_dict = self._cache.get(session.sid)
+        sid_dict[key] = value
+        self._cache.set(session.sid, sid_dict)
+
+    def _del(self, key):
+        self._sid_check()
+        sid_dict = self._cache.get(session.sid)
+        del sid_dict[key]
+        self._cache.set(session.sid, sid_dict)
 
     def __getitem__(self, key):
-        return self._cache.get('toui-vars')[key]
+        return self._get_toui_vars()[key]
     
     def __setitem__(self, key, value):
-        toui_vars = self._cache.get('toui-vars')
+        toui_vars = self._get_toui_vars()
         toui_vars[key] = value
-        self._cache.set('toui-vars', toui_vars)
+        self._set_toui_vars(toui_vars)
 
     def __delitem__(self, key: Any) -> None:
-        toui_vars = self._cache.get('toui-vars')
+        toui_vars = self._get_toui_vars()
         del toui_vars[key]
-        self._cache.set('toui-vars', toui_vars)
+        self._set_toui_vars(toui_vars)
 
     def __iter__(self):
-        for key in self._cache.get('toui-vars'):
+        for key in self._get_toui_vars():
             yield key
 
     def __len__(self) -> int:
-        return len(self._cache.get('toui-vars'))
+        return len(self._get_toui_vars())
     
     def __getattr__(self, name: str) -> Any:
-        return getattr(self._cache.get('toui-vars'), name)
+        return getattr(self._get_toui_vars(), name)
     
     def __repr__(self) -> str:
-        return repr(self._cache.get('toui-vars'))
+        return repr(self._get_toui_vars())
     
 
 class Website(_App):
     """
     A class that creates a web application from HTML files.
 
     Examples
```

### Comparing `toui-2.4.0/toui/elements.py` & `toui-2.4.1/toui/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -563,17 +563,15 @@
         style = self.get_attr('style')
         parser = tinycss.make_parser("page3")
         declarations = parser.parse_style_attr(style)[0]
         for declaration in declarations:
             if declaration.name == property:
                 property_value = ""
                 for v in declaration.value:
-                    property_value += str(v.value)
-                    if v.unit is not None:
-                        property_value += str(v.unit)
+                    property_value += v.as_css()
                 return property_value
 
     def set_style_property(self, property, value):
         """
         Sets the value of a CSS property inside the ``style`` attribute.
 
         Parameters
@@ -597,15 +595,15 @@
             new_style += declaration.name + ": "
             if declaration.name == property:
                 property_value = value
                 property_is_set = True
             else:
                 property_value = ""
                 for v in declaration.value:
-                    property_value += str(v.value) + str(v.unit)
+                    property_value += v.as_css()
             new_style += f"{property_value};"
         if not property_is_set:
             new_style += f"{property}: {value};"
         self.set_attr(name="style", value=new_style)
 
     def get_width_property(self):
         """
```

### Comparing `toui-2.4.0/toui/pages.py` & `toui-2.4.1/toui/pages.py`

 * *Files 0% similar despite different names*

```diff
@@ -468,15 +468,15 @@
             the return value will be ignored.
 
         """
         def new_func():
             original_return = self._basic_view_func()
             session['user page'] = copy(self)
             try:
-                user_id = self._app._cache.get("user-id")
+                user_id = self._app._user_vars._get("user-id")
                 if user_id:
                     session['_user_id'] = user_id
                 new_return = func()
                 if display_return_value:
                     del session['user page']
                     return new_return
                 else:
```

### Comparing `toui-2.4.0/toui/structure.py` & `toui-2.4.1/toui/structure.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.0/toui.egg-info/PKG-INFO` & `toui-2.4.1/toui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 2.4.0
+Version: 2.4.1
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `toui-2.4.0/toui.egg-info/SOURCES.txt` & `toui-2.4.1/toui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

