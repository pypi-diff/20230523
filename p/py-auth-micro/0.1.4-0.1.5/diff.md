# Comparing `tmp/py_auth_micro-0.1.4.tar.gz` & `tmp/py_auth_micro-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_auth_micro-0.1.4.tar", last modified: Mon May 22 13:06:03 2023, max compression
+gzip compressed data, was "py_auth_micro-0.1.5.tar", last modified: Mon May 22 15:21:56 2023, max compression
```

## Comparing `py_auth_micro-0.1.4.tar` & `py_auth_micro-0.1.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:06:03.316560 py_auth_micro-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-22 13:06:03.316560 py_auth_micro-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:06:03.308560 py_auth_micro-0.1.4/py_auth_micro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:06:03.308560 py_auth_micro-0.1.4/py_auth_micro/Config/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/Config/_appconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/Config/_dbconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/Config/_ldapconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:06:03.312560 py_auth_micro-0.1.4/py_auth_micro/Core/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/Core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/Core/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/Core/_ldap_interactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:06:03.312560 py_auth_micro-0.1.4/py_auth_micro/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/Exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:06:03.312560 py_auth_micro-0.1.4/py_auth_micro/LoginHandler/
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/LoginHandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/LoginHandler/_loginbaseclass.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/LoginHandler/_loginkerberos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/LoginHandler/_loginldap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/LoginHandler/_loginlocal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:06:03.312560 py_auth_micro-0.1.4/py_auth_micro/Models/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/Models/_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/Models/_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/Models/_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:06:03.316560 py_auth_micro-0.1.4/py_auth_micro/WorkFlows/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/WorkFlows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7945 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/WorkFlows/_groupworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/WorkFlows/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/WorkFlows/_sessionworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/WorkFlows/_userworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/py_auth_micro/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:06:03.308560 py_auth_micro-0.1.4/py_auth_micro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-22 13:06:03.000000 py_auth_micro-0.1.4/py_auth_micro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-22 13:06:03.000000 py_auth_micro-0.1.4/py_auth_micro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:06:03.000000 py_auth_micro-0.1.4/py_auth_micro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-22 13:06:03.000000 py_auth_micro-0.1.4/py_auth_micro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 13:06:03.000000 py_auth_micro-0.1.4/py_auth_micro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-22 13:06:03.316560 py_auth_micro-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-22 13:05:10.000000 py_auth_micro-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:56.540946 py_auth_micro-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-22 15:21:56.540946 py_auth_micro-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:56.536946 py_auth_micro-0.1.5/py_auth_micro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:56.540946 py_auth_micro-0.1.5/py_auth_micro/Config/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/Config/_appconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/Config/_dbconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/Config/_ldapconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:56.540946 py_auth_micro-0.1.5/py_auth_micro/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/Core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/Core/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/Core/_ldap_interactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:56.540946 py_auth_micro-0.1.5/py_auth_micro/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/Exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:56.540946 py_auth_micro-0.1.5/py_auth_micro/LoginHandler/
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/LoginHandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/LoginHandler/_loginbaseclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/LoginHandler/_loginkerberos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/LoginHandler/_loginldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/LoginHandler/_loginlocal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:56.540946 py_auth_micro-0.1.5/py_auth_micro/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/Models/_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/Models/_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/Models/_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:56.540946 py_auth_micro-0.1.5/py_auth_micro/WorkFlows/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/WorkFlows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/WorkFlows/_groupworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/WorkFlows/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/WorkFlows/_sessionworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/WorkFlows/_userworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/py_auth_micro/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:56.540946 py_auth_micro-0.1.5/py_auth_micro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-22 15:21:56.000000 py_auth_micro-0.1.5/py_auth_micro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-22 15:21:56.000000 py_auth_micro-0.1.5/py_auth_micro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:21:56.000000 py_auth_micro-0.1.5/py_auth_micro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-22 15:21:56.000000 py_auth_micro-0.1.5/py_auth_micro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 15:21:56.000000 py_auth_micro-0.1.5/py_auth_micro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-22 15:21:56.540946 py_auth_micro-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-22 15:21:12.000000 py_auth_micro-0.1.5/setup.py
```

### Comparing `py_auth_micro-0.1.4/LICENSE` & `py_auth_micro-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.4/PKG-INFO` & `py_auth_micro-0.1.5/py_auth_micro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py_auth_micro
-Version: 0.1.4
+Name: py-auth-micro
+Version: 0.1.5
 Summary: A wrapper around pyjwt
 Home-page: https://github.com/bad-microservices/py_auth_micro
 Author: Ole Hannemann
 Author-email: cerberus885@gmail.com
 License: MIT
 Keywords: JWT
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `py_auth_micro-0.1.4/README.rst` & `py_auth_micro-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.4/py_auth_micro/Config/_appconfig.py` & `py_auth_micro-0.1.5/py_auth_micro/Config/_appconfig.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.4/py_auth_micro/Config/_dbconfig.py` & `py_auth_micro-0.1.5/py_auth_micro/Config/_dbconfig.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.4/py_auth_micro/Config/_ldapconfig.py` & `py_auth_micro-0.1.5/py_auth_micro/Config/_ldapconfig.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.4/py_auth_micro/Core/_ldap_interactions.py` & `py_auth_micro-0.1.5/py_auth_micro/Core/_ldap_interactions.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.4/py_auth_micro/LoginHandler/__init__.py` & `py_auth_micro-0.1.5/py_auth_micro/LoginHandler/__init__.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.4/py_auth_micro/LoginHandler/_loginbaseclass.py` & `py_auth_micro-0.1.5/py_auth_micro/LoginHandler/_loginbaseclass.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.4/py_auth_micro/LoginHandler/_loginldap.py` & `py_auth_micro-0.1.5/py_auth_micro/LoginHandler/_loginldap.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.4/py_auth_micro/LoginHandler/_loginlocal.py` & `py_auth_micro-0.1.5/py_auth_micro/LoginHandler/_loginlocal.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.4/py_auth_micro/Models/_token.py` & `py_auth_micro-0.1.5/py_auth_micro/Models/_token.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.4/py_auth_micro/Models/_user.py` & `py_auth_micro-0.1.5/py_auth_micro/Models/_user.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.4/py_auth_micro/WorkFlows/__init__.py` & `py_auth_micro-0.1.5/py_auth_micro/WorkFlows/__init__.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.4/py_auth_micro/WorkFlows/_groupworkflow.py` & `py_auth_micro-0.1.5/py_auth_micro/WorkFlows/_groupworkflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
 
         try:
             await group.users.remove(user)
         except Exception:
             return {
                 "resp_code": 500,
                 "resp_data": {
-                    "msg": f"could not remove user {username} to group {groupname}"
+                    "msg": f"could not remove user {username} from group {groupname}"
                 },
             }
 
         return {
             "resp_code": 200,
-            "resp_data": {"msg": f"removed user {username} to group {groupname}"},
+            "resp_data": {"msg": f"removed user {username} from group {groupname}"},
         }
```

