# Comparing `tmp/jupyterlab_sql_editor-0.1.63.tar.gz` & `tmp/jupyterlab_sql_editor-0.1.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_sql_editor-0.1.63.tar", last modified: Wed May 10 18:41:39 2023, max compression
+gzip compressed data, was "jupyterlab_sql_editor-0.1.64.tar", last modified: Tue May 23 16:31:50 2023, max compression
```

## Comparing `jupyterlab_sql_editor-0.1.63.tar` & `jupyterlab_sql_editor-0.1.64.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-10 18:41:39.961706 jupyterlab_sql_editor-0.1.63/
--rw-r--r--   0 vsts      (1001) docker     (123)     1074 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      472 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     8103 2023-05-10 18:41:39.961706 jupyterlab_sql_editor-0.1.63/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     6834 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1905 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/RELEASE.md
--rw-r--r--   0 vsts      (1001) docker     (123)      203 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/install.json
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-10 18:41:39.953705 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/
--rw-r--r--   0 vsts      (1001) docker     (123)      261 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      471 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/_version.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-10 18:41:39.953705 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython/
--rw-r--r--   0 vsts      (1001) docker     (123)     3125 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython/SparkSchemaWidget.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8098 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython/balls_line.gif
--rw-r--r--   0 vsts      (1001) docker     (123)     3958 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython/common.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8623 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython/spark_streaming_query.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7667 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython/sparkdf.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-10 18:41:39.953705 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-10 18:41:39.953705 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/common/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/common/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4621 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/common/base.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9263 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/common/export.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-10 18:41:39.953705 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/sparksql/
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/sparksql/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1768 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/sparksql/main.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4722 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/sparksql/spark_export.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10706 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/sparksql/sparksql.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-10 18:41:39.957705 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/trino/
--rw-r--r--   0 vsts      (1001) docker     (123)       99 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/trino/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1750 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/trino/main.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5389 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/trino/parser.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7418 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/trino/parser_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)    35548 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/trino/parsetab.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9992 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/trino/trino.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3539 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/trino/trino_export.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-10 18:41:39.957705 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/
--rw-r--r--   0 vsts      (1001) docker     (123)    21458 2023-05-10 18:41:16.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/build_log.json
--rw-r--r--   0 vsts      (1001) docker     (123)     4683 2023-05-10 18:41:17.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/package.json
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-10 18:41:39.949705 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/schemas/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-10 18:41:39.957705 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/
--rw-r--r--   0 vsts      (1001) docker     (123)     4541 2023-05-10 18:41:16.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/package.json.orig
--rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-05-10 18:41:16.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/plugin.json
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-10 18:41:39.957705 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/
--rw-r--r--   0 vsts      (1001) docker     (123)    23427 2023-05-10 18:41:17.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js
--rw-r--r--   0 vsts      (1001) docker     (123)    31873 2023-05-10 18:41:17.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js.map
--rw-r--r--   0 vsts      (1001) docker     (123)    29515 2023-05-10 18:41:17.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/remoteEntry.84edd756b78db1078f1a.js
--rw-r--r--   0 vsts      (1001) docker     (123)    28397 2023-05-10 18:41:17.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/remoteEntry.84edd756b78db1078f1a.js.map
--rw-r--r--   0 vsts      (1001) docker     (123)      164 2023-05-10 18:41:16.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/style.js
--rw-r--r--   0 vsts      (1001) docker     (123)     4266 2023-05-10 18:41:17.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js
--rw-r--r--   0 vsts      (1001) docker     (123)     1437 2023-05-10 18:41:17.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js.map
--rw-r--r--   0 vsts      (1001) docker     (123)    12072 2023-05-10 18:41:17.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js
--rw-r--r--   0 vsts      (1001) docker     (123)    13811 2023-05-10 18:41:17.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js.map
--rw-r--r--   0 vsts      (1001) docker     (123)   361933 2023-05-10 18:41:17.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js
--rw-r--r--   0 vsts      (1001) docker     (123)   485462 2023-05-10 18:41:17.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js.map
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-10 18:41:39.953705 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     8103 2023-05-10 18:41:39.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     3163 2023-05-10 18:41:39.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-10 18:41:39.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      357 2023-05-10 18:41:39.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-10 18:39:59.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       68 2023-05-10 18:41:39.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       22 2023-05-10 18:41:39.000000 jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-10 18:41:39.961706 jupyterlab_sql_editor-0.1.63/overrides/
--rw-r--r--   0 vsts      (1001) docker     (123)      676 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/overrides/sparksql-lsp.json
--rw-r--r--   0 vsts      (1001) docker     (123)       91 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/overrides/syntax_highlighting.json
--rw-r--r--   0 vsts      (1001) docker     (123)      671 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/overrides/trino-lsp.json
--rw-r--r--   0 vsts      (1001) docker     (123)     4541 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/package.json
--rw-r--r--   0 vsts      (1001) docker     (123)      619 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/pyproject.toml
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-10 18:41:39.961706 jupyterlab_sql_editor-0.1.63/schema/
--rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/schema/plugin.json
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-10 18:41:39.961706 jupyterlab_sql_editor-0.1.63/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     3876 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-10 18:41:39.961706 jupyterlab_sql_editor-0.1.63/src/
--rw-r--r--   0 vsts      (1001) docker     (123)      362 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/src/constants.ts
--rw-r--r--   0 vsts      (1001) docker     (123)     8368 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/src/formatter.ts
--rw-r--r--   0 vsts      (1001) docker     (123)     6249 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/src/index.ts
--rw-r--r--   0 vsts      (1001) docker     (123)     3429 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/src/utils.ts
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-10 18:41:39.961706 jupyterlab_sql_editor-0.1.63/style/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/style/base.css
--rw-r--r--   0 vsts      (1001) docker     (123)       25 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/style/index.css
--rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/style/index.js
--rw-r--r--   0 vsts      (1001) docker     (123)      554 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/tsconfig.json
--rw-r--r--   0 vsts      (1001) docker     (123)   325438 2023-05-10 18:39:14.000000 jupyterlab_sql_editor-0.1.63/yarn.lock
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-23 16:31:50.560449 jupyterlab_sql_editor-0.1.64/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1074 2023-05-23 16:29:03.000000 jupyterlab_sql_editor-0.1.64/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)      472 2023-05-23 16:29:03.000000 jupyterlab_sql_editor-0.1.64/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     8197 2023-05-23 16:31:50.560449 jupyterlab_sql_editor-0.1.64/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     6928 2023-05-23 16:29:03.000000 jupyterlab_sql_editor-0.1.64/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1905 2023-05-23 16:29:03.000000 jupyterlab_sql_editor-0.1.64/RELEASE.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      203 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/install.json
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-23 16:31:50.548449 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/
+-rw-r--r--   0 vsts      (1001) docker     (123)      261 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      471 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/_version.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-23 16:31:50.548449 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3125 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython/SparkSchemaWidget.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8098 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython/balls_line.gif
+-rw-r--r--   0 vsts      (1001) docker     (123)     4785 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython/common.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8623 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython/spark_streaming_query.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7805 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython/sparkdf.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-23 16:31:50.548449 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-23 16:31:50.548449 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/common/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/common/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4621 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/common/base.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9263 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/common/export.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-23 16:31:50.552449 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/sparksql/
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/sparksql/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1768 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/sparksql/main.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4722 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/sparksql/spark_export.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10703 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/sparksql/sparksql.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-23 16:31:50.552449 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/trino/
+-rw-r--r--   0 vsts      (1001) docker     (123)       99 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/trino/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1750 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/trino/main.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5389 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/trino/parser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7418 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/trino/parser_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    35548 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/trino/parsetab.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10313 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/trino/trino.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3539 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/trino/trino_export.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-23 16:31:50.552449 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/
+-rw-r--r--   0 vsts      (1001) docker     (123)    21040 2023-05-23 16:31:21.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/build_log.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     4029 2023-05-23 16:31:22.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/package.json
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-23 16:31:50.544448 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/schemas/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-23 16:31:50.552449 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3887 2023-05-23 16:31:21.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/package.json.orig
+-rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-05-23 16:31:21.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/plugin.json
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-23 16:31:50.556449 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/
+-rw-r--r--   0 vsts      (1001) docker     (123)    23411 2023-05-23 16:31:22.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js
+-rw-r--r--   0 vsts      (1001) docker     (123)    31873 2023-05-23 16:31:22.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js.map
+-rw-r--r--   0 vsts      (1001) docker     (123)    29612 2023-05-23 16:31:22.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/remoteEntry.f9d09d2e2aeaf511a32b.js
+-rw-r--r--   0 vsts      (1001) docker     (123)    28460 2023-05-23 16:31:22.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/remoteEntry.f9d09d2e2aeaf511a32b.js.map
+-rw-r--r--   0 vsts      (1001) docker     (123)      164 2023-05-23 16:31:21.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/style.js
+-rw-r--r--   0 vsts      (1001) docker     (123)     4266 2023-05-23 16:31:22.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js
+-rw-r--r--   0 vsts      (1001) docker     (123)     1437 2023-05-23 16:31:22.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js.map
+-rw-r--r--   0 vsts      (1001) docker     (123)    12072 2023-05-23 16:31:22.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js
+-rw-r--r--   0 vsts      (1001) docker     (123)    13811 2023-05-23 16:31:22.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js.map
+-rw-r--r--   0 vsts      (1001) docker     (123)   361933 2023-05-23 16:31:22.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js
+-rw-r--r--   0 vsts      (1001) docker     (123)   485462 2023-05-23 16:31:22.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js.map
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-23 16:31:50.548449 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     8197 2023-05-23 16:31:50.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     3163 2023-05-23 16:31:50.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-23 16:31:50.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      357 2023-05-23 16:31:50.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-23 16:30:03.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       78 2023-05-23 16:31:50.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       22 2023-05-23 16:31:50.000000 jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-23 16:31:50.556449 jupyterlab_sql_editor-0.1.64/overrides/
+-rw-r--r--   0 vsts      (1001) docker     (123)      676 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/overrides/sparksql-lsp.json
+-rw-r--r--   0 vsts      (1001) docker     (123)       91 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/overrides/syntax_highlighting.json
+-rw-r--r--   0 vsts      (1001) docker     (123)      671 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/overrides/trino-lsp.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     3887 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/package.json
+-rw-r--r--   0 vsts      (1001) docker     (123)      619 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/pyproject.toml
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-23 16:31:50.556449 jupyterlab_sql_editor-0.1.64/schema/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/schema/plugin.json
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-23 16:31:50.560449 jupyterlab_sql_editor-0.1.64/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3960 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-23 16:31:50.556449 jupyterlab_sql_editor-0.1.64/src/
+-rw-r--r--   0 vsts      (1001) docker     (123)      362 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/src/constants.ts
+-rw-r--r--   0 vsts      (1001) docker     (123)     8368 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/src/formatter.ts
+-rw-r--r--   0 vsts      (1001) docker     (123)     6249 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/src/index.ts
+-rw-r--r--   0 vsts      (1001) docker     (123)     3429 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/src/utils.ts
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-23 16:31:50.556449 jupyterlab_sql_editor-0.1.64/style/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/style/base.css
+-rw-r--r--   0 vsts      (1001) docker     (123)       25 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/style/index.css
+-rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/style/index.js
+-rw-r--r--   0 vsts      (1001) docker     (123)      554 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/tsconfig.json
+-rw-r--r--   0 vsts      (1001) docker     (123)   228103 2023-05-23 16:29:04.000000 jupyterlab_sql_editor-0.1.64/yarn.lock
```

### Comparing `jupyterlab_sql_editor-0.1.63/LICENSE` & `jupyterlab_sql_editor-0.1.64/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/PKG-INFO` & `jupyterlab_sql_editor-0.1.64/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_sql_editor
-Version: 0.1.63
+Version: 0.1.64
 Summary: SQL editor support for formatting, syntax highlighting and code completion of SQL in cell magic, line magic, python string and file editor.
 Home-page: https://github.com/CybercentreCanada/jupyterlab-sql-editor
 Author: cccs-jc
 Author-email: contact@cyber.gc.ca
 License: MIT License (MIT)
 Keywords: sql,Jupyter,JupyterLab,JupyterLab3,jupyter,jupyterlab-extension,spark,trino,dataframe,cccs,canada
 Platform: Linux
