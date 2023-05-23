# Comparing `tmp/ana_sdk-0.1.3.tar.gz` & `tmp/ana_sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ana_sdk-0.1.3.tar", max compression
+gzip compressed data, was "ana_sdk-0.1.4.tar", max compression
```

## Comparing `ana_sdk-0.1.3.tar` & `ana_sdk-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.1.3/ana_sdk/__init__.py
--rw-r--r--   0        0        0    11388 2023-05-23 02:28:17.697025 ana_sdk-0.1.3/ana_sdk/ana.py
--rw-r--r--   0        0        0      177 2023-05-23 01:43:08.849263 ana_sdk-0.1.3/ana_sdk/clients/__init__.py
--rw-r--r--   0        0        0     4332 2023-05-23 01:51:36.706872 ana_sdk-0.1.3/ana_sdk/clients/ana_data_client.py
--rw-r--r--   0        0        0     1770 2023-05-18 23:09:59.503498 ana_sdk-0.1.3/ana_sdk/clients/base_client.py
--rw-r--r--   0        0        0     4635 2023-05-23 01:51:45.997363 ana_sdk-0.1.3/ana_sdk/clients/dashboard_api_client.py
--rw-r--r--   0        0        0     1439 2023-05-18 23:50:34.941495 ana_sdk-0.1.3/ana_sdk/clients/oauth_client.py
--rw-r--r--   0        0        0     3320 2023-05-23 01:51:51.763464 ana_sdk-0.1.3/ana_sdk/clients/rpa_api_client.py
--rw-r--r--   0        0        0      439 2023-05-23 02:28:30.388033 ana_sdk-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.1.3/README.md
--rw-r--r--   0        0        0     2521 1970-01-01 00:00:00.000000 ana_sdk-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.1.4/ana_sdk/__init__.py
+-rw-r--r--   0        0        0    12890 2023-05-23 02:52:39.273005 ana_sdk-0.1.4/ana_sdk/ana.py
+-rw-r--r--   0        0        0      177 2023-05-23 01:43:08.849263 ana_sdk-0.1.4/ana_sdk/clients/__init__.py
+-rw-r--r--   0        0        0     4332 2023-05-23 01:51:36.706872 ana_sdk-0.1.4/ana_sdk/clients/ana_data_client.py
+-rw-r--r--   0        0        0     1770 2023-05-18 23:09:59.503498 ana_sdk-0.1.4/ana_sdk/clients/base_client.py
+-rw-r--r--   0        0        0     4635 2023-05-23 01:51:45.997363 ana_sdk-0.1.4/ana_sdk/clients/dashboard_api_client.py
+-rw-r--r--   0        0        0     1439 2023-05-18 23:50:34.941495 ana_sdk-0.1.4/ana_sdk/clients/oauth_client.py
+-rw-r--r--   0        0        0     3320 2023-05-23 01:51:51.763464 ana_sdk-0.1.4/ana_sdk/clients/rpa_api_client.py
+-rw-r--r--   0        0        0      465 2023-05-23 02:54:02.710563 ana_sdk-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.1.4/README.md
+-rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 ana_sdk-0.1.4/PKG-INFO
```

### Comparing `ana_sdk-0.1.3/ana_sdk/ana.py` & `ana_sdk-0.1.4/ana_sdk/ana.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import os
 import time
 from pprint import PrettyPrinter
 
 from jsonschema import validate
 from requests import HTTPError
+from dotenv import load_dotenv
 
 from .clients.oauth_client import OAuthClient
 from .clients.dashboard_api_client import DashboardAPIClient
 from .clients.rpa_api_client import RPAAPIClient
 from .clients.ana_data_client import ANADataClient
 
 
@@ -25,54 +27,82 @@
         _access_token (str): Token de acesso gerado pelo OAuth.
         api (DashboardAPIClient): Cliente da Dashboard API que realiza
         consultas as dados dos clientes cadastrados na ANA.
         rpa (RPAAPIClient): Cliente da API de RPA da ANA, responsável
         por executar automações.
         data (ANADataClient): Cliente para interagir com os dados do ERP
         dos clientes ANA.
