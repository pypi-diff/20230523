# Comparing `tmp/hagworm-5.5.5.tar.gz` & `tmp/hagworm-5.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagworm-5.5.5.tar", last modified: Mon May 22 03:51:14 2023, max compression
+gzip compressed data, was "hagworm-5.5.6.tar", last modified: Tue May 23 05:41:25 2023, max compression
```

## Comparing `hagworm-5.5.5.tar` & `hagworm-5.5.6.tar`

### file list

```diff
@@ -1,95 +1,91 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.854727 hagworm-5.5.5/
--rw-rw-rw-   0        0        0    11362 2023-03-01 02:07:14.000000 hagworm-5.5.5/LICENSE
--rw-rw-rw-   0        0        0     7508 2023-05-22 03:51:14.853728 hagworm-5.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     6065 2023-04-08 01:06:26.000000 hagworm-5.5.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.749728 hagworm-5.5.5/c_extend/
--rw-rw-rw-   0        0        0      847 2023-03-01 02:07:14.000000 hagworm-5.5.5/c_extend/math.c
-drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.751728 hagworm-5.5.5/example/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.757728 hagworm-5.5.5/example/fastapi_demo/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/example/fastapi_demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.760731 hagworm-5.5.5/example/fastapi_demo/controller/
--rw-rw-rw-   0        0        0      211 2023-03-01 02:07:14.000000 hagworm-5.5.5/example/fastapi_demo/controller/__init__.py
--rw-rw-rw-   0        0        0      397 2023-03-01 02:07:14.000000 hagworm-5.5.5/example/fastapi_demo/controller/home.py
--rw-rw-rw-   0        0        0      888 2023-05-11 03:07:54.000000 hagworm-5.5.5/example/fastapi_demo/gunicorn.config.py
--rw-rw-rw-   0        0        0     1431 2023-05-17 08:11:13.000000 hagworm-5.5.5/example/fastapi_demo/main.py
-drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.762730 hagworm-5.5.5/example/fastapi_demo/model/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/example/fastapi_demo/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.763731 hagworm-5.5.5/example/fastapi_demo/service/
--rw-rw-rw-   0        0        0     3496 2023-05-22 00:30:47.000000 hagworm-5.5.5/example/fastapi_demo/service/__init__.py
--rw-rw-rw-   0        0        0     2096 2023-03-01 02:07:14.000000 hagworm-5.5.5/example/fastapi_demo/setting.py
--rw-rw-rw-   0        0        0      800 2023-05-11 03:07:54.000000 hagworm-5.5.5/example/main_test.py
-drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.764730 hagworm-5.5.5/hagworm/
--rw-rw-rw-   0        0        0      495 2023-05-22 03:46:07.000000 hagworm-5.5.5/hagworm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.799728 hagworm-5.5.5/hagworm/extend/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.827728 hagworm-5.5.5/hagworm/extend/asyncio/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/asyncio/__init__.py
--rw-rw-rw-   0        0        0    16802 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/asyncio/base.py
--rw-rw-rw-   0        0        0     4988 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/asyncio/buffer.py
--rw-rw-rw-   0        0        0     2396 2023-05-11 03:07:54.000000 hagworm-5.5.5/hagworm/extend/asyncio/command.py
--rw-rw-rw-   0        0        0     2432 2023-05-18 10:57:40.000000 hagworm-5.5.5/hagworm/extend/asyncio/etcd.py
--rw-rw-rw-   0        0        0     3194 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/asyncio/event.py
--rw-rw-rw-   0        0        0     1370 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/asyncio/file.py
--rw-rw-rw-   0        0        0     4232 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/asyncio/future.py
--rw-rw-rw-   0        0        0     2603 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/asyncio/mail.py
--rw-rw-rw-   0        0        0     3897 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/asyncio/mongo.py
--rw-rw-rw-   0        0        0    15022 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/asyncio/mysql.py
--rw-rw-rw-   0        0        0    13489 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/asyncio/net.py
--rw-rw-rw-   0        0        0     4149 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/asyncio/ntp.py
--rw-rw-rw-   0        0        0     1570 2023-05-20 02:55:55.000000 hagworm-5.5.5/hagworm/extend/asyncio/pool.py
--rw-rw-rw-   0        0        0    12507 2023-05-22 03:45:54.000000 hagworm-5.5.5/hagworm/extend/asyncio/redis.py
--rw-rw-rw-   0        0        0     7279 2023-05-11 03:07:54.000000 hagworm-5.5.5/hagworm/extend/asyncio/socket.py
--rw-rw-rw-   0        0        0     6170 2023-04-11 07:28:18.000000 hagworm-5.5.5/hagworm/extend/asyncio/task.py
--rw-rw-rw-   0        0        0     1360 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/asyncio/transaction.py
--rw-rw-rw-   0        0        0     3792 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/asyncio/zmq.py
--rw-rw-rw-   0        0        0    22623 2023-05-11 03:07:54.000000 hagworm-5.5.5/hagworm/extend/base.py
--rw-rw-rw-   0        0        0     2365 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/cache.py
--rw-rw-rw-   0        0        0     1839 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/compile.py
--rw-rw-rw-   0        0        0     3857 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/config.py
--rw-rw-rw-   0        0        0     1487 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/crypto.py
--rw-rw-rw-   0        0        0     1792 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/error.py
--rw-rw-rw-   0        0        0     1220 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/event.py
--rw-rw-rw-   0        0        0     4558 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/igraph.py
--rw-rw-rw-   0        0        0     2326 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/interface.py
--rw-rw-rw-   0        0        0    14870 2023-05-13 05:06:56.000000 hagworm-5.5.5/hagworm/extend/logging.py
--rw-rw-rw-   0        0        0     1791 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/media.py
--rw-rw-rw-   0        0        0     1603 2023-05-10 07:58:09.000000 hagworm-5.5.5/hagworm/extend/metaclass.py
--rw-rw-rw-   0        0        0     4500 2023-05-11 03:07:54.000000 hagworm-5.5.5/hagworm/extend/process.py
--rw-rw-rw-   0        0        0      551 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/qrcode.py
--rw-rw-rw-   0        0        0     7235 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/struct.py
--rw-rw-rw-   0        0        0     3758 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/extend/text.py
--rw-rw-rw-   0        0        0     2409 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/trace.py
--rw-rw-rw-   0        0        0     2677 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/transaction.py
--rw-rw-rw-   0        0        0     6411 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/extend/validator.py
-drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.832728 hagworm-5.5.5/hagworm/frame/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/frame/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.839729 hagworm-5.5.5/hagworm/frame/fastapi/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/frame/fastapi/__init__.py
--rw-rw-rw-   0        0        0     8148 2023-05-22 01:25:41.000000 hagworm-5.5.5/hagworm/frame/fastapi/base.py
--rw-rw-rw-   0        0        0     8494 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/frame/fastapi/field.py
--rw-rw-rw-   0        0        0     1389 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/frame/fastapi/model.py
--rw-rw-rw-   0        0        0     1000 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/frame/fastapi/response.py
--rw-rw-rw-   0        0        0     1304 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/frame/gunicorn.py
--rw-rw-rw-   0        0        0     3846 2023-05-11 03:07:54.000000 hagworm-5.5.5/hagworm/frame/stress_tests.py
-drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.842729 hagworm-5.5.5/hagworm/static/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/static/__init__.py
--rw-rw-rw-   0        0        0   208075 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/static/cacert.pem
-drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.843728 hagworm-5.5.5/hagworm/third/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/third/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.846728 hagworm-5.5.5/hagworm/third/consul/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/third/consul/__init__.py
--rw-rw-rw-   0        0        0     1288 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/third/consul/config.py
-drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.852729 hagworm-5.5.5/hagworm/third/rabbitmq/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.5/hagworm/third/rabbitmq/__init__.py
--rw-rw-rw-   0        0        0     3564 2023-05-07 00:52:16.000000 hagworm-5.5.5/hagworm/third/rabbitmq/consume.py
--rw-rw-rw-   0        0        0     5183 2023-05-20 03:08:12.000000 hagworm-5.5.5/hagworm/third/rabbitmq/publish.py
--rw-rw-rw-   0        0        0     5743 2023-05-20 02:53:42.000000 hagworm-5.5.5/hagworm/third/rabbitmq/rpc.py
-drwxrwxrwx   0        0        0        0 2023-05-22 03:51:14.771730 hagworm-5.5.5/hagworm.egg-info/
--rw-rw-rw-   0        0        0     7508 2023-05-22 03:51:14.000000 hagworm-5.5.5/hagworm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2195 2023-05-22 03:51:14.000000 hagworm-5.5.5/hagworm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 03:51:14.000000 hagworm-5.5.5/hagworm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      724 2023-05-22 03:51:14.000000 hagworm-5.5.5/hagworm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-22 03:51:14.000000 hagworm-5.5.5/hagworm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 03:51:14.854727 hagworm-5.5.5/setup.cfg
--rw-rw-rw-   0        0        0     2401 2023-05-22 03:46:54.000000 hagworm-5.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 05:41:25.946450 hagworm-5.5.6/
+-rw-rw-rw-   0        0        0    11362 2023-03-01 02:07:14.000000 hagworm-5.5.6/LICENSE
+-rw-rw-rw-   0        0        0     7508 2023-05-23 05:41:25.946450 hagworm-5.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6065 2023-04-08 01:06:26.000000 hagworm-5.5.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 05:41:25.825451 hagworm-5.5.6/c_extend/
+-rw-rw-rw-   0        0        0      847 2023-03-01 02:07:14.000000 hagworm-5.5.6/c_extend/math.c
+drwxrwxrwx   0        0        0        0 2023-05-23 05:41:25.828450 hagworm-5.5.6/example/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.6/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 05:41:25.835451 hagworm-5.5.6/example/fastapi_demo/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.6/example/fastapi_demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 05:41:25.838450 hagworm-5.5.6/example/fastapi_demo/controller/
+-rw-rw-rw-   0        0        0      211 2023-03-01 02:07:14.000000 hagworm-5.5.6/example/fastapi_demo/controller/__init__.py
+-rw-rw-rw-   0        0        0      397 2023-03-01 02:07:14.000000 hagworm-5.5.6/example/fastapi_demo/controller/home.py
+-rw-rw-rw-   0        0        0      888 2023-05-11 03:07:54.000000 hagworm-5.5.6/example/fastapi_demo/gunicorn.config.py
+-rw-rw-rw-   0        0        0     1431 2023-05-17 08:11:13.000000 hagworm-5.5.6/example/fastapi_demo/main.py
+drwxrwxrwx   0        0        0        0 2023-05-23 05:41:25.840449 hagworm-5.5.6/example/fastapi_demo/model/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.6/example/fastapi_demo/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 05:41:25.842449 hagworm-5.5.6/example/fastapi_demo/service/
+-rw-rw-rw-   0        0        0     3496 2023-05-22 00:30:47.000000 hagworm-5.5.6/example/fastapi_demo/service/__init__.py
+-rw-rw-rw-   0        0        0     2096 2023-03-01 02:07:14.000000 hagworm-5.5.6/example/fastapi_demo/setting.py
+-rw-rw-rw-   0        0        0      800 2023-05-11 03:07:54.000000 hagworm-5.5.6/example/main_test.py
+drwxrwxrwx   0        0        0        0 2023-05-23 05:41:25.844449 hagworm-5.5.6/hagworm/
+-rw-rw-rw-   0        0        0      495 2023-05-23 05:37:41.000000 hagworm-5.5.6/hagworm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 05:41:25.886451 hagworm-5.5.6/hagworm/extend/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 05:41:25.918448 hagworm-5.5.6/hagworm/extend/asyncio/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/extend/asyncio/__init__.py
+-rw-rw-rw-   0        0        0    16802 2023-05-07 00:52:16.000000 hagworm-5.5.6/hagworm/extend/asyncio/base.py
+-rw-rw-rw-   0        0        0     4988 2023-05-07 00:52:16.000000 hagworm-5.5.6/hagworm/extend/asyncio/buffer.py
+-rw-rw-rw-   0        0        0     2396 2023-05-11 03:07:54.000000 hagworm-5.5.6/hagworm/extend/asyncio/command.py
+-rw-rw-rw-   0        0        0     3194 2023-05-07 00:52:16.000000 hagworm-5.5.6/hagworm/extend/asyncio/event.py
+-rw-rw-rw-   0        0        0     1370 2023-05-07 00:52:16.000000 hagworm-5.5.6/hagworm/extend/asyncio/file.py
+-rw-rw-rw-   0        0        0     4232 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/extend/asyncio/future.py
+-rw-rw-rw-   0        0        0     2603 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/extend/asyncio/mail.py
+-rw-rw-rw-   0        0        0     3897 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/extend/asyncio/mongo.py
+-rw-rw-rw-   0        0        0    15022 2023-05-07 00:52:16.000000 hagworm-5.5.6/hagworm/extend/asyncio/mysql.py
+-rw-rw-rw-   0        0        0    13489 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/extend/asyncio/net.py
+-rw-rw-rw-   0        0        0     4149 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/extend/asyncio/ntp.py
+-rw-rw-rw-   0        0        0     1570 2023-05-20 02:55:55.000000 hagworm-5.5.6/hagworm/extend/asyncio/pool.py
+-rw-rw-rw-   0        0        0    12507 2023-05-22 03:45:54.000000 hagworm-5.5.6/hagworm/extend/asyncio/redis.py
+-rw-rw-rw-   0        0        0     7279 2023-05-11 03:07:54.000000 hagworm-5.5.6/hagworm/extend/asyncio/socket.py
+-rw-rw-rw-   0        0        0     6170 2023-04-11 07:28:18.000000 hagworm-5.5.6/hagworm/extend/asyncio/task.py
+-rw-rw-rw-   0        0        0     1360 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/extend/asyncio/transaction.py
+-rw-rw-rw-   0        0        0     3792 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/extend/asyncio/zmq.py
+-rw-rw-rw-   0        0        0    22623 2023-05-11 03:07:54.000000 hagworm-5.5.6/hagworm/extend/base.py
+-rw-rw-rw-   0        0        0     2365 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/extend/cache.py
+-rw-rw-rw-   0        0        0     1839 2023-05-07 00:52:16.000000 hagworm-5.5.6/hagworm/extend/compile.py
+-rw-rw-rw-   0        0        0     3857 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/extend/config.py
+-rw-rw-rw-   0        0        0     1487 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/extend/crypto.py
+-rw-rw-rw-   0        0        0     1792 2023-05-07 00:52:16.000000 hagworm-5.5.6/hagworm/extend/error.py
+-rw-rw-rw-   0        0        0     1220 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/extend/event.py
+-rw-rw-rw-   0        0        0     4558 2023-05-07 00:52:16.000000 hagworm-5.5.6/hagworm/extend/igraph.py
+-rw-rw-rw-   0        0        0     2326 2023-05-07 00:52:16.000000 hagworm-5.5.6/hagworm/extend/interface.py
+-rw-rw-rw-   0        0        0    14870 2023-05-13 05:06:56.000000 hagworm-5.5.6/hagworm/extend/logging.py
+-rw-rw-rw-   0        0        0     1791 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/extend/media.py
+-rw-rw-rw-   0        0        0     1603 2023-05-10 07:58:09.000000 hagworm-5.5.6/hagworm/extend/metaclass.py
+-rw-rw-rw-   0        0        0     4500 2023-05-11 03:07:54.000000 hagworm-5.5.6/hagworm/extend/process.py
+-rw-rw-rw-   0        0        0      551 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/extend/qrcode.py
+-rw-rw-rw-   0        0        0     7235 2023-05-07 00:52:16.000000 hagworm-5.5.6/hagworm/extend/struct.py
+-rw-rw-rw-   0        0        0     3758 2023-05-07 00:52:16.000000 hagworm-5.5.6/hagworm/extend/text.py
+-rw-rw-rw-   0        0        0     2409 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/extend/trace.py
+-rw-rw-rw-   0        0        0     2677 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/extend/transaction.py
+-rw-rw-rw-   0        0        0     6411 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/extend/validator.py
+drwxrwxrwx   0        0        0        0 2023-05-23 05:41:25.923453 hagworm-5.5.6/hagworm/frame/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/frame/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 05:41:25.932449 hagworm-5.5.6/hagworm/frame/fastapi/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/frame/fastapi/__init__.py
+-rw-rw-rw-   0        0        0     8148 2023-05-22 01:25:41.000000 hagworm-5.5.6/hagworm/frame/fastapi/base.py
+-rw-rw-rw-   0        0        0     8494 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/frame/fastapi/field.py
+-rw-rw-rw-   0        0        0     1389 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/frame/fastapi/model.py
+-rw-rw-rw-   0        0        0     1000 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/frame/fastapi/response.py
+-rw-rw-rw-   0        0        0     1304 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/frame/gunicorn.py
+-rw-rw-rw-   0        0        0     3846 2023-05-11 03:07:54.000000 hagworm-5.5.6/hagworm/frame/stress_tests.py
+drwxrwxrwx   0        0        0        0 2023-05-23 05:41:25.935450 hagworm-5.5.6/hagworm/static/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/static/__init__.py
+-rw-rw-rw-   0        0        0   208075 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/static/cacert.pem
+drwxrwxrwx   0        0        0        0 2023-05-23 05:41:25.937449 hagworm-5.5.6/hagworm/third/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/third/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 05:41:25.944449 hagworm-5.5.6/hagworm/third/rabbitmq/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.6/hagworm/third/rabbitmq/__init__.py
+-rw-rw-rw-   0        0        0     3564 2023-05-07 00:52:16.000000 hagworm-5.5.6/hagworm/third/rabbitmq/consume.py
+-rw-rw-rw-   0        0        0     5183 2023-05-20 03:08:12.000000 hagworm-5.5.6/hagworm/third/rabbitmq/publish.py
+-rw-rw-rw-   0        0        0     5743 2023-05-20 02:53:42.000000 hagworm-5.5.6/hagworm/third/rabbitmq/rpc.py
+drwxrwxrwx   0        0        0        0 2023-05-23 05:41:25.852451 hagworm-5.5.6/hagworm.egg-info/
+-rw-rw-rw-   0        0        0     7508 2023-05-23 05:41:25.000000 hagworm-5.5.6/hagworm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2100 2023-05-23 05:41:25.000000 hagworm-5.5.6/hagworm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 05:41:25.000000 hagworm-5.5.6/hagworm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      683 2023-05-23 05:41:25.000000 hagworm-5.5.6/hagworm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-23 05:41:25.000000 hagworm-5.5.6/hagworm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 05:41:25.946450 hagworm-5.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     2334 2023-05-23 05:36:51.000000 hagworm-5.5.6/setup.py
```

### Comparing `hagworm-5.5.5/LICENSE` & `hagworm-5.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/PKG-INFO` & `hagworm-5.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.5.5
+Version: 5.5.6
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Description: # Hagworm
```

### Comparing `hagworm-5.5.5/README.md` & `hagworm-5.5.6/README.md`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/c_extend/math.c` & `hagworm-5.5.6/c_extend/math.c`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/example/fastapi_demo/gunicorn.config.py` & `hagworm-5.5.6/example/fastapi_demo/gunicorn.config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/example/fastapi_demo/main.py` & `hagworm-5.5.6/example/fastapi_demo/main.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/example/fastapi_demo/service/__init__.py` & `hagworm-5.5.6/example/fastapi_demo/service/__init__.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/example/fastapi_demo/setting.py` & `hagworm-5.5.6/example/fastapi_demo/setting.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/example/main_test.py` & `hagworm-5.5.6/example/main_test.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/asyncio/base.py` & `hagworm-5.5.6/hagworm/extend/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/asyncio/buffer.py` & `hagworm-5.5.6/hagworm/extend/asyncio/buffer.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/asyncio/command.py` & `hagworm-5.5.6/hagworm/extend/asyncio/command.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/asyncio/event.py` & `hagworm-5.5.6/hagworm/extend/asyncio/event.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/asyncio/file.py` & `hagworm-5.5.6/hagworm/extend/asyncio/file.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/asyncio/future.py` & `hagworm-5.5.6/hagworm/extend/asyncio/future.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/asyncio/mail.py` & `hagworm-5.5.6/hagworm/extend/asyncio/mail.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/asyncio/mongo.py` & `hagworm-5.5.6/hagworm/extend/asyncio/mongo.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/asyncio/mysql.py` & `hagworm-5.5.6/hagworm/extend/asyncio/mysql.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/asyncio/net.py` & `hagworm-5.5.6/hagworm/extend/asyncio/net.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/asyncio/ntp.py` & `hagworm-5.5.6/hagworm/extend/asyncio/ntp.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/asyncio/pool.py` & `hagworm-5.5.6/hagworm/extend/asyncio/pool.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/asyncio/redis.py` & `hagworm-5.5.6/hagworm/extend/asyncio/redis.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/asyncio/socket.py` & `hagworm-5.5.6/hagworm/extend/asyncio/socket.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/asyncio/task.py` & `hagworm-5.5.6/hagworm/extend/asyncio/task.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/asyncio/transaction.py` & `hagworm-5.5.6/hagworm/extend/asyncio/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/asyncio/zmq.py` & `hagworm-5.5.6/hagworm/extend/asyncio/zmq.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/base.py` & `hagworm-5.5.6/hagworm/extend/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/cache.py` & `hagworm-5.5.6/hagworm/extend/cache.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/compile.py` & `hagworm-5.5.6/hagworm/extend/compile.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/config.py` & `hagworm-5.5.6/hagworm/extend/config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/crypto.py` & `hagworm-5.5.6/hagworm/extend/crypto.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/error.py` & `hagworm-5.5.6/hagworm/extend/error.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/event.py` & `hagworm-5.5.6/hagworm/extend/event.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/igraph.py` & `hagworm-5.5.6/hagworm/extend/igraph.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/interface.py` & `hagworm-5.5.6/hagworm/extend/interface.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/logging.py` & `hagworm-5.5.6/hagworm/extend/logging.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/media.py` & `hagworm-5.5.6/hagworm/extend/media.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/metaclass.py` & `hagworm-5.5.6/hagworm/extend/metaclass.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/process.py` & `hagworm-5.5.6/hagworm/extend/process.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/qrcode.py` & `hagworm-5.5.6/hagworm/extend/qrcode.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/struct.py` & `hagworm-5.5.6/hagworm/extend/struct.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/text.py` & `hagworm-5.5.6/hagworm/extend/text.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/trace.py` & `hagworm-5.5.6/hagworm/extend/trace.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/transaction.py` & `hagworm-5.5.6/hagworm/extend/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/extend/validator.py` & `hagworm-5.5.6/hagworm/extend/validator.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/frame/fastapi/base.py` & `hagworm-5.5.6/hagworm/frame/fastapi/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/frame/fastapi/field.py` & `hagworm-5.5.6/hagworm/frame/fastapi/field.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/frame/fastapi/model.py` & `hagworm-5.5.6/hagworm/frame/fastapi/model.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/frame/fastapi/response.py` & `hagworm-5.5.6/hagworm/frame/fastapi/response.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/frame/gunicorn.py` & `hagworm-5.5.6/hagworm/frame/gunicorn.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/frame/stress_tests.py` & `hagworm-5.5.6/hagworm/frame/stress_tests.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/static/cacert.pem` & `hagworm-5.5.6/hagworm/static/cacert.pem`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/third/rabbitmq/consume.py` & `hagworm-5.5.6/hagworm/third/rabbitmq/consume.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/third/rabbitmq/publish.py` & `hagworm-5.5.6/hagworm/third/rabbitmq/publish.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm/third/rabbitmq/rpc.py` & `hagworm-5.5.6/hagworm/third/rabbitmq/rpc.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.5/hagworm.egg-info/PKG-INFO` & `hagworm-5.5.6/hagworm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.5.5
+Version: 5.5.6
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Description: # Hagworm
```

