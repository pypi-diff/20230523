# Comparing `tmp/openworld-sdk-python-core-0.6.2.tar.gz` & `tmp/openworld-sdk-python-core-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openworld-sdk-python-core-0.6.2.tar", last modified: Tue May  2 17:09:37 2023, max compression
+gzip compressed data, was "openworld-sdk-python-core-0.7.0.tar", last modified: Tue May 23 17:17:34 2023, max compression
```

## Comparing `openworld-sdk-python-core-0.6.2.tar` & `openworld-sdk-python-core-0.7.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:09:37.068401 openworld-sdk-python-core-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-02 17:09:37.068401 openworld-sdk-python-core-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:09:37.064401 openworld-sdk-python-core-0.6.2/client/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/client/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/client/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/client/openworld_auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/client/rapid_auth_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:09:37.064401 openworld-sdk-python-core-0.6.2/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/configuration/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/configuration/client_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:09:37.064401 openworld-sdk-python-core-0.6.2/constant/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/constant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/constant/body.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/constant/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/constant/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/constant/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/constant/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/constant/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:09:37.064401 openworld-sdk-python-core-0.6.2/model/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/model/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/model/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:09:37.064401 openworld-sdk-python-core-0.6.2/model/exception/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/model/exception/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/model/exception/openworld.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/model/exception/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/model/rapid_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:09:37.068401 openworld-sdk-python-core-0.6.2/openworld_sdk_python_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-02 17:09:37.000000 openworld-sdk-python-core-0.6.2/openworld_sdk_python_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-02 17:09:37.000000 openworld-sdk-python-core-0.6.2/openworld_sdk_python_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:09:37.000000 openworld-sdk-python-core-0.6.2/openworld_sdk_python_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:09:37.000000 openworld-sdk-python-core-0.6.2/openworld_sdk_python_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 17:09:37.000000 openworld-sdk-python-core-0.6.2/openworld_sdk_python_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:09:37.068401 openworld-sdk-python-core-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:09:37.064401 openworld-sdk-python-core-0.6.2/util/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-02 17:09:24.000000 openworld-sdk-python-core-0.6.2/util/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:17:34.735520 openworld-sdk-python-core-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-23 17:17:34.735520 openworld-sdk-python-core-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:17:34.731520 openworld-sdk-python-core-0.7.0/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/client/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/client/openworld_auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/client/rapid_auth_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:17:34.731520 openworld-sdk-python-core-0.7.0/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/configuration/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/configuration/client_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:17:34.731520 openworld-sdk-python-core-0.7.0/constant/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/constant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/constant/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/constant/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/constant/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/constant/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/constant/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/constant/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:17:34.735520 openworld-sdk-python-core-0.7.0/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/model/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/model/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:17:34.735520 openworld-sdk-python-core-0.7.0/model/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/model/exception/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/model/exception/openworld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/model/exception/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/model/rapid_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:17:34.735520 openworld-sdk-python-core-0.7.0/openworld_sdk_python_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-23 17:17:34.000000 openworld-sdk-python-core-0.7.0/openworld_sdk_python_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-23 17:17:34.000000 openworld-sdk-python-core-0.7.0/openworld_sdk_python_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:17:34.000000 openworld-sdk-python-core-0.7.0/openworld_sdk_python_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 17:17:34.000000 openworld-sdk-python-core-0.7.0/openworld_sdk_python_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 17:17:34.000000 openworld-sdk-python-core-0.7.0/openworld_sdk_python_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 17:17:34.735520 openworld-sdk-python-core-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:17:34.735520 openworld-sdk-python-core-0.7.0/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-23 17:17:22.000000 openworld-sdk-python-core-0.7.0/util/log.py
```

### Comparing `openworld-sdk-python-core-0.6.2/PKG-INFO` & `openworld-sdk-python-core-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openworld-sdk-python-core
-Version: 0.6.2
+Version: 0.7.0
 Summary: Open World SDK Core Library for Python
 Home-page: https://github.com/ExpediaGroup/openworld-sdk-python
 Author: Expedia Group
 Author-email: oss@expediagroup.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

### Comparing `openworld-sdk-python-core-0.6.2/__init__.py` & `openworld-sdk-python-core-0.7.0/__init__.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/client/__init__.py` & `openworld-sdk-python-core-0.7.0/client/__init__.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/client/api.py` & `openworld-sdk-python-core-0.7.0/client/api.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/client/auth_client.py` & `openworld-sdk-python-core-0.7.0/client/auth_client.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/client/openworld_auth_client.py` & `openworld-sdk-python-core-0.7.0/client/openworld_auth_client.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/client/rapid_auth_client.py` & `openworld-sdk-python-core-0.7.0/client/rapid_auth_client.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/configuration/__init__.py` & `openworld-sdk-python-core-0.7.0/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/configuration/auth_config.py` & `openworld-sdk-python-core-0.7.0/configuration/auth_config.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/configuration/client_config.py` & `openworld-sdk-python-core-0.7.0/configuration/client_config.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/constant/__init__.py` & `openworld-sdk-python-core-0.7.0/constant/__init__.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/constant/body.py` & `openworld-sdk-python-core-0.7.0/constant/body.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/constant/constant.py` & `openworld-sdk-python-core-0.7.0/constant/constant.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/constant/header.py` & `openworld-sdk-python-core-0.7.0/constant/header.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/constant/log.py` & `openworld-sdk-python-core-0.7.0/constant/log.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/constant/message.py` & `openworld-sdk-python-core-0.7.0/constant/message.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/constant/url.py` & `openworld-sdk-python-core-0.7.0/constant/url.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/model/__init__.py` & `openworld-sdk-python-core-0.7.0/model/__init__.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/model/authentication.py` & `openworld-sdk-python-core-0.7.0/model/authentication.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/model/error.py` & `openworld-sdk-python-core-0.7.0/model/error.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/model/exception/client.py` & `openworld-sdk-python-core-0.7.0/model/exception/client.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/model/exception/openworld.py` & `openworld-sdk-python-core-0.7.0/model/exception/openworld.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/model/exception/service.py` & `openworld-sdk-python-core-0.7.0/model/exception/service.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/model/rapid_auth.py` & `openworld-sdk-python-core-0.7.0/model/rapid_auth.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/openworld_sdk_python_core.egg-info/PKG-INFO` & `openworld-sdk-python-core-0.7.0/openworld_sdk_python_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openworld-sdk-python-core
-Version: 0.6.2
+Version: 0.7.0
 Summary: Open World SDK Core Library for Python
 Home-page: https://github.com/ExpediaGroup/openworld-sdk-python
 Author: Expedia Group
 Author-email: oss@expediagroup.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

### Comparing `openworld-sdk-python-core-0.6.2/openworld_sdk_python_core.egg-info/SOURCES.txt` & `openworld-sdk-python-core-0.7.0/openworld_sdk_python_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/setup.py` & `openworld-sdk-python-core-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/util/__init__.py` & `openworld-sdk-python-core-0.7.0/util/__init__.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.6.2/util/log.py` & `openworld-sdk-python-core-0.7.0/util/log.py`

 * *Files identical despite different names*

