# Comparing `tmp/alibabacloud_avatar20220130-1.0.8.tar.gz` & `tmp/alibabacloud_avatar20220130-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_avatar20220130-1.0.8.tar", last modified: Fri Nov  4 03:15:25 2022, max compression
+gzip compressed data, was "dist/alibabacloud_avatar20220130-1.0.9.tar", last modified: Mon Nov 28 06:56:37 2022, max compression
```

## Comparing `alibabacloud_avatar20220130-1.0.8.tar` & `alibabacloud_avatar20220130-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-04 03:15:25.000000 alibabacloud_avatar20220130-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      446 2022-11-04 03:15:24.000000 alibabacloud_avatar20220130-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-11-04 03:15:24.000000 alibabacloud_avatar20220130-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-11-04 03:15:24.000000 alibabacloud_avatar20220130-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2346 2022-11-04 03:15:25.000000 alibabacloud_avatar20220130-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1031 2022-11-04 03:15:24.000000 alibabacloud_avatar20220130-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2022-11-04 03:15:24.000000 alibabacloud_avatar20220130-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-04 03:15:25.000000 alibabacloud_avatar20220130-1.0.8/alibabacloud_avatar20220130/
--rw-r--r--   0 root         (0) root         (0)       21 2022-11-04 03:15:24.000000 alibabacloud_avatar20220130-1.0.8/alibabacloud_avatar20220130/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43824 2022-11-04 03:15:24.000000 alibabacloud_avatar20220130-1.0.8/alibabacloud_avatar20220130/client.py
--rw-r--r--   0 root         (0) root         (0)    92353 2022-11-04 03:15:24.000000 alibabacloud_avatar20220130-1.0.8/alibabacloud_avatar20220130/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-04 03:15:25.000000 alibabacloud_avatar20220130-1.0.8/alibabacloud_avatar20220130.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2346 2022-11-04 03:15:25.000000 alibabacloud_avatar20220130-1.0.8/alibabacloud_avatar20220130.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      444 2022-11-04 03:15:25.000000 alibabacloud_avatar20220130-1.0.8/alibabacloud_avatar20220130.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-04 03:15:25.000000 alibabacloud_avatar20220130-1.0.8/alibabacloud_avatar20220130.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-11-04 03:15:25.000000 alibabacloud_avatar20220130-1.0.8/alibabacloud_avatar20220130.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2022-11-04 03:15:25.000000 alibabacloud_avatar20220130-1.0.8/alibabacloud_avatar20220130.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-11-04 03:15:25.000000 alibabacloud_avatar20220130-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2625 2022-11-04 03:15:24.000000 alibabacloud_avatar20220130-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      517 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2346 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1031 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44582 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130/client.py
+-rw-r--r--   0 root         (0) root         (0)    96120 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2346 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      444 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2625 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/setup.py
```

### Comparing `alibabacloud_avatar20220130-1.0.8/LICENSE` & `alibabacloud_avatar20220130-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_avatar20220130-1.0.8/PKG-INFO` & `alibabacloud_avatar20220130-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_avatar20220130
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud avatar (20220130) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_avatar20220130-1.0.8/README-CN.md` & `alibabacloud_avatar20220130-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_avatar20220130-1.0.8/README.md` & `alibabacloud_avatar20220130-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_avatar20220130-1.0.8/alibabacloud_avatar20220130/client.py` & `alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         tmp_req: avatar_20220130_models.CancelVideoTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> avatar_20220130_models.CancelVideoTaskResponse:
         UtilClient.validate_model(tmp_req)
         request = avatar_20220130_models.CancelVideoTaskShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.app):
-            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.app), 'App', 'json')
+            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.app, 'App', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_shrink):
             query['App'] = request.app_shrink
         if not UtilClient.is_unset(request.task_uuid):
             query['TaskUuid'] = request.task_uuid
         if not UtilClient.is_unset(request.tenant_id):
             query['TenantId'] = request.tenant_id
@@ -82,15 +82,15 @@
         tmp_req: avatar_20220130_models.CancelVideoTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> avatar_20220130_models.CancelVideoTaskResponse:
         UtilClient.validate_model(tmp_req)
         request = avatar_20220130_models.CancelVideoTaskShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.app):
