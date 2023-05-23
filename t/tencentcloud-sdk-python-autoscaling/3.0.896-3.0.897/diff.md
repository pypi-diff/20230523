# Comparing `tmp/tencentcloud-sdk-python-autoscaling-3.0.896.tar.gz` & `tmp/tencentcloud-sdk-python-autoscaling-3.0.897.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-autoscaling-3.0.896.tar", last modified: Mon May 22 00:14:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-autoscaling-3.0.897.tar", last modified: Tue May 23 02:13:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-autoscaling-3.0.896.tar` & `tencentcloud-sdk-python-autoscaling-3.0.897.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:14:45.000000 tencentcloud-sdk-python-autoscaling-3.0.896/
--rw-r--r--   0 root         (0) root         (0)      761 2023-05-22 00:14:45.000000 tencentcloud-sdk-python-autoscaling-3.0.896/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:14:45.000000 tencentcloud-sdk-python-autoscaling-3.0.896/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:14:45.000000 tencentcloud-sdk-python-autoscaling-3.0.896/tencentcloud/autoscaling/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:14:45.000000 tencentcloud-sdk-python-autoscaling-3.0.896/tencentcloud/autoscaling/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:14:45.000000 tencentcloud-sdk-python-autoscaling-3.0.896/tencentcloud/autoscaling/v20180419/
--rw-r--r--   0 root         (0) root         (0)    60396 2023-05-22 00:14:45.000000 tencentcloud-sdk-python-autoscaling-3.0.896/tencentcloud/autoscaling/v20180419/autoscaling_client.py
--rw-r--r--   0 root         (0) root         (0)    19836 2023-05-22 00:14:45.000000 tencentcloud-sdk-python-autoscaling-3.0.896/tencentcloud/autoscaling/v20180419/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:14:45.000000 tencentcloud-sdk-python-autoscaling-3.0.896/tencentcloud/autoscaling/v20180419/__init__.py
--rw-r--r--   0 root         (0) root         (0)   258492 2023-05-22 00:14:45.000000 tencentcloud-sdk-python-autoscaling-3.0.896/tencentcloud/autoscaling/v20180419/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:14:45.000000 tencentcloud-sdk-python-autoscaling-3.0.896/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1699 2023-05-22 00:14:45.000000 tencentcloud-sdk-python-autoscaling-3.0.896/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:14:45.000000 tencentcloud-sdk-python-autoscaling-3.0.896/tencentcloud_sdk_python_autoscaling.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:14:45.000000 tencentcloud-sdk-python-autoscaling-3.0.896/tencentcloud_sdk_python_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      525 2023-05-22 00:14:45.000000 tencentcloud-sdk-python-autoscaling-3.0.896/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1699 2023-05-22 00:14:45.000000 tencentcloud-sdk-python-autoscaling-3.0.896/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:14:45.000000 tencentcloud-sdk-python-autoscaling-3.0.896/tencentcloud_sdk_python_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1022 2023-05-22 00:14:45.000000 tencentcloud-sdk-python-autoscaling-3.0.896/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:14:45.000000 tencentcloud-sdk-python-autoscaling-3.0.896/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:13:58.000000 tencentcloud-sdk-python-autoscaling-3.0.897/
+-rw-r--r--   0 root         (0) root         (0)      761 2023-05-23 02:13:58.000000 tencentcloud-sdk-python-autoscaling-3.0.897/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:13:58.000000 tencentcloud-sdk-python-autoscaling-3.0.897/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:13:58.000000 tencentcloud-sdk-python-autoscaling-3.0.897/tencentcloud/autoscaling/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:13:58.000000 tencentcloud-sdk-python-autoscaling-3.0.897/tencentcloud/autoscaling/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:13:58.000000 tencentcloud-sdk-python-autoscaling-3.0.897/tencentcloud/autoscaling/v20180419/
+-rw-r--r--   0 root         (0) root         (0)    60396 2023-05-23 02:13:58.000000 tencentcloud-sdk-python-autoscaling-3.0.897/tencentcloud/autoscaling/v20180419/autoscaling_client.py
+-rw-r--r--   0 root         (0) root         (0)    19836 2023-05-23 02:13:58.000000 tencentcloud-sdk-python-autoscaling-3.0.897/tencentcloud/autoscaling/v20180419/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:13:58.000000 tencentcloud-sdk-python-autoscaling-3.0.897/tencentcloud/autoscaling/v20180419/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   258492 2023-05-23 02:13:58.000000 tencentcloud-sdk-python-autoscaling-3.0.897/tencentcloud/autoscaling/v20180419/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:13:58.000000 tencentcloud-sdk-python-autoscaling-3.0.897/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-05-23 02:13:58.000000 tencentcloud-sdk-python-autoscaling-3.0.897/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:13:58.000000 tencentcloud-sdk-python-autoscaling-3.0.897/tencentcloud_sdk_python_autoscaling.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:13:58.000000 tencentcloud-sdk-python-autoscaling-3.0.897/tencentcloud_sdk_python_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      525 2023-05-23 02:13:58.000000 tencentcloud-sdk-python-autoscaling-3.0.897/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-05-23 02:13:58.000000 tencentcloud-sdk-python-autoscaling-3.0.897/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:13:58.000000 tencentcloud-sdk-python-autoscaling-3.0.897/tencentcloud_sdk_python_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-05-23 02:13:58.000000 tencentcloud-sdk-python-autoscaling-3.0.897/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:13:58.000000 tencentcloud-sdk-python-autoscaling-3.0.897/setup.cfg
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.896/README.rst` & `tencentcloud-sdk-python-autoscaling-3.0.897/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.896/tencentcloud/autoscaling/v20180419/autoscaling_client.py` & `tencentcloud-sdk-python-autoscaling-3.0.897/tencentcloud/autoscaling/v20180419/autoscaling_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.896/tencentcloud/autoscaling/v20180419/errorcodes.py` & `tencentcloud-sdk-python-autoscaling-3.0.897/tencentcloud/autoscaling/v20180419/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.896/tencentcloud/autoscaling/v20180419/models.py` & `tencentcloud-sdk-python-autoscaling-3.0.897/tencentcloud/autoscaling/v20180419/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.896/tencentcloud/__init__.py` & `tencentcloud-sdk-python-autoscaling-3.0.897/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.896'
+__version__ = '3.0.897'
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.896/PKG-INFO` & `tencentcloud-sdk-python-autoscaling-3.0.897/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-autoscaling
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Autoscaling SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.896/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-autoscaling-3.0.897/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.896/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO` & `tencentcloud-sdk-python-autoscaling-3.0.897/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-autoscaling
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Autoscaling SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.896/setup.py` & `tencentcloud-sdk-python-autoscaling-3.0.897/setup.py`

 * *Files identical despite different names*

