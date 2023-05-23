# Comparing `tmp/fast-resource-0.1.0.tar.gz` & `tmp/fast-resource-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\fast-resource-0.1.0.tar", last modified: Tue Feb  7 10:11:19 2023, max compression
+gzip compressed data, was "D:\www\fast_resource\dist\.tmp-tmn74tzo\fast-resource-0.1.1.tar", last modified: Tue May 23 06:26:26 2023, max compression
```

## Comparing `fast-resource-0.1.0.tar` & `fast-resource-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-02-07 10:11:19.389370 fast-resource-0.1.0/
--rw-rw-rw-   0        0        0    11556 2023-02-07 09:26:48.000000 fast-resource-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2761 2023-02-07 10:11:19.389370 fast-resource-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2299 2023-02-07 09:26:48.000000 fast-resource-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-07 10:11:19.358371 fast-resource-0.1.0/examples/
--rw-rw-rw-   0        0        0        0 2023-02-07 09:26:48.000000 fast-resource-0.1.0/examples/__init__.py
--rw-rw-rw-   0        0        0      646 2023-02-07 09:26:48.000000 fast-resource-0.1.0/examples/fastapi.py
--rw-rw-rw-   0        0        0      674 2023-02-07 09:26:48.000000 fast-resource-0.1.0/examples/flask.py
--rw-rw-rw-   0        0        0     1097 2023-02-07 09:26:48.000000 fast-resource-0.1.0/examples/sample.py
-drwxrwxrwx   0        0        0        0 2023-02-07 10:11:19.361370 fast-resource-0.1.0/fast_resource/
--rw-rw-rw-   0        0        0       67 2023-02-07 09:26:48.000000 fast-resource-0.1.0/fast_resource/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-07 10:11:19.381367 fast-resource-0.1.0/fast_resource/cache/
--rw-rw-rw-   0        0        0      107 2023-02-07 09:26:48.000000 fast-resource-0.1.0/fast_resource/cache/__init__.py
--rw-rw-rw-   0        0        0      560 2023-02-07 09:26:48.000000 fast-resource-0.1.0/fast_resource/cache/cache.py
--rw-rw-rw-   0        0        0      663 2023-02-07 09:26:48.000000 fast-resource-0.1.0/fast_resource/cache/memcached_cache.py
--rw-rw-rw-   0        0        0      599 2023-02-07 09:26:48.000000 fast-resource-0.1.0/fast_resource/cache/redis_cache.py
--rw-rw-rw-   0        0        0     2242 2023-02-07 09:26:48.000000 fast-resource-0.1.0/fast_resource/resource.py
--rw-rw-rw-   0        0        0     3335 2023-02-07 09:26:48.000000 fast-resource-0.1.0/fast_resource/resource_cache.py
-drwxrwxrwx   0        0        0        0 2023-02-07 10:11:19.376369 fast-resource-0.1.0/fast_resource.egg-info/
--rw-rw-rw-   0        0        0     2761 2023-02-07 10:11:19.000000 fast-resource-0.1.0/fast_resource.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2023-02-07 10:11:19.000000 fast-resource-0.1.0/fast_resource.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-07 10:11:19.000000 fast-resource-0.1.0/fast_resource.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-02-07 10:11:19.000000 fast-resource-0.1.0/fast_resource.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-02-07 10:11:19.000000 fast-resource-0.1.0/fast_resource.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-07 10:11:19.390370 fast-resource-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      726 2023-02-07 10:11:16.000000 fast-resource-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-07 10:11:19.387371 fast-resource-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2023-02-07 09:26:48.000000 fast-resource-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0      518 2023-02-07 09:26:48.000000 fast-resource-0.1.0/tests/config.py
--rw-rw-rw-   0        0        0     3071 2023-02-07 09:26:48.000000 fast-resource-0.1.0/tests/test_cache.py
--rw-rw-rw-   0        0        0      878 2023-02-07 09:26:48.000000 fast-resource-0.1.0/tests/test_resource.py
+drwxrwxrwx   0        0        0        0 2023-05-23 06:26:26.629260 fast-resource-0.1.1/
+-rw-rw-rw-   0        0        0    11556 2023-02-07 09:26:48.000000 fast-resource-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3044 2023-05-23 06:26:26.629081 fast-resource-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2539 2023-05-15 06:48:45.000000 fast-resource-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 06:26:26.597516 fast-resource-0.1.1/examples/
+-rw-rw-rw-   0        0        0        0 2023-02-07 09:26:48.000000 fast-resource-0.1.1/examples/__init__.py
+-rw-rw-rw-   0        0        0      646 2023-02-07 09:26:48.000000 fast-resource-0.1.1/examples/fastapi.py
+-rw-rw-rw-   0        0        0      674 2023-02-07 09:26:48.000000 fast-resource-0.1.1/examples/flask.py
+-rw-rw-rw-   0        0        0     1096 2023-04-26 19:58:16.000000 fast-resource-0.1.1/examples/sample.py
+drwxrwxrwx   0        0        0        0 2023-05-23 06:26:26.601704 fast-resource-0.1.1/fast_resource/
+-rw-rw-rw-   0        0        0       67 2023-02-07 09:26:48.000000 fast-resource-0.1.1/fast_resource/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 06:26:26.621790 fast-resource-0.1.1/fast_resource/cache/
+-rw-rw-rw-   0        0        0      106 2023-04-28 05:32:03.000000 fast-resource-0.1.1/fast_resource/cache/__init__.py
+-rw-rw-rw-   0        0        0      560 2023-02-07 09:26:48.000000 fast-resource-0.1.1/fast_resource/cache/cache.py
+-rw-rw-rw-   0        0        0      662 2023-04-28 05:31:07.000000 fast-resource-0.1.1/fast_resource/cache/memcached_cache.py
+-rw-rw-rw-   0        0        0      599 2023-02-07 09:26:48.000000 fast-resource-0.1.1/fast_resource/cache/redis_cache.py
+-rw-rw-rw-   0        0        0     2026 2023-04-26 20:48:02.000000 fast-resource-0.1.1/fast_resource/resource.py
+-rw-rw-rw-   0        0        0     3293 2023-04-26 20:50:31.000000 fast-resource-0.1.1/fast_resource/resource_cache.py
+drwxrwxrwx   0        0        0        0 2023-05-23 06:26:26.615758 fast-resource-0.1.1/fast_resource.egg-info/
+-rw-rw-rw-   0        0        0     3044 2023-05-23 06:26:26.000000 fast-resource-0.1.1/fast_resource.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-05-23 06:26:26.000000 fast-resource-0.1.1/fast_resource.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 06:26:26.000000 fast-resource-0.1.1/fast_resource.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-23 06:26:26.000000 fast-resource-0.1.1/fast_resource.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-05-23 06:26:26.000000 fast-resource-0.1.1/fast_resource.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 06:26:26.630044 fast-resource-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      769 2023-05-23 06:26:12.000000 fast-resource-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 06:26:26.627404 fast-resource-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-02-07 09:26:48.000000 fast-resource-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      623 2023-04-26 20:22:23.000000 fast-resource-0.1.1/tests/config.py
+-rw-rw-rw-   0        0        0     3069 2023-04-28 19:37:05.000000 fast-resource-0.1.1/tests/test_cache.py
+-rw-rw-rw-   0        0        0      878 2023-02-07 09:26:48.000000 fast-resource-0.1.1/tests/test_resource.py
```

### Comparing `fast-resource-0.1.0/LICENSE` & `fast-resource-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fast-resource-0.1.0/PKG-INFO` & `fast-resource-0.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,103 +1,89 @@
-Metadata-Version: 2.1
-Name: fast-resource
-Version: 0.1.0
-Summary: fast-resource is a data transformation layer between the database and data returned to the application's users. Also, it can cache data by using Redis and Memcached.
-Home-page: https://github.com/bagher/fast-resource
-Author: Bagher Rokni
-Author-email: bagher.rokni@gmail.com
-License: LICENSE.txt
-Requires-Python: >=3.*
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # fast-resource
-## Introduction
-`fast-resource` is a data transformation layer between the database and data returned to the application's users. Also, it can cache data by using Redis and Memcached.
+`fast-resource` is a data transformation layer that sits between the database and the application's users, enabling quick data retrieval. It further enhances performance by caching data using Redis and Memcached.
+## Why Use fast-resource?
+fast-resource is useful in situations where there are numerous data retrieval queries, multiple data sources requiring data aggregation, and shared data between entities that need to be cached. Additionally, the type of database used is not important.
 ## Requirements
 - `redis`
 - `pymemcache`
 ## Install
 ```shell
 > pip install fast-resource
 ```
 ## Usage
 
 ### Quick Start
 
 ```python
-from typing import Dict
 from fast_resource import Resource
 
 
 class UserResource(Resource):
     class Meta:
         fields = (
             'id',
             'name',
         )
 
-    def name(self, input_data: Dict) -> str:
+    def name(self, input_data) -> str:
         return f'{input_data["name"]} {input_data["family"]}'
 
 
 UserResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).to_dict()
 ```
 ### Custom output
 ```python
 UserResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).to_dict(('id',))
 ```
 ### Use cache decoder
 ```python
-from typing import Dict
 from redis.client import Redis
 from fast_resource import Resource, cache
 from fast_resource.cache import RedisCache
 
 def my_key_builder(input_data, field):
-    return f'post.{input_data["id"]}.{field}'
-
+    return f'user.{input_data["id"]}.{field}'
 
-class PostResource(Resource):
+class UserResource(Resource):
     class Meta:
         fields = (
             'id',
-            'title',
-            'comment_count',
+            'name',
         )
 
     @cache(key=my_key_builder)
-    def comment_count(self, input_data: Dict) -> str:
-        return comment.filter(id=input_data['id']).count()
+    def name(self, input_data) -> str:
+        return f'{input_data["name"]} {input_data["family"]}'
 
 
 Resource.cache_init(driver=RedisCache(Redis()))
-PostResource({'id': 1, 'title': 'Why fast-resource?'}).to_dict()
+UserResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).to_dict()
 ```
 ### Custom cache expire_time
 ```python
-    @cache(key=my_key_builder, expire_time=60)
-    def comment_count(self, input_data: Dict) -> str:
-        return comment.filter(id=input_data['id']).count()
+@cache(key=my_key_builder, expire_time=60)
+def name(self, input_data) -> str:
+    return f'{input_data["name"]} {input_data["family"]}'
 ```
 ### Cache delete
 ```python
-PostResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).cache_delete()
+UserResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).cache_delete()
 ```
 ### Cache delete & rebuild
 ```python
-PostResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).cache_delete(rebuild=True)
+UserResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).cache_delete(rebuild=True)
 ```
 
 ### Cache delete by keys
 ```python
-PostResource.cache_delete(['post.1.comment_count'])
+UserResource.cache_delete_by_keys(['user.1.name'])
 ```
 
 ### Create collection
 ```python
 user_collection = UserResource.collection([
     {'id': 1, 'name': 'bagher', 'family': 'rokni'},
-    {'id': 2, 'name': 'sepehr', 'family': 'rokni'}
+    {'id': 2, 'name': 'sepehr', 'family': 'rokni'},
+    {'id': 3, 'name': 'sama', 'family': 'rokni'},
 ])
 user_collection.to_dict()
-```
+```
```

