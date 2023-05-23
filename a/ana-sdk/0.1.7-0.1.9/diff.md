# Comparing `tmp/ana_sdk-0.1.7.tar.gz` & `tmp/ana_sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ana_sdk-0.1.7.tar", max compression
+gzip compressed data, was "ana_sdk-0.1.9.tar", max compression
```

## Comparing `ana_sdk-0.1.7.tar` & `ana_sdk-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.1.7/ana_sdk/__init__.py
--rw-r--r--   0        0        0    12932 2023-05-23 03:03:39.447540 ana_sdk-0.1.7/ana_sdk/ana.py
--rw-r--r--   0        0        0      177 2023-05-23 01:43:08.849263 ana_sdk-0.1.7/ana_sdk/clients/__init__.py
--rw-r--r--   0        0        0     4523 2023-05-23 02:57:33.535000 ana_sdk-0.1.7/ana_sdk/clients/ana_data_client.py
--rw-r--r--   0        0        0     1770 2023-05-18 23:09:59.503498 ana_sdk-0.1.7/ana_sdk/clients/base_client.py
--rw-r--r--   0        0        0     4635 2023-05-23 01:51:45.997363 ana_sdk-0.1.7/ana_sdk/clients/dashboard_api_client.py
--rw-r--r--   0        0        0     1438 2023-05-23 03:23:45.283114 ana_sdk-0.1.7/ana_sdk/clients/oauth_client.py
--rw-r--r--   0        0        0     3320 2023-05-23 01:51:51.763464 ana_sdk-0.1.7/ana_sdk/clients/rpa_api_client.py
--rw-r--r--   0        0        0      465 2023-05-23 03:24:02.400008 ana_sdk-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.1.7/README.md
--rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 ana_sdk-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.1.9/ana_sdk/__init__.py
+-rw-r--r--   0        0        0    12932 2023-05-23 04:23:59.369816 ana_sdk-0.1.9/ana_sdk/ana.py
+-rw-r--r--   0        0        0      177 2023-05-23 01:43:08.849263 ana_sdk-0.1.9/ana_sdk/clients/__init__.py
+-rw-r--r--   0        0        0     4523 2023-05-23 02:57:33.535000 ana_sdk-0.1.9/ana_sdk/clients/ana_data_client.py
+-rw-r--r--   0        0        0     1770 2023-05-18 23:09:59.503498 ana_sdk-0.1.9/ana_sdk/clients/base_client.py
+-rw-r--r--   0        0        0     4635 2023-05-23 01:51:45.997363 ana_sdk-0.1.9/ana_sdk/clients/dashboard_api_client.py
+-rw-r--r--   0        0        0     1438 2023-05-23 03:23:45.283114 ana_sdk-0.1.9/ana_sdk/clients/oauth_client.py
+-rw-r--r--   0        0        0     3320 2023-05-23 01:51:51.763464 ana_sdk-0.1.9/ana_sdk/clients/rpa_api_client.py
+-rw-r--r--   0        0        0      463 2023-05-23 04:24:14.161660 ana_sdk-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.1.9/README.md
+-rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 ana_sdk-0.1.9/PKG-INFO
```

### Comparing `ana_sdk-0.1.7/ana_sdk/ana.py` & `ana_sdk-0.1.9/ana_sdk/ana.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.7/ana_sdk/clients/ana_data_client.py` & `ana_sdk-0.1.9/ana_sdk/clients/ana_data_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.7/ana_sdk/clients/base_client.py` & `ana_sdk-0.1.9/ana_sdk/clients/base_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.7/ana_sdk/clients/dashboard_api_client.py` & `ana_sdk-0.1.9/ana_sdk/clients/dashboard_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.7/ana_sdk/clients/oauth_client.py` & `ana_sdk-0.1.9/ana_sdk/clients/oauth_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.7/ana_sdk/clients/rpa_api_client.py` & `ana_sdk-0.1.9/ana_sdk/clients/rpa_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.7/README.md` & `ana_sdk-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.1.7/PKG-INFO` & `ana_sdk-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ana-sdk
-Version: 0.1.7
+Version: 0.1.9
 Summary: SDK que visa fornecer uma interface para interagir com os serviços ANA.
 License: MIT
 Author: Jovane Mafort
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

