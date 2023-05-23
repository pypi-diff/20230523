# Comparing `tmp/MindsDB-23.5.3.2.tar.gz` & `tmp/MindsDB-23.5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MindsDB-23.5.3.2.tar", last modified: Tue May 16 12:04:09 2023, max compression
+gzip compressed data, was "dist/MindsDB-23.5.4.1.tar", last modified: Tue May 23 09:12:35 2023, max compression
```

## Comparing `MindsDB-23.5.3.2.tar` & `MindsDB-23.5.4.1.tar`

### file list

```diff
@@ -1,1298 +1,1331 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-16 12:03:54.000000 MindsDB-23.5.3.2/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/MindsDB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23210 2023-05-16 12:04:08.000000 MindsDB-23.5.3.2/MindsDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    61801 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/MindsDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:04:08.000000 MindsDB-23.5.3.2/MindsDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-16 12:04:08.000000 MindsDB-23.5.3.2/MindsDB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 12:04:08.000000 MindsDB-23.5.3.2/MindsDB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23210 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21164 2023-05-16 12:03:54.000000 MindsDB-23.5.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/common/check_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/gunicorn_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/configs/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/configs/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/configs/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/configs/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/configs/default.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/configs/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/configs/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/configs/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/configs/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/configs/streams.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/configs/tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/configs/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/configs/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/namespaces/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/http/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/classes/query_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/classes/responder.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/classes/responder_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/classes/scram.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/classes/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/add_shard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/buildinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/coll_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/company_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/connection_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/count.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/db_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/end_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/find.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/get_cmd_line_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/get_free_monitoring_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/get_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/getlog.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/host_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/insert.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/is_master.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/is_master_lower.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/list_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/list_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/list_indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/recv_chunk_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/replsetgetstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/sasl_continue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/sasl_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/update_range_deletions.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/responders/whatsmyuri.py
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/utilities/mongodb_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/utilities/mongodb_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mongo/utilities/mongodb_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    56525 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/datahub/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/datahub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/datahub/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/datahub/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/datahub/datahub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)    23115 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/executor/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/executor/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/executor/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    67024 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/external_libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/libs/constants/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35316 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/libs/constants/response_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    31908 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/utilities/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/utilities/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/mysql/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/nlp/nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/postgres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/executor/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/executor/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    40804 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py
--rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/api/postgres/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/access_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/access_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/access_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/access_handler/access_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    32145 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/access_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/access_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/access_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/access_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/airtable_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/airtable_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/airtable_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/airtable_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/airtable_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/airtable_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/altibase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/altibase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/altibase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   342129 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/altibase_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/altibase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/altibase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/aurora_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/aurora_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/aurora_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/aurora_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/aurora_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/aurora_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/autokeras_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/autokeras_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/autokeras_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/autokeras_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/autokeras_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/autosklearn_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/autosklearn_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/autosklearn_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/autosklearn_handler/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/autosklearn_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/bigquery_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/bigquery_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/bigquery_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/bigquery_handler/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/bigquery_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/binance_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/binance_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/binance_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/binance_handler/binance_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/binance_handler/binance_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/binance_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/binance_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/byom_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/byom_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/byom_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/byom_handler/byom_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cassandra_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cassandra_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cassandra_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   176707 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cassandra_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cassandra_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ckan_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ckan_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ckan_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ckan_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ckan_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ckan_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/clickhouse_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/clickhouse_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_spanner_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_sql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    37571 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_sql_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cockroach_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cockroach_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cockroach_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cockroach_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/confluence_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/confluence_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/confluence_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/confluence_handler/confluence_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    76194 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/confluence_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/confluence_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/couchbase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/couchbase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/couchbase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/couchbase_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/couchbase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/crate_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/crate_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/crate_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/crate_handler/crate_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/crate_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/crate_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/crate_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/d0lt_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/d0lt_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/d0lt_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85600 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/d0lt_handler/create-db.png
--rw-r--r--   0 runner    (1001) docker     (123)    98275 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/d0lt_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    98983 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/d0lt_handler/predict-target.png
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/d0lt_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databend_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databend_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databend_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databend_handler/databend_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databend_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databend_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databend_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/databricks/
--rw-r--r--   0 runner    (1001) docker     (123)    86110 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    58645 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    21694 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62078 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/datastax_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/datastax_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/datastax_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/datastax_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/datastax_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/datastax_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/db2_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/db2_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/db2_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/db2_handler/db2_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/db2_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/db2_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/db2_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/derby_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/derby_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/derby_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/derby_handler/derby_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/derby_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/derby_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/derby_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/dremio_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/dremio_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/dremio_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/dremio_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/dremio_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/dremio_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/druid_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/druid_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/druid_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/druid_handler/druid_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    29112 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/druid_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/druid_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/druid_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/duckdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/duckdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/duckdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19548 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/duckdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/duckdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/duckdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/dynamodb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    55623 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/dynamodb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/dynamodb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/dynamodb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/edgelessdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/edgelessdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/elasticsearch_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/elasticsearch_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/elasticsearch_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/empress_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/empress_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/empress_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/empress_handler/empress_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/empress_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/empress_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/empress_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/eventstoredb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/eventstoredb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/file_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/file_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/file_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/file_handler/file_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/firebird_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/firebird_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/firebird_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    54033 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/firebird_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/firebird_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/firebird_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/github_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/github_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/github_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/github_handler/github_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/github_handler/github_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/github_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/github_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/gitlab_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/gitlab_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/gitlab_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/gitlab_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/gitlab_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_books_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_books_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_books_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_books_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_books_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_books_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_books_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_calendar_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_calendar_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_calendar_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10399 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_calendar_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_calendar_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_calendar_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_calendar_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_content_shopping_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_content_shopping_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    34337 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_content_shopping_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_content_shopping_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_content_shopping_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_fit_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_fit_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_fit_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    21355 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_fit_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_fit_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_search_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_search_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_search_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_search_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_search_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_search_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_search_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hackernews_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hackernews_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hackernews_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hackernews_handler/hn_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hackernews_handler/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hana_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hana_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hana_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hana_handler/hana_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hana_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hana_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hive_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hive_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hive_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hive_handler/hive_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hive_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hive_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hive_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hsqldb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hsqldb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/huggingface_api_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/huggingface_api_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/huggingface_api_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/huggingface_api_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/huggingface_api_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/huggingface_api_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/huggingface_api_handler/tests/test_huggingface_api_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/huggingface_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/huggingface_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/huggingface_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/huggingface_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ignite_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ignite_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ignite_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45779 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ignite_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ignite_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ignite_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/impala_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/impala_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/impala_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/impala_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/impala_handler/impala_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/impala_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/impala_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/influxdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/influxdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/influxdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63375 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/influxdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/influxdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/informix_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/informix_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/informix_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/informix_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/informix_handler/informix_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/informix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/informix_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ingres_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ingres_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ingres_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ingres_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ingres_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ingres_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/jira_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/jira_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/jira_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/jira_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/jira_handler/jira_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/jira_handler/jira_table.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/jira_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/langchain_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/langchain_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/langchain_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16667 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/langchain_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/langchain_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/lightwood_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/lightwood_handler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20556 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/lightwood_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/lightwood_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ludwig_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ludwig_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ludwig_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ludwig_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ludwig_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ludwig_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mariadb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)    88354 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mariadb_handler/1-create_db.png
--rw-r--r--   0 runner    (1001) docker     (123)   110633 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mariadb_handler/2-create_predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)   109269 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mariadb_handler/3-predict_target.png
--rw-r--r--   0 runner    (1001) docker     (123)    62778 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mariadb_handler/4-drop_db.png
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mariadb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mariadb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    99045 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mariadb_handler/create-db.png
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mariadb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    98530 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mariadb_handler/predict-db.png
--rw-r--r--   0 runner    (1001) docker     (123)   100718 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mariadb_handler/predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/materialize_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/materialize_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/materialize_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47935 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/materialize_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/materialize_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/materialize_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/matrixone_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/matrixone_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/matrixone_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57976 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/matrixone_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/matrixone_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/maxdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/maxdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/maxdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/maxdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/maxdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/maxdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/maxdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/merlion_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/merlion_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/merlion_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/merlion_handler/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/merlion_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/merlion_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mlflow_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mlflow_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mlflow_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mlflow_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   544421 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/create-database.png
--rw-r--r--   0 runner    (1001) docker     (123)   423554 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)    64685 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)   445044 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mongodb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mongodb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mongodb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mongodb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mongodb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mssql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mssql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mssql_handler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14543 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mssql_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mssql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mssql_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mysql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mysql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mysql_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mysql_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/mysql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/neuralforecast_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/neuralforecast_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/newsapi_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/newsapi_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/newsapi_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/newsapi_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/newsapi_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/newsapi_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/newsapi_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/nuo_jdbc_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    95071 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/oceanbase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37289 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/oceanbase_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/oceanbase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/openai_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/openai_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/openai_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/openai_handler/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28123 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/openai_handler/openai_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/openai_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/openai_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/opengauss_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/opengauss_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/opengauss_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/opengauss_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/oracle_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/oracle_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/oracle_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/oracle_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/oracle_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/oracle_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/orioledb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/orioledb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/orioledb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/orioledb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/orioledb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/phoenix_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/phoenix_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/phoenix_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/phoenix_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/phoenix_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/pinot_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/pinot_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/pinot_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/pinot_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/pinot_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/pinot_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/plaid_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/plaid_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/plaid_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/plaid_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/plaid_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/plaid_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/planetscale_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/planetscale_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/planetscale_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    97032 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/planetscale_handler/create-db.png
--rw-r--r--   0 runner    (1001) docker     (123)    98334 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)    63619 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/planetscale_handler/drop-db.png
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/planetscale_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   112840 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/planetscale_handler/predict-target.png
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/postgres_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/postgres_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/postgres_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/postgres_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/postgres_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/questdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/questdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/questdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/questdb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/questdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/questdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/quickbooks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/quickbooks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/quickbooks_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/quickbooks_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/quickbooks_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ray_serve_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ray_serve_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ray_serve_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ray_serve_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/ray_serve_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/reddit_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/reddit_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/reddit_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/reddit_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/reddit_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/redshift_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/redshift_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/redshift_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/redshift_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/redshift_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/redshift_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/rockset_handler/
--rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/rockset_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/rockset_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/rockset_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   194064 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/rockset_handler/tests/test.png
--rw-r--r--   0 runner    (1001) docker     (123)   108141 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/s3_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/s3_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/s3_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/s3_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/s3_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/s3_handler/s3_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/s3_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/scylla_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/scylla_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/scylla_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/scylla_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/scylla_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/scylla_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sendinblue_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sendinblue_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sendinblue_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sendinblue_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sendinblue_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sheets_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sheets_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sheets_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27211 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sheets_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sheets_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sheets_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/singlestore_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/singlestore_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/singlestore_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/singlestore_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/slack_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/slack_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/slack_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/slack_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/slack_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13091 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/slack_handler/slack_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/slack_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/slack_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/snowflake_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/snowflake_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/snowflake_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/snowflake_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/solr_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/solr_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/solr_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/solr_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/solr_handler/solr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/solr_handler/solr_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/solr_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlany_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlany_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlany_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlany_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   521282 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/db_connection.png
--rw-r--r--   0 runner    (1001) docker     (123)   369371 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/error.png
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)   479779 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/model_drop.png
--rw-r--r--   0 runner    (1001) docker     (123)   477242 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png
--rw-r--r--   0 runner    (1001) docker     (123)   552154 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqreamdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqreamdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqreamdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/starrocks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/starrocks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/starrocks_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/starrocks_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/starrocks_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/statsforecast_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/statsforecast_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/strava_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/strava_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/strava_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/strava_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/strava_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/strava_handler/strava_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/strava_handler/strava_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/supabase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/supabase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/supabase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/supabase_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/supabase_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/supabase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/surrealdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/surrealdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/surrealdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/surrealdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/surrealdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/surrealdb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tdengine_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tdengine_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tdengine_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tdengine_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tdengine_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/teradata_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/teradata_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/teradata_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/teradata_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/teradata_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tidb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tidb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tidb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tidb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tidb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/timescaledb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/timescaledb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tpot_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tpot_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tpot_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tpot_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tpot_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/trino_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/trino_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/trino_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/trino_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/trino_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/trino_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/trino_handler/trino_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/twitter_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/twitter_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/twitter_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/twitter_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/twitter_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/vertica_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/vertica_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/vertica_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/vertica_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/vertica_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/vertica_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/vitess_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/vitess_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/vitess_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/vitess_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/vitess_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/vitess_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/youtube_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/youtube_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/youtube_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/youtube_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/youtube_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/yugabyte_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/yugabyte_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers_client/db_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers_client/db_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers_client/ml_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers_client/ml_grpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers_wrapper/db_handler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/libs/api_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/libs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/libs/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/libs/handler_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17834 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/libs/ml_exec_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/libs/ml_handler_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/libs/net_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/libs/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/libs/storage_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/integrations/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/utilities/date_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/utilities/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/utilities/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/utilities/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/utilities/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/utilities/time_series_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/integrations/utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/interfaces/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    22951 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/database/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/database/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/database/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/interfaces/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/file/file_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/interfaces/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/jobs/jobs_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/jobs/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/interfaces/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/model/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22438 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/model/model_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/interfaces/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/storage/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/storage/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/storage/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/storage/model_fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/interfaces/stream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/stream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/interfaces/stream/base/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/stream/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/stream/base/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/interfaces/stream/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/stream/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/stream/kafka/kafkadb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/interfaces/stream/redis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/stream/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/stream/redis/redisdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/interfaces/stream/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/microservices_grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/microservices_grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/microservices_grpc/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/microservices_grpc/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/microservices_grpc/db/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/microservices_grpc/db/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/microservices_grpc/db/db_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/microservices_grpc/db/db_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/microservices_grpc/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/microservices_grpc/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/microservices_grpc/executor/executor_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/microservices_grpc/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/microservices_grpc/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/microservices_grpc/ml/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/microservices_grpc/ml/ml_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/migrations/versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/utilities/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/utilities/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/utilities/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/utilities/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/utilities/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/utilities/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/utilities/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/utilities/hooks/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/utilities/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/utilities/log_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/mindsdb/utilities/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/utilities/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/utilities/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/utilities/ps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/utilities/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/mindsdb/utilities/wizards.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 12:04:09.000000 MindsDB-23.5.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-16 12:03:55.000000 MindsDB-23.5.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/MindsDB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23039 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/MindsDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    63528 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/MindsDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/MindsDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/MindsDB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/MindsDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23039 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20993 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/common/check_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/gunicorn_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/classes/query_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/classes/responder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/classes/responder_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/classes/scram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/classes/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/add_shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/buildinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/coll_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/company_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/connection_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/db_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/end_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/get_cmd_line_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/get_free_monitoring_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/get_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/getlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/host_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/is_master.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/is_master_lower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/list_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/list_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/list_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/recv_chunk_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/replsetgetstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/sasl_continue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/sasl_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/update_range_deletions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/whatsmyuri.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/utilities/mongodb_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/utilities/mongodb_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/utilities/mongodb_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56525 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/datahub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67108 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/external_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/libs/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35316 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/libs/constants/response_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31908 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/nlp/nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/executor/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40804 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/access_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32145 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   342129 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autokeras_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autokeras_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autokeras_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autokeras_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autokeras_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/binance_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/binance_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/binance_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/binance_handler/binance_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/binance_handler/binance_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/binance_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/binance_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/byom_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/byom_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/byom_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/byom_handler/byom_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   176707 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37571 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cockroach_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cockroach_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cockroach_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cockroach_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/confluence_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76194 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/crate_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85600 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/create-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)    98275 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    98983 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/predict-target.png
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/databend_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)    86110 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    58645 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    21694 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62078 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/db2_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/derby_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/druid_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29112 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19548 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55623 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/empress_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/eventstoredb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/eventstoredb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/file_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/file_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/file_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/file_handler/file_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54033 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/frappe_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/frappe_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/frappe_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/frappe_handler/frappe_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/frappe_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/frappe_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/github_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/github_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/github_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/github_handler/github_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/github_handler/github_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/github_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/github_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gitlab_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gitlab_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gitlab_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gitlab_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gitlab_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gmail_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gmail_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gmail_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gmail_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gmail_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gmail_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gmail_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10399 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34337 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_fit_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_fit_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_fit_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21355 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_fit_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_fit_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hackernews_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hackernews_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hackernews_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hackernews_handler/hn_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hackernews_handler/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hana_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hana_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hana_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hana_handler/hana_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hana_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hana_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/hive_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hsqldb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hsqldb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/test_huggingface_api_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45779 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/impala_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63375 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/informix_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/jira_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/jira_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/langchain_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/langchain_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/langchain_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16667 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/langchain_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/langchain_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20556 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ludwig_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ludwig_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ludwig_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ludwig_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ludwig_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ludwig_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)    88354 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/1-create_db.png
+-rw-r--r--   0 runner    (1001) docker     (123)   110633 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/2-create_predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)   109269 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/3-predict_target.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62778 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/4-drop_db.png
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99045 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/create-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98530 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/predict-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)   100718 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47935 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57976 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/merlion_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/merlion_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/merlion_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/merlion_handler/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/merlion_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/merlion_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mlflow_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mlflow_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mlflow_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mlflow_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   544421 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/create-database.png
+-rw-r--r--   0 runner    (1001) docker     (123)   423554 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    64685 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   445044 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14543 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mysql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mysql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mysql_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mysql_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mysql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/neuralforecast_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/neuralforecast_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95071 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37289 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/openai_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/openai_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/openai_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/openai_handler/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28123 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/openai_handler/openai_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/openai_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/openai_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97032 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/create-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)    98334 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63619 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/drop-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112840 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/predict-target.png
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/postgres_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/postgres_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/postgres_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/postgres_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/postgres_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ray_serve_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ray_serve_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ray_serve_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ray_serve_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ray_serve_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/reddit_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/reddit_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/reddit_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/reddit_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/reddit_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rocket_chat_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rocket_chat_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rocket_chat_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rocket_chat_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rockset_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rockset_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rockset_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rockset_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   194064 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rockset_handler/tests/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)   108141 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/s3_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sendinblue_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sendinblue_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sendinblue_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sendinblue_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sendinblue_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27211 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/shopify_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/shopify_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/shopify_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26694 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/shopify_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/shopify_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/shopify_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/singlestore_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/singlestore_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/singlestore_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/singlestore_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13091 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/slack_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/snowflake_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/snowflake_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/snowflake_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/snowflake_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/solr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/solr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlany_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlany_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlany_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlany_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   521282 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/db_connection.png
+-rw-r--r--   0 runner    (1001) docker     (123)   369371 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   479779 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/model_drop.png
+-rw-r--r--   0 runner    (1001) docker     (123)   477242 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png
+-rw-r--r--   0 runner    (1001) docker     (123)   552154 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/statsforecast_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/statsforecast_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/strava_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/strava_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/teradata_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/teradata_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/teradata_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/teradata_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/teradata_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tpot_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tpot_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tpot_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tpot_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tpot_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/trino_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/twitter_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/twitter_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/twitter_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/twitter_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/twitter_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_client/db_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_client/db_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_client/ml_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_client/ml_grpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_wrapper/db_handler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/handler_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/ml_exec_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/ml_handler_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/net_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/storage_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/utilities/date_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/utilities/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/utilities/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/utilities/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/utilities/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/utilities/time_series_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/interfaces/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23057 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/database/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/database/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/database/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/interfaces/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/file/file_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/interfaces/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/jobs/jobs_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/jobs/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/interfaces/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/model/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22507 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/model/model_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/interfaces/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/storage/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/storage/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/storage/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/storage/model_fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/base/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/kafka/kafkadb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/redis/redisdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/db/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/db/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/db/db_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/db/db_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/executor/executor_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/ml/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/ml/ml_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/utilities/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/hooks/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/log_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/utilities/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/setup.py
```

### Comparing `MindsDB-23.5.3.2/MindsDB.egg-info/PKG-INFO` & `MindsDB-23.5.4.1/MindsDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MindsDB
-Version: 23.5.3.2
+Version: 23.5.4.1
 Summary: MindsDB server, provides server capabilities to mindsdb native python library
 Home-page: https://github.com/mindsdb/mindsdb
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb/
 Description: <h1 align="center">
