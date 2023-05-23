# Comparing `tmp/bemserver-api-client-0.8.0.tar.gz` & `tmp/bemserver-api-client-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bemserver-api-client-0.8.0.tar", last modified: Thu Jan 12 11:32:56 2023, max compression
+gzip compressed data, was "bemserver-api-client-0.9.0.tar", last modified: Thu Jan 12 15:46:57 2023, max compression
```

## Comparing `bemserver-api-client-0.8.0.tar` & `bemserver-api-client-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 11:32:56.398436 bemserver-api-client-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-01-12 11:32:56.398436 bemserver-api-client-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 11:32:56.398436 bemserver-api-client-0.8.0/bemserver_api_client/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/bemserver_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/bemserver_api_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/bemserver_api_client/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/bemserver_api_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/bemserver_api_client/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 11:32:56.398436 bemserver-api-client-0.8.0/bemserver_api_client/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/bemserver_api_client/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/bemserver_api_client/resources/about.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/bemserver_api_client/resources/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/bemserver_api_client/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/bemserver_api_client/resources/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/bemserver_api_client/resources/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/bemserver_api_client/resources/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/bemserver_api_client/resources/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/bemserver_api_client/resources/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 11:32:56.398436 bemserver-api-client-0.8.0/bemserver_api_client/resources/services/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/bemserver_api_client/resources/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/bemserver_api_client/resources/services/check_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/bemserver_api_client/resources/services/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/bemserver_api_client/resources/structural_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/bemserver_api_client/resources/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/bemserver_api_client/resources/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/bemserver_api_client/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 11:32:56.398436 bemserver-api-client-0.8.0/bemserver_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-01-12 11:32:56.000000 bemserver-api-client-0.8.0/bemserver_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-01-12 11:32:56.000000 bemserver-api-client-0.8.0/bemserver_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 11:32:56.000000 bemserver-api-client-0.8.0/bemserver_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-12 11:32:56.000000 bemserver-api-client-0.8.0/bemserver_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-12 11:32:56.000000 bemserver-api-client-0.8.0/bemserver_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-01-12 11:32:56.402436 bemserver-api-client-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-01-12 11:32:44.000000 bemserver-api-client-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:46:57.810791 bemserver-api-client-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-01-12 15:46:57.810791 bemserver-api-client-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:46:57.810791 bemserver-api-client-0.9.0/bemserver_api_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/bemserver_api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/bemserver_api_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/bemserver_api_client/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/bemserver_api_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/bemserver_api_client/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:46:57.810791 bemserver-api-client-0.9.0/bemserver_api_client/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/bemserver_api_client/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/bemserver_api_client/resources/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/bemserver_api_client/resources/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/bemserver_api_client/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/bemserver_api_client/resources/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/bemserver_api_client/resources/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/bemserver_api_client/resources/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/bemserver_api_client/resources/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/bemserver_api_client/resources/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:46:57.810791 bemserver-api-client-0.9.0/bemserver_api_client/resources/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/bemserver_api_client/resources/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/bemserver_api_client/resources/services/check_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/bemserver_api_client/resources/services/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/bemserver_api_client/resources/structural_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/bemserver_api_client/resources/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/bemserver_api_client/resources/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/bemserver_api_client/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:46:57.810791 bemserver-api-client-0.9.0/bemserver_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-01-12 15:46:57.000000 bemserver-api-client-0.9.0/bemserver_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-01-12 15:46:57.000000 bemserver-api-client-0.9.0/bemserver_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 15:46:57.000000 bemserver-api-client-0.9.0/bemserver_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-12 15:46:57.000000 bemserver-api-client-0.9.0/bemserver_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-12 15:46:57.000000 bemserver-api-client-0.9.0/bemserver_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-01-12 15:46:57.810791 bemserver-api-client-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-01-12 15:46:45.000000 bemserver-api-client-0.9.0/setup.py
```

### Comparing `bemserver-api-client-0.8.0/LICENSE` & `bemserver-api-client-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bemserver-api-client-0.8.0/PKG-INFO` & `bemserver-api-client-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bemserver-api-client
-Version: 0.8.0
+Version: 0.9.0
 Summary: BEMServer API client
 Home-page: https://github.com/BEMServer/bemserver-api-client
 Author: Nobatek/INEF4
 Author-email: dfrederique@nobatek.inef4.com
 License: AGPLv3+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `bemserver-api-client-0.8.0/README.rst` & `bemserver-api-client-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `bemserver-api-client-0.8.0/bemserver_api_client/client.py` & `bemserver-api-client-0.9.0/bemserver_api_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,16 +61,16 @@
     NotificationResources,
 )
 
 
 APICLI_LOGGER = logging.getLogger(__name__)
 
 REQUIRED_API_VERSION = {
-    "min": Version("0.8.0"),
-    "max": Version("0.9.0"),
+    "min": Version("0.9.0"),
+    "max": Version("0.10.0"),
 }
 
 
 class BEMServerApiClient:
     """API client"""
 
     def __init__(
```

### Comparing `bemserver-api-client-0.8.0/bemserver_api_client/enums.py` & `bemserver-api-client-0.9.0/bemserver_api_client/enums.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-client-0.8.0/bemserver_api_client/exceptions.py` & `bemserver-api-client-0.9.0/bemserver_api_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-client-0.8.0/bemserver_api_client/request.py` & `bemserver-api-client-0.9.0/bemserver_api_client/request.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-client-0.8.0/bemserver_api_client/resources/__init__.py` & `bemserver-api-client-0.9.0/bemserver_api_client/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-client-0.8.0/bemserver_api_client/resources/analysis.py` & `bemserver-api-client-0.9.0/bemserver_api_client/resources/analysis.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-client-0.8.0/bemserver_api_client/resources/base.py` & `bemserver-api-client-0.9.0/bemserver_api_client/resources/base.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-client-0.8.0/bemserver_api_client/resources/campaigns.py` & `bemserver-api-client-0.9.0/bemserver_api_client/resources/campaigns.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-client-0.8.0/bemserver_api_client/resources/energy.py` & `bemserver-api-client-0.9.0/bemserver_api_client/resources/energy.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-client-0.8.0/bemserver_api_client/resources/events.py` & `bemserver-api-client-0.9.0/bemserver_api_client/resources/events.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-client-0.8.0/bemserver_api_client/resources/io.py` & `bemserver-api-client-0.9.0/bemserver_api_client/resources/io.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-client-0.8.0/bemserver_api_client/resources/services/cleanup.py` & `bemserver-api-client-0.9.0/bemserver_api_client/resources/services/cleanup.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-client-0.8.0/bemserver_api_client/resources/structural_elements.py` & `bemserver-api-client-0.9.0/bemserver_api_client/resources/structural_elements.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-client-0.8.0/bemserver_api_client/resources/timeseries.py` & `bemserver-api-client-0.9.0/bemserver_api_client/resources/timeseries.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-client-0.8.0/bemserver_api_client/resources/users.py` & `bemserver-api-client-0.9.0/bemserver_api_client/resources/users.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-client-0.8.0/bemserver_api_client/response.py` & `bemserver-api-client-0.9.0/bemserver_api_client/response.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-client-0.8.0/bemserver_api_client.egg-info/PKG-INFO` & `bemserver-api-client-0.9.0/bemserver_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bemserver-api-client
-Version: 0.8.0
+Version: 0.9.0
 Summary: BEMServer API client
 Home-page: https://github.com/BEMServer/bemserver-api-client
 Author: Nobatek/INEF4
 Author-email: dfrederique@nobatek.inef4.com
 License: AGPLv3+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `bemserver-api-client-0.8.0/bemserver_api_client.egg-info/SOURCES.txt` & `bemserver-api-client-0.9.0/bemserver_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bemserver-api-client-0.8.0/setup.py` & `bemserver-api-client-0.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 with open("README.rst", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="bemserver-api-client",
-    version="0.8.0",
+    version="0.9.0",
     description="BEMServer API client",
     long_description=long_description,
     url="https://github.com/BEMServer/bemserver-api-client",
     author="Nobatek/INEF4",
     author_email="dfrederique@nobatek.inef4.com",
     license="AGPLv3+",
     classifiers=[
```