### Comparing `hagworm-5.5.5/hagworm.egg-info/SOURCES.txt` & `hagworm-5.5.6/hagworm.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 hagworm/extend/trace.py
 hagworm/extend/transaction.py
 hagworm/extend/validator.py
 hagworm/extend/asyncio/__init__.py
 hagworm/extend/asyncio/base.py
 hagworm/extend/asyncio/buffer.py
 hagworm/extend/asyncio/command.py
-hagworm/extend/asyncio/etcd.py
 hagworm/extend/asyncio/event.py
 hagworm/extend/asyncio/file.py
 hagworm/extend/asyncio/future.py
 hagworm/extend/asyncio/mail.py
 hagworm/extend/asyncio/mongo.py
 hagworm/extend/asyncio/mysql.py
 hagworm/extend/asyncio/net.py
@@ -64,13 +63,11 @@
 hagworm/frame/fastapi/base.py
 hagworm/frame/fastapi/field.py
 hagworm/frame/fastapi/model.py
 hagworm/frame/fastapi/response.py
 hagworm/static/__init__.py
 hagworm/static/cacert.pem
 hagworm/third/__init__.py
-hagworm/third/consul/__init__.py
-hagworm/third/consul/config.py
 hagworm/third/rabbitmq/__init__.py
 hagworm/third/rabbitmq/consume.py
 hagworm/third/rabbitmq/publish.py
 hagworm/third/rabbitmq/rpc.py
