# Comparing `tmp/alibabacloud_ocr-api20210707-1.1.7.tar.gz` & `tmp/alibabacloud_ocr-api20210707-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ocr-api20210707-1.1.7.tar", last modified: Mon Jun 20 05:54:32 2022, max compression
+gzip compressed data, was "dist/alibabacloud_ocr-api20210707-1.1.8.tar", last modified: Tue Aug 23 05:31:51 2022, max compression
```

## Comparing `alibabacloud_ocr-api20210707-1.1.7.tar` & `alibabacloud_ocr-api20210707-1.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 05:54:32.000000 alibabacloud_ocr-api20210707-1.1.7/
--rw-r--r--   0 root         (0) root         (0)      425 2022-06-20 05:54:32.000000 alibabacloud_ocr-api20210707-1.1.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-06-20 05:54:32.000000 alibabacloud_ocr-api20210707-1.1.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-06-20 05:54:32.000000 alibabacloud_ocr-api20210707-1.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2352 2022-06-20 05:54:32.000000 alibabacloud_ocr-api20210707-1.1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1034 2022-06-20 05:54:32.000000 alibabacloud_ocr-api20210707-1.1.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2022-06-20 05:54:32.000000 alibabacloud_ocr-api20210707-1.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 05:54:32.000000 alibabacloud_ocr-api20210707-1.1.7/alibabacloud_ocr_api20210707/
--rw-r--r--   0 root         (0) root         (0)       21 2022-06-20 05:54:32.000000 alibabacloud_ocr-api20210707-1.1.7/alibabacloud_ocr_api20210707/__init__.py
--rw-r--r--   0 root         (0) root         (0)   217477 2022-06-20 05:54:32.000000 alibabacloud_ocr-api20210707-1.1.7/alibabacloud_ocr_api20210707/client.py
--rw-r--r--   0 root         (0) root         (0)   279370 2022-06-20 05:54:32.000000 alibabacloud_ocr-api20210707-1.1.7/alibabacloud_ocr_api20210707/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 05:54:32.000000 alibabacloud_ocr-api20210707-1.1.7/alibabacloud_ocr_api20210707.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2352 2022-06-20 05:54:32.000000 alibabacloud_ocr-api20210707-1.1.7/alibabacloud_ocr_api20210707.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2022-06-20 05:54:32.000000 alibabacloud_ocr-api20210707-1.1.7/alibabacloud_ocr_api20210707.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-20 05:54:32.000000 alibabacloud_ocr-api20210707-1.1.7/alibabacloud_ocr_api20210707.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-06-20 05:54:32.000000 alibabacloud_ocr-api20210707-1.1.7/alibabacloud_ocr_api20210707.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2022-06-20 05:54:32.000000 alibabacloud_ocr-api20210707-1.1.7/alibabacloud_ocr_api20210707.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-06-20 05:54:32.000000 alibabacloud_ocr-api20210707-1.1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2632 2022-06-20 05:54:32.000000 alibabacloud_ocr-api20210707-1.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 05:31:51.000000 alibabacloud_ocr-api20210707-1.1.8/
+-rw-r--r--   0 root         (0) root         (0)      464 2022-08-23 05:31:51.000000 alibabacloud_ocr-api20210707-1.1.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-08-23 05:31:51.000000 alibabacloud_ocr-api20210707-1.1.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-08-23 05:31:51.000000 alibabacloud_ocr-api20210707-1.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2352 2022-08-23 05:31:51.000000 alibabacloud_ocr-api20210707-1.1.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1034 2022-08-23 05:31:51.000000 alibabacloud_ocr-api20210707-1.1.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2022-08-23 05:31:51.000000 alibabacloud_ocr-api20210707-1.1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 05:31:51.000000 alibabacloud_ocr-api20210707-1.1.8/alibabacloud_ocr_api20210707/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-08-23 05:31:51.000000 alibabacloud_ocr-api20210707-1.1.8/alibabacloud_ocr_api20210707/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   208951 2022-08-23 05:31:51.000000 alibabacloud_ocr-api20210707-1.1.8/alibabacloud_ocr_api20210707/client.py
+-rw-r--r--   0 root         (0) root         (0)   254009 2022-08-23 05:31:51.000000 alibabacloud_ocr-api20210707-1.1.8/alibabacloud_ocr_api20210707/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 05:31:51.000000 alibabacloud_ocr-api20210707-1.1.8/alibabacloud_ocr_api20210707.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2352 2022-08-23 05:31:51.000000 alibabacloud_ocr-api20210707-1.1.8/alibabacloud_ocr_api20210707.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2022-08-23 05:31:51.000000 alibabacloud_ocr-api20210707-1.1.8/alibabacloud_ocr_api20210707.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-23 05:31:51.000000 alibabacloud_ocr-api20210707-1.1.8/alibabacloud_ocr_api20210707.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-08-23 05:31:51.000000 alibabacloud_ocr-api20210707-1.1.8/alibabacloud_ocr_api20210707.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2022-08-23 05:31:51.000000 alibabacloud_ocr-api20210707-1.1.8/alibabacloud_ocr_api20210707.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-08-23 05:31:51.000000 alibabacloud_ocr-api20210707-1.1.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2632 2022-08-23 05:31:51.000000 alibabacloud_ocr-api20210707-1.1.8/setup.py
```

### Comparing `alibabacloud_ocr-api20210707-1.1.7/LICENSE` & `alibabacloud_ocr-api20210707-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ocr-api20210707-1.1.7/PKG-INFO` & `alibabacloud_ocr-api20210707-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ocr-api20210707
-Version: 1.1.7
+Version: 1.1.8
 Summary: Alibaba Cloud ocr-api (20210707) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ocr-api20210707-1.1.7/README-CN.md` & `alibabacloud_ocr-api20210707-1.1.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ocr-api20210707-1.1.7/README.md` & `alibabacloud_ocr-api20210707-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ocr-api20210707-1.1.7/alibabacloud_ocr_api20210707/client.py` & `alibabacloud_ocr-api20210707-1.1.8/alibabacloud_ocr_api20210707/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -513,112 +513,14 @@
     async def recognize_basic_async(
         self,
         request: ocr_api_20210707_models.RecognizeBasicRequest,
     ) -> ocr_api_20210707_models.RecognizeBasicResponse:
         runtime = util_models.RuntimeOptions()
         return await self.recognize_basic_with_options_async(request, runtime)
 
