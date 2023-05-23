# Comparing `tmp/redis_simple_orm-2.0.1.tar.gz` & `tmp/redis_simple_orm-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_simple_orm-2.0.1.tar", last modified: Wed May 17 09:06:11 2023, max compression
+gzip compressed data, was "redis_simple_orm-2.1.0.tar", last modified: Tue May 23 07:28:35 2023, max compression
```

## Comparing `redis_simple_orm-2.0.1.tar` & `redis_simple_orm-2.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:06:11.536223 redis_simple_orm-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-17 09:06:11.536223 redis_simple_orm-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10511 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:06:11.532223 redis_simple_orm-2.0.1/RSO/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/RSO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:06:11.536223 redis_simple_orm-2.0.1/RSO/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/RSO/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/RSO/asyncio/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/RSO/asyncio/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/RSO/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/RSO/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/RSO/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:06:11.536223 redis_simple_orm-2.0.1/RSO/txredisapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/RSO/txredisapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/RSO/txredisapi/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/RSO/txredisapi/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:06:11.536223 redis_simple_orm-2.0.1/redis_simple_orm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-17 09:06:11.000000 redis_simple_orm-2.0.1/redis_simple_orm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-17 09:06:11.000000 redis_simple_orm-2.0.1/redis_simple_orm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:06:11.000000 redis_simple_orm-2.0.1/redis_simple_orm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-17 09:06:11.000000 redis_simple_orm-2.0.1/redis_simple_orm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-17 09:06:11.000000 redis_simple_orm-2.0.1/redis_simple_orm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-17 09:06:11.536223 redis_simple_orm-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:06:11.536223 redis_simple_orm-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/tests/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:28:35.650308 redis_simple_orm-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-23 07:28:35.650308 redis_simple_orm-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10511 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:28:35.650308 redis_simple_orm-2.1.0/RSO/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/RSO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:28:35.650308 redis_simple_orm-2.1.0/RSO/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/RSO/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/RSO/asyncio/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/RSO/asyncio/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/RSO/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/RSO/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/RSO/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:28:35.650308 redis_simple_orm-2.1.0/RSO/txredisapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/RSO/txredisapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/RSO/txredisapi/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/RSO/txredisapi/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:28:35.650308 redis_simple_orm-2.1.0/redis_simple_orm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-23 07:28:35.000000 redis_simple_orm-2.1.0/redis_simple_orm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-23 07:28:35.000000 redis_simple_orm-2.1.0/redis_simple_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:28:35.000000 redis_simple_orm-2.1.0/redis_simple_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-23 07:28:35.000000 redis_simple_orm-2.1.0/redis_simple_orm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-23 07:28:35.000000 redis_simple_orm-2.1.0/redis_simple_orm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-23 07:28:35.650308 redis_simple_orm-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:28:35.650308 redis_simple_orm-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/tests/test_model.py
```

### Comparing `redis_simple_orm-2.0.1/LICENSE` & `redis_simple_orm-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.0.1/PKG-INFO` & `redis_simple_orm-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis_simple_orm
-Version: 2.0.1
+Version: 2.1.0
 Summary: Simple Redis ORM (Sync and Async).
 Home-page: https://github.com/jockerz/redis_simple_orm
 Author: Jockerz
 Author-email: jockerz@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `redis_simple_orm-2.0.1/README.md` & `redis_simple_orm-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.0.1/RSO/asyncio/index.py` & `redis_simple_orm-2.1.0/RSO/asyncio/index.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,90 +1,102 @@
 from typing import Any, Optional, TypeVar, Union
 
-from aioredis.client import Redis, Pipeline
 from redis.asyncio.client import Redis as Redis2, Pipeline as Pipeline2
+try:
+    from aioredis.client import Redis, Pipeline
+except ImportError:
+    T_PIPE = Pipeline2
+    T_REDIS = Redis2
+    T_REDIS_PIPE = Union[Redis2, Pipeline2]
+    PIPE_CLS = (Pipeline2,)
+else:
+    T_PIPE = [Pipeline, Pipeline2]
+    T_REDIS = Union[Redis, Redis2]
+    T_REDIS_PIPE = Union[Redis, Redis2, Pipeline, Pipeline2]
+    PIPE_CLS = (Pipeline, Pipeline2)
+
 from RSO.base import BaseModel, BaseHashIndex, BaseListIndex, BaseSetIndex
 
 T = TypeVar('T')
 
 
 class HashIndex(BaseHashIndex):
     @classmethod
     async def save(
-        cls, redis: Union[Pipeline, Pipeline2], model_obj: T
+        cls, redis: T_PIPE, model_obj: T
     ) -> None:
         index_value = getattr(model_obj, cls.__key__)
         redis.hset(cls.redis_key(), mapping={
             index_value: cls.model_key_value(model_obj)
         })
 
     @classmethod
     async def remove(
-        cls, redis: Union[Pipeline, Pipeline2], model_obj: T
+        cls, redis: T_PIPE, model_obj: T
     ) -> None:
         redis.hdel(cls.redis_key(), cls.index_key_value(model_obj))
 
     @classmethod
-    async def search_model(cls, redis: Union[Redis, Redis2], index_value):
+    async def search_model(cls, redis: T_REDIS, index_value):
         redis_key = cls.redis_key()
         if not bool(await redis.exists(redis_key)):
             return
 
         model_key_value = await redis.hmget(redis_key, index_value)
         if model_key_value and isinstance(model_key_value, list):
             model_key_value = model_key_value[0]
         return await cls.__model__.search(redis, model_key_value)
 
 
 class ListIndex(BaseListIndex):
     @classmethod
     async def save(
-        cls, redis: Union[Pipeline, Pipeline2], model_obj: T
+        cls, redis: T_PIPE, model_obj: T
     ) -> None:
         redis.lpush(cls.redis_key(model_obj), cls.model_key_value(model_obj))
 
     @classmethod
     async def remove(
-        cls, redis: Union[Pipeline, Pipeline2], model_obj: T, count: int = 1
+        cls, redis: T_PIPE, model_obj: T, count: int = 1
     ):
         """count = 0 to remove all"""
         redis.lrem(
             cls.redis_key(model_obj),
             count,
             cls.model_key_value(model_obj)
         )
 
     @classmethod
-    async def get_members(cls, redis: Redis, index_value):
+    async def get_members(cls, redis: T_REDIS, index_value):
         redis_key = cls.redis_key_from_value(index_value)
         return await redis.lrange(redis_key, 0, -1)
 
     @classmethod
-    async def search_models(cls, redis: Redis, index_value):
+    async def search_models(cls, redis: T_REDIS, index_value):
         redis_key = cls.redis_key_from_value(index_value)
         if not bool(await redis.exists(redis_key)):
             return []
 
         model_instances = []
         for value in (await redis.lrange(redis_key, 0, -1)):
             model_instance = await cls.__model__.search(redis, value)
             model_instances.append(model_instance)
         return model_instances
 
     @classmethod
-    async def has_member(cls, redis: [Redis, Redis2], model_obj: T) -> bool:
+    async def has_member(cls, redis: T_REDIS, model_obj: T) -> bool:
         return await cls.has_member_value(
             redis,
             getattr(model_obj, cls.__key__),
             getattr(model_obj, model_obj.__key__)
         )
 
     @classmethod
     async def has_member_value(
-        cls, redis: [Redis, Redis2], index_value: Any, model_value: Any
+        cls, redis: T_REDIS, index_value: Any, model_value: Any
     ) -> bool:
         if hasattr(redis, 'lpos'):
             result = await redis.lpos(
                 cls.redis_key_from_value(index_value),
                 model_value
             )
         else:
@@ -93,46 +105,46 @@
                 cls.redis_key_from_value(index_value),
                 model_value
             )
         return result is not None
 
     @classmethod
     async def get_by_rpoplpush(
-        cls, redis: [Redis, Redis2], index_value: Any,
+        cls, redis: T_REDIS, index_value: Any,
     ) -> Optional[BaseModel]:
         redis_key = cls.redis_key_from_value(index_value)
         if bool(await redis.exists(redis_key)) is False:
             return
         else:
             model_value = await redis.rpoplpush(redis_key, redis_key)
             return await cls.__model__.search(redis, model_value)
 
 
 class SetIndex(BaseSetIndex):
     @classmethod
-    async def save(cls, redis: [Pipeline, Pipeline2], model_obj: T) -> None:
+    async def save(cls, redis: T_PIPE, model_obj: T) -> None:
         redis.sadd(
             cls.redis_key(model_obj),
             cls.model_key_value(model_obj)
         )
 
     @classmethod
-    async def remove(cls, redis: [Pipeline, Pipeline2], model_obj: T) -> None:
+    async def remove(cls, redis: T_PIPE, model_obj: T) -> None:
         redis.srem(
             cls.redis_key(model_obj),
             cls.model_key_value(model_obj)
         )
 
     @classmethod
-    async def get_members(cls, redis: Redis, index_value):
+    async def get_members(cls, redis: T_REDIS, index_value):
         redis_key = cls.redis_key_from_value(index_value)
         return await redis.smembers(redis_key)
 
     @classmethod
-    async def search_models(cls, redis: Redis, index_value):
+    async def search_models(cls, redis: T_REDIS, index_value):
         redis_key = cls.redis_key_from_value(index_value)
         if not bool(await redis.exists(redis_key)):
             return []
 
         model_instances = []
         for value in (await redis.smembers(redis_key)):
             model_instance = await cls.__model__.search(redis, value)
```