```

### Comparing `hagworm-5.5.5/setup.py` & `hagworm-5.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         r'PyYAML==6.0',
         r'SQLAlchemy==2.0.14',
         r'coredis==2.3.2',
         r'aiohttp==3.8.4',
         r'aiomysql==0.1.1',
         r'aiosmtplib==2.0.1',
         r'aio-pika==9.0.7',
-        r'async-etcd3gw==0.8',
         r'cachetools==5.3.0',
         r'confluent-kafka==2.1.1',
         r'cryptography==40.0.2',
         r'elasticsearch==8.1.1',
         r'fastapi==0.95.2',
         r'fastapi-health==0.4.0',
         r'gunicorn==20.1.0',
@@ -55,15 +54,14 @@
         r'ntplib==0.4.0',
         r'numpy==1.24.3',
         r'psutil==5.9.5',
         r'pyahocorasick==2.0.0',
         r'pytest-asyncio==0.21.0',
         r'python-dateutil==2.8.2',
         r'python-stdnum==1.18',
-        r'python-consul2==0.1.5',
         r'python-multipart==0.0.6',
         r'pyzmq==25.0.2',
         r'qrcode==7.4.2',
         r'texttable==1.6.7',
         r'ujson==5.7.0',
         r'uvicorn[standard]==0.22.0',
         r'uvloop==0.17.0;sys_platform!="win32"',
```

