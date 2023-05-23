# Comparing `tmp/apify_client-1.2.0b2.tar.gz` & `tmp/apify_client-1.2.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify_client-1.2.0b2.tar", last modified: Tue May 23 14:10:41 2023, max compression
+gzip compressed data, was "apify_client-1.2.1b1.tar", last modified: Tue May 23 16:49:19 2023, max compression
```

## Comparing `apify_client-1.2.0b2.tar` & `apify_client-1.2.1b1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:10:41.190507 apify_client-1.2.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-05-23 14:10:41.190507 apify_client-1.2.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-23 14:10:37.000000 apify_client-1.2.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:10:41.190507 apify_client-1.2.0b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:10:41.182507 apify_client-1.2.0b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:10:41.182507 apify_client-1.2.0b2/src/apify_client/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:10:41.182507 apify_client-1.2.0b2/src/apify_client/clients/
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:10:41.186507 apify_client-1.2.0b2/src/apify_client/clients/base/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/base/actor_job_base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/base/base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/base/resource_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/base/resource_collection_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:10:41.190507 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30492 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/actor_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/actor_env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/actor_env_var_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/actor_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/actor_version_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/build_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    46610 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/dataset_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    15646 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/key_value_store_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/request_queue_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16014 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/run_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/schedule_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    21010 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/task_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/webhook_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/webhook_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/clients/resource_clients/webhook_dispatch_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:09:59.000000 apify_client-1.2.0b2/src/apify_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:10:41.182507 apify_client-1.2.0b2/src/apify_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-05-23 14:10:41.000000 apify_client-1.2.0b2/src/apify_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-23 14:10:41.000000 apify_client-1.2.0b2/src/apify_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:10:41.000000 apify_client-1.2.0b2/src/apify_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-23 14:10:41.000000 apify_client-1.2.0b2/src/apify_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 14:10:41.000000 apify_client-1.2.0b2/src/apify_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:49:19.509238 apify_client-1.2.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-05-23 16:49:19.509238 apify_client-1.2.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-23 16:49:15.000000 apify_client-1.2.1b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 16:49:19.509238 apify_client-1.2.1b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:49:19.501237 apify_client-1.2.1b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:49:19.501237 apify_client-1.2.1b1/src/apify_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:49:19.501237 apify_client-1.2.1b1/src/apify_client/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:49:19.505238 apify_client-1.2.1b1/src/apify_client/clients/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/base/actor_job_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/base/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/base/resource_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/base/resource_collection_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:49:19.509238 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30492 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/actor_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/actor_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/actor_env_var_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/actor_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/actor_version_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/build_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46610 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/dataset_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15646 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/key_value_store_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/request_queue_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16014 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/run_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/schedule_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21010 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/task_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/webhook_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/webhook_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/clients/resource_clients/webhook_dispatch_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:48:39.000000 apify_client-1.2.1b1/src/apify_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:49:19.501237 apify_client-1.2.1b1/src/apify_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-05-23 16:49:19.000000 apify_client-1.2.1b1/src/apify_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-23 16:49:19.000000 apify_client-1.2.1b1/src/apify_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:49:19.000000 apify_client-1.2.1b1/src/apify_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-23 16:49:19.000000 apify_client-1.2.1b1/src/apify_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 16:49:19.000000 apify_client-1.2.1b1/src/apify_client.egg-info/top_level.txt
```

### Comparing `apify_client-1.2.0b2/LICENSE` & `apify_client-1.2.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/PKG-INFO` & `apify_client-1.2.1b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify_client
-Version: 1.2.0b2
+Version: 1.2.1b1
 Summary: Apify API client for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/api/client/python/
 Project-URL: Documentation, https://docs.apify.com/api/client/python/
 Project-URL: Source, https://github.com/apify/apify-client-python
 Project-URL: Issue tracker, https://github.com/apify/apify-client-python/issues
```

### Comparing `apify_client-1.2.0b2/README.md` & `apify_client-1.2.1b1/README.md`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/pyproject.toml` & `apify_client-1.2.1b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 
 name = "apify_client"
 
-version = "1.2.0b2"
+version = "1.2.1b1"
 description = "Apify API client for Python"
 
 readme = "README.md"
 
 license = {text = "Apache Software License"}
 
 authors = [
@@ -43,15 +43,15 @@
 
 
 
 requires-python = ">=3.8"
 
 dependencies = [
 
-    "httpx ~= 0.24.1"
+    "httpx >= 0.24.1"
 
 ]
 
 
 
 [project.optional-dependencies]
```

### Comparing `apify_client-1.2.0b2/src/apify_client/_errors.py` & `apify_client-1.2.1b1/src/apify_client/_errors.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/_http_client.py` & `apify_client-1.2.1b1/src/apify_client/_http_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/_logging.py` & `apify_client-1.2.1b1/src/apify_client/_logging.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/_utils.py` & `apify_client-1.2.1b1/src/apify_client/_utils.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/client.py` & `apify_client-1.2.1b1/src/apify_client/client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/__init__.py` & `apify_client-1.2.1b1/src/apify_client/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/base/actor_job_base_client.py` & `apify_client-1.2.1b1/src/apify_client/clients/base/actor_job_base_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/base/base_client.py` & `apify_client-1.2.1b1/src/apify_client/clients/base/base_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/base/resource_client.py` & `apify_client-1.2.1b1/src/apify_client/clients/base/resource_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/base/resource_collection_client.py` & `apify_client-1.2.1b1/src/apify_client/clients/base/resource_collection_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/__init__.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/actor.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/actor.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/actor_collection.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/actor_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/actor_env_var.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/actor_env_var.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/actor_env_var_collection.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/actor_env_var_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/actor_version.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/actor_version.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/actor_version_collection.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/actor_version_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/build.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/build.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/build_collection.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/build_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/dataset.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/dataset.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/dataset_collection.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/key_value_store.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/key_value_store.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/key_value_store_collection.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/key_value_store_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/log.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/log.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/request_queue.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/request_queue_collection.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/request_queue_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/run.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/run.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/run_collection.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/run_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/schedule.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/schedule.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/schedule_collection.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/schedule_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/task.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/task.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/task_collection.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/task_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/user.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/user.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/webhook.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/webhook.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/webhook_collection.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/webhook_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/webhook_dispatch.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/webhook_dispatch.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/clients/resource_clients/webhook_dispatch_collection.py` & `apify_client-1.2.1b1/src/apify_client/clients/resource_clients/webhook_dispatch_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client/consts.py` & `apify_client-1.2.1b1/src/apify_client/consts.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client.egg-info/PKG-INFO` & `apify_client-1.2.1b1/src/apify_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify-client
-Version: 1.2.0b2
+Version: 1.2.1b1
 Summary: Apify API client for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/api/client/python/
 Project-URL: Documentation, https://docs.apify.com/api/client/python/
 Project-URL: Source, https://github.com/apify/apify-client-python
 Project-URL: Issue tracker, https://github.com/apify/apify-client-python/issues
```

### Comparing `apify_client-1.2.0b2/src/apify_client.egg-info/SOURCES.txt` & `apify_client-1.2.1b1/src/apify_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apify_client-1.2.0b2/src/apify_client.egg-info/requires.txt` & `apify_client-1.2.1b1/src/apify_client.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-httpx~=0.24.1
+httpx>=0.24.1
 
 [dev]
 autopep8~=2.0.2
 build~=0.10.0
 flake8~=6.0.0
 flake8-bugbear~=23.5.9
 flake8-commas~=2.1.0
```

