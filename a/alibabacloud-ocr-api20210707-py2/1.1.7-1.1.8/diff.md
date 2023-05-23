# Comparing `tmp/alibabacloud_ocr-api20210707_py2-1.1.7.tar.gz` & `tmp/alibabacloud_ocr-api20210707_py2-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ocr-api20210707_py2-1.1.7.tar", last modified: Mon Jun 20 05:54:15 2022, max compression
+gzip compressed data, was "dist/alibabacloud_ocr-api20210707_py2-1.1.8.tar", last modified: Tue Aug 23 05:31:06 2022, max compression
```

## Comparing `alibabacloud_ocr-api20210707_py2-1.1.7.tar` & `alibabacloud_ocr-api20210707_py2-1.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 05:54:15.000000 alibabacloud_ocr-api20210707_py2-1.1.7/
--rw-r--r--   0 root         (0) root         (0)      187 2022-06-20 05:54:14.000000 alibabacloud_ocr-api20210707_py2-1.1.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-06-20 05:54:14.000000 alibabacloud_ocr-api20210707_py2-1.1.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-06-20 05:54:14.000000 alibabacloud_ocr-api20210707_py2-1.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2496 2022-06-20 05:54:15.000000 alibabacloud_ocr-api20210707_py2-1.1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1045 2022-06-20 05:54:14.000000 alibabacloud_ocr-api20210707_py2-1.1.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2022-06-20 05:54:14.000000 alibabacloud_ocr-api20210707_py2-1.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 05:54:15.000000 alibabacloud_ocr-api20210707_py2-1.1.7/alibabacloud_ocr_api20210707/
--rw-r--r--   0 root         (0) root         (0)       21 2022-06-20 05:54:14.000000 alibabacloud_ocr-api20210707_py2-1.1.7/alibabacloud_ocr_api20210707/__init__.py
--rw-r--r--   0 root         (0) root         (0)    85266 2022-06-20 05:54:14.000000 alibabacloud_ocr-api20210707_py2-1.1.7/alibabacloud_ocr_api20210707/client.py
--rw-r--r--   0 root         (0) root         (0)   281183 2022-06-20 05:54:14.000000 alibabacloud_ocr-api20210707_py2-1.1.7/alibabacloud_ocr_api20210707/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 05:54:15.000000 alibabacloud_ocr-api20210707_py2-1.1.7/alibabacloud_ocr_api20210707_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2496 2022-06-20 05:54:15.000000 alibabacloud_ocr-api20210707_py2-1.1.7/alibabacloud_ocr_api20210707_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2022-06-20 05:54:15.000000 alibabacloud_ocr-api20210707_py2-1.1.7/alibabacloud_ocr_api20210707_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-20 05:54:15.000000 alibabacloud_ocr-api20210707_py2-1.1.7/alibabacloud_ocr_api20210707_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-06-20 05:54:15.000000 alibabacloud_ocr-api20210707_py2-1.1.7/alibabacloud_ocr_api20210707_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2022-06-20 05:54:15.000000 alibabacloud_ocr-api20210707_py2-1.1.7/alibabacloud_ocr_api20210707_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-06-20 05:54:15.000000 alibabacloud_ocr-api20210707_py2-1.1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2925 2022-06-20 05:54:14.000000 alibabacloud_ocr-api20210707_py2-1.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 05:31:06.000000 alibabacloud_ocr-api20210707_py2-1.1.8/
+-rw-r--r--   0 root         (0) root         (0)      226 2022-08-23 05:31:06.000000 alibabacloud_ocr-api20210707_py2-1.1.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2022-08-23 05:31:06.000000 alibabacloud_ocr-api20210707_py2-1.1.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2022-08-23 05:31:06.000000 alibabacloud_ocr-api20210707_py2-1.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2496 2022-08-23 05:31:06.000000 alibabacloud_ocr-api20210707_py2-1.1.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1045 2022-08-23 05:31:06.000000 alibabacloud_ocr-api20210707_py2-1.1.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2022-08-23 05:31:06.000000 alibabacloud_ocr-api20210707_py2-1.1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 05:31:06.000000 alibabacloud_ocr-api20210707_py2-1.1.8/alibabacloud_ocr_api20210707/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-08-23 05:31:06.000000 alibabacloud_ocr-api20210707_py2-1.1.8/alibabacloud_ocr_api20210707/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81987 2022-08-23 05:31:06.000000 alibabacloud_ocr-api20210707_py2-1.1.8/alibabacloud_ocr_api20210707/client.py
+-rw-r--r--   0 root         (0) root         (0)   255754 2022-08-23 05:31:06.000000 alibabacloud_ocr-api20210707_py2-1.1.8/alibabacloud_ocr_api20210707/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 05:31:06.000000 alibabacloud_ocr-api20210707_py2-1.1.8/alibabacloud_ocr_api20210707_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2496 2022-08-23 05:31:06.000000 alibabacloud_ocr-api20210707_py2-1.1.8/alibabacloud_ocr_api20210707_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2022-08-23 05:31:06.000000 alibabacloud_ocr-api20210707_py2-1.1.8/alibabacloud_ocr_api20210707_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-23 05:31:06.000000 alibabacloud_ocr-api20210707_py2-1.1.8/alibabacloud_ocr_api20210707_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2022-08-23 05:31:06.000000 alibabacloud_ocr-api20210707_py2-1.1.8/alibabacloud_ocr_api20210707_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2022-08-23 05:31:06.000000 alibabacloud_ocr-api20210707_py2-1.1.8/alibabacloud_ocr_api20210707_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-08-23 05:31:06.000000 alibabacloud_ocr-api20210707_py2-1.1.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2925 2022-08-23 05:31:06.000000 alibabacloud_ocr-api20210707_py2-1.1.8/setup.py
```

### Comparing `alibabacloud_ocr-api20210707_py2-1.1.7/LICENSE` & `alibabacloud_ocr-api20210707_py2-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ocr-api20210707_py2-1.1.7/PKG-INFO` & `alibabacloud_ocr-api20210707_py2-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ocr-api20210707_py2
-Version: 1.1.7
+Version: 1.1.8
 Summary: Alibaba Cloud ocr-api (20210707) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ocr-api20210707_py2-1.1.7/README-CN.md` & `alibabacloud_ocr-api20210707_py2-1.1.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ocr-api20210707_py2-1.1.7/README.md` & `alibabacloud_ocr-api20210707_py2-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ocr-api20210707_py2-1.1.7/alibabacloud_ocr_api20210707/client.py` & `alibabacloud_ocr-api20210707_py2-1.1.8/alibabacloud_ocr_api20210707/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,56 +222,14 @@
             self.call_api(params, req, runtime)
         )
 
     def recognize_basic(self, request):
         runtime = util_models.RuntimeOptions()
         return self.recognize_basic_with_options(request, runtime)
 
