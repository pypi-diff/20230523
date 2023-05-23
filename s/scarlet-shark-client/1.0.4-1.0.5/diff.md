# Comparing `tmp/scarlet-shark-client-1.0.4.tar.gz` & `tmp/scarlet-shark-client-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scarlet-shark-client-1.0.4.tar", last modified: Wed May 10 11:22:24 2023, max compression
+gzip compressed data, was "scarlet-shark-client-1.0.5.tar", last modified: Tue May 23 09:30:52 2023, max compression
```

## Comparing `scarlet-shark-client-1.0.4.tar` & `scarlet-shark-client-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:22:24.670947 scarlet-shark-client-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-10 11:22:14.000000 scarlet-shark-client-1.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-10 11:22:24.670947 scarlet-shark-client-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-10 11:22:14.000000 scarlet-shark-client-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:22:24.670947 scarlet-shark-client-1.0.4/scarlet_shark_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:22:14.000000 scarlet-shark-client-1.0.4/scarlet_shark_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-10 11:22:14.000000 scarlet-shark-client-1.0.4/scarlet_shark_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:22:24.670947 scarlet-shark-client-1.0.4/scarlet_shark_client/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:22:14.000000 scarlet-shark-client-1.0.4/scarlet_shark_client/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-05-10 11:22:14.000000 scarlet-shark-client-1.0.4/scarlet_shark_client/clients/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-10 11:22:14.000000 scarlet-shark-client-1.0.4/scarlet_shark_client/clients/v04_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:22:24.670947 scarlet-shark-client-1.0.4/scarlet_shark_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-10 11:22:24.000000 scarlet-shark-client-1.0.4/scarlet_shark_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-10 11:22:24.000000 scarlet-shark-client-1.0.4/scarlet_shark_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 11:22:24.000000 scarlet-shark-client-1.0.4/scarlet_shark_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 11:22:24.000000 scarlet-shark-client-1.0.4/scarlet_shark_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 11:22:24.000000 scarlet-shark-client-1.0.4/scarlet_shark_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 11:22:24.670947 scarlet-shark-client-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-10 11:22:14.000000 scarlet-shark-client-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:30:52.889477 scarlet-shark-client-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-23 09:30:40.000000 scarlet-shark-client-1.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-23 09:30:52.889477 scarlet-shark-client-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-23 09:30:40.000000 scarlet-shark-client-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:30:52.885477 scarlet-shark-client-1.0.5/scarlet_shark_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:30:40.000000 scarlet-shark-client-1.0.5/scarlet_shark_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-23 09:30:40.000000 scarlet-shark-client-1.0.5/scarlet_shark_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:30:52.889477 scarlet-shark-client-1.0.5/scarlet_shark_client/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:30:40.000000 scarlet-shark-client-1.0.5/scarlet_shark_client/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-05-23 09:30:40.000000 scarlet-shark-client-1.0.5/scarlet_shark_client/clients/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-23 09:30:40.000000 scarlet-shark-client-1.0.5/scarlet_shark_client/clients/v04_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:30:52.889477 scarlet-shark-client-1.0.5/scarlet_shark_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-23 09:30:52.000000 scarlet-shark-client-1.0.5/scarlet_shark_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-23 09:30:52.000000 scarlet-shark-client-1.0.5/scarlet_shark_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:30:52.000000 scarlet-shark-client-1.0.5/scarlet_shark_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 09:30:52.000000 scarlet-shark-client-1.0.5/scarlet_shark_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 09:30:52.000000 scarlet-shark-client-1.0.5/scarlet_shark_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 09:30:52.889477 scarlet-shark-client-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-23 09:30:40.000000 scarlet-shark-client-1.0.5/setup.py
```

### Comparing `scarlet-shark-client-1.0.4/LICENSE.txt` & `scarlet-shark-client-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scarlet-shark-client-1.0.4/PKG-INFO` & `scarlet-shark-client-1.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scarlet-shark-client
-Version: 1.0.4
+Version: 1.0.5
 Summary: Scarlet Shark REST API Python client
 Home-page: https://github.com/PiRogueToolSuite/scarlet-shark-python
 Author: U+039b
 Author-email: esther@pts-project.org
 License: UNKNOWN
 Description: # scarlet-shark-python
         Scarlet Shark REST API Python client.
```

### Comparing `scarlet-shark-client-1.0.4/README.md` & `scarlet-shark-client-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `scarlet-shark-client-1.0.4/scarlet_shark_client/client.py` & `scarlet-shark-client-1.0.5/scarlet_shark_client/client.py`

 * *Files identical despite different names*

### Comparing `scarlet-shark-client-1.0.4/scarlet_shark_client/clients/abstract.py` & `scarlet-shark-client-1.0.5/scarlet_shark_client/clients/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,22 @@
 
     def _resolve_url(self, action_name: str, params) -> str:
         if action_name not in self.api_actions:
             raise Exception(f'The action [{action_name}] is not supported')
         query_parameters: dict = {}
         for k, v in params.items():
             if k != 'self' and v:
-                query_parameters[k] = v
+                key = k
+                if k == 'ip' and action_name == 'search_ip':
+                    key = 'ips[]'
+                elif k == 'email' and action_name == 'search_email':
+                    key = 'emails[]'
+                elif k == 'url' and action_name == 'search_url':
+                    key = 'urls[]'
+                query_parameters[key] = v
         if not query_parameters:
             raise Exception(f'At least query parameter has to be specified in [{params}]')
         endpoint = self.api_actions[action_name]
         query_string = urlencode(query_parameters)
         return f'{self.version}{endpoint}?{query_string}'
 
     def _prepare_request(self, uri: str):
