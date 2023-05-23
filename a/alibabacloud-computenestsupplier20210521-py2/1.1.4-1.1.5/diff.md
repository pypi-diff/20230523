# Comparing `tmp/alibabacloud_computenestsupplier20210521_py2-1.1.4.tar.gz` & `tmp/alibabacloud_computenestsupplier20210521_py2-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_computenestsupplier20210521_py2-1.1.4.tar", last modified: Tue May 16 10:12:04 2023, max compression
+gzip compressed data, was "dist/alibabacloud_computenestsupplier20210521_py2-1.1.5.tar", last modified: Tue May 23 05:35:08 2023, max compression
```

## Comparing `alibabacloud_computenestsupplier20210521_py2-1.1.4.tar` & `alibabacloud_computenestsupplier20210521_py2-1.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:12:04.000000 alibabacloud_computenestsupplier20210521_py2-1.1.4/
--rw-r--r--   0 root         (0) root         (0)      313 2023-05-16 10:12:04.000000 alibabacloud_computenestsupplier20210521_py2-1.1.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-05-16 10:12:04.000000 alibabacloud_computenestsupplier20210521_py2-1.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-05-16 10:12:04.000000 alibabacloud_computenestsupplier20210521_py2-1.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2568 2023-05-16 10:12:04.000000 alibabacloud_computenestsupplier20210521_py2-1.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1081 2023-05-16 10:12:04.000000 alibabacloud_computenestsupplier20210521_py2-1.1.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1164 2023-05-16 10:12:04.000000 alibabacloud_computenestsupplier20210521_py2-1.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:12:04.000000 alibabacloud_computenestsupplier20210521_py2-1.1.4/alibabacloud_computenestsupplier20210521/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 10:12:04.000000 alibabacloud_computenestsupplier20210521_py2-1.1.4/alibabacloud_computenestsupplier20210521/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28594 2023-05-16 10:12:04.000000 alibabacloud_computenestsupplier20210521_py2-1.1.4/alibabacloud_computenestsupplier20210521/client.py
--rw-r--r--   0 root         (0) root         (0)   188472 2023-05-16 10:12:04.000000 alibabacloud_computenestsupplier20210521_py2-1.1.4/alibabacloud_computenestsupplier20210521/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:12:04.000000 alibabacloud_computenestsupplier20210521_py2-1.1.4/alibabacloud_computenestsupplier20210521_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2568 2023-05-16 10:12:04.000000 alibabacloud_computenestsupplier20210521_py2-1.1.4/alibabacloud_computenestsupplier20210521_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      568 2023-05-16 10:12:04.000000 alibabacloud_computenestsupplier20210521_py2-1.1.4/alibabacloud_computenestsupplier20210521_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 10:12:04.000000 alibabacloud_computenestsupplier20210521_py2-1.1.4/alibabacloud_computenestsupplier20210521_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-05-16 10:12:04.000000 alibabacloud_computenestsupplier20210521_py2-1.1.4/alibabacloud_computenestsupplier20210521_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-05-16 10:12:04.000000 alibabacloud_computenestsupplier20210521_py2-1.1.4/alibabacloud_computenestsupplier20210521_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 10:12:04.000000 alibabacloud_computenestsupplier20210521_py2-1.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2983 2023-05-16 10:12:04.000000 alibabacloud_computenestsupplier20210521_py2-1.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:35:08.000000 alibabacloud_computenestsupplier20210521_py2-1.1.5/
+-rw-r--r--   0 root         (0) root         (0)      386 2023-05-23 05:35:08.000000 alibabacloud_computenestsupplier20210521_py2-1.1.5/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-23 05:35:08.000000 alibabacloud_computenestsupplier20210521_py2-1.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-23 05:35:08.000000 alibabacloud_computenestsupplier20210521_py2-1.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2568 2023-05-23 05:35:08.000000 alibabacloud_computenestsupplier20210521_py2-1.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-05-23 05:35:08.000000 alibabacloud_computenestsupplier20210521_py2-1.1.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1164 2023-05-23 05:35:08.000000 alibabacloud_computenestsupplier20210521_py2-1.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:35:08.000000 alibabacloud_computenestsupplier20210521_py2-1.1.5/alibabacloud_computenestsupplier20210521/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-23 05:35:08.000000 alibabacloud_computenestsupplier20210521_py2-1.1.5/alibabacloud_computenestsupplier20210521/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29726 2023-05-23 05:35:08.000000 alibabacloud_computenestsupplier20210521_py2-1.1.5/alibabacloud_computenestsupplier20210521/client.py
+-rw-r--r--   0 root         (0) root         (0)   194923 2023-05-23 05:35:08.000000 alibabacloud_computenestsupplier20210521_py2-1.1.5/alibabacloud_computenestsupplier20210521/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:35:08.000000 alibabacloud_computenestsupplier20210521_py2-1.1.5/alibabacloud_computenestsupplier20210521_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2568 2023-05-23 05:35:08.000000 alibabacloud_computenestsupplier20210521_py2-1.1.5/alibabacloud_computenestsupplier20210521_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      568 2023-05-23 05:35:08.000000 alibabacloud_computenestsupplier20210521_py2-1.1.5/alibabacloud_computenestsupplier20210521_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 05:35:08.000000 alibabacloud_computenestsupplier20210521_py2-1.1.5/alibabacloud_computenestsupplier20210521_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-23 05:35:08.000000 alibabacloud_computenestsupplier20210521_py2-1.1.5/alibabacloud_computenestsupplier20210521_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-23 05:35:08.000000 alibabacloud_computenestsupplier20210521_py2-1.1.5/alibabacloud_computenestsupplier20210521_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-23 05:35:08.000000 alibabacloud_computenestsupplier20210521_py2-1.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2983 2023-05-23 05:35:08.000000 alibabacloud_computenestsupplier20210521_py2-1.1.5/setup.py
```

### Comparing `alibabacloud_computenestsupplier20210521_py2-1.1.4/LICENSE` & `alibabacloud_computenestsupplier20210521_py2-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_computenestsupplier20210521_py2-1.1.4/PKG-INFO` & `alibabacloud_computenestsupplier20210521_py2-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_computenestsupplier20210521_py2
-Version: 1.1.4
+Version: 1.1.5
 Summary: Alibaba Cloud ComputeNestSupplier (20210521) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_computenestsupplier20210521_py2-1.1.4/README-CN.md` & `alibabacloud_computenestsupplier20210521_py2-1.1.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_computenestsupplier20210521_py2-1.1.4/README.md` & `alibabacloud_computenestsupplier20210521_py2-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_computenestsupplier20210521_py2-1.1.4/alibabacloud_computenestsupplier20210521/client.py` & `alibabacloud_computenestsupplier20210521_py2-1.1.5/alibabacloud_computenestsupplier20210521/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,14 +207,16 @@
         return self.delete_service_with_options(request, runtime)
 
     def get_artifact_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.artifact_id):
             query['ArtifactId'] = request.artifact_id
