# Comparing `tmp/directory_cms_client-8.3.0-py3-none-any.whl.zip` & `tmp/directory_cms_client-9.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 7855 bytes, number of entries: 16
--rw-r--r--  2.0 unx       94 b- defN 19-Feb-27 12:03 directory_cms_client/__init__.py
--rw-r--r--  2.0 unx     3960 b- defN 19-Feb-27 12:03 directory_cms_client/client.py
--rw-r--r--  2.0 unx       74 b- defN 19-Feb-27 12:03 directory_cms_client/constants.py
--rw-r--r--  2.0 unx      353 b- defN 19-Feb-27 12:03 directory_cms_client/helpers.py
--rw-r--r--  2.0 unx       22 b- defN 19-Feb-27 12:03 directory_cms_client/version.py
--rw-r--r--  2.0 unx        0 b- defN 19-Feb-27 12:03 tests/__init__.py
--rw-r--r--  2.0 unx      669 b- defN 19-Feb-27 12:03 tests/conftest.py
--rw-r--r--  2.0 unx      244 b- defN 19-Feb-27 12:03 tests/helpers.py
--rw-r--r--  2.0 unx     6059 b- defN 19-Feb-27 12:03 tests/test_client.py
--rw-r--r--  2.0 unx      137 b- defN 19-Feb-27 12:03 tests/test_constants.py
--rw-r--r--  2.0 unx      963 b- defN 19-Feb-27 12:03 tests/test_helpers.py
--rw-r--r--  2.0 unx     1091 b- defN 19-Feb-27 12:04 directory_cms_client-8.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3662 b- defN 19-Feb-27 12:04 directory_cms_client-8.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 19-Feb-27 12:04 directory_cms_client-8.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       27 b- defN 19-Feb-27 12:04 directory_cms_client-8.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1335 b- defN 19-Feb-27 12:04 directory_cms_client-8.3.0.dist-info/RECORD
-16 files, 18782 bytes uncompressed, 5627 bytes compressed:  70.0%
+Zip file size: 7894 bytes, number of entries: 16
+-rw-r--r--  2.0 unx       94 b- defN 19-Apr-23 09:18 directory_cms_client/__init__.py
+-rw-r--r--  2.0 unx     3816 b- defN 19-Apr-23 09:18 directory_cms_client/client.py
+-rw-r--r--  2.0 unx       74 b- defN 19-Apr-23 09:18 directory_cms_client/constants.py
+-rw-r--r--  2.0 unx      353 b- defN 19-Apr-23 09:18 directory_cms_client/helpers.py
+-rw-r--r--  2.0 unx       22 b- defN 19-Apr-23 09:18 directory_cms_client/version.py
+-rw-r--r--  2.0 unx        0 b- defN 19-Apr-23 09:18 tests/__init__.py
+-rw-r--r--  2.0 unx      669 b- defN 19-Apr-23 09:18 tests/conftest.py
+-rw-r--r--  2.0 unx      244 b- defN 19-Apr-23 09:18 tests/helpers.py
+-rw-r--r--  2.0 unx     5832 b- defN 19-Apr-23 09:18 tests/test_client.py
+-rw-r--r--  2.0 unx      137 b- defN 19-Apr-23 09:18 tests/test_constants.py
+-rw-r--r--  2.0 unx      963 b- defN 19-Apr-23 09:18 tests/test_helpers.py
+-rw-r--r--  2.0 unx     1091 b- defN 19-Apr-23 09:19 directory_cms_client-9.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3662 b- defN 19-Apr-23 09:19 directory_cms_client-9.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 19-Apr-23 09:19 directory_cms_client-9.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       27 b- defN 19-Apr-23 09:19 directory_cms_client-9.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1335 b- defN 19-Apr-23 09:19 directory_cms_client-9.0.0.dist-info/RECORD
+16 files, 18411 bytes uncompressed, 5666 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: tests/test_constants.py
 Comment: 
 
 Filename: tests/test_helpers.py
 Comment: 
 
