# Comparing `tmp/getgeo-python-1.0.0.tar.gz` & `tmp/getgeo-python-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getgeo-python-1.0.0.tar", last modified: Tue May 23 08:35:25 2023, max compression
+gzip compressed data, was "getgeo-python-1.1.0.tar", last modified: Tue May 23 09:28:27 2023, max compression
```

## Comparing `getgeo-python-1.0.0.tar` & `getgeo-python-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 freedom   (1000) freedom   (1000)        0 2023-05-23 08:35:25.136818 getgeo-python-1.0.0/
--rw-rw-r--   0 freedom   (1000) freedom   (1000)     1070 2023-05-12 16:42:11.000000 getgeo-python-1.0.0/LICENSE
--rw-rw-r--   0 freedom   (1000) freedom   (1000)     1978 2023-05-23 08:35:25.136818 getgeo-python-1.0.0/PKG-INFO
--rw-rw-r--   0 freedom   (1000) freedom   (1000)     1138 2023-05-23 08:30:37.000000 getgeo-python-1.0.0/README.md
-drwxrwxr-x   0 freedom   (1000) freedom   (1000)        0 2023-05-23 08:35:25.132818 getgeo-python-1.0.0/getgeo/
--rw-rw-r--   0 freedom   (1000) freedom   (1000)        0 2023-05-12 16:43:50.000000 getgeo-python-1.0.0/getgeo/__init__.py
--rw-rw-r--   0 freedom   (1000) freedom   (1000)      437 2023-05-13 07:37:57.000000 getgeo-python-1.0.0/getgeo/base.py
--rw-rw-r--   0 freedom   (1000) freedom   (1000)      507 2023-05-12 17:55:16.000000 getgeo-python-1.0.0/getgeo/geodata.py
-drwxrwxr-x   0 freedom   (1000) freedom   (1000)        0 2023-05-23 08:35:25.136818 getgeo-python-1.0.0/getgeo_python.egg-info/
--rw-rw-r--   0 freedom   (1000) freedom   (1000)     1978 2023-05-23 08:35:25.000000 getgeo-python-1.0.0/getgeo_python.egg-info/PKG-INFO
--rw-rw-r--   0 freedom   (1000) freedom   (1000)      262 2023-05-23 08:35:25.000000 getgeo-python-1.0.0/getgeo_python.egg-info/SOURCES.txt
--rw-rw-r--   0 freedom   (1000) freedom   (1000)        1 2023-05-23 08:35:25.000000 getgeo-python-1.0.0/getgeo_python.egg-info/dependency_links.txt
--rw-rw-r--   0 freedom   (1000) freedom   (1000)       17 2023-05-23 08:35:25.000000 getgeo-python-1.0.0/getgeo_python.egg-info/requires.txt
--rw-rw-r--   0 freedom   (1000) freedom   (1000)        7 2023-05-23 08:35:25.000000 getgeo-python-1.0.0/getgeo_python.egg-info/top_level.txt
--rw-rw-r--   0 freedom   (1000) freedom   (1000)       38 2023-05-23 08:35:25.136818 getgeo-python-1.0.0/setup.cfg
--rw-rw-r--   0 freedom   (1000) freedom   (1000)     1139 2023-05-23 08:33:39.000000 getgeo-python-1.0.0/setup.py
+drwxrwxr-x   0 freedom   (1000) freedom   (1000)        0 2023-05-23 09:28:27.678384 getgeo-python-1.1.0/
+-rw-rw-r--   0 freedom   (1000) freedom   (1000)     1070 2023-05-12 16:42:11.000000 getgeo-python-1.1.0/LICENSE
+-rw-rw-r--   0 freedom   (1000) freedom   (1000)     3557 2023-05-23 09:28:27.678384 getgeo-python-1.1.0/PKG-INFO
+-rw-rw-r--   0 freedom   (1000) freedom   (1000)     2786 2023-05-23 09:26:19.000000 getgeo-python-1.1.0/README.md
+drwxrwxr-x   0 freedom   (1000) freedom   (1000)        0 2023-05-23 09:28:27.674384 getgeo-python-1.1.0/getgeo/
+-rw-rw-r--   0 freedom   (1000) freedom   (1000)        0 2023-05-12 16:43:50.000000 getgeo-python-1.1.0/getgeo/__init__.py
+-rw-rw-r--   0 freedom   (1000) freedom   (1000)      437 2023-05-13 07:37:57.000000 getgeo-python-1.1.0/getgeo/base.py
+-rw-rw-r--   0 freedom   (1000) freedom   (1000)      507 2023-05-12 17:55:16.000000 getgeo-python-1.1.0/getgeo/geodata.py
+drwxrwxr-x   0 freedom   (1000) freedom   (1000)        0 2023-05-23 09:28:27.674384 getgeo-python-1.1.0/getgeo_python.egg-info/
+-rw-rw-r--   0 freedom   (1000) freedom   (1000)     3557 2023-05-23 09:28:27.000000 getgeo-python-1.1.0/getgeo_python.egg-info/PKG-INFO
+-rw-rw-r--   0 freedom   (1000) freedom   (1000)      262 2023-05-23 09:28:27.000000 getgeo-python-1.1.0/getgeo_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 freedom   (1000) freedom   (1000)        1 2023-05-23 09:28:27.000000 getgeo-python-1.1.0/getgeo_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 freedom   (1000) freedom   (1000)       17 2023-05-23 09:28:27.000000 getgeo-python-1.1.0/getgeo_python.egg-info/requires.txt
+-rw-rw-r--   0 freedom   (1000) freedom   (1000)        7 2023-05-23 09:28:27.000000 getgeo-python-1.1.0/getgeo_python.egg-info/top_level.txt
+-rw-rw-r--   0 freedom   (1000) freedom   (1000)       38 2023-05-23 09:28:27.678384 getgeo-python-1.1.0/setup.cfg
+-rw-rw-r--   0 freedom   (1000) freedom   (1000)     1058 2023-05-23 09:27:15.000000 getgeo-python-1.1.0/setup.py
```

### Comparing `getgeo-python-1.0.0/LICENSE` & `getgeo-python-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `getgeo-python-1.0.0/PKG-INFO` & `getgeo-python-1.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: getgeo-python
-Version: 1.0.0
-Summary: A python wrapper for the API provided by getgeoapi.com
-Home-page: https://github.com/LoisaKitakaya/getgeo-python
-Author: Loisa Kitakaya
-Author-email: kitakayaloisa@gmail.com
-Maintainer: Loisa Kitakaya
-Maintainer-email: kitakayaloisa@gmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/LoisaKitakaya/getgeo-python/issues
-Project-URL: Documentation, https://github.com/LoisaKitakaya/getgeo-python#readme
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # getgeo-python
 
 getgeo-python is a python wrapper for the API provided by [getgeoapi.com](https://getgeoapi.com).
 
 This API allows the one to access a wide range of information to better understand ones customers.
 
 #### Information provided by [getgeoapi.com](https://getgeoapi.com) includes:
@@ -38,7 +16,74 @@
 #### Why use [getgeoapi.com](https://getgeoapi.com):
 
 - IPv4 and IPv6 | Access location and security data whether you have an IPv4 or IPv6 address
 - Reliable | Scalable infrastructure with 99.99% up time
 - Secure | 256-bit SSL encryption to ensure your data is transmitted safely
 - Fast | Average response time is 66ms
 
+## Usage
+
+#### Requirements
+
+For you to be able to use this package you must have `Python 3` installed in your system.
+
+You must also have an api_key provided by [getgeoapi.com](https://getgeoapi.com). To get an api_key for your application, simply create an account, and click the 'Generate API Key' button.
+
+Copy your api_key to a secure location.
+
+#### Installation
+
+To use getgeo-python, you need to first install it as follows:
+
+```
+# upgrade pip
+pip install --upgrade pip
+
+# install getgeo-python
+pip install getgeo-python
+```
+
+Once installation is complete, you can now start using getgeo-python.
+
+#### Usage
+
+Import `GetGeoData` class, and create a new instance of it by providing your api key.
+
+```
+# import GetGeoData
+from getgeo.geodata import GetGeoData
+
+# setup api key
+your_api_key = "exampleofapikey"
+
+# create a new instance of GetGeoData
+ip_data = GetGeoData("your_api_key")
+```
+
+Don't forget to replace `"exampleofapikey"` with your actual api_key.
+
+The class `GetGeoData` has two instance methods, i.e.:
+
+- `get_my_geo_data`
+- `get_geo_data`
+
+The `get_my_geo_data` method returns information based on your IP address. While the `get_geo_data` method, takes one argument (any IP address\_\_IPV4 or IPV6), and returns information based on the IP address.
+
+The response of both methods in in json format.
+
+Example:
+
+```
+# get my own geo data
+my_geo_data = ip_data.get_my_geo_data()
+
+print(my_geo_data)
+
+# get geo data of given IP address
+# Google's IPv6 address
+# 2001:4860:4860::8888
+geo_data = ip_data.get_geo_data("2001:4860:4860::8888")
+
+print(geo_data)
+```
+
+For more information visit [getgeoapi.com](https://getgeoapi.com).
```

### Comparing `getgeo-python-1.0.0/setup.py` & `getgeo-python-1.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as file:
     long_description = file.read()
 
 setup(
     name="getgeo-python",
-    version="1.0.0",
+    version="1.1.0",
     description="A python wrapper for the API provided by getgeoapi.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Loisa Kitakaya",
     author_email="kitakayaloisa@gmail.com",
-    maintainer="Loisa Kitakaya",
-    maintainer_email="kitakayaloisa@gmail.com",
     url="https://github.com/LoisaKitakaya/getgeo-python",
     project_urls={
         "Bug Tracker": "https://github.com/LoisaKitakaya/getgeo-python/issues",
         "Documentation": "https://github.com/LoisaKitakaya/getgeo-python#readme",
     },
     packages=find_packages(),
     classifiers=[
```