@@ -114,15 +114,15 @@
 |`--database NAME`|Spark database to use.|
 |`-l LIMIT` `--limit LIMIT`|The maximum number of rows to display. A value of zero is equivalent to `--output skip`|
 |`-r all\|local\|none` `--refresh all\|local\|none`|Force the regeneration of the schema cache file. The `local` option will only update tables/views created in the local Spark context.|
 |`-d NAME` `--dataframe NAME`|Capture dataframe in a local variable named `NAME`.|
 |`-c` `--cache`|Cache dataframe.|
 |`-e` `--eager`|Cache dataframe with eager load.|
 |`-v VIEW` `--view VIEW`|Create or replace a temporary view named `VIEW`.|
-|`-o sql\|json\|html\|grid\|text\|schema\|skip\|none` `--output sql\|json\|html\|grid\|text\|schema\|skip\|none`|Output format. Defaults to html. The `sql` option prints the SQL statement that will be executed (useful to test jinja templated statements).|
+|`-o sql\|json\|html\|aggrid\|grid\|text\|schema\|skip\|none` `--output sql\|json\|html\|aggrid\|grid\|text\|schema\|skip\|none`|Output format. Defaults to html. The `sql` option prints the SQL statement that will be executed (useful to test jinja templated statements).|
 |`-s` `--show-nonprinting`|Replace none printable characters with their ascii codes (`LF` -> `\x0a`)|
 |`-j` `--jinja`|Enable Jinja templating support.|
 |`-b` `--dbt`|Enable DBT templating support.|
 |`-t LIMIT` `--truncate LIMIT`|Truncate output.|
 |`-m update\|complete` `--streaming_mode update\|complete`|The mode of streaming queries.|
 |`-x` `--lean-exceptions`|Shortened exceptions. Might be helpful if the exceptions reported by Spark are noisy such as with big SQL queries.|
 
@@ -130,15 +130,15 @@
 |Parameter|Description|
 |---|---|
 |`-c NAME` `--catalog NAME`|Trino catalog to use.|
 |`-s NAME` `--schema NAME`|Trino schema to use.|
 |`-l LIMIT` `--limit LIMIT`|The maximum number of rows to display. A value of zero is equivalent to `--output skip`|
 |`-r all\|none` `--refresh all\|none`|Force the regeneration of the schema cache file.|
 |`-d NAME` `--dataframe NAME`|Capture dataframe in a local variable named `NAME`.|
-|`-o sql\|json\|html\|grid\|text\|schema\|skip\|none` `--output sql\|json\|html\|grid\|text\|schema\|skip\|none`|Output format. Defaults to html. The `sql` option prints the SQL statement that will be executed (useful to test jinja templated statements).|
+|`-o sql\|json\|html\|aggrid\|grid\|text\|schema\|skip\|none` `--output sql\|json\|html\|aggrid\|grid\|text\|schema\|skip\|none`|Output format. Defaults to html. The `sql` option prints the SQL statement that will be executed (useful to test jinja templated statements).|
 |`-s` `--show-nonprinting`|Replace none printable characters with their ascii codes (`LF` -> `\x0a`).|
 |`-j` `--jinja`|Enable Jinja templating support.|
 |`-t LIMIT` `--truncate LIMIT`|Truncate output.|
 |`-x STATEMENT` `--raw STATEMENT`|Run statement as is. Do not wrap statement with a limit. Use this option to run statement which can't be wrapped in a SELECT/LIMIT statement. For example EXPLAIN, SHOW TABLE, SHOW CATALOGS.|
 
 ## Security Vulnerability Reporting
 