@@ -74,19 +81,19 @@
         :return: Returns information on the given domain.
         """
         pass
 
     @abstractmethod
     def search_email(
             self,
-            emails: list[str],
+            email: str,
             nonce: Optional[int] = None) -> Optional[dict]:
         """
         Returns threat information for the given email addresses.
-        :param emails: String Array - Email addresses to search for threat data on
+        :param email: String - Email address to search for threat data on
         :param nonce: Integer [optional] - A nonce that is returned, if provided in the request
         :return: Returns threat information for the given email addresses.
         """
         pass
 
     @abstractmethod
     def search_hash(
@@ -102,22 +109,22 @@
         :return: Returns information on either a SHA256 or a MD5 hash.
         """
         pass
 
     @abstractmethod
     def search_ip(
             self,
-            ips: list[str],
+            ip: str,
             context: Optional[str] = None,
             time_period: Optional[int] = None,
             time_zone: Optional[str] = None,
             nonce: Optional[int] = None) -> Optional[dict]:
         """
         Looks up information for an IP and any threat intel information about that IP.
-        :param ips: String array - v4 or v6 IP address
+        :param ip: String - v4 or v6 IP address
         :param context: String [optional] – Possible values: [user_activity, none] - The context of the IP look up. This helps give a more accurate threat classification.
         :param time_period: Integer - The number of days to show security issues for.
         :param time_zone: String [optional] - PHP Time Zone Strings. Results will be returned in the given time zone. UTC is the default. See: https://www.php.net/manual/en/timezones.php
         :param nonce: Integer [optional] - A nonce that is returned, if provided in the request
         :return: Looks up information for an IP and any threat intel information about that IP
         """
         pass
@@ -166,16 +173,16 @@
         :return: Information about a given threat tool. The threat tool can be malware or a legitimate tool.
         """
         pass
 
     @abstractmethod
     def search_url(
             self,
-            urls: list[str],
+            url: str,
             nonce: Optional[int] = None) -> Optional[dict]:
         """
-        Looks up threat information for the given URLs.
-        :param urls: String Array - URLs to search for threat data on. The domain of each URL will automatically be changed from Unicode to an IDNA ASCII-compatible format
+        Looks up threat information for the given URL.
+        :param url: String - URL to search for threat data on.
         :param nonce: Integer [optional] - A nonce that is returned, if provided in the request
-        :return: Looks up threat information for the given URLs
+        :return: Looks up threat information for the given URL
         """
         pass
```

### Comparing `scarlet-shark-client-1.0.4/scarlet_shark_client/clients/v04_client.py` & `scarlet-shark-client-1.0.5/scarlet_shark_client/clients/v04_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,30 +31,30 @@
             domain: str,
             nonce: Optional[int] = None) -> Optional[dict]:
         uri = self._resolve_url(sys._getframe().f_code.co_name, locals())
         return self._prepare_request(uri)
 
     def search_email(
             self,
-            emails: list[str],
+            email: str,
             nonce: Optional[int] = None) -> Optional[dict]:
         uri = self._resolve_url(sys._getframe().f_code.co_name, locals())
         return self._prepare_request(uri)
 
     def search_hash(
             self,
             sha256: Optional[str] = None,
             md5: Optional[str] = None,
             nonce: Optional[int] = None) -> Optional[dict]:
         uri = self._resolve_url(sys._getframe().f_code.co_name, locals())
         return self._prepare_request(uri)
 
     def search_ip(
             self,
-            ips: list[str],
+            ip: str,
             context: Optional[str] = None,
             time_period: Optional[int] = None,
             time_zone: Optional[str] = None,
             nonce: Optional[int] = None) -> Optional[dict]:
         uri = self._resolve_url(sys._getframe().f_code.co_name, locals())
         return self._prepare_request(uri)
 
@@ -80,11 +80,11 @@
             threat_actor_id: Optional[int] = None,
             nonce: Optional[int] = None) -> Optional[dict]:
         uri = self._resolve_url(sys._getframe().f_code.co_name, locals())
         return self._prepare_request(uri)
 
     def search_url(
             self,
-            urls: list[str],
+            url: str,
             nonce: Optional[int] = None) -> Optional[dict]:
         uri = self._resolve_url(sys._getframe().f_code.co_name, locals())
         return self._prepare_request(uri)
```

### Comparing `scarlet-shark-client-1.0.4/scarlet_shark_client.egg-info/PKG-INFO` & `scarlet-shark-client-1.0.5/scarlet_shark_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scarlet-shark-client
-Version: 1.0.4
+Version: 1.0.5
 Summary: Scarlet Shark REST API Python client
 Home-page: https://github.com/PiRogueToolSuite/scarlet-shark-python
 Author: U+039b
 Author-email: esther@pts-project.org
 License: UNKNOWN
 Description: # scarlet-shark-python
         Scarlet Shark REST API Python client.
```

### Comparing `scarlet-shark-client-1.0.4/setup.py` & `scarlet-shark-client-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 install_requires = [
     'requests==2.29.0'
 ]
 
 setup(
     name='scarlet-shark-client',
-    version='1.0.4',
+    version='1.0.5',
     description='Scarlet Shark REST API Python client',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='U+039b',
     author_email='esther@pts-project.org',
     url='https://github.com/PiRogueToolSuite/scarlet-shark-python',
     packages=find_packages(exclude=['*.tests', '*.tests.*', 'test*', 'tests']),
```