-Filename: directory_cms_client-8.3.0.dist-info/LICENSE
+Filename: directory_cms_client-9.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: directory_cms_client-8.3.0.dist-info/METADATA
+Filename: directory_cms_client-9.0.0.dist-info/METADATA
 Comment: 
 
-Filename: directory_cms_client-8.3.0.dist-info/WHEEL
+Filename: directory_cms_client-9.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: directory_cms_client-8.3.0.dist-info/top_level.txt
+Filename: directory_cms_client-9.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: directory_cms_client-8.3.0.dist-info/RECORD
+Filename: directory_cms_client-9.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## directory_cms_client/client.py

```diff
@@ -4,39 +4,36 @@
 from django.conf import settings
 from django.core.cache import caches
 
 from directory_cms_client.version import __version__
 
 
 def build_params(
-        full_path=None,
         language_code=None,
         draft_token=None,
         fields=None,
         region=None,
 ):
     params = {'fields': fields or ['*']}
     if language_code:
         params['lang'] = language_code
     if draft_token:
         params['draft_token'] = draft_token
-    if full_path:
-        params['full_path'] = full_path
     if region:
         params['region'] = region
     return params
 
 
 class DirectoryCMSClient(AbstractAPIClient):
     endpoints = {
         'ping': 'healthcheck/ping/',
         'page-by-type': '/api/pages/lookup-by-type/{page_type}/',
         'page-by-slug': '/api/pages/lookup-by-slug/{slug}/',
         'page-by-tag': '/api/pages/lookup-by-tag/{slug}/',
-        'page-by-full-path': '/api/pages/lookup-by-full-path/',
+        'page-by-path': '/api/pages/lookup-by-path/{site_id}/{path}',
         'pages-by-type': '/api/pages/'
     }
     version = __version__
 
     def __init__(
         self, base_url, api_key, sender_id, timeout, default_service_name,
     ):
@@ -85,32 +82,31 @@
             url=self.endpoints['page-by-slug'].format(slug=slug),
             params={
                 **base_params,
                 'service_name': service_name or self.default_service_name,
             },
         )
 
-    def lookup_by_full_path(
+    def lookup_by_path(
         self,
-        full_path,
+        site_id,
+        path,
         fields=None,
         draft_token=None,
         language_code=None,
-        service_name=None,
+        region=None,
     ):
         base_params = build_params(
-            fields=fields, language_code=language_code,
-            draft_token=draft_token, full_path=full_path)
-        return self.get(
-            url=self.endpoints['page-by-full-path'],
-            params={
-                **base_params,
-                'service_name': service_name or self.default_service_name,
-            },
+            fields=fields,
+            draft_token=draft_token,
+            language_code=language_code,
+            region=region,
         )
+        url = self.endpoints['page-by-path'].format(site_id=site_id, path=path)
+        return self.get(url=url, params=base_params)
 
     def list_by_page_type(
         self,
         page_type,
         fields=None,
         draft_token=None,
         language_code=None
```

## directory_cms_client/version.py

```diff
@@ -1 +1 @@
-__version__ = '8.3.0'
+__version__ = '9.0.0'
```

## tests/test_client.py

