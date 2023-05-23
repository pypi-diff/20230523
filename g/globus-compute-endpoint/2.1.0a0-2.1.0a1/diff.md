# Comparing `tmp/globus-compute-endpoint-2.1.0a0.tar.gz` & `tmp/globus-compute-endpoint-2.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-endpoint-2.1.0a0.tar", last modified: Tue May 23 18:43:57 2023, max compression
+gzip compressed data, was "globus-compute-endpoint-2.1.0a1.tar", last modified: Tue May 23 18:47:21 2023, max compression
```

## Comparing `globus-compute-endpoint-2.1.0a0.tar` & `globus-compute-endpoint-2.1.0a1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:57.362364 globus-compute-endpoint-2.1.0a0/
--rw-rw-r--   0 reid      (1000) reid      (1000)    11330 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/LICENSE
--rw-rw-r--   0 reid      (1000) reid      (1000)       16 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/MANIFEST.in
--rw-rw-rw-   0 reid      (1000) reid      (1000)     1840 2023-05-23 18:43:57.362364 globus-compute-endpoint-2.1.0a0/PKG-INFO
--rw-rw-r--   0 reid      (1000) reid      (1000)      871 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/PyPI.md
-drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:57.350364 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/
--rw-rw-r--   0 reid      (1000) reid      (1000)      131 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    19439 2023-05-23 18:23:02.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/cli.py
-drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:57.350364 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/
--rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     2895 2023-05-22 19:56:07.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/config.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      772 2023-05-22 19:56:07.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/default_config.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    28831 2023-05-23 18:23:02.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/endpoint.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    19658 2023-05-22 19:56:07.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/endpoint_manager.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    24838 2023-05-22 19:56:07.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/interchange.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     2773 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/messages_compat.py
-drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:57.354364 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/rabbit_mq/
--rw-rw-r--   0 reid      (1000) reid      (1000)      307 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      689 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    11834 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     3068 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    14076 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     5184 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/result_store.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     7275 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/taskqueue.py
-drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:57.354364 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/utils/
--rw-rw-r--   0 reid      (1000) reid      (1000)     1017 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/utils/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     6129 2023-05-22 19:56:07.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/utils/config.py
-drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:57.354364 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/engines/
--rw-rw-r--   0 reid      (1000) reid      (1000)      318 2023-05-08 18:31:13.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/engines/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     5954 2023-05-08 18:31:13.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/engines/base.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     3721 2023-05-11 19:15:28.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/engines/globus_compute.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     4336 2023-05-08 18:31:13.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/engines/helper.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     3721 2023-05-11 19:15:28.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/engines/process_pool.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     3715 2023-05-11 19:15:28.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/engines/thread_pool.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     1834 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/exception_handling.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      220 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/exceptions.py
-drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:57.354364 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/
--rw-rw-r--   0 reid      (1000) reid      (1000)      141 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/__init__.py
-drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:57.358364 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/high_throughput/
--rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/high_throughput/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     1943 2023-05-01 20:50:52.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/high_throughput/container_sched.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    35357 2023-05-16 23:00:07.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/high_throughput/executor.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    50314 2023-05-11 19:15:28.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/high_throughput/interchange.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     9712 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      267 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
--rwxrwxr-x   0 reid      (1000) reid      (1000)    36129 2023-05-11 19:15:28.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/high_throughput/manager.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     9114 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/high_throughput/messages.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     8683 2023-04-20 18:06:21.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/high_throughput/worker.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    19094 2023-05-01 20:50:52.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/high_throughput/worker_map.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     5433 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     8219 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/logging_config.py
-drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:57.358364 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/providers/
--rw-rw-r--   0 reid      (1000) reid      (1000)      115 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/providers/__init__.py
-drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:57.358364 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/providers/kubernetes/
--rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/providers/kubernetes/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    12926 2023-05-01 20:50:52.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/providers/kubernetes/kube.py
--rw-rw-r--   0 reid      (1000) reid      (1000)       50 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/providers/kubernetes/template.py
-drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:57.362364 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/strategies/
--rw-rw-r--   0 reid      (1000) reid      (1000)      280 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/strategies/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     7018 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/strategies/base.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     5470 2023-05-01 20:50:52.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/strategies/kube_simple.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     6145 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/strategies/simple.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     1610 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/strategies/test.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      806 2023-05-23 18:27:39.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/version.py
-drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:57.350364 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint.egg-info/
--rw-rw-r--   0 reid      (1000) reid      (1000)     1840 2023-05-23 18:43:57.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint.egg-info/PKG-INFO
--rw-rw-r--   0 reid      (1000) reid      (1000)     2928 2023-05-23 18:43:57.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint.egg-info/SOURCES.txt
--rw-rw-r--   0 reid      (1000) reid      (1000)        1 2023-05-23 18:43:57.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint.egg-info/dependency_links.txt
--rw-rw-r--   0 reid      (1000) reid      (1000)      359 2023-05-23 18:43:57.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint.egg-info/entry_points.txt
--rw-rw-r--   0 reid      (1000) reid      (1000)      306 2023-05-23 18:43:57.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint.egg-info/requires.txt
--rw-rw-r--   0 reid      (1000) reid      (1000)       30 2023-05-23 18:43:57.000000 globus-compute-endpoint-2.1.0a0/globus_compute_endpoint.egg-info/top_level.txt
--rw-rw-r--   0 reid      (1000) reid      (1000)      282 2023-05-23 18:43:57.362364 globus-compute-endpoint-2.1.0a0/setup.cfg
--rw-rw-r--   0 reid      (1000) reid      (1000)     3633 2023-05-11 19:15:28.000000 globus-compute-endpoint-2.1.0a0/setup.py
-drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:57.362364 globus-compute-endpoint-2.1.0a0/tests/
--rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a0/tests/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     2709 2023-05-01 20:50:52.000000 globus-compute-endpoint-2.1.0a0/tests/conftest.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     2925 2023-05-08 18:31:13.000000 globus-compute-endpoint-2.1.0a0/tests/utils.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.543599 globus-compute-endpoint-2.1.0a1/
+-rw-rw-r--   0 reid      (1000) reid      (1000)    11330 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/LICENSE
+-rw-rw-r--   0 reid      (1000) reid      (1000)       16 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/MANIFEST.in
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1840 2023-05-23 18:47:21.543599 globus-compute-endpoint-2.1.0a1/PKG-INFO
+-rw-rw-r--   0 reid      (1000) reid      (1000)      871 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/PyPI.md
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.535599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      131 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    19439 2023-05-23 18:23:02.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/cli.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.535599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     2895 2023-05-22 19:56:07.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/config.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      772 2023-05-22 19:56:07.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/default_config.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    28831 2023-05-23 18:23:02.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/endpoint.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    19658 2023-05-22 19:56:07.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/endpoint_manager.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    24838 2023-05-22 19:56:07.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/interchange.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     2773 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/messages_compat.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.539599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/rabbit_mq/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      307 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      689 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/rabbit_mq/base.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    11834 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     3068 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    14076 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     5184 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/result_store.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     7275 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/taskqueue.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.539599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/utils/
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1017 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/utils/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     6129 2023-05-22 19:56:07.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/utils/config.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.539599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      318 2023-05-08 18:31:13.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     5954 2023-05-08 18:31:13.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/base.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     3721 2023-05-11 19:15:28.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/globus_compute.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     4336 2023-05-08 18:31:13.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/helper.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     3721 2023-05-11 19:15:28.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/process_pool.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     3715 2023-05-11 19:15:28.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/thread_pool.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1834 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/exception_handling.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      220 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/exceptions.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.539599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      141 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/__init__.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.539599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1943 2023-05-01 20:50:52.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/container_sched.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    35357 2023-05-16 23:00:07.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/executor.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    50314 2023-05-11 19:15:28.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/interchange.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     9712 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      267 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
+-rwxrwxr-x   0 reid      (1000) reid      (1000)    36129 2023-05-11 19:15:28.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/manager.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     9114 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/messages.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     8683 2023-04-20 18:06:21.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/worker.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    19094 2023-05-01 20:50:52.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/worker_map.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     5433 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     8219 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/logging_config.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.539599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/providers/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      115 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/providers/__init__.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.543599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/providers/kubernetes/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/providers/kubernetes/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    12926 2023-05-01 20:50:52.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/providers/kubernetes/kube.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)       50 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/providers/kubernetes/template.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.543599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/strategies/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      280 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/strategies/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     7018 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/strategies/base.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     5470 2023-05-01 20:50:52.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/strategies/kube_simple.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     6145 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/strategies/simple.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1610 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/strategies/test.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      806 2023-05-23 18:46:22.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/version.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.535599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint.egg-info/
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1840 2023-05-23 18:47:21.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint.egg-info/PKG-INFO
+-rw-rw-r--   0 reid      (1000) reid      (1000)     2928 2023-05-23 18:47:21.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint.egg-info/SOURCES.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)        1 2023-05-23 18:47:21.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint.egg-info/dependency_links.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)      359 2023-05-23 18:47:21.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint.egg-info/entry_points.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)      308 2023-05-23 18:47:21.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint.egg-info/requires.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)       30 2023-05-23 18:47:21.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint.egg-info/top_level.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)      282 2023-05-23 18:47:21.543599 globus-compute-endpoint-2.1.0a1/setup.cfg
+-rw-rw-r--   0 reid      (1000) reid      (1000)     3635 2023-05-23 18:46:19.000000 globus-compute-endpoint-2.1.0a1/setup.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.543599 globus-compute-endpoint-2.1.0a1/tests/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/tests/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     2709 2023-05-01 20:50:52.000000 globus-compute-endpoint-2.1.0a1/tests/conftest.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     2925 2023-05-08 18:31:13.000000 globus-compute-endpoint-2.1.0a1/tests/utils.py
```

### Comparing `globus-compute-endpoint-2.1.0a0/LICENSE` & `globus-compute-endpoint-2.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/PKG-INFO` & `globus-compute-endpoint-2.1.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.1.0a0
+Version: 2.1.0a1
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-endpoint-2.1.0a0/PyPI.md` & `globus-compute-endpoint-2.1.0a1/PyPI.md`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/cli.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/cli.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/config.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/default_config.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/default_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/endpoint.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/endpoint_manager.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/interchange.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/messages_compat.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/messages_compat.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/rabbit_mq/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/result_store.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/result_store.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/taskqueue.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/taskqueue.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/utils/__init__.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/endpoint/utils/config.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/utils/config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/engines/base.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/engines/globus_compute.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/globus_compute.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/engines/helper.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/helper.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/engines/process_pool.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/process_pool.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/engines/thread_pool.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/thread_pool.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/exception_handling.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/exception_handling.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/high_throughput/container_sched.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/container_sched.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/high_throughput/executor.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/executor.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/high_throughput/interchange.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/high_throughput/manager.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/high_throughput/messages.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/messages.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/high_throughput/worker.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/worker.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/high_throughput/worker_map.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/worker_map.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/logging_config.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/logging_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/providers/kubernetes/kube.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/strategies/base.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/strategies/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/strategies/kube_simple.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/strategies/kube_simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/strategies/simple.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/strategies/simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/strategies/test.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/strategies/test.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint/version.py` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.1.0a0"
+__version__ = "2.1.0a1"
 
 # TODO: remove after a `globus-compute-sdk` release
 # this is needed because it's imported by `globus-compute-sdk` to do the version check
 VERSION = __version__
 
 # Here as it's the easier way for funcx-endpoint cli to display it
 DEPRECATION_FUNCX_ENDPOINT = """
```

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint.egg-info/PKG-INFO` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.1.0a0
+Version: 2.1.0a1
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-endpoint-2.1.0a0/globus_compute_endpoint.egg-info/SOURCES.txt` & `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/setup.py` & `globus-compute-endpoint-2.1.0a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
     "requests>=2.20.0,<3",
     "globus-sdk",  # version will be bounded by `globus-compute-sdk`
-    "globus-compute-sdk==2.0.3",
+    "globus-compute-sdk==2.1.0a1",
     "globus-compute-common==0.2.0",
     # table printing used in list-endpoints
     "texttable>=1.6.4,<2",
     # although psutil does not declare itself to use semver, it appears to offer
     # strong backwards-compatibility promises based on its changelog, usage, and
     # history
     #
```

### Comparing `globus-compute-endpoint-2.1.0a0/tests/conftest.py` & `globus-compute-endpoint-2.1.0a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a0/tests/utils.py` & `globus-compute-endpoint-2.1.0a1/tests/utils.py`

 * *Files identical despite different names*

