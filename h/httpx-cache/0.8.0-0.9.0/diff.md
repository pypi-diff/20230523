# Comparing `tmp/httpx_cache-0.8.0.tar.gz` & `tmp/httpx_cache-0.9.0.tar.gz`

## Comparing `httpx_cache-0.8.0.tar` & `httpx_cache-0.9.0.tar`

### file list

```diff
@@ -1,45 +1,47 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/.flake8
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/mkdocs.yml
--rw-r--r--   0        0        0    89693 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/poetry.lock
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/poetry.toml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/.vscode/settings.json
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/docs/api.md
--rw-r--r--   0        0        0     5022 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/docs/cache_control.md
--rw-r--r--   0        0        0     9024 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/docs/guide.md
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/docs/index.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/docs/css/custom.css
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/examples/async_cache_client.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/examples/dict_cache_client.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/examples/file_cache_client.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/examples/streaming_response.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/httpx_cache/__init__.py
--rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/httpx_cache/cache_control.py
--rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/httpx_cache/client.py
--rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/httpx_cache/transport.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/httpx_cache/utils.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/httpx_cache/cache/__init__.py
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/httpx_cache/cache/base.py
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/httpx_cache/cache/file.py
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/httpx_cache/cache/memory.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/httpx_cache/serializer/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/httpx_cache/serializer/base.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/httpx_cache/serializer/common.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/tests/conftest.py
--rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/tests/test_cache_control.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/tests/test_client.py
--rw-r--r--   0        0        0    14267 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/tests/test_transport.py
--rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/tests/test_utils.py
--rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/tests/cache/test_cache_file.py
--rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/tests/cache/test_cache_memory.py
--rw-r--r--   0        0        0    26546 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/tests/serializer/test_serializer_common.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/.gitignore
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/LICENSE
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/README.md
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 httpx_cache-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/.flake8
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/mkdocs.yml
+-rw-r--r--   0        0        0    89693 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/poetry.lock
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/poetry.toml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/.vscode/settings.json
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/docs/api.md
+-rw-r--r--   0        0        0     5022 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/docs/cache_control.md
+-rw-r--r--   0        0        0    10139 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/docs/guide.md
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/docs/index.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/docs/css/custom.css
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/examples/async_cache_client.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/examples/dict_cache_client.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/examples/file_cache_client.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/examples/streaming_response.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/httpx_cache/__init__.py
+-rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/httpx_cache/cache_control.py
+-rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/httpx_cache/client.py
+-rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/httpx_cache/transport.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/httpx_cache/utils.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/httpx_cache/cache/__init__.py
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/httpx_cache/cache/base.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/httpx_cache/cache/file.py
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/httpx_cache/cache/memory.py
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/httpx_cache/cache/redis.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/httpx_cache/serializer/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/httpx_cache/serializer/base.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/httpx_cache/serializer/common.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/tests/test_cache_control.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/tests/test_client.py
+-rw-r--r--   0        0        0    14267 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/tests/test_transport.py
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/tests/test_utils.py
+-rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/tests/cache/test_cache_file.py
+-rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/tests/cache/test_cache_memory.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/tests/cache/test_cache_redis.py
+-rw-r--r--   0        0        0    26546 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/tests/serializer/test_serializer_common.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/README.md
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 httpx_cache-0.9.0/PKG-INFO
```

### Comparing `httpx_cache-0.8.0/CODE_OF_CONDUCT.md` & `httpx_cache-0.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/mkdocs.yml` & `httpx_cache-0.9.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/poetry.lock` & `httpx_cache-0.9.0/poetry.lock`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md` & `httpx_cache-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md` & `httpx_cache-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/.github/workflows/publish.yml` & `httpx_cache-0.9.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/.github/workflows/test.yml` & `httpx_cache-0.9.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/.vscode/settings.json` & `httpx_cache-0.9.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/docs/api.md` & `httpx_cache-0.9.0/docs/api.md`

 * *Files 16% similar despite different names*

