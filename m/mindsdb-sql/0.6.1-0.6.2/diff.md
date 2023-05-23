# Comparing `tmp/mindsdb_sql-0.6.1.tar.gz` & `tmp/mindsdb_sql-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mindsdb_sql-0.6.1.tar", last modified: Fri Apr 21 11:49:27 2023, max compression
+gzip compressed data, was "dist\mindsdb_sql-0.6.2.tar", last modified: Tue May 23 14:41:16 2023, max compression
```

## Comparing `mindsdb_sql-0.6.1.tar` & `mindsdb_sql-0.6.2.tar`

### file list

```diff
@@ -1,141 +1,143 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/
--rw-rw-rw-   0        0        0      535 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     7245 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/mindsdb_sql/
--rw-rw-rw-   0        0        0      365 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/__about__.py
--rw-rw-rw-   0        0        0     1195 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/__init__.py
--rw-rw-rw-   0        0        0      170 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/
--rw-rw-rw-   0        0        0        0 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/
--rw-rw-rw-   0        0        0      537 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/__init__.py
--rw-rw-rw-   0        0        0      842 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/alter_table.py
--rw-rw-rw-   0        0        0     1343 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/base.py
--rw-rw-rw-   0        0        0      460 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/commit_transaction.py
--rw-rw-rw-   0        0        0     2287 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/create.py
--rw-rw-rw-   0        0        0      994 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/delete.py
--rw-rw-rw-   0        0        0      942 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/describe.py
--rw-rw-rw-   0        0        0     3056 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/drop.py
--rw-rw-rw-   0        0        0      659 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/explain.py
--rw-rw-rw-   0        0        0     3099 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/insert.py
--rw-rw-rw-   0        0        0      466 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/rollback_transaction.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/
--rw-rw-rw-   0        0        0      567 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/__init__.py
--rw-rw-rw-   0        0        0     1482 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/case.py
--rw-rw-rw-   0        0        0     1113 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/common_table_expression.py
--rw-rw-rw-   0        0        0     1593 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/constant.py
--rw-rw-rw-   0        0        0     2372 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/identifier.py
--rw-rw-rw-   0        0        0     1381 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/join.py
--rw-rw-rw-   0        0        0      662 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/native_query.py
--rw-rw-rw-   0        0        0     5949 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/operation.py
--rw-rw-rw-   0        0        0      806 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/order_by.py
--rw-rw-rw-   0        0        0      464 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/parameter.py
--rw-rw-rw-   0        0        0     5904 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/select.py
--rw-rw-rw-   0        0        0      504 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/star.py
--rw-rw-rw-   0        0        0      648 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/tuple.py
--rw-rw-rw-   0        0        0      774 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/type_cast.py
--rw-rw-rw-   0        0        0     1178 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/union.py
--rw-rw-rw-   0        0        0     3296 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/set.py
--rw-rw-rw-   0        0        0     2979 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/show.py
--rw-rw-rw-   0        0        0      469 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/start_transaction.py
--rw-rw-rw-   0        0        0     2407 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/update.py
--rw-rw-rw-   0        0        0      639 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/use.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/
--rw-rw-rw-   0        0        0        0 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/
--rw-rw-rw-   0        0        0      720 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/__init__.py
--rw-rw-rw-   0        0        0     1595 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/create_database.py
--rw-rw-rw-   0        0        0      953 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/create_file.py
--rw-rw-rw-   0        0        0     2078 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/create_job.py
--rw-rw-rw-   0        0        0     1201 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py
--rw-rw-rw-   0        0        0     5361 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py
--rw-rw-rw-   0        0        0     1534 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/create_view.py
--rw-rw-rw-   0        0        0      704 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py
--rw-rw-rw-   0        0        0      713 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py
--rw-rw-rw-   0        0        0      737 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py
--rw-rw-rw-   0        0        0      692 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/drop_job.py
--rw-rw-rw-   0        0        0      708 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py
--rw-rw-rw-   0        0        0      906 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py
--rw-rw-rw-   0        0        0     1313 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/evaluate.py
--rw-rw-rw-   0        0        0      223 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/finetune_predictor.py
--rw-rw-rw-   0        0        0      359 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/latest.py
--rw-rw-rw-   0        0        0     8101 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/lexer.py
--rw-rw-rw-   0        0        0    44300 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/parser.py
--rw-rw-rw-   0        0        0      311 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/retrain_predictor.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mysql/
--rw-rw-rw-   0        0        0       67 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mysql/__init__.py
--rw-rw-rw-   0        0        0     1046 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mysql/lexer.py
--rw-rw-rw-   0        0        0    29491 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mysql/parser.py
--rw-rw-rw-   0        0        0      904 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mysql/show_index.py
--rw-rw-rw-   0        0        0      686 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mysql/variable.py
--rw-rw-rw-   0        0        0     6226 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/lexer.py
--rw-rw-rw-   0        0        0      751 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/logger.py
--rw-rw-rw-   0        0        0    21382 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/parser.py
--rw-rw-rw-   0        0        0     2497 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/mindsdb_sql/planner/
--rw-rw-rw-   0        0        0      150 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/planner/__init__.py
--rw-rw-rw-   0        0        0      878 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/planner/query_plan.py
--rw-rw-rw-   0        0        0    50020 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/planner/query_planner.py
--rw-rw-rw-   0        0        0    21367 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/planner/query_prepare.py
--rw-rw-rw-   0        0        0      536 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/planner/step_result.py
--rw-rw-rw-   0        0        0     8276 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/planner/steps.py
--rw-rw-rw-   0        0        0     2981 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/planner/ts_utils.py
--rw-rw-rw-   0        0        0    17886 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/planner/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/mindsdb_sql/render/
--rw-rw-rw-   0        0        0        0 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/render/__init__.py
--rw-rw-rw-   0        0        0    20561 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/mindsdb_sql/render/sqlalchemy_render.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/mindsdb_sql.egg-info/
--rw-rw-rw-   0        0        0      535 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/mindsdb_sql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5187 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/mindsdb_sql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/mindsdb_sql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/mindsdb_sql.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/mindsdb_sql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0      843 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/tests/
--rw-rw-rw-   0        0        0        0 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/tests/test_parser/
--rw-rw-rw-   0        0        0        0 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/
--rw-rw-rw-   0        0        0        0 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/__init__.py
--rw-rw-rw-   0        0        0      776 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_ast.py
--rw-rw-rw-   0        0        0    11910 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_base_lexer.py
--rw-rw-rw-   0        0        0      223 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_base_sql.py
--rw-rw-rw-   0        0        0     1480 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_create.py
--rw-rw-rw-   0        0        0     2481 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_ddl.py
--rw-rw-rw-   0        0        0     1075 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_delete.py
--rw-rw-rw-   0        0        0     1094 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_describe.py
--rw-rw-rw-   0        0        0     2426 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_insert.py
--rw-rw-rw-   0        0        0     6945 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_misc_sql_queries.py
--rw-rw-rw-   0        0        0     3625 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_select_common_table_expression.py
--rw-rw-rw-   0        0        0    24799 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_select_operations.py
--rw-rw-rw-   0        0        0    45563 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_select_structure.py
--rw-rw-rw-   0        0        0    13620 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_show.py
--rw-rw-rw-   0        0        0     3114 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_union.py
--rw-rw-rw-   0        0        0     2462 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_update.py
--rw-rw-rw-   0        0        0      514 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_use.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/
--rw-rw-rw-   0        0        0        0 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/__init__.py
--rw-rw-rw-   0        0        0      605 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_create_file.py
--rw-rw-rw-   0        0        0     4203 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_create_integration.py
--rw-rw-rw-   0        0        0     6617 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_create_predictor.py
--rw-rw-rw-   0        0        0     2651 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_create_view.py
--rw-rw-rw-   0        0        0      520 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_drop_dataset.py
--rw-rw-rw-   0        0        0      861 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_drop_datasource.py
--rw-rw-rw-   0        0        0      866 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_drop_integration.py
--rw-rw-rw-   0        0        0     1708 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_drop_predictor.py
--rw-rw-rw-   0        0        0     1824 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_evaluate.py
--rw-rw-rw-   0        0        0     1339 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_finetune_predictor.py
--rw-rw-rw-   0        0        0     2073 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_jobs.py
--rw-rw-rw-   0        0        0     1587 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_ml_engine.py
--rw-rw-rw-   0        0        0     2242 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_retrain_predictor.py
--rw-rw-rw-   0        0        0     3572 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_selects.py
--rw-rw-rw-   0        0        0     1226 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_show_mindsdb.py
--rw-rw-rw-   0        0        0      959 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_timeseries.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mysql/
--rw-rw-rw-   0        0        0        0 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mysql/__init__.py
--rw-rw-rw-   0        0        0      714 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mysql/test_mysql_lexer.py
--rw-rw-rw-   0        0        0     3050 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_parser/test_mysql/test_mysql_parser.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:49:27.000000 mindsdb_sql-0.6.1/tests/test_render/
--rw-rw-rw-   0        0        0        0 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_render/__init__.py
--rw-rw-rw-   0        0        0     6391 2023-04-21 11:48:46.000000 mindsdb_sql-0.6.1/tests/test_render/test_sqlalchemyrender.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/
+-rw-rw-rw-   0        0        0      535 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7245 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql/
+-rw-rw-rw-   0        0        0      365 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/__about__.py
+-rw-rw-rw-   0        0        0     1195 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/__init__.py
+-rw-rw-rw-   0        0        0      170 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/
+-rw-rw-rw-   0        0        0        0 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/
+-rw-rw-rw-   0        0        0      537 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/alter_table.py
+-rw-rw-rw-   0        0        0     1343 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/base.py
+-rw-rw-rw-   0        0        0      460 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/commit_transaction.py
+-rw-rw-rw-   0        0        0     2287 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/create.py
+-rw-rw-rw-   0        0        0      994 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/delete.py
+-rw-rw-rw-   0        0        0      942 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/describe.py
+-rw-rw-rw-   0        0        0     3056 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/drop.py
+-rw-rw-rw-   0        0        0      659 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/explain.py
+-rw-rw-rw-   0        0        0     3260 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/insert.py
+-rw-rw-rw-   0        0        0      466 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/rollback_transaction.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/
+-rw-rw-rw-   0        0        0      567 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/__init__.py
+-rw-rw-rw-   0        0        0     1482 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/case.py
+-rw-rw-rw-   0        0        0     1113 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/common_table_expression.py
+-rw-rw-rw-   0        0        0     1593 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/constant.py
+-rw-rw-rw-   0        0        0     3136 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/identifier.py
+-rw-rw-rw-   0        0        0     1381 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/join.py
+-rw-rw-rw-   0        0        0      662 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/native_query.py
+-rw-rw-rw-   0        0        0     5949 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/operation.py
+-rw-rw-rw-   0        0        0      806 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/order_by.py
+-rw-rw-rw-   0        0        0      464 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/parameter.py
+-rw-rw-rw-   0        0        0     5904 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/select.py
+-rw-rw-rw-   0        0        0      504 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/star.py
+-rw-rw-rw-   0        0        0      648 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/tuple.py
+-rw-rw-rw-   0        0        0      774 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/type_cast.py
+-rw-rw-rw-   0        0        0     1178 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/union.py
+-rw-rw-rw-   0        0        0     3296 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/set.py
+-rw-rw-rw-   0        0        0     2979 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/show.py
+-rw-rw-rw-   0        0        0      469 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/start_transaction.py
+-rw-rw-rw-   0        0        0     2407 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/update.py
+-rw-rw-rw-   0        0        0      639 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/use.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/
+-rw-rw-rw-   0        0        0        0 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/
+-rw-rw-rw-   0        0        0      769 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/__init__.py
+-rw-rw-rw-   0        0        0     1818 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/chatbot.py
+-rw-rw-rw-   0        0        0     1595 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_database.py
+-rw-rw-rw-   0        0        0      953 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_file.py
+-rw-rw-rw-   0        0        0     2078 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_job.py
+-rw-rw-rw-   0        0        0     1201 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py
+-rw-rw-rw-   0        0        0     5361 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py
+-rw-rw-rw-   0        0        0     1534 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_view.py
+-rw-rw-rw-   0        0        0      704 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py
+-rw-rw-rw-   0        0        0      713 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py
+-rw-rw-rw-   0        0        0      737 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py
+-rw-rw-rw-   0        0        0      692 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_job.py
+-rw-rw-rw-   0        0        0      708 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py
+-rw-rw-rw-   0        0        0      906 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py
+-rw-rw-rw-   0        0        0     1313 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/evaluate.py
+-rw-rw-rw-   0        0        0      223 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/finetune_predictor.py
+-rw-rw-rw-   0        0        0      359 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/latest.py
+-rw-rw-rw-   0        0        0     8140 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/lexer.py
+-rw-rw-rw-   0        0        0    44911 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/parser.py
+-rw-rw-rw-   0        0        0      311 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/retrain_predictor.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mysql/
+-rw-rw-rw-   0        0        0       67 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mysql/__init__.py
+-rw-rw-rw-   0        0        0     1046 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mysql/lexer.py
+-rw-rw-rw-   0        0        0    29491 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mysql/parser.py
+-rw-rw-rw-   0        0        0      904 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mysql/show_index.py
+-rw-rw-rw-   0        0        0      686 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mysql/variable.py
+-rw-rw-rw-   0        0        0     6226 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/lexer.py
+-rw-rw-rw-   0        0        0      751 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/logger.py
+-rw-rw-rw-   0        0        0    21382 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/parser.py
+-rw-rw-rw-   0        0        0     2497 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql/planner/
+-rw-rw-rw-   0        0        0      150 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/planner/__init__.py
+-rw-rw-rw-   0        0        0      878 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/planner/query_plan.py
+-rw-rw-rw-   0        0        0    50030 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/planner/query_planner.py
+-rw-rw-rw-   0        0        0    21367 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/planner/query_prepare.py
+-rw-rw-rw-   0        0        0      536 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/planner/step_result.py
+-rw-rw-rw-   0        0        0     8276 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/planner/steps.py
+-rw-rw-rw-   0        0        0     2981 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/planner/ts_utils.py
+-rw-rw-rw-   0        0        0    17922 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/planner/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql/render/
+-rw-rw-rw-   0        0        0        0 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/render/__init__.py
+-rw-rw-rw-   0        0        0    20561 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/render/sqlalchemy_render.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql.egg-info/
+-rw-rw-rw-   0        0        0      535 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5282 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0      843 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/tests/test_parser/
+-rw-rw-rw-   0        0        0        0 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/
+-rw-rw-rw-   0        0        0        0 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/__init__.py
+-rw-rw-rw-   0        0        0      776 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_ast.py
+-rw-rw-rw-   0        0        0    11910 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_base_lexer.py
+-rw-rw-rw-   0        0        0      223 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_base_sql.py
+-rw-rw-rw-   0        0        0     1480 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_create.py
+-rw-rw-rw-   0        0        0     2481 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_ddl.py
+-rw-rw-rw-   0        0        0     1075 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_delete.py
+-rw-rw-rw-   0        0        0     1094 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_describe.py
+-rw-rw-rw-   0        0        0     2426 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_insert.py
+-rw-rw-rw-   0        0        0     6945 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_misc_sql_queries.py
+-rw-rw-rw-   0        0        0     3625 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_select_common_table_expression.py
+-rw-rw-rw-   0        0        0    24799 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_select_operations.py
+-rw-rw-rw-   0        0        0    45563 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_select_structure.py
+-rw-rw-rw-   0        0        0    13620 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_show.py
+-rw-rw-rw-   0        0        0     3114 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_union.py
+-rw-rw-rw-   0        0        0     2462 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_update.py
+-rw-rw-rw-   0        0        0      514 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_use.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/
+-rw-rw-rw-   0        0        0        0 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/__init__.py
+-rw-rw-rw-   0        0        0     1643 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_chatbots.py
+-rw-rw-rw-   0        0        0      605 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_create_file.py
+-rw-rw-rw-   0        0        0     4203 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_create_integration.py
+-rw-rw-rw-   0        0        0     6617 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_create_predictor.py
+-rw-rw-rw-   0        0        0     2651 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_create_view.py
+-rw-rw-rw-   0        0        0      520 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_drop_dataset.py
+-rw-rw-rw-   0        0        0      861 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_drop_datasource.py
+-rw-rw-rw-   0        0        0      866 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_drop_integration.py
+-rw-rw-rw-   0        0        0     1708 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_drop_predictor.py
+-rw-rw-rw-   0        0        0     1824 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_evaluate.py
+-rw-rw-rw-   0        0        0     1339 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_finetune_predictor.py
+-rw-rw-rw-   0        0        0     2056 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_jobs.py
+-rw-rw-rw-   0        0        0     1587 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_ml_engine.py
+-rw-rw-rw-   0        0        0     2242 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_retrain_predictor.py
+-rw-rw-rw-   0        0        0     3572 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_selects.py
+-rw-rw-rw-   0        0        0     1226 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_show_mindsdb.py
+-rw-rw-rw-   0        0        0      959 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_timeseries.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mysql/
+-rw-rw-rw-   0        0        0        0 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mysql/__init__.py
+-rw-rw-rw-   0        0        0      714 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mysql/test_mysql_lexer.py
+-rw-rw-rw-   0        0        0     3050 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mysql/test_mysql_parser.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/tests/test_render/
+-rw-rw-rw-   0        0        0        0 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_render/__init__.py
+-rw-rw-rw-   0        0        0     6391 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_render/test_sqlalchemyrender.py
```

### Comparing `mindsdb_sql-0.6.1/PKG-INFO` & `mindsdb_sql-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mindsdb_sql
-Version: 0.6.1
+Version: 0.6.2
 Summary: Pure python SQL parser
 Home-page: https://github.com/mindsdb/mindsdb_sql
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb_sql
 Description: UNKNOWN
