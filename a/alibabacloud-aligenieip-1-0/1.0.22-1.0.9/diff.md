# Comparing `tmp/alibabacloud_aligenieip_1_0-1.0.22.tar.gz` & `tmp/alibabacloud_aligenieip_1_0-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aligenieip_1_0-1.0.22.tar", last modified: Tue May 23 02:51:11 2023, max compression
+gzip compressed data, was "dist/alibabacloud_aligenieip_1_0-1.0.9.tar", last modified: Mon Aug 22 08:17:28 2022, max compression
```

## Comparing `alibabacloud_aligenieip_1_0-1.0.22.tar` & `alibabacloud_aligenieip_1_0-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:51:11.000000 alibabacloud_aligenieip_1_0-1.0.22/
--rw-r--r--   0 root         (0) root         (0)      355 2023-05-23 02:51:10.000000 alibabacloud_aligenieip_1_0-1.0.22/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-23 02:51:10.000000 alibabacloud_aligenieip_1_0-1.0.22/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-23 02:51:10.000000 alibabacloud_aligenieip_1_0-1.0.22/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2349 2023-05-23 02:51:11.000000 alibabacloud_aligenieip_1_0-1.0.22/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2023-05-23 02:51:10.000000 alibabacloud_aligenieip_1_0-1.0.22/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1118 2023-05-23 02:51:10.000000 alibabacloud_aligenieip_1_0-1.0.22/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:51:11.000000 alibabacloud_aligenieip_1_0-1.0.22/alibabacloud_aligenieip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-23 02:51:10.000000 alibabacloud_aligenieip_1_0-1.0.22/alibabacloud_aligenieip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   383838 2023-05-23 02:51:10.000000 alibabacloud_aligenieip_1_0-1.0.22/alibabacloud_aligenieip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   666007 2023-05-23 02:51:10.000000 alibabacloud_aligenieip_1_0-1.0.22/alibabacloud_aligenieip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:51:11.000000 alibabacloud_aligenieip_1_0-1.0.22/alibabacloud_aligenieip_1_0.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2349 2023-05-23 02:51:11.000000 alibabacloud_aligenieip_1_0-1.0.22/alibabacloud_aligenieip_1_0.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      444 2023-05-23 02:51:11.000000 alibabacloud_aligenieip_1_0-1.0.22/alibabacloud_aligenieip_1_0.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:51:11.000000 alibabacloud_aligenieip_1_0-1.0.22/alibabacloud_aligenieip_1_0.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-05-23 02:51:11.000000 alibabacloud_aligenieip_1_0-1.0.22/alibabacloud_aligenieip_1_0.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-05-23 02:51:11.000000 alibabacloud_aligenieip_1_0-1.0.22/alibabacloud_aligenieip_1_0.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-23 02:51:11.000000 alibabacloud_aligenieip_1_0-1.0.22/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2629 2023-05-23 02:51:10.000000 alibabacloud_aligenieip_1_0-1.0.22/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:17:28.000000 alibabacloud_aligenieip_1_0-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      600 2022-08-22 08:17:27.000000 alibabacloud_aligenieip_1_0-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-08-22 08:17:27.000000 alibabacloud_aligenieip_1_0-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2348 2022-08-22 08:17:28.000000 alibabacloud_aligenieip_1_0-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2022-08-22 08:17:27.000000 alibabacloud_aligenieip_1_0-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1118 2022-08-22 08:17:27.000000 alibabacloud_aligenieip_1_0-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:17:28.000000 alibabacloud_aligenieip_1_0-1.0.9/alibabacloud_aligenieip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-08-22 08:17:27.000000 alibabacloud_aligenieip_1_0-1.0.9/alibabacloud_aligenieip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66474 2022-08-22 08:17:27.000000 alibabacloud_aligenieip_1_0-1.0.9/alibabacloud_aligenieip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   125043 2022-08-22 08:17:27.000000 alibabacloud_aligenieip_1_0-1.0.9/alibabacloud_aligenieip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:17:28.000000 alibabacloud_aligenieip_1_0-1.0.9/alibabacloud_aligenieip_1_0.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2348 2022-08-22 08:17:27.000000 alibabacloud_aligenieip_1_0-1.0.9/alibabacloud_aligenieip_1_0.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      431 2022-08-22 08:17:28.000000 alibabacloud_aligenieip_1_0-1.0.9/alibabacloud_aligenieip_1_0.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-22 08:17:27.000000 alibabacloud_aligenieip_1_0-1.0.9/alibabacloud_aligenieip_1_0.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-08-22 08:17:27.000000 alibabacloud_aligenieip_1_0-1.0.9/alibabacloud_aligenieip_1_0.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2022-08-22 08:17:27.000000 alibabacloud_aligenieip_1_0-1.0.9/alibabacloud_aligenieip_1_0.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-08-22 08:17:28.000000 alibabacloud_aligenieip_1_0-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2629 2022-08-22 08:17:27.000000 alibabacloud_aligenieip_1_0-1.0.9/setup.py
```

### Comparing `alibabacloud_aligenieip_1_0-1.0.22/LICENSE` & `alibabacloud_aligenieip_1_0-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieip_1_0-1.0.22/PKG-INFO` & `alibabacloud_aligenieip_1_0-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aligenieip_1_0
-Version: 1.0.22
+Version: 1.0.9
 Summary: Alibaba Cloud AliGenie (ip_1_0) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aligenieip_1_0-1.0.22/README-CN.md` & `alibabacloud_aligenieip_1_0-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieip_1_0-1.0.22/README.md` & `alibabacloud_aligenieip_1_0-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieip_1_0-1.0.22/alibabacloud_aligenieip_1_0.egg-info/PKG-INFO` & `alibabacloud_aligenieip_1_0-1.0.9/alibabacloud_aligenieip_1_0.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aligenieip-1-0
-Version: 1.0.22
+Version: 1.0.9
 Summary: Alibaba Cloud AliGenie (ip_1_0) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aligenieip_1_0-1.0.22/setup.py` & `alibabacloud_aligenieip_1_0-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_aligenieip_1_0.
 
-Created on 23/05/2023
+Created on 22/08/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_aligenieip_1_0"
 NAME = "alibabacloud_aligenieip_1_0" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AliGenie (ip_1_0) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
-    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
+    "alibabacloud_tea_util>=0.3.6, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
+    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

