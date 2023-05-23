# Comparing `tmp/common-test-29.9.40.tar.gz` & `tmp/common-test-29.9.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-test-29.9.40.tar", last modified: Wed May 10 06:50:37 2023, max compression
+gzip compressed data, was "common-test-29.9.41.tar", last modified: Mon May 15 06:11:16 2023, max compression
```

## Comparing `common-test-29.9.40.tar` & `common-test-29.9.41.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.639226 common-test-29.9.40/
--rw-r--r--   0 edz        (502) staff       (20)      623 2023-05-10 06:50:37.639351 common-test-29.9.40/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.606327 common-test-29.9.40/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 common-test-29.9.40/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.608648 common-test-29.9.40/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 common-test-29.9.40/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     8490 2023-05-09 01:49:15.000000 common-test-29.9.40/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 common-test-29.9.40/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 common-test-29.9.40/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.611263 common-test-29.9.40/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 common-test-29.9.40/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 common-test-29.9.40/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3578 2023-05-08 02:03:18.000000 common-test-29.9.40/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 common-test-29.9.40/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.612283 common-test-29.9.40/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.40/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 common-test-29.9.40/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.615192 common-test-29.9.40/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 common-test-29.9.40/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    17412 2023-05-06 06:06:25.000000 common-test-29.9.40/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)     8662 2023-04-23 07:58:21.000000 common-test-29.9.40/common/data/handle_common.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.619295 common-test-29.9.40/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.40/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3436 2023-04-14 00:29:00.000000 common-test-29.9.40/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 common-test-29.9.40/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 common-test-29.9.40/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 common-test-29.9.40/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 common-test-29.9.40/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.624854 common-test-29.9.40/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 common-test-29.9.40/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 common-test-29.9.40/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11091 2023-05-05 06:58:50.000000 common-test-29.9.40/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-04-14 00:29:00.000000 common-test-29.9.40/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 common-test-29.9.40/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 common-test-29.9.40/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 common-test-29.9.40/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.626320 common-test-29.9.40/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.40/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 common-test-29.9.40/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.630209 common-test-29.9.40/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)     3531 2023-05-08 04:08:54.000000 common-test-29.9.40/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 common-test-29.9.40/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 common-test-29.9.40/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    13650 2023-05-10 06:42:48.000000 common-test-29.9.40/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     5059 2023-05-05 07:02:08.000000 common-test-29.9.40/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     8570 2023-05-08 05:47:33.000000 common-test-29.9.40/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.636839 common-test-29.9.40/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 common-test-29.9.40/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 common-test-29.9.40/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 common-test-29.9.40/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     8263 2023-05-10 00:52:04.000000 common-test-29.9.40/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     6651 2023-05-10 00:52:04.000000 common-test-29.9.40/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     3721 2023-05-04 05:30:58.000000 common-test-29.9.40/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    10894 2023-05-08 02:03:18.000000 common-test-29.9.40/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 common-test-29.9.40/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:00.000000 common-test-29.9.40/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    16835 2023-05-10 05:59:48.000000 common-test-29.9.40/common/plugin/pytest_plugin.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.638935 common-test-29.9.40/common_test.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      623 2023-05-10 06:50:37.000000 common-test-29.9.40/common_test.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1475 2023-05-10 06:50:37.000000 common-test-29.9.40/common_test.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2023-05-10 06:50:37.000000 common-test-29.9.40/common_test.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2023-05-10 06:50:37.000000 common-test-29.9.40/common_test.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      571 2023-05-10 06:50:37.000000 common-test-29.9.40/common_test.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2023-05-10 06:50:37.000000 common-test-29.9.40/common_test.egg-info/top_level.txt
--rw-r--r--   0 edz        (502) staff       (20)      440 2023-05-10 06:50:37.640488 common-test-29.9.40/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1641 2023-05-04 07:57:23.000000 common-test-29.9.40/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-15 06:11:16.321110 common-test-29.9.41/
+-rw-r--r--   0 edz        (502) staff       (20)      623 2023-05-15 06:11:16.321261 common-test-29.9.41/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-15 06:11:16.295292 common-test-29.9.41/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 common-test-29.9.41/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-15 06:11:16.296415 common-test-29.9.41/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 common-test-29.9.41/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     8490 2023-05-09 01:49:15.000000 common-test-29.9.41/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 common-test-29.9.41/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 common-test-29.9.41/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-15 06:11:16.297839 common-test-29.9.41/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 common-test-29.9.41/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 common-test-29.9.41/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3578 2023-05-08 02:03:18.000000 common-test-29.9.41/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 common-test-29.9.41/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-15 06:11:16.298462 common-test-29.9.41/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.41/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 common-test-29.9.41/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-15 06:11:16.299442 common-test-29.9.41/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 common-test-29.9.41/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    17395 2023-05-15 02:25:41.000000 common-test-29.9.41/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)     8661 2023-05-15 02:03:28.000000 common-test-29.9.41/common/data/handle_common.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-15 06:11:16.301402 common-test-29.9.41/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.41/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3954 2023-05-15 02:25:41.000000 common-test-29.9.41/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 common-test-29.9.41/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 common-test-29.9.41/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 common-test-29.9.41/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 common-test-29.9.41/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-15 06:11:16.304436 common-test-29.9.41/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 common-test-29.9.41/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 common-test-29.9.41/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11091 2023-05-05 06:58:50.000000 common-test-29.9.41/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-04-14 00:29:00.000000 common-test-29.9.41/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 common-test-29.9.41/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 common-test-29.9.41/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 common-test-29.9.41/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-15 06:11:16.305019 common-test-29.9.41/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.41/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 common-test-29.9.41/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-15 06:11:16.307479 common-test-29.9.41/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3441 2023-05-15 00:55:54.000000 common-test-29.9.41/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 common-test-29.9.41/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 common-test-29.9.41/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7695 2023-05-10 06:58:57.000000 common-test-29.9.41/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     5866 2023-05-15 02:26:35.000000 common-test-29.9.41/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     8570 2023-05-08 05:47:33.000000 common-test-29.9.41/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-15 06:11:16.317769 common-test-29.9.41/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 common-test-29.9.41/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 common-test-29.9.41/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 common-test-29.9.41/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     8119 2023-05-12 08:10:57.000000 common-test-29.9.41/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     6651 2023-05-10 00:52:04.000000 common-test-29.9.41/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     3721 2023-05-04 05:30:58.000000 common-test-29.9.41/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    10894 2023-05-08 02:03:18.000000 common-test-29.9.41/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 common-test-29.9.41/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:00.000000 common-test-29.9.41/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    17019 2023-05-15 05:31:01.000000 common-test-29.9.41/common/plugin/pytest_plugin.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-15 06:11:16.320765 common-test-29.9.41/common_test.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      623 2023-05-15 06:11:16.000000 common-test-29.9.41/common_test.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1475 2023-05-15 06:11:16.000000 common-test-29.9.41/common_test.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2023-05-15 06:11:16.000000 common-test-29.9.41/common_test.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2023-05-15 06:11:16.000000 common-test-29.9.41/common_test.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      571 2023-05-15 06:11:16.000000 common-test-29.9.41/common_test.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2023-05-15 06:11:16.000000 common-test-29.9.41/common_test.egg-info/top_level.txt
+-rw-r--r--   0 edz        (502) staff       (20)      440 2023-05-15 06:11:16.321987 common-test-29.9.41/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     1641 2023-05-04 07:57:23.000000 common-test-29.9.41/setup.py
```

### Comparing `common-test-29.9.40/PKG-INFO` & `common-test-29.9.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-test
-Version: 29.9.40
+Version: 29.9.41
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `common-test-29.9.40/common/autotest/base_requests.py` & `common-test-29.9.41/common/autotest/base_requests.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/autotest/handle_allure.py` & `common-test-29.9.41/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/autotest/handle_assert.py` & `common-test-29.9.41/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/common/api_driver.py` & `common-test-29.9.41/common/common/api_driver.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/common/constant.py` & `common-test-29.9.41/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/common/test.py` & `common-test-29.9.41/common/common/test.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/config/config.py` & `common-test-29.9.41/common/config/config.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/data/data_process.py` & `common-test-29.9.41/common/data/data_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,15 +231,15 @@
                         _temp = c
             return _temp
 
     @classmethod
     def check_test_case(datas: list):
         _datas = list()
         try:
-            _config = {'key':'traffic','env':'test'}
+            _config = {'key':'atf'}
             _mysql = MysqlDB(_config)
         except Exception as e:
             _mysql = None
         for testdata in datas:
             casename = format_caseName(testdata[Constant.CASE_TITLE])
             if DataProcess.isNotNull(get_system_key(Constant.ISSUE_KEY)) and DataProcess.isNotNull(
                     get_system_key(Constant.TEST_SRTCYCLE_ID)):
```

