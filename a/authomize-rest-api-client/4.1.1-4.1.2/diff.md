# Comparing `tmp/authomize-rest-api-client-4.1.1.tar.gz` & `tmp/authomize-rest-api-client-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-4.1.1.tar", last modified: Tue May 23 02:31:24 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-4.1.2.tar", last modified: Tue May 23 14:31:43 2023, max compression
```

## Comparing `authomize-rest-api-client-4.1.1.tar` & `authomize-rest-api-client-4.1.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:31:24.447895 authomize-rest-api-client-4.1.1/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-05-23 02:31:24.447895 authomize-rest-api-client-4.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2160 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:31:24.443895 authomize-rest-api-client-4.1.1/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:31:24.447895 authomize-rest-api-client-4.1.1/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:31:24.447895 authomize-rest-api-client-4.1.1/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2925 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10105 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    12633 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:31:24.447895 authomize-rest-api-client-4.1.1/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:31:24.447895 authomize-rest-api-client-4.1.1/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:31:24.447895 authomize-rest-api-client-4.1.1/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    73614 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:31:24.447895 authomize-rest-api-client-4.1.1/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35822 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:31:24.447895 authomize-rest-api-client-4.1.1/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:31:24.447895 authomize-rest-api-client-4.1.1/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   185721 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:31:24.447895 authomize-rest-api-client-4.1.1/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89185 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-23 02:31:04.000000 authomize-rest-api-client-4.1.1/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:31:24.447895 authomize-rest-api-client-4.1.1/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-05-23 02:31:24.000000 authomize-rest-api-client-4.1.1/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-05-23 02:31:24.000000 authomize-rest-api-client-4.1.1/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:31:24.000000 authomize-rest-api-client-4.1.1/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-23 02:31:24.000000 authomize-rest-api-client-4.1.1/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-23 02:31:24.000000 authomize-rest-api-client-4.1.1/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-05-23 02:31:24.447895 authomize-rest-api-client-4.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-23 02:31:08.000000 authomize-rest-api-client-4.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2194 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2538 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10358 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    13027 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75246 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35822 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   189364 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89185 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-05-23 14:31:43.000000 authomize-rest-api-client-4.1.2/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-05-23 14:31:43.000000 authomize-rest-api-client-4.1.2/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 14:31:43.000000 authomize-rest-api-client-4.1.2/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-23 14:31:43.000000 authomize-rest-api-client-4.1.2/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-23 14:31:43.000000 authomize-rest-api-client-4.1.2/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-05-23 14:31:27.000000 authomize-rest-api-client-4.1.2/setup.py
```

### Comparing `authomize-rest-api-client-4.1.1/LICENSE.txt` & `authomize-rest-api-client-4.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.1/README.md` & `authomize-rest-api-client-4.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,17 @@
 
 for connectors-rest-api:
 ```
 curl --socks5-hostname 127.0.0.1:1337 http://connectors-rest-api.application.svc:8080/openapi-extended.json | jq --indent 2 . > authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
 ```
 ```
 pip install -e .[codegen]
-datamodel-codegen --use-default-kwarg --input authomize/rest_api_client/openapi/connectors_rest_api/openapi.json --output authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+datamodel-codegen --use-default-kwarg --encoding=utf-8 --input authomize/rest_api_client/openapi/connectors_rest_api/openapi.json --output authomize/rest_api_client/generated/connectors_rest_api/schemas.py
 ```
 
 for external-rest-api:
 ```
 curl https://apidev.authomize.com/openapi-platform.json | jq --indent 2 . > authomize/rest_api_client/openapi/external_rest_api/openapi.json
 ```
 ```
-datamodel-codegen --use-default-kwarg --input authomize/rest_api_client/openapi/external_rest_api/openapi.json --output authomize/rest_api_client/generated/external_rest_api/schemas.py
+datamodel-codegen --use-default-kwarg --encoding=utf-8 --input authomize/rest_api_client/openapi/external_rest_api/openapi.json --output authomize/rest_api_client/generated/external_rest_api/schemas.py
 ```
