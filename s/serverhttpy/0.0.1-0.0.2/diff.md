# Comparing `tmp/serverhttpy-0.0.1.tar.gz` & `tmp/serverhttpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serverhttpy-0.0.1.tar", last modified: Thu May 18 22:15:32 2023, max compression
+gzip compressed data, was "serverhttpy-0.0.2.tar", last modified: Tue May 23 21:47:43 2023, max compression
```

## Comparing `serverhttpy-0.0.1.tar` & `serverhttpy-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:15:32.314177 serverhttpy-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-18 22:15:32.314177 serverhttpy-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:15:32.314177 serverhttpy-0.0.1/serverhttpy/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/serverhttpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/serverhttpy/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:15:32.314177 serverhttpy-0.0.1/serverhttpy/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/serverhttpy/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/serverhttpy/enums/http_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/serverhttpy/enums/status_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:15:32.314177 serverhttpy-0.0.1/serverhttpy/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/serverhttpy/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/serverhttpy/exceptions/invalid_header_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/serverhttpy/exceptions/invalid_path_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/serverhttpy/exceptions/invalid_query_param_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/serverhttpy/exceptions/invalid_request_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/serverhttpy/exceptions/no_action_registered_in_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/serverhttpy/exceptions/unsupported_method_specified.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:15:32.314177 serverhttpy-0.0.1/serverhttpy/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/serverhttpy/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/serverhttpy/models/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/serverhttpy/models/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/serverhttpy/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/serverhttpy/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/serverhttpy/models/uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/serverhttpy/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:15:32.314177 serverhttpy-0.0.1/serverhttpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-18 22:15:32.000000 serverhttpy-0.0.1/serverhttpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-18 22:15:32.000000 serverhttpy-0.0.1/serverhttpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 22:15:32.000000 serverhttpy-0.0.1/serverhttpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 22:15:32.000000 serverhttpy-0.0.1/serverhttpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 22:15:32.314177 serverhttpy-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-18 22:15:23.000000 serverhttpy-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:47:43.397045 serverhttpy-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-23 21:47:43.397045 serverhttpy-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:47:43.393045 serverhttpy-0.0.2/serverhttpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:47:43.393045 serverhttpy-0.0.2/serverhttpy/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/enums/http_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/enums/status_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:47:43.393045 serverhttpy-0.0.2/serverhttpy/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/examples/example_clients_managment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/examples/sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:47:43.397045 serverhttpy-0.0.2/serverhttpy/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/exceptions/invalid_header_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/exceptions/invalid_path_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/exceptions/invalid_query_param_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/exceptions/invalid_request_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/exceptions/no_action_registered_in_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/exceptions/unsupported_method_specified.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:47:43.397045 serverhttpy-0.0.2/serverhttpy/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/models/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/models/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/models/uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/serverhttpy/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:47:43.393045 serverhttpy-0.0.2/serverhttpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-23 21:47:43.000000 serverhttpy-0.0.2/serverhttpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-23 21:47:43.000000 serverhttpy-0.0.2/serverhttpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:47:43.000000 serverhttpy-0.0.2/serverhttpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 21:47:43.000000 serverhttpy-0.0.2/serverhttpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 21:47:43.397045 serverhttpy-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-23 21:47:32.000000 serverhttpy-0.0.2/setup.py
```

### Comparing `serverhttpy-0.0.1/serverhttpy/enums/status_code.py` & `serverhttpy-0.0.2/serverhttpy/enums/status_code.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,14 +7,14 @@
     NotFound = 404
     MethodNotAllowed = 405
     InternalServerError = 500
     NotImplemented = 501
 
     def description(self):
         return {
-            StatusCode.OK: 'OK',
-            StatusCode.BadRequest: 'Bad Request',
-            StatusCode.NotFound: 'Not Found',
-            StatusCode.MethodNotAllowed: 'Method Not Allowed',
-            StatusCode.InternalServerError: 'Internal Server Error',
-            StatusCode.NotImplemented: 'Not Implemented'
+            StatusCode.OK: "OK",
+            StatusCode.BadRequest: "Bad Request",
+            StatusCode.NotFound: "Not Found",
+            StatusCode.MethodNotAllowed: "Method Not Allowed",
+            StatusCode.InternalServerError: "Internal Server Error",
+            StatusCode.NotImplemented: "Not Implemented",
         }[self]
