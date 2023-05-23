# Comparing `tmp/apiip-1.0.1.tar.gz` & `tmp/apiip-1.0.2.tar.gz`

## Comparing `apiip-1.0.1.tar` & `apiip-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 apiip-1.0.1/.vscode/settings.json
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 apiip-1.0.1/src/apiip/__init__.py
--rw-r--r--   0        0        0    10629 2020-02-02 00:00:00.000000 apiip-1.0.1/LICENCE
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 apiip-1.0.1/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 apiip-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 apiip-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 apiip-1.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 apiip-1.0.2/src/apiip/__init__.py
+-rw-r--r--   0        0        0    10629 2020-02-02 00:00:00.000000 apiip-1.0.2/LICENCE
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 apiip-1.0.2/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 apiip-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 apiip-1.0.2/PKG-INFO
```

### Comparing `apiip-1.0.1/src/apiip/__init__.py` & `apiip-1.0.2/src/apiip/__init__.py`

 * *Files identical despite different names*

### Comparing `apiip-1.0.1/LICENCE` & `apiip-1.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `apiip-1.0.1/README.md` & `apiip-1.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ```
 
 ## Usage
 
 The package needs to be configured with your account's API key, which is available in the [Apiip.net Dashboard](https://apiip.net/user/dashboard)
 
 ```python
-import apiip
+from apiip import apiip
 
 api_client = apiip('YOUR_API_KEY')
 
 info = api_client.get_location()
 
 print(info)
 ```
@@ -33,29 +33,29 @@
 ## HTTPS Encryption
 
 By default, the SSL/TLS is turned off, if you want to enable it just pass the options parameter
 
 #### Example
 
 ```python
-import apiip
+from apiip import apiip
 
 api_client = apiip('YOUR_API_KEY', {'ssl': True})
 
 info = api_client.get_location()
 
 print(info)
 ```
 
 ## Configuration
 
 Call getLocation method with config object
 
 ```python
-import apiip
+from apiip import apiip
 
 api_client = apiip('YOUR_API_KEY', {'ssl': True})
 
 info = api_client.getLocation({
     'ip': "67.250.186.196", # '67.250.186.196, 188.79.34.191, 60.138.7.24' - for bulk request
     'output': "xml",
     'fields': "city, countryName, currency.name",
```

### Comparing `apiip-1.0.1/pyproject.toml` & `apiip-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "apiip"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="apiip", email="apiipnet.business@gmail.com" },
 ]
 description = "Official python package for apiip.net, it offers one of the leading IP to geolocation API, get the location of any IP with a world-class API serving city, region, country, lat/long data, etc."
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `apiip-1.0.1/PKG-INFO` & `apiip-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiip
-Version: 1.0.1
+Version: 1.0.2
 Summary: Official python package for apiip.net, it offers one of the leading IP to geolocation API, get the location of any IP with a world-class API serving city, region, country, lat/long data, etc.
 Project-URL: Homepage, https://apiip.net
 Project-URL: Documentation, https://apiip.net/documentation
 Author-email: apiip <apiipnet.business@gmail.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -30,15 +30,15 @@
 ```
 
 ## Usage
 
 The package needs to be configured with your account's API key, which is available in the [Apiip.net Dashboard](https://apiip.net/user/dashboard)
 
 ```python
-import apiip
+from apiip import apiip
 
 api_client = apiip('YOUR_API_KEY')
 
 info = api_client.get_location()
 
 print(info)
 ```
@@ -46,29 +46,29 @@
 ## HTTPS Encryption
 
 By default, the SSL/TLS is turned off, if you want to enable it just pass the options parameter
 
 #### Example
 
 ```python
-import apiip
+from apiip import apiip
 
 api_client = apiip('YOUR_API_KEY', {'ssl': True})
 
 info = api_client.get_location()
 
 print(info)
 ```
 
 ## Configuration
 
 Call getLocation method with config object
 
 ```python
-import apiip
+from apiip import apiip
 
 api_client = apiip('YOUR_API_KEY', {'ssl': True})
 
 info = api_client.getLocation({
     'ip': "67.250.186.196", # '67.250.186.196, 188.79.34.191, 60.138.7.24' - for bulk request
     'output': "xml",
     'fields': "city, countryName, currency.name",
```

