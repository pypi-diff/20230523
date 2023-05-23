# Comparing `tmp/anduin-8.4.8.tar.gz` & `tmp/anduin-8.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anduin-8.4.8.tar", last modified: Fri Mar 17 07:18:16 2023, max compression
+gzip compressed data, was "anduin-8.4.9.tar", last modified: Mon Mar 20 07:05:24 2023, max compression
```

## Comparing `anduin-8.4.8.tar` & `anduin-8.4.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-17 07:18:16.834312 anduin-8.4.8/
--rw-r--r--   0 Campanula   (501) staff       (20)      849 2023-03-17 07:18:16.833777 anduin-8.4.8/PKG-INFO
--rw-r--r--   0 Campanula   (501) staff       (20)      209 2023-01-15 17:04:33.000000 anduin-8.4.8/README.md
-drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-17 07:18:16.806928 anduin-8.4.8/anduin/
--rw-r--r--   0 Campanula   (501) staff       (20)      964 2023-03-09 04:34:35.000000 anduin-8.4.8/anduin/Scheduler.py
--rw-r--r--   0 Campanula   (501) staff       (20)     3317 2023-03-17 07:18:15.000000 anduin-8.4.8/anduin/__init__.py
-drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-17 07:18:16.812814 anduin-8.4.8/anduin/common/
--rw-r--r--   0 Campanula   (501) staff       (20)       21 2023-03-09 04:34:35.000000 anduin-8.4.8/anduin/common/__init__.py
--rw-r--r--   0 Campanula   (501) staff       (20)     3136 2023-03-15 03:52:36.000000 anduin-8.4.8/anduin/common/tools.py
--rw-r--r--   0 Campanula   (501) staff       (20)     3619 2021-05-06 12:21:24.000000 anduin-8.4.8/anduin/construct_file.py
-drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-17 07:18:16.813684 anduin-8.4.8/anduin/db/
--rw-r--r--   0 Campanula   (501) staff       (20)       82 2023-03-09 06:43:34.000000 anduin-8.4.8/anduin/db/__init__.py
-drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-17 07:18:16.814824 anduin-8.4.8/anduin/db/no_sql/
--rw-r--r--   0 Campanula   (501) staff       (20)       82 2023-03-09 06:41:44.000000 anduin-8.4.8/anduin/db/no_sql/__init__.py
-drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-17 07:18:16.817630 anduin-8.4.8/anduin/db/no_sql/async_redis/
--rw-r--r--   0 Campanula   (501) staff       (20)       82 2023-03-09 06:41:53.000000 anduin-8.4.8/anduin/db/no_sql/async_redis/__init__.py
--rw-r--r--   0 Campanula   (501) staff       (20)     1897 2023-03-10 04:47:02.000000 anduin-8.4.8/anduin/db/no_sql/async_redis/redis_client.py
--rw-r--r--   0 Campanula   (501) staff       (20)     1366 2023-03-10 01:34:20.000000 anduin-8.4.8/anduin/db/no_sql/async_redis/redis_client_manager.py
-drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-17 07:18:16.819805 anduin-8.4.8/anduin/db/no_sql/redis/
--rw-r--r--   0 Campanula   (501) staff       (20)        0 2023-03-10 01:34:20.000000 anduin-8.4.8/anduin/db/no_sql/redis/__init__.py
--rw-r--r--   0 Campanula   (501) staff       (20)     1826 2023-03-10 04:47:02.000000 anduin-8.4.8/anduin/db/no_sql/redis/redis_client.py
--rw-r--r--   0 Campanula   (501) staff       (20)     1417 2023-03-10 01:44:56.000000 anduin-8.4.8/anduin/db/no_sql/redis/redis_client_manager.py
-drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-17 07:18:16.820855 anduin-8.4.8/anduin/db/sql/
--rw-r--r--   0 Campanula   (501) staff       (20)       82 2023-03-09 06:43:34.000000 anduin-8.4.8/anduin/db/sql/__init__.py
-drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-17 07:18:16.822999 anduin-8.4.8/anduin/db/sql/async_mysql/
--rw-r--r--   0 Campanula   (501) staff       (20)       82 2023-03-09 06:43:34.000000 anduin-8.4.8/anduin/db/sql/async_mysql/__init__.py
--rw-r--r--   0 Campanula   (501) staff       (20)     6182 2023-03-17 06:57:22.000000 anduin-8.4.8/anduin/db/sql/async_mysql/db_client.py
--rw-r--r--   0 Campanula   (501) staff       (20)     1399 2023-03-10 07:28:20.000000 anduin-8.4.8/anduin/db/sql/async_mysql/db_client_manager.py
-drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-17 07:18:16.826222 anduin-8.4.8/anduin/db/sql/mysql/
--rw-r--r--   0 Campanula   (501) staff       (20)       82 2023-03-09 06:43:34.000000 anduin-8.4.8/anduin/db/sql/mysql/__init__.py
--rw-r--r--   0 Campanula   (501) staff       (20)    10784 2023-03-17 07:17:55.000000 anduin-8.4.8/anduin/db/sql/mysql/db_client.py
--rw-r--r--   0 Campanula   (501) staff       (20)     1343 2023-03-10 01:34:20.000000 anduin-8.4.8/anduin/db/sql/mysql/db_client_manager.py
-drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-17 07:18:16.829523 anduin-8.4.8/anduin/db/sql/sqlite/
--rw-r--r--   0 Campanula   (501) staff       (20)       82 2023-03-09 06:43:34.000000 anduin-8.4.8/anduin/db/sql/sqlite/__init__.py
--rw-r--r--   0 Campanula   (501) staff       (20)     5344 2023-03-17 06:57:22.000000 anduin-8.4.8/anduin/db/sql/sqlite/db_client.py
--rw-r--r--   0 Campanula   (501) staff       (20)     1270 2023-03-10 01:34:20.000000 anduin-8.4.8/anduin/db/sql/sqlite/db_client_manager.py
-drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-17 07:18:16.831434 anduin-8.4.8/anduin/frames/
--rw-r--r--   0 Campanula   (501) staff       (20)        0 2023-03-09 06:43:10.000000 anduin-8.4.8/anduin/frames/__init__.py
--rw-r--r--   0 Campanula   (501) staff       (20)      962 2023-03-16 02:57:11.000000 anduin-8.4.8/anduin/frames/client_base.py
--rw-r--r--   0 Campanula   (501) staff       (20)     2338 2023-03-10 08:40:09.000000 anduin-8.4.8/anduin/frames/manager_base.py
-drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-17 07:18:16.832871 anduin-8.4.8/anduin/parser/
--rw-r--r--   0 Campanula   (501) staff       (20)       82 2023-03-09 06:43:34.000000 anduin-8.4.8/anduin/parser/__init__.py
--rw-r--r--   0 Campanula   (501) staff       (20)     4386 2023-03-09 06:08:22.000000 anduin-8.4.8/anduin/parser/sql_parser.py
-drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-17 07:18:16.810438 anduin-8.4.8/anduin.egg-info/
--rw-r--r--   0 Campanula   (501) staff       (20)      849 2023-03-17 07:18:16.000000 anduin-8.4.8/anduin.egg-info/PKG-INFO
--rw-r--r--   0 Campanula   (501) staff       (20)     1120 2023-03-17 07:18:16.000000 anduin-8.4.8/anduin.egg-info/SOURCES.txt
--rw-r--r--   0 Campanula   (501) staff       (20)        1 2023-03-17 07:18:16.000000 anduin-8.4.8/anduin.egg-info/dependency_links.txt
--rw-r--r--   0 Campanula   (501) staff       (20)       57 2023-03-17 07:18:16.000000 anduin-8.4.8/anduin.egg-info/requires.txt
--rw-r--r--   0 Campanula   (501) staff       (20)        7 2023-03-17 07:18:16.000000 anduin-8.4.8/anduin.egg-info/top_level.txt
--rw-r--r--   0 Campanula   (501) staff       (20)        1 2021-04-01 08:25:26.000000 anduin-8.4.8/anduin.egg-info/zip-safe
--rw-r--r--   0 Campanula   (501) staff       (20)       38 2023-03-17 07:18:16.834498 anduin-8.4.8/setup.cfg
--rw-r--r--   0 Campanula   (501) staff       (20)     1304 2023-03-17 07:18:15.000000 anduin-8.4.8/setup.py
+drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-20 07:05:24.570078 anduin-8.4.9/
+-rw-r--r--   0 Campanula   (501) staff       (20)      849 2023-03-20 07:05:24.569595 anduin-8.4.9/PKG-INFO
+-rw-r--r--   0 Campanula   (501) staff       (20)      209 2023-01-15 17:04:33.000000 anduin-8.4.9/README.md
+drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-20 07:05:24.539455 anduin-8.4.9/anduin/
+-rw-r--r--   0 Campanula   (501) staff       (20)      964 2023-03-09 04:34:35.000000 anduin-8.4.9/anduin/Scheduler.py
+-rw-r--r--   0 Campanula   (501) staff       (20)     3317 2023-03-20 07:05:23.000000 anduin-8.4.9/anduin/__init__.py
+drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-20 07:05:24.545750 anduin-8.4.9/anduin/common/
+-rw-r--r--   0 Campanula   (501) staff       (20)       21 2023-03-09 04:34:35.000000 anduin-8.4.9/anduin/common/__init__.py
+-rw-r--r--   0 Campanula   (501) staff       (20)     3136 2023-03-15 03:52:36.000000 anduin-8.4.9/anduin/common/tools.py
+-rw-r--r--   0 Campanula   (501) staff       (20)     3619 2021-05-06 12:21:24.000000 anduin-8.4.9/anduin/construct_file.py
+drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-20 07:05:24.546600 anduin-8.4.9/anduin/db/
+-rw-r--r--   0 Campanula   (501) staff       (20)       82 2023-03-09 06:43:34.000000 anduin-8.4.9/anduin/db/__init__.py
+drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-20 07:05:24.547978 anduin-8.4.9/anduin/db/no_sql/
+-rw-r--r--   0 Campanula   (501) staff       (20)       82 2023-03-09 06:41:44.000000 anduin-8.4.9/anduin/db/no_sql/__init__.py
+drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-20 07:05:24.555433 anduin-8.4.9/anduin/db/no_sql/async_redis/
+-rw-r--r--   0 Campanula   (501) staff       (20)       82 2023-03-09 06:41:53.000000 anduin-8.4.9/anduin/db/no_sql/async_redis/__init__.py
+-rw-r--r--   0 Campanula   (501) staff       (20)     1897 2023-03-10 04:47:02.000000 anduin-8.4.9/anduin/db/no_sql/async_redis/redis_client.py
+-rw-r--r--   0 Campanula   (501) staff       (20)     1362 2023-03-20 07:05:21.000000 anduin-8.4.9/anduin/db/no_sql/async_redis/redis_client_manager.py
+drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-20 07:05:24.557596 anduin-8.4.9/anduin/db/no_sql/redis/
+-rw-r--r--   0 Campanula   (501) staff       (20)        0 2023-03-10 01:34:20.000000 anduin-8.4.9/anduin/db/no_sql/redis/__init__.py
+-rw-r--r--   0 Campanula   (501) staff       (20)     1826 2023-03-10 04:47:02.000000 anduin-8.4.9/anduin/db/no_sql/redis/redis_client.py
+-rw-r--r--   0 Campanula   (501) staff       (20)     1413 2023-03-20 07:05:21.000000 anduin-8.4.9/anduin/db/no_sql/redis/redis_client_manager.py
+drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-20 07:05:24.558161 anduin-8.4.9/anduin/db/sql/
+-rw-r--r--   0 Campanula   (501) staff       (20)       82 2023-03-09 06:43:34.000000 anduin-8.4.9/anduin/db/sql/__init__.py
+drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-20 07:05:24.560710 anduin-8.4.9/anduin/db/sql/async_mysql/
+-rw-r--r--   0 Campanula   (501) staff       (20)       82 2023-03-09 06:43:34.000000 anduin-8.4.9/anduin/db/sql/async_mysql/__init__.py
+-rw-r--r--   0 Campanula   (501) staff       (20)     6182 2023-03-17 06:57:22.000000 anduin-8.4.9/anduin/db/sql/async_mysql/db_client.py
+-rw-r--r--   0 Campanula   (501) staff       (20)     1395 2023-03-20 07:04:34.000000 anduin-8.4.9/anduin/db/sql/async_mysql/db_client_manager.py
+drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-20 07:05:24.562486 anduin-8.4.9/anduin/db/sql/mysql/
+-rw-r--r--   0 Campanula   (501) staff       (20)       82 2023-03-09 06:43:34.000000 anduin-8.4.9/anduin/db/sql/mysql/__init__.py
+-rw-r--r--   0 Campanula   (501) staff       (20)    10755 2023-03-20 05:49:30.000000 anduin-8.4.9/anduin/db/sql/mysql/db_client.py
+-rw-r--r--   0 Campanula   (501) staff       (20)     1424 2023-03-20 07:05:21.000000 anduin-8.4.9/anduin/db/sql/mysql/db_client_manager.py
+drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-20 07:05:24.565196 anduin-8.4.9/anduin/db/sql/sqlite/
+-rw-r--r--   0 Campanula   (501) staff       (20)       82 2023-03-09 06:43:34.000000 anduin-8.4.9/anduin/db/sql/sqlite/__init__.py
+-rw-r--r--   0 Campanula   (501) staff       (20)     5344 2023-03-17 06:57:22.000000 anduin-8.4.9/anduin/db/sql/sqlite/db_client.py
+-rw-r--r--   0 Campanula   (501) staff       (20)     1266 2023-03-20 07:05:21.000000 anduin-8.4.9/anduin/db/sql/sqlite/db_client_manager.py
+drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-20 07:05:24.567153 anduin-8.4.9/anduin/frames/
+-rw-r--r--   0 Campanula   (501) staff       (20)        0 2023-03-09 06:43:10.000000 anduin-8.4.9/anduin/frames/__init__.py
+-rw-r--r--   0 Campanula   (501) staff       (20)      962 2023-03-16 02:57:11.000000 anduin-8.4.9/anduin/frames/client_base.py
+-rw-r--r--   0 Campanula   (501) staff       (20)     2539 2023-03-20 07:04:34.000000 anduin-8.4.9/anduin/frames/manager_base.py
+drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-20 07:05:24.568470 anduin-8.4.9/anduin/parser/
+-rw-r--r--   0 Campanula   (501) staff       (20)       82 2023-03-09 06:43:34.000000 anduin-8.4.9/anduin/parser/__init__.py
+-rw-r--r--   0 Campanula   (501) staff       (20)     4386 2023-03-09 06:08:22.000000 anduin-8.4.9/anduin/parser/sql_parser.py
+drwxr-xr-x   0 Campanula   (501) staff       (20)        0 2023-03-20 07:05:24.543485 anduin-8.4.9/anduin.egg-info/
+-rw-r--r--   0 Campanula   (501) staff       (20)      849 2023-03-20 07:05:24.000000 anduin-8.4.9/anduin.egg-info/PKG-INFO
+-rw-r--r--   0 Campanula   (501) staff       (20)     1120 2023-03-20 07:05:24.000000 anduin-8.4.9/anduin.egg-info/SOURCES.txt
+-rw-r--r--   0 Campanula   (501) staff       (20)        1 2023-03-20 07:05:24.000000 anduin-8.4.9/anduin.egg-info/dependency_links.txt
+-rw-r--r--   0 Campanula   (501) staff       (20)       57 2023-03-20 07:05:24.000000 anduin-8.4.9/anduin.egg-info/requires.txt
+-rw-r--r--   0 Campanula   (501) staff       (20)        7 2023-03-20 07:05:24.000000 anduin-8.4.9/anduin.egg-info/top_level.txt
+-rw-r--r--   0 Campanula   (501) staff       (20)        1 2021-04-01 08:25:26.000000 anduin-8.4.9/anduin.egg-info/zip-safe
+-rw-r--r--   0 Campanula   (501) staff       (20)       38 2023-03-20 07:05:24.570243 anduin-8.4.9/setup.cfg
+-rw-r--r--   0 Campanula   (501) staff       (20)     1304 2023-03-20 07:05:23.000000 anduin-8.4.9/setup.py
```

### Comparing `anduin-8.4.8/PKG-INFO` & `anduin-8.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: anduin
-Version: 8.4.8
+Version: 8.4.9
 Summary: a lite mysql & sqlite3 & async_redis connect engine, mapping table into k-v structure , support async work
 Home-page: https://github.com/campanulamediuml/Anduin
 Author: campanula
 Author-email: campanulamediuml@gmail.com
 License: MIT
 Description: 一个轻量化的sqlite/mysql数据序列化操作引擎
         名称来自《指环王》
