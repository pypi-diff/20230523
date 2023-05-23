# Comparing `tmp/aiokeepin-0.1.1.tar.gz` & `tmp/aiokeepin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiokeepin-0.1.1.tar", max compression
+gzip compressed data, was "aiokeepin-0.2.0.tar", max compression
```

## Comparing `aiokeepin-0.1.1.tar` & `aiokeepin-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2023-05-22 16:36:51.227873 aiokeepin-0.1.1/LICENSE
--rw-r--r--   0        0        0     2876 2023-05-22 16:37:38.305705 aiokeepin-0.1.1/README.md
--rw-r--r--   0        0        0       61 2023-05-11 15:06:34.887235 aiokeepin-0.1.1/aiokeepin/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 10:23:08.751590 aiokeepin-0.1.1/aiokeepin/adapters/__init__.py
--rw-r--r--   0        0        0     5925 2023-05-23 05:48:48.170073 aiokeepin-0.1.1/aiokeepin/adapters/base.py
--rw-r--r--   0        0        0       92 2023-05-22 07:00:50.261516 aiokeepin-0.1.1/aiokeepin/client.py
--rw-r--r--   0        0        0       69 2023-05-23 05:48:48.170073 aiokeepin-0.1.1/aiokeepin/exceptions/__init__.py
--rw-r--r--   0        0        0      288 2023-05-23 06:41:31.020732 aiokeepin-0.1.1/aiokeepin/exceptions/base.py
--rw-r--r--   0        0        0      607 2023-05-23 06:42:06.786322 aiokeepin-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3735 1970-01-01 00:00:00.000000 aiokeepin-0.1.1/setup.py
--rw-r--r--   0        0        0     3532 1970-01-01 00:00:00.000000 aiokeepin-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-22 16:36:51.227873 aiokeepin-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4104 2023-05-23 17:40:17.773751 aiokeepin-0.2.0/README.md
+-rw-r--r--   0        0        0       61 2023-05-11 15:06:34.887235 aiokeepin-0.2.0/aiokeepin/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 10:23:08.751590 aiokeepin-0.2.0/aiokeepin/adapters/__init__.py
+-rw-r--r--   0        0        0     6552 2023-05-23 15:51:06.238335 aiokeepin-0.2.0/aiokeepin/adapters/base.py
+-rw-r--r--   0        0        0       92 2023-05-22 07:00:50.261516 aiokeepin-0.2.0/aiokeepin/client.py
+-rw-r--r--   0        0        0      271 2023-05-23 15:51:06.051331 aiokeepin-0.2.0/aiokeepin/exceptions/__init__.py
+-rw-r--r--   0        0        0      798 2023-05-23 17:40:03.550505 aiokeepin-0.2.0/aiokeepin/exceptions/base.py
+-rw-r--r--   0        0        0      665 2023-05-23 17:51:22.878034 aiokeepin-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4979 1970-01-01 00:00:00.000000 aiokeepin-0.2.0/setup.py
+-rw-r--r--   0        0        0     4760 1970-01-01 00:00:00.000000 aiokeepin-0.2.0/PKG-INFO
```

### Comparing `aiokeepin-0.1.1/LICENSE` & `aiokeepin-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiokeepin-0.1.1/aiokeepin/adapters/base.py` & `aiokeepin-0.2.0/aiokeepin/adapters/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import logging
 from typing import Any, Dict, List, Optional
 
 from httpx import AsyncClient, HTTPStatusError, Response
 
-from aiokeepin.exceptions.base import KeepinStatusError
-
+from aiokeepin.exceptions.base import (
+    InternalServerError,
+    InvalidAPIKeyError,
+    KeepinStatusError,
+    NotFoundError,
+    ValidationError,
+)
 
 BASE_URL = "https://api.keepincrm.com/v1"
 logger = logging.getLogger(__name__)
 
 
 class BaseAdapter:
     def __init__(
@@ -53,15 +58,25 @@
             json=json,
             headers=headers,
         )
 
         try:
             response.raise_for_status()
         except HTTPStatusError as e:
-            raise KeepinStatusError(e.response.status_code) from e
+            status_code = e.response.status_code
+            response_data = e.response.text
+            if status_code == 401:
+                raise InvalidAPIKeyError(status_code, response_data) from e
+            if status_code == 422:
+                raise ValidationError(status_code, response_data) from e
+            if status_code == 404:
+                raise NotFoundError(status_code, response_data) from e
+            if status_code >= 500:
+                raise InternalServerError(status_code, response_data) from e
+            raise KeepinStatusError(status_code, response_data) from e
 
         return response
 
     async def post(
         self, path: str, json: Any, params: Optional[Dict[str, Any]] = None
     ) -> Dict[str, Any]:
         """
@@ -186,15 +201,15 @@
             Defaults to `None`.
         - `params` (Optional[Dict[str, Any]], optional): Query
             parameters. Defaults to `None`.
 
         ### Returns:
         - `List[Dict]`: List of items.
         """
-    
+
         items = []
 
         if not params:
             params = {}
 
         page = 1
         total_pages = 1
```

### Comparing `aiokeepin-0.1.1/setup.py` & `aiokeepin-0.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,145 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+# Async Python Wrapper for KeepinCRM API
 
-packages = \
-['aiokeepin', 'aiokeepin.adapters', 'aiokeepin.exceptions']
+This is an async Python wrapper for the KeepinCRM API that allows you to interact with the API using simple and convenient methods. The wrapper provides a `KeepinClient` class with async methods for making HTTP requests and retrieving data from the API.
 
-package_data = \
-{'': ['*']}
+## Installation
 