-    def recognize_batch_recognize_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.image_name):
-            query['ImageName'] = request.image_name
-        if not UtilClient.is_unset(request.image_op):
-            query['ImageOp'] = request.image_op
-        if not UtilClient.is_unset(request.image_oss_key):
-            query['ImageOssKey'] = request.image_oss_key
-        if not UtilClient.is_unset(request.need_rotate):
-            query['NeedRotate'] = request.need_rotate
-        if not UtilClient.is_unset(request.need_sort_page):
-            query['NeedSortPage'] = request.need_sort_page
-        if not UtilClient.is_unset(request.output_char_info):
-            query['OutputCharInfo'] = request.output_char_info
-        if not UtilClient.is_unset(request.output_table):
-            query['OutputTable'] = request.output_table
-        if not UtilClient.is_unset(request.url):
-            query['Url'] = request.url
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='RecognizeBatchRecognize',
-            version='2021-07-07',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_api_20210707_models.RecognizeBatchRecognizeResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def recognize_batch_recognize(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.recognize_batch_recognize_with_options(request, runtime)
-
     def recognize_birth_certification_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.url):
             query['Url'] = request.url
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
@@ -598,41 +556,61 @@
             self.call_api(params, req, runtime)
         )
 
     def recognize_ctwo_medical_device_manage_license(self, request):
         runtime = util_models.RuntimeOptions()
         return self.recognize_ctwo_medical_device_manage_license_with_options(request, runtime)
 
-    def recognize_delete_excel_record_with_options(self, request, runtime):
+    def recognize_document_structure_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.id):
-            query['Id'] = request.id
+        if not UtilClient.is_unset(request.need_rotate):
+            query['NeedRotate'] = request.need_rotate
+        if not UtilClient.is_unset(request.need_sort_page):
+            query['NeedSortPage'] = request.need_sort_page
+        if not UtilClient.is_unset(request.no_stamp):
+            query['NoStamp'] = request.no_stamp
+        if not UtilClient.is_unset(request.output_char_info):
+            query['OutputCharInfo'] = request.output_char_info
+        if not UtilClient.is_unset(request.output_table):
+            query['OutputTable'] = request.output_table
+        if not UtilClient.is_unset(request.page):
+            query['Page'] = request.page
+        if not UtilClient.is_unset(request.paragraph):
+            query['Paragraph'] = request.paragraph
+        if not UtilClient.is_unset(request.row):
+            query['Row'] = request.row
+        if not UtilClient.is_unset(request.url):
+            query['Url'] = request.url
+        if not UtilClient.is_unset(request.use_new_style_output):
+            query['UseNewStyleOutput'] = request.use_new_style_output
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
+            query=OpenApiUtilClient.query(query),
+            body=request.body,
+            stream=request.body
         )
         params = open_api_models.Params(
-            action='RecognizeDeleteExcelRecord',
+            action='RecognizeDocumentStructure',
             version='2021-07-07',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
             req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
-            ocr_api_20210707_models.RecognizeDeleteExcelRecordResponse(),
+            ocr_api_20210707_models.RecognizeDocumentStructureResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def recognize_delete_excel_record(self, request):
+    def recognize_document_structure(self, request):
         runtime = util_models.RuntimeOptions()
-        return self.recognize_delete_excel_record_with_options(request, runtime)
+        return self.recognize_document_structure_with_options(request, runtime)
 
     def recognize_driving_license_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.url):
             query['Url'] = request.url
         req = open_api_models.OpenApiRequest(
@@ -918,80 +896,14 @@
             self.call_api(params, req, runtime)
         )
 
     def recognize_estate_certification(self, request):
         runtime = util_models.RuntimeOptions()
         return self.recognize_estate_certification_with_options(request, runtime)
 
-    def recognize_excel_export_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.file_name):
-            query['FileName'] = request.file_name
-        if not UtilClient.is_unset(request.image_op):
-            query['ImageOp'] = request.image_op
-        if not UtilClient.is_unset(request.ocr_image_count):
-            query['OcrImageCount'] = request.ocr_image_count
-        if not UtilClient.is_unset(request.ocr_result):
-            query['OcrResult'] = request.ocr_result
-        if not UtilClient.is_unset(request.ocr_type):
-            query['OcrType'] = request.ocr_type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='RecognizeExcelExport',
-            version='2021-07-07',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_api_20210707_models.RecognizeExcelExportResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def recognize_excel_export(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.recognize_excel_export_with_options(request, runtime)
-
-    def recognize_excel_record_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.curr_page):
-            query['CurrPage'] = request.curr_page
-        if not UtilClient.is_unset(request.page_size):
-            query['PageSize'] = request.page_size
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='RecognizeExcelRecord',
-            version='2021-07-07',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_api_20210707_models.RecognizeExcelRecordResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def recognize_excel_record(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.recognize_excel_record_with_options(request, runtime)
-
     def recognize_exit_entry_permit_to_hkwith_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.output_figure):
             query['OutputFigure'] = request.output_figure
         if not UtilClient.is_unset(request.url):
             query['Url'] = request.url
```

### Comparing `alibabacloud_ocr-api20210707_py2-1.1.7/alibabacloud_ocr_api20210707/models.py` & `alibabacloud_ocr-api20210707_py2-1.1.8/alibabacloud_ocr_api20210707/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,33 +2,23 @@
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 
 
 class RecognizeAdvancedRequest(TeaModel):
     def __init__(self, need_rotate=None, need_sort_page=None, no_stamp=None, output_char_info=None,
                  output_figure=None, output_table=None, paragraph=None, row=None, url=None, body=None):
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate  # type: bool
-        # 是否按顺序输出文字块。false表示从左往右，从上到下的顺序；true表示从上到下，从左往右的顺序
         self.need_sort_page = need_sort_page  # type: bool