### Comparing `common-test-29.9.40/common/data/handle_common.py` & `common-test-29.9.41/common/data/handle_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import re
 import json
 from jsonpath import jsonpath
-
 from loguru import logger
 from common.common.constant import Constant
 from common.plugin.hooks_plugin import exec_func
 
 
 
 def extractor(obj: dict, expr: str = '.', error_flag: bool = False) -> object:
```

### Comparing `common-test-29.9.40/common/db/handle_db.py` & `common-test-29.9.41/common/db/handle_db.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+
 import pymysql
 from loguru import logger
 from common.data.handle_common import print_info
 from common.common.api_driver import APIDriver
 from common.common.constant import Constant
 
 
@@ -28,14 +30,25 @@
                  port=db_config.get('port'),
                  user=db_config.get("dbUsername"),
                  password=db_config.get("dbPasswd"),
                  db=db_config.get("dbName"),
                  charset='utf8mb4',
                  cursorclass=pymysql.cursors.DictCursor
              )
+        if config.get("atf") is not None:
+            db_config = self.get_db_config(os.environ['ATFDB'], os.environ['ATFEVN'])
+            self.conn = pymysql.connect(
+                host=db_config.get('host'),
+                port=db_config.get('port'),
+                user=db_config.get("dbUsername"),
+                password=db_config.get("dbPasswd"),
+                db=db_config.get("dbName"),
+                charset='utf8mb4',
+                cursorclass=pymysql.cursors.DictCursor
+            )
 
 
     def get_db_config(self, db_key, db_env):
         _tempdata = APIDriver.http_request(url=f"{Constant.ATF_URL_API}/getDBConfig/{db_key}/{db_env}",
                                            method='get'
                                            )
         return _tempdata.json()