```

### Comparing `authomize-rest-api-client-4.1.1/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-4.1.2/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.1/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-4.1.2/authomize/rest_api_client/client/base_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,14 +19,29 @@
         self.session.headers.update({'Authorization': self.authorization_header})
 
     @property
     def authorization_header(self) -> str:
         raise NotImplementedError()
 
     @staticmethod
+    def _handle_response(response: Response):
+        if response.ok:
+            return BaseClient._handle_ok_response(response)
+        try:
+            response_json = response.json()
+            detail = response_json.get('detail')
+            if 400 <= response.status_code < 500:
+                response.reason = response.text
+        except Exception:
+            detail = None
+        if detail:
+            raise ClientError(str(detail))
+        response.raise_for_status()
+
+    @staticmethod
     def _handle_ok_response(response: Response) -> dict:
         if content_type := response.headers.get('content-type'):
             if content_type.startswith('application/json'):
                 return response.json()
 
         raise ClientError(
             message={
@@ -36,55 +51,31 @@
                 'raw': response.content,
             }
         )
 
     def http_get(self, url, params=None):
         url = self.base_url + url
         response = self.session.get(url, params=params)
-        if response.ok:
-            return self._handle_ok_response(response)
-        try:
-            response_json = response.json()
-            detail = response_json.get('detail')
-            if 400 <= response.status_code < 500:
-                response.reason = response.text
-        except Exception:
-            detail = None
-        if detail:
-            raise ClientError(str(detail))
-        response.raise_for_status()
+        self._handle_response(response)
 
     def http_post(self, url: str, body: Optional[str] = None):
         url = self.base_url + url
         response = self.session.post(
             url,
             headers={'Content-Type': 'application/json'},
             data=body,
         )
-        if response.ok:
-            return self._handle_ok_response(response)
-        try:
-            response_json = response.json()
-            detail = response_json.get('detail')
-            if 400 <= response.status_code < 500:
-                response.reason = response.text
-        except Exception:
-            detail = None
-        if detail:
-            raise ClientError(str(detail))
-        response.raise_for_status()
+        self._handle_response(response)
+
+    def http_patch(self, url: str, body: Optional[str] = None):
+        url = self.base_url + url
+        response = self.session.patch(
+            url,
+            headers={'Content-Type': 'application/json'},
+            data=body,
+        )
+        self._handle_response(response)
 
     def http_delete(self, url: str, params=None):
         url = self.base_url + url
         response = self.session.delete(url, params=params)
-        if response.ok:
-            return self._handle_ok_response(response)
-        try:
-            response_json = response.json()
-            detail = response_json.get('detail')
-            if 400 <= response.status_code < 500:
-                response.reason = response.text
-        except Exception:
-            detail = None
-        if detail:
-            raise ClientError(str(detail))
-        response.raise_for_status()
+        self._handle_response(response)
```

### Comparing `authomize-rest-api-client-4.1.1/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-4.1.2/authomize/rest_api_client/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     SearchGroupingsAssociationsListResponseSchema,
     SearchIdentitiesListResponseSchema,
     SearchPermissionResponseSchema,
     SearchPrivilegeGrantsListResponseSchema,
     SearchPrivilegesListResponseSchema,
     SearchUsersListResponseSchema,
     SubmitResponse,
+    UpdateAppSchema,
 )
 from authomize.rest_api_client.generated.external_rest_api.schemas import (
     IncidentExpansion,
     IsAliveResponse,
     MeResponse,
 )
 
@@ -133,14 +134,24 @@
         modified_before: Optional[datetime] = None,
     ) -> SubmitResponse:
         return self.connectors_client.delete_app_data(
             app_id=app_id,
             modified_before=modified_before,
         )
 
