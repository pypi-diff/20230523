# Comparing `tmp/fedops-0.1.8.tar.gz` & `tmp/fedops-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedops-0.1.8.tar", last modified: Tue May 23 05:13:23 2023, max compression
+gzip compressed data, was "fedops-0.1.9.tar", last modified: Tue May 23 05:51:02 2023, max compression
```

## Comparing `fedops-0.1.8.tar` & `fedops-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:13:23.465133 fedops-0.1.8/
--rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 05:13:23.464970 fedops-0.1.8/PKG-INFO
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:13:23.460924 fedops-0.1.8/fedops/
--rw-r--r--   0 yangsemo   (501) staff       (20)      872 2023-05-23 04:42:21.000000 fedops-0.1.8/fedops/__init__.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:13:23.463579 fedops-0.1.8/fedops/client/
--rw-r--r--   0 yangsemo   (501) staff       (20)      987 2023-05-23 04:42:21.000000 fedops-0.1.8/fedops/client/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     7031 2023-05-23 04:42:21.000000 fedops-0.1.8/fedops/client/app.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     5010 2023-05-22 17:11:45.000000 fedops-0.1.8/fedops/client/app_test.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2817 2023-05-23 04:42:21.000000 fedops-0.1.8/fedops/client/client_api.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     6088 2023-05-23 04:42:21.000000 fedops-0.1.8/fedops/client/client_fl.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     3478 2023-05-23 04:42:21.000000 fedops-0.1.8/fedops/client/client_utils.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2238 2023-05-23 04:42:21.000000 fedops-0.1.8/fedops/client/client_wandb.py
--rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.1.8/fedops/client/test.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:13:23.464375 fedops-0.1.8/fedops/server/
--rw-r--r--   0 yangsemo   (501) staff       (20)      977 2023-05-23 04:42:21.000000 fedops-0.1.8/fedops/server/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     8969 2023-05-23 05:09:34.000000 fedops-0.1.8/fedops/server/app.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     1283 2023-05-22 17:11:45.000000 fedops-0.1.8/fedops/server/server_api.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     3229 2023-05-23 04:42:21.000000 fedops-0.1.8/fedops/server/server_utils.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:13:23.464630 fedops-0.1.8/fedops/utils/
--rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.1.8/fedops/utils/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)      832 2023-05-22 17:11:45.000000 fedops-0.1.8/fedops/utils/version.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:13:23.461800 fedops-0.1.8/fedops.egg-info/
--rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 05:13:23.000000 fedops-0.1.8/fedops.egg-info/PKG-INFO
--rw-r--r--   0 yangsemo   (501) staff       (20)      540 2023-05-23 05:13:23.000000 fedops-0.1.8/fedops.egg-info/SOURCES.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)        1 2023-05-23 05:13:23.000000 fedops-0.1.8/fedops.egg-info/dependency_links.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)      187 2023-05-23 05:13:23.000000 fedops-0.1.8/fedops.egg-info/requires.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)        7 2023-05-23 05:13:23.000000 fedops-0.1.8/fedops.egg-info/top_level.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)       38 2023-05-23 05:13:23.465176 fedops-0.1.8/setup.cfg
--rw-r--r--   0 yangsemo   (501) staff       (20)     1130 2023-05-23 05:12:56.000000 fedops-0.1.8/setup.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:51:02.725041 fedops-0.1.9/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 05:51:02.724887 fedops-0.1.9/PKG-INFO
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:51:02.720565 fedops-0.1.9/fedops/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      872 2023-05-23 04:42:21.000000 fedops-0.1.9/fedops/__init__.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:51:02.723378 fedops-0.1.9/fedops/client/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      987 2023-05-23 04:42:21.000000 fedops-0.1.9/fedops/client/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     6957 2023-05-23 05:45:41.000000 fedops-0.1.9/fedops/client/app.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     5010 2023-05-22 17:11:45.000000 fedops-0.1.9/fedops/client/app_test.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2817 2023-05-23 04:42:21.000000 fedops-0.1.9/fedops/client/client_api.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     6088 2023-05-23 04:42:21.000000 fedops-0.1.9/fedops/client/client_fl.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     3478 2023-05-23 04:42:21.000000 fedops-0.1.9/fedops/client/client_utils.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2533 2023-05-23 05:49:05.000000 fedops-0.1.9/fedops/client/client_wandb.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.1.9/fedops/client/test.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:51:02.724295 fedops-0.1.9/fedops/server/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      977 2023-05-23 04:42:21.000000 fedops-0.1.9/fedops/server/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     8963 2023-05-23 05:44:14.000000 fedops-0.1.9/fedops/server/app.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     1283 2023-05-22 17:11:45.000000 fedops-0.1.9/fedops/server/server_api.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     3229 2023-05-23 04:42:21.000000 fedops-0.1.9/fedops/server/server_utils.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:51:02.724573 fedops-0.1.9/fedops/utils/
+-rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.1.9/fedops/utils/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)      832 2023-05-22 17:11:45.000000 fedops-0.1.9/fedops/utils/version.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:51:02.721562 fedops-0.1.9/fedops.egg-info/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 05:51:02.000000 fedops-0.1.9/fedops.egg-info/PKG-INFO
+-rw-r--r--   0 yangsemo   (501) staff       (20)      540 2023-05-23 05:51:02.000000 fedops-0.1.9/fedops.egg-info/SOURCES.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)        1 2023-05-23 05:51:02.000000 fedops-0.1.9/fedops.egg-info/dependency_links.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)      187 2023-05-23 05:51:02.000000 fedops-0.1.9/fedops.egg-info/requires.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)        7 2023-05-23 05:51:02.000000 fedops-0.1.9/fedops.egg-info/top_level.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)       38 2023-05-23 05:51:02.725083 fedops-0.1.9/setup.cfg
+-rw-r--r--   0 yangsemo   (501) staff       (20)     1130 2023-05-23 05:49:15.000000 fedops-0.1.9/setup.py
```

### Comparing `fedops-0.1.8/PKG-INFO` & `fedops-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedops
-Version: 0.1.8
+Version: 0.1.9
 Summary: FL Lifecycle Operations Management Platform
 Home-page: https://github.com/gachon-CCLab/FedOps.git
 Author: Semo Yang
 Author-email: tpah20@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedops-0.1.8/fedops/__init__.py` & `fedops-0.1.9/fedops/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.8/fedops/client/__init__.py` & `fedops-0.1.9/fedops/client/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.8/fedops/client/app.py` & `fedops-0.1.9/fedops/client/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,17 +94,14 @@
             # Send client_time_result to client_performance pod
             client_api.ClientServerAPI(self.task_id).put_client_time_result(json_result)
 
             # Get client system result from wandb and send it to client_performance pod
             client_wandb.client_system_wandb(self.task_id, self.status.FL_client_mac, self.status.FL_next_gl_model,
                                              wandb_name, self.wandb_account)
 