```

### Comparing `anduin-8.4.8/anduin/Scheduler.py` & `anduin-8.4.9/anduin/Scheduler.py`

 * *Files identical despite different names*

### Comparing `anduin-8.4.8/anduin/__init__.py` & `anduin-8.4.9/anduin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,11 +71,11 @@
 
 Data = auto_init()
 if Data is None:
     dbg('自动初始化同步mysql失败')
 
 
 
-__version__ = "8.4.8"
+__version__ = "8.4.9"
```

### Comparing `anduin-8.4.8/anduin/common/tools.py` & `anduin-8.4.9/anduin/common/tools.py`

 * *Files identical despite different names*

### Comparing `anduin-8.4.8/anduin/construct_file.py` & `anduin-8.4.9/anduin/construct_file.py`

 * *Files identical despite different names*

### Comparing `anduin-8.4.8/anduin/db/no_sql/async_redis/redis_client.py` & `anduin-8.4.9/anduin/db/no_sql/async_redis/redis_client.py`

 * *Files identical despite different names*

### Comparing `anduin-8.4.8/anduin/db/no_sql/async_redis/redis_client_manager.py` & `anduin-8.4.9/anduin/db/no_sql/async_redis/redis_client_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # !/usr/bin/env python
 # -*-coding:utf-8 -*-
 # Author     ：Campanula 梦芸 何
 import time
 
 from anduin.common import ENGINE_REDIS,dbg,get_db_index
 from anduin.db.no_sql.async_redis.redis_client import AsyncRedisClient
