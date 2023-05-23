# Comparing `tmp/clickzetta-connector-0.7.3.tar.gz` & `tmp/clickzetta-connector-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickzetta-connector-0.7.3.tar", last modified: Tue May 23 06:13:37 2023, max compression
+gzip compressed data, was "clickzetta-connector-0.7.4.tar", last modified: Tue May 23 06:34:51 2023, max compression
```

## Comparing `clickzetta-connector-0.7.3.tar` & `clickzetta-connector-0.7.4.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:13:37.472121 clickzetta-connector-0.7.3/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       49 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.3/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)      421 2023-05-23 06:13:37.471982 clickzetta-connector-0.7.3/PKG-INFO
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:13:37.457841 clickzetta-connector-0.7.3/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      159 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.3/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     9899 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.3/clickzetta/_helpers.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:13:37.458526 clickzetta-connector-0.7.3/clickzetta/bulkload/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-03-20 02:30:34.000000 clickzetta-connector-0.7.3/clickzetta/bulkload/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7190 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.3/clickzetta/bulkload/bulkload_enums.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4387 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.3/clickzetta/bulkload/bulkload_stream.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    14842 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.3/clickzetta/bulkload/bulkload_writer.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      483 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.3/clickzetta/bulkload/cz_table.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    39500 2023-05-18 07:25:29.000000 clickzetta-connector-0.7.3/clickzetta/client.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:13:37.459673 clickzetta-connector-0.7.3/clickzetta/dbapi/
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1677 2022-11-05 16:51:08.000000 clickzetta-connector-0.7.3/clickzetta/dbapi/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1000 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.3/clickzetta/dbapi/_helpers.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2761 2022-12-13 11:25:14.000000 clickzetta-connector-0.7.3/clickzetta/dbapi/connection.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4100 2023-05-19 07:53:05.000000 clickzetta-connector-0.7.3/clickzetta/dbapi/cursor.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1100 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.3/clickzetta/dbapi/exceptions.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1131 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.3/clickzetta/dbapi/types.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7203 2023-03-13 07:16:08.000000 clickzetta-connector-0.7.3/clickzetta/enums.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:13:37.454906 clickzetta-connector-0.7.3/clickzetta/proto/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:13:37.466945 clickzetta-connector-0.7.3/clickzetta/proto/generated/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2488 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/account_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/account_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1623 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/block_bloom_filter_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/block_bloom_filter_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1078 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/bucket_info_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/bucket_info_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1233 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/compression_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/compression_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1739 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/connection_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/connection_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5567 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/data_type_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/data_type_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4689 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/expression_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/expression_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1251 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/file_format_type_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/file_format_type_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3623 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/file_meta_data_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/file_meta_data_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1087 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/file_system_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/file_system_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2232 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/function_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/function_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1106 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/hash_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/hash_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    18361 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/ingestion_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    20165 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/ingestion_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6794 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/input_split_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/input_split_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5520 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/job_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/job_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1683 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/job_result_cache_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/job_result_cache_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    11392 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/kudu_common_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/kudu_common_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4271 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/metadata_entity_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/metadata_entity_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1300 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/network_policy_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/network_policy_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2847 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/object_identifier_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/object_identifier_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    35572 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/operator_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/operator_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1430 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/pb_util_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/pb_util_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1130 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/property_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/property_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1861 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/rm_app_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/rm_app_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1354 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/role_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/role_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2102 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/row_operations_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/row_operations_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      944 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/schema_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/schema_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1509 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/share_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/share_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5493 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/statistics_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/statistics_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    11527 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/table_common_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/table_common_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3834 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/table_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/table_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4089 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_cluster_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_cluster_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6210 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_cluster_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_cluster_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1382 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_cluster_size_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_cluster_size_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1836 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_value_info_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_value_info_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1208 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/workspace_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/workspace_meta_pb2_grpc.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:13:37.470990 clickzetta-connector-0.7.3/clickzetta/proto/source/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      770 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/account.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1549 2023-03-16 07:43:26.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/block_bloom_filter.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      190 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/bucket_info.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1017 2023-03-16 07:44:39.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/compression.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      413 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/connection_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2033 2023-03-13 07:16:08.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/data_type.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1697 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/expression.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      284 2023-03-13 07:16:08.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/file_format_type.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1781 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/file_meta_data.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      121 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/file_system.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      643 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/function_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1007 2023-03-16 07:43:26.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/hash.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     8197 2023-05-23 06:09:29.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/ingestion.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2908 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/input_split.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2134 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/job_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/job_result_cache_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)    18379 2022-08-20 14:59:08.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/kudu_common.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1417 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/metadata_entity.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      311 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/network_policy.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1071 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/object_identifier.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)    16166 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/operator.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1805 2023-03-16 07:43:26.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/pb_util.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      157 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/property.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      515 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/rm_app_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      232 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/role_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3795 2023-03-16 07:43:26.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/row_operations.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)       81 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/schema.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      312 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/share_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2539 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/statistics.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4801 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/table_common.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1895 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/table_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2387 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/virtual_cluster.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1337 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/virtual_cluster_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      253 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/virtual_cluster_size.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1034 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/virtual_value_info.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      376 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/workspace_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     8617 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.3/clickzetta/query_result.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6368 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.3/clickzetta/schema.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3557 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.3/clickzetta/session.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4780 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.3/clickzetta/standard_sql.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2277 2022-11-09 13:50:16.000000 clickzetta-connector-0.7.3/clickzetta/table.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       21 2023-05-23 06:13:30.000000 clickzetta-connector-0.7.3/clickzetta/version.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:13:37.471813 clickzetta-connector-0.7.3/clickzetta_connector.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      421 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta_connector.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6027 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta_connector.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta_connector.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta_connector.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)      629 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta_connector.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       11 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta_connector.egg-info/top_level.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-23 06:13:37.472166 clickzetta-connector-0.7.3/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2888 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.3/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:34:51.015734 clickzetta-connector-0.7.4/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       49 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.4/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      414 2023-05-23 06:34:51.015598 clickzetta-connector-0.7.4/PKG-INFO
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:34:51.000305 clickzetta-connector-0.7.4/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      159 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.4/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     9899 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.4/clickzetta/_helpers.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:34:51.001196 clickzetta-connector-0.7.4/clickzetta/bulkload/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-03-20 02:30:34.000000 clickzetta-connector-0.7.4/clickzetta/bulkload/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7190 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.4/clickzetta/bulkload/bulkload_enums.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4387 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.4/clickzetta/bulkload/bulkload_stream.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    14842 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.4/clickzetta/bulkload/bulkload_writer.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      483 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.4/clickzetta/bulkload/cz_table.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    38185 2023-05-23 06:31:15.000000 clickzetta-connector-0.7.4/clickzetta/client.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:34:51.002511 clickzetta-connector-0.7.4/clickzetta/dbapi/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1677 2022-11-05 16:51:08.000000 clickzetta-connector-0.7.4/clickzetta/dbapi/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1000 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.4/clickzetta/dbapi/_helpers.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2761 2022-12-13 11:25:14.000000 clickzetta-connector-0.7.4/clickzetta/dbapi/connection.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4100 2023-05-19 07:53:05.000000 clickzetta-connector-0.7.4/clickzetta/dbapi/cursor.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1100 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.4/clickzetta/dbapi/exceptions.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1131 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.4/clickzetta/dbapi/types.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7203 2023-03-13 07:16:08.000000 clickzetta-connector-0.7.4/clickzetta/enums.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:34:50.997545 clickzetta-connector-0.7.4/clickzetta/proto/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:34:51.011006 clickzetta-connector-0.7.4/clickzetta/proto/generated/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2488 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/account_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/account_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1623 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/block_bloom_filter_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/block_bloom_filter_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1078 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/bucket_info_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/bucket_info_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1233 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/compression_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/compression_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1739 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/connection_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/connection_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5567 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/data_type_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/data_type_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4689 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/expression_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/expression_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1251 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/file_format_type_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/file_format_type_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3623 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/file_meta_data_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/file_meta_data_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1087 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/file_system_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/file_system_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2232 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/function_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/function_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1106 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/hash_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/hash_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    18361 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/ingestion_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    20165 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/ingestion_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6794 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/input_split_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/input_split_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5520 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/job_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/job_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1683 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/job_result_cache_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/job_result_cache_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    11392 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/kudu_common_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/kudu_common_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4271 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/metadata_entity_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/metadata_entity_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1300 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/network_policy_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/network_policy_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2847 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/object_identifier_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/object_identifier_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    35572 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/operator_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/operator_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1430 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/pb_util_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/pb_util_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1130 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/property_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/property_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1861 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/rm_app_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/rm_app_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1354 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/role_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/role_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2102 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/row_operations_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/row_operations_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      944 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/schema_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/schema_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1509 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/share_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/share_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5493 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/statistics_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/statistics_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    11527 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/table_common_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/table_common_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3834 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/table_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/table_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4089 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/virtual_cluster_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/virtual_cluster_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6210 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/virtual_cluster_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/virtual_cluster_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1382 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/virtual_cluster_size_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/virtual_cluster_size_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1836 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/virtual_value_info_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/virtual_value_info_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1208 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/workspace_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta/proto/generated/workspace_meta_pb2_grpc.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:34:51.014791 clickzetta-connector-0.7.4/clickzetta/proto/source/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      770 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/account.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1549 2023-03-16 07:43:26.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/block_bloom_filter.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      190 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/bucket_info.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1017 2023-03-16 07:44:39.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/compression.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      413 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/connection_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2033 2023-03-13 07:16:08.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/data_type.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1697 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/expression.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      284 2023-03-13 07:16:08.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/file_format_type.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1781 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/file_meta_data.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      121 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/file_system.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      643 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/function_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1007 2023-03-16 07:43:26.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/hash.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     8197 2023-05-23 06:09:29.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/ingestion.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2908 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/input_split.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2134 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/job_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/job_result_cache_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    18379 2022-08-20 14:59:08.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/kudu_common.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1417 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/metadata_entity.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      311 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/network_policy.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1071 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/object_identifier.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    16166 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/operator.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1805 2023-03-16 07:43:26.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/pb_util.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      157 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/property.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      515 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/rm_app_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      232 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/role_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3795 2023-03-16 07:43:26.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/row_operations.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       81 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/schema.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      312 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/share_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2539 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/statistics.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4801 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/table_common.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1895 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/table_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2387 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/virtual_cluster.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1337 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/virtual_cluster_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      253 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/virtual_cluster_size.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1034 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/virtual_value_info.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      376 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.4/clickzetta/proto/source/workspace_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     8617 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.4/clickzetta/query_result.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6368 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.4/clickzetta/schema.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3557 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.4/clickzetta/session.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4780 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.4/clickzetta/standard_sql.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2277 2022-11-09 13:50:16.000000 clickzetta-connector-0.7.4/clickzetta/table.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       21 2023-05-23 06:34:43.000000 clickzetta-connector-0.7.4/clickzetta/version.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:34:51.015402 clickzetta-connector-0.7.4/clickzetta_connector.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      414 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta_connector.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6027 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta_connector.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      612 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta_connector.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       11 2023-05-23 06:34:50.000000 clickzetta-connector-0.7.4/clickzetta_connector.egg-info/top_level.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-23 06:34:51.015781 clickzetta-connector-0.7.4/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2855 2023-05-23 06:34:43.000000 clickzetta-connector-0.7.4/setup.py
```

### Comparing `clickzetta-connector-0.7.3/clickzetta/_helpers.py` & `clickzetta-connector-0.7.4/clickzetta/_helpers.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/bulkload/bulkload_enums.py` & `clickzetta-connector-0.7.4/clickzetta/bulkload/bulkload_enums.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/bulkload/bulkload_stream.py` & `clickzetta-connector-0.7.4/clickzetta/bulkload/bulkload_stream.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/bulkload/bulkload_writer.py` & `clickzetta-connector-0.7.4/clickzetta/bulkload/bulkload_writer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/client.py` & `clickzetta-connector-0.7.4/clickzetta/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from __future__ import absolute_import
 from __future__ import division
 
 import time
 
 import clickzetta
