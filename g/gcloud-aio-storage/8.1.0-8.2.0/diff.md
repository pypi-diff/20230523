# Comparing `tmp/gcloud_aio_storage-8.1.0.tar.gz` & `tmp/gcloud_aio_storage-8.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcloud_aio_storage-8.1.0.tar", max compression
+gzip compressed data, was "gcloud_aio_storage-8.2.0.tar", max compression
```

## Comparing `gcloud_aio_storage-8.1.0.tar` & `gcloud_aio_storage-8.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-03-21 19:11:35.023106 gcloud_aio_storage-8.1.0/LICENSE
--rw-r--r--   0        0        0     1284 2023-03-21 19:11:35.023106 gcloud_aio_storage-8.1.0/README.rst
--rw-r--r--   0        0        0      212 2023-03-21 19:11:35.023106 gcloud_aio_storage-8.1.0/gcloud/__init__.py
--rw-r--r--   0        0        0      212 2023-03-21 19:11:35.023106 gcloud_aio_storage-8.1.0/gcloud/aio/__init__.py
--rw-r--r--   0        0        0        0 2023-03-21 19:11:35.023106 gcloud_aio_storage-8.1.0/gcloud/aio/py.typed
--rw-r--r--   0        0        0     5560 2023-03-21 19:11:35.023106 gcloud_aio_storage-8.1.0/gcloud/aio/storage/__init__.py
--rw-r--r--   0        0        0     7379 2023-03-21 19:11:35.023106 gcloud_aio_storage-8.1.0/gcloud/aio/storage/blob.py
--rw-r--r--   0        0        0     2787 2023-03-21 19:11:35.023106 gcloud_aio_storage-8.1.0/gcloud/aio/storage/bucket.py
--rw-r--r--   0        0        0       70 2023-03-21 19:11:35.023106 gcloud_aio_storage-8.1.0/gcloud/aio/storage/constants.py
--rw-r--r--   0        0        0        0 2023-03-21 19:11:35.023106 gcloud_aio_storage-8.1.0/gcloud/aio/storage/py.typed
--rw-r--r--   0        0        0    27844 2023-03-21 19:11:35.023106 gcloud_aio_storage-8.1.0/gcloud/aio/storage/storage.py
--rw-r--r--   0        0        0        0 2023-03-21 19:11:35.023106 gcloud_aio_storage-8.1.0/gcloud/py.typed
--rw-r--r--   0        0        0     1100 2023-03-21 19:11:35.023106 gcloud_aio_storage-8.1.0/pyproject.toml
--rw-r--r--   0        0        0     2391 1970-01-01 00:00:00.000000 gcloud_aio_storage-8.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-05 18:05:04.809676 gcloud_aio_storage-8.2.0/LICENSE
+-rw-r--r--   0        0        0     1284 2023-04-05 18:05:04.813675 gcloud_aio_storage-8.2.0/README.rst
+-rw-r--r--   0        0        0      212 2023-04-05 18:05:04.813675 gcloud_aio_storage-8.2.0/gcloud/__init__.py
+-rw-r--r--   0        0        0      212 2023-04-05 18:05:04.813675 gcloud_aio_storage-8.2.0/gcloud/aio/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-05 18:05:04.813675 gcloud_aio_storage-8.2.0/gcloud/aio/py.typed
+-rw-r--r--   0        0        0     5560 2023-04-05 18:05:04.813675 gcloud_aio_storage-8.2.0/gcloud/aio/storage/__init__.py
+-rw-r--r--   0        0        0     7396 2023-04-05 18:05:04.813675 gcloud_aio_storage-8.2.0/gcloud/aio/storage/blob.py
+-rw-r--r--   0        0        0     2787 2023-04-05 18:05:04.813675 gcloud_aio_storage-8.2.0/gcloud/aio/storage/bucket.py
+-rw-r--r--   0        0        0       70 2023-04-05 18:05:04.813675 gcloud_aio_storage-8.2.0/gcloud/aio/storage/constants.py
+-rw-r--r--   0        0        0        0 2023-04-05 18:05:04.813675 gcloud_aio_storage-8.2.0/gcloud/aio/storage/py.typed
+-rw-r--r--   0        0        0    27794 2023-04-05 18:05:04.813675 gcloud_aio_storage-8.2.0/gcloud/aio/storage/storage.py
+-rw-r--r--   0        0        0        0 2023-04-05 18:05:04.813675 gcloud_aio_storage-8.2.0/gcloud/py.typed
+-rw-r--r--   0        0        0     1100 2023-04-05 18:05:04.813675 gcloud_aio_storage-8.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2391 1970-01-01 00:00:00.000000 gcloud_aio_storage-8.2.0/PKG-INFO
```

### Comparing `gcloud_aio_storage-8.1.0/LICENSE` & `gcloud_aio_storage-8.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gcloud_aio_storage-8.1.0/README.rst` & `gcloud_aio_storage-8.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `gcloud_aio_storage-8.1.0/gcloud/aio/storage/__init__.py` & `gcloud_aio_storage-8.2.0/gcloud/aio/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `gcloud_aio_storage-8.1.0/gcloud/aio/storage/blob.py` & `gcloud_aio_storage-8.2.0/gcloud/aio/storage/blob.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         if expiration > 604800:
             raise ValueError(
                 "expiration time can't be longer than 604800 "
                 'seconds (7 days)',
             )
 
         quoted_name = quote(self.name, safe=b'/~')