### Comparing `redis_simple_orm-2.0.1/RSO/asyncio/model.py` & `redis_simple_orm-2.1.0/RSO/model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,78 +1,75 @@
 from typing import List, Optional, Union
 
-from aioredis.client import Redis, Pipeline
-from redis.asyncio.client import Redis as Redis2, Pipeline as Pipeline2
+from redis.client import Pipeline, Redis
 
 from RSO.base import BaseModel
 
 
 class Model(BaseModel):
-    async def is_exists(self, redis: Union[Redis, Redis2]):
-        return bool(await redis.exists(self.redis_key))
+    def is_exists(self, redis: Redis):
+        return bool(redis.exists(self.redis_key))
 
-    async def save(self, redis: Union[Pipeline, Pipeline2, Redis, Redis2]):
-        if isinstance(redis, (Pipeline, Pipeline2)):
+    def save(self, redis: Union[Pipeline, Redis]):
+        if isinstance(redis, Pipeline):
             pipe = redis
         else:
             pipe = redis.pipeline()
 
         pipe.hset(self.redis_key, mapping=self.to_redis())
-
-        for index_class in self.__indexes__:
-            if getattr(self, index_class.__key__, None) is None:
+        for index_class in self.__indexes__ or []:
+            if getattr(self, index_class.__key__) is None:
                 continue
