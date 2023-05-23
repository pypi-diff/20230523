# Comparing `tmp/tencentcloud-sdk-python-cbs-3.0.896.tar.gz` & `tmp/tencentcloud-sdk-python-cbs-3.0.897.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cbs-3.0.896.tar", last modified: Mon May 22 00:16:54 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cbs-3.0.897.tar", last modified: Tue May 23 02:16:08 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cbs-3.0.896.tar` & `tencentcloud-sdk-python-cbs-3.0.897.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:16:54.000000 tencentcloud-sdk-python-cbs-3.0.896/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:16:54.000000 tencentcloud-sdk-python-cbs-3.0.896/tencentcloud_sdk_python_cbs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:16:54.000000 tencentcloud-sdk-python-cbs-3.0.896/tencentcloud_sdk_python_cbs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-22 00:16:54.000000 tencentcloud-sdk-python-cbs-3.0.896/tencentcloud_sdk_python_cbs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:16:54.000000 tencentcloud-sdk-python-cbs-3.0.896/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:16:54.000000 tencentcloud-sdk-python-cbs-3.0.896/tencentcloud_sdk_python_cbs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-22 00:16:54.000000 tencentcloud-sdk-python-cbs-3.0.896/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:16:54.000000 tencentcloud-sdk-python-cbs-3.0.896/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:16:54.000000 tencentcloud-sdk-python-cbs-3.0.896/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:16:54.000000 tencentcloud-sdk-python-cbs-3.0.896/tencentcloud/cbs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:16:54.000000 tencentcloud-sdk-python-cbs-3.0.896/tencentcloud/cbs/v20170312/
--rw-r--r--   0 root         (0) root         (0)     7755 2023-05-22 00:16:54.000000 tencentcloud-sdk-python-cbs-3.0.896/tencentcloud/cbs/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53328 2023-05-22 00:16:54.000000 tencentcloud-sdk-python-cbs-3.0.896/tencentcloud/cbs/v20170312/cbs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:16:54.000000 tencentcloud-sdk-python-cbs-3.0.896/tencentcloud/cbs/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   159351 2023-05-22 00:16:54.000000 tencentcloud-sdk-python-cbs-3.0.896/tencentcloud/cbs/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:16:54.000000 tencentcloud-sdk-python-cbs-3.0.896/tencentcloud/cbs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:16:54.000000 tencentcloud-sdk-python-cbs-3.0.896/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-22 00:16:54.000000 tencentcloud-sdk-python-cbs-3.0.896/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:16:54.000000 tencentcloud-sdk-python-cbs-3.0.896/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:16:08.000000 tencentcloud-sdk-python-cbs-3.0.897/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:16:08.000000 tencentcloud-sdk-python-cbs-3.0.897/tencentcloud_sdk_python_cbs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:16:08.000000 tencentcloud-sdk-python-cbs-3.0.897/tencentcloud_sdk_python_cbs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-23 02:16:08.000000 tencentcloud-sdk-python-cbs-3.0.897/tencentcloud_sdk_python_cbs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:16:08.000000 tencentcloud-sdk-python-cbs-3.0.897/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:16:08.000000 tencentcloud-sdk-python-cbs-3.0.897/tencentcloud_sdk_python_cbs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-23 02:16:08.000000 tencentcloud-sdk-python-cbs-3.0.897/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:16:08.000000 tencentcloud-sdk-python-cbs-3.0.897/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:16:08.000000 tencentcloud-sdk-python-cbs-3.0.897/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:16:08.000000 tencentcloud-sdk-python-cbs-3.0.897/tencentcloud/cbs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:16:08.000000 tencentcloud-sdk-python-cbs-3.0.897/tencentcloud/cbs/v20170312/
+-rw-r--r--   0 root         (0) root         (0)     7755 2023-05-23 02:16:08.000000 tencentcloud-sdk-python-cbs-3.0.897/tencentcloud/cbs/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53328 2023-05-23 02:16:08.000000 tencentcloud-sdk-python-cbs-3.0.897/tencentcloud/cbs/v20170312/cbs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:16:08.000000 tencentcloud-sdk-python-cbs-3.0.897/tencentcloud/cbs/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   159813 2023-05-23 02:16:08.000000 tencentcloud-sdk-python-cbs-3.0.897/tencentcloud/cbs/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:16:08.000000 tencentcloud-sdk-python-cbs-3.0.897/tencentcloud/cbs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:16:08.000000 tencentcloud-sdk-python-cbs-3.0.897/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-23 02:16:08.000000 tencentcloud-sdk-python-cbs-3.0.897/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:16:08.000000 tencentcloud-sdk-python-cbs-3.0.897/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.896/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cbs-3.0.897/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cbs
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Cbs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.896/README.rst` & `tencentcloud-sdk-python-cbs-3.0.897/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cbs-3.0.896/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cbs-3.0.897/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cbs-3.0.896/tencentcloud/cbs/v20170312/errorcodes.py` & `tencentcloud-sdk-python-cbs-3.0.897/tencentcloud/cbs/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cbs-3.0.896/tencentcloud/cbs/v20170312/cbs_client.py` & `tencentcloud-sdk-python-cbs-3.0.897/tencentcloud/cbs/v20170312/cbs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cbs-3.0.896/tencentcloud/cbs/v20170312/models.py` & `tencentcloud-sdk-python-cbs-3.0.897/tencentcloud/cbs/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -739,14 +739,16 @@
         :type DiskChargePrepaid: :class:`tencentcloud.cbs.v20170312.models.DiskChargePrepaid`
         :param DeleteSnapshot: 销毁云盘时删除关联的非永久保留快照。0 表示非永久快照不随云盘销毁而销毁，1表示非永久快照随云盘销毁而销毁，默认取0。快照是否永久保留可以通过DescribeSnapshots接口返回的快照详情的IsPermanent字段来判断，true表示永久快照，false表示非永久快照。
         :type DeleteSnapshot: int
         :param AutoMountConfiguration: 创建云盘时指定自动挂载并初始化该数据盘。
         :type AutoMountConfiguration: :class:`tencentcloud.cbs.v20170312.models.AutoMountConfiguration`
         :param DiskBackupQuota: 指定云硬盘备份点配额。
         :type DiskBackupQuota: int
