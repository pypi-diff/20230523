# Comparing `tmp/blaster-server-0.0.431b0.tar.gz` & `tmp/blaster-server-0.0.432.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaster-server-0.0.431b0.tar", last modified: Wed May 17 08:28:05 2023, max compression
+gzip compressed data, was "blaster-server-0.0.432.tar", last modified: Mon May 22 22:34:58 2023, max compression
```

## Comparing `blaster-server-0.0.431b0.tar` & `blaster-server-0.0.432.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-17 08:28:05.418887 blaster-server-0.0.431b0/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1061 2019-07-03 19:03:00.000000 blaster-server-0.0.431b0/LICENSE.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2022-11-07 18:47:07.000000 blaster-server-0.0.431b0/MANIFEST.in
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-05-17 08:28:05.418887 blaster-server-0.0.431b0/PKG-INFO
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2620 2022-11-14 12:45:11.000000 blaster-server-0.0.431b0/README.md
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2021-10-05 11:27:02.000000 blaster-server-0.0.431b0/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-17 08:28:05.414886 blaster-server-0.0.431b0/blaster/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      875 2023-01-09 13:10:46.000000 blaster-server-0.0.431b0/blaster/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-17 08:28:05.414886 blaster-server-0.0.431b0/blaster/cloud/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2022-11-09 17:29:08.000000 blaster-server-0.0.431b0/blaster/cloud/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3215 2023-04-30 12:43:59.000000 blaster-server-0.0.431b0/blaster/cloud/analytics.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-17 08:28:05.414886 blaster-server-0.0.431b0/blaster/cloud/aws/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       78 2019-07-03 19:03:00.000000 blaster-server-0.0.431b0/blaster/cloud/aws/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2022-12-01 11:30:06.000000 blaster-server-0.0.431b0/blaster/cloud/aws/ses_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-10 23:46:29.000000 blaster-server-0.0.431b0/blaster/cloud/push_tasks.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-06 07:07:21.000000 blaster-server-0.0.431b0/blaster/cloud/storage.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3828 2023-05-15 14:10:32.000000 blaster-server-0.0.431b0/blaster/config.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-01-28 12:57:17.000000 blaster-server-0.0.431b0/blaster/connection_pool.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       99 2020-11-22 14:37:38.000000 blaster-server-0.0.431b0/blaster/constants.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5290 2023-05-15 14:09:30.000000 blaster-server-0.0.431b0/blaster/logging.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62877 2023-05-10 08:42:24.000000 blaster-server-0.0.431b0/blaster/mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15728 2023-05-17 08:23:45.000000 blaster-server-0.0.431b0/blaster/schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    36583 2023-04-18 10:02:10.000000 blaster-server-0.0.431b0/blaster/server.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    46443 2023-05-15 14:15:15.000000 blaster-server-0.0.431b0/blaster/tools.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-17 08:28:05.414886 blaster-server-0.0.431b0/blaster/utils/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.431b0/blaster/utils/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-17 08:28:05.414886 blaster-server-0.0.431b0/blaster/utils/data/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2022-11-08 15:22:07.000000 blaster-server-0.0.431b0/blaster/utils/data/countries.json
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2022-12-01 10:20:50.000000 blaster-server-0.0.431b0/blaster/utils/data/mime_types.json
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-14 10:13:13.000000 blaster-server-0.0.431b0/blaster/utils/data_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-01-07 12:42:21.000000 blaster-server-0.0.431b0/blaster/utils/events.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-03-30 16:36:26.000000 blaster-server-0.0.431b0/blaster/utils/fork.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1076 2023-02-21 07:52:48.000000 blaster-server-0.0.431b0/blaster/utils/lat_long_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5564 2023-05-09 13:55:03.000000 blaster-server-0.0.431b0/blaster/utils/phone_number_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     6773 2020-12-14 07:56:42.000000 blaster-server-0.0.431b0/blaster/utils/xss_html.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-17 08:28:05.414886 blaster-server-0.0.431b0/blaster/websocket/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1022 2019-07-03 19:03:00.000000 blaster-server-0.0.431b0/blaster/websocket/__init__.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12874 2019-07-03 19:03:00.000000 blaster-server-0.0.431b0/blaster/websocket/_abnf.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2022-01-06 11:42:20.000000 blaster-server-0.0.431b0/blaster/websocket/_app.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    16360 2019-07-03 19:03:00.000000 blaster-server-0.0.431b0/blaster/websocket/_core.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2141 2019-07-03 19:03:00.000000 blaster-server-0.0.431b0/blaster/websocket/_exceptions.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     4793 2019-07-03 19:03:00.000000 blaster-server-0.0.431b0/blaster/websocket/_handshake.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7288 2019-07-03 19:03:00.000000 blaster-server-0.0.431b0/blaster/websocket/_http.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1870 2019-07-03 19:03:00.000000 blaster-server-0.0.431b0/blaster/websocket/_logging.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3623 2019-07-03 19:03:00.000000 blaster-server-0.0.431b0/blaster/websocket/_socket.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1550 2019-07-03 19:03:00.000000 blaster-server-0.0.431b0/blaster/websocket/_ssl_compat.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3670 2019-07-03 19:03:00.000000 blaster-server-0.0.431b0/blaster/websocket/_url.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3632 2019-07-03 19:03:00.000000 blaster-server-0.0.431b0/blaster/websocket/_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12758 2021-10-03 12:23:56.000000 blaster-server-0.0.431b0/blaster/websocket/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-17 08:28:05.414886 blaster-server-0.0.431b0/blaster/websocket/tests/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.431b0/blaster/websocket/tests/__init__.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    26115 2019-07-03 19:03:00.000000 blaster-server-0.0.431b0/blaster/websocket/tests/test_websocket.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-17 08:28:05.418887 blaster-server-0.0.431b0/blaster_server.egg-info/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      851 2023-05-17 08:28:05.000000 blaster-server-0.0.431b0/blaster_server.egg-info/PKG-INFO
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1682 2023-05-17 08:28:05.000000 blaster-server-0.0.431b0/blaster_server.egg-info/SOURCES.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        1 2023-05-17 08:28:05.000000 blaster-server-0.0.431b0/blaster_server.egg-info/dependency_links.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      206 2023-05-17 08:28:05.000000 blaster-server-0.0.431b0/blaster_server.egg-info/requires.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       41 2023-05-17 08:28:05.000000 blaster-server-0.0.431b0/blaster_server.egg-info/top_level.txt
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-17 08:28:05.418887 blaster-server-0.0.431b0/examples/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.431b0/examples/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2022-01-06 11:42:20.000000 blaster-server-0.0.431b0/examples/fast_api_test.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      636 2019-07-03 19:03:00.000000 blaster-server-0.0.431b0/examples/gevent_wsgi_test.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      233 2021-10-04 14:48:01.000000 blaster-server-0.0.431b0/examples/meinheld_flask.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1743 2022-06-17 17:10:40.000000 blaster-server-0.0.431b0/examples/mongo_ormexample.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2022-11-14 12:13:43.000000 blaster-server-0.0.431b0/examples/simple_examples.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1088 2019-07-03 19:03:00.000000 blaster-server-0.0.431b0/examples/test_chat_room.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      614 2021-02-24 01:34:32.000000 blaster-server-0.0.431b0/examples/tornado_hello_world.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      791 2021-02-24 01:20:44.000000 blaster-server-0.0.431b0/examples/wheezy_hello.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       79 2023-05-17 08:28:05.418887 blaster-server-0.0.431b0/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1540 2023-05-17 08:24:26.000000 blaster-server-0.0.431b0/setup.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-17 08:28:05.418887 blaster-server-0.0.431b0/test/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2022-07-26 21:35:40.000000 blaster-server-0.0.431b0/test/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-01-07 00:03:08.000000 blaster-server-0.0.431b0/test/test_mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-17 08:26:43.000000 blaster-server-0.0.431b0/test/test_schema.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5457 2022-12-09 21:19:51.000000 blaster-server-0.0.431b0/test/test_tools.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-16 18:26:08.000000 blaster-server-0.0.431b0/test/test_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      615 2021-02-24 11:15:27.000000 blaster-server-0.0.431b0/test/timeit_snippets.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.216565 blaster-server-0.0.432/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1061 2019-07-03 19:03:00.000000 blaster-server-0.0.432/LICENSE.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2022-11-07 18:47:07.000000 blaster-server-0.0.432/MANIFEST.in
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-05-22 22:34:58.216565 blaster-server-0.0.432/PKG-INFO
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2620 2022-11-14 12:45:11.000000 blaster-server-0.0.432/README.md
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2021-10-05 11:27:02.000000 blaster-server-0.0.432/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.212565 blaster-server-0.0.432/blaster/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      875 2023-01-09 13:10:46.000000 blaster-server-0.0.432/blaster/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.212565 blaster-server-0.0.432/blaster/cloud/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2022-11-09 17:29:08.000000 blaster-server-0.0.432/blaster/cloud/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3215 2023-04-30 12:43:59.000000 blaster-server-0.0.432/blaster/cloud/analytics.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.212565 blaster-server-0.0.432/blaster/cloud/aws/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       78 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/cloud/aws/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2022-12-01 11:30:06.000000 blaster-server-0.0.432/blaster/cloud/aws/ses_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-10 23:46:29.000000 blaster-server-0.0.432/blaster/cloud/push_tasks.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-19 10:42:50.000000 blaster-server-0.0.432/blaster/cloud/storage.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3828 2023-05-15 14:10:32.000000 blaster-server-0.0.432/blaster/config.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-01-28 12:57:17.000000 blaster-server-0.0.432/blaster/connection_pool.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       99 2020-11-22 14:37:38.000000 blaster-server-0.0.432/blaster/constants.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5290 2023-05-15 14:09:30.000000 blaster-server-0.0.432/blaster/logging.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62877 2023-05-10 08:42:24.000000 blaster-server-0.0.432/blaster/mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15728 2023-05-17 08:23:45.000000 blaster-server-0.0.432/blaster/schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    38823 2023-05-22 20:14:53.000000 blaster-server-0.0.432/blaster/server.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    46589 2023-05-22 20:12:00.000000 blaster-server-0.0.432/blaster/tools.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.212565 blaster-server-0.0.432/blaster/utils/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/utils/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.212565 blaster-server-0.0.432/blaster/utils/data/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2022-11-08 15:22:07.000000 blaster-server-0.0.432/blaster/utils/data/countries.json
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2022-12-01 10:20:50.000000 blaster-server-0.0.432/blaster/utils/data/mime_types.json
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-14 10:13:13.000000 blaster-server-0.0.432/blaster/utils/data_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-01-07 12:42:21.000000 blaster-server-0.0.432/blaster/utils/events.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-03-30 16:36:26.000000 blaster-server-0.0.432/blaster/utils/fork.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1076 2023-02-21 07:52:48.000000 blaster-server-0.0.432/blaster/utils/lat_long_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5564 2023-05-09 13:55:03.000000 blaster-server-0.0.432/blaster/utils/phone_number_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     6773 2020-12-14 07:56:42.000000 blaster-server-0.0.432/blaster/utils/xss_html.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.212565 blaster-server-0.0.432/blaster/websocket/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1022 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/__init__.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12874 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/_abnf.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2022-01-06 11:42:20.000000 blaster-server-0.0.432/blaster/websocket/_app.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    16360 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/_core.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2141 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/_exceptions.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     4793 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/_handshake.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7288 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/_http.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1870 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/_logging.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3623 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/_socket.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1550 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/_ssl_compat.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3670 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/_url.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3632 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12758 2021-10-03 12:23:56.000000 blaster-server-0.0.432/blaster/websocket/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.212565 blaster-server-0.0.432/blaster/websocket/tests/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/tests/__init__.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    26115 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/tests/test_websocket.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.216565 blaster-server-0.0.432/blaster_server.egg-info/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      849 2023-05-22 22:34:58.000000 blaster-server-0.0.432/blaster_server.egg-info/PKG-INFO
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1682 2023-05-22 22:34:58.000000 blaster-server-0.0.432/blaster_server.egg-info/SOURCES.txt
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        1 2023-05-22 22:34:58.000000 blaster-server-0.0.432/blaster_server.egg-info/dependency_links.txt
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      206 2023-05-22 22:34:58.000000 blaster-server-0.0.432/blaster_server.egg-info/requires.txt
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       41 2023-05-22 22:34:58.000000 blaster-server-0.0.432/blaster_server.egg-info/top_level.txt
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.216565 blaster-server-0.0.432/examples/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.432/examples/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2022-01-06 11:42:20.000000 blaster-server-0.0.432/examples/fast_api_test.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      636 2019-07-03 19:03:00.000000 blaster-server-0.0.432/examples/gevent_wsgi_test.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      233 2021-10-04 14:48:01.000000 blaster-server-0.0.432/examples/meinheld_flask.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1743 2022-06-17 17:10:40.000000 blaster-server-0.0.432/examples/mongo_ormexample.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2022-11-14 12:13:43.000000 blaster-server-0.0.432/examples/simple_examples.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1088 2019-07-03 19:03:00.000000 blaster-server-0.0.432/examples/test_chat_room.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      614 2021-02-24 01:34:32.000000 blaster-server-0.0.432/examples/tornado_hello_world.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      791 2021-02-24 01:20:44.000000 blaster-server-0.0.432/examples/wheezy_hello.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       79 2023-05-22 22:34:58.216565 blaster-server-0.0.432/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1539 2023-05-17 20:32:09.000000 blaster-server-0.0.432/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.216565 blaster-server-0.0.432/test/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2022-07-26 21:35:40.000000 blaster-server-0.0.432/test/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-01-07 00:03:08.000000 blaster-server-0.0.432/test/test_mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-17 08:26:43.000000 blaster-server-0.0.432/test/test_schema.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5457 2022-12-09 21:19:51.000000 blaster-server-0.0.432/test/test_tools.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-16 18:26:08.000000 blaster-server-0.0.432/test/test_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      615 2021-02-24 11:15:27.000000 blaster-server-0.0.432/test/timeit_snippets.py
```

### Comparing `blaster-server-0.0.431b0/LICENSE.txt` & `blaster-server-0.0.432/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/PKG-INFO` & `blaster-server-0.0.432/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.431b0
+Version: 0.0.432
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.431b0/README.md` & `blaster-server-0.0.432/README.md`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/__init__.py` & `blaster-server-0.0.432/blaster/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/cloud/analytics.py` & `blaster-server-0.0.432/blaster/cloud/analytics.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/cloud/aws/ses_utils.py` & `blaster-server-0.0.432/blaster/cloud/aws/ses_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/cloud/push_tasks.py` & `blaster-server-0.0.432/blaster/cloud/push_tasks.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/cloud/storage.py` & `blaster-server-0.0.432/blaster/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/config.py` & `blaster-server-0.0.432/blaster/config.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/connection_pool.py` & `blaster-server-0.0.432/blaster/connection_pool.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/logging.py` & `blaster-server-0.0.432/blaster/logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/mongo_orm.py` & `blaster-server-0.0.432/blaster/mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/schema.py` & `blaster-server-0.0.432/blaster/schema.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/server.py` & `blaster-server-0.0.432/blaster/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1245,7 +1245,19 @@
 	# sends handshake automatically
 	ws = WebSocketServerHandler(req.sock)
 	ws.do_handshake(req.HEADERS())
 	return ws
 
 
 Request.set_arg_type_hook(WebSocketServerHandler, _get_web_socket_handler)
+
+
+# Utils
+
+MOILE_USER_AGENT_REGEX = re.compile(r"(android|bb\\d+|meego).+mobile|avantgo|bada\\/|blackberry|blazer|compal|elaine|fennec|hiptop|iemobile|ip(hone|od)|iris|kindle|lge |maemo|midp|mmp|mobile.+firefox|netfront|opera m(ob|in)i|palm( os)?|phone|p(ixi|re)\\/|plucker|pocket|psp|series(4|6)0|symbian|treo|up\\.(browser|link)|vodafone|wap|windows ce|xda|xiino", re.I|re.M)
+
+MOILE_USER_AGENT_REGEX2 = re.compile(r"1207|6310|6590|3gso|4thp|50[1-6]i|770s|802s|a wa|abac|ac(er|oo|s\\-)|ai(ko|rn)|al(av|ca|co)|amoi|an(ex|ny|yw)|aptu|ar(ch|go)|as(te|us)|attw|au(di|\\-m|r |s )|avan|be(ck|ll|nq)|bi(lb|rd)|bl(ac|az)|br(e|v)w|bumb|bw\\-(n|u)|c55\\/|capi|ccwa|cdm\\-|cell|chtm|cldc|cmd\\-|co(mp|nd)|craw|da(it|ll|ng)|dbte|dc\\-s|devi|dica|dmob|do(c|p)o|ds(12|\\-d)|el(49|ai)|em(l2|ul)|er(ic|k0)|esl8|ez([4-7]0|os|wa|ze)|fetc|fly(\\-|_)|g1 u|g560|gene|gf\\-5|g\\-mo|go(\\.w|od)|gr(ad|un)|haie|hcit|hd\\-(m|p|t)|hei\\-|hi(pt|ta)|hp( i|ip)|hs\\-c|ht(c(\\-| |_|a|g|p|s|t)|tp)|hu(aw|tc)|i\\-(20|go|ma)|i230|iac( |\\-|\\/)|ibro|idea|ig01|ikom|im1k|inno|ipaq|iris|ja(t|v)a|jbro|jemu|jigs|kddi|keji|kgt( |\\/)|klon|kpt |kwc\\-|kyo(c|k)|le(no|xi)|lg( g|\\/(k|l|u)|50|54|\\-[a-w])|libw|lynx|m1\\-w|m3ga|m50\\/|ma(te|ui|xo)|mc(01|21|ca)|m\\-cr|me(rc|ri)|mi(o8|oa|ts)|mmef|mo(01|02|bi|de|do|t(\\-| |o|v)|zz)|mt(50|p1|v )|mwbp|mywa|n10[0-2]|n20[2-3]|n30(0|2)|n50(0|2|5)|n7(0(0|1)|10)|ne((c|m)\\-|on|tf|wf|wg|wt)|nok(6|i)|nzph|o2im|op(ti|wv)|oran|owg1|p800|pan(a|d|t)|pdxg|pg(13|\\-([1-8]|c))|phil|pire|pl(ay|uc)|pn\\-2|po(ck|rt|se)|prox|psio|pt\\-g|qa\\-a|qc(07|12|21|32|60|\\-[2-7]|i\\-)|qtek|r380|r600|raks|rim9|ro(ve|zo)|s55\\/|sa(ge|ma|mm|ms|ny|va)|sc(01|h\\-|oo|p\\-)|sdk\\/|se(c(\\-|0|1)|47|mc|nd|ri)|sgh\\-|shar|sie(\\-|m)|sk\\-0|sl(45|id)|sm(al|ar|b3|it|t5)|so(ft|ny)|sp(01|h\\-|v\\-|v )|sy(01|mb)|t2(18|50)|t6(00|10|18)|ta(gt|lk)|tcl\\-|tdg\\-|tel(i|m)|tim\\-|t\\-mo|to(pl|sh)|ts(70|m\\-|m3|m5)|tx\\-9|up(\\.b|g1|si)|utst|v400|v750|veri|vi(rg|te)|vk(40|5[0-3]|\\-v)|vm40|voda|vulc|vx(52|53|60|61|70|80|81|83|85|98)|w3c(\\-| )|webc|whit|wi(g |nc|nw)|wmlb|wonu|x700|yas\\-|your|zeto|zte\\-", re.I | re.M)
+
+
+def is_mobile_user_agent(user_agent):
+	return MOILE_USER_AGENT_REGEX.search(user_agent) \
+		or MOILE_USER_AGENT_REGEX2.search(user_agent[0:4])
```

