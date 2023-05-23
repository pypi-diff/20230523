# Comparing `tmp/ana_sdk-0.1.0.tar.gz` & `tmp/ana_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ana_sdk-0.1.0.tar", max compression
+gzip compressed data, was "ana_sdk-0.1.1.tar", max compression
```

## Comparing `ana_sdk-0.1.0.tar` & `ana_sdk-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.1.0/ana_sdk/__init__.py
--rw-r--r--   0        0        0    11367 2023-05-19 18:31:00.184979 ana_sdk-0.1.0/ana_sdk/ana.py
--rw-r--r--   0        0        0        0 2023-05-16 05:19:04.257434 ana_sdk-0.1.0/ana_sdk/clients/__init__.py
--rw-r--r--   0        0        0     4328 2023-05-19 00:26:58.894867 ana_sdk-0.1.0/ana_sdk/clients/ana_data_client.py
--rw-r--r--   0        0        0     1770 2023-05-18 23:09:59.503498 ana_sdk-0.1.0/ana_sdk/clients/base_client.py
--rw-r--r--   0        0        0     4633 2023-05-18 23:13:44.462134 ana_sdk-0.1.0/ana_sdk/clients/dashboard_api_client.py
--rw-r--r--   0        0        0     1439 2023-05-18 23:50:34.941495 ana_sdk-0.1.0/ana_sdk/clients/oauth_client.py
--rw-r--r--   0        0        0     3318 2023-05-18 23:14:28.182946 ana_sdk-0.1.0/ana_sdk/clients/rpa_api_client.py
--rw-r--r--   0        0        0      439 2023-05-22 14:00:52.418267 ana_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.1.0/README.md
--rw-r--r--   0        0        0     2521 1970-01-01 00:00:00.000000 ana_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.1.1/ana_sdk/__init__.py
+-rw-r--r--   0        0        0    11370 2023-05-23 01:44:56.277612 ana_sdk-0.1.1/ana_sdk/ana.py
+-rw-r--r--   0        0        0      177 2023-05-23 01:43:08.849263 ana_sdk-0.1.1/ana_sdk/clients/__init__.py
+-rw-r--r--   0        0        0     4328 2023-05-19 00:26:58.894867 ana_sdk-0.1.1/ana_sdk/clients/ana_data_client.py
+-rw-r--r--   0        0        0     1770 2023-05-18 23:09:59.503498 ana_sdk-0.1.1/ana_sdk/clients/base_client.py
+-rw-r--r--   0        0        0     4633 2023-05-18 23:13:44.462134 ana_sdk-0.1.1/ana_sdk/clients/dashboard_api_client.py
+-rw-r--r--   0        0        0     1439 2023-05-18 23:50:34.941495 ana_sdk-0.1.1/ana_sdk/clients/oauth_client.py
+-rw-r--r--   0        0        0     3318 2023-05-18 23:14:28.182946 ana_sdk-0.1.1/ana_sdk/clients/rpa_api_client.py
+-rw-r--r--   0        0        0      439 2023-05-23 01:47:49.084941 ana_sdk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.1.1/README.md
+-rw-r--r--   0        0        0     2521 1970-01-01 00:00:00.000000 ana_sdk-0.1.1/PKG-INFO
```

### Comparing `ana_sdk-0.1.0/ana_sdk/ana.py` & `ana_sdk-0.1.1/ana_sdk/ana.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import time
 from pprint import PrettyPrinter
 
 from jsonschema import validate
 from requests import HTTPError
 
-from clients.oauth_client import OAuthClient
-from clients.dashboard_api_client import DashboardAPIClient
-from clients.rpa_api_client import RPAAPIClient
-from clients.ana_data_client import ANADataClient
+from .clients.oauth_client import OAuthClient
+from .clients.dashboard_api_client import DashboardAPIClient
+from .clients.rpa_api_client import RPAAPIClient
+from .clients.ana_data_client import ANADataClient
 
 
 class ANA:
     """
     A classe ANA fornece uma interface para interagir com os serviços
     relacionados ao ambiente de automação de negócios, dados e clientes.
     Permite realizar login, executar comandos, definir tenant, cliente
@@ -167,15 +167,15 @@
 
     def set_tenant(self, id: int) -> None:
         """
         Define o tenant atual com base no ID fornecido. Configura o
         cliente do ANA Data.
         
         Args:
-            id (int): O ID da empresa.
+            id (int): O ID do tenant.
 
         Returns:
             None
 
         Raises:
             requests.HTTPError: Se ocorrer um erro ao fazer as requisições.
         """
@@ -186,15 +186,15 @@
     def set_cliente(self, id: int) -> None:
         """
         Define o cliente atual com base no ID fornecido. Obtém o
         tenant associado ao cliente e chama o método set_tenant()
         para configurar o ANA Data.
         
         Args:
-            id (int): O ID da empresa.
+            id (int): O ID do cliente.
 
         Returns:
             None
 
         Raises:
             requests.HTTPError: Se ocorrer um erro ao fazer as requisições.
         """
```

### Comparing `ana_sdk-0.1.0/ana_sdk/clients/ana_data_client.py` & `ana_sdk-0.1.1/ana_sdk/clients/ana_data_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.0/ana_sdk/clients/base_client.py` & `ana_sdk-0.1.1/ana_sdk/clients/base_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.0/ana_sdk/clients/dashboard_api_client.py` & `ana_sdk-0.1.1/ana_sdk/clients/dashboard_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.0/ana_sdk/clients/oauth_client.py` & `ana_sdk-0.1.1/ana_sdk/clients/oauth_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.0/ana_sdk/clients/rpa_api_client.py` & `ana_sdk-0.1.1/ana_sdk/clients/rpa_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.0/README.md` & `ana_sdk-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.0/PKG-INFO` & `ana_sdk-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ana-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: SDK que visa fornecer uma interface para interagir com os serviços ANA.
 License: MIT
 Author: Jovane Mafort
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