+        :param BurstPerformance: 创建云盘时是否开启性能突发
+        :type BurstPerformance: bool
         """
         self.Placement = None
         self.DiskChargeType = None
         self.DiskType = None
         self.DiskName = None
         self.Tags = None
         self.SnapshotId = None
@@ -756,14 +758,15 @@
         self.Shareable = None
         self.ClientToken = None
         self.Encrypt = None
         self.DiskChargePrepaid = None
         self.DeleteSnapshot = None
         self.AutoMountConfiguration = None
         self.DiskBackupQuota = None
+        self.BurstPerformance = None
 
 
     def _deserialize(self, params):
         if params.get("Placement") is not None:
             self.Placement = Placement()
             self.Placement._deserialize(params.get("Placement"))
         self.DiskChargeType = params.get("DiskChargeType")
@@ -786,14 +789,15 @@
             self.DiskChargePrepaid = DiskChargePrepaid()
             self.DiskChargePrepaid._deserialize(params.get("DiskChargePrepaid"))
         self.DeleteSnapshot = params.get("DeleteSnapshot")
         if params.get("AutoMountConfiguration") is not None:
             self.AutoMountConfiguration = AutoMountConfiguration()
             self.AutoMountConfiguration._deserialize(params.get("AutoMountConfiguration"))
         self.DiskBackupQuota = params.get("DiskBackupQuota")
+        self.BurstPerformance = params.get("BurstPerformance")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2843,30 +2847,34 @@
         :type Portable: bool
         :param ProjectId: 新的云硬盘项目ID，只支持修改弹性云盘的项目ID。通过[DescribeProject](/document/api/378/4400)接口查询可用项目及其ID。
         :type ProjectId: int
         :param DeleteWithInstance: 成功挂载到云主机后该云硬盘是否随云主机销毁，TRUE表示随云主机销毁，FALSE表示不随云主机销毁。仅支持按量计费云硬盘数据盘。
         :type DeleteWithInstance: bool
         :param DiskType: 变更云盘类型时，可传入该参数，表示变更的目标类型，取值范围：<br><li>CLOUD_PREMIUM：表示高性能云硬盘<br><li>CLOUD_SSD：表示SSD云硬盘。<br>当前不支持批量变更类型，即传入DiskType时，DiskIds仅支持传入一块云盘；<br>变更云盘类型时不支持同时变更其他属性。
         :type DiskType: str
+        :param BurstPerformanceOperation: 开启/关闭云盘性能突发功能
+        :type BurstPerformanceOperation: str
         """
         self.DiskIds = None
         self.DiskName = None
         self.Portable = None
         self.ProjectId = None
         self.DeleteWithInstance = None
         self.DiskType = None
+        self.BurstPerformanceOperation = None
 
 
     def _deserialize(self, params):
         self.DiskIds = params.get("DiskIds")
         self.DiskName = params.get("DiskName")
         self.Portable = params.get("Portable")
         self.ProjectId = params.get("ProjectId")
         self.DeleteWithInstance = params.get("DeleteWithInstance")
         self.DiskType = params.get("DiskType")
+        self.BurstPerformanceOperation = params.get("BurstPerformanceOperation")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.896/PKG-INFO` & `tencentcloud-sdk-python-cbs-3.0.897/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cbs
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Cbs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.896/setup.py` & `tencentcloud-sdk-python-cbs-3.0.897/setup.py`

 * *Files identical despite different names*