-        # 是否需要去除印章功能，默认不需要。true：需要 false：不需要
         self.no_stamp = no_stamp  # type: bool
-        # 是否输出单字识别结果
         self.output_char_info = output_char_info  # type: bool
-        # 是否需要图案检测功能，默认不需要。true：需要 false：不需要
         self.output_figure = output_figure  # type: bool
-        # 是否输出表格识别结果，包含单元格信息
         self.output_table = output_table  # type: bool
-        # 是否需要分段功能，默认不需要。true：需要 false：不需要
         self.paragraph = paragraph  # type: bool
-        # 是否需要成行返回功能，默认不需要
         self.row = row  # type: bool
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeAdvancedRequest, self).to_map()
@@ -81,21 +71,17 @@
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
 
 
 class RecognizeAdvancedResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
         self.code = code  # type: str
-        # 返回数据
         self.data = data  # type: str
-        # 错误提示
         self.message = message  # type: str
-        # 请求唯一 ID
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeAdvancedResponseBody, self).to_map()
@@ -163,17 +149,15 @@
             temp_model = RecognizeAdvancedResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeAirItineraryRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeAirItineraryRequest, self).to_map()
@@ -272,17 +256,15 @@
             temp_model = RecognizeAirItineraryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeBankAcceptanceRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeBankAcceptanceRequest, self).to_map()
@@ -303,21 +285,17 @@
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
 
 
 class RecognizeBankAcceptanceResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
         self.code = code  # type: str
-        # 返回数据
         self.data = data  # type: str
-        # 错误提示
         self.message = message  # type: str
-        # 请求唯一 ID
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeBankAcceptanceResponseBody, self).to_map()
@@ -385,17 +363,15 @@
             temp_model = RecognizeBankAcceptanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeBankAccountLicenseRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeBankAccountLicenseRequest, self).to_map()
@@ -494,17 +470,15 @@
             temp_model = RecognizeBankAccountLicenseResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeBankCardRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeBankCardRequest, self).to_map()
@@ -603,17 +577,15 @@
             temp_model = RecognizeBankCardResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeBasicRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeBasicRequest, self).to_map()
@@ -710,169 +682,17 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RecognizeBasicResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class RecognizeBatchRecognizeRequest(TeaModel):
-    def __init__(self, image_name=None, image_op=None, image_oss_key=None, need_rotate=None, need_sort_page=None,
-                 output_char_info=None, output_table=None, url=None):
-        # 图片名称
-        self.image_name = image_name  # type: str
-        # 图片识别op类型
-        self.image_op = image_op  # type: str
-        # 图片存入oss中的key
-        self.image_oss_key = image_oss_key  # type: str
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
-        self.need_rotate = need_rotate  # type: bool
-        # 是否按顺序输出文字块。false表示从左往右，从上到下的顺序；true表示从上到下，从左往右的顺序
-        self.need_sort_page = need_sort_page  # type: bool
-        # 是否输出单字识别结果
-        self.output_char_info = output_char_info  # type: bool
-        # 是否输出表格识别结果，包含单元格信息
-        self.output_table = output_table  # type: bool
-        # 图片链接（长度不超 2048，不支持 base64）
-        self.url = url  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(RecognizeBatchRecognizeRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.image_name is not None:
-            result['ImageName'] = self.image_name
-        if self.image_op is not None:
-            result['ImageOp'] = self.image_op
-        if self.image_oss_key is not None:
-            result['ImageOssKey'] = self.image_oss_key
-        if self.need_rotate is not None:
-            result['NeedRotate'] = self.need_rotate
-        if self.need_sort_page is not None:
-            result['NeedSortPage'] = self.need_sort_page
-        if self.output_char_info is not None:
-            result['OutputCharInfo'] = self.output_char_info
-        if self.output_table is not None:
-            result['OutputTable'] = self.output_table
-        if self.url is not None:
-            result['Url'] = self.url
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('ImageName') is not None:
-            self.image_name = m.get('ImageName')
-        if m.get('ImageOp') is not None:
-            self.image_op = m.get('ImageOp')
-        if m.get('ImageOssKey') is not None:
-            self.image_oss_key = m.get('ImageOssKey')
-        if m.get('NeedRotate') is not None:
-            self.need_rotate = m.get('NeedRotate')
-        if m.get('NeedSortPage') is not None:
-            self.need_sort_page = m.get('NeedSortPage')
-        if m.get('OutputCharInfo') is not None:
-            self.output_char_info = m.get('OutputCharInfo')
-        if m.get('OutputTable') is not None:
-            self.output_table = m.get('OutputTable')
-        if m.get('Url') is not None:
-            self.url = m.get('Url')
-        return self
-
-
-class RecognizeBatchRecognizeResponseBody(TeaModel):
-    def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
-        self.code = code  # type: str
-        # 返回数据
-        self.data = data  # type: str
-        # 错误提示
-        self.message = message  # type: str
-        # 请求唯一 ID
-        self.request_id = request_id  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(RecognizeBatchRecognizeResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.code is not None:
-            result['Code'] = self.code
-        if self.data is not None:
-            result['Data'] = self.data
-        if self.message is not None:
-            result['Message'] = self.message
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Code') is not None:
-            self.code = m.get('Code')
-        if m.get('Data') is not None:
-            self.data = m.get('Data')
-        if m.get('Message') is not None:
-            self.message = m.get('Message')
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        return self
-
-
-class RecognizeBatchRecognizeResponse(TeaModel):
-    def __init__(self, headers=None, status_code=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.status_code = status_code  # type: int
-        self.body = body  # type: RecognizeBatchRecognizeResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(RecognizeBatchRecognizeResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = RecognizeBatchRecognizeResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class RecognizeBirthCertificationRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeBirthCertificationRequest, self).to_map()
@@ -971,17 +791,15 @@
             temp_model = RecognizeBirthCertificationResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeBusShipTicketRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeBusShipTicketRequest, self).to_map()
@@ -1002,21 +820,17 @@
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
 
 
 class RecognizeBusShipTicketResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
         self.code = code  # type: str
-        # 返回数据
         self.data = data  # type: str
-        # 错误提示
         self.message = message  # type: str
-        # 请求唯一 ID
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeBusShipTicketResponseBody, self).to_map()
@@ -1084,17 +898,15 @@
             temp_model = RecognizeBusShipTicketResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeBusinessLicenseRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeBusinessLicenseRequest, self).to_map()
