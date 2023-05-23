# Comparing `tmp/tencentcloud-sdk-python-cdn-3.0.896.tar.gz` & `tmp/tencentcloud-sdk-python-cdn-3.0.897.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.896.tar", last modified: Mon May 22 00:17:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.897.tar", last modified: Tue May 23 02:16:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdn-3.0.896.tar` & `tencentcloud-sdk-python-cdn-3.0.897.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:17:22.000000 tencentcloud-sdk-python-cdn-3.0.896/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-22 00:17:22.000000 tencentcloud-sdk-python-cdn-3.0.896/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:17:22.000000 tencentcloud-sdk-python-cdn-3.0.896/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:17:22.000000 tencentcloud-sdk-python-cdn-3.0.896/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:17:22.000000 tencentcloud-sdk-python-cdn-3.0.896/tencentcloud/cdn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:17:22.000000 tencentcloud-sdk-python-cdn-3.0.896/tencentcloud/cdn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:17:22.000000 tencentcloud-sdk-python-cdn-3.0.896/tencentcloud/cdn/v20180606/
--rw-r--r--   0 root         (0) root         (0)    21972 2023-05-22 00:17:22.000000 tencentcloud-sdk-python-cdn-3.0.896/tencentcloud/cdn/v20180606/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    80657 2023-05-22 00:17:22.000000 tencentcloud-sdk-python-cdn-3.0.896/tencentcloud/cdn/v20180606/cdn_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:17:22.000000 tencentcloud-sdk-python-cdn-3.0.896/tencentcloud/cdn/v20180606/__init__.py
--rw-r--r--   0 root         (0) root         (0)   571918 2023-05-22 00:17:22.000000 tencentcloud-sdk-python-cdn-3.0.896/tencentcloud/cdn/v20180606/models.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:17:22.000000 tencentcloud-sdk-python-cdn-3.0.896/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:17:22.000000 tencentcloud-sdk-python-cdn-3.0.896/tencentcloud_sdk_python_cdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:17:22.000000 tencentcloud-sdk-python-cdn-3.0.896/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-22 00:17:22.000000 tencentcloud-sdk-python-cdn-3.0.896/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:17:22.000000 tencentcloud-sdk-python-cdn-3.0.896/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:17:22.000000 tencentcloud-sdk-python-cdn-3.0.896/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-22 00:17:22.000000 tencentcloud-sdk-python-cdn-3.0.896/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:17:22.000000 tencentcloud-sdk-python-cdn-3.0.896/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:16:34.000000 tencentcloud-sdk-python-cdn-3.0.897/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-23 02:16:34.000000 tencentcloud-sdk-python-cdn-3.0.897/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:16:34.000000 tencentcloud-sdk-python-cdn-3.0.897/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:16:34.000000 tencentcloud-sdk-python-cdn-3.0.897/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:16:34.000000 tencentcloud-sdk-python-cdn-3.0.897/tencentcloud/cdn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:16:34.000000 tencentcloud-sdk-python-cdn-3.0.897/tencentcloud/cdn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:16:34.000000 tencentcloud-sdk-python-cdn-3.0.897/tencentcloud/cdn/v20180606/
+-rw-r--r--   0 root         (0) root         (0)    21972 2023-05-23 02:16:34.000000 tencentcloud-sdk-python-cdn-3.0.897/tencentcloud/cdn/v20180606/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    80657 2023-05-23 02:16:34.000000 tencentcloud-sdk-python-cdn-3.0.897/tencentcloud/cdn/v20180606/cdn_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:16:34.000000 tencentcloud-sdk-python-cdn-3.0.897/tencentcloud/cdn/v20180606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   572032 2023-05-23 02:16:34.000000 tencentcloud-sdk-python-cdn-3.0.897/tencentcloud/cdn/v20180606/models.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:16:34.000000 tencentcloud-sdk-python-cdn-3.0.897/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:16:34.000000 tencentcloud-sdk-python-cdn-3.0.897/tencentcloud_sdk_python_cdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:16:34.000000 tencentcloud-sdk-python-cdn-3.0.897/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-23 02:16:34.000000 tencentcloud-sdk-python-cdn-3.0.897/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:16:34.000000 tencentcloud-sdk-python-cdn-3.0.897/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:16:34.000000 tencentcloud-sdk-python-cdn-3.0.897/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-23 02:16:34.000000 tencentcloud-sdk-python-cdn-3.0.897/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:16:34.000000 tencentcloud-sdk-python-cdn-3.0.897/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.896/README.rst` & `tencentcloud-sdk-python-cdn-3.0.897/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.896/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdn-3.0.897/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdn-3.0.896/tencentcloud/cdn/v20180606/errorcodes.py` & `tencentcloud-sdk-python-cdn-3.0.897/tencentcloud/cdn/v20180606/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.896/tencentcloud/cdn/v20180606/cdn_client.py` & `tencentcloud-sdk-python-cdn-3.0.897/tencentcloud/cdn/v20180606/cdn_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.896/tencentcloud/cdn/v20180606/models.py` & `tencentcloud-sdk-python-cdn-3.0.897/tencentcloud/cdn/v20180606/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -947,15 +947,17 @@
         :type RuleName: str
         :param DetectionTime: 探测时长
 注意：此字段可能返回 null，表示取不到有效值。
         :type DetectionTime: int
         :param FrequencyLimit: 限频阈值
 注意：此字段可能返回 null，表示取不到有效值。
         :type FrequencyLimit: int
