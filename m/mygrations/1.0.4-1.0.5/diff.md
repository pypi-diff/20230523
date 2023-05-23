# Comparing `tmp/mygrations-1.0.4.tar.gz` & `tmp/mygrations-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mygrations-1.0.4.tar", last modified: Wed Nov  2 10:46:02 2022, max compression
+gzip compressed data, was "mygrations-1.0.5.tar", last modified: Tue May 23 17:34:06 2023, max compression
```

## Comparing `mygrations-1.0.4.tar` & `mygrations-1.0.5.tar`

### file list

```diff
@@ -1,225 +1,225 @@
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.487293 mygrations-1.0.4/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1065 2021-10-09 17:05:45.000000 mygrations-1.0.4/LICENSE.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    11940 2022-11-02 10:46:02.487293 mygrations-1.0.4/PKG-INFO
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    11241 2022-04-10 02:22:10.000000 mygrations-1.0.4/README.md
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.431294 mygrations-1.0.4/mygrations/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       22 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.431294 mygrations-1.0.4/mygrations/core/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.435294 mygrations-1.0.4/mygrations/core/commands/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      557 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/commands/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      627 2022-04-10 11:02:41.000000 mygrations-1.0.4/mygrations/core/commands/apply.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5197 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/commands/base.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      979 2022-04-10 11:03:16.000000 mygrations-1.0.4/mygrations/core/commands/check.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2488 2022-04-10 11:02:36.000000 mygrations-1.0.4/mygrations/core/commands/plan.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2731 2022-04-10 11:02:19.000000 mygrations-1.0.4/mygrations/core/commands/plan_export.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      510 2022-04-10 11:02:26.000000 mygrations-1.0.4/mygrations/core/commands/version.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.443294 mygrations-1.0.4/mygrations/core/definitions/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      539 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/base.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.451294 mygrations-1.0.4/mygrations/core/definitions/columns/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      102 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/columns/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     9401 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/columns/column.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2143 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/columns/column_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2405 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/columns/date.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2125 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/columns/enum.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      808 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/columns/enum_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5152 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/columns/numeric.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3140 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/columns/numeric_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4669 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/columns/string.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4498 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/columns/string_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4860 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/constraint.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1181 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/constraint_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    17791 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/database.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4061 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/index.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1651 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/index_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2151 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/option.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      431 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/option_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2654 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/rows.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    26764 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/table.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4180 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/definitions/table_test.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.463294 mygrations-1.0.4/mygrations/core/operations/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/operations/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1578 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/operations/add_column.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      388 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/operations/add_column_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      509 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/operations/add_constraint.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      503 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/operations/add_constraint_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      448 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/operations/add_index.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      348 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/operations/add_index_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      861 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/operations/add_row.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      375 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/operations/add_row_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/operations/add_table.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      731 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/operations/alter_table.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      922 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/operations/alter_table_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      478 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/operations/change_column.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      311 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/operations/change_column_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      537 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/operations/change_constraint.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      526 2022-04-10 02:22:10.000000 mygrations-1.0.4/mygrations/core/operations/change_constraint_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      465 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/operations/change_index.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      350 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/operations/change_index_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      950 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/operations/change_row.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      382 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/operations/change_row_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1189 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/operations/create_table.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1017 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/operations/create_table_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      154 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/operations/disable_checks.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      209 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/operations/disable_checks_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      155 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/operations/enable_checks.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      205 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/operations/enable_checks_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      459 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/operations/remove_column.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      317 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/operations/remove_column_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      513 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/operations/remove_constraint.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      355 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/operations/remove_constraint_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      531 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/operations/remove_index.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      435 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/operations/remove_index_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      618 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/operations/remove_row.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      223 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/operations/remove_row_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      451 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/operations/remove_table.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      212 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/operations/remove_table_test.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.463294 mygrations-1.0.4/mygrations/core/parse/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/parse/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3792 2022-11-02 10:35:31.000000 mygrations-1.0.4/mygrations/core/parse/parser.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3006 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/parse/rule_base.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3841 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/parse/rule_children.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2581 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/parse/rule_children_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5448 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/parse/rule_delimited.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2626 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/parse/rule_delimited_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1760 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/parse/rule_literal.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1532 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/parse/rule_literal_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1783 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/parse/rule_regexp.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1789 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/core/parse/rule_regexp_test.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.463294 mygrations-1.0.4/mygrations/drivers/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/drivers/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.463294 mygrations-1.0.4/mygrations/drivers/pymysql/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/drivers/pymysql/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2945 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/drivers/pymysql/pymysql.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.463294 mygrations-1.0.4/mygrations/formats/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:17:58.000000 mygrations-1.0.4/mygrations/formats/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.463294 mygrations-1.0.4/mygrations/formats/mysql/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:17:58.000000 mygrations-1.0.4/mygrations/formats/mysql/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.463294 mygrations-1.0.4/mygrations/formats/mysql/db_reader/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:17:58.000000 mygrations-1.0.4/mygrations/formats/mysql/db_reader/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3339 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/db_reader/database.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.467294 mygrations-1.0.4/mygrations/formats/mysql/definitions/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      162 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/definitions/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.467294 mygrations-1.0.4/mygrations/formats/mysql/definitions/columns/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      151 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/definitions/columns/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1260 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/definitions/columns/date.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1260 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/definitions/columns/enum.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1275 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/definitions/columns/numeric.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1270 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/definitions/columns/string.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      517 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/definitions/constraint.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      634 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/definitions/constraint_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      113 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/definitions/database.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       98 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/definitions/index.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       93 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/definitions/rows.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     9343 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/definitions/table.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.467294 mygrations-1.0.4/mygrations/formats/mysql/file_reader/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      126 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2674 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/comment_parser.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3828 2022-11-02 10:37:23.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/create_parser.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3764 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/create_parser_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3830 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/database.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6409 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/database_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1856 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/insert_parser.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2143 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/insert_parser_test.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.471294 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      711 2022-11-02 10:38:24.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3435 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/constraint_foreign.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     8342 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/constraint_foreign_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      977 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/index_key.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2064 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/index_key_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      815 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/index_primary.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1434 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/index_primary_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1039 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/index_unique.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2258 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/index_unique_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      739 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/insert_values.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1638 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/insert_values_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      639 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/table_option.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2061 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/table_options_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2693 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4664 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_character.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2717 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_character_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4543 2022-11-02 10:35:17.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_datetime.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      767 2022-11-02 10:35:39.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_datetime_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2486 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_decimal.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2224 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_decimal_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2998 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_enum.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2161 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_enum_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2676 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_numeric.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2633 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_numeric_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1381 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_plain.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1616 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_plain_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3693 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_text.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1727 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_text_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5702 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/reader.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1387 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/file_reader/reader_test.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.471294 mygrations-1.0.4/mygrations/formats/mysql/file_writer/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:17:58.000000 mygrations-1.0.4/mygrations/formats/mysql/file_writer/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:17:58.000000 mygrations-1.0.4/mygrations/formats/mysql/file_writer/writer.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.471294 mygrations-1.0.4/mygrations/formats/mysql/mygrations/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    16995 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/mygration.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.475293 mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1536 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/add_column.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      495 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/add_constraint.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      433 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/add_key.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:17:58.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/add_table.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      777 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/alter_table.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      506 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/change_column.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      566 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/change_constraint.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      480 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/change_key.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1416 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/create_table.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      154 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/disable_checks.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      155 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/enable_checks.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      485 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/remove_column.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      540 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/remove_constraint.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      544 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/remove_key.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      524 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/remove_table.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      594 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/row_delete.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      842 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/row_insert.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      913 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/row_update.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4057 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/formats/mysql/mygrations/row_mygration.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.479293 mygrations-1.0.4/mygrations/helpers/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:17:58.000000 mygrations-1.0.4/mygrations/helpers/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1369 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/helpers/db_credentials.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6043 2022-04-10 02:17:58.000000 mygrations-1.0.4/mygrations/helpers/dotenv.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     9362 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/helpers/dotenv_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      719 2022-04-10 11:03:32.000000 mygrations-1.0.4/mygrations/mygrate.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.479293 mygrations-1.0.4/mygrations/tests/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.483293 mygrations-1.0.4/mygrations/tests/integration/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/integration/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2134 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/integration/add_conflicting_fks_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1119 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/integration/add_only_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2097 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/integration/backslashes_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    18662 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/integration/database_unfulfilled_fks_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2809 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/integration/mygrate_nulls_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1853 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/integration/mygrate_rows_different_types_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5687 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/integration/mygrate_rows_simple_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3826 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/integration/regression_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    10730 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/integration/simple_modify_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2407 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/integration/table_constraint_regressions_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3250 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/integration/table_decimal_false_positives_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4532 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/integration/table_difference_columns_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6217 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/integration/table_difference_keys_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2782 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/integration/table_operations_column_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3079 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/integration/table_operations_constraints_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2414 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/integration/table_operations_key_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2045 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/integration/table_return_create_test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4933 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/integration/table_text_false_positives_test.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.483293 mygrations-1.0.4/mygrations/tests/mocks/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/mocks/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.483293 mygrations-1.0.4/mygrations/tests/mocks/db/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/mocks/db/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.483293 mygrations-1.0.4/mygrations/tests/mocks/db/mysql/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/mocks/db/mysql/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4255 2022-04-10 02:22:11.000000 mygrations-1.0.4/mygrations/tests/mocks/db/mysql/db_structure.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-02 10:46:02.431294 mygrations-1.0.4/mygrations.egg-info/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    11940 2022-11-02 10:46:02.000000 mygrations-1.0.4/mygrations.egg-info/PKG-INFO
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     9574 2022-11-02 10:46:02.000000 mygrations-1.0.4/mygrations.egg-info/SOURCES.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        1 2022-11-02 10:46:02.000000 mygrations-1.0.4/mygrations.egg-info/dependency_links.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        8 2022-11-02 10:46:02.000000 mygrations-1.0.4/mygrations.egg-info/requires.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       11 2022-11-02 10:46:02.000000 mygrations-1.0.4/mygrations.egg-info/top_level.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       79 2022-11-02 10:46:02.487293 mygrations-1.0.4/setup.cfg
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1605 2022-11-02 10:37:53.000000 mygrations-1.0.4/setup.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.111560 mygrations-1.0.5/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1065 2021-10-09 17:05:45.000000 mygrations-1.0.5/LICENSE.txt
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    11940 2023-05-23 17:34:06.111560 mygrations-1.0.5/PKG-INFO
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    11241 2022-04-10 02:22:10.000000 mygrations-1.0.5/README.md
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.075560 mygrations-1.0.5/mygrations/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       22 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/__init__.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.075560 mygrations-1.0.5/mygrations/core/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/__init__.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.079560 mygrations-1.0.5/mygrations/core/commands/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      557 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/commands/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      627 2022-04-10 11:02:41.000000 mygrations-1.0.5/mygrations/core/commands/apply.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5197 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/commands/base.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      979 2022-04-10 11:03:16.000000 mygrations-1.0.5/mygrations/core/commands/check.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2488 2022-04-10 11:02:36.000000 mygrations-1.0.5/mygrations/core/commands/plan.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2731 2022-04-10 11:02:19.000000 mygrations-1.0.5/mygrations/core/commands/plan_export.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      510 2022-04-10 11:02:26.000000 mygrations-1.0.5/mygrations/core/commands/version.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.083560 mygrations-1.0.5/mygrations/core/definitions/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      539 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/base.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.083560 mygrations-1.0.5/mygrations/core/definitions/columns/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      102 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/columns/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     9401 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/columns/column.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2143 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/columns/column_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2405 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/columns/date.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2125 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/columns/enum.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      808 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/columns/enum_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5152 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/columns/numeric.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3140 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/columns/numeric_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4669 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/columns/string.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4498 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/columns/string_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4860 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/constraint.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1181 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/constraint_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    17791 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/database.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4061 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/index.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1651 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/index_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2151 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/option.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      431 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/option_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2654 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/rows.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    26764 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/table.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4180 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/definitions/table_test.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.091560 mygrations-1.0.5/mygrations/core/operations/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/operations/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1578 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/operations/add_column.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      388 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/operations/add_column_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      509 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/operations/add_constraint.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      503 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/operations/add_constraint_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      448 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/operations/add_index.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      348 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/operations/add_index_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      861 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/operations/add_row.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      375 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/operations/add_row_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/operations/add_table.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      731 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/operations/alter_table.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      922 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/operations/alter_table_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      478 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/operations/change_column.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      311 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/operations/change_column_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      537 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/operations/change_constraint.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      526 2022-04-10 02:22:10.000000 mygrations-1.0.5/mygrations/core/operations/change_constraint_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      465 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/operations/change_index.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      350 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/operations/change_index_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      950 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/operations/change_row.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      382 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/operations/change_row_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1189 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/operations/create_table.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1017 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/operations/create_table_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      154 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/operations/disable_checks.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      209 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/operations/disable_checks_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      155 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/operations/enable_checks.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      205 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/operations/enable_checks_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      459 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/operations/remove_column.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      317 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/operations/remove_column_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      513 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/operations/remove_constraint.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      355 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/operations/remove_constraint_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      531 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/operations/remove_index.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      435 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/operations/remove_index_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      618 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/operations/remove_row.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      223 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/operations/remove_row_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      451 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/operations/remove_table.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      212 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/operations/remove_table_test.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.091560 mygrations-1.0.5/mygrations/core/parse/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/parse/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3792 2022-11-02 10:35:31.000000 mygrations-1.0.5/mygrations/core/parse/parser.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3006 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/parse/rule_base.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3841 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/parse/rule_children.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2581 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/parse/rule_children_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5448 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/parse/rule_delimited.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2626 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/parse/rule_delimited_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1760 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/parse/rule_literal.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1532 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/parse/rule_literal_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1783 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/parse/rule_regexp.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1789 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/core/parse/rule_regexp_test.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.091560 mygrations-1.0.5/mygrations/drivers/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/drivers/__init__.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.091560 mygrations-1.0.5/mygrations/drivers/pymysql/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/drivers/pymysql/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2945 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/drivers/pymysql/pymysql.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.091560 mygrations-1.0.5/mygrations/formats/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:17:58.000000 mygrations-1.0.5/mygrations/formats/__init__.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.095560 mygrations-1.0.5/mygrations/formats/mysql/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:17:58.000000 mygrations-1.0.5/mygrations/formats/mysql/__init__.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.095560 mygrations-1.0.5/mygrations/formats/mysql/db_reader/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:17:58.000000 mygrations-1.0.5/mygrations/formats/mysql/db_reader/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3339 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/db_reader/database.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.095560 mygrations-1.0.5/mygrations/formats/mysql/definitions/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      162 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/definitions/__init__.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.095560 mygrations-1.0.5/mygrations/formats/mysql/definitions/columns/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      151 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/definitions/columns/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1260 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/definitions/columns/date.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1260 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/definitions/columns/enum.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1275 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/definitions/columns/numeric.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1270 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/definitions/columns/string.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      517 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/definitions/constraint.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      634 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/definitions/constraint_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      113 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/definitions/database.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       98 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/definitions/index.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       93 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/definitions/rows.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     9343 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/definitions/table.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.099560 mygrations-1.0.5/mygrations/formats/mysql/file_reader/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      126 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2674 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/comment_parser.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3828 2022-11-02 10:37:23.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/create_parser.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3764 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/create_parser_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3830 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/database.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6409 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/database_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1856 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/insert_parser.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2143 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/insert_parser_test.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.103560 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      711 2022-11-02 10:38:24.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3435 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/constraint_foreign.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     8342 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/constraint_foreign_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      977 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/index_key.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2064 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/index_key_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      815 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/index_primary.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1434 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/index_primary_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1039 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/index_unique.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2258 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/index_unique_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      739 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/insert_values.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1638 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/insert_values_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      639 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/table_option.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2061 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/table_options_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2693 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4664 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_character.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2717 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_character_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4543 2022-11-02 10:35:17.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_datetime.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      767 2022-11-02 10:35:39.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_datetime_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2486 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_decimal.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2224 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_decimal_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2998 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_enum.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2161 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_enum_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2676 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_numeric.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2633 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_numeric_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1471 2023-05-23 17:33:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_plain.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1616 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_plain_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3693 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_text.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1727 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_text_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5702 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/reader.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1387 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/file_reader/reader_test.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.103560 mygrations-1.0.5/mygrations/formats/mysql/file_writer/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:17:58.000000 mygrations-1.0.5/mygrations/formats/mysql/file_writer/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:17:58.000000 mygrations-1.0.5/mygrations/formats/mysql/file_writer/writer.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.103560 mygrations-1.0.5/mygrations/formats/mysql/mygrations/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    16995 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/mygration.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.107560 mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1536 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/add_column.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      495 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/add_constraint.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      433 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/add_key.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:17:58.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/add_table.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      777 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/alter_table.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      506 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/change_column.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      566 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/change_constraint.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      480 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/change_key.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1416 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/create_table.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      154 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/disable_checks.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      155 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/enable_checks.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      485 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/remove_column.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      540 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/remove_constraint.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      544 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/remove_key.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      524 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/remove_table.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      594 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/row_delete.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      842 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/row_insert.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      913 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/row_update.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4057 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/formats/mysql/mygrations/row_mygration.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.107560 mygrations-1.0.5/mygrations/helpers/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:17:58.000000 mygrations-1.0.5/mygrations/helpers/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1369 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/helpers/db_credentials.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6043 2022-04-10 02:17:58.000000 mygrations-1.0.5/mygrations/helpers/dotenv.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     9362 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/helpers/dotenv_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      719 2022-04-10 11:03:32.000000 mygrations-1.0.5/mygrations/mygrate.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.107560 mygrations-1.0.5/mygrations/tests/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/__init__.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.111560 mygrations-1.0.5/mygrations/tests/integration/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/integration/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2134 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/integration/add_conflicting_fks_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1119 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/integration/add_only_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2097 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/integration/backslashes_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    18662 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/integration/database_unfulfilled_fks_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2809 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/integration/mygrate_nulls_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1853 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/integration/mygrate_rows_different_types_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5687 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/integration/mygrate_rows_simple_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3826 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/integration/regression_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    10730 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/integration/simple_modify_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2407 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/integration/table_constraint_regressions_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3250 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/integration/table_decimal_false_positives_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4532 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/integration/table_difference_columns_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6217 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/integration/table_difference_keys_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2782 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/integration/table_operations_column_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3079 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/integration/table_operations_constraints_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2414 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/integration/table_operations_key_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2045 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/integration/table_return_create_test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4933 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/integration/table_text_false_positives_test.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.111560 mygrations-1.0.5/mygrations/tests/mocks/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/mocks/__init__.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.111560 mygrations-1.0.5/mygrations/tests/mocks/db/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/mocks/db/__init__.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.111560 mygrations-1.0.5/mygrations/tests/mocks/db/mysql/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/mocks/db/mysql/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4255 2022-04-10 02:22:11.000000 mygrations-1.0.5/mygrations/tests/mocks/db/mysql/db_structure.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 17:34:06.075560 mygrations-1.0.5/mygrations.egg-info/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    11940 2023-05-23 17:34:06.000000 mygrations-1.0.5/mygrations.egg-info/PKG-INFO
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     9574 2023-05-23 17:34:06.000000 mygrations-1.0.5/mygrations.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        1 2023-05-23 17:34:06.000000 mygrations-1.0.5/mygrations.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        8 2023-05-23 17:34:06.000000 mygrations-1.0.5/mygrations.egg-info/requires.txt
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       11 2023-05-23 17:34:06.000000 mygrations-1.0.5/mygrations.egg-info/top_level.txt
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       79 2023-05-23 17:34:06.111560 mygrations-1.0.5/setup.cfg
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1605 2023-05-23 17:33:21.000000 mygrations-1.0.5/setup.py
```

### Comparing `mygrations-1.0.4/LICENSE.txt` & `mygrations-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/PKG-INFO` & `mygrations-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mygrations
-Version: 1.0.4
+Version: 1.0.5
 Summary: A general purpose migration tool for managing MySQL updates
 Home-page: https://github.com/cmancone/mygrations
 Download-URL: https://github.com/cmancone/mygrations/archive/v1.0.0.tar.gz
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 License: MIT
 Keywords: setuptools development migrations mysql
