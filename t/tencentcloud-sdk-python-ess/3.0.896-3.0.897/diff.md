# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.896.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.897.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.896.tar", last modified: Mon May 22 00:23:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.897.tar", last modified: Tue May 23 02:22:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.896.tar` & `tencentcloud-sdk-python-ess-3.0.897.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    50900 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    23727 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223240 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    50900 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    23810 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223352 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.896/README.rst` & `tencentcloud-sdk-python-ess-3.0.897/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.896/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.897/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.896/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.897/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.896/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.897/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,14 +244,17 @@
 
 # 实名认证渠道不正确。
 INVALIDPARAMETER_INVALIDVERIFYCHANNEL = 'InvalidParameter.InvalidVerifyChannel'
 
 # 验证码不正确。
 INVALIDPARAMETER_INVALIDVERIFYCODE = 'InvalidParameter.InvalidVerifyCode'
 
+# Limit参数超出最大限制
+INVALIDPARAMETER_LIMIT = 'InvalidParameter.Limit'
+
 # 缺少必填控件的值。
 INVALIDPARAMETER_MISSINGREQUIREDCOMPONENTVALUE = 'InvalidParameter.MissingRequiredComponentValue'
 
 # 不合法的手机号，请检查后重试。
 INVALIDPARAMETER_MOBILE = 'InvalidParameter.Mobile'
 
 # 不合法的用户名称，请修改后重试。
```

### Comparing `tencentcloud-sdk-python-ess-3.0.896/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.897/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -652,14 +652,15 @@
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
@@ -3271,15 +3272,15 @@
         :param Operator: 操作人信息
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param Limit: 返回最大数量，最大为200
         :type Limit: int
         :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param Filters: 查询的关键字段:
-Key:"RoleType",Vales:["1"]查询系统角色，Values:["2]查询自定义角色
+Key:"RoleType",Values:["1"]查询系统角色，Values:["2"]查询自定义角色
 Key:"RoleStatus",Values:["1"]查询启用角色，Values:["2"]查询禁用角色
 Key:"IsGroupRole"，Values:["0"],查询非集团角色，Values:["1"]表示查询集团角色
         :type Filters: list of Filter
         :param Offset: 偏移量，默认为0，最大为2000
         :type Offset: int
         """
         self.Operator = None
@@ -4679,15 +4680,15 @@
         r"""
         :param RoleId: 角色id
 注意：此字段可能返回 null，表示取不到有效值。
         :type RoleId: str
         :param RoleName: 角色名
 注意：此字段可能返回 null，表示取不到有效值。
         :type RoleName: str
-        :param RoleStatus: 角色类型：1-系统角色，2-自定义角色
+        :param RoleStatus: 角色状态，1-启用，2-禁用
 注意：此字段可能返回 null，表示取不到有效值。
         :type RoleStatus: int
         :param IsGroupRole: 是否是集团角色
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsGroupRole: bool
         :param SubOrgIdList: 管辖的子企业列表
 注意：此字段可能返回 null，表示取不到有效值。
```

### Comparing `tencentcloud-sdk-python-ess-3.0.896/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.897/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.896/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.897/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.896/setup.py` & `tencentcloud-sdk-python-ess-3.0.897/setup.py`

 * *Files identical despite different names*