```

### Comparing `mindsdb_sql-0.6.1/README.md` & `mindsdb_sql-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/__init__.py` & `mindsdb_sql-0.6.2/mindsdb_sql/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/__init__.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/alter_table.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/alter_table.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/base.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/base.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/create.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/create.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/delete.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/delete.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/describe.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/describe.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/drop.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/drop.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/explain.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/explain.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/insert.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/insert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from mindsdb_sql.parser.ast.base import ASTNode
 from mindsdb_sql.parser.utils import indent
 from mindsdb_sql.parser.ast.create import TableColumn
 from mindsdb_sql.parser.ast.select.identifier import Identifier
-
+from mindsdb_sql.parser.ast.select.constant import Constant
 
 class Insert(ASTNode):
 
     def __init__(self,
                  table,
                  columns=None,
                  values=None,
@@ -28,15 +28,17 @@
         self.from_select = from_select
 
     def to_column(self, col):
         if isinstance(col, str):
             return TableColumn(col)
         elif isinstance(col, Identifier):
             return TableColumn(col.parts[0])
-        return col
+        elif isinstance(col, Constant):
+            return TableColumn(col.value)
+        return TableColumn(str(col))
 
     def to_value(self, val):
         if isinstance(val, ASTNode) :
             return val.to_string()
         return repr(val)
 
     def to_tree(self, *args, level=0, **kwargs):
```

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/__init__.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/case.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/case.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/common_table_expression.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/common_table_expression.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/constant.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/constant.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/identifier.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/identifier.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import re
+from copy import copy, deepcopy
+
 from mindsdb_sql.parser.ast.base import ASTNode
 from mindsdb_sql.parser.utils import indent
 from mindsdb_sql.parser.ast.select import Star
 
-import re
 
 no_wrap_identifier_regex = re.compile(r'[a-zA-Z_][a-zA-Z_0-9]*')
 path_str_parts_regex = re.compile(r'(?:(?:(`[^`]+`))|([^.]+))')
 
 