-from anduin.frames.manager_base import ManagerBase, TIMEOUT
+from anduin.frames.manager_base import ManagerBase
 
 
 class AsyncRedisManager(ManagerBase):
     def __init__(self,config):
         super().__init__(config)
 
     def create_connection(self)->AsyncRedisClient:
@@ -23,15 +23,15 @@
 
     def get_free_client(self)->AsyncRedisClient:
         self.clean_pool()
         my_client = None
         cur_time = int(time.time())
         my_pool = self.get_cur_client_pool_by_thread_id()
         for sid, client in my_pool.items():
-            if cur_time - client.last_connect_time < TIMEOUT:
+            if cur_time - client.last_connect_time < self.TIMEOUT:
                 if client.is_lock is False:
                     my_client = client
                     break
         if my_client is None:
             my_client = self.create_connection()
         my_client.lock()
         return my_client
```

### Comparing `anduin-8.4.8/anduin/db/no_sql/redis/redis_client.py` & `anduin-8.4.9/anduin/db/no_sql/redis/redis_client.py`

 * *Files identical despite different names*

### Comparing `anduin-8.4.8/anduin/db/no_sql/redis/redis_client_manager.py` & `anduin-8.4.9/anduin/db/no_sql/redis/redis_client_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # !/usr/bin/env python
 # -*-coding:utf-8 -*-
 # Author     ：Campanula 梦芸 何
 import time
 
 from anduin.common import ENGINE_REDIS,dbg,get_db_index
 from anduin.db.no_sql.redis.redis_client import RedisClient