@@ -1193,17 +1005,15 @@
             temp_model = RecognizeBusinessLicenseResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeCarInvoiceRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeCarInvoiceRequest, self).to_map()
@@ -1302,17 +1112,15 @@
             temp_model = RecognizeCarInvoiceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeCarNumberRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeCarNumberRequest, self).to_map()
@@ -1411,17 +1219,15 @@
             temp_model = RecognizeCarNumberResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeCarVinCodeRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeCarVinCodeRequest, self).to_map()
@@ -1520,19 +1326,16 @@
             temp_model = RecognizeCarVinCodeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeChinesePassportRequest(TeaModel):
     def __init__(self, output_figure=None, url=None, body=None):
-        # 是否需要图案检测功能，默认需要
         self.output_figure = output_figure  # type: bool
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeChinesePassportRequest, self).to_map()
@@ -1557,21 +1360,17 @@
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
 
 
 class RecognizeChinesePassportResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
         self.code = code  # type: str
-        # 返回数据
         self.data = data  # type: str
-        # 错误提示
         self.message = message  # type: str
-        # 请求唯一 ID
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeChinesePassportResponseBody, self).to_map()
@@ -1639,17 +1438,15 @@
             temp_model = RecognizeChinesePassportResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeCommonPrintedInvoiceRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeCommonPrintedInvoiceRequest, self).to_map()
@@ -1670,21 +1467,17 @@
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
 
 
 class RecognizeCommonPrintedInvoiceResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
         self.code = code  # type: str
-        # 返回数据
         self.data = data  # type: str
-        # 错误提示
         self.message = message  # type: str
-        # 请求唯一 ID
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeCommonPrintedInvoiceResponseBody, self).to_map()
@@ -1752,17 +1545,15 @@
             temp_model = RecognizeCommonPrintedInvoiceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeCosmeticProduceLicenseRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeCosmeticProduceLicenseRequest, self).to_map()
@@ -1862,17 +1653,15 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeCovidTestReportRequest(TeaModel):
     def __init__(self, multiple_result=None, url=None, body=None):
         self.multiple_result = multiple_result  # type: bool
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeCovidTestReportRequest, self).to_map()
@@ -1897,21 +1686,17 @@
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
 
 
 class RecognizeCovidTestReportResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
         self.code = code  # type: str
-        # 返回数据
         self.data = data  # type: str
-        # 错误提示
         self.message = message  # type: str
-        # 请求唯一 ID
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeCovidTestReportResponseBody, self).to_map()
@@ -1979,17 +1764,15 @@
             temp_model = RecognizeCovidTestReportResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeCtwoMedicalDeviceManageLicenseRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeCtwoMedicalDeviceManageLicenseRequest, self).to_map()
@@ -2086,54 +1869,101 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RecognizeCtwoMedicalDeviceManageLicenseResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class RecognizeDeleteExcelRecordRequest(TeaModel):
-    def __init__(self, id=None):
-        self.id = id  # type: str
+class RecognizeDocumentStructureRequest(TeaModel):
+    def __init__(self, need_rotate=None, need_sort_page=None, no_stamp=None, output_char_info=None,
+                 output_table=None, page=None, paragraph=None, row=None, url=None, use_new_style_output=None, body=None):
+        self.need_rotate = need_rotate  # type: bool
+        self.need_sort_page = need_sort_page  # type: bool
+        self.no_stamp = no_stamp  # type: bool
+        self.output_char_info = output_char_info  # type: bool
+        self.output_table = output_table  # type: bool
+        self.page = page  # type: bool
+        self.paragraph = paragraph  # type: bool
+        self.row = row  # type: bool
+        self.url = url  # type: str
+        self.use_new_style_output = use_new_style_output  # type: bool
+        self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
-        _map = super(RecognizeDeleteExcelRecordRequest, self).to_map()
+        _map = super(RecognizeDocumentStructureRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.id is not None:
-            result['Id'] = self.id
+        if self.need_rotate is not None:
+            result['NeedRotate'] = self.need_rotate
+        if self.need_sort_page is not None:
+            result['NeedSortPage'] = self.need_sort_page
+        if self.no_stamp is not None:
+            result['NoStamp'] = self.no_stamp
+        if self.output_char_info is not None:
+            result['OutputCharInfo'] = self.output_char_info
+        if self.output_table is not None:
+            result['OutputTable'] = self.output_table
+        if self.page is not None:
+            result['Page'] = self.page
+        if self.paragraph is not None:
+            result['Paragraph'] = self.paragraph
+        if self.row is not None:
+            result['Row'] = self.row
+        if self.url is not None:
+            result['Url'] = self.url
+        if self.use_new_style_output is not None:
+            result['UseNewStyleOutput'] = self.use_new_style_output
+        if self.body is not None:
+            result['body'] = self.body
         return result
 
     def from_map(self, m=None):
         m = m or dict()
-        if m.get('Id') is not None:
-            self.id = m.get('Id')
+        if m.get('NeedRotate') is not None:
+            self.need_rotate = m.get('NeedRotate')
+        if m.get('NeedSortPage') is not None:
+            self.need_sort_page = m.get('NeedSortPage')
+        if m.get('NoStamp') is not None:
+            self.no_stamp = m.get('NoStamp')
+        if m.get('OutputCharInfo') is not None:
+            self.output_char_info = m.get('OutputCharInfo')
+        if m.get('OutputTable') is not None:
+            self.output_table = m.get('OutputTable')
+        if m.get('Page') is not None:
+            self.page = m.get('Page')
+        if m.get('Paragraph') is not None:
+            self.paragraph = m.get('Paragraph')
+        if m.get('Row') is not None:
+            self.row = m.get('Row')
+        if m.get('Url') is not None:
+            self.url = m.get('Url')
+        if m.get('UseNewStyleOutput') is not None:
+            self.use_new_style_output = m.get('UseNewStyleOutput')
+        if m.get('body') is not None:
+            self.body = m.get('body')
         return self
 
 
-class RecognizeDeleteExcelRecordResponseBody(TeaModel):
+class RecognizeDocumentStructureResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
         self.code = code  # type: str
-        # 返回数据
         self.data = data  # type: str
-        # 错误提示
         self.message = message  # type: str
-        # 请求唯一 ID
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
-        _map = super(RecognizeDeleteExcelRecordResponseBody, self).to_map()
+        _map = super(RecognizeDocumentStructureResponseBody, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
         if self.data is not None:
@@ -2153,29 +1983,29 @@
         if m.get('Message') is not None:
             self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
-class RecognizeDeleteExcelRecordResponse(TeaModel):
+class RecognizeDocumentStructureResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
-        self.body = body  # type: RecognizeDeleteExcelRecordResponseBody
+        self.body = body  # type: RecognizeDocumentStructureResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
-        _map = super(RecognizeDeleteExcelRecordResponse, self).to_map()
+        _map = super(RecognizeDocumentStructureResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.status_code is not None:
@@ -2187,24 +2017,22 @@
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = RecognizeDeleteExcelRecordResponseBody()
+            temp_model = RecognizeDocumentStructureResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeDrivingLicenseRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeDrivingLicenseRequest, self).to_map()
@@ -2303,17 +2131,15 @@
             temp_model = RecognizeDrivingLicenseResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeEduFormulaRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeEduFormulaRequest, self).to_map()
@@ -2412,17 +2238,15 @@
             temp_model = RecognizeEduFormulaResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeEduOralCalculationRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeEduOralCalculationRequest, self).to_map()
