# Comparing `tmp/oteapi-core-0.4.2.tar.gz` & `tmp/oteapi-core-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oteapi-core-0.4.2.tar", last modified: Fri May 12 13:38:49 2023, max compression
+gzip compressed data, was "oteapi-core-0.4.3.tar", last modified: Tue May 23 15:08:14 2023, max compression
```

## Comparing `oteapi-core-0.4.2.tar` & `oteapi-core-0.4.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.904651 oteapi-core-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-05-12 13:38:49.904651 oteapi-core-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.896651 oteapi-core-0.4.2/oteapi/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-12 13:38:46.000000 oteapi-core-0.4.2/oteapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.896651 oteapi-core-0.4.2/oteapi/datacache/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/datacache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/datacache/datacache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.896651 oteapi-core-0.4.2/oteapi/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/interfaces/idownloadstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/interfaces/ifilterstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/interfaces/ifunctionstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/interfaces/imappingstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/interfaces/iparsestrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/interfaces/iresourcestrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/interfaces/itransformationstrategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.900651 oteapi-core-0.4.2/oteapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/datacacheconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/filterconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/functionconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/genericconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/mappingconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/resourceconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/secretconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/sessionupdate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/transformationconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/triplestoreconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.900651 oteapi-core-0.4.2/oteapi/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/plugins/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/plugins/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.900651 oteapi-core-0.4.2/oteapi/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.900651 oteapi-core-0.4.2/oteapi/strategies/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/download/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/download/https.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/download/sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.900651 oteapi-core-0.4.2/oteapi/strategies/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/filter/crop_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/filter/sql_query_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.900651 oteapi-core-0.4.2/oteapi/strategies/mapping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/mapping/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.900651 oteapi-core-0.4.2/oteapi/strategies/parse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/parse/application_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/parse/application_vnd_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/parse/excel_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/parse/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/parse/text_csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.900651 oteapi-core-0.4.2/oteapi/strategies/transformation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/transformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/transformation/celery_remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.900651 oteapi-core-0.4.2/oteapi/triplestore/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/triplestore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/triplestore/triplestore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.900651 oteapi-core-0.4.2/oteapi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/utils/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.904651 oteapi-core-0.4.2/oteapi_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-05-12 13:38:49.000000 oteapi-core-0.4.2/oteapi_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-12 13:38:49.000000 oteapi-core-0.4.2/oteapi_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:38:49.000000 oteapi-core-0.4.2/oteapi_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-12 13:38:49.000000 oteapi-core-0.4.2/oteapi_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-12 13:38:49.000000 oteapi-core-0.4.2/oteapi_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 13:38:49.000000 oteapi-core-0.4.2/oteapi_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-12 13:38:49.904651 oteapi-core-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:08:14.845792 oteapi-core-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-05-23 15:08:14.845792 oteapi-core-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:08:14.833792 oteapi-core-0.4.3/oteapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-23 15:08:11.000000 oteapi-core-0.4.3/oteapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:08:14.833792 oteapi-core-0.4.3/oteapi/datacache/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/datacache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/datacache/datacache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:08:14.837792 oteapi-core-0.4.3/oteapi/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/interfaces/idownloadstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/interfaces/ifilterstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/interfaces/ifunctionstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/interfaces/imappingstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/interfaces/iparsestrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/interfaces/iresourcestrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/interfaces/itransformationstrategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:08:14.837792 oteapi-core-0.4.3/oteapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/models/datacacheconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/models/filterconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/models/functionconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/models/genericconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/models/mappingconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/models/resourceconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/models/secretconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/models/sessionupdate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/models/transformationconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/models/triplestoreconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:08:14.841792 oteapi-core-0.4.3/oteapi/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/plugins/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/plugins/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:08:14.841792 oteapi-core-0.4.3/oteapi/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/strategies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:08:14.841792 oteapi-core-0.4.3/oteapi/strategies/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/strategies/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/strategies/download/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/strategies/download/https.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/strategies/download/sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:08:14.841792 oteapi-core-0.4.3/oteapi/strategies/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/strategies/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/strategies/filter/crop_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/strategies/filter/sql_query_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:08:14.841792 oteapi-core-0.4.3/oteapi/strategies/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/strategies/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/strategies/mapping/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:08:14.841792 oteapi-core-0.4.3/oteapi/strategies/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/strategies/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/strategies/parse/application_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/strategies/parse/application_vnd_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/strategies/parse/excel_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/strategies/parse/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/strategies/parse/text_csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:08:14.845792 oteapi-core-0.4.3/oteapi/strategies/transformation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/strategies/transformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/strategies/transformation/celery_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:08:14.845792 oteapi-core-0.4.3/oteapi/triplestore/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/triplestore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/triplestore/triplestore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:08:14.845792 oteapi-core-0.4.3/oteapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/oteapi/utils/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:08:14.845792 oteapi-core-0.4.3/oteapi_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-05-23 15:08:14.000000 oteapi-core-0.4.3/oteapi_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-23 15:08:14.000000 oteapi-core-0.4.3/oteapi_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:08:14.000000 oteapi-core-0.4.3/oteapi_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-23 15:08:14.000000 oteapi-core-0.4.3/oteapi_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-23 15:08:14.000000 oteapi-core-0.4.3/oteapi_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 15:08:14.000000 oteapi-core-0.4.3/oteapi_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-23 15:08:14.845792 oteapi-core-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-23 15:07:04.000000 oteapi-core-0.4.3/setup.py
```

### Comparing `oteapi-core-0.4.2/LICENSE` & `oteapi-core-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/PKG-INFO` & `oteapi-core-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oteapi-core
-Version: 0.4.2
+Version: 0.4.3
 Summary: Open Translation Environment (OTE) API.
 Home-page: https://github.com/EMMC-ASBL/oteapi-core
 Author: SINTEF
 Author-email: Team4.0@SINTEF.no
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `oteapi-core-0.4.2/README.md` & `oteapi-core-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/datacache/datacache.py` & `oteapi-core-0.4.3/oteapi/datacache/datacache.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/interfaces/__init__.py` & `oteapi-core-0.4.3/oteapi/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/interfaces/idownloadstrategy.py` & `oteapi-core-0.4.3/oteapi/interfaces/idownloadstrategy.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/interfaces/ifilterstrategy.py` & `oteapi-core-0.4.3/oteapi/interfaces/ifilterstrategy.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/interfaces/ifunctionstrategy.py` & `oteapi-core-0.4.3/oteapi/interfaces/ifunctionstrategy.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/interfaces/imappingstrategy.py` & `oteapi-core-0.4.3/oteapi/interfaces/imappingstrategy.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/interfaces/iparsestrategy.py` & `oteapi-core-0.4.3/oteapi/interfaces/iparsestrategy.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/interfaces/iresourcestrategy.py` & `oteapi-core-0.4.3/oteapi/interfaces/iresourcestrategy.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/interfaces/itransformationstrategy.py` & `oteapi-core-0.4.3/oteapi/interfaces/itransformationstrategy.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/models/__init__.py` & `oteapi-core-0.4.3/oteapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/models/datacacheconfig.py` & `oteapi-core-0.4.3/oteapi/models/datacacheconfig.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/models/filterconfig.py` & `oteapi-core-0.4.3/oteapi/models/filterconfig.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/models/genericconfig.py` & `oteapi-core-0.4.3/oteapi/models/genericconfig.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/models/mappingconfig.py` & `oteapi-core-0.4.3/oteapi/models/mappingconfig.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/models/resourceconfig.py` & `oteapi-core-0.4.3/oteapi/models/resourceconfig.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/models/secretconfig.py` & `oteapi-core-0.4.3/oteapi/models/secretconfig.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/models/transformationconfig.py` & `oteapi-core-0.4.3/oteapi/models/transformationconfig.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/models/triplestoreconfig.py` & `oteapi-core-0.4.3/oteapi/models/triplestoreconfig.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/plugins/entry_points.py` & `oteapi-core-0.4.3/oteapi/plugins/entry_points.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/plugins/factories.py` & `oteapi-core-0.4.3/oteapi/plugins/factories.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/settings.py` & `oteapi-core-0.4.3/oteapi/settings.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/strategies/download/file.py` & `oteapi-core-0.4.3/oteapi/strategies/download/file.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/strategies/download/https.py` & `oteapi-core-0.4.3/oteapi/strategies/download/https.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/strategies/download/sftp.py` & `oteapi-core-0.4.3/oteapi/strategies/download/sftp.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/strategies/filter/crop_filter.py` & `oteapi-core-0.4.3/oteapi/strategies/filter/crop_filter.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/strategies/filter/sql_query_filter.py` & `oteapi-core-0.4.3/oteapi/strategies/filter/sql_query_filter.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/strategies/mapping/mapping.py` & `oteapi-core-0.4.3/oteapi/strategies/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/strategies/parse/application_json.py` & `oteapi-core-0.4.3/oteapi/strategies/parse/application_json.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/strategies/parse/application_vnd_sqlite.py` & `oteapi-core-0.4.3/oteapi/strategies/parse/application_vnd_sqlite.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/strategies/parse/excel_xlsx.py` & `oteapi-core-0.4.3/oteapi/strategies/parse/excel_xlsx.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/strategies/parse/image.py` & `oteapi-core-0.4.3/oteapi/strategies/parse/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 """Strategy class for image/jpg."""
 # pylint: disable=unused-argument
+import sys
 from enum import Enum
-from typing import TYPE_CHECKING, Literal, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Optional, Tuple
+
+if sys.version_info >= (3, 10):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
 
 import numpy as np
 from PIL import Image
 from pydantic import Field
 from pydantic.dataclasses import dataclass
 
 from oteapi.datacache import DataCache
@@ -45,22 +51,22 @@
         ),
     )
 
 
 class ImageParserResourceConfig(ResourceConfig):
     """Image parse strategy resource config."""
 
-    mediaType: Union[
-        Literal["image/jpg"],
-        Literal["image/jpeg"],
-        Literal["image/jp2"],
-        Literal["image/png"],
-        Literal["image/gif"],
-        Literal["image/tiff"],
-        Literal["image/eps"],
+    mediaType: Literal[
+        "image/jpg",
+        "image/jpeg",
+        "image/jp2",
+        "image/png",
+        "image/gif",
+        "image/tiff",
+        "image/eps",
     ] = Field(
         ...,
         description=ResourceConfig.__fields__["mediaType"].field_info.description,
     )
     configuration: ImageParserConfig = Field(
         ImageParserConfig(),
         description="Image parse strategy-specific configuration.",
```

