# Comparing `tmp/alibabacloud_avatar20220130_py2-1.0.2.tar.gz` & `tmp/alibabacloud_avatar20220130_py2-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_avatar20220130_py2-1.0.2.tar", last modified: Wed Jul 27 09:32:32 2022, max compression
+gzip compressed data, was "dist/alibabacloud_avatar20220130_py2-1.0.3.tar", last modified: Thu Jul 28 03:49:33 2022, max compression
```

## Comparing `alibabacloud_avatar20220130_py2-1.0.2.tar` & `alibabacloud_avatar20220130_py2-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 09:32:32.000000 alibabacloud_avatar20220130_py2-1.0.2/
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-27 09:32:32.000000 alibabacloud_avatar20220130_py2-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-07-27 09:32:32.000000 alibabacloud_avatar20220130_py2-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-07-27 09:32:32.000000 alibabacloud_avatar20220130_py2-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2490 2022-07-27 09:32:32.000000 alibabacloud_avatar20220130_py2-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1042 2022-07-27 09:32:32.000000 alibabacloud_avatar20220130_py2-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2022-07-27 09:32:32.000000 alibabacloud_avatar20220130_py2-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 09:32:32.000000 alibabacloud_avatar20220130_py2-1.0.2/alibabacloud_avatar20220130/
--rw-r--r--   0 root         (0) root         (0)       21 2022-07-27 09:32:32.000000 alibabacloud_avatar20220130_py2-1.0.2/alibabacloud_avatar20220130/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7069 2022-07-27 09:32:32.000000 alibabacloud_avatar20220130_py2-1.0.2/alibabacloud_avatar20220130/client.py
--rw-r--r--   0 root         (0) root         (0)    32681 2022-07-27 09:32:32.000000 alibabacloud_avatar20220130_py2-1.0.2/alibabacloud_avatar20220130/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 09:32:32.000000 alibabacloud_avatar20220130_py2-1.0.2/alibabacloud_avatar20220130_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2490 2022-07-27 09:32:32.000000 alibabacloud_avatar20220130_py2-1.0.2/alibabacloud_avatar20220130_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2022-07-27 09:32:32.000000 alibabacloud_avatar20220130_py2-1.0.2/alibabacloud_avatar20220130_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-27 09:32:32.000000 alibabacloud_avatar20220130_py2-1.0.2/alibabacloud_avatar20220130_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-07-27 09:32:32.000000 alibabacloud_avatar20220130_py2-1.0.2/alibabacloud_avatar20220130_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2022-07-27 09:32:32.000000 alibabacloud_avatar20220130_py2-1.0.2/alibabacloud_avatar20220130_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-07-27 09:32:32.000000 alibabacloud_avatar20220130_py2-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2918 2022-07-27 09:32:32.000000 alibabacloud_avatar20220130_py2-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      139 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2490 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1042 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7719 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130/client.py
+-rw-r--r--   0 root         (0) root         (0)    35687 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2490 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2918 2022-07-28 03:49:33.000000 alibabacloud_avatar20220130_py2-1.0.3/setup.py
```

### Comparing `alibabacloud_avatar20220130_py2-1.0.2/LICENSE` & `alibabacloud_avatar20220130_py2-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_avatar20220130_py2-1.0.2/PKG-INFO` & `alibabacloud_avatar20220130_py2-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_avatar20220130_py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud avatar (20220130) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_avatar20220130_py2-1.0.2/README-CN.md` & `alibabacloud_avatar20220130_py2-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_avatar20220130_py2-1.0.2/README.md` & `alibabacloud_avatar20220130_py2-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_avatar20220130_py2-1.0.2/alibabacloud_avatar20220130/client.py` & `alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,21 +66,25 @@
 
     def send_message_with_options(self, tmp_req, runtime):
         UtilClient.validate_model(tmp_req)
         request = avatar_20220130_models.SendMessageShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.text_request):
             request.text_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.text_request), 'TextRequest', 'json')
+        if not UtilClient.is_unset(tmp_req.vamlrequest):
+            request.vamlrequest_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.vamlrequest), 'VAMLRequest', 'json')
         query = {}
         if not UtilClient.is_unset(request.session_id):
             query['SessionId'] = request.session_id
         if not UtilClient.is_unset(request.tenant_id):
             query['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.text_request_shrink):
             query['TextRequest'] = request.text_request_shrink
+        if not UtilClient.is_unset(request.vamlrequest_shrink):
+            query['VAMLRequest'] = request.vamlrequest_shrink
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SendMessage',
             version='2022-01-30',
             protocol='HTTPS',
@@ -102,19 +106,23 @@
 
     def start_instance_with_options(self, tmp_req, runtime):
         UtilClient.validate_model(tmp_req)
         request = avatar_20220130_models.StartInstanceShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.app):
             request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.app), 'App', 'json')