-from anduin.frames.manager_base import ManagerBase, TIMEOUT
+from anduin.frames.manager_base import ManagerBase
 
 
 class RedisManager(ManagerBase):
     def __init__(self,config):
         super().__init__(config)
 
     def create_connection(self)->RedisClient:
@@ -26,15 +26,15 @@
 
     def get_free_client(self)->RedisClient:
         self.clean_pool()
         my_client = None
         cur_time = int(time.time())
         my_pool = self.get_cur_client_pool_by_thread_id()
         for sid, client in my_pool.items():
-            if cur_time - client.last_connect_time < TIMEOUT:
+            if cur_time - client.last_connect_time < self.TIMEOUT:
                 if client.is_lock is False:
                     my_client = client
                     break
         if my_client is None:
             my_client = self.create_connection()
         my_client.lock()
         return my_client
```

### Comparing `anduin-8.4.8/anduin/db/sql/async_mysql/db_client.py` & `anduin-8.4.9/anduin/db/sql/async_mysql/db_client.py`

 * *Files identical despite different names*

### Comparing `anduin-8.4.8/anduin/db/sql/async_mysql/db_client_manager.py` & `anduin-8.4.9/anduin/db/sql/async_mysql/db_client_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Author     ：Campanula 梦芸 何
 import asyncio
 import time
 
 
 from anduin.common import dbg,get_db_index,ENGINE_MYSQL
 from anduin.db.sql.async_mysql.db_client import AsyncMySQLClient
