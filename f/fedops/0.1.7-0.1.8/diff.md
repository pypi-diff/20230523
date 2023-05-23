# Comparing `tmp/fedops-0.1.7.tar.gz` & `tmp/fedops-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedops-0.1.7.tar", last modified: Tue May 23 04:20:17 2023, max compression
+gzip compressed data, was "fedops-0.1.8.tar", last modified: Tue May 23 05:13:23 2023, max compression
```

## Comparing `fedops-0.1.7.tar` & `fedops-0.1.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 04:20:17.383427 fedops-0.1.7/
--rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 04:20:17.383275 fedops-0.1.7/PKG-INFO
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 04:20:17.379364 fedops-0.1.7/fedops/
--rw-r--r--   0 yangsemo   (501) staff       (20)      872 2023-05-23 02:14:46.000000 fedops-0.1.7/fedops/__init__.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 04:20:17.381647 fedops-0.1.7/fedops/client/
--rw-r--r--   0 yangsemo   (501) staff       (20)      987 2023-05-23 03:33:41.000000 fedops-0.1.7/fedops/client/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     7031 2023-05-23 03:33:41.000000 fedops-0.1.7/fedops/client/app.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     5010 2023-05-22 17:11:45.000000 fedops-0.1.7/fedops/client/app_test.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2817 2023-05-23 03:33:41.000000 fedops-0.1.7/fedops/client/client_api.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     6088 2023-05-23 04:15:04.000000 fedops-0.1.7/fedops/client/client_fl.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     3478 2023-05-23 03:34:07.000000 fedops-0.1.7/fedops/client/client_utils.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2238 2023-05-23 03:34:17.000000 fedops-0.1.7/fedops/client/client_wandb.py
--rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.1.7/fedops/client/test.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 04:20:17.382544 fedops-0.1.7/fedops/server/
--rw-r--r--   0 yangsemo   (501) staff       (20)      977 2023-05-23 04:19:10.000000 fedops-0.1.7/fedops/server/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     8874 2023-05-23 03:31:10.000000 fedops-0.1.7/fedops/server/app.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     1283 2023-05-22 17:11:45.000000 fedops-0.1.7/fedops/server/server_api.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     3229 2023-05-23 03:59:45.000000 fedops-0.1.7/fedops/server/server_utils.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 04:20:17.382974 fedops-0.1.7/fedops/utils/
--rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.1.7/fedops/utils/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)      832 2023-05-22 17:11:45.000000 fedops-0.1.7/fedops/utils/version.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 04:20:17.379958 fedops-0.1.7/fedops.egg-info/
--rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 04:20:17.000000 fedops-0.1.7/fedops.egg-info/PKG-INFO
--rw-r--r--   0 yangsemo   (501) staff       (20)      540 2023-05-23 04:20:17.000000 fedops-0.1.7/fedops.egg-info/SOURCES.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)        1 2023-05-23 04:20:17.000000 fedops-0.1.7/fedops.egg-info/dependency_links.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)      187 2023-05-23 04:20:17.000000 fedops-0.1.7/fedops.egg-info/requires.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)        7 2023-05-23 04:20:17.000000 fedops-0.1.7/fedops.egg-info/top_level.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)       38 2023-05-23 04:20:17.383468 fedops-0.1.7/setup.cfg
--rw-r--r--   0 yangsemo   (501) staff       (20)     1130 2023-05-23 04:19:20.000000 fedops-0.1.7/setup.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:13:23.465133 fedops-0.1.8/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 05:13:23.464970 fedops-0.1.8/PKG-INFO
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:13:23.460924 fedops-0.1.8/fedops/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      872 2023-05-23 04:42:21.000000 fedops-0.1.8/fedops/__init__.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:13:23.463579 fedops-0.1.8/fedops/client/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      987 2023-05-23 04:42:21.000000 fedops-0.1.8/fedops/client/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     7031 2023-05-23 04:42:21.000000 fedops-0.1.8/fedops/client/app.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     5010 2023-05-22 17:11:45.000000 fedops-0.1.8/fedops/client/app_test.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2817 2023-05-23 04:42:21.000000 fedops-0.1.8/fedops/client/client_api.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     6088 2023-05-23 04:42:21.000000 fedops-0.1.8/fedops/client/client_fl.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     3478 2023-05-23 04:42:21.000000 fedops-0.1.8/fedops/client/client_utils.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2238 2023-05-23 04:42:21.000000 fedops-0.1.8/fedops/client/client_wandb.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.1.8/fedops/client/test.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:13:23.464375 fedops-0.1.8/fedops/server/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      977 2023-05-23 04:42:21.000000 fedops-0.1.8/fedops/server/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     8969 2023-05-23 05:09:34.000000 fedops-0.1.8/fedops/server/app.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     1283 2023-05-22 17:11:45.000000 fedops-0.1.8/fedops/server/server_api.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     3229 2023-05-23 04:42:21.000000 fedops-0.1.8/fedops/server/server_utils.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:13:23.464630 fedops-0.1.8/fedops/utils/
+-rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.1.8/fedops/utils/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)      832 2023-05-22 17:11:45.000000 fedops-0.1.8/fedops/utils/version.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:13:23.461800 fedops-0.1.8/fedops.egg-info/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 05:13:23.000000 fedops-0.1.8/fedops.egg-info/PKG-INFO
+-rw-r--r--   0 yangsemo   (501) staff       (20)      540 2023-05-23 05:13:23.000000 fedops-0.1.8/fedops.egg-info/SOURCES.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)        1 2023-05-23 05:13:23.000000 fedops-0.1.8/fedops.egg-info/dependency_links.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)      187 2023-05-23 05:13:23.000000 fedops-0.1.8/fedops.egg-info/requires.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)        7 2023-05-23 05:13:23.000000 fedops-0.1.8/fedops.egg-info/top_level.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)       38 2023-05-23 05:13:23.465176 fedops-0.1.8/setup.cfg
+-rw-r--r--   0 yangsemo   (501) staff       (20)     1130 2023-05-23 05:12:56.000000 fedops-0.1.8/setup.py
```

### Comparing `fedops-0.1.7/PKG-INFO` & `fedops-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedops
-Version: 0.1.7
+Version: 0.1.8
 Summary: FL Lifecycle Operations Management Platform
 Home-page: https://github.com/gachon-CCLab/FedOps.git
 Author: Semo Yang
 Author-email: tpah20@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedops-0.1.7/fedops/__init__.py` & `fedops-0.1.8/fedops/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.7/fedops/client/__init__.py` & `fedops-0.1.8/fedops/client/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.7/fedops/client/app.py` & `fedops-0.1.8/fedops/client/app.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.7/fedops/client/app_test.py` & `fedops-0.1.8/fedops/client/app_test.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.7/fedops/client/client_api.py` & `fedops-0.1.8/fedops/client/client_api.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.7/fedops/client/client_fl.py` & `fedops-0.1.8/fedops/client/client_fl.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.7/fedops/client/client_utils.py` & `fedops-0.1.8/fedops/client/client_utils.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.7/fedops/client/client_wandb.py` & `fedops-0.1.8/fedops/client/client_wandb.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.7/fedops/server/__init__.py` & `fedops-0.1.8/fedops/server/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.7/fedops/server/app.py` & `fedops-0.1.8/fedops/server/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,41 +13,45 @@
 
 logging.basicConfig(level=logging.DEBUG, format="%(asctime)s [%(levelname)8.8s] %(message)s",
                     handlers=[logging.StreamHandler()])
 logger = logging.getLogger(__name__)
 
 
 class FLServer():
