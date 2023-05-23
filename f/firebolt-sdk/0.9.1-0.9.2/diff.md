# Comparing `tmp/firebolt_sdk-0.9.1.tar.gz` & `tmp/firebolt_sdk-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/firebolt-python-sdk/firebolt-python-sdk/dist/tmp91fx0t5k/firebolt_sdk-0.9.1.tar", last modified: Tue Jul 26 15:11:47 2022, max compression
+gzip compressed data, was "/home/runner/work/firebolt-python-sdk/firebolt-python-sdk/dist/tmptxr54geo/firebolt_sdk-0.9.2.tar", last modified: Fri Jul 29 07:55:00 2022, max compression
```

## Comparing `firebolt_sdk-0.9.1.tar` & `firebolt_sdk-0.9.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 15:11:47.000000 firebolt_sdk-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11354 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3682 2022-07-26 15:11:47.000000 firebolt_sdk-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2895 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (121)      348 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (121)     2186 2022-07-26 15:11:47.000000 firebolt_sdk-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 15:11:47.000000 firebolt_sdk-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 15:11:47.000000 firebolt_sdk-0.9.1/src/firebolt/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-26 15:11:37.000000 firebolt_sdk-0.9.1/src/firebolt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 15:11:47.000000 firebolt_sdk-0.9.1/src/firebolt/async_db/
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/async_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12210 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/async_db/_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    14458 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/async_db/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)    21359 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/async_db/cursor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1431 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/async_db/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 15:11:47.000000 firebolt_sdk-0.9.1/src/firebolt/client/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 15:11:47.000000 firebolt_sdk-0.9.1/src/firebolt/client/auth/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/client/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3618 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/client/auth/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/client/auth/token.py
--rw-r--r--   0 runner    (1001) docker     (121)     3462 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/client/auth/username_password.py
--rw-r--r--   0 runner    (1001) docker     (121)     5178 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/client/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2134 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/client/resource_manager_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 15:11:47.000000 firebolt_sdk-0.9.1/src/firebolt/common/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/common/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     2787 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/common/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/common/token_storage.py
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/common/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/common/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 15:11:47.000000 firebolt_sdk-0.9.1/src/firebolt/db/
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2405 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/db/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3346 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/db/cursor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 15:11:47.000000 firebolt_sdk-0.9.1/src/firebolt/model/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      916 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/model/binding.py
--rw-r--r--   0 runner    (1001) docker     (121)     5290 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/model/database.py
--rw-r--r--   0 runner    (1001) docker     (121)    16888 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/model/engine.py
--rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/model/engine_revision.py
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/model/instance_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/model/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/model/region.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 15:11:47.000000 firebolt_sdk-0.9.1/src/firebolt/service/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/service/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4984 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/service/binding.py
--rw-r--r--   0 runner    (1001) docker     (121)     4391 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/service/database.py
--rw-r--r--   0 runner    (1001) docker     (121)     8109 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/service/engine.py
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/service/engine_revision.py
--rw-r--r--   0 runner    (1001) docker     (121)     3742 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/service/instance_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     2781 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/service/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/service/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     2081 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/service/region.py
--rw-r--r--   0 runner    (1001) docker     (121)    10236 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/service/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 15:11:47.000000 firebolt_sdk-0.9.1/src/firebolt/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6121 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     4946 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/utils/token_storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/utils/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     5522 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/utils/usage_tracker.py
--rw-r--r--   0 runner    (1001) docker     (121)     5248 2022-07-26 15:11:28.000000 firebolt_sdk-0.9.1/src/firebolt/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 15:11:47.000000 firebolt_sdk-0.9.1/src/firebolt_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3682 2022-07-26 15:11:47.000000 firebolt_sdk-0.9.1/src/firebolt_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1823 2022-07-26 15:11:47.000000 firebolt_sdk-0.9.1/src/firebolt_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-26 15:11:47.000000 firebolt_sdk-0.9.1/src/firebolt_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-07-26 15:11:47.000000 firebolt_sdk-0.9.1/src/firebolt_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-07-26 15:11:47.000000 firebolt_sdk-0.9.1/src/firebolt_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 07:55:00.000000 firebolt_sdk-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)    11354 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3682 2022-07-29 07:55:00.000000 firebolt_sdk-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2895 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (121)      348 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2187 2022-07-29 07:55:00.000000 firebolt_sdk-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 07:55:00.000000 firebolt_sdk-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 07:55:00.000000 firebolt_sdk-0.9.2/src/firebolt/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-29 07:54:47.000000 firebolt_sdk-0.9.2/src/firebolt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 07:55:00.000000 firebolt_sdk-0.9.2/src/firebolt/async_db/
+-rw-r--r--   0 runner    (1001) docker     (121)      719 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/async_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12236 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/async_db/_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14557 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/async_db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21347 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/async_db/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/async_db/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 07:55:00.000000 firebolt_sdk-0.9.2/src/firebolt/client/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 07:55:00.000000 firebolt_sdk-0.9.2/src/firebolt/client/auth/
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/client/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3626 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/client/auth/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/client/auth/token.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3463 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/client/auth/username_password.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5181 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      339 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2134 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/client/resource_manager_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 07:55:00.000000 firebolt_sdk-0.9.2/src/firebolt/common/
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/common/exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2765 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/common/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/common/token_storage.py
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/common/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/common/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 07:55:00.000000 firebolt_sdk-0.9.2/src/firebolt/db/
+-rw-r--r--   0 runner    (1001) docker     (121)      682 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2405 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3346 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/db/cursor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 07:55:00.000000 firebolt_sdk-0.9.2/src/firebolt/model/
+-rw-r--r--   0 runner    (1001) docker     (121)      876 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      917 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/model/binding.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5290 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/model/database.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16865 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/model/engine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1638 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/model/engine_revision.py
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/model/instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/model/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)      452 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/model/region.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 07:55:00.000000 firebolt_sdk-0.9.2/src/firebolt/service/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      538 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/service/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4982 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/service/binding.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4383 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/service/database.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8086 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/service/engine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/service/engine_revision.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3741 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/service/instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2780 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/service/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)      370 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/service/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2079 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/service/region.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10219 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/service/types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 07:55:00.000000 firebolt_sdk-0.9.2/src/firebolt/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6033 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4950 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/utils/token_storage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/utils/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5522 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/utils/usage_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5255 2022-07-29 07:54:31.000000 firebolt_sdk-0.9.2/src/firebolt/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 07:55:00.000000 firebolt_sdk-0.9.2/src/firebolt_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3682 2022-07-29 07:55:00.000000 firebolt_sdk-0.9.2/src/firebolt_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1823 2022-07-29 07:55:00.000000 firebolt_sdk-0.9.2/src/firebolt_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-29 07:55:00.000000 firebolt_sdk-0.9.2/src/firebolt_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-07-29 07:55:00.000000 firebolt_sdk-0.9.2/src/firebolt_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-07-29 07:55:00.000000 firebolt_sdk-0.9.2/src/firebolt_sdk.egg-info/top_level.txt
```

### Comparing `firebolt_sdk-0.9.1/LICENSE` & `firebolt_sdk-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-0.9.1/PKG-INFO` & `firebolt_sdk-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebolt_sdk
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python SDK for Firebolt
 Home-page: https://github.com/firebolt-db/firebolt-sdk
 Author: Firebolt
 Author-email: support@firebolt.io
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/firebolt-db/firebolt-sdk/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `firebolt_sdk-0.9.1/README.md` & `firebolt_sdk-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-0.9.1/setup.cfg` & `firebolt_sdk-0.9.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 	ciso8601==2.2.0
 dev = 
 	devtools==0.7.0
 	mypy==0.910
 	pre-commit==2.15.0
 	pyfakefs>=4.5.3
 	pytest==6.2.5
-	pytest-asyncio<0.19.0
+	pytest-asyncio==0.19.0
 	pytest-cov==3.0.0
 	pytest-httpx==0.21.0
 	pytest-mock==3.6.1
 	pytest-timeout==2.1.0
 	pytest-xdist==2.5.0
 	types-cryptography==3.3.18
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/async_db/__init__.py` & `firebolt_sdk-0.9.2/src/firebolt/async_db/__init__.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-0.9.1/src/firebolt/async_db/_types.py` & `firebolt_sdk-0.9.2/src/firebolt/async_db/_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,34 +42,34 @@
 ParameterType = Union[int, float, str, datetime, date, bool, Decimal, Sequence]
 
 # These definitions are required by PEP-249
 Date = date
 
 
 def DateFromTicks(t: int) -> date:
-    """Convert ticks to date for firebolt db."""
+    """Convert `ticks` to `date` for Firebolt DB."""
     return datetime.fromtimestamp(t).date()
 
 
 def Time(hour: int, minute: int, second: int) -> None:
-    """Unsupported: construct time for firebolt db."""
-    raise NotSupportedError("time is not supported by Firebolt")
+    """Unsupported: Construct `time`, for Firebolt DB."""
+    raise NotSupportedError("The time construct is not supported by Firebolt")
 
 
 def TimeFromTicks(t: int) -> None:
-    """Unsupported: convert ticks to time for firebolt db."""
-    raise NotSupportedError("time is not supported by Firebolt")
+    """Unsupported: Convert `ticks` to `time` for Firebolt DB."""
+    raise NotSupportedError("The time construct is not supported by Firebolt")
 
 
 Timestamp = datetime
 TimestampFromTicks = datetime.fromtimestamp
 
 
 def Binary(value: str) -> str:
-    """Convert string to binary for firebolt db, does nothing."""
+    """Convert string to binary for Firebolt DB does nothing."""
     return value
 
 
 STRING = BINARY = str
 NUMBER = int
 DATETIME = datetime
 ROWID = int
@@ -85,15 +85,15 @@
         "scale",
         "null_ok",
     ),
 )
 
 
 class ARRAY:
-    """Class for holding information about array column type in firebolt db."""
+    """Class for holding `array` column type information in Firebolt DB."""
 
     _prefix = "Array("
 
     def __init__(self, subtype: Union[type, ARRAY, DECIMAL, DATETIME64]):
         assert (subtype in _col_types and subtype is not list) or isinstance(
             subtype, (ARRAY, DECIMAL, DATETIME64)
         ), f"Invalid array subtype: {str(subtype)}"
@@ -105,15 +105,15 @@
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, ARRAY):
             return NotImplemented
         return other.subtype == self.subtype
 
 
 class DECIMAL:
-    """Class for holding imformation about decimal value in firebolt db."""
+    """Class for holding `decimal` value information in Firebolt DB."""
 
     _prefix = "Decimal("
 
     def __init__(self, precision: int, scale: int):
         self.precision = precision
         self.scale = scale
 
@@ -123,15 +123,15 @@
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, DECIMAL):
             return NotImplemented
         return other.precision == self.precision and other.scale == self.scale
 
 
 class DATETIME64:
-    """Class for holding imformation about datetime64 value in firebolt db."""
+    """Class for holding `datetime64` value information in Firebolt DB."""
 
     _prefix = "DateTime64("
 
     def __init__(self, precision: int):
         self.precision = precision
 
     def __str__(self) -> str:
@@ -143,15 +143,15 @@
         return other.precision == self.precision
 
 
 NULLABLE_PREFIX = "Nullable("
 
 
 class _InternalType(Enum):
-    """Enum of all internal firebolt types except for array."""
+    """Enum of all internal Firebolt types, except for `array`."""
 
     # INT, INTEGER
     Int8 = "Int8"
     UInt8 = "UInt8"
     Int16 = "Int16"
     UInt16 = "UInt16"
     Int32 = "Int32"
@@ -178,15 +178,15 @@
     DateTime = "DateTime"
 
     # Nullable(Nothing)
     Nothing = "Nothing"
 
     @cached_property
     def python_type(self) -> type:
-        """Convert internal type to python type."""
+        """Convert internal type to Python type."""
         types = {
             _InternalType.Int8: int,
             _InternalType.UInt8: int,
             _InternalType.Int16: int,
             _InternalType.UInt16: int,
             _InternalType.Int32: int,
             _InternalType.UInt32: int,
@@ -201,15 +201,15 @@
             # For simplicity, this could happen only during 'select null' query
             _InternalType.Nothing: str,
         }
         return types[self]
 
 
 def parse_type(raw_type: str) -> Union[type, ARRAY, DECIMAL, DATETIME64]:
-    """Parse typename, provided by query metadata into python type."""
+    """Parse typename provided by query metadata into Python type."""
     if not isinstance(raw_type, str):
         raise DataError(f"Invalid typename {str(raw_type)}: str expected")
     # Handle arrays
     if raw_type.startswith(ARRAY._prefix) and raw_type.endswith(")"):
         return ARRAY(parse_type(raw_type[len(ARRAY._prefix) : -1]))
     # Handle decimal
     if raw_type.startswith(DECIMAL._prefix) and raw_type.endswith(")"):
@@ -240,15 +240,15 @@
         return str
 
 
 def parse_value(
     value: RawColType,
     ctype: Union[type, ARRAY, DECIMAL, DATETIME64],
 ) -> ColType:
-    """Provided raw value and python type, parses first into python value."""
+    """Provided raw value, and Python type; parses first into Python value."""
     if value is None:
         return None
     if ctype in (int, str, float):
         assert isinstance(ctype, type)
         return ctype(value)
     if ctype is date:
         if not isinstance(value, str):
@@ -272,15 +272,15 @@
     "\0": "\\0",
     "\\": "\\\\",
     "'": "\\'",
 }
 
 
 def format_value(value: ParameterType) -> str:
-    """For python value to be used in a SQL query"""
+    """For Python value to be used in a SQL query."""
     if isinstance(value, bool):
         return str(int(value))
     if isinstance(value, (int, float, Decimal)):
         return str(value)
     elif isinstance(value, str):
         return f"'{''.join(escape_chars.get(c, c) for c in value)}'"
     elif isinstance(value, datetime):
@@ -295,15 +295,15 @@
         return f"[{', '.join(format_value(it) for it in value)}]"
 
     raise DataError(f"unsupported parameter type {type(value)}")
 
 
 def format_statement(statement: Statement, parameters: Sequence[ParameterType]) -> str:
     """
-    Substitute placeholders in a sqlparse statement with provided values.
+    Substitute placeholders in a `sqlparse` statement with provided values.
     """
     idx = 0
 
     def process_token(token: Token) -> Token:
         nonlocal idx
         if token.ttype == TokenType.Name.Placeholder:
             # Replace placeholder with formatted parameter
@@ -332,15 +332,18 @@
     return formatted_sql
 
 
 SetParameter = namedtuple("SetParameter", ["name", "value"])
 
 
 def statement_to_set(statement: Statement) -> Optional[SetParameter]:
-    """Try to parse statement as a SET command. Return None if it's not a SET command"""
+    """
+    Try to parse `statement` as a `SET` command.
+    Return `None` if it's not a `SET` command.
+    """
     # Filter out meaningless tokens like Punctuation and Whitespaces
     tokens = [
         token
         for token in statement.tokens
         if token.ttype == TokenType.Keyword or isinstance(token, Comparison)
     ]
 
@@ -366,17 +369,16 @@
     return str(statement).strip().rstrip(";")
 
 
 def split_format_sql(
     query: str, parameters: Sequence[Sequence[ParameterType]]
 ) -> List[Union[str, SetParameter]]:
     """
-    Split a query into separate statement, and format it with parameters
-    if it's a single statement
-    Trying to format a multi-statement query would result in NotSupportedError
+    Multi-statement query formatting will result in `NotSupportedError`.
+    Instead, split a query into a separate statement and format with parameters.
     """
     statements = parse_sql(query)
     if not statements:
         return [query]
 
     if parameters:
         if len(statements) > 1:
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/async_db/connection.py` & `firebolt_sdk-0.9.2/src/firebolt/async_db/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,17 @@
 )
 from firebolt.utils.usage_tracker import get_user_agent_header
 from firebolt.utils.util import fix_url_schema
 
 DEFAULT_TIMEOUT_SECONDS: int = 5
 KEEPALIVE_FLAG: int = 1
 KEEPIDLE_RATE: int = 60  # seconds
-AUTH_CREDENTIALS_DEPRECATION_MESSAGE = """ Passing connection credentials directly to `connect` function is deprecated.
- Please consider passing Auth object instead.
+AUTH_CREDENTIALS_DEPRECATION_MESSAGE = """ Passing connection credentials
+ directly to the `connect` function is deprecated.
+ Pass the `Auth` object instead.
  Examples:
   >>> from firebolt.client.auth import UsernamePassword
   >>> ...
   >>> connect(auth=UsernamePassword(username, password), ...)
  or
   >>> from firebolt.client.auth import Token
   >>> ...
@@ -124,37 +125,37 @@
 
 def _get_auth(
     username: Optional[str],
     password: Optional[str],
     access_token: Optional[str],
     use_token_cache: bool,
 ) -> Auth:
-    """Create Auth class based on provided credentials.
+    """Create `Auth` class based on provided credentials.
 
-    If access_token is provided, it's used for Auth creation.
-    Username and password are used otherwise.
+    If `access_token` is provided, it's used for `Auth` creation.
+    Otherwise, username/password are used.
 
     Returns:
-        Auth: auth object
+        Auth: `auth object`
 
     Raises:
-        ConfigurationError: Invalid combination of credentials provided
+        `ConfigurationError`: Invalid combination of credentials provided
 
     """
     if not access_token:
         if not username or not password:
             raise ConfigurationError(
                 "Neither username/password nor access_token are provided. Provide one"
-                " to authenticate"
+                " to authenticate."
             )
         return UsernamePassword(username, password, use_token_cache)
     if username or password:
         raise ConfigurationError(
-            "Either username/password and access_token are provided. Provide only one"
-            " to authenticate"
+            "Username/password and access_token are both provided. Provide only one"
+            " to authenticate."
         )
     return Token(access_token)
 
 
 def async_connect_factory(connection_class: Type) -> Callable:
     async def connect_inner(
         database: str = None,
@@ -168,32 +169,32 @@
         api_endpoint: str = DEFAULT_API_URL,
         use_token_cache: bool = True,
         additional_parameters: Dict[str, Any] = {},
     ) -> Connection:
         """Connect to Firebolt database.
 
         Args:
-            database (str): Name of the database to connect
-            username (Optional[str]): User name to use for authentication (Deprecated)
-            password (Optional[str]): Password to use for authentication (Deprecated)
-            access_token (Optional[str]): Authentication token to use insead of
+            `database` (str): Name of the database to connect
+            `username` (Optional[str]): User name to use for authentication (Deprecated)
+            `password` (Optional[str]): Password to use for authentication (Deprecated)
+            `access_token` (Optional[str]): Authentication token to use instead of
                                           credentials (Deprecated)
-            auth (Auth)L Authentication object
-            engine_name (Optional[str]): The name of the engine to connect to
-            engine_url (Optional[str]): The engine endpoint to use
-            account_name (Optional[str]): For customers with multiple accounts;
-                                          if None uses default.
-            api_endpoint (str): Firebolt API endpoint. Used for authentication.
-            use_token_cache (bool): Cached authentication token in filesystem.
+            `auth` (Auth)L Authentication object.
+            `engine_name` (Optional[str]): Name of the engine to connect to
+            `engine_url` (Optional[str]): The engine endpoint to use
+            `account_name` (Optional[str]): For customers with multiple accounts;
+                                          if none, default is used
+            `api_endpoint` (str): Firebolt API endpoint. Used for authentication
+            `use_token_cache` (bool): Cached authentication token in filesystem
                                     Default: True
-            additional_parameters (Optional[Dict]): Dictionary of less widely-used
-                                    arguments for connection.
+            `additional_parameters` (Optional[Dict]): Dictionary of less widely-used
+                                    arguments for connection
 
         Note:
-            Providing both `engine_name` and `engine_url` would result in an error.
+            Providing both `engine_name` and `engine_url` will result in an error
 
         """
         # These parameters are optional in function signature
         # but are required to connect.
         # PEP 249 recommends making them kwargs.
         if not database:
             raise ConfigurationError("database name is required to connect.")
@@ -247,19 +248,20 @@
         )
 
     return connect_inner
 
 
 class OverriddenHttpBackend(AutoBackend):
     """
-    This class is a short-term solution for TCP keep-alive issue:
+    `OverriddenHttpBackend` is a short-term solution for the TCP
+    connection idle timeout issue described in the following article:
     https://docs.aws.amazon.com/elasticloadbalancing/latest/network/network-load-balancers.html#connection-idle-timeout
-    Since httpx creates a connection right before executing a request
-    backend has to be overridden in order to set the socket KEEPALIVE
-    and KEEPIDLE settings.
+    Since httpx creates a connection right before executing a request, the
+    backend must be overridden to set the socket to `KEEPALIVE`
+    and `KEEPIDLE` settings.
     """
 
     async def connect_tcp(
         self,
         host: str,
         port: int,
         timeout: Optional[float] = None,
@@ -326,15 +328,15 @@
 
     def _cursor(self, **kwargs: Any) -> BaseCursor:
         """
         Create new cursor object.
         """
 
         if self.closed:
-            raise ConnectionClosedError("Unable to create cursor: connection closed")
+            raise ConnectionClosedError("Unable to create cursor: connection closed.")
 
         c = self.cursor_class(self._client, self, **kwargs)
         self._cursors.append(c)
         return c
 
     async def _aclose(self) -> None:
         """Close connection and all underlying cursors."""
@@ -350,47 +352,47 @@
             # but it shouldn't raise an error in this case
             c.close()
         await self._client.aclose()
         self._is_closed = True
 
     @property
     def closed(self) -> bool:
-        """True if connection is closed, False otherwise."""
+        """`True if connection is closed; False otherwise."""
         return self._is_closed
 
     def _remove_cursor(self, cursor: Cursor) -> None:
         # This way it's atomic
         try:
             self._cursors.remove(cursor)
         except ValueError:
             pass
 
     def commit(self) -> None:
-        """Does nothing since Firebolt doesn't have transactions"""
+        """Does nothing since Firebolt doesn't have transactions."""
 
         if self.closed:
-            raise ConnectionClosedError("Unable to commit: connection closed")
+            raise ConnectionClosedError("Unable to commit: Connection closed.")
 
 
 class Connection(BaseConnection):
     """
-    Firebolt asyncronous database connection class. Implements `PEP 249`_.
+    Firebolt asynchronous database connection class. Implements `PEP 249`_.
 
     Args:
-        engine_url: Firebolt database engine REST API url
-        database: Firebolt database name
-        username: Firebolt account username
-        password: Firebolt account password
-        api_endpoint: Optional. Firebolt API endpoint. Used for authentication.
-        connector_versions: Optional. Tuple of connector name and version or
-            list of tuples of your connector stack. Useful for tracking custom
+        `engine_url`: Firebolt database engine REST API url
+        `database`: Firebolt database name
+        `username`: Firebolt account username
+        `password`: Firebolt account password
+        `api_endpoint`: Optional. Firebolt API endpoint used for authentication
+        `connector_versions`: Optional. Tuple of connector name and version, or
+            a list of tuples of your connector stack. Useful for tracking custom
             connector usage.
 
     Note:
-        Firebolt currenly doesn't support transactions
+        Firebolt does not support transactions,
         so commit and rollback methods are not implemented.
 
     .. _PEP 249:
         https://www.python.org/dev/peps/pep-0249/
 
     """
 