### Comparing `oteapi-core-0.4.2/oteapi/strategies/parse/text_csv.py` & `oteapi-core-0.4.3/oteapi/strategies/parse/text_csv.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/strategies/transformation/celery_remote.py` & `oteapi-core-0.4.3/oteapi/strategies/transformation/celery_remote.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/triplestore/triplestore.py` & `oteapi-core-0.4.3/oteapi/triplestore/triplestore.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi/utils/paths.py` & `oteapi-core-0.4.3/oteapi/utils/paths.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi_core.egg-info/PKG-INFO` & `oteapi-core-0.4.3/oteapi_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oteapi-core
-Version: 0.4.2
+Version: 0.4.3
 Summary: Open Translation Environment (OTE) API.
 Home-page: https://github.com/EMMC-ASBL/oteapi-core
 Author: SINTEF
 Author-email: Team4.0@SINTEF.no
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `oteapi-core-0.4.2/oteapi_core.egg-info/SOURCES.txt` & `oteapi-core-0.4.3/oteapi_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi_core.egg-info/entry_points.txt` & `oteapi-core-0.4.3/oteapi_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/oteapi_core.egg-info/requires.txt` & `oteapi-core-0.4.3/oteapi_core.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 fastapi-plugins~=0.12.0
 numpy<2,>=1.21
 openpyxl<4,>=3.0.9
 Pillow<10,>=9.0.0
 pydantic<2,>=1.9.0
 pysftp~=0.2.9
 requests<3,>=2.26.0
+typing-extensions~=4.6
 urllib3<2
 
 [dev]
 pylint~=2.17
 pytest~=7.3
 pytest-celery
 pytest-cov~=4.0
```

### Comparing `oteapi-core-0.4.2/pyproject.toml` & `oteapi-core-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/setup.cfg` & `oteapi-core-0.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.2/setup.py` & `oteapi-core-0.4.3/setup.py`

 * *Files identical despite different names*