```

### Comparing `common-test-29.9.40/common/db/handle_db_batch.py` & `common-test-29.9.41/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/db/handle_mysqldb.py` & `common-test-29.9.41/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/db/handle_oracle.py` & `common-test-29.9.41/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/db/handle_sqlserver.py` & `common-test-29.9.41/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/file/ReadFile.py` & `common-test-29.9.41/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/file/handle_excel.py` & `common-test-29.9.41/common/file/handle_excel.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/file/handle_file.py` & `common-test-29.9.41/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/file/handle_reques.py` & `common-test-29.9.41/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/file/handle_system.py` & `common-test-29.9.41/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/file/handle_yaml.py` & `common-test-29.9.41/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/mq/handle_rabbit.py` & `common-test-29.9.41/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/plat/ATF_platform.py` & `common-test-29.9.41/common/plat/ATF_platform.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,16 +69,13 @@
         run = ServicePlatForm.getCaseRunByNameOrID(cycleId, issuekey)
         if run['caserunid'] == '00000':
             run = ServicePlatForm.getCaseRunByNameOrID(cycleId, name)
         return run
 
 
 
-if __name__ == '__main__':
-    print(ATFPlatForm.getCaseInfoByNameOrID("DS21059-16373"))
-
```

### Comparing `common-test-29.9.40/common/plat/jenkin_platform.py` & `common-test-29.9.41/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/plat/mysql_platform.py` & `common-test-29.9.41/common/plat/mysql_platform.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import datetime
+import os
+
 from loguru import logger
 from common.db.handle_db import MysqlDB
 from common.data.handle_common import get_system_key,format_caseName
 from common.common.constant import Constant
 from common.plat.jira_platform import JiraPlatForm
 from common.data.data_process import DataProcess
 
@@ -13,14 +15,16 @@
         if DataProcess.isNotNull(get_system_key(Constant.GIT_PROJECTNAME)):
             testname, gitname, scripturl, scriptclass, scriptmethod, scriptname = DataProcess.getCaseUrlMeta(testname,
                                                                                                              caseurl)
             if DataProcess.isNotNull(scripturl):
                 if caseid != '00000':
                     JiraPlatForm.updateDescription(caseid, scripturl)
                     JiraPlatForm.updateTestReference(caseid, caseurl)