-            # Close wandb
-            client_wandb.client_finish_wandb()
-
             # Delete client object
             del client
 
             # Complete Client training
             self.status.FL_client_start = await client_utils.notify_fin()
             logging.info('FL Client Learning Finish')
```

### Comparing `fedops-0.1.8/fedops/client/app_test.py` & `fedops-0.1.9/fedops/client/app_test.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.8/fedops/client/client_api.py` & `fedops-0.1.9/fedops/client/client_api.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.8/fedops/client/client_fl.py` & `fedops-0.1.9/fedops/client/client_fl.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.8/fedops/client/client_utils.py` & `fedops-0.1.9/fedops/client/client_utils.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.8/fedops/client/client_wandb.py` & `fedops-0.1.9/fedops/client/client_wandb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import logging
+import time
+
 import wandb
 
 from . import client_api
 
 
 def start_wandb(wandb_key, task_id, wandb_name):
     wandb.login(key=wandb_key)
@@ -21,47 +24,53 @@
 
 def data_status_wandb(run, labels):
     table = wandb.Table(data=labels, columns=["label", "data_size"])
     run.log({'Data Lable Histogram': wandb.plot.bar(table, "label", "data_size", title="Data Size Distribution")})
 
 
 def client_system_wandb(fl_task_id, client_mac, next_gl_model_v, wandb_name, wandb_account):
+    try:
+        time.sleep(2)
 