@@ -2521,23 +2345,18 @@
             temp_model = RecognizeEduOralCalculationResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeEduPaperCutRequest(TeaModel):
     def __init__(self, cut_type=None, image_type=None, subject=None, url=None, body=None):
-        # 切题类型
         self.cut_type = cut_type  # type: str
-        # 图片类型
         self.image_type = image_type  # type: str
-        # 年级学科
         self.subject = subject  # type: str
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeEduPaperCutRequest, self).to_map()
@@ -2648,23 +2467,18 @@
             temp_model = RecognizeEduPaperCutResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeEduPaperOcrRequest(TeaModel):
     def __init__(self, image_type=None, output_oricoord=None, subject=None, url=None, body=None):
-        # 图片类型
         self.image_type = image_type  # type: str
-        # 是否输出原图坐标信息(如果图片被做过旋转，图片校正等处理)
         self.output_oricoord = output_oricoord  # type: bool
-        # 年级学科
         self.subject = subject  # type: str
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeEduPaperOcrRequest, self).to_map()
@@ -2775,21 +2589,17 @@
             temp_model = RecognizeEduPaperOcrResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeEduPaperStructedRequest(TeaModel):
     def __init__(self, need_rotate=None, subject=None, url=None, body=None):
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate  # type: bool
-        # 学科类型
         self.subject = subject  # type: str
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeEduPaperStructedRequest, self).to_map()
@@ -2896,19 +2706,16 @@
             temp_model = RecognizeEduPaperStructedResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeEduQuestionOcrRequest(TeaModel):
     def __init__(self, need_rotate=None, url=None, body=None):
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate  # type: bool
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeEduQuestionOcrRequest, self).to_map()
@@ -3011,21 +2818,17 @@
             temp_model = RecognizeEduQuestionOcrResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeEnglishRequest(TeaModel):
     def __init__(self, need_rotate=None, output_table=None, url=None, body=None):
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate  # type: bool
-        # 是否输出表格识别结果，包含单元格信息
         self.output_table = output_table  # type: bool
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeEnglishRequest, self).to_map()
@@ -3132,17 +2935,15 @@
             temp_model = RecognizeEnglishResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeEstateCertificationRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeEstateCertificationRequest, self).to_map()
