# Comparing `tmp/tencentcloud-sdk-python-ssl-3.0.896.tar.gz` & `tmp/tencentcloud-sdk-python-ssl-3.0.897.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ssl-3.0.896.tar", last modified: Mon May 22 00:31:27 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ssl-3.0.897.tar", last modified: Tue May 23 02:30:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ssl-3.0.896.tar` & `tencentcloud-sdk-python-ssl-3.0.897.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:31:27.000000 tencentcloud-sdk-python-ssl-3.0.896/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-22 00:31:26.000000 tencentcloud-sdk-python-ssl-3.0.896/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:31:27.000000 tencentcloud-sdk-python-ssl-3.0.896/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:31:26.000000 tencentcloud-sdk-python-ssl-3.0.896/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:31:27.000000 tencentcloud-sdk-python-ssl-3.0.896/tencentcloud/ssl/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:31:26.000000 tencentcloud-sdk-python-ssl-3.0.896/tencentcloud/ssl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:31:27.000000 tencentcloud-sdk-python-ssl-3.0.896/tencentcloud/ssl/v20191205/
--rw-r--r--   0 root         (0) root         (0)     8810 2023-05-22 00:31:26.000000 tencentcloud-sdk-python-ssl-3.0.896/tencentcloud/ssl/v20191205/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:31:26.000000 tencentcloud-sdk-python-ssl-3.0.896/tencentcloud/ssl/v20191205/__init__.py
--rw-r--r--   0 root         (0) root         (0)   217317 2023-05-22 00:31:26.000000 tencentcloud-sdk-python-ssl-3.0.896/tencentcloud/ssl/v20191205/models.py
--rw-r--r--   0 root         (0) root         (0)    48579 2023-05-22 00:31:26.000000 tencentcloud-sdk-python-ssl-3.0.896/tencentcloud/ssl/v20191205/ssl_client.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:31:27.000000 tencentcloud-sdk-python-ssl-3.0.896/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-22 00:31:26.000000 tencentcloud-sdk-python-ssl-3.0.896/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:31:27.000000 tencentcloud-sdk-python-ssl-3.0.896/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:31:27.000000 tencentcloud-sdk-python-ssl-3.0.896/tencentcloud_sdk_python_ssl.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:31:27.000000 tencentcloud-sdk-python-ssl-3.0.896/tencentcloud_sdk_python_ssl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-22 00:31:27.000000 tencentcloud-sdk-python-ssl-3.0.896/tencentcloud_sdk_python_ssl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:31:27.000000 tencentcloud-sdk-python-ssl-3.0.896/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:31:27.000000 tencentcloud-sdk-python-ssl-3.0.896/tencentcloud_sdk_python_ssl.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:30:34.000000 tencentcloud-sdk-python-ssl-3.0.897/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-23 02:30:34.000000 tencentcloud-sdk-python-ssl-3.0.897/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:30:34.000000 tencentcloud-sdk-python-ssl-3.0.897/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:30:34.000000 tencentcloud-sdk-python-ssl-3.0.897/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:30:34.000000 tencentcloud-sdk-python-ssl-3.0.897/tencentcloud/ssl/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:30:34.000000 tencentcloud-sdk-python-ssl-3.0.897/tencentcloud/ssl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:30:34.000000 tencentcloud-sdk-python-ssl-3.0.897/tencentcloud/ssl/v20191205/
+-rw-r--r--   0 root         (0) root         (0)     8810 2023-05-23 02:30:34.000000 tencentcloud-sdk-python-ssl-3.0.897/tencentcloud/ssl/v20191205/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:30:34.000000 tencentcloud-sdk-python-ssl-3.0.897/tencentcloud/ssl/v20191205/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   217317 2023-05-23 02:30:34.000000 tencentcloud-sdk-python-ssl-3.0.897/tencentcloud/ssl/v20191205/models.py
+-rw-r--r--   0 root         (0) root         (0)    48579 2023-05-23 02:30:34.000000 tencentcloud-sdk-python-ssl-3.0.897/tencentcloud/ssl/v20191205/ssl_client.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:30:34.000000 tencentcloud-sdk-python-ssl-3.0.897/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-23 02:30:34.000000 tencentcloud-sdk-python-ssl-3.0.897/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:30:34.000000 tencentcloud-sdk-python-ssl-3.0.897/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:30:34.000000 tencentcloud-sdk-python-ssl-3.0.897/tencentcloud_sdk_python_ssl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:30:34.000000 tencentcloud-sdk-python-ssl-3.0.897/tencentcloud_sdk_python_ssl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-23 02:30:34.000000 tencentcloud-sdk-python-ssl-3.0.897/tencentcloud_sdk_python_ssl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:30:34.000000 tencentcloud-sdk-python-ssl-3.0.897/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:30:34.000000 tencentcloud-sdk-python-ssl-3.0.897/tencentcloud_sdk_python_ssl.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.896/README.rst` & `tencentcloud-sdk-python-ssl-3.0.897/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.896/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ssl-3.0.897/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ssl-3.0.896/tencentcloud/ssl/v20191205/errorcodes.py` & `tencentcloud-sdk-python-ssl-3.0.897/tencentcloud/ssl/v20191205/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.896/tencentcloud/ssl/v20191205/models.py` & `tencentcloud-sdk-python-ssl-3.0.897/tencentcloud/ssl/v20191205/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.896/tencentcloud/ssl/v20191205/ssl_client.py` & `tencentcloud-sdk-python-ssl-3.0.897/tencentcloud/ssl/v20191205/ssl_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.896/PKG-INFO` & `tencentcloud-sdk-python-ssl-3.0.897/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssl
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Ssl SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.896/setup.py` & `tencentcloud-sdk-python-ssl-3.0.897/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.896/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ssl-3.0.897/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssl
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Ssl SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

