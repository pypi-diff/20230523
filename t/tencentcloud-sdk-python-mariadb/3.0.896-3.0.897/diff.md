# Comparing `tmp/tencentcloud-sdk-python-mariadb-3.0.896.tar.gz` & `tmp/tencentcloud-sdk-python-mariadb-3.0.897.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mariadb-3.0.896.tar", last modified: Mon May 22 00:27:08 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mariadb-3.0.897.tar", last modified: Tue May 23 02:26:22 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mariadb-3.0.896.tar` & `tencentcloud-sdk-python-mariadb-3.0.897.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:27:08.000000 tencentcloud-sdk-python-mariadb-3.0.896/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:27:08.000000 tencentcloud-sdk-python-mariadb-3.0.896/tencentcloud_sdk_python_mariadb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:27:08.000000 tencentcloud-sdk-python-mariadb-3.0.896/tencentcloud_sdk_python_mariadb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-22 00:27:08.000000 tencentcloud-sdk-python-mariadb-3.0.896/tencentcloud_sdk_python_mariadb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-22 00:27:08.000000 tencentcloud-sdk-python-mariadb-3.0.896/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:27:08.000000 tencentcloud-sdk-python-mariadb-3.0.896/tencentcloud_sdk_python_mariadb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      749 2023-05-22 00:27:08.000000 tencentcloud-sdk-python-mariadb-3.0.896/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:27:08.000000 tencentcloud-sdk-python-mariadb-3.0.896/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:27:08.000000 tencentcloud-sdk-python-mariadb-3.0.896/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:27:08.000000 tencentcloud-sdk-python-mariadb-3.0.896/tencentcloud/mariadb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:27:08.000000 tencentcloud-sdk-python-mariadb-3.0.896/tencentcloud/mariadb/v20170312/
--rw-r--r--   0 root         (0) root         (0)    69766 2023-05-22 00:27:08.000000 tencentcloud-sdk-python-mariadb-3.0.896/tencentcloud/mariadb/v20170312/mariadb_client.py
--rw-r--r--   0 root         (0) root         (0)    14808 2023-05-22 00:27:08.000000 tencentcloud-sdk-python-mariadb-3.0.896/tencentcloud/mariadb/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:27:08.000000 tencentcloud-sdk-python-mariadb-3.0.896/tencentcloud/mariadb/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   213570 2023-05-22 00:27:08.000000 tencentcloud-sdk-python-mariadb-3.0.896/tencentcloud/mariadb/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:27:08.000000 tencentcloud-sdk-python-mariadb-3.0.896/tencentcloud/mariadb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-22 00:27:08.000000 tencentcloud-sdk-python-mariadb-3.0.896/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-05-22 00:27:08.000000 tencentcloud-sdk-python-mariadb-3.0.896/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:27:08.000000 tencentcloud-sdk-python-mariadb-3.0.896/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:26:22.000000 tencentcloud-sdk-python-mariadb-3.0.897/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:26:22.000000 tencentcloud-sdk-python-mariadb-3.0.897/tencentcloud_sdk_python_mariadb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:26:22.000000 tencentcloud-sdk-python-mariadb-3.0.897/tencentcloud_sdk_python_mariadb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-23 02:26:22.000000 tencentcloud-sdk-python-mariadb-3.0.897/tencentcloud_sdk_python_mariadb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-23 02:26:22.000000 tencentcloud-sdk-python-mariadb-3.0.897/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:26:22.000000 tencentcloud-sdk-python-mariadb-3.0.897/tencentcloud_sdk_python_mariadb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      749 2023-05-23 02:26:22.000000 tencentcloud-sdk-python-mariadb-3.0.897/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:26:22.000000 tencentcloud-sdk-python-mariadb-3.0.897/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:26:22.000000 tencentcloud-sdk-python-mariadb-3.0.897/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:26:22.000000 tencentcloud-sdk-python-mariadb-3.0.897/tencentcloud/mariadb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:26:22.000000 tencentcloud-sdk-python-mariadb-3.0.897/tencentcloud/mariadb/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    70751 2023-05-23 02:26:22.000000 tencentcloud-sdk-python-mariadb-3.0.897/tencentcloud/mariadb/v20170312/mariadb_client.py
+-rw-r--r--   0 root         (0) root         (0)    14808 2023-05-23 02:26:22.000000 tencentcloud-sdk-python-mariadb-3.0.897/tencentcloud/mariadb/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:26:22.000000 tencentcloud-sdk-python-mariadb-3.0.897/tencentcloud/mariadb/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   216004 2023-05-23 02:26:22.000000 tencentcloud-sdk-python-mariadb-3.0.897/tencentcloud/mariadb/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:26:22.000000 tencentcloud-sdk-python-mariadb-3.0.897/tencentcloud/mariadb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-23 02:26:22.000000 tencentcloud-sdk-python-mariadb-3.0.897/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-23 02:26:22.000000 tencentcloud-sdk-python-mariadb-3.0.897/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:26:22.000000 tencentcloud-sdk-python-mariadb-3.0.897/setup.cfg
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.896/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mariadb-3.0.897/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mariadb
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Mariadb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.896/README.rst` & `tencentcloud-sdk-python-mariadb-3.0.897/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mariadb-3.0.896/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mariadb-3.0.897/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mariadb-3.0.896/tencentcloud/mariadb/v20170312/mariadb_client.py` & `tencentcloud-sdk-python-mariadb-3.0.897/tencentcloud/mariadb/v20170312/mariadb_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1645,8 +1645,31 @@
             model = models.UpgradeDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def UpgradeDedicatedDBInstance(self, request):