@@ -3239,265 +3040,18 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RecognizeEstateCertificationResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class RecognizeExcelExportRequest(TeaModel):
-    def __init__(self, file_name=None, image_op=None, ocr_image_count=None, ocr_result=None, ocr_type=None):
-        # 文件名称
-        self.file_name = file_name  # type: str
-        # 图片识别op类型
-        self.image_op = image_op  # type: str
-        # 识别图片数量
-        self.ocr_image_count = ocr_image_count  # type: long
-        # 存储图片识别结果集的oss地址
-        self.ocr_result = ocr_result  # type: str
-        # 票证类型
-        self.ocr_type = ocr_type  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(RecognizeExcelExportRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.file_name is not None:
-            result['FileName'] = self.file_name
-        if self.image_op is not None:
-            result['ImageOp'] = self.image_op
-        if self.ocr_image_count is not None:
-            result['OcrImageCount'] = self.ocr_image_count
-        if self.ocr_result is not None:
-            result['OcrResult'] = self.ocr_result
-        if self.ocr_type is not None:
-            result['OcrType'] = self.ocr_type
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('FileName') is not None:
-            self.file_name = m.get('FileName')
-        if m.get('ImageOp') is not None:
-            self.image_op = m.get('ImageOp')
-        if m.get('OcrImageCount') is not None:
-            self.ocr_image_count = m.get('OcrImageCount')
-        if m.get('OcrResult') is not None:
-            self.ocr_result = m.get('OcrResult')
-        if m.get('OcrType') is not None:
-            self.ocr_type = m.get('OcrType')
-        return self
-
-
-class RecognizeExcelExportResponseBody(TeaModel):
-    def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
-        self.code = code  # type: str
-        # 返回数据
-        self.data = data  # type: str
-        # 错误提示
-        self.message = message  # type: str
-        # 请求唯一 ID
-        self.request_id = request_id  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(RecognizeExcelExportResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.code is not None:
-            result['Code'] = self.code
-        if self.data is not None:
-            result['Data'] = self.data
-        if self.message is not None:
-            result['Message'] = self.message
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Code') is not None:
-            self.code = m.get('Code')
-        if m.get('Data') is not None:
-            self.data = m.get('Data')
-        if m.get('Message') is not None:
-            self.message = m.get('Message')
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        return self
-
-
-class RecognizeExcelExportResponse(TeaModel):
-    def __init__(self, headers=None, status_code=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.status_code = status_code  # type: int
-        self.body = body  # type: RecognizeExcelExportResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(RecognizeExcelExportResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = RecognizeExcelExportResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
-class RecognizeExcelRecordRequest(TeaModel):
-    def __init__(self, curr_page=None, page_size=None):
-        # 页码
-        self.curr_page = curr_page  # type: long
-        # 每页数据
-        self.page_size = page_size  # type: long
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(RecognizeExcelRecordRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.curr_page is not None:
-            result['CurrPage'] = self.curr_page
-        if self.page_size is not None:
-            result['PageSize'] = self.page_size
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('CurrPage') is not None:
-            self.curr_page = m.get('CurrPage')
-        if m.get('PageSize') is not None:
-            self.page_size = m.get('PageSize')
-        return self
-
-
-class RecognizeExcelRecordResponseBody(TeaModel):
-    def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
-        self.code = code  # type: str
-        # 返回数据
-        self.data = data  # type: str
-        # 错误提示
-        self.message = message  # type: str
-        # 请求唯一 ID
-        self.request_id = request_id  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(RecognizeExcelRecordResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.code is not None:
-            result['Code'] = self.code
-        if self.data is not None:
-            result['Data'] = self.data
-        if self.message is not None:
-            result['Message'] = self.message
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Code') is not None:
-            self.code = m.get('Code')
-        if m.get('Data') is not None:
-            self.data = m.get('Data')
-        if m.get('Message') is not None:
-            self.message = m.get('Message')
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        return self
-
-
-class RecognizeExcelRecordResponse(TeaModel):
-    def __init__(self, headers=None, status_code=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.status_code = status_code  # type: int
-        self.body = body  # type: RecognizeExcelRecordResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(RecognizeExcelRecordResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = RecognizeExcelRecordResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class RecognizeExitEntryPermitToHKRequest(TeaModel):
     def __init__(self, output_figure=None, url=None, body=None):
-        # 图案坐标信息输出，针对结构化，如身份证人脸头像
         self.output_figure = output_figure  # type: bool
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeExitEntryPermitToHKRequest, self).to_map()
@@ -3522,21 +3076,17 @@
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
 
 
 class RecognizeExitEntryPermitToHKResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
         self.code = code  # type: str
-        # 返回数据
         self.data = data  # type: str
-        # 错误提示
         self.message = message  # type: str
-        # 请求唯一 ID
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeExitEntryPermitToHKResponseBody, self).to_map()
@@ -3604,19 +3154,16 @@
             temp_model = RecognizeExitEntryPermitToHKResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeExitEntryPermitToMainlandRequest(TeaModel):
     def __init__(self, output_figure=None, url=None, body=None):
-        # 图案坐标信息输出，针对结构化，如身份证人脸头像
         self.output_figure = output_figure  # type: bool
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeExitEntryPermitToMainlandRequest, self).to_map()
@@ -3641,21 +3188,17 @@
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
 
 
 class RecognizeExitEntryPermitToMainlandResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
         self.code = code  # type: str
-        # 返回数据
         self.data = data  # type: str
-        # 错误提示
         self.message = message  # type: str
-        # 请求唯一 ID
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeExitEntryPermitToMainlandResponseBody, self).to_map()
@@ -3723,17 +3266,15 @@
             temp_model = RecognizeExitEntryPermitToMainlandResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeFoodManageLicenseRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeFoodManageLicenseRequest, self).to_map()
@@ -3832,17 +3373,15 @@
             temp_model = RecognizeFoodManageLicenseResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeFoodProduceLicenseRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeFoodProduceLicenseRequest, self).to_map()
@@ -3941,17 +3480,15 @@
             temp_model = RecognizeFoodProduceLicenseResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeGeneralRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeGeneralRequest, self).to_map()
@@ -4051,25 +3588,19 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeHandwritingRequest(TeaModel):
     def __init__(self, need_rotate=None, need_sort_page=None, output_char_info=None, output_table=None, url=None,
                  body=None):
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate  # type: bool
-        # 是否按顺序输出文字块。false表示从左往右，从上到下的顺序；true表示从上到下，从左往右的顺序
         self.need_sort_page = need_sort_page  # type: bool
-        # 是否输出单字识别结果
         self.output_char_info = output_char_info  # type: bool
-        # 是否输出表格识别结果，包含单元格信息
         self.output_table = output_table  # type: bool
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeHandwritingRequest, self).to_map()
@@ -4184,17 +3715,15 @@
             temp_model = RecognizeHandwritingResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeHealthCodeRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeHealthCodeRequest, self).to_map()
@@ -4215,21 +3744,17 @@
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
 
 
 class RecognizeHealthCodeResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
         self.code = code  # type: str
-        # 返回数据
         self.data = data  # type: str
-        # 错误提示
         self.message = message  # type: str
-        # 请求唯一 ID
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeHealthCodeResponseBody, self).to_map()
@@ -4297,17 +3822,15 @@
             temp_model = RecognizeHealthCodeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeHotelConsumeRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeHotelConsumeRequest, self).to_map()
@@ -4407,17 +3930,15 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeHouseholdRequest(TeaModel):
     def __init__(self, is_resident_page=None, url=None, body=None):
         self.is_resident_page = is_resident_page  # type: bool
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeHouseholdRequest, self).to_map()
@@ -4520,19 +4041,16 @@
             temp_model = RecognizeHouseholdResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeIdcardRequest(TeaModel):
     def __init__(self, output_figure=None, url=None, body=None):
-        # 是否需要图案检测功能，默认不需要
         self.output_figure = output_figure  # type: bool
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeIdcardRequest, self).to_map()
@@ -4635,17 +4153,15 @@
             temp_model = RecognizeIdcardResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeInvoiceRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeInvoiceRequest, self).to_map()
@@ -4744,23 +4260,18 @@
             temp_model = RecognizeInvoiceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeJanpaneseRequest(TeaModel):
     def __init__(self, need_rotate=None, output_char_info=None, output_table=None, url=None, body=None):
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate  # type: bool
-        # 是否输出单字识别结果
         self.output_char_info = output_char_info  # type: bool
-        # 是否输出表格识别结果，包含单元格信息
         self.output_table = output_table  # type: bool
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeJanpaneseRequest, self).to_map()
@@ -4871,23 +4382,18 @@
             temp_model = RecognizeJanpaneseResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeKoreanRequest(TeaModel):
     def __init__(self, need_rotate=None, output_char_info=None, output_table=None, url=None, body=None):
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate  # type: bool
-        # 是否输出单字识别结果
         self.output_char_info = output_char_info  # type: bool
