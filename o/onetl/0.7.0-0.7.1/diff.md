# Comparing `tmp/onetl-0.7.0.tar.gz` & `tmp/onetl-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onetl-0.7.0.tar", last modified: Mon May 15 08:32:36 2023, max compression
+gzip compressed data, was "onetl-0.7.1.tar", last modified: Tue May 23 08:11:54 2023, max compression
```

## Comparing `onetl-0.7.0.tar` & `onetl-0.7.1.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.531095 onetl-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-05-15 08:32:26.000000 onetl-0.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-15 08:32:26.000000 onetl-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17367 2023-05-15 08:32:36.531095 onetl-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-05-15 08:32:26.000000 onetl-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.511095 onetl-0.7.0/onetl/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/_internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.515095 onetl-0.7.0/onetl/base/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/base/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/base/base_db_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/base/base_file_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/base/base_file_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/base/base_file_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/base/contains_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/base/contains_get_df_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/base/path_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/base/path_stat_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.515095 onetl-0.7.0/onetl/connection/
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.515095 onetl-0.7.0/onetl/connection/db_connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/db_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.519095 onetl-0.7.0/onetl/connection/db_connection/dialect_mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/dialect_mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/dialect_mixins/support_columns_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/dialect_mixins/support_columns_none.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/dialect_mixins/support_df_schema_none.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/dialect_mixins/support_df_schema_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/dialect_mixins/support_hint_none.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/dialect_mixins/support_hint_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_none.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/dialect_mixins/support_table_with_dbschema.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/dialect_mixins/support_table_without_dbschema.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/dialect_mixins/support_where_str.py
--rw-r--r--   0 runner    (1001) docker     (123)    26511 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/greenplum.py
--rw-r--r--   0 runner    (1001) docker     (123)    32279 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/hive.py
--rw-r--r--   0 runner    (1001) docker     (123)    27892 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/jdbc_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    23510 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/jdbc_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    25845 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/mssql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/db_connection/teradata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.519095 onetl-0.7.0/onetl/connection/file_connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/file_connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25013 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/file_connection/file_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/file_connection/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/file_connection/ftps.py
--rw-r--r--   0 runner    (1001) docker     (123)    26223 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/file_connection/hdfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/file_connection/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/file_connection/sftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/file_connection/webdav.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/connection/kerberos_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.519095 onetl-0.7.0/onetl/core/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.519095 onetl-0.7.0/onetl/core/db_reader/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/db_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21789 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/db_reader/db_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/db_reader/strategy_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.519095 onetl-0.7.0/onetl/core/db_writer/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/db_writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/db_writer/db_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.519095 onetl-0.7.0/onetl/core/file_downloader/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/file_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/file_downloader/download_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    25273 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/file_downloader/file_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.523095 onetl-0.7.0/onetl/core/file_filter/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/file_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/file_filter/file_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/file_filter/file_hwm_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/file_filter/match_all_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.523095 onetl-0.7.0/onetl/core/file_limit/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/file_limit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/file_limit/file_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/file_limit/limits_reached.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.523095 onetl-0.7.0/onetl/core/file_result/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/file_result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18432 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/file_result/file_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/file_result/file_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.523095 onetl-0.7.0/onetl/core/file_uploader/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/file_uploader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/file_uploader/file_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/core/file_uploader/upload_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.523095 onetl-0.7.0/onetl/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/hooks/hook_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/hooks/hooks_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/hooks/method_inheritance_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)    20801 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/hooks/slot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/hooks/support_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.523095 onetl-0.7.0/onetl/hwm/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/hwm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/hwm/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.527095 onetl-0.7.0/onetl/hwm/store/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/hwm/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/hwm/store/base_hwm_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/hwm/store/hwm_class_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/hwm/store/hwm_store_class_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/hwm/store/hwm_store_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/hwm/store/memory_hwm_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/hwm/store/yaml_hwm_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.527095 onetl-0.7.0/onetl/impl/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/impl/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/impl/failed_local_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/impl/file_write_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/impl/frozen_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/impl/generic_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/impl/local_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/impl/path_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/impl/path_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/impl/remote_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/impl/remote_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/impl/remote_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/impl/remote_path_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.527095 onetl-0.7.0/onetl/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/plugins/import_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.527095 onetl-0.7.0/onetl/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/strategy/base_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/strategy/batch_hwm_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.527095 onetl-0.7.0/onetl/strategy/hwm_store/
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/strategy/hwm_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/strategy/hwm_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19047 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/strategy/incremental_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/strategy/snapshot_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/strategy/strategy_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-15 08:32:26.000000 onetl-0.7.0/onetl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.511095 onetl-0.7.0/onetl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17367 2023-05-15 08:32:36.000000 onetl-0.7.0/onetl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-15 08:32:36.000000 onetl-0.7.0/onetl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 08:32:36.000000 onetl-0.7.0/onetl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 08:32:36.000000 onetl-0.7.0/onetl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-15 08:32:36.000000 onetl-0.7.0/onetl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 08:32:36.000000 onetl-0.7.0/onetl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-15 08:32:26.000000 onetl-0.7.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.531095 onetl-0.7.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-15 08:32:26.000000 onetl-0.7.0/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-15 08:32:26.000000 onetl-0.7.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-15 08:32:26.000000 onetl-0.7.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-15 08:32:26.000000 onetl-0.7.0/requirements/ftp.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-15 08:32:26.000000 onetl-0.7.0/requirements/hdfs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-15 08:32:26.000000 onetl-0.7.0/requirements/kerberos.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 08:32:26.000000 onetl-0.7.0/requirements/s3.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 08:32:26.000000 onetl-0.7.0/requirements/sftp.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 08:32:26.000000 onetl-0.7.0/requirements/spark.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:32:36.531095 onetl-0.7.0/requirements/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 08:32:26.000000 onetl-0.7.0/requirements/tests/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 08:32:26.000000 onetl-0.7.0/requirements/tests/clickhouse.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 08:32:26.000000 onetl-0.7.0/requirements/tests/mongodb.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 08:32:26.000000 onetl-0.7.0/requirements/tests/mssql.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 08:32:26.000000 onetl-0.7.0/requirements/tests/mysql.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 08:32:26.000000 onetl-0.7.0/requirements/tests/oracle.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 08:32:26.000000 onetl-0.7.0/requirements/tests/postgres.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-15 08:32:26.000000 onetl-0.7.0/requirements/tests/spark-2.4.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-15 08:32:26.000000 onetl-0.7.0/requirements/tests/spark-3.2.3.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-15 08:32:26.000000 onetl-0.7.0/requirements/tests/spark-3.3.2.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-15 08:32:26.000000 onetl-0.7.0/requirements/tests/spark-3.4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 08:32:26.000000 onetl-0.7.0/requirements/webdav.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-15 08:32:36.535095 onetl-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-15 08:32:26.000000 onetl-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.730814 onetl-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-05-23 08:11:50.000000 onetl-0.7.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-23 08:11:50.000000 onetl-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17338 2023-05-23 08:11:54.730814 onetl-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-05-23 08:11:50.000000 onetl-0.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.714814 onetl-0.7.1/onetl/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/_internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.718814 onetl-0.7.1/onetl/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/base/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/base/base_db_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/base/base_file_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/base/base_file_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/base/base_file_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/base/contains_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/base/contains_get_df_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/base/path_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/base/path_stat_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.718814 onetl-0.7.1/onetl/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.718814 onetl-0.7.1/onetl/connection/db_connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/db_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.718814 onetl-0.7.1/onetl/connection/db_connection/dialect_mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/dialect_mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/dialect_mixins/support_columns_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/dialect_mixins/support_columns_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/dialect_mixins/support_df_schema_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/dialect_mixins/support_df_schema_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/dialect_mixins/support_hint_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/dialect_mixins/support_hint_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/dialect_mixins/support_table_with_dbschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/dialect_mixins/support_table_without_dbschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/dialect_mixins/support_where_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26511 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/greenplum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32279 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/hive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27892 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/jdbc_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23510 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/jdbc_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25845 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/db_connection/teradata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.722814 onetl-0.7.1/onetl/connection/file_connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/file_connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25013 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/file_connection/file_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/file_connection/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/file_connection/ftps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26222 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/file_connection/hdfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/file_connection/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/file_connection/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/file_connection/webdav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/connection/kerberos_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.722814 onetl-0.7.1/onetl/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.722814 onetl-0.7.1/onetl/core/db_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/db_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21805 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/db_reader/db_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/db_reader/strategy_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.722814 onetl-0.7.1/onetl/core/db_writer/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/db_writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/db_writer/db_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.722814 onetl-0.7.1/onetl/core/file_downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/file_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/file_downloader/download_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25273 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/file_downloader/file_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.722814 onetl-0.7.1/onetl/core/file_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/file_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/file_filter/file_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/file_filter/file_hwm_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/file_filter/match_all_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.722814 onetl-0.7.1/onetl/core/file_limit/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/file_limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/file_limit/file_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/file_limit/limits_reached.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.722814 onetl-0.7.1/onetl/core/file_result/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/file_result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18432 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/file_result/file_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/file_result/file_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.722814 onetl-0.7.1/onetl/core/file_uploader/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/file_uploader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/file_uploader/file_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/core/file_uploader/upload_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.726814 onetl-0.7.1/onetl/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/hooks/hook_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/hooks/hooks_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/hooks/method_inheritance_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20801 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/hooks/slot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/hooks/support_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.726814 onetl-0.7.1/onetl/hwm/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/hwm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/hwm/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.726814 onetl-0.7.1/onetl/hwm/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/hwm/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/hwm/store/base_hwm_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/hwm/store/hwm_class_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/hwm/store/hwm_store_class_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/hwm/store/hwm_store_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/hwm/store/memory_hwm_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/hwm/store/yaml_hwm_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.726814 onetl-0.7.1/onetl/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/impl/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/impl/failed_local_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/impl/file_write_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/impl/frozen_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/impl/generic_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/impl/local_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/impl/path_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/impl/path_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/impl/remote_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/impl/remote_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/impl/remote_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/impl/remote_path_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.726814 onetl-0.7.1/onetl/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/plugins/import_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.726814 onetl-0.7.1/onetl/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/strategy/base_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/strategy/batch_hwm_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.726814 onetl-0.7.1/onetl/strategy/hwm_store/
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/strategy/hwm_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/strategy/hwm_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19047 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/strategy/incremental_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/strategy/snapshot_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/strategy/strategy_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-23 08:11:50.000000 onetl-0.7.1/onetl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.714814 onetl-0.7.1/onetl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17338 2023-05-23 08:11:54.000000 onetl-0.7.1/onetl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-23 08:11:54.000000 onetl-0.7.1/onetl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:11:54.000000 onetl-0.7.1/onetl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:11:54.000000 onetl-0.7.1/onetl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-23 08:11:54.000000 onetl-0.7.1/onetl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 08:11:54.000000 onetl-0.7.1/onetl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-23 08:11:50.000000 onetl-0.7.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.730814 onetl-0.7.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 08:11:50.000000 onetl-0.7.1/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-23 08:11:50.000000 onetl-0.7.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-23 08:11:50.000000 onetl-0.7.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-23 08:11:50.000000 onetl-0.7.1/requirements/ftp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 08:11:50.000000 onetl-0.7.1/requirements/hdfs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 08:11:50.000000 onetl-0.7.1/requirements/kerberos.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 08:11:50.000000 onetl-0.7.1/requirements/s3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 08:11:50.000000 onetl-0.7.1/requirements/sftp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 08:11:50.000000 onetl-0.7.1/requirements/spark.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:11:54.730814 onetl-0.7.1/requirements/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 08:11:50.000000 onetl-0.7.1/requirements/tests/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 08:11:50.000000 onetl-0.7.1/requirements/tests/clickhouse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 08:11:50.000000 onetl-0.7.1/requirements/tests/mongodb.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 08:11:50.000000 onetl-0.7.1/requirements/tests/mssql.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 08:11:50.000000 onetl-0.7.1/requirements/tests/mysql.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 08:11:50.000000 onetl-0.7.1/requirements/tests/oracle.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 08:11:50.000000 onetl-0.7.1/requirements/tests/postgres.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-23 08:11:50.000000 onetl-0.7.1/requirements/tests/spark-2.4.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-23 08:11:50.000000 onetl-0.7.1/requirements/tests/spark-3.2.3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-23 08:11:50.000000 onetl-0.7.1/requirements/tests/spark-3.3.2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 08:11:50.000000 onetl-0.7.1/requirements/tests/spark-3.4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 08:11:50.000000 onetl-0.7.1/requirements/webdav.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-23 08:11:54.730814 onetl-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-23 08:11:50.000000 onetl-0.7.1/setup.py
```

### Comparing `onetl-0.7.0/LICENSE.txt` & `onetl-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/PKG-INFO` & `onetl-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: onetl
-Version: 0.7.0
+Version: 0.7.1
 Summary: One ETL tool to rule them all
 Home-page: https://github.com/MobileTeleSystems/onetl
 Author: DataOps.ETL
 Author-email: onetools@mts.ru
 License: Apache License 2.0
