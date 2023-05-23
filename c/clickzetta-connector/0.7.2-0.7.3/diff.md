# Comparing `tmp/clickzetta-connector-0.7.2.tar.gz` & `tmp/clickzetta-connector-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickzetta-connector-0.7.2.tar", last modified: Fri May 19 07:27:34 2023, max compression
+gzip compressed data, was "clickzetta-connector-0.7.3.tar", last modified: Tue May 23 06:13:37 2023, max compression
```

## Comparing `clickzetta-connector-0.7.2.tar` & `clickzetta-connector-0.7.3.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-19 07:27:34.108563 clickzetta-connector-0.7.2/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       49 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.2/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)      421 2023-05-19 07:27:34.108410 clickzetta-connector-0.7.2/PKG-INFO
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-19 07:27:34.092517 clickzetta-connector-0.7.2/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      159 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.2/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     9899 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.2/clickzetta/_helpers.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-19 07:27:34.093281 clickzetta-connector-0.7.2/clickzetta/bulkload/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-03-20 02:30:34.000000 clickzetta-connector-0.7.2/clickzetta/bulkload/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7190 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.2/clickzetta/bulkload/bulkload_enums.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4387 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.2/clickzetta/bulkload/bulkload_stream.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    14842 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.2/clickzetta/bulkload/bulkload_writer.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      483 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.2/clickzetta/bulkload/cz_table.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    39500 2023-05-18 07:25:29.000000 clickzetta-connector-0.7.2/clickzetta/client.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-19 07:27:34.094530 clickzetta-connector-0.7.2/clickzetta/dbapi/
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1677 2022-11-05 16:51:08.000000 clickzetta-connector-0.7.2/clickzetta/dbapi/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1000 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.2/clickzetta/dbapi/_helpers.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2761 2022-12-13 11:25:14.000000 clickzetta-connector-0.7.2/clickzetta/dbapi/connection.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4595 2023-05-19 03:17:02.000000 clickzetta-connector-0.7.2/clickzetta/dbapi/cursor.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1100 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.2/clickzetta/dbapi/exceptions.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1131 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.2/clickzetta/dbapi/types.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7203 2023-03-13 07:16:08.000000 clickzetta-connector-0.7.2/clickzetta/enums.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-19 07:27:34.089720 clickzetta-connector-0.7.2/clickzetta/proto/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-19 07:27:34.103586 clickzetta-connector-0.7.2/clickzetta/proto/generated/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2488 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/account_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/account_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1623 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/block_bloom_filter_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/block_bloom_filter_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1078 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/bucket_info_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/bucket_info_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1233 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/compression_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/compression_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1739 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/connection_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/connection_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5567 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/data_type_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/data_type_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4689 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/expression_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/expression_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1251 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/file_format_type_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/file_format_type_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3623 2023-05-19 07:27:34.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/file_meta_data_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/file_meta_data_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1087 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/file_system_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/file_system_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2232 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/function_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/function_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1106 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/hash_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:34.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/hash_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    17705 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/ingestion_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    20165 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/ingestion_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6794 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/input_split_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/input_split_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5520 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/job_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/job_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1683 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/job_result_cache_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/job_result_cache_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    11392 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/kudu_common_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/kudu_common_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4271 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/metadata_entity_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/metadata_entity_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1300 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/network_policy_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/network_policy_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2847 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/object_identifier_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/object_identifier_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    35572 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/operator_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/operator_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1430 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/pb_util_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/pb_util_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1130 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/property_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/property_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1861 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/rm_app_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/rm_app_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1354 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/role_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/role_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2102 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/row_operations_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/row_operations_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      944 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/schema_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/schema_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1509 2023-05-19 07:27:34.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/share_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/share_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5493 2023-05-19 07:27:34.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/statistics_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:34.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/statistics_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    11527 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/table_common_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/table_common_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3834 2023-05-19 07:27:34.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/table_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/table_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4089 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/virtual_cluster_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/virtual_cluster_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6210 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/virtual_cluster_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/virtual_cluster_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1382 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/virtual_cluster_size_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/virtual_cluster_size_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1836 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/virtual_value_info_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/virtual_value_info_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1208 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/workspace_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-19 07:27:33.000000 clickzetta-connector-0.7.2/clickzetta/proto/generated/workspace_meta_pb2_grpc.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-19 07:27:34.107680 clickzetta-connector-0.7.2/clickzetta/proto/source/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      770 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/account.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1549 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/block_bloom_filter.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      190 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/bucket_info.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1017 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/compression.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      413 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/connection_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2033 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/data_type.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1697 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/expression.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      284 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/file_format_type.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1781 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/file_meta_data.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      121 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/file_system.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      643 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/function_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1007 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/hash.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7935 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/ingestion.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2908 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/input_split.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2134 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/job_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/job_result_cache_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)    18379 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/kudu_common.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1417 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/metadata_entity.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      311 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/network_policy.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1071 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/object_identifier.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)    16166 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/operator.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1805 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/pb_util.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      157 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/property.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      515 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/rm_app_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      232 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/role_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3795 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/row_operations.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)       81 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/schema.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      312 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/share_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2539 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/statistics.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4801 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/table_common.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1895 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/table_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2387 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/virtual_cluster.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1337 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/virtual_cluster_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      253 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/virtual_cluster_size.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1034 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/virtual_value_info.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      376 2023-03-20 02:30:48.000000 clickzetta-connector-0.7.2/clickzetta/proto/source/workspace_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     8617 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.2/clickzetta/query_result.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6368 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.2/clickzetta/schema.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3557 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.2/clickzetta/session.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4780 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.2/clickzetta/standard_sql.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2277 2022-11-09 13:50:16.000000 clickzetta-connector-0.7.2/clickzetta/table.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       21 2023-05-19 07:27:27.000000 clickzetta-connector-0.7.2/clickzetta/version.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-19 07:27:34.108239 clickzetta-connector-0.7.2/clickzetta_connector.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      421 2023-05-19 07:27:34.000000 clickzetta-connector-0.7.2/clickzetta_connector.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6027 2023-05-19 07:27:34.000000 clickzetta-connector-0.7.2/clickzetta_connector.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-19 07:27:34.000000 clickzetta-connector-0.7.2/clickzetta_connector.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-19 07:27:34.000000 clickzetta-connector-0.7.2/clickzetta_connector.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)      629 2023-05-19 07:27:34.000000 clickzetta-connector-0.7.2/clickzetta_connector.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       11 2023-05-19 07:27:34.000000 clickzetta-connector-0.7.2/clickzetta_connector.egg-info/top_level.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-19 07:27:34.108613 clickzetta-connector-0.7.2/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2888 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.2/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:13:37.472121 clickzetta-connector-0.7.3/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       49 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.3/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      421 2023-05-23 06:13:37.471982 clickzetta-connector-0.7.3/PKG-INFO
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:13:37.457841 clickzetta-connector-0.7.3/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      159 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.3/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     9899 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.3/clickzetta/_helpers.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:13:37.458526 clickzetta-connector-0.7.3/clickzetta/bulkload/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-03-20 02:30:34.000000 clickzetta-connector-0.7.3/clickzetta/bulkload/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7190 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.3/clickzetta/bulkload/bulkload_enums.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4387 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.3/clickzetta/bulkload/bulkload_stream.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    14842 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.3/clickzetta/bulkload/bulkload_writer.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      483 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.3/clickzetta/bulkload/cz_table.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    39500 2023-05-18 07:25:29.000000 clickzetta-connector-0.7.3/clickzetta/client.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:13:37.459673 clickzetta-connector-0.7.3/clickzetta/dbapi/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1677 2022-11-05 16:51:08.000000 clickzetta-connector-0.7.3/clickzetta/dbapi/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1000 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.3/clickzetta/dbapi/_helpers.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2761 2022-12-13 11:25:14.000000 clickzetta-connector-0.7.3/clickzetta/dbapi/connection.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4100 2023-05-19 07:53:05.000000 clickzetta-connector-0.7.3/clickzetta/dbapi/cursor.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1100 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.3/clickzetta/dbapi/exceptions.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1131 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.3/clickzetta/dbapi/types.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7203 2023-03-13 07:16:08.000000 clickzetta-connector-0.7.3/clickzetta/enums.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:13:37.454906 clickzetta-connector-0.7.3/clickzetta/proto/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:13:37.466945 clickzetta-connector-0.7.3/clickzetta/proto/generated/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2488 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/account_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/account_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1623 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/block_bloom_filter_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/block_bloom_filter_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1078 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/bucket_info_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/bucket_info_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1233 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/compression_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/compression_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1739 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/connection_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/connection_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5567 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/data_type_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/data_type_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4689 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/expression_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/expression_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1251 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/file_format_type_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/file_format_type_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3623 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/file_meta_data_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/file_meta_data_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1087 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/file_system_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/file_system_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2232 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/function_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/function_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1106 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/hash_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/hash_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    18361 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/ingestion_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    20165 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/ingestion_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6794 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/input_split_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/input_split_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5520 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/job_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/job_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1683 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/job_result_cache_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/job_result_cache_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    11392 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/kudu_common_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/kudu_common_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4271 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/metadata_entity_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/metadata_entity_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1300 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/network_policy_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/network_policy_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2847 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/object_identifier_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/object_identifier_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    35572 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/operator_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/operator_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1430 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/pb_util_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/pb_util_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1130 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/property_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/property_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1861 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/rm_app_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/rm_app_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1354 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/role_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/role_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2102 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/row_operations_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/row_operations_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      944 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/schema_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/schema_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1509 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/share_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/share_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5493 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/statistics_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/statistics_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    11527 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/table_common_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/table_common_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3834 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/table_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/table_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4089 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_cluster_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_cluster_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6210 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_cluster_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_cluster_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1382 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_cluster_size_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_cluster_size_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1836 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_value_info_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_value_info_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1208 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/workspace_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta/proto/generated/workspace_meta_pb2_grpc.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:13:37.470990 clickzetta-connector-0.7.3/clickzetta/proto/source/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      770 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/account.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1549 2023-03-16 07:43:26.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/block_bloom_filter.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      190 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/bucket_info.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1017 2023-03-16 07:44:39.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/compression.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      413 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/connection_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2033 2023-03-13 07:16:08.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/data_type.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1697 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/expression.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      284 2023-03-13 07:16:08.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/file_format_type.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1781 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/file_meta_data.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      121 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/file_system.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      643 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/function_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1007 2023-03-16 07:43:26.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/hash.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     8197 2023-05-23 06:09:29.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/ingestion.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2908 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/input_split.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2134 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/job_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/job_result_cache_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    18379 2022-08-20 14:59:08.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/kudu_common.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1417 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/metadata_entity.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      311 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/network_policy.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1071 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/object_identifier.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    16166 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/operator.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1805 2023-03-16 07:43:26.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/pb_util.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      157 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/property.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      515 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/rm_app_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      232 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/role_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3795 2023-03-16 07:43:26.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/row_operations.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       81 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/schema.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      312 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/share_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2539 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/statistics.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4801 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/table_common.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1895 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/table_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2387 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/virtual_cluster.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1337 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/virtual_cluster_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      253 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/virtual_cluster_size.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1034 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/virtual_value_info.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      376 2023-05-23 06:02:13.000000 clickzetta-connector-0.7.3/clickzetta/proto/source/workspace_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     8617 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.3/clickzetta/query_result.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6368 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.3/clickzetta/schema.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3557 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.3/clickzetta/session.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4780 2022-11-01 03:39:08.000000 clickzetta-connector-0.7.3/clickzetta/standard_sql.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2277 2022-11-09 13:50:16.000000 clickzetta-connector-0.7.3/clickzetta/table.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       21 2023-05-23 06:13:30.000000 clickzetta-connector-0.7.3/clickzetta/version.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-23 06:13:37.471813 clickzetta-connector-0.7.3/clickzetta_connector.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      421 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta_connector.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6027 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta_connector.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      629 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta_connector.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       11 2023-05-23 06:13:37.000000 clickzetta-connector-0.7.3/clickzetta_connector.egg-info/top_level.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-23 06:13:37.472166 clickzetta-connector-0.7.3/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2888 2023-05-16 07:24:44.000000 clickzetta-connector-0.7.3/setup.py
```

### Comparing `clickzetta-connector-0.7.2/clickzetta/_helpers.py` & `clickzetta-connector-0.7.3/clickzetta/_helpers.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/bulkload/bulkload_enums.py` & `clickzetta-connector-0.7.3/clickzetta/bulkload/bulkload_enums.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/bulkload/bulkload_stream.py` & `clickzetta-connector-0.7.3/clickzetta/bulkload/bulkload_stream.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/bulkload/bulkload_writer.py` & `clickzetta-connector-0.7.3/clickzetta/bulkload/bulkload_writer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/client.py` & `clickzetta-connector-0.7.3/clickzetta/client.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/dbapi/__init__.py` & `clickzetta-connector-0.7.3/clickzetta/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/dbapi/_helpers.py` & `clickzetta-connector-0.7.3/clickzetta/dbapi/_helpers.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/dbapi/connection.py` & `clickzetta-connector-0.7.3/clickzetta/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/dbapi/cursor.py` & `clickzetta-connector-0.7.3/clickzetta/dbapi/cursor.py`

 * *Files 10% similar despite different names*

```diff
@@ -113,24 +113,14 @@
             return self._query_data.fetch_many(size)
         except StopIteration:
             return None
 
     def fetchall(self):
         return self._query_data.fetch_all()
 