+        ana_email (str): E-mail da ANA para requisições ao ANA-Data. É
+        automaticamente carregada caso exista a variável de ambiente
+        `ANA_EMAIL`.
+        _ana_password (str): Senha da ANA para requisições ao ANA-Data.
+        É automaticamente carregada caso exista a variável de ambiente
+        `ANA_PASSWORD`.
         rpa_api_base_url (str): A URL base da RPA API.
         dashboard_api_base_url (str): A URL base da Dashboard API.
         oauth_token_full_url (str): A URL completa para obter o 
         token do usuário na API do OAuth.
     """
 
     current_empresa: dict = None
     current_cliente: dict = None
     current_tenant: dict = None
 
     api: DashboardAPIClient = None
     rpa: RPAAPIClient = None
     data: ANADataClient = None
+    ana_email: str = None
+    _ana_password: str = None
 
     rpa_api_base_url: str = None
     dashboard_api_base_url: str = None
     oauth_token_full_url: str = None
 
     _auth: OAuthClient = None
     _access_token: str = None
 
     def __init__(
         self,
         rpa_api_base_url: str,
         dashboard_api_base_url: str,
-        oauth_token_full_url: str
+        oauth_token_full_url: str,
+        ana_email: str = None,
+        ana_password: str = None
     ):
         """
         Inicializa uma instância da classe ANA.
 
         Args:
             rpa_api_base_url (str): A URL base da RPA API.
             dashboard_api_base_url (str): A URL base da Dashboard API.
             oauth_token_full_url (str): A URL completa para obter o 
             token do usuário na API do OAuth.
+            ana_email (str): E-mail da ANA para requisições ao ANA-Data.
+            Tem precedência sobre a variável de ambiente `ANA_EMAIL`.
+            ana_password (str): Senha da ANA para requisições ao ANA-Data.
+            Tem precedência sobre a variável de ambiente `ANA_PASSWORD`.
 
         Returns:
             None
         """
 
+        load_dotenv()
+        env_ana_email = os.getenv("ANA_EMAIL")
+        env_ana_password = os.getenv("ANA_PASSWORD")
+
+        if not ((ana_email or env_ana_email) and (ana_password or env_ana_password)):
+            raise ValueError(
+                "Defina as variáveis de ambiente [ANA_EMAIL] e [ANA_PASSWORD]"
+                "ou instancie a classe passando [ana_email] e [ana_password]"
+                "como parâmetros para o construtor."
+            )
+
+        self.ana_email = ana_email or env_ana_email
+        self._ana_password = ana_password or env_ana_password
+        
         self.rpa_api_base_url = rpa_api_base_url
         self.dashboard_api_base_url = dashboard_api_base_url
         self.oauth_token_full_url = oauth_token_full_url
 
     def login(self, email: str, password: str):
         """
         Realiza o login do usuário com as credenciais fornecidas,
@@ -177,15 +207,19 @@
             None
 
         Raises:
             requests.HTTPError: Se ocorrer um erro ao fazer as requisições.
         """
 
         self.current_tenant = self.api.get_tenant(id)
-        self.data = ANADataClient(self.current_tenant["configuracoes"]["ana_data_base_url"])
+        self.data = ANADataClient(
+            self.ana_email,
+            self._ana_password,
+            self.current_tenant["configuracoes"]["ana_data_base_url"]
+        )
 
     def set_cliente(self, id: int) -> None:
         """
         Define o cliente atual com base no ID fornecido. Obtém o
         tenant associado ao cliente e chama o método set_tenant()
         para configurar o ANA Data.
```

### Comparing `ana_sdk-0.1.3/ana_sdk/clients/ana_data_client.py` & `ana_sdk-0.1.4/ana_sdk/clients/ana_data_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.3/ana_sdk/clients/base_client.py` & `ana_sdk-0.1.4/ana_sdk/clients/base_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.3/ana_sdk/clients/dashboard_api_client.py` & `ana_sdk-0.1.4/ana_sdk/clients/dashboard_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.3/ana_sdk/clients/oauth_client.py` & `ana_sdk-0.1.4/ana_sdk/clients/oauth_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.3/ana_sdk/clients/rpa_api_client.py` & `ana_sdk-0.1.4/ana_sdk/clients/rpa_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.3/README.md` & `ana_sdk-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.3/PKG-INFO` & `ana_sdk-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: ana-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: SDK que visa fornecer uma interface para interagir com os serviços ANA.
 License: MIT
 Author: Jovane Mafort
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # ANA SDK
 
 O projeto ANA SDK visa fornecer uma interface para interagir com os serviços
 relacionados ao ambiente de automação de negócios, dados e clientes da ANA.
```

