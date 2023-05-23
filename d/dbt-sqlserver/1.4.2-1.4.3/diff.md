# Comparing `tmp/dbt-sqlserver-1.4.2.tar.gz` & `tmp/dbt-sqlserver-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-sqlserver-1.4.2.tar", last modified: Mon May 22 20:32:32 2023, max compression
+gzip compressed data, was "dbt-sqlserver-1.4.3.tar", last modified: Tue May 23 02:01:21 2023, max compression
```

## Comparing `dbt-sqlserver-1.4.2.tar` & `dbt-sqlserver-1.4.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.320621 dbt-sqlserver-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-22 20:32:32.320621 dbt-sqlserver-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.312620 dbt-sqlserver-1.4.2/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.312620 dbt-sqlserver-1.4.2/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/sql_server_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/sql_server_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/sql_server_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/sql_server_connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/sql_server_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/indexes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/incremental/incremental_strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/incremental/merge.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/table/create_table_as.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/view/create_view_as.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/seeds/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/snapshots/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/tests/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/tests/test.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.320621 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.320621 dbt-sqlserver-1.4.2/dbt_sqlserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-22 20:32:32.000000 dbt-sqlserver-1.4.2/dbt_sqlserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-22 20:32:32.000000 dbt-sqlserver-1.4.2/dbt_sqlserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:32:32.000000 dbt-sqlserver-1.4.2/dbt_sqlserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 20:32:32.000000 dbt-sqlserver-1.4.2/dbt_sqlserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-22 20:32:32.000000 dbt-sqlserver-1.4.2/dbt_sqlserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 20:32:32.320621 dbt-sqlserver-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:01:21.980053 dbt-sqlserver-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-23 02:01:21.976053 dbt-sqlserver-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:01:21.960053 dbt-sqlserver-1.4.3/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:01:21.960053 dbt-sqlserver-1.4.3/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:01:21.968053 dbt-sqlserver-1.4.3/dbt/adapters/sqlserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/adapters/sqlserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/adapters/sqlserver/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/adapters/sqlserver/sql_server_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/adapters/sqlserver/sql_server_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/adapters/sqlserver/sql_server_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/adapters/sqlserver/sql_server_connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/adapters/sqlserver/sql_server_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:01:21.960053 dbt-sqlserver-1.4.3/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:01:21.968053 dbt-sqlserver-1.4.3/dbt/include/sqlserver/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:01:21.964053 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:01:21.968053 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/adapters/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:01:21.964053 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:01:21.960053 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:01:21.968053 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/models/incremental/incremental_strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/models/incremental/merge.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:01:21.968053 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/models/table/create_table_as.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:01:21.972053 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/models/view/create_view_as.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:01:21.972053 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:01:21.972053 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/snapshots/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:01:21.972053 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/tests/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/tests/test.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:01:21.976053 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/utils/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:01:21.976053 dbt-sqlserver-1.4.3/dbt_sqlserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-23 02:01:21.000000 dbt-sqlserver-1.4.3/dbt_sqlserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-23 02:01:21.000000 dbt-sqlserver-1.4.3/dbt_sqlserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 02:01:21.000000 dbt-sqlserver-1.4.3/dbt_sqlserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-23 02:01:21.000000 dbt-sqlserver-1.4.3/dbt_sqlserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-23 02:01:21.000000 dbt-sqlserver-1.4.3/dbt_sqlserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 02:01:21.980053 dbt-sqlserver-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-23 02:00:45.000000 dbt-sqlserver-1.4.3/setup.py
```

### Comparing `dbt-sqlserver-1.4.2/LICENSE` & `dbt-sqlserver-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.2/PKG-INFO` & `dbt-sqlserver-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-sqlserver
-Version: 1.4.2
+Version: 1.4.3
 Summary: A Microsoft SQL Server adapter plugin for dbt
 Home-page: https://github.com/dbt-msft/dbt-sqlserver
 Author: Mikael Ene, Anders Swanson, Sam Debruyn, Cor Zuurmond
 License: MIT
 Project-URL: Setup & configuration, https://docs.getdbt.com/reference/warehouse-profiles/mssql-profile
 Project-URL: Documentation & usage, https://docs.getdbt.com/reference/resource-configs/mssql-configs
 Project-URL: Changelog, https://github.com/dbt-msft/dbt-sqlserver/blob/master/CHANGELOG.md