```

### Comparing `serverhttpy-0.0.1/serverhttpy/models/endpoint.py` & `serverhttpy-0.0.2/serverhttpy/models/endpoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 from typing import Callable
 
 from serverhttpy.enums.http_method import HTTPMethod
-from serverhttpy.exceptions.no_action_registered_in_endpoint import NoActionRegisteredInEndpointException
+from serverhttpy.exceptions.no_action_registered_in_endpoint import (
+    NoActionRegisteredInEndpointException,
+)
 from serverhttpy.models.path import Path
 from serverhttpy.models.request import Request
 from serverhttpy.models.response import Response
 
 
 class Endpoint:
     path: Path
     http_method: HTTPMethod
     action: Callable[[Request], Response]
 
-    def __init__(self, path: Path, http_method: HTTPMethod, action: Callable[[Request], Response] = None):
+    def __init__(
+        self,
+        path: Path,
+        http_method: HTTPMethod,
+        action: Callable[[Request], Response] = None,
+    ):
         self.path = path
         self.http_method = http_method
         self.action = action
 
     def __eq__(self, other):
-        return isinstance(other, Endpoint) and self.path == other.path and self.http_method == other.http_method
+        return (
+            isinstance(other, Endpoint)
+            and self.path == other.path
+            and self.http_method == other.http_method
+        )
 
     def __hash__(self):
         return hash(repr(self))
 
     def __repr__(self):
-        return f'{self.http_method} {self.path}'
+        return f"{self.http_method} {self.path}"
 
     def execute(self, request: Request):
         if self.action is None:
             raise NoActionRegisteredInEndpointException(repr(Endpoint))
         return self.action(request)
```

### Comparing `serverhttpy-0.0.1/serverhttpy/models/request.py` & `serverhttpy-0.0.2/serverhttpy/models/request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 from serverhttpy.enums.http_method import HTTPMethod
-from serverhttpy.exceptions.invalid_header_structure import InvalidHeaderStructureException
-from serverhttpy.exceptions.unsupported_method_specified import UnsupportedMethodSpecifiedException
+from serverhttpy.exceptions.invalid_header_structure import (
+    InvalidHeaderStructureException,
+)
+from serverhttpy.exceptions.unsupported_method_specified import (
+    UnsupportedMethodSpecifiedException,
+)
 from serverhttpy.models.uri import URI
 
 
 class Request:
     method: HTTPMethod
     protocol: str
     headers: dict
     uri: URI
     body: str
+    request_arguments: dict
 
     def __str__(self):
-        return f'{self.method.value} {self.uri} {self.protocol}'
+        return f"{self.method.value} {self.uri} {self.protocol}"
 
     def __init__(self, request_string: str):
         request_lines = request_string.splitlines()
 
         if len(request_lines) == 0:
-            raise InvalidHeaderStructureException('Header does not exist')
+            raise InvalidHeaderStructureException("Header does not exist")
 
         header_row = request_lines[0]
-        header_row_words = header_row.split(' ')
+        header_row_words = header_row.split(" ")
 
         if len(header_row_words) != 3:
             raise InvalidHeaderStructureException(header_row)
 
         try:
             self.method = HTTPMethod(header_row_words[0])
         except ValueError:
@@ -33,22 +38,22 @@
 
         self.uri = URI(header_row_words[1])
         self.protocol = header_row_words[2]
 
         self.headers = dict()
         index = 1
         for index in range(1, len(request_lines)):
-            if request_lines[index] == '':
+            if request_lines[index] == "":
                 break
 
-            header = request_lines[index].split(': ')
+            header = request_lines[index].split(": ")
 
             if len(header) != 2:
                 raise InvalidHeaderStructureException(header)
 
             self.headers[header[0]] = header[1]
 