-            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.app), 'App', 'json')
+            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.app, 'App', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_shrink):
             query['App'] = request.app_shrink
         if not UtilClient.is_unset(request.task_uuid):
             query['TaskUuid'] = request.task_uuid
         if not UtilClient.is_unset(request.tenant_id):
             query['TenantId'] = request.tenant_id
@@ -134,15 +134,15 @@
     ) -> avatar_20220130_models.DuplexDecisionResponse:
         UtilClient.validate_model(tmp_req)
         request = avatar_20220130_models.DuplexDecisionShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.custom_keywords):
             request.custom_keywords_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.custom_keywords, 'CustomKeywords', 'json')
         if not UtilClient.is_unset(tmp_req.dialog_context):
-            request.dialog_context_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.dialog_context), 'DialogContext', 'json')
+            request.dialog_context_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.dialog_context, 'DialogContext', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.biz_request_id):
             query['BizRequestId'] = request.biz_request_id
         if not UtilClient.is_unset(request.call_time):
             query['CallTime'] = request.call_time
@@ -186,15 +186,15 @@
     ) -> avatar_20220130_models.DuplexDecisionResponse:
         UtilClient.validate_model(tmp_req)
         request = avatar_20220130_models.DuplexDecisionShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.custom_keywords):
             request.custom_keywords_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.custom_keywords, 'CustomKeywords', 'json')
         if not UtilClient.is_unset(tmp_req.dialog_context):
-            request.dialog_context_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.dialog_context), 'DialogContext', 'json')
+            request.dialog_context_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.dialog_context, 'DialogContext', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.biz_request_id):
             query['BizRequestId'] = request.biz_request_id
         if not UtilClient.is_unset(request.call_time):
             query['CallTime'] = request.call_time
@@ -250,15 +250,15 @@
         tmp_req: avatar_20220130_models.GetVideoTaskInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> avatar_20220130_models.GetVideoTaskInfoResponse:
         UtilClient.validate_model(tmp_req)
         request = avatar_20220130_models.GetVideoTaskInfoShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.app):
-            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.app), 'App', 'json')
+            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.app, 'App', 'json')
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetVideoTaskInfo',
             version='2022-01-30',
@@ -280,15 +280,15 @@
         tmp_req: avatar_20220130_models.GetVideoTaskInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> avatar_20220130_models.GetVideoTaskInfoResponse:
         UtilClient.validate_model(tmp_req)
         request = avatar_20220130_models.GetVideoTaskInfoShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.app):
-            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.app), 'App', 'json')
+            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.app, 'App', 'json')
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetVideoTaskInfo',
             version='2022-01-30',
@@ -324,15 +324,15 @@
         tmp_req: avatar_20220130_models.QueryRunningInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> avatar_20220130_models.QueryRunningInstanceResponse:
         UtilClient.validate_model(tmp_req)
         request = avatar_20220130_models.QueryRunningInstanceShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.app):
-            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.app), 'App', 'json')
+            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.app, 'App', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_shrink):
             query['App'] = request.app_shrink
         if not UtilClient.is_unset(request.session_id):
             query['SessionId'] = request.session_id
         if not UtilClient.is_unset(request.tenant_id):
             query['TenantId'] = request.tenant_id
@@ -360,15 +360,15 @@
         tmp_req: avatar_20220130_models.QueryRunningInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> avatar_20220130_models.QueryRunningInstanceResponse:
         UtilClient.validate_model(tmp_req)
         request = avatar_20220130_models.QueryRunningInstanceShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.app):
-            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.app), 'App', 'json')
+            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.app, 'App', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_shrink):
             query['App'] = request.app_shrink
         if not UtilClient.is_unset(request.session_id):
             query['SessionId'] = request.session_id
         if not UtilClient.is_unset(request.tenant_id):
             query['TenantId'] = request.tenant_id
@@ -410,17 +410,17 @@
         tmp_req: avatar_20220130_models.SendMessageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> avatar_20220130_models.SendMessageResponse:
         UtilClient.validate_model(tmp_req)
         request = avatar_20220130_models.SendMessageShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.text_request):
-            request.text_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.text_request), 'TextRequest', 'json')
+            request.text_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.text_request, 'TextRequest', 'json')
         if not UtilClient.is_unset(tmp_req.vamlrequest):