-        :param PunishmentSwitch: IP 惩罚开关，可选on|off
+        :param PunishmentSwitch: IP 惩罚配置开关，取值有：
+on：开启
+off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type PunishmentSwitch: str
         :param PunishmentTime: IP 惩罚时长
 注意：此字段可能返回 null，表示取不到有效值。
         :type PunishmentTime: int
         :param Action: 执行动作，intercept|redirect
 注意：此字段可能返回 null，表示取不到有效值。
@@ -7831,15 +7833,15 @@
         :param Name: 过滤字段名，支持的列表如下：
 - origin：主源站。
 - domain：域名。
 - resourceId：域名id。
 - status：域名状态，online，offline或processing。
 - serviceType：业务类型，web，download，media，hybrid或dynamic。
 - projectId：项目ID。
-- domainType：主源站类型，cname表示自有源，cos表示cos接入，third_party表示第三方对象存储。
+- domainType：主源站类型，cname表示自有源，cos表示cos接入，third_party表示第三方对象存储，igtm表示IGTM多活源。
 - fullUrlCache：全路径缓存，on或off。
 - https：是否配置https，on，off或processing。
 - originPullProtocol：回源协议类型，支持http，follow或https。
 - tagKey：标签键。
         :type Name: str
         :param Value: 过滤字段值。
         :type Value: list of str
@@ -8821,15 +8823,15 @@
     """HTTPS服务，若关闭，下发配置拦截https请求，开启时会产生计费
 
     """
 
     def __init__(self):
         r"""
         :param Switch: HTTPS服务配置开关，取值有：
-on：开启，缺省时默认开启【会产生计费】
+on：开启，缺省时默认开启，会产生计费
 off：关闭，拦截https请求
 
         :type Switch: str
         """
         self.Switch = None
 
 
@@ -10916,14 +10918,15 @@
         :type Origins: list of str
         :param OriginType: 主源站类型
 入参支持以下几种类型：
 domain：域名类型
 domainv6：域名解析V6类型
 cos：对象存储源站
 third_party: 第三方存储源站
+igtm: IGTM多活源
 ip：IP 列表作为源站
 ipv6：源站列表为一个单独的 IPv6 地址
 ip_ipv6：源站列表为多个 IPv4 地址和IPv6 地址
 ip_domain: 支持IP和域名形式源站混填（白名单功能）
 ip_domainv6：源站列表为多个 IPv4 地址以及域名解析v6地址
 ipv6_domain: 源站列表为多个 IPv6 地址以及域名
 ipv6_domainv6：源站列表为多个 IPv6 地址以及域名解析v6地址
@@ -11644,17 +11647,18 @@
 class PostSize(AbstractModel):
     """POST请求上传文件流式传输最大限制
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 是调整POST请求限制，平台默认为32MB。
-关闭：off，
-开启：on。
+        :param Switch: POST请求上传文件流式传输最大限制配置开关，取值有：
+on：开启，平台默认为32MB
+off：关闭
+
         :type Switch: str
         :param MaxSize: 最大限制，取值在1MB和200MB之间。
         :type MaxSize: int
         """
         self.Switch = None
         self.MaxSize = None
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.896/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.897/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.896/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.897/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.896/setup.py` & `tencentcloud-sdk-python-cdn-3.0.897/setup.py`

 * *Files identical despite different names*