+                traffic = get_system_key('ATFDB')
+                env =get_system_key('ATFEVN')
                 _config = {'key': 'traffic', 'env': 'test'}
                 _mysql = MysqlDB(_config)
                 sql = f"delete from test_autotest_script where testname='{testname}' and gitname='{gitname}'"
                 _list = _mysql.execute(sql)
                 _mysql.conn.commit()
                 _date = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
                 _sql = f"INSERT INTO `traffic_test`.`test_autotest_script`(`gitname`, `suitname`, `tagversion`, `testid`, `testname`, `scriptclass`, `scriptmethod`, `scriptname`, `scriptpackage`, `status`, `updatetime`, `caseurl`, `scripturl`) " \
@@ -30,72 +34,93 @@
                 _mysql.close()
                 logger.info(f'保存用例和脚本关系成功：用例名称:{testname} 脚本路径:{caseurl}')
 
     @classmethod
     def insert_api_data(self, _url, _methond, _header, _data, _reponse_time,_reponse_code):
         _hash = hash(f'{_url}:{_methond}:{_header}:{_data}:{_reponse_time}')
         _data= str(_data).replace("'","")
-        _config = {'key':'traffic','env':'test'}
-        _date=datetime.datetime.now()
-        _sql=f"INSERT INTO `traffic_test`.`base_api_data`(`hash_id`, `url`,`method`, `data`, `reponse_time`,`reponse_code`, `create_time`) VALUES ('{_hash}', '{_url}', '{_methond}', '{_data}', '{_reponse_time}', '{_reponse_code}','{_date}')"
+        _config = {'key':'atf'}
+        _date = datetime.datetime.now()
+        _project_alice = os.environ['ProjectAlice']
+        _sql=f"INSERT INTO `traffic_test`.`base_api_data`(`hash_id`,`project_alice`, `url`,`method`, `data`, `reponse_time`,`reponse_code`, `create_time`) VALUES ('{_hash}','{_project_alice}', '{_url}', '{_methond}', '{_data}', '{_reponse_time}', '{_reponse_code}','{_date}')"
         _mysql = MysqlDB(_config)
         _mysql.execute(_sql)
         _mysql.conn.commit()
         _mysql.close()
 
     @classmethod
     def getScriptyPathByCaseNameList(self, CaseNameList):
-        _config = {'key':'traffic','env':'test'}
+        _config = {'key':'atf'}
         _mysql = MysqlDB(_config)
         sql = f"select distinct(caseurl) from test_autotest_script where `status` = '0'"
         sql += " and testname in (%s)" % ','.join(["'%s'" % testname for testname in CaseNameList])
         _list = _mysql.execute(sql).fetchall()
         _mysql.close()
         return _list
 
 
     @classmethod
     def get_test_autotest_run(self, jirakey, cycleId, result:str="'通过','未执行','失败','自动化执行'"):
         _info = []
         _sql = f"select * from `traffic_test`.`test_autotest_run` where jirakey='{jirakey}' and cycleId='{cycleId}' and status in ({result})"
         try:
-            _config = {'key':'traffic','env':'test'}
+            _config = {'key':'atf'}
             _mysql = MysqlDB(_config)
             _info = _mysql.execute(_sql).fetchall()
             return _info
         except Exception as e:
             logger.error(f'查询SQL异常：{_sql}')
             return _info
 
     @classmethod
+    def sync_projectConfig(self, gitName):
+        _info = []
+        _sql = f"select count(*) as _count from `traffic_test`.`test_autotest_script` where gitname='{gitName}'"
+        try:
+            _config = {'key': 'atf'}
+            _mysql = MysqlDB(_config)
+            _info = _mysql.execute(_sql).fetchall()
+            _sql = f"update `traffic_test`.`system_global_conf` set `case_count`={_info[0]['_count']} where git_project_name='{gitName}'"
+            _mysql = MysqlDB(_config)
+            _mysql.execute(_sql)
+            _mysql.conn.commit()
+            return _info
+        except Exception as e:
+            logger.error(f'查询SQL异常：{_sql}')
+            return _info
+
+    @classmethod
     def get_test_case_info(self, jirakey, cycleId, caseName):