-    def __init__(self, config):
+    def __init__(self, config, model, model_name, x_val, y_val):
         self.task_id = os.environ.get('TASK_ID') # Set FL Task ID
         self.server = server_utils.FLServerStatus() # Set FLServerStatus class
         self.dataset = config['data']['name']
         self.fraction_fit = float(config['aggregation']['fedAvg']['fraction_fit'])
         self.fraction_evaluate = float(config['aggregation']['fedAvg']['fraction_evaluate'])
         self.min_fit_clients = int(config['aggregation']['fedAvg']['min_fit_clients'])
         self.min_evaluate_clients = int(config['aggregation']['fedAvg']['min_evaluate_clients'])
         self.min_available_clients = int(config['aggregation']['fedAvg']['min_available_clients'])
 
         self.batch_size = int(config['fl_server']['batch_size'])
         self.local_epochs = int(config['fl_server']['local_epochs'])
         self.num_rounds = int(config['fl_server']['num_rounds'])
         self.val_steps = int(config['fl_server']['val_steps'])
 
-        self.x_val = None
-        self.y_val = None
+        self.init_model = model
+        self.init_model_name = model_name
+        self.next_model = None
+        self.next_model_name = None
+        self.x_val = x_val
+        self.y_val = y_val
 
 
 
     def init_gl_model_registration(self, model, gl_model_name) -> None:
         logging.info(f'latest_gl_model_v: {self.server.latest_gl_model_v}')
 
         if not model:
 
             logging.info('init global model making')
