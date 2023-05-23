# Comparing `tmp/eve_client-2.0.8.tar.gz` & `tmp/eve_client-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eve_client-2.0.8.tar", max compression
+gzip compressed data, was "eve_client-2.0.9.tar", max compression
```

## Comparing `eve_client-2.0.8.tar` & `eve_client-2.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1468 2023-04-18 12:43:35.900999 eve_client-2.0.8/LICENSE.md
--rw-r--r--   0        0        0     6038 2023-01-26 22:55:48.000000 eve_client-2.0.8/README.md
--rw-r--r--   0        0        0        0 2023-01-26 19:08:28.000000 eve_client-2.0.8/eve_client/__init__.py
--rw-r--r--   0        0        0       22 2023-05-10 01:22:55.842200 eve_client-2.0.8/eve_client/__version__.py
--rw-r--r--   0        0        0    23781 2023-05-02 13:16:15.720415 eve_client-2.0.8/eve_client/eve.py
--rw-r--r--   0        0        0      632 2022-06-01 02:54:44.000000 eve_client-2.0.8/eve_client/helper.py
--rw-r--r--   0        0        0      798 2023-05-10 01:22:59.743162 eve_client-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     6712 1970-01-01 00:00:00.000000 eve_client-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1468 2023-04-18 12:43:35.900999 eve_client-2.0.9/LICENSE.md
+-rw-r--r--   0        0        0     6099 2023-05-10 01:25:01.262992 eve_client-2.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-01-26 19:08:28.000000 eve_client-2.0.9/eve_client/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-10 01:25:19.093821 eve_client-2.0.9/eve_client/__version__.py
+-rw-r--r--   0        0        0    23781 2023-05-02 13:16:15.720415 eve_client-2.0.9/eve_client/eve.py
+-rw-r--r--   0        0        0      632 2022-06-01 02:54:44.000000 eve_client-2.0.9/eve_client/helper.py
+-rw-r--r--   0        0        0      798 2023-05-10 01:25:10.701902 eve_client-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6773 1970-01-01 00:00:00.000000 eve_client-2.0.9/PKG-INFO
```

### Comparing `eve_client-2.0.8/LICENSE.md` & `eve_client-2.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eve_client-2.0.8/README.md` & `eve_client-2.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 The EVE API Client is a python class that allows interaction with the [Exodus Vulnerability Enrichment (EVE):](<https://eve.exodusintel.com>) platform.
 
 Welcome to the EVE API Client's documentation. Please get started by reading about how to use it and add it to your projects.
 
 What's new
 ==========
 
-- Access to EVE API version 2.
-    - Search endpoint.
-    - Simplified data structure.
+- Access to EVE API version 2.0
+    - Search endpoints
+    - Organization
+    - Notifications
+    - Saved Searches
+    - Simplified data structure
 - Access to EVE API Anonymous endpoint.
 
+
 Pre-requisites
 ==============
 - An Exodus Intelligence account is required if you want to take advantage of the ful EVE platform.
 - [Python](https://www.python.org/downloads/) 3.8 or newer is required.
 - The EVE platform provides an endpoint to deliver essential information about Common Vulnerabilities and Exposures CVE anonymously.
 
 Getting started
```

### Comparing `eve_client-2.0.8/eve_client/eve.py` & `eve_client-2.0.9/eve_client/eve.py`

 * *Files identical despite different names*

### Comparing `eve_client-2.0.8/eve_client/helper.py` & `eve_client-2.0.9/eve_client/helper.py`

 * *Files identical despite different names*

### Comparing `eve_client-2.0.8/pyproject.toml` & `eve_client-2.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eve_client"
-version = "2.0.8"
+version = "2.0.9"
 description = "EVE Client API Library from Exodus Intelligence LLC."
 authors = ["DevTeam <dev@exodusintel.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 packages = [{include = "eve_client"}]
 
 [tool.poetry.dependencies]
```

### Comparing `eve_client-2.0.8/PKG-INFO` & `eve_client-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eve-client
-Version: 2.0.8
+Version: 2.0.9
 Summary: EVE Client API Library from Exodus Intelligence LLC.
 License: BSD-3-Clause
 Author: DevTeam
 Author-email: dev@exodusintel.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -20,19 +20,23 @@
 The EVE API Client is a python class that allows interaction with the [Exodus Vulnerability Enrichment (EVE):](<https://eve.exodusintel.com>) platform.
 
 Welcome to the EVE API Client's documentation. Please get started by reading about how to use it and add it to your projects.
 
 What's new
 ==========
 
-- Access to EVE API version 2.
-    - Search endpoint.
-    - Simplified data structure.
+- Access to EVE API version 2.0
+    - Search endpoints
+    - Organization
+    - Notifications
+    - Saved Searches
+    - Simplified data structure
 - Access to EVE API Anonymous endpoint.
 
+
 Pre-requisites
 ==============
 - An Exodus Intelligence account is required if you want to take advantage of the ful EVE platform.
 - [Python](https://www.python.org/downloads/) 3.8 or newer is required.
 - The EVE platform provides an endpoint to deliver essential information about Common Vulnerabilities and Exposures CVE anonymously.
 
 Getting started
```

