# Comparing `tmp/tencentcloud-sdk-python-faceid-3.0.896.tar.gz` & `tmp/tencentcloud-sdk-python-faceid-3.0.897.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.896.tar", last modified: Mon May 22 00:23:19 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.897.tar", last modified: Tue May 23 02:22:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-faceid-3.0.896.tar` & `tencentcloud-sdk-python-faceid-3.0.897.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:19.000000 tencentcloud-sdk-python-faceid-3.0.896/
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-22 00:23:19.000000 tencentcloud-sdk-python-faceid-3.0.896/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:19.000000 tencentcloud-sdk-python-faceid-3.0.896/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:19.000000 tencentcloud-sdk-python-faceid-3.0.896/tencentcloud/faceid/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:19.000000 tencentcloud-sdk-python-faceid-3.0.896/tencentcloud/faceid/v20180301/
--rw-r--r--   0 root         (0) root         (0)    34030 2023-05-22 00:23:19.000000 tencentcloud-sdk-python-faceid-3.0.896/tencentcloud/faceid/v20180301/faceid_client.py
--rw-r--r--   0 root         (0) root         (0)     9370 2023-05-22 00:23:19.000000 tencentcloud-sdk-python-faceid-3.0.896/tencentcloud/faceid/v20180301/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:23:19.000000 tencentcloud-sdk-python-faceid-3.0.896/tencentcloud/faceid/v20180301/__init__.py
--rw-r--r--   0 root         (0) root         (0)   141050 2023-05-22 00:23:19.000000 tencentcloud-sdk-python-faceid-3.0.896/tencentcloud/faceid/v20180301/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:23:19.000000 tencentcloud-sdk-python-faceid-3.0.896/tencentcloud/faceid/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:23:19.000000 tencentcloud-sdk-python-faceid-3.0.896/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-05-22 00:23:19.000000 tencentcloud-sdk-python-faceid-3.0.896/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-05-22 00:23:19.000000 tencentcloud-sdk-python-faceid-3.0.896/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:19.000000 tencentcloud-sdk-python-faceid-3.0.896/tencentcloud_sdk_python_faceid.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:23:19.000000 tencentcloud-sdk-python-faceid-3.0.896/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-05-22 00:23:19.000000 tencentcloud-sdk-python-faceid-3.0.896/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-05-22 00:23:19.000000 tencentcloud-sdk-python-faceid-3.0.896/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:23:19.000000 tencentcloud-sdk-python-faceid-3.0.896/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:23:19.000000 tencentcloud-sdk-python-faceid-3.0.896/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:48.000000 tencentcloud-sdk-python-faceid-3.0.897/
+-rw-r--r--   0 root         (0) root         (0)      746 2023-05-23 02:22:48.000000 tencentcloud-sdk-python-faceid-3.0.897/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:48.000000 tencentcloud-sdk-python-faceid-3.0.897/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:48.000000 tencentcloud-sdk-python-faceid-3.0.897/tencentcloud/faceid/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:48.000000 tencentcloud-sdk-python-faceid-3.0.897/tencentcloud/faceid/v20180301/
+-rw-r--r--   0 root         (0) root         (0)    34030 2023-05-23 02:22:48.000000 tencentcloud-sdk-python-faceid-3.0.897/tencentcloud/faceid/v20180301/faceid_client.py
+-rw-r--r--   0 root         (0) root         (0)     9370 2023-05-23 02:22:48.000000 tencentcloud-sdk-python-faceid-3.0.897/tencentcloud/faceid/v20180301/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:22:48.000000 tencentcloud-sdk-python-faceid-3.0.897/tencentcloud/faceid/v20180301/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   141322 2023-05-23 02:22:48.000000 tencentcloud-sdk-python-faceid-3.0.897/tencentcloud/faceid/v20180301/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:22:48.000000 tencentcloud-sdk-python-faceid-3.0.897/tencentcloud/faceid/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:22:48.000000 tencentcloud-sdk-python-faceid-3.0.897/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-05-23 02:22:48.000000 tencentcloud-sdk-python-faceid-3.0.897/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-05-23 02:22:48.000000 tencentcloud-sdk-python-faceid-3.0.897/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:48.000000 tencentcloud-sdk-python-faceid-3.0.897/tencentcloud_sdk_python_faceid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:22:48.000000 tencentcloud-sdk-python-faceid-3.0.897/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-05-23 02:22:48.000000 tencentcloud-sdk-python-faceid-3.0.897/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-05-23 02:22:48.000000 tencentcloud-sdk-python-faceid-3.0.897/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:22:48.000000 tencentcloud-sdk-python-faceid-3.0.897/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:22:48.000000 tencentcloud-sdk-python-faceid-3.0.897/setup.cfg
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.896/README.rst` & `tencentcloud-sdk-python-faceid-3.0.897/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.896/tencentcloud/faceid/v20180301/faceid_client.py` & `tencentcloud-sdk-python-faceid-3.0.897/tencentcloud/faceid/v20180301/faceid_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.896/tencentcloud/faceid/v20180301/errorcodes.py` & `tencentcloud-sdk-python-faceid-3.0.897/tencentcloud/faceid/v20180301/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.896/tencentcloud/faceid/v20180301/models.py` & `tencentcloud-sdk-python-faceid-3.0.897/tencentcloud/faceid/v20180301/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1771,35 +1771,39 @@
         :type IntentionMode: str
         :param IntentionVerifyText: 意愿核身朗读模式使用的文案，若未使用意愿核身朗读功能，该字段无需传入。默认为空，最长可接受120的字符串长度。
         :type IntentionVerifyText: str
         :param IntentionQuestions: 意愿核身问答模式的配置列表。当前仅支持一个问答。
         :type IntentionQuestions: list of IntentionQuestion
         :param IntentionRecognition: 意愿核身过程中识别用户的回答意图，开启后除了IntentionQuestions的Answers列表中的标准回答会通过，近似意图的回答也会通过，默认不开启。
         :type IntentionRecognition: bool
+        :param IsSupportHMTResidentPermitOCR: 是否支持港澳台居住证识别
+        :type IsSupportHMTResidentPermitOCR: bool
         """
         self.InputType = None
         self.UseIntentionVerify = None
         self.IntentionMode = None
         self.IntentionVerifyText = None
         self.IntentionQuestions = None
         self.IntentionRecognition = None
+        self.IsSupportHMTResidentPermitOCR = None
 
 
     def _deserialize(self, params):
         self.InputType = params.get("InputType")
         self.UseIntentionVerify = params.get("UseIntentionVerify")
         self.IntentionMode = params.get("IntentionMode")
         self.IntentionVerifyText = params.get("IntentionVerifyText")
         if params.get("IntentionQuestions") is not None:
             self.IntentionQuestions = []
             for item in params.get("IntentionQuestions"):
                 obj = IntentionQuestion()
                 obj._deserialize(item)
                 self.IntentionQuestions.append(obj)
         self.IntentionRecognition = params.get("IntentionRecognition")
+        self.IsSupportHMTResidentPermitOCR = params.get("IsSupportHMTResidentPermitOCR")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.896/tencentcloud/__init__.py` & `tencentcloud-sdk-python-faceid-3.0.897/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-faceid-3.0.896/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.897/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.896/setup.py` & `tencentcloud-sdk-python-faceid-3.0.897/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.896/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.897/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

