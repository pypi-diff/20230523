# Comparing `tmp/im-squeck-1.0.1.tar.gz` & `tmp/im-squeck-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "im-squeck-1.0.1.tar", last modified: Wed Oct 26 14:50:09 2022, max compression
+gzip compressed data, was "im-squeck-1.0.2.tar", last modified: Tue May 23 13:27:10 2023, max compression
```

## Comparing `im-squeck-1.0.1.tar` & `im-squeck-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:50:09.987139 im-squeck-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-10-26 14:49:56.000000 im-squeck-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-10-26 14:49:56.000000 im-squeck-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3331 2022-10-26 14:50:09.987139 im-squeck-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2701 2022-10-26 14:49:56.000000 im-squeck-1.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-10-26 14:49:56.000000 im-squeck-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-10-26 14:49:56.000000 im-squeck-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-26 14:50:09.987139 im-squeck-1.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1594 2022-10-26 14:49:56.000000 im-squeck-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:50:09.983139 im-squeck-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:50:09.983139 im-squeck-1.0.1/src/im_squeck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3331 2022-10-26 14:50:09.000000 im-squeck-1.0.1/src/im_squeck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-10-26 14:50:09.000000 im-squeck-1.0.1/src/im_squeck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 14:50:09.000000 im-squeck-1.0.1/src/im_squeck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-26 14:50:09.000000 im-squeck-1.0.1/src/im_squeck.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 14:50:09.000000 im-squeck-1.0.1/src/im_squeck.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-10-26 14:50:09.000000 im-squeck-1.0.1/src/im_squeck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-26 14:50:09.000000 im-squeck-1.0.1/src/im_squeck.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:50:09.987139 im-squeck-1.0.1/src/squeck/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-26 14:50:03.000000 im-squeck-1.0.1/src/squeck/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 14:49:56.000000 im-squeck-1.0.1/src/squeck/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      391 2022-10-26 14:49:56.000000 im-squeck-1.0.1/src/squeck/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-10-26 14:49:56.000000 im-squeck-1.0.1/src/squeck/access_token.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-10-26 14:49:56.000000 im-squeck-1.0.1/src/squeck/common.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2825 2022-10-26 14:49:56.000000 im-squeck-1.0.1/src/squeck/squeck.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:50:09.987139 im-squeck-1.0.1/src/squeck/widgets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 14:49:56.000000 im-squeck-1.0.1/src/squeck/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5838 2022-10-26 14:49:56.000000 im-squeck-1.0.1/src/squeck/widgets/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:27:10.528102 im-squeck-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-23 13:26:56.000000 im-squeck-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-23 13:26:56.000000 im-squeck-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-23 13:27:10.524101 im-squeck-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-23 13:26:56.000000 im-squeck-1.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 13:26:56.000000 im-squeck-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-23 13:26:56.000000 im-squeck-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:27:10.528102 im-squeck-1.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1594 2023-05-23 13:26:56.000000 im-squeck-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:27:10.524101 im-squeck-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:27:10.524101 im-squeck-1.0.2/src/im_squeck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-23 13:27:10.000000 im-squeck-1.0.2/src/im_squeck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-23 13:27:10.000000 im-squeck-1.0.2/src/im_squeck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:27:10.000000 im-squeck-1.0.2/src/im_squeck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 13:27:10.000000 im-squeck-1.0.2/src/im_squeck.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:27:10.000000 im-squeck-1.0.2/src/im_squeck.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-23 13:27:10.000000 im-squeck-1.0.2/src/im_squeck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 13:27:10.000000 im-squeck-1.0.2/src/im_squeck.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:27:10.524101 im-squeck-1.0.2/src/squeck/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 13:27:02.000000 im-squeck-1.0.2/src/squeck/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:56.000000 im-squeck-1.0.2/src/squeck/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      391 2023-05-23 13:26:56.000000 im-squeck-1.0.2/src/squeck/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-23 13:26:56.000000 im-squeck-1.0.2/src/squeck/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-23 13:26:56.000000 im-squeck-1.0.2/src/squeck/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2825 2023-05-23 13:26:56.000000 im-squeck-1.0.2/src/squeck/squeck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:27:10.524101 im-squeck-1.0.2/src/squeck/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:56.000000 im-squeck-1.0.2/src/squeck/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-05-23 13:26:56.000000 im-squeck-1.0.2/src/squeck/widgets/env.py
```

### Comparing `im-squeck-1.0.1/LICENSE` & `im-squeck-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `im-squeck-1.0.1/PKG-INFO` & `im-squeck-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-squeck
-Version: 1.0.1
+Version: 1.0.2
 Summary: The IM Squonk2 Deck (Squeck)
 Home-page: https://github.com/informaticsmatters/squonk2-deck
 Author: Alan Christie
 Author-email: achristie@informaticsmatters.com
 License: MIT
 Keywords: configuration
 Platform: any
```

### Comparing `im-squeck-1.0.1/README.rst` & `im-squeck-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `im-squeck-1.0.1/setup.py` & `im-squeck-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `im-squeck-1.0.1/src/im_squeck.egg-info/PKG-INFO` & `im-squeck-1.0.2/src/im_squeck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-squeck
-Version: 1.0.1
+Version: 1.0.2
 Summary: The IM Squonk2 Deck (Squeck)
 Home-page: https://github.com/informaticsmatters/squonk2-deck
 Author: Alan Christie
 Author-email: achristie@informaticsmatters.com
 License: MIT
 Keywords: configuration
 Platform: any
