# Comparing `tmp/rook-0.1.98.tar.gz` & `tmp/rook-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rook-0.1.98.tar", last modified: Mon Dec  9 13:10:39 2019, max compression
+gzip compressed data, was "dist/rook-0.1.99.tar", last modified: Sun Dec 22 12:01:29 2019, max compression
```

## Comparing `rook-0.1.98.tar` & `rook-0.1.99.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook.egg-info/
--rw-r--r--   0 root         (0) root         (0)      136 2019-12-09 13:10:38.000000 rook-0.1.98/rook.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-12-09 13:10:38.000000 rook-0.1.98/rook.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     5427 2019-12-09 13:10:39.000000 rook-0.1.98/rook.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       23 2019-12-09 13:10:38.000000 rook-0.1.98/rook.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1176 2019-12-09 13:10:38.000000 rook-0.1.98/rook.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2019-12-09 13:10:26.000000 rook-0.1.98/rook.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     3223 2019-12-09 13:06:54.000000 rook-0.1.98/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/
--rw-r--r--   0 root         (0) root         (0)      612 2019-12-09 13:06:54.000000 rook-0.1.98/rook/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1930 2019-12-09 13:06:54.000000 rook-0.1.98/rook/pyspark_daemon.py
--rw-r--r--   0 root         (0) root         (0)      834 2019-12-09 13:06:54.000000 rook-0.1.98/rook/user_warnings.py
--rw-r--r--   0 root         (0) root         (0)        3 2019-12-09 13:06:54.000000 rook-0.1.98/rook/rookout-config.json
--rw-r--r--   0 root         (0) root         (0)      285 2019-12-09 13:06:54.000000 rook-0.1.98/rook/auto_start.py
--rw-r--r--   0 root         (0) root         (0)     2645 2019-12-09 13:06:54.000000 rook-0.1.98/rook/trigger_services.py
--rw-r--r--   0 root         (0) root         (0)      821 2019-12-09 13:06:54.000000 rook-0.1.98/rook/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/protobuf/
--rw-r--r--   0 root         (0) root         (0)     6859 2019-12-09 13:10:38.000000 rook-0.1.98/rook/protobuf/controller_info_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2019-12-09 13:10:38.000000 rook-0.1.98/rook/protobuf/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37926 2019-12-09 13:10:38.000000 rook-0.1.98/rook/protobuf/messages_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2903 2019-12-09 13:10:38.000000 rook-0.1.98/rook/protobuf/envelope_pb2.py
--rw-r--r--   0 root         (0) root         (0)    40997 2019-12-09 13:10:38.000000 rook-0.1.98/rook/protobuf/variant_pb2.py
--rw-r--r--   0 root         (0) root         (0)    19073 2019-12-09 13:10:38.000000 rook-0.1.98/rook/protobuf/agent_info_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/logger/
--rw-r--r--   0 root         (0) root         (0)     7248 2019-12-09 13:06:54.000000 rook-0.1.98/rook/logger/__init__.py
--rw-r--r--   0 root         (0) root         (0)       19 2019-12-09 13:06:54.000000 rook-0.1.98/rook/version.py
--rw-r--r--   0 root         (0) root         (0)     1088 2019-12-09 13:06:54.000000 rook-0.1.98/rook/git.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/native_extensions/
--rw-r--r--   0 root         (0) root         (0)      253 2019-12-09 13:06:54.000000 rook-0.1.98/rook/native_extensions/native_extensions.h
--rw-r--r--   0 root         (0) root         (0)      933 2019-12-09 13:06:54.000000 rook-0.1.98/rook/native_extensions/atfork.cc
--rw-r--r--   0 root         (0) root         (0)     2122 2019-12-09 13:06:54.000000 rook-0.1.98/rook/native_extensions/native_extensions.cc
--rw-r--r--   0 root         (0) root         (0)      258 2019-12-09 13:06:54.000000 rook-0.1.98/rook/native_extensions/atfork.h
--rw-r--r--   0 root         (0) root         (0)     2977 2019-12-09 13:06:54.000000 rook-0.1.98/rook/native_extensions/cpython_importhook.cc
--rw-r--r--   0 root         (0) root         (0)      449 2019-12-09 13:06:54.000000 rook-0.1.98/rook/native_extensions/common.h
--rw-r--r--   0 root         (0) root         (0)      396 2019-12-09 13:06:54.000000 rook-0.1.98/rook/native_extensions/cpython_importhook.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/augs/
--rw-r--r--   0 root         (0) root         (0)        0 2019-12-09 13:06:54.000000 rook-0.1.98/rook/augs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5729 2019-12-09 13:06:54.000000 rook-0.1.98/rook/augs/aug.py
--rw-r--r--   0 root         (0) root         (0)     2024 2019-12-09 13:06:54.000000 rook-0.1.98/rook/augs/augs_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/augs/conditions/
--rw-r--r--   0 root         (0) root         (0)       64 2019-12-09 13:06:54.000000 rook-0.1.98/rook/augs/conditions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      442 2019-12-09 13:06:54.000000 rook-0.1.98/rook/augs/conditions/if_condition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/augs/locations/
--rw-r--r--   0 root         (0) root         (0)      346 2019-12-09 13:06:54.000000 rook-0.1.98/rook/augs/locations/location_log_handler.py
--rw-r--r--   0 root         (0) root         (0)      227 2019-12-09 13:06:54.000000 rook-0.1.98/rook/augs/locations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4960 2019-12-09 13:06:54.000000 rook-0.1.98/rook/augs/locations/location_file_line.py
--rw-r--r--   0 root         (0) root         (0)      354 2019-12-09 13:06:54.000000 rook-0.1.98/rook/augs/locations/http_server_handler.py
--rw-r--r--   0 root         (0) root         (0)     4518 2019-12-09 13:06:54.000000 rook-0.1.98/rook/augs/aug_factory.py
--rw-r--r--   0 root         (0) root         (0)     1859 2019-12-09 13:06:54.000000 rook-0.1.98/rook/augs/aug_rate_limiter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/augs/extractors/
--rw-r--r--   0 root         (0) root         (0)       14 2019-12-09 13:06:54.000000 rook-0.1.98/rook/augs/extractors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/augs/processor_extensions/
--rw-r--r--   0 root         (0) root         (0)        0 2019-12-09 13:06:54.000000 rook-0.1.98/rook/augs/processor_extensions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/augs/processor_extensions/namespaces/
--rw-r--r--   0 root         (0) root         (0)        0 2019-12-09 13:06:54.000000 rook-0.1.98/rook/augs/processor_extensions/namespaces/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1541 2019-12-09 13:06:54.000000 rook-0.1.98/rook/augs/processor_extensions/namespaces/log_record_namespace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/augs/processor_extensions/paths/
--rw-r--r--   0 root         (0) root         (0)        0 2019-12-09 13:06:54.000000 rook-0.1.98/rook/augs/processor_extensions/paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/augs/processor_extensions/operations/
--rw-r--r--   0 root         (0) root         (0)        0 2019-12-09 13:06:54.000000 rook-0.1.98/rook/augs/processor_extensions/operations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1559 2019-12-09 13:06:54.000000 rook-0.1.98/rook/augs/processor_extensions/operations/celery_rdb.py
--rw-r--r--   0 root         (0) root         (0)     8142 2019-12-09 13:06:54.000000 rook-0.1.98/rook/augs/processor_extensions/operations/rdb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/augs/actions/
--rw-r--r--   0 root         (0) root         (0)       88 2019-12-09 13:06:54.000000 rook-0.1.98/rook/augs/actions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      692 2019-12-09 13:06:54.000000 rook-0.1.98/rook/augs/actions/action_run_processor.py
--rw-r--r--   0 root         (0) root         (0)     5244 2019-12-09 13:06:54.000000 rook-0.1.98/rook/singleton.py
--rw-r--r--   0 root         (0) root         (0)     2172 2019-12-09 13:06:54.000000 rook-0.1.98/rook/file_utils.py
--rw-r--r--   0 root         (0) root         (0)     1123 2019-12-09 13:06:54.000000 rook-0.1.98/rook/serverless.py
--rw-r--r--   0 root         (0) root         (0)     2273 2019-12-09 13:06:54.000000 rook-0.1.98/rook/atfork.py
--rw-r--r--   0 root         (0) root         (0)     2141 2019-12-09 13:06:54.000000 rook-0.1.98/rook/config.py
--rw-r--r--   0 root         (0) root         (0)      786 2019-12-09 13:06:54.000000 rook-0.1.98/rook/machine.py
--rw-r--r--   0 root         (0) root         (0)     7648 2019-12-09 13:06:54.000000 rook-0.1.98/rook/interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/processor/
--rw-r--r--   0 root         (0) root         (0)        0 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27268 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/namespace_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/processor/namespaces/
--rw-r--r--   0 root         (0) root         (0)      366 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/namespaces/error_namespace.py
--rw-r--r--   0 root         (0) root         (0)        0 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/namespaces/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2386 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/namespaces/python_utils_namespace.py
--rw-r--r--   0 root         (0) root         (0)      717 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/namespaces/dumped_primitive_namespace.py
--rw-r--r--   0 root         (0) root         (0)     3245 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/namespaces/collection_namespace.py
--rw-r--r--   0 root         (0) root         (0)      296 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/namespaces/unknown_namespace.py
--rw-r--r--   0 root         (0) root         (0)     1294 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/namespaces/delayed_namespace.py
--rw-r--r--   0 root         (0) root         (0)     1820 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/namespaces/stack_namespace.py
--rw-r--r--   0 root         (0) root         (0)       80 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/namespaces/max_depth_namespace.py
--rw-r--r--   0 root         (0) root         (0)     1942 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/namespaces/trace_namespace.py
--rw-r--r--   0 root         (0) root         (0)      907 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/namespaces/container_namespace.py
--rw-r--r--   0 root         (0) root         (0)      931 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/namespaces/namespace.py
--rw-r--r--   0 root         (0) root         (0)      183 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/namespaces/formatted_namespace.py
--rw-r--r--   0 root         (0) root         (0)     6356 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/namespaces/python_object_namespace.py
--rw-r--r--   0 root         (0) root         (0)     3727 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/namespaces/frame_namespace.py
--rw-r--r--   0 root         (0) root         (0)      751 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/namespaces/dumped_object_namespace.py
--rw-r--r--   0 root         (0) root         (0)      821 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/namespaces/code_object_namespace.py
--rw-r--r--   0 root         (0) root         (0)      650 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/namespaces/string_namespace.py
--rw-r--r--   0 root         (0) root         (0)      258 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/namespaces/user_object_namespace.py
--rw-r--r--   0 root         (0) root         (0)      156 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/namespaces/dynamic_object_namespace.py
--rw-r--r--   0 root         (0) root         (0)      729 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/paths_factory.py
--rw-r--r--   0 root         (0) root         (0)     2246 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/error.py
--rw-r--r--   0 root         (0) root         (0)      738 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/processor.py
--rw-r--r--   0 root         (0) root         (0)      455 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/operations_factory.py
--rw-r--r--   0 root         (0) root         (0)      831 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/processor_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/processor/paths/
--rw-r--r--   0 root         (0) root         (0)        0 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)   126283 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/paths/arithmetic_path_internal.py
--rw-r--r--   0 root         (0) root         (0)    18217 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/paths/arithmetic_path.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/processor/operations/
--rw-r--r--   0 root         (0) root         (0)      184 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/operations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1295 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/operations/eval.py
--rw-r--r--   0 root         (0) root         (0)      207 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/operations/return_operation.py
--rw-r--r--   0 root         (0) root         (0)      622 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/operations/_exec.py
--rw-r--r--   0 root         (0) root         (0)     1558 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/operations/set.py
--rw-r--r--   0 root         (0) root         (0)     1739 2019-12-09 13:06:54.000000 rook-0.1.98/rook/processor/operations/format.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/com_ws/
--rw-r--r--   0 root         (0) root         (0)        0 2019-12-09 13:06:54.000000 rook-0.1.98/rook/com_ws/__init__.py
--rw-r--r--   0 root         (0) root         (0)      792 2019-12-09 13:06:54.000000 rook-0.1.98/rook/com_ws/command_handler.py
--rw-r--r--   0 root         (0) root         (0)     4922 2019-12-09 13:06:54.000000 rook-0.1.98/rook/com_ws/output_ws.py
--rw-r--r--   0 root         (0) root         (0)    14405 2019-12-09 13:06:54.000000 rook-0.1.98/rook/com_ws/agent_com_ws.py
--rw-r--r--   0 root         (0) root         (0)     5475 2019-12-09 13:06:54.000000 rook-0.1.98/rook/com_ws/information.py
--rw-r--r--   0 root         (0) root         (0)     1016 2019-12-09 13:06:54.000000 rook-0.1.98/rook/com_ws/token_bucket.py
--rw-r--r--   0 root         (0) root         (0)     2174 2019-12-09 13:06:54.000000 rook-0.1.98/rook/com_ws/socketpair_compat.py
--rw-r--r--   0 root         (0) root         (0)      958 2019-12-09 13:06:54.000000 rook-0.1.98/rook/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/services/
--rw-r--r--   0 root         (0) root         (0)      233 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14838 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/import_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/services/http_server_services/
--rw-r--r--   0 root         (0) root         (0)        0 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/http_server_services/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2660 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/http_server_services/flask_tracer.py
--rw-r--r--   0 root         (0) root         (0)     1803 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/http_server_services/http_server_services.py
--rw-r--r--   0 root         (0) root         (0)     3720 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/bdb_location_service.py
--rw-r--r--   0 root         (0) root         (0)    19144 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/py_bdb.py
--rw-r--r--   0 root         (0) root         (0)     5150 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/google_bdb.py
--rw-r--r--   0 root         (0) root         (0)     7181 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/logging_location_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/services/exts/
--rw-r--r--   0 root         (0) root         (0)        0 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/
--rw-r--r--   0 root         (0) root         (0)        0 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4903 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/bytecode_breakpoint.h
--rw-r--r--   0 root         (0) root         (0)    12012 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/native_module.cc
--rw-r--r--   0 root         (0) root         (0)     5376 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/immutability_tracer.h
--rw-r--r--   0 root         (0) root         (0)     3781 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/conditional_breakpoint.cc
--rw-r--r--   0 root         (0) root         (0)     2054 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/python_callback.cc
--rw-r--r--   0 root         (0) root         (0)     5285 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/bytecode_manipulator.h
--rw-r--r--   0 root         (0) root         (0)     3612 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/rate_limit.cc
--rw-r--r--   0 root         (0) root         (0)    14679 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/immutability_tracer.cc
--rw-r--r--   0 root         (0) root         (0)     3984 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/leaky_bucket.cc
--rw-r--r--   0 root         (0) root         (0)     4231 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/leaky_bucket.h
--rw-r--r--   0 root         (0) root         (0)     2097 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/rate_limit.h
--rw-r--r--   0 root         (0) root         (0)     9286 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/python_util.h
--rw-r--r--   0 root         (0) root         (0)    28295 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/bytecode_manipulator.cc
--rw-r--r--   0 root         (0) root         (0)     3260 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/conditional_breakpoint.h
--rw-r--r--   0 root         (0) root         (0)     8984 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/module_explorer.py
--rw-r--r--   0 root         (0) root         (0)     2639 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/common.h
--rw-r--r--   0 root         (0) root         (0)     2255 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/nullable.h
--rw-r--r--   0 root         (0) root         (0)    11350 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/bytecode_breakpoint.cc
--rw-r--r--   0 root         (0) root         (0)     8248 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/python_util.cc
--rw-r--r--   0 root         (0) root         (0)     1708 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/python_callback.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/glog/
--rw-r--r--   0 root         (0) root         (0)     1170 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/glog/logging.h
--rw-r--r--   0 root         (0) root         (0)      962 2019-12-09 13:06:54.000000 rook-0.1.98/rook/services/exts/cloud_debug_python/native_module.h
--rw-r--r--   0 root         (0) root         (0)      850 2019-12-09 13:06:54.000000 rook-0.1.98/rook/rookout_json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/exceptions/
--rw-r--r--   0 root         (0) root         (0)       61 2019-12-09 13:06:54.000000 rook-0.1.98/rook/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13132 2019-12-09 13:06:54.000000 rook-0.1.98/rook/exceptions/tool_exceptions.py
--rw-r--r--   0 root         (0) root         (0)      115 2019-12-09 13:06:54.000000 rook-0.1.98/rook/exceptions/core_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-09 13:10:39.000000 rook-0.1.98/rook/configuration/
--rw-r--r--   0 root         (0) root         (0)       22 2019-12-09 13:06:54.000000 rook-0.1.98/rook/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3877 2019-12-09 13:06:54.000000 rook-0.1.98/rook/configuration/config.py
--rw-r--r--   0 root         (0) root         (0)     4147 2019-12-09 13:06:54.000000 rook-0.1.98/rook/configuration/test_config.py
--rw-r--r--   0 root         (0) root         (0)      181 2019-12-09 13:06:54.000000 rook-0.1.98/README.rst
--rw-r--r--   0 root         (0) root         (0)     1176 2019-12-09 13:10:39.000000 rook-0.1.98/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1957 2019-12-09 13:06:54.000000 rook-0.1.98/LICENSE
--rw-r--r--   0 root         (0) root         (0)      191 2019-12-09 13:06:54.000000 rook-0.1.98/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)       38 2019-12-09 13:10:39.000000 rook-0.1.98/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/
+-rw-r--r--   0 root         (0) root         (0)     2141 2019-12-22 11:58:22.000000 rook-0.1.99/rook/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/com_ws/
+-rw-r--r--   0 root         (0) root         (0)     1016 2019-12-22 11:58:22.000000 rook-0.1.99/rook/com_ws/token_bucket.py
+-rw-r--r--   0 root         (0) root         (0)      792 2019-12-22 11:58:22.000000 rook-0.1.99/rook/com_ws/command_handler.py
+-rw-r--r--   0 root         (0) root         (0)        0 2019-12-22 11:58:22.000000 rook-0.1.99/rook/com_ws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5475 2019-12-22 11:58:22.000000 rook-0.1.99/rook/com_ws/information.py
+-rw-r--r--   0 root         (0) root         (0)     4922 2019-12-22 11:58:22.000000 rook-0.1.99/rook/com_ws/output_ws.py
+-rw-r--r--   0 root         (0) root         (0)    14405 2019-12-22 11:58:22.000000 rook-0.1.99/rook/com_ws/agent_com_ws.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2019-12-22 11:58:22.000000 rook-0.1.99/rook/com_ws/socketpair_compat.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2019-12-22 11:58:22.000000 rook-0.1.99/rook/git.py
+-rw-r--r--   0 root         (0) root         (0)     1123 2019-12-22 11:58:22.000000 rook-0.1.99/rook/serverless.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/logger/
+-rw-r--r--   0 root         (0) root         (0)     7248 2019-12-22 11:58:22.000000 rook-0.1.99/rook/logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      958 2019-12-22 11:58:22.000000 rook-0.1.99/rook/factory.py
+-rw-r--r--   0 root         (0) root         (0)      834 2019-12-22 11:58:22.000000 rook-0.1.99/rook/user_warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/protobuf/
+-rw-r--r--   0 root         (0) root         (0)     6859 2019-12-22 12:01:29.000000 rook-0.1.99/rook/protobuf/controller_info_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    37926 2019-12-22 12:01:29.000000 rook-0.1.99/rook/protobuf/messages_pb2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/protobuf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40997 2019-12-22 12:01:29.000000 rook-0.1.99/rook/protobuf/variant_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    19073 2019-12-22 12:01:29.000000 rook-0.1.99/rook/protobuf/agent_info_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2903 2019-12-22 12:01:29.000000 rook-0.1.99/rook/protobuf/envelope_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/services/
+-rw-r--r--   0 root         (0) root         (0)     5150 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/google_bdb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/services/http_server_services/
+-rw-r--r--   0 root         (0) root         (0)     2660 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/http_server_services/flask_tracer.py
+-rw-r--r--   0 root         (0) root         (0)        0 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/http_server_services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/http_server_services/http_server_services.py
+-rw-r--r--   0 root         (0) root         (0)     7181 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/logging_location_service.py
+-rw-r--r--   0 root         (0) root         (0)    14838 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/import_service.py
+-rw-r--r--   0 root         (0) root         (0)      233 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/services/exts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/
+-rw-r--r--   0 root         (0) root         (0)     8984 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/module_explorer.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/nullable.h
+-rw-r--r--   0 root         (0) root         (0)      962 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/native_module.h
+-rw-r--r--   0 root         (0) root         (0)     3612 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/rate_limit.cc
+-rw-r--r--   0 root         (0) root         (0)     8248 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/python_util.cc
+-rw-r--r--   0 root         (0) root         (0)    12012 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/native_module.cc
+-rw-r--r--   0 root         (0) root         (0)    28295 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/bytecode_manipulator.cc
+-rw-r--r--   0 root         (0) root         (0)     2054 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/python_callback.cc
+-rw-r--r--   0 root         (0) root         (0)    11350 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/bytecode_breakpoint.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/glog/
+-rw-r--r--   0 root         (0) root         (0)     1170 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/glog/logging.h
+-rw-r--r--   0 root         (0) root         (0)     5285 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/bytecode_manipulator.h
+-rw-r--r--   0 root         (0) root         (0)     4903 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/bytecode_breakpoint.h
+-rw-r--r--   0 root         (0) root         (0)     9286 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/python_util.h
+-rw-r--r--   0 root         (0) root         (0)     2097 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/rate_limit.h
+-rw-r--r--   0 root         (0) root         (0)     3984 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/leaky_bucket.cc
+-rw-r--r--   0 root         (0) root         (0)        0 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5376 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/immutability_tracer.h
+-rw-r--r--   0 root         (0) root         (0)     2639 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/common.h
+-rw-r--r--   0 root         (0) root         (0)     1708 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/python_callback.h
+-rw-r--r--   0 root         (0) root         (0)    14679 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/immutability_tracer.cc
+-rw-r--r--   0 root         (0) root         (0)     4231 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/leaky_bucket.h
+-rw-r--r--   0 root         (0) root         (0)     3260 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/conditional_breakpoint.h
+-rw-r--r--   0 root         (0) root         (0)     3781 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/cloud_debug_python/conditional_breakpoint.cc
+-rw-r--r--   0 root         (0) root         (0)        0 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/exts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19144 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/py_bdb.py
+-rw-r--r--   0 root         (0) root         (0)     3720 2019-12-22 11:58:22.000000 rook-0.1.99/rook/services/bdb_location_service.py
+-rw-r--r--   0 root         (0) root         (0)     2645 2019-12-22 11:58:22.000000 rook-0.1.99/rook/trigger_services.py
+-rw-r--r--   0 root         (0) root         (0)     2172 2019-12-22 11:58:22.000000 rook-0.1.99/rook/file_utils.py
+-rw-r--r--   0 root         (0) root         (0)      821 2019-12-22 11:58:22.000000 rook-0.1.99/rook/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/exceptions/
+-rw-r--r--   0 root         (0) root         (0)    13132 2019-12-22 11:58:22.000000 rook-0.1.99/rook/exceptions/tool_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)       61 2019-12-22 11:58:22.000000 rook-0.1.99/rook/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      115 2019-12-22 11:58:22.000000 rook-0.1.99/rook/exceptions/core_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/processor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/processor/paths/
+-rw-r--r--   0 root         (0) root         (0)    18217 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/paths/arithmetic_path.py
+-rw-r--r--   0 root         (0) root         (0)        0 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   126283 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/paths/arithmetic_path_internal.py
+-rw-r--r--   0 root         (0) root         (0)      831 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/processor_factory.py
+-rw-r--r--   0 root         (0) root         (0)      729 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/paths_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/processor/operations/
+-rw-r--r--   0 root         (0) root         (0)      207 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/operations/return_operation.py
+-rw-r--r--   0 root         (0) root         (0)     1739 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/operations/format.py
+-rw-r--r--   0 root         (0) root         (0)      622 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/operations/_exec.py
+-rw-r--r--   0 root         (0) root         (0)      184 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/operations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1295 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/operations/eval.py
+-rw-r--r--   0 root         (0) root         (0)     1558 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/operations/set.py
+-rw-r--r--   0 root         (0) root         (0)        0 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27967 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/namespace_serializer.py
+-rw-r--r--   0 root         (0) root         (0)      455 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/operations_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/processor/namespaces/
+-rw-r--r--   0 root         (0) root         (0)      183 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/namespaces/formatted_namespace.py
+-rw-r--r--   0 root         (0) root         (0)     2386 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/namespaces/python_utils_namespace.py
+-rw-r--r--   0 root         (0) root         (0)     6356 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/namespaces/python_object_namespace.py
+-rw-r--r--   0 root         (0) root         (0)      751 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/namespaces/dumped_object_namespace.py
+-rw-r--r--   0 root         (0) root         (0)      650 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/namespaces/string_namespace.py
+-rw-r--r--   0 root         (0) root         (0)     3245 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/namespaces/collection_namespace.py
+-rw-r--r--   0 root         (0) root         (0)     1942 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/namespaces/trace_namespace.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/namespaces/frame_namespace.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/namespaces/stack_namespace.py
+-rw-r--r--   0 root         (0) root         (0)      366 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/namespaces/error_namespace.py
+-rw-r--r--   0 root         (0) root         (0)      821 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/namespaces/code_object_namespace.py
+-rw-r--r--   0 root         (0) root         (0)      156 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/namespaces/dynamic_object_namespace.py
+-rw-r--r--   0 root         (0) root         (0)       80 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/namespaces/max_depth_namespace.py
+-rw-r--r--   0 root         (0) root         (0)      258 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/namespaces/user_object_namespace.py
+-rw-r--r--   0 root         (0) root         (0)      931 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/namespaces/namespace.py
+-rw-r--r--   0 root         (0) root         (0)        0 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/namespaces/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1294 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/namespaces/delayed_namespace.py
+-rw-r--r--   0 root         (0) root         (0)      296 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/namespaces/unknown_namespace.py
+-rw-r--r--   0 root         (0) root         (0)      907 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/namespaces/container_namespace.py
+-rw-r--r--   0 root         (0) root         (0)      717 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/namespaces/dumped_primitive_namespace.py
+-rw-r--r--   0 root         (0) root         (0)      738 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/processor.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2019-12-22 11:58:22.000000 rook-0.1.99/rook/processor/error.py
+-rw-r--r--   0 root         (0) root         (0)      850 2019-12-22 11:58:22.000000 rook-0.1.99/rook/rookout_json.py
+-rw-r--r--   0 root         (0) root         (0)      786 2019-12-22 11:58:22.000000 rook-0.1.99/rook/machine.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2019-12-22 11:58:22.000000 rook-0.1.99/rook/atfork.py
+-rw-r--r--   0 root         (0) root         (0)       19 2019-12-22 11:58:22.000000 rook-0.1.99/rook/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/native_extensions/
+-rw-r--r--   0 root         (0) root         (0)     2977 2019-12-22 11:58:22.000000 rook-0.1.99/rook/native_extensions/cpython_importhook.cc
+-rw-r--r--   0 root         (0) root         (0)     2122 2019-12-22 11:58:22.000000 rook-0.1.99/rook/native_extensions/native_extensions.cc
+-rw-r--r--   0 root         (0) root         (0)      253 2019-12-22 11:58:22.000000 rook-0.1.99/rook/native_extensions/native_extensions.h
+-rw-r--r--   0 root         (0) root         (0)      396 2019-12-22 11:58:22.000000 rook-0.1.99/rook/native_extensions/cpython_importhook.h
+-rw-r--r--   0 root         (0) root         (0)      258 2019-12-22 11:58:22.000000 rook-0.1.99/rook/native_extensions/atfork.h
+-rw-r--r--   0 root         (0) root         (0)      449 2019-12-22 11:58:22.000000 rook-0.1.99/rook/native_extensions/common.h
+-rw-r--r--   0 root         (0) root         (0)      933 2019-12-22 11:58:22.000000 rook-0.1.99/rook/native_extensions/atfork.cc
+-rw-r--r--   0 root         (0) root         (0)      612 2019-12-22 11:58:22.000000 rook-0.1.99/rook/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      285 2019-12-22 11:58:22.000000 rook-0.1.99/rook/auto_start.py
+-rw-r--r--   0 root         (0) root         (0)        3 2019-12-22 11:58:22.000000 rook-0.1.99/rook/rookout-config.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/configuration/
+-rw-r--r--   0 root         (0) root         (0)     3877 2019-12-22 11:58:22.000000 rook-0.1.99/rook/configuration/config.py
+-rw-r--r--   0 root         (0) root         (0)     4147 2019-12-22 11:58:22.000000 rook-0.1.99/rook/configuration/test_config.py
+-rw-r--r--   0 root         (0) root         (0)       22 2019-12-22 11:58:22.000000 rook-0.1.99/rook/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5244 2019-12-22 11:58:22.000000 rook-0.1.99/rook/singleton.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2019-12-22 11:58:22.000000 rook-0.1.99/rook/pyspark_daemon.py
+-rw-r--r--   0 root         (0) root         (0)     7648 2019-12-22 11:58:22.000000 rook-0.1.99/rook/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/augs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/augs/actions/
+-rw-r--r--   0 root         (0) root         (0)       88 2019-12-22 11:58:22.000000 rook-0.1.99/rook/augs/actions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      692 2019-12-22 11:58:22.000000 rook-0.1.99/rook/augs/actions/action_run_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/augs/locations/
+-rw-r--r--   0 root         (0) root         (0)      354 2019-12-22 11:58:22.000000 rook-0.1.99/rook/augs/locations/http_server_handler.py
+-rw-r--r--   0 root         (0) root         (0)      346 2019-12-22 11:58:22.000000 rook-0.1.99/rook/augs/locations/location_log_handler.py
+-rw-r--r--   0 root         (0) root         (0)      227 2019-12-22 11:58:22.000000 rook-0.1.99/rook/augs/locations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4960 2019-12-22 11:58:22.000000 rook-0.1.99/rook/augs/locations/location_file_line.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/augs/extractors/
+-rw-r--r--   0 root         (0) root         (0)       14 2019-12-22 11:58:22.000000 rook-0.1.99/rook/augs/extractors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4518 2019-12-22 11:58:22.000000 rook-0.1.99/rook/augs/aug_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/augs/processor_extensions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/augs/processor_extensions/paths/
+-rw-r--r--   0 root         (0) root         (0)        0 2019-12-22 11:58:22.000000 rook-0.1.99/rook/augs/processor_extensions/paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/augs/processor_extensions/operations/
+-rw-r--r--   0 root         (0) root         (0)     1559 2019-12-22 11:58:22.000000 rook-0.1.99/rook/augs/processor_extensions/operations/celery_rdb.py
+-rw-r--r--   0 root         (0) root         (0)     8142 2019-12-22 11:58:22.000000 rook-0.1.99/rook/augs/processor_extensions/operations/rdb.py
+-rw-r--r--   0 root         (0) root         (0)        0 2019-12-22 11:58:22.000000 rook-0.1.99/rook/augs/processor_extensions/operations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2019-12-22 11:58:22.000000 rook-0.1.99/rook/augs/processor_extensions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/augs/processor_extensions/namespaces/
+-rw-r--r--   0 root         (0) root         (0)        0 2019-12-22 11:58:22.000000 rook-0.1.99/rook/augs/processor_extensions/namespaces/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1541 2019-12-22 11:58:22.000000 rook-0.1.99/rook/augs/processor_extensions/namespaces/log_record_namespace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook/augs/conditions/
+-rw-r--r--   0 root         (0) root         (0)      442 2019-12-22 11:58:22.000000 rook-0.1.99/rook/augs/conditions/if_condition.py
+-rw-r--r--   0 root         (0) root         (0)       64 2019-12-22 11:58:22.000000 rook-0.1.99/rook/augs/conditions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2019-12-22 11:58:22.000000 rook-0.1.99/rook/augs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1859 2019-12-22 11:58:22.000000 rook-0.1.99/rook/augs/aug_rate_limiter.py
+-rw-r--r--   0 root         (0) root         (0)     2024 2019-12-22 11:58:22.000000 rook-0.1.99/rook/augs/augs_manager.py
+-rw-r--r--   0 root         (0) root         (0)     5729 2019-12-22 11:58:22.000000 rook-0.1.99/rook/augs/aug.py
+-rw-r--r--   0 root         (0) root         (0)      181 2019-12-22 11:58:22.000000 rook-0.1.99/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-22 12:01:29.000000 rook-0.1.99/rook.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2019-12-22 12:01:18.000000 rook-0.1.99/rook.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       23 2019-12-22 12:01:29.000000 rook-0.1.99/rook.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5427 2019-12-22 12:01:29.000000 rook-0.1.99/rook.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1176 2019-12-22 12:01:29.000000 rook-0.1.99/rook.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2019-12-22 12:01:29.000000 rook-0.1.99/rook.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2019-12-22 12:01:29.000000 rook-0.1.99/rook.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     3223 2019-12-22 11:58:22.000000 rook-0.1.99/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1176 2019-12-22 12:01:29.000000 rook-0.1.99/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      191 2019-12-22 11:58:22.000000 rook-0.1.99/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)       38 2019-12-22 12:01:29.000000 rook-0.1.99/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1957 2019-12-22 11:58:22.000000 rook-0.1.99/LICENSE
```

### Comparing `rook-0.1.98/rook.egg-info/SOURCES.txt` & `rook-0.1.99/rook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook.egg-info/PKG-INFO` & `rook-0.1.99/rook.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rook
-Version: 0.1.98
+Version: 0.1.99
 Summary: Rook is a Python package for on the fly debugging and data extraction for application in production
 Home-page: http://rookout.com/
 Author: Rookout
 Author-email: liran@rookout.com
 License: https://get.rookout.com/SDK_LICENSE.pdf
 Description: Python Rook
         ==================