-    def recognize_batch_recognize_with_options(
-        self,
-        request: ocr_api_20210707_models.RecognizeBatchRecognizeRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_api_20210707_models.RecognizeBatchRecognizeResponse:
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
-    async def recognize_batch_recognize_with_options_async(
-        self,
-        request: ocr_api_20210707_models.RecognizeBatchRecognizeRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_api_20210707_models.RecognizeBatchRecognizeResponse:
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
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def recognize_batch_recognize(
-        self,
-        request: ocr_api_20210707_models.RecognizeBatchRecognizeRequest,
-    ) -> ocr_api_20210707_models.RecognizeBatchRecognizeResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.recognize_batch_recognize_with_options(request, runtime)
-
-    async def recognize_batch_recognize_async(
-        self,
-        request: ocr_api_20210707_models.RecognizeBatchRecognizeRequest,
-    ) -> ocr_api_20210707_models.RecognizeBatchRecognizeResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.recognize_batch_recognize_with_options_async(request, runtime)
-
     def recognize_birth_certification_with_options(
         self,
         request: ocr_api_20210707_models.RecognizeBirthCertificationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocr_api_20210707_models.RecognizeBirthCertificationResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -1433,83 +1335,123 @@
     async def recognize_ctwo_medical_device_manage_license_async(
         self,
         request: ocr_api_20210707_models.RecognizeCtwoMedicalDeviceManageLicenseRequest,
     ) -> ocr_api_20210707_models.RecognizeCtwoMedicalDeviceManageLicenseResponse:
         runtime = util_models.RuntimeOptions()
         return await self.recognize_ctwo_medical_device_manage_license_with_options_async(request, runtime)
 
-    def recognize_delete_excel_record_with_options(
+    def recognize_document_structure_with_options(
         self,
-        request: ocr_api_20210707_models.RecognizeDeleteExcelRecordRequest,
+        request: ocr_api_20210707_models.RecognizeDocumentStructureRequest,
         runtime: util_models.RuntimeOptions,
-    ) -> ocr_api_20210707_models.RecognizeDeleteExcelRecordResponse:
+    ) -> ocr_api_20210707_models.RecognizeDocumentStructureResponse:
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
 
-    async def recognize_delete_excel_record_with_options_async(
+    async def recognize_document_structure_with_options_async(
         self,
-        request: ocr_api_20210707_models.RecognizeDeleteExcelRecordRequest,
+        request: ocr_api_20210707_models.RecognizeDocumentStructureRequest,
         runtime: util_models.RuntimeOptions,
-    ) -> ocr_api_20210707_models.RecognizeDeleteExcelRecordResponse:
+    ) -> ocr_api_20210707_models.RecognizeDocumentStructureResponse:
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
             await self.call_api_async(params, req, runtime)
         )
 
-    def recognize_delete_excel_record(
+    def recognize_document_structure(
         self,
-        request: ocr_api_20210707_models.RecognizeDeleteExcelRecordRequest,
-    ) -> ocr_api_20210707_models.RecognizeDeleteExcelRecordResponse:
+        request: ocr_api_20210707_models.RecognizeDocumentStructureRequest,
+    ) -> ocr_api_20210707_models.RecognizeDocumentStructureResponse:
         runtime = util_models.RuntimeOptions()
-        return self.recognize_delete_excel_record_with_options(request, runtime)
+        return self.recognize_document_structure_with_options(request, runtime)
 
-    async def recognize_delete_excel_record_async(
+    async def recognize_document_structure_async(
         self,
-        request: ocr_api_20210707_models.RecognizeDeleteExcelRecordRequest,
-    ) -> ocr_api_20210707_models.RecognizeDeleteExcelRecordResponse:
+        request: ocr_api_20210707_models.RecognizeDocumentStructureRequest,
+    ) -> ocr_api_20210707_models.RecognizeDocumentStructureResponse:
         runtime = util_models.RuntimeOptions()
-        return await self.recognize_delete_excel_record_with_options_async(request, runtime)
+        return await self.recognize_document_structure_with_options_async(request, runtime)
 
     def recognize_driving_license_with_options(
         self,
         request: ocr_api_20210707_models.RecognizeDrivingLicenseRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocr_api_20210707_models.RecognizeDrivingLicenseResponse:
         UtilClient.validate_model(request)
@@ -2213,174 +2155,14 @@
     async def recognize_estate_certification_async(
         self,
         request: ocr_api_20210707_models.RecognizeEstateCertificationRequest,
     ) -> ocr_api_20210707_models.RecognizeEstateCertificationResponse:
         runtime = util_models.RuntimeOptions()
         return await self.recognize_estate_certification_with_options_async(request, runtime)
 
-    def recognize_excel_export_with_options(
-        self,
-        request: ocr_api_20210707_models.RecognizeExcelExportRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_api_20210707_models.RecognizeExcelExportResponse:
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
-    async def recognize_excel_export_with_options_async(
-        self,
-        request: ocr_api_20210707_models.RecognizeExcelExportRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_api_20210707_models.RecognizeExcelExportResponse:
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
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def recognize_excel_export(
-        self,
-        request: ocr_api_20210707_models.RecognizeExcelExportRequest,
-    ) -> ocr_api_20210707_models.RecognizeExcelExportResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.recognize_excel_export_with_options(request, runtime)
-
-    async def recognize_excel_export_async(
-        self,
-        request: ocr_api_20210707_models.RecognizeExcelExportRequest,
-    ) -> ocr_api_20210707_models.RecognizeExcelExportResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.recognize_excel_export_with_options_async(request, runtime)
-
-    def recognize_excel_record_with_options(
-        self,
-        request: ocr_api_20210707_models.RecognizeExcelRecordRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_api_20210707_models.RecognizeExcelRecordResponse:
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
-    async def recognize_excel_record_with_options_async(
-        self,
-        request: ocr_api_20210707_models.RecognizeExcelRecordRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_api_20210707_models.RecognizeExcelRecordResponse:
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
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def recognize_excel_record(
-        self,
-        request: ocr_api_20210707_models.RecognizeExcelRecordRequest,
-    ) -> ocr_api_20210707_models.RecognizeExcelRecordResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.recognize_excel_record_with_options(request, runtime)
-
-    async def recognize_excel_record_async(
-        self,
-        request: ocr_api_20210707_models.RecognizeExcelRecordRequest,
-    ) -> ocr_api_20210707_models.RecognizeExcelRecordResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.recognize_excel_record_with_options_async(request, runtime)
-
     def recognize_exit_entry_permit_to_hkwith_options(
         self,
         request: ocr_api_20210707_models.RecognizeExitEntryPermitToHKRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocr_api_20210707_models.RecognizeExitEntryPermitToHKResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_ocr-api20210707-1.1.7/alibabacloud_ocr_api20210707/models.py` & `alibabacloud_ocr-api20210707-1.1.8/alibabacloud_ocr_api20210707/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,33 +14,23 @@
         output_figure: bool = None,
         output_table: bool = None,
         paragraph: bool = None,
         row: bool = None,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate
-        # 是否按顺序输出文字块。false表示从左往右，从上到下的顺序；true表示从上到下，从左往右的顺序
         self.need_sort_page = need_sort_page
-        # 是否需要去除印章功能，默认不需要。true：需要 false：不需要
         self.no_stamp = no_stamp
-        # 是否输出单字识别结果
         self.output_char_info = output_char_info
-        # 是否需要图案检测功能，默认不需要。true：需要 false：不需要
         self.output_figure = output_figure
-        # 是否输出表格识别结果，包含单元格信息
         self.output_table = output_table
-        # 是否需要分段功能，默认不需要。true：需要 false：不需要
         self.paragraph = paragraph
-        # 是否需要成行返回功能，默认不需要
         self.row = row
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -99,21 +89,17 @@
     def __init__(
         self,
         code: str = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
-        # 错误码
         self.code = code
-        # 返回数据
         self.data = data
-        # 错误提示
         self.message = message
-        # 请求唯一 ID
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -190,17 +176,15 @@
 
 class RecognizeAirItineraryRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -314,17 +298,15 @@
 
 class RecognizeBankAcceptanceRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -351,21 +333,17 @@
     def __init__(
         self,
         code: str = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
-        # 错误码
         self.code = code
-        # 返回数据
         self.data = data
-        # 错误提示
         self.message = message
-        # 请求唯一 ID
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -442,17 +420,15 @@
 
 class RecognizeBankAccountLicenseRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -566,17 +542,15 @@
 
 class RecognizeBankCardRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -690,17 +664,15 @@
 
 class RecognizeBasicRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -808,193 +780,21 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RecognizeBasicResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class RecognizeBatchRecognizeRequest(TeaModel):
-    def __init__(
-        self,
-        image_name: str = None,
-        image_op: str = None,
-        image_oss_key: str = None,
-        need_rotate: bool = None,
-        need_sort_page: bool = None,
-        output_char_info: bool = None,
-        output_table: bool = None,
-        url: str = None,
-    ):
-        # 图片名称
-        self.image_name = image_name
-        # 图片识别op类型
-        self.image_op = image_op
-        # 图片存入oss中的key
-        self.image_oss_key = image_oss_key
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
-        self.need_rotate = need_rotate
-        # 是否按顺序输出文字块。false表示从左往右，从上到下的顺序；true表示从上到下，从左往右的顺序
-        self.need_sort_page = need_sort_page
-        # 是否输出单字识别结果
-        self.output_char_info = output_char_info
-        # 是否输出表格识别结果，包含单元格信息
-        self.output_table = output_table
-        # 图片链接（长度不超 2048，不支持 base64）
-        self.url = url
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
-    def __init__(
-        self,
-        code: str = None,
-        data: str = None,
-        message: str = None,
-        request_id: str = None,
-    ):
-        # 错误码
-        self.code = code
-        # 返回数据
-        self.data = data
-        # 错误提示
-        self.message = message
-        # 请求唯一 ID
-        self.request_id = request_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
-    def __init__(
-        self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: RecognizeBatchRecognizeResponseBody = None,
-    ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1108,17 +908,15 @@
 
 class RecognizeBusShipTicketRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1145,21 +943,17 @@
     def __init__(
         self,
         code: str = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
-        # 错误码
         self.code = code
-        # 返回数据
         self.data = data
-        # 错误提示
         self.message = message
-        # 请求唯一 ID
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1236,17 +1030,15 @@
 
 class RecognizeBusinessLicenseRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1360,17 +1152,15 @@
 
 class RecognizeCarInvoiceRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1484,17 +1274,15 @@
 
 class RecognizeCarNumberRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1608,17 +1396,15 @@
 
 class RecognizeCarVinCodeRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1733,19 +1519,16 @@
 class RecognizeChinesePassportRequest(TeaModel):
     def __init__(
         self,
         output_figure: bool = None,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 是否需要图案检测功能，默认需要
         self.output_figure = output_figure
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1776,21 +1559,17 @@
     def __init__(
         self,
         code: str = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
-        # 错误码
         self.code = code
-        # 返回数据
         self.data = data
-        # 错误提示
         self.message = message
-        # 请求唯一 ID
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1867,17 +1646,15 @@
 
 class RecognizeCommonPrintedInvoiceRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1904,21 +1681,17 @@
     def __init__(
         self,
         code: str = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
-        # 错误码
         self.code = code
-        # 返回数据
         self.data = data
-        # 错误提示
         self.message = message
-        # 请求唯一 ID
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1995,17 +1768,15 @@
 
 class RecognizeCosmeticProduceLicenseRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2121,17 +1892,15 @@
     def __init__(
         self,
         multiple_result: bool = None,
         url: str = None,
         body: BinaryIO = None,
     ):
         self.multiple_result = multiple_result
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2162,21 +1931,17 @@
     def __init__(
         self,
         code: str = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
-        # 错误码
         self.code = code
-        # 返回数据
         self.data = data
-        # 错误提示
         self.message = message
-        # 请求唯一 ID
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2253,17 +2018,15 @@
 
 class RecognizeCtwoMedicalDeviceManageLicenseRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2371,56 +2134,112 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RecognizeCtwoMedicalDeviceManageLicenseResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class RecognizeDeleteExcelRecordRequest(TeaModel):
+class RecognizeDocumentStructureRequest(TeaModel):
     def __init__(
         self,
-        id: str = None,
+        need_rotate: bool = None,
+        need_sort_page: bool = None,
+        no_stamp: bool = None,
+        output_char_info: bool = None,
+        output_table: bool = None,
+        page: bool = None,
+        paragraph: bool = None,
+        row: bool = None,
+        url: str = None,
+        use_new_style_output: bool = None,
+        body: BinaryIO = None,
     ):
-        self.id = id
+        self.need_rotate = need_rotate
+        self.need_sort_page = need_sort_page
+        self.no_stamp = no_stamp
+        self.output_char_info = output_char_info
+        self.output_table = output_table
+        self.page = page
+        self.paragraph = paragraph
+        self.row = row
+        self.url = url
+        self.use_new_style_output = use_new_style_output
+        self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
     def __init__(
         self,
         code: str = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
-        # 错误码
         self.code = code
-        # 返回数据
         self.data = data
-        # 错误提示
         self.message = message
-        # 请求唯一 ID
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2447,20 +2266,20 @@
         if m.get('Message') is not None:
             self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
-class RecognizeDeleteExcelRecordResponse(TeaModel):
+class RecognizeDocumentStructureResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: RecognizeDeleteExcelRecordResponseBody = None,
+        body: RecognizeDocumentStructureResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -2486,28 +2305,26 @@
     def from_map(self, m: dict = None):
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
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2621,17 +2438,15 @@
 
 class RecognizeEduFormulaRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2745,17 +2560,15 @@
 
 class RecognizeEduOralCalculationRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2872,23 +2685,18 @@
         self,
         cut_type: str = None,
         image_type: str = None,
         subject: str = None,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 切题类型
         self.cut_type = cut_type
-        # 图片类型
         self.image_type = image_type
-        # 年级学科
         self.subject = subject
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3017,23 +2825,18 @@
         self,
         image_type: str = None,
         output_oricoord: bool = None,
         subject: str = None,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片类型
         self.image_type = image_type
-        # 是否输出原图坐标信息(如果图片被做过旋转，图片校正等处理)
         self.output_oricoord = output_oricoord
-        # 年级学科
         self.subject = subject
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3161,21 +2964,17 @@
     def __init__(
         self,
         need_rotate: bool = None,
         subject: str = None,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate
-        # 学科类型
         self.subject = subject
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3298,19 +3097,16 @@
 class RecognizeEduQuestionOcrRequest(TeaModel):
     def __init__(
         self,
         need_rotate: bool = None,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3430,21 +3226,17 @@
     def __init__(
         self,
         need_rotate: bool = None,
         output_table: bool = None,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate
-        # 是否输出表格识别结果，包含单元格信息
         self.output_table = output_table
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3566,17 +3358,15 @@
 
 class RecognizeEstateCertificationRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3684,303 +3474,23 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RecognizeEstateCertificationResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class RecognizeExcelExportRequest(TeaModel):
-    def __init__(
-        self,
-        file_name: str = None,
-        image_op: str = None,
-        ocr_image_count: int = None,
-        ocr_result: str = None,
-        ocr_type: str = None,
-    ):
-        # 文件名称
-        self.file_name = file_name
-        # 图片识别op类型
-        self.image_op = image_op
-        # 识别图片数量
-        self.ocr_image_count = ocr_image_count
-        # 存储图片识别结果集的oss地址
-        self.ocr_result = ocr_result
-        # 票证类型
-        self.ocr_type = ocr_type
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
-    def __init__(
-        self,
-        code: str = None,
-        data: str = None,
-        message: str = None,
-        request_id: str = None,
-    ):
-        # 错误码
-        self.code = code
-        # 返回数据
-        self.data = data
-        # 错误提示
-        self.message = message
-        # 请求唯一 ID
-        self.request_id = request_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
-    def __init__(
-        self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: RecognizeExcelExportResponseBody = None,
-    ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
-    def __init__(
-        self,
-        curr_page: int = None,
-        page_size: int = None,
-    ):
-        # 页码
-        self.curr_page = curr_page
-        # 每页数据
-        self.page_size = page_size
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('CurrPage') is not None:
-            self.curr_page = m.get('CurrPage')
-        if m.get('PageSize') is not None:
-            self.page_size = m.get('PageSize')
-        return self
-
-
-class RecognizeExcelRecordResponseBody(TeaModel):
-    def __init__(
-        self,
-        code: str = None,
-        data: str = None,
-        message: str = None,
-        request_id: str = None,
-    ):
-        # 错误码
-        self.code = code
-        # 返回数据
-        self.data = data
-        # 错误提示
-        self.message = message
-        # 请求唯一 ID
-        self.request_id = request_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
-    def __init__(
-        self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: RecognizeExcelRecordResponseBody = None,
-    ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         output_figure: bool = None,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图案坐标信息输出，针对结构化，如身份证人脸头像
         self.output_figure = output_figure
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4011,21 +3521,17 @@
     def __init__(
         self,
         code: str = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
-        # 错误码
         self.code = code
-        # 返回数据
         self.data = data
-        # 错误提示
         self.message = message
-        # 请求唯一 ID
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4103,19 +3609,16 @@
 class RecognizeExitEntryPermitToMainlandRequest(TeaModel):
     def __init__(
         self,
         output_figure: bool = None,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图案坐标信息输出，针对结构化，如身份证人脸头像
         self.output_figure = output_figure
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4146,21 +3649,17 @@
     def __init__(
         self,
         code: str = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
-        # 错误码
         self.code = code
-        # 返回数据
         self.data = data
-        # 错误提示
         self.message = message
-        # 请求唯一 ID
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4237,17 +3736,15 @@
 
 class RecognizeFoodManageLicenseRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4361,17 +3858,15 @@
 
 class RecognizeFoodProduceLicenseRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4485,17 +3980,15 @@
 
 class RecognizeGeneralRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4613,25 +4106,19 @@
         need_rotate: bool = None,
         need_sort_page: bool = None,
         output_char_info: bool = None,
         output_table: bool = None,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate
-        # 是否按顺序输出文字块。false表示从左往右，从上到下的顺序；true表示从上到下，从左往右的顺序
         self.need_sort_page = need_sort_page
-        # 是否输出单字识别结果
         self.output_char_info = output_char_info
-        # 是否输出表格识别结果，包含单元格信息
         self.output_table = output_table
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4761,17 +4248,15 @@
 
 class RecognizeHealthCodeRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4798,21 +4283,17 @@
     def __init__(
         self,
         code: str = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
-        # 错误码
         self.code = code
-        # 返回数据
         self.data = data
-        # 错误提示
         self.message = message
-        # 请求唯一 ID
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4889,17 +4370,15 @@
 
 class RecognizeHotelConsumeRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5015,17 +4494,15 @@
     def __init__(
         self,
         is_resident_page: bool = None,
         url: str = None,
         body: BinaryIO = None,
     ):
         self.is_resident_page = is_resident_page
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5144,19 +4621,16 @@
 class RecognizeIdcardRequest(TeaModel):
     def __init__(
         self,
         output_figure: bool = None,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 是否需要图案检测功能，默认不需要
         self.output_figure = output_figure
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5274,17 +4748,15 @@
 
 class RecognizeInvoiceRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5401,23 +4873,18 @@
         self,
         need_rotate: bool = None,
         output_char_info: bool = None,
         output_table: bool = None,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate
-        # 是否输出单字识别结果
         self.output_char_info = output_char_info
-        # 是否输出表格识别结果，包含单元格信息
         self.output_table = output_table
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5546,23 +5013,18 @@
         self,
         need_rotate: bool = None,
         output_char_info: bool = None,
         output_table: bool = None,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate
-        # 是否输出单字识别结果
         self.output_char_info = output_char_info
-        # 是否输出表格识别结果，包含单元格信息
         self.output_table = output_table
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5691,23 +5153,18 @@
         self,
         need_rotate: bool = None,
         output_char_info: bool = None,
         output_table: bool = None,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate
-        # 是否输出单字识别结果
         self.output_char_info = output_char_info
-        # 是否输出表格识别结果，包含单元格信息
         self.output_table = output_table
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5833,17 +5290,15 @@
 
 class RecognizeMedicalDeviceManageLicenseRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5957,17 +5412,15 @@
 
 class RecognizeMedicalDeviceProduceLicenseRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6081,17 +5534,15 @@
 
 class RecognizeMixedInvoicesRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6210,27 +5661,20 @@
         need_rotate: bool = None,
         need_sort_page: bool = None,
         output_char_info: bool = None,
         output_table: bool = None,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 识别语种
         self.languages = languages
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate
-        # 是否按顺序输出文字块。false表示从左往右，从上到下的顺序；true表示从上到下，从左往右的顺序
         self.need_sort_page = need_sort_page
-        # 是否输出单字识别结果
         self.output_char_info = output_char_info
-        # 是否输出表格识别结果，包含单元格信息
         self.output_table = output_table
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6280,27 +5724,20 @@
         need_rotate: bool = None,
         need_sort_page: bool = None,
         output_char_info: bool = None,
         output_table: bool = None,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 识别语种
         self.languages_shrink = languages_shrink
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate
-        # 是否按顺序输出文字块。false表示从左往右，从上到下的顺序；true表示从上到下，从左往右的顺序
         self.need_sort_page = need_sort_page
-        # 是否输出单字识别结果
         self.output_char_info = output_char_info
-        # 是否输出表格识别结果，包含单元格信息
         self.output_table = output_table
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6434,17 +5871,15 @@
 
 class RecognizeNonTaxInvoiceRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6558,17 +5993,15 @@
 
 class RecognizePassportRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6682,17 +6115,15 @@
 
 class RecognizePaymentRecordRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6806,17 +6237,15 @@
 
 class RecognizePurchaseRecordRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6930,17 +6359,15 @@
 
 class RecognizeQuotaInvoiceRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7054,17 +6481,15 @@
 
 class RecognizeRideHailingItineraryRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7091,21 +6516,17 @@
     def __init__(
         self,
         code: str = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
-        # 错误码
         self.code = code
-        # 返回数据
         self.data = data
-        # 错误提示
         self.message = message
-        # 请求唯一 ID
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7182,17 +6603,15 @@
 
 class RecognizeRollTicketRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7309,23 +6728,18 @@
         self,
         need_rotate: bool = None,
         output_char_info: bool = None,
         output_table: bool = None,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate
-        # 是否输出单字识别结果
         self.output_char_info = output_char_info
-        # 是否输出表格识别结果，包含单元格信息
         self.output_table = output_table
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7451,17 +6865,15 @@
 
 class RecognizeShoppingReceiptRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7488,21 +6900,17 @@
     def __init__(
         self,
         code: str = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
-        # 错误码
         self.code = code
-        # 返回数据
         self.data = data
-        # 错误提示
         self.message = message
-        # 请求唯一 ID
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7579,17 +6987,15 @@
 
 class RecognizeSocialSecurityCardRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7616,21 +7022,17 @@
     def __init__(
         self,
         code: str = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
-        # 错误码
         self.code = code
-        # 返回数据
         self.data = data
-        # 错误提示
         self.message = message
-        # 请求唯一 ID
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7707,17 +7109,15 @@
 
 class RecognizeSocialSecurityCardVersionIIRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7744,21 +7144,17 @@
     def __init__(
         self,
         code: str = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
-        # 错误码
         self.code = code
-        # 返回数据
         self.data = data
-        # 错误提示
         self.message = message
-        # 请求唯一 ID
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7838,23 +7234,18 @@
         self,
         line_less: bool = None,
         need_rotate: bool = None,
         skip_detection: bool = None,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 是否无线条
         self.line_less = line_less
-        # 是否需要自动旋转功能，默认需要
         self.need_rotate = need_rotate
-        # 是否跳过表格识别，如果没有检测到表格，可以设置"skip_detection":true
         self.skip_detection = skip_detection
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7980,17 +7371,15 @@
 
 class RecognizeTaxClearanceCertificateRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8017,21 +7406,17 @@
     def __init__(
         self,
         code: str = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
-        # 错误码
         self.code = code
-        # 返回数据
         self.data = data
-        # 错误提示
         self.message = message
-        # 请求唯一 ID
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8108,17 +7493,15 @@
 
 class RecognizeTaxiInvoiceRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8235,23 +7618,18 @@
         self,
         need_rotate: bool = None,
         output_char_info: bool = None,
         output_table: bool = None,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 是否需要自动旋转功能(结构化检测、混贴场景、教育相关场景会自动做旋转，无需设置)，返回角度信息
         self.need_rotate = need_rotate
-        # 是否输出单字识别结果
         self.output_char_info = output_char_info
-        # 是否输出表格识别结果，包含单元格信息
         self.output_table = output_table
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8377,17 +7755,15 @@
 
 class RecognizeTollInvoiceRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8414,21 +7790,17 @@
     def __init__(
         self,
         code: str = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
-        # 错误码
         self.code = code
-        # 返回数据
         self.data = data
-        # 错误提示
         self.message = message
-        # 请求唯一 ID
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8505,17 +7877,15 @@
 
 class RecognizeTradeMarkCertificationRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8629,17 +7999,15 @@
 
 class RecognizeTrainInvoiceRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8753,17 +8121,15 @@
 
 class RecognizeTravelCardRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8790,21 +8156,17 @@
     def __init__(
         self,
         code: str = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
-        # 错误码
         self.code = code
-        # 返回数据
         self.data = data
-        # 错误提示
         self.message = message
-        # 请求唯一 ID
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8881,17 +8243,15 @@
 
 class RecognizeUsedCarInvoiceRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8918,21 +8278,17 @@
     def __init__(
         self,
         code: str = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
-        # 错误码
         self.code = code
-        # 返回数据
         self.data = data
-        # 错误提示
         self.message = message
-        # 请求唯一 ID
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9009,17 +8365,15 @@
 
 class RecognizeVehicleCertificationRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9046,21 +8400,17 @@
     def __init__(
         self,
         code: str = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
-        # 错误码
         self.code = code
-        # 返回数据
         self.data = data
-        # 错误提示
         self.message = message
-        # 请求唯一 ID
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9137,17 +8487,15 @@
 
 class RecognizeVehicleLicenseRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9261,17 +8609,15 @@
 
 class RecognizeVehicleRegistrationRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9298,21 +8644,17 @@
     def __init__(
         self,
         code: str = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
-        # 错误码
         self.code = code
-        # 返回数据
         self.data = data
-        # 错误提示
         self.message = message
-        # 请求唯一 ID
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9389,17 +8731,15 @@
 
 class RecognizeWaybillRequest(TeaModel):
     def __init__(
         self,
         url: str = None,
         body: BinaryIO = None,
     ):
-        # 图片链接（长度不超 2048，不支持 base64）
         self.url = url
-        # 图片二进制字节流，最大10MB
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `alibabacloud_ocr-api20210707-1.1.7/alibabacloud_ocr_api20210707.egg-info/PKG-INFO` & `alibabacloud_ocr-api20210707-1.1.8/alibabacloud_ocr_api20210707.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ocr-api20210707
-Version: 1.1.7
+Version: 1.1.8
 Summary: Alibaba Cloud ocr-api (20210707) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ocr-api20210707-1.1.7/setup.py` & `alibabacloud_ocr-api20210707-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ocr-api20210707.
 
-Created on 20/06/2022
+Created on 23/08/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ocr_api20210707"
 NAME = "alibabacloud_ocr-api20210707" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ocr-api (20210707) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.5, <1.0.0",
+    "alibabacloud_tea_util>=0.3.6, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
     "alibabacloud_openapi_util>=0.1.6, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