-        # 是否输出表格识别结果，包含单元格信息
         self.output_table = output_table  # type: bool
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeKoreanRequest, self).to_map()
@@ -4998,23 +4504,18 @@
             temp_model = RecognizeKoreanResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeLatinRequest(TeaModel):
     def __init__(self, need_rotate=None, output_char_info=None, output_table=None, url=None, body=None):
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate  # type: bool
-        # 是否输出单字识别结果
         self.output_char_info = output_char_info  # type: bool
-        # 是否输出表格识别结果，包含单元格信息
         self.output_table = output_table  # type: bool
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeLatinRequest, self).to_map()
@@ -5125,17 +4626,15 @@
             temp_model = RecognizeLatinResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeMedicalDeviceManageLicenseRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeMedicalDeviceManageLicenseRequest, self).to_map()
@@ -5234,17 +4733,15 @@
             temp_model = RecognizeMedicalDeviceManageLicenseResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeMedicalDeviceProduceLicenseRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeMedicalDeviceProduceLicenseRequest, self).to_map()
@@ -5343,17 +4840,15 @@
             temp_model = RecognizeMedicalDeviceProduceLicenseResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeMixedInvoicesRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeMixedInvoicesRequest, self).to_map()
@@ -5453,27 +4948,20 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeMultiLanguageRequest(TeaModel):
     def __init__(self, languages=None, need_rotate=None, need_sort_page=None, output_char_info=None,
                  output_table=None, url=None, body=None):
-        # 识别语种
         self.languages = languages  # type: list[str]
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate  # type: bool
-        # 是否按顺序输出文字块。false表示从左往右，从上到下的顺序；true表示从上到下，从左往右的顺序
         self.need_sort_page = need_sort_page  # type: bool
-        # 是否输出单字识别结果
         self.output_char_info = output_char_info  # type: bool
-        # 是否输出表格识别结果，包含单元格信息
         self.output_table = output_table  # type: bool
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeMultiLanguageRequest, self).to_map()
@@ -5515,27 +5003,20 @@
             self.body = m.get('body')
         return self
 
 
 class RecognizeMultiLanguageShrinkRequest(TeaModel):
     def __init__(self, languages_shrink=None, need_rotate=None, need_sort_page=None, output_char_info=None,
                  output_table=None, url=None, body=None):
-        # 识别语种
         self.languages_shrink = languages_shrink  # type: str
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate  # type: bool
-        # 是否按顺序输出文字块。false表示从左往右，从上到下的顺序；true表示从上到下，从左往右的顺序
         self.need_sort_page = need_sort_page  # type: bool
-        # 是否输出单字识别结果
         self.output_char_info = output_char_info  # type: bool
-        # 是否输出表格识别结果，包含单元格信息
         self.output_table = output_table  # type: bool
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeMultiLanguageShrinkRequest, self).to_map()
@@ -5654,17 +5135,15 @@
             temp_model = RecognizeMultiLanguageResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeNonTaxInvoiceRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeNonTaxInvoiceRequest, self).to_map()
@@ -5763,17 +5242,15 @@
             temp_model = RecognizeNonTaxInvoiceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizePassportRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizePassportRequest, self).to_map()
@@ -5872,17 +5349,15 @@
             temp_model = RecognizePassportResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizePaymentRecordRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizePaymentRecordRequest, self).to_map()
@@ -5981,17 +5456,15 @@
             temp_model = RecognizePaymentRecordResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizePurchaseRecordRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizePurchaseRecordRequest, self).to_map()
@@ -6090,17 +5563,15 @@
             temp_model = RecognizePurchaseRecordResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeQuotaInvoiceRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeQuotaInvoiceRequest, self).to_map()
@@ -6199,17 +5670,15 @@
             temp_model = RecognizeQuotaInvoiceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeRideHailingItineraryRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeRideHailingItineraryRequest, self).to_map()
@@ -6230,21 +5699,17 @@
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
 
 
 class RecognizeRideHailingItineraryResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
         self.code = code  # type: str
-        # 返回数据
         self.data = data  # type: str
-        # 错误提示
         self.message = message  # type: str
-        # 请求唯一 ID
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeRideHailingItineraryResponseBody, self).to_map()
@@ -6312,17 +5777,15 @@
             temp_model = RecognizeRideHailingItineraryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeRollTicketRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeRollTicketRequest, self).to_map()
@@ -6421,23 +5884,18 @@
             temp_model = RecognizeRollTicketResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeRussianRequest(TeaModel):
     def __init__(self, need_rotate=None, output_char_info=None, output_table=None, url=None, body=None):
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate  # type: bool
-        # 是否输出单字识别结果
         self.output_char_info = output_char_info  # type: bool
-        # 是否输出表格识别结果，包含单元格信息
         self.output_table = output_table  # type: bool
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeRussianRequest, self).to_map()
@@ -6548,17 +6006,15 @@
             temp_model = RecognizeRussianResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeShoppingReceiptRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeShoppingReceiptRequest, self).to_map()
@@ -6579,21 +6035,17 @@
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
 
 
 class RecognizeShoppingReceiptResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
         self.code = code  # type: str
-        # 返回数据
         self.data = data  # type: str
-        # 错误提示
         self.message = message  # type: str
-        # 请求唯一 ID
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeShoppingReceiptResponseBody, self).to_map()
@@ -6661,17 +6113,15 @@
             temp_model = RecognizeShoppingReceiptResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeSocialSecurityCardRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeSocialSecurityCardRequest, self).to_map()
@@ -6692,21 +6142,17 @@
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
 
 
 class RecognizeSocialSecurityCardResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
         self.code = code  # type: str
-        # 返回数据
         self.data = data  # type: str
-        # 错误提示
         self.message = message  # type: str
-        # 请求唯一 ID
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeSocialSecurityCardResponseBody, self).to_map()
@@ -6774,17 +6220,15 @@
             temp_model = RecognizeSocialSecurityCardResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeSocialSecurityCardVersionIIRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeSocialSecurityCardVersionIIRequest, self).to_map()