```

### Comparing `mygrations-1.0.4/README.md` & `mygrations-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/commands/__init__.py` & `mygrations-1.0.5/mygrations/core/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/commands/apply.py` & `mygrations-1.0.5/mygrations/core/commands/apply.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/commands/base.py` & `mygrations-1.0.5/mygrations/core/commands/base.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/commands/check.py` & `mygrations-1.0.5/mygrations/core/commands/check.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/commands/plan.py` & `mygrations-1.0.5/mygrations/core/commands/plan.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/commands/plan_export.py` & `mygrations-1.0.5/mygrations/core/commands/plan_export.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/definitions/base.py` & `mygrations-1.0.5/mygrations/core/definitions/base.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/definitions/columns/column.py` & `mygrations-1.0.5/mygrations/core/definitions/columns/column.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/definitions/columns/column_test.py` & `mygrations-1.0.5/mygrations/core/definitions/columns/column_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/definitions/columns/date.py` & `mygrations-1.0.5/mygrations/core/definitions/columns/date.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/definitions/columns/enum.py` & `mygrations-1.0.5/mygrations/core/definitions/columns/enum.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/definitions/columns/enum_test.py` & `mygrations-1.0.5/mygrations/core/definitions/columns/enum_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/definitions/columns/numeric.py` & `mygrations-1.0.5/mygrations/core/definitions/columns/numeric.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/definitions/columns/numeric_test.py` & `mygrations-1.0.5/mygrations/core/definitions/columns/numeric_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/definitions/columns/string.py` & `mygrations-1.0.5/mygrations/core/definitions/columns/string.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/definitions/columns/string_test.py` & `mygrations-1.0.5/mygrations/core/definitions/columns/string_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/definitions/constraint.py` & `mygrations-1.0.5/mygrations/core/definitions/constraint.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/definitions/constraint_test.py` & `mygrations-1.0.5/mygrations/core/definitions/constraint_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/definitions/database.py` & `mygrations-1.0.5/mygrations/core/definitions/database.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/definitions/index.py` & `mygrations-1.0.5/mygrations/core/definitions/index.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/definitions/index_test.py` & `mygrations-1.0.5/mygrations/core/definitions/index_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/definitions/option.py` & `mygrations-1.0.5/mygrations/core/definitions/option.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/definitions/rows.py` & `mygrations-1.0.5/mygrations/core/definitions/rows.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/definitions/table.py` & `mygrations-1.0.5/mygrations/core/definitions/table.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/definitions/table_test.py` & `mygrations-1.0.5/mygrations/core/definitions/table_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/operations/add_column.py` & `mygrations-1.0.5/mygrations/core/operations/add_column.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/operations/add_row.py` & `mygrations-1.0.5/mygrations/core/operations/add_row.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/operations/alter_table.py` & `mygrations-1.0.5/mygrations/core/operations/alter_table.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/operations/alter_table_test.py` & `mygrations-1.0.5/mygrations/core/operations/alter_table_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/operations/change_constraint.py` & `mygrations-1.0.5/mygrations/core/operations/change_constraint.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/operations/change_constraint_test.py` & `mygrations-1.0.5/mygrations/core/operations/change_constraint_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/operations/change_row.py` & `mygrations-1.0.5/mygrations/core/operations/change_row.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/operations/create_table.py` & `mygrations-1.0.5/mygrations/core/operations/create_table.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/operations/create_table_test.py` & `mygrations-1.0.5/mygrations/core/operations/create_table_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/operations/remove_constraint.py` & `mygrations-1.0.5/mygrations/core/operations/remove_constraint.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/operations/remove_index.py` & `mygrations-1.0.5/mygrations/core/operations/remove_index.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/operations/remove_row.py` & `mygrations-1.0.5/mygrations/core/operations/remove_row.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/parse/parser.py` & `mygrations-1.0.5/mygrations/core/parse/parser.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/parse/rule_base.py` & `mygrations-1.0.5/mygrations/core/parse/rule_base.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/parse/rule_children.py` & `mygrations-1.0.5/mygrations/core/parse/rule_children.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/parse/rule_children_test.py` & `mygrations-1.0.5/mygrations/core/parse/rule_children_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/parse/rule_delimited.py` & `mygrations-1.0.5/mygrations/core/parse/rule_delimited.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/parse/rule_delimited_test.py` & `mygrations-1.0.5/mygrations/core/parse/rule_delimited_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/parse/rule_literal.py` & `mygrations-1.0.5/mygrations/core/parse/rule_literal.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/parse/rule_literal_test.py` & `mygrations-1.0.5/mygrations/core/parse/rule_literal_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/parse/rule_regexp.py` & `mygrations-1.0.5/mygrations/core/parse/rule_regexp.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/core/parse/rule_regexp_test.py` & `mygrations-1.0.5/mygrations/core/parse/rule_regexp_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/drivers/pymysql/pymysql.py` & `mygrations-1.0.5/mygrations/drivers/pymysql/pymysql.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/db_reader/database.py` & `mygrations-1.0.5/mygrations/formats/mysql/db_reader/database.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/definitions/columns/date.py` & `mygrations-1.0.5/mygrations/formats/mysql/definitions/columns/date.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/definitions/columns/enum.py` & `mygrations-1.0.5/mygrations/formats/mysql/definitions/columns/enum.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/definitions/columns/numeric.py` & `mygrations-1.0.5/mygrations/formats/mysql/definitions/columns/numeric.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/definitions/columns/string.py` & `mygrations-1.0.5/mygrations/formats/mysql/definitions/columns/string.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/definitions/constraint.py` & `mygrations-1.0.5/mygrations/formats/mysql/definitions/constraint.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/definitions/constraint_test.py` & `mygrations-1.0.5/mygrations/formats/mysql/definitions/constraint_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/definitions/table.py` & `mygrations-1.0.5/mygrations/formats/mysql/definitions/table.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/comment_parser.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/comment_parser.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/create_parser.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/create_parser.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/create_parser_test.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/create_parser_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/database.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/database.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/database_test.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/database_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/insert_parser.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/insert_parser.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/insert_parser_test.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/insert_parser_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/__init__.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/constraint_foreign.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/constraint_foreign.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/constraint_foreign_test.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/constraint_foreign_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/index_key.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/index_key.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/index_key_test.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/index_key_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/index_primary.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/index_primary.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/index_primary_test.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/index_primary_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/index_unique.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/index_unique.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/index_unique_test.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/index_unique_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/insert_values.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/insert_values.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/insert_values_test.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/insert_values_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/table_option.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/table_option.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/table_options_test.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/table_options_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_character.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_character.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_character_test.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_character_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_datetime.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_datetime.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_datetime_test.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_datetime_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_decimal.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_decimal.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_decimal_test.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_decimal_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_enum.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_enum.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_enum_test.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_enum_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_numeric.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_numeric.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_numeric_test.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_numeric_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_plain.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_plain.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,18 @@
         'name': 'name'
     }, {
         'type': 'regexp',
         'value': '\w+',
         'name': 'type'
     }, {
         'type': 'literal',
+        'value': 'UNSIGNED',
+        'optional': True
+    }, {
+        'type': 'literal',
         'value': 'NOT NULL',
         'optional': True
     }, {
         'type': 'regexp',
         'value': 'DEFAULT ([^\(\s\),]+)',
         'optional': True,
         'name': 'default'
```

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_plain_test.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_plain_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_text.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_text.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/parsers/type_text_test.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/parsers/type_text_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/reader.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/reader.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/file_reader/reader_test.py` & `mygrations-1.0.5/mygrations/formats/mysql/file_reader/reader_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/mygrations/mygration.py` & `mygrations-1.0.5/mygrations/formats/mysql/mygrations/mygration.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/add_column.py` & `mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/add_column.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/alter_table.py` & `mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/alter_table.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/change_constraint.py` & `mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/change_constraint.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/create_table.py` & `mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/create_table.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/remove_constraint.py` & `mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/remove_constraint.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/remove_key.py` & `mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/remove_key.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/remove_table.py` & `mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/remove_table.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/row_delete.py` & `mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/row_delete.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/row_insert.py` & `mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/row_insert.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/mygrations/operations/row_update.py` & `mygrations-1.0.5/mygrations/formats/mysql/mygrations/operations/row_update.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/formats/mysql/mygrations/row_mygration.py` & `mygrations-1.0.5/mygrations/formats/mysql/mygrations/row_mygration.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/helpers/db_credentials.py` & `mygrations-1.0.5/mygrations/helpers/db_credentials.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/helpers/dotenv.py` & `mygrations-1.0.5/mygrations/helpers/dotenv.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/helpers/dotenv_test.py` & `mygrations-1.0.5/mygrations/helpers/dotenv_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/mygrate.py` & `mygrations-1.0.5/mygrations/mygrate.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/tests/integration/add_conflicting_fks_test.py` & `mygrations-1.0.5/mygrations/tests/integration/add_conflicting_fks_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/tests/integration/add_only_test.py` & `mygrations-1.0.5/mygrations/tests/integration/add_only_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/tests/integration/backslashes_test.py` & `mygrations-1.0.5/mygrations/tests/integration/backslashes_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/tests/integration/database_unfulfilled_fks_test.py` & `mygrations-1.0.5/mygrations/tests/integration/database_unfulfilled_fks_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/tests/integration/mygrate_nulls_test.py` & `mygrations-1.0.5/mygrations/tests/integration/mygrate_nulls_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/tests/integration/mygrate_rows_different_types_test.py` & `mygrations-1.0.5/mygrations/tests/integration/mygrate_rows_different_types_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/tests/integration/mygrate_rows_simple_test.py` & `mygrations-1.0.5/mygrations/tests/integration/mygrate_rows_simple_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/tests/integration/regression_test.py` & `mygrations-1.0.5/mygrations/tests/integration/regression_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/tests/integration/simple_modify_test.py` & `mygrations-1.0.5/mygrations/tests/integration/simple_modify_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/tests/integration/table_constraint_regressions_test.py` & `mygrations-1.0.5/mygrations/tests/integration/table_constraint_regressions_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/tests/integration/table_decimal_false_positives_test.py` & `mygrations-1.0.5/mygrations/tests/integration/table_decimal_false_positives_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/tests/integration/table_difference_columns_test.py` & `mygrations-1.0.5/mygrations/tests/integration/table_difference_columns_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/tests/integration/table_difference_keys_test.py` & `mygrations-1.0.5/mygrations/tests/integration/table_difference_keys_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/tests/integration/table_operations_column_test.py` & `mygrations-1.0.5/mygrations/tests/integration/table_operations_column_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/tests/integration/table_operations_constraints_test.py` & `mygrations-1.0.5/mygrations/tests/integration/table_operations_constraints_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/tests/integration/table_operations_key_test.py` & `mygrations-1.0.5/mygrations/tests/integration/table_operations_key_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/tests/integration/table_return_create_test.py` & `mygrations-1.0.5/mygrations/tests/integration/table_return_create_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/tests/integration/table_text_false_positives_test.py` & `mygrations-1.0.5/mygrations/tests/integration/table_text_false_positives_test.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations/tests/mocks/db/mysql/db_structure.py` & `mygrations-1.0.5/mygrations/tests/mocks/db/mysql/db_structure.py`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/mygrations.egg-info/PKG-INFO` & `mygrations-1.0.5/mygrations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mygrations
-Version: 1.0.4
+Version: 1.0.5
 Summary: A general purpose migration tool for managing MySQL updates
 Home-page: https://github.com/cmancone/mygrations
 Download-URL: https://github.com/cmancone/mygrations/archive/v1.0.0.tar.gz
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 License: MIT
 Keywords: setuptools development migrations mysql
```

### Comparing `mygrations-1.0.4/mygrations.egg-info/SOURCES.txt` & `mygrations-1.0.5/mygrations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mygrations-1.0.4/setup.py` & `mygrations-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='mygrations',
-    version='1.0.4',
+    version='1.0.5',
     description='A general purpose migration tool for managing MySQL updates',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/cmancone/mygrations',
     author='Conor Mancone',
     author_email='cmancone@gmail.com',
     license='MIT',
```