```

### Comparing `im-squeck-1.0.1/src/im_squeck.egg-info/SOURCES.txt` & `im-squeck-1.0.2/src/im_squeck.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `im-squeck-1.0.1/src/squeck/access_token.py` & `im-squeck-1.0.2/src/squeck/access_token.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,38 +12,38 @@
     def get_as_access_token(
         cls, env: Environment, *, prior_token: Optional[str] = None
     ) -> Optional[str]:
         """Returns a token for the AS API.
         This returns None on error or if the client ID is not defined.
         """
         assert env
-        if not env.keycloak_as_client_id():
+        if not env.keycloak_as_client_id:
             return None
         access_token: Optional[str] = Auth.get_access_token(
-            keycloak_url=env.keycloak_url(),
-            keycloak_realm=env.keycloak_realm(),
-            keycloak_client_id=env.keycloak_as_client_id(),
-            username=env.admin_user(),
-            password=env.admin_password(),
+            keycloak_url=env.keycloak_url,
+            keycloak_realm=env.keycloak_realm,
+            keycloak_client_id=env.keycloak_as_client_id,
+            username=env.admin_user,
+            password=env.admin_password,
             prior_token=prior_token,
             timeout_s=2,
         )
         return access_token
 
     @classmethod
     def get_dm_access_token(
         cls, env: Environment, *, prior_token: Optional[str] = None
     ) -> Optional[str]:
         """Returns a token for the DM API
         or None if a token could not be obtained."""
         assert env
-        if not env.keycloak_dm_client_id():
+        if not env.keycloak_dm_client_id:
             return None
         access_token: Optional[str] = Auth.get_access_token(
-            keycloak_url=env.keycloak_url(),
-            keycloak_realm=env.keycloak_realm(),
-            keycloak_client_id=env.keycloak_dm_client_id(),
-            username=env.admin_user(),
-            password=env.admin_password(),
+            keycloak_url=env.keycloak_url,
+            keycloak_realm=env.keycloak_realm,
+            keycloak_client_id=env.keycloak_dm_client_id,
+            username=env.admin_user,
+            password=env.admin_password,
             prior_token=prior_token,
         )
         return access_token
```

### Comparing `im-squeck-1.0.1/src/squeck/common.py` & `im-squeck-1.0.2/src/squeck/common.py`

 * *Files identical despite different names*

### Comparing `im-squeck-1.0.1/src/squeck/squeck.py` & `im-squeck-1.0.2/src/squeck/squeck.py`

 * *Files identical despite different names*

### Comparing `im-squeck-1.0.1/src/squeck/widgets/env.py` & `im-squeck-1.0.2/src/squeck/widgets/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 
     def __init__(self, environment_name: str) -> None:
         super().__init__()
         self.environment_name = environment_name
         self.environment = Environment(environment_name)
 
         self.as_api: Optional[AsApi] = None
-        if self.environment.as_api():
+        if self.environment.as_api:
             self.as_api = AsApi()
-            self.as_api.set_api_url(self.environment.as_api(), verify_ssl_cert=False)
+            self.as_api.set_api_url(self.environment.as_api, verify_ssl_cert=False)
         self.dm_api: Optional[AsApi] = None
-        if self.environment.dm_api():
+        if self.environment.dm_api:
             self.dm_api = DmApi()
-            self.dm_api.set_api_url(self.environment.dm_api(), verify_ssl_cert=False)
+            self.dm_api.set_api_url(self.environment.dm_api, verify_ssl_cert=False)
 
         self.panel_style: Style = Style(color="grey54", bgcolor="black")
 
     def on_mount(self) -> None:
         """Widget initialisation."""
         # Set an interval timer - we check the AS and DM APIs
         # regularly trying to get the version of each.
@@ -102,30 +102,28 @@
             collapse_padding=True,
             box=None,
         )
         table.add_column("Key", style=_KEY_STYLE, no_wrap=True, justify="right")
         table.add_column("Value", style=_KEY_VALUE_STYLE, no_wrap=True)
 
         # The 'Authentication host'
-        kc_host = Text(
-            f"{self.environment.keycloak_hostname()}", style=_KEY_VALUE_STYLE
-        )
+        kc_host = Text(f"{self.environment.keycloak_hostname}", style=_KEY_VALUE_STYLE)
 
         # The API lines are also dynamically styled.
-        as_hostname: Optional[str] = self.environment.as_hostname()
+        as_hostname: Optional[str] = self.environment.as_hostname
         if as_hostname:
             as_hostname_text: Text = Text(as_hostname + " ", style=_KEY_VALUE_STYLE)
             if self.as_access_token:
                 as_hostname_text.append(common.TICK)
             else:
                 as_hostname_text.append(common.CROSS)
         else:
             as_hostname_text = Text("Undefined", style=_VALUE_ERROR_STYLE)
 
-        dm_hostname: Optional[str] = self.environment.dm_hostname()
+        dm_hostname: Optional[str] = self.environment.dm_hostname
         if dm_hostname:
             dm_hostname_text: Text = Text(dm_hostname + " ", style=_KEY_VALUE_STYLE)
             if self.dm_access_token:
                 dm_hostname_text.append(common.TICK)
             else:
                 dm_hostname_text.append(common.CROSS)
         else:
```

