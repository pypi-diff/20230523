# Comparing `tmp/ana_sdk-0.2.0.tar.gz` & `tmp/ana_sdk-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ana_sdk-0.2.0.tar", max compression
+gzip compressed data, was "ana_sdk-0.2.1.tar", max compression
```

## Comparing `ana_sdk-0.2.0.tar` & `ana_sdk-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.2.0/ana_sdk/__init__.py
--rw-r--r--   0        0        0    14777 2023-05-23 18:20:02.428746 ana_sdk-0.2.0/ana_sdk/ana.py
--rw-r--r--   0        0        0      177 2023-05-23 01:43:08.849263 ana_sdk-0.2.0/ana_sdk/clients/__init__.py
--rw-r--r--   0        0        0     4523 2023-05-23 02:57:33.535000 ana_sdk-0.2.0/ana_sdk/clients/ana_data_client.py
--rw-r--r--   0        0        0     1770 2023-05-18 23:09:59.503498 ana_sdk-0.2.0/ana_sdk/clients/base_client.py
--rw-r--r--   0        0        0     4635 2023-05-23 01:51:45.997363 ana_sdk-0.2.0/ana_sdk/clients/dashboard_api_client.py
--rw-r--r--   0        0        0     1438 2023-05-23 03:23:45.283114 ana_sdk-0.2.0/ana_sdk/clients/oauth_client.py
--rw-r--r--   0        0        0     3320 2023-05-23 01:51:51.763464 ana_sdk-0.2.0/ana_sdk/clients/rpa_api_client.py
--rw-r--r--   0        0        0      463 2023-05-23 18:21:30.994581 ana_sdk-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.2.0/README.md
--rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 ana_sdk-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.2.1/ana_sdk/__init__.py
+-rw-r--r--   0        0        0    14791 2023-05-23 18:27:45.153492 ana_sdk-0.2.1/ana_sdk/ana.py
+-rw-r--r--   0        0        0      177 2023-05-23 01:43:08.849263 ana_sdk-0.2.1/ana_sdk/clients/__init__.py
+-rw-r--r--   0        0        0     4523 2023-05-23 02:57:33.535000 ana_sdk-0.2.1/ana_sdk/clients/ana_data_client.py
+-rw-r--r--   0        0        0     1770 2023-05-18 23:09:59.503498 ana_sdk-0.2.1/ana_sdk/clients/base_client.py
+-rw-r--r--   0        0        0     4635 2023-05-23 01:51:45.997363 ana_sdk-0.2.1/ana_sdk/clients/dashboard_api_client.py
+-rw-r--r--   0        0        0     1438 2023-05-23 03:23:45.283114 ana_sdk-0.2.1/ana_sdk/clients/oauth_client.py
+-rw-r--r--   0        0        0     3320 2023-05-23 01:51:51.763464 ana_sdk-0.2.1/ana_sdk/clients/rpa_api_client.py
+-rw-r--r--   0        0        0      463 2023-05-23 18:27:52.206419 ana_sdk-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.2.1/README.md
+-rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 ana_sdk-0.2.1/PKG-INFO
```

### Comparing `ana_sdk-0.2.0/ana_sdk/ana.py` & `ana_sdk-0.2.1/ana_sdk/ana.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         self.ana_email = ana_email or env_ana_email
         self._ana_password = ana_password or env_ana_password
         
         self.rpa_api_base_url = rpa_api_base_url or env_rpa_api_base_url
         self.dashboard_api_base_url = dashboard_api_base_url or env_dashboard_api_base_url
         self.oauth_token_full_url = oauth_token_full_url or env_oauth_token_full_url
 
-    def login(self, email: str, password: str):
+    def login(self, email: str = None, password: str = None):
         """
         Realiza o login do usuário com as credenciais fornecidas,
         obtendo o token de acesso e configurando os clientes para
         interagir com os serviços fornecidos.
 
         Args:
             email (str): O email do usuário.
```

### Comparing `ana_sdk-0.2.0/ana_sdk/clients/ana_data_client.py` & `ana_sdk-0.2.1/ana_sdk/clients/ana_data_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.0/ana_sdk/clients/base_client.py` & `ana_sdk-0.2.1/ana_sdk/clients/base_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.0/ana_sdk/clients/dashboard_api_client.py` & `ana_sdk-0.2.1/ana_sdk/clients/dashboard_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.0/ana_sdk/clients/oauth_client.py` & `ana_sdk-0.2.1/ana_sdk/clients/oauth_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.0/ana_sdk/clients/rpa_api_client.py` & `ana_sdk-0.2.1/ana_sdk/clients/rpa_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.0/README.md` & `ana_sdk-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.0/PKG-INFO` & `ana_sdk-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ana-sdk
-Version: 0.2.0
+Version: 0.2.1
 Summary: SDK que visa fornecer uma interface para interagir com os serviços ANA.
 License: MIT
 Author: Jovane Mafort
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