### Comparing `py_auth_micro-0.1.4/py_auth_micro/WorkFlows/_misc.py` & `py_auth_micro-0.1.5/py_auth_micro/WorkFlows/_misc.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.4/py_auth_micro/WorkFlows/_sessionworkflow.py` & `py_auth_micro-0.1.5/py_auth_micro/WorkFlows/_sessionworkflow.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.4/py_auth_micro/WorkFlows/_userworkflow.py` & `py_auth_micro-0.1.5/py_auth_micro/WorkFlows/_userworkflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,39 +158,36 @@
         Args:
             username (str): Username of the User we want the Data from
             access_token (str, optional): Access Token of the Requesting User. Defaults to None.
 
         Returns:
             dict: Dictionary containing User Information
         """
-        try:
-            user = await User.get(username=username)
-        except Exception:
-            return "wtf"
+        user = await User.get(username=username)
 
         user_dict = {}
         user_dict["username"] = user.username
         user_dict["activated"] = user.activated
         user_dict["created_at"] = user.created_at.isoformat()
 
         if access_token is None:
-            return user_dict
+            return {"resp_code": 200, "resp_data": user_dict}
 
         requesting_user, is_admin = _get_info_from_token(
             self.jwt_validator, self.app_cfg, access_token
         )
 
         if user.username != requesting_user and not is_admin:
-            return user_dict
+            return {"resp_code": 200, "resp_data": user_dict}
 
         token = await user.token
 
         if token is None:
             user_dict["token_info"] = None
-            return user_dict
+            return {"resp_code": 200, "resp_data": user_dict}
 
         user_dict["token_info"] = {
             "valid_until": token.valid_until.isoformat(),
             "last_use": token.last_use.isoformat(),
             "vhost": token.vhost,
         }
```

### Comparing `py_auth_micro-0.1.4/py_auth_micro.egg-info/PKG-INFO` & `py_auth_micro-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py-auth-micro
-Version: 0.1.4
+Name: py_auth_micro
+Version: 0.1.5
 Summary: A wrapper around pyjwt
 Home-page: https://github.com/bad-microservices/py_auth_micro
 Author: Ole Hannemann
 Author-email: cerberus885@gmail.com
 License: MIT
 Keywords: JWT
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `py_auth_micro-0.1.4/py_auth_micro.egg-info/SOURCES.txt` & `py_auth_micro-0.1.5/py_auth_micro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.4/setup.cfg` & `py_auth_micro-0.1.5/setup.cfg`

 * *Files identical despite different names*

