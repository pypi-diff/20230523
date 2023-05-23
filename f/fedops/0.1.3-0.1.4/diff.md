# Comparing `tmp/fedops-0.1.3.tar.gz` & `tmp/fedops-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedops-0.1.3.tar", last modified: Tue May 23 02:15:53 2023, max compression
+gzip compressed data, was "fedops-0.1.4.tar", last modified: Tue May 23 03:41:42 2023, max compression
```

## Comparing `fedops-0.1.3.tar` & `fedops-0.1.4.tar`

### file list

```diff
@@ -1,34 +1,29 @@
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 02:15:53.898847 fedops-0.1.3/
--rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 02:15:53.898721 fedops-0.1.3/PKG-INFO
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 02:15:53.894563 fedops-0.1.3/fedops/
--rw-r--r--   0 yangsemo   (501) staff       (20)      872 2023-05-23 02:14:46.000000 fedops-0.1.3/fedops/__init__.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 02:15:53.897200 fedops-0.1.3/fedops/client/
--rw-r--r--   0 yangsemo   (501) staff       (20)     1165 2023-05-23 02:13:21.000000 fedops-0.1.3/fedops/client/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     7003 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/client/app.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     5010 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/client/app_test.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2809 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/client/client_api.py
--rw-r--r--   0 yangsemo   (501) staff       (20)    12517 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/client/client_data.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     6073 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/client/client_fl.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2909 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/client/client_model.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2059 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/client/client_task.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     3574 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/client/client_utils.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2230 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/client/client_wandb.py
--rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/client/test.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 02:15:53.898299 fedops-0.1.3/fedops/server/
--rw-r--r--   0 yangsemo   (501) staff       (20)      961 2023-05-23 02:13:53.000000 fedops-0.1.3/fedops/server/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     8967 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/server/app.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2909 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/server/init_gl_model.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     1283 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/server/server_api.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2209 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/server/server_task.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     3715 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/server/server_utils.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 02:15:53.898523 fedops-0.1.3/fedops/utils/
--rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/utils/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)      832 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/utils/version.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 02:15:53.895278 fedops-0.1.3/fedops.egg-info/
--rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 02:15:53.000000 fedops-0.1.3/fedops.egg-info/PKG-INFO
--rw-r--r--   0 yangsemo   (501) staff       (20)      688 2023-05-23 02:15:53.000000 fedops-0.1.3/fedops.egg-info/SOURCES.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)        1 2023-05-23 02:15:53.000000 fedops-0.1.3/fedops.egg-info/dependency_links.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)      187 2023-05-23 02:15:53.000000 fedops-0.1.3/fedops.egg-info/requires.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)        7 2023-05-23 02:15:53.000000 fedops-0.1.3/fedops.egg-info/top_level.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)       38 2023-05-23 02:15:53.898887 fedops-0.1.3/setup.cfg
--rw-r--r--   0 yangsemo   (501) staff       (20)     1130 2023-05-23 02:14:13.000000 fedops-0.1.3/setup.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 03:41:42.301210 fedops-0.1.4/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 03:41:42.301071 fedops-0.1.4/PKG-INFO
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 03:41:42.297197 fedops-0.1.4/fedops/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      872 2023-05-23 02:14:46.000000 fedops-0.1.4/fedops/__init__.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 03:41:42.299643 fedops-0.1.4/fedops/client/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      987 2023-05-23 03:33:41.000000 fedops-0.1.4/fedops/client/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     7031 2023-05-23 03:33:41.000000 fedops-0.1.4/fedops/client/app.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     5010 2023-05-22 17:11:45.000000 fedops-0.1.4/fedops/client/app_test.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2817 2023-05-23 03:33:41.000000 fedops-0.1.4/fedops/client/client_api.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     6081 2023-05-23 03:33:41.000000 fedops-0.1.4/fedops/client/client_fl.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     3478 2023-05-23 03:34:07.000000 fedops-0.1.4/fedops/client/client_utils.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2238 2023-05-23 03:34:17.000000 fedops-0.1.4/fedops/client/client_wandb.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.1.4/fedops/client/test.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 03:41:42.300454 fedops-0.1.4/fedops/server/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      977 2023-05-23 03:35:26.000000 fedops-0.1.4/fedops/server/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     8874 2023-05-23 03:31:10.000000 fedops-0.1.4/fedops/server/app.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     1283 2023-05-22 17:11:45.000000 fedops-0.1.4/fedops/server/server_api.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     3226 2023-05-23 03:35:26.000000 fedops-0.1.4/fedops/server/server_utils.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 03:41:42.300749 fedops-0.1.4/fedops/utils/
+-rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.1.4/fedops/utils/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)      832 2023-05-22 17:11:45.000000 fedops-0.1.4/fedops/utils/version.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 03:41:42.297907 fedops-0.1.4/fedops.egg-info/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 03:41:42.000000 fedops-0.1.4/fedops.egg-info/PKG-INFO
+-rw-r--r--   0 yangsemo   (501) staff       (20)      540 2023-05-23 03:41:42.000000 fedops-0.1.4/fedops.egg-info/SOURCES.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)        1 2023-05-23 03:41:42.000000 fedops-0.1.4/fedops.egg-info/dependency_links.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)      187 2023-05-23 03:41:42.000000 fedops-0.1.4/fedops.egg-info/requires.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)        7 2023-05-23 03:41:42.000000 fedops-0.1.4/fedops.egg-info/top_level.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)       38 2023-05-23 03:41:42.301255 fedops-0.1.4/setup.cfg
+-rw-r--r--   0 yangsemo   (501) staff       (20)     1130 2023-05-23 03:35:51.000000 fedops-0.1.4/setup.py
```

### Comparing `fedops-0.1.3/PKG-INFO` & `fedops-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedops
-Version: 0.1.3
+Version: 0.1.4
 Summary: FL Lifecycle Operations Management Platform
 Home-page: https://github.com/gachon-CCLab/FedOps.git
 Author: Semo Yang
 Author-email: tpah20@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedops-0.1.3/fedops/__init__.py` & `fedops-0.1.4/fedops/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.3/fedops/client/app.py` & `fedops-0.1.4/fedops/client/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging, json
 import time
