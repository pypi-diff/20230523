# Comparing `tmp/ptapi42-1.0.3.tar.gz` & `tmp/ptapi42-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptapi42-1.0.3.tar", last modified: Tue Apr 11 08:09:03 2023, max compression
+gzip compressed data, was "ptapi42-1.0.4.tar", last modified: Tue May 23 09:46:15 2023, max compression
```

## Comparing `ptapi42-1.0.3.tar` & `ptapi42-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 vitor     (1000) vitor     (1000)        0 2023-04-11 08:09:03.896004 ptapi42-1.0.3/
--rw-rw-r--   0 vitor     (1000) vitor     (1000)     1073 2023-04-11 08:06:49.000000 ptapi42-1.0.3/LICENSE
--rw-rw-r--   0 vitor     (1000) vitor     (1000)     5677 2023-04-11 08:09:03.896004 ptapi42-1.0.3/PKG-INFO
--rw-rw-r--   0 vitor     (1000) vitor     (1000)     3865 2023-04-11 08:06:49.000000 ptapi42-1.0.3/README.md
-drwxrwxr-x   0 vitor     (1000) vitor     (1000)        0 2023-04-11 08:09:03.896004 ptapi42-1.0.3/ptapi42/
--rw-rw-r--   0 vitor     (1000) vitor     (1000)       39 2023-04-11 08:06:49.000000 ptapi42-1.0.3/ptapi42/__init__.py
--rw-rw-r--   0 vitor     (1000) vitor     (1000)    26159 2023-04-11 08:06:49.000000 ptapi42-1.0.3/ptapi42/api42.py
--rw-rw-r--   0 vitor     (1000) vitor     (1000)     3210 2023-04-11 08:06:49.000000 ptapi42-1.0.3/ptapi42/api42_token.py
--rw-rw-r--   0 vitor     (1000) vitor     (1000)     1372 2023-04-11 08:06:49.000000 ptapi42-1.0.3/ptapi42/config.py
-drwxrwxr-x   0 vitor     (1000) vitor     (1000)        0 2023-04-11 08:09:03.896004 ptapi42-1.0.3/ptapi42.egg-info/
--rw-rw-r--   0 vitor     (1000) vitor     (1000)     5677 2023-04-11 08:09:03.000000 ptapi42-1.0.3/ptapi42.egg-info/PKG-INFO
--rw-rw-r--   0 vitor     (1000) vitor     (1000)      234 2023-04-11 08:09:03.000000 ptapi42-1.0.3/ptapi42.egg-info/SOURCES.txt
--rw-rw-r--   0 vitor     (1000) vitor     (1000)        1 2023-04-11 08:09:03.000000 ptapi42-1.0.3/ptapi42.egg-info/dependency_links.txt
--rw-rw-r--   0 vitor     (1000) vitor     (1000)        8 2023-04-11 08:09:03.000000 ptapi42-1.0.3/ptapi42.egg-info/top_level.txt
--rw-rw-r--   0 vitor     (1000) vitor     (1000)      648 2023-04-11 08:07:51.000000 ptapi42-1.0.3/pyproject.toml
--rw-rw-r--   0 vitor     (1000) vitor     (1000)       38 2023-04-11 08:09:03.896004 ptapi42-1.0.3/setup.cfg
+drwxrwxr-x   0 vitor     (1000) vitor     (1000)        0 2023-05-23 09:46:15.880854 ptapi42-1.0.4/
+-rw-rw-r--   0 vitor     (1000) vitor     (1000)     1073 2023-04-11 08:06:49.000000 ptapi42-1.0.4/LICENSE
+-rw-rw-r--   0 vitor     (1000) vitor     (1000)     5677 2023-05-23 09:46:15.880854 ptapi42-1.0.4/PKG-INFO
+-rw-rw-r--   0 vitor     (1000) vitor     (1000)     3865 2023-04-11 08:06:49.000000 ptapi42-1.0.4/README.md
+drwxrwxr-x   0 vitor     (1000) vitor     (1000)        0 2023-05-23 09:46:15.876854 ptapi42-1.0.4/ptapi42/
+-rw-rw-r--   0 vitor     (1000) vitor     (1000)       39 2023-04-11 08:06:49.000000 ptapi42-1.0.4/ptapi42/__init__.py
+-rw-rw-r--   0 vitor     (1000) vitor     (1000)    26764 2023-05-23 09:41:21.000000 ptapi42-1.0.4/ptapi42/api42.py
+-rw-rw-r--   0 vitor     (1000) vitor     (1000)     3210 2023-04-11 08:06:49.000000 ptapi42-1.0.4/ptapi42/api42_token.py
+-rw-rw-r--   0 vitor     (1000) vitor     (1000)     1372 2023-04-11 08:06:49.000000 ptapi42-1.0.4/ptapi42/config.py
+drwxrwxr-x   0 vitor     (1000) vitor     (1000)        0 2023-05-23 09:46:15.876854 ptapi42-1.0.4/ptapi42.egg-info/
+-rw-rw-r--   0 vitor     (1000) vitor     (1000)     5677 2023-05-23 09:46:15.000000 ptapi42-1.0.4/ptapi42.egg-info/PKG-INFO
+-rw-rw-r--   0 vitor     (1000) vitor     (1000)      234 2023-05-23 09:46:15.000000 ptapi42-1.0.4/ptapi42.egg-info/SOURCES.txt
+-rw-rw-r--   0 vitor     (1000) vitor     (1000)        1 2023-05-23 09:46:15.000000 ptapi42-1.0.4/ptapi42.egg-info/dependency_links.txt
+-rw-rw-r--   0 vitor     (1000) vitor     (1000)        8 2023-05-23 09:46:15.000000 ptapi42-1.0.4/ptapi42.egg-info/top_level.txt
+-rw-rw-r--   0 vitor     (1000) vitor     (1000)      648 2023-05-23 09:43:12.000000 ptapi42-1.0.4/pyproject.toml
+-rw-rw-r--   0 vitor     (1000) vitor     (1000)       38 2023-05-23 09:46:15.880854 ptapi42-1.0.4/setup.cfg
```

### Comparing `ptapi42-1.0.3/LICENSE` & `ptapi42-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ptapi42-1.0.3/PKG-INFO` & `ptapi42-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptapi42
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python package that simplifies the process of making API requests to 42's API.
 Author: 42 Portugal
 Author-email: root@42porto.com
 License: MIT License
         
         Copyright (c) 2023 Maria Sottomayor