-    # check client system resource usage from wandb
-    api = wandb.Api()
-    runs = api.runs(f"{wandb_account}/{fl_task_id}")
-
-    sys_df = runs[0].history(stream="system")
-
-    col = ['system.network.sent', 'system.network.recv', 'system.disk', '_runtime', 'system.proc.memory.rssMB','system.proc.memory.availableMB', 'system.cpu', 'system.proc.cpu.threads', 'system.memory', 'system.proc.memory.percent', '_timestamp']
-
-    sys_df = sys_df[col]
-
-    sys_df.rename(columns={
-        "system.network.sent": "network_sent",
-        "system.network.recv": "network_recv",
-        "system.disk": "disk",
-        "_runtime": "runtime",
-        "system.proc.memory.rssMB": "memory_rssMB",
-        "system.proc.memory.availableMB": "memory_availableMB",
-        "system.cpu": "cpu",
-        "system.proc.cpu.threads": "cpu_threads",
-        "system.memory": "memory",
-        "system.proc.memory.percent": "memory_percent",
-        "_timestamp": "timestamp",
-    }, inplace=True)
-
-    # Extract df_row by row
-    for i in range(len(sys_df)):
-        sys_df_row = sys_df.iloc[i]
-        sys_df_row['fl_task_id'] = fl_task_id
-        sys_df_row['client_mac'] = client_mac
-        sys_df_row['next_gl_model_v'] = next_gl_model_v
-        sys_df_row['wandb_name'] = wandb_name
-
-        sys_df_row_json = sys_df_row.to_json()
-
-        # send client_system  to client_performance pod
-        client_api.ClientServerAPI(fl_task_id).put_client_system(sys_df_row_json)
-
-def client_finish_wandb():
-    wandb.finish()
+        # check client system resource usage from wandb
+        api = wandb.Api()
+        runs = api.runs(f"{wandb_account}/{fl_task_id}")
+
+        sys_df = runs[0].history(stream="system")
+
+        col = ['system.network.sent', 'system.network.recv', 'system.disk', '_runtime', 'system.proc.memory.rssMB','system.proc.memory.availableMB', 'system.cpu', 'system.proc.cpu.threads', 'system.memory', 'system.proc.memory.percent', '_timestamp']
+
+        sys_df = sys_df[col]
+
+        sys_df.rename(columns={
+            "system.network.sent": "network_sent",
+            "system.network.recv": "network_recv",
+            "system.disk": "disk",
+            "_runtime": "runtime",
+            "system.proc.memory.rssMB": "memory_rssMB",
+            "system.proc.memory.availableMB": "memory_availableMB",
+            "system.cpu": "cpu",
+            "system.proc.cpu.threads": "cpu_threads",
+            "system.memory": "memory",
+            "system.proc.memory.percent": "memory_percent",
+            "_timestamp": "timestamp",
+        }, inplace=True)
+
+        # Extract df_row by row
+        for i in range(len(sys_df)):
+            sys_df_row = sys_df.iloc[i]
+            sys_df_row['fl_task_id'] = fl_task_id
+            sys_df_row['client_mac'] = client_mac
+            sys_df_row['next_gl_model_v'] = next_gl_model_v
+            sys_df_row['wandb_name'] = wandb_name
+
+            sys_df_row_json = sys_df_row.to_json()
+
+            # send client_system  to client_performance pod
+            client_api.ClientServerAPI(fl_task_id).put_client_system(sys_df_row_json)
+
+        # close wandb
+        wandb.finish()
+
+    except Exception as e:
+        logging.error(f'wandb system load error: {e}')
+        wandb.finish() # close wandb
```

### Comparing `fedops-0.1.8/fedops/server/__init__.py` & `fedops-0.1.9/fedops/server/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.8/fedops/server/app.py` & `fedops-0.1.9/fedops/server/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,16 +124,14 @@
 
 
     def fit_config(self, rnd: int):
         """Return training configuration dict for each round.
         Keep batch size fixed at 32, perform two rounds of training with one
         local epoch, increase to two local epochs afterwards.
         """
-
-
         fl_config = {
             "batch_size": self.batch_size,
             "local_epochs": self.local_epochs,
             "num_rounds": self.num_rounds,
         }
 
         # increase round
@@ -200,15 +198,15 @@
 
             # upload global model
             global_model_file_name = f"{gl_model_name}_gl_model_V{self.server.next_gl_model_v}.h5"
             server_utils.upload_model_to_bucket(self.task_id, global_model_file_name)
 
             logging.info(f'upload {global_model_file_name} model in s3')
 
-            # server_status error
+        # server_status error
         except Exception as e:
             logging.error('error: ', e)
             data_inform = {'FLSeReady': False}
             server_api.ServerAPI(self.task_id).put_server_status(json.dumps(data_inform))
 
         finally:
             logging.info('server close')
```

### Comparing `fedops-0.1.8/fedops/server/server_api.py` & `fedops-0.1.9/fedops/server/server_api.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.8/fedops/server/server_utils.py` & `fedops-0.1.9/fedops/server/server_utils.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.8/fedops/utils/version.py` & `fedops-0.1.9/fedops/utils/version.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.8/fedops.egg-info/PKG-INFO` & `fedops-0.1.9/fedops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedops
-Version: 0.1.8
+Version: 0.1.9
 Summary: FL Lifecycle Operations Management Platform
 Home-page: https://github.com/gachon-CCLab/FedOps.git
 Author: Semo Yang
 Author-email: tpah20@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedops-0.1.8/fedops.egg-info/SOURCES.txt` & `fedops-0.1.9/fedops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fedops-0.1.8/setup.py` & `fedops-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fedops',
-    version='0.1.8',
+    version='0.1.9',
     author='Semo Yang',
     author_email='tpah20@gmail.com',
     description='FL Lifecycle Operations Management Platform',
     long_description='Long description of your library',
     url='https://github.com/gachon-CCLab/FedOps.git',
     packages=find_packages(),
     install_requires=[
```