-            request.vamlrequest_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.vamlrequest), 'VAMLRequest', 'json')
+            request.vamlrequest_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.vamlrequest, 'VAMLRequest', 'json')
         query = {}
         if not UtilClient.is_unset(request.session_id):
             query['SessionId'] = request.session_id
         if not UtilClient.is_unset(request.tenant_id):
             query['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.text_request_shrink):
             query['TextRequest'] = request.text_request_shrink
@@ -450,17 +450,17 @@
         tmp_req: avatar_20220130_models.SendMessageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> avatar_20220130_models.SendMessageResponse:
         UtilClient.validate_model(tmp_req)
         request = avatar_20220130_models.SendMessageShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.text_request):
-            request.text_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.text_request), 'TextRequest', 'json')
+            request.text_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.text_request, 'TextRequest', 'json')
         if not UtilClient.is_unset(tmp_req.vamlrequest):
-            request.vamlrequest_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.vamlrequest), 'VAMLRequest', 'json')
+            request.vamlrequest_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.vamlrequest, 'VAMLRequest', 'json')
         query = {}
         if not UtilClient.is_unset(request.session_id):
             query['SessionId'] = request.session_id
         if not UtilClient.is_unset(request.tenant_id):
             query['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.text_request_shrink):
             query['TextRequest'] = request.text_request_shrink
@@ -504,21 +504,21 @@
         tmp_req: avatar_20220130_models.StartInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> avatar_20220130_models.StartInstanceResponse:
         UtilClient.validate_model(tmp_req)
         request = avatar_20220130_models.StartInstanceShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.app):
-            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.app), 'App', 'json')
+            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.app, 'App', 'json')
         if not UtilClient.is_unset(tmp_req.channel):
-            request.channel_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.channel), 'Channel', 'json')
+            request.channel_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.channel, 'Channel', 'json')
         if not UtilClient.is_unset(tmp_req.command_request):
-            request.command_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.command_request), 'CommandRequest', 'json')
+            request.command_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.command_request, 'CommandRequest', 'json')
         if not UtilClient.is_unset(tmp_req.user):
-            request.user_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user), 'User', 'json')
+            request.user_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user, 'User', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_shrink):
             query['App'] = request.app_shrink
         if not UtilClient.is_unset(request.channel_shrink):
             query['Channel'] = request.channel_shrink
         if not UtilClient.is_unset(request.command_request_shrink):
             query['CommandRequest'] = request.command_request_shrink
@@ -550,21 +550,21 @@
         tmp_req: avatar_20220130_models.StartInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> avatar_20220130_models.StartInstanceResponse:
         UtilClient.validate_model(tmp_req)
         request = avatar_20220130_models.StartInstanceShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.app):
-            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.app), 'App', 'json')
+            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.app, 'App', 'json')
         if not UtilClient.is_unset(tmp_req.channel):
-            request.channel_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.channel), 'Channel', 'json')
+            request.channel_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.channel, 'Channel', 'json')
         if not UtilClient.is_unset(tmp_req.command_request):
-            request.command_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.command_request), 'CommandRequest', 'json')
+            request.command_request_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.command_request, 'CommandRequest', 'json')
         if not UtilClient.is_unset(tmp_req.user):
-            request.user_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.user), 'User', 'json')
+            request.user_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user, 'User', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_shrink):
             query['App'] = request.app_shrink
         if not UtilClient.is_unset(request.channel_shrink):
             query['Channel'] = request.channel_shrink
         if not UtilClient.is_unset(request.command_request_shrink):
             query['CommandRequest'] = request.command_request_shrink
@@ -684,20 +684,28 @@
         tmp_req: avatar_20220130_models.SubmitTextTo2DAvatarVideoTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> avatar_20220130_models.SubmitTextTo2DAvatarVideoTaskResponse:
         UtilClient.validate_model(tmp_req)
         request = avatar_20220130_models.SubmitTextTo2DAvatarVideoTaskShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.app):