-            await index_class.save(pipe, self)
+            index_class.save(pipe, self)
 
-        if not isinstance(redis, (Pipeline, Pipeline2)):
-            await pipe.execute()
+        if not isinstance(redis, Pipeline):
+            pipe.execute()
 
     @classmethod
-    async def search(cls, redis: Redis, value) -> Optional['Model']:
+    def search(cls, redis: Redis, value) -> Optional['Model']:
         redis_key = cls.redis_key_from_value(value)
-        if bool(await redis.exists(redis_key)) is True:
+        if bool(redis.exists(redis_key)):
             fields = cls.get_fields()
-            redis_data = await redis.hmget(redis_key, fields)
+            redis_data = redis.hmget(redis_key, fields)
             dict_data = cls.from_redis(dict(zip(fields, redis_data)))
             return cls(**dict_data)
         else:
             return None
 
     @classmethod
-    async def all(cls, redis: [Redis, Redis2]) -> List['Model']:
+    def all(cls, redis: Redis) -> List['Model']:
         redis_key = cls.redis_key_from_value('*')
-        members = await redis.keys(redis_key)
+        members = redis.keys(redis_key)
         indexes = []
         for index_class in cls.__indexes__:
             indexes.append(
                 f'::{index_class.__index_name__}::{index_class.__key__}'
             )
