# Comparing `tmp/tencentcloud-sdk-python-lighthouse-3.0.896.tar.gz` & `tmp/tencentcloud-sdk-python-lighthouse-3.0.897.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.896.tar", last modified: Mon May 22 00:26:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.897.tar", last modified: Tue May 23 02:25:56 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lighthouse-3.0.896.tar` & `tencentcloud-sdk-python-lighthouse-3.0.897.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:26:39.000000 tencentcloud-sdk-python-lighthouse-3.0.896/
--rw-r--r--   0 root         (0) root         (0)      758 2023-05-22 00:26:39.000000 tencentcloud-sdk-python-lighthouse-3.0.896/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:26:39.000000 tencentcloud-sdk-python-lighthouse-3.0.896/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:26:39.000000 tencentcloud-sdk-python-lighthouse-3.0.896/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:26:39.000000 tencentcloud-sdk-python-lighthouse-3.0.896/tencentcloud/lighthouse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:26:39.000000 tencentcloud-sdk-python-lighthouse-3.0.896/tencentcloud/lighthouse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:26:39.000000 tencentcloud-sdk-python-lighthouse-3.0.896/tencentcloud/lighthouse/v20200324/
--rw-r--r--   0 root         (0) root         (0)    25956 2023-05-22 00:26:39.000000 tencentcloud-sdk-python-lighthouse-3.0.896/tencentcloud/lighthouse/v20200324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    92541 2023-05-22 00:26:39.000000 tencentcloud-sdk-python-lighthouse-3.0.896/tencentcloud/lighthouse/v20200324/lighthouse_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:26:39.000000 tencentcloud-sdk-python-lighthouse-3.0.896/tencentcloud/lighthouse/v20200324/__init__.py
--rw-r--r--   0 root         (0) root         (0)   240429 2023-05-22 00:26:39.000000 tencentcloud-sdk-python-lighthouse-3.0.896/tencentcloud/lighthouse/v20200324/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:26:39.000000 tencentcloud-sdk-python-lighthouse-3.0.896/tencentcloud_sdk_python_lighthouse.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:26:39.000000 tencentcloud-sdk-python-lighthouse-3.0.896/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-05-22 00:26:39.000000 tencentcloud-sdk-python-lighthouse-3.0.896/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-05-22 00:26:39.000000 tencentcloud-sdk-python-lighthouse-3.0.896/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:26:39.000000 tencentcloud-sdk-python-lighthouse-3.0.896/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-05-22 00:26:39.000000 tencentcloud-sdk-python-lighthouse-3.0.896/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-05-22 00:26:39.000000 tencentcloud-sdk-python-lighthouse-3.0.896/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:26:39.000000 tencentcloud-sdk-python-lighthouse-3.0.896/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:25:56.000000 tencentcloud-sdk-python-lighthouse-3.0.897/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-05-23 02:25:56.000000 tencentcloud-sdk-python-lighthouse-3.0.897/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:25:56.000000 tencentcloud-sdk-python-lighthouse-3.0.897/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:25:56.000000 tencentcloud-sdk-python-lighthouse-3.0.897/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:25:56.000000 tencentcloud-sdk-python-lighthouse-3.0.897/tencentcloud/lighthouse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:25:56.000000 tencentcloud-sdk-python-lighthouse-3.0.897/tencentcloud/lighthouse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:25:56.000000 tencentcloud-sdk-python-lighthouse-3.0.897/tencentcloud/lighthouse/v20200324/
+-rw-r--r--   0 root         (0) root         (0)    25956 2023-05-23 02:25:56.000000 tencentcloud-sdk-python-lighthouse-3.0.897/tencentcloud/lighthouse/v20200324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    92541 2023-05-23 02:25:56.000000 tencentcloud-sdk-python-lighthouse-3.0.897/tencentcloud/lighthouse/v20200324/lighthouse_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:25:56.000000 tencentcloud-sdk-python-lighthouse-3.0.897/tencentcloud/lighthouse/v20200324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   240370 2023-05-23 02:25:56.000000 tencentcloud-sdk-python-lighthouse-3.0.897/tencentcloud/lighthouse/v20200324/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:25:56.000000 tencentcloud-sdk-python-lighthouse-3.0.897/tencentcloud_sdk_python_lighthouse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:25:56.000000 tencentcloud-sdk-python-lighthouse-3.0.897/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-05-23 02:25:56.000000 tencentcloud-sdk-python-lighthouse-3.0.897/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-05-23 02:25:56.000000 tencentcloud-sdk-python-lighthouse-3.0.897/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:25:56.000000 tencentcloud-sdk-python-lighthouse-3.0.897/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-05-23 02:25:56.000000 tencentcloud-sdk-python-lighthouse-3.0.897/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-05-23 02:25:56.000000 tencentcloud-sdk-python-lighthouse-3.0.897/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:25:56.000000 tencentcloud-sdk-python-lighthouse-3.0.897/setup.cfg
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.896/README.rst` & `tencentcloud-sdk-python-lighthouse-3.0.897/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.896/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lighthouse-3.0.897/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.896/tencentcloud/lighthouse/v20200324/errorcodes.py` & `tencentcloud-sdk-python-lighthouse-3.0.897/tencentcloud/lighthouse/v20200324/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.896/tencentcloud/lighthouse/v20200324/lighthouse_client.py` & `tencentcloud-sdk-python-lighthouse-3.0.897/tencentcloud/lighthouse/v20200324/lighthouse_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.896/tencentcloud/lighthouse/v20200324/models.py` & `tencentcloud-sdk-python-lighthouse-3.0.897/tencentcloud/lighthouse/v20200324/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -501,19 +501,19 @@
         r"""
         :param BundleId: 套餐 ID。
         :type BundleId: str
         :param Memory: 内存大小，单位 GB。
         :type Memory: int
         :param SystemDiskType: 系统盘类型。
 取值范围： 
-<li> LOCAL_BASIC：本地硬盘</li><li> LOCAL_SSD：本地 SSD 硬盘</li><li> CLOUD_BASIC：普通云硬盘</li><li> CLOUD_SSD：SSD 云硬盘</li><li> CLOUD_PREMIUM：高性能云硬盘</li>
+<li> CLOUD_SSD：SSD 云硬盘</li><li> CLOUD_PREMIUM：高性能云硬盘</li>
         :type SystemDiskType: str
-        :param SystemDiskSize: 系统盘大小。
+        :param SystemDiskSize: 系统盘大小。单位GB。
         :type SystemDiskSize: int
-        :param MonthlyTraffic: 每月网络流量，单位 Gb。
+        :param MonthlyTraffic: 每月网络流量，单位 GB。
         :type MonthlyTraffic: int
         :param SupportLinuxUnixPlatform: 是否支持 Linux/Unix 平台。
         :type SupportLinuxUnixPlatform: bool
         :param SupportWindowsPlatform: 是否支持 Windows 平台。
         :type SupportWindowsPlatform: bool
         :param Price: 套餐当前单位价格信息。
         :type Price: :class:`tencentcloud.lighthouse.v20200324.models.Price`
@@ -1685,23 +1685,23 @@
         :param Limit: 返回数量，默认为 20，最大值为 100。关于`Limit`的更进一步介绍请参考 API [简介](https://cloud.tencent.com/document/product/1207/47578)中的相关小节。
         :type Limit: int
         :param Filters: 过滤器列表。
 <li>bundle-id</li>按照【套餐 ID】进行过滤。
 类型：String
 必选：否
 <li>support-platform-type</li>按照【系统类型】进行过滤。
-取值： LINUX_UNIX（Linux/Unix系统）；WINDOWS（Windows 系统）
+取值： LINUX_UNIX(Linux/Unix系统) ;WINDOWS(Windows 系统)
 类型：String
 必选：否
 <li>bundle-type</li>按照 【套餐类型进行过滤】。
-取值：GENERAL_BUNDLE (通用型套餐); STORAGE_BUNDLE(存储型套餐);ENTERPRISE_BUNDLE( 企业型套餐);EXCLUSIVE_BUNDLE(专属型套餐);BEFAST_BUNDLE(蜂驰型套餐);
+取值：GENERAL_BUNDLE (通用型套餐); STORAGE_BUNDLE(存储型套餐);ENTERPRISE_BUNDLE( 企业型套餐);EXCLUSIVE_BUNDLE(专属型套餐);BEFAST_BUNDLE(蜂驰型套餐);STARTER_BUNDLE(入门型套餐);CAREFREE_BUNDLE(无忧型套餐);
 类型：String
 必选：否
 <li>bundle-state</li>按照【套餐状态】进行过滤。
-取值: ‘ONLINE’(在线); ‘OFFLINE’(下线);
+取值: ONLINE(在线); OFFLINE(下线);
 类型：String
 必选：否
 每次请求的 Filters 的上限为 10，Filter.Values 的上限为 5。参数不支持同时指定 BundleIds 和 Filters。
         :type Filters: list of Filter
         :param Zones: 可用区列表。默认为全部可用区。
         :type Zones: list of str
         """
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.896/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-lighthouse-3.0.897/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.896/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.897/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.896/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.897/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.896/setup.py` & `tencentcloud-sdk-python-lighthouse-3.0.897/setup.py`

 * *Files identical despite different names*

