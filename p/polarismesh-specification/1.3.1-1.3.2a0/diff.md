# Comparing `tmp/polarismesh_specification-1.3.1.tar.gz` & `tmp/polarismesh_specification-1.3.2a0.tar.gz`

## Comparing `polarismesh_specification-1.3.1.tar` & `polarismesh_specification-1.3.2a0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/__about__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/__init__.pyi
--rw-r--r--   0        0        0     8830 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py
--rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/config_file_pb2_grpc.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py
--rw-r--r--   0        0        0     8034 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2_grpc.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.pyi
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/__init__.pyi
--rw-r--r--   0        0        0    12836 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py
--rw-r--r--   0        0        0    21477 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2_grpc.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2_grpc.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/__init__.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/__init__.pyi
--rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/code_pb2.py
--rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/code_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/code_pb2_grpc.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/model_pb2.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/model_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/model_pb2_grpc.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/namespace_pb2.py
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/namespace_pb2_grpc.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/security/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/security/__init__.pyi
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/security/auth_pb2.py
--rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/security/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/security/auth_pb2_grpc.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/__init__.pyi
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/client_pb2.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/client_pb2_grpc.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2_grpc.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.pyi
--rw-r--r--   0        0        0    13179 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2_grpc.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/request_pb2.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/request_pb2_grpc.py
--rw-r--r--   0        0        0     7810 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/response_pb2.py
--rw-r--r--   0        0        0    13032 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/response_pb2_grpc.py
--rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/service_pb2.py
--rw-r--r--   0        0        0    11915 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/service_pb2_grpc.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/__init__.pyi
--rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py
--rw-r--r--   0        0        0    15322 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2_grpc.py
--rw-r--r--   0        0        0     9246 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py
--rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2_grpc.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/.gitignore
--rw-r--r--   0        0        0    48229 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/LICENSE.txt
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/README.md
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/__about__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/config_manage/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/config_manage/__init__.pyi
+-rw-r--r--   0        0        0     9065 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py
+-rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/config_manage/config_file_pb2_grpc.py
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py
+-rw-r--r--   0        0        0     8034 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2_grpc.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.pyi
+-rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/fault_tolerance/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/fault_tolerance/__init__.pyi
+-rw-r--r--   0        0        0    13575 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py
+-rw-r--r--   0        0        0    22438 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2_grpc.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2_grpc.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/model/__init__.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/model/__init__.pyi
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/model/code_pb2.py
+-rw-r--r--   0        0        0    11989 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/model/code_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/model/code_pb2_grpc.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/model/model_pb2.py
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/model/model_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/model/model_pb2_grpc.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/model/namespace_pb2.py
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/model/namespace_pb2_grpc.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/security/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/security/__init__.pyi
+-rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/security/auth_pb2.py
+-rw-r--r--   0        0        0    14327 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/security/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/security/auth_pb2_grpc.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/__init__.pyi
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/client_pb2.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/client_pb2_grpc.py
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2_grpc.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.pyi
+-rw-r--r--   0        0        0    13179 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2_grpc.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/request_pb2.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/request_pb2_grpc.py
+-rw-r--r--   0        0        0     8045 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/response_pb2.py
+-rw-r--r--   0        0        0    13649 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/response_pb2_grpc.py
+-rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/service_pb2.py
+-rw-r--r--   0        0        0    12096 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/service_pb2_grpc.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/traffic_manage/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/traffic_manage/__init__.pyi
+-rw-r--r--   0        0        0    10090 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py
+-rw-r--r--   0        0        0    15969 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2_grpc.py
+-rw-r--r--   0        0        0     9793 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py
+-rw-r--r--   0        0        0    14067 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2_grpc.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/.gitignore
+-rw-r--r--   0        0        0    48229 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/LICENSE.txt
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/README.md
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/pyproject.toml
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a0/PKG-INFO
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: config_file.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x63onfig_file.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\"\xa3\x06\n\x0f\x43onfigFileGroup\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0b\x63reate_time\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfileCount\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x38\n\x08user_ids\x18\n \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x08user_ids\x12:\n\tgroup_ids\x18\x0b \x03(\x0b\x32\x1c.google.protobuf.StringValueR\tgroup_ids\x12\x46\n\x0fremove_user_ids\x18\r \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x0fremove_user_ids\x12H\n\x10remove_group_ids\x18\x0e \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x10remove_group_ids\x12,\n\x08\x65\x64itable\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12+\n\x05owner\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xaf\x06\n\nConfigFile\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x66ormat\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06status\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1f\n\x04tags\x18\t \x03(\x0b\x32\x11.v1.ConfigFileTag\x12\x31\n\x0b\x63reate_time\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x32\n\x0crelease_time\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\nrelease_by\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\x0cis_encrypted\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x32\n\x0c\x65ncrypt_algo\x18\x11 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"g\n\rConfigFileTag\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xf8\x04\n\x11\x43onfigFileRelease\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfile_name\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x03md5\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07version\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x31\n\x0b\x63reate_time\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xf9\x05\n\x18\x43onfigFileReleaseHistory\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfile_name\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x66ormat\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x03md5\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04type\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06status\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1f\n\x04tags\x18\x0c \x03(\x0b\x32\x11.v1.ConfigFileTag\x12\x31\n\x0b\x63reate_time\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xbe\x03\n\x12\x43onfigFileTemplate\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x66ormat\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0b\x63reate_time\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xc2\x03\n\x14\x43lientConfigFileInfo\x12/\n\tnamespace\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfile_name\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07version\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12)\n\x03md5\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\x0cis_encrypted\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12.\n\x08\x64\x61ta_key\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\npublic_key\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xb2\x01\n\x1c\x43lientWatchConfigFileRequest\x12/\n\tclient_ip\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x32\n\x0cservice_name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x0bwatch_files\x18\x03 \x03(\x0b\x32\x18.v1.ClientConfigFileInfo\"\xa5\x01\n\x17\x43onfigFileExportRequest\x12/\n\tnamespace\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06groups\x18\x02 \x03(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05names\x18\x03 \x03(\x0b\x32\x1c.google.protobuf.StringValueB\x8e\x01\n6com.tencent.polaris.specification.api.v1.config.manageB\x0f\x43onfigFileProtoZCgithub.com/polarismesh/specification/source/go/api/v1/config_manageb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'config_file_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'config_file_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n6com.tencent.polaris.specification.api.v1.config.manageB\017ConfigFileProtoZCgithub.com/polarismesh/specification/source/go/api/v1/config_manage'
-  _CONFIGFILEGROUP._serialized_start=58
-  _CONFIGFILEGROUP._serialized_end=861
-  _CONFIGFILE._serialized_start=864
-  _CONFIGFILE._serialized_end=1679
-  _CONFIGFILETAG._serialized_start=1681
-  _CONFIGFILETAG._serialized_end=1784
-  _CONFIGFILERELEASE._serialized_start=1787
-  _CONFIGFILERELEASE._serialized_end=2419
-  _CONFIGFILERELEASEHISTORY._serialized_start=2422
-  _CONFIGFILERELEASEHISTORY._serialized_end=3183
-  _CONFIGFILETEMPLATE._serialized_start=3186
-  _CONFIGFILETEMPLATE._serialized_end=3632
-  _CLIENTCONFIGFILEINFO._serialized_start=3635
-  _CLIENTCONFIGFILEINFO._serialized_end=4085
-  _CLIENTWATCHCONFIGFILEREQUEST._serialized_start=4088
-  _CLIENTWATCHCONFIGFILEREQUEST._serialized_end=4266
-  _CONFIGFILEEXPORTREQUEST._serialized_start=4269
-  _CONFIGFILEEXPORTREQUEST._serialized_end=4434
+  _globals['_CONFIGFILEGROUP']._serialized_start=58
+  _globals['_CONFIGFILEGROUP']._serialized_end=861
+  _globals['_CONFIGFILE']._serialized_start=864
+  _globals['_CONFIGFILE']._serialized_end=1679
+  _globals['_CONFIGFILETAG']._serialized_start=1681
+  _globals['_CONFIGFILETAG']._serialized_end=1784
+  _globals['_CONFIGFILERELEASE']._serialized_start=1787
+  _globals['_CONFIGFILERELEASE']._serialized_end=2419
+  _globals['_CONFIGFILERELEASEHISTORY']._serialized_start=2422
+  _globals['_CONFIGFILERELEASEHISTORY']._serialized_end=3183
+  _globals['_CONFIGFILETEMPLATE']._serialized_start=3186
+  _globals['_CONFIGFILETEMPLATE']._serialized_end=3632
+  _globals['_CLIENTCONFIGFILEINFO']._serialized_start=3635
+  _globals['_CLIENTCONFIGFILEINFO']._serialized_end=4085
+  _globals['_CLIENTWATCHCONFIGFILEREQUEST']._serialized_start=4088
+  _globals['_CLIENTWATCHCONFIGFILEREQUEST']._serialized_end=4266
+  _globals['_CONFIGFILEEXPORTREQUEST']._serialized_start=4269
+  _globals['_CONFIGFILEEXPORTREQUEST']._serialized_end=4434
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,216 +2,216 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class ClientConfigFileInfo(_message.Message):
-    __slots__ = ["content", "data_key", "file_name", "group", "is_encrypted", "md5", "namespace", "public_key", "version"]
-    CONTENT_FIELD_NUMBER: _ClassVar[int]
-    DATA_KEY_FIELD_NUMBER: _ClassVar[int]
-    FILE_NAME_FIELD_NUMBER: _ClassVar[int]
-    GROUP_FIELD_NUMBER: _ClassVar[int]
-    IS_ENCRYPTED_FIELD_NUMBER: _ClassVar[int]
-    MD5_FIELD_NUMBER: _ClassVar[int]
+class ConfigFileGroup(_message.Message):
+    __slots__ = ["id", "name", "namespace", "comment", "create_time", "create_by", "modify_time", "modify_by", "fileCount", "user_ids", "group_ids", "remove_user_ids", "remove_group_ids", "editable", "owner"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
     NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    PUBLIC_KEY_FIELD_NUMBER: _ClassVar[int]
-    VERSION_FIELD_NUMBER: _ClassVar[int]
-    content: _wrappers_pb2.StringValue
-    data_key: _wrappers_pb2.StringValue
-    file_name: _wrappers_pb2.StringValue
-    group: _wrappers_pb2.StringValue
-    is_encrypted: _wrappers_pb2.BoolValue
-    md5: _wrappers_pb2.StringValue
+    COMMENT_FIELD_NUMBER: _ClassVar[int]
+    CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
+    CREATE_BY_FIELD_NUMBER: _ClassVar[int]
+    MODIFY_TIME_FIELD_NUMBER: _ClassVar[int]
+    MODIFY_BY_FIELD_NUMBER: _ClassVar[int]
+    FILECOUNT_FIELD_NUMBER: _ClassVar[int]
+    USER_IDS_FIELD_NUMBER: _ClassVar[int]
+    GROUP_IDS_FIELD_NUMBER: _ClassVar[int]
+    REMOVE_USER_IDS_FIELD_NUMBER: _ClassVar[int]
+    REMOVE_GROUP_IDS_FIELD_NUMBER: _ClassVar[int]
+    EDITABLE_FIELD_NUMBER: _ClassVar[int]
+    OWNER_FIELD_NUMBER: _ClassVar[int]
+    id: _wrappers_pb2.UInt64Value
+    name: _wrappers_pb2.StringValue
     namespace: _wrappers_pb2.StringValue
-    public_key: _wrappers_pb2.StringValue
-    version: _wrappers_pb2.UInt64Value
-    def __init__(self, namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., group: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., file_name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., content: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., version: _Optional[_Union[_wrappers_pb2.UInt64Value, _Mapping]] = ..., md5: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., is_encrypted: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., data_key: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., public_key: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
-
-class ClientWatchConfigFileRequest(_message.Message):
-    __slots__ = ["client_ip", "service_name", "watch_files"]
-    CLIENT_IP_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_NAME_FIELD_NUMBER: _ClassVar[int]
-    WATCH_FILES_FIELD_NUMBER: _ClassVar[int]
-    client_ip: _wrappers_pb2.StringValue
-    service_name: _wrappers_pb2.StringValue
-    watch_files: _containers.RepeatedCompositeFieldContainer[ClientConfigFileInfo]
-    def __init__(self, client_ip: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., service_name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., watch_files: _Optional[_Iterable[_Union[ClientConfigFileInfo, _Mapping]]] = ...) -> None: ...
+    comment: _wrappers_pb2.StringValue
+    create_time: _wrappers_pb2.StringValue
+    create_by: _wrappers_pb2.StringValue
+    modify_time: _wrappers_pb2.StringValue
+    modify_by: _wrappers_pb2.StringValue
+    fileCount: _wrappers_pb2.UInt64Value
+    user_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
+    group_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
+    remove_user_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
+    remove_group_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
+    editable: _wrappers_pb2.BoolValue
+    owner: _wrappers_pb2.StringValue
+    def __init__(self, id: _Optional[_Union[_wrappers_pb2.UInt64Value, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., create_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., create_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., modify_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., modify_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., fileCount: _Optional[_Union[_wrappers_pb2.UInt64Value, _Mapping]] = ..., user_ids: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ..., group_ids: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ..., remove_user_ids: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ..., remove_group_ids: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ..., editable: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., owner: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
 
 class ConfigFile(_message.Message):
-    __slots__ = ["comment", "content", "create_by", "create_time", "encrypt_algo", "format", "group", "id", "is_encrypted", "modify_by", "modify_time", "name", "namespace", "release_by", "release_time", "status", "tags"]
-    COMMENT_FIELD_NUMBER: _ClassVar[int]
-    CONTENT_FIELD_NUMBER: _ClassVar[int]
-    CREATE_BY_FIELD_NUMBER: _ClassVar[int]
-    CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
-    ENCRYPT_ALGO_FIELD_NUMBER: _ClassVar[int]
-    FORMAT_FIELD_NUMBER: _ClassVar[int]
-    GROUP_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["id", "name", "namespace", "group", "content", "format", "comment", "status", "tags", "create_time", "create_by", "modify_time", "modify_by", "release_time", "release_by", "is_encrypted", "encrypt_algo"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    IS_ENCRYPTED_FIELD_NUMBER: _ClassVar[int]
-    MODIFY_BY_FIELD_NUMBER: _ClassVar[int]
-    MODIFY_TIME_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    RELEASE_BY_FIELD_NUMBER: _ClassVar[int]
-    RELEASE_TIME_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    GROUP_FIELD_NUMBER: _ClassVar[int]
+    CONTENT_FIELD_NUMBER: _ClassVar[int]
+    FORMAT_FIELD_NUMBER: _ClassVar[int]
+    COMMENT_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     TAGS_FIELD_NUMBER: _ClassVar[int]
-    comment: _wrappers_pb2.StringValue
-    content: _wrappers_pb2.StringValue
-    create_by: _wrappers_pb2.StringValue
-    create_time: _wrappers_pb2.StringValue
-    encrypt_algo: _wrappers_pb2.StringValue
-    format: _wrappers_pb2.StringValue
-    group: _wrappers_pb2.StringValue
+    CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
+    CREATE_BY_FIELD_NUMBER: _ClassVar[int]
+    MODIFY_TIME_FIELD_NUMBER: _ClassVar[int]
+    MODIFY_BY_FIELD_NUMBER: _ClassVar[int]
+    RELEASE_TIME_FIELD_NUMBER: _ClassVar[int]
+    RELEASE_BY_FIELD_NUMBER: _ClassVar[int]
+    IS_ENCRYPTED_FIELD_NUMBER: _ClassVar[int]
+    ENCRYPT_ALGO_FIELD_NUMBER: _ClassVar[int]
     id: _wrappers_pb2.UInt64Value
-    is_encrypted: _wrappers_pb2.BoolValue
-    modify_by: _wrappers_pb2.StringValue
-    modify_time: _wrappers_pb2.StringValue
     name: _wrappers_pb2.StringValue
     namespace: _wrappers_pb2.StringValue
-    release_by: _wrappers_pb2.StringValue
-    release_time: _wrappers_pb2.StringValue
+    group: _wrappers_pb2.StringValue
+    content: _wrappers_pb2.StringValue
+    format: _wrappers_pb2.StringValue
+    comment: _wrappers_pb2.StringValue
     status: _wrappers_pb2.StringValue
     tags: _containers.RepeatedCompositeFieldContainer[ConfigFileTag]
+    create_time: _wrappers_pb2.StringValue
+    create_by: _wrappers_pb2.StringValue
+    modify_time: _wrappers_pb2.StringValue
+    modify_by: _wrappers_pb2.StringValue
+    release_time: _wrappers_pb2.StringValue
+    release_by: _wrappers_pb2.StringValue
+    is_encrypted: _wrappers_pb2.BoolValue
+    encrypt_algo: _wrappers_pb2.StringValue
     def __init__(self, id: _Optional[_Union[_wrappers_pb2.UInt64Value, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., group: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., content: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., format: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., status: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., tags: _Optional[_Iterable[_Union[ConfigFileTag, _Mapping]]] = ..., create_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., create_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., modify_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., modify_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., release_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., release_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., is_encrypted: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., encrypt_algo: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
 
-class ConfigFileExportRequest(_message.Message):
-    __slots__ = ["groups", "names", "namespace"]
-    GROUPS_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    NAMES_FIELD_NUMBER: _ClassVar[int]
-    groups: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
-    names: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
-    namespace: _wrappers_pb2.StringValue
-    def __init__(self, namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., groups: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ..., names: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ...) -> None: ...
+class ConfigFileTag(_message.Message):
+    __slots__ = ["key", "value"]
+    KEY_FIELD_NUMBER: _ClassVar[int]
+    VALUE_FIELD_NUMBER: _ClassVar[int]
+    key: _wrappers_pb2.StringValue
+    value: _wrappers_pb2.StringValue
+    def __init__(self, key: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., value: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
 
-class ConfigFileGroup(_message.Message):
-    __slots__ = ["comment", "create_by", "create_time", "editable", "fileCount", "group_ids", "id", "modify_by", "modify_time", "name", "namespace", "owner", "remove_group_ids", "remove_user_ids", "user_ids"]
-    COMMENT_FIELD_NUMBER: _ClassVar[int]
-    CREATE_BY_FIELD_NUMBER: _ClassVar[int]
-    CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
-    EDITABLE_FIELD_NUMBER: _ClassVar[int]
-    FILECOUNT_FIELD_NUMBER: _ClassVar[int]
-    GROUP_IDS_FIELD_NUMBER: _ClassVar[int]
+class ConfigFileRelease(_message.Message):
+    __slots__ = ["id", "name", "namespace", "group", "file_name", "content", "comment", "md5", "version", "create_time", "create_by", "modify_time", "modify_by"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    MODIFY_BY_FIELD_NUMBER: _ClassVar[int]
-    MODIFY_TIME_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    OWNER_FIELD_NUMBER: _ClassVar[int]
-    REMOVE_GROUP_IDS_FIELD_NUMBER: _ClassVar[int]
-    REMOVE_USER_IDS_FIELD_NUMBER: _ClassVar[int]
-    USER_IDS_FIELD_NUMBER: _ClassVar[int]
-    comment: _wrappers_pb2.StringValue
-    create_by: _wrappers_pb2.StringValue
-    create_time: _wrappers_pb2.StringValue
-    editable: _wrappers_pb2.BoolValue
-    fileCount: _wrappers_pb2.UInt64Value
-    group_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
-    id: _wrappers_pb2.UInt64Value
-    modify_by: _wrappers_pb2.StringValue
-    modify_time: _wrappers_pb2.StringValue
-    name: _wrappers_pb2.StringValue
-    namespace: _wrappers_pb2.StringValue
-    owner: _wrappers_pb2.StringValue
-    remove_group_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
-    remove_user_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
-    user_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
-    def __init__(self, id: _Optional[_Union[_wrappers_pb2.UInt64Value, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., create_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., create_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., modify_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., modify_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., fileCount: _Optional[_Union[_wrappers_pb2.UInt64Value, _Mapping]] = ..., user_ids: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ..., group_ids: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ..., remove_user_ids: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ..., remove_group_ids: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ..., editable: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., owner: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
-
-class ConfigFileRelease(_message.Message):
-    __slots__ = ["comment", "content", "create_by", "create_time", "file_name", "group", "id", "md5", "modify_by", "modify_time", "name", "namespace", "version"]
-    COMMENT_FIELD_NUMBER: _ClassVar[int]
-    CONTENT_FIELD_NUMBER: _ClassVar[int]
-    CREATE_BY_FIELD_NUMBER: _ClassVar[int]
-    CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
-    FILE_NAME_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
     GROUP_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
+    FILE_NAME_FIELD_NUMBER: _ClassVar[int]
+    CONTENT_FIELD_NUMBER: _ClassVar[int]
+    COMMENT_FIELD_NUMBER: _ClassVar[int]
     MD5_FIELD_NUMBER: _ClassVar[int]
-    MODIFY_BY_FIELD_NUMBER: _ClassVar[int]
-    MODIFY_TIME_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
-    comment: _wrappers_pb2.StringValue
-    content: _wrappers_pb2.StringValue
-    create_by: _wrappers_pb2.StringValue
-    create_time: _wrappers_pb2.StringValue
-    file_name: _wrappers_pb2.StringValue
-    group: _wrappers_pb2.StringValue
+    CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
+    CREATE_BY_FIELD_NUMBER: _ClassVar[int]
+    MODIFY_TIME_FIELD_NUMBER: _ClassVar[int]
+    MODIFY_BY_FIELD_NUMBER: _ClassVar[int]
     id: _wrappers_pb2.UInt64Value
-    md5: _wrappers_pb2.StringValue
-    modify_by: _wrappers_pb2.StringValue
-    modify_time: _wrappers_pb2.StringValue
     name: _wrappers_pb2.StringValue
     namespace: _wrappers_pb2.StringValue
+    group: _wrappers_pb2.StringValue
+    file_name: _wrappers_pb2.StringValue
+    content: _wrappers_pb2.StringValue
+    comment: _wrappers_pb2.StringValue
+    md5: _wrappers_pb2.StringValue
     version: _wrappers_pb2.UInt64Value
+    create_time: _wrappers_pb2.StringValue
+    create_by: _wrappers_pb2.StringValue
+    modify_time: _wrappers_pb2.StringValue
+    modify_by: _wrappers_pb2.StringValue
     def __init__(self, id: _Optional[_Union[_wrappers_pb2.UInt64Value, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., group: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., file_name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., content: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., md5: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., version: _Optional[_Union[_wrappers_pb2.UInt64Value, _Mapping]] = ..., create_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., create_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., modify_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., modify_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
 
 class ConfigFileReleaseHistory(_message.Message):
-    __slots__ = ["comment", "content", "create_by", "create_time", "file_name", "format", "group", "id", "md5", "modify_by", "modify_time", "name", "namespace", "status", "tags", "type"]
-    COMMENT_FIELD_NUMBER: _ClassVar[int]
-    CONTENT_FIELD_NUMBER: _ClassVar[int]
-    CREATE_BY_FIELD_NUMBER: _ClassVar[int]
-    CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["id", "name", "namespace", "group", "file_name", "content", "format", "comment", "md5", "type", "status", "tags", "create_time", "create_by", "modify_time", "modify_by"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    GROUP_FIELD_NUMBER: _ClassVar[int]
     FILE_NAME_FIELD_NUMBER: _ClassVar[int]
+    CONTENT_FIELD_NUMBER: _ClassVar[int]
     FORMAT_FIELD_NUMBER: _ClassVar[int]
-    GROUP_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
+    COMMENT_FIELD_NUMBER: _ClassVar[int]
     MD5_FIELD_NUMBER: _ClassVar[int]
-    MODIFY_BY_FIELD_NUMBER: _ClassVar[int]
-    MODIFY_TIME_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     TAGS_FIELD_NUMBER: _ClassVar[int]
-    TYPE_FIELD_NUMBER: _ClassVar[int]
-    comment: _wrappers_pb2.StringValue
-    content: _wrappers_pb2.StringValue
-    create_by: _wrappers_pb2.StringValue
-    create_time: _wrappers_pb2.StringValue
-    file_name: _wrappers_pb2.StringValue
-    format: _wrappers_pb2.StringValue
-    group: _wrappers_pb2.StringValue
+    CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
+    CREATE_BY_FIELD_NUMBER: _ClassVar[int]
+    MODIFY_TIME_FIELD_NUMBER: _ClassVar[int]
+    MODIFY_BY_FIELD_NUMBER: _ClassVar[int]
     id: _wrappers_pb2.UInt64Value
-    md5: _wrappers_pb2.StringValue
-    modify_by: _wrappers_pb2.StringValue
-    modify_time: _wrappers_pb2.StringValue
     name: _wrappers_pb2.StringValue
     namespace: _wrappers_pb2.StringValue
+    group: _wrappers_pb2.StringValue
+    file_name: _wrappers_pb2.StringValue
+    content: _wrappers_pb2.StringValue
+    format: _wrappers_pb2.StringValue
+    comment: _wrappers_pb2.StringValue
+    md5: _wrappers_pb2.StringValue
+    type: _wrappers_pb2.StringValue
     status: _wrappers_pb2.StringValue
     tags: _containers.RepeatedCompositeFieldContainer[ConfigFileTag]
-    type: _wrappers_pb2.StringValue
+    create_time: _wrappers_pb2.StringValue
+    create_by: _wrappers_pb2.StringValue
+    modify_time: _wrappers_pb2.StringValue
+    modify_by: _wrappers_pb2.StringValue
     def __init__(self, id: _Optional[_Union[_wrappers_pb2.UInt64Value, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., group: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., file_name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., content: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., format: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., md5: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., type: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., status: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., tags: _Optional[_Iterable[_Union[ConfigFileTag, _Mapping]]] = ..., create_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., create_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., modify_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., modify_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
 
-class ConfigFileTag(_message.Message):
-    __slots__ = ["key", "value"]
-    KEY_FIELD_NUMBER: _ClassVar[int]
-    VALUE_FIELD_NUMBER: _ClassVar[int]
-    key: _wrappers_pb2.StringValue
-    value: _wrappers_pb2.StringValue
-    def __init__(self, key: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., value: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
-
 class ConfigFileTemplate(_message.Message):
-    __slots__ = ["comment", "content", "create_by", "create_time", "format", "id", "modify_by", "modify_time", "name"]
-    COMMENT_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["id", "name", "content", "format", "comment", "create_time", "create_by", "modify_time", "modify_by"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
     CONTENT_FIELD_NUMBER: _ClassVar[int]
-    CREATE_BY_FIELD_NUMBER: _ClassVar[int]
-    CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
     FORMAT_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    MODIFY_BY_FIELD_NUMBER: _ClassVar[int]
+    COMMENT_FIELD_NUMBER: _ClassVar[int]
+    CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
+    CREATE_BY_FIELD_NUMBER: _ClassVar[int]
     MODIFY_TIME_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    comment: _wrappers_pb2.StringValue
+    MODIFY_BY_FIELD_NUMBER: _ClassVar[int]
+    id: _wrappers_pb2.UInt64Value
+    name: _wrappers_pb2.StringValue
     content: _wrappers_pb2.StringValue
-    create_by: _wrappers_pb2.StringValue
-    create_time: _wrappers_pb2.StringValue
     format: _wrappers_pb2.StringValue
-    id: _wrappers_pb2.UInt64Value
-    modify_by: _wrappers_pb2.StringValue
+    comment: _wrappers_pb2.StringValue
+    create_time: _wrappers_pb2.StringValue
+    create_by: _wrappers_pb2.StringValue
     modify_time: _wrappers_pb2.StringValue
-    name: _wrappers_pb2.StringValue
+    modify_by: _wrappers_pb2.StringValue
     def __init__(self, id: _Optional[_Union[_wrappers_pb2.UInt64Value, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., content: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., format: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., create_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., create_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., modify_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., modify_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
+
+class ClientConfigFileInfo(_message.Message):
+    __slots__ = ["namespace", "group", "file_name", "content", "version", "md5", "is_encrypted", "data_key", "public_key"]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    GROUP_FIELD_NUMBER: _ClassVar[int]
+    FILE_NAME_FIELD_NUMBER: _ClassVar[int]
+    CONTENT_FIELD_NUMBER: _ClassVar[int]
+    VERSION_FIELD_NUMBER: _ClassVar[int]
+    MD5_FIELD_NUMBER: _ClassVar[int]
+    IS_ENCRYPTED_FIELD_NUMBER: _ClassVar[int]
+    DATA_KEY_FIELD_NUMBER: _ClassVar[int]
+    PUBLIC_KEY_FIELD_NUMBER: _ClassVar[int]
+    namespace: _wrappers_pb2.StringValue
+    group: _wrappers_pb2.StringValue
+    file_name: _wrappers_pb2.StringValue
+    content: _wrappers_pb2.StringValue
+    version: _wrappers_pb2.UInt64Value
+    md5: _wrappers_pb2.StringValue
+    is_encrypted: _wrappers_pb2.BoolValue
+    data_key: _wrappers_pb2.StringValue
+    public_key: _wrappers_pb2.StringValue
+    def __init__(self, namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., group: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., file_name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., content: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., version: _Optional[_Union[_wrappers_pb2.UInt64Value, _Mapping]] = ..., md5: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., is_encrypted: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., data_key: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., public_key: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
+
+class ClientWatchConfigFileRequest(_message.Message):
+    __slots__ = ["client_ip", "service_name", "watch_files"]
+    CLIENT_IP_FIELD_NUMBER: _ClassVar[int]
+    SERVICE_NAME_FIELD_NUMBER: _ClassVar[int]
+    WATCH_FILES_FIELD_NUMBER: _ClassVar[int]
+    client_ip: _wrappers_pb2.StringValue
+    service_name: _wrappers_pb2.StringValue
+    watch_files: _containers.RepeatedCompositeFieldContainer[ClientConfigFileInfo]
+    def __init__(self, client_ip: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., service_name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., watch_files: _Optional[_Iterable[_Union[ClientConfigFileInfo, _Mapping]]] = ...) -> None: ...
+
+class ConfigFileExportRequest(_message.Message):
+    __slots__ = ["namespace", "groups", "names"]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    GROUPS_FIELD_NUMBER: _ClassVar[int]
+    NAMES_FIELD_NUMBER: _ClassVar[int]
+    namespace: _wrappers_pb2.StringValue
+    groups: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
+    names: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
+    def __init__(self, namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., groups: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ..., names: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ...) -> None: ...
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: config_file_response.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from ..config_manage import config_file_pb2 as config__file__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x63onfig_file_response.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x11\x63onfig_file.proto\"n\n\x14\x43onfigSimpleResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xe0\x02\n\x0e\x43onfigResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x0f\x63onfigFileGroup\x18\x03 \x01(\x0b\x32\x13.v1.ConfigFileGroup\x12\"\n\nconfigFile\x18\x04 \x01(\x0b\x32\x0e.v1.ConfigFile\x12\x30\n\x11\x63onfigFileRelease\x18\x05 \x01(\x0b\x32\x15.v1.ConfigFileRelease\x12>\n\x18\x63onfigFileReleaseHistory\x18\x06 \x01(\x0b\x32\x1c.v1.ConfigFileReleaseHistory\x12\x32\n\x12\x63onfigFileTemplate\x18\x07 \x01(\x0b\x32\x16.v1.ConfigFileTemplate\"\xc6\x01\n\x18\x43onfigBatchWriteResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05total\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12%\n\tresponses\x18\x04 \x03(\x0b\x32\x12.v1.ConfigResponse\"\x9d\x03\n\x18\x43onfigBatchQueryResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05total\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12-\n\x10\x63onfigFileGroups\x18\x04 \x03(\x0b\x32\x13.v1.ConfigFileGroup\x12#\n\x0b\x63onfigFiles\x18\x05 \x03(\x0b\x32\x0e.v1.ConfigFile\x12\x31\n\x12\x63onfigFileReleases\x18\x06 \x03(\x0b\x32\x15.v1.ConfigFileRelease\x12@\n\x1a\x63onfigFileReleaseHistories\x18\x07 \x03(\x0b\x32\x1c.v1.ConfigFileReleaseHistory\x12\x33\n\x13\x63onfigFileTemplates\x18\x08 \x03(\x0b\x32\x16.v1.ConfigFileTemplate\"\x9c\x01\n\x14\x43onfigClientResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\nconfigFile\x18\x03 \x01(\x0b\x32\x18.v1.ClientConfigFileInfo\"\xf0\x01\n\x14\x43onfigImportResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x11\x63reateConfigFiles\x18\x03 \x03(\x0b\x32\x0e.v1.ConfigFile\x12\'\n\x0fskipConfigFiles\x18\x04 \x03(\x0b\x32\x0e.v1.ConfigFile\x12,\n\x14overwriteConfigFiles\x18\x05 \x03(\x0b\x32\x0e.v1.ConfigFile\"\x99\x01\n\x14\x43onfigExportResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.BytesValue\"\xaa\x01\n\x1e\x43onfigEncryptAlgorithmResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\nalgorithms\x18\x03 \x03(\x0b\x32\x1c.google.protobuf.StringValueB\x96\x01\n6com.tencent.polaris.specification.api.v1.config.manageB\x17\x43onfigFileResponseProtoZCgithub.com/polarismesh/specification/source/go/api/v1/config_manageb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'config_file_response_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'config_file_response_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n6com.tencent.polaris.specification.api.v1.config.manageB\027ConfigFileResponseProtoZCgithub.com/polarismesh/specification/source/go/api/v1/config_manage'
-  _CONFIGSIMPLERESPONSE._serialized_start=85
-  _CONFIGSIMPLERESPONSE._serialized_end=195
-  _CONFIGRESPONSE._serialized_start=198
-  _CONFIGRESPONSE._serialized_end=550
-  _CONFIGBATCHWRITERESPONSE._serialized_start=553
-  _CONFIGBATCHWRITERESPONSE._serialized_end=751
-  _CONFIGBATCHQUERYRESPONSE._serialized_start=754
-  _CONFIGBATCHQUERYRESPONSE._serialized_end=1167
-  _CONFIGCLIENTRESPONSE._serialized_start=1170
-  _CONFIGCLIENTRESPONSE._serialized_end=1326
-  _CONFIGIMPORTRESPONSE._serialized_start=1329
-  _CONFIGIMPORTRESPONSE._serialized_end=1569
-  _CONFIGEXPORTRESPONSE._serialized_start=1572
-  _CONFIGEXPORTRESPONSE._serialized_end=1725
-  _CONFIGENCRYPTALGORITHMRESPONSE._serialized_start=1728
-  _CONFIGENCRYPTALGORITHMRESPONSE._serialized_end=1898
+  _globals['_CONFIGSIMPLERESPONSE']._serialized_start=85
+  _globals['_CONFIGSIMPLERESPONSE']._serialized_end=195
+  _globals['_CONFIGRESPONSE']._serialized_start=198
+  _globals['_CONFIGRESPONSE']._serialized_end=550
+  _globals['_CONFIGBATCHWRITERESPONSE']._serialized_start=553
+  _globals['_CONFIGBATCHWRITERESPONSE']._serialized_end=751
+  _globals['_CONFIGBATCHQUERYRESPONSE']._serialized_start=754
+  _globals['_CONFIGBATCHQUERYRESPONSE']._serialized_end=1167
+  _globals['_CONFIGCLIENTRESPONSE']._serialized_start=1170
+  _globals['_CONFIGCLIENTRESPONSE']._serialized_end=1326
+  _globals['_CONFIGIMPORTRESPONSE']._serialized_start=1329
+  _globals['_CONFIGIMPORTRESPONSE']._serialized_end=1569
+  _globals['_CONFIGEXPORTRESPONSE']._serialized_start=1572
+  _globals['_CONFIGEXPORTRESPONSE']._serialized_end=1725
+  _globals['_CONFIGENCRYPTALGORITHMRESPONSE']._serialized_start=1728
+  _globals['_CONFIGENCRYPTALGORITHMRESPONSE']._serialized_end=1898
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -3,108 +3,108 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class ConfigBatchQueryResponse(_message.Message):
-    __slots__ = ["code", "configFileGroups", "configFileReleaseHistories", "configFileReleases", "configFileTemplates", "configFiles", "info", "total"]
+class ConfigSimpleResponse(_message.Message):
+    __slots__ = ["code", "info"]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    CONFIGFILEGROUPS_FIELD_NUMBER: _ClassVar[int]
-    CONFIGFILERELEASEHISTORIES_FIELD_NUMBER: _ClassVar[int]
-    CONFIGFILERELEASES_FIELD_NUMBER: _ClassVar[int]
-    CONFIGFILES_FIELD_NUMBER: _ClassVar[int]
-    CONFIGFILETEMPLATES_FIELD_NUMBER: _ClassVar[int]
     INFO_FIELD_NUMBER: _ClassVar[int]
-    TOTAL_FIELD_NUMBER: _ClassVar[int]
     code: _wrappers_pb2.UInt32Value
-    configFileGroups: _containers.RepeatedCompositeFieldContainer[_config_file_pb2.ConfigFileGroup]
-    configFileReleaseHistories: _containers.RepeatedCompositeFieldContainer[_config_file_pb2.ConfigFileReleaseHistory]
-    configFileReleases: _containers.RepeatedCompositeFieldContainer[_config_file_pb2.ConfigFileRelease]
-    configFileTemplates: _containers.RepeatedCompositeFieldContainer[_config_file_pb2.ConfigFileTemplate]
-    configFiles: _containers.RepeatedCompositeFieldContainer[_config_file_pb2.ConfigFile]
     info: _wrappers_pb2.StringValue
-    total: _wrappers_pb2.UInt32Value
-    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., total: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., configFileGroups: _Optional[_Iterable[_Union[_config_file_pb2.ConfigFileGroup, _Mapping]]] = ..., configFiles: _Optional[_Iterable[_Union[_config_file_pb2.ConfigFile, _Mapping]]] = ..., configFileReleases: _Optional[_Iterable[_Union[_config_file_pb2.ConfigFileRelease, _Mapping]]] = ..., configFileReleaseHistories: _Optional[_Iterable[_Union[_config_file_pb2.ConfigFileReleaseHistory, _Mapping]]] = ..., configFileTemplates: _Optional[_Iterable[_Union[_config_file_pb2.ConfigFileTemplate, _Mapping]]] = ...) -> None: ...
+    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
 
-class ConfigBatchWriteResponse(_message.Message):
-    __slots__ = ["code", "info", "responses", "total"]
+class ConfigResponse(_message.Message):
+    __slots__ = ["code", "info", "configFileGroup", "configFile", "configFileRelease", "configFileReleaseHistory", "configFileTemplate"]
     CODE_FIELD_NUMBER: _ClassVar[int]
     INFO_FIELD_NUMBER: _ClassVar[int]
-    RESPONSES_FIELD_NUMBER: _ClassVar[int]
-    TOTAL_FIELD_NUMBER: _ClassVar[int]
+    CONFIGFILEGROUP_FIELD_NUMBER: _ClassVar[int]
+    CONFIGFILE_FIELD_NUMBER: _ClassVar[int]
+    CONFIGFILERELEASE_FIELD_NUMBER: _ClassVar[int]
+    CONFIGFILERELEASEHISTORY_FIELD_NUMBER: _ClassVar[int]
+    CONFIGFILETEMPLATE_FIELD_NUMBER: _ClassVar[int]
     code: _wrappers_pb2.UInt32Value
     info: _wrappers_pb2.StringValue
-    responses: _containers.RepeatedCompositeFieldContainer[ConfigResponse]
-    total: _wrappers_pb2.UInt32Value
-    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., total: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., responses: _Optional[_Iterable[_Union[ConfigResponse, _Mapping]]] = ...) -> None: ...
+    configFileGroup: _config_file_pb2.ConfigFileGroup
+    configFile: _config_file_pb2.ConfigFile
+    configFileRelease: _config_file_pb2.ConfigFileRelease
+    configFileReleaseHistory: _config_file_pb2.ConfigFileReleaseHistory
+    configFileTemplate: _config_file_pb2.ConfigFileTemplate
+    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., configFileGroup: _Optional[_Union[_config_file_pb2.ConfigFileGroup, _Mapping]] = ..., configFile: _Optional[_Union[_config_file_pb2.ConfigFile, _Mapping]] = ..., configFileRelease: _Optional[_Union[_config_file_pb2.ConfigFileRelease, _Mapping]] = ..., configFileReleaseHistory: _Optional[_Union[_config_file_pb2.ConfigFileReleaseHistory, _Mapping]] = ..., configFileTemplate: _Optional[_Union[_config_file_pb2.ConfigFileTemplate, _Mapping]] = ...) -> None: ...
 
-class ConfigClientResponse(_message.Message):
-    __slots__ = ["code", "configFile", "info"]
+class ConfigBatchWriteResponse(_message.Message):
+    __slots__ = ["code", "info", "total", "responses"]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    CONFIGFILE_FIELD_NUMBER: _ClassVar[int]
     INFO_FIELD_NUMBER: _ClassVar[int]
+    TOTAL_FIELD_NUMBER: _ClassVar[int]
+    RESPONSES_FIELD_NUMBER: _ClassVar[int]
     code: _wrappers_pb2.UInt32Value
-    configFile: _config_file_pb2.ClientConfigFileInfo
     info: _wrappers_pb2.StringValue
-    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., configFile: _Optional[_Union[_config_file_pb2.ClientConfigFileInfo, _Mapping]] = ...) -> None: ...
+    total: _wrappers_pb2.UInt32Value
+    responses: _containers.RepeatedCompositeFieldContainer[ConfigResponse]
+    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., total: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., responses: _Optional[_Iterable[_Union[ConfigResponse, _Mapping]]] = ...) -> None: ...
 
-class ConfigEncryptAlgorithmResponse(_message.Message):
-    __slots__ = ["algorithms", "code", "info"]
-    ALGORITHMS_FIELD_NUMBER: _ClassVar[int]
+class ConfigBatchQueryResponse(_message.Message):
+    __slots__ = ["code", "info", "total", "configFileGroups", "configFiles", "configFileReleases", "configFileReleaseHistories", "configFileTemplates"]
     CODE_FIELD_NUMBER: _ClassVar[int]
     INFO_FIELD_NUMBER: _ClassVar[int]
-    algorithms: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
+    TOTAL_FIELD_NUMBER: _ClassVar[int]
+    CONFIGFILEGROUPS_FIELD_NUMBER: _ClassVar[int]
+    CONFIGFILES_FIELD_NUMBER: _ClassVar[int]
+    CONFIGFILERELEASES_FIELD_NUMBER: _ClassVar[int]
+    CONFIGFILERELEASEHISTORIES_FIELD_NUMBER: _ClassVar[int]
+    CONFIGFILETEMPLATES_FIELD_NUMBER: _ClassVar[int]
     code: _wrappers_pb2.UInt32Value
     info: _wrappers_pb2.StringValue
-    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., algorithms: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ...) -> None: ...
+    total: _wrappers_pb2.UInt32Value
+    configFileGroups: _containers.RepeatedCompositeFieldContainer[_config_file_pb2.ConfigFileGroup]
+    configFiles: _containers.RepeatedCompositeFieldContainer[_config_file_pb2.ConfigFile]
+    configFileReleases: _containers.RepeatedCompositeFieldContainer[_config_file_pb2.ConfigFileRelease]
+    configFileReleaseHistories: _containers.RepeatedCompositeFieldContainer[_config_file_pb2.ConfigFileReleaseHistory]
+    configFileTemplates: _containers.RepeatedCompositeFieldContainer[_config_file_pb2.ConfigFileTemplate]
+    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., total: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., configFileGroups: _Optional[_Iterable[_Union[_config_file_pb2.ConfigFileGroup, _Mapping]]] = ..., configFiles: _Optional[_Iterable[_Union[_config_file_pb2.ConfigFile, _Mapping]]] = ..., configFileReleases: _Optional[_Iterable[_Union[_config_file_pb2.ConfigFileRelease, _Mapping]]] = ..., configFileReleaseHistories: _Optional[_Iterable[_Union[_config_file_pb2.ConfigFileReleaseHistory, _Mapping]]] = ..., configFileTemplates: _Optional[_Iterable[_Union[_config_file_pb2.ConfigFileTemplate, _Mapping]]] = ...) -> None: ...
 
-class ConfigExportResponse(_message.Message):
-    __slots__ = ["code", "data", "info"]
+class ConfigClientResponse(_message.Message):
+    __slots__ = ["code", "info", "configFile"]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    DATA_FIELD_NUMBER: _ClassVar[int]
     INFO_FIELD_NUMBER: _ClassVar[int]
+    CONFIGFILE_FIELD_NUMBER: _ClassVar[int]
     code: _wrappers_pb2.UInt32Value
-    data: _wrappers_pb2.BytesValue
     info: _wrappers_pb2.StringValue
-    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., data: _Optional[_Union[_wrappers_pb2.BytesValue, _Mapping]] = ...) -> None: ...
+    configFile: _config_file_pb2.ClientConfigFileInfo
+    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., configFile: _Optional[_Union[_config_file_pb2.ClientConfigFileInfo, _Mapping]] = ...) -> None: ...
 
 class ConfigImportResponse(_message.Message):
-    __slots__ = ["code", "createConfigFiles", "info", "overwriteConfigFiles", "skipConfigFiles"]
+    __slots__ = ["code", "info", "createConfigFiles", "skipConfigFiles", "overwriteConfigFiles"]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    CREATECONFIGFILES_FIELD_NUMBER: _ClassVar[int]
     INFO_FIELD_NUMBER: _ClassVar[int]
-    OVERWRITECONFIGFILES_FIELD_NUMBER: _ClassVar[int]
+    CREATECONFIGFILES_FIELD_NUMBER: _ClassVar[int]
     SKIPCONFIGFILES_FIELD_NUMBER: _ClassVar[int]
+    OVERWRITECONFIGFILES_FIELD_NUMBER: _ClassVar[int]
     code: _wrappers_pb2.UInt32Value
-    createConfigFiles: _containers.RepeatedCompositeFieldContainer[_config_file_pb2.ConfigFile]
     info: _wrappers_pb2.StringValue
-    overwriteConfigFiles: _containers.RepeatedCompositeFieldContainer[_config_file_pb2.ConfigFile]
+    createConfigFiles: _containers.RepeatedCompositeFieldContainer[_config_file_pb2.ConfigFile]
     skipConfigFiles: _containers.RepeatedCompositeFieldContainer[_config_file_pb2.ConfigFile]
+    overwriteConfigFiles: _containers.RepeatedCompositeFieldContainer[_config_file_pb2.ConfigFile]
     def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., createConfigFiles: _Optional[_Iterable[_Union[_config_file_pb2.ConfigFile, _Mapping]]] = ..., skipConfigFiles: _Optional[_Iterable[_Union[_config_file_pb2.ConfigFile, _Mapping]]] = ..., overwriteConfigFiles: _Optional[_Iterable[_Union[_config_file_pb2.ConfigFile, _Mapping]]] = ...) -> None: ...
 
-class ConfigResponse(_message.Message):
-    __slots__ = ["code", "configFile", "configFileGroup", "configFileRelease", "configFileReleaseHistory", "configFileTemplate", "info"]
+class ConfigExportResponse(_message.Message):
+    __slots__ = ["code", "info", "data"]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    CONFIGFILEGROUP_FIELD_NUMBER: _ClassVar[int]
-    CONFIGFILERELEASEHISTORY_FIELD_NUMBER: _ClassVar[int]
-    CONFIGFILERELEASE_FIELD_NUMBER: _ClassVar[int]
-    CONFIGFILETEMPLATE_FIELD_NUMBER: _ClassVar[int]
-    CONFIGFILE_FIELD_NUMBER: _ClassVar[int]
     INFO_FIELD_NUMBER: _ClassVar[int]
+    DATA_FIELD_NUMBER: _ClassVar[int]
     code: _wrappers_pb2.UInt32Value
-    configFile: _config_file_pb2.ConfigFile
-    configFileGroup: _config_file_pb2.ConfigFileGroup
-    configFileRelease: _config_file_pb2.ConfigFileRelease
-    configFileReleaseHistory: _config_file_pb2.ConfigFileReleaseHistory
-    configFileTemplate: _config_file_pb2.ConfigFileTemplate
     info: _wrappers_pb2.StringValue
-    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., configFileGroup: _Optional[_Union[_config_file_pb2.ConfigFileGroup, _Mapping]] = ..., configFile: _Optional[_Union[_config_file_pb2.ConfigFile, _Mapping]] = ..., configFileRelease: _Optional[_Union[_config_file_pb2.ConfigFileRelease, _Mapping]] = ..., configFileReleaseHistory: _Optional[_Union[_config_file_pb2.ConfigFileReleaseHistory, _Mapping]] = ..., configFileTemplate: _Optional[_Union[_config_file_pb2.ConfigFileTemplate, _Mapping]] = ...) -> None: ...
+    data: _wrappers_pb2.BytesValue
+    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., data: _Optional[_Union[_wrappers_pb2.BytesValue, _Mapping]] = ...) -> None: ...
 
-class ConfigSimpleResponse(_message.Message):
-    __slots__ = ["code", "info"]
+class ConfigEncryptAlgorithmResponse(_message.Message):
+    __slots__ = ["code", "info", "algorithms"]
     CODE_FIELD_NUMBER: _ClassVar[int]
     INFO_FIELD_NUMBER: _ClassVar[int]
+    ALGORITHMS_FIELD_NUMBER: _ClassVar[int]
     code: _wrappers_pb2.UInt32Value
     info: _wrappers_pb2.StringValue
-    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
+    algorithms: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
+    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., algorithms: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ...) -> None: ...
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: grpc_config_api.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ..config_manage import config_file_pb2 as config__file__pb2
 from ..config_manage import config_file_response_pb2 as config__file__response__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15grpc_config_api.proto\x12\x02v1\x1a\x11\x63onfig_file.proto\x1a\x1a\x63onfig_file_response.proto2\xac\x01\n\x11PolarisConfigGRPC\x12\x45\n\rGetConfigFile\x12\x18.v1.ClientConfigFileInfo\x1a\x18.v1.ConfigClientResponse\"\x00\x12P\n\x10WatchConfigFiles\x12 .v1.ClientWatchConfigFileRequest\x1a\x18.v1.ConfigClientResponse\"\x00\x42\x97\x01\n6com.tencent.polaris.specification.api.v1.config.manageB\x18PolarisConfigGRPCServiceZCgithub.com/polarismesh/specification/source/go/api/v1/config_manageb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15grpc_config_api.proto\x12\x02v1\x1a\x11\x63onfig_file.proto\x1a\x1a\x63onfig_file_response.proto2\x8b\x03\n\x11PolarisConfigGRPC\x12\x45\n\rGetConfigFile\x12\x18.v1.ClientConfigFileInfo\x1a\x18.v1.ConfigClientResponse\"\x00\x12H\n\x10\x43reateConfigFile\x12\x18.v1.ClientConfigFileInfo\x1a\x18.v1.ConfigClientResponse\"\x00\x12H\n\x10UpdateConfigFile\x12\x18.v1.ClientConfigFileInfo\x1a\x18.v1.ConfigClientResponse\"\x00\x12I\n\x11PublishConfigFile\x12\x18.v1.ClientConfigFileInfo\x1a\x18.v1.ConfigClientResponse\"\x00\x12P\n\x10WatchConfigFiles\x12 .v1.ClientWatchConfigFileRequest\x1a\x18.v1.ConfigClientResponse\"\x00\x42\x97\x01\n6com.tencent.polaris.specification.api.v1.config.manageB\x18PolarisConfigGRPCServiceZCgithub.com/polarismesh/specification/source/go/api/v1/config_manageb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'grpc_config_api_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'grpc_config_api_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n6com.tencent.polaris.specification.api.v1.config.manageB\030PolarisConfigGRPCServiceZCgithub.com/polarismesh/specification/source/go/api/v1/config_manage'
-  _POLARISCONFIGGRPC._serialized_start=77
-  _POLARISCONFIGGRPC._serialized_end=249
+  _globals['_POLARISCONFIGGRPC']._serialized_start=77
+  _globals['_POLARISCONFIGGRPC']._serialized_end=472
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,91 +1,92 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: circuitbreaker.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from ..model import model_pb2 as model__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x63ircuitbreaker.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x0bmodel.proto\"\x8e\x06\n\x0e\x43ircuitBreaker\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07version\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04name\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07service\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x37\n\x11service_namespace\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1c\n\x08inbounds\x18\x07 \x03(\x0b\x32\n.v1.CbRule\x12\x1d\n\toutbounds\x18\x08 \x03(\x0b\x32\n.v1.CbRule\x12+\n\x05token\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06owners\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\x08\x62usiness\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\ndepartment\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05\x63time\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05mtime\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\x08revision\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12%\n\x05rules\x18\x15 \x03(\x0b\x32\x16.v1.CircuitBreakerRuleJ\x04\x08\x11\x10\x15\"\xde\x01\n\rSourceMatcher\x12-\n\x07service\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x06labels\x18\x03 \x03(\x0b\x32\x1d.v1.SourceMatcher.LabelsEntry\x1a>\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.v1.MatchString:\x02\x38\x01\"\xb3\x03\n\rRecoverConfig\x12.\n\x0bsleepWindow\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12;\n\x15maxRetryAfterHalfOpen\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12>\n\x18requestRateAfterHalfOpen\x18\x03 \x03(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x38\n\x12successRateToClose\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12?\n\x19requestCountAfterHalfOpen\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12>\n\x11outlierDetectWhen\x18\x06 \x01(\x0e\x32#.v1.RecoverConfig.OutlierDetectWhen\":\n\x11OutlierDetectWhen\x12\t\n\x05NEVER\x10\x00\x12\x0e\n\nON_RECOVER\x10\x01\x12\n\n\x06\x41LWAYS\x10\x02\"\xb9\t\n\x08\x43\x62Policy\x12-\n\terrorRate\x18\x01 \x01(\x0b\x32\x1a.v1.CbPolicy.ErrRateConfig\x12-\n\x08slowRate\x18\x02 \x01(\x0b\x32\x1b.v1.CbPolicy.SlowRateConfig\x12\x30\n\rjudgeDuration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x38\n\x12maxEjectionPercent\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x36\n\x0b\x63onsecutive\x18\x05 \x01(\x0b\x32!.v1.CbPolicy.ConsecutiveErrConfig\x1a\x8a\x04\n\rErrRateConfig\x12*\n\x06\x65nable\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12<\n\x16requestVolumeThreshold\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12:\n\x14\x65rrorRateToPreserved\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x35\n\x0f\x65rrorRateToOpen\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12:\n\x08specials\x18\x05 \x03(\x0b\x32(.v1.CbPolicy.ErrRateConfig.SpecialConfig\x1a\xdf\x01\n\rSpecialConfig\x12*\n\x04type\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\nerrorCodes\x18\x02 \x03(\x0b\x32\x1b.google.protobuf.Int64Value\x12:\n\x14\x65rrorRateToPreserved\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x35\n\x0f\x65rrorRateToOpen\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x1a\xd7\x01\n\x0eSlowRateConfig\x12*\n\x06\x65nable\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12(\n\x05maxRt\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x39\n\x13slowRateToPreserved\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x34\n\x0eslowRateToOpen\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x1a\xc3\x01\n\x14\x43onsecutiveErrConfig\x12*\n\x06\x65nable\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x41\n\x1b\x63onsecutiveErrorToPreserved\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12<\n\x16\x63onsecutiveErrorToOpen\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\"\xf8\x05\n\x0e\x44\x65stinationSet\x12-\n\x07service\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x32\n\x08metadata\x18\x03 \x03(\x0b\x32 .v1.DestinationSet.MetadataEntry\x12-\n\x08resource\x18\x04 \x01(\x0e\x32\x1b.v1.DestinationSet.Resource\x12%\n\x04type\x18\x05 \x01(\x0e\x32\x17.v1.DestinationSet.Type\x12\'\n\x05scope\x18\x06 \x01(\x0e\x32\x18.v1.DestinationSet.Scope\x12/\n\x0cmetricWindow\x18\x07 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x35\n\x0fmetricPrecision\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x31\n\x0eupdateInterval\x18\t \x01(\x0b\x32\x19.google.protobuf.Duration\x12\"\n\x07recover\x18\n \x01(\x0b\x32\x11.v1.RecoverConfig\x12\x1c\n\x06policy\x18\x0b \x01(\x0b\x32\x0c.v1.CbPolicy\x12\x1f\n\x06method\x18\x0c \x01(\x0b\x32\x0f.v1.MatchString\x12/\n\nerrorCodes\x18\r \x03(\x0b\x32\x1b.google.protobuf.Int64Value\x1a@\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.v1.MatchString:\x02\x38\x01\"$\n\x08Resource\x12\n\n\x06SUBSET\x10\x00\x12\x0c\n\x08INSTANCE\x10\x01\"\x1d\n\x04Type\x12\n\n\x06GLOBAL\x10\x00\x12\t\n\x05LOCAL\x10\x01\"\x1d\n\x05Scope\x12\x07\n\x03\x41LL\x10\x00\x12\x0b\n\x07\x43URRENT\x10\x01\"V\n\x06\x43\x62Rule\x12\"\n\x07sources\x18\x01 \x03(\x0b\x32\x11.v1.SourceMatcher\x12(\n\x0c\x64\x65stinations\x18\x02 \x03(\x0b\x32\x12.v1.DestinationSet\"\x85\x02\n\x0bRuleMatcher\x12-\n\x06source\x18\x01 \x01(\x0b\x32\x1d.v1.RuleMatcher.SourceService\x12\x37\n\x0b\x64\x65stination\x18\x02 \x01(\x0b\x32\".v1.RuleMatcher.DestinationService\x1a\x33\n\rSourceService\x12\x0f\n\x07service\x18\x01 \x01(\t\x12\x11\n\tnamespace\x18\x02 \x01(\t\x1aY\n\x12\x44\x65stinationService\x12\x0f\n\x07service\x18\x01 \x01(\t\x12\x11\n\tnamespace\x18\x02 \x01(\t\x12\x1f\n\x06method\x18\x03 \x01(\x0b\x32\x0f.v1.MatchString\"\xf7\x03\n\x12\x43ircuitBreakerRule\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0e\n\x06\x65nable\x18\x04 \x01(\x08\x12\x10\n\x08revision\x18\x05 \x01(\t\x12\r\n\x05\x63time\x18\x06 \x01(\t\x12\r\n\x05mtime\x18\x07 \x01(\t\x12\r\n\x05\x65time\x18\x08 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\t \x01(\t\x12\x18\n\x05level\x18\x15 \x01(\x0e\x32\t.v1.Level\x12%\n\x0crule_matcher\x18\x16 \x01(\x0b\x32\x0f.v1.RuleMatcher\x12,\n\x10\x65rror_conditions\x18\x17 \x03(\x0b\x32\x12.v1.ErrorCondition\x12/\n\x11trigger_condition\x18\x18 \x03(\x0b\x32\x14.v1.TriggerCondition\x12\x1c\n\x14max_ejection_percent\x18\x19 \x01(\r\x12.\n\x10recoverCondition\x18\x1a \x01(\x0b\x32\x14.v1.RecoverCondition\x12\x30\n\x11\x66\x61ultDetectConfig\x18\x1b \x01(\x0b\x32\x15.v1.FaultDetectConfig\x12*\n\x0e\x66\x61llbackConfig\x18\x1c \x01(\x0b\x32\x12.v1.FallbackConfigJ\x04\x08\n\x10\x15\"\x99\x01\n\x0e\x45rrorCondition\x12\x30\n\ninput_type\x18\x01 \x01(\x0e\x32\x1c.v1.ErrorCondition.InputType\x12\"\n\tcondition\x18\x02 \x01(\x0b\x32\x0f.v1.MatchString\"1\n\tInputType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08RET_CODE\x10\x01\x12\t\n\x05\x44\x45LAY\x10\x02\"\xe4\x01\n\x10TriggerCondition\x12\x36\n\x0ctrigger_type\x18\x01 \x01(\x0e\x32 .v1.TriggerCondition.TriggerType\x12\x13\n\x0b\x65rror_count\x18\x02 \x01(\r\x12\x15\n\rerror_percent\x18\x03 \x01(\r\x12\x10\n\x08interval\x18\x04 \x01(\r\x12\x17\n\x0fminimum_request\x18\x05 \x01(\r\"A\n\x0bTriggerType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0e\n\nERROR_RATE\x10\x01\x12\x15\n\x11\x43ONSECUTIVE_ERROR\x10\x02\"D\n\x10RecoverCondition\x12\x14\n\x0csleep_window\x18\x01 \x01(\r\x12\x1a\n\x12\x63onsecutiveSuccess\x18\x02 \x01(\r\"#\n\x11\x46\x61ultDetectConfig\x12\x0e\n\x06\x65nable\x18\x01 \x01(\x08\"H\n\x0e\x46\x61llbackConfig\x12\x0e\n\x06\x65nable\x18\x01 \x01(\x08\x12&\n\x08response\x18\x02 \x01(\x0b\x32\x14.v1.FallbackResponse\"\x90\x01\n\x10\x46\x61llbackResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x33\n\x07headers\x18\x02 \x03(\x0b\x32\".v1.FallbackResponse.MessageHeader\x12\x0c\n\x04\x62ody\x18\x03 \x01(\t\x1a+\n\rMessageHeader\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t*F\n\x05Level\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SERVICE\x10\x01\x12\n\n\x06METHOD\x10\x02\x12\t\n\x05GROUP\x10\x03\x12\x0c\n\x08INSTANCE\x10\x04\x42\x96\x01\n8com.tencent.polaris.specification.api.v1.fault.toleranceB\x13\x43ircuitBreakerProtoZEgithub.com/polarismesh/specification/source/go/api/v1/fault_toleranceb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'circuitbreaker_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'circuitbreaker_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n8com.tencent.polaris.specification.api.v1.fault.toleranceB\023CircuitBreakerProtoZEgithub.com/polarismesh/specification/source/go/api/v1/fault_tolerance'
   _SOURCEMATCHER_LABELSENTRY._options = None
   _SOURCEMATCHER_LABELSENTRY._serialized_options = b'8\001'
   _DESTINATIONSET_METADATAENTRY._options = None
   _DESTINATIONSET_METADATAENTRY._serialized_options = b'8\001'
-  _LEVEL._serialized_start=5101
-  _LEVEL._serialized_end=5171
-  _CIRCUITBREAKER._serialized_start=106
-  _CIRCUITBREAKER._serialized_end=888
-  _SOURCEMATCHER._serialized_start=891
-  _SOURCEMATCHER._serialized_end=1113
-  _SOURCEMATCHER_LABELSENTRY._serialized_start=1051
-  _SOURCEMATCHER_LABELSENTRY._serialized_end=1113
-  _RECOVERCONFIG._serialized_start=1116
-  _RECOVERCONFIG._serialized_end=1551
-  _RECOVERCONFIG_OUTLIERDETECTWHEN._serialized_start=1493
-  _RECOVERCONFIG_OUTLIERDETECTWHEN._serialized_end=1551
-  _CBPOLICY._serialized_start=1554
-  _CBPOLICY._serialized_end=2763
-  _CBPOLICY_ERRRATECONFIG._serialized_start=1825
-  _CBPOLICY_ERRRATECONFIG._serialized_end=2347
-  _CBPOLICY_ERRRATECONFIG_SPECIALCONFIG._serialized_start=2124
-  _CBPOLICY_ERRRATECONFIG_SPECIALCONFIG._serialized_end=2347
-  _CBPOLICY_SLOWRATECONFIG._serialized_start=2350
-  _CBPOLICY_SLOWRATECONFIG._serialized_end=2565
-  _CBPOLICY_CONSECUTIVEERRCONFIG._serialized_start=2568
-  _CBPOLICY_CONSECUTIVEERRCONFIG._serialized_end=2763
-  _DESTINATIONSET._serialized_start=2766
-  _DESTINATIONSET._serialized_end=3526
-  _DESTINATIONSET_METADATAENTRY._serialized_start=3362
-  _DESTINATIONSET_METADATAENTRY._serialized_end=3426
-  _DESTINATIONSET_RESOURCE._serialized_start=3428
-  _DESTINATIONSET_RESOURCE._serialized_end=3464
-  _DESTINATIONSET_TYPE._serialized_start=3466
-  _DESTINATIONSET_TYPE._serialized_end=3495
-  _DESTINATIONSET_SCOPE._serialized_start=3497
-  _DESTINATIONSET_SCOPE._serialized_end=3526
-  _CBRULE._serialized_start=3528
-  _CBRULE._serialized_end=3614
-  _RULEMATCHER._serialized_start=3617
-  _RULEMATCHER._serialized_end=3878
-  _RULEMATCHER_SOURCESERVICE._serialized_start=3736
-  _RULEMATCHER_SOURCESERVICE._serialized_end=3787
-  _RULEMATCHER_DESTINATIONSERVICE._serialized_start=3789
-  _RULEMATCHER_DESTINATIONSERVICE._serialized_end=3878
-  _CIRCUITBREAKERRULE._serialized_start=3881
-  _CIRCUITBREAKERRULE._serialized_end=4384
-  _ERRORCONDITION._serialized_start=4387
-  _ERRORCONDITION._serialized_end=4540
-  _ERRORCONDITION_INPUTTYPE._serialized_start=4491
-  _ERRORCONDITION_INPUTTYPE._serialized_end=4540
-  _TRIGGERCONDITION._serialized_start=4543
-  _TRIGGERCONDITION._serialized_end=4771
-  _TRIGGERCONDITION_TRIGGERTYPE._serialized_start=4706
-  _TRIGGERCONDITION_TRIGGERTYPE._serialized_end=4771
-  _RECOVERCONDITION._serialized_start=4773
-  _RECOVERCONDITION._serialized_end=4841
-  _FAULTDETECTCONFIG._serialized_start=4843
-  _FAULTDETECTCONFIG._serialized_end=4878
-  _FALLBACKCONFIG._serialized_start=4880
-  _FALLBACKCONFIG._serialized_end=4952
-  _FALLBACKRESPONSE._serialized_start=4955
-  _FALLBACKRESPONSE._serialized_end=5099
-  _FALLBACKRESPONSE_MESSAGEHEADER._serialized_start=5056
-  _FALLBACKRESPONSE_MESSAGEHEADER._serialized_end=5099
+  _globals['_LEVEL']._serialized_start=5101
+  _globals['_LEVEL']._serialized_end=5171
+  _globals['_CIRCUITBREAKER']._serialized_start=106
+  _globals['_CIRCUITBREAKER']._serialized_end=888
+  _globals['_SOURCEMATCHER']._serialized_start=891
+  _globals['_SOURCEMATCHER']._serialized_end=1113
+  _globals['_SOURCEMATCHER_LABELSENTRY']._serialized_start=1051
+  _globals['_SOURCEMATCHER_LABELSENTRY']._serialized_end=1113
+  _globals['_RECOVERCONFIG']._serialized_start=1116
+  _globals['_RECOVERCONFIG']._serialized_end=1551
+  _globals['_RECOVERCONFIG_OUTLIERDETECTWHEN']._serialized_start=1493
+  _globals['_RECOVERCONFIG_OUTLIERDETECTWHEN']._serialized_end=1551
+  _globals['_CBPOLICY']._serialized_start=1554
+  _globals['_CBPOLICY']._serialized_end=2763
+  _globals['_CBPOLICY_ERRRATECONFIG']._serialized_start=1825
+  _globals['_CBPOLICY_ERRRATECONFIG']._serialized_end=2347
+  _globals['_CBPOLICY_ERRRATECONFIG_SPECIALCONFIG']._serialized_start=2124
+  _globals['_CBPOLICY_ERRRATECONFIG_SPECIALCONFIG']._serialized_end=2347
+  _globals['_CBPOLICY_SLOWRATECONFIG']._serialized_start=2350
+  _globals['_CBPOLICY_SLOWRATECONFIG']._serialized_end=2565
+  _globals['_CBPOLICY_CONSECUTIVEERRCONFIG']._serialized_start=2568
+  _globals['_CBPOLICY_CONSECUTIVEERRCONFIG']._serialized_end=2763
+  _globals['_DESTINATIONSET']._serialized_start=2766
+  _globals['_DESTINATIONSET']._serialized_end=3526
+  _globals['_DESTINATIONSET_METADATAENTRY']._serialized_start=3362
+  _globals['_DESTINATIONSET_METADATAENTRY']._serialized_end=3426
+  _globals['_DESTINATIONSET_RESOURCE']._serialized_start=3428
+  _globals['_DESTINATIONSET_RESOURCE']._serialized_end=3464
+  _globals['_DESTINATIONSET_TYPE']._serialized_start=3466
+  _globals['_DESTINATIONSET_TYPE']._serialized_end=3495
+  _globals['_DESTINATIONSET_SCOPE']._serialized_start=3497
+  _globals['_DESTINATIONSET_SCOPE']._serialized_end=3526
+  _globals['_CBRULE']._serialized_start=3528
+  _globals['_CBRULE']._serialized_end=3614
+  _globals['_RULEMATCHER']._serialized_start=3617
+  _globals['_RULEMATCHER']._serialized_end=3878
+  _globals['_RULEMATCHER_SOURCESERVICE']._serialized_start=3736
+  _globals['_RULEMATCHER_SOURCESERVICE']._serialized_end=3787
+  _globals['_RULEMATCHER_DESTINATIONSERVICE']._serialized_start=3789
+  _globals['_RULEMATCHER_DESTINATIONSERVICE']._serialized_end=3878
+  _globals['_CIRCUITBREAKERRULE']._serialized_start=3881
+  _globals['_CIRCUITBREAKERRULE']._serialized_end=4384
+  _globals['_ERRORCONDITION']._serialized_start=4387
+  _globals['_ERRORCONDITION']._serialized_end=4540
+  _globals['_ERRORCONDITION_INPUTTYPE']._serialized_start=4491
+  _globals['_ERRORCONDITION_INPUTTYPE']._serialized_end=4540
+  _globals['_TRIGGERCONDITION']._serialized_start=4543
+  _globals['_TRIGGERCONDITION']._serialized_end=4771
+  _globals['_TRIGGERCONDITION_TRIGGERTYPE']._serialized_start=4706
+  _globals['_TRIGGERCONDITION_TRIGGERTYPE']._serialized_end=4771
+  _globals['_RECOVERCONDITION']._serialized_start=4773
+  _globals['_RECOVERCONDITION']._serialized_end=4841
+  _globals['_FAULTDETECTCONFIG']._serialized_start=4843
+  _globals['_FAULTDETECTCONFIG']._serialized_end=4878
+  _globals['_FALLBACKCONFIG']._serialized_start=4880
+  _globals['_FALLBACKCONFIG']._serialized_end=4952
+  _globals['_FALLBACKRESPONSE']._serialized_start=4955
+  _globals['_FALLBACKRESPONSE']._serialized_end=5099
+  _globals['_FALLBACKRESPONSE_MESSAGEHEADER']._serialized_start=5056
+  _globals['_FALLBACKRESPONSE_MESSAGEHEADER']._serialized_end=5099
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,339 +4,359 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
+
+class Level(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    UNKNOWN: _ClassVar[Level]
+    SERVICE: _ClassVar[Level]
+    METHOD: _ClassVar[Level]
+    GROUP: _ClassVar[Level]
+    INSTANCE: _ClassVar[Level]
+UNKNOWN: Level
+SERVICE: Level
+METHOD: Level
 GROUP: Level
 INSTANCE: Level
-METHOD: Level
-SERVICE: Level
-UNKNOWN: Level
+
+class CircuitBreaker(_message.Message):
+    __slots__ = ["id", "version", "name", "namespace", "service", "service_namespace", "inbounds", "outbounds", "token", "owners", "business", "department", "comment", "ctime", "mtime", "revision", "rules"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    VERSION_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    SERVICE_FIELD_NUMBER: _ClassVar[int]
+    SERVICE_NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    INBOUNDS_FIELD_NUMBER: _ClassVar[int]
+    OUTBOUNDS_FIELD_NUMBER: _ClassVar[int]
+    TOKEN_FIELD_NUMBER: _ClassVar[int]
+    OWNERS_FIELD_NUMBER: _ClassVar[int]
+    BUSINESS_FIELD_NUMBER: _ClassVar[int]
+    DEPARTMENT_FIELD_NUMBER: _ClassVar[int]
+    COMMENT_FIELD_NUMBER: _ClassVar[int]
+    CTIME_FIELD_NUMBER: _ClassVar[int]
+    MTIME_FIELD_NUMBER: _ClassVar[int]
+    REVISION_FIELD_NUMBER: _ClassVar[int]
+    RULES_FIELD_NUMBER: _ClassVar[int]
+    id: _wrappers_pb2.StringValue
+    version: _wrappers_pb2.StringValue
+    name: _wrappers_pb2.StringValue
+    namespace: _wrappers_pb2.StringValue
+    service: _wrappers_pb2.StringValue
+    service_namespace: _wrappers_pb2.StringValue
+    inbounds: _containers.RepeatedCompositeFieldContainer[CbRule]
+    outbounds: _containers.RepeatedCompositeFieldContainer[CbRule]
+    token: _wrappers_pb2.StringValue
+    owners: _wrappers_pb2.StringValue
+    business: _wrappers_pb2.StringValue
+    department: _wrappers_pb2.StringValue
+    comment: _wrappers_pb2.StringValue
+    ctime: _wrappers_pb2.StringValue
+    mtime: _wrappers_pb2.StringValue
+    revision: _wrappers_pb2.StringValue
+    rules: _containers.RepeatedCompositeFieldContainer[CircuitBreakerRule]
+    def __init__(self, id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., version: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., service: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., service_namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., inbounds: _Optional[_Iterable[_Union[CbRule, _Mapping]]] = ..., outbounds: _Optional[_Iterable[_Union[CbRule, _Mapping]]] = ..., token: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., owners: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., business: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., department: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., ctime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mtime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., revision: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., rules: _Optional[_Iterable[_Union[CircuitBreakerRule, _Mapping]]] = ...) -> None: ...
+
+class SourceMatcher(_message.Message):
+    __slots__ = ["service", "namespace", "labels"]
+    class LabelsEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: _model_pb2.MatchString
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[_model_pb2.MatchString, _Mapping]] = ...) -> None: ...
+    SERVICE_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    LABELS_FIELD_NUMBER: _ClassVar[int]
+    service: _wrappers_pb2.StringValue
+    namespace: _wrappers_pb2.StringValue
+    labels: _containers.MessageMap[str, _model_pb2.MatchString]
+    def __init__(self, service: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., labels: _Optional[_Mapping[str, _model_pb2.MatchString]] = ...) -> None: ...
+
+class RecoverConfig(_message.Message):
+    __slots__ = ["sleepWindow", "maxRetryAfterHalfOpen", "requestRateAfterHalfOpen", "successRateToClose", "requestCountAfterHalfOpen", "outlierDetectWhen"]
+    class OutlierDetectWhen(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        NEVER: _ClassVar[RecoverConfig.OutlierDetectWhen]
+        ON_RECOVER: _ClassVar[RecoverConfig.OutlierDetectWhen]
+        ALWAYS: _ClassVar[RecoverConfig.OutlierDetectWhen]
+    NEVER: RecoverConfig.OutlierDetectWhen
+    ON_RECOVER: RecoverConfig.OutlierDetectWhen
+    ALWAYS: RecoverConfig.OutlierDetectWhen
+    SLEEPWINDOW_FIELD_NUMBER: _ClassVar[int]
+    MAXRETRYAFTERHALFOPEN_FIELD_NUMBER: _ClassVar[int]
+    REQUESTRATEAFTERHALFOPEN_FIELD_NUMBER: _ClassVar[int]
+    SUCCESSRATETOCLOSE_FIELD_NUMBER: _ClassVar[int]
+    REQUESTCOUNTAFTERHALFOPEN_FIELD_NUMBER: _ClassVar[int]
+    OUTLIERDETECTWHEN_FIELD_NUMBER: _ClassVar[int]
+    sleepWindow: _duration_pb2.Duration
+    maxRetryAfterHalfOpen: _wrappers_pb2.UInt32Value
+    requestRateAfterHalfOpen: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.UInt32Value]
+    successRateToClose: _wrappers_pb2.UInt32Value
+    requestCountAfterHalfOpen: _wrappers_pb2.UInt32Value
+    outlierDetectWhen: RecoverConfig.OutlierDetectWhen
+    def __init__(self, sleepWindow: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., maxRetryAfterHalfOpen: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., requestRateAfterHalfOpen: _Optional[_Iterable[_Union[_wrappers_pb2.UInt32Value, _Mapping]]] = ..., successRateToClose: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., requestCountAfterHalfOpen: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., outlierDetectWhen: _Optional[_Union[RecoverConfig.OutlierDetectWhen, str]] = ...) -> None: ...
 
 class CbPolicy(_message.Message):
-    __slots__ = ["consecutive", "errorRate", "judgeDuration", "maxEjectionPercent", "slowRate"]
-    class ConsecutiveErrConfig(_message.Message):
-        __slots__ = ["consecutiveErrorToOpen", "consecutiveErrorToPreserved", "enable"]
-        CONSECUTIVEERRORTOOPEN_FIELD_NUMBER: _ClassVar[int]
-        CONSECUTIVEERRORTOPRESERVED_FIELD_NUMBER: _ClassVar[int]
-        ENABLE_FIELD_NUMBER: _ClassVar[int]
-        consecutiveErrorToOpen: _wrappers_pb2.UInt32Value
-        consecutiveErrorToPreserved: _wrappers_pb2.UInt32Value
-        enable: _wrappers_pb2.BoolValue
-        def __init__(self, enable: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., consecutiveErrorToPreserved: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., consecutiveErrorToOpen: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ...) -> None: ...
+    __slots__ = ["errorRate", "slowRate", "judgeDuration", "maxEjectionPercent", "consecutive"]
     class ErrRateConfig(_message.Message):
-        __slots__ = ["enable", "errorRateToOpen", "errorRateToPreserved", "requestVolumeThreshold", "specials"]
+        __slots__ = ["enable", "requestVolumeThreshold", "errorRateToPreserved", "errorRateToOpen", "specials"]
         class SpecialConfig(_message.Message):
-            __slots__ = ["errorCodes", "errorRateToOpen", "errorRateToPreserved", "type"]
+            __slots__ = ["type", "errorCodes", "errorRateToPreserved", "errorRateToOpen"]
+            TYPE_FIELD_NUMBER: _ClassVar[int]
             ERRORCODES_FIELD_NUMBER: _ClassVar[int]
-            ERRORRATETOOPEN_FIELD_NUMBER: _ClassVar[int]
             ERRORRATETOPRESERVED_FIELD_NUMBER: _ClassVar[int]
-            TYPE_FIELD_NUMBER: _ClassVar[int]
+            ERRORRATETOOPEN_FIELD_NUMBER: _ClassVar[int]
+            type: _wrappers_pb2.StringValue
             errorCodes: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.Int64Value]
-            errorRateToOpen: _wrappers_pb2.UInt32Value
             errorRateToPreserved: _wrappers_pb2.UInt32Value
-            type: _wrappers_pb2.StringValue
+            errorRateToOpen: _wrappers_pb2.UInt32Value
             def __init__(self, type: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., errorCodes: _Optional[_Iterable[_Union[_wrappers_pb2.Int64Value, _Mapping]]] = ..., errorRateToPreserved: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., errorRateToOpen: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ...) -> None: ...
         ENABLE_FIELD_NUMBER: _ClassVar[int]
-        ERRORRATETOOPEN_FIELD_NUMBER: _ClassVar[int]
-        ERRORRATETOPRESERVED_FIELD_NUMBER: _ClassVar[int]
         REQUESTVOLUMETHRESHOLD_FIELD_NUMBER: _ClassVar[int]
+        ERRORRATETOPRESERVED_FIELD_NUMBER: _ClassVar[int]
+        ERRORRATETOOPEN_FIELD_NUMBER: _ClassVar[int]
         SPECIALS_FIELD_NUMBER: _ClassVar[int]
         enable: _wrappers_pb2.BoolValue
-        errorRateToOpen: _wrappers_pb2.UInt32Value
-        errorRateToPreserved: _wrappers_pb2.UInt32Value
         requestVolumeThreshold: _wrappers_pb2.UInt32Value
+        errorRateToPreserved: _wrappers_pb2.UInt32Value
+        errorRateToOpen: _wrappers_pb2.UInt32Value
         specials: _containers.RepeatedCompositeFieldContainer[CbPolicy.ErrRateConfig.SpecialConfig]
         def __init__(self, enable: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., requestVolumeThreshold: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., errorRateToPreserved: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., errorRateToOpen: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., specials: _Optional[_Iterable[_Union[CbPolicy.ErrRateConfig.SpecialConfig, _Mapping]]] = ...) -> None: ...
     class SlowRateConfig(_message.Message):
-        __slots__ = ["enable", "maxRt", "slowRateToOpen", "slowRateToPreserved"]
+        __slots__ = ["enable", "maxRt", "slowRateToPreserved", "slowRateToOpen"]
         ENABLE_FIELD_NUMBER: _ClassVar[int]
         MAXRT_FIELD_NUMBER: _ClassVar[int]
-        SLOWRATETOOPEN_FIELD_NUMBER: _ClassVar[int]
         SLOWRATETOPRESERVED_FIELD_NUMBER: _ClassVar[int]
+        SLOWRATETOOPEN_FIELD_NUMBER: _ClassVar[int]
         enable: _wrappers_pb2.BoolValue
         maxRt: _duration_pb2.Duration
-        slowRateToOpen: _wrappers_pb2.UInt32Value
         slowRateToPreserved: _wrappers_pb2.UInt32Value
+        slowRateToOpen: _wrappers_pb2.UInt32Value
         def __init__(self, enable: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., maxRt: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., slowRateToPreserved: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., slowRateToOpen: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ...) -> None: ...
-    CONSECUTIVE_FIELD_NUMBER: _ClassVar[int]
+    class ConsecutiveErrConfig(_message.Message):
+        __slots__ = ["enable", "consecutiveErrorToPreserved", "consecutiveErrorToOpen"]
+        ENABLE_FIELD_NUMBER: _ClassVar[int]
+        CONSECUTIVEERRORTOPRESERVED_FIELD_NUMBER: _ClassVar[int]
+        CONSECUTIVEERRORTOOPEN_FIELD_NUMBER: _ClassVar[int]
+        enable: _wrappers_pb2.BoolValue
+        consecutiveErrorToPreserved: _wrappers_pb2.UInt32Value
+        consecutiveErrorToOpen: _wrappers_pb2.UInt32Value
+        def __init__(self, enable: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., consecutiveErrorToPreserved: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., consecutiveErrorToOpen: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ...) -> None: ...
     ERRORRATE_FIELD_NUMBER: _ClassVar[int]
+    SLOWRATE_FIELD_NUMBER: _ClassVar[int]
     JUDGEDURATION_FIELD_NUMBER: _ClassVar[int]
     MAXEJECTIONPERCENT_FIELD_NUMBER: _ClassVar[int]
-    SLOWRATE_FIELD_NUMBER: _ClassVar[int]
-    consecutive: CbPolicy.ConsecutiveErrConfig
+    CONSECUTIVE_FIELD_NUMBER: _ClassVar[int]
     errorRate: CbPolicy.ErrRateConfig
+    slowRate: CbPolicy.SlowRateConfig
     judgeDuration: _duration_pb2.Duration
     maxEjectionPercent: _wrappers_pb2.UInt32Value
-    slowRate: CbPolicy.SlowRateConfig
+    consecutive: CbPolicy.ConsecutiveErrConfig
     def __init__(self, errorRate: _Optional[_Union[CbPolicy.ErrRateConfig, _Mapping]] = ..., slowRate: _Optional[_Union[CbPolicy.SlowRateConfig, _Mapping]] = ..., judgeDuration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., maxEjectionPercent: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., consecutive: _Optional[_Union[CbPolicy.ConsecutiveErrConfig, _Mapping]] = ...) -> None: ...
 
-class CbRule(_message.Message):
-    __slots__ = ["destinations", "sources"]
-    DESTINATIONS_FIELD_NUMBER: _ClassVar[int]
-    SOURCES_FIELD_NUMBER: _ClassVar[int]
-    destinations: _containers.RepeatedCompositeFieldContainer[DestinationSet]
-    sources: _containers.RepeatedCompositeFieldContainer[SourceMatcher]
-    def __init__(self, sources: _Optional[_Iterable[_Union[SourceMatcher, _Mapping]]] = ..., destinations: _Optional[_Iterable[_Union[DestinationSet, _Mapping]]] = ...) -> None: ...
-
-class CircuitBreaker(_message.Message):
-    __slots__ = ["business", "comment", "ctime", "department", "id", "inbounds", "mtime", "name", "namespace", "outbounds", "owners", "revision", "rules", "service", "service_namespace", "token", "version"]
-    BUSINESS_FIELD_NUMBER: _ClassVar[int]
-    COMMENT_FIELD_NUMBER: _ClassVar[int]
-    CTIME_FIELD_NUMBER: _ClassVar[int]
-    DEPARTMENT_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    INBOUNDS_FIELD_NUMBER: _ClassVar[int]
-    MTIME_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    OUTBOUNDS_FIELD_NUMBER: _ClassVar[int]
-    OWNERS_FIELD_NUMBER: _ClassVar[int]
-    REVISION_FIELD_NUMBER: _ClassVar[int]
-    RULES_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    TOKEN_FIELD_NUMBER: _ClassVar[int]
-    VERSION_FIELD_NUMBER: _ClassVar[int]
-    business: _wrappers_pb2.StringValue
-    comment: _wrappers_pb2.StringValue
-    ctime: _wrappers_pb2.StringValue
-    department: _wrappers_pb2.StringValue
-    id: _wrappers_pb2.StringValue
-    inbounds: _containers.RepeatedCompositeFieldContainer[CbRule]
-    mtime: _wrappers_pb2.StringValue
-    name: _wrappers_pb2.StringValue
-    namespace: _wrappers_pb2.StringValue
-    outbounds: _containers.RepeatedCompositeFieldContainer[CbRule]
-    owners: _wrappers_pb2.StringValue
-    revision: _wrappers_pb2.StringValue
-    rules: _containers.RepeatedCompositeFieldContainer[CircuitBreakerRule]
-    service: _wrappers_pb2.StringValue
-    service_namespace: _wrappers_pb2.StringValue
-    token: _wrappers_pb2.StringValue
-    version: _wrappers_pb2.StringValue
-    def __init__(self, id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., version: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., service: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., service_namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., inbounds: _Optional[_Iterable[_Union[CbRule, _Mapping]]] = ..., outbounds: _Optional[_Iterable[_Union[CbRule, _Mapping]]] = ..., token: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., owners: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., business: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., department: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., ctime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mtime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., revision: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., rules: _Optional[_Iterable[_Union[CircuitBreakerRule, _Mapping]]] = ...) -> None: ...
-
-class CircuitBreakerRule(_message.Message):
-    __slots__ = ["ctime", "description", "enable", "error_conditions", "etime", "fallbackConfig", "faultDetectConfig", "id", "level", "max_ejection_percent", "mtime", "name", "namespace", "recoverCondition", "revision", "rule_matcher", "trigger_condition"]
-    CTIME_FIELD_NUMBER: _ClassVar[int]
-    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    ENABLE_FIELD_NUMBER: _ClassVar[int]
-    ERROR_CONDITIONS_FIELD_NUMBER: _ClassVar[int]
-    ETIME_FIELD_NUMBER: _ClassVar[int]
-    FALLBACKCONFIG_FIELD_NUMBER: _ClassVar[int]
-    FAULTDETECTCONFIG_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    LEVEL_FIELD_NUMBER: _ClassVar[int]
-    MAX_EJECTION_PERCENT_FIELD_NUMBER: _ClassVar[int]
-    MTIME_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    RECOVERCONDITION_FIELD_NUMBER: _ClassVar[int]
-    REVISION_FIELD_NUMBER: _ClassVar[int]
-    RULE_MATCHER_FIELD_NUMBER: _ClassVar[int]
-    TRIGGER_CONDITION_FIELD_NUMBER: _ClassVar[int]
-    ctime: str
-    description: str
-    enable: bool
-    error_conditions: _containers.RepeatedCompositeFieldContainer[ErrorCondition]
-    etime: str
-    fallbackConfig: FallbackConfig
-    faultDetectConfig: FaultDetectConfig
-    id: str
-    level: Level
-    max_ejection_percent: int
-    mtime: str
-    name: str
-    namespace: str
-    recoverCondition: RecoverCondition
-    revision: str
-    rule_matcher: RuleMatcher
-    trigger_condition: _containers.RepeatedCompositeFieldContainer[TriggerCondition]
-    def __init__(self, id: _Optional[str] = ..., name: _Optional[str] = ..., namespace: _Optional[str] = ..., enable: bool = ..., revision: _Optional[str] = ..., ctime: _Optional[str] = ..., mtime: _Optional[str] = ..., etime: _Optional[str] = ..., description: _Optional[str] = ..., level: _Optional[_Union[Level, str]] = ..., rule_matcher: _Optional[_Union[RuleMatcher, _Mapping]] = ..., error_conditions: _Optional[_Iterable[_Union[ErrorCondition, _Mapping]]] = ..., trigger_condition: _Optional[_Iterable[_Union[TriggerCondition, _Mapping]]] = ..., max_ejection_percent: _Optional[int] = ..., recoverCondition: _Optional[_Union[RecoverCondition, _Mapping]] = ..., faultDetectConfig: _Optional[_Union[FaultDetectConfig, _Mapping]] = ..., fallbackConfig: _Optional[_Union[FallbackConfig, _Mapping]] = ...) -> None: ...
-
 class DestinationSet(_message.Message):
-    __slots__ = ["errorCodes", "metadata", "method", "metricPrecision", "metricWindow", "namespace", "policy", "recover", "resource", "scope", "service", "type", "updateInterval"]
+    __slots__ = ["service", "namespace", "metadata", "resource", "type", "scope", "metricWindow", "metricPrecision", "updateInterval", "recover", "policy", "method", "errorCodes"]
     class Resource(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
-    class Scope(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
+        SUBSET: _ClassVar[DestinationSet.Resource]
+        INSTANCE: _ClassVar[DestinationSet.Resource]
+    SUBSET: DestinationSet.Resource
+    INSTANCE: DestinationSet.Resource
     class Type(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        GLOBAL: _ClassVar[DestinationSet.Type]
+        LOCAL: _ClassVar[DestinationSet.Type]
+    GLOBAL: DestinationSet.Type
+    LOCAL: DestinationSet.Type
+    class Scope(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        ALL: _ClassVar[DestinationSet.Scope]
+        CURRENT: _ClassVar[DestinationSet.Scope]
+    ALL: DestinationSet.Scope
+    CURRENT: DestinationSet.Scope
     class MetadataEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: _model_pb2.MatchString
         def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[_model_pb2.MatchString, _Mapping]] = ...) -> None: ...
-    ALL: DestinationSet.Scope
-    CURRENT: DestinationSet.Scope
-    ERRORCODES_FIELD_NUMBER: _ClassVar[int]
-    GLOBAL: DestinationSet.Type
-    INSTANCE: DestinationSet.Resource
-    LOCAL: DestinationSet.Type
-    METADATA_FIELD_NUMBER: _ClassVar[int]
-    METHOD_FIELD_NUMBER: _ClassVar[int]
-    METRICPRECISION_FIELD_NUMBER: _ClassVar[int]
-    METRICWINDOW_FIELD_NUMBER: _ClassVar[int]
+    SERVICE_FIELD_NUMBER: _ClassVar[int]
     NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    POLICY_FIELD_NUMBER: _ClassVar[int]
-    RECOVER_FIELD_NUMBER: _ClassVar[int]
+    METADATA_FIELD_NUMBER: _ClassVar[int]
     RESOURCE_FIELD_NUMBER: _ClassVar[int]
-    SCOPE_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_FIELD_NUMBER: _ClassVar[int]
-    SUBSET: DestinationSet.Resource
     TYPE_FIELD_NUMBER: _ClassVar[int]
+    SCOPE_FIELD_NUMBER: _ClassVar[int]
+    METRICWINDOW_FIELD_NUMBER: _ClassVar[int]
+    METRICPRECISION_FIELD_NUMBER: _ClassVar[int]
     UPDATEINTERVAL_FIELD_NUMBER: _ClassVar[int]
-    errorCodes: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.Int64Value]
-    metadata: _containers.MessageMap[str, _model_pb2.MatchString]
-    method: _model_pb2.MatchString
-    metricPrecision: _wrappers_pb2.UInt32Value
-    metricWindow: _duration_pb2.Duration
+    RECOVER_FIELD_NUMBER: _ClassVar[int]
+    POLICY_FIELD_NUMBER: _ClassVar[int]
+    METHOD_FIELD_NUMBER: _ClassVar[int]
+    ERRORCODES_FIELD_NUMBER: _ClassVar[int]
+    service: _wrappers_pb2.StringValue
     namespace: _wrappers_pb2.StringValue
-    policy: CbPolicy
-    recover: RecoverConfig
+    metadata: _containers.MessageMap[str, _model_pb2.MatchString]
     resource: DestinationSet.Resource
-    scope: DestinationSet.Scope
-    service: _wrappers_pb2.StringValue
     type: DestinationSet.Type
+    scope: DestinationSet.Scope
+    metricWindow: _duration_pb2.Duration
+    metricPrecision: _wrappers_pb2.UInt32Value
     updateInterval: _duration_pb2.Duration
+    recover: RecoverConfig
+    policy: CbPolicy
+    method: _model_pb2.MatchString
+    errorCodes: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.Int64Value]
     def __init__(self, service: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., metadata: _Optional[_Mapping[str, _model_pb2.MatchString]] = ..., resource: _Optional[_Union[DestinationSet.Resource, str]] = ..., type: _Optional[_Union[DestinationSet.Type, str]] = ..., scope: _Optional[_Union[DestinationSet.Scope, str]] = ..., metricWindow: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., metricPrecision: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., updateInterval: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., recover: _Optional[_Union[RecoverConfig, _Mapping]] = ..., policy: _Optional[_Union[CbPolicy, _Mapping]] = ..., method: _Optional[_Union[_model_pb2.MatchString, _Mapping]] = ..., errorCodes: _Optional[_Iterable[_Union[_wrappers_pb2.Int64Value, _Mapping]]] = ...) -> None: ...
 
+class CbRule(_message.Message):
+    __slots__ = ["sources", "destinations"]
+    SOURCES_FIELD_NUMBER: _ClassVar[int]
+    DESTINATIONS_FIELD_NUMBER: _ClassVar[int]
+    sources: _containers.RepeatedCompositeFieldContainer[SourceMatcher]
+    destinations: _containers.RepeatedCompositeFieldContainer[DestinationSet]
+    def __init__(self, sources: _Optional[_Iterable[_Union[SourceMatcher, _Mapping]]] = ..., destinations: _Optional[_Iterable[_Union[DestinationSet, _Mapping]]] = ...) -> None: ...
+
+class RuleMatcher(_message.Message):
+    __slots__ = ["source", "destination"]
+    class SourceService(_message.Message):
+        __slots__ = ["service", "namespace"]
+        SERVICE_FIELD_NUMBER: _ClassVar[int]
+        NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+        service: str
+        namespace: str
+        def __init__(self, service: _Optional[str] = ..., namespace: _Optional[str] = ...) -> None: ...
+    class DestinationService(_message.Message):
+        __slots__ = ["service", "namespace", "method"]
+        SERVICE_FIELD_NUMBER: _ClassVar[int]
+        NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+        METHOD_FIELD_NUMBER: _ClassVar[int]
+        service: str
+        namespace: str
+        method: _model_pb2.MatchString
+        def __init__(self, service: _Optional[str] = ..., namespace: _Optional[str] = ..., method: _Optional[_Union[_model_pb2.MatchString, _Mapping]] = ...) -> None: ...
+    SOURCE_FIELD_NUMBER: _ClassVar[int]
+    DESTINATION_FIELD_NUMBER: _ClassVar[int]
+    source: RuleMatcher.SourceService
+    destination: RuleMatcher.DestinationService
+    def __init__(self, source: _Optional[_Union[RuleMatcher.SourceService, _Mapping]] = ..., destination: _Optional[_Union[RuleMatcher.DestinationService, _Mapping]] = ...) -> None: ...
+
+class CircuitBreakerRule(_message.Message):
+    __slots__ = ["id", "name", "namespace", "enable", "revision", "ctime", "mtime", "etime", "description", "level", "rule_matcher", "error_conditions", "trigger_condition", "max_ejection_percent", "recoverCondition", "faultDetectConfig", "fallbackConfig"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    ENABLE_FIELD_NUMBER: _ClassVar[int]
+    REVISION_FIELD_NUMBER: _ClassVar[int]
+    CTIME_FIELD_NUMBER: _ClassVar[int]
+    MTIME_FIELD_NUMBER: _ClassVar[int]
+    ETIME_FIELD_NUMBER: _ClassVar[int]
+    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
+    LEVEL_FIELD_NUMBER: _ClassVar[int]
+    RULE_MATCHER_FIELD_NUMBER: _ClassVar[int]
+    ERROR_CONDITIONS_FIELD_NUMBER: _ClassVar[int]
+    TRIGGER_CONDITION_FIELD_NUMBER: _ClassVar[int]
+    MAX_EJECTION_PERCENT_FIELD_NUMBER: _ClassVar[int]
+    RECOVERCONDITION_FIELD_NUMBER: _ClassVar[int]
+    FAULTDETECTCONFIG_FIELD_NUMBER: _ClassVar[int]
+    FALLBACKCONFIG_FIELD_NUMBER: _ClassVar[int]
+    id: str
+    name: str
+    namespace: str
+    enable: bool
+    revision: str
+    ctime: str
+    mtime: str
+    etime: str
+    description: str
+    level: Level
+    rule_matcher: RuleMatcher
+    error_conditions: _containers.RepeatedCompositeFieldContainer[ErrorCondition]
+    trigger_condition: _containers.RepeatedCompositeFieldContainer[TriggerCondition]
+    max_ejection_percent: int
+    recoverCondition: RecoverCondition
+    faultDetectConfig: FaultDetectConfig
+    fallbackConfig: FallbackConfig
+    def __init__(self, id: _Optional[str] = ..., name: _Optional[str] = ..., namespace: _Optional[str] = ..., enable: bool = ..., revision: _Optional[str] = ..., ctime: _Optional[str] = ..., mtime: _Optional[str] = ..., etime: _Optional[str] = ..., description: _Optional[str] = ..., level: _Optional[_Union[Level, str]] = ..., rule_matcher: _Optional[_Union[RuleMatcher, _Mapping]] = ..., error_conditions: _Optional[_Iterable[_Union[ErrorCondition, _Mapping]]] = ..., trigger_condition: _Optional[_Iterable[_Union[TriggerCondition, _Mapping]]] = ..., max_ejection_percent: _Optional[int] = ..., recoverCondition: _Optional[_Union[RecoverCondition, _Mapping]] = ..., faultDetectConfig: _Optional[_Union[FaultDetectConfig, _Mapping]] = ..., fallbackConfig: _Optional[_Union[FallbackConfig, _Mapping]] = ...) -> None: ...
+
 class ErrorCondition(_message.Message):
-    __slots__ = ["condition", "input_type"]
+    __slots__ = ["input_type", "condition"]
     class InputType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
-    CONDITION_FIELD_NUMBER: _ClassVar[int]
+        UNKNOWN: _ClassVar[ErrorCondition.InputType]
+        RET_CODE: _ClassVar[ErrorCondition.InputType]
+        DELAY: _ClassVar[ErrorCondition.InputType]
+    UNKNOWN: ErrorCondition.InputType
+    RET_CODE: ErrorCondition.InputType
     DELAY: ErrorCondition.InputType
     INPUT_TYPE_FIELD_NUMBER: _ClassVar[int]
-    RET_CODE: ErrorCondition.InputType
-    UNKNOWN: ErrorCondition.InputType
-    condition: _model_pb2.MatchString
+    CONDITION_FIELD_NUMBER: _ClassVar[int]
     input_type: ErrorCondition.InputType
+    condition: _model_pb2.MatchString
     def __init__(self, input_type: _Optional[_Union[ErrorCondition.InputType, str]] = ..., condition: _Optional[_Union[_model_pb2.MatchString, _Mapping]] = ...) -> None: ...
 
+class TriggerCondition(_message.Message):
+    __slots__ = ["trigger_type", "error_count", "error_percent", "interval", "minimum_request"]
+    class TriggerType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        UNKNOWN: _ClassVar[TriggerCondition.TriggerType]
+        ERROR_RATE: _ClassVar[TriggerCondition.TriggerType]
+        CONSECUTIVE_ERROR: _ClassVar[TriggerCondition.TriggerType]
+    UNKNOWN: TriggerCondition.TriggerType
+    ERROR_RATE: TriggerCondition.TriggerType
+    CONSECUTIVE_ERROR: TriggerCondition.TriggerType
+    TRIGGER_TYPE_FIELD_NUMBER: _ClassVar[int]
+    ERROR_COUNT_FIELD_NUMBER: _ClassVar[int]
+    ERROR_PERCENT_FIELD_NUMBER: _ClassVar[int]
+    INTERVAL_FIELD_NUMBER: _ClassVar[int]
+    MINIMUM_REQUEST_FIELD_NUMBER: _ClassVar[int]
+    trigger_type: TriggerCondition.TriggerType
+    error_count: int
+    error_percent: int
+    interval: int
+    minimum_request: int
+    def __init__(self, trigger_type: _Optional[_Union[TriggerCondition.TriggerType, str]] = ..., error_count: _Optional[int] = ..., error_percent: _Optional[int] = ..., interval: _Optional[int] = ..., minimum_request: _Optional[int] = ...) -> None: ...
+
+class RecoverCondition(_message.Message):
+    __slots__ = ["sleep_window", "consecutiveSuccess"]
+    SLEEP_WINDOW_FIELD_NUMBER: _ClassVar[int]
+    CONSECUTIVESUCCESS_FIELD_NUMBER: _ClassVar[int]
+    sleep_window: int
+    consecutiveSuccess: int
+    def __init__(self, sleep_window: _Optional[int] = ..., consecutiveSuccess: _Optional[int] = ...) -> None: ...
+
+class FaultDetectConfig(_message.Message):
+    __slots__ = ["enable"]
+    ENABLE_FIELD_NUMBER: _ClassVar[int]
+    enable: bool
+    def __init__(self, enable: bool = ...) -> None: ...
+
 class FallbackConfig(_message.Message):
     __slots__ = ["enable", "response"]
     ENABLE_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_FIELD_NUMBER: _ClassVar[int]
     enable: bool
     response: FallbackResponse
     def __init__(self, enable: bool = ..., response: _Optional[_Union[FallbackResponse, _Mapping]] = ...) -> None: ...
 
 class FallbackResponse(_message.Message):
-    __slots__ = ["body", "code", "headers"]
+    __slots__ = ["code", "headers", "body"]
     class MessageHeader(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
         def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
-    BODY_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
     HEADERS_FIELD_NUMBER: _ClassVar[int]
-    body: str
+    BODY_FIELD_NUMBER: _ClassVar[int]
     code: int
     headers: _containers.RepeatedCompositeFieldContainer[FallbackResponse.MessageHeader]
+    body: str
     def __init__(self, code: _Optional[int] = ..., headers: _Optional[_Iterable[_Union[FallbackResponse.MessageHeader, _Mapping]]] = ..., body: _Optional[str] = ...) -> None: ...
-
-class FaultDetectConfig(_message.Message):
-    __slots__ = ["enable"]
-    ENABLE_FIELD_NUMBER: _ClassVar[int]
-    enable: bool
-    def __init__(self, enable: bool = ...) -> None: ...
-
-class RecoverCondition(_message.Message):
-    __slots__ = ["consecutiveSuccess", "sleep_window"]
-    CONSECUTIVESUCCESS_FIELD_NUMBER: _ClassVar[int]
-    SLEEP_WINDOW_FIELD_NUMBER: _ClassVar[int]
-    consecutiveSuccess: int
-    sleep_window: int
-    def __init__(self, sleep_window: _Optional[int] = ..., consecutiveSuccess: _Optional[int] = ...) -> None: ...
-
-class RecoverConfig(_message.Message):
-    __slots__ = ["maxRetryAfterHalfOpen", "outlierDetectWhen", "requestCountAfterHalfOpen", "requestRateAfterHalfOpen", "sleepWindow", "successRateToClose"]
-    class OutlierDetectWhen(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    ALWAYS: RecoverConfig.OutlierDetectWhen
-    MAXRETRYAFTERHALFOPEN_FIELD_NUMBER: _ClassVar[int]
-    NEVER: RecoverConfig.OutlierDetectWhen
-    ON_RECOVER: RecoverConfig.OutlierDetectWhen
-    OUTLIERDETECTWHEN_FIELD_NUMBER: _ClassVar[int]
-    REQUESTCOUNTAFTERHALFOPEN_FIELD_NUMBER: _ClassVar[int]
-    REQUESTRATEAFTERHALFOPEN_FIELD_NUMBER: _ClassVar[int]
-    SLEEPWINDOW_FIELD_NUMBER: _ClassVar[int]
-    SUCCESSRATETOCLOSE_FIELD_NUMBER: _ClassVar[int]
-    maxRetryAfterHalfOpen: _wrappers_pb2.UInt32Value
-    outlierDetectWhen: RecoverConfig.OutlierDetectWhen
-    requestCountAfterHalfOpen: _wrappers_pb2.UInt32Value
-    requestRateAfterHalfOpen: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.UInt32Value]
-    sleepWindow: _duration_pb2.Duration
-    successRateToClose: _wrappers_pb2.UInt32Value
-    def __init__(self, sleepWindow: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., maxRetryAfterHalfOpen: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., requestRateAfterHalfOpen: _Optional[_Iterable[_Union[_wrappers_pb2.UInt32Value, _Mapping]]] = ..., successRateToClose: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., requestCountAfterHalfOpen: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., outlierDetectWhen: _Optional[_Union[RecoverConfig.OutlierDetectWhen, str]] = ...) -> None: ...
-
-class RuleMatcher(_message.Message):
-    __slots__ = ["destination", "source"]
-    class DestinationService(_message.Message):
-        __slots__ = ["method", "namespace", "service"]
-        METHOD_FIELD_NUMBER: _ClassVar[int]
-        NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-        SERVICE_FIELD_NUMBER: _ClassVar[int]
-        method: _model_pb2.MatchString
-        namespace: str
-        service: str
-        def __init__(self, service: _Optional[str] = ..., namespace: _Optional[str] = ..., method: _Optional[_Union[_model_pb2.MatchString, _Mapping]] = ...) -> None: ...
-    class SourceService(_message.Message):
-        __slots__ = ["namespace", "service"]
-        NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-        SERVICE_FIELD_NUMBER: _ClassVar[int]
-        namespace: str
-        service: str
-        def __init__(self, service: _Optional[str] = ..., namespace: _Optional[str] = ...) -> None: ...
-    DESTINATION_FIELD_NUMBER: _ClassVar[int]
-    SOURCE_FIELD_NUMBER: _ClassVar[int]
-    destination: RuleMatcher.DestinationService
-    source: RuleMatcher.SourceService
-    def __init__(self, source: _Optional[_Union[RuleMatcher.SourceService, _Mapping]] = ..., destination: _Optional[_Union[RuleMatcher.DestinationService, _Mapping]] = ...) -> None: ...
-
-class SourceMatcher(_message.Message):
-    __slots__ = ["labels", "namespace", "service"]
-    class LabelsEntry(_message.Message):
-        __slots__ = ["key", "value"]
-        KEY_FIELD_NUMBER: _ClassVar[int]
-        VALUE_FIELD_NUMBER: _ClassVar[int]
-        key: str
-        value: _model_pb2.MatchString
-        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[_model_pb2.MatchString, _Mapping]] = ...) -> None: ...
-    LABELS_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_FIELD_NUMBER: _ClassVar[int]
-    labels: _containers.MessageMap[str, _model_pb2.MatchString]
-    namespace: _wrappers_pb2.StringValue
-    service: _wrappers_pb2.StringValue
-    def __init__(self, service: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., labels: _Optional[_Mapping[str, _model_pb2.MatchString]] = ...) -> None: ...
-
-class TriggerCondition(_message.Message):
-    __slots__ = ["error_count", "error_percent", "interval", "minimum_request", "trigger_type"]
-    class TriggerType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    CONSECUTIVE_ERROR: TriggerCondition.TriggerType
-    ERROR_COUNT_FIELD_NUMBER: _ClassVar[int]
-    ERROR_PERCENT_FIELD_NUMBER: _ClassVar[int]
-    ERROR_RATE: TriggerCondition.TriggerType
-    INTERVAL_FIELD_NUMBER: _ClassVar[int]
-    MINIMUM_REQUEST_FIELD_NUMBER: _ClassVar[int]
-    TRIGGER_TYPE_FIELD_NUMBER: _ClassVar[int]
-    UNKNOWN: TriggerCondition.TriggerType
-    error_count: int
-    error_percent: int
-    interval: int
-    minimum_request: int
-    trigger_type: TriggerCondition.TriggerType
-    def __init__(self, trigger_type: _Optional[_Union[TriggerCondition.TriggerType, str]] = ..., error_count: _Optional[int] = ..., error_percent: _Optional[int] = ..., interval: _Optional[int] = ..., minimum_request: _Optional[int] = ...) -> None: ...
-
-class Level(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: fault_detector.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ..model import model_pb2 as model__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x66\x61ult_detector.proto\x12\x02v1\x1a\x0bmodel.proto\"E\n\rFaultDetector\x12\"\n\x05rules\x18\x01 \x03(\x0b\x32\x13.v1.FaultDetectRule\x12\x10\n\x08revision\x18\x02 \x01(\t\"\xbd\x04\n\x0f\x46\x61ultDetectRule\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x10\n\x08revision\x18\x04 \x01(\t\x12\r\n\x05\x63time\x18\x05 \x01(\t\x12\r\n\x05mtime\x18\x06 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12>\n\x0etarget_service\x18\x15 \x01(\x0b\x32&.v1.FaultDetectRule.DestinationService\x12\x10\n\x08interval\x18\x16 \x01(\r\x12\x0f\n\x07timeout\x18\x17 \x01(\r\x12\x0c\n\x04port\x18\x18 \x01(\r\x12.\n\x08protocol\x18\x19 \x01(\x0e\x32\x1c.v1.FaultDetectRule.Protocol\x12+\n\x0bhttp_config\x18\x1a \x01(\x0b\x32\x16.v1.HttpProtocolConfig\x12)\n\ntcp_config\x18\x1b \x01(\x0b\x32\x15.v1.TcpProtocolConfig\x12)\n\nudp_config\x18\x1c \x01(\x0b\x32\x15.v1.UdpProtocolConfig\x1aY\n\x12\x44\x65stinationService\x12\x0f\n\x07service\x18\x01 \x01(\t\x12\x11\n\tnamespace\x18\x02 \x01(\t\x12\x1f\n\x06method\x18\x03 \x01(\x0b\x32\x0f.v1.MatchString\"3\n\x08Protocol\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04HTTP\x10\x01\x12\x07\n\x03TCP\x10\x02\x12\x07\n\x03UDP\x10\x03J\x04\x08\x08\x10\x15\"\xa3\x01\n\x12HttpProtocolConfig\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\x35\n\x07headers\x18\x03 \x03(\x0b\x32$.v1.HttpProtocolConfig.MessageHeader\x12\x0c\n\x04\x62ody\x18\x04 \x01(\t\x1a+\n\rMessageHeader\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"2\n\x11TcpProtocolConfig\x12\x0c\n\x04send\x18\x01 \x01(\t\x12\x0f\n\x07receive\x18\x02 \x03(\t\"2\n\x11UdpProtocolConfig\x12\x0c\n\x04send\x18\x01 \x01(\t\x12\x0f\n\x07receive\x18\x02 \x03(\tB\x95\x01\n8com.tencent.polaris.specification.api.v1.fault.toleranceB\x12\x46\x61ultDetectorProtoZEgithub.com/polarismesh/specification/source/go/api/v1/fault_toleranceb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fault_detector_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fault_detector_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n8com.tencent.polaris.specification.api.v1.fault.toleranceB\022FaultDetectorProtoZEgithub.com/polarismesh/specification/source/go/api/v1/fault_tolerance'
-  _FAULTDETECTOR._serialized_start=41
-  _FAULTDETECTOR._serialized_end=110
-  _FAULTDETECTRULE._serialized_start=113
-  _FAULTDETECTRULE._serialized_end=686
-  _FAULTDETECTRULE_DESTINATIONSERVICE._serialized_start=538
-  _FAULTDETECTRULE_DESTINATIONSERVICE._serialized_end=627
-  _FAULTDETECTRULE_PROTOCOL._serialized_start=629
-  _FAULTDETECTRULE_PROTOCOL._serialized_end=680
-  _HTTPPROTOCOLCONFIG._serialized_start=689
-  _HTTPPROTOCOLCONFIG._serialized_end=852
-  _HTTPPROTOCOLCONFIG_MESSAGEHEADER._serialized_start=809
-  _HTTPPROTOCOLCONFIG_MESSAGEHEADER._serialized_end=852
-  _TCPPROTOCOLCONFIG._serialized_start=854
-  _TCPPROTOCOLCONFIG._serialized_end=904
-  _UDPPROTOCOLCONFIG._serialized_start=906
-  _UDPPROTOCOLCONFIG._serialized_end=956
+  _globals['_FAULTDETECTOR']._serialized_start=41
+  _globals['_FAULTDETECTOR']._serialized_end=110
+  _globals['_FAULTDETECTRULE']._serialized_start=113
+  _globals['_FAULTDETECTRULE']._serialized_end=686
+  _globals['_FAULTDETECTRULE_DESTINATIONSERVICE']._serialized_start=538
+  _globals['_FAULTDETECTRULE_DESTINATIONSERVICE']._serialized_end=627
+  _globals['_FAULTDETECTRULE_PROTOCOL']._serialized_start=629
+  _globals['_FAULTDETECTRULE_PROTOCOL']._serialized_end=680
+  _globals['_HTTPPROTOCOLCONFIG']._serialized_start=689
+  _globals['_HTTPPROTOCOLCONFIG']._serialized_end=852
+  _globals['_HTTPPROTOCOLCONFIG_MESSAGEHEADER']._serialized_start=809
+  _globals['_HTTPPROTOCOLCONFIG_MESSAGEHEADER']._serialized_end=852
+  _globals['_TCPPROTOCOLCONFIG']._serialized_start=854
+  _globals['_TCPPROTOCOLCONFIG']._serialized_end=904
+  _globals['_UDPPROTOCOLCONFIG']._serialized_start=906
+  _globals['_UDPPROTOCOLCONFIG']._serialized_end=956
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -3,98 +3,102 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
+class FaultDetector(_message.Message):
+    __slots__ = ["rules", "revision"]
+    RULES_FIELD_NUMBER: _ClassVar[int]
+    REVISION_FIELD_NUMBER: _ClassVar[int]
+    rules: _containers.RepeatedCompositeFieldContainer[FaultDetectRule]
+    revision: str
+    def __init__(self, rules: _Optional[_Iterable[_Union[FaultDetectRule, _Mapping]]] = ..., revision: _Optional[str] = ...) -> None: ...
+
 class FaultDetectRule(_message.Message):
-    __slots__ = ["ctime", "description", "http_config", "id", "interval", "mtime", "name", "namespace", "port", "protocol", "revision", "target_service", "tcp_config", "timeout", "udp_config"]
+    __slots__ = ["id", "name", "namespace", "revision", "ctime", "mtime", "description", "target_service", "interval", "timeout", "port", "protocol", "http_config", "tcp_config", "udp_config"]
     class Protocol(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        UNKNOWN: _ClassVar[FaultDetectRule.Protocol]
+        HTTP: _ClassVar[FaultDetectRule.Protocol]
+        TCP: _ClassVar[FaultDetectRule.Protocol]
+        UDP: _ClassVar[FaultDetectRule.Protocol]
+    UNKNOWN: FaultDetectRule.Protocol
+    HTTP: FaultDetectRule.Protocol
+    TCP: FaultDetectRule.Protocol
+    UDP: FaultDetectRule.Protocol
     class DestinationService(_message.Message):
-        __slots__ = ["method", "namespace", "service"]
-        METHOD_FIELD_NUMBER: _ClassVar[int]
-        NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+        __slots__ = ["service", "namespace", "method"]
         SERVICE_FIELD_NUMBER: _ClassVar[int]
-        method: _model_pb2.MatchString
-        namespace: str
+        NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+        METHOD_FIELD_NUMBER: _ClassVar[int]
         service: str
+        namespace: str
+        method: _model_pb2.MatchString
         def __init__(self, service: _Optional[str] = ..., namespace: _Optional[str] = ..., method: _Optional[_Union[_model_pb2.MatchString, _Mapping]] = ...) -> None: ...
+    ID_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    REVISION_FIELD_NUMBER: _ClassVar[int]
     CTIME_FIELD_NUMBER: _ClassVar[int]
+    MTIME_FIELD_NUMBER: _ClassVar[int]
     DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    HTTP: FaultDetectRule.Protocol
-    HTTP_CONFIG_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
+    TARGET_SERVICE_FIELD_NUMBER: _ClassVar[int]
     INTERVAL_FIELD_NUMBER: _ClassVar[int]
-    MTIME_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
+    TIMEOUT_FIELD_NUMBER: _ClassVar[int]
     PORT_FIELD_NUMBER: _ClassVar[int]
     PROTOCOL_FIELD_NUMBER: _ClassVar[int]
-    REVISION_FIELD_NUMBER: _ClassVar[int]
-    TARGET_SERVICE_FIELD_NUMBER: _ClassVar[int]
-    TCP: FaultDetectRule.Protocol
+    HTTP_CONFIG_FIELD_NUMBER: _ClassVar[int]
     TCP_CONFIG_FIELD_NUMBER: _ClassVar[int]
-    TIMEOUT_FIELD_NUMBER: _ClassVar[int]
-    UDP: FaultDetectRule.Protocol
     UDP_CONFIG_FIELD_NUMBER: _ClassVar[int]
-    UNKNOWN: FaultDetectRule.Protocol
-    ctime: str
-    description: str
-    http_config: HttpProtocolConfig
     id: str
-    interval: int
-    mtime: str
     name: str
     namespace: str
-    port: int
-    protocol: FaultDetectRule.Protocol
     revision: str
+    ctime: str
+    mtime: str
+    description: str
     target_service: FaultDetectRule.DestinationService
-    tcp_config: TcpProtocolConfig
+    interval: int
     timeout: int
+    port: int
+    protocol: FaultDetectRule.Protocol
+    http_config: HttpProtocolConfig
+    tcp_config: TcpProtocolConfig
     udp_config: UdpProtocolConfig
     def __init__(self, id: _Optional[str] = ..., name: _Optional[str] = ..., namespace: _Optional[str] = ..., revision: _Optional[str] = ..., ctime: _Optional[str] = ..., mtime: _Optional[str] = ..., description: _Optional[str] = ..., target_service: _Optional[_Union[FaultDetectRule.DestinationService, _Mapping]] = ..., interval: _Optional[int] = ..., timeout: _Optional[int] = ..., port: _Optional[int] = ..., protocol: _Optional[_Union[FaultDetectRule.Protocol, str]] = ..., http_config: _Optional[_Union[HttpProtocolConfig, _Mapping]] = ..., tcp_config: _Optional[_Union[TcpProtocolConfig, _Mapping]] = ..., udp_config: _Optional[_Union[UdpProtocolConfig, _Mapping]] = ...) -> None: ...
 
-class FaultDetector(_message.Message):
-    __slots__ = ["revision", "rules"]
-    REVISION_FIELD_NUMBER: _ClassVar[int]
-    RULES_FIELD_NUMBER: _ClassVar[int]
-    revision: str
-    rules: _containers.RepeatedCompositeFieldContainer[FaultDetectRule]
-    def __init__(self, rules: _Optional[_Iterable[_Union[FaultDetectRule, _Mapping]]] = ..., revision: _Optional[str] = ...) -> None: ...
-
 class HttpProtocolConfig(_message.Message):
-    __slots__ = ["body", "headers", "method", "url"]
+    __slots__ = ["method", "url", "headers", "body"]
     class MessageHeader(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
         def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
-    BODY_FIELD_NUMBER: _ClassVar[int]
-    HEADERS_FIELD_NUMBER: _ClassVar[int]
     METHOD_FIELD_NUMBER: _ClassVar[int]
     URL_FIELD_NUMBER: _ClassVar[int]
-    body: str
-    headers: _containers.RepeatedCompositeFieldContainer[HttpProtocolConfig.MessageHeader]
+    HEADERS_FIELD_NUMBER: _ClassVar[int]
+    BODY_FIELD_NUMBER: _ClassVar[int]
     method: str
     url: str
+    headers: _containers.RepeatedCompositeFieldContainer[HttpProtocolConfig.MessageHeader]
+    body: str
     def __init__(self, method: _Optional[str] = ..., url: _Optional[str] = ..., headers: _Optional[_Iterable[_Union[HttpProtocolConfig.MessageHeader, _Mapping]]] = ..., body: _Optional[str] = ...) -> None: ...
 
 class TcpProtocolConfig(_message.Message):
-    __slots__ = ["receive", "send"]
-    RECEIVE_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["send", "receive"]
     SEND_FIELD_NUMBER: _ClassVar[int]
-    receive: _containers.RepeatedScalarFieldContainer[str]
+    RECEIVE_FIELD_NUMBER: _ClassVar[int]
     send: str
+    receive: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, send: _Optional[str] = ..., receive: _Optional[_Iterable[str]] = ...) -> None: ...
 
 class UdpProtocolConfig(_message.Message):
-    __slots__ = ["receive", "send"]
-    RECEIVE_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["send", "receive"]
     SEND_FIELD_NUMBER: _ClassVar[int]
-    receive: _containers.RepeatedScalarFieldContainer[str]
+    RECEIVE_FIELD_NUMBER: _ClassVar[int]
     send: str
+    receive: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, send: _Optional[str] = ..., receive: _Optional[_Iterable[str]] = ...) -> None: ...
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/code_pb2.py` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/model/code_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: code.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\ncode.proto\x12\x02v1*\xa4%\n\x04\x43ode\x12\x0b\n\x07Unknown\x10\x00\x12\x14\n\x0e\x45xecuteSuccess\x10\xc0\x9a\x0c\x12\x12\n\x0c\x44\x61taNoChange\x10\xc1\x9a\x0c\x12\x12\n\x0cNoNeedUpdate\x10\xc2\x9a\x0c\x12\x10\n\nBadRequest\x10\x80\xb5\x18\x12\x14\n\x0eParseException\x10\x81\xb5\x18\x12\x12\n\x0c\x45mptyRequest\x10\x82\xb5\x18\x12\x18\n\x12\x42\x61tchSizeOverLimit\x10\x83\xb5\x18\x12\x1d\n\x17InvalidDiscoverResource\x10\x84\xb5\x18\x12\x16\n\x10InvalidRequestID\x10\xe4\xb5\x18\x12\x15\n\x0fInvalidUserName\x10\xe5\xb5\x18\x12\x16\n\x10InvalidUserToken\x10\xe6\xb5\x18\x12\x16\n\x10InvalidParameter\x10\xe7\xb5\x18\x12\x19\n\x13\x45mptyQueryParameter\x10\xe8\xb5\x18\x12\x1e\n\x18InvalidQueryInsParameter\x10\xe9\xb5\x18\x12\x1a\n\x14InvalidNamespaceName\x10\xee\xb5\x18\x12\x1c\n\x16InvalidNamespaceOwners\x10\xef\xb5\x18\x12\x1b\n\x15InvalidNamespaceToken\x10\xf0\xb5\x18\x12\x18\n\x12InvalidServiceName\x10\xf8\xb5\x18\x12\x1a\n\x14InvalidServiceOwners\x10\xf9\xb5\x18\x12\x19\n\x13InvalidServiceToken\x10\xfa\xb5\x18\x12\x1c\n\x16InvalidServiceMetadata\x10\xfb\xb5\x18\x12\x19\n\x13InvalidServicePorts\x10\xfc\xb5\x18\x12\x1c\n\x16InvalidServiceBusiness\x10\xfd\xb5\x18\x12\x1e\n\x18InvalidServiceDepartment\x10\xfe\xb5\x18\x12\x18\n\x12InvalidServiceCMDB\x10\xff\xb5\x18\x12\x1b\n\x15InvalidServiceComment\x10\x80\xb6\x18\x12 \n\x1aInvalidServiceAliasComment\x10\x81\xb6\x18\x12\x17\n\x11InvalidInstanceID\x10\x82\xb6\x18\x12\x19\n\x13InvalidInstanceHost\x10\x83\xb6\x18\x12\x19\n\x13InvalidInstancePort\x10\x84\xb6\x18\x12\x19\n\x13InvalidServiceAlias\x10\x85\xb6\x18\x12\x1f\n\x19InvalidNamespaceWithAlias\x10\x86\xb6\x18\x12\x1f\n\x19InvalidServiceAliasOwners\x10\x87\xb6\x18\x12\x1d\n\x17InvalidInstanceProtocol\x10\x88\xb6\x18\x12\x1c\n\x16InvalidInstanceVersion\x10\x89\xb6\x18\x12\x1d\n\x17InvalidInstanceLogicSet\x10\x8a\xb6\x18\x12\x1c\n\x16InvalidInstanceIsolate\x10\x8b\xb6\x18\x12\x18\n\x12HealthCheckNotOpen\x10\x8c\xb6\x18\x12\x1c\n\x16HeartbeatOnDisabledIns\x10\x8d\xb6\x18\x12\x1a\n\x14HeartbeatExceedLimit\x10\x8e\xb6\x18\x12\x1b\n\x15HeartbeatTypeNotFound\x10\x8f\xb6\x18\x12\x15\n\x0fInvalidMetadata\x10\x96\xb6\x18\x12\x18\n\x12InvalidRateLimitID\x10\x97\xb6\x18\x12\x1c\n\x16InvalidRateLimitLabels\x10\x98\xb6\x18\x12\x1d\n\x17InvalidRateLimitAmounts\x10\x99\xb6\x18\x12\x1a\n\x14InvalidRateLimitName\x10\x9a\xb6\x18\x12\x1d\n\x17InvalidCircuitBreakerID\x10\xa0\xb6\x18\x12\"\n\x1cInvalidCircuitBreakerVersion\x10\xa1\xb6\x18\x12\x1f\n\x19InvalidCircuitBreakerName\x10\xa2\xb6\x18\x12$\n\x1eInvalidCircuitBreakerNamespace\x10\xa3\xb6\x18\x12!\n\x1bInvalidCircuitBreakerOwners\x10\xa4\xb6\x18\x12 \n\x1aInvalidCircuitBreakerToken\x10\xa5\xb6\x18\x12#\n\x1dInvalidCircuitBreakerBusiness\x10\xa6\xb6\x18\x12%\n\x1fInvalidCircuitBreakerDepartment\x10\xa7\xb6\x18\x12\"\n\x1cInvalidCircuitBreakerComment\x10\xa8\xb6\x18\x12\x1f\n\x19\x43ircuitBreakerRuleExisted\x10\xa9\xb6\x18\x12\x16\n\x10InvalidRoutingID\x10\xbc\xba\x18\x12\x1a\n\x14InvalidRoutingPolicy\x10\xbd\xba\x18\x12\x18\n\x12InvalidRoutingName\x10\xbe\xba\x18\x12\x1c\n\x16InvalidRoutingPriority\x10\xbf\xba\x18\x12\x1a\n\x14InvalidFaultDetectID\x10\x84\xbc\x18\x12\x1c\n\x16InvalidFaultDetectName\x10\x85\xbc\x18\x12!\n\x1bInvalidFaultDetectNamespace\x10\x86\xbc\x18\x12\x1c\n\x16\x46\x61ultDetectRuleExisted\x10\x87\xbc\x18\x12\x19\n\x13ServicesExistedMesh\x10\xaa\xb6\x18\x12\x1a\n\x14ResourcesExistedMesh\x10\xab\xb6\x18\x12\x1a\n\x14InvalidMeshParameter\x10\xac\xb6\x18\x12\x17\n\x11InvalidPlatformID\x10\xb4\xb6\x18\x12\x19\n\x13InvalidPlatformName\x10\xb5\xb6\x18\x12\x1b\n\x15InvalidPlatformDomain\x10\xb6\xb6\x18\x12\x18\n\x12InvalidPlatformQPS\x10\xb7\xb6\x18\x12\x1a\n\x14InvalidPlatformToken\x10\xb8\xb6\x18\x12\x1a\n\x14InvalidPlatformOwner\x10\xb9\xb6\x18\x12\x1f\n\x19InvalidPlatformDepartment\x10\xba\xb6\x18\x12\x1c\n\x16InvalidPlatformComment\x10\xbb\xb6\x18\x12\x16\n\x10NotFoundPlatform\x10\xbc\xb6\x18\x12\x1c\n\x16InvalidFluxRateLimitId\x10\xbe\xb6\x18\x12\x1d\n\x17InvalidFluxRateLimitQps\x10\xbf\xb6\x18\x12 \n\x1aInvalidFluxRateLimitSetKey\x10\xc0\xb6\x18\x12\x15\n\x0f\x45xistedResource\x10\xc9\xb6\x18\x12\x16\n\x10NotFoundResource\x10\xca\xb6\x18\x12\x1e\n\x18NamespaceExistedServices\x10\xcb\xb6\x18\x12\x1d\n\x17ServiceExistedInstances\x10\xcc\xb6\x18\x12\x1c\n\x16ServiceExistedRoutings\x10\xcd\xb6\x18\x12\x1e\n\x18ServiceExistedRateLimits\x10\xce\xb6\x18\x12\x19\n\x13\x45xistReleasedConfig\x10\xcf\xb6\x18\x12\x19\n\x13SameInstanceRequest\x10\xd0\xb6\x18\x12#\n\x1dServiceExistedCircuitBreakers\x10\xd1\xb6\x18\x12\x19\n\x13ServiceExistedAlias\x10\xd2\xb6\x18\x12#\n\x1dNamespaceExistedMeshResources\x10\xd3\xb6\x18\x12%\n\x1fNamespaceExistedCircuitBreakers\x10\xd4\xb6\x18\x12\x1f\n\x19ServiceSubscribedByMeshes\x10\xd5\xb6\x18\x12\"\n\x1cServiceExistedFluxRateLimits\x10\xd6\xb6\x18\x12\"\n\x1cNamespaceExistedConfigGroups\x10\xdb\xb6\x18\x12\x15\n\x0fNotFoundService\x10\xad\xb7\x18\x12\x15\n\x0fNotFoundRouting\x10\xae\xb7\x18\x12\x16\n\x10NotFoundInstance\x10\xaf\xb7\x18\x12\x1a\n\x14NotFoundServiceAlias\x10\xb0\xb7\x18\x12\x17\n\x11NotFoundNamespace\x10\xb1\xb7\x18\x12\x1b\n\x15NotFoundSourceService\x10\xb2\xb7\x18\x12\x17\n\x11NotFoundRateLimit\x10\xb3\xb7\x18\x12\x1c\n\x16NotFoundCircuitBreaker\x10\xb4\xb7\x18\x12\x1a\n\x14NotFoundMasterConfig\x10\xb5\xb7\x18\x12\x17\n\x11NotFoundTagConfig\x10\xb6\xb7\x18\x12 \n\x1aNotFoundTagConfigOrService\x10\xb7\xb7\x18\x12\x16\n\x10\x43lientAPINotOpen\x10\x91\xb8\x18\x12\x1d\n\x17NotAllowBusinessService\x10\x92\xb8\x18\x12\x19\n\x13NotAllowAliasUpdate\x10\xf5\xb8\x18\x12!\n\x1bNotAllowAliasCreateInstance\x10\xf6\xb8\x18\x12 \n\x1aNotAllowAliasCreateRouting\x10\xf7\xb8\x18\x12!\n\x1bNotAllowCreateAliasForAlias\x10\xf8\xb8\x18\x12\"\n\x1cNotAllowAliasCreateRateLimit\x10\xf9\xb8\x18\x12\x1b\n\x15NotAllowAliasBindRule\x10\xfa\xb8\x18\x12(\n\"NotAllowDifferentNamespaceBindRule\x10\xfb\xb8\x18\x12\x12\n\x0cUnauthorized\x10\xe8\xbc\x18\x12\x16\n\x10NotAllowedAccess\x10\xe9\xbc\x18\x12\x15\n\x0f\x43MDBNotFindHost\x10\xa1\xd4\x18\x12\x12\n\x0c\x44\x61taConflict\x10\xa8\xfb\x18\x12\x1d\n\x17InstanceTooManyRequests\x10\xc9\x97\x1a\x12\x11\n\x0bIPRateLimit\x10\xca\x97\x1a\x12\x12\n\x0c\x41PIRateLimit\x10\xbb\xcc\x18\x12\x16\n\x10\x45xecuteException\x10\xa0\xc2\x1e\x12\x19\n\x13StoreLayerException\x10\xa1\xc2\x1e\x12\x19\n\x13\x43MDBPluginException\x10\xa2\xc2\x1e\x12\x1b\n\x15ParseRoutingException\x10\xa4\xc2\x1e\x12\x1d\n\x17ParseRateLimitException\x10\xa5\xc2\x1e\x12\"\n\x1cParseCircuitBreakerException\x10\xa6\xc2\x1e\x12\x18\n\x12HeartbeatException\x10\xa7\xc2\x1e\x12\x1a\n\x14InstanceRegisTimeout\x10\xa8\xc2\x1e\x12 \n\x1aInvalidConfigFileGroupName\x10\xa1\xbb\x18\x12\x1b\n\x15InvalidConfigFileName\x10\xa2\xbb\x18\x12$\n\x1eInvalidConfigFileContentLength\x10\xa3\xbb\x18\x12\x1d\n\x17InvalidConfigFileFormat\x10\xa4\xbb\x18\x12\x1b\n\x15InvalidConfigFileTags\x10\xa5\xbb\x18\x12\"\n\x1cInvalidWatchConfigFileFormat\x10\xa6\xbb\x18\x12 \n\x1aNotFoundResourceConfigFile\x10\xa7\xbb\x18\x12#\n\x1dInvalidConfigFileTemplateName\x10\xa8\xbb\x18\x12 \n\x1a\x45ncryptConfigFileException\x10\xa9\xbb\x18\x12 \n\x1a\x44\x65\x63ryptConfigFileException\x10\xaa\xbb\x18\x12\x17\n\x11InvalidUserOwners\x10\x9a\xb8\x18\x12\x13\n\rInvalidUserID\x10\x9b\xb8\x18\x12\x19\n\x13InvalidUserPassword\x10\x9c\xb8\x18\x12\x17\n\x11InvalidUserMobile\x10\x9d\xb8\x18\x12\x16\n\x10InvalidUserEmail\x10\x9e\xb8\x18\x12\x1c\n\x16InvalidUserGroupOwners\x10\xa4\xb8\x18\x12\x18\n\x12InvalidUserGroupID\x10\xa5\xb8\x18\x12\x1f\n\x19InvalidAuthStrategyOwners\x10\xae\xb8\x18\x12\x1d\n\x17InvalidAuthStrategyName\x10\xaf\xb8\x18\x12\x1b\n\x15InvalidAuthStrategyID\x10\xb0\xb8\x18\x12\x1a\n\x14InvalidPrincipalType\x10\xb8\xb8\x18\x12\x11\n\x0bUserExisted\x10\xd7\xb6\x18\x12\x16\n\x10UserGroupExisted\x10\xd8\xb6\x18\x12\x1d\n\x17\x41uthStrategyRuleExisted\x10\xd9\xb6\x18\x12\x17\n\x11SubAccountExisted\x10\xda\xb6\x18\x12\x12\n\x0cNotFoundUser\x10\xb8\xb7\x18\x12\x17\n\x11NotFoundOwnerUser\x10\xb9\xb7\x18\x12\x17\n\x11NotFoundUserGroup\x10\xba\xb7\x18\x12\x1e\n\x18NotFoundAuthStrategyRule\x10\xbb\xb7\x18\x12,\n&NotAllowModifyDefaultStrategyPrincipal\x10\xfc\xb8\x18\x12(\n\"NotAllowModifyOwnerDefaultStrategy\x10\xfd\xb8\x18\x12\x13\n\rEmptyAutToken\x10\xea\xbc\x18\x12\x13\n\rTokenDisabled\x10\xeb\xbc\x18\x12\x15\n\x0fTokenNotExisted\x10\xec\xbc\x18\x12\x18\n\x12\x41uthTokenForbidden\x10\xb9\xcc\x18\x12\x1c\n\x16OperationRoleForbidden\x10\xba\xcc\x18\x42x\n.com.tencent.polaris.specification.api.v1.modelB\tCodeProtoZ;github.com/polarismesh/specification/source/go/api/v1/modelb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'code_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'code_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n.com.tencent.polaris.specification.api.v1.modelB\tCodeProtoZ;github.com/polarismesh/specification/source/go/api/v1/model'
-  _CODE._serialized_start=19
-  _CODE._serialized_end=4791
+  _globals['_CODE']._serialized_start=19
+  _globals['_CODE']._serialized_end=4791
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/model_pb2.py` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/model/model_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: model.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0bmodel.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\"\x92\x01\n\x08Location\x12,\n\x06region\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04zone\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x63\x61mpus\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xb0\x02\n\x0bMatchString\x12-\n\x04type\x18\x01 \x01(\x0e\x32\x1f.v1.MatchString.MatchStringType\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x39\n\nvalue_type\x18\x03 \x01(\x0e\x32\x19.v1.MatchString.ValueTypeR\nvalue_type\"V\n\x0fMatchStringType\x12\t\n\x05\x45XACT\x10\x00\x12\t\n\x05REGEX\x10\x01\x12\x0e\n\nNOT_EQUALS\x10\x02\x12\x06\n\x02IN\x10\x03\x12\n\n\x06NOT_IN\x10\x04\x12\t\n\x05RANGE\x10\x05\"2\n\tValueType\x12\x08\n\x04TEXT\x10\x00\x12\r\n\tPARAMETER\x10\x01\x12\x0c\n\x08VARIABLE\x10\x02\"\x1c\n\nStringList\x12\x0e\n\x06values\x18\x01 \x03(\t\"\xb1\x01\n\x07Summary\x12\x30\n\x13total_service_count\x18\x01 \x01(\rR\x13total_service_count\x12@\n\x1btotal_health_instance_count\x18\x02 \x01(\rR\x1btotal_health_instance_count\x12\x32\n\x14total_instance_count\x18\x03 \x01(\rR\x14total_instance_countBy\n.com.tencent.polaris.specification.api.v1.modelB\nModelProtoZ;github.com/polarismesh/specification/source/go/api/v1/modelb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'model_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'model_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n.com.tencent.polaris.specification.api.v1.modelB\nModelProtoZ;github.com/polarismesh/specification/source/go/api/v1/model'
-  _LOCATION._serialized_start=52
-  _LOCATION._serialized_end=198
-  _MATCHSTRING._serialized_start=201
-  _MATCHSTRING._serialized_end=505
-  _MATCHSTRING_MATCHSTRINGTYPE._serialized_start=367
-  _MATCHSTRING_MATCHSTRINGTYPE._serialized_end=453
-  _MATCHSTRING_VALUETYPE._serialized_start=455
-  _MATCHSTRING_VALUETYPE._serialized_end=505
-  _STRINGLIST._serialized_start=507
-  _STRINGLIST._serialized_end=535
-  _SUMMARY._serialized_start=538
-  _SUMMARY._serialized_end=715
+  _globals['_LOCATION']._serialized_start=52
+  _globals['_LOCATION']._serialized_end=198
+  _globals['_MATCHSTRING']._serialized_start=201
+  _globals['_MATCHSTRING']._serialized_end=505
+  _globals['_MATCHSTRING_MATCHSTRINGTYPE']._serialized_start=367
+  _globals['_MATCHSTRING_MATCHSTRINGTYPE']._serialized_end=453
+  _globals['_MATCHSTRING_VALUETYPE']._serialized_start=455
+  _globals['_MATCHSTRING_VALUETYPE']._serialized_end=505
+  _globals['_STRINGLIST']._serialized_start=507
+  _globals['_STRINGLIST']._serialized_end=535
+  _globals['_SUMMARY']._serialized_start=538
+  _globals['_SUMMARY']._serialized_end=715
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/model_pb2.pyi` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/model/model_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -4,54 +4,63 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Location(_message.Message):
-    __slots__ = ["campus", "region", "zone"]
-    CAMPUS_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["region", "zone", "campus"]
     REGION_FIELD_NUMBER: _ClassVar[int]
     ZONE_FIELD_NUMBER: _ClassVar[int]
-    campus: _wrappers_pb2.StringValue
+    CAMPUS_FIELD_NUMBER: _ClassVar[int]
     region: _wrappers_pb2.StringValue
     zone: _wrappers_pb2.StringValue
+    campus: _wrappers_pb2.StringValue
     def __init__(self, region: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., zone: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., campus: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
 
 class MatchString(_message.Message):
     __slots__ = ["type", "value", "value_type"]
     class MatchStringType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
-    class ValueType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
+        EXACT: _ClassVar[MatchString.MatchStringType]
+        REGEX: _ClassVar[MatchString.MatchStringType]
+        NOT_EQUALS: _ClassVar[MatchString.MatchStringType]
+        IN: _ClassVar[MatchString.MatchStringType]
+        NOT_IN: _ClassVar[MatchString.MatchStringType]
+        RANGE: _ClassVar[MatchString.MatchStringType]
     EXACT: MatchString.MatchStringType
-    IN: MatchString.MatchStringType
+    REGEX: MatchString.MatchStringType
     NOT_EQUALS: MatchString.MatchStringType
+    IN: MatchString.MatchStringType
     NOT_IN: MatchString.MatchStringType
-    PARAMETER: MatchString.ValueType
     RANGE: MatchString.MatchStringType
-    REGEX: MatchString.MatchStringType
+    class ValueType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        TEXT: _ClassVar[MatchString.ValueType]
+        PARAMETER: _ClassVar[MatchString.ValueType]
+        VARIABLE: _ClassVar[MatchString.ValueType]
     TEXT: MatchString.ValueType
+    PARAMETER: MatchString.ValueType
+    VARIABLE: MatchString.ValueType
     TYPE_FIELD_NUMBER: _ClassVar[int]
     VALUE_FIELD_NUMBER: _ClassVar[int]
     VALUE_TYPE_FIELD_NUMBER: _ClassVar[int]
-    VARIABLE: MatchString.ValueType
     type: MatchString.MatchStringType
     value: _wrappers_pb2.StringValue
     value_type: MatchString.ValueType
     def __init__(self, type: _Optional[_Union[MatchString.MatchStringType, str]] = ..., value: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., value_type: _Optional[_Union[MatchString.ValueType, str]] = ...) -> None: ...
 
 class StringList(_message.Message):
     __slots__ = ["values"]
     VALUES_FIELD_NUMBER: _ClassVar[int]
     values: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, values: _Optional[_Iterable[str]] = ...) -> None: ...
 
 class Summary(_message.Message):
-    __slots__ = ["total_health_instance_count", "total_instance_count", "total_service_count"]
+    __slots__ = ["total_service_count", "total_health_instance_count", "total_instance_count"]
+    TOTAL_SERVICE_COUNT_FIELD_NUMBER: _ClassVar[int]
     TOTAL_HEALTH_INSTANCE_COUNT_FIELD_NUMBER: _ClassVar[int]
     TOTAL_INSTANCE_COUNT_FIELD_NUMBER: _ClassVar[int]
-    TOTAL_SERVICE_COUNT_FIELD_NUMBER: _ClassVar[int]
+    total_service_count: int
     total_health_instance_count: int
     total_instance_count: int
-    total_service_count: int
     def __init__(self, total_service_count: _Optional[int] = ..., total_health_instance_count: _Optional[int] = ..., total_instance_count: _Optional[int] = ...) -> None: ...
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/namespace_pb2.py` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/model/namespace_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: namespace.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fnamespace.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\"\xfd\x06\n\tNamespace\x12*\n\x04name\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06owners\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05token\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05\x63time\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05mtime\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12N\n\x13total_service_count\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.UInt32ValueR\x13total_service_count\x12^\n\x1btotal_health_instance_count\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.UInt32ValueR\x1btotal_health_instance_count\x12P\n\x14total_instance_count\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt32ValueR\x14total_instance_count\x12\x38\n\x08user_ids\x18\n \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x08user_ids\x12:\n\tgroup_ids\x18\x0b \x03(\x0b\x32\x1c.google.protobuf.StringValueR\tgroup_ids\x12\x46\n\x0fremove_user_ids\x18\r \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x0fremove_user_ids\x12H\n\x10remove_group_ids\x18\x0e \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x10remove_group_ids\x12(\n\x02id\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x08\x65\x64itable\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.BoolValueB}\n.com.tencent.polaris.specification.api.v1.modelB\x0eNamespaceProtoZ;github.com/polarismesh/specification/source/go/api/v1/modelb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'namespace_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'namespace_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n.com.tencent.polaris.specification.api.v1.modelB\016NamespaceProtoZ;github.com/polarismesh/specification/source/go/api/v1/model'
-  _NAMESPACE._serialized_start=56
-  _NAMESPACE._serialized_end=949
+  _globals['_NAMESPACE']._serialized_start=56
+  _globals['_NAMESPACE']._serialized_end=949
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -3,39 +3,39 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Namespace(_message.Message):
-    __slots__ = ["comment", "ctime", "editable", "group_ids", "id", "mtime", "name", "owners", "remove_group_ids", "remove_user_ids", "token", "total_health_instance_count", "total_instance_count", "total_service_count", "user_ids"]
-    COMMENT_FIELD_NUMBER: _ClassVar[int]
-    CTIME_FIELD_NUMBER: _ClassVar[int]
-    EDITABLE_FIELD_NUMBER: _ClassVar[int]
-    GROUP_IDS_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    MTIME_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["name", "comment", "owners", "token", "ctime", "mtime", "total_service_count", "total_health_instance_count", "total_instance_count", "user_ids", "group_ids", "remove_user_ids", "remove_group_ids", "id", "editable"]
     NAME_FIELD_NUMBER: _ClassVar[int]
+    COMMENT_FIELD_NUMBER: _ClassVar[int]
     OWNERS_FIELD_NUMBER: _ClassVar[int]
-    REMOVE_GROUP_IDS_FIELD_NUMBER: _ClassVar[int]
-    REMOVE_USER_IDS_FIELD_NUMBER: _ClassVar[int]
     TOKEN_FIELD_NUMBER: _ClassVar[int]
+    CTIME_FIELD_NUMBER: _ClassVar[int]
+    MTIME_FIELD_NUMBER: _ClassVar[int]
+    TOTAL_SERVICE_COUNT_FIELD_NUMBER: _ClassVar[int]
     TOTAL_HEALTH_INSTANCE_COUNT_FIELD_NUMBER: _ClassVar[int]
     TOTAL_INSTANCE_COUNT_FIELD_NUMBER: _ClassVar[int]
-    TOTAL_SERVICE_COUNT_FIELD_NUMBER: _ClassVar[int]
     USER_IDS_FIELD_NUMBER: _ClassVar[int]
-    comment: _wrappers_pb2.StringValue
-    ctime: _wrappers_pb2.StringValue
-    editable: _wrappers_pb2.BoolValue
-    group_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
-    id: _wrappers_pb2.StringValue
-    mtime: _wrappers_pb2.StringValue
+    GROUP_IDS_FIELD_NUMBER: _ClassVar[int]
+    REMOVE_USER_IDS_FIELD_NUMBER: _ClassVar[int]
+    REMOVE_GROUP_IDS_FIELD_NUMBER: _ClassVar[int]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    EDITABLE_FIELD_NUMBER: _ClassVar[int]
     name: _wrappers_pb2.StringValue
+    comment: _wrappers_pb2.StringValue
     owners: _wrappers_pb2.StringValue
-    remove_group_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
-    remove_user_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
     token: _wrappers_pb2.StringValue
+    ctime: _wrappers_pb2.StringValue
+    mtime: _wrappers_pb2.StringValue
+    total_service_count: _wrappers_pb2.UInt32Value
     total_health_instance_count: _wrappers_pb2.UInt32Value
     total_instance_count: _wrappers_pb2.UInt32Value
-    total_service_count: _wrappers_pb2.UInt32Value
     user_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
+    group_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
+    remove_user_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
+    remove_group_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
+    id: _wrappers_pb2.StringValue
+    editable: _wrappers_pb2.BoolValue
     def __init__(self, name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., owners: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., token: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., ctime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mtime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., total_service_count: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., total_health_instance_count: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., total_instance_count: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., user_ids: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ..., group_ids: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ..., remove_user_ids: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ..., remove_group_ids: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ..., id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., editable: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...) -> None: ...
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/security/auth_pb2.py` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/security/auth_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: auth.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nauth.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\"\x97\x01\n\x0cLoginRequest\x12+\n\x05owner\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\x08password\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\x86\x02\n\rLoginResponse\x12\x36\n\x07user_id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x07user_id\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04role\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x38\n\x08owner_id\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x08owner_id\x12+\n\x05token\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\x85\x05\n\x04User\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\x08password\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05owner\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06source\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12<\n\nauth_token\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\nauth_token\x12>\n\x0ctoken_enable\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x0ctoken_enable\x12-\n\x07\x63omment\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05\x63time\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05mtime\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12:\n\tuser_type\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValueR\tuser_type\x12,\n\x06mobile\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05\x65mail\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xc2\x01\n\x12ModifyUserPassword\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12@\n\x0cold_password\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x0cold_password\x12@\n\x0cnew_password\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x0cnew_password\"f\n\x11UserGroupRelation\x12\x38\n\x08group_id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x08group_id\x12\x17\n\x05users\x18\x02 \x03(\x0b\x32\x08.v1.User\"\xfc\x03\n\tUserGroup\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05owner\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12<\n\nauth_token\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\nauth_token\x12>\n\x0ctoken_enable\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x0ctoken_enable\x12-\n\x07\x63omment\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05\x63time\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05mtime\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\'\n\x08relation\x18\t \x01(\x0b\x32\x15.v1.UserGroupRelation\x12<\n\nuser_count\x18\n \x01(\x0b\x32\x1c.google.protobuf.UInt32ValueR\nuser_count\"\xc1\x03\n\x0fModifyUserGroup\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05owner\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04name\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12<\n\nauth_token\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\nauth_token\x12>\n\x0ctoken_enable\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x0ctoken_enable\x12-\n\x07\x63omment\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12;\n\radd_relations\x18\x07 \x01(\x0b\x32\x15.v1.UserGroupRelationR\radd_relations\x12\x41\n\x10remove_relations\x18\x08 \x01(\x0b\x32\x15.v1.UserGroupRelationR\x10remove_relations\"a\n\tPrincipal\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"I\n\nPrincipals\x12\x1c\n\x05users\x18\x01 \x03(\x0b\x32\r.v1.Principal\x12\x1d\n\x06groups\x18\x02 \x03(\x0b\x32\r.v1.Principal\"\x9e\x01\n\x15StrategyResourceEntry\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04name\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xf0\x01\n\x11StrategyResources\x12>\n\x0bstrategy_id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x0bstrategy_id\x12-\n\nnamespaces\x18\x02 \x03(\x0b\x32\x19.v1.StrategyResourceEntry\x12+\n\x08services\x18\x03 \x03(\x0b\x32\x19.v1.StrategyResourceEntry\x12?\n\rconfig_groups\x18\x04 \x03(\x0b\x32\x19.v1.StrategyResourceEntryR\rconfig_groups\"\x8e\x04\n\x0c\x41uthStrategy\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\"\n\nprincipals\x18\x03 \x01(\x0b\x32\x0e.v1.Principals\x12(\n\tresources\x18\x04 \x01(\x0b\x32\x15.v1.StrategyResources\x12\x1e\n\x06\x61\x63tion\x18\x05 \x01(\x0e\x32\x0e.v1.AuthAction\x12-\n\x07\x63omment\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05owner\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05\x63time\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05mtime\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12<\n\nauth_token\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValueR\nauth_token\x12\x46\n\x10\x64\x65\x66\x61ult_strategy\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x10\x64\x65\x66\x61ult_strategy\"\xdc\x03\n\x12ModifyAuthStrategy\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x36\n\x0e\x61\x64\x64_principals\x18\x03 \x01(\x0b\x32\x0e.v1.PrincipalsR\x0e\x61\x64\x64_principals\x12<\n\x11remove_principals\x18\x04 \x01(\x0b\x32\x0e.v1.PrincipalsR\x11remove_principals\x12;\n\radd_resources\x18\x05 \x01(\x0b\x32\x15.v1.StrategyResourcesR\radd_resources\x12\x41\n\x10remove_resources\x18\x06 \x01(\x0b\x32\x15.v1.StrategyResourcesR\x10remove_resources\x12\x1e\n\x06\x61\x63tion\x18\x07 \x01(\x0e\x32\x0e.v1.AuthAction\x12-\n\x07\x63omment\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05owner\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue*+\n\nAuthAction\x12\r\n\tONLY_READ\x10\x00\x12\x0e\n\nREAD_WRITE\x10\x01*>\n\x0cResourceType\x12\x0e\n\nNamespaces\x10\x00\x12\x0c\n\x08Services\x10\x01\x12\x10\n\x0c\x43onfigGroups\x10\x02\x42\x82\x01\n1com.tencent.polaris.specification.api.v1.securityB\rSecurityProtoZ>github.com/polarismesh/specification/source/go/api/v1/securityb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'auth_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'auth_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n1com.tencent.polaris.specification.api.v1.securityB\rSecurityProtoZ>github.com/polarismesh/specification/source/go/api/v1/security'
-  _AUTHACTION._serialized_start=3967
-  _AUTHACTION._serialized_end=4010
-  _RESOURCETYPE._serialized_start=4012
-  _RESOURCETYPE._serialized_end=4074
-  _LOGINREQUEST._serialized_start=51
-  _LOGINREQUEST._serialized_end=202
-  _LOGINRESPONSE._serialized_start=205
-  _LOGINRESPONSE._serialized_end=467
-  _USER._serialized_start=470
-  _USER._serialized_end=1115
-  _MODIFYUSERPASSWORD._serialized_start=1118
-  _MODIFYUSERPASSWORD._serialized_end=1312
-  _USERGROUPRELATION._serialized_start=1314
-  _USERGROUPRELATION._serialized_end=1416
-  _USERGROUP._serialized_start=1419
-  _USERGROUP._serialized_end=1927
-  _MODIFYUSERGROUP._serialized_start=1930
-  _MODIFYUSERGROUP._serialized_end=2379
-  _PRINCIPAL._serialized_start=2381
-  _PRINCIPAL._serialized_end=2478
-  _PRINCIPALS._serialized_start=2480
-  _PRINCIPALS._serialized_end=2553
-  _STRATEGYRESOURCEENTRY._serialized_start=2556
-  _STRATEGYRESOURCEENTRY._serialized_end=2714
-  _STRATEGYRESOURCES._serialized_start=2717
-  _STRATEGYRESOURCES._serialized_end=2957
-  _AUTHSTRATEGY._serialized_start=2960
-  _AUTHSTRATEGY._serialized_end=3486
-  _MODIFYAUTHSTRATEGY._serialized_start=3489
-  _MODIFYAUTHSTRATEGY._serialized_end=3965
+  _globals['_AUTHACTION']._serialized_start=3967
+  _globals['_AUTHACTION']._serialized_end=4010
+  _globals['_RESOURCETYPE']._serialized_start=4012
+  _globals['_RESOURCETYPE']._serialized_end=4074
+  _globals['_LOGINREQUEST']._serialized_start=51
+  _globals['_LOGINREQUEST']._serialized_end=202
+  _globals['_LOGINRESPONSE']._serialized_start=205
+  _globals['_LOGINRESPONSE']._serialized_end=467
+  _globals['_USER']._serialized_start=470
+  _globals['_USER']._serialized_end=1115
+  _globals['_MODIFYUSERPASSWORD']._serialized_start=1118
+  _globals['_MODIFYUSERPASSWORD']._serialized_end=1312
+  _globals['_USERGROUPRELATION']._serialized_start=1314
+  _globals['_USERGROUPRELATION']._serialized_end=1416
+  _globals['_USERGROUP']._serialized_start=1419
+  _globals['_USERGROUP']._serialized_end=1927
+  _globals['_MODIFYUSERGROUP']._serialized_start=1930
+  _globals['_MODIFYUSERGROUP']._serialized_end=2379
+  _globals['_PRINCIPAL']._serialized_start=2381
+  _globals['_PRINCIPAL']._serialized_end=2478
+  _globals['_PRINCIPALS']._serialized_start=2480
+  _globals['_PRINCIPALS']._serialized_end=2553
+  _globals['_STRATEGYRESOURCEENTRY']._serialized_start=2556
+  _globals['_STRATEGYRESOURCEENTRY']._serialized_end=2714
+  _globals['_STRATEGYRESOURCES']._serialized_start=2717
+  _globals['_STRATEGYRESOURCES']._serialized_end=2957
+  _globals['_AUTHSTRATEGY']._serialized_start=2960
+  _globals['_AUTHSTRATEGY']._serialized_end=3486
+  _globals['_MODIFYAUTHSTRATEGY']._serialized_start=3489
+  _globals['_MODIFYAUTHSTRATEGY']._serialized_end=3965
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/security/auth_pb2.pyi` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/security/auth_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,221 +1,226 @@
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
-ConfigGroups: ResourceType
 DESCRIPTOR: _descriptor.FileDescriptor
-Namespaces: ResourceType
+
+class AuthAction(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    ONLY_READ: _ClassVar[AuthAction]
+    READ_WRITE: _ClassVar[AuthAction]
+
+class ResourceType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    Namespaces: _ClassVar[ResourceType]
+    Services: _ClassVar[ResourceType]
+    ConfigGroups: _ClassVar[ResourceType]
 ONLY_READ: AuthAction
 READ_WRITE: AuthAction
+Namespaces: ResourceType
 Services: ResourceType
-
-class AuthStrategy(_message.Message):
-    __slots__ = ["action", "auth_token", "comment", "ctime", "default_strategy", "id", "mtime", "name", "owner", "principals", "resources"]
-    ACTION_FIELD_NUMBER: _ClassVar[int]
-    AUTH_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    COMMENT_FIELD_NUMBER: _ClassVar[int]
-    CTIME_FIELD_NUMBER: _ClassVar[int]
-    DEFAULT_STRATEGY_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    MTIME_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    OWNER_FIELD_NUMBER: _ClassVar[int]
-    PRINCIPALS_FIELD_NUMBER: _ClassVar[int]
-    RESOURCES_FIELD_NUMBER: _ClassVar[int]
-    action: AuthAction
-    auth_token: _wrappers_pb2.StringValue
-    comment: _wrappers_pb2.StringValue
-    ctime: _wrappers_pb2.StringValue
-    default_strategy: _wrappers_pb2.BoolValue
-    id: _wrappers_pb2.StringValue
-    mtime: _wrappers_pb2.StringValue
-    name: _wrappers_pb2.StringValue
-    owner: _wrappers_pb2.StringValue
-    principals: Principals
-    resources: StrategyResources
-    def __init__(self, id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., principals: _Optional[_Union[Principals, _Mapping]] = ..., resources: _Optional[_Union[StrategyResources, _Mapping]] = ..., action: _Optional[_Union[AuthAction, str]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., owner: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., ctime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mtime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., auth_token: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., default_strategy: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...) -> None: ...
+ConfigGroups: ResourceType
 
 class LoginRequest(_message.Message):
-    __slots__ = ["name", "owner", "password"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["owner", "name", "password"]
     OWNER_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
     PASSWORD_FIELD_NUMBER: _ClassVar[int]
-    name: _wrappers_pb2.StringValue
     owner: _wrappers_pb2.StringValue
+    name: _wrappers_pb2.StringValue
     password: _wrappers_pb2.StringValue
     def __init__(self, owner: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., password: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
 
 class LoginResponse(_message.Message):
-    __slots__ = ["name", "owner_id", "role", "token", "user_id"]
+    __slots__ = ["user_id", "name", "role", "owner_id", "token"]
+    USER_ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    OWNER_ID_FIELD_NUMBER: _ClassVar[int]
     ROLE_FIELD_NUMBER: _ClassVar[int]
+    OWNER_ID_FIELD_NUMBER: _ClassVar[int]
     TOKEN_FIELD_NUMBER: _ClassVar[int]
-    USER_ID_FIELD_NUMBER: _ClassVar[int]
+    user_id: _wrappers_pb2.StringValue
     name: _wrappers_pb2.StringValue
-    owner_id: _wrappers_pb2.StringValue
     role: _wrappers_pb2.StringValue
+    owner_id: _wrappers_pb2.StringValue
     token: _wrappers_pb2.StringValue
-    user_id: _wrappers_pb2.StringValue
     def __init__(self, user_id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., role: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., owner_id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., token: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
 
-class ModifyAuthStrategy(_message.Message):
-    __slots__ = ["action", "add_principals", "add_resources", "comment", "id", "name", "owner", "remove_principals", "remove_resources"]
-    ACTION_FIELD_NUMBER: _ClassVar[int]
-    ADD_PRINCIPALS_FIELD_NUMBER: _ClassVar[int]
-    ADD_RESOURCES_FIELD_NUMBER: _ClassVar[int]
-    COMMENT_FIELD_NUMBER: _ClassVar[int]
+class User(_message.Message):
+    __slots__ = ["id", "name", "password", "owner", "source", "auth_token", "token_enable", "comment", "ctime", "mtime", "user_type", "mobile", "email"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
+    PASSWORD_FIELD_NUMBER: _ClassVar[int]
     OWNER_FIELD_NUMBER: _ClassVar[int]
-    REMOVE_PRINCIPALS_FIELD_NUMBER: _ClassVar[int]
-    REMOVE_RESOURCES_FIELD_NUMBER: _ClassVar[int]
-    action: AuthAction
-    add_principals: Principals
-    add_resources: StrategyResources
-    comment: _wrappers_pb2.StringValue
+    SOURCE_FIELD_NUMBER: _ClassVar[int]
+    AUTH_TOKEN_FIELD_NUMBER: _ClassVar[int]
+    TOKEN_ENABLE_FIELD_NUMBER: _ClassVar[int]
+    COMMENT_FIELD_NUMBER: _ClassVar[int]
+    CTIME_FIELD_NUMBER: _ClassVar[int]
+    MTIME_FIELD_NUMBER: _ClassVar[int]
+    USER_TYPE_FIELD_NUMBER: _ClassVar[int]
+    MOBILE_FIELD_NUMBER: _ClassVar[int]
+    EMAIL_FIELD_NUMBER: _ClassVar[int]
     id: _wrappers_pb2.StringValue
     name: _wrappers_pb2.StringValue
+    password: _wrappers_pb2.StringValue
     owner: _wrappers_pb2.StringValue
-    remove_principals: Principals
-    remove_resources: StrategyResources
-    def __init__(self, id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., add_principals: _Optional[_Union[Principals, _Mapping]] = ..., remove_principals: _Optional[_Union[Principals, _Mapping]] = ..., add_resources: _Optional[_Union[StrategyResources, _Mapping]] = ..., remove_resources: _Optional[_Union[StrategyResources, _Mapping]] = ..., action: _Optional[_Union[AuthAction, str]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., owner: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
+    source: _wrappers_pb2.StringValue
+    auth_token: _wrappers_pb2.StringValue
+    token_enable: _wrappers_pb2.BoolValue
+    comment: _wrappers_pb2.StringValue
+    ctime: _wrappers_pb2.StringValue
+    mtime: _wrappers_pb2.StringValue
+    user_type: _wrappers_pb2.StringValue
+    mobile: _wrappers_pb2.StringValue
+    email: _wrappers_pb2.StringValue
+    def __init__(self, id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., password: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., owner: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., source: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., auth_token: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., token_enable: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., ctime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mtime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., user_type: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mobile: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., email: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
 
-class ModifyUserGroup(_message.Message):
-    __slots__ = ["add_relations", "auth_token", "comment", "id", "name", "owner", "remove_relations", "token_enable"]
-    ADD_RELATIONS_FIELD_NUMBER: _ClassVar[int]
-    AUTH_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    COMMENT_FIELD_NUMBER: _ClassVar[int]
+class ModifyUserPassword(_message.Message):
+    __slots__ = ["id", "old_password", "new_password"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    OLD_PASSWORD_FIELD_NUMBER: _ClassVar[int]
+    NEW_PASSWORD_FIELD_NUMBER: _ClassVar[int]
+    id: _wrappers_pb2.StringValue
+    old_password: _wrappers_pb2.StringValue
+    new_password: _wrappers_pb2.StringValue
+    def __init__(self, id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., old_password: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., new_password: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
+
+class UserGroupRelation(_message.Message):
+    __slots__ = ["group_id", "users"]
+    GROUP_ID_FIELD_NUMBER: _ClassVar[int]
+    USERS_FIELD_NUMBER: _ClassVar[int]
+    group_id: _wrappers_pb2.StringValue
+    users: _containers.RepeatedCompositeFieldContainer[User]
+    def __init__(self, group_id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., users: _Optional[_Iterable[_Union[User, _Mapping]]] = ...) -> None: ...
+
+class UserGroup(_message.Message):
+    __slots__ = ["id", "name", "owner", "auth_token", "token_enable", "comment", "ctime", "mtime", "relation", "user_count"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     OWNER_FIELD_NUMBER: _ClassVar[int]
-    REMOVE_RELATIONS_FIELD_NUMBER: _ClassVar[int]
+    AUTH_TOKEN_FIELD_NUMBER: _ClassVar[int]
     TOKEN_ENABLE_FIELD_NUMBER: _ClassVar[int]
-    add_relations: UserGroupRelation
-    auth_token: _wrappers_pb2.StringValue
-    comment: _wrappers_pb2.StringValue
+    COMMENT_FIELD_NUMBER: _ClassVar[int]
+    CTIME_FIELD_NUMBER: _ClassVar[int]
+    MTIME_FIELD_NUMBER: _ClassVar[int]
+    RELATION_FIELD_NUMBER: _ClassVar[int]
+    USER_COUNT_FIELD_NUMBER: _ClassVar[int]
     id: _wrappers_pb2.StringValue
     name: _wrappers_pb2.StringValue
     owner: _wrappers_pb2.StringValue
-    remove_relations: UserGroupRelation
+    auth_token: _wrappers_pb2.StringValue
     token_enable: _wrappers_pb2.BoolValue
-    def __init__(self, id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., owner: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., auth_token: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., token_enable: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., add_relations: _Optional[_Union[UserGroupRelation, _Mapping]] = ..., remove_relations: _Optional[_Union[UserGroupRelation, _Mapping]] = ...) -> None: ...
+    comment: _wrappers_pb2.StringValue
+    ctime: _wrappers_pb2.StringValue
+    mtime: _wrappers_pb2.StringValue
+    relation: UserGroupRelation
+    user_count: _wrappers_pb2.UInt32Value
+    def __init__(self, id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., owner: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., auth_token: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., token_enable: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., ctime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mtime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., relation: _Optional[_Union[UserGroupRelation, _Mapping]] = ..., user_count: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ...) -> None: ...
 
-class ModifyUserPassword(_message.Message):
-    __slots__ = ["id", "new_password", "old_password"]
+class ModifyUserGroup(_message.Message):
+    __slots__ = ["id", "owner", "name", "auth_token", "token_enable", "comment", "add_relations", "remove_relations"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    NEW_PASSWORD_FIELD_NUMBER: _ClassVar[int]
-    OLD_PASSWORD_FIELD_NUMBER: _ClassVar[int]
+    OWNER_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    AUTH_TOKEN_FIELD_NUMBER: _ClassVar[int]
+    TOKEN_ENABLE_FIELD_NUMBER: _ClassVar[int]
+    COMMENT_FIELD_NUMBER: _ClassVar[int]
+    ADD_RELATIONS_FIELD_NUMBER: _ClassVar[int]
+    REMOVE_RELATIONS_FIELD_NUMBER: _ClassVar[int]
     id: _wrappers_pb2.StringValue
-    new_password: _wrappers_pb2.StringValue
-    old_password: _wrappers_pb2.StringValue
-    def __init__(self, id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., old_password: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., new_password: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
+    owner: _wrappers_pb2.StringValue
+    name: _wrappers_pb2.StringValue
+    auth_token: _wrappers_pb2.StringValue
+    token_enable: _wrappers_pb2.BoolValue
+    comment: _wrappers_pb2.StringValue
+    add_relations: UserGroupRelation
+    remove_relations: UserGroupRelation
+    def __init__(self, id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., owner: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., auth_token: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., token_enable: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., add_relations: _Optional[_Union[UserGroupRelation, _Mapping]] = ..., remove_relations: _Optional[_Union[UserGroupRelation, _Mapping]] = ...) -> None: ...
 
 class Principal(_message.Message):
     __slots__ = ["id", "name"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     id: _wrappers_pb2.StringValue
     name: _wrappers_pb2.StringValue
     def __init__(self, id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
 
 class Principals(_message.Message):
-    __slots__ = ["groups", "users"]
-    GROUPS_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["users", "groups"]
     USERS_FIELD_NUMBER: _ClassVar[int]
-    groups: _containers.RepeatedCompositeFieldContainer[Principal]
+    GROUPS_FIELD_NUMBER: _ClassVar[int]
     users: _containers.RepeatedCompositeFieldContainer[Principal]
+    groups: _containers.RepeatedCompositeFieldContainer[Principal]
     def __init__(self, users: _Optional[_Iterable[_Union[Principal, _Mapping]]] = ..., groups: _Optional[_Iterable[_Union[Principal, _Mapping]]] = ...) -> None: ...
 
 class StrategyResourceEntry(_message.Message):
-    __slots__ = ["id", "name", "namespace"]
+    __slots__ = ["id", "namespace", "name"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAMESPACE_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     id: _wrappers_pb2.StringValue
-    name: _wrappers_pb2.StringValue
     namespace: _wrappers_pb2.StringValue
+    name: _wrappers_pb2.StringValue
     def __init__(self, id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
 
 class StrategyResources(_message.Message):
-    __slots__ = ["config_groups", "namespaces", "services", "strategy_id"]
-    CONFIG_GROUPS_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["strategy_id", "namespaces", "services", "config_groups"]
+    STRATEGY_ID_FIELD_NUMBER: _ClassVar[int]
     NAMESPACES_FIELD_NUMBER: _ClassVar[int]
     SERVICES_FIELD_NUMBER: _ClassVar[int]
-    STRATEGY_ID_FIELD_NUMBER: _ClassVar[int]
-    config_groups: _containers.RepeatedCompositeFieldContainer[StrategyResourceEntry]
+    CONFIG_GROUPS_FIELD_NUMBER: _ClassVar[int]
+    strategy_id: _wrappers_pb2.StringValue
     namespaces: _containers.RepeatedCompositeFieldContainer[StrategyResourceEntry]
     services: _containers.RepeatedCompositeFieldContainer[StrategyResourceEntry]
-    strategy_id: _wrappers_pb2.StringValue
+    config_groups: _containers.RepeatedCompositeFieldContainer[StrategyResourceEntry]
     def __init__(self, strategy_id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespaces: _Optional[_Iterable[_Union[StrategyResourceEntry, _Mapping]]] = ..., services: _Optional[_Iterable[_Union[StrategyResourceEntry, _Mapping]]] = ..., config_groups: _Optional[_Iterable[_Union[StrategyResourceEntry, _Mapping]]] = ...) -> None: ...
 
-class User(_message.Message):
-    __slots__ = ["auth_token", "comment", "ctime", "email", "id", "mobile", "mtime", "name", "owner", "password", "source", "token_enable", "user_type"]
-    AUTH_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    COMMENT_FIELD_NUMBER: _ClassVar[int]
-    CTIME_FIELD_NUMBER: _ClassVar[int]
-    EMAIL_FIELD_NUMBER: _ClassVar[int]
+class AuthStrategy(_message.Message):
+    __slots__ = ["id", "name", "principals", "resources", "action", "comment", "owner", "ctime", "mtime", "auth_token", "default_strategy"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    MOBILE_FIELD_NUMBER: _ClassVar[int]
-    MTIME_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
+    PRINCIPALS_FIELD_NUMBER: _ClassVar[int]
+    RESOURCES_FIELD_NUMBER: _ClassVar[int]
+    ACTION_FIELD_NUMBER: _ClassVar[int]
+    COMMENT_FIELD_NUMBER: _ClassVar[int]
     OWNER_FIELD_NUMBER: _ClassVar[int]
-    PASSWORD_FIELD_NUMBER: _ClassVar[int]
-    SOURCE_FIELD_NUMBER: _ClassVar[int]
-    TOKEN_ENABLE_FIELD_NUMBER: _ClassVar[int]
-    USER_TYPE_FIELD_NUMBER: _ClassVar[int]
-    auth_token: _wrappers_pb2.StringValue
-    comment: _wrappers_pb2.StringValue
-    ctime: _wrappers_pb2.StringValue
-    email: _wrappers_pb2.StringValue
+    CTIME_FIELD_NUMBER: _ClassVar[int]
+    MTIME_FIELD_NUMBER: _ClassVar[int]
+    AUTH_TOKEN_FIELD_NUMBER: _ClassVar[int]
+    DEFAULT_STRATEGY_FIELD_NUMBER: _ClassVar[int]
     id: _wrappers_pb2.StringValue
-    mobile: _wrappers_pb2.StringValue
-    mtime: _wrappers_pb2.StringValue
     name: _wrappers_pb2.StringValue
+    principals: Principals
+    resources: StrategyResources
+    action: AuthAction
+    comment: _wrappers_pb2.StringValue
     owner: _wrappers_pb2.StringValue
-    password: _wrappers_pb2.StringValue
-    source: _wrappers_pb2.StringValue
-    token_enable: _wrappers_pb2.BoolValue
-    user_type: _wrappers_pb2.StringValue
-    def __init__(self, id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., password: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., owner: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., source: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., auth_token: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., token_enable: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., ctime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mtime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., user_type: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mobile: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., email: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
+    ctime: _wrappers_pb2.StringValue
+    mtime: _wrappers_pb2.StringValue
+    auth_token: _wrappers_pb2.StringValue
+    default_strategy: _wrappers_pb2.BoolValue
+    def __init__(self, id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., principals: _Optional[_Union[Principals, _Mapping]] = ..., resources: _Optional[_Union[StrategyResources, _Mapping]] = ..., action: _Optional[_Union[AuthAction, str]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., owner: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., ctime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mtime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., auth_token: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., default_strategy: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...) -> None: ...
 
-class UserGroup(_message.Message):
-    __slots__ = ["auth_token", "comment", "ctime", "id", "mtime", "name", "owner", "relation", "token_enable", "user_count"]
-    AUTH_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    COMMENT_FIELD_NUMBER: _ClassVar[int]
-    CTIME_FIELD_NUMBER: _ClassVar[int]
+class ModifyAuthStrategy(_message.Message):
+    __slots__ = ["id", "name", "add_principals", "remove_principals", "add_resources", "remove_resources", "action", "comment", "owner"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    MTIME_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
+    ADD_PRINCIPALS_FIELD_NUMBER: _ClassVar[int]
+    REMOVE_PRINCIPALS_FIELD_NUMBER: _ClassVar[int]
+    ADD_RESOURCES_FIELD_NUMBER: _ClassVar[int]
+    REMOVE_RESOURCES_FIELD_NUMBER: _ClassVar[int]
+    ACTION_FIELD_NUMBER: _ClassVar[int]
+    COMMENT_FIELD_NUMBER: _ClassVar[int]
     OWNER_FIELD_NUMBER: _ClassVar[int]
-    RELATION_FIELD_NUMBER: _ClassVar[int]
-    TOKEN_ENABLE_FIELD_NUMBER: _ClassVar[int]
-    USER_COUNT_FIELD_NUMBER: _ClassVar[int]
-    auth_token: _wrappers_pb2.StringValue
-    comment: _wrappers_pb2.StringValue
-    ctime: _wrappers_pb2.StringValue
     id: _wrappers_pb2.StringValue
-    mtime: _wrappers_pb2.StringValue
     name: _wrappers_pb2.StringValue
+    add_principals: Principals
+    remove_principals: Principals
+    add_resources: StrategyResources
+    remove_resources: StrategyResources
+    action: AuthAction
+    comment: _wrappers_pb2.StringValue
     owner: _wrappers_pb2.StringValue
-    relation: UserGroupRelation
-    token_enable: _wrappers_pb2.BoolValue
-    user_count: _wrappers_pb2.UInt32Value
-    def __init__(self, id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., owner: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., auth_token: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., token_enable: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., ctime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mtime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., relation: _Optional[_Union[UserGroupRelation, _Mapping]] = ..., user_count: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ...) -> None: ...
-
-class UserGroupRelation(_message.Message):
-    __slots__ = ["group_id", "users"]
-    GROUP_ID_FIELD_NUMBER: _ClassVar[int]
-    USERS_FIELD_NUMBER: _ClassVar[int]
-    group_id: _wrappers_pb2.StringValue
-    users: _containers.RepeatedCompositeFieldContainer[User]
-    def __init__(self, group_id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., users: _Optional[_Iterable[_Union[User, _Mapping]]] = ...) -> None: ...
-
-class AuthAction(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
-
-class ResourceType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
+    def __init__(self, id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., add_principals: _Optional[_Union[Principals, _Mapping]] = ..., remove_principals: _Optional[_Union[Principals, _Mapping]] = ..., add_resources: _Optional[_Union[StrategyResources, _Mapping]] = ..., remove_resources: _Optional[_Union[StrategyResources, _Mapping]] = ..., action: _Optional[_Union[AuthAction, str]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., owner: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/client_pb2.py` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/client_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: client.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from ..model import model_pb2 as model__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63lient.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x0bmodel.proto\"\xf7\x02\n\x06\x43lient\x12*\n\x04host\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12#\n\x04type\x18\x02 \x01(\x0e\x32\x15.v1.Client.ClientType\x12-\n\x07version\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1e\n\x08location\x18\x04 \x01(\x0b\x32\x0c.v1.Location\x12(\n\x02id\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1a\n\x04stat\x18\x06 \x03(\x0b\x32\x0c.v1.StatInfo\x12+\n\x05\x63time\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05mtime\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"-\n\nClientType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03SDK\x10\x01\x12\t\n\x05\x41GENT\x10\x02\"\xc0\x01\n\x08StatInfo\x12,\n\x06target\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04port\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04path\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\x08protocol\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValueB\x8c\x01\n7com.tencent.polaris.specification.api.v1.service.manageB\x0b\x43lientProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'client_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'client_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n7com.tencent.polaris.specification.api.v1.service.manageB\013ClientProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manage'
-  _CLIENT._serialized_start=66
-  _CLIENT._serialized_end=441
-  _CLIENT_CLIENTTYPE._serialized_start=396
-  _CLIENT_CLIENTTYPE._serialized_end=441
-  _STATINFO._serialized_start=444
-  _STATINFO._serialized_end=636
+  _globals['_CLIENT']._serialized_start=66
+  _globals['_CLIENT']._serialized_end=441
+  _globals['_CLIENT_CLIENTTYPE']._serialized_start=396
+  _globals['_CLIENT_CLIENTTYPE']._serialized_end=441
+  _globals['_STATINFO']._serialized_start=444
+  _globals['_STATINFO']._serialized_end=636
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -5,42 +5,45 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Client(_message.Message):
-    __slots__ = ["ctime", "host", "id", "location", "mtime", "stat", "type", "version"]
+    __slots__ = ["host", "type", "version", "location", "id", "stat", "ctime", "mtime"]
     class ClientType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        UNKNOWN: _ClassVar[Client.ClientType]
+        SDK: _ClassVar[Client.ClientType]
+        AGENT: _ClassVar[Client.ClientType]
+    UNKNOWN: Client.ClientType
+    SDK: Client.ClientType
     AGENT: Client.ClientType
-    CTIME_FIELD_NUMBER: _ClassVar[int]
     HOST_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    LOCATION_FIELD_NUMBER: _ClassVar[int]
-    MTIME_FIELD_NUMBER: _ClassVar[int]
-    SDK: Client.ClientType
-    STAT_FIELD_NUMBER: _ClassVar[int]
     TYPE_FIELD_NUMBER: _ClassVar[int]
-    UNKNOWN: Client.ClientType
     VERSION_FIELD_NUMBER: _ClassVar[int]
-    ctime: _wrappers_pb2.StringValue
+    LOCATION_FIELD_NUMBER: _ClassVar[int]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    STAT_FIELD_NUMBER: _ClassVar[int]
+    CTIME_FIELD_NUMBER: _ClassVar[int]
+    MTIME_FIELD_NUMBER: _ClassVar[int]
     host: _wrappers_pb2.StringValue
-    id: _wrappers_pb2.StringValue
-    location: _model_pb2.Location
-    mtime: _wrappers_pb2.StringValue
-    stat: _containers.RepeatedCompositeFieldContainer[StatInfo]
     type: Client.ClientType
     version: _wrappers_pb2.StringValue
+    location: _model_pb2.Location
+    id: _wrappers_pb2.StringValue
+    stat: _containers.RepeatedCompositeFieldContainer[StatInfo]
+    ctime: _wrappers_pb2.StringValue
+    mtime: _wrappers_pb2.StringValue
     def __init__(self, host: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., type: _Optional[_Union[Client.ClientType, str]] = ..., version: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., location: _Optional[_Union[_model_pb2.Location, _Mapping]] = ..., id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., stat: _Optional[_Iterable[_Union[StatInfo, _Mapping]]] = ..., ctime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mtime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
 
 class StatInfo(_message.Message):
-    __slots__ = ["path", "port", "protocol", "target"]
-    PATH_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["target", "port", "path", "protocol"]
+    TARGET_FIELD_NUMBER: _ClassVar[int]
     PORT_FIELD_NUMBER: _ClassVar[int]
+    PATH_FIELD_NUMBER: _ClassVar[int]
     PROTOCOL_FIELD_NUMBER: _ClassVar[int]
-    TARGET_FIELD_NUMBER: _ClassVar[int]
-    path: _wrappers_pb2.StringValue
+    target: _wrappers_pb2.StringValue
     port: _wrappers_pb2.UInt32Value
+    path: _wrappers_pb2.StringValue
     protocol: _wrappers_pb2.StringValue
-    target: _wrappers_pb2.StringValue
     def __init__(self, target: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., port: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., path: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., protocol: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: configrelease.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from ..service_manage import service_pb2 as service__pb2
 from ..fault_tolerance import circuitbreaker_pb2 as circuitbreaker__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13\x63onfigrelease.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\rservice.proto\x1a\x14\x63ircuitbreaker.proto\"\xb3\x01\n\rConfigRelease\x12\x1c\n\x07service\x18\x01 \x01(\x0b\x32\x0b.v1.Service\x12+\n\x05\x63time\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05mtime\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x0e\x63ircuitBreaker\x18\x04 \x01(\x0b\x32\x12.v1.CircuitBreaker\"^\n\x11\x43onfigWithService\x12\x1d\n\x08services\x18\x01 \x03(\x0b\x32\x0b.v1.Service\x12*\n\x0e\x63ircuitBreaker\x18\x02 \x01(\x0b\x32\x12.v1.CircuitBreakerB\x93\x01\n7com.tencent.polaris.specification.api.v1.service.manageB\x12\x43onfigReleaseProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'configrelease_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'configrelease_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n7com.tencent.polaris.specification.api.v1.service.manageB\022ConfigReleaseProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manage'
-  _CONFIGRELEASE._serialized_start=97
-  _CONFIGRELEASE._serialized_end=276
-  _CONFIGWITHSERVICE._serialized_start=278
-  _CONFIGWITHSERVICE._serialized_end=372
+  _globals['_CONFIGRELEASE']._serialized_start=97
+  _globals['_CONFIGRELEASE']._serialized_end=276
+  _globals['_CONFIGWITHSERVICE']._serialized_start=278
+  _globals['_CONFIGWITHSERVICE']._serialized_end=372
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class ConfigRelease(_message.Message):
-    __slots__ = ["circuitBreaker", "ctime", "mtime", "service"]
-    CIRCUITBREAKER_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["service", "ctime", "mtime", "circuitBreaker"]
+    SERVICE_FIELD_NUMBER: _ClassVar[int]
     CTIME_FIELD_NUMBER: _ClassVar[int]
     MTIME_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_FIELD_NUMBER: _ClassVar[int]
-    circuitBreaker: _circuitbreaker_pb2.CircuitBreaker
+    CIRCUITBREAKER_FIELD_NUMBER: _ClassVar[int]
+    service: _service_pb2.Service
     ctime: _wrappers_pb2.StringValue
     mtime: _wrappers_pb2.StringValue
-    service: _service_pb2.Service
+    circuitBreaker: _circuitbreaker_pb2.CircuitBreaker
     def __init__(self, service: _Optional[_Union[_service_pb2.Service, _Mapping]] = ..., ctime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mtime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., circuitBreaker: _Optional[_Union[_circuitbreaker_pb2.CircuitBreaker, _Mapping]] = ...) -> None: ...
 
 class ConfigWithService(_message.Message):
-    __slots__ = ["circuitBreaker", "services"]
-    CIRCUITBREAKER_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["services", "circuitBreaker"]
     SERVICES_FIELD_NUMBER: _ClassVar[int]
-    circuitBreaker: _circuitbreaker_pb2.CircuitBreaker
+    CIRCUITBREAKER_FIELD_NUMBER: _ClassVar[int]
     services: _containers.RepeatedCompositeFieldContainer[_service_pb2.Service]
+    circuitBreaker: _circuitbreaker_pb2.CircuitBreaker
     def __init__(self, services: _Optional[_Iterable[_Union[_service_pb2.Service, _Mapping]]] = ..., circuitBreaker: _Optional[_Union[_circuitbreaker_pb2.CircuitBreaker, _Mapping]] = ...) -> None: ...
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: grpcapi.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ..service_manage import client_pb2 as client__pb2
 from ..service_manage import service_pb2 as service__pb2
 from ..service_manage import request_pb2 as request__pb2
 from ..service_manage import response_pb2 as response__pb2
 from ..service_manage import heartbeat_pb2 as heartbeat__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rgrpcapi.proto\x12\x02v1\x1a\x0c\x63lient.proto\x1a\rservice.proto\x1a\rrequest.proto\x1a\x0eresponse.proto\x1a\x0fheartbeat.proto2\xe6\x03\n\x0bPolarisGRPC\x12*\n\x0cReportClient\x12\n.v1.Client\x1a\x0c.v1.Response\"\x00\x12\x30\n\x10RegisterInstance\x12\x0c.v1.Instance\x1a\x0c.v1.Response\"\x00\x12\x32\n\x12\x44\x65registerInstance\x12\x0c.v1.Instance\x1a\x0c.v1.Response\"\x00\x12;\n\x08\x44iscover\x12\x13.v1.DiscoverRequest\x1a\x14.v1.DiscoverResponse\"\x00(\x01\x30\x01\x12)\n\tHeartbeat\x12\x0c.v1.Instance\x1a\x0c.v1.Response\"\x00\x12\x45\n\x0e\x42\x61tchHeartbeat\x12\x15.v1.HeartbeatsRequest\x1a\x16.v1.HeartbeatsResponse\"\x00(\x01\x30\x01\x12J\n\x11\x42\x61tchGetHeartbeat\x12\x18.v1.GetHeartbeatsRequest\x1a\x19.v1.GetHeartbeatsResponse\"\x00\x12J\n\x11\x42\x61tchDelHeartbeat\x12\x18.v1.DelHeartbeatsRequest\x1a\x19.v1.DelHeartbeatsResponse\"\x00\x42\x93\x01\n7com.tencent.polaris.specification.api.v1.service.manageB\x12PolarisGRPCServiceZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'grpcapi_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'grpcapi_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n7com.tencent.polaris.specification.api.v1.service.manageB\022PolarisGRPCServiceZDgithub.com/polarismesh/specification/source/go/api/v1/service_manage'
-  _POLARISGRPC._serialized_start=99
-  _POLARISGRPC._serialized_end=585
+  _globals['_POLARISGRPC']._serialized_start=99
+  _globals['_POLARISGRPC']._serialized_end=585
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: heartbeat.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ..service_manage import service_pb2 as service__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fheartbeat.proto\x12\x02v1\x1a\rservice.proto\"|\n\x0fHeartbeatRecord\x12\x1f\n\ninstanceId\x18\x01 \x01(\tR\x0binstance_id\x12,\n\x10lastHeartbeatSec\x18\x06 \x01(\x03R\x12last_heartbeat_sec\x12\x14\n\x05\x65xist\x18\x07 \x01(\x08R\x05\x65xistJ\x04\x08\x02\x10\x06\"\x94\x01\n\x11InstanceHeartbeat\x12\x1f\n\ninstanceId\x18\x01 \x01(\tR\x0binstance_id\x12\x18\n\x07service\x18\x02 \x01(\tR\x07service\x12\x1c\n\tnamespace\x18\x03 \x01(\tR\tnamespace\x12\x12\n\x04host\x18\x04 \x01(\tR\x04host\x12\x12\n\x04port\x18\x05 \x01(\rR\x04port\"J\n\x11HeartbeatsRequest\x12\x35\n\nheartbeats\x18\x01 \x03(\x0b\x32\x15.v1.InstanceHeartbeatR\nheartbeats\"\x14\n\x12HeartbeatsResponse\"9\n\x14GetHeartbeatsRequest\x12!\n\x0binstanceIds\x18\x01 \x03(\tR\x0cinstance_ids\"F\n\x15GetHeartbeatsResponse\x12-\n\x07records\x18\x01 \x03(\x0b\x32\x13.v1.HeartbeatRecordR\x07records\"9\n\x14\x44\x65lHeartbeatsRequest\x12!\n\x0binstanceIds\x18\x01 \x03(\tR\x0cinstance_ids\"3\n\x15\x44\x65lHeartbeatsResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\r\x12\x0c\n\x04info\x18\x02 \x01(\tB\x7f\n7com.tencent.polaris.specification.api.v1.service.manageZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'heartbeat_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'heartbeat_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n7com.tencent.polaris.specification.api.v1.service.manageZDgithub.com/polarismesh/specification/source/go/api/v1/service_manage'
-  _HEARTBEATRECORD._serialized_start=38
-  _HEARTBEATRECORD._serialized_end=162
-  _INSTANCEHEARTBEAT._serialized_start=165
-  _INSTANCEHEARTBEAT._serialized_end=313
-  _HEARTBEATSREQUEST._serialized_start=315
-  _HEARTBEATSREQUEST._serialized_end=389
-  _HEARTBEATSRESPONSE._serialized_start=391
-  _HEARTBEATSRESPONSE._serialized_end=411
-  _GETHEARTBEATSREQUEST._serialized_start=413
-  _GETHEARTBEATSREQUEST._serialized_end=470
-  _GETHEARTBEATSRESPONSE._serialized_start=472
-  _GETHEARTBEATSRESPONSE._serialized_end=542
-  _DELHEARTBEATSREQUEST._serialized_start=544
-  _DELHEARTBEATSREQUEST._serialized_end=601
-  _DELHEARTBEATSRESPONSE._serialized_start=603
-  _DELHEARTBEATSRESPONSE._serialized_end=654
+  _globals['_HEARTBEATRECORD']._serialized_start=38
+  _globals['_HEARTBEATRECORD']._serialized_end=162
+  _globals['_INSTANCEHEARTBEAT']._serialized_start=165
+  _globals['_INSTANCEHEARTBEAT']._serialized_end=313
+  _globals['_HEARTBEATSREQUEST']._serialized_start=315
+  _globals['_HEARTBEATSREQUEST']._serialized_end=389
+  _globals['_HEARTBEATSRESPONSE']._serialized_start=391
+  _globals['_HEARTBEATSRESPONSE']._serialized_end=411
+  _globals['_GETHEARTBEATSREQUEST']._serialized_start=413
+  _globals['_GETHEARTBEATSREQUEST']._serialized_end=470
+  _globals['_GETHEARTBEATSRESPONSE']._serialized_start=472
+  _globals['_GETHEARTBEATSRESPONSE']._serialized_end=542
+  _globals['_DELHEARTBEATSREQUEST']._serialized_start=544
+  _globals['_DELHEARTBEATSREQUEST']._serialized_end=601
+  _globals['_DELHEARTBEATSRESPONSE']._serialized_start=603
+  _globals['_DELHEARTBEATSRESPONSE']._serialized_end=654
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,66 +2,66 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class DelHeartbeatsRequest(_message.Message):
-    __slots__ = ["instanceIds"]
-    INSTANCEIDS_FIELD_NUMBER: _ClassVar[int]
-    instanceIds: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, instanceIds: _Optional[_Iterable[str]] = ...) -> None: ...
-
-class DelHeartbeatsResponse(_message.Message):
-    __slots__ = ["code", "info"]
-    CODE_FIELD_NUMBER: _ClassVar[int]
-    INFO_FIELD_NUMBER: _ClassVar[int]
-    code: int
-    info: str
-    def __init__(self, code: _Optional[int] = ..., info: _Optional[str] = ...) -> None: ...
-
-class GetHeartbeatsRequest(_message.Message):
-    __slots__ = ["instanceIds"]
-    INSTANCEIDS_FIELD_NUMBER: _ClassVar[int]
-    instanceIds: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, instanceIds: _Optional[_Iterable[str]] = ...) -> None: ...
-
-class GetHeartbeatsResponse(_message.Message):
-    __slots__ = ["records"]
-    RECORDS_FIELD_NUMBER: _ClassVar[int]
-    records: _containers.RepeatedCompositeFieldContainer[HeartbeatRecord]
-    def __init__(self, records: _Optional[_Iterable[_Union[HeartbeatRecord, _Mapping]]] = ...) -> None: ...
-
 class HeartbeatRecord(_message.Message):
-    __slots__ = ["exist", "instanceId", "lastHeartbeatSec"]
-    EXIST_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["instanceId", "lastHeartbeatSec", "exist"]
     INSTANCEID_FIELD_NUMBER: _ClassVar[int]
     LASTHEARTBEATSEC_FIELD_NUMBER: _ClassVar[int]
-    exist: bool
+    EXIST_FIELD_NUMBER: _ClassVar[int]
     instanceId: str
     lastHeartbeatSec: int
+    exist: bool
     def __init__(self, instanceId: _Optional[str] = ..., lastHeartbeatSec: _Optional[int] = ..., exist: bool = ...) -> None: ...
 
+class InstanceHeartbeat(_message.Message):
+    __slots__ = ["instanceId", "service", "namespace", "host", "port"]
+    INSTANCEID_FIELD_NUMBER: _ClassVar[int]
+    SERVICE_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    HOST_FIELD_NUMBER: _ClassVar[int]
+    PORT_FIELD_NUMBER: _ClassVar[int]
+    instanceId: str
+    service: str
+    namespace: str
+    host: str
+    port: int
+    def __init__(self, instanceId: _Optional[str] = ..., service: _Optional[str] = ..., namespace: _Optional[str] = ..., host: _Optional[str] = ..., port: _Optional[int] = ...) -> None: ...
+
 class HeartbeatsRequest(_message.Message):
     __slots__ = ["heartbeats"]
     HEARTBEATS_FIELD_NUMBER: _ClassVar[int]
     heartbeats: _containers.RepeatedCompositeFieldContainer[InstanceHeartbeat]
     def __init__(self, heartbeats: _Optional[_Iterable[_Union[InstanceHeartbeat, _Mapping]]] = ...) -> None: ...
 
 class HeartbeatsResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
-class InstanceHeartbeat(_message.Message):
-    __slots__ = ["host", "instanceId", "namespace", "port", "service"]
-    HOST_FIELD_NUMBER: _ClassVar[int]
-    INSTANCEID_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    PORT_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_FIELD_NUMBER: _ClassVar[int]
-    host: str
-    instanceId: str
-    namespace: str
-    port: int
-    service: str
-    def __init__(self, instanceId: _Optional[str] = ..., service: _Optional[str] = ..., namespace: _Optional[str] = ..., host: _Optional[str] = ..., port: _Optional[int] = ...) -> None: ...
+class GetHeartbeatsRequest(_message.Message):
+    __slots__ = ["instanceIds"]
+    INSTANCEIDS_FIELD_NUMBER: _ClassVar[int]
+    instanceIds: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, instanceIds: _Optional[_Iterable[str]] = ...) -> None: ...
+
+class GetHeartbeatsResponse(_message.Message):
+    __slots__ = ["records"]
+    RECORDS_FIELD_NUMBER: _ClassVar[int]
+    records: _containers.RepeatedCompositeFieldContainer[HeartbeatRecord]
+    def __init__(self, records: _Optional[_Iterable[_Union[HeartbeatRecord, _Mapping]]] = ...) -> None: ...
+
+class DelHeartbeatsRequest(_message.Message):
+    __slots__ = ["instanceIds"]
+    INSTANCEIDS_FIELD_NUMBER: _ClassVar[int]
+    instanceIds: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, instanceIds: _Optional[_Iterable[str]] = ...) -> None: ...
+
+class DelHeartbeatsResponse(_message.Message):
+    __slots__ = ["code", "info"]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    INFO_FIELD_NUMBER: _ClassVar[int]
+    code: int
+    info: str
+    def __init__(self, code: _Optional[int] = ..., info: _Optional[str] = ...) -> None: ...
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/request_pb2.py` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/request_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: request.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ..service_manage import service_pb2 as service__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rrequest.proto\x12\x02v1\x1a\rservice.proto\"\x96\x02\n\x0f\x44iscoverRequest\x12\x35\n\x04type\x18\x01 \x01(\x0e\x32\'.v1.DiscoverRequest.DiscoverRequestType\x12\x1c\n\x07service\x18\x02 \x01(\x0b\x32\x0b.v1.Service\"\xa7\x01\n\x13\x44iscoverRequestType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08INSTANCE\x10\x01\x12\x0b\n\x07\x43LUSTER\x10\x02\x12\x0b\n\x07ROUTING\x10\x03\x12\x0e\n\nRATE_LIMIT\x10\x04\x12\x13\n\x0f\x43IRCUIT_BREAKER\x10\x05\x12\x0c\n\x08SERVICES\x10\x06\x12\x0e\n\nNAMESPACES\x10\x0c\x12\x12\n\x0e\x46\x41ULT_DETECTOR\x10\r\"\x04\x08\x07\x10\x0bJ\x04\x08\x03\x10\x05\x42\x8d\x01\n7com.tencent.polaris.specification.api.v1.service.manageB\x0cRequestProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'request_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'request_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n7com.tencent.polaris.specification.api.v1.service.manageB\014RequestProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manage'
-  _DISCOVERREQUEST._serialized_start=37
-  _DISCOVERREQUEST._serialized_end=315
-  _DISCOVERREQUEST_DISCOVERREQUESTTYPE._serialized_start=142
-  _DISCOVERREQUEST_DISCOVERREQUESTTYPE._serialized_end=309
+  _globals['_DISCOVERREQUEST']._serialized_start=37
+  _globals['_DISCOVERREQUEST']._serialized_end=315
+  _globals['_DISCOVERREQUEST_DISCOVERREQUESTTYPE']._serialized_start=142
+  _globals['_DISCOVERREQUEST_DISCOVERREQUESTTYPE']._serialized_end=309
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/response_pb2.py` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/response_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: response.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
@@ -23,36 +23,37 @@
 from ..service_manage import configrelease_pb2 as configrelease__pb2
 from ..fault_tolerance import fault_detector_pb2 as fault__detector__pb2
 from ..security import auth_pb2 as auth__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0eresponse.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x19google/protobuf/any.proto\x1a\x0fnamespace.proto\x1a\rservice.proto\x1a\rrouting.proto\x1a\x0fratelimit.proto\x1a\x14\x63ircuitbreaker.proto\x1a\x0bmodel.proto\x1a\x0c\x63lient.proto\x1a\x13\x63onfigrelease.proto\x1a\x14\x66\x61ult_detector.proto\x1a\nauth.proto\"\xcf\x06\n\x08Response\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1a\n\x06\x63lient\x18\x03 \x01(\x0b\x32\n.v1.Client\x12 \n\tnamespace\x18\x04 \x01(\x0b\x32\r.v1.Namespace\x12\x1c\n\x07service\x18\x05 \x01(\x0b\x32\x0b.v1.Service\x12\x1e\n\x08instance\x18\x06 \x01(\x0b\x32\x0c.v1.Instance\x12\x1c\n\x07routing\x18\x07 \x01(\x0b\x32\x0b.v1.Routing\x12\x1f\n\x05\x61lias\x18\x08 \x01(\x0b\x32\x10.v1.ServiceAlias\x12\x1b\n\trateLimit\x18\t \x01(\x0b\x32\x08.v1.Rule\x12*\n\x0e\x63ircuitBreaker\x18\n \x01(\x0b\x32\x12.v1.CircuitBreaker\x12(\n\rconfigRelease\x18\x0b \x01(\x0b\x32\x11.v1.ConfigRelease\x12\x16\n\x04user\x18\x13 \x01(\x0b\x32\x08.v1.User\x12 \n\tuserGroup\x18\x14 \x01(\x0b\x32\r.v1.UserGroup\x12&\n\x0c\x61uthStrategy\x18\x15 \x01(\x0b\x32\x10.v1.AuthStrategy\x12\'\n\x08relation\x18\x16 \x01(\x0b\x32\x15.v1.UserGroupRelation\x12(\n\rloginResponse\x18\x17 \x01(\x0b\x32\x11.v1.LoginResponse\x12\x32\n\x12modifyAuthStrategy\x18\x18 \x01(\x0b\x32\x16.v1.ModifyAuthStrategy\x12,\n\x0fmodifyUserGroup\x18\x19 \x01(\x0b\x32\x13.v1.ModifyUserGroup\x12(\n\tresources\x18\x1a \x01(\x0b\x32\x15.v1.StrategyResources\x12&\n\x0coptionSwitch\x18\x1b \x01(\x0b\x32\x10.v1.OptionSwitch\x12*\n\x0einstanceLabels\x18\x1c \x01(\x0b\x32\x12.v1.InstanceLabels\x12\"\n\x04\x64\x61ta\x18\x1d \x01(\x0b\x32\x14.google.protobuf.AnyJ\x04\x08\x0c\x10\x13\"\xb9\x01\n\x12\x42\x61tchWriteResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04size\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x1f\n\tresponses\x18\x04 \x03(\x0b\x32\x0c.v1.Response\"\x87\x05\n\x12\x42\x61tchQueryResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x61mount\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04size\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12!\n\nnamespaces\x18\x05 \x03(\x0b\x32\r.v1.Namespace\x12\x1d\n\x08services\x18\x06 \x03(\x0b\x32\x0b.v1.Service\x12\x1f\n\tinstances\x18\x07 \x03(\x0b\x32\x0c.v1.Instance\x12\x1d\n\x08routings\x18\x08 \x03(\x0b\x32\x0b.v1.Routing\x12!\n\x07\x61liases\x18\t \x03(\x0b\x32\x10.v1.ServiceAlias\x12\x1c\n\nrateLimits\x18\n \x03(\x0b\x32\x08.v1.Rule\x12\x31\n\x12\x63onfigWithServices\x18\x0b \x03(\x0b\x32\x15.v1.ConfigWithService\x12\x17\n\x05users\x18\x12 \x03(\x0b\x32\x08.v1.User\x12!\n\nuserGroups\x18\x13 \x03(\x0b\x32\r.v1.UserGroup\x12(\n\x0e\x61uthStrategies\x18\x14 \x03(\x0b\x32\x10.v1.AuthStrategy\x12\x1b\n\x07\x63lients\x18\x15 \x03(\x0b\x32\n.v1.Client\x12\"\n\x04\x64\x61ta\x18\x16 \x03(\x0b\x32\x14.google.protobuf.Any\x12\x1c\n\x07summary\x18\x17 \x01(\x0b\x32\x0b.v1.SummaryJ\x04\x08\x0c\x10\x12\"\xc4\x05\n\x10\x44iscoverResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x37\n\x04type\x18\x03 \x01(\x0e\x32).v1.DiscoverResponse.DiscoverResponseType\x12\x1c\n\x07service\x18\x04 \x01(\x0b\x32\x0b.v1.Service\x12\x1f\n\tinstances\x18\x05 \x03(\x0b\x32\x0c.v1.Instance\x12\x1c\n\x07routing\x18\x06 \x01(\x0b\x32\x0b.v1.Routing\x12 \n\trateLimit\x18\x07 \x01(\x0b\x32\r.v1.RateLimit\x12*\n\x0e\x63ircuitBreaker\x18\x08 \x01(\x0b\x32\x12.v1.CircuitBreaker\x12\x1d\n\x08services\x18\t \x03(\x0b\x32\x0b.v1.Service\x12!\n\nnamespaces\x18\n \x03(\x0b\x32\r.v1.Namespace\x12(\n\rfaultDetector\x18\x0b \x01(\x0b\x32\x11.v1.FaultDetector\x12\x1d\n\x08\x61liasFor\x18\x15 \x01(\x0b\x32\x0b.v1.Service\"\xe2\x01\n\x14\x44iscoverResponseType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08INSTANCE\x10\x01\x12\x0b\n\x07\x43LUSTER\x10\x02\x12\x0b\n\x07ROUTING\x10\x03\x12\x0e\n\nRATE_LIMIT\x10\x04\x12\x13\n\x0f\x43IRCUIT_BREAKER\x10\x05\x12\x0c\n\x08SERVICES\x10\x06\x12\x0e\n\nNAMESPACES\x10\x0c\x12\x12\n\x0e\x46\x41ULT_DETECTOR\x10\r\"\x04\x08\x07\x10\x0b*\x04MESH*\x0bMESH_CONFIG*\x0e\x46LUX_DBREFRESH*\x08\x46LUX_SDK*\x0b\x46LUX_SERVERJ\x04\x08\x0c\x10\x15\"n\n\x0cOptionSwitch\x12.\n\x07options\x18\x01 \x03(\x0b\x32\x1d.v1.OptionSwitch.OptionsEntry\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x7f\n\x0eInstanceLabels\x12.\n\x06labels\x18\x01 \x03(\x0b\x32\x1e.v1.InstanceLabels.LabelsEntry\x1a=\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.v1.StringList:\x02\x38\x01\x42\x8e\x01\n7com.tencent.polaris.specification.api.v1.service.manageB\rResponseProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'response_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'response_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n7com.tencent.polaris.specification.api.v1.service.manageB\rResponseProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manage'
   _OPTIONSWITCH_OPTIONSENTRY._options = None
   _OPTIONSWITCH_OPTIONSENTRY._serialized_options = b'8\001'
   _INSTANCELABELS_LABELSENTRY._options = None
   _INSTANCELABELS_LABELSENTRY._serialized_options = b'8\001'
-  _RESPONSE._serialized_start=250
-  _RESPONSE._serialized_end=1097
-  _BATCHWRITERESPONSE._serialized_start=1100
-  _BATCHWRITERESPONSE._serialized_end=1285
-  _BATCHQUERYRESPONSE._serialized_start=1288
-  _BATCHQUERYRESPONSE._serialized_end=1935
-  _DISCOVERRESPONSE._serialized_start=1938
-  _DISCOVERRESPONSE._serialized_end=2646
-  _DISCOVERRESPONSE_DISCOVERRESPONSETYPE._serialized_start=2414
-  _DISCOVERRESPONSE_DISCOVERRESPONSETYPE._serialized_end=2640
-  _OPTIONSWITCH._serialized_start=2648
-  _OPTIONSWITCH._serialized_end=2758
-  _OPTIONSWITCH_OPTIONSENTRY._serialized_start=2712
-  _OPTIONSWITCH_OPTIONSENTRY._serialized_end=2758
-  _INSTANCELABELS._serialized_start=2760
-  _INSTANCELABELS._serialized_end=2887
-  _INSTANCELABELS_LABELSENTRY._serialized_start=2826
-  _INSTANCELABELS_LABELSENTRY._serialized_end=2887
+  _globals['_RESPONSE']._serialized_start=250
+  _globals['_RESPONSE']._serialized_end=1097
+  _globals['_BATCHWRITERESPONSE']._serialized_start=1100
+  _globals['_BATCHWRITERESPONSE']._serialized_end=1285
+  _globals['_BATCHQUERYRESPONSE']._serialized_start=1288
+  _globals['_BATCHQUERYRESPONSE']._serialized_end=1935
+  _globals['_DISCOVERRESPONSE']._serialized_start=1938
+  _globals['_DISCOVERRESPONSE']._serialized_end=2646
+  _globals['_DISCOVERRESPONSE_DISCOVERRESPONSETYPE']._serialized_start=2414
+  _globals['_DISCOVERRESPONSE_DISCOVERRESPONSETYPE']._serialized_end=2640
+  _globals['_OPTIONSWITCH']._serialized_start=2648
+  _globals['_OPTIONSWITCH']._serialized_end=2758
+  _globals['_OPTIONSWITCH_OPTIONSENTRY']._serialized_start=2712
+  _globals['_OPTIONSWITCH_OPTIONSENTRY']._serialized_end=2758
+  _globals['_INSTANCELABELS']._serialized_start=2760
+  _globals['_INSTANCELABELS']._serialized_end=2887
+  _globals['_INSTANCELABELS_LABELSENTRY']._serialized_start=2826
+  _globals['_INSTANCELABELS_LABELSENTRY']._serialized_end=2887
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -14,169 +14,178 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class BatchQueryResponse(_message.Message):
-    __slots__ = ["aliases", "amount", "authStrategies", "clients", "code", "configWithServices", "data", "info", "instances", "namespaces", "rateLimits", "routings", "services", "size", "summary", "userGroups", "users"]
-    ALIASES_FIELD_NUMBER: _ClassVar[int]
-    AMOUNT_FIELD_NUMBER: _ClassVar[int]
-    AUTHSTRATEGIES_FIELD_NUMBER: _ClassVar[int]
-    CLIENTS_FIELD_NUMBER: _ClassVar[int]
+class Response(_message.Message):
+    __slots__ = ["code", "info", "client", "namespace", "service", "instance", "routing", "alias", "rateLimit", "circuitBreaker", "configRelease", "user", "userGroup", "authStrategy", "relation", "loginResponse", "modifyAuthStrategy", "modifyUserGroup", "resources", "optionSwitch", "instanceLabels", "data"]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    CONFIGWITHSERVICES_FIELD_NUMBER: _ClassVar[int]
+    INFO_FIELD_NUMBER: _ClassVar[int]
+    CLIENT_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    SERVICE_FIELD_NUMBER: _ClassVar[int]
+    INSTANCE_FIELD_NUMBER: _ClassVar[int]
+    ROUTING_FIELD_NUMBER: _ClassVar[int]
+    ALIAS_FIELD_NUMBER: _ClassVar[int]
+    RATELIMIT_FIELD_NUMBER: _ClassVar[int]
+    CIRCUITBREAKER_FIELD_NUMBER: _ClassVar[int]
+    CONFIGRELEASE_FIELD_NUMBER: _ClassVar[int]
+    USER_FIELD_NUMBER: _ClassVar[int]
+    USERGROUP_FIELD_NUMBER: _ClassVar[int]
+    AUTHSTRATEGY_FIELD_NUMBER: _ClassVar[int]
+    RELATION_FIELD_NUMBER: _ClassVar[int]
+    LOGINRESPONSE_FIELD_NUMBER: _ClassVar[int]
+    MODIFYAUTHSTRATEGY_FIELD_NUMBER: _ClassVar[int]
+    MODIFYUSERGROUP_FIELD_NUMBER: _ClassVar[int]
+    RESOURCES_FIELD_NUMBER: _ClassVar[int]
+    OPTIONSWITCH_FIELD_NUMBER: _ClassVar[int]
+    INSTANCELABELS_FIELD_NUMBER: _ClassVar[int]
     DATA_FIELD_NUMBER: _ClassVar[int]
+    code: _wrappers_pb2.UInt32Value
+    info: _wrappers_pb2.StringValue
+    client: _client_pb2.Client
+    namespace: _namespace_pb2.Namespace
+    service: _service_pb2.Service
+    instance: _service_pb2.Instance
+    routing: _routing_pb2.Routing
+    alias: _service_pb2.ServiceAlias
+    rateLimit: _ratelimit_pb2.Rule
+    circuitBreaker: _circuitbreaker_pb2.CircuitBreaker
+    configRelease: _configrelease_pb2.ConfigRelease
+    user: _auth_pb2.User
+    userGroup: _auth_pb2.UserGroup
+    authStrategy: _auth_pb2.AuthStrategy
+    relation: _auth_pb2.UserGroupRelation
+    loginResponse: _auth_pb2.LoginResponse
+    modifyAuthStrategy: _auth_pb2.ModifyAuthStrategy
+    modifyUserGroup: _auth_pb2.ModifyUserGroup
+    resources: _auth_pb2.StrategyResources
+    optionSwitch: OptionSwitch
+    instanceLabels: InstanceLabels
+    data: _any_pb2.Any
+    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., client: _Optional[_Union[_client_pb2.Client, _Mapping]] = ..., namespace: _Optional[_Union[_namespace_pb2.Namespace, _Mapping]] = ..., service: _Optional[_Union[_service_pb2.Service, _Mapping]] = ..., instance: _Optional[_Union[_service_pb2.Instance, _Mapping]] = ..., routing: _Optional[_Union[_routing_pb2.Routing, _Mapping]] = ..., alias: _Optional[_Union[_service_pb2.ServiceAlias, _Mapping]] = ..., rateLimit: _Optional[_Union[_ratelimit_pb2.Rule, _Mapping]] = ..., circuitBreaker: _Optional[_Union[_circuitbreaker_pb2.CircuitBreaker, _Mapping]] = ..., configRelease: _Optional[_Union[_configrelease_pb2.ConfigRelease, _Mapping]] = ..., user: _Optional[_Union[_auth_pb2.User, _Mapping]] = ..., userGroup: _Optional[_Union[_auth_pb2.UserGroup, _Mapping]] = ..., authStrategy: _Optional[_Union[_auth_pb2.AuthStrategy, _Mapping]] = ..., relation: _Optional[_Union[_auth_pb2.UserGroupRelation, _Mapping]] = ..., loginResponse: _Optional[_Union[_auth_pb2.LoginResponse, _Mapping]] = ..., modifyAuthStrategy: _Optional[_Union[_auth_pb2.ModifyAuthStrategy, _Mapping]] = ..., modifyUserGroup: _Optional[_Union[_auth_pb2.ModifyUserGroup, _Mapping]] = ..., resources: _Optional[_Union[_auth_pb2.StrategyResources, _Mapping]] = ..., optionSwitch: _Optional[_Union[OptionSwitch, _Mapping]] = ..., instanceLabels: _Optional[_Union[InstanceLabels, _Mapping]] = ..., data: _Optional[_Union[_any_pb2.Any, _Mapping]] = ...) -> None: ...
+
+class BatchWriteResponse(_message.Message):
+    __slots__ = ["code", "info", "size", "responses"]
+    CODE_FIELD_NUMBER: _ClassVar[int]
     INFO_FIELD_NUMBER: _ClassVar[int]
-    INSTANCES_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACES_FIELD_NUMBER: _ClassVar[int]
-    RATELIMITS_FIELD_NUMBER: _ClassVar[int]
-    ROUTINGS_FIELD_NUMBER: _ClassVar[int]
-    SERVICES_FIELD_NUMBER: _ClassVar[int]
     SIZE_FIELD_NUMBER: _ClassVar[int]
-    SUMMARY_FIELD_NUMBER: _ClassVar[int]
-    USERGROUPS_FIELD_NUMBER: _ClassVar[int]
-    USERS_FIELD_NUMBER: _ClassVar[int]
-    aliases: _containers.RepeatedCompositeFieldContainer[_service_pb2.ServiceAlias]
-    amount: _wrappers_pb2.UInt32Value
-    authStrategies: _containers.RepeatedCompositeFieldContainer[_auth_pb2.AuthStrategy]
-    clients: _containers.RepeatedCompositeFieldContainer[_client_pb2.Client]
+    RESPONSES_FIELD_NUMBER: _ClassVar[int]
     code: _wrappers_pb2.UInt32Value
-    configWithServices: _containers.RepeatedCompositeFieldContainer[_configrelease_pb2.ConfigWithService]
-    data: _containers.RepeatedCompositeFieldContainer[_any_pb2.Any]
     info: _wrappers_pb2.StringValue
-    instances: _containers.RepeatedCompositeFieldContainer[_service_pb2.Instance]
-    namespaces: _containers.RepeatedCompositeFieldContainer[_namespace_pb2.Namespace]
-    rateLimits: _containers.RepeatedCompositeFieldContainer[_ratelimit_pb2.Rule]
-    routings: _containers.RepeatedCompositeFieldContainer[_routing_pb2.Routing]
-    services: _containers.RepeatedCompositeFieldContainer[_service_pb2.Service]
     size: _wrappers_pb2.UInt32Value
-    summary: _model_pb2.Summary
-    userGroups: _containers.RepeatedCompositeFieldContainer[_auth_pb2.UserGroup]
-    users: _containers.RepeatedCompositeFieldContainer[_auth_pb2.User]
-    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., amount: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., size: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., namespaces: _Optional[_Iterable[_Union[_namespace_pb2.Namespace, _Mapping]]] = ..., services: _Optional[_Iterable[_Union[_service_pb2.Service, _Mapping]]] = ..., instances: _Optional[_Iterable[_Union[_service_pb2.Instance, _Mapping]]] = ..., routings: _Optional[_Iterable[_Union[_routing_pb2.Routing, _Mapping]]] = ..., aliases: _Optional[_Iterable[_Union[_service_pb2.ServiceAlias, _Mapping]]] = ..., rateLimits: _Optional[_Iterable[_Union[_ratelimit_pb2.Rule, _Mapping]]] = ..., configWithServices: _Optional[_Iterable[_Union[_configrelease_pb2.ConfigWithService, _Mapping]]] = ..., users: _Optional[_Iterable[_Union[_auth_pb2.User, _Mapping]]] = ..., userGroups: _Optional[_Iterable[_Union[_auth_pb2.UserGroup, _Mapping]]] = ..., authStrategies: _Optional[_Iterable[_Union[_auth_pb2.AuthStrategy, _Mapping]]] = ..., clients: _Optional[_Iterable[_Union[_client_pb2.Client, _Mapping]]] = ..., data: _Optional[_Iterable[_Union[_any_pb2.Any, _Mapping]]] = ..., summary: _Optional[_Union[_model_pb2.Summary, _Mapping]] = ...) -> None: ...
+    responses: _containers.RepeatedCompositeFieldContainer[Response]
+    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., size: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., responses: _Optional[_Iterable[_Union[Response, _Mapping]]] = ...) -> None: ...
 
-class BatchWriteResponse(_message.Message):
-    __slots__ = ["code", "info", "responses", "size"]
+class BatchQueryResponse(_message.Message):
+    __slots__ = ["code", "info", "amount", "size", "namespaces", "services", "instances", "routings", "aliases", "rateLimits", "configWithServices", "users", "userGroups", "authStrategies", "clients", "data", "summary"]
     CODE_FIELD_NUMBER: _ClassVar[int]
     INFO_FIELD_NUMBER: _ClassVar[int]
-    RESPONSES_FIELD_NUMBER: _ClassVar[int]
+    AMOUNT_FIELD_NUMBER: _ClassVar[int]
     SIZE_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACES_FIELD_NUMBER: _ClassVar[int]
+    SERVICES_FIELD_NUMBER: _ClassVar[int]
+    INSTANCES_FIELD_NUMBER: _ClassVar[int]
+    ROUTINGS_FIELD_NUMBER: _ClassVar[int]
+    ALIASES_FIELD_NUMBER: _ClassVar[int]
+    RATELIMITS_FIELD_NUMBER: _ClassVar[int]
+    CONFIGWITHSERVICES_FIELD_NUMBER: _ClassVar[int]
+    USERS_FIELD_NUMBER: _ClassVar[int]
+    USERGROUPS_FIELD_NUMBER: _ClassVar[int]
+    AUTHSTRATEGIES_FIELD_NUMBER: _ClassVar[int]
+    CLIENTS_FIELD_NUMBER: _ClassVar[int]
+    DATA_FIELD_NUMBER: _ClassVar[int]
+    SUMMARY_FIELD_NUMBER: _ClassVar[int]
     code: _wrappers_pb2.UInt32Value
     info: _wrappers_pb2.StringValue
-    responses: _containers.RepeatedCompositeFieldContainer[Response]
+    amount: _wrappers_pb2.UInt32Value
     size: _wrappers_pb2.UInt32Value
-    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., size: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., responses: _Optional[_Iterable[_Union[Response, _Mapping]]] = ...) -> None: ...
+    namespaces: _containers.RepeatedCompositeFieldContainer[_namespace_pb2.Namespace]
+    services: _containers.RepeatedCompositeFieldContainer[_service_pb2.Service]
+    instances: _containers.RepeatedCompositeFieldContainer[_service_pb2.Instance]
+    routings: _containers.RepeatedCompositeFieldContainer[_routing_pb2.Routing]
+    aliases: _containers.RepeatedCompositeFieldContainer[_service_pb2.ServiceAlias]
+    rateLimits: _containers.RepeatedCompositeFieldContainer[_ratelimit_pb2.Rule]
+    configWithServices: _containers.RepeatedCompositeFieldContainer[_configrelease_pb2.ConfigWithService]
+    users: _containers.RepeatedCompositeFieldContainer[_auth_pb2.User]
+    userGroups: _containers.RepeatedCompositeFieldContainer[_auth_pb2.UserGroup]
+    authStrategies: _containers.RepeatedCompositeFieldContainer[_auth_pb2.AuthStrategy]
+    clients: _containers.RepeatedCompositeFieldContainer[_client_pb2.Client]
+    data: _containers.RepeatedCompositeFieldContainer[_any_pb2.Any]
+    summary: _model_pb2.Summary
+    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., amount: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., size: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., namespaces: _Optional[_Iterable[_Union[_namespace_pb2.Namespace, _Mapping]]] = ..., services: _Optional[_Iterable[_Union[_service_pb2.Service, _Mapping]]] = ..., instances: _Optional[_Iterable[_Union[_service_pb2.Instance, _Mapping]]] = ..., routings: _Optional[_Iterable[_Union[_routing_pb2.Routing, _Mapping]]] = ..., aliases: _Optional[_Iterable[_Union[_service_pb2.ServiceAlias, _Mapping]]] = ..., rateLimits: _Optional[_Iterable[_Union[_ratelimit_pb2.Rule, _Mapping]]] = ..., configWithServices: _Optional[_Iterable[_Union[_configrelease_pb2.ConfigWithService, _Mapping]]] = ..., users: _Optional[_Iterable[_Union[_auth_pb2.User, _Mapping]]] = ..., userGroups: _Optional[_Iterable[_Union[_auth_pb2.UserGroup, _Mapping]]] = ..., authStrategies: _Optional[_Iterable[_Union[_auth_pb2.AuthStrategy, _Mapping]]] = ..., clients: _Optional[_Iterable[_Union[_client_pb2.Client, _Mapping]]] = ..., data: _Optional[_Iterable[_Union[_any_pb2.Any, _Mapping]]] = ..., summary: _Optional[_Union[_model_pb2.Summary, _Mapping]] = ...) -> None: ...
 
 class DiscoverResponse(_message.Message):
-    __slots__ = ["aliasFor", "circuitBreaker", "code", "faultDetector", "info", "instances", "namespaces", "rateLimit", "routing", "service", "services", "type"]
+    __slots__ = ["code", "info", "type", "service", "instances", "routing", "rateLimit", "circuitBreaker", "services", "namespaces", "faultDetector", "aliasFor"]
     class DiscoverResponseType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
-    ALIASFOR_FIELD_NUMBER: _ClassVar[int]
-    CIRCUITBREAKER_FIELD_NUMBER: _ClassVar[int]
-    CIRCUIT_BREAKER: DiscoverResponse.DiscoverResponseType
+        UNKNOWN: _ClassVar[DiscoverResponse.DiscoverResponseType]
+        INSTANCE: _ClassVar[DiscoverResponse.DiscoverResponseType]
+        CLUSTER: _ClassVar[DiscoverResponse.DiscoverResponseType]
+        ROUTING: _ClassVar[DiscoverResponse.DiscoverResponseType]
+        RATE_LIMIT: _ClassVar[DiscoverResponse.DiscoverResponseType]
+        CIRCUIT_BREAKER: _ClassVar[DiscoverResponse.DiscoverResponseType]
+        SERVICES: _ClassVar[DiscoverResponse.DiscoverResponseType]
+        NAMESPACES: _ClassVar[DiscoverResponse.DiscoverResponseType]
+        FAULT_DETECTOR: _ClassVar[DiscoverResponse.DiscoverResponseType]
+    UNKNOWN: DiscoverResponse.DiscoverResponseType
+    INSTANCE: DiscoverResponse.DiscoverResponseType
     CLUSTER: DiscoverResponse.DiscoverResponseType
-    CODE_FIELD_NUMBER: _ClassVar[int]
-    FAULTDETECTOR_FIELD_NUMBER: _ClassVar[int]
+    ROUTING: DiscoverResponse.DiscoverResponseType
+    RATE_LIMIT: DiscoverResponse.DiscoverResponseType
+    CIRCUIT_BREAKER: DiscoverResponse.DiscoverResponseType
+    SERVICES: DiscoverResponse.DiscoverResponseType
+    NAMESPACES: DiscoverResponse.DiscoverResponseType
     FAULT_DETECTOR: DiscoverResponse.DiscoverResponseType
+    CODE_FIELD_NUMBER: _ClassVar[int]
     INFO_FIELD_NUMBER: _ClassVar[int]
-    INSTANCE: DiscoverResponse.DiscoverResponseType
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    SERVICE_FIELD_NUMBER: _ClassVar[int]
     INSTANCES_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACES: DiscoverResponse.DiscoverResponseType
-    NAMESPACES_FIELD_NUMBER: _ClassVar[int]
-    RATELIMIT_FIELD_NUMBER: _ClassVar[int]
-    RATE_LIMIT: DiscoverResponse.DiscoverResponseType
-    ROUTING: DiscoverResponse.DiscoverResponseType
     ROUTING_FIELD_NUMBER: _ClassVar[int]
-    SERVICES: DiscoverResponse.DiscoverResponseType
+    RATELIMIT_FIELD_NUMBER: _ClassVar[int]
+    CIRCUITBREAKER_FIELD_NUMBER: _ClassVar[int]
     SERVICES_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_FIELD_NUMBER: _ClassVar[int]
-    TYPE_FIELD_NUMBER: _ClassVar[int]
-    UNKNOWN: DiscoverResponse.DiscoverResponseType
-    aliasFor: _service_pb2.Service
-    circuitBreaker: _circuitbreaker_pb2.CircuitBreaker
+    NAMESPACES_FIELD_NUMBER: _ClassVar[int]
+    FAULTDETECTOR_FIELD_NUMBER: _ClassVar[int]
+    ALIASFOR_FIELD_NUMBER: _ClassVar[int]
     code: _wrappers_pb2.UInt32Value
-    faultDetector: _fault_detector_pb2.FaultDetector
     info: _wrappers_pb2.StringValue
+    type: DiscoverResponse.DiscoverResponseType
+    service: _service_pb2.Service
     instances: _containers.RepeatedCompositeFieldContainer[_service_pb2.Instance]
-    namespaces: _containers.RepeatedCompositeFieldContainer[_namespace_pb2.Namespace]
-    rateLimit: _ratelimit_pb2.RateLimit
     routing: _routing_pb2.Routing
-    service: _service_pb2.Service
+    rateLimit: _ratelimit_pb2.RateLimit
+    circuitBreaker: _circuitbreaker_pb2.CircuitBreaker
     services: _containers.RepeatedCompositeFieldContainer[_service_pb2.Service]
-    type: DiscoverResponse.DiscoverResponseType
+    namespaces: _containers.RepeatedCompositeFieldContainer[_namespace_pb2.Namespace]
+    faultDetector: _fault_detector_pb2.FaultDetector
+    aliasFor: _service_pb2.Service
     def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., type: _Optional[_Union[DiscoverResponse.DiscoverResponseType, str]] = ..., service: _Optional[_Union[_service_pb2.Service, _Mapping]] = ..., instances: _Optional[_Iterable[_Union[_service_pb2.Instance, _Mapping]]] = ..., routing: _Optional[_Union[_routing_pb2.Routing, _Mapping]] = ..., rateLimit: _Optional[_Union[_ratelimit_pb2.RateLimit, _Mapping]] = ..., circuitBreaker: _Optional[_Union[_circuitbreaker_pb2.CircuitBreaker, _Mapping]] = ..., services: _Optional[_Iterable[_Union[_service_pb2.Service, _Mapping]]] = ..., namespaces: _Optional[_Iterable[_Union[_namespace_pb2.Namespace, _Mapping]]] = ..., faultDetector: _Optional[_Union[_fault_detector_pb2.FaultDetector, _Mapping]] = ..., aliasFor: _Optional[_Union[_service_pb2.Service, _Mapping]] = ...) -> None: ...
 
-class InstanceLabels(_message.Message):
-    __slots__ = ["labels"]
-    class LabelsEntry(_message.Message):
-        __slots__ = ["key", "value"]
-        KEY_FIELD_NUMBER: _ClassVar[int]
-        VALUE_FIELD_NUMBER: _ClassVar[int]
-        key: str
-        value: _model_pb2.StringList
-        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[_model_pb2.StringList, _Mapping]] = ...) -> None: ...
-    LABELS_FIELD_NUMBER: _ClassVar[int]
-    labels: _containers.MessageMap[str, _model_pb2.StringList]
-    def __init__(self, labels: _Optional[_Mapping[str, _model_pb2.StringList]] = ...) -> None: ...
-
 class OptionSwitch(_message.Message):
     __slots__ = ["options"]
     class OptionsEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
         def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
     OPTIONS_FIELD_NUMBER: _ClassVar[int]
     options: _containers.ScalarMap[str, str]
     def __init__(self, options: _Optional[_Mapping[str, str]] = ...) -> None: ...
 
-class Response(_message.Message):
-    __slots__ = ["alias", "authStrategy", "circuitBreaker", "client", "code", "configRelease", "data", "info", "instance", "instanceLabels", "loginResponse", "modifyAuthStrategy", "modifyUserGroup", "namespace", "optionSwitch", "rateLimit", "relation", "resources", "routing", "service", "user", "userGroup"]
-    ALIAS_FIELD_NUMBER: _ClassVar[int]
-    AUTHSTRATEGY_FIELD_NUMBER: _ClassVar[int]
-    CIRCUITBREAKER_FIELD_NUMBER: _ClassVar[int]
-    CLIENT_FIELD_NUMBER: _ClassVar[int]
-    CODE_FIELD_NUMBER: _ClassVar[int]
-    CONFIGRELEASE_FIELD_NUMBER: _ClassVar[int]
-    DATA_FIELD_NUMBER: _ClassVar[int]
-    INFO_FIELD_NUMBER: _ClassVar[int]
-    INSTANCELABELS_FIELD_NUMBER: _ClassVar[int]
-    INSTANCE_FIELD_NUMBER: _ClassVar[int]
-    LOGINRESPONSE_FIELD_NUMBER: _ClassVar[int]
-    MODIFYAUTHSTRATEGY_FIELD_NUMBER: _ClassVar[int]
-    MODIFYUSERGROUP_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    OPTIONSWITCH_FIELD_NUMBER: _ClassVar[int]
-    RATELIMIT_FIELD_NUMBER: _ClassVar[int]
-    RELATION_FIELD_NUMBER: _ClassVar[int]
-    RESOURCES_FIELD_NUMBER: _ClassVar[int]
-    ROUTING_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_FIELD_NUMBER: _ClassVar[int]
-    USERGROUP_FIELD_NUMBER: _ClassVar[int]
-    USER_FIELD_NUMBER: _ClassVar[int]
-    alias: _service_pb2.ServiceAlias
-    authStrategy: _auth_pb2.AuthStrategy
-    circuitBreaker: _circuitbreaker_pb2.CircuitBreaker
-    client: _client_pb2.Client
-    code: _wrappers_pb2.UInt32Value
-    configRelease: _configrelease_pb2.ConfigRelease
-    data: _any_pb2.Any
-    info: _wrappers_pb2.StringValue
-    instance: _service_pb2.Instance
-    instanceLabels: InstanceLabels
-    loginResponse: _auth_pb2.LoginResponse
-    modifyAuthStrategy: _auth_pb2.ModifyAuthStrategy
-    modifyUserGroup: _auth_pb2.ModifyUserGroup
-    namespace: _namespace_pb2.Namespace
-    optionSwitch: OptionSwitch
-    rateLimit: _ratelimit_pb2.Rule
-    relation: _auth_pb2.UserGroupRelation
-    resources: _auth_pb2.StrategyResources
-    routing: _routing_pb2.Routing
-    service: _service_pb2.Service
-    user: _auth_pb2.User
-    userGroup: _auth_pb2.UserGroup
-    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., client: _Optional[_Union[_client_pb2.Client, _Mapping]] = ..., namespace: _Optional[_Union[_namespace_pb2.Namespace, _Mapping]] = ..., service: _Optional[_Union[_service_pb2.Service, _Mapping]] = ..., instance: _Optional[_Union[_service_pb2.Instance, _Mapping]] = ..., routing: _Optional[_Union[_routing_pb2.Routing, _Mapping]] = ..., alias: _Optional[_Union[_service_pb2.ServiceAlias, _Mapping]] = ..., rateLimit: _Optional[_Union[_ratelimit_pb2.Rule, _Mapping]] = ..., circuitBreaker: _Optional[_Union[_circuitbreaker_pb2.CircuitBreaker, _Mapping]] = ..., configRelease: _Optional[_Union[_configrelease_pb2.ConfigRelease, _Mapping]] = ..., user: _Optional[_Union[_auth_pb2.User, _Mapping]] = ..., userGroup: _Optional[_Union[_auth_pb2.UserGroup, _Mapping]] = ..., authStrategy: _Optional[_Union[_auth_pb2.AuthStrategy, _Mapping]] = ..., relation: _Optional[_Union[_auth_pb2.UserGroupRelation, _Mapping]] = ..., loginResponse: _Optional[_Union[_auth_pb2.LoginResponse, _Mapping]] = ..., modifyAuthStrategy: _Optional[_Union[_auth_pb2.ModifyAuthStrategy, _Mapping]] = ..., modifyUserGroup: _Optional[_Union[_auth_pb2.ModifyUserGroup, _Mapping]] = ..., resources: _Optional[_Union[_auth_pb2.StrategyResources, _Mapping]] = ..., optionSwitch: _Optional[_Union[OptionSwitch, _Mapping]] = ..., instanceLabels: _Optional[_Union[InstanceLabels, _Mapping]] = ..., data: _Optional[_Union[_any_pb2.Any, _Mapping]] = ...) -> None: ...
+class InstanceLabels(_message.Message):
+    __slots__ = ["labels"]
+    class LabelsEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: _model_pb2.StringList
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[_model_pb2.StringList, _Mapping]] = ...) -> None: ...
+    LABELS_FIELD_NUMBER: _ClassVar[int]
+    labels: _containers.MessageMap[str, _model_pb2.StringList]
+    def __init__(self, labels: _Optional[_Mapping[str, _model_pb2.StringList]] = ...) -> None: ...
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/service_pb2.py` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/service_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from ..model import model_pb2 as model__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rservice.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x0bmodel.proto\"\xe3\n\n\x07Service\x12*\n\x04name\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x08metadata\x18\x03 \x03(\x0b\x32\x19.v1.Service.MetadataEntry\x12+\n\x05ports\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\x08\x62usiness\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\ndepartment\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12:\n\tcmdb_mod1\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\tcmdb_mod1\x12:\n\tcmdb_mod2\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\tcmdb_mod2\x12:\n\tcmdb_mod3\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValueR\tcmdb_mod3\x12-\n\x07\x63omment\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06owners\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05token\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05\x63time\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05mtime\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\x08revision\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12>\n\x0bplatform_id\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x0bplatform_id\x12P\n\x14total_instance_count\x18\x11 \x01(\x0b\x32\x1c.google.protobuf.UInt32ValueR\x14total_instance_count\x12T\n\x16healthy_instance_count\x18\x12 \x01(\x0b\x32\x1c.google.protobuf.UInt32ValueR\x16healthy_instance_count\x12\x38\n\x08user_ids\x18\x13 \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x08user_ids\x12:\n\tgroup_ids\x18\x14 \x03(\x0b\x32\x1c.google.protobuf.StringValueR\tgroup_ids\x12\x46\n\x0fremove_user_ids\x18\x16 \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x0fremove_user_ids\x12H\n\x10remove_group_ids\x18\x17 \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x10remove_group_ids\x12(\n\x02id\x18\x15 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x08\x65\x64itable\x18\x18 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xd3\x04\n\x0cServiceAlias\x12-\n\x07service\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05\x61lias\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x46\n\x0f\x61lias_namespace\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x0f\x61lias_namespace\x12\x1b\n\x04type\x18\x05 \x01(\x0e\x32\r.v1.AliasType\x12,\n\x06owners\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x42\n\rservice_token\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\rservice_token\x12+\n\x05\x63time\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05mtime\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12(\n\x02id\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x08\x65\x64itable\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\xa2\x08\n\x08Instance\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07service\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x34\n\x06vpc_id\x18\x15 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x06vpc_id\x12*\n\x04host\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04port\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12.\n\x08protocol\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07version\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\x08priority\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12,\n\x06weight\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x37\n\x13\x65nable_health_check\x18\x14 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12%\n\x0chealth_check\x18\n \x01(\x0b\x32\x0f.v1.HealthCheck\x12+\n\x07healthy\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12+\n\x07isolate\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x1e\n\x08location\x18\r \x01(\x0b\x32\x0c.v1.Location\x12,\n\x08metadata\x18\x0e \x03(\x0b\x32\x1a.v1.Instance.MetadataEntry\x12:\n\tlogic_set\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.StringValueR\tlogic_set\x12+\n\x05\x63time\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05mtime\x18\x11 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\x08revision\x18\x12 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x42\n\rservice_token\x18\x13 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\rservice_token\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x98\x01\n\x0bHealthCheck\x12-\n\x04type\x18\x01 \x01(\x0e\x32\x1f.v1.HealthCheck.HealthCheckType\x12+\n\theartbeat\x18\x02 \x01(\x0b\x32\x18.v1.HeartbeatHealthCheck\"-\n\x0fHealthCheckType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\r\n\tHEARTBEAT\x10\x01\"A\n\x14HeartbeatHealthCheck\x12)\n\x03ttl\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value*$\n\tAliasType\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\n\n\x06\x43L5SID\x10\x01\x42\x8d\x01\n7com.tencent.polaris.specification.api.v1.service.manageB\x0cServiceProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'service_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n7com.tencent.polaris.specification.api.v1.service.manageB\014ServiceProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manage'
   _SERVICE_METADATAENTRY._options = None
   _SERVICE_METADATAENTRY._serialized_options = b'8\001'
   _INSTANCE_METADATAENTRY._options = None
   _INSTANCE_METADATAENTRY._serialized_options = b'8\001'
-  _ALIASTYPE._serialized_start=3329
-  _ALIASTYPE._serialized_end=3365
-  _SERVICE._serialized_start=67
-  _SERVICE._serialized_end=1446
-  _SERVICE_METADATAENTRY._serialized_start=1399
-  _SERVICE_METADATAENTRY._serialized_end=1446
-  _SERVICEALIAS._serialized_start=1449
-  _SERVICEALIAS._serialized_end=2044
-  _INSTANCE._serialized_start=2047
-  _INSTANCE._serialized_end=3105
-  _INSTANCE_METADATAENTRY._serialized_start=1399
-  _INSTANCE_METADATAENTRY._serialized_end=1446
-  _HEALTHCHECK._serialized_start=3108
-  _HEALTHCHECK._serialized_end=3260
-  _HEALTHCHECK_HEALTHCHECKTYPE._serialized_start=3215
-  _HEALTHCHECK_HEALTHCHECKTYPE._serialized_end=3260
-  _HEARTBEATHEALTHCHECK._serialized_start=3262
-  _HEARTBEATHEALTHCHECK._serialized_end=3327
+  _globals['_ALIASTYPE']._serialized_start=3329
+  _globals['_ALIASTYPE']._serialized_end=3365
+  _globals['_SERVICE']._serialized_start=67
+  _globals['_SERVICE']._serialized_end=1446
+  _globals['_SERVICE_METADATAENTRY']._serialized_start=1399
+  _globals['_SERVICE_METADATAENTRY']._serialized_end=1446
+  _globals['_SERVICEALIAS']._serialized_start=1449
+  _globals['_SERVICEALIAS']._serialized_end=2044
+  _globals['_INSTANCE']._serialized_start=2047
+  _globals['_INSTANCE']._serialized_end=3105
+  _globals['_INSTANCE_METADATAENTRY']._serialized_start=1399
+  _globals['_INSTANCE_METADATAENTRY']._serialized_end=1446
+  _globals['_HEALTHCHECK']._serialized_start=3108
+  _globals['_HEALTHCHECK']._serialized_end=3260
+  _globals['_HEALTHCHECK_HEALTHCHECKTYPE']._serialized_start=3215
+  _globals['_HEALTHCHECK_HEALTHCHECKTYPE']._serialized_end=3260
+  _globals['_HEARTBEATHEALTHCHECK']._serialized_start=3262
+  _globals['_HEARTBEATHEALTHCHECK']._serialized_end=3327
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,171 +2,175 @@
 from ..model import model_pb2 as _model_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
-CL5SID: AliasType
-DEFAULT: AliasType
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class HealthCheck(_message.Message):
-    __slots__ = ["heartbeat", "type"]
-    class HealthCheckType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    HEARTBEAT: HealthCheck.HealthCheckType
-    HEARTBEAT_FIELD_NUMBER: _ClassVar[int]
-    TYPE_FIELD_NUMBER: _ClassVar[int]
-    UNKNOWN: HealthCheck.HealthCheckType
-    heartbeat: HeartbeatHealthCheck
-    type: HealthCheck.HealthCheckType
-    def __init__(self, type: _Optional[_Union[HealthCheck.HealthCheckType, str]] = ..., heartbeat: _Optional[_Union[HeartbeatHealthCheck, _Mapping]] = ...) -> None: ...
-
-class HeartbeatHealthCheck(_message.Message):
-    __slots__ = ["ttl"]
-    TTL_FIELD_NUMBER: _ClassVar[int]
-    ttl: _wrappers_pb2.UInt32Value
-    def __init__(self, ttl: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ...) -> None: ...
-
-class Instance(_message.Message):
-    __slots__ = ["ctime", "enable_health_check", "health_check", "healthy", "host", "id", "isolate", "location", "logic_set", "metadata", "mtime", "namespace", "port", "priority", "protocol", "revision", "service", "service_token", "version", "vpc_id", "weight"]
-    class MetadataEntry(_message.Message):
-        __slots__ = ["key", "value"]
-        KEY_FIELD_NUMBER: _ClassVar[int]
-        VALUE_FIELD_NUMBER: _ClassVar[int]
-        key: str
-        value: str
-        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
-    CTIME_FIELD_NUMBER: _ClassVar[int]
-    ENABLE_HEALTH_CHECK_FIELD_NUMBER: _ClassVar[int]
-    HEALTHY_FIELD_NUMBER: _ClassVar[int]
-    HEALTH_CHECK_FIELD_NUMBER: _ClassVar[int]
-    HOST_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    ISOLATE_FIELD_NUMBER: _ClassVar[int]
-    LOCATION_FIELD_NUMBER: _ClassVar[int]
-    LOGIC_SET_FIELD_NUMBER: _ClassVar[int]
-    METADATA_FIELD_NUMBER: _ClassVar[int]
-    MTIME_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    PORT_FIELD_NUMBER: _ClassVar[int]
-    PRIORITY_FIELD_NUMBER: _ClassVar[int]
-    PROTOCOL_FIELD_NUMBER: _ClassVar[int]
-    REVISION_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    VERSION_FIELD_NUMBER: _ClassVar[int]
-    VPC_ID_FIELD_NUMBER: _ClassVar[int]
-    WEIGHT_FIELD_NUMBER: _ClassVar[int]
-    ctime: _wrappers_pb2.StringValue
-    enable_health_check: _wrappers_pb2.BoolValue
-    health_check: HealthCheck
-    healthy: _wrappers_pb2.BoolValue
-    host: _wrappers_pb2.StringValue
-    id: _wrappers_pb2.StringValue
-    isolate: _wrappers_pb2.BoolValue
-    location: _model_pb2.Location
-    logic_set: _wrappers_pb2.StringValue
-    metadata: _containers.ScalarMap[str, str]
-    mtime: _wrappers_pb2.StringValue
-    namespace: _wrappers_pb2.StringValue
-    port: _wrappers_pb2.UInt32Value
-    priority: _wrappers_pb2.UInt32Value
-    protocol: _wrappers_pb2.StringValue
-    revision: _wrappers_pb2.StringValue
-    service: _wrappers_pb2.StringValue
-    service_token: _wrappers_pb2.StringValue
-    version: _wrappers_pb2.StringValue
-    vpc_id: _wrappers_pb2.StringValue
-    weight: _wrappers_pb2.UInt32Value
-    def __init__(self, id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., service: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., vpc_id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., host: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., port: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., protocol: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., version: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., priority: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., weight: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., enable_health_check: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., health_check: _Optional[_Union[HealthCheck, _Mapping]] = ..., healthy: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., isolate: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., location: _Optional[_Union[_model_pb2.Location, _Mapping]] = ..., metadata: _Optional[_Mapping[str, str]] = ..., logic_set: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., ctime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mtime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., revision: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., service_token: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
+class AliasType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    DEFAULT: _ClassVar[AliasType]
+    CL5SID: _ClassVar[AliasType]
+DEFAULT: AliasType
+CL5SID: AliasType
 
 class Service(_message.Message):
-    __slots__ = ["business", "cmdb_mod1", "cmdb_mod2", "cmdb_mod3", "comment", "ctime", "department", "editable", "group_ids", "healthy_instance_count", "id", "metadata", "mtime", "name", "namespace", "owners", "platform_id", "ports", "remove_group_ids", "remove_user_ids", "revision", "token", "total_instance_count", "user_ids"]
+    __slots__ = ["name", "namespace", "metadata", "ports", "business", "department", "cmdb_mod1", "cmdb_mod2", "cmdb_mod3", "comment", "owners", "token", "ctime", "mtime", "revision", "platform_id", "total_instance_count", "healthy_instance_count", "user_ids", "group_ids", "remove_user_ids", "remove_group_ids", "id", "editable"]
     class MetadataEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
         def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    METADATA_FIELD_NUMBER: _ClassVar[int]
+    PORTS_FIELD_NUMBER: _ClassVar[int]
     BUSINESS_FIELD_NUMBER: _ClassVar[int]
+    DEPARTMENT_FIELD_NUMBER: _ClassVar[int]
     CMDB_MOD1_FIELD_NUMBER: _ClassVar[int]
     CMDB_MOD2_FIELD_NUMBER: _ClassVar[int]
     CMDB_MOD3_FIELD_NUMBER: _ClassVar[int]
     COMMENT_FIELD_NUMBER: _ClassVar[int]
+    OWNERS_FIELD_NUMBER: _ClassVar[int]
+    TOKEN_FIELD_NUMBER: _ClassVar[int]
     CTIME_FIELD_NUMBER: _ClassVar[int]
-    DEPARTMENT_FIELD_NUMBER: _ClassVar[int]
-    EDITABLE_FIELD_NUMBER: _ClassVar[int]
-    GROUP_IDS_FIELD_NUMBER: _ClassVar[int]
-    HEALTHY_INSTANCE_COUNT_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    METADATA_FIELD_NUMBER: _ClassVar[int]
     MTIME_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    OWNERS_FIELD_NUMBER: _ClassVar[int]
-    PLATFORM_ID_FIELD_NUMBER: _ClassVar[int]
-    PORTS_FIELD_NUMBER: _ClassVar[int]
-    REMOVE_GROUP_IDS_FIELD_NUMBER: _ClassVar[int]
-    REMOVE_USER_IDS_FIELD_NUMBER: _ClassVar[int]
     REVISION_FIELD_NUMBER: _ClassVar[int]
-    TOKEN_FIELD_NUMBER: _ClassVar[int]
+    PLATFORM_ID_FIELD_NUMBER: _ClassVar[int]
     TOTAL_INSTANCE_COUNT_FIELD_NUMBER: _ClassVar[int]
+    HEALTHY_INSTANCE_COUNT_FIELD_NUMBER: _ClassVar[int]
     USER_IDS_FIELD_NUMBER: _ClassVar[int]
+    GROUP_IDS_FIELD_NUMBER: _ClassVar[int]
+    REMOVE_USER_IDS_FIELD_NUMBER: _ClassVar[int]
+    REMOVE_GROUP_IDS_FIELD_NUMBER: _ClassVar[int]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    EDITABLE_FIELD_NUMBER: _ClassVar[int]
+    name: _wrappers_pb2.StringValue
+    namespace: _wrappers_pb2.StringValue
+    metadata: _containers.ScalarMap[str, str]
+    ports: _wrappers_pb2.StringValue
     business: _wrappers_pb2.StringValue
+    department: _wrappers_pb2.StringValue
     cmdb_mod1: _wrappers_pb2.StringValue
     cmdb_mod2: _wrappers_pb2.StringValue
     cmdb_mod3: _wrappers_pb2.StringValue
     comment: _wrappers_pb2.StringValue
+    owners: _wrappers_pb2.StringValue
+    token: _wrappers_pb2.StringValue
     ctime: _wrappers_pb2.StringValue
-    department: _wrappers_pb2.StringValue
-    editable: _wrappers_pb2.BoolValue
-    group_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
-    healthy_instance_count: _wrappers_pb2.UInt32Value
-    id: _wrappers_pb2.StringValue
-    metadata: _containers.ScalarMap[str, str]
     mtime: _wrappers_pb2.StringValue
-    name: _wrappers_pb2.StringValue
-    namespace: _wrappers_pb2.StringValue
-    owners: _wrappers_pb2.StringValue
-    platform_id: _wrappers_pb2.StringValue
-    ports: _wrappers_pb2.StringValue
-    remove_group_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
-    remove_user_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
     revision: _wrappers_pb2.StringValue
-    token: _wrappers_pb2.StringValue
+    platform_id: _wrappers_pb2.StringValue
     total_instance_count: _wrappers_pb2.UInt32Value
+    healthy_instance_count: _wrappers_pb2.UInt32Value
     user_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
+    group_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
+    remove_user_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
+    remove_group_ids: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
+    id: _wrappers_pb2.StringValue
+    editable: _wrappers_pb2.BoolValue
     def __init__(self, name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., metadata: _Optional[_Mapping[str, str]] = ..., ports: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., business: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., department: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., cmdb_mod1: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., cmdb_mod2: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., cmdb_mod3: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., owners: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., token: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., ctime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mtime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., revision: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., platform_id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., total_instance_count: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., healthy_instance_count: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., user_ids: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ..., group_ids: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ..., remove_user_ids: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ..., remove_group_ids: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ..., id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., editable: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...) -> None: ...
 
 class ServiceAlias(_message.Message):
-    __slots__ = ["alias", "alias_namespace", "comment", "ctime", "editable", "id", "mtime", "namespace", "owners", "service", "service_token", "type"]
+    __slots__ = ["service", "namespace", "alias", "alias_namespace", "type", "owners", "comment", "service_token", "ctime", "mtime", "id", "editable"]
+    SERVICE_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
     ALIAS_FIELD_NUMBER: _ClassVar[int]
     ALIAS_NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    OWNERS_FIELD_NUMBER: _ClassVar[int]
     COMMENT_FIELD_NUMBER: _ClassVar[int]
+    SERVICE_TOKEN_FIELD_NUMBER: _ClassVar[int]
     CTIME_FIELD_NUMBER: _ClassVar[int]
-    EDITABLE_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
     MTIME_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    OWNERS_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    TYPE_FIELD_NUMBER: _ClassVar[int]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    EDITABLE_FIELD_NUMBER: _ClassVar[int]
+    service: _wrappers_pb2.StringValue
+    namespace: _wrappers_pb2.StringValue
     alias: _wrappers_pb2.StringValue
     alias_namespace: _wrappers_pb2.StringValue
+    type: AliasType
+    owners: _wrappers_pb2.StringValue
     comment: _wrappers_pb2.StringValue
+    service_token: _wrappers_pb2.StringValue
     ctime: _wrappers_pb2.StringValue
+    mtime: _wrappers_pb2.StringValue
+    id: _wrappers_pb2.StringValue
     editable: _wrappers_pb2.BoolValue
+    def __init__(self, service: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., alias: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., alias_namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., type: _Optional[_Union[AliasType, str]] = ..., owners: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., service_token: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., ctime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mtime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., editable: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...) -> None: ...
+
+class Instance(_message.Message):
+    __slots__ = ["id", "service", "namespace", "vpc_id", "host", "port", "protocol", "version", "priority", "weight", "enable_health_check", "health_check", "healthy", "isolate", "location", "metadata", "logic_set", "ctime", "mtime", "revision", "service_token"]
+    class MetadataEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    ID_FIELD_NUMBER: _ClassVar[int]
+    SERVICE_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    VPC_ID_FIELD_NUMBER: _ClassVar[int]
+    HOST_FIELD_NUMBER: _ClassVar[int]
+    PORT_FIELD_NUMBER: _ClassVar[int]
+    PROTOCOL_FIELD_NUMBER: _ClassVar[int]
+    VERSION_FIELD_NUMBER: _ClassVar[int]
+    PRIORITY_FIELD_NUMBER: _ClassVar[int]
+    WEIGHT_FIELD_NUMBER: _ClassVar[int]
+    ENABLE_HEALTH_CHECK_FIELD_NUMBER: _ClassVar[int]
+    HEALTH_CHECK_FIELD_NUMBER: _ClassVar[int]
+    HEALTHY_FIELD_NUMBER: _ClassVar[int]
+    ISOLATE_FIELD_NUMBER: _ClassVar[int]
+    LOCATION_FIELD_NUMBER: _ClassVar[int]
+    METADATA_FIELD_NUMBER: _ClassVar[int]
+    LOGIC_SET_FIELD_NUMBER: _ClassVar[int]
+    CTIME_FIELD_NUMBER: _ClassVar[int]
+    MTIME_FIELD_NUMBER: _ClassVar[int]
+    REVISION_FIELD_NUMBER: _ClassVar[int]
+    SERVICE_TOKEN_FIELD_NUMBER: _ClassVar[int]
     id: _wrappers_pb2.StringValue
-    mtime: _wrappers_pb2.StringValue
-    namespace: _wrappers_pb2.StringValue
-    owners: _wrappers_pb2.StringValue
     service: _wrappers_pb2.StringValue
+    namespace: _wrappers_pb2.StringValue
+    vpc_id: _wrappers_pb2.StringValue
+    host: _wrappers_pb2.StringValue
+    port: _wrappers_pb2.UInt32Value
+    protocol: _wrappers_pb2.StringValue
+    version: _wrappers_pb2.StringValue
+    priority: _wrappers_pb2.UInt32Value
+    weight: _wrappers_pb2.UInt32Value
+    enable_health_check: _wrappers_pb2.BoolValue
+    health_check: HealthCheck
+    healthy: _wrappers_pb2.BoolValue
+    isolate: _wrappers_pb2.BoolValue
+    location: _model_pb2.Location
+    metadata: _containers.ScalarMap[str, str]
+    logic_set: _wrappers_pb2.StringValue
+    ctime: _wrappers_pb2.StringValue
+    mtime: _wrappers_pb2.StringValue
+    revision: _wrappers_pb2.StringValue
     service_token: _wrappers_pb2.StringValue
-    type: AliasType
-    def __init__(self, service: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., alias: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., alias_namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., type: _Optional[_Union[AliasType, str]] = ..., owners: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., service_token: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., ctime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mtime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., editable: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...) -> None: ...
+    def __init__(self, id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., service: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., vpc_id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., host: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., port: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., protocol: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., version: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., priority: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., weight: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., enable_health_check: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., health_check: _Optional[_Union[HealthCheck, _Mapping]] = ..., healthy: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., isolate: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., location: _Optional[_Union[_model_pb2.Location, _Mapping]] = ..., metadata: _Optional[_Mapping[str, str]] = ..., logic_set: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., ctime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mtime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., revision: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., service_token: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
 
-class AliasType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
+class HealthCheck(_message.Message):
+    __slots__ = ["type", "heartbeat"]
+    class HealthCheckType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        UNKNOWN: _ClassVar[HealthCheck.HealthCheckType]
+        HEARTBEAT: _ClassVar[HealthCheck.HealthCheckType]
+    UNKNOWN: HealthCheck.HealthCheckType
+    HEARTBEAT: HealthCheck.HealthCheckType
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    HEARTBEAT_FIELD_NUMBER: _ClassVar[int]
+    type: HealthCheck.HealthCheckType
+    heartbeat: HeartbeatHealthCheck
+    def __init__(self, type: _Optional[_Union[HealthCheck.HealthCheckType, str]] = ..., heartbeat: _Optional[_Union[HeartbeatHealthCheck, _Mapping]] = ...) -> None: ...
+
+class HeartbeatHealthCheck(_message.Message):
+    __slots__ = ["ttl"]
+    TTL_FIELD_NUMBER: _ClassVar[int]
+    ttl: _wrappers_pb2.UInt32Value
+    def __init__(self, ttl: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ...) -> None: ...
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,74 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: ratelimit.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from ..model import model_pb2 as model__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fratelimit.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x0bmodel.proto\"T\n\tRateLimit\x12\x17\n\x05rules\x18\x01 \x03(\x0b\x32\x08.v1.Rule\x12.\n\x08revision\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xa9\x0b\n\x04Rule\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07service\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12$\n\x06subset\x18\x04 \x03(\x0b\x32\x14.v1.Rule.SubsetEntry\x12.\n\x08priority\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12#\n\x08resource\x18\x06 \x01(\x0e\x32\x11.v1.Rule.Resource\x12\x1b\n\x04type\x18\x07 \x01(\x0e\x32\r.v1.Rule.Type\x12$\n\x06labels\x18\x08 \x03(\x0b\x32\x14.v1.Rule.LabelsEntry\x12\x1b\n\x07\x61mounts\x18\t \x03(\x0b\x32\n.v1.Amount\x12,\n\x06\x61\x63tion\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x07\x64isable\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x1a\n\x06report\x18\x0c \x01(\x0b\x32\n.v1.Report\x12+\n\x05\x63time\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05mtime\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\x08revision\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x42\n\rservice_token\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\rservice_token\x12$\n\x08\x61\x64juster\x18\x11 \x01(\x0b\x32\x12.v1.AmountAdjuster\x12@\n\rregex_combine\x18\x12 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\rregex_combine\x12(\n\x0b\x61mount_mode\x18\x13 \x01(\x0e\x32\x13.v1.Rule.AmountMode\x12\'\n\x08\x66\x61ilover\x18\x14 \x01(\x0e\x32\x15.v1.Rule.FailoverType\x12%\n\x07\x63luster\x18\x15 \x01(\x0b\x32\x14.v1.RateLimitCluster\x12\x1f\n\x06method\x18\x16 \x01(\x0b\x32\x0f.v1.MatchString\x12$\n\targuments\x18\x17 \x03(\x0b\x32\x11.v1.MatchArgument\x12*\n\x04name\x18\x18 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05\x65time\x18\x19 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x46\n\x0fmax_queue_delay\x18\x1a \x01(\x0b\x32\x1c.google.protobuf.UInt32ValueR\x0fmax_queue_delay\x1a>\n\x0bSubsetEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.v1.MatchString:\x02\x38\x01\x1a>\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.v1.MatchString:\x02\x38\x01\"$\n\x08Resource\x12\x07\n\x03QPS\x10\x00\x12\x0f\n\x0b\x43ONCURRENCY\x10\x01\"\x1d\n\x04Type\x12\n\n\x06GLOBAL\x10\x00\x12\t\n\x05LOCAL\x10\x01\"1\n\nAmountMode\x12\x10\n\x0cGLOBAL_TOTAL\x10\x00\x12\x11\n\rSHARE_EQUALLY\x10\x01\"5\n\x0c\x46\x61iloverType\x12\x12\n\x0e\x46\x41ILOVER_LOCAL\x10\x00\x12\x11\n\rFAILOVER_PASS\x10\x01\"\xbc\x01\n\rMatchArgument\x12$\n\x04type\x18\x01 \x01(\x0e\x32\x16.v1.MatchArgument.Type\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\x1e\n\x05value\x18\x03 \x01(\x0b\x32\x0f.v1.MatchString\"X\n\x04Type\x12\n\n\x06\x43USTOM\x10\x00\x12\n\n\x06METHOD\x10\x01\x12\n\n\x06HEADER\x10\x02\x12\t\n\x05QUERY\x10\x03\x12\x12\n\x0e\x43\x41LLER_SERVICE\x10\x04\x12\r\n\tCALLER_IP\x10\x05\"r\n\x10RateLimitCluster\x12-\n\x07service\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\x80\x02\n\x06\x41mount\x12/\n\tmaxAmount\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x30\n\rvalidDuration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12/\n\tprecision\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x31\n\x0bstartAmount\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12/\n\tminAmount\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\"j\n\x06Report\x12+\n\x08interval\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x33\n\ramountPercent\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\"0\n\x0e\x41mountAdjuster\x12\x1e\n\x05\x63limb\x18\x01 \x01(\x0b\x32\x0f.v1.ClimbConfig\"\xec\x0b\n\x0b\x43limbConfig\x12*\n\x06\x65nable\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12,\n\x06metric\x18\x02 \x01(\x0b\x32\x1c.v1.ClimbConfig.MetricConfig\x12-\n\x06policy\x18\x03 \x01(\x0b\x32\x1d.v1.ClimbConfig.TriggerPolicy\x12\x33\n\nthrottling\x18\x04 \x01(\x0b\x32\x1f.v1.ClimbConfig.ClimbThrottling\x1a\x9d\x01\n\x0cMetricConfig\x12)\n\x06window\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12/\n\tprecision\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x31\n\x0ereportInterval\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x1a\xa7\x05\n\rTriggerPolicy\x12:\n\terrorRate\x18\x01 \x01(\x0b\x32\'.v1.ClimbConfig.TriggerPolicy.ErrorRate\x12\x38\n\x08slowRate\x18\x02 \x01(\x0b\x32&.v1.ClimbConfig.TriggerPolicy.SlowRate\x1a\x8d\x03\n\tErrorRate\x12*\n\x06\x65nable\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12<\n\x16requestVolumeThreshold\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12.\n\terrorRate\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12G\n\x08specials\x18\x04 \x03(\x0b\x32\x35.v1.ClimbConfig.TriggerPolicy.ErrorRate.SpecialConfig\x1a\x9c\x01\n\rSpecialConfig\x12*\n\x04type\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\nerrorCodes\x18\x02 \x03(\x0b\x32\x1b.google.protobuf.Int64Value\x12.\n\terrorRate\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x1a\x8f\x01\n\x08SlowRate\x12*\n\x06\x65nable\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12(\n\x05maxRt\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12-\n\x08slowRate\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x1a\xd4\x03\n\x0f\x43limbThrottling\x12:\n\x15\x63oldBelowTuneDownRate\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x38\n\x13\x63oldBelowTuneUpRate\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12:\n\x15\x63oldAboveTuneDownRate\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x38\n\x13\x63oldAboveTuneUpRate\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12;\n\x16limitThresholdToTuneUp\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x30\n\rjudgeDuration\x18\x06 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x31\n\x0ctuneUpPeriod\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x33\n\x0etuneDownPeriod\x18\x08 \x01(\x0b\x32\x1b.google.protobuf.Int32ValueB\x8f\x01\n7com.tencent.polaris.specification.api.v1.traffic.manageB\x0eRateLimitProtoZDgithub.com/polarismesh/specification/source/go/api/v1/traffic_manageb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ratelimit_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ratelimit_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n7com.tencent.polaris.specification.api.v1.traffic.manageB\016RateLimitProtoZDgithub.com/polarismesh/specification/source/go/api/v1/traffic_manage'
   _RULE_SUBSETENTRY._options = None
   _RULE_SUBSETENTRY._serialized_options = b'8\001'
   _RULE_LABELSENTRY._options = None
   _RULE_LABELSENTRY._serialized_options = b'8\001'
-  _RATELIMIT._serialized_start=100
-  _RATELIMIT._serialized_end=184
-  _RULE._serialized_start=187
-  _RULE._serialized_end=1636
-  _RULE_SUBSETENTRY._serialized_start=1335
-  _RULE_SUBSETENTRY._serialized_end=1397
-  _RULE_LABELSENTRY._serialized_start=1399
-  _RULE_LABELSENTRY._serialized_end=1461
-  _RULE_RESOURCE._serialized_start=1463
-  _RULE_RESOURCE._serialized_end=1499
-  _RULE_TYPE._serialized_start=1501
-  _RULE_TYPE._serialized_end=1530
-  _RULE_AMOUNTMODE._serialized_start=1532
-  _RULE_AMOUNTMODE._serialized_end=1581
-  _RULE_FAILOVERTYPE._serialized_start=1583
-  _RULE_FAILOVERTYPE._serialized_end=1636
-  _MATCHARGUMENT._serialized_start=1639
-  _MATCHARGUMENT._serialized_end=1827
-  _MATCHARGUMENT_TYPE._serialized_start=1739
-  _MATCHARGUMENT_TYPE._serialized_end=1827
-  _RATELIMITCLUSTER._serialized_start=1829
-  _RATELIMITCLUSTER._serialized_end=1943
-  _AMOUNT._serialized_start=1946
-  _AMOUNT._serialized_end=2202
-  _REPORT._serialized_start=2204
-  _REPORT._serialized_end=2310
-  _AMOUNTADJUSTER._serialized_start=2312
-  _AMOUNTADJUSTER._serialized_end=2360
-  _CLIMBCONFIG._serialized_start=2363
-  _CLIMBCONFIG._serialized_end=3879
-  _CLIMBCONFIG_METRICCONFIG._serialized_start=2569
-  _CLIMBCONFIG_METRICCONFIG._serialized_end=2726
-  _CLIMBCONFIG_TRIGGERPOLICY._serialized_start=2729
-  _CLIMBCONFIG_TRIGGERPOLICY._serialized_end=3408
-  _CLIMBCONFIG_TRIGGERPOLICY_ERRORRATE._serialized_start=2865
-  _CLIMBCONFIG_TRIGGERPOLICY_ERRORRATE._serialized_end=3262
-  _CLIMBCONFIG_TRIGGERPOLICY_ERRORRATE_SPECIALCONFIG._serialized_start=3106
-  _CLIMBCONFIG_TRIGGERPOLICY_ERRORRATE_SPECIALCONFIG._serialized_end=3262
-  _CLIMBCONFIG_TRIGGERPOLICY_SLOWRATE._serialized_start=3265
-  _CLIMBCONFIG_TRIGGERPOLICY_SLOWRATE._serialized_end=3408
-  _CLIMBCONFIG_CLIMBTHROTTLING._serialized_start=3411
-  _CLIMBCONFIG_CLIMBTHROTTLING._serialized_end=3879
+  _globals['_RATELIMIT']._serialized_start=100
+  _globals['_RATELIMIT']._serialized_end=184
+  _globals['_RULE']._serialized_start=187
+  _globals['_RULE']._serialized_end=1636
+  _globals['_RULE_SUBSETENTRY']._serialized_start=1335
+  _globals['_RULE_SUBSETENTRY']._serialized_end=1397
+  _globals['_RULE_LABELSENTRY']._serialized_start=1399
+  _globals['_RULE_LABELSENTRY']._serialized_end=1461
+  _globals['_RULE_RESOURCE']._serialized_start=1463
+  _globals['_RULE_RESOURCE']._serialized_end=1499
+  _globals['_RULE_TYPE']._serialized_start=1501
+  _globals['_RULE_TYPE']._serialized_end=1530
+  _globals['_RULE_AMOUNTMODE']._serialized_start=1532
+  _globals['_RULE_AMOUNTMODE']._serialized_end=1581
+  _globals['_RULE_FAILOVERTYPE']._serialized_start=1583
+  _globals['_RULE_FAILOVERTYPE']._serialized_end=1636
+  _globals['_MATCHARGUMENT']._serialized_start=1639
+  _globals['_MATCHARGUMENT']._serialized_end=1827
+  _globals['_MATCHARGUMENT_TYPE']._serialized_start=1739
+  _globals['_MATCHARGUMENT_TYPE']._serialized_end=1827
+  _globals['_RATELIMITCLUSTER']._serialized_start=1829
+  _globals['_RATELIMITCLUSTER']._serialized_end=1943
+  _globals['_AMOUNT']._serialized_start=1946
+  _globals['_AMOUNT']._serialized_end=2202
+  _globals['_REPORT']._serialized_start=2204
+  _globals['_REPORT']._serialized_end=2310
+  _globals['_AMOUNTADJUSTER']._serialized_start=2312
+  _globals['_AMOUNTADJUSTER']._serialized_end=2360
+  _globals['_CLIMBCONFIG']._serialized_start=2363
+  _globals['_CLIMBCONFIG']._serialized_end=3879
+  _globals['_CLIMBCONFIG_METRICCONFIG']._serialized_start=2569
+  _globals['_CLIMBCONFIG_METRICCONFIG']._serialized_end=2726
+  _globals['_CLIMBCONFIG_TRIGGERPOLICY']._serialized_start=2729
+  _globals['_CLIMBCONFIG_TRIGGERPOLICY']._serialized_end=3408
+  _globals['_CLIMBCONFIG_TRIGGERPOLICY_ERRORRATE']._serialized_start=2865
+  _globals['_CLIMBCONFIG_TRIGGERPOLICY_ERRORRATE']._serialized_end=3262
+  _globals['_CLIMBCONFIG_TRIGGERPOLICY_ERRORRATE_SPECIALCONFIG']._serialized_start=3106
+  _globals['_CLIMBCONFIG_TRIGGERPOLICY_ERRORRATE_SPECIALCONFIG']._serialized_end=3262
+  _globals['_CLIMBCONFIG_TRIGGERPOLICY_SLOWRATE']._serialized_start=3265
+  _globals['_CLIMBCONFIG_TRIGGERPOLICY_SLOWRATE']._serialized_end=3408
+  _globals['_CLIMBCONFIG_CLIMBTHROTTLING']._serialized_start=3411
+  _globals['_CLIMBCONFIG_CLIMBTHROTTLING']._serialized_end=3879
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -5,84 +5,207 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
+class RateLimit(_message.Message):
+    __slots__ = ["rules", "revision"]
+    RULES_FIELD_NUMBER: _ClassVar[int]
+    REVISION_FIELD_NUMBER: _ClassVar[int]
+    rules: _containers.RepeatedCompositeFieldContainer[Rule]
+    revision: _wrappers_pb2.StringValue
+    def __init__(self, rules: _Optional[_Iterable[_Union[Rule, _Mapping]]] = ..., revision: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
+
+class Rule(_message.Message):
+    __slots__ = ["id", "service", "namespace", "subset", "priority", "resource", "type", "labels", "amounts", "action", "disable", "report", "ctime", "mtime", "revision", "service_token", "adjuster", "regex_combine", "amount_mode", "failover", "cluster", "method", "arguments", "name", "etime", "max_queue_delay"]
+    class Resource(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        QPS: _ClassVar[Rule.Resource]
+        CONCURRENCY: _ClassVar[Rule.Resource]
+    QPS: Rule.Resource
+    CONCURRENCY: Rule.Resource
+    class Type(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        GLOBAL: _ClassVar[Rule.Type]
+        LOCAL: _ClassVar[Rule.Type]
+    GLOBAL: Rule.Type
+    LOCAL: Rule.Type
+    class AmountMode(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        GLOBAL_TOTAL: _ClassVar[Rule.AmountMode]
+        SHARE_EQUALLY: _ClassVar[Rule.AmountMode]
+    GLOBAL_TOTAL: Rule.AmountMode
+    SHARE_EQUALLY: Rule.AmountMode
+    class FailoverType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        FAILOVER_LOCAL: _ClassVar[Rule.FailoverType]
+        FAILOVER_PASS: _ClassVar[Rule.FailoverType]
+    FAILOVER_LOCAL: Rule.FailoverType
+    FAILOVER_PASS: Rule.FailoverType
+    class SubsetEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: _model_pb2.MatchString
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[_model_pb2.MatchString, _Mapping]] = ...) -> None: ...
+    class LabelsEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: _model_pb2.MatchString
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[_model_pb2.MatchString, _Mapping]] = ...) -> None: ...
+    ID_FIELD_NUMBER: _ClassVar[int]
+    SERVICE_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    SUBSET_FIELD_NUMBER: _ClassVar[int]
+    PRIORITY_FIELD_NUMBER: _ClassVar[int]
+    RESOURCE_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    LABELS_FIELD_NUMBER: _ClassVar[int]
+    AMOUNTS_FIELD_NUMBER: _ClassVar[int]
+    ACTION_FIELD_NUMBER: _ClassVar[int]
+    DISABLE_FIELD_NUMBER: _ClassVar[int]
+    REPORT_FIELD_NUMBER: _ClassVar[int]
+    CTIME_FIELD_NUMBER: _ClassVar[int]
+    MTIME_FIELD_NUMBER: _ClassVar[int]
+    REVISION_FIELD_NUMBER: _ClassVar[int]
+    SERVICE_TOKEN_FIELD_NUMBER: _ClassVar[int]
+    ADJUSTER_FIELD_NUMBER: _ClassVar[int]
+    REGEX_COMBINE_FIELD_NUMBER: _ClassVar[int]
+    AMOUNT_MODE_FIELD_NUMBER: _ClassVar[int]
+    FAILOVER_FIELD_NUMBER: _ClassVar[int]
+    CLUSTER_FIELD_NUMBER: _ClassVar[int]
+    METHOD_FIELD_NUMBER: _ClassVar[int]
+    ARGUMENTS_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    ETIME_FIELD_NUMBER: _ClassVar[int]
+    MAX_QUEUE_DELAY_FIELD_NUMBER: _ClassVar[int]
+    id: _wrappers_pb2.StringValue
+    service: _wrappers_pb2.StringValue
+    namespace: _wrappers_pb2.StringValue
+    subset: _containers.MessageMap[str, _model_pb2.MatchString]
+    priority: _wrappers_pb2.UInt32Value
+    resource: Rule.Resource
+    type: Rule.Type
+    labels: _containers.MessageMap[str, _model_pb2.MatchString]
+    amounts: _containers.RepeatedCompositeFieldContainer[Amount]
+    action: _wrappers_pb2.StringValue
+    disable: _wrappers_pb2.BoolValue
+    report: Report
+    ctime: _wrappers_pb2.StringValue
+    mtime: _wrappers_pb2.StringValue
+    revision: _wrappers_pb2.StringValue
+    service_token: _wrappers_pb2.StringValue
+    adjuster: AmountAdjuster
+    regex_combine: _wrappers_pb2.BoolValue
+    amount_mode: Rule.AmountMode
+    failover: Rule.FailoverType
+    cluster: RateLimitCluster
+    method: _model_pb2.MatchString
+    arguments: _containers.RepeatedCompositeFieldContainer[MatchArgument]
+    name: _wrappers_pb2.StringValue
+    etime: _wrappers_pb2.StringValue
+    max_queue_delay: _wrappers_pb2.UInt32Value
+    def __init__(self, id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., service: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., subset: _Optional[_Mapping[str, _model_pb2.MatchString]] = ..., priority: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., resource: _Optional[_Union[Rule.Resource, str]] = ..., type: _Optional[_Union[Rule.Type, str]] = ..., labels: _Optional[_Mapping[str, _model_pb2.MatchString]] = ..., amounts: _Optional[_Iterable[_Union[Amount, _Mapping]]] = ..., action: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., disable: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., report: _Optional[_Union[Report, _Mapping]] = ..., ctime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mtime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., revision: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., service_token: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., adjuster: _Optional[_Union[AmountAdjuster, _Mapping]] = ..., regex_combine: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., amount_mode: _Optional[_Union[Rule.AmountMode, str]] = ..., failover: _Optional[_Union[Rule.FailoverType, str]] = ..., cluster: _Optional[_Union[RateLimitCluster, _Mapping]] = ..., method: _Optional[_Union[_model_pb2.MatchString, _Mapping]] = ..., arguments: _Optional[_Iterable[_Union[MatchArgument, _Mapping]]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., etime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., max_queue_delay: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ...) -> None: ...
+
+class MatchArgument(_message.Message):
+    __slots__ = ["type", "key", "value"]
+    class Type(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        CUSTOM: _ClassVar[MatchArgument.Type]
+        METHOD: _ClassVar[MatchArgument.Type]
+        HEADER: _ClassVar[MatchArgument.Type]
+        QUERY: _ClassVar[MatchArgument.Type]
+        CALLER_SERVICE: _ClassVar[MatchArgument.Type]
+        CALLER_IP: _ClassVar[MatchArgument.Type]
+    CUSTOM: MatchArgument.Type
+    METHOD: MatchArgument.Type
+    HEADER: MatchArgument.Type
+    QUERY: MatchArgument.Type
+    CALLER_SERVICE: MatchArgument.Type
+    CALLER_IP: MatchArgument.Type
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    KEY_FIELD_NUMBER: _ClassVar[int]
+    VALUE_FIELD_NUMBER: _ClassVar[int]
+    type: MatchArgument.Type
+    key: str
+    value: _model_pb2.MatchString
+    def __init__(self, type: _Optional[_Union[MatchArgument.Type, str]] = ..., key: _Optional[str] = ..., value: _Optional[_Union[_model_pb2.MatchString, _Mapping]] = ...) -> None: ...
+
+class RateLimitCluster(_message.Message):
+    __slots__ = ["service", "namespace"]
+    SERVICE_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    service: _wrappers_pb2.StringValue
+    namespace: _wrappers_pb2.StringValue
+    def __init__(self, service: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
+
 class Amount(_message.Message):
-    __slots__ = ["maxAmount", "minAmount", "precision", "startAmount", "validDuration"]
+    __slots__ = ["maxAmount", "validDuration", "precision", "startAmount", "minAmount"]
     MAXAMOUNT_FIELD_NUMBER: _ClassVar[int]
-    MINAMOUNT_FIELD_NUMBER: _ClassVar[int]
+    VALIDDURATION_FIELD_NUMBER: _ClassVar[int]
     PRECISION_FIELD_NUMBER: _ClassVar[int]
     STARTAMOUNT_FIELD_NUMBER: _ClassVar[int]
-    VALIDDURATION_FIELD_NUMBER: _ClassVar[int]
+    MINAMOUNT_FIELD_NUMBER: _ClassVar[int]
     maxAmount: _wrappers_pb2.UInt32Value
-    minAmount: _wrappers_pb2.UInt32Value
+    validDuration: _duration_pb2.Duration
     precision: _wrappers_pb2.UInt32Value
     startAmount: _wrappers_pb2.UInt32Value
-    validDuration: _duration_pb2.Duration
+    minAmount: _wrappers_pb2.UInt32Value
     def __init__(self, maxAmount: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., validDuration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., precision: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., startAmount: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., minAmount: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ...) -> None: ...
 
+class Report(_message.Message):
+    __slots__ = ["interval", "amountPercent"]
+    INTERVAL_FIELD_NUMBER: _ClassVar[int]
+    AMOUNTPERCENT_FIELD_NUMBER: _ClassVar[int]
+    interval: _duration_pb2.Duration
+    amountPercent: _wrappers_pb2.UInt32Value
+    def __init__(self, interval: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., amountPercent: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ...) -> None: ...
+
 class AmountAdjuster(_message.Message):
     __slots__ = ["climb"]
     CLIMB_FIELD_NUMBER: _ClassVar[int]
     climb: ClimbConfig
     def __init__(self, climb: _Optional[_Union[ClimbConfig, _Mapping]] = ...) -> None: ...
 
 class ClimbConfig(_message.Message):
     __slots__ = ["enable", "metric", "policy", "throttling"]
-    class ClimbThrottling(_message.Message):
-        __slots__ = ["coldAboveTuneDownRate", "coldAboveTuneUpRate", "coldBelowTuneDownRate", "coldBelowTuneUpRate", "judgeDuration", "limitThresholdToTuneUp", "tuneDownPeriod", "tuneUpPeriod"]
-        COLDABOVETUNEDOWNRATE_FIELD_NUMBER: _ClassVar[int]
-        COLDABOVETUNEUPRATE_FIELD_NUMBER: _ClassVar[int]
-        COLDBELOWTUNEDOWNRATE_FIELD_NUMBER: _ClassVar[int]
-        COLDBELOWTUNEUPRATE_FIELD_NUMBER: _ClassVar[int]
-        JUDGEDURATION_FIELD_NUMBER: _ClassVar[int]
-        LIMITTHRESHOLDTOTUNEUP_FIELD_NUMBER: _ClassVar[int]
-        TUNEDOWNPERIOD_FIELD_NUMBER: _ClassVar[int]
-        TUNEUPPERIOD_FIELD_NUMBER: _ClassVar[int]
-        coldAboveTuneDownRate: _wrappers_pb2.Int32Value
-        coldAboveTuneUpRate: _wrappers_pb2.Int32Value
-        coldBelowTuneDownRate: _wrappers_pb2.Int32Value
-        coldBelowTuneUpRate: _wrappers_pb2.Int32Value
-        judgeDuration: _duration_pb2.Duration
-        limitThresholdToTuneUp: _wrappers_pb2.Int32Value
-        tuneDownPeriod: _wrappers_pb2.Int32Value
-        tuneUpPeriod: _wrappers_pb2.Int32Value
-        def __init__(self, coldBelowTuneDownRate: _Optional[_Union[_wrappers_pb2.Int32Value, _Mapping]] = ..., coldBelowTuneUpRate: _Optional[_Union[_wrappers_pb2.Int32Value, _Mapping]] = ..., coldAboveTuneDownRate: _Optional[_Union[_wrappers_pb2.Int32Value, _Mapping]] = ..., coldAboveTuneUpRate: _Optional[_Union[_wrappers_pb2.Int32Value, _Mapping]] = ..., limitThresholdToTuneUp: _Optional[_Union[_wrappers_pb2.Int32Value, _Mapping]] = ..., judgeDuration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., tuneUpPeriod: _Optional[_Union[_wrappers_pb2.Int32Value, _Mapping]] = ..., tuneDownPeriod: _Optional[_Union[_wrappers_pb2.Int32Value, _Mapping]] = ...) -> None: ...
     class MetricConfig(_message.Message):
-        __slots__ = ["precision", "reportInterval", "window"]
+        __slots__ = ["window", "precision", "reportInterval"]
+        WINDOW_FIELD_NUMBER: _ClassVar[int]
         PRECISION_FIELD_NUMBER: _ClassVar[int]
         REPORTINTERVAL_FIELD_NUMBER: _ClassVar[int]
-        WINDOW_FIELD_NUMBER: _ClassVar[int]
+        window: _duration_pb2.Duration
         precision: _wrappers_pb2.UInt32Value
         reportInterval: _duration_pb2.Duration
-        window: _duration_pb2.Duration
         def __init__(self, window: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., precision: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., reportInterval: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ...) -> None: ...
     class TriggerPolicy(_message.Message):
         __slots__ = ["errorRate", "slowRate"]
         class ErrorRate(_message.Message):
-            __slots__ = ["enable", "errorRate", "requestVolumeThreshold", "specials"]
+            __slots__ = ["enable", "requestVolumeThreshold", "errorRate", "specials"]
             class SpecialConfig(_message.Message):
-                __slots__ = ["errorCodes", "errorRate", "type"]
+                __slots__ = ["type", "errorCodes", "errorRate"]
+                TYPE_FIELD_NUMBER: _ClassVar[int]
                 ERRORCODES_FIELD_NUMBER: _ClassVar[int]
                 ERRORRATE_FIELD_NUMBER: _ClassVar[int]
-                TYPE_FIELD_NUMBER: _ClassVar[int]
+                type: _wrappers_pb2.StringValue
                 errorCodes: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.Int64Value]
                 errorRate: _wrappers_pb2.Int32Value
-                type: _wrappers_pb2.StringValue
                 def __init__(self, type: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., errorCodes: _Optional[_Iterable[_Union[_wrappers_pb2.Int64Value, _Mapping]]] = ..., errorRate: _Optional[_Union[_wrappers_pb2.Int32Value, _Mapping]] = ...) -> None: ...
             ENABLE_FIELD_NUMBER: _ClassVar[int]
-            ERRORRATE_FIELD_NUMBER: _ClassVar[int]
             REQUESTVOLUMETHRESHOLD_FIELD_NUMBER: _ClassVar[int]
+            ERRORRATE_FIELD_NUMBER: _ClassVar[int]
             SPECIALS_FIELD_NUMBER: _ClassVar[int]
             enable: _wrappers_pb2.BoolValue
-            errorRate: _wrappers_pb2.Int32Value
             requestVolumeThreshold: _wrappers_pb2.UInt32Value
+            errorRate: _wrappers_pb2.Int32Value
             specials: _containers.RepeatedCompositeFieldContainer[ClimbConfig.TriggerPolicy.ErrorRate.SpecialConfig]
             def __init__(self, enable: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., requestVolumeThreshold: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., errorRate: _Optional[_Union[_wrappers_pb2.Int32Value, _Mapping]] = ..., specials: _Optional[_Iterable[_Union[ClimbConfig.TriggerPolicy.ErrorRate.SpecialConfig, _Mapping]]] = ...) -> None: ...
         class SlowRate(_message.Message):
             __slots__ = ["enable", "maxRt", "slowRate"]
             ENABLE_FIELD_NUMBER: _ClassVar[int]
             MAXRT_FIELD_NUMBER: _ClassVar[int]
             SLOWRATE_FIELD_NUMBER: _ClassVar[int]
@@ -91,144 +214,35 @@
             slowRate: _wrappers_pb2.Int32Value
             def __init__(self, enable: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., maxRt: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., slowRate: _Optional[_Union[_wrappers_pb2.Int32Value, _Mapping]] = ...) -> None: ...
         ERRORRATE_FIELD_NUMBER: _ClassVar[int]
         SLOWRATE_FIELD_NUMBER: _ClassVar[int]
         errorRate: ClimbConfig.TriggerPolicy.ErrorRate
         slowRate: ClimbConfig.TriggerPolicy.SlowRate
         def __init__(self, errorRate: _Optional[_Union[ClimbConfig.TriggerPolicy.ErrorRate, _Mapping]] = ..., slowRate: _Optional[_Union[ClimbConfig.TriggerPolicy.SlowRate, _Mapping]] = ...) -> None: ...
+    class ClimbThrottling(_message.Message):
+        __slots__ = ["coldBelowTuneDownRate", "coldBelowTuneUpRate", "coldAboveTuneDownRate", "coldAboveTuneUpRate", "limitThresholdToTuneUp", "judgeDuration", "tuneUpPeriod", "tuneDownPeriod"]
+        COLDBELOWTUNEDOWNRATE_FIELD_NUMBER: _ClassVar[int]
+        COLDBELOWTUNEUPRATE_FIELD_NUMBER: _ClassVar[int]
+        COLDABOVETUNEDOWNRATE_FIELD_NUMBER: _ClassVar[int]
+        COLDABOVETUNEUPRATE_FIELD_NUMBER: _ClassVar[int]
+        LIMITTHRESHOLDTOTUNEUP_FIELD_NUMBER: _ClassVar[int]
+        JUDGEDURATION_FIELD_NUMBER: _ClassVar[int]
+        TUNEUPPERIOD_FIELD_NUMBER: _ClassVar[int]
+        TUNEDOWNPERIOD_FIELD_NUMBER: _ClassVar[int]
+        coldBelowTuneDownRate: _wrappers_pb2.Int32Value
+        coldBelowTuneUpRate: _wrappers_pb2.Int32Value
+        coldAboveTuneDownRate: _wrappers_pb2.Int32Value
+        coldAboveTuneUpRate: _wrappers_pb2.Int32Value
+        limitThresholdToTuneUp: _wrappers_pb2.Int32Value
+        judgeDuration: _duration_pb2.Duration
+        tuneUpPeriod: _wrappers_pb2.Int32Value
+        tuneDownPeriod: _wrappers_pb2.Int32Value
+        def __init__(self, coldBelowTuneDownRate: _Optional[_Union[_wrappers_pb2.Int32Value, _Mapping]] = ..., coldBelowTuneUpRate: _Optional[_Union[_wrappers_pb2.Int32Value, _Mapping]] = ..., coldAboveTuneDownRate: _Optional[_Union[_wrappers_pb2.Int32Value, _Mapping]] = ..., coldAboveTuneUpRate: _Optional[_Union[_wrappers_pb2.Int32Value, _Mapping]] = ..., limitThresholdToTuneUp: _Optional[_Union[_wrappers_pb2.Int32Value, _Mapping]] = ..., judgeDuration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., tuneUpPeriod: _Optional[_Union[_wrappers_pb2.Int32Value, _Mapping]] = ..., tuneDownPeriod: _Optional[_Union[_wrappers_pb2.Int32Value, _Mapping]] = ...) -> None: ...
     ENABLE_FIELD_NUMBER: _ClassVar[int]
     METRIC_FIELD_NUMBER: _ClassVar[int]
     POLICY_FIELD_NUMBER: _ClassVar[int]
     THROTTLING_FIELD_NUMBER: _ClassVar[int]
     enable: _wrappers_pb2.BoolValue
     metric: ClimbConfig.MetricConfig
     policy: ClimbConfig.TriggerPolicy
     throttling: ClimbConfig.ClimbThrottling
     def __init__(self, enable: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., metric: _Optional[_Union[ClimbConfig.MetricConfig, _Mapping]] = ..., policy: _Optional[_Union[ClimbConfig.TriggerPolicy, _Mapping]] = ..., throttling: _Optional[_Union[ClimbConfig.ClimbThrottling, _Mapping]] = ...) -> None: ...
-
-class MatchArgument(_message.Message):
-    __slots__ = ["key", "type", "value"]
-    class Type(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    CALLER_IP: MatchArgument.Type
-    CALLER_SERVICE: MatchArgument.Type
-    CUSTOM: MatchArgument.Type
-    HEADER: MatchArgument.Type
-    KEY_FIELD_NUMBER: _ClassVar[int]
-    METHOD: MatchArgument.Type
-    QUERY: MatchArgument.Type
-    TYPE_FIELD_NUMBER: _ClassVar[int]
-    VALUE_FIELD_NUMBER: _ClassVar[int]
-    key: str
-    type: MatchArgument.Type
-    value: _model_pb2.MatchString
-    def __init__(self, type: _Optional[_Union[MatchArgument.Type, str]] = ..., key: _Optional[str] = ..., value: _Optional[_Union[_model_pb2.MatchString, _Mapping]] = ...) -> None: ...
-
-class RateLimit(_message.Message):
-    __slots__ = ["revision", "rules"]
-    REVISION_FIELD_NUMBER: _ClassVar[int]
-    RULES_FIELD_NUMBER: _ClassVar[int]
-    revision: _wrappers_pb2.StringValue
-    rules: _containers.RepeatedCompositeFieldContainer[Rule]
-    def __init__(self, rules: _Optional[_Iterable[_Union[Rule, _Mapping]]] = ..., revision: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
-
-class RateLimitCluster(_message.Message):
-    __slots__ = ["namespace", "service"]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_FIELD_NUMBER: _ClassVar[int]
-    namespace: _wrappers_pb2.StringValue
-    service: _wrappers_pb2.StringValue
-    def __init__(self, service: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
-
-class Report(_message.Message):
-    __slots__ = ["amountPercent", "interval"]
-    AMOUNTPERCENT_FIELD_NUMBER: _ClassVar[int]
-    INTERVAL_FIELD_NUMBER: _ClassVar[int]
-    amountPercent: _wrappers_pb2.UInt32Value
-    interval: _duration_pb2.Duration
-    def __init__(self, interval: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., amountPercent: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ...) -> None: ...
-
-class Rule(_message.Message):
-    __slots__ = ["action", "adjuster", "amount_mode", "amounts", "arguments", "cluster", "ctime", "disable", "etime", "failover", "id", "labels", "max_queue_delay", "method", "mtime", "name", "namespace", "priority", "regex_combine", "report", "resource", "revision", "service", "service_token", "subset", "type"]
-    class AmountMode(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    class FailoverType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    class Resource(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    class Type(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    class LabelsEntry(_message.Message):
-        __slots__ = ["key", "value"]
-        KEY_FIELD_NUMBER: _ClassVar[int]
-        VALUE_FIELD_NUMBER: _ClassVar[int]
-        key: str
-        value: _model_pb2.MatchString
-        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[_model_pb2.MatchString, _Mapping]] = ...) -> None: ...
-    class SubsetEntry(_message.Message):
-        __slots__ = ["key", "value"]
-        KEY_FIELD_NUMBER: _ClassVar[int]
-        VALUE_FIELD_NUMBER: _ClassVar[int]
-        key: str
-        value: _model_pb2.MatchString
-        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[_model_pb2.MatchString, _Mapping]] = ...) -> None: ...
-    ACTION_FIELD_NUMBER: _ClassVar[int]
-    ADJUSTER_FIELD_NUMBER: _ClassVar[int]
-    AMOUNTS_FIELD_NUMBER: _ClassVar[int]
-    AMOUNT_MODE_FIELD_NUMBER: _ClassVar[int]
-    ARGUMENTS_FIELD_NUMBER: _ClassVar[int]
-    CLUSTER_FIELD_NUMBER: _ClassVar[int]
-    CONCURRENCY: Rule.Resource
-    CTIME_FIELD_NUMBER: _ClassVar[int]
-    DISABLE_FIELD_NUMBER: _ClassVar[int]
-    ETIME_FIELD_NUMBER: _ClassVar[int]
-    FAILOVER_FIELD_NUMBER: _ClassVar[int]
-    FAILOVER_LOCAL: Rule.FailoverType
-    FAILOVER_PASS: Rule.FailoverType
-    GLOBAL: Rule.Type
-    GLOBAL_TOTAL: Rule.AmountMode
-    ID_FIELD_NUMBER: _ClassVar[int]
-    LABELS_FIELD_NUMBER: _ClassVar[int]
-    LOCAL: Rule.Type
-    MAX_QUEUE_DELAY_FIELD_NUMBER: _ClassVar[int]
-    METHOD_FIELD_NUMBER: _ClassVar[int]
-    MTIME_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    PRIORITY_FIELD_NUMBER: _ClassVar[int]
-    QPS: Rule.Resource
-    REGEX_COMBINE_FIELD_NUMBER: _ClassVar[int]
-    REPORT_FIELD_NUMBER: _ClassVar[int]
-    RESOURCE_FIELD_NUMBER: _ClassVar[int]
-    REVISION_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    SHARE_EQUALLY: Rule.AmountMode
-    SUBSET_FIELD_NUMBER: _ClassVar[int]
-    TYPE_FIELD_NUMBER: _ClassVar[int]
-    action: _wrappers_pb2.StringValue
-    adjuster: AmountAdjuster
-    amount_mode: Rule.AmountMode
-    amounts: _containers.RepeatedCompositeFieldContainer[Amount]
-    arguments: _containers.RepeatedCompositeFieldContainer[MatchArgument]
-    cluster: RateLimitCluster
-    ctime: _wrappers_pb2.StringValue
-    disable: _wrappers_pb2.BoolValue
-    etime: _wrappers_pb2.StringValue
-    failover: Rule.FailoverType
-    id: _wrappers_pb2.StringValue
-    labels: _containers.MessageMap[str, _model_pb2.MatchString]
-    max_queue_delay: _wrappers_pb2.UInt32Value
-    method: _model_pb2.MatchString
-    mtime: _wrappers_pb2.StringValue
-    name: _wrappers_pb2.StringValue
-    namespace: _wrappers_pb2.StringValue
-    priority: _wrappers_pb2.UInt32Value
-    regex_combine: _wrappers_pb2.BoolValue
-    report: Report
-    resource: Rule.Resource
-    revision: _wrappers_pb2.StringValue
-    service: _wrappers_pb2.StringValue
-    service_token: _wrappers_pb2.StringValue
-    subset: _containers.MessageMap[str, _model_pb2.MatchString]
-    type: Rule.Type
-    def __init__(self, id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., service: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., subset: _Optional[_Mapping[str, _model_pb2.MatchString]] = ..., priority: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., resource: _Optional[_Union[Rule.Resource, str]] = ..., type: _Optional[_Union[Rule.Type, str]] = ..., labels: _Optional[_Mapping[str, _model_pb2.MatchString]] = ..., amounts: _Optional[_Iterable[_Union[Amount, _Mapping]]] = ..., action: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., disable: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., report: _Optional[_Union[Report, _Mapping]] = ..., ctime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mtime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., revision: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., service_token: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., adjuster: _Optional[_Union[AmountAdjuster, _Mapping]] = ..., regex_combine: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., amount_mode: _Optional[_Union[Rule.AmountMode, str]] = ..., failover: _Optional[_Union[Rule.FailoverType, str]] = ..., cluster: _Optional[_Union[RateLimitCluster, _Mapping]] = ..., method: _Optional[_Union[_model_pb2.MatchString, _Mapping]] = ..., arguments: _Optional[_Iterable[_Union[MatchArgument, _Mapping]]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., etime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., max_queue_delay: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ...) -> None: ...
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: routing.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from ..model import model_pb2 as model__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rrouting.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x19google/protobuf/any.proto\x1a\x0bmodel.proto\"\x96\x03\n\x07Routing\x12-\n\x07service\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1b\n\x08inbounds\x18\x03 \x03(\x0b\x32\t.v1.Route\x12\x1c\n\toutbounds\x18\x04 \x03(\x0b\x32\t.v1.Route\x12+\n\x05\x63time\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05mtime\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\x08revision\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x42\n\rservice_token\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\rservice_token\x12\x1c\n\x05rules\x18\x15 \x03(\x0b\x32\r.v1.RouteRuleJ\x04\x08\t\x10\x15\"\xad\x01\n\x05Route\x12\x1b\n\x07sources\x18\x01 \x03(\x0b\x32\n.v1.Source\x12%\n\x0c\x64\x65stinations\x18\x02 \x03(\x0b\x32\x0f.v1.Destination\x12-\n\nextendInfo\x18\x03 \x03(\x0b\x32\x19.v1.Route.ExtendInfoEntry\x1a\x31\n\x0f\x45xtendInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xd6\x01\n\x06Source\x12-\n\x07service\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x08metadata\x18\x03 \x03(\x0b\x32\x18.v1.Source.MetadataEntry\x1a@\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.v1.MatchString:\x02\x38\x01\"\xc7\x03\n\x0b\x44\x65stination\x12-\n\x07service\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\x08metadata\x18\x03 \x03(\x0b\x32\x1d.v1.Destination.MetadataEntry\x12.\n\x08priority\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12,\n\x06weight\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12.\n\x08transfer\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x07isolate\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12*\n\x04name\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x1a@\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.v1.MatchString:\x02\x38\x01\"\x8d\x03\n\tRouteRule\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0e\n\x06\x65nable\x18\x04 \x01(\x08\x12\x39\n\x0erouting_policy\x18\x05 \x01(\x0e\x32\x11.v1.RoutingPolicyR\x0erouting_policy\x12<\n\x0erouting_config\x18\x06 \x01(\x0b\x32\x14.google.protobuf.AnyR\x0erouting_config\x12\x10\n\x08revision\x18\x07 \x01(\t\x12\r\n\x05\x63time\x18\x08 \x01(\t\x12\r\n\x05mtime\x18\t \x01(\t\x12\r\n\x05\x65time\x18\n \x01(\t\x12\x10\n\x08priority\x18\x0b \x01(\r\x12\x13\n\x0b\x64\x65scription\x18\x0c \x01(\t\x12\x31\n\nextendInfo\x18\x14 \x03(\x0b\x32\x1d.v1.RouteRule.ExtendInfoEntry\x1a\x31\n\x0f\x45xtendInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe5\x01\n\x10MetadataFailover\x12:\n\x0e\x66\x61ilover_range\x18\x01 \x01(\x0e\x32\".v1.MetadataFailover.FailoverRange\x12\x30\n\x06labels\x18\x02 \x03(\x0b\x32 .v1.MetadataFailover.LabelsEntry\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"4\n\rFailoverRange\x12\x07\n\x03\x41LL\x10\x00\x12\n\n\x06OTHERS\x10\x01\x12\x0e\n\nOTHER_KEYS\x10\x02\"\xc9\x01\n\x15MetadataRoutingConfig\x12\x0f\n\x07service\x18\x01 \x01(\t\x12\x11\n\tnamespace\x18\x02 \x01(\t\x12\x35\n\x06labels\x18\x03 \x03(\x0b\x32%.v1.MetadataRoutingConfig.LabelsEntry\x12&\n\x08\x66\x61ilover\x18\x04 \x01(\x0b\x32\x14.v1.MetadataFailover\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x86\x01\n\x11RuleRoutingConfig\x12\"\n\x07sources\x18\x01 \x03(\x0b\x32\x11.v1.SourceService\x12*\n\x0c\x64\x65stinations\x18\x02 \x03(\x0b\x32\x14.v1.DestinationGroup\x12!\n\x05rules\x18\x03 \x03(\x0b\x32\x12.v1.SubRuleRouting\"n\n\x0eSubRuleRouting\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\"\n\x07sources\x18\x02 \x03(\x0b\x32\x11.v1.SourceService\x12*\n\x0c\x64\x65stinations\x18\x03 \x03(\x0b\x32\x14.v1.DestinationGroup\"W\n\rSourceService\x12\x0f\n\x07service\x18\x01 \x01(\t\x12\x11\n\tnamespace\x18\x02 \x01(\t\x12\"\n\targuments\x18\x03 \x03(\x0b\x32\x0f.v1.SourceMatch\"\xfb\x01\n\x10\x44\x65stinationGroup\x12\x0f\n\x07service\x18\x01 \x01(\t\x12\x11\n\tnamespace\x18\x02 \x01(\t\x12\x30\n\x06labels\x18\x03 \x03(\x0b\x32 .v1.DestinationGroup.LabelsEntry\x12\x10\n\x08priority\x18\x04 \x01(\r\x12\x0e\n\x06weight\x18\x05 \x01(\r\x12\x10\n\x08transfer\x18\x06 \x01(\t\x12\x0f\n\x07isolate\x18\x07 \x01(\x08\x12\x0c\n\x04name\x18\x08 \x01(\t\x1a>\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.v1.MatchString:\x02\x38\x01\"\xba\x01\n\x0bSourceMatch\x12\"\n\x04type\x18\x01 \x01(\x0e\x32\x14.v1.SourceMatch.Type\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\x1e\n\x05value\x18\x03 \x01(\x0b\x32\x0f.v1.MatchString\"Z\n\x04Type\x12\n\n\x06\x43USTOM\x10\x00\x12\n\n\x06METHOD\x10\x01\x12\n\n\x06HEADER\x10\x02\x12\t\n\x05QUERY\x10\x03\x12\r\n\tCALLER_IP\x10\x04\x12\x08\n\x04PATH\x10\x05\x12\n\n\x06\x43OOKIE\x10\x06*3\n\rRoutingPolicy\x12\x0e\n\nRulePolicy\x10\x00\x12\x12\n\x0eMetadataPolicy\x10\x01\x42\x8d\x01\n7com.tencent.polaris.specification.api.v1.traffic.manageB\x0cRoutingProtoZDgithub.com/polarismesh/specification/source/go/api/v1/traffic_manageb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'routing_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'routing_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n7com.tencent.polaris.specification.api.v1.traffic.manageB\014RoutingProtoZDgithub.com/polarismesh/specification/source/go/api/v1/traffic_manage'
   _ROUTE_EXTENDINFOENTRY._options = None
   _ROUTE_EXTENDINFOENTRY._serialized_options = b'8\001'
   _SOURCE_METADATAENTRY._options = None
@@ -34,52 +35,52 @@
   _ROUTERULE_EXTENDINFOENTRY._serialized_options = b'8\001'
   _METADATAFAILOVER_LABELSENTRY._options = None
   _METADATAFAILOVER_LABELSENTRY._serialized_options = b'8\001'
   _METADATAROUTINGCONFIG_LABELSENTRY._options = None
   _METADATAROUTINGCONFIG_LABELSENTRY._serialized_options = b'8\001'
   _DESTINATIONGROUP_LABELSENTRY._options = None
   _DESTINATIONGROUP_LABELSENTRY._serialized_options = b'8\001'
-  _ROUTINGPOLICY._serialized_start=2970
-  _ROUTINGPOLICY._serialized_end=3021
-  _ROUTING._serialized_start=94
-  _ROUTING._serialized_end=500
-  _ROUTE._serialized_start=503
-  _ROUTE._serialized_end=676
-  _ROUTE_EXTENDINFOENTRY._serialized_start=627
-  _ROUTE_EXTENDINFOENTRY._serialized_end=676
-  _SOURCE._serialized_start=679
-  _SOURCE._serialized_end=893
-  _SOURCE_METADATAENTRY._serialized_start=829
-  _SOURCE_METADATAENTRY._serialized_end=893
-  _DESTINATION._serialized_start=896
-  _DESTINATION._serialized_end=1351
-  _DESTINATION_METADATAENTRY._serialized_start=829
-  _DESTINATION_METADATAENTRY._serialized_end=893
-  _ROUTERULE._serialized_start=1354
-  _ROUTERULE._serialized_end=1751
-  _ROUTERULE_EXTENDINFOENTRY._serialized_start=627
-  _ROUTERULE_EXTENDINFOENTRY._serialized_end=676
-  _METADATAFAILOVER._serialized_start=1754
-  _METADATAFAILOVER._serialized_end=1983
-  _METADATAFAILOVER_LABELSENTRY._serialized_start=1884
-  _METADATAFAILOVER_LABELSENTRY._serialized_end=1929
-  _METADATAFAILOVER_FAILOVERRANGE._serialized_start=1931
-  _METADATAFAILOVER_FAILOVERRANGE._serialized_end=1983
-  _METADATAROUTINGCONFIG._serialized_start=1986
-  _METADATAROUTINGCONFIG._serialized_end=2187
-  _METADATAROUTINGCONFIG_LABELSENTRY._serialized_start=1884
-  _METADATAROUTINGCONFIG_LABELSENTRY._serialized_end=1929
-  _RULEROUTINGCONFIG._serialized_start=2190
-  _RULEROUTINGCONFIG._serialized_end=2324
-  _SUBRULEROUTING._serialized_start=2326
-  _SUBRULEROUTING._serialized_end=2436
-  _SOURCESERVICE._serialized_start=2438
-  _SOURCESERVICE._serialized_end=2525
-  _DESTINATIONGROUP._serialized_start=2528
-  _DESTINATIONGROUP._serialized_end=2779
-  _DESTINATIONGROUP_LABELSENTRY._serialized_start=2717
-  _DESTINATIONGROUP_LABELSENTRY._serialized_end=2779
-  _SOURCEMATCH._serialized_start=2782
-  _SOURCEMATCH._serialized_end=2968
-  _SOURCEMATCH_TYPE._serialized_start=2878
-  _SOURCEMATCH_TYPE._serialized_end=2968
+  _globals['_ROUTINGPOLICY']._serialized_start=2970
+  _globals['_ROUTINGPOLICY']._serialized_end=3021
+  _globals['_ROUTING']._serialized_start=94
+  _globals['_ROUTING']._serialized_end=500
+  _globals['_ROUTE']._serialized_start=503
+  _globals['_ROUTE']._serialized_end=676
+  _globals['_ROUTE_EXTENDINFOENTRY']._serialized_start=627
+  _globals['_ROUTE_EXTENDINFOENTRY']._serialized_end=676
+  _globals['_SOURCE']._serialized_start=679
+  _globals['_SOURCE']._serialized_end=893
+  _globals['_SOURCE_METADATAENTRY']._serialized_start=829
+  _globals['_SOURCE_METADATAENTRY']._serialized_end=893
+  _globals['_DESTINATION']._serialized_start=896
+  _globals['_DESTINATION']._serialized_end=1351
+  _globals['_DESTINATION_METADATAENTRY']._serialized_start=829
+  _globals['_DESTINATION_METADATAENTRY']._serialized_end=893
+  _globals['_ROUTERULE']._serialized_start=1354
+  _globals['_ROUTERULE']._serialized_end=1751
+  _globals['_ROUTERULE_EXTENDINFOENTRY']._serialized_start=627
+  _globals['_ROUTERULE_EXTENDINFOENTRY']._serialized_end=676
+  _globals['_METADATAFAILOVER']._serialized_start=1754
+  _globals['_METADATAFAILOVER']._serialized_end=1983
+  _globals['_METADATAFAILOVER_LABELSENTRY']._serialized_start=1884
+  _globals['_METADATAFAILOVER_LABELSENTRY']._serialized_end=1929
+  _globals['_METADATAFAILOVER_FAILOVERRANGE']._serialized_start=1931
+  _globals['_METADATAFAILOVER_FAILOVERRANGE']._serialized_end=1983
+  _globals['_METADATAROUTINGCONFIG']._serialized_start=1986
+  _globals['_METADATAROUTINGCONFIG']._serialized_end=2187
+  _globals['_METADATAROUTINGCONFIG_LABELSENTRY']._serialized_start=1884
+  _globals['_METADATAROUTINGCONFIG_LABELSENTRY']._serialized_end=1929
+  _globals['_RULEROUTINGCONFIG']._serialized_start=2190
+  _globals['_RULEROUTINGCONFIG']._serialized_end=2324
+  _globals['_SUBRULEROUTING']._serialized_start=2326
+  _globals['_SUBRULEROUTING']._serialized_end=2436
+  _globals['_SOURCESERVICE']._serialized_start=2438
+  _globals['_SOURCESERVICE']._serialized_end=2525
+  _globals['_DESTINATIONGROUP']._serialized_start=2528
+  _globals['_DESTINATIONGROUP']._serialized_end=2779
+  _globals['_DESTINATIONGROUP_LABELSENTRY']._serialized_start=2717
+  _globals['_DESTINATIONGROUP_LABELSENTRY']._serialized_end=2779
+  _globals['_SOURCEMATCH']._serialized_start=2782
+  _globals['_SOURCEMATCH']._serialized_end=2968
+  _globals['_SOURCEMATCH_TYPE']._serialized_start=2878
+  _globals['_SOURCEMATCH_TYPE']._serialized_end=2968
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi` & `polarismesh_specification-1.3.2a0/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,247 +4,259 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
-MetadataPolicy: RoutingPolicy
+
+class RoutingPolicy(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    RulePolicy: _ClassVar[RoutingPolicy]
+    MetadataPolicy: _ClassVar[RoutingPolicy]
 RulePolicy: RoutingPolicy
+MetadataPolicy: RoutingPolicy
 
-class Destination(_message.Message):
-    __slots__ = ["isolate", "metadata", "name", "namespace", "priority", "service", "transfer", "weight"]
+class Routing(_message.Message):
+    __slots__ = ["service", "namespace", "inbounds", "outbounds", "ctime", "mtime", "revision", "service_token", "rules"]
+    SERVICE_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    INBOUNDS_FIELD_NUMBER: _ClassVar[int]
+    OUTBOUNDS_FIELD_NUMBER: _ClassVar[int]
+    CTIME_FIELD_NUMBER: _ClassVar[int]
+    MTIME_FIELD_NUMBER: _ClassVar[int]
+    REVISION_FIELD_NUMBER: _ClassVar[int]
+    SERVICE_TOKEN_FIELD_NUMBER: _ClassVar[int]
+    RULES_FIELD_NUMBER: _ClassVar[int]
+    service: _wrappers_pb2.StringValue
+    namespace: _wrappers_pb2.StringValue
+    inbounds: _containers.RepeatedCompositeFieldContainer[Route]
+    outbounds: _containers.RepeatedCompositeFieldContainer[Route]
+    ctime: _wrappers_pb2.StringValue
+    mtime: _wrappers_pb2.StringValue
+    revision: _wrappers_pb2.StringValue
+    service_token: _wrappers_pb2.StringValue
+    rules: _containers.RepeatedCompositeFieldContainer[RouteRule]
+    def __init__(self, service: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., inbounds: _Optional[_Iterable[_Union[Route, _Mapping]]] = ..., outbounds: _Optional[_Iterable[_Union[Route, _Mapping]]] = ..., ctime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mtime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., revision: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., service_token: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., rules: _Optional[_Iterable[_Union[RouteRule, _Mapping]]] = ...) -> None: ...
+
+class Route(_message.Message):
+    __slots__ = ["sources", "destinations", "extendInfo"]
+    class ExtendInfoEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    SOURCES_FIELD_NUMBER: _ClassVar[int]
+    DESTINATIONS_FIELD_NUMBER: _ClassVar[int]
+    EXTENDINFO_FIELD_NUMBER: _ClassVar[int]
+    sources: _containers.RepeatedCompositeFieldContainer[Source]
+    destinations: _containers.RepeatedCompositeFieldContainer[Destination]
+    extendInfo: _containers.ScalarMap[str, str]
+    def __init__(self, sources: _Optional[_Iterable[_Union[Source, _Mapping]]] = ..., destinations: _Optional[_Iterable[_Union[Destination, _Mapping]]] = ..., extendInfo: _Optional[_Mapping[str, str]] = ...) -> None: ...
+
+class Source(_message.Message):
+    __slots__ = ["service", "namespace", "metadata"]
     class MetadataEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: _model_pb2.MatchString
         def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[_model_pb2.MatchString, _Mapping]] = ...) -> None: ...
-    ISOLATE_FIELD_NUMBER: _ClassVar[int]
+    SERVICE_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
     METADATA_FIELD_NUMBER: _ClassVar[int]
+    service: _wrappers_pb2.StringValue
+    namespace: _wrappers_pb2.StringValue
+    metadata: _containers.MessageMap[str, _model_pb2.MatchString]
+    def __init__(self, service: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., metadata: _Optional[_Mapping[str, _model_pb2.MatchString]] = ...) -> None: ...
+
+class Destination(_message.Message):
+    __slots__ = ["service", "namespace", "metadata", "priority", "weight", "transfer", "isolate", "name"]
+    class MetadataEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: _model_pb2.MatchString
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[_model_pb2.MatchString, _Mapping]] = ...) -> None: ...
+    SERVICE_FIELD_NUMBER: _ClassVar[int]
     NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
+    METADATA_FIELD_NUMBER: _ClassVar[int]
     PRIORITY_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_FIELD_NUMBER: _ClassVar[int]
-    TRANSFER_FIELD_NUMBER: _ClassVar[int]
     WEIGHT_FIELD_NUMBER: _ClassVar[int]
-    isolate: _wrappers_pb2.BoolValue
-    metadata: _containers.MessageMap[str, _model_pb2.MatchString]
-    name: _wrappers_pb2.StringValue
+    TRANSFER_FIELD_NUMBER: _ClassVar[int]
+    ISOLATE_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    service: _wrappers_pb2.StringValue
     namespace: _wrappers_pb2.StringValue
+    metadata: _containers.MessageMap[str, _model_pb2.MatchString]
     priority: _wrappers_pb2.UInt32Value
-    service: _wrappers_pb2.StringValue
-    transfer: _wrappers_pb2.StringValue
     weight: _wrappers_pb2.UInt32Value
+    transfer: _wrappers_pb2.StringValue
+    isolate: _wrappers_pb2.BoolValue
+    name: _wrappers_pb2.StringValue
     def __init__(self, service: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., metadata: _Optional[_Mapping[str, _model_pb2.MatchString]] = ..., priority: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., weight: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., transfer: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., isolate: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
 
-class DestinationGroup(_message.Message):
-    __slots__ = ["isolate", "labels", "name", "namespace", "priority", "service", "transfer", "weight"]
-    class LabelsEntry(_message.Message):
+class RouteRule(_message.Message):
+    __slots__ = ["id", "name", "namespace", "enable", "routing_policy", "routing_config", "revision", "ctime", "mtime", "etime", "priority", "description", "extendInfo"]
+    class ExtendInfoEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
-        value: _model_pb2.MatchString
-        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[_model_pb2.MatchString, _Mapping]] = ...) -> None: ...
-    ISOLATE_FIELD_NUMBER: _ClassVar[int]
-    LABELS_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    ENABLE_FIELD_NUMBER: _ClassVar[int]
+    ROUTING_POLICY_FIELD_NUMBER: _ClassVar[int]
+    ROUTING_CONFIG_FIELD_NUMBER: _ClassVar[int]
+    REVISION_FIELD_NUMBER: _ClassVar[int]
+    CTIME_FIELD_NUMBER: _ClassVar[int]
+    MTIME_FIELD_NUMBER: _ClassVar[int]
+    ETIME_FIELD_NUMBER: _ClassVar[int]
     PRIORITY_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_FIELD_NUMBER: _ClassVar[int]
-    TRANSFER_FIELD_NUMBER: _ClassVar[int]
-    WEIGHT_FIELD_NUMBER: _ClassVar[int]
-    isolate: bool
-    labels: _containers.MessageMap[str, _model_pb2.MatchString]
+    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
+    EXTENDINFO_FIELD_NUMBER: _ClassVar[int]
+    id: str
     name: str
     namespace: str
+    enable: bool
+    routing_policy: RoutingPolicy
+    routing_config: _any_pb2.Any
+    revision: str
+    ctime: str
+    mtime: str
+    etime: str
     priority: int
-    service: str
-    transfer: str
-    weight: int
-    def __init__(self, service: _Optional[str] = ..., namespace: _Optional[str] = ..., labels: _Optional[_Mapping[str, _model_pb2.MatchString]] = ..., priority: _Optional[int] = ..., weight: _Optional[int] = ..., transfer: _Optional[str] = ..., isolate: bool = ..., name: _Optional[str] = ...) -> None: ...
+    description: str
+    extendInfo: _containers.ScalarMap[str, str]
+    def __init__(self, id: _Optional[str] = ..., name: _Optional[str] = ..., namespace: _Optional[str] = ..., enable: bool = ..., routing_policy: _Optional[_Union[RoutingPolicy, str]] = ..., routing_config: _Optional[_Union[_any_pb2.Any, _Mapping]] = ..., revision: _Optional[str] = ..., ctime: _Optional[str] = ..., mtime: _Optional[str] = ..., etime: _Optional[str] = ..., priority: _Optional[int] = ..., description: _Optional[str] = ..., extendInfo: _Optional[_Mapping[str, str]] = ...) -> None: ...
 
 class MetadataFailover(_message.Message):
     __slots__ = ["failover_range", "labels"]
     class FailoverRange(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        ALL: _ClassVar[MetadataFailover.FailoverRange]
+        OTHERS: _ClassVar[MetadataFailover.FailoverRange]
+        OTHER_KEYS: _ClassVar[MetadataFailover.FailoverRange]
+    ALL: MetadataFailover.FailoverRange
+    OTHERS: MetadataFailover.FailoverRange
+    OTHER_KEYS: MetadataFailover.FailoverRange
     class LabelsEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
         def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
-    ALL: MetadataFailover.FailoverRange
     FAILOVER_RANGE_FIELD_NUMBER: _ClassVar[int]
     LABELS_FIELD_NUMBER: _ClassVar[int]
-    OTHERS: MetadataFailover.FailoverRange
-    OTHER_KEYS: MetadataFailover.FailoverRange
     failover_range: MetadataFailover.FailoverRange
     labels: _containers.ScalarMap[str, str]
     def __init__(self, failover_range: _Optional[_Union[MetadataFailover.FailoverRange, str]] = ..., labels: _Optional[_Mapping[str, str]] = ...) -> None: ...
 
 class MetadataRoutingConfig(_message.Message):
-    __slots__ = ["failover", "labels", "namespace", "service"]
+    __slots__ = ["service", "namespace", "labels", "failover"]
     class LabelsEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
         def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
-    FAILOVER_FIELD_NUMBER: _ClassVar[int]
-    LABELS_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
     SERVICE_FIELD_NUMBER: _ClassVar[int]
-    failover: MetadataFailover
-    labels: _containers.ScalarMap[str, str]
-    namespace: str
-    service: str
-    def __init__(self, service: _Optional[str] = ..., namespace: _Optional[str] = ..., labels: _Optional[_Mapping[str, str]] = ..., failover: _Optional[_Union[MetadataFailover, _Mapping]] = ...) -> None: ...
-
-class Route(_message.Message):
-    __slots__ = ["destinations", "extendInfo", "sources"]
-    class ExtendInfoEntry(_message.Message):
-        __slots__ = ["key", "value"]
-        KEY_FIELD_NUMBER: _ClassVar[int]
-        VALUE_FIELD_NUMBER: _ClassVar[int]
-        key: str
-        value: str
-        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
-    DESTINATIONS_FIELD_NUMBER: _ClassVar[int]
-    EXTENDINFO_FIELD_NUMBER: _ClassVar[int]
-    SOURCES_FIELD_NUMBER: _ClassVar[int]
-    destinations: _containers.RepeatedCompositeFieldContainer[Destination]
-    extendInfo: _containers.ScalarMap[str, str]
-    sources: _containers.RepeatedCompositeFieldContainer[Source]
-    def __init__(self, sources: _Optional[_Iterable[_Union[Source, _Mapping]]] = ..., destinations: _Optional[_Iterable[_Union[Destination, _Mapping]]] = ..., extendInfo: _Optional[_Mapping[str, str]] = ...) -> None: ...
-
-class RouteRule(_message.Message):
-    __slots__ = ["ctime", "description", "enable", "etime", "extendInfo", "id", "mtime", "name", "namespace", "priority", "revision", "routing_config", "routing_policy"]
-    class ExtendInfoEntry(_message.Message):
-        __slots__ = ["key", "value"]
-        KEY_FIELD_NUMBER: _ClassVar[int]
-        VALUE_FIELD_NUMBER: _ClassVar[int]
-        key: str
-        value: str
-        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
-    CTIME_FIELD_NUMBER: _ClassVar[int]
-    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    ENABLE_FIELD_NUMBER: _ClassVar[int]
-    ETIME_FIELD_NUMBER: _ClassVar[int]
-    EXTENDINFO_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    MTIME_FIELD_NUMBER: _ClassVar[int]
     NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    PRIORITY_FIELD_NUMBER: _ClassVar[int]
-    REVISION_FIELD_NUMBER: _ClassVar[int]
-    ROUTING_CONFIG_FIELD_NUMBER: _ClassVar[int]
-    ROUTING_POLICY_FIELD_NUMBER: _ClassVar[int]
-    ctime: str
-    description: str
-    enable: bool
-    etime: str
-    extendInfo: _containers.ScalarMap[str, str]
-    id: str
-    mtime: str
-    name: str
+    LABELS_FIELD_NUMBER: _ClassVar[int]
+    FAILOVER_FIELD_NUMBER: _ClassVar[int]
+    service: str
     namespace: str
-    priority: int
-    revision: str
-    routing_config: _any_pb2.Any
-    routing_policy: RoutingPolicy
-    def __init__(self, id: _Optional[str] = ..., name: _Optional[str] = ..., namespace: _Optional[str] = ..., enable: bool = ..., routing_policy: _Optional[_Union[RoutingPolicy, str]] = ..., routing_config: _Optional[_Union[_any_pb2.Any, _Mapping]] = ..., revision: _Optional[str] = ..., ctime: _Optional[str] = ..., mtime: _Optional[str] = ..., etime: _Optional[str] = ..., priority: _Optional[int] = ..., description: _Optional[str] = ..., extendInfo: _Optional[_Mapping[str, str]] = ...) -> None: ...
-
-class Routing(_message.Message):
-    __slots__ = ["ctime", "inbounds", "mtime", "namespace", "outbounds", "revision", "rules", "service", "service_token"]
-    CTIME_FIELD_NUMBER: _ClassVar[int]
-    INBOUNDS_FIELD_NUMBER: _ClassVar[int]
-    MTIME_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    OUTBOUNDS_FIELD_NUMBER: _ClassVar[int]
-    REVISION_FIELD_NUMBER: _ClassVar[int]
-    RULES_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    ctime: _wrappers_pb2.StringValue
-    inbounds: _containers.RepeatedCompositeFieldContainer[Route]
-    mtime: _wrappers_pb2.StringValue
-    namespace: _wrappers_pb2.StringValue
-    outbounds: _containers.RepeatedCompositeFieldContainer[Route]
-    revision: _wrappers_pb2.StringValue
-    rules: _containers.RepeatedCompositeFieldContainer[RouteRule]
-    service: _wrappers_pb2.StringValue
-    service_token: _wrappers_pb2.StringValue
-    def __init__(self, service: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., inbounds: _Optional[_Iterable[_Union[Route, _Mapping]]] = ..., outbounds: _Optional[_Iterable[_Union[Route, _Mapping]]] = ..., ctime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., mtime: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., revision: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., service_token: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., rules: _Optional[_Iterable[_Union[RouteRule, _Mapping]]] = ...) -> None: ...
+    labels: _containers.ScalarMap[str, str]
+    failover: MetadataFailover
+    def __init__(self, service: _Optional[str] = ..., namespace: _Optional[str] = ..., labels: _Optional[_Mapping[str, str]] = ..., failover: _Optional[_Union[MetadataFailover, _Mapping]] = ...) -> None: ...
 
 class RuleRoutingConfig(_message.Message):
-    __slots__ = ["destinations", "rules", "sources"]
+    __slots__ = ["sources", "destinations", "rules"]
+    SOURCES_FIELD_NUMBER: _ClassVar[int]
     DESTINATIONS_FIELD_NUMBER: _ClassVar[int]
     RULES_FIELD_NUMBER: _ClassVar[int]
-    SOURCES_FIELD_NUMBER: _ClassVar[int]
+    sources: _containers.RepeatedCompositeFieldContainer[SourceService]
     destinations: _containers.RepeatedCompositeFieldContainer[DestinationGroup]
     rules: _containers.RepeatedCompositeFieldContainer[SubRuleRouting]
-    sources: _containers.RepeatedCompositeFieldContainer[SourceService]
     def __init__(self, sources: _Optional[_Iterable[_Union[SourceService, _Mapping]]] = ..., destinations: _Optional[_Iterable[_Union[DestinationGroup, _Mapping]]] = ..., rules: _Optional[_Iterable[_Union[SubRuleRouting, _Mapping]]] = ...) -> None: ...
 
-class Source(_message.Message):
-    __slots__ = ["metadata", "namespace", "service"]
-    class MetadataEntry(_message.Message):
+class SubRuleRouting(_message.Message):
+    __slots__ = ["name", "sources", "destinations"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    SOURCES_FIELD_NUMBER: _ClassVar[int]
+    DESTINATIONS_FIELD_NUMBER: _ClassVar[int]
+    name: str
+    sources: _containers.RepeatedCompositeFieldContainer[SourceService]
+    destinations: _containers.RepeatedCompositeFieldContainer[DestinationGroup]
+    def __init__(self, name: _Optional[str] = ..., sources: _Optional[_Iterable[_Union[SourceService, _Mapping]]] = ..., destinations: _Optional[_Iterable[_Union[DestinationGroup, _Mapping]]] = ...) -> None: ...
+
+class SourceService(_message.Message):
+    __slots__ = ["service", "namespace", "arguments"]
+    SERVICE_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    ARGUMENTS_FIELD_NUMBER: _ClassVar[int]
+    service: str
+    namespace: str
+    arguments: _containers.RepeatedCompositeFieldContainer[SourceMatch]
+    def __init__(self, service: _Optional[str] = ..., namespace: _Optional[str] = ..., arguments: _Optional[_Iterable[_Union[SourceMatch, _Mapping]]] = ...) -> None: ...
+
+class DestinationGroup(_message.Message):
+    __slots__ = ["service", "namespace", "labels", "priority", "weight", "transfer", "isolate", "name"]
+    class LabelsEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: _model_pb2.MatchString
         def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[_model_pb2.MatchString, _Mapping]] = ...) -> None: ...
-    METADATA_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
     SERVICE_FIELD_NUMBER: _ClassVar[int]
-    metadata: _containers.MessageMap[str, _model_pb2.MatchString]
-    namespace: _wrappers_pb2.StringValue
-    service: _wrappers_pb2.StringValue
-    def __init__(self, service: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., metadata: _Optional[_Mapping[str, _model_pb2.MatchString]] = ...) -> None: ...
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    LABELS_FIELD_NUMBER: _ClassVar[int]
+    PRIORITY_FIELD_NUMBER: _ClassVar[int]
+    WEIGHT_FIELD_NUMBER: _ClassVar[int]
+    TRANSFER_FIELD_NUMBER: _ClassVar[int]
+    ISOLATE_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    service: str
+    namespace: str
+    labels: _containers.MessageMap[str, _model_pb2.MatchString]
+    priority: int
+    weight: int
+    transfer: str
+    isolate: bool
+    name: str
+    def __init__(self, service: _Optional[str] = ..., namespace: _Optional[str] = ..., labels: _Optional[_Mapping[str, _model_pb2.MatchString]] = ..., priority: _Optional[int] = ..., weight: _Optional[int] = ..., transfer: _Optional[str] = ..., isolate: bool = ..., name: _Optional[str] = ...) -> None: ...
 
 class SourceMatch(_message.Message):
-    __slots__ = ["key", "type", "value"]
+    __slots__ = ["type", "key", "value"]
     class Type(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
-    CALLER_IP: SourceMatch.Type
-    COOKIE: SourceMatch.Type
+        CUSTOM: _ClassVar[SourceMatch.Type]
+        METHOD: _ClassVar[SourceMatch.Type]
+        HEADER: _ClassVar[SourceMatch.Type]
+        QUERY: _ClassVar[SourceMatch.Type]
+        CALLER_IP: _ClassVar[SourceMatch.Type]
+        PATH: _ClassVar[SourceMatch.Type]
+        COOKIE: _ClassVar[SourceMatch.Type]
     CUSTOM: SourceMatch.Type
-    HEADER: SourceMatch.Type
-    KEY_FIELD_NUMBER: _ClassVar[int]
     METHOD: SourceMatch.Type
-    PATH: SourceMatch.Type
+    HEADER: SourceMatch.Type
     QUERY: SourceMatch.Type
+    CALLER_IP: SourceMatch.Type
+    PATH: SourceMatch.Type
+    COOKIE: SourceMatch.Type
     TYPE_FIELD_NUMBER: _ClassVar[int]
+    KEY_FIELD_NUMBER: _ClassVar[int]
     VALUE_FIELD_NUMBER: _ClassVar[int]
-    key: str
     type: SourceMatch.Type
+    key: str
     value: _model_pb2.MatchString
     def __init__(self, type: _Optional[_Union[SourceMatch.Type, str]] = ..., key: _Optional[str] = ..., value: _Optional[_Union[_model_pb2.MatchString, _Mapping]] = ...) -> None: ...
-
-class SourceService(_message.Message):
-    __slots__ = ["arguments", "namespace", "service"]
-    ARGUMENTS_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_FIELD_NUMBER: _ClassVar[int]
-    arguments: _containers.RepeatedCompositeFieldContainer[SourceMatch]
-    namespace: str
-    service: str
-    def __init__(self, service: _Optional[str] = ..., namespace: _Optional[str] = ..., arguments: _Optional[_Iterable[_Union[SourceMatch, _Mapping]]] = ...) -> None: ...
-
-class SubRuleRouting(_message.Message):
-    __slots__ = ["destinations", "name", "sources"]
-    DESTINATIONS_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    SOURCES_FIELD_NUMBER: _ClassVar[int]
-    destinations: _containers.RepeatedCompositeFieldContainer[DestinationGroup]
-    name: str
-    sources: _containers.RepeatedCompositeFieldContainer[SourceService]
-    def __init__(self, name: _Optional[str] = ..., sources: _Optional[_Iterable[_Union[SourceService, _Mapping]]] = ..., destinations: _Optional[_Iterable[_Union[DestinationGroup, _Mapping]]] = ...) -> None: ...
-
-class RoutingPolicy(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
```

### Comparing `polarismesh_specification-1.3.1/LICENSE.txt` & `polarismesh_specification-1.3.2a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.1/README.md` & `polarismesh_specification-1.3.2a0/README.md`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.1/pyproject.toml` & `polarismesh_specification-1.3.2a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.1/PKG-INFO` & `polarismesh_specification-1.3.2a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polarismesh-specification
-Version: 1.3.1
+Version: 1.3.2a0
 Project-URL: Documentation, https://github.com/polarismesh/specification#readme
 Project-URL: Issues, https://github.com/polarismesh/specification/issues
 Project-URL: Source, https://github.com/polarismesh/specification
 Author-email: "{authemail@qq.com}" <authemail@qq.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