-        async with redis.pipeline(transaction=True) as pipe:
+        with redis.pipeline(transaction=True) as pipe:
             for member in members:
                 is_index = False
                 for index in indexes:
                     if index in member:
                         is_index = True
                         break
                 if not is_index:
                     pipe.hgetall(member)
-            result_data = await pipe.execute()
+            result_data = pipe.execute()
 
         result = []
         for data in result_data:
             result.append(cls(**data))
         return result
 
-
-    async def delete(self, redis: [Pipeline, Pipeline2, Redis, Redis2]) -> None:
-        if isinstance(redis, (Pipeline, Pipeline2)):
+    def delete(self, redis: Union[Pipeline, Redis]):
+        if isinstance(redis, Pipeline):
             pipe = redis
         else:
             pipe = redis.pipeline()
 
         for index_class in self.__indexes__:
             if getattr(self, index_class.__key__) is not None:
-                await index_class.remove(pipe, self)
+                index_class.remove(pipe, self)
 
         pipe.delete(self.redis_key)
-        if not isinstance(redis, (Pipeline, Pipeline2)):
-            await pipe.execute()
+        if not isinstance(redis, Pipeline):
+            pipe.execute()
```

### Comparing `redis_simple_orm-2.0.1/RSO/base.py` & `redis_simple_orm-2.1.0/RSO/base.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.0.1/RSO/index.py` & `redis_simple_orm-2.1.0/RSO/index.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.0.1/RSO/model.py` & `redis_simple_orm-2.1.0/RSO/txredisapi/model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,75 +1,86 @@
 from typing import List, Optional, Union
 
-from redis.client import Pipeline, Redis
+from txredisapi import BaseRedisProtocol, ConnectionHandler
+from twisted.internet.defer import inlineCallbacks
 
 from RSO.base import BaseModel
 
 
 class Model(BaseModel):
-    def is_exists(self, redis: Redis):
-        return bool(redis.exists(self.redis_key))
-
-    def save(self, redis: Union[Pipeline, Redis]):
-        if isinstance(redis, Pipeline):
-            pipe = redis
+    @inlineCallbacks
+    def is_exist(self, redis: ConnectionHandler):
+        result = yield redis.exists(self.redis_key)
+        return bool(result)
+
+    @inlineCallbacks
+    def save(self, redis: Union[BaseRedisProtocol, ConnectionHandler]):
+        if isinstance(redis, ConnectionHandler):
+            pipe = yield redis.multi()
+            do_commit = True
         else:
-            pipe = redis.pipeline()
+            pipe = redis
+            do_commit = False
 
-        pipe.hset(self.redis_key, mapping=self.to_redis())
+        pipe.hmset(self.redis_key, self.to_redis())
         for index_class in self.__indexes__ or []:
-            if getattr(self, index_class.__key__) is None:
+            if getattr(self, index_class.__key__, None) is None:
                 continue
-            index_class.save(pipe, self)
-
-        if not isinstance(redis, Pipeline):
-            pipe.execute()
+            yield index_class.save(pipe, self)
+        if do_commit:
+            yield pipe.commit()
 
     @classmethod
-    def search(cls, redis: Redis, value) -> Optional['Model']:
+    @inlineCallbacks
+    def search(cls, redis: ConnectionHandler, value) -> Optional['Model']:
         redis_key = cls.redis_key_from_value(value)
