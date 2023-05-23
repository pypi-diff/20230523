# Comparing `tmp/im-squonk2-client-2.1.2.tar.gz` & `tmp/im-squonk2-client-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "im-squonk2-client-2.1.2.tar", last modified: Wed Oct 26 17:00:16 2022, max compression
+gzip compressed data, was "im-squonk2-client-2.2.0.tar", last modified: Tue May 23 14:49:51 2023, max compression
```

## Comparing `im-squonk2-client-2.1.2.tar` & `im-squonk2-client-2.2.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 17:00:16.214166 im-squonk2-client-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-10-26 17:00:06.000000 im-squonk2-client-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-26 17:00:06.000000 im-squonk2-client-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7885 2022-10-26 17:00:16.210166 im-squonk2-client-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7151 2022-10-26 17:00:06.000000 im-squonk2-client-2.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-10-26 17:00:06.000000 im-squonk2-client-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-10-26 17:00:06.000000 im-squonk2-client-2.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-26 17:00:16.214166 im-squonk2-client-2.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1579 2022-10-26 17:00:06.000000 im-squonk2-client-2.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 17:00:16.210166 im-squonk2-client-2.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 17:00:16.210166 im-squonk2-client-2.1.2/src/im_squonk2_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7885 2022-10-26 17:00:16.000000 im-squonk2-client-2.1.2/src/im_squonk2_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-10-26 17:00:16.000000 im-squonk2-client-2.1.2/src/im_squonk2_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 17:00:16.000000 im-squonk2-client-2.1.2/src/im_squonk2_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 17:00:15.000000 im-squonk2-client-2.1.2/src/im_squonk2_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-26 17:00:16.000000 im-squonk2-client-2.1.2/src/im_squonk2_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-26 17:00:16.000000 im-squonk2-client-2.1.2/src/im_squonk2_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 17:00:16.210166 im-squonk2-client-2.1.2/src/squonk2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 17:00:06.000000 im-squonk2-client-2.1.2/src/squonk2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19931 2022-10-26 17:00:06.000000 im-squonk2-client-2.1.2/src/squonk2/as_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4751 2022-10-26 17:00:06.000000 im-squonk2-client-2.1.2/src/squonk2/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)    46803 2022-10-26 17:00:06.000000 im-squonk2-client-2.1.2/src/squonk2/dm_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     9935 2022-10-26 17:00:06.000000 im-squonk2-client-2.1.2/src/squonk2/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:49:51.820092 im-squonk2-client-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-05-23 14:49:51.820092 im-squonk2-client-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:49:51.820092 im-squonk2-client-2.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1579 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:49:51.812091 im-squonk2-client-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:49:51.816091 im-squonk2-client-2.2.0/src/im_squonk2_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-05-23 14:49:51.000000 im-squonk2-client-2.2.0/src/im_squonk2_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-23 14:49:51.000000 im-squonk2-client-2.2.0/src/im_squonk2_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:49:51.000000 im-squonk2-client-2.2.0/src/im_squonk2_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:49:51.000000 im-squonk2-client-2.2.0/src/im_squonk2_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 14:49:51.000000 im-squonk2-client-2.2.0/src/im_squonk2_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 14:49:51.000000 im-squonk2-client-2.2.0/src/im_squonk2_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:49:51.820092 im-squonk2-client-2.2.0/src/squonk2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/src/squonk2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19931 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/src/squonk2/as_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/src/squonk2/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46803 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/src/squonk2/dm_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/src/squonk2/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-23 14:49:39.000000 im-squonk2-client-2.2.0/src/squonk2/ui_api.py
```

### Comparing `im-squonk2-client-2.1.2/LICENSE` & `im-squonk2-client-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `im-squonk2-client-2.1.2/PKG-INFO` & `im-squonk2-client-2.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-squonk2-client
-Version: 2.1.2
+Version: 2.2.0
 Summary: Squonk2 Python Client
 Home-page: https://github.com/informaticsmatters/squonk2-python-client
 Author: Alan Christie
 Author-email: achristie@informaticsmatters.com
 License: MIT
 Keywords: api
 Platform: any
@@ -116,14 +116,30 @@
 
 - ``AsApiRv``
 
 It contains a boolean ``success`` field and a dictionary ``msg`` field. The
 ``msg`` typically contains the underlying REST API response content
 (rendered as a Python dictionary), or an error message if the call failed.
 
+Simplified UI API
+=================
+The following Squonk2 UI API functions are available: -
+
+- ``UiApi.set_api_url()``
+
+- ``UiApi.get_version()``
+
+A ``namedtuple`` is used as the return value for many of the methods: -
+
+- ``UiApiRv``
+
+It contains a boolean ``success`` field and a dictionary ``msg`` field. The
+``msg`` typically contains the underlying REST API response content
+(rendered as a Python dictionary), or an error message if the call failed.
+
 Debugging the API requests
 ==========================
 For development purposes you can expose detailed debug information relating to
 the underlying API requests by setting the environment variable
 ``SQUONK2_API_DEBUG_REQUESTS``::
 
     export SQUONK2_API_DEBUG_REQUESTS=yes
@@ -182,14 +198,17 @@
         as-hostname: as.example.com
         dm-hostname: dm.example.com
         # The username and password of an admin user that has access
         # to the Account Server and Data Manager.
         # The user *MUST* have admin rights.
         admin-user: dlister
         admin-password: blob1234
+        # The hostname of the Squonk2 web application, without a 'http' prefix.
+        # if present, this is used to obtain the UI version.
+        ui-hostname: ui.example.com
 
     # The final part of the file is a 'default' property,
     # which Squeck uses to select the an environment from the block above
     # when all else fails. It's simply the name of one of the environment
     # declarations above.
     default: site-a
```