-            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.app), 'App', 'json')
+            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.app, 'App', 'json')
+        if not UtilClient.is_unset(tmp_req.audio_info):
+            request.audio_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.audio_info, 'AudioInfo', 'json')
+        if not UtilClient.is_unset(tmp_req.avatar_info):
+            request.avatar_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.avatar_info, 'AvatarInfo', 'json')
         if not UtilClient.is_unset(tmp_req.video_info):
-            request.video_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.video_info), 'VideoInfo', 'json')
+            request.video_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.video_info, 'VideoInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_shrink):
             query['App'] = request.app_shrink
+        if not UtilClient.is_unset(request.audio_info_shrink):
+            query['AudioInfo'] = request.audio_info_shrink
+        if not UtilClient.is_unset(request.avatar_info_shrink):
+            query['AvatarInfo'] = request.avatar_info_shrink
         if not UtilClient.is_unset(request.tenant_id):
             query['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.text):
             query['Text'] = request.text
         if not UtilClient.is_unset(request.title):
             query['Title'] = request.title
         if not UtilClient.is_unset(request.video_info_shrink):
@@ -726,20 +734,28 @@
         tmp_req: avatar_20220130_models.SubmitTextTo2DAvatarVideoTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> avatar_20220130_models.SubmitTextTo2DAvatarVideoTaskResponse:
         UtilClient.validate_model(tmp_req)
         request = avatar_20220130_models.SubmitTextTo2DAvatarVideoTaskShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.app):
-            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.app), 'App', 'json')
+            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.app, 'App', 'json')
+        if not UtilClient.is_unset(tmp_req.audio_info):
+            request.audio_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.audio_info, 'AudioInfo', 'json')
+        if not UtilClient.is_unset(tmp_req.avatar_info):
+            request.avatar_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.avatar_info, 'AvatarInfo', 'json')
         if not UtilClient.is_unset(tmp_req.video_info):
-            request.video_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.video_info), 'VideoInfo', 'json')
+            request.video_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.video_info, 'VideoInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_shrink):
             query['App'] = request.app_shrink
+        if not UtilClient.is_unset(request.audio_info_shrink):
+            query['AudioInfo'] = request.audio_info_shrink
+        if not UtilClient.is_unset(request.avatar_info_shrink):
+            query['AvatarInfo'] = request.avatar_info_shrink
         if not UtilClient.is_unset(request.tenant_id):
             query['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.text):
             query['Text'] = request.text
         if not UtilClient.is_unset(request.title):
             query['Title'] = request.title
         if not UtilClient.is_unset(request.video_info_shrink):
@@ -782,17 +798,17 @@
         tmp_req: avatar_20220130_models.SubmitTextTo3DAvatarVideoTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> avatar_20220130_models.SubmitTextTo3DAvatarVideoTaskResponse:
         UtilClient.validate_model(tmp_req)
         request = avatar_20220130_models.SubmitTextTo3DAvatarVideoTaskShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.app):
-            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.app), 'App', 'json')
+            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.app, 'App', 'json')
         if not UtilClient.is_unset(tmp_req.video_info):
-            request.video_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.video_info), 'VideoInfo', 'json')
+            request.video_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.video_info, 'VideoInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_shrink):
             query['App'] = request.app_shrink
         if not UtilClient.is_unset(request.tenant_id):
             query['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.text):
             query['Text'] = request.text
@@ -824,17 +840,17 @@
         tmp_req: avatar_20220130_models.SubmitTextTo3DAvatarVideoTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> avatar_20220130_models.SubmitTextTo3DAvatarVideoTaskResponse:
         UtilClient.validate_model(tmp_req)
         request = avatar_20220130_models.SubmitTextTo3DAvatarVideoTaskShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.app):
-            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.app), 'App', 'json')
+            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.app, 'App', 'json')
         if not UtilClient.is_unset(tmp_req.video_info):
-            request.video_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.video_info), 'VideoInfo', 'json')
+            request.video_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.video_info, 'VideoInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_shrink):
             query['App'] = request.app_shrink
         if not UtilClient.is_unset(request.tenant_id):
             query['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.text):
             query['Text'] = request.text
@@ -880,17 +896,17 @@
         tmp_req: avatar_20220130_models.SubmitTextToSignVideoTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> avatar_20220130_models.SubmitTextToSignVideoTaskResponse:
         UtilClient.validate_model(tmp_req)
         request = avatar_20220130_models.SubmitTextToSignVideoTaskShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.app):
