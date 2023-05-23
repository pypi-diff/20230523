# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.896.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.897.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.896.tar", last modified: Mon May 22 00:37:21 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.897.tar", last modified: Tue May 23 02:36:05 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.896.tar` & `tencentcloud-sdk-python-vpc-3.0.897.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/vpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   332171 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)    41601 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   851287 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/vpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/vpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   332171 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)    41601 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   851409 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/vpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.896/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.897/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.896/README.rst` & `tencentcloud-sdk-python-vpc-3.0.897/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/vpc/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -11602,15 +11602,15 @@
         :type InstanceId: str
         :param StartDate: 开始日期，格式%Y-%m-%d %H:%M:%S。
         :type StartDate: str
         :param EndDate: 结束日期，格式%Y-%m-%d %H:%M:%S。
         :type EndDate: str
         :param Offset: 偏移量，默认为0。
         :type Offset: int
-        :param Limit: 返回数量，默认为20，最大为200。
+        :param Limit: 返回数量，默认为20，最大为100。
         :type Limit: int
         """
         self.BusinessType = None
         self.InstanceId = None
         self.StartDate = None
         self.EndDate = None
         self.Offset = None
@@ -12246,25 +12246,25 @@
 class DescribeVpcEndPointServiceRequest(AbstractModel):
     """DescribeVpcEndPointService请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Filters: 过滤条件。
+        :param Filters: 过滤条件。不支持同时传入参数 EndPointServiceIds and Filters。
 <li> service-id - String - （过滤条件）终端节点服务唯一ID。</li>
 <li>service-name - String - （过滤条件）终端节点实例名称。</li>
 <li>service-instance-id - String - （过滤条件）后端服务的唯一ID，比如lb-xxx。</li>
 <li>service-type - String - （过滤条件）后端PAAS服务类型，CLB,CDB,CRS，不填默认查询类型为CLB。</li>
         :type Filters: list of Filter
         :param Offset: 偏移量，默认为0。
         :type Offset: int
         :param Limit: 单页返回数量，默认为20，最大值为100。
         :type Limit: int
-        :param EndPointServiceIds: 终端节点服务ID。
+        :param EndPointServiceIds: 终端节点服务ID。不支持同时传入参数 EndPointServiceIds and Filters。
         :type EndPointServiceIds: list of str
         """
         self.Filters = None
         self.Offset = None
         self.Limit = None
         self.EndPointServiceIds = None
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vpc-3.0.896/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.897/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.896/setup.py` & `tencentcloud-sdk-python-vpc-3.0.897/setup.py`

 * *Files identical despite different names*