-from anduin.frames.manager_base import ManagerBase, TIMEOUT
+from anduin.frames.manager_base import ManagerBase
 
 
 class AsyncMySQLManager(ManagerBase):
     def __init__(self, config):
         super().__init__(config)
 
     async def create_connection(self):
@@ -26,15 +26,15 @@
 
     async def get_free_client(self):
         self.clean_pool()
         my_client = None
         cur_time = int(time.time())
         my_pool = self.get_cur_client_pool_by_thread_id()
         for sid, client in my_pool.items():
-            if cur_time - client.last_connect_time < TIMEOUT:
+            if cur_time - client.last_connect_time < self.TIMEOUT:
                 if client.is_lock is False:
                     my_client = client
                     break
         if my_client is None:
             my_client = await self.create_connection()
         my_client.lock()
         return my_client
```

### Comparing `anduin-8.4.8/anduin/db/sql/mysql/db_client.py` & `anduin-8.4.9/anduin/db/sql/mysql/db_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     def commit(self):
         '''
         commit本次事务
         '''
         self.db.commit()
 
-    def query(self, sql: str, show_sql=None, sql_params=None, return_dict=False):
+    def query(self, sql: str, show_sql=False, sql_params=None, return_dict=False):
         '''
         直接执行sql语句
         :param
             sql:数据库sql语句
             show_sql:是否展示本次语句
             sql_params:当sql为带参数语句的时候，是否使用参数
             return_dict:是否使用Dict类型
@@ -238,15 +238,14 @@
                 默认False，开启后将会显示此次执行的sql内容并写入日志
         '''
         sql, sql_params = Parser.insert_parser(table, content)
         r = self.query(sql, show_sql, sql_params)
         return r
 
     def update(self, table, conditions, or_cond=None, params=None, show_sql=False):