-import sqlparse
 import sqlalchemy
 import json
 import random
 import os
 import requests.exceptions
 import typing
 from typing import (
@@ -126,39 +125,14 @@
                 raise requests.exceptions.RequestException("user:" + login_params.username + "is Unauthorized")
             else:
                 token = result_dict['data']['token']
                 return token
         except requests.exceptions.RequestException:
             raise
 
-    def get_table_infos_from_show_statement(self, sql: string):
-        format_sql = sqlparse.format(sql, reindent=True, keyword_case='upper')
-        stmt = sqlparse.parse(format_sql)[0]
-        columns = []
-        types = []
-
-        for token in stmt.tokens:
-            if not isinstance(token, sqlparse.sql.Parenthesis):
-                continue
-            else:
-                for sub_token in token.tokens:
-                    if isinstance(sub_token, sqlparse.sql.Identifier) and not sub_token.value.startswith('NOVALID'):
-                        columns.append(sub_token.value.upper())
-                    elif isinstance(sub_token, sqlparse.sql.Token) and sub_token.ttype is not None and len(
-                            sub_token.ttype) == 2 and sub_token.ttype[
-                        1] == 'Builtin':
-                        types.append(sub_token.value.replace('\\', '').upper())
-                    elif isinstance(sub_token, sqlparse.sql.Function) and not sub_token.value.startswith(
-                            "UNIQUE") and not sub_token.value.startswith("KEY"):
-                        types.append(sub_token.value.replace('\\', '').upper())
-                    else:
-                        continue
-                break
-        return {'columns': columns, 'types': types}
-
     def create_bulkload_stream(self, schema_name: string, table_name: string,
                                options: BulkLoadOptions) -> BulkLoadMetaData:
         create_bulk_load_request = ingestion_pb2.CreateBulkLoadStreamRequest()
         account = ingestion_pb2.Account()
         user_ident = ingestion_pb2.UserIdentifier()
         user_ident.instance_id = self.instance_id
         user_ident.workspace = self.workspace
```

### Comparing `clickzetta-connector-0.7.3/clickzetta/dbapi/__init__.py` & `clickzetta-connector-0.7.4/clickzetta/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/dbapi/_helpers.py` & `clickzetta-connector-0.7.4/clickzetta/dbapi/_helpers.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/dbapi/connection.py` & `clickzetta-connector-0.7.4/clickzetta/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/dbapi/cursor.py` & `clickzetta-connector-0.7.4/clickzetta/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/dbapi/exceptions.py` & `clickzetta-connector-0.7.4/clickzetta/dbapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/dbapi/types.py` & `clickzetta-connector-0.7.4/clickzetta/dbapi/types.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/enums.py` & `clickzetta-connector-0.7.4/clickzetta/enums.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/account_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/account_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/block_bloom_filter_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/block_bloom_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/bucket_info_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/bucket_info_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/compression_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/compression_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/connection_meta_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/connection_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/data_type_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/data_type_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/expression_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/file_format_type_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/file_format_type_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/file_meta_data_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/file_meta_data_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/file_system_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/file_system_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/function_meta_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/function_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/hash_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/hash_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/ingestion_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/ingestion_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/ingestion_pb2_grpc.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/ingestion_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/input_split_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/input_split_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/job_meta_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/job_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/job_result_cache_meta_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/job_result_cache_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/kudu_common_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/kudu_common_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/metadata_entity_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/metadata_entity_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/network_policy_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/network_policy_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/object_identifier_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/object_identifier_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/operator_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/operator_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/pb_util_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/pb_util_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/property_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/property_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/rm_app_meta_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/rm_app_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/role_meta_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/role_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/row_operations_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/row_operations_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/schema_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/share_meta_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/share_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/statistics_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/table_common_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/table_common_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/table_meta_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/table_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_cluster_meta_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/virtual_cluster_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_cluster_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/virtual_cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_cluster_size_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/virtual_cluster_size_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_value_info_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/virtual_value_info_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/generated/workspace_meta_pb2.py` & `clickzetta-connector-0.7.4/clickzetta/proto/generated/workspace_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/account.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/account.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/block_bloom_filter.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/block_bloom_filter.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/compression.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/compression.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/data_type.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/data_type.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/expression.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/expression.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/file_meta_data.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/file_meta_data.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/function_meta.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/function_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/hash.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/hash.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/ingestion.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/ingestion.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/input_split.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/input_split.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/job_meta.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/job_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/kudu_common.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/kudu_common.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/metadata_entity.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/metadata_entity.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/object_identifier.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/object_identifier.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/operator.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/operator.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/pb_util.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/pb_util.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/rm_app_meta.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/rm_app_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/row_operations.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/row_operations.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/statistics.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/statistics.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/table_common.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/table_common.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/table_meta.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/table_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/virtual_cluster.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/virtual_cluster.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/virtual_cluster_meta.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/virtual_cluster_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/proto/source/virtual_value_info.proto` & `clickzetta-connector-0.7.4/clickzetta/proto/source/virtual_value_info.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/query_result.py` & `clickzetta-connector-0.7.4/clickzetta/query_result.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/schema.py` & `clickzetta-connector-0.7.4/clickzetta/schema.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/session.py` & `clickzetta-connector-0.7.4/clickzetta/session.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/standard_sql.py` & `clickzetta-connector-0.7.4/clickzetta/standard_sql.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta/table.py` & `clickzetta-connector-0.7.4/clickzetta/table.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta_connector.egg-info/SOURCES.txt` & `clickzetta-connector-0.7.4/clickzetta_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.3/clickzetta_connector.egg-info/requires.txt` & `clickzetta-connector-0.7.4/clickzetta_connector.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 proto-plus<2.0.0dev,>=1.22.0
 packaging<24.0.0dev,>=14.3
 protobuf!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0dev,>=3.19.5
 python-dateutil<3.0dev,>=2.7.2
 requests<3.0.0dev,>=2.21.0
-sqlparser>=0.0.9
 pyarrow>=11.0.0
 ossfs>=2023.1.0
 
 [all]
 pandas>=1.0.0
 db-dtypes<2.0.0dev,>=0.3.0
 ipywidgets==7.7.1
```

### Comparing `clickzetta-connector-0.7.3/setup.py` & `clickzetta-connector-0.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 release_status = "Development Status :: 3 - Alpha"
 dependencies = [
     "proto-plus >= 1.22.0, <2.0.0dev",
     "packaging >= 14.3, <24.0.0dev",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "python-dateutil >= 2.7.2, <3.0dev",
     "requests >= 2.21.0, < 3.0.0dev",
-    "sqlparser >= 0.0.9",
     "pyarrow >= 11.0.0",
     "ossfs >= 2023.1.0"
 ]
 extras = {
     "pandas": ["pandas>=1.0.0", "db-dtypes>=0.3.0,<2.0.0dev"],
     "ipywidgets": ["ipywidgets==7.7.1"],
     "geopandas": ["geopandas>=0.9.0, <1.0dev", "Shapely>=1.6.0, <2.0dev"],
@@ -78,11 +77,11 @@
     url='https://www.zettadecision.com/',
     author="mocun",
     author_email="hanmiao.li@clickzetta.com",
     platforms="Posix; MacOS X;",
     packages=packages,
     install_requires=dependencies,
     extras_require=extras,
-    python_requires=">=3.7, <3.11",
+    python_requires=">=3.7",
     include_package_data=True,
     zip_safe=False,
 )
```

