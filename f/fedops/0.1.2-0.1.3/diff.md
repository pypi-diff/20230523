# Comparing `tmp/fedops-0.1.2.tar.gz` & `tmp/fedops-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedops-0.1.2.tar", last modified: Mon May 22 17:03:14 2023, max compression
+gzip compressed data, was "fedops-0.1.3.tar", last modified: Tue May 23 02:15:53 2023, max compression
```

## Comparing `fedops-0.1.2.tar` & `fedops-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:03:14.756381 fedops-0.1.2/
--rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-22 17:03:14.756178 fedops-0.1.2/PKG-INFO
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:03:14.746076 fedops-0.1.2/fedops/
--rw-r--r--   0 yangsemo   (501) staff       (20)      872 2023-05-22 16:52:45.000000 fedops-0.1.2/fedops/__init__.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:03:14.753264 fedops-0.1.2/fedops/client/
--rw-r--r--   0 yangsemo   (501) staff       (20)     1129 2023-05-22 16:03:54.000000 fedops-0.1.2/fedops/client/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     7003 2023-05-22 16:00:57.000000 fedops-0.1.2/fedops/client/app.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     5010 2023-05-22 04:50:21.000000 fedops-0.1.2/fedops/client/app_test.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2809 2023-05-18 10:47:23.000000 fedops-0.1.2/fedops/client/client_api.py
--rw-r--r--   0 yangsemo   (501) staff       (20)    12517 2023-05-18 10:32:47.000000 fedops-0.1.2/fedops/client/client_data.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     6073 2023-05-19 05:35:33.000000 fedops-0.1.2/fedops/client/client_fl.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2909 2023-05-18 08:14:34.000000 fedops-0.1.2/fedops/client/client_model.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2059 2023-05-22 15:51:31.000000 fedops-0.1.2/fedops/client/client_task.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     1614 2023-05-22 04:50:40.000000 fedops-0.1.2/fedops/client/client_task_copy.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     3571 2023-05-22 15:54:13.000000 fedops-0.1.2/fedops/client/client_utils.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2230 2023-05-22 11:55:10.000000 fedops-0.1.2/fedops/client/client_wandb.py
--rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 04:17:43.000000 fedops-0.1.2/fedops/client/test.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:03:14.755363 fedops-0.1.2/fedops/server/
--rw-r--r--   0 yangsemo   (501) staff       (20)      868 2023-05-22 16:40:03.000000 fedops-0.1.2/fedops/server/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     8967 2023-05-22 16:31:47.000000 fedops-0.1.2/fedops/server/app.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2909 2023-05-18 12:01:35.000000 fedops-0.1.2/fedops/server/init_gl_model.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     1283 2023-05-19 06:37:19.000000 fedops-0.1.2/fedops/server/server_api.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     2209 2023-05-22 16:31:47.000000 fedops-0.1.2/fedops/server/server_task.py
--rw-r--r--   0 yangsemo   (501) staff       (20)     3715 2023-05-19 07:54:45.000000 fedops-0.1.2/fedops/server/server_utils.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:03:14.755761 fedops-0.1.2/fedops/utils/
--rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 03:47:38.000000 fedops-0.1.2/fedops/utils/__init__.py
--rw-r--r--   0 yangsemo   (501) staff       (20)      832 2023-05-22 03:48:03.000000 fedops-0.1.2/fedops/utils/version.py
-drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:03:14.747399 fedops-0.1.2/fedops.egg-info/
--rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-22 17:03:14.000000 fedops-0.1.2/fedops.egg-info/PKG-INFO
--rw-r--r--   0 yangsemo   (501) staff       (20)      722 2023-05-22 17:03:14.000000 fedops-0.1.2/fedops.egg-info/SOURCES.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)        1 2023-05-22 17:03:14.000000 fedops-0.1.2/fedops.egg-info/dependency_links.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)      187 2023-05-22 17:03:14.000000 fedops-0.1.2/fedops.egg-info/requires.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)        7 2023-05-22 17:03:14.000000 fedops-0.1.2/fedops.egg-info/top_level.txt
--rw-r--r--   0 yangsemo   (501) staff       (20)       38 2023-05-22 17:03:14.756448 fedops-0.1.2/setup.cfg
--rw-r--r--   0 yangsemo   (501) staff       (20)     1130 2023-05-22 17:02:37.000000 fedops-0.1.2/setup.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 02:15:53.898847 fedops-0.1.3/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 02:15:53.898721 fedops-0.1.3/PKG-INFO
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 02:15:53.894563 fedops-0.1.3/fedops/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      872 2023-05-23 02:14:46.000000 fedops-0.1.3/fedops/__init__.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 02:15:53.897200 fedops-0.1.3/fedops/client/
+-rw-r--r--   0 yangsemo   (501) staff       (20)     1165 2023-05-23 02:13:21.000000 fedops-0.1.3/fedops/client/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     7003 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/client/app.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     5010 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/client/app_test.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2809 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/client/client_api.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)    12517 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/client/client_data.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     6073 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/client/client_fl.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2909 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/client/client_model.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2059 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/client/client_task.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     3574 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/client/client_utils.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2230 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/client/client_wandb.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/client/test.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 02:15:53.898299 fedops-0.1.3/fedops/server/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      961 2023-05-23 02:13:53.000000 fedops-0.1.3/fedops/server/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     8967 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/server/app.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2909 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/server/init_gl_model.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     1283 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/server/server_api.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     2209 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/server/server_task.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)     3715 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/server/server_utils.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 02:15:53.898523 fedops-0.1.3/fedops/utils/
+-rw-r--r--   0 yangsemo   (501) staff       (20)        0 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/utils/__init__.py
+-rw-r--r--   0 yangsemo   (501) staff       (20)      832 2023-05-22 17:11:45.000000 fedops-0.1.3/fedops/utils/version.py
+drwxr-xr-x   0 yangsemo   (501) staff       (20)        0 2023-05-23 02:15:53.895278 fedops-0.1.3/fedops.egg-info/
+-rw-r--r--   0 yangsemo   (501) staff       (20)      647 2023-05-23 02:15:53.000000 fedops-0.1.3/fedops.egg-info/PKG-INFO
+-rw-r--r--   0 yangsemo   (501) staff       (20)      688 2023-05-23 02:15:53.000000 fedops-0.1.3/fedops.egg-info/SOURCES.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)        1 2023-05-23 02:15:53.000000 fedops-0.1.3/fedops.egg-info/dependency_links.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)      187 2023-05-23 02:15:53.000000 fedops-0.1.3/fedops.egg-info/requires.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)        7 2023-05-23 02:15:53.000000 fedops-0.1.3/fedops.egg-info/top_level.txt
+-rw-r--r--   0 yangsemo   (501) staff       (20)       38 2023-05-23 02:15:53.898887 fedops-0.1.3/setup.cfg
+-rw-r--r--   0 yangsemo   (501) staff       (20)     1130 2023-05-23 02:14:13.000000 fedops-0.1.3/setup.py
```

### Comparing `fedops-0.1.2/PKG-INFO` & `fedops-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedops
-Version: 0.1.2
+Version: 0.1.3
 Summary: FL Lifecycle Operations Management Platform
 Home-page: https://github.com/gachon-CCLab/FedOps.git
 Author: Semo Yang
 Author-email: tpah20@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedops-0.1.2/fedops/__init__.py` & `fedops-0.1.3/fedops/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""FedOps main package."""
+"""FedOps Main Package."""
 
 from .utils.version import package_version as _package_version
 
 from . import client, server
 
 __all__ = [
     "client",
```

### Comparing `fedops-0.1.2/fedops/client/__init__.py` & `fedops-0.1.3/fedops/client/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,28 +8,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""FedOps client."""
+"""FedOps Client."""
 