-    def fetchmany_with_schema(self, size=None) -> dict:
-        result_dict = {'schema': self.description, 'data': self._query_data.fetch_many(size),
-                       'total_row_count': self._query_result.total_row_count}
-        return result_dict
-
-    def fetchall_with_schema(self) -> dict:
-        result_dict = {'schema': self.description, 'data': self._query_data.fetch_all(),
-                       'total_row_count': self._query_result.total_row_count}
-        return result_dict
-
     def setinputsizes(self, sizes):
         """No-op, but for consistency raise an error if cursor is closed."""
 
     def setoutputsize(self, size, column=None):
         """No-op, but for consistency raise an error if cursor is closed."""
 
     def __iter__(self):
```

### Comparing `clickzetta-connector-0.7.2/clickzetta/dbapi/exceptions.py` & `clickzetta-connector-0.7.3/clickzetta/dbapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/dbapi/types.py` & `clickzetta-connector-0.7.3/clickzetta/dbapi/types.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/enums.py` & `clickzetta-connector-0.7.3/clickzetta/enums.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/account_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/account_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/block_bloom_filter_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/block_bloom_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/bucket_info_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/bucket_info_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/compression_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/compression_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/connection_meta_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/connection_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/data_type_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/data_type_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/expression_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/file_format_type_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/file_format_type_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/file_meta_data_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/file_meta_data_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/file_system_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/file_system_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/function_meta_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/function_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/hash_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/hash_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/ingestion_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/ingestion_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,35 +11,37 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import data_type_pb2 as data__type__pb2
 from . import file_format_type_pb2 as file__format__type__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fingestion.proto\x12\x12\x63z.proto.ingestion\x1a\x0f\x64\x61ta_type.proto\x1a\x16\x66ile_format_type.proto\"^\n\x0eGatewayRequest\x12\x17\n\x0fmethodEnumValue\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x12\n\ninstanceId\x18\x03 \x01(\x03\x12\x0e\n\x06userId\x18\x04 \x01(\x03\"]\n\x0fGatewayResponse\x12\x39\n\x06status\x18\x01 \x01(\x0b\x32).cz.proto.ingestion.GateWayResponseStatus\x12\x0f\n\x07message\x18\x02 \x01(\t\"\\\n\x0eUserIdentifier\x12\x13\n\x0binstance_id\x18\x01 \x01(\x03\x12\x11\n\tworkspace\x18\x02 \x01(\t\x12\x11\n\tuser_name\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\x03\"P\n\x07\x41\x63\x63ount\x12\x36\n\nuser_ident\x18\x01 \x01(\x0b\x32\".cz.proto.ingestion.UserIdentifier\x12\r\n\x05token\x18\x02 \x01(\t\"b\n\x0fTableIdentifier\x12\x13\n\x0binstance_id\x18\x01 \x01(\x03\x12\x11\n\tworkspace\x18\x02 \x01(\t\x12\x13\n\x0bschema_name\x18\x03 \x01(\t\x12\x12\n\ntable_name\x18\x04 \x01(\t\"d\n\x15GateWayResponseStatus\x12&\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x18.cz.proto.ingestion.Code\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x12\n\nrequest_id\x18\x03 \x01(\t\"c\n\x0eResponseStatus\x12&\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x18.cz.proto.ingestion.Code\x12\x15\n\rerror_message\x18\x02 \x01(\t\x12\x12\n\nrequest_id\x18\x03 \x01(\t\";\n\tDataField\x12\x0c\n\x04name\x18\x01 \x01(\t\x12 \n\x04type\x18\x02 \x01(\x0b\x32\x12.cz.proto.DataType\"R\n\x10\x44istributionSpec\x12\x11\n\tfield_ids\x18\x01 \x03(\r\x12\x16\n\x0ehash_functions\x18\x02 \x03(\t\x12\x13\n\x0bnum_buckets\x18\x03 \x01(\r\"#\n\x0ePrimaryKeySpec\x12\x11\n\tfield_ids\x18\x01 \x03(\r\"&\n\rPartitionSpec\x12\x15\n\rsrc_field_ids\x18\x01 \x03(\r\"\xf4\x01\n\x0cStreamSchema\x12\x32\n\x0b\x64\x61ta_fields\x18\x01 \x03(\x0b\x32\x1d.cz.proto.ingestion.DataField\x12\x37\n\tdist_spec\x18\x02 \x01(\x0b\x32$.cz.proto.ingestion.DistributionSpec\x12<\n\x10primary_key_spec\x18\x03 \x01(\x0b\x32\".cz.proto.ingestion.PrimaryKeySpec\x12\x39\n\x0epartition_spec\x18\x04 \x01(\x0b\x32!.cz.proto.ingestion.PartitionSpec\"\x97\x01\n\x18\x43reateOrGetStreamRequest\x12,\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x1b.cz.proto.ingestion.Account\x12\x38\n\x0btable_ident\x18\x02 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\x12\x13\n\x0bnum_tablets\x18\x03 \x01(\r\"\xd8\x01\n\x19\x43reateOrGetStreamResponse\x12\x38\n\x0btable_ident\x18\x01 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\x12\x35\n\x0b\x64\x61ta_schema\x18\x02 \x01(\x0b\x32 .cz.proto.ingestion.StreamSchema\x12\x16\n\x0e\x61lready_exists\x18\x03 \x01(\x08\x12\x32\n\x06status\x18\x04 \x01(\x0b\x32\".cz.proto.ingestion.ResponseStatus\"|\n\x12\x43loseStreamRequest\x12,\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x1b.cz.proto.ingestion.Account\x12\x38\n\x0btable_ident\x18\x02 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\"I\n\x13\x43loseStreamResponse\x12\x32\n\x06status\x18\x01 \x01(\x0b\x32\".cz.proto.ingestion.ResponseStatus\"\x94\x01\n\x12OssStagingPathInfo\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x11\n\tsts_ak_id\x18\x03 \x01(\t\x12\x15\n\rsts_ak_secret\x18\x04 \x01(\t\x12\x11\n\tsts_token\x18\x05 \x01(\t\x12\x14\n\x0coss_endpoint\x18\x06 \x01(\t\x12\x1d\n\x15oss_internal_endpoint\x18\x07 \x01(\t\"Z\n\x0fStagingPathInfo\x12:\n\x08oss_path\x18\x01 \x01(\x0b\x32&.cz.proto.ingestion.OssStagingPathInfoH\x00\x42\x0b\n\tpath_info\"\xf0\x02\n\x12\x42ulkLoadStreamInfo\x12\x11\n\tstream_id\x18\x01 \x01(\t\x12=\n\x0cstream_state\x18\x02 \x01(\x0e\x32\'.cz.proto.ingestion.BulkLoadStreamState\x12\x12\n\nsql_job_id\x18\x03 \x01(\t\x12\x37\n\nidentifier\x18\x04 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\x12>\n\toperation\x18\x05 \x01(\x0e\x32+.cz.proto.ingestion.BulkLoadStreamOperation\x12\x16\n\x0epartition_spec\x18\x06 \x01(\t\x12\x13\n\x0brecord_keys\x18\x07 \x03(\t\x12\x37\n\rstream_schema\x18\x08 \x01(\x0b\x32 .cz.proto.ingestion.StreamSchema\x12\x15\n\rsql_error_msg\x18\t \x01(\t\"\xc9\x01\n\x1a\x42ulkLoadStreamWriterConfig\x12\x39\n\x0cstaging_path\x18\x01 \x01(\x0b\x32#.cz.proto.ingestion.StagingPathInfo\x12-\n\x0b\x66ile_format\x18\x02 \x01(\x0e\x32\x18.cz.proto.FileFormatType\x12\x1d\n\x15max_num_rows_per_file\x18\x03 \x01(\x03\x12\"\n\x1amax_size_in_bytes_per_file\x18\x04 \x01(\x03\"\xf1\x01\n\x1b\x43reateBulkLoadStreamRequest\x12,\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x1b.cz.proto.ingestion.Account\x12\x37\n\nidentifier\x18\x02 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\x12>\n\toperation\x18\x03 \x01(\x0e\x32+.cz.proto.ingestion.BulkLoadStreamOperation\x12\x16\n\x0epartition_spec\x18\x04 \x01(\t\x12\x13\n\x0brecord_keys\x18\x05 \x03(\t\"\x88\x01\n\x1c\x43reateBulkLoadStreamResponse\x12\x32\n\x06status\x18\x01 \x01(\x0b\x32\".cz.proto.ingestion.ResponseStatus\x12\x34\n\x04info\x18\x02 \x01(\x0b\x32&.cz.proto.ingestion.BulkLoadStreamInfo\"\xad\x01\n\x18GetBulkLoadStreamRequest\x12,\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x1b.cz.proto.ingestion.Account\x12\x37\n\nidentifier\x18\x02 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\x12\x11\n\tstream_id\x18\x03 \x01(\t\x12\x17\n\x0fneed_table_meta\x18\x04 \x01(\x08\"\x85\x01\n\x19GetBulkLoadStreamResponse\x12\x32\n\x06status\x18\x01 \x01(\x0b\x32\".cz.proto.ingestion.ResponseStatus\x12\x34\n\x04info\x18\x02 \x01(\x0b\x32&.cz.proto.ingestion.BulkLoadStreamInfo\"\xeb\x02\n\x1b\x43ommitBulkLoadStreamRequest\x12,\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x1b.cz.proto.ingestion.Account\x12\x37\n\nidentifier\x18\x02 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\x12\x11\n\tstream_id\x18\x03 \x01(\t\x12\x19\n\x11\x65xecute_workspace\x18\x04 \x01(\t\x12\x17\n\x0f\x65xecute_vc_name\x18\x05 \x01(\t\x12O\n\x0b\x63ommit_mode\x18\x06 \x01(\x0e\x32:.cz.proto.ingestion.CommitBulkLoadStreamRequest.CommitMode\x12\x1a\n\x12spec_partition_ids\x18\x07 \x03(\r\"1\n\nCommitMode\x12\x11\n\rCOMMIT_STREAM\x10\x00\x12\x10\n\x0c\x41\x42ORT_STREAM\x10\x01\"\x88\x01\n\x1c\x43ommitBulkLoadStreamResponse\x12\x32\n\x06status\x18\x01 \x01(\x0b\x32\".cz.proto.ingestion.ResponseStatus\x12\x34\n\x04info\x18\x02 \x01(\x0b\x32&.cz.proto.ingestion.BulkLoadStreamInfo\"\xb1\x01\n\x1fOpenBulkLoadStreamWriterRequest\x12,\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x1b.cz.proto.ingestion.Account\x12\x37\n\nidentifier\x18\x02 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\x12\x11\n\tstream_id\x18\x03 \x01(\t\x12\x14\n\x0cpartition_id\x18\x04 \x01(\r\"\x96\x01\n OpenBulkLoadStreamWriterResponse\x12\x32\n\x06status\x18\x01 \x01(\x0b\x32\".cz.proto.ingestion.ResponseStatus\x12>\n\x06\x63onfig\x18\x02 \x01(\x0b\x32..cz.proto.ingestion.BulkLoadStreamWriterConfig\"\xe3\x01\n!FinishBulkLoadStreamWriterRequest\x12,\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x1b.cz.proto.ingestion.Account\x12\x37\n\nidentifier\x18\x02 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\x12\x11\n\tstream_id\x18\x03 \x01(\t\x12\x14\n\x0cpartition_id\x18\x04 \x01(\r\x12\x15\n\rwritten_files\x18\x05 \x03(\t\x12\x17\n\x0fwritten_lengths\x18\x06 \x03(\x04\"X\n\"FinishBulkLoadStreamWriterResponse\x12\x32\n\x06status\x18\x01 \x01(\x0b\x32\".cz.proto.ingestion.ResponseStatus\"\x9c\x01\n\x16GetRouteWorkersRequest\x12\x38\n\x0btable_ident\x18\x01 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\x12\x35\n\x0c\x63onnect_mode\x18\x02 \x01(\x0e\x32\x1f.cz.proto.ingestion.ConnectMode\x12\x11\n\ttablet_id\x18\x03 \x03(\x03\"+\n\rHostPortTuple\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"\x92\x01\n\x17GetRouteWorkersResponse\x12\x30\n\x05tuple\x18\x01 \x03(\x0b\x32!.cz.proto.ingestion.HostPortTuple\x12\x11\n\ttablet_id\x18\x02 \x03(\x03\x12\x32\n\x06status\x18\x03 \x01(\x0b\x32\".cz.proto.ingestion.ResponseStatus\"H\n\x11OperationTypeList\x12\x33\n\x08op_types\x18\x01 \x03(\x0e\x32!.cz.proto.ingestion.OperationType\"\xf6\x01\n\tDataBlock\x12\x15\n\rarrow_payload\x18\x01 \x01(\x0c\x12\x1e\n\x16is_set_bitmaps_payload\x18\x02 \x01(\x0c\x12\x41\n\x10row_op_type_list\x18\x03 \x01(\x0b\x32%.cz.proto.ingestion.OperationTypeListH\x00\x12:\n\rblock_op_type\x18\x04 \x01(\x0e\x32!.cz.proto.ingestion.OperationTypeH\x00\x12\x11\n\tbucket_id\x18\x05 \x01(\r\x12\x10\n\x08num_rows\x18\x06 \x01(\rB\x0e\n\x0cop_type_info\"c\n\x0fMutateRowStatus\x12&\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x18.cz.proto.ingestion.Code\x12\x15\n\rerror_message\x18\x02 \x01(\t\x12\x11\n\trow_index\x18\x03 \x01(\x05\"\xd6\x01\n\rMutateRequest\x12,\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x1b.cz.proto.ingestion.Account\x12\x38\n\x0btable_ident\x18\x02 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\x12\x10\n\x08\x62\x61tch_id\x18\x03 \x01(\x03\x12\x17\n\x0fwrite_timestamp\x18\x04 \x01(\x03\x12\x32\n\x0b\x64\x61ta_blocks\x18\x05 \x03(\x0b\x32\x1d.cz.proto.ingestion.DataBlock\"\xa6\x01\n\x0eMutateResponse\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\x03\x12\x10\n\x08num_rows\x18\x02 \x01(\x03\x12\x32\n\x06status\x18\x03 \x01(\x0b\x32\".cz.proto.ingestion.ResponseStatus\x12<\n\x0frow_status_list\x18\x04 \x03(\x0b\x32#.cz.proto.ingestion.MutateRowStatus*\x91\x05\n\nMethodEnum\x12\x14\n\x10GATEWAY_RPC_CALL\x10\x00\x12\x12\n\x0eGET_TABLE_META\x10\x01\x12\x11\n\rCREATE_TABLET\x10\x02\x12\x15\n\x11GET_MUTATE_WORKER\x10\x03\x12\x11\n\rCOMMIT_TABLET\x10\x04\x12\x0f\n\x0b\x44ROP_TABLET\x10\x05\x12\x16\n\x12\x43HECK_TABLE_EXISTS\x10\x06\x12\x19\n\x15\x43REATE_PENDING_STREAM\x10\x07\x12\x19\n\x15\x43OMMIT_PENDING_STREAM\x10\x08\x12\x16\n\x12GET_PENDING_STREAM\x10\t\x12\x17\n\x13JOIN_PENDING_STREAM\x10\n\x12\x1b\n\x17\x43REATE_BULK_LOAD_STREAM\x10\x0b\x12\x18\n\x14GET_BULK_LOAD_STREAM\x10\x0c\x12\x1b\n\x17\x43OMMIT_BULK_LOAD_STREAM\x10\r\x12 \n\x1cOPEN_BULK_LOAD_STREAM_WRITER\x10\x0e\x12\"\n\x1e\x46INISH_BULK_LOAD_STREAM_WRITER\x10\x0f\x12\x1b\n\x17\x43REATE_OR_GET_STREAM_V2\x10\x10\x12\x13\n\x0f\x43LOSE_STREAM_V2\x10\x11\x12\x17\n\x13GET_ROUTE_WORKER_V2\x10\x12\x12\x1e\n\x1a\x43REATE_BULK_LOAD_STREAM_V2\x10\x13\x12\x1b\n\x17GET_BULK_LOAD_STREAM_V2\x10\x14\x12\x1e\n\x1a\x43OMMIT_BULK_LOAD_STREAM_V2\x10\x15\x12#\n\x1fOPEN_BULK_LOAD_STREAM_WRITER_V2\x10\x16\x12%\n!FINISH_BULK_LOAD_STREAM_WRITER_V2\x10\x17*1\n\x0cIGSTableType\x12\n\n\x06NORMAL\x10\x00\x12\x0b\n\x07\x43LUSTER\x10\x01\x12\x08\n\x04\x41\x43ID\x10\x02*.\n\x04\x43ode\x12\x0b\n\x07SUCCESS\x10\x00\x12\n\n\x06\x46\x41ILED\x10\x01\x12\r\n\tTHROTTLED\x10\x02*\x8c\x01\n\x13\x42ulkLoadStreamState\x12\x0e\n\nBL_CREATED\x10\x00\x12\r\n\tBL_SEALED\x10\x01\x12\x17\n\x13\x42L_COMMIT_SUBMITTED\x10\x02\x12\x15\n\x11\x42L_COMMIT_SUCCESS\x10\x03\x12\x14\n\x10\x42L_COMMIT_FAILED\x10\x04\x12\x10\n\x0c\x42L_CANCELLED\x10\x05*I\n\x17\x42ulkLoadStreamOperation\x12\r\n\tBL_APPEND\x10\x00\x12\x10\n\x0c\x42L_OVERWRITE\x10\x01\x12\r\n\tBL_UPSERT\x10\x02*<\n\x0b\x43onnectMode\x12\n\n\x06\x44IRECT\x10\x00\x12\x0b\n\x07GATEWAY\x10\x01\x12\x14\n\x10GATEWAY_INTERNAL\x10\x02*\x85\x01\n\rOperationType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06INSERT\x10\x01\x12\n\n\x06UPDATE\x10\x02\x12\n\n\x06\x44\x45LETE\x10\x03\x12\n\n\x06UPSERT\x10\x04\x12\x11\n\rINSERT_IGNORE\x10\x05\x12\x11\n\rUPDATE_IGNORE\x10\x06\x12\x11\n\rDELETE_IGNORE\x10\x07\x32\xb3\x08\n\x1aIngestionControllerService\x12Y\n\x0eGatewayRpcCall\x12\".cz.proto.ingestion.GatewayRequest\x1a#.cz.proto.ingestion.GatewayResponse\x12p\n\x11\x43reateOrGetStream\x12,.cz.proto.ingestion.CreateOrGetStreamRequest\x1a-.cz.proto.ingestion.CreateOrGetStreamResponse\x12^\n\x0b\x43loseStream\x12&.cz.proto.ingestion.CloseStreamRequest\x1a\'.cz.proto.ingestion.CloseStreamResponse\x12j\n\x0fGetRouteWorkers\x12*.cz.proto.ingestion.GetRouteWorkersRequest\x1a+.cz.proto.ingestion.GetRouteWorkersResponse\x12y\n\x14\x43reateBulkLoadStream\x12/.cz.proto.ingestion.CreateBulkLoadStreamRequest\x1a\x30.cz.proto.ingestion.CreateBulkLoadStreamResponse\x12p\n\x11GetBulkLoadStream\x12,.cz.proto.ingestion.GetBulkLoadStreamRequest\x1a-.cz.proto.ingestion.GetBulkLoadStreamResponse\x12y\n\x14\x43ommitBulkLoadStream\x12/.cz.proto.ingestion.CommitBulkLoadStreamRequest\x1a\x30.cz.proto.ingestion.CommitBulkLoadStreamResponse\x12\x85\x01\n\x18OpenBulkLoadStreamWriter\x12\x33.cz.proto.ingestion.OpenBulkLoadStreamWriterRequest\x1a\x34.cz.proto.ingestion.OpenBulkLoadStreamWriterResponse\x12\x8b\x01\n\x1a\x46inishBulkLoadStreamWriter\x12\x35.cz.proto.ingestion.FinishBulkLoadStreamWriterRequest\x1a\x36.cz.proto.ingestion.FinishBulkLoadStreamWriterResponse2\xca\x01\n\x16IngestionWorkerService\x12S\n\x06Mutate\x12!.cz.proto.ingestion.MutateRequest\x1a\".cz.proto.ingestion.MutateResponse(\x01\x30\x01\x12[\n\x0eMutateInternal\x12!.cz.proto.ingestion.MutateRequest\x1a\".cz.proto.ingestion.MutateResponse(\x01\x30\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fingestion.proto\x12\x12\x63z.proto.ingestion\x1a\x0f\x64\x61ta_type.proto\x1a\x16\x66ile_format_type.proto\"^\n\x0eGatewayRequest\x12\x17\n\x0fmethodEnumValue\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x12\n\ninstanceId\x18\x03 \x01(\x03\x12\x0e\n\x06userId\x18\x04 \x01(\x03\"]\n\x0fGatewayResponse\x12\x39\n\x06status\x18\x01 \x01(\x0b\x32).cz.proto.ingestion.GateWayResponseStatus\x12\x0f\n\x07message\x18\x02 \x01(\t\"\\\n\x0eUserIdentifier\x12\x13\n\x0binstance_id\x18\x01 \x01(\x03\x12\x11\n\tworkspace\x18\x02 \x01(\t\x12\x11\n\tuser_name\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\x03\"P\n\x07\x41\x63\x63ount\x12\x36\n\nuser_ident\x18\x01 \x01(\x0b\x32\".cz.proto.ingestion.UserIdentifier\x12\r\n\x05token\x18\x02 \x01(\t\"b\n\x0fTableIdentifier\x12\x13\n\x0binstance_id\x18\x01 \x01(\x03\x12\x11\n\tworkspace\x18\x02 \x01(\t\x12\x13\n\x0bschema_name\x18\x03 \x01(\t\x12\x12\n\ntable_name\x18\x04 \x01(\t\"d\n\x15GateWayResponseStatus\x12&\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x18.cz.proto.ingestion.Code\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x12\n\nrequest_id\x18\x03 \x01(\t\"c\n\x0eResponseStatus\x12&\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x18.cz.proto.ingestion.Code\x12\x15\n\rerror_message\x18\x02 \x01(\t\x12\x12\n\nrequest_id\x18\x03 \x01(\t\";\n\tDataField\x12\x0c\n\x04name\x18\x01 \x01(\t\x12 \n\x04type\x18\x02 \x01(\x0b\x32\x12.cz.proto.DataType\"R\n\x10\x44istributionSpec\x12\x11\n\tfield_ids\x18\x01 \x03(\r\x12\x16\n\x0ehash_functions\x18\x02 \x03(\t\x12\x13\n\x0bnum_buckets\x18\x03 \x01(\r\"#\n\x0ePrimaryKeySpec\x12\x11\n\tfield_ids\x18\x01 \x03(\r\"&\n\rPartitionSpec\x12\x15\n\rsrc_field_ids\x18\x01 \x03(\r\"\xf4\x01\n\x0cStreamSchema\x12\x32\n\x0b\x64\x61ta_fields\x18\x01 \x03(\x0b\x32\x1d.cz.proto.ingestion.DataField\x12\x37\n\tdist_spec\x18\x02 \x01(\x0b\x32$.cz.proto.ingestion.DistributionSpec\x12<\n\x10primary_key_spec\x18\x03 \x01(\x0b\x32\".cz.proto.ingestion.PrimaryKeySpec\x12\x39\n\x0epartition_spec\x18\x04 \x01(\x0b\x32!.cz.proto.ingestion.PartitionSpec\"\x97\x01\n\x18\x43reateOrGetStreamRequest\x12,\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x1b.cz.proto.ingestion.Account\x12\x38\n\x0btable_ident\x18\x02 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\x12\x13\n\x0bnum_tablets\x18\x03 \x01(\r\"\xd8\x01\n\x19\x43reateOrGetStreamResponse\x12\x38\n\x0btable_ident\x18\x01 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\x12\x35\n\x0b\x64\x61ta_schema\x18\x02 \x01(\x0b\x32 .cz.proto.ingestion.StreamSchema\x12\x16\n\x0e\x61lready_exists\x18\x03 \x01(\x08\x12\x32\n\x06status\x18\x04 \x01(\x0b\x32\".cz.proto.ingestion.ResponseStatus\"|\n\x12\x43loseStreamRequest\x12,\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x1b.cz.proto.ingestion.Account\x12\x38\n\x0btable_ident\x18\x02 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\"I\n\x13\x43loseStreamResponse\x12\x32\n\x06status\x18\x01 \x01(\x0b\x32\".cz.proto.ingestion.ResponseStatus\"\xad\x01\n\x12OssStagingPathInfo\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x11\n\tsts_ak_id\x18\x03 \x01(\t\x12\x15\n\rsts_ak_secret\x18\x04 \x01(\t\x12\x11\n\tsts_token\x18\x05 \x01(\t\x12\x14\n\x0coss_endpoint\x18\x06 \x01(\t\x12\x1d\n\x15oss_internal_endpoint\x18\x07 \x01(\t\x12\x17\n\x0foss_expire_time\x18\x08 \x01(\x04\"Z\n\x0fStagingPathInfo\x12:\n\x08oss_path\x18\x01 \x01(\x0b\x32&.cz.proto.ingestion.OssStagingPathInfoH\x00\x42\x0b\n\tpath_info\"\xa7\x04\n\x12\x42ulkLoadStreamInfo\x12\x11\n\tstream_id\x18\x01 \x01(\t\x12=\n\x0cstream_state\x18\x02 \x01(\x0e\x32\'.cz.proto.ingestion.BulkLoadStreamState\x12\x12\n\nsql_job_id\x18\x03 \x01(\t\x12\x37\n\nidentifier\x18\x04 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\x12>\n\toperation\x18\x05 \x01(\x0e\x32+.cz.proto.ingestion.BulkLoadStreamOperation\x12\x16\n\x0epartition_spec\x18\x06 \x01(\t\x12\x13\n\x0brecord_keys\x18\x07 \x03(\t\x12\x37\n\rstream_schema\x18\x08 \x01(\x0b\x32 .cz.proto.ingestion.StreamSchema\x12\x15\n\rsql_error_msg\x18\t \x01(\t\x12 \n\x18prefer_internal_endpoint\x18\n \x01(\x08\x12Y\n\x12\x65ncryption_options\x18\x0b \x03(\x0b\x32=.cz.proto.ingestion.BulkLoadStreamInfo.EncryptionOptionsEntry\x1a\x38\n\x16\x45ncryptionOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xc9\x01\n\x1a\x42ulkLoadStreamWriterConfig\x12\x39\n\x0cstaging_path\x18\x01 \x01(\x0b\x32#.cz.proto.ingestion.StagingPathInfo\x12-\n\x0b\x66ile_format\x18\x02 \x01(\x0e\x32\x18.cz.proto.FileFormatType\x12\x1d\n\x15max_num_rows_per_file\x18\x03 \x01(\x03\x12\"\n\x1amax_size_in_bytes_per_file\x18\x04 \x01(\x03\"\x93\x02\n\x1b\x43reateBulkLoadStreamRequest\x12,\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x1b.cz.proto.ingestion.Account\x12\x37\n\nidentifier\x18\x02 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\x12>\n\toperation\x18\x03 \x01(\x0e\x32+.cz.proto.ingestion.BulkLoadStreamOperation\x12\x16\n\x0epartition_spec\x18\x04 \x01(\t\x12\x13\n\x0brecord_keys\x18\x05 \x03(\t\x12 \n\x18prefer_internal_endpoint\x18\x06 \x01(\x08\"\x88\x01\n\x1c\x43reateBulkLoadStreamResponse\x12\x32\n\x06status\x18\x01 \x01(\x0b\x32\".cz.proto.ingestion.ResponseStatus\x12\x34\n\x04info\x18\x02 \x01(\x0b\x32&.cz.proto.ingestion.BulkLoadStreamInfo\"\xad\x01\n\x18GetBulkLoadStreamRequest\x12,\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x1b.cz.proto.ingestion.Account\x12\x37\n\nidentifier\x18\x02 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\x12\x11\n\tstream_id\x18\x03 \x01(\t\x12\x17\n\x0fneed_table_meta\x18\x04 \x01(\x08\"\x85\x01\n\x19GetBulkLoadStreamResponse\x12\x32\n\x06status\x18\x01 \x01(\x0b\x32\".cz.proto.ingestion.ResponseStatus\x12\x34\n\x04info\x18\x02 \x01(\x0b\x32&.cz.proto.ingestion.BulkLoadStreamInfo\"\xeb\x02\n\x1b\x43ommitBulkLoadStreamRequest\x12,\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x1b.cz.proto.ingestion.Account\x12\x37\n\nidentifier\x18\x02 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\x12\x11\n\tstream_id\x18\x03 \x01(\t\x12\x19\n\x11\x65xecute_workspace\x18\x04 \x01(\t\x12\x17\n\x0f\x65xecute_vc_name\x18\x05 \x01(\t\x12O\n\x0b\x63ommit_mode\x18\x06 \x01(\x0e\x32:.cz.proto.ingestion.CommitBulkLoadStreamRequest.CommitMode\x12\x1a\n\x12spec_partition_ids\x18\x07 \x03(\r\"1\n\nCommitMode\x12\x11\n\rCOMMIT_STREAM\x10\x00\x12\x10\n\x0c\x41\x42ORT_STREAM\x10\x01\"\x88\x01\n\x1c\x43ommitBulkLoadStreamResponse\x12\x32\n\x06status\x18\x01 \x01(\x0b\x32\".cz.proto.ingestion.ResponseStatus\x12\x34\n\x04info\x18\x02 \x01(\x0b\x32&.cz.proto.ingestion.BulkLoadStreamInfo\"\xb1\x01\n\x1fOpenBulkLoadStreamWriterRequest\x12,\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x1b.cz.proto.ingestion.Account\x12\x37\n\nidentifier\x18\x02 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\x12\x11\n\tstream_id\x18\x03 \x01(\t\x12\x14\n\x0cpartition_id\x18\x04 \x01(\r\"\x96\x01\n OpenBulkLoadStreamWriterResponse\x12\x32\n\x06status\x18\x01 \x01(\x0b\x32\".cz.proto.ingestion.ResponseStatus\x12>\n\x06\x63onfig\x18\x02 \x01(\x0b\x32..cz.proto.ingestion.BulkLoadStreamWriterConfig\"\xe3\x01\n!FinishBulkLoadStreamWriterRequest\x12,\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x1b.cz.proto.ingestion.Account\x12\x37\n\nidentifier\x18\x02 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\x12\x11\n\tstream_id\x18\x03 \x01(\t\x12\x14\n\x0cpartition_id\x18\x04 \x01(\r\x12\x15\n\rwritten_files\x18\x05 \x03(\t\x12\x17\n\x0fwritten_lengths\x18\x06 \x03(\x04\"X\n\"FinishBulkLoadStreamWriterResponse\x12\x32\n\x06status\x18\x01 \x01(\x0b\x32\".cz.proto.ingestion.ResponseStatus\"\x9c\x01\n\x16GetRouteWorkersRequest\x12\x38\n\x0btable_ident\x18\x01 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\x12\x35\n\x0c\x63onnect_mode\x18\x02 \x01(\x0e\x32\x1f.cz.proto.ingestion.ConnectMode\x12\x11\n\ttablet_id\x18\x03 \x03(\x03\"+\n\rHostPortTuple\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"\x92\x01\n\x17GetRouteWorkersResponse\x12\x30\n\x05tuple\x18\x01 \x03(\x0b\x32!.cz.proto.ingestion.HostPortTuple\x12\x11\n\ttablet_id\x18\x02 \x03(\x03\x12\x32\n\x06status\x18\x03 \x01(\x0b\x32\".cz.proto.ingestion.ResponseStatus\"H\n\x11OperationTypeList\x12\x33\n\x08op_types\x18\x01 \x03(\x0e\x32!.cz.proto.ingestion.OperationType\"\xf6\x01\n\tDataBlock\x12\x15\n\rarrow_payload\x18\x01 \x01(\x0c\x12\x1e\n\x16is_set_bitmaps_payload\x18\x02 \x01(\x0c\x12\x41\n\x10row_op_type_list\x18\x03 \x01(\x0b\x32%.cz.proto.ingestion.OperationTypeListH\x00\x12:\n\rblock_op_type\x18\x04 \x01(\x0e\x32!.cz.proto.ingestion.OperationTypeH\x00\x12\x11\n\tbucket_id\x18\x05 \x01(\r\x12\x10\n\x08num_rows\x18\x06 \x01(\rB\x0e\n\x0cop_type_info\"c\n\x0fMutateRowStatus\x12&\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x18.cz.proto.ingestion.Code\x12\x15\n\rerror_message\x18\x02 \x01(\t\x12\x11\n\trow_index\x18\x03 \x01(\x05\"\xd6\x01\n\rMutateRequest\x12,\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x1b.cz.proto.ingestion.Account\x12\x38\n\x0btable_ident\x18\x02 \x01(\x0b\x32#.cz.proto.ingestion.TableIdentifier\x12\x10\n\x08\x62\x61tch_id\x18\x03 \x01(\x03\x12\x17\n\x0fwrite_timestamp\x18\x04 \x01(\x03\x12\x32\n\x0b\x64\x61ta_blocks\x18\x05 \x03(\x0b\x32\x1d.cz.proto.ingestion.DataBlock\"\xa6\x01\n\x0eMutateResponse\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\x03\x12\x10\n\x08num_rows\x18\x02 \x01(\x03\x12\x32\n\x06status\x18\x03 \x01(\x0b\x32\".cz.proto.ingestion.ResponseStatus\x12<\n\x0frow_status_list\x18\x04 \x03(\x0b\x32#.cz.proto.ingestion.MutateRowStatus*\x91\x05\n\nMethodEnum\x12\x14\n\x10GATEWAY_RPC_CALL\x10\x00\x12\x12\n\x0eGET_TABLE_META\x10\x01\x12\x11\n\rCREATE_TABLET\x10\x02\x12\x15\n\x11GET_MUTATE_WORKER\x10\x03\x12\x11\n\rCOMMIT_TABLET\x10\x04\x12\x0f\n\x0b\x44ROP_TABLET\x10\x05\x12\x16\n\x12\x43HECK_TABLE_EXISTS\x10\x06\x12\x19\n\x15\x43REATE_PENDING_STREAM\x10\x07\x12\x19\n\x15\x43OMMIT_PENDING_STREAM\x10\x08\x12\x16\n\x12GET_PENDING_STREAM\x10\t\x12\x17\n\x13JOIN_PENDING_STREAM\x10\n\x12\x1b\n\x17\x43REATE_BULK_LOAD_STREAM\x10\x0b\x12\x18\n\x14GET_BULK_LOAD_STREAM\x10\x0c\x12\x1b\n\x17\x43OMMIT_BULK_LOAD_STREAM\x10\r\x12 \n\x1cOPEN_BULK_LOAD_STREAM_WRITER\x10\x0e\x12\"\n\x1e\x46INISH_BULK_LOAD_STREAM_WRITER\x10\x0f\x12\x1b\n\x17\x43REATE_OR_GET_STREAM_V2\x10\x10\x12\x13\n\x0f\x43LOSE_STREAM_V2\x10\x11\x12\x17\n\x13GET_ROUTE_WORKER_V2\x10\x12\x12\x1e\n\x1a\x43REATE_BULK_LOAD_STREAM_V2\x10\x13\x12\x1b\n\x17GET_BULK_LOAD_STREAM_V2\x10\x14\x12\x1e\n\x1a\x43OMMIT_BULK_LOAD_STREAM_V2\x10\x15\x12#\n\x1fOPEN_BULK_LOAD_STREAM_WRITER_V2\x10\x16\x12%\n!FINISH_BULK_LOAD_STREAM_WRITER_V2\x10\x17*1\n\x0cIGSTableType\x12\n\n\x06NORMAL\x10\x00\x12\x0b\n\x07\x43LUSTER\x10\x01\x12\x08\n\x04\x41\x43ID\x10\x02*.\n\x04\x43ode\x12\x0b\n\x07SUCCESS\x10\x00\x12\n\n\x06\x46\x41ILED\x10\x01\x12\r\n\tTHROTTLED\x10\x02*\x8c\x01\n\x13\x42ulkLoadStreamState\x12\x0e\n\nBL_CREATED\x10\x00\x12\r\n\tBL_SEALED\x10\x01\x12\x17\n\x13\x42L_COMMIT_SUBMITTED\x10\x02\x12\x15\n\x11\x42L_COMMIT_SUCCESS\x10\x03\x12\x14\n\x10\x42L_COMMIT_FAILED\x10\x04\x12\x10\n\x0c\x42L_CANCELLED\x10\x05*I\n\x17\x42ulkLoadStreamOperation\x12\r\n\tBL_APPEND\x10\x00\x12\x10\n\x0c\x42L_OVERWRITE\x10\x01\x12\r\n\tBL_UPSERT\x10\x02*<\n\x0b\x43onnectMode\x12\n\n\x06\x44IRECT\x10\x00\x12\x0b\n\x07GATEWAY\x10\x01\x12\x14\n\x10GATEWAY_INTERNAL\x10\x02*\x85\x01\n\rOperationType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06INSERT\x10\x01\x12\n\n\x06UPDATE\x10\x02\x12\n\n\x06\x44\x45LETE\x10\x03\x12\n\n\x06UPSERT\x10\x04\x12\x11\n\rINSERT_IGNORE\x10\x05\x12\x11\n\rUPDATE_IGNORE\x10\x06\x12\x11\n\rDELETE_IGNORE\x10\x07\x32\xb3\x08\n\x1aIngestionControllerService\x12Y\n\x0eGatewayRpcCall\x12\".cz.proto.ingestion.GatewayRequest\x1a#.cz.proto.ingestion.GatewayResponse\x12p\n\x11\x43reateOrGetStream\x12,.cz.proto.ingestion.CreateOrGetStreamRequest\x1a-.cz.proto.ingestion.CreateOrGetStreamResponse\x12^\n\x0b\x43loseStream\x12&.cz.proto.ingestion.CloseStreamRequest\x1a\'.cz.proto.ingestion.CloseStreamResponse\x12j\n\x0fGetRouteWorkers\x12*.cz.proto.ingestion.GetRouteWorkersRequest\x1a+.cz.proto.ingestion.GetRouteWorkersResponse\x12y\n\x14\x43reateBulkLoadStream\x12/.cz.proto.ingestion.CreateBulkLoadStreamRequest\x1a\x30.cz.proto.ingestion.CreateBulkLoadStreamResponse\x12p\n\x11GetBulkLoadStream\x12,.cz.proto.ingestion.GetBulkLoadStreamRequest\x1a-.cz.proto.ingestion.GetBulkLoadStreamResponse\x12y\n\x14\x43ommitBulkLoadStream\x12/.cz.proto.ingestion.CommitBulkLoadStreamRequest\x1a\x30.cz.proto.ingestion.CommitBulkLoadStreamResponse\x12\x85\x01\n\x18OpenBulkLoadStreamWriter\x12\x33.cz.proto.ingestion.OpenBulkLoadStreamWriterRequest\x1a\x34.cz.proto.ingestion.OpenBulkLoadStreamWriterResponse\x12\x8b\x01\n\x1a\x46inishBulkLoadStreamWriter\x12\x35.cz.proto.ingestion.FinishBulkLoadStreamWriterRequest\x1a\x36.cz.proto.ingestion.FinishBulkLoadStreamWriterResponse2\xca\x01\n\x16IngestionWorkerService\x12S\n\x06Mutate\x12!.cz.proto.ingestion.MutateRequest\x1a\".cz.proto.ingestion.MutateResponse(\x01\x30\x01\x12[\n\x0eMutateInternal\x12!.cz.proto.ingestion.MutateRequest\x1a\".cz.proto.ingestion.MutateResponse(\x01\x30\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ingestion_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _METHODENUM._serialized_start=5628
-  _METHODENUM._serialized_end=6285
-  _IGSTABLETYPE._serialized_start=6287
-  _IGSTABLETYPE._serialized_end=6336
-  _CODE._serialized_start=6338
-  _CODE._serialized_end=6384
-  _BULKLOADSTREAMSTATE._serialized_start=6387
-  _BULKLOADSTREAMSTATE._serialized_end=6527
-  _BULKLOADSTREAMOPERATION._serialized_start=6529
-  _BULKLOADSTREAMOPERATION._serialized_end=6602
-  _CONNECTMODE._serialized_start=6604
-  _CONNECTMODE._serialized_end=6664
-  _OPERATIONTYPE._serialized_start=6667
-  _OPERATIONTYPE._serialized_end=6800
+  _BULKLOADSTREAMINFO_ENCRYPTIONOPTIONSENTRY._options = None
+  _BULKLOADSTREAMINFO_ENCRYPTIONOPTIONSENTRY._serialized_options = b'8\001'
+  _METHODENUM._serialized_start=5870
+  _METHODENUM._serialized_end=6527
+  _IGSTABLETYPE._serialized_start=6529
+  _IGSTABLETYPE._serialized_end=6578
+  _CODE._serialized_start=6580
+  _CODE._serialized_end=6626
+  _BULKLOADSTREAMSTATE._serialized_start=6629
+  _BULKLOADSTREAMSTATE._serialized_end=6769
+  _BULKLOADSTREAMOPERATION._serialized_start=6771
+  _BULKLOADSTREAMOPERATION._serialized_end=6844
+  _CONNECTMODE._serialized_start=6846
+  _CONNECTMODE._serialized_end=6906
+  _OPERATIONTYPE._serialized_start=6909
+  _OPERATIONTYPE._serialized_end=7042
   _GATEWAYREQUEST._serialized_start=80
   _GATEWAYREQUEST._serialized_end=174
   _GATEWAYRESPONSE._serialized_start=176
   _GATEWAYRESPONSE._serialized_end=269
   _USERIDENTIFIER._serialized_start=271
   _USERIDENTIFIER._serialized_end=363
   _ACCOUNT._serialized_start=365
@@ -65,57 +67,59 @@
   _CREATEORGETSTREAMRESPONSE._serialized_start=1374
   _CREATEORGETSTREAMRESPONSE._serialized_end=1590
   _CLOSESTREAMREQUEST._serialized_start=1592
   _CLOSESTREAMREQUEST._serialized_end=1716
   _CLOSESTREAMRESPONSE._serialized_start=1718
   _CLOSESTREAMRESPONSE._serialized_end=1791
   _OSSSTAGINGPATHINFO._serialized_start=1794
-  _OSSSTAGINGPATHINFO._serialized_end=1942
-  _STAGINGPATHINFO._serialized_start=1944
-  _STAGINGPATHINFO._serialized_end=2034
-  _BULKLOADSTREAMINFO._serialized_start=2037
-  _BULKLOADSTREAMINFO._serialized_end=2405
-  _BULKLOADSTREAMWRITERCONFIG._serialized_start=2408
-  _BULKLOADSTREAMWRITERCONFIG._serialized_end=2609
-  _CREATEBULKLOADSTREAMREQUEST._serialized_start=2612
-  _CREATEBULKLOADSTREAMREQUEST._serialized_end=2853
-  _CREATEBULKLOADSTREAMRESPONSE._serialized_start=2856
-  _CREATEBULKLOADSTREAMRESPONSE._serialized_end=2992
-  _GETBULKLOADSTREAMREQUEST._serialized_start=2995
-  _GETBULKLOADSTREAMREQUEST._serialized_end=3168
-  _GETBULKLOADSTREAMRESPONSE._serialized_start=3171
-  _GETBULKLOADSTREAMRESPONSE._serialized_end=3304
-  _COMMITBULKLOADSTREAMREQUEST._serialized_start=3307
-  _COMMITBULKLOADSTREAMREQUEST._serialized_end=3670
-  _COMMITBULKLOADSTREAMREQUEST_COMMITMODE._serialized_start=3621
-  _COMMITBULKLOADSTREAMREQUEST_COMMITMODE._serialized_end=3670
-  _COMMITBULKLOADSTREAMRESPONSE._serialized_start=3673
-  _COMMITBULKLOADSTREAMRESPONSE._serialized_end=3809
-  _OPENBULKLOADSTREAMWRITERREQUEST._serialized_start=3812
-  _OPENBULKLOADSTREAMWRITERREQUEST._serialized_end=3989
-  _OPENBULKLOADSTREAMWRITERRESPONSE._serialized_start=3992
-  _OPENBULKLOADSTREAMWRITERRESPONSE._serialized_end=4142
-  _FINISHBULKLOADSTREAMWRITERREQUEST._serialized_start=4145
-  _FINISHBULKLOADSTREAMWRITERREQUEST._serialized_end=4372
-  _FINISHBULKLOADSTREAMWRITERRESPONSE._serialized_start=4374
-  _FINISHBULKLOADSTREAMWRITERRESPONSE._serialized_end=4462
-  _GETROUTEWORKERSREQUEST._serialized_start=4465
-  _GETROUTEWORKERSREQUEST._serialized_end=4621
-  _HOSTPORTTUPLE._serialized_start=4623
-  _HOSTPORTTUPLE._serialized_end=4666
-  _GETROUTEWORKERSRESPONSE._serialized_start=4669
-  _GETROUTEWORKERSRESPONSE._serialized_end=4815
-  _OPERATIONTYPELIST._serialized_start=4817
-  _OPERATIONTYPELIST._serialized_end=4889
-  _DATABLOCK._serialized_start=4892
-  _DATABLOCK._serialized_end=5138
-  _MUTATEROWSTATUS._serialized_start=5140
-  _MUTATEROWSTATUS._serialized_end=5239
-  _MUTATEREQUEST._serialized_start=5242
-  _MUTATEREQUEST._serialized_end=5456
-  _MUTATERESPONSE._serialized_start=5459
-  _MUTATERESPONSE._serialized_end=5625
-  _INGESTIONCONTROLLERSERVICE._serialized_start=6803
-  _INGESTIONCONTROLLERSERVICE._serialized_end=7878
-  _INGESTIONWORKERSERVICE._serialized_start=7881
-  _INGESTIONWORKERSERVICE._serialized_end=8083
+  _OSSSTAGINGPATHINFO._serialized_end=1967
+  _STAGINGPATHINFO._serialized_start=1969
+  _STAGINGPATHINFO._serialized_end=2059
+  _BULKLOADSTREAMINFO._serialized_start=2062
+  _BULKLOADSTREAMINFO._serialized_end=2613
+  _BULKLOADSTREAMINFO_ENCRYPTIONOPTIONSENTRY._serialized_start=2557
+  _BULKLOADSTREAMINFO_ENCRYPTIONOPTIONSENTRY._serialized_end=2613
+  _BULKLOADSTREAMWRITERCONFIG._serialized_start=2616
+  _BULKLOADSTREAMWRITERCONFIG._serialized_end=2817
+  _CREATEBULKLOADSTREAMREQUEST._serialized_start=2820
+  _CREATEBULKLOADSTREAMREQUEST._serialized_end=3095
+  _CREATEBULKLOADSTREAMRESPONSE._serialized_start=3098
+  _CREATEBULKLOADSTREAMRESPONSE._serialized_end=3234
+  _GETBULKLOADSTREAMREQUEST._serialized_start=3237
+  _GETBULKLOADSTREAMREQUEST._serialized_end=3410
+  _GETBULKLOADSTREAMRESPONSE._serialized_start=3413
+  _GETBULKLOADSTREAMRESPONSE._serialized_end=3546
+  _COMMITBULKLOADSTREAMREQUEST._serialized_start=3549
+  _COMMITBULKLOADSTREAMREQUEST._serialized_end=3912
+  _COMMITBULKLOADSTREAMREQUEST_COMMITMODE._serialized_start=3863
+  _COMMITBULKLOADSTREAMREQUEST_COMMITMODE._serialized_end=3912
+  _COMMITBULKLOADSTREAMRESPONSE._serialized_start=3915
+  _COMMITBULKLOADSTREAMRESPONSE._serialized_end=4051
+  _OPENBULKLOADSTREAMWRITERREQUEST._serialized_start=4054
+  _OPENBULKLOADSTREAMWRITERREQUEST._serialized_end=4231
+  _OPENBULKLOADSTREAMWRITERRESPONSE._serialized_start=4234
+  _OPENBULKLOADSTREAMWRITERRESPONSE._serialized_end=4384
+  _FINISHBULKLOADSTREAMWRITERREQUEST._serialized_start=4387
+  _FINISHBULKLOADSTREAMWRITERREQUEST._serialized_end=4614
+  _FINISHBULKLOADSTREAMWRITERRESPONSE._serialized_start=4616
+  _FINISHBULKLOADSTREAMWRITERRESPONSE._serialized_end=4704
+  _GETROUTEWORKERSREQUEST._serialized_start=4707
+  _GETROUTEWORKERSREQUEST._serialized_end=4863
+  _HOSTPORTTUPLE._serialized_start=4865
+  _HOSTPORTTUPLE._serialized_end=4908
+  _GETROUTEWORKERSRESPONSE._serialized_start=4911
+  _GETROUTEWORKERSRESPONSE._serialized_end=5057
+  _OPERATIONTYPELIST._serialized_start=5059
+  _OPERATIONTYPELIST._serialized_end=5131
+  _DATABLOCK._serialized_start=5134
+  _DATABLOCK._serialized_end=5380
+  _MUTATEROWSTATUS._serialized_start=5382
+  _MUTATEROWSTATUS._serialized_end=5481
+  _MUTATEREQUEST._serialized_start=5484
+  _MUTATEREQUEST._serialized_end=5698
+  _MUTATERESPONSE._serialized_start=5701
+  _MUTATERESPONSE._serialized_end=5867
+  _INGESTIONCONTROLLERSERVICE._serialized_start=7045
+  _INGESTIONCONTROLLERSERVICE._serialized_end=8120
+  _INGESTIONWORKERSERVICE._serialized_start=8123
+  _INGESTIONWORKERSERVICE._serialized_end=8325
 # @@protoc_insertion_point(module_scope)
```

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/ingestion_pb2_grpc.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/ingestion_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/input_split_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/input_split_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/job_meta_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/job_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/job_result_cache_meta_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/job_result_cache_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/kudu_common_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/kudu_common_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/metadata_entity_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/metadata_entity_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/network_policy_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/network_policy_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/object_identifier_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/object_identifier_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/operator_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/operator_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/pb_util_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/pb_util_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/property_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/property_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/rm_app_meta_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/rm_app_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/role_meta_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/role_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/row_operations_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/row_operations_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/schema_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/share_meta_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/share_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/statistics_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/table_common_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/table_common_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/table_meta_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/table_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/virtual_cluster_meta_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_cluster_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/virtual_cluster_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/virtual_cluster_size_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_cluster_size_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/virtual_value_info_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/virtual_value_info_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/generated/workspace_meta_pb2.py` & `clickzetta-connector-0.7.3/clickzetta/proto/generated/workspace_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/account.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/account.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/block_bloom_filter.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/block_bloom_filter.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/compression.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/compression.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/data_type.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/data_type.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/expression.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/expression.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/file_meta_data.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/file_meta_data.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/function_meta.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/function_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/hash.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/hash.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/ingestion.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/ingestion.proto`

 * *Files 3% similar despite different names*

```diff
@@ -164,14 +164,15 @@
 message OssStagingPathInfo {
   string path = 1;
   string sts_ak_id = 3;
   string sts_ak_secret = 4;
   string sts_token = 5;
   string oss_endpoint = 6;
   string oss_internal_endpoint = 7;
+  uint64 oss_expire_time = 8;
 }
 
 message StagingPathInfo {
   oneof path_info {
     OssStagingPathInfo oss_path = 1;
   }
 }
@@ -182,14 +183,18 @@
   string sql_job_id = 3;
   TableIdentifier identifier = 4;
   BulkLoadStreamOperation operation = 5;
   string partition_spec = 6;
   repeated string record_keys = 7;
   StreamSchema stream_schema = 8;
   string sql_error_msg = 9;
+  bool prefer_internal_endpoint = 10;
+  // Encryption config of cloud object stores.
+  // Use a map here as these options vary from cloud to cloud.
+  map<string, string> encryption_options = 11;
 }
 
 message BulkLoadStreamWriterConfig {
   StagingPathInfo staging_path = 1;
   cz.proto.FileFormatType file_format = 2;
   int64 max_num_rows_per_file = 3;
   int64 max_size_in_bytes_per_file = 4;
@@ -197,14 +202,15 @@
 
 message CreateBulkLoadStreamRequest {
   Account account = 1;
   TableIdentifier identifier = 2;
   BulkLoadStreamOperation operation = 3;
   string partition_spec = 4;
   repeated string record_keys = 5;
+  bool prefer_internal_endpoint = 6;
 }
 
 message CreateBulkLoadStreamResponse {
   ResponseStatus status = 1;
   BulkLoadStreamInfo info = 2;
 }
```

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/input_split.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/input_split.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/job_meta.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/job_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/kudu_common.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/kudu_common.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/metadata_entity.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/metadata_entity.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/object_identifier.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/object_identifier.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/operator.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/operator.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/pb_util.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/pb_util.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/rm_app_meta.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/rm_app_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/row_operations.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/row_operations.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/statistics.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/statistics.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/table_common.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/table_common.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/table_meta.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/table_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/virtual_cluster.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/virtual_cluster.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/virtual_cluster_meta.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/virtual_cluster_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/proto/source/virtual_value_info.proto` & `clickzetta-connector-0.7.3/clickzetta/proto/source/virtual_value_info.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/query_result.py` & `clickzetta-connector-0.7.3/clickzetta/query_result.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/schema.py` & `clickzetta-connector-0.7.3/clickzetta/schema.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/session.py` & `clickzetta-connector-0.7.3/clickzetta/session.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/standard_sql.py` & `clickzetta-connector-0.7.3/clickzetta/standard_sql.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta/table.py` & `clickzetta-connector-0.7.3/clickzetta/table.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta_connector.egg-info/SOURCES.txt` & `clickzetta-connector-0.7.3/clickzetta_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/clickzetta_connector.egg-info/requires.txt` & `clickzetta-connector-0.7.3/clickzetta_connector.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.2/setup.py` & `clickzetta-connector-0.7.3/setup.py`

 * *Files identical despite different names*

