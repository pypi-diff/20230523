# Comparing `tmp/fedops-0.1.5.tar.gz` & `tmp/fedops-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedops-0.1.5.tar", last modified: Tue May 23 04:00:33 2023, max compression
+gzip compressed data, was "fedops-0.1.6.tar", last modified: Tue May 23 04:15:37 2023, max compression
```

## Comparing `fedops-0.1.5.tar` & `fedops-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 04:00:33.817306 fedops-0.1.5/
--rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 04:00:33.817083 fedops-0.1.5/PKG-INFO
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 04:00:33.811419 fedops-0.1.5/fedops/
--rw-r--r--   0 yangsemo   (501) staff       (20)      872 2023-05-23 02:14:46.000000 fedops-0.1.5/fedops/__init__.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 04:00:33.814732 fedops-0.1.5/fedops/client/
--rw-r--r--   0 yangsemo   (501) staff       (20)      987 2023-05-23 03:33:41.000000 fedops-0.1.5/fedops/client/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     7031 2023-05-23 03:33:41.000000 fedops-0.1.5/fedops/client/app.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     5010 2023-05-22 17:11:45.000000 fedops-0.1.5/fedops/client/app_test.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2817 2023-05-23 03:33:41.000000 fedops-0.1.5/fedops/client/client_api.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     6081 2023-05-23 03:33:41.000000 fedops-0.1.5/fedops/client/client_fl.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     3478 2023-05-23 03:34:07.000000 fedops-0.1.5/fedops/client/client_utils.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2238 2023-05-23 03:34:17.000000 fedops-0.1.5/fedops/client/client_wandb.py
--rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.1.5/fedops/client/test.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 04:00:33.816094 fedops-0.1.5/fedops/server/
--rw-r--r--   0 yangsemo   (501) staff       (20)      977 2023-05-23 03:35:26.000000 fedops-0.1.5/fedops/server/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     8874 2023-05-23 03:31:10.000000 fedops-0.1.5/fedops/server/app.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     1283 2023-05-22 17:11:45.000000 fedops-0.1.5/fedops/server/server_api.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     3229 2023-05-23 03:59:45.000000 fedops-0.1.5/fedops/server/server_utils.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 04:00:33.816579 fedops-0.1.5/fedops/utils/
--rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.1.5/fedops/utils/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)      832 2023-05-22 17:11:45.000000 fedops-0.1.5/fedops/utils/version.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 04:00:33.812465 fedops-0.1.5/fedops.egg-info/
--rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 04:00:33.000000 fedops-0.1.5/fedops.egg-info/PKG-INFO
--rw-r--r--   0 yangsemo   (501) staff       (20)      540 2023-05-23 04:00:33.000000 fedops-0.1.5/fedops.egg-info/SOURCES.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)        1 2023-05-23 04:00:33.000000 fedops-0.1.5/fedops.egg-info/dependency_links.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)      187 2023-05-23 04:00:33.000000 fedops-0.1.5/fedops.egg-info/requires.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)        7 2023-05-23 04:00:33.000000 fedops-0.1.5/fedops.egg-info/top_level.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)       38 2023-05-23 04:00:33.817374 fedops-0.1.5/setup.cfg
--rw-r--r--   0 yangsemo   (501) staff       (20)     1130 2023-05-23 04:00:12.000000 fedops-0.1.5/setup.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 04:15:37.012311 fedops-0.1.6/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 04:15:37.012137 fedops-0.1.6/PKG-INFO
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 04:15:37.008117 fedops-0.1.6/fedops/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      872 2023-05-23 02:14:46.000000 fedops-0.1.6/fedops/__init__.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 04:15:37.010611 fedops-0.1.6/fedops/client/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      987 2023-05-23 03:33:41.000000 fedops-0.1.6/fedops/client/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     7031 2023-05-23 03:33:41.000000 fedops-0.1.6/fedops/client/app.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     5010 2023-05-22 17:11:45.000000 fedops-0.1.6/fedops/client/app_test.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2817 2023-05-23 03:33:41.000000 fedops-0.1.6/fedops/client/client_api.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     6088 2023-05-23 04:15:04.000000 fedops-0.1.6/fedops/client/client_fl.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     3478 2023-05-23 03:34:07.000000 fedops-0.1.6/fedops/client/client_utils.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2238 2023-05-23 03:34:17.000000 fedops-0.1.6/fedops/client/client_wandb.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.1.6/fedops/client/test.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 04:15:37.011495 fedops-0.1.6/fedops/server/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      977 2023-05-23 03:35:26.000000 fedops-0.1.6/fedops/server/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     8874 2023-05-23 03:31:10.000000 fedops-0.1.6/fedops/server/app.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     1283 2023-05-22 17:11:45.000000 fedops-0.1.6/fedops/server/server_api.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     3229 2023-05-23 03:59:45.000000 fedops-0.1.6/fedops/server/server_utils.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 04:15:37.011827 fedops-0.1.6/fedops/utils/
+-rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.1.6/fedops/utils/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)      832 2023-05-22 17:11:45.000000 fedops-0.1.6/fedops/utils/version.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 04:15:37.008719 fedops-0.1.6/fedops.egg-info/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 04:15:36.000000 fedops-0.1.6/fedops.egg-info/PKG-INFO
+-rw-r--r--   0 yangsemo   (501) staff       (20)      540 2023-05-23 04:15:36.000000 fedops-0.1.6/fedops.egg-info/SOURCES.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)        1 2023-05-23 04:15:36.000000 fedops-0.1.6/fedops.egg-info/dependency_links.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)      187 2023-05-23 04:15:36.000000 fedops-0.1.6/fedops.egg-info/requires.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)        7 2023-05-23 04:15:36.000000 fedops-0.1.6/fedops.egg-info/top_level.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)       38 2023-05-23 04:15:37.012356 fedops-0.1.6/setup.cfg
+-rw-r--r--   0 yangsemo   (501) staff       (20)     1130 2023-05-23 04:15:17.000000 fedops-0.1.6/setup.py
```

### Comparing `fedops-0.1.5/PKG-INFO` & `fedops-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedops
-Version: 0.1.5
+Version: 0.1.6
 Summary: FL Lifecycle Operations Management Platform
 Home-page: https://github.com/gachon-CCLab/FedOps.git
 Author: Semo Yang
 Author-email: tpah20@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedops-0.1.5/fedops/__init__.py` & `fedops-0.1.6/fedops/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.5/fedops/client/__init__.py` & `fedops-0.1.6/fedops/client/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.5/fedops/client/app.py` & `fedops-0.1.6/fedops/client/app.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.5/fedops/client/app_test.py` & `fedops-0.1.6/fedops/client/app_test.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.5/fedops/client/client_api.py` & `fedops-0.1.6/fedops/client/client_api.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.5/fedops/client/client_fl.py` & `fedops-0.1.6/fedops/client/client_fl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json, logging
 
 import flwr as fl
 import time, os
 from functools import partial
 
 import tensorflow as tf