-        _config = {'key':'traffic','env':'test'}
+        _config = {'key':'atf'}
         _sql = f"select * from `traffic_test`.`test_autotest_run` where jirakey='{jirakey}' and cycleId='{cycleId}' and casename='{caseName}'"
         _mysql = MysqlDB(_config)
         _info = _mysql.execute(_sql).fetchall()
         return _info
 
     @classmethod
     def get_test_case_info_ByID(self, jirakey, cycleId, caseid):
-        _config = {'key':'traffic','env':'test'}
+        _config = {'key':'atf'}
         _sql = f"select * from `traffic_test`.`test_autotest_run` where jirakey='{jirakey}' and cycleId='{cycleId}' and caseid='{caseid}'"
         _mysql = MysqlDB(_config)
         _info = _mysql.execute(_sql).fetchall()
         return _info
 
 
     @classmethod
     def get_api_data(self, _url, _methond, _header, _data, _reponse_time, _reponse_code):
-        _config = {'key':'traffic','env':'test'}
+        _config = {'key':'atf'}
         _sql = f"select * from `traffic_test`.`base_api_data` where `url`='{_url}' and `method`='{_methond}' and `data`='{_data}' and `reponse_code`={_reponse_code} "
         _mysql = MysqlDB(_config)
         _time=''
         _info=''
         for _temp in  _mysql.execute(_sql).fetchall():
             _time=str(_temp['reponse_time'])+"S, "+_time
             _info =str(_temp['create_time']) +"执行时间:"+str(_temp['reponse_time']) + "S, " + _info
         return _time,_info
 
 
 
 
 
+
+
+
```

### Comparing `common-test-29.9.40/common/plat/service_platform.py` & `common-test-29.9.41/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/plugin/allure_plugin.py` & `common-test-29.9.41/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/plugin/assert_plugin.py` & `common-test-29.9.41/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/plugin/atf_plugin.py` & `common-test-29.9.41/common/plugin/atf_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,16 +153,15 @@
                 uid = uids[i]
                 _caseurl = f'{buildurl}allure/#behaviors/{parentUid}/{uid}'
                 _caseTitleList = caseName[i].split(';')
                 for temp in _caseTitleList:
                     ATFPlatForm.sent_result_byCaseName(temp, "", "", _caseurl)
 
 
-if __name__ == '__main__':
-    print(ATFPlugin.db_ops("psn", "select * from flight_quota where FLIGHT_NO = 'MU5119' ORDER BY FLIGHT_DATE desc"))
+
```

### Comparing `common-test-29.9.40/common/plugin/data_bus.py` & `common-test-29.9.41/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/plugin/data_plugin.py` & `common-test-29.9.41/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/plugin/file_plugin.py` & `common-test-29.9.41/common/plugin/file_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/plugin/hooks_plugin.py` & `common-test-29.9.41/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/plugin/pytest_playwright.py` & `common-test-29.9.41/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common/plugin/pytest_plugin.py` & `common-test-29.9.41/common/plugin/pytest_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,16 @@
                 if len(_caseNameList) == 0:
                     logger.info("无测试用例列表可运行")
                 else:
                     PytestPlugin.runSceneCase(_caseNameList)
             else:
                 logger.info("运行测试文件:" + get_system_key(Constant.TEST_CASE_PATH))
                 PytestPlugin.runPathCase(get_system_key(Constant.TEST_CASE_PATH))
+            if DataProcess.isNotNull(get_system_key('type')) and get_system_key('type').strip() == '脚本同步':
+                MysqlPlatForm.sync_projectConfig(get_system_key('gitProjectName'))
 
     @classmethod
     def allure_report(cls):
         """
         生成测试报告
         :return:
         """
@@ -232,15 +234,15 @@
                 _args= item.__dict__['keywords'].__dict__['_markers']['pytestmark']
                 for arg in _args:
                      label_type = arg.__dict__['kwargs']['label_type']
                      if label_type == 'as_id':
                          _caseNo = arg.__dict__['args'][0]
         except Exception as e:
             print_info('未通过装饰器ID获取到用例信息')