-            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.app), 'App', 'json')
+            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.app, 'App', 'json')
         if not UtilClient.is_unset(tmp_req.video_info):
-            request.video_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.video_info), 'VideoInfo', 'json')
+            request.video_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.video_info, 'VideoInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_shrink):
             query['App'] = request.app_shrink
         if not UtilClient.is_unset(request.tenant_id):
             query['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.text):
             query['Text'] = request.text
@@ -922,17 +938,17 @@
         tmp_req: avatar_20220130_models.SubmitTextToSignVideoTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> avatar_20220130_models.SubmitTextToSignVideoTaskResponse:
         UtilClient.validate_model(tmp_req)
         request = avatar_20220130_models.SubmitTextToSignVideoTaskShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.app):
-            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.app), 'App', 'json')
+            request.app_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.app, 'App', 'json')
         if not UtilClient.is_unset(tmp_req.video_info):
-            request.video_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.video_info), 'VideoInfo', 'json')
+            request.video_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.video_info, 'VideoInfo', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_shrink):
             query['App'] = request.app_shrink
         if not UtilClient.is_unset(request.tenant_id):
             query['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.text):
             query['Text'] = request.text
```

### Comparing `alibabacloud_avatar20220130-1.0.8/alibabacloud_avatar20220130/models.py` & `alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2202,76 +2202,166 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AppId') is not None:
             self.app_id = m.get('AppId')
         return self
 
 
+class SubmitTextTo2DAvatarVideoTaskRequestAudioInfo(TeaModel):
+    def __init__(
+        self,
+        pitch_rate: int = None,
+        speech_rate: int = None,
+        voice: str = None,
+        volume: int = None,
+    ):
+        self.pitch_rate = pitch_rate
+        self.speech_rate = speech_rate
+        self.voice = voice
+        self.volume = volume
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.pitch_rate is not None:
+            result['PitchRate'] = self.pitch_rate
+        if self.speech_rate is not None:
+            result['SpeechRate'] = self.speech_rate
+        if self.voice is not None:
+            result['Voice'] = self.voice
+        if self.volume is not None:
+            result['Volume'] = self.volume
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('PitchRate') is not None:
+            self.pitch_rate = m.get('PitchRate')
+        if m.get('SpeechRate') is not None:
+            self.speech_rate = m.get('SpeechRate')
+        if m.get('Voice') is not None:
+            self.voice = m.get('Voice')
+        if m.get('Volume') is not None:
+            self.volume = m.get('Volume')
+        return self
+
+
+class SubmitTextTo2DAvatarVideoTaskRequestAvatarInfo(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+    ):
+        self.code = code
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        return self
+
+
 class SubmitTextTo2DAvatarVideoTaskRequestVideoInfo(TeaModel):
     def __init__(
         self,
+        background_image_url: str = None,
         is_alpha: bool = None,
         is_subtitles: bool = None,
     ):
+        self.background_image_url = background_image_url
         self.is_alpha = is_alpha
         self.is_subtitles = is_subtitles
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.background_image_url is not None:
+            result['BackgroundImageUrl'] = self.background_image_url
         if self.is_alpha is not None:
             result['IsAlpha'] = self.is_alpha
         if self.is_subtitles is not None:
             result['IsSubtitles'] = self.is_subtitles
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('BackgroundImageUrl') is not None:
+            self.background_image_url = m.get('BackgroundImageUrl')
         if m.get('IsAlpha') is not None:
             self.is_alpha = m.get('IsAlpha')
         if m.get('IsSubtitles') is not None:
             self.is_subtitles = m.get('IsSubtitles')
         return self
 
 
 class SubmitTextTo2DAvatarVideoTaskRequest(TeaModel):
     def __init__(
         self,
         app: SubmitTextTo2DAvatarVideoTaskRequestApp = None,
+        audio_info: SubmitTextTo2DAvatarVideoTaskRequestAudioInfo = None,
+        avatar_info: SubmitTextTo2DAvatarVideoTaskRequestAvatarInfo = None,
         tenant_id: int = None,
         text: str = None,
         title: str = None,
         video_info: SubmitTextTo2DAvatarVideoTaskRequestVideoInfo = None,
     ):
         self.app = app
+        self.audio_info = audio_info
+        self.avatar_info = avatar_info
         self.tenant_id = tenant_id
         self.text = text
         self.title = title
         self.video_info = video_info
 
     def validate(self):
         if self.app:
             self.app.validate()
+        if self.audio_info:
+            self.audio_info.validate()
+        if self.avatar_info:
+            self.avatar_info.validate()
         if self.video_info:
             self.video_info.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.app is not None:
             result['App'] = self.app.to_map()
+        if self.audio_info is not None:
+            result['AudioInfo'] = self.audio_info.to_map()
+        if self.avatar_info is not None:
+            result['AvatarInfo'] = self.avatar_info.to_map()
         if self.tenant_id is not None:
             result['TenantId'] = self.tenant_id
         if self.text is not None:
             result['Text'] = self.text
         if self.title is not None:
             result['Title'] = self.title
         if self.video_info is not None:
@@ -2279,14 +2369,20 @@
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('App') is not None:
             temp_model = SubmitTextTo2DAvatarVideoTaskRequestApp()
             self.app = temp_model.from_map(m['App'])
+        if m.get('AudioInfo') is not None:
+            temp_model = SubmitTextTo2DAvatarVideoTaskRequestAudioInfo()
+            self.audio_info = temp_model.from_map(m['AudioInfo'])
+        if m.get('AvatarInfo') is not None:
+            temp_model = SubmitTextTo2DAvatarVideoTaskRequestAvatarInfo()
+            self.avatar_info = temp_model.from_map(m['AvatarInfo'])
         if m.get('TenantId') is not None:
             self.tenant_id = m.get('TenantId')
         if m.get('Text') is not None:
             self.text = m.get('Text')
         if m.get('Title') is not None:
             self.title = m.get('Title')
         if m.get('VideoInfo') is not None:
@@ -2295,20 +2391,24 @@
         return self
 
 
 class SubmitTextTo2DAvatarVideoTaskShrinkRequest(TeaModel):
     def __init__(
         self,
         app_shrink: str = None,
+        audio_info_shrink: str = None,
+        avatar_info_shrink: str = None,
         tenant_id: int = None,
         text: str = None,
         title: str = None,
         video_info_shrink: str = None,
     ):
         self.app_shrink = app_shrink
+        self.audio_info_shrink = audio_info_shrink
+        self.avatar_info_shrink = avatar_info_shrink
         self.tenant_id = tenant_id
         self.text = text
         self.title = title
         self.video_info_shrink = video_info_shrink
 
     def validate(self):
         pass
@@ -2317,28 +2417,36 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.app_shrink is not None:
             result['App'] = self.app_shrink
+        if self.audio_info_shrink is not None:
+            result['AudioInfo'] = self.audio_info_shrink
+        if self.avatar_info_shrink is not None:
+            result['AvatarInfo'] = self.avatar_info_shrink
         if self.tenant_id is not None:
             result['TenantId'] = self.tenant_id
         if self.text is not None:
             result['Text'] = self.text
         if self.title is not None:
             result['Title'] = self.title
         if self.video_info_shrink is not None:
             result['VideoInfo'] = self.video_info_shrink
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('App') is not None:
             self.app_shrink = m.get('App')
+        if m.get('AudioInfo') is not None:
+            self.audio_info_shrink = m.get('AudioInfo')
+        if m.get('AvatarInfo') is not None:
+            self.avatar_info_shrink = m.get('AvatarInfo')
         if m.get('TenantId') is not None:
             self.tenant_id = m.get('TenantId')
         if m.get('Text') is not None:
             self.text = m.get('Text')
         if m.get('Title') is not None:
             self.title = m.get('Title')
         if m.get('VideoInfo') is not None:
```

### Comparing `alibabacloud_avatar20220130-1.0.8/alibabacloud_avatar20220130.egg-info/PKG-INFO` & `alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-avatar20220130
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud avatar (20220130) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_avatar20220130-1.0.8/setup.py` & `alibabacloud_avatar20220130-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_avatar20220130.
 
-Created on 04/11/2022
+Created on 28/11/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_avatar20220130"
 NAME = "alibabacloud_avatar20220130" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud avatar (20220130) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.5, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.0, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