```diff
@@ -32,15 +32,19 @@
     :docstring:
     :members:
 
 ::: httpx_cache.FileCache
     :docstring:
     :members:
 
-!!! **Note** FileCache only supports `httpx_cache.MsgPackSerializer` and `httpx_cache.BytesJsonSerializer` serializers.
+::: httpx_cache.cache.redis.RedisCache
+    :docstring:
+    :members:
+
+!!! **Note** FileCache and RedisCache only supports `httpx_cache.MsgPackSerializer` and `httpx_cache.BytesJsonSerializer` serializers.
 
 ## Serializer
 
 ::: httpx_cache.DictSerializer
     :docstring:
     :members:
```

### Comparing `httpx_cache-0.8.0/docs/cache_control.md` & `httpx_cache-0.9.0/docs/cache_control.md`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/docs/guide.md` & `httpx_cache-0.9.0/docs/guide.md`

 * *Files 6% similar despite different names*

```diff
@@ -164,24 +164,54 @@
 ```py
 import httpx_cache
 
 with httpx_cache.Client(cache=httpx_cache.FileCache(cache_dir="./my-custom-dir")) as client:
   response = client.get("https://httpbin.org/get")
 ```
 
+### RedisCache
+
+You need to install `redis` package to use this cache type, or install `httpx-cache[redis]` to install it automatically.
+
+```py
+import httpx_cache
+from httpx.cache.redis import RedisCache
+
+with httpx_cache.Client(cache=RedisCache(redis_url="redis://localhost:6379/0")) as client:
+  response = client.get("https://httpbin.org/get")
+```
+
+By default all cached responses are saved under the namespace `htppx_cache`.
+
+Optionally a TTL can be provided so that the cached responses expire after the given time (as a python timedelta).
+
+It can also accepts direct instances of `redis.Redis` or `redis.StrictRedis` clients.
+
+```py
+import httpx_cache
+from redis import Redis
+from httpx.cache.redis import RedisCache
+
+redis_client = Redis(host="localhost", port=6379, db=0)
+cache = RedisCache(redis=redis_client, namespace="my-custom-namespace", default_ttl=timedelta(hours=1))
+
+with httpx_cache.Client(cache=cache) as client:
+  response = client.get("https://httpbin.org/get")
+```
+
 ## Serializer Types
 
 Before caching an httpx.Response it needs to be serialized to a cacheable format supported by the used cache type (Dict/File).
 
-|     Serializer       |      DictCache     |     FileCache      |
-| -------------------- | ------------------ | ------------------ |
-| DictSerializer       | :white_check_mark: |       :x:          |
-| StringJsonSerializer | :white_check_mark: |       :x:          |
-| BytesJsonSerializer  | :white_check_mark: | :white_check_mark: |
-| MsgPackSerializer    | :white_check_mark: | :white_check_mark: |
+|     Serializer       |      DictCache     |     FileCache      |     RedisCache     |
+| -------------------- | ------------------ | ------------------ | ------------------ |
+| DictSerializer       | :white_check_mark: |       :x:          |       :x:          |
+| StringJsonSerializer | :white_check_mark: |       :x:          |       :x:          |
+| BytesJsonSerializer  | :white_check_mark: | :white_check_mark: | :white_check_mark: |
+| MsgPackSerializer    | :white_check_mark: | :white_check_mark: | :white_check_mark: |
 
 A custom serializer can be used anytime with:
 
 ```py
 import httpx_cache
 
 with httpx.Client(cache=httpx_cache.DictCache(serializer=httpx_cache.DictSerializer())) as client:
```

### Comparing `httpx_cache-0.8.0/examples/async_cache_client.py` & `httpx_cache-0.9.0/examples/async_cache_client.py`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/examples/dict_cache_client.py` & `httpx_cache-0.9.0/examples/dict_cache_client.py`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/examples/file_cache_client.py` & `httpx_cache-0.9.0/examples/file_cache_client.py`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/examples/streaming_response.py` & `httpx_cache-0.9.0/examples/streaming_response.py`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/httpx_cache/__init__.py` & `httpx_cache-0.9.0/httpx_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/httpx_cache/cache_control.py` & `httpx_cache-0.9.0/httpx_cache/cache_control.py`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/httpx_cache/client.py` & `httpx_cache-0.9.0/httpx_cache/client.py`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/httpx_cache/transport.py` & `httpx_cache-0.9.0/httpx_cache/transport.py`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/httpx_cache/utils.py` & `httpx_cache-0.9.0/httpx_cache/utils.py`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/httpx_cache/cache/base.py` & `httpx_cache-0.9.0/httpx_cache/cache/base.py`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/httpx_cache/cache/file.py` & `httpx_cache-0.9.0/httpx_cache/cache/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing as tp
 from pathlib import Path
 
 import anyio
-import fasteners
-from aiorwlock import RWLock
+from fasteners import ReaderWriterLock as RWLock
+from aiorwlock import RWLock as AsyncRWLock
 import httpx
 
 from httpx_cache.cache.base import BaseCache
 from httpx_cache.serializer.base import BaseSerializer
 from httpx_cache.serializer.common import MsgPackSerializer
 from httpx_cache.utils import get_cache_filepath
 
@@ -20,15 +20,15 @@
     Args:
         cache_dir: Optional custom cache_dir where to store cache files, defaults to
             ~/.cache/httpx-cache
         serializer: Optional serializer for the data to cache, defaults to:
             httpx_cache.MsgPackSerializer
     """
 
-    lock = fasteners.ReaderWriterLock()
+    lock = RWLock()
 
     def __init__(
         self,
         cache_dir: tp.Union[None, str, Path] = None,
         serializer: tp.Optional[BaseSerializer] = None,
     ) -> None:
         self.serializer = serializer or MsgPackSerializer()
@@ -44,28 +44,36 @@
         elif not isinstance(cache_dir, Path):
             assert isinstance(cache_dir, str)
             cache_dir = Path(cache_dir)
 
         self.cache_dir = cache_dir
         self.cache_dir.mkdir(parents=True, exist_ok=True)
 
+        self._async_lock: tp.Optional[AsyncRWLock] = None
+
+    @property
+    def async_lock(self) -> AsyncRWLock:
+        if self._async_lock is None:
+            self._async_lock = AsyncRWLock()
+        return self._async_lock
+
     def get(self, request: httpx.Request) -> tp.Optional[httpx.Response]:
         filepath = get_cache_filepath(self.cache_dir, request, extra=self._extra)
         if filepath.is_file():
             with self.lock.read_lock():
                 cached = filepath.read_bytes()
             return self.serializer.loads(request=request, cached=cached)
         return None
 
     async def aget(self, request: httpx.Request) -> tp.Optional[httpx.Response]:
         filepath = anyio.Path(
             get_cache_filepath(self.cache_dir, request, extra=self._extra)
         )
         if await filepath.is_file():
-            async with RWLock().reader:
+            async with self.async_lock.reader:
                 cached = await filepath.read_bytes()
             return self.serializer.loads(request=request, cached=cached)
         return None
 
     def set(
         self,
         *,
@@ -85,22 +93,22 @@
         response: httpx.Response,
         content: tp.Optional[bytes] = None,
     ) -> None:
         filepath = anyio.Path(
             get_cache_filepath(self.cache_dir, request, extra=self._extra)
         )
         to_cache = self.serializer.dumps(response=response, content=content)
-        async with RWLock().writer:
+        async with self.async_lock.writer:
             await filepath.write_bytes(to_cache)
 
     def delete(self, request: httpx.Request) -> None:
         filepath = get_cache_filepath(self.cache_dir, request, extra=self._extra)
         if filepath.is_file():
             with self.lock.write_lock():
                 filepath.unlink()
 
     async def adelete(self, request: httpx.Request) -> None:
         filepath = anyio.Path(
             get_cache_filepath(self.cache_dir, request, extra=self._extra)
         )
-        async with RWLock().writer:
+        async with self.async_lock.writer:
             await filepath.unlink(missing_ok=True)
```