@@ -133,16 +133,16 @@
         | <a href="https://docs.mindsdb.com/data-integrations/cockroachdb"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/ckan"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/clickhouse"><img src="https://img.shields.io/badge/Clickhouse-e6e600?style=for-the-badge&logo=clickhouse&logoColor=white" alt="Connect Clickhouse"></a> | <a href="https://docs.mindsdb.com/data-integrations/google-bigquery"><img src="https://img.shields.io/badge/Google Big Query-0466C8?logo=Big Query&logoColor=fff&style=for-the-badge" alt="Google Big Query Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/sqlite"><img src="https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=fff&style=for-the-badge" alt="SQLite Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/tidb#tidb-handler"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/data-integrations/cratedb"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href=" https://docs.mindsdb.com/data-integrations/timescaledb"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/d0lt"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/amazon-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/ibm-db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/yugabytedb"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
-        | <a href="https://docs.mindsdb.com/data-integrations/questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/apache-druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> |
-        | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/redis-%23DD0031.svg?&style=for-the-badge&logo=redis&logoColor=white" alt="Connect Redis"></a> | <a href="https://docs.mindsdb.com/data-integrations/vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/apache-druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href="https://docs.mindsdb.com/data-integrations/elasticsearch"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#scylla"><img src="https://img.shields.io/badge/ScyllaDB-53CADD?style=for-the-badge&logo=scylladbb&logoColor=white" alt="Connect ScyllaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#firebird"><img src="https://img.shields.io/badge/Firebird-F40D12?logo=Firebird&logoColor=fff&style=for-the-badge" alt="Firebird Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#singlestore"><img src="https://img.shields.io/badge/Singlestore-5f07b4?style=for-the-badge&logo=singlestore&logoColor=white" alt="Connect Singlestore"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#hive"><img src="https://img.shields.io/badge/Apache%20Hive-FDEE21?logo=apachehive&logoColor=000&style=for-the-badge" alt="Apache Hive Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/teradata"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
         | <a href=" https://docs.mindsdb.com/data-integrations/snowflake"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/trino"><img src="https://img.shields.io/badge/Trino-dd00a1?style=for-the-badge&logo=trino&logoColor=white" alt="Connect Trino"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#monetdb"><img src="https://img.shields.io/badge/Monetdb-0099E5?logo=Monetdb&logoColor=fff&style=for-the-badge" alt="Monetdb Badge"></a> |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MindsDB Version: 23.5.3.2 Summary: MindsDB server,