+        if not UtilClient.is_unset(request.artifact_name):
+            query['ArtifactName'] = request.artifact_name
         if not UtilClient.is_unset(request.artifact_version):
             query['ArtifactVersion'] = request.artifact_version
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetArtifact',
@@ -368,14 +370,42 @@
             self.call_api(params, req, runtime)
         )
 
     def get_service_instance(self, request):
         runtime = util_models.RuntimeOptions()
         return self.get_service_instance_with_options(request, runtime)
 
+    def get_upload_credentials_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.file_name):
+            query['FileName'] = request.file_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetUploadCredentials',
+            version='2021-05-21',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            compute_nest_supplier_20210521_models.GetUploadCredentialsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def get_upload_credentials(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.get_upload_credentials_with_options(request, runtime)
+
     def list_artifact_versions_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.artifact_id):
             query['ArtifactId'] = request.artifact_id
         if not UtilClient.is_unset(request.max_result):
             query['MaxResult'] = request.max_result
```

### Comparing `alibabacloud_computenestsupplier20210521_py2-1.1.4/alibabacloud_computenestsupplier20210521/models.py` & `alibabacloud_computenestsupplier20210521_py2-1.1.5/alibabacloud_computenestsupplier20210521/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -772,37 +772,42 @@
         if m.get('body') is not None:
             temp_model = DeleteServiceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetArtifactRequest(TeaModel):
-    def __init__(self, artifact_id=None, artifact_version=None):
+    def __init__(self, artifact_id=None, artifact_name=None, artifact_version=None):
         self.artifact_id = artifact_id  # type: str
+        self.artifact_name = artifact_name  # type: str
         self.artifact_version = artifact_version  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetArtifactRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.artifact_id is not None:
             result['ArtifactId'] = self.artifact_id