-import client_api
+from . import client_api
 
 # set log format
 handlers_list = [logging.StreamHandler()]
 
 # if os.environ["MONITORING"] == '1':
 #     handlers_list.append(logging.FileHandler('./fedops/fl_client.log'))
 # else:
```

### Comparing `fedops-0.1.5/fedops/client/client_utils.py` & `fedops-0.1.6/fedops/client/client_utils.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.5/fedops/client/client_wandb.py` & `fedops-0.1.6/fedops/client/client_wandb.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.5/fedops/server/__init__.py` & `fedops-0.1.6/fedops/server/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.5/fedops/server/app.py` & `fedops-0.1.6/fedops/server/app.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.5/fedops/server/server_api.py` & `fedops-0.1.6/fedops/server/server_api.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.5/fedops/server/server_utils.py` & `fedops-0.1.6/fedops/server/server_utils.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.5/fedops/utils/version.py` & `fedops-0.1.6/fedops/utils/version.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.5/fedops.egg-info/PKG-INFO` & `fedops-0.1.6/fedops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedops
-Version: 0.1.5
+Version: 0.1.6
 Summary: FL Lifecycle Operations Management Platform
 Home-page: https://github.com/gachon-CCLab/FedOps.git
 Author: Semo Yang
 Author-email: tpah20@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedops-0.1.5/fedops.egg-info/SOURCES.txt` & `fedops-0.1.6/fedops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fedops-0.1.5/setup.py` & `fedops-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fedops',
-    version='0.1.5',
+    version='0.1.6',
     author='Semo Yang',
     author_email='tpah20@gmail.com',
     description='FL Lifecycle Operations Management Platform',
     long_description='Long description of your library',
     url='https://github.com/gachon-CCLab/FedOps.git',
     packages=find_packages(),
     install_requires=[
```

