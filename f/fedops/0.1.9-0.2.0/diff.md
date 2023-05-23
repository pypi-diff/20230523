# Comparing `tmp/fedops-0.1.9.tar.gz` & `tmp/fedops-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedops-0.1.9.tar", last modified: Tue May 23 05:51:02 2023, max compression
+gzip compressed data, was "fedops-0.2.0.tar", last modified: Tue May 23 06:11:38 2023, max compression
```

## Comparing `fedops-0.1.9.tar` & `fedops-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:51:02.725041 fedops-0.1.9/
--rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 05:51:02.724887 fedops-0.1.9/PKG-INFO
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:51:02.720565 fedops-0.1.9/fedops/
--rw-r--r--   0 yangsemo   (501) staff       (20)      872 2023-05-23 04:42:21.000000 fedops-0.1.9/fedops/__init__.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:51:02.723378 fedops-0.1.9/fedops/client/
--rw-r--r--   0 yangsemo   (501) staff       (20)      987 2023-05-23 04:42:21.000000 fedops-0.1.9/fedops/client/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     6957 2023-05-23 05:45:41.000000 fedops-0.1.9/fedops/client/app.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     5010 2023-05-22 17:11:45.000000 fedops-0.1.9/fedops/client/app_test.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2817 2023-05-23 04:42:21.000000 fedops-0.1.9/fedops/client/client_api.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     6088 2023-05-23 04:42:21.000000 fedops-0.1.9/fedops/client/client_fl.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     3478 2023-05-23 04:42:21.000000 fedops-0.1.9/fedops/client/client_utils.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2533 2023-05-23 05:49:05.000000 fedops-0.1.9/fedops/client/client_wandb.py
--rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.1.9/fedops/client/test.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:51:02.724295 fedops-0.1.9/fedops/server/
--rw-r--r--   0 yangsemo   (501) staff       (20)      977 2023-05-23 04:42:21.000000 fedops-0.1.9/fedops/server/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     8963 2023-05-23 05:44:14.000000 fedops-0.1.9/fedops/server/app.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     1283 2023-05-22 17:11:45.000000 fedops-0.1.9/fedops/server/server_api.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     3229 2023-05-23 04:42:21.000000 fedops-0.1.9/fedops/server/server_utils.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:51:02.724573 fedops-0.1.9/fedops/utils/
--rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.1.9/fedops/utils/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)      832 2023-05-22 17:11:45.000000 fedops-0.1.9/fedops/utils/version.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 05:51:02.721562 fedops-0.1.9/fedops.egg-info/
--rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 05:51:02.000000 fedops-0.1.9/fedops.egg-info/PKG-INFO
--rw-r--r--   0 yangsemo   (501) staff       (20)      540 2023-05-23 05:51:02.000000 fedops-0.1.9/fedops.egg-info/SOURCES.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)        1 2023-05-23 05:51:02.000000 fedops-0.1.9/fedops.egg-info/dependency_links.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)      187 2023-05-23 05:51:02.000000 fedops-0.1.9/fedops.egg-info/requires.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)        7 2023-05-23 05:51:02.000000 fedops-0.1.9/fedops.egg-info/top_level.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)       38 2023-05-23 05:51:02.725083 fedops-0.1.9/setup.cfg
--rw-r--r--   0 yangsemo   (501) staff       (20)     1130 2023-05-23 05:49:15.000000 fedops-0.1.9/setup.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 06:11:38.043498 fedops-0.2.0/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 06:11:38.043364 fedops-0.2.0/PKG-INFO
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 06:11:38.039616 fedops-0.2.0/fedops/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      872 2023-05-23 04:42:21.000000 fedops-0.2.0/fedops/__init__.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 06:11:38.042131 fedops-0.2.0/fedops/client/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      987 2023-05-23 04:42:21.000000 fedops-0.2.0/fedops/client/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     6957 2023-05-23 05:45:41.000000 fedops-0.2.0/fedops/client/app.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     5010 2023-05-22 17:11:45.000000 fedops-0.2.0/fedops/client/app_test.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2817 2023-05-23 04:42:21.000000 fedops-0.2.0/fedops/client/client_api.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     6088 2023-05-23 04:42:21.000000 fedops-0.2.0/fedops/client/client_fl.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     3478 2023-05-23 04:42:21.000000 fedops-0.2.0/fedops/client/client_utils.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2561 2023-05-23 06:06:12.000000 fedops-0.2.0/fedops/client/client_wandb.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.2.0/fedops/client/test.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 06:11:38.042847 fedops-0.2.0/fedops/server/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      977 2023-05-23 04:42:21.000000 fedops-0.2.0/fedops/server/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     8963 2023-05-23 05:44:14.000000 fedops-0.2.0/fedops/server/app.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     1283 2023-05-22 17:11:45.000000 fedops-0.2.0/fedops/server/server_api.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     3229 2023-05-23 04:42:21.000000 fedops-0.2.0/fedops/server/server_utils.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 06:11:38.043063 fedops-0.2.0/fedops/utils/
+-rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.2.0/fedops/utils/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)      832 2023-05-22 17:11:45.000000 fedops-0.2.0/fedops/utils/version.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 06:11:38.040551 fedops-0.2.0/fedops.egg-info/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 06:11:38.000000 fedops-0.2.0/fedops.egg-info/PKG-INFO
+-rw-r--r--   0 yangsemo   (501) staff       (20)      540 2023-05-23 06:11:38.000000 fedops-0.2.0/fedops.egg-info/SOURCES.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)        1 2023-05-23 06:11:38.000000 fedops-0.2.0/fedops.egg-info/dependency_links.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)      187 2023-05-23 06:11:38.000000 fedops-0.2.0/fedops.egg-info/requires.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)        7 2023-05-23 06:11:38.000000 fedops-0.2.0/fedops.egg-info/top_level.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)       38 2023-05-23 06:11:38.043537 fedops-0.2.0/setup.cfg
+-rw-r--r--   0 yangsemo   (501) staff       (20)     1130 2023-05-23 06:11:24.000000 fedops-0.2.0/setup.py
```

### Comparing `fedops-0.1.9/PKG-INFO` & `fedops-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedops
-Version: 0.1.9
+Version: 0.2.0
 Summary: FL Lifecycle Operations Management Platform
 Home-page: https://github.com/gachon-CCLab/FedOps.git
 Author: Semo Yang
 Author-email: tpah20@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedops-0.1.9/fedops/__init__.py` & `fedops-0.2.0/fedops/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.9/fedops/client/__init__.py` & `fedops-0.2.0/fedops/client/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.9/fedops/client/app.py` & `fedops-0.2.0/fedops/client/app.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.9/fedops/client/app_test.py` & `fedops-0.2.0/fedops/client/app_test.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.9/fedops/client/client_api.py` & `fedops-0.2.0/fedops/client/client_api.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.9/fedops/client/client_fl.py` & `fedops-0.2.0/fedops/client/client_fl.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.9/fedops/client/client_utils.py` & `fedops-0.2.0/fedops/client/client_utils.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.9/fedops/client/client_wandb.py` & `fedops-0.2.0/fedops/client/client_wandb.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,25 +25,24 @@
 def data_status_wandb(run, labels):
     table = wandb.Table(data=labels, columns=["label", "data_size"])
     run.log({'Data Lable Histogram': wandb.plot.bar(table, "label", "data_size", title="Data Size Distribution")})
 
 
 def client_system_wandb(fl_task_id, client_mac, next_gl_model_v, wandb_name, wandb_account):
     try:
-        time.sleep(2)
-
         # check client system resource usage from wandb
         api = wandb.Api()
         runs = api.runs(f"{wandb_account}/{fl_task_id}")
 
         sys_df = runs[0].history(stream="system")
 
         col = ['system.network.sent', 'system.network.recv', 'system.disk', '_runtime', 'system.proc.memory.rssMB','system.proc.memory.availableMB', 'system.cpu', 'system.proc.cpu.threads', 'system.memory', 'system.proc.memory.percent', '_timestamp']
+        cols = [c.replace('\n', '') for c in col]
 
-        sys_df = sys_df[col]
+        sys_df = sys_df[cols]
 
         sys_df.rename(columns={
             "system.network.sent": "network_sent",
             "system.network.recv": "network_recv",
             "system.disk": "disk",
             "_runtime": "runtime",
             "system.proc.memory.rssMB": "memory_rssMB",
```

### Comparing `fedops-0.1.9/fedops/server/__init__.py` & `fedops-0.2.0/fedops/server/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.9/fedops/server/app.py` & `fedops-0.2.0/fedops/server/app.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.9/fedops/server/server_api.py` & `fedops-0.2.0/fedops/server/server_api.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.9/fedops/server/server_utils.py` & `fedops-0.2.0/fedops/server/server_utils.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.9/fedops/utils/version.py` & `fedops-0.2.0/fedops/utils/version.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.9/fedops.egg-info/PKG-INFO` & `fedops-0.2.0/fedops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedops
-Version: 0.1.9
+Version: 0.2.0
 Summary: FL Lifecycle Operations Management Platform
 Home-page: https://github.com/gachon-CCLab/FedOps.git
 Author: Semo Yang
 Author-email: tpah20@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedops-0.1.9/fedops.egg-info/SOURCES.txt` & `fedops-0.2.0/fedops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fedops-0.1.9/setup.py` & `fedops-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fedops',
-    version='0.1.9',
+    version='0.2.0',
     author='Semo Yang',
     author_email='tpah20@gmail.com',
     description='FL Lifecycle Operations Management Platform',
     long_description='Long description of your library',
     url='https://github.com/gachon-CCLab/FedOps.git',
     packages=find_packages(),
     install_requires=[
```