+    def update_app_data(
+        self,
+        app_id: str,
+        body: UpdateAppSchema,
+    ) -> SubmitResponse:
+        return self.connectors_client.update_app_data(
+            app_id=app_id,
+            body=body,
+        )
+
     def search_users(
         self,
         app_id: str,
         start_date: Optional[datetime] = None,
     ) -> SearchUsersListResponseSchema:
         return self.connectors_client.search_users(
             app_id=app_id,
```

### Comparing `authomize-rest-api-client-4.1.1/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-4.1.2/authomize/rest_api_client/client/connectors_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     SearchGroupingsAssociationsListResponseSchema,
     SearchIdentitiesListResponseSchema,
     SearchPermissionResponseSchema,
     SearchPrivilegeGrantsListResponseSchema,
     SearchPrivilegesListResponseSchema,
     SearchUsersListResponseSchema,
     SubmitResponse,
+    UpdateAppSchema,
 )
 
 
 class ConnectorsClient(BaseClient):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -110,14 +111,29 @@
         if not app_id:
             raise ValueError('Missing app_id')
         date_filter = ''
         if modified_before:
             date_filter = f'?modifiedBefore={str(modified_before)}'
         return self.http_delete(url=f"/v2/apps/{app_id}/data{date_filter}")
 
+    def update_app_data(
+        self,
+        app_id: str,
+        body: UpdateAppSchema,
+    ) -> SubmitResponse:
+        if not app_id:
+            raise ValueError('Missing app_id')
+        return self.http_patch(
+            url=f"/v2/apps/{app_id}",
+            body=json.dumps(
+                body,
+                default=pydantic_encoder
+            )
+        )
+
     def search_users(
         self,
         app_id: str,
         start_date: Optional[datetime] = None,
     ) -> SearchUsersListResponseSchema:
         if not app_id:
             raise ValueError('Missing app_id')
```

### Comparing `authomize-rest-api-client-4.1.1/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-4.1.2/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.1/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-4.1.2/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-04-30T09:35:02+00:00
+#   timestamp: 2023-05-23T14:21:16+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
@@ -555,15 +555,15 @@
 class NewGroupingsListRequestSchema(BaseModel):
     data: List[NewGroupingRequestSchema] = Field(
         ..., description='New Groupings', max_items=10000, min_items=1, title='Data'
     )
     validateOnly: Optional[bool] = Field(
         default=False,
         description='Validate the request without uploading the data into the system.',
-        title='Validateonly',
+        title='Validate Only\n',
     )
 
 
 class NewIdentityResponseSchema(BaseModel):
     acceptedTimestamp: Optional[datetime] = Field(
         default=None,
         description='**The accepted time of the request**',
@@ -839,14 +839,20 @@
     Failed = 'Failed'
     Ingest = 'Ingest'
     IngestChunk = 'IngestChunk'
     PostProcess = 'PostProcess'
     Queue = 'Queue'
 
 
+class UpdateAppSchema(BaseModel):
+    name: Optional[str] = Field(
+        default=None, description='The name of the Application.\n', title='Name'
+    )
+
+
 class UpdateAssetRequestSchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
         ..., description='Asset ID. **Mandatory, must be unique.**\n', title='Uniqueid'
     )
     originId: Optional[constr(min_length=1)] = Field(
         default=None,
         description="The asset ID in the source system.\nAs opposed to `uniqueId`, it's not mandatory and can be non-unique\n",
@@ -1012,14 +1018,15 @@
     accessType: AccessTypes
     accessName: Optional[str] = Field(default=None, title='Accessname')
 
 
 class AssetDescription(BaseModel):
     id: str = Field(..., title='Id')
     name: str = Field(..., title='Name')
+    customName: Optional[str] = Field(default=None, title='Customname')
     type: AssetTypes
     description: Optional[str] = Field(default=None, title='Description')
     logoUrl: Optional[str] = Field(default=None, title='Logourl')
     href: Optional[str] = Field(default=None, title='Href')
     createdAt: Optional[datetime] = Field(default=None, title='Createdat')
     isAuxiliary: Optional[bool] = Field(default=None, title='Isauxiliary')
     service: Optional[str] = Field(default=None, title='Service')
@@ -1357,24 +1364,29 @@
         default=False,
         description='If `true`, the permissions represent the role in the source application.\nThe default is `false`.\n',
         title='Isrole',
     )
     tags: Optional[List[constr(min_length=1)]] = Field(
         default=None, description='Tags on access permissions.\n', title='Tags'
     )
