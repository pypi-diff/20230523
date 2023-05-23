# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.896.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.897.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.896.tar", last modified: Mon May 22 00:28:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.897.tar", last modified: Tue May 23 02:28:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.896.tar` & `tencentcloud-sdk-python-ocr-3.0.897.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:28:51.000000 tencentcloud-sdk-python-ocr-3.0.896/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:28:51.000000 tencentcloud-sdk-python-ocr-3.0.896/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:28:51.000000 tencentcloud-sdk-python-ocr-3.0.896/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-22 00:28:51.000000 tencentcloud-sdk-python-ocr-3.0.896/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:28:51.000000 tencentcloud-sdk-python-ocr-3.0.896/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:28:51.000000 tencentcloud-sdk-python-ocr-3.0.896/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-22 00:28:51.000000 tencentcloud-sdk-python-ocr-3.0.896/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:28:51.000000 tencentcloud-sdk-python-ocr-3.0.896/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:28:51.000000 tencentcloud-sdk-python-ocr-3.0.896/tencentcloud/ocr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:28:51.000000 tencentcloud-sdk-python-ocr-3.0.896/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)   113504 2023-05-22 00:28:51.000000 tencentcloud-sdk-python-ocr-3.0.896/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)     5764 2023-05-22 00:28:51.000000 tencentcloud-sdk-python-ocr-3.0.896/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:28:51.000000 tencentcloud-sdk-python-ocr-3.0.896/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)   505665 2023-05-22 00:28:51.000000 tencentcloud-sdk-python-ocr-3.0.896/tencentcloud/ocr/v20181119/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:28:51.000000 tencentcloud-sdk-python-ocr-3.0.896/tencentcloud/ocr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:28:51.000000 tencentcloud-sdk-python-ocr-3.0.896/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:28:51.000000 tencentcloud-sdk-python-ocr-3.0.896/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-22 00:28:51.000000 tencentcloud-sdk-python-ocr-3.0.896/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:28:51.000000 tencentcloud-sdk-python-ocr-3.0.896/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/ocr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)   113504 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)     5764 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   505982 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/ocr/v20181119/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/ocr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.896/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.897/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.896/README.rst` & `tencentcloud-sdk-python-ocr-3.0.897/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.896/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.896/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.896/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/ocr/v20181119/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1812,20 +1812,21 @@
 
     """
 
     def __init__(self):
         r"""
         :param ImageBase64: 图片的 Base64 值。
 支持的图片格式：PNG、JPG、JPEG，暂不支持 GIF 格式。
-支持的图片大小：所下载图片经Base64编码后不超过 7M。图片下载时间不超过 3 秒。
+支持的图片大小：所下载图片经Base64编码后不超过 7M。图片下载时间不超过 3 秒。像素须介于20-10000px之间。
 图片的 ImageUrl、ImageBase64 必须提供一个，如果都提供，只使用 ImageUrl。
+
         :type ImageBase64: str
         :param ImageUrl: 图片的 Url 地址。
 支持的图片格式：PNG、JPG、JPEG，暂不支持 GIF 格式。
-支持的图片大小：所下载图片经 Base64 编码后不超过 7M。图片下载时间不超过 3 秒。
+支持的图片大小：所下载图片经 Base64 编码后不超过 7M。图片下载时间不超过 3 秒。像素须介于20-10000px之间。
 图片存储于腾讯云的 Url 可保障更高的下载速度和稳定性，建议图片存储于腾讯云。
 非腾讯云存储的 Url 速度和稳定性可能受一定影响。
         :type ImageUrl: str
         :param EnableCoordPoint: 单词四点坐标开关，开启可返回图片中单词的四点坐标。
 该参数默认值为false。
         :type EnableCoordPoint: bool
         :param EnableCandWord: 候选字开关，开启可返回识别时多个可能的候选字（每个候选字对应其置信度）。
@@ -3961,20 +3962,25 @@
 
     """
 
     def __init__(self):
         r"""
         :param AutoName: 自动识别的字段名称
         :type AutoName: str
+        :param ConfigName: 定义的字段名称（传key的名称）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ConfigName: str
         """
         self.AutoName = None
+        self.ConfigName = None
 
 
     def _deserialize(self, params):
         self.AutoName = params.get("AutoName")
+        self.ConfigName = params.get("ConfigName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.896/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.896/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.897/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.896/setup.py` & `tencentcloud-sdk-python-ocr-3.0.897/setup.py`

 * *Files identical despite different names*