-        canonical_uri = f'/{quoted_name}'
+        canonical_uri = f'/{self.bucket.name}/{quoted_name}'
 
         datetime_now = datetime.datetime.utcnow()
         request_timestamp = datetime_now.strftime('%Y%m%dT%H%M%SZ')
         datestamp = datetime_now.strftime('%Y%m%d')
 
         # TODO: support for GCE_METADATA and AUTHORIZED_USER tokens. It should
         # be possible via API, but seems to not be working for us in some
@@ -144,17 +144,18 @@
                 'account file',
             )
 
         credential_scope = f'{datestamp}/auto/storage/goog4_request'
         credential = f'{client_email}/{credential_scope}'
 
         headers = headers or {}
-        headers['host'] = f'{self.bucket.name}.{HOST}'
+        headers['host'] = HOST
 
-        ordered_headers = collections.OrderedDict(sorted(headers.items()))
+        ordered_headers = collections.OrderedDict(
+            sorted(headers.items(), key=lambda x: x[0].lower()))
         canonical_headers = ''.join(
             f'{str(k).lower()}:{str(v).lower()}\n'
             for k, v in ordered_headers.items()
         )
 
         signed_headers = ';'.join(
             f'{str(k).lower()}' for k in ordered_headers.keys()
@@ -212,10 +213,10 @@
 
         key = rsa.key.PrivateKey.load_pkcs1(key_bytes, format='DER')
         signed_blob = rsa.pkcs1.sign(str_to_sign.encode(), key, 'SHA-256')
 
         signature = binascii.hexlify(signed_blob).decode()
 
         return (
-            f'https://{self.bucket.name}.{HOST}{canonical_uri}?'
+            f'https://{HOST}{canonical_uri}?'
             f'{canonical_query_str}&X-Goog-Signature={signature}'
         )
```

### Comparing `gcloud_aio_storage-8.1.0/gcloud/aio/storage/bucket.py` & `gcloud_aio_storage-8.2.0/gcloud/aio/storage/bucket.py`

 * *Files identical despite different names*

### Comparing `gcloud_aio_storage-8.1.0/gcloud/aio/storage/storage.py` & `gcloud_aio_storage-8.2.0/gcloud/aio/storage/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,38 +69,38 @@
 
     Very heavily modified to be compatible with our gcloud-rest converter and
     to avoid unnecessary urllib3 dependencies (since that's only included with
     requests, not aiohttp).
     """
     body: List[bytes] = []
     for headers, data in fields:
-        body.append(f'--{boundary}\r\n'.encode('utf-8'))
+        body.append(f'--{boundary}\r\n'.encode())
 
         # The below is from RequestFields.render_headers()
         # Since we only use Content-Type, we could simplify the below to a
         # single line... but probably best to be safe for future modifications.
         for field in [
             'Content-Disposition', 'Content-Type',
             'Content-Location',
         ]:
             value = headers.pop(field, None)
             if value:
-                body.append(f'{field}: {value}\r\n'.encode('utf-8'))
+                body.append(f'{field}: {value}\r\n'.encode())
         for field, value in headers.items():
             # N.B. potential bug copied from urllib3 code; zero values should
             # be sent! Keeping it for now, since Google libs use urllib3 for
             # their examples.
             if value:
-                body.append(f'{field}: {value}\r\n'.encode('utf-8'))
+                body.append(f'{field}: {value}\r\n'.encode())
 
         body.append(b'\r\n')
         body.append(data)
         body.append(b'\r\n')
 
-    body.append(f'--{boundary}--\r\n'.encode('utf-8'))
+    body.append(f'--{boundary}--\r\n'.encode())
 
     # N.B. 'multipart/form-data' in upstream, but Google wants 'related'
     content_type = f'multipart/related; boundary={boundary}'
 
     return b''.join(body), content_type
 
 
@@ -171,25 +171,23 @@
         return {
             'Authorization': f'Bearer {token}',
         }
 
     def get_bucket(self, bucket_name: str) -> Bucket:
         return Bucket(self, bucket_name)
 
-    # pylint: disable=too-many-locals
     async def copy(
         self, bucket: str, object_name: str,
         destination_bucket: str, *, new_name: Optional[str] = None,
         metadata: Optional[Dict[str, Any]] = None,
         params: Optional[Dict[str, str]] = None,
         headers: Optional[Dict[str, str]] = None,
         timeout: int = DEFAULT_TIMEOUT,
-        session: Optional[Session] = None
+        session: Optional[Session] = None,
     ) -> Dict[str, Any]:
-
         """
         When files are too large, multiple calls to `rewriteTo` are made. We
         refer to the same copy job by using the `rewriteToken` from the
         previous return payload in subsequent `rewriteTo` calls.
 
         Using the `rewriteTo` GCS API is preferred in part because it is able
         to make multiple calls to fully copy an object whereas the `copyTo` GCS
@@ -198,14 +196,15 @@
 
         In the rare case you need to resume a copy operation, include the
         `rewriteToken` in the `params` dictionary. Once you begin a multi-part
         copy operation, you then have 1 week to complete the copy job.
 
         https://cloud.google.com/storage/docs/json_api/v1/objects/rewrite
         """
+        # pylint: disable=too-many-locals
         if not new_name:
             new_name = object_name
 
         url = (
             f'{self._api_root_read}/{bucket}/o/'
             f'{quote(object_name, safe="")}/rewriteTo/b/'
             f'{destination_bucket}/o/{quote(new_name, safe="")}'
@@ -256,15 +255,15 @@
         return data
 
     async def delete(
         self, bucket: str, object_name: str, *,
         timeout: int = DEFAULT_TIMEOUT,
         params: Optional[Dict[str, str]] = None,
         headers: Optional[Dict[str, str]] = None,
-        session: Optional[Session] = None
+        session: Optional[Session] = None,
     ) -> str:
         # https://cloud.google.com/storage/docs/request-endpoints#encoding
         encoded_object_name = quote(object_name, safe='')
         url = f'{self._api_root_read}/{bucket}/o/{encoded_object_name}'
         headers = headers or {}
         headers.update(await self._headers())
 
@@ -281,52 +280,52 @@
 
         return data
 
     async def download(
         self, bucket: str, object_name: str, *,
         headers: Optional[Dict[str, Any]] = None,
         timeout: int = DEFAULT_TIMEOUT,
-        session: Optional[Session] = None
+        session: Optional[Session] = None,
     ) -> bytes:
         return await self._download(
             bucket, object_name, headers=headers,
             timeout=timeout, params={'alt': 'media'},
             session=session,
         )
 
     async def download_to_filename(
         self, bucket: str, object_name: str,
-        filename: str, **kwargs: Any
+        filename: str, **kwargs: Any,
     ) -> None:
         async with file_open(  # type: ignore[attr-defined]
                 filename,
                 mode='wb+',
         ) as file_object:
             await file_object.write(
                 await self.download(bucket, object_name, **kwargs),
             )
 
     async def download_metadata(
         self, bucket: str, object_name: str, *,
         headers: Optional[Dict[str, Any]] = None,
         session: Optional[Session] = None,
-        timeout: int = DEFAULT_TIMEOUT
+        timeout: int = DEFAULT_TIMEOUT,
     ) -> Dict[str, Any]:
         data = await self._download(
             bucket, object_name, headers=headers,
             timeout=timeout, session=session,
         )
         metadata: Dict[str, Any] = json.loads(data.decode())
         return metadata
 
     async def download_stream(
         self, bucket: str, object_name: str, *,
         headers: Optional[Dict[str, Any]] = None,
         timeout: int = DEFAULT_TIMEOUT,
-        session: Optional[Session] = None
+        session: Optional[Session] = None,
     ) -> StreamResponse:
         """Download a GCS object in a buffered stream.
 
         Args:
             bucket (str): The bucket from which to download.
             object_name (str): The object within the bucket to download.
             headers (Optional[Dict[str, Any]], optional): Custom header values
@@ -349,15 +348,15 @@
         )
 
     async def list_objects(
         self, bucket: str, *,
         params: Optional[Dict[str, str]] = None,
         headers: Optional[Dict[str, Any]] = None,
         session: Optional[Session] = None,
-        timeout: int = DEFAULT_TIMEOUT
+        timeout: int = DEFAULT_TIMEOUT,
     ) -> Dict[str, Any]:
         url = f'{self._api_root_read}/{bucket}/o'
         headers = headers or {}
         headers.update(await self._headers())
 
         s = AioSession(session) if session else self.session
         resp = await s.get(
@@ -373,15 +372,15 @@
         self, bucket: str, object_name: str, file_data: Any,
         *, content_type: Optional[str] = None,
         parameters: Optional[Dict[str, str]] = None,
         headers: Optional[Dict[str, str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         session: Optional[Session] = None,
         force_resumable_upload: Optional[bool] = None,
-        timeout: int = 30
+        timeout: int = 30,
     ) -> Dict[str, Any]:
         url = f'{self._api_root_write}/{bucket}/o'
 
         stream = self._preprocess_data(file_data)
 
         if BUILD_GCLOUD_REST and isinstance(stream, io.StringIO):
             # HACK: `requests` library does not accept `str` as `data` in `put`
@@ -425,25 +424,22 @@
             )
 
         raise TypeError(f'upload type {upload_type} not supported')
 
     async def upload_from_filename(
         self, bucket: str, object_name: str,
         filename: str,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> Dict[str, Any]:
         async with file_open(  # type: ignore[attr-defined]
                 filename,
                 mode='rb',
         ) as file_object:
             contents = await file_object.read()
-            return await self.upload(
-                bucket, object_name, contents,
-                **kwargs
-            )
+            return await self.upload(bucket, object_name, contents, **kwargs)
 
     @staticmethod
     def _get_stream_len(stream: IO[AnyStr]) -> int:
         current = stream.tell()
         try:
             return stream.seek(0, os.SEEK_END)
         finally:
@@ -506,15 +502,15 @@
         return ''.join(parts)
 
     async def _download(
         self, bucket: str, object_name: str, *,
         params: Optional[Dict[str, str]] = None,
         headers: Optional[Dict[str, str]] = None,
         timeout: int = DEFAULT_TIMEOUT,
-        session: Optional[Session] = None
+        session: Optional[Session] = None,
     ) -> bytes:
         # https://cloud.google.com/storage/docs/request-endpoints#encoding
         encoded_object_name = quote(object_name, safe='')
         url = f'{self._api_root_read}/{bucket}/o/{encoded_object_name}'
         headers = headers or {}
         headers.update(await self._headers())
 
@@ -535,15 +531,15 @@
         return data
 
     async def _download_stream(
         self, bucket: str, object_name: str, *,
         params: Optional[Dict[str, str]] = None,
         headers: Optional[Dict[str, str]] = None,
         timeout: int = DEFAULT_TIMEOUT,
-        session: Optional[Session] = None
+        session: Optional[Session] = None,
     ) -> StreamResponse:
         # https://cloud.google.com/storage/docs/request-endpoints#encoding
         encoded_object_name = quote(object_name, safe='')
         url = f'{self._api_root_read}/{bucket}/o/{encoded_object_name}'
         headers = headers or {}
         headers.update(await self._headers())
 
@@ -566,15 +562,15 @@
         )
 
     async def _upload_simple(
         self, url: str, object_name: str,
         stream: IO[AnyStr], params: Dict[str, str],
         headers: Dict[str, str], *,
         session: Optional[Session] = None,
-        timeout: int = 30
+        timeout: int = 30,
     ) -> Dict[str, Any]:
         # https://cloud.google.com/storage/docs/json_api/v1/how-tos/simple-upload
         params['name'] = object_name
         params['uploadType'] = 'media'
 
         s = AioSession(session) if session else self.session
         resp = await s.post(
@@ -586,15 +582,15 @@
 
     async def _upload_multipart(
         self, url: str, object_name: str,
         stream: IO[AnyStr], params: Dict[str, str],
         headers: Dict[str, str],
         metadata: Dict[str, Any], *,
         session: Optional[Session] = None,
-        timeout: int = 30
+        timeout: int = 30,
     ) -> Dict[str, Any]:
         # https://cloud.google.com/storage/docs/json_api/v1/how-tos/multipart-upload
         params['uploadType'] = 'multipart'
 
         metadata_headers = {'Content-Type': 'application/json; charset=UTF-8'}
         metadata = {
             self._format_metadata_key(k): v
@@ -641,15 +637,15 @@
 
     async def _upload_resumable(
         self, url: str, object_name: str,
         stream: IO[AnyStr], params: Dict[str, str],
         headers: Dict[str, str], *,
         metadata: Optional[Dict[str, Any]] = None,
         session: Optional[Session] = None,
-        timeout: int = 30
+        timeout: int = 30,
     ) -> Dict[str, Any]:
         # https://cloud.google.com/storage/docs/json_api/v1/how-tos/resumable-upload
         session_uri = await self._initiate_upload(
             url, object_name, params,
             headers, metadata=metadata,
             session=session,
         )
@@ -659,15 +655,15 @@
         )
 
     async def _initiate_upload(
         self, url: str, object_name: str,
         params: Dict[str, str], headers: Dict[str, str],
         *, metadata: Optional[Dict[str, Any]] = None,
         timeout: int = DEFAULT_TIMEOUT,
-        session: Optional[Session] = None
+        session: Optional[Session] = None,
     ) -> str:
         params['uploadType'] = 'resumable'
 
         metadict = (metadata or {}).copy()
         metadict = {
             self._format_metadata_key(k): v
             for k, v in metadict.items()
@@ -697,22 +693,22 @@
         session_uri: str = resp.headers['Location']
         return session_uri
 
     async def _do_upload(
         self, session_uri: str, stream: IO[AnyStr],
         headers: Dict[str, str], *, retries: int = 5,
         session: Optional[Session] = None,
-        timeout: int = 30
+        timeout: int = 30,
     ) -> Dict[str, Any]:
         s = AioSession(session) if session else self.session
 
         original_close = stream.close
         original_position = stream.tell()
         # Prevent the stream being closed if put operation fails
-        stream.close = lambda: None  # type: ignore[assignment]
+        stream.close = lambda: None  # type: ignore[method-assign]
         try:
             for tries in range(retries):
                 try:
                     resp = await s.put(
                         session_uri, headers=headers,
                         data=stream, timeout=timeout,
                     )
@@ -732,15 +728,15 @@
         return data
 
     async def patch_metadata(
             self, bucket: str, object_name: str, metadata: Dict[str, Any],
             *, params: Optional[Dict[str, str]] = None,
             headers: Optional[Dict[str, str]] = None,
             session: Optional[Session] = None,
-            timeout: int = DEFAULT_TIMEOUT
+            timeout: int = DEFAULT_TIMEOUT,
     ) -> Dict[str, Any]:
         # https://cloud.google.com/storage/docs/json_api/v1/objects/patch
         encoded_object_name = quote(object_name, safe='')
         url = f'{self._api_root_read}/{bucket}/o/{encoded_object_name}'
         params = params or {}
         headers = headers or {}
         headers.update(await self._headers())
@@ -756,15 +752,15 @@
         return data
 
     async def get_bucket_metadata(
         self, bucket: str, *,
         params: Optional[Dict[str, str]] = None,
         headers: Optional[Dict[str, str]] = None,
         session: Optional[Session] = None,
-        timeout: int = DEFAULT_TIMEOUT
+        timeout: int = DEFAULT_TIMEOUT,
     ) -> Dict[str, Any]:
         url = f'{self._api_root_read}/{bucket}'
         headers = headers or {}
         headers.update(await self._headers())
 
         s = AioSession(session) if session else self.session
         resp = await s.get(
```

### Comparing `gcloud_aio_storage-8.1.0/pyproject.toml` & `gcloud_aio_storage-8.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gcloud-aio-storage"
-version = "8.1.0"
+version = "8.2.0"
 description = "Python Client for Google Cloud Storage"
 readme = "README.rst"
 
 repository = "https://github.com/talkiq/gcloud-aio"
 authors = ["Vi Engineering <voiceai-eng@dialpad.com>"]
 license = "MIT"
 
@@ -17,24 +17,24 @@
     'Intended Audience :: Developers',
     'Operating System :: OS Independent',
     'Topic :: Internet',
 ]
 
 [tool.poetry.dependencies]
 python = ">= 3.7, < 4.0"
-aiofiles = ">= 0.6.0, < 23.0.0"
+aiofiles = ">= 0.6.0, < 24.0.0"
 gcloud-aio-auth = ">= 3.6.0, < 5.0.0"
 pyasn1-modules = ">= 0.2.1, < 0.3.0"
 rsa = ">= 3.1.4, < 5.0.0"
 setuptools = ">= 66.0.0, < 67.0.0"  # TODO: upgrade to PEP 420 namespace packages
 
 [tool.poetry.dev-dependencies]
 gcloud-aio-auth = { path = "../auth" }
 pytest = ">= 4.0.0, < 8.0.0"
-pytest-asyncio = ">= 0.16.0, < 0.21.0"
+pytest-asyncio = ">= 0.16.0, < 0.22.0"
 pytest-mock = ">= 2.0.0, < 4.0.0"
 
 [tool.pytest.ini_options]
 # addopts = "-Werror"  # TODO: fixme
 asyncio_mode = "auto"
 
 [build-system]
```

### Comparing `gcloud_aio_storage-8.1.0/PKG-INFO` & `gcloud_aio_storage-8.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcloud-aio-storage
-Version: 8.1.0
+Version: 8.2.0
 Summary: Python Client for Google Cloud Storage
 Home-page: https://github.com/talkiq/gcloud-aio
 License: MIT
 Author: Vi Engineering
 Author-email: voiceai-eng@dialpad.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
-Requires-Dist: aiofiles (>=0.6.0,<23.0.0)
+Requires-Dist: aiofiles (>=0.6.0,<24.0.0)
 Requires-Dist: gcloud-aio-auth (>=3.6.0,<5.0.0)
 Requires-Dist: pyasn1-modules (>=0.2.1,<0.3.0)
 Requires-Dist: rsa (>=3.1.4,<5.0.0)
 Requires-Dist: setuptools (>=66.0.0,<67.0.0)
 Project-URL: Repository, https://github.com/talkiq/gcloud-aio
 Description-Content-Type: text/x-rst
```