-Project-URL: Documentation, https://onetl.readthedocs.io/en/stable/
+Project-URL: Documentation, https://onetl.readthedocs.io/
 Project-URL: Source, https://github.com/MobileTeleSystems/onetl
 Project-URL: CI/CD, https://github.com/MobileTeleSystems/onetl/actions
 Project-URL: Tracker, https://github.com/MobileTeleSystems/onetl/issues
 Keywords: Spark,ETL,JDBC,HWM
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pydantic :: 1
@@ -48,23 +48,23 @@
 onETL
 =====
 
 |Repo Status| |PyPI| |PyPI License| |PyPI Python Version|
 |Documentation| |Build Status| |Coverage|
 
 .. |Repo Status| image:: https://www.repostatus.org/badges/latest/active.svg
-    :target: https://www.repostatus.org/#active
+    :target: https://github.com/MobileTeleSystems/onetl
 .. |PyPI| image:: https://img.shields.io/pypi/v/onetl
     :target: https://pypi.org/project/onetl/
 .. |PyPI License| image:: https://img.shields.io/pypi/l/onetl.svg
     :target: https://github.com/MobileTeleSystems/onetl/blob/develop/LICENSE.txt
 .. |PyPI Python Version| image:: https://img.shields.io/pypi/pyversions/onetl.svg
     :target: https://badge.fury.io/py/onetl
 .. |Documentation| image:: https://readthedocs.org/projects/onetl/badge/?version=stable