```diff
@@ -88,104 +88,98 @@
         assert request.qs == {
             'service_name': ['foo'],
             'region': ['eu'],
             'fields': ['*'],
         }
 
 
-def test_cms_client_lookup_by_full_path_language(default_client):
+def test_cms_client_lookup_by_tag_draft(default_client):
     with requests_mock.mock() as mock:
-        mock.get('http://example.com/api/pages/lookup-by-full-path/')
-        default_client.lookup_by_full_path('thing', language_code='de')
+        mock.get('http://example.com/api/pages/lookup-by-tag/thing/')
+        default_client.lookup_by_tag('thing', draft_token='draft-token')
         request = mock.request_history[0]
 
         assert request.qs == {
-            'lang': ['de'],
             'fields': ['*'],
-            'full_path': ['thing'],
+            'draft_token': ['draft-token'],
             'service_name': ['foo'],
         }
 
 
-def test_cms_client_lookup_by_full_path_draft(default_client):
+def test_cms_client_lookup_by_tag(default_client):
     with requests_mock.mock() as mock:
-        mock.get('http://example.com/api/pages/lookup-by-full-path/')
-        default_client.lookup_by_full_path('thing', draft_token='draft-token')
+        mock.get('http://example.com/api/pages/lookup-by-tag/thing/')
+        default_client.lookup_by_tag('thing')
         request = mock.request_history[0]
 
         assert request.qs == {
-            'draft_token': ['draft-token'],
             'fields': ['*'],
-            'full_path': ['thing'],
             'service_name': ['foo'],
         }
 
 
-def test_cms_client_lookup_by_full_path(default_client):
+def test_cms_client_lookup_by_tag_service_name(default_client):
     with requests_mock.mock() as mock:
-        mock.get('http://example.com/api/pages/lookup-by-full-path/')
-        default_client.lookup_by_full_path('thing')
+        mock.get('http://example.com/api/pages/lookup-by-tag/thing/')
+        default_client.lookup_by_tag(
+            'thing', service_name='test-service')
         request = mock.request_history[0]
 
         assert request.qs == {
             'fields': ['*'],
-            'full_path': ['thing'],
-            'service_name': ['foo'],
+            'service_name': ['test-service'],
         }
 
 
-def test_cms_client_lookup_by_full_path_service_name(default_client):
+def test_cms_client_lookup_by_path(default_client):
     with requests_mock.mock() as mock:
-        mock.get('http://example.com/api/pages/lookup-by-full-path/')
-        default_client.lookup_by_full_path(
-            'thing', service_name='test-service')
+        mock.get('http://example.com/api/pages/lookup-by-path/1/thing')
+        default_client.lookup_by_path(site_id=1, path='thing')
         request = mock.request_history[0]
 
         assert request.qs == {
             'fields': ['*'],
-            'full_path': ['thing'],
-            'service_name': ['test-service'],
         }
 
 
-def test_cms_client_lookup_by_tag_draft(default_client):
+def test_cms_client_lookup_by_path_with_language(default_client):
     with requests_mock.mock() as mock:
-        mock.get('http://example.com/api/pages/lookup-by-tag/thing/')
-        default_client.lookup_by_tag('thing', draft_token='draft-token')
+        mock.get('http://example.com/api/pages/lookup-by-path/1/thing')
+        default_client.lookup_by_path(
+            site_id=1, path='thing', language_code='de')
         request = mock.request_history[0]
 
         assert request.qs == {
+            'lang': ['de'],
             'fields': ['*'],
-            'draft_token': ['draft-token'],
-            'service_name': ['foo'],
         }
 
 
-def test_cms_client_lookup_by_tag(default_client):
+def test_cms_client_lookup_by_path_with_draft_token(default_client):
     with requests_mock.mock() as mock:
-        mock.get('http://example.com/api/pages/lookup-by-tag/thing/')
-        default_client.lookup_by_tag('thing')
+        mock.get('http://example.com/api/pages/lookup-by-path/1/thing')
+        default_client.lookup_by_path(
+            site_id=1, path='thing', draft_token='draft-token')
         request = mock.request_history[0]
 
         assert request.qs == {
+            'draft_token': ['draft-token'],
             'fields': ['*'],
-            'service_name': ['foo'],
         }
 
 
-def test_cms_client_lookup_by_tag_service_name(default_client):
+def test_cms_client_lookup_by_path_with_region(default_client):
     with requests_mock.mock() as mock:
-        mock.get('http://example.com/api/pages/lookup-by-tag/thing/')
-        default_client.lookup_by_tag(
-            'thing', service_name='test-service')
+        mock.get('http://example.com/api/pages/lookup-by-path/1/thing')
+        default_client.lookup_by_path(site_id=1, path='thing', region='eu')
         request = mock.request_history[0]
 
         assert request.qs == {
+            'region': ['eu'],
             'fields': ['*'],
-            'service_name': ['test-service'],
         }
 
 
 def test_timeout(default_client):
     assert default_client.timeout == 5
```