+        """本接口(UpgradeDedicatedDBInstance)用于扩容独享云数据库实例。
+
+        :param request: Request instance for UpgradeDedicatedDBInstance.
+        :type request: :class:`tencentcloud.mariadb.v20170312.models.UpgradeDedicatedDBInstanceRequest`
+        :rtype: :class:`tencentcloud.mariadb.v20170312.models.UpgradeDedicatedDBInstanceResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UpgradeDedicatedDBInstance", params, headers=headers)
+            response = json.loads(body)
+            model = models.UpgradeDedicatedDBInstanceResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
                 raise TencentCloudSDKException(e.message, e.message)
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.896/tencentcloud/mariadb/v20170312/errorcodes.py` & `tencentcloud-sdk-python-mariadb-3.0.897/tencentcloud/mariadb/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mariadb-3.0.896/tencentcloud/mariadb/v20170312/models.py` & `tencentcloud-sdk-python-mariadb-3.0.897/tencentcloud/mariadb/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6124,14 +6124,81 @@
 
 
     def _deserialize(self, params):
         self.DealName = params.get("DealName")
         self.RequestId = params.get("RequestId")
 
 
+class UpgradeDedicatedDBInstanceRequest(AbstractModel):
+    """UpgradeDedicatedDBInstance请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 待升级的实例ID。形如：tdsql-ow728lmc，可以通过 DescribeDBInstances 查询实例获得。
+        :type InstanceId: str
+        :param Memory: 内存大小，单位：GB，可以通过 DescribeFenceDBInstanceSpecs
+ 查询实例规格获得。
+        :type Memory: int
+        :param Storage: 存储空间大小，单位：GB，可以通过 DescribeFenceDBInstanceSpecs
+ 查询实例规格获得不同内存大小对应的磁盘规格下限和上限。
+        :type Storage: int
+        :param SwitchAutoRetry: 错过切换时间窗口时，是否自动重试一次，0-否，1-是
+        :type SwitchAutoRetry: int
+        :param SwitchStartTime: 切换时间窗口开始时间
+        :type SwitchStartTime: str
+        :param SwitchEndTime: 切换时间窗口结束时间
+        :type SwitchEndTime: str
+        """
+        self.InstanceId = None
+        self.Memory = None
+        self.Storage = None
+        self.SwitchAutoRetry = None
+        self.SwitchStartTime = None
+        self.SwitchEndTime = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.Memory = params.get("Memory")
+        self.Storage = params.get("Storage")
+        self.SwitchAutoRetry = params.get("SwitchAutoRetry")
+        self.SwitchStartTime = params.get("SwitchStartTime")
+        self.SwitchEndTime = params.get("SwitchEndTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpgradeDedicatedDBInstanceResponse(AbstractModel):
+    """UpgradeDedicatedDBInstance返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FlowId: 异步流程Id
+        :type FlowId: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.FlowId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.FlowId = params.get("FlowId")
+        self.RequestId = params.get("RequestId")
+
+
 class ViewPrivileges(AbstractModel):
     """视图权限信息
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.896/PKG-INFO` & `tencentcloud-sdk-python-mariadb-3.0.897/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mariadb
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Mariadb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.896/setup.py` & `tencentcloud-sdk-python-mariadb-3.0.897/setup.py`

 * *Files identical despite different names*