-            init_model, model_name = server_task.build_gl_model(self.dataset)
+            init_model, model_name = self.init_model, self.init_model_name
             print(f'init_gl_model_name: {model_name}')
 
             self.fl_server_start(init_model, model_name)
             return model_name
 
 
         else:
@@ -59,16 +63,14 @@
 
 
     def fl_server_start(self, model, model_name):
         # Load and compile model for
         # 1. server-side parameter initialization
         # 2. server-side parameter evaluation
 
-
-
         strategy = fl.server.strategy.FedAvg(
             fraction_fit=self.fraction_fit,
             fraction_evaluate=self.fraction_evaluate,
             min_fit_clients=self.min_fit_clients,
             min_evaluate_clients=self.min_evaluate_clients,
             min_available_clients=self.min_available_clients,
             evaluate_fn=self.get_eval_fn(model, model_name),
@@ -151,26 +153,24 @@
         batches) during rounds one to three, then increase to ten local
         evaluation steps.
         """
 
         return {"val_steps": self.val_steps}
 
     def start(self):
-        # Load dataset for evaluating gl model
-        self.x_val, self.y_val = server_task.load_data(self.dataset)
 
         today = datetime.datetime.today()
         today_time = today.strftime('%Y-%m-%d %H-%M-%S')
 
         # global model init
         # model = None
         # server.latest_gl_model_v = 0
 
         # Loaded latest global model or no global model
-        model, model_name, self.server.latest_gl_model_v = server_utils.model_download(self.task_id)
+        self.next_model, self.next_model_name, self.server.latest_gl_model_v = server_utils.model_download(self.task_id)
         # logging.info('Loaded latest global model or no global model')
 
         # New Global Model Version
         self.server.next_gl_model_v = self.server.latest_gl_model_v + 1
 
         # API that sends server status to server manager
         inform_Payload = {
@@ -183,15 +183,15 @@
         server_status_json = json.dumps(inform_Payload)
         server_api.ServerAPI(self.task_id).put_server_status(server_status_json)
 
         try:
             fl_start_time = time.time()
 
             # Run fl server
-            gl_model_name = self.init_gl_model_registration(model, model_name)
+            gl_model_name = self.init_gl_model_registration(self.next_model, self.next_model_name)
 
             fl_end_time = time.time() - fl_start_time  # FL end time
 
             server_all_time_result = {"fl_task_id": self.task_id, "server_operation_time": fl_end_time,
                                       "next_gl_model_v": self.server.next_gl_model_v}
             json_all_time_result = json.dumps(server_all_time_result)
             logging.info(f'server_operation_time - {json_all_time_result}')
```

### Comparing `fedops-0.1.7/fedops/server/server_api.py` & `fedops-0.1.8/fedops/server/server_api.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.7/fedops/server/server_utils.py` & `fedops-0.1.8/fedops/server/server_utils.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.7/fedops/utils/version.py` & `fedops-0.1.8/fedops/utils/version.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.7/fedops.egg-info/PKG-INFO` & `fedops-0.1.8/fedops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedops
-Version: 0.1.7
+Version: 0.1.8
 Summary: FL Lifecycle Operations Management Platform
 Home-page: https://github.com/gachon-CCLab/FedOps.git
 Author: Semo Yang
 Author-email: tpah20@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedops-0.1.7/fedops.egg-info/SOURCES.txt` & `fedops-0.1.8/fedops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fedops-0.1.7/setup.py` & `fedops-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fedops',
-    version='0.1.7',
+    version='0.1.8',
     author='Semo Yang',
     author_email='tpah20@gmail.com',
     description='FL Lifecycle Operations Management Platform',
     long_description='Long description of your library',
     url='https://github.com/gachon-CCLab/FedOps.git',
     packages=find_packages(),
     install_requires=[
```