-    :target: https://onetl.readthedocs.io/en/stable/
+    :target: https://onetl.readthedocs.io/
 .. |Build Status| image:: https://github.com/MobileTeleSystems/onetl/workflows/Tests/badge.svg
     :target: https://github.com/MobileTeleSystems/onetl/actions
 .. |Coverage| image:: https://codecov.io/gh/MobileTeleSystems/onetl/branch/develop/graph/badge.svg?token=RIO8URKNZJ
     :target: https://codecov.io/gh/MobileTeleSystems/onetl
 
 |Logo|
 
@@ -92,27 +92,27 @@
 
 Supported storages
 ------------------
 
 +------------+------------+----------------------------------------------------------------------------------------------------------+
 | Type       | Storage    | Powered by                                                                                               |
 +============+============+==========================================================================================================+
-| Database   | Clickhouse | Apache Spark `JDBC Data Source <https://spark.apache.org/docs/2.4.8/sql-data-sources-jdbc.html>`_        |
+| Database   | Clickhouse | Apache Spark `JDBC Data Source <https://spark.apache.org/docs/3.4.0/sql-data-sources-jdbc.html>`_        |
 +            +------------+                                                                                                          +
 |            | MSSQL      |                                                                                                          |
 +            +------------+                                                                                                          +
 |            | MySQL      |                                                                                                          |
 +            +------------+                                                                                                          +
 |            | Postgres   |                                                                                                          |
 +            +------------+                                                                                                          +
 |            | Oracle     |                                                                                                          |
 +            +------------+                                                                                                          +
 |            | Teradata   |                                                                                                          |
 +            +------------+----------------------------------------------------------------------------------------------------------+
