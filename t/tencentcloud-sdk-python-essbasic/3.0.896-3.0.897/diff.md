# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.896.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.897.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.896.tar", last modified: Mon May 22 00:23:06 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.897.tar", last modified: Tue May 23 02:22:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.896.tar` & `tencentcloud-sdk-python-essbasic-3.0.897.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    15673 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    50877 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   230804 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)    15914 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    50877 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   230929 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:22:34.000000 tencentcloud-sdk-python-essbasic-3.0.897/setup.cfg
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.896/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.897/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 
 # 合同数目超出。
 FAILEDOPERATION_FLOWNUMEXCEED = 'FailedOperation.FlowNumExceed'
 
 # 已授权。
 FAILEDOPERATION_HASAUTHORIZED = 'FailedOperation.HasAuthorized'
 
+# 无角色授权，请确认数据是否存在
+FAILEDOPERATION_NOROLEAUTH = 'FailedOperation.NoRoleAuth'
+
 # 当前合同状态无法进行签署审批。
 FAILEDOPERATION_NOTAVAILABLESIGNREVIEW = 'FailedOperation.NotAvailableSignReview'
 
 # 发起签署存在填写控件。
 FAILEDOPERATION_QRCODECREATORSIGNCOMPONENTS = 'FailedOperation.QrCodeCreatorSignComponents'
 
 # 模板签署人不存在。
@@ -388,14 +391,17 @@
 
 # 超出查询上限。
 OPERATIONDENIED_OUTQUERYLIMIT = 'OperationDenied.OutQueryLimit'
 
 # 当前企业员工没有开通境外签署能力。
 OPERATIONDENIED_OVERSEAABILITYNOTOPEN = 'OperationDenied.OverseaAbilityNotOpen'
 
+# 该用户已关闭或者未开启自动签服务
+OPERATIONDENIED_PERSONNOOPENSERVERSIGN = 'OperationDenied.PersonNoOpenServerSign'
+
 # 出证计费额度不足。
 OPERATIONDENIED_PROVENOQUOTA = 'OperationDenied.ProveNoQuota'
 
 # 必填控件未填
 OPERATIONDENIED_REQUIREDCOMPONENTNOTFILL = 'OperationDenied.RequiredComponentNotFill'
 
 # 用户不归属于当前企业，无法操作，请检查后重试。
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2392,14 +2392,15 @@
 ComponentType为SIGN_SIGNATURE类型可以控制签署方式
 {“ComponentTypeLimit”: [“xxx”]}
 xxx可以为：
 HANDWRITE – 手写签名
 BORDERLESS_ESIGN – 自动生成无边框腾讯体
 OCR_ESIGN -- AI智能识别手写签名
 ESIGN -- 个人印章类型
+SYSTEM_ESIGN -- 系统签名（该类型可以在用户签署时根据用户姓名一键生成一个签名来进行签署）
 如：{“ComponentTypeLimit”: [“BORDERLESS_ESIGN”]}
 
 ComponentType为SIGN_DATE时，支持以下参数：
 1 Font：字符串类型目前只支持"黑体"、"宋体"，如果不填默认为"黑体"
 2 FontSize： 数字类型，范围6-72，默认值为12
 3 FontAlign： 字符串类型，可取Left/Right/Center，对应左对齐/居中/右对齐
 4 Format： 字符串类型，日期格式，必须是以下五种之一 “yyyy m d”，”yyyy年m月d日”，”yyyy/m/d”，”yyyy-m-d”，”yyyy.m.d”。
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.897/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.896/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.897/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.896/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.897/setup.py`

 * *Files identical despite different names*