### Comparing `blaster-server-0.0.431b0/blaster/tools.py` & `blaster-server-0.0.432/blaster/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1439,18 +1439,18 @@
 	return args_map
 
 
 # PARSE COMMAND LINE ARGUMENTS BY DEFAULT
 CommandLineArgs = parse_cmd_line_arguments()
 
 
-def run_shell(cmd, output_parser=None, shell=False, max_buf=5000, fail=True):
+def run_shell(cmd, output_parser=None, shell=False, max_buf=5000, fail=True, state=None, env=None, **kwargs):
 
 	DEBUG_PRINT_LEVEL > 2 and print(f"#RUNNING: {cmd}")
-	state = DummyObject()
+	state = state if state != None else DummyObject()
 	state.total_output = ""
 	state.total_err = ""
 
 	# keep parsing output
 	def process_output(proc_out, proc_in):
 		while(state.is_running):
 			_out = proc_out.read(1)
@@ -1490,21 +1490,26 @@
 			else:
 				print(_err, end="", flush=True)
 
 	if(isinstance(cmd, str) and not shell):
 		cmd = shlex.split(cmd)
 
 	dup_stdin = os.dup(sys.stdin.fileno()) if shell else subprocess.PIPE
-	proc = subprocess.Popen(
+	_env = os.environ.copy()
+	if(env):
+		_env.update(env)
+
+	state.proc = proc = subprocess.Popen(
 		cmd,
 		stdin=dup_stdin,
 		stdout=subprocess.PIPE,
 		stderr=subprocess.PIPE,
 		shell=shell,
-		env=os.environ.copy()
+		env=_env,
+		**kwargs
 	)
 	state.is_running = True
 
 	# process output reader
 	output_parser_thread = Thread(
 		target=process_output,
 		args=(
@@ -1524,21 +1529,21 @@
 	err_parser_thread.start()
 
 	os.close(dup_stdin) if dup_stdin != subprocess.PIPE else None
 
 	# just keep printing error
 	# wait for process to terminate
 	ret_code = proc.wait()
-	if(ret_code and fail):
-		raise Exception(f"Non zero return code :{ret_code}")
 	state.return_code = ret_code
 	state.is_running = False
-
 	output_parser_thread.join()
 	err_parser_thread.join()
+	state.proc = None
+	if(ret_code and fail):
+		raise Exception(f"Non zero return code :{ret_code}")
 	return state
 
 
 # args is array of strings or array or array of words
 # you can use this to return a bunch of strings to index
 # in elasticsearch with key "search_words"
 def condense_for_search(*args):
```

### Comparing `blaster-server-0.0.431b0/blaster/utils/data/countries.json` & `blaster-server-0.0.432/blaster/utils/data/countries.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/utils/data/mime_types.json` & `blaster-server-0.0.432/blaster/utils/data/mime_types.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/utils/data_utils.py` & `blaster-server-0.0.432/blaster/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/utils/events.py` & `blaster-server-0.0.432/blaster/utils/events.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/utils/fork.py` & `blaster-server-0.0.432/blaster/utils/fork.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/utils/lat_long_utils.py` & `blaster-server-0.0.432/blaster/utils/lat_long_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/utils/phone_number_utils.py` & `blaster-server-0.0.432/blaster/utils/phone_number_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/utils/xss_html.py` & `blaster-server-0.0.432/blaster/utils/xss_html.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/websocket/__init__.py` & `blaster-server-0.0.432/blaster/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/websocket/_abnf.py` & `blaster-server-0.0.432/blaster/websocket/_abnf.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/websocket/_app.py` & `blaster-server-0.0.432/blaster/websocket/_app.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/websocket/_core.py` & `blaster-server-0.0.432/blaster/websocket/_core.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/websocket/_exceptions.py` & `blaster-server-0.0.432/blaster/websocket/_exceptions.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/websocket/_handshake.py` & `blaster-server-0.0.432/blaster/websocket/_handshake.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/websocket/_http.py` & `blaster-server-0.0.432/blaster/websocket/_http.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/websocket/_logging.py` & `blaster-server-0.0.432/blaster/websocket/_logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/websocket/_socket.py` & `blaster-server-0.0.432/blaster/websocket/_socket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/websocket/_ssl_compat.py` & `blaster-server-0.0.432/blaster/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/websocket/_url.py` & `blaster-server-0.0.432/blaster/websocket/_url.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/websocket/_utils.py` & `blaster-server-0.0.432/blaster/websocket/_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/websocket/server.py` & `blaster-server-0.0.432/blaster/websocket/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster/websocket/tests/test_websocket.py` & `blaster-server-0.0.432/blaster/websocket/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/blaster_server.egg-info/PKG-INFO` & `blaster-server-0.0.432/blaster_server.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.431b0
+Version: 0.0.432
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.431b0/blaster_server.egg-info/SOURCES.txt` & `blaster-server-0.0.432/blaster_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/examples/gevent_wsgi_test.py` & `blaster-server-0.0.432/examples/gevent_wsgi_test.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/examples/mongo_ormexample.py` & `blaster-server-0.0.432/examples/mongo_ormexample.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/examples/simple_examples.py` & `blaster-server-0.0.432/examples/simple_examples.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/examples/test_chat_room.py` & `blaster-server-0.0.432/examples/test_chat_room.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/examples/tornado_hello_world.py` & `blaster-server-0.0.432/examples/tornado_hello_world.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/examples/wheezy_hello.py` & `blaster-server-0.0.432/examples/wheezy_hello.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/setup.py` & `blaster-server-0.0.432/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 	name='blaster-server',
 	packages=find_packages() + ["blaster/utils/data"],
-	version='0.0.431b',
+	version='0.0.432',
 	license='MIT',
 	description='Gevent based python server built from scratch for maximum performance',
 	author='Abhinav Reddy',                   # Type in your name
 	author_email='abhinavabcd@gmail.com',      # Type in your E-Mail
 	url='https://github.com/abhinavabcd/blaster',
 	download_url='https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz',
 	keywords=['server', 'superfast', 'Like FastApi or Flask but 10x faster'],
```

### Comparing `blaster-server-0.0.431b0/test/test_mongo_orm.py` & `blaster-server-0.0.432/test/test_mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/test/test_schema.py` & `blaster-server-0.0.432/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/test/test_tools.py` & `blaster-server-0.0.432/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/test/test_utils.py` & `blaster-server-0.0.432/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.431b0/test/timeit_snippets.py` & `blaster-server-0.0.432/test/timeit_snippets.py`

 * *Files identical despite different names*