```

### Comparing `rook-0.1.98/setup.py` & `rook-0.1.99/setup.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/__init__.py` & `rook-0.1.99/rook/__init__.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/pyspark_daemon.py` & `rook-0.1.99/rook/pyspark_daemon.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/user_warnings.py` & `rook-0.1.99/rook/user_warnings.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/trigger_services.py` & `rook-0.1.99/rook/trigger_services.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/__main__.py` & `rook-0.1.99/rook/__main__.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/protobuf/controller_info_pb2.py` & `rook-0.1.99/rook/protobuf/controller_info_pb2.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/protobuf/messages_pb2.py` & `rook-0.1.99/rook/protobuf/messages_pb2.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/protobuf/envelope_pb2.py` & `rook-0.1.99/rook/protobuf/envelope_pb2.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/protobuf/variant_pb2.py` & `rook-0.1.99/rook/protobuf/variant_pb2.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/protobuf/agent_info_pb2.py` & `rook-0.1.99/rook/protobuf/agent_info_pb2.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/logger/__init__.py` & `rook-0.1.99/rook/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/git.py` & `rook-0.1.99/rook/git.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/native_extensions/atfork.cc` & `rook-0.1.99/rook/native_extensions/atfork.cc`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/native_extensions/native_extensions.cc` & `rook-0.1.99/rook/native_extensions/native_extensions.cc`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/native_extensions/cpython_importhook.cc` & `rook-0.1.99/rook/native_extensions/cpython_importhook.cc`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/augs/aug.py` & `rook-0.1.99/rook/augs/aug.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/augs/augs_manager.py` & `rook-0.1.99/rook/augs/augs_manager.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/augs/locations/location_file_line.py` & `rook-0.1.99/rook/augs/locations/location_file_line.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/augs/aug_factory.py` & `rook-0.1.99/rook/augs/aug_factory.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/augs/aug_rate_limiter.py` & `rook-0.1.99/rook/augs/aug_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/augs/processor_extensions/namespaces/log_record_namespace.py` & `rook-0.1.99/rook/augs/processor_extensions/namespaces/log_record_namespace.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/augs/processor_extensions/operations/celery_rdb.py` & `rook-0.1.99/rook/augs/processor_extensions/operations/celery_rdb.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/augs/processor_extensions/operations/rdb.py` & `rook-0.1.99/rook/augs/processor_extensions/operations/rdb.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/augs/actions/action_run_processor.py` & `rook-0.1.99/rook/augs/actions/action_run_processor.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/singleton.py` & `rook-0.1.99/rook/singleton.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/file_utils.py` & `rook-0.1.99/rook/file_utils.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/serverless.py` & `rook-0.1.99/rook/serverless.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/atfork.py` & `rook-0.1.99/rook/atfork.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/config.py` & `rook-0.1.99/rook/config.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/machine.py` & `rook-0.1.99/rook/machine.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/interface.py` & `rook-0.1.99/rook/interface.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/namespace_serializer.py` & `rook-0.1.99/rook/processor/namespace_serializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 import traceback
+import decimal
 from types import FunctionType, MethodType, TracebackType
 from collections import Iterable
 
 import six
 
 from google.protobuf.internal.type_checkers import Int32ValueChecker, Int64ValueChecker
 
@@ -223,20 +224,20 @@
                     except AttributeError:
                         value = None
                     self._dump_python_object(value, attribute.value, current_depth + 1, config, log_errors)
 
     try:
         BINARY_TYPES = (buffer, bytearray)
         CODE_TYPES = (FunctionType, MethodType, TypeType)
-        PRIMITIVE_TYPES = (type(None), int, long, float, str, unicode, complex) + BINARY_TYPES + CODE_TYPES + (datetime.datetime,)
+        PRIMITIVE_TYPES = (type(None), int, long, float, str, unicode, complex, decimal.Decimal) + BINARY_TYPES + CODE_TYPES + (datetime.datetime,)
 
     except NameError:
         BINARY_TYPES = (bytearray, bytes)
         CODE_TYPES = (FunctionType, MethodType, type)
-        PRIMITIVE_TYPES = (type(None), int, float, str, complex) + BINARY_TYPES + CODE_TYPES + (datetime.datetime,)
+        PRIMITIVE_TYPES = (type(None), int, float, str, complex, decimal.Decimal) + BINARY_TYPES + CODE_TYPES + (datetime.datetime,)
 
     @staticmethod
     def _is_primitive(obj):
         return isinstance(obj, NamespaceSerializer.PRIMITIVE_TYPES)
 
     def _dump_max_depth(self, namespace, variant):
         variant.variant_type = variant.VARIANT_MAX_DEPTH
@@ -261,14 +262,21 @@
             variant.variant_type = variant.VARIANT_INT
             variant.int_value = int(obj)
 
         elif isinstance(obj, float):
             variant.variant_type = variant.VARIANT_DOUBLE
             variant.double_value = float(obj)
 
+        elif isinstance(obj, decimal.Decimal):
+            serialized_decimal = str(obj)
+
+            variant.variant_type = variant.VARIANT_STRING
+            variant.string_value.original_size = len(serialized_decimal)
+            variant.string_value.value = serialized_decimal
+
         elif isinstance(obj, six.string_types):
             variant.variant_type = variant.VARIANT_STRING
             variant.string_value.original_size = len(obj)
 
             if len(obj) > max_string:
                 obj = obj[:max_string]
 
@@ -355,14 +363,15 @@
         args.name = "args"
         self._dump_python_object(exc.args, args.value, current_depth + 1, config, log_errors)
 
     def _dump_user_class(self, obj, variant, current_depth, config):
         variant.variant_type = variant.VARIANT_OBJECT
 
     def _dump_not_supported(self, obj, variant):
+        logger.warning("Unsupported type in serializer: %s".format(type(obj)))
         variant.variant_type = variant.VARIANT_UKNOWN_OBJECT
 
     def _dump_dumped_object_namespace(self, namespace, variant, log_errors):
         variant.original_type = namespace.type
 
         for key, value in six.iteritems(namespace.attributes):
             attribute = variant.attributes.add()
@@ -439,14 +448,18 @@
                 return DumpedPrimitiveNamespace(variant.long_value, variant.original_type, "int", self._load_attributes(variant))
             elif variant.variant_type == variant_pb2.Variant.VARIANT_DOUBLE:
                 return DumpedPrimitiveNamespace(variant.double_value, variant.original_type, "float", self._load_attributes(variant))
             elif variant.variant_type == variant_pb2.Variant.VARIANT_BINARY:
                 return StringNamespace(variant.binary_value.value, variant.binary_value.original_size,
                                        variant.original_type, "binary", self._load_attributes(variant))
             elif variant.variant_type == variant_pb2.Variant.VARIANT_STRING:
+                if variant.original_type == str(decimal.Decimal):
+                    return DumpedPrimitiveNamespace(
+                        decimal.Decimal(variant.string_value.value),
+                        variant.original_type, "float", self._load_attributes(variant))
                 return StringNamespace(variant.string_value.value, variant.string_value.original_size,
                                        variant.original_type, "string", self._load_attributes(variant))
             elif variant.variant_type == variant_pb2.Variant.VARIANT_TIME:
                 return DumpedPrimitiveNamespace(variant.time_value.ToDatetime(), variant.original_type,
                                                 "datetime", self._load_attributes(variant))
             elif variant.variant_type == variant_pb2.Variant.VARIANT_LIST:
                 return self._load_list(variant)
```