+    escalationPathPossible: Optional[bool] = Field(
+        default=False,
+        description="If `true`, it's possible to perform a privilege escalation using the permission.   \nexample: User has Read access to a secret containing credentials of another user.  This allows \nprivilege escalation.\nopposite example: User has Read metadata permission to a secret containing credentials of another user. This *Does NOT* allows \nprivilege escalation.\n\n",
+        title='Escalationpathpossible',
+    )
 
 
 class NewPermissionsListRequestSchema(BaseModel):
     data: List[NewPermissionRequestSchema] = Field(
         ..., description='New Permissions', max_items=10000, min_items=1, title='Data'
     )
     validateOnly: Optional[bool] = Field(
         default=False,
         description='Validate the request without uploading the data into the system.',
-        title='Validateonly',
+        title='Validate Only\n',
     )
 
 
 class NewPrivilegeRequestSchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
         ...,
         description='Privilege ID.\n\nIf not defined, set as originName. **Mandatory, must be unique.**\n',
@@ -1494,14 +1506,19 @@
         default=False,
         description='If `true`, the permissions represent the role in the source application.\nThe default is `false`.\n',
         title='Isrole',
     )
     tags: Optional[List[constr(min_length=1)]] = Field(
         default=None, description='Tags on access permissions.\n', title='Tags'
     )
+    escalationPathPossible: Optional[bool] = Field(
+        default=False,
+        description="If `true`, it's possible to perform a privilege escalation using the permission.   \nexample: User has Read access to a secret containing credentials of another user.  This allows \nprivilege escalation.\nopposite example: User has Read metadata permission to a secret containing credentials of another user. This *Does NOT* allows \nprivilege escalation.\n\n",
+        title='Escalationpathpossible',
+    )
 
 
 class PrivilegeSchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
         ...,
         description='Privilege ID.\n\nIf not defined, set as originName. **Mandatory, must be unique.**\n',
         title='Uniqueid',
@@ -1537,15 +1554,15 @@
     new_groupings: Optional[List[NewGroupingRequestSchema]] = Field(
         default=None,
         description='The Create Groupings API is used to create groups that have access to a particular app.',
         title='New Groupings',
     )
     new_permissions: Optional[List[NewPermissionRequestSchema]] = Field(
         default=None,
-        description='The Create Permissions API is used to create a set of privileges, assigned to a specific target.\nA permission (also referred to as an “entitlement”) is a set of privileges, assigned to a specific target. \nExamples include: file permissions, file shares, GCP entitlements, the actual policies assigning access to roles in AWS, and inline policies.',
+        description='The Create Permissions API is used to create a set of privileges, assigned to a specific target.\nA permission (also referred to as an "entitlement") is a set of privileges, assigned to a specific target. \nExamples include: file permissions, file shares, GCP entitlements, the actual policies assigning access to roles in AWS, and inline policies.\n',
         title='New Permissions',
     )
     new_privileges: Optional[List[NewPrivilegeRequestSchema]] = Field(
         default=None,
         description='The Create Privileges API is used to define privileges that can be associated with assets.\nFor example, Read privileges on a file.\nHere you can define the type of privileges and associate it to assets in the Permission API.\n',
         title='New Privileges',
     )
@@ -1579,14 +1596,19 @@
         title='New Assets Inheritance',
     )
     new_identities: Optional[List[NewIdentityRequestSchema]] = Field(
         default=None,
         description='The Create Identities API is used to create identities. \nThe data of the identity from this API is considered "the source of truth" and overrides the identity data from other systems.\n',
         title='New Identities',
     )
+    app: Optional[NewAssetRequestSchema] = Field(
+        default=None,
+        description='The Update Application Data API is used to update app data on `{appId}`.\n',
+        title='App',
+    )
 
 
 class RestApiConnectorListSchema(BaseModel):
     pagination: Pagination
     data: List[RestApiConnectorSchema] = Field(..., title='Data')
 
 