-|            | Hive       | Apache Spark `Hive integration <https://spark.apache.org/docs/2.4.8/sql-data-sources-hive-tables.html>`_ |
+|            | Hive       | Apache Spark `Hive integration <https://spark.apache.org/docs/3.4.0/sql-data-sources-hive-tables.html>`_ |
 +            +------------+----------------------------------------------------------------------------------------------------------+
 |            | Greenplum  | Pivotal `Greenplum Spark connector <https://network.tanzu.vmware.com/products/vmware-tanzu-greenplum>`_  |
 +            +------------+----------------------------------------------------------------------------------------------------------+
 |            | MongoDB    | `MongoDB Spark connector <https://www.mongodb.com/docs/spark-connector/current>`_                        |
 +------------+------------+----------------------------------------------------------------------------------------------------------+
 | File       | HDFS       | `HDFS Python client <https://pypi.org/project/hdfs/>`_                                                   |
 +            +------------+----------------------------------------------------------------------------------------------------------+
@@ -129,15 +129,15 @@
 
 
 .. documentation
 
 Documentation
 -------------
 
-See https://onetl.readthedocs.io/en/stable/
+See https://onetl.readthedocs.io/
 
 .. contribution
 
 Contribution guide
 -------------------
 
 See `<CONTRIBUTING.rst>`__
@@ -238,15 +238,15 @@
 All file connection classes (``FTP``,  ``SFTP``, ``HDFS`` and so on) requires specific Python clients to be installed.
 
 Each client can be installed explicitly by passing connector name (in lowercase) to ``extras``:
 
 .. code:: bash
 
     pip install onetl[ftp]  # specific connector
-    pip install onetl[ftp, ftps, sftp, hdfs, s3, webdav]  # multiple connectors
+    pip install onetl[ftp,ftps,sftp,hdfs,s3,webdav]  # multiple connectors
 
 To install all file connectors at once you can pass ``files`` to ``extras``:
 
 .. code:: bash
 
     pip install onetl[files]
 
@@ -297,15 +297,15 @@
 To install all connectors and dependencies, you can pass ``all`` into ``extras``:
 
 .. code:: bash
 
     pip install onetl[all]
 
     # this is just the same as
-    pip install onetl[spark, files, kerberos]
+    pip install onetl[spark,files,kerberos]
 
 .. warning::
 
     This method consumes a lot of disk space, and requires for Java & Kerberos libraries to be installed into your OS.
 
 .. develops
```

### Comparing `onetl-0.7.0/README.rst` & `onetl-0.7.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 onETL
 =====
 
 |Repo Status| |PyPI| |PyPI License| |PyPI Python Version|
 |Documentation| |Build Status| |Coverage|
 
 .. |Repo Status| image:: https://www.repostatus.org/badges/latest/active.svg
-    :target: https://www.repostatus.org/#active
+    :target: https://github.com/MobileTeleSystems/onetl
 .. |PyPI| image:: https://img.shields.io/pypi/v/onetl
     :target: https://pypi.org/project/onetl/
 .. |PyPI License| image:: https://img.shields.io/pypi/l/onetl.svg
     :target: https://github.com/MobileTeleSystems/onetl/blob/develop/LICENSE.txt
 .. |PyPI Python Version| image:: https://img.shields.io/pypi/pyversions/onetl.svg
     :target: https://badge.fury.io/py/onetl
 .. |Documentation| image:: https://readthedocs.org/projects/onetl/badge/?version=stable
-    :target: https://onetl.readthedocs.io/en/stable/
+    :target: https://onetl.readthedocs.io/
 .. |Build Status| image:: https://github.com/MobileTeleSystems/onetl/workflows/Tests/badge.svg
     :target: https://github.com/MobileTeleSystems/onetl/actions
 .. |Coverage| image:: https://codecov.io/gh/MobileTeleSystems/onetl/branch/develop/graph/badge.svg?token=RIO8URKNZJ
     :target: https://codecov.io/gh/MobileTeleSystems/onetl
 
 |Logo|
 
@@ -47,27 +47,27 @@
 
 Supported storages
 ------------------
 
 +------------+------------+----------------------------------------------------------------------------------------------------------+
 | Type       | Storage    | Powered by                                                                                               |
 +============+============+==========================================================================================================+
-| Database   | Clickhouse | Apache Spark `JDBC Data Source <https://spark.apache.org/docs/2.4.8/sql-data-sources-jdbc.html>`_        |
+| Database   | Clickhouse | Apache Spark `JDBC Data Source <https://spark.apache.org/docs/3.4.0/sql-data-sources-jdbc.html>`_        |
 +            +------------+                                                                                                          +
 |            | MSSQL      |                                                                                                          |
 +            +------------+                                                                                                          +
 |            | MySQL      |                                                                                                          |
 +            +------------+                                                                                                          +
 |            | Postgres   |                                                                                                          |
 +            +------------+                                                                                                          +
 |            | Oracle     |                                                                                                          |
 +            +------------+                                                                                                          +
 |            | Teradata   |                                                                                                          |
 +            +------------+----------------------------------------------------------------------------------------------------------+
-|            | Hive       | Apache Spark `Hive integration <https://spark.apache.org/docs/2.4.8/sql-data-sources-hive-tables.html>`_ |
+|            | Hive       | Apache Spark `Hive integration <https://spark.apache.org/docs/3.4.0/sql-data-sources-hive-tables.html>`_ |
 +            +------------+----------------------------------------------------------------------------------------------------------+
 |            | Greenplum  | Pivotal `Greenplum Spark connector <https://network.tanzu.vmware.com/products/vmware-tanzu-greenplum>`_  |
 +            +------------+----------------------------------------------------------------------------------------------------------+
 |            | MongoDB    | `MongoDB Spark connector <https://www.mongodb.com/docs/spark-connector/current>`_                        |
 +------------+------------+----------------------------------------------------------------------------------------------------------+
 | File       | HDFS       | `HDFS Python client <https://pypi.org/project/hdfs/>`_                                                   |
 +            +------------+----------------------------------------------------------------------------------------------------------+
