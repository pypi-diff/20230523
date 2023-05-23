# Comparing `tmp/redis_simple_orm-2.1.0.tar.gz` & `tmp/redis_simple_orm-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_simple_orm-2.1.0.tar", last modified: Tue May 23 07:28:35 2023, max compression
+gzip compressed data, was "redis_simple_orm-2.1.1.tar", last modified: Tue May 23 07:34:54 2023, max compression
```

## Comparing `redis_simple_orm-2.1.0.tar` & `redis_simple_orm-2.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:28:35.650308 redis_simple_orm-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-23 07:28:35.650308 redis_simple_orm-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10511 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:28:35.650308 redis_simple_orm-2.1.0/RSO/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/RSO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:28:35.650308 redis_simple_orm-2.1.0/RSO/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/RSO/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/RSO/asyncio/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/RSO/asyncio/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/RSO/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/RSO/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/RSO/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:28:35.650308 redis_simple_orm-2.1.0/RSO/txredisapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/RSO/txredisapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/RSO/txredisapi/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/RSO/txredisapi/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:28:35.650308 redis_simple_orm-2.1.0/redis_simple_orm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-23 07:28:35.000000 redis_simple_orm-2.1.0/redis_simple_orm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-23 07:28:35.000000 redis_simple_orm-2.1.0/redis_simple_orm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:28:35.000000 redis_simple_orm-2.1.0/redis_simple_orm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-23 07:28:35.000000 redis_simple_orm-2.1.0/redis_simple_orm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-23 07:28:35.000000 redis_simple_orm-2.1.0/redis_simple_orm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-23 07:28:35.650308 redis_simple_orm-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:28:35.650308 redis_simple_orm-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-23 07:28:21.000000 redis_simple_orm-2.1.0/tests/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:54.164361 redis_simple_orm-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-23 07:34:54.164361 redis_simple_orm-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10511 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:54.164361 redis_simple_orm-2.1.1/RSO/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/RSO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:54.164361 redis_simple_orm-2.1.1/RSO/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/RSO/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/RSO/asyncio/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/RSO/asyncio/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/RSO/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/RSO/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/RSO/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:54.164361 redis_simple_orm-2.1.1/RSO/txredisapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/RSO/txredisapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/RSO/txredisapi/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/RSO/txredisapi/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:54.164361 redis_simple_orm-2.1.1/redis_simple_orm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-23 07:34:54.000000 redis_simple_orm-2.1.1/redis_simple_orm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-23 07:34:54.000000 redis_simple_orm-2.1.1/redis_simple_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:34:54.000000 redis_simple_orm-2.1.1/redis_simple_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-23 07:34:54.000000 redis_simple_orm-2.1.1/redis_simple_orm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-23 07:34:54.000000 redis_simple_orm-2.1.1/redis_simple_orm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-23 07:34:54.164361 redis_simple_orm-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:54.164361 redis_simple_orm-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-23 07:34:43.000000 redis_simple_orm-2.1.1/tests/test_model.py
```

### Comparing `redis_simple_orm-2.1.0/LICENSE` & `redis_simple_orm-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.1.0/PKG-INFO` & `redis_simple_orm-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis_simple_orm
-Version: 2.1.0
+Version: 2.1.1
 Summary: Simple Redis ORM (Sync and Async).
 Home-page: https://github.com/jockerz/redis_simple_orm
 Author: Jockerz
 Author-email: jockerz@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `redis_simple_orm-2.1.0/README.md` & `redis_simple_orm-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.1.0/RSO/asyncio/index.py` & `redis_simple_orm-2.1.1/RSO/asyncio/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Optional, TypeVar, Union
 
 from redis.asyncio.client import Redis as Redis2, Pipeline as Pipeline2
 try:
     from aioredis.client import Redis, Pipeline
-except ImportError:
+except (ImportError, ModuleNotFoundError):
     T_PIPE = Pipeline2
     T_REDIS = Redis2
     T_REDIS_PIPE = Union[Redis2, Pipeline2]
     PIPE_CLS = (Pipeline2,)
 else:
     T_PIPE = [Pipeline, Pipeline2]
     T_REDIS = Union[Redis, Redis2]
```

### Comparing `redis_simple_orm-2.1.0/RSO/asyncio/model.py` & `redis_simple_orm-2.1.1/RSO/asyncio/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Optional, Union
 
 from redis.asyncio.client import Redis as Redis2, Pipeline as Pipeline2
 try:
     from aioredis.client import Redis, Pipeline
-except ImportError:
+except (ImportError, ModuleNotFoundError):
     T_REDIS = Union[Redis2]
     T_REDIS_PIPE = Union[Redis2, Pipeline2]
     PIPE_CLS = (Pipeline2,)
 else:
     T_REDIS = Union[Redis, Redis2]
     T_REDIS_PIPE = Union[Redis, Redis2, Pipeline, Pipeline2]
     PIPE_CLS = (Pipeline, Pipeline2)
```

### Comparing `redis_simple_orm-2.1.0/RSO/base.py` & `redis_simple_orm-2.1.1/RSO/base.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.1.0/RSO/index.py` & `redis_simple_orm-2.1.1/RSO/index.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.1.0/RSO/model.py` & `redis_simple_orm-2.1.1/RSO/model.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.1.0/RSO/txredisapi/index.py` & `redis_simple_orm-2.1.1/RSO/txredisapi/index.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.1.0/RSO/txredisapi/model.py` & `redis_simple_orm-2.1.1/RSO/txredisapi/model.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.1.0/redis_simple_orm.egg-info/PKG-INFO` & `redis_simple_orm-2.1.1/redis_simple_orm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-simple-orm
-Version: 2.1.0
+Version: 2.1.1
 Summary: Simple Redis ORM (Sync and Async).
 Home-page: https://github.com/jockerz/redis_simple_orm
 Author: Jockerz
 Author-email: jockerz@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `redis_simple_orm-2.1.0/setup.py` & `redis_simple_orm-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.1.0/tests/test_example.py` & `redis_simple_orm-2.1.1/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.1.0/tests/test_index.py` & `redis_simple_orm-2.1.1/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.1.0/tests/test_model.py` & `redis_simple_orm-2.1.1/tests/test_model.py`

 * *Files identical despite different names*