+        if self.artifact_name is not None:
+            result['ArtifactName'] = self.artifact_name
         if self.artifact_version is not None:
             result['ArtifactVersion'] = self.artifact_version
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ArtifactId') is not None:
             self.artifact_id = m.get('ArtifactId')
+        if m.get('ArtifactName') is not None:
+            self.artifact_name = m.get('ArtifactName')
         if m.get('ArtifactVersion') is not None:
             self.artifact_version = m.get('ArtifactVersion')
         return self
 
 
 class GetArtifactResponseBody(TeaModel):
     def __init__(self, artifact_id=None, artifact_property=None, artifact_type=None, artifact_version=None,
@@ -2386,14 +2391,183 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetServiceInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetUploadCredentialsRequest(TeaModel):
+    def __init__(self, file_name=None):
+        self.file_name = file_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetUploadCredentialsRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.file_name is not None:
+            result['FileName'] = self.file_name
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('FileName') is not None:
+            self.file_name = m.get('FileName')
+        return self
+
+
+class GetUploadCredentialsResponseBodyData(TeaModel):
+    def __init__(self, access_key_id=None, access_key_secret=None, bucket_name=None, expire_date=None, key=None,
+                 region_id=None, security_token=None):
+        self.access_key_id = access_key_id  # type: str
+        self.access_key_secret = access_key_secret  # type: str
+        self.bucket_name = bucket_name  # type: str
+        self.expire_date = expire_date  # type: str
+        self.key = key  # type: str
+        self.region_id = region_id  # type: str
+        self.security_token = security_token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetUploadCredentialsResponseBodyData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_key_id is not None:
+            result['AccessKeyId'] = self.access_key_id
+        if self.access_key_secret is not None:
+            result['AccessKeySecret'] = self.access_key_secret
+        if self.bucket_name is not None:
+            result['BucketName'] = self.bucket_name
+        if self.expire_date is not None:
+            result['ExpireDate'] = self.expire_date
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AccessKeyId') is not None:
+            self.access_key_id = m.get('AccessKeyId')
+        if m.get('AccessKeySecret') is not None:
+            self.access_key_secret = m.get('AccessKeySecret')
+        if m.get('BucketName') is not None:
+            self.bucket_name = m.get('BucketName')
+        if m.get('ExpireDate') is not None:
+            self.expire_date = m.get('ExpireDate')
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        return self
+
+
+class GetUploadCredentialsResponseBody(TeaModel):
+    def __init__(self, code=None, data=None, http_status_code=None, message=None, request_id=None, success=None):
+        self.code = code  # type: str
+        self.data = data  # type: GetUploadCredentialsResponseBodyData
+        self.http_status_code = http_status_code  # type: int
+        self.message = message  # type: str
+        self.request_id = request_id  # type: str
+        self.success = success  # type: bool
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(GetUploadCredentialsResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.http_status_code is not None:
+            result['HttpStatusCode'] = self.http_status_code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = GetUploadCredentialsResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('HttpStatusCode') is not None:
+            self.http_status_code = m.get('HttpStatusCode')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetUploadCredentialsResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetUploadCredentialsResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetUploadCredentialsResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetUploadCredentialsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListArtifactVersionsRequest(TeaModel):
     def __init__(self, artifact_id=None, max_result=None, next_token=None):
         self.artifact_id = artifact_id  # type: str
         self.max_result = max_result  # type: str
         self.next_token = next_token  # type: str
 
     def validate(self):
```

### Comparing `alibabacloud_computenestsupplier20210521_py2-1.1.4/alibabacloud_computenestsupplier20210521_py2.egg-info/PKG-INFO` & `alibabacloud_computenestsupplier20210521_py2-1.1.5/alibabacloud_computenestsupplier20210521_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-computenestsupplier20210521-py2
-Version: 1.1.4
+Version: 1.1.5
 Summary: Alibaba Cloud ComputeNestSupplier (20210521) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_computenestsupplier20210521_py2-1.1.4/alibabacloud_computenestsupplier20210521_py2.egg-info/SOURCES.txt` & `alibabacloud_computenestsupplier20210521_py2-1.1.5/alibabacloud_computenestsupplier20210521_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_computenestsupplier20210521_py2-1.1.4/setup.py` & `alibabacloud_computenestsupplier20210521_py2-1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_computenestsupplier20210521_py2.
 
-Created on 16/05/2023
+Created on 23/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_computenestsupplier20210521"
 NAME = "alibabacloud_computenestsupplier20210521_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ComputeNestSupplier (20210521) SDK Library for Python2"
```