### Comparing `fast-resource-0.1.0/README.md` & `fast-resource-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,91 +1,101 @@
+Metadata-Version: 2.1
+Name: fast-resource
+Version: 0.1.1
+Summary: fast-resource is a data transformation layer that sits between the database and the application's users, enabling quick data retrieval. It further enhances performance by caching data using Redis and Memcached.
+Home-page: https://github.com/bagher/fast-resource
+Author: Bagher Rokni
+Author-email: bagher.rokni@gmail.com
+License: LICENSE.txt
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # fast-resource
-## Introduction
-`fast-resource` is a data transformation layer between the database and data returned to the application's users. Also, it can cache data by using Redis and Memcached.
+`fast-resource` is a data transformation layer that sits between the database and the application's users, enabling quick data retrieval. It further enhances performance by caching data using Redis and Memcached.
+## Why Use fast-resource?
+fast-resource is useful in situations where there are numerous data retrieval queries, multiple data sources requiring data aggregation, and shared data between entities that need to be cached. Additionally, the type of database used is not important.
 ## Requirements
 - `redis`
 - `pymemcache`
 ## Install
 ```shell
 > pip install fast-resource
 ```
 ## Usage
 
 ### Quick Start
 
 ```python
-from typing import Dict
 from fast_resource import Resource
 
 
 class UserResource(Resource):
     class Meta:
         fields = (
             'id',
             'name',
         )
 
-    def name(self, input_data: Dict) -> str:
+    def name(self, input_data) -> str:
         return f'{input_data["name"]} {input_data["family"]}'
 
 
 UserResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).to_dict()
 ```
 ### Custom output
 ```python
 UserResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).to_dict(('id',))
 ```
 ### Use cache decoder
 ```python
-from typing import Dict
 from redis.client import Redis
 from fast_resource import Resource, cache
 from fast_resource.cache import RedisCache
 
 def my_key_builder(input_data, field):
-    return f'post.{input_data["id"]}.{field}'
-
+    return f'user.{input_data["id"]}.{field}'
 
-class PostResource(Resource):
+class UserResource(Resource):
     class Meta:
         fields = (
             'id',
-            'title',
-            'comment_count',
+            'name',
         )
 
     @cache(key=my_key_builder)
-    def comment_count(self, input_data: Dict) -> str:
-        return comment.filter(id=input_data['id']).count()
+    def name(self, input_data) -> str:
+        return f'{input_data["name"]} {input_data["family"]}'
 
 
 Resource.cache_init(driver=RedisCache(Redis()))
-PostResource({'id': 1, 'title': 'Why fast-resource?'}).to_dict()
+UserResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).to_dict()
 ```
 ### Custom cache expire_time
 ```python
-    @cache(key=my_key_builder, expire_time=60)
-    def comment_count(self, input_data: Dict) -> str:
-        return comment.filter(id=input_data['id']).count()
+@cache(key=my_key_builder, expire_time=60)
+def name(self, input_data) -> str:
+    return f'{input_data["name"]} {input_data["family"]}'
 ```
 ### Cache delete
 ```python
-PostResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).cache_delete()
+UserResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).cache_delete()
 ```
 ### Cache delete & rebuild
 ```python
-PostResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).cache_delete(rebuild=True)
+UserResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).cache_delete(rebuild=True)
 ```
 
 ### Cache delete by keys
 ```python
-PostResource.cache_delete(['post.1.comment_count'])
+UserResource.cache_delete_by_keys(['user.1.name'])
 ```
 
 ### Create collection
 ```python
 user_collection = UserResource.collection([
     {'id': 1, 'name': 'bagher', 'family': 'rokni'},
-    {'id': 2, 'name': 'sepehr', 'family': 'rokni'}
+    {'id': 2, 'name': 'sepehr', 'family': 'rokni'},
+    {'id': 3, 'name': 'sama', 'family': 'rokni'},
 ])
 user_collection.to_dict()
-```
+```
```