## Comparing `directory_cms_client-8.3.0.dist-info/LICENSE` & `directory_cms_client-9.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `directory_cms_client-8.3.0.dist-info/METADATA` & `directory_cms_client-9.0.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directory-cms-client
-Version: 8.3.0
+Version: 9.0.0
 Summary: Python API client for Directory CMS.
 Home-page: https://github.com/uktrade/directory-cms-client
 Author: Department for International Trade
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Requires-Dist: directory-client-core (<5.0.0,>=4.3.0)
```

## Comparing `directory_cms_client-8.3.0.dist-info/RECORD` & `directory_cms_client-9.0.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 directory_cms_client/__init__.py,sha256=lEFdFdZaBicbbTXlMXC8RICbGOHf2xzqzfusEsoBsDs,94
-directory_cms_client/client.py,sha256=oKhLoyCs2STu2NzeSYHoBQi2UB4FeJ0kNKyfJmWCBNk,3960
+directory_cms_client/client.py,sha256=_UTvgOqXDCCyYNtN6QUINN_0Y60LHiEDC40Ix5XOzlk,3816
 directory_cms_client/constants.py,sha256=MtsOpg1N7SyJmiuSq8gqPgeIbX7pKQo6jfd-b0jwHaU,74
 directory_cms_client/helpers.py,sha256=8KS1eLddnaYF2HXI5kqA5298dgdDzuiSL34BOA7gqSs,353
-directory_cms_client/version.py,sha256=tcfhzCNY4r5E0tEL1zPUEXmomhpImXbYq1U_BRpvuEg,22
+directory_cms_client/version.py,sha256=iClVkjpwank7OuEaFabEKHvM8y6mO5hZxGvUfg5OmmU,22
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/conftest.py,sha256=2c-DDIwgyaVmV5anZbKrsPgknO9C5NXXaUdT3KXECxg,669
 tests/helpers.py,sha256=unVRi7Suv7EhXOvyM3YKX0NanWPI2_PRFzMIVGpa6pI,244
-tests/test_client.py,sha256=MQqz-vmArPUQWXARH0mEycOHjuw2Z-k-vmMP7369jJg,6059
+tests/test_client.py,sha256=vI7h5pU3OlOPIRoYGeqSn7v_MOhaIrlNjDBSbJde2r8,5832
 tests/test_constants.py,sha256=rV3x3JY1P4kEpEwiHIh-yQyWP9iVRy8k5mKBLbZ1ewo,137
 tests/test_helpers.py,sha256=txfZG3h7CjjYmxp57wHXnJlO8-9EmY6v5fVlE2nyc-w,963
-directory_cms_client-8.3.0.dist-info/LICENSE,sha256=q4QjlbTN37umB_xq3DRmS0qvT2tMO_5_-u0WWzYcDQE,1091
-directory_cms_client-8.3.0.dist-info/METADATA,sha256=taM3YPpkiFalCOTDlCKaMKC3kRu3JqFZx17V0ds_JQ4,3662
-directory_cms_client-8.3.0.dist-info/WHEEL,sha256=U88EhGIw8Sj2_phqajeu_EAi3RAo8-C6zV3REsWbWbs,92
-directory_cms_client-8.3.0.dist-info/top_level.txt,sha256=iI6-GzmY2NkNhvhJ4u26300Vs3PsXpXuuwudFX9vm_U,27
-directory_cms_client-8.3.0.dist-info/RECORD,,
+directory_cms_client-9.0.0.dist-info/LICENSE,sha256=q4QjlbTN37umB_xq3DRmS0qvT2tMO_5_-u0WWzYcDQE,1091
+directory_cms_client-9.0.0.dist-info/METADATA,sha256=6g1dnY7yOiaMDdEst1i1PH6VgH-qDtuXbURqP2eNLE0,3662
+directory_cms_client-9.0.0.dist-info/WHEEL,sha256=U88EhGIw8Sj2_phqajeu_EAi3RAo8-C6zV3REsWbWbs,92
+directory_cms_client-9.0.0.dist-info/top_level.txt,sha256=iI6-GzmY2NkNhvhJ4u26300Vs3PsXpXuuwudFX9vm_U,27
+directory_cms_client-9.0.0.dist-info/RECORD,,
```