-        # dbg('开始执行')
         """
         传入参数：
             table:表名称
                 数据类型为字符串
 
             conditions:查询条件
                 数据类型为列表内包含可迭代对象（元组，列表，集合），逻辑为and
```

### Comparing `anduin-8.4.8/anduin/db/sql/mysql/db_client_manager.py` & `anduin-8.4.9/anduin/db/sql/mysql/db_client_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # !/usr/bin/env python
 # -*-coding:utf-8 -*-
 # Author     ：Campanula 梦芸 何
 import time
 
 from anduin.common import ENGINE_MYSQL,get_db_index,dbg
 from anduin.db.sql.mysql.db_client import MySQLClient
-from anduin.frames.manager_base import ManagerBase, TIMEOUT
+from anduin.frames.manager_base import ManagerBase
 
 
 class MySQLManager(ManagerBase):
     def __init__(self, config):
         super().__init__(config)
 
     def create_connection(self):
@@ -17,21 +17,24 @@
         db_client = MySQLClient(self.host, self.user, self.password, self.port, self.database, ENGINE_MYSQL,
                                 self.charset)
         my_pool = self.get_cur_client_pool_by_thread_id()
         sid = id(db_client)
         my_pool[sid] = db_client
         return db_client
 
-    def get_free_client(self):
+    def get_free_client(self) ->MySQLClient:
+        '''
+        获取一个mysql链接客户端实例
+        '''
         # print(self.get_cur_thread_id())
         my_client = None
         cur_time = int(time.time())
         my_pool = self.get_cur_client_pool_by_thread_id()
         for sid, client in my_pool.items():
-            if cur_time - client.last_connect_time < TIMEOUT:
+            if cur_time - client.last_connect_time < self.TIMEOUT:
                 if client.is_lock is False:
                     my_client = client
                     break
         if my_client is None:
             my_client = self.create_connection()
         my_client.lock()
         self.clean_pool()
```

### Comparing `anduin-8.4.8/anduin/db/sql/sqlite/db_client.py` & `anduin-8.4.9/anduin/db/sql/sqlite/db_client.py`

 * *Files identical despite different names*

### Comparing `anduin-8.4.8/anduin/db/sql/sqlite/db_client_manager.py` & `anduin-8.4.9/anduin/db/sql/sqlite/db_client_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # !/usr/bin/env python
 # -*-coding:utf-8 -*-
 # Author     ：Campanula 梦芸 何
 import time
 
 from anduin.common import ENGINE_SQLITE,get_db_index,dbg
 from anduin.db.sql.sqlite.db_client import SQLiteClient
-from anduin.frames.manager_base import ManagerBase, TIMEOUT
+from anduin.frames.manager_base import ManagerBase
 
 
 class SQLiteManager(ManagerBase):
     def __init__(self, config):
         super().__init__(config)
 
     def create_connection(self):
@@ -22,15 +22,15 @@
 
     def get_free_client(self):
         self.clean_pool()
         my_client = None
         cur_time = int(time.time())
         my_pool = self.get_cur_client_pool_by_thread_id()
         for sid, client in my_pool.items():
-            if cur_time - client.last_connect_time < TIMEOUT:
+            if cur_time - client.last_connect_time < self.TIMEOUT:
                 if client.is_lock is False:
                     my_client = client
                     break
         if my_client is None:
             my_client = self.create_connection()
         my_client.lock()
         return my_client
```

### Comparing `anduin-8.4.8/anduin/frames/client_base.py` & `anduin-8.4.9/anduin/frames/client_base.py`

 * *Files identical despite different names*

### Comparing `anduin-8.4.8/anduin/frames/manager_base.py` & `anduin-8.4.9/anduin/frames/manager_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 import threading
 import time
 from typing import List, Dict
 
 from anduin.common import dbg, get_obj_name
 from anduin.frames.client_base import ClientBase
 
-TIMEOUT = 30
+
 
 class ManagerBase(abc.ABC):
     def __init__(self, db_config):
+        self.TIMEOUT = 30
         self.use_cache = False
         self.t_data = db_config
         self.host = db_config.get('host')
         self.user = db_config.get('user')
         self.password = db_config.get('password')
         self.database = db_config.get('database')
         self.charset = db_config.get('charset')
@@ -64,16 +65,25 @@
     def clean_pool(self):
         cur_time = int(time.time())
         cur_out_time_pool = self.get_cur_outtime_pool_by_thread_id()
         cur_pool = self.get_cur_client_pool_by_thread_id()
         # print(cur_out_time_pool)
         # print(cur_pool)
         for sid,client in cur_pool.items():
-            if cur_time - client.last_connect_time > TIMEOUT:
+            if cur_time - client.last_connect_time > self.TIMEOUT:
                 if client.is_lock is False:
                     cur_out_time_pool.append(sid)
         for sid in cur_out_time_pool:
             if sid in cur_pool:
                 cur_pool.pop(sid)
 
+    def get_time_out(self):
+        return self.TIMEOUT
+
+    def set_time_out(self,time_out:int):
+        '''
+        设置超时时间
+        '''
+        self.TIMEOUT = time_out
+
```

### Comparing `anduin-8.4.8/anduin/parser/sql_parser.py` & `anduin-8.4.9/anduin/parser/sql_parser.py`

 * *Files identical despite different names*

### Comparing `anduin-8.4.8/anduin.egg-info/PKG-INFO` & `anduin-8.4.9/anduin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: anduin
-Version: 8.4.8
+Version: 8.4.9
 Summary: a lite mysql & sqlite3 & async_redis connect engine, mapping table into k-v structure , support async work
 Home-page: https://github.com/campanulamediuml/Anduin
 Author: campanula
 Author-email: campanulamediuml@gmail.com
 License: MIT
 Description: 一个轻量化的sqlite/mysql数据序列化操作引擎
         名称来自《指环王》
```

### Comparing `anduin-8.4.8/anduin.egg-info/SOURCES.txt` & `anduin-8.4.9/anduin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anduin-8.4.8/setup.py` & `anduin-8.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import codecs
 import os
 from setuptools import setup, find_packages
 
-VER = "8.4.8"
+VER = "8.4.9"
 
 def read(fname):
     return codecs.open(os.path.join(os.path.dirname(__file__), fname),encoding='utf-8').read()
 
 if __name__ == '__main__':
     setup(
         # 以下为必需参数
```

