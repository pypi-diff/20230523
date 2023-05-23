# Comparing `tmp/gcloud_rest_storage-8.2.0.tar.gz` & `tmp/gcloud_rest_storage-8.2.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcloud_rest_storage-8.2.0.tar", max compression
+gzip compressed data, was "gcloud_rest_storage-8.2.1a0.tar", max compression
```

## Comparing `gcloud_rest_storage-8.2.0.tar` & `gcloud_rest_storage-8.2.1a0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-04-05 17:59:58.000000 gcloud_rest_storage-8.2.0/LICENSE
--rw-r--r--   0        0        0     1293 2023-04-05 17:59:58.000000 gcloud_rest_storage-8.2.0/README.rst
--rw-r--r--   0        0        0      212 2023-04-05 17:59:59.000000 gcloud_rest_storage-8.2.0/gcloud/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 17:59:58.000000 gcloud_rest_storage-8.2.0/gcloud/py.typed
--rw-r--r--   0        0        0      216 2023-04-05 17:59:59.000000 gcloud_rest_storage-8.2.0/gcloud/rest/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 17:59:58.000000 gcloud_rest_storage-8.2.0/gcloud/rest/py.typed
--rw-r--r--   0        0        0     5485 2023-04-05 17:59:59.000000 gcloud_rest_storage-8.2.0/gcloud/rest/storage/__init__.py
--rw-r--r--   0        0        0     7369 2023-04-05 17:59:59.000000 gcloud_rest_storage-8.2.0/gcloud/rest/storage/blob.py
--rw-r--r--   0        0        0     2741 2023-04-05 17:59:59.000000 gcloud_rest_storage-8.2.0/gcloud/rest/storage/bucket.py
--rw-r--r--   0        0        0       70 2023-04-05 17:59:59.000000 gcloud_rest_storage-8.2.0/gcloud/rest/storage/constants.py
--rw-r--r--   0        0        0        0 2023-04-05 17:59:58.000000 gcloud_rest_storage-8.2.0/gcloud/rest/storage/py.typed
--rw-r--r--   0        0        0    27214 2023-04-05 17:59:59.000000 gcloud_rest_storage-8.2.0/gcloud/rest/storage/storage.py
--rw-r--r--   0        0        0     1109 2023-04-05 17:59:58.000000 gcloud_rest_storage-8.2.0/pyproject.toml
--rw-r--r--   0        0        0     2360 1970-01-01 00:00:00.000000 gcloud_rest_storage-8.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-23 15:41:29.000000 gcloud_rest_storage-8.2.1a0/LICENSE
+-rw-r--r--   0        0        0     1293 2023-05-23 15:41:29.000000 gcloud_rest_storage-8.2.1a0/README.rst
+-rw-r--r--   0        0        0      212 2023-05-23 15:41:30.000000 gcloud_rest_storage-8.2.1a0/gcloud/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 15:41:29.000000 gcloud_rest_storage-8.2.1a0/gcloud/py.typed
+-rw-r--r--   0        0        0      216 2023-05-23 15:41:30.000000 gcloud_rest_storage-8.2.1a0/gcloud/rest/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 15:41:29.000000 gcloud_rest_storage-8.2.1a0/gcloud/rest/py.typed
+-rw-r--r--   0        0        0     5485 2023-05-23 15:41:30.000000 gcloud_rest_storage-8.2.1a0/gcloud/rest/storage/__init__.py
+-rw-r--r--   0        0        0     7369 2023-05-23 15:41:30.000000 gcloud_rest_storage-8.2.1a0/gcloud/rest/storage/blob.py
+-rw-r--r--   0        0        0     2741 2023-05-23 15:41:30.000000 gcloud_rest_storage-8.2.1a0/gcloud/rest/storage/bucket.py
+-rw-r--r--   0        0        0       70 2023-05-23 15:41:30.000000 gcloud_rest_storage-8.2.1a0/gcloud/rest/storage/constants.py
+-rw-r--r--   0        0        0        0 2023-05-23 15:41:29.000000 gcloud_rest_storage-8.2.1a0/gcloud/rest/storage/py.typed
+-rw-r--r--   0        0        0    28388 2023-05-23 15:41:30.000000 gcloud_rest_storage-8.2.1a0/gcloud/rest/storage/storage.py
+-rw-r--r--   0        0        0     1111 2023-05-23 15:41:29.000000 gcloud_rest_storage-8.2.1a0/pyproject.toml
+-rw-r--r--   0        0        0     2362 1970-01-01 00:00:00.000000 gcloud_rest_storage-8.2.1a0/PKG-INFO
```

### Comparing `gcloud_rest_storage-8.2.0/LICENSE` & `gcloud_rest_storage-8.2.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `gcloud_rest_storage-8.2.0/README.rst` & `gcloud_rest_storage-8.2.1a0/README.rst`

 * *Files identical despite different names*