+Metadata-Version: 2.1 Name: MindsDB Version: 23.5.4.1 Summary: MindsDB server,
 provides server capabilities to mindsdb native python library Home-page: https:
 //github.com/mindsdb/mindsdb Author: MindsDB Inc Author-email:
 jorge@mindsdb.com License: GPL-3.0 Download-URL: https://pypi.org/project/
 mindsdb/ Description:
                                ****** [MindsDB]
                                      ******
       [ROSS_Index_-_Fastest_Growing_Open-Source_Startups_|_Runa_Capital]
@@ -92,23 +92,23 @@
 Badge] | [Pinot_Badge] | | [Connect_Cassandra] | [DataStax_Badge] | [Amazon_S3
 Badge] | | [Connect_CockroachDB] | [ckan_Badge] | [Supabase_Badge] | | [Connect
 Clickhouse] | [Google_Big_Query_Badge] | [SQLite_Badge] | | [Connect_MariaDB] |
 [Couchbase_Badge] | [TiDB_Badge] | | [Connect_SQL_Server] | [CrateDB_Badge] |
 [Timescale_Badge] | | [Connect_MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB
 Badge] | | [Connect_PostgreSQL] | [IBMDB2_Badge] | [openGauss_Badge] | |
 [Connect_MySQL] | [Databricks_Badge] | [YugabyteDB_Badge] | [Connect_QuestDB] |