### Comparing `im-squonk2-client-2.1.2/README.rst` & `im-squonk2-client-2.2.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -95,14 +95,30 @@
 
 - ``AsApiRv``
 
 It contains a boolean ``success`` field and a dictionary ``msg`` field. The
 ``msg`` typically contains the underlying REST API response content
 (rendered as a Python dictionary), or an error message if the call failed.
 
+Simplified UI API
+=================
+The following Squonk2 UI API functions are available: -
+
+- ``UiApi.set_api_url()``
+
+- ``UiApi.get_version()``
+
+A ``namedtuple`` is used as the return value for many of the methods: -
+
+- ``UiApiRv``
+
+It contains a boolean ``success`` field and a dictionary ``msg`` field. The
+``msg`` typically contains the underlying REST API response content
+(rendered as a Python dictionary), or an error message if the call failed.
+
 Debugging the API requests
 ==========================
 For development purposes you can expose detailed debug information relating to
 the underlying API requests by setting the environment variable
 ``SQUONK2_API_DEBUG_REQUESTS``::
 
     export SQUONK2_API_DEBUG_REQUESTS=yes
@@ -161,14 +177,17 @@
         as-hostname: as.example.com
         dm-hostname: dm.example.com
         # The username and password of an admin user that has access
         # to the Account Server and Data Manager.
         # The user *MUST* have admin rights.
         admin-user: dlister
         admin-password: blob1234
+        # The hostname of the Squonk2 web application, without a 'http' prefix.
+        # if present, this is used to obtain the UI version.
+        ui-hostname: ui.example.com
 
     # The final part of the file is a 'default' property,
     # which Squeck uses to select the an environment from the block above
     # when all else fails. It's simply the name of one of the environment
     # declarations above.
     default: site-a