@@ -1809,15 +1831,15 @@
     new_groupings: Optional[List[NewGroupingRequestSchema]] = Field(
         default=None,
         description='The Create Groupings API is used to create groups that have access to a particular app.',
         title='New Groupings',
     )
     new_permissions: Optional[List[NewPermissionRequestSchema]] = Field(
         default=None,
-        description='The Create Permissions API is used to create a set of privileges, assigned to a specific target.\nA permission (also referred to as an “entitlement”) is a set of privileges, assigned to a specific target. \nExamples include: file permissions, file shares, GCP entitlements, the actual policies assigning access to roles in AWS, and inline policies.',
+        description='The Create Permissions API is used to create a set of privileges, assigned to a specific target.\nA permission (also referred to as an "entitlement") is a set of privileges, assigned to a specific target. \nExamples include: file permissions, file shares, GCP entitlements, the actual policies assigning access to roles in AWS, and inline policies.\n',
         title='New Permissions',
     )
     new_privileges: Optional[List[NewPrivilegeRequestSchema]] = Field(
         default=None,
         description='The Create Privileges API is used to define privileges that can be associated with assets.\nFor example, Read privileges on a file.\nHere you can define the type of privileges and associate it to assets in the Permission API.\n',
         title='New Privileges',
     )
@@ -1851,14 +1873,19 @@
         title='New Assets Inheritance',
     )
     new_identities: Optional[List[NewIdentityRequestSchema]] = Field(
         default=None,
         description='The Create Identities API is used to create identities. \nThe data of the identity from this API is considered "the source of truth" and overrides the identity data from other systems.\n',
         title='New Identities',
     )