### Comparing `gcloud_rest_storage-8.2.0/gcloud/rest/storage/__init__.py` & `gcloud_rest_storage-8.2.1a0/gcloud/rest/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `gcloud_rest_storage-8.2.0/gcloud/rest/storage/blob.py` & `gcloud_rest_storage-8.2.1a0/gcloud/rest/storage/blob.py`

 * *Files identical despite different names*

### Comparing `gcloud_rest_storage-8.2.0/gcloud/rest/storage/bucket.py` & `gcloud_rest_storage-8.2.1a0/gcloud/rest/storage/bucket.py`

 * *Files identical despite different names*

### Comparing `gcloud_rest_storage-8.2.0/gcloud/rest/storage/storage.py` & `gcloud_rest_storage-8.2.1a0/gcloud/rest/storage/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,14 +168,46 @@
             return {}
 
         token = self.token.get()
         return {
             'Authorization': f'Bearer {token}',
         }
 
+    # This method makes the following API call:
+    # https://cloud.google.com/storage/docs/json_api/v1/buckets/list
+    def list_buckets(
+        self, project: str, *,
+        params: Optional[Dict[str, str]] = None,
+        headers: Optional[Dict[str, Any]] = None,
+        session: Optional[Session] = None,
+        timeout: int = DEFAULT_TIMEOUT,
+    ) -> List[Bucket]:
+        url = f'{self._api_root_read}?project={project}'
+        headers = headers or {}
+        headers.update(self._headers())
+        params = params or {}
+        if not params.get('pageToken'):
+            params['pageToken'] = ''
+        s = SyncSession(session) if session else self.session
+        buckets = []
+
+        while True:
+            resp = s.get(url, headers=headers,
+                               params=params or {},
+                               timeout=timeout)
+
+            content: Dict[str, Any] = resp.json()
+            for item in content.get('items', []):
+                buckets.append(Bucket(self, item['id']))
+
+            params['pageToken'] = content.get('nextPageToken', '')
+            if not params['pageToken']:
+                break
+        return buckets
+
     def get_bucket(self, bucket_name: str) -> Bucket:
         return Bucket(self, bucket_name)
 
     def copy(
         self, bucket: str, object_name: str,
         destination_bucket: str, *, new_name: Optional[str] = None,
         metadata: Optional[Dict[str, Any]] = None,
```

### Comparing `gcloud_rest_storage-8.2.0/pyproject.toml` & `gcloud_rest_storage-8.2.1a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gcloud-rest-storage"
-version = "8.2.0"
+version = "8.2.1a0"
 description = "Python Client for Google Cloud Storage"
 readme = "README.rst"
 
 repository = "https://github.com/talkiq/gcloud-aio"
 authors = ["Vi Engineering <voiceai-eng@dialpad.com>"]
 license = "MIT"
```

### Comparing `gcloud_rest_storage-8.2.0/PKG-INFO` & `gcloud_rest_storage-8.2.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcloud-rest-storage
-Version: 8.2.0
+Version: 8.2.1a0
 Summary: Python Client for Google Cloud Storage
 Home-page: https://github.com/talkiq/gcloud-aio
 License: MIT
 Author: Vi Engineering
 Author-email: voiceai-eng@dialpad.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