@@ -6805,21 +6249,17 @@
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
 
 
 class RecognizeSocialSecurityCardVersionIIResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
         self.code = code  # type: str
-        # 返回数据
         self.data = data  # type: str
-        # 错误提示
         self.message = message  # type: str
-        # 请求唯一 ID
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeSocialSecurityCardVersionIIResponseBody, self).to_map()
@@ -6887,23 +6327,18 @@
             temp_model = RecognizeSocialSecurityCardVersionIIResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeTableOcrRequest(TeaModel):
     def __init__(self, line_less=None, need_rotate=None, skip_detection=None, url=None, body=None):
-        # 是否无线条
         self.line_less = line_less  # type: bool
-        # 是否需要自动旋转功能，默认需要
         self.need_rotate = need_rotate  # type: bool
-        # 是否跳过表格识别，如果没有检测到表格，可以设置"skip_detection":true
         self.skip_detection = skip_detection  # type: bool
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeTableOcrRequest, self).to_map()
@@ -7014,17 +6449,15 @@
             temp_model = RecognizeTableOcrResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeTaxClearanceCertificateRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeTaxClearanceCertificateRequest, self).to_map()
@@ -7045,21 +6478,17 @@
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
 
 
 class RecognizeTaxClearanceCertificateResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
         self.code = code  # type: str
-        # 返回数据
         self.data = data  # type: str
-        # 错误提示
         self.message = message  # type: str
-        # 请求唯一 ID
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeTaxClearanceCertificateResponseBody, self).to_map()
@@ -7127,17 +6556,15 @@
             temp_model = RecognizeTaxClearanceCertificateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeTaxiInvoiceRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeTaxiInvoiceRequest, self).to_map()
@@ -7236,23 +6663,18 @@
             temp_model = RecognizeTaxiInvoiceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeThaiRequest(TeaModel):
     def __init__(self, need_rotate=None, output_char_info=None, output_table=None, url=None, body=None):
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate  # type: bool
-        # 是否输出单字识别结果
         self.output_char_info = output_char_info  # type: bool
-        # 是否输出表格识别结果，包含单元格信息
         self.output_table = output_table  # type: bool
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeThaiRequest, self).to_map()
@@ -7363,17 +6785,15 @@
             temp_model = RecognizeThaiResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeTollInvoiceRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeTollInvoiceRequest, self).to_map()
@@ -7394,21 +6814,17 @@
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
 
 
 class RecognizeTollInvoiceResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
         self.code = code  # type: str
-        # 返回数据
         self.data = data  # type: str
-        # 错误提示
         self.message = message  # type: str
-        # 请求唯一 ID
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeTollInvoiceResponseBody, self).to_map()
@@ -7476,17 +6892,15 @@
             temp_model = RecognizeTollInvoiceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeTradeMarkCertificationRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeTradeMarkCertificationRequest, self).to_map()
@@ -7585,17 +6999,15 @@
             temp_model = RecognizeTradeMarkCertificationResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeTrainInvoiceRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeTrainInvoiceRequest, self).to_map()
@@ -7694,17 +7106,15 @@
             temp_model = RecognizeTrainInvoiceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeTravelCardRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeTravelCardRequest, self).to_map()
@@ -7725,21 +7135,17 @@
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
 
 
 class RecognizeTravelCardResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
         self.code = code  # type: str
-        # 返回数据
         self.data = data  # type: str
-        # 错误提示
         self.message = message  # type: str
-        # 请求唯一 ID
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeTravelCardResponseBody, self).to_map()
@@ -7807,17 +7213,15 @@
             temp_model = RecognizeTravelCardResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeUsedCarInvoiceRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeUsedCarInvoiceRequest, self).to_map()
@@ -7838,21 +7242,17 @@
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
 
 
 class RecognizeUsedCarInvoiceResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
         self.code = code  # type: str
-        # 返回数据
         self.data = data  # type: str
-        # 错误提示
         self.message = message  # type: str
-        # 请求唯一 ID
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeUsedCarInvoiceResponseBody, self).to_map()
@@ -7920,17 +7320,15 @@
             temp_model = RecognizeUsedCarInvoiceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeVehicleCertificationRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeVehicleCertificationRequest, self).to_map()
@@ -7951,21 +7349,17 @@
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
 
 
 class RecognizeVehicleCertificationResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
         self.code = code  # type: str
-        # 返回数据
         self.data = data  # type: str
-        # 错误提示
         self.message = message  # type: str
-        # 请求唯一 ID
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeVehicleCertificationResponseBody, self).to_map()
@@ -8033,17 +7427,15 @@
             temp_model = RecognizeVehicleCertificationResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeVehicleLicenseRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeVehicleLicenseRequest, self).to_map()
@@ -8142,17 +7534,15 @@
             temp_model = RecognizeVehicleLicenseResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeVehicleRegistrationRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeVehicleRegistrationRequest, self).to_map()
@@ -8173,21 +7563,17 @@
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
 
 
 class RecognizeVehicleRegistrationResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # 错误码
         self.code = code  # type: str
-        # 返回数据
         self.data = data  # type: str
-        # 错误提示
         self.message = message  # type: str
-        # 请求唯一 ID
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeVehicleRegistrationResponseBody, self).to_map()
@@ -8255,17 +7641,15 @@
             temp_model = RecognizeVehicleRegistrationResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeWaybillRequest(TeaModel):
     def __init__(self, url=None, body=None):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url  # type: str
-        # 图片二进制字节流，最大10MB
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeWaybillRequest, self).to_map()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `alibabacloud_ocr-api20210707_py2-1.1.7/alibabacloud_ocr_api20210707_py2.egg-info/PKG-INFO` & `alibabacloud_ocr-api20210707_py2-1.1.8/alibabacloud_ocr_api20210707_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ocr-api20210707-py2
-Version: 1.1.7
+Version: 1.1.8
 Summary: Alibaba Cloud ocr-api (20210707) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ocr-api20210707_py2-1.1.7/setup.py` & `alibabacloud_ocr-api20210707_py2-1.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ocr-api20210707_py2.
 
-Created on 20/06/2022
+Created on 23/08/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ocr_api20210707"
 NAME = "alibabacloud_ocr-api20210707_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ocr-api (20210707) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.5, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.6, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.3, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.0.8, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
```