+    app: Optional[NewAssetRequestSchema] = Field(
+        default=None,
+        description='The Update Application Data API is used to update app data on `{appId}`.\n',
+        title='App',
+    )
 
 
 class NewIdentitiesListRequestSchema(BaseModel):
     data: List[NewIdentityRequestSchema] = Field(
         ..., description='New Identities', max_items=10000, min_items=1, title='Data'
     )
     validateOnly: Optional[bool] = Field(
```

### Comparing `authomize-rest-api-client-4.1.1/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-4.1.2/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.1/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-4.1.2/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9830731405455104%*

 * *Differences: {"'components'": "{'schemas': {'AssetDescription': {'properties': {'customName': "*

 * *                 "OrderedDict([('title', 'Customname'), ('type', 'string')])}}, "*

 * *                 "'IngestionDataBundleSchema': {'properties': {'new_permissions': {'description': "*

 * *                 "'The Create Permissions API is used to create a set of privileges, assigned to a "*

 * *                 'specific target.\\nA permission (also referred to as an "entitlement") is a set '*

 * *                 'of privileges, assigned to a […]*

```diff
@@ -101,14 +101,18 @@
             "AssetDescription": {
                 "properties": {
                     "createdAt": {
                         "format": "date-time",
                         "title": "Createdat",
                         "type": "string"
                     },
+                    "customName": {
+                        "title": "Customname",
+                        "type": "string"
+                    },
                     "description": {
                         "title": "Description",
                         "type": "string"
                     },
                     "href": {
                         "title": "Href",
                         "type": "string"
@@ -823,14 +827,23 @@
                     "TaskPerformer",
                     "BusinessAccount"
                 ],
                 "title": "IdentityTypes"
             },
             "IngestionDataBundleSchema": {
                 "properties": {
+                    "app": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/NewAssetRequestSchema"
+                            }
+                        ],
+                        "description": "The Update Application Data API is used to update app data on `{appId}`.\n",
+                        "title": "App"
+                    },
                     "new_accounts_association": {
                         "description": "The Create Accounts Association API creates account associations between user accounts and groups.",
                         "items": {
                             "$ref": "#/components/schemas/NewAccountsAssociationRequestSchema"
                         },
                         "title": "New Accounts Association",
                         "type": "array"
@@ -872,15 +885,15 @@
                         "items": {
                             "$ref": "#/components/schemas/NewIdentityRequestSchema"
                         },
                         "title": "New Identities",
                         "type": "array"
                     },
                     "new_permissions": {
-                        "description": "The Create Permissions API is used to create a set of privileges, assigned to a specific target.\nA permission (also referred to as an \u201centitlement\u201d) is a set of privileges, assigned to a specific target. \nExamples include: file permissions, file shares, GCP entitlements, the actual policies assigning access to roles in AWS, and inline policies.",
+                        "description": "The Create Permissions API is used to create a set of privileges, assigned to a specific target.\nA permission (also referred to as an \"entitlement\") is a set of privileges, assigned to a specific target. \nExamples include: file permissions, file shares, GCP entitlements, the actual policies assigning access to roles in AWS, and inline policies.\n",
                         "items": {
                             "$ref": "#/components/schemas/NewPermissionRequestSchema"
                         },
                         "title": "New Permissions",
                         "type": "array"
                     },
                     "new_privileges": {
@@ -1684,15 +1697,15 @@
                         "minItems": 1,
                         "title": "Data",
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
-                        "title": "Validateonly",
+                        "title": "Validate Only\n",
                         "type": "boolean"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewGroupingsListRequestSchema",
@@ -1876,14 +1889,20 @@
                 "description": "New permission request schema",
                 "properties": {
                     "assetId": {
                         "description": "The ID of the asset.\n\nWhen `null`, this is a global permission on the entire application (not just locally).",
                         "title": "Assetid",
                         "type": "string"
                     },
+                    "escalationPathPossible": {
+                        "default": false,
+                        "description": "If `true`, it's possible to perform a privilege escalation using the permission.   \nexample: User has Read access to a secret containing credentials of another user.  This allows \nprivilege escalation.\nopposite example: User has Read metadata permission to a secret containing credentials of another user. This *Does NOT* allows \nprivilege escalation.\n\n",
+                        "title": "Escalationpathpossible",
+                        "type": "boolean"
+                    },
                     "isRole": {
                         "default": false,
                         "description": "If `true`, the permissions represent the role in the source application.\nThe default is `false`.\n",
                         "title": "Isrole",
                         "type": "boolean"
                     },
                     "privilegeId": {
@@ -1936,15 +1955,15 @@
                         "minItems": 1,
                         "title": "Data",
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
-                        "title": "Validateonly",
+                        "title": "Validate Only\n",
                         "type": "boolean"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewPermissionsListRequestSchema",
@@ -2485,14 +2504,20 @@
                 "description": "Permission schema",
                 "properties": {
                     "assetId": {
                         "description": "The ID of the asset.\n\nWhen `null`, this is a global permission on the entire application (not just locally).",
                         "title": "Assetid",
                         "type": "string"
                     },
+                    "escalationPathPossible": {
+                        "default": false,
+                        "description": "If `true`, it's possible to perform a privilege escalation using the permission.   \nexample: User has Read access to a secret containing credentials of another user.  This allows \nprivilege escalation.\nopposite example: User has Read metadata permission to a secret containing credentials of another user. This *Does NOT* allows \nprivilege escalation.\n\n",
+                        "title": "Escalationpathpossible",
+                        "type": "boolean"
+                    },
                     "isRole": {
                         "default": false,
                         "description": "If `true`, the permissions represent the role in the source application.\nThe default is `false`.\n",
                         "title": "Isrole",
                         "type": "boolean"
                     },
                     "privilegeId": {
@@ -2644,14 +2669,23 @@
                     "requestId"
                 ],
                 "title": "RequestSubmitResponse",
                 "type": "object"
             },
             "RequestsBundleSchema": {
                 "properties": {
+                    "app": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/NewAssetRequestSchema"
+                            }
+                        ],
+                        "description": "The Update Application Data API is used to update app data on `{appId}`.\n",
+                        "title": "App"
+                    },
                     "createdAt": {
                         "format": "date-time",
                         "title": "Createdat",
                         "type": "string"
                     },
                     "delete_app_data": {
                         "default": false,
@@ -2704,15 +2738,15 @@
                         "items": {
                             "$ref": "#/components/schemas/NewIdentityRequestSchema"
                         },
                         "title": "New Identities",
                         "type": "array"
                     },
                     "new_permissions": {
-                        "description": "The Create Permissions API is used to create a set of privileges, assigned to a specific target.\nA permission (also referred to as an \u201centitlement\u201d) is a set of privileges, assigned to a specific target. \nExamples include: file permissions, file shares, GCP entitlements, the actual policies assigning access to roles in AWS, and inline policies.",
+                        "description": "The Create Permissions API is used to create a set of privileges, assigned to a specific target.\nA permission (also referred to as an \"entitlement\") is a set of privileges, assigned to a specific target. \nExamples include: file permissions, file shares, GCP entitlements, the actual policies assigning access to roles in AWS, and inline policies.\n",
                         "items": {
                             "$ref": "#/components/schemas/NewPermissionRequestSchema"
                         },
                         "title": "New Permissions",
                         "type": "array"
                     },
                     "new_privileges": {
@@ -3070,14 +3104,25 @@
                     "Ingest",
                     "IngestChunk",
                     "PostProcess",
                     "Queue"
                 ],
                 "title": "TransactionStateType"
             },
+            "UpdateAppSchema": {
+                "properties": {
+                    "name": {
+                        "description": "The name of the Application.\n",
+                        "title": "Name",
+                        "type": "string"
+                    }
+                },
+                "title": "UpdateAppSchema",
+                "type": "object"
+            },
             "UpdateAssetRequestSchema": {
                 "description": "Update asset request schema",
                 "properties": {
                     "createdAt": {
                         "description": "The date (in ISO 8601 format) that the asset was created.\nThe default is `null`.\n",
                         "format": "date-time",
                         "title": "Createdat",
@@ -3719,15 +3764,15 @@
                 "type": "apiKey"
             }
         }
     },
     "info": {
         "description": "Authomize enables users to integrate your applications with Authomize via custom connectors.\n\nYou can use the APIs described in this document to create your connector.\n\nOnce data is uploaded and processed successfully, your custom connector will function in the same way as the connectors created by Authomize.\n\n## How does Authomize work?\nAuthomize works by gathering information about:\n\n\u00b7 individuals, teams and functions.\n\n\u00b7 apps, assets and accounts.\n\n\u00b7 all the relationships between them.\n\n![img.png](https://storagetry1.blob.core.windows.net/public/78d82650-71b0-4909-8444-022aab79add5.png)\n\n## Connector APIs\n\nAuthomize connector APIs enable pushing data into Authomize from external sources.\n\nThese APIs enable data extracted from outside applications (via application APIs) to be delivered to Authomize.\n\nA connector processes extracted application data to transform it into a format compatible with Authomize.\n\n![img_1.png](https://storagetry1.blob.core.windows.net/public/341bf6ef-2e5b-4284-b715-45105ffbf0f8.png)\n\n## Authentication\nTo Authenticate use the API Token, with the format: `Authorization: API_Token`.\n\nAn API Token is a token you provide when making API calls. \n\n\nThe API Token should be included in every request to the API in an `Authorization` header.\n```\ncurl -v -X POST \\n\n     -H \"Authorization: {API_Token}\" \\n\n     ...\n```\n\n## Limits\nRequests cannot exceed a size of 1MB.\n",
         "title": "Authomize API Reference",
-        "version": "3.1.6",
+        "version": "4.1.1",
         "x-logo": {
             "url": "https://static.authomize.com/public/icons/authomize-green.svg"
         }
     },
     "openapi": "3.0.2",
     "paths": {
         "/is_alive": {
@@ -4454,15 +4499,15 @@
                 "tags": [
                     "v1"
                 ]
             }
         },
         "/v2/apps/files/template": {
             "get": {
-                "description": "Download template file for file-provider based on REST API schema",
+                "description": "The Get File Template API downloads a template file for file-provider based on the REST API schema.",
                 "operationId": "get_file_template_v2_apps_files_template_get",
                 "responses": {
                     "200": {
                         "content": {
                             "application/json": {
                                 "schema": {}
                             }
@@ -4472,14 +4517,72 @@
                 },
                 "summary": "Get File Template",
                 "tags": [
                     "Apps"
                 ]
             }
         },
+        "/v2/apps/{appId}": {
+            "patch": {
+                "description": "The Update Application Data API is used to update app data on `{appId}`.\n",
+                "operationId": "update_application_data_v2_apps__appId__patch",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "appId",
+                        "required": true,
+                        "schema": {
+                            "title": "Appid",
+                            "type": "string"
+                        }
+                    }
+                ],
+                "requestBody": {
+                    "content": {
+                        "application/json": {
+                            "schema": {
+                                "$ref": "#/components/schemas/UpdateAppSchema"
+                            }
+                        }
+                    },
+                    "required": true
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/RequestSubmitResponse"
+                                }
+                            }
+                        },
+                        "description": "Successful Response"
+                    },
+                    "422": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/HTTPValidationError"
+                                }
+                            }
+                        },
+                        "description": "Validation Error"
+                    }
+                },
+                "security": [
+                    {
+                        "APIKeyHeader": []
+                    }
+                ],
+                "summary": "Update Application Data",
+                "tags": [
+                    "Apps"
+                ]
+            }
+        },
         "/v2/apps/{appId}/access/grouping": {
             "get": {
                 "description": "The Search Grouping API is used to get a list of groups that have access to a particular app.",
                 "operationId": "search_groupings_v2_apps__appId__access_grouping_get",
                 "parameters": [
                     {
                         "in": "path",
@@ -4646,15 +4749,15 @@
                 "tags": [
                     "Access"
                 ]
             }
         },
         "/v2/apps/{appId}/access/permissions": {
             "get": {
-                "description": "The Search Permissions API is used to list the privileges, assigned to a specific target.\nA permission (also referred to as an \u201centitlement\u201d) is a set of privileges, assigned to a specific target. \nExamples include: file permissions, file shares, GCP entitlements, the actual policies assigning access to roles in AWS, and inline policies. ",
+                "description": "The Search Permissions API is used to list the privileges, assigned to a specific target.\nA permission (also referred to as an \"entitlement\") is a set of privileges, assigned to a specific target. \nExamples include: file permissions, file shares, GCP entitlements, the actual policies assigning access to roles in AWS, and inline policies. \n",
                 "operationId": "search_permissions_v2_apps__appId__access_permissions_get",
                 "parameters": [
                     {
                         "in": "path",
                         "name": "appId",
                         "required": true,
                         "schema": {
@@ -4704,15 +4807,15 @@
                 ],
                 "summary": "Search Permissions",
                 "tags": [
                     "Access"
                 ]
             },
             "post": {
-                "description": "The Create Permissions API is used to create a set of privileges, assigned to a specific target.\nA permission (also referred to as an \u201centitlement\u201d) is a set of privileges, assigned to a specific target. \nExamples include: file permissions, file shares, GCP entitlements, the actual policies assigning access to roles in AWS, and inline policies.",
+                "description": "The Create Permissions API is used to create a set of privileges, assigned to a specific target.\nA permission (also referred to as an \"entitlement\") is a set of privileges, assigned to a specific target. \nExamples include: file permissions, file shares, GCP entitlements, the actual policies assigning access to roles in AWS, and inline policies.\n",
                 "operationId": "create_permissions_v2_apps__appId__access_permissions_post",
                 "parameters": [
                     {
                         "in": "path",
                         "name": "appId",
                         "required": true,
                         "schema": {
@@ -5468,15 +5571,15 @@
                         "schema": {
                             "title": "Appid",
                             "type": "string"
                         }
                     },
                     {
                         "description": "Delete all the app data lastly updated before the given date.",
-                        "example": "2023-04-30T09:34:20.489062+00:00",
+                        "example": "2023-05-23T09:23:41.791121+00:00",
                         "in": "query",
                         "name": "modifiedBefore",
                         "required": false,
                         "schema": {
                             "description": "Delete all the app data lastly updated before the given date.",
                             "format": "date-time",
                             "title": "Modifiedbefore",
```

### Comparing `authomize-rest-api-client-4.1.1/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-4.1.2/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.1/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-4.1.2/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.1/setup.py` & `authomize-rest-api-client-4.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='4.1.1',
+        version='4.1.2',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