### Comparing `httpx_cache-0.8.0/httpx_cache/cache/memory.py` & `httpx_cache-0.9.0/httpx_cache/cache/memory.py`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/httpx_cache/serializer/common.py` & `httpx_cache-0.9.0/httpx_cache/serializer/common.py`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/tests/test_cache_control.py` & `httpx_cache-0.9.0/tests/test_cache_control.py`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/tests/test_client.py` & `httpx_cache-0.9.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/tests/test_transport.py` & `httpx_cache-0.9.0/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/tests/test_utils.py` & `httpx_cache-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/tests/cache/test_cache_file.py` & `httpx_cache-0.9.0/tests/cache/test_cache_file.py`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/tests/cache/test_cache_memory.py` & `httpx_cache-0.9.0/tests/cache/test_cache_memory.py`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/tests/serializer/test_serializer_common.py` & `httpx_cache-0.9.0/tests/serializer/test_serializer_common.py`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/.gitignore` & `httpx_cache-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/LICENSE` & `httpx_cache-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/README.md` & `httpx_cache-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `httpx_cache-0.8.0/pyproject.toml` & `httpx_cache-0.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "httpx-cache"
-version = "0.8.0"
+version = "0.9.0"
 description = "Simple caching transport for httpx."
 readme = "README.md"
 requires-python = ">=3.7"
 license-files = { paths = ["LICENSE"] }
 authors = [
     { name = "Ouail Bendidi", email = "ouail.bendidi@gmail.com" },
 ]
@@ -37,20 +37,24 @@
   "anyio~=3.0",
   "msgpack~=1.0",
   "fasteners>=0.16.3,<0.18.0",
   "attrs>=21.4,<23.0",
   "aiorwlock~=1.2"
 ]
 
+[project.optional-dependencies]
+redis = ["redis~=4.5"]
+
 [project.urls]
 Homepage = "https://github.com/obendidi/httpx-cache"
 Documentation = "https://obendidi.github.io/httpx-cache/"
 
 [tool.hatch.envs.dev]
 extra-dependencies = [
+    "httpx-cache[redis]",
     # Test dependencies
     "pytest~=7.2",
     "coverage[toml]~=6.5",
     "pytest-cov~=3.0",
     "chardet~=5.0",
     "types-chardet~=5.0",
     "pytest-cases~=3.6.8",
@@ -72,14 +76,15 @@
 [tool.hatch.envs.dev.scripts]
 fmt = ["ruff --fix .", "black ."]
 lint = ["ruff .", "black --check --diff ."]
 typing = "mypy --install-types --non-interactive httpx_cache"
 test = "pytest -ra -q -vv --cov=httpx_cache --cov-report=term-missing --cov-report=xml --cov-config=pyproject.toml"
 docs-build = "mkdocs build --clean --strict"
 docs-serve = "mkdocs serve --dev-addr localhost:8000"
+docs-deploy = "mkdocs gh-deploy"
 
 [tool.ruff.isort]
 known-first-party = ["httpx_cache"]
 known-third-party = ["httpx", "attrs", "msgpack", "anyio"]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
```

### Comparing `httpx_cache-0.8.0/PKG-INFO` & `httpx_cache-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpx-cache
-Version: 0.8.0
+Version: 0.9.0
 Summary: Simple caching transport for httpx.
 Project-URL: Homepage, https://github.com/obendidi/httpx-cache
 Project-URL: Documentation, https://obendidi.github.io/httpx-cache/
 Author-email: Ouail Bendidi <ouail.bendidi@gmail.com>
 License-File: LICENSE
 Keywords: cache,cache-control,httpx
 Classifier: Development Status :: 3 - Alpha
@@ -25,14 +25,16 @@
 Requires-Python: >=3.7
 Requires-Dist: aiorwlock~=1.2
 Requires-Dist: anyio~=3.0
 Requires-Dist: attrs<23.0,>=21.4
 Requires-Dist: fasteners<0.18.0,>=0.16.3
 Requires-Dist: httpx~=0.23
 Requires-Dist: msgpack~=1.0
+Provides-Extra: redis
+Requires-Dist: redis~=4.5; extra == 'redis'
 Description-Content-Type: text/markdown
 
 # HTTPX-CACHE
 
 [![codecov](https://codecov.io/gh/obendidi/httpx-cache/branch/main/graph/badge.svg?token=FHHRA6F17X)](https://codecov.io/gh/obendidi/httpx-cache)
 
 httpx-cache is an implementation of the caching algorithms in [httplib2](https://github.com/httplib2/httplib2) and [CacheControl](https://github.com/ionrock/cachecontrol) for use with [httpx](https://github.com/encode/httpx) transport object.
```

