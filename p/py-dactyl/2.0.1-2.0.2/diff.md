# Comparing `tmp/py-dactyl-2.0.1.tar.gz` & `tmp/py-dactyl-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-dactyl-2.0.1.tar", last modified: Tue Apr 18 22:35:21 2023, max compression
+gzip compressed data, was "py-dactyl-2.0.2.tar", last modified: Tue May 23 02:36:19 2023, max compression
```

## Comparing `py-dactyl-2.0.1.tar` & `py-dactyl-2.0.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 22:35:21.765143 py-dactyl-2.0.1/
--rw-rw-rw-   0        0        0     1087 2019-09-06 01:53:10.000000 py-dactyl-2.0.1/LICENSE
--rw-rw-rw-   0        0        0    11902 2023-04-18 22:35:21.765143 py-dactyl-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    11232 2023-02-07 17:35:42.000000 py-dactyl-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 22:35:21.739120 py-dactyl-2.0.1/py_dactyl.egg-info/
--rw-rw-rw-   0        0        0    11902 2023-04-18 22:35:21.000000 py-dactyl-2.0.1/py_dactyl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1635 2023-04-18 22:35:21.000000 py-dactyl-2.0.1/py_dactyl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 22:35:21.000000 py-dactyl-2.0.1/py_dactyl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-18 22:35:21.000000 py-dactyl-2.0.1/py_dactyl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-18 22:35:21.000000 py-dactyl-2.0.1/py_dactyl.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-18 22:35:21.741121 py-dactyl-2.0.1/pydactyl/
--rw-rw-rw-   0        0        0      266 2021-12-13 10:15:35.000000 py-dactyl-2.0.1/pydactyl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:35:21.745125 py-dactyl-2.0.1/pydactyl/api/
--rw-rw-rw-   0        0        0        0 2021-12-16 03:59:43.000000 py-dactyl-2.0.1/pydactyl/api/__init__.py
--rw-rw-rw-   0        0        0     5066 2022-10-22 21:51:34.000000 py-dactyl-2.0.1/pydactyl/api/base.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:35:21.746126 py-dactyl-2.0.1/pydactyl/api/client/
--rw-rw-rw-   0        0        0        0 2021-12-13 10:15:35.000000 py-dactyl-2.0.1/pydactyl/api/client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:35:21.747127 py-dactyl-2.0.1/pydactyl/api/client/account/
--rw-rw-rw-   0        0        0       63 2022-07-21 04:46:12.000000 py-dactyl-2.0.1/pydactyl/api/client/account/__init__.py
--rw-rw-rw-   0        0        0     3930 2022-07-21 04:46:12.000000 py-dactyl-2.0.1/pydactyl/api/client/account/base.py
--rw-rw-rw-   0        0        0     3042 2021-12-13 10:15:35.000000 py-dactyl-2.0.1/pydactyl/api/client/client_api.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:35:21.753133 py-dactyl-2.0.1/pydactyl/api/client/servers/
--rw-rw-rw-   0        0        0       67 2022-07-21 04:46:12.000000 py-dactyl-2.0.1/pydactyl/api/client/servers/__init__.py
--rw-rw-rw-   0        0        0     2389 2022-07-21 04:46:12.000000 py-dactyl-2.0.1/pydactyl/api/client/servers/backups.py
--rw-rw-rw-   0        0        0     4915 2022-10-13 04:24:57.000000 py-dactyl-2.0.1/pydactyl/api/client/servers/base.py
--rw-rw-rw-   0        0        0     2734 2022-10-13 04:15:39.000000 py-dactyl-2.0.1/pydactyl/api/client/servers/databases.py
--rw-rw-rw-   0        0        0     7057 2022-09-11 23:21:10.000000 py-dactyl-2.0.1/pydactyl/api/client/servers/files.py
--rw-rw-rw-   0        0        0     2598 2021-12-13 10:15:35.000000 py-dactyl-2.0.1/pydactyl/api/client/servers/network.py
--rw-rw-rw-   0        0        0     7856 2022-09-11 20:33:30.000000 py-dactyl-2.0.1/pydactyl/api/client/servers/schedules.py
--rw-rw-rw-   0        0        0      934 2021-12-13 10:15:35.000000 py-dactyl-2.0.1/pydactyl/api/client/servers/settings.py
--rw-rw-rw-   0        0        0     1021 2021-12-13 10:15:35.000000 py-dactyl-2.0.1/pydactyl/api/client/servers/startup.py
--rw-rw-rw-   0        0        0     2762 2021-12-13 10:15:35.000000 py-dactyl-2.0.1/pydactyl/api/client/servers/users.py
--rw-rw-rw-   0        0        0     3061 2022-10-13 01:06:05.000000 py-dactyl-2.0.1/pydactyl/api/locations.py
--rw-rw-rw-   0        0        0     2346 2022-10-13 03:47:18.000000 py-dactyl-2.0.1/pydactyl/api/nests.py
--rw-rw-rw-   0        0        0     8738 2022-10-13 03:48:05.000000 py-dactyl-2.0.1/pydactyl/api/nodes.py
--rw-rw-rw-   0        0        0    23394 2023-04-18 22:27:33.000000 py-dactyl-2.0.1/pydactyl/api/servers.py
--rw-rw-rw-   0        0        0     6850 2022-10-13 02:05:07.000000 py-dactyl-2.0.1/pydactyl/api/user.py
--rw-rw-rw-   0        0        0     3773 2022-10-22 21:13:54.000000 py-dactyl-2.0.1/pydactyl/api_client.py
--rw-rw-rw-   0        0        0      300 2023-04-18 22:30:36.000000 py-dactyl-2.0.1/pydactyl/constants.py
--rw-rw-rw-   0        0        0      458 2021-06-13 20:23:08.000000 py-dactyl-2.0.1/pydactyl/exceptions.py
--rw-rw-rw-   0        0        0     3039 2022-10-22 22:20:10.000000 py-dactyl-2.0.1/pydactyl/responses.py
--rw-rw-rw-   0        0        0       42 2023-04-18 22:35:21.765143 py-dactyl-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1343 2020-05-21 18:13:17.000000 py-dactyl-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:35:21.753133 py-dactyl-2.0.1/tests/
--rw-rw-rw-   0        0        0        0 2021-12-13 23:56:07.000000 py-dactyl-2.0.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:35:21.756135 py-dactyl-2.0.1/tests/application/
--rw-rw-rw-   0        0        0        0 2022-07-21 04:46:12.000000 py-dactyl-2.0.1/tests/application/__init__.py
--rw-rw-rw-   0        0        0     2519 2022-10-13 01:07:04.000000 py-dactyl-2.0.1/tests/application/locations_test.py
--rw-rw-rw-   0        0        0     3112 2022-10-22 16:12:24.000000 py-dactyl-2.0.1/tests/application/nests_test.py
--rw-rw-rw-   0        0        0     5680 2022-10-13 03:51:41.000000 py-dactyl-2.0.1/tests/application/nodes_test.py
--rw-rw-rw-   0        0        0     8498 2022-10-13 04:03:48.000000 py-dactyl-2.0.1/tests/application/servers_test.py
--rw-rw-rw-   0        0        0     6500 2022-10-22 16:45:53.000000 py-dactyl-2.0.1/tests/application/user_test.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:35:21.758137 py-dactyl-2.0.1/tests/base/
--rw-rw-rw-   0        0        0        0 2022-07-21 04:46:12.000000 py-dactyl-2.0.1/tests/base/__init__.py
--rw-rw-rw-   0        0        0      915 2022-10-22 21:09:04.000000 py-dactyl-2.0.1/tests/base/api_client_test.py
--rw-rw-rw-   0        0        0     8255 2022-10-28 15:58:11.000000 py-dactyl-2.0.1/tests/base/base_test.py
--rw-rw-rw-   0        0        0     5466 2022-10-22 21:05:54.000000 py-dactyl-2.0.1/tests/base/responses_test.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:35:21.764142 py-dactyl-2.0.1/tests/client/
--rw-rw-rw-   0        0        0        0 2022-07-21 04:46:12.000000 py-dactyl-2.0.1/tests/client/__init__.py
--rw-rw-rw-   0        0        0     3588 2022-07-21 04:46:12.000000 py-dactyl-2.0.1/tests/client/account_test.py
--rw-rw-rw-   0        0        0     2147 2022-07-21 04:46:12.000000 py-dactyl-2.0.1/tests/client/backups_test.py
--rw-rw-rw-   0        0        0     3139 2022-10-13 04:25:19.000000 py-dactyl-2.0.1/tests/client/client_servers_test.py
--rw-rw-rw-   0        0        0     2971 2022-10-13 04:14:58.000000 py-dactyl-2.0.1/tests/client/databases_test.py
--rw-rw-rw-   0        0        0     8319 2022-09-11 23:21:44.000000 py-dactyl-2.0.1/tests/client/files_test.py
--rw-rw-rw-   0        0        0     2255 2021-12-13 10:15:35.000000 py-dactyl-2.0.1/tests/client/network_test.py
--rw-rw-rw-   0        0        0     4607 2022-09-11 20:33:34.000000 py-dactyl-2.0.1/tests/client/schedules_test.py
--rw-rw-rw-   0        0        0     1050 2021-12-13 10:15:35.000000 py-dactyl-2.0.1/tests/client/settings_test.py
--rw-rw-rw-   0        0        0     1094 2021-12-13 10:15:35.000000 py-dactyl-2.0.1/tests/client/startup_test.py
--rw-rw-rw-   0        0        0     2331 2022-10-22 16:45:53.000000 py-dactyl-2.0.1/tests/client/users_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.753814 py-dactyl-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-23 02:36:06.000000 py-dactyl-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-05-23 02:36:19.753814 py-dactyl-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-05-23 02:36:06.000000 py-dactyl-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.741814 py-dactyl-2.0.2/py_dactyl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-05-23 02:36:19.000000 py-dactyl-2.0.2/py_dactyl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-23 02:36:19.000000 py-dactyl-2.0.2/py_dactyl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 02:36:19.000000 py-dactyl-2.0.2/py_dactyl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 02:36:19.000000 py-dactyl-2.0.2/py_dactyl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 02:36:19.000000 py-dactyl-2.0.2/py_dactyl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.741814 py-dactyl-2.0.2/pydactyl/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-23 02:36:06.000000 py-dactyl-2.0.2/pydactyl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.745814 py-dactyl-2.0.2/pydactyl/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:06.000000 py-dactyl-2.0.2/pydactyl/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-05-23 02:36:06.000000 py-dactyl-2.0.2/pydactyl/api/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.745814 py-dactyl-2.0.2/pydactyl/api/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:06.000000 py-dactyl-2.0.2/pydactyl/api/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.745814 py-dactyl-2.0.2/pydactyl/api/client/account/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-23 02:36:06.000000 py-dactyl-2.0.2/pydactyl/api/client/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/account/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/client_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.745814 py-dactyl-2.0.2/pydactyl/api/client/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/servers/backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/servers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/servers/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/servers/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/servers/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/servers/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/servers/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/servers/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/servers/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/nests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22896 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 02:36:19.753814 py-dactyl-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.745814 py-dactyl-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.745814 py-dactyl-2.0.2/tests/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/application/locations_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/application/nests_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/application/nodes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/application/servers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/application/user_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.749814 py-dactyl-2.0.2/tests/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/base/api_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/base/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/base/responses_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.749814 py-dactyl-2.0.2/tests/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/account_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/backups_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/client_servers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/databases_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/files_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/network_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/schedules_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/settings_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/startup_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/users_test.py
```

### Comparing `py-dactyl-2.0.1/LICENSE` & `py-dactyl-2.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2019 Ryan Kubiak
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2019 Ryan Kubiak
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `py-dactyl-2.0.1/PKG-INFO` & `py-dactyl-2.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,335 +1,331 @@
-Metadata-Version: 2.1
-Name: py-dactyl
-Version: 2.0.1
-Summary: An easy to use Python wrapper for the Pterodactyl Panel API.
-Home-page: https://github.com/iamkubi/pydactyl
-Author: Ryan Kubiak
-Author-email: iamkubi@gmail.com
-License: UNKNOWN
-Project-URL: Documentation, https://pydactyl.readthedocs.io/
-Project-URL: Source, https://github.com/iamkubi/pydactyl
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pydactyl
-
-![lint-and-test]
-[![Latest docs][docs-img]][docs]
-[![Coverage][codecov-img]][codecov]
-[![Latest version][pypi-img]][pypi]
-[![Discord][discord-img]][discord-join]
-
-An easy to use Python wrapper for the Pterodactyl Panel API.
-
-## State of the project
-
-Support for the Pterodactyl 1.x API is complete.
-The 2.0 Pydactyl release was created to standardize how includes and params 
-are passed.  As a result some endpoints (namely nests) **will break** when 
-upgrading from Pydactyl 1.x to 2.0.
-
-Pull Requests are being accepted and new endpoints will continue to be added.
-
-If you encounter problems, find APIs that haven't been implemented, or have a
-feature request please file a [Github issue][issues].
-
-## Documentation
-
-Generated documentation can be found at [https://pydactyl.readthedocs.io/][docs]
-.
-
-## Installing
-
-To install with pip:
-
-```shell
-pip install py-dactyl
-```
-
-**If you get an error saying `ImportError: cannot import name 
-'PterodactylClient' from 'pydactyl'` this probably means you installed the 
-wrong package from pip.**
-
-## Getting Started
-
-**Pterodactyl has two different types of API keys: Client (also known as 
-Account) and Application.**  Any user can generate an Account API key to 
-control their own servers.  The Account API key for an Administrator user will
-be able to access any server's Client API.
-
-Application API keys can only be generated by administrators.  These keys can be used to create, modify, and delete servers, among other things.  They have access to any server on the panel and can be destructive, so use with care.
-
-### Exploring the API
-In addition to the documentation you can explore the interface in an 
-interactive Python interpreter using built-ins like `dir()` and the
-`__doc__` attribute as shown below.
-
-```python
-from pydactyl import PterodactylClient
-api = PterodactylClient('debug', 'anything')
-
-[i for i in dir(api.client.servers) if not i.startswith('_')]
-# ['account', 'backups', 'databases', 'files', 'get_server', 'get_server_utilization', 'list_permissions', 'list_servers', 'network', 'schedules', 'send_console_command', 'send_power_action', 'servers', 'settings', 'startup', 'users']
-[i for i in dir(api.client.servers.settings) if not i.startswith('_')]
-# ['reinstall_server', 'rename_server']
-print(api.client.servers.settings.rename_server.__doc__)
-#Renames the server.
-#        Args:
-#            server_id(str): Server identifier (abbreviated UUID)
-#            name(str): New name for the server
-```
-
-### Client API
-The Client API or Account API is accessed by users of the Pterodactyl panel. 
-Below is the layout of the Client API namespace.
-
-```python
-api.client.account
-api.client.servers
-api.client.servers.backups
-api.client.servers.databases
-api.client.servers.files
-api.client.servers.network
-api.client.servers.schedules
-api.client.servers.settings
-api.client.servers.startup
-api.client.servers.users
-```
-
-A full list of methods available can be found in the [documentation][docs]. 
-
-
-Below are examples of how you might get information about your servers.
-
-```python
-from pydactyl import PterodactylClient
-
-# Create a client to connect to the panel and authenticate with your API key.
-api = PterodactylClient('https://panel.mydomain.com', 'MySuperSecretApiKey')
-
-# Get a list of all servers the user has access to
-my_servers = api.client.servers.list_servers()
-# Get the unique identifier for the first server.
-srv_id = my_servers[0]['attributes']['identifier']
-
-# Check the utilization of the server
-srv_utilization = api.client.servers.get_server_utilization(srv_id)
-print(srv_utilization)
-
-# Turn the server on.
-api.client.servers.send_power_action(srv_id, 'start')
-```
-
-### Application API
-**As of Pterodactyl 1.8.0 Application API keys are deprecated and client API keys should now be used exclusively.**  
-
-The Application API is the administrative API of the Pterodactyl panel. 
-Below is the layout of the Application API namespace.
-
-```python
-api.locations
-api.nests
-api.nodes
-api.servers
-api.user
-```
-
-Below are examples of how you might use this API.
-
-```python
-from pydactyl import PterodactylClient
-
-# Create a client to connect to the panel and authenticate with your API key.
-api = PterodactylClient('https://panel.mydomain.com', 'MySuperSecretApiKey')
-
-# Create a server.  Customize the Nest and Egg IDs to match the IDs in your panel.
-# This server is created with a limit of 8000 MB of memory, no access to swap, unlimited disk space, in location_id 1.
-api.servers.create_server(name='My Paper Server', user_id=1, nest_id=1,
-                          egg_id=3, memory_limit=8000, swap_limit=0,
-                          backup_limit=0, disk_limit=0, location_ids=[1])
-< Response[201] >
-```
-
-A 201 response indicates success, however if there is a problem with the request
-Pydactyl will raise an exception with additional details. When updating the
-location_ids field to an invalid location it displays an error:
-
- ```python
-api.servers.create_server(name='My Paper Server', user_id=1, nest_id=1,
-                          egg_id=3, memory_limit=8000, swap_limit=0,
-                          disk_limit=0, location_ids=[199])
-Traceback (most recent call last):
- File "<input>", line 6, in <module>
- File "D:\code\pydactyl\pydactyl\api\servers.py", line 268, in create_server
-   mode='POST', data=data, json=False)
- File "D:\code\pydactyl\pydactyl\api\base.py", line 98, in _api_request
-   'code'], errors['detail'])
-pydactyl.exceptions.PterodactylApiError: Bad API Request(400) - NoViableNodeException - No nodes satisfying the requirements specified for automatic deployment could be found.
-```
-
-You can use the User class to add, modify, and delete panel users.
-
-```python
-# Create a new user
-result = api.user.create_user('test_user', 'test@gmail.com', 'Test', 'Name')
-# Get the ID of the created user
-user_id = result['attributes']['id']
-# Get the user info, also returned by create_user()
-api.user.get_user_info(user_id)
-{'object': 'user', 'attributes': {'id': 14, 'external_id': None, .... }}
-# Delete the user
-api.user.delete_user(user_id=14)
-```
-
-### Includes
-
-Pterodactyl API endpoints have different sets of includes you can pass to alter 
-the response.  Using includes will cause additional information to show up 
-in the relationships field of the response data.  Some endpoints have no 
-includes and some have many.
-
-Pydactyl docstrings include examples of 
-valid includes for each endpoint, but they are **not an exhaustive list**.
-
-```
-server_includes = [
-    'allocations', 'user', 'subusers', 'pack', 'nest', 'egg', 'variables',
-    'location', 'node', 'databases']
-```
-
-As an example the application server details endpoint has 10 potential 
-includes according to the API docs.  Note that the API docs are not always 
-accurate either!
-
-Most endpoints that generate lists will have optional includes that can be 
-passed as lists or tuples.
-
-```python
-api.nodes.list_nodes(includes=('allocations', 'location'))
-api.servers.get_server_info(
-    server_id=53,
-    includes=['user', 'subusers', 'location'])
-```
-
-### Params
-
-Most endpoints with includes will also have a `params` parameter.  This can 
-be used to pass additional parameters.  Many endpoint specific `params` are 
-already supported by Pydactyl, however some additional params apply 
-universally like `per_page`.
-
-```python
-api.nodes.list_nodes(params={'per_page': 9001})
-api.servers.list_servers(params={'per_page': 9001})
-api.users.list_users(params={'per_page': 9001})
-```
-
-## PterodactylClient
-
-Each of the classes in pydactyl could be imported independently, but the 
-PterodactylClient class [pydactyl/api_client.py](pydactyl/api_client.py) 
-provides a simplified interface that imports libraries for you and provides 
-some convenience features like retries and debug logging.
-
-### Retries
-
-Instances of [PterodactylClient](pydactyl/api_client.py) will automatically
-retry calls that fail with a 429 status code indicating that the request was
-rate-limited by Pterodactyl.
-
-By default it uses a backoff_factor of 1 with 3 retries. You can configure the
-number of retries and backoff_factor when instantiating a client.
-
-```python
-PterodactylClient('panel', 'key', backoff_factor=2, retries=10)
-```
-
-Details on backoff_factor and retires can be found in the
-[urllib3.util.Retry documentation](https://urllib3.readthedocs.io/en/stable/reference/urllib3.util.html#urllib3.util.Retry)
-.
-
-If your server is overloaded or intermittently unavailable you may want to retry
-on other status codes as well. To do this you can pass in a list of integer HTTP
-status codes.
-
-```python
-PterodactylClient('foo', 'bar', extra_retry_codes=[502, 504])
-```
-
-### Debug logging
-
-Most errors from pydactyl will present as exceptions and there is no logging 
-by default, however sometimes additional logging is helpful.  You can get 
-request logging by passing `debug=True` to PterodactylClient.
-
-```python
-app_api = PterodactylClient('https://why', 'broken', debug=True)
-app_api.servers.list_servers(includes=('egg', 'nest'))
-DEBUG:urllib3.connectionpool:Starting new HTTPS connection (1): why:443
-DEBUG:urllib3.connectionpool:https://why:443 "GET /api/application/servers?include=egg%2Cnest HTTP/1.1" 200 None
-```
-
-## Paginated Responses
-
-Pydactyl API responses return
-a [PaginatedResponse object](pydactyl/responses.py#L4) that can be iterated over
-to automatically fetch additional pages as required. This is currently 
-implemented on many endpoints which frequently return multi-page responses, 
-but not all.
-
-```python
-# Create a list of all ports
-allocs = api.nodes.list_node_allocations(node_id)
-ports = []
-for page in allocs:
-    for item in page:
-        ports.append(item['attributes']['port'])
-len(ports)
-151
-```
-
-#### collect()
-
-The `collect()` method will fetch the data from all pages of a
-PaginatedResponse. This allows you to easily fetch all results when you want all
-the data without having to iterate over the pages.
-
-The above example to get a list of ports now looks like:
-
-```python
-# Create a list of all ports
-allocs = api.nodes.list_node_allocations(node_id)
-ports = allocs.collect()
-len(ports)
-151
-```
-
-[docs]: https://pydactyl.readthedocs.io/
-
-[docs-img]: https://readthedocs.org/projects/pydactyl/badge/?version=latest (Latest docs)
-
-[pulls]: https://github.com/iamkubi/pydactyl/pulls
-
-[issues]: https://github.com/iamkubi/pydactyl/issues
-
-[pypi]: https://pypi.python.org/pypi/py-dactyl/
-
-[pypi-img]: https://img.shields.io/pypi/v/py-dactyl.svg
-
-[codecov]: https://codecov.io/gh/iamkubi/pydactyl
-
-[codecov-img]: https://codecov.io/gh/iamkubi/pydactyl/branch/main/graph/badge.svg
-
-[discord-img]: https://img.shields.io/badge/discord-join-7289DA.svg?logo=discord&longCache=true&style=flat
-
-[discord-join]: https://discord.gg/TgZDHPB
-
-[lint-and-test]: https://github.com/iamkubi/pydactyl/actions/workflows/lint-and-test.yml/badge.svg?branch=main (https://github.com/iamkubi/pydactyl/actions/workflows/lint-and-test.yml)
-
-
+Metadata-Version: 2.1
+Name: py-dactyl
+Version: 2.0.2
+Summary: An easy to use Python wrapper for the Pterodactyl Panel API.
+Home-page: https://github.com/iamkubi/pydactyl
+Author: Ryan Kubiak
+Author-email: iamkubi@gmail.com
+Project-URL: Documentation, https://pydactyl.readthedocs.io/
+Project-URL: Source, https://github.com/iamkubi/pydactyl
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pydactyl
+
+![lint-and-test]
+[![Latest docs][docs-img]][docs]
+[![Coverage][codecov-img]][codecov]
+[![Latest version][pypi-img]][pypi]
+[![Discord][discord-img]][discord-join]
+
+An easy to use Python wrapper for the Pterodactyl Panel API.
+
+## State of the project
+
+Support for the Pterodactyl 1.x API is complete.
+The 2.0 Pydactyl release was created to standardize how includes and params 
+are passed.  As a result some endpoints (namely nests) **will break** when 
+upgrading from Pydactyl 1.x to 2.0.
+
+Pull Requests are being accepted and new endpoints will continue to be added.
+
+If you encounter problems, find APIs that haven't been implemented, or have a
+feature request please file a [Github issue][issues].
+
+## Documentation
+
+Generated documentation can be found at [https://pydactyl.readthedocs.io/][docs]
+.
+
+## Installing
+
+To install with pip:
+
+```shell
+pip install py-dactyl
+```
+
+**If you get an error saying `ImportError: cannot import name 
+'PterodactylClient' from 'pydactyl'` this probably means you installed the 
+wrong package from pip.**
+
+## Getting Started
+
+**Pterodactyl has two different types of API keys: Client (also known as 
+Account) and Application.**  Any user can generate an Account API key to 
+control their own servers.  The Account API key for an Administrator user will
+be able to access any server's Client API.
+
+Application API keys can only be generated by administrators.  These keys can be used to create, modify, and delete servers, among other things.  They have access to any server on the panel and can be destructive, so use with care.
+
+### Exploring the API
+In addition to the documentation you can explore the interface in an 
+interactive Python interpreter using built-ins like `dir()` and the
+`__doc__` attribute as shown below.
+
+```python
+from pydactyl import PterodactylClient
+api = PterodactylClient('debug', 'anything')
+
+[i for i in dir(api.client.servers) if not i.startswith('_')]
+# ['account', 'backups', 'databases', 'files', 'get_server', 'get_server_utilization', 'list_permissions', 'list_servers', 'network', 'schedules', 'send_console_command', 'send_power_action', 'servers', 'settings', 'startup', 'users']
+[i for i in dir(api.client.servers.settings) if not i.startswith('_')]
+# ['reinstall_server', 'rename_server']
+print(api.client.servers.settings.rename_server.__doc__)
+#Renames the server.
+#        Args:
+#            server_id(str): Server identifier (abbreviated UUID)
+#            name(str): New name for the server
+```
+
+### Client API
+The Client API or Account API is accessed by users of the Pterodactyl panel. 
+Below is the layout of the Client API namespace.
+
+```python
+api.client.account
+api.client.servers
+api.client.servers.backups
+api.client.servers.databases
+api.client.servers.files
+api.client.servers.network
+api.client.servers.schedules
+api.client.servers.settings
+api.client.servers.startup
+api.client.servers.users
+```
+
+A full list of methods available can be found in the [documentation][docs]. 
+
+
+Below are examples of how you might get information about your servers.
+
+```python
+from pydactyl import PterodactylClient
+
+# Create a client to connect to the panel and authenticate with your API key.
+api = PterodactylClient('https://panel.mydomain.com', 'MySuperSecretApiKey')
+
+# Get a list of all servers the user has access to
+my_servers = api.client.servers.list_servers()
+# Get the unique identifier for the first server.
+srv_id = my_servers[0]['attributes']['identifier']
+
+# Check the utilization of the server
+srv_utilization = api.client.servers.get_server_utilization(srv_id)
+print(srv_utilization)
+
+# Turn the server on.
+api.client.servers.send_power_action(srv_id, 'start')
+```
+
+### Application API
+**As of Pterodactyl 1.8.0 Application API keys are deprecated and client API keys should now be used exclusively.**  
+
+The Application API is the administrative API of the Pterodactyl panel. 
+Below is the layout of the Application API namespace.
+
+```python
+api.locations
+api.nests
+api.nodes
+api.servers
+api.user
+```
+
+Below are examples of how you might use this API.
+
+```python
+from pydactyl import PterodactylClient
+
+# Create a client to connect to the panel and authenticate with your API key.
+api = PterodactylClient('https://panel.mydomain.com', 'MySuperSecretApiKey')
+
+# Create a server.  Customize the Nest and Egg IDs to match the IDs in your panel.
+# This server is created with a limit of 8000 MB of memory, no access to swap, unlimited disk space, in location_id 1.
+api.servers.create_server(name='My Paper Server', user_id=1, nest_id=1,
+                          egg_id=3, memory_limit=8000, swap_limit=0,
+                          backup_limit=0, disk_limit=0, location_ids=[1])
+< Response[201] >
+```
+
+A 201 response indicates success, however if there is a problem with the request
+Pydactyl will raise an exception with additional details. When updating the
+location_ids field to an invalid location it displays an error:
+
+ ```python
+api.servers.create_server(name='My Paper Server', user_id=1, nest_id=1,
+                          egg_id=3, memory_limit=8000, swap_limit=0,
+                          disk_limit=0, location_ids=[199])
+Traceback (most recent call last):
+ File "<input>", line 6, in <module>
+ File "D:\code\pydactyl\pydactyl\api\servers.py", line 268, in create_server
+   mode='POST', data=data, json=False)
+ File "D:\code\pydactyl\pydactyl\api\base.py", line 98, in _api_request
+   'code'], errors['detail'])
+pydactyl.exceptions.PterodactylApiError: Bad API Request(400) - NoViableNodeException - No nodes satisfying the requirements specified for automatic deployment could be found.
+```
+
+You can use the User class to add, modify, and delete panel users.
+
+```python
+# Create a new user
+result = api.user.create_user('test_user', 'test@gmail.com', 'Test', 'Name')
+# Get the ID of the created user
+user_id = result['attributes']['id']
+# Get the user info, also returned by create_user()
+api.user.get_user_info(user_id)
+{'object': 'user', 'attributes': {'id': 14, 'external_id': None, .... }}
+# Delete the user
+api.user.delete_user(user_id=14)
+```
+
+### Includes
+
+Pterodactyl API endpoints have different sets of includes you can pass to alter 
+the response.  Using includes will cause additional information to show up 
+in the relationships field of the response data.  Some endpoints have no 
+includes and some have many.
+
+Pydactyl docstrings include examples of 
+valid includes for each endpoint, but they are **not an exhaustive list**.
+
+```
+server_includes = [
+    'allocations', 'user', 'subusers', 'pack', 'nest', 'egg', 'variables',
+    'location', 'node', 'databases']
+```
+
+As an example the application server details endpoint has 10 potential 
+includes according to the API docs.  Note that the API docs are not always 
+accurate either!
+
+Most endpoints that generate lists will have optional includes that can be 
+passed as lists or tuples.
+
+```python
+api.nodes.list_nodes(includes=('allocations', 'location'))
+api.servers.get_server_info(
+    server_id=53,
+    includes=['user', 'subusers', 'location'])
+```
+
+### Params
+
+Most endpoints with includes will also have a `params` parameter.  This can 
+be used to pass additional parameters.  Many endpoint specific `params` are 
+already supported by Pydactyl, however some additional params apply 
+universally like `per_page`.
+
+```python
+api.nodes.list_nodes(params={'per_page': 9001})
+api.servers.list_servers(params={'per_page': 9001})
+api.users.list_users(params={'per_page': 9001})
+```
+
+## PterodactylClient
+
+Each of the classes in pydactyl could be imported independently, but the 
+PterodactylClient class [pydactyl/api_client.py](pydactyl/api_client.py) 
+provides a simplified interface that imports libraries for you and provides 
+some convenience features like retries and debug logging.
+
+### Retries
+
+Instances of [PterodactylClient](pydactyl/api_client.py) will automatically
+retry calls that fail with a 429 status code indicating that the request was
+rate-limited by Pterodactyl.
+
+By default it uses a backoff_factor of 1 with 3 retries. You can configure the
+number of retries and backoff_factor when instantiating a client.
+
+```python
+PterodactylClient('panel', 'key', backoff_factor=2, retries=10)
+```
+
+Details on backoff_factor and retires can be found in the
+[urllib3.util.Retry documentation](https://urllib3.readthedocs.io/en/stable/reference/urllib3.util.html#urllib3.util.Retry)
+.
+
+If your server is overloaded or intermittently unavailable you may want to retry
+on other status codes as well. To do this you can pass in a list of integer HTTP
+status codes.
+
+```python
+PterodactylClient('foo', 'bar', extra_retry_codes=[502, 504])
+```
+
+### Debug logging
+
+Most errors from pydactyl will present as exceptions and there is no logging 
+by default, however sometimes additional logging is helpful.  You can get 
+request logging by passing `debug=True` to PterodactylClient.
+
+```python
+app_api = PterodactylClient('https://why', 'broken', debug=True)
+app_api.servers.list_servers(includes=('egg', 'nest'))
+DEBUG:urllib3.connectionpool:Starting new HTTPS connection (1): why:443
+DEBUG:urllib3.connectionpool:https://why:443 "GET /api/application/servers?include=egg%2Cnest HTTP/1.1" 200 None
+```
+
+## Paginated Responses
+
+Pydactyl API responses return
+a [PaginatedResponse object](pydactyl/responses.py#L4) that can be iterated over
+to automatically fetch additional pages as required. This is currently 
+implemented on many endpoints which frequently return multi-page responses, 
+but not all.
+
+```python
+# Create a list of all ports
+allocs = api.nodes.list_node_allocations(node_id)
+ports = []
+for page in allocs:
+    for item in page:
+        ports.append(item['attributes']['port'])
+len(ports)
+151
+```
+
+#### collect()
+
+The `collect()` method will fetch the data from all pages of a
+PaginatedResponse. This allows you to easily fetch all results when you want all
+the data without having to iterate over the pages.
+
+The above example to get a list of ports now looks like:
+
+```python
+# Create a list of all ports
+allocs = api.nodes.list_node_allocations(node_id)
+ports = allocs.collect()
+len(ports)
+151
+```
+
+[docs]: https://pydactyl.readthedocs.io/
+
+[docs-img]: https://readthedocs.org/projects/pydactyl/badge/?version=latest (Latest docs)
+
+[pulls]: https://github.com/iamkubi/pydactyl/pulls
+
+[issues]: https://github.com/iamkubi/pydactyl/issues
+
+[pypi]: https://pypi.python.org/pypi/py-dactyl/
+
+[pypi-img]: https://img.shields.io/pypi/v/py-dactyl.svg
+
+[codecov]: https://codecov.io/gh/iamkubi/pydactyl
+
+[codecov-img]: https://codecov.io/gh/iamkubi/pydactyl/branch/main/graph/badge.svg
+
+[discord-img]: https://img.shields.io/badge/discord-join-7289DA.svg?logo=discord&longCache=true&style=flat
+
+[discord-join]: https://discord.gg/TgZDHPB
+
+[lint-and-test]: https://github.com/iamkubi/pydactyl/actions/workflows/lint-and-test.yml/badge.svg?branch=main (https://github.com/iamkubi/pydactyl/actions/workflows/lint-and-test.yml)
```