```

### Comparing `dbt-sqlserver-1.4.2/README.md` & `dbt-sqlserver-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/__init__.py` & `dbt-sqlserver-1.4.3/dbt/adapters/sqlserver/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/sql_server_adapter.py` & `dbt-sqlserver-1.4.3/dbt/adapters/sqlserver/sql_server_adapter.py`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/sql_server_column.py` & `dbt-sqlserver-1.4.3/dbt/adapters/sqlserver/sql_server_column.py`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/sql_server_connection_manager.py` & `dbt-sqlserver-1.4.3/dbt/adapters/sqlserver/sql_server_connection_manager.py`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/sql_server_credentials.py` & `dbt-sqlserver-1.4.3/dbt/adapters/sqlserver/sql_server_credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/apply_grants.sql` & `dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/columns.sql` & `dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/indexes.sql` & `dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/metadata.sql` & `dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/relation.sql` & `dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/adapters/relation.sql`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,27 @@
     {{ sqlserver__drop_relation_script(relation) }}
   {%- endcall %}
 {% endmacro %}
 
 {% macro sqlserver__drop_relation_script(relation) -%}
     {% call statement('find_references', fetch_result=true) %}
         USE [{{ relation.database }}];
-        SELECT referencing_schema_name, referencing_entity_name
-        FROM sys.dm_sql_referencing_entities ('{{ relation.include(database=false) }}', 'object')
+        select
+            sch.name as schema_name,
+            obj.name as view_name
+        from sys.sql_expression_dependencies refs
+        inner join sys.objects obj
+        on refs.referencing_id = obj.object_id
+        inner join sys.schemas sch
+        on obj.schema_id = sch.schema_id
+        where refs.referenced_database_name = '{{ relation.database }}'
+        and refs.referenced_schema_name = '{{ relation.schema }}'
+        and refs.referenced_entity_name = '{{ relation.identifier }}'
+        and refs.referencing_class = 1
+        and obj.type = 'V'
     {% endcall %}
     {% set references = load_result('find_references')['data'] %}
     {% for reference in references -%}
         -- dropping referenced view {{ reference[0] }}.{{ reference[1] }}
         {{ sqlserver__drop_relation_script(relation.incorporate(
             type="view",
             path={"schema": reference[0], "identifier": reference[1]})) }}
```

### Comparing `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/schema.sql` & `dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/incremental/merge.sql` & `dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/table/create_table_as.sql` & `dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/view/create_view_as.sql` & `dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/models/view/create_view_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/seeds/helpers.sql` & `dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/snapshots/snapshot.sql` & `dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/tests/test.sql` & `dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/materializations/tests/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/split_part.sql` & `dbt-sqlserver-1.4.3/dbt/include/sqlserver/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.2/dbt_sqlserver.egg-info/PKG-INFO` & `dbt-sqlserver-1.4.3/dbt_sqlserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-sqlserver
-Version: 1.4.2
+Version: 1.4.3
 Summary: A Microsoft SQL Server adapter plugin for dbt
 Home-page: https://github.com/dbt-msft/dbt-sqlserver
 Author: Mikael Ene, Anders Swanson, Sam Debruyn, Cor Zuurmond
 License: MIT
 Project-URL: Setup & configuration, https://docs.getdbt.com/reference/warehouse-profiles/mssql-profile
 Project-URL: Documentation & usage, https://docs.getdbt.com/reference/resource-configs/mssql-configs
 Project-URL: Changelog, https://github.com/dbt-msft/dbt-sqlserver/blob/master/CHANGELOG.md
```

### Comparing `dbt-sqlserver-1.4.2/dbt_sqlserver.egg-info/SOURCES.txt` & `dbt-sqlserver-1.4.3/dbt_sqlserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.2/setup.py` & `dbt-sqlserver-1.4.3/setup.py`

 * *Files identical despite different names*

