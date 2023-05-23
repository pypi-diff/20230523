# Comparing `tmp/armonik-3.8.2.dev345.tar.gz` & `tmp/armonik-3.8.2.dev349.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "armonik-3.8.2.dev345.tar", last modified: Wed May 17 14:43:00 2023, max compression
+gzip compressed data, was "armonik-3.8.2.dev349.tar", last modified: Tue May 23 12:25:29 2023, max compression
```

## Comparing `armonik-3.8.2.dev345.tar` & `armonik-3.8.2.dev349.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:43:00.385304 armonik-3.8.2.dev345/
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-17 14:43:00.385304 armonik-3.8.2.dev345/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-17 14:42:43.000000 armonik-3.8.2.dev345/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-17 14:42:43.000000 armonik-3.8.2.dev345/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 14:43:00.385304 armonik-3.8.2.dev345/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:43:00.373304 armonik-3.8.2.dev345/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:43:00.373304 armonik-3.8.2.dev345/src/armonik/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-17 14:42:43.000000 armonik-3.8.2.dev345/src/armonik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:43:00.373304 armonik-3.8.2.dev345/src/armonik/client/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-17 14:42:43.000000 armonik-3.8.2.dev345/src/armonik/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-05-17 14:42:43.000000 armonik-3.8.2.dev345/src/armonik/client/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-17 14:42:43.000000 armonik-3.8.2.dev345/src/armonik/client/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:43:00.373304 armonik-3.8.2.dev345/src/armonik/common/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-17 14:42:43.000000 armonik-3.8.2.dev345/src/armonik/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-17 14:42:43.000000 armonik-3.8.2.dev345/src/armonik/common/enumwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-17 14:42:43.000000 armonik-3.8.2.dev345/src/armonik/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-17 14:42:43.000000 armonik-3.8.2.dev345/src/armonik/common/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:43:00.373304 armonik-3.8.2.dev345/src/armonik/protogen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:43:00.377303 armonik-3.8.2.dev345/src/armonik/protogen/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/applications_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/applications_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/applications_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/auth_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/auth_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/auth_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/events_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/events_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/events_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/partitions_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/partitions_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/partitions_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/results_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/results_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/results_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/sessions_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/sessions_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/sessions_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/submitter_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/submitter_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27332 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/submitter_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/tasks_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/tasks_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/client/tasks_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:43:00.381304 armonik-3.8.2.dev345/src/armonik/protogen/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/agent_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/agent_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/agent_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/applications_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/applications_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/applications_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/auth_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/auth_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/auth_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/events_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/events_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/events_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/objects_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/objects_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/objects_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/partitions_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/partitions_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/partitions_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/result_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/result_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/result_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/results_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/results_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/results_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/session_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/session_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/session_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/sessions_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/sessions_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/sessions_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/submitter_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/submitter_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/submitter_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/task_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/task_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/task_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/tasks_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15628 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/tasks_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/tasks_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/worker_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/worker_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/common/worker_common_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:43:00.381304 armonik-3.8.2.dev345/src/armonik/protogen/worker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/worker/agent_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/worker/agent_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/worker/agent_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/worker/worker_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/worker/worker_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-17 14:42:54.000000 armonik-3.8.2.dev345/src/armonik/protogen/worker/worker_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:43:00.381304 armonik-3.8.2.dev345/src/armonik/worker/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-17 14:42:43.000000 armonik-3.8.2.dev345/src/armonik/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-17 14:42:43.000000 armonik-3.8.2.dev345/src/armonik/worker/seqlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-17 14:42:43.000000 armonik-3.8.2.dev345/src/armonik/worker/taskhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-17 14:42:43.000000 armonik-3.8.2.dev345/src/armonik/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:43:00.373304 armonik-3.8.2.dev345/src/armonik.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-17 14:43:00.000000 armonik-3.8.2.dev345/src/armonik.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-17 14:43:00.000000 armonik-3.8.2.dev345/src/armonik.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:43:00.000000 armonik-3.8.2.dev345/src/armonik.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-17 14:43:00.000000 armonik-3.8.2.dev345/src/armonik.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 14:43:00.000000 armonik-3.8.2.dev345/src/armonik.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:25:29.040168 armonik-3.8.2.dev349/
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-23 12:25:29.040168 armonik-3.8.2.dev349/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-23 12:25:09.000000 armonik-3.8.2.dev349/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-23 12:25:09.000000 armonik-3.8.2.dev349/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 12:25:29.040168 armonik-3.8.2.dev349/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:25:29.024168 armonik-3.8.2.dev349/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:25:29.028168 armonik-3.8.2.dev349/src/armonik/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 12:25:09.000000 armonik-3.8.2.dev349/src/armonik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-23 12:25:22.000000 armonik-3.8.2.dev349/src/armonik/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:25:29.028168 armonik-3.8.2.dev349/src/armonik/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-23 12:25:09.000000 armonik-3.8.2.dev349/src/armonik/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-05-23 12:25:09.000000 armonik-3.8.2.dev349/src/armonik/client/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-23 12:25:09.000000 armonik-3.8.2.dev349/src/armonik/client/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:25:29.028168 armonik-3.8.2.dev349/src/armonik/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-23 12:25:09.000000 armonik-3.8.2.dev349/src/armonik/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-23 12:25:09.000000 armonik-3.8.2.dev349/src/armonik/common/enumwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-23 12:25:09.000000 armonik-3.8.2.dev349/src/armonik/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-23 12:25:09.000000 armonik-3.8.2.dev349/src/armonik/common/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:25:29.024168 armonik-3.8.2.dev349/src/armonik/protogen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:25:29.032168 armonik-3.8.2.dev349/src/armonik/protogen/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/applications_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/applications_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/applications_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/auth_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/auth_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/auth_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/events_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/events_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/events_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/partitions_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/partitions_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/partitions_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/results_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/results_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/results_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/sessions_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/sessions_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/sessions_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/submitter_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/submitter_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27332 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/submitter_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/tasks_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/tasks_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/client/tasks_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:25:29.040168 armonik-3.8.2.dev349/src/armonik/protogen/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/agent_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/agent_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/agent_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/applications_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/applications_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/applications_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/auth_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/auth_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/auth_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/events_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/events_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/events_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/objects_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/objects_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/objects_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/partitions_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/partitions_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/partitions_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/result_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/result_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/result_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/results_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/results_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/results_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/session_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/session_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/session_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/sessions_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/sessions_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/sessions_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/submitter_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/submitter_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/submitter_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/task_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/task_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/task_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/tasks_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/tasks_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/tasks_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/worker_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/worker_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/common/worker_common_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:25:29.040168 armonik-3.8.2.dev349/src/armonik/protogen/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/worker/agent_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/worker/agent_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/worker/agent_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/worker/worker_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/worker/worker_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-23 12:25:21.000000 armonik-3.8.2.dev349/src/armonik/protogen/worker/worker_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:25:29.040168 armonik-3.8.2.dev349/src/armonik/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 12:25:09.000000 armonik-3.8.2.dev349/src/armonik/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-23 12:25:09.000000 armonik-3.8.2.dev349/src/armonik/worker/seqlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-23 12:25:09.000000 armonik-3.8.2.dev349/src/armonik/worker/taskhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-23 12:25:09.000000 armonik-3.8.2.dev349/src/armonik/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:25:29.028168 armonik-3.8.2.dev349/src/armonik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-23 12:25:29.000000 armonik-3.8.2.dev349/src/armonik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-23 12:25:29.000000 armonik-3.8.2.dev349/src/armonik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:25:29.000000 armonik-3.8.2.dev349/src/armonik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-23 12:25:29.000000 armonik-3.8.2.dev349/src/armonik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 12:25:29.000000 armonik-3.8.2.dev349/src/armonik.egg-info/top_level.txt
```

### Comparing `armonik-3.8.2.dev345/PKG-INFO` & `armonik-3.8.2.dev349/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armonik
-Version: 3.8.2.dev345
+Version: 3.8.2.dev349
 Summary: GRPC python binding for the ArmoniK orchestrator API
 License: Apache v2.0 LICENSE
 Project-URL: Homepage, https://github.com/aneoconsulting/ArmoniK.Api
 Project-URL: Bug Tracker, https://github.com/aneoconsulting/ArmoniK/issues
 Keywords: cloud,HTC,gRPC,ArmoniK,Aneo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `armonik-3.8.2.dev345/README.md` & `armonik-3.8.2.dev349/README.md`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev345/pyproject.toml` & `armonik-3.8.2.dev349/pyproject.toml`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev345/src/armonik/client/submitter.py` & `armonik-3.8.2.dev349/src/armonik/client/submitter.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev345/src/armonik/client/tasks.py` & `armonik-3.8.2.dev349/src/armonik/client/tasks.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev345/src/armonik/common/enumwrapper.py` & `armonik-3.8.2.dev349/src/armonik/common/enumwrapper.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev345/src/armonik/common/helpers.py` & `armonik-3.8.2.dev349/src/armonik/common/helpers.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev345/src/armonik/common/objects.py` & `armonik-3.8.2.dev349/src/armonik/common/objects.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/client/applications_service_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/client/applications_service_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: applications_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ..common import applications_common_pb2 as applications__common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x61pplications_service.proto\x12 armonik.api.grpc.v1.applications\x1a\x19\x61pplications_common.proto2\xb0\x02\n\x0c\x41pplications\x12\x8b\x01\n\x10ListApplications\x12\x39.armonik.api.grpc.v1.applications.ListApplicationsRequest\x1a:.armonik.api.grpc.v1.applications.ListApplicationsResponse\"\x00\x12\x91\x01\n\x12\x43ountTasksByStatus\x12;.armonik.api.grpc.v1.applications.CountTasksByStatusRequest\x1a<.armonik.api.grpc.v1.applications.CountTasksByStatusResponse\"\x00\x42#\xaa\x02 ArmoniK.Api.gRPC.V1.Applicationsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'applications_service_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'applications_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002 ArmoniK.Api.gRPC.V1.Applications'
-  _APPLICATIONS._serialized_start=92
-  _APPLICATIONS._serialized_end=396
+  _globals['_APPLICATIONS']._serialized_start=92
+  _globals['_APPLICATIONS']._serialized_end=396
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/client/applications_service_pb2_grpc.py` & `armonik-3.8.2.dev349/src/armonik/protogen/client/applications_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/client/auth_service_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/client/auth_service_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: auth_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ..common import auth_common_pb2 as auth__common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x61uth_service.proto\x12\x18\x61rmonik.api.grpc.v1.auth\x1a\x11\x61uth_common.proto2\x87\x01\n\x0e\x41uthentication\x12u\n\x0eGetCurrentUser\x12/.armonik.api.grpc.v1.auth.GetCurrentUserRequest\x1a\x30.armonik.api.grpc.v1.auth.GetCurrentUserResponse\"\x00\x42\x1b\xaa\x02\x18\x41rmoniK.Api.gRPC.V1.Authb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'auth_service_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'auth_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\030ArmoniK.Api.gRPC.V1.Auth'
-  _AUTHENTICATION._serialized_start=68
-  _AUTHENTICATION._serialized_end=203
+  _globals['_AUTHENTICATION']._serialized_start=68
+  _globals['_AUTHENTICATION']._serialized_end=203
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/client/auth_service_pb2_grpc.py` & `armonik-3.8.2.dev349/src/armonik/protogen/client/auth_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/client/events_service_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/client/events_service_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: events_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ..common import events_common_pb2 as events__common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x65vents_service.proto\x12\x1a\x61rmonik.api.grpc.v1.events\x1a\x13\x65vents_common.proto2\x84\x01\n\x06\x45vents\x12z\n\tGetEvents\x12\x34.armonik.api.grpc.v1.events.EventSubscriptionRequest\x1a\x35.armonik.api.grpc.v1.events.EventSubscriptionResponse0\x01\x42\x1d\xaa\x02\x1a\x41rmoniK.Api.gRPC.V1.Eventsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'events_service_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'events_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\032ArmoniK.Api.gRPC.V1.Events'
-  _EVENTS._serialized_start=74
-  _EVENTS._serialized_end=206
+  _globals['_EVENTS']._serialized_start=74
+  _globals['_EVENTS']._serialized_end=206
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/client/events_service_pb2_grpc.py` & `armonik-3.8.2.dev349/src/armonik/protogen/client/events_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/client/partitions_service_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/client/partitions_service_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: partitions_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ..common import partitions_common_pb2 as partitions__common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18partitions_service.proto\x12\x1e\x61rmonik.api.grpc.v1.partitions\x1a\x17partitions_common.proto2\x8d\x02\n\nPartitions\x12\x81\x01\n\x0eListPartitions\x12\x35.armonik.api.grpc.v1.partitions.ListPartitionsRequest\x1a\x36.armonik.api.grpc.v1.partitions.ListPartitionsResponse\"\x00\x12{\n\x0cGetPartition\x12\x33.armonik.api.grpc.v1.partitions.GetPartitionRequest\x1a\x34.armonik.api.grpc.v1.partitions.GetPartitionResponse\"\x00\x42!\xaa\x02\x1e\x41rmonik.Api.Grpc.V1.Partitionsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'partitions_service_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'partitions_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\036Armonik.Api.Grpc.V1.Partitions'
-  _PARTITIONS._serialized_start=86
-  _PARTITIONS._serialized_end=355
+  _globals['_PARTITIONS']._serialized_start=86
+  _globals['_PARTITIONS']._serialized_end=355
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/client/partitions_service_pb2_grpc.py` & `armonik-3.8.2.dev349/src/armonik/protogen/client/partitions_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/client/results_service_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/client/results_service_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: results_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ..common import objects_pb2 as objects__pb2
 from ..common import results_common_pb2 as results__common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15results_service.proto\x12\x1b\x61rmonik.api.grpc.v1.results\x1a\robjects.proto\x1a\x14results_common.proto2\x97\x08\n\x07Results\x12r\n\x0bListResults\x12/.armonik.api.grpc.v1.results.ListResultsRequest\x1a\x30.armonik.api.grpc.v1.results.ListResultsResponse\"\x00\x12y\n\x0eGetOwnerTaskId\x12\x32.armonik.api.grpc.v1.results.GetOwnerTaskIdRequest\x1a\x33.armonik.api.grpc.v1.results.GetOwnerTaskIdResponse\x12\x90\x01\n\x15\x43reateResultsMetaData\x12\x39.armonik.api.grpc.v1.results.CreateResultsMetaDataRequest\x1a:.armonik.api.grpc.v1.results.CreateResultsMetaDataResponse\"\x00\x12x\n\rCreateResults\x12\x31.armonik.api.grpc.v1.results.CreateResultsRequest\x1a\x32.armonik.api.grpc.v1.results.CreateResultsResponse\"\x00\x12\x83\x01\n\x10UploadResultData\x12\x34.armonik.api.grpc.v1.results.UploadResultDataRequest\x1a\x35.armonik.api.grpc.v1.results.UploadResultDataResponse\"\x00(\x01\x12\x89\x01\n\x12\x44ownloadResultData\x12\x36.armonik.api.grpc.v1.results.DownloadResultDataRequest\x1a\x37.armonik.api.grpc.v1.results.DownloadResultDataResponse\"\x00\x30\x01\x12\x84\x01\n\x11\x44\x65leteResultsData\x12\x35.armonik.api.grpc.v1.results.DeleteResultsDataRequest\x1a\x36.armonik.api.grpc.v1.results.DeleteResultsDataResponse\"\x00\x12w\n\x17GetServiceConfiguration\x12\x1a.armonik.api.grpc.v1.Empty\x1a@.armonik.api.grpc.v1.results.ResultsServiceConfigurationResponseB\x1e\xaa\x02\x1b\x41rmoniK.Api.gRPC.V1.Resultsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'results_service_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'results_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\033ArmoniK.Api.gRPC.V1.Results'
-  _RESULTS._serialized_start=92
-  _RESULTS._serialized_end=1139
+  _globals['_RESULTS']._serialized_start=92
+  _globals['_RESULTS']._serialized_end=1139
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/client/results_service_pb2_grpc.py` & `armonik-3.8.2.dev349/src/armonik/protogen/client/results_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/client/sessions_service_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/client/sessions_service_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: sessions_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ..common import sessions_common_pb2 as sessions__common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16sessions_service.proto\x12\x1c\x61rmonik.api.grpc.v1.sessions\x1a\x15sessions_common.proto2\xfc\x03\n\x08Sessions\x12u\n\x0cListSessions\x12\x31.armonik.api.grpc.v1.sessions.ListSessionsRequest\x1a\x32.armonik.api.grpc.v1.sessions.ListSessionsResponse\x12q\n\nGetSession\x12/.armonik.api.grpc.v1.sessions.GetSessionRequest\x1a\x30.armonik.api.grpc.v1.sessions.GetSessionResponse\"\x00\x12z\n\rCancelSession\x12\x32.armonik.api.grpc.v1.sessions.CancelSessionRequest\x1a\x33.armonik.api.grpc.v1.sessions.CancelSessionResponse\"\x00\x12\x89\x01\n\x12\x43ountTasksByStatus\x12\x37.armonik.api.grpc.v1.sessions.CountTasksByStatusRequest\x1a\x38.armonik.api.grpc.v1.sessions.CountTasksByStatusResponse\"\x00\x42\x1f\xaa\x02\x1c\x41rmoniK.Api.gRPC.V1.Sessionsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sessions_service_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sessions_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\034ArmoniK.Api.gRPC.V1.Sessions'
-  _SESSIONS._serialized_start=80
-  _SESSIONS._serialized_end=588
+  _globals['_SESSIONS']._serialized_start=80
+  _globals['_SESSIONS']._serialized_end=588
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/client/sessions_service_pb2_grpc.py` & `armonik-3.8.2.dev349/src/armonik/protogen/client/sessions_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/client/submitter_service_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/client/submitter_service_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: submitter_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ..common import objects_pb2 as objects__pb2
 from ..common import submitter_common_pb2 as submitter__common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17submitter_service.proto\x12\x1d\x61rmonik.api.grpc.v1.submitter\x1a\robjects.proto\x1a\x16submitter_common.proto2\x99\r\n\tSubmitter\x12Y\n\x17GetServiceConfiguration\x12\x1a.armonik.api.grpc.v1.Empty\x1a\".armonik.api.grpc.v1.Configuration\x12w\n\rCreateSession\x12\x33.armonik.api.grpc.v1.submitter.CreateSessionRequest\x1a\x31.armonik.api.grpc.v1.submitter.CreateSessionReply\x12I\n\rCancelSession\x12\x1c.armonik.api.grpc.v1.Session\x1a\x1a.armonik.api.grpc.v1.Empty\x12y\n\x10\x43reateSmallTasks\x12\x35.armonik.api.grpc.v1.submitter.CreateSmallTaskRequest\x1a..armonik.api.grpc.v1.submitter.CreateTaskReply\x12{\n\x10\x43reateLargeTasks\x12\x35.armonik.api.grpc.v1.submitter.CreateLargeTaskRequest\x1a..armonik.api.grpc.v1.submitter.CreateTaskReply(\x01\x12W\n\tListTasks\x12).armonik.api.grpc.v1.submitter.TaskFilter\x1a\x1f.armonik.api.grpc.v1.TaskIdList\x12j\n\x0cListSessions\x12,.armonik.api.grpc.v1.submitter.SessionFilter\x1a,.armonik.api.grpc.v1.submitter.SessionIdList\x12S\n\nCountTasks\x12).armonik.api.grpc.v1.submitter.TaskFilter\x1a\x1a.armonik.api.grpc.v1.Count\x12\x66\n\x12TryGetResultStream\x12\".armonik.api.grpc.v1.ResultRequest\x1a*.armonik.api.grpc.v1.submitter.ResultReply0\x01\x12W\n\x10TryGetTaskOutput\x12&.armonik.api.grpc.v1.TaskOutputRequest\x1a\x1b.armonik.api.grpc.v1.Output\x12p\n\x13WaitForAvailability\x12\".armonik.api.grpc.v1.ResultRequest\x1a\x30.armonik.api.grpc.v1.submitter.AvailabilityReply\"\x03\x88\x02\x01\x12[\n\x11WaitForCompletion\x12*.armonik.api.grpc.v1.submitter.WaitRequest\x1a\x1a.armonik.api.grpc.v1.Count\x12T\n\x0b\x43\x61ncelTasks\x12).armonik.api.grpc.v1.submitter.TaskFilter\x1a\x1a.armonik.api.grpc.v1.Empty\x12w\n\rGetTaskStatus\x12\x33.armonik.api.grpc.v1.submitter.GetTaskStatusRequest\x1a\x31.armonik.api.grpc.v1.submitter.GetTaskStatusReply\x12\x82\x01\n\x0fGetResultStatus\x12\x35.armonik.api.grpc.v1.submitter.GetResultStatusRequest\x1a\x33.armonik.api.grpc.v1.submitter.GetResultStatusReply\"\x03\x88\x02\x01\x12w\n\x0cWatchResults\x12\x31.armonik.api.grpc.v1.submitter.WatchResultRequest\x1a\x30.armonik.api.grpc.v1.submitter.WatchResultStream(\x01\x30\x01\x42 \xaa\x02\x1d\x41rmoniK.Api.gRPC.V1.Submitterb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'submitter_service_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'submitter_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\035ArmoniK.Api.gRPC.V1.Submitter'
   _SUBMITTER.methods_by_name['WaitForAvailability']._options = None
   _SUBMITTER.methods_by_name['WaitForAvailability']._serialized_options = b'\210\002\001'
   _SUBMITTER.methods_by_name['GetResultStatus']._options = None
   _SUBMITTER.methods_by_name['GetResultStatus']._serialized_options = b'\210\002\001'
-  _SUBMITTER._serialized_start=98
-  _SUBMITTER._serialized_end=1787
+  _globals['_SUBMITTER']._serialized_start=98
+  _globals['_SUBMITTER']._serialized_end=1787
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/client/submitter_service_pb2_grpc.py` & `armonik-3.8.2.dev349/src/armonik/protogen/client/submitter_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/client/tasks_service_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/client/tasks_service_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: tasks_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ..common import tasks_common_pb2 as tasks__common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13tasks_service.proto\x12\x19\x61rmonik.api.grpc.v1.tasks\x1a\x12tasks_common.proto2\x9c\x06\n\x05Tasks\x12h\n\tListTasks\x12+.armonik.api.grpc.v1.tasks.ListTasksRequest\x1a,.armonik.api.grpc.v1.tasks.ListTasksResponse\"\x00\x12n\n\x0cListTasksRaw\x12+.armonik.api.grpc.v1.tasks.ListTasksRequest\x1a/.armonik.api.grpc.v1.tasks.ListTasksRawResponse\"\x00\x12\x62\n\x07GetTask\x12).armonik.api.grpc.v1.tasks.GetTaskRequest\x1a*.armonik.api.grpc.v1.tasks.GetTaskResponse\"\x00\x12n\n\x0b\x43\x61ncelTasks\x12-.armonik.api.grpc.v1.tasks.CancelTasksRequest\x1a..armonik.api.grpc.v1.tasks.CancelTasksResponse\"\x00\x12o\n\x0cGetResultIds\x12..armonik.api.grpc.v1.tasks.GetResultIdsRequest\x1a/.armonik.api.grpc.v1.tasks.GetResultIdsResponse\x12\x83\x01\n\x12\x43ountTasksByStatus\x12\x34.armonik.api.grpc.v1.tasks.CountTasksByStatusRequest\x1a\x35.armonik.api.grpc.v1.tasks.CountTasksByStatusResponse\"\x00\x12n\n\x0bSubmitTasks\x12-.armonik.api.grpc.v1.tasks.SubmitTasksRequest\x1a..armonik.api.grpc.v1.tasks.SubmitTasksResponse\"\x00\x42\x1c\xaa\x02\x19\x41rmoniK.Api.gRPC.V1.Tasksb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tasks_service_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tasks_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\031ArmoniK.Api.gRPC.V1.Tasks'
-  _TASKS._serialized_start=71
-  _TASKS._serialized_end=867
+  _globals['_TASKS']._serialized_start=71
+  _globals['_TASKS']._serialized_end=867
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/client/tasks_service_pb2_grpc.py` & `armonik-3.8.2.dev349/src/armonik/protogen/client/tasks_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/agent_common_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/common/agent_common_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,77 +1,78 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: agent_common.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from . import objects_pb2 as objects__pb2
 from . import result_status_pb2 as result__status__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x61gent_common.proto\x12\x19\x61rmonik.api.grpc.v1.agent\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\robjects.proto\x1a\x13result_status.proto\"\xc4\x02\n\x11\x43reateTaskRequest\x12P\n\x0cinit_request\x18\x01 \x01(\x0b\x32\x38.armonik.api.grpc.v1.agent.CreateTaskRequest.InitRequestH\x00\x12\x39\n\tinit_task\x18\x02 \x01(\x0b\x32$.armonik.api.grpc.v1.InitTaskRequestH\x00\x12\x36\n\x0ctask_payload\x18\x03 \x01(\x0b\x32\x1e.armonik.api.grpc.v1.DataChunkH\x00\x12\x1b\n\x13\x63ommunication_token\x18\x04 \x01(\t\x1a\x45\n\x0bInitRequest\x12\x36\n\x0ctask_options\x18\x01 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptionsB\x06\n\x04type\"\xf7\x03\n\x0f\x43reateTaskReply\x12]\n\x14\x63reation_status_list\x18\x01 \x01(\x0b\x32=.armonik.api.grpc.v1.agent.CreateTaskReply.CreationStatusListH\x00\x12\x0f\n\x05\x65rror\x18\x02 \x01(\tH\x00\x12\x1b\n\x13\x63ommunication_token\x18\x04 \x01(\t\x1ah\n\x08TaskInfo\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x1c\n\x14\x65xpected_output_keys\x18\x02 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x03 \x03(\t\x12\x12\n\npayload_id\x18\x04 \x01(\t\x1au\n\x0e\x43reationStatus\x12H\n\ttask_info\x18\x01 \x01(\x0b\x32\x33.armonik.api.grpc.v1.agent.CreateTaskReply.TaskInfoH\x00\x12\x0f\n\x05\x65rror\x18\x02 \x01(\tH\x00\x42\x08\n\x06Status\x1aj\n\x12\x43reationStatusList\x12T\n\x11\x63reation_statuses\x18\x01 \x03(\x0b\x32\x39.armonik.api.grpc.v1.agent.CreateTaskReply.CreationStatusB\n\n\x08Response\"7\n\x0b\x44\x61taRequest\x12\x1b\n\x13\x63ommunication_token\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\"\x90\x02\n\tDataReply\x12\x1b\n\x13\x63ommunication_token\x18\x01 \x01(\t\x12\x39\n\x04init\x18\x02 \x01(\x0b\x32).armonik.api.grpc.v1.agent.DataReply.InitH\x00\x12.\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x1e.armonik.api.grpc.v1.DataChunkH\x00\x12\x0f\n\x05\x65rror\x18\x04 \x01(\tH\x00\x1a\x62\n\x04Init\x12\x0b\n\x03key\x18\x01 \x01(\t\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.armonik.api.grpc.v1.DataChunkH\x00\x12\x0f\n\x05\x65rror\x18\x03 \x01(\tH\x00\x42\x0c\n\nhas_resultB\x06\n\x04type\"\x97\x01\n\x06Result\x12\x38\n\x04init\x18\x01 \x01(\x0b\x32(.armonik.api.grpc.v1.InitKeyedDataStreamH\x00\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.armonik.api.grpc.v1.DataChunkH\x00\x12\x1b\n\x13\x63ommunication_token\x18\x03 \x01(\tB\x06\n\x04type\"m\n\x0bResultReply\x12\x1b\n\x13\x63ommunication_token\x18\x03 \x01(\t\x12(\n\x02Ok\x18\x01 \x01(\x0b\x32\x1a.armonik.api.grpc.v1.EmptyH\x00\x12\x0f\n\x05\x45rror\x18\x02 \x01(\tH\x00\x42\x06\n\x04type\"\xc4\x01\n\x1c\x43reateResultsMetaDataRequest\x12U\n\x07results\x18\x01 \x03(\x0b\x32\x44.armonik.api.grpc.v1.agent.CreateResultsMetaDataRequest.ResultCreate\x12\x12\n\nsession_id\x18\x02 \x01(\t\x12\x1b\n\x13\x63ommunication_token\x18\x03 \x01(\t\x1a\x1c\n\x0cResultCreate\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xb6\x01\n\x0eResultMetaData\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12?\n\x06status\x18\x04 \x01(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"x\n\x1d\x43reateResultsMetaDataResponse\x12:\n\x07results\x18\x01 \x03(\x0b\x32).armonik.api.grpc.v1.agent.ResultMetaData\x12\x1b\n\x13\x63ommunication_token\x18\x02 \x01(\t\"\xe7\x02\n\x12SubmitTasksRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x36\n\x0ctask_options\x18\x02 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12R\n\x0etask_creations\x18\x03 \x03(\x0b\x32:.armonik.api.grpc.v1.agent.SubmitTasksRequest.TaskCreation\x12\x1b\n\x13\x63ommunication_token\x18\x04 \x01(\t\x1a\x93\x01\n\x0cTaskCreation\x12\x1c\n\x14\x65xpected_output_keys\x18\x01 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x02 \x03(\t\x12\x12\n\npayload_id\x18\x03 \x01(\t\x12\x36\n\x0ctask_options\x18\x04 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\"\xe8\x01\n\x13SubmitTasksResponse\x12K\n\ntask_infos\x18\x01 \x03(\x0b\x32\x37.armonik.api.grpc.v1.agent.SubmitTasksResponse.TaskInfo\x12\x1b\n\x13\x63ommunication_token\x18\x02 \x01(\t\x1ag\n\x08TaskInfo\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x1b\n\x13\x65xpected_output_ids\x18\x02 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x03 \x03(\t\x12\x12\n\npayload_id\x18\x04 \x01(\t\"\xc2\x01\n\x14\x43reateResultsRequest\x12M\n\x07results\x18\x01 \x03(\x0b\x32<.armonik.api.grpc.v1.agent.CreateResultsRequest.ResultCreate\x12\x12\n\nsession_id\x18\x02 \x01(\t\x12\x1b\n\x13\x63ommunication_token\x18\x03 \x01(\t\x1a*\n\x0cResultCreate\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"p\n\x15\x43reateResultsResponse\x12:\n\x07results\x18\x01 \x03(\x0b\x32).armonik.api.grpc.v1.agent.ResultMetaData\x12\x1b\n\x13\x63ommunication_token\x18\x02 \x01(\t\"\xe2\x01\n\x17UploadResultDataRequest\x12Q\n\x02id\x18\x01 \x01(\x0b\x32\x43.armonik.api.grpc.v1.agent.UploadResultDataRequest.ResultIdentifierH\x00\x12\x14\n\ndata_chunk\x18\x02 \x01(\x0cH\x00\x12\x1b\n\x13\x63ommunication_token\x18\x04 \x01(\t\x1a\x39\n\x10ResultIdentifier\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x01(\tB\x06\n\x04type\"J\n\x18UploadResultDataResponse\x12\x11\n\tresult_id\x18\x01 \x01(\t\x12\x1b\n\x13\x63ommunication_token\x18\x02 \x01(\tB\x1c\xaa\x02\x19\x41rmoniK.Api.gRPC.V1.Agentb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'agent_common_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'agent_common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\031ArmoniK.Api.gRPC.V1.Agent'
-  _CREATETASKREQUEST._serialized_start=119
-  _CREATETASKREQUEST._serialized_end=443
-  _CREATETASKREQUEST_INITREQUEST._serialized_start=366
-  _CREATETASKREQUEST_INITREQUEST._serialized_end=435
-  _CREATETASKREPLY._serialized_start=446
-  _CREATETASKREPLY._serialized_end=949
-  _CREATETASKREPLY_TASKINFO._serialized_start=606
-  _CREATETASKREPLY_TASKINFO._serialized_end=710
-  _CREATETASKREPLY_CREATIONSTATUS._serialized_start=712
-  _CREATETASKREPLY_CREATIONSTATUS._serialized_end=829
-  _CREATETASKREPLY_CREATIONSTATUSLIST._serialized_start=831
-  _CREATETASKREPLY_CREATIONSTATUSLIST._serialized_end=937
-  _DATAREQUEST._serialized_start=951
-  _DATAREQUEST._serialized_end=1006
-  _DATAREPLY._serialized_start=1009
-  _DATAREPLY._serialized_end=1281
-  _DATAREPLY_INIT._serialized_start=1175
-  _DATAREPLY_INIT._serialized_end=1273
-  _RESULT._serialized_start=1284
-  _RESULT._serialized_end=1435
-  _RESULTREPLY._serialized_start=1437
-  _RESULTREPLY._serialized_end=1546
-  _CREATERESULTSMETADATAREQUEST._serialized_start=1549
-  _CREATERESULTSMETADATAREQUEST._serialized_end=1745
-  _CREATERESULTSMETADATAREQUEST_RESULTCREATE._serialized_start=1717
-  _CREATERESULTSMETADATAREQUEST_RESULTCREATE._serialized_end=1745
-  _RESULTMETADATA._serialized_start=1748
-  _RESULTMETADATA._serialized_end=1930
-  _CREATERESULTSMETADATARESPONSE._serialized_start=1932
-  _CREATERESULTSMETADATARESPONSE._serialized_end=2052
-  _SUBMITTASKSREQUEST._serialized_start=2055
-  _SUBMITTASKSREQUEST._serialized_end=2414
-  _SUBMITTASKSREQUEST_TASKCREATION._serialized_start=2267
-  _SUBMITTASKSREQUEST_TASKCREATION._serialized_end=2414
-  _SUBMITTASKSRESPONSE._serialized_start=2417
-  _SUBMITTASKSRESPONSE._serialized_end=2649
-  _SUBMITTASKSRESPONSE_TASKINFO._serialized_start=2546
-  _SUBMITTASKSRESPONSE_TASKINFO._serialized_end=2649
-  _CREATERESULTSREQUEST._serialized_start=2652
-  _CREATERESULTSREQUEST._serialized_end=2846
-  _CREATERESULTSREQUEST_RESULTCREATE._serialized_start=2804
-  _CREATERESULTSREQUEST_RESULTCREATE._serialized_end=2846
-  _CREATERESULTSRESPONSE._serialized_start=2848
-  _CREATERESULTSRESPONSE._serialized_end=2960
-  _UPLOADRESULTDATAREQUEST._serialized_start=2963
-  _UPLOADRESULTDATAREQUEST._serialized_end=3189
-  _UPLOADRESULTDATAREQUEST_RESULTIDENTIFIER._serialized_start=3124
-  _UPLOADRESULTDATAREQUEST_RESULTIDENTIFIER._serialized_end=3181
-  _UPLOADRESULTDATARESPONSE._serialized_start=3191
-  _UPLOADRESULTDATARESPONSE._serialized_end=3265
+  _globals['_CREATETASKREQUEST']._serialized_start=119
+  _globals['_CREATETASKREQUEST']._serialized_end=443
+  _globals['_CREATETASKREQUEST_INITREQUEST']._serialized_start=366
+  _globals['_CREATETASKREQUEST_INITREQUEST']._serialized_end=435
+  _globals['_CREATETASKREPLY']._serialized_start=446
+  _globals['_CREATETASKREPLY']._serialized_end=949
+  _globals['_CREATETASKREPLY_TASKINFO']._serialized_start=606
+  _globals['_CREATETASKREPLY_TASKINFO']._serialized_end=710
+  _globals['_CREATETASKREPLY_CREATIONSTATUS']._serialized_start=712
+  _globals['_CREATETASKREPLY_CREATIONSTATUS']._serialized_end=829
+  _globals['_CREATETASKREPLY_CREATIONSTATUSLIST']._serialized_start=831
+  _globals['_CREATETASKREPLY_CREATIONSTATUSLIST']._serialized_end=937
+  _globals['_DATAREQUEST']._serialized_start=951
+  _globals['_DATAREQUEST']._serialized_end=1006
+  _globals['_DATAREPLY']._serialized_start=1009
+  _globals['_DATAREPLY']._serialized_end=1281
+  _globals['_DATAREPLY_INIT']._serialized_start=1175
+  _globals['_DATAREPLY_INIT']._serialized_end=1273
+  _globals['_RESULT']._serialized_start=1284
+  _globals['_RESULT']._serialized_end=1435
+  _globals['_RESULTREPLY']._serialized_start=1437
+  _globals['_RESULTREPLY']._serialized_end=1546
+  _globals['_CREATERESULTSMETADATAREQUEST']._serialized_start=1549
+  _globals['_CREATERESULTSMETADATAREQUEST']._serialized_end=1745
+  _globals['_CREATERESULTSMETADATAREQUEST_RESULTCREATE']._serialized_start=1717
+  _globals['_CREATERESULTSMETADATAREQUEST_RESULTCREATE']._serialized_end=1745
+  _globals['_RESULTMETADATA']._serialized_start=1748
+  _globals['_RESULTMETADATA']._serialized_end=1930
+  _globals['_CREATERESULTSMETADATARESPONSE']._serialized_start=1932
+  _globals['_CREATERESULTSMETADATARESPONSE']._serialized_end=2052
+  _globals['_SUBMITTASKSREQUEST']._serialized_start=2055
+  _globals['_SUBMITTASKSREQUEST']._serialized_end=2414
+  _globals['_SUBMITTASKSREQUEST_TASKCREATION']._serialized_start=2267
+  _globals['_SUBMITTASKSREQUEST_TASKCREATION']._serialized_end=2414
+  _globals['_SUBMITTASKSRESPONSE']._serialized_start=2417
+  _globals['_SUBMITTASKSRESPONSE']._serialized_end=2649
+  _globals['_SUBMITTASKSRESPONSE_TASKINFO']._serialized_start=2546
+  _globals['_SUBMITTASKSRESPONSE_TASKINFO']._serialized_end=2649
+  _globals['_CREATERESULTSREQUEST']._serialized_start=2652
+  _globals['_CREATERESULTSREQUEST']._serialized_end=2846
+  _globals['_CREATERESULTSREQUEST_RESULTCREATE']._serialized_start=2804
+  _globals['_CREATERESULTSREQUEST_RESULTCREATE']._serialized_end=2846
+  _globals['_CREATERESULTSRESPONSE']._serialized_start=2848
+  _globals['_CREATERESULTSRESPONSE']._serialized_end=2960
+  _globals['_UPLOADRESULTDATAREQUEST']._serialized_start=2963
+  _globals['_UPLOADRESULTDATAREQUEST']._serialized_end=3189
+  _globals['_UPLOADRESULTDATAREQUEST_RESULTIDENTIFIER']._serialized_start=3124
+  _globals['_UPLOADRESULTDATAREQUEST_RESULTIDENTIFIER']._serialized_end=3181
+  _globals['_UPLOADRESULTDATARESPONSE']._serialized_start=3191
+  _globals['_UPLOADRESULTDATARESPONSE']._serialized_end=3265
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/agent_common_pb2.pyi` & `armonik-3.8.2.dev349/src/armonik/protogen/common/agent_common_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,234 +4,234 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class CreateResultsMetaDataRequest(_message.Message):
-    __slots__ = ["communication_token", "results", "session_id"]
-    class ResultCreate(_message.Message):
-        __slots__ = ["name"]
-        NAME_FIELD_NUMBER: _ClassVar[int]
-        name: str
-        def __init__(self, name: _Optional[str] = ...) -> None: ...
-    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    RESULTS_FIELD_NUMBER: _ClassVar[int]
-    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-    communication_token: str
-    results: _containers.RepeatedCompositeFieldContainer[CreateResultsMetaDataRequest.ResultCreate]
-    session_id: str
-    def __init__(self, results: _Optional[_Iterable[_Union[CreateResultsMetaDataRequest.ResultCreate, _Mapping]]] = ..., session_id: _Optional[str] = ..., communication_token: _Optional[str] = ...) -> None: ...
-
-class CreateResultsMetaDataResponse(_message.Message):
-    __slots__ = ["communication_token", "results"]
-    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    RESULTS_FIELD_NUMBER: _ClassVar[int]
-    communication_token: str
-    results: _containers.RepeatedCompositeFieldContainer[ResultMetaData]
-    def __init__(self, results: _Optional[_Iterable[_Union[ResultMetaData, _Mapping]]] = ..., communication_token: _Optional[str] = ...) -> None: ...
-
-class CreateResultsRequest(_message.Message):
-    __slots__ = ["communication_token", "results", "session_id"]
-    class ResultCreate(_message.Message):
-        __slots__ = ["data", "name"]
-        DATA_FIELD_NUMBER: _ClassVar[int]
-        NAME_FIELD_NUMBER: _ClassVar[int]
-        data: bytes
-        name: str
-        def __init__(self, name: _Optional[str] = ..., data: _Optional[bytes] = ...) -> None: ...
-    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    RESULTS_FIELD_NUMBER: _ClassVar[int]
-    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-    communication_token: str
-    results: _containers.RepeatedCompositeFieldContainer[CreateResultsRequest.ResultCreate]
-    session_id: str
-    def __init__(self, results: _Optional[_Iterable[_Union[CreateResultsRequest.ResultCreate, _Mapping]]] = ..., session_id: _Optional[str] = ..., communication_token: _Optional[str] = ...) -> None: ...
-
-class CreateResultsResponse(_message.Message):
-    __slots__ = ["communication_token", "results"]
+class CreateTaskRequest(_message.Message):
+    __slots__ = ["init_request", "init_task", "task_payload", "communication_token"]
+    class InitRequest(_message.Message):
+        __slots__ = ["task_options"]
+        TASK_OPTIONS_FIELD_NUMBER: _ClassVar[int]
+        task_options: _objects_pb2.TaskOptions
+        def __init__(self, task_options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ...) -> None: ...
+    INIT_REQUEST_FIELD_NUMBER: _ClassVar[int]
+    INIT_TASK_FIELD_NUMBER: _ClassVar[int]
+    TASK_PAYLOAD_FIELD_NUMBER: _ClassVar[int]
     COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    RESULTS_FIELD_NUMBER: _ClassVar[int]
+    init_request: CreateTaskRequest.InitRequest
+    init_task: _objects_pb2.InitTaskRequest
+    task_payload: _objects_pb2.DataChunk
     communication_token: str
-    results: _containers.RepeatedCompositeFieldContainer[ResultMetaData]
-    def __init__(self, results: _Optional[_Iterable[_Union[ResultMetaData, _Mapping]]] = ..., communication_token: _Optional[str] = ...) -> None: ...
+    def __init__(self, init_request: _Optional[_Union[CreateTaskRequest.InitRequest, _Mapping]] = ..., init_task: _Optional[_Union[_objects_pb2.InitTaskRequest, _Mapping]] = ..., task_payload: _Optional[_Union[_objects_pb2.DataChunk, _Mapping]] = ..., communication_token: _Optional[str] = ...) -> None: ...
 
 class CreateTaskReply(_message.Message):
-    __slots__ = ["communication_token", "creation_status_list", "error"]
+    __slots__ = ["creation_status_list", "error", "communication_token"]
+    class TaskInfo(_message.Message):
+        __slots__ = ["task_id", "expected_output_keys", "data_dependencies", "payload_id"]
+        TASK_ID_FIELD_NUMBER: _ClassVar[int]
+        EXPECTED_OUTPUT_KEYS_FIELD_NUMBER: _ClassVar[int]
+        DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
+        PAYLOAD_ID_FIELD_NUMBER: _ClassVar[int]
+        task_id: str
+        expected_output_keys: _containers.RepeatedScalarFieldContainer[str]
+        data_dependencies: _containers.RepeatedScalarFieldContainer[str]
+        payload_id: str
+        def __init__(self, task_id: _Optional[str] = ..., expected_output_keys: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., payload_id: _Optional[str] = ...) -> None: ...
     class CreationStatus(_message.Message):
-        __slots__ = ["error", "task_info"]
-        ERROR_FIELD_NUMBER: _ClassVar[int]
+        __slots__ = ["task_info", "error"]
         TASK_INFO_FIELD_NUMBER: _ClassVar[int]
-        error: str
+        ERROR_FIELD_NUMBER: _ClassVar[int]
         task_info: CreateTaskReply.TaskInfo
+        error: str
         def __init__(self, task_info: _Optional[_Union[CreateTaskReply.TaskInfo, _Mapping]] = ..., error: _Optional[str] = ...) -> None: ...
     class CreationStatusList(_message.Message):
         __slots__ = ["creation_statuses"]
         CREATION_STATUSES_FIELD_NUMBER: _ClassVar[int]
         creation_statuses: _containers.RepeatedCompositeFieldContainer[CreateTaskReply.CreationStatus]
         def __init__(self, creation_statuses: _Optional[_Iterable[_Union[CreateTaskReply.CreationStatus, _Mapping]]] = ...) -> None: ...
-    class TaskInfo(_message.Message):
-        __slots__ = ["data_dependencies", "expected_output_keys", "payload_id", "task_id"]
-        DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
-        EXPECTED_OUTPUT_KEYS_FIELD_NUMBER: _ClassVar[int]
-        PAYLOAD_ID_FIELD_NUMBER: _ClassVar[int]
-        TASK_ID_FIELD_NUMBER: _ClassVar[int]
-        data_dependencies: _containers.RepeatedScalarFieldContainer[str]
-        expected_output_keys: _containers.RepeatedScalarFieldContainer[str]
-        payload_id: str
-        task_id: str
-        def __init__(self, task_id: _Optional[str] = ..., expected_output_keys: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., payload_id: _Optional[str] = ...) -> None: ...
-    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
     CREATION_STATUS_LIST_FIELD_NUMBER: _ClassVar[int]
     ERROR_FIELD_NUMBER: _ClassVar[int]
-    communication_token: str
+    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
     creation_status_list: CreateTaskReply.CreationStatusList
     error: str
+    communication_token: str
     def __init__(self, creation_status_list: _Optional[_Union[CreateTaskReply.CreationStatusList, _Mapping]] = ..., error: _Optional[str] = ..., communication_token: _Optional[str] = ...) -> None: ...
 
-class CreateTaskRequest(_message.Message):
-    __slots__ = ["communication_token", "init_request", "init_task", "task_payload"]
-    class InitRequest(_message.Message):
-        __slots__ = ["task_options"]
-        TASK_OPTIONS_FIELD_NUMBER: _ClassVar[int]
-        task_options: _objects_pb2.TaskOptions
-        def __init__(self, task_options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ...) -> None: ...
+class DataRequest(_message.Message):
+    __slots__ = ["communication_token", "key"]
     COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    INIT_REQUEST_FIELD_NUMBER: _ClassVar[int]
-    INIT_TASK_FIELD_NUMBER: _ClassVar[int]
-    TASK_PAYLOAD_FIELD_NUMBER: _ClassVar[int]
+    KEY_FIELD_NUMBER: _ClassVar[int]
     communication_token: str
-    init_request: CreateTaskRequest.InitRequest
-    init_task: _objects_pb2.InitTaskRequest
-    task_payload: _objects_pb2.DataChunk
-    def __init__(self, init_request: _Optional[_Union[CreateTaskRequest.InitRequest, _Mapping]] = ..., init_task: _Optional[_Union[_objects_pb2.InitTaskRequest, _Mapping]] = ..., task_payload: _Optional[_Union[_objects_pb2.DataChunk, _Mapping]] = ..., communication_token: _Optional[str] = ...) -> None: ...
+    key: str
+    def __init__(self, communication_token: _Optional[str] = ..., key: _Optional[str] = ...) -> None: ...
 
 class DataReply(_message.Message):
-    __slots__ = ["communication_token", "data", "error", "init"]
+    __slots__ = ["communication_token", "init", "data", "error"]
     class Init(_message.Message):
-        __slots__ = ["data", "error", "key"]
+        __slots__ = ["key", "data", "error"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
         DATA_FIELD_NUMBER: _ClassVar[int]
         ERROR_FIELD_NUMBER: _ClassVar[int]
-        KEY_FIELD_NUMBER: _ClassVar[int]
+        key: str
         data: _objects_pb2.DataChunk
         error: str
-        key: str
         def __init__(self, key: _Optional[str] = ..., data: _Optional[_Union[_objects_pb2.DataChunk, _Mapping]] = ..., error: _Optional[str] = ...) -> None: ...
     COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
+    INIT_FIELD_NUMBER: _ClassVar[int]
     DATA_FIELD_NUMBER: _ClassVar[int]
     ERROR_FIELD_NUMBER: _ClassVar[int]
-    INIT_FIELD_NUMBER: _ClassVar[int]
     communication_token: str
+    init: DataReply.Init
     data: _objects_pb2.DataChunk
     error: str
-    init: DataReply.Init
     def __init__(self, communication_token: _Optional[str] = ..., init: _Optional[_Union[DataReply.Init, _Mapping]] = ..., data: _Optional[_Union[_objects_pb2.DataChunk, _Mapping]] = ..., error: _Optional[str] = ...) -> None: ...
 
-class DataRequest(_message.Message):
-    __slots__ = ["communication_token", "key"]
+class Result(_message.Message):
+    __slots__ = ["init", "data", "communication_token"]
+    INIT_FIELD_NUMBER: _ClassVar[int]
+    DATA_FIELD_NUMBER: _ClassVar[int]
     COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    KEY_FIELD_NUMBER: _ClassVar[int]
+    init: _objects_pb2.InitKeyedDataStream
+    data: _objects_pb2.DataChunk
     communication_token: str
-    key: str
-    def __init__(self, communication_token: _Optional[str] = ..., key: _Optional[str] = ...) -> None: ...
+    def __init__(self, init: _Optional[_Union[_objects_pb2.InitKeyedDataStream, _Mapping]] = ..., data: _Optional[_Union[_objects_pb2.DataChunk, _Mapping]] = ..., communication_token: _Optional[str] = ...) -> None: ...
 
-class Result(_message.Message):
-    __slots__ = ["communication_token", "data", "init"]
+class ResultReply(_message.Message):
+    __slots__ = ["communication_token", "Ok", "Error"]
     COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    DATA_FIELD_NUMBER: _ClassVar[int]
-    INIT_FIELD_NUMBER: _ClassVar[int]
+    OK_FIELD_NUMBER: _ClassVar[int]
+    ERROR_FIELD_NUMBER: _ClassVar[int]
     communication_token: str
-    data: _objects_pb2.DataChunk
-    init: _objects_pb2.InitKeyedDataStream
-    def __init__(self, init: _Optional[_Union[_objects_pb2.InitKeyedDataStream, _Mapping]] = ..., data: _Optional[_Union[_objects_pb2.DataChunk, _Mapping]] = ..., communication_token: _Optional[str] = ...) -> None: ...
+    Ok: _objects_pb2.Empty
+    Error: str
+    def __init__(self, communication_token: _Optional[str] = ..., Ok: _Optional[_Union[_objects_pb2.Empty, _Mapping]] = ..., Error: _Optional[str] = ...) -> None: ...
+
+class CreateResultsMetaDataRequest(_message.Message):
+    __slots__ = ["results", "session_id", "communication_token"]
+    class ResultCreate(_message.Message):
+        __slots__ = ["name"]
+        NAME_FIELD_NUMBER: _ClassVar[int]
+        name: str
+        def __init__(self, name: _Optional[str] = ...) -> None: ...
+    RESULTS_FIELD_NUMBER: _ClassVar[int]
+    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
+    results: _containers.RepeatedCompositeFieldContainer[CreateResultsMetaDataRequest.ResultCreate]
+    session_id: str
+    communication_token: str
+    def __init__(self, results: _Optional[_Iterable[_Union[CreateResultsMetaDataRequest.ResultCreate, _Mapping]]] = ..., session_id: _Optional[str] = ..., communication_token: _Optional[str] = ...) -> None: ...
 
 class ResultMetaData(_message.Message):
-    __slots__ = ["created_at", "name", "result_id", "session_id", "status"]
-    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    RESULT_ID_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["session_id", "result_id", "name", "status", "created_at"]
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+    RESULT_ID_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
-    created_at: _timestamp_pb2.Timestamp
-    name: str
-    result_id: str
+    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
     session_id: str
+    result_id: str
+    name: str
     status: _result_status_pb2.ResultStatus
+    created_at: _timestamp_pb2.Timestamp
     def __init__(self, session_id: _Optional[str] = ..., result_id: _Optional[str] = ..., name: _Optional[str] = ..., status: _Optional[_Union[_result_status_pb2.ResultStatus, str]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
 
-class ResultReply(_message.Message):
-    __slots__ = ["Error", "Ok", "communication_token"]
+class CreateResultsMetaDataResponse(_message.Message):
+    __slots__ = ["results", "communication_token"]
+    RESULTS_FIELD_NUMBER: _ClassVar[int]
     COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    ERROR_FIELD_NUMBER: _ClassVar[int]
-    Error: str
-    OK_FIELD_NUMBER: _ClassVar[int]
-    Ok: _objects_pb2.Empty
+    results: _containers.RepeatedCompositeFieldContainer[ResultMetaData]
     communication_token: str
-    def __init__(self, communication_token: _Optional[str] = ..., Ok: _Optional[_Union[_objects_pb2.Empty, _Mapping]] = ..., Error: _Optional[str] = ...) -> None: ...
+    def __init__(self, results: _Optional[_Iterable[_Union[ResultMetaData, _Mapping]]] = ..., communication_token: _Optional[str] = ...) -> None: ...
 
 class SubmitTasksRequest(_message.Message):
-    __slots__ = ["communication_token", "session_id", "task_creations", "task_options"]
+    __slots__ = ["session_id", "task_options", "task_creations", "communication_token"]
     class TaskCreation(_message.Message):
-        __slots__ = ["data_dependencies", "expected_output_keys", "payload_id", "task_options"]
-        DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
+        __slots__ = ["expected_output_keys", "data_dependencies", "payload_id", "task_options"]
         EXPECTED_OUTPUT_KEYS_FIELD_NUMBER: _ClassVar[int]
+        DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
         PAYLOAD_ID_FIELD_NUMBER: _ClassVar[int]
         TASK_OPTIONS_FIELD_NUMBER: _ClassVar[int]
-        data_dependencies: _containers.RepeatedScalarFieldContainer[str]
         expected_output_keys: _containers.RepeatedScalarFieldContainer[str]
+        data_dependencies: _containers.RepeatedScalarFieldContainer[str]
         payload_id: str
         task_options: _objects_pb2.TaskOptions
         def __init__(self, expected_output_keys: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., payload_id: _Optional[str] = ..., task_options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ...) -> None: ...
-    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-    TASK_CREATIONS_FIELD_NUMBER: _ClassVar[int]
     TASK_OPTIONS_FIELD_NUMBER: _ClassVar[int]
-    communication_token: str
+    TASK_CREATIONS_FIELD_NUMBER: _ClassVar[int]
+    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
     session_id: str
-    task_creations: _containers.RepeatedCompositeFieldContainer[SubmitTasksRequest.TaskCreation]
     task_options: _objects_pb2.TaskOptions
+    task_creations: _containers.RepeatedCompositeFieldContainer[SubmitTasksRequest.TaskCreation]
+    communication_token: str
     def __init__(self, session_id: _Optional[str] = ..., task_options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., task_creations: _Optional[_Iterable[_Union[SubmitTasksRequest.TaskCreation, _Mapping]]] = ..., communication_token: _Optional[str] = ...) -> None: ...
 
 class SubmitTasksResponse(_message.Message):
-    __slots__ = ["communication_token", "task_infos"]
+    __slots__ = ["task_infos", "communication_token"]
     class TaskInfo(_message.Message):
-        __slots__ = ["data_dependencies", "expected_output_ids", "payload_id", "task_id"]
-        DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
+        __slots__ = ["task_id", "expected_output_ids", "data_dependencies", "payload_id"]
+        TASK_ID_FIELD_NUMBER: _ClassVar[int]
         EXPECTED_OUTPUT_IDS_FIELD_NUMBER: _ClassVar[int]
+        DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
         PAYLOAD_ID_FIELD_NUMBER: _ClassVar[int]
-        TASK_ID_FIELD_NUMBER: _ClassVar[int]
-        data_dependencies: _containers.RepeatedScalarFieldContainer[str]
+        task_id: str
         expected_output_ids: _containers.RepeatedScalarFieldContainer[str]
+        data_dependencies: _containers.RepeatedScalarFieldContainer[str]
         payload_id: str
-        task_id: str
         def __init__(self, task_id: _Optional[str] = ..., expected_output_ids: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., payload_id: _Optional[str] = ...) -> None: ...
-    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
     TASK_INFOS_FIELD_NUMBER: _ClassVar[int]
-    communication_token: str
+    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
     task_infos: _containers.RepeatedCompositeFieldContainer[SubmitTasksResponse.TaskInfo]
+    communication_token: str
     def __init__(self, task_infos: _Optional[_Iterable[_Union[SubmitTasksResponse.TaskInfo, _Mapping]]] = ..., communication_token: _Optional[str] = ...) -> None: ...
 
+class CreateResultsRequest(_message.Message):
+    __slots__ = ["results", "session_id", "communication_token"]
+    class ResultCreate(_message.Message):
+        __slots__ = ["name", "data"]
+        NAME_FIELD_NUMBER: _ClassVar[int]
+        DATA_FIELD_NUMBER: _ClassVar[int]
+        name: str
+        data: bytes
+        def __init__(self, name: _Optional[str] = ..., data: _Optional[bytes] = ...) -> None: ...
+    RESULTS_FIELD_NUMBER: _ClassVar[int]
+    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
+    results: _containers.RepeatedCompositeFieldContainer[CreateResultsRequest.ResultCreate]
+    session_id: str
+    communication_token: str
+    def __init__(self, results: _Optional[_Iterable[_Union[CreateResultsRequest.ResultCreate, _Mapping]]] = ..., session_id: _Optional[str] = ..., communication_token: _Optional[str] = ...) -> None: ...
+
+class CreateResultsResponse(_message.Message):
+    __slots__ = ["results", "communication_token"]
+    RESULTS_FIELD_NUMBER: _ClassVar[int]
+    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
+    results: _containers.RepeatedCompositeFieldContainer[ResultMetaData]
+    communication_token: str
+    def __init__(self, results: _Optional[_Iterable[_Union[ResultMetaData, _Mapping]]] = ..., communication_token: _Optional[str] = ...) -> None: ...
+
 class UploadResultDataRequest(_message.Message):
-    __slots__ = ["communication_token", "data_chunk", "id"]
+    __slots__ = ["id", "data_chunk", "communication_token"]
     class ResultIdentifier(_message.Message):
-        __slots__ = ["result_id", "session_id"]
-        RESULT_ID_FIELD_NUMBER: _ClassVar[int]
+        __slots__ = ["session_id", "result_id"]
         SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-        result_id: str
+        RESULT_ID_FIELD_NUMBER: _ClassVar[int]
         session_id: str
+        result_id: str
         def __init__(self, session_id: _Optional[str] = ..., result_id: _Optional[str] = ...) -> None: ...
-    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    DATA_CHUNK_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
-    communication_token: str
-    data_chunk: bytes
+    DATA_CHUNK_FIELD_NUMBER: _ClassVar[int]
+    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
     id: UploadResultDataRequest.ResultIdentifier
+    data_chunk: bytes
+    communication_token: str
     def __init__(self, id: _Optional[_Union[UploadResultDataRequest.ResultIdentifier, _Mapping]] = ..., data_chunk: _Optional[bytes] = ..., communication_token: _Optional[str] = ...) -> None: ...
 
 class UploadResultDataResponse(_message.Message):
-    __slots__ = ["communication_token", "result_id"]
-    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["result_id", "communication_token"]
     RESULT_ID_FIELD_NUMBER: _ClassVar[int]
-    communication_token: str
+    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
     result_id: str
+    communication_token: str
     def __init__(self, result_id: _Optional[str] = ..., communication_token: _Optional[str] = ...) -> None: ...
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/applications_common_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/common/applications_common_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: applications_common.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from . import objects_pb2 as objects__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x61pplications_common.proto\x12 armonik.api.grpc.v1.applications\x1a\robjects.proto\"S\n\x0e\x41pplicationRaw\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0f\n\x07service\x18\x04 \x01(\t\"\xeb\x05\n\x17ListApplicationsRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12P\n\x06\x66ilter\x18\x03 \x01(\x0b\x32@.armonik.api.grpc.v1.applications.ListApplicationsRequest.Filter\x12L\n\x04sort\x18\x04 \x01(\x0b\x32>.armonik.api.grpc.v1.applications.ListApplicationsRequest.Sort\x1aK\n\x06\x46ilter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0f\n\x07service\x18\x04 \x01(\t\x1a\xbb\x01\n\x04Sort\x12V\n\x06\x66ields\x18\x01 \x03(\x0e\x32\x46.armonik.api.grpc.v1.applications.ListApplicationsRequest.OrderByField\x12[\n\tdirection\x18\x02 \x01(\x0e\x32H.armonik.api.grpc.v1.applications.ListApplicationsRequest.OrderDirection\"\x9d\x01\n\x0cOrderByField\x12\x1e\n\x1aORDER_BY_FIELD_UNSPECIFIED\x10\x00\x12\x17\n\x13ORDER_BY_FIELD_NAME\x10\x01\x12\x1a\n\x16ORDER_BY_FIELD_VERSION\x10\x02\x12\x1c\n\x18ORDER_BY_FIELD_NAMESPACE\x10\x03\x12\x1a\n\x16ORDER_BY_FIELD_SERVICE\x10\x04\"d\n\x0eOrderDirection\x12\x1f\n\x1bORDER_DIRECTION_UNSPECIFIED\x10\x00\x12\x17\n\x13ORDER_DIRECTION_ASC\x10\x01\x12\x18\n\x14ORDER_DIRECTION_DESC\x10\x02\"\x92\x01\n\x18ListApplicationsResponse\x12\x46\n\x0c\x61pplications\x18\x01 \x03(\x0b\x32\x30.armonik.api.grpc.v1.applications.ApplicationRaw\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\":\n\x19\x43ountTasksByStatusRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"N\n\x1a\x43ountTasksByStatusResponse\x12\x30\n\x06status\x18\x01 \x03(\x0b\x32 .armonik.api.grpc.v1.StatusCountB#\xaa\x02 ArmoniK.Api.gRPC.V1.Applicationsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'applications_common_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'applications_common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002 ArmoniK.Api.gRPC.V1.Applications'
-  _APPLICATIONRAW._serialized_start=78
-  _APPLICATIONRAW._serialized_end=161
-  _LISTAPPLICATIONSREQUEST._serialized_start=164
-  _LISTAPPLICATIONSREQUEST._serialized_end=911
-  _LISTAPPLICATIONSREQUEST_FILTER._serialized_start=384
-  _LISTAPPLICATIONSREQUEST_FILTER._serialized_end=459
-  _LISTAPPLICATIONSREQUEST_SORT._serialized_start=462
-  _LISTAPPLICATIONSREQUEST_SORT._serialized_end=649
-  _LISTAPPLICATIONSREQUEST_ORDERBYFIELD._serialized_start=652
-  _LISTAPPLICATIONSREQUEST_ORDERBYFIELD._serialized_end=809
-  _LISTAPPLICATIONSREQUEST_ORDERDIRECTION._serialized_start=811
-  _LISTAPPLICATIONSREQUEST_ORDERDIRECTION._serialized_end=911
-  _LISTAPPLICATIONSRESPONSE._serialized_start=914
-  _LISTAPPLICATIONSRESPONSE._serialized_end=1060
-  _COUNTTASKSBYSTATUSREQUEST._serialized_start=1062
-  _COUNTTASKSBYSTATUSREQUEST._serialized_end=1120
-  _COUNTTASKSBYSTATUSRESPONSE._serialized_start=1122
-  _COUNTTASKSBYSTATUSRESPONSE._serialized_end=1200
+  _globals['_APPLICATIONRAW']._serialized_start=78
+  _globals['_APPLICATIONRAW']._serialized_end=161
+  _globals['_LISTAPPLICATIONSREQUEST']._serialized_start=164
+  _globals['_LISTAPPLICATIONSREQUEST']._serialized_end=911
+  _globals['_LISTAPPLICATIONSREQUEST_FILTER']._serialized_start=384
+  _globals['_LISTAPPLICATIONSREQUEST_FILTER']._serialized_end=459
+  _globals['_LISTAPPLICATIONSREQUEST_SORT']._serialized_start=462
+  _globals['_LISTAPPLICATIONSREQUEST_SORT']._serialized_end=649
+  _globals['_LISTAPPLICATIONSREQUEST_ORDERBYFIELD']._serialized_start=652
+  _globals['_LISTAPPLICATIONSREQUEST_ORDERBYFIELD']._serialized_end=809
+  _globals['_LISTAPPLICATIONSREQUEST_ORDERDIRECTION']._serialized_start=811
+  _globals['_LISTAPPLICATIONSREQUEST_ORDERDIRECTION']._serialized_end=911
+  _globals['_LISTAPPLICATIONSRESPONSE']._serialized_start=914
+  _globals['_LISTAPPLICATIONSRESPONSE']._serialized_end=1060
+  _globals['_COUNTTASKSBYSTATUSREQUEST']._serialized_start=1062
+  _globals['_COUNTTASKSBYSTATUSREQUEST']._serialized_end=1120
+  _globals['_COUNTTASKSBYSTATUSRESPONSE']._serialized_start=1122
+  _globals['_COUNTTASKSBYSTATUSRESPONSE']._serialized_end=1200
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/applications_common_pb2.pyi` & `armonik-3.8.2.dev349/src/armonik/protogen/common/applications_common_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -4,85 +4,93 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class ApplicationRaw(_message.Message):
-    __slots__ = ["name", "namespace", "service", "version"]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["name", "version", "namespace", "service"]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    SERVICE_FIELD_NUMBER: _ClassVar[int]
     name: str
+    version: str
     namespace: str
     service: str
-    version: str
     def __init__(self, name: _Optional[str] = ..., version: _Optional[str] = ..., namespace: _Optional[str] = ..., service: _Optional[str] = ...) -> None: ...
 
-class CountTasksByStatusRequest(_message.Message):
-    __slots__ = ["name", "version"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    VERSION_FIELD_NUMBER: _ClassVar[int]
-    name: str
-    version: str
-    def __init__(self, name: _Optional[str] = ..., version: _Optional[str] = ...) -> None: ...
-
-class CountTasksByStatusResponse(_message.Message):
-    __slots__ = ["status"]
-    STATUS_FIELD_NUMBER: _ClassVar[int]
-    status: _containers.RepeatedCompositeFieldContainer[_objects_pb2.StatusCount]
-    def __init__(self, status: _Optional[_Iterable[_Union[_objects_pb2.StatusCount, _Mapping]]] = ...) -> None: ...
-
 class ListApplicationsRequest(_message.Message):
-    __slots__ = ["filter", "page", "page_size", "sort"]
+    __slots__ = ["page", "page_size", "filter", "sort"]
     class OrderByField(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        ORDER_BY_FIELD_UNSPECIFIED: _ClassVar[ListApplicationsRequest.OrderByField]
+        ORDER_BY_FIELD_NAME: _ClassVar[ListApplicationsRequest.OrderByField]
+        ORDER_BY_FIELD_VERSION: _ClassVar[ListApplicationsRequest.OrderByField]
+        ORDER_BY_FIELD_NAMESPACE: _ClassVar[ListApplicationsRequest.OrderByField]
+        ORDER_BY_FIELD_SERVICE: _ClassVar[ListApplicationsRequest.OrderByField]
+    ORDER_BY_FIELD_UNSPECIFIED: ListApplicationsRequest.OrderByField
+    ORDER_BY_FIELD_NAME: ListApplicationsRequest.OrderByField
+    ORDER_BY_FIELD_VERSION: ListApplicationsRequest.OrderByField
+    ORDER_BY_FIELD_NAMESPACE: ListApplicationsRequest.OrderByField
+    ORDER_BY_FIELD_SERVICE: ListApplicationsRequest.OrderByField
     class OrderDirection(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        ORDER_DIRECTION_UNSPECIFIED: _ClassVar[ListApplicationsRequest.OrderDirection]
+        ORDER_DIRECTION_ASC: _ClassVar[ListApplicationsRequest.OrderDirection]
+        ORDER_DIRECTION_DESC: _ClassVar[ListApplicationsRequest.OrderDirection]
+    ORDER_DIRECTION_UNSPECIFIED: ListApplicationsRequest.OrderDirection
+    ORDER_DIRECTION_ASC: ListApplicationsRequest.OrderDirection
+    ORDER_DIRECTION_DESC: ListApplicationsRequest.OrderDirection
     class Filter(_message.Message):
-        __slots__ = ["name", "namespace", "service", "version"]
-        NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+        __slots__ = ["name", "version", "namespace", "service"]
         NAME_FIELD_NUMBER: _ClassVar[int]
-        SERVICE_FIELD_NUMBER: _ClassVar[int]
         VERSION_FIELD_NUMBER: _ClassVar[int]
+        NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+        SERVICE_FIELD_NUMBER: _ClassVar[int]
         name: str
+        version: str
         namespace: str
         service: str
-        version: str
         def __init__(self, name: _Optional[str] = ..., version: _Optional[str] = ..., namespace: _Optional[str] = ..., service: _Optional[str] = ...) -> None: ...
     class Sort(_message.Message):
-        __slots__ = ["direction", "fields"]
-        DIRECTION_FIELD_NUMBER: _ClassVar[int]
+        __slots__ = ["fields", "direction"]
         FIELDS_FIELD_NUMBER: _ClassVar[int]
-        direction: ListApplicationsRequest.OrderDirection
+        DIRECTION_FIELD_NUMBER: _ClassVar[int]
         fields: _containers.RepeatedScalarFieldContainer[ListApplicationsRequest.OrderByField]
+        direction: ListApplicationsRequest.OrderDirection
         def __init__(self, fields: _Optional[_Iterable[_Union[ListApplicationsRequest.OrderByField, str]]] = ..., direction: _Optional[_Union[ListApplicationsRequest.OrderDirection, str]] = ...) -> None: ...
-    FILTER_FIELD_NUMBER: _ClassVar[int]
-    ORDER_BY_FIELD_NAME: ListApplicationsRequest.OrderByField
-    ORDER_BY_FIELD_NAMESPACE: ListApplicationsRequest.OrderByField
-    ORDER_BY_FIELD_SERVICE: ListApplicationsRequest.OrderByField
-    ORDER_BY_FIELD_UNSPECIFIED: ListApplicationsRequest.OrderByField
-    ORDER_BY_FIELD_VERSION: ListApplicationsRequest.OrderByField
-    ORDER_DIRECTION_ASC: ListApplicationsRequest.OrderDirection
-    ORDER_DIRECTION_DESC: ListApplicationsRequest.OrderDirection
-    ORDER_DIRECTION_UNSPECIFIED: ListApplicationsRequest.OrderDirection
     PAGE_FIELD_NUMBER: _ClassVar[int]
     PAGE_SIZE_FIELD_NUMBER: _ClassVar[int]
+    FILTER_FIELD_NUMBER: _ClassVar[int]
     SORT_FIELD_NUMBER: _ClassVar[int]
-    filter: ListApplicationsRequest.Filter
     page: int
     page_size: int
+    filter: ListApplicationsRequest.Filter
     sort: ListApplicationsRequest.Sort
     def __init__(self, page: _Optional[int] = ..., page_size: _Optional[int] = ..., filter: _Optional[_Union[ListApplicationsRequest.Filter, _Mapping]] = ..., sort: _Optional[_Union[ListApplicationsRequest.Sort, _Mapping]] = ...) -> None: ...
 
 class ListApplicationsResponse(_message.Message):
     __slots__ = ["applications", "page", "page_size", "total"]
     APPLICATIONS_FIELD_NUMBER: _ClassVar[int]
     PAGE_FIELD_NUMBER: _ClassVar[int]
     PAGE_SIZE_FIELD_NUMBER: _ClassVar[int]
     TOTAL_FIELD_NUMBER: _ClassVar[int]
     applications: _containers.RepeatedCompositeFieldContainer[ApplicationRaw]
     page: int
     page_size: int
     total: int
     def __init__(self, applications: _Optional[_Iterable[_Union[ApplicationRaw, _Mapping]]] = ..., page: _Optional[int] = ..., page_size: _Optional[int] = ..., total: _Optional[int] = ...) -> None: ...
+
+class CountTasksByStatusRequest(_message.Message):
+    __slots__ = ["name", "version"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    VERSION_FIELD_NUMBER: _ClassVar[int]
+    name: str
+    version: str
+    def __init__(self, name: _Optional[str] = ..., version: _Optional[str] = ...) -> None: ...
+
+class CountTasksByStatusResponse(_message.Message):
+    __slots__ = ["status"]
+    STATUS_FIELD_NUMBER: _ClassVar[int]
+    status: _containers.RepeatedCompositeFieldContainer[_objects_pb2.StatusCount]
+    def __init__(self, status: _Optional[_Iterable[_Union[_objects_pb2.StatusCount, _Mapping]]] = ...) -> None: ...
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/auth_common_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/common/result_status_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: auth_common.proto
+# source: result_status.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x61uth_common.proto\x12\x18\x61rmonik.api.grpc.v1.auth\"<\n\x04User\x12\x10\n\x08username\x18\x01 \x01(\t\x12\r\n\x05roles\x18\x02 \x03(\t\x12\x13\n\x0bpermissions\x18\x03 \x03(\t\"\x17\n\x15GetCurrentUserRequest\"F\n\x16GetCurrentUserResponse\x12,\n\x04user\x18\x01 \x01(\x0b\x32\x1e.armonik.api.grpc.v1.auth.UserB\x1b\xaa\x02\x18\x41rmoniK.Api.gRPC.V1.Authb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13result_status.proto\x12!armonik.api.grpc.v1.result_status*\x9c\x01\n\x0cResultStatus\x12\x1d\n\x19RESULT_STATUS_UNSPECIFIED\x10\x00\x12\x19\n\x15RESULT_STATUS_CREATED\x10\x01\x12\x1b\n\x17RESULT_STATUS_COMPLETED\x10\x02\x12\x19\n\x15RESULT_STATUS_ABORTED\x10\x03\x12\x1a\n\x16RESULT_STATUS_NOTFOUND\x10\x7f\x42\x16\xaa\x02\x13\x41rmoniK.Api.gRPC.V1b\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'auth_common_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'result_status_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\252\002\030ArmoniK.Api.gRPC.V1.Auth'
-  _USER._serialized_start=47
-  _USER._serialized_end=107
-  _GETCURRENTUSERREQUEST._serialized_start=109
-  _GETCURRENTUSERREQUEST._serialized_end=132
-  _GETCURRENTUSERRESPONSE._serialized_start=134
-  _GETCURRENTUSERRESPONSE._serialized_end=204
+  DESCRIPTOR._serialized_options = b'\252\002\023ArmoniK.Api.gRPC.V1'
+  _globals['_RESULTSTATUS']._serialized_start=59
+  _globals['_RESULTSTATUS']._serialized_end=215
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/auth_common_pb2.pyi` & `armonik-3.8.2.dev349/src/armonik/protogen/common/auth_common_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
+class User(_message.Message):
+    __slots__ = ["username", "roles", "permissions"]
+    USERNAME_FIELD_NUMBER: _ClassVar[int]
+    ROLES_FIELD_NUMBER: _ClassVar[int]
+    PERMISSIONS_FIELD_NUMBER: _ClassVar[int]
+    username: str
+    roles: _containers.RepeatedScalarFieldContainer[str]
+    permissions: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, username: _Optional[str] = ..., roles: _Optional[_Iterable[str]] = ..., permissions: _Optional[_Iterable[str]] = ...) -> None: ...
+
 class GetCurrentUserRequest(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class GetCurrentUserResponse(_message.Message):
     __slots__ = ["user"]
     USER_FIELD_NUMBER: _ClassVar[int]
     user: User
     def __init__(self, user: _Optional[_Union[User, _Mapping]] = ...) -> None: ...
-
-class User(_message.Message):
-    __slots__ = ["permissions", "roles", "username"]
-    PERMISSIONS_FIELD_NUMBER: _ClassVar[int]
-    ROLES_FIELD_NUMBER: _ClassVar[int]
-    USERNAME_FIELD_NUMBER: _ClassVar[int]
-    permissions: _containers.RepeatedScalarFieldContainer[str]
-    roles: _containers.RepeatedScalarFieldContainer[str]
-    username: str
-    def __init__(self, username: _Optional[str] = ..., roles: _Optional[_Iterable[str]] = ..., permissions: _Optional[_Iterable[str]] = ...) -> None: ...
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/events_common_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/common/events_common_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: events_common.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from . import result_status_pb2 as result__status__pb2
 from . import task_status_pb2 as task__status__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13\x65vents_common.proto\x12\x1a\x61rmonik.api.grpc.v1.events\x1a\x13result_status.proto\x1a\x11task_status.proto\".\n\x18\x45ventSubscriptionRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"\x8c\t\n\x19\x45ventSubscriptionResponse\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x64\n\x12task_status_update\x18\x02 \x01(\x0b\x32\x46.armonik.api.grpc.v1.events.EventSubscriptionResponse.TaskStatusUpdateH\x00\x12h\n\x14result_status_update\x18\x03 \x01(\x0b\x32H.armonik.api.grpc.v1.events.EventSubscriptionResponse.ResultStatusUpdateH\x00\x12\x66\n\x13result_owner_update\x18\x04 \x01(\x0b\x32G.armonik.api.grpc.v1.events.EventSubscriptionResponse.ResultOwnerUpdateH\x00\x12Q\n\x08new_task\x18\x05 \x01(\x0b\x32=.armonik.api.grpc.v1.events.EventSubscriptionResponse.NewTaskH\x00\x12U\n\nnew_result\x18\x06 \x01(\x0b\x32?.armonik.api.grpc.v1.events.EventSubscriptionResponse.NewResultH\x00\x1a`\n\x10TaskStatusUpdate\x12\x0f\n\x07task_id\x18\n \x01(\t\x12;\n\x06status\x18\x0b \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x1ah\n\x12ResultStatusUpdate\x12\x11\n\tresult_id\x18\x14 \x01(\t\x12?\n\x06status\x18\x15 \x01(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\x1a[\n\x11ResultOwnerUpdate\x12\x11\n\tresult_id\x18\x1e \x01(\t\x12\x19\n\x11previous_owner_id\x18\x1f \x01(\t\x12\x18\n\x10\x63urrent_owner_id\x18  \x01(\t\x1a\xd2\x01\n\x07NewTask\x12\x0f\n\x07task_id\x18( \x01(\t\x12\x12\n\npayload_id\x18) \x01(\t\x12\x16\n\x0eorigin_task_id\x18* \x01(\t\x12;\n\x06status\x18+ \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12\x1c\n\x14\x65xpected_output_keys\x18, \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18- \x03(\t\x12\x14\n\x0cretry_of_ids\x18. \x03(\t\x1aq\n\tNewResult\x12\x11\n\tresult_id\x18\x32 \x01(\t\x12\x10\n\x08owner_id\x18\x33 \x01(\t\x12?\n\x06status\x18\x34 \x01(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatusB\x08\n\x06updateB\x1d\xaa\x02\x1a\x41rmoniK.Api.gRPC.V1.Eventsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'events_common_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'events_common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\032ArmoniK.Api.gRPC.V1.Events'
-  _EVENTSUBSCRIPTIONREQUEST._serialized_start=91
-  _EVENTSUBSCRIPTIONREQUEST._serialized_end=137
-  _EVENTSUBSCRIPTIONRESPONSE._serialized_start=140
-  _EVENTSUBSCRIPTIONRESPONSE._serialized_end=1304
-  _EVENTSUBSCRIPTIONRESPONSE_TASKSTATUSUPDATE._serialized_start=671
-  _EVENTSUBSCRIPTIONRESPONSE_TASKSTATUSUPDATE._serialized_end=767
-  _EVENTSUBSCRIPTIONRESPONSE_RESULTSTATUSUPDATE._serialized_start=769
-  _EVENTSUBSCRIPTIONRESPONSE_RESULTSTATUSUPDATE._serialized_end=873
-  _EVENTSUBSCRIPTIONRESPONSE_RESULTOWNERUPDATE._serialized_start=875
-  _EVENTSUBSCRIPTIONRESPONSE_RESULTOWNERUPDATE._serialized_end=966
-  _EVENTSUBSCRIPTIONRESPONSE_NEWTASK._serialized_start=969
-  _EVENTSUBSCRIPTIONRESPONSE_NEWTASK._serialized_end=1179
-  _EVENTSUBSCRIPTIONRESPONSE_NEWRESULT._serialized_start=1181
-  _EVENTSUBSCRIPTIONRESPONSE_NEWRESULT._serialized_end=1294
+  _globals['_EVENTSUBSCRIPTIONREQUEST']._serialized_start=91
+  _globals['_EVENTSUBSCRIPTIONREQUEST']._serialized_end=137
+  _globals['_EVENTSUBSCRIPTIONRESPONSE']._serialized_start=140
+  _globals['_EVENTSUBSCRIPTIONRESPONSE']._serialized_end=1304
+  _globals['_EVENTSUBSCRIPTIONRESPONSE_TASKSTATUSUPDATE']._serialized_start=671
+  _globals['_EVENTSUBSCRIPTIONRESPONSE_TASKSTATUSUPDATE']._serialized_end=767
+  _globals['_EVENTSUBSCRIPTIONRESPONSE_RESULTSTATUSUPDATE']._serialized_start=769
+  _globals['_EVENTSUBSCRIPTIONRESPONSE_RESULTSTATUSUPDATE']._serialized_end=873
+  _globals['_EVENTSUBSCRIPTIONRESPONSE_RESULTOWNERUPDATE']._serialized_start=875
+  _globals['_EVENTSUBSCRIPTIONRESPONSE_RESULTOWNERUPDATE']._serialized_end=966
+  _globals['_EVENTSUBSCRIPTIONRESPONSE_NEWTASK']._serialized_start=969
+  _globals['_EVENTSUBSCRIPTIONRESPONSE_NEWTASK']._serialized_end=1179
+  _globals['_EVENTSUBSCRIPTIONRESPONSE_NEWRESULT']._serialized_start=1181
+  _globals['_EVENTSUBSCRIPTIONRESPONSE_NEWRESULT']._serialized_end=1294
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/events_common_pb2.pyi` & `armonik-3.8.2.dev349/src/armonik/protogen/common/events_common_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -10,70 +10,70 @@
 class EventSubscriptionRequest(_message.Message):
     __slots__ = ["session_id"]
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
     session_id: str
     def __init__(self, session_id: _Optional[str] = ...) -> None: ...
 
 class EventSubscriptionResponse(_message.Message):
-    __slots__ = ["new_result", "new_task", "result_owner_update", "result_status_update", "session_id", "task_status_update"]
-    class NewResult(_message.Message):
-        __slots__ = ["owner_id", "result_id", "status"]
-        OWNER_ID_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["session_id", "task_status_update", "result_status_update", "result_owner_update", "new_task", "new_result"]
+    class TaskStatusUpdate(_message.Message):
+        __slots__ = ["task_id", "status"]
+        TASK_ID_FIELD_NUMBER: _ClassVar[int]
+        STATUS_FIELD_NUMBER: _ClassVar[int]
+        task_id: str
+        status: _task_status_pb2.TaskStatus
+        def __init__(self, task_id: _Optional[str] = ..., status: _Optional[_Union[_task_status_pb2.TaskStatus, str]] = ...) -> None: ...
+    class ResultStatusUpdate(_message.Message):
+        __slots__ = ["result_id", "status"]
         RESULT_ID_FIELD_NUMBER: _ClassVar[int]
         STATUS_FIELD_NUMBER: _ClassVar[int]
-        owner_id: str
         result_id: str
         status: _result_status_pb2.ResultStatus
-        def __init__(self, result_id: _Optional[str] = ..., owner_id: _Optional[str] = ..., status: _Optional[_Union[_result_status_pb2.ResultStatus, str]] = ...) -> None: ...
+        def __init__(self, result_id: _Optional[str] = ..., status: _Optional[_Union[_result_status_pb2.ResultStatus, str]] = ...) -> None: ...
+    class ResultOwnerUpdate(_message.Message):
+        __slots__ = ["result_id", "previous_owner_id", "current_owner_id"]
+        RESULT_ID_FIELD_NUMBER: _ClassVar[int]
+        PREVIOUS_OWNER_ID_FIELD_NUMBER: _ClassVar[int]
+        CURRENT_OWNER_ID_FIELD_NUMBER: _ClassVar[int]
+        result_id: str
+        previous_owner_id: str
+        current_owner_id: str
+        def __init__(self, result_id: _Optional[str] = ..., previous_owner_id: _Optional[str] = ..., current_owner_id: _Optional[str] = ...) -> None: ...
     class NewTask(_message.Message):
-        __slots__ = ["data_dependencies", "expected_output_keys", "origin_task_id", "payload_id", "retry_of_ids", "status", "task_id"]
-        DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
-        EXPECTED_OUTPUT_KEYS_FIELD_NUMBER: _ClassVar[int]
-        ORIGIN_TASK_ID_FIELD_NUMBER: _ClassVar[int]
+        __slots__ = ["task_id", "payload_id", "origin_task_id", "status", "expected_output_keys", "data_dependencies", "retry_of_ids"]
+        TASK_ID_FIELD_NUMBER: _ClassVar[int]
         PAYLOAD_ID_FIELD_NUMBER: _ClassVar[int]
-        RETRY_OF_IDS_FIELD_NUMBER: _ClassVar[int]
+        ORIGIN_TASK_ID_FIELD_NUMBER: _ClassVar[int]
         STATUS_FIELD_NUMBER: _ClassVar[int]
-        TASK_ID_FIELD_NUMBER: _ClassVar[int]
-        data_dependencies: _containers.RepeatedScalarFieldContainer[str]
-        expected_output_keys: _containers.RepeatedScalarFieldContainer[str]
-        origin_task_id: str
+        EXPECTED_OUTPUT_KEYS_FIELD_NUMBER: _ClassVar[int]
+        DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
+        RETRY_OF_IDS_FIELD_NUMBER: _ClassVar[int]
+        task_id: str
         payload_id: str
-        retry_of_ids: _containers.RepeatedScalarFieldContainer[str]
+        origin_task_id: str
         status: _task_status_pb2.TaskStatus
-        task_id: str
+        expected_output_keys: _containers.RepeatedScalarFieldContainer[str]
+        data_dependencies: _containers.RepeatedScalarFieldContainer[str]
+        retry_of_ids: _containers.RepeatedScalarFieldContainer[str]
         def __init__(self, task_id: _Optional[str] = ..., payload_id: _Optional[str] = ..., origin_task_id: _Optional[str] = ..., status: _Optional[_Union[_task_status_pb2.TaskStatus, str]] = ..., expected_output_keys: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., retry_of_ids: _Optional[_Iterable[str]] = ...) -> None: ...
-    class ResultOwnerUpdate(_message.Message):
-        __slots__ = ["current_owner_id", "previous_owner_id", "result_id"]
-        CURRENT_OWNER_ID_FIELD_NUMBER: _ClassVar[int]
-        PREVIOUS_OWNER_ID_FIELD_NUMBER: _ClassVar[int]
-        RESULT_ID_FIELD_NUMBER: _ClassVar[int]
-        current_owner_id: str
-        previous_owner_id: str
-        result_id: str
-        def __init__(self, result_id: _Optional[str] = ..., previous_owner_id: _Optional[str] = ..., current_owner_id: _Optional[str] = ...) -> None: ...
-    class ResultStatusUpdate(_message.Message):
-        __slots__ = ["result_id", "status"]
+    class NewResult(_message.Message):
+        __slots__ = ["result_id", "owner_id", "status"]
         RESULT_ID_FIELD_NUMBER: _ClassVar[int]
+        OWNER_ID_FIELD_NUMBER: _ClassVar[int]
         STATUS_FIELD_NUMBER: _ClassVar[int]
         result_id: str
+        owner_id: str
         status: _result_status_pb2.ResultStatus
-        def __init__(self, result_id: _Optional[str] = ..., status: _Optional[_Union[_result_status_pb2.ResultStatus, str]] = ...) -> None: ...
-    class TaskStatusUpdate(_message.Message):
-        __slots__ = ["status", "task_id"]
-        STATUS_FIELD_NUMBER: _ClassVar[int]
-        TASK_ID_FIELD_NUMBER: _ClassVar[int]
-        status: _task_status_pb2.TaskStatus
-        task_id: str
-        def __init__(self, task_id: _Optional[str] = ..., status: _Optional[_Union[_task_status_pb2.TaskStatus, str]] = ...) -> None: ...
-    NEW_RESULT_FIELD_NUMBER: _ClassVar[int]
-    NEW_TASK_FIELD_NUMBER: _ClassVar[int]
-    RESULT_OWNER_UPDATE_FIELD_NUMBER: _ClassVar[int]
-    RESULT_STATUS_UPDATE_FIELD_NUMBER: _ClassVar[int]
+        def __init__(self, result_id: _Optional[str] = ..., owner_id: _Optional[str] = ..., status: _Optional[_Union[_result_status_pb2.ResultStatus, str]] = ...) -> None: ...
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
     TASK_STATUS_UPDATE_FIELD_NUMBER: _ClassVar[int]
-    new_result: EventSubscriptionResponse.NewResult
-    new_task: EventSubscriptionResponse.NewTask
-    result_owner_update: EventSubscriptionResponse.ResultOwnerUpdate
-    result_status_update: EventSubscriptionResponse.ResultStatusUpdate
+    RESULT_STATUS_UPDATE_FIELD_NUMBER: _ClassVar[int]
+    RESULT_OWNER_UPDATE_FIELD_NUMBER: _ClassVar[int]
+    NEW_TASK_FIELD_NUMBER: _ClassVar[int]
+    NEW_RESULT_FIELD_NUMBER: _ClassVar[int]
     session_id: str
     task_status_update: EventSubscriptionResponse.TaskStatusUpdate
+    result_status_update: EventSubscriptionResponse.ResultStatusUpdate
+    result_owner_update: EventSubscriptionResponse.ResultOwnerUpdate
+    new_task: EventSubscriptionResponse.NewTask
+    new_result: EventSubscriptionResponse.NewResult
     def __init__(self, session_id: _Optional[str] = ..., task_status_update: _Optional[_Union[EventSubscriptionResponse.TaskStatusUpdate, _Mapping]] = ..., result_status_update: _Optional[_Union[EventSubscriptionResponse.ResultStatusUpdate, _Mapping]] = ..., result_owner_update: _Optional[_Union[EventSubscriptionResponse.ResultOwnerUpdate, _Mapping]] = ..., new_task: _Optional[_Union[EventSubscriptionResponse.NewTask, _Mapping]] = ..., new_result: _Optional[_Union[EventSubscriptionResponse.NewResult, _Mapping]] = ...) -> None: ...
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/objects_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/common/objects_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,73 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: objects.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from . import task_status_pb2 as task__status__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\robjects.proto\x12\x13\x61rmonik.api.grpc.v1\x1a\x1egoogle/protobuf/duration.proto\x1a\x11task_status.proto\"\x07\n\x05\x45mpty\"\xf3\x02\n\x0bTaskOptions\x12>\n\x07options\x18\x01 \x03(\x0b\x32-.armonik.api.grpc.v1.TaskOptions.OptionsEntry\x12/\n\x0cmax_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x13\n\x0bmax_retries\x18\x03 \x01(\x05\x12\x10\n\x08priority\x18\x04 \x01(\x05\x12\x14\n\x0cpartition_id\x18\x05 \x01(\t\x12\x18\n\x10\x61pplication_name\x18\x06 \x01(\t\x12\x1b\n\x13\x61pplication_version\x18\x07 \x01(\t\x12\x1d\n\x15\x61pplication_namespace\x18\x08 \x01(\t\x12\x1b\n\x13\x61pplication_service\x18\t \x01(\t\x12\x13\n\x0b\x65ngine_type\x18\n \x01(\t\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x15\n\x07Session\x12\n\n\x02id\x18\x01 \x01(\t\",\n\rConfiguration\x12\x1b\n\x13\x64\x61ta_chunk_max_size\x18\x01 \x01(\x05\"\x88\x01\n\x06Output\x12(\n\x02ok\x18\x02 \x01(\x0b\x32\x1a.armonik.api.grpc.v1.EmptyH\x00\x12\x32\n\x05\x65rror\x18\x03 \x01(\x0b\x32!.armonik.api.grpc.v1.Output.ErrorH\x00\x1a\x18\n\x05\x45rror\x12\x0f\n\x07\x64\x65tails\x18\x01 \x01(\tB\x06\n\x04type\"m\n\x0bTaskRequest\x12\x1c\n\x14\x65xpected_output_keys\x18\x01 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x02 \x03(\t\x12\x0f\n\x07payload\x18\x03 \x01(\x0c\x12\x14\n\x0cpayload_name\x18\x04 \x01(\t\"C\n\x13InitKeyedDataStream\x12\r\n\x03key\x18\x01 \x01(\tH\x00\x12\x15\n\x0blast_result\x18\x02 \x01(\x08H\x00\x42\x06\n\x04type\"<\n\tDataChunk\x12\x0e\n\x04\x64\x61ta\x18\x01 \x01(\x0cH\x00\x12\x17\n\rdata_complete\x18\x02 \x01(\x08H\x00\x42\x06\n\x04type\"L\n\x11TaskRequestHeader\x12\x1c\n\x14\x65xpected_output_keys\x18\x01 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x02 \x03(\t\"h\n\x0fInitTaskRequest\x12\x38\n\x06header\x18\x01 \x01(\x0b\x32&.armonik.api.grpc.v1.TaskRequestHeaderH\x00\x12\x13\n\tlast_task\x18\x02 \x01(\x08H\x00\x42\x06\n\x04type\"\'\n\x06TaskId\x12\x0f\n\x07session\x18\x01 \x01(\t\x12\x0c\n\x04task\x18\x02 \x01(\t\"\x1e\n\nTaskIdList\x12\x10\n\x08task_ids\x18\x01 \x03(\t\"Y\n\x0bStatusCount\x12;\n\x06status\x18\x01 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12\r\n\x05\x63ount\x18\x02 \x01(\x05\"9\n\x05\x43ount\x12\x30\n\x06values\x18\x01 \x03(\x0b\x32 .armonik.api.grpc.v1.StatusCount\"3\n\rResultRequest\x12\x0f\n\x07session\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x01(\t\"5\n\x11TaskOutputRequest\x12\x0f\n\x07session\x18\x01 \x01(\t\x12\x0f\n\x07task_id\x18\x02 \x01(\t\"Y\n\x05\x45rror\x12@\n\x0btask_status\x18\x01 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12\x0e\n\x06\x64\x65tail\x18\x02 \x01(\t\"H\n\tTaskError\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12*\n\x06\x65rrors\x18\x02 \x03(\x0b\x32\x1a.armonik.api.grpc.v1.Error\"9\n\x08TaskList\x12-\n\x08task_ids\x18\x01 \x03(\x0b\x32\x1b.armonik.api.grpc.v1.TaskId\"}\n\x10TaskIdWithStatus\x12,\n\x07task_id\x18\x01 \x01(\x0b\x32\x1b.armonik.api.grpc.v1.TaskId\x12;\n\x06status\x18\x02 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatusB\x16\xaa\x02\x13\x41rmoniK.Api.gRPC.V1b\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'objects_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'objects_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\023ArmoniK.Api.gRPC.V1'
   _TASKOPTIONS_OPTIONSENTRY._options = None
   _TASKOPTIONS_OPTIONSENTRY._serialized_options = b'8\001'
-  _EMPTY._serialized_start=89
-  _EMPTY._serialized_end=96
-  _TASKOPTIONS._serialized_start=99
-  _TASKOPTIONS._serialized_end=470
-  _TASKOPTIONS_OPTIONSENTRY._serialized_start=424
-  _TASKOPTIONS_OPTIONSENTRY._serialized_end=470
-  _SESSION._serialized_start=472
-  _SESSION._serialized_end=493
-  _CONFIGURATION._serialized_start=495
-  _CONFIGURATION._serialized_end=539
-  _OUTPUT._serialized_start=542
-  _OUTPUT._serialized_end=678
-  _OUTPUT_ERROR._serialized_start=646
-  _OUTPUT_ERROR._serialized_end=670
-  _TASKREQUEST._serialized_start=680
-  _TASKREQUEST._serialized_end=789
-  _INITKEYEDDATASTREAM._serialized_start=791
-  _INITKEYEDDATASTREAM._serialized_end=858
-  _DATACHUNK._serialized_start=860
-  _DATACHUNK._serialized_end=920
-  _TASKREQUESTHEADER._serialized_start=922
-  _TASKREQUESTHEADER._serialized_end=998
-  _INITTASKREQUEST._serialized_start=1000
-  _INITTASKREQUEST._serialized_end=1104
-  _TASKID._serialized_start=1106
-  _TASKID._serialized_end=1145
-  _TASKIDLIST._serialized_start=1147
-  _TASKIDLIST._serialized_end=1177
-  _STATUSCOUNT._serialized_start=1179
-  _STATUSCOUNT._serialized_end=1268
-  _COUNT._serialized_start=1270
-  _COUNT._serialized_end=1327
-  _RESULTREQUEST._serialized_start=1329
-  _RESULTREQUEST._serialized_end=1380
-  _TASKOUTPUTREQUEST._serialized_start=1382
-  _TASKOUTPUTREQUEST._serialized_end=1435
-  _ERROR._serialized_start=1437
-  _ERROR._serialized_end=1526
-  _TASKERROR._serialized_start=1528
-  _TASKERROR._serialized_end=1600
-  _TASKLIST._serialized_start=1602
-  _TASKLIST._serialized_end=1659
-  _TASKIDWITHSTATUS._serialized_start=1661
-  _TASKIDWITHSTATUS._serialized_end=1786
+  _globals['_EMPTY']._serialized_start=89
+  _globals['_EMPTY']._serialized_end=96
+  _globals['_TASKOPTIONS']._serialized_start=99
+  _globals['_TASKOPTIONS']._serialized_end=470
+  _globals['_TASKOPTIONS_OPTIONSENTRY']._serialized_start=424
+  _globals['_TASKOPTIONS_OPTIONSENTRY']._serialized_end=470
+  _globals['_SESSION']._serialized_start=472
+  _globals['_SESSION']._serialized_end=493
+  _globals['_CONFIGURATION']._serialized_start=495
+  _globals['_CONFIGURATION']._serialized_end=539
+  _globals['_OUTPUT']._serialized_start=542
+  _globals['_OUTPUT']._serialized_end=678
+  _globals['_OUTPUT_ERROR']._serialized_start=646
+  _globals['_OUTPUT_ERROR']._serialized_end=670
+  _globals['_TASKREQUEST']._serialized_start=680
+  _globals['_TASKREQUEST']._serialized_end=789
+  _globals['_INITKEYEDDATASTREAM']._serialized_start=791
+  _globals['_INITKEYEDDATASTREAM']._serialized_end=858
+  _globals['_DATACHUNK']._serialized_start=860
+  _globals['_DATACHUNK']._serialized_end=920
+  _globals['_TASKREQUESTHEADER']._serialized_start=922
+  _globals['_TASKREQUESTHEADER']._serialized_end=998
+  _globals['_INITTASKREQUEST']._serialized_start=1000
+  _globals['_INITTASKREQUEST']._serialized_end=1104
+  _globals['_TASKID']._serialized_start=1106
+  _globals['_TASKID']._serialized_end=1145
+  _globals['_TASKIDLIST']._serialized_start=1147
+  _globals['_TASKIDLIST']._serialized_end=1177
+  _globals['_STATUSCOUNT']._serialized_start=1179
+  _globals['_STATUSCOUNT']._serialized_end=1268
+  _globals['_COUNT']._serialized_start=1270
+  _globals['_COUNT']._serialized_end=1327
+  _globals['_RESULTREQUEST']._serialized_start=1329
+  _globals['_RESULTREQUEST']._serialized_end=1380
+  _globals['_TASKOUTPUTREQUEST']._serialized_start=1382
+  _globals['_TASKOUTPUTREQUEST']._serialized_end=1435
+  _globals['_ERROR']._serialized_start=1437
+  _globals['_ERROR']._serialized_end=1526
+  _globals['_TASKERROR']._serialized_start=1528
+  _globals['_TASKERROR']._serialized_end=1600
+  _globals['_TASKLIST']._serialized_start=1602
+  _globals['_TASKLIST']._serialized_end=1659
+  _globals['_TASKIDWITHSTATUS']._serialized_start=1661
+  _globals['_TASKIDWITHSTATUS']._serialized_end=1786
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/objects_pb2.pyi` & `armonik-3.8.2.dev349/src/armonik/protogen/common/objects_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -3,184 +3,184 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
+class Empty(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
+
+class TaskOptions(_message.Message):
+    __slots__ = ["options", "max_duration", "max_retries", "priority", "partition_id", "application_name", "application_version", "application_namespace", "application_service", "engine_type"]
+    class OptionsEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    OPTIONS_FIELD_NUMBER: _ClassVar[int]
+    MAX_DURATION_FIELD_NUMBER: _ClassVar[int]
+    MAX_RETRIES_FIELD_NUMBER: _ClassVar[int]
+    PRIORITY_FIELD_NUMBER: _ClassVar[int]
+    PARTITION_ID_FIELD_NUMBER: _ClassVar[int]
+    APPLICATION_NAME_FIELD_NUMBER: _ClassVar[int]
+    APPLICATION_VERSION_FIELD_NUMBER: _ClassVar[int]
+    APPLICATION_NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    APPLICATION_SERVICE_FIELD_NUMBER: _ClassVar[int]
+    ENGINE_TYPE_FIELD_NUMBER: _ClassVar[int]
+    options: _containers.ScalarMap[str, str]
+    max_duration: _duration_pb2.Duration
+    max_retries: int
+    priority: int
+    partition_id: str
+    application_name: str
+    application_version: str
+    application_namespace: str
+    application_service: str
+    engine_type: str
+    def __init__(self, options: _Optional[_Mapping[str, str]] = ..., max_duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., max_retries: _Optional[int] = ..., priority: _Optional[int] = ..., partition_id: _Optional[str] = ..., application_name: _Optional[str] = ..., application_version: _Optional[str] = ..., application_namespace: _Optional[str] = ..., application_service: _Optional[str] = ..., engine_type: _Optional[str] = ...) -> None: ...
+
+class Session(_message.Message):
+    __slots__ = ["id"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    id: str
+    def __init__(self, id: _Optional[str] = ...) -> None: ...
+
 class Configuration(_message.Message):
     __slots__ = ["data_chunk_max_size"]
     DATA_CHUNK_MAX_SIZE_FIELD_NUMBER: _ClassVar[int]
     data_chunk_max_size: int
     def __init__(self, data_chunk_max_size: _Optional[int] = ...) -> None: ...
 
-class Count(_message.Message):
-    __slots__ = ["values"]
-    VALUES_FIELD_NUMBER: _ClassVar[int]
-    values: _containers.RepeatedCompositeFieldContainer[StatusCount]
-    def __init__(self, values: _Optional[_Iterable[_Union[StatusCount, _Mapping]]] = ...) -> None: ...
-
-class DataChunk(_message.Message):
-    __slots__ = ["data", "data_complete"]
-    DATA_COMPLETE_FIELD_NUMBER: _ClassVar[int]
-    DATA_FIELD_NUMBER: _ClassVar[int]
-    data: bytes
-    data_complete: bool
-    def __init__(self, data: _Optional[bytes] = ..., data_complete: bool = ...) -> None: ...
-
-class Empty(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
+class Output(_message.Message):
+    __slots__ = ["ok", "error"]
+    class Error(_message.Message):
+        __slots__ = ["details"]
+        DETAILS_FIELD_NUMBER: _ClassVar[int]
+        details: str
+        def __init__(self, details: _Optional[str] = ...) -> None: ...
+    OK_FIELD_NUMBER: _ClassVar[int]
+    ERROR_FIELD_NUMBER: _ClassVar[int]
+    ok: Empty
+    error: Output.Error
+    def __init__(self, ok: _Optional[_Union[Empty, _Mapping]] = ..., error: _Optional[_Union[Output.Error, _Mapping]] = ...) -> None: ...
 
-class Error(_message.Message):
-    __slots__ = ["detail", "task_status"]
-    DETAIL_FIELD_NUMBER: _ClassVar[int]
-    TASK_STATUS_FIELD_NUMBER: _ClassVar[int]
-    detail: str
-    task_status: _task_status_pb2.TaskStatus
-    def __init__(self, task_status: _Optional[_Union[_task_status_pb2.TaskStatus, str]] = ..., detail: _Optional[str] = ...) -> None: ...
+class TaskRequest(_message.Message):
+    __slots__ = ["expected_output_keys", "data_dependencies", "payload", "payload_name"]
+    EXPECTED_OUTPUT_KEYS_FIELD_NUMBER: _ClassVar[int]
+    DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
+    PAYLOAD_FIELD_NUMBER: _ClassVar[int]
+    PAYLOAD_NAME_FIELD_NUMBER: _ClassVar[int]
+    expected_output_keys: _containers.RepeatedScalarFieldContainer[str]
+    data_dependencies: _containers.RepeatedScalarFieldContainer[str]
+    payload: bytes
+    payload_name: str
+    def __init__(self, expected_output_keys: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., payload: _Optional[bytes] = ..., payload_name: _Optional[str] = ...) -> None: ...
 
 class InitKeyedDataStream(_message.Message):
     __slots__ = ["key", "last_result"]
     KEY_FIELD_NUMBER: _ClassVar[int]
     LAST_RESULT_FIELD_NUMBER: _ClassVar[int]
     key: str
     last_result: bool
     def __init__(self, key: _Optional[str] = ..., last_result: bool = ...) -> None: ...
 
+class DataChunk(_message.Message):
+    __slots__ = ["data", "data_complete"]
+    DATA_FIELD_NUMBER: _ClassVar[int]
+    DATA_COMPLETE_FIELD_NUMBER: _ClassVar[int]
+    data: bytes
+    data_complete: bool
+    def __init__(self, data: _Optional[bytes] = ..., data_complete: bool = ...) -> None: ...
+
+class TaskRequestHeader(_message.Message):
+    __slots__ = ["expected_output_keys", "data_dependencies"]
+    EXPECTED_OUTPUT_KEYS_FIELD_NUMBER: _ClassVar[int]
+    DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
+    expected_output_keys: _containers.RepeatedScalarFieldContainer[str]
+    data_dependencies: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, expected_output_keys: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ...) -> None: ...
+
 class InitTaskRequest(_message.Message):
     __slots__ = ["header", "last_task"]
     HEADER_FIELD_NUMBER: _ClassVar[int]
     LAST_TASK_FIELD_NUMBER: _ClassVar[int]
     header: TaskRequestHeader
     last_task: bool
     def __init__(self, header: _Optional[_Union[TaskRequestHeader, _Mapping]] = ..., last_task: bool = ...) -> None: ...
 
-class Output(_message.Message):
-    __slots__ = ["error", "ok"]
-    class Error(_message.Message):
-        __slots__ = ["details"]
-        DETAILS_FIELD_NUMBER: _ClassVar[int]
-        details: str
-        def __init__(self, details: _Optional[str] = ...) -> None: ...
-    ERROR_FIELD_NUMBER: _ClassVar[int]
-    OK_FIELD_NUMBER: _ClassVar[int]
-    error: Output.Error
-    ok: Empty
-    def __init__(self, ok: _Optional[_Union[Empty, _Mapping]] = ..., error: _Optional[_Union[Output.Error, _Mapping]] = ...) -> None: ...
-
-class ResultRequest(_message.Message):
-    __slots__ = ["result_id", "session"]
-    RESULT_ID_FIELD_NUMBER: _ClassVar[int]
-    SESSION_FIELD_NUMBER: _ClassVar[int]
-    result_id: str
-    session: str
-    def __init__(self, session: _Optional[str] = ..., result_id: _Optional[str] = ...) -> None: ...
-
-class Session(_message.Message):
-    __slots__ = ["id"]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    id: str
-    def __init__(self, id: _Optional[str] = ...) -> None: ...
-
-class StatusCount(_message.Message):
-    __slots__ = ["count", "status"]
-    COUNT_FIELD_NUMBER: _ClassVar[int]
-    STATUS_FIELD_NUMBER: _ClassVar[int]
-    count: int
-    status: _task_status_pb2.TaskStatus
-    def __init__(self, status: _Optional[_Union[_task_status_pb2.TaskStatus, str]] = ..., count: _Optional[int] = ...) -> None: ...
-
-class TaskError(_message.Message):
-    __slots__ = ["errors", "task_id"]
-    ERRORS_FIELD_NUMBER: _ClassVar[int]
-    TASK_ID_FIELD_NUMBER: _ClassVar[int]
-    errors: _containers.RepeatedCompositeFieldContainer[Error]
-    task_id: str
-    def __init__(self, task_id: _Optional[str] = ..., errors: _Optional[_Iterable[_Union[Error, _Mapping]]] = ...) -> None: ...
-
 class TaskId(_message.Message):
     __slots__ = ["session", "task"]
     SESSION_FIELD_NUMBER: _ClassVar[int]
     TASK_FIELD_NUMBER: _ClassVar[int]
     session: str
     task: str
     def __init__(self, session: _Optional[str] = ..., task: _Optional[str] = ...) -> None: ...
 
 class TaskIdList(_message.Message):
     __slots__ = ["task_ids"]
     TASK_IDS_FIELD_NUMBER: _ClassVar[int]
     task_ids: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, task_ids: _Optional[_Iterable[str]] = ...) -> None: ...
 
-class TaskIdWithStatus(_message.Message):
-    __slots__ = ["status", "task_id"]
+class StatusCount(_message.Message):
+    __slots__ = ["status", "count"]
     STATUS_FIELD_NUMBER: _ClassVar[int]
-    TASK_ID_FIELD_NUMBER: _ClassVar[int]
+    COUNT_FIELD_NUMBER: _ClassVar[int]
     status: _task_status_pb2.TaskStatus
-    task_id: TaskId
-    def __init__(self, task_id: _Optional[_Union[TaskId, _Mapping]] = ..., status: _Optional[_Union[_task_status_pb2.TaskStatus, str]] = ...) -> None: ...
+    count: int
+    def __init__(self, status: _Optional[_Union[_task_status_pb2.TaskStatus, str]] = ..., count: _Optional[int] = ...) -> None: ...
 
-class TaskList(_message.Message):
-    __slots__ = ["task_ids"]
-    TASK_IDS_FIELD_NUMBER: _ClassVar[int]
-    task_ids: _containers.RepeatedCompositeFieldContainer[TaskId]
-    def __init__(self, task_ids: _Optional[_Iterable[_Union[TaskId, _Mapping]]] = ...) -> None: ...
+class Count(_message.Message):
+    __slots__ = ["values"]
+    VALUES_FIELD_NUMBER: _ClassVar[int]
+    values: _containers.RepeatedCompositeFieldContainer[StatusCount]
+    def __init__(self, values: _Optional[_Iterable[_Union[StatusCount, _Mapping]]] = ...) -> None: ...
 
-class TaskOptions(_message.Message):
-    __slots__ = ["application_name", "application_namespace", "application_service", "application_version", "engine_type", "max_duration", "max_retries", "options", "partition_id", "priority"]
-    class OptionsEntry(_message.Message):
-        __slots__ = ["key", "value"]
-        KEY_FIELD_NUMBER: _ClassVar[int]
-        VALUE_FIELD_NUMBER: _ClassVar[int]
-        key: str
-        value: str
-        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
-    APPLICATION_NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    APPLICATION_NAME_FIELD_NUMBER: _ClassVar[int]
-    APPLICATION_SERVICE_FIELD_NUMBER: _ClassVar[int]
-    APPLICATION_VERSION_FIELD_NUMBER: _ClassVar[int]
-    ENGINE_TYPE_FIELD_NUMBER: _ClassVar[int]
-    MAX_DURATION_FIELD_NUMBER: _ClassVar[int]
-    MAX_RETRIES_FIELD_NUMBER: _ClassVar[int]
-    OPTIONS_FIELD_NUMBER: _ClassVar[int]
-    PARTITION_ID_FIELD_NUMBER: _ClassVar[int]
-    PRIORITY_FIELD_NUMBER: _ClassVar[int]
-    application_name: str
-    application_namespace: str
-    application_service: str
-    application_version: str
-    engine_type: str
-    max_duration: _duration_pb2.Duration
-    max_retries: int
-    options: _containers.ScalarMap[str, str]
-    partition_id: str
-    priority: int
-    def __init__(self, options: _Optional[_Mapping[str, str]] = ..., max_duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., max_retries: _Optional[int] = ..., priority: _Optional[int] = ..., partition_id: _Optional[str] = ..., application_name: _Optional[str] = ..., application_version: _Optional[str] = ..., application_namespace: _Optional[str] = ..., application_service: _Optional[str] = ..., engine_type: _Optional[str] = ...) -> None: ...
+class ResultRequest(_message.Message):
+    __slots__ = ["session", "result_id"]
+    SESSION_FIELD_NUMBER: _ClassVar[int]
+    RESULT_ID_FIELD_NUMBER: _ClassVar[int]
+    session: str
+    result_id: str
+    def __init__(self, session: _Optional[str] = ..., result_id: _Optional[str] = ...) -> None: ...
 
 class TaskOutputRequest(_message.Message):
     __slots__ = ["session", "task_id"]
     SESSION_FIELD_NUMBER: _ClassVar[int]
     TASK_ID_FIELD_NUMBER: _ClassVar[int]
     session: str
     task_id: str
     def __init__(self, session: _Optional[str] = ..., task_id: _Optional[str] = ...) -> None: ...
 
-class TaskRequest(_message.Message):
-    __slots__ = ["data_dependencies", "expected_output_keys", "payload", "payload_name"]
-    DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
-    EXPECTED_OUTPUT_KEYS_FIELD_NUMBER: _ClassVar[int]
-    PAYLOAD_FIELD_NUMBER: _ClassVar[int]
-    PAYLOAD_NAME_FIELD_NUMBER: _ClassVar[int]
-    data_dependencies: _containers.RepeatedScalarFieldContainer[str]
-    expected_output_keys: _containers.RepeatedScalarFieldContainer[str]
-    payload: bytes
-    payload_name: str
-    def __init__(self, expected_output_keys: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., payload: _Optional[bytes] = ..., payload_name: _Optional[str] = ...) -> None: ...
+class Error(_message.Message):
+    __slots__ = ["task_status", "detail"]
+    TASK_STATUS_FIELD_NUMBER: _ClassVar[int]
+    DETAIL_FIELD_NUMBER: _ClassVar[int]
+    task_status: _task_status_pb2.TaskStatus
+    detail: str
+    def __init__(self, task_status: _Optional[_Union[_task_status_pb2.TaskStatus, str]] = ..., detail: _Optional[str] = ...) -> None: ...
 
-class TaskRequestHeader(_message.Message):
-    __slots__ = ["data_dependencies", "expected_output_keys"]
-    DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
-    EXPECTED_OUTPUT_KEYS_FIELD_NUMBER: _ClassVar[int]
-    data_dependencies: _containers.RepeatedScalarFieldContainer[str]
-    expected_output_keys: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, expected_output_keys: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ...) -> None: ...
+class TaskError(_message.Message):
+    __slots__ = ["task_id", "errors"]
+    TASK_ID_FIELD_NUMBER: _ClassVar[int]
+    ERRORS_FIELD_NUMBER: _ClassVar[int]
+    task_id: str
+    errors: _containers.RepeatedCompositeFieldContainer[Error]
+    def __init__(self, task_id: _Optional[str] = ..., errors: _Optional[_Iterable[_Union[Error, _Mapping]]] = ...) -> None: ...
+
+class TaskList(_message.Message):
+    __slots__ = ["task_ids"]
+    TASK_IDS_FIELD_NUMBER: _ClassVar[int]
+    task_ids: _containers.RepeatedCompositeFieldContainer[TaskId]
+    def __init__(self, task_ids: _Optional[_Iterable[_Union[TaskId, _Mapping]]] = ...) -> None: ...
+
+class TaskIdWithStatus(_message.Message):
+    __slots__ = ["task_id", "status"]
+    TASK_ID_FIELD_NUMBER: _ClassVar[int]
+    STATUS_FIELD_NUMBER: _ClassVar[int]
+    task_id: TaskId
+    status: _task_status_pb2.TaskStatus
+    def __init__(self, task_id: _Optional[_Union[TaskId, _Mapping]] = ..., status: _Optional[_Union[_task_status_pb2.TaskStatus, str]] = ...) -> None: ...
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/partitions_common_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/common/partitions_common_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: partitions_common.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17partitions_common.proto\x12\x1e\x61rmonik.api.grpc.v1.partitions\"\xa8\x02\n\x0cPartitionRaw\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1c\n\x14parent_partition_ids\x18\x02 \x03(\t\x12\x14\n\x0cpod_reserved\x18\x03 \x01(\x03\x12\x0f\n\x07pod_max\x18\x04 \x01(\x03\x12]\n\x11pod_configuration\x18\x07 \x03(\x0b\x32\x42.armonik.api.grpc.v1.partitions.PartitionRaw.PodConfigurationEntry\x12\x1d\n\x15preemption_percentage\x18\x05 \x01(\x03\x12\x10\n\x08priority\x18\x06 \x01(\x03\x1a\x37\n\x15PodConfigurationEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xec\x06\n\x15ListPartitionsRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12L\n\x06\x66ilter\x18\x03 \x01(\x0b\x32<.armonik.api.grpc.v1.partitions.ListPartitionsRequest.Filter\x12H\n\x04sort\x18\x04 \x01(\x0b\x32:.armonik.api.grpc.v1.partitions.ListPartitionsRequest.Sort\x1a\x89\x01\n\x06\x46ilter\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1b\n\x13parent_partition_id\x18\x02 \x01(\t\x12\x14\n\x0cpod_reserved\x18\x03 \x01(\x05\x12\x0f\n\x07pod_max\x18\x04 \x01(\x05\x12\x1d\n\x15preemption_percentage\x18\x05 \x01(\x05\x12\x10\n\x08priority\x18\x06 \x01(\x05\x1a\xb2\x01\n\x04Sort\x12Q\n\x05\x66ield\x18\x01 \x01(\x0e\x32\x42.armonik.api.grpc.v1.partitions.ListPartitionsRequest.OrderByField\x12W\n\tdirection\x18\x02 \x01(\x0e\x32\x44.armonik.api.grpc.v1.partitions.ListPartitionsRequest.OrderDirection\"\xf2\x01\n\x0cOrderByField\x12\x1e\n\x1aORDER_BY_FIELD_UNSPECIFIED\x10\x00\x12\x15\n\x11ORDER_BY_FIELD_ID\x10\x01\x12\'\n#ORDER_BY_FIELD_PARENT_PARTITION_IDS\x10\x02\x12\x1f\n\x1bORDER_BY_FIELD_POD_RESERVED\x10\x03\x12\x1a\n\x16ORDER_BY_FIELD_POD_MAX\x10\x04\x12(\n$ORDER_BY_FIELD_PREEMPTION_PERCENTAGE\x10\x05\x12\x1b\n\x17ORDER_BY_FIELD_PRIORITY\x10\x06\"d\n\x0eOrderDirection\x12\x1f\n\x1bORDER_DIRECTION_UNSPECIFIED\x10\x00\x12\x17\n\x13ORDER_DIRECTION_ASC\x10\x01\x12\x18\n\x14ORDER_DIRECTION_DESC\x10\x02\"\x8a\x01\n\x16ListPartitionsResponse\x12@\n\npartitions\x18\x01 \x03(\x0b\x32,.armonik.api.grpc.v1.partitions.PartitionRaw\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"!\n\x13GetPartitionRequest\x12\n\n\x02id\x18\x01 \x01(\t\"W\n\x14GetPartitionResponse\x12?\n\tpartition\x18\x01 \x01(\x0b\x32,.armonik.api.grpc.v1.partitions.PartitionRawB!\xaa\x02\x1e\x41rmonik.Api.Grpc.V1.Partitionsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'partitions_common_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'partitions_common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\036Armonik.Api.Grpc.V1.Partitions'
   _PARTITIONRAW_PODCONFIGURATIONENTRY._options = None
   _PARTITIONRAW_PODCONFIGURATIONENTRY._serialized_options = b'8\001'
-  _PARTITIONRAW._serialized_start=60
-  _PARTITIONRAW._serialized_end=356
-  _PARTITIONRAW_PODCONFIGURATIONENTRY._serialized_start=301
-  _PARTITIONRAW_PODCONFIGURATIONENTRY._serialized_end=356
-  _LISTPARTITIONSREQUEST._serialized_start=359
-  _LISTPARTITIONSREQUEST._serialized_end=1235
-  _LISTPARTITIONSREQUEST_FILTER._serialized_start=570
-  _LISTPARTITIONSREQUEST_FILTER._serialized_end=707
-  _LISTPARTITIONSREQUEST_SORT._serialized_start=710
-  _LISTPARTITIONSREQUEST_SORT._serialized_end=888
-  _LISTPARTITIONSREQUEST_ORDERBYFIELD._serialized_start=891
-  _LISTPARTITIONSREQUEST_ORDERBYFIELD._serialized_end=1133
-  _LISTPARTITIONSREQUEST_ORDERDIRECTION._serialized_start=1135
-  _LISTPARTITIONSREQUEST_ORDERDIRECTION._serialized_end=1235
-  _LISTPARTITIONSRESPONSE._serialized_start=1238
-  _LISTPARTITIONSRESPONSE._serialized_end=1376
-  _GETPARTITIONREQUEST._serialized_start=1378
-  _GETPARTITIONREQUEST._serialized_end=1411
-  _GETPARTITIONRESPONSE._serialized_start=1413
-  _GETPARTITIONRESPONSE._serialized_end=1500
+  _globals['_PARTITIONRAW']._serialized_start=60
+  _globals['_PARTITIONRAW']._serialized_end=356
+  _globals['_PARTITIONRAW_PODCONFIGURATIONENTRY']._serialized_start=301
+  _globals['_PARTITIONRAW_PODCONFIGURATIONENTRY']._serialized_end=356
+  _globals['_LISTPARTITIONSREQUEST']._serialized_start=359
+  _globals['_LISTPARTITIONSREQUEST']._serialized_end=1235
+  _globals['_LISTPARTITIONSREQUEST_FILTER']._serialized_start=570
+  _globals['_LISTPARTITIONSREQUEST_FILTER']._serialized_end=707
+  _globals['_LISTPARTITIONSREQUEST_SORT']._serialized_start=710
+  _globals['_LISTPARTITIONSREQUEST_SORT']._serialized_end=888
+  _globals['_LISTPARTITIONSREQUEST_ORDERBYFIELD']._serialized_start=891
+  _globals['_LISTPARTITIONSREQUEST_ORDERBYFIELD']._serialized_end=1133
+  _globals['_LISTPARTITIONSREQUEST_ORDERDIRECTION']._serialized_start=1135
+  _globals['_LISTPARTITIONSREQUEST_ORDERDIRECTION']._serialized_end=1235
+  _globals['_LISTPARTITIONSRESPONSE']._serialized_start=1238
+  _globals['_LISTPARTITIONSRESPONSE']._serialized_end=1376
+  _globals['_GETPARTITIONREQUEST']._serialized_start=1378
+  _globals['_GETPARTITIONREQUEST']._serialized_end=1411
+  _globals['_GETPARTITIONRESPONSE']._serialized_start=1413
+  _globals['_GETPARTITIONRESPONSE']._serialized_end=1500
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/partitions_common_pb2.pyi` & `armonik-3.8.2.dev349/src/armonik/protogen/common/partitions_common_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -2,103 +2,113 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class GetPartitionRequest(_message.Message):
-    __slots__ = ["id"]
+class PartitionRaw(_message.Message):
+    __slots__ = ["id", "parent_partition_ids", "pod_reserved", "pod_max", "pod_configuration", "preemption_percentage", "priority"]
+    class PodConfigurationEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
     ID_FIELD_NUMBER: _ClassVar[int]
+    PARENT_PARTITION_IDS_FIELD_NUMBER: _ClassVar[int]
+    POD_RESERVED_FIELD_NUMBER: _ClassVar[int]
+    POD_MAX_FIELD_NUMBER: _ClassVar[int]
+    POD_CONFIGURATION_FIELD_NUMBER: _ClassVar[int]
+    PREEMPTION_PERCENTAGE_FIELD_NUMBER: _ClassVar[int]
+    PRIORITY_FIELD_NUMBER: _ClassVar[int]
     id: str
-    def __init__(self, id: _Optional[str] = ...) -> None: ...
-
-class GetPartitionResponse(_message.Message):
-    __slots__ = ["partition"]
-    PARTITION_FIELD_NUMBER: _ClassVar[int]
-    partition: PartitionRaw
-    def __init__(self, partition: _Optional[_Union[PartitionRaw, _Mapping]] = ...) -> None: ...
+    parent_partition_ids: _containers.RepeatedScalarFieldContainer[str]
+    pod_reserved: int
+    pod_max: int
+    pod_configuration: _containers.ScalarMap[str, str]
+    preemption_percentage: int
+    priority: int
+    def __init__(self, id: _Optional[str] = ..., parent_partition_ids: _Optional[_Iterable[str]] = ..., pod_reserved: _Optional[int] = ..., pod_max: _Optional[int] = ..., pod_configuration: _Optional[_Mapping[str, str]] = ..., preemption_percentage: _Optional[int] = ..., priority: _Optional[int] = ...) -> None: ...
 
 class ListPartitionsRequest(_message.Message):
-    __slots__ = ["filter", "page", "page_size", "sort"]
+    __slots__ = ["page", "page_size", "filter", "sort"]
     class OrderByField(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        ORDER_BY_FIELD_UNSPECIFIED: _ClassVar[ListPartitionsRequest.OrderByField]
+        ORDER_BY_FIELD_ID: _ClassVar[ListPartitionsRequest.OrderByField]
+        ORDER_BY_FIELD_PARENT_PARTITION_IDS: _ClassVar[ListPartitionsRequest.OrderByField]
+        ORDER_BY_FIELD_POD_RESERVED: _ClassVar[ListPartitionsRequest.OrderByField]
+        ORDER_BY_FIELD_POD_MAX: _ClassVar[ListPartitionsRequest.OrderByField]
+        ORDER_BY_FIELD_PREEMPTION_PERCENTAGE: _ClassVar[ListPartitionsRequest.OrderByField]
+        ORDER_BY_FIELD_PRIORITY: _ClassVar[ListPartitionsRequest.OrderByField]
+    ORDER_BY_FIELD_UNSPECIFIED: ListPartitionsRequest.OrderByField
+    ORDER_BY_FIELD_ID: ListPartitionsRequest.OrderByField
+    ORDER_BY_FIELD_PARENT_PARTITION_IDS: ListPartitionsRequest.OrderByField
+    ORDER_BY_FIELD_POD_RESERVED: ListPartitionsRequest.OrderByField
+    ORDER_BY_FIELD_POD_MAX: ListPartitionsRequest.OrderByField
+    ORDER_BY_FIELD_PREEMPTION_PERCENTAGE: ListPartitionsRequest.OrderByField
+    ORDER_BY_FIELD_PRIORITY: ListPartitionsRequest.OrderByField
     class OrderDirection(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        ORDER_DIRECTION_UNSPECIFIED: _ClassVar[ListPartitionsRequest.OrderDirection]
+        ORDER_DIRECTION_ASC: _ClassVar[ListPartitionsRequest.OrderDirection]
+        ORDER_DIRECTION_DESC: _ClassVar[ListPartitionsRequest.OrderDirection]
+    ORDER_DIRECTION_UNSPECIFIED: ListPartitionsRequest.OrderDirection
+    ORDER_DIRECTION_ASC: ListPartitionsRequest.OrderDirection
+    ORDER_DIRECTION_DESC: ListPartitionsRequest.OrderDirection
     class Filter(_message.Message):
-        __slots__ = ["id", "parent_partition_id", "pod_max", "pod_reserved", "preemption_percentage", "priority"]
+        __slots__ = ["id", "parent_partition_id", "pod_reserved", "pod_max", "preemption_percentage", "priority"]
         ID_FIELD_NUMBER: _ClassVar[int]
         PARENT_PARTITION_ID_FIELD_NUMBER: _ClassVar[int]
-        POD_MAX_FIELD_NUMBER: _ClassVar[int]
         POD_RESERVED_FIELD_NUMBER: _ClassVar[int]
+        POD_MAX_FIELD_NUMBER: _ClassVar[int]
         PREEMPTION_PERCENTAGE_FIELD_NUMBER: _ClassVar[int]
         PRIORITY_FIELD_NUMBER: _ClassVar[int]
         id: str
         parent_partition_id: str
-        pod_max: int
         pod_reserved: int
+        pod_max: int
         preemption_percentage: int
         priority: int
         def __init__(self, id: _Optional[str] = ..., parent_partition_id: _Optional[str] = ..., pod_reserved: _Optional[int] = ..., pod_max: _Optional[int] = ..., preemption_percentage: _Optional[int] = ..., priority: _Optional[int] = ...) -> None: ...
     class Sort(_message.Message):
-        __slots__ = ["direction", "field"]
-        DIRECTION_FIELD_NUMBER: _ClassVar[int]
+        __slots__ = ["field", "direction"]
         FIELD_FIELD_NUMBER: _ClassVar[int]
-        direction: ListPartitionsRequest.OrderDirection
+        DIRECTION_FIELD_NUMBER: _ClassVar[int]
         field: ListPartitionsRequest.OrderByField
+        direction: ListPartitionsRequest.OrderDirection
         def __init__(self, field: _Optional[_Union[ListPartitionsRequest.OrderByField, str]] = ..., direction: _Optional[_Union[ListPartitionsRequest.OrderDirection, str]] = ...) -> None: ...
-    FILTER_FIELD_NUMBER: _ClassVar[int]
-    ORDER_BY_FIELD_ID: ListPartitionsRequest.OrderByField
-    ORDER_BY_FIELD_PARENT_PARTITION_IDS: ListPartitionsRequest.OrderByField
-    ORDER_BY_FIELD_POD_MAX: ListPartitionsRequest.OrderByField
-    ORDER_BY_FIELD_POD_RESERVED: ListPartitionsRequest.OrderByField
-    ORDER_BY_FIELD_PREEMPTION_PERCENTAGE: ListPartitionsRequest.OrderByField
-    ORDER_BY_FIELD_PRIORITY: ListPartitionsRequest.OrderByField
-    ORDER_BY_FIELD_UNSPECIFIED: ListPartitionsRequest.OrderByField
-    ORDER_DIRECTION_ASC: ListPartitionsRequest.OrderDirection
-    ORDER_DIRECTION_DESC: ListPartitionsRequest.OrderDirection
-    ORDER_DIRECTION_UNSPECIFIED: ListPartitionsRequest.OrderDirection
     PAGE_FIELD_NUMBER: _ClassVar[int]
     PAGE_SIZE_FIELD_NUMBER: _ClassVar[int]
+    FILTER_FIELD_NUMBER: _ClassVar[int]
     SORT_FIELD_NUMBER: _ClassVar[int]
-    filter: ListPartitionsRequest.Filter
     page: int
     page_size: int
+    filter: ListPartitionsRequest.Filter
     sort: ListPartitionsRequest.Sort
     def __init__(self, page: _Optional[int] = ..., page_size: _Optional[int] = ..., filter: _Optional[_Union[ListPartitionsRequest.Filter, _Mapping]] = ..., sort: _Optional[_Union[ListPartitionsRequest.Sort, _Mapping]] = ...) -> None: ...
 
 class ListPartitionsResponse(_message.Message):
-    __slots__ = ["page", "page_size", "partitions", "total"]
+    __slots__ = ["partitions", "page", "page_size", "total"]
+    PARTITIONS_FIELD_NUMBER: _ClassVar[int]
     PAGE_FIELD_NUMBER: _ClassVar[int]
     PAGE_SIZE_FIELD_NUMBER: _ClassVar[int]
-    PARTITIONS_FIELD_NUMBER: _ClassVar[int]
     TOTAL_FIELD_NUMBER: _ClassVar[int]
+    partitions: _containers.RepeatedCompositeFieldContainer[PartitionRaw]
     page: int
     page_size: int
-    partitions: _containers.RepeatedCompositeFieldContainer[PartitionRaw]
     total: int
     def __init__(self, partitions: _Optional[_Iterable[_Union[PartitionRaw, _Mapping]]] = ..., page: _Optional[int] = ..., page_size: _Optional[int] = ..., total: _Optional[int] = ...) -> None: ...
 
-class PartitionRaw(_message.Message):
-    __slots__ = ["id", "parent_partition_ids", "pod_configuration", "pod_max", "pod_reserved", "preemption_percentage", "priority"]
-    class PodConfigurationEntry(_message.Message):
-        __slots__ = ["key", "value"]
-        KEY_FIELD_NUMBER: _ClassVar[int]
-        VALUE_FIELD_NUMBER: _ClassVar[int]
-        key: str
-        value: str
-        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+class GetPartitionRequest(_message.Message):
+    __slots__ = ["id"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    PARENT_PARTITION_IDS_FIELD_NUMBER: _ClassVar[int]
-    POD_CONFIGURATION_FIELD_NUMBER: _ClassVar[int]
-    POD_MAX_FIELD_NUMBER: _ClassVar[int]
-    POD_RESERVED_FIELD_NUMBER: _ClassVar[int]
-    PREEMPTION_PERCENTAGE_FIELD_NUMBER: _ClassVar[int]
-    PRIORITY_FIELD_NUMBER: _ClassVar[int]
     id: str
-    parent_partition_ids: _containers.RepeatedScalarFieldContainer[str]
-    pod_configuration: _containers.ScalarMap[str, str]
-    pod_max: int
-    pod_reserved: int
-    preemption_percentage: int
-    priority: int
-    def __init__(self, id: _Optional[str] = ..., parent_partition_ids: _Optional[_Iterable[str]] = ..., pod_reserved: _Optional[int] = ..., pod_max: _Optional[int] = ..., pod_configuration: _Optional[_Mapping[str, str]] = ..., preemption_percentage: _Optional[int] = ..., priority: _Optional[int] = ...) -> None: ...
+    def __init__(self, id: _Optional[str] = ...) -> None: ...
+
+class GetPartitionResponse(_message.Message):
+    __slots__ = ["partition"]
+    PARTITION_FIELD_NUMBER: _ClassVar[int]
+    partition: PartitionRaw
+    def __init__(self, partition: _Optional[_Union[PartitionRaw, _Mapping]] = ...) -> None: ...
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/result_status_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/common/task_status_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: result_status.proto
+# source: task_status.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13result_status.proto\x12!armonik.api.grpc.v1.result_status*\x9c\x01\n\x0cResultStatus\x12\x1d\n\x19RESULT_STATUS_UNSPECIFIED\x10\x00\x12\x19\n\x15RESULT_STATUS_CREATED\x10\x01\x12\x1b\n\x17RESULT_STATUS_COMPLETED\x10\x02\x12\x19\n\x15RESULT_STATUS_ABORTED\x10\x03\x12\x1a\n\x16RESULT_STATUS_NOTFOUND\x10\x7f\x42\x16\xaa\x02\x13\x41rmoniK.Api.gRPC.V1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11task_status.proto\x12\x1f\x61rmonik.api.grpc.v1.task_status*\xcc\x02\n\nTaskStatus\x12\x1b\n\x17TASK_STATUS_UNSPECIFIED\x10\x00\x12\x18\n\x14TASK_STATUS_CREATING\x10\x01\x12\x19\n\x15TASK_STATUS_SUBMITTED\x10\x02\x12\x1a\n\x16TASK_STATUS_DISPATCHED\x10\x03\x12\x19\n\x15TASK_STATUS_COMPLETED\x10\x04\x12\x15\n\x11TASK_STATUS_ERROR\x10\x05\x12\x17\n\x13TASK_STATUS_TIMEOUT\x10\x06\x12\x1a\n\x16TASK_STATUS_CANCELLING\x10\x07\x12\x19\n\x15TASK_STATUS_CANCELLED\x10\x08\x12\x1a\n\x16TASK_STATUS_PROCESSING\x10\t\x12\x19\n\x15TASK_STATUS_PROCESSED\x10\n\x12\x17\n\x13TASK_STATUS_RETRIED\x10\x0b\x42\x16\xaa\x02\x13\x41rmoniK.Api.gRPC.V1b\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'result_status_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'task_status_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\023ArmoniK.Api.gRPC.V1'
-  _RESULTSTATUS._serialized_start=59
-  _RESULTSTATUS._serialized_end=215
+  _globals['_TASKSTATUS']._serialized_start=55
+  _globals['_TASKSTATUS']._serialized_end=387
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/results_common_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/common/results_common_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,75 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: results_common.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from . import result_status_pb2 as result__status__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14results_common.proto\x12\x1b\x61rmonik.api.grpc.v1.results\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x13result_status.proto\"\xb0\x02\n\tResultRaw\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rowner_task_id\x18\x03 \x01(\t\x12?\n\x06status\x18\x04 \x01(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63ompleted_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10wait_for_data_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tresult_id\x18\x08 \x01(\t\"\x90\t\n\x12ListResultsRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x46\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x36.armonik.api.grpc.v1.results.ListResultsRequest.Filter\x12\x42\n\x04sort\x18\x04 \x01(\x0b\x32\x34.armonik.api.grpc.v1.results.ListResultsRequest.Sort\x1a\xda\x03\n\x06\x46ilter\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rowner_task_id\x18\x03 \x01(\t\x12?\n\x06status\x18\x04 \x01(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\x12\x31\n\rcreated_after\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0e\x63reated_before\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0f\x63ompleted_after\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x63ompleted_before\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\x13wait_for_data_after\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x14wait_for_data_before\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tresult_id\x18\x0b \x01(\t\x1a\xa6\x01\n\x04Sort\x12K\n\x05\x66ield\x18\x01 \x01(\x0e\x32<.armonik.api.grpc.v1.results.ListResultsRequest.OrderByField\x12Q\n\tdirection\x18\x02 \x01(\x0e\x32>.armonik.api.grpc.v1.results.ListResultsRequest.OrderDirection\"\xe0\x01\n\x0cOrderByField\x12\x1e\n\x1aORDER_BY_FIELD_UNSPECIFIED\x10\x00\x12\x1d\n\x19ORDER_BY_FIELD_SESSION_ID\x10\x01\x12\x17\n\x13ORDER_BY_FIELD_NAME\x10\x02\x12 \n\x1cORDER_BY_FIELD_OWNER_TASK_ID\x10\x03\x12\x19\n\x15ORDER_BY_FIELD_STATUS\x10\x04\x12\x1d\n\x19ORDER_BY_FIELD_CREATED_AT\x10\x05\x12\x1c\n\x18ORDER_BY_FIELD_RESULT_ID\x10\x06\"d\n\x0eOrderDirection\x12\x1f\n\x1bORDER_DIRECTION_UNSPECIFIED\x10\x00\x12\x17\n\x13ORDER_DIRECTION_ASC\x10\x01\x12\x18\n\x14ORDER_DIRECTION_DESC\x10\x02\"~\n\x13ListResultsResponse\x12\x37\n\x07results\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\">\n\x15GetOwnerTaskIdRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x03(\t\"\xb9\x01\n\x16GetOwnerTaskIdResponse\x12V\n\x0bresult_task\x18\x01 \x03(\x0b\x32\x41.armonik.api.grpc.v1.results.GetOwnerTaskIdResponse.MapResultTask\x12\x12\n\nsession_id\x18\x02 \x01(\t\x1a\x33\n\rMapResultTask\x12\x11\n\tresult_id\x18\x01 \x01(\t\x12\x0f\n\x07task_id\x18\x02 \x01(\t\"\xa9\x01\n\x1c\x43reateResultsMetaDataRequest\x12W\n\x07results\x18\x01 \x03(\x0b\x32\x46.armonik.api.grpc.v1.results.CreateResultsMetaDataRequest.ResultCreate\x12\x12\n\nsession_id\x18\x02 \x01(\t\x1a\x1c\n\x0cResultCreate\x12\x0c\n\x04name\x18\x01 \x01(\t\"X\n\x1d\x43reateResultsMetaDataResponse\x12\x37\n\x07results\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\"\xa7\x01\n\x14\x43reateResultsRequest\x12O\n\x07results\x18\x01 \x03(\x0b\x32>.armonik.api.grpc.v1.results.CreateResultsRequest.ResultCreate\x12\x12\n\nsession_id\x18\x02 \x01(\t\x1a*\n\x0cResultCreate\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"P\n\x15\x43reateResultsResponse\x12\x37\n\x07results\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\"\xc7\x01\n\x17UploadResultDataRequest\x12S\n\x02id\x18\x01 \x01(\x0b\x32\x45.armonik.api.grpc.v1.results.UploadResultDataRequest.ResultIdentifierH\x00\x12\x14\n\ndata_chunk\x18\x02 \x01(\x0cH\x00\x1a\x39\n\x10ResultIdentifier\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x01(\tB\x06\n\x04type\"R\n\x18UploadResultDataResponse\x12\x36\n\x06result\x18\x01 \x01(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\"B\n#ResultsServiceConfigurationResponse\x12\x1b\n\x13\x64\x61ta_chunk_max_size\x18\x01 \x01(\x05\"B\n\x19\x44ownloadResultDataRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x01(\t\"0\n\x1a\x44ownloadResultDataResponse\x12\x12\n\ndata_chunk\x18\x01 \x01(\x0c\"A\n\x18\x44\x65leteResultsDataRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x03(\t\"B\n\x19\x44\x65leteResultsDataResponse\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x03(\tB\x1e\xaa\x02\x1b\x41rmoniK.Api.gRPC.V1.Resultsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'results_common_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'results_common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\033ArmoniK.Api.gRPC.V1.Results'
-  _RESULTRAW._serialized_start=108
-  _RESULTRAW._serialized_end=412
-  _LISTRESULTSREQUEST._serialized_start=415
-  _LISTRESULTSREQUEST._serialized_end=1583
-  _LISTRESULTSREQUEST_FILTER._serialized_start=611
-  _LISTRESULTSREQUEST_FILTER._serialized_end=1085
-  _LISTRESULTSREQUEST_SORT._serialized_start=1088
-  _LISTRESULTSREQUEST_SORT._serialized_end=1254
-  _LISTRESULTSREQUEST_ORDERBYFIELD._serialized_start=1257
-  _LISTRESULTSREQUEST_ORDERBYFIELD._serialized_end=1481
-  _LISTRESULTSREQUEST_ORDERDIRECTION._serialized_start=1483
-  _LISTRESULTSREQUEST_ORDERDIRECTION._serialized_end=1583
-  _LISTRESULTSRESPONSE._serialized_start=1585
-  _LISTRESULTSRESPONSE._serialized_end=1711
-  _GETOWNERTASKIDREQUEST._serialized_start=1713
-  _GETOWNERTASKIDREQUEST._serialized_end=1775
-  _GETOWNERTASKIDRESPONSE._serialized_start=1778
-  _GETOWNERTASKIDRESPONSE._serialized_end=1963
-  _GETOWNERTASKIDRESPONSE_MAPRESULTTASK._serialized_start=1912
-  _GETOWNERTASKIDRESPONSE_MAPRESULTTASK._serialized_end=1963
-  _CREATERESULTSMETADATAREQUEST._serialized_start=1966
-  _CREATERESULTSMETADATAREQUEST._serialized_end=2135
-  _CREATERESULTSMETADATAREQUEST_RESULTCREATE._serialized_start=2107
-  _CREATERESULTSMETADATAREQUEST_RESULTCREATE._serialized_end=2135
-  _CREATERESULTSMETADATARESPONSE._serialized_start=2137
-  _CREATERESULTSMETADATARESPONSE._serialized_end=2225
-  _CREATERESULTSREQUEST._serialized_start=2228
-  _CREATERESULTSREQUEST._serialized_end=2395
-  _CREATERESULTSREQUEST_RESULTCREATE._serialized_start=2353
-  _CREATERESULTSREQUEST_RESULTCREATE._serialized_end=2395
-  _CREATERESULTSRESPONSE._serialized_start=2397
-  _CREATERESULTSRESPONSE._serialized_end=2477
-  _UPLOADRESULTDATAREQUEST._serialized_start=2480
-  _UPLOADRESULTDATAREQUEST._serialized_end=2679
-  _UPLOADRESULTDATAREQUEST_RESULTIDENTIFIER._serialized_start=2614
-  _UPLOADRESULTDATAREQUEST_RESULTIDENTIFIER._serialized_end=2671
-  _UPLOADRESULTDATARESPONSE._serialized_start=2681
-  _UPLOADRESULTDATARESPONSE._serialized_end=2763
-  _RESULTSSERVICECONFIGURATIONRESPONSE._serialized_start=2765
-  _RESULTSSERVICECONFIGURATIONRESPONSE._serialized_end=2831
-  _DOWNLOADRESULTDATAREQUEST._serialized_start=2833
-  _DOWNLOADRESULTDATAREQUEST._serialized_end=2899
-  _DOWNLOADRESULTDATARESPONSE._serialized_start=2901
-  _DOWNLOADRESULTDATARESPONSE._serialized_end=2949
-  _DELETERESULTSDATAREQUEST._serialized_start=2951
-  _DELETERESULTSDATAREQUEST._serialized_end=3016
-  _DELETERESULTSDATARESPONSE._serialized_start=3018
-  _DELETERESULTSDATARESPONSE._serialized_end=3084
+  _globals['_RESULTRAW']._serialized_start=108
+  _globals['_RESULTRAW']._serialized_end=412
+  _globals['_LISTRESULTSREQUEST']._serialized_start=415
+  _globals['_LISTRESULTSREQUEST']._serialized_end=1583
+  _globals['_LISTRESULTSREQUEST_FILTER']._serialized_start=611
+  _globals['_LISTRESULTSREQUEST_FILTER']._serialized_end=1085
+  _globals['_LISTRESULTSREQUEST_SORT']._serialized_start=1088
+  _globals['_LISTRESULTSREQUEST_SORT']._serialized_end=1254
+  _globals['_LISTRESULTSREQUEST_ORDERBYFIELD']._serialized_start=1257
+  _globals['_LISTRESULTSREQUEST_ORDERBYFIELD']._serialized_end=1481
+  _globals['_LISTRESULTSREQUEST_ORDERDIRECTION']._serialized_start=1483
+  _globals['_LISTRESULTSREQUEST_ORDERDIRECTION']._serialized_end=1583
+  _globals['_LISTRESULTSRESPONSE']._serialized_start=1585
+  _globals['_LISTRESULTSRESPONSE']._serialized_end=1711
+  _globals['_GETOWNERTASKIDREQUEST']._serialized_start=1713
+  _globals['_GETOWNERTASKIDREQUEST']._serialized_end=1775
+  _globals['_GETOWNERTASKIDRESPONSE']._serialized_start=1778
+  _globals['_GETOWNERTASKIDRESPONSE']._serialized_end=1963
+  _globals['_GETOWNERTASKIDRESPONSE_MAPRESULTTASK']._serialized_start=1912
+  _globals['_GETOWNERTASKIDRESPONSE_MAPRESULTTASK']._serialized_end=1963
+  _globals['_CREATERESULTSMETADATAREQUEST']._serialized_start=1966
+  _globals['_CREATERESULTSMETADATAREQUEST']._serialized_end=2135
+  _globals['_CREATERESULTSMETADATAREQUEST_RESULTCREATE']._serialized_start=2107
+  _globals['_CREATERESULTSMETADATAREQUEST_RESULTCREATE']._serialized_end=2135
+  _globals['_CREATERESULTSMETADATARESPONSE']._serialized_start=2137
+  _globals['_CREATERESULTSMETADATARESPONSE']._serialized_end=2225
+  _globals['_CREATERESULTSREQUEST']._serialized_start=2228
+  _globals['_CREATERESULTSREQUEST']._serialized_end=2395
+  _globals['_CREATERESULTSREQUEST_RESULTCREATE']._serialized_start=2353
+  _globals['_CREATERESULTSREQUEST_RESULTCREATE']._serialized_end=2395
+  _globals['_CREATERESULTSRESPONSE']._serialized_start=2397
+  _globals['_CREATERESULTSRESPONSE']._serialized_end=2477
+  _globals['_UPLOADRESULTDATAREQUEST']._serialized_start=2480
+  _globals['_UPLOADRESULTDATAREQUEST']._serialized_end=2679
+  _globals['_UPLOADRESULTDATAREQUEST_RESULTIDENTIFIER']._serialized_start=2614
+  _globals['_UPLOADRESULTDATAREQUEST_RESULTIDENTIFIER']._serialized_end=2671
+  _globals['_UPLOADRESULTDATARESPONSE']._serialized_start=2681
+  _globals['_UPLOADRESULTDATARESPONSE']._serialized_end=2763
+  _globals['_RESULTSSERVICECONFIGURATIONRESPONSE']._serialized_start=2765
+  _globals['_RESULTSSERVICECONFIGURATIONRESPONSE']._serialized_end=2831
+  _globals['_DOWNLOADRESULTDATAREQUEST']._serialized_start=2833
+  _globals['_DOWNLOADRESULTDATAREQUEST']._serialized_end=2899
+  _globals['_DOWNLOADRESULTDATARESPONSE']._serialized_start=2901
+  _globals['_DOWNLOADRESULTDATARESPONSE']._serialized_end=2949
+  _globals['_DELETERESULTSDATAREQUEST']._serialized_start=2951
+  _globals['_DELETERESULTSDATAREQUEST']._serialized_end=3016
+  _globals['_DELETERESULTSDATARESPONSE']._serialized_start=3018
+  _globals['_DELETERESULTSDATARESPONSE']._serialized_end=3084
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/results_common_pb2.pyi` & `armonik-3.8.2.dev349/src/armonik/protogen/common/results_common_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,216 +4,226 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class CreateResultsMetaDataRequest(_message.Message):
-    __slots__ = ["results", "session_id"]
-    class ResultCreate(_message.Message):
-        __slots__ = ["name"]
-        NAME_FIELD_NUMBER: _ClassVar[int]
-        name: str
-        def __init__(self, name: _Optional[str] = ...) -> None: ...
-    RESULTS_FIELD_NUMBER: _ClassVar[int]
-    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-    results: _containers.RepeatedCompositeFieldContainer[CreateResultsMetaDataRequest.ResultCreate]
-    session_id: str
-    def __init__(self, results: _Optional[_Iterable[_Union[CreateResultsMetaDataRequest.ResultCreate, _Mapping]]] = ..., session_id: _Optional[str] = ...) -> None: ...
-
-class CreateResultsMetaDataResponse(_message.Message):
-    __slots__ = ["results"]
-    RESULTS_FIELD_NUMBER: _ClassVar[int]
-    results: _containers.RepeatedCompositeFieldContainer[ResultRaw]
-    def __init__(self, results: _Optional[_Iterable[_Union[ResultRaw, _Mapping]]] = ...) -> None: ...
-
-class CreateResultsRequest(_message.Message):
-    __slots__ = ["results", "session_id"]
-    class ResultCreate(_message.Message):
-        __slots__ = ["data", "name"]
-        DATA_FIELD_NUMBER: _ClassVar[int]
-        NAME_FIELD_NUMBER: _ClassVar[int]
-        data: bytes
-        name: str
-        def __init__(self, name: _Optional[str] = ..., data: _Optional[bytes] = ...) -> None: ...
-    RESULTS_FIELD_NUMBER: _ClassVar[int]
-    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-    results: _containers.RepeatedCompositeFieldContainer[CreateResultsRequest.ResultCreate]
-    session_id: str
-    def __init__(self, results: _Optional[_Iterable[_Union[CreateResultsRequest.ResultCreate, _Mapping]]] = ..., session_id: _Optional[str] = ...) -> None: ...
-
-class CreateResultsResponse(_message.Message):
-    __slots__ = ["results"]
-    RESULTS_FIELD_NUMBER: _ClassVar[int]
-    results: _containers.RepeatedCompositeFieldContainer[ResultRaw]
-    def __init__(self, results: _Optional[_Iterable[_Union[ResultRaw, _Mapping]]] = ...) -> None: ...
-
-class DeleteResultsDataRequest(_message.Message):
-    __slots__ = ["result_id", "session_id"]
-    RESULT_ID_FIELD_NUMBER: _ClassVar[int]
+class ResultRaw(_message.Message):
+    __slots__ = ["session_id", "name", "owner_task_id", "status", "created_at", "completed_at", "wait_for_data_at", "result_id"]
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-    result_id: _containers.RepeatedScalarFieldContainer[str]
-    session_id: str
-    def __init__(self, session_id: _Optional[str] = ..., result_id: _Optional[_Iterable[str]] = ...) -> None: ...
-
-class DeleteResultsDataResponse(_message.Message):
-    __slots__ = ["result_id", "session_id"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    OWNER_TASK_ID_FIELD_NUMBER: _ClassVar[int]
+    STATUS_FIELD_NUMBER: _ClassVar[int]
+    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
+    COMPLETED_AT_FIELD_NUMBER: _ClassVar[int]
+    WAIT_FOR_DATA_AT_FIELD_NUMBER: _ClassVar[int]
     RESULT_ID_FIELD_NUMBER: _ClassVar[int]
-    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-    result_id: _containers.RepeatedScalarFieldContainer[str]
     session_id: str
-    def __init__(self, session_id: _Optional[str] = ..., result_id: _Optional[_Iterable[str]] = ...) -> None: ...
-
-class DownloadResultDataRequest(_message.Message):
-    __slots__ = ["result_id", "session_id"]
-    RESULT_ID_FIELD_NUMBER: _ClassVar[int]
-    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+    name: str
+    owner_task_id: str
+    status: _result_status_pb2.ResultStatus
+    created_at: _timestamp_pb2.Timestamp
+    completed_at: _timestamp_pb2.Timestamp
+    wait_for_data_at: _timestamp_pb2.Timestamp
     result_id: str
-    session_id: str
-    def __init__(self, session_id: _Optional[str] = ..., result_id: _Optional[str] = ...) -> None: ...
-
-class DownloadResultDataResponse(_message.Message):
-    __slots__ = ["data_chunk"]
-    DATA_CHUNK_FIELD_NUMBER: _ClassVar[int]
-    data_chunk: bytes
-    def __init__(self, data_chunk: _Optional[bytes] = ...) -> None: ...
-
-class GetOwnerTaskIdRequest(_message.Message):
-    __slots__ = ["result_id", "session_id"]
-    RESULT_ID_FIELD_NUMBER: _ClassVar[int]
-    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-    result_id: _containers.RepeatedScalarFieldContainer[str]
-    session_id: str
-    def __init__(self, session_id: _Optional[str] = ..., result_id: _Optional[_Iterable[str]] = ...) -> None: ...
-
-class GetOwnerTaskIdResponse(_message.Message):
-    __slots__ = ["result_task", "session_id"]
-    class MapResultTask(_message.Message):
-        __slots__ = ["result_id", "task_id"]
-        RESULT_ID_FIELD_NUMBER: _ClassVar[int]
-        TASK_ID_FIELD_NUMBER: _ClassVar[int]
-        result_id: str
-        task_id: str
-        def __init__(self, result_id: _Optional[str] = ..., task_id: _Optional[str] = ...) -> None: ...
-    RESULT_TASK_FIELD_NUMBER: _ClassVar[int]
-    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-    result_task: _containers.RepeatedCompositeFieldContainer[GetOwnerTaskIdResponse.MapResultTask]
-    session_id: str
-    def __init__(self, result_task: _Optional[_Iterable[_Union[GetOwnerTaskIdResponse.MapResultTask, _Mapping]]] = ..., session_id: _Optional[str] = ...) -> None: ...
+    def __init__(self, session_id: _Optional[str] = ..., name: _Optional[str] = ..., owner_task_id: _Optional[str] = ..., status: _Optional[_Union[_result_status_pb2.ResultStatus, str]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., completed_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., wait_for_data_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., result_id: _Optional[str] = ...) -> None: ...
 
 class ListResultsRequest(_message.Message):
-    __slots__ = ["filter", "page", "page_size", "sort"]
+    __slots__ = ["page", "page_size", "filter", "sort"]
     class OrderByField(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        ORDER_BY_FIELD_UNSPECIFIED: _ClassVar[ListResultsRequest.OrderByField]
+        ORDER_BY_FIELD_SESSION_ID: _ClassVar[ListResultsRequest.OrderByField]
+        ORDER_BY_FIELD_NAME: _ClassVar[ListResultsRequest.OrderByField]
+        ORDER_BY_FIELD_OWNER_TASK_ID: _ClassVar[ListResultsRequest.OrderByField]
+        ORDER_BY_FIELD_STATUS: _ClassVar[ListResultsRequest.OrderByField]
+        ORDER_BY_FIELD_CREATED_AT: _ClassVar[ListResultsRequest.OrderByField]
+        ORDER_BY_FIELD_RESULT_ID: _ClassVar[ListResultsRequest.OrderByField]
+    ORDER_BY_FIELD_UNSPECIFIED: ListResultsRequest.OrderByField
+    ORDER_BY_FIELD_SESSION_ID: ListResultsRequest.OrderByField
+    ORDER_BY_FIELD_NAME: ListResultsRequest.OrderByField
+    ORDER_BY_FIELD_OWNER_TASK_ID: ListResultsRequest.OrderByField
+    ORDER_BY_FIELD_STATUS: ListResultsRequest.OrderByField
+    ORDER_BY_FIELD_CREATED_AT: ListResultsRequest.OrderByField
+    ORDER_BY_FIELD_RESULT_ID: ListResultsRequest.OrderByField
     class OrderDirection(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        ORDER_DIRECTION_UNSPECIFIED: _ClassVar[ListResultsRequest.OrderDirection]
+        ORDER_DIRECTION_ASC: _ClassVar[ListResultsRequest.OrderDirection]
+        ORDER_DIRECTION_DESC: _ClassVar[ListResultsRequest.OrderDirection]
+    ORDER_DIRECTION_UNSPECIFIED: ListResultsRequest.OrderDirection
+    ORDER_DIRECTION_ASC: ListResultsRequest.OrderDirection
+    ORDER_DIRECTION_DESC: ListResultsRequest.OrderDirection
     class Filter(_message.Message):
-        __slots__ = ["completed_after", "completed_before", "created_after", "created_before", "name", "owner_task_id", "result_id", "session_id", "status", "wait_for_data_after", "wait_for_data_before"]
-        COMPLETED_AFTER_FIELD_NUMBER: _ClassVar[int]
-        COMPLETED_BEFORE_FIELD_NUMBER: _ClassVar[int]
-        CREATED_AFTER_FIELD_NUMBER: _ClassVar[int]
-        CREATED_BEFORE_FIELD_NUMBER: _ClassVar[int]
+        __slots__ = ["session_id", "name", "owner_task_id", "status", "created_after", "created_before", "completed_after", "completed_before", "wait_for_data_after", "wait_for_data_before", "result_id"]
+        SESSION_ID_FIELD_NUMBER: _ClassVar[int]
         NAME_FIELD_NUMBER: _ClassVar[int]
         OWNER_TASK_ID_FIELD_NUMBER: _ClassVar[int]
-        RESULT_ID_FIELD_NUMBER: _ClassVar[int]
-        SESSION_ID_FIELD_NUMBER: _ClassVar[int]
         STATUS_FIELD_NUMBER: _ClassVar[int]
+        CREATED_AFTER_FIELD_NUMBER: _ClassVar[int]
+        CREATED_BEFORE_FIELD_NUMBER: _ClassVar[int]
+        COMPLETED_AFTER_FIELD_NUMBER: _ClassVar[int]
+        COMPLETED_BEFORE_FIELD_NUMBER: _ClassVar[int]
         WAIT_FOR_DATA_AFTER_FIELD_NUMBER: _ClassVar[int]
         WAIT_FOR_DATA_BEFORE_FIELD_NUMBER: _ClassVar[int]
-        completed_after: _timestamp_pb2.Timestamp
-        completed_before: _timestamp_pb2.Timestamp
-        created_after: _timestamp_pb2.Timestamp
-        created_before: _timestamp_pb2.Timestamp
+        RESULT_ID_FIELD_NUMBER: _ClassVar[int]
+        session_id: str
         name: str
         owner_task_id: str
-        result_id: str
-        session_id: str
         status: _result_status_pb2.ResultStatus
+        created_after: _timestamp_pb2.Timestamp
+        created_before: _timestamp_pb2.Timestamp
+        completed_after: _timestamp_pb2.Timestamp
+        completed_before: _timestamp_pb2.Timestamp
         wait_for_data_after: _timestamp_pb2.Timestamp
         wait_for_data_before: _timestamp_pb2.Timestamp
+        result_id: str
         def __init__(self, session_id: _Optional[str] = ..., name: _Optional[str] = ..., owner_task_id: _Optional[str] = ..., status: _Optional[_Union[_result_status_pb2.ResultStatus, str]] = ..., created_after: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., created_before: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., completed_after: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., completed_before: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., wait_for_data_after: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., wait_for_data_before: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., result_id: _Optional[str] = ...) -> None: ...
     class Sort(_message.Message):
-        __slots__ = ["direction", "field"]
-        DIRECTION_FIELD_NUMBER: _ClassVar[int]
+        __slots__ = ["field", "direction"]
         FIELD_FIELD_NUMBER: _ClassVar[int]
-        direction: ListResultsRequest.OrderDirection
+        DIRECTION_FIELD_NUMBER: _ClassVar[int]
         field: ListResultsRequest.OrderByField
+        direction: ListResultsRequest.OrderDirection
         def __init__(self, field: _Optional[_Union[ListResultsRequest.OrderByField, str]] = ..., direction: _Optional[_Union[ListResultsRequest.OrderDirection, str]] = ...) -> None: ...
-    FILTER_FIELD_NUMBER: _ClassVar[int]
-    ORDER_BY_FIELD_CREATED_AT: ListResultsRequest.OrderByField
-    ORDER_BY_FIELD_NAME: ListResultsRequest.OrderByField
-    ORDER_BY_FIELD_OWNER_TASK_ID: ListResultsRequest.OrderByField
-    ORDER_BY_FIELD_RESULT_ID: ListResultsRequest.OrderByField
-    ORDER_BY_FIELD_SESSION_ID: ListResultsRequest.OrderByField
-    ORDER_BY_FIELD_STATUS: ListResultsRequest.OrderByField
-    ORDER_BY_FIELD_UNSPECIFIED: ListResultsRequest.OrderByField
-    ORDER_DIRECTION_ASC: ListResultsRequest.OrderDirection
-    ORDER_DIRECTION_DESC: ListResultsRequest.OrderDirection
-    ORDER_DIRECTION_UNSPECIFIED: ListResultsRequest.OrderDirection
     PAGE_FIELD_NUMBER: _ClassVar[int]
     PAGE_SIZE_FIELD_NUMBER: _ClassVar[int]
+    FILTER_FIELD_NUMBER: _ClassVar[int]
     SORT_FIELD_NUMBER: _ClassVar[int]
-    filter: ListResultsRequest.Filter
     page: int
     page_size: int
+    filter: ListResultsRequest.Filter
     sort: ListResultsRequest.Sort
     def __init__(self, page: _Optional[int] = ..., page_size: _Optional[int] = ..., filter: _Optional[_Union[ListResultsRequest.Filter, _Mapping]] = ..., sort: _Optional[_Union[ListResultsRequest.Sort, _Mapping]] = ...) -> None: ...
 
 class ListResultsResponse(_message.Message):
-    __slots__ = ["page", "page_size", "results", "total"]
+    __slots__ = ["results", "page", "page_size", "total"]
+    RESULTS_FIELD_NUMBER: _ClassVar[int]
     PAGE_FIELD_NUMBER: _ClassVar[int]
     PAGE_SIZE_FIELD_NUMBER: _ClassVar[int]
-    RESULTS_FIELD_NUMBER: _ClassVar[int]
     TOTAL_FIELD_NUMBER: _ClassVar[int]
+    results: _containers.RepeatedCompositeFieldContainer[ResultRaw]
     page: int
     page_size: int
-    results: _containers.RepeatedCompositeFieldContainer[ResultRaw]
     total: int
     def __init__(self, results: _Optional[_Iterable[_Union[ResultRaw, _Mapping]]] = ..., page: _Optional[int] = ..., page_size: _Optional[int] = ..., total: _Optional[int] = ...) -> None: ...
 
-class ResultRaw(_message.Message):
-    __slots__ = ["completed_at", "created_at", "name", "owner_task_id", "result_id", "session_id", "status", "wait_for_data_at"]
-    COMPLETED_AT_FIELD_NUMBER: _ClassVar[int]
-    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    OWNER_TASK_ID_FIELD_NUMBER: _ClassVar[int]
+class GetOwnerTaskIdRequest(_message.Message):
+    __slots__ = ["session_id", "result_id"]
+    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
     RESULT_ID_FIELD_NUMBER: _ClassVar[int]
+    session_id: str
+    result_id: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, session_id: _Optional[str] = ..., result_id: _Optional[_Iterable[str]] = ...) -> None: ...
+
+class GetOwnerTaskIdResponse(_message.Message):
+    __slots__ = ["result_task", "session_id"]
+    class MapResultTask(_message.Message):
+        __slots__ = ["result_id", "task_id"]
+        RESULT_ID_FIELD_NUMBER: _ClassVar[int]
+        TASK_ID_FIELD_NUMBER: _ClassVar[int]
+        result_id: str
+        task_id: str
+        def __init__(self, result_id: _Optional[str] = ..., task_id: _Optional[str] = ...) -> None: ...
+    RESULT_TASK_FIELD_NUMBER: _ClassVar[int]
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-    STATUS_FIELD_NUMBER: _ClassVar[int]
-    WAIT_FOR_DATA_AT_FIELD_NUMBER: _ClassVar[int]
-    completed_at: _timestamp_pb2.Timestamp
-    created_at: _timestamp_pb2.Timestamp
-    name: str
-    owner_task_id: str
-    result_id: str
+    result_task: _containers.RepeatedCompositeFieldContainer[GetOwnerTaskIdResponse.MapResultTask]
     session_id: str
-    status: _result_status_pb2.ResultStatus
-    wait_for_data_at: _timestamp_pb2.Timestamp
-    def __init__(self, session_id: _Optional[str] = ..., name: _Optional[str] = ..., owner_task_id: _Optional[str] = ..., status: _Optional[_Union[_result_status_pb2.ResultStatus, str]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., completed_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., wait_for_data_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., result_id: _Optional[str] = ...) -> None: ...
+    def __init__(self, result_task: _Optional[_Iterable[_Union[GetOwnerTaskIdResponse.MapResultTask, _Mapping]]] = ..., session_id: _Optional[str] = ...) -> None: ...
 
-class ResultsServiceConfigurationResponse(_message.Message):
-    __slots__ = ["data_chunk_max_size"]
-    DATA_CHUNK_MAX_SIZE_FIELD_NUMBER: _ClassVar[int]
-    data_chunk_max_size: int
-    def __init__(self, data_chunk_max_size: _Optional[int] = ...) -> None: ...
+class CreateResultsMetaDataRequest(_message.Message):
+    __slots__ = ["results", "session_id"]
+    class ResultCreate(_message.Message):
+        __slots__ = ["name"]
+        NAME_FIELD_NUMBER: _ClassVar[int]
+        name: str
+        def __init__(self, name: _Optional[str] = ...) -> None: ...
+    RESULTS_FIELD_NUMBER: _ClassVar[int]
+    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+    results: _containers.RepeatedCompositeFieldContainer[CreateResultsMetaDataRequest.ResultCreate]
+    session_id: str
+    def __init__(self, results: _Optional[_Iterable[_Union[CreateResultsMetaDataRequest.ResultCreate, _Mapping]]] = ..., session_id: _Optional[str] = ...) -> None: ...
+
+class CreateResultsMetaDataResponse(_message.Message):
+    __slots__ = ["results"]
+    RESULTS_FIELD_NUMBER: _ClassVar[int]
+    results: _containers.RepeatedCompositeFieldContainer[ResultRaw]
+    def __init__(self, results: _Optional[_Iterable[_Union[ResultRaw, _Mapping]]] = ...) -> None: ...
+
+class CreateResultsRequest(_message.Message):
+    __slots__ = ["results", "session_id"]
+    class ResultCreate(_message.Message):
+        __slots__ = ["name", "data"]
+        NAME_FIELD_NUMBER: _ClassVar[int]
+        DATA_FIELD_NUMBER: _ClassVar[int]
+        name: str
+        data: bytes
+        def __init__(self, name: _Optional[str] = ..., data: _Optional[bytes] = ...) -> None: ...
+    RESULTS_FIELD_NUMBER: _ClassVar[int]
+    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+    results: _containers.RepeatedCompositeFieldContainer[CreateResultsRequest.ResultCreate]
+    session_id: str
+    def __init__(self, results: _Optional[_Iterable[_Union[CreateResultsRequest.ResultCreate, _Mapping]]] = ..., session_id: _Optional[str] = ...) -> None: ...
+
+class CreateResultsResponse(_message.Message):
+    __slots__ = ["results"]
+    RESULTS_FIELD_NUMBER: _ClassVar[int]
+    results: _containers.RepeatedCompositeFieldContainer[ResultRaw]
+    def __init__(self, results: _Optional[_Iterable[_Union[ResultRaw, _Mapping]]] = ...) -> None: ...
 
 class UploadResultDataRequest(_message.Message):
-    __slots__ = ["data_chunk", "id"]
+    __slots__ = ["id", "data_chunk"]
     class ResultIdentifier(_message.Message):
-        __slots__ = ["result_id", "session_id"]
-        RESULT_ID_FIELD_NUMBER: _ClassVar[int]
+        __slots__ = ["session_id", "result_id"]
         SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-        result_id: str
+        RESULT_ID_FIELD_NUMBER: _ClassVar[int]
         session_id: str
+        result_id: str
         def __init__(self, session_id: _Optional[str] = ..., result_id: _Optional[str] = ...) -> None: ...
-    DATA_CHUNK_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
-    data_chunk: bytes
+    DATA_CHUNK_FIELD_NUMBER: _ClassVar[int]
     id: UploadResultDataRequest.ResultIdentifier
+    data_chunk: bytes
     def __init__(self, id: _Optional[_Union[UploadResultDataRequest.ResultIdentifier, _Mapping]] = ..., data_chunk: _Optional[bytes] = ...) -> None: ...
 
 class UploadResultDataResponse(_message.Message):
     __slots__ = ["result"]
     RESULT_FIELD_NUMBER: _ClassVar[int]
     result: ResultRaw
     def __init__(self, result: _Optional[_Union[ResultRaw, _Mapping]] = ...) -> None: ...
+
+class ResultsServiceConfigurationResponse(_message.Message):
+    __slots__ = ["data_chunk_max_size"]
+    DATA_CHUNK_MAX_SIZE_FIELD_NUMBER: _ClassVar[int]
+    data_chunk_max_size: int
+    def __init__(self, data_chunk_max_size: _Optional[int] = ...) -> None: ...
+
+class DownloadResultDataRequest(_message.Message):
+    __slots__ = ["session_id", "result_id"]
+    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+    RESULT_ID_FIELD_NUMBER: _ClassVar[int]
+    session_id: str
+    result_id: str
+    def __init__(self, session_id: _Optional[str] = ..., result_id: _Optional[str] = ...) -> None: ...
+
+class DownloadResultDataResponse(_message.Message):
+    __slots__ = ["data_chunk"]
+    DATA_CHUNK_FIELD_NUMBER: _ClassVar[int]
+    data_chunk: bytes
+    def __init__(self, data_chunk: _Optional[bytes] = ...) -> None: ...
+
+class DeleteResultsDataRequest(_message.Message):
+    __slots__ = ["session_id", "result_id"]
+    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+    RESULT_ID_FIELD_NUMBER: _ClassVar[int]
+    session_id: str
+    result_id: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, session_id: _Optional[str] = ..., result_id: _Optional[_Iterable[str]] = ...) -> None: ...
+
+class DeleteResultsDataResponse(_message.Message):
+    __slots__ = ["session_id", "result_id"]
+    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+    RESULT_ID_FIELD_NUMBER: _ClassVar[int]
+    session_id: str
+    result_id: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, session_id: _Optional[str] = ..., result_id: _Optional[_Iterable[str]] = ...) -> None: ...
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/session_status_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/common/session_status_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: session_status.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14session_status.proto\x12\"armonik.api.grpc.v1.session_status*i\n\rSessionStatus\x12\x1e\n\x1aSESSION_STATUS_UNSPECIFIED\x10\x00\x12\x1a\n\x16SESSION_STATUS_RUNNING\x10\x01\x12\x1c\n\x18SESSION_STATUS_CANCELLED\x10\x02\x42\x16\xaa\x02\x13\x41rmoniK.Api.gRPC.V1b\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'session_status_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'session_status_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\023ArmoniK.Api.gRPC.V1'
-  _SESSIONSTATUS._serialized_start=60
-  _SESSIONSTATUS._serialized_end=165
+  _globals['_SESSIONSTATUS']._serialized_start=60
+  _globals['_SESSIONSTATUS']._serialized_end=165
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/sessions_common_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/common/sessions_common_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: sessions_common.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from . import objects_pb2 as objects__pb2
 from . import session_status_pb2 as session__status__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15sessions_common.proto\x12\x1c\x61rmonik.api.grpc.v1.sessions\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\robjects.proto\x1a\x14session_status.proto\"\xbc\x02\n\nSessionRaw\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x41\n\x06status\x18\x02 \x01(\x0e\x32\x31.armonik.api.grpc.v1.session_status.SessionStatus\x12\x15\n\rpartition_ids\x18\x03 \x03(\t\x12\x31\n\x07options\x18\x04 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63\x61ncelled_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x08\x64uration\x18\x07 \x01(\x0b\x32\x19.google.protobuf.Duration\"\xa9\x02\n\x0eSessionSummary\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x41\n\x06status\x18\x02 \x01(\x0e\x32\x31.armonik.api.grpc.v1.session_status.SessionStatus\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63\x61ncelled_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x08\x64uration\x18\x07 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x31\n\x07options\x18\x05 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\"\x8a\x08\n\x13ListSessionsRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12H\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x38.armonik.api.grpc.v1.sessions.ListSessionsRequest.Filter\x12\x44\n\x04sort\x18\x04 \x01(\x0b\x32\x36.armonik.api.grpc.v1.sessions.ListSessionsRequest.Sort\x12\x19\n\x11with_task_options\x18\x05 \x01(\x08\x1a\xe8\x02\n\x06\x46ilter\x12\x18\n\x10\x61pplication_name\x18\x01 \x01(\t\x12\x1b\n\x13\x61pplication_version\x18\x02 \x01(\t\x12\x12\n\nsession_id\x18\x03 \x01(\t\x12\x31\n\rcreated_after\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0e\x63reated_before\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0f\x63\x61ncelled_after\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x63\x61ncelled_before\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x41\n\x06status\x18\x08 \x01(\x0e\x32\x31.armonik.api.grpc.v1.session_status.SessionStatus\x1a\xaa\x01\n\x04Sort\x12M\n\x05\x66ield\x18\x01 \x01(\x0e\x32>.armonik.api.grpc.v1.sessions.ListSessionsRequest.OrderByField\x12S\n\tdirection\x18\x02 \x01(\x0e\x32@.armonik.api.grpc.v1.sessions.ListSessionsRequest.OrderDirection\"\xa8\x01\n\x0cOrderByField\x12\x1e\n\x1aORDER_BY_FIELD_UNSPECIFIED\x10\x00\x12\x1d\n\x19ORDER_BY_FIELD_SESSION_ID\x10\x01\x12\x19\n\x15ORDER_BY_FIELD_STATUS\x10\x02\x12\x1d\n\x19ORDER_BY_FIELD_CREATED_AT\x10\x03\x12\x1f\n\x1bORDER_BY_FIELD_CANCELLED_AT\x10\x04\"d\n\x0eOrderDirection\x12\x1f\n\x1bORDER_DIRECTION_UNSPECIFIED\x10\x00\x12\x17\n\x13ORDER_DIRECTION_ASC\x10\x01\x12\x18\n\x14ORDER_DIRECTION_DESC\x10\x02\"\x86\x01\n\x14ListSessionsResponse\x12>\n\x08sessions\x18\x01 \x03(\x0b\x32,.armonik.api.grpc.v1.sessions.SessionSummary\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"\'\n\x11GetSessionRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"O\n\x12GetSessionResponse\x12\x39\n\x07session\x18\x01 \x01(\x0b\x32(.armonik.api.grpc.v1.sessions.SessionRaw\"*\n\x14\x43\x61ncelSessionRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"R\n\x15\x43\x61ncelSessionResponse\x12\x39\n\x07session\x18\x01 \x01(\x0b\x32(.armonik.api.grpc.v1.sessions.SessionRaw\"/\n\x19\x43ountTasksByStatusRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"N\n\x1a\x43ountTasksByStatusResponse\x12\x30\n\x06status\x18\x01 \x03(\x0b\x32 .armonik.api.grpc.v1.StatusCountB\x1f\xaa\x02\x1c\x41rmoniK.Api.gRPC.V1.Sessionsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sessions_common_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sessions_common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\034ArmoniK.Api.gRPC.V1.Sessions'
-  _SESSIONRAW._serialized_start=158
-  _SESSIONRAW._serialized_end=474
-  _SESSIONSUMMARY._serialized_start=477
-  _SESSIONSUMMARY._serialized_end=774
-  _LISTSESSIONSREQUEST._serialized_start=777
-  _LISTSESSIONSREQUEST._serialized_end=1811
-  _LISTSESSIONSREQUEST_FILTER._serialized_start=1005
-  _LISTSESSIONSREQUEST_FILTER._serialized_end=1365
-  _LISTSESSIONSREQUEST_SORT._serialized_start=1368
-  _LISTSESSIONSREQUEST_SORT._serialized_end=1538
-  _LISTSESSIONSREQUEST_ORDERBYFIELD._serialized_start=1541
-  _LISTSESSIONSREQUEST_ORDERBYFIELD._serialized_end=1709
-  _LISTSESSIONSREQUEST_ORDERDIRECTION._serialized_start=1711
-  _LISTSESSIONSREQUEST_ORDERDIRECTION._serialized_end=1811
-  _LISTSESSIONSRESPONSE._serialized_start=1814
-  _LISTSESSIONSRESPONSE._serialized_end=1948
-  _GETSESSIONREQUEST._serialized_start=1950
-  _GETSESSIONREQUEST._serialized_end=1989
-  _GETSESSIONRESPONSE._serialized_start=1991
-  _GETSESSIONRESPONSE._serialized_end=2070
-  _CANCELSESSIONREQUEST._serialized_start=2072
-  _CANCELSESSIONREQUEST._serialized_end=2114
-  _CANCELSESSIONRESPONSE._serialized_start=2116
-  _CANCELSESSIONRESPONSE._serialized_end=2198
-  _COUNTTASKSBYSTATUSREQUEST._serialized_start=2200
-  _COUNTTASKSBYSTATUSREQUEST._serialized_end=2247
-  _COUNTTASKSBYSTATUSRESPONSE._serialized_start=2249
-  _COUNTTASKSBYSTATUSRESPONSE._serialized_end=2327
+  _globals['_SESSIONRAW']._serialized_start=158
+  _globals['_SESSIONRAW']._serialized_end=474
+  _globals['_SESSIONSUMMARY']._serialized_start=477
+  _globals['_SESSIONSUMMARY']._serialized_end=774
+  _globals['_LISTSESSIONSREQUEST']._serialized_start=777
+  _globals['_LISTSESSIONSREQUEST']._serialized_end=1811
+  _globals['_LISTSESSIONSREQUEST_FILTER']._serialized_start=1005
+  _globals['_LISTSESSIONSREQUEST_FILTER']._serialized_end=1365
+  _globals['_LISTSESSIONSREQUEST_SORT']._serialized_start=1368
+  _globals['_LISTSESSIONSREQUEST_SORT']._serialized_end=1538
+  _globals['_LISTSESSIONSREQUEST_ORDERBYFIELD']._serialized_start=1541
+  _globals['_LISTSESSIONSREQUEST_ORDERBYFIELD']._serialized_end=1709
+  _globals['_LISTSESSIONSREQUEST_ORDERDIRECTION']._serialized_start=1711
+  _globals['_LISTSESSIONSREQUEST_ORDERDIRECTION']._serialized_end=1811
+  _globals['_LISTSESSIONSRESPONSE']._serialized_start=1814
+  _globals['_LISTSESSIONSRESPONSE']._serialized_end=1948
+  _globals['_GETSESSIONREQUEST']._serialized_start=1950
+  _globals['_GETSESSIONREQUEST']._serialized_end=1989
+  _globals['_GETSESSIONRESPONSE']._serialized_start=1991
+  _globals['_GETSESSIONRESPONSE']._serialized_end=2070
+  _globals['_CANCELSESSIONREQUEST']._serialized_start=2072
+  _globals['_CANCELSESSIONREQUEST']._serialized_end=2114
+  _globals['_CANCELSESSIONRESPONSE']._serialized_start=2116
+  _globals['_CANCELSESSIONRESPONSE']._serialized_end=2198
+  _globals['_COUNTTASKSBYSTATUSREQUEST']._serialized_start=2200
+  _globals['_COUNTTASKSBYSTATUSREQUEST']._serialized_end=2247
+  _globals['_COUNTTASKSBYSTATUSRESPONSE']._serialized_start=2249
+  _globals['_COUNTTASKSBYSTATUSRESPONSE']._serialized_end=2327
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/sessions_common_pb2.pyi` & `armonik-3.8.2.dev349/src/armonik/protogen/common/sessions_common_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -6,140 +6,148 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class CancelSessionRequest(_message.Message):
-    __slots__ = ["session_id"]
+class SessionRaw(_message.Message):
+    __slots__ = ["session_id", "status", "partition_ids", "options", "created_at", "cancelled_at", "duration"]
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+    STATUS_FIELD_NUMBER: _ClassVar[int]
+    PARTITION_IDS_FIELD_NUMBER: _ClassVar[int]
+    OPTIONS_FIELD_NUMBER: _ClassVar[int]
+    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
+    CANCELLED_AT_FIELD_NUMBER: _ClassVar[int]
+    DURATION_FIELD_NUMBER: _ClassVar[int]
     session_id: str
-    def __init__(self, session_id: _Optional[str] = ...) -> None: ...
-
-class CancelSessionResponse(_message.Message):
-    __slots__ = ["session"]
-    SESSION_FIELD_NUMBER: _ClassVar[int]
-    session: SessionRaw
-    def __init__(self, session: _Optional[_Union[SessionRaw, _Mapping]] = ...) -> None: ...
+    status: _session_status_pb2.SessionStatus
+    partition_ids: _containers.RepeatedScalarFieldContainer[str]
+    options: _objects_pb2.TaskOptions
+    created_at: _timestamp_pb2.Timestamp
+    cancelled_at: _timestamp_pb2.Timestamp
+    duration: _duration_pb2.Duration
+    def __init__(self, session_id: _Optional[str] = ..., status: _Optional[_Union[_session_status_pb2.SessionStatus, str]] = ..., partition_ids: _Optional[_Iterable[str]] = ..., options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., cancelled_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ...) -> None: ...
 
-class CountTasksByStatusRequest(_message.Message):
-    __slots__ = ["session_id"]
+class SessionSummary(_message.Message):
+    __slots__ = ["session_id", "status", "created_at", "cancelled_at", "duration", "options"]
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-    session_id: str
-    def __init__(self, session_id: _Optional[str] = ...) -> None: ...
-
-class CountTasksByStatusResponse(_message.Message):
-    __slots__ = ["status"]
     STATUS_FIELD_NUMBER: _ClassVar[int]
-    status: _containers.RepeatedCompositeFieldContainer[_objects_pb2.StatusCount]
-    def __init__(self, status: _Optional[_Iterable[_Union[_objects_pb2.StatusCount, _Mapping]]] = ...) -> None: ...
-
-class GetSessionRequest(_message.Message):
-    __slots__ = ["session_id"]
-    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
+    CANCELLED_AT_FIELD_NUMBER: _ClassVar[int]
+    DURATION_FIELD_NUMBER: _ClassVar[int]
+    OPTIONS_FIELD_NUMBER: _ClassVar[int]
     session_id: str
-    def __init__(self, session_id: _Optional[str] = ...) -> None: ...
-
-class GetSessionResponse(_message.Message):
-    __slots__ = ["session"]
-    SESSION_FIELD_NUMBER: _ClassVar[int]
-    session: SessionRaw
-    def __init__(self, session: _Optional[_Union[SessionRaw, _Mapping]] = ...) -> None: ...
+    status: _session_status_pb2.SessionStatus
+    created_at: _timestamp_pb2.Timestamp
+    cancelled_at: _timestamp_pb2.Timestamp
+    duration: _duration_pb2.Duration
+    options: _objects_pb2.TaskOptions
+    def __init__(self, session_id: _Optional[str] = ..., status: _Optional[_Union[_session_status_pb2.SessionStatus, str]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., cancelled_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ...) -> None: ...
 
 class ListSessionsRequest(_message.Message):
-    __slots__ = ["filter", "page", "page_size", "sort", "with_task_options"]
+    __slots__ = ["page", "page_size", "filter", "sort", "with_task_options"]
     class OrderByField(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        ORDER_BY_FIELD_UNSPECIFIED: _ClassVar[ListSessionsRequest.OrderByField]
+        ORDER_BY_FIELD_SESSION_ID: _ClassVar[ListSessionsRequest.OrderByField]
+        ORDER_BY_FIELD_STATUS: _ClassVar[ListSessionsRequest.OrderByField]
+        ORDER_BY_FIELD_CREATED_AT: _ClassVar[ListSessionsRequest.OrderByField]
+        ORDER_BY_FIELD_CANCELLED_AT: _ClassVar[ListSessionsRequest.OrderByField]
+    ORDER_BY_FIELD_UNSPECIFIED: ListSessionsRequest.OrderByField
+    ORDER_BY_FIELD_SESSION_ID: ListSessionsRequest.OrderByField
+    ORDER_BY_FIELD_STATUS: ListSessionsRequest.OrderByField
+    ORDER_BY_FIELD_CREATED_AT: ListSessionsRequest.OrderByField
+    ORDER_BY_FIELD_CANCELLED_AT: ListSessionsRequest.OrderByField
     class OrderDirection(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        ORDER_DIRECTION_UNSPECIFIED: _ClassVar[ListSessionsRequest.OrderDirection]
+        ORDER_DIRECTION_ASC: _ClassVar[ListSessionsRequest.OrderDirection]
+        ORDER_DIRECTION_DESC: _ClassVar[ListSessionsRequest.OrderDirection]
+    ORDER_DIRECTION_UNSPECIFIED: ListSessionsRequest.OrderDirection
+    ORDER_DIRECTION_ASC: ListSessionsRequest.OrderDirection
+    ORDER_DIRECTION_DESC: ListSessionsRequest.OrderDirection
     class Filter(_message.Message):
-        __slots__ = ["application_name", "application_version", "cancelled_after", "cancelled_before", "created_after", "created_before", "session_id", "status"]
+        __slots__ = ["application_name", "application_version", "session_id", "created_after", "created_before", "cancelled_after", "cancelled_before", "status"]
         APPLICATION_NAME_FIELD_NUMBER: _ClassVar[int]
         APPLICATION_VERSION_FIELD_NUMBER: _ClassVar[int]
-        CANCELLED_AFTER_FIELD_NUMBER: _ClassVar[int]
-        CANCELLED_BEFORE_FIELD_NUMBER: _ClassVar[int]
+        SESSION_ID_FIELD_NUMBER: _ClassVar[int]
         CREATED_AFTER_FIELD_NUMBER: _ClassVar[int]
         CREATED_BEFORE_FIELD_NUMBER: _ClassVar[int]
-        SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+        CANCELLED_AFTER_FIELD_NUMBER: _ClassVar[int]
+        CANCELLED_BEFORE_FIELD_NUMBER: _ClassVar[int]
         STATUS_FIELD_NUMBER: _ClassVar[int]
         application_name: str
         application_version: str
-        cancelled_after: _timestamp_pb2.Timestamp
-        cancelled_before: _timestamp_pb2.Timestamp
+        session_id: str
         created_after: _timestamp_pb2.Timestamp
         created_before: _timestamp_pb2.Timestamp
-        session_id: str
+        cancelled_after: _timestamp_pb2.Timestamp
+        cancelled_before: _timestamp_pb2.Timestamp
         status: _session_status_pb2.SessionStatus
         def __init__(self, application_name: _Optional[str] = ..., application_version: _Optional[str] = ..., session_id: _Optional[str] = ..., created_after: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., created_before: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., cancelled_after: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., cancelled_before: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., status: _Optional[_Union[_session_status_pb2.SessionStatus, str]] = ...) -> None: ...
     class Sort(_message.Message):
-        __slots__ = ["direction", "field"]
-        DIRECTION_FIELD_NUMBER: _ClassVar[int]
+        __slots__ = ["field", "direction"]
         FIELD_FIELD_NUMBER: _ClassVar[int]
-        direction: ListSessionsRequest.OrderDirection
+        DIRECTION_FIELD_NUMBER: _ClassVar[int]
         field: ListSessionsRequest.OrderByField
+        direction: ListSessionsRequest.OrderDirection
         def __init__(self, field: _Optional[_Union[ListSessionsRequest.OrderByField, str]] = ..., direction: _Optional[_Union[ListSessionsRequest.OrderDirection, str]] = ...) -> None: ...
-    FILTER_FIELD_NUMBER: _ClassVar[int]
-    ORDER_BY_FIELD_CANCELLED_AT: ListSessionsRequest.OrderByField
-    ORDER_BY_FIELD_CREATED_AT: ListSessionsRequest.OrderByField
-    ORDER_BY_FIELD_SESSION_ID: ListSessionsRequest.OrderByField
-    ORDER_BY_FIELD_STATUS: ListSessionsRequest.OrderByField
-    ORDER_BY_FIELD_UNSPECIFIED: ListSessionsRequest.OrderByField
-    ORDER_DIRECTION_ASC: ListSessionsRequest.OrderDirection
-    ORDER_DIRECTION_DESC: ListSessionsRequest.OrderDirection
-    ORDER_DIRECTION_UNSPECIFIED: ListSessionsRequest.OrderDirection
     PAGE_FIELD_NUMBER: _ClassVar[int]
     PAGE_SIZE_FIELD_NUMBER: _ClassVar[int]
+    FILTER_FIELD_NUMBER: _ClassVar[int]
     SORT_FIELD_NUMBER: _ClassVar[int]
     WITH_TASK_OPTIONS_FIELD_NUMBER: _ClassVar[int]
-    filter: ListSessionsRequest.Filter
     page: int
     page_size: int
+    filter: ListSessionsRequest.Filter
     sort: ListSessionsRequest.Sort
     with_task_options: bool
     def __init__(self, page: _Optional[int] = ..., page_size: _Optional[int] = ..., filter: _Optional[_Union[ListSessionsRequest.Filter, _Mapping]] = ..., sort: _Optional[_Union[ListSessionsRequest.Sort, _Mapping]] = ..., with_task_options: bool = ...) -> None: ...
 
 class ListSessionsResponse(_message.Message):
-    __slots__ = ["page", "page_size", "sessions", "total"]
+    __slots__ = ["sessions", "page", "page_size", "total"]
+    SESSIONS_FIELD_NUMBER: _ClassVar[int]
     PAGE_FIELD_NUMBER: _ClassVar[int]
     PAGE_SIZE_FIELD_NUMBER: _ClassVar[int]
-    SESSIONS_FIELD_NUMBER: _ClassVar[int]
     TOTAL_FIELD_NUMBER: _ClassVar[int]
+    sessions: _containers.RepeatedCompositeFieldContainer[SessionSummary]
     page: int
     page_size: int
-    sessions: _containers.RepeatedCompositeFieldContainer[SessionSummary]
     total: int
     def __init__(self, sessions: _Optional[_Iterable[_Union[SessionSummary, _Mapping]]] = ..., page: _Optional[int] = ..., page_size: _Optional[int] = ..., total: _Optional[int] = ...) -> None: ...
 
-class SessionRaw(_message.Message):
-    __slots__ = ["cancelled_at", "created_at", "duration", "options", "partition_ids", "session_id", "status"]
-    CANCELLED_AT_FIELD_NUMBER: _ClassVar[int]
-    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
-    DURATION_FIELD_NUMBER: _ClassVar[int]
-    OPTIONS_FIELD_NUMBER: _ClassVar[int]
-    PARTITION_IDS_FIELD_NUMBER: _ClassVar[int]
+class GetSessionRequest(_message.Message):
+    __slots__ = ["session_id"]
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-    STATUS_FIELD_NUMBER: _ClassVar[int]
-    cancelled_at: _timestamp_pb2.Timestamp
-    created_at: _timestamp_pb2.Timestamp
-    duration: _duration_pb2.Duration
-    options: _objects_pb2.TaskOptions
-    partition_ids: _containers.RepeatedScalarFieldContainer[str]
     session_id: str
-    status: _session_status_pb2.SessionStatus
-    def __init__(self, session_id: _Optional[str] = ..., status: _Optional[_Union[_session_status_pb2.SessionStatus, str]] = ..., partition_ids: _Optional[_Iterable[str]] = ..., options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., cancelled_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ...) -> None: ...
+    def __init__(self, session_id: _Optional[str] = ...) -> None: ...
 
-class SessionSummary(_message.Message):
-    __slots__ = ["cancelled_at", "created_at", "duration", "options", "session_id", "status"]
-    CANCELLED_AT_FIELD_NUMBER: _ClassVar[int]
-    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
-    DURATION_FIELD_NUMBER: _ClassVar[int]
-    OPTIONS_FIELD_NUMBER: _ClassVar[int]
+class GetSessionResponse(_message.Message):
+    __slots__ = ["session"]
+    SESSION_FIELD_NUMBER: _ClassVar[int]
+    session: SessionRaw
+    def __init__(self, session: _Optional[_Union[SessionRaw, _Mapping]] = ...) -> None: ...
+
+class CancelSessionRequest(_message.Message):
+    __slots__ = ["session_id"]
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-    STATUS_FIELD_NUMBER: _ClassVar[int]
-    cancelled_at: _timestamp_pb2.Timestamp
-    created_at: _timestamp_pb2.Timestamp
-    duration: _duration_pb2.Duration
-    options: _objects_pb2.TaskOptions
     session_id: str
-    status: _session_status_pb2.SessionStatus
-    def __init__(self, session_id: _Optional[str] = ..., status: _Optional[_Union[_session_status_pb2.SessionStatus, str]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., cancelled_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ...) -> None: ...
+    def __init__(self, session_id: _Optional[str] = ...) -> None: ...
+
+class CancelSessionResponse(_message.Message):
+    __slots__ = ["session"]
+    SESSION_FIELD_NUMBER: _ClassVar[int]
+    session: SessionRaw
+    def __init__(self, session: _Optional[_Union[SessionRaw, _Mapping]] = ...) -> None: ...
+
+class CountTasksByStatusRequest(_message.Message):
+    __slots__ = ["session_id"]
+    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+    session_id: str
+    def __init__(self, session_id: _Optional[str] = ...) -> None: ...
+
+class CountTasksByStatusResponse(_message.Message):
+    __slots__ = ["status"]
+    STATUS_FIELD_NUMBER: _ClassVar[int]
+    status: _containers.RepeatedCompositeFieldContainer[_objects_pb2.StatusCount]
+    def __init__(self, status: _Optional[_Iterable[_Union[_objects_pb2.StatusCount, _Mapping]]] = ...) -> None: ...
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/submitter_common_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/common/submitter_common_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: submitter_common.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from . import objects_pb2 as objects__pb2
 from . import result_status_pb2 as result__status__pb2
 from . import session_status_pb2 as session__status__pb2
 from . import task_status_pb2 as task__status__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16submitter_common.proto\x12\x1d\x61rmonik.api.grpc.v1.submitter\x1a\robjects.proto\x1a\x13result_status.proto\x1a\x14session_status.proto\x1a\x11task_status.proto\"=\n\x0bSessionList\x12.\n\x08sessions\x18\x01 \x03(\x0b\x32\x1c.armonik.api.grpc.v1.Session\"$\n\rSessionIdList\x12\x13\n\x0bsession_ids\x18\x01 \x03(\t\"l\n\x14\x43reateSessionRequest\x12=\n\x13\x64\x65\x66\x61ult_task_option\x18\x01 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12\x15\n\rpartition_ids\x18\x02 \x03(\t\"(\n\x12\x43reateSessionReply\x12\x12\n\nsession_id\x18\x01 \x01(\t\"\x9d\x01\n\x16\x43reateSmallTaskRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x36\n\x0ctask_options\x18\x02 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12\x37\n\rtask_requests\x18\x03 \x03(\x0b\x32 .armonik.api.grpc.v1.TaskRequest\"\xc9\x02\n\x16\x43reateLargeTaskRequest\x12Y\n\x0cinit_request\x18\x01 \x01(\x0b\x32\x41.armonik.api.grpc.v1.submitter.CreateLargeTaskRequest.InitRequestH\x00\x12\x39\n\tinit_task\x18\x02 \x01(\x0b\x32$.armonik.api.grpc.v1.InitTaskRequestH\x00\x12\x36\n\x0ctask_payload\x18\x03 \x01(\x0b\x32\x1e.armonik.api.grpc.v1.DataChunkH\x00\x1aY\n\x0bInitRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x36\n\x0ctask_options\x18\x02 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptionsB\x06\n\x04type\"\xe6\x03\n\x0f\x43reateTaskReply\x12\x61\n\x14\x63reation_status_list\x18\x01 \x01(\x0b\x32\x41.armonik.api.grpc.v1.submitter.CreateTaskReply.CreationStatusListH\x00\x12\x0f\n\x05\x65rror\x18\x02 \x01(\tH\x00\x1ah\n\x08TaskInfo\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x1c\n\x14\x65xpected_output_keys\x18\x02 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x03 \x03(\t\x12\x12\n\npayload_id\x18\x04 \x01(\t\x1ay\n\x0e\x43reationStatus\x12L\n\ttask_info\x18\x01 \x01(\x0b\x32\x37.armonik.api.grpc.v1.submitter.CreateTaskReply.TaskInfoH\x00\x12\x0f\n\x05\x65rror\x18\x02 \x01(\tH\x00\x42\x08\n\x06Status\x1an\n\x12\x43reationStatusList\x12X\n\x11\x63reation_statuses\x18\x01 \x03(\x0b\x32=.armonik.api.grpc.v1.submitter.CreateTaskReply.CreationStatusB\n\n\x08Response\"\xb9\x03\n\nTaskFilter\x12G\n\x07session\x18\x01 \x01(\x0b\x32\x34.armonik.api.grpc.v1.submitter.TaskFilter.IdsRequestH\x00\x12\x44\n\x04task\x18\x03 \x01(\x0b\x32\x34.armonik.api.grpc.v1.submitter.TaskFilter.IdsRequestH\x00\x12M\n\x08included\x18\x04 \x01(\x0b\x32\x39.armonik.api.grpc.v1.submitter.TaskFilter.StatusesRequestH\x01\x12M\n\x08\x65xcluded\x18\x05 \x01(\x0b\x32\x39.armonik.api.grpc.v1.submitter.TaskFilter.StatusesRequestH\x01\x1a\x19\n\nIdsRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\x1aP\n\x0fStatusesRequest\x12=\n\x08statuses\x18\x01 \x03(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatusB\x05\n\x03idsB\n\n\x08statuses\"\xa9\x02\n\rSessionFilter\x12\x10\n\x08sessions\x18\x01 \x03(\t\x12P\n\x08included\x18\x04 \x01(\x0b\x32<.armonik.api.grpc.v1.submitter.SessionFilter.StatusesRequestH\x00\x12P\n\x08\x65xcluded\x18\x05 \x01(\x0b\x32<.armonik.api.grpc.v1.submitter.SessionFilter.StatusesRequestH\x00\x1aV\n\x0fStatusesRequest\x12\x43\n\x08statuses\x18\x01 \x03(\x0e\x32\x31.armonik.api.grpc.v1.session_status.SessionStatusB\n\n\x08statuses\"(\n\x14GetTaskStatusRequest\x12\x10\n\x08task_ids\x18\x01 \x03(\t\"\xbf\x01\n\x12GetTaskStatusReply\x12O\n\x0bid_statuses\x18\x01 \x03(\x0b\x32:.armonik.api.grpc.v1.submitter.GetTaskStatusReply.IdStatus\x1aX\n\x08IdStatus\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12;\n\x06status\x18\x02 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\"@\n\x16GetResultStatusRequest\x12\x12\n\nresult_ids\x18\x01 \x03(\t\x12\x12\n\nsession_id\x18\x02 \x01(\t\"\xc9\x01\n\x14GetResultStatusReply\x12Q\n\x0bid_statuses\x18\x01 \x03(\x0b\x32<.armonik.api.grpc.v1.submitter.GetResultStatusReply.IdStatus\x1a^\n\x08IdStatus\x12\x11\n\tresult_id\x18\x01 \x01(\t\x12?\n\x06status\x18\x02 \x01(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\"\x96\x01\n\x0bResultReply\x12\x30\n\x06result\x18\x01 \x01(\x0b\x32\x1e.armonik.api.grpc.v1.DataChunkH\x00\x12/\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1e.armonik.api.grpc.v1.TaskErrorH\x00\x12\x1c\n\x12not_completed_task\x18\x03 \x01(\tH\x00\x42\x06\n\x04type\"\x94\x01\n\x11\x41vailabilityReply\x12(\n\x02ok\x18\x01 \x01(\x0b\x32\x1a.armonik.api.grpc.v1.EmptyH\x00\x12/\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1e.armonik.api.grpc.v1.TaskErrorH\x00\x12\x1c\n\x12not_completed_task\x18\x03 \x01(\tH\x00\x42\x06\n\x04type\"\x93\x01\n\x0bWaitRequest\x12\x39\n\x06\x66ilter\x18\x01 \x01(\x0b\x32).armonik.api.grpc.v1.submitter.TaskFilter\x12 \n\x18stop_on_first_task_error\x18\x02 \x01(\x08\x12\'\n\x1fstop_on_first_task_cancellation\x18\x03 \x01(\x08\"\xba\x01\n\x12WatchResultRequest\x12G\n\x0e\x66\x65tch_statuses\x18\x01 \x03(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\x12G\n\x0ewatch_statuses\x18\x02 \x03(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\x12\x12\n\nresult_ids\x18\x03 \x03(\t\"h\n\x11WatchResultStream\x12?\n\x06status\x18\x01 \x01(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\x12\x12\n\nresult_ids\x18\x02 \x03(\tB \xaa\x02\x1d\x41rmoniK.Api.gRPC.V1.Submitterb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'submitter_common_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'submitter_common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\035ArmoniK.Api.gRPC.V1.Submitter'
-  _SESSIONLIST._serialized_start=134
-  _SESSIONLIST._serialized_end=195
-  _SESSIONIDLIST._serialized_start=197
-  _SESSIONIDLIST._serialized_end=233
-  _CREATESESSIONREQUEST._serialized_start=235
-  _CREATESESSIONREQUEST._serialized_end=343
-  _CREATESESSIONREPLY._serialized_start=345
-  _CREATESESSIONREPLY._serialized_end=385
-  _CREATESMALLTASKREQUEST._serialized_start=388
-  _CREATESMALLTASKREQUEST._serialized_end=545
-  _CREATELARGETASKREQUEST._serialized_start=548
-  _CREATELARGETASKREQUEST._serialized_end=877
-  _CREATELARGETASKREQUEST_INITREQUEST._serialized_start=780
-  _CREATELARGETASKREQUEST_INITREQUEST._serialized_end=869
-  _CREATETASKREPLY._serialized_start=880
-  _CREATETASKREPLY._serialized_end=1366
-  _CREATETASKREPLY_TASKINFO._serialized_start=1015
-  _CREATETASKREPLY_TASKINFO._serialized_end=1119
-  _CREATETASKREPLY_CREATIONSTATUS._serialized_start=1121
-  _CREATETASKREPLY_CREATIONSTATUS._serialized_end=1242
-  _CREATETASKREPLY_CREATIONSTATUSLIST._serialized_start=1244
-  _CREATETASKREPLY_CREATIONSTATUSLIST._serialized_end=1354
-  _TASKFILTER._serialized_start=1369
-  _TASKFILTER._serialized_end=1810
-  _TASKFILTER_IDSREQUEST._serialized_start=1684
-  _TASKFILTER_IDSREQUEST._serialized_end=1709
-  _TASKFILTER_STATUSESREQUEST._serialized_start=1711
-  _TASKFILTER_STATUSESREQUEST._serialized_end=1791
-  _SESSIONFILTER._serialized_start=1813
-  _SESSIONFILTER._serialized_end=2110
-  _SESSIONFILTER_STATUSESREQUEST._serialized_start=2012
-  _SESSIONFILTER_STATUSESREQUEST._serialized_end=2098
-  _GETTASKSTATUSREQUEST._serialized_start=2112
-  _GETTASKSTATUSREQUEST._serialized_end=2152
-  _GETTASKSTATUSREPLY._serialized_start=2155
-  _GETTASKSTATUSREPLY._serialized_end=2346
-  _GETTASKSTATUSREPLY_IDSTATUS._serialized_start=2258
-  _GETTASKSTATUSREPLY_IDSTATUS._serialized_end=2346
-  _GETRESULTSTATUSREQUEST._serialized_start=2348
-  _GETRESULTSTATUSREQUEST._serialized_end=2412
-  _GETRESULTSTATUSREPLY._serialized_start=2415
-  _GETRESULTSTATUSREPLY._serialized_end=2616
-  _GETRESULTSTATUSREPLY_IDSTATUS._serialized_start=2522
-  _GETRESULTSTATUSREPLY_IDSTATUS._serialized_end=2616
-  _RESULTREPLY._serialized_start=2619
-  _RESULTREPLY._serialized_end=2769
-  _AVAILABILITYREPLY._serialized_start=2772
-  _AVAILABILITYREPLY._serialized_end=2920
-  _WAITREQUEST._serialized_start=2923
-  _WAITREQUEST._serialized_end=3070
-  _WATCHRESULTREQUEST._serialized_start=3073
-  _WATCHRESULTREQUEST._serialized_end=3259
-  _WATCHRESULTSTREAM._serialized_start=3261
-  _WATCHRESULTSTREAM._serialized_end=3365
+  _globals['_SESSIONLIST']._serialized_start=134
+  _globals['_SESSIONLIST']._serialized_end=195
+  _globals['_SESSIONIDLIST']._serialized_start=197
+  _globals['_SESSIONIDLIST']._serialized_end=233
+  _globals['_CREATESESSIONREQUEST']._serialized_start=235
+  _globals['_CREATESESSIONREQUEST']._serialized_end=343
+  _globals['_CREATESESSIONREPLY']._serialized_start=345
+  _globals['_CREATESESSIONREPLY']._serialized_end=385
+  _globals['_CREATESMALLTASKREQUEST']._serialized_start=388
+  _globals['_CREATESMALLTASKREQUEST']._serialized_end=545
+  _globals['_CREATELARGETASKREQUEST']._serialized_start=548
+  _globals['_CREATELARGETASKREQUEST']._serialized_end=877
+  _globals['_CREATELARGETASKREQUEST_INITREQUEST']._serialized_start=780
+  _globals['_CREATELARGETASKREQUEST_INITREQUEST']._serialized_end=869
+  _globals['_CREATETASKREPLY']._serialized_start=880
+  _globals['_CREATETASKREPLY']._serialized_end=1366
+  _globals['_CREATETASKREPLY_TASKINFO']._serialized_start=1015
+  _globals['_CREATETASKREPLY_TASKINFO']._serialized_end=1119
+  _globals['_CREATETASKREPLY_CREATIONSTATUS']._serialized_start=1121
+  _globals['_CREATETASKREPLY_CREATIONSTATUS']._serialized_end=1242
+  _globals['_CREATETASKREPLY_CREATIONSTATUSLIST']._serialized_start=1244
+  _globals['_CREATETASKREPLY_CREATIONSTATUSLIST']._serialized_end=1354
+  _globals['_TASKFILTER']._serialized_start=1369
+  _globals['_TASKFILTER']._serialized_end=1810
+  _globals['_TASKFILTER_IDSREQUEST']._serialized_start=1684
+  _globals['_TASKFILTER_IDSREQUEST']._serialized_end=1709
+  _globals['_TASKFILTER_STATUSESREQUEST']._serialized_start=1711
+  _globals['_TASKFILTER_STATUSESREQUEST']._serialized_end=1791
+  _globals['_SESSIONFILTER']._serialized_start=1813
+  _globals['_SESSIONFILTER']._serialized_end=2110
+  _globals['_SESSIONFILTER_STATUSESREQUEST']._serialized_start=2012
+  _globals['_SESSIONFILTER_STATUSESREQUEST']._serialized_end=2098
+  _globals['_GETTASKSTATUSREQUEST']._serialized_start=2112
+  _globals['_GETTASKSTATUSREQUEST']._serialized_end=2152
+  _globals['_GETTASKSTATUSREPLY']._serialized_start=2155
+  _globals['_GETTASKSTATUSREPLY']._serialized_end=2346
+  _globals['_GETTASKSTATUSREPLY_IDSTATUS']._serialized_start=2258
+  _globals['_GETTASKSTATUSREPLY_IDSTATUS']._serialized_end=2346
+  _globals['_GETRESULTSTATUSREQUEST']._serialized_start=2348
+  _globals['_GETRESULTSTATUSREQUEST']._serialized_end=2412
+  _globals['_GETRESULTSTATUSREPLY']._serialized_start=2415
+  _globals['_GETRESULTSTATUSREPLY']._serialized_end=2616
+  _globals['_GETRESULTSTATUSREPLY_IDSTATUS']._serialized_start=2522
+  _globals['_GETRESULTSTATUSREPLY_IDSTATUS']._serialized_end=2616
+  _globals['_RESULTREPLY']._serialized_start=2619
+  _globals['_RESULTREPLY']._serialized_end=2769
+  _globals['_AVAILABILITYREPLY']._serialized_start=2772
+  _globals['_AVAILABILITYREPLY']._serialized_end=2920
+  _globals['_WAITREQUEST']._serialized_start=2923
+  _globals['_WAITREQUEST']._serialized_end=3070
+  _globals['_WATCHRESULTREQUEST']._serialized_start=3073
+  _globals['_WATCHRESULTREQUEST']._serialized_end=3259
+  _globals['_WATCHRESULTSTREAM']._serialized_start=3261
+  _globals['_WATCHRESULTSTREAM']._serialized_end=3365
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/submitter_common_pb2.pyi` & `armonik-3.8.2.dev349/src/armonik/protogen/common/submitter_common_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -5,215 +5,215 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class AvailabilityReply(_message.Message):
-    __slots__ = ["error", "not_completed_task", "ok"]
-    ERROR_FIELD_NUMBER: _ClassVar[int]
-    NOT_COMPLETED_TASK_FIELD_NUMBER: _ClassVar[int]
-    OK_FIELD_NUMBER: _ClassVar[int]
-    error: _objects_pb2.TaskError
-    not_completed_task: str
-    ok: _objects_pb2.Empty
-    def __init__(self, ok: _Optional[_Union[_objects_pb2.Empty, _Mapping]] = ..., error: _Optional[_Union[_objects_pb2.TaskError, _Mapping]] = ..., not_completed_task: _Optional[str] = ...) -> None: ...
-
-class CreateLargeTaskRequest(_message.Message):
-    __slots__ = ["init_request", "init_task", "task_payload"]
-    class InitRequest(_message.Message):
-        __slots__ = ["session_id", "task_options"]
-        SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-        TASK_OPTIONS_FIELD_NUMBER: _ClassVar[int]
-        session_id: str
-        task_options: _objects_pb2.TaskOptions
-        def __init__(self, session_id: _Optional[str] = ..., task_options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ...) -> None: ...
-    INIT_REQUEST_FIELD_NUMBER: _ClassVar[int]
-    INIT_TASK_FIELD_NUMBER: _ClassVar[int]
-    TASK_PAYLOAD_FIELD_NUMBER: _ClassVar[int]
-    init_request: CreateLargeTaskRequest.InitRequest
-    init_task: _objects_pb2.InitTaskRequest
-    task_payload: _objects_pb2.DataChunk
-    def __init__(self, init_request: _Optional[_Union[CreateLargeTaskRequest.InitRequest, _Mapping]] = ..., init_task: _Optional[_Union[_objects_pb2.InitTaskRequest, _Mapping]] = ..., task_payload: _Optional[_Union[_objects_pb2.DataChunk, _Mapping]] = ...) -> None: ...
+class SessionList(_message.Message):
+    __slots__ = ["sessions"]
+    SESSIONS_FIELD_NUMBER: _ClassVar[int]
+    sessions: _containers.RepeatedCompositeFieldContainer[_objects_pb2.Session]
+    def __init__(self, sessions: _Optional[_Iterable[_Union[_objects_pb2.Session, _Mapping]]] = ...) -> None: ...
 
-class CreateSessionReply(_message.Message):
-    __slots__ = ["session_id"]
-    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-    session_id: str
-    def __init__(self, session_id: _Optional[str] = ...) -> None: ...
+class SessionIdList(_message.Message):
+    __slots__ = ["session_ids"]
+    SESSION_IDS_FIELD_NUMBER: _ClassVar[int]
+    session_ids: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, session_ids: _Optional[_Iterable[str]] = ...) -> None: ...
 
 class CreateSessionRequest(_message.Message):
     __slots__ = ["default_task_option", "partition_ids"]
     DEFAULT_TASK_OPTION_FIELD_NUMBER: _ClassVar[int]
     PARTITION_IDS_FIELD_NUMBER: _ClassVar[int]
     default_task_option: _objects_pb2.TaskOptions
     partition_ids: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, default_task_option: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., partition_ids: _Optional[_Iterable[str]] = ...) -> None: ...
 
+class CreateSessionReply(_message.Message):
+    __slots__ = ["session_id"]
+    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+    session_id: str
+    def __init__(self, session_id: _Optional[str] = ...) -> None: ...
+
 class CreateSmallTaskRequest(_message.Message):
     __slots__ = ["session_id", "task_options", "task_requests"]
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
     TASK_OPTIONS_FIELD_NUMBER: _ClassVar[int]
     TASK_REQUESTS_FIELD_NUMBER: _ClassVar[int]
     session_id: str
     task_options: _objects_pb2.TaskOptions
     task_requests: _containers.RepeatedCompositeFieldContainer[_objects_pb2.TaskRequest]
     def __init__(self, session_id: _Optional[str] = ..., task_options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., task_requests: _Optional[_Iterable[_Union[_objects_pb2.TaskRequest, _Mapping]]] = ...) -> None: ...
 
+class CreateLargeTaskRequest(_message.Message):
+    __slots__ = ["init_request", "init_task", "task_payload"]
+    class InitRequest(_message.Message):
+        __slots__ = ["session_id", "task_options"]
+        SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+        TASK_OPTIONS_FIELD_NUMBER: _ClassVar[int]
+        session_id: str
+        task_options: _objects_pb2.TaskOptions
+        def __init__(self, session_id: _Optional[str] = ..., task_options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ...) -> None: ...
+    INIT_REQUEST_FIELD_NUMBER: _ClassVar[int]
+    INIT_TASK_FIELD_NUMBER: _ClassVar[int]
+    TASK_PAYLOAD_FIELD_NUMBER: _ClassVar[int]
+    init_request: CreateLargeTaskRequest.InitRequest
+    init_task: _objects_pb2.InitTaskRequest
+    task_payload: _objects_pb2.DataChunk
+    def __init__(self, init_request: _Optional[_Union[CreateLargeTaskRequest.InitRequest, _Mapping]] = ..., init_task: _Optional[_Union[_objects_pb2.InitTaskRequest, _Mapping]] = ..., task_payload: _Optional[_Union[_objects_pb2.DataChunk, _Mapping]] = ...) -> None: ...
+
 class CreateTaskReply(_message.Message):
     __slots__ = ["creation_status_list", "error"]
+    class TaskInfo(_message.Message):
+        __slots__ = ["task_id", "expected_output_keys", "data_dependencies", "payload_id"]
+        TASK_ID_FIELD_NUMBER: _ClassVar[int]
+        EXPECTED_OUTPUT_KEYS_FIELD_NUMBER: _ClassVar[int]
+        DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
+        PAYLOAD_ID_FIELD_NUMBER: _ClassVar[int]
+        task_id: str
+        expected_output_keys: _containers.RepeatedScalarFieldContainer[str]
+        data_dependencies: _containers.RepeatedScalarFieldContainer[str]
+        payload_id: str
+        def __init__(self, task_id: _Optional[str] = ..., expected_output_keys: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., payload_id: _Optional[str] = ...) -> None: ...
     class CreationStatus(_message.Message):
-        __slots__ = ["error", "task_info"]
-        ERROR_FIELD_NUMBER: _ClassVar[int]
+        __slots__ = ["task_info", "error"]
         TASK_INFO_FIELD_NUMBER: _ClassVar[int]
-        error: str
+        ERROR_FIELD_NUMBER: _ClassVar[int]
         task_info: CreateTaskReply.TaskInfo
+        error: str
         def __init__(self, task_info: _Optional[_Union[CreateTaskReply.TaskInfo, _Mapping]] = ..., error: _Optional[str] = ...) -> None: ...
     class CreationStatusList(_message.Message):
         __slots__ = ["creation_statuses"]
         CREATION_STATUSES_FIELD_NUMBER: _ClassVar[int]
         creation_statuses: _containers.RepeatedCompositeFieldContainer[CreateTaskReply.CreationStatus]
         def __init__(self, creation_statuses: _Optional[_Iterable[_Union[CreateTaskReply.CreationStatus, _Mapping]]] = ...) -> None: ...
-    class TaskInfo(_message.Message):
-        __slots__ = ["data_dependencies", "expected_output_keys", "payload_id", "task_id"]
-        DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
-        EXPECTED_OUTPUT_KEYS_FIELD_NUMBER: _ClassVar[int]
-        PAYLOAD_ID_FIELD_NUMBER: _ClassVar[int]
-        TASK_ID_FIELD_NUMBER: _ClassVar[int]
-        data_dependencies: _containers.RepeatedScalarFieldContainer[str]
-        expected_output_keys: _containers.RepeatedScalarFieldContainer[str]
-        payload_id: str
-        task_id: str
-        def __init__(self, task_id: _Optional[str] = ..., expected_output_keys: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., payload_id: _Optional[str] = ...) -> None: ...
     CREATION_STATUS_LIST_FIELD_NUMBER: _ClassVar[int]
     ERROR_FIELD_NUMBER: _ClassVar[int]
     creation_status_list: CreateTaskReply.CreationStatusList
     error: str
     def __init__(self, creation_status_list: _Optional[_Union[CreateTaskReply.CreationStatusList, _Mapping]] = ..., error: _Optional[str] = ...) -> None: ...
 
-class GetResultStatusReply(_message.Message):
+class TaskFilter(_message.Message):
+    __slots__ = ["session", "task", "included", "excluded"]
+    class IdsRequest(_message.Message):
+        __slots__ = ["ids"]
+        IDS_FIELD_NUMBER: _ClassVar[int]
+        ids: _containers.RepeatedScalarFieldContainer[str]
+        def __init__(self, ids: _Optional[_Iterable[str]] = ...) -> None: ...
+    class StatusesRequest(_message.Message):
+        __slots__ = ["statuses"]
+        STATUSES_FIELD_NUMBER: _ClassVar[int]
+        statuses: _containers.RepeatedScalarFieldContainer[_task_status_pb2.TaskStatus]
+        def __init__(self, statuses: _Optional[_Iterable[_Union[_task_status_pb2.TaskStatus, str]]] = ...) -> None: ...
+    SESSION_FIELD_NUMBER: _ClassVar[int]
+    TASK_FIELD_NUMBER: _ClassVar[int]
+    INCLUDED_FIELD_NUMBER: _ClassVar[int]
+    EXCLUDED_FIELD_NUMBER: _ClassVar[int]
+    session: TaskFilter.IdsRequest
+    task: TaskFilter.IdsRequest
+    included: TaskFilter.StatusesRequest
+    excluded: TaskFilter.StatusesRequest
+    def __init__(self, session: _Optional[_Union[TaskFilter.IdsRequest, _Mapping]] = ..., task: _Optional[_Union[TaskFilter.IdsRequest, _Mapping]] = ..., included: _Optional[_Union[TaskFilter.StatusesRequest, _Mapping]] = ..., excluded: _Optional[_Union[TaskFilter.StatusesRequest, _Mapping]] = ...) -> None: ...
+
+class SessionFilter(_message.Message):
+    __slots__ = ["sessions", "included", "excluded"]
+    class StatusesRequest(_message.Message):
+        __slots__ = ["statuses"]
+        STATUSES_FIELD_NUMBER: _ClassVar[int]
+        statuses: _containers.RepeatedScalarFieldContainer[_session_status_pb2.SessionStatus]
+        def __init__(self, statuses: _Optional[_Iterable[_Union[_session_status_pb2.SessionStatus, str]]] = ...) -> None: ...
+    SESSIONS_FIELD_NUMBER: _ClassVar[int]
+    INCLUDED_FIELD_NUMBER: _ClassVar[int]
+    EXCLUDED_FIELD_NUMBER: _ClassVar[int]
+    sessions: _containers.RepeatedScalarFieldContainer[str]
+    included: SessionFilter.StatusesRequest
+    excluded: SessionFilter.StatusesRequest
+    def __init__(self, sessions: _Optional[_Iterable[str]] = ..., included: _Optional[_Union[SessionFilter.StatusesRequest, _Mapping]] = ..., excluded: _Optional[_Union[SessionFilter.StatusesRequest, _Mapping]] = ...) -> None: ...
+
+class GetTaskStatusRequest(_message.Message):
+    __slots__ = ["task_ids"]
+    TASK_IDS_FIELD_NUMBER: _ClassVar[int]
+    task_ids: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, task_ids: _Optional[_Iterable[str]] = ...) -> None: ...
+
+class GetTaskStatusReply(_message.Message):
     __slots__ = ["id_statuses"]
     class IdStatus(_message.Message):
-        __slots__ = ["result_id", "status"]
-        RESULT_ID_FIELD_NUMBER: _ClassVar[int]
+        __slots__ = ["task_id", "status"]
+        TASK_ID_FIELD_NUMBER: _ClassVar[int]
         STATUS_FIELD_NUMBER: _ClassVar[int]
-        result_id: str
-        status: _result_status_pb2.ResultStatus
-        def __init__(self, result_id: _Optional[str] = ..., status: _Optional[_Union[_result_status_pb2.ResultStatus, str]] = ...) -> None: ...
+        task_id: str
+        status: _task_status_pb2.TaskStatus
+        def __init__(self, task_id: _Optional[str] = ..., status: _Optional[_Union[_task_status_pb2.TaskStatus, str]] = ...) -> None: ...
     ID_STATUSES_FIELD_NUMBER: _ClassVar[int]
-    id_statuses: _containers.RepeatedCompositeFieldContainer[GetResultStatusReply.IdStatus]
-    def __init__(self, id_statuses: _Optional[_Iterable[_Union[GetResultStatusReply.IdStatus, _Mapping]]] = ...) -> None: ...
+    id_statuses: _containers.RepeatedCompositeFieldContainer[GetTaskStatusReply.IdStatus]
+    def __init__(self, id_statuses: _Optional[_Iterable[_Union[GetTaskStatusReply.IdStatus, _Mapping]]] = ...) -> None: ...
 
 class GetResultStatusRequest(_message.Message):
     __slots__ = ["result_ids", "session_id"]
     RESULT_IDS_FIELD_NUMBER: _ClassVar[int]
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
     result_ids: _containers.RepeatedScalarFieldContainer[str]
     session_id: str
     def __init__(self, result_ids: _Optional[_Iterable[str]] = ..., session_id: _Optional[str] = ...) -> None: ...
 
-class GetTaskStatusReply(_message.Message):
+class GetResultStatusReply(_message.Message):
     __slots__ = ["id_statuses"]
     class IdStatus(_message.Message):
-        __slots__ = ["status", "task_id"]
+        __slots__ = ["result_id", "status"]
+        RESULT_ID_FIELD_NUMBER: _ClassVar[int]
         STATUS_FIELD_NUMBER: _ClassVar[int]
-        TASK_ID_FIELD_NUMBER: _ClassVar[int]
-        status: _task_status_pb2.TaskStatus
-        task_id: str
-        def __init__(self, task_id: _Optional[str] = ..., status: _Optional[_Union[_task_status_pb2.TaskStatus, str]] = ...) -> None: ...
+        result_id: str
+        status: _result_status_pb2.ResultStatus
+        def __init__(self, result_id: _Optional[str] = ..., status: _Optional[_Union[_result_status_pb2.ResultStatus, str]] = ...) -> None: ...
     ID_STATUSES_FIELD_NUMBER: _ClassVar[int]
-    id_statuses: _containers.RepeatedCompositeFieldContainer[GetTaskStatusReply.IdStatus]
-    def __init__(self, id_statuses: _Optional[_Iterable[_Union[GetTaskStatusReply.IdStatus, _Mapping]]] = ...) -> None: ...
-
-class GetTaskStatusRequest(_message.Message):
-    __slots__ = ["task_ids"]
-    TASK_IDS_FIELD_NUMBER: _ClassVar[int]
-    task_ids: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, task_ids: _Optional[_Iterable[str]] = ...) -> None: ...
+    id_statuses: _containers.RepeatedCompositeFieldContainer[GetResultStatusReply.IdStatus]
+    def __init__(self, id_statuses: _Optional[_Iterable[_Union[GetResultStatusReply.IdStatus, _Mapping]]] = ...) -> None: ...
 
 class ResultReply(_message.Message):
-    __slots__ = ["error", "not_completed_task", "result"]
+    __slots__ = ["result", "error", "not_completed_task"]
+    RESULT_FIELD_NUMBER: _ClassVar[int]
     ERROR_FIELD_NUMBER: _ClassVar[int]
     NOT_COMPLETED_TASK_FIELD_NUMBER: _ClassVar[int]
-    RESULT_FIELD_NUMBER: _ClassVar[int]
+    result: _objects_pb2.DataChunk
     error: _objects_pb2.TaskError
     not_completed_task: str
-    result: _objects_pb2.DataChunk
     def __init__(self, result: _Optional[_Union[_objects_pb2.DataChunk, _Mapping]] = ..., error: _Optional[_Union[_objects_pb2.TaskError, _Mapping]] = ..., not_completed_task: _Optional[str] = ...) -> None: ...
 
-class SessionFilter(_message.Message):
-    __slots__ = ["excluded", "included", "sessions"]
-    class StatusesRequest(_message.Message):
-        __slots__ = ["statuses"]
-        STATUSES_FIELD_NUMBER: _ClassVar[int]
-        statuses: _containers.RepeatedScalarFieldContainer[_session_status_pb2.SessionStatus]
-        def __init__(self, statuses: _Optional[_Iterable[_Union[_session_status_pb2.SessionStatus, str]]] = ...) -> None: ...
-    EXCLUDED_FIELD_NUMBER: _ClassVar[int]
-    INCLUDED_FIELD_NUMBER: _ClassVar[int]
-    SESSIONS_FIELD_NUMBER: _ClassVar[int]
-    excluded: SessionFilter.StatusesRequest
-    included: SessionFilter.StatusesRequest
-    sessions: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, sessions: _Optional[_Iterable[str]] = ..., included: _Optional[_Union[SessionFilter.StatusesRequest, _Mapping]] = ..., excluded: _Optional[_Union[SessionFilter.StatusesRequest, _Mapping]] = ...) -> None: ...
-
-class SessionIdList(_message.Message):
-    __slots__ = ["session_ids"]
-    SESSION_IDS_FIELD_NUMBER: _ClassVar[int]
-    session_ids: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, session_ids: _Optional[_Iterable[str]] = ...) -> None: ...
-
-class SessionList(_message.Message):
-    __slots__ = ["sessions"]
-    SESSIONS_FIELD_NUMBER: _ClassVar[int]
-    sessions: _containers.RepeatedCompositeFieldContainer[_objects_pb2.Session]
-    def __init__(self, sessions: _Optional[_Iterable[_Union[_objects_pb2.Session, _Mapping]]] = ...) -> None: ...
-
-class TaskFilter(_message.Message):
-    __slots__ = ["excluded", "included", "session", "task"]
-    class IdsRequest(_message.Message):
-        __slots__ = ["ids"]
-        IDS_FIELD_NUMBER: _ClassVar[int]
-        ids: _containers.RepeatedScalarFieldContainer[str]
-        def __init__(self, ids: _Optional[_Iterable[str]] = ...) -> None: ...
-    class StatusesRequest(_message.Message):
-        __slots__ = ["statuses"]
-        STATUSES_FIELD_NUMBER: _ClassVar[int]
-        statuses: _containers.RepeatedScalarFieldContainer[_task_status_pb2.TaskStatus]
-        def __init__(self, statuses: _Optional[_Iterable[_Union[_task_status_pb2.TaskStatus, str]]] = ...) -> None: ...
-    EXCLUDED_FIELD_NUMBER: _ClassVar[int]
-    INCLUDED_FIELD_NUMBER: _ClassVar[int]
-    SESSION_FIELD_NUMBER: _ClassVar[int]
-    TASK_FIELD_NUMBER: _ClassVar[int]
-    excluded: TaskFilter.StatusesRequest
-    included: TaskFilter.StatusesRequest
-    session: TaskFilter.IdsRequest
-    task: TaskFilter.IdsRequest
-    def __init__(self, session: _Optional[_Union[TaskFilter.IdsRequest, _Mapping]] = ..., task: _Optional[_Union[TaskFilter.IdsRequest, _Mapping]] = ..., included: _Optional[_Union[TaskFilter.StatusesRequest, _Mapping]] = ..., excluded: _Optional[_Union[TaskFilter.StatusesRequest, _Mapping]] = ...) -> None: ...
+class AvailabilityReply(_message.Message):
+    __slots__ = ["ok", "error", "not_completed_task"]
+    OK_FIELD_NUMBER: _ClassVar[int]
+    ERROR_FIELD_NUMBER: _ClassVar[int]
+    NOT_COMPLETED_TASK_FIELD_NUMBER: _ClassVar[int]
+    ok: _objects_pb2.Empty
+    error: _objects_pb2.TaskError
+    not_completed_task: str
+    def __init__(self, ok: _Optional[_Union[_objects_pb2.Empty, _Mapping]] = ..., error: _Optional[_Union[_objects_pb2.TaskError, _Mapping]] = ..., not_completed_task: _Optional[str] = ...) -> None: ...
 
 class WaitRequest(_message.Message):
-    __slots__ = ["filter", "stop_on_first_task_cancellation", "stop_on_first_task_error"]
+    __slots__ = ["filter", "stop_on_first_task_error", "stop_on_first_task_cancellation"]
     FILTER_FIELD_NUMBER: _ClassVar[int]
-    STOP_ON_FIRST_TASK_CANCELLATION_FIELD_NUMBER: _ClassVar[int]
     STOP_ON_FIRST_TASK_ERROR_FIELD_NUMBER: _ClassVar[int]
+    STOP_ON_FIRST_TASK_CANCELLATION_FIELD_NUMBER: _ClassVar[int]
     filter: TaskFilter
-    stop_on_first_task_cancellation: bool
     stop_on_first_task_error: bool
+    stop_on_first_task_cancellation: bool
     def __init__(self, filter: _Optional[_Union[TaskFilter, _Mapping]] = ..., stop_on_first_task_error: bool = ..., stop_on_first_task_cancellation: bool = ...) -> None: ...
 
 class WatchResultRequest(_message.Message):
-    __slots__ = ["fetch_statuses", "result_ids", "watch_statuses"]
+    __slots__ = ["fetch_statuses", "watch_statuses", "result_ids"]
     FETCH_STATUSES_FIELD_NUMBER: _ClassVar[int]
-    RESULT_IDS_FIELD_NUMBER: _ClassVar[int]
     WATCH_STATUSES_FIELD_NUMBER: _ClassVar[int]
+    RESULT_IDS_FIELD_NUMBER: _ClassVar[int]
     fetch_statuses: _containers.RepeatedScalarFieldContainer[_result_status_pb2.ResultStatus]
-    result_ids: _containers.RepeatedScalarFieldContainer[str]
     watch_statuses: _containers.RepeatedScalarFieldContainer[_result_status_pb2.ResultStatus]
+    result_ids: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, fetch_statuses: _Optional[_Iterable[_Union[_result_status_pb2.ResultStatus, str]]] = ..., watch_statuses: _Optional[_Iterable[_Union[_result_status_pb2.ResultStatus, str]]] = ..., result_ids: _Optional[_Iterable[str]] = ...) -> None: ...
 
 class WatchResultStream(_message.Message):
-    __slots__ = ["result_ids", "status"]
-    RESULT_IDS_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["status", "result_ids"]
     STATUS_FIELD_NUMBER: _ClassVar[int]
-    result_ids: _containers.RepeatedScalarFieldContainer[str]
+    RESULT_IDS_FIELD_NUMBER: _ClassVar[int]
     status: _result_status_pb2.ResultStatus
+    result_ids: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, status: _Optional[_Union[_result_status_pb2.ResultStatus, str]] = ..., result_ids: _Optional[_Iterable[str]] = ...) -> None: ...
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/tasks_common_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/common/tasks_common_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,75 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: tasks_common.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from . import objects_pb2 as objects__pb2
 from . import task_status_pb2 as task__status__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12tasks_common.proto\x12\x19\x61rmonik.api.grpc.v1.tasks\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\robjects.proto\x1a\x11task_status.proto\"\xf4\x06\n\x07TaskRaw\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nsession_id\x18\x02 \x01(\t\x12\x14\n\x0cowner_pod_id\x18\x03 \x01(\t\x12\x17\n\x0fparent_task_ids\x18\x04 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x05 \x03(\t\x12\x1b\n\x13\x65xpected_output_ids\x18\x06 \x03(\t\x12\x14\n\x0cretry_of_ids\x18\x07 \x03(\t\x12;\n\x06status\x18\x08 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12\x16\n\x0estatus_message\x18\t \x01(\t\x12\x31\n\x07options\x18\n \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12.\n\ncreated_at\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0csubmitted_at\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nstarted_at\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nded_at\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12;\n\x18\x63reation_to_end_duration\x18\x14 \x01(\x0b\x32\x19.google.protobuf.Duration\x12=\n\x1aprocessing_to_end_duration\x18\x15 \x01(\x0b\x32\x19.google.protobuf.Duration\x12+\n\x07pod_ttl\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x06output\x18\x10 \x01(\x0b\x32).armonik.api.grpc.v1.tasks.TaskRaw.Output\x12\x14\n\x0cpod_hostname\x18\x11 \x01(\t\x12/\n\x0breceived_at\x18\x12 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0b\x61\x63quired_at\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x1a(\n\x06Output\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"\xb6\x03\n\x0bTaskSummary\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nsession_id\x18\x02 \x01(\t\x12\x31\n\x07options\x18\x03 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12;\n\x06status\x18\x04 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nstarted_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nded_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12;\n\x18\x63reation_to_end_duration\x18\x0f \x01(\x0b\x32\x19.google.protobuf.Duration\x12=\n\x1aprocessing_to_end_duration\x18\x10 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\r\n\x05\x65rror\x18\x08 \x01(\t\"\xc2\x08\n\x10ListTasksRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x42\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x32.armonik.api.grpc.v1.tasks.ListTasksRequest.Filter\x12>\n\x04sort\x18\x04 \x01(\x0b\x32\x30.armonik.api.grpc.v1.tasks.ListTasksRequest.Sort\x12\x13\n\x0bwith_errors\x18\x05 \x01(\x08\x1a\x8a\x03\n\x06\x46ilter\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12;\n\x06status\x18\x02 \x03(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12\x31\n\rcreated_after\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0e\x63reated_before\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rstarted_after\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0estarted_before\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0b\x65nded_after\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x65nded_before\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x1a\x9e\x01\n\x04Sort\x12G\n\x05\x66ield\x18\x01 \x01(\x0e\x32\x38.armonik.api.grpc.v1.tasks.ListTasksRequest.OrderByField\x12M\n\tdirection\x18\x02 \x01(\x0e\x32:.armonik.api.grpc.v1.tasks.ListTasksRequest.OrderDirection\"\xdf\x01\n\x0cOrderByField\x12\x1e\n\x1aORDER_BY_FIELD_UNSPECIFIED\x10\x00\x12\x1a\n\x16ORDER_BY_FIELD_TASK_ID\x10\x01\x12\x1d\n\x19ORDER_BY_FIELD_SESSION_ID\x10\x02\x12\x19\n\x15ORDER_BY_FIELD_STATUS\x10\x03\x12\x1d\n\x19ORDER_BY_FIELD_CREATED_AT\x10\x04\x12\x1d\n\x19ORDER_BY_FIELD_STARTED_AT\x10\x05\x12\x1b\n\x17ORDER_BY_FIELD_ENDED_AT\x10\x06\"d\n\x0eOrderDirection\x12\x1f\n\x1bORDER_DIRECTION_UNSPECIFIED\x10\x00\x12\x17\n\x13ORDER_DIRECTION_ASC\x10\x01\x12\x18\n\x14ORDER_DIRECTION_DESC\x10\x02\"z\n\x11ListTasksResponse\x12\x35\n\x05tasks\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.tasks.TaskSummary\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"y\n\x14ListTasksRawResponse\x12\x31\n\x05tasks\x18\x01 \x03(\x0b\x32\".armonik.api.grpc.v1.tasks.TaskRaw\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"!\n\x0eGetTaskRequest\x12\x0f\n\x07task_id\x18\x01 \x01(\t\"C\n\x0fGetTaskResponse\x12\x30\n\x04task\x18\x01 \x01(\x0b\x32\".armonik.api.grpc.v1.tasks.TaskRaw\"&\n\x12\x43\x61ncelTasksRequest\x12\x10\n\x08task_ids\x18\x01 \x03(\t\"L\n\x13\x43\x61ncelTasksResponse\x12\x35\n\x05tasks\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.tasks.TaskSummary\"&\n\x13GetResultIdsRequest\x12\x0f\n\x07task_id\x18\x01 \x03(\t\"\xa1\x01\n\x14GetResultIdsResponse\x12S\n\x0ctask_results\x18\x01 \x03(\x0b\x32=.armonik.api.grpc.v1.tasks.GetResultIdsResponse.MapTaskResult\x1a\x34\n\rMapTaskResult\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x12\n\nresult_ids\x18\x02 \x03(\t\"\x1b\n\x19\x43ountTasksByStatusRequest\"N\n\x1a\x43ountTasksByStatusResponse\x12\x30\n\x06status\x18\x01 \x03(\x0b\x32 .armonik.api.grpc.v1.StatusCount\"\xca\x02\n\x12SubmitTasksRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x36\n\x0ctask_options\x18\x02 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12R\n\x0etask_creations\x18\x03 \x03(\x0b\x32:.armonik.api.grpc.v1.tasks.SubmitTasksRequest.TaskCreation\x1a\x93\x01\n\x0cTaskCreation\x12\x1c\n\x14\x65xpected_output_keys\x18\x01 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x02 \x03(\t\x12\x12\n\npayload_id\x18\x03 \x01(\t\x12\x36\n\x0ctask_options\x18\x04 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\"\xcb\x01\n\x13SubmitTasksResponse\x12K\n\ntask_infos\x18\x01 \x03(\x0b\x32\x37.armonik.api.grpc.v1.tasks.SubmitTasksResponse.TaskInfo\x1ag\n\x08TaskInfo\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x1b\n\x13\x65xpected_output_ids\x18\x02 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x03 \x03(\t\x12\x12\n\npayload_id\x18\x04 \x01(\tB\x1c\xaa\x02\x19\x41rmoniK.Api.gRPC.V1.Tasksb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tasks_common_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tasks_common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\031ArmoniK.Api.gRPC.V1.Tasks'
-  _TASKRAW._serialized_start=149
-  _TASKRAW._serialized_end=1033
-  _TASKRAW_OUTPUT._serialized_start=993
-  _TASKRAW_OUTPUT._serialized_end=1033
-  _TASKSUMMARY._serialized_start=1036
-  _TASKSUMMARY._serialized_end=1474
-  _LISTTASKSREQUEST._serialized_start=1477
-  _LISTTASKSREQUEST._serialized_end=2567
-  _LISTTASKSREQUEST_FILTER._serialized_start=1684
-  _LISTTASKSREQUEST_FILTER._serialized_end=2078
-  _LISTTASKSREQUEST_SORT._serialized_start=2081
-  _LISTTASKSREQUEST_SORT._serialized_end=2239
-  _LISTTASKSREQUEST_ORDERBYFIELD._serialized_start=2242
-  _LISTTASKSREQUEST_ORDERBYFIELD._serialized_end=2465
-  _LISTTASKSREQUEST_ORDERDIRECTION._serialized_start=2467
-  _LISTTASKSREQUEST_ORDERDIRECTION._serialized_end=2567
-  _LISTTASKSRESPONSE._serialized_start=2569
-  _LISTTASKSRESPONSE._serialized_end=2691
-  _LISTTASKSRAWRESPONSE._serialized_start=2693
-  _LISTTASKSRAWRESPONSE._serialized_end=2814
-  _GETTASKREQUEST._serialized_start=2816
-  _GETTASKREQUEST._serialized_end=2849
-  _GETTASKRESPONSE._serialized_start=2851
-  _GETTASKRESPONSE._serialized_end=2918
-  _CANCELTASKSREQUEST._serialized_start=2920
-  _CANCELTASKSREQUEST._serialized_end=2958
-  _CANCELTASKSRESPONSE._serialized_start=2960
-  _CANCELTASKSRESPONSE._serialized_end=3036
-  _GETRESULTIDSREQUEST._serialized_start=3038
-  _GETRESULTIDSREQUEST._serialized_end=3076
-  _GETRESULTIDSRESPONSE._serialized_start=3079
-  _GETRESULTIDSRESPONSE._serialized_end=3240
-  _GETRESULTIDSRESPONSE_MAPTASKRESULT._serialized_start=3188
-  _GETRESULTIDSRESPONSE_MAPTASKRESULT._serialized_end=3240
-  _COUNTTASKSBYSTATUSREQUEST._serialized_start=3242
-  _COUNTTASKSBYSTATUSREQUEST._serialized_end=3269
-  _COUNTTASKSBYSTATUSRESPONSE._serialized_start=3271
-  _COUNTTASKSBYSTATUSRESPONSE._serialized_end=3349
-  _SUBMITTASKSREQUEST._serialized_start=3352
-  _SUBMITTASKSREQUEST._serialized_end=3682
-  _SUBMITTASKSREQUEST_TASKCREATION._serialized_start=3535
-  _SUBMITTASKSREQUEST_TASKCREATION._serialized_end=3682
-  _SUBMITTASKSRESPONSE._serialized_start=3685
-  _SUBMITTASKSRESPONSE._serialized_end=3888
-  _SUBMITTASKSRESPONSE_TASKINFO._serialized_start=3785
-  _SUBMITTASKSRESPONSE_TASKINFO._serialized_end=3888
+  _globals['_TASKRAW']._serialized_start=149
+  _globals['_TASKRAW']._serialized_end=1033
+  _globals['_TASKRAW_OUTPUT']._serialized_start=993
+  _globals['_TASKRAW_OUTPUT']._serialized_end=1033
+  _globals['_TASKSUMMARY']._serialized_start=1036
+  _globals['_TASKSUMMARY']._serialized_end=1474
+  _globals['_LISTTASKSREQUEST']._serialized_start=1477
+  _globals['_LISTTASKSREQUEST']._serialized_end=2567
+  _globals['_LISTTASKSREQUEST_FILTER']._serialized_start=1684
+  _globals['_LISTTASKSREQUEST_FILTER']._serialized_end=2078
+  _globals['_LISTTASKSREQUEST_SORT']._serialized_start=2081
+  _globals['_LISTTASKSREQUEST_SORT']._serialized_end=2239
+  _globals['_LISTTASKSREQUEST_ORDERBYFIELD']._serialized_start=2242
+  _globals['_LISTTASKSREQUEST_ORDERBYFIELD']._serialized_end=2465
+  _globals['_LISTTASKSREQUEST_ORDERDIRECTION']._serialized_start=2467
+  _globals['_LISTTASKSREQUEST_ORDERDIRECTION']._serialized_end=2567
+  _globals['_LISTTASKSRESPONSE']._serialized_start=2569
+  _globals['_LISTTASKSRESPONSE']._serialized_end=2691
+  _globals['_LISTTASKSRAWRESPONSE']._serialized_start=2693
+  _globals['_LISTTASKSRAWRESPONSE']._serialized_end=2814
+  _globals['_GETTASKREQUEST']._serialized_start=2816
+  _globals['_GETTASKREQUEST']._serialized_end=2849
+  _globals['_GETTASKRESPONSE']._serialized_start=2851
+  _globals['_GETTASKRESPONSE']._serialized_end=2918
+  _globals['_CANCELTASKSREQUEST']._serialized_start=2920
+  _globals['_CANCELTASKSREQUEST']._serialized_end=2958
+  _globals['_CANCELTASKSRESPONSE']._serialized_start=2960
+  _globals['_CANCELTASKSRESPONSE']._serialized_end=3036
+  _globals['_GETRESULTIDSREQUEST']._serialized_start=3038
+  _globals['_GETRESULTIDSREQUEST']._serialized_end=3076
+  _globals['_GETRESULTIDSRESPONSE']._serialized_start=3079
+  _globals['_GETRESULTIDSRESPONSE']._serialized_end=3240
+  _globals['_GETRESULTIDSRESPONSE_MAPTASKRESULT']._serialized_start=3188
+  _globals['_GETRESULTIDSRESPONSE_MAPTASKRESULT']._serialized_end=3240
+  _globals['_COUNTTASKSBYSTATUSREQUEST']._serialized_start=3242
+  _globals['_COUNTTASKSBYSTATUSREQUEST']._serialized_end=3269
+  _globals['_COUNTTASKSBYSTATUSRESPONSE']._serialized_start=3271
+  _globals['_COUNTTASKSBYSTATUSRESPONSE']._serialized_end=3349
+  _globals['_SUBMITTASKSREQUEST']._serialized_start=3352
+  _globals['_SUBMITTASKSREQUEST']._serialized_end=3682
+  _globals['_SUBMITTASKSREQUEST_TASKCREATION']._serialized_start=3535
+  _globals['_SUBMITTASKSREQUEST_TASKCREATION']._serialized_end=3682
+  _globals['_SUBMITTASKSRESPONSE']._serialized_start=3685
+  _globals['_SUBMITTASKSRESPONSE']._serialized_end=3888
+  _globals['_SUBMITTASKSRESPONSE_TASKINFO']._serialized_start=3785
+  _globals['_SUBMITTASKSRESPONSE_TASKINFO']._serialized_end=3888
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/tasks_common_pb2.pyi` & `armonik-3.8.2.dev349/src/armonik/protogen/common/tasks_common_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -6,252 +6,262 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class CancelTasksRequest(_message.Message):
-    __slots__ = ["task_ids"]
-    TASK_IDS_FIELD_NUMBER: _ClassVar[int]
-    task_ids: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, task_ids: _Optional[_Iterable[str]] = ...) -> None: ...
-
-class CancelTasksResponse(_message.Message):
-    __slots__ = ["tasks"]
-    TASKS_FIELD_NUMBER: _ClassVar[int]
-    tasks: _containers.RepeatedCompositeFieldContainer[TaskSummary]
-    def __init__(self, tasks: _Optional[_Iterable[_Union[TaskSummary, _Mapping]]] = ...) -> None: ...
-
-class CountTasksByStatusRequest(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
-
-class CountTasksByStatusResponse(_message.Message):
-    __slots__ = ["status"]
+class TaskRaw(_message.Message):
+    __slots__ = ["id", "session_id", "owner_pod_id", "parent_task_ids", "data_dependencies", "expected_output_ids", "retry_of_ids", "status", "status_message", "options", "created_at", "submitted_at", "started_at", "ended_at", "creation_to_end_duration", "processing_to_end_duration", "pod_ttl", "output", "pod_hostname", "received_at", "acquired_at"]
+    class Output(_message.Message):
+        __slots__ = ["success", "error"]
+        SUCCESS_FIELD_NUMBER: _ClassVar[int]
+        ERROR_FIELD_NUMBER: _ClassVar[int]
+        success: bool
+        error: str
+        def __init__(self, success: bool = ..., error: _Optional[str] = ...) -> None: ...
+    ID_FIELD_NUMBER: _ClassVar[int]
+    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+    OWNER_POD_ID_FIELD_NUMBER: _ClassVar[int]
+    PARENT_TASK_IDS_FIELD_NUMBER: _ClassVar[int]
+    DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
+    EXPECTED_OUTPUT_IDS_FIELD_NUMBER: _ClassVar[int]
+    RETRY_OF_IDS_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
-    status: _containers.RepeatedCompositeFieldContainer[_objects_pb2.StatusCount]
-    def __init__(self, status: _Optional[_Iterable[_Union[_objects_pb2.StatusCount, _Mapping]]] = ...) -> None: ...
-
-class GetResultIdsRequest(_message.Message):
-    __slots__ = ["task_id"]
-    TASK_ID_FIELD_NUMBER: _ClassVar[int]
-    task_id: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, task_id: _Optional[_Iterable[str]] = ...) -> None: ...
-
-class GetResultIdsResponse(_message.Message):
-    __slots__ = ["task_results"]
-    class MapTaskResult(_message.Message):
-        __slots__ = ["result_ids", "task_id"]
-        RESULT_IDS_FIELD_NUMBER: _ClassVar[int]
-        TASK_ID_FIELD_NUMBER: _ClassVar[int]
-        result_ids: _containers.RepeatedScalarFieldContainer[str]
-        task_id: str
-        def __init__(self, task_id: _Optional[str] = ..., result_ids: _Optional[_Iterable[str]] = ...) -> None: ...
-    TASK_RESULTS_FIELD_NUMBER: _ClassVar[int]
-    task_results: _containers.RepeatedCompositeFieldContainer[GetResultIdsResponse.MapTaskResult]
-    def __init__(self, task_results: _Optional[_Iterable[_Union[GetResultIdsResponse.MapTaskResult, _Mapping]]] = ...) -> None: ...
-
-class GetTaskRequest(_message.Message):
-    __slots__ = ["task_id"]
-    TASK_ID_FIELD_NUMBER: _ClassVar[int]
-    task_id: str
-    def __init__(self, task_id: _Optional[str] = ...) -> None: ...
-
-class GetTaskResponse(_message.Message):
-    __slots__ = ["task"]
-    TASK_FIELD_NUMBER: _ClassVar[int]
-    task: TaskRaw
-    def __init__(self, task: _Optional[_Union[TaskRaw, _Mapping]] = ...) -> None: ...
+    STATUS_MESSAGE_FIELD_NUMBER: _ClassVar[int]
+    OPTIONS_FIELD_NUMBER: _ClassVar[int]
+    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
+    SUBMITTED_AT_FIELD_NUMBER: _ClassVar[int]
+    STARTED_AT_FIELD_NUMBER: _ClassVar[int]
+    ENDED_AT_FIELD_NUMBER: _ClassVar[int]
+    CREATION_TO_END_DURATION_FIELD_NUMBER: _ClassVar[int]
+    PROCESSING_TO_END_DURATION_FIELD_NUMBER: _ClassVar[int]
+    POD_TTL_FIELD_NUMBER: _ClassVar[int]
+    OUTPUT_FIELD_NUMBER: _ClassVar[int]
+    POD_HOSTNAME_FIELD_NUMBER: _ClassVar[int]
+    RECEIVED_AT_FIELD_NUMBER: _ClassVar[int]
+    ACQUIRED_AT_FIELD_NUMBER: _ClassVar[int]
+    id: str
+    session_id: str
+    owner_pod_id: str
+    parent_task_ids: _containers.RepeatedScalarFieldContainer[str]
+    data_dependencies: _containers.RepeatedScalarFieldContainer[str]
+    expected_output_ids: _containers.RepeatedScalarFieldContainer[str]
+    retry_of_ids: _containers.RepeatedScalarFieldContainer[str]
+    status: _task_status_pb2.TaskStatus
+    status_message: str
+    options: _objects_pb2.TaskOptions
+    created_at: _timestamp_pb2.Timestamp
+    submitted_at: _timestamp_pb2.Timestamp
+    started_at: _timestamp_pb2.Timestamp
+    ended_at: _timestamp_pb2.Timestamp
+    creation_to_end_duration: _duration_pb2.Duration
+    processing_to_end_duration: _duration_pb2.Duration
+    pod_ttl: _timestamp_pb2.Timestamp
+    output: TaskRaw.Output
+    pod_hostname: str
+    received_at: _timestamp_pb2.Timestamp
+    acquired_at: _timestamp_pb2.Timestamp
+    def __init__(self, id: _Optional[str] = ..., session_id: _Optional[str] = ..., owner_pod_id: _Optional[str] = ..., parent_task_ids: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., expected_output_ids: _Optional[_Iterable[str]] = ..., retry_of_ids: _Optional[_Iterable[str]] = ..., status: _Optional[_Union[_task_status_pb2.TaskStatus, str]] = ..., status_message: _Optional[str] = ..., options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., submitted_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., ended_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., creation_to_end_duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., processing_to_end_duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., pod_ttl: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., output: _Optional[_Union[TaskRaw.Output, _Mapping]] = ..., pod_hostname: _Optional[str] = ..., received_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., acquired_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
 
-class ListTasksRawResponse(_message.Message):
-    __slots__ = ["page", "page_size", "tasks", "total"]
-    PAGE_FIELD_NUMBER: _ClassVar[int]
-    PAGE_SIZE_FIELD_NUMBER: _ClassVar[int]
-    TASKS_FIELD_NUMBER: _ClassVar[int]
-    TOTAL_FIELD_NUMBER: _ClassVar[int]
-    page: int
-    page_size: int
-    tasks: _containers.RepeatedCompositeFieldContainer[TaskRaw]
-    total: int
-    def __init__(self, tasks: _Optional[_Iterable[_Union[TaskRaw, _Mapping]]] = ..., page: _Optional[int] = ..., page_size: _Optional[int] = ..., total: _Optional[int] = ...) -> None: ...
+class TaskSummary(_message.Message):
+    __slots__ = ["id", "session_id", "options", "status", "created_at", "started_at", "ended_at", "creation_to_end_duration", "processing_to_end_duration", "error"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+    OPTIONS_FIELD_NUMBER: _ClassVar[int]
+    STATUS_FIELD_NUMBER: _ClassVar[int]
+    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
+    STARTED_AT_FIELD_NUMBER: _ClassVar[int]
+    ENDED_AT_FIELD_NUMBER: _ClassVar[int]
+    CREATION_TO_END_DURATION_FIELD_NUMBER: _ClassVar[int]
+    PROCESSING_TO_END_DURATION_FIELD_NUMBER: _ClassVar[int]
+    ERROR_FIELD_NUMBER: _ClassVar[int]
+    id: str
+    session_id: str
+    options: _objects_pb2.TaskOptions
+    status: _task_status_pb2.TaskStatus
+    created_at: _timestamp_pb2.Timestamp
+    started_at: _timestamp_pb2.Timestamp
+    ended_at: _timestamp_pb2.Timestamp
+    creation_to_end_duration: _duration_pb2.Duration
+    processing_to_end_duration: _duration_pb2.Duration
+    error: str
+    def __init__(self, id: _Optional[str] = ..., session_id: _Optional[str] = ..., options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., status: _Optional[_Union[_task_status_pb2.TaskStatus, str]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., ended_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., creation_to_end_duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., processing_to_end_duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., error: _Optional[str] = ...) -> None: ...
 
 class ListTasksRequest(_message.Message):
-    __slots__ = ["filter", "page", "page_size", "sort", "with_errors"]
+    __slots__ = ["page", "page_size", "filter", "sort", "with_errors"]
     class OrderByField(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        ORDER_BY_FIELD_UNSPECIFIED: _ClassVar[ListTasksRequest.OrderByField]
+        ORDER_BY_FIELD_TASK_ID: _ClassVar[ListTasksRequest.OrderByField]
+        ORDER_BY_FIELD_SESSION_ID: _ClassVar[ListTasksRequest.OrderByField]
+        ORDER_BY_FIELD_STATUS: _ClassVar[ListTasksRequest.OrderByField]
+        ORDER_BY_FIELD_CREATED_AT: _ClassVar[ListTasksRequest.OrderByField]
+        ORDER_BY_FIELD_STARTED_AT: _ClassVar[ListTasksRequest.OrderByField]
+        ORDER_BY_FIELD_ENDED_AT: _ClassVar[ListTasksRequest.OrderByField]
+    ORDER_BY_FIELD_UNSPECIFIED: ListTasksRequest.OrderByField
+    ORDER_BY_FIELD_TASK_ID: ListTasksRequest.OrderByField
+    ORDER_BY_FIELD_SESSION_ID: ListTasksRequest.OrderByField
+    ORDER_BY_FIELD_STATUS: ListTasksRequest.OrderByField
+    ORDER_BY_FIELD_CREATED_AT: ListTasksRequest.OrderByField
+    ORDER_BY_FIELD_STARTED_AT: ListTasksRequest.OrderByField
+    ORDER_BY_FIELD_ENDED_AT: ListTasksRequest.OrderByField
     class OrderDirection(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        ORDER_DIRECTION_UNSPECIFIED: _ClassVar[ListTasksRequest.OrderDirection]
+        ORDER_DIRECTION_ASC: _ClassVar[ListTasksRequest.OrderDirection]
+        ORDER_DIRECTION_DESC: _ClassVar[ListTasksRequest.OrderDirection]
+    ORDER_DIRECTION_UNSPECIFIED: ListTasksRequest.OrderDirection
+    ORDER_DIRECTION_ASC: ListTasksRequest.OrderDirection
+    ORDER_DIRECTION_DESC: ListTasksRequest.OrderDirection
     class Filter(_message.Message):
-        __slots__ = ["created_after", "created_before", "ended_after", "ended_before", "session_id", "started_after", "started_before", "status"]
+        __slots__ = ["session_id", "status", "created_after", "created_before", "started_after", "started_before", "ended_after", "ended_before"]
+        SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+        STATUS_FIELD_NUMBER: _ClassVar[int]
         CREATED_AFTER_FIELD_NUMBER: _ClassVar[int]
         CREATED_BEFORE_FIELD_NUMBER: _ClassVar[int]
-        ENDED_AFTER_FIELD_NUMBER: _ClassVar[int]
-        ENDED_BEFORE_FIELD_NUMBER: _ClassVar[int]
-        SESSION_ID_FIELD_NUMBER: _ClassVar[int]
         STARTED_AFTER_FIELD_NUMBER: _ClassVar[int]
         STARTED_BEFORE_FIELD_NUMBER: _ClassVar[int]
-        STATUS_FIELD_NUMBER: _ClassVar[int]
+        ENDED_AFTER_FIELD_NUMBER: _ClassVar[int]
+        ENDED_BEFORE_FIELD_NUMBER: _ClassVar[int]
+        session_id: str
+        status: _containers.RepeatedScalarFieldContainer[_task_status_pb2.TaskStatus]
         created_after: _timestamp_pb2.Timestamp
         created_before: _timestamp_pb2.Timestamp
-        ended_after: _timestamp_pb2.Timestamp
-        ended_before: _timestamp_pb2.Timestamp
-        session_id: str
         started_after: _timestamp_pb2.Timestamp
         started_before: _timestamp_pb2.Timestamp
-        status: _containers.RepeatedScalarFieldContainer[_task_status_pb2.TaskStatus]
+        ended_after: _timestamp_pb2.Timestamp
+        ended_before: _timestamp_pb2.Timestamp
         def __init__(self, session_id: _Optional[str] = ..., status: _Optional[_Iterable[_Union[_task_status_pb2.TaskStatus, str]]] = ..., created_after: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., created_before: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., started_after: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., started_before: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., ended_after: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., ended_before: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
     class Sort(_message.Message):
-        __slots__ = ["direction", "field"]
-        DIRECTION_FIELD_NUMBER: _ClassVar[int]
+        __slots__ = ["field", "direction"]
         FIELD_FIELD_NUMBER: _ClassVar[int]
-        direction: ListTasksRequest.OrderDirection
+        DIRECTION_FIELD_NUMBER: _ClassVar[int]
         field: ListTasksRequest.OrderByField
+        direction: ListTasksRequest.OrderDirection
         def __init__(self, field: _Optional[_Union[ListTasksRequest.OrderByField, str]] = ..., direction: _Optional[_Union[ListTasksRequest.OrderDirection, str]] = ...) -> None: ...
-    FILTER_FIELD_NUMBER: _ClassVar[int]
-    ORDER_BY_FIELD_CREATED_AT: ListTasksRequest.OrderByField
-    ORDER_BY_FIELD_ENDED_AT: ListTasksRequest.OrderByField
-    ORDER_BY_FIELD_SESSION_ID: ListTasksRequest.OrderByField
-    ORDER_BY_FIELD_STARTED_AT: ListTasksRequest.OrderByField
-    ORDER_BY_FIELD_STATUS: ListTasksRequest.OrderByField
-    ORDER_BY_FIELD_TASK_ID: ListTasksRequest.OrderByField
-    ORDER_BY_FIELD_UNSPECIFIED: ListTasksRequest.OrderByField
-    ORDER_DIRECTION_ASC: ListTasksRequest.OrderDirection
-    ORDER_DIRECTION_DESC: ListTasksRequest.OrderDirection
-    ORDER_DIRECTION_UNSPECIFIED: ListTasksRequest.OrderDirection
     PAGE_FIELD_NUMBER: _ClassVar[int]
     PAGE_SIZE_FIELD_NUMBER: _ClassVar[int]
+    FILTER_FIELD_NUMBER: _ClassVar[int]
     SORT_FIELD_NUMBER: _ClassVar[int]
     WITH_ERRORS_FIELD_NUMBER: _ClassVar[int]
-    filter: ListTasksRequest.Filter
     page: int
     page_size: int
+    filter: ListTasksRequest.Filter
     sort: ListTasksRequest.Sort
     with_errors: bool
     def __init__(self, page: _Optional[int] = ..., page_size: _Optional[int] = ..., filter: _Optional[_Union[ListTasksRequest.Filter, _Mapping]] = ..., sort: _Optional[_Union[ListTasksRequest.Sort, _Mapping]] = ..., with_errors: bool = ...) -> None: ...
 
 class ListTasksResponse(_message.Message):
-    __slots__ = ["page", "page_size", "tasks", "total"]
+    __slots__ = ["tasks", "page", "page_size", "total"]
+    TASKS_FIELD_NUMBER: _ClassVar[int]
     PAGE_FIELD_NUMBER: _ClassVar[int]
     PAGE_SIZE_FIELD_NUMBER: _ClassVar[int]
-    TASKS_FIELD_NUMBER: _ClassVar[int]
     TOTAL_FIELD_NUMBER: _ClassVar[int]
+    tasks: _containers.RepeatedCompositeFieldContainer[TaskSummary]
     page: int
     page_size: int
-    tasks: _containers.RepeatedCompositeFieldContainer[TaskSummary]
     total: int
     def __init__(self, tasks: _Optional[_Iterable[_Union[TaskSummary, _Mapping]]] = ..., page: _Optional[int] = ..., page_size: _Optional[int] = ..., total: _Optional[int] = ...) -> None: ...
 
+class ListTasksRawResponse(_message.Message):
+    __slots__ = ["tasks", "page", "page_size", "total"]
+    TASKS_FIELD_NUMBER: _ClassVar[int]
+    PAGE_FIELD_NUMBER: _ClassVar[int]
+    PAGE_SIZE_FIELD_NUMBER: _ClassVar[int]
+    TOTAL_FIELD_NUMBER: _ClassVar[int]
+    tasks: _containers.RepeatedCompositeFieldContainer[TaskRaw]
+    page: int
+    page_size: int
+    total: int
+    def __init__(self, tasks: _Optional[_Iterable[_Union[TaskRaw, _Mapping]]] = ..., page: _Optional[int] = ..., page_size: _Optional[int] = ..., total: _Optional[int] = ...) -> None: ...
+
+class GetTaskRequest(_message.Message):
+    __slots__ = ["task_id"]
+    TASK_ID_FIELD_NUMBER: _ClassVar[int]
+    task_id: str
+    def __init__(self, task_id: _Optional[str] = ...) -> None: ...
+
+class GetTaskResponse(_message.Message):
+    __slots__ = ["task"]
+    TASK_FIELD_NUMBER: _ClassVar[int]
+    task: TaskRaw
+    def __init__(self, task: _Optional[_Union[TaskRaw, _Mapping]] = ...) -> None: ...
+
+class CancelTasksRequest(_message.Message):
+    __slots__ = ["task_ids"]
+    TASK_IDS_FIELD_NUMBER: _ClassVar[int]
+    task_ids: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, task_ids: _Optional[_Iterable[str]] = ...) -> None: ...
+
+class CancelTasksResponse(_message.Message):
+    __slots__ = ["tasks"]
+    TASKS_FIELD_NUMBER: _ClassVar[int]
+    tasks: _containers.RepeatedCompositeFieldContainer[TaskSummary]
+    def __init__(self, tasks: _Optional[_Iterable[_Union[TaskSummary, _Mapping]]] = ...) -> None: ...
+
+class GetResultIdsRequest(_message.Message):
+    __slots__ = ["task_id"]
+    TASK_ID_FIELD_NUMBER: _ClassVar[int]
+    task_id: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, task_id: _Optional[_Iterable[str]] = ...) -> None: ...
+
+class GetResultIdsResponse(_message.Message):
+    __slots__ = ["task_results"]
+    class MapTaskResult(_message.Message):
+        __slots__ = ["task_id", "result_ids"]
+        TASK_ID_FIELD_NUMBER: _ClassVar[int]
+        RESULT_IDS_FIELD_NUMBER: _ClassVar[int]
+        task_id: str
+        result_ids: _containers.RepeatedScalarFieldContainer[str]
+        def __init__(self, task_id: _Optional[str] = ..., result_ids: _Optional[_Iterable[str]] = ...) -> None: ...
+    TASK_RESULTS_FIELD_NUMBER: _ClassVar[int]
+    task_results: _containers.RepeatedCompositeFieldContainer[GetResultIdsResponse.MapTaskResult]
+    def __init__(self, task_results: _Optional[_Iterable[_Union[GetResultIdsResponse.MapTaskResult, _Mapping]]] = ...) -> None: ...
+
+class CountTasksByStatusRequest(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
+
+class CountTasksByStatusResponse(_message.Message):
+    __slots__ = ["status"]
+    STATUS_FIELD_NUMBER: _ClassVar[int]
+    status: _containers.RepeatedCompositeFieldContainer[_objects_pb2.StatusCount]
+    def __init__(self, status: _Optional[_Iterable[_Union[_objects_pb2.StatusCount, _Mapping]]] = ...) -> None: ...
+
 class SubmitTasksRequest(_message.Message):
-    __slots__ = ["session_id", "task_creations", "task_options"]
+    __slots__ = ["session_id", "task_options", "task_creations"]
     class TaskCreation(_message.Message):
-        __slots__ = ["data_dependencies", "expected_output_keys", "payload_id", "task_options"]
-        DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
+        __slots__ = ["expected_output_keys", "data_dependencies", "payload_id", "task_options"]
         EXPECTED_OUTPUT_KEYS_FIELD_NUMBER: _ClassVar[int]
+        DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
         PAYLOAD_ID_FIELD_NUMBER: _ClassVar[int]
         TASK_OPTIONS_FIELD_NUMBER: _ClassVar[int]
-        data_dependencies: _containers.RepeatedScalarFieldContainer[str]
         expected_output_keys: _containers.RepeatedScalarFieldContainer[str]
+        data_dependencies: _containers.RepeatedScalarFieldContainer[str]
         payload_id: str
         task_options: _objects_pb2.TaskOptions
         def __init__(self, expected_output_keys: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., payload_id: _Optional[str] = ..., task_options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ...) -> None: ...
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-    TASK_CREATIONS_FIELD_NUMBER: _ClassVar[int]
     TASK_OPTIONS_FIELD_NUMBER: _ClassVar[int]
+    TASK_CREATIONS_FIELD_NUMBER: _ClassVar[int]
     session_id: str
-    task_creations: _containers.RepeatedCompositeFieldContainer[SubmitTasksRequest.TaskCreation]
     task_options: _objects_pb2.TaskOptions
+    task_creations: _containers.RepeatedCompositeFieldContainer[SubmitTasksRequest.TaskCreation]
     def __init__(self, session_id: _Optional[str] = ..., task_options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., task_creations: _Optional[_Iterable[_Union[SubmitTasksRequest.TaskCreation, _Mapping]]] = ...) -> None: ...
 
 class SubmitTasksResponse(_message.Message):
     __slots__ = ["task_infos"]
     class TaskInfo(_message.Message):
-        __slots__ = ["data_dependencies", "expected_output_ids", "payload_id", "task_id"]
-        DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
+        __slots__ = ["task_id", "expected_output_ids", "data_dependencies", "payload_id"]
+        TASK_ID_FIELD_NUMBER: _ClassVar[int]
         EXPECTED_OUTPUT_IDS_FIELD_NUMBER: _ClassVar[int]
+        DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
         PAYLOAD_ID_FIELD_NUMBER: _ClassVar[int]
-        TASK_ID_FIELD_NUMBER: _ClassVar[int]
-        data_dependencies: _containers.RepeatedScalarFieldContainer[str]
+        task_id: str
         expected_output_ids: _containers.RepeatedScalarFieldContainer[str]
+        data_dependencies: _containers.RepeatedScalarFieldContainer[str]
         payload_id: str
-        task_id: str
         def __init__(self, task_id: _Optional[str] = ..., expected_output_ids: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., payload_id: _Optional[str] = ...) -> None: ...
     TASK_INFOS_FIELD_NUMBER: _ClassVar[int]
     task_infos: _containers.RepeatedCompositeFieldContainer[SubmitTasksResponse.TaskInfo]
     def __init__(self, task_infos: _Optional[_Iterable[_Union[SubmitTasksResponse.TaskInfo, _Mapping]]] = ...) -> None: ...
-
-class TaskRaw(_message.Message):
-    __slots__ = ["acquired_at", "created_at", "creation_to_end_duration", "data_dependencies", "ended_at", "expected_output_ids", "id", "options", "output", "owner_pod_id", "parent_task_ids", "pod_hostname", "pod_ttl", "processing_to_end_duration", "received_at", "retry_of_ids", "session_id", "started_at", "status", "status_message", "submitted_at"]
-    class Output(_message.Message):
-        __slots__ = ["error", "success"]
-        ERROR_FIELD_NUMBER: _ClassVar[int]
-        SUCCESS_FIELD_NUMBER: _ClassVar[int]
-        error: str
-        success: bool
-        def __init__(self, success: bool = ..., error: _Optional[str] = ...) -> None: ...
-    ACQUIRED_AT_FIELD_NUMBER: _ClassVar[int]
-    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
-    CREATION_TO_END_DURATION_FIELD_NUMBER: _ClassVar[int]
-    DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
-    ENDED_AT_FIELD_NUMBER: _ClassVar[int]
-    EXPECTED_OUTPUT_IDS_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    OPTIONS_FIELD_NUMBER: _ClassVar[int]
-    OUTPUT_FIELD_NUMBER: _ClassVar[int]
-    OWNER_POD_ID_FIELD_NUMBER: _ClassVar[int]
-    PARENT_TASK_IDS_FIELD_NUMBER: _ClassVar[int]
-    POD_HOSTNAME_FIELD_NUMBER: _ClassVar[int]
-    POD_TTL_FIELD_NUMBER: _ClassVar[int]
-    PROCESSING_TO_END_DURATION_FIELD_NUMBER: _ClassVar[int]
-    RECEIVED_AT_FIELD_NUMBER: _ClassVar[int]
-    RETRY_OF_IDS_FIELD_NUMBER: _ClassVar[int]
-    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-    STARTED_AT_FIELD_NUMBER: _ClassVar[int]
-    STATUS_FIELD_NUMBER: _ClassVar[int]
-    STATUS_MESSAGE_FIELD_NUMBER: _ClassVar[int]
-    SUBMITTED_AT_FIELD_NUMBER: _ClassVar[int]
-    acquired_at: _timestamp_pb2.Timestamp
-    created_at: _timestamp_pb2.Timestamp
-    creation_to_end_duration: _duration_pb2.Duration
-    data_dependencies: _containers.RepeatedScalarFieldContainer[str]
-    ended_at: _timestamp_pb2.Timestamp
-    expected_output_ids: _containers.RepeatedScalarFieldContainer[str]
-    id: str
-    options: _objects_pb2.TaskOptions
-    output: TaskRaw.Output
-    owner_pod_id: str
-    parent_task_ids: _containers.RepeatedScalarFieldContainer[str]
-    pod_hostname: str
-    pod_ttl: _timestamp_pb2.Timestamp
-    processing_to_end_duration: _duration_pb2.Duration
-    received_at: _timestamp_pb2.Timestamp
-    retry_of_ids: _containers.RepeatedScalarFieldContainer[str]
-    session_id: str
-    started_at: _timestamp_pb2.Timestamp
-    status: _task_status_pb2.TaskStatus
-    status_message: str
-    submitted_at: _timestamp_pb2.Timestamp
-    def __init__(self, id: _Optional[str] = ..., session_id: _Optional[str] = ..., owner_pod_id: _Optional[str] = ..., parent_task_ids: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., expected_output_ids: _Optional[_Iterable[str]] = ..., retry_of_ids: _Optional[_Iterable[str]] = ..., status: _Optional[_Union[_task_status_pb2.TaskStatus, str]] = ..., status_message: _Optional[str] = ..., options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., submitted_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., ended_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., creation_to_end_duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., processing_to_end_duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., pod_ttl: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., output: _Optional[_Union[TaskRaw.Output, _Mapping]] = ..., pod_hostname: _Optional[str] = ..., received_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., acquired_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
-
-class TaskSummary(_message.Message):
-    __slots__ = ["created_at", "creation_to_end_duration", "ended_at", "error", "id", "options", "processing_to_end_duration", "session_id", "started_at", "status"]
-    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
-    CREATION_TO_END_DURATION_FIELD_NUMBER: _ClassVar[int]
-    ENDED_AT_FIELD_NUMBER: _ClassVar[int]
-    ERROR_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    OPTIONS_FIELD_NUMBER: _ClassVar[int]
-    PROCESSING_TO_END_DURATION_FIELD_NUMBER: _ClassVar[int]
-    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-    STARTED_AT_FIELD_NUMBER: _ClassVar[int]
-    STATUS_FIELD_NUMBER: _ClassVar[int]
-    created_at: _timestamp_pb2.Timestamp
-    creation_to_end_duration: _duration_pb2.Duration
-    ended_at: _timestamp_pb2.Timestamp
-    error: str
-    id: str
-    options: _objects_pb2.TaskOptions
-    processing_to_end_duration: _duration_pb2.Duration
-    session_id: str
-    started_at: _timestamp_pb2.Timestamp
-    status: _task_status_pb2.TaskStatus
-    def __init__(self, id: _Optional[str] = ..., session_id: _Optional[str] = ..., options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., status: _Optional[_Union[_task_status_pb2.TaskStatus, str]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., ended_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., creation_to_end_duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., processing_to_end_duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., error: _Optional[str] = ...) -> None: ...
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/worker_common_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/common/worker_common_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: worker_common.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from . import objects_pb2 as objects__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13worker_common.proto\x12\x1a\x61rmonik.api.grpc.v1.worker\x1a\robjects.proto\"\xde\x05\n\x0eProcessRequest\x12\x1b\n\x13\x63ommunication_token\x18\x01 \x01(\t\x12J\n\x07\x63ompute\x18\x02 \x01(\x0b\x32\x39.armonik.api.grpc.v1.worker.ProcessRequest.ComputeRequest\x1a\xe2\x04\n\x0e\x43omputeRequest\x12]\n\x0cinit_request\x18\x01 \x01(\x0b\x32\x45.armonik.api.grpc.v1.worker.ProcessRequest.ComputeRequest.InitRequestH\x00\x12\x31\n\x07payload\x18\x02 \x01(\x0b\x32\x1e.armonik.api.grpc.v1.DataChunkH\x00\x12W\n\tinit_data\x18\x03 \x01(\x0b\x32\x42.armonik.api.grpc.v1.worker.ProcessRequest.ComputeRequest.InitDataH\x00\x12.\n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32\x1e.armonik.api.grpc.v1.DataChunkH\x00\x1a\xf4\x01\n\x0bInitRequest\x12\x39\n\rconfiguration\x18\x01 \x01(\x0b\x32\".armonik.api.grpc.v1.Configuration\x12\x12\n\nsession_id\x18\x02 \x01(\t\x12\x0f\n\x07task_id\x18\x03 \x01(\t\x12\x36\n\x0ctask_options\x18\x04 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12\x1c\n\x14\x65xpected_output_keys\x18\x05 \x03(\t\x12/\n\x07payload\x18\x06 \x01(\x0b\x32\x1e.armonik.api.grpc.v1.DataChunk\x1a\x36\n\x08InitData\x12\r\n\x03key\x18\x01 \x01(\tH\x00\x12\x13\n\tlast_data\x18\x02 \x01(\x08H\x00\x42\x06\n\x04typeB\x06\n\x04type\"X\n\x0cProcessReply\x12\x1b\n\x13\x63ommunication_token\x18\x01 \x01(\t\x12+\n\x06output\x18\x02 \x01(\x0b\x32\x1b.armonik.api.grpc.v1.Output\"\x9a\x01\n\x10HealthCheckReply\x12J\n\x06status\x18\x01 \x01(\x0e\x32:.armonik.api.grpc.v1.worker.HealthCheckReply.ServingStatus\":\n\rServingStatus\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SERVING\x10\x01\x12\x0f\n\x0bNOT_SERVING\x10\x02\x42\x1d\xaa\x02\x1a\x41rmoniK.Api.gRPC.V1.Workerb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'worker_common_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'worker_common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\032ArmoniK.Api.gRPC.V1.Worker'
-  _PROCESSREQUEST._serialized_start=67
-  _PROCESSREQUEST._serialized_end=801
-  _PROCESSREQUEST_COMPUTEREQUEST._serialized_start=191
-  _PROCESSREQUEST_COMPUTEREQUEST._serialized_end=801
-  _PROCESSREQUEST_COMPUTEREQUEST_INITREQUEST._serialized_start=493
-  _PROCESSREQUEST_COMPUTEREQUEST_INITREQUEST._serialized_end=737
-  _PROCESSREQUEST_COMPUTEREQUEST_INITDATA._serialized_start=739
-  _PROCESSREQUEST_COMPUTEREQUEST_INITDATA._serialized_end=793
-  _PROCESSREPLY._serialized_start=803
-  _PROCESSREPLY._serialized_end=891
-  _HEALTHCHECKREPLY._serialized_start=894
-  _HEALTHCHECKREPLY._serialized_end=1048
-  _HEALTHCHECKREPLY_SERVINGSTATUS._serialized_start=990
-  _HEALTHCHECKREPLY_SERVINGSTATUS._serialized_end=1048
+  _globals['_PROCESSREQUEST']._serialized_start=67
+  _globals['_PROCESSREQUEST']._serialized_end=801
+  _globals['_PROCESSREQUEST_COMPUTEREQUEST']._serialized_start=191
+  _globals['_PROCESSREQUEST_COMPUTEREQUEST']._serialized_end=801
+  _globals['_PROCESSREQUEST_COMPUTEREQUEST_INITREQUEST']._serialized_start=493
+  _globals['_PROCESSREQUEST_COMPUTEREQUEST_INITREQUEST']._serialized_end=737
+  _globals['_PROCESSREQUEST_COMPUTEREQUEST_INITDATA']._serialized_start=739
+  _globals['_PROCESSREQUEST_COMPUTEREQUEST_INITDATA']._serialized_end=793
+  _globals['_PROCESSREPLY']._serialized_start=803
+  _globals['_PROCESSREPLY']._serialized_end=891
+  _globals['_HEALTHCHECKREPLY']._serialized_start=894
+  _globals['_HEALTHCHECKREPLY']._serialized_end=1048
+  _globals['_HEALTHCHECKREPLY_SERVINGSTATUS']._serialized_start=990
+  _globals['_HEALTHCHECKREPLY_SERVINGSTATUS']._serialized_end=1048
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/common/worker_common_pb2.pyi` & `armonik-3.8.2.dev349/src/armonik/protogen/common/worker_common_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -3,66 +3,69 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class HealthCheckReply(_message.Message):
-    __slots__ = ["status"]
-    class ServingStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    NOT_SERVING: HealthCheckReply.ServingStatus
-    SERVING: HealthCheckReply.ServingStatus
-    STATUS_FIELD_NUMBER: _ClassVar[int]
-    UNKNOWN: HealthCheckReply.ServingStatus
-    status: HealthCheckReply.ServingStatus
-    def __init__(self, status: _Optional[_Union[HealthCheckReply.ServingStatus, str]] = ...) -> None: ...
-
-class ProcessReply(_message.Message):
-    __slots__ = ["communication_token", "output"]
-    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    OUTPUT_FIELD_NUMBER: _ClassVar[int]
-    communication_token: str
-    output: _objects_pb2.Output
-    def __init__(self, communication_token: _Optional[str] = ..., output: _Optional[_Union[_objects_pb2.Output, _Mapping]] = ...) -> None: ...
-
 class ProcessRequest(_message.Message):
     __slots__ = ["communication_token", "compute"]
     class ComputeRequest(_message.Message):
-        __slots__ = ["data", "init_data", "init_request", "payload"]
-        class InitData(_message.Message):
-            __slots__ = ["key", "last_data"]
-            KEY_FIELD_NUMBER: _ClassVar[int]
-            LAST_DATA_FIELD_NUMBER: _ClassVar[int]
-            key: str
-            last_data: bool
-            def __init__(self, key: _Optional[str] = ..., last_data: bool = ...) -> None: ...
+        __slots__ = ["init_request", "payload", "init_data", "data"]
         class InitRequest(_message.Message):
-            __slots__ = ["configuration", "expected_output_keys", "payload", "session_id", "task_id", "task_options"]
+            __slots__ = ["configuration", "session_id", "task_id", "task_options", "expected_output_keys", "payload"]
             CONFIGURATION_FIELD_NUMBER: _ClassVar[int]
-            EXPECTED_OUTPUT_KEYS_FIELD_NUMBER: _ClassVar[int]
-            PAYLOAD_FIELD_NUMBER: _ClassVar[int]
             SESSION_ID_FIELD_NUMBER: _ClassVar[int]
             TASK_ID_FIELD_NUMBER: _ClassVar[int]
             TASK_OPTIONS_FIELD_NUMBER: _ClassVar[int]
+            EXPECTED_OUTPUT_KEYS_FIELD_NUMBER: _ClassVar[int]
+            PAYLOAD_FIELD_NUMBER: _ClassVar[int]
             configuration: _objects_pb2.Configuration
-            expected_output_keys: _containers.RepeatedScalarFieldContainer[str]
-            payload: _objects_pb2.DataChunk
             session_id: str
             task_id: str
             task_options: _objects_pb2.TaskOptions
+            expected_output_keys: _containers.RepeatedScalarFieldContainer[str]
+            payload: _objects_pb2.DataChunk
             def __init__(self, configuration: _Optional[_Union[_objects_pb2.Configuration, _Mapping]] = ..., session_id: _Optional[str] = ..., task_id: _Optional[str] = ..., task_options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., expected_output_keys: _Optional[_Iterable[str]] = ..., payload: _Optional[_Union[_objects_pb2.DataChunk, _Mapping]] = ...) -> None: ...
-        DATA_FIELD_NUMBER: _ClassVar[int]
-        INIT_DATA_FIELD_NUMBER: _ClassVar[int]
+        class InitData(_message.Message):
+            __slots__ = ["key", "last_data"]
+            KEY_FIELD_NUMBER: _ClassVar[int]
+            LAST_DATA_FIELD_NUMBER: _ClassVar[int]
+            key: str
+            last_data: bool
+            def __init__(self, key: _Optional[str] = ..., last_data: bool = ...) -> None: ...
         INIT_REQUEST_FIELD_NUMBER: _ClassVar[int]
         PAYLOAD_FIELD_NUMBER: _ClassVar[int]
-        data: _objects_pb2.DataChunk
-        init_data: ProcessRequest.ComputeRequest.InitData
+        INIT_DATA_FIELD_NUMBER: _ClassVar[int]
+        DATA_FIELD_NUMBER: _ClassVar[int]
         init_request: ProcessRequest.ComputeRequest.InitRequest
         payload: _objects_pb2.DataChunk
+        init_data: ProcessRequest.ComputeRequest.InitData
+        data: _objects_pb2.DataChunk
         def __init__(self, init_request: _Optional[_Union[ProcessRequest.ComputeRequest.InitRequest, _Mapping]] = ..., payload: _Optional[_Union[_objects_pb2.DataChunk, _Mapping]] = ..., init_data: _Optional[_Union[ProcessRequest.ComputeRequest.InitData, _Mapping]] = ..., data: _Optional[_Union[_objects_pb2.DataChunk, _Mapping]] = ...) -> None: ...
     COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
     COMPUTE_FIELD_NUMBER: _ClassVar[int]
     communication_token: str
     compute: ProcessRequest.ComputeRequest
     def __init__(self, communication_token: _Optional[str] = ..., compute: _Optional[_Union[ProcessRequest.ComputeRequest, _Mapping]] = ...) -> None: ...
+
+class ProcessReply(_message.Message):
+    __slots__ = ["communication_token", "output"]
+    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
+    OUTPUT_FIELD_NUMBER: _ClassVar[int]
+    communication_token: str
+    output: _objects_pb2.Output
+    def __init__(self, communication_token: _Optional[str] = ..., output: _Optional[_Union[_objects_pb2.Output, _Mapping]] = ...) -> None: ...
+
+class HealthCheckReply(_message.Message):
+    __slots__ = ["status"]
+    class ServingStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        UNKNOWN: _ClassVar[HealthCheckReply.ServingStatus]
+        SERVING: _ClassVar[HealthCheckReply.ServingStatus]
+        NOT_SERVING: _ClassVar[HealthCheckReply.ServingStatus]
+    UNKNOWN: HealthCheckReply.ServingStatus
+    SERVING: HealthCheckReply.ServingStatus
+    NOT_SERVING: HealthCheckReply.ServingStatus
+    STATUS_FIELD_NUMBER: _ClassVar[int]
+    status: HealthCheckReply.ServingStatus
+    def __init__(self, status: _Optional[_Union[HealthCheckReply.ServingStatus, str]] = ...) -> None: ...
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/worker/agent_service_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/worker/agent_service_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: agent_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ..common import agent_common_pb2 as agent__common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13\x61gent_service.proto\x12\x19\x61rmonik.api.grpc.v1.agent\x1a\x12\x61gent_common.proto2\xe7\x07\n\x05\x41gent\x12\x8c\x01\n\x15\x43reateResultsMetaData\x12\x37.armonik.api.grpc.v1.agent.CreateResultsMetaDataRequest\x1a\x38.armonik.api.grpc.v1.agent.CreateResultsMetaDataResponse\"\x00\x12t\n\rCreateResults\x12/.armonik.api.grpc.v1.agent.CreateResultsRequest\x1a\x30.armonik.api.grpc.v1.agent.CreateResultsResponse\"\x00\x12\x7f\n\x10UploadResultData\x12\x32.armonik.api.grpc.v1.agent.UploadResultDataRequest\x1a\x33.armonik.api.grpc.v1.agent.UploadResultDataResponse\"\x00(\x01\x12n\n\x0bSubmitTasks\x12-.armonik.api.grpc.v1.agent.SubmitTasksRequest\x1a..armonik.api.grpc.v1.agent.SubmitTasksResponse\"\x00\x12h\n\nCreateTask\x12,.armonik.api.grpc.v1.agent.CreateTaskRequest\x1a*.armonik.api.grpc.v1.agent.CreateTaskReply(\x01\x12\x61\n\x0fGetResourceData\x12&.armonik.api.grpc.v1.agent.DataRequest\x1a$.armonik.api.grpc.v1.agent.DataReply0\x01\x12_\n\rGetCommonData\x12&.armonik.api.grpc.v1.agent.DataRequest\x1a$.armonik.api.grpc.v1.agent.DataReply0\x01\x12_\n\rGetDirectData\x12&.armonik.api.grpc.v1.agent.DataRequest\x1a$.armonik.api.grpc.v1.agent.DataReply0\x01\x12Y\n\nSendResult\x12!.armonik.api.grpc.v1.agent.Result\x1a&.armonik.api.grpc.v1.agent.ResultReply(\x01\x42\x1c\xaa\x02\x19\x41rmoniK.Api.gRPC.V1.Agentb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'agent_service_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'agent_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\031ArmoniK.Api.gRPC.V1.Agent'
-  _AGENT._serialized_start=71
-  _AGENT._serialized_end=1070
+  _globals['_AGENT']._serialized_start=71
+  _globals['_AGENT']._serialized_end=1070
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/worker/agent_service_pb2_grpc.py` & `armonik-3.8.2.dev349/src/armonik/protogen/worker/agent_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/worker/worker_service_pb2.py` & `armonik-3.8.2.dev349/src/armonik/protogen/worker/worker_service_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: worker_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ..common import objects_pb2 as objects__pb2
 from ..common import worker_common_pb2 as worker__common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14worker_service.proto\x12\x1a\x61rmonik.api.grpc.v1.worker\x1a\robjects.proto\x1a\x13worker_common.proto2\xc4\x01\n\x06Worker\x12\x61\n\x07Process\x12*.armonik.api.grpc.v1.worker.ProcessRequest\x1a(.armonik.api.grpc.v1.worker.ProcessReply(\x01\x12W\n\x0bHealthCheck\x12\x1a.armonik.api.grpc.v1.Empty\x1a,.armonik.api.grpc.v1.worker.HealthCheckReplyB\x1d\xaa\x02\x1a\x41rmoniK.Api.gRPC.V1.Workerb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'worker_service_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'worker_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\032ArmoniK.Api.gRPC.V1.Worker'
-  _WORKER._serialized_start=89
-  _WORKER._serialized_end=285
+  _globals['_WORKER']._serialized_start=89
+  _globals['_WORKER']._serialized_end=285
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev345/src/armonik/protogen/worker/worker_service_pb2_grpc.py` & `armonik-3.8.2.dev349/src/armonik/protogen/worker/worker_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev345/src/armonik/worker/seqlogger.py` & `armonik-3.8.2.dev349/src/armonik/worker/seqlogger.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev345/src/armonik/worker/taskhandler.py` & `armonik-3.8.2.dev349/src/armonik/worker/taskhandler.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev345/src/armonik/worker/worker.py` & `armonik-3.8.2.dev349/src/armonik/worker/worker.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev345/src/armonik.egg-info/PKG-INFO` & `armonik-3.8.2.dev349/src/armonik.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armonik
-Version: 3.8.2.dev345
+Version: 3.8.2.dev349
 Summary: GRPC python binding for the ArmoniK orchestrator API
 License: Apache v2.0 LICENSE
 Project-URL: Homepage, https://github.com/aneoconsulting/ArmoniK.Api
 Project-URL: Bug Tracker, https://github.com/aneoconsulting/ArmoniK/issues
 Keywords: cloud,HTC,gRPC,ArmoniK,Aneo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `armonik-3.8.2.dev345/src/armonik.egg-info/SOURCES.txt` & `armonik-3.8.2.dev349/src/armonik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