-        self.body = ''
+        self.body = ""
         for body_index in range(index + 1, len(request_lines)):
             self.body += request_lines[body_index]
             if body_index < len(request_lines) - 1:
-                self.body += '\n'
+                self.body += "\n"
```

### Comparing `serverhttpy-0.0.1/serverhttpy/models/response.py` & `serverhttpy-0.0.2/serverhttpy/models/response.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,31 @@
 class Response:
     status_code: StatusCode
     protocol: str
     headers: dict
     body: str
 
     def __str__(self):
-        return f'{self.protocol} {self.status_code.value} {self.status_code.description()}'
+        return (
+            f"{self.protocol} {self.status_code.value} {self.status_code.description()}"
+        )
 
     def __repr__(self):
         base = self.__str__()
 
         if self.headers is not None:
             for index, header in enumerate(self.headers):
                 if index == 0:
-                    base += '\n'
-                base += f'{header}: {self.headers[header]}'
+                    base += "\n"
+                base += f"{header}: {self.headers[header]}"
                 if index <= len(self.headers) - 1:
-                    base += '\n'
+                    base += "\n"
 
         if self.body is not None and len(self.body) > 0:
-            base += '\n'
+            base += "\n"
             base += self.body
 
         return base
 
     def __init__(self, status_code: StatusCode, headers: dict = None, body: str = None):
         self.status_code = status_code
         self.protocol = supported_protocol
```

### Comparing `serverhttpy-0.0.1/serverhttpy/models/uri.py` & `serverhttpy-0.0.2/serverhttpy/models/uri.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 from serverhttpy.exceptions.invalid_path_structure import InvalidPathStructureException
-from serverhttpy.exceptions.invalid_query_param_structure import InvalidQueryParamStructureException
+from serverhttpy.exceptions.invalid_query_param_structure import (
+    InvalidQueryParamStructureException,
+)
 from serverhttpy.models.path import Path
 
 
 class URI:
     path: Path
     query_params: dict
 
     def __str__(self):
-        base = f'{self.path}'
+        base = f"{self.path}"
         if len(self.query_params) > 0:
-            base += '?'
+            base += "?"
             for index, param in enumerate(self.query_params):
-                base += f'{param}={self.query_params[param]}'
+                base += f"{param}={self.query_params[param]}"
                 if index < len(self.query_params) - 1:
-                    base += '&'
+                    base += "&"
         return base
 
     def __init__(self, path_string: str):
-        path_elems = path_string.split('?')
+        path_elems = path_string.split("?")
 
         if 1 > len(path_elems) > 2:
             raise InvalidPathStructureException(path_string)
 
         self.path = Path(path_elems[0])
         self.query_params = dict()
 
         if len(path_elems) > 1:
-            query_params = path_elems[1].split('&')
+            query_params = path_elems[1].split("&")
             for param in query_params:
-                key_value = param.split('=')
+                key_value = param.split("=")
 
                 if len(key_value) != 2:
                     raise InvalidQueryParamStructureException(param)
 
                 self.query_params[key_value[0]] = key_value[1]
-
```

### Comparing `serverhttpy-0.0.1/serverhttpy.egg-info/SOURCES.txt` & `serverhttpy-0.0.2/serverhttpy.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 serverhttpy.egg-info/PKG-INFO
 serverhttpy.egg-info/SOURCES.txt
 serverhttpy.egg-info/dependency_links.txt
 serverhttpy.egg-info/top_level.txt
 serverhttpy/enums/__init__.py
 serverhttpy/enums/http_method.py
 serverhttpy/enums/status_code.py
+serverhttpy/examples/example_clients_managment.py
+serverhttpy/examples/sample_data.py
 serverhttpy/exceptions/__init__.py
 serverhttpy/exceptions/invalid_header_structure.py
 serverhttpy/exceptions/invalid_path_structure.py
 serverhttpy/exceptions/invalid_query_param_structure.py
 serverhttpy/exceptions/invalid_request_structure.py
 serverhttpy/exceptions/no_action_registered_in_endpoint.py
 serverhttpy/exceptions/unsupported_method_specified.py
```