### Comparing `rook-0.1.98/rook/processor/namespaces/python_utils_namespace.py` & `rook-0.1.99/rook/processor/namespaces/python_utils_namespace.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/namespaces/dumped_primitive_namespace.py` & `rook-0.1.99/rook/processor/namespaces/dumped_primitive_namespace.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/namespaces/collection_namespace.py` & `rook-0.1.99/rook/processor/namespaces/collection_namespace.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/namespaces/delayed_namespace.py` & `rook-0.1.99/rook/processor/namespaces/delayed_namespace.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/namespaces/stack_namespace.py` & `rook-0.1.99/rook/processor/namespaces/stack_namespace.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/namespaces/trace_namespace.py` & `rook-0.1.99/rook/processor/namespaces/trace_namespace.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/namespaces/container_namespace.py` & `rook-0.1.99/rook/processor/namespaces/container_namespace.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/namespaces/namespace.py` & `rook-0.1.99/rook/processor/namespaces/namespace.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/namespaces/python_object_namespace.py` & `rook-0.1.99/rook/processor/namespaces/python_object_namespace.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/namespaces/frame_namespace.py` & `rook-0.1.99/rook/processor/namespaces/frame_namespace.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/namespaces/dumped_object_namespace.py` & `rook-0.1.99/rook/processor/namespaces/dumped_object_namespace.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/namespaces/code_object_namespace.py` & `rook-0.1.99/rook/processor/namespaces/code_object_namespace.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/namespaces/string_namespace.py` & `rook-0.1.99/rook/processor/namespaces/string_namespace.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/paths_factory.py` & `rook-0.1.99/rook/processor/paths_factory.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/error.py` & `rook-0.1.99/rook/processor/error.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/processor.py` & `rook-0.1.99/rook/processor/processor.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/processor_factory.py` & `rook-0.1.99/rook/processor/processor_factory.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/paths/arithmetic_path_internal.py` & `rook-0.1.99/rook/processor/paths/arithmetic_path_internal.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/paths/arithmetic_path.py` & `rook-0.1.99/rook/processor/paths/arithmetic_path.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/operations/eval.py` & `rook-0.1.99/rook/processor/operations/eval.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/operations/_exec.py` & `rook-0.1.99/rook/processor/operations/_exec.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/operations/set.py` & `rook-0.1.99/rook/processor/operations/set.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/processor/operations/format.py` & `rook-0.1.99/rook/processor/operations/format.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/com_ws/command_handler.py` & `rook-0.1.99/rook/com_ws/command_handler.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/com_ws/output_ws.py` & `rook-0.1.99/rook/com_ws/output_ws.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/com_ws/agent_com_ws.py` & `rook-0.1.99/rook/com_ws/agent_com_ws.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/com_ws/information.py` & `rook-0.1.99/rook/com_ws/information.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/com_ws/token_bucket.py` & `rook-0.1.99/rook/com_ws/token_bucket.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/com_ws/socketpair_compat.py` & `rook-0.1.99/rook/com_ws/socketpair_compat.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/factory.py` & `rook-0.1.99/rook/factory.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/import_service.py` & `rook-0.1.99/rook/services/import_service.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/http_server_services/flask_tracer.py` & `rook-0.1.99/rook/services/http_server_services/flask_tracer.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/http_server_services/http_server_services.py` & `rook-0.1.99/rook/services/http_server_services/http_server_services.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/bdb_location_service.py` & `rook-0.1.99/rook/services/bdb_location_service.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/py_bdb.py` & `rook-0.1.99/rook/services/py_bdb.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/google_bdb.py` & `rook-0.1.99/rook/services/google_bdb.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/logging_location_service.py` & `rook-0.1.99/rook/services/logging_location_service.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/bytecode_breakpoint.h` & `rook-0.1.99/rook/services/exts/cloud_debug_python/bytecode_breakpoint.h`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/native_module.cc` & `rook-0.1.99/rook/services/exts/cloud_debug_python/native_module.cc`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/immutability_tracer.h` & `rook-0.1.99/rook/services/exts/cloud_debug_python/immutability_tracer.h`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/conditional_breakpoint.cc` & `rook-0.1.99/rook/services/exts/cloud_debug_python/conditional_breakpoint.cc`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/python_callback.cc` & `rook-0.1.99/rook/services/exts/cloud_debug_python/python_callback.cc`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/bytecode_manipulator.h` & `rook-0.1.99/rook/services/exts/cloud_debug_python/bytecode_manipulator.h`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/rate_limit.cc` & `rook-0.1.99/rook/services/exts/cloud_debug_python/rate_limit.cc`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/immutability_tracer.cc` & `rook-0.1.99/rook/services/exts/cloud_debug_python/immutability_tracer.cc`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/leaky_bucket.cc` & `rook-0.1.99/rook/services/exts/cloud_debug_python/leaky_bucket.cc`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/leaky_bucket.h` & `rook-0.1.99/rook/services/exts/cloud_debug_python/leaky_bucket.h`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/rate_limit.h` & `rook-0.1.99/rook/services/exts/cloud_debug_python/rate_limit.h`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/python_util.h` & `rook-0.1.99/rook/services/exts/cloud_debug_python/python_util.h`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/bytecode_manipulator.cc` & `rook-0.1.99/rook/services/exts/cloud_debug_python/bytecode_manipulator.cc`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/conditional_breakpoint.h` & `rook-0.1.99/rook/services/exts/cloud_debug_python/conditional_breakpoint.h`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/module_explorer.py` & `rook-0.1.99/rook/services/exts/cloud_debug_python/module_explorer.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/common.h` & `rook-0.1.99/rook/services/exts/cloud_debug_python/common.h`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/nullable.h` & `rook-0.1.99/rook/services/exts/cloud_debug_python/nullable.h`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/bytecode_breakpoint.cc` & `rook-0.1.99/rook/services/exts/cloud_debug_python/bytecode_breakpoint.cc`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/python_util.cc` & `rook-0.1.99/rook/services/exts/cloud_debug_python/python_util.cc`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/python_callback.h` & `rook-0.1.99/rook/services/exts/cloud_debug_python/python_callback.h`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/glog/logging.h` & `rook-0.1.99/rook/services/exts/cloud_debug_python/glog/logging.h`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/services/exts/cloud_debug_python/native_module.h` & `rook-0.1.99/rook/services/exts/cloud_debug_python/native_module.h`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/rookout_json.py` & `rook-0.1.99/rook/rookout_json.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/exceptions/tool_exceptions.py` & `rook-0.1.99/rook/exceptions/tool_exceptions.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/configuration/config.py` & `rook-0.1.99/rook/configuration/config.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/rook/configuration/test_config.py` & `rook-0.1.99/rook/configuration/test_config.py`

 * *Files identical despite different names*

### Comparing `rook-0.1.98/PKG-INFO` & `rook-0.1.99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rook
-Version: 0.1.98
+Version: 0.1.99
 Summary: Rook is a Python package for on the fly debugging and data extraction for application in production
 Home-page: http://rookout.com/
 Author: Rookout
 Author-email: liran@rookout.com
 License: https://get.rookout.com/SDK_LICENSE.pdf
 Description: Python Rook
         ==================
```

### Comparing `rook-0.1.98/LICENSE` & `rook-0.1.99/LICENSE`

 * *Files identical despite different names*