```

### Comparing `ptapi42-1.0.3/README.md` & `ptapi42-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ptapi42-1.0.3/ptapi42/api42.py` & `ptapi42-1.0.4/ptapi42/api42.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,18 +284,22 @@
             except requests.exceptions.HTTPError as e:
                 # Log the error and optionally raise an exception
                 self.__log.error(
                     f'{request} {resp.status_code}: {resp.reason}'
                     f'\n\tHeaders: {resp.headers}'
                     f'\n\tContent: {resp.content or {}}'
                 )
+
                 if self.__raises:
-                    raise Api42RequestError(
-                        f'{request}: {e}'
-                    ) from e
+                    raise Api42RequestError({
+                            'request': request,
+                            'status_code': resp.status_code,
+                            'reason': resp.reason,
+                            'content': resp.content
+                        }) from e
 
             # Log the successful request
             self.__log.debug(f'{request} {resp.status_code}: {resp.reason}')
 
             # return the request in json format if possible else return content
             try:
                 return resp.json()
@@ -343,15 +347,20 @@
             # Log the error and optionally raise an exception
             self.__log.error(
                 f'GET {resp.url} {resp.status_code}: {resp.reason}'
                 f'\n\tHeaders: {resp.headers}'
                 f'\n\tContent: {resp.content or {}}'
             )
             if self.__raises:
-                raise Api42RequestError(f'Failed: {e}') from e
+                raise Api42RequestError({
+                        'request': resp.url,
+                        'status_code': resp.status_code,
+                        'reason': resp.reason,
+                        'content': resp.content
+                    }) from e
             return []
 
         # Log the successful request
         self.__log.debug(f'GET {resp.url} {resp.status_code}: {resp.reason}')
 
         # Extract the response content as JSON
         results: list = resp.json()
@@ -605,15 +614,20 @@
                 # Log the error and optionally raise an exception
                 self.__log.error(
                     f'{req} {resp.status_code}: {resp.reason}'
                     f'\n\tHeaders: {resp.headers}'
                     f'\n\tContent: {resp.content or {}}'
                 )
                 if self.__raises:
-                    raise Api42RequestError(f'{req}: {e}') from e
+                    raise Api42RequestError({
+                            'request': req,
+                            'status_code': resp.status_code,
+                            'reason': resp.reason,
+                            'content': resp.content
+                        }) from e
             # Log the successful request
             self.__log.debug(f'{req} {resp.status_code}: {resp.reason}')
 
             # return the request in json format if possible else return content
             try:
                 return resp.json()
             except requests.exceptions.JSONDecodeError:
```

### Comparing `ptapi42-1.0.3/ptapi42/api42_token.py` & `ptapi42-1.0.4/ptapi42/api42_token.py`

 * *Files identical despite different names*

### Comparing `ptapi42-1.0.3/ptapi42/config.py` & `ptapi42-1.0.4/ptapi42/config.py`

 * *Files identical despite different names*

### Comparing `ptapi42-1.0.3/ptapi42.egg-info/PKG-INFO` & `ptapi42-1.0.4/ptapi42.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptapi42
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python package that simplifies the process of making API requests to 42's API.
 Author: 42 Portugal
 Author-email: root@42porto.com
 License: MIT License
         
         Copyright (c) 2023 Maria Sottomayor
```

### Comparing `ptapi42-1.0.3/pyproject.toml` & `ptapi42-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]  # PEP 508 specifications.
 
 [project]
 name = "ptapi42"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   {name="42 Portugal"},
   {email="root@42porto.com"},
 ]
 description = "A python package that simplifies the process of making API requests to 42's API."
 readme = "README.md"
 requires-python = ">=3.10"
```

