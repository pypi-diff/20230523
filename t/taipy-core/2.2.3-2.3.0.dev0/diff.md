# Comparing `tmp/taipy-core-2.2.3.tar.gz` & `tmp/taipy-core-2.3.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-core-2.2.3.tar", last modified: Thu Apr 27 12:02:02 2023, max compression
+gzip compressed data, was "taipy-core-2.3.0.dev0.tar", last modified: Tue May 23 20:17:16 2023, max compression
```

## Comparing `taipy-core-2.2.3.tar` & `taipy-core-2.3.0.dev0.tar`

### file list

```diff
@@ -1,165 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.591877 taipy-core-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-27 12:01:50.000000 taipy-core-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-27 12:01:50.000000 taipy-core-2.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-04-27 12:02:02.591877 taipy-core-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-04-27 12:01:50.000000 taipy-core-2.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-27 12:01:50.000000 taipy-core-2.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 12:02:02.591877 taipy-core-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-27 12:01:50.000000 taipy-core-2.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.571875 taipy-core-2.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.571875 taipy-core-2.2.3/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.571875 taipy-core-2.2.3/src/taipy/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.575876 taipy-core-2.2.3/src/taipy/core/_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_manager/_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_manager/_manager_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.575876 taipy-core-2.2.3/src/taipy/core/_repository/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_repository/_filesystem_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_repository/_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_repository/_repository_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_repository/_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_repository/_sql_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_repository/_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.575876 taipy-core-2.2.3/src/taipy/core/_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_scheduler/_abstract_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.575876 taipy-core-2.2.3/src/taipy/core/_scheduler/_dispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_scheduler/_dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_scheduler/_dispatcher/_development_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_scheduler/_dispatcher/_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_scheduler/_dispatcher/_standalone_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    12353 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_scheduler/_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_scheduler/_scheduler_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.575876 taipy-core-2.2.3/src/taipy/core/_version/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/_version_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/_version_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/_version_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/_version_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/_version_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/_version_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/_version_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/_version_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.579876 taipy-core-2.2.3/src/taipy/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/_entity_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/_get_valid_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/_listattributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/_reload.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/_repr_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/default_custom_document.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.579876 taipy-core-2.2.3/src/taipy/core/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.579876 taipy-core-2.2.3/src/taipy/core/config/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/checkers/_data_node_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/checkers/_job_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/checkers/_pipeline_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/checkers/_scenario_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/checkers/_task_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14342 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/config.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    32343 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/data_node_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/job_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/pipeline_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/scenario_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9199 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/task_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.579876 taipy-core-2.2.3/src/taipy/core/cycle/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/cycle/_cycle_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/cycle/_cycle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/cycle/_cycle_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/cycle/_cycle_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/cycle/_cycle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/cycle/_cycle_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/cycle/_cycle_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/cycle/cycle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.583876 taipy-core-2.2.3/src/taipy/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/_data_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/_data_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/_data_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/_data_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/_data_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/abstract_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    20110 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/data_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8770 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/sql_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.583876 taipy-core-2.2.3/src/taipy/core/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.583876 taipy-core-2.2.3/src/taipy/core/job/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/job/_job_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/job/_job_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/job/_job_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/job/_job_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/job/_job_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/job/_job_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/job/_job_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/job/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/job/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.587876 taipy-core-2.2.3/src/taipy/core/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/pipeline/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.587876 taipy-core-2.2.3/src/taipy/core/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/scenario/_scenario_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/scenario/_scenario_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/scenario/_scenario_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/scenario/_scenario_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/scenario/_scenario_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/scenario/_scenario_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/scenario/_scenario_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12425 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/scenario/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)    23645 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/taipy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.587876 taipy-core-2.2.3/src/taipy/core/task/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/task/_task_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/task/_task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/task/_task_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/task/_task_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/task/_task_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/task/_task_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/task/_task_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/version.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.587876 taipy-core-2.2.3/src/taipy_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-04-27 12:02:02.000000 taipy-core-2.2.3/src/taipy_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-04-27 12:02:02.000000 taipy-core-2.2.3/src/taipy_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 12:02:02.000000 taipy-core-2.2.3/src/taipy_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 12:01:55.000000 taipy-core-2.2.3/src/taipy_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-27 12:02:02.000000 taipy-core-2.2.3/src/taipy_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 12:02:02.000000 taipy-core-2.2.3/src/taipy_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.587876 taipy-core-2.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-04-27 12:01:50.000000 taipy-core-2.2.3/tests/test_complex_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    26443 2023-04-27 12:01:50.000000 taipy-core-2.2.3/tests/test_taipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.536005 taipy-core-2.3.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-05-23 20:17:16.536005 taipy-core-2.3.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 20:17:16.536005 taipy-core-2.3.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.512005 taipy-core-2.3.0.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.512005 taipy-core-2.3.0.dev0/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.516005 taipy-core-2.3.0.dev0/src/taipy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.516005 taipy-core-2.3.0.dev0/src/taipy/core/_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_backup/_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_core_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.516005 taipy-core-2.3.0.dev0/src/taipy/core/_entity/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_entity/_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_entity/_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_entity/_entity_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_entity/_labeled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_entity/_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_entity/_reload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_entity/_submittable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.516005 taipy-core-2.3.0.dev0/src/taipy/core/_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_manager/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_manager/_manager_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.516005 taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_abstract_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.516005 taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_orchestrator_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.516005 taipy-core-2.3.0.dev0/src/taipy/core/_repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_repository/_filesystem_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_repository/_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_repository/_repository_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_repository/_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_repository/_sql_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_repository/_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.520005 taipy-core-2.3.0.dev0/src/taipy/core/_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.520005 taipy-core-2.3.0.dev0/src/taipy/core/_version/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_cli/_bcolor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_cli/_version_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.520005 taipy-core-2.3.0.dev0/src/taipy/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/common/_listattributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/common/_repr_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/common/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/common/_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/common/default_custom_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/common/warn_if_inputs_not_ready.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.520005 taipy-core-2.3.0.dev0/src/taipy/core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/_core_section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.524005 taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_config_id_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_data_node_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_job_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_pipeline_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_scenario_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_task_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/config.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40959 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/data_node_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/job_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/pipeline_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/scenario_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/config/task_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.524005 taipy-core-2.3.0.dev0/src/taipy/core/cycle/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/cycle/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/cycle/cycle_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.528005 taipy-core-2.3.0.dev0/src/taipy/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/_data_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/_data_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/_data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/_data_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/_data_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/abstract_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/abstract_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21107 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/data_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/data_node_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13615 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11704 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/data/sql_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.528005 taipy-core-2.3.0.dev0/src/taipy/core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.528005 taipy-core-2.3.0.dev0/src/taipy/core/job/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/_job_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/_job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/_job_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/_job_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/_job_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/_job_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/_job_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/job_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/job/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.528005 taipy-core-2.3.0.dev0/src/taipy/core/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/notification/core_event_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/notification/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/notification/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/notification/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/notification/registration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/notification/topic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.532005 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/pipeline/pipeline_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.532005 taipy-core-2.3.0.dev0/src/taipy/core/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13787 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/scenario/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/scenario/scenario_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25672 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/taipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.536005 taipy-core-2.3.0.dev0/src/taipy/core/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/task/_task_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/task/_task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/task/_task_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/task/_task_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/task/_task_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/task/_task_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/task/_task_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/task/task_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/src/taipy/core/version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.536005 taipy-core-2.3.0.dev0/src/taipy_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-05-23 20:17:16.000000 taipy-core-2.3.0.dev0/src/taipy_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-05-23 20:17:16.000000 taipy-core-2.3.0.dev0/src/taipy_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:17:16.000000 taipy-core-2.3.0.dev0/src/taipy_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:17:09.000000 taipy-core-2.3.0.dev0/src/taipy_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-23 20:17:16.000000 taipy-core-2.3.0.dev0/src/taipy_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 20:17:16.000000 taipy-core-2.3.0.dev0/src/taipy_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:17:16.536005 taipy-core-2.3.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/tests/test_complex_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29447 2023-05-23 20:17:04.000000 taipy-core-2.3.0.dev0/tests/test_taipy.py
```

### Comparing `taipy-core-2.2.3/LICENSE` & `taipy-core-2.3.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/PKG-INFO` & `taipy-core-2.3.0.dev0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-core
-Version: 2.2.3
+Version: 2.3.0.dev0
 Summary: A Python library to build powerful and customized data-driven back-end applications.
 Home-page: https://github.com/avaiga/taipy-core
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-core
 Classifier: Intended Audience :: Developers
@@ -26,15 +26,15 @@
 # Taipy Core
 [![tests](https://github.com/Avaiga/taipy-core/actions/workflows/tests.yml/badge.svg)](https://github.com/Avaiga/taipy-core/actions/workflows/tests.yml)
 [![Python](https://img.shields.io/pypi/pyversions/taipy-core)](https://pypi.org/project/taipy-core)
 [![PyPI](https://img.shields.io/pypi/v/taipy-core.svg?label=pip&logo=PyPI&logoColor=white)](https://pypi.org/project/taipy-core)
 
 
 ## License
-Copyright 2022 Avaiga Private Limited
+Copyright 2023 Avaiga Private Limited
 
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with
 the License. You may obtain a copy of the License at
 [http://www.apache.org/licenses/LICENSE-2.0](https://www.apache.org/licenses/LICENSE-2.0.txt)
 
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
@@ -73,16 +73,18 @@
 
 Want to be part of the _Taipy Core_ community? Check out our [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) file.
 
 ## Directory Structure
 
 - `taipy/core`:
     - `taipy/core`:
+        - `_manager`: Internal package for entity manager.
         - `_repository`: Internal package for data storage.
-        - `_scheduler`: Internal package for task scheduling and execution.
+        - `_orchestrator`: Internal package for task orchestrating and execution.
+        - `_version`: Internal package for managing Taipy Core application version.
         - `common`: Shared data structures, types, and functions.
         - `config`: Configuration definition, management and implementation. `config.config.Config` is the main
           entrypoint for configuring a Taipy Core application.
         - `cycle`: Work cycle definition, management and implementation.
         - `data`: Data Node definition, management and implementation.
         - `exceptions`: _taipy-core_ exceptions.
         - `job`: Job definition, management and implementation.
@@ -93,9 +95,10 @@
     - `tests`: Unit tests following the `taipy/core` structure.
 - `CODE_OF_CONDUCT.md`: Code of conduct for members and contributors of _taipy-core_.
 - `CONTRIBUTING.md`: Instructions to contribute to _taipy-core_.
 - `INSTALLATION.md`: Instructions to install _taipy-core_.
 - `LICENSE`: The Apache 2.0 License.
 - `Pipfile`: File used by the Pipenv virtual environment to manage project dependencies.
 - `README.md`: Current file.
+- `contributors.txt`: The list of contributors.
 - `setup.py`: The setup script managing building, distributing, and installing _taipy-core_.
 - `tox.ini`: Contains test scenarios to be run.
```

### Comparing `taipy-core-2.2.3/README.md` & `taipy-core-2.3.0.dev0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Taipy Core
 [![tests](https://github.com/Avaiga/taipy-core/actions/workflows/tests.yml/badge.svg)](https://github.com/Avaiga/taipy-core/actions/workflows/tests.yml)
 [![Python](https://img.shields.io/pypi/pyversions/taipy-core)](https://pypi.org/project/taipy-core)
 [![PyPI](https://img.shields.io/pypi/v/taipy-core.svg?label=pip&logo=PyPI&logoColor=white)](https://pypi.org/project/taipy-core)
 
 
 ## License
-Copyright 2022 Avaiga Private Limited
+Copyright 2023 Avaiga Private Limited
 
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with
 the License. You may obtain a copy of the License at
 [http://www.apache.org/licenses/LICENSE-2.0](https://www.apache.org/licenses/LICENSE-2.0.txt)
 
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
@@ -48,16 +48,18 @@
 
 Want to be part of the _Taipy Core_ community? Check out our [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) file.
 
 ## Directory Structure
 
 - `taipy/core`:
     - `taipy/core`:
+        - `_manager`: Internal package for entity manager.
         - `_repository`: Internal package for data storage.
-        - `_scheduler`: Internal package for task scheduling and execution.
+        - `_orchestrator`: Internal package for task orchestrating and execution.
+        - `_version`: Internal package for managing Taipy Core application version.
         - `common`: Shared data structures, types, and functions.
         - `config`: Configuration definition, management and implementation. `config.config.Config` is the main
           entrypoint for configuring a Taipy Core application.
         - `cycle`: Work cycle definition, management and implementation.
         - `data`: Data Node definition, management and implementation.
         - `exceptions`: _taipy-core_ exceptions.
         - `job`: Job definition, management and implementation.
@@ -68,9 +70,10 @@
     - `tests`: Unit tests following the `taipy/core` structure.
 - `CODE_OF_CONDUCT.md`: Code of conduct for members and contributors of _taipy-core_.
 - `CONTRIBUTING.md`: Instructions to contribute to _taipy-core_.
 - `INSTALLATION.md`: Instructions to install _taipy-core_.
 - `LICENSE`: The Apache 2.0 License.
 - `Pipfile`: File used by the Pipenv virtual environment to manage project dependencies.
 - `README.md`: Current file.
+- `contributors.txt`: The list of contributors.
 - `setup.py`: The setup script managing building, distributing, and installing _taipy-core_.
 - `tox.ini`: Contains test scenarios to be run.
```

### Comparing `taipy-core-2.2.3/setup.py` & `taipy-core-2.3.0.dev0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "pyarrow>=10.0.1,<11.0",
     "networkx>=2.6,<3.0",
     "openpyxl>=3.0.7,<3.1",
     "modin[dask]>=0.16.2,<1.0",
     "pymongo>=4.2.0,<5.0",
     "sqlalchemy>=1.4,<2.0",
     "toml>=0.10,<0.11",
-    "taipy-config>=2.2,<2.3",
+    "taipy-config>=2.3.0.dev0",
 ]
 
 test_requirements = ["pytest>=3.8"]
 
 extras_require = {
     "fastparquet": ["fastparquet==2022.11.0"],
     "mssql": ["pyodbc>=4,<4.1"],
```

### Comparing `taipy-core-2.2.3/src/taipy/__init__.py` & `taipy-core-2.3.0.dev0/src/taipy/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,34 +13,39 @@
 
 if find_spec("taipy"):
     if find_spec("taipy.config"):
         from taipy.config import Config, Frequency, Scope
 
     if find_spec("taipy.core"):
         from taipy.core._core import Core
-        from taipy.core.common.alias import CycleId, DataNodeId, JobId, PipelineId, ScenarioId, TaskId
         from taipy.core.cycle.cycle import Cycle
+        from taipy.core.cycle.cycle_id import CycleId
         from taipy.core.data.data_node import DataNode
+        from taipy.core.data.data_node_id import DataNodeId
         from taipy.core.job.job import Job
+        from taipy.core.job.job_id import JobId
         from taipy.core.job.status import Status
         from taipy.core.pipeline.pipeline import Pipeline
+        from taipy.core.pipeline.pipeline_id import PipelineId
         from taipy.core.scenario.scenario import Scenario
+        from taipy.core.scenario.scenario_id import ScenarioId
         from taipy.core.taipy import (
             cancel_job,
             clean_all_entities,
             clean_all_entities_by_version,
             compare_scenarios,
             create_pipeline,
             create_scenario,
             delete,
             delete_job,
             delete_jobs,
             export_scenario,
             get,
             get_cycles,
+            get_cycles_scenarios,
             get_data_nodes,
             get_jobs,
             get_latest_job,
             get_parents,
             get_pipelines,
             get_primary,
             get_primary_scenarios,
@@ -53,14 +58,15 @@
             subscribe_scenario,
             tag,
             unsubscribe_pipeline,
             unsubscribe_scenario,
             untag,
         )
         from taipy.core.task.task import Task
+        from taipy.core.task.task_id import TaskId
 
     if find_spec("taipy.gui"):
         from taipy.gui import Gui
 
         if find_spec("taipy.enterprise") and find_spec("taipy.enterprise.gui"):
             from taipy.enterprise.gui import _init_gui_enterprise
```

### Comparing `taipy-core-2.2.3/src/taipy/core/__init__.py` & `taipy-core-2.3.0.dev0/src/taipy/core/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,36 +38,41 @@
     [running services](../../../manuals/running_services/) page of the user manual for more details.
 
 """
 import json
 import os
 
 from ._core import Core
-from .common.alias import CycleId, DataNodeId, Edit, JobId, PipelineId, ScenarioId, TaskId
 from .common.default_custom_document import DefaultCustomDocument
 from .cycle.cycle import Cycle
+from .cycle.cycle_id import CycleId
 from .data.data_node import DataNode
+from .data.data_node_id import DataNodeId, Edit
 from .exceptions import exceptions
 from .job.job import Job
+from .job.job_id import JobId
 from .job.status import Status
 from .pipeline.pipeline import Pipeline
+from .pipeline.pipeline_id import PipelineId
 from .scenario.scenario import Scenario
+from .scenario.scenario_id import ScenarioId
 from .taipy import (
     cancel_job,
     clean_all_entities,
     clean_all_entities_by_version,
     compare_scenarios,
     create_pipeline,
     create_scenario,
     delete,
     delete_job,
     delete_jobs,
     export_scenario,
     get,
     get_cycles,
+    get_cycles_scenarios,
     get_data_nodes,
     get_jobs,
     get_latest_job,
     get_parents,
     get_pipelines,
     get_primary,
     get_primary_scenarios,
@@ -80,14 +85,15 @@
     subscribe_scenario,
     tag,
     unsubscribe_pipeline,
     unsubscribe_scenario,
     untag,
 )
 from .task.task import Task
+from .task.task_id import TaskId
 
 with open(f"{os.path.dirname(os.path.abspath(__file__))}{os.sep}version.json") as version_file:
     version = json.load(version_file)
     version_string = f'{version.get("major", 0)}.{version.get("minor", 0)}.{version.get("patch", 0)}'
     if vext := version.get("ext"):
         version_string = f"{version_string}.{vext}"
```

### Comparing `taipy-core-2.2.3/src/taipy/core/_core.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_repository.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,107 +5,92 @@
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
-import uuid
-from typing import Optional
+import pathlib
+from datetime import datetime
+from typing import Any, Iterable, List, Optional, Union
 
 from taipy.config import Config
-from taipy.logger._taipy_logger import _TaipyLogger
 
-from ._scheduler._dispatcher._job_dispatcher import _JobDispatcher
-from ._scheduler._scheduler import _Scheduler
-from ._scheduler._scheduler_factory import _SchedulerFactory
-from ._version._version_cli import _VersioningCLI
-from ._version._version_manager_factory import _VersionManagerFactory
-from .exceptions.exceptions import VersionConflictWithPythonConfig
-from .taipy import clean_all_entities_by_version
-
-
-class Core:
-    """
-    Core service
-    """
-
-    _scheduler: Optional[_Scheduler] = None
-    _dispatcher: Optional[_JobDispatcher] = None
-
-    def __init__(self):
-        """
-        Initialize a Core service.
-        """
-        _VersioningCLI._create_parser()
-        self.cli_args = _VersioningCLI._parse_arguments()
-        self._scheduler = _SchedulerFactory._build_scheduler()
-
-    def run(self, force_restart=False):
-        """
-        Start a Core service.
-
-        This function check the configuration, start a dispatcher and lock the Config.
-        """
-        self.__check_config()
-        self.__manage_version(*self.cli_args)
-        self.__start_dispatcher(force_restart)
-
-    def stop(self):
-        """
-        Stop the Core service.
-
-        This function stops the dispatcher and unblock the Config for update.
-        """
-        Config.unblock_update()
-
-        if self._dispatcher:
-            self._dispatcher = _SchedulerFactory._remove_dispatcher()
-            _TaipyLogger._get_logger().info("Core service has been stopped.")
-
-    def __check_config(self):
-        Config.check()
-        Config.block_update()
-
-    def __manage_version(self, mode, _version_number, force, clean_entities):
-        if mode == "development":
-            current_version_number = _VersionManagerFactory._build_manager()._get_development_version()
-
-            clean_all_entities_by_version(current_version_number)
-            _TaipyLogger._get_logger().info(f"Development mode: Clean all entities of version {current_version_number}")
-
-            _VersionManagerFactory._build_manager()._set_development_version(current_version_number)
-
-        elif mode in ["experiment", "production"]:
-            default_version_number = {
-                "experiment": str(uuid.uuid4()),
-                "production": _VersionManagerFactory._build_manager()._get_latest_version(),
-            }
-
-            version_setter = {
-                "experiment": _VersionManagerFactory._build_manager()._set_experiment_version,
-                "production": _VersionManagerFactory._build_manager()._set_production_version,
-            }
-
-            if _version_number:
-                current_version_number = _version_number
-            else:
-                current_version_number = default_version_number[mode]
-
-            if clean_entities:
-                clean_all_entities_by_version(current_version_number)
-                _TaipyLogger._get_logger().info(f"Clean all entities of version {current_version_number}")
-
-            try:
-                version_setter[mode](current_version_number, force)
-            except VersionConflictWithPythonConfig as e:
-                raise SystemExit(e.message)
-
-        else:
-            raise SystemExit(f"Undefined execution mode: {mode}.")
-
-    def __start_dispatcher(self, force_restart):
-        if dispatcher := _SchedulerFactory._build_dispatcher(force_restart=force_restart):
-            self._dispatcher = dispatcher
+from .._repository._repository import _AbstractRepository
+from .._repository._repository_adapter import _RepositoryAdapter
+from ._version import _Version
+from ._version_model import _VersionModel
 
-        if Config.job_config.is_development:
-            _Scheduler._check_and_execute_jobs_if_development_mode()
+
+class _VersionRepository(_AbstractRepository[_VersionModel, _Version]):  # type: ignore
+    _LATEST_VERSION_KEY = "latest_version"
+    _DEVELOPMENT_VERSION_KEY = "development_version"
+    _PRODUCTION_VERSION_KEY = "production_version"
+
+    def __init__(self, **kwargs):
+        kwargs.update({"to_model_fct": self._to_model, "from_model_fct": self._from_model})
+        self.repo = _RepositoryAdapter.select_base_repository()(**kwargs)
+
+    @property
+    def repository(self):
+        return self.repo
+
+    def _to_model(self, version: _Version):
+        return _VersionModel(
+            id=version.id, config=Config._to_json(version.config), creation_date=version.creation_date.isoformat()
+        )
+
+    def _from_model(self, model):
+        version = _Version(id=model.id, config=Config._from_json(model.config))
+        version.creation_date = datetime.fromisoformat(model.creation_date)
+        return version
+
+    def load(self, model_id: str) -> _Version:
+        return self.repo.load(model_id)
+
+    def _load_all(self, version_number: Optional[str] = "all") -> List[_Version]:
+        return self.repo._load_all(version_number)
+
+    def _load_all_by(self, by, version_number: Optional[str] = "all") -> List[_Version]:
+        return self.repo._load_all_by(by, version_number)
+
+    def _save(self, entity: _Version):
+        return self.repo._save(entity)
+
+    def _delete(self, entity_id: str):
+        return self.repo._delete(entity_id)
+
+    def _delete_all(self):
+        return self.repo._delete_all()
+
+    def _delete_many(self, ids: Iterable[str]):
+        return self.repo._delete_many(ids)
+
+    def _delete_by(self, attribute: str, value: str, version_number: Optional[str] = None):
+        return self.repo._delete_by(attribute, value, version_number)
+
+    def _search(self, attribute: str, value: Any, version_number: Optional[str] = None) -> Optional[_Version]:
+        return self.repo._search(attribute, value, version_number)
+
+    def _export(self, entity_id: str, folder_path: Union[str, pathlib.Path]):
+        return self.repo._export(entity_id, folder_path)
+
+    def _set_latest_version(self, version_number):
+        self.repo._set_latest_version(version_number)
+
+    def _get_latest_version(self) -> str:
+        return self.repo._get_latest_version()
+
+    def _set_development_version(self, version_number):
+        self.repo._set_development_version(version_number)
+
+    def _get_development_version(self) -> str:
+        return self.repo._get_development_version()
+
+    def _set_production_version(self, version_number):
+        self.repo._set_production_version(version_number)
+
+    def _get_production_versions(self) -> List[str]:
+        return self.repo._get_production_versions()
+
+    def _delete_production_version(self, version_number):
+        self.repo._delete_production_version(version_number)
```

### Comparing `taipy-core-2.2.3/src/taipy/core/_manager/__init__.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/_manager/_manager.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_manager/_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 # specific language governing permissions and limitations under the License.
 
 import pathlib
 from typing import Generic, Iterable, List, Optional, TypeVar, Union
 
 from taipy.logger._taipy_logger import _TaipyLogger
 
+from .._entity._entity_ids import _EntityIds
 from .._repository import _AbstractRepository
-from ..common._entity_ids import _EntityIds
 from ..exceptions.exceptions import ModelNotFound
+from ..notification import EventOperation, _publish_event
 
 EntityType = TypeVar("EntityType")
 
 
 class _Manager(Generic[EntityType]):
     _repository: _AbstractRepository
     _logger = _TaipyLogger._get_logger()
@@ -28,35 +29,44 @@
 
     @classmethod
     def _delete_all(cls):
         """
         Deletes all entities.
         """
         cls._repository._delete_all()
+        if hasattr(cls, "_EVENT_ENTITY_TYPE"):
+            _publish_event(cls._EVENT_ENTITY_TYPE, "all", EventOperation.DELETION, None)
 
     @classmethod
     def _delete_many(cls, ids: Iterable):
         """
         Deletes entities by a list of ids.
         """
         cls._repository._delete_many(ids)
+        if hasattr(cls, "_EVENT_ENTITY_TYPE"):
+            for entity_id in ids:
+                _publish_event(cls._EVENT_ENTITY_TYPE, entity_id, EventOperation.DELETION, None)  # type: ignore
 
     @classmethod
     def _delete_by_version(cls, version_number: str):
         """
         Deletes entities by version number.
         """
         cls._repository._delete_by(attribute="version", value=version_number, version_number="all")  # type: ignore
+        if hasattr(cls, "_EVENT_ENTITY_TYPE"):
+            _publish_event(cls._EVENT_ENTITY_TYPE, None, EventOperation.DELETION, None)  # type: ignore
 
     @classmethod
     def _delete(cls, id):
         """
         Deletes an entity by id.
         """
         cls._repository._delete(id)
+        if hasattr(cls, "_EVENT_ENTITY_TYPE"):
+            _publish_event(cls._EVENT_ENTITY_TYPE, id, EventOperation.DELETION, None)
 
     @classmethod
     def _set(cls, entity: EntityType):
         """
         Save or update an entity.
         """
         cls._repository._save(entity)
@@ -108,7 +118,14 @@
 
     @classmethod
     def _export(cls, id: str, folder_path: Union[str, pathlib.Path]):
         """
         Export an entity.
         """
         return cls._repository._export(id, folder_path)
+
+    @classmethod
+    def _get_by_config_id(cls, config_id: str) -> List[EntityType]:
+        """
+        Get all entities by its config id.
+        """
+        return cls._repository._get_by_config_id(config_id)
```

### Comparing `taipy-core-2.2.3/src/taipy/core/_manager/_manager_factory.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_manager/_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/_repository/__init__.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_repository/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/_repository/_filesystem_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_repository/_filesystem_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,21 @@
     def _delete_by(self, attribute: str, value: str, version_number: Optional[str] = None):
         while entity := self._search(attribute, value, version_number):
             self._delete(entity.id)  # type: ignore
 
     def _search(self, attribute: str, value: str, version_number: Optional[str] = None) -> Optional[Entity]:
         return next(self.__search(attribute, value, version_number), None)
 
+    def _get_by_config_id(self, config_id: str) -> List[Entity]:
+        entities: List[Entity] = []
+        for f in filter(lambda f: config_id in f.name, self.dir_path.iterdir()):
+            if entity := self.__to_entity(f, retry=Config.global_config.read_entity_retry or 0):
+                entities.append(entity)
+        return entities
+
     def _get_by_config_and_owner_id(self, config_id: str, owner_id: Optional[str]) -> Optional[Entity]:
         # Only get the entity from the latest version
         from .._version._version_manager_factory import _VersionManagerFactory
 
         version_number = _VersionManagerFactory._build_manager()._replace_version_number(None)
 
         try:
```

### Comparing `taipy-core-2.2.3/src/taipy/core/_repository/_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_repository/_repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,14 +131,28 @@
         Args:
             entity_id (str): The id of the entity to be exported.
             folder_path (Union[str, pathlib.Path]): The folder path to export the entity to.
 
         """
         raise NotImplementedError
 
+    @abstractmethod
+    def _get_by_config_id(cls, config_id: str) -> List[Entity]:
+        """
+        Get the entities by its config id.
+
+        Args:
+            config_id (str): The config id of the entities
+
+        Returns:
+            A list of entities corresponding to the config id
+
+        """
+        raise NotImplementedError
+
 
 def _timedelta_to_str(obj: timedelta) -> str:
     total_seconds = obj.total_seconds()
     return (
         f"{int(total_seconds // 86400)}d"
         f"{int(total_seconds % 86400 // 3600)}h"
         f"{int(total_seconds % 3600 // 60)}m"
```

### Comparing `taipy-core-2.2.3/src/taipy/core/_repository/_repository_adapter.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_repository/_repository_adapter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/_repository/_repository_factory.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_repository/_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/_repository/_sql_model.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_repository/_sql_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/_repository/_sql_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_repository/_sql_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 # specific language governing permissions and limitations under the License.
 
 import json
 import pathlib
 from abc import abstractmethod
 from typing import Any, Callable, Iterable, List, Optional, Type, TypeVar, Union
 
-from sqlalchemy import create_engine, delete
+from sqlalchemy import create_engine, delete, or_
 from sqlalchemy.exc import NoResultFound
-from sqlalchemy.orm import sessionmaker
+from sqlalchemy.orm import Query, sessionmaker
 from sqlalchemy.pool import StaticPool
 
 from taipy.config.config import Config
 
 from ..exceptions.exceptions import MissingRequiredProperty, ModelNotFound, VersionIsNotProductionVersion
 from ._repository import _AbstractRepository, _CustomDecoder, _CustomEncoder
 from ._sql_model import Base, _TaipyModel, _TaipyVersion
@@ -128,17 +128,16 @@
     def _delete(self, model_id: str):
         number_of_deleted_entries = self.session.query(self._table).filter_by(model_id=model_id).delete()
         if not number_of_deleted_entries:
             raise ModelNotFound(str(self.model.__name__), model_id)
         self.session.commit()
 
     def _delete_by(self, attribute: str, value: str, version_number: Optional[str] = None):
-        entries = self._search(attribute, value, version_number)
-        if entries:
-            self._delete_many([e.id for e in entries])  # type: ignore
+        while entity := self._search(attribute, value, version_number):
+            self._delete(entity.id)  # type: ignore
 
     def _delete_all(self):
         self.session.query(self._table).filter_by(model_name=self.model_name).delete()
         self.session.commit()
 
     def _delete_many(self, ids: Iterable[str]):
         self.session.execute(delete(self._table).where(self._table.model_id.in_(ids)))
@@ -152,34 +151,43 @@
         )
         query = self.__filter_by_version(query, version_number)
         entry = query.first()
         if not entry:
             return None
         return self.__to_entity(entry)
 
+    def _get_by_config_id(self, config_id: str) -> List[Entity]:
+        query = (
+            self.session.query(self._table)
+            .filter_by(model_name=self.model_name)
+            .filter(self._table.document.contains(f'"config_id": "{config_id}"'))
+        )
+        entity_models = query.all()
+        return [self.__to_entity(entity_model) for entity_model in entity_models]
+
     def _get_by_config_and_owner_id(self, config_id: str, owner_id: Optional[str]) -> Optional[Entity]:
-        entity = self.__get_entities_by_config_and_owner(config_id, owner_id)
-        return self.__to_entity(entity)
+        model = self.__get_model_by_config_and_owner(config_id, owner_id)
+        return self.__to_entity(model)
 
     def _get_by_configs_and_owner_ids(self, configs_and_owner_ids):
         # Design in order to optimize performance on Entity creation.
         # Maintainability and readability were impacted.
         res = {}
         configs_and_owner_ids = set(configs_and_owner_ids)
 
         for config, owner in configs_and_owner_ids:
-            entry = self.__get_entities_by_config_and_owner(config.id, owner)
+            entry = self.__get_model_by_config_and_owner(config.id, owner)
             if entry:
                 entity = self.__to_entity(entry)
                 key = config, owner
                 res[key] = entity
 
         return res
 
-    def __get_entities_by_config_and_owner(
+    def __get_model_by_config_and_owner(
         self, config_id: str, owner_id: Optional[str] = "", version_number: Optional[str] = None
     ) -> _TaipyModel:
         if owner_id:
             query = (
                 self.session.query(self._table)
                 .filter_by(model_name=self.model_name)
                 .filter(self._table.document.contains(f'"config_id": "{config_id}"'))
@@ -219,21 +227,26 @@
             check_circular=False,
         )
         self.session.commit()
 
     def __to_entity(self, entry: _TaipyModel) -> Entity:
         return self.__model_to_entity(entry.document) if entry else None
 
-    def __filter_by_version(self, query, version_number):
+    def __filter_by_version(self, query: Query, version_number: Optional[str]):
         from .._version._version_manager_factory import _VersionManagerFactory
 
         version_number = _VersionManagerFactory._build_manager()._replace_version_number(version_number)
 
+        if not isinstance(version_number, List):
+            version_number = [version_number] if version_number else []  # type: ignore
+
         if version_number:
-            query = query.filter(self._table.document.contains(f'"version": "{version_number}"'))
+            version_query = list(map(lambda version: f'"version": "{version}"', version_number))
+            search_args = [self._table.document.contains(query) for query in version_query]
+            query = query.filter(or_(*search_args))
         return query
 
     def __model_to_entity(self, file_content):
         data = json.loads(file_content, cls=_CustomDecoder)
         model = self.model.from_dict(data)  # type: ignore
         entity = self._from_model(model)
         # Add version attribute on old entities. Used to migrate from <=2.0 to >=2.1 version.
@@ -350,15 +363,15 @@
 
     def __insert_model(self, model: ModelType):
         entry = self._table(id=model.id, config=model.config, creation_date=model.creation_date)  # type: ignore
         self.session.add(entry)
         self.session.commit()
 
     def __update_entry(self, entry, model):
-        entry.config = Config._to_json(model.config)
+        entry.config = model.config
         self.session.commit()
 
     def __to_entity(self, entry: _TaipyVersion) -> Entity:
         return self._from_model(entry)
         # return self.__model_to_entity(entry.config) if entry else None
 
     def __model_to_entity(self, file_content):
@@ -387,15 +400,15 @@
         version.is_latest = True
 
         self.session.commit()
 
     def _get_latest_version(self):
         if latest := self.session.query(self._table).filter_by(is_latest=True).first():
             return latest.id
-        return ""
+        raise ModelNotFound(self.model, "")
 
     def _set_development_version(self, version_number):
         if old_development := self.session.query(self._table).filter_by(is_development=True).first():
             old_development.is_development = False
 
         version = self.__get_by_id(version_number)
         version.is_development = True
@@ -403,34 +416,34 @@
         self._set_latest_version(version_number)
 
         self.session.commit()
 
     def _get_development_version(self):
         if development := self.session.query(self._table).filter_by(is_development=True).first():
             return development.id
-        raise ModelNotFound
+        raise ModelNotFound(self.model, "")
 
     def _set_production_version(self, version_number):
         version = self.__get_by_id(version_number)
         version.is_production = True
 
         self._set_latest_version(version_number)
 
         self.session.commit()
 
-    def _get_production_version(self):
+    def _get_production_versions(self):
         if productions := self.session.query(self._table).filter_by(is_production=True).all():
             return [p.id for p in productions]
-        return []
+        raise ModelNotFound(self.model, "")
 
     def _delete_production_version(self, version_number):
         version = self.__get_by_id(version_number)
 
         if not version or not version.is_production:
-            raise VersionIsNotProductionVersion(f"Version {version_number} is not a production version.")
+            raise VersionIsNotProductionVersion(f"Version '{version_number}' is not a production version.")
         version.is_production = False
 
         self.session.commit()
 
 
 class _SQLRepository(_BaseSQLRepository):
     def __init__(
@@ -479,14 +492,17 @@
 
     def _get_by_config_and_owner_id(self, config_id: str, owner_id: Optional[str]) -> Optional[Entity]:
         return self._table._get_by_config_and_owner_id(config_id, owner_id)  # type: ignore
 
     def _get_by_configs_and_owner_ids(self, configs_and_owner_ids):
         return self._table._get_by_configs_and_owner_ids(configs_and_owner_ids)
 
+    def _get_by_config_id(self, config_id=str) -> List[Entity]:
+        return self._table._get_by_config_id(config_id)
+
     def _set_latest_version(self, version_number):
         self._table._set_latest_version(version_number)
 
     def _get_latest_version(self):
         return self._table._get_latest_version()
 
     def _set_development_version(self, version_number):
@@ -494,12 +510,12 @@
 
     def _get_development_version(self):
         return self._table._get_development_version()
 
     def _set_production_version(self, version_number):
         self._table._set_production_version(version_number)
 
-    def _get_production_version(self):
-        return self._table._get_production_version()
+    def _get_production_versions(self):
+        return self._table._get_production_versions()
 
     def _delete_production_version(self, version_number):
         self._table._delete_production_version(version_number)
```

### Comparing `taipy-core-2.2.3/src/taipy/core/_scheduler/__init__.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_entity/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/_scheduler/_abstract_scheduler.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_abstract_orchestrator.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from abc import abstractmethod
 from typing import Callable, Iterable, List, Optional, Union
 
 from ..job.job import Job
 from ..task.task import Task
 
 
-class _AbstractScheduler:
-    """Creates, Enqueues and schedules jobs as instances of `Job^` class."""
+class _AbstractOrchestrator:
+    """Creates, enqueues, and orchestrates jobs as instances of `Job^` class."""
 
     @classmethod
     @abstractmethod
     def initialize(cls):
         raise NotImplementedError
 
     @classmethod
@@ -37,18 +37,18 @@
         raise NotImplementedError
 
     @classmethod
     @abstractmethod
     def submit_task(
         cls,
         task: Task,
-        submit_id: str = None,
+        submit_id: Optional[str] = None,
         callbacks: Optional[Iterable[Callable]] = None,
         force: bool = False,
-        wait=False,
+        wait: bool = False,
         timeout: Optional[Union[float, int]] = None,
     ) -> Job:
         raise NotImplementedError
 
     @classmethod
     @abstractmethod
     def cancel_job(cls, job):
```

### Comparing `taipy-core-2.2.3/src/taipy/core/_scheduler/_dispatcher/__init__.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/_scheduler/_dispatcher/_development_job_dispatcher.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
-from taipy.config._toml_serializer import _TomlSerializer
+from taipy.config._serializer._toml_serializer import _TomlSerializer
 from taipy.config.config import Config
 
 from ...job.job import Job
-from .._abstract_scheduler import _AbstractScheduler
+from .._abstract_orchestrator import _AbstractOrchestrator
 from ._job_dispatcher import _JobDispatcher
 
 
 class _DevelopmentJobDispatcher(_JobDispatcher):
     """Manages job dispatching (instances of `Job^` class) in a synchronous way."""
 
-    def __init__(self, scheduler: _AbstractScheduler):
-        super().__init__(scheduler)
+    def __init__(self, orchestrator: _AbstractOrchestrator):
+        super().__init__(orchestrator)
 
     def start(self):
         raise NotImplementedError
 
     def is_running(self) -> bool:
         return True
```

### Comparing `taipy-core-2.2.3/src/taipy/core/_scheduler/_dispatcher/_job_dispatcher.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,42 +9,42 @@
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import threading
 from abc import abstractmethod
 from typing import Any, Dict, List
 
-from taipy.config._toml_serializer import _TomlSerializer
+from taipy.config._serializer._toml_serializer import _TomlSerializer
 from taipy.config.config import Config
 from taipy.logger._taipy_logger import _TaipyLogger
 
-from ...common.alias import JobId
 from ...config.job_config import JobConfig
 from ...data._data_manager_factory import _DataManagerFactory
 from ...data.data_node import DataNode
 from ...exceptions.exceptions import DataNodeWritingError
 from ...job._job_manager_factory import _JobManagerFactory
 from ...job.job import Job
+from ...job.job_id import JobId
 from ...task.task import Task
-from .._abstract_scheduler import _AbstractScheduler
+from .._abstract_orchestrator import _AbstractOrchestrator
 
 
 class _JobDispatcher(threading.Thread):
     """Manages job dispatching (instances of `Job^` class) on executors."""
 
     _STOP_FLAG = False
     _dispatched_processes: Dict = {}
     __logger = _TaipyLogger._get_logger()
     _nb_available_workers: int = 1
 
-    def __init__(self, scheduler: _AbstractScheduler):
+    def __init__(self, orchestrator: _AbstractOrchestrator):
         threading.Thread.__init__(self, name="Thread-Taipy-JobDispatcher")
         self.daemon = True
-        self.scheduler = scheduler
-        self.lock = self.scheduler.lock  # type: ignore
+        self.orchestrator = orchestrator
+        self.lock = self.orchestrator.lock  # type: ignore
         Config.block_update()
 
     def start(self):
         """Start the dispatcher"""
         threading.Thread.start(self)
 
     def is_running(self) -> bool:
@@ -56,17 +56,17 @@
         self._STOP_FLAG = True
 
     def run(self):
         while not self._STOP_FLAG:
             try:
                 if self._can_execute():
                     with self.lock:
-                        job = self.scheduler.jobs_to_run.get(block=True, timeout=0.1)
+                        job = self.orchestrator.jobs_to_run.get(block=True, timeout=0.1)
                     self._execute_job(job)
-            except:  # In case the last job of the queue has been removed.  # noqa: E722
+            except Exception:  # In case the last job of the queue has been removed.
                 pass
 
     def _can_execute(self) -> bool:
         """Returns True if the dispatcher have resources to execute a new job."""
         return self._nb_available_workers > 0
 
     def _execute_job(self, job: Job):
@@ -77,19 +77,19 @@
             self._dispatch(job)
         else:
             job._unlock_edit_on_outputs()
             job.skipped()
             self.__logger.info(f"job {job.id} is skipped.")
 
     def _execute_jobs_synchronously(self):
-        while not self.scheduler.jobs_to_run.empty():
+        while not self.orchestrator.jobs_to_run.empty():
             with self.lock:
                 try:
-                    job = self.scheduler.jobs_to_run.get()
-                except:  # In case the last job of the queue has been removed.  # noqa: E722
+                    job = self.orchestrator.jobs_to_run.get()
+                except Exception:  # In case the last job of the queue has been removed.
                     self.__logger.warning(f"{job.id} is no longer in the list of jobs to run.")
             self._execute_job(job)
 
     @staticmethod
     def _needs_to_run(task: Task) -> bool:
         """
         Returns True if the task has no output or if at least one input was modified since the latest run.
```

### Comparing `taipy-core-2.2.3/src/taipy/core/_scheduler/_dispatcher/_standalone_job_dispatcher.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 from concurrent.futures import ProcessPoolExecutor
 from functools import partial
 
-from taipy.config._toml_serializer import _TomlSerializer
+from taipy.config._serializer._toml_serializer import _TomlSerializer
 from taipy.config.config import Config
 
 from ...job.job import Job
-from .._abstract_scheduler import _AbstractScheduler
+from .._abstract_orchestrator import _AbstractOrchestrator
 from ._job_dispatcher import _JobDispatcher
 
 
 class _StandaloneJobDispatcher(_JobDispatcher):
     """Manages job dispatching (instances of `Job^` class) in an asynchronous way using a ProcessPoolExecutor."""
 
-    def __init__(self, scheduler: _AbstractScheduler):
-        super().__init__(scheduler)
+    def __init__(self, orchestrator: _AbstractOrchestrator):
+        super().__init__(orchestrator)
         self._executor = ProcessPoolExecutor(Config.job_config.max_nb_of_workers or 1)  # type: ignore
         self._nb_available_workers = self._executor._max_workers  # type: ignore
 
     def _dispatch(self, job: Job):
         """Dispatches the given `Job^` on an available worker for execution.
 
         Parameters:
```

### Comparing `taipy-core-2.2.3/src/taipy/core/_scheduler/_scheduler.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_orchestrator.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,67 +16,63 @@
 from queue import Queue
 from time import sleep
 from typing import Callable, Iterable, List, Optional, Set, Union
 
 from taipy.config.config import Config
 from taipy.logger._taipy_logger import _TaipyLogger
 
-from ..common.alias import JobId
-from ..data import CSVDataNode, DataNode, ExcelDataNode, JSONDataNode, ParquetDataNode, PickleDataNode
+from .._entity._submittable import _Submittable
 from ..data._data_manager_factory import _DataManagerFactory
 from ..job._job_manager_factory import _JobManagerFactory
 from ..job.job import Job
-from ..pipeline.pipeline import Pipeline
+from ..job.job_id import JobId
 from ..task.task import Task
-from ._abstract_scheduler import _AbstractScheduler
+from ._abstract_orchestrator import _AbstractOrchestrator
 
 
-class _Scheduler(_AbstractScheduler):
+class _Orchestrator(_AbstractOrchestrator):
     """
-    Handles the functional scheduling.
-
-    Attributes:
-
+    Handles the functional orchestrating.
     """
 
     jobs_to_run: Queue = Queue()
     blocked_jobs: List = []
     lock = Lock()
     __logger = _TaipyLogger._get_logger()
 
     @classmethod
     def initialize(cls):
         pass
 
     @classmethod
     def submit(
         cls,
-        pipeline: Pipeline,
+        submittable: _Submittable,
         callbacks: Optional[Iterable[Callable]] = None,
         force: bool = False,
         wait: bool = False,
         timeout: Optional[Union[float, int]] = None,
     ) -> List[Job]:
-        """Submit the given `Pipeline^` for an execution.
+        """Submit the given `Scenario^` or `Pipeline^` for an execution.
 
         Parameters:
-             pipeline (Pipeline^): The pipeline to submit for execution.
+             submittable (Union[SCenario^, Pipeline^]): The scenario or pipeline to submit for execution.
              callbacks: The optional list of functions that should be executed on jobs status change.
-             force (bool) : Enforce execution of the pipeline's tasks even if their output data
+             force (bool) : Enforce execution of the scenario's or pipeline's tasks even if their output data
                 nodes are cached.
-             wait (bool): Wait for the scheduled jobs created from the pipeline submission to be finished in
-                asynchronous mode.
+             wait (bool): Wait for the orchestrated jobs created from the scenario or pipeline submission to be
+                finished in asynchronous mode.
              timeout (Union[float, int]): The optional maximum number of seconds to wait for the jobs to be finished
                 before returning.
         Returns:
             The created Jobs.
         """
         submit_id = cls.__generate_submit_id()
         res = []
-        tasks = pipeline._get_sorted_tasks()
+        tasks = submittable._get_sorted_tasks()
         with cls.lock:
             for ts in tasks:
                 for task in ts:
                     res.append(cls._submit_task(task, submit_id, callbacks=callbacks, force=force))
 
         if Config.job_config.is_development:
             cls._check_and_execute_jobs_if_development_mode()
@@ -85,28 +81,28 @@
                 cls.__wait_until_job_finished(res, timeout=timeout)
         return res
 
     @classmethod
     def submit_task(
         cls,
         task: Task,
-        submit_id: str = None,
+        submit_id: Optional[str] = None,
         callbacks: Optional[Iterable[Callable]] = None,
         force: bool = False,
         wait=False,
         timeout: Optional[Union[float, int]] = None,
     ) -> Job:
         """Submit the given `Task^` for an execution.
 
         Parameters:
              task (Task^): The task to submit for execution.
              submit_id (str): The optional id to differentiate each submission.
              callbacks: The optional list of functions that should be executed on job status change.
              force (bool): Enforce execution of the task even if its output data nodes are cached.
-             wait (bool): Wait for the scheduled job created from the task submission to be finished in asynchronous
+             wait (bool): Wait for the orchestrated job created from the task submission to be finished in asynchronous
                 mode.
              timeout (Union[float, int]): The optional maximum number of seconds to wait for the job to be finished
                 before returning.
         Returns:
             The created `Job^`.
         """
         with cls.lock:
@@ -119,35 +115,35 @@
                 cls.__wait_until_job_finished(job, timeout=timeout)
         return job
 
     @classmethod
     def _submit_task(
         cls,
         task: Task,
-        submit_id: str = None,
+        submit_id: Optional[str] = None,
         callbacks: Optional[Iterable[Callable]] = None,
         force: bool = False,
     ) -> Job:
         submit_id = submit_id if submit_id else cls.__generate_submit_id()
 
         for dn in task.output.values():
             dn.lock_edit()
         job = _JobManagerFactory._build_manager()._create(
             task, itertools.chain([cls._on_status_change], callbacks or []), submit_id, force=force
         )
-        cls._schedule_job_to_run_or_block(job)
+        cls._orchestrate_job_to_run_or_block(job)
 
         return job
 
     @staticmethod
     def __generate_submit_id():
         return f"SUBMISSION_{str(uuid.uuid4())}"
 
     @classmethod
-    def _schedule_job_to_run_or_block(cls, job: Job):
+    def _orchestrate_job_to_run_or_block(cls, job: Job):
         if cls._is_blocked(job):
             job.blocked()
             cls.blocked_jobs.append(job)
         else:
             job.pending()
             cls.jobs_to_run.put(job)
 
@@ -178,37 +174,17 @@
 
         Parameters:
              obj (Union[Task^, Job^]): The job or task entity to run.
 
         Returns:
              True if one of its input data nodes is blocked.
         """
-
-        data_nodes = obj.task.input.values() if isinstance(obj, Job) else obj.input.values()
+        input_data_nodes = obj.task.input.values() if isinstance(obj, Job) else obj.input.values()
         data_manager = _DataManagerFactory._build_manager()
-
-        def get_dn_is_ready_for_reading(dn: DataNode):
-            dn = data_manager._get(dn.id)
-            if dn.is_ready_for_reading is False and not dn._last_edit_date:
-                if dn.storage_type() in [
-                    CSVDataNode.storage_type(),
-                    ExcelDataNode.storage_type(),
-                    JSONDataNode.storage_type(),
-                    PickleDataNode.storage_type(),
-                    ParquetDataNode.storage_type(),
-                ]:
-                    cls.__logger.warning(
-                        f"{dn.id} cannot be read because it has never been written. Hint: The data node may refer to "
-                        f"a wrong path : {dn.path} "
-                    )
-                else:
-                    cls.__logger.warning(f"{dn.id} cannot be read because it has never been written.")
-            return dn.is_ready_for_reading
-
-        return any(not get_dn_is_ready_for_reading(dn) for dn in data_nodes)
+        return any(not data_manager._get(dn.id).is_ready_for_reading for dn in input_data_nodes)
 
     @staticmethod
     def _unlock_edit_on_jobs_outputs(jobs: Union[Job, List[Job], Set[Job]]):
         jobs = [jobs] if isinstance(jobs, Job) else jobs
         for job in jobs:
             job._unlock_edit_on_outputs()
 
@@ -293,28 +269,28 @@
             to_fail_or_abandon_jobs.update([failed_job])
             cls.__remove_blocked_jobs(to_fail_or_abandon_jobs)
             cls.__remove_jobs_to_run(to_fail_or_abandon_jobs)
             cls._unlock_edit_on_jobs_outputs(to_fail_or_abandon_jobs)
 
     @classmethod
     def _cancel_jobs(cls, job_id_to_cancel: JobId, jobs: Set[Job]):
-        from ._scheduler_factory import _SchedulerFactory
+        from ._orchestrator_factory import _OrchestratorFactory
 
         for job in jobs:
-            if job.id in _SchedulerFactory._dispatcher._dispatched_processes.keys():  # type: ignore
+            if job.id in _OrchestratorFactory._dispatcher._dispatched_processes.keys():  # type: ignore
                 cls.__logger.info(f"{job.id} is running and cannot be canceled.")
             elif job.is_completed() or job.is_skipped():
                 cls.__logger.info(f"{job.id} has already been completed and cannot be canceled.")
             elif job.is_skipped():
                 cls.__logger.info(f"{job.id} has already been skipped and cannot be canceled.")
             else:
                 if job_id_to_cancel == job.id:
                     job.canceled()
                 else:
                     job.abandoned()
 
     @staticmethod
     def _check_and_execute_jobs_if_development_mode():
-        from ._scheduler_factory import _SchedulerFactory
+        from ._orchestrator_factory import _OrchestratorFactory
 
-        if dispatcher := _SchedulerFactory._dispatcher:
+        if dispatcher := _OrchestratorFactory._dispatcher:
             dispatcher._execute_jobs_synchronously()
```

### Comparing `taipy-core-2.2.3/src/taipy/core/_scheduler/_scheduler_factory.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/_orchestrator_factory.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,47 +11,47 @@
 
 from importlib import util
 from typing import Optional, Type
 
 from taipy.config.config import Config
 
 from ..common._utils import _load_fct
-from ..exceptions.exceptions import ModeNotAvailable, SchedulerNotBuilt
-from ._abstract_scheduler import _AbstractScheduler
+from ..exceptions.exceptions import ModeNotAvailable, OrchestratorNotBuilt
+from ._abstract_orchestrator import _AbstractOrchestrator
 from ._dispatcher import _DevelopmentJobDispatcher, _JobDispatcher, _StandaloneJobDispatcher
-from ._scheduler import _Scheduler
+from ._orchestrator import _Orchestrator
 
 
-class _SchedulerFactory:
+class _OrchestratorFactory:
     _TAIPY_ENTERPRISE_MODULE = "taipy.enterprise"
-    _TAIPY_ENTERPRISE_CORE_SCHEDULER_MODULE = _TAIPY_ENTERPRISE_MODULE + ".core._scheduler._scheduler"
-    _TAIPY_ENTERPRISE_CORE_DISPATCHER_MODULE = _TAIPY_ENTERPRISE_MODULE + ".core._scheduler._dispatcher"
+    _TAIPY_ENTERPRISE_CORE_ORCHESTRATOR_MODULE = _TAIPY_ENTERPRISE_MODULE + ".core._orchestrator._orchestrator"
+    _TAIPY_ENTERPRISE_CORE_DISPATCHER_MODULE = _TAIPY_ENTERPRISE_MODULE + ".core._orchestrator._dispatcher"
     __STANDADLONE_JOB_DISPATCHER_TYPE = "_StandaloneJobDispatcher"
 
-    _scheduler: Optional[_Scheduler] = None
+    _orchestrator: Optional[_Orchestrator] = None
     _dispatcher: Optional[_JobDispatcher] = None
 
     @classmethod
-    def _build_scheduler(cls) -> Type[_AbstractScheduler]:
+    def _build_orchestrator(cls) -> Type[_AbstractOrchestrator]:
         if util.find_spec(cls._TAIPY_ENTERPRISE_MODULE) is not None:
-            cls._scheduler = _load_fct(
-                cls._TAIPY_ENTERPRISE_CORE_SCHEDULER_MODULE,
-                "Scheduler",
+            cls._orchestrator = _load_fct(
+                cls._TAIPY_ENTERPRISE_CORE_ORCHESTRATOR_MODULE,
+                "Orchestrator",
             )  # type: ignore
         else:
-            cls._scheduler = _Scheduler  # type: ignore
+            cls._orchestrator = _Orchestrator  # type: ignore
 
-        cls._scheduler.initialize()  # type: ignore
+        cls._orchestrator.initialize()  # type: ignore
 
-        return cls._scheduler  # type: ignore
+        return cls._orchestrator  # type: ignore
 
     @classmethod
     def _build_dispatcher(cls, force_restart=False) -> Optional[_JobDispatcher]:
-        if not cls._scheduler:
-            raise SchedulerNotBuilt
+        if not cls._orchestrator:
+            raise OrchestratorNotBuilt
         if Config.job_config.is_standalone:
             return cls.__build_standalone_job_dispatcher(force_restart=force_restart)
         elif Config.job_config.is_development:
             return cls.__build_development_job_dispatcher()
         else:
             raise ModeNotAvailable(f"Job mode {Config.job_config.mode} is not available.")
 
@@ -75,22 +75,22 @@
                 cls._dispatcher.stop()
             else:
                 return None
 
         if util.find_spec(cls._TAIPY_ENTERPRISE_MODULE) is not None:
             cls._dispatcher = _load_fct(
                 cls._TAIPY_ENTERPRISE_CORE_DISPATCHER_MODULE, cls.__STANDADLONE_JOB_DISPATCHER_TYPE
-            )(cls._scheduler)
+            )(cls._orchestrator)
         else:
-            cls._dispatcher = _StandaloneJobDispatcher(cls._scheduler)  # type: ignore
+            cls._dispatcher = _StandaloneJobDispatcher(cls._orchestrator)  # type: ignore
 
         cls._dispatcher.start()  # type: ignore
         return cls._dispatcher
 
     @classmethod
     def __build_development_job_dispatcher(cls) -> _JobDispatcher:
         if isinstance(cls._dispatcher, _StandaloneJobDispatcher) and not isinstance(
             cls._dispatcher, _DevelopmentJobDispatcher
         ):
             cls._dispatcher.stop()
-        cls._dispatcher = _DevelopmentJobDispatcher(cls._scheduler)  # type: ignore
+        cls._dispatcher = _DevelopmentJobDispatcher(cls._orchestrator)  # type: ignore
         return cls._dispatcher
```

### Comparing `taipy-core-2.2.3/src/taipy/core/_version/__init__.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/_version/_utils.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_manager_factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,20 +5,24 @@
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
+from typing import Type
 
-def _version_migration() -> str:
-    """Add version attribute on old entities. Used to migrate from <=2.0 to >=2.1 version."""
-    from ._version_cli import _VersioningCLI
-    from ._version_manager import _VersionManager
+from .._manager._manager_factory import _ManagerFactory
+from ..common._utils import _load_fct
+from ._version_manager import _VersionManager
+from ._version_repository_factory import _VersionRepositoryFactory
 
-    _VersioningCLI._create_parser()
-    mode = _VersioningCLI._parse_arguments()[0]
-    if mode != "development":
-        return _VersionManager._get_latest_version()
-    else:
-        _VersionManager._get_or_create("LEGACY-VERSION", True)
-        return "LEGACY-VERSION"
+
+class _VersionManagerFactory(_ManagerFactory):
+    @classmethod
+    def _build_manager(cls) -> Type[_VersionManager]:  # type: ignore
+        if cls._using_enterprise():
+            return _load_fct(
+                cls._TAIPY_ENTERPRISE_CORE_MODULE + "._version._version_manager", "_VersionManager"
+            )  # type: ignore
+        _VersionManager._repository = _VersionRepositoryFactory._build_repository()  # type: ignore
+        return _VersionManager
```

### Comparing `taipy-core-2.2.3/src/taipy/core/_version/_version.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_version/_version.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from datetime import datetime
 from typing import Any
 
 from taipy.config import Config
 from taipy.config._config import _Config
 
-from ..common._entity import _Entity
+from .._entity._entity import _Entity
 
 
 class _Version(_Entity):
     def __init__(self, id: str, config: Any) -> None:
         self.id: str = id
         self.config: _Config = config
         self.creation_date: datetime = datetime.now()
```

### Comparing `taipy-core-2.2.3/src/taipy/core/_version/_version_fs_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_fs_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,33 +119,33 @@
             json.dumps(
                 file_content,
                 ensure_ascii=False,
                 indent=0,
             )
         )
 
-    def _get_production_version(self) -> List[str]:
+    def _get_production_versions(self) -> List[str]:
         with open(self._version_file_path, "r") as f:
             file_content = json.load(f)
 
         return file_content[self._PRODUCTION_VERSION_KEY]
 
     def _delete_production_version(self, version_number):
         try:
             with open(self._version_file_path, "r") as f:
                 file_content = json.load(f)
 
             if version_number not in file_content[self._PRODUCTION_VERSION_KEY]:
-                raise VersionIsNotProductionVersion(f"Version {version_number} is not a production version.")
+                raise VersionIsNotProductionVersion(f"Version '{version_number}' is not a production version.")
 
             file_content[self._PRODUCTION_VERSION_KEY].remove(version_number)
 
             self._version_file_path.write_text(
                 json.dumps(
                     file_content,
                     ensure_ascii=False,
                     indent=0,
                 )
             )
 
         except FileNotFoundError:
-            raise VersionIsNotProductionVersion(f"Version {version_number} is not a production version.")
+            raise VersionIsNotProductionVersion(f"Version '{version_number}' is not a production version.")
```

### Comparing `taipy-core-2.2.3/src/taipy/core/_version/_version_manager.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,62 +9,59 @@
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import uuid
 from typing import List, Optional, Union
 
 from taipy.config import Config
-from taipy.config._config_comparator import _ConfigComparator
+from taipy.config._config_comparator._comparator_result import _ComparatorResult
 from taipy.config.exceptions.exceptions import InconsistentEnvVariableError
 from taipy.logger._taipy_logger import _TaipyLogger
 
 from .._manager._manager import _Manager
-from ..exceptions.exceptions import ModelNotFound, NonExistingVersion, VersionConflictWithPythonConfig
+from ..exceptions.exceptions import ModelNotFound, NonExistingVersion
 from ._version import _Version
 from ._version_repository_factory import _VersionRepositoryFactory
 
 
 class _VersionManager(_Manager[_Version]):
     _ENTITY_NAME = _Version.__name__
 
+    __logger = _TaipyLogger._get_logger()
+
     __DEVELOPMENT_VERSION = ["development", "dev"]
     __LATEST_VERSION = "latest"
     __PRODUCTION_VERSION = "production"
     __ALL_VERSION = ["all", ""]
 
     __DEFAULT_VERSION = __LATEST_VERSION
 
-    _repository = _VersionRepositoryFactory._build_repository()  # type: ignore
+    _repository = _VersionRepositoryFactory._build_repository()
 
     @classmethod
     def _get(cls, entity: Union[str, _Version], default=None) -> _Version:
         """
         Returns the version entity by id or reference.
         """
-        entity_id = entity if isinstance(entity, str) else entity.id  # type: ignore
+        entity_id = entity if isinstance(entity, str) else entity.id
         try:
             return cls._repository.load(entity_id)
         except ModelNotFound:
             return default
 
     @classmethod
     def _get_or_create(cls, id: str, force: bool) -> _Version:
         if version := cls._get(id):
-            config_diff = _ConfigComparator(version.config, Config._applied_config)
-            if config_diff["added_items"] or config_diff["removed_items"] or config_diff["modified_items"]:
-                _TaipyLogger._get_logger().warning(
-                    f"The Configuration of version {id} is conflicted with the current Python Config."
-                )
-
+            comparator_result = Config._comparator._find_conflict_config(version.config, Config._applied_config, id)
+            if comparator_result.get(_ComparatorResult.CONFLICTED_SECTION_KEY):
                 if force:
                     _TaipyLogger._get_logger().warning(f"Overriding version {id} ...")
                     version.config = Config._applied_config
                 else:
-                    raise VersionConflictWithPythonConfig(config_diff)
-
+                    raise SystemExit("The application is stopped. Please check the error log for more information.")
         else:
             version = _Version(id=id, config=Config._applied_config)
 
         cls._set(version)
         return version
 
     @classmethod
@@ -87,106 +84,135 @@
         cls._repository._set_development_version(version_number)
         return version_number
 
     @classmethod
     def _get_development_version(cls) -> str:
         try:
             return cls._repository._get_development_version()
-        except:  # noqa: E722
+        except (FileNotFoundError, ModelNotFound):
             return cls._set_development_version(str(uuid.uuid4()))
 
     @classmethod
-    def _set_experiment_version(cls, version_number: str, force: bool) -> str:
+    def _set_experiment_version(cls, version_number: str, force: bool = False) -> str:
         if version_number == cls._get_development_version():
             raise SystemExit(
                 f"Version number {version_number} is already a development version. Please choose a different version "
                 f"number for experiment mode. "
             )
 
-        if version_number in cls._get_production_version():
+        if version_number in cls._get_production_versions():
             raise SystemExit(
                 f"Version number {version_number} is already a production version. Please choose a different version "
                 f"number for experiment mode. "
             )
 
         cls._get_or_create(version_number, force)
         cls._repository._set_latest_version(version_number)
         return version_number
 
     @classmethod
     def _get_latest_version(cls) -> str:
         try:
             return cls._repository._get_latest_version()
-        except:  # noqa: E722
+        except (FileNotFoundError, ModelNotFound):
             # If there is no version in the system yet, create a new version as development version
             # This set the default versioning behavior on Jupyter notebook to Development mode
             return cls._set_development_version(str(uuid.uuid4()))
 
     @classmethod
-    def _set_production_version(cls, version_number: str, force: bool) -> str:
-        production_versions = cls._get_production_version()
+    def _set_production_version(cls, version_number: str, force: bool = False) -> str:
+        production_versions = cls._get_production_versions()
 
         # Check if all previous production versions are compatible with current Python Config
         for production_version in production_versions:
             if production_version == version_number:
                 continue
 
             if version := cls._get(production_version):
-                config_diff = _ConfigComparator(version.config, Config._applied_config)
-                if config_diff["added_items"] or config_diff["removed_items"] or config_diff["modified_items"]:
-                    _TaipyLogger._get_logger().error(
-                        f"The Configuration of version {production_version} is conflicted with the current Python"
-                        " Config."
-                    )
-                    raise VersionConflictWithPythonConfig(config_diff)
+                comparator_result = Config._comparator._find_conflict_config(
+                    version.config, Config._applied_config, production_version
+                )
+                if comparator_result.get(_ComparatorResult.CONFLICTED_SECTION_KEY):
+                    raise SystemExit("The application is stopped. Please check the error log for more information.")
+
             else:
                 raise NonExistingVersion(production_version)
 
         if version_number == cls._get_development_version():
             cls._set_development_version(str(uuid.uuid4()))
 
         cls._get_or_create(version_number, force)
         cls._repository._set_production_version(version_number)
         return version_number
 
     @classmethod
-    def _get_production_version(cls) -> List[str]:
+    def _get_production_versions(cls) -> List[str]:
         try:
-            return cls._repository._get_production_version()
-        except:  # noqa: E722
+            return cls._repository._get_production_versions()
+        except (FileNotFoundError, ModelNotFound):
             return []
 
     @classmethod
     def _delete_production_version(cls, version_number) -> str:
         return cls._repository._delete_production_version(version_number)
 
     @classmethod
-    def _replace_version_number(cls, version_number):
+    def _replace_version_number(cls, version_number: Optional[str]):
         if version_number is None:
             version_number = cls._replace_version_number(cls.__DEFAULT_VERSION)
 
-            production_versions = cls._get_production_version()
+            production_versions = cls._get_production_versions()
 
             if version_number not in production_versions:
                 return version_number
             return production_versions
 
         if version_number == cls.__LATEST_VERSION:
             return cls._get_latest_version()
         if version_number in cls.__DEVELOPMENT_VERSION:
             return cls._get_development_version()
         if version_number in cls.__PRODUCTION_VERSION:
-            return cls._get_production_version()
+            return cls._get_production_versions()
         if version_number in cls.__ALL_VERSION:
             return ""
 
         try:
             if version := cls._get(version_number):
                 return version.id
         except InconsistentEnvVariableError:  # The version exist but the Config is alternated
             return version_number
 
         raise NonExistingVersion(version_number)
 
     @classmethod
     def _delete_entities_of_multiple_types(cls, _entity_ids):
         return NotImplementedError
+
+    @classmethod
+    def _manage_version(cls):
+        from ..taipy import clean_all_entities_by_version
+
+        if Config.core.mode == "development":
+            current_version_number = cls._get_development_version()
+            cls.__logger.info(f"Development mode: Clean all entities of version {current_version_number}")
+            clean_all_entities_by_version(current_version_number)
+            cls._set_development_version(current_version_number)
+
+        elif Config.core.mode in ["experiment", "production"]:
+            default_version_number = {
+                "experiment": str(uuid.uuid4()),
+                "production": cls._get_latest_version(),
+            }
+            version_setter = {
+                "experiment": cls._set_experiment_version,
+                "production": cls._set_production_version,
+            }
+            if Config.core.version_number:
+                current_version_number = Config.core.version_number
+            else:
+                current_version_number = default_version_number[Config.core.mode]
+            if Config.core.clean_entities:
+                if clean_all_entities_by_version(current_version_number):
+                    cls.__logger.info(f"Clean all entities of version {current_version_number}")
+            version_setter[Config.core.mode](current_version_number, Config.core.force)
+        else:
+            raise SystemExit(f"Undefined execution mode: {Config.core.mode}.")
```

### Comparing `taipy-core-2.2.3/src/taipy/core/_version/_version_manager_factory.py` & `taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_manager_factory.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 from typing import Type
 
 from .._manager._manager_factory import _ManagerFactory
 from ..common._utils import _load_fct
-from ._version_manager import _VersionManager
-from ._version_repository_factory import _VersionRepositoryFactory
+from ._scenario_manager import _ScenarioManager
+from ._scenario_repository_factory import _ScenarioRepositoryFactory
 
 
-class _VersionManagerFactory(_ManagerFactory):
+class _ScenarioManagerFactory(_ManagerFactory):
     @classmethod
-    def _build_manager(cls) -> Type[_VersionManager]:  # type: ignore
+    def _build_manager(cls) -> Type[_ScenarioManager]:  # type: ignore
         if cls._using_enterprise():
             return _load_fct(
-                cls._TAIPY_ENTERPRISE_CORE_MODULE + "._version._version_manager", "_VersionManager"
+                cls._TAIPY_ENTERPRISE_CORE_MODULE + ".scenario._scenario_manager", "_ScenarioManager"
             )  # type: ignore
-        _VersionManager._repository = _VersionRepositoryFactory._build_repository()  # type: ignore
-        return _VersionManager
+        _ScenarioManager._repository = _ScenarioRepositoryFactory._build_repository()  # type: ignore
+        return _ScenarioManager
```

### Comparing `taipy-core-2.2.3/src/taipy/core/_version/_version_model.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/_version/_version_repository_factory.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/_version/_version_sql_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_version/_version_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/common/__init__.py` & `taipy-core-2.3.0.dev0/src/taipy/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/common/_entity.py` & `taipy-core-2.3.0.dev0/src/taipy/core/scenario/scenario_id.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,21 +5,11 @@
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
-from ._reload import _set_entity
+from typing import NewType
 
-
-class _Entity:
-    _MANAGER_NAME: str
-    _is_in_context = False
-
-    def __enter__(self):
-        self._is_in_context = True
-        return self
-
-    def __exit__(self, exc_type, exc_value, exc_traceback):
-        self._is_in_context = False
-        _set_entity(self._MANAGER_NAME, self)
+ScenarioId = NewType("ScenarioId", str)
+ScenarioId.__doc__ = """Type that holds a `Scenario^` identifier."""
```

### Comparing `taipy-core-2.2.3/src/taipy/core/common/_entity_ids.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_entity/_entity_ids.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/common/_get_valid_filename.py` & `taipy-core-2.3.0.dev0/src/taipy/core/cycle/cycle_id.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,24 +5,11 @@
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
-import re
+from typing import NewType
 
-
-class _SuspiciousFileOperation(Exception):
-    pass
-
-
-def _get_valid_filename(name: str) -> str:
-    """
-    Source: https://github.com/django/django/blob/main/django/utils/text.py
-    """
-    s = str(name).strip().replace(" ", "_")
-    s = re.sub(r"(?u)[^-\w.]", "", s)
-    if s in {"", ".", ".."}:
-        raise _SuspiciousFileOperation("Could not derive file name from '%s'" % name)
-    s = str(s).strip().replace(" ", "_")
-    return re.sub(r"(?u)[^-\w.]", "", s)
+CycleId = NewType("CycleId", str)
+CycleId.__doc__ = """Type that holds a `Cycle^` identifier."""
```

### Comparing `taipy-core-2.2.3/src/taipy/core/common/_listattributes.py` & `taipy-core-2.3.0.dev0/src/taipy/core/common/_listattributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     def __set_self(self):
         from ... import core as tp
 
         if hasattr(self, "_parent"):
             tp.set(self._parent)
 
     def __add__(self, value):
+        # TODO: publish event of changing attributes
         if hasattr(value, "__iter__"):
             self.__add_iterable(value)
         else:
             self.append(value)
         return self
 
     def extend(self, value) -> None:
```

### Comparing `taipy-core-2.2.3/src/taipy/core/common/_reload.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_entity/_reload.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import functools
 
+from ..notification import EventEntityType, EventOperation, _publish_event
+
 
 @functools.lru_cache
 def _get_manager(manager: str):
     from ..cycle._cycle_manager_factory import _CycleManagerFactory
     from ..data._data_manager_factory import _DataManagerFactory
     from ..job._job_manager_factory import _JobManagerFactory
     from ..pipeline._pipeline_manager_factory import _PipelineManagerFactory
@@ -31,25 +33,23 @@
     }[manager]
 
 
 def _reload(manager: str, obj):
     return _get_manager(manager)._get(obj, obj)
 
 
-def _set_entity(manager: str, obj):
-    _get_manager(manager)._set(obj)
-
-
 def _self_setter(manager):
     def __set_entity(fct):
         @functools.wraps(fct)
         def _do_set_entity(self, *args, **kwargs):
             fct(self, *args, **kwargs)
             if not self._is_in_context:
-                _set_entity(manager, self)
+                entity_manager = _get_manager(manager)
+                entity_manager._set(self)
+                _publish_event(entity_manager._EVENT_ENTITY_TYPE, self.id, EventOperation.UPDATE, fct.__name__)
 
         return _do_set_entity
 
     return __set_entity
 
 
 def _self_reload(manager):
```

### Comparing `taipy-core-2.2.3/src/taipy/core/common/_repr_enum.py` & `taipy-core-2.3.0.dev0/src/taipy/core/common/_repr_enum.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/common/_utils.py` & `taipy-core-2.3.0.dev0/src/taipy/core/common/_utils.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/common/_warnings.py` & `taipy-core-2.3.0.dev0/src/taipy/core/common/_warnings.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,33 +7,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import functools
 import warnings
+from typing import Optional
 
 warnings.simplefilter("once", ResourceWarning)
 
 
-def _warn_deprecated(deprecated: str, suggest: str = None, stacklevel: int = 3) -> None:
+def _warn_deprecated(deprecated: str, suggest: Optional[str] = None, stacklevel: int = 3) -> None:
     category = DeprecationWarning
     message = f"{deprecated} is deprecated."
     if suggest:
         message += f" Use {suggest} instead."
     warnings.warn(message=message, category=category, stacklevel=stacklevel)
 
 
 def _warn_no_core_service(stacklevel: int = 3):
     def inner(f):
         @functools.wraps(f)
         def _check_if_core_service_is_running(*args, **kwargs):
-            from .._scheduler._scheduler_factory import _SchedulerFactory
+            from .._orchestrator._orchestrator_factory import _OrchestratorFactory
 
-            if not _SchedulerFactory._dispatcher:
+            if not _OrchestratorFactory._dispatcher:
                 message = "The Core service is NOT running"
                 warnings.warn(message=message, category=ResourceWarning, stacklevel=stacklevel)
 
             return f(*args, **kwargs)
 
         return _check_if_core_service_is_running
```

### Comparing `taipy-core-2.2.3/src/taipy/core/common/default_custom_document.py` & `taipy-core-2.3.0.dev0/src/taipy/core/common/default_custom_document.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/config/__init__.py` & `taipy-core-2.3.0.dev0/src/taipy/core/config/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,33 +4,42 @@
 # the License. You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
+
 from taipy.config import _inject_section
 from taipy.config.checker._checker import _Checker
 from taipy.config.common.frequency import Frequency  # type: ignore
 from taipy.config.common.scope import Scope  # type: ignore
 from taipy.config.config import Config  # type: ignore
 from taipy.config.global_app.global_app_config import GlobalAppConfig  # type: ignore
 
+from ._core_section import CoreSection
+from .checkers._config_id_checker import _ConfigIdChecker
 from .checkers._data_node_config_checker import _DataNodeConfigChecker
 from .checkers._job_config_checker import _JobConfigChecker
 from .checkers._pipeline_config_checker import _PipelineConfigChecker
 from .checkers._scenario_config_checker import _ScenarioConfigChecker
 from .checkers._task_config_checker import _TaskConfigChecker
 from .data_node_config import DataNodeConfig
 from .job_config import JobConfig
 from .pipeline_config import PipelineConfig
 from .scenario_config import ScenarioConfig
 from .task_config import TaskConfig
 
-_inject_section(JobConfig, "job_config", JobConfig("development"), [("configure_job_executions", JobConfig._configure)])
+_inject_section(
+    JobConfig,
+    "job_config",
+    JobConfig("development"),
+    [("configure_job_executions", JobConfig._configure)],
+    add_to_unconflicted_sections=True,
+)
 _inject_section(
     DataNodeConfig,
     "data_nodes",
     DataNodeConfig.default_config(),
     [
         ("configure_data_node", DataNodeConfig._configure),
         ("configure_default_data_node", DataNodeConfig._configure_default),
@@ -67,13 +76,21 @@
     ScenarioConfig.default_config(),
     [
         ("configure_scenario", ScenarioConfig._configure),
         ("configure_default_scenario", ScenarioConfig._configure_default),
         ("configure_scenario_from_tasks", ScenarioConfig._configure_from_tasks),
     ],
 )
+_inject_section(
+    CoreSection,
+    "core",
+    CoreSection.default_config(),
+    [("configure_core", CoreSection._configure)],
+    add_to_unconflicted_sections=True,
+)
 
+_Checker.add_checker(_ConfigIdChecker)
 _Checker.add_checker(_JobConfigChecker)
 _Checker.add_checker(_DataNodeConfigChecker)
 _Checker.add_checker(_TaskConfigChecker)
 _Checker.add_checker(_PipelineConfigChecker)
 _Checker.add_checker(_ScenarioConfigChecker)
```

### Comparing `taipy-core-2.2.3/src/taipy/core/config/checkers/__init__.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_orchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/config/checkers/_data_node_config_checker.py` & `taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_data_node_config_checker.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,107 +23,157 @@
     def __init__(self, config: _Config, collector: IssueCollector):
         super().__init__(config, collector)
 
     def _check(self) -> IssueCollector:
         data_node_configs: Dict[str, DataNodeConfig] = self._config._sections[DataNodeConfig.name]
         for data_node_config_id, data_node_config in data_node_configs.items():
             self._check_existing_config_id(data_node_config)
+            self._check_if_entity_property_key_used_is_predefined(data_node_config)
             self._check_storage_type(data_node_config_id, data_node_config)
             self._check_scope(data_node_config_id, data_node_config)
             self._check_required_properties(data_node_config_id, data_node_config)
-            self._check_generic_read_write_fct(data_node_config_id, data_node_config)
-            self._check_generic_read_write_fct_params(data_node_config_id, data_node_config)
+            self._check_callable(data_node_config_id, data_node_config)
+            self._check_generic_read_write_fct_and_args(data_node_config_id, data_node_config)
             self._check_exposed_type(data_node_config_id, data_node_config)
         return self._collector
 
     def _check_storage_type(self, data_node_config_id: str, data_node_config: DataNodeConfig):
         if data_node_config.storage_type not in DataNodeConfig._ALL_STORAGE_TYPES:
             self._error(
                 data_node_config._STORAGE_TYPE_KEY,
                 data_node_config.storage_type,
-                f"`{data_node_config._STORAGE_TYPE_KEY}` field of DataNode `{data_node_config_id}` must be either csv, "
-                f"sql_table, sql, mongo_collection, pickle, excel, generic, json, parquet or in_memory.",
+                f"`{data_node_config._STORAGE_TYPE_KEY}` field of DataNodeConfig `{data_node_config_id}` must be"
+                f" either csv, sql_table, sql, mongo_collection, pickle, excel, generic, json, parquet, or in_memory.",
             )
 
     def _check_scope(self, data_node_config_id: str, data_node_config: DataNodeConfig):
         if not isinstance(data_node_config.scope, Scope):
             self._error(
                 data_node_config._SCOPE_KEY,
                 data_node_config.scope,
-                f"`{data_node_config._SCOPE_KEY}` field of DataNode `{data_node_config_id}` must be populated with a "
-                f"Scope value.",
+                f"`{data_node_config._SCOPE_KEY}` field of DataNodeConfig `{data_node_config_id}` must be"
+                f" populated with a Scope value.",
             )
 
     def _check_required_properties(self, data_node_config_id: str, data_node_config: DataNodeConfig):
         if storage_type := data_node_config.storage_type:
             if storage_type in DataNodeConfig._REQUIRED_PROPERTIES:
                 required_properties = DataNodeConfig._REQUIRED_PROPERTIES[storage_type]
                 if storage_type == DataNodeConfig._STORAGE_TYPE_VALUE_SQL:
                     if data_node_config.properties:
                         if engine := data_node_config.properties.get(DataNodeConfig._REQUIRED_DB_ENGINE_SQL_PROPERTY):
-                            if engine == DataNodeConfig._REQUIRED_DB_ENGINE_SQLITE:
+                            if engine == DataNodeConfig._DB_ENGINE_SQLITE:
                                 required_properties = [
                                     DataNodeConfig._REQUIRED_DB_NAME_SQL_PROPERTY,
                                     DataNodeConfig._REQUIRED_DB_ENGINE_SQL_PROPERTY,
                                     DataNodeConfig._REQUIRED_READ_QUERY_SQL_PROPERTY,
                                     DataNodeConfig._REQUIRED_WRITE_QUERY_BUILDER_SQL_PROPERTY,
                                 ]
+                            else:
+                                required_properties = [
+                                    DataNodeConfig._OPTIONAL_DB_USERNAME_SQL_PROPERTY,
+                                    DataNodeConfig._OPTIONAL_DB_PASSWORD_SQL_PROPERTY,
+                                    DataNodeConfig._REQUIRED_DB_NAME_SQL_PROPERTY,
+                                    DataNodeConfig._REQUIRED_DB_ENGINE_SQL_PROPERTY,
+                                    DataNodeConfig._REQUIRED_READ_QUERY_SQL_PROPERTY,
+                                    DataNodeConfig._REQUIRED_WRITE_QUERY_BUILDER_SQL_PROPERTY,
+                                ]
                 if storage_type == DataNodeConfig._STORAGE_TYPE_VALUE_SQL_TABLE:
                     if data_node_config.properties:
                         if engine := data_node_config.properties.get(DataNodeConfig._REQUIRED_DB_ENGINE_SQL_PROPERTY):
-                            if engine == DataNodeConfig._REQUIRED_DB_ENGINE_SQLITE:
+                            if engine == DataNodeConfig._DB_ENGINE_SQLITE:
+                                required_properties = [
+                                    DataNodeConfig._REQUIRED_DB_NAME_SQL_PROPERTY,
+                                    DataNodeConfig._REQUIRED_DB_ENGINE_SQL_PROPERTY,
+                                    DataNodeConfig._REQUIRED_TABLE_NAME_SQL_TABLE_PROPERTY,
+                                ]
+                            else:
                                 required_properties = [
+                                    DataNodeConfig._OPTIONAL_DB_USERNAME_SQL_PROPERTY,
+                                    DataNodeConfig._OPTIONAL_DB_PASSWORD_SQL_PROPERTY,
                                     DataNodeConfig._REQUIRED_DB_NAME_SQL_PROPERTY,
                                     DataNodeConfig._REQUIRED_DB_ENGINE_SQL_PROPERTY,
-                                    DataNodeConfig._REQUIRED_TABLE_NAME_PROPERTY,
+                                    DataNodeConfig._REQUIRED_TABLE_NAME_SQL_TABLE_PROPERTY,
                                 ]
                 for required_property in required_properties:
                     if not data_node_config.properties or required_property not in data_node_config.properties:
-                        self._error(
-                            "properties",
-                            required_property,
-                            f"`{data_node_config_id}` DataNode is missing the required "
-                            f"property `{required_property}` for type `{storage_type}`",
-                        )
+                        if data_node_config_id == DataNodeConfig._DEFAULT_KEY:
+                            self._warning(
+                                required_property,
+                                None,
+                                f"DataNodeConfig `{data_node_config_id}` is missing the required "
+                                f"property `{required_property}` for type `{storage_type}`.",
+                            )
+                        else:
+                            self._error(
+                                required_property,
+                                None,
+                                f"DataNodeConfig `{data_node_config_id}` is missing the required "
+                                f"property `{required_property}` for type `{storage_type}`.",
+                            )
 
-    def _check_generic_read_write_fct_params(self, data_node_config_id: str, data_node_config: DataNodeConfig):
+    def _check_generic_read_write_fct_and_args(self, data_node_config_id: str, data_node_config: DataNodeConfig):
         if data_node_config.storage_type == DataNodeConfig._STORAGE_TYPE_VALUE_GENERIC:
             properties_to_check = [
-                DataNodeConfig._OPTIONAL_READ_FUNCTION_PARAMS_GENERIC_PROPERTY,
-                DataNodeConfig._OPTIONAL_WRITE_FUNCTION_PARAMS_GENERIC_PROPERTY,
+                DataNodeConfig._OPTIONAL_READ_FUNCTION_ARGS_GENERIC_PROPERTY,
+                DataNodeConfig._OPTIONAL_WRITE_FUNCTION_ARGS_GENERIC_PROPERTY,
             ]
             for prop_key in properties_to_check:
                 if data_node_config.properties and prop_key in data_node_config.properties:
                     prop_value = data_node_config.properties[prop_key]
-                    if not isinstance(prop_value, tuple):  # type: ignore
+                    if not isinstance(prop_value, list):
                         self._error(
                             prop_key,
                             prop_value,
-                            f"`{prop_key}` field of DataNode"
-                            f" `{data_node_config_id}` must be populated with a Tuple value.",
+                            f"`{prop_key}` field of DataNodeConfig"
+                            f" `{data_node_config_id}` must be populated with a List value.",
                         )
+            if data_node_config_id != DataNodeConfig._DEFAULT_KEY:
+                properties_to_check_at_least_one = [
+                    DataNodeConfig._OPTIONAL_READ_FUNCTION_GENERIC_PROPERTY,
+                    DataNodeConfig._OPTIONAL_WRITE_FUNCTION_GENERIC_PROPERTY,
+                ]
+                has_at_least_one = False
+                for prop_key in properties_to_check_at_least_one:
+                    if data_node_config.properties and prop_key in data_node_config.properties:
+                        has_at_least_one = True
+                if not has_at_least_one:
+                    self._error(
+                        ", ".join(properties_to_check_at_least_one),
+                        None,
+                        f"Either `{DataNodeConfig._OPTIONAL_READ_FUNCTION_GENERIC_PROPERTY}` field or "
+                        f"`{DataNodeConfig._OPTIONAL_WRITE_FUNCTION_GENERIC_PROPERTY}` field of "
+                        f"DataNodeConfig `{data_node_config_id}` must be populated with a Callable function.",
+                    )
 
-    def _check_generic_read_write_fct(self, data_node_config_id: str, data_node_config: DataNodeConfig):
-        if data_node_config.storage_type == DataNodeConfig._STORAGE_TYPE_VALUE_GENERIC:
-            properties_to_check = [
-                DataNodeConfig._REQUIRED_READ_FUNCTION_GENERIC_PROPERTY,
-                DataNodeConfig._REQUIRED_WRITE_FUNCTION_GENERIC_PROPERTY,
-            ]
-            for prop_key in properties_to_check:
+    def _check_callable(self, data_node_config_id: str, data_node_config: DataNodeConfig):
+        properties_to_check = {
+            DataNodeConfig._STORAGE_TYPE_VALUE_GENERIC: [
+                DataNodeConfig._OPTIONAL_READ_FUNCTION_GENERIC_PROPERTY,
+                DataNodeConfig._OPTIONAL_WRITE_FUNCTION_GENERIC_PROPERTY,
+            ],
+            DataNodeConfig._STORAGE_TYPE_VALUE_SQL: [
+                DataNodeConfig._REQUIRED_WRITE_QUERY_BUILDER_SQL_PROPERTY,
+            ],
+        }
+
+        if data_node_config.storage_type in properties_to_check.keys():
+            for prop_key in properties_to_check[data_node_config.storage_type]:
                 prop_value = data_node_config.properties.get(prop_key) if data_node_config.properties else None
                 if prop_value and not callable(prop_value):
                     self._error(
                         prop_key,
                         prop_value,
-                        f"`{prop_key}` of DataNode `{data_node_config_id}` must be populated with a Callable function.",
+                        f"`{prop_key}` of DataNodeConfig `{data_node_config_id}` must be"
+                        f" populated with a Callable function.",
                     )
 
     def _check_exposed_type(self, data_node_config_id: str, data_node_config: DataNodeConfig):
         if not isinstance(data_node_config.exposed_type, str):
             return
         if data_node_config.exposed_type not in DataNodeConfig._ALL_EXPOSED_TYPES:
             self._error(
                 data_node_config._EXPOSED_TYPE_KEY,
                 data_node_config.exposed_type,
-                f"The `{data_node_config._EXPOSED_TYPE_KEY}` of the DataNodeConfig `{data_node_config_id}` "
-                f'must be either "pandas", "modin", "numpy" or a custom type.',
+                f"The `{data_node_config._EXPOSED_TYPE_KEY}` of DataNodeConfig `{data_node_config_id}` "
+                f'must be either "pandas", "modin", "numpy", or a custom type.',
             )
```

### Comparing `taipy-core-2.2.3/src/taipy/core/config/checkers/_job_config_checker.py` & `taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_job_config_checker.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,10 +32,10 @@
     def _check_multiprocess_mode(self, job_config: JobConfig, data_node_configs: Dict[str, DataNodeConfig]):
         if job_config.is_standalone:
             for cfg_id, data_node_config in data_node_configs.items():
                 if data_node_config.storage_type == DataNodeConfig._STORAGE_TYPE_VALUE_IN_MEMORY:
                     self._error(
                         DataNodeConfig._STORAGE_TYPE_KEY,
                         data_node_config.storage_type,
-                        f"DataNode {cfg_id}: In-memory storage type can ONLY be used in "
-                        f"{JobConfig._DEVELOPMENT_MODE} mode",
+                        f"DataNode `{cfg_id}`: In-memory storage type can ONLY be used in "
+                        f"{JobConfig._DEVELOPMENT_MODE} mode.",
                     )
```

### Comparing `taipy-core-2.2.3/src/taipy/core/config/checkers/_pipeline_config_checker.py` & `taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_pipeline_config_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     def __init__(self, config: _Config, collector: IssueCollector):
         super().__init__(config, collector)
 
     def _check(self) -> IssueCollector:
         pipeline_configs = self._config._sections[PipelineConfig.name]
         for pipeline_config_id, pipeline_config in pipeline_configs.items():
             if pipeline_config_id != _Config.DEFAULT_KEY:
+                self._check_if_entity_property_key_used_is_predefined(pipeline_config)
                 self._check_existing_config_id(pipeline_config)
                 self._check_tasks(pipeline_config_id, pipeline_config)
         return self._collector
 
     def _check_tasks(self, pipeline_config_id: str, pipeline_config: PipelineConfig):
         self._check_children(
             PipelineConfig, pipeline_config_id, pipeline_config._TASK_KEY, pipeline_config.tasks, TaskConfig
```

### Comparing `taipy-core-2.2.3/src/taipy/core/config/checkers/_scenario_config_checker.py` & `taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_scenario_config_checker.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     def __init__(self, config: _Config, collector: IssueCollector):
         super().__init__(config, collector)
 
     def _check(self) -> IssueCollector:
         scenario_configs = self._config._sections[ScenarioConfig.name]
         for scenario_config_id, scenario_config in scenario_configs.items():
             if scenario_config_id != _Config.DEFAULT_KEY:
+                self._check_if_entity_property_key_used_is_predefined(scenario_config)
                 self._check_existing_config_id(scenario_config)
                 self._check_frequency(scenario_config_id, scenario_config)
                 self._check_pipelines(scenario_config_id, scenario_config)
                 self._check_comparators(scenario_config_id, scenario_config)
         return self._collector
 
     def _check_pipelines(self, scenario_config_id: str, scenario_config: ScenarioConfig):
@@ -42,18 +43,18 @@
         )
 
     def _check_frequency(self, scenario_config_id: str, scenario_config: ScenarioConfig):
         if scenario_config.frequency and not isinstance(scenario_config.frequency, Frequency):
             self._error(
                 scenario_config._FREQUENCY_KEY,
                 scenario_config.frequency,
-                f"{scenario_config._FREQUENCY_KEY} field of Scenario {scenario_config_id} must be populated with a "
-                f"Frequency value.",
+                f"{scenario_config._FREQUENCY_KEY} field of ScenarioConfig `{scenario_config_id}` must be"
+                f" populated with a Frequency value.",
             )
 
     def _check_comparators(self, scenario_config_id: str, scenario_config: ScenarioConfig):
         if not scenario_config.comparators:
             self._info(
                 scenario_config._COMPARATOR_KEY,
                 scenario_config.comparators,
-                f"No scenario {scenario_config._COMPARATOR_KEY} defined for scenario {scenario_config_id}",
+                f"No scenario {scenario_config._COMPARATOR_KEY} defined for ScenarioConfig `{scenario_config_id}`.",
             )
```

### Comparing `taipy-core-2.2.3/src/taipy/core/config/checkers/_task_config_checker.py` & `taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/_task_config_checker.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         super().__init__(config, collector)
 
     def _check(self) -> IssueCollector:
         task_configs = self._config._sections[TaskConfig.name]
         for task_config_id, task_config in task_configs.items():
             if task_config_id != _Config.DEFAULT_KEY:
                 self._check_existing_config_id(task_config)
+                self._check_if_entity_property_key_used_is_predefined(task_config)
                 self._check_existing_function(task_config_id, task_config)
                 self._check_inputs(task_config_id, task_config)
                 self._check_outputs(task_config_id, task_config)
         return self._collector
 
     def _check_inputs(self, task_config_id: str, task_config: TaskConfig):
         self._check_children(
@@ -42,16 +43,17 @@
         )
 
     def _check_existing_function(self, task_config_id: str, task_config: TaskConfig):
         if not task_config.function:
             self._error(
                 task_config._FUNCTION,
                 task_config.function,
-                f"{task_config._FUNCTION} field of Task {task_config_id} is empty.",
+                f"{task_config._FUNCTION} field of TaskConfig `{task_config_id}` is empty.",
             )
         else:
             if not callable(task_config.function):
                 self._error(
                     task_config._FUNCTION,
                     task_config.function,
-                    f"{task_config._FUNCTION} field of task {task_config_id} must be populated with Callable value.",
+                    f"{task_config._FUNCTION} field of TaskConfig `{task_config_id}` must be"
+                    f" populated with Callable value.",
                 )
```

### Comparing `taipy-core-2.2.3/src/taipy/core/config/config.schema.json` & `taipy-core-2.3.0.dev0/src/taipy/core/config/config.schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999603174603174%*

 * *Differences: {"'properties'": "{'DATA_NODE': {'additionalProperties': {'properties': {'read_fct_args': "*

 * *                 "OrderedDict([('description', 'storage_type: generic specific.'), ('type', "*

 * *                 "'array')]), 'write_fct_args': OrderedDict([('description', 'storage_type: "*

 * *                 "generic specific.'), ('type', 'array')]), delete: ['read_fct_params', "*

 * *                 "'write_fct_params']}}}}"}*

```diff
@@ -172,15 +172,15 @@
                         }
                     },
                     "read_fct": {
                         "description": "storage_type: generic specific.",
                         "taipy_function": true,
                         "type": "string"
                     },
-                    "read_fct_params": {
+                    "read_fct_args": {
                         "description": "storage_type: generic specific.",
                         "type": "array"
                     },
                     "read_kwargs": {
                         "description": "storage_type: parquet specific. Additional parameters when reading parquet files, default is an empty dictionary",
                         "type": "object"
                     },
@@ -232,15 +232,15 @@
                         ]
                     },
                     "write_fct": {
                         "description": "storage_type: generic specific.",
                         "taipy_function": true,
                         "type": "string"
                     },
-                    "write_fct_params": {
+                    "write_fct_args": {
                         "description": "storage_type: generic specific.",
                         "type": "array"
                     },
                     "write_kwargs": {
                         "description": "storage_type: parquet specific.Additional parameters when writing parquet files, default is an empty dictionary",
                         "type": "object"
                     },
```

### Comparing `taipy-core-2.2.3/src/taipy/core/config/data_node_config.py` & `taipy-core-2.3.0.dev0/src/taipy/core/config/data_node_config.py`

 * *Files 27% similar despite different names*

```diff
@@ -22,29 +22,29 @@
 
 from ..common._warnings import _warn_deprecated
 from ..common.default_custom_document import DefaultCustomDocument
 
 
 class DataNodeConfig(Section):
     """
-    Configuration fields needed to instantiate an actual `DataNode^` from the DataNodeConfig.
+    Configuration fields needed to instantiate a `DataNode^`.
 
     A Data Node config is made to be used as a generator for actual data nodes. It holds configuration information
     needed to create an actual data node.
 
     Attributes:
         id (str): Unique identifier of the data node config. It must be a valid Python variable name.
         storage_type (str): Storage type of the data nodes created from the data node config. The possible values
             are : "csv", "excel", "pickle", "sql_table", "sql", "mongo_collection", "generic", "json", "parquet" and
             "in_memory".
             The default value is "pickle".
             Note that the "in_memory" value can only be used when `JobConfig^`.mode is "standalone".
-        scope (Scope^):  The `Scope^` of the data nodes instantiated from the data node config. The default value is
-            SCENARIO.
-        **properties (dict[str, Any]): A dictionary of additional properties.
+        scope (Optional[Scope^]): The optional `Scope^` of the data nodes instantiated from the data node config.
+            The default value is SCENARIO.
+        **properties (dict[str, any]): A dictionary of additional properties.
     """
 
     name = "DATA_NODE"
 
     _STORAGE_TYPE_KEY = "storage_type"
     _STORAGE_TYPE_VALUE_PICKLE = "pickle"
     _STORAGE_TYPE_VALUE_SQL_TABLE = "sql_table"
@@ -78,134 +78,168 @@
 
     _ALL_EXPOSED_TYPES = [
         _EXPOSED_TYPE_PANDAS,
         _EXPOSED_TYPE_MODIN,
         _EXPOSED_TYPE_NUMPY,
     ]
     # Generic
-    _REQUIRED_READ_FUNCTION_GENERIC_PROPERTY = "read_fct"
-    _OPTIONAL_READ_FUNCTION_PARAMS_GENERIC_PROPERTY = "read_fct_params"
-    _REQUIRED_WRITE_FUNCTION_GENERIC_PROPERTY = "write_fct"
-    _OPTIONAL_WRITE_FUNCTION_PARAMS_GENERIC_PROPERTY = "write_fct_params"
+    _OPTIONAL_READ_FUNCTION_GENERIC_PROPERTY = "read_fct"
+    _OPTIONAL_READ_FUNCTION_ARGS_GENERIC_PROPERTY = "read_fct_args"
+    _OPTIONAL_WRITE_FUNCTION_GENERIC_PROPERTY = "write_fct"
+    _OPTIONAL_WRITE_FUNCTION_ARGS_GENERIC_PROPERTY = "write_fct_args"
     # CSV
     _OPTIONAL_EXPOSED_TYPE_CSV_PROPERTY = "exposed_type"
     _OPTIONAL_DEFAULT_PATH_CSV_PROPERTY = "default_path"
     _OPTIONAL_HAS_HEADER_CSV_PROPERTY = "has_header"
     # Excel
     _OPTIONAL_EXPOSED_TYPE_EXCEL_PROPERTY = "exposed_type"
     _OPTIONAL_DEFAULT_PATH_EXCEL_PROPERTY = "default_path"
     _OPTIONAL_HAS_HEADER_EXCEL_PROPERTY = "has_header"
     _OPTIONAL_SHEET_NAME_EXCEL_PROPERTY = "sheet_name"
     # In memory
     _OPTIONAL_DEFAULT_DATA_IN_MEMORY_PROPERTY = "default_data"
     # SQL
-    _OPTIONAL_EXPOSED_TYPE_SQL_PROPERTY = "exposed_type"
-    _REQUIRED_DB_USERNAME_SQL_PROPERTY = "db_username"
-    _REQUIRED_DB_PASSWORD_SQL_PROPERTY = "db_password"
     _REQUIRED_DB_NAME_SQL_PROPERTY = "db_name"
     _REQUIRED_DB_ENGINE_SQL_PROPERTY = "db_engine"
-    _REQUIRED_DB_ENGINE_SQLITE = "sqlite"
-    _REQUIRED_DB_ENGINE_MSSQL = "mssql"
+    _DB_ENGINE_SQLITE = "sqlite"
+    _OPTIONAL_FOLDER_PATH_SQLITE_PROPERTY = "sqlite_folder_path"
+    _OPTIONAL_FILE_EXTENSION_SQLITE_PROPERTY = "sqlite_file_extension"
+    _OPTIONAL_DB_PASSWORD_SQL_PROPERTY = "db_password"
+    _OPTIONAL_DB_USERNAME_SQL_PROPERTY = "db_username"
+    _OPTIONAL_PORT_SQL_PROPERTY = "db_port"
+    _OPTIONAL_HOST_SQL_PROPERTY = "db_host"
+    _OPTIONAL_DRIVER_SQL_PROPERTY = "db_driver"
     _OPTIONAL_DB_EXTRA_ARGS_SQL_PROPERTY = "db_extra_args"
+    _OPTIONAL_EXPOSED_TYPE_SQL_PROPERTY = "exposed_type"
     # SQL_TABLE
-    _REQUIRED_TABLE_NAME_PROPERTY = "table_name"
+    _REQUIRED_TABLE_NAME_SQL_TABLE_PROPERTY = "table_name"
     # SQL
     _REQUIRED_READ_QUERY_SQL_PROPERTY = "read_query"
     _REQUIRED_WRITE_QUERY_BUILDER_SQL_PROPERTY = "write_query_builder"
     # MONGO
     _REQUIRED_DB_NAME_MONGO_PROPERTY = "db_name"
     _REQUIRED_COLLECTION_NAME_MONGO_PROPERTY = "collection_name"
     _OPTIONAL_CUSTOM_DOCUMENT_MONGO_PROPERTY = "custom_document"
-    _OPTIONAL_DB_USERNAME_MONGO_PROPERTY = "db_username"
-    _OPTIONAL_DB_PASSWORD_MONGO_PROPERTY = "db_password"
+    _OPTIONAL_USERNAME_MONGO_PROPERTY = "db_username"
+    _OPTIONAL_PASSWORD_MONGO_PROPERTY = "db_password"
+    _OPTIONAL_HOST_MONGO_PROPERTY = "db_host"
+    _OPTIONAL_PORT_MONGO_PROPERTY = "db_port"
     _OPTIONAL_DB_EXTRA_ARGS_MONGO_PROPERTY = "db_extra_args"
     # Pickle
     _OPTIONAL_DEFAULT_PATH_PICKLE_PROPERTY = "default_path"
     _OPTIONAL_DEFAULT_DATA_PICKLE_PROPERTY = "default_data"
     # JSON
     _OPTIONAL_ENCODER_JSON_PROPERTY = "encoder"
-    _OPTIONAL_DECODER_TYPE_JSON_PROPERTY = "decoder"
-    _REQUIRED_DEFAULT_PATH_JSON_PROPERTY = "default_path"
+    _OPTIONAL_DECODER_JSON_PROPERTY = "decoder"
+    _OPTIONAL_DEFAULT_PATH_JSON_PROPERTY = "default_path"
     # Parquet
     _OPTIONAL_EXPOSED_TYPE_PARQUET_PROPERTY = "exposed_type"
     _OPTIONAL_DEFAULT_PATH_PARQUET_PROPERTY = "default_path"
-    _OPTIONAL_COLUMNS_PARQUET_PROPERTY = "columns"
+    _OPTIONAL_ENGINE_PARQUET_PROPERTY = "engine"
     _OPTIONAL_COMPRESSION_PARQUET_PROPERTY = "compression"
+    _OPTIONAL_READ_KWARGS_PARQUET_PROPERTY = "read_kwargs"
+    _OPTIONAL_WRITE_KWARGS_PARQUET_PROPERTY = "write_kwargs"
 
     _REQUIRED_PROPERTIES: Dict[str, List] = {
         _STORAGE_TYPE_VALUE_PICKLE: [],
         _STORAGE_TYPE_VALUE_SQL_TABLE: [
-            _REQUIRED_DB_USERNAME_SQL_PROPERTY,
-            _REQUIRED_DB_PASSWORD_SQL_PROPERTY,
             _REQUIRED_DB_NAME_SQL_PROPERTY,
             _REQUIRED_DB_ENGINE_SQL_PROPERTY,
-            _REQUIRED_TABLE_NAME_PROPERTY,
+            _REQUIRED_TABLE_NAME_SQL_TABLE_PROPERTY,
         ],
         _STORAGE_TYPE_VALUE_SQL: [
-            _REQUIRED_DB_USERNAME_SQL_PROPERTY,
-            _REQUIRED_DB_PASSWORD_SQL_PROPERTY,
             _REQUIRED_DB_NAME_SQL_PROPERTY,
             _REQUIRED_DB_ENGINE_SQL_PROPERTY,
             _REQUIRED_READ_QUERY_SQL_PROPERTY,
             _REQUIRED_WRITE_QUERY_BUILDER_SQL_PROPERTY,
         ],
         _STORAGE_TYPE_VALUE_MONGO_COLLECTION: [
             _REQUIRED_DB_NAME_MONGO_PROPERTY,
             _REQUIRED_COLLECTION_NAME_MONGO_PROPERTY,
         ],
         _STORAGE_TYPE_VALUE_CSV: [],
         _STORAGE_TYPE_VALUE_EXCEL: [],
         _STORAGE_TYPE_VALUE_IN_MEMORY: [],
-        _STORAGE_TYPE_VALUE_GENERIC: [
-            _REQUIRED_READ_FUNCTION_GENERIC_PROPERTY,
-            _REQUIRED_WRITE_FUNCTION_GENERIC_PROPERTY,
-        ],
-        _STORAGE_TYPE_VALUE_JSON: [_REQUIRED_DEFAULT_PATH_JSON_PROPERTY],
+        _STORAGE_TYPE_VALUE_GENERIC: [],
+        _STORAGE_TYPE_VALUE_JSON: [],
         _STORAGE_TYPE_VALUE_PARQUET: [],
     }
 
     _OPTIONAL_PROPERTIES = {
-        _STORAGE_TYPE_VALUE_GENERIC: [
-            _OPTIONAL_READ_FUNCTION_PARAMS_GENERIC_PROPERTY,
-            _OPTIONAL_WRITE_FUNCTION_PARAMS_GENERIC_PROPERTY,
-        ],
-        _STORAGE_TYPE_VALUE_CSV: [
-            _OPTIONAL_EXPOSED_TYPE_CSV_PROPERTY,
-            _OPTIONAL_DEFAULT_PATH_CSV_PROPERTY,
-            _OPTIONAL_HAS_HEADER_CSV_PROPERTY,
-        ],
-        _STORAGE_TYPE_VALUE_EXCEL: [
-            _OPTIONAL_EXPOSED_TYPE_EXCEL_PROPERTY,
-            _OPTIONAL_DEFAULT_PATH_EXCEL_PROPERTY,
-            _OPTIONAL_HAS_HEADER_EXCEL_PROPERTY,
-            _OPTIONAL_SHEET_NAME_EXCEL_PROPERTY,
-        ],
-        _STORAGE_TYPE_VALUE_IN_MEMORY: [_OPTIONAL_DEFAULT_DATA_IN_MEMORY_PROPERTY],
-        _STORAGE_TYPE_VALUE_SQL_TABLE: [_OPTIONAL_EXPOSED_TYPE_SQL_PROPERTY, _OPTIONAL_DB_EXTRA_ARGS_SQL_PROPERTY],
-        _STORAGE_TYPE_VALUE_SQL: [_OPTIONAL_EXPOSED_TYPE_SQL_PROPERTY, _OPTIONAL_DB_EXTRA_ARGS_SQL_PROPERTY],
-        _STORAGE_TYPE_VALUE_MONGO_COLLECTION: [
-            _OPTIONAL_CUSTOM_DOCUMENT_MONGO_PROPERTY,
-            _OPTIONAL_DB_USERNAME_MONGO_PROPERTY,
-            _OPTIONAL_DB_PASSWORD_MONGO_PROPERTY,
-            _OPTIONAL_DB_EXTRA_ARGS_MONGO_PROPERTY,
-        ],
-        _STORAGE_TYPE_VALUE_PICKLE: [_OPTIONAL_DEFAULT_PATH_PICKLE_PROPERTY, _OPTIONAL_DEFAULT_DATA_PICKLE_PROPERTY],
-        _STORAGE_TYPE_VALUE_JSON: [_OPTIONAL_ENCODER_JSON_PROPERTY, _OPTIONAL_DECODER_TYPE_JSON_PROPERTY],
-        _STORAGE_TYPE_VALUE_PARQUET: [
-            _OPTIONAL_EXPOSED_TYPE_PARQUET_PROPERTY,
-            _OPTIONAL_DEFAULT_PATH_PARQUET_PROPERTY,
-            _OPTIONAL_COLUMNS_PARQUET_PROPERTY,
-            _OPTIONAL_COMPRESSION_PARQUET_PROPERTY,
-        ],
+        _STORAGE_TYPE_VALUE_GENERIC: {
+            _OPTIONAL_READ_FUNCTION_GENERIC_PROPERTY: None,
+            _OPTIONAL_WRITE_FUNCTION_GENERIC_PROPERTY: None,
+            _OPTIONAL_READ_FUNCTION_ARGS_GENERIC_PROPERTY: None,
+            _OPTIONAL_WRITE_FUNCTION_ARGS_GENERIC_PROPERTY: None,
+        },
+        _STORAGE_TYPE_VALUE_CSV: {
+            _OPTIONAL_DEFAULT_PATH_CSV_PROPERTY: None,
+            _OPTIONAL_HAS_HEADER_CSV_PROPERTY: True,
+            _OPTIONAL_EXPOSED_TYPE_CSV_PROPERTY: _DEFAULT_EXPOSED_TYPE,
+        },
+        _STORAGE_TYPE_VALUE_EXCEL: {
+            _OPTIONAL_DEFAULT_PATH_EXCEL_PROPERTY: None,
+            _OPTIONAL_HAS_HEADER_EXCEL_PROPERTY: True,
+            _OPTIONAL_SHEET_NAME_EXCEL_PROPERTY: None,
+            _OPTIONAL_EXPOSED_TYPE_EXCEL_PROPERTY: _DEFAULT_EXPOSED_TYPE,
+        },
+        _STORAGE_TYPE_VALUE_IN_MEMORY: {_OPTIONAL_DEFAULT_DATA_IN_MEMORY_PROPERTY: None},
+        _STORAGE_TYPE_VALUE_SQL_TABLE: {
+            _OPTIONAL_DB_USERNAME_SQL_PROPERTY: None,
+            _OPTIONAL_DB_PASSWORD_SQL_PROPERTY: None,
+            _OPTIONAL_HOST_SQL_PROPERTY: "localhost",
+            _OPTIONAL_PORT_SQL_PROPERTY: 1433,
+            _OPTIONAL_DRIVER_SQL_PROPERTY: "",
+            _OPTIONAL_FOLDER_PATH_SQLITE_PROPERTY: None,
+            _OPTIONAL_FILE_EXTENSION_SQLITE_PROPERTY: ".db",
+            _OPTIONAL_DB_EXTRA_ARGS_SQL_PROPERTY: None,
+            _OPTIONAL_EXPOSED_TYPE_SQL_PROPERTY: _DEFAULT_EXPOSED_TYPE,
+        },
+        _STORAGE_TYPE_VALUE_SQL: {
+            _OPTIONAL_DB_USERNAME_SQL_PROPERTY: None,
+            _OPTIONAL_DB_PASSWORD_SQL_PROPERTY: None,
+            _OPTIONAL_HOST_SQL_PROPERTY: "localhost",
+            _OPTIONAL_PORT_SQL_PROPERTY: 1433,
+            _OPTIONAL_DRIVER_SQL_PROPERTY: "",
+            _OPTIONAL_FOLDER_PATH_SQLITE_PROPERTY: None,
+            _OPTIONAL_FILE_EXTENSION_SQLITE_PROPERTY: ".db",
+            _OPTIONAL_DB_EXTRA_ARGS_SQL_PROPERTY: None,
+            _OPTIONAL_EXPOSED_TYPE_SQL_PROPERTY: _DEFAULT_EXPOSED_TYPE,
+        },
+        _STORAGE_TYPE_VALUE_MONGO_COLLECTION: {
+            _OPTIONAL_CUSTOM_DOCUMENT_MONGO_PROPERTY: DefaultCustomDocument,
+            _OPTIONAL_USERNAME_MONGO_PROPERTY: "",
+            _OPTIONAL_PASSWORD_MONGO_PROPERTY: "",
+            _OPTIONAL_HOST_MONGO_PROPERTY: "localhost",
+            _OPTIONAL_PORT_MONGO_PROPERTY: 27017,
+            _OPTIONAL_DB_EXTRA_ARGS_MONGO_PROPERTY: None,
+        },
+        _STORAGE_TYPE_VALUE_PICKLE: {
+            _OPTIONAL_DEFAULT_PATH_PICKLE_PROPERTY: None,
+            _OPTIONAL_DEFAULT_DATA_PICKLE_PROPERTY: None,
+        },
+        _STORAGE_TYPE_VALUE_JSON: {
+            _OPTIONAL_DEFAULT_PATH_PICKLE_PROPERTY: None,
+            _OPTIONAL_ENCODER_JSON_PROPERTY: None,
+            _OPTIONAL_DECODER_JSON_PROPERTY: None,
+        },
+        _STORAGE_TYPE_VALUE_PARQUET: {
+            _OPTIONAL_DEFAULT_PATH_PARQUET_PROPERTY: None,
+            _OPTIONAL_ENGINE_PARQUET_PROPERTY: "pyarrow",
+            _OPTIONAL_COMPRESSION_PARQUET_PROPERTY: "snappy",
+            _OPTIONAL_READ_KWARGS_PARQUET_PROPERTY: None,
+            _OPTIONAL_WRITE_KWARGS_PARQUET_PROPERTY: None,
+            _OPTIONAL_EXPOSED_TYPE_PARQUET_PROPERTY: _DEFAULT_EXPOSED_TYPE,
+        },
     }
 
     _SCOPE_KEY = "scope"
     _DEFAULT_SCOPE = Scope.SCENARIO
 
-    def __init__(self, id: str, storage_type: str = None, scope: Scope = None, **properties):
+    def __init__(self, id: str, storage_type: Optional[str] = None, scope: Scope = None, **properties):
         self._storage_type = storage_type
         self._scope = scope
         super().__init__(id, **properties)
 
     def __copy__(self):
         return DataNodeConfig(self.id, self._storage_type, self._scope, **copy(self._properties))
 
@@ -265,494 +299,574 @@
         scope = as_dict.pop(cls._SCOPE_KEY, None)
         return DataNodeConfig(id=id, storage_type=storage_type, scope=scope, **as_dict)
 
     def _update(self, as_dict, default_section=None):
         self._storage_type = as_dict.pop(self._STORAGE_TYPE_KEY, self._storage_type)
         if self._storage_type is None and default_section:
             self._storage_type = default_section.storage_type
+
         self._scope = as_dict.pop(self._SCOPE_KEY, self._scope)
         if self._scope is None and default_section:
-            self._scope = default_section.scope
+            if default_section.scope and self._storage_type == default_section.storage_type:
+                self._scope = default_section.scope
+            else:
+                self._scope = self._DEFAULT_SCOPE
+
         self._properties.update(as_dict)
-        if default_section:
+        if default_section and self._storage_type == default_section.storage_type:
             self._properties = {**default_section.properties, **self._properties}
 
+        # Assign default value to optional properties if not defined by user
+        if self._OPTIONAL_PROPERTIES.get(self._storage_type):
+            for optional_property, default_value in self._OPTIONAL_PROPERTIES[self._storage_type].items():
+                if default_value is not None and self._properties.get(optional_property) is None:
+                    self._properties[optional_property] = default_value
+
     @staticmethod
-    def _configure_default(storage_type: str, scope: Scope = _DEFAULT_SCOPE, **properties):
+    def _configure_default(storage_type: str, scope: Optional[Scope] = None, **properties) -> "DataNodeConfig":
         """Configure the default values for data node configurations.
+
         This function creates the _default data node configuration_ object,
         where all data node configuration objects will find their default
         values when needed.
+
         Parameters:
             storage_type (str): The default storage type for all data node configurations.
-                The possible values are _"pickle"_ (the default value), _"csv"_, _"excel"_,
-                _"sql"_, _"mongo_collection"_, _"in_memory"_, _"json"_, _"parquet"_ or _"generic"_.
-            scope (Scope^): The default scope for all data node configurations.
+                The possible values are *"pickle"* (the default value), *"csv"*, *"excel"*,
+                *"sql"*, *"mongo_collection"*, *"in_memory"*, *"json"*, *"parquet"* or
+                *"generic"*.
+            scope (Optional[Scope^]): The default scope for all data node configurations.<br/>
                 The default value is `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
         Returns:
-            `DataNodeConfig^`: The default data node configuration.
+            The default data node configuration.
         """
         section = DataNodeConfig(_Config.DEFAULT_KEY, storage_type, scope, **properties)
-        Config._register(section)
+        Config._register_default(section)
         return Config.sections[DataNodeConfig.name][_Config.DEFAULT_KEY]
 
-    @staticmethod
+    @classmethod
     def _configure(
-        id: str,
-        storage_type: Optional[str] = None,
-        scope: Scope = _DEFAULT_SCOPE,
-        **properties,
-    ):
+        cls, id: str, storage_type: Optional[str] = None, scope: Optional[Scope] = None, **properties
+    ) -> "DataNodeConfig":
         """Configure a new data node configuration.
+
         Parameters:
             id (str): The unique identifier of the new data node configuration.
             storage_type (Optional[str]): The data node configuration storage type. The possible values
-                are _None_ (which is the default value of _"pickle"_, unless it has been overloaded by the
-                _storage_type_ value set in the default data node configuration
-                (see `(Config.)configure_default_data_node()^`)), _"pickle"_, _"csv"_, _"excel"_, _"sql_table"_,
-                _"sql"_, _"json"_, _"parquet"_, _"mongo_collection"_, _"in_memory"_, or _"generic"_.
-            scope (Scope^): The scope of the data node configuration. The default value is
-                `Scope.SCENARIO` (or the one specified in
+                are None (which is the default value of *"pickle"*, unless it has been overloaded by the
+                *storage_type* value set in the default data node configuration
+                (see `(Config.)configure_default_data_node()^`)), *"pickle"*, *"csv"*, *"excel"*,
+                *"sql_table"*, *"sql"*, *"json"*, *"parquet"*, *"mongo_collection"*, *"in_memory"*, or
+                *"generic"*.
+            scope (Optional[Scope^]): The scope of the data node configuration.<br/>
+                The default value is `Scope.SCENARIO` (or the one specified in
                 `(Config.)configure_default_data_node()^`).
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
         Returns:
-            `DataNodeConfig^`: The new data node configuration.
+            The new data node configuration.
         """
-        section = DataNodeConfig(id, storage_type, scope, **properties)
-        Config._register(section)
-        return Config.sections[DataNodeConfig.name][id]
+        configuration_map: Dict[str, Callable] = {
+            cls._STORAGE_TYPE_VALUE_PICKLE: cls._configure_pickle,
+            cls._STORAGE_TYPE_VALUE_SQL_TABLE: cls._configure_sql_table,
+            cls._STORAGE_TYPE_VALUE_SQL: cls._configure_sql,
+            cls._STORAGE_TYPE_VALUE_MONGO_COLLECTION: cls._configure_mongo_collection,
+            cls._STORAGE_TYPE_VALUE_CSV: cls._configure_csv,
+            cls._STORAGE_TYPE_VALUE_EXCEL: cls._configure_excel,
+            cls._STORAGE_TYPE_VALUE_IN_MEMORY: cls._configure_in_memory,
+            cls._STORAGE_TYPE_VALUE_GENERIC: cls._configure_generic,
+            cls._STORAGE_TYPE_VALUE_JSON: cls._configure_json,
+            cls._STORAGE_TYPE_VALUE_PARQUET: cls._configure_parquet,
+        }
 
-    @staticmethod
+        if storage_type in cls._ALL_STORAGE_TYPES:
+            return configuration_map[storage_type](id=id, scope=scope, **properties)
+
+        return cls.__configure(id, storage_type, scope, **properties)
+
+    @classmethod
     def _configure_csv(
+        cls,
         id: str,
-        default_path: str = None,
-        has_header: bool = True,
-        exposed_type=_DEFAULT_EXPOSED_TYPE,
-        scope=_DEFAULT_SCOPE,
+        default_path: Optional[str] = None,
+        has_header: Optional[bool] = None,
+        exposed_type: Optional[str] = None,
+        scope: Optional[Scope] = None,
         **properties,
-    ):
+    ) -> "DataNodeConfig":
         """Configure a new CSV data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new CSV data node configuration.
-            default_path (str): The default path of the CSV file.
-            has_header (bool): If True, indicates that the CSV file has a header.
-            exposed_type: The exposed type of the data read from CSV file. The default value is `pandas`.
-            scope (Scope^): The scope of the CSV data node configuration. The default value
-                is `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
-        Returns:
-            `DataNodeConfig^`: The new CSV data node configuration.
-        """
-        section = DataNodeConfig(
-            id,
-            DataNodeConfig._STORAGE_TYPE_VALUE_CSV,
-            scope=scope,
-            default_path=default_path,
-            has_header=has_header,
-            exposed_type=exposed_type,
-            **properties,
-        )
-        Config._register(section)
-        return Config.sections[DataNodeConfig.name][id]
+            default_path (Optional[str]): The default path of the CSV file.
+            has_header (Optional[bool]): If True, indicates that the CSV file has a header.
+            exposed_type (Optional[str]): The exposed type of the data read from CSV file.<br/>
+                The default value is `pandas`.
+            scope (Optional[Scope^]): The scope of the CSV data node configuration.<br/>
+                The default value is `Scope.SCENARIO`.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
-    @staticmethod
+        Returns:
+            The new CSV data node configuration.
+        """
+        if default_path is not None:
+            properties[cls._OPTIONAL_DEFAULT_PATH_CSV_PROPERTY] = default_path
+        if has_header is not None:
+            properties[cls._OPTIONAL_HAS_HEADER_CSV_PROPERTY] = has_header
+        if exposed_type is not None:
+            properties[cls._OPTIONAL_EXPOSED_TYPE_CSV_PROPERTY] = exposed_type
+
+        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_CSV, scope, **properties)
+
+    @classmethod
     def _configure_json(
+        cls,
         id: str,
-        default_path: str = None,
-        encoder: json.JSONEncoder = None,
-        decoder: json.JSONDecoder = None,
-        scope=_DEFAULT_SCOPE,
+        default_path: Optional[str] = None,
+        encoder: Optional[json.JSONEncoder] = None,
+        decoder: Optional[json.JSONDecoder] = None,
+        scope: Optional[Scope] = None,
         **properties,
-    ):
+    ) -> "DataNodeConfig":
         """Configure a new JSON data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new JSON data node configuration.
-            default_path (str): The default path of the JSON file.
-            encoder (json.JSONEncoder): The JSON encoder used to write data into the JSON file.
-            decoder (json.JSONDecoder): The JSON decoder used to read data from the JSON file.
-            scope (Scope^): The scope of the JSON data node configuration. The default value
-                is `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
-        Returns:
-            `DataNodeConfig^`: The new JSON data node configuration.
-        """
-        section = DataNodeConfig(
-            id,
-            DataNodeConfig._STORAGE_TYPE_VALUE_JSON,
-            scope=scope,
-            default_path=default_path,
-            encoder=encoder,
-            decoder=decoder,
-            **properties,
-        )
-        Config._register(section)
-        return Config.sections[DataNodeConfig.name][id]
+            default_path (Optional[str]): The default path of the JSON file.
+            encoder (Optional[json.JSONEncoder]): The JSON encoder used to write data into the JSON file.
+            decoder (Optional[json.JSONDecoder]): The JSON decoder used to read data from the JSON file.
+            scope (Optional[Scope^]): The scope of the JSON data node configuration.<br/>
+                The default value is `Scope.SCENARIO`.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+        Returns:
+            The new JSON data node configuration.
+        """
+        if default_path is not None:
+            properties[cls._OPTIONAL_DEFAULT_PATH_JSON_PROPERTY] = default_path
+        if encoder is not None:
+            properties[cls._OPTIONAL_ENCODER_JSON_PROPERTY] = encoder
+        if decoder is not None:
+            properties[cls._OPTIONAL_DECODER_JSON_PROPERTY] = decoder
 
-    @staticmethod
+        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_JSON, scope, **properties)
+
+    @classmethod
     def _configure_parquet(
+        cls,
         id: str,
-        default_path: str = None,
-        exposed_type=_DEFAULT_EXPOSED_TYPE,
-        engine: Optional[str] = "pyarrow",
-        compression: Optional[str] = "snappy",
-        read_kwargs: Dict = dict(),
-        write_kwargs: Dict = dict(),
-        scope=_DEFAULT_SCOPE,
+        default_path: Optional[str] = None,
+        engine: Optional[str] = None,
+        compression: Optional[str] = None,
+        read_kwargs: Optional[Dict] = None,
+        write_kwargs: Optional[Dict] = None,
+        exposed_type: Optional[str] = None,
+        scope: Optional[Scope] = None,
         **properties,
-    ):
+    ) -> "DataNodeConfig":
         """Configure a new Parquet data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new Parquet data node configuration.
-            default_path (str): The default path of the Parquet file.
-            exposed_type: The exposed type of the data read from Parquet file. The default value is `pandas`.
-            engine (Optional[str]): Parquet library to use. Possible values are _"fastparquet"_ or _"pyarrow"_.
-                The default value is _"pyarrow"_.
-            compression (Optional[str]): Name of the compression to use. Use None for no compression.
-                `{'snappy', 'gzip', 'brotli', None}`, default `'snappy'`.
-            read_kwargs (Optional[Dict]): Additional parameters passed to the `pandas.read_parquet` method.
-            write_kwargs (Optional[Dict]): Additional parameters passed to the `pandas.DataFrame.write_parquet` method.
-                The parameters in "read_kwargs" and "write_kwargs" have a **higher precedence** than the top-level
-                parameters which are also passed to Pandas.
-            scope (Scope^): The scope of the Parquet data node configuration. The default value
-                is `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
-        Returns:
-            `DataNodeConfig^`: The new Parquet data node configuration.
-        """
-        section = DataNodeConfig(
-            id,
-            DataNodeConfig._STORAGE_TYPE_VALUE_PARQUET,
-            scope=scope,
-            default_path=default_path,
-            engine=engine,
-            compression=compression,
-            read_kwargs=read_kwargs,
-            write_kwargs=write_kwargs,
-            exposed_type=exposed_type,
-            **properties,
-        )
-        Config._register(section)
-        return Config.sections[DataNodeConfig.name][id]
+            default_path (Optional[str]): The default path of the Parquet file.
+            engine (Optional[str]): Parquet library to use. Possible values are *"fastparquet"* or
+                *"pyarrow"*.<br/>
+                The default value is *"pyarrow"*.
+            compression (Optional[str]): Name of the compression to use. Possible values are *"snappy"*,
+                *"gzip"*, *"brotli"*, or *"none"* (no compression). The default value is *"snappy"*.
+            read_kwargs (Optional[dict]): Additional parameters passed to the `pandas.read_parquet()`
+                function.
+            write_kwargs (Optional[dict]): Additional parameters passed to the
+                `pandas.DataFrame.write_parquet()` function.<br/>
+                The parameters in *read_kwargs* and *write_kwargs* have a **higher precedence** than the
+                top-level parameters which are also passed to Pandas.
+            exposed_type (Optional[str]): The exposed type of the data read from Parquet file.<br/>
+                The default value is `pandas`.
+            scope (Optional[Scope^]): The scope of the Parquet data node configuration.<br/>
+                The default value is `Scope.SCENARIO`.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
-    @staticmethod
+        Returns:
+            The new Parquet data node configuration.
+        """
+        if default_path is not None:
+            properties[cls._OPTIONAL_DEFAULT_PATH_PARQUET_PROPERTY] = default_path
+        if engine is not None:
+            properties[cls._OPTIONAL_ENGINE_PARQUET_PROPERTY] = engine
+        if compression is not None:
+            properties[cls._OPTIONAL_COMPRESSION_PARQUET_PROPERTY] = compression
+        if read_kwargs is not None:
+            properties[cls._OPTIONAL_READ_KWARGS_PARQUET_PROPERTY] = read_kwargs
+        if write_kwargs is not None:
+            properties[cls._OPTIONAL_WRITE_KWARGS_PARQUET_PROPERTY] = write_kwargs
+        if exposed_type is not None:
+            properties[cls._OPTIONAL_EXPOSED_TYPE_PARQUET_PROPERTY] = exposed_type
+
+        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_PARQUET, scope, **properties)
+
+    @classmethod
     def _configure_excel(
+        cls,
         id: str,
-        default_path: str = None,
-        has_header: bool = True,
-        sheet_name: Union[List[str], str] = None,
-        exposed_type=_DEFAULT_EXPOSED_TYPE,
-        scope: Scope = _DEFAULT_SCOPE,
+        default_path: Optional[str] = None,
+        has_header: Optional[bool] = None,
+        sheet_name: Optional[Union[List[str], str]] = None,
+        exposed_type: Optional[str] = None,
+        scope: Optional[Scope] = None,
         **properties,
-    ):
+    ) -> "DataNodeConfig":
         """Configure a new Excel data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new Excel data node configuration.
-            default_path (str): The path of the Excel file.
-            has_header (bool): If True, indicates that the Excel file has a header.
-            sheet_name (Union[List[str], str]): The list of sheet names to be used. This
-                can be a unique name.
-            exposed_type: The exposed type of the data read from Excel file. The default value is `pandas`.
-            scope (Scope^): The scope of the Excel data node configuration. The default
-                value is `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
-        Returns:
-            `DataNodeConfig^`: The new CSV data node configuration.
-        """
-        section = DataNodeConfig(
-            id,
-            DataNodeConfig._STORAGE_TYPE_VALUE_EXCEL,
-            scope=scope,
-            default_path=default_path,
-            has_header=has_header,
-            sheet_name=sheet_name,
-            exposed_type=exposed_type,
-            **properties,
-        )
-        Config._register(section)
-        return Config.sections[DataNodeConfig.name][id]
+            default_path (Optional[str]): The path of the Excel file.
+            has_header (Optional[bool]): If True, indicates that the Excel file has a header.
+            sheet_name (Optional[Union[List[str], str]]): The list of sheet names to be used.
+                This can be a unique name.
+            exposed_type (Optional[str]): The exposed type of the data read from Excel file.<br/>
+                The default value is `pandas`.
+            scope (Optional[Scope^]): The scope of the Excel data node configuration.<br/>
+                The default value is `Scope.SCENARIO`.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
-    @staticmethod
+        Returns:
+            The new Excel data node configuration.
+        """
+        if default_path is not None:
+            properties[cls._OPTIONAL_DEFAULT_PATH_EXCEL_PROPERTY] = default_path
+        if has_header is not None:
+            properties[cls._OPTIONAL_HAS_HEADER_EXCEL_PROPERTY] = has_header
+        if sheet_name is not None:
+            properties[cls._OPTIONAL_SHEET_NAME_EXCEL_PROPERTY] = sheet_name
+        if exposed_type is not None:
+            properties[cls._OPTIONAL_EXPOSED_TYPE_EXCEL_PROPERTY] = exposed_type
+
+        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_EXCEL, scope, **properties)
+
+    @classmethod
     def _configure_generic(
+        cls,
         id: str,
-        read_fct: Callable = None,
-        write_fct: Callable = None,
-        read_fct_params: List = None,
-        write_fct_params: List = None,
-        scope: Scope = _DEFAULT_SCOPE,
+        read_fct: Optional[Callable] = None,
+        write_fct: Optional[Callable] = None,
+        read_fct_args: Optional[List] = None,
+        write_fct_args: Optional[List] = None,
+        scope: Optional[Scope] = None,
         **properties,
-    ):
+    ) -> "DataNodeConfig":
         """Configure a new generic data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new generic data node configuration.
             read_fct (Optional[Callable]): The Python function called to read the data.
             write_fct (Optional[Callable]): The Python function called to write the data.
-                The provided function must have at least one parameter that receives the data
-                to be written.
-            read_fct_params (Optional[List]): The parameters that are passed to _read_fct_
-                to read the data.
-            write_fct_params (Optional[List]): The parameters that are passed to _write_fct_
-                to write the data.
-            scope (Optional[Scope^]): The scope of the Generic data node configuration.
-                The default value is `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
-        Returns:
-            `DataNodeConfig^`: The new Generic data node configuration.
-        """
-        section = DataNodeConfig(
-            id,
-            DataNodeConfig._STORAGE_TYPE_VALUE_GENERIC,
-            scope=scope,
-            read_fct=read_fct,
-            write_fct=write_fct,
-            read_fct_params=read_fct_params,
-            write_fct_params=write_fct_params,
-            **properties,
-        )
-        Config._register(section)
-        return Config.sections[DataNodeConfig.name][id]
+                The provided function must have at least one parameter that receives the data to be written.
+            read_fct_args (Optional[List]): The list of arguments that are passed to the function
+                *read_fct* to read data.
+            write_fct_args (Optional[List]): The list of arguments that are passed to the function
+                *write_fct* to write the data.
+            scope (Optional[Scope^]): The scope of the Generic data node configuration.<br/>
+                The default value is `Scope.SCENARIO`.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+        Returns:
+            The new Generic data node configuration.
+        """
+        if read_fct is not None:
+            properties[cls._OPTIONAL_READ_FUNCTION_GENERIC_PROPERTY] = read_fct
+        if write_fct is not None:
+            properties[cls._OPTIONAL_WRITE_FUNCTION_GENERIC_PROPERTY] = write_fct
+        if read_fct_args is not None:
+            properties[cls._OPTIONAL_READ_FUNCTION_ARGS_GENERIC_PROPERTY] = read_fct_args
+        if write_fct_args is not None:
+            properties[cls._OPTIONAL_WRITE_FUNCTION_ARGS_GENERIC_PROPERTY] = write_fct_args
 
-    @staticmethod
+        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_GENERIC, scope, **properties)
+
+    @classmethod
     def _configure_in_memory(
-        id: str,
-        default_data: Optional[Any] = None,
-        scope: Scope = _DEFAULT_SCOPE,
-        **properties,
-    ):
-        """Configure a new _in_memory_ data node configuration.
+        cls, id: str, default_data: Optional[Any] = None, scope: Optional[Scope] = None, **properties
+    ) -> "DataNodeConfig":
+        """Configure a new *in-memory* data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new in_memory data node configuration.
-            default_data (Optional[Any]): The default data of the data nodes instantiated from
+            default_data (Optional[any]): The default data of the data nodes instantiated from
                 this in_memory data node configuration.
-            scope (Scope^): The scope of the in_memory data node configuration. The default
-                value is `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
-        Returns:
-            `DataNodeConfig^`: The new _in_memory_ data node configuration.
-        """
-        section = DataNodeConfig(
-            id,
-            DataNodeConfig._STORAGE_TYPE_VALUE_IN_MEMORY,
-            scope=scope,
-            default_data=default_data,
-            **properties,
-        )
-        Config._register(section)
-        return Config.sections[DataNodeConfig.name][id]
+            scope (Optional[Scope^]): The scope of the in_memory data node configuration.<br/>
+                The default value is `Scope.SCENARIO`.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
-    @staticmethod
+        Returns:
+            The new *in-memory* data node configuration.
+        """
+        if default_data is not None:
+            properties[cls._OPTIONAL_DEFAULT_DATA_IN_MEMORY_PROPERTY] = default_data
+
+        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_IN_MEMORY, scope, **properties)
+
+    @classmethod
     def _configure_pickle(
+        cls,
         id: str,
+        default_path: Optional[str] = None,
         default_data: Optional[Any] = None,
-        scope: Scope = _DEFAULT_SCOPE,
+        scope: Optional[Scope] = None,
         **properties,
-    ):
+    ) -> "DataNodeConfig":
         """Configure a new pickle data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new pickle data node configuration.
-            default_data (Optional[Any]): The default data of the data nodes instantiated from
+            default_path (Optional[str]): The path of the pickle file.
+            default_data (Optional[any]): The default data of the data nodes instantiated from
                 this pickle data node configuration.
-            scope (Scope^): The scope of the pickle data node configuration. The default value
-                is `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
-        Returns:
-            `DataNodeConfig^`: The new pickle data node configuration.
-        """
-        section = DataNodeConfig(
-            id,
-            DataNodeConfig._STORAGE_TYPE_VALUE_PICKLE,
-            scope=scope,
-            default_data=default_data,
-            **properties,
-        )
-        Config._register(section)
-        return Config.sections[DataNodeConfig.name][id]
+            scope (Optional[Scope^]): The scope of the pickle data node configuration.<br/>
+                The default value is `Scope.SCENARIO`.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
-    @staticmethod
+        Returns:
+            The new pickle data node configuration.
+        """
+        if default_path is not None:
+            properties[cls._OPTIONAL_DEFAULT_PATH_PICKLE_PROPERTY] = default_path
+        if default_data is not None:
+            properties[cls._OPTIONAL_DEFAULT_DATA_PICKLE_PROPERTY] = default_data
+
+        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_PICKLE, scope, **properties)
+
+    @classmethod
     def _configure_sql_table(
+        cls,
         id: str,
-        db_username: str,
-        db_password: str,
         db_name: str,
         db_engine: str,
-        table_name: str = None,
-        db_port: int = 1433,
-        db_host: str = "localhost",
-        db_driver: str = "",
-        db_extra_args: Dict[str, Any] = None,
-        exposed_type=_EXPOSED_TYPE_PANDAS,
-        scope: Scope = _DEFAULT_SCOPE,
+        table_name: str,
+        db_username: Optional[str] = None,
+        db_password: Optional[str] = None,
+        db_host: Optional[str] = None,
+        db_port: Optional[int] = None,
+        db_driver: Optional[str] = None,
+        sqlite_folder_path: Optional[str] = None,
+        sqlite_file_extension: Optional[str] = None,
+        db_extra_args: Optional[Dict[str, Any]] = None,
+        exposed_type: Optional[str] = None,
+        scope: Optional[Scope] = None,
         **properties,
-    ):
+    ) -> "DataNodeConfig":
         """Configure a new SQL table data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new SQL data node configuration.
-            db_username (str): The database username.
-            db_password (str): The database password.
             db_name (str): The database name, or the name of the SQLite database file.
-            db_host (str): The database host. The default value is _"localhost"_.
-            db_engine (str): The database engine. Possible values are _"sqlite"_, _"mssql"_, _"mysql"_, or
-                _"postgresql"_.
-            db_driver (str): The database driver.
-            db_port (int): The database port. The default value is 1433.
-            db_extra_args (Dict[str, Any]): A dictionary of additional arguments to be passed into database
-                connection string.
+            db_engine (str): The database engine. Possible values are *"sqlite"*, *"mssql"*, *"mysql"*,
+                or *"postgresql"*.
             table_name (str): The name of the SQL table.
-            exposed_type: The exposed type of the data read from SQL query. The default value is `pandas`.
-            scope (Scope^): The scope of the SQL data node configuration. The default value is
-                `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
-        Returns:
-            `DataNodeConfig^`: The new SQL data node configuration.
-        """
-        section = DataNodeConfig(
-            id,
-            DataNodeConfig._STORAGE_TYPE_VALUE_SQL_TABLE,
-            scope=scope,
-            db_username=db_username,
-            db_password=db_password,
-            db_name=db_name,
-            db_host=db_host,
-            db_engine=db_engine,
-            db_driver=db_driver,
-            db_port=db_port,
-            db_extra_args=db_extra_args,
-            table_name=table_name,
-            exposed_type=exposed_type,
-            **properties,
+            db_username (Optional[str]): The database username. Required by the *"mssql"*, *"mysql"*, and
+                *"postgresql"* engines.
+            db_password (Optional[str]): The database password. Required by the *"mssql"*, *"mysql"*, and
+                *"postgresql"* engines.
+            db_host (Optional[str]): The database host.<br/>
+                The default value is "localhost".
+            db_port (Optional[int]): The database port.<br/>
+                The default value is 1433.
+            db_driver (Optional[str]): The database driver.
+            sqlite_folder_path (Optional[str]): The path to the folder that contains SQLite file.<br/>
+                The default value is the current working folder.
+            sqlite_file_extension (Optional[str]): The file extension of the SQLite file.<br/>
+                The default value is ".db".
+            db_extra_args (Optional[dict[str, any]]): A dictionary of additional arguments to be passed
+                into database connection string.
+            exposed_type (Optional[str]): The exposed type of the data read from SQL table.<br/>
+                The default value is "pandas".
+            scope (Optional[Scope^]): The scope of the SQL data node configuration.<br/>
+                The default value is `Scope.SCENARIO`.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
+        Returns:
+            The new SQL data node configuration.
+        """
+        properties.update(
+            {
+                cls._REQUIRED_DB_NAME_SQL_PROPERTY: db_name,
+                cls._REQUIRED_DB_ENGINE_SQL_PROPERTY: db_engine,
+                cls._REQUIRED_TABLE_NAME_SQL_TABLE_PROPERTY: table_name,
+            }
         )
-        Config._register(section)
-        return Config.sections[DataNodeConfig.name][id]
 
-    @staticmethod
+        if db_username is not None:
+            properties[cls._OPTIONAL_DB_USERNAME_SQL_PROPERTY] = db_username
+        if db_password is not None:
+            properties[cls._OPTIONAL_DB_PASSWORD_SQL_PROPERTY] = db_password
+        if db_host is not None:
+            properties[cls._OPTIONAL_HOST_SQL_PROPERTY] = db_host
+        if db_port is not None:
+            properties[cls._OPTIONAL_PORT_SQL_PROPERTY] = db_port
+        if db_driver is not None:
+            properties[cls._OPTIONAL_DRIVER_SQL_PROPERTY] = db_driver
+        if sqlite_folder_path is not None:
+            properties[cls._OPTIONAL_FOLDER_PATH_SQLITE_PROPERTY] = sqlite_folder_path
+        if sqlite_file_extension is not None:
+            properties[cls._OPTIONAL_FILE_EXTENSION_SQLITE_PROPERTY] = sqlite_file_extension
+        if db_extra_args is not None:
+            properties[cls._OPTIONAL_DB_EXTRA_ARGS_SQL_PROPERTY] = db_extra_args
+        if exposed_type is not None:
+            properties[cls._OPTIONAL_EXPOSED_TYPE_SQL_PROPERTY] = exposed_type
+
+        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_SQL_TABLE, scope, **properties)
+
+    @classmethod
     def _configure_sql(
+        cls,
         id: str,
-        db_username: str,
-        db_password: str,
         db_name: str,
         db_engine: str,
-        db_port: int = 1433,
-        db_host: str = "localhost",
-        db_driver: str = "",
-        db_extra_args: Dict[str, Any] = None,
-        read_query: str = None,
-        write_query_builder: Callable = None,
-        exposed_type=_DEFAULT_EXPOSED_TYPE,
-        scope: Scope = _DEFAULT_SCOPE,
+        read_query: str,
+        write_query_builder: Callable,
+        db_username: Optional[str] = None,
+        db_password: Optional[str] = None,
+        db_host: Optional[str] = None,
+        db_port: Optional[int] = None,
+        db_driver: Optional[str] = None,
+        sqlite_folder_path: Optional[str] = None,
+        sqlite_file_extension: Optional[str] = None,
+        db_extra_args: Optional[Dict[str, Any]] = None,
+        exposed_type: Optional[str] = None,
+        scope: Optional[Scope] = None,
         **properties,
-    ):
+    ) -> "DataNodeConfig":
         """Configure a new SQL data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new SQL data node configuration.
-            db_username (str): The database username.
-            db_password (str): The database password.
             db_name (str): The database name, or the name of the SQLite database file.
-            db_engine (str): The database engine. Possible values are _"sqlite"_, _"mssql"_, _"mysql"_, or
-                _"postgresql"_.
-            db_port (int): The database port. The default value is 1433.
-            db_host (str): The database host. The default value is _"localhost"_.
-            db_driver (str): The database driver.
-            db_extra_args (Dict[str, Any]): A dictionary of additional arguments to be passed into database
-                connection string.
+            db_engine (str): The database engine. Possible values are *"sqlite"*, *"mssql"*, *"mysql"*,
+                or *"postgresql"*.
             read_query (str): The SQL query string used to read the data from the database.
-            write_query_builder (Callable): A callback function that takes the data as an input parameter and returns a
-                list of SQL queries.
-            exposed_type: The exposed type of the data read from SQL query. The default value is `pandas`.
-            scope (Scope^): The scope of the SQL data node configuration. The default value is
-                `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
-        Returns:
-            `DataNodeConfig^`: The new SQL data node configuration.
-        """
-        section = DataNodeConfig(
-            id,
-            DataNodeConfig._STORAGE_TYPE_VALUE_SQL,
-            scope=scope,
-            db_username=db_username,
-            db_password=db_password,
-            db_name=db_name,
-            db_host=db_host,
-            db_engine=db_engine,
-            db_driver=db_driver,
-            read_query=read_query,
-            write_query_builder=write_query_builder,
-            db_port=db_port,
-            db_extra_args=db_extra_args,
-            exposed_type=exposed_type,
-            **properties,
+            write_query_builder (Callable): A callback function that takes the data as an input parameter
+                and returns a list of SQL queries.
+            db_username (Optional[str]): The database username. Required by the *"mssql"*, *"mysql"*, and
+                *"postgresql"* engines.
+            db_password (Optional[str]): The database password. Required by the *"mssql"*, *"mysql"*, and
+                *"postgresql"* engines.
+            db_host (Optional[str]): The database host.<br/>
+                The default value is "localhost".
+            db_port (Optional[int]): The database port.<br/>
+                The default value is 1433.
+            db_driver (Optional[str]): The database driver.
+            sqlite_folder_path (Optional[str]): The path to the folder that contains SQLite file.<br/>
+                The default value is the current working folder.
+            sqlite_file_extension (Optional[str]): The file extension of the SQLite file.<br/>
+                The default value is ".db".
+            db_extra_args (Optional[dict[str, any]]): A dictionary of additional arguments to be passed
+                into database connection string.
+            exposed_type (Optional[str]): The exposed type of the data read from SQL query.<br/>
+                The default value is "pandas".
+            scope (Optional[Scope^]): The scope of the SQL data node configuration.<br/>
+                The default value is `Scope.SCENARIO`.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+        Returns:
+            The new SQL data node configuration.
+        """
+        properties.update(
+            {
+                cls._REQUIRED_DB_NAME_SQL_PROPERTY: db_name,
+                cls._REQUIRED_DB_ENGINE_SQL_PROPERTY: db_engine,
+                cls._REQUIRED_READ_QUERY_SQL_PROPERTY: read_query,
+                cls._REQUIRED_WRITE_QUERY_BUILDER_SQL_PROPERTY: write_query_builder,
+            }
         )
-        Config._register(section)
-        return Config.sections[DataNodeConfig.name][id]
 
-    @staticmethod
+        if db_username is not None:
+            properties[cls._OPTIONAL_DB_USERNAME_SQL_PROPERTY] = db_username
+        if db_password is not None:
+            properties[cls._OPTIONAL_DB_PASSWORD_SQL_PROPERTY] = db_password
+        if db_host is not None:
+            properties[cls._OPTIONAL_HOST_SQL_PROPERTY] = db_host
+        if db_port is not None:
+            properties[cls._OPTIONAL_PORT_SQL_PROPERTY] = db_port
+        if db_driver is not None:
+            properties[cls._OPTIONAL_DRIVER_SQL_PROPERTY] = db_driver
+        if sqlite_folder_path is not None:
+            properties[cls._OPTIONAL_FOLDER_PATH_SQLITE_PROPERTY] = sqlite_folder_path
+        if sqlite_file_extension is not None:
+            properties[cls._OPTIONAL_FILE_EXTENSION_SQLITE_PROPERTY] = sqlite_file_extension
+        if db_extra_args is not None:
+            properties[cls._OPTIONAL_DB_EXTRA_ARGS_SQL_PROPERTY] = db_extra_args
+        if exposed_type is not None:
+            properties[cls._OPTIONAL_EXPOSED_TYPE_SQL_PROPERTY] = exposed_type
+
+        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_SQL, scope, **properties)
+
+    @classmethod
     def _configure_mongo_collection(
+        cls,
         id: str,
         db_name: str,
         collection_name: str,
-        custom_document: Any = DefaultCustomDocument,
-        db_username: str = "",
-        db_password: str = "",
-        db_host: str = "localhost",
-        db_port: int = 27017,
-        db_extra_args: Dict[str, Any] = {},
-        scope: Scope = _DEFAULT_SCOPE,
+        custom_document: Optional[Any] = None,
+        db_username: Optional[str] = None,
+        db_password: Optional[str] = None,
+        db_host: Optional[str] = None,
+        db_port: Optional[int] = None,
+        db_extra_args: Optional[Dict[str, Any]] = None,
+        scope: Optional[Scope] = None,
         **properties,
-    ):
+    ) -> "DataNodeConfig":
         """Configure a new Mongo collection data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new Mongo collection data node configuration.
             db_name (str): The database name.
             collection_name (str): The collection in the database to read from and to write the data to.
-            custom_document (Any): The custom document class to store, encode, and decode data when reading and writing
-                to a Mongo collection. The custom_document can have optional `decode` method to decode data in the
-                Mongo collection to a custom object, and `encode` method to encode the object's properties to the
-                Mongo collection when writing.
-            db_username (str): The database username.
-            db_password (str): The database password.
-            db_host (str): The database host. The default value is _"localhost"_.
-            db_port (int): The database port. The default value is 27017.
-            db_extra_args (Dict[str, Any]): A dictionary of additional arguments to be passed into database connection
-                string.
-            scope (Scope^): The scope of the Mongo collection data node configuration. The default value is
-                `Scope.SCENARIO`.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
-        Returns:
-            `DataNodeConfig^`: The new Mongo collection data node configuration.
-        """
-        section = DataNodeConfig(
-            id,
-            DataNodeConfig._STORAGE_TYPE_VALUE_MONGO_COLLECTION,
-            scope=scope,
-            db_username=db_username,
-            db_password=db_password,
-            db_name=db_name,
-            collection_name=collection_name,
-            custom_document=custom_document,
-            db_host=db_host,
-            db_port=db_port,
-            db_extra_args=db_extra_args,
-            **properties,
+            custom_document (Optional[any]): The custom document class to store, encode, and decode data
+                when reading and writing to a Mongo collection. The custom_document can have an optional
+                *decode()* method to decode data in the Mongo collection to a custom object, and an
+                optional *encode()*) method to encode the object's properties to the Mongo collection
+                when writing.
+            db_username (Optional[str]): The database username.
+            db_password (Optional[str]): The database password.
+            db_host (Optional[str]): The database host.<br/>
+                The default value is "localhost".
+            db_port (Optional[int]): The database port.<br/>
+                The default value is 27017.
+            db_extra_args (Optional[dict[str, any]]): A dictionary of additional arguments to be passed
+                into database connection string.
+            scope (Optional[Scope^]): The scope of the Mongo collection data node configuration.<br/>
+                The default value is `Scope.SCENARIO`.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
+        Returns:
+            The new Mongo collection data node configuration.
+        """
+        properties.update(
+            {
+                cls._REQUIRED_DB_NAME_MONGO_PROPERTY: db_name,
+                cls._REQUIRED_COLLECTION_NAME_MONGO_PROPERTY: collection_name,
+            }
         )
+
+        if custom_document is not None:
+            properties[cls._OPTIONAL_CUSTOM_DOCUMENT_MONGO_PROPERTY] = custom_document
+        if db_username is not None:
+            properties[cls._OPTIONAL_USERNAME_MONGO_PROPERTY] = db_username
+        if db_password is not None:
+            properties[cls._OPTIONAL_PASSWORD_MONGO_PROPERTY] = db_password
+        if db_host is not None:
+            properties[cls._OPTIONAL_HOST_MONGO_PROPERTY] = db_host
+        if db_port is not None:
+            properties[cls._OPTIONAL_PORT_MONGO_PROPERTY] = db_port
+        if db_extra_args is not None:
+            properties[cls._OPTIONAL_DB_EXTRA_ARGS_MONGO_PROPERTY] = db_extra_args
+
+        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_MONGO_COLLECTION, scope, **properties)
+
+    @staticmethod
+    def __configure(
+        id: str,
+        storage_type: Optional[str] = None,
+        scope: Optional[Scope] = None,
+        **properties,
+    ):
+        section = DataNodeConfig(id, storage_type, scope, **properties)
         Config._register(section)
         return Config.sections[DataNodeConfig.name][id]
```

### Comparing `taipy-core-2.2.3/src/taipy/core/config/job_config.py` & `taipy-core-2.3.0.dev0/src/taipy/core/config/job_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 class JobConfig(UniqueSection):
     """
     Configuration fields related to the jobs' executions.
 
     Parameters:
         mode (str): The Taipy operating mode. By default, the "development" mode is set for testing and debugging the
             executions of jobs. A "standalone" mode is also available.
-        **properties (dict[str, Any]): A dictionary of additional properties.
+        **properties (dict[str, any]): A dictionary of additional properties.
     """
 
     name = "JOB"
 
     _MODE_KEY = "mode"
     _STANDALONE_MODE = "standalone"
     _DEVELOPMENT_MODE = "development"
@@ -72,28 +72,31 @@
             self._config = self._create_config(self.mode, **as_dict)
         if self._config is not None:
             self._update_config(as_dict)
 
     @staticmethod
     def _configure(
         mode: str = None, nb_of_workers: Union[int, str] = None, max_nb_of_workers: Union[int, str] = None, **properties
-    ):
+    ) -> "JobConfig":
         """Configure job execution.
+
         Parameters:
             mode (Optional[str]): The job execution mode.
-                Possible values are: _"standalone"_ (the default value) or
-                _"development"_.
-            max_nb_of_workers (Optional[int, str]): Parameter used only in default _"standalone"_ mode. The maximum
-                number of jobs able to run in parallel. The default value is 1.<br/>
+                Possible values are: *"standalone"* (the default value) or *"development"*.
+            max_nb_of_workers (Optional[int, str]): Parameter used only in default *"standalone"* mode.
+                This indicates the maximum number of jobs able to run in parallel.<br/>
+                The default value is 1.<br/>
                 A string can be provided to dynamically set the value using an environment
                 variable. The string must follow the pattern: `ENV[&lt;env_var&gt;]` where
-                `&lt;env_var&gt;` is the name of environment variable.
-            nb_of_workers (Optional[int, str]): Deprecated. Use max_nb_of_workers instead.
+                `&lt;env_var&gt;` is the name of an environment variable.
+            nb_of_workers (Optional[int, str]): Deprecated. Use *max_nb_of_workers* instead.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
         Returns:
-            `JobConfig^`: The job execution configuration.
+            The new job execution configuration.
         """
         if nb_of_workers:
             _warn_deprecated("nb_or_workers", suggest="max_nb_of_workers")
             if not max_nb_of_workers:
                 max_nb_of_workers = nb_of_workers
 
         section = JobConfig(mode, max_nb_of_workers=max_nb_of_workers, **properties)
```

### Comparing `taipy-core-2.2.3/src/taipy/core/config/pipeline_config.py` & `taipy-core-2.3.0.dev0/src/taipy/core/config/pipeline_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,21 @@
 from taipy.config.section import Section
 
 from .task_config import TaskConfig
 
 
 class PipelineConfig(Section):
     """
-    Holds all the configuration fields needed to instantiate an actual `Pipeline^` from the PipelineConfig.
+    Configuration fields needed to instantiate an actual `Pipeline^`.
 
     Attributes:
         id (str): Identifier of the pipeline configuration. It must be a valid Python variable name.
-        task_configs (Union[TaskConfig, List[TaskConfig]]): List of task configs. The default value is [].
-        **properties (dict[str, Any]): A dictionary of additional properties.
+        task_configs (Union[TaskConfig, List[TaskConfig]]): List of task configs.<br/>
+            The default value is [].
+        **properties (dict[str, any]): A dictionary of additional properties.
     """
 
     name = "PIPELINE"
 
     _TASK_KEY = "tasks"
 
     def __init__(self, id: str, tasks: Union[TaskConfig, List[TaskConfig]] = None, **properties):
@@ -76,44 +77,43 @@
         if self._tasks is None and default_section:
             self._tasks = default_section._tasks
         self._properties.update(as_dict)
         if default_section:
             self._properties = {**default_section.properties, **self._properties}
 
     @staticmethod
-    def _configure(id: str, task_configs: Union[TaskConfig, List[TaskConfig]], **properties):
+    def _configure(id: str, task_configs: Union[TaskConfig, List[TaskConfig]], **properties) -> "PipelineConfig":
         """Configure a new pipeline configuration.
 
         Parameters:
             id (str): The unique identifier of the new pipeline configuration.
             task_configs (Union[TaskConfig^, List[TaskConfig^]]): The list of the task
                 configurations that make this new pipeline. This can be a single task
                 configuration object is this pipeline holds a single task.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
         Returns:
-            `PipelineConfig^`: The new pipeline configuration.
+            The new pipeline configuration.
         """
         section = PipelineConfig(id, task_configs, **properties)
         Config._register(section)
         return Config.sections[PipelineConfig.name][id]
 
     @staticmethod
-    def _configure_default(task_configs: Union[TaskConfig, List[TaskConfig]], **properties):
+    def _configure_default(task_configs: Union[TaskConfig, List[TaskConfig]], **properties) -> "PipelineConfig":
         """Configure the default values for pipeline configurations.
 
-        This function creates the _default pipeline configuration_ object,
+        This function creates the *default pipeline configuration* object,
         where all pipeline configuration objects will find their default
         values when needed.
 
         Parameters:
             task_configs (Union[TaskConfig^, List[TaskConfig^]]): The list of the task
                 configurations that make the default pipeline configuration. This can be
                 a single task configuration object is this pipeline holds a single task.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
         Returns:
-            `PipelineConfig^`: The default pipeline configuration.
+            The default pipeline configuration.
         """
         section = PipelineConfig(_Config.DEFAULT_KEY, task_configs, **properties)
         Config._register(section)
         return Config.sections[PipelineConfig.name][_Config.DEFAULT_KEY]
```

### Comparing `taipy-core-2.2.3/src/taipy/core/config/scenario_config.py` & `taipy-core-2.3.0.dev0/src/taipy/core/config/scenario_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 
 from .pipeline_config import PipelineConfig
 from .task_config import TaskConfig
 
 
 class ScenarioConfig(Section):
     """
-    Holds all the configuration fields needed to instantiate an actual `Scenario^` from the `ScenarioConfig`.
+    Configuration fields needed to instantiate an actual `Scenario^`.
 
     Attributes:
         id (str): Identifier of the scenario config. It must be a valid Python variable name.
-        pipeline_configs (Union[PipelineConfig, List[PipelineConfig]]): List of pipeline configs. The default value
-            is [].
-        **properties (dict[str, Any]): A dictionary of additional properties.
+        pipeline_configs (Union[PipelineConfig, List[PipelineConfig]]): List of pipeline configs.<br/>
+            The default value is [].
+        **properties (dict[str, any]): A dictionary of additional properties.
     """
 
     name = "SCENARIO"
 
     _PIPELINE_KEY = "pipelines"
     _FREQUENCY_KEY = "frequency"
     _COMPARATOR_KEY = "comparators"
@@ -125,53 +125,53 @@
     @staticmethod
     def _configure(
         id: str,
         pipeline_configs: List[PipelineConfig],
         frequency: Optional[Frequency] = None,
         comparators: Optional[Dict[str, Union[List[Callable], Callable]]] = None,
         **properties,
-    ):
+    ) -> "ScenarioConfig":
         """Configure a new scenario configuration.
 
         Parameters:
             id (str): The unique identifier of the new scenario configuration.
             pipeline_configs (List[PipelineConfig^]): The list of pipeline configurations used
                 by this new scenario configuration.
-            frequency (Optional[Frequency^]): The scenario frequency.
+            frequency (Optional[Frequency^]): The scenario frequency.<br/>
                 It corresponds to the recurrence of the scenarios instantiated from this
                 configuration. Based on this frequency each scenario will be attached to the
                 relevant cycle.
             comparators (Optional[Dict[str, Union[List[Callable], Callable]]]): The list of
                 functions used to compare scenarios. A comparator function is attached to a
                 scenario's data node configuration. The key of the dictionary parameter
                 corresponds to the data node configuration id. During the scenarios'
                 comparison, each comparator is applied to all the data nodes instantiated from
                 the data node configuration attached to the comparator. See
                 `(taipy.)compare_scenarios()^` more more details.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
         Returns:
-            `ScenarioConfig^`: The new scenario configuration.
+            The new scenario configuration.
         """
         section = ScenarioConfig(id, pipeline_configs, frequency=frequency, comparators=comparators, **properties)
         Config._register(section)
         return Config.sections[ScenarioConfig.name][id]
 
     @staticmethod
     def _configure_from_tasks(
         id: str,
         task_configs: List[TaskConfig],
         frequency: Optional[Frequency] = None,
         comparators: Optional[Dict[str, Union[List[Callable], Callable]]] = None,
         pipeline_id: Optional[str] = None,
         **properties,
-    ):
+    ) -> "ScenarioConfig":
         """Configure a new scenario configuration made of a single new pipeline configuration.
 
-        A new pipeline configuration is created as well. If _pipeline_id_ is not provided,
+        A new pipeline configuration is created as well. If *pipeline_id* is not provided,
         the new pipeline configuration identifier is set to the scenario configuration identifier
         post-fixed by '_pipeline'.
 
         Parameters:
             id (str): The unique identifier of the scenario configuration.
             task_configs (List[TaskConfig^]): The list of task configurations used by the
                 new pipeline configuration that is created.
@@ -182,38 +182,37 @@
             comparators (Optional[Dict[str, Union[List[Callable], Callable]]]): The list of
                 functions used to compare scenarios. A comparator function is attached to a
                 scenario's data node configuration. The key of the dictionary parameter
                 corresponds to the data node configuration id. During the scenarios'
                 comparison, each comparator is applied to all the data nodes instantiated from
                 the data node configuration attached to the comparator. See
                 `(taipy.)compare_scenarios()` more more details.
-            pipeline_id (str): The identifier of the new pipeline configuration to be
-                configured.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+            pipeline_id (Optional[str]): The identifier of the new pipeline configuration to be configured.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
         Returns:
-            `ScenarioConfig^`: The new scenario configuration.
+            The new scenario configuration.
         """
         if not pipeline_id:
             pipeline_id = f"{id}_pipeline"
         pipeline_config = Config.configure_pipeline(pipeline_id, task_configs, **properties)
         section = ScenarioConfig(id, [pipeline_config], frequency=frequency, comparators=comparators, **properties)
         Config._register(section)
         return Config.sections[ScenarioConfig.name][id]
 
     @staticmethod
     def _configure_default(
         pipeline_configs: List[PipelineConfig],
         frequency: Optional[Frequency] = None,
         comparators: Optional[Dict[str, Union[List[Callable], Callable]]] = None,
         **properties,
-    ):
+    ) -> "ScenarioConfig":
         """Configure the default values for scenario configurations.
 
-        This function creates the _default scenario configuration_ object,
+        This function creates the *default scenario configuration* object,
         where all scenario configuration objects will find their default
         values when needed.
 
         Parameters:
             pipeline_configs (List[PipelineConfig^]): The list of pipeline configurations used
                 by this scenario configuration.
             frequency (Optional[Frequency^]): The scenario frequency.
@@ -223,17 +222,17 @@
             comparators (Optional[Dict[str, Union[List[Callable], Callable]]]): The list of
                 functions used to compare scenarios. A comparator function is attached to a
                 scenario's data node configuration. The key of the dictionary parameter
                 corresponds to the data node configuration id. During the scenarios'
                 comparison, each comparator is applied to all the data nodes instantiated from
                 the data node configuration attached to the comparator. See
                 `taipy.compare_scenarios()^` more more details.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
         Returns:
-            `ScenarioConfig^`: The default scenario configuration.
+            The new default scenario configuration.
         """
         section = ScenarioConfig(
             _Config.DEFAULT_KEY, pipeline_configs, frequency=frequency, comparators=comparators, **properties
         )
         Config._register(section)
         return Config.sections[ScenarioConfig.name][_Config.DEFAULT_KEY]
```

### Comparing `taipy-core-2.2.3/src/taipy/core/config/task_config.py` & `taipy-core-2.3.0.dev0/src/taipy/core/config/task_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,28 +19,32 @@
 
 from ..common._warnings import _warn_deprecated
 from .data_node_config import DataNodeConfig
 
 
 class TaskConfig(Section):
     """
-    Holds all the configuration fields needed to create an actual `Task^` from the `TaskConfig`.
+    Configuration fields needed to instantiate an actual `Task^`.
 
     Attributes:
         id (str): Identifier of the task config. Must be a valid Python variable name.
-        inputs (Union[DataNodeConfig^, List[DataNodeConfig^]]): The optional list of `DataNodeConfig^` inputs. The
-            default value is [].
-        outputs (Union[DataNodeConfig^, List[DataNodeConfig^]]): The optional list of `DataNodeConfig^` outputs. The
-            default value is [].
-        skippable (bool): If True, indicates that the task can be skipped if no change has been made on inputs. The
-            default value is _False_.
-        function (Callable): User function taking as inputs some parameters compatible with the exposed types
-            (_exposed_type_ field) of the input data nodes and returning results compatible with the exposed types
-            (_exposed_type_ field) of the outputs list. The default value is None.
-        **properties (dict[str, Any]): A dictionary of additional properties.
+        inputs (Union[DataNodeConfig^, List[DataNodeConfig^]]): The optional list of
+            `DataNodeConfig^` inputs.<br/>
+            The default value is [].
+        outputs (Union[DataNodeConfig^, List[DataNodeConfig^]]): The optional list of
+            `DataNodeConfig^` outputs.<br/>
+            The default value is [].
+        skippable (bool): If True, indicates that the task can be skipped if no change has
+            been made on inputs.<br/>
+            The default value is False.
+        function (Callable): User function taking as inputs some parameters compatible with the
+            exposed types (*exposed_type* field) of the input data nodes and returning results
+            compatible with the exposed types (*exposed_type* field) of the outputs list.<br/>
+            The default value is None.
+        **properties (dict[str, any]): A dictionary of additional properties.
     """
 
     name = "TASK"
 
     _INPUT_KEY = "inputs"
     _FUNCTION = "function"
     _OUTPUT_KEY = "outputs"
@@ -143,62 +147,64 @@
     def _configure(
         id: str,
         function,
         input: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = None,
         output: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = None,
         skippable: Optional[bool] = False,
         **properties,
-    ):
+    ) -> "TaskConfig":
         """Configure a new task configuration.
 
         Parameters:
             id (str): The unique identifier of this task configuration.
             function (Callable): The python function called by Taipy to run the task.
             input (Optional[Union[DataNodeConfig^, List[DataNodeConfig^]]]): The list of the
                 function input data node configurations. This can be a unique data node
                 configuration if there is a single input data node, or None if there are none.
             output (Optional[Union[DataNodeConfig^, List[DataNodeConfig^]]]): The list of the
                 function output data node configurations. This can be a unique data node
                 configuration if there is a single output data node, or None if there are none.
             skippable (bool): If True, indicates that the task can be skipped if no change has
-                been made on inputs. The default value is _False_.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
-                arguments.
+                been made on inputs.<br/>
+                The default value is False.
+            **properties (dict[str, any]): A keyworded variable length list of additional arguments.
+
         Returns:
-            `TaskConfig^`: The new task configuration.
+            The new task configuration.
         """
         section = TaskConfig(id, function, input, output, skippable, **properties)
         Config._register(section)
         return Config.sections[TaskConfig.name][id]
 
     @staticmethod
     def _configure_default(
         function,
         input: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = None,
         output: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = None,
         skippable: Optional[bool] = False,
         **properties,
-    ):
+    ) -> "TaskConfig":
         """Configure the default values for task configurations.
 
-        This function creates the _default task configuration_ object,
+        This function creates the *default task configuration* object,
         where all task configuration objects will find their default
         values when needed.
 
         Parameters:
             function (Callable): The python function called by Taipy to run the task.
             input (Optional[Union[DataNodeConfig^, List[DataNodeConfig^]]]): The list of the
                 input data node configurations. This can be a unique data node
                 configuration if there is a single input data node, or None if there are none.
             output (Optional[Union[DataNodeConfig^, List[DataNodeConfig^]]]): The list of the
                 output data node configurations. This can be a unique data node
                 configuration if there is a single output data node, or None if there are none.
             skippable (bool): If True, indicates that the task can be skipped if no change has
-                been made on inputs. The default value is _False_.
-            **properties (Dict[str, Any]): A keyworded variable length list of additional
+                been made on inputs.<br/>
+                The default value is False.
+            **properties (dict[str, any]): A keyworded variable length list of additional
                 arguments.
         Returns:
-            `TaskConfig^`: The default task configuration.
+            The default task configuration.
         """
         section = TaskConfig(_Config.DEFAULT_KEY, function, input, output, skippable, **properties)
         Config._register(section)
         return Config.sections[TaskConfig.name][_Config.DEFAULT_KEY]
```

### Comparing `taipy-core-2.2.3/src/taipy/core/cycle/__init__.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_version/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/cycle/_cycle_fs_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/cycle/_cycle_manager.py` & `taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,38 +11,40 @@
 
 import calendar
 from datetime import datetime, time, timedelta
 from typing import List, Optional
 
 from taipy.config.common.frequency import Frequency
 
+from .._entity._entity_ids import _EntityIds
 from .._manager._manager import _Manager
-from ..common._entity_ids import _EntityIds
-from ..common.alias import CycleId
 from ..job._job_manager_factory import _JobManagerFactory
+from ..notification import EventEntityType, EventOperation, _publish_event
 from ._cycle_repository_factory import _CycleRepositoryFactory
 from .cycle import Cycle
+from .cycle_id import CycleId
 
 
 class _CycleManager(_Manager[Cycle]):
-    _repository = _CycleRepositoryFactory._build_repository()  # type: ignore
+    _repository = _CycleRepositoryFactory._build_repository()
     _ENTITY_NAME = Cycle.__name__
+    _EVENT_ENTITY_TYPE = EventEntityType.CYCLE
 
     @classmethod
     def _create(
-        cls, frequency: Frequency, name: str = None, creation_date: datetime = None, display_name=None, **properties
+        cls, frequency: Frequency, name: Optional[str] = None, creation_date: Optional[datetime] = None, **properties
     ):
         creation_date = creation_date if creation_date else datetime.now()
         start_date = _CycleManager._get_start_date_of_cycle(frequency, creation_date)
         end_date = _CycleManager._get_end_date_of_cycle(frequency, start_date)
-        properties["display_name"] = display_name if display_name else start_date.isoformat()
         cycle = Cycle(
             frequency, properties, creation_date=creation_date, start_date=start_date, end_date=end_date, name=name
         )
         cls._set(cycle)
+        _publish_event(cls._EVENT_ENTITY_TYPE, cycle.id, EventOperation.CREATION, None)
         return cycle
 
     @classmethod
     def _get_all(cls, version_number: Optional[str] = "all") -> List[Cycle]:
         """
         Returns all entities.
         """
@@ -53,25 +55,23 @@
         """
         Returns all entities based on a criteria.
         """
         return cls._repository._load_all_by(by, version_number)
 
     @classmethod
     def _get_or_create(
-        cls, frequency: Frequency, creation_date: Optional[datetime] = None, display_name: Optional[str] = None
+        cls, frequency: Frequency, creation_date: Optional[datetime] = None, name: Optional[str] = None
     ) -> Cycle:
         creation_date = creation_date if creation_date else datetime.now()
         start_date = _CycleManager._get_start_date_of_cycle(frequency, creation_date)
-        cycles = cls._repository.get_cycles_by_frequency_and_start_date(
-            frequency=frequency, start_date=start_date
-        )  # type: ignore
+        cycles = cls._repository.get_cycles_by_frequency_and_start_date(frequency=frequency, start_date=start_date)
         if len(cycles) > 0:
             return cycles[0]
         else:
-            return cls._create(frequency=frequency, creation_date=creation_date, display_name=display_name)
+            return cls._create(frequency=frequency, creation_date=creation_date, name=name)
 
     @staticmethod
     def _get_start_date_of_cycle(frequency: Frequency, creation_date: datetime):
         start_date = creation_date.date()
         start_time = time()
         if frequency == Frequency.DAILY:
             start_date = start_date
```

### Comparing `taipy-core-2.2.3/src/taipy/core/cycle/_cycle_manager_factory.py` & `taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/cycle/_cycle_model.py` & `taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import dataclasses
 from dataclasses import dataclass
 from typing import Any, Dict
 
 from taipy.config.common.frequency import Frequency
 
-from ..common.alias import CycleId
+from .cycle_id import CycleId
 
 
 @dataclass
 class _CycleModel:
     id: CycleId
     name: str
     frequency: Frequency
```

### Comparing `taipy-core-2.2.3/src/taipy/core/cycle/_cycle_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/cycle/_cycle_repository_factory.py` & `taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/cycle/_cycle_sql_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/cycle/_cycle_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/data/__init__.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/data/_data_fs_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/_data_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/data/_data_manager.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/_data_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,37 +12,43 @@
 import os
 from typing import Dict, Iterable, Optional, Set, Union
 
 from taipy.config._config import _Config
 from taipy.config.common.scope import Scope
 from taipy.config.config import Config
 
+from .._backup._backup import append_to_backup_file, remove_from_backup_file
 from .._manager._manager import _Manager
 from .._version._version_manager_factory import _VersionManagerFactory
-from ..common.alias import CycleId, DataNodeId, PipelineId, ScenarioId, TaskId
 from ..config.data_node_config import DataNodeConfig
+from ..cycle.cycle_id import CycleId
 from ..exceptions.exceptions import InvalidDataNodeType
+from ..notification import EventEntityType, EventOperation, _publish_event
+from ..pipeline.pipeline_id import PipelineId
+from ..scenario.scenario_id import ScenarioId
 from ._data_repository_factory import _DataRepositoryFactory
+from .abstract_file import _AbstractFileDataNode
 from .data_node import DataNode
+from .data_node_id import DataNodeId
 from .pickle import PickleDataNode
 
 
 class _DataManager(_Manager[DataNode]):
     __DATA_NODE_CLASS_MAP = DataNode._class_map()  # type: ignore
     _repository = _DataRepositoryFactory._build_repository()  # type: ignore
     _ENTITY_NAME = DataNode.__name__
+    _EVENT_ENTITY_TYPE = EventEntityType.DATA_NODE
 
     @classmethod
     def _bulk_get_or_create(
         cls,
         data_node_configs: Set[DataNodeConfig],
         cycle_id: Optional[CycleId] = None,
         scenario_id: Optional[ScenarioId] = None,
         pipeline_id: Optional[PipelineId] = None,
-        task_id: Optional[TaskId] = None,
     ) -> Dict[DataNodeConfig, DataNode]:
         dn_configs_and_owner_id = []
         for dn_config in data_node_configs:
             scope = dn_config.scope
             owner_id: Union[Optional[PipelineId], Optional[ScenarioId], Optional[CycleId]]
             if scope == Scope.PIPELINE:
                 owner_id = pipeline_id
@@ -63,66 +69,93 @@
 
     @classmethod
     def _create_and_set(
         cls, data_node_config: DataNodeConfig, owner_id: Optional[str], parent_ids: Optional[Set[str]]
     ) -> DataNode:
         data_node = cls.__create(data_node_config, owner_id, parent_ids)
         cls._set(data_node)
+        if isinstance(data_node, _AbstractFileDataNode):
+            append_to_backup_file(new_file_path=data_node._path)
+        _publish_event(cls._EVENT_ENTITY_TYPE, data_node.id, EventOperation.CREATION, None)
         return data_node
 
     @classmethod
     def __create(
         cls, data_node_config: DataNodeConfig, owner_id: Optional[str], parent_ids: Optional[Set[str]]
     ) -> DataNode:
         try:
             version = _VersionManagerFactory._build_manager()._get_latest_version()
             props = data_node_config._properties.copy()
             validity_period = props.pop("validity_period", None)
+
             if data_node_config.storage_type:
                 storage_type = data_node_config.storage_type
             else:
                 storage_type = Config.sections[DataNodeConfig.name][_Config.DEFAULT_KEY].storage_type
 
-            return cls.__DATA_NODE_CLASS_MAP[storage_type](  # type: ignore
+            return cls.__DATA_NODE_CLASS_MAP[storage_type](
                 config_id=data_node_config.id,
                 scope=data_node_config.scope or DataNodeConfig._DEFAULT_SCOPE,
                 owner_id=owner_id,
                 parent_ids=parent_ids,
                 version=version,
                 validity_period=validity_period,
                 properties=props,
             )
         except KeyError:
             raise InvalidDataNodeType(data_node_config.storage_type)
 
     @classmethod
-    def _clean_pickle_file(cls, data_node: Union[DataNode, DataNodeId]):
-        data_node = cls._get(data_node) if isinstance(data_node, str) else data_node
+    def _clean_pickle_file(cls, data_node: DataNode):
         if not isinstance(data_node, PickleDataNode):
             return
         if data_node.is_generated and os.path.exists(data_node.path):
             os.remove(data_node.path)
 
     @classmethod
-    def _clean_pickle_files(cls, data_nodes: Iterable[Union[DataNode, DataNodeId]]):
+    def _clean_pickle_files(cls, data_nodes: Iterable[DataNode]):
         for data_node in data_nodes:
             cls._clean_pickle_file(data_node)
 
     @classmethod
-    def _delete(cls, data_node_id: DataNodeId):  # type:ignore
-        cls._clean_pickle_file(data_node_id)
+    def _remove_dn_file_path_in_backup_file(cls, data_node: DataNode):
+        if isinstance(data_node, _AbstractFileDataNode):
+            remove_from_backup_file(to_remove_file_path=data_node.path)
+
+    @classmethod
+    def _remove_dn_file_paths_in_backup_file(cls, data_nodes: Iterable[DataNode]):
+        for data_node in data_nodes:
+            if isinstance(data_node, _AbstractFileDataNode):
+                remove_from_backup_file(to_remove_file_path=data_node.path)
+
+    @classmethod
+    def _delete(cls, data_node_id: DataNodeId):
+        data_node = cls._get(data_node_id, None)
         super()._delete(data_node_id)
+        if data_node:
+            cls._clean_pickle_file(data_node)
+            cls._remove_dn_file_path_in_backup_file(data_node)
 
     @classmethod
-    def _delete_many(cls, data_node_ids: Iterable[DataNodeId]):  # type:ignore
-        cls._clean_pickle_files(data_node_ids)
+    def _delete_many(cls, data_node_ids: Iterable[DataNodeId]):
+        data_nodes = []
+        for data_node_id in data_node_ids:
+            if data_node := cls._get(data_node_id):
+                data_nodes.append(data_node)
         super()._delete_many(data_node_ids)
+        cls._clean_pickle_files(data_nodes)
+        cls._remove_dn_file_paths_in_backup_file(data_nodes)
 
     @classmethod
     def _delete_all(cls):
-        cls._clean_pickle_files(cls._get_all())
+        data_nodes = cls._get_all()
         super()._delete_all()
+        cls._clean_pickle_files(data_nodes)
+        cls._remove_dn_file_paths_in_backup_file(data_nodes)
 
     @classmethod
     def _delete_by_version(cls, version_number: str):
-        cls._clean_pickle_files(cls._get_all(version_number))
-        cls._repository._delete_by(attribute="version", value=version_number, version_number="all")  # type: ignore
+        data_nodes = cls._get_all(version_number)
+        cls._repository._delete_by(attribute="version", value=version_number, version_number="all")
+        cls._clean_pickle_files(data_nodes)
+        cls._remove_dn_file_paths_in_backup_file(data_nodes)
+        _publish_event(cls._EVENT_ENTITY_TYPE, None, EventOperation.DELETION, None)
```

### Comparing `taipy-core-2.2.3/src/taipy/core/data/_data_manager_factory.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/_data_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/data/_data_model.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/_data_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from datetime import datetime
 from typing import Any, Dict, List, Optional, cast
 
 from taipy.config.common.scope import Scope
 
 from .._version._utils import _version_migration
 from ..common._warnings import _warn_deprecated
-from ..common.alias import Edit
+from .data_node_id import Edit
 
 
 def _to_edits_migration(job_ids: Optional[List[str]]) -> List[Edit]:
     "Migrate a list of job IDs to a list of Edits. Used to migrate data model from <=2.0 to >=2.1 version." ""
     _warn_deprecated("job_ids", suggest="edits")
     if not job_ids:
         return []
@@ -34,15 +34,15 @@
 
 @dataclass
 class _DataNodeModel:
     id: str
     config_id: str
     scope: Scope
     storage_type: str
-    name: str
+    name: Optional[str]
     owner_id: Optional[str]
     parent_ids: List[str]
     last_edit_date: Optional[str]
     edits: List[Edit]
     version: str
     validity_days: Optional[float]
     validity_seconds: Optional[float]
@@ -59,15 +59,15 @@
         if data.get("cacheable"):
             dn_properties["cacheable"] = True
         return _DataNodeModel(
             id=data["id"],
             config_id=data["config_id"],
             scope=Scope._from_repr(data["scope"]),
             storage_type=data["storage_type"],
-            name=data["name"],
+            name=data.get("name"),
             owner_id=data.get("owner_id", data.get("parent_id")),
             parent_ids=data.get("parent_ids", []),
             last_edit_date=data.get("last_edit_date", data.get("last_edition_date")),
             edits=data.get("edits", _to_edits_migration(data.get("job_ids"))),
             version=data["version"] if "version" in data.keys() else _version_migration(),
             validity_days=data["validity_days"],
             validity_seconds=data["validity_seconds"],
```

### Comparing `taipy-core-2.2.3/src/taipy/core/data/_data_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/_data_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,25 +47,25 @@
     @property
     def repository(self):
         return self.repo
 
     def _to_model(self, data_node: DataNode):
         properties = data_node._properties.data.copy()
         if data_node.storage_type() == GenericDataNode.storage_type():
-            read_fct = data_node._properties[GenericDataNode._REQUIRED_READ_FUNCTION_PROPERTY]
+            read_fct = data_node._properties.get(GenericDataNode._OPTIONAL_READ_FUNCTION_PROPERTY, None)
             properties[self._READ_FCT_NAME_KEY] = read_fct.__name__ if read_fct else None
             properties[self._READ_FCT_MODULE_KEY] = read_fct.__module__ if read_fct else None
 
-            write_fct = data_node._properties[GenericDataNode._REQUIRED_WRITE_FUNCTION_PROPERTY]
+            write_fct = data_node._properties.get(GenericDataNode._OPTIONAL_WRITE_FUNCTION_PROPERTY, None)
             properties[self._WRITE_FCT_NAME_KEY] = write_fct.__name__ if write_fct else None
             properties[self._WRITE_FCT_MODULE_KEY] = write_fct.__module__ if write_fct else None
 
             del (
-                properties[GenericDataNode._REQUIRED_READ_FUNCTION_PROPERTY],
-                properties[GenericDataNode._REQUIRED_WRITE_FUNCTION_PROPERTY],
+                properties[GenericDataNode._OPTIONAL_READ_FUNCTION_PROPERTY],
+                properties[GenericDataNode._OPTIONAL_WRITE_FUNCTION_PROPERTY],
             )
 
         if data_node.storage_type() == JSONDataNode.storage_type():
             encoder = data_node._properties.get(JSONDataNode._ENCODER_KEY)
             properties[self._JSON_ENCODER_NAME_KEY] = encoder.__name__ if encoder else None
             properties[self._JSON_ENCODER_MODULE_KEY] = encoder.__module__ if encoder else None
             properties.pop(JSONDataNode._ENCODER_KEY, None)
@@ -121,28 +121,28 @@
             data_node._edit_in_progress,
             properties,
         )
 
     def _from_model(self, model: _DataNodeModel):
         if model.storage_type == GenericDataNode.storage_type():
             if model.data_node_properties[self._READ_FCT_MODULE_KEY]:
-                model.data_node_properties[GenericDataNode._REQUIRED_READ_FUNCTION_PROPERTY] = _load_fct(
+                model.data_node_properties[GenericDataNode._OPTIONAL_READ_FUNCTION_PROPERTY] = _load_fct(
                     model.data_node_properties[self._READ_FCT_MODULE_KEY],
                     model.data_node_properties[self._READ_FCT_NAME_KEY],
                 )
             else:
-                model.data_node_properties[GenericDataNode._REQUIRED_READ_FUNCTION_PROPERTY] = None
+                model.data_node_properties[GenericDataNode._OPTIONAL_READ_FUNCTION_PROPERTY] = None
 
             if model.data_node_properties[self._WRITE_FCT_MODULE_KEY]:
-                model.data_node_properties[GenericDataNode._REQUIRED_WRITE_FUNCTION_PROPERTY] = _load_fct(
+                model.data_node_properties[GenericDataNode._OPTIONAL_WRITE_FUNCTION_PROPERTY] = _load_fct(
                     model.data_node_properties[self._WRITE_FCT_MODULE_KEY],
                     model.data_node_properties[self._WRITE_FCT_NAME_KEY],
                 )
             else:
-                model.data_node_properties[GenericDataNode._REQUIRED_WRITE_FUNCTION_PROPERTY] = None
+                model.data_node_properties[GenericDataNode._OPTIONAL_WRITE_FUNCTION_PROPERTY] = None
 
             del model.data_node_properties[self._READ_FCT_NAME_KEY]
             del model.data_node_properties[self._READ_FCT_MODULE_KEY]
             del model.data_node_properties[self._WRITE_FCT_NAME_KEY]
             del model.data_node_properties[self._WRITE_FCT_MODULE_KEY]
 
         if model.storage_type == JSONDataNode.storage_type():
@@ -245,7 +245,10 @@
         return self.repo._delete_many(ids)
 
     def _search(self, attribute: str, value: Any, version_number: Optional[str] = None) -> Optional[DataNode]:
         return self.repo._search(attribute, value, version_number)
 
     def _export(self, entity_id: str, folder_path: Union[str, pathlib.Path]):
         return self.repo._export(entity_id, folder_path)
+
+    def _get_by_config_id(self, config_id: str) -> List[DataNode]:
+        return self.repo._get_by_config_id(config_id)
```

### Comparing `taipy-core-2.2.3/src/taipy/core/data/_data_repository_factory.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/_data_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/data/_data_sql_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/_data_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/data/_filter.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/_filter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/data/abstract_sql.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/abstract_sql.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 import modin.pandas as modin_pd
 import pandas as pd
 from sqlalchemy import create_engine, text
 
 from taipy.config.common.scope import Scope
 
 from .._version._version_manager_factory import _VersionManagerFactory
-from ..common.alias import DataNodeId, Edit
 from ..exceptions.exceptions import InvalidExposedType, MissingRequiredProperty, UnknownDatabaseEngine
 from .data_node import DataNode
+from .data_node_id import DataNodeId, Edit
 
 
 class _AbstractSQLDataNode(DataNode):
     """Abstract base class for data node implementations (SQLDataNode and SQLTableDataNode) that use SQL."""
 
     __STORAGE_TYPE = "NOT_IMPLEMENTED"
 
@@ -43,30 +43,34 @@
     __DB_USERNAME_KEY = "db_username"
     __DB_PASSWORD_KEY = "db_password"
     __DB_HOST_KEY = "db_host"
     __DB_PORT_KEY = "db_port"
     __DB_ENGINE_KEY = "db_engine"
     __DB_DRIVER_KEY = "db_driver"
     __DB_EXTRA_ARGS_KEY = "db_extra_args"
-    __SQLITE_PATH_KEY = "path"
+    __SQLITE_FOLDER_PATH = "sqlite_folder_path"
+    __SQLITE_FILE_EXTENSION = "sqlite_file_extension"
 
     __ENGINE_PROPERTIES: List[str] = [
         __DB_NAME_KEY,
         __DB_USERNAME_KEY,
         __DB_PASSWORD_KEY,
         __DB_HOST_KEY,
         __DB_PORT_KEY,
         __DB_DRIVER_KEY,
         __DB_EXTRA_ARGS_KEY,
-        __SQLITE_PATH_KEY,
+        __SQLITE_FOLDER_PATH,
+        __SQLITE_FILE_EXTENSION,
     ]
 
     __DB_HOST_DEFAULT = "localhost"
     __DB_PORT_DEFAULT = 1433
     __DB_DRIVER_DEFAULT = ""
+    __SQLITE_FOLDER_PATH_DEFAULT = ""
+    __SQLITE_FILE_EXTENSION_DEFAULT = ".db"
 
     __ENGINE_MSSQL = "mssql"
     __ENGINE_SQLITE = "sqlite"
     __ENGINE_MYSQL = "mysql"
     __ENGINE_POSTGRESQL = "postgresql"
 
     _ENGINE_REQUIRED_PROPERTIES: Dict[str, List[str]] = {
@@ -171,16 +175,17 @@
         if engine == self.__ENGINE_MSSQL:
             return f"mssql+pyodbc://{username}:{password}@{host}:{port}/{db_name}?{extra_args_str}"
         elif engine == self.__ENGINE_MYSQL:
             return f"mysql+pymysql://{username}:{password}@{host}:{port}/{db_name}?{extra_args_str}"
         elif engine == self.__ENGINE_POSTGRESQL:
             return f"postgresql+psycopg2://{username}:{password}@{host}:{port}/{db_name}?{extra_args_str}"
         elif engine == self.__ENGINE_SQLITE:
-            path = self.properties.get(self.__SQLITE_PATH_KEY, "")
-            return os.path.join("sqlite:///", path, f"{db_name}")
+            folder_path = self.properties.get(self.__SQLITE_FOLDER_PATH, self.__SQLITE_FOLDER_PATH_DEFAULT)
+            file_extension = self.properties.get(self.__SQLITE_FILE_EXTENSION, self.__SQLITE_FILE_EXTENSION_DEFAULT)
+            return "sqlite:///" + os.path.join(folder_path, f"{db_name}{file_extension}")
 
         raise UnknownDatabaseEngine(f"Unknown engine: {engine}")
 
     def _read(self):
         if self.properties[self.__EXPOSED_TYPE_PROPERTY] == self.__EXPOSED_TYPE_PANDAS:
             return self._read_as_pandas_dataframe()
         if self.properties[self.__EXPOSED_TYPE_PROPERTY] == self.__EXPOSED_TYPE_MODIN:
@@ -219,17 +224,17 @@
     def _write(self, data) -> None:
         """Check data against a collection of types to handle insertion on the database."""
         engine = self._get_engine()
         with engine.connect() as connection:
             with connection.begin() as transaction:
                 try:
                     self._do_write(data, engine, connection)
-                except:  # noqa: E722
+                except Exception as e:
                     transaction.rollback()
-                    raise
+                    raise e
                 else:
                     transaction.commit()
 
     def __setattr__(self, key: str, value) -> None:
         if key in self.__ENGINE_PROPERTIES:
             self._engine = None
         return super().__setattr__(key, value)
```

### Comparing `taipy-core-2.2.3/src/taipy/core/data/csv.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,31 +6,35 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import csv
+import os
 from datetime import datetime, timedelta
 from os.path import isfile
 from typing import Any, Dict, List, Optional, Set
 
 import modin.pandas as modin_pd
 import pandas as pd
 
 from taipy.config.common.scope import Scope
 
+from .._backup._backup import replace_in_backup_file
+from .._entity._reload import _self_reload
 from .._version._version_manager_factory import _VersionManagerFactory
-from ..common._reload import _self_reload
-from ..common.alias import DataNodeId, Edit, JobId
-from ..exceptions.exceptions import InvalidExposedType, MissingRequiredProperty
+from ..exceptions.exceptions import InvalidExposedType
+from ..job.job_id import JobId
+from .abstract_file import _AbstractFileDataNode
 from .data_node import DataNode
+from .data_node_id import DataNodeId, Edit
 
 
-class CSVDataNode(DataNode):
+class CSVDataNode(DataNode, _AbstractFileDataNode):
     """Data Node stored as a CSV file.
 
     Attributes:
         config_id (str): Identifier of the data node configuration. This string must be a valid
             Python identifier.
         scope (Scope^): The scope of this data node.
         id (str): The unique identifier of this data node.
@@ -59,14 +63,15 @@
     __EXPOSED_TYPE_PROPERTY = "exposed_type"
     __EXPOSED_TYPE_NUMPY = "numpy"
     __EXPOSED_TYPE_PANDAS = "pandas"
     __EXPOSED_TYPE_MODIN = "modin"
     __VALID_STRING_EXPOSED_TYPES = [__EXPOSED_TYPE_PANDAS, __EXPOSED_TYPE_MODIN, __EXPOSED_TYPE_NUMPY]
     __PATH_KEY = "path"
     __DEFAULT_PATH_KEY = "default_path"
+    __DEFAULT_DATA_KEY = "default_data"
     __HAS_HEADER_PROPERTY = "has_header"
     _REQUIRED_PROPERTIES: List[str] = []
 
     def __init__(
         self,
         config_id: str,
         scope: Scope,
@@ -79,28 +84,20 @@
         version: str = None,
         validity_period: Optional[timedelta] = None,
         edit_in_progress: bool = False,
         properties: Dict = None,
     ):
         if properties is None:
             properties = {}
-        if missing := set(self._REQUIRED_PROPERTIES) - set(properties.keys()):
-            raise MissingRequiredProperty(
-                f"The following properties " f"{', '.join(x for x in missing)} were not informed and are required"
-            )
+
+        default_value = properties.pop(self.__DEFAULT_DATA_KEY, None)
 
         if self.__HAS_HEADER_PROPERTY not in properties.keys():
             properties[self.__HAS_HEADER_PROPERTY] = True
 
-        self._path = properties.get(self.__PATH_KEY, properties.get(self.__DEFAULT_PATH_KEY))
-        if self._path is None:
-            raise MissingRequiredProperty("default_path is required in a CSV data node config")
-        else:
-            properties[self.__PATH_KEY] = self._path
-
         if self.__EXPOSED_TYPE_PROPERTY not in properties.keys():
             properties[self.__EXPOSED_TYPE_PROPERTY] = self.__EXPOSED_TYPE_PANDAS
         self._check_exposed_type(properties[self.__EXPOSED_TYPE_PROPERTY])
 
         super().__init__(
             config_id,
             scope,
@@ -111,30 +108,39 @@
             last_edit_date,
             edits,
             version or _VersionManagerFactory._build_manager()._get_latest_version(),
             validity_period,
             edit_in_progress,
             **properties,
         )
+        self._path = properties.get(self.__PATH_KEY, properties.get(self.__DEFAULT_PATH_KEY))
+        if not self._path:
+            self._path = self._build_path(self.storage_type())
+        properties[self.__PATH_KEY] = self._path
+
         if not self._last_edit_date and isfile(self._path):
             self.last_edit_date = datetime.now()  # type: ignore
+        if default_value is not None and not os.path.exists(self._path):
+            self.write(default_value)
 
     @classmethod
     def storage_type(cls) -> str:
         return cls.__STORAGE_TYPE
 
     @property  # type: ignore
     @_self_reload(DataNode._MANAGER_NAME)
     def path(self):
         return self._path
 
     @path.setter
     def path(self, value):
+        tmp_old_path = self._path
         self._path = value
         self.properties[self.__PATH_KEY] = value
+        replace_in_backup_file(old_file_path=tmp_old_path, new_file_path=self._path)
 
     def _check_exposed_type(self, exposed_type):
         if isinstance(exposed_type, str) and exposed_type not in self.__VALID_STRING_EXPOSED_TYPES:
             raise InvalidExposedType(
                 f"Invalid string exposed type {exposed_type}. Supported values are "
                 f"{', '.join(self.__VALID_STRING_EXPOSED_TYPES)}"
             )
```

### Comparing `taipy-core-2.2.3/src/taipy/core/data/data_node.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/data_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,79 +10,83 @@
 # specific language governing permissions and limitations under the License.
 
 import os
 import uuid
 from abc import abstractmethod
 from datetime import datetime, timedelta
 from functools import reduce
-from typing import Any, List, Optional, Set, Tuple, Union
+from typing import Any, Dict, List, Optional, Set, Tuple, Union
 
 import modin.pandas as modin_pd
 import numpy as np
 import pandas as pd
 
 from taipy.config.common._validate_id import _validate_id
 from taipy.config.common.scope import Scope
 from taipy.logger._taipy_logger import _TaipyLogger
 
+from .._entity._entity import _Entity
+from .._entity._labeled import _Labeled
+from .._entity._properties import _Properties
+from .._entity._reload import _reload, _self_reload, _self_setter
 from .._version._version_manager_factory import _VersionManagerFactory
-from ..common._entity import _Entity
-from ..common._properties import _Properties
-from ..common._reload import _reload, _self_reload, _self_setter
 from ..common._warnings import _warn_deprecated
-from ..common.alias import DataNodeId, Edit, JobId
 from ..exceptions.exceptions import NoData
+from ..job.job_id import JobId
 from ._filter import _FilterDataNode
+from .data_node_id import DataNodeId, Edit
 from .operator import JoinOperator, Operator
 
 
-class DataNode(_Entity):
+class DataNode(_Entity, _Labeled):
     """Reference to a dataset.
 
     A Data Node is an abstract class that holds metadata related to the dataset it refers to.
     In particular, a data node holds the name, the scope, the owner identifier, the last
     edit date, and some additional properties of the data.<br/>
     A Data Node also contains information and methods needed to access the dataset. This
     information depends on the type of storage, and it is held by subclasses (such as
     SQL Data Node, CSV Data Node, ...).
 
     !!! note
-        It is recommended not to instantiate subclasses of DataNode directly.
+        It is recommended not to instantiate subclasses of `DataNode` directly.
 
     Attributes:
         config_id (str): Identifier of the data node configuration. It must be a valid Python
             identifier.
         scope (Scope^): The scope of this data node.
         id (str): The unique identifier of this data node.
         name (str): A user-readable name of this data node.
         owner_id (str): The identifier of the owner (pipeline_id, scenario_id, cycle_id) or
-            `None`.
+            None.
         parent_ids (Optional[Set[str]]): The set of identifiers of the parent tasks.
         last_edit_date (datetime): The date and time of the last modification.
-        edits (List[Edit^]): The list of Edits (an alias for dict) containing medata about each edition of that node.
-        version (str): The string indicates the application version of the data node to instantiate. If not provided,
-            the current version is used.
+        edits (List[Edit^]): The list of Edits (an alias for dict) containing medata about each
+            edition of that node.
+        version (str): The string indicates the application version of the data node to
+            instantiate. If not provided, the current version is used.
         validity_period (Optional[timedelta]): The validity period of a data node.
-            Implemented as a timedelta. If _validity_period_ is set to None, the data_node is
+            Implemented as a timedelta. If *validity_period* is set to None, the data node is
             always up-to-date.
-        edit_in_progress (bool): True if the data node is locked for modification. False otherwise.
+        edit_in_progress (bool): True if the data node is locked for modification. False
+            otherwise.
         kwargs: A dictionary of additional properties.
     """
 
     _ID_PREFIX = "DATANODE"
     __ID_SEPARATOR = "_"
     __logger = _TaipyLogger._get_logger()
     _REQUIRED_PROPERTIES: List[str] = []
     _MANAGER_NAME = "data"
     __PATH_KEY = "path"
 
     def __init__(
         self,
         config_id,
-        scope: Scope = Scope(Scope.PIPELINE),
+        scope: Scope = Scope(Scope.SCENARIO),
         id: Optional[DataNodeId] = None,
         name: Optional[str] = None,
         owner_id: Optional[str] = None,
         parent_ids: Optional[Set[str]] = None,
         last_edit_date: Optional[datetime] = None,
         edits: Optional[List[Edit]] = None,
         version: Optional[str] = None,
@@ -92,60 +96,60 @@
     ):
         self.config_id = _validate_id(config_id)
         self.id = id or DataNodeId(self.__ID_SEPARATOR.join([self._ID_PREFIX, self.config_id, str(uuid.uuid4())]))
         self.owner_id = owner_id
         self._parent_ids = parent_ids or set()
         self._scope = scope
         self._last_edit_date = last_edit_date
-        self._name = name or self.id
+        self._name = name
         self._edit_in_progress = edit_in_progress
         self._version = version or _VersionManagerFactory._build_manager()._get_latest_version()
         self._validity_period = validity_period
 
         # Track edits
         self._edits = edits or list()
 
         self._properties = _Properties(self, **kwargs)
 
-    @property  # type: ignore
+    @property
     def parent_id(self):
-        """
-        Deprecated. Use owner_id instead.
-        """
+        """Deprecated. Use `owner_id` instead."""
         _warn_deprecated("parent_id", suggest="owner_id")
         return self.owner_id
 
-    @parent_id.setter  # type: ignore
+    @parent_id.setter
     def parent_id(self, val):
-        """
-        Deprecated. Use owner_id instead.
-        """
+        """Deprecated. Use `owner_id` instead."""
         _warn_deprecated("parent_id", suggest="owner_id")
         self.owner_id = val
 
     def get_parents(self):
-        """Get all parents of the data node."""
+        """Get all parents of this data node."""
         from ... import core as tp
 
         return tp.get_parents(self)
 
     @property  # type: ignore
     @_self_reload(_MANAGER_NAME)
     def parent_ids(self):
-        """List of parent ids of the data node."""
+        """List of parent ids of this data node."""
         return self._parent_ids
 
     @property  # type: ignore
     @_self_reload(_MANAGER_NAME)
     def edits(self):
-        """Get all `Edit^`s of the data node."""
+        """Get all `Edit^`s of this data node."""
         return self._edits
 
-    def get_last_edit(self):
-        """Get last `Edit^` of the data node, or None"""
+    def get_last_edit(self) -> Optional[Edit]:
+        """Get last `Edit^` of this data node.
+
+        Returns:
+            None if there has been no `Edit^` on this data node.
+        """
         if self._edits:
             return self._edits[-1]
         return None
 
     @property  # type: ignore
     @_self_reload(_MANAGER_NAME)
     def last_edit_date(self):
@@ -156,21 +160,21 @@
             return self._last_edit_date
 
     @last_edit_date.setter  # type: ignore
     @_self_setter(_MANAGER_NAME)
     def last_edit_date(self, val):
         self._last_edit_date = val
 
-    @property  # type: ignore
+    @property
     def last_edition_date(self):
-        """Deprecated. Use last_edit_date instead."""
+        """Deprecated. Use `last_edit_date` instead."""
         _warn_deprecated("last_edition_date", suggest="last_edit_date")
         return self.last_edit_date
 
-    @last_edition_date.setter  # type: ignore
+    @last_edition_date.setter
     def last_edition_date(self, val):
         _warn_deprecated("last_edition_date", suggest="last_edit_date")
         self.last_edit_date = val
 
     @property  # type: ignore
     @_self_reload(_MANAGER_NAME)
     def scope(self):
@@ -190,15 +194,15 @@
     @_self_setter(_MANAGER_NAME)
     def validity_period(self, val):
         self._validity_period = val
 
     @property  # type: ignore
     @_self_reload(_MANAGER_NAME)
     def expiration_date(self) -> datetime:
-        """Datetime instant of the expiration date of the data node."""
+        """Datetime instant of the expiration date of this data node."""
         last_edit_date = self.last_edit_date
         validity_period = self._validity_period
 
         if not last_edit_date:
             raise NoData(f"Data node {self.id} from config {self.config_id} has not been written yet.")
 
         return last_edit_date + validity_period if validity_period else last_edit_date
@@ -209,57 +213,57 @@
         return self._name
 
     @name.setter  # type: ignore
     @_self_setter(_MANAGER_NAME)
     def name(self, val):
         self._name = val
 
-    @property  # type: ignore
+    @property
     def version(self):
         return self._version
 
-    @property  # type: ignore
+    @property
     def cacheable(self):
         """Deprecated. Use `skippable` attribute of a `Task^` instead."""
         _warn_deprecated("cacheable", suggest="the skippable feature")
         return self.properties.get("cacheable", False)
 
-    @cacheable.setter  # type: ignore
+    @cacheable.setter
     def cacheable(self, val):
         _warn_deprecated("cacheable", suggest="the skippable feature")
 
     @property  # type: ignore
     @_self_reload(_MANAGER_NAME)
     def edit_in_progress(self):
         return self._edit_in_progress
 
     @edit_in_progress.setter  # type: ignore
     @_self_setter(_MANAGER_NAME)
     def edit_in_progress(self, val):
         self._edit_in_progress = val
 
-    @property  # type: ignore
+    @property
     def edition_in_progress(self):
-        """Deprecated. Use edit_in_progress instead."""
+        """Deprecated. Use `edit_in_progress` instead."""
         _warn_deprecated("edition_in_progress", suggest="edit_in_progress")
         return self.edit_in_progress
 
-    @edition_in_progress.setter  # type: ignore
+    @edition_in_progress.setter
     def edition_in_progress(self, val):
-        """Deprecated. Use edit_in_progress instead."""
+        """Deprecated. Use `edit_in_progress` instead."""
         _warn_deprecated("edition_in_progress", suggest="edit_in_progress")
         self.edit_in_progress = val
 
     @property  # type: ignore
     @_self_reload(_MANAGER_NAME)
     def job_ids(self):
-        """List of the jobs having edited the data node."""
+        """List of the jobs having edited this data node."""
         return [edit.get("job_id") for edit in self.edits if edit.get("job_id")]
 
-    @property  # type: ignore
+    @property
     def properties(self):
         """Dictionary of custom properties."""
         r = _reload(self._MANAGER_NAME, self)
         self._properties = r._properties
         return self._properties
 
     def __eq__(self, other):
@@ -281,28 +285,40 @@
         protected_attribute_name = _validate_id(attribute_name)
         if protected_attribute_name in self._properties:
             return self._properties[protected_attribute_name]
         raise AttributeError(f"{attribute_name} is not an attribute of data node {self.id}")
 
     def __get_last_modified_datetime(self) -> Optional[datetime]:
         path = self._properties.get(self.__PATH_KEY, None)
-        if path and os.path.exists(path):
+        if path and os.path.isfile(path):
             return datetime.fromtimestamp(os.path.getmtime(path))
-        return None
+
+        last_modified_datetime = None
+        if path and os.path.isdir(path):
+            for filename in os.listdir(path):
+                filepath = os.path.join(path, filename)
+                if os.path.isfile(filepath):
+                    file_mtime = datetime.fromtimestamp(os.path.getmtime(filepath))
+
+                    if last_modified_datetime is None or file_mtime > last_modified_datetime:
+                        last_modified_datetime = file_mtime
+
+        return last_modified_datetime
 
     @classmethod
     @abstractmethod
     def storage_type(cls) -> str:
         return NotImplementedError  # type: ignore
 
     def read_or_raise(self) -> Any:
         """Read the data referenced by this data node.
 
         Returns:
             The data referenced by this data node.
+
         Raises:
             NoData^: If the data has not been written yet.
         """
         if not self.last_edit_date:
             raise NoData(f"Data node {self.id} from config {self.config_id} has not been written yet.")
         return self._read()
 
@@ -316,21 +332,22 @@
             return self.read_or_raise()
         except NoData:
             self.__logger.warning(
                 f"Data node {self.id} from config {self.config_id} is being read but has never been " f"written."
             )
             return None
 
-    def write(self, data, job_id: Optional[JobId] = None, **kwargs):
+    def write(self, data, job_id: Optional[JobId] = None, **kwargs: Dict[str, Any]):
         """Write some data to this data node.
 
         Parameters:
             data (Any): The data to write to this data node.
             job_id (JobId^): An optional identifier of the writer.
-            **kwargs: Extra information to attach to the edit document corresponding to this write.
+            **kwargs (dict[str, any]): Extra information to attach to the edit document
+                corresponding to this write.
         """
         from ._data_manager_factory import _DataManagerFactory
 
         self._write(data)
         self._track_edit(job_id=job_id, **kwargs)
         self.unlock_edit()
         _DataManagerFactory._build_manager()._set(self)
@@ -351,36 +368,37 @@
 
         Note:
             The data node can be unlocked with the method `(DataNode.)unlock_edit()^`.
         """
         self.edit_in_progress = True
 
     def lock_edition(self):
-        """Deprecated. Use lock_edit instead."""
+        """Deprecated. Use `lock_edit` instead."""
         _warn_deprecated("lock_edition", suggest="lock_edit")
         self.lock_edit()
 
     def unlock_edit(self, at: Optional[datetime] = None, job_id: Optional[JobId] = None):
         """Unlocks the data node modification.
 
         Parameters:
             at (Optional[datetime]): Deprecated.
             job_id (Optional[JobId^]): Deprecated.
+
         Note:
             The data node can be locked with the method `(DataNode.)lock_edit()^`.
         """
         self.edit_in_progress = False  # type: ignore
 
     def unlock_edition(self, at: Optional[datetime] = None, job_id: Optional[JobId] = None):
         """Deprecated. Use `(DataNode.)unlock_edit()^` instead."""
         _warn_deprecated("unlock_edition", suggest="unlock_edit")
         self.unlock_edit()
 
     def filter(self, operators: Union[List, Tuple], join_operator=JoinOperator.AND):
-        """Read the data referenced by the data node, appying a filter.
+        """Read and filter the data referenced by this data node.
 
         The data is filtered by the provided list of 3-tuples (key, value, `Operator^`).
 
         If multiple filter operators are provided, filtered data will be joined based on the
         join operator (_AND_ or _OR_).
 
         Parameters:
@@ -503,20 +521,20 @@
         if not self._last_edit_date:
             # Never been written so it is not up-to-date
             return False
         return True
 
     @property  # type: ignore
     @_self_reload(_MANAGER_NAME)
-    def is_up_to_date(self):
+    def is_up_to_date(self) -> bool:
         """Indicate if this data node is up-to-date.
 
         Returns:
-            False if the data ever been written or the expiration date has passed.
-                True otherwise.
+            False if the data ever been written or the expiration date has passed.<br/>
+            True otherwise.
         """
         if not self._last_edit_date:
             # Never been written so it is not up-to-date
             return False
         if not self._validity_period:
             # No validity period and has already been written, so it is up-to-date
             return True
@@ -530,7 +548,23 @@
         def all_subclasses(cls):
             subclasses = set(cls.__subclasses__())
             for s in cls.__subclasses__():
                 subclasses.update(all_subclasses(s))
             return subclasses
 
         return {c.storage_type(): c for c in all_subclasses(DataNode) if c.storage_type() is not None}
+
+    def get_label(self) -> str:
+        """Returns the data node simple label prefixed by its owner label.
+
+        Returns:
+            The label of the data node as a string.
+        """
+        return self._get_label()
+
+    def get_simple_label(self) -> str:
+        """Returns the data node simple label.
+
+        Returns:
+            The simple label of the data node as a string.
+        """
+        return self._get_simple_label()
```

### Comparing `taipy-core-2.2.3/src/taipy/core/data/excel.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/excel.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,40 +4,38 @@
 # the License. You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
-
+import os
 from collections import defaultdict
 from datetime import datetime, timedelta
 from os.path import isfile
 from typing import Any, Dict, List, Optional, Set, Tuple, Union
 
 import modin.pandas as modin_pd
 import numpy as np
 import pandas as pd
 from openpyxl import load_workbook
 
 from taipy.config.common.scope import Scope
 
+from .._backup._backup import replace_in_backup_file
+from .._entity._reload import _self_reload
 from .._version._version_manager_factory import _VersionManagerFactory
-from ..common._reload import _self_reload
-from ..common.alias import DataNodeId, Edit, JobId
-from ..exceptions.exceptions import (
-    ExposedTypeLengthMismatch,
-    InvalidExposedType,
-    MissingRequiredProperty,
-    NonExistingExcelSheet,
-)
+from ..exceptions.exceptions import ExposedTypeLengthMismatch, InvalidExposedType, NonExistingExcelSheet
+from ..job.job_id import JobId
+from .abstract_file import _AbstractFileDataNode
 from .data_node import DataNode
+from .data_node_id import DataNodeId, Edit
 
 
-class ExcelDataNode(DataNode):
+class ExcelDataNode(DataNode, _AbstractFileDataNode):
     """Data Node stored as an Excel file.
 
     The Excel file format is _xlsx_.
 
     Attributes:
         config_id (str): Identifier of this data node configuration. It must be a valid Python
             identifier.
@@ -70,14 +68,15 @@
     __STORAGE_TYPE = "excel"
     __EXPOSED_TYPE_PROPERTY = "exposed_type"
     __EXPOSED_TYPE_NUMPY = "numpy"
     __EXPOSED_TYPE_PANDAS = "pandas"
     __EXPOSED_TYPE_MODIN = "modin"
     __VALID_STRING_EXPOSED_TYPES = [__EXPOSED_TYPE_PANDAS, __EXPOSED_TYPE_MODIN, __EXPOSED_TYPE_NUMPY]
     __PATH_KEY = "path"
+    __DEFAULT_DATA_KEY = "default_data"
     __DEFAULT_PATH_KEY = "default_path"
     __HAS_HEADER_PROPERTY = "has_header"
     __SHEET_NAME_PROPERTY = "sheet_name"
     _REQUIRED_PROPERTIES: List[str] = []
 
     def __init__(
         self,
@@ -92,24 +91,18 @@
         version: str = None,
         validity_period: Optional[timedelta] = None,
         edit_in_progress: bool = False,
         properties: Dict = None,
     ):
         if properties is None:
             properties = {}
-        if missing := set(self._REQUIRED_PROPERTIES) - set(properties.keys()):
-            raise MissingRequiredProperty(
-                f"The following properties " f"{', '.join(x for x in missing)} were not informed and are required"
-            )
 
+        default_value = properties.pop(self.__DEFAULT_DATA_KEY, None)
         self._path = properties.get(self.__PATH_KEY, properties.get(self.__DEFAULT_PATH_KEY))
-        if self._path is None:
-            raise MissingRequiredProperty("default_path is required in a Excel data node config")
-        else:
-            properties[self.__PATH_KEY] = self._path
+        properties[self.__PATH_KEY] = self._path
 
         if self.__SHEET_NAME_PROPERTY not in properties.keys():
             properties[self.__SHEET_NAME_PROPERTY] = None
         if self.__HAS_HEADER_PROPERTY not in properties.keys():
             properties[self.__HAS_HEADER_PROPERTY] = True
         if self.__EXPOSED_TYPE_PROPERTY not in properties.keys():
             properties[self.__EXPOSED_TYPE_PROPERTY] = self.__EXPOSED_TYPE_PANDAS
@@ -125,27 +118,35 @@
             last_edit_date,
             edits,
             version or _VersionManagerFactory._build_manager()._get_latest_version(),
             validity_period,
             edit_in_progress,
             **properties,
         )
+        if not self._path:
+            self._path = self._build_path(self.storage_type())
+            properties[self.__PATH_KEY] = self._path
+
+        if default_value is not None and not os.path.exists(self._path):
+            self.write(default_value)
 
         if not self._last_edit_date and isfile(self._path):
             self.last_edit_date = datetime.now()  # type: ignore
 
     @property  # type: ignore
     @_self_reload(DataNode._MANAGER_NAME)
     def path(self):
         return self._path
 
     @path.setter
     def path(self, value):
+        tmp_old_path = self._path
         self._path = value
         self.properties[self.__PATH_KEY] = value
+        replace_in_backup_file(old_file_path=tmp_old_path, new_file_path=self._path)
 
     @classmethod
     def storage_type(cls) -> str:
         return cls.__STORAGE_TYPE
 
     def _check_exposed_type(self, exposed_type):
         if isinstance(exposed_type, str) and exposed_type not in self.__VALID_STRING_EXPOSED_TYPES:
@@ -233,64 +234,58 @@
 
     def _read_as_numpy(self):
         sheets = self._read_as_pandas_dataframe()
         if isinstance(sheets, dict):
             return {sheet_name: df.to_numpy() for sheet_name, df in sheets.items()}
         return sheets.to_numpy()
 
-    def _read_as_pandas_dataframe(self, sheet_names=None) -> Union[Dict[Union[int, str], pd.DataFrame], pd.DataFrame]:
-        if sheet_names is None:
-            sheet_names = self.properties[self.__SHEET_NAME_PROPERTY]
-        try:
-            kwargs: Dict[str, Any] = {}
-            if not self.properties[self.__HAS_HEADER_PROPERTY]:
-                kwargs["header"] = None
-            df = pd.read_excel(
-                self._path,
-                sheet_name=sheet_names,
-                **kwargs,
-            )
-            if isinstance(df, dict):
+    def _do_read_excel(self, engine, sheet_names, kwargs) -> pd.DataFrame:
+        df = pd.read_excel(
+            self._path,
+            sheet_name=sheet_names,
+            **kwargs,
+        )
+        # We are using pandas to load modin dataframes because of a modin issue
+        # https://github.com/modin-project/modin/issues/4924
+        if engine == "modin":
+            if isinstance(df, dict):  # Check if it s a multiple sheet Excel file
                 for key, value in df.items():
-                    df[key] = pd.DataFrame(value)
+                    df[key] = modin_pd.DataFrame(value)
                 return df
+            return modin_pd.DataFrame(df)
+        return df
 
-            return pd.DataFrame(df)
+    def __get_sheet_names_and_header(self, sheet_names):
+        kwargs: Dict[str, Any] = {}
+        if sheet_names is None:
+            sheet_names = self.properties[self.__SHEET_NAME_PROPERTY]
+        if not self.properties[self.__HAS_HEADER_PROPERTY]:
+            kwargs["header"] = None
+        return sheet_names, kwargs
 
+    def _read_as_pandas_dataframe(self, sheet_names=None) -> Union[Dict[Union[int, str], pd.DataFrame], pd.DataFrame]:
+        sheet_names, kwargs = self.__get_sheet_names_and_header(sheet_names)
+        try:
+            return self._do_read_excel("pandas", sheet_names, kwargs)
         except pd.errors.EmptyDataError:
             return pd.DataFrame()
 
     def _read_as_modin_dataframe(
         self, sheet_names=None
     ) -> Union[Dict[Union[int, str], modin_pd.DataFrame], modin_pd.DataFrame]:
-        if sheet_names is None:
-            sheet_names = self.properties[self.__SHEET_NAME_PROPERTY]
+        sheet_names, kwargs = self.__get_sheet_names_and_header(sheet_names)
         try:
-            kwargs: Dict[str, Any] = {}
-            if not self.properties[self.__HAS_HEADER_PROPERTY]:
-                kwargs["header"] = None
             if kwargs.get("header", None):
                 return modin_pd.read_excel(
                     self._path,
                     sheet_name=sheet_names,
                     **kwargs,
                 )
             else:
-                df = pd.read_excel(
-                    self._path,
-                    sheet_name=sheet_names,
-                    **kwargs,
-                )
-                if isinstance(df, dict):
-                    for key, value in df.items():
-                        df[key] = modin_pd.DataFrame(value)
-                    return df
-
-            return modin_pd.DataFrame(df)
-
+                return self._do_read_excel("modin", sheet_names, kwargs)
         except pd.errors.EmptyDataError:
             return modin_pd.DataFrame()
 
     def _write(self, data: Any):
         if isinstance(data, Dict) and all(
             [isinstance(x, (pd.DataFrame, modin_pd.DataFrame, np.ndarray)) for x in data.values()]
         ):
```

### Comparing `taipy-core-2.2.3/src/taipy/core/data/generic.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/generic.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 from datetime import datetime, timedelta
 from typing import Any, Dict, List, Optional, Set
 
 from taipy.config.common.scope import Scope
 
 from .._version._version_manager_factory import _VersionManagerFactory
-from ..common.alias import DataNodeId, Edit
 from ..exceptions.exceptions import MissingReadFunction, MissingRequiredProperty, MissingWriteFunction
 from .data_node import DataNode
+from .data_node_id import DataNodeId, Edit
 
 
 class GenericDataNode(DataNode):
     """Generic Data Node that uses custom read and write functions.
 
     The read and write function for this data node type can be implemented is Python.
 
@@ -40,26 +40,27 @@
             the current version is used.
         validity_period (Optional[timedelta]): The validity period of a data node.
             Implemented as a timedelta. If _validity_period_ is set to None, the data node is
             always up-to-date.
         edit_in_progress (bool): True if a task computing the data node has been submitted
             and not completed yet. False otherwise.
         properties (dict[str, Any]): A dictionary of additional properties. Note that the
-            _properties_ parameter must at least contain an entry for _"read_fct"_ or
+            _properties_ parameter must at least contain an entry for either _"read_fct"_ or
             _"write_fct"_ representing the read and write functions.
-            Entries for _"read_fct_params"_ and _"write_fct_params"_ respectively represent
+            Entries for _"read_fct_args"_ and _"write_fct_args"_ respectively represent
             potential parameters for the _"read_fct"_ and _"write_fct"_ functions.
     """
 
     __STORAGE_TYPE = "generic"
-    _REQUIRED_READ_FUNCTION_PROPERTY = "read_fct"
-    _READ_FUNCTION_PARAMS_PROPERTY = "read_fct_params"
-    _REQUIRED_WRITE_FUNCTION_PROPERTY = "write_fct"
-    _WRITE_FUNCTION_PARAMS_PROPERTY = "write_fct_params"
-    _REQUIRED_PROPERTIES: List[str] = [_REQUIRED_READ_FUNCTION_PROPERTY, _REQUIRED_WRITE_FUNCTION_PROPERTY]
+    _OPTIONAL_READ_FUNCTION_PROPERTY = "read_fct"
+    _READ_FUNCTION_ARGS_PROPERTY = "read_fct_args"
+    _OPTIONAL_WRITE_FUNCTION_PROPERTY = "write_fct"
+    _WRITE_FUNCTION_ARGS_PROPERTY = "write_fct_args"
+    _REQUIRED_PROPERTIES: List[str] = []
+    _REQUIRED_AT_LEAST_ONE_PROPERTY: List[str] = [_OPTIONAL_READ_FUNCTION_PROPERTY, _OPTIONAL_WRITE_FUNCTION_PROPERTY]
 
     def __init__(
         self,
         config_id: str,
         scope: Scope,
         id: Optional[DataNodeId] = None,
         name: Optional[str] = None,
@@ -72,17 +73,26 @@
         edit_in_progress: bool = False,
         properties: Dict = None,
     ):
         if properties is None:
             properties = {}
         if missing := set(self._REQUIRED_PROPERTIES) - set(properties.keys()):
             raise MissingRequiredProperty(
-                f"The following properties " f"{', '.join(x for x in missing)} were not informed and are required"
+                f"The following properties " f"{', '.join(x for x in missing)} were not informed and are required."
             )
 
+        missing_optional_fcts = set(self._REQUIRED_AT_LEAST_ONE_PROPERTY) - set(properties.keys())
+        if len(missing_optional_fcts) == len(self._REQUIRED_AT_LEAST_ONE_PROPERTY):
+            raise MissingRequiredProperty(
+                f"None of the following properties "
+                f"{', '.join(x for x in missing)} were informed and at least one must be populated."
+            )
+        for missing_optional_fct in missing_optional_fcts:
+            properties[missing_optional_fct] = None
+
         super().__init__(
             config_id,
             scope,
             id,
             name,
             owner_id,
             parent_ids,
@@ -97,19 +107,23 @@
             self.last_edit_date = datetime.now()  # type: ignore
 
     @classmethod
     def storage_type(cls) -> str:
         return cls.__STORAGE_TYPE
 
     def _read(self):
-        if read_fct := self.properties[self._REQUIRED_READ_FUNCTION_PROPERTY]:
-            if self._READ_FUNCTION_PARAMS_PROPERTY in self.properties.keys():
-                return read_fct(*self.properties[self._READ_FUNCTION_PARAMS_PROPERTY])
+        if read_fct := self.properties[self._OPTIONAL_READ_FUNCTION_PROPERTY]:
+            if read_fct_args := self.properties.get(self._READ_FUNCTION_ARGS_PROPERTY, None):
+                if not isinstance(read_fct_args, list):
+                    return read_fct(*[read_fct_args])
+                return read_fct(*read_fct_args)
             return read_fct()
         raise MissingReadFunction(f"The read function is not defined in data node config {self.config_id}.")
 
     def _write(self, data: Any):
-        if write_fct := self.properties[self._REQUIRED_WRITE_FUNCTION_PROPERTY]:
-            if self._WRITE_FUNCTION_PARAMS_PROPERTY in self.properties.keys():
-                return write_fct(data, *self.properties[self._WRITE_FUNCTION_PARAMS_PROPERTY])
+        if write_fct := self.properties[self._OPTIONAL_WRITE_FUNCTION_PROPERTY]:
+            if write_fct_args := self.properties.get(self._WRITE_FUNCTION_ARGS_PROPERTY, None):
+                if not isinstance(write_fct_args, list):
+                    return write_fct(data, *[write_fct_args])
+                return write_fct(data, *write_fct_args)
             return write_fct(data)
         raise MissingWriteFunction(f"The write function is not defined in data node config {self.config_id}.")
```

### Comparing `taipy-core-2.2.3/src/taipy/core/data/in_memory.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/in_memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 from datetime import datetime, timedelta
 from typing import Any, Dict, List, Optional, Set
 
 from taipy.config.common.scope import Scope
 
 from .._version._version_manager_factory import _VersionManagerFactory
-from ..common.alias import DataNodeId, Edit
 from .data_node import DataNode
+from .data_node_id import DataNodeId, Edit
 
 in_memory_storage: Dict[str, Any] = {}
 
 
 class InMemoryDataNode(DataNode):
     """Data Node stored in memory.
```

### Comparing `taipy-core-2.2.3/src/taipy/core/data/json.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/json.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,30 +7,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import dataclasses
 import json
+import os
 from datetime import date, datetime, timedelta
 from enum import Enum
 from os.path import isfile
 from pydoc import locate
 from typing import Any, Dict, List, Optional, Set
 
 from taipy.config.common.scope import Scope
 
+from .._backup._backup import replace_in_backup_file
+from .._entity._reload import _self_reload
 from .._version._version_manager_factory import _VersionManagerFactory
-from ..common._reload import _self_reload
-from ..common.alias import DataNodeId, Edit
-from ..exceptions.exceptions import MissingRequiredProperty
+from .abstract_file import _AbstractFileDataNode
 from .data_node import DataNode
+from .data_node_id import DataNodeId, Edit
 
 
-class JSONDataNode(DataNode):
+class JSONDataNode(DataNode, _AbstractFileDataNode):
     """Data Node stored as a JSON file.
 
     Attributes:
         config_id (str): Identifier of the data node configuration. This string must be a valid
             Python identifier.
         scope (Scope^): The scope of this data node.
         id (str): The unique identifier of this data node.
@@ -50,14 +52,15 @@
         encoder (json.JSONEncoder): The JSON encoder that is used to write into the JSON file.
         decoder (json.JSONDecoder): The JSON decoder that is used to read from the JSON file.
         properties (dict[str, Any]): A dictionary of additional properties. The _properties_
             must have a _"default_path"_ or _"path"_ entry with the path of the JSON file.
     """
 
     __STORAGE_TYPE = "json"
+    __DEFAULT_DATA_KEY = "default_data"
     __DEFAULT_PATH_KEY = "default_path"
     __PATH_KEY = "path"
     _ENCODER_KEY = "encoder"
     _DECODER_KEY = "decoder"
     _REQUIRED_PROPERTIES: List[str] = []
 
     def __init__(
@@ -73,24 +76,16 @@
         version: str = None,
         validity_period: Optional[timedelta] = None,
         edit_in_progress: bool = False,
         properties: Dict = None,
     ):
         if properties is None:
             properties = {}
-        if missing := set(self._REQUIRED_PROPERTIES) - set(properties.keys()):
-            raise MissingRequiredProperty(
-                f"The following properties " f"{', '.join(x for x in missing)} were not informed and are required"
-            )
 
-        self._path = properties.get(self.__PATH_KEY, properties.get(self.__DEFAULT_PATH_KEY))
-        if self._path is None:
-            raise MissingRequiredProperty("default_path is required in a JSON data node config")
-        else:
-            properties[self.__PATH_KEY] = self._path
+        default_value = properties.pop(self.__DEFAULT_DATA_KEY, None)
 
         super().__init__(
             config_id,
             scope,
             id,
             name,
             owner_id,
@@ -98,33 +93,43 @@
             last_edit_date,
             edits,
             version or _VersionManagerFactory._build_manager()._get_latest_version(),
             validity_period,
             edit_in_progress,
             **properties,
         )
+        self._path = properties.get(self.__PATH_KEY, properties.get(self.__DEFAULT_PATH_KEY))
+        if not self._path:
+            self._path = self._build_path(self.storage_type())
+        properties[self.__PATH_KEY] = self._path
+
         self._decoder = self._properties.get(self._DECODER_KEY, _DefaultJSONDecoder)
         self._encoder = self._properties.get(self._ENCODER_KEY, _DefaultJSONEncoder)
 
+        if default_value is not None and not os.path.exists(self._path):
+            self.write(default_value)
+
         if not self._last_edit_date and isfile(self._path):  # type: ignore
             self.last_edit_date = datetime.now()  # type: ignore
 
     @classmethod
     def storage_type(cls) -> str:
         return cls.__STORAGE_TYPE
 
     @property  # type: ignore
     @_self_reload(DataNode._MANAGER_NAME)
     def path(self):
         return self._path
 
     @path.setter
     def path(self, value):
+        tmp_old_path = self._path
         self._path = value
         self.properties[self.__PATH_KEY] = value
+        replace_in_backup_file(old_file_path=tmp_old_path, new_file_path=self._path)
 
     @property  # type: ignore
     @_self_reload(DataNode._MANAGER_NAME)
     def encoder(self):
         return self._encoder
 
     @encoder.setter
```

### Comparing `taipy-core-2.2.3/src/taipy/core/data/mongo.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/mongo.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from typing import Any, Dict, List, Optional, Set
 
 import pymongo
 
 from taipy.config.common.scope import Scope
 
 from .._version._version_manager_factory import _VersionManagerFactory
-from ..common.alias import DataNodeId, Edit
 from ..exceptions.exceptions import InvalidCustomDocument, MissingRequiredProperty
 from .data_node import DataNode
+from .data_node_id import DataNodeId, Edit
 
 
 class MongoCollectionDataNode(DataNode):
     """Data Node stored in a Mongo collection.
 
     Attributes:
         config_id (str): Identifier of the data node configuration. It must be a valid Python
```

### Comparing `taipy-core-2.2.3/src/taipy/core/data/operator.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/operator.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/data/parquet.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/parquet.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,36 +5,35 @@
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
+import os
 from datetime import datetime, timedelta
-from os.path import isfile
+from os.path import isdir, isfile
 from typing import Any, Dict, List, Optional, Set
 
 import modin.pandas as modin_pd
 import pandas as pd
 
 from taipy.config.common.scope import Scope
 
+from .._backup._backup import replace_in_backup_file
+from .._entity._reload import _self_reload
 from .._version._version_manager_factory import _VersionManagerFactory
-from ..common._reload import _self_reload
-from ..common.alias import DataNodeId, Edit, JobId
-from ..exceptions.exceptions import (
-    InvalidExposedType,
-    MissingRequiredProperty,
-    UnknownCompressionAlgorithm,
-    UnknownParquetEngine,
-)
+from ..exceptions.exceptions import InvalidExposedType, UnknownCompressionAlgorithm, UnknownParquetEngine
+from ..job.job_id import JobId
+from .abstract_file import _AbstractFileDataNode
 from .data_node import DataNode
+from .data_node_id import DataNodeId, Edit
 
 
-class ParquetDataNode(DataNode):
+class ParquetDataNode(DataNode, _AbstractFileDataNode):
     """Data Node stored as a Parquet file.
 
     Attributes:
         config_id (str): Identifier of the data node configuration. This string must be a valid
             Python identifier.
         scope (Scope^): The scope of this data node.
         id (str): The unique identifier of this data node.
@@ -42,83 +41,89 @@
         owner_id (str): The identifier of the owner (pipeline_id, scenario_id, cycle_id) or `None`.
         parent_ids (Optional[Set[str]]): The identifiers of the parent tasks or `None`.
         last_edit_date (datetime): The date and time of the last modification.
         edits (List[Edit^]): The ordered list of edits for that job.
         version (str): The string indicates the application version of the data node to instantiate. If not provided,
             the current version is used.
         validity_period (Optional[timedelta]): The validity period of a data node.
-            Implemented as a timedelta. If _validity_period_ is set to None, the data_node is
+            Implemented as a timedelta. If *validity_period* is set to None, the data_node is
             always up-to-date.
         edit_in_progress (bool): True if a task computing the data node has been submitted
             and not completed yet. False otherwise.
         path (str): The path to the Parquet file.
-        properties (dict[str, Any]): A dictionary of additional properties. The _properties_
-            must have a _"default_path"_ or _"path"_ entry with the path of the Parquet file:
+        properties (dict[str, Any]): A dictionary of additional properties. *properties*
+            must have a *"default_path"* or *"path"* entry with the path of the Parquet file:
 
-            - _"default_path"_ `(str)`: The default path of the Parquet file.\n
-            - _"exposed_type"_: The exposed type of the data read from Parquet file. The default value is `pandas`.\n
-            - _"engine"_ `(Optional[str])`: Parquet library to use. Possible values are _"fastparquet"_ or _"pyarrow"_.
-                The default value is _"pyarrow"_.
-            - _"compression"_ `(Optional[str])`: Name of the compression to use. Use None for no compression.
-                `{'snappy', 'gzip', 'brotli', None}`, default `'snappy'`.\n
-            - _"read_kwargs"_ `(Optional[Dict])`: Additional parameters passed to the _pandas.read_parquet_ method.\n
-            - _"write_kwargs"_ `(Optional[Dict])`: Additional parameters passed to the _pandas.DataFrame.write_parquet_
-                method.
-                The parameters in _"read_kwargs"_ and _"write_kwargs"_ have a **higher precedence** than the top-level
-                parameters which are also passed to Pandas.\n
+            - *"default_path"* (`str`): The default path of the Parquet file.
+            - *"exposed_type"*: The exposed type of the data read from Parquet file. The default
+                value is `pandas`.
+            - *"engine"* (`Optional[str]`): Parquet library to use. Possible values are
+                *"fastparquet"* or *"pyarrow"*.<br/>
+                The default value is *"pyarrow"*.
+            - *"compression"* (`Optional[str]`): Name of the compression to use. Possible values
+                are *"snappy"*, *"gzip"*, *"brotli"*, or *"none"* (no compression).<br/>
+                The default value is *"snappy"*.
+            - *"read_kwargs"* (`Optional[dict]`): Additional parameters passed to the
+                *pandas.read_parquet()* function.
+            - *"write_kwargs"* (`Optional[dict]`): Additional parameters passed to the
+                *pandas.DataFrame.write_parquet()* fucntion.
+                The parameters in *"read_kwargs"* and *"write_kwargs"* have a
+                **higher precedence** than the top-level parameters which are also passed to
+                Pandas.
     """
 
     __STORAGE_TYPE = "parquet"
     __EXPOSED_TYPE_PROPERTY = "exposed_type"
     __EXPOSED_TYPE_NUMPY = "numpy"
     __EXPOSED_TYPE_PANDAS = "pandas"
     __EXPOSED_TYPE_MODIN = "modin"
     __VALID_STRING_EXPOSED_TYPES = [__EXPOSED_TYPE_PANDAS, __EXPOSED_TYPE_MODIN, __EXPOSED_TYPE_NUMPY]
     __PATH_KEY = "path"
+    __DEFAULT_DATA_KEY = "default_data"
     __DEFAULT_PATH_KEY = "default_path"
     __ENGINE_PROPERTY = "engine"
     __VALID_PARQUET_ENGINES = ["pyarrow", "fastparquet"]
     __COMPRESSION_PROPERTY = "compression"
-    __VALID_COMPRESSION_ALGORITHMS = ["snappy", "gzip", "brotli"]
+    __VALID_COMPRESSION_ALGORITHMS = ["snappy", "gzip", "brotli", "none"]
     __READ_KWARGS_PROPERTY = "read_kwargs"
     __WRITE_KWARGS_PROPERTY = "write_kwargs"
     _REQUIRED_PROPERTIES: List[str] = []
 
     def __init__(
         self,
         config_id: str,
         scope: Scope,
         id: Optional[DataNodeId] = None,
         name: Optional[str] = None,
         owner_id: Optional[str] = None,
         parent_ids: Optional[Set[str]] = None,
         last_edit_date: Optional[datetime] = None,
-        edits: List[Edit] = None,
-        version: str = None,
+        edits: Optional[List[Edit]] = None,
+        version: Optional[str] = None,
         validity_period: Optional[timedelta] = None,
         edit_in_progress: bool = False,
-        properties: Dict = None,
+        properties: Optional[Dict] = None,
     ):
         if properties is None:
             properties = {}
-        if missing := set(self._REQUIRED_PROPERTIES) - set(properties.keys()):
-            raise MissingRequiredProperty(
-                f"The following properties " f"{', '.join(x for x in missing)} were not informed and are required"
-            )
+
+        default_value = properties.pop(self.__DEFAULT_DATA_KEY, None)
 
         if self.__ENGINE_PROPERTY not in properties.keys():
             properties[self.__ENGINE_PROPERTY] = "pyarrow"
         if properties[self.__ENGINE_PROPERTY] not in self.__VALID_PARQUET_ENGINES:
             raise UnknownParquetEngine(
                 f"Invalid parquet engine: {properties[self.__ENGINE_PROPERTY]}. "
                 f"Supported engines are {', '.join(self.__VALID_PARQUET_ENGINES)}"
             )
 
         if self.__COMPRESSION_PROPERTY not in properties.keys():
             properties[self.__COMPRESSION_PROPERTY] = "snappy"
+        if properties[self.__COMPRESSION_PROPERTY] == "none":
+            properties[self.__COMPRESSION_PROPERTY] = None
         if (
             properties[self.__COMPRESSION_PROPERTY]
             and properties[self.__COMPRESSION_PROPERTY] not in self.__VALID_COMPRESSION_ALGORITHMS
         ):
             raise UnknownCompressionAlgorithm(
                 f"Unsupported compression algorithm: {properties[self.__COMPRESSION_PROPERTY]}. "
                 f"Supported algorithms are {', '.join(self.__VALID_COMPRESSION_ALGORITHMS)}"
@@ -126,20 +131,14 @@
 
         if self.__READ_KWARGS_PROPERTY not in properties.keys():
             properties[self.__READ_KWARGS_PROPERTY] = {}
 
         if self.__WRITE_KWARGS_PROPERTY not in properties.keys():
             properties[self.__WRITE_KWARGS_PROPERTY] = {}
 
-        self._path = properties.get(self.__PATH_KEY, properties.get(self.__DEFAULT_PATH_KEY))
-        if self._path is None:
-            raise MissingRequiredProperty("default_path is required in a Parquet data node config")
-        else:
-            properties[self.__PATH_KEY] = self._path
-
         if self.__EXPOSED_TYPE_PROPERTY not in properties.keys():
             properties[self.__EXPOSED_TYPE_PROPERTY] = self.__EXPOSED_TYPE_PANDAS
         self._check_exposed_type(properties[self.__EXPOSED_TYPE_PROPERTY])
 
         super().__init__(
             config_id,
             scope,
@@ -150,30 +149,40 @@
             last_edit_date,
             edits,
             version or _VersionManagerFactory._build_manager()._get_latest_version(),
             validity_period,
             edit_in_progress,
             **properties,
         )
-        if not self._last_edit_date and isfile(self._path):
+        self._path = properties.get(self.__PATH_KEY, properties.get(self.__DEFAULT_PATH_KEY))
+        if not self._path:
+            self._path = self._build_path(self.storage_type())
+        properties[self.__PATH_KEY] = self._path
+
+        if default_value is not None and not os.path.exists(self._path):
+            self.write(default_value)
+
+        if not self._last_edit_date and (isfile(self._path) or isdir(self._path)):
             self.last_edit_date = datetime.now()  # type: ignore
 
     @classmethod
     def storage_type(cls) -> str:
         return cls.__STORAGE_TYPE
 
     @property  # type: ignore
     @_self_reload(DataNode._MANAGER_NAME)
     def path(self):
         return self._path
 
     @path.setter
     def path(self, value):
+        tmp_old_path = self._path
         self._path = value
         self.properties[self.__PATH_KEY] = value
+        replace_in_backup_file(old_file_path=tmp_old_path, new_file_path=self._path)
 
     def _check_exposed_type(self, exposed_type):
         if isinstance(exposed_type, str) and exposed_type not in self.__VALID_STRING_EXPOSED_TYPES:
             raise InvalidExposedType(
                 f"Invalid string exposed type {exposed_type}. Supported values are "
                 f"{', '.join(self.__VALID_STRING_EXPOSED_TYPES)}"
             )
@@ -195,45 +204,45 @@
     def _read_as_modin_dataframe(self, read_kwargs: Dict) -> modin_pd.DataFrame:
         return modin_pd.read_parquet(self._path, **read_kwargs)
 
     def _write(self, data: Any):
         self.write_with_kwargs(data)
 
     def write_with_kwargs(self, data: Any, job_id: Optional[JobId] = None, **write_kwargs):
-        """Write data, with keyword arguments passed to `pandas.DataFrame.to_parquet`.
+        """Write the data referenced by this data node.
 
         Keyword arguments here which are also present in the Data Node config will overwrite them.
 
         Parameters:
             data (Any): The data to write.
             job_id (JobId^): An optional identifier of the writer.
-            **write_kwargs: The keyword arguments are passed to `pandas.DataFrame.to_parquet`.
+            **write_kwargs (dict[str, any]): The keyword arguments passed to the function
+                `pandas.DataFrame.to_parquet()`.
         """
-
         kwargs = {
             self.__ENGINE_PROPERTY: self.properties[self.__ENGINE_PROPERTY],
             self.__COMPRESSION_PROPERTY: self.properties[self.__COMPRESSION_PROPERTY],
         }
         kwargs.update(self.properties[self.__WRITE_KWARGS_PROPERTY])
         kwargs.update(write_kwargs)
         if isinstance(data, (pd.DataFrame, modin_pd.DataFrame)):
             data.to_parquet(self._path, **kwargs)
         else:
             pd.DataFrame(data).to_parquet(self._path, **kwargs)
         self._track_edit(timestamp=datetime.now(), job_id=job_id)
 
     def read_with_kwargs(self, **read_kwargs):
-        """Read data node, with keyword arguments passed to `pandas.read_parquet`.
+        """Read data from this data node.
 
         Keyword arguments here which are also present in the Data Node config will overwrite them.
 
         Parameters:
-            **read_kwargs: The keyword arguments are passed to `pandas.read_parquet`.
+            **read_kwargs (dict[str, any]): The keyword arguments passed to the function
+                `pandas.read_parquet()`.
         """
-
         # return None if data was never written
         if not self.last_edit_date:
             self._DataNode__logger.warning(
                 f"Data node {self.id} from config {self.config_id} is being read but has never been written."
             )
             return None
```

### Comparing `taipy-core-2.2.3/src/taipy/core/data/pickle.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/pickle.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,30 +6,31 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import os
-import pathlib
 import pickle
 from datetime import datetime, timedelta
 from typing import Any, List, Optional, Set
 
 import modin.pandas as pd
 
 from taipy.config.common.scope import Scope
 
+from .._backup._backup import replace_in_backup_file
+from .._entity._reload import _self_reload
 from .._version._version_manager_factory import _VersionManagerFactory
-from ..common._reload import _self_reload
-from ..common.alias import DataNodeId, Edit
+from .abstract_file import _AbstractFileDataNode
 from .data_node import DataNode
+from .data_node_id import DataNodeId, Edit
 
 
-class PickleDataNode(DataNode):
+class PickleDataNode(DataNode, _AbstractFileDataNode):
     """Data Node stored as a pickle file.
 
     Attributes:
         config_id (str): Identifier of the data node configuration. It must be a valid Python
             identifer.
         scope (Scope^): The scope of this data node.
         id (str): The unique identifier of this data node.
@@ -95,15 +96,15 @@
             edits,
             version or _VersionManagerFactory._build_manager()._get_latest_version(),
             validity_period,
             edit_in_progress,
             **properties,
         )
         if self._path is None:
-            self._path = self.__build_path()
+            self._path = self._build_path(self.storage_type())
         if not self._last_edit_date and os.path.exists(self._path):
             self.last_edit_date = datetime.now()  # type: ignore
         if default_value is not None and not os.path.exists(self._path):
             self.write(default_value)
 
     @classmethod
     def storage_type(cls) -> str:
@@ -112,17 +113,19 @@
     @property  # type: ignore
     @_self_reload(DataNode._MANAGER_NAME)
     def path(self) -> Any:
         return self._path
 
     @path.setter  # type: ignore
     def path(self, value):
+        tmp_old_path = self._path
         self._path = value
         self.properties[self.__PATH_KEY] = value
         self.properties[self.__IS_GENERATED_KEY] = False
+        replace_in_backup_file(old_file_path=tmp_old_path, new_file_path=self._path)
 
     @property  # type: ignore
     @_self_reload(DataNode._MANAGER_NAME)
     def is_generated(self) -> bool:
         return self._is_generated
 
     def _read(self):
@@ -131,15 +134,7 @@
             return pickle.load(pf)
 
     def _write(self, data):
         if isinstance(data, (pd.DataFrame, pd.Series)):
             os.environ["MODIN_PERSISTENT_PICKLE"] = "True"
         with open(self._path, "wb") as pf:
             pickle.dump(data, pf)
-
-    def __build_path(self):
-        from taipy.config.config import Config
-
-        dir_path = pathlib.Path(Config.global_config.storage_folder) / "pickles"
-        if not dir_path.exists():
-            dir_path.mkdir(parents=True, exist_ok=True)
-        return dir_path / f"{self.id}.p"
```

### Comparing `taipy-core-2.2.3/src/taipy/core/data/sql.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/sql.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 from datetime import datetime, timedelta
 from typing import Dict, List, Optional, Set
 
 from taipy.config.common.scope import Scope
 
 from .._version._version_manager_factory import _VersionManagerFactory
-from ..common.alias import DataNodeId, Edit
 from ..exceptions.exceptions import MissingRequiredProperty
 from .abstract_sql import _AbstractSQLDataNode
+from .data_node_id import DataNodeId, Edit
 
 
 class SQLDataNode(_AbstractSQLDataNode):
     """Data Node stored in a SQL database.
 
     Attributes:
         config_id (str): Identifier of the data node configuration. It must be a valid Python
@@ -38,30 +38,33 @@
             the current version is used.
         validity_period (Optional[timedelta]): The validity period of a data node.
             Implemented as a timedelta. If _validity_period_ is set to None, the data_node is
             always up-to-date.
         edit_in_progress (bool): True if a task computing the data node has been submitted
             and not completed yet. False otherwise.
         properties (dict[str, Any]): A dictionary of additional properties. Note that the
-            _properties_ parameter must at least contain an entry for _"db_username"_,
-            _"db_password"_, _"db_name"_, _"db_engine"_, _"read_query"_, and _"write_query_builder"_:
+            _properties_ parameter must at least contain an entry for _"db_name"_, _"db_engine"_, _"read_query"_,
+            and _"write_query_builder"_:
 
-            - _"db_username"_ `(str)`: The database username.
-            - _"db_password"_ `(str)`: The database password.
             - _"db_name"_ `(str)`: The database name, or the name of the SQLite database file.
             - _"db_engine"_ `(str)`: The database engine. Possible values are _"sqlite"_, _"mssql"_, _"mysql"_, or
                 _"postgresql"_.
-            - _"db_port"_ `(int)`: The database port. The default value is 1433.
+            - _"read_query"_ `(str)`: The SQL query string used to read the data from the database.
+            - _"write_query_builder"_ `(Callable)`: A callback function that takes the data as an input parameter and
+                returns a list of SQL queries.
+            - _"db_username"_ `(str)`: The database username.
+            - _"db_password"_ `(str)`: The database password.
             - _"db_host"_ `(str)`: The database host. The default value is _"localhost"_.
+            - _"db_port"_ `(int)`: The database port. The default value is 1433.
             - _"db_driver"_ `(str)`: The database driver.
+            - _"sqlite_folder_path"_ (str): The path to the folder that contains SQLite file. The default value
+                is the current working folder.
+            - _"sqlite_file_extension"_ (str): The filename extension of the SQLite file. The default value is ".db".
             - _"db_extra_args"_ `(Dict[str, Any])`: A dictionary of additional arguments to be passed into database
                 connection string.
-            - _"read_query"_ `(str)`: The SQL query string used to read the data from the database.
-            - _"write_query_builder"_ `(Callable)`: A callback function that takes the data as an input parameter and
-                returns a list of SQL queries.
             - _"exposed_type"_: The exposed type of the data read from SQL query. The default value is `pandas`.
     """
 
     __STORAGE_TYPE = "sql"
     __READ_QUERY_KEY = "read_query"
     _WRITE_QUERY_BUILDER_KEY = "write_query_builder"
```

### Comparing `taipy-core-2.2.3/src/taipy/core/data/sql_table.py` & `taipy-core-2.3.0.dev0/src/taipy/core/data/sql_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 import numpy as np
 import pandas as pd
 from sqlalchemy import MetaData, Table
 
 from taipy.config.common.scope import Scope
 
 from .._version._version_manager_factory import _VersionManagerFactory
-from ..common.alias import DataNodeId, Edit
 from ..exceptions.exceptions import MissingRequiredProperty
 from .abstract_sql import _AbstractSQLDataNode
+from .data_node_id import DataNodeId, Edit
 
 
 class SQLTableDataNode(_AbstractSQLDataNode):
     """Data Node stored in a SQL table.
 
     Attributes:
         config_id (str): Identifier of the data node configuration. It must be a valid Python
@@ -43,28 +43,30 @@
             the current version is used.
         validity_period (Optional[timedelta]): The validity period of a data node.
             Implemented as a timedelta. If _validity_period_ is set to None, the data_node is
             always up-to-date.
         edit_in_progress (bool): True if a task computing the data node has been submitted
             and not completed yet. False otherwise.
         properties (dict[str, Any]): A dictionary of additional properties. Note that the
-            _properties_ parameter must at least contain an entry for _"db_username"_,
-            _"db_password"_, _"db_name"_, _"db_engine"_, _"table_name"_:
+            _properties_ parameter must at least contain an entry for _"db_name"_, _"db_engine"_, _"table_name"_:
 
-            - _"db_username"_ `(str)`: The database username.
-            - _"db_password"_ `(str)`: The database password.
             - _"db_name"_ `(str)`: The database name, or the name of the SQLite database file.
-            - _"db_host"_ `(str)`: The database host. The default value is _"localhost"_.
             - _"db_engine"_ `(str)`: The database engine. For now, the accepted values are _"sqlite"_, _"mssql"_,
                 _"mysql"_, or _"postgresql"_.
-            - _"db_driver"_ `(str)`: The database driver.
+            - _"table_name"_ `(str)`: The name of the SQL table.
+            - _"db_username"_ `(str)`: The database username.
+            - _"db_password"_ `(str)`: The database password.
+            - _"db_host"_ `(str)`: The database host. The default value is _"localhost"_.
             - _"db_port"_ `(int)`: The database port. The default value is 1433.
+            - _"db_driver"_ `(str)`: The database driver.
+            - _"sqlite_folder_path"_ (str): The path to the folder that contains SQLite file. The default value
+                is the current working folder.
+            - _"sqlite_file_extension"_ (str): The filename extension of the SQLite file. The default value is ".db".
             - _"db_extra_args"_ `(Dict[str, Any])`: A dictionary of additional arguments to be passed into database
                 connection string.
-            - _"table_name"_ `(str)`: The name of the SQL table.
             - _"exposed_type"_: The exposed type of the data read from SQL query. The default value is `pandas`.
     """
 
     __STORAGE_TYPE = "sql_table"
     __TABLE_KEY = "table_name"
 
     def __init__(
```

### Comparing `taipy-core-2.2.3/src/taipy/core/exceptions/__init__.py` & `taipy-core-2.3.0.dev0/src/taipy/core/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/job/__init__.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_version/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/job/_job_fs_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/job/_job_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/job/_job_manager.py` & `taipy-core-2.3.0.dev0/src/taipy/core/job/_job_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,59 +10,61 @@
 # specific language governing permissions and limitations under the License.
 
 import uuid
 from typing import Callable, Iterable, Optional, Union
 
 from .._manager._manager import _Manager
 from .._version._version_manager_factory import _VersionManagerFactory
-from ..common.alias import JobId
 from ..exceptions.exceptions import JobNotDeletedException
+from ..notification import EventEntityType, EventOperation, _publish_event
 from ..task.task import Task
 from ._job_repository_factory import _JobRepositoryFactory
 from .job import Job
+from .job_id import JobId
 
 
 class _JobManager(_Manager[Job]):
-    _repository = _JobRepositoryFactory._build_repository()  # type: ignore
+    _repository = _JobRepositoryFactory._build_repository()
     _ENTITY_NAME = Job.__name__
-    _ID_PREFIX = "JOB_"
+    _EVENT_ENTITY_TYPE = EventEntityType.JOB
 
     @classmethod
     def _create(cls, task: Task, callbacks: Iterable[Callable], submit_id: str, force=False) -> Job:
         version = _VersionManagerFactory._build_manager()._get_latest_version()
         job = Job(
-            id=JobId(f"{cls._ID_PREFIX}{task.config_id}_{uuid.uuid4()}"),
+            id=JobId(f"{Job._ID_PREFIX}_{task.config_id}_{uuid.uuid4()}"),
             task=task,
             submit_id=submit_id,
             force=force,
             version=version,
         )
         cls._set(job)
+        _publish_event(cls._EVENT_ENTITY_TYPE, job.id, EventOperation.CREATION, None)
         job._on_status_change(*callbacks)
         return job
 
     @classmethod
-    def _delete(cls, job: Job, force=False):  # type:ignore
+    def _delete(cls, job: Job, force=False):
         if job.is_finished() or force:
             super()._delete(job.id)
-            from .._scheduler._dispatcher._job_dispatcher import _JobDispatcher
+            from .._orchestrator._dispatcher._job_dispatcher import _JobDispatcher
 
-            _JobDispatcher._pop_dispatched_process(job.id)  # type: ignore
+            _JobDispatcher._pop_dispatched_process(job.id)
         else:
             err = JobNotDeletedException(job.id)
             cls._logger.warning(err)
             raise err
 
     @classmethod
     def _cancel(cls, job: Union[str, Job]):
         job = cls._get(job) if isinstance(job, str) else job
 
-        from .._scheduler._scheduler_factory import _SchedulerFactory
+        from .._orchestrator._orchestrator_factory import _OrchestratorFactory
 
-        _SchedulerFactory._build_scheduler().cancel_job(job)
+        _OrchestratorFactory._build_orchestrator().cancel_job(job)
 
     @classmethod
     def _get_latest(cls, task: Task) -> Optional[Job]:
         jobs_of_task = list(filter(lambda job: task in job, cls._get_all()))
         if len(jobs_of_task) == 0:
             return None
         if len(jobs_of_task) == 1:
```

### Comparing `taipy-core-2.2.3/src/taipy/core/job/_job_manager_factory.py` & `taipy-core-2.3.0.dev0/src/taipy/core/job/_job_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/job/_job_model.py` & `taipy-core-2.3.0.dev0/src/taipy/core/job/_job_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # specific language governing permissions and limitations under the License.
 
 import dataclasses
 from dataclasses import dataclass
 from typing import Any, Dict, List
 
 from .._version._utils import _version_migration
-from ..common.alias import JobId
+from .job_id import JobId
 from .status import Status
 
 
 @dataclass
 class _JobModel:
     id: JobId
     task_id: str
```

### Comparing `taipy-core-2.2.3/src/taipy/core/job/_job_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/job/_job_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,17 @@
 
     def _from_model(self, model: _JobModel):
         task_repository = _TaskRepositoryFactory._build_repository()
         job = Job(
             id=model.id, task=task_repository.load(model.task_id), submit_id=model.submit_id, version=model.version
         )
 
-        job.status = model.status  # type: ignore
-        job.force = model.force  # type: ignore
-        job.creation_date = datetime.fromisoformat(model.creation_date)  # type: ignore
+        job._status = model.status
+        job._force = model.force
+        job._creation_date = datetime.fromisoformat(model.creation_date)  # type: ignore
         for it in model.subscribers:
             try:
                 job._subscribers.append(_load_fct(it.get("fct_module"), it.get("fct_name")))  # type:ignore
             except AttributeError:
                 raise InvalidSubscriber(f"The subscriber function {it.get('fct_name')} cannot be loaded.")
         job._stacktrace = model.stacktrace
```

### Comparing `taipy-core-2.2.3/src/taipy/core/job/_job_repository_factory.py` & `taipy-core-2.3.0.dev0/src/taipy/core/job/_job_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/job/_job_sql_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/job/_job_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/job/job.py` & `taipy-core-2.3.0.dev0/src/taipy/core/job/job.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,32 +13,33 @@
 
 import traceback
 from datetime import datetime
 from typing import Callable, List
 
 from taipy.logger._taipy_logger import _TaipyLogger
 
+from .._entity._entity import _Entity
+from .._entity._labeled import _Labeled
+from .._entity._reload import _self_reload, _self_setter
 from .._version._version_manager_factory import _VersionManagerFactory
-from ..common._entity import _Entity
-from ..common._reload import _self_reload, _self_setter
-from ..common.alias import JobId
 from ..task.task import Task
+from .job_id import JobId
 from .status import Status
 
 
 def _run_callbacks(fn):
     def __run_callbacks(job):
         fn(job)
         for fct in job._subscribers:
             fct(job)
 
     return __run_callbacks
 
 
-class Job(_Entity):
+class Job(_Entity, _Labeled):
     """Execution of a `Task^`.
 
     A job handles the status of the execution, contains the stacktrace of exceptions that were
     raised during the execution, and notifies subscribers on status change.
 
     Attributes:
         id (str): The identifier of this job.
@@ -49,14 +50,15 @@
         creation_date (datetime): The date of this job's creation.
         stacktrace (List[str]): The list of stacktraces of the exceptions raised during the execution.
         version (str): The string indicates the application version of the job to instantiate. If not provided,
             the latest version is used.
     """
 
     _MANAGER_NAME = "job"
+    _ID_PREFIX = "JOB"
 
     def __init__(self, id: JobId, task: Task, submit_id: str, force=False, version=None):
         self.id = id
         self._task = task
         self._force = force
         self._status = Status.SUBMITTED
         self._creation_date = datetime.now()
@@ -72,14 +74,18 @@
         return self._task
 
     @task.setter  # type: ignore
     @_self_setter(_MANAGER_NAME)
     def task(self, val):
         self._task = val
 
+    @property
+    def owner_id(self) -> str:
+        return self.task.id
+
     @property  # type: ignore
     @_self_reload(_MANAGER_NAME)
     def force(self):
         return self._force
 
     @force.setter  # type: ignore
     @_self_setter(_MANAGER_NAME)
@@ -110,15 +116,15 @@
     def creation_date(self, val):
         self._creation_date = val
 
     @property
     def stacktrace(self) -> List[str]:
         return self._stacktrace
 
-    @property  # type: ignore
+    @property
     def version(self):
         return self._version
 
     def __contains__(self, task: Task):
         return self.task.id == task.id
 
     def __lt__(self, other):
@@ -299,7 +305,23 @@
 
     def __hash__(self):
         return hash(self.id)
 
     def _unlock_edit_on_outputs(self):
         for dn in self.task.output.values():
             dn.unlock_edit()
+
+    def get_label(self) -> str:
+        """Returns the job simple label prefixed by its owner label.
+
+        Returns:
+            The label of the job as a string.
+        """
+        return self._get_label()
+
+    def get_simple_label(self) -> str:
+        """Returns the job simple label.
+
+        Returns:
+            The simple label of the job as a string.
+        """
+        return self._get_simple_label()
```

### Comparing `taipy-core-2.2.3/src/taipy/core/job/status.py` & `taipy-core-2.3.0.dev0/src/taipy/core/job/status.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,17 +16,17 @@
     """Execution status of a `Job^`.
 
     It is implemented as an enumeration.
 
     The possible values are:
 
     - `SUBMITTED`: A `SUBMITTED` job has been submitted for execution but not processed yet by
-        the scheduler.
+        the orchestrator.
 
-    - `PENDING`: A `PENDING` job has been enqueued by the scheduler. It is waiting for an executor
+    - `PENDING`: A `PENDING` job has been enqueued by the orchestrator. It is waiting for an executor
         to be available for its execution.
 
     - `BLOCKED`: A `BLOCKED` job has been blocked because its input data nodes are not ready yet.
         It is waiting for the completion of another `Job^`
 
     - `RUNNING`: A `RUNNING` job is currently executed by a dedicated executor.
```

### Comparing `taipy-core-2.2.3/src/taipy/core/pipeline/__init__.py` & `taipy-core-2.3.0.dev0/src/taipy/core/config/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_fs_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_manager.py` & `taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,34 +8,38 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 from functools import partial
 from typing import Any, Callable, List, Optional, Union
 
-from taipy.config import Config
 from taipy.config.common.scope import Scope
 
+from .._entity._entity_ids import _EntityIds
 from .._manager._manager import _Manager
 from .._version._version_manager_factory import _VersionManagerFactory
-from ..common._entity_ids import _EntityIds
-from ..common.alias import CycleId, PipelineId, ScenarioId
+from ..common.warn_if_inputs_not_ready import _warn_if_inputs_not_ready
 from ..config.pipeline_config import PipelineConfig
+from ..cycle.cycle_id import CycleId
 from ..exceptions.exceptions import NonExistingPipeline
 from ..job._job_manager_factory import _JobManagerFactory
 from ..job.job import Job
+from ..notification import EventEntityType, EventOperation, _publish_event
+from ..scenario.scenario_id import ScenarioId
 from ..task._task_manager_factory import _TaskManagerFactory
 from ..task.task import Task
 from ._pipeline_repository_factory import _PipelineRepositoryFactory
 from .pipeline import Pipeline
+from .pipeline_id import PipelineId
 
 
 class _PipelineManager(_Manager[Pipeline]):
-    _repository = _PipelineRepositoryFactory._build_repository()  # type: ignore
+    _repository = _PipelineRepositoryFactory._build_repository()
     _ENTITY_NAME = Pipeline.__name__
+    _EVENT_ENTITY_TYPE = EventEntityType.PIPELINE
 
     @classmethod
     def _subscribe(
         cls,
         callback: Callable[[Pipeline, Job], None],
         params: Optional[List[Any]] = None,
         pipeline: Optional[Pipeline] = None,
@@ -76,15 +80,15 @@
     @classmethod
     def _get_or_create(
         cls,
         pipeline_config: PipelineConfig,
         cycle_id: Optional[CycleId] = None,
         scenario_id: Optional[ScenarioId] = None,
     ) -> Pipeline:
-        pipeline_id = Pipeline._new_id(str(pipeline_config.id))  # type: ignore
+        pipeline_id = Pipeline._new_id(str(pipeline_config.id))
 
         task_manager = _TaskManagerFactory._build_manager()
         tasks = task_manager._bulk_get_or_create(pipeline_config.task_configs, cycle_id, scenario_id, pipeline_id)
 
         scope = min(task.scope for task in tasks) if len(tasks) != 0 else Scope.GLOBAL
         owner_id: Union[Optional[PipelineId], Optional[ScenarioId], Optional[CycleId]]
         if scope == Scope.PIPELINE:
@@ -97,26 +101,27 @@
             owner_id = None
 
         if pipelines_from_owner := cls._repository._get_by_config_and_owner_id(str(pipeline_config.id), owner_id):
             return pipelines_from_owner
 
         version = _VersionManagerFactory._build_manager()._get_latest_version()
         pipeline = Pipeline(
-            str(pipeline_config.id),  # type: ignore
+            str(pipeline_config.id),
             dict(**pipeline_config._properties),
             tasks,
             pipeline_id,
             owner_id,
             {scenario_id} if scenario_id else None,
             version=version,
         )
         for task in tasks:
             task._parent_ids.update([pipeline_id])
         cls.__save_tasks(tasks)
         cls._set(pipeline)
+        _publish_event(cls._EVENT_ENTITY_TYPE, pipeline.id, EventOperation.CREATION, None)
         return pipeline
 
     @classmethod
     def __save_tasks(cls, tasks):
         task_manager = _TaskManagerFactory._build_manager()
         for i in tasks:
             task_manager._set(i)
@@ -125,26 +130,32 @@
     def _submit(
         cls,
         pipeline: Union[PipelineId, Pipeline],
         callbacks: Optional[List[Callable]] = None,
         force: bool = False,
         wait: bool = False,
         timeout: Optional[Union[float, int]] = None,
-    ):
-        callbacks = callbacks or []
+        check_inputs_are_ready: bool = True,
+    ) -> List[Job]:
         pipeline_id = pipeline.id if isinstance(pipeline, Pipeline) else pipeline
         pipeline = cls._get(pipeline_id)
         if pipeline is None:
             raise NonExistingPipeline(pipeline_id)
+        callbacks = callbacks or []
         pipeline_subscription_callback = cls.__get_status_notifier_callbacks(pipeline) + callbacks
-        return (
+        if check_inputs_are_ready:
+            _warn_if_inputs_not_ready(pipeline._get_inputs())
+
+        jobs = (
             _TaskManagerFactory._build_manager()
-            ._scheduler()
+            ._orchestrator()
             .submit(pipeline, callbacks=pipeline_subscription_callback, force=force, wait=wait, timeout=timeout)
         )
+        _publish_event(cls._EVENT_ENTITY_TYPE, pipeline.id, EventOperation.SUBMISSION, None)
+        return jobs
 
     @staticmethod
     def __get_status_notifier_callbacks(pipeline: Pipeline) -> List:
         return [partial(c.callback, *c.params, pipeline) for c in pipeline.subscribers]
 
     @classmethod
     def _hard_delete(cls, pipeline_id: PipelineId):
```

### Comparing `taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_manager_factory.py` & `taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_model.py` & `taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 # specific language governing permissions and limitations under the License.
 
 import dataclasses
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional
 
 from .._version._utils import _version_migration
-from ..common.alias import PipelineId, TaskId
+from ..task.task_id import TaskId
+from .pipeline_id import PipelineId
 
 
 @dataclass
 class _PipelineModel:
     id: PipelineId
     owner_id: Optional[str]
     parent_ids: List[str]
```

### Comparing `taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_repository.py`

 * *Files 5% similar despite different names*

```diff
@@ -104,7 +104,10 @@
 
     def _export(self, entity_id: str, folder_path: Union[str, pathlib.Path]):
         return self.repo._export(entity_id, folder_path)
 
     @staticmethod
     def __to_task_ids(tasks):
         return [t.id if isinstance(t, Task) else t for t in tasks]
+
+    def _get_by_config_id(self, config_id: str) -> List[Pipeline]:
+        return self.repo._get_by_config_id(config_id)
```

### Comparing `taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_repository_factory.py` & `taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_sql_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/pipeline/_pipeline_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/pipeline/pipeline.py` & `taipy-core-2.3.0.dev0/src/taipy/core/pipeline/pipeline.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,29 +15,32 @@
 from typing import Any, Callable, Dict, List, Optional, Set, Union
 
 import networkx as nx
 
 from taipy.config.common._template_handler import _TemplateHandler as _tpl
 from taipy.config.common._validate_id import _validate_id
 
+from .._entity._entity import _Entity
+from .._entity._labeled import _Labeled
+from .._entity._properties import _Properties
+from .._entity._reload import _reload, _self_reload, _self_setter
+from .._entity._submittable import _Submittable
 from .._version._version_manager_factory import _VersionManagerFactory
-from ..common._entity import _Entity
 from ..common._listattributes import _ListAttributes
-from ..common._properties import _Properties
-from ..common._reload import _reload, _self_reload, _self_setter
 from ..common._utils import _Subscriber
 from ..common._warnings import _warn_deprecated
-from ..common.alias import PipelineId, TaskId
 from ..data.data_node import DataNode
 from ..exceptions.exceptions import NonExistingTask
 from ..job.job import Job
 from ..task.task import Task
+from ..task.task_id import TaskId
+from .pipeline_id import PipelineId
 
 
-class Pipeline(_Entity):
+class Pipeline(_Entity, _Submittable, _Labeled):
     """List of `Task^`s and additional attributes representing a set of data processing
     elements connected as a direct acyclic graph.
 
     Attributes:
         config_id (str): The identifier of the `PipelineConfig^`.
         properties (dict[str, Any]): A dictionary of additional properties.
         tasks (List[Task^]): The list of `Task`s.
@@ -53,67 +56,65 @@
     _MANAGER_NAME = "pipeline"
 
     def __init__(
         self,
         config_id: str,
         properties: Dict[str, Any],
         tasks: Union[List[TaskId], List[Task], List[Union[TaskId, Task]]],
-        pipeline_id: PipelineId = None,
+        pipeline_id: Optional[PipelineId] = None,
         owner_id: Optional[str] = None,
         parent_ids: Optional[Set[str]] = None,
-        subscribers: List[_Subscriber] = None,
+        subscribers: Optional[List[_Subscriber]] = None,
         version: str = None,
     ):
+        super().__init__(subscribers)
         self.config_id = _validate_id(config_id)
         self.id: PipelineId = pipeline_id or self._new_id(self.config_id)
+        self._tasks = tasks
         self.owner_id = owner_id
         self._parent_ids = parent_ids or set()
-        self._tasks = tasks
-
-        self._subscribers = _ListAttributes(self, subscribers or list())
         self._properties = _Properties(self, **properties)
-
         self._version = version or _VersionManagerFactory._build_manager()._get_latest_version()
 
-    @property  # type: ignore
-    def parent_id(self):
-        """
-        Deprecated. Use owner_id instead.
-        """
-        _warn_deprecated("parent_id", suggest="owner_id")
-        return self.owner_id
-
-    @parent_id.setter  # type: ignore
-    def parent_id(self, val):
-        """
-        Deprecated. Use owner_id instead.
-        """
-        _warn_deprecated("parent_id", suggest="owner_id")
-        self.owner_id = val
-
-    @property  # type: ignore
-    @_self_reload(_MANAGER_NAME)
-    def parent_ids(self):
-        return self._parent_ids
+    @staticmethod
+    def _new_id(config_id: str) -> PipelineId:
+        return PipelineId(Pipeline.__SEPARATOR.join([Pipeline._ID_PREFIX, _validate_id(config_id), str(uuid.uuid4())]))
 
     def __getstate__(self):
         return self.id
 
     def __setstate__(self, id):
-        import taipy.core as tp
+        from ... import core as tp
 
         p = tp.get(id)
         self.__dict__ = p.__dict__
 
     def __hash__(self):
         return hash(self.id)
 
+    def __eq__(self, other):
+        return self.id == other.id
+
+    def __getattr__(self, attribute_name):
+        protected_attribute_name = _validate_id(attribute_name)
+        if protected_attribute_name in self._properties:
+            return _tpl._replace_templates(self._properties[protected_attribute_name])
+        tasks = self._get_tasks()
+        if protected_attribute_name in tasks:
+            return tasks[protected_attribute_name]
+        for task in tasks.values():
+            if protected_attribute_name in task.input:
+                return task.input[protected_attribute_name]
+            if protected_attribute_name in task.output:
+                return task.output[protected_attribute_name]
+        raise AttributeError(f"{attribute_name} is not an attribute of pipeline {self.id}")
+
     @property  # type: ignore
     @_self_reload(_MANAGER_NAME)
-    def tasks(self):
+    def tasks(self) -> Dict[str, Task]:
         return self._get_tasks()
 
     @tasks.setter  # type: ignore
     @_self_setter(_MANAGER_NAME)
     def tasks(self, tasks: Union[List[TaskId], List[Task]]):
         self._tasks = tasks
 
@@ -123,123 +124,91 @@
         list_data_nodes = [task.data_nodes for task in self._get_tasks().values()]
         for data_node in list_data_nodes:
             for k, v in data_node.items():
                 data_nodes[k] = v
         return data_nodes
 
     @property  # type: ignore
-    @_self_reload(_MANAGER_NAME)
-    def subscribers(self):
-        return self._subscribers
+    def parent_id(self):
+        """
+        Deprecated. Use owner_id instead.
+        """
+        _warn_deprecated("parent_id", suggest="owner_id")
+        return self.owner_id
 
-    @subscribers.setter  # type: ignore
-    @_self_setter(_MANAGER_NAME)
-    def subscribers(self, val):
-        self._subscribers = val or set()
+    @parent_id.setter  # type: ignore
+    def parent_id(self, val):
+        """
+        Deprecated. Use owner_id instead.
+        """
+        _warn_deprecated("parent_id", suggest="owner_id")
+        self.owner_id = val
+
+    @property  # type: ignore
+    @_self_reload(_MANAGER_NAME)
+    def parent_ids(self):
+        return self._parent_ids
 
     @property  # type: ignore
     def version(self):
         return self._version
 
     @property  # type: ignore
     def properties(self):
         self._properties = _reload("pipeline", self)._properties
         return self._properties
 
-    def __eq__(self, other):
-        return self.id == other.id
-
-    @staticmethod
-    def _new_id(config_id: str) -> PipelineId:
-        return PipelineId(Pipeline.__SEPARATOR.join([Pipeline._ID_PREFIX, _validate_id(config_id), str(uuid.uuid4())]))
-
-    def __getattr__(self, attribute_name):
-        protected_attribute_name = _validate_id(attribute_name)
-        if protected_attribute_name in self._properties:
-            return _tpl._replace_templates(self._properties[protected_attribute_name])
-        tasks = self._get_tasks()
-        if protected_attribute_name in tasks:
-            return tasks[protected_attribute_name]
-        for task in tasks.values():
-            if protected_attribute_name in task.input:
-                return task.input[protected_attribute_name]
-            if protected_attribute_name in task.output:
-                return task.output[protected_attribute_name]
-        raise AttributeError(f"{attribute_name} is not an attribute of pipeline {self.id}")
-
     def _is_consistent(self) -> bool:
-        dag = self.__build_dag()
+        dag = self._build_dag()
         if not nx.is_directed_acyclic_graph(dag):
             return False
         is_data_node = True
         for nodes in nx.topological_generations(dag):
             for node in nodes:
                 if is_data_node and not isinstance(node, DataNode):
                     return False
                 if not is_data_node and not isinstance(node, Task):
                     return False
             is_data_node = not is_data_node
         return True
 
-    def __build_dag(self):
-        graph = nx.DiGraph()
-        tasks = self._get_tasks()
-        for task in tasks.values():
-            if has_input := task.input:
-                for predecessor in task.input.values():
-                    graph.add_edges_from([(predecessor, task)])
-            if has_output := task.output:
-                for successor in task.output.values():
-                    graph.add_edges_from([(task, successor)])
-            if not has_input and not has_output:
-                graph.add_node(task)
-        return graph
-
-    def _get_tasks(self):
+    def _get_tasks(self) -> Dict[str, Task]:
         from ..task._task_manager_factory import _TaskManagerFactory
 
         tasks = {}
         task_manager = _TaskManagerFactory._build_manager()
         for task_or_id in self._tasks:
             t = task_manager._get(task_or_id, task_or_id)
             if not isinstance(t, Task):
                 raise NonExistingTask(task_or_id)
             tasks[t.config_id] = t
+        return tasks
 
+    def _get_set_of_tasks(self) -> Set[Task]:
+        from ..task._task_manager_factory import _TaskManagerFactory
+
+        tasks = set()
+        task_manager = _TaskManagerFactory._build_manager()
+        for task_or_id in self._tasks:
+            task = task_manager._get(task_or_id, task_or_id)
+            if not isinstance(task, Task):
+                raise NonExistingTask(task_or_id)
+            tasks.add(task)
         return tasks
 
     @property  # type: ignore
     @_self_reload(_MANAGER_NAME)
     def subscribers(self):
         return self._subscribers
 
     @subscribers.setter  # type: ignore
     @_self_setter(_MANAGER_NAME)
     def subscribers(self, val):
         self._subscribers = _ListAttributes(self, val)
 
-    def _add_subscriber(self, callback: Callable, params: Optional[List[Any]] = None):
-        params = [] if params is None else params
-        self._subscribers.append(_Subscriber(callback=callback, params=params))
-
-    def _remove_subscriber(self, callback: Callable, params: Optional[List[Any]] = None):
-        if params is not None:
-            self._subscribers.remove(_Subscriber(callback, params))
-        else:
-            elem = [x for x in self._subscribers if x.callback == callback]
-            if not elem:
-                raise ValueError
-            self._subscribers.remove(elem[0])
-
-    def _get_sorted_tasks(self) -> List[List[Task]]:
-        dag = self.__build_dag()
-        remove = [node for node, degree in dict(dag.in_degree).items() if degree == 0 and isinstance(node, DataNode)]
-        dag.remove_nodes_from(remove)
-        return list(nodes for nodes in nx.topological_generations(dag) if (Task in (type(node) for node in nodes)))
-
     def get_parents(self):
         """Get parents of the pipeline entity"""
         from ... import core as tp
 
         return tp.get_parents(self)
 
     def subscribe(
@@ -276,25 +245,42 @@
 
     def submit(
         self,
         callbacks: Optional[List[Callable]] = None,
         force: bool = False,
         wait: bool = False,
         timeout: Optional[Union[float, int]] = None,
-    ):
+    ) -> List[Job]:
         """Submit the pipeline for execution.
 
         All the `Task^`s of the pipeline will be submitted for execution.
 
         Parameters:
             callbacks (List[Callable]): The list of callable functions to be called on status
                 change.
             force (bool): Force execution even if the data nodes are in cache.
-            wait (bool): Wait for the scheduled jobs created from the pipeline submission to be finished in asynchronous
-                mode.
+            wait (bool): Wait for the orchestrated jobs created from the pipeline submission to be finished
+                in asynchronous mode.
             timeout (Union[float, int]): The maximum number of seconds to wait for the jobs to be finished before
                 returning.
-
+        Returns:
+            A list of created `Job^`s.
         """
         from ._pipeline_manager_factory import _PipelineManagerFactory
 
         return _PipelineManagerFactory._build_manager()._submit(self, callbacks, force, wait, timeout)
+
+    def get_label(self) -> str:
+        """Returns the pipeline simple label prefixed by its owner label.
+
+        Returns:
+            The label of the pipeline as a string.
+        """
+        return self._get_label()
+
+    def get_simple_label(self) -> str:
+        """Returns the pipeline simple label.
+
+        Returns:
+            The simple label of the pipeline as a string.
+        """
+        return self._get_simple_label()
```

### Comparing `taipy-core-2.2.3/src/taipy/core/scenario/__init__.py` & `taipy-core-2.3.0.dev0/src/taipy/core/cycle/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/scenario/_scenario_fs_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/scenario/_scenario_manager.py` & `taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 import datetime
 from functools import partial
 from typing import Any, Callable, List, Optional, Union
 
 from taipy.config import Config
 
+from .._entity._entity_ids import _EntityIds
 from .._manager._manager import _Manager
 from .._version._version_manager_factory import _VersionManagerFactory
-from ..common._entity_ids import _EntityIds
-from ..common.alias import ScenarioId
+from ..common.warn_if_inputs_not_ready import _warn_if_inputs_not_ready
 from ..config.scenario_config import ScenarioConfig
 from ..cycle._cycle_manager_factory import _CycleManagerFactory
 from ..cycle.cycle import Cycle
 from ..exceptions.exceptions import (
     DeletingPrimaryScenario,
     DifferentScenarioConfigs,
     DoesNotBelongToACycle,
@@ -30,25 +30,28 @@
     NonExistingComparator,
     NonExistingScenario,
     NonExistingScenarioConfig,
     UnauthorizedTagError,
 )
 from ..job._job_manager_factory import _JobManagerFactory
 from ..job.job import Job
+from ..notification import EventEntityType, EventOperation, _publish_event
 from ..pipeline._pipeline_manager_factory import _PipelineManagerFactory
 from ..task._task_manager_factory import _TaskManagerFactory
 from ..task.task import Task
 from ._scenario_repository_factory import _ScenarioRepositoryFactory
 from .scenario import Scenario
+from .scenario_id import ScenarioId
 
 
 class _ScenarioManager(_Manager[Scenario]):
     _AUTHORIZED_TAGS_KEY = "authorized_tags"
-    _repository = _ScenarioRepositoryFactory._build_repository()  # type: ignore
+    _repository = _ScenarioRepositoryFactory._build_repository()
     _ENTITY_NAME = Scenario.__name__
+    _EVENT_ENTITY_TYPE = EventEntityType.SCENARIO
 
     @classmethod
     def _subscribe(
         cls,
         callback: Callable[[Scenario, Job], None],
         params: Optional[List[Any]] = None,
         scenario: Optional[Scenario] = None,
@@ -86,18 +89,18 @@
         scenario._remove_subscriber(callback, params)
         cls._set(scenario)
 
     @classmethod
     def _create(
         cls,
         config: ScenarioConfig,
-        creation_date: datetime.datetime = None,
-        name: str = None,
+        creation_date: Optional[datetime.datetime] = None,
+        name: Optional[str] = None,
     ) -> Scenario:
-        scenario_id = Scenario._new_id(str(config.id))  # type: ignore
+        scenario_id = Scenario._new_id(str(config.id))
         cycle = (
             _CycleManagerFactory._build_manager()._get_or_create(config.frequency, creation_date)
             if config.frequency
             else None
         )
 
         pipelines = [
@@ -107,54 +110,62 @@
 
         is_primary_scenario = len(cls._get_all_by_cycle(cycle)) == 0 if cycle else False
         props = config._properties.copy()
         if name:
             props["name"] = name
         version = _VersionManagerFactory._build_manager()._get_latest_version()
         scenario = Scenario(
-            str(config.id),  # type: ignore
+            str(config.id),
             pipelines,
             props,
             scenario_id,
             creation_date,
             is_primary=is_primary_scenario,
             cycle=cycle,
             version=version,
         )
         for pipeline in pipelines:
             pipeline._parent_ids.update([scenario_id])
         cls.__save_pipelines(pipelines)
         cls._set(scenario)
+        _publish_event(cls._EVENT_ENTITY_TYPE, scenario.id, EventOperation.CREATION, None)
         return scenario
 
     @classmethod
     def __save_pipelines(cls, pipelines):
         pipeline_manager = _PipelineManagerFactory._build_manager()
         for i in pipelines:
             pipeline_manager._set(i)
 
     @classmethod
     def _submit(
         cls,
         scenario: Union[Scenario, ScenarioId],
+        callbacks: Optional[List[Callable]] = None,
         force: bool = False,
         wait: bool = False,
         timeout: Optional[Union[float, int]] = None,
-    ):
+        check_inputs_are_ready: bool = True,
+    ) -> List[Job]:
         scenario_id = scenario.id if isinstance(scenario, Scenario) else scenario
         scenario = cls._get(scenario_id)
         if scenario is None:
             raise NonExistingScenario(scenario_id)
-        callbacks = cls.__get_status_notifier_callbacks(scenario)
-        jobs_in_pipelines = {}
-        for pipeline in scenario.pipelines.values():
-            jobs_in_pipelines[pipeline.id] = _PipelineManagerFactory._build_manager()._submit(
-                pipeline, callbacks=callbacks, force=force, wait=wait, timeout=timeout
-            )
-        return jobs_in_pipelines
+        callbacks = callbacks or []
+        scenario_subscription_callback = cls.__get_status_notifier_callbacks(scenario) + callbacks
+        if check_inputs_are_ready:
+            _warn_if_inputs_not_ready(scenario._get_inputs())
+
+        jobs = (
+            _TaskManagerFactory._build_manager()
+            ._orchestrator()
+            .submit(scenario, callbacks=scenario_subscription_callback, force=force, wait=wait, timeout=timeout)
+        )
+        _publish_event(cls._EVENT_ENTITY_TYPE, scenario.id, EventOperation.SUBMISSION, None)
+        return jobs
 
     @classmethod
     def __get_status_notifier_callbacks(cls, scenario: Scenario) -> List:
         return [partial(c.callback, *c.params, scenario) for c in scenario.subscribers]
 
     @classmethod
     def _get_primary(cls, cycle: Cycle) -> Optional[Scenario]:
@@ -221,27 +232,27 @@
 
     @classmethod
     def _untag(cls, scenario: Scenario, tag: str):
         scenario._remove_tag(tag)
         cls._set(scenario)
 
     @classmethod
-    def _delete(cls, scenario_id: ScenarioId):  # type: ignore
+    def _delete(cls, scenario_id: ScenarioId):
         scenario = cls._get(scenario_id)
         if scenario.is_primary:
             if len(cls._get_all_by_cycle(scenario.cycle)) > 1:
                 raise DeletingPrimaryScenario(
                     f"Scenario {scenario.id}, which has config id {scenario.config_id}, is primary and there are "
                     f"other scenarios in the same cycle. "
                 )
             _CycleManagerFactory._build_manager()._delete(scenario.cycle.id)
         super()._delete(scenario_id)
 
     @classmethod
-    def _compare(cls, *scenarios: Scenario, data_node_config_id: str = None):
+    def _compare(cls, *scenarios: Scenario, data_node_config_id: Optional[str] = None):
         if len(scenarios) < 2:
             raise InsufficientScenarioToCompare("At least two scenarios are required to compare.")
 
         if not all(scenarios[0].config_id == scenario.config_id for scenario in scenarios):
             raise DifferentScenarioConfigs("Scenarios to compare must have the same configuration.")
 
         if scenario_config := _ScenarioManager.__get_config(scenarios[0]):
@@ -290,15 +301,15 @@
         Deletes scenario by the version number.
 
         Check if the cycle is only attached to this scenario, then delete it.
         """
         while scenario := cls._repository._search("version", version_number, version_number="all"):
             if scenario.cycle and len(cls._get_all_by_cycle(scenario.cycle)) == 1:
                 _CycleManagerFactory._build_manager()._delete(scenario.cycle.id)
-            cls._repository._delete(scenario.id)
+            super()._delete(scenario.id)
 
     @classmethod
     def _get_children_entity_ids(cls, scenario: Scenario) -> _EntityIds:
         entity_ids = _EntityIds()
 
         for pipeline in scenario.pipelines.values():
             if pipeline.owner_id in (pipeline.id, scenario.id):
```

### Comparing `taipy-core-2.2.3/src/taipy/core/scenario/_scenario_manager_factory.py` & `taipy-core-2.3.0.dev0/src/taipy/core/task/_task_manager_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,20 +9,18 @@
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 from typing import Type
 
 from .._manager._manager_factory import _ManagerFactory
 from ..common._utils import _load_fct
-from ._scenario_manager import _ScenarioManager
-from ._scenario_repository_factory import _ScenarioRepositoryFactory
+from ..task._task_repository_factory import _TaskRepositoryFactory
+from ._task_manager import _TaskManager
 
 
-class _ScenarioManagerFactory(_ManagerFactory):
+class _TaskManagerFactory(_ManagerFactory):
     @classmethod
-    def _build_manager(cls) -> Type[_ScenarioManager]:  # type: ignore
+    def _build_manager(cls) -> Type[_TaskManager]:  # type: ignore
         if cls._using_enterprise():
-            return _load_fct(
-                cls._TAIPY_ENTERPRISE_CORE_MODULE + ".scenario._scenario_manager", "_ScenarioManager"
-            )  # type: ignore
-        _ScenarioManager._repository = _ScenarioRepositoryFactory._build_repository()  # type: ignore
-        return _ScenarioManager
+            return _load_fct(cls._TAIPY_ENTERPRISE_CORE_MODULE + ".task._task_manager", "_TaskManager")  # type: ignore
+        _TaskManager._repository = _TaskRepositoryFactory._build_repository()  # type: ignore
+        return _TaskManager
```

### Comparing `taipy-core-2.2.3/src/taipy/core/scenario/_scenario_model.py` & `taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 # specific language governing permissions and limitations under the License.
 
 import dataclasses
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional
 
 from .._version._utils import _version_migration
-from ..common.alias import CycleId, PipelineId, ScenarioId
+from ..cycle.cycle_id import CycleId
+from ..pipeline.pipeline_id import PipelineId
+from .scenario_id import ScenarioId
 
 
 @dataclass
 class _ScenarioModel:
     id: ScenarioId
     config_id: str
     pipelines: List[PipelineId]
```

### Comparing `taipy-core-2.2.3/src/taipy/core/scenario/_scenario_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 from datetime import datetime
 from typing import Any, Iterable, List, Optional, Union
 
 from .._repository._repository import _AbstractRepository
 from .._repository._repository_adapter import _RepositoryAdapter
 from ..common import _utils
 from ..common._utils import _Subscriber
-from ..common.alias import CycleId, PipelineId
 from ..cycle._cycle_manager_factory import _CycleManagerFactory
 from ..cycle.cycle import Cycle
+from ..cycle.cycle_id import CycleId
 from ..pipeline.pipeline import Pipeline
+from ..pipeline.pipeline_id import PipelineId
 from ._scenario_model import _ScenarioModel
 from .scenario import Scenario
 
 
 class _ScenarioRepository(_AbstractRepository[_ScenarioModel, Scenario]):  # type: ignore
     def __init__(self, **kwargs):
         kwargs.update({"to_model_fct": self._to_model, "from_model_fct": self._from_model})
@@ -89,14 +90,17 @@
 
     def _search(self, attribute: str, value: Any, version_number: Optional[str] = None) -> Optional[Scenario]:
         return self.repo._search(attribute, value, version_number)
 
     def _export(self, entity_id: str, folder_path: Union[str, pathlib.Path]):
         return self.repo._export(entity_id, folder_path)
 
+    def _get_by_config_id(self, config_id: str) -> List[Scenario]:
+        return self.repo._get_by_config_id(config_id)
+
     @staticmethod
     def __to_pipeline_ids(pipelines) -> List[PipelineId]:
         return [p.id if isinstance(p, Pipeline) else p for p in pipelines]
 
     @staticmethod
     def __to_cycle(cycle_id: CycleId = None) -> Optional[Cycle]:
         return _CycleManagerFactory._build_manager()._get(cycle_id) if cycle_id else None
```

### Comparing `taipy-core-2.2.3/src/taipy/core/scenario/_scenario_repository_factory.py` & `taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/scenario/_scenario_sql_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/scenario/_scenario_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/scenario/scenario.py` & `taipy-core-2.3.0.dev0/src/taipy/core/scenario/scenario.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,30 +15,34 @@
 import uuid
 from datetime import datetime
 from typing import Any, Callable, Dict, List, Optional, Set, Union
 
 from taipy.config.common._template_handler import _TemplateHandler as _tpl
 from taipy.config.common._validate_id import _validate_id
 
+from .._entity._entity import _Entity
+from .._entity._labeled import _Labeled
+from .._entity._properties import _Properties
+from .._entity._reload import _reload, _self_reload, _self_setter
+from .._entity._submittable import _Submittable
 from .._version._version_manager_factory import _VersionManagerFactory
-from ..common._entity import _Entity
 from ..common._listattributes import _ListAttributes
-from ..common._properties import _Properties
-from ..common._reload import _reload, _self_reload, _self_setter
 from ..common._utils import _Subscriber
-from ..common.alias import PipelineId, ScenarioId
 from ..cycle.cycle import Cycle
 from ..data.data_node import DataNode
 from ..exceptions.exceptions import NonExistingPipeline
 from ..job.job import Job
 from ..pipeline._pipeline_manager_factory import _PipelineManagerFactory
 from ..pipeline.pipeline import Pipeline
+from ..pipeline.pipeline_id import PipelineId
+from ..task.task import Task
+from .scenario_id import ScenarioId
 
 
-class Scenario(_Entity):
+class Scenario(_Entity, _Submittable, _Labeled):
     """Instance of a Business case to solve.
 
     A scenario holds a list of pipelines (instances of `Pipeline^` class) to submit for execution
     in order to solve the Business case.
 
     Attributes:
         config_id (str): The identifier of the `ScenarioConfig^`.
@@ -59,57 +63,103 @@
     __SEPARATOR = "_"
 
     def __init__(
         self,
         config_id: str,
         pipelines: Union[List[PipelineId], List[Pipeline]],
         properties: Dict[str, Any],
-        scenario_id: ScenarioId = None,
-        creation_date=None,
+        scenario_id: Optional[ScenarioId] = None,
+        creation_date: Optional[datetime] = None,
         is_primary: bool = False,
-        cycle: Cycle = None,
-        subscribers: List[_Subscriber] = None,
-        tags: Set[str] = None,
+        cycle: Optional[Cycle] = None,
+        subscribers: Optional[List[_Subscriber]] = None,
+        tags: Optional[Set[str]] = None,
         version: str = None,
     ):
+        super().__init__(subscribers)
         self.config_id = _validate_id(config_id)
         self.id: ScenarioId = scenario_id or self._new_id(self.config_id)
         self._pipelines = pipelines
         self._creation_date = creation_date or datetime.now()
         self._cycle = cycle
-        self._subscribers = _ListAttributes(self, subscribers or list())
         self._primary_scenario = is_primary
         self._tags = tags or set()
+        self._properties = _Properties(self, **properties)
         self._version = version or _VersionManagerFactory._build_manager()._get_latest_version()
 
-        self._properties = _Properties(self, **properties)
+    @staticmethod
+    def _new_id(config_id: str) -> ScenarioId:
+        """Generate a unique scenario identifier."""
+        return ScenarioId(Scenario.__SEPARATOR.join([Scenario._ID_PREFIX, _validate_id(config_id), str(uuid.uuid4())]))
 
     def __getstate__(self):
         return self.id
 
     def __setstate__(self, id):
         from ... import core as tp
 
         sc = tp.get(id)
         self.__dict__ = sc.__dict__
 
     def __hash__(self):
         return hash(self.id)
 
+    def __eq__(self, other):
+        return self.id == other.id
+
+    def __getattr__(self, attribute_name):
+        protected_attribute_name = _validate_id(attribute_name)
+        if protected_attribute_name in self._properties:
+            return _tpl._replace_templates(self._properties[protected_attribute_name])
+        pipelines = self.pipelines
+        if protected_attribute_name in pipelines:
+            return pipelines[protected_attribute_name]
+        for pipeline in pipelines.values():
+            tasks = pipeline.tasks
+            if protected_attribute_name in tasks:
+                return tasks[protected_attribute_name]
+            for task in tasks.values():
+                if protected_attribute_name in task.input:
+                    return task.input[protected_attribute_name]
+                if protected_attribute_name in task.output:
+                    return task.output[protected_attribute_name]
+        raise AttributeError(f"{attribute_name} is not an attribute of scenario {self.id}")
+
     @property  # type: ignore
     @_self_reload(_MANAGER_NAME)
     def pipelines(self):
         return self.__get_pipelines()
 
     @pipelines.setter  # type: ignore
     @_self_setter(_MANAGER_NAME)
     def pipelines(self, pipelines: Union[List[PipelineId], List[Pipeline]]):
         self._pipelines = pipelines
 
     @property
+    def tasks(self) -> Dict[str, List[Task]]:
+        tasks: Dict[str, List[Task]] = {}
+        list_dict_tasks = [pipeline.tasks for pipeline in self.pipelines.values()]
+        for dict_task in list_dict_tasks:
+            for task_config_id, task in dict_task.items():
+                if task_config_id in tasks:
+                    if task not in tasks[task_config_id]:
+                        tasks[task_config_id].append(task)
+                else:
+                    tasks[task_config_id] = [task]
+        return tasks
+
+    def _get_set_of_tasks(self) -> Set[Task]:
+        tasks = set()
+        list_dict_tasks = [pipeline.tasks for pipeline in self.pipelines.values()]
+        for dict_task in list_dict_tasks:
+            for task in dict_task.values():
+                tasks.add(task)
+        return tasks
+
+    @property
     def data_nodes(self) -> Dict[str, DataNode]:
         data_nodes = {}
         list_data_nodes = [pipeline.data_nodes for pipeline in self.pipelines.values()]
         for data_node in list_data_nodes:
             for k, v in data_node.items():
                 data_nodes[k] = v
         return data_nodes
@@ -160,85 +210,50 @@
         return self._tags
 
     @tags.setter  # type: ignore
     @_self_setter(_MANAGER_NAME)
     def tags(self, val):
         self._tags = val or set()
 
-    @property  # type: ignore
+    @property
     def version(self):
         return self._version
 
-    @property  # type: ignore
+    @property
+    def owner_id(self):
+        return self._cycle.id
+
+    @property
     def properties(self):
         self._properties = _reload(self._MANAGER_NAME, self)._properties
         return self._properties
 
     @property  # type: ignore
     @_self_reload(_MANAGER_NAME)
     def name(self) -> Optional[str]:
         return self._properties.get("name")
 
     @name.setter  # type: ignore
     @_self_setter(_MANAGER_NAME)
     def name(self, val):
         self._properties["name"] = val
 
-    def __eq__(self, other):
-        return self.id == other.id
-
-    @staticmethod
-    def _new_id(config_id: str) -> ScenarioId:
-        """Generate a unique scenario identifier."""
-        return ScenarioId(Scenario.__SEPARATOR.join([Scenario._ID_PREFIX, _validate_id(config_id), str(uuid.uuid4())]))
-
-    def __getattr__(self, attribute_name):
-        protected_attribute_name = _validate_id(attribute_name)
-        if protected_attribute_name in self._properties:
-            return _tpl._replace_templates(self._properties[protected_attribute_name])
-        pipelines = self.pipelines
-        if protected_attribute_name in pipelines:
-            return pipelines[protected_attribute_name]
-        for pipeline in pipelines.values():
-            tasks = pipeline.tasks
-            if protected_attribute_name in tasks:
-                return tasks[protected_attribute_name]
-            for task in tasks.values():
-                if protected_attribute_name in task.input:
-                    return task.input[protected_attribute_name]
-                if protected_attribute_name in task.output:
-                    return task.output[protected_attribute_name]
-        raise AttributeError(f"{attribute_name} is not an attribute of scenario {self.id}")
-
-    def _add_subscriber(self, callback: Callable, params: Optional[List[Any]] = None):
-        params = [] if params is None else params
-        self._subscribers.append(_Subscriber(callback=callback, params=params))
-
-    def _add_tag(self, tag: str):
-        self._tags = _reload("scenario", self)._tags
-        self._tags.add(tag)
-
     def has_tag(self, tag: str) -> bool:
         """Indicate if the scenario has a given tag.
 
         Parameters:
             tag (str): The tag to search among the set of scenario's tags.
         Returns:
             True if the scenario has the tag given as parameter. False otherwise.
         """
         return tag in self.tags
 
-    def _remove_subscriber(self, callback: Callable, params: Optional[List[Any]] = None):
-        if params is not None:
-            self._subscribers.remove(_Subscriber(callback, params))
-        else:
-            elem = [x for x in self._subscribers if x.callback == callback]
-            if not elem:
-                raise ValueError
-            self._subscribers.remove(elem[0])
+    def _add_tag(self, tag: str):
+        self._tags = _reload("scenario", self)._tags
+        self._tags.add(tag)
 
     def _remove_tag(self, tag: str):
         self._tags = _reload("scenario", self)._tags
         if self.has_tag(tag):
             self._tags.remove(tag)
 
     def subscribe(
@@ -263,37 +278,49 @@
         return tp.subscribe_scenario(callback, params, self)
 
     def unsubscribe(self, callback: Callable[[Scenario, Job], None], params: Optional[List[Any]] = None):
         """Unsubscribe a function that is called when the status of a `Job^` changes.
 
         Parameters:
             callback (Callable[[Scenario^, Job^], None]): The callable function to unsubscribe.
+            params (Optional[List[Any]]): The parameters to be passed to the _callback_.
 
         Note:
             The function will continue to be called for ongoing jobs.
         """
         from ... import core as tp
 
         return tp.unsubscribe_scenario(callback, params, self)
 
-    def submit(self, force: bool = False, wait: bool = False, timeout: Optional[Union[float, int]] = None):
+    def submit(
+        self,
+        callbacks: Optional[List[Callable]] = None,
+        force: bool = False,
+        wait: bool = False,
+        timeout: Optional[Union[float, int]] = None,
+    ) -> List[Job]:
         """Submit this scenario for execution.
 
         All the `Task^`s of the scenario will be submitted for execution.
 
         Parameters:
+            callbacks (List[Callable]): The list of callable functions to be called on status
+                change.
             force (bool): Force execution even if the data nodes are in cache.
-            wait (bool): Wait for the scheduled jobs created from the scenario submission to be finished in
+            wait (bool): Wait for the orchestrated jobs created from the scenario submission to be finished in
                 asynchronous mode.
             timeout (Union[float, int]): The optional maximum number of seconds to wait for the jobs to be finished
                 before returning.
+
+        Returns:
+            A list of created `Job^`s.
         """
-        from ... import core as tp
+        from ._scenario_manager_factory import _ScenarioManagerFactory
 
-        return tp.submit(self, force, wait, timeout)
+        return _ScenarioManagerFactory._build_manager()._submit(self, callbacks, force, wait, timeout)
 
     def export(
         self,
         folder_path: Union[str, pathlib.Path],
     ):
         """Export all related entities of this scenario to a folder.
 
@@ -344,7 +371,23 @@
         for pipeline_or_id in self._pipelines:
             p = pipeline_manager._get(pipeline_or_id, pipeline_or_id)
 
             if not isinstance(p, Pipeline):
                 raise NonExistingPipeline(pipeline_or_id)
             pipelines[p.config_id] = p
         return pipelines
+
+    def get_label(self) -> str:
+        """Returns the scenario simple label prefixed by its owner label.
+
+        Returns:
+            The label of the scenario as a string.
+        """
+        return self._get_label()
+
+    def get_simple_label(self) -> str:
+        """Returns the scenario simple label.
+
+        Returns:
+            The simple label of the scenario as a string.
+        """
+        return self._get_simple_label()
```

### Comparing `taipy-core-2.2.3/src/taipy/core/taipy.py` & `taipy-core-2.3.0.dev0/src/taipy/core/taipy.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,33 +13,38 @@
 import shutil
 from datetime import datetime
 from typing import Any, Callable, Dict, List, Optional, Set, Union, overload
 
 from taipy.config.config import Config
 from taipy.logger._taipy_logger import _TaipyLogger
 
+from ._entity._entity import _Entity
 from ._version._version_manager_factory import _VersionManagerFactory
-from .common._entity import _Entity
 from .common._warnings import _warn_no_core_service
-from .common.alias import CycleId, DataNodeId, JobId, PipelineId, ScenarioId, TaskId
 from .config.pipeline_config import PipelineConfig
 from .config.scenario_config import ScenarioConfig
 from .cycle._cycle_manager_factory import _CycleManagerFactory
 from .cycle.cycle import Cycle
+from .cycle.cycle_id import CycleId
 from .data._data_manager_factory import _DataManagerFactory
 from .data.data_node import DataNode
+from .data.data_node_id import DataNodeId
 from .exceptions.exceptions import ModelNotFound, NonExistingVersion, VersionIsNotProductionVersion
 from .job._job_manager_factory import _JobManagerFactory
 from .job.job import Job
+from .job.job_id import JobId
 from .pipeline._pipeline_manager_factory import _PipelineManagerFactory
 from .pipeline.pipeline import Pipeline
+from .pipeline.pipeline_id import PipelineId
 from .scenario._scenario_manager_factory import _ScenarioManagerFactory
 from .scenario.scenario import Scenario
+from .scenario.scenario_id import ScenarioId
 from .task._task_manager_factory import _TaskManagerFactory
 from .task.task import Task
+from .task.task_id import TaskId
 
 __logger = _TaipyLogger._get_logger()
 
 
 def set(entity: Union[DataNode, Task, Pipeline, Scenario, Cycle]):
     """Save or update an entity.
 
@@ -61,27 +66,32 @@
 
 @_warn_no_core_service()
 def submit(
     entity: Union[Scenario, Pipeline, Task],
     force: bool = False,
     wait: bool = False,
     timeout: Optional[Union[float, int]] = None,
-):
+) -> Union[Job, List[Job]]:
     """Submit an entity for execution.
 
     If the entity is a pipeline or a scenario, all the tasks of the entity are
     submitted for execution.
 
     Parameters:
         entity (Union[Scenario^, Pipeline^, Task^]): The entity to submit.
         force (bool): If True, the execution is forced even if the data nodes are in cache.
-        wait (bool): Wait for the scheduled jobs created from the submission to be finished in asynchronous mode.
-        timeout (Union[float, int]): The optional maximum number of seconds to wait for the jobs to be finished before
-            returning.
+        wait (bool): Wait for the orchestrated jobs created from the submission to be finished
+            in asynchronous mode.
+        timeout (Union[float, int]): The optional maximum number of seconds to wait
+            for the jobs to be finished before returning.
+    Returns:
+        The created `Job^` or a collection of the created `Job^` depends on the submitted entity.
 
+        - If a `Scenario^` or a `Pipeline^` is provided, it will return a list of `Job^`.
+        - If a `Task^` is provided, it will return the created `Job^`.
     """
     if isinstance(entity, Scenario):
         return _ScenarioManagerFactory._build_manager()._submit(entity, force=force, wait=wait, timeout=timeout)
     if isinstance(entity, Pipeline):
         return _PipelineManagerFactory._build_manager()._submit(entity, force=force, wait=wait, timeout=timeout)
     if isinstance(entity, Task):
         return _TaskManagerFactory._build_manager()._submit(entity, force=force, wait=wait, timeout=timeout)
@@ -113,30 +123,35 @@
 
 
 @overload
 def get(entity_id: JobId) -> Job:
     ...
 
 
+@overload
+def get(entity_id: str) -> Union[Task, DataNode, Pipeline, Scenario, Job, Cycle]:
+    ...
+
+
 def get(
-    entity_id: Union[TaskId, DataNodeId, PipelineId, ScenarioId, JobId, CycleId]
+    entity_id: Union[TaskId, DataNodeId, PipelineId, ScenarioId, JobId, CycleId, str]
 ) -> Union[Task, DataNode, Pipeline, Scenario, Job, Cycle]:
     """Get an entity from its identifier.
 
     Parameters:
         entity_id (Union[TaskId^, DataNodeId^, PipelineId^, ScenarioId^]): The identifier
             of the entity to get.<br/>
             It must match the identifier pattern of one of the entities (`Task^`, `DataNode^`,
             `Pipeline^` or `Scenario^`).
     Returns:
         The entity matching the corresponding identifier. None if no entity is found.
     Raises:
         ModelNotFound^: If _entity_id_ does not match a correct entity pattern.
     """
-    if entity_id.startswith(_JobManagerFactory._build_manager()._ID_PREFIX):
+    if entity_id.startswith(Job._ID_PREFIX):
         return _JobManagerFactory._build_manager()._get(JobId(entity_id))
     if entity_id.startswith(Cycle._ID_PREFIX):
         return _CycleManagerFactory._build_manager()._get(CycleId(entity_id))
     if entity_id.startswith(Scenario._ID_PREFIX):
         return _ScenarioManagerFactory._build_manager()._get(ScenarioId(entity_id))
     if entity_id.startswith(Pipeline._ID_PREFIX):
         return _PipelineManagerFactory._build_manager()._get(PipelineId(entity_id))
@@ -171,15 +186,15 @@
 
     Parameters:
         entity_id (Union[TaskId^, DataNodeId^, PipelineId^, ScenarioId^, JobId^, CycleId^]): The
             identifier of the entity to delete.
     Raises:
         ModelNotFound^: No entity corresponds to _entity_id_.
     """
-    if entity_id.startswith(_JobManagerFactory._build_manager()._ID_PREFIX):
+    if entity_id.startswith(Job._ID_PREFIX):
         job_manager = _JobManagerFactory._build_manager()
         return job_manager._delete(job_manager._get(JobId(entity_id)))  # type: ignore
     if entity_id.startswith(Cycle._ID_PREFIX):
         return _CycleManagerFactory._build_manager()._hard_delete(CycleId(entity_id))
     if entity_id.startswith(Scenario._ID_PREFIX):
         return _ScenarioManagerFactory._build_manager()._hard_delete(ScenarioId(entity_id))
     if entity_id.startswith(Pipeline._ID_PREFIX):
@@ -497,34 +512,41 @@
     _ScenarioManagerFactory._build_manager()._delete_all()
     _CycleManagerFactory._build_manager()._delete_all()
     _JobManagerFactory._build_manager()._delete_all()
     _VersionManagerFactory._build_manager()._delete_all()
     return True
 
 
-def clean_all_entities_by_version(version_number):
-    """Delete all entities belongs to a version from the Taipy data folder."""
+def clean_all_entities_by_version(version_number) -> bool:
+    """Delete all entities belongs to a version from the Taipy data folder.
+
+    Returns:
+        True if the operation succeeded, False otherwise.
+    """
     version_manager = _VersionManagerFactory._build_manager()
     try:
         version_number = version_manager._replace_version_number(version_number)
     except NonExistingVersion as e:
-        raise SystemExit(e.message)
+        __logger.warning(f"{e.message} Abort cleaning the entities of version '{version_number}'.")
+        return False
 
     _JobManagerFactory._build_manager()._delete_by_version(version_number)
     _ScenarioManagerFactory._build_manager()._delete_by_version(version_number)
     _PipelineManagerFactory._build_manager()._delete_by_version(version_number)
     _TaskManagerFactory._build_manager()._delete_by_version(version_number)
     _DataManagerFactory._build_manager()._delete_by_version(version_number)
 
     version_manager._delete(version_number)
     try:
         version_manager._delete_production_version(version_number)
     except VersionIsNotProductionVersion:
         pass
 
+    return True
+
 
 def export_scenario(
     scenario_id: ScenarioId,
     folder_path: Union[str, pathlib.Path],
 ):
     """Export all related entities of a scenario to a folder.
 
@@ -604,7 +626,47 @@
     if isinstance(entity, DataNode):
         parent_entity_key = "tasks"
         update_parent_dict(parents, parent_dict, parent_entity_key)
         for parent in parent_dict[parent_entity_key]:
             get_parents(parent, parent_dict)
 
     return parent_dict
+
+
+def get_cycles_scenarios() -> Dict[Optional[Cycle], List[Scenario]]:
+    """Get the scenarios grouped by cycles.
+
+    Returns:
+        The dictionary of all cycles and their corresponding scenarios.
+    """
+
+    cycles_scenarios: Dict[Optional[Cycle], List[Scenario]] = {}
+    for scenario in get_scenarios():
+        if scenario.cycle in cycles_scenarios.keys():
+            cycles_scenarios[scenario.cycle].append(scenario)
+        else:
+            cycles_scenarios[scenario.cycle] = [scenario]
+    return cycles_scenarios
+
+
+def get_entities_by_config_id(
+    config_id: str,
+) -> Union[List, List[Task], List[DataNode], List[Pipeline], List[Scenario]]:
+    """Get the entities by its cofig id.
+
+    Parameters:
+        config_id (str): The config id of the entities
+    Returns:
+        The list of all entities by the config id.
+    """
+
+    entities: List = []
+
+    if entities := _ScenarioManagerFactory._build_manager()._get_by_config_id(config_id):
+        return entities
+    if entities := _PipelineManagerFactory._build_manager()._get_by_config_id(config_id):
+        return entities
+    if entities := _TaskManagerFactory._build_manager()._get_by_config_id(config_id):
+        return entities
+    if entities := _DataManagerFactory._build_manager()._get_by_config_id(config_id):
+        return entities
+    return entities
```

### Comparing `taipy-core-2.2.3/src/taipy/core/task/__init__.py` & `taipy-core-2.3.0.dev0/src/taipy/core/job/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/task/_task_fs_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/task/_task_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/task/_task_manager.py` & `taipy-core-2.3.0.dev0/src/taipy/core/task/_task_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,35 +9,41 @@
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 from typing import Callable, List, Optional, Type, Union
 
 from taipy.config.common.scope import Scope
 
+from .._entity._entity_ids import _EntityIds
 from .._manager._manager import _Manager
-from .._scheduler._abstract_scheduler import _AbstractScheduler
-from .._scheduler._scheduler_factory import _SchedulerFactory
+from .._orchestrator._abstract_orchestrator import _AbstractOrchestrator
+from .._orchestrator._orchestrator_factory import _OrchestratorFactory
 from .._version._version_manager_factory import _VersionManagerFactory
-from ..common._entity_ids import _EntityIds
-from ..common.alias import CycleId, PipelineId, ScenarioId, TaskId
+from ..common.warn_if_inputs_not_ready import _warn_if_inputs_not_ready
 from ..config.task_config import TaskConfig
+from ..cycle.cycle_id import CycleId
 from ..data._data_manager_factory import _DataManagerFactory
 from ..exceptions.exceptions import NonExistingTask
 from ..job._job_manager_factory import _JobManagerFactory
+from ..notification import EventEntityType, EventOperation, _publish_event
+from ..pipeline.pipeline_id import PipelineId
+from ..scenario.scenario_id import ScenarioId
 from ..task._task_repository_factory import _TaskRepositoryFactory
 from ..task.task import Task
+from .task_id import TaskId
 
 
 class _TaskManager(_Manager[Task]):
-    _repository = _TaskRepositoryFactory._build_repository()  # type: ignore
+    _repository = _TaskRepositoryFactory._build_repository()
     _ENTITY_NAME = Task.__name__
+    _EVENT_ENTITY_TYPE = EventEntityType.TASK
 
     @classmethod
-    def _scheduler(cls) -> Type[_AbstractScheduler]:
-        return _SchedulerFactory._build_scheduler()
+    def _orchestrator(cls) -> Type[_AbstractOrchestrator]:
+        return _OrchestratorFactory._build_orchestrator()
 
     @classmethod
     def _set(cls, task: Task):
         cls.__save_data_nodes(task.input.values())
         cls.__save_data_nodes(task.output.values())
         super()._set(task)
 
@@ -71,39 +77,40 @@
             elif scope == Scope.CYCLE:
                 owner_id = cycle_id
             else:
                 owner_id = None
 
             tasks_configs_and_owner_id.append((task_config, owner_id))
 
-        tasks_by_config = cls._repository._get_by_configs_and_owner_ids(tasks_configs_and_owner_id)  # type: ignore
+        tasks_by_config = cls._repository._get_by_configs_and_owner_ids(tasks_configs_and_owner_id)
 
         tasks = []
         for task_config, owner_id in tasks_configs_and_owner_id:
             if task := tasks_by_config.get((task_config, owner_id)):
                 tasks.append(task)
             else:
                 version = _VersionManagerFactory._build_manager()._get_latest_version()
                 inputs = [data_nodes[input_config] for input_config in task_config.input_configs]
                 outputs = [data_nodes[output_config] for output_config in task_config.output_configs]
                 skippable = task_config.skippable
                 task = Task(
-                    str(task_config.id),  # type: ignore
+                    str(task_config.id),
                     dict(**task_config._properties),
                     task_config.function,
                     inputs,
                     outputs,
                     owner_id=owner_id,
                     parent_ids=set(),
                     version=version,
                     skippable=skippable,
                 )
                 for dn in set(inputs + outputs):
                     dn._parent_ids.update([task.id])
                 cls._set(task)
+                _publish_event(cls._EVENT_ENTITY_TYPE, task.id, EventOperation.CREATION, None)
                 tasks.append(task)
         return tasks
 
     @classmethod
     def __save_data_nodes(cls, data_nodes):
         data_manager = _DataManagerFactory._build_manager()
         for i in data_nodes:
@@ -129,13 +136,18 @@
     def _submit(
         cls,
         task: Union[TaskId, Task],
         callbacks: Optional[List[Callable]] = None,
         force: bool = False,
         wait: bool = False,
         timeout: Optional[Union[float, int]] = None,
+        check_inputs_are_ready: bool = True,
     ):
         task_id = task.id if isinstance(task, Task) else task
         task = cls._get(task_id)
         if task is None:
             raise NonExistingTask(task_id)
-        return cls._scheduler().submit_task(task, callbacks=callbacks, force=force, wait=wait, timeout=timeout)
+        if check_inputs_are_ready:
+            _warn_if_inputs_not_ready(task.input.values())
+        job = cls._orchestrator().submit_task(task, callbacks=callbacks, force=force, wait=wait, timeout=timeout)
+        _publish_event(cls._EVENT_ENTITY_TYPE, task.id, EventOperation.SUBMISSION, None)
+        return job
```

### Comparing `taipy-core-2.2.3/src/taipy/core/task/_task_manager_factory.py` & `taipy-core-2.3.0.dev0/src/taipy/core/_version/_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
-from typing import Type
+from .._core_cli import _CoreCLI
+from ..config import CoreSection
+from ._version_manager_factory import _VersionManagerFactory
 
-from .._manager._manager_factory import _ManagerFactory
-from ..common._utils import _load_fct
-from ..task._task_repository_factory import _TaskRepositoryFactory
-from ._task_manager import _TaskManager
 
+def _version_migration() -> str:
+    """Add version attribute on old entities. Used to migrate from <=2.0 to >=2.1 version."""
 
-class _TaskManagerFactory(_ManagerFactory):
-    @classmethod
-    def _build_manager(cls) -> Type[_TaskManager]:  # type: ignore
-        if cls._using_enterprise():
-            return _load_fct(cls._TAIPY_ENTERPRISE_CORE_MODULE + ".task._task_manager", "_TaskManager")  # type: ignore
-        _TaskManager._repository = _TaskRepositoryFactory._build_repository()  # type: ignore
-        return _TaskManager
+    args = _CoreCLI.parse_arguments()
+
+    if args[CoreSection._MODE_KEY] != CoreSection._DEVELOPMENT_MODE:
+        return _VersionManagerFactory._build_manager()._get_latest_version()
+    else:
+        _VersionManagerFactory._build_manager()._get_or_create("LEGACY-VERSION", True)
+        return "LEGACY-VERSION"
```

### Comparing `taipy-core-2.2.3/src/taipy/core/task/_task_model.py` & `taipy-core-2.3.0.dev0/src/taipy/core/task/_task_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/task/_task_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/task/_task_repository.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 
 import pathlib
 from typing import Any, Iterable, List, Optional, Union
 
 from .._repository._repository import _AbstractRepository
 from .._repository._repository_adapter import _RepositoryAdapter
 from ..common._utils import _load_fct
-from ..common.alias import TaskId
 from ..data._data_manager_factory import _DataManagerFactory
 from ..exceptions.exceptions import NonExistingDataNode
 from ._task_model import _TaskModel
 from .task import Task
+from .task_id import TaskId
 
 
 class _TaskRepository(_AbstractRepository[_TaskModel, Task]):  # type: ignore
     def __init__(self, **kwargs):
         kwargs.update({"to_model_fct": self._to_model, "from_model_fct": self._from_model})
         self.repo = _RepositoryAdapter.select_base_repository()(**kwargs)
 
@@ -100,7 +100,10 @@
         data_manager = _DataManagerFactory._build_manager()
         for _id in data_nodes_ids:
             if data_node := data_manager._get(_id):
                 data_nodes.append(data_node)
             else:
                 raise NonExistingDataNode(_id)
         return data_nodes
+
+    def _get_by_config_id(self, config_id: str) -> List[Task]:
+        return self.repo._get_by_config_id(config_id)
```

### Comparing `taipy-core-2.2.3/src/taipy/core/task/_task_repository_factory.py` & `taipy-core-2.3.0.dev0/src/taipy/core/task/_task_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/task/_task_sql_repository.py` & `taipy-core-2.3.0.dev0/src/taipy/core/task/_task_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.3/src/taipy/core/task/task.py` & `taipy-core-2.3.0.dev0/src/taipy/core/task/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,30 +6,34 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import uuid
-from typing import Any, Callable, Dict, Iterable, List, Optional, Set, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, List, Optional, Set, Union
 
 from taipy.config.common._template_handler import _TemplateHandler as _tpl
 from taipy.config.common._validate_id import _validate_id
 from taipy.config.common.scope import Scope
 
+from .._entity._entity import _Entity
+from .._entity._labeled import _Labeled
+from .._entity._properties import _Properties
+from .._entity._reload import _reload, _self_reload, _self_setter
 from .._version._version_manager_factory import _VersionManagerFactory
-from ..common._entity import _Entity
-from ..common._properties import _Properties
-from ..common._reload import _reload, _self_reload, _self_setter
 from ..common._warnings import _warn_deprecated
-from ..common.alias import TaskId
 from ..data.data_node import DataNode
+from .task_id import TaskId
 
+if TYPE_CHECKING:
+    from ..job.job import Job
 
-class Task(_Entity):
+
+class Task(_Entity, _Labeled):
     """Hold a user function that will be executed, its parameters and the results.
 
     A `Task` brings together the user code as function, the inputs and the outputs as data nodes
     (instances of the `DataNode^` class).
 
     Attributes:
         config_id (str): The identifier of the `TaskConfig^`.
@@ -55,15 +59,15 @@
     def __init__(
         self,
         config_id: str,
         properties: Dict[str, Any],
         function,
         input: Optional[Iterable[DataNode]] = None,
         output: Optional[Iterable[DataNode]] = None,
-        id: TaskId = None,
+        id: Optional[TaskId] = None,
         owner_id: Optional[str] = None,
         parent_ids: Optional[Set[str]] = None,
         version: str = None,
         skippable: bool = False,
     ):
         self.config_id = _validate_id(config_id)
         self.id = id or TaskId(self.__ID_SEPARATOR.join([self._ID_PREFIX, self.config_id, str(uuid.uuid4())]))
@@ -72,23 +76,32 @@
         self.__input = {dn.config_id: dn for dn in input or []}
         self.__output = {dn.config_id: dn for dn in output or []}
         self._function = function
         self._version = version or _VersionManagerFactory._build_manager()._get_latest_version()
         self._skippable = skippable
         self._properties = _Properties(self, **properties)
 
-    @property  # type: ignore
-    @_self_reload(_MANAGER_NAME)
-    def skippable(self):
-        return self._skippable
+    def __hash__(self):
+        return hash(self.id)
 
-    @skippable.setter  # type: ignore
-    @_self_setter(_MANAGER_NAME)
-    def skippable(self, val):
-        self._skippable = val
+    def __getstate__(self):
+        return vars(self)
+
+    def __setstate__(self, state):
+        vars(self).update(state)
+
+    def __getattr__(self, attribute_name):
+        protected_attribute_name = _validate_id(attribute_name)
+        if protected_attribute_name in self._properties:
+            return _tpl._replace_templates(self._properties[protected_attribute_name])
+        if protected_attribute_name in self.input:
+            return self.input[protected_attribute_name]
+        if protected_attribute_name in self.output:
+            return self.output[protected_attribute_name]
+        raise AttributeError(f"{attribute_name} is not an attribute of task {self.id}")
 
     @property  # type: ignore
     def properties(self):
         self._properties = _reload(self._MANAGER_NAME, self)._properties
         return self._properties
 
     @property  # type: ignore
@@ -110,23 +123,14 @@
         return tp.get_parents(self)
 
     @property  # type: ignore
     @_self_reload(_MANAGER_NAME)
     def parent_ids(self):
         return self._parent_ids
 
-    def __hash__(self):
-        return hash(self.id)
-
-    def __getstate__(self):
-        return vars(self)
-
-    def __setstate__(self, state):
-        vars(self).update(state)
-
     @property  # type: ignore
     def input(self) -> Dict[str, DataNode]:
         return self.__input
 
     @property  # type: ignore
     def output(self) -> Dict[str, DataNode]:
         return self.__output
@@ -141,23 +145,23 @@
         return self._function
 
     @function.setter  # type: ignore
     @_self_setter(_MANAGER_NAME)
     def function(self, val):
         self._function = val
 
-    def __getattr__(self, attribute_name):
-        protected_attribute_name = _validate_id(attribute_name)
-        if protected_attribute_name in self._properties:
-            return _tpl._replace_templates(self._properties[protected_attribute_name])
-        if protected_attribute_name in self.input:
-            return self.input[protected_attribute_name]
-        if protected_attribute_name in self.output:
-            return self.output[protected_attribute_name]
-        raise AttributeError(f"{attribute_name} is not an attribute of task {self.id}")
+    @property  # type: ignore
+    @_self_reload(_MANAGER_NAME)
+    def skippable(self):
+        return self._skippable
+
+    @skippable.setter  # type: ignore
+    @_self_setter(_MANAGER_NAME)
+    def skippable(self, val):
+        self._skippable = val
 
     @property
     def scope(self) -> Scope:
         """Retrieve the lowest scope of the task based on its data nodes.
 
         Returns:
             The lowest scope present in input and output data nodes or GLOBAL if there are
@@ -173,22 +177,41 @@
 
     def submit(
         self,
         callbacks: Optional[List[Callable]] = None,
         force: bool = False,
         wait: bool = False,
         timeout: Optional[Union[float, int]] = None,
-    ):
+    ) -> "Job":  # noqa
         """Submit the task for execution.
 
         Parameters:
             callbacks (List[Callable]): The list of callable functions to be called on status
                 change.
             force (bool): Force execution even if the data nodes are in cache.
-            wait (bool): Wait for the scheduled job created from the task submission to be finished in asynchronous
+            wait (bool): Wait for the orchestrated job created from the task submission to be finished in asynchronous
                 mode.
             timeout (Union[float, int]): The maximum number of seconds to wait for the job to be finished before
                 returning.
+
+        Returns:
+            The created `Job^`.
         """
         from ._task_manager_factory import _TaskManagerFactory
 
-        _TaskManagerFactory._build_manager()._submit(self, callbacks, force, wait, timeout)
+        return _TaskManagerFactory._build_manager()._submit(self, callbacks, force, wait, timeout)
+
+    def get_label(self) -> str:
+        """Returns the task simple label prefixed by its owner label.
+
+        Returns:
+            The label of the task as a string.
+        """
+        return self._get_label()
+
+    def get_simple_label(self) -> str:
+        """Returns the task simple label.
+
+        Returns:
+            The simple label of the task as a string.
+        """
+        return self._get_simple_label()
```

### Comparing `taipy-core-2.2.3/src/taipy_core.egg-info/PKG-INFO` & `taipy-core-2.3.0.dev0/src/taipy_core.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-core
-Version: 2.2.3
+Version: 2.3.0.dev0
 Summary: A Python library to build powerful and customized data-driven back-end applications.
 Home-page: https://github.com/avaiga/taipy-core
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-core
 Classifier: Intended Audience :: Developers
@@ -26,15 +26,15 @@
 # Taipy Core
 [![tests](https://github.com/Avaiga/taipy-core/actions/workflows/tests.yml/badge.svg)](https://github.com/Avaiga/taipy-core/actions/workflows/tests.yml)
 [![Python](https://img.shields.io/pypi/pyversions/taipy-core)](https://pypi.org/project/taipy-core)
 [![PyPI](https://img.shields.io/pypi/v/taipy-core.svg?label=pip&logo=PyPI&logoColor=white)](https://pypi.org/project/taipy-core)
 
 
 ## License
-Copyright 2022 Avaiga Private Limited
+Copyright 2023 Avaiga Private Limited
 
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with
 the License. You may obtain a copy of the License at
 [http://www.apache.org/licenses/LICENSE-2.0](https://www.apache.org/licenses/LICENSE-2.0.txt)
 
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
@@ -73,16 +73,18 @@
 
 Want to be part of the _Taipy Core_ community? Check out our [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) file.
 
 ## Directory Structure
 
 - `taipy/core`:
     - `taipy/core`:
+        - `_manager`: Internal package for entity manager.
         - `_repository`: Internal package for data storage.
-        - `_scheduler`: Internal package for task scheduling and execution.
+        - `_orchestrator`: Internal package for task orchestrating and execution.
+        - `_version`: Internal package for managing Taipy Core application version.
         - `common`: Shared data structures, types, and functions.
         - `config`: Configuration definition, management and implementation. `config.config.Config` is the main
           entrypoint for configuring a Taipy Core application.
         - `cycle`: Work cycle definition, management and implementation.
         - `data`: Data Node definition, management and implementation.
         - `exceptions`: _taipy-core_ exceptions.
         - `job`: Job definition, management and implementation.
@@ -93,9 +95,10 @@
     - `tests`: Unit tests following the `taipy/core` structure.
 - `CODE_OF_CONDUCT.md`: Code of conduct for members and contributors of _taipy-core_.
 - `CONTRIBUTING.md`: Instructions to contribute to _taipy-core_.
 - `INSTALLATION.md`: Instructions to install _taipy-core_.
 - `LICENSE`: The Apache 2.0 License.
 - `Pipfile`: File used by the Pipenv virtual environment to manage project dependencies.
 - `README.md`: Current file.
+- `contributors.txt`: The list of contributors.
 - `setup.py`: The setup script managing building, distributing, and installing _taipy-core_.
 - `tox.ini`: Contains test scenarios to be run.
```

### Comparing `taipy-core-2.2.3/src/taipy_core.egg-info/SOURCES.txt` & `taipy-core-2.3.0.dev0/src/taipy_core.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -2,91 +2,104 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/taipy/__init__.py
 src/taipy/core/__init__.py
 src/taipy/core/_core.py
+src/taipy/core/_core_cli.py
 src/taipy/core/taipy.py
 src/taipy/core/version.json
+src/taipy/core/_backup/__init__.py
+src/taipy/core/_backup/_backup.py
+src/taipy/core/_entity/__init__.py
+src/taipy/core/_entity/_dag.py
+src/taipy/core/_entity/_entity.py
+src/taipy/core/_entity/_entity_ids.py
+src/taipy/core/_entity/_labeled.py
+src/taipy/core/_entity/_properties.py
+src/taipy/core/_entity/_reload.py
+src/taipy/core/_entity/_submittable.py
 src/taipy/core/_manager/__init__.py
 src/taipy/core/_manager/_manager.py
 src/taipy/core/_manager/_manager_factory.py
+src/taipy/core/_orchestrator/__init__.py
+src/taipy/core/_orchestrator/_abstract_orchestrator.py
+src/taipy/core/_orchestrator/_orchestrator.py
+src/taipy/core/_orchestrator/_orchestrator_factory.py
+src/taipy/core/_orchestrator/_dispatcher/__init__.py
+src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py
+src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py
+src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py
 src/taipy/core/_repository/__init__.py
 src/taipy/core/_repository/_filesystem_repository.py
 src/taipy/core/_repository/_repository.py
 src/taipy/core/_repository/_repository_adapter.py
 src/taipy/core/_repository/_repository_factory.py
 src/taipy/core/_repository/_sql_model.py
 src/taipy/core/_repository/_sql_repository.py
-src/taipy/core/_scheduler/__init__.py
-src/taipy/core/_scheduler/_abstract_scheduler.py
-src/taipy/core/_scheduler/_scheduler.py
-src/taipy/core/_scheduler/_scheduler_factory.py
-src/taipy/core/_scheduler/_dispatcher/__init__.py
-src/taipy/core/_scheduler/_dispatcher/_development_job_dispatcher.py
-src/taipy/core/_scheduler/_dispatcher/_job_dispatcher.py
-src/taipy/core/_scheduler/_dispatcher/_standalone_job_dispatcher.py
 src/taipy/core/_version/__init__.py
 src/taipy/core/_version/_utils.py
 src/taipy/core/_version/_version.py
-src/taipy/core/_version/_version_cli.py
 src/taipy/core/_version/_version_fs_repository.py
 src/taipy/core/_version/_version_manager.py
 src/taipy/core/_version/_version_manager_factory.py
 src/taipy/core/_version/_version_model.py
 src/taipy/core/_version/_version_repository.py
 src/taipy/core/_version/_version_repository_factory.py
 src/taipy/core/_version/_version_sql_repository.py
+src/taipy/core/_version/_cli/__init__.py
+src/taipy/core/_version/_cli/_bcolor.py
+src/taipy/core/_version/_cli/_version_cli.py
 src/taipy/core/common/__init__.py
-src/taipy/core/common/_entity.py
-src/taipy/core/common/_entity_ids.py
-src/taipy/core/common/_get_valid_filename.py
 src/taipy/core/common/_listattributes.py
-src/taipy/core/common/_properties.py
-src/taipy/core/common/_reload.py
 src/taipy/core/common/_repr_enum.py
 src/taipy/core/common/_utils.py
 src/taipy/core/common/_warnings.py
-src/taipy/core/common/alias.py
 src/taipy/core/common/default_custom_document.py
+src/taipy/core/common/warn_if_inputs_not_ready.py
 src/taipy/core/config/__init__.py
+src/taipy/core/config/_core_section.py
 src/taipy/core/config/config.schema.json
 src/taipy/core/config/data_node_config.py
 src/taipy/core/config/job_config.py
 src/taipy/core/config/pipeline_config.py
 src/taipy/core/config/scenario_config.py
 src/taipy/core/config/task_config.py
 src/taipy/core/config/checkers/__init__.py
+src/taipy/core/config/checkers/_config_id_checker.py
 src/taipy/core/config/checkers/_data_node_config_checker.py
 src/taipy/core/config/checkers/_job_config_checker.py
 src/taipy/core/config/checkers/_pipeline_config_checker.py
 src/taipy/core/config/checkers/_scenario_config_checker.py
 src/taipy/core/config/checkers/_task_config_checker.py
 src/taipy/core/cycle/__init__.py
 src/taipy/core/cycle/_cycle_fs_repository.py
 src/taipy/core/cycle/_cycle_manager.py
 src/taipy/core/cycle/_cycle_manager_factory.py
 src/taipy/core/cycle/_cycle_model.py
 src/taipy/core/cycle/_cycle_repository.py
 src/taipy/core/cycle/_cycle_repository_factory.py
 src/taipy/core/cycle/_cycle_sql_repository.py
 src/taipy/core/cycle/cycle.py
+src/taipy/core/cycle/cycle_id.py
 src/taipy/core/data/__init__.py
 src/taipy/core/data/_data_fs_repository.py
 src/taipy/core/data/_data_manager.py
 src/taipy/core/data/_data_manager_factory.py
 src/taipy/core/data/_data_model.py
 src/taipy/core/data/_data_repository.py
 src/taipy/core/data/_data_repository_factory.py
 src/taipy/core/data/_data_sql_repository.py
 src/taipy/core/data/_filter.py
+src/taipy/core/data/abstract_file.py
 src/taipy/core/data/abstract_sql.py
 src/taipy/core/data/csv.py
 src/taipy/core/data/data_node.py
+src/taipy/core/data/data_node_id.py
 src/taipy/core/data/excel.py
 src/taipy/core/data/generic.py
 src/taipy/core/data/in_memory.py
 src/taipy/core/data/json.py
 src/taipy/core/data/mongo.py
 src/taipy/core/data/operator.py
 src/taipy/core/data/parquet.py
@@ -100,42 +113,53 @@
 src/taipy/core/job/_job_manager.py
 src/taipy/core/job/_job_manager_factory.py
 src/taipy/core/job/_job_model.py
 src/taipy/core/job/_job_repository.py
 src/taipy/core/job/_job_repository_factory.py
 src/taipy/core/job/_job_sql_repository.py
 src/taipy/core/job/job.py
+src/taipy/core/job/job_id.py
 src/taipy/core/job/status.py
+src/taipy/core/notification/__init__.py
+src/taipy/core/notification/core_event_consumer.py
+src/taipy/core/notification/event.py
+src/taipy/core/notification/notifier.py
+src/taipy/core/notification/registration.py
+src/taipy/core/notification/registration_id.py
+src/taipy/core/notification/topic.py
 src/taipy/core/pipeline/__init__.py
 src/taipy/core/pipeline/_pipeline_fs_repository.py
 src/taipy/core/pipeline/_pipeline_manager.py
 src/taipy/core/pipeline/_pipeline_manager_factory.py
 src/taipy/core/pipeline/_pipeline_model.py
 src/taipy/core/pipeline/_pipeline_repository.py
 src/taipy/core/pipeline/_pipeline_repository_factory.py
 src/taipy/core/pipeline/_pipeline_sql_repository.py
 src/taipy/core/pipeline/pipeline.py
+src/taipy/core/pipeline/pipeline_id.py
 src/taipy/core/scenario/__init__.py
 src/taipy/core/scenario/_scenario_fs_repository.py
 src/taipy/core/scenario/_scenario_manager.py
 src/taipy/core/scenario/_scenario_manager_factory.py
 src/taipy/core/scenario/_scenario_model.py
 src/taipy/core/scenario/_scenario_repository.py
 src/taipy/core/scenario/_scenario_repository_factory.py
 src/taipy/core/scenario/_scenario_sql_repository.py
 src/taipy/core/scenario/scenario.py
+src/taipy/core/scenario/scenario_id.py
 src/taipy/core/task/__init__.py
 src/taipy/core/task/_task_fs_repository.py
 src/taipy/core/task/_task_manager.py
 src/taipy/core/task/_task_manager_factory.py
 src/taipy/core/task/_task_model.py
 src/taipy/core/task/_task_repository.py
 src/taipy/core/task/_task_repository_factory.py
 src/taipy/core/task/_task_sql_repository.py
 src/taipy/core/task/task.py
+src/taipy/core/task/task_id.py
 src/taipy_core.egg-info/PKG-INFO
 src/taipy_core.egg-info/SOURCES.txt
 src/taipy_core.egg-info/dependency_links.txt
 src/taipy_core.egg-info/not-zip-safe
 src/taipy_core.egg-info/requires.txt
 src/taipy_core.egg-info/top_level.txt
 tests/test_complex_application.py
```

### Comparing `taipy-core-2.2.3/tests/test_complex_application.py` & `taipy-core-2.3.0.dev0/tests/test_complex_application.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import pathlib
 from time import sleep
 
 import pandas as pd
 
 import src.taipy.core.taipy as tp
 from src.taipy.core import Status
-from src.taipy.core._scheduler._scheduler_factory import _SchedulerFactory
+from src.taipy.core._orchestrator._orchestrator_factory import _OrchestratorFactory
 from src.taipy.core.config.job_config import JobConfig
 from taipy.config import Config
 
 # ################################  USER FUNCTIONS  ##################################
 
 
 def sum(a, b):
@@ -67,15 +67,15 @@
 
 
 # ################################  TEST METHODS    ##################################
 
 
 def test_skipped_jobs():
     Config.configure_job_executions(mode=JobConfig._DEVELOPMENT_MODE)
-    _SchedulerFactory._build_scheduler()
+    _OrchestratorFactory._build_orchestrator()
     input_config = Config.configure_data_node("input")
     intermediate_config = Config.configure_data_node("intermediate")
     output_config = Config.configure_data_node("output")
     task_config_1 = Config.configure_task("first", mult_by_2, input_config, intermediate_config, skippable=True)
     task_config_2 = Config.configure_task("second", mult_by_2, intermediate_config, output_config, skippable=True)
     pipeline_config = Config.configure_pipeline("pipeline", [task_config_1, task_config_2])
 
@@ -107,15 +107,15 @@
     # |      |            |     t6 --- d8 -------------------
     # |      t3 --- d6 ---|
     # |      |
     # |      |
     # t4     d4
 
     Config.configure_job_executions(mode=JobConfig._DEVELOPMENT_MODE)
-    _SchedulerFactory._build_scheduler()
+    _OrchestratorFactory._build_orchestrator()
 
     csv_path_inp = os.path.join(pathlib.Path(__file__).parent.resolve(), "data_sample/example.csv")
     excel_path_inp = os.path.join(pathlib.Path(__file__).parent.resolve(), "data_sample/example.xlsx")
 
     csv_path_sum = os.path.join(pathlib.Path(__file__).parent.resolve(), "data_sample/sum.csv")
     excel_path_sum = os.path.join(pathlib.Path(__file__).parent.resolve(), "data_sample/sum.xlsx")
 
@@ -191,15 +191,15 @@
 
     for path in [csv_path_sum, excel_path_sum, csv_path_out, excel_path_out]:
         os.remove(path)
 
 
 # def test_same_pipeline_submission_with_overlap_datanode():
 #     Config.configure_job_executions(mode=JobConfig._STANDALONE_MODE, nb_of_workers=1)
-#     _Scheduler._update_job_config()
+#     _Orchestrator._update_job_config()
 
 #     # d1 ---- t1 ---- d2 ---- t2
 #     # t3 ---- d2
 
 #     csv_path_inp = os.path.join(pathlib.Path(__file__).parent.resolve(), "data_sample/example.csv")
 
 #     dn1_inp_csv = Config.configure_csv_data_node("dn1_inp_csv", default_path=csv_path_inp)
@@ -223,35 +223,35 @@
 #     pipeline_div_print = tp.create_pipeline(pipeline_div_print_config)
 #     pipeline_populate_constant = tp.create_pipeline(pipeline_populate_constant_config)
 
 #     tp.submit(pipeline_div_print)
 #     tp.submit(pipeline_div_print)
 #     tp.submit(pipeline_populate_constant)
 
-#     assert _Scheduler.jobs_to_run.qsize() == 2
+#     assert _Orchestrator.jobs_to_run.qsize() == 2
 #     assert pipeline_div_print.dn2_div.read() is None
 
 #     sleep(1.5)
-#     assert _Scheduler.jobs_to_run.qsize() == 2
+#     assert _Orchestrator.jobs_to_run.qsize() == 2
 #     assert pipeline_div_print.dn2_div.read() is not None
 #     assert len(pipeline_div_print.dn2_div.read()) == 10
 
 #     sleep(1)
-#     assert _Scheduler.jobs_to_run.qsize() == 2
+#     assert _Orchestrator.jobs_to_run.qsize() == 2
 #     assert pipeline_div_print.dn2_div.read() is not None
 #     assert len(pipeline_div_print.dn2_div.read()) == 10
 
 #     sleep(1.5)
-#     assert _Scheduler.jobs_to_run.qsize() == 0
+#     assert _Orchestrator.jobs_to_run.qsize() == 0
 #     assert pipeline_div_print.dn2_div.read() == 10
 
 #     Config.configure_job_executions(mode=JobConfig._STANDALONE_MODE, nb_of_workers=2)
-#     _Scheduler._update_job_config()
+#     _Orchestrator._update_job_config()
 
 #     tp.submit(pipeline_div_print)
 #     tp.submit(pipeline_div_print)
 
-#     assert _Scheduler.jobs_to_run.qsize() == 0
+#     assert _Orchestrator.jobs_to_run.qsize() == 0
 
 #     sleep(2.5)
 #     assert pipeline_div_print.dn2_div.read() is not None
 #     assert len(pipeline_div_print.dn2_div.read()) == 10
```

### Comparing `taipy-core-2.2.3/tests/test_taipy.py` & `taipy-core-2.3.0.dev0/tests/test_taipy.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,17 @@
 import pathlib
 import shutil
 from unittest import mock
 
 import pytest
 
 import src.taipy.core.taipy as tp
-from src.taipy.core import Core
-from src.taipy.core._scheduler._scheduler_factory import _SchedulerFactory
+from src.taipy.core import Core, CycleId, JobId, PipelineId, ScenarioId, TaskId
+from src.taipy.core._orchestrator._orchestrator_factory import _OrchestratorFactory
 from src.taipy.core._version._version_manager import _VersionManager
-from src.taipy.core.common.alias import CycleId, JobId, PipelineId, ScenarioId, TaskId
 from src.taipy.core.config.job_config import JobConfig
 from src.taipy.core.config.pipeline_config import PipelineConfig
 from src.taipy.core.config.scenario_config import ScenarioConfig
 from src.taipy.core.cycle._cycle_manager import _CycleManager
 from src.taipy.core.data._data_manager import _DataManager
 from src.taipy.core.exceptions.exceptions import InvalidExportPath
 from src.taipy.core.job._job_manager import _JobManager
@@ -83,15 +82,15 @@
             tp.submit(pipeline, True, True, 60)
             mck.assert_called_once_with(pipeline, force=True, wait=True, timeout=60)
         with mock.patch("src.taipy.core.task._task_manager._TaskManager._submit") as mck:
             tp.submit(task, True, True, 60)
             mck.assert_called_once_with(task, force=True, wait=True, timeout=60)
 
     def test_warning_no_core_service_running(self, scenario):
-        _SchedulerFactory._remove_dispatcher()
+        _OrchestratorFactory._remove_dispatcher()
 
         with pytest.warns(ResourceWarning) as warning:
             with mock.patch("src.taipy.core.scenario._scenario_manager._ScenarioManager._submit"):
                 tp.submit(scenario)
 
         assert len(warning) == 1
         assert warning[0].message.args[0] == "The Core service is NOT running"
@@ -387,31 +386,29 @@
         input_cfg_2 = Config.configure_data_node(id="i2", storage_type="pickle", default_data=2, scope=Scope.SCENARIO)
         output_cfg_2 = Config.configure_data_node(id="o2", storage_type="pickle", scope=Scope.SCENARIO)
         task_cfg_2 = Config.configure_task("t2", print, input_cfg_2, output_cfg_2)
         pipeline_cfg_2 = Config.configure_pipeline("p2", task_cfg_2)
         scenario_cfg_2 = Config.configure_scenario("s2", pipeline_cfg_2, Frequency.DAILY)
 
         scenario_1 = tp.create_scenario(scenario_cfg_1)
-        job_1 = tp.submit(scenario_1)
-        job_1 = job_1[scenario_1.p1.id][0]
+        job_1 = tp.submit(scenario_1)[0]
 
         # Export scenario 1
         tp.export_scenario(scenario_1.id, "./tmp/exp_scenario_1")
         assert sorted(os.listdir("./tmp/exp_scenario_1/data_nodes")) == sorted(
             [f"{scenario_1.i1.id}.json", f"{scenario_1.o1.id}.json"]
         )
         assert sorted(os.listdir("./tmp/exp_scenario_1/tasks")) == sorted([f"{scenario_1.t1.id}.json"])
         assert sorted(os.listdir("./tmp/exp_scenario_1/pipelines")) == sorted([f"{scenario_1.p1.id}.json"])
         assert sorted(os.listdir("./tmp/exp_scenario_1/scenarios")) == sorted([f"{scenario_1.id}.json"])
         assert sorted(os.listdir("./tmp/exp_scenario_1/jobs")) == sorted([f"{job_1.id}.json"])
         assert sorted(os.listdir("./tmp/exp_scenario_1/cycles")) == sorted([f"{scenario_1.cycle.id}.json"])
 
         scenario_2 = tp.create_scenario(scenario_cfg_2)
-        job_2 = tp.submit(scenario_2)
-        job_2 = job_2[scenario_2.p2.id][0]
+        job_2 = tp.submit(scenario_2)[0]
 
         # Export scenario 2
         scenario_2.export(pathlib.Path.cwd() / "./tmp/exp_scenario_2")
         assert sorted(os.listdir("./tmp/exp_scenario_2/data_nodes")) == sorted(
             [f"{scenario_2.i2.id}.json", f"{scenario_2.o2.id}.json"]
         )
         assert sorted(os.listdir("./tmp/exp_scenario_2/tasks")) == sorted([f"{scenario_2.t2.id}.json"])
@@ -495,7 +492,71 @@
         expected_parents = {}
         parents = tp.get_parents(scenario)
         assert_result_parents_and_expected_parents(parents, expected_parents)
 
         expected_parents = {}
         parents = tp.get_parents(scenario.cycle)
         assert_result_parents_and_expected_parents(parents, expected_parents)
+
+    def test_get_cycles_scenarios(self):
+        scenario_cfg_1 = Config.configure_scenario(
+            "s1",
+            [],
+            Frequency.DAILY,
+        )
+        scenario_cfg_2 = Config.configure_scenario("s2", [], Frequency.WEEKLY)
+        scenario_cfg_3 = Config.configure_scenario("s3", [], Frequency.MONTHLY)
+        scenario_cfg_4 = Config.configure_scenario("s4", [], Frequency.YEARLY)
+        scenario_cfg_5 = Config.configure_scenario("s5", [], None)
+
+        now = datetime.datetime.now()
+        scenario_1_1 = tp.create_scenario(scenario_cfg_1, now)
+        scenario_1_2 = tp.create_scenario(scenario_cfg_1, datetime.datetime.now())
+        scenario_1_3 = tp.create_scenario(scenario_cfg_1, now + datetime.timedelta(days=1))
+        scenario_1_4 = tp.create_scenario(scenario_cfg_1, now + datetime.timedelta(days=8))
+        scenario_1_5 = tp.create_scenario(scenario_cfg_1, now + datetime.timedelta(days=25))
+        scenario_2 = tp.create_scenario(scenario_cfg_2)
+        scenario_3 = tp.create_scenario(scenario_cfg_3)
+        scenario_4 = tp.create_scenario(scenario_cfg_4)
+        scenario_5_1 = tp.create_scenario(scenario_cfg_5)
+        scenario_5_2 = tp.create_scenario(scenario_cfg_5)
+        scenario_5_3 = tp.create_scenario(scenario_cfg_5)
+
+        expected_cycles_scenarios = {
+            scenario_1_1.cycle: [scenario_1_1.id, scenario_1_2.id],
+            scenario_1_3.cycle: [scenario_1_3.id],
+            scenario_1_4.cycle: [scenario_1_4.id],
+            scenario_1_5.cycle: [scenario_1_5.id],
+            scenario_2.cycle: [scenario_2.id],
+            scenario_3.cycle: [scenario_3.id],
+            scenario_4.cycle: [scenario_4.id],
+            None: [scenario_5_1.id, scenario_5_2.id, scenario_5_3.id],
+        }
+
+        cycles_scenarios = tp.get_cycles_scenarios()
+
+        assert expected_cycles_scenarios.keys() == cycles_scenarios.keys()
+        for cycle, scenarios in cycles_scenarios.items():
+            expected_scenarios = expected_cycles_scenarios[cycle]
+            assert sorted([scenario.id for scenario in scenarios]) == sorted(expected_scenarios)
+
+    def test_get_entities_by_config_id(self):
+        scenario_config_1 = Config.configure_scenario("s1", pipeline_configs=[])
+        scenario_config_2 = Config.configure_scenario("s2", pipeline_configs=[])
+
+        s_1_1 = tp.create_scenario(scenario_config_1)
+        s_1_2 = tp.create_scenario(scenario_config_1)
+        s_1_3 = tp.create_scenario(scenario_config_1)
+
+        assert len(tp.get_scenarios()) == 3
+
+        s_2_1 = tp.create_scenario(scenario_config_2)
+        s_2_2 = tp.create_scenario(scenario_config_2)
+        assert len(tp.get_scenarios()) == 5
+
+        s1_scenarios = tp.get_entities_by_config_id(scenario_config_1.id)
+        assert len(s1_scenarios) == 3
+        assert sorted([s_1_1.id, s_1_2.id, s_1_3.id]) == sorted([scenario.id for scenario in s1_scenarios])
+
+        s2_scenarios = tp.get_entities_by_config_id(scenario_config_2.id)
+        assert len(s2_scenarios) == 2
+        assert sorted([s_2_1.id, s_2_2.id]) == sorted([scenario.id for scenario in s2_scenarios])
```

