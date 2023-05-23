# Comparing `tmp/apiip-1.0.0.tar.gz` & `tmp/apiip-1.0.1.tar.gz`

## Comparing `apiip-1.0.0.tar` & `apiip-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 apiip-1.0.0/.vscode/settings.json
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 apiip-1.0.0/src/apiip/__init__.py
--rw-r--r--   0        0        0    10629 2020-02-02 00:00:00.000000 apiip-1.0.0/LICENCE
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 apiip-1.0.0/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 apiip-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 apiip-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 apiip-1.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 apiip-1.0.1/src/apiip/__init__.py
+-rw-r--r--   0        0        0    10629 2020-02-02 00:00:00.000000 apiip-1.0.1/LICENCE
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 apiip-1.0.1/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 apiip-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 apiip-1.0.1/PKG-INFO
```

### Comparing `apiip-1.0.0/src/apiip/__init__.py` & `apiip-1.0.1/src/apiip/__init__.py`

 * *Files identical despite different names*

### Comparing `apiip-1.0.0/LICENCE` & `apiip-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `apiip-1.0.0/README.md` & `apiip-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 You need to get your API key from here: https://apiip.net/get-started and you'll get 5.000 free requests/month
 
 For more details, please visit: [API Documentation](https://apiip.net/documentation)
 
 To install this package type the following (for PyPI):
 
 ```sh
-pip install apiip.net
+pip install apiip
 ```
 
 ## Usage
 
 The package needs to be configured with your account's API key, which is available in the [Apiip.net Dashboard](https://apiip.net/user/dashboard)
 
 ```python
```

### Comparing `apiip-1.0.0/pyproject.toml` & `apiip-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "apiip"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="apiip", email="apiipnet.business@gmail.com" },
 ]
 description = "Official python package for apiip.net, it offers one of the leading IP to geolocation API, get the location of any IP with a world-class API serving city, region, country, lat/long data, etc."
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `apiip-1.0.0/PKG-INFO` & `apiip-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiip
-Version: 1.0.0
+Version: 1.0.1
 Summary: Official python package for apiip.net, it offers one of the leading IP to geolocation API, get the location of any IP with a world-class API serving city, region, country, lat/long data, etc.
 Project-URL: Homepage, https://apiip.net
 Project-URL: Documentation, https://apiip.net/documentation
 Author-email: apiip <apiipnet.business@gmail.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -22,15 +22,15 @@
 You need to get your API key from here: https://apiip.net/get-started and you'll get 5.000 free requests/month
 
 For more details, please visit: [API Documentation](https://apiip.net/documentation)
 
 To install this package type the following (for PyPI):
 
 ```sh
-pip install apiip.net
+pip install apiip
 ```
 
 ## Usage
 
 The package needs to be configured with your account's API key, which is available in the [Apiip.net Dashboard](https://apiip.net/user/dashboard)
 
 ```python
```