-def path_str_to_parts(path_str):
+def path_str_to_parts(path_str: str):
     match = re.finditer(path_str_parts_regex, path_str)
     parts = [x[0].strip('`') for x in match]
     return parts
 
 
 RESERVED_KEYWORDS = {
     'PERSIST', 'IF', 'EXISTS', 'NULLS', 'FIRST', 'LAST',
@@ -21,14 +23,17 @@
 
 
 class Identifier(ASTNode):
     def __init__(self, path_str=None, parts=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
         assert path_str or parts, "Either path_str or parts must be provided for an Identifier"
         assert not (path_str and parts), "Provide either path_str or parts, but not both"
+        if isinstance(path_str, Star) and not parts:
+            parts = [Star()]
+
         if path_str and not parts:
             parts = path_str_to_parts(path_str)
         assert isinstance(parts, list)
         self.parts = parts
 
         from mindsdb_sql.parser.lexer import SQLLexer
         from mindsdb_sql.parser.dialects.mindsdb.lexer import MindsDBLexer
@@ -48,23 +53,37 @@
         out_parts = []
         for part in self.parts:
             if isinstance(part, Star):
                 part = str(part)
             else:
                 if (
                     not no_wrap_identifier_regex.fullmatch(part)
-                  or
+                    or
                     part.upper() in self.reserved
                 ):
                     part = f'`{part}`'
 
             out_parts.append(part)
         return '.'.join(out_parts)
 
     def to_tree(self, *args, level=0, **kwargs):
         alias_str = f', alias={self.alias.to_tree()}' if self.alias else ''
         return indent(level) + f'Identifier(parts={[str(i) for i in self.parts]}{alias_str})'
 
     def get_string(self, *args, **kwargs):
         return self.parts_to_str()
 
-
+    def __copy__(self):
+        identifier = Identifier(parts=copy(self.parts))
+        identifier.alias = deepcopy(self.alias)
+        identifier.parentheses = self.parentheses
+        if hasattr(self, 'sub_select'):
+            identifier.sub_select = deepcopy(self.sub_select)
+        return identifier
+
+    def __deepcopy__(self, memo):
+        identifier = Identifier(parts=copy(self.parts))
+        identifier.alias = deepcopy(self.alias)
+        identifier.parentheses = self.parentheses
+        if hasattr(self, 'sub_select'):
+            identifier.sub_select = deepcopy(self.sub_select)
+        return identifier
```

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/join.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/join.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/native_query.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/native_query.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/operation.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/operation.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/order_by.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/order_by.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/select.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/select.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/tuple.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/tuple.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/type_cast.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/type_cast.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/select/union.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/union.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/set.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/set.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/show.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/show.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/update.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/update.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/ast/use.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/use.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/__init__.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,10 +10,11 @@
 from .evaluate import Evaluate
 from .latest import Latest
 from .create_file import CreateFile
 from .create_ml_engine import CreateMLEngine
 from .drop_ml_engine import DropMLEngine
 from .create_job import CreateJob
 from .drop_job import DropJob
+from .chatbot import CreateChatBot, DropChatBot
 
 # remove it in next release
 CreateDatasource = CreateDatabase
```

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/create_database.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_database.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/create_file.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_file.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/create_job.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_job.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/create_view.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_view.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/drop_job.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_job.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/evaluate.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/evaluate.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/lexer.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         # Mindsdb special
 
         PREDICTOR, PREDICTORS, DATASOURCE, INTEGRATION, INTEGRATIONS,DATASOURCES,
         STREAM, STREAMS, PUBLICATION, PUBLICATIONS, VIEW, VIEWS, DATASETS, DATASET,
         MODEL, MODELS, ML_ENGINE, ML_ENGINES, HANDLERS,
         FINETUNE, EVALUATE,
         LATEST, HORIZON, USING,
-        ENGINE, TRAIN, PREDICT, PARAMETERS, JOB, EVERY,PROJECT,
+        ENGINE, TRAIN, PREDICT, PARAMETERS, JOB, CHATBOT, EVERY,PROJECT,
 
         # SHOW/DDL Keywords
 
         SHOW, SCHEMAS, SCHEMA, DATABASES, DATABASE, TABLES, TABLE, FULL, EXTENDED, PROCESSLIST,
         MUTEX, CODE, SLAVE, REPLICA, REPLICAS, CHANNEL, TRIGGERS, KEYS, STORAGE, LOGS, BINARY,
         MASTER, PRIVILEGES, PROFILES, HOSTS, OPEN, INDEXES,
         VARIABLES, SESSION, STATUS,
@@ -101,14 +101,15 @@
     LATEST = r'\bLATEST\b'
     MODEL = r'\bMODEL\b'
     MODELS = r'\bMODELS\b'
     ML_ENGINE = r'\bML_ENGINE\b'
     ML_ENGINES = r'\bML_ENGINES\b'
     HANDLERS = r'\bHANDLERS\b'
     JOB = r'\bJOB\b'
+    CHATBOT = r'\bCHATBOT\b'
     EVERY = r'\bEVERY\b'
     PROJECT = r'\bPROJECT\b'
     EVALUATE = r'\bEVALUATE\b'
 
     # Misc
     SET = r'\bSET\b'
     START = r'\bSTART\b'
```

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mindsdb/parser.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from mindsdb_sql.parser.dialects.mindsdb.drop_dataset import DropDataset
 from mindsdb_sql.parser.dialects.mindsdb.drop_ml_engine import DropMLEngine
 from mindsdb_sql.parser.dialects.mindsdb.create_predictor import CreatePredictor
 from mindsdb_sql.parser.dialects.mindsdb.create_database import CreateDatabase
 from mindsdb_sql.parser.dialects.mindsdb.create_ml_engine import CreateMLEngine
 from mindsdb_sql.parser.dialects.mindsdb.create_view import CreateView
 from mindsdb_sql.parser.dialects.mindsdb.create_job import CreateJob
+from mindsdb_sql.parser.dialects.mindsdb.chatbot import CreateChatBot, DropChatBot
 from mindsdb_sql.parser.dialects.mindsdb.drop_job import DropJob
 from mindsdb_sql.parser.dialects.mindsdb.latest import Latest
 from mindsdb_sql.parser.dialects.mindsdb.evaluate import Evaluate
 from mindsdb_sql.parser.dialects.mindsdb.create_file import CreateFile
 from mindsdb_sql.exceptions import ParsingException
 from mindsdb_sql.parser.dialects.mindsdb.lexer import MindsDBLexer
 from mindsdb_sql.parser.dialects.mindsdb.retrain_predictor import RetrainPredictor
@@ -72,14 +73,31 @@
        'create_table',
        'create_job',
        'drop_job',
        )
     def query(self, p):
         return p[0]
 
+    # -- ChatBot --
+    @_('CREATE CHATBOT identifier USING kw_parameter_list')
+    def create_job(self, p):
+        params = p.kw_parameter_list
+
+        database = Identifier(params.pop('database'))
+        model = Identifier(params.pop('model'))
+        return CreateChatBot(
+            name=p.identifier,
+            database=database,
+            model=model,
+            params=params
+        )
+
+    @_('DROP CHATBOT identifier')
+    def drop_job(self, p):
+        return DropChatBot(name=p.identifier)
 
     # -- Jobs --
     @_('CREATE JOB identifier LPAREN raw_query RPAREN job_schedule',
        'CREATE JOB identifier AS LPAREN raw_query RPAREN job_schedule',
        'CREATE JOB identifier LPAREN raw_query RPAREN',
        'CREATE JOB identifier AS LPAREN raw_query RPAREN')
     def create_job(self, p):
```

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mysql/lexer.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mysql/lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mysql/parser.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mysql/parser.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mysql/show_index.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mysql/show_index.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/dialects/mysql/variable.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mysql/variable.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/lexer.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/logger.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/logger.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/parser.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/parser.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/parser/utils.py` & `mindsdb_sql-0.6.2/mindsdb_sql/parser/utils.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/planner/query_plan.py` & `mindsdb_sql-0.6.2/mindsdb_sql/planner/query_plan.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/planner/query_planner.py` & `mindsdb_sql-0.6.2/mindsdb_sql/planner/query_planner.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,15 @@
             )
         else:
             new_query_targets = []
             for target in select.targets:
                 if isinstance(target, Identifier):
                     new_query_targets.append(
                         disambiguate_predictor_column_identifier(target, predictor))
-                elif type(target) in (Star, Constant):
+                elif type(target) in (Star, Constant, Function):
                     new_query_targets.append(target)
                 else:
                     raise PlanningException(f'Unknown select target {type(target)}')
 
             if select.group_by or select.having:
                 raise PlanningException(f'Unsupported operation when querying predictor. Only WHERE is allowed and required.')
```

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/planner/query_prepare.py` & `mindsdb_sql-0.6.2/mindsdb_sql/planner/query_prepare.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/planner/step_result.py` & `mindsdb_sql-0.6.2/mindsdb_sql/planner/step_result.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/planner/steps.py` & `mindsdb_sql-0.6.2/mindsdb_sql/planner/steps.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/planner/ts_utils.py` & `mindsdb_sql-0.6.2/mindsdb_sql/planner/ts_utils.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/planner/utils.py` & `mindsdb_sql-0.6.2/mindsdb_sql/planner/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     elif len(parts) == 1:
         # if parts[0] != column_table_ref:
         parts = column_table_ref + parts
 
     new_identifier = Identifier(parts=parts)
     if identifier.alias:
         new_identifier.alias = identifier.alias
-    elif initial_name_as_alias:
+    elif initial_name_as_alias and not isinstance(parts[-1], Star):
         new_identifier.alias = Identifier(parts[-1])
 
     return new_identifier
 
 
 def disambiguate_predictor_column_identifier(identifier, predictor):
     """Removes integration name from column if it's present, adds table path if it's absent"""
```

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql/render/sqlalchemy_render.py` & `mindsdb_sql-0.6.2/mindsdb_sql/render/sqlalchemy_render.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql.egg-info/PKG-INFO` & `mindsdb_sql-0.6.2/mindsdb_sql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mindsdb-sql
-Version: 0.6.1
+Version: 0.6.2
 Summary: Pure python SQL parser
 Home-page: https://github.com/mindsdb/mindsdb_sql
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb_sql
 Description: UNKNOWN
```

### Comparing `mindsdb_sql-0.6.1/mindsdb_sql.egg-info/SOURCES.txt` & `mindsdb_sql-0.6.2/mindsdb_sql.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 mindsdb_sql/parser/ast/select/select.py
 mindsdb_sql/parser/ast/select/star.py
 mindsdb_sql/parser/ast/select/tuple.py
 mindsdb_sql/parser/ast/select/type_cast.py
 mindsdb_sql/parser/ast/select/union.py
 mindsdb_sql/parser/dialects/__init__.py
 mindsdb_sql/parser/dialects/mindsdb/__init__.py
+mindsdb_sql/parser/dialects/mindsdb/chatbot.py
 mindsdb_sql/parser/dialects/mindsdb/create_database.py
 mindsdb_sql/parser/dialects/mindsdb/create_file.py
 mindsdb_sql/parser/dialects/mindsdb/create_job.py
 mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py
 mindsdb_sql/parser/dialects/mindsdb/create_predictor.py
 mindsdb_sql/parser/dialects/mindsdb/create_view.py
 mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py
@@ -95,14 +96,15 @@
 tests/test_parser/test_base_sql/test_select_operations.py
 tests/test_parser/test_base_sql/test_select_structure.py
 tests/test_parser/test_base_sql/test_show.py
 tests/test_parser/test_base_sql/test_union.py
 tests/test_parser/test_base_sql/test_update.py
 tests/test_parser/test_base_sql/test_use.py
 tests/test_parser/test_mindsdb/__init__.py
+tests/test_parser/test_mindsdb/test_chatbots.py
 tests/test_parser/test_mindsdb/test_create_file.py
 tests/test_parser/test_mindsdb/test_create_integration.py
 tests/test_parser/test_mindsdb/test_create_predictor.py
 tests/test_parser/test_mindsdb/test_create_view.py
 tests/test_parser/test_mindsdb/test_drop_dataset.py
 tests/test_parser/test_mindsdb/test_drop_datasource.py
 tests/test_parser/test_mindsdb/test_drop_integration.py
```

### Comparing `mindsdb_sql-0.6.1/setup.py` & `mindsdb_sql-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_ast.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_ast.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_base_lexer.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_base_lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_create.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_create.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_ddl.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_ddl.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_delete.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_delete.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_describe.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_describe.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_insert.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_insert.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_misc_sql_queries.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_misc_sql_queries.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_select_common_table_expression.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_select_common_table_expression.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_select_operations.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_select_operations.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_select_structure.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_select_structure.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_show.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_show.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_union.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_union.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_update.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_update.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_base_sql/test_use.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_use.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_create_file.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_create_file.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_create_integration.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_create_integration.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_create_predictor.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_create_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_create_view.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_create_view.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_drop_dataset.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_drop_dataset.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_drop_datasource.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_drop_datasource.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_drop_integration.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_drop_integration.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_drop_predictor.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_drop_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_evaluate.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_finetune_predictor.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_finetune_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_jobs.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_jobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import pytest
-
 from mindsdb_sql import parse_sql
 from mindsdb_sql.parser.dialects.mindsdb import *
 from mindsdb_sql.parser.ast import *
 
 
 class TestJobs:
     def test_test_create_job(self):
```

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_ml_engine.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_ml_engine.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_retrain_predictor.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_retrain_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_selects.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_selects.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_show_mindsdb.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_show_mindsdb.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_mindsdb/test_timeseries.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_mysql/test_mysql_lexer.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_mysql/test_mysql_lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_parser/test_mysql/test_mysql_parser.py` & `mindsdb_sql-0.6.2/tests/test_parser/test_mysql/test_mysql_parser.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.1/tests/test_render/test_sqlalchemyrender.py` & `mindsdb_sql-0.6.2/tests/test_render/test_sqlalchemyrender.py`

 * *Files identical despite different names*