-        print_info(f"执行用例名称：{_caseTitle} 用例编号:{_caseNo}")
+        print_info(f"执行用例名称:{_caseTitle} 用例编号:{_caseNo}")
         print_info(f'用例数据:{_caseData}')
         return _caseTitle, _caseNo
 
     @classmethod
     def send_case_result(self, item: Item, result):
             _caseTitle, _caseNo = PytestPlugin.getCaseName(item)
             if DataProcess.isNotNull(_caseTitle):
@@ -254,43 +256,43 @@
                         info = ATFPlatForm.getCaseInfoByNameOrID(temp)
                         if result != 'skipped' and info['key'] != '00000':
                             caseInfoList = caseInfoList + info['summary'] + "(" + info['key'] + "),"
                             ATFPlatForm.sent_result_byCaseName(info['summary'], info['key'], result, "")
                         else:
                             caseInfoList = caseInfoList + temp + "(" + info['key'] + "),"
                 if result != Constant.STATUS_AUTOTEST:
-                    logger.info(f"---用例列表：{caseInfoList}  执行状态:{result}")
+                    logger.info(f"---用例列表:{caseInfoList}  执行状态:{result}")
             else:
-                logger.info(f"---用例列表：无用例列表【请检查是否设置用例名称或者编号】 执行状态:{result}")
+                logger.info(f"---用例列表:无用例列表【请检查是否设置用例名称或者编号】 执行状态:{result}")
 
     @classmethod
     def sync_case_Script(self, item: Item, _caseTitle, _caseNo):
         _caseurl = PytestPlugin.getCaseUrl(item)
         if DataProcess.isNotNull(_caseTitle):
             _caseTitleList = _caseTitle.split(';')
         if DataProcess.isNotNull(_caseNo) and _caseNo != '00000':
             _caseTitleList.extend(_caseNo.split(';'))
         if DataProcess.isNotNull(_caseTitleList):
             caseInfoList = ""
             if DataProcess.isNotNull(get_system_key('type')) and get_system_key('type').strip() == '脚本同步':
-                logger.info(f"---获取用例列表：{_caseTitleList} 脚本路径:{_caseurl} 执行状态:用例同步")
+                logger.info(f"---获取用例列表:{_caseTitleList} 脚本路径:{_caseurl} 执行状态:用例同步")
                 for _name in _caseTitleList:
                     if DataProcess.isNotNull(_name) and _name != '00000':
                         info = ATFPlatForm.getCaseInfoByNameOrID(_name)
                         caseInfoList = caseInfoList + _name + "(" + info['key'] + "),"
                         MysqlPlatForm.sync_autotest_script(info['summary'], info['key'], _caseurl)
                 logger.info(f"---用例列表：{caseInfoList} 脚本路径:{_caseurl}  执行状态:同步成功")
                 assert "测试用例检查" == "脚本用例同步【执行结果可忽略】"
             if PytestPlugin.checkCaseRun(item, _caseTitle, _caseNo) == False:
-                logger.info(f"---获取用例列表：{_caseTitleList} 脚本路径:{_caseurl} 执行状态:执行中断")
+                logger.info(f"---获取用例列表:{_caseTitleList} 脚本路径:{_caseurl} 执行状态:执行中断")
                 assert "测试用例检查" == "未在测试周期中【执行中断】"
             else:
-                logger.info(f"---获取用例列表：{_caseTitleList} 脚本路径:{_caseurl} 执行状态:开始执行")
+                logger.info(f"---获取用例列表:{_caseTitleList} 脚本路径:{_caseurl} 执行状态:开始执行")
         else:
-            logger.info(f"---用例列表：无用例列表【请检查是否设置用例名称或者编号】")
+            logger.info(f"---用例列表:无用例列表【请检查是否设置用例名称或者编号】")
             assert "测试用例检查" == "无用例列表【执行结果可忽略】"
 
 
     @classmethod
     def checkCaseRun(self,item: Item, _caseTitle, _caseNo):
         isRun = False
         if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)):
```

### Comparing `common-test-29.9.40/common_test.egg-info/PKG-INFO` & `common-test-29.9.41/common_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-test
-Version: 29.9.40
+Version: 29.9.41
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `common-test-29.9.40/common_test.egg-info/SOURCES.txt` & `common-test-29.9.41/common_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/common_test.egg-info/requires.txt` & `common-test-29.9.41/common_test.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `common-test-29.9.40/setup.py` & `common-test-29.9.41/setup.py`

 * *Files identical despite different names*