-
 from fastapi import FastAPI, BackgroundTasks
 import asyncio
 import uvicorn
-import client_utils
-import client_fl
-import client_wandb
-import client_api
 from datetime import datetime
 
+from . import client_utils
+from . import client_fl
+from . import client_wandb
+from . import client_api
+
 class FLClientTask():
     def __init__(self, config, fl_task):
         self.app = FastAPI()
         
         self.x_train = fl_task[0]
         self.x_test = fl_task[1]
         self.y_train = fl_task[2]
```

### Comparing `fedops-0.1.3/fedops/client/app_test.py` & `fedops-0.1.4/fedops/client/app_test.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.3/fedops/client/client_api.py` & `fedops-0.1.4/fedops/client/client_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import requests
 import sys
 import logging, os
 
 # set log format
 handlers_list = [logging.StreamHandler()]
 
-if os.environ["MONITORING"] == '1':
-    handlers_list.append(logging.FileHandler('./fedops/fl_client.log'))
-else:
-    pass
+# if os.environ["MONITORING"] == '1':
+#     handlers_list.append(logging.FileHandler('./fedops/fl_client.log'))
+# else:
+#     pass
 
 logging.basicConfig(level=logging.DEBUG, format="%(asctime)s [%(levelname)8.8s] %(message)s",
                     handlers=handlers_list)
 
 logger = logging.getLogger(__name__)
 
 class ClientMangerAPI():
```

### Comparing `fedops-0.1.3/fedops/client/client_fl.py` & `fedops-0.1.4/fedops/client/client_fl.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 import tensorflow as tf
 import client_api
 
 # set log format
 handlers_list = [logging.StreamHandler()]
 
-if os.environ["MONITORING"] == '1':
-    handlers_list.append(logging.FileHandler('./fedops/fl_client.log'))
-else:
-    pass
+# if os.environ["MONITORING"] == '1':
+#     handlers_list.append(logging.FileHandler('./fedops/fl_client.log'))
+# else:
+#     pass
 
 logging.basicConfig(level=logging.DEBUG, format="%(asctime)s [%(levelname)8.8s] %(message)s",
                     handlers=handlers_list)
 
 logger = logging.getLogger(__name__)
```

### Comparing `fedops-0.1.3/fedops/client/client_utils.py` & `fedops-0.1.4/fedops/client/client_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 import asyncio
 import os
-from collections import Counter
-from typing import Optional, Union
-
 import requests
-import torch
-from pydantic.main import BaseModel, BaseConfig
+from pydantic.main import BaseModel
 import re
 import tensorflow as tf
 import logging
 import yaml, uuid, socket
-import client_api
-import numpy as np
+
+from . import client_api
 
 # set log format
 handlers_list = [logging.StreamHandler()]
 
-if os.environ["MONITORING"] == '1':
-    handlers_list.append(logging.FileHandler('./fedops/fl_client.log'))
-else:
-    pass
+# if os.environ["MONITORING"] == '1':
+#     handlers_list.append(logging.FileHandler('./fedops/fl_client.log'))
+# else:
+#     pass
 
 logging.basicConfig(level=logging.DEBUG, format="%(asctime)s [%(levelname)8.8s] %(message)s",
                     handlers=handlers_list)
 
 logger = logging.getLogger(__name__)
