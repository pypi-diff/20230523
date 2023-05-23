# Comparing `tmp/alibabacloud_paiplugin20220112-1.0.8.tar.gz` & `tmp/alibabacloud_paiplugin20220112-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_paiplugin20220112-1.0.8.tar", last modified: Tue Mar  8 04:02:16 2022, max compression
+gzip compressed data, was "dist/alibabacloud_paiplugin20220112-1.0.9.tar", last modified: Tue Mar  8 07:20:23 2022, max compression
```

## Comparing `alibabacloud_paiplugin20220112-1.0.8.tar` & `alibabacloud_paiplugin20220112-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-08 04:02:16.000000 alibabacloud_paiplugin20220112-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      430 2022-03-08 04:02:15.000000 alibabacloud_paiplugin20220112-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-03-08 04:02:15.000000 alibabacloud_paiplugin20220112-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-03-08 04:02:15.000000 alibabacloud_paiplugin20220112-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2364 2022-03-08 04:02:16.000000 alibabacloud_paiplugin20220112-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2022-03-08 04:02:15.000000 alibabacloud_paiplugin20220112-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2022-03-08 04:02:15.000000 alibabacloud_paiplugin20220112-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-08 04:02:16.000000 alibabacloud_paiplugin20220112-1.0.8/alibabacloud_paiplugin20220112/
--rw-r--r--   0 root         (0) root         (0)       21 2022-03-08 04:02:15.000000 alibabacloud_paiplugin20220112-1.0.8/alibabacloud_paiplugin20220112/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55964 2022-03-08 04:02:15.000000 alibabacloud_paiplugin20220112-1.0.8/alibabacloud_paiplugin20220112/client.py
--rw-r--r--   0 root         (0) root         (0)   104132 2022-03-08 04:02:15.000000 alibabacloud_paiplugin20220112-1.0.8/alibabacloud_paiplugin20220112/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-08 04:02:16.000000 alibabacloud_paiplugin20220112-1.0.8/alibabacloud_paiplugin20220112.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2364 2022-03-08 04:02:15.000000 alibabacloud_paiplugin20220112-1.0.8/alibabacloud_paiplugin20220112.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2022-03-08 04:02:15.000000 alibabacloud_paiplugin20220112-1.0.8/alibabacloud_paiplugin20220112.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-08 04:02:15.000000 alibabacloud_paiplugin20220112-1.0.8/alibabacloud_paiplugin20220112.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-03-08 04:02:15.000000 alibabacloud_paiplugin20220112-1.0.8/alibabacloud_paiplugin20220112.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-03-08 04:02:15.000000 alibabacloud_paiplugin20220112-1.0.8/alibabacloud_paiplugin20220112.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-03-08 04:02:16.000000 alibabacloud_paiplugin20220112-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2640 2022-03-08 04:02:15.000000 alibabacloud_paiplugin20220112-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-08 07:20:23.000000 alibabacloud_paiplugin20220112-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      494 2022-03-08 07:20:23.000000 alibabacloud_paiplugin20220112-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-03-08 07:20:23.000000 alibabacloud_paiplugin20220112-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-03-08 07:20:23.000000 alibabacloud_paiplugin20220112-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2364 2022-03-08 07:20:23.000000 alibabacloud_paiplugin20220112-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1040 2022-03-08 07:20:23.000000 alibabacloud_paiplugin20220112-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2022-03-08 07:20:23.000000 alibabacloud_paiplugin20220112-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-08 07:20:23.000000 alibabacloud_paiplugin20220112-1.0.9/alibabacloud_paiplugin20220112/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-03-08 07:20:23.000000 alibabacloud_paiplugin20220112-1.0.9/alibabacloud_paiplugin20220112/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56174 2022-03-08 07:20:23.000000 alibabacloud_paiplugin20220112-1.0.9/alibabacloud_paiplugin20220112/client.py
+-rw-r--r--   0 root         (0) root         (0)   104471 2022-03-08 07:20:23.000000 alibabacloud_paiplugin20220112-1.0.9/alibabacloud_paiplugin20220112/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-08 07:20:23.000000 alibabacloud_paiplugin20220112-1.0.9/alibabacloud_paiplugin20220112.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2364 2022-03-08 07:20:23.000000 alibabacloud_paiplugin20220112-1.0.9/alibabacloud_paiplugin20220112.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2022-03-08 07:20:23.000000 alibabacloud_paiplugin20220112-1.0.9/alibabacloud_paiplugin20220112.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-08 07:20:23.000000 alibabacloud_paiplugin20220112-1.0.9/alibabacloud_paiplugin20220112.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-03-08 07:20:23.000000 alibabacloud_paiplugin20220112-1.0.9/alibabacloud_paiplugin20220112.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2022-03-08 07:20:23.000000 alibabacloud_paiplugin20220112-1.0.9/alibabacloud_paiplugin20220112.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-03-08 07:20:23.000000 alibabacloud_paiplugin20220112-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2640 2022-03-08 07:20:23.000000 alibabacloud_paiplugin20220112-1.0.9/setup.py
```

### Comparing `alibabacloud_paiplugin20220112-1.0.8/LICENSE` & `alibabacloud_paiplugin20220112-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_paiplugin20220112-1.0.8/PKG-INFO` & `alibabacloud_paiplugin20220112-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_paiplugin20220112
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud PaiPlugin (20220112) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_paiplugin20220112-1.0.8/README-CN.md` & `alibabacloud_paiplugin20220112-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_paiplugin20220112-1.0.8/README.md` & `alibabacloud_paiplugin20220112-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_paiplugin20220112-1.0.8/alibabacloud_paiplugin20220112/client.py` & `alibabacloud_paiplugin20220112-1.0.9/alibabacloud_paiplugin20220112/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,14 +159,16 @@
         body = {}
         if not UtilClient.is_unset(request.content):
             body['Content'] = request.content
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
+        if not UtilClient.is_unset(request.signature):
+            body['Signature'] = request.signature
         if not UtilClient.is_unset(request.signature_id):
             body['SignatureId'] = request.signature_id
         if not UtilClient.is_unset(request.type):
             body['Type'] = request.type
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
@@ -197,14 +199,16 @@
         body = {}
         if not UtilClient.is_unset(request.content):
             body['Content'] = request.content
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
+        if not UtilClient.is_unset(request.signature):
+            body['Signature'] = request.signature
         if not UtilClient.is_unset(request.signature_id):
             body['SignatureId'] = request.signature_id
         if not UtilClient.is_unset(request.type):
             body['Type'] = request.type
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
```

### Comparing `alibabacloud_paiplugin20220112-1.0.8/alibabacloud_paiplugin20220112/models.py` & `alibabacloud_paiplugin20220112-1.0.9/alibabacloud_paiplugin20220112/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,23 +188,26 @@
 
 class CreateTemplateRequest(TeaModel):
     def __init__(
         self,
         content: str = None,
         description: str = None,
         name: str = None,
+        signature: str = None,
         signature_id: str = None,
         type: int = None,
     ):
