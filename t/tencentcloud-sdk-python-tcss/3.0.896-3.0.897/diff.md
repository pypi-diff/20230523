# Comparing `tmp/tencentcloud-sdk-python-tcss-3.0.896.tar.gz` & `tmp/tencentcloud-sdk-python-tcss-3.0.897.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcss-3.0.896.tar", last modified: Mon May 22 00:33:41 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcss-3.0.897.tar", last modified: Tue May 23 02:32:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcss-3.0.896.tar` & `tencentcloud-sdk-python-tcss-3.0.897.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:33:41.000000 tencentcloud-sdk-python-tcss-3.0.896/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-22 00:33:41.000000 tencentcloud-sdk-python-tcss-3.0.896/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:33:41.000000 tencentcloud-sdk-python-tcss-3.0.896/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:33:41.000000 tencentcloud-sdk-python-tcss-3.0.896/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:33:41.000000 tencentcloud-sdk-python-tcss-3.0.896/tencentcloud/tcss/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:33:41.000000 tencentcloud-sdk-python-tcss-3.0.896/tencentcloud/tcss/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:33:41.000000 tencentcloud-sdk-python-tcss-3.0.896/tencentcloud/tcss/v20201101/
--rw-r--r--   0 root         (0) root         (0)   316128 2023-05-22 00:33:41.000000 tencentcloud-sdk-python-tcss-3.0.896/tencentcloud/tcss/v20201101/tcss_client.py
--rw-r--r--   0 root         (0) root         (0)     3916 2023-05-22 00:33:41.000000 tencentcloud-sdk-python-tcss-3.0.896/tencentcloud/tcss/v20201101/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:33:41.000000 tencentcloud-sdk-python-tcss-3.0.896/tencentcloud/tcss/v20201101/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1040070 2023-05-22 00:33:41.000000 tencentcloud-sdk-python-tcss-3.0.896/tencentcloud/tcss/v20201101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:33:41.000000 tencentcloud-sdk-python-tcss-3.0.896/tencentcloud_sdk_python_tcss.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:33:41.000000 tencentcloud-sdk-python-tcss-3.0.896/tencentcloud_sdk_python_tcss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-22 00:33:41.000000 tencentcloud-sdk-python-tcss-3.0.896/tencentcloud_sdk_python_tcss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-22 00:33:41.000000 tencentcloud-sdk-python-tcss-3.0.896/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:33:41.000000 tencentcloud-sdk-python-tcss-3.0.896/tencentcloud_sdk_python_tcss.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-22 00:33:41.000000 tencentcloud-sdk-python-tcss-3.0.896/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-22 00:33:41.000000 tencentcloud-sdk-python-tcss-3.0.896/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:33:41.000000 tencentcloud-sdk-python-tcss-3.0.896/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:32:31.000000 tencentcloud-sdk-python-tcss-3.0.897/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-23 02:32:31.000000 tencentcloud-sdk-python-tcss-3.0.897/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:32:31.000000 tencentcloud-sdk-python-tcss-3.0.897/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:32:31.000000 tencentcloud-sdk-python-tcss-3.0.897/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:32:31.000000 tencentcloud-sdk-python-tcss-3.0.897/tencentcloud/tcss/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:32:31.000000 tencentcloud-sdk-python-tcss-3.0.897/tencentcloud/tcss/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:32:31.000000 tencentcloud-sdk-python-tcss-3.0.897/tencentcloud/tcss/v20201101/
+-rw-r--r--   0 root         (0) root         (0)   316128 2023-05-23 02:32:31.000000 tencentcloud-sdk-python-tcss-3.0.897/tencentcloud/tcss/v20201101/tcss_client.py
+-rw-r--r--   0 root         (0) root         (0)     3916 2023-05-23 02:32:31.000000 tencentcloud-sdk-python-tcss-3.0.897/tencentcloud/tcss/v20201101/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:32:31.000000 tencentcloud-sdk-python-tcss-3.0.897/tencentcloud/tcss/v20201101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1040213 2023-05-23 02:32:31.000000 tencentcloud-sdk-python-tcss-3.0.897/tencentcloud/tcss/v20201101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:32:31.000000 tencentcloud-sdk-python-tcss-3.0.897/tencentcloud_sdk_python_tcss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:32:31.000000 tencentcloud-sdk-python-tcss-3.0.897/tencentcloud_sdk_python_tcss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-23 02:32:31.000000 tencentcloud-sdk-python-tcss-3.0.897/tencentcloud_sdk_python_tcss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-23 02:32:31.000000 tencentcloud-sdk-python-tcss-3.0.897/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:32:31.000000 tencentcloud-sdk-python-tcss-3.0.897/tencentcloud_sdk_python_tcss.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-23 02:32:31.000000 tencentcloud-sdk-python-tcss-3.0.897/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-23 02:32:31.000000 tencentcloud-sdk-python-tcss-3.0.897/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:32:31.000000 tencentcloud-sdk-python-tcss-3.0.897/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.896/README.rst` & `tencentcloud-sdk-python-tcss-3.0.897/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.896/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcss-3.0.897/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcss-3.0.896/tencentcloud/tcss/v20201101/tcss_client.py` & `tencentcloud-sdk-python-tcss-3.0.897/tencentcloud/tcss/v20201101/tcss_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.896/tencentcloud/tcss/v20201101/errorcodes.py` & `tencentcloud-sdk-python-tcss-3.0.897/tencentcloud/tcss/v20201101/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.896/tencentcloud/tcss/v20201101/models.py` & `tencentcloud-sdk-python-tcss-3.0.897/tencentcloud/tcss/v20201101/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -21922,14 +21922,16 @@
         :type RegionID: int
         :param Project: 所属项目
 注意：此字段可能返回 null，表示取不到有效值。
         :type Project: :class:`tencentcloud.tcss.v20201101.models.ProjectInfo`
         :param Tags: 标签
 注意：此字段可能返回 null，表示取不到有效值。
         :type Tags: list of TagInfo
+        :param ClusterID: 集群id
+        :type ClusterID: str
         """
         self.HostID = None
         self.HostIP = None
         self.HostName = None
         self.Group = None
         self.DockerVersion = None
         self.DockerFileSystemDriver = None
@@ -21940,14 +21942,15 @@
         self.MachineType = None
         self.PublicIp = None
         self.Uuid = None
         self.InstanceID = None
         self.RegionID = None
         self.Project = None
         self.Tags = None
+        self.ClusterID = None
 
 
     def _deserialize(self, params):
         self.HostID = params.get("HostID")
         self.HostIP = params.get("HostIP")
         self.HostName = params.get("HostName")
         self.Group = params.get("Group")
@@ -21967,14 +21970,15 @@
             self.Project._deserialize(params.get("Project"))
         if params.get("Tags") is not None:
             self.Tags = []
             for item in params.get("Tags"):
                 obj = TagInfo()
                 obj._deserialize(item)
                 self.Tags.append(obj)
+        self.ClusterID = params.get("ClusterID")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.896/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcss-3.0.897/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcss
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Tcss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.896/PKG-INFO` & `tencentcloud-sdk-python-tcss-3.0.897/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcss
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Tcss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.896/setup.py` & `tencentcloud-sdk-python-tcss-3.0.897/setup.py`

 * *Files identical despite different names*