@@ -84,15 +84,15 @@
 
 
 .. documentation
 
 Documentation
 -------------
 
-See https://onetl.readthedocs.io/en/stable/
+See https://onetl.readthedocs.io/
 
 .. contribution
 
 Contribution guide
 -------------------
 
 See `<CONTRIBUTING.rst>`__
@@ -193,15 +193,15 @@
 All file connection classes (``FTP``,  ``SFTP``, ``HDFS`` and so on) requires specific Python clients to be installed.
 
 Each client can be installed explicitly by passing connector name (in lowercase) to ``extras``:
 
 .. code:: bash
 
     pip install onetl[ftp]  # specific connector
-    pip install onetl[ftp, ftps, sftp, hdfs, s3, webdav]  # multiple connectors
+    pip install onetl[ftp,ftps,sftp,hdfs,s3,webdav]  # multiple connectors
 
 To install all file connectors at once you can pass ``files`` to ``extras``:
 
 .. code:: bash
 
     pip install onetl[files]
 
@@ -252,15 +252,15 @@
 To install all connectors and dependencies, you can pass ``all`` into ``extras``:
 
 .. code:: bash
 
     pip install onetl[all]
 
     # this is just the same as
-    pip install onetl[spark, files, kerberos]
+    pip install onetl[spark,files,kerberos]
 
 .. warning::
 
     This method consumes a lot of disk space, and requires for Java & Kerberos libraries to be installed into your OS.
 
 .. develops