-install_requires = \
-['httpx>=0.24.0,<0.25.0']
-
-setup_kwargs = {
-    'name': 'aiokeepin',
-    'version': '0.1.1',
-    'description': 'Async python wrapper for KeepinCRM API',
-    'long_description': '# Async Python Wrapper for KeepinCRM API\n\nThis is an async Python wrapper for the KeepinCRM API that allows you to interact with the API using simple and convenient methods. The wrapper provides a `KeepinClient` class with async methods for making HTTP requests and retrieving data from the API.\n\n## Installation\n\nYou can install the library using pip:\n\n```shell\npip install aiokeepin\n```\n\n## Usage\n\nTo use the KeepinCRM async Python wrapper, import the `KeepinClient` class from the library:\n\n```python\nfrom aiokeepin import KeepinClient\n```\n\n### Initializing the Client\n\nCreate an instance of the `KeepinClient` class by providing your API key:\n\n```python\nclient = KeepinClient(api_key=\'YOUR_API_KEY\')\n```\n\n### Making API Requests\n\nThe `KeepinClient` instance provides async methods that correspond to the different HTTP request methods (`GET`, `POST`, `PATCH`, `PUT`, `DELETE`). Each method returns a dictionary containing the response from the API.\n\n#### GET Request Example\n\n```python\nresponse = await client.get(\'/clients\')\nprint(response)\n```\n\n#### POST Request Example\n\n```python\ndata = {\n  "email": "pib@example.com",\n  "company": "Назва чи ПІБ",\n  "lead": True,\n  "source_id": 5,\n  "status_id": 1,\n  "phones": [\n    "+380000000001"\n  ],\n  "tag_names": [\n    "VIP"\n  ],\n  "contacts_attributes": [\n    {\n      "fullname": "Прізвище Імʼя По батькові",\n      "phones": [\n        "+380000000002"\n      ],\n      "custom_fields": [\n        {\n          "name": "Посада",\n          "value": "Директор"\n        }\n      ]\n    }\n  ]\n}\n\nresponse = await client.post(\'/clients\', data=data)\nprint(response)\n```\n\n#### PATCH Request Example\n\n```python\ndata = {\n  "email": "new_email@example.com"\n}\n\nresponse = await client.patch(\'/clients/{client_id}\', data=data)\nprint(response)\n```\n\n#### PUT Request Example\n\n```python\ndata = {\n  "email": "updated_email@example.com"\n}\n\nresponse = await client.put(\'/clients/{client_id}\', data=data)\nprint(response)\n```\n\n#### DELETE Request Example\n\n```python\nresponse = await client.delete(\'/clients/{client_id}\')\nprint(response)\n```\n\n#### GET Paginated Items Example\n\n```python\nresponse = await client.get_paginated_items(\'/clients\')\n```\n\n## Error Handling\n\nIn case of an error response from the API, an exception will be raised. You can handle exceptions using try-except blocks. Here\'s an example:\n\n```python\nfrom aiokeepin.exceptions import KeepinStatusError\n\ntry:\n    response = await client.get(\'/nonexistent_endpoint\')\nexcept KeepinStatusError as e:\n    print(f"Error: {e}")\n```\n\n## Documentation\n\nFor detailed information on the KeepinCRM API, refer to the official API documentation: [KeepinCRM API Documentation](https://app.swaggerhub.com/apis/KeepInCRM/keepincrm-api/0.12.3)\n\n## License\n\nThis project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.',
-    'author': 'Vadim Radzih',
-    'author_email': 'iphonevadim2003@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/radzih/aiokeepin',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
+You can install the library using pip:
+
+```shell
+pip install aiokeepin
+```
+
+## Usage
+
+To use the KeepinCRM async Python wrapper, import the `KeepinClient` class from the library:
+
+```python
+from aiokeepin import KeepinClient
+```
+
+### Initializing the Client
+
+Create an instance of the `KeepinClient` class by providing your API key:
+
+```python
+client = KeepinClient(api_key='YOUR_API_KEY')
+```
+
+### Making API Requests
+
+The `KeepinClient` instance provides async methods that correspond to the different HTTP request methods (`GET`, `POST`, `PATCH`, `PUT`, `DELETE`). Each method returns a dictionary containing the response from the API.
+
+#### GET Request Example
+
+```python
+response = await client.get('/clients')
+print(response)
+```
+
+#### POST Request Example
+
+```python
+data = {
+  "email": "pib@example.com",
+  "company": "Назва чи ПІБ",
+  "lead": True,
+  "source_id": 5,
+  "status_id": 1,
+  "phones": [
+    "+380000000001"
+  ],
+  "tag_names": [
+    "VIP"
+  ],
+  "contacts_attributes": [
+    {
+      "fullname": "Прізвище Імʼя По батькові",
+      "phones": [
+        "+380000000002"
+      ],
+      "custom_fields": [
+        {
+          "name": "Посада",
+          "value": "Директор"
+        }
+      ]
+    }
+  ]
+}
+
+response = await client.post('/clients', data=data)
+print(response)
+```
+
+#### PATCH Request Example
+
+```python
+data = {
+  "email": "new_email@example.com"
 }
 
+response = await client.patch('/clients/{client_id}', data=data)
+print(response)
+```
+
+#### PUT Request Example
+
+```python
+data = {
+  "email": "updated_email@example.com"
+}
+
+response = await client.put('/clients/{client_id}', data=data)
+print(response)
+```
+
+#### DELETE Request Example
+
+```python
+response = await client.delete('/clients/{client_id}')
+print(response)
+```
+
+#### GET Paginated Items Example
+
+```python
+response = await client.get_paginated_items('/clients')
+```
+
+## Error Handling
+
+In case of an error response from the KeepinCRM API, an exception will be raised. The exceptions provided by the aiokeepin library inherit from the base `KeepinException` class. There are several specific exceptions available for different types of errors:
+
+- `KeepinStatusError`: This exception is raised for non-2xx status codes. It contains the `status_code` and `response` attributes, providing information about the error.
+
+- `InvalidAPIKeyError`: This exception is raised specifically for an invalid API key.
+
+- `ValidationError`: This exception is raised for invalid data.
+
+- `NotFoundError`: This exception is raised when the requested resource is not found.
+
+- `InternalServerError`: This exception is raised for internal server errors.
+
+When making API requests, you can handle exceptions using try-except blocks to capture and handle specific types of errors. Here's an example:
+
+```python
+from aiokeepin.exceptions import KeepinStatusError, InvalidAPIKeyError
+
+try:
+    response = await client.get('/nonexistent_endpoint')
+except InvalidAPIKeyError:
+    print("Invalid API key provided.")
+except KeepinStatusError as e:
+    print(f"Error: {e.status_code} - {e.response}")
+```
+
+You can customize the exception handling based on your specific needs. By catching the appropriate exceptions, you can handle different error scenarios and provide appropriate error messages or take specific actions. Make sure to refer to the documentation for the KeepinCRM API for more details on the possible error responses and their corresponding status codes.
+
+## Documentation
+
+For detailed information on the KeepinCRM API, refer to the official API documentation: [KeepinCRM API Documentation](https://app.swaggerhub.com/apis/KeepInCRM/keepincrm-api/0.12.3)
+
+## License
 
-setup(**setup_kwargs)
+This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
```