-        if bool(redis.exists(redis_key)):
+        result = yield redis.exists(redis_key)
+        if bool(result):
             fields = cls.get_fields()
-            redis_data = redis.hmget(redis_key, fields)
+            redis_data = yield redis.hmget(redis_key, fields)
             dict_data = cls.from_redis(dict(zip(fields, redis_data)))
             return cls(**dict_data)
-        else:
-            return None
+        return
 
     @classmethod
-    def all(cls, redis: Redis) -> List['Model']:
+    @inlineCallbacks
+    def all(cls, redis: ConnectionHandler) -> List['Model']:
         redis_key = cls.redis_key_from_value('*')
-        members = redis.keys(redis_key)
+        members = yield redis.keys(redis_key)
         indexes = []
         for index_class in cls.__indexes__:
             indexes.append(
                 f'::{index_class.__index_name__}::{index_class.__key__}'
             )
-        with redis.pipeline(transaction=True) as pipe:
-            for member in members:
-                is_index = False
-                for index in indexes:
-                    if index in member:
-                        is_index = True
-                        break
-                if not is_index:
-                    pipe.hgetall(member)
-            result_data = pipe.execute()
+
+        pipe = yield redis.multi()
+        for member in members:
+            is_index = False
+            for index in indexes:
+                if index in member:
+                    is_index = True
+                    break
+            if not is_index:
+                yield pipe.hgetall(member)
+        result_data = yield pipe.commit()
 
         result = []
         for data in result_data:
             result.append(cls(**data))
         return result
 
-    def delete(self, redis: Union[Pipeline, Redis]):
-        if isinstance(redis, Pipeline):
-            pipe = redis
+    @inlineCallbacks
+    def delete(self, redis: Union[BaseRedisProtocol, ConnectionHandler]):
+        if isinstance(redis, ConnectionHandler):
+            pipe = yield redis.multi()
+            do_commit = True
         else:
-            pipe = redis.pipeline()
+            pipe = redis
+            do_commit = False
 
-        for index_class in self.__indexes__:
-            if getattr(self, index_class.__key__) is not None:
-                index_class.remove(pipe, self)
-
-        pipe.delete(self.redis_key)
-        if not isinstance(redis, Pipeline):
-            pipe.execute()
+        for index_class in self.__indexes__ or []:
+            if getattr(self, index_class.__key__) is None:
+                continue
+            index_class.remove(pipe, self)
+        yield pipe.delete(self.redis_key)
+        if do_commit:
+            yield pipe.commit()
```

### Comparing `redis_simple_orm-2.0.1/RSO/txredisapi/index.py` & `redis_simple_orm-2.1.0/RSO/txredisapi/index.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.0.1/redis_simple_orm.egg-info/PKG-INFO` & `redis_simple_orm-2.1.0/redis_simple_orm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-simple-orm
-Version: 2.0.1
+Version: 2.1.0
 Summary: Simple Redis ORM (Sync and Async).
 Home-page: https://github.com/jockerz/redis_simple_orm
 Author: Jockerz
 Author-email: jockerz@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `redis_simple_orm-2.0.1/setup.py` & `redis_simple_orm-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     data_files=[("", ["LICENSE"])],
     install_requires=[
         'aiocontextvars;python_version<"3.7"',
     ],
     extras_require={
         "redis-py": ["redis"],
         "aioredis": ["aioredis"],
-        "txredisapi": ["txredisapi"],
+        "txredisapi": ["pyopenssl", "txredisapi"],
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `redis_simple_orm-2.0.1/tests/test_example.py` & `redis_simple_orm-2.1.0/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.0.1/tests/test_index.py` & `redis_simple_orm-2.1.0/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.0.1/tests/test_model.py` & `redis_simple_orm-2.1.0/tests/test_model.py`

 * *Files identical despite different names*