@@ -402,15 +404,15 @@
         c = super()._cursor()
         assert isinstance(c, Cursor)  # typecheck
         return c
 
     # Context manager support
     async def __aenter__(self) -> Connection:
         if self.closed:
-            raise ConnectionClosedError("Connection is already closed")
+            raise ConnectionClosedError("Connection is already closed.")
         return self
 
     async def __aexit__(
         self, exc_type: type, exc_val: Exception, exc_tb: TracebackType
     ) -> None:
         await self._aclose()
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/async_db/cursor.py` & `firebolt_sdk-0.9.2/src/firebolt/async_db/cursor.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     ERROR = 2
     DONE = 3
     CLOSED = 4
 
 
 class Statistics(BaseModel):
     """
-    Class for query execution statistics
+    Class for query execution statistics.
     """
 
     elapsed: float
     rows_read: int
     bytes_read: int
     time_before_execution: float
     time_to_execute: float
@@ -148,15 +148,15 @@
     def __del__(self) -> None:
         self.close()
 
     @property  # type: ignore
     @check_not_closed
     def description(self) -> Optional[List[Column]]:
         """
-        Provides information about a single result row of a query
+        Provides information about a single result row of a query.
 
         Attributes:
             * ``name``
             * ``type_code``
             * ``display_size``
             * ``internal_size``
             * ``precision``
@@ -164,15 +164,15 @@
             * ``null_ok``
         """
         return self._descriptions
 
     @property  # type: ignore
     @check_not_closed
     def statistics(self) -> Optional[Statistics]:
-        """Query execution statistics returned by the backend"""
+        """Query execution statistics returned by the backend."""
         return self._statistics
 
     @property  # type: ignore
     @check_not_closed
     def rowcount(self) -> int:
         """The number of rows produced by last query."""
         return self._rowcount
@@ -206,16 +206,16 @@
 
     @check_not_closed
     @check_query_executed
     def nextset(self) -> Optional[bool]:
         """
         Skip to the next available set, discarding any remaining rows
         from the current set.
-        Returns True if operation was successful,
-        None if there are no more sets to retrive
+        Returns True if operation was successful;
+        None if there are no more sets to retrive.
         """
         return self._pop_next_set()
 
     def _pop_next_set(self) -> Optional[bool]:
         """
         Same functionality as .nextset, but doesn't check that query has been executed.
         """
@@ -334,22 +334,22 @@
         set_parameters: Optional[Dict] = None,
         skip_parsing: bool = False,
     ) -> None:
         self._reset()
         if set_parameters is not None:
             logger.warning(
                 "Passing set parameters as an argument is deprecated. Please run "
-                "a query 'SET <param> = <value>'"
+                "a query 'SET <param> = <value>'."
             )
         try:
 
             if parameters and skip_parsing:
                 logger.warning(
                     "Query formatting parameters are provided with skip_parsing."
-                    " They will be ignored"
+                    " They will be ignored."
                 )
 
             # Allow users to manually skip parsing for performance improvement
             queries: List[Union[SetParameter, str]] = (
                 [raw_query] if skip_parsing else split_format_sql(raw_query, parameters)
             )
 
@@ -412,34 +412,34 @@
         """Prepare and execute a database query.
 
         Supported features:
             Parameterized queries: placeholder characters ('?') are substituted
                 with values provided in `parameters`. Values are formatted to
                 be properly recognized by database and to exclude SQL injection.
             Multi-statement queries: multiple statements, provided in a single query
-                and separated by semicolon are executed separatelly and sequentially.
+                and separated by semicolon, are executed separatelly and sequentially.
                 To switch to next statement result, `nextset` method should be used.
             SET statements: to provide additional query execution parameters, execute
                 `SET param=value` statement before it. All parameters are stored in
                 cursor object until it's closed. They can also be removed with
                 `flush_parameters` method call.
 
         Args:
             query (str): SQL query to execute
             parameters (Optional[Sequence[ParameterType]]): A sequence of substitution
                 parameters. Used to replace '?' placeholders inside a query with
-                actual values
+                actual values.
             set_parameters (Optional[Dict]): List of set parameters to execute
-                a query with. DEPRECATED: Use SET SQL statements instead
+                a query with. DEPRECATED: Use SET SQL statements instead.
             skip_parsing (bool): Flag to disable query parsing. This will
-                disable parameterized, multi-statement and SET queries,
-                while improving performance
+                disable parameterized, multi-statement, and SET queries,
+                while improving performance.
 
         Returns:
-            int: Query row count
+            int: Query row count.
         """
         params_list = [parameters] if parameters else []
         await self._do_execute(query, params_list, set_parameters, skip_parsing)
         return self.rowcount
 
     @check_not_closed
     async def executemany(
@@ -447,50 +447,50 @@
     ) -> int:
         """Prepare and execute a database query.
 
         Supports providing multiple substitution parameter sets, executing them
         as multiple statements sequentially.
 
         Supported features:
-            Parameterized queries: placeholder characters ('?') are substituted
+            Parameterized queries: Placeholder characters ('?') are substituted
                 with values provided in `parameters`. Values are formatted to
                 be properly recognized by database and to exclude SQL injection.
-            Multi-statement queries: multiple statements, provided in a single query
-                and separated by semicolon are executed separatelly and sequentially.
-                To switch to next statement result, `nextset` method should be used.
-            SET statements: to provide additional query execution parameters, execute
+            Multi-statement queries: Multiple statements, provided in a single query
+                and separated by semicolon, are executed separately and sequentially.
+                To switch to next statement result, use `nextset` method.
+            SET statements: To provide additional query execution parameters, execute
                 `SET param=value` statement before it. All parameters are stored in
                 cursor object until it's closed. They can also be removed with
                 `flush_parameters` method call.
 
         Args:
-            query (str): SQL query to execute
+            query (str): SQL query to execute.
             parameters_seq (Sequence[Sequence[ParameterType]]): A sequence of
                substitution parameter sets. Used to replace '?' placeholders inside a
                query with actual values from each set in a sequence. Resulting queries
                for each subset are executed sequentially.
 
         Returns:
             int: Query row count
         """
         await self._do_execute(query, parameters_seq)
         return self.rowcount
 
     def _parse_row(self, row: List[RawColType]) -> List[ColType]:
-        """Parse a single data row based on query column types"""
+        """Parse a single data row based on query column types."""
         assert len(row) == len(self.description)
         return [
             parse_value(col, self.description[i].type_code) for i, col in enumerate(row)
         ]
 
     def _get_next_range(self, size: int) -> Tuple[int, int]:
         cleandoc(
             """
             Return range of next rows of size (if possible),
-            and update _idx to point to the end of this range
+            and update _idx to point to the end of this range.
             """
         )
 
         if self._rows is None:
             # No elements to take
             raise DataError("no rows to fetch")
 
@@ -510,15 +510,15 @@
         assert self._rows is not None
         return self._parse_row(self._rows[left])
 
     @check_not_closed
     @check_query_executed
     def fetchmany(self, size: Optional[int] = None) -> List[List[ColType]]:
         """
-        Fetch the next set of rows of a query result,
+        Fetch the next set of rows of a query result;
         cursor.arraysize is default size.
         """
         size = size if size is not None else self.arraysize
         left, right = self._get_next_range(size)
         assert self._rows is not None
         rows = self._rows[left:right]
         return [self._parse_row(row) for row in rows]
