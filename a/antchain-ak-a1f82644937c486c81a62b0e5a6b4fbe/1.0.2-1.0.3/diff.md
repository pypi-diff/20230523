# Comparing `tmp/antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2.tar.gz` & `tmp/antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2.tar", last modified: Sun Apr 23 07:55:20 2023, max compression
+gzip compressed data, was "dist/antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3.tar", last modified: Mon Apr 24 13:12:42 2023, max compression
```

## Comparing `antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2.tar` & `antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:55:20.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-23 07:55:19.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-23 07:55:19.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-04-23 07:55:20.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-04-23 07:55:19.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-04-23 07:55:19.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:55:20.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-04-23 07:55:19.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-04-23 07:55:19.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 07:55:19.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-23 07:55:19.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-04-23 07:55:19.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 07:55:20.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/antchain_sdk_ak_a1f82644937c486c81a62b0e5a6b4fbe/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-23 07:55:19.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/antchain_sdk_ak_a1f82644937c486c81a62b0e5a6b4fbe/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15340 2023-04-23 07:55:19.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/antchain_sdk_ak_a1f82644937c486c81a62b0e5a6b4fbe/client.py
--rw-r--r--   0 root         (0) root         (0)     9460 2023-04-23 07:55:19.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/antchain_sdk_ak_a1f82644937c486c81a62b0e5a6b4fbe/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-23 07:55:20.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-04-23 07:55:19.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:12:42.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-24 13:12:41.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-24 13:12:41.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-04-24 13:12:42.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-04-24 13:12:41.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-04-24 13:12:41.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:12:42.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-04-24 13:12:41.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-04-24 13:12:41.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 13:12:41.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-04-24 13:12:41.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-04-24 13:12:41.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:12:42.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/antchain_sdk_ak_a1f82644937c486c81a62b0e5a6b4fbe/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-24 13:12:41.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/antchain_sdk_ak_a1f82644937c486c81a62b0e5a6b4fbe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15340 2023-04-24 13:12:41.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/antchain_sdk_ak_a1f82644937c486c81a62b0e5a6b4fbe/client.py
+-rw-r--r--   0 root         (0) root         (0)     9460 2023-04-24 13:12:41.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/antchain_sdk_ak_a1f82644937c486c81a62b0e5a6b4fbe/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-24 13:12:42.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-04-24 13:12:41.000000 antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/setup.py
```

### Comparing `antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/LICENSE` & `antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/PKG-INFO` & `antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe
-Version: 1.0.2
+Version: 1.0.3
 Summary: Ant Chain Ak_a1f82644937c486c81a62b0e5a6b4fbe SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/README-CN.md` & `antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/README.md` & `antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe.egg-info/PKG-INFO` & `antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-a1f82644937c486c81a62b0e5a6b4fbe
-Version: 1.0.2
+Version: 1.0.3
 Summary: Ant Chain Ak_a1f82644937c486c81a62b0e5a6b4fbe SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe.egg-info/SOURCES.txt` & `antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/antchain_sdk_ak_a1f82644937c486c81a62b0e5a6b4fbe/client.py` & `antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/antchain_sdk_ak_a1f82644937c486c81a62b0e5a6b4fbe/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.2',
+                    'sdk_version': '1.0.3',
                     '_prod_code': 'ak_a1f82644937c486c81a62b0e5a6b4fbe',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -233,15 +233,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.2',
+                    'sdk_version': '1.0.3',
                     '_prod_code': 'ak_a1f82644937c486c81a62b0e5a6b4fbe',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/antchain_sdk_ak_a1f82644937c486c81a62b0e5a6b4fbe/models.py` & `antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/antchain_sdk_ak_a1f82644937c486c81a62b0e5a6b4fbe/models.py`

 * *Files identical despite different names*

### Comparing `antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.2/setup.py` & `antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe.
 
-Created on 23/04/2023
+Created on 24/04/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_ak_a1f82644937c486c81a62b0e5a6b4fbe"
 NAME = "antchain_ak_a1f82644937c486c81a62b0e5a6b4fbe" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain Ak_a1f82644937c486c81a62b0e5a6b4fbe SDK Library for Python"
```

