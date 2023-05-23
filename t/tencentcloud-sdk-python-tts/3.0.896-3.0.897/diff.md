# Comparing `tmp/tencentcloud-sdk-python-tts-3.0.896.tar.gz` & `tmp/tencentcloud-sdk-python-tts-3.0.897.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tts-3.0.896.tar", last modified: Mon May 22 00:36:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tts-3.0.897.tar", last modified: Tue May 23 02:35:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tts-3.0.896.tar` & `tencentcloud-sdk-python-tts-3.0.897.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:36:45.000000 tencentcloud-sdk-python-tts-3.0.896/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-22 00:36:45.000000 tencentcloud-sdk-python-tts-3.0.896/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:36:45.000000 tencentcloud-sdk-python-tts-3.0.896/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:36:45.000000 tencentcloud-sdk-python-tts-3.0.896/tencentcloud/tts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:36:45.000000 tencentcloud-sdk-python-tts-3.0.896/tencentcloud/tts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:36:45.000000 tencentcloud-sdk-python-tts-3.0.896/tencentcloud/tts/v20190823/
--rw-r--r--   0 root         (0) root         (0)     5572 2023-05-22 00:36:45.000000 tencentcloud-sdk-python-tts-3.0.896/tencentcloud/tts/v20190823/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:36:45.000000 tencentcloud-sdk-python-tts-3.0.896/tencentcloud/tts/v20190823/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21052 2023-05-22 00:36:45.000000 tencentcloud-sdk-python-tts-3.0.896/tencentcloud/tts/v20190823/models.py
--rw-r--r--   0 root         (0) root         (0)     5910 2023-05-22 00:36:45.000000 tencentcloud-sdk-python-tts-3.0.896/tencentcloud/tts/v20190823/tts_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:36:45.000000 tencentcloud-sdk-python-tts-3.0.896/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:36:45.000000 tencentcloud-sdk-python-tts-3.0.896/tencentcloud_sdk_python_tts.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:36:45.000000 tencentcloud-sdk-python-tts-3.0.896/tencentcloud_sdk_python_tts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-22 00:36:45.000000 tencentcloud-sdk-python-tts-3.0.896/tencentcloud_sdk_python_tts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:36:45.000000 tencentcloud-sdk-python-tts-3.0.896/tencentcloud_sdk_python_tts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:36:45.000000 tencentcloud-sdk-python-tts-3.0.896/tencentcloud_sdk_python_tts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:36:45.000000 tencentcloud-sdk-python-tts-3.0.896/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-22 00:36:45.000000 tencentcloud-sdk-python-tts-3.0.896/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:36:45.000000 tencentcloud-sdk-python-tts-3.0.896/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:35:32.000000 tencentcloud-sdk-python-tts-3.0.897/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-23 02:35:32.000000 tencentcloud-sdk-python-tts-3.0.897/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:35:32.000000 tencentcloud-sdk-python-tts-3.0.897/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:35:32.000000 tencentcloud-sdk-python-tts-3.0.897/tencentcloud/tts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:35:32.000000 tencentcloud-sdk-python-tts-3.0.897/tencentcloud/tts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:35:32.000000 tencentcloud-sdk-python-tts-3.0.897/tencentcloud/tts/v20190823/
+-rw-r--r--   0 root         (0) root         (0)     5572 2023-05-23 02:35:32.000000 tencentcloud-sdk-python-tts-3.0.897/tencentcloud/tts/v20190823/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:35:32.000000 tencentcloud-sdk-python-tts-3.0.897/tencentcloud/tts/v20190823/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21052 2023-05-23 02:35:32.000000 tencentcloud-sdk-python-tts-3.0.897/tencentcloud/tts/v20190823/models.py
+-rw-r--r--   0 root         (0) root         (0)     5910 2023-05-23 02:35:32.000000 tencentcloud-sdk-python-tts-3.0.897/tencentcloud/tts/v20190823/tts_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:35:32.000000 tencentcloud-sdk-python-tts-3.0.897/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:35:32.000000 tencentcloud-sdk-python-tts-3.0.897/tencentcloud_sdk_python_tts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:35:32.000000 tencentcloud-sdk-python-tts-3.0.897/tencentcloud_sdk_python_tts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-23 02:35:32.000000 tencentcloud-sdk-python-tts-3.0.897/tencentcloud_sdk_python_tts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:35:32.000000 tencentcloud-sdk-python-tts-3.0.897/tencentcloud_sdk_python_tts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:35:32.000000 tencentcloud-sdk-python-tts-3.0.897/tencentcloud_sdk_python_tts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:35:32.000000 tencentcloud-sdk-python-tts-3.0.897/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-23 02:35:32.000000 tencentcloud-sdk-python-tts-3.0.897/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:35:32.000000 tencentcloud-sdk-python-tts-3.0.897/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tts-3.0.896/README.rst` & `tencentcloud-sdk-python-tts-3.0.897/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.896/tencentcloud/tts/v20190823/errorcodes.py` & `tencentcloud-sdk-python-tts-3.0.897/tencentcloud/tts/v20190823/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.896/tencentcloud/tts/v20190823/models.py` & `tencentcloud-sdk-python-tts-3.0.897/tencentcloud/tts/v20190823/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.896/tencentcloud/tts/v20190823/tts_client.py` & `tencentcloud-sdk-python-tts-3.0.897/tencentcloud/tts/v20190823/tts_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.896/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tts-3.0.897/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tts-3.0.896/tencentcloud_sdk_python_tts.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tts-3.0.897/tencentcloud_sdk_python_tts.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tts
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Tts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tts-3.0.896/PKG-INFO` & `tencentcloud-sdk-python-tts-3.0.897/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tts
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Tts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tts-3.0.896/setup.py` & `tencentcloud-sdk-python-tts-3.0.897/setup.py`

 * *Files identical despite different names*