```

### Comparing `fedops-0.1.3/fedops/client/client_wandb.py` & `fedops-0.1.4/fedops/client/client_wandb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import wandb
-import client_api
+
+from . import client_api
 
 
 def start_wandb(wandb_key, task_id, wandb_name):
     wandb.login(key=wandb_key)
     config_wandb = {
         "learning_rate": 0,
         "optimizer": '',
```

### Comparing `fedops-0.1.3/fedops/server/__init__.py` & `fedops-0.1.4/fedops/server/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,18 +14,16 @@
 # ==============================================================================
 """FedOps Server."""
 
 # from .app import FLServer
 # from .server_api import ServerAPI
 # from .server_utils import FLServerStatus
 
-import app
-import init_gl_model
-import server_utils
-import server_api
+from . import app as app
+from . import server_utils as server_utlis
+from . import server_api as server_api
 
 __all__ = [
     "app",
-    "init_gl_model",
     "server_utils",
     "server_api",
 ]
```

### Comparing `fedops-0.1.3/fedops/server/app.py` & `fedops-0.1.4/fedops/server/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,16 @@
-# https://github.com/adap/flower/tree/main/examples/advanced_tensorflow 참조
-
 import logging
 from typing import Dict, Optional, Tuple
-
 import flwr as fl
-
-
 import datetime
 import os
-import requests, json
+import json
 import time
-
-import server_api
-import server_utils, server_task
+from . import server_api
+from . import server_utils
 
 # TF warning log filtering
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
 
 logging.basicConfig(level=logging.DEBUG, format="%(asctime)s [%(levelname)8.8s] %(message)s",
                     handlers=[logging.StreamHandler()])
 logger = logging.getLogger(__name__)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fedops-0.1.3/fedops/server/server_api.py` & `fedops-0.1.4/fedops/server/server_api.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.3/fedops/server/server_utils.py` & `fedops-0.1.4/fedops/server/server_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import yaml
 import boto3
 import os, logging, re
 import tensorflow as tf
-# from dotenv import load_dotenv
 
 # FL Server Status Class
 class FLServerStatus:
     latest_gl_model_v = 0  # Previous Global Model Version
     next_gl_model_v = 0  # Global model version to be created
     start_by_round = 0  # fit aggregation start
     end_by_round = 0  # fit aggregation end
@@ -17,27 +16,22 @@
     # Read the YAML configuration file
     config_file_path = './config.yaml'
     with open(config_file_path, 'r') as file:
         config = yaml.safe_load(file)
     return config
 
 
-# load_dotenv()
-# 참고: https://loosie.tistory.com/210, https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html
-# aws session 연결
+# Connect aws session
 def aws_session(region_name='ap-northeast-2'):
     return boto3.session.Session(aws_access_key_id=os.environ.get('ACCESS_KEY_ID'),
                                  aws_secret_access_key=os.environ.get('ACCESS_SECRET_KEY'),
                                  region_name=region_name)
-# def aws_session(region_name='ap-northeast-2'):
-#     return boto3.session.Session(aws_access_key_id=os.getenv('ACCESS_KEY_ID'),
-#                                  aws_secret_access_key=os.getenv('ACCESS_SECRET_KEY'),
-#                                  region_name=region_name)
 
-# s3에 global model upload
+
+# Global model upload in S3
 def upload_model_to_bucket(task_id, global_model_name):
     bucket_name = os.environ.get('BUCKET_NAME')
     # bucket_name = os.getenv('BUCKET_NAME')
 
     # logging.info(f'Upload {global_model_name}')
 
     session = aws_session()
@@ -88,15 +82,15 @@
         gl_model_save_path = f'/app/{latest_gl_model_file}'
         s3_resource.download_file(bucket_name, gl_model_path, gl_model_save_path)
 
         gl_model = tf.keras.models.load_model(gl_model_save_path)
 
         return gl_model, gl_model_name, gl_model_version
 
-    # s3에 global model 없을 경우
+
     except Exception as e:
         logging.error('No read global model')
         gl_model = None
         gl_model_name = None
         gl_model_version=0
         logging.info(f'gl_model: {gl_model}, gl_model_v: {gl_model_version}')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fedops-0.1.3/fedops/utils/version.py` & `fedops-0.1.4/fedops/utils/version.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.3/fedops.egg-info/PKG-INFO` & `fedops-0.1.4/fedops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedops
-Version: 0.1.3
+Version: 0.1.4
 Summary: FL Lifecycle Operations Management Platform
 Home-page: https://github.com/gachon-CCLab/FedOps.git
 Author: Semo Yang
 Author-email: tpah20@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedops-0.1.3/fedops.egg-info/SOURCES.txt` & `fedops-0.1.4/fedops.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,22 +5,17 @@
 fedops.egg-info/dependency_links.txt
 fedops.egg-info/requires.txt
 fedops.egg-info/top_level.txt
 fedops/client/__init__.py
 fedops/client/app.py
 fedops/client/app_test.py
 fedops/client/client_api.py
-fedops/client/client_data.py
 fedops/client/client_fl.py
-fedops/client/client_model.py
-fedops/client/client_task.py
 fedops/client/client_utils.py
 fedops/client/client_wandb.py
 fedops/client/test.py
 fedops/server/__init__.py
 fedops/server/app.py
-fedops/server/init_gl_model.py
 fedops/server/server_api.py
-fedops/server/server_task.py
 fedops/server/server_utils.py
 fedops/utils/__init__.py
 fedops/utils/version.py
```

### Comparing `fedops-0.1.3/setup.py` & `fedops-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fedops',
-    version='0.1.3',
+    version='0.1.4',
     author='Semo Yang',
     author_email='tpah20@gmail.com',
     description='FL Lifecycle Operations Management Platform',
     long_description='Long description of your library',
     url='https://github.com/gachon-CCLab/FedOps.git',
     packages=find_packages(),
     install_requires=[
```

