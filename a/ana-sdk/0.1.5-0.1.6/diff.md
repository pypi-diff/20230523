# Comparing `tmp/ana_sdk-0.1.5.tar.gz` & `tmp/ana_sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ana_sdk-0.1.5.tar", max compression
+gzip compressed data, was "ana_sdk-0.1.6.tar", max compression
```

## Comparing `ana_sdk-0.1.5.tar` & `ana_sdk-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.1.5/ana_sdk/__init__.py
--rw-r--r--   0        0        0    12890 2023-05-23 02:52:39.273005 ana_sdk-0.1.5/ana_sdk/ana.py
--rw-r--r--   0        0        0      177 2023-05-23 01:43:08.849263 ana_sdk-0.1.5/ana_sdk/clients/__init__.py
--rw-r--r--   0        0        0     4523 2023-05-23 02:57:33.535000 ana_sdk-0.1.5/ana_sdk/clients/ana_data_client.py
--rw-r--r--   0        0        0     1770 2023-05-18 23:09:59.503498 ana_sdk-0.1.5/ana_sdk/clients/base_client.py
--rw-r--r--   0        0        0     4635 2023-05-23 01:51:45.997363 ana_sdk-0.1.5/ana_sdk/clients/dashboard_api_client.py
--rw-r--r--   0        0        0     1439 2023-05-18 23:50:34.941495 ana_sdk-0.1.5/ana_sdk/clients/oauth_client.py
--rw-r--r--   0        0        0     3320 2023-05-23 01:51:51.763464 ana_sdk-0.1.5/ana_sdk/clients/rpa_api_client.py
--rw-r--r--   0        0        0      465 2023-05-23 02:57:47.200524 ana_sdk-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.1.5/README.md
--rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 ana_sdk-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.1.6/ana_sdk/__init__.py
+-rw-r--r--   0        0        0    12930 2023-05-23 02:58:56.276660 ana_sdk-0.1.6/ana_sdk/ana.py
+-rw-r--r--   0        0        0      177 2023-05-23 01:43:08.849263 ana_sdk-0.1.6/ana_sdk/clients/__init__.py
+-rw-r--r--   0        0        0     4523 2023-05-23 02:57:33.535000 ana_sdk-0.1.6/ana_sdk/clients/ana_data_client.py
+-rw-r--r--   0        0        0     1770 2023-05-18 23:09:59.503498 ana_sdk-0.1.6/ana_sdk/clients/base_client.py
+-rw-r--r--   0        0        0     4635 2023-05-23 01:51:45.997363 ana_sdk-0.1.6/ana_sdk/clients/dashboard_api_client.py
+-rw-r--r--   0        0        0     1439 2023-05-18 23:50:34.941495 ana_sdk-0.1.6/ana_sdk/clients/oauth_client.py
+-rw-r--r--   0        0        0     3320 2023-05-23 01:51:51.763464 ana_sdk-0.1.6/ana_sdk/clients/rpa_api_client.py
+-rw-r--r--   0        0        0      465 2023-05-23 02:59:11.061947 ana_sdk-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.1.6/README.md
+-rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 ana_sdk-0.1.6/PKG-INFO
```

### Comparing `ana_sdk-0.1.5/ana_sdk/ana.py` & `ana_sdk-0.1.6/ana_sdk/ana.py`

 * *Files 4% similar despite different names*

```diff
@@ -210,15 +210,16 @@
             requests.HTTPError: Se ocorrer um erro ao fazer as requisições.
         """
 
         self.current_tenant = self.api.get_tenant(id)
         self.data = ANADataClient(
             self.ana_email,
             self._ana_password,
-            self.current_tenant["configuracoes"]["ana_data_base_url"]
+            self.current_tenant["configuracoes"]["ana_data_base_url"],
+            self.oauth_token_full_url
         )
 
     def set_cliente(self, id: int) -> None:
         """
         Define o cliente atual com base no ID fornecido. Obtém o
         tenant associado ao cliente e chama o método set_tenant()
         para configurar o ANA Data.
```

### Comparing `ana_sdk-0.1.5/ana_sdk/clients/ana_data_client.py` & `ana_sdk-0.1.6/ana_sdk/clients/ana_data_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.5/ana_sdk/clients/base_client.py` & `ana_sdk-0.1.6/ana_sdk/clients/base_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.5/ana_sdk/clients/dashboard_api_client.py` & `ana_sdk-0.1.6/ana_sdk/clients/dashboard_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.5/ana_sdk/clients/oauth_client.py` & `ana_sdk-0.1.6/ana_sdk/clients/oauth_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.5/ana_sdk/clients/rpa_api_client.py` & `ana_sdk-0.1.6/ana_sdk/clients/rpa_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.5/README.md` & `ana_sdk-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.5/PKG-INFO` & `ana_sdk-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ana-sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: SDK que visa fornecer uma interface para interagir com os serviços ANA.
 License: MIT
 Author: Jovane Mafort
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

