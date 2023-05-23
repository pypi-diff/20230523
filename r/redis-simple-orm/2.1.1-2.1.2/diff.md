# Comparing `tmp/redis_simple_orm-2.1.1.tar.gz` & `tmp/redis_simple_orm-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_simple_orm-2.1.1.tar", last modified: Tue May 23 07:34:54 2023, max compression
+gzip compressed data, was "redis_simple_orm-2.1.2.tar", last modified: Tue May 23 08:35:51 2023, max compression
```

## Comparing `redis_simple_orm-2.1.1.tar` & `redis_simple_orm-2.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:54.164361 redis_simple_orm-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-23 07:34:54.164361 redis_simple_orm-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10511 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:54.164361 redis_simple_orm-2.1.1/RSO/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/RSO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:54.164361 redis_simple_orm-2.1.1/RSO/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/RSO/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/RSO/asyncio/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/RSO/asyncio/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/RSO/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/RSO/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/RSO/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:54.164361 redis_simple_orm-2.1.1/RSO/txredisapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/RSO/txredisapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/RSO/txredisapi/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/RSO/txredisapi/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:54.164361 redis_simple_orm-2.1.1/redis_simple_orm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-23 07:34:54.000000 redis_simple_orm-2.1.1/redis_simple_orm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-23 07:34:54.000000 redis_simple_orm-2.1.1/redis_simple_orm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:34:54.000000 redis_simple_orm-2.1.1/redis_simple_orm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-23 07:34:54.000000 redis_simple_orm-2.1.1/redis_simple_orm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-23 07:34:54.000000 redis_simple_orm-2.1.1/redis_simple_orm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-23 07:34:54.164361 redis_simple_orm-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:54.164361 redis_simple_orm-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/tests/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:35:51.970314 redis_simple_orm-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-23 08:35:37.000000 redis_simple_orm-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 08:35:37.000000 redis_simple_orm-2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-23 08:35:51.970314 redis_simple_orm-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10511 2023-05-23 08:35:37.000000 redis_simple_orm-2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:35:51.970314 redis_simple_orm-2.1.2/RSO/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 08:35:37.000000 redis_simple_orm-2.1.2/RSO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:35:51.970314 redis_simple_orm-2.1.2/RSO/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 08:35:37.000000 redis_simple_orm-2.1.2/RSO/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-23 08:35:37.000000 redis_simple_orm-2.1.2/RSO/asyncio/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-23 08:35:37.000000 redis_simple_orm-2.1.2/RSO/asyncio/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-23 08:35:37.000000 redis_simple_orm-2.1.2/RSO/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-23 08:35:37.000000 redis_simple_orm-2.1.2/RSO/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-23 08:35:37.000000 redis_simple_orm-2.1.2/RSO/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:35:51.970314 redis_simple_orm-2.1.2/RSO/txredisapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 08:35:37.000000 redis_simple_orm-2.1.2/RSO/txredisapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-05-23 08:35:37.000000 redis_simple_orm-2.1.2/RSO/txredisapi/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-23 08:35:37.000000 redis_simple_orm-2.1.2/RSO/txredisapi/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:35:51.970314 redis_simple_orm-2.1.2/redis_simple_orm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-23 08:35:51.000000 redis_simple_orm-2.1.2/redis_simple_orm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-23 08:35:51.000000 redis_simple_orm-2.1.2/redis_simple_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:35:51.000000 redis_simple_orm-2.1.2/redis_simple_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-23 08:35:51.000000 redis_simple_orm-2.1.2/redis_simple_orm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-23 08:35:51.000000 redis_simple_orm-2.1.2/redis_simple_orm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-23 08:35:51.970314 redis_simple_orm-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-23 08:35:37.000000 redis_simple_orm-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:35:51.970314 redis_simple_orm-2.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-23 08:35:37.000000 redis_simple_orm-2.1.2/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-05-23 08:35:37.000000 redis_simple_orm-2.1.2/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-23 08:35:37.000000 redis_simple_orm-2.1.2/tests/test_model.py
```

### Comparing `redis_simple_orm-2.1.1/LICENSE` & `redis_simple_orm-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.1.1/PKG-INFO` & `redis_simple_orm-2.1.2/redis_simple_orm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: redis_simple_orm
-Version: 2.1.1
+Name: redis-simple-orm
+Version: 2.1.2
 Summary: Simple Redis ORM (Sync and Async).
 Home-page: https://github.com/jockerz/redis_simple_orm
 Author: Jockerz
 Author-email: jockerz@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `redis_simple_orm-2.1.1/README.md` & `redis_simple_orm-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.1.1/RSO/asyncio/index.py` & `redis_simple_orm-2.1.2/RSO/asyncio/index.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.1.1/RSO/asyncio/model.py` & `redis_simple_orm-2.1.2/RSO/asyncio/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         pipe.hset(self.redis_key, mapping=self.to_redis())
 
         for index_class in self.__indexes__:
             if getattr(self, index_class.__key__, None) is None:
                 continue
             await index_class.save(pipe, self)
 
-        if not isinstance(redis, (Pipeline, Pipeline2)):
+        if not isinstance(redis, PIPE_CLS):
             await pipe.execute()
 
     @classmethod
     async def search(cls, redis: T_REDIS, value) -> Optional['Model']:
         redis_key = cls.redis_key_from_value(value)
         if bool(await redis.exists(redis_key)) is True:
             fields = cls.get_fields()
```

### Comparing `redis_simple_orm-2.1.1/RSO/base.py` & `redis_simple_orm-2.1.2/RSO/base.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.1.1/RSO/index.py` & `redis_simple_orm-2.1.2/RSO/index.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.1.1/RSO/model.py` & `redis_simple_orm-2.1.2/RSO/model.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.1.1/RSO/txredisapi/index.py` & `redis_simple_orm-2.1.2/RSO/txredisapi/index.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.1.1/RSO/txredisapi/model.py` & `redis_simple_orm-2.1.2/RSO/txredisapi/model.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.1.1/redis_simple_orm.egg-info/PKG-INFO` & `redis_simple_orm-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: redis-simple-orm
-Version: 2.1.1
+Name: redis_simple_orm
+Version: 2.1.2
 Summary: Simple Redis ORM (Sync and Async).
 Home-page: https://github.com/jockerz/redis_simple_orm
 Author: Jockerz
 Author-email: jockerz@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `redis_simple_orm-2.1.1/setup.py` & `redis_simple_orm-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.1.1/tests/test_example.py` & `redis_simple_orm-2.1.2/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.1.1/tests/test_index.py` & `redis_simple_orm-2.1.2/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.1.1/tests/test_model.py` & `redis_simple_orm-2.1.2/tests/test_model.py`

 * *Files identical despite different names*