-from .app import FLClientTask
-from .client_api import ClientMangerAPI
-from .client_api import ClientServerAPI
-from .client_fl import FLClient
-from .client_fl import flower_client_start
-from .client_utils import FLClientStatus
-from .client_utils import ManagerData
+# from .app import FLClientTask
+# from .client_api import ClientMangerAPI
+# from .client_api import ClientServerAPI
+# from .client_fl import FLClient
+# from .client_fl import flower_client_start
+# from .client_utils import FLClientStatus
+# from .client_utils import ManagerData
 
+import client_utils
+import app
+import client_fl
+import client_api
+import client_wandb
 
-__all__ = [
-    "FLClientTask",
-    "ClientMangerAPI",
-    "ClientServerAPI",
-    "FLClient",
-    "flower_client_start",
-    "FLClientStatus",
-    "ManagerData",
 
+__all__ = [
+    "client_utils",
+    "app",
+    "client_fl",
+    "client_api",
+    "client_wandb",
 ]
```

### Comparing `fedops-0.1.2/fedops/client/app.py` & `fedops-0.1.3/fedops/client/app.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.2/fedops/client/app_test.py` & `fedops-0.1.3/fedops/client/app_test.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.2/fedops/client/client_api.py` & `fedops-0.1.3/fedops/client/client_api.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.2/fedops/client/client_data.py` & `fedops-0.1.3/fedops/client/client_data.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.2/fedops/client/client_fl.py` & `fedops-0.1.3/fedops/client/client_fl.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.2/fedops/client/client_model.py` & `fedops-0.1.3/fedops/client/client_model.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.2/fedops/client/client_task.py` & `fedops-0.1.3/fedops/client/client_task.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.2/fedops/client/client_utils.py` & `fedops-0.1.3/fedops/client/client_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,17 @@
 
 # Get manager data info
 class ManagerData(BaseModel):
     server_ip: str
     client_mac: str
 
 
-def read_config():
+def read_config(file_path):
     # Read the YAML configuration file
-    config_file_path = './config.yaml'
+    config_file_path = file_path
     with open(config_file_path, 'r') as file:
         config = yaml.safe_load(file)
     return config
 
 
 def get_mac_address():
     mac = uuid.UUID(int=uuid.getnode()).hex[-12:]
```

### Comparing `fedops-0.1.2/fedops/client/client_wandb.py` & `fedops-0.1.3/fedops/client/client_wandb.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.2/fedops/server/__init__.py` & `fedops-0.1.3/fedops/server/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,18 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""FedOps client."""
+"""FedOps Server."""
 
-from .app import FLServer
-from .server_api import ServerAPI
-from .server_utils import FLServerStatus
+# from .app import FLServer
+# from .server_api import ServerAPI
+# from .server_utils import FLServerStatus
+
+import app
+import init_gl_model
+import server_utils
+import server_api
 
 __all__ = [
-    "FLServer",
-    "ServerAPI",
-    "FLServerStatus"
+    "app",
+    "init_gl_model",
+    "server_utils",
+    "server_api",
 ]
```

### Comparing `fedops-0.1.2/fedops/server/app.py` & `fedops-0.1.3/fedops/server/app.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.2/fedops/server/init_gl_model.py` & `fedops-0.1.3/fedops/server/init_gl_model.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.2/fedops/server/server_api.py` & `fedops-0.1.3/fedops/server/server_api.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.2/fedops/server/server_task.py` & `fedops-0.1.3/fedops/server/server_task.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.2/fedops/server/server_utils.py` & `fedops-0.1.3/fedops/server/server_utils.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.2/fedops/utils/version.py` & `fedops-0.1.3/fedops/utils/version.py`

 * *Files identical despite different names*

### Comparing `fedops-0.1.2/fedops.egg-info/PKG-INFO` & `fedops-0.1.3/fedops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedops
-Version: 0.1.2
+Version: 0.1.3
 Summary: FL Lifecycle Operations Management Platform
 Home-page: https://github.com/gachon-CCLab/FedOps.git
 Author: Semo Yang
 Author-email: tpah20@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedops-0.1.2/fedops.egg-info/SOURCES.txt` & `fedops-0.1.3/fedops.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 fedops/client/app.py
 fedops/client/app_test.py
 fedops/client/client_api.py
 fedops/client/client_data.py
 fedops/client/client_fl.py
 fedops/client/client_model.py
 fedops/client/client_task.py
-fedops/client/client_task_copy.py
 fedops/client/client_utils.py
 fedops/client/client_wandb.py
 fedops/client/test.py
 fedops/server/__init__.py
 fedops/server/app.py
 fedops/server/init_gl_model.py
 fedops/server/server_api.py
```

### Comparing `fedops-0.1.2/setup.py` & `fedops-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fedops',
-    version='0.1.2',
+    version='0.1.3',
     author='Semo Yang',
     author_email='tpah20@gmail.com',
     description='FL Lifecycle Operations Management Platform',
     long_description='Long description of your library',
     url='https://github.com/gachon-CCLab/FedOps.git',
     packages=find_packages(),
     install_requires=[
```