-[Apache_Druid_Badge] | [StarRocks_Badge] | | [Connect_Redis] | [Vertica_Badge]
-| [DuckDB_Badge] | | [Connect_SAP_HANA] | [Elastic_Badge] | [Cloud_Spanner
-Badge] | | [Connect_ScyllaDB] | [Firebird_Badge] | | [Connect_Singlestore] |
-[Apache_Hive_Badge] | | [Connect_Teradata] | [Matrixone_Badge] | | [Connect
-Snowflake] | [Informix_Badge] | | [Connect_Trino] | [Monetdb_Badge] | [:
-question: :wave: Missing integration?](https://github.com/mindsdb/mindsdb/
-issues/new?assignees=&labels=&template=feature-mindsdb-request.yaml) ##
-Documentation You can find the complete documentation of MindsDB at
-[docs.mindsdb.com](https://
+[Apache_Druid_Badge] | | [StarRocks_Badge] | [Vertica_Badge] | [DuckDB_Badge] |
+| [Connect_SAP_HANA] | [Elastic_Badge] | [Cloud_Spanner_Badge] | | [Connect
+ScyllaDB] | [Firebird_Badge] | | [Connect_Singlestore] | [Apache_Hive_Badge] |
+| [Connect_Teradata] | [Matrixone_Badge] | | [Connect_Snowflake] | [Informix
+Badge] | | [Connect_Trino] | [Monetdb_Badge] | [:question: :wave: Missing
+integration?](https://github.com/mindsdb/mindsdb/issues/
+new?assignees=&labels=&template=feature-mindsdb-request.yaml) ## Documentation
+You can find the complete documentation of MindsDB at [docs.mindsdb.com](https:
+//
 docs.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
 ## Support If you found a bug, please submit an [issue on GitHub](https://
 github.com/mindsdb/mindsdb/issues/new/choose). To get community support, you
 can: * Post at MindsDB [Slack community](https://mindsdb.com/joincommunity). *
 Ask for help at our [GitHub Discussions](https://github.com/mindsdb/mindsdb/
 discussions). * Ask a question at [Stackoverflow](https://stackoverflow.com/
 questions/tagged/mindsdb) with a MindsDB tag. If you need commercial support,
```

### Comparing `MindsDB-23.5.3.2/MindsDB.egg-info/SOURCES.txt` & `MindsDB-23.5.4.1/MindsDB.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -402,26 +402,40 @@
 mindsdb/integrations/handlers/firebird_handler/__about__.py
 mindsdb/integrations/handlers/firebird_handler/__init__.py
 mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
 mindsdb/integrations/handlers/firebird_handler/icon.png
 mindsdb/integrations/handlers/firebird_handler/requirements.txt
 mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
 mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
+mindsdb/integrations/handlers/frappe_handler/__about__.py
+mindsdb/integrations/handlers/frappe_handler/__init__.py
+mindsdb/integrations/handlers/frappe_handler/frappe_client.py
+mindsdb/integrations/handlers/frappe_handler/frappe_handler.py
+mindsdb/integrations/handlers/frappe_handler/frappe_tables.py
+mindsdb/integrations/handlers/frappe_handler/icon.svg
+mindsdb/integrations/handlers/frappe_handler/requirements.txt
 mindsdb/integrations/handlers/github_handler/__about__.py
 mindsdb/integrations/handlers/github_handler/__init__.py
 mindsdb/integrations/handlers/github_handler/github_handler.py
 mindsdb/integrations/handlers/github_handler/github_tables.py
 mindsdb/integrations/handlers/github_handler/icon.svg
 mindsdb/integrations/handlers/github_handler/requirements.txt
 mindsdb/integrations/handlers/gitlab_handler/__about__.py
 mindsdb/integrations/handlers/gitlab_handler/__init__.py
 mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py
 mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py
 mindsdb/integrations/handlers/gitlab_handler/icon.svg
 mindsdb/integrations/handlers/gitlab_handler/requirements.txt
+mindsdb/integrations/handlers/gmail_handler/__about__.py
+mindsdb/integrations/handlers/gmail_handler/__init__.py
+mindsdb/integrations/handlers/gmail_handler/gmail_handler.py
+mindsdb/integrations/handlers/gmail_handler/icon.svg
+mindsdb/integrations/handlers/gmail_handler/requirements.txt
+mindsdb/integrations/handlers/gmail_handler/tests/__init__.py
+mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py
 mindsdb/integrations/handlers/google_books_handler/__about__.py
 mindsdb/integrations/handlers/google_books_handler/__init__.py
 mindsdb/integrations/handlers/google_books_handler/google_books_handler.py
 mindsdb/integrations/handlers/google_books_handler/google_books_tables.py
 mindsdb/integrations/handlers/google_books_handler/icon.svg
 mindsdb/integrations/handlers/google_books_handler/requirements.txt
 mindsdb/integrations/handlers/google_books_handler/tests/__init__.py
@@ -742,14 +756,21 @@
 mindsdb/integrations/handlers/redshift_handler/__about__.py
 mindsdb/integrations/handlers/redshift_handler/__init__.py
 mindsdb/integrations/handlers/redshift_handler/icon.png
 mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
 mindsdb/integrations/handlers/redshift_handler/requirements.txt
 mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
 mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
+mindsdb/integrations/handlers/rocket_chat_handler/__about__.py
+mindsdb/integrations/handlers/rocket_chat_handler/__init__.py
+mindsdb/integrations/handlers/rocket_chat_handler/icon.svg
+mindsdb/integrations/handlers/rocket_chat_handler/requirements.txt
+mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_client.py
+mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py
+mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py
 mindsdb/integrations/handlers/rockset_handler/icon.png
 mindsdb/integrations/handlers/rockset_handler/requirements.txt
 mindsdb/integrations/handlers/rockset_handler/tests/test.png
 mindsdb/integrations/handlers/rockset_handler/tests/test2.png
 mindsdb/integrations/handlers/s3_handler/__about__.py
 mindsdb/integrations/handlers/s3_handler/__init__.py
 mindsdb/integrations/handlers/s3_handler/icon.png
@@ -773,14 +794,21 @@
 mindsdb/integrations/handlers/sheets_handler/__about__.py
 mindsdb/integrations/handlers/sheets_handler/__init__.py
 mindsdb/integrations/handlers/sheets_handler/icon.png
 mindsdb/integrations/handlers/sheets_handler/requirements.txt
 mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
 mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
 mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
+mindsdb/integrations/handlers/shopify_handler/__about__.py
+mindsdb/integrations/handlers/shopify_handler/__init__.py
+mindsdb/integrations/handlers/shopify_handler/icon.png
+mindsdb/integrations/handlers/shopify_handler/requirements.txt
+mindsdb/integrations/handlers/shopify_handler/shopify_handler.py
+mindsdb/integrations/handlers/shopify_handler/shopify_tables.py
+mindsdb/integrations/handlers/shopify_handler/utils.py
 mindsdb/integrations/handlers/singlestore_handler/__about__.py
 mindsdb/integrations/handlers/singlestore_handler/__init__.py
 mindsdb/integrations/handlers/singlestore_handler/requirements.txt
 mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
 mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
 mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
 mindsdb/integrations/handlers/slack_handler/__about__.py
```

### Comparing `MindsDB-23.5.3.2/MindsDB.egg-info/requires.txt` & `MindsDB-23.5.4.1/MindsDB.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/PKG-INFO` & `MindsDB-23.5.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MindsDB
-Version: 23.5.3.2
+Version: 23.5.4.1
 Summary: MindsDB server, provides server capabilities to mindsdb native python library
 Home-page: https://github.com/mindsdb/mindsdb
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb/
 Description: <h1 align="center">
@@ -133,16 +133,16 @@
         | <a href="https://docs.mindsdb.com/data-integrations/cockroachdb"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/ckan"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/clickhouse"><img src="https://img.shields.io/badge/Clickhouse-e6e600?style=for-the-badge&logo=clickhouse&logoColor=white" alt="Connect Clickhouse"></a> | <a href="https://docs.mindsdb.com/data-integrations/google-bigquery"><img src="https://img.shields.io/badge/Google Big Query-0466C8?logo=Big Query&logoColor=fff&style=for-the-badge" alt="Google Big Query Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/sqlite"><img src="https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=fff&style=for-the-badge" alt="SQLite Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/tidb#tidb-handler"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/data-integrations/cratedb"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href=" https://docs.mindsdb.com/data-integrations/timescaledb"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/d0lt"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/amazon-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/ibm-db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/yugabytedb"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
-        | <a href="https://docs.mindsdb.com/data-integrations/questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/apache-druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> |
-        | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/redis-%23DD0031.svg?&style=for-the-badge&logo=redis&logoColor=white" alt="Connect Redis"></a> | <a href="https://docs.mindsdb.com/data-integrations/vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/apache-druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href="https://docs.mindsdb.com/data-integrations/elasticsearch"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#scylla"><img src="https://img.shields.io/badge/ScyllaDB-53CADD?style=for-the-badge&logo=scylladbb&logoColor=white" alt="Connect ScyllaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#firebird"><img src="https://img.shields.io/badge/Firebird-F40D12?logo=Firebird&logoColor=fff&style=for-the-badge" alt="Firebird Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#singlestore"><img src="https://img.shields.io/badge/Singlestore-5f07b4?style=for-the-badge&logo=singlestore&logoColor=white" alt="Connect Singlestore"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#hive"><img src="https://img.shields.io/badge/Apache%20Hive-FDEE21?logo=apachehive&logoColor=000&style=for-the-badge" alt="Apache Hive Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/teradata"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
         | <a href=" https://docs.mindsdb.com/data-integrations/snowflake"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/trino"><img src="https://img.shields.io/badge/Trino-dd00a1?style=for-the-badge&logo=trino&logoColor=white" alt="Connect Trino"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#monetdb"><img src="https://img.shields.io/badge/Monetdb-0099E5?logo=Monetdb&logoColor=fff&style=for-the-badge" alt="Monetdb Badge"></a> |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MindsDB Version: 23.5.3.2 Summary: MindsDB server,
+Metadata-Version: 2.1 Name: MindsDB Version: 23.5.4.1 Summary: MindsDB server,
 provides server capabilities to mindsdb native python library Home-page: https:
 //github.com/mindsdb/mindsdb Author: MindsDB Inc Author-email:
 jorge@mindsdb.com License: GPL-3.0 Download-URL: https://pypi.org/project/
 mindsdb/ Description:
                                ****** [MindsDB]
                                      ******
       [ROSS_Index_-_Fastest_Growing_Open-Source_Startups_|_Runa_Capital]
@@ -92,23 +92,23 @@
 Badge] | [Pinot_Badge] | | [Connect_Cassandra] | [DataStax_Badge] | [Amazon_S3
 Badge] | | [Connect_CockroachDB] | [ckan_Badge] | [Supabase_Badge] | | [Connect
 Clickhouse] | [Google_Big_Query_Badge] | [SQLite_Badge] | | [Connect_MariaDB] |
 [Couchbase_Badge] | [TiDB_Badge] | | [Connect_SQL_Server] | [CrateDB_Badge] |
 [Timescale_Badge] | | [Connect_MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB
 Badge] | | [Connect_PostgreSQL] | [IBMDB2_Badge] | [openGauss_Badge] | |
 [Connect_MySQL] | [Databricks_Badge] | [YugabyteDB_Badge] | [Connect_QuestDB] |
-[Apache_Druid_Badge] | [StarRocks_Badge] | | [Connect_Redis] | [Vertica_Badge]
-| [DuckDB_Badge] | | [Connect_SAP_HANA] | [Elastic_Badge] | [Cloud_Spanner
-Badge] | | [Connect_ScyllaDB] | [Firebird_Badge] | | [Connect_Singlestore] |
-[Apache_Hive_Badge] | | [Connect_Teradata] | [Matrixone_Badge] | | [Connect
-Snowflake] | [Informix_Badge] | | [Connect_Trino] | [Monetdb_Badge] | [:
-question: :wave: Missing integration?](https://github.com/mindsdb/mindsdb/
-issues/new?assignees=&labels=&template=feature-mindsdb-request.yaml) ##
-Documentation You can find the complete documentation of MindsDB at
-[docs.mindsdb.com](https://
+[Apache_Druid_Badge] | | [StarRocks_Badge] | [Vertica_Badge] | [DuckDB_Badge] |
+| [Connect_SAP_HANA] | [Elastic_Badge] | [Cloud_Spanner_Badge] | | [Connect
+ScyllaDB] | [Firebird_Badge] | | [Connect_Singlestore] | [Apache_Hive_Badge] |
+| [Connect_Teradata] | [Matrixone_Badge] | | [Connect_Snowflake] | [Informix
+Badge] | | [Connect_Trino] | [Monetdb_Badge] | [:question: :wave: Missing
+integration?](https://github.com/mindsdb/mindsdb/issues/
+new?assignees=&labels=&template=feature-mindsdb-request.yaml) ## Documentation
+You can find the complete documentation of MindsDB at [docs.mindsdb.com](https:
+//
 docs.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
 ## Support If you found a bug, please submit an [issue on GitHub](https://
 github.com/mindsdb/mindsdb/issues/new/choose). To get community support, you
 can: * Post at MindsDB [Slack community](https://mindsdb.com/joincommunity). *
 Ask for help at our [GitHub Discussions](https://github.com/mindsdb/mindsdb/
 discussions). * Ask a question at [Stackoverflow](https://stackoverflow.com/
 questions/tagged/mindsdb) with a MindsDB tag. If you need commercial support,
```

### Comparing `MindsDB-23.5.3.2/README.md` & `MindsDB-23.5.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -124,16 +124,16 @@
 | <a href="https://docs.mindsdb.com/data-integrations/cockroachdb"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/ckan"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/clickhouse"><img src="https://img.shields.io/badge/Clickhouse-e6e600?style=for-the-badge&logo=clickhouse&logoColor=white" alt="Connect Clickhouse"></a> | <a href="https://docs.mindsdb.com/data-integrations/google-bigquery"><img src="https://img.shields.io/badge/Google Big Query-0466C8?logo=Big Query&logoColor=fff&style=for-the-badge" alt="Google Big Query Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/sqlite"><img src="https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=fff&style=for-the-badge" alt="SQLite Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/tidb#tidb-handler"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/data-integrations/cratedb"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href=" https://docs.mindsdb.com/data-integrations/timescaledb"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/d0lt"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/amazon-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/ibm-db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/yugabytedb"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
-| <a href="https://docs.mindsdb.com/data-integrations/questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/apache-druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> |
-| <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/redis-%23DD0031.svg?&style=for-the-badge&logo=redis&logoColor=white" alt="Connect Redis"></a> | <a href="https://docs.mindsdb.com/data-integrations/vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/apache-druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href="https://docs.mindsdb.com/data-integrations/elasticsearch"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#scylla"><img src="https://img.shields.io/badge/ScyllaDB-53CADD?style=for-the-badge&logo=scylladbb&logoColor=white" alt="Connect ScyllaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#firebird"><img src="https://img.shields.io/badge/Firebird-F40D12?logo=Firebird&logoColor=fff&style=for-the-badge" alt="Firebird Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#singlestore"><img src="https://img.shields.io/badge/Singlestore-5f07b4?style=for-the-badge&logo=singlestore&logoColor=white" alt="Connect Singlestore"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#hive"><img src="https://img.shields.io/badge/Apache%20Hive-FDEE21?logo=apachehive&logoColor=000&style=for-the-badge" alt="Apache Hive Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/teradata"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
 | <a href=" https://docs.mindsdb.com/data-integrations/snowflake"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/trino"><img src="https://img.shields.io/badge/Trino-dd00a1?style=for-the-badge&logo=trino&logoColor=white" alt="Connect Trino"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#monetdb"><img src="https://img.shields.io/badge/Monetdb-0099E5?logo=Monetdb&logoColor=fff&style=for-the-badge" alt="Monetdb Badge"></a> |
```

#### html2text {}

```diff
@@ -87,23 +87,23 @@
 Badge] | [Pinot_Badge] | | [Connect_Cassandra] | [DataStax_Badge] | [Amazon_S3
 Badge] | | [Connect_CockroachDB] | [ckan_Badge] | [Supabase_Badge] | | [Connect
 Clickhouse] | [Google_Big_Query_Badge] | [SQLite_Badge] | | [Connect_MariaDB] |
 [Couchbase_Badge] | [TiDB_Badge] | | [Connect_SQL_Server] | [CrateDB_Badge] |
 [Timescale_Badge] | | [Connect_MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB
 Badge] | | [Connect_PostgreSQL] | [IBMDB2_Badge] | [openGauss_Badge] | |
 [Connect_MySQL] | [Databricks_Badge] | [YugabyteDB_Badge] | [Connect_QuestDB] |
-[Apache_Druid_Badge] | [StarRocks_Badge] | | [Connect_Redis] | [Vertica_Badge]
-| [DuckDB_Badge] | | [Connect_SAP_HANA] | [Elastic_Badge] | [Cloud_Spanner
-Badge] | | [Connect_ScyllaDB] | [Firebird_Badge] | | [Connect_Singlestore] |
-[Apache_Hive_Badge] | | [Connect_Teradata] | [Matrixone_Badge] | | [Connect
-Snowflake] | [Informix_Badge] | | [Connect_Trino] | [Monetdb_Badge] | [:
-question: :wave: Missing integration?](https://github.com/mindsdb/mindsdb/
-issues/new?assignees=&labels=&template=feature-mindsdb-request.yaml) ##
-Documentation You can find the complete documentation of MindsDB at
-[docs.mindsdb.com](https://
+[Apache_Druid_Badge] | | [StarRocks_Badge] | [Vertica_Badge] | [DuckDB_Badge] |
+| [Connect_SAP_HANA] | [Elastic_Badge] | [Cloud_Spanner_Badge] | | [Connect
+ScyllaDB] | [Firebird_Badge] | | [Connect_Singlestore] | [Apache_Hive_Badge] |
+| [Connect_Teradata] | [Matrixone_Badge] | | [Connect_Snowflake] | [Informix
+Badge] | | [Connect_Trino] | [Monetdb_Badge] | [:question: :wave: Missing
+integration?](https://github.com/mindsdb/mindsdb/issues/
+new?assignees=&labels=&template=feature-mindsdb-request.yaml) ## Documentation
+You can find the complete documentation of MindsDB at [docs.mindsdb.com](https:
+//
 docs.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
 ## Support If you found a bug, please submit an [issue on GitHub](https://
 github.com/mindsdb/mindsdb/issues/new/choose). To get community support, you
 can: * Post at MindsDB [Slack community](https://mindsdb.com/joincommunity). *
 Ask for help at our [GitHub Discussions](https://github.com/mindsdb/mindsdb/
 discussions). * Ask a question at [Stackoverflow](https://stackoverflow.com/
 questions/tagged/mindsdb) with a MindsDB tag. If you need commercial support,
```

### Comparing `MindsDB-23.5.3.2/mindsdb/__main__.py` & `MindsDB-23.5.4.1/mindsdb/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import json
 import atexit
 import signal
 import psutil
 import asyncio
 import secrets
 import traceback
+import threading
 from packaging import version
 
 from mindsdb.__about__ import __version__ as mindsdb_version
 from mindsdb.api.http.start import start as start_http
 from mindsdb.api.mysql.start import start as start_mysql
 from mindsdb.api.mongo.start import start as start_mongo
 from mindsdb.api.postgres.start import start as start_postgres
@@ -21,37 +22,33 @@
 from mindsdb.utilities.functions import args_parse, get_versions_where_predictors_become_obsolete
 from mindsdb.utilities import log
 from mindsdb.interfaces.stream.stream import StreamController
 from mindsdb.interfaces.stream.utilities import STOP_THREADS_EVENT
 from mindsdb.interfaces.database.integrations import integration_controller
 import mindsdb.interfaces.storage.db as db
 from mindsdb.integrations.utilities.install import install_dependencies
-from mindsdb.utilities.fs import create_dirs_recursive
+from mindsdb.utilities.fs import create_dirs_recursive, clean_process_marks, clean_unlinked_process_marks
 from mindsdb.utilities.telemetry import telemetry_file_exists, disable_telemetry
 from mindsdb.utilities.context import context as ctx
 from mindsdb.utilities.auth import register_oauth_client, get_aws_meta_data
 
 
 import torch.multiprocessing as mp
 try:
     mp.set_start_method('spawn')
 except RuntimeError:
     log.logger.info('Torch multiprocessing context already set, ignoring...')
 
-# is_ray_worker = False
-# if sys.argv[0].endswith('ray/workers/default_worker.py'):
-#     is_ray_worker = True
-#
-# is_alembic = os.path.basename(sys.argv[0]).split('.')[0] == 'alembic'
-# is_pytest = os.path.basename(sys.argv[0]).split('.')[0] == 'pytest'
-#
-# if not is_ray_worker:
+
+_stop_event = threading.Event()
 
 
 def close_api_gracefully(apis):
+    _stop_event.set()
+    STOP_THREADS_EVENT.set()
     try:
         for api in apis.values():
             process = api['process']
             childs = get_child_pids(process.pid)
             for p in childs:
                 try:
                     os.kill(p, signal.SIGTERM)
@@ -63,16 +60,22 @@
             sys.stdout.flush()
     except KeyboardInterrupt:
         sys.exit(0)
     except psutil.NoSuchProcess:
         pass
 
 
+def do_clean_process_marks():
+    while _stop_event.wait(timeout=5) is False:
+        clean_unlinked_process_marks()
+
+
 if __name__ == '__main__':
     # ----------------  __init__.py section ------------------
+    clean_process_marks()
     ctx.set_default()
     args = args_parse()
 
     # ---- CHECK SYSTEM ----
     if not (sys.version_info[0] >= 3 and sys.version_info[1] >= 6):
         print("""
      MindsDB server requires Python >= 3.7 to run
@@ -193,14 +196,17 @@
     for handler_name, handler_meta in integration_controller.get_handlers_import_status().items():
         import_meta = handler_meta.get('import', {})
         dependencies = import_meta.get('dependencies')
         if import_meta.get('success', False) is not True:
             print(f"Dependencies for the handler '{handler_name}' are not installed by default.\n",
                   f'If you want to use "{handler_name}" please install "{dependencies}"')
 
+    # from mindsdb.utilities.fs import get_marked_processes_and_threads
+    # marks = get_marked_processes_and_threads()
+
     if not is_cloud:
         # region creating permanent integrations
         for integration_name, handler in integration_controller.get_handlers_import_status().items():
             if handler.get('permanent'):
                 integration_meta = integration_controller.get(name=integration_name)
                 if integration_meta is None:
                     integration_record = db.Integration(
@@ -328,18 +334,29 @@
         for i, future in enumerate(asyncio.as_completed(futures)):
             api_name, port, started = await future
             if started:
                 print(f"{api_name} API: started on {port}")
             else:
                 log.logger.error(f"ERROR: {api_name} API cant start on {port}")
 
-    ioloop = asyncio.get_event_loop()
+    async def join_process(process, name):
+        try:
+            process.join()
+        except KeyboardInterrupt:
+            print('Got keyboard interrupt, stopping APIs')
+            close_api_gracefully(apis)
+        finally:
+            print(f'{name} API: stopped')
+
+    async def gather_apis():
+        await asyncio.gather(
+            *[join_process(api_data['process'], api_name) for api_name, api_data in apis.items()],
+            return_exceptions=False
+        )
+
+    ioloop = asyncio.new_event_loop()
     ioloop.run_until_complete(wait_apis_start())
-    ioloop.close()
 
-    try:
-        for api_data in apis.values():
-            api_data['process'].join()
-    except KeyboardInterrupt:
-        print('Stopping stream integrations...')
-        STOP_THREADS_EVENT.set()
-        print('Closing app...')
+    threading.Thread(target=do_clean_process_marks).start()
+
+    ioloop.run_until_complete(gather_apis())
+    ioloop.close()
```

### Comparing `MindsDB-23.5.3.2/mindsdb/api/common/check_auth.py` & `MindsDB-23.5.4.1/mindsdb/api/common/check_auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/http/gui.py` & `MindsDB-23.5.4.1/mindsdb/api/http/gui.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/http/gunicorn_wrapper.py` & `MindsDB-23.5.4.1/mindsdb/api/http/gunicorn_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/http/initialize.py` & `MindsDB-23.5.4.1/mindsdb/api/http/initialize.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/http/namespaces/analysis.py` & `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/analysis.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/http/namespaces/auth.py` & `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/http/namespaces/config.py` & `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/http/namespaces/databases.py` & `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/databases.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/http/namespaces/default.py` & `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/default.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/http/namespaces/file.py` & `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/file.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/http/namespaces/handlers.py` & `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/handlers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/http/namespaces/models.py` & `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/models.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/http/namespaces/projects.py` & `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/http/namespaces/sql.py` & `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/http/namespaces/stream.py` & `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/stream.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/http/namespaces/tab.py` & `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/tab.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/http/namespaces/tree.py` & `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/tree.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/http/namespaces/util.py` & `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/util.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/http/namespaces/views.py` & `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/http/start.py` & `MindsDB-23.5.4.1/mindsdb/api/http/start.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/http/utils.py` & `MindsDB-23.5.4.1/mindsdb/api/http/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/classes/query_sql.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/classes/query_sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/classes/responder.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/classes/responder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/classes/responder_collection.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/classes/responder_collection.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/classes/scram.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/classes/scram.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/classes/session.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/classes/session.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/responders/__init__.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/responders/aggregate.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/aggregate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/responders/coll_stats.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/coll_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/responders/company_id.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/company_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/responders/connection_status.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/connection_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/responders/db_stats.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/db_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/responders/delete.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/delete.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/responders/find.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/find.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/responders/get_parameter.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/get_parameter.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/responders/host_info.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/host_info.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/responders/insert.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/insert.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/responders/list_collections.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/list_collections.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/responders/list_databases.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/list_databases.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/responders/list_indexes.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/list_indexes.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/responders/sasl_continue.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/sasl_continue.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/responders/sasl_start.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/sasl_start.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/server.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/server.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/utilities/mongodb_ast.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/utilities/mongodb_ast.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/utilities/mongodb_parser.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/utilities/mongodb_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mongo/utilities/mongodb_query.py` & `MindsDB-23.5.4.1/mindsdb/api/mongo/utilities/mongodb_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
         'PLUGINS': ['PLUGIN_NAME', 'PLUGIN_VERSION', 'PLUGIN_STATUS', 'PLUGIN_TYPE', 'PLUGIN_TYPE_VERSION', 'PLUGIN_LIBRARY', 'PLUGIN_LIBRARY_VERSION', 'PLUGIN_AUTHOR', 'PLUGIN_DESCRIPTION', 'PLUGIN_LICENSE', 'LOAD_OPTION', 'PLUGIN_MATURITY', 'PLUGIN_AUTH_VERSION'],
         'ENGINES': ['ENGINE', 'SUPPORT', 'COMMENT', 'TRANSACTIONS', 'XA', 'SAVEPOINTS'],
         'KEY_COLUMN_USAGE': ['CONSTRAINT_CATALOG', 'CONSTRAINT_SCHEMA', 'CONSTRAINT_NAME', 'TABLE_CATALOG', 'TABLE_SCHEMA', 'TABLE_NAME', 'COLUMN_NAME', 'ORDINAL_POSITION', 'POSITION_IN_UNIQUE_CONSTRAINT', 'REFERENCED_TABLE_SCHEMA', 'REFERENCED_TABLE_NAME', 'REFERENCED_COLUMN_NAME'],
         'STATISTICS': ['TABLE_CATALOG', 'TABLE_SCHEMA', 'TABLE_NAME', 'NON_UNIQUE', 'INDEX_SCHEMA', 'INDEX_NAME', 'SEQ_IN_INDEX', 'COLUMN_NAME', 'COLLATION', 'CARDINALITY', 'SUB_PART', 'PACKED', 'NULLABLE', 'INDEX_TYPE', 'COMMENT', 'INDEX_COMMENT', 'IS_VISIBLE', 'EXPRESSION'],
         'CHARACTER_SETS': ['CHARACTER_SET_NAME', 'DEFAULT_COLLATE_NAME', 'DESCRIPTION', 'MAXLEN'],
         'COLLATIONS': ['COLLATION_NAME', 'CHARACTER_SET_NAME', 'ID', 'IS_DEFAULT', 'IS_COMPILED', 'SORTLEN', 'PAD_ATTRIBUTE'],
         # MindsDB specific:
-        'MODELS': ['NAME', 'ENGINE', 'PROJECT', 'VERSION', 'STATUS', 'ACCURACY', 'PREDICT', 'UPDATE_STATUS', 'MINDSDB_VERSION', 'ERROR', 'SELECT_DATA_QUERY', 'TRAINING_OPTIONS', 'CURRENT_TRAINING_PHASE', 'TOTAL_TRAINING_PHASES', 'TRAINING_PHASE_NAME', 'TAG', 'CREATED_AT'],
-        'MODELS_VERSIONS': ['NAME', 'ENGINE', 'PROJECT', 'ACTIVE', 'VERSION', 'STATUS', 'ACCURACY', 'PREDICT', 'UPDATE_STATUS', 'MINDSDB_VERSION', 'ERROR', 'SELECT_DATA_QUERY', 'TRAINING_OPTIONS', 'TAG', 'CREATED_AT'],
+        'MODELS': ['NAME', 'ENGINE', 'PROJECT', 'VERSION', 'STATUS', 'ACCURACY', 'PREDICT', 'UPDATE_STATUS', 'MINDSDB_VERSION', 'ERROR', 'SELECT_DATA_QUERY', 'TRAINING_OPTIONS', 'CURRENT_TRAINING_PHASE', 'TOTAL_TRAINING_PHASES', 'TRAINING_PHASE_NAME', 'TAG', 'CREATED_AT', 'TRAINING_TIME'],
+        'MODELS_VERSIONS': ['NAME', 'ENGINE', 'PROJECT', 'ACTIVE', 'VERSION', 'STATUS', 'ACCURACY', 'PREDICT', 'UPDATE_STATUS', 'MINDSDB_VERSION', 'ERROR', 'SELECT_DATA_QUERY', 'TRAINING_OPTIONS', 'TAG', 'CREATED_AT', 'TRAINING_TIME'],
         'DATABASES': ['NAME', 'TYPE', 'ENGINE'],
         'ML_ENGINES': ['NAME', 'HANDLER', 'CONNECTION_DATA'],
         'HANDLERS': ['NAME', 'TITLE', 'DESCRIPTION', 'VERSION', 'CONNECTION_ARGS', 'IMPORT_SUCCESS', 'IMPORT_ERROR'],
         'JOBS': ['NAME', 'PROJECT', 'START_AT', 'END_AT', 'NEXT_RUN_AT', 'SCHEDULE_STR', 'QUERY'],
         'JOBS_HISTORY': ['NAME', 'PROJECT', 'RUN_START', 'RUN_END', 'ERROR', 'QUERY']
     }
 
@@ -337,15 +337,15 @@
                     continue
                 data.append([
                     table_name, table_meta['engine'], project_name, table_meta['version'], table_meta['status'],
                     table_meta['accuracy'], table_meta['predict'], table_meta['update_status'],
                     table_meta['mindsdb_version'], table_meta['error'], table_meta['select_data_query'],
                     table_meta['training_options'], table_meta['current_training_phase'],
                     table_meta['total_training_phases'], table_meta['training_phase_name'],
-                    table_meta['label'], row['created_at']
+                    table_meta['label'], row['created_at'], table_meta['training_time']
                 ])
             # TODO optimise here
             # if target_table is not None and target_table != project_name:
             #     continue
 
         df = pd.DataFrame(data, columns=columns)
         return df
@@ -359,15 +359,15 @@
             for row in project_models:
                 table_name = row['name']
                 table_meta = row['metadata']
                 data.append([
                     table_name, table_meta['engine'], project_name, table_meta['active'], table_meta['version'], table_meta['status'],
                     table_meta['accuracy'], table_meta['predict'], table_meta['update_status'],
                     table_meta['mindsdb_version'], table_meta['error'], table_meta['select_data_query'],
-                    table_meta['training_options'], table_meta['label'], row['created_at']
+                    table_meta['training_options'], table_meta['label'], row['created_at'], table_meta['training_time']
                 ])
 
         df = pd.DataFrame(data, columns=columns)
         return df
 
     def _get_columns(self, query: ASTNode = None):
         columns = self.information_schema['COLUMNS']
```

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/executor/data_types.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/data_types.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/executor/executor.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     get_predictor_integration,
 )
 from mindsdb.integrations.libs.const import PREDICTOR_STATUS
 from mindsdb.interfaces.database.projects import ProjectController
 from mindsdb.interfaces.jobs.jobs_controller import JobsController
 from mindsdb.interfaces.storage.model_fs import HandlerStorage
 from mindsdb.utilities.context import context as ctx
+from mindsdb.utilities.functions import resolve_model_identifier
 import mindsdb.utilities.profiler as profiler
 
 
 def _get_show_where(
         statement: ASTNode,
         from_name: Optional[str] = None,
         like_name: Optional[str] = None,
@@ -681,21 +682,21 @@
             data=df_dict['data']
         )
 
     def _get_model_info(self, identifier, except_absent=True):
         if len(identifier.parts) == 1:
             identifier.parts = [self.session.database, identifier.parts[0]]
 
-        if len(identifier.parts) == 2:
-            database_name, model_name = identifier.parts[-2:]
-        else:
-            return None
+        database_name, model_name, model_version, _describe = resolve_model_identifier(identifier)
 
         model_record = get_model_record(
-            name=model_name, project_name=database_name, except_absent=except_absent
+            name=model_name,
+            project_name=database_name,
+            except_absent=except_absent,
+            version=model_version
         )
         if not model_record:
             return None
         return {
             'model_record': model_record,
             'project_name': database_name
         }
```

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/utilities/functions.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/mysql/mysql_proxy/utilities/sql.py` & `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/nlp/nlp.py` & `MindsDB-23.5.4.1/mindsdb/api/nlp/nlp.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/executor/executor.py` & `MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/executor/executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py` & `MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py` & `MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py` & `MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py` & `MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py` & `MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py` & `MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py` & `MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/access_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/access_handler/access_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/access_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/airtable_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/airtable_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/altibase_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/altibase_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/aurora_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/aurora_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/autokeras_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/autokeras_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/autokeras_handler/setup.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/autokeras_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/autosklearn_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/autosklearn_handler/config.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/autosklearn_handler/setup.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/bigquery_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/bigquery_handler/logo.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/logo.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/binance_handler/binance_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/binance_handler/binance_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/binance_handler/binance_tables.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/binance_handler/binance_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/binance_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/binance_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/byom_handler/byom_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/byom_handler/byom_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/cassandra_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/cassandra_handler/logo.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/ckan_handler/logo.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/clickhouse_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_sql_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/confluence_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/confluence_handler/confluence_table.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/confluence_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/confluence_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/couchbase_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/couchbase_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/crate_handler/crate_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/crate_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/d0lt_handler/create-db.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/create-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/d0lt_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/d0lt_handler/predict-target.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/predict-target.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/databend_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/databend_handler/databend_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/databend_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/datastax_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/datastax_handler/logo.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/db2_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/db2_handler/db2_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/db2_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/derby_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/derby_handler/derby_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/derby_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/dremio_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/dremio_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/druid_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/druid_handler/druid_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/druid_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/duckdb_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/duckdb_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/dynamodb_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/dynamodb_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/elasticsearch_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/empress_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/empress_handler/empress_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/empress_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/file_handler/file_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/file_handler/file_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/firebird_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/firebird_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/github_handler/github_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/github_handler/github_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/github_handler/github_tables.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/github_handler/github_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/github_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/github_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/gitlab_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/gitlab_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_books_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_calendar_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_calendar_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_fit_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_fit_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_search_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_search_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/hackernews_handler/hn_table.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hackernews_handler/hn_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/hackernews_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hackernews_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/hana_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hana_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/hana_handler/hana_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hana_handler/hana_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/hana_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hana_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/hive_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/hive_handler/hive_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/hive_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/hsqldb_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hsqldb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/hsqldb_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hsqldb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/huggingface_api_handler/setup.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/huggingface_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/huggingface_handler/setup.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/ignite_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/ignite_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/impala_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/impala_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/impala_handler/impala_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/influxdb_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/influxdb_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/informix_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/informix_handler/informix_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/ingres_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/ingres_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/jira_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/jira_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/jira_handler/jira_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/jira_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/jira_handler/jira_table.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/jira_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/langchain_handler/setup.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/langchain_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,24 +210,23 @@
             name=predictor_record.name,
         )
         predictor_records = [
             x for x in predictor_records
             if x.training_stop_at is not None
         ]
         predictor_records.sort(key=lambda x: x.training_stop_at)
-        for record in predictor_records:
-            record.active = False
-        predictor_records[-1].active = True
         db.session.commit()
 
     except Exception as e:
         log.logger.error(e)
         predictor_id = model_storage.predictor_id
         predictor_record = db.Predictor.query.with_for_update().get(predictor_id)
         print(traceback.format_exc())
         error_message = format_exception_error(e)
         predictor_record.data = {"error": error_message}
+        predictor_record.status = PREDICTOR_STATUS.ERROR
         db.session.commit()
-
-    if predictor_record.training_stop_at is None:
-        predictor_record.training_stop_at = datetime.now()
-        db.session.commit()
+        raise
+    finally:
+        if predictor_record.training_stop_at is None:
+            predictor_record.training_stop_at = datetime.now()
+            db.session.commit()
```

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/lightwood_handler/setup.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/ludwig_handler/setup.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ludwig_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/mariadb_handler/1-create_db.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/1-create_db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/mariadb_handler/2-create_predictor.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/2-create_predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/mariadb_handler/3-predict_target.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/3-predict_target.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/mariadb_handler/4-drop_db.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/4-drop_db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/mariadb_handler/create-db.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/create-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/mariadb_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/mariadb_handler/predict-db.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/predict-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/mariadb_handler/predictor.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/materialize_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/matrixone_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/matrixone_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/maxdb_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/maxdb_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/merlion_handler/adapters.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/merlion_handler/adapters.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/merlion_handler/setup.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/merlion_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/mlflow_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mlflow_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/mlflow_handler/setup.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mlflow_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/create-database.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/create-database.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/mongodb_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/mssql_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/mysql_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mysql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/mysql_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mysql_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/neuralforecast_handler/setup.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/neuralforecast_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/newsapi_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/newsapi_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/oceanbase_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/openai_handler/helpers.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/openai_handler/helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/openai_handler/openai_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/openai_handler/openai_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/openai_handler/setup.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/openai_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/opengauss_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/oracle_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/oracle_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/orioledb_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/phoenix_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/phoenix_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/pinot_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/pinot_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/plaid_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/planetscale_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/planetscale_handler/create-db.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/create-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/planetscale_handler/drop-db.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/drop-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/planetscale_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/planetscale_handler/predict-target.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/predict-target.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/postgres_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/postgres_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/questdb_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/quickbooks_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/quickbooks_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/ray_serve_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ray_serve_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/ray_serve_handler/setup.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ray_serve_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/reddit_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/reddit_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/redshift_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/redshift_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/rockset_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/rockset_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/rockset_handler/tests/test.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/rockset_handler/tests/test.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/rockset_handler/tests/test2.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/rockset_handler/tests/test2.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/s3_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/s3_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/s3_handler/s3_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/scylla_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/scylla_handler/logo.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sendinblue_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sendinblue_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sendinblue_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sendinblue_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sheets_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sheets_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/slack_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/slack_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/slack_handler/slack_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/slack_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/solr_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/solr_handler/solr.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/solr.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/solr_handler/solr_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlany_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlany_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlany_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlany_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/db_connection.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/db_connection.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/error.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/error.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/model_drop.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/model_drop.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqreamdb_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/starrocks_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/statsforecast_handler/setup.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/statsforecast_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/strava_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/strava_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/strava_handler/strava_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/strava_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/strava_handler/strava_tables.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/strava_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/supabase_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/surrealdb_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/surrealdb_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/tdengine_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/tdengine_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/teradata_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/teradata_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/teradata_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/teradata_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/tidb_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/timescaledb_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/tpot_handler/setup.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/tpot_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/trino_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/trino_handler/trino_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/trino_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/twitter_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/twitter_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/vertica_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/vertica_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/vitess_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/youtube_handler/__init__.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/youtube_handler/icon.png` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/yugabyte_handler/icon.svg` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers_client/db_client_factory.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers_client/db_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers_client/db_grpc_client.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers_client/db_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers_client/ml_client_factory.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers_client/ml_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers_client/ml_grpc_client.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers_client/ml_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers_wrapper/db_handler_service.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers_wrapper/db_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/handlers_wrapper/ml_handler_service.py` & `MindsDB-23.5.4.1/mindsdb/integrations/handlers_wrapper/ml_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/libs/api_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/libs/api_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Any
 import ast as py_ast
 
 import pandas as pd
 
 from mindsdb_sql.parser.ast import ASTNode, Select, Insert, Update, Delete
+from mindsdb_sql.parser.ast.select.identifier import Identifier
 
 from mindsdb.integrations.libs.base import BaseHandler
 
 from mindsdb.integrations.libs.response import (
     HandlerResponse as Response,
     RESPONSE_TYPE
 )
@@ -163,19 +164,19 @@
 
     def _register_table(self, table_name: str, table_class: Any):
         """
         Register the data resource. For e.g if you are using Twitter API it registers the `tweets` resource from `/api/v2/tweets`.
         """
         self._tables[table_name] = table_class
 
-    def _get_table(self, name):
+    def _get_table(self, name: Identifier):
         """
         Check if the table name was added to the the _register_table
         Args:
-            name (str): the table name
+            name (Identifier): the table name
         """
         name = name.parts[-1]
         if name not in self._tables:
             raise RuntimeError(f'Table not found: {name}')
         return self._tables[name]
 
     def query(self, query: ASTNode):
@@ -203,27 +204,26 @@
         Returns a list of entity columns
         Args:
             table_name (str): the table name
         Returns:
             RESPONSE_TYPE.TABLE
         """
 
-        result = self._get_table(table_name).get_columns()
+        result = self._get_table(Identifier(table_name)).get_columns()
 
         df = pd.DataFrame(result, columns=['Field'])
         df['Type'] = 'str'
 
         return Response(RESPONSE_TYPE.TABLE, df)
 
     def get_tables(self) -> Response:
         """
         Return list of entities
         Returns:
             RESPONSE_TYPE.TABLE
         """
-
         result = list(self._tables.keys())
 
         df = pd.DataFrame(result, columns=['table_name'])
         df['table_type'] = 'BASE TABLE'
 
         return Response(RESPONSE_TYPE.TABLE, df)
```

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/libs/base.py` & `MindsDB-23.5.4.1/mindsdb/integrations/libs/base.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/libs/handler_helpers.py` & `MindsDB-23.5.4.1/mindsdb/integrations/libs/handler_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/libs/ml_exec_base.py` & `MindsDB-23.5.4.1/mindsdb/integrations/libs/ml_exec_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,24 +60,25 @@
 
 class MLEngineException(Exception):
     pass
 
 
 @mark_process(name='learn')
 def learn_process(class_path, engine, context_dump, integration_id,
-                  predictor_id, data_integration_ref, fetch_data_query,
-                  project_name, problem_definition, set_active,
-                  base_predictor_id=None):
+                  predictor_id, problem_definition, set_active,
+                  base_predictor_id=None, training_data_df=None,
+                  data_integration_ref=None, fetch_data_query=None, project_name=None):
     ctx.load(context_dump)
     db.init()
 
     predictor_record = db.Predictor.query.with_for_update().get(predictor_id)
 
     try:
         target = problem_definition['target']
+
         training_data_df = None
 
         database_controller = DatabaseController()
 
         sql_session = make_sql_session()
         if data_integration_ref is not None:
             if data_integration_ref['type'] == 'integration':
@@ -137,14 +138,15 @@
         # fine-tune (partially train) existing model
         else:
             # load model from previous version, use it as starting point
             problem_definition['base_model_id'] = base_predictor_id
             ml_handler.finetune(df=training_data_df, args=problem_definition)
 
         predictor_record.status = PREDICTOR_STATUS.COMPLETE
+        predictor_record.active = set_active
         db.session.commit()
         # if retrain and set_active after success creation
         if set_active is True:
             models = get_model_records(
                 name=predictor_record.name,
                 project_id=predictor_record.project_id,
                 active=None
@@ -322,23 +324,25 @@
         p = HandlerProcess(
             learn_process,
             class_path,
             self.engine,
             ctx.dump(),
             self.integration_id,
             predictor_record.id,
-            data_integration_ref,
-            fetch_data_query,
-            project_name,
             problem_definition,
-            set_active
+            set_active,
+            data_integration_ref=data_integration_ref,
+            fetch_data_query=fetch_data_query,
+            project_name=project_name
         )
         p.start()
         if join_learn_process is True:
             p.join()
+            predictor_record = db.Predictor.query.get(predictor_record.id)
+            db.session.refresh(predictor_record)
 
         return predictor_record
 
     def predict(self, model_name: str, data: list, pred_format: str = 'dict',
                 project_name: str = None, version=None, params: dict = None):
         """ Generates predictions with some model and input data. """
         if isinstance(data, dict):
@@ -457,19 +461,21 @@
         p = HandlerProcess(
             learn_process,
             class_path,
             self.engine,
             ctx.dump(),
             self.integration_id,
             predictor_record.id,
-            data_integration_ref,
-            fetch_data_query,
-            project_name,
             predictor_record.learn_args,
             set_active,
             base_predictor_record.id,
+            data_integration_ref=data_integration_ref,
+            fetch_data_query=fetch_data_query,
+            project_name=project_name
         )
         p.start()
         if join_learn_process is True:
             p.join()
+            predictor_record = db.Predictor.query.get(predictor_record.id)
+            db.session.refresh(predictor_record)
 
-        return base_predictor_record
+        return predictor_record
```

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/libs/ml_handler_proc.py` & `MindsDB-23.5.4.1/mindsdb/integrations/libs/ml_handler_proc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/libs/net_helpers.py` & `MindsDB-23.5.4.1/mindsdb/integrations/libs/net_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/libs/response.py` & `MindsDB-23.5.4.1/mindsdb/integrations/libs/response.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/libs/storage_handler.py` & `MindsDB-23.5.4.1/mindsdb/integrations/libs/storage_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/utilities/date_utils.py` & `MindsDB-23.5.4.1/mindsdb/integrations/utilities/date_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/utilities/install.py` & `MindsDB-23.5.4.1/mindsdb/integrations/utilities/install.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/utilities/sql_utils.py` & `MindsDB-23.5.4.1/mindsdb/integrations/utilities/sql_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/utilities/test_utils.py` & `MindsDB-23.5.4.1/mindsdb/integrations/utilities/test_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/integrations/utilities/time_series_utils.py` & `MindsDB-23.5.4.1/mindsdb/integrations/utilities/time_series_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/interfaces/database/database.py` & `MindsDB-23.5.4.1/mindsdb/interfaces/database/database.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/interfaces/database/integrations.py` & `MindsDB-23.5.4.1/mindsdb/interfaces/database/integrations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import sys
 import base64
 import shutil
 import tempfile
 import importlib
 import threading
+import multiprocessing
 from time import time
 from pathlib import Path
 from copy import deepcopy
 from typing import Optional
 from collections import OrderedDict
 
 from sqlalchemy import func
@@ -66,18 +67,20 @@
 
     def set(self, handler: DatabaseHandler):
         """ add (or replace) handler in cache
 
             Args:
                 handler (DatabaseHandler)
         """
-        # print(f'!!!! set {handler.name} {ctx.company_id} {threading.get_ident()}')
+        # do not cache connections in handlers processes
+        if multiprocessing.current_process().name.startswith('HandlerProcess'):
+            return
         with self._lock:
             try:
-                key = (handler.name, ctx.company_id, threading.get_ident())
+                key = (handler.name, ctx.company_id, threading.get_native_id())
                 handler.connect()
                 self.handlers[key] = {
                     'handler': handler,
                     'expired_at': time() + self.ttl
                 }
             except Exception:
                 pass
@@ -89,15 +92,15 @@
             Args:
                 name (str): handler name
 
             Returns:
                 DatabaseHandler
         """
         with self._lock:
-            key = (name, ctx.company_id, threading.get_ident())
+            key = (name, ctx.company_id, threading.get_native_id())
             if (
                 key not in self.handlers
                 or self.handlers[key]['expired_at'] < time()
             ):
                 return None
             self.handlers[key]['expired_at'] = time() + self.ttl
             return self.handlers[key]['handler']
@@ -105,15 +108,15 @@
     def delete(self, name: str) -> None:
         """ delete handler from cache
 
             Args:
                 name (str): handler name
         """
         with self._lock:
-            key = (name, ctx.company_id, threading.get_ident())
+            key = (name, ctx.company_id, threading.get_native_id())
             if key in self.handlers:
                 try:
                     self.handlers[key].disconnect()
                 except Exception:
                     pass
                 del self.handlers[key]
             if len(self.handlers) == 0:
```

### Comparing `MindsDB-23.5.3.2/mindsdb/interfaces/database/projects.py` & `MindsDB-23.5.4.1/mindsdb/interfaces/database/projects.py`

 * *Files 8% similar despite different names*

```diff
@@ -128,14 +128,26 @@
         if model_id is not None:
             query = query.filter(db.Predictor.id == model_id)
 
         data = []
 
         for predictor_record, integraion_record in query.all():
             predictor_data = predictor_record.data or {}
+            training_time = None
+            if (
+                predictor_record.training_start_at is not None
+                and predictor_record.training_stop_at is None
+                and predictor_record.status != 'error'
+            ):
+                training_time = int((datetime.datetime.now() - predictor_record.training_start_at).total_seconds())
+            elif (
+                predictor_record.training_start_at is not None
+                and predictor_record.training_stop_at is not None
+            ):
+                training_time = int((predictor_record.training_stop_at - predictor_record.training_start_at).total_seconds())
             predictor_meta = {
                 'type': 'model',
                 'id': predictor_record.id,
                 'engine': integraion_record.engine,
                 'engine_name': integraion_record.name,
                 'active': predictor_record.active,
                 'version': predictor_record.version,
@@ -148,14 +160,15 @@
                 'select_data_query': predictor_record.fetch_data_query,
                 'training_options': predictor_record.learn_args,
                 'deletable': True,
                 'label': predictor_record.label,
                 'current_training_phase': predictor_record.training_phase_current,
                 'total_training_phases': predictor_record.training_phase_total,
                 'training_phase_name': predictor_record.training_phase_name,
+                'training_time': training_time
             }
             if predictor_data.get('accuracies', None) is not None:
                 if len(predictor_data['accuracies']) > 0:
                     predictor_meta['accuracy'] = float(np.mean(list(predictor_data['accuracies'].values())))
             data.append({
                 'name': predictor_record.name,
                 'metadata': predictor_meta,
```

### Comparing `MindsDB-23.5.3.2/mindsdb/interfaces/database/views.py` & `MindsDB-23.5.4.1/mindsdb/interfaces/database/views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/interfaces/file/file_controller.py` & `MindsDB-23.5.4.1/mindsdb/interfaces/file/file_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/interfaces/jobs/jobs_controller.py` & `MindsDB-23.5.4.1/mindsdb/interfaces/jobs/jobs_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/interfaces/jobs/scheduler.py` & `MindsDB-23.5.4.1/mindsdb/interfaces/jobs/scheduler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/interfaces/model/functions.py` & `MindsDB-23.5.4.1/mindsdb/interfaces/model/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/interfaces/model/model_controller.py` & `MindsDB-23.5.4.1/mindsdb/interfaces/model/model_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from mindsdb.interfaces.model.functions import (
     get_model_record,
     get_model_records
 )
 from mindsdb.interfaces.storage.json import get_json_storage
 from mindsdb.interfaces.storage.model_fs import ModelStorage
 from mindsdb.utilities.context import context as ctx
+from mindsdb.utilities.functions import resolve_model_identifier
 
 IS_PY36 = sys.version_info[1] <= 6
 
 
 class ModelController():
     config: Config
     fs_store: FsStore
@@ -409,30 +410,29 @@
         for m in models:
             if m.version is not None:
                 last_version = max(last_version, m.version)
 
         return last_version + 1
 
     def prepare_finetune_statement(self, statement, database_controller):
-        project_name = statement.name.parts[0].lower()
-        model_name = statement.name.parts[1].lower()
+        project_name, model_name, model_version, _describe = resolve_model_identifier(statement.name)
         data_integration_ref, fetch_data_query = self._get_data_integration_ref(statement, database_controller)
 
         label = None
         args = {}
         if statement.using is not None:
             label = statement.using.pop('tag', None)
             args = statement.using
 
         join_learn_process = args.pop('join_learn_process', False)
 
         base_predictor_record = get_model_record(
             name=model_name,
             project_name=project_name,
-            active=True
+            version=model_version
         )
         version = self._get_retrain_finetune_version(model_name, project_name, base_predictor_record)
 
         if data_integration_ref is None:
             data_integration_ref = base_predictor_record.data_integration_ref
         if fetch_data_query is None:
             fetch_data_query = base_predictor_record.fetch_data_query
```

### Comparing `MindsDB-23.5.3.2/mindsdb/interfaces/storage/db.py` & `MindsDB-23.5.4.1/mindsdb/interfaces/storage/db.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/interfaces/storage/fs.py` & `MindsDB-23.5.4.1/mindsdb/interfaces/storage/fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/interfaces/storage/json.py` & `MindsDB-23.5.4.1/mindsdb/interfaces/storage/json.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/interfaces/storage/model_fs.py` & `MindsDB-23.5.4.1/mindsdb/interfaces/storage/model_fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/interfaces/stream/base/integration.py` & `MindsDB-23.5.4.1/mindsdb/interfaces/stream/base/integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/interfaces/stream/kafka/kafkadb.py` & `MindsDB-23.5.4.1/mindsdb/interfaces/stream/kafka/kafkadb.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/interfaces/stream/redis/redisdb.py` & `MindsDB-23.5.4.1/mindsdb/interfaces/stream/redis/redisdb.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/interfaces/stream/stream.py` & `MindsDB-23.5.4.1/mindsdb/interfaces/stream/stream.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/microservices_grpc/db/common_pb2.py` & `MindsDB-23.5.4.1/mindsdb/microservices_grpc/db/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/microservices_grpc/db/db_pb2.py` & `MindsDB-23.5.4.1/mindsdb/microservices_grpc/db/db_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/microservices_grpc/db/db_pb2_grpc.py` & `MindsDB-23.5.4.1/mindsdb/microservices_grpc/db/db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/microservices_grpc/executor/executor_pb2.py` & `MindsDB-23.5.4.1/mindsdb/microservices_grpc/executor/executor_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py` & `MindsDB-23.5.4.1/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/microservices_grpc/ml/common_pb2.py` & `MindsDB-23.5.4.1/mindsdb/microservices_grpc/ml/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/microservices_grpc/ml/ml_pb2.py` & `MindsDB-23.5.4.1/mindsdb/microservices_grpc/ml/ml_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py` & `MindsDB-23.5.4.1/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/alembic.ini` & `MindsDB-23.5.4.1/mindsdb/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/env.py` & `MindsDB-23.5.4.1/mindsdb/migrations/env.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/migrate.py` & `MindsDB-23.5.4.1/mindsdb/migrations/migrate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py` & `MindsDB-23.5.4.1/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/utilities/auth.py` & `MindsDB-23.5.4.1/mindsdb/utilities/auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/utilities/cache.py` & `MindsDB-23.5.4.1/mindsdb/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/utilities/config.py` & `MindsDB-23.5.4.1/mindsdb/utilities/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/utilities/context.py` & `MindsDB-23.5.4.1/mindsdb/utilities/context.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/utilities/hooks/profiling.py` & `MindsDB-23.5.4.1/mindsdb/utilities/hooks/profiling.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/utilities/json_encoder.py` & `MindsDB-23.5.4.1/mindsdb/utilities/json_encoder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/utilities/log.py` & `MindsDB-23.5.4.1/mindsdb/utilities/log.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/utilities/log_controller.py` & `MindsDB-23.5.4.1/mindsdb/utilities/log_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/utilities/profiler/profiler.py` & `MindsDB-23.5.4.1/mindsdb/utilities/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/utilities/ps.py` & `MindsDB-23.5.4.1/mindsdb/utilities/ps.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/utilities/telemetry.py` & `MindsDB-23.5.4.1/mindsdb/utilities/telemetry.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/mindsdb/utilities/wizards.py` & `MindsDB-23.5.4.1/mindsdb/utilities/wizards.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/requirements.txt` & `MindsDB-23.5.4.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.3.2/setup.py` & `MindsDB-23.5.4.1/setup.py`

 * *Files identical despite different names*