### Comparing `fast-resource-0.1.0/examples/fastapi.py` & `fast-resource-0.1.1/examples/fastapi.py`

 * *Files identical despite different names*

### Comparing `fast-resource-0.1.0/examples/flask.py` & `fast-resource-0.1.1/examples/flask.py`

 * *Files identical despite different names*

### Comparing `fast-resource-0.1.0/examples/sample.py` & `fast-resource-0.1.1/examples/sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,14 @@
             'user',
         )
 
     @cache(key=post_cache_key_builder)
     def comment_count(self, input_data: Dict) -> int:
         return 10
 
-    @cache(key=lambda input_data, field: f'user1.{input_data["user_id"]}')
+    @cache(key=lambda input_data, field: f'user.{input_data["user_id"]}')
     def user(self, input_data):
         return UserResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).to_dict()
 
 
 Resource.cache_init(driver=RedisCache(Redis()))
 p = PostResource({'id': 1, 'title': 'Why fast-resource?', 'user_id': 1}).to_dict()
```

### Comparing `fast-resource-0.1.0/fast_resource/cache/cache.py` & `fast-resource-0.1.1/fast_resource/cache/cache.py`

 * *Files identical despite different names*

### Comparing `fast-resource-0.1.0/fast_resource/cache/memcached_cache.py` & `fast-resource-0.1.1/fast_resource/cache/memcached_cache.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .cache import Cache
 from typing import List, Dict
 from pymemcache.client.base import Client
 
 