-        # 模板内容，请注意控制总字数在70个字以内，超出部分按长短信收费，按67个字为单位记一条短信，必须在结尾添加”回T退订“。
+        # 模板内容，请注意控制总字数在70个字以内，超出部分按长短信收费，按67个字为单位记一条短信，营销短信必须在结尾添加“回T退订”。
         self.content = content
         # 申请说明。
         self.description = description
         # 模板名称。
         self.name = name
+        # 签名名称，同时只能指定签名名称或签名Id其中之一。
+        self.signature = signature
         # 签名Id，可通过ListSignatures获取审核状态为已通过的签名列表，获取签名Id。
         self.signature_id = signature_id
         # 模板类型。
         # - 0 : 验证码。
         # - 1 : 短信通知。
         # - 2 : 推广短信。
         self.type = type
@@ -220,28 +223,32 @@
         result = dict()
         if self.content is not None:
             result['Content'] = self.content
         if self.description is not None:
             result['Description'] = self.description
         if self.name is not None:
             result['Name'] = self.name
+        if self.signature is not None:
+            result['Signature'] = self.signature
         if self.signature_id is not None:
             result['SignatureId'] = self.signature_id
         if self.type is not None:
             result['Type'] = self.type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Content') is not None:
             self.content = m.get('Content')
         if m.get('Description') is not None:
             self.description = m.get('Description')
         if m.get('Name') is not None:
             self.name = m.get('Name')
+        if m.get('Signature') is not None:
+            self.signature = m.get('Signature')
         if m.get('SignatureId') is not None:
             self.signature_id = m.get('SignatureId')
         if m.get('Type') is not None:
             self.type = m.get('Type')
         return self
```

### Comparing `alibabacloud_paiplugin20220112-1.0.8/alibabacloud_paiplugin20220112.egg-info/PKG-INFO` & `alibabacloud_paiplugin20220112-1.0.9/alibabacloud_paiplugin20220112.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-paiplugin20220112
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud PaiPlugin (20220112) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_paiplugin20220112-1.0.8/setup.py` & `alibabacloud_paiplugin20220112-1.0.9/setup.py`

 * *Files identical despite different names*

