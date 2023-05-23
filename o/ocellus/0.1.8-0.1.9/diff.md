# Comparing `tmp/ocellus-0.1.8.tar.gz` & `tmp/ocellus-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocellus-0.1.8.tar", last modified: Thu Jun  9 15:07:53 2022, max compression
+gzip compressed data, was "ocellus-0.1.9.tar", last modified: Thu Jun  9 15:30:04 2022, max compression
```

## Comparing `ocellus-0.1.8.tar` & `ocellus-0.1.9.tar`

### file list

```diff
@@ -1,89 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:07:53.389694 ocellus-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     9669 2022-06-09 15:07:53.385693 ocellus-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7299 2022-06-09 15:07:43.000000 ocellus-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 15:07:53.389694 ocellus-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1428 2022-06-09 15:07:52.000000 ocellus-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:07:53.381693 ocellus-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:07:53.381693 ocellus-0.1.8/src/ocellus/
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:07:53.381693 ocellus-0.1.8/src/ocellus/api/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:07:53.381693 ocellus-0.1.8/src/ocellus/api/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19526 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/api/v1/ocellus_api_command_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    14141 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/api/v1/ocellus_api_command_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    10198 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/api/v1/ocellus_api_module_data_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     4793 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/api/v1/ocellus_api_module_data_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    38994 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/api/v1/ocellus_api_module_info_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    20690 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/api/v1/ocellus_api_module_info_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:07:53.381693 ocellus-0.1.8/src/ocellus/google/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:07:53.385693 ocellus-0.1.8/src/ocellus/google/api/
--rw-r--r--   0 runner    (1001) docker     (121)     1545 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/annotations_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/annotations_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4219 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/auth_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/auth_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2148 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/backend_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/backend_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2325 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/billing_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/billing_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/client_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/client_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2701 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/config_change_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/config_change_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2467 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/consumer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/consumer_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2060 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/context_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/context_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1498 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/control_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/control_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     6431 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/distribution_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/distribution_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2949 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/documentation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/documentation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1774 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/endpoint_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/endpoint_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2152 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/field_behavior_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/field_behavior_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2997 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/http_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/http_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/httpbody_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/httpbody_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/label_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/label_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1585 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/launch_stage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/launch_stage_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1776 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/log_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2406 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/logging_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/logging_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3924 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/metric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/metric_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     5204 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/monitored_resource_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/monitored_resource_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2515 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/monitoring_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/monitoring_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4510 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/quota_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/quota_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4155 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/resource_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/resource_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2521 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/routing_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/routing_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     5321 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/source_info_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/source_info_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2879 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/system_parameter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/system_parameter_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2241 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/usage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/google/api/usage_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     6285 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/ocellus_dataflow_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     4331 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/ocellus_dataflow_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     7999 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/ocellus_module_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     4753 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/ocellus_module_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    23961 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/ocellus_types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:07:43.000000 ocellus-0.1.8/src/ocellus/ocellus_types_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:07:53.381693 ocellus-0.1.8/src/ocellus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9669 2022-06-09 15:07:53.000000 ocellus-0.1.8/src/ocellus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3296 2022-06-09 15:07:53.000000 ocellus-0.1.8/src/ocellus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 15:07:53.000000 ocellus-0.1.8/src/ocellus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-06-09 15:07:53.000000 ocellus-0.1.8/src/ocellus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-09 15:07:53.000000 ocellus-0.1.8/src/ocellus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:30:04.525245 ocellus-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     9669 2022-06-09 15:30:04.525245 ocellus-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7299 2022-06-09 15:29:53.000000 ocellus-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 15:30:04.525245 ocellus-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-06-09 15:30:03.000000 ocellus-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:30:04.513245 ocellus-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:30:04.517245 ocellus-0.1.9/src/ocellus/
+-rw-r--r--   0 runner    (1001) docker     (121)      551 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:30:04.513245 ocellus-0.1.9/src/ocellus/api/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:30:04.517245 ocellus-0.1.9/src/ocellus/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19526 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_command_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14141 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_command_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10198 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_module_data_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4793 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_module_data_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38994 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_module_info_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20690 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_module_info_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:30:04.513245 ocellus-0.1.9/src/ocellus/google/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:30:04.525245 ocellus-0.1.9/src/ocellus/google/api/
+-rw-r--r--   0 runner    (1001) docker     (121)     1545 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/annotations_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4219 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/auth_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/auth_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2148 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/backend_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/backend_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2325 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/billing_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/billing_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/client_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/client_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2701 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/config_change_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/config_change_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2467 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/consumer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/consumer_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2060 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/context_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/context_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1498 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/control_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/control_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6431 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/distribution_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/distribution_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2949 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/documentation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/documentation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1774 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/endpoint_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/endpoint_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2152 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/field_behavior_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/field_behavior_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2997 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/http_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/http_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/httpbody_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/httpbody_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/label_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/label_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1585 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/launch_stage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/launch_stage_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1776 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2406 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/logging_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/logging_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3924 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/metric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/metric_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5204 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/monitored_resource_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/monitored_resource_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2515 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/monitoring_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/monitoring_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4510 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/quota_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/quota_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4155 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/resource_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/resource_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2521 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/routing_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/routing_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5321 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/source_info_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/source_info_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2879 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/system_parameter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/system_parameter_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2241 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/usage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/google/api/usage_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6285 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/ocellus_dataflow_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4331 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/ocellus_dataflow_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7999 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/ocellus_module_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4753 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/ocellus_module_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23961 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/ocellus_types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/ocellus_types_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:30:04.513245 ocellus-0.1.9/src/ocellus/protoc_gen_swagger/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:30:04.525245 ocellus-0.1.9/src/ocellus/protoc_gen_swagger/options/
+-rw-r--r--   0 runner    (1001) docker     (121)     2955 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/protoc_gen_swagger/options/annotations_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/protoc_gen_swagger/options/annotations_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24954 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/protoc_gen_swagger/options/openapiv2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 15:29:53.000000 ocellus-0.1.9/src/ocellus/protoc_gen_swagger/options/openapiv2_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:30:04.517245 ocellus-0.1.9/src/ocellus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     9669 2022-06-09 15:30:04.000000 ocellus-0.1.9/src/ocellus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3534 2022-06-09 15:30:04.000000 ocellus-0.1.9/src/ocellus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 15:30:04.000000 ocellus-0.1.9/src/ocellus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-06-09 15:30:04.000000 ocellus-0.1.9/src/ocellus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-09 15:30:04.000000 ocellus-0.1.9/src/ocellus.egg-info/top_level.txt
```

### Comparing `ocellus-0.1.8/PKG-INFO` & `ocellus-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocellus
-Version: 0.1.8
+Version: 0.1.9
 Summary: Ocellus API Python Client
 Home-page: https://docs.ocellus.io/
 Author: Byte Motion AB
 Author-email: python@bytemotion.se
 License: MIT
 Description: # ocellus-python-client
         Autogenerated python client from [byte-motion/ProtobufDefs](https://github.com/byte-motion/ProtobufDefs/)
```

### Comparing `ocellus-0.1.8/README.md` & `ocellus-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/setup.py` & `ocellus-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(CWD, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="ocellus",
-    version="0.1.8",
+    version="0.1.9",
     description="Ocellus API Python Client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://docs.ocellus.io/",
     author="Byte Motion AB",
     author_email="python@bytemotion.se",
     license="MIT",
@@ -34,15 +34,16 @@
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
     package_dir={"": "src"},
     packages=[
         'ocellus',
         'ocellus.api.v1',
-        'ocellus.google.api'
+        'ocellus.google.api',
+        'ocellus.protoc_gen_swagger.options'
     ],
     include_package_data=True,
     install_requires=[
         "grpcio == 1.43.0",
         "protobuf == 3.19.3"
     ]
 )
```

### Comparing `ocellus-0.1.8/src/ocellus/api/v1/ocellus_api_command_service_pb2.py` & `ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_command_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/api/v1/ocellus_api_command_service_pb2_grpc.py` & `ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_command_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/api/v1/ocellus_api_module_data_service_pb2.py` & `ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_module_data_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/api/v1/ocellus_api_module_data_service_pb2_grpc.py` & `ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_module_data_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/api/v1/ocellus_api_module_info_service_pb2.py` & `ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_module_info_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/api/v1/ocellus_api_module_info_service_pb2_grpc.py` & `ocellus-0.1.9/src/ocellus/api/v1/ocellus_api_module_info_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/annotations_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/auth_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/backend_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/backend_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/billing_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/billing_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/client_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/client_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/config_change_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/config_change_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/consumer_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/consumer_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/context_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/context_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/control_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/control_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/distribution_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/distribution_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/documentation_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/documentation_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/endpoint_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/endpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/field_behavior_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/field_behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/http_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/httpbody_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/httpbody_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/label_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/label_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/launch_stage_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/launch_stage_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/log_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/log_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/logging_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/logging_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/metric_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/monitored_resource_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/monitored_resource_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/monitoring_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/quota_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/quota_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/resource_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/routing_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/routing_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/service_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/service_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/source_info_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/source_info_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/system_parameter_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/system_parameter_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/google/api/usage_pb2.py` & `ocellus-0.1.9/src/ocellus/google/api/usage_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/ocellus_dataflow_service_pb2.py` & `ocellus-0.1.9/src/ocellus/ocellus_dataflow_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/ocellus_dataflow_service_pb2_grpc.py` & `ocellus-0.1.9/src/ocellus/ocellus_dataflow_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/ocellus_module_service_pb2.py` & `ocellus-0.1.9/src/ocellus/ocellus_module_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/ocellus_module_service_pb2_grpc.py` & `ocellus-0.1.9/src/ocellus/ocellus_module_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus/ocellus_types_pb2.py` & `ocellus-0.1.9/src/ocellus/ocellus_types_pb2.py`

 * *Files identical despite different names*

### Comparing `ocellus-0.1.8/src/ocellus.egg-info/PKG-INFO` & `ocellus-0.1.9/src/ocellus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocellus
-Version: 0.1.8
+Version: 0.1.9
 Summary: Ocellus API Python Client
 Home-page: https://docs.ocellus.io/
 Author: Byte Motion AB
 Author-email: python@bytemotion.se
 License: MIT
 Description: # ocellus-python-client
         Autogenerated python client from [byte-motion/ProtobufDefs](https://github.com/byte-motion/ProtobufDefs/)
```

### Comparing `ocellus-0.1.8/src/ocellus.egg-info/SOURCES.txt` & `ocellus-0.1.9/src/ocellus.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -72,8 +72,12 @@
 src/ocellus/google/api/service_pb2.py
 src/ocellus/google/api/service_pb2_grpc.py
 src/ocellus/google/api/source_info_pb2.py
 src/ocellus/google/api/source_info_pb2_grpc.py
 src/ocellus/google/api/system_parameter_pb2.py
 src/ocellus/google/api/system_parameter_pb2_grpc.py
 src/ocellus/google/api/usage_pb2.py
-src/ocellus/google/api/usage_pb2_grpc.py
+src/ocellus/google/api/usage_pb2_grpc.py
+src/ocellus/protoc_gen_swagger/options/annotations_pb2.py
+src/ocellus/protoc_gen_swagger/options/annotations_pb2_grpc.py
+src/ocellus/protoc_gen_swagger/options/openapiv2_pb2.py
+src/ocellus/protoc_gen_swagger/options/openapiv2_pb2_grpc.py
```

