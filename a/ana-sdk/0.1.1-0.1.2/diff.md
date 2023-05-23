# Comparing `tmp/ana_sdk-0.1.1.tar.gz` & `tmp/ana_sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ana_sdk-0.1.1.tar", max compression
+gzip compressed data, was "ana_sdk-0.1.2.tar", max compression
```

## Comparing `ana_sdk-0.1.1.tar` & `ana_sdk-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.1.1/ana_sdk/__init__.py
--rw-r--r--   0        0        0    11370 2023-05-23 01:44:56.277612 ana_sdk-0.1.1/ana_sdk/ana.py
--rw-r--r--   0        0        0      177 2023-05-23 01:43:08.849263 ana_sdk-0.1.1/ana_sdk/clients/__init__.py
--rw-r--r--   0        0        0     4328 2023-05-19 00:26:58.894867 ana_sdk-0.1.1/ana_sdk/clients/ana_data_client.py
--rw-r--r--   0        0        0     1770 2023-05-18 23:09:59.503498 ana_sdk-0.1.1/ana_sdk/clients/base_client.py
--rw-r--r--   0        0        0     4633 2023-05-18 23:13:44.462134 ana_sdk-0.1.1/ana_sdk/clients/dashboard_api_client.py
--rw-r--r--   0        0        0     1439 2023-05-18 23:50:34.941495 ana_sdk-0.1.1/ana_sdk/clients/oauth_client.py
--rw-r--r--   0        0        0     3318 2023-05-18 23:14:28.182946 ana_sdk-0.1.1/ana_sdk/clients/rpa_api_client.py
--rw-r--r--   0        0        0      439 2023-05-23 01:47:49.084941 ana_sdk-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.1.1/README.md
--rw-r--r--   0        0        0     2521 1970-01-01 00:00:00.000000 ana_sdk-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.1.2/ana_sdk/__init__.py
+-rw-r--r--   0        0        0    11370 2023-05-23 01:44:56.277612 ana_sdk-0.1.2/ana_sdk/ana.py
+-rw-r--r--   0        0        0      177 2023-05-23 01:43:08.849263 ana_sdk-0.1.2/ana_sdk/clients/__init__.py
+-rw-r--r--   0        0        0     4332 2023-05-23 01:51:36.706872 ana_sdk-0.1.2/ana_sdk/clients/ana_data_client.py
+-rw-r--r--   0        0        0     1770 2023-05-18 23:09:59.503498 ana_sdk-0.1.2/ana_sdk/clients/base_client.py
+-rw-r--r--   0        0        0     4635 2023-05-23 01:51:45.997363 ana_sdk-0.1.2/ana_sdk/clients/dashboard_api_client.py
+-rw-r--r--   0        0        0     1439 2023-05-18 23:50:34.941495 ana_sdk-0.1.2/ana_sdk/clients/oauth_client.py
+-rw-r--r--   0        0        0     3320 2023-05-23 01:51:51.763464 ana_sdk-0.1.2/ana_sdk/clients/rpa_api_client.py
+-rw-r--r--   0        0        0      439 2023-05-23 01:52:12.738973 ana_sdk-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.1.2/README.md
+-rw-r--r--   0        0        0     2521 1970-01-01 00:00:00.000000 ana_sdk-0.1.2/PKG-INFO
```

### Comparing `ana_sdk-0.1.1/ana_sdk/ana.py` & `ana_sdk-0.1.2/ana_sdk/ana.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.1/ana_sdk/clients/ana_data_client.py` & `ana_sdk-0.1.2/ana_sdk/clients/ana_data_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 
-from clients.oauth_client import OAuthClient
-from clients.base_client import BaseClient
+from ..clients.oauth_client import OAuthClient
+from ..clients.base_client import BaseClient
 
 
 class ANADataClient(BaseClient):
     """
     Classe para interagir com a API do ANA Data.
 
     Attributes:
```

### Comparing `ana_sdk-0.1.1/ana_sdk/clients/base_client.py` & `ana_sdk-0.1.2/ana_sdk/clients/base_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.1/ana_sdk/clients/dashboard_api_client.py` & `ana_sdk-0.1.2/ana_sdk/clients/dashboard_api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from clients.base_client import BaseClient
+from ..clients.base_client import BaseClient
 
 
 class DashboardAPIClient(BaseClient):
     """
     Classe para interagir com a API do Dashboard.
 
     Atributos:
```

### Comparing `ana_sdk-0.1.1/ana_sdk/clients/oauth_client.py` & `ana_sdk-0.1.2/ana_sdk/clients/oauth_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.1/ana_sdk/clients/rpa_api_client.py` & `ana_sdk-0.1.2/ana_sdk/clients/rpa_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 
-from clients.base_client import BaseClient
+from ..clients.base_client import BaseClient
 
 
 class RPAAPIClient(BaseClient):
     """
     Classe para interagir com o cliente RPA API.
 
     Atributos:
```

### Comparing `ana_sdk-0.1.1/README.md` & `ana_sdk-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.1/PKG-INFO` & `ana_sdk-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ana-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: SDK que visa fornecer uma interface para interagir com os serviços ANA.
 License: MIT
 Author: Jovane Mafort
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