+        if not UtilClient.is_unset(tmp_req.channel):
+            request.channel_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.channel), 'Channel', 'json')
         if not UtilClient.is_unset(tmp_req.user):
             request.user_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user), 'User', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_shrink):
             query['App'] = request.app_shrink
+        if not UtilClient.is_unset(request.channel_shrink):
+            query['Channel'] = request.channel_shrink
         if not UtilClient.is_unset(request.tenant_id):
             query['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.user_shrink):
             query['User'] = request.user_shrink
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
```

### Comparing `alibabacloud_avatar20220130_py2-1.0.2/alibabacloud_avatar20220130/models.py` & `alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -346,55 +346,93 @@
         if m.get('SpeechText') is not None:
             self.speech_text = m.get('SpeechText')
         if m.get('interrupt') is not None:
             self.interrupt = m.get('interrupt')
         return self
 
 
+class SendMessageRequestVAMLRequest(TeaModel):
+    def __init__(self, code=None, vaml=None):
+        self.code = code  # type: str
+        self.vaml = vaml  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SendMessageRequestVAMLRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.vaml is not None:
+            result['Vaml'] = self.vaml
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Vaml') is not None:
+            self.vaml = m.get('Vaml')
+        return self
+
+
 class SendMessageRequest(TeaModel):
-    def __init__(self, session_id=None, tenant_id=None, text_request=None):
+    def __init__(self, session_id=None, tenant_id=None, text_request=None, vamlrequest=None):
         self.session_id = session_id  # type: str
         self.tenant_id = tenant_id  # type: long
         self.text_request = text_request  # type: SendMessageRequestTextRequest
+        self.vamlrequest = vamlrequest  # type: SendMessageRequestVAMLRequest
 
     def validate(self):
         if self.text_request:
             self.text_request.validate()
+        if self.vamlrequest:
+            self.vamlrequest.validate()
 
     def to_map(self):
         _map = super(SendMessageRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.session_id is not None:
             result['SessionId'] = self.session_id
         if self.tenant_id is not None:
             result['TenantId'] = self.tenant_id
         if self.text_request is not None:
             result['TextRequest'] = self.text_request.to_map()
+        if self.vamlrequest is not None:
+            result['VAMLRequest'] = self.vamlrequest.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('SessionId') is not None:
             self.session_id = m.get('SessionId')
         if m.get('TenantId') is not None:
             self.tenant_id = m.get('TenantId')
         if m.get('TextRequest') is not None:
             temp_model = SendMessageRequestTextRequest()
             self.text_request = temp_model.from_map(m['TextRequest'])
+        if m.get('VAMLRequest') is not None:
+            temp_model = SendMessageRequestVAMLRequest()
+            self.vamlrequest = temp_model.from_map(m['VAMLRequest'])
         return self
 
 
 class SendMessageShrinkRequest(TeaModel):
-    def __init__(self, session_id=None, tenant_id=None, text_request_shrink=None):
+    def __init__(self, session_id=None, tenant_id=None, text_request_shrink=None, vamlrequest_shrink=None):
         self.session_id = session_id  # type: str
         self.tenant_id = tenant_id  # type: long
         self.text_request_shrink = text_request_shrink  # type: str
+        self.vamlrequest_shrink = vamlrequest_shrink  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SendMessageShrinkRequest, self).to_map()
         if _map is not None:
@@ -403,24 +441,28 @@
         result = dict()
         if self.session_id is not None:
             result['SessionId'] = self.session_id
         if self.tenant_id is not None:
             result['TenantId'] = self.tenant_id
         if self.text_request_shrink is not None:
             result['TextRequest'] = self.text_request_shrink
+        if self.vamlrequest_shrink is not None:
+            result['VAMLRequest'] = self.vamlrequest_shrink
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('SessionId') is not None:
             self.session_id = m.get('SessionId')
         if m.get('TenantId') is not None:
             self.tenant_id = m.get('TenantId')
         if m.get('TextRequest') is not None:
             self.text_request_shrink = m.get('TextRequest')
+        if m.get('VAMLRequest') is not None:
+            self.vamlrequest_shrink = m.get('VAMLRequest')
         return self
 
 
 class SendMessageResponseBodyData(TeaModel):
     def __init__(self, request_id=None, session_id=None):
         self.request_id = request_id  # type: str
         self.session_id = session_id  # type: str
@@ -549,14 +591,43 @@
     def from_map(self, m=None):
         m = m or dict()
         if m.get('AppId') is not None:
             self.app_id = m.get('AppId')
         return self
 
 
+class StartInstanceRequestChannel(TeaModel):
+    def __init__(self, req_config=None, type=None):
+        self.req_config = req_config  # type: dict[str, any]
+        self.type = type  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(StartInstanceRequestChannel, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_config is not None:
+            result['ReqConfig'] = self.req_config
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ReqConfig') is not None:
+            self.req_config = m.get('ReqConfig')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
 class StartInstanceRequestUser(TeaModel):
     def __init__(self, user_id=None, user_name=None):
         self.user_id = user_id  # type: str
         self.user_name = user_name  # type: str
 
     def validate(self):
         pass
@@ -579,79 +650,92 @@
             self.user_id = m.get('UserId')
         if m.get('UserName') is not None:
             self.user_name = m.get('UserName')
         return self
 
 
 class StartInstanceRequest(TeaModel):
-    def __init__(self, app=None, tenant_id=None, user=None):
+    def __init__(self, app=None, channel=None, tenant_id=None, user=None):
         self.app = app  # type: StartInstanceRequestApp
+        self.channel = channel  # type: StartInstanceRequestChannel
         self.tenant_id = tenant_id  # type: long
         self.user = user  # type: StartInstanceRequestUser
 
     def validate(self):
         if self.app:
             self.app.validate()
+        if self.channel:
+            self.channel.validate()
         if self.user:
             self.user.validate()
 
     def to_map(self):
         _map = super(StartInstanceRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.app is not None:
             result['App'] = self.app.to_map()
+        if self.channel is not None:
+            result['Channel'] = self.channel.to_map()
         if self.tenant_id is not None:
             result['TenantId'] = self.tenant_id
         if self.user is not None:
             result['User'] = self.user.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('App') is not None:
             temp_model = StartInstanceRequestApp()
             self.app = temp_model.from_map(m['App'])
+        if m.get('Channel') is not None:
+            temp_model = StartInstanceRequestChannel()
+            self.channel = temp_model.from_map(m['Channel'])
         if m.get('TenantId') is not None:
             self.tenant_id = m.get('TenantId')
         if m.get('User') is not None:
             temp_model = StartInstanceRequestUser()
             self.user = temp_model.from_map(m['User'])
         return self
 
 
 class StartInstanceShrinkRequest(TeaModel):
-    def __init__(self, app_shrink=None, tenant_id=None, user_shrink=None):
+    def __init__(self, app_shrink=None, channel_shrink=None, tenant_id=None, user_shrink=None):
         self.app_shrink = app_shrink  # type: str
+        self.channel_shrink = channel_shrink  # type: str
         self.tenant_id = tenant_id  # type: long
         self.user_shrink = user_shrink  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(StartInstanceShrinkRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.app_shrink is not None:
             result['App'] = self.app_shrink
+        if self.channel_shrink is not None:
+            result['Channel'] = self.channel_shrink
         if self.tenant_id is not None:
             result['TenantId'] = self.tenant_id
         if self.user_shrink is not None:
             result['User'] = self.user_shrink
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('App') is not None:
             self.app_shrink = m.get('App')
+        if m.get('Channel') is not None:
+            self.channel_shrink = m.get('Channel')
         if m.get('TenantId') is not None:
             self.tenant_id = m.get('TenantId')
         if m.get('User') is not None:
             self.user_shrink = m.get('User')
         return self
```

### Comparing `alibabacloud_avatar20220130_py2-1.0.2/alibabacloud_avatar20220130_py2.egg-info/PKG-INFO` & `alibabacloud_avatar20220130_py2-1.0.3/alibabacloud_avatar20220130_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-avatar20220130-py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud avatar (20220130) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_avatar20220130_py2-1.0.2/setup.py` & `alibabacloud_avatar20220130_py2-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_avatar20220130_py2.
 
-Created on 27/07/2022
+Created on 28/07/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_avatar20220130"
 NAME = "alibabacloud_avatar20220130_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud avatar (20220130) SDK Library for Python2"
```