```

### Comparing `onetl-0.7.0/onetl/__init__.py` & `onetl-0.7.1/onetl/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/_internal.py` & `onetl-0.7.1/onetl/_internal.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/base/__init__.py` & `onetl-0.7.1/onetl/base/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/base/base_connection.py` & `onetl-0.7.1/onetl/base/base_connection.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/base/base_db_connection.py` & `onetl-0.7.1/onetl/base/base_db_connection.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/base/base_file_connection.py` & `onetl-0.7.1/onetl/base/base_file_connection.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/base/base_file_filter.py` & `onetl-0.7.1/onetl/base/base_file_filter.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/base/base_file_limit.py` & `onetl-0.7.1/onetl/base/base_file_limit.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/base/contains_exception.py` & `onetl-0.7.1/onetl/base/contains_exception.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/base/contains_get_df_schema.py` & `onetl-0.7.1/onetl/base/contains_get_df_schema.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/base/path_protocol.py` & `onetl-0.7.1/onetl/base/path_protocol.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/base/path_stat_protocol.py` & `onetl-0.7.1/onetl/base/path_stat_protocol.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/__init__.py` & `onetl-0.7.1/onetl/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/db_connection/clickhouse.py` & `onetl-0.7.1/onetl/connection/db_connection/clickhouse.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/db_connection/db_connection.py` & `onetl-0.7.1/onetl/connection/db_connection/db_connection.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/db_connection/dialect_mixins/__init__.py` & `onetl-0.7.1/onetl/connection/db_connection/dialect_mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/db_connection/dialect_mixins/support_hint_str.py` & `onetl-0.7.1/onetl/connection/db_connection/dialect_mixins/support_hint_str.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_str.py` & `onetl-0.7.1/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_str.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/db_connection/dialect_mixins/support_where_str.py` & `onetl-0.7.1/onetl/connection/db_connection/dialect_mixins/support_where_str.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/db_connection/greenplum.py` & `onetl-0.7.1/onetl/connection/db_connection/greenplum.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/db_connection/hive.py` & `onetl-0.7.1/onetl/connection/db_connection/hive.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/db_connection/jdbc_connection.py` & `onetl-0.7.1/onetl/connection/db_connection/jdbc_connection.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/db_connection/jdbc_mixin.py` & `onetl-0.7.1/onetl/connection/db_connection/jdbc_mixin.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/db_connection/mongodb.py` & `onetl-0.7.1/onetl/connection/db_connection/mongodb.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/db_connection/mssql.py` & `onetl-0.7.1/onetl/connection/db_connection/mssql.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/db_connection/mysql.py` & `onetl-0.7.1/onetl/connection/db_connection/mysql.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/db_connection/oracle.py` & `onetl-0.7.1/onetl/connection/db_connection/oracle.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/db_connection/postgres.py` & `onetl-0.7.1/onetl/connection/db_connection/postgres.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/db_connection/teradata.py` & `onetl-0.7.1/onetl/connection/db_connection/teradata.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/file_connection/file_connection.py` & `onetl-0.7.1/onetl/connection/file_connection/file_connection.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/file_connection/ftp.py` & `onetl-0.7.1/onetl/connection/file_connection/ftp.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/file_connection/ftps.py` & `onetl-0.7.1/onetl/connection/file_connection/ftps.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/file_connection/hdfs.py` & `onetl-0.7.1/onetl/connection/file_connection/hdfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -484,15 +484,15 @@
             except (ImportError, NameError) as e:
                 raise ImportError(
                     textwrap.dedent(
                         """
                         Cannot import module "hdfs.ext.kerberos".
 
                         Since onETL v0.7.0 you should install package as follows:
-                            pip install onetl[hdfs, kerberos]
+                            pip install onetl[hdfs,kerberos]
 
                         or
                             pip install onetl[all]
 
                         You should also have Kerberos libraries installed to OS,
                         specifically ``kinit`` executable.
                         """,
```

### Comparing `onetl-0.7.0/onetl/connection/file_connection/s3.py` & `onetl-0.7.1/onetl/connection/file_connection/s3.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/file_connection/sftp.py` & `onetl-0.7.1/onetl/connection/file_connection/sftp.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/file_connection/webdav.py` & `onetl-0.7.1/onetl/connection/file_connection/webdav.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/connection/kerberos_helpers.py` & `onetl-0.7.1/onetl/connection/kerberos_helpers.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/core/__init__.py` & `onetl-0.7.1/onetl/core/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/core/db_reader/__init__.py` & `onetl-0.7.1/onetl/core/db_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/core/db_reader/db_reader.py` & `onetl-0.7.1/onetl/core/db_reader/db_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,15 +389,15 @@
 
         if df_schema is not None and hwm_column not in df_schema.fieldNames():
             raise ValueError(
                 "'df_schema' struct must contain column specified in 'hwm_column'. "
                 "Otherwise DBReader cannot determine HWM type for this column",
             )
 
-        values["hwm_column"] = Column(name=hwm_column)
+        values["hwm_column"] = Column(name=hwm_column)  # type: ignore
         values["hwm_expression"] = hwm_expression
 
         return values
 
     @root_validator(pre=True)  # noqa: WPS231
     def validate_columns(cls, values: dict) -> dict:
         connection: BaseDBConnection = values["connection"]
```

### Comparing `onetl-0.7.0/onetl/core/db_reader/strategy_helper.py` & `onetl-0.7.1/onetl/core/db_reader/strategy_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -198,27 +198,30 @@
         row = max_df.collect()[0]
         max_hwm_value = row["max_value"]
         log.info("|DBReader| Max value is: %r", max_hwm_value)
 
         self.strategy.update_hwm(max_hwm_value)
         return df
 
-    def get_boundaries(self) -> Tuple[Optional[Statement], Optional[Statement]]:
-        start_from: Optional[Statement] = None
-        end_at: Optional[Statement] = None
+    def get_boundaries(self) -> tuple[Statement | None, Statement | None]:
+        start_from: Statement | None = None
+        end_at: Statement | None = None
+        hwm: ColumnHWM | None = self.strategy.hwm  # type: ignore
 
-        # `self.strategy.hwm is not None` is need only to handle mypy warnings
-        if self.strategy.current_value is not None and self.strategy.hwm is not None:
+        if hwm is None:
+            return None, None
+
+        if self.strategy.current_value is not None:
             start_from = Statement(
-                expression=self.hwm_expression or self.strategy.hwm.name,
+                expression=self.hwm_expression or hwm.name,
                 operator=self.strategy.current_value_comparator,
                 value=self.strategy.current_value,
             )
 
-        if self.strategy.next_value is not None and self.strategy.hwm is not None:
+        if self.strategy.next_value is not None:
             end_at = Statement(
-                expression=self.hwm_expression or self.strategy.hwm.name,
+                expression=self.hwm_expression or hwm.name,
                 operator=self.strategy.next_value_comparator,
                 value=self.strategy.next_value,
             )
 
         return start_from, end_at
```

### Comparing `onetl-0.7.0/onetl/core/db_writer/__init__.py` & `onetl-0.7.1/onetl/core/db_writer/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/core/db_writer/db_writer.py` & `onetl-0.7.1/onetl/core/db_writer/db_writer.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/core/file_downloader/__init__.py` & `onetl-0.7.1/onetl/core/file_downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/core/file_downloader/download_result.py` & `onetl-0.7.1/onetl/core/file_downloader/download_result.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/core/file_downloader/file_downloader.py` & `onetl-0.7.1/onetl/core/file_downloader/file_downloader.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/core/file_filter/__init__.py` & `onetl-0.7.1/onetl/core/file_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/core/file_filter/file_filter.py` & `onetl-0.7.1/onetl/core/file_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/core/file_filter/file_hwm_filter.py` & `onetl-0.7.1/onetl/core/file_filter/file_hwm_filter.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/core/file_filter/match_all_filters.py` & `onetl-0.7.1/onetl/core/file_filter/match_all_filters.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/core/file_limit/__init__.py` & `onetl-0.7.1/onetl/core/file_limit/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/core/file_limit/file_limit.py` & `onetl-0.7.1/onetl/core/file_limit/file_limit.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/core/file_limit/limits_reached.py` & `onetl-0.7.1/onetl/core/file_limit/limits_reached.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/core/file_result/__init__.py` & `onetl-0.7.1/onetl/core/file_result/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/core/file_result/file_result.py` & `onetl-0.7.1/onetl/core/file_result/file_result.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/core/file_result/file_set.py` & `onetl-0.7.1/onetl/core/file_result/file_set.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/core/file_uploader/__init__.py` & `onetl-0.7.1/onetl/core/file_uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/core/file_uploader/file_uploader.py` & `onetl-0.7.1/onetl/core/file_uploader/file_uploader.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/core/file_uploader/upload_result.py` & `onetl-0.7.1/onetl/core/file_uploader/upload_result.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/exception.py` & `onetl-0.7.1/onetl/exception.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/hooks/hook.py` & `onetl-0.7.1/onetl/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/hooks/hook_collection.py` & `onetl-0.7.1/onetl/hooks/hook_collection.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/hooks/hooks_state.py` & `onetl-0.7.1/onetl/hooks/hooks_state.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/hooks/method_inheritance_stack.py` & `onetl-0.7.1/onetl/hooks/method_inheritance_stack.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/hooks/slot.py` & `onetl-0.7.1/onetl/hooks/slot.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/hooks/support_hooks.py` & `onetl-0.7.1/onetl/hooks/support_hooks.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/hwm/store/__init__.py` & `onetl-0.7.1/onetl/hwm/store/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/hwm/store/base_hwm_store.py` & `onetl-0.7.1/onetl/hwm/store/base_hwm_store.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/hwm/store/hwm_class_registry.py` & `onetl-0.7.1/onetl/hwm/store/hwm_class_registry.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/hwm/store/hwm_store_class_registry.py` & `onetl-0.7.1/onetl/hwm/store/hwm_store_class_registry.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/hwm/store/hwm_store_manager.py` & `onetl-0.7.1/onetl/hwm/store/hwm_store_manager.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/hwm/store/memory_hwm_store.py` & `onetl-0.7.1/onetl/hwm/store/memory_hwm_store.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/hwm/store/yaml_hwm_store.py` & `onetl-0.7.1/onetl/hwm/store/yaml_hwm_store.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/impl/__init__.py` & `onetl-0.7.1/onetl/impl/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/impl/base_model.py` & `onetl-0.7.1/onetl/impl/base_model.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/impl/failed_local_file.py` & `onetl-0.7.1/onetl/impl/failed_local_file.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/impl/file_write_mode.py` & `onetl-0.7.1/onetl/impl/file_write_mode.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/impl/frozen_model.py` & `onetl-0.7.1/onetl/impl/frozen_model.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/impl/generic_options.py` & `onetl-0.7.1/onetl/impl/generic_options.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/impl/local_path.py` & `onetl-0.7.1/onetl/impl/local_path.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/impl/path_container.py` & `onetl-0.7.1/onetl/impl/path_container.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/impl/path_repr.py` & `onetl-0.7.1/onetl/impl/path_repr.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/impl/remote_directory.py` & `onetl-0.7.1/onetl/impl/remote_directory.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/impl/remote_file.py` & `onetl-0.7.1/onetl/impl/remote_file.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/impl/remote_path.py` & `onetl-0.7.1/onetl/impl/remote_path.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/impl/remote_path_stat.py` & `onetl-0.7.1/onetl/impl/remote_path_stat.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/log.py` & `onetl-0.7.1/onetl/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 log = logging.getLogger(__name__)
 onetl_log = logging.getLogger("onetl")
 root_log = logging.getLogger()
 
 HALF_SCREEN_SIZE = 45
 BASE_LOG_INDENT = 8
-LOG_FORMAT = "%(asctime)s [%(levelname:8s)s] %(message)s"
+LOG_FORMAT = "%(asctime)s [%(levelname)-8s] %(message)s"
 CLIENT_MODULES = {"hdfs", "paramiko", "ftputil", "smbclient"}
 
 DISABLED = 9999  # CRITICAL is 50, we need even higher to disable all logs
 logging.addLevelName(DISABLED, "DISABLED")
 
 NOTICE = 5  # DEBUG is 10, we need lower value for less verbose logs even on debug level
 logging.addLevelName(NOTICE, "NOTICE")
```

### Comparing `onetl-0.7.0/onetl/plugins/import_plugins.py` & `onetl-0.7.1/onetl/plugins/import_plugins.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/strategy/__init__.py` & `onetl-0.7.1/onetl/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/strategy/base_strategy.py` & `onetl-0.7.1/onetl/strategy/base_strategy.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/strategy/batch_hwm_strategy.py` & `onetl-0.7.1/onetl/strategy/batch_hwm_strategy.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/strategy/hwm_store/__init__.py` & `onetl-0.7.1/onetl/strategy/hwm_store/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/strategy/hwm_strategy.py` & `onetl-0.7.1/onetl/strategy/hwm_strategy.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/strategy/incremental_strategy.py` & `onetl-0.7.1/onetl/strategy/incremental_strategy.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/strategy/snapshot_strategy.py` & `onetl-0.7.1/onetl/strategy/snapshot_strategy.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/strategy/strategy_manager.py` & `onetl-0.7.1/onetl/strategy/strategy_manager.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl/version.py` & `onetl-0.7.1/onetl/version.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/onetl.egg-info/PKG-INFO` & `onetl-0.7.1/onetl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: onetl
-Version: 0.7.0
+Version: 0.7.1
 Summary: One ETL tool to rule them all
 Home-page: https://github.com/MobileTeleSystems/onetl
 Author: DataOps.ETL
 Author-email: onetools@mts.ru
 License: Apache License 2.0
-Project-URL: Documentation, https://onetl.readthedocs.io/en/stable/
+Project-URL: Documentation, https://onetl.readthedocs.io/
 Project-URL: Source, https://github.com/MobileTeleSystems/onetl
 Project-URL: CI/CD, https://github.com/MobileTeleSystems/onetl/actions
 Project-URL: Tracker, https://github.com/MobileTeleSystems/onetl/issues
 Keywords: Spark,ETL,JDBC,HWM
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pydantic :: 1
@@ -48,23 +48,23 @@
 onETL
 =====
 
 |Repo Status| |PyPI| |PyPI License| |PyPI Python Version|
 |Documentation| |Build Status| |Coverage|
 
 .. |Repo Status| image:: https://www.repostatus.org/badges/latest/active.svg
-    :target: https://www.repostatus.org/#active
+    :target: https://github.com/MobileTeleSystems/onetl
 .. |PyPI| image:: https://img.shields.io/pypi/v/onetl
     :target: https://pypi.org/project/onetl/
 .. |PyPI License| image:: https://img.shields.io/pypi/l/onetl.svg
     :target: https://github.com/MobileTeleSystems/onetl/blob/develop/LICENSE.txt
 .. |PyPI Python Version| image:: https://img.shields.io/pypi/pyversions/onetl.svg
     :target: https://badge.fury.io/py/onetl
 .. |Documentation| image:: https://readthedocs.org/projects/onetl/badge/?version=stable
-    :target: https://onetl.readthedocs.io/en/stable/
+    :target: https://onetl.readthedocs.io/
 .. |Build Status| image:: https://github.com/MobileTeleSystems/onetl/workflows/Tests/badge.svg
     :target: https://github.com/MobileTeleSystems/onetl/actions
 .. |Coverage| image:: https://codecov.io/gh/MobileTeleSystems/onetl/branch/develop/graph/badge.svg?token=RIO8URKNZJ
     :target: https://codecov.io/gh/MobileTeleSystems/onetl
 
 |Logo|
 
@@ -92,27 +92,27 @@
 
 Supported storages
 ------------------
 
 +------------+------------+----------------------------------------------------------------------------------------------------------+
 | Type       | Storage    | Powered by                                                                                               |
 +============+============+==========================================================================================================+
-| Database   | Clickhouse | Apache Spark `JDBC Data Source <https://spark.apache.org/docs/2.4.8/sql-data-sources-jdbc.html>`_        |
+| Database   | Clickhouse | Apache Spark `JDBC Data Source <https://spark.apache.org/docs/3.4.0/sql-data-sources-jdbc.html>`_        |
 +            +------------+                                                                                                          +
 |            | MSSQL      |                                                                                                          |
 +            +------------+                                                                                                          +
 |            | MySQL      |                                                                                                          |
 +            +------------+                                                                                                          +
 |            | Postgres   |                                                                                                          |
 +            +------------+                                                                                                          +
 |            | Oracle     |                                                                                                          |
 +            +------------+                                                                                                          +
 |            | Teradata   |                                                                                                          |
 +            +------------+----------------------------------------------------------------------------------------------------------+
-|            | Hive       | Apache Spark `Hive integration <https://spark.apache.org/docs/2.4.8/sql-data-sources-hive-tables.html>`_ |
+|            | Hive       | Apache Spark `Hive integration <https://spark.apache.org/docs/3.4.0/sql-data-sources-hive-tables.html>`_ |
 +            +------------+----------------------------------------------------------------------------------------------------------+
 |            | Greenplum  | Pivotal `Greenplum Spark connector <https://network.tanzu.vmware.com/products/vmware-tanzu-greenplum>`_  |
 +            +------------+----------------------------------------------------------------------------------------------------------+
 |            | MongoDB    | `MongoDB Spark connector <https://www.mongodb.com/docs/spark-connector/current>`_                        |
 +------------+------------+----------------------------------------------------------------------------------------------------------+
 | File       | HDFS       | `HDFS Python client <https://pypi.org/project/hdfs/>`_                                                   |
 +            +------------+----------------------------------------------------------------------------------------------------------+
@@ -129,15 +129,15 @@
 
 
 .. documentation
 
 Documentation
 -------------
 
-See https://onetl.readthedocs.io/en/stable/
+See https://onetl.readthedocs.io/
 
 .. contribution
 
 Contribution guide
 -------------------
 
 See `<CONTRIBUTING.rst>`__
@@ -238,15 +238,15 @@
 All file connection classes (``FTP``,  ``SFTP``, ``HDFS`` and so on) requires specific Python clients to be installed.
 
 Each client can be installed explicitly by passing connector name (in lowercase) to ``extras``:
 
 .. code:: bash
 
     pip install onetl[ftp]  # specific connector
-    pip install onetl[ftp, ftps, sftp, hdfs, s3, webdav]  # multiple connectors
+    pip install onetl[ftp,ftps,sftp,hdfs,s3,webdav]  # multiple connectors
 
 To install all file connectors at once you can pass ``files`` to ``extras``:
 
 .. code:: bash
 
     pip install onetl[files]
 
@@ -297,15 +297,15 @@
 To install all connectors and dependencies, you can pass ``all`` into ``extras``:
 
 .. code:: bash
 
     pip install onetl[all]
 
     # this is just the same as
-    pip install onetl[spark, files, kerberos]
+    pip install onetl[spark,files,kerberos]
 
 .. warning::
 
     This method consumes a lot of disk space, and requires for Java & Kerberos libraries to be installed into your OS.
 
 .. develops
```

### Comparing `onetl-0.7.0/onetl.egg-info/SOURCES.txt` & `onetl-0.7.1/onetl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/setup.cfg` & `onetl-0.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `onetl-0.7.0/setup.py` & `onetl-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Java Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: System :: Distributed Computing",
         "Typing :: Typed",
     ],
     project_urls={
-        "Documentation": "https://onetl.readthedocs.io/en/stable/",
+        "Documentation": "https://onetl.readthedocs.io/",
         "Source": "https://github.com/MobileTeleSystems/onetl",
         "CI/CD": "https://github.com/MobileTeleSystems/onetl/actions",
         "Tracker": "https://github.com/MobileTeleSystems/onetl/issues",
     },
     keywords=["Spark", "ETL", "JDBC", "HWM"],
     packages=find_packages(exclude=["docs", "docs.*", "tests", "tests.*"]),
     python_requires=">=3.7",
```