@@ -160,7 +160,8 @@
 
 - [krassowski/jupyterlab-lsp](https://github.com/jupyter-lsp/jupyterlab-lsp)
 - [joe-re/sql-language-server](https://github.com/joe-re/sql-language-server)
 - [zeroturnaround/sql-formatter](https://github.com/zeroturnaround/sql-formatter)
 - [cryeo/sparksql-magic](https://github.com/cryeo/sparksql-magic)
 - [trino-python-client](https://github.com/trinodb/trino-python-client)
 - [bloomberg/ipydatagrid](https://github.com/bloomberg/ipydatagrid)
+- [widgetti/ipyaggrid](https://github.com/widgetti/ipyaggrid)
```

### Comparing `jupyterlab_sql_editor-0.1.63/README.md` & `jupyterlab_sql_editor-0.1.64/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 |`--database NAME`|Spark database to use.|
 |`-l LIMIT` `--limit LIMIT`|The maximum number of rows to display. A value of zero is equivalent to `--output skip`|
 |`-r all\|local\|none` `--refresh all\|local\|none`|Force the regeneration of the schema cache file. The `local` option will only update tables/views created in the local Spark context.|
 |`-d NAME` `--dataframe NAME`|Capture dataframe in a local variable named `NAME`.|
 |`-c` `--cache`|Cache dataframe.|
 |`-e` `--eager`|Cache dataframe with eager load.|
 |`-v VIEW` `--view VIEW`|Create or replace a temporary view named `VIEW`.|
-|`-o sql\|json\|html\|grid\|text\|schema\|skip\|none` `--output sql\|json\|html\|grid\|text\|schema\|skip\|none`|Output format. Defaults to html. The `sql` option prints the SQL statement that will be executed (useful to test jinja templated statements).|
+|`-o sql\|json\|html\|aggrid\|grid\|text\|schema\|skip\|none` `--output sql\|json\|html\|aggrid\|grid\|text\|schema\|skip\|none`|Output format. Defaults to html. The `sql` option prints the SQL statement that will be executed (useful to test jinja templated statements).|
 |`-s` `--show-nonprinting`|Replace none printable characters with their ascii codes (`LF` -> `\x0a`)|
 |`-j` `--jinja`|Enable Jinja templating support.|
 |`-b` `--dbt`|Enable DBT templating support.|
 |`-t LIMIT` `--truncate LIMIT`|Truncate output.|
 |`-m update\|complete` `--streaming_mode update\|complete`|The mode of streaming queries.|
 |`-x` `--lean-exceptions`|Shortened exceptions. Might be helpful if the exceptions reported by Spark are noisy such as with big SQL queries.|
 
@@ -101,15 +101,15 @@
 |Parameter|Description|
 |---|---|
 |`-c NAME` `--catalog NAME`|Trino catalog to use.|
 |`-s NAME` `--schema NAME`|Trino schema to use.|
 |`-l LIMIT` `--limit LIMIT`|The maximum number of rows to display. A value of zero is equivalent to `--output skip`|
 |`-r all\|none` `--refresh all\|none`|Force the regeneration of the schema cache file.|
 |`-d NAME` `--dataframe NAME`|Capture dataframe in a local variable named `NAME`.|
-|`-o sql\|json\|html\|grid\|text\|schema\|skip\|none` `--output sql\|json\|html\|grid\|text\|schema\|skip\|none`|Output format. Defaults to html. The `sql` option prints the SQL statement that will be executed (useful to test jinja templated statements).|
+|`-o sql\|json\|html\|aggrid\|grid\|text\|schema\|skip\|none` `--output sql\|json\|html\|aggrid\|grid\|text\|schema\|skip\|none`|Output format. Defaults to html. The `sql` option prints the SQL statement that will be executed (useful to test jinja templated statements).|
 |`-s` `--show-nonprinting`|Replace none printable characters with their ascii codes (`LF` -> `\x0a`).|
 |`-j` `--jinja`|Enable Jinja templating support.|
 |`-t LIMIT` `--truncate LIMIT`|Truncate output.|
 |`-x STATEMENT` `--raw STATEMENT`|Run statement as is. Do not wrap statement with a limit. Use this option to run statement which can't be wrapped in a SELECT/LIMIT statement. For example EXPLAIN, SHOW TABLE, SHOW CATALOGS.|
 
 ## Security Vulnerability Reporting
 
@@ -131,7 +131,8 @@
 
 - [krassowski/jupyterlab-lsp](https://github.com/jupyter-lsp/jupyterlab-lsp)
 - [joe-re/sql-language-server](https://github.com/joe-re/sql-language-server)
 - [zeroturnaround/sql-formatter](https://github.com/zeroturnaround/sql-formatter)
 - [cryeo/sparksql-magic](https://github.com/cryeo/sparksql-magic)
 - [trino-python-client](https://github.com/trinodb/trino-python-client)
 - [bloomberg/ipydatagrid](https://github.com/bloomberg/ipydatagrid)
+- [widgetti/ipyaggrid](https://github.com/widgetti/ipyaggrid)
```

### Comparing `jupyterlab_sql_editor-0.1.63/RELEASE.md` & `jupyterlab_sql_editor-0.1.64/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython/SparkSchemaWidget.py` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython/SparkSchemaWidget.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython/balls_line.gif` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython/balls_line.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython/common.py` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 import re
 import string
 from html import escape
 from html import escape as html_escape
 from os import environ, listdir
 from os.path import isdir, join
 
+from ipyaggrid import Grid
 from ipydatagrid import DataGrid, TextRenderer
 
+DEFAULT_COLUMN_DEF = {"editable": False, "filter": True, "resizable": True, "sortable": True}
+
 PRINTABLE = string.ascii_letters + string.digits + string.punctuation + " "
 
 replchars = re.compile("([^" + re.escape(PRINTABLE) + "])")
 
 JS_MAX_SAFE_INTEGER = 9007199254740991
 
 JS_MIN_SAFE_INTEGER = -9007199254740991
@@ -58,14 +61,39 @@
         selection_mode="row",
         layout={"height": layout_height},
         header_renderer=TextRenderer(text_wrap=True),
         default_renderer=TextRenderer(text_wrap=True),
     )
 
 
+def render_ag_grid(pdf):
+    grid_options = {
+        "columnDefs": [
+            {"headerName": c, "field": c, "sortable": True, "enableRowGroup": True, "autoHeight": True}
+            for c in pdf.columns
+        ],
+        "defaultColDef": DEFAULT_COLUMN_DEF,
+        "enableRangeSelection": True,
+        "suppressColumnVirtualisation": True,
+        "animateRows": True,
+    }
+
+    ag_grid_license_key = environ.get("AG_GRID_LICENSE_KEY")
+
+    return Grid(
+        grid_data=pdf,
+        grid_options=grid_options,
+        quick_filter=True,
+        theme="ag-theme-balham",
+        columns_fit="auto",
+        index=False,
+        license=ag_grid_license_key if ag_grid_license_key else "",
+    )
+
+
 def replchars_to_hex(match):
     return r"\x{0:02x}".format(ord(match.group()))
 
 
 def recursive_escape(input):
     # check whether it's a dict, list, tuple, or scalar
     if isinstance(input, dict):
```

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython/spark_streaming_query.py` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython/spark_streaming_query.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython/sparkdf.py` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython/sparkdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import inspect
 import json
 import os
 from time import time
 
 import pandas as pd
-import pyspark.sql.functions as F
 from IPython import get_ipython
 from IPython.display import HTML, JSON, TextDisplayObject, display
 from ipywidgets import Output
 from pyspark.rdd import _load_from_socket
 from pyspark.serializers import BatchedSerializer, PickleSerializer
 from pyspark.sql.session import SparkSession
 
 import jupyterlab_sql_editor.ipython.spark_streaming_query as streaming
 from jupyterlab_sql_editor.ipython.common import (
     cast_unsafe_ints_to_str,
     escape_control_chars,
     recursive_escape,
+    render_ag_grid,
     render_grid,
     rows_to_html,
 )
 from jupyterlab_sql_editor.ipython.SparkSchemaWidget import SparkSchemaWidget
 
 
 def retrieve_name(var):
@@ -52,14 +52,17 @@
     """
     displays = []
     start = time()
     has_more_data = False
     if output == "grid":
         has_more_data, pdf = to_pandas(df, limit, truncate, show_nonprinting)
         displays.append(render_grid(pdf, limit))
+    elif output == "aggrid":
+        has_more_data, pdf = to_pandas(df, limit, truncate, show_nonprinting)
+        displays.append(render_ag_grid(pdf))
     elif output == "json":
         json_array = []
         warnings = []
         results = df.toJSON().map(lambda j: json.loads(j)).take(limit)
         if df.count() > limit:
             has_more_data = True
         # cast unsafe ints to str for display
```

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/common/base.py` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/common/base.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/common/export.py` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/common/export.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/sparksql/main.py` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/sparksql/main.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/sparksql/spark_export.py` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/sparksql/spark_export.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/sparksql/sparksql.py` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/sparksql/sparksql.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from jupyterlab_sql_editor.ipython.sparkdf import display_df
 from jupyterlab_sql_editor.ipython_magic.common.base import Base
 from jupyterlab_sql_editor.ipython_magic.sparksql.spark_export import (
     update_database_schema,
     update_local_database,
 )
 
-VALID_OUTPUTS = ["sql", "text", "json", "html", "grid", "schema", "skip", "none"]
+VALID_OUTPUTS = ["sql", "text", "json", "html", "aggrid", "grid", "schema", "skip", "none"]
 PYSPARK_ERROR_TYPES = (
     AnalysisException,
     IllegalArgumentException,
     ParseException,
     QueryExecutionException,
     StreamingQueryException,
 )
@@ -70,15 +70,15 @@
     @argument("-d", "--dataframe", metavar="name", type=str, help="Capture dataframe in a local variable named `name`")
     @argument("-c", "--cache", action="store_true", help="Cache dataframe")
     @argument("-e", "--eager", action="store_true", help="Cache dataframe with eager load")
     @argument("-v", "--view", metavar="name", type=str, help="Create or replace a temporary view named `name`")
     @argument(
         "-o",
         "--output",
-        metavar="sql|json|html|grid|text|schema|skip|none",
+        metavar="sql|json|html|aggrid|grid|text|schema|skip|none",
         type=str,
         default="html",
         help="Output format. Defaults to html. The `sql` option prints the SQL statement that will be executed (useful to test jinja templated statements)",
     )
     @argument(
         "-s",
         "--show-nonprinting",
@@ -118,15 +118,15 @@
             truncate = args.truncate
 
         limit = args.limit
         if limit is None:
             limit = self.limit
 
         if output not in VALID_OUTPUTS:
-            print(f"Invalid output option {args.output}. The valid options are [sql|json|text|html|grid|skip|none].")
+            print(f"Invalid output option {args.output}. The valid options are {VALID_OUTPUTS}.")
             return
 
         self.spark = self.get_instantiated_spark_session()
         if self.spark is None:
             print("Active spark session is not found")
             return
```

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/trino/main.py` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/trino/main.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/trino/parser.py` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/trino/parser.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/trino/parser_test.py` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/trino/parser_test.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/trino/parsetab.py` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/trino/parsetab.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/trino/trino.py` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/trino/trino.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 from traitlets import Bool, Instance, Int, Unicode, Union
 
 from jupyterlab_sql_editor.ipython.common import (
     cast_unsafe_ints_to_str,
     escape_control_chars,
     make_tag,
     recursive_escape,
+    render_ag_grid,
     render_grid,
     rows_to_html,
 )
 from jupyterlab_sql_editor.ipython_magic.common.base import Base
 from jupyterlab_sql_editor.ipython_magic.trino.trino_export import (
     update_database_schema,
 )
 
-VALID_OUTPUTS = ["sql", "text", "json", "html", "grid", "skip", "none"]
+VALID_OUTPUTS = ["sql", "text", "json", "html", "aggrid", "grid", "skip", "none"]
 
 
 @magics_class
 class Trino(Base):
     host = Unicode("localhost", config=True, help="Trino server hostname")
     port = Int(443, config=True, help="Trino server port number")
     auth = Instance(
@@ -70,15 +71,15 @@
         default="none",
         help="Force the regeneration of the schema cache file.",
     )
     @argument("-d", "--dataframe", metavar="name", type=str, help="Capture results in pandas dataframe")
     @argument(
         "-o",
         "--output",
-        metavar="sql|json|html|grid|text|skip|none",
+        metavar="sql|json|html|aggrid|grid|text|skip|none",
         type=str,
         default="html",
         help="Output format. Defaults to html. The `sql` option prints the SQL statement that will be executed (useful to test jinja templated statements)",
     )
     @argument(
         "-s",
         "--show-nonprinting",
@@ -180,14 +181,20 @@
     def display_results(self, results, columns, output, limit=20, show_nonprinting=False, args=None):
         if output == "grid":
             pdf = pd.DataFrame.from_records(results, columns=columns)
             if show_nonprinting:
                 for c in pdf.columns:
                     pdf[c] = pdf[c].apply(lambda v: escape_control_chars(str(v)))
             display(render_grid(pdf, limit))
+        elif output == "aggrid":
+            pdf = pd.DataFrame.from_records(results, columns=columns)
+            if show_nonprinting:
+                for c in pdf.columns:
+                    pdf[c] = pdf[c].apply(lambda v: escape_control_chars(str(v)))
+            display(render_ag_grid(pdf))
         elif output == "json":
             json_array = []
             warnings = []
             json_string = pd.DataFrame.from_records(results, columns=columns).to_json(orient="records")
             json_dict = json.loads(json_string)
             # cast unsafe ints to str for display
             for row in json_dict:
@@ -207,17 +214,17 @@
             return True
         if refresh_arg != "none":
             print(f"Invalid refresh option given {refresh_arg}. Valid refresh options are [all|local|none]")
         return False
 
     @staticmethod
     def format_cell(v, output="html", truncate=256):
-        if output != "json" and len(v) > truncate:
-            v = str(v) if v is not None else "null"
-            v = v[:truncate] + "..."
+        if output != "json" and isinstance(v, str):
+            if len(v) > truncate:
+                v = v[:truncate] + "..."
         return v
 
     @staticmethod
     def render_text(rows, columns):
         string_builder = ""
         num_cols = len(columns)
         # We set a minimum column width at '3'
```

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/ipython_magic/trino/trino_export.py` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/ipython_magic/trino/trino_export.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/build_log.json` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/build_log.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998534572879332%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'@jupyterlab/application': {'requiredVersion': "*

 * *      "'^3.6.1'}, '@jupyterlab/application-extension': {'requiredVersion': '^3.6.1'}, "*

 * *      "'@jupyterlab/apputils-extension': {'requiredVersion': '^3.6.1'}, "*

 * *      "'@jupyterlab/cell-toolbar-extension': {'requiredVersion': '^3.6.1'}, "*

 * *      "'@jupyterlab/celltags-extension': {'requiredVersion': '^3.6.1'}, "*

 * *      "'@jupyterlab/codemirror-extension': {'requiredVersion': '^3.6.1'}, "*

 * *      "'@jupyterlab/colla […]*

```diff
@@ -119,446 +119,440 @@
                         ],
                         "type": "var"
                     },
                     "name": "jupyterlab-sql-editor",
                     "shared": {
                         "@jupyter/ydoc": {
                             "import": false,
-                            "requiredVersion": "^0.2.3",
+                            "requiredVersion": "^0.2.0",
                             "singleton": true
                         },
                         "@jupyterlab/application": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/application-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/apputils": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/apputils-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/attachments": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
-                        "@jupyterlab/builder": {},
                         "@jupyterlab/cell-toolbar": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/cell-toolbar-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/cells": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/celltags": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/celltags-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/codeeditor": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/collaboration": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/collaboration-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/completer": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/completer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/console": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/console-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/coreutils": {
                             "import": false,
-                            "requiredVersion": "^5.6.3",
+                            "requiredVersion": "^5.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/csvviewer": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/csvviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/debugger": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/debugger-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/docmanager": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/docmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/docprovider": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/docprovider-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/docregistry": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/documentsearch": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/documentsearch-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/extensionmanager": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/extensionmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/filebrowser": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/filebrowser-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/fileeditor": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/fileeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/help-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/htmlviewer": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/htmlviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/hub-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/imageviewer": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/imageviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/inspector": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/inspector-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/javascript-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/json-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/launcher": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/launcher-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/logconsole": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/logconsole-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/mainmenu": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/mainmenu-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/markdownviewer": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/markdownviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/mathjax2": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/mathjax2-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/metapackage": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/nbconvert-css": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/nbformat": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/notebook": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/notebook-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/observables": {
                             "import": false,
-                            "requiredVersion": "^4.6.3"
+                            "requiredVersion": "^4.6.1"
                         },
                         "@jupyterlab/outputarea": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/pdf-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/property-inspector": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/rendermime": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/rendermime-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/rendermime-interfaces": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/running": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/running-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/services": {
                             "import": false,
-                            "requiredVersion": "^6.6.3",
+                            "requiredVersion": "^6.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/settingregistry": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
-                            "singleton": true
-                        },
-                        "@jupyterlab/shared-models": {
-                            "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/shortcuts-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/statedb": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/terminal": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/terminal-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/theme-dark-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/theme-light-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/toc": {
                             "import": false,
-                            "requiredVersion": "^5.6.3",
+                            "requiredVersion": "^5.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/toc-extension": {
                             "import": false,
-                            "requiredVersion": "^5.6.3"
+                            "requiredVersion": "^5.6.1"
                         },
                         "@jupyterlab/tooltip": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/tooltip-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/translation": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/translation-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/ui-components": {
                             "import": false,
-                            "requiredVersion": "^3.6.3",
+                            "requiredVersion": "^3.6.1",
                             "singleton": true
                         },
                         "@jupyterlab/ui-components-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/vdom": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/vdom-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/vega5-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.3"
+                            "requiredVersion": "^3.6.1"
                         },
                         "@krassowski/jupyterlab-lsp": {
                             "import": false,
                             "singleton": true
                         },
                         "@lumino/algorithm": {
                             "import": false,
                             "requiredVersion": "^1.9.0",
                             "singleton": true
                         },
                         "@lumino/application": {
                             "import": false,
-                            "requiredVersion": "^1.31.4",
+                            "requiredVersion": "^1.31.3",
                             "singleton": true
                         },
                         "@lumino/commands": {
                             "import": false,
                             "requiredVersion": "^1.19.0",
                             "singleton": true
                         },
@@ -600,41 +594,36 @@
                         "@lumino/virtualdom": {
                             "import": false,
                             "requiredVersion": "^1.14.0",
                             "singleton": true
                         },
                         "@lumino/widgets": {
                             "import": false,
-                            "requiredVersion": "^1.37.2",
+                            "requiredVersion": "^1.37.1",
                             "singleton": true
                         },
                         "@types/codemirror": {},
-                        "json-schema": {},
+                        "codemirror": {},
                         "jupyterlab-sql-editor": {
                             "import": "/home/vsts/work/1/s/lib/index.js",
                             "singleton": true,
-                            "version": "0.1.63"
+                            "version": "0.1.64"
                         },
-                        "lsp-ws-connection": {},
                         "npm-run-all": {},
                         "react": {
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
                         },
                         "react-dom": {
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
                         },
                         "sql-formatter": {},
-                        "sql-language-server": {},
-                        "vscode-languageserver": {},
-                        "vscode-languageserver-protocol": {},
-                        "vscode-languageserver-types": {},
                         "yjs": {
                             "import": false,
                             "requiredVersion": "^13.5.17",
                             "singleton": true
                         }
                     }
                 }
```

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/package.json` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/package.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8428977272727274%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '3.6.1', '@jupyterlab/apputils': '3.6.1', "*

 * *                   "'@jupyterlab/docmanager': '3.6.1', '@jupyterlab/fileeditor': '3.6.1', "*

 * *                   "'@jupyterlab/logconsole': '3.6.1', '@jupyterlab/notebook': '3.6.1', "*

 * *                   "'@jupyterlab/settingregistry': '3.6.1', '@krassowski/jupyterlab-lsp': "*

 * *                   "'^3.10.2', '@jupyterlab/cells': '3.6.1', '@jupyterlab/codemirror': '3.6.1', "*

 * *                   "'codemirror': '~5.61.0', del […]*

```diff
@@ -3,65 +3,53 @@
         "email": "contact@cyber.gc.ca",
         "name": "cccs-jc"
     },
     "bugs": {
         "url": "https://github.com/CybercentreCanada/jupyterlab-sql-editor/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.6.0",
-        "@jupyterlab/apputils": "^3.6.0",
-        "@jupyterlab/builder": "^3.6.0",
-        "@jupyterlab/codemirror-extension": "^3.6.0",
-        "@jupyterlab/docmanager": "^3.6.0",
-        "@jupyterlab/fileeditor": "^3.6.0",
-        "@jupyterlab/logconsole": "^3.6.0",
-        "@jupyterlab/mainmenu": "^3.6.0",
-        "@jupyterlab/notebook": "^3.6.0",
-        "@jupyterlab/settingregistry": "^3.6.0",
-        "@krassowski/jupyterlab-lsp": "^3.10.1",
-        "@lumino/widgets": "^1.26.1",
+        "@jupyterlab/application": "3.6.1",
+        "@jupyterlab/apputils": "3.6.1",
+        "@jupyterlab/cells": "3.6.1",
+        "@jupyterlab/codemirror": "3.6.1",
+        "@jupyterlab/docmanager": "3.6.1",
+        "@jupyterlab/fileeditor": "3.6.1",
+        "@jupyterlab/logconsole": "3.6.1",
+        "@jupyterlab/notebook": "3.6.1",
+        "@jupyterlab/settingregistry": "3.6.1",
+        "@krassowski/jupyterlab-lsp": "^3.10.2",
         "@types/codemirror": "^5.60.5",
-        "json-schema": "^0.4.0",
-        "lsp-ws-connection": "^0.7.0",
+        "codemirror": "~5.61.0",
         "npm-run-all": "^4.1.5",
-        "sql-formatter": "6.1.2",
-        "sql-language-server": "^1.2.1",
-        "vscode-languageserver": "8.0.0-next.8",
-        "vscode-languageserver-protocol": "3.16.0-next.13",
-        "vscode-languageserver-types": "3.16.0-next.7"
+        "sql-formatter": "6.1.2"
     },
     "description": "SQL editor support for formatting, syntax highlighting and code completion of SQL in cell magic, line magic, python string and file editor.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.6.0",
-        "@types/node": "^18.11.9",
+        "@jupyterlab/builder": "3.6.1",
+        "@types/node": "~18.11.9",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
         "rimraf": "^3.0.2",
-        "stylelint": "^14.3.0",
-        "stylelint-config-prettier": "^9.0.4",
-        "stylelint-config-recommended": "^6.0.0",
-        "stylelint-config-standard": "~24.0.0",
-        "stylelint-prettier": "^2.0.0",
         "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/CybercentreCanada/jupyterlab-sql-editor",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.84edd756b78db1078f1a.js",
+            "load": "static/remoteEntry.f9d09d2e2aeaf511a32b.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_sql_editor/labextension",
         "schemaDir": "schema",
         "sharedPackages": {
             "@krassowski/jupyterlab-lsp": {
@@ -77,56 +65,53 @@
         "Spark",
         "Trino",
         "Dataframe"
     ],
     "license": "MIT License (MIT)",
     "main": "lib/index.js",
     "name": "jupyterlab-sql-editor",
-    "overrides": {
-        "lsp-ws-connection": {
-            "vscode-languageserver-protocol": "3.16.0-next.13",
-            "vscode-languageserver-types": "3.16.0-next.7"
-        }
-    },
+    "packageManager": "yarn@3.5.1",
     "repository": {
         "type": "git",
         "url": "https://github.com/CybercentreCanada/jupyterlab-sql-editor.git"
     },
     "resolutions": {
+        "@jupyterlab/cells": "3.6.1",
+        "@jupyterlab/outputarea": "3.6.1",
+        "@jupyterlab/rendermime": "3.6.1",
+        "@jupyterlab/rendermime-interfaces": "3.6.1",
         "vscode-languageserver-protocol": "3.16.0-next.13",
         "vscode-languageserver-types": "3.16.0-next.7"
     },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --sourceMap",
         "build:lib:prod": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
         "clean:labextension": "rimraf jupyterlab_sql_editor/labextension jupyterlab_sql_editor/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
-        "clean:lintcache": "rimraf .eslintcache .stylelintcache",
+        "clean:lintcache": "rimraf .eslintcache",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
-        "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
-        "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
+        "lint": "jlpm prettier && jlpm eslint",
+        "lint:check": "jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
-        "stylelint": "jlpm stylelint:check --fix",
-        "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.63"
+    "version": "0.1.64"
 }
```

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/package.json.orig` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/package.json.orig`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8432765151515152%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '3.6.1', '@jupyterlab/apputils': '3.6.1', "*

 * *                   "'@jupyterlab/docmanager': '3.6.1', '@jupyterlab/fileeditor': '3.6.1', "*

 * *                   "'@jupyterlab/logconsole': '3.6.1', '@jupyterlab/notebook': '3.6.1', "*

 * *                   "'@jupyterlab/settingregistry': '3.6.1', '@krassowski/jupyterlab-lsp': "*

 * *                   "'^3.10.2', '@jupyterlab/cells': '3.6.1', '@jupyterlab/codemirror': '3.6.1', "*

 * *                   "'codemirror': '~5.61.0', del […]*

```diff
@@ -3,53 +3,41 @@
         "email": "contact@cyber.gc.ca",
         "name": "cccs-jc"
     },
     "bugs": {
         "url": "https://github.com/CybercentreCanada/jupyterlab-sql-editor/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.6.0",
-        "@jupyterlab/apputils": "^3.6.0",
-        "@jupyterlab/builder": "^3.6.0",
-        "@jupyterlab/codemirror-extension": "^3.6.0",
-        "@jupyterlab/docmanager": "^3.6.0",
-        "@jupyterlab/fileeditor": "^3.6.0",
-        "@jupyterlab/logconsole": "^3.6.0",
-        "@jupyterlab/mainmenu": "^3.6.0",
-        "@jupyterlab/notebook": "^3.6.0",
-        "@jupyterlab/settingregistry": "^3.6.0",
-        "@krassowski/jupyterlab-lsp": "^3.10.1",
-        "@lumino/widgets": "^1.26.1",
+        "@jupyterlab/application": "3.6.1",
+        "@jupyterlab/apputils": "3.6.1",
+        "@jupyterlab/cells": "3.6.1",
+        "@jupyterlab/codemirror": "3.6.1",
+        "@jupyterlab/docmanager": "3.6.1",
+        "@jupyterlab/fileeditor": "3.6.1",
+        "@jupyterlab/logconsole": "3.6.1",
+        "@jupyterlab/notebook": "3.6.1",
+        "@jupyterlab/settingregistry": "3.6.1",
+        "@krassowski/jupyterlab-lsp": "^3.10.2",
         "@types/codemirror": "^5.60.5",
-        "json-schema": "^0.4.0",
-        "lsp-ws-connection": "^0.7.0",
+        "codemirror": "~5.61.0",
         "npm-run-all": "^4.1.5",
-        "sql-formatter": "6.1.2",
-        "sql-language-server": "^1.2.1",
-        "vscode-languageserver": "8.0.0-next.8",
-        "vscode-languageserver-protocol": "3.16.0-next.13",
-        "vscode-languageserver-types": "3.16.0-next.7"
+        "sql-formatter": "6.1.2"
     },
     "description": "SQL editor support for formatting, syntax highlighting and code completion of SQL in cell magic, line magic, python string and file editor.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.6.0",
-        "@types/node": "^18.11.9",
+        "@jupyterlab/builder": "3.6.1",
+        "@types/node": "~18.11.9",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
         "rimraf": "^3.0.2",
-        "stylelint": "^14.3.0",
-        "stylelint-config-prettier": "^9.0.4",
-        "stylelint-config-recommended": "^6.0.0",
-        "stylelint-config-standard": "~24.0.0",
-        "stylelint-prettier": "^2.0.0",
         "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
@@ -72,56 +60,53 @@
         "Spark",
         "Trino",
         "Dataframe"
     ],
     "license": "MIT License (MIT)",
     "main": "lib/index.js",
     "name": "jupyterlab-sql-editor",
-    "overrides": {
-        "lsp-ws-connection": {
-            "vscode-languageserver-protocol": "3.16.0-next.13",
-            "vscode-languageserver-types": "3.16.0-next.7"
-        }
-    },
+    "packageManager": "yarn@3.5.1",
     "repository": {
         "type": "git",
         "url": "https://github.com/CybercentreCanada/jupyterlab-sql-editor.git"
     },
     "resolutions": {
+        "@jupyterlab/cells": "3.6.1",
+        "@jupyterlab/outputarea": "3.6.1",
+        "@jupyterlab/rendermime": "3.6.1",
+        "@jupyterlab/rendermime-interfaces": "3.6.1",
         "vscode-languageserver-protocol": "3.16.0-next.13",
         "vscode-languageserver-types": "3.16.0-next.7"
     },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --sourceMap",
         "build:lib:prod": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
         "clean:labextension": "rimraf jupyterlab_sql_editor/labextension jupyterlab_sql_editor/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
-        "clean:lintcache": "rimraf .eslintcache .stylelintcache",
+        "clean:lintcache": "rimraf .eslintcache",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
-        "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
-        "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
+        "lint": "jlpm prettier && jlpm eslint",
+        "lint:check": "jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
-        "stylelint": "jlpm stylelint:check --fix",
-        "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.63"
+    "version": "0.1.64"
 }
```

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/plugin.json` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
             /***/
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
                 __webpack_require__.r(__webpack_exports__);
                 /* harmony export */
                 __webpack_require__.d(__webpack_exports__, {
                     /* harmony export */
-                    "Constants": () => ( /* binding */ Constants)
+                    Constants: () => ( /* binding */ Constants)
                     /* harmony export */
                 });
                 var Constants;
                 (function(Constants) {
                     Constants.SHORT_PLUGIN_NAME = 'jupyterlab-sql-editor';
                     Constants.FORMAT_COMMAND = `${Constants.SHORT_PLUGIN_NAME}:format_cell`;
                     Constants.FORMAT_COMMAND_DOCUMENT = `${Constants.SHORT_PLUGIN_NAME}:format_document`;
@@ -38,17 +38,17 @@
             /***/
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
                 __webpack_require__.r(__webpack_exports__);
                 /* harmony export */
                 __webpack_require__.d(__webpack_exports__, {
                     /* harmony export */
-                    "JupyterLabCodeFormatter": () => ( /* binding */ JupyterLabCodeFormatter),
+                    JupyterLabCodeFormatter: () => ( /* binding */ JupyterLabCodeFormatter),
                     /* harmony export */
-                    "SqlFormatter": () => ( /* binding */ SqlFormatter)
+                    SqlFormatter: () => ( /* binding */ SqlFormatter)
                     /* harmony export */
                 });
                 /* harmony import */
                 var _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! @jupyterlab/apputils */ "webpack/sharing/consume/default/@jupyterlab/apputils");
                 /* harmony import */
                 var _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_0__);
                 /* harmony import */
@@ -437,23 +437,23 @@
             /***/
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
                 __webpack_require__.r(__webpack_exports__);
                 /* harmony export */
                 __webpack_require__.d(__webpack_exports__, {
                     /* harmony export */
-                    "cellMagicExtractor": () => ( /* binding */ cellMagicExtractor),
+                    cellMagicExtractor: () => ( /* binding */ cellMagicExtractor),
                     /* harmony export */
-                    "lineMagicExtractor": () => ( /* binding */ lineMagicExtractor),
+                    lineMagicExtractor: () => ( /* binding */ lineMagicExtractor),
                     /* harmony export */
-                    "markerExtractor": () => ( /* binding */ markerExtractor),
+                    markerExtractor: () => ( /* binding */ markerExtractor),
                     /* harmony export */
-                    "registerCodeMirrorFor": () => ( /* binding */ registerCodeMirrorFor),
+                    registerCodeMirrorFor: () => ( /* binding */ registerCodeMirrorFor),
                     /* harmony export */
-                    "sqlCodeMirrorModesFor": () => ( /* binding */ sqlCodeMirrorModesFor)
+                    sqlCodeMirrorModesFor: () => ( /* binding */ sqlCodeMirrorModesFor)
                     /* harmony export */
                 });
                 /* harmony import */
                 var _krassowski_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! @krassowski/jupyterlab-lsp */ "webpack/sharing/consume/default/@krassowski/jupyterlab-lsp");
                 /* harmony import */
                 var _krassowski_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_krassowski_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_0__);
```

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js.map` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/remoteEntry.84edd756b78db1078f1a.js` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/remoteEntry.f9d09d2e2aeaf511a32b.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -302,15 +302,15 @@
                 /******/
                 script.parentNode && script.parentNode.removeChild(script);
                 /******/
                 doneFns && doneFns.forEach((fn) => (fn(event)));
                 /******/
                 if (prev) return prev(event);
                 /******/
-            };
+            }
             /******/
             var timeout = setTimeout(onScriptComplete.bind(null, undefined, {
                 type: 'timeout',
                 target: script
             }), 120000);
             /******/
             script.onerror = onScriptComplete.bind(null, script.onerror);
@@ -376,15 +376,19 @@
             /******/ // creates a new share scope if needed
             /******/
             if (!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};
             /******/ // runs all init snippets from all modules reachable
             /******/
             var scope = __webpack_require__.S[name];
             /******/
-            var warn = (msg) => (typeof console !== "undefined" && console.warn && console.warn(msg));
+            var warn = (msg) => {
+                /******/
+                if (typeof console !== "undefined" && console.warn) console.warn(msg);
+                /******/
+            };
             /******/
             var uniqueName = "jupyterlab-sql-editor";
             /******/
             var register = (name, version, factory, eager) => {
                 /******/
                 var versions = scope[name] = scope[name] || {};
                 /******/
@@ -424,15 +428,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("jupyterlab-sql-editor", "0.1.63", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("jupyterlab-sql-editor", "0.1.64", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                     register("sql-formatter", "6.1.2", () => (__webpack_require__.e("vendors-node_modules_sql-formatter_lib_index_js").then(() => (() => (__webpack_require__( /*! ./node_modules/sql-formatter/lib/index.js */ "./node_modules/sql-formatter/lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
@@ -457,21 +461,27 @@
         /******/
         var document = __webpack_require__.g.document;
         /******/
         if (!scriptUrl && document) {
             /******/
             if (document.currentScript)
                 /******/
-                scriptUrl = document.currentScript.src
+                scriptUrl = document.currentScript.src;
             /******/
             if (!scriptUrl) {
                 /******/
                 var scripts = document.getElementsByTagName("script");
                 /******/
-                if (scripts.length) scriptUrl = scripts[scripts.length - 1].src
+                if (scripts.length) {
+                    /******/
+                    var i = scripts.length - 1;
+                    /******/
+                    while (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;
+                    /******/
+                }
                 /******/
             }
             /******/
         }
         /******/ // When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration
         /******/ // or pass an empty string ("") and set the __webpack_public_path__ variable from your code to use your own logic.
         /******/
@@ -636,15 +646,15 @@
             /******/
         };
         /******/
         var getSingletonVersion = (scope, scopeName, key, requiredVersion) => {
             /******/
             var version = findSingletonVersionKey(scope, key);
             /******/
-            if (!satisfy(requiredVersion, version)) typeof console !== "undefined" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));
+            if (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));
             /******/
             return get(scope[key][version]);
             /******/
         };
         /******/
         var getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {
             /******/
@@ -692,17 +702,23 @@
             /******/
             if (entry) return get(entry);
             /******/
             throw new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));
             /******/
         };
         /******/
+        var warn = (msg) => {
+            /******/
+            if (typeof console !== "undefined" && console.warn) console.warn(msg);
+            /******/
+        };
+        /******/
         var warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {
             /******/
-            typeof console !== "undefined" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));
+            warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));
             /******/
         };
         /******/
         var get = (entry) => {
             /******/
             entry.loaded = 1;
             /******/
@@ -815,25 +831,25 @@
             /******/
         });
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/settingregistry": () => (loadSingletonVersionCheck("default", "@jupyterlab/settingregistry", [1, 3, 6, 3])),
+            "webpack/sharing/consume/default/@jupyterlab/settingregistry": () => (loadSingletonVersionCheck("default", "@jupyterlab/settingregistry", [1, 3, 6, 1])),
             /******/
-            "webpack/sharing/consume/default/@krassowski/jupyterlab-lsp": () => (loadSingletonVersionCheck("default", "@krassowski/jupyterlab-lsp", [1, 3, 10, 1])),
+            "webpack/sharing/consume/default/@krassowski/jupyterlab-lsp": () => (loadSingletonVersionCheck("default", "@krassowski/jupyterlab-lsp", [1, 3, 10, 2])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/codemirror": () => (loadSingletonVersionCheck("default", "@jupyterlab/codemirror", [1, 3, 6, 3])),
+            "webpack/sharing/consume/default/@jupyterlab/codemirror": () => (loadSingletonVersionCheck("default", "@jupyterlab/codemirror", [1, 3, 6, 1])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 3, 6, 3])),
+            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 3, 6, 1])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/fileeditor": () => (loadSingletonVersionCheck("default", "@jupyterlab/fileeditor", [1, 3, 6, 3])),
+            "webpack/sharing/consume/default/@jupyterlab/fileeditor": () => (loadSingletonVersionCheck("default", "@jupyterlab/fileeditor", [1, 3, 6, 1])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 3, 6, 3])),
+            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 3, 6, 1])),
             /******/
             "webpack/sharing/consume/default/sql-formatter/sql-formatter": () => (loadStrictVersionCheckFallback("default", "sql-formatter", [4, 6, 1, 2], () => (__webpack_require__.e("vendors-node_modules_sql-formatter_lib_index_js").then(() => (() => (__webpack_require__( /*! sql-formatter */ "./node_modules/sql-formatter/lib/index.js")))))))
             /******/
         };
         /******/ // no consumes in initial chunks
         /******/
         var chunkMapping = {
@@ -990,15 +1006,15 @@
                                 /******/
                             }
                             /******/
                         };
                         /******/
                         __webpack_require__.l(url, loadingEnded, "chunk-" + chunkId, chunkId);
                         /******/
-                    } else installedChunks[chunkId] = 0;
+                    }
                     /******/
                 }
                 /******/
             }
             /******/
         };
         /******/
@@ -1083,8 +1099,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyterlab-sql-editor");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["jupyterlab-sql-editor"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.84edd756b78db1078f1a.js.map
+//# sourceMappingURL=remoteEntry.f9d09d2e2aeaf511a32b.js.map
```

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/remoteEntry.84edd756b78db1078f1a.js.map` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/remoteEntry.f9d09d2e2aeaf511a32b.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8260869565217391%*

 * *Differences: {"'file'": "'remoteEntry.f9d09d2e2aeaf511a32b.js'",*

 * * "'mappings'": "';;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "remoteEntry.84edd756b78db1078f1a.js",
-    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,qRAAqR;WACnT;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC5CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCnLA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
+    "file": "remoteEntry.f9d09d2e2aeaf511a32b.js",
+    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,qRAAqR;WACnT;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC9CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCtLA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-sql-editor/webpack/container-entry",
         "webpack://jupyterlab-sql-editor/webpack/bootstrap",
         "webpack://jupyterlab-sql-editor/webpack/runtime/compat get default export",
         "webpack://jupyterlab-sql-editor/webpack/runtime/define property getters",
@@ -28,20 +28,20 @@
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
         "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"67b6c3715f795c58c5d6\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"8ab7ecce559b1f364311\",\"style_index_js\":\"7a9353dfa84524daa532\",\"vendors-node_modules_sql-formatter_lib_index_js\":\"1955e937c0ff0f3413ea\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
-        "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab-sql-editor:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t};\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
+        "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab-sql-editor:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"jupyterlab-sql-editor\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-sql-editor\", \"0.1.63\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"sql-formatter\", \"6.1.2\", () => (__webpack_require__.e(\"vendors-node_modules_sql-formatter_lib_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/sql-formatter/lib/index.js */ \"./node_modules/sql-formatter/lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
-        "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@krassowski/jupyterlab-lsp\": () => (loadSingletonVersionCheck(\"default\", \"@krassowski/jupyterlab-lsp\", [1,3,10,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/codemirror\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/codemirror\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/fileeditor\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/fileeditor\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/sql-formatter/sql-formatter\": () => (loadStrictVersionCheckFallback(\"default\", \"sql-formatter\", [4,6,1,2], () => (__webpack_require__.e(\"vendors-node_modules_sql-formatter_lib_index_js\").then(() => (() => (__webpack_require__(/*! sql-formatter */ \"./node_modules/sql-formatter/lib/index.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\",\n\t\t\"webpack/sharing/consume/default/@krassowski/jupyterlab-lsp\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/codemirror\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/fileeditor\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/sql-formatter/sql-formatter\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
-        "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab-sql-editor\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_sql_editor\"] = self[\"webpackChunkjupyterlab_sql_editor\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab-sql-editor\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-sql-editor\", \"0.1.64\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"sql-formatter\", \"6.1.2\", () => (__webpack_require__.e(\"vendors-node_modules_sql-formatter_lib_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/sql-formatter/lib/index.js */ \"./node_modules/sql-formatter/lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/@krassowski/jupyterlab-lsp\": () => (loadSingletonVersionCheck(\"default\", \"@krassowski/jupyterlab-lsp\", [1,3,10,2])),\n\t\"webpack/sharing/consume/default/@jupyterlab/codemirror\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/codemirror\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/fileeditor\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/fileeditor\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/sql-formatter/sql-formatter\": () => (loadStrictVersionCheckFallback(\"default\", \"sql-formatter\", [4,6,1,2], () => (__webpack_require__.e(\"vendors-node_modules_sql-formatter_lib_index_js\").then(() => (() => (__webpack_require__(/*! sql-formatter */ \"./node_modules/sql-formatter/lib/index.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\",\n\t\t\"webpack/sharing/consume/default/@krassowski/jupyterlab-lsp\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/codemirror\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/fileeditor\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/sql-formatter/sql-formatter\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab-sql-editor\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_sql_editor\"] = self[\"webpackChunkjupyterlab_sql_editor\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyterlab-sql-editor\");\n",
         ""
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js.map` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js.map` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js.map` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor.egg-info/PKG-INFO` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-sql-editor
-Version: 0.1.63
+Version: 0.1.64
 Summary: SQL editor support for formatting, syntax highlighting and code completion of SQL in cell magic, line magic, python string and file editor.
 Home-page: https://github.com/CybercentreCanada/jupyterlab-sql-editor
 Author: cccs-jc
 Author-email: contact@cyber.gc.ca
 License: MIT License (MIT)
 Keywords: sql,Jupyter,JupyterLab,JupyterLab3,jupyter,jupyterlab-extension,spark,trino,dataframe,cccs,canada
 Platform: Linux
@@ -114,15 +114,15 @@
 |`--database NAME`|Spark database to use.|
 |`-l LIMIT` `--limit LIMIT`|The maximum number of rows to display. A value of zero is equivalent to `--output skip`|
 |`-r all\|local\|none` `--refresh all\|local\|none`|Force the regeneration of the schema cache file. The `local` option will only update tables/views created in the local Spark context.|
 |`-d NAME` `--dataframe NAME`|Capture dataframe in a local variable named `NAME`.|
 |`-c` `--cache`|Cache dataframe.|
 |`-e` `--eager`|Cache dataframe with eager load.|
 |`-v VIEW` `--view VIEW`|Create or replace a temporary view named `VIEW`.|
-|`-o sql\|json\|html\|grid\|text\|schema\|skip\|none` `--output sql\|json\|html\|grid\|text\|schema\|skip\|none`|Output format. Defaults to html. The `sql` option prints the SQL statement that will be executed (useful to test jinja templated statements).|
+|`-o sql\|json\|html\|aggrid\|grid\|text\|schema\|skip\|none` `--output sql\|json\|html\|aggrid\|grid\|text\|schema\|skip\|none`|Output format. Defaults to html. The `sql` option prints the SQL statement that will be executed (useful to test jinja templated statements).|
 |`-s` `--show-nonprinting`|Replace none printable characters with their ascii codes (`LF` -> `\x0a`)|
 |`-j` `--jinja`|Enable Jinja templating support.|
 |`-b` `--dbt`|Enable DBT templating support.|
 |`-t LIMIT` `--truncate LIMIT`|Truncate output.|
 |`-m update\|complete` `--streaming_mode update\|complete`|The mode of streaming queries.|
 |`-x` `--lean-exceptions`|Shortened exceptions. Might be helpful if the exceptions reported by Spark are noisy such as with big SQL queries.|
 
@@ -130,15 +130,15 @@
 |Parameter|Description|
 |---|---|
 |`-c NAME` `--catalog NAME`|Trino catalog to use.|
 |`-s NAME` `--schema NAME`|Trino schema to use.|
 |`-l LIMIT` `--limit LIMIT`|The maximum number of rows to display. A value of zero is equivalent to `--output skip`|
 |`-r all\|none` `--refresh all\|none`|Force the regeneration of the schema cache file.|
 |`-d NAME` `--dataframe NAME`|Capture dataframe in a local variable named `NAME`.|
-|`-o sql\|json\|html\|grid\|text\|schema\|skip\|none` `--output sql\|json\|html\|grid\|text\|schema\|skip\|none`|Output format. Defaults to html. The `sql` option prints the SQL statement that will be executed (useful to test jinja templated statements).|
+|`-o sql\|json\|html\|aggrid\|grid\|text\|schema\|skip\|none` `--output sql\|json\|html\|aggrid\|grid\|text\|schema\|skip\|none`|Output format. Defaults to html. The `sql` option prints the SQL statement that will be executed (useful to test jinja templated statements).|
 |`-s` `--show-nonprinting`|Replace none printable characters with their ascii codes (`LF` -> `\x0a`).|
 |`-j` `--jinja`|Enable Jinja templating support.|
 |`-t LIMIT` `--truncate LIMIT`|Truncate output.|
 |`-x STATEMENT` `--raw STATEMENT`|Run statement as is. Do not wrap statement with a limit. Use this option to run statement which can't be wrapped in a SELECT/LIMIT statement. For example EXPLAIN, SHOW TABLE, SHOW CATALOGS.|
 
 ## Security Vulnerability Reporting
 
@@ -160,7 +160,8 @@
 
 - [krassowski/jupyterlab-lsp](https://github.com/jupyter-lsp/jupyterlab-lsp)
 - [joe-re/sql-language-server](https://github.com/joe-re/sql-language-server)
 - [zeroturnaround/sql-formatter](https://github.com/zeroturnaround/sql-formatter)
 - [cryeo/sparksql-magic](https://github.com/cryeo/sparksql-magic)
 - [trino-python-client](https://github.com/trinodb/trino-python-client)
 - [bloomberg/ipydatagrid](https://github.com/bloomberg/ipydatagrid)
+- [widgetti/ipyaggrid](https://github.com/widgetti/ipyaggrid)
```

### Comparing `jupyterlab_sql_editor-0.1.63/jupyterlab_sql_editor.egg-info/SOURCES.txt` & `jupyterlab_sql_editor-0.1.64/jupyterlab_sql_editor.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 jupyterlab_sql_editor/ipython_magic/trino/trino_export.py
 jupyterlab_sql_editor/labextension/build_log.json
 jupyterlab_sql_editor/labextension/package.json
 jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/package.json.orig
 jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/plugin.json
 jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js
 jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js.map
-jupyterlab_sql_editor/labextension/static/remoteEntry.84edd756b78db1078f1a.js
-jupyterlab_sql_editor/labextension/static/remoteEntry.84edd756b78db1078f1a.js.map
+jupyterlab_sql_editor/labextension/static/remoteEntry.f9d09d2e2aeaf511a32b.js
+jupyterlab_sql_editor/labextension/static/remoteEntry.f9d09d2e2aeaf511a32b.js.map
 jupyterlab_sql_editor/labextension/static/style.js
 jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js
 jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js.map
 jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js
 jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js.map
 jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js
 jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js.map
```

### Comparing `jupyterlab_sql_editor-0.1.63/overrides/sparksql-lsp.json` & `jupyterlab_sql_editor-0.1.64/overrides/sparksql-lsp.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/overrides/trino-lsp.json` & `jupyterlab_sql_editor-0.1.64/overrides/trino-lsp.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/package.json` & `jupyterlab_sql_editor-0.1.64/package.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8432765151515152%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '3.6.1', '@jupyterlab/apputils': '3.6.1', "*

 * *                   "'@jupyterlab/docmanager': '3.6.1', '@jupyterlab/fileeditor': '3.6.1', "*

 * *                   "'@jupyterlab/logconsole': '3.6.1', '@jupyterlab/notebook': '3.6.1', "*

 * *                   "'@jupyterlab/settingregistry': '3.6.1', '@krassowski/jupyterlab-lsp': "*

 * *                   "'^3.10.2', '@jupyterlab/cells': '3.6.1', '@jupyterlab/codemirror': '3.6.1', "*

 * *                   "'codemirror': '~5.61.0', del […]*

```diff
@@ -3,53 +3,41 @@
         "email": "contact@cyber.gc.ca",
         "name": "cccs-jc"
     },
     "bugs": {
         "url": "https://github.com/CybercentreCanada/jupyterlab-sql-editor/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.6.0",
-        "@jupyterlab/apputils": "^3.6.0",
-        "@jupyterlab/builder": "^3.6.0",
-        "@jupyterlab/codemirror-extension": "^3.6.0",
-        "@jupyterlab/docmanager": "^3.6.0",
-        "@jupyterlab/fileeditor": "^3.6.0",
-        "@jupyterlab/logconsole": "^3.6.0",
-        "@jupyterlab/mainmenu": "^3.6.0",
-        "@jupyterlab/notebook": "^3.6.0",
-        "@jupyterlab/settingregistry": "^3.6.0",
-        "@krassowski/jupyterlab-lsp": "^3.10.1",
-        "@lumino/widgets": "^1.26.1",
+        "@jupyterlab/application": "3.6.1",
+        "@jupyterlab/apputils": "3.6.1",
+        "@jupyterlab/cells": "3.6.1",
+        "@jupyterlab/codemirror": "3.6.1",
+        "@jupyterlab/docmanager": "3.6.1",
+        "@jupyterlab/fileeditor": "3.6.1",
+        "@jupyterlab/logconsole": "3.6.1",
+        "@jupyterlab/notebook": "3.6.1",
+        "@jupyterlab/settingregistry": "3.6.1",
+        "@krassowski/jupyterlab-lsp": "^3.10.2",
         "@types/codemirror": "^5.60.5",
-        "json-schema": "^0.4.0",
-        "lsp-ws-connection": "^0.7.0",
+        "codemirror": "~5.61.0",
         "npm-run-all": "^4.1.5",
-        "sql-formatter": "6.1.2",
-        "sql-language-server": "^1.2.1",
-        "vscode-languageserver": "8.0.0-next.8",
-        "vscode-languageserver-protocol": "3.16.0-next.13",
-        "vscode-languageserver-types": "3.16.0-next.7"
+        "sql-formatter": "6.1.2"
     },
     "description": "SQL editor support for formatting, syntax highlighting and code completion of SQL in cell magic, line magic, python string and file editor.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.6.0",
-        "@types/node": "^18.11.9",
+        "@jupyterlab/builder": "3.6.1",
+        "@types/node": "~18.11.9",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
         "rimraf": "^3.0.2",
-        "stylelint": "^14.3.0",
-        "stylelint-config-prettier": "^9.0.4",
-        "stylelint-config-recommended": "^6.0.0",
-        "stylelint-config-standard": "~24.0.0",
-        "stylelint-prettier": "^2.0.0",
         "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
@@ -72,56 +60,53 @@
         "Spark",
         "Trino",
         "Dataframe"
     ],
     "license": "MIT License (MIT)",
     "main": "lib/index.js",
     "name": "jupyterlab-sql-editor",
-    "overrides": {
-        "lsp-ws-connection": {
-            "vscode-languageserver-protocol": "3.16.0-next.13",
-            "vscode-languageserver-types": "3.16.0-next.7"
-        }
-    },
+    "packageManager": "yarn@3.5.1",
     "repository": {
         "type": "git",
         "url": "https://github.com/CybercentreCanada/jupyterlab-sql-editor.git"
     },
     "resolutions": {
+        "@jupyterlab/cells": "3.6.1",
+        "@jupyterlab/outputarea": "3.6.1",
+        "@jupyterlab/rendermime": "3.6.1",
+        "@jupyterlab/rendermime-interfaces": "3.6.1",
         "vscode-languageserver-protocol": "3.16.0-next.13",
         "vscode-languageserver-types": "3.16.0-next.7"
     },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --sourceMap",
         "build:lib:prod": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
         "clean:labextension": "rimraf jupyterlab_sql_editor/labextension jupyterlab_sql_editor/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
-        "clean:lintcache": "rimraf .eslintcache .stylelintcache",
+        "clean:lintcache": "rimraf .eslintcache",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
-        "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
-        "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
+        "lint": "jlpm prettier && jlpm eslint",
+        "lint:check": "jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
-        "stylelint": "jlpm stylelint:check --fix",
-        "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.63"
+    "version": "0.1.64"
 }
```

### Comparing `jupyterlab_sql_editor-0.1.63/pyproject.toml` & `jupyterlab_sql_editor-0.1.64/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/schema/plugin.json` & `jupyterlab_sql_editor-0.1.64/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/setup.py` & `jupyterlab_sql_editor-0.1.64/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,24 @@
     author=pkg_json["author"]["name"],
     author_email=pkg_json["author"]["email"],
     description=pkg_json["description"],
     license=pkg_json["license"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
-    install_requires=["trino", "ipydatagrid", "Jinja2", "ipytree", "ply", "dbt-core", "jupyter-events>=0.6.1"],
+    install_requires=[
+        "trino",
+        "ipydatagrid",
+        "ipyaggrid",
+        "Jinja2",
+        "ipytree",
+        "ply",
+        "dbt-core",
+        "jupyter-events>=0.6.1",
+    ],
     zip_safe=False,
     include_package_data=True,
     python_requires=">=3.6",
     platforms="Linux, Mac OS X, Windows",
     keywords=[
         "sql",
         "Jupyter",
```

### Comparing `jupyterlab_sql_editor-0.1.63/src/formatter.ts` & `jupyterlab_sql_editor-0.1.64/src/formatter.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/src/index.ts` & `jupyterlab_sql_editor-0.1.64/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/src/utils.ts` & `jupyterlab_sql_editor-0.1.64/src/utils.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.63/tsconfig.json` & `jupyterlab_sql_editor-0.1.64/tsconfig.json`

 * *Files identical despite different names*