```

### Comparing `im-squonk2-client-2.1.2/setup.py` & `im-squonk2-client-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `im-squonk2-client-2.1.2/src/im_squonk2_client.egg-info/PKG-INFO` & `im-squonk2-client-2.2.0/src/im_squonk2_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-squonk2-client
-Version: 2.1.2
+Version: 2.2.0
 Summary: Squonk2 Python Client
 Home-page: https://github.com/informaticsmatters/squonk2-python-client
 Author: Alan Christie
 Author-email: achristie@informaticsmatters.com
 License: MIT
 Keywords: api
 Platform: any
@@ -116,14 +116,30 @@
 
 - ``AsApiRv``
 
 It contains a boolean ``success`` field and a dictionary ``msg`` field. The
 ``msg`` typically contains the underlying REST API response content
 (rendered as a Python dictionary), or an error message if the call failed.
 
+Simplified UI API
+=================
+The following Squonk2 UI API functions are available: -
+
+- ``UiApi.set_api_url()``
+
+- ``UiApi.get_version()``
+
+A ``namedtuple`` is used as the return value for many of the methods: -
+
+- ``UiApiRv``
+
+It contains a boolean ``success`` field and a dictionary ``msg`` field. The
+``msg`` typically contains the underlying REST API response content
+(rendered as a Python dictionary), or an error message if the call failed.
+
 Debugging the API requests
 ==========================
 For development purposes you can expose detailed debug information relating to
 the underlying API requests by setting the environment variable
 ``SQUONK2_API_DEBUG_REQUESTS``::
 
     export SQUONK2_API_DEBUG_REQUESTS=yes
@@ -182,14 +198,17 @@
         as-hostname: as.example.com
         dm-hostname: dm.example.com
         # The username and password of an admin user that has access
         # to the Account Server and Data Manager.
         # The user *MUST* have admin rights.
         admin-user: dlister
         admin-password: blob1234
+        # The hostname of the Squonk2 web application, without a 'http' prefix.
+        # if present, this is used to obtain the UI version.
+        ui-hostname: ui.example.com
 
     # The final part of the file is a 'default' property,
     # which Squeck uses to select the an environment from the block above
     # when all else fails. It's simply the name of one of the environment
     # declarations above.
     default: site-a
```

### Comparing `im-squonk2-client-2.1.2/src/squonk2/as_api.py` & `im-squonk2-client-2.2.0/src/squonk2/as_api.py`

 * *Files identical despite different names*

### Comparing `im-squonk2-client-2.1.2/src/squonk2/auth.py` & `im-squonk2-client-2.2.0/src/squonk2/auth.py`

 * *Files identical despite different names*

### Comparing `im-squonk2-client-2.1.2/src/squonk2/dm_api.py` & `im-squonk2-client-2.2.0/src/squonk2/dm_api.py`

 * *Files identical despite different names*

### Comparing `im-squonk2-client-2.1.2/src/squonk2/environment.py` & `im-squonk2-client-2.2.0/src/squonk2/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 _KEYCLOAK_DM_CLIENT_ID_KEY: str = "keycloak-dm-client-id"
 _DM_HOSTNAME_KEY: str = "dm-hostname"
 _ADMIN_USER_KEY: str = "admin-user"
 _ADMIN_PASSWORD_KEY: str = "admin-password"
 # Optional keys
 _KEYCLOAK_AS_CLIENT_ID_KEY: str = "keycloak-as-client-id"
 _AS_HOSTNAME_KEY: str = "as-hostname"
+_UI_HOSTNAME_KEY: str = "ui-hostname"
 
 
 class Environment:
     """Loads the values from the environment file for the given environment."""
 
     # Location of the file
     __environments_file: str = os.path.expandvars(os.path.expanduser(_ENVIRONMENT_FILE))
@@ -159,14 +160,17 @@
         # Get the optional key values...
         self.__keycloak_as_client_id: Optional[str] = self.__get_config_value(
             _KEYCLOAK_AS_CLIENT_ID_KEY, optional=True
         )
         self.__as_hostname: Optional[str] = self.__get_config_value(
             _AS_HOSTNAME_KEY, optional=True
         )
+        self.__ui_hostname: Optional[str] = self.__get_config_value(
+            _UI_HOSTNAME_KEY, optional=True
+        )
 
     @property
     def environment(self) -> str:
         """Return the environment name."""
         return self.__environment
 
     @property
@@ -251,7 +255,27 @@
         if not self.__dm_hostname.startswith("http"):
             ret_val: str = f"https://{self.__dm_hostname}"
         else:
             ret_val = self.__dm_hostname
         if not ret_val.endswith("/data-manager-api"):
             ret_val += "/data-manager-api"
         return ret_val
+
+    @property
+    def ui_hostname(self) -> Optional[str]:
+        """Return the web/UI hostname. This is the unmodified
+        value found in the environment.
+        """
+        return self.__ui_hostname
+
+    @property
+    def ui_api(self) -> Optional[str]:
+        """Return the web/UI API. This is the UI hostname
+        with a 'http' prefix and '/api' postfix.
+        """
+        if not self.__ui_hostname:
+            return None
+        if not self.__ui_hostname.startswith("http"):
+            ret_val: str = f"https://{self.__ui_hostname}/api"
+        else:
+            ret_val = self.__ui_hostname
+        return ret_val
```