@@ -549,24 +549,24 @@
         self, exc_type: type, exc_val: Exception, exc_tb: TracebackType
     ) -> None:
         self.close()
 
 
 class Cursor(BaseCursor):
     """
-    Class, responsible for executing asyncio queries to Firebolt Database.
-    Should not be created directly,
+    Executes asyncio queries to Firebolt Database.
+    Should not be created directly;
     use :py:func:`connection.cursor <firebolt.async_db.connection.Connection>`
 
     Args:
-        description: information about a single result row
-        rowcount: the number of rows produced by last query
-        closed: True if connection is closed, False otherwise
+        description: Information about a single result row.
+        rowcount: The number of rows produced by last query.
+        closed: True if connection is closed; False otherwise.
         arraysize: Read/Write, specifies the number of rows to fetch at a time
-            with the :py:func:`fetchmany` method
+            with the :py:func:`fetchmany` method.
 
     """
 
     __slots__ = BaseCursor.__slots__ + ("_async_query_lock",)
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         self._async_query_lock = RWLock()
@@ -589,35 +589,35 @@
     async def executemany(
         self, query: str, parameters_seq: Sequence[Sequence[ParameterType]]
     ) -> int:
         async with self._async_query_lock.writer:
             return await super().executemany(query, parameters_seq)
         """
             Prepare and execute a database query against all parameter
-            sequences provided
+            sequences provided.
         """
 
     @wraps(BaseCursor.fetchone)
     async def fetchone(self) -> Optional[List[ColType]]:
         async with self._async_query_lock.reader:
             return super().fetchone()
-        """Fetch the next row of a query result set"""
+        """Fetch the next row of a query result set."""
 
     @wraps(BaseCursor.fetchmany)
     async def fetchmany(self, size: Optional[int] = None) -> List[List[ColType]]:
         async with self._async_query_lock.reader:
             return super().fetchmany(size)
-        """fetch the next set of rows of a query result,
-          size is cursor.arraysize by default"""
+        """Fetch the next set of rows of a query result;
+          size is cursor.arraysize by default."""
 
     @wraps(BaseCursor.fetchall)
     async def fetchall(self) -> List[List[ColType]]:
         async with self._async_query_lock.reader:
             return super().fetchall()
-        """Fetch all remaining rows of a query result"""
+        """Fetch all remaining rows of a query result."""
 
     @wraps(BaseCursor.nextset)
     async def nextset(self) -> None:
         async with self._async_query_lock.reader:
             return super().nextset()
 
     # Iteration support
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/async_db/util.py` & `firebolt_sdk-0.9.2/src/firebolt/async_db/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 from firebolt.utils.urls import DATABASES_URL, ENGINES_URL
 
 if TYPE_CHECKING:
     from firebolt.async_db.connection import Connection
 
 
 async def is_db_available(connection: Connection, database_name: str) -> bool:
-    """Verify if the database exists"""
+    """Verify if the database exists."""
     resp = await _filter_request(
         connection, DATABASES_URL, {"filter.name_contains": database_name}
     )
     return len(resp.json()["edges"]) > 0
 
 
 async def is_engine_running(connection: Connection, engine_url: str) -> bool:
-    """Verify if the engine is running"""
+    """Verify if the engine is running."""
     # Url is not always guaranteed to be of this structure
     # but for the sake of error check this is sufficient
     engine_name = URL(engine_url).host.split(".")[0]
     resp = await _filter_request(
         connection,
         ENGINES_URL,
         {
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/client/auth/base.py` & `firebolt_sdk-0.9.2/src/firebolt/client/auth/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class Auth(HttpxAuth):
     """Base authentication class for Firebolt database.
 
     Updates all http requests with bearer token authorization header
 
     Args:
-        use_token_cache (bool): True if token should be cached in filesystem,
+        use_token_cache (bool): True if token should be cached in filesystem;
             False otherwise
     """
 
     __slots__ = (
         "_token",
         "_expires",
         "_use_token_cache",
@@ -62,35 +62,35 @@
         """
         return self._expires is not None and self._expires <= int(time())
 
     @cached_property
     def _token_storage(self) -> Optional[TokenSecureStorage]:
         """Token filesystem cache storage.
 
-        This is evaluated lazily, only if caching is enabled
+        This is evaluated lazily, only if caching is enabled.
 
         Returns:
             Optional[TokenSecureStorage]: Token filesystem cache storage if any
         """
         return None
 
     def _get_cached_token(self) -> Optional[str]:
-        """If caching enabled, get token from filesystem cache.
+        """If caching is enabled, get token from filesystem cache.
 
-        If caching is disabled, None is returned
+        If caching is disabled, None is returned.
 
         Returns:
-            Optional[str]: Token if any and if caching is enabled, None otherwise
+            Optional[str]: Token if any, and if caching is enabled; None otherwise
         """
         if not self._use_token_cache or not self._token_storage:
             return None
         return self._token_storage.get_cached_token()
 
     def _cache_token(self) -> None:
-        """If caching enabled, cache token to filesystem."""
+        """If caching isenabled, cache token to filesystem."""
         if not self._use_token_cache or not self._token_storage:
             return
         # Only cache if token and expiration are retrieved
         if self._token and self._expires:
             self._token_storage.cache_token(self._token, self._expires)
 
     def get_new_token_generator(self) -> Generator[Request, Response, None]:
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/client/auth/token.py` & `firebolt_sdk-0.9.2/src/firebolt/client/auth/token.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from httpx import Request, Response
 
 from firebolt.client.auth import Auth
 from firebolt.utils.exception import AuthorizationError
 
 
 class Token(Auth):
-    """Token authentication class for Firebolt database.
+    """Token authentication class for Firebolt Database.
 
     Uses provided token for authentication. Doesn't cache token and doesn't
-    refresh it on expiration
+    refresh it on expiration.
 
     Args:
         token (str): Authorization token
 
     Attributes:
         token (str):
     """
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/client/auth/username_password.py` & `firebolt_sdk-0.9.2/src/firebolt/client/auth/username_password.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 from firebolt.utils.exception import AuthenticationError
 from firebolt.utils.token_storage import TokenSecureStorage
 from firebolt.utils.urls import AUTH_URL
 from firebolt.utils.util import cached_property
 
 
 class UsernamePassword(Auth):
-    """Username/Password authentication class for Firebolt database.
+    """Username/Password authentication class for Firebolt Database.
 
     Gets authentication token using
-    provided credentials and updates it when it expires
+    provided credentials and updates it when it expires.
 
     Args:
         username (str): Username
         password (str): Password
-        use_token_cache (bool): True if token should be cached in filesystem,
+        use_token_cache (bool): True if token should be cached in filesystem;
             False otherwise
 
     Attributes:
         username (str): Username
         password (str): Password
     """
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/client/client.py` & `firebolt_sdk-0.9.2/src/firebolt/client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,18 +79,18 @@
     Handles the authentication for Firebolt database.
     Authentication can be passed through auth keyword as a tuple or as a
     FireboltAuth instance
     """
 
     @cached_property
     def account_id(self) -> str:
-        """User account id.
+        """User account ID.
 
-        If account_name was provided during Client construction, returns it's id.
-        Gets default account otherwise
+        If account_name was provided during Client construction, returns its ID;
+        gets default account otherwise.
 
         Returns:
             str: Account ID
 
         Raises:
             AccountNotFoundError: No account found with provided name
         """
@@ -114,25 +114,25 @@
             self._merge_auth_request(request), *args, **kwargs
         )
 
 
 class AsyncClient(FireboltClientMixin, HttpxAsyncClient):
     """An HTTP client, based on httpx.AsyncClient.
 
-    Asyncronously handles authentication for Firebolt database.
-    Authentication can be passed through auth keyword as a tuple or as a
-    FireboltAuth instance
+    Asynchronously handles authentication for Firebolt database.
+    Authentication can be passed through auth keyword as a tuple, or as a
+    FireboltAuth instance.
     """
 
     @async_cached_property
     async def account_id(self) -> str:
         """User account id.
 
-        If account_name was provided during AsyncClient construction, returns it's id.
-        Gets default account otherwise
+        If account_name was provided during AsyncClient construction, returns its ID;
+        gets default account otherwise.
 
         Returns:
             str: Account ID
 
         Raises:
             AccountNotFoundError: No account found with provided name
         """
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/client/resource_manager_hooks.py` & `firebolt_sdk-0.9.2/src/firebolt/client/resource_manager_hooks.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,16 +35,16 @@
         response.status_code,
     )
 
 
 def raise_on_4xx_5xx(response: Response) -> None:
     """Raise an error on HTTP response with error return code.
 
-    Hook for an HTTP client
-    If an error is message is found raise as an ApiError
+    Hook for an HTTP client.
+    If an error message is found, raise as an ApiError.
 
     Args:
         response (Response): Response to check for error code
 
     Raises:
         RequestError: Error during performing request
         RuntimeError: Error processing request on server
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/common/settings.py` & `firebolt_sdk-0.9.2/src/firebolt/common/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pydantic import BaseSettings, Field, SecretStr, root_validator
 
 from firebolt.client.auth import Auth
 
 logger = logging.getLogger(__name__)
 
 AUTH_CREDENTIALS_DEPRECATION_MESSAGE = """ Passing connection credentials directly in Settings is deprecated.
- Please consider passing Auth object instead.
+ Use Auth object instead.
  Examples:
   >>> from firebolt.client.auth import UsernamePassword
   >>> ...
   >>> settings = Settings(auth=UsernamePassword(username, password), ...)
  or
   >>> from firebolt.client.auth import Token
   >>> ...
@@ -20,19 +20,19 @@
 
 class Settings(BaseSettings):
     """Settings for Firebolt SDK.
 
     Attributes:
         user (Optional[str]): User name
         password (Optional[str]): User password
-        access_token (Optional[str]): Access token to use for authentication.
+        access_token (Optional[str]): Access token to use for authentication
             Mutually exclusive with user and password
-        account_name (Optional[str]): Account name.
+        account_name (Optional[str]): Account name
             Default user account is used if none provided
-        server (Optional[str]): Environment api endpoint (Advanced).
+        server (Optional[str]): Environment api endpoint (Advanced)
             Default api endpoint is used if none provided
         default_region (str): Default region for provisioning
     """
 
     auth: Auth = Field(None)
     # Authorization
     user: str = Field(None, env="FIREBOLT_USER")
@@ -67,15 +67,15 @@
         params_present = (
             values.get("user") is not None or values.get("password") is not None,
             values.get("access_token") is not None,
             values.get("auth") is not None,
         )
         if sum(params_present) == 0:
             raise ValueError(
-                "Provide at least one of auth, user/password or access_token"
+                "Provide at least one of auth, user/password or access_token."
             )
         if sum(params_present) > 1:
             raise ValueError("Provide only one of auth, user/password or access_token")
         if any(values.get(f) for f in ("user", "password", "access_token")):
             logger.warning(AUTH_CREDENTIALS_DEPRECATION_MESSAGE)
 
         return values
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/db/__init__.py` & `firebolt_sdk-0.9.2/src/firebolt/db/__init__.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-0.9.1/src/firebolt/db/connection.py` & `firebolt_sdk-0.9.2/src/firebolt/db/connection.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-0.9.1/src/firebolt/db/cursor.py` & `firebolt_sdk-0.9.2/src/firebolt/db/cursor.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-0.9.1/src/firebolt/model/__init__.py` & `firebolt_sdk-0.9.2/src/firebolt/model/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 class FireboltBaseModel(BaseModel):
     class Config:
         allow_population_by_field_name = True
         extra = "forbid"
 
     def jsonable_dict(self, *args: Any, **kwargs: Any) -> dict:
         """
-        Generate a dictionary representation of the service that is contains serialized
-        primitive types, and is therefore json-ready.
+        Generate a dictionary representation of the service that contains serialized
+        primitive types, and is therefore JSON-ready.
 
-        This could be replaced with something native, once this issue is resolved:
+        This could be replaced with something native once this issue is resolved:
         https://github.com/samuelcolvin/pydantic/issues/1409
 
-        This function is intended to improve the compatibility with httpx, which
-        expects to take in a dictionary of primitives as input to the json parameter
+        This function is intended to improve the compatibility with HTTPX, which
+        expects to take in a dictionary of primitives as input to the JSON parameter
         of its request function. See: https://www.python-httpx.org/api/#helper-functions
         """
         return json.loads(self.json(*args, **kwargs))
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/model/binding.py` & `firebolt_sdk-0.9.2/src/firebolt/model/binding.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class BindingKey(BaseModel):
     account_id: str
     database_id: str
     engine_id: str
 
 
 class Binding(FireboltBaseModel):
-    """A Binding between an Engine and a Database"""
+    """A binding between an engine and a database."""
 
     binding_key: BindingKey = Field(alias="id")
     is_default_engine: bool = Field(alias="engine_is_default")
 
     # optional
     current_status: Optional[str]
     health_status: Optional[str]
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/model/database.py` & `firebolt_sdk-0.9.2/src/firebolt/model/database.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-0.9.1/src/firebolt/model/engine.py` & `firebolt_sdk-0.9.2/src/firebolt/model/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,17 +46,17 @@
         raise TimeoutError(error_message)
     if verbose:
         print(".", end="")
 
 
 class EngineSettings(FireboltBaseModel):
     """
-    Engine Settings.
+    Engine settings.
 
-    See Also: :py:class:`EngineRevisionSpecification
+    See also: :py:class:`EngineRevisionSpecification
     <firebolt.model.engine_revision.EngineRevisionSpecification>`
     which also contains engine configuration.
     """
 
     preset: str
     auto_stop_delay_duration: str = Field(regex=r"^[0-9]+[sm]$|^0$")
     minimum_logging_level: str
@@ -101,15 +101,15 @@
 
 class FieldMask(FireboltBaseModel):
     paths: Sequence[str] = Field(alias="paths")
 
 
 class Engine(FireboltBaseModel):
     """
-    A Firebolt engine. Responsible for performing work (queries, data ingestion).
+    A Firebolt engine. Responsible for performing work (queries, ingestion).
 
     Engines are configured in :py:class:`Settings
     <firebolt.model.engine.EngineSettings>`
     and in :py:class:`EngineRevisionSpecification
     <firebolt.model.engine_revision.EngineRevisionSpecification>`.
     """
 
@@ -158,37 +158,37 @@
     @property
     def database(self) -> Optional[Database]:
         return self._service.resource_manager.bindings.get_database_bound_to_engine(
             engine=self
         )
 
     def get_latest(self) -> Engine:
-        """Get an up-to-date instance of the Engine from Firebolt."""
+        """Get an up-to-date instance of the engine from Firebolt."""
         return self._service.get(id_=self.engine_id)
 
     def attach_to_database(
         self, database: Database, is_default_engine: bool = False
     ) -> Binding:
         """
         Attach this engine to a database.
 
         Args:
-            database: Database to which the engine will be attached.
+            database: Database to which the engine will be attached
             is_default_engine:
                 Whether this engine should be used as default for this database.
                 Only one engine can be set as default for a single database.
                 This will overwrite any existing default.
         """
         return self._service.resource_manager.bindings.create(
             engine=self, database=database, is_default_engine=is_default_engine
         )
 
     @check_attached_to_database
     def get_connection(self) -> Connection:
-        """Get a connection to the attached database, for running queries.
+        """Get a connection to the attached database for running queries.
 
         Returns:
             Connection: engine connection instance
 
         """
         return connect(
             database=self.database.name,  # type: ignore # already checked by decorator
@@ -207,24 +207,24 @@
     ) -> Engine:
         """
         Start an engine. If it's already started, do nothing.
 
         Args:
             wait_for_startup:
                 If True, wait for startup to complete.
-                If false, return immediately after requesting startup.
+                If False, return immediately after requesting startup.
             wait_timeout_seconds:
                 Number of seconds to wait for startup to complete
-                before raising a TimeoutError.
+                before raising a TimeoutError
             verbose:
-                If True, print dots periodically while waiting for engine startup.
-                If false, do not print any dots.
+                If True, print dots periodically while waiting for engine start.
+                If False, do not print any dots.
 
         Returns:
-            The updated Engine from Firebolt.
+            The updated engine from Firebolt.
         """
         timeout_time = time.time() + wait_timeout_seconds
 
         engine = self.get_latest()
         if (
             engine.current_status_summary
             == EngineStatusSummary.ENGINE_STATUS_SUMMARY_RUNNING
@@ -328,20 +328,20 @@
         spec: Optional[str] = None,
         auto_stop: Optional[int] = None,
         warmup: Optional[WarmupMethod] = None,
         description: Optional[str] = None,
         use_spot: Optional[bool] = None,
     ) -> Engine:
         """
-        update the engine, and returns an updated version of the engine, all parameters
-        could be set to None, this would keep the old engine parameter value
+        Updates the engine and returns an updated version of the engine. If all
+        parameters are set to None, old engine parameter values remain.
         """
 
         class _EngineUpdateRequest(FireboltBaseModel):
-            """Helper model for sending Engine update requests."""
+            """Helper model for sending engine update requests."""
 
             account_id: str
             desired_revision: Optional[EngineRevision]
             engine: Engine
             engine_id: str
             update_mask: FieldMask
 
@@ -424,21 +424,21 @@
     ) -> Engine:
         """
         Restart an engine.
 
         Args:
             wait_for_startup:
                 If True, wait for startup to complete.
-                If false, return immediately after requesting startup.
+                If False, return immediately after requesting startup.
             wait_timeout_seconds:
                 Number of seconds to wait for startup to complete
                 before raising a TimeoutError.
 
         Returns:
-            The updated Engine from Firebolt.
+            The updated engine from Firebolt.
         """
         timeout_time = time.time() + wait_timeout_seconds
 
         engine = self._send_engine_request(ACCOUNT_ENGINE_RESTART_URL)
         logger.info(f"Stopping Engine (engine_id={self.engine_id}, name={self.name})")
 
         while wait_for_startup and engine.current_status_summary not in {
@@ -455,15 +455,15 @@
             )
 
             engine = engine.get_latest()
 
         return engine
 
     def delete(self) -> Engine:
-        """Delete an Engine from Firebolt."""
+        """Delete an engine from Firebolt."""
         response = self._service.client.delete(
             url=ACCOUNT_ENGINE_URL.format(
                 account_id=self._service.account_id, engine_id=self.engine_id
             ),
         )
         logger.info(f"Deleting Engine (engine_id={self.engine_id}, name={self.name})")
         return Engine.parse_obj_with_service(
@@ -478,12 +478,12 @@
         )
         return Engine.parse_obj_with_service(
             obj=response.json()["engine"], engine_service=self._service
         )
 
 
 class _EngineCreateRequest(FireboltBaseModel):
-    """Helper model for sending Engine create requests."""
+    """Helper model for sending engine create requests."""
 
     account_id: str
     engine: Engine
     engine_revision: Optional[EngineRevision]
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/model/engine_revision.py` & `firebolt_sdk-0.9.2/src/firebolt/model/engine_revision.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,17 @@
     account_id: str
     engine_id: str
     engine_revision_id: str
 
 
 class EngineRevisionSpecification(FireboltBaseModel):
     """
-    An EngineRevision Specification.
+    An EngineRevision specification.
 
-    Notably, it determines which instance types and how many of them its Engine gets.
+    Determines which instance types and how many of them its engine gets.
 
     See Also: :py:class:`Settings
     <firebolt.model.engine.EngineSettings>`,
     which also contains engine configuration.
     """
 
     db_compute_instances_type_key: InstanceTypeKey = Field(
@@ -35,16 +35,16 @@
     proxy_instances_type_key: InstanceTypeKey = Field(alias="proxy_instances_type_id")
     proxy_instances_count: PositiveInt = 1
     proxy_version: str = ""
 
 
 class EngineRevision(FireboltBaseModel):
     """
-    A Firebolt Engine revision,
-    which contains a Specification (instance types, counts).
+    A Firebolt engine revision,
+    which contains a specification (instance types, counts).
 
     As engines are updated with new settings, revisions are created.
     """
 
     specification: EngineRevisionSpecification
 
     # optional
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/model/instance_type.py` & `firebolt_sdk-0.9.2/src/firebolt/model/instance_type.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-0.9.1/src/firebolt/service/base.py` & `firebolt_sdk-0.9.2/src/firebolt/service/base.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-0.9.1/src/firebolt/service/binding.py` & `firebolt_sdk-0.9.2/src/firebolt/service/binding.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from firebolt.utils.util import prune_dict
 
 logger = logging.getLogger(__name__)
 
 
 class BindingService(BaseService):
     def get_by_key(self, binding_key: BindingKey) -> Binding:
-        """Get a binding by it's BindingKey"""
+        """Get a binding by its BindingKey"""
         response = self.client.get(
             url=ACCOUNT_DATABASE_BINDING_URL.format(
                 account_id=binding_key.account_id,
                 database_id=binding_key.database_id,
                 engine_id=binding_key.engine_id,
             )
         )
@@ -46,15 +46,15 @@
                 If None, match any engines.
             is_system_database:
                 If True, return only system databases.
                 If False, return only non-system databases.
                 If None, do not filter on this parameter.
 
         Returns:
-            List of bindings matching the filter parameters.
+            List of bindings matching the filter parameters
         """
 
         response = self.client.get(
             url=ACCOUNT_BINDINGS_URL.format(account_id=self.account_id),
             params=prune_dict(
                 {
                     "page.first": 5000,  # FUTURE: pagination support w/ generator
@@ -63,15 +63,15 @@
                     "filter.is_system_database_eq": is_system_database,
                 }
             ),
         )
         return [Binding.parse_obj(i["node"]) for i in response.json()["edges"]]
 
     def get_database_bound_to_engine(self, engine: Engine) -> Optional[Database]:
-        """Get the Database to which an engine is bound, if any."""
+        """Get the database to which an engine is bound, if any."""
         try:
             binding = self.get_many(engine_id=engine.engine_id)[0]
         except IndexError:
             return None
         try:
             return self.resource_manager.databases.get(id_=binding.database_id)
         except (KeyError, IndexError):
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/service/database.py` & `firebolt_sdk-0.9.2/src/firebolt/service/database.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 from firebolt.utils.util import prune_dict
 
 logger = logging.getLogger(__name__)
 
 
 class DatabaseService(BaseService):
     def get(self, id_: str) -> Database:
-        """Get a Database from Firebolt by its id."""
+        """Get a Database from Firebolt by its ID."""
 
         response = self.client.get(
             url=ACCOUNT_DATABASE_URL.format(account_id=self.account_id, database_id=id_)
         )
         return Database.parse_obj_with_service(
             obj=response.json()["database"], database_service=self
         )
 
     def get_by_name(self, name: str) -> Database:
-        """Get a Database from Firebolt by its name."""
+        """Get a database from Firebolt by its name."""
 
         database_id = self.get_id_by_name(name=name)
         return self.get(id_=database_id)
 
     def get_id_by_name(self, name: str) -> str:
-        """Get a Database id from Firebolt by its name."""
+        """Get a database ID from Firebolt by its name."""
 
         response = self.client.get(
             url=ACCOUNT_DATABASE_BY_NAME_URL.format(account_id=self.account_id),
             params={"database_name": name},
         )
         database_id = response.json()["database_id"]["database_id"]
         return database_id
@@ -49,23 +49,23 @@
         attached_engine_name_contains: Optional[str] = None,
         order_by: Optional[Union[str, DatabaseOrder]] = None,
     ) -> List[Database]:
         """
         Get a list of databases on Firebolt.
 
         Args:
-            name_contains: Filter for databases with a name containing this substring.
-            attached_engine_name_eq: Filter for databases by an exact engine name.
+            name_contains: Filter for databases with a name containing this substring
+            attached_engine_name_eq: Filter for databases by an exact engine name
             attached_engine_name_contains: Filter for databases by engines with a
-                name containing this substring.
+                name containing this substring
             order_by: Method by which to order the results.
-            See :py:class:`firebolt.service.types.DatabaseOrder`.
+            See :py:class:`firebolt.service.types.DatabaseOrder`
 
         Returns:
-            A list of databases matching the filters.
+            A list of databases matching the filters
         """
 
         if isinstance(order_by, str):
             order_by = DatabaseOrder[order_by].name
 
         params = {
             "page.first": "1000",
@@ -88,23 +88,23 @@
     def create(
         self, name: str, region: Optional[str] = None, description: Optional[str] = None
     ) -> Database:
         """
         Create a new Database on Firebolt.
 
         Args:
-            name: Name of the database.
-            region: Region name in which to create the database.
+            name: Name of the database
+            region: Region name in which to create the database
 
         Returns:
-            The newly created Database.
+            The newly created database
         """
 
         class _DatabaseCreateRequest(FireboltBaseModel):
-            """Helper model for sending Database creation requests."""
+            """Helper model for sending database creation requests."""
 
             account_id: str
             database: Database
 
         if region is None:
             region_key = self.resource_manager.regions.default_region.key
         else:
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/service/engine.py` & `firebolt_sdk-0.9.2/src/firebolt/service/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 from firebolt.utils.util import prune_dict
 
 logger = getLogger(__name__)
 
 
 class EngineService(BaseService):
     def get(self, id_: str) -> Engine:
-        """Get an Engine from Firebolt by its id."""
+        """Get an engine from Firebolt by its ID."""
 
         response = self.client.get(
             url=ACCOUNT_ENGINE_URL.format(account_id=self.account_id, engine_id=id_),
         )
         engine_entry: dict = response.json()["engine"]
         return Engine.parse_obj_with_service(obj=engine_entry, engine_service=self)
 
     def get_by_ids(self, ids: List[str]) -> List[Engine]:
-        """Get multiple Engines from Firebolt by their ids."""
+        """Get multiple engines from Firebolt by ID."""
         response = self.client.post(
             url=ENGINES_BY_IDS_URL,
             json={
                 "engine_ids": [
                     {"account_id": self.account_id, "engine_id": engine_id}
                     for engine_id in ids
                 ]
@@ -44,15 +44,15 @@
         )
         return [
             Engine.parse_obj_with_service(obj=e, engine_service=self)
             for e in response.json()["engines"]
         ]
 
     def get_by_name(self, name: str) -> Engine:
-        """Get an Engine from Firebolt by its name."""
+        """Get an engine from Firebolt by its name."""
 
         response = self.client.get(
             url=ACCOUNT_ENGINE_BY_NAME_URL.format(account_id=self.account_id),
             params={"engine_name": name},
         )
         engine_id = response.json()["engine_id"]["engine_id"]
         return self.get(id_=engine_id)
@@ -65,22 +65,22 @@
         region_eq: Optional[str] = None,
         order_by: Optional[Union[str, EngineOrder]] = None,
     ) -> List[Engine]:
         """
         Get a list of engines on Firebolt.
 
         Args:
-            name_contains: Filter for engines with a name containing this substring.
-            current_status_eq: Filter for engines with this status.
-            current_status_not_eq: Filter for engines that do not have this status.
-            region_eq: Filter for engines by region.
-            order_by: Method by which to order the results. See [EngineOrder].
+            name_contains: Filter for engines with a name containing this substring
+            current_status_eq: Filter for engines with this status
+            current_status_not_eq: Filter for engines that do not have this status
+            region_eq: Filter for engines by region
+            order_by: Method by which to order the results. See [EngineOrder]
 
         Returns:
-            A list of engines matching the filters.
+            A list of engines matching the filters
         """
 
         if isinstance(order_by, str):
             order_by = EngineOrder[order_by].name
 
         if region_eq is not None:
             region_eq = self.resource_manager.regions.get_by_name(
@@ -115,38 +115,38 @@
         auto_stop: int = 20,
         warmup: Union[str, WarmupMethod] = WarmupMethod.PRELOAD_INDEXES,
         description: str = "",
         engine_settings_kwargs: Dict[str, Any] = {},
         revision_spec_kwargs: Dict[str, Any] = {},
     ) -> Engine:
         """
-        Create a new Engine.
+        Create a new engine.
 
         Args:
-            name: An identifier that specifies the name of the engine.
-            region: The AWS region in which the engine runs.
+            name: An identifier that specifies the name of the engine
+            region: The AWS region in which the engine runs
             engine_type: The engine type. GENERAL_PURPOSE or DATA_ANALYTICS
             scale: The number of compute instances on the engine.
                 The scale can be any int from 1 to 128.
-            spec: Firebolt instance type. If not set will default to
+            spec: Firebolt instance type. If not set, will default to
                 the cheapest instance.
             auto_stop: The amount of time (in minutes)
-            after which the engine automatically stops.
-            warmup: The warmup method that should be used.
+            after which the engine automatically stops
+            warmup: The warmup method that should be used:
 
-                `MINIMAL` - On-demand loading (both indexes and tables' data).
+                `MINIMAL` - On-demand loading (both indexes and tables' data)
 
-                `PRELOAD_INDEXES` - Load indexes only.
+                `PRELOAD_INDEXES` - Load indexes only
 
                 `PRELOAD_ALL_DATA` - Full data auto-load
-                (both indexes and table data - full warmup).
-            description: A short description of the engine's purpose.
+                (both indexes and table data - full warmup)
+            description: A short description of the engine's purpose
 
         Returns:
-            Engine with the specified settings.
+            Engine with the specified settings
         """
 
         logger.info(f"Creating Engine (name={name})")
 
         if isinstance(engine_type, str):
             engine_type = EngineType[engine_type]
         if isinstance(warmup, str):
@@ -198,19 +198,19 @@
     def _send_create_engine(
         self, engine: Engine, engine_revision: Optional[EngineRevision] = None
     ) -> Engine:
         """
         Create a new Engine on Firebolt from the local Engine object.
 
         Args:
-            engine: The Engine to create.
-            engine_revision: EngineRevision to use for configuring the Engine.
+            engine: The engine to create
+            engine_revision: EngineRevision to use for configuring the engine
 
         Returns:
-            The newly created engine.
+            The newly created engine
         """
 
         response = self.client.post(
             url=ACCOUNT_ENGINES_URL.format(account_id=self.account_id),
             headers={"Content-type": "application/json"},
             json=_EngineCreateRequest(
                 account_id=self.account_id,
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/service/engine_revision.py` & `firebolt_sdk-0.9.2/src/firebolt/service/engine_revision.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         )
 
     def get_by_key(self, key: EngineRevisionKey) -> EngineRevision:
         """
         Fetch an EngineRevision from Firebolt by its key.
 
         Args:
-            key: Key of the desired EngineRevision.
+            key: Key of the desired EngineRevision
 
         Returns:
             The requested EngineRevision
         """
 
         response = self.client.get(
             url=ACCOUNT_ENGINE_REVISION_URL.format(
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/service/instance_type.py` & `firebolt_sdk-0.9.2/src/firebolt/service/instance_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from firebolt.model.region import Region
 from firebolt.service.base import BaseService
 from firebolt.utils.urls import ACCOUNT_INSTANCE_TYPES_URL
 from firebolt.utils.util import cached_property
 
 
 class InstanceTypeLookup(NamedTuple):
-    """Helper tuple for looking up instance types by names"""
+    """Helper tuple for looking up instance types by names."""
 
     region_name: str
     instance_type_name: str
 
 
 class InstanceTypeService(BaseService):
     @cached_property
@@ -89,21 +89,21 @@
         instance_type_name: str,
         region_name: Optional[str] = None,
     ) -> InstanceType:
         """
         Get an instance type by name.
 
         Args:
-            instance_type_name: Name of the instance (eg. "i3.4xlarge").
+            instance_type_name: Name of the instance (eg. "i3.4xlarge")
             region_name:
                 Name of the AWS region from which to get the instance.
                 If not provided, use the default region name from the client.
 
         Returns:
-            The requested instance type.
+            The requested instance type
         """
 
         # Will raise an error if neither set
         region_name = region_name or self.resource_manager.regions.default_region.name
         return self.instance_types_by_name[
             InstanceTypeLookup(
                 region_name=region_name,
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/service/manager.py` & `firebolt_sdk-0.9.2/src/firebolt/service/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     - engines
     - bindings (the bindings between an engine and a database)
     - engine revisions (versions of an engine)
 
     Also provides listings of:
 
     - regions (AWS regions in which engines can run)
-
     - instance types (AWS instance types which engines can use)
     """
 
     def __init__(self, settings: Optional[Settings] = None):
         self.settings = settings or Settings()
 
         auth = self.settings.auth
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/service/region.py` & `firebolt_sdk-0.9.2/src/firebolt/service/region.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 from firebolt.utils.urls import REGIONS_URL
 from firebolt.utils.util import cached_property
 
 
 class RegionService(BaseService):
     def __init__(self, resource_manager: ResourceManager):
         """
-        Service to manage AWS Regions (us-east-1, etc).
+        Service to manage AWS regions (us-east-1, etc)
 
         Args:
-            resource_manager: Resource manager to use.
+            resource_manager: Resource manager to use
         """
 
         super().__init__(resource_manager=resource_manager)
 
     @cached_property
     def regions(self) -> List[Region]:
-        """List of available AWS Regions on Firebolt."""
+        """List of available AWS regions on Firebolt."""
 
         response = self.client.get(url=REGIONS_URL, params={"page.first": 5000})
         return [Region.parse_obj(i["node"]) for i in response.json()["edges"]]
 
     @cached_property
     def regions_by_name(self) -> Dict[str, Region]:
         """Dict of {RegionLookup to Region}"""
@@ -35,31 +35,31 @@
     def regions_by_key(self) -> Dict[RegionKey, Region]:
         """Dict of {RegionKey to Region}"""
 
         return {r.key: r for r in self.regions}
 
     @cached_property
     def default_region(self) -> Region:
-        """Default AWS Region, could be provided from environment."""
+        """Default AWS region, could be provided from environment."""
 
         if not self.settings.default_region:
             raise ValueError(
                 "The environment variable FIREBOLT_DEFAULT_REGION must be set."
             )
         return self.get_by_name(name=self.settings.default_region)
 
     def get_by_name(self, name: str) -> Region:
         """Get an AWS region by its name (eg. us-east-1)."""
 
         return self.regions_by_name[name]
 
     def get_by_key(self, key: RegionKey) -> Region:
-        """Get an AWS Region by its key."""
+        """Get an AWS region by its key."""
 
         return self.regions_by_key[key]
 
     def get_by_id(self, id_: str) -> Region:
-        """Get an AWS Region by region_id."""
+        """Get an AWS region by region_id."""
 
         return self.get_by_key(
             RegionKey(provider_id=self.resource_manager.provider_id, region_id=id_)
         )
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/service/types.py` & `firebolt_sdk-0.9.2/src/firebolt/service/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,17 @@
     """
     Detailed engine status.
 
     See: https://api.dev.firebolt.io/devDocs#operation/coreV1GetEngine
     """
 
     ENGINE_STATUS_UNSPECIFIED = "ENGINE_STATUS_UNSPECIFIED"
-    """ Logical record is created, however underlying infrastructure
+    """ Logical record is created, however, underlying infrastructure
     is not initialized.
-    In other words this means that engine is stopped."""
+    In other words, this means that engine is stopped."""
 
     ENGINE_STATUS_CREATED = "ENGINE_STATUS_CREATED"
     """Engine status was created."""
 
     ENGINE_STATUS_PROVISIONING_PENDING = "ENGINE_STATUS_PROVISIONING_PENDING"
     """ Engine initialization request was sent."""
 
@@ -58,51 +58,51 @@
 
     ENGINE_STATUS_RUNNING_IDLE = "ENGINE_STATUS_RUNNING_IDLE"
     """ Engine is initialized,
     but there are no running or starting engine revisions."""
 
     ENGINE_STATUS_RUNNING_REVISION_STARTING = "ENGINE_STATUS_RUNNING_REVISION_STARTING"
     """ Engine is initialized,
-    there are no running engine revision but it's starting."""
+    there are no running engine revisions, but it's starting."""
 
     ENGINE_STATUS_RUNNING_REVISION_STARTUP_FAILED = (
         "ENGINE_STATUS_RUNNING_REVISION_STARTUP_FAILED"
     )
-    """ Engine is initialized,
-    initial revision is failed to provision or start."""
+    """ Engine is initialized;
+    initial revision failed to provision or start."""
 
     ENGINE_STATUS_RUNNING_REVISION_SERVING = "ENGINE_STATUS_RUNNING_REVISION_SERVING"
     """ Engine is ready (serves an engine revision). """
 
     ENGINE_STATUS_RUNNING_REVISION_CHANGING = "ENGINE_STATUS_RUNNING_REVISION_CHANGING"
-    """ Engine is ready (serves an engine revision),
+    """ Engine is ready (serves an engine revision);
      zero-downtime replacement revision is starting."""
 
     ENGINE_STATUS_RUNNING_REVISION_CHANGE_FAILED = (
         "ENGINE_STATUS_RUNNING_REVISION_CHANGE_FAILED"
     )
-    """ Engine is ready (serves an engine revision),
+    """ Engine is ready (serves an engine revision);
      replacement revision failed to provision or start."""
 
     ENGINE_STATUS_RUNNING_REVISION_RESTARTING = (
         "ENGINE_STATUS_RUNNING_REVISION_RESTARTING"
     )
-    """ Engine is initialized,
+    """ Engine is initialized;
     replacement of the revision with a downtime is in progress."""
 
     ENGINE_STATUS_RUNNING_REVISION_RESTART_FAILED = (
         "ENGINE_STATUS_RUNNING_REVISION_RESTART_FAILED"
     )
-    """ Engine is initialized,
+    """ Engine is initialized;
     replacement revision failed to provision or start."""
 
     ENGINE_STATUS_RUNNING_REVISIONS_TERMINATING = (
         "ENGINE_STATUS_RUNNING_REVISIONS_TERMINATING"
     )
-    """ Engine is initialized,
+    """ Engine is initialized;
     all child revisions are being terminated."""
 
     # Engine termination request was sent.
     ENGINE_STATUS_TERMINATION_PENDING = "ENGINE_STATUS_TERMINATION_PENDING"
     """ Engine termination request was sent."""
 
     ENGINE_STATUS_TERMINATION_ST = "ENGINE_STATUS_TERMINATION_STARTED"
@@ -128,41 +128,41 @@
     ENGINE_STATUS_SUMMARY_UNSPECIFIED = "ENGINE_STATUS_SUMMARY_UNSPECIFIED"
     """Status unspecified"""
 
     ENGINE_STATUS_SUMMARY_STOPPED = "ENGINE_STATUS_SUMMARY_STOPPED"
     """ Fully stopped."""
 
     ENGINE_STATUS_SUMMARY_STARTING = "ENGINE_STATUS_SUMMARY_STARTING"
-    """ Provisioning process is in progress.
-     We are creating cloud infra for this engine."""
+    """ Provisioning process is in progress;
+     creating cloud infra for this engine."""
 
     ENGINE_STATUS_SUMMARY_STARTING_INITIALIZING = (
         "ENGINE_STATUS_SUMMARY_STARTING_INITIALIZING"
     )
-    """ Provisioning process is complete.
-     We are now waiting for PackDB cluster to initialize and start."""
+    """ Provisioning process is complete;
+     waiting for PackDB cluster to initialize and start."""
 
     ENGINE_STATUS_SUMMARY_RUNNING = "ENGINE_STATUS_SUMMARY_RUNNING"
-    """ Fully started.
-     Engine is ready to serve requests."""
+    """ Fully started;
+     engine is ready to serve requests."""
 
     ENGINE_STATUS_SUMMARY_UPGRADING = "ENGINE_STATUS_SUMMARY_UPGRADING"
     """ Version of the PackDB is changing.
      This is zero downtime operation that does not affect engine work.
      This status is reserved for future use (not used fow now)."""
 
     ENGINE_STATUS_SUMMARY_RESTARTING = "ENGINE_STATUS_SUMMARY_RESTARTING"
     """ Hard restart (full stop/start cycle) is in progress.
     Underlying infrastructure is being recreated."""
 
     ENGINE_STATUS_SUMMARY_RESTARTING_INITIALIZING = (
         "ENGINE_STATUS_SUMMARY_RESTARTING_INITIALIZING"
     )
     """ Hard restart (full stop/start cycle) is in progress.
-     Underlying infrastructure is ready, waiting for
+     Underlying infrastructure is ready. Waiting for
      PackDB cluster to initialize and start.
      This status is logically the same as ENGINE_STATUS_SUMMARY_STARTING_INITIALIZING,
      but used during restart cycle."""
 
     ENGINE_STATUS_SUMMARY_REPAIRING = "ENGINE_STATUS_SUMMARY_REPAIRING"
     """ Underlying infrastructure has issues and is being repaired.
      Engine is still running, but it's not fully healthy and some queries may fail."""
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/utils/exception.py` & `firebolt_sdk-0.9.2/src/firebolt/utils/exception.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 
 
 class FireboltEngineError(FireboltError):
     """Base class for engine related errors."""
 
 
 class EngineNotRunningError(FireboltEngineError):
-    """Engine, that's being queried, is not running."""
+    """Engine that's being queried is not running."""
 
 
 class NoAttachedDatabaseError(FireboltEngineError):
-    """Engine, that's being accessed, is not running.
+    """Engine that's being accessed is not running.
 
     Args:
-        method_name (str): Name of the method, which caused issue
+        method_name (str): Method that caused the error
 
     Attributes:
-        method_name (str): Name of the method, which caused issue
+        method_name (str): Method that caused the error
     """
 
     def __init__(self, method_name: str):
         super().__init__(
             f"Unable to call {method_name}: "
-            "Engine must to be attached to a database first."
+            "Engine must be attached to a database first."
         )
         self.method_name = method_name
 
 
 class AlreadyBoundError(FireboltEngineError):
     """Engine is already bound to a database."""
 
@@ -36,33 +36,33 @@
     """Base class for database related errors."""
 
 
 class AccountNotFoundError(FireboltError):
     """Account with provided name doesn't exist.
 
     Args:
-        account_name (str): Name of account, that wasn't found
+        account_name (str): Name of account that wasn't found
 
     Attributes:
-        account_name (str): Name of account, that wasn't found
+        account_name (str): Name of account that wasn't found
     """
 
     def __init__(self, account_name: str):
         super().__init__(f"Account '{account_name}' does not exist.")
         self.account_name = account_name
 
 
 class AttachedEngineInUseError(FireboltDatabaseError):
-    """Engine is unavailable because it's starting/stopping.
+    """Engine unavailable because it's starting/stopping.
 
     Args:
-        method_name (str): Name of the method, which caused issue
+        method_name (str): Method that caused the error
 
     Attributes:
-        method_name (str): Name of the method, which caused issue
+        method_name (str): Method that caused the error
     """
 
     def __init__(self, method_name: str):
         super().__init__(
             f"Unable to call {method_name}: "
             "Engine must not be in starting or stopping state."
         )
@@ -81,51 +81,51 @@
     """Base class for cursor related errors."""
 
 
 class CursorClosedError(CursorError):
     """Cursor operations are unavailable since it's closed.
 
     Args:
-        method_name (str): Name of the method, which caused issue
+        method_name (str): Method that caused the error
 
     Attributes:
-        method_name (str): Name of the method, which caused issue
+        method_name (str): Method that caused the error
     """
 
     def __init__(self, method_name: str):
         super().__init__(f"Unable to call {method_name}: cursor closed.")
         self.method_name = method_name
 
 
 class QueryNotRunError(CursorError):
     """Some cursor methods are unavailable before a query is run.
 
     Args:
-        method_name (str): Name of the method, which caused issue
+        method_name (str): Method that caused the error
 
     Attributes:
-        method_name (str): Name of the method, which caused issue
+        method_name (str): Method that caused the error
     """
 
     def __init__(self, method_name: str):
         super().__init__(f"Unable to call {method_name}: need to run a query first.")
         self.method_name = method_name
 
 
 class AuthenticationError(FireboltError):
     """Firebolt authentication error.
 
     Stores error cause and authentication endpoint.
 
     Args:
-        api_endpoint (str): Environment api endpoint, used for authentication
+        api_endpoint (str): Environment api endpoint used for authentication
         cause (str): Reason for authentication failure
 
     Attributes:
-        api_endpoint (str): Environment api endpoint, used for authentication
+        api_endpoint (str): Environment api endpoint used for authentication
         cause (str): Reason for authentication failure
     """
 
     def __init__(self, cause: str):
         super().__init__(f"Failed to authenticate: {cause}.")
         self.cause = cause
 
@@ -168,57 +168,57 @@
 class DatabaseError(Error):
     """Exception raised for errors that are related to the database."""
 
 
 class DataError(DatabaseError):
     """Data processing error.
 
-    Exception raised for errors that are due to problems with the processed data
+    Exception raised for errors that are due to problems with the processed data,
     like division by zero, numeric value out of range, etc.
     """
 
 
 class OperationalError(DatabaseError):
     """Database operating error.
 
     Exception raised for errors that are related to the database's operation
-    and not necessarily under the control of the programmer, e.g. an unexpected
+    and not necessarily under the control of the programmer, e.g., an unexpected
     disconnect occurs, the data source name is not found, a transaction could not
     be processed, a memory allocation error occurred during processing, etc.
     """
 
 
 class IntegrityError(DatabaseError):
     """Database data integrity error.
 
     Exception raised when the relational integrity of the database is affected,
-    e.g. a foreign key check fails.
+    e.g., a foreign key check fails.
     """
 
 
 class InternalError(DatabaseError):
     """Database internal error.
 
     Exception raised when the database encounters an internal error,
-    e.g. the cursor is not valid anymore, the transaction is out of sync, etc.
+    e.g., the cursor is not valid anymore, the transaction is out of sync, etc.
     """
 
 
 class ProgrammingError(DatabaseError):
     """Database programming error.
 
-    Exception raised for programming errors, e.g. table not found or already exists,
+    Exception raised for programming errors, e.g., table not found or already exists,
     syntax error in the SQL statement, wrong number of parameters specified, etc.
     """
 
 
 class NotSupportedError(DatabaseError):
     """Operation not supported.
 
     Exception raised in case a method or database API was used which is not supported
-    by the database, e.g. requesting a .rollback() on a connection that
+    by the database, e.g., requesting a .rollback() on a connection that
     does not support transaction or has transactions turned off.
     """
 
 
 class ConfigurationError(InterfaceError):
     """Invalid configuration error."""
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/utils/token_storage.py` & `firebolt_sdk-0.9.2/src/firebolt/utils/token_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             except JSONDecodeError:
                 return {}
 
     def get_cached_token(self) -> Optional[str]:
         """Get decrypted token.
 
         If token is not found, cannot be decrypted with username and password,
-        or is expired - None will be returned
+        or is expired - None will be returned.
 
         Returns:
             Optional[str]: Decrypted token or None
         """
         res = self._read_data_json()
         if "token" not in res:
             return None
@@ -110,15 +110,15 @@
 
         return self.encrypter.decrypt(res["token"])
 
     def cache_token(self, token: str, expiration_ts: int) -> None:
         """Encrypt and store token in file system.
 
         Expiration timestamp is also stored with token in order to later
-        be ableto check if it's expired
+        be able to check if it's expired.
 
         Args:
             token (str): Token to store
             expiration_ts (int): Token expiration timestamp
         """
         token = self.encrypter.encrypt(token)
 
@@ -127,15 +127,15 @@
                 {"token": token, "salt": self.salt, "expiration": expiration_ts}, f
             )
 
 
 class FernetEncrypter:
     """PBDKF2HMAC based encrypter.
 
-    Username and password combination is used as a key
+    Username and password combination is used as a key.
 
     Args:
         salt (str): Salt value for encryption
         username: Username for key
         password: Password for key
     """
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/utils/urls.py` & `firebolt_sdk-0.9.2/src/firebolt/utils/urls.py`

 * *Files identical despite different names*

### Comparing `firebolt_sdk-0.9.1/src/firebolt/utils/usage_tracker.py` & `firebolt_sdk-0.9.2/src/firebolt/utils/usage_tracker.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -46,23 +46,23 @@
     (
         "AirbyteSource",
         "establish_async_connection",
         Path("source_firebolt/source.py"),
         "",
     ),
     ("FireboltCLI", "create_connection", Path("firebolt_cli/utils.py"), "firebolt_cli"),
-]
-
-DRIVER_MAP = [
     (
         "DBT",
         "open",
         Path("dbt/adapters/firebolt/connections.py"),
         "dbt.adapters.firebolt",
     ),
+]
+
+DRIVER_MAP = [
     ("SQLAlchemy", "connect", Path("sqlalchemy/engine/default.py"), "firebolt_db"),
 ]
 
 
 def _os_compare(file: Path, expected: Path) -> bool:
     """
     System-independent path comparison.
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt/utils/util.py` & `firebolt_sdk-0.9.2/src/firebolt/utils/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,21 +47,21 @@
 
 TMix = TypeVar("TMix")
 
 
 def mixin_for(baseclass: Type[TMix]) -> Type[TMix]:
     """Define mixin with baseclass typehint.
 
-    Should be used as a mixin base class to fix typehints
+    Should be used as a mixin base class to fix typehints.
 
     Args:
         baseclass (Type[TMix]): Class which mixin will be made for
 
     Returns:
-        Type[TMix]: Mixin type to inherin from
+        Type[TMix]: Mixin type to inherit from
 
     Examples:
         ```
         class ReadonlyMixin(mixin_for(BaseClass))):
             ...
         ```
 
@@ -81,50 +81,50 @@
         str: URL with schema present
 
     """
     return url if url.startswith("http") else f"https://{url}"
 
 
 class AsyncJobThread:
-    """Thread runner that allows running async tasks syncronously in a separate thread.
+    """Thread runner that allows running async tasks synchronously in a separate thread.
 
     Caches loop to be reused in all threads.
-    It allows running async functions syncronously inside a running event loop.
+    It allows running async functions synchronously inside a running event loop.
     Since nesting loops is not allowed, we create a separate thread for a new event loop
 
     Attributes:
         result (Any): Value, returned by coroutine execution
-        exception (Optional[BaseException]): If any, exception that occured
+        exception (Optional[BaseException]): If any, exception that occurred
             during coroutine execution
     """
 
     def __init__(self) -> None:
         self._loop: Optional[AbstractEventLoop] = None
         self.result: Any = None
         self.exception: Optional[BaseException] = None
 
     def _initialize_loop(self) -> None:
         """Initialize a loop once to use for later execution.
 
         Tries to get a running loop.
-        Creates a new loop if no active one and sets it as active.
+        Creates a new loop if no active one, and sets it as active.
         """
         if not self._loop:
             try:
                 # despite the docs, this function fails if no loop is set
                 self._loop = get_event_loop()
             except RuntimeError:
                 self._loop = new_event_loop()
         set_event_loop(self._loop)
 
     def _run(self, coro: Coroutine) -> None:
         """Run coroutine in an event loop.
 
-        Execution return value is stored into ``result`` field
-        If an exception occures, it will be caught and stored into ``exception`` field
+        Execution return value is stored into ``result`` field.
+        If an exception occurs, it will be caught and stored into ``exception`` field.
 
         Args:
             coro (Coroutine): Coroutine to execute
         """
         try:
             self._initialize_loop()
             assert self._loop is not None
@@ -157,15 +157,15 @@
 
     Args:
         f (Callable): function to convert
         async_job_thread (AsyncJobThread): Job thread instance to use for async excution
             (Default value = None)
 
     Returns:
-        Callable: regular function, which can be executed syncronously
+        Callable: regular function, which can be executed synchronously
     """
 
     @wraps(f)
     def sync(*args: Any, **kwargs: Any) -> Any:
         try:
             loop = get_event_loop()
         except RuntimeError:
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt_sdk.egg-info/PKG-INFO` & `firebolt_sdk-0.9.2/src/firebolt_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebolt-sdk
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python SDK for Firebolt
 Home-page: https://github.com/firebolt-db/firebolt-sdk
 Author: Firebolt
 Author-email: support@firebolt.io
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/firebolt-db/firebolt-sdk/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `firebolt_sdk-0.9.1/src/firebolt_sdk.egg-info/SOURCES.txt` & `firebolt_sdk-0.9.2/src/firebolt_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