### Comparing `py-dactyl-2.0.1/README.md` & `py-dactyl-2.0.2/py_dactyl.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,314 +1,331 @@
-# pydactyl
-
-![lint-and-test]
-[![Latest docs][docs-img]][docs]
-[![Coverage][codecov-img]][codecov]
-[![Latest version][pypi-img]][pypi]
-[![Discord][discord-img]][discord-join]
-
-An easy to use Python wrapper for the Pterodactyl Panel API.
-
-## State of the project
-
-Support for the Pterodactyl 1.x API is complete.
-The 2.0 Pydactyl release was created to standardize how includes and params 
-are passed.  As a result some endpoints (namely nests) **will break** when 
-upgrading from Pydactyl 1.x to 2.0.
-
-Pull Requests are being accepted and new endpoints will continue to be added.
-
-If you encounter problems, find APIs that haven't been implemented, or have a
-feature request please file a [Github issue][issues].
-
-## Documentation
-
-Generated documentation can be found at [https://pydactyl.readthedocs.io/][docs]
-.
-
-## Installing
-
-To install with pip:
-
-```shell
-pip install py-dactyl
-```
-
-**If you get an error saying `ImportError: cannot import name 
-'PterodactylClient' from 'pydactyl'` this probably means you installed the 
-wrong package from pip.**
-
-## Getting Started
-
-**Pterodactyl has two different types of API keys: Client (also known as 
-Account) and Application.**  Any user can generate an Account API key to 
-control their own servers.  The Account API key for an Administrator user will
-be able to access any server's Client API.
-
-Application API keys can only be generated by administrators.  These keys can be used to create, modify, and delete servers, among other things.  They have access to any server on the panel and can be destructive, so use with care.
-
-### Exploring the API
-In addition to the documentation you can explore the interface in an 
-interactive Python interpreter using built-ins like `dir()` and the
-`__doc__` attribute as shown below.
-
-```python
-from pydactyl import PterodactylClient
-api = PterodactylClient('debug', 'anything')
-
-[i for i in dir(api.client.servers) if not i.startswith('_')]
-# ['account', 'backups', 'databases', 'files', 'get_server', 'get_server_utilization', 'list_permissions', 'list_servers', 'network', 'schedules', 'send_console_command', 'send_power_action', 'servers', 'settings', 'startup', 'users']
-[i for i in dir(api.client.servers.settings) if not i.startswith('_')]
-# ['reinstall_server', 'rename_server']
-print(api.client.servers.settings.rename_server.__doc__)
-#Renames the server.
-#        Args:
-#            server_id(str): Server identifier (abbreviated UUID)
-#            name(str): New name for the server
-```
-
-### Client API
-The Client API or Account API is accessed by users of the Pterodactyl panel. 
-Below is the layout of the Client API namespace.
-
-```python
-api.client.account
-api.client.servers
-api.client.servers.backups
-api.client.servers.databases
-api.client.servers.files
-api.client.servers.network
-api.client.servers.schedules
-api.client.servers.settings
-api.client.servers.startup
-api.client.servers.users
-```
-
-A full list of methods available can be found in the [documentation][docs]. 
-
-
-Below are examples of how you might get information about your servers.
-
-```python
-from pydactyl import PterodactylClient
-
-# Create a client to connect to the panel and authenticate with your API key.
-api = PterodactylClient('https://panel.mydomain.com', 'MySuperSecretApiKey')
-
-# Get a list of all servers the user has access to
-my_servers = api.client.servers.list_servers()
-# Get the unique identifier for the first server.
-srv_id = my_servers[0]['attributes']['identifier']
-
-# Check the utilization of the server
-srv_utilization = api.client.servers.get_server_utilization(srv_id)
-print(srv_utilization)
-
-# Turn the server on.
-api.client.servers.send_power_action(srv_id, 'start')
-```
-
-### Application API
-**As of Pterodactyl 1.8.0 Application API keys are deprecated and client API keys should now be used exclusively.**  
-
-The Application API is the administrative API of the Pterodactyl panel. 
-Below is the layout of the Application API namespace.
-
-```python
-api.locations
-api.nests
-api.nodes
-api.servers
-api.user
-```
-
-Below are examples of how you might use this API.
-
-```python
-from pydactyl import PterodactylClient
-
-# Create a client to connect to the panel and authenticate with your API key.
-api = PterodactylClient('https://panel.mydomain.com', 'MySuperSecretApiKey')
-
-# Create a server.  Customize the Nest and Egg IDs to match the IDs in your panel.
-# This server is created with a limit of 8000 MB of memory, no access to swap, unlimited disk space, in location_id 1.
-api.servers.create_server(name='My Paper Server', user_id=1, nest_id=1,
-                          egg_id=3, memory_limit=8000, swap_limit=0,
-                          backup_limit=0, disk_limit=0, location_ids=[1])
-< Response[201] >
-```
-
-A 201 response indicates success, however if there is a problem with the request
-Pydactyl will raise an exception with additional details. When updating the
-location_ids field to an invalid location it displays an error:
-
- ```python
-api.servers.create_server(name='My Paper Server', user_id=1, nest_id=1,
-                          egg_id=3, memory_limit=8000, swap_limit=0,
-                          disk_limit=0, location_ids=[199])
-Traceback (most recent call last):
- File "<input>", line 6, in <module>
- File "D:\code\pydactyl\pydactyl\api\servers.py", line 268, in create_server
-   mode='POST', data=data, json=False)
- File "D:\code\pydactyl\pydactyl\api\base.py", line 98, in _api_request
-   'code'], errors['detail'])
-pydactyl.exceptions.PterodactylApiError: Bad API Request(400) - NoViableNodeException - No nodes satisfying the requirements specified for automatic deployment could be found.
-```
-
-You can use the User class to add, modify, and delete panel users.
-
-```python
-# Create a new user
-result = api.user.create_user('test_user', 'test@gmail.com', 'Test', 'Name')
-# Get the ID of the created user
-user_id = result['attributes']['id']
-# Get the user info, also returned by create_user()
-api.user.get_user_info(user_id)
-{'object': 'user', 'attributes': {'id': 14, 'external_id': None, .... }}
-# Delete the user
-api.user.delete_user(user_id=14)
-```
-
-### Includes
-
-Pterodactyl API endpoints have different sets of includes you can pass to alter 
-the response.  Using includes will cause additional information to show up 
-in the relationships field of the response data.  Some endpoints have no 
-includes and some have many.
-
-Pydactyl docstrings include examples of 
-valid includes for each endpoint, but they are **not an exhaustive list**.
-
-```
-server_includes = [
-    'allocations', 'user', 'subusers', 'pack', 'nest', 'egg', 'variables',
-    'location', 'node', 'databases']
-```
-
-As an example the application server details endpoint has 10 potential 
-includes according to the API docs.  Note that the API docs are not always 
-accurate either!
-
-Most endpoints that generate lists will have optional includes that can be 
-passed as lists or tuples.
-
-```python
-api.nodes.list_nodes(includes=('allocations', 'location'))
-api.servers.get_server_info(
-    server_id=53,
-    includes=['user', 'subusers', 'location'])
-```
-
-### Params
-
-Most endpoints with includes will also have a `params` parameter.  This can 
-be used to pass additional parameters.  Many endpoint specific `params` are 
-already supported by Pydactyl, however some additional params apply 
-universally like `per_page`.
-
-```python
-api.nodes.list_nodes(params={'per_page': 9001})
-api.servers.list_servers(params={'per_page': 9001})
-api.users.list_users(params={'per_page': 9001})
-```
-
-## PterodactylClient
-
-Each of the classes in pydactyl could be imported independently, but the 
-PterodactylClient class [pydactyl/api_client.py](pydactyl/api_client.py) 
-provides a simplified interface that imports libraries for you and provides 
-some convenience features like retries and debug logging.
-
-### Retries
-
-Instances of [PterodactylClient](pydactyl/api_client.py) will automatically
-retry calls that fail with a 429 status code indicating that the request was
-rate-limited by Pterodactyl.
-
-By default it uses a backoff_factor of 1 with 3 retries. You can configure the
-number of retries and backoff_factor when instantiating a client.
-
-```python
-PterodactylClient('panel', 'key', backoff_factor=2, retries=10)
-```
-
-Details on backoff_factor and retires can be found in the
-[urllib3.util.Retry documentation](https://urllib3.readthedocs.io/en/stable/reference/urllib3.util.html#urllib3.util.Retry)
-.
-
-If your server is overloaded or intermittently unavailable you may want to retry
-on other status codes as well. To do this you can pass in a list of integer HTTP
-status codes.
-
-```python
-PterodactylClient('foo', 'bar', extra_retry_codes=[502, 504])
-```
-
-### Debug logging
-
-Most errors from pydactyl will present as exceptions and there is no logging 
-by default, however sometimes additional logging is helpful.  You can get 
-request logging by passing `debug=True` to PterodactylClient.
-
-```python
-app_api = PterodactylClient('https://why', 'broken', debug=True)
-app_api.servers.list_servers(includes=('egg', 'nest'))
-DEBUG:urllib3.connectionpool:Starting new HTTPS connection (1): why:443
-DEBUG:urllib3.connectionpool:https://why:443 "GET /api/application/servers?include=egg%2Cnest HTTP/1.1" 200 None
-```
-
-## Paginated Responses
-
-Pydactyl API responses return
-a [PaginatedResponse object](pydactyl/responses.py#L4) that can be iterated over
-to automatically fetch additional pages as required. This is currently 
-implemented on many endpoints which frequently return multi-page responses, 
-but not all.
-
-```python
-# Create a list of all ports
-allocs = api.nodes.list_node_allocations(node_id)
-ports = []
-for page in allocs:
-    for item in page:
-        ports.append(item['attributes']['port'])
-len(ports)
-151
-```
-
-#### collect()
-
-The `collect()` method will fetch the data from all pages of a
-PaginatedResponse. This allows you to easily fetch all results when you want all
-the data without having to iterate over the pages.
-
-The above example to get a list of ports now looks like:
-
-```python
-# Create a list of all ports
-allocs = api.nodes.list_node_allocations(node_id)
-ports = allocs.collect()
-len(ports)
-151
-```
-
-[docs]: https://pydactyl.readthedocs.io/
-
-[docs-img]: https://readthedocs.org/projects/pydactyl/badge/?version=latest (Latest docs)
-
-[pulls]: https://github.com/iamkubi/pydactyl/pulls
-
-[issues]: https://github.com/iamkubi/pydactyl/issues
-
-[pypi]: https://pypi.python.org/pypi/py-dactyl/
-
-[pypi-img]: https://img.shields.io/pypi/v/py-dactyl.svg
-
-[codecov]: https://codecov.io/gh/iamkubi/pydactyl
-
-[codecov-img]: https://codecov.io/gh/iamkubi/pydactyl/branch/main/graph/badge.svg
-
-[discord-img]: https://img.shields.io/badge/discord-join-7289DA.svg?logo=discord&longCache=true&style=flat
-
-[discord-join]: https://discord.gg/TgZDHPB
-
-[lint-and-test]: https://github.com/iamkubi/pydactyl/actions/workflows/lint-and-test.yml/badge.svg?branch=main (https://github.com/iamkubi/pydactyl/actions/workflows/lint-and-test.yml)
+Metadata-Version: 2.1
+Name: py-dactyl
+Version: 2.0.2
+Summary: An easy to use Python wrapper for the Pterodactyl Panel API.
+Home-page: https://github.com/iamkubi/pydactyl
+Author: Ryan Kubiak
+Author-email: iamkubi@gmail.com
+Project-URL: Documentation, https://pydactyl.readthedocs.io/
+Project-URL: Source, https://github.com/iamkubi/pydactyl
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pydactyl
+
+![lint-and-test]
+[![Latest docs][docs-img]][docs]
+[![Coverage][codecov-img]][codecov]
+[![Latest version][pypi-img]][pypi]
+[![Discord][discord-img]][discord-join]
+
+An easy to use Python wrapper for the Pterodactyl Panel API.
+
+## State of the project
+
+Support for the Pterodactyl 1.x API is complete.
+The 2.0 Pydactyl release was created to standardize how includes and params 
+are passed.  As a result some endpoints (namely nests) **will break** when 
+upgrading from Pydactyl 1.x to 2.0.
+
+Pull Requests are being accepted and new endpoints will continue to be added.
+
+If you encounter problems, find APIs that haven't been implemented, or have a
+feature request please file a [Github issue][issues].
+
+## Documentation
+
+Generated documentation can be found at [https://pydactyl.readthedocs.io/][docs]
+.
+
+## Installing
+
+To install with pip:
+
+```shell
+pip install py-dactyl
+```
+
+**If you get an error saying `ImportError: cannot import name 
+'PterodactylClient' from 'pydactyl'` this probably means you installed the 
+wrong package from pip.**
+
+## Getting Started
+
+**Pterodactyl has two different types of API keys: Client (also known as 
+Account) and Application.**  Any user can generate an Account API key to 
+control their own servers.  The Account API key for an Administrator user will
+be able to access any server's Client API.
+
+Application API keys can only be generated by administrators.  These keys can be used to create, modify, and delete servers, among other things.  They have access to any server on the panel and can be destructive, so use with care.
+
+### Exploring the API
+In addition to the documentation you can explore the interface in an 
+interactive Python interpreter using built-ins like `dir()` and the
+`__doc__` attribute as shown below.
+
+```python
+from pydactyl import PterodactylClient
+api = PterodactylClient('debug', 'anything')
+
+[i for i in dir(api.client.servers) if not i.startswith('_')]
+# ['account', 'backups', 'databases', 'files', 'get_server', 'get_server_utilization', 'list_permissions', 'list_servers', 'network', 'schedules', 'send_console_command', 'send_power_action', 'servers', 'settings', 'startup', 'users']
+[i for i in dir(api.client.servers.settings) if not i.startswith('_')]
+# ['reinstall_server', 'rename_server']
+print(api.client.servers.settings.rename_server.__doc__)
+#Renames the server.
+#        Args:
+#            server_id(str): Server identifier (abbreviated UUID)
+#            name(str): New name for the server
+```
+
+### Client API
+The Client API or Account API is accessed by users of the Pterodactyl panel. 
+Below is the layout of the Client API namespace.
+
+```python
+api.client.account
+api.client.servers
+api.client.servers.backups
+api.client.servers.databases
+api.client.servers.files
+api.client.servers.network
+api.client.servers.schedules
+api.client.servers.settings
+api.client.servers.startup
+api.client.servers.users
+```
+
+A full list of methods available can be found in the [documentation][docs]. 
+
+
+Below are examples of how you might get information about your servers.
+
+```python
+from pydactyl import PterodactylClient
+
+# Create a client to connect to the panel and authenticate with your API key.
+api = PterodactylClient('https://panel.mydomain.com', 'MySuperSecretApiKey')
+
+# Get a list of all servers the user has access to
+my_servers = api.client.servers.list_servers()
+# Get the unique identifier for the first server.
+srv_id = my_servers[0]['attributes']['identifier']
+
+# Check the utilization of the server
+srv_utilization = api.client.servers.get_server_utilization(srv_id)
+print(srv_utilization)
+
+# Turn the server on.
+api.client.servers.send_power_action(srv_id, 'start')
+```
+
+### Application API
+**As of Pterodactyl 1.8.0 Application API keys are deprecated and client API keys should now be used exclusively.**  
+
+The Application API is the administrative API of the Pterodactyl panel. 
+Below is the layout of the Application API namespace.
+
+```python
+api.locations
+api.nests
+api.nodes
+api.servers
+api.user
+```
+
+Below are examples of how you might use this API.
+
+```python
+from pydactyl import PterodactylClient
+
+# Create a client to connect to the panel and authenticate with your API key.
+api = PterodactylClient('https://panel.mydomain.com', 'MySuperSecretApiKey')
+
+# Create a server.  Customize the Nest and Egg IDs to match the IDs in your panel.
+# This server is created with a limit of 8000 MB of memory, no access to swap, unlimited disk space, in location_id 1.
+api.servers.create_server(name='My Paper Server', user_id=1, nest_id=1,
+                          egg_id=3, memory_limit=8000, swap_limit=0,
+                          backup_limit=0, disk_limit=0, location_ids=[1])
+< Response[201] >
+```
+
+A 201 response indicates success, however if there is a problem with the request
+Pydactyl will raise an exception with additional details. When updating the
+location_ids field to an invalid location it displays an error:
+
+ ```python
+api.servers.create_server(name='My Paper Server', user_id=1, nest_id=1,
+                          egg_id=3, memory_limit=8000, swap_limit=0,
+                          disk_limit=0, location_ids=[199])
+Traceback (most recent call last):
+ File "<input>", line 6, in <module>
+ File "D:\code\pydactyl\pydactyl\api\servers.py", line 268, in create_server
+   mode='POST', data=data, json=False)
+ File "D:\code\pydactyl\pydactyl\api\base.py", line 98, in _api_request
+   'code'], errors['detail'])
+pydactyl.exceptions.PterodactylApiError: Bad API Request(400) - NoViableNodeException - No nodes satisfying the requirements specified for automatic deployment could be found.
+```
+
+You can use the User class to add, modify, and delete panel users.
+
+```python
+# Create a new user
+result = api.user.create_user('test_user', 'test@gmail.com', 'Test', 'Name')
+# Get the ID of the created user
+user_id = result['attributes']['id']
+# Get the user info, also returned by create_user()
+api.user.get_user_info(user_id)
+{'object': 'user', 'attributes': {'id': 14, 'external_id': None, .... }}
+# Delete the user
+api.user.delete_user(user_id=14)
+```
+
+### Includes
+
+Pterodactyl API endpoints have different sets of includes you can pass to alter 
+the response.  Using includes will cause additional information to show up 
+in the relationships field of the response data.  Some endpoints have no 
+includes and some have many.
+
+Pydactyl docstrings include examples of 
+valid includes for each endpoint, but they are **not an exhaustive list**.
+
+```
+server_includes = [
+    'allocations', 'user', 'subusers', 'pack', 'nest', 'egg', 'variables',
+    'location', 'node', 'databases']
+```
+
+As an example the application server details endpoint has 10 potential 
+includes according to the API docs.  Note that the API docs are not always 
+accurate either!
+
+Most endpoints that generate lists will have optional includes that can be 
+passed as lists or tuples.
+
+```python
+api.nodes.list_nodes(includes=('allocations', 'location'))
+api.servers.get_server_info(
+    server_id=53,
+    includes=['user', 'subusers', 'location'])
+```
+
+### Params
+
+Most endpoints with includes will also have a `params` parameter.  This can 
+be used to pass additional parameters.  Many endpoint specific `params` are 
+already supported by Pydactyl, however some additional params apply 
+universally like `per_page`.
+
+```python
+api.nodes.list_nodes(params={'per_page': 9001})
+api.servers.list_servers(params={'per_page': 9001})
+api.users.list_users(params={'per_page': 9001})
+```
+
+## PterodactylClient
+
+Each of the classes in pydactyl could be imported independently, but the 
+PterodactylClient class [pydactyl/api_client.py](pydactyl/api_client.py) 
+provides a simplified interface that imports libraries for you and provides 
+some convenience features like retries and debug logging.
+
+### Retries
+
+Instances of [PterodactylClient](pydactyl/api_client.py) will automatically
+retry calls that fail with a 429 status code indicating that the request was
+rate-limited by Pterodactyl.
+
+By default it uses a backoff_factor of 1 with 3 retries. You can configure the
+number of retries and backoff_factor when instantiating a client.
+
+```python
+PterodactylClient('panel', 'key', backoff_factor=2, retries=10)
+```
+
+Details on backoff_factor and retires can be found in the
+[urllib3.util.Retry documentation](https://urllib3.readthedocs.io/en/stable/reference/urllib3.util.html#urllib3.util.Retry)
+.
+
+If your server is overloaded or intermittently unavailable you may want to retry
+on other status codes as well. To do this you can pass in a list of integer HTTP
+status codes.
+
+```python
+PterodactylClient('foo', 'bar', extra_retry_codes=[502, 504])
+```
+
+### Debug logging
+
+Most errors from pydactyl will present as exceptions and there is no logging 
+by default, however sometimes additional logging is helpful.  You can get 
+request logging by passing `debug=True` to PterodactylClient.
+
+```python
+app_api = PterodactylClient('https://why', 'broken', debug=True)
+app_api.servers.list_servers(includes=('egg', 'nest'))
+DEBUG:urllib3.connectionpool:Starting new HTTPS connection (1): why:443
+DEBUG:urllib3.connectionpool:https://why:443 "GET /api/application/servers?include=egg%2Cnest HTTP/1.1" 200 None
+```
+
+## Paginated Responses
+
+Pydactyl API responses return
+a [PaginatedResponse object](pydactyl/responses.py#L4) that can be iterated over
+to automatically fetch additional pages as required. This is currently 
+implemented on many endpoints which frequently return multi-page responses, 
+but not all.
+
+```python
+# Create a list of all ports
+allocs = api.nodes.list_node_allocations(node_id)
+ports = []
+for page in allocs:
+    for item in page:
+        ports.append(item['attributes']['port'])
+len(ports)
+151
+```
+
+#### collect()
+
+The `collect()` method will fetch the data from all pages of a
+PaginatedResponse. This allows you to easily fetch all results when you want all
+the data without having to iterate over the pages.
+
+The above example to get a list of ports now looks like:
+
+```python
+# Create a list of all ports
+allocs = api.nodes.list_node_allocations(node_id)
+ports = allocs.collect()
+len(ports)
+151
+```
+
+[docs]: https://pydactyl.readthedocs.io/
+
+[docs-img]: https://readthedocs.org/projects/pydactyl/badge/?version=latest (Latest docs)
+
+[pulls]: https://github.com/iamkubi/pydactyl/pulls
+
+[issues]: https://github.com/iamkubi/pydactyl/issues
+
+[pypi]: https://pypi.python.org/pypi/py-dactyl/
+
+[pypi-img]: https://img.shields.io/pypi/v/py-dactyl.svg
+
+[codecov]: https://codecov.io/gh/iamkubi/pydactyl
+
+[codecov-img]: https://codecov.io/gh/iamkubi/pydactyl/branch/main/graph/badge.svg
+
+[discord-img]: https://img.shields.io/badge/discord-join-7289DA.svg?logo=discord&longCache=true&style=flat
+
+[discord-join]: https://discord.gg/TgZDHPB
+
+[lint-and-test]: https://github.com/iamkubi/pydactyl/actions/workflows/lint-and-test.yml/badge.svg?branch=main (https://github.com/iamkubi/pydactyl/actions/workflows/lint-and-test.yml)
```

### Comparing `py-dactyl-2.0.1/py_dactyl.egg-info/PKG-INFO` & `py-dactyl-2.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,335 +1,314 @@
-Metadata-Version: 2.1
-Name: py-dactyl
-Version: 2.0.1
-Summary: An easy to use Python wrapper for the Pterodactyl Panel API.
-Home-page: https://github.com/iamkubi/pydactyl
-Author: Ryan Kubiak
-Author-email: iamkubi@gmail.com
-License: UNKNOWN
-Project-URL: Documentation, https://pydactyl.readthedocs.io/
-Project-URL: Source, https://github.com/iamkubi/pydactyl
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pydactyl
-
-![lint-and-test]
-[![Latest docs][docs-img]][docs]
-[![Coverage][codecov-img]][codecov]
-[![Latest version][pypi-img]][pypi]
-[![Discord][discord-img]][discord-join]
-
-An easy to use Python wrapper for the Pterodactyl Panel API.
-
-## State of the project
-
-Support for the Pterodactyl 1.x API is complete.
-The 2.0 Pydactyl release was created to standardize how includes and params 
-are passed.  As a result some endpoints (namely nests) **will break** when 
-upgrading from Pydactyl 1.x to 2.0.
-
-Pull Requests are being accepted and new endpoints will continue to be added.
-
-If you encounter problems, find APIs that haven't been implemented, or have a
-feature request please file a [Github issue][issues].
-
-## Documentation
-
-Generated documentation can be found at [https://pydactyl.readthedocs.io/][docs]
-.
-
-## Installing
-
-To install with pip:
-
-```shell
-pip install py-dactyl
-```
-
-**If you get an error saying `ImportError: cannot import name 
-'PterodactylClient' from 'pydactyl'` this probably means you installed the 
-wrong package from pip.**
-
-## Getting Started
-
-**Pterodactyl has two different types of API keys: Client (also known as 
-Account) and Application.**  Any user can generate an Account API key to 
-control their own servers.  The Account API key for an Administrator user will
-be able to access any server's Client API.
-
-Application API keys can only be generated by administrators.  These keys can be used to create, modify, and delete servers, among other things.  They have access to any server on the panel and can be destructive, so use with care.
-
-### Exploring the API
-In addition to the documentation you can explore the interface in an 
-interactive Python interpreter using built-ins like `dir()` and the
-`__doc__` attribute as shown below.
-
-```python
-from pydactyl import PterodactylClient
-api = PterodactylClient('debug', 'anything')
-
-[i for i in dir(api.client.servers) if not i.startswith('_')]
-# ['account', 'backups', 'databases', 'files', 'get_server', 'get_server_utilization', 'list_permissions', 'list_servers', 'network', 'schedules', 'send_console_command', 'send_power_action', 'servers', 'settings', 'startup', 'users']
-[i for i in dir(api.client.servers.settings) if not i.startswith('_')]
-# ['reinstall_server', 'rename_server']
-print(api.client.servers.settings.rename_server.__doc__)
-#Renames the server.
-#        Args:
-#            server_id(str): Server identifier (abbreviated UUID)
-#            name(str): New name for the server
-```
-
-### Client API
-The Client API or Account API is accessed by users of the Pterodactyl panel. 
-Below is the layout of the Client API namespace.
-
-```python
-api.client.account
-api.client.servers
-api.client.servers.backups
-api.client.servers.databases
-api.client.servers.files
-api.client.servers.network
-api.client.servers.schedules
-api.client.servers.settings
-api.client.servers.startup
-api.client.servers.users
-```
-
-A full list of methods available can be found in the [documentation][docs]. 
-
-
-Below are examples of how you might get information about your servers.
-
-```python
-from pydactyl import PterodactylClient
-
-# Create a client to connect to the panel and authenticate with your API key.
-api = PterodactylClient('https://panel.mydomain.com', 'MySuperSecretApiKey')
-
-# Get a list of all servers the user has access to
-my_servers = api.client.servers.list_servers()
-# Get the unique identifier for the first server.
-srv_id = my_servers[0]['attributes']['identifier']
-
-# Check the utilization of the server
-srv_utilization = api.client.servers.get_server_utilization(srv_id)
-print(srv_utilization)
-
-# Turn the server on.
-api.client.servers.send_power_action(srv_id, 'start')
-```
-
-### Application API
-**As of Pterodactyl 1.8.0 Application API keys are deprecated and client API keys should now be used exclusively.**  
-
-The Application API is the administrative API of the Pterodactyl panel. 
-Below is the layout of the Application API namespace.
-
-```python
-api.locations
-api.nests
-api.nodes
-api.servers
-api.user
-```
-
-Below are examples of how you might use this API.
-
-```python
-from pydactyl import PterodactylClient
-
-# Create a client to connect to the panel and authenticate with your API key.
-api = PterodactylClient('https://panel.mydomain.com', 'MySuperSecretApiKey')
-
-# Create a server.  Customize the Nest and Egg IDs to match the IDs in your panel.
-# This server is created with a limit of 8000 MB of memory, no access to swap, unlimited disk space, in location_id 1.
-api.servers.create_server(name='My Paper Server', user_id=1, nest_id=1,
-                          egg_id=3, memory_limit=8000, swap_limit=0,
-                          backup_limit=0, disk_limit=0, location_ids=[1])
-< Response[201] >
-```
-
-A 201 response indicates success, however if there is a problem with the request
-Pydactyl will raise an exception with additional details. When updating the
-location_ids field to an invalid location it displays an error:
-
- ```python
-api.servers.create_server(name='My Paper Server', user_id=1, nest_id=1,
-                          egg_id=3, memory_limit=8000, swap_limit=0,
-                          disk_limit=0, location_ids=[199])
-Traceback (most recent call last):
- File "<input>", line 6, in <module>
- File "D:\code\pydactyl\pydactyl\api\servers.py", line 268, in create_server
-   mode='POST', data=data, json=False)
- File "D:\code\pydactyl\pydactyl\api\base.py", line 98, in _api_request
-   'code'], errors['detail'])
-pydactyl.exceptions.PterodactylApiError: Bad API Request(400) - NoViableNodeException - No nodes satisfying the requirements specified for automatic deployment could be found.
-```
-
-You can use the User class to add, modify, and delete panel users.
-
-```python
-# Create a new user
-result = api.user.create_user('test_user', 'test@gmail.com', 'Test', 'Name')
-# Get the ID of the created user
-user_id = result['attributes']['id']
-# Get the user info, also returned by create_user()
-api.user.get_user_info(user_id)
-{'object': 'user', 'attributes': {'id': 14, 'external_id': None, .... }}
-# Delete the user
-api.user.delete_user(user_id=14)
-```
-
-### Includes
-
-Pterodactyl API endpoints have different sets of includes you can pass to alter 
-the response.  Using includes will cause additional information to show up 
-in the relationships field of the response data.  Some endpoints have no 
-includes and some have many.
-
-Pydactyl docstrings include examples of 
-valid includes for each endpoint, but they are **not an exhaustive list**.
-
-```
-server_includes = [
-    'allocations', 'user', 'subusers', 'pack', 'nest', 'egg', 'variables',
-    'location', 'node', 'databases']
-```
-
-As an example the application server details endpoint has 10 potential 
-includes according to the API docs.  Note that the API docs are not always 
-accurate either!
-
-Most endpoints that generate lists will have optional includes that can be 
-passed as lists or tuples.
-
-```python
-api.nodes.list_nodes(includes=('allocations', 'location'))
-api.servers.get_server_info(
-    server_id=53,
-    includes=['user', 'subusers', 'location'])
-```
-
-### Params
-
-Most endpoints with includes will also have a `params` parameter.  This can 
-be used to pass additional parameters.  Many endpoint specific `params` are 
-already supported by Pydactyl, however some additional params apply 
-universally like `per_page`.
-
-```python
-api.nodes.list_nodes(params={'per_page': 9001})
-api.servers.list_servers(params={'per_page': 9001})
-api.users.list_users(params={'per_page': 9001})
-```
-
-## PterodactylClient
-
-Each of the classes in pydactyl could be imported independently, but the 
-PterodactylClient class [pydactyl/api_client.py](pydactyl/api_client.py) 
-provides a simplified interface that imports libraries for you and provides 
-some convenience features like retries and debug logging.
-
-### Retries
-
-Instances of [PterodactylClient](pydactyl/api_client.py) will automatically
-retry calls that fail with a 429 status code indicating that the request was
-rate-limited by Pterodactyl.
-
-By default it uses a backoff_factor of 1 with 3 retries. You can configure the
-number of retries and backoff_factor when instantiating a client.
-
-```python
-PterodactylClient('panel', 'key', backoff_factor=2, retries=10)
-```
-
-Details on backoff_factor and retires can be found in the
-[urllib3.util.Retry documentation](https://urllib3.readthedocs.io/en/stable/reference/urllib3.util.html#urllib3.util.Retry)
-.
-
-If your server is overloaded or intermittently unavailable you may want to retry
-on other status codes as well. To do this you can pass in a list of integer HTTP
-status codes.
-
-```python
-PterodactylClient('foo', 'bar', extra_retry_codes=[502, 504])
-```
-
-### Debug logging
-
-Most errors from pydactyl will present as exceptions and there is no logging 
-by default, however sometimes additional logging is helpful.  You can get 
-request logging by passing `debug=True` to PterodactylClient.
-
-```python
-app_api = PterodactylClient('https://why', 'broken', debug=True)
-app_api.servers.list_servers(includes=('egg', 'nest'))
-DEBUG:urllib3.connectionpool:Starting new HTTPS connection (1): why:443
-DEBUG:urllib3.connectionpool:https://why:443 "GET /api/application/servers?include=egg%2Cnest HTTP/1.1" 200 None
-```
-
-## Paginated Responses
-
-Pydactyl API responses return
-a [PaginatedResponse object](pydactyl/responses.py#L4) that can be iterated over
-to automatically fetch additional pages as required. This is currently 
-implemented on many endpoints which frequently return multi-page responses, 
-but not all.
-
-```python
-# Create a list of all ports
-allocs = api.nodes.list_node_allocations(node_id)
-ports = []
-for page in allocs:
-    for item in page:
-        ports.append(item['attributes']['port'])
-len(ports)
-151
-```
-
-#### collect()
-
-The `collect()` method will fetch the data from all pages of a
-PaginatedResponse. This allows you to easily fetch all results when you want all
-the data without having to iterate over the pages.
-
-The above example to get a list of ports now looks like:
-
-```python
-# Create a list of all ports
-allocs = api.nodes.list_node_allocations(node_id)
-ports = allocs.collect()
-len(ports)
-151
-```
-
-[docs]: https://pydactyl.readthedocs.io/
-
-[docs-img]: https://readthedocs.org/projects/pydactyl/badge/?version=latest (Latest docs)
-
-[pulls]: https://github.com/iamkubi/pydactyl/pulls
-
-[issues]: https://github.com/iamkubi/pydactyl/issues
-
-[pypi]: https://pypi.python.org/pypi/py-dactyl/
-
-[pypi-img]: https://img.shields.io/pypi/v/py-dactyl.svg
-
-[codecov]: https://codecov.io/gh/iamkubi/pydactyl
-
-[codecov-img]: https://codecov.io/gh/iamkubi/pydactyl/branch/main/graph/badge.svg
-
-[discord-img]: https://img.shields.io/badge/discord-join-7289DA.svg?logo=discord&longCache=true&style=flat
-
-[discord-join]: https://discord.gg/TgZDHPB
-
-[lint-and-test]: https://github.com/iamkubi/pydactyl/actions/workflows/lint-and-test.yml/badge.svg?branch=main (https://github.com/iamkubi/pydactyl/actions/workflows/lint-and-test.yml)
-
-
+# pydactyl
+
+![lint-and-test]
+[![Latest docs][docs-img]][docs]
+[![Coverage][codecov-img]][codecov]
+[![Latest version][pypi-img]][pypi]
+[![Discord][discord-img]][discord-join]
+
+An easy to use Python wrapper for the Pterodactyl Panel API.
+
+## State of the project
+
+Support for the Pterodactyl 1.x API is complete.
+The 2.0 Pydactyl release was created to standardize how includes and params 
+are passed.  As a result some endpoints (namely nests) **will break** when 
+upgrading from Pydactyl 1.x to 2.0.
+
+Pull Requests are being accepted and new endpoints will continue to be added.
+
+If you encounter problems, find APIs that haven't been implemented, or have a
+feature request please file a [Github issue][issues].
+
+## Documentation
+
+Generated documentation can be found at [https://pydactyl.readthedocs.io/][docs]
+.
+
+## Installing
+
+To install with pip:
+
+```shell
+pip install py-dactyl
+```
+
+**If you get an error saying `ImportError: cannot import name 
+'PterodactylClient' from 'pydactyl'` this probably means you installed the 
+wrong package from pip.**
+
+## Getting Started
+
+**Pterodactyl has two different types of API keys: Client (also known as 
+Account) and Application.**  Any user can generate an Account API key to 
+control their own servers.  The Account API key for an Administrator user will
+be able to access any server's Client API.
+
+Application API keys can only be generated by administrators.  These keys can be used to create, modify, and delete servers, among other things.  They have access to any server on the panel and can be destructive, so use with care.
+
+### Exploring the API
+In addition to the documentation you can explore the interface in an 
+interactive Python interpreter using built-ins like `dir()` and the
+`__doc__` attribute as shown below.
+
+```python
+from pydactyl import PterodactylClient
+api = PterodactylClient('debug', 'anything')
+
+[i for i in dir(api.client.servers) if not i.startswith('_')]
+# ['account', 'backups', 'databases', 'files', 'get_server', 'get_server_utilization', 'list_permissions', 'list_servers', 'network', 'schedules', 'send_console_command', 'send_power_action', 'servers', 'settings', 'startup', 'users']
+[i for i in dir(api.client.servers.settings) if not i.startswith('_')]
+# ['reinstall_server', 'rename_server']
+print(api.client.servers.settings.rename_server.__doc__)
+#Renames the server.
+#        Args:
+#            server_id(str): Server identifier (abbreviated UUID)
+#            name(str): New name for the server
+```
+
+### Client API
+The Client API or Account API is accessed by users of the Pterodactyl panel. 
+Below is the layout of the Client API namespace.
+
+```python
+api.client.account
+api.client.servers
+api.client.servers.backups
+api.client.servers.databases
+api.client.servers.files
+api.client.servers.network
+api.client.servers.schedules
+api.client.servers.settings
+api.client.servers.startup
+api.client.servers.users
+```
+
+A full list of methods available can be found in the [documentation][docs]. 
+
+
+Below are examples of how you might get information about your servers.
+
+```python
+from pydactyl import PterodactylClient
+
+# Create a client to connect to the panel and authenticate with your API key.
+api = PterodactylClient('https://panel.mydomain.com', 'MySuperSecretApiKey')
+
+# Get a list of all servers the user has access to
+my_servers = api.client.servers.list_servers()
+# Get the unique identifier for the first server.
+srv_id = my_servers[0]['attributes']['identifier']
+
+# Check the utilization of the server
+srv_utilization = api.client.servers.get_server_utilization(srv_id)
+print(srv_utilization)
+
+# Turn the server on.
+api.client.servers.send_power_action(srv_id, 'start')
+```
+
+### Application API
+**As of Pterodactyl 1.8.0 Application API keys are deprecated and client API keys should now be used exclusively.**  
+
+The Application API is the administrative API of the Pterodactyl panel. 
+Below is the layout of the Application API namespace.
+
+```python
+api.locations
+api.nests
+api.nodes
+api.servers
+api.user
+```
+
+Below are examples of how you might use this API.
+
+```python
+from pydactyl import PterodactylClient
+
+# Create a client to connect to the panel and authenticate with your API key.
+api = PterodactylClient('https://panel.mydomain.com', 'MySuperSecretApiKey')
+
+# Create a server.  Customize the Nest and Egg IDs to match the IDs in your panel.
+# This server is created with a limit of 8000 MB of memory, no access to swap, unlimited disk space, in location_id 1.
+api.servers.create_server(name='My Paper Server', user_id=1, nest_id=1,
+                          egg_id=3, memory_limit=8000, swap_limit=0,
+                          backup_limit=0, disk_limit=0, location_ids=[1])
+< Response[201] >
+```
+
+A 201 response indicates success, however if there is a problem with the request
+Pydactyl will raise an exception with additional details. When updating the
+location_ids field to an invalid location it displays an error:
+
+ ```python
+api.servers.create_server(name='My Paper Server', user_id=1, nest_id=1,
+                          egg_id=3, memory_limit=8000, swap_limit=0,
+                          disk_limit=0, location_ids=[199])
+Traceback (most recent call last):
+ File "<input>", line 6, in <module>
+ File "D:\code\pydactyl\pydactyl\api\servers.py", line 268, in create_server
+   mode='POST', data=data, json=False)
+ File "D:\code\pydactyl\pydactyl\api\base.py", line 98, in _api_request
+   'code'], errors['detail'])
+pydactyl.exceptions.PterodactylApiError: Bad API Request(400) - NoViableNodeException - No nodes satisfying the requirements specified for automatic deployment could be found.
+```
+
+You can use the User class to add, modify, and delete panel users.
+
+```python
+# Create a new user
+result = api.user.create_user('test_user', 'test@gmail.com', 'Test', 'Name')
+# Get the ID of the created user
+user_id = result['attributes']['id']
+# Get the user info, also returned by create_user()
+api.user.get_user_info(user_id)
+{'object': 'user', 'attributes': {'id': 14, 'external_id': None, .... }}
+# Delete the user
+api.user.delete_user(user_id=14)
+```
+
+### Includes
+
+Pterodactyl API endpoints have different sets of includes you can pass to alter 
+the response.  Using includes will cause additional information to show up 
+in the relationships field of the response data.  Some endpoints have no 
+includes and some have many.
+
+Pydactyl docstrings include examples of 
+valid includes for each endpoint, but they are **not an exhaustive list**.
+
+```
+server_includes = [
+    'allocations', 'user', 'subusers', 'pack', 'nest', 'egg', 'variables',
+    'location', 'node', 'databases']
+```
+
+As an example the application server details endpoint has 10 potential 
+includes according to the API docs.  Note that the API docs are not always 
+accurate either!
+
+Most endpoints that generate lists will have optional includes that can be 
+passed as lists or tuples.
+
+```python
+api.nodes.list_nodes(includes=('allocations', 'location'))
+api.servers.get_server_info(
+    server_id=53,
+    includes=['user', 'subusers', 'location'])
+```
+
+### Params
+
+Most endpoints with includes will also have a `params` parameter.  This can 
+be used to pass additional parameters.  Many endpoint specific `params` are 
+already supported by Pydactyl, however some additional params apply 
+universally like `per_page`.
+
+```python
+api.nodes.list_nodes(params={'per_page': 9001})
+api.servers.list_servers(params={'per_page': 9001})
+api.users.list_users(params={'per_page': 9001})
+```
+
+## PterodactylClient
+
+Each of the classes in pydactyl could be imported independently, but the 
+PterodactylClient class [pydactyl/api_client.py](pydactyl/api_client.py) 
+provides a simplified interface that imports libraries for you and provides 
+some convenience features like retries and debug logging.
+
+### Retries
+
+Instances of [PterodactylClient](pydactyl/api_client.py) will automatically
+retry calls that fail with a 429 status code indicating that the request was
+rate-limited by Pterodactyl.
+
+By default it uses a backoff_factor of 1 with 3 retries. You can configure the
+number of retries and backoff_factor when instantiating a client.
+
+```python
+PterodactylClient('panel', 'key', backoff_factor=2, retries=10)
+```
+
+Details on backoff_factor and retires can be found in the
+[urllib3.util.Retry documentation](https://urllib3.readthedocs.io/en/stable/reference/urllib3.util.html#urllib3.util.Retry)
+.
+
+If your server is overloaded or intermittently unavailable you may want to retry
+on other status codes as well. To do this you can pass in a list of integer HTTP
+status codes.
+
+```python
+PterodactylClient('foo', 'bar', extra_retry_codes=[502, 504])
+```
+
+### Debug logging
+
+Most errors from pydactyl will present as exceptions and there is no logging 
+by default, however sometimes additional logging is helpful.  You can get 
+request logging by passing `debug=True` to PterodactylClient.
+
+```python
+app_api = PterodactylClient('https://why', 'broken', debug=True)
+app_api.servers.list_servers(includes=('egg', 'nest'))
+DEBUG:urllib3.connectionpool:Starting new HTTPS connection (1): why:443
+DEBUG:urllib3.connectionpool:https://why:443 "GET /api/application/servers?include=egg%2Cnest HTTP/1.1" 200 None
+```
+
+## Paginated Responses
+
+Pydactyl API responses return
+a [PaginatedResponse object](pydactyl/responses.py#L4) that can be iterated over
+to automatically fetch additional pages as required. This is currently 
+implemented on many endpoints which frequently return multi-page responses, 
+but not all.
+
+```python
+# Create a list of all ports
+allocs = api.nodes.list_node_allocations(node_id)
+ports = []
+for page in allocs:
+    for item in page:
+        ports.append(item['attributes']['port'])
+len(ports)
+151
+```
+
+#### collect()
+
+The `collect()` method will fetch the data from all pages of a
+PaginatedResponse. This allows you to easily fetch all results when you want all
+the data without having to iterate over the pages.
+
+The above example to get a list of ports now looks like:
+
+```python
+# Create a list of all ports
+allocs = api.nodes.list_node_allocations(node_id)
+ports = allocs.collect()
+len(ports)
+151
+```
+
+[docs]: https://pydactyl.readthedocs.io/
+
+[docs-img]: https://readthedocs.org/projects/pydactyl/badge/?version=latest (Latest docs)
+
+[pulls]: https://github.com/iamkubi/pydactyl/pulls
+
+[issues]: https://github.com/iamkubi/pydactyl/issues
+
+[pypi]: https://pypi.python.org/pypi/py-dactyl/
+
+[pypi-img]: https://img.shields.io/pypi/v/py-dactyl.svg
+
+[codecov]: https://codecov.io/gh/iamkubi/pydactyl
+
+[codecov-img]: https://codecov.io/gh/iamkubi/pydactyl/branch/main/graph/badge.svg
+
+[discord-img]: https://img.shields.io/badge/discord-join-7289DA.svg?logo=discord&longCache=true&style=flat
+
+[discord-join]: https://discord.gg/TgZDHPB
+
+[lint-and-test]: https://github.com/iamkubi/pydactyl/actions/workflows/lint-and-test.yml/badge.svg?branch=main (https://github.com/iamkubi/pydactyl/actions/workflows/lint-and-test.yml)
```

### Comparing `py-dactyl-2.0.1/py_dactyl.egg-info/SOURCES.txt` & `py-dactyl-2.0.2/py_dactyl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.1/pydactyl/api/base.py` & `py-dactyl-2.0.2/pydactyl/api/base.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,134 +1,134 @@
-import requests
-
-from pydactyl.constants import REQUEST_TYPES
-from pydactyl.exceptions import BadRequestError
-from pydactyl.exceptions import PterodactylApiError
-
-
-def parse_response(response, detail=False):
-    """Parse the response data.
-
-    Optionally includes additional data that specifies the object type
-    and requires accessing the data through a nested dictionary.  The
-    Client API doesn't include any additional information, but the
-    Servers API includes created and updated timestamps in the detailed
-    response.
-
-    Args:
-         response(dict): A request response object.
-         detail(bool): Include additional data from the raw response.
-    """
-    if detail:
-        data = response
-    else:
-        if response['object'] == 'list':
-            data = [item.get('attributes') for item in response.get('data')]
-        else:
-            data = response.get('attributes')
-
-    return data
-
-
-def url_join(*args):
-    """Join combine URL parts to get the full endpoint address."""
-    return '/'.join(arg.strip('/') for arg in args)
-
-
-class PterodactylAPI(object):
-    """Pterodactyl API client."""
-
-    def __init__(self, url, api_key, session=None):
-        self._api_key = api_key
-        self._url = url
-        self._session = session or requests.Session()
-
-    def _get_headers(self):
-        """Headers to use for API calls."""
-        headers = {
-            'Authorization': 'Bearer {0}'.format(self._api_key),
-            'Accept': 'application/json',
-            'Content-Type': 'application/json',
-        }
-        return headers
-
-    def _api_request(self, endpoint, mode='GET', params=None, data=None,
-                     json=None, override_headers=None, data_as_json=True,
-                     includes=None):
-        """Make a request to the Pterodactyl API.
-
-        Args:
-            endpoint(str): URI for the API
-            mode(str): Request type, one of ('GET', 'POST', 'PATCH',
-                    'DELETE', 'PUT')
-            params(dict): Extra parameters to pass to the endpoint,
-                    e.g. a query string
-            data(dict): POST data
-            json(bool): Set to False to return the response object,
-                    True for just JSON.  Defaults to returning JSON if possible
-                    otherwise the response object.
-            override_headers(dict): Headers to override, e.g. to set the
-                    Content-Type
-            data_as_json(bool): If True data will be posted as JSON
-            includes(iter): List of includes to be added as a param,
-                    e.g. ('servers', 'users')
-
-        Returns:
-            response: A HTTP response object or the JSON response depending on
-                    the value of the json parameter.
-        """
-        if not endpoint:
-            raise BadRequestError('No API endpoint was specified.')
-
-        url = url_join(self._url, 'api', endpoint)
-        headers = self._get_headers()
-        if override_headers:
-            headers.update(override_headers)
-
-        if includes:
-            include_str = ','.join(includes)
-            if params and params.get('include'):
-                params['include'] += ',' + include_str
-            elif params:
-                params['include'] = include_str
-            else:
-                params = {'include': include_str}
-
-        if mode == 'GET':
-            response = self._session.get(url, params=params, headers=headers)
-        elif mode == 'POST':
-            if data_as_json:
-                response = self._session.post(url, params=params,
-                                              headers=headers, json=data)
-            else:
-                response = self._session.post(url, params=params,
-                                              headers=headers, data=data)
-        elif mode == 'PATCH':
-            response = self._session.patch(url, params=params, headers=headers,
-                                           json=data)
-        elif mode == 'DELETE':
-            response = self._session.delete(url, params=params, headers=headers)
-        elif mode == 'PUT':
-            response = self._session.put(url, params=params, headers=headers,
-                                         json=data)
-        else:
-            raise BadRequestError(
-                'Invalid request type specified(%s).  Must be one of %r.' % (
-                    mode, REQUEST_TYPES))
-
-        try:
-            response_json = response.json()
-        except ValueError:
-            response_json = {}
-
-        if response.status_code in (400, 422):
-            raise PterodactylApiError('API Request resulted in errors: %s' %
-                                      response_json.get('errors'))
-        else:
-            response.raise_for_status()
-
-        if json is True:
-            return response_json
-        elif json is False:
-            return response
-        else:
-            return response_json or response
+import requests
+
+from pydactyl.constants import REQUEST_TYPES
+from pydactyl.exceptions import BadRequestError
+from pydactyl.exceptions import PterodactylApiError
+
+
+def parse_response(response, detail=False):
+    """Parse the response data.
+
+    Optionally includes additional data that specifies the object type
+    and requires accessing the data through a nested dictionary.  The
+    Client API doesn't include any additional information, but the
+    Servers API includes created and updated timestamps in the detailed
+    response.
+
+    Args:
+         response(dict): A request response object.
+         detail(bool): Include additional data from the raw response.
+    """
+    if detail:
+        data = response
+    else:
+        if response['object'] == 'list':
+            data = [item.get('attributes') for item in response.get('data')]
+        else:
+            data = response.get('attributes')
+
+    return data
+
+
+def url_join(*args):
+    """Join combine URL parts to get the full endpoint address."""
+    return '/'.join(arg.strip('/') for arg in args)
+
+
+class PterodactylAPI(object):
+    """Pterodactyl API client."""
+
+    def __init__(self, url, api_key, session=None):
+        self._api_key = api_key
+        self._url = url
+        self._session = session or requests.Session()
+
+    def _get_headers(self):
+        """Headers to use for API calls."""
+        headers = {
+            'Authorization': 'Bearer {0}'.format(self._api_key),
+            'Accept': 'application/json',
+            'Content-Type': 'application/json',
+        }
+        return headers
+
+    def _api_request(self, endpoint, mode='GET', params=None, data=None,
+                     json=None, override_headers=None, data_as_json=True,
+                     includes=None):
+        """Make a request to the Pterodactyl API.
+
+        Args:
+            endpoint(str): URI for the API
+            mode(str): Request type, one of ('GET', 'POST', 'PATCH',
+                    'DELETE', 'PUT')
+            params(dict): Extra parameters to pass to the endpoint,
+                    e.g. a query string
+            data(dict): POST data
+            json(bool): Set to False to return the response object,
+                    True for just JSON.  Defaults to returning JSON if possible
+                    otherwise the response object.
+            override_headers(dict): Headers to override, e.g. to set the
+                    Content-Type
+            data_as_json(bool): If True data will be posted as JSON
+            includes(iter): List of includes to be added as a param,
+                    e.g. ('servers', 'users')
+
+        Returns:
+            response: A HTTP response object or the JSON response depending on
+                    the value of the json parameter.
+        """
+        if not endpoint:
+            raise BadRequestError('No API endpoint was specified.')
+
+        url = url_join(self._url, 'api', endpoint)
+        headers = self._get_headers()
+        if override_headers:
+            headers.update(override_headers)
+
+        if includes:
+            include_str = ','.join(includes)
+            if params and params.get('include'):
+                params['include'] += ',' + include_str
+            elif params:
+                params['include'] = include_str
+            else:
+                params = {'include': include_str}
+
+        if mode == 'GET':
+            response = self._session.get(url, params=params, headers=headers)
+        elif mode == 'POST':
+            if data_as_json:
+                response = self._session.post(url, params=params,
+                                              headers=headers, json=data)
+            else:
+                response = self._session.post(url, params=params,
+                                              headers=headers, data=data)
+        elif mode == 'PATCH':
+            response = self._session.patch(url, params=params, headers=headers,
+                                           json=data)
+        elif mode == 'DELETE':
+            response = self._session.delete(url, params=params, headers=headers)
+        elif mode == 'PUT':
+            response = self._session.put(url, params=params, headers=headers,
+                                         json=data)
+        else:
+            raise BadRequestError(
+                'Invalid request type specified(%s).  Must be one of %r.' % (
+                    mode, REQUEST_TYPES))
+
+        try:
+            response_json = response.json()
+        except ValueError:
+            response_json = {}
+
+        if response.status_code in (400, 422):
+            raise PterodactylApiError('API Request resulted in errors: %s' %
+                                      response_json.get('errors'))
+        else:
+            response.raise_for_status()
+
+        if json is True:
+            return response_json
+        elif json is False:
+            return response
+        else:
+            return response_json or response
```

### Comparing `py-dactyl-2.0.1/pydactyl/api/client/account/base.py` & `py-dactyl-2.0.2/pydactyl/api/client/account/base.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-from pydactyl.api import base
-
-
-class Account(base.PterodactylAPI):
-    """Class for interacting with the Pterodactyl Client API.
-
-    Methods in this class appear in the base **client.account** namespace
-    when using PterodactylClient.
-    """
-
-    def get_account(self):
-        """List details of the account belonging to the client API key."""
-        endpoint = 'client/account'
-        response = self._api_request(endpoint=endpoint)
-        return response
-
-    def get_2fa_setup_code(self):
-        """Generates a TOTP QR code image to allow the setup of 2FA."""
-        endpoint = 'client/account/two-factor'
-        response = self._api_request(endpoint=endpoint)
-        return response
-
-    def enable_2fa(self, code: str):
-        """Enables TOTP 2FA.
-
-        Takes a TOTP code generated by a client configured using the code
-        from get_2fa_setup_code().  This does not take the code directly and
-        you must first setup an authenticator app such as Google
-        Authenticator to generate the code provided to this method.
-
-        Args:
-            code(str): TOTP code generated by authenticator app
-        """
-        data = {'code': code}
-        endpoint = 'client/account/two-factor'
-        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
-        return response
-
-    def disable_2fa(self, password: str):
-        """Disables 2FA on the account.
-
-        Args:
-            password(str): User's account password
-        """
-        data = {'password': password}
-        endpoint = 'client/account/two-factor'
-        response = self._api_request(endpoint=endpoint, mode='DELETE',
-                                     data=data)
-        return response
-
-    def update_email(self, email: str, password: str):
-        """Updates the email address of the account.
-
-        Args:
-            email(str): New email address
-            password(str): User's account password
-        """
-        data = {'email': email, 'password': password}
-        endpoint = 'client/account/email'
-        response = self._api_request(endpoint=endpoint, mode='PUT',
-                                     data=data)
-        return response
-
-    def update_password(self, current: str, new: str, new_confirm: str):
-        """Updates the password of the account.
-
-        Args:
-            current(str): User's current password
-            new(str): New password for the account, must match new_confirm
-            new_confirm(str): New password for the account, must match new
-        """
-        data = {'current_password': current, 'password': new,
-                'password_confirmation': new_confirm}
-        endpoint = 'client/account/password'
-        response = self._api_request(endpoint=endpoint, mode='PUT',
-                                     data=data)
-        return response
-
-    def api_key_list(self):
-        """List client's API keys."""
-        endpoint = 'client/account/api-keys'
-        response = self._api_request(endpoint=endpoint)
-        return base.parse_response(response, detail=False)
-
-    def api_key_create(self, description: str, allowed_ips: list):
-        """Create a client API key.
-
-        Args:
-            description(str): Note for the API key
-            allowed_ips(iter): List of allowed IPs
-        """
-        endpoint = 'client/account/api-keys'
-        data = {'description': description, 'allowed_ips': allowed_ips}
-        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
-        return response
-
-    def api_key_delete(self, identifier):
-        """Delete a client API key.
-
-        Args:
-            identifier(str): API key identifier
-        """
-        endpoint = 'client/account/api-keys/{}'.format(identifier)
-        response = self._api_request(endpoint=endpoint, mode='DELETE')
-        return response
+from pydactyl.api import base
+
+
+class Account(base.PterodactylAPI):
+    """Class for interacting with the Pterodactyl Client API.
+
+    Methods in this class appear in the base **client.account** namespace
+    when using PterodactylClient.
+    """
+
+    def get_account(self):
+        """List details of the account belonging to the client API key."""
+        endpoint = 'client/account'
+        response = self._api_request(endpoint=endpoint)
+        return response
+
+    def get_2fa_setup_code(self):
+        """Generates a TOTP QR code image to allow the setup of 2FA."""
+        endpoint = 'client/account/two-factor'
+        response = self._api_request(endpoint=endpoint)
+        return response
+
+    def enable_2fa(self, code: str):
+        """Enables TOTP 2FA.
+
+        Takes a TOTP code generated by a client configured using the code
+        from get_2fa_setup_code().  This does not take the code directly and
+        you must first setup an authenticator app such as Google
+        Authenticator to generate the code provided to this method.
+
+        Args:
+            code(str): TOTP code generated by authenticator app
+        """
+        data = {'code': code}
+        endpoint = 'client/account/two-factor'
+        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
+        return response
+
+    def disable_2fa(self, password: str):
+        """Disables 2FA on the account.
+
+        Args:
+            password(str): User's account password
+        """
+        data = {'password': password}
+        endpoint = 'client/account/two-factor'
+        response = self._api_request(endpoint=endpoint, mode='DELETE',
+                                     data=data)
+        return response
+
+    def update_email(self, email: str, password: str):
+        """Updates the email address of the account.
+
+        Args:
+            email(str): New email address
+            password(str): User's account password
+        """
+        data = {'email': email, 'password': password}
+        endpoint = 'client/account/email'
+        response = self._api_request(endpoint=endpoint, mode='PUT',
+                                     data=data)
+        return response
+
+    def update_password(self, current: str, new: str, new_confirm: str):
+        """Updates the password of the account.
+
+        Args:
+            current(str): User's current password
+            new(str): New password for the account, must match new_confirm
+            new_confirm(str): New password for the account, must match new
+        """
+        data = {'current_password': current, 'password': new,
+                'password_confirmation': new_confirm}
+        endpoint = 'client/account/password'
+        response = self._api_request(endpoint=endpoint, mode='PUT',
+                                     data=data)
+        return response
+
+    def api_key_list(self):
+        """List client's API keys."""
+        endpoint = 'client/account/api-keys'
+        response = self._api_request(endpoint=endpoint)
+        return base.parse_response(response, detail=False)
+
+    def api_key_create(self, description: str, allowed_ips: list):
+        """Create a client API key.
+
+        Args:
+            description(str): Note for the API key
+            allowed_ips(iter): List of allowed IPs
+        """
+        endpoint = 'client/account/api-keys'
+        data = {'description': description, 'allowed_ips': allowed_ips}
+        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
+        return response
+
+    def api_key_delete(self, identifier):
+        """Delete a client API key.
+
+        Args:
+            identifier(str): API key identifier
+        """
+        endpoint = 'client/account/api-keys/{}'.format(identifier)
+        response = self._api_request(endpoint=endpoint, mode='DELETE')
+        return response
```

### Comparing `py-dactyl-2.0.1/pydactyl/api/client/client_api.py` & `py-dactyl-2.0.2/pydactyl/api/client/client_api.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-# Client Account APIs
-from pydactyl.api.client.account.base import Account
-
-# Client Server APIs
-from pydactyl.api.client.servers.backups import Backups
-from pydactyl.api.client.servers.base import ServersBase
-from pydactyl.api.client.servers.databases import Databases
-from pydactyl.api.client.servers.files import Files
-from pydactyl.api.client.servers.network import Network
-from pydactyl.api.client.servers.schedules import Schedules
-from pydactyl.api.client.servers.settings import Settings
-from pydactyl.api.client.servers.startup import Startup
-from pydactyl.api.client.servers.users import Users
-
-from pydactyl.api.base import PterodactylAPI
-
-
-class ClientAPI(PterodactylAPI):
-    """Provides a simplified interface to the Pterodactyl Panel API.
-
-    This class is only used by PterodactylClient.  It provides an interface
-    for the Client API endpoints.
-    """
-
-    def __init__(self, *args, **kwargs):
-        """Initialize a Pterodactyl class instance."""
-        self._account = None
-        self._servers = None
-        super().__init__(*args, **kwargs)
-
-    @property
-    def account(self):
-        self._account = Account(self._url, self._api_key)
-        return self._account
-
-    @property
-    def servers(self):
-        self._servers = ClientServersAPI(self._url, self._api_key)
-        return self._servers
-
-
-class ClientServersAPI(ServersBase, ClientAPI):
-    """Provides a simplified interface to the Pterodactyl Panel API.
-
-    This class is only used by PterodactylClient.  It provides an interface
-    for the Client API endpoints.
-    """
-
-    def __init__(self, *args, **kwargs):
-        """Initialize a Pterodactyl class instance."""
-        self._backups = None
-        self._databases = None
-        self._files = None
-        self._network = None
-        self._schedules = None
-        self._settings = None
-        self._startup = None
-        self._users = None
-        super().__init__(*args, **kwargs)
-
-    @property
-    def backups(self):
-        self._backups = Backups(self._url, self._api_key)
-        return self._backups
-
-    @property
-    def databases(self):
-        self._databases = Databases(self._url, self._api_key)
-        return self._databases
-
-    @property
-    def files(self):
-        self._files = Files(self._url, self._api_key)
-        return self._files
-
-    @property
-    def network(self):
-        self._network = Network(self._url, self._api_key)
-        return self._network
-
-    @property
-    def schedules(self):
-        self._schedules = Schedules(self._url, self._api_key)
-        return self._schedules
-
-    @property
-    def settings(self):
-        self._settings = Settings(self._url, self._api_key)
-        return self._settings
-
-    @property
-    def startup(self):
-        self._startup = Startup(self._url, self._api_key)
-        return self._startup
-
-    @property
-    def users(self):
-        self._users = Users(self._url, self._api_key)
-        return self._users
+# Client Account APIs
+from pydactyl.api.client.account.base import Account
+
+# Client Server APIs
+from pydactyl.api.client.servers.backups import Backups
+from pydactyl.api.client.servers.base import ServersBase
+from pydactyl.api.client.servers.databases import Databases
+from pydactyl.api.client.servers.files import Files
+from pydactyl.api.client.servers.network import Network
+from pydactyl.api.client.servers.schedules import Schedules
+from pydactyl.api.client.servers.settings import Settings
+from pydactyl.api.client.servers.startup import Startup
+from pydactyl.api.client.servers.users import Users
+
+from pydactyl.api.base import PterodactylAPI
+
+
+class ClientAPI(PterodactylAPI):
+    """Provides a simplified interface to the Pterodactyl Panel API.
+
+    This class is only used by PterodactylClient.  It provides an interface
+    for the Client API endpoints.
+    """
+
+    def __init__(self, *args, **kwargs):
+        """Initialize a Pterodactyl class instance."""
+        self._account = None
+        self._servers = None
+        super().__init__(*args, **kwargs)
+
+    @property
+    def account(self):
+        self._account = Account(self._url, self._api_key)
+        return self._account
+
+    @property
+    def servers(self):
+        self._servers = ClientServersAPI(self._url, self._api_key)
+        return self._servers
+
+
+class ClientServersAPI(ServersBase, ClientAPI):
+    """Provides a simplified interface to the Pterodactyl Panel API.
+
+    This class is only used by PterodactylClient.  It provides an interface
+    for the Client API endpoints.
+    """
+
+    def __init__(self, *args, **kwargs):
+        """Initialize a Pterodactyl class instance."""
+        self._backups = None
+        self._databases = None
+        self._files = None
+        self._network = None
+        self._schedules = None
+        self._settings = None
+        self._startup = None
+        self._users = None
+        super().__init__(*args, **kwargs)
+
+    @property
+    def backups(self):
+        self._backups = Backups(self._url, self._api_key)
+        return self._backups
+
+    @property
+    def databases(self):
+        self._databases = Databases(self._url, self._api_key)
+        return self._databases
+
+    @property
+    def files(self):
+        self._files = Files(self._url, self._api_key)
+        return self._files
+
+    @property
+    def network(self):
+        self._network = Network(self._url, self._api_key)
+        return self._network
+
+    @property
+    def schedules(self):
+        self._schedules = Schedules(self._url, self._api_key)
+        return self._schedules
+
+    @property
+    def settings(self):
+        self._settings = Settings(self._url, self._api_key)
+        return self._settings
+
+    @property
+    def startup(self):
+        self._startup = Startup(self._url, self._api_key)
+        return self._startup
+
+    @property
+    def users(self):
+        self._users = Users(self._url, self._api_key)
+        return self._users
```

### Comparing `py-dactyl-2.0.1/pydactyl/api/client/servers/backups.py` & `py-dactyl-2.0.2/pydactyl/api/client/servers/backups.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-from pydactyl.api import base
-
-
-class Backups(base.PterodactylAPI):
-    """Pterodactyl Client Server Backups API."""
-
-    def list_backups(self, server_id: str):
-        """List files belonging to specified server.
-
-        Optionally specify a directory and only return results in the
-        specified directory.  Directory is relative to the server's root.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-        """
-        endpoint = 'client/servers/{}/backups'.format(server_id)
-        response = self._api_request(endpoint=endpoint)
-        return response
-
-    def create_backup(self, server_id: str):
-        """Create a new backup of the specified server.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-        """
-        endpoint = 'client/servers/{}/backups'.format(server_id)
-        response = self._api_request(endpoint=endpoint, mode='POST')
-        return response
-
-    def get_backup_detail(self, server_id: str, backup_id: str):
-        """Retrieves information about the specified backup.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            backup_id(str): Backup identifier (long UUID)
-        """
-        endpoint = 'client/servers/{}/backups/{}'.format(server_id, backup_id)
-        response = self._api_request(endpoint=endpoint)
-        return response
-
-    def get_backup_download(self, server_id: str, backup_id: str):
-        """Generates a download link for the specified backup.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            backup_id(str): Backup identifier (long UUID)
-        """
-        endpoint = 'client/servers/{}/backups/{}/download'.format(server_id,
-                                                                  backup_id)
-        response = self._api_request(endpoint=endpoint)
-        return response
-
-    def delete_backup(self, server_id: str, backup_id: str):
-        """Deletes the specified backup.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            backup_id(str): Backup identifier (long UUID)
-        """
-        endpoint = 'client/servers/{}/backups/{}'.format(server_id, backup_id)
-        response = self._api_request(endpoint=endpoint, mode='DELETE')
-        return response
+from pydactyl.api import base
+
+
+class Backups(base.PterodactylAPI):
+    """Pterodactyl Client Server Backups API."""
+
+    def list_backups(self, server_id: str):
+        """List files belonging to specified server.
+
+        Optionally specify a directory and only return results in the
+        specified directory.  Directory is relative to the server's root.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+        """
+        endpoint = 'client/servers/{}/backups'.format(server_id)
+        response = self._api_request(endpoint=endpoint)
+        return response
+
+    def create_backup(self, server_id: str):
+        """Create a new backup of the specified server.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+        """
+        endpoint = 'client/servers/{}/backups'.format(server_id)
+        response = self._api_request(endpoint=endpoint, mode='POST')
+        return response
+
+    def get_backup_detail(self, server_id: str, backup_id: str):
+        """Retrieves information about the specified backup.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            backup_id(str): Backup identifier (long UUID)
+        """
+        endpoint = 'client/servers/{}/backups/{}'.format(server_id, backup_id)
+        response = self._api_request(endpoint=endpoint)
+        return response
+
+    def get_backup_download(self, server_id: str, backup_id: str):
+        """Generates a download link for the specified backup.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            backup_id(str): Backup identifier (long UUID)
+        """
+        endpoint = 'client/servers/{}/backups/{}/download'.format(server_id,
+                                                                  backup_id)
+        response = self._api_request(endpoint=endpoint)
+        return response
+
+    def delete_backup(self, server_id: str, backup_id: str):
+        """Deletes the specified backup.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            backup_id(str): Backup identifier (long UUID)
+        """
+        endpoint = 'client/servers/{}/backups/{}'.format(server_id, backup_id)
+        response = self._api_request(endpoint=endpoint, mode='DELETE')
+        return response
```

### Comparing `py-dactyl-2.0.1/pydactyl/api/client/servers/databases.py` & `py-dactyl-2.0.2/pydactyl/api/client/servers/databases.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from pydactyl.api import base
-
-
-class Databases(base.PterodactylAPI):
-    """Pterodactyl Client Server Databases API."""
-
-    def list_databases(self, server_id: str, include_passwords: bool = False,
-                       includes: list = [], params: dict = None):
-        """List all databases for a server.
-
-        Optionally includes the database user passwords.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            include_passwords(bool): True to include database user passwords
-            includes(iter): List of includes, e.g. ('password')
-            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
-        """
-        if include_passwords:
-            includes.append('password')
-        endpoint = 'client/servers/{}/databases'.format(server_id)
-        response = self._api_request(endpoint=endpoint,
-                                     includes=includes or None, params=params)
-        return response
-
-    def create_database(self, server_id: str, name: str, remote: str = '%'):
-        """Create a new database for the specified server.
-
-        Limits connections to the address specified in remote, defaulting to
-        allowing from all.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            remote(str): Remote address to allow connections from (e.g. 1.2.3.4)
-        """
-        data = {'database': name, 'remote': remote}
-        endpoint = 'client/servers/{}/databases'.format(server_id)
-        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
-        return response
-
-    def rotate_database_password(self, server_id: str, database_id: str):
-        """Changes the password of the specified database.
-
-        Generates a new password and returns it in the response.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            database_id(str): Database identifier (long UUID)
-        """
-        endpoint = 'client/servers/{}/databases/{}/rotate-password'.format(
-            server_id, database_id)
-        response = self._api_request(endpoint=endpoint, mode='POST')
-        return response
-
-    def delete_database(self, server_id: str, database_id: str):
-        """Deletes the specified database.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            database_id(str): Database identifier (long UUID)
-        """
-        endpoint = 'client/servers/{}/databases/{}'.format(server_id,
-                                                           database_id)
-        response = self._api_request(endpoint=endpoint, mode='DELETE')
-        return response
+from pydactyl.api import base
+
+
+class Databases(base.PterodactylAPI):
+    """Pterodactyl Client Server Databases API."""
+
+    def list_databases(self, server_id: str, include_passwords: bool = False,
+                       includes: list = [], params: dict = None):
+        """List all databases for a server.
+
+        Optionally includes the database user passwords.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            include_passwords(bool): True to include database user passwords
+            includes(iter): List of includes, e.g. ('password')
+            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
+        """
+        if include_passwords:
+            includes.append('password')
+        endpoint = 'client/servers/{}/databases'.format(server_id)
+        response = self._api_request(endpoint=endpoint,
+                                     includes=includes or None, params=params)
+        return response
+
+    def create_database(self, server_id: str, name: str, remote: str = '%'):
+        """Create a new database for the specified server.
+
+        Limits connections to the address specified in remote, defaulting to
+        allowing from all.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            remote(str): Remote address to allow connections from (e.g. 1.2.3.4)
+        """
+        data = {'database': name, 'remote': remote}
+        endpoint = 'client/servers/{}/databases'.format(server_id)
+        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
+        return response
+
+    def rotate_database_password(self, server_id: str, database_id: str):
+        """Changes the password of the specified database.
+
+        Generates a new password and returns it in the response.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            database_id(str): Database identifier (long UUID)
+        """
+        endpoint = 'client/servers/{}/databases/{}/rotate-password'.format(
+            server_id, database_id)
+        response = self._api_request(endpoint=endpoint, mode='POST')
+        return response
+
+    def delete_database(self, server_id: str, database_id: str):
+        """Deletes the specified database.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            database_id(str): Database identifier (long UUID)
+        """
+        endpoint = 'client/servers/{}/databases/{}'.format(server_id,
+                                                           database_id)
+        response = self._api_request(endpoint=endpoint, mode='DELETE')
+        return response
```

### Comparing `py-dactyl-2.0.1/pydactyl/api/client/servers/files.py` & `py-dactyl-2.0.2/pydactyl/api/client/servers/files.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,169 +1,169 @@
-from pydactyl.api import base
-
-
-class Files(base.PterodactylAPI):
-    """Class for interacting with the Pterodactyl Client API."""
-
-    def list_files(self, server_id: str, path: str = None):
-        """List files belonging to specified server.
-
-        Optionally specify a directory and only return results in the
-        specified directory.  Directory is relative to the server's root.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            path(str): Path to list in (e.g. 'save_game')
-        """
-        params = {}
-        endpoint = 'client/servers/{}/files/list'.format(server_id)
-        if path is not None:
-            params = {'directory': path}
-        response = self._api_request(endpoint=endpoint, params=params)
-        return response
-
-    def download_file(self, server_id: str, path: str) -> str:
-        """Get a download link for the specified file on the specified server.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            path(str): URL encoded path to desired file (e.g. 'eula.txt')
-
-        Returns:
-            response(str): Signed URL to download file
-        """
-        endpoint = 'client/servers/{}/files/download'.format(server_id)
-        params = {'file': path}
-        response = self._api_request(endpoint=endpoint, params=params)
-        return response.get('attributes').get('url')
-
-    def get_file_contents(self, server_id: str, path: str) -> str:
-        """Get contents of the specified file on the specified server.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            path(str): URL encoded path to desired file (e.g. 'eula.txt')
-        """
-        endpoint = 'client/servers/{}/files/contents'.format(server_id)
-        params = {'file': path}
-        response = self._api_request(endpoint=endpoint, params=params)
-        return response
-
-    def rename_file(self, server_id: str, old_name: str, new_name: str,
-                    root: str = '/'):
-        """Rename a file.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            old_name(str): Name of existing file to rename
-            new_name(str): New filename
-            root(str): Path to files, relative to server root
-        """
-        endpoint = 'client/servers/{}/files/rename'.format(server_id)
-        data = {'root': root, 'files': [{'from': old_name, 'to': new_name}]}
-        response = self._api_request(endpoint=endpoint, mode='PUT', data=data)
-        return response
-
-    def copy_file(self, server_id: str, path: str):
-        """Makes a copy of a file.
-
-        This is primarily used by the file manager.
-
-        Makes a copy of the file with a unique name.  You cannot specify the
-        new name of the file, it just picks one for you.  For example
-        'test.txt' will have a copy created named 'test copy.txt'.  Running
-        it again will create 'test copy 1.txt'.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            path(str): URL encoded path to desired file (e.g. 'eula.txt')
-        """
-        endpoint = 'client/servers/{}/files/copy'.format(server_id)
-        data = {'location': path}
-        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
-        return response
-
-    def write_file(self, server_id: str, path: str, contents: str):
-        """Writes contents to a file.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            path(str): Path to desired file (e.g. 'eula.txt')
-            contents(str): Contents to write to the file.
-        """
-        params = {'file': path}
-        endpoint = 'client/servers/{}/files/write'.format(server_id)
-        response = self._api_request(
-            endpoint=endpoint, mode='POST', params=params, data=contents,
-            override_headers={'Content-Type': 'application/text'},
-            data_as_json=False)
-        return response
-
-    def compress_files(self, server_id: str, files: iter, path: str = '/'):
-        """Creates a compressed archive.
-
-        Creates a tar.gz compressed file containing the listed files.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            files(iter): List of files to add to the archive
-            path(str): Root path to create the archive from
-        """
-        data = {'root': path, 'files': files}
-        endpoint = 'client/servers/{}/files/compress'.format(server_id)
-        response = self._api_request(endpoint=endpoint, mode='POST',
-                                     data=data)
-        return response
-
-    def decompress_file(self, server_id: str, file: str, path: str = '/'):
-        """Decompresses an archive.
-
-        Decompresses a compressed file to the specified path.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            file(str): Name of the archive file to decompress
-            path(str): Root path to decompress in
-        """
-        data = {'root': path, 'file': file}
-        endpoint = 'client/servers/{}/files/decompress'.format(server_id)
-        response = self._api_request(endpoint=endpoint, mode='POST',
-                                     data=data)
-        return response
-
-    def delete_files(self, server_id: str, files: iter, path: str = '/'):
-        """Deletes the specified file(s) or directory(s).
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            files(iter): List of files to delete
-            path(str): Root path look for files in
-        """
-        data = {'root': path, 'files': files}
-        endpoint = 'client/servers/{}/files/delete'.format(server_id)
-        response = self._api_request(endpoint=endpoint, mode='POST',
-                                     data=data)
-        return response
-
-    def create_folder(self, server_id: str, name: str, path: str = '/'):
-        """Creates the specified folder in the specified directory.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            name(str): Name of the directory to create
-            path(str): Root path to create the directory in
-        """
-        data = {'root': path, 'name': name}
-        endpoint = 'client/servers/{}/files/create-folder'.format(server_id)
-        response = self._api_request(endpoint=endpoint, mode='POST',
-                                     data=data)
-        return response
-
-    def get_upload_file_url(self, server_id: str) -> str:
-        """Returns a signed URL used to upload files to the server using POST.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-        """
-        endpoint = 'client/servers/{}/files/upload'.format(server_id)
-        response = self._api_request(endpoint=endpoint)
-        return response.get('attributes').get('url')
+from pydactyl.api import base
+
+
+class Files(base.PterodactylAPI):
+    """Class for interacting with the Pterodactyl Client API."""
+
+    def list_files(self, server_id: str, path: str = None):
+        """List files belonging to specified server.
+
+        Optionally specify a directory and only return results in the
+        specified directory.  Directory is relative to the server's root.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            path(str): Path to list in (e.g. 'save_game')
+        """
+        params = {}
+        endpoint = 'client/servers/{}/files/list'.format(server_id)
+        if path is not None:
+            params = {'directory': path}
+        response = self._api_request(endpoint=endpoint, params=params)
+        return response
+
+    def download_file(self, server_id: str, path: str) -> str:
+        """Get a download link for the specified file on the specified server.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            path(str): URL encoded path to desired file (e.g. 'eula.txt')
+
+        Returns:
+            response(str): Signed URL to download file
+        """
+        endpoint = 'client/servers/{}/files/download'.format(server_id)
+        params = {'file': path}
+        response = self._api_request(endpoint=endpoint, params=params)
+        return response.get('attributes').get('url')
+
+    def get_file_contents(self, server_id: str, path: str) -> str:
+        """Get contents of the specified file on the specified server.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            path(str): URL encoded path to desired file (e.g. 'eula.txt')
+        """
+        endpoint = 'client/servers/{}/files/contents'.format(server_id)
+        params = {'file': path}
+        response = self._api_request(endpoint=endpoint, params=params)
+        return response
+
+    def rename_file(self, server_id: str, old_name: str, new_name: str,
+                    root: str = '/'):
+        """Rename a file.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            old_name(str): Name of existing file to rename
+            new_name(str): New filename
+            root(str): Path to files, relative to server root
+        """
+        endpoint = 'client/servers/{}/files/rename'.format(server_id)
+        data = {'root': root, 'files': [{'from': old_name, 'to': new_name}]}
+        response = self._api_request(endpoint=endpoint, mode='PUT', data=data)
+        return response
+
+    def copy_file(self, server_id: str, path: str):
+        """Makes a copy of a file.
+
+        This is primarily used by the file manager.
+
+        Makes a copy of the file with a unique name.  You cannot specify the
+        new name of the file, it just picks one for you.  For example
+        'test.txt' will have a copy created named 'test copy.txt'.  Running
+        it again will create 'test copy 1.txt'.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            path(str): URL encoded path to desired file (e.g. 'eula.txt')
+        """
+        endpoint = 'client/servers/{}/files/copy'.format(server_id)
+        data = {'location': path}
+        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
+        return response
+
+    def write_file(self, server_id: str, path: str, contents: str):
+        """Writes contents to a file.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            path(str): Path to desired file (e.g. 'eula.txt')
+            contents(str): Contents to write to the file.
+        """
+        params = {'file': path}
+        endpoint = 'client/servers/{}/files/write'.format(server_id)
+        response = self._api_request(
+            endpoint=endpoint, mode='POST', params=params, data=contents,
+            override_headers={'Content-Type': 'application/text'},
+            data_as_json=False)
+        return response
+
+    def compress_files(self, server_id: str, files: iter, path: str = '/'):
+        """Creates a compressed archive.
+
+        Creates a tar.gz compressed file containing the listed files.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            files(iter): List of files to add to the archive
+            path(str): Root path to create the archive from
+        """
+        data = {'root': path, 'files': files}
+        endpoint = 'client/servers/{}/files/compress'.format(server_id)
+        response = self._api_request(endpoint=endpoint, mode='POST',
+                                     data=data)
+        return response
+
+    def decompress_file(self, server_id: str, file: str, path: str = '/'):
+        """Decompresses an archive.
+
+        Decompresses a compressed file to the specified path.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            file(str): Name of the archive file to decompress
+            path(str): Root path to decompress in
+        """
+        data = {'root': path, 'file': file}
+        endpoint = 'client/servers/{}/files/decompress'.format(server_id)
+        response = self._api_request(endpoint=endpoint, mode='POST',
+                                     data=data)
+        return response
+
+    def delete_files(self, server_id: str, files: iter, path: str = '/'):
+        """Deletes the specified file(s) or directory(s).
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            files(iter): List of files to delete
+            path(str): Root path look for files in
+        """
+        data = {'root': path, 'files': files}
+        endpoint = 'client/servers/{}/files/delete'.format(server_id)
+        response = self._api_request(endpoint=endpoint, mode='POST',
+                                     data=data)
+        return response
+
+    def create_folder(self, server_id: str, name: str, path: str = '/'):
+        """Creates the specified folder in the specified directory.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            name(str): Name of the directory to create
+            path(str): Root path to create the directory in
+        """
+        data = {'root': path, 'name': name}
+        endpoint = 'client/servers/{}/files/create-folder'.format(server_id)
+        response = self._api_request(endpoint=endpoint, mode='POST',
+                                     data=data)
+        return response
+
+    def get_upload_file_url(self, server_id: str) -> str:
+        """Returns a signed URL used to upload files to the server using POST.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+        """
+        endpoint = 'client/servers/{}/files/upload'.format(server_id)
+        response = self._api_request(endpoint=endpoint)
+        return response.get('attributes').get('url')
```

### Comparing `py-dactyl-2.0.1/pydactyl/api/client/servers/network.py` & `py-dactyl-2.0.2/pydactyl/api/client/servers/network.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-from pydactyl.api import base
-
-
-class Network(base.PterodactylAPI):
-    """Pterodactyl Client Server Network API."""
-
-    def list_allocations(self, server_id: str):
-        """Retrieves network information for the specified server.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-        """
-        endpoint = 'client/servers/{}/network/allocations'.format(server_id)
-        response = self._api_request(endpoint=endpoint)
-        return response
-
-    def assign_allocation(self, server_id: str):
-        """Assigns an allocation to the server.
-
-        Automatically assigns a new allocation if auto-assign is enabled on
-        the instance.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-        """
-        endpoint = 'client/servers/{}/network/allocations'.format(server_id)
-        response = self._api_request(endpoint=endpoint, mode='POST')
-        return response
-
-    def set_allocation_note(self, server_id: str, allocation_id: int,
-                            note: str):
-        """Sets the note on an allocation.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            allocation_id(int): Allocation identifier (e.g. 2)
-            note(str): Contents of the note
-        """
-        data = {'notes': note}
-        endpoint = 'client/servers/{}/network/allocations/{}'.format(
-            server_id, allocation_id)
-        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
-        return response
-
-    def set_primary_allocation(self, server_id: str, allocation_id: int):
-        """Sets the specified allocation as the primary allocation.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            allocation_id(int): Allocation identifier (e.g. 2)
-        """
-        endpoint = 'client/servers/{}/network/allocations/{}/primary'.format(
-            server_id, allocation_id)
-        response = self._api_request(endpoint=endpoint, mode='POST')
-        return response
-
-    def unassign_allocation(self, server_id: str, allocation_id: int):
-        """Deletes the specified non-primary allocation.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            allocation_id(int): Allocation identifier (e.g. 2)
-        """
-        endpoint = 'client/servers/{}/network/allocations/{}'.format(
-            server_id, allocation_id)
-        response = self._api_request(endpoint=endpoint, mode='DELETE')
-        return response
+from pydactyl.api import base
+
+
+class Network(base.PterodactylAPI):
+    """Pterodactyl Client Server Network API."""
+
+    def list_allocations(self, server_id: str):
+        """Retrieves network information for the specified server.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+        """
+        endpoint = 'client/servers/{}/network/allocations'.format(server_id)
+        response = self._api_request(endpoint=endpoint)
+        return response
+
+    def assign_allocation(self, server_id: str):
+        """Assigns an allocation to the server.
+
+        Automatically assigns a new allocation if auto-assign is enabled on
+        the instance.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+        """
+        endpoint = 'client/servers/{}/network/allocations'.format(server_id)
+        response = self._api_request(endpoint=endpoint, mode='POST')
+        return response
+
+    def set_allocation_note(self, server_id: str, allocation_id: int,
+                            note: str):
+        """Sets the note on an allocation.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            allocation_id(int): Allocation identifier (e.g. 2)
+            note(str): Contents of the note
+        """
+        data = {'notes': note}
+        endpoint = 'client/servers/{}/network/allocations/{}'.format(
+            server_id, allocation_id)
+        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
+        return response
+
+    def set_primary_allocation(self, server_id: str, allocation_id: int):
+        """Sets the specified allocation as the primary allocation.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            allocation_id(int): Allocation identifier (e.g. 2)
+        """
+        endpoint = 'client/servers/{}/network/allocations/{}/primary'.format(
+            server_id, allocation_id)
+        response = self._api_request(endpoint=endpoint, mode='POST')
+        return response
+
+    def unassign_allocation(self, server_id: str, allocation_id: int):
+        """Deletes the specified non-primary allocation.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            allocation_id(int): Allocation identifier (e.g. 2)
+        """
+        endpoint = 'client/servers/{}/network/allocations/{}'.format(
+            server_id, allocation_id)
+        response = self._api_request(endpoint=endpoint, mode='DELETE')
+        return response
```

### Comparing `py-dactyl-2.0.1/pydactyl/api/client/servers/schedules.py` & `py-dactyl-2.0.2/pydactyl/api/client/servers/schedules.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,169 +1,169 @@
-from pydactyl.api import base
-from pydactyl.constants import SCHEDULE_ACTIONS
-from pydactyl.exceptions import BadRequestError
-
-
-def check_schedule_action_valid(action):
-    if action not in SCHEDULE_ACTIONS:
-        raise BadRequestError(
-            'Invalid schedule action sent({}), must be one of: {}'.format(
-                action, SCHEDULE_ACTIONS))
-
-
-class Schedules(base.PterodactylAPI):
-    """Pterodactyl Client Server Databases API."""
-
-    def list_schedules(self, server_id: str):
-        """List all schedules for a server.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-        """
-        endpoint = 'client/servers/{}/schedules'.format(server_id)
-        response = self._api_request(endpoint=endpoint)
-        return response
-
-    def create_schedule(self, server_id: str, name: str, minute: str,
-                        hour: str, day_of_week: str, day_of_month: str,
-                        month: str, is_active: bool = True, 
-                        only_when_online: bool = False):
-        """Creates a new schedule for the specified server.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            name(str): Friendly name for the schedule
-            minute(str): Value for Cron minute field
-            hour(str): Value for Cron hour field
-            day_of_week(str): Value for Cron day_of_week field
-            day_of_month(str): Value for Cron day_of_month field
-            month(str): Value for Cron month field
-            is_active(bool): False to create the schedule as disabled
-            only_when_online(bool): True to run schedule only when server is running
-        """
-        data = {'name': name, 'minute': minute, 'hour': hour,
-                'day_of_week': day_of_week, 'day_of_month': day_of_month,
-                'month': month, 'is_active': is_active, 
-                'only_when_online': only_when_online}
-        endpoint = 'client/servers/{}/schedules'.format(server_id)
-        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
-        return response
-
-    def get_schedule_details(self, server_id: str, schedule_id: int):
-        """Retrieves the specified schedule.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            schedule_id(int): Schedule identifier (e.g. 2)
-        """
-        endpoint = 'client/servers/{}/schedules/{}'.format(server_id,
-                                                           schedule_id)
-        response = self._api_request(endpoint=endpoint)
-        return response
-
-    def update_schedule(self, server_id: str, schedule_id: int, name: str,
-                        minute: str, hour: str, day_of_week: str,
-                        day_of_month: str, month: str, is_active: bool = True, 
-                        only_when_online: bool = False):
-        """Updates the specified schedule.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            schedule_id(int): Schedule identifier (e.g. 2)
-
-            name(str): Friendly name for the schedule
-            minute(str): Value for Cron minute field
-            hour(str): Value for Cron hour field
-            day_of_week(str): Value for Cron day_of_week field
-            day_of_month(str): Value for Cron day_of_month field
-            month(str): Value for Cron month field
-            is_active(bool): False to create the schedule as disabled
-            only_when_online(bool): True to run schedule only when server is running
-        """
-        data = {'name': name, 'minute': minute, 'hour': hour,
-                'day_of_week': day_of_week, 'day_of_month': day_of_month,
-                'month': month, 'is_active': is_active, 
-                'only_when_online': only_when_online}
-        endpoint = 'client/servers/{}/schedules/{}'.format(server_id,
-                                                           schedule_id)
-        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
-        return response
-
-    def delete_schedule(self, server_id: str, schedule_id: int):
-        """Deletes the specified schedule.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            schedule_id(int): Schedule identifier (e.g. 2)
-        """
-        endpoint = 'client/servers/{}/schedules/{}'.format(server_id,
-                                                           schedule_id)
-        response = self._api_request(endpoint=endpoint, mode='DELETE')
-        return response
-
-    def create_task(self, server_id: str, schedule_id: int, action: str,
-                    payload: str, time_offset: str = '0', 
-                    continue_on_failure: bool = False):
-        """Creates a new task on the specified schedule.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            schedule_id(int): Schedule identifier (e.g. 2)
-            action(str): Type of action to use
-            payload(str): Payload to send for the action
-            time_offset(str): Offset in seconds
-            continue_on_failure(bool): True to continue schedule run if this task fails
-        """
-        check_schedule_action_valid(action)
-        data = {'action': action, 'payload': payload,
-                'time_offset': time_offset, 'continue_on_failure': continue_on_failure}
-        endpoint = 'client/servers/{}/schedules/{}/tasks'.format(server_id,
-                                                                 schedule_id)
-        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
-        return response
-
-    def update_task(self, server_id: str, schedule_id: int, task_id: int,
-                    action: str, payload: str, time_offset: str = '0', 
-                    continue_on_failure: bool = False):
-        """Updates the specified task.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            schedule_id(int): Schedule identifier (e.g. 2)
-            task_id(int): Task identifier (e.g. 4)
-            action(str): Type of action to use
-            payload(str): Payload to send for the action
-            time_offset(str): Offset in seconds
-            continue_on_failure(bool): True to continue schedule run if this task fails
-        """
-        check_schedule_action_valid(action)
-        data = {'action': action, 'payload': payload,
-                'time_offset': time_offset, 'continue_on_failure': continue_on_failure}
-        endpoint = 'client/servers/{}/schedules/{}/tasks/{}'.format(
-            server_id, schedule_id, task_id)
-        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
-        return response
-
-    def delete_task(self, server_id: str, schedule_id: int, task_id: int):
-        """Deletes the specified task.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            schedule_id(int): Schedule identifier (e.g. 2)
-            task_id(int): Task identifier (e.g. 4)
-        """
-        endpoint = 'client/servers/{}/schedules/{}/tasks/{}'.format(
-            server_id, schedule_id, task_id)
-        response = self._api_request(endpoint=endpoint, mode='DELETE')
-        return response
-
-    def run_schedule(self, server_id: str, schedule_id: int):
-        """Runs the specified schedule.
-        
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            schedule_id(int): Schedule identifier
-        """
-        endpoint = 'client/servers/{}/schedules/{}/execute'.format(
-            server_id, schedule_id)
-        response = self._api_request(endpoint=endpoint, mode='POST')
-        return response
+from pydactyl.api import base
+from pydactyl.constants import SCHEDULE_ACTIONS
+from pydactyl.exceptions import BadRequestError
+
+
+def check_schedule_action_valid(action):
+    if action not in SCHEDULE_ACTIONS:
+        raise BadRequestError(
+            'Invalid schedule action sent({}), must be one of: {}'.format(
+                action, SCHEDULE_ACTIONS))
+
+
+class Schedules(base.PterodactylAPI):
+    """Pterodactyl Client Server Databases API."""
+
+    def list_schedules(self, server_id: str):
+        """List all schedules for a server.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+        """
+        endpoint = 'client/servers/{}/schedules'.format(server_id)
+        response = self._api_request(endpoint=endpoint)
+        return response
+
+    def create_schedule(self, server_id: str, name: str, minute: str,
+                        hour: str, day_of_week: str, day_of_month: str,
+                        month: str, is_active: bool = True, 
+                        only_when_online: bool = False):
+        """Creates a new schedule for the specified server.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            name(str): Friendly name for the schedule
+            minute(str): Value for Cron minute field
+            hour(str): Value for Cron hour field
+            day_of_week(str): Value for Cron day_of_week field
+            day_of_month(str): Value for Cron day_of_month field
+            month(str): Value for Cron month field
+            is_active(bool): False to create the schedule as disabled
+            only_when_online(bool): True to run schedule only when server is running
+        """
+        data = {'name': name, 'minute': minute, 'hour': hour,
+                'day_of_week': day_of_week, 'day_of_month': day_of_month,
+                'month': month, 'is_active': is_active, 
+                'only_when_online': only_when_online}
+        endpoint = 'client/servers/{}/schedules'.format(server_id)
+        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
+        return response
+
+    def get_schedule_details(self, server_id: str, schedule_id: int):
+        """Retrieves the specified schedule.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            schedule_id(int): Schedule identifier (e.g. 2)
+        """
+        endpoint = 'client/servers/{}/schedules/{}'.format(server_id,
+                                                           schedule_id)
+        response = self._api_request(endpoint=endpoint)
+        return response
+
+    def update_schedule(self, server_id: str, schedule_id: int, name: str,
+                        minute: str, hour: str, day_of_week: str,
+                        day_of_month: str, month: str, is_active: bool = True, 
+                        only_when_online: bool = False):
+        """Updates the specified schedule.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            schedule_id(int): Schedule identifier (e.g. 2)
+
+            name(str): Friendly name for the schedule
+            minute(str): Value for Cron minute field
+            hour(str): Value for Cron hour field
+            day_of_week(str): Value for Cron day_of_week field
+            day_of_month(str): Value for Cron day_of_month field
+            month(str): Value for Cron month field
+            is_active(bool): False to create the schedule as disabled
+            only_when_online(bool): True to run schedule only when server is running
+        """
+        data = {'name': name, 'minute': minute, 'hour': hour,
+                'day_of_week': day_of_week, 'day_of_month': day_of_month,
+                'month': month, 'is_active': is_active, 
+                'only_when_online': only_when_online}
+        endpoint = 'client/servers/{}/schedules/{}'.format(server_id,
+                                                           schedule_id)
+        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
+        return response
+
+    def delete_schedule(self, server_id: str, schedule_id: int):
+        """Deletes the specified schedule.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            schedule_id(int): Schedule identifier (e.g. 2)
+        """
+        endpoint = 'client/servers/{}/schedules/{}'.format(server_id,
+                                                           schedule_id)
+        response = self._api_request(endpoint=endpoint, mode='DELETE')
+        return response
+
+    def create_task(self, server_id: str, schedule_id: int, action: str,
+                    payload: str, time_offset: str = '0', 
+                    continue_on_failure: bool = False):
+        """Creates a new task on the specified schedule.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            schedule_id(int): Schedule identifier (e.g. 2)
+            action(str): Type of action to use
+            payload(str): Payload to send for the action
+            time_offset(str): Offset in seconds
+            continue_on_failure(bool): True to continue schedule run if this task fails
+        """
+        check_schedule_action_valid(action)
+        data = {'action': action, 'payload': payload,
+                'time_offset': time_offset, 'continue_on_failure': continue_on_failure}
+        endpoint = 'client/servers/{}/schedules/{}/tasks'.format(server_id,
+                                                                 schedule_id)
+        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
+        return response
+
+    def update_task(self, server_id: str, schedule_id: int, task_id: int,
+                    action: str, payload: str, time_offset: str = '0', 
+                    continue_on_failure: bool = False):
+        """Updates the specified task.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            schedule_id(int): Schedule identifier (e.g. 2)
+            task_id(int): Task identifier (e.g. 4)
+            action(str): Type of action to use
+            payload(str): Payload to send for the action
+            time_offset(str): Offset in seconds
+            continue_on_failure(bool): True to continue schedule run if this task fails
+        """
+        check_schedule_action_valid(action)
+        data = {'action': action, 'payload': payload,
+                'time_offset': time_offset, 'continue_on_failure': continue_on_failure}
+        endpoint = 'client/servers/{}/schedules/{}/tasks/{}'.format(
+            server_id, schedule_id, task_id)
+        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
+        return response
+
+    def delete_task(self, server_id: str, schedule_id: int, task_id: int):
+        """Deletes the specified task.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            schedule_id(int): Schedule identifier (e.g. 2)
+            task_id(int): Task identifier (e.g. 4)
+        """
+        endpoint = 'client/servers/{}/schedules/{}/tasks/{}'.format(
+            server_id, schedule_id, task_id)
+        response = self._api_request(endpoint=endpoint, mode='DELETE')
+        return response
+
+    def run_schedule(self, server_id: str, schedule_id: int):
+        """Runs the specified schedule.
+        
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            schedule_id(int): Schedule identifier
+        """
+        endpoint = 'client/servers/{}/schedules/{}/execute'.format(
+            server_id, schedule_id)
+        response = self._api_request(endpoint=endpoint, mode='POST')
+        return response
```

### Comparing `py-dactyl-2.0.1/pydactyl/api/client/servers/settings.py` & `py-dactyl-2.0.2/pydactyl/api/client/servers/settings.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from pydactyl.api import base
-
-
-class Settings(base.PterodactylAPI):
-    """Pterodactyl Client Server Settings API."""
-
-    def rename_server(self, server_id: str, name: str):
-        """Renames the server.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            name(str): New name for the server
-        """
-        data = {'name': name}
-        endpoint = 'client/servers/{}/settings/rename'.format(server_id)
-        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
-        return response
-
-    def reinstall_server(self, server_id: str):
-        """Reinstalls the specified server.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-        """
-        endpoint = 'client/servers/{}/settings/reinstall'.format(server_id)
-        response = self._api_request(endpoint=endpoint, mode='POST')
-        return response
+from pydactyl.api import base
+
+
+class Settings(base.PterodactylAPI):
+    """Pterodactyl Client Server Settings API."""
+
+    def rename_server(self, server_id: str, name: str):
+        """Renames the server.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            name(str): New name for the server
+        """
+        data = {'name': name}
+        endpoint = 'client/servers/{}/settings/rename'.format(server_id)
+        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
+        return response
+
+    def reinstall_server(self, server_id: str):
+        """Reinstalls the specified server.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+        """
+        endpoint = 'client/servers/{}/settings/reinstall'.format(server_id)
+        response = self._api_request(endpoint=endpoint, mode='POST')
+        return response
```

### Comparing `py-dactyl-2.0.1/pydactyl/api/client/servers/users.py` & `py-dactyl-2.0.2/pydactyl/api/client/servers/users.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-from pydactyl.api import base
-
-
-class Users(base.PterodactylAPI):
-    """Pterodactyl Client Server Backups API."""
-
-    def list_users(self, server_id: str):
-        """List all users added to the server.
-
-        Includes user details and permissions assigned to them.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-        """
-        endpoint = 'client/servers/{}/users'.format(server_id)
-        response = self._api_request(endpoint=endpoint)
-        return response
-
-    def create_user(self, server_id: str, email: str, permissions: iter,
-                    username: str = None):
-        """Adds a new user to the server.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            email(str): Email address of the new user
-            permissions(iter): List of permissions to assign to the user
-            username(str): Username to assign, randomized if not specified
-        """
-        data = {'email': email, 'permissions': permissions}
-        if username:
-            data['username'] = username
-        endpoint = 'client/servers/{}/users'.format(server_id)
-        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
-        return response
-
-    def get_user(self, server_id: str, user_id: str):
-        """Retrieves details about the specified user.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            user_id(str): User identifier (long UUID)
-        """
-        endpoint = 'client/servers/{}/users/{}'.format(server_id, user_id)
-        response = self._api_request(endpoint=endpoint)
-        return response
-
-    def update_user(self, server_id: str, user_id: str, permissions):
-        """Updates the specified user.
-
-        This probably has more options than the documentation list.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            user_id(str): User identifier (long UUID)
-            permissions(iter): List of permissions to assign to the user
-        """
-        data = {'permissions': permissions}
-        endpoint = 'client/servers/{}/users/{}'.format(server_id, user_id)
-        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
-        return response
-
-    def delete_user(self, server_id: str, user_id: str):
-        """Deletes the specified user.
-
-        Args:
-            server_id(str): Server identifier (abbreviated UUID)
-            user_id(str): User identifier (long UUID)
-        """
-        endpoint = 'client/servers/{}/users/{}'.format(server_id, user_id)
-        response = self._api_request(endpoint=endpoint, mode='DELETE')
-        return response
+from pydactyl.api import base
+
+
+class Users(base.PterodactylAPI):
+    """Pterodactyl Client Server Backups API."""
+
+    def list_users(self, server_id: str):
+        """List all users added to the server.
+
+        Includes user details and permissions assigned to them.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+        """
+        endpoint = 'client/servers/{}/users'.format(server_id)
+        response = self._api_request(endpoint=endpoint)
+        return response
+
+    def create_user(self, server_id: str, email: str, permissions: iter,
+                    username: str = None):
+        """Adds a new user to the server.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            email(str): Email address of the new user
+            permissions(iter): List of permissions to assign to the user
+            username(str): Username to assign, randomized if not specified
+        """
+        data = {'email': email, 'permissions': permissions}
+        if username:
+            data['username'] = username
+        endpoint = 'client/servers/{}/users'.format(server_id)
+        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
+        return response
+
+    def get_user(self, server_id: str, user_id: str):
+        """Retrieves details about the specified user.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            user_id(str): User identifier (long UUID)
+        """
+        endpoint = 'client/servers/{}/users/{}'.format(server_id, user_id)
+        response = self._api_request(endpoint=endpoint)
+        return response
+
+    def update_user(self, server_id: str, user_id: str, permissions):
+        """Updates the specified user.
+
+        This probably has more options than the documentation list.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            user_id(str): User identifier (long UUID)
+            permissions(iter): List of permissions to assign to the user
+        """
+        data = {'permissions': permissions}
+        endpoint = 'client/servers/{}/users/{}'.format(server_id, user_id)
+        response = self._api_request(endpoint=endpoint, mode='POST', data=data)
+        return response
+
+    def delete_user(self, server_id: str, user_id: str):
+        """Deletes the specified user.
+
+        Args:
+            server_id(str): Server identifier (abbreviated UUID)
+            user_id(str): User identifier (long UUID)
+        """
+        endpoint = 'client/servers/{}/users/{}'.format(server_id, user_id)
+        response = self._api_request(endpoint=endpoint, mode='DELETE')
+        return response
```

### Comparing `py-dactyl-2.0.1/pydactyl/api/nests.py` & `py-dactyl-2.0.2/pydactyl/api/nests.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from pydactyl.api.base import PterodactylAPI
-from pydactyl.responses import PaginatedResponse
-
-
-class Nests(PterodactylAPI):
-    """Class for interacting with the Pterdactyl Nests API."""
-
-    def list_nests(self, includes=None, params=None):
-        """List all nests.
-
-        Args:
-            includes(iter): List of includes, e.g. ('eggs', 'servers')
-            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
-        """
-        endpoint = 'application/nests'
-        response = self._api_request(endpoint=endpoint, includes=includes,
-                                     params=params)
-        return PaginatedResponse(self, endpoint, response)
-
-    def get_nest_info(self, nest_id, includes=None, params=None):
-        """Get detailed info for the specified nest.
-
-        Args:
-            nest_id(int): Pterodactyl Nest ID.
-            includes(iter): List of includes, e.g. ('eggs', 'servers')
-            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
-        """
-        response = self._api_request(
-            endpoint='application/nests/{}'.format(nest_id),
-            includes=includes, params=params)
-        return response
-
-    def get_eggs_in_nest(self, nest_id, includes=None, params=None):
-        """Get detailed info for the specified nest.
-
-        Args:
-            nest_id(int): Pterodactyl Nest ID.
-            includes(iter): List of includes, e.g. ('config', 'nest', 'script')
-            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
-        """
-        response = self._api_request(
-            endpoint='application/nests/{}/eggs'.format(nest_id),
-            includes=includes, params=params)
-        return response
-
-    def get_egg_info(self, nest_id, egg_id, includes=None, params=None):
-        """Get detailed info for the specified egg.
-
-        Args:
-            nest_id(int): Pterodactyl Nest ID.
-            egg_id(int): Pterodactyl Egg ID.
-            includes(iter): List of includes, e.g. ('config', 'nest', 'script')
-            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
-        """
-        response = self._api_request(
-            endpoint='application/nests/{}/eggs/{}'.format(nest_id, egg_id),
-            includes=includes, params=params)
-        return response
+from pydactyl.api.base import PterodactylAPI
+from pydactyl.responses import PaginatedResponse
+
+
+class Nests(PterodactylAPI):
+    """Class for interacting with the Pterdactyl Nests API."""
+
+    def list_nests(self, includes=None, params=None):
+        """List all nests.
+
+        Args:
+            includes(iter): List of includes, e.g. ('eggs', 'servers')
+            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
+        """
+        endpoint = 'application/nests'
+        response = self._api_request(endpoint=endpoint, includes=includes,
+                                     params=params)
+        return PaginatedResponse(self, endpoint, response)
+
+    def get_nest_info(self, nest_id, includes=None, params=None):
+        """Get detailed info for the specified nest.
+
+        Args:
+            nest_id(int): Pterodactyl Nest ID.
+            includes(iter): List of includes, e.g. ('eggs', 'servers')
+            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
+        """
+        response = self._api_request(
+            endpoint='application/nests/{}'.format(nest_id),
+            includes=includes, params=params)
+        return response
+
+    def get_eggs_in_nest(self, nest_id, includes=None, params=None):
+        """Get detailed info for the specified nest.
+
+        Args:
+            nest_id(int): Pterodactyl Nest ID.
+            includes(iter): List of includes, e.g. ('config', 'nest', 'script')
+            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
+        """
+        response = self._api_request(
+            endpoint='application/nests/{}/eggs'.format(nest_id),
+            includes=includes, params=params)
+        return response
+
+    def get_egg_info(self, nest_id, egg_id, includes=None, params=None):
+        """Get detailed info for the specified egg.
+
+        Args:
+            nest_id(int): Pterodactyl Nest ID.
+            egg_id(int): Pterodactyl Egg ID.
+            includes(iter): List of includes, e.g. ('config', 'nest', 'script')
+            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
+        """
+        response = self._api_request(
+            endpoint='application/nests/{}/eggs/{}'.format(nest_id, egg_id),
+            includes=includes, params=params)
+        return response
```

### Comparing `py-dactyl-2.0.1/pydactyl/api/servers.py` & `py-dactyl-2.0.2/pydactyl/api/servers.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,498 +1,498 @@
-from pydactyl.api import base
-from pydactyl.exceptions import BadRequestError
-from pydactyl.responses import PaginatedResponse
-
-
-class Servers(base.PterodactylAPI):
-    """Class for interacting with the Pterdactyl Servers API."""
-
-    def list_servers(self, includes=None, params=None):
-        """List all servers.
-
-        Args:
-            includes(iter): List of includes, e.g. ('allocations', 'node')
-            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
-        """
-        endpoint = 'application/servers'
-        response = base.parse_response(
-            self._api_request(endpoint=endpoint, includes=includes,
-                              params=params),
-            detail=True)
-        return PaginatedResponse(self, endpoint, response)
-
-    def get_server_info(self, server_id=None, external_id=None, detail=False,
-                        includes=None, params=None):
-        """Get detailed info for the specified server.
-
-        Args:
-            server_id(int): Pterodactyl Server ID.
-            external_id(int): Server ID from an external system like WHMCS
-            detail(bool): If True includes created and updated timestamps.
-            includes(iter): List of includes, e.g. ('egg', 'allocations')
-            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
-        """
-        if not server_id and not external_id:
-            raise BadRequestError('Must specify either server_id or '
-                                  'external_id.')
-        if server_id and external_id:
-            raise BadRequestError('Specify either server_id or external_id, '
-                                  'not both.')
-
-        if server_id:
-            endpoint = 'application/servers/{}'.format(server_id)
-        else:
-            endpoint = 'application/servers/external/{}'.format(external_id)
-
-        response = self._api_request(endpoint=endpoint, includes=includes,
-                                     params=params)
-        return base.parse_response(response, detail)
-
-    def suspend_server(self, server_id):
-        """Suspend the server with the specified internal ID.
-
-        Args:
-            server_id(int): Pterodactyl Server ID.
-        """
-        response = self._api_request(
-            endpoint='application/servers/{}/suspend'.format(server_id),
-            mode='POST')
-        return response
-
-    def unsuspend_server(self, server_id):
-        """Suspend the server with the specified internal ID.
-
-        Args:
-            server_id(int): Pterodactyl Server ID.
-        """
-        response = self._api_request(
-            endpoint='application/servers/{}/unsuspend'.format(server_id),
-            mode='POST')
-        return response
-
-    def reinstall_server(self, server_id):
-        """Reinstall the server with the specified internal ID.
-
-        Args:
-            server_id(int): Pterodactyl Server ID.
-        """
-        response = self._api_request(
-            endpoint='application/servers/{}/reinstall'.format(server_id),
-            mode='POST')
-        return response
-
-    def rebuild_server(self, server_id):
-        """Rebuild the server with the specified internal ID.
-
-        Args:
-            server_id(int): Pterodactyl Server ID.
-        """
-        response = self._api_request(
-            endpoint='application/servers/{}/rebuild'.format(server_id),
-            mode='POST')
-        return response
-
-    def delete_server(self, server_id, force=False):
-        """Delete the server with the specified internal ID.
-
-        Attempts to delete the server from both the panel and daemon.
-        By default if either one reports an error the action will be cancelled.
-
-        Args:
-            server_id(int): Pterodactyl Server ID.
-            force(bool): If True the delete action will continue if the panel or
-                    daemon reports an error.
-        """
-        endpoint = 'application/servers/{}'.format(server_id)
-        if force:
-            endpoint += '/force'
-
-        response = self._api_request(endpoint=endpoint, mode='DELETE')
-        return response
-
-    def list_server_databases(self, server_id, includes=None, params=None):
-        """List the database servers assigned to the specified server ID.
-
-        Args:
-            server_id(int): Pterodactyl Server ID.
-            includes(iter): List of includes, e.g. ('password', 'host')
-            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
-        """
-        endpoint = 'application/servers/{}/databases'.format(server_id)
-        response = self._api_request(endpoint=endpoint, includes=includes,
-                                     params=params)
-        return PaginatedResponse(self, endpoint, response)
-
-    def get_server_database_info(self, server_id, database_id, detail=False,
-                                 includes=None, params=None):
-        """Get information about the specified database on the specified server.
-
-        Args:
-            server_id(int): Pterodactyl Server ID.
-            database_id(int): Database ID for specified server.
-            detail(bool): If True includes the object type and a nested data
-                    structure.
-            includes(iter): List of includes, e.g. ('password', 'host')
-            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
-        """
-        endpoint = 'application/servers/{}/databases/{}'.format(server_id,
-                                                                database_id)
-        response = self._api_request(endpoint=endpoint, includes=includes,
-                                     params=params)
-        return base.parse_response(response, detail)
-
-    def create_server_database(self, server_id):
-        """Create a database for the specified server.
-
-        Args:
-            server_id(int): Pterodactyl Server ID.
-        """
-        response = self._api_request(
-            endpoint='application/servers/{}/databases'.format(server_id),
-            mode='POST')
-        return response
-
-    def delete_server_database(self, server_id, database_id):
-        """Delete the specified database for the specified server.
-
-        Args:
-            server_id(int): Pterodactyl Server ID.
-            database_id(int): Database ID for specified server.
-        """
-        response = self._api_request(
-            endpoint='application/servers/{}/databases/{}'.format(server_id,
-                                                                  database_id),
-            mode='DELETE')
-        return response
-
-    def reset_server_database_password(self, server_id, database_id):
-        """Resets the password for the specified server database.
-
-        Args:
-            server_id(int): Pterodactyl Server ID.
-            database_id(int): Database ID for specified server.
-        """
-        response = self._api_request(
-            endpoint='application/servers/{}/databases/{}'
-                     '/reset-password'.format(server_id, database_id),
-            mode='POST')
-        return response
-
-    def create_server(self, name, user_id, nest_id, egg_id, memory_limit,
-                      swap_limit, disk_limit, location_ids=[], port_range=[],
-                      environment={}, cpu_limit=0, io_limit=500,
-                      database_limit=0, allocation_limit=0, backup_limit=0,
-                      docker_image=None, startup_cmd=None, dedicated_ip=False,
-                      start_on_completion=True, oom_disabled=True,
-                      default_allocation=None, additional_allocations=None,
-                      external_id=None, description=None):
-        """Creates one or more servers in the specified locations.
-
-        Creates server instance(s) and begins the install process using the
-        specified configurations and limits.  If more than one value is
-        specified for location_ids then identical servers will be created in
-        each location.
-
-        Args:
-            name(str): Name of the server to display in the panel.
-            user_id(int): User ID that will own the server.
-            nest_id(int): Nest ID for the created server.
-            egg_id(int): Egg ID for the created server.
-            memory_limit(int): Memory limit in MB for the Docker container.  To
-                    allow unlimited memory limit set to 0.
-            swap_limit(int): Swap limit in MB for the Docker container.  To not
-                    assign any swap set to 0.  For unlimited swap set to -1.
-            disk_limit(int): Disk limit in MB for the Docker container.  To
-                    allow unlimited disk space set to 0.
-            environment(dict): Key value pairs of Service Variables to set.
-                    Every variable from the egg must be set or the API will
-                    return an error.  Default values will be pulled from the egg
-                    config or set to None.
-            location_ids(iter): List of location_ids where the server(s) will be
-                    created.  If more than one location is specified
-                    identical servers will be created at each.
-            port_range(iter): List of ports or port ranges to use when
-                    selecting an allocation.  If empty, all ports will be
-                    considered.  If set, only ports appearing in the list or
-                    range will be used.  e.g. [20715, '20815-20915']
-            cpu_limit(int): CPU limit for the Docker container.  To allow
-                    unlimited CPU usage set to 0.  To limit to one core set
-                    to 100.  For four cores set to 400.
-            io_limit(int): Block IO weight for the Docker container.
-                    Must be between 10 and 1000.
-            database_limit(int): Maximum number of databases that can be
-                    assigned to this server.
-            allocation_limit(int): Maximum number of allocations that can be
-                    assigned to this server.
-            backup_limit(int): Maximum number of backups that can be
-                    created for this server.
-            docker_image(str): Name or URL of the Docker server to use.
-                    e.g. quay.io/pterodactyl/core:java-glibc
-            startup_cmd(str): Startup command, if specified replaces the
-                    egg's default value.
-            dedicated_ip(bool): Limit allocations to IPs without any existing
-                    allocations.
-            start_on_completion(bool): Start server after install completes.
-            oom_disabled(bool): Disables OOM-killer on the Docker container.
-            default_allocation(int): Specify allocation(s) instead of using the
-                    Pterodactyl deployment service.  Uses the allocation's
-                    internal ID and not the port number.
-            additional_allocations(iter): Additional allocations on top of
-                    default_allocation.
-            description(str): A description of the server if needed
-        """
-        if default_allocation is None and not location_ids:
-            raise BadRequestError('Must specify either default_allocation or '
-                                  'location_ids')
-
-        # Fetch the Egg variables which are required to create the server.
-        egg_info = self._api_request(
-            endpoint='application/nests/{}/eggs/{}'.format(
-                nest_id, egg_id), params={'include': 'variables'})['attributes']
-        egg_vars = egg_info['relationships']['variables']['data']
-
-        # Build a dict of environment variables.  Prefer values passed in the
-        # environment parameter, otherwise use the default value from the Egg
-        # config.
-        env_with_defaults = {}
-        for var in egg_vars:
-            var_name = var['attributes']['env_variable']
-            if var_name in environment:
-                env_with_defaults[var_name] = environment[var_name]
-            else:
-                env_with_defaults[var_name] = var['attributes'].get(
-                    'default_value')
-
-        if not docker_image:
-            docker_image = egg_info.get('docker_image')
-        if not startup_cmd:
-            startup_cmd = egg_info.get('startup')
-
-        data = {
-            'name': name,
-            'user': user_id,
-            'external_id': external_id,
-            'nest': nest_id,
-            'egg': egg_id,
-            'docker_image': docker_image,
-            'startup': startup_cmd,
-            'oom_disabled': oom_disabled,
-            'limits': {
-                'memory': memory_limit,
-                'swap': swap_limit,
-                'disk': disk_limit,
-                'io': io_limit,
-                'cpu': cpu_limit,
-            },
-            'feature_limits': {
-                'databases': database_limit,
-                'allocations': allocation_limit,
-                'backups': backup_limit
-            },
-            'environment': env_with_defaults,
-            'start_on_completion': start_on_completion,
-            'description': description,
-        }
-
-        if default_allocation is not None:
-            data['allocation'] = {'default': default_allocation,
-                                  'additional': additional_allocations}
-        elif location_ids:
-            data['deploy'] = {'locations': location_ids,
-                              'dedicated_ip': dedicated_ip,
-                              'port_range': port_range}
-
-        response = self._api_request(endpoint='application/servers',
-                                     mode='POST', data=data, json=False)
-        return response
-    
-    def update_server_details(self, server_id, name, user_id, external_id=None, description=None):
-        """Updates the details of an existing server.
-        
-        Modifies an existing server details identified by its Pterodactyl id.
-        
-        Example of a working set of parameters:
-            update_server_details(server_id=10, name='My awesome Server', external_id='some_id2389234', description='This is really an awesome server !'
-            
-        Args:
-            server_id(int): Internal server ID, e.g. 12
-            name(str): Name of the server to display in the panel.
-            user_id(int): User ID that will own the server.
-            external_id(int): Server ID from an external system like WHMCS
-            description(str): A description of the server if needed"""
-
-        data = {
-            'name': name,
-            'user': user_id,
-            'external_id': external_id,
-            'description': description
-        }
-
-        response = self._api_request(
-            endpoint='application/servers/{}/details'.format(server_id),
-            mode='PATCH', data=data, json=False)
-        return response
-
-
-
-    def update_server_build(self, server_id, allocation_id, memory_limit=None,
-                            swap_limit=None, disk_limit=None, cpu_limit=None,
-                            io_limit=None, database_limit=None,
-                            allocation_limit=None, backup_limit=None,
-                            add_allocations=None,
-                            remove_allocations=None, oom_disabled=None):
-        """Updates the build configuration for an existing server.
-
-        Modifies an existing server identified by allocation_id and updates
-        any parameters that are passed.
-
-        *** WARNING ***
-        This endpoint has a lot of requirements and it doesn't always surface
-        helpful errors.  Sometimes they're in the panel logs.  I plan to
-        automate some of the painful parts so you can specify only the fields
-        you want to update, however currently you must satisfy the API's
-        requirements by passing in everything.
-
-        Example of a working set of parameters:
-            update_server_build(server_id=12, allocation_id=81, 
-                    memory_limit=2048, swap_limit=2048, disk_limit=5120, 
-                    cpu_limit=100, io_limit=500, database_limit=1, 
-                    allocation_limit=2, backup_limit=4, 
-                    add_allocations=None, remove_allocations=None, 
-                    oom_disabled=True)
-
-        Args:
-            server_id(int): Internal server ID, e.g. 12
-            allocation_id(int): Base allocation of the server to modify.
-            memory_limit(int): Memory limit in MB for the Docker container.  To
-                    allow unlimited memory limit set to 0.
-            swap_limit(int): Swap limit in MB for the Docker container.  To not
-                    assign any swap set to 0.  For unlimited swap set to -1.
-            disk_limit(int): Disk limit in MB for the Docker container.  To
-                    allow unlimited disk space set to 0.
-            cpu_limit(int): CPU limit for the Docker container.  To allow
-                    unlimited CPU usage set to 0.  To limit to one core set
-                    to 100.  For four cores set to 400.
-            io_limit(int): Block IO weight for the Docker container.
-                    Must be between 10 and 1000.
-            database_limit(int): Maximum number of databases that can be
-                    assigned to this server.
-            allocation_limit(int): Maximum number of allocations that can be
-                    assigned to this server.
-            backup_limit(int): Maximum number of backups that can be
-                    assigned to this server.
-            add_allocations(iter): List of allocation IDs to add to the server.
-            remove_allocations(iter): List of allocation IDs to remove from
-                    the server.
-            oom_disabled(bool): Disables OOM-killer on the Docker container.
-        """
-        data = {
-            'allocation': allocation_id,
-            'limits': {},
-            'feature_limits': {},
-        }
-
-        if memory_limit is not None:
-            data['limits']['memory'] = memory_limit
-        if swap_limit is not None:
-            data['limits']['swap'] = swap_limit
-        if disk_limit is not None:
-            data['limits']['disk'] = disk_limit
-        if cpu_limit is not None:
-            data['limits']['cpu'] = cpu_limit
-        if io_limit is not None:
-            data['limits']['io'] = io_limit
-        if database_limit is not None:
-            data['feature_limits']['databases'] = database_limit
-        if allocation_limit is not None:
-            data['feature_limits']['allocations'] = allocation_limit
-        if backup_limit is not None:
-            data['feature_limits']['backups'] = backup_limit
-        if add_allocations is not None:
-            data['add_allocations'] = add_allocations
-        if remove_allocations is not None:
-            data['remove_allocations'] = remove_allocations
-        if oom_disabled is not None:
-            data['oom_disabled'] = oom_disabled
-
-        response = self._api_request(
-            endpoint='application/servers/{}/build'.format(server_id),
-            mode='PATCH', data=data, json=False)
-        return response
-
-    def update_server_startup(self, server_id, egg_id=None,
-                              environment={}, docker_image=None,
-                              startup_cmd=None, skip_scripts=None):
-        """Updates the startup config for the specified server.
-
-        Modifies the startup config of an existing server replacing any
-        specified values.  Unspecified values will not be changed.
-
-        Args:
-            egg_id(int): Egg ID to update on the server.
-            environment(dict): Key value pairs of Service Variables to set.
-                    Every variable from the egg must be set or the API will
-                    return an error.  Any keys specified will be overwritten
-                    in the existing environment list.  Unspecified keys will
-                    not be modified. Extra keys will be dropped.
-            docker_image(str): Name or URL of the Docker server to use.
-                    e.g. quay.io/pterodactyl/core:java-glibc
-            startup_cmd(str): Startup command, if specified replaces the
-                    egg's default value.
-            skip_scripts(bool): True to skip egg scripts.
-        """
-        server_info = self._api_request(
-            endpoint='application/servers/{}'.format(server_id),
-            params={'include': 'variables'})['attributes']
-        container = server_info['container']
-        current_env = container['environment']
-        current_egg = server_info['egg']
-        merged_env = {}
-        if egg_id is not None and egg_id != current_egg:
-            nest_id = server_info['nest']
-            egg_info = self._api_request(
-                endpoint='application/nests/{}/eggs/{}'.format(nest_id, egg_id),
-                params={'include': 'variables'})['attributes']
-            egg_vars = egg_info['relationships']['variables']['data']
-
-            # Build a dict of environment variables. Prefer values passed in
-            # the environment parameter, then those set in the current env,
-            # then finally use the default value from the Egg config.
-            for var in egg_vars:
-                var_name = var['attributes']['env_variable']
-                if var_name in environment:
-                    merged_env[var_name] = environment[var_name]
-                elif var_name in current_env:
-                    merged_env[var_name] = current_env[var_name]
-                else:
-                    merged_env[var_name] = var['attributes'].get(
-                        'default_value')
-            if not docker_image:
-                docker_image = egg_info.get('docker_image')
-            if not startup_cmd:
-                startup_cmd = egg_info.get('startup')
-        elif environment is not None:
-            # If extra values are passed they are silently dropped by the API
-            #   could detect attempts to set invalid variables and throw.
-            # Also could reduce the contents of current_env down to the
-            #   set of variables, there's extra info in here that seems
-            #   to not matter if it's set or not.
-            merged_env = current_env
-            merged_env.update(environment)
-
-        data = {
-            'egg': egg_id if egg_id is not None else current_egg,
-            'startup': startup_cmd if startup_cmd is not None else container[
-                'startup_command'],
-            'image': docker_image if docker_image is not None else container[
-                'image'],
-            # Cant find a way to get the current value for this setting
-            #   and this seems better than assuming true or false
-            'skip_scripts': skip_scripts if skip_scripts is not None else
-            container['installed'] == 1,
-            'environment': merged_env
-        }
-
-        response = self._api_request(
-            endpoint='application/servers/{}/startup'.format(server_id),
-            mode='PATCH', data=data, json=False)
-        return response
+from pydactyl.api import base
+from pydactyl.exceptions import BadRequestError
+from pydactyl.responses import PaginatedResponse
+
+
+class Servers(base.PterodactylAPI):
+    """Class for interacting with the Pterdactyl Servers API."""
+
+    def list_servers(self, includes=None, params=None):
+        """List all servers.
+
+        Args:
+            includes(iter): List of includes, e.g. ('allocations', 'node')
+            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
+        """
+        endpoint = 'application/servers'
+        response = base.parse_response(
+            self._api_request(endpoint=endpoint, includes=includes,
+                              params=params),
+            detail=True)
+        return PaginatedResponse(self, endpoint, response)
+
+    def get_server_info(self, server_id=None, external_id=None, detail=False,
+                        includes=None, params=None):
+        """Get detailed info for the specified server.
+
+        Args:
+            server_id(int): Pterodactyl Server ID.
+            external_id(int): Server ID from an external system like WHMCS
+            detail(bool): If True includes created and updated timestamps.
+            includes(iter): List of includes, e.g. ('egg', 'allocations')
+            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
+        """
+        if not server_id and not external_id:
+            raise BadRequestError('Must specify either server_id or '
+                                  'external_id.')
+        if server_id and external_id:
+            raise BadRequestError('Specify either server_id or external_id, '
+                                  'not both.')
+
+        if server_id:
+            endpoint = 'application/servers/{}'.format(server_id)
+        else:
+            endpoint = 'application/servers/external/{}'.format(external_id)
+
+        response = self._api_request(endpoint=endpoint, includes=includes,
+                                     params=params)
+        return base.parse_response(response, detail)
+
+    def suspend_server(self, server_id):
+        """Suspend the server with the specified internal ID.
+
+        Args:
+            server_id(int): Pterodactyl Server ID.
+        """
+        response = self._api_request(
+            endpoint='application/servers/{}/suspend'.format(server_id),
+            mode='POST')
+        return response
+
+    def unsuspend_server(self, server_id):
+        """Suspend the server with the specified internal ID.
+
+        Args:
+            server_id(int): Pterodactyl Server ID.
+        """
+        response = self._api_request(
+            endpoint='application/servers/{}/unsuspend'.format(server_id),
+            mode='POST')
+        return response
+
+    def reinstall_server(self, server_id):
+        """Reinstall the server with the specified internal ID.
+
+        Args:
+            server_id(int): Pterodactyl Server ID.
+        """
+        response = self._api_request(
+            endpoint='application/servers/{}/reinstall'.format(server_id),
+            mode='POST')
+        return response
+
+    def rebuild_server(self, server_id):
+        """Rebuild the server with the specified internal ID.
+
+        Args:
+            server_id(int): Pterodactyl Server ID.
+        """
+        response = self._api_request(
+            endpoint='application/servers/{}/rebuild'.format(server_id),
+            mode='POST')
+        return response
+
+    def delete_server(self, server_id, force=False):
+        """Delete the server with the specified internal ID.
+
+        Attempts to delete the server from both the panel and daemon.
+        By default if either one reports an error the action will be cancelled.
+
+        Args:
+            server_id(int): Pterodactyl Server ID.
+            force(bool): If True the delete action will continue if the panel or
+                    daemon reports an error.
+        """
+        endpoint = 'application/servers/{}'.format(server_id)
+        if force:
+            endpoint += '/force'
+
+        response = self._api_request(endpoint=endpoint, mode='DELETE')
+        return response
+
+    def list_server_databases(self, server_id, includes=None, params=None):
+        """List the database servers assigned to the specified server ID.
+
+        Args:
+            server_id(int): Pterodactyl Server ID.
+            includes(iter): List of includes, e.g. ('password', 'host')
+            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
+        """
+        endpoint = 'application/servers/{}/databases'.format(server_id)
+        response = self._api_request(endpoint=endpoint, includes=includes,
+                                     params=params)
+        return PaginatedResponse(self, endpoint, response)
+
+    def get_server_database_info(self, server_id, database_id, detail=False,
+                                 includes=None, params=None):
+        """Get information about the specified database on the specified server.
+
+        Args:
+            server_id(int): Pterodactyl Server ID.
+            database_id(int): Database ID for specified server.
+            detail(bool): If True includes the object type and a nested data
+                    structure.
+            includes(iter): List of includes, e.g. ('password', 'host')
+            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
+        """
+        endpoint = 'application/servers/{}/databases/{}'.format(server_id,
+                                                                database_id)
+        response = self._api_request(endpoint=endpoint, includes=includes,
+                                     params=params)
+        return base.parse_response(response, detail)
+
+    def create_server_database(self, server_id):
+        """Create a database for the specified server.
+
+        Args:
+            server_id(int): Pterodactyl Server ID.
+        """
+        response = self._api_request(
+            endpoint='application/servers/{}/databases'.format(server_id),
+            mode='POST')
+        return response
+
+    def delete_server_database(self, server_id, database_id):
+        """Delete the specified database for the specified server.
+
+        Args:
+            server_id(int): Pterodactyl Server ID.
+            database_id(int): Database ID for specified server.
+        """
+        response = self._api_request(
+            endpoint='application/servers/{}/databases/{}'.format(server_id,
+                                                                  database_id),
+            mode='DELETE')
+        return response
+
+    def reset_server_database_password(self, server_id, database_id):
+        """Resets the password for the specified server database.
+
+        Args:
+            server_id(int): Pterodactyl Server ID.
+            database_id(int): Database ID for specified server.
+        """
+        response = self._api_request(
+            endpoint='application/servers/{}/databases/{}'
+                     '/reset-password'.format(server_id, database_id),
+            mode='POST')
+        return response
+
+    def create_server(self, name, user_id, nest_id, egg_id, memory_limit,
+                      swap_limit, disk_limit, location_ids=[], port_range=[],
+                      environment={}, cpu_limit=0, io_limit=500,
+                      database_limit=0, allocation_limit=0, backup_limit=0,
+                      docker_image=None, startup_cmd=None, dedicated_ip=False,
+                      start_on_completion=True, oom_disabled=True,
+                      default_allocation=None, additional_allocations=None,
+                      external_id=None, description=None):
+        """Creates one or more servers in the specified locations.
+
+        Creates server instance(s) and begins the install process using the
+        specified configurations and limits.  If more than one value is
+        specified for location_ids then identical servers will be created in
+        each location.
+
+        Args:
+            name(str): Name of the server to display in the panel.
+            user_id(int): User ID that will own the server.
+            nest_id(int): Nest ID for the created server.
+            egg_id(int): Egg ID for the created server.
+            memory_limit(int): Memory limit in MB for the Docker container.  To
+                    allow unlimited memory limit set to 0.
+            swap_limit(int): Swap limit in MB for the Docker container.  To not
+                    assign any swap set to 0.  For unlimited swap set to -1.
+            disk_limit(int): Disk limit in MB for the Docker container.  To
+                    allow unlimited disk space set to 0.
+            environment(dict): Key value pairs of Service Variables to set.
+                    Every variable from the egg must be set or the API will
+                    return an error.  Default values will be pulled from the egg
+                    config or set to None.
+            location_ids(iter): List of location_ids where the server(s) will be
+                    created.  If more than one location is specified
+                    identical servers will be created at each.
+            port_range(iter): List of ports or port ranges to use when
+                    selecting an allocation.  If empty, all ports will be
+                    considered.  If set, only ports appearing in the list or
+                    range will be used.  e.g. [20715, '20815-20915']
+            cpu_limit(int): CPU limit for the Docker container.  To allow
+                    unlimited CPU usage set to 0.  To limit to one core set
+                    to 100.  For four cores set to 400.
+            io_limit(int): Block IO weight for the Docker container.
+                    Must be between 10 and 1000.
+            database_limit(int): Maximum number of databases that can be
+                    assigned to this server.
+            allocation_limit(int): Maximum number of allocations that can be
+                    assigned to this server.
+            backup_limit(int): Maximum number of backups that can be
+                    created for this server.
+            docker_image(str): Name or URL of the Docker server to use.
+                    e.g. quay.io/pterodactyl/core:java-glibc
+            startup_cmd(str): Startup command, if specified replaces the
+                    egg's default value.
+            dedicated_ip(bool): Limit allocations to IPs without any existing
+                    allocations.
+            start_on_completion(bool): Start server after install completes.
+            oom_disabled(bool): Disables OOM-killer on the Docker container.
+            default_allocation(int): Specify allocation(s) instead of using the
+                    Pterodactyl deployment service.  Uses the allocation's
+                    internal ID and not the port number.
+            additional_allocations(iter): Additional allocations on top of
+                    default_allocation.
+            description(str): A description of the server if needed
+        """
+        if default_allocation is None and not location_ids:
+            raise BadRequestError('Must specify either default_allocation or '
+                                  'location_ids')
+
+        # Fetch the Egg variables which are required to create the server.
+        egg_info = self._api_request(
+            endpoint='application/nests/{}/eggs/{}'.format(
+                nest_id, egg_id), params={'include': 'variables'})['attributes']
+        egg_vars = egg_info['relationships']['variables']['data']
+
+        # Build a dict of environment variables.  Prefer values passed in the
+        # environment parameter, otherwise use the default value from the Egg
+        # config.
+        env_with_defaults = {}
+        for var in egg_vars:
+            var_name = var['attributes']['env_variable']
+            if var_name in environment:
+                env_with_defaults[var_name] = environment[var_name]
+            else:
+                env_with_defaults[var_name] = var['attributes'].get(
+                    'default_value')
+
+        if not docker_image:
+            docker_image = egg_info.get('docker_image')
+        if not startup_cmd:
+            startup_cmd = egg_info.get('startup')
+
+        data = {
+            'name': name,
+            'user': user_id,
+            'external_id': external_id,
+            'nest': nest_id,
+            'egg': egg_id,
+            'docker_image': docker_image,
+            'startup': startup_cmd,
+            'oom_disabled': oom_disabled,
+            'limits': {
+                'memory': memory_limit,
+                'swap': swap_limit,
+                'disk': disk_limit,
+                'io': io_limit,
+                'cpu': cpu_limit,
+            },
+            'feature_limits': {
+                'databases': database_limit,
+                'allocations': allocation_limit,
+                'backups': backup_limit
+            },
+            'environment': env_with_defaults,
+            'start_on_completion': start_on_completion,
+            'description': description,
+        }
+
+        if default_allocation is not None:
+            data['allocation'] = {'default': default_allocation,
+                                  'additional': additional_allocations}
+        elif location_ids:
+            data['deploy'] = {'locations': location_ids,
+                              'dedicated_ip': dedicated_ip,
+                              'port_range': port_range}
+
+        response = self._api_request(endpoint='application/servers',
+                                     mode='POST', data=data, json=False)
+        return response
+    
+    def update_server_details(self, server_id, name, user_id, external_id=None, description=None):
+        """Updates the details of an existing server.
+        
+        Modifies an existing server details identified by its Pterodactyl id.
+        
+        Example of a working set of parameters:
+            update_server_details(server_id=10, name='My awesome Server', external_id='some_id2389234', description='This is really an awesome server !'
+            
+        Args:
+            server_id(int): Internal server ID, e.g. 12
+            name(str): Name of the server to display in the panel.
+            user_id(int): User ID that will own the server.
+            external_id(int): Server ID from an external system like WHMCS
+            description(str): A description of the server if needed"""
+
+        data = {
+            'name': name,
+            'user': user_id,
+            'external_id': external_id,
+            'description': description
+        }
+
+        response = self._api_request(
+            endpoint='application/servers/{}/details'.format(server_id),
+            mode='PATCH', data=data, json=False)
+        return response
+
+
+
+    def update_server_build(self, server_id, allocation_id, memory_limit=None,
+                            swap_limit=None, disk_limit=None, cpu_limit=None,
+                            io_limit=None, database_limit=None,
+                            allocation_limit=None, backup_limit=None,
+                            add_allocations=None,
+                            remove_allocations=None, oom_disabled=None):
+        """Updates the build configuration for an existing server.
+
+        Modifies an existing server identified by allocation_id and updates
+        any parameters that are passed.
+
+        *** WARNING ***
+        This endpoint has a lot of requirements and it doesn't always surface
+        helpful errors.  Sometimes they're in the panel logs.  I plan to
+        automate some of the painful parts so you can specify only the fields
+        you want to update, however currently you must satisfy the API's
+        requirements by passing in everything.
+
+        Example of a working set of parameters:
+            update_server_build(server_id=12, allocation_id=81, 
+                    memory_limit=2048, swap_limit=2048, disk_limit=5120, 
+                    cpu_limit=100, io_limit=500, database_limit=1, 
+                    allocation_limit=2, backup_limit=4, 
+                    add_allocations=None, remove_allocations=None, 
+                    oom_disabled=True)
+
+        Args:
+            server_id(int): Internal server ID, e.g. 12
+            allocation_id(int): Base allocation of the server to modify.
+            memory_limit(int): Memory limit in MB for the Docker container.  To
+                    allow unlimited memory limit set to 0.
+            swap_limit(int): Swap limit in MB for the Docker container.  To not
+                    assign any swap set to 0.  For unlimited swap set to -1.
+            disk_limit(int): Disk limit in MB for the Docker container.  To
+                    allow unlimited disk space set to 0.
+            cpu_limit(int): CPU limit for the Docker container.  To allow
+                    unlimited CPU usage set to 0.  To limit to one core set
+                    to 100.  For four cores set to 400.
+            io_limit(int): Block IO weight for the Docker container.
+                    Must be between 10 and 1000.
+            database_limit(int): Maximum number of databases that can be
+                    assigned to this server.
+            allocation_limit(int): Maximum number of allocations that can be
+                    assigned to this server.
+            backup_limit(int): Maximum number of backups that can be
+                    assigned to this server.
+            add_allocations(iter): List of allocation IDs to add to the server.
+            remove_allocations(iter): List of allocation IDs to remove from
+                    the server.
+            oom_disabled(bool): Disables OOM-killer on the Docker container.
+        """
+        data = {
+            'allocation': allocation_id,
+            'limits': {},
+            'feature_limits': {},
+        }
+
+        if memory_limit is not None:
+            data['limits']['memory'] = memory_limit
+        if swap_limit is not None:
+            data['limits']['swap'] = swap_limit
+        if disk_limit is not None:
+            data['limits']['disk'] = disk_limit
+        if cpu_limit is not None:
+            data['limits']['cpu'] = cpu_limit
+        if io_limit is not None:
+            data['limits']['io'] = io_limit
+        if database_limit is not None:
+            data['feature_limits']['databases'] = database_limit
+        if allocation_limit is not None:
+            data['feature_limits']['allocations'] = allocation_limit
+        if backup_limit is not None:
+            data['feature_limits']['backups'] = backup_limit
+        if add_allocations is not None:
+            data['add_allocations'] = add_allocations
+        if remove_allocations is not None:
+            data['remove_allocations'] = remove_allocations
+        if oom_disabled is not None:
+            data['oom_disabled'] = oom_disabled
+
+        response = self._api_request(
+            endpoint='application/servers/{}/build'.format(server_id),
+            mode='PATCH', data=data, json=False)
+        return response
+
+    def update_server_startup(self, server_id, egg_id=None,
+                              environment={}, docker_image=None,
+                              startup_cmd=None, skip_scripts=None):
+        """Updates the startup config for the specified server.
+
+        Modifies the startup config of an existing server replacing any
+        specified values.  Unspecified values will not be changed.
+
+        Args:
+            egg_id(int): Egg ID to update on the server.
+            environment(dict): Key value pairs of Service Variables to set.
+                    Every variable from the egg must be set or the API will
+                    return an error.  Any keys specified will be overwritten
+                    in the existing environment list.  Unspecified keys will
+                    not be modified. Extra keys will be dropped.
+            docker_image(str): Name or URL of the Docker server to use.
+                    e.g. quay.io/pterodactyl/core:java-glibc
+            startup_cmd(str): Startup command, if specified replaces the
+                    egg's default value.
+            skip_scripts(bool): True to skip egg scripts.
+        """
+        server_info = self._api_request(
+            endpoint='application/servers/{}'.format(server_id),
+            params={'include': 'variables'})['attributes']
+        container = server_info['container']
+        current_env = container['environment']
+        current_egg = server_info['egg']
+        merged_env = {}
+        if egg_id is not None and egg_id != current_egg:
+            nest_id = server_info['nest']
+            egg_info = self._api_request(
+                endpoint='application/nests/{}/eggs/{}'.format(nest_id, egg_id),
+                params={'include': 'variables'})['attributes']
+            egg_vars = egg_info['relationships']['variables']['data']
+
+            # Build a dict of environment variables. Prefer values passed in
+            # the environment parameter, then those set in the current env,
+            # then finally use the default value from the Egg config.
+            for var in egg_vars:
+                var_name = var['attributes']['env_variable']
+                if var_name in environment:
+                    merged_env[var_name] = environment[var_name]
+                elif var_name in current_env:
+                    merged_env[var_name] = current_env[var_name]
+                else:
+                    merged_env[var_name] = var['attributes'].get(
+                        'default_value')
+            if not docker_image:
+                docker_image = egg_info.get('docker_image')
+            if not startup_cmd:
+                startup_cmd = egg_info.get('startup')
+        elif environment is not None:
+            # If extra values are passed they are silently dropped by the API
+            #   could detect attempts to set invalid variables and throw.
+            # Also could reduce the contents of current_env down to the
+            #   set of variables, there's extra info in here that seems
+            #   to not matter if it's set or not.
+            merged_env = current_env
+            merged_env.update(environment)
+
+        data = {
+            'egg': egg_id if egg_id is not None else current_egg,
+            'startup': startup_cmd if startup_cmd is not None else container[
+                'startup_command'],
+            'image': docker_image if docker_image is not None else container[
+                'image'],
+            # Cant find a way to get the current value for this setting
+            #   and this seems better than assuming true or false
+            'skip_scripts': skip_scripts if skip_scripts is not None else
+            container['installed'] == 1,
+            'environment': merged_env
+        }
+
+        response = self._api_request(
+            endpoint='application/servers/{}/startup'.format(server_id),
+            mode='PATCH', data=data, json=False)
+        return response
```

### Comparing `py-dactyl-2.0.1/pydactyl/api/user.py` & `py-dactyl-2.0.2/pydactyl/api/user.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-from pydactyl.api import base
-from pydactyl.api.base import PterodactylAPI
-from pydactyl.exceptions import BadRequestError
-from pydactyl.responses import PaginatedResponse
-
-
-class User(PterodactylAPI):
-    """Class for interacting with the Pterdactyl Client API."""
-
-    def list_users(self, email=None, uuid=None, username=None,
-                   external_id=None, includes=None, params=None):
-        """List all users.
-
-        Accepts optional filter parameters.  If multiple filters are specified
-        only results that match all filters will be returned.
-
-        Args:
-            email(str): Filter by email
-            uuid(str): Filter by uuid
-            username(str): Filter by username
-            external_id(int): Filter by external_id
-            includes(iter): List of includes, e.g. ('servers')
-            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
-        """
-        filters = {}
-        if email:
-            filters['filter[email]'] = email
-        if uuid:
-            filters['filter[uuid]'] = uuid
-        if username:
-            filters['filter[username]'] = username
-        if external_id:
-            filters['filter[external_id]'] = external_id
-
-        if params:
-            filters.update(params)
-        endpoint = 'application/users'
-        response = self._api_request(endpoint=endpoint,
-                                     includes=includes, params=filters)
-        return PaginatedResponse(self, endpoint, response)
-
-    def get_user_info(self, user_id=None, external_id=None, detail=True,
-                      includes=None, params=None):
-        """List detailed user information for specified user_id.
-
-        Args:
-            user_id(int): Pterodactyl user ID
-            external_id(int): User ID from external system like WHMCS
-            detail(bool): If True includes created and updated timestamps.
-            includes(iter): List of includes, e.g. ('servers')
-            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
-        """
-        if not user_id and not external_id:
-            raise BadRequestError('Must specify either user_id or external_id.')
-        if user_id and external_id:
-            raise BadRequestError('Specify either user_id or external_id, '
-                                  'not both.')
-
-        if user_id:
-            endpoint = 'application/users/{}'.format(user_id)
-        else:
-            endpoint = 'application/users/external/{}'.format(external_id)
-
-        response = self._api_request(endpoint=endpoint, includes=includes,
-                                     params=params)
-        return base.parse_response(response, detail=detail)
-
-    def create_user(self, username, email, first_name, last_name,
-                    external_id=None, password=None, root_admin=False,
-                    language='en'):
-        """Creates a primary user on the Pterodactyl panel.
-
-        Args:
-            username(str): Username, must be unique, required.
-            email(str): Full email, required.
-            first_name(str): User's first name, required.
-            last_name(str): User's last name, required.
-            external_id(str): User ID from external system like WHMCS.
-            password(str): Optionally specify a password.  If not specified
-                    user will receive an email to setup their password.
-            root_admin(bool): Whether the account is an admin.
-            language(str): Used to specify the default language for an account.
-        """
-        data = {'username': username,
-                'email': email,
-                'first_name': first_name,
-                'last_name': last_name,
-                'external_id': external_id,
-                'password': password,
-                'root_admin': root_admin,
-                'language': language,
-                }
-        response = self._api_request(endpoint='application/users',
-                                     mode='POST', data=data)
-        return base.parse_response(response, detail=True)
-
-    def edit_user(self, user_id, username, email, first_name, last_name,
-                  external_id=None, password=None, root_admin=False,
-                  language='en'):
-        """Edits an existing user on the Pterodactyl panel.
-
-        The user_id is used to find the existing user.  All other parameters
-        will be updated on that user_id.
-
-        Args:
-            user_id(int): Pterodactyl User ID for the user to update.
-            username(str): Username, must be unique, required.
-            email(str): Full email, required.
-            first_name(str): User's first name, required.
-            last_name(str): User's last name, required.
-            external_id(str): User ID from external system like WHMCS.
-            password(str): Optionally specify a password.  If not specified
-                    user will receive an email to setup their password.
-            root_admin(bool): Whether the account is an admin.
-            language(str): Used to specify the default language for an account.
-        """
-        data = {'username': username,
-                'email': email,
-                'first_name': first_name,
-                'last_name': last_name,
-                'external_id': external_id,
-                'password': password,
-                'root_admin': root_admin,
-                'language': language,
-                }
-        response = self._api_request(
-            endpoint='application/users/{}'.format(user_id), mode='PATCH',
-            data=data)
-        return base.parse_response(response, detail=True)
-
-    def delete_user(self, user_id=None, external_id=None, detail=True):
-        """Deletes the specified user.
-
-        Will look up by external_id if provided.  This action cannot be
-        reversed so use with care.
-
-        Args:
-            user_id(int): Pterodactyl user ID
-            external_id(int): User ID from external system like WHMCS
-            detail(bool): If True includes created and updated timestamps.
-        """
-        if not user_id and not external_id:
-            raise BadRequestError('Must specify either user_id or external_id.')
-        if user_id and external_id:
-            raise BadRequestError('Specify either user_id or external_id, '
-                                  'not both.')
-
-        if external_id:
-            response = self._api_request(
-                endpoint='application/users/external/{}'.format(external_id))
-            user_id = response['attributes']['id']
-
-        response = self._api_request(
-            endpoint='application/users/{}'.format(user_id), mode='DELETE')
-        return base.parse_response(response, detail=detail)
+from pydactyl.api import base
+from pydactyl.api.base import PterodactylAPI
+from pydactyl.exceptions import BadRequestError
+from pydactyl.responses import PaginatedResponse
+
+
+class User(PterodactylAPI):
+    """Class for interacting with the Pterdactyl Client API."""
+
+    def list_users(self, email=None, uuid=None, username=None,
+                   external_id=None, includes=None, params=None):
+        """List all users.
+
+        Accepts optional filter parameters.  If multiple filters are specified
+        only results that match all filters will be returned.
+
+        Args:
+            email(str): Filter by email
+            uuid(str): Filter by uuid
+            username(str): Filter by username
+            external_id(int): Filter by external_id
+            includes(iter): List of includes, e.g. ('servers')
+            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
+        """
+        filters = {}
+        if email:
+            filters['filter[email]'] = email
+        if uuid:
+            filters['filter[uuid]'] = uuid
+        if username:
+            filters['filter[username]'] = username
+        if external_id:
+            filters['filter[external_id]'] = external_id
+
+        if params:
+            filters.update(params)
+        endpoint = 'application/users'
+        response = self._api_request(endpoint=endpoint,
+                                     includes=includes, params=filters)
+        return PaginatedResponse(self, endpoint, response)
+
+    def get_user_info(self, user_id=None, external_id=None, detail=True,
+                      includes=None, params=None):
+        """List detailed user information for specified user_id.
+
+        Args:
+            user_id(int): Pterodactyl user ID
+            external_id(int): User ID from external system like WHMCS
+            detail(bool): If True includes created and updated timestamps.
+            includes(iter): List of includes, e.g. ('servers')
+            params(dict): Extra parameters to pass, e.g. {'per_page': 300}
+        """
+        if not user_id and not external_id:
+            raise BadRequestError('Must specify either user_id or external_id.')
+        if user_id and external_id:
+            raise BadRequestError('Specify either user_id or external_id, '
+                                  'not both.')
+
+        if user_id:
+            endpoint = 'application/users/{}'.format(user_id)
+        else:
+            endpoint = 'application/users/external/{}'.format(external_id)
+
+        response = self._api_request(endpoint=endpoint, includes=includes,
+                                     params=params)
+        return base.parse_response(response, detail=detail)
+
+    def create_user(self, username, email, first_name, last_name,
+                    external_id=None, password=None, root_admin=False,
+                    language='en'):
+        """Creates a primary user on the Pterodactyl panel.
+
+        Args:
+            username(str): Username, must be unique, required.
+            email(str): Full email, required.
+            first_name(str): User's first name, required.
+            last_name(str): User's last name, required.
+            external_id(str): User ID from external system like WHMCS.
+            password(str): Optionally specify a password.  If not specified
+                    user will receive an email to setup their password.
+            root_admin(bool): Whether the account is an admin.
+            language(str): Used to specify the default language for an account.
+        """
+        data = {'username': username,
+                'email': email,
+                'first_name': first_name,
+                'last_name': last_name,
+                'external_id': external_id,
+                'password': password,
+                'root_admin': root_admin,
+                'language': language,
+                }
+        response = self._api_request(endpoint='application/users',
+                                     mode='POST', data=data)
+        return base.parse_response(response, detail=True)
+
+    def edit_user(self, user_id, username, email, first_name, last_name,
+                  external_id=None, password=None, root_admin=False,
+                  language='en'):
+        """Edits an existing user on the Pterodactyl panel.
+
+        The user_id is used to find the existing user.  All other parameters
+        will be updated on that user_id.
+
+        Args:
+            user_id(int): Pterodactyl User ID for the user to update.
+            username(str): Username, must be unique, required.
+            email(str): Full email, required.
+            first_name(str): User's first name, required.
+            last_name(str): User's last name, required.
+            external_id(str): User ID from external system like WHMCS.
+            password(str): Optionally specify a password.  If not specified
+                    user will receive an email to setup their password.
+            root_admin(bool): Whether the account is an admin.
+            language(str): Used to specify the default language for an account.
+        """
+        data = {'username': username,
+                'email': email,
+                'first_name': first_name,
+                'last_name': last_name,
+                'external_id': external_id,
+                'password': password,
+                'root_admin': root_admin,
+                'language': language,
+                }
+        response = self._api_request(
+            endpoint='application/users/{}'.format(user_id), mode='PATCH',
+            data=data)
+        return base.parse_response(response, detail=True)
+
+    def delete_user(self, user_id=None, external_id=None, detail=True):
+        """Deletes the specified user.
+
+        Will look up by external_id if provided.  This action cannot be
+        reversed so use with care.
+
+        Args:
+            user_id(int): Pterodactyl user ID
+            external_id(int): User ID from external system like WHMCS
+            detail(bool): If True includes created and updated timestamps.
+        """
+        if not user_id and not external_id:
+            raise BadRequestError('Must specify either user_id or external_id.')
+        if user_id and external_id:
+            raise BadRequestError('Specify either user_id or external_id, '
+                                  'not both.')
+
+        if external_id:
+            response = self._api_request(
+                endpoint='application/users/external/{}'.format(external_id))
+            user_id = response['attributes']['id']
+
+        response = self._api_request(
+            endpoint='application/users/{}'.format(user_id), mode='DELETE')
+        return base.parse_response(response, detail=detail)
```

### Comparing `py-dactyl-2.0.1/pydactyl/api_client.py` & `py-dactyl-2.0.2/pydactyl/api_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-import logging
-import requests
-
-from pydactyl.api.client.client_api import ClientAPI
-from pydactyl.api.locations import Locations
-from pydactyl.api.nests import Nests
-from pydactyl.api.nodes import Nodes
-from pydactyl.api.servers import Servers
-from pydactyl.api.user import User
-from pydactyl.exceptions import ClientConfigError
-
-
-def http_adapter(backoff_factor, retries, extra_retry_codes):
-    """Configures an HTTP adapter with retries and backoff."""
-    retry_codes = [429] + extra_retry_codes
-    retries = requests.packages.urllib3.util.retry.Retry(
-        total=retries, status_forcelist=retry_codes,
-        backoff_factor=backoff_factor,
-        method_whitelist=['DELETE', 'GET', 'HEAD', 'OPTIONS', 'POST', 'PUT'])
-    adapter = requests.adapters.HTTPAdapter(max_retries=retries)
-    return adapter
-
-
-def set_logger(debug):
-    """Configure debug logging if requested."""
-    if debug:
-        level = logging.DEBUG
-    else:
-        level = logging.NOTSET
-
-    logging.basicConfig()
-    logging.getLogger().setLevel(level)
-    requests_log = logging.getLogger('requests.packages.urllib3')
-    requests_log.setLevel(level)
-    requests_log.propagate = True
-
-
-class PterodactylClient(object):
-    """Provides a simplified interface to the Pterodactyl Panel API.
-
-    Instances of this class allow interaction with the Pterodactyl Panel API.
-    """
-
-    def __init__(self, url=None, api_key=None, backoff_factor=1, retries=3,
-                 extra_retry_codes=[], debug=False):
-        """Initialize a Pterodactyl class instance.
-
-        Args:
-            url(str): The base URL of the panel to connect to.
-            api_key(str): Pterodactyl Panel API key.
-            backoff_factor(int): urllib3 retry backoff_factor
-            retries(int): maximum number of retries per call
-            extra_retry_codes(iter): list of additional integer HTTP status
-                    codes to retry on, e.g. [502, 504]
-            debug(bool): enable debug logging for requests
-        """
-        if not url:
-            raise ClientConfigError(
-                'You must specify the hostname of a Pterodactyl instance.')
-
-        if not api_key:
-            raise ClientConfigError(
-                'You must specify a Pterodactyl API key to authenticate.')
-
-        self._api_key = api_key
-        self._url = url
-
-        self._session = requests.Session()
-        adapter = http_adapter(backoff_factor=backoff_factor,
-                               retries=retries,
-                               extra_retry_codes=extra_retry_codes)
-        self._session.mount('https://', adapter)
-        self._session.mount('http://', adapter)
-
-        set_logger(debug)
-
-        self._client = None
-        self._locations = None
-        self._nests = None
-        self._nodes = None
-        self._servers = None
-        self._user = None
-
-    @property
-    def client(self):
-        self._client = ClientAPI(self._url, self._api_key, self._session)
-        return self._client
-
-    @property
-    def locations(self):
-        self._locations = Locations(self._url, self._api_key, self._session)
-        return self._locations
-
-    @property
-    def nests(self):
-        self._nests = Nests(self._url, self._api_key, self._session)
-        return self._nests
-
-    @property
-    def nodes(self):
-        self._nodes = Nodes(self._url, self._api_key, self._session)
-        return self._nodes
-
-    @property
-    def servers(self):
-        self._servers = Servers(self._url, self._api_key, self._session)
-        return self._servers
-
-    @property
-    def user(self):
-        self._user = User(self._url, self._api_key, self._session)
-        return self._user
+import logging
+import requests
+
+from pydactyl.api.client.client_api import ClientAPI
+from pydactyl.api.locations import Locations
+from pydactyl.api.nests import Nests
+from pydactyl.api.nodes import Nodes
+from pydactyl.api.servers import Servers
+from pydactyl.api.user import User
+from pydactyl.exceptions import ClientConfigError
+
+
+def http_adapter(backoff_factor, retries, extra_retry_codes):
+    """Configures an HTTP adapter with retries and backoff."""
+    retry_codes = [429] + extra_retry_codes
+    retries = requests.adapters.Retry(
+        total=retries, status_forcelist=retry_codes,
+        backoff_factor=backoff_factor,
+        allowed_methods=['DELETE', 'GET', 'HEAD', 'OPTIONS', 'POST', 'PUT'])
+    adapter = requests.adapters.HTTPAdapter(max_retries=retries)
+    return adapter
+
+
+def set_logger(debug):
+    """Configure debug logging if requested."""
+    if debug:
+        level = logging.DEBUG
+    else:
+        level = logging.NOTSET
+
+    logging.basicConfig()
+    logging.getLogger().setLevel(level)
+    requests_log = logging.getLogger('requests.packages.urllib3')
+    requests_log.setLevel(level)
+    requests_log.propagate = True
+
+
+class PterodactylClient(object):
+    """Provides a simplified interface to the Pterodactyl Panel API.
+
+    Instances of this class allow interaction with the Pterodactyl Panel API.
+    """
+
+    def __init__(self, url=None, api_key=None, backoff_factor=1, retries=3,
+                 extra_retry_codes=[], debug=False):
+        """Initialize a Pterodactyl class instance.
+
+        Args:
+            url(str): The base URL of the panel to connect to.
+            api_key(str): Pterodactyl Panel API key.
+            backoff_factor(int): urllib3 retry backoff_factor
+            retries(int): maximum number of retries per call
+            extra_retry_codes(iter): list of additional integer HTTP status
+                    codes to retry on, e.g. [502, 504]
+            debug(bool): enable debug logging for requests
+        """
+        if not url:
+            raise ClientConfigError(
+                'You must specify the hostname of a Pterodactyl instance.')
+
+        if not api_key:
+            raise ClientConfigError(
+                'You must specify a Pterodactyl API key to authenticate.')
+
+        self._api_key = api_key
+        self._url = url
+
+        self._session = requests.Session()
+        adapter = http_adapter(backoff_factor=backoff_factor,
+                               retries=retries,
+                               extra_retry_codes=extra_retry_codes)
+        self._session.mount('https://', adapter)
+        self._session.mount('http://', adapter)
+
+        set_logger(debug)
+
+        self._client = None
+        self._locations = None
+        self._nests = None
+        self._nodes = None
+        self._servers = None
+        self._user = None
+
+    @property
+    def client(self):
+        self._client = ClientAPI(self._url, self._api_key, self._session)
+        return self._client
+
+    @property
+    def locations(self):
+        self._locations = Locations(self._url, self._api_key, self._session)
+        return self._locations
+
+    @property
+    def nests(self):
+        self._nests = Nests(self._url, self._api_key, self._session)
+        return self._nests
+
+    @property
+    def nodes(self):
+        self._nodes = Nodes(self._url, self._api_key, self._session)
+        return self._nodes
+
+    @property
+    def servers(self):
+        self._servers = Servers(self._url, self._api_key, self._session)
+        return self._servers
+
+    @property
+    def user(self):
+        self._user = User(self._url, self._api_key, self._session)
+        return self._user
```

### Comparing `py-dactyl-2.0.1/pydactyl/responses.py` & `py-dactyl-2.0.2/pydactyl/responses.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-"""Classes used for creating responses."""
-
-
-class PaginatedResponse(object):
-    """An iterable API response that returns paginated results."""
-
-    def __init__(self, client, endpoint, data):
-        self._client = client
-        self.data = data['data']
-        self.endpoint = endpoint
-        self.meta = data['meta']
-
-    def __getitem__(self, item):
-        if isinstance(item, int):
-            return self.data[item]
-        if hasattr(self, item):
-            return getattr(self, item, None)
-        raise KeyError(item)
-
-    def __iter__(self):
-        if hasattr(self, '_iteration'):
-            return iter(self.data)
-        else:
-            self._iteration = 0
-            return self
-
-    def __next__(self):
-        """"Retrieves the next page of results.
-
-        Returns:
-            object: An instance of PaginatedResponse
-
-        Raises:
-            PterodactylApiError: If the API request fails
-            StopIteration: When the next page does not exist.
-        """
-        self._iteration += 1
-        if self._iteration == 1:
-            # PaginatedResponses are initialized with the first page of results
-            return self
-        if self._next_page_exists(self.meta):
-            params = {'page': self._iteration}
-            response = self._client._api_request(endpoint=self.endpoint,
-                                                 params=params)
-            self.data = response['data']
-            self.meta = response['meta']
-            return self
-        else:
-            raise StopIteration
-
-    def __str__(self):
-        return '{}'.format(self.data)
-
-    def get(self, key, default=None):
-        """Retrieves a key from the paginated response.
-
-        Returns:
-            Value for the specified key
-        """
-        return getattr(self, key, default)
-
-    def collect(self):
-        """Collect all results from all pages.
-
-        Returns:
-            iter: Combined responses from all pages
-        """
-        collected = []
-        for page in self:
-            collected.extend(page.data)
-        return collected
-
-    def get_next_page_link(self):
-        """Get a link to the next page.
-
-        Returns:
-            str: Link provided by API
-        """
-        return self.meta['pagination']['links'].get('next')
-
-    def get_previous_page_link(self):
-        """Get a link to the previous page.
-
-        Returns:
-            str: Link provided by API
-        """
-        return self.meta['pagination']['links'].get('previous')
-
-    @staticmethod
-    def _next_page_exists(data):
-        """Determine if the response contains a valid link to the next page.
-
-        Returns:
-            bool: True if next page exists.
-        """
-        exists = ('pagination' in data
-                  and 'links' in data['pagination']
-                  and 'next' in data['pagination']['links']
-                  and data['pagination']['links']['next'] != '')
-        return exists
+"""Classes used for creating responses."""
+
+
+class PaginatedResponse(object):
+    """An iterable API response that returns paginated results."""
+
+    def __init__(self, client, endpoint, data):
+        self._client = client
+        self.data = data['data']
+        self.endpoint = endpoint
+        self.meta = data['meta']
+
+    def __getitem__(self, item):
+        if isinstance(item, int):
+            return self.data[item]
+        if hasattr(self, item):
+            return getattr(self, item, None)
+        raise KeyError(item)
+
+    def __iter__(self):
+        if hasattr(self, '_iteration'):
+            return iter(self.data)
+        else:
+            self._iteration = 0
+            return self
+
+    def __next__(self):
+        """"Retrieves the next page of results.
+
+        Returns:
+            object: An instance of PaginatedResponse
+
+        Raises:
+            PterodactylApiError: If the API request fails
+            StopIteration: When the next page does not exist.
+        """
+        self._iteration += 1
+        if self._iteration == 1:
+            # PaginatedResponses are initialized with the first page of results
+            return self
+        if self._next_page_exists(self.meta):
+            params = {'page': self._iteration}
+            response = self._client._api_request(endpoint=self.endpoint,
+                                                 params=params)
+            self.data = response['data']
+            self.meta = response['meta']
+            return self
+        else:
+            raise StopIteration
+
+    def __str__(self):
+        return '{}'.format(self.data)
+
+    def get(self, key, default=None):
+        """Retrieves a key from the paginated response.
+
+        Returns:
+            Value for the specified key
+        """
+        return getattr(self, key, default)
+
+    def collect(self):
+        """Collect all results from all pages.
+
+        Returns:
+            iter: Combined responses from all pages
+        """
+        collected = []
+        for page in self:
+            collected.extend(page.data)
+        return collected
+
+    def get_next_page_link(self):
+        """Get a link to the next page.
+
+        Returns:
+            str: Link provided by API
+        """
+        return self.meta['pagination']['links'].get('next')
+
+    def get_previous_page_link(self):
+        """Get a link to the previous page.
+
+        Returns:
+            str: Link provided by API
+        """
+        return self.meta['pagination']['links'].get('previous')
+
+    @staticmethod
+    def _next_page_exists(data):
+        """Determine if the response contains a valid link to the next page.
+
+        Returns:
+            bool: True if next page exists.
+        """
+        exists = ('pagination' in data
+                  and 'links' in data['pagination']
+                  and 'next' in data['pagination']['links']
+                  and data['pagination']['links']['next'] != '')
+        return exists
```

### Comparing `py-dactyl-2.0.1/setup.py` & `py-dactyl-2.0.2/setup.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import os
-import re
-import sys
-
-import setuptools
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-with open("pydactyl/constants.py") as fh:
-    VERSION = re.search('__version__ = \'([^\']+)\'', fh.read()).group(1)
-
-# 'setup.py publish' shortcut.
-if sys.argv[-1] == 'publish':
-    os.system('python setup.py sdist bdist_wheel')
-    os.system('twine upload dist/*')
-    sys.exit()
-
-
-setuptools.setup(
-    name="py-dactyl",
-    version=VERSION,
-    author="Ryan Kubiak",
-    author_email="iamkubi@gmail.com",
-    description="An easy to use Python wrapper for the Pterodactyl Panel API.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/iamkubi/pydactyl",
-    packages=setuptools.find_packages(),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Natural Language :: English",
-        "Operating System :: OS Independent",
-    ],
-    python_requires='>=3.4',
-    install_requires=[
-        "requests >=2.21.0",
-    ],
-    tests_require=[
-        "pytest >=3",
-        "pytest-cov",
-    ],
-    project_urls={
-        "Documentation": "https://pydactyl.readthedocs.io/",
-        "Source": "https://github.com/iamkubi/pydactyl",
-    }
-)
+import os
+import re
+import sys
+
+import setuptools
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+with open("pydactyl/constants.py") as fh:
+    VERSION = re.search('__version__ = \'([^\']+)\'', fh.read()).group(1)
+
+# 'setup.py publish' shortcut.
+if sys.argv[-1] == 'publish':
+    os.system('python setup.py sdist bdist_wheel')
+    os.system('twine upload dist/*')
+    sys.exit()
+
+
+setuptools.setup(
+    name="py-dactyl",
+    version=VERSION,
+    author="Ryan Kubiak",
+    author_email="iamkubi@gmail.com",
+    description="An easy to use Python wrapper for the Pterodactyl Panel API.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/iamkubi/pydactyl",
+    packages=setuptools.find_packages(),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
+        "Operating System :: OS Independent",
+    ],
+    python_requires='>=3.4',
+    install_requires=[
+        "requests >=2.21.0",
+    ],
+    tests_require=[
+        "pytest >=3",
+        "pytest-cov",
+    ],
+    project_urls={
+        "Documentation": "https://pydactyl.readthedocs.io/",
+        "Source": "https://github.com/iamkubi/pydactyl",
+    }
+)
```

### Comparing `py-dactyl-2.0.1/tests/application/locations_test.py` & `py-dactyl-2.0.2/tests/application/nests_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,89 @@
-from unittest import main, mock, TestCase
-
-from pydactyl import PterodactylClient
-from pydactyl.exceptions import BadRequestError
-
-
-class LocationsTests(TestCase):
-
-    def setUp(self):
-        self.client = PterodactylClient(url='dummy', api_key='dummy')
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_list_locations(self, mock_api):
-        expected = {
-            'endpoint': 'application/locations',
-            'includes': None,
-            'params': None,
-        }
-        self.client.locations.list_locations()
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_get_location_info(self, mock_api):
-        expected = {
-            'endpoint': 'application/locations/11',
-            'includes': None,
-            'params': None,
-        }
-        self.client.locations.get_location_info(11)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_create_location(self, mock_api):
-        expected = {
-            'endpoint': 'application/locations',
-            'mode': 'POST',
-            'data': {'shortcode': 'eu.ams.1-2_3',
-                     'description': 'Test Location'},
-        }
-        self.client.locations.create_location('eu.ams.1-2_3', 'Test Location')
-        mock_api.assert_called_with(**expected)
-
-    def test_edit_location_invalid_arguments(self):
-        with self.assertRaises(BadRequestError):
-            self.client.locations.edit_location(5)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_edit_location(self, mock_api):
-        expected = {
-            'endpoint': 'application/locations/33',
-            'mode': 'PATCH',
-            'data': {'shortcode': 'us.nyc.lvl3',
-                     'description': 'Level3 NYC Server'},
-        }
-        self.client.locations.edit_location(33, shortcode='us.nyc.lvl3',
-                                            description='Level3 NYC Server')
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_delete_location(self, mock_api):
-        expected = {
-            'endpoint': 'application/locations/44',
-            'mode': 'DELETE',
-        }
-        self.client.locations.delete_location(44)
-        mock_api.assert_called_with(**expected)
-
-
-if __name__ == '__main__':
-    main()
+from unittest import main, mock, TestCase
+
+from pydactyl import PterodactylClient
+
+
+class NestsTests(TestCase):
+
+    def setUp(self):
+        self.client = PterodactylClient(url='dummy', api_key='dummy')
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_list_nests(self, mock_api):
+        expected = {
+            'endpoint': 'application/nests',
+            'includes': None,
+            'params': None,
+        }
+        self.client.nests.list_nests()
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_list_nests_with_includes(self, mock_api):
+        expected = {
+            'endpoint': 'application/nests',
+            'includes': ['eggs', 'servers'],
+            'params': None,
+        }
+        self.client.nests.list_nests(['eggs', 'servers'])
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def get_nest_info(self, mock_api):
+        expected = {
+            'endpoint': 'application/nests/11',
+        }
+        self.client.nests.get_nest_info(11)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def get_nest_info_with_include(self, mock_api):
+        expected = {
+            'endpoint': 'application/nests/11',
+        }
+        self.client.nests.get_nest_info(11, 'config')
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_get_eggs_in_nest(self, mock_api):
+        expected = {
+            'endpoint': 'application/nests/22/eggs',
+            'includes': None,
+            'params': None,
+        }
+        self.client.nests.get_eggs_in_nest(22)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_get_eggs_in_nest_with_includes(self, mock_api):
+        expected = {
+            'endpoint': 'application/nests/22/eggs',
+            'includes': ['nest', 'config'],
+            'params': None,
+        }
+        self.client.nests.get_eggs_in_nest(22, ['nest', 'config'])
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_get_egg_info(self, mock_api):
+        expected = {
+            'endpoint': 'application/nests/33/eggs/44',
+            'includes': None,
+            'params': None,
+        }
+        self.client.nests.get_egg_info(33, 44)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_get_egg_info_with_includes(self, mock_api):
+        expected = {
+            'endpoint': 'application/nests/33/eggs/44',
+            'includes': ('servers', 'config'),
+            'params': None,
+        }
+        self.client.nests.get_egg_info(33, 44, ('servers', 'config'))
+        mock_api.assert_called_with(**expected)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `py-dactyl-2.0.1/tests/application/nodes_test.py` & `py-dactyl-2.0.2/tests/application/nodes_test.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-from unittest import main, mock, TestCase
-
-from pydactyl import PterodactylClient
-
-
-class NodesTests(TestCase):
-
-    def setUp(self):
-        self.client = PterodactylClient(url='dummy', api_key='dummy')
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_list_nodes(self, mock_api):
-        expected = {
-            'endpoint': 'application/nodes',
-            'includes': None,
-            'params': None,
-        }
-        self.client.nodes.list_nodes()
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_get_node_details(self, mock_api):
-        expected = {
-            'endpoint': 'application/nodes/11',
-            'includes': None,
-            'params': None,
-        }
-        self.client.nodes.get_node_details(11)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_get_node_config(self, mock_api):
-        expected = {
-            'endpoint': 'application/nodes/111/configuration',
-        }
-        self.client.nodes.get_node_config(111)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_create_node(self, mock_api):
-        expected_data = {
-            'name': 'Test-Name 1_2.3',
-            'description': 'foo bar',
-            'location_id': 1,
-            'fqdn': 'server1.testy.com',
-            'memory': 1024,
-            'disk': 5000,
-            'memory_overallocate': 0,
-            'disk_overallocate': 0,
-            'use_ssl': True,
-            'behind_proxy': False,
-            'daemon_base': '/srv/daemon-data',
-            'daemon_sftp': 2022,
-            'daemon_listen': 8080,
-            'upload_size': 100,
-            'public': True,
-            'maintenance_mode': False,
-        }
-
-        self.client.nodes.create_node(**expected_data)
-        del expected_data['use_ssl']
-        expected_data['scheme'] = 'https'
-
-        expected = {
-            'endpoint': 'application/nodes',
-            'mode': 'POST',
-            'data': expected_data,
-        }
-
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_edit_node(self, mock_api):
-        expected_data = {
-            'name': 'nodey node',
-            'description': 'does stuff',
-            'location_id': 33,
-            'fqdn': 'nodey.nodeynode.com',
-            'memory': 1024,
-            'disk': 5000,
-            'memory_overallocate': 0,
-            'disk_overallocate': 0,
-            'use_ssl': True,
-            'behind_proxy': False,
-            'daemon_sftp': 2022,
-            'daemon_listen': 8080,
-            'upload_size': 222,
-            'maintenance_mode': False,
-        }
-
-        self.client.nodes.edit_node(11, **expected_data)
-        del expected_data['use_ssl']
-        expected_data['scheme'] = 'https'
-
-        expected = {
-            'endpoint': 'application/nodes/11',
-            'mode': 'PATCH',
-            'data': expected_data,
-        }
-
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_list_node_allocations(self, mock_api):
-        expected = {
-            'endpoint': 'application/nodes/12/allocations',
-            'includes': None,
-            'params': None,
-        }
-        self.client.nodes.list_node_allocations(12)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_create_allocation_single(self, mock_api):
-        expected = {
-            'endpoint': 'application/nodes/13/allocations',
-            'mode': 'POST',
-            'data': {'ip': '10.2.3.4', 'alias': '1.2.3.4', 'ports': ['5000']},
-            'json': False,
-        }
-        self.client.nodes.create_allocations(13, '10.2.3.4', ['5000'],
-                                             '1.2.3.4')
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_create_allocation_multiple(self, mock_api):
-        expected = {
-            'endpoint': 'application/nodes/14/allocations',
-            'mode': 'POST',
-            'data': {'ip': '10.2.3.4', 'alias': '1.2.3.4', 'ports': ['5000',
-                                                                     '5005']},
-            'json': False,
-        }
-        self.client.nodes.create_allocations(14, '10.2.3.4', ['5000', '5005'],
-                                             '1.2.3.4')
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_create_allocation_without_alias(self, mock_api):
-        expected = {
-            'endpoint': 'application/nodes/15/allocations',
-            'mode': 'POST',
-            'data': {'ip': '1.2.3.4', 'ports': ['5001']},
-            'json': False,
-        }
-        self.client.nodes.create_allocations(
-            15, '1.2.3.4', ['5001'])
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_delete_allocation(self, mock_api):
-        expected = {
-            'endpoint': 'application/nodes/16/allocations/123',
-            'mode': 'DELETE',
-            'json': False,
-        }
-        self.client.nodes.delete_allocation(16, 123)
-        mock_api.assert_called_with(**expected)
-
-
-if __name__ == '__main__':
-    main()
+from unittest import main, mock, TestCase
+
+from pydactyl import PterodactylClient
+
+
+class NodesTests(TestCase):
+
+    def setUp(self):
+        self.client = PterodactylClient(url='dummy', api_key='dummy')
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_list_nodes(self, mock_api):
+        expected = {
+            'endpoint': 'application/nodes',
+            'includes': None,
+            'params': None,
+        }
+        self.client.nodes.list_nodes()
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_get_node_details(self, mock_api):
+        expected = {
+            'endpoint': 'application/nodes/11',
+            'includes': None,
+            'params': None,
+        }
+        self.client.nodes.get_node_details(11)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_get_node_config(self, mock_api):
+        expected = {
+            'endpoint': 'application/nodes/111/configuration',
+        }
+        self.client.nodes.get_node_config(111)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_create_node(self, mock_api):
+        expected_data = {
+            'name': 'Test-Name 1_2.3',
+            'description': 'foo bar',
+            'location_id': 1,
+            'fqdn': 'server1.testy.com',
+            'memory': 1024,
+            'disk': 5000,
+            'memory_overallocate': 0,
+            'disk_overallocate': 0,
+            'use_ssl': True,
+            'behind_proxy': False,
+            'daemon_base': '/srv/daemon-data',
+            'daemon_sftp': 2022,
+            'daemon_listen': 8080,
+            'upload_size': 100,
+            'public': True,
+            'maintenance_mode': False,
+        }
+
+        self.client.nodes.create_node(**expected_data)
+        del expected_data['use_ssl']
+        expected_data['scheme'] = 'https'
+
+        expected = {
+            'endpoint': 'application/nodes',
+            'mode': 'POST',
+            'data': expected_data,
+        }
+
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_edit_node(self, mock_api):
+        expected_data = {
+            'name': 'nodey node',
+            'description': 'does stuff',
+            'location_id': 33,
+            'fqdn': 'nodey.nodeynode.com',
+            'memory': 1024,
+            'disk': 5000,
+            'memory_overallocate': 0,
+            'disk_overallocate': 0,
+            'use_ssl': True,
+            'behind_proxy': False,
+            'daemon_sftp': 2022,
+            'daemon_listen': 8080,
+            'upload_size': 222,
+            'maintenance_mode': False,
+        }
+
+        self.client.nodes.edit_node(11, **expected_data)
+        del expected_data['use_ssl']
+        expected_data['scheme'] = 'https'
+
+        expected = {
+            'endpoint': 'application/nodes/11',
+            'mode': 'PATCH',
+            'data': expected_data,
+        }
+
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_list_node_allocations(self, mock_api):
+        expected = {
+            'endpoint': 'application/nodes/12/allocations',
+            'includes': None,
+            'params': None,
+        }
+        self.client.nodes.list_node_allocations(12)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_create_allocation_single(self, mock_api):
+        expected = {
+            'endpoint': 'application/nodes/13/allocations',
+            'mode': 'POST',
+            'data': {'ip': '10.2.3.4', 'alias': '1.2.3.4', 'ports': ['5000']},
+            'json': False,
+        }
+        self.client.nodes.create_allocations(13, '10.2.3.4', ['5000'],
+                                             '1.2.3.4')
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_create_allocation_multiple(self, mock_api):
+        expected = {
+            'endpoint': 'application/nodes/14/allocations',
+            'mode': 'POST',
+            'data': {'ip': '10.2.3.4', 'alias': '1.2.3.4', 'ports': ['5000',
+                                                                     '5005']},
+            'json': False,
+        }
+        self.client.nodes.create_allocations(14, '10.2.3.4', ['5000', '5005'],
+                                             '1.2.3.4')
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_create_allocation_without_alias(self, mock_api):
+        expected = {
+            'endpoint': 'application/nodes/15/allocations',
+            'mode': 'POST',
+            'data': {'ip': '1.2.3.4', 'ports': ['5001']},
+            'json': False,
+        }
+        self.client.nodes.create_allocations(
+            15, '1.2.3.4', ['5001'])
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_delete_allocation(self, mock_api):
+        expected = {
+            'endpoint': 'application/nodes/16/allocations/123',
+            'mode': 'DELETE',
+            'json': False,
+        }
+        self.client.nodes.delete_allocation(16, 123)
+        mock_api.assert_called_with(**expected)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `py-dactyl-2.0.1/tests/application/servers_test.py` & `py-dactyl-2.0.2/tests/application/servers_test.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,206 +1,206 @@
-from unittest import main, mock, TestCase
-
-from pydactyl import PterodactylClient
-from pydactyl.exceptions import BadRequestError
-
-
-class ServersTests(TestCase):
-
-    def setUp(self):
-        self.client = PterodactylClient(url='dummy', api_key='dummy')
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_list_servers(self, mock_api):
-        expected = {
-            'endpoint': 'application/servers',
-            'includes': None,
-            'params': None,
-        }
-        self.client.servers.list_servers()
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_get_server_info_by_external_id(self, mock_api):
-        expected = {
-            'endpoint': 'application/servers/external/11',
-            'includes': None,
-            'params': None,
-        }
-        self.client.servers.get_server_info(external_id=11)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_get_server_info_by_server_id(self, mock_api):
-        expected = {
-            'endpoint': 'application/servers/22',
-            'includes': None,
-            'params': None,
-        }
-        self.client.servers.get_server_info(server_id=22)
-        mock_api.assert_called_with(**expected)
-
-    def test_get_server_info_raises_with_no_id(self):
-        with self.assertRaises(BadRequestError):
-            self.client.servers.get_server_info()
-
-    def test_get_server_info_raises_with_both_ids(self):
-        with self.assertRaises(BadRequestError):
-            self.client.servers.get_server_info(server_id=1, external_id=2)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_suspend_server(self, mock_api):
-        expected = {
-            'endpoint': 'application/servers/33/suspend',
-            'mode': 'POST',
-        }
-        self.client.servers.suspend_server(server_id=33)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_unsuspend_server(self, mock_api):
-        expected = {
-            'endpoint': 'application/servers/44/unsuspend',
-            'mode': 'POST',
-        }
-        self.client.servers.unsuspend_server(server_id=44)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_reinstall_server(self, mock_api):
-        expected = {
-            'endpoint': 'application/servers/55/reinstall',
-            'mode': 'POST',
-        }
-        self.client.servers.reinstall_server(server_id=55)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_rebuild_server(self, mock_api):
-        expected = {
-            'endpoint': 'application/servers/66/rebuild',
-            'mode': 'POST',
-        }
-        self.client.servers.rebuild_server(server_id=66)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_delete_server(self, mock_api):
-        expected = {
-            'endpoint': 'application/servers/77',
-            'mode': 'DELETE',
-        }
-        self.client.servers.delete_server(server_id=77)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_force_delete_server(self, mock_api):
-        expected = {
-            'endpoint': 'application/servers/88/force',
-            'mode': 'DELETE',
-        }
-        self.client.servers.delete_server(server_id=88, force=True)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_list_server_databases(self, mock_api):
-        expected = {
-            'endpoint': 'application/servers/99/databases',
-            'includes': None,
-            'params': None,
-        }
-        self.client.servers.list_server_databases(server_id=99)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_get_server_database_info(self, mock_api):
-        expected = {
-            'endpoint': 'application/servers/111/databases/5',
-            'includes': None,
-            'params': None,
-        }
-        self.client.servers.get_server_database_info(server_id=111,
-                                                     database_id=5)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_create_server_database(self, mock_api):
-        expected = {
-            'endpoint': 'application/servers/222/databases',
-            'mode': 'POST',
-        }
-        self.client.servers.create_server_database(server_id=222)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_delete_server_database(self, mock_api):
-        expected = {
-            'endpoint': 'application/servers/333/databases/6',
-            'mode': 'DELETE',
-        }
-        self.client.servers.delete_server_database(server_id=333, database_id=6)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_reset_server_database_password(self, mock_api):
-        expected = {
-            'endpoint': 'application/servers/333/databases/6/reset-password',
-            'mode': 'POST',
-        }
-        self.client.servers.reset_server_database_password(server_id=333,
-                                                           database_id=6)
-        mock_api.assert_called_with(**expected)
-
-    def test_create_server_without_allocation_or_location_raises(self):
-        with self.assertRaisesRegex(BadRequestError, 'default_allocation'):
-            self.client.servers.create_server('test server', 1, 1, 1, 0, 0, 0)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_create_server_with_location(self, mock_api):
-        self.client.servers.create_server('test server', 1, 2, 3, 4, 5, 6,
-                                          location_ids=[7])
-        mock_api.assert_called()
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_create_server_with_allocation(self, mock_api):
-        self.client.servers.create_server('test server', 1, 2, 3, 4, 5, 6,
-                                          default_allocation=1234)
-        mock_api.assert_called()
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_update_server_build(self, mock_api):
-        expected = {
-            'endpoint': 'application/servers/42/build',
-            'mode': 'PATCH',
-            'data': {'allocation': 88,
-                     'limits': {'memory': 1024, 'swap': 1, 'disk': 5000,
-                                'cpu': 150, 'io': 500},
-                     'feature_limits': {'databases': 3, 'allocations': 9,
-                                        'backups': 2},
-                     'add_allocations': 89,
-                     'remove_allocations': 88,
-                     'oom_disabled': True,
-                     },
-            'json': False,
-        }
-        self.client.servers.update_server_build(
-            server_id=42, allocation_id=88, memory_limit=1024, swap_limit=1,
-            disk_limit=5000, cpu_limit=150, io_limit=500, database_limit=3,
-            allocation_limit=9, backup_limit=2, add_allocations=89,
-            remove_allocations=88, oom_disabled=True)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_update_server_startup(self, mock_api):
-        expected = {
-            'endpoint': 'application/servers/11/startup',
-            'mode': 'PATCH',
-            'data': {'egg': 19, 'startup': 'startup.sh', 'image':
-                'ghcr.io/image:tag', 'skip_scripts': False, 'environment': {}},
-            'json': False}
-        self.client.servers.update_server_startup(
-            server_id=11, egg_id=19, docker_image='ghcr.io/image:tag',
-            startup_cmd='startup.sh', skip_scripts=False)
-        mock_api.assert_called_with(**expected)
-
-if __name__ == '__main__':
-    main()
+from unittest import main, mock, TestCase
+
+from pydactyl import PterodactylClient
+from pydactyl.exceptions import BadRequestError
+
+
+class ServersTests(TestCase):
+
+    def setUp(self):
+        self.client = PterodactylClient(url='dummy', api_key='dummy')
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_list_servers(self, mock_api):
+        expected = {
+            'endpoint': 'application/servers',
+            'includes': None,
+            'params': None,
+        }
+        self.client.servers.list_servers()
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_get_server_info_by_external_id(self, mock_api):
+        expected = {
+            'endpoint': 'application/servers/external/11',
+            'includes': None,
+            'params': None,
+        }
+        self.client.servers.get_server_info(external_id=11)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_get_server_info_by_server_id(self, mock_api):
+        expected = {
+            'endpoint': 'application/servers/22',
+            'includes': None,
+            'params': None,
+        }
+        self.client.servers.get_server_info(server_id=22)
+        mock_api.assert_called_with(**expected)
+
+    def test_get_server_info_raises_with_no_id(self):
+        with self.assertRaises(BadRequestError):
+            self.client.servers.get_server_info()
+
+    def test_get_server_info_raises_with_both_ids(self):
+        with self.assertRaises(BadRequestError):
+            self.client.servers.get_server_info(server_id=1, external_id=2)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_suspend_server(self, mock_api):
+        expected = {
+            'endpoint': 'application/servers/33/suspend',
+            'mode': 'POST',
+        }
+        self.client.servers.suspend_server(server_id=33)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_unsuspend_server(self, mock_api):
+        expected = {
+            'endpoint': 'application/servers/44/unsuspend',
+            'mode': 'POST',
+        }
+        self.client.servers.unsuspend_server(server_id=44)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_reinstall_server(self, mock_api):
+        expected = {
+            'endpoint': 'application/servers/55/reinstall',
+            'mode': 'POST',
+        }
+        self.client.servers.reinstall_server(server_id=55)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_rebuild_server(self, mock_api):
+        expected = {
+            'endpoint': 'application/servers/66/rebuild',
+            'mode': 'POST',
+        }
+        self.client.servers.rebuild_server(server_id=66)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_delete_server(self, mock_api):
+        expected = {
+            'endpoint': 'application/servers/77',
+            'mode': 'DELETE',
+        }
+        self.client.servers.delete_server(server_id=77)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_force_delete_server(self, mock_api):
+        expected = {
+            'endpoint': 'application/servers/88/force',
+            'mode': 'DELETE',
+        }
+        self.client.servers.delete_server(server_id=88, force=True)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_list_server_databases(self, mock_api):
+        expected = {
+            'endpoint': 'application/servers/99/databases',
+            'includes': None,
+            'params': None,
+        }
+        self.client.servers.list_server_databases(server_id=99)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_get_server_database_info(self, mock_api):
+        expected = {
+            'endpoint': 'application/servers/111/databases/5',
+            'includes': None,
+            'params': None,
+        }
+        self.client.servers.get_server_database_info(server_id=111,
+                                                     database_id=5)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_create_server_database(self, mock_api):
+        expected = {
+            'endpoint': 'application/servers/222/databases',
+            'mode': 'POST',
+        }
+        self.client.servers.create_server_database(server_id=222)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_delete_server_database(self, mock_api):
+        expected = {
+            'endpoint': 'application/servers/333/databases/6',
+            'mode': 'DELETE',
+        }
+        self.client.servers.delete_server_database(server_id=333, database_id=6)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_reset_server_database_password(self, mock_api):
+        expected = {
+            'endpoint': 'application/servers/333/databases/6/reset-password',
+            'mode': 'POST',
+        }
+        self.client.servers.reset_server_database_password(server_id=333,
+                                                           database_id=6)
+        mock_api.assert_called_with(**expected)
+
+    def test_create_server_without_allocation_or_location_raises(self):
+        with self.assertRaisesRegex(BadRequestError, 'default_allocation'):
+            self.client.servers.create_server('test server', 1, 1, 1, 0, 0, 0)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_create_server_with_location(self, mock_api):
+        self.client.servers.create_server('test server', 1, 2, 3, 4, 5, 6,
+                                          location_ids=[7])
+        mock_api.assert_called()
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_create_server_with_allocation(self, mock_api):
+        self.client.servers.create_server('test server', 1, 2, 3, 4, 5, 6,
+                                          default_allocation=1234)
+        mock_api.assert_called()
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_update_server_build(self, mock_api):
+        expected = {
+            'endpoint': 'application/servers/42/build',
+            'mode': 'PATCH',
+            'data': {'allocation': 88,
+                     'limits': {'memory': 1024, 'swap': 1, 'disk': 5000,
+                                'cpu': 150, 'io': 500},
+                     'feature_limits': {'databases': 3, 'allocations': 9,
+                                        'backups': 2},
+                     'add_allocations': 89,
+                     'remove_allocations': 88,
+                     'oom_disabled': True,
+                     },
+            'json': False,
+        }
+        self.client.servers.update_server_build(
+            server_id=42, allocation_id=88, memory_limit=1024, swap_limit=1,
+            disk_limit=5000, cpu_limit=150, io_limit=500, database_limit=3,
+            allocation_limit=9, backup_limit=2, add_allocations=89,
+            remove_allocations=88, oom_disabled=True)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_update_server_startup(self, mock_api):
+        expected = {
+            'endpoint': 'application/servers/11/startup',
+            'mode': 'PATCH',
+            'data': {'egg': 19, 'startup': 'startup.sh', 'image':
+                'ghcr.io/image:tag', 'skip_scripts': False, 'environment': {}},
+            'json': False}
+        self.client.servers.update_server_startup(
+            server_id=11, egg_id=19, docker_image='ghcr.io/image:tag',
+            startup_cmd='startup.sh', skip_scripts=False)
+        mock_api.assert_called_with(**expected)
+
+if __name__ == '__main__':
+    main()
```

### Comparing `py-dactyl-2.0.1/tests/application/user_test.py` & `py-dactyl-2.0.2/tests/application/user_test.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-from unittest import main, mock, TestCase
-
-from pydactyl import PterodactylClient
-from pydactyl.exceptions import BadRequestError
-
-
-class UserTests(TestCase):
-
-    def setUp(self):
-        self.client = PterodactylClient(url='dummy', api_key='dummy')
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_list_users(self, mock_api):
-        expected = {
-            'endpoint': 'application/users',
-            'includes': None,
-            'params': {},
-        }
-        self.client.user.list_users()
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_list_users_with_filter(self, mock_api):
-        expected = {
-            'endpoint': 'application/users',
-            'includes': None,
-            'params': {'filter[email]': 'best@test.com'}
-        }
-        self.client.user.list_users(email='best@test.com')
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_list_users_with_multiple_filter_params(self, mock_api):
-        expected = {
-            'endpoint': 'application/users',
-            'includes': None,
-            'params': {'filter[email]': 'best@test.com',
-                       'filter[uuid]': 2,
-                       'filter[username]': 'best',
-                       'filter[external_id]': 4}
-        }
-        self.client.user.list_users(email='best@test.com', uuid=2,
-                                    username='best', external_id=4)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_list_users_with_multiple_filter_params_and_includes(
-            self, mock_api):
-        expected = {
-            'endpoint': 'application/users',
-            'params': {'filter[email]': 'best@test.com',
-                       'filter[username]': 'best',
-                       'per_page': 300},
-            'includes': ['servers', 'databases']
-        }
-        self.client.user.list_users(
-            email='best@test.com', username='best', params={'per_page': 300},
-            includes=['servers', 'databases'])
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_list_users_with_one_param_no_filters(
-            self, mock_api):
-        expected = {
-            'endpoint': 'application/users',
-            'includes': None,
-            'params': {'per_page': 300},
-        }
-        self.client.user.list_users(params={'per_page': 300})
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_get_user_info_by_external_id(self, mock_api):
-        expected = {
-            'endpoint': 'application/users/external/11',
-            'includes': None,
-            'params': None,
-        }
-        self.client.user.get_user_info(external_id=11)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_get_user_info_by_user_id(self, mock_api):
-        expected = {
-            'endpoint': 'application/users/22',
-            'includes': None,
-            'params': None,
-        }
-        self.client.user.get_user_info(user_id=22)
-        mock_api.assert_called_with(**expected)
-
-    def test_get_user_info_raises_with_no_id(self):
-        with self.assertRaises(BadRequestError):
-            self.client.user.get_user_info()
-
-    def test_get_user_info_raises_with_both_ids(self):
-        with self.assertRaises(BadRequestError):
-            self.client.user.get_user_info(user_id=1, external_id=2)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_delete_user_with_user_id(self, mock_api):
-        expected = {
-            'endpoint': 'application/users/77',
-            'mode': 'DELETE',
-        }
-        self.client.user.delete_user(user_id=77)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_delete_user_with_external_id(self, mock_api):
-        mock_api.return_value = {'attributes': {'id': 88}}
-        expected = [mock.call(endpoint='application/users/external/11'),
-                    mock.call(endpoint='application/users/88', mode='DELETE')]
-        self.client.user.delete_user(external_id=11)
-        mock_api.assert_has_calls(expected)
-
-    def test_delete_user_raises_with_no_id(self):
-        with self.assertRaises(BadRequestError):
-            self.client.user.delete_user()
-
-    def test_delete_user_raises_with_both_ids(self):
-        with self.assertRaises(BadRequestError):
-            self.client.user.delete_user(user_id=1, external_id=2)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_create_user(self, mock_api):
-        expected = {
-            'endpoint': 'application/users',
-            'mode': 'POST',
-            'data': {'username': 'best', 'email': 'best@test.com',
-                     'first_name': 'first', 'last_name': 'last',
-                     'external_id': 42,
-                     'password': 'hunter2', 'root_admin': True, 'language': 'en'
-             },
-        }
-        self.client.user.create_user(
-            username='best', email='best@test.com', first_name='first',
-            last_name='last', external_id=42, password='hunter2',
-            root_admin=True, language='en')
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_edit_user(self, mock_api):
-        expected = {
-            'endpoint': 'application/users/11',
-            'mode': 'PATCH',
-            'data': {'username': 'best', 'email': 'best@test.com',
-                     'first_name': 'first', 'last_name': 'last',
-                     'external_id': 43,
-                     'password': 'hunter2', 'root_admin': False, 'language':
-                         'en'
-             },
-        }
-        self.client.user.edit_user(
-            user_id=11, username='best', email='best@test.com',
-            first_name='first', last_name='last', external_id=43,
-            password='hunter2', root_admin=False, language='en')
-        mock_api.assert_called_with(**expected)
-
-
-if __name__ == '__main__':
-    main()
+from unittest import main, mock, TestCase
+
+from pydactyl import PterodactylClient
+from pydactyl.exceptions import BadRequestError
+
+
+class UserTests(TestCase):
+
+    def setUp(self):
+        self.client = PterodactylClient(url='dummy', api_key='dummy')
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_list_users(self, mock_api):
+        expected = {
+            'endpoint': 'application/users',
+            'includes': None,
+            'params': {},
+        }
+        self.client.user.list_users()
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_list_users_with_filter(self, mock_api):
+        expected = {
+            'endpoint': 'application/users',
+            'includes': None,
+            'params': {'filter[email]': 'best@test.com'}
+        }
+        self.client.user.list_users(email='best@test.com')
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_list_users_with_multiple_filter_params(self, mock_api):
+        expected = {
+            'endpoint': 'application/users',
+            'includes': None,
+            'params': {'filter[email]': 'best@test.com',
+                       'filter[uuid]': 2,
+                       'filter[username]': 'best',
+                       'filter[external_id]': 4}
+        }
+        self.client.user.list_users(email='best@test.com', uuid=2,
+                                    username='best', external_id=4)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_list_users_with_multiple_filter_params_and_includes(
+            self, mock_api):
+        expected = {
+            'endpoint': 'application/users',
+            'params': {'filter[email]': 'best@test.com',
+                       'filter[username]': 'best',
+                       'per_page': 300},
+            'includes': ['servers', 'databases']
+        }
+        self.client.user.list_users(
+            email='best@test.com', username='best', params={'per_page': 300},
+            includes=['servers', 'databases'])
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_list_users_with_one_param_no_filters(
+            self, mock_api):
+        expected = {
+            'endpoint': 'application/users',
+            'includes': None,
+            'params': {'per_page': 300},
+        }
+        self.client.user.list_users(params={'per_page': 300})
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_get_user_info_by_external_id(self, mock_api):
+        expected = {
+            'endpoint': 'application/users/external/11',
+            'includes': None,
+            'params': None,
+        }
+        self.client.user.get_user_info(external_id=11)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_get_user_info_by_user_id(self, mock_api):
+        expected = {
+            'endpoint': 'application/users/22',
+            'includes': None,
+            'params': None,
+        }
+        self.client.user.get_user_info(user_id=22)
+        mock_api.assert_called_with(**expected)
+
+    def test_get_user_info_raises_with_no_id(self):
+        with self.assertRaises(BadRequestError):
+            self.client.user.get_user_info()
+
+    def test_get_user_info_raises_with_both_ids(self):
+        with self.assertRaises(BadRequestError):
+            self.client.user.get_user_info(user_id=1, external_id=2)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_delete_user_with_user_id(self, mock_api):
+        expected = {
+            'endpoint': 'application/users/77',
+            'mode': 'DELETE',
+        }
+        self.client.user.delete_user(user_id=77)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_delete_user_with_external_id(self, mock_api):
+        mock_api.return_value = {'attributes': {'id': 88}}
+        expected = [mock.call(endpoint='application/users/external/11'),
+                    mock.call(endpoint='application/users/88', mode='DELETE')]
+        self.client.user.delete_user(external_id=11)
+        mock_api.assert_has_calls(expected)
+
+    def test_delete_user_raises_with_no_id(self):
+        with self.assertRaises(BadRequestError):
+            self.client.user.delete_user()
+
+    def test_delete_user_raises_with_both_ids(self):
+        with self.assertRaises(BadRequestError):
+            self.client.user.delete_user(user_id=1, external_id=2)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_create_user(self, mock_api):
+        expected = {
+            'endpoint': 'application/users',
+            'mode': 'POST',
+            'data': {'username': 'best', 'email': 'best@test.com',
+                     'first_name': 'first', 'last_name': 'last',
+                     'external_id': 42,
+                     'password': 'hunter2', 'root_admin': True, 'language': 'en'
+             },
+        }
+        self.client.user.create_user(
+            username='best', email='best@test.com', first_name='first',
+            last_name='last', external_id=42, password='hunter2',
+            root_admin=True, language='en')
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_edit_user(self, mock_api):
+        expected = {
+            'endpoint': 'application/users/11',
+            'mode': 'PATCH',
+            'data': {'username': 'best', 'email': 'best@test.com',
+                     'first_name': 'first', 'last_name': 'last',
+                     'external_id': 43,
+                     'password': 'hunter2', 'root_admin': False, 'language':
+                         'en'
+             },
+        }
+        self.client.user.edit_user(
+            user_id=11, username='best', email='best@test.com',
+            first_name='first', last_name='last', external_id=43,
+            password='hunter2', root_admin=False, language='en')
+        mock_api.assert_called_with(**expected)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `py-dactyl-2.0.1/tests/base/api_client_test.py` & `py-dactyl-2.0.2/tests/base/api_client_test.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import logging
-import unittest
-
-from pydactyl.exceptions import ClientConfigError
-from pydactyl import api_client
-
-
-class ApiClientTests(unittest.TestCase):
-
-    def test_pterodactyl_client_raises_without_required_params(self):
-        with self.assertRaises(ClientConfigError):
-            api_client.PterodactylClient(api_key='key', url=None)
-        with self.assertRaises(ClientConfigError):
-            api_client.PterodactylClient(api_key=None, url='url')
-
-    def test_pterodactyl_client_debug_param(self):
-        requests_log = logging.getLogger('requests.packages.urllib3')
-        self.assertEqual(logging.NOTSET, requests_log.level)
-        api_client.PterodactylClient('foo', 'bar', debug=True)
-        self.assertEqual(logging.DEBUG, requests_log.level)
-        api_client.PterodactylClient('foo', 'bar', debug=False)
-        self.assertEqual(logging.NOTSET, requests_log.level)
+import logging
+import unittest
+
+from pydactyl.exceptions import ClientConfigError
+from pydactyl import api_client
+
+
+class ApiClientTests(unittest.TestCase):
+
+    def test_pterodactyl_client_raises_without_required_params(self):
+        with self.assertRaises(ClientConfigError):
+            api_client.PterodactylClient(api_key='key', url=None)
+        with self.assertRaises(ClientConfigError):
+            api_client.PterodactylClient(api_key=None, url='url')
+
+    def test_pterodactyl_client_debug_param(self):
+        requests_log = logging.getLogger('requests.packages.urllib3')
+        self.assertEqual(logging.NOTSET, requests_log.level)
+        api_client.PterodactylClient('foo', 'bar', debug=True)
+        self.assertEqual(logging.DEBUG, requests_log.level)
+        api_client.PterodactylClient('foo', 'bar', debug=False)
+        self.assertEqual(logging.NOTSET, requests_log.level)
```

### Comparing `py-dactyl-2.0.1/tests/base/base_test.py` & `py-dactyl-2.0.2/tests/base/base_test.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,195 +1,195 @@
-import unittest
-from unittest import mock
-
-from requests import Session
-
-from pydactyl.api import base
-from pydactyl.exceptions import BadRequestError
-
-
-class BaseTests(unittest.TestCase):
-
-    def setUp(self):
-        self.api = base.PterodactylAPI(url='https://dummy.com',
-                                       api_key='dummy_key')
-
-    def test_init(self):
-        self.assertEqual('dummy_key', self.api._api_key)
-        self.assertEqual('https://dummy.com', self.api._url)
-
-    def test_get_headers(self):
-        expected = {
-            'Authorization': 'Bearer dummy_key',
-            'Accept': 'application/json',
-            'Content-Type': 'application/json',
-        }
-        self.assertDictEqual(expected, self.api._get_headers())
-
-    def test_url_join(self):
-        self.assertEqual('www.test.com/path', base.url_join(
-            'www.test.com', 'path'))
-        self.assertEqual('test.com/path/to/thing',
-                         base.url_join('test.com', 'path', 'to', 'thing'))
-        self.assertEqual('https://asdf.com/api/other/things',
-                         base.url_join('https://asdf.com', '/api/',
-                                       'other/things'))
-
-    def test_parse_response_with_detail(self):
-        expected = {'object': 'server', 'attributes': {'id': 12}}
-        self.assertEqual(expected, base.parse_response(expected, detail=True))
-
-    def test_parse_response_without_detail(self):
-        expected = {'id': 12}
-        response = {'object': 'server', 'attributes': {'id': 12}}
-        self.assertEqual(expected, base.parse_response(response, detail=False))
-
-    def test_parse_response_list_object_with_detail(self):
-        expected = {'object': 'list',
-                    'data': [{'object': 'server', 'attributes': {'id': 5}},
-                             {'object': 'server', 'attributes': {'id': 6}}]}
-        self.assertEqual(expected, base.parse_response(expected, detail=True))
-
-    def test_parse_response_list_object_without_detail(self):
-        expected = [{'id': 5}, {'id': 6}]
-        response = {'object': 'list',
-                    'data': [{'object': 'server', 'attributes': {'id': 5}},
-                             {'object': 'server', 'attributes': {'id': 6}}]}
-        self.assertEqual(expected, base.parse_response(response, detail=False))
-
-    @mock.patch.object(Session, 'get')
-    def test_valid_api_get_request(self, mock_request):
-        expected = {
-            'params': None,
-            'headers': self.api._get_headers(),
-        }
-        self.api._api_request(endpoint='nomorecoffee')
-        mock_request.assert_called_with('https://dummy.com/api/nomorecoffee',
-                                        **expected)
-
-    @mock.patch.object(Session, 'post')
-    def test_valid_api_post_request(self, mock_request):
-        data = {'test': 'data'}
-        expected = {
-            'params': None,
-            'headers': self.api._get_headers(),
-        }
-        self.api._api_request(endpoint='foo', mode='POST', data=data)
-        mock_request.assert_called_with('https://dummy.com/api/foo', json=data,
-                                        **expected)
-
-    @mock.patch.object(Session, 'post')
-    def test_valid_api_post_request_with_raw_data(self, mock_request):
-        data = {'test': 'data'}
-        expected = {
-            'params': None,
-            'headers': self.api._get_headers(),
-        }
-        self.api._api_request(endpoint='foo', mode='POST', data=data,
-                              data_as_json=False)
-        mock_request.assert_called_with('https://dummy.com/api/foo', data=data,
-                                        **expected)
-
-    @mock.patch.object(Session, 'patch')
-    def test_valid_api_patch_request(self, mock_request):
-        data = {'patch': 'me'}
-        expected = {
-            'params': None,
-            'headers': self.api._get_headers(),
-            'json': data,
-        }
-        self.api._api_request(endpoint='bar', mode='PATCH', data=data)
-        mock_request.assert_called_with('https://dummy.com/api/bar', **expected)
-
-    @mock.patch.object(Session, 'delete')
-    def test_valid_api_delete_request(self, mock_request):
-        expected = {
-            'params': None,
-            'headers': self.api._get_headers(),
-        }
-        self.api._api_request(endpoint='havecoffee', mode='DELETE')
-        mock_request.assert_called_with('https://dummy.com/api/havecoffee',
-                                        **expected)
-
-    @mock.patch.object(Session, 'put')
-    def test_valid_api_put_request(self, mock_request):
-        data = {'put': 'me'}
-        expected = {
-            'params': None,
-            'headers': self.api._get_headers(),
-            'json': data,
-        }
-        self.api._api_request(endpoint='putstuff', mode='PUT', data=data)
-        mock_request.assert_called_with('https://dummy.com/api/putstuff',
-                                        **expected)
-
-    @mock.patch.object(Session, 'post')
-    def test_api_request_with_override_headers(self, mock_request):
-        data = {'dummy': 'asdf'}
-        expected_headers = self.api._get_headers()
-        expected_headers['Content-Type'] = 'application/text'
-        expected = {
-            'params': None,
-            'headers': expected_headers,
-            'json': data,
-        }
-        self.api._api_request(
-            endpoint='overridetest', mode='POST', data=data,
-            override_headers={'Content-Type': 'application/text'})
-        mock_request.assert_called_with('https://dummy.com/api/overridetest',
-                                        **expected)
-
-    @mock.patch.object(Session, 'get')
-    def test_api_request_with_includes(self, mock_request):
-        expected = {
-            'params': {'include': 'allocations,users,servers'},
-            'headers': self.api._get_headers(),
-        }
-        self.api._api_request(endpoint='includetest', mode='GET', includes=(
-            'allocations', 'users', 'servers'))
-        mock_request.assert_called_with('https://dummy.com/api/includetest',
-                                        **expected)
-
-    @mock.patch.object(Session, 'get')
-    def test_api_request_with_params(self, mock_request):
-        expected = {
-            'params': {'per_page': 300},
-            'headers': self.api._get_headers(),
-        }
-        self.api._api_request(endpoint='includetest', mode='GET', params={
-            'per_page': 300})
-        mock_request.assert_called_with('https://dummy.com/api/includetest',
-                                        **expected)
-
-    @mock.patch.object(Session, 'get')
-    def test_api_request_with_includes_and_params(self, mock_request):
-        expected = {
-            'params': {'include': 'allocations,users,servers', 'per_page': 300},
-            'headers': self.api._get_headers(),
-        }
-        self.api._api_request(endpoint='inptest', mode='GET', includes=(
-            'allocations', 'users', 'servers'), params={'per_page': 300})
-        mock_request.assert_called_with('https://dummy.com/api/inptest',
-                                        **expected)
-
-    @mock.patch.object(Session, 'post')
-    def test_api_request_with_includes_and_params_and_include_param(
-            self, mock_request):
-        expected = {
-            'params': {'include': 'questionablethings,users,asdf',
-                       'per_page': 300},
-            'headers': self.api._get_headers(),
-            'json': None,
-        }
-        self.api._api_request(
-            endpoint='inptest', mode='POST', includes=('users', 'asdf'),
-            params={'per_page': 300, 'include': 'questionablethings'})
-        mock_request.assert_called_with('https://dummy.com/api/inptest',
-                                        **expected)
-
-    def test_api_request_raises_without_endpoint(self):
-        with self.assertRaises(BadRequestError):
-            self.api._api_request(endpoint=None)
-
-    def test_api_request_raises_with_bad_mode(self):
-        with self.assertRaises(BadRequestError):
-            self.api._api_request(endpoint='any', mode='NOPE')
+import unittest
+from unittest import mock
+
+from requests import Session
+
+from pydactyl.api import base
+from pydactyl.exceptions import BadRequestError
+
+
+class BaseTests(unittest.TestCase):
+
+    def setUp(self):
+        self.api = base.PterodactylAPI(url='https://dummy.com',
+                                       api_key='dummy_key')
+
+    def test_init(self):
+        self.assertEqual('dummy_key', self.api._api_key)
+        self.assertEqual('https://dummy.com', self.api._url)
+
+    def test_get_headers(self):
+        expected = {
+            'Authorization': 'Bearer dummy_key',
+            'Accept': 'application/json',
+            'Content-Type': 'application/json',
+        }
+        self.assertDictEqual(expected, self.api._get_headers())
+
+    def test_url_join(self):
+        self.assertEqual('www.test.com/path', base.url_join(
+            'www.test.com', 'path'))
+        self.assertEqual('test.com/path/to/thing',
+                         base.url_join('test.com', 'path', 'to', 'thing'))
+        self.assertEqual('https://asdf.com/api/other/things',
+                         base.url_join('https://asdf.com', '/api/',
+                                       'other/things'))
+
+    def test_parse_response_with_detail(self):
+        expected = {'object': 'server', 'attributes': {'id': 12}}
+        self.assertEqual(expected, base.parse_response(expected, detail=True))
+
+    def test_parse_response_without_detail(self):
+        expected = {'id': 12}
+        response = {'object': 'server', 'attributes': {'id': 12}}
+        self.assertEqual(expected, base.parse_response(response, detail=False))
+
+    def test_parse_response_list_object_with_detail(self):
+        expected = {'object': 'list',
+                    'data': [{'object': 'server', 'attributes': {'id': 5}},
+                             {'object': 'server', 'attributes': {'id': 6}}]}
+        self.assertEqual(expected, base.parse_response(expected, detail=True))
+
+    def test_parse_response_list_object_without_detail(self):
+        expected = [{'id': 5}, {'id': 6}]
+        response = {'object': 'list',
+                    'data': [{'object': 'server', 'attributes': {'id': 5}},
+                             {'object': 'server', 'attributes': {'id': 6}}]}
+        self.assertEqual(expected, base.parse_response(response, detail=False))
+
+    @mock.patch.object(Session, 'get')
+    def test_valid_api_get_request(self, mock_request):
+        expected = {
+            'params': None,
+            'headers': self.api._get_headers(),
+        }
+        self.api._api_request(endpoint='nomorecoffee')
+        mock_request.assert_called_with('https://dummy.com/api/nomorecoffee',
+                                        **expected)
+
+    @mock.patch.object(Session, 'post')
+    def test_valid_api_post_request(self, mock_request):
+        data = {'test': 'data'}
+        expected = {
+            'params': None,
+            'headers': self.api._get_headers(),
+        }
+        self.api._api_request(endpoint='foo', mode='POST', data=data)
+        mock_request.assert_called_with('https://dummy.com/api/foo', json=data,
+                                        **expected)
+
+    @mock.patch.object(Session, 'post')
+    def test_valid_api_post_request_with_raw_data(self, mock_request):
+        data = {'test': 'data'}
+        expected = {
+            'params': None,
+            'headers': self.api._get_headers(),
+        }
+        self.api._api_request(endpoint='foo', mode='POST', data=data,
+                              data_as_json=False)
+        mock_request.assert_called_with('https://dummy.com/api/foo', data=data,
+                                        **expected)
+
+    @mock.patch.object(Session, 'patch')
+    def test_valid_api_patch_request(self, mock_request):
+        data = {'patch': 'me'}
+        expected = {
+            'params': None,
+            'headers': self.api._get_headers(),
+            'json': data,
+        }
+        self.api._api_request(endpoint='bar', mode='PATCH', data=data)
+        mock_request.assert_called_with('https://dummy.com/api/bar', **expected)
+
+    @mock.patch.object(Session, 'delete')
+    def test_valid_api_delete_request(self, mock_request):
+        expected = {
+            'params': None,
+            'headers': self.api._get_headers(),
+        }
+        self.api._api_request(endpoint='havecoffee', mode='DELETE')
+        mock_request.assert_called_with('https://dummy.com/api/havecoffee',
+                                        **expected)
+
+    @mock.patch.object(Session, 'put')
+    def test_valid_api_put_request(self, mock_request):
+        data = {'put': 'me'}
+        expected = {
+            'params': None,
+            'headers': self.api._get_headers(),
+            'json': data,
+        }
+        self.api._api_request(endpoint='putstuff', mode='PUT', data=data)
+        mock_request.assert_called_with('https://dummy.com/api/putstuff',
+                                        **expected)
+
+    @mock.patch.object(Session, 'post')
+    def test_api_request_with_override_headers(self, mock_request):
+        data = {'dummy': 'asdf'}
+        expected_headers = self.api._get_headers()
+        expected_headers['Content-Type'] = 'application/text'
+        expected = {
+            'params': None,
+            'headers': expected_headers,
+            'json': data,
+        }
+        self.api._api_request(
+            endpoint='overridetest', mode='POST', data=data,
+            override_headers={'Content-Type': 'application/text'})
+        mock_request.assert_called_with('https://dummy.com/api/overridetest',
+                                        **expected)
+
+    @mock.patch.object(Session, 'get')
+    def test_api_request_with_includes(self, mock_request):
+        expected = {
+            'params': {'include': 'allocations,users,servers'},
+            'headers': self.api._get_headers(),
+        }
+        self.api._api_request(endpoint='includetest', mode='GET', includes=(
+            'allocations', 'users', 'servers'))
+        mock_request.assert_called_with('https://dummy.com/api/includetest',
+                                        **expected)
+
+    @mock.patch.object(Session, 'get')
+    def test_api_request_with_params(self, mock_request):
+        expected = {
+            'params': {'per_page': 300},
+            'headers': self.api._get_headers(),
+        }
+        self.api._api_request(endpoint='includetest', mode='GET', params={
+            'per_page': 300})
+        mock_request.assert_called_with('https://dummy.com/api/includetest',
+                                        **expected)
+
+    @mock.patch.object(Session, 'get')
+    def test_api_request_with_includes_and_params(self, mock_request):
+        expected = {
+            'params': {'include': 'allocations,users,servers', 'per_page': 300},
+            'headers': self.api._get_headers(),
+        }
+        self.api._api_request(endpoint='inptest', mode='GET', includes=(
+            'allocations', 'users', 'servers'), params={'per_page': 300})
+        mock_request.assert_called_with('https://dummy.com/api/inptest',
+                                        **expected)
+
+    @mock.patch.object(Session, 'post')
+    def test_api_request_with_includes_and_params_and_include_param(
+            self, mock_request):
+        expected = {
+            'params': {'include': 'questionablethings,users,asdf',
+                       'per_page': 300},
+            'headers': self.api._get_headers(),
+            'json': None,
+        }
+        self.api._api_request(
+            endpoint='inptest', mode='POST', includes=('users', 'asdf'),
+            params={'per_page': 300, 'include': 'questionablethings'})
+        mock_request.assert_called_with('https://dummy.com/api/inptest',
+                                        **expected)
+
+    def test_api_request_raises_without_endpoint(self):
+        with self.assertRaises(BadRequestError):
+            self.api._api_request(endpoint=None)
+
+    def test_api_request_raises_with_bad_mode(self):
+        with self.assertRaises(BadRequestError):
+            self.api._api_request(endpoint='any', mode='NOPE')
```

### Comparing `py-dactyl-2.0.1/tests/base/responses_test.py` & `py-dactyl-2.0.2/tests/base/responses_test.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-import unittest
-from copy import deepcopy
-from unittest import mock
-
-from pydactyl import PterodactylClient
-from pydactyl.responses import PaginatedResponse
-
-TEST_META = {
-    'pagination':
-        {'total': 106, 'count': 25, 'per_page': 25, 'current_page': 1,
-         'total_pages': 5, 'links': {
-            'next': 'https://panel.mydomain.com/api/application/nodes/1'
-                    '/allocations?page=3',
-            'previous': 'https://panel.mydomain.com/api/application/nodes/1'
-                        '/allocations?page=1'}}}
-TEST_DATA = {'data': [{'dummy': 'data1'}, {'dummy': 'data2'}], 'meta':
-    TEST_META}
-
-MULTIPAGE_TEST_DATA = [
-    {'data': ['thing1', 'thing2', 'sometimespage1isweird'], 'meta': TEST_META},
-    {'data': ['thing3', 'thing4'], 'meta': TEST_META},
-    {'data': ['thing84', 'thing97', 'fdas', 'pepperoni'], 'meta': TEST_META},
-    {'data': ['one', 'two', 'three', 4, 5, '6'], 'meta': TEST_META},
-    {'data': ['pineappleisanacceptablepizzatopping'], 'meta': TEST_META},
-]
-
-
-class PaginatedResponseTests(unittest.TestCase):
-
-    def setUp(self):
-        self.client = PterodactylClient(url='dummy', api_key='dummy')
-
-    def test_paginated_response_init(self):
-        response = PaginatedResponse(self.client, 'anyendpoint', TEST_DATA)
-
-        self.assertEqual(response[0]['dummy'], 'data1')
-        self.assertEqual(response[1]['dummy'], 'data2')
-
-    def test_paginated_response_get(self):
-        response = PaginatedResponse(self.client, 'anyendpoint', TEST_DATA)
-        self.assertEqual(response.get('meta'), TEST_META)
-
-    def test_paginated_response_get_nonexistant_item(self):
-        response = PaginatedResponse(self.client, 'anyendpoint', TEST_DATA)
-        self.assertEqual(response.get('fountainofyouth'), None)
-
-    def test_paginated_response_get_with_default(self):
-        response = PaginatedResponse(self.client, 'anyendpoint', TEST_DATA)
-        self.assertEqual(response.get('badname', 'test_default'),
-                         'test_default')
-
-    def test_paginated_response_get_next_page_link(self):
-        response = PaginatedResponse(self.client, 'anyendpoint', TEST_DATA)
-        self.assertEqual(
-            response.get_next_page_link(),
-            'https://panel.mydomain.com/api/application/nodes/1/allocations'
-            '?page=3')
-
-    def test_paginated_response_get_previous_page_link(self):
-        response = PaginatedResponse(self.client, 'anyendpoint', TEST_DATA)
-        self.assertEqual(
-            response.get_previous_page_link(),
-            'https://panel.mydomain.com/api/application/nodes/1/allocations'
-            '?page=1')
-
-    def test_paginated_response_next_page_exists(self):
-        self.assertTrue(PaginatedResponse._next_page_exists(TEST_META))
-
-    def test_paginated_response_next_page_does_not_exist(self):
-        data = deepcopy(TEST_META)
-        self.assertTrue(PaginatedResponse._next_page_exists(data))
-        del data['pagination']['links']['next']
-        self.assertFalse(PaginatedResponse._next_page_exists(data))
-
-    def test_paginated_response_fetches_first_page(self):
-        expected = {
-            'endpoint': 'api/asdf',
-            'params': {'page': 2},
-        }
-        self.client._api_request = mock.MagicMock()
-        response = PaginatedResponse(self.client, 'api/asdf', TEST_DATA)
-        for _ in response:
-            continue
-
-        self.client._api_request.assert_called_with(**expected)
-
-    def test_paginated_response_data_property_returns_data(self):
-        response = PaginatedResponse(self.client, 'anyendpoint', TEST_DATA)
-        self.assertEqual(response.data, TEST_DATA['data'])
-
-    def test_paginated_response_str_method(self):
-        response = PaginatedResponse(self.client, 'anyendpoint', TEST_DATA)
-        self.assertEqual(str(response), str(TEST_DATA['data']))
-
-    def test_paginated_response_collect_method(self):
-        self.client._api_request = mock.MagicMock()
-        self.client._api_request.side_effect = MULTIPAGE_TEST_DATA[1:]
-        response = PaginatedResponse(self.client, 'asdf',
-                                     MULTIPAGE_TEST_DATA[0])
-        self.assertListEqual(
-            response.collect(),
-            [item for data in MULTIPAGE_TEST_DATA for item in data['data']])
-
-    def test_paginated_response_multipage_iterator(self):
-        self.client._api_request = mock.MagicMock()
-        self.client._api_request.side_effect = MULTIPAGE_TEST_DATA[1:]
-        response = PaginatedResponse(self.client, 'asdf',
-                                     MULTIPAGE_TEST_DATA[0])
-        expected = [item for data in MULTIPAGE_TEST_DATA for item in
-                    data['data']]
-        self.assertListEqual(expected,
-                             [item for page in response for item in page])
-
-    def test_paginated_response_has_correct_number_of_items(self):
-        self.client._api_request = mock.MagicMock()
-        self.client._api_request.side_effect = MULTIPAGE_TEST_DATA[1:]
-        response = PaginatedResponse(self.client, 'asdf',
-                                     MULTIPAGE_TEST_DATA[0])
-        expected = [item for data in MULTIPAGE_TEST_DATA for item in
-                    data['data']]
-        expected_count = 16
-        self.assertEqual(expected_count, len(expected))
-        self.assertEqual(expected_count, len(response.collect()))
+import unittest
+from copy import deepcopy
+from unittest import mock
+
+from pydactyl import PterodactylClient
+from pydactyl.responses import PaginatedResponse
+
+TEST_META = {
+    'pagination':
+        {'total': 106, 'count': 25, 'per_page': 25, 'current_page': 1,
+         'total_pages': 5, 'links': {
+            'next': 'https://panel.mydomain.com/api/application/nodes/1'
+                    '/allocations?page=3',
+            'previous': 'https://panel.mydomain.com/api/application/nodes/1'
+                        '/allocations?page=1'}}}
+TEST_DATA = {'data': [{'dummy': 'data1'}, {'dummy': 'data2'}], 'meta':
+    TEST_META}
+
+MULTIPAGE_TEST_DATA = [
+    {'data': ['thing1', 'thing2', 'sometimespage1isweird'], 'meta': TEST_META},
+    {'data': ['thing3', 'thing4'], 'meta': TEST_META},
+    {'data': ['thing84', 'thing97', 'fdas', 'pepperoni'], 'meta': TEST_META},
+    {'data': ['one', 'two', 'three', 4, 5, '6'], 'meta': TEST_META},
+    {'data': ['pineappleisanacceptablepizzatopping'], 'meta': TEST_META},
+]
+
+
+class PaginatedResponseTests(unittest.TestCase):
+
+    def setUp(self):
+        self.client = PterodactylClient(url='dummy', api_key='dummy')
+
+    def test_paginated_response_init(self):
+        response = PaginatedResponse(self.client, 'anyendpoint', TEST_DATA)
+
+        self.assertEqual(response[0]['dummy'], 'data1')
+        self.assertEqual(response[1]['dummy'], 'data2')
+
+    def test_paginated_response_get(self):
+        response = PaginatedResponse(self.client, 'anyendpoint', TEST_DATA)
+        self.assertEqual(response.get('meta'), TEST_META)
+
+    def test_paginated_response_get_nonexistant_item(self):
+        response = PaginatedResponse(self.client, 'anyendpoint', TEST_DATA)
+        self.assertEqual(response.get('fountainofyouth'), None)
+
+    def test_paginated_response_get_with_default(self):
+        response = PaginatedResponse(self.client, 'anyendpoint', TEST_DATA)
+        self.assertEqual(response.get('badname', 'test_default'),
+                         'test_default')
+
+    def test_paginated_response_get_next_page_link(self):
+        response = PaginatedResponse(self.client, 'anyendpoint', TEST_DATA)
+        self.assertEqual(
+            response.get_next_page_link(),
+            'https://panel.mydomain.com/api/application/nodes/1/allocations'
+            '?page=3')
+
+    def test_paginated_response_get_previous_page_link(self):
+        response = PaginatedResponse(self.client, 'anyendpoint', TEST_DATA)
+        self.assertEqual(
+            response.get_previous_page_link(),
+            'https://panel.mydomain.com/api/application/nodes/1/allocations'
+            '?page=1')
+
+    def test_paginated_response_next_page_exists(self):
+        self.assertTrue(PaginatedResponse._next_page_exists(TEST_META))
+
+    def test_paginated_response_next_page_does_not_exist(self):
+        data = deepcopy(TEST_META)
+        self.assertTrue(PaginatedResponse._next_page_exists(data))
+        del data['pagination']['links']['next']
+        self.assertFalse(PaginatedResponse._next_page_exists(data))
+
+    def test_paginated_response_fetches_first_page(self):
+        expected = {
+            'endpoint': 'api/asdf',
+            'params': {'page': 2},
+        }
+        self.client._api_request = mock.MagicMock()
+        response = PaginatedResponse(self.client, 'api/asdf', TEST_DATA)
+        for _ in response:
+            continue
+
+        self.client._api_request.assert_called_with(**expected)
+
+    def test_paginated_response_data_property_returns_data(self):
+        response = PaginatedResponse(self.client, 'anyendpoint', TEST_DATA)
+        self.assertEqual(response.data, TEST_DATA['data'])
+
+    def test_paginated_response_str_method(self):
+        response = PaginatedResponse(self.client, 'anyendpoint', TEST_DATA)
+        self.assertEqual(str(response), str(TEST_DATA['data']))
+
+    def test_paginated_response_collect_method(self):
+        self.client._api_request = mock.MagicMock()
+        self.client._api_request.side_effect = MULTIPAGE_TEST_DATA[1:]
+        response = PaginatedResponse(self.client, 'asdf',
+                                     MULTIPAGE_TEST_DATA[0])
+        self.assertListEqual(
+            response.collect(),
+            [item for data in MULTIPAGE_TEST_DATA for item in data['data']])
+
+    def test_paginated_response_multipage_iterator(self):
+        self.client._api_request = mock.MagicMock()
+        self.client._api_request.side_effect = MULTIPAGE_TEST_DATA[1:]
+        response = PaginatedResponse(self.client, 'asdf',
+                                     MULTIPAGE_TEST_DATA[0])
+        expected = [item for data in MULTIPAGE_TEST_DATA for item in
+                    data['data']]
+        self.assertListEqual(expected,
+                             [item for page in response for item in page])
+
+    def test_paginated_response_has_correct_number_of_items(self):
+        self.client._api_request = mock.MagicMock()
+        self.client._api_request.side_effect = MULTIPAGE_TEST_DATA[1:]
+        response = PaginatedResponse(self.client, 'asdf',
+                                     MULTIPAGE_TEST_DATA[0])
+        expected = [item for data in MULTIPAGE_TEST_DATA for item in
+                    data['data']]
+        expected_count = 16
+        self.assertEqual(expected_count, len(expected))
+        self.assertEqual(expected_count, len(response.collect()))
```

### Comparing `py-dactyl-2.0.1/tests/client/account_test.py` & `py-dactyl-2.0.2/tests/client/account_test.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-import unittest
-from unittest import mock
-
-from pydactyl import PterodactylClient
-
-
-class AccountTests(unittest.TestCase):
-
-    def setUp(self):
-        self.api = PterodactylClient(url='dummy', api_key='dummy')
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_get_account(self, mock_api):
-        expected = {
-            'endpoint': 'client/account',
-        }
-        self.api.client.account.get_account()
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_get_2fa_setup_code(self, mock_api):
-        expected = {
-            'endpoint': 'client/account/two-factor',
-        }
-        self.api.client.account.get_2fa_setup_code()
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_enable_2fa(self, mock_api):
-        expected = {
-            'endpoint': 'client/account/two-factor',
-            'mode': 'POST',
-            'data': {'code': '123456'},
-        }
-        self.api.client.account.enable_2fa('123456')
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_disable_2fa(self, mock_api):
-        expected = {
-            'endpoint': 'client/account/two-factor',
-            'mode': 'DELETE',
-            'data': {'password': '123456'},
-        }
-        self.api.client.account.disable_2fa('123456')
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_update_email(self, mock_api):
-        expected = {
-            'endpoint': 'client/account/email',
-            'mode': 'PUT',
-            'data': {'email': 'me@me.com', 'password': 'hunter2'},
-        }
-        self.api.client.account.update_email('me@me.com', 'hunter2')
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_update_password(self, mock_api):
-        expected = {
-            'endpoint': 'client/account/password',
-            'mode': 'PUT',
-            'data': {'current_password': 'hunter2', 'password': 'hunter3',
-                     'password_confirmation': 'hunter3'},
-        }
-        self.api.client.account.update_password('hunter2', 'hunter3', 'hunter3')
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_list_api_keys(self, mock_api):
-        expected = {
-            'endpoint': 'client/account/api-keys',
-        }
-        self.api.client.account.api_key_list()
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_create_api_key(self, mock_api):
-        expected = {
-            'endpoint': 'client/account/api-keys',
-            'mode': 'POST',
-            'data': {'description': 'Test key', 'allowed_ips': ["127.0.0.1"]},
-        }
-        self.api.client.account.api_key_create('Test key', ["127.0.0.1"])
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_delete_api_key(self, mock_api):
-        expected = {
-            'endpoint': 'client/account/api-keys/abc123',
-            'mode': 'DELETE',
-        }
-        self.api.client.account.api_key_delete('abc123')
-        mock_api.assert_called_with(**expected)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from unittest import mock
+
+from pydactyl import PterodactylClient
+
+
+class AccountTests(unittest.TestCase):
+
+    def setUp(self):
+        self.api = PterodactylClient(url='dummy', api_key='dummy')
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_get_account(self, mock_api):
+        expected = {
+            'endpoint': 'client/account',
+        }
+        self.api.client.account.get_account()
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_get_2fa_setup_code(self, mock_api):
+        expected = {
+            'endpoint': 'client/account/two-factor',
+        }
+        self.api.client.account.get_2fa_setup_code()
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_enable_2fa(self, mock_api):
+        expected = {
+            'endpoint': 'client/account/two-factor',
+            'mode': 'POST',
+            'data': {'code': '123456'},
+        }
+        self.api.client.account.enable_2fa('123456')
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_disable_2fa(self, mock_api):
+        expected = {
+            'endpoint': 'client/account/two-factor',
+            'mode': 'DELETE',
+            'data': {'password': '123456'},
+        }
+        self.api.client.account.disable_2fa('123456')
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_update_email(self, mock_api):
+        expected = {
+            'endpoint': 'client/account/email',
+            'mode': 'PUT',
+            'data': {'email': 'me@me.com', 'password': 'hunter2'},
+        }
+        self.api.client.account.update_email('me@me.com', 'hunter2')
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_update_password(self, mock_api):
+        expected = {
+            'endpoint': 'client/account/password',
+            'mode': 'PUT',
+            'data': {'current_password': 'hunter2', 'password': 'hunter3',
+                     'password_confirmation': 'hunter3'},
+        }
+        self.api.client.account.update_password('hunter2', 'hunter3', 'hunter3')
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_list_api_keys(self, mock_api):
+        expected = {
+            'endpoint': 'client/account/api-keys',
+        }
+        self.api.client.account.api_key_list()
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_create_api_key(self, mock_api):
+        expected = {
+            'endpoint': 'client/account/api-keys',
+            'mode': 'POST',
+            'data': {'description': 'Test key', 'allowed_ips': ["127.0.0.1"]},
+        }
+        self.api.client.account.api_key_create('Test key', ["127.0.0.1"])
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_delete_api_key(self, mock_api):
+        expected = {
+            'endpoint': 'client/account/api-keys/abc123',
+            'mode': 'DELETE',
+        }
+        self.api.client.account.api_key_delete('abc123')
+        mock_api.assert_called_with(**expected)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `py-dactyl-2.0.1/tests/client/databases_test.py` & `py-dactyl-2.0.2/tests/client/databases_test.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-import unittest
-from unittest import mock
-
-from pydactyl import PterodactylClient
-
-
-class DatabasesTest(unittest.TestCase):
-
-    def setUp(self):
-        self.api = PterodactylClient(url='dummy', api_key='dummy')
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_list_databases(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/fds173/databases',
-            'includes': None,
-            'params': None,
-        }
-        self.api.client.servers.databases.list_databases('fds173')
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_list_databases_with_passwords(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/fds173/databases',
-            'includes': ['password'],
-            'params': None,
-        }
-        self.api.client.servers.databases.list_databases('fds173',
-                                                         include_passwords=True)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_create_database(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/fds173/databases',
-            'mode': 'POST',
-            'data': {'database': 'testdb', 'remote': '%'},
-        }
-        self.api.client.servers.databases.create_database('fds173', 'testdb')
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_create_database_with_remote(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/fds173/databases',
-            'mode': 'POST',
-            'data': {'database': 'testdb', 'remote': '1.1.1.1'},
-        }
-        self.api.client.servers.databases.create_database('fds173', 'testdb',
-                                                          '1.1.1.1')
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_rotate_database_password(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/fds173/databases/longlong/rotate'
-                        '-password',
-            'mode': 'POST',
-        }
-        self.api.client.servers.databases.rotate_database_password('fds173',
-                                                                   'longlong')
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_delete_database(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/fds173/databases/longlong',
-            'mode': 'DELETE',
-        }
-        self.api.client.servers.databases.delete_database('fds173', 'longlong')
-        mock_api.assert_called_with(**expected)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from unittest import mock
+
+from pydactyl import PterodactylClient
+
+
+class DatabasesTest(unittest.TestCase):
+
+    def setUp(self):
+        self.api = PterodactylClient(url='dummy', api_key='dummy')
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_list_databases(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/fds173/databases',
+            'includes': None,
+            'params': None,
+        }
+        self.api.client.servers.databases.list_databases('fds173')
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_list_databases_with_passwords(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/fds173/databases',
+            'includes': ['password'],
+            'params': None,
+        }
+        self.api.client.servers.databases.list_databases('fds173',
+                                                         include_passwords=True)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_create_database(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/fds173/databases',
+            'mode': 'POST',
+            'data': {'database': 'testdb', 'remote': '%'},
+        }
+        self.api.client.servers.databases.create_database('fds173', 'testdb')
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_create_database_with_remote(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/fds173/databases',
+            'mode': 'POST',
+            'data': {'database': 'testdb', 'remote': '1.1.1.1'},
+        }
+        self.api.client.servers.databases.create_database('fds173', 'testdb',
+                                                          '1.1.1.1')
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_rotate_database_password(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/fds173/databases/longlong/rotate'
+                        '-password',
+            'mode': 'POST',
+        }
+        self.api.client.servers.databases.rotate_database_password('fds173',
+                                                                   'longlong')
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_delete_database(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/fds173/databases/longlong',
+            'mode': 'DELETE',
+        }
+        self.api.client.servers.databases.delete_database('fds173', 'longlong')
+        mock_api.assert_called_with(**expected)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `py-dactyl-2.0.1/tests/client/network_test.py` & `py-dactyl-2.0.2/tests/client/network_test.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import unittest
-from unittest import mock
-
-from pydactyl import PterodactylClient
-
-
-class NetworkTests(unittest.TestCase):
-
-    def setUp(self):
-        self.api = PterodactylClient(url='dummy', api_key='dummy')
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_list_allocations(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/notwork/network/allocations',
-        }
-        self.api.client.servers.network.list_allocations('notwork')
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_assign_allocation(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/notwork/network/allocations',
-            'mode': 'POST',
-        }
-        self.api.client.servers.network.assign_allocation('notwork')
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_set_allocation_note(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/notwork/network/allocations/2',
-            'mode': 'POST',
-            'data': {'notes': 'some note'},
-        }
-        self.api.client.servers.network.set_allocation_note('notwork', 2,
-                                                            'some note')
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_set_primary_allocation(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/notwork/network/allocations/33/primary',
-            'mode': 'POST',
-        }
-        self.api.client.servers.network.set_primary_allocation('notwork', 33)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_unassign_allocation(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/notwork/network/allocations/44',
-            'mode': 'DELETE',
-        }
-        self.api.client.servers.network.unassign_allocation('notwork', 44)
-        mock_api.assert_called_with(**expected)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from unittest import mock
+
+from pydactyl import PterodactylClient
+
+
+class NetworkTests(unittest.TestCase):
+
+    def setUp(self):
+        self.api = PterodactylClient(url='dummy', api_key='dummy')
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_list_allocations(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/notwork/network/allocations',
+        }
+        self.api.client.servers.network.list_allocations('notwork')
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_assign_allocation(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/notwork/network/allocations',
+            'mode': 'POST',
+        }
+        self.api.client.servers.network.assign_allocation('notwork')
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_set_allocation_note(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/notwork/network/allocations/2',
+            'mode': 'POST',
+            'data': {'notes': 'some note'},
+        }
+        self.api.client.servers.network.set_allocation_note('notwork', 2,
+                                                            'some note')
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_set_primary_allocation(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/notwork/network/allocations/33/primary',
+            'mode': 'POST',
+        }
+        self.api.client.servers.network.set_primary_allocation('notwork', 33)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_unassign_allocation(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/notwork/network/allocations/44',
+            'mode': 'DELETE',
+        }
+        self.api.client.servers.network.unassign_allocation('notwork', 44)
+        mock_api.assert_called_with(**expected)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `py-dactyl-2.0.1/tests/client/schedules_test.py` & `py-dactyl-2.0.2/tests/client/schedules_test.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-import unittest
-from unittest import mock
-
-from pydactyl import PterodactylClient
-
-
-class SchedulesTests(unittest.TestCase):
-
-    def setUp(self):
-        self.api = PterodactylClient(url='dummy', api_key='dummy')
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_list_schedules(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/srv123/schedules',
-        }
-        self.api.client.servers.schedules.list_schedules('srv123')
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_create_schedule(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/srv123/schedules',
-            'mode': 'POST',
-            'data': {'name': 'test', 'minute': '*', 'hour': '1',
-                     'day_of_week': 'pants', 'day_of_month': 'doggo',
-                     'month': 'may', 'only_when_online': False,
-                     'is_active': True},
-        }
-        self.api.client.servers.schedules.create_schedule(
-            'srv123', 'test', '*', '1', 'pants', 'doggo', 'may')
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_get_schedule_details(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/srv123/schedules/3',
-        }
-        self.api.client.servers.schedules.get_schedule_details('srv123', 3)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_update_schedule(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/srv123/schedules/4',
-            'mode': 'POST',
-            'data': {'name': 'test', 'minute': '*', 'hour': '1',
-                     'day_of_week': 'pants', 'day_of_month': 'doggo',
-                     'month': 'may', 'only_when_online': False,
-                     'is_active': True},
-        }
-        self.api.client.servers.schedules.update_schedule(
-            'srv123', 4, 'test', '*', '1', 'pants', 'doggo', 'may')
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_delete_schedule(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/srv123/schedules/5',
-            'mode': 'DELETE',
-        }
-        self.api.client.servers.schedules.delete_schedule('srv123', 5)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_create_task(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/srv123/schedules/5/tasks',
-            'mode': 'POST',
-            'data': {'action': 'command', 'payload': 'say Hello World',
-                     'time_offset': '6', 'continue_on_failure': False}
-        }
-        self.api.client.servers.schedules.create_task('srv123', 5, 'command',
-                                                      'say Hello World', '6')
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_update_task(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/srv123/schedules/5/tasks/4',
-            'mode': 'POST',
-            'data': {'action': 'command', 'payload': 'say Hello World',
-                     'time_offset': '6', 'continue_on_failure': True}
-        }
-        self.api.client.servers.schedules.update_task('srv123', 5, 4, 'command',
-                                                      'say Hello World', '6',
-                                                      True)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_delete_task(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/srv123/schedules/5/tasks/4',
-            'mode': 'DELETE',
-        }
-        self.api.client.servers.schedules.delete_task('srv123', 5, 4)
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_run_schedule(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/srv123/schedules/7/execute',
-            'mode': 'POST',
-        }
-        self.api.client.servers.schedules.run_schedule('srv123', 7)
-        mock_api.assert_called_with(**expected)
-        
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from unittest import mock
+
+from pydactyl import PterodactylClient
+
+
+class SchedulesTests(unittest.TestCase):
+
+    def setUp(self):
+        self.api = PterodactylClient(url='dummy', api_key='dummy')
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_list_schedules(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/srv123/schedules',
+        }
+        self.api.client.servers.schedules.list_schedules('srv123')
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_create_schedule(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/srv123/schedules',
+            'mode': 'POST',
+            'data': {'name': 'test', 'minute': '*', 'hour': '1',
+                     'day_of_week': 'pants', 'day_of_month': 'doggo',
+                     'month': 'may', 'only_when_online': False,
+                     'is_active': True},
+        }
+        self.api.client.servers.schedules.create_schedule(
+            'srv123', 'test', '*', '1', 'pants', 'doggo', 'may')
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_get_schedule_details(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/srv123/schedules/3',
+        }
+        self.api.client.servers.schedules.get_schedule_details('srv123', 3)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_update_schedule(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/srv123/schedules/4',
+            'mode': 'POST',
+            'data': {'name': 'test', 'minute': '*', 'hour': '1',
+                     'day_of_week': 'pants', 'day_of_month': 'doggo',
+                     'month': 'may', 'only_when_online': False,
+                     'is_active': True},
+        }
+        self.api.client.servers.schedules.update_schedule(
+            'srv123', 4, 'test', '*', '1', 'pants', 'doggo', 'may')
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_delete_schedule(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/srv123/schedules/5',
+            'mode': 'DELETE',
+        }
+        self.api.client.servers.schedules.delete_schedule('srv123', 5)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_create_task(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/srv123/schedules/5/tasks',
+            'mode': 'POST',
+            'data': {'action': 'command', 'payload': 'say Hello World',
+                     'time_offset': '6', 'continue_on_failure': False}
+        }
+        self.api.client.servers.schedules.create_task('srv123', 5, 'command',
+                                                      'say Hello World', '6')
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_update_task(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/srv123/schedules/5/tasks/4',
+            'mode': 'POST',
+            'data': {'action': 'command', 'payload': 'say Hello World',
+                     'time_offset': '6', 'continue_on_failure': True}
+        }
+        self.api.client.servers.schedules.update_task('srv123', 5, 4, 'command',
+                                                      'say Hello World', '6',
+                                                      True)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_delete_task(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/srv123/schedules/5/tasks/4',
+            'mode': 'DELETE',
+        }
+        self.api.client.servers.schedules.delete_task('srv123', 5, 4)
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_run_schedule(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/srv123/schedules/7/execute',
+            'mode': 'POST',
+        }
+        self.api.client.servers.schedules.run_schedule('srv123', 7)
+        mock_api.assert_called_with(**expected)
+        
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `py-dactyl-2.0.1/tests/client/startup_test.py` & `py-dactyl-2.0.2/tests/client/startup_test.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import unittest
-from unittest import mock
-
-from pydactyl import PterodactylClient
-
-
-class StartupTests(unittest.TestCase):
-
-    def setUp(self):
-        self.api = PterodactylClient(url='dummy', api_key='dummy')
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_list_variables(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/srv123/startup',
-        }
-        self.api.client.servers.startup.list_variables('srv123')
-        mock_api.assert_called_with(**expected)
-
-    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
-    def test_update_variable(self, mock_api):
-        expected = {
-            'endpoint': 'client/servers/srv123/startup/variable',
-            'mode': 'PUT',
-            'data': {'key': 'varname', 'value': 'someval'},
-        }
-        self.api.client.servers.startup.update_variable('srv123', 'varname',
-                                                        'someval')
-        mock_api.assert_called_with(**expected)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from unittest import mock
+
+from pydactyl import PterodactylClient
+
+
+class StartupTests(unittest.TestCase):
+
+    def setUp(self):
+        self.api = PterodactylClient(url='dummy', api_key='dummy')
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_list_variables(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/srv123/startup',
+        }
+        self.api.client.servers.startup.list_variables('srv123')
+        mock_api.assert_called_with(**expected)
+
+    @mock.patch('pydactyl.api.base.PterodactylAPI._api_request')
+    def test_update_variable(self, mock_api):
+        expected = {
+            'endpoint': 'client/servers/srv123/startup/variable',
+            'mode': 'PUT',
+            'data': {'key': 'varname', 'value': 'someval'},
+        }
+        self.api.client.servers.startup.update_variable('srv123', 'varname',
+                                                        'someval')
+        mock_api.assert_called_with(**expected)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