-class MemcachedClient(Cache):
+class MemcachedCache(Cache):
     def __init__(self, memcached: Client):
         self.memcached = memcached
 
     def get(self, keys: List) -> Dict:
         return {
             index: self.decode(value)
             for index, value in self.memcached.get_many(keys).items()
```

### Comparing `fast-resource-0.1.0/fast_resource/cache/redis_cache.py` & `fast-resource-0.1.1/fast_resource/cache/redis_cache.py`

 * *Files identical despite different names*

### Comparing `fast-resource-0.1.0/fast_resource/resource_cache.py` & `fast-resource-0.1.1/fast_resource/resource_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,17 @@
 
         return self.cache_fields_config[class_name]
 
     def get_cache_keys(self, field_name=None) -> Union[Dict, str]:
         if not self.cache_fields_alias:
             fields = self.__get_cache_fields_config()
             for index, field in fields.items():
-                key = field['key'] if isinstance(field['key'], str) else field['key'](self.input_data, index)
+                key = field.get('key')
+                if callable(key):
+                    key = key(self.input_data, index)
                 self.cache_fields_alias[index] = f'{self.cache_prefix}.{key}'
         return self.cache_fields_alias[field_name] if field_name else self.cache_fields_alias
 
     def _get_cache_data(self) -> Dict:
         return self.cache_data or {}
 
     def _cache_save(self, output_data: Dict) -> None:
@@ -65,19 +67,16 @@
                     self.cache_driver.set(
                         self.get_cache_keys(k),
                         value,
                         self.__get_cache_fields_config()[k]['expire_time']
                     )
 
     def cache_delete(self, fields: List = None, rebuild=False) -> int:
-        for_remove = []
         fields = fields or self.Meta.fields
-        for field in fields:
-            if field in self.get_cache_keys():
-                for_remove.append(self.get_cache_keys(field))
+        for_remove = [self.get_cache_keys(field) for field in fields if field in self.get_cache_keys()]
         total = self.cache_driver.delete(for_remove)
         if rebuild:
             self.cache_data = {}
             output_data = self._fetch_data(fields)
             self._cache_save(output_data)
         return total
```

### Comparing `fast-resource-0.1.0/fast_resource.egg-info/PKG-INFO` & `fast-resource-0.1.1/fast_resource.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,103 +1,101 @@
 Metadata-Version: 2.1
 Name: fast-resource
-Version: 0.1.0
-Summary: fast-resource is a data transformation layer between the database and data returned to the application's users. Also, it can cache data by using Redis and Memcached.
+Version: 0.1.1
+Summary: fast-resource is a data transformation layer that sits between the database and the application's users, enabling quick data retrieval. It further enhances performance by caching data using Redis and Memcached.
 Home-page: https://github.com/bagher/fast-resource
 Author: Bagher Rokni
 Author-email: bagher.rokni@gmail.com
 License: LICENSE.txt
-Requires-Python: >=3.*
+Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fast-resource
-## Introduction
-`fast-resource` is a data transformation layer between the database and data returned to the application's users. Also, it can cache data by using Redis and Memcached.
+`fast-resource` is a data transformation layer that sits between the database and the application's users, enabling quick data retrieval. It further enhances performance by caching data using Redis and Memcached.
+## Why Use fast-resource?
+fast-resource is useful in situations where there are numerous data retrieval queries, multiple data sources requiring data aggregation, and shared data between entities that need to be cached. Additionally, the type of database used is not important.
 ## Requirements
 - `redis`
 - `pymemcache`
 ## Install
 ```shell
 > pip install fast-resource
 ```
 ## Usage
 
 ### Quick Start
 
 ```python
-from typing import Dict
 from fast_resource import Resource
 
 
 class UserResource(Resource):
     class Meta:
         fields = (
             'id',
             'name',
         )
 
-    def name(self, input_data: Dict) -> str:
+    def name(self, input_data) -> str:
         return f'{input_data["name"]} {input_data["family"]}'
 
 
 UserResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).to_dict()
 ```
 ### Custom output
 ```python
 UserResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).to_dict(('id',))
 ```
 ### Use cache decoder
 ```python
-from typing import Dict
 from redis.client import Redis
 from fast_resource import Resource, cache
 from fast_resource.cache import RedisCache
 
 def my_key_builder(input_data, field):
-    return f'post.{input_data["id"]}.{field}'
+    return f'user.{input_data["id"]}.{field}'
 
-
-class PostResource(Resource):
+class UserResource(Resource):
     class Meta:
         fields = (
             'id',
-            'title',
-            'comment_count',
+            'name',
         )
 
     @cache(key=my_key_builder)
-    def comment_count(self, input_data: Dict) -> str:
-        return comment.filter(id=input_data['id']).count()
+    def name(self, input_data) -> str:
+        return f'{input_data["name"]} {input_data["family"]}'
 
 
 Resource.cache_init(driver=RedisCache(Redis()))
-PostResource({'id': 1, 'title': 'Why fast-resource?'}).to_dict()
+UserResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).to_dict()
 ```
 ### Custom cache expire_time
 ```python
-    @cache(key=my_key_builder, expire_time=60)
-    def comment_count(self, input_data: Dict) -> str:
-        return comment.filter(id=input_data['id']).count()
+@cache(key=my_key_builder, expire_time=60)
+def name(self, input_data) -> str:
+    return f'{input_data["name"]} {input_data["family"]}'
 ```
 ### Cache delete
 ```python
-PostResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).cache_delete()
+UserResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).cache_delete()
 ```
 ### Cache delete & rebuild
 ```python
-PostResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).cache_delete(rebuild=True)
+UserResource({'id': 1, 'name': 'bagher', 'family': 'rokni'}).cache_delete(rebuild=True)
 ```
 
 ### Cache delete by keys
 ```python
-PostResource.cache_delete(['post.1.comment_count'])
+UserResource.cache_delete_by_keys(['user.1.name'])
 ```
 
 ### Create collection
 ```python
 user_collection = UserResource.collection([
     {'id': 1, 'name': 'bagher', 'family': 'rokni'},
-    {'id': 2, 'name': 'sepehr', 'family': 'rokni'}
+    {'id': 2, 'name': 'sepehr', 'family': 'rokni'},
+    {'id': 3, 'name': 'sama', 'family': 'rokni'},
 ])
 user_collection.to_dict()
 ```
```

### Comparing `fast-resource-0.1.0/fast_resource.egg-info/SOURCES.txt` & `fast-resource-0.1.1/fast_resource.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fast-resource-0.1.0/setup.py` & `fast-resource-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fast-resource',
-    version='0.1.0',
+    version='0.1.1',
     author='Bagher Rokni',
     author_email='bagher.rokni@gmail.com',
     packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
     url='https://github.com/bagher/fast-resource',
     license='LICENSE.txt',
-    description='fast-resource is a data transformation layer between the database and data returned to the '
-                'application\'s users. Also, it can cache data by using Redis and Memcached.',
+    description='fast-resource is a data transformation layer that sits between the database and the '
+                'application\'s users, enabling quick data retrieval. It further enhances performance by caching data using Redis and Memcached.',
     long_description=open('README.md').read(),
     install_requires=['redis', 'pymemcache'],
     long_description_content_type='text/markdown',
-    python_requires='>=3.*',
+    python_requires='>=3',
 )
```

### Comparing `fast-resource-0.1.0/tests/test_cache.py` & `fast-resource-0.1.1/tests/test_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import time
 from fast_resource import Resource, cache
 import unittest
-from fast_resource.cache import RedisCache, MemcachedClient
+from fast_resource.cache import RedisCache, MemcachedCache
 from redis.client import Redis
 from .config import UserResource, inputs
 from pymemcache.client.base import Client
 
 
 class TestResourceCache(unittest.TestCase):
     def setUp(self):
-        self.cache = MemcachedClient(Client(server='127.0.0.1:11211'))
+        self.cache = MemcachedCache(Client(server='127.0.0.1:11211'))
         Resource.cache_init(driver=self.cache, prefix='resources.test')
         self.user = UserResource(inputs['bagher'])
         self.users = UserResource.collection(inputs.values())
 
     def test_resource_constructor(self):
         self.assertIsInstance(self.user, Resource)
```

### Comparing `fast-resource-0.1.0/tests/test_resource.py` & `fast-resource-0.1.1/tests/test_resource.py`

 * *Files identical despite different names*

