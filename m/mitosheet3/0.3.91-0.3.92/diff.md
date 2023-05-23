# Comparing `tmp/mitosheet3-0.3.91.tar.gz` & `tmp/mitosheet3-0.3.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitosheet3-0.3.91.tar", last modified: Mon Jul  5 05:01:26 2021, max compression
+gzip compressed data, was "mitosheet3-0.3.92.tar", last modified: Mon Jul  5 15:09:18 2021, max compression
```

## Comparing `mitosheet3-0.3.91.tar` & `mitosheet3-0.3.92.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 05:01:26.828819 mitosheet3-0.3.91/
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2021-07-05 04:47:35.000000 mitosheet3-0.3.91/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1836 2021-07-05 05:01:26.828819 mitosheet3-0.3.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4823 2021-07-05 04:47:35.000000 mitosheet3-0.3.91/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 05:01:26.816818 mitosheet3-0.3.91/mitosheet/
--rw-r--r--   0 runner    (1001) docker     (121)     1662 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      370 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (121)     1660 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 05:01:26.816818 mitosheet3-0.3.91/mitosheet/api/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4875 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/api/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1662 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/api/get_column_describe.py
--rw-r--r--   0 runner    (1001) docker     (121)      252 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/api/get_column_dtype.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/api/get_datafiles.py
--rw-r--r--   0 runner    (1001) docker     (121)      195 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/api/get_dateframe_as_csv.py
--rw-r--r--   0 runner    (1001) docker     (121)    32222 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/api/get_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     1656 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/api/get_import_summary.py
--rw-r--r--   0 runner    (1001) docker     (121)     2452 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/api/get_path_contents.py
--rw-r--r--   0 runner    (1001) docker     (121)      674 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/api/get_path_join.py
--rw-r--r--   0 runner    (1001) docker     (121)     1467 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/api/get_saved_analysis_description.py
--rw-r--r--   0 runner    (1001) docker     (121)     3400 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/data_in_mito.py
--rw-r--r--   0 runner    (1001) docker     (121)    13814 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 05:01:26.816818 mitosheet3-0.3.91/mitosheet/labextension/
--rw-r--r--   0 runner    (1001) docker     (121)     4134 2021-07-05 05:01:21.000000 mitosheet3-0.3.91/mitosheet/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 05:01:26.820818 mitosheet3-0.3.91/mitosheet/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (121)    36616 2021-07-05 05:01:21.000000 mitosheet3-0.3.91/mitosheet/labextension/static/0.bdbf1960886caa2f64e0.js
--rw-r--r--   0 runner    (1001) docker     (121)      313 2021-07-05 05:01:21.000000 mitosheet3-0.3.91/mitosheet/labextension/static/0.bdbf1960886caa2f64e0.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4020 2021-07-05 05:01:21.000000 mitosheet3-0.3.91/mitosheet/labextension/static/149.a955b532a2f6424f09da.js
--rw-r--r--   0 runner    (1001) docker     (121)     4020 2021-07-05 05:01:21.000000 mitosheet3-0.3.91/mitosheet/labextension/static/461.cc00aa043b123b43d40d.js
--rw-r--r--   0 runner    (1001) docker     (121)   317534 2021-07-05 05:01:21.000000 mitosheet3-0.3.91/mitosheet/labextension/static/480.e084e61bbf78e5e83444.js
--rw-r--r--   0 runner    (1001) docker     (121)   181922 2021-07-05 05:01:21.000000 mitosheet3-0.3.91/mitosheet/labextension/static/534.ecfeee9921699bf3929e.js
--rw-r--r--   0 runner    (1001) docker     (121)      475 2021-07-05 05:01:21.000000 mitosheet3-0.3.91/mitosheet/labextension/static/534.ecfeee9921699bf3929e.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      290 2021-07-05 05:01:21.000000 mitosheet3-0.3.91/mitosheet/labextension/static/568.e067c39c389e7e86b7ee.js
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2021-07-05 05:01:21.000000 mitosheet3-0.3.91/mitosheet/labextension/static/7.a501bf39686c40af057f.js
--rw-r--r--   0 runner    (1001) docker     (121)   152717 2021-07-05 05:01:21.000000 mitosheet3-0.3.91/mitosheet/labextension/static/812.a706af7a2a6413de9561.js
--rw-r--r--   0 runner    (1001) docker     (121)   915037 2021-07-05 05:01:21.000000 mitosheet3-0.3.91/mitosheet/labextension/static/853.4123dc4d2193c3ad8e88.js
--rw-r--r--   0 runner    (1001) docker     (121)      403 2021-07-05 05:01:21.000000 mitosheet3-0.3.91/mitosheet/labextension/static/853.4123dc4d2193c3ad8e88.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8484 2021-07-05 05:01:21.000000 mitosheet3-0.3.91/mitosheet/labextension/static/remoteEntry.25954ef11e950542a78c.js
--rw-r--r--   0 runner    (1001) docker     (121)      118 2021-07-05 05:01:05.000000 mitosheet3-0.3.91/mitosheet/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (121)    15704 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/mito_analytics.py
--rw-r--r--   0 runner    (1001) docker     (121)    12967 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/mito_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     8325 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 05:01:26.820818 mitosheet3-0.3.91/mitosheet/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/preprocessing/preprocess_check_args_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      940 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/preprocessing/preprocess_copy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2951 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/preprocessing/preprocess_read_file_paths.py
--rw-r--r--   0 runner    (1001) docker     (121)     1795 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/preprocessing/preprocess_rename_headers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/profiling.py
--rw-r--r--   0 runner    (1001) docker     (121)     6563 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/save_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 05:01:26.820818 mitosheet3-0.3.91/mitosheet/saves/
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/saves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      630 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/saves/mito_simple_raw_import.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 05:01:26.820818 mitosheet3-0.3.91/mitosheet/saves/tutorial_v3/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/saves/tutorial_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      539 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/saves/tutorial_v3/mito_tutorial_checkpoint_2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/saves/tutorial_v3/mito_tutorial_checkpoint_3.py
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/saves/tutorial_v3/mito_tutorial_checkpoint_4.py
--rw-r--r--   0 runner    (1001) docker     (121)     2061 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/saves/tutorial_v3/mito_tutorial_checkpoint_5.py
--rw-r--r--   0 runner    (1001) docker     (121)     2493 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/saves/tutorial_v3/mito_tutorial_checkpoint_6.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 05:01:26.820818 mitosheet3-0.3.91/mitosheet/sheet_functions/
--rw-r--r--   0 runner    (1001) docker     (121)      764 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/sheet_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5607 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/sheet_functions/control_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4098 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/sheet_functions/date_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4746 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/sheet_functions/misc_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    13942 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/sheet_functions/number_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1557 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/sheet_functions/sheet_function_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    14445 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/sheet_functions/string_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 05:01:26.824818 mitosheet3-0.3.91/mitosheet/sheet_functions/types/
--rw-r--r--   0 runner    (1001) docker     (121)      820 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/sheet_functions/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8712 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/sheet_functions/types/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1533 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/sheet_functions/types/to_boolean_series.py
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/sheet_functions/types/to_datetime_series.py
--rw-r--r--   0 runner    (1001) docker     (121)     4493 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/sheet_functions/types/to_number_series.py
--rw-r--r--   0 runner    (1001) docker     (121)     1407 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/sheet_functions/types/to_string_series.py
--rw-r--r--   0 runner    (1001) docker     (121)     6018 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/sheet_functions/types/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 05:01:26.824818 mitosheet3-0.3.91/mitosheet/steps/
--rw-r--r--   0 runner    (1001) docker     (121)     2358 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 05:01:26.824818 mitosheet3-0.3.91/mitosheet/steps/column_steps/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/steps/column_steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3633 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/steps/column_steps/add_column.py
--rw-r--r--   0 runner    (1001) docker     (121)    14330 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/steps/column_steps/change_column_dtype.py
--rw-r--r--   0 runner    (1001) docker     (121)     3337 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/steps/column_steps/delete_column.py
--rw-r--r--   0 runner    (1001) docker     (121)     5722 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/steps/column_steps/rename_column.py
--rw-r--r--   0 runner    (1001) docker     (121)     3970 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/steps/column_steps/reorder_column.py
--rw-r--r--   0 runner    (1001) docker     (121)    12870 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/steps/column_steps/set_column_formula.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 05:01:26.824818 mitosheet3-0.3.91/mitosheet/steps/dataframe_steps/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/steps/dataframe_steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2402 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/steps/dataframe_steps/dataframe_delete.py
--rw-r--r--   0 runner    (1001) docker     (121)     2508 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/steps/dataframe_steps/dataframe_duplicate.py
--rw-r--r--   0 runner    (1001) docker     (121)     3935 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/steps/dataframe_steps/dataframe_rename.py
--rw-r--r--   0 runner    (1001) docker     (121)    18555 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/steps/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 05:01:26.824818 mitosheet3-0.3.91/mitosheet/steps/import_steps/
--rw-r--r--   0 runner    (1001) docker     (121)      119 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/steps/import_steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3670 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/steps/import_steps/raw_python_import.py
--rw-r--r--   0 runner    (1001) docker     (121)     5430 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/steps/import_steps/simple_import.py
--rw-r--r--   0 runner    (1001) docker     (121)     3323 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/steps/initalize.py
--rw-r--r--   0 runner    (1001) docker     (121)     7180 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/steps/merge.py
--rw-r--r--   0 runner    (1001) docker     (121)    10171 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/steps/pivot.py
--rw-r--r--   0 runner    (1001) docker     (121)     3441 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/steps/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 05:01:26.824818 mitosheet3-0.3.91/mitosheet/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     5621 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      939 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/tests/test_execution_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2945 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/tests/test_format.py
--rw-r--r--   0 runner    (1001) docker     (121)      246 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/tests/test_mito_analytics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1414 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/tests/test_mitosheet_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      274 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/tests/test_multi_threaded.py
--rw-r--r--   0 runner    (1001) docker     (121)     8172 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (121)    14346 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/tests/test_save_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5393 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/tests/test_step_format.py
--rw-r--r--   0 runner    (1001) docker     (121)     3699 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/tests/test_topological_sort.py
--rw-r--r--   0 runner    (1001) docker     (121)    12668 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/tests/test_transpile.py
--rw-r--r--   0 runner    (1001) docker     (121)     5721 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/tests/test_ts_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     9442 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/tests/test_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (121)    13742 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5017 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/tests/test_widget_state_container.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 05:01:26.828819 mitosheet3-0.3.91/mitosheet/tests/user/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/tests/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3369 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/tests/user/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     6587 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/tests/user/test_user.py
--rw-r--r--   0 runner    (1001) docker     (121)     1330 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/tests/user/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4010 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/topological_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 05:01:26.828819 mitosheet3-0.3.91/mitosheet/transpiler/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/transpiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2544 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/transpiler/transpile.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 05:01:26.828819 mitosheet3-0.3.91/mitosheet/updates/
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/updates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/updates/append_user_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     2816 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/updates/args_update.py
--rw-r--r--   0 runner    (1001) docker     (121)      656 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/updates/checkout_step_by_idx.py
--rw-r--r--   0 runner    (1001) docker     (121)      762 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/updates/delete_saved_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)      842 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/updates/rename_saved_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     2219 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/updates/replay_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)      657 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/updates/save_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)      894 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/updates/set_user_field_update.py
--rw-r--r--   0 runner    (1001) docker     (121)      902 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/updates/undo.py
--rw-r--r--   0 runner    (1001) docker     (121)     8147 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 05:01:26.828819 mitosheet3-0.3.91/mitosheet/user/
--rw-r--r--   0 runner    (1001) docker     (121)      643 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4594 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/user/create.py
--rw-r--r--   0 runner    (1001) docker     (121)     1276 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/user/db.py
--rw-r--r--   0 runner    (1001) docker     (121)     3692 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/user/schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)     5500 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/user/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (121)     2162 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/user/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8097 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    14945 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/mitosheet/widget_state_container.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 05:01:26.828819 mitosheet3-0.3.91/mitosheet3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1836 2021-07-05 05:01:26.000000 mitosheet3-0.3.91/mitosheet3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5287 2021-07-05 05:01:26.000000 mitosheet3-0.3.91/mitosheet3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-05 05:01:26.000000 mitosheet3-0.3.91/mitosheet3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-05 04:59:32.000000 mitosheet3-0.3.91/mitosheet3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      168 2021-07-05 05:01:26.000000 mitosheet3-0.3.91/mitosheet3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-07-05 05:01:26.000000 mitosheet3-0.3.91/mitosheet3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      145 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-07-05 05:01:26.828819 mitosheet3-0.3.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     8954 2021-07-05 04:47:36.000000 mitosheet3-0.3.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 15:09:18.221458 mitosheet3-0.3.92/
+-rw-r--r--   0 runner    (1001) docker     (121)     1489 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1836 2021-07-05 15:09:18.221458 mitosheet3-0.3.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4823 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 15:09:18.205457 mitosheet3-0.3.92/mitosheet/
+-rw-r--r--   0 runner    (1001) docker     (121)     1662 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1106 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      370 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1660 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 15:09:18.205457 mitosheet3-0.3.92/mitosheet/api/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4875 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1662 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/api/get_column_describe.py
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/api/get_column_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (121)      837 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/api/get_datafiles.py
+-rw-r--r--   0 runner    (1001) docker     (121)      195 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/api/get_dateframe_as_csv.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32222 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/api/get_graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1656 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/api/get_import_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2452 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/api/get_path_contents.py
+-rw-r--r--   0 runner    (1001) docker     (121)      674 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/api/get_path_join.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1467 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/api/get_saved_analysis_description.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3400 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/data_in_mito.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13814 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 15:09:18.205457 mitosheet3-0.3.92/mitosheet/labextension/
+-rw-r--r--   0 runner    (1001) docker     (121)     4134 2021-07-05 15:09:11.000000 mitosheet3-0.3.92/mitosheet/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 15:09:18.209457 mitosheet3-0.3.92/mitosheet/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (121)    36616 2021-07-05 15:09:11.000000 mitosheet3-0.3.92/mitosheet/labextension/static/0.bdbf1960886caa2f64e0.js
+-rw-r--r--   0 runner    (1001) docker     (121)      313 2021-07-05 15:09:11.000000 mitosheet3-0.3.92/mitosheet/labextension/static/0.bdbf1960886caa2f64e0.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4020 2021-07-05 15:09:11.000000 mitosheet3-0.3.92/mitosheet/labextension/static/149.a955b532a2f6424f09da.js
+-rw-r--r--   0 runner    (1001) docker     (121)     4020 2021-07-05 15:09:11.000000 mitosheet3-0.3.92/mitosheet/labextension/static/461.cc00aa043b123b43d40d.js
+-rw-r--r--   0 runner    (1001) docker     (121)   317701 2021-07-05 15:09:11.000000 mitosheet3-0.3.92/mitosheet/labextension/static/480.b800b2485bc1f4911b0e.js
+-rw-r--r--   0 runner    (1001) docker     (121)   181922 2021-07-05 15:09:11.000000 mitosheet3-0.3.92/mitosheet/labextension/static/534.ecfeee9921699bf3929e.js
+-rw-r--r--   0 runner    (1001) docker     (121)      475 2021-07-05 15:09:11.000000 mitosheet3-0.3.92/mitosheet/labextension/static/534.ecfeee9921699bf3929e.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2021-07-05 15:09:11.000000 mitosheet3-0.3.92/mitosheet/labextension/static/568.e067c39c389e7e86b7ee.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1821 2021-07-05 15:09:11.000000 mitosheet3-0.3.92/mitosheet/labextension/static/7.a501bf39686c40af057f.js
+-rw-r--r--   0 runner    (1001) docker     (121)   152717 2021-07-05 15:09:11.000000 mitosheet3-0.3.92/mitosheet/labextension/static/812.a706af7a2a6413de9561.js
+-rw-r--r--   0 runner    (1001) docker     (121)   915037 2021-07-05 15:09:11.000000 mitosheet3-0.3.92/mitosheet/labextension/static/853.4123dc4d2193c3ad8e88.js
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2021-07-05 15:09:11.000000 mitosheet3-0.3.92/mitosheet/labextension/static/853.4123dc4d2193c3ad8e88.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8484 2021-07-05 15:09:11.000000 mitosheet3-0.3.92/mitosheet/labextension/static/remoteEntry.84d311aab4baee4ad12b.js
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2021-07-05 15:08:53.000000 mitosheet3-0.3.92/mitosheet/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (121)    15704 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/mito_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12967 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/mito_widget.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8325 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 15:09:18.209457 mitosheet3-0.3.92/mitosheet/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (121)     1362 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1548 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/preprocessing/preprocess_check_args_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      940 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/preprocessing/preprocess_copy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2951 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/preprocessing/preprocess_read_file_paths.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1795 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/preprocessing/preprocess_rename_headers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1009 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6563 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/save_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 15:09:18.209457 mitosheet3-0.3.92/mitosheet/saves/
+-rw-r--r--   0 runner    (1001) docker     (121)     1461 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/saves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      630 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/saves/mito_simple_raw_import.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 15:09:18.209457 mitosheet3-0.3.92/mitosheet/saves/tutorial_v3/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/saves/tutorial_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      539 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/saves/tutorial_v3/mito_tutorial_checkpoint_2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1133 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/saves/tutorial_v3/mito_tutorial_checkpoint_3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1377 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/saves/tutorial_v3/mito_tutorial_checkpoint_4.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2061 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/saves/tutorial_v3/mito_tutorial_checkpoint_5.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2493 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/saves/tutorial_v3/mito_tutorial_checkpoint_6.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 15:09:18.213457 mitosheet3-0.3.92/mitosheet/sheet_functions/
+-rw-r--r--   0 runner    (1001) docker     (121)      764 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/sheet_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5607 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/sheet_functions/control_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4098 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/sheet_functions/date_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4746 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/sheet_functions/misc_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13942 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/sheet_functions/number_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1557 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/sheet_functions/sheet_function_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14445 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/sheet_functions/string_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 15:09:18.213457 mitosheet3-0.3.92/mitosheet/sheet_functions/types/
+-rw-r--r--   0 runner    (1001) docker     (121)      820 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/sheet_functions/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8712 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/sheet_functions/types/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1533 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/sheet_functions/types/to_boolean_series.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1208 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/sheet_functions/types/to_datetime_series.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4493 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/sheet_functions/types/to_number_series.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1407 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/sheet_functions/types/to_string_series.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6018 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/sheet_functions/types/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 15:09:18.213457 mitosheet3-0.3.92/mitosheet/steps/
+-rw-r--r--   0 runner    (1001) docker     (121)     2358 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 15:09:18.213457 mitosheet3-0.3.92/mitosheet/steps/column_steps/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/steps/column_steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3633 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/steps/column_steps/add_column.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14330 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/steps/column_steps/change_column_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3337 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/steps/column_steps/delete_column.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5722 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/steps/column_steps/rename_column.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3970 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/steps/column_steps/reorder_column.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12870 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/steps/column_steps/set_column_formula.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 15:09:18.213457 mitosheet3-0.3.92/mitosheet/steps/dataframe_steps/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/steps/dataframe_steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2402 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/steps/dataframe_steps/dataframe_delete.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2508 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/steps/dataframe_steps/dataframe_duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3935 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/steps/dataframe_steps/dataframe_rename.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18555 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/steps/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 15:09:18.213457 mitosheet3-0.3.92/mitosheet/steps/import_steps/
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/steps/import_steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3670 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/steps/import_steps/raw_python_import.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5430 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/steps/import_steps/simple_import.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3323 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/steps/initalize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7180 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/steps/merge.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10171 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/steps/pivot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3441 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/steps/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 15:09:18.217457 mitosheet3-0.3.92/mitosheet/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1100 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5621 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)      939 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/tests/test_execution_errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2945 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/tests/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/tests/test_mito_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1414 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/tests/test_mitosheet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/tests/test_multi_threaded.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8172 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14346 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/tests/test_save_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5393 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/tests/test_step_format.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3699 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/tests/test_topological_sort.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12668 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/tests/test_transpile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5721 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/tests/test_ts_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9442 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/tests/test_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13742 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5017 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/tests/test_widget_state_container.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 15:09:18.217457 mitosheet3-0.3.92/mitosheet/tests/user/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/tests/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3369 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/tests/user/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6587 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/tests/user/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1330 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/tests/user/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4010 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/topological_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 15:09:18.217457 mitosheet3-0.3.92/mitosheet/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/transpiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2544 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/transpiler/transpile.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 15:09:18.221458 mitosheet3-0.3.92/mitosheet/updates/
+-rw-r--r--   0 runner    (1001) docker     (121)     1401 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/updates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1198 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/updates/append_user_field.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2816 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/updates/args_update.py
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/updates/checkout_step_by_idx.py
+-rw-r--r--   0 runner    (1001) docker     (121)      762 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/updates/delete_saved_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)      842 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/updates/rename_saved_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2219 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/updates/replay_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)      657 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/updates/save_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)      894 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/updates/set_user_field_update.py
+-rw-r--r--   0 runner    (1001) docker     (121)      902 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/updates/undo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8147 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 15:09:18.221458 mitosheet3-0.3.92/mitosheet/user/
+-rw-r--r--   0 runner    (1001) docker     (121)      643 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4594 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/user/create.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1276 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/user/db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3692 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/user/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5500 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/user/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2162 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/user/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8097 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14945 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/mitosheet/widget_state_container.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-05 15:09:18.221458 mitosheet3-0.3.92/mitosheet3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1836 2021-07-05 15:09:18.000000 mitosheet3-0.3.92/mitosheet3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5287 2021-07-05 15:09:18.000000 mitosheet3-0.3.92/mitosheet3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-05 15:09:18.000000 mitosheet3-0.3.92/mitosheet3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-05 15:07:08.000000 mitosheet3-0.3.92/mitosheet3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2021-07-05 15:09:18.000000 mitosheet3-0.3.92/mitosheet3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-07-05 15:09:18.000000 mitosheet3-0.3.92/mitosheet3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2021-07-05 15:09:18.221458 mitosheet3-0.3.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     8954 2021-07-05 14:54:25.000000 mitosheet3-0.3.92/setup.py
```

### Comparing `mitosheet3-0.3.91/LICENSE.txt` & `mitosheet3-0.3.92/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/PKG-INFO` & `mitosheet3-0.3.92/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitosheet3
-Version: 0.3.91
+Version: 0.3.92
 Summary: The Mito Spreadsheet
 Home-page: https://github.com/mito/mito
 Author: Mito Sheet
 Author-email: naterush1997@gmail.com
 License: Other/Proprietary License
 Description: 
                     To learn more about Mito, checkout out our documentation: https://docs.trymito.io/getting-started/installing-mito
```

### Comparing `mitosheet3-0.3.91/README.md` & `mitosheet3-0.3.92/README.md`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/__init__.py` & `mitosheet3-0.3.92/mitosheet/__init__.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/__main__.py` & `mitosheet3-0.3.92/mitosheet/__main__.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/_version.py` & `mitosheet3-0.3.92/mitosheet/_version.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/api/api.py` & `mitosheet3-0.3.92/mitosheet/api/api.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/api/get_column_describe.py` & `mitosheet3-0.3.92/mitosheet/api/get_column_describe.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/api/get_datafiles.py` & `mitosheet3-0.3.92/mitosheet/api/get_datafiles.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/api/get_graph.py` & `mitosheet3-0.3.92/mitosheet/api/get_graph.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/api/get_import_summary.py` & `mitosheet3-0.3.92/mitosheet/api/get_import_summary.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/api/get_path_contents.py` & `mitosheet3-0.3.92/mitosheet/api/get_path_contents.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/api/get_path_join.py` & `mitosheet3-0.3.92/mitosheet/api/get_path_join.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/api/get_saved_analysis_description.py` & `mitosheet3-0.3.92/mitosheet/api/get_saved_analysis_description.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/data_in_mito.py` & `mitosheet3-0.3.92/mitosheet/data_in_mito.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/errors.py` & `mitosheet3-0.3.92/mitosheet/errors.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/labextension/package.json` & `mitosheet3-0.3.92/mitosheet/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.957175925925926%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.84d311aab4baee4ad12b.js'}}",*

 * * "'version'": "'0.3.92'",*

 * * "'versions'": "{'mitosheet': '0.1.302', 'mitosheet3': '0.3.92'}"}*

```diff
@@ -51,15 +51,15 @@
         "css/**/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/mito/mito",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.25954ef11e950542a78c.js"
+            "load": "static/remoteEntry.84d311aab4baee4ad12b.js"
         },
         "extension": "lib/plugin",
         "outputDir": "mitosheet/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -109,13 +109,13 @@
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch",
         "watch:src": "tsc -w"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.3.91",
+    "version": "0.3.92",
     "versions": {
-        "mitosheet": "0.1.301",
-        "mitosheet3": "0.3.91"
+        "mitosheet": "0.1.302",
+        "mitosheet3": "0.3.92"
     }
 }
```

### Comparing `mitosheet3-0.3.91/mitosheet/labextension/static/0.bdbf1960886caa2f64e0.js` & `mitosheet3-0.3.92/mitosheet/labextension/static/0.bdbf1960886caa2f64e0.js`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/labextension/static/149.a955b532a2f6424f09da.js` & `mitosheet3-0.3.92/mitosheet/labextension/static/149.a955b532a2f6424f09da.js`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/labextension/static/461.cc00aa043b123b43d40d.js` & `mitosheet3-0.3.92/mitosheet/labextension/static/461.cc00aa043b123b43d40d.js`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/labextension/static/480.e084e61bbf78e5e83444.js` & `mitosheet3-0.3.92/mitosheet/labextension/static/480.b800b2485bc1f4911b0e.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -242,26 +242,26 @@
                 for (a = 0; a < n.length - 1; a++) {
                     const e = n[a],
                         s = n[a + 1];
                     e.length + s.length <= 9 ? (t.push(e + s), a++) : t.push(e)
                 }
                 return a === n.length - 1 && t.push(n[n.length - 1]), t
             }
-            const _ = e => o().createElement("svg", {
+            const k = e => o().createElement("svg", {
                     width: e.width || "13",
                     height: e.height || "10",
                     viewBox: "0 0 9 7",
                     fill: "none",
                     xmlns: "http://www.w3.org/2000/svg"
                 }, o().createElement("path", {
                     d: "M3.63486 6.75C3.49679 6.75 3.38486 6.63807 3.38486 6.5V4.18709C3.38486 4.00613 3.31943 3.83127 3.20064 3.69476L0.781003 0.91411C0.640219 0.75232 0.755131 0.5 0.969598 0.5L8.30011 0.5C8.51458 0.5 8.62949 0.75232 8.48871 0.91411L6.06907 3.69476C5.95028 3.83127 5.88486 4.00613 5.88486 4.18709L5.88486 6.5C5.88486 6.63807 5.77293 6.75 5.63486 6.75H3.63486Z",
                     stroke: "#343434",
                     strokeWidth: "0.5"
                 })),
-                k = () => o().createElement("svg", {
+                _ = () => o().createElement("svg", {
                     width: "13",
                     height: "10",
                     viewBox: "0 0 9 7",
                     fill: "none",
                     xmlns: "http://www.w3.org/2000/svg"
                 }, o().createElement("path", {
                     d: "M3.63481 6.75C3.49674 6.75 3.38481 6.63807 3.38481 6.5V4.18709C3.38481 4.00613 3.31939 3.83127 3.2006 3.69476L0.780957 0.91411C0.640173 0.75232 0.755085 0.5 0.969552 0.5L8.30007 0.5C8.51453 0.5 8.62945 0.75232 8.48866 0.91411L6.06903 3.69476C5.95024 3.83127 5.88481 4.00613 5.88481 4.18709L5.88481 6.5C5.88481 6.63807 5.77288 6.75 5.63481 6.75H3.63481Z",
@@ -1162,15 +1162,15 @@
                     return !0
                 },
                 we = e => {
                     const t = /[A-z0-9_]+/.exec(e);
                     return null !== t && 1 == t.length && t[0] === e && !be(e)
                 },
                 Se = e => we(e) || 0 === e.length ? "" : e.indexOf(" ") >= 0 ? "Invalid column name. Please remove all spaces." : e.indexOf("-") >= 0 ? 'Invalid column name. Try switching "-" for "_".' : be(e) ? "Invalid column name. Add at least one non-digit." : 'Invalid column name. All characters must be letters, digits, and "_".';
-            class _e extends o().Component {
+            class ke extends o().Component {
                 constructor(e) {
                     super(e), this.updateUnsubmittedNewColumnHeader = e => {
                         const t = e.target.value;
                         this.setState({
                             unsubmittedNewColumnHeader: t
                         }), this.setInvalidInputError(Se(t))
                     }, this.changeColumnHeader = async () => {
@@ -1265,15 +1265,15 @@
                         stroke: "#343434",
                         strokeWidth: "2"
                     })))), o().createElement(Ce, {
                         message: this.state.invalidInputError
                     }))
                 }
             }
-            const ke = _e,
+            const _e = ke,
                 Ae = function(e) {
                     const [t, n] = (0, i.useState)({}), [a, s] = (0, i.useState)(!0);
                     return (0, i.useEffect)((() => {
                         !async function() {
                             const t = await e.mitoAPI.getColumnDescribe(e.selectedSheetIndex, e.columnHeader);
                             n(t), s(!1)
                         }()
@@ -1352,15 +1352,15 @@
             var Me;
             ! function(e) {
                 e[e.FilterSort = 0] = "FilterSort", e[e.SummaryStats = 1] = "SummaryStats"
             }(Me || (Me = {}));
             const Le = function(e) {
                     return o().createElement(o().Fragment, null, o().createElement("div", {
                         className: "control-panel-taskpane-container default-taskpane-div"
-                    }, o().createElement(ke, {
+                    }, o().createElement(_e, {
                         columnHeader: e.columnHeader,
                         openEditingColumnHeader: e.openEditingColumnHeader,
                         selectedSheetIndex: e.selectedSheetIndex,
                         mitoAPI: e.mitoAPI,
                         setCurrOpenTaskpane: e.setCurrOpenTaskpane
                     }), o().createElement("div", {
                         className: "default-taskpane-body-div mb-30px"
@@ -1543,15 +1543,15 @@
                         },
                         className: "column-header-column-header mr-1"
                     }, t)), o().createElement("div", {
                         className: "column-header-icon-container"
                     }, o().createElement("div", {
                         id: "filter-icon",
                         onClick: n
-                    }, 0 === e.filters.length && o().createElement(_, null), 0 !== e.filters.length && o().createElement(k, null)), o().createElement("div", {
+                    }, 0 === e.filters.length && o().createElement(k, null), 0 !== e.filters.length && o().createElement(_, null)), o().createElement("div", {
                         onClick: n
                     }, (a = e.columnMitoType) === Oa.STRING_SERIES ? o().createElement(De, null) : a === Oa.NUMBER_SERIES ? o().createElement(Be, null) : a === Oa.DATETIME_SERIES ? o().createElement(Fe, null) : a === Oa.TIMEDELTA_SERIES ? o().createElement(Pe, null) : a === Oa.BOOLEAN_SERIES ? o().createElement(Re, null) : o().createElement(De, null))));
                     var a
                 },
                 Ue = "mito_index";
 
             function He(e, t) {
@@ -2715,15 +2715,15 @@
                     r: "6.75",
                     stroke: "#404040",
                     strokeWidth: "0.6"
                 }), o().createElement("path", {
                     d: "M7.27173 8.43865C7.2624 8.34531 7.2624 8.30798 7.2624 8.26131C7.2624 7.89731 7.38373 7.56131 7.67307 7.36531L8.1024 7.07598C8.64373 6.71198 9.0544 6.19865 9.0544 5.45198C9.0544 4.49998 8.31707 3.57598 7.0104 3.57598C5.57307 3.57598 4.94773 4.63065 4.94773 5.48931C4.94773 5.65731 4.9664 5.80665 5.00373 5.93731L5.90907 6.04931C5.87173 5.94665 5.84373 5.75065 5.84373 5.59198C5.84373 5.00398 6.1984 4.39731 7.0104 4.39731C7.75707 4.39731 8.12107 4.91065 8.12107 5.46131C8.12107 5.82531 7.94373 6.16131 7.6264 6.37598L7.21573 6.65598C6.66507 7.02931 6.44107 7.49598 6.44107 8.11198C6.44107 8.23331 6.44107 8.32665 6.4504 8.43865H7.27173ZM6.24507 9.77331C6.24507 10.1093 6.51573 10.38 6.85173 10.38C7.18773 10.38 7.46773 10.1093 7.46773 9.77331C7.46773 9.43731 7.18773 9.15731 6.85173 9.15731C6.51573 9.15731 6.24507 9.43731 6.24507 9.77331Z",
                     fill: "#343434"
                 })),
-                _t = () => o().createElement("svg", {
+                kt = () => o().createElement("svg", {
                     width: "25",
                     height: "25",
                     viewBox: "0 0 14 14",
                     fill: "none",
                     xmlns: "http://www.w3.org/2000/svg"
                 }, o().createElement("path", {
                     d: "M13.3141 1.00002C13.3141 0.834334 13.1798 0.700019 13.0141 0.70002L10.3141 0.700019C10.1484 0.70002 10.0141 0.834334 10.0141 1.00002C10.0141 1.1657 10.1484 1.30002 10.3141 1.30002H12.7141V3.70002C12.7141 3.8657 12.8484 4.00002 13.0141 4.00002C13.1798 4.00002 13.3141 3.86571 13.3141 3.70002L13.3141 1.00002ZM8.07966 6.35874L13.2262 1.21215L12.802 0.787887L7.65539 5.93447L8.07966 6.35874Z",
@@ -2734,15 +2734,15 @@
                 }), o().createElement("path", {
                     d: "M13.1141 13.2999C13.2798 13.2997 13.4139 13.1652 13.4137 12.9995L13.4105 10.2995C13.4103 10.1338 13.2759 9.99968 13.1102 9.99987C12.9445 10.0001 12.8103 10.1345 12.8105 10.3002L12.8134 12.7002L10.4134 12.7031C10.2477 12.7033 10.1135 12.8377 10.1137 13.0034C10.1139 13.1691 10.2484 13.3033 10.4141 13.3031L13.1141 13.2999ZM7.74918 8.07176L12.9019 13.2123L13.3256 12.7875L8.17294 7.64699L7.74918 8.07176Z",
                     fill: "#343434"
                 }), o().createElement("path", {
                     d: "M0.994269 0.799772C0.828614 0.802948 0.696899 0.939813 0.700076 1.10547L0.751844 3.80497C0.755021 3.97063 0.891886 4.10234 1.05754 4.09916C1.2232 4.09599 1.35491 3.95912 1.35173 3.79347L1.30572 1.39391L3.70528 1.34789C3.87093 1.34472 4.00265 1.20785 3.99947 1.0422C3.99629 0.876542 3.85943 0.744827 3.69377 0.748004L0.994269 0.799772ZM6.45153 5.92971L1.20805 0.883556L0.791995 1.31588L6.03547 6.36203L6.45153 5.92971Z",
                     fill: "#343434"
                 })),
-                kt = () => o().createElement("svg", {
+                _t = () => o().createElement("svg", {
                     width: "25",
                     height: "25",
                     viewBox: "0 0 16 16",
                     fill: "none",
                     xmlns: "http://www.w3.org/2000/svg"
                 }, o().createElement("path", {
                     d: "M9.69561 5.99947C9.69531 6.16516 9.82939 6.29971 9.99508 6.3L12.6951 6.30476C12.8608 6.30505 12.9953 6.17097 12.9956 6.00529C12.9959 5.8396 12.8618 5.70505 12.6961 5.70476L10.2961 5.70053L10.3004 3.30053C10.3007 3.13485 10.1666 3.0003 10.0009 3C9.83521 2.99971 9.70066 3.13379 9.70037 3.29948L9.69561 5.99947ZM13.798 1.78749L9.78385 5.78749L10.2074 6.21251L14.2215 2.21251L13.798 1.78749Z",
@@ -3020,22 +3020,22 @@
                     }, o().createElement(St, null)), o().createElement("p", {
                         className: "mito-toolbar-item-label"
                     }, "Docs")), t && o().createElement("button", {
                         className: "mito-toolbar-item",
                         onClick: a
                     }, o().createElement("div", {
                         className: "mito-toolbar-item-icon-container"
-                    }, o().createElement(kt, null)), o().createElement("p", {
+                    }, o().createElement(_t, null)), o().createElement("p", {
                         className: "mito-toolbar-item-label"
                     }, "Fullscreen")), !t && o().createElement("button", {
                         className: "mito-toolbar-item",
                         onClick: a
                     }, o().createElement("div", {
                         className: "mito-toolbar-item-icon-container"
-                    }, o().createElement(_t, null)), o().createElement("p", {
+                    }, o().createElement(kt, null)), o().createElement("p", {
                         className: "mito-toolbar-item-label"
                     }, "Fullscreen"))))
                 };
             var It = n(9369);
             c()(It.Z, {
                 insert: "head",
                 singleton: !1
@@ -4059,23 +4059,23 @@
                         className: "documentation-basic-example-instructions-list-element-content-centered mb-1"
                     }, "=LEFT(FirstColumn)"), "Replace FirstColumn with the name of the first column in your data. The column will update with the first characters from the first column!")), o().createElement("li", {
                         className: "documentation-basic-example-instructions-list-element"
                     }, o().createElement("div", null, "4."), o().createElement("div", {
                         className: "documentation-basic-example-instructions-list-element-content"
                     }, "To see a full list of the functions available, click the back arrow at the top of this taskpane and scroll down!"))))
                 }],
-                _n = e => {
+                kn = e => {
                     const t = Sn.find((t => t.basicExampleName == e.basicExampleName));
                     return o().createElement(o().Fragment, null, null == t ? void 0 : t.content())
                 };
-            var kn = n(2092);
-            c()(kn.Z, {
+            var _n = n(2092);
+            c()(_n.Z, {
                 insert: "head",
                 singleton: !1
-            }), kn.Z.locals;
+            }), _n.Z.locals;
             const An = "What is the most frustrating thing about Mito? Please be as specific as possible!",
                 Nn = "I struggled to create a pivot table because I did not understand how to switch the aggregation methods. Also, it would be nice to set color of cells in the sheet to present data to my coworkers.",
                 Tn = (e, t) => 2 === t && e <= 1 ? {
                     question: An,
                     placeholder: Nn
                 } : 5 === t && e <= 2 ? {
                     question: "What features/functionality are you finding most valuable with Mito? Please be as specific as possible!",
@@ -4101,15 +4101,15 @@
                     }), []), o().createElement(Xt, {
                         header: "Please provide feedback!",
                         setCurrOpenTaskpane: e.setCurrOpenTaskpane,
                         notCloseable: e.openLocation === On.AUTO_POPUP,
                         taskpaneBody: o().createElement(i.Fragment, null, o().createElement("p", {
                             className: "mb-10px txt-15"
                         }, n), o().createElement("textarea", {
-                            className: "feedback-taskpane-textarea",
+                            className: "feedback-taskpane-textarea feedback-taskpane-textarea-tall",
                             style: {
                                 border: l ? "2px solid red" : "1px solid black"
                             },
                             placeholder: a,
                             value: s,
                             onChange: e => {
                                 r(e.target.value)
@@ -4279,15 +4279,15 @@
                         strokeWidth: "2"
                     })))), o().createElement("div", {
                         className: "default-taskpane-body-div"
                     }, void 0 === t ? o().createElement(Ln, {
                         setCurrOpenTaskpane: e.setCurrOpenTaskpane,
                         setSelectedDocumentation: n,
                         mitoAPI: e.mitoAPI
-                    }) : "basic" === t.kind ? o().createElement(_n, {
+                    }) : "basic" === t.kind ? o().createElement(kn, {
                         basicExampleName: t.basicExampleName
                     }) : "function" === t.kind ? o().createElement(yn, {
                         function: t.function
                     }) : void 0))
                 },
                 Dn = e => o().createElement("svg", {
                     style: {
@@ -5504,15 +5504,15 @@
                         onChange: e => {
                             a(e.target.value)
                         }
                     }), o().createElement("label", null, o().createElement("h3", {
                         className: "mt-25px mb-10px"
                     }, s)), o().createElement("textarea", {
                         required: !0,
-                        className: "feedback-taskpane-textarea",
+                        className: "feedback-taskpane-textarea feedback-taskpane-textarea-small",
                         placeholder: "I struggle to merge two dataframes on a shared ID column in Pandas using pd.merge(). Specifically, it is hard to understand which columns I want to keep from which dataset while I am merging them.",
                         value: r,
                         onChange: e => {
                             l(e.target.value)
                         }
                     })), o().createElement("div", {
                         className: "signup-modal-buttons"
@@ -5775,15 +5775,15 @@
                         return o().createElement(wt, null);
                     case Vn.DeleteColumn:
                         return o().createElement(bt, null);
                     case Vn.RenameColumn:
                     case Vn.ReorderColumn:
                         return o().createElement(Xn, null);
                     case Vn.FilterColumn:
-                        return o().createElement(_, {
+                        return o().createElement(k, {
                             height: "20",
                             width: "20"
                         });
                     case Vn.SetColumnFormula:
                         return o().createElement("div", {
                             className: "step-taskpane-missing-icon"
                         }, "Fx");
@@ -6334,15 +6334,15 @@
                     stepHeader: "See all of Mito's formulas",
                     stepHeaderBackgroundColor: "#79C2F8",
                     stepText: o().createElement("div", null, "Congrats on writing your first formula! To see a full list of Mito’s functions, ", o().createElement("b", null, "click on the Docs"), " button in the top right corner of Mito."),
                     location: ya.BOTTOM_LEFT,
                     advanceButtonText: "Continue",
                     displayBackButton: !0
                 }],
-                _a = [{
+                ka = [{
                     tourName: Ea.EXPLORE_DATA,
                     stepNumber: 1,
                     stepHeader: "Exploring data with Mito",
                     stepHeaderBackgroundColor: "#BCDFBC",
                     stepText: o().createElement("div", null, " Mito makes it easy to build intuition for your data by automatically generating summary information about each column. To get started, ", o().createElement("b", null, "click on the filter button in the column header"), " of one of your columns."),
                     location: ya.BOTTOM_LEFT,
                     advanceButtonText: "Continue",
@@ -6380,15 +6380,15 @@
                     stepHeader: "Enjoy your cleaned data",
                     stepHeaderBackgroundColor: "#FFCBDE",
                     stepText: o().createElement("div", null, "Nice work! In just a few clicks, we’ve built some intuition for our data and removed the values we're not interested in. "),
                     location: ya.BOTTOM_LEFT,
                     advanceButtonText: "Continue",
                     displayBackButton: !0
                 }],
-                ka = {
+                _a = {
                     Intro: ba,
                     Pivot: wa,
                     Tutorial: [{
                         tourName: Ea.TUTORIAL,
                         stepNumber: 1,
                         stepHeader: "Before you go!",
                         stepHeaderBackgroundColor: "#FFDAAE",
@@ -6401,26 +6401,26 @@
                             }
                         }, "here"), "."),
                         location: ya.BOTTOM_LEFT,
                         advanceButtonText: "Close",
                         displayBackButton: !0
                     }],
                     Column_Formulas: Sa,
-                    Explore_Datasets: _a
+                    Explore_Datasets: ka
                 },
                 Aa = {
                     [ya.BOTTOM_LEFT]: "tour-container tour-container-bottom-left",
                     [ya.BOTTOM_RIGHT]: "tour-container tour-container-bottom-right",
                     [ya.TOP_LEFT]: "tour-container tour-container-top-left",
                     [ya.TOP_RIGHT]: "tour-container tour-container-top-right"
                 },
                 Na = e => {
                     const [t, n] = (0, i.useState)(0), [a, s] = (0, i.useState)(!1), r = [];
                     e.tourNames.forEach((e => {
-                        r.push(...ka[e])
+                        r.push(..._a[e])
                     })), (0, i.useEffect)((() => {
                         e.mitoAPI.sendLogMessage("begin_tour", {
                             tour_names: e.tourNames,
                             total_number_of_tour_steps: r.length
                         })
                     }), []), (0, i.useEffect)((() => {
                         r[t].tourName === Ea.PIVOT && 1 === r[t].stepNumber ? e.setHighlightPivotTableButton(!0) : r[t].tourName === Ea.COLUMN_FORMULAS && 1 === r[t].stepNumber ? e.setHighlightAddColButton(!0) : (e.setHighlightPivotTableButton(!1), e.setHighlightAddColButton(!1))
@@ -7769,15 +7769,15 @@
             n.d(t, {
                 Z: () => i
             });
             var a = n(3645),
                 s = n.n(a)()((function(e) {
                     return e[1]
                 }));
-            s.push([e.id, ".feedback-taskpane-answer-container {\n    margin: auto;\n    width: 90%;\n}\n\n.feedback-taskpane-textarea {\n    resize: none;\n\n    margin: 0px;\n\n    width: 90%;\n    height: 200px;\n\n    background-color: #F8F8F8;\n\n    border: 1px solid var(--mito-grey);\n    border-radius: 3px;\n\n    font-family: var(--jp-ui-font-family);\n    font-size: 12px;\n}", ""]);
+            s.push([e.id, ".feedback-taskpane-answer-container {\n    margin: auto;\n    width: 90%;\n}\n\n.feedback-taskpane-textarea {\n    resize: none;\n\n    margin: 0px;\n\n    width: 90%;\n\n    background-color: #F8F8F8;\n\n    border: 1px solid var(--mito-grey);\n    border-radius: 3px;\n\n    font-family: var(--jp-ui-font-family);\n    font-size: 12px;\n}\n\n.feedback-taskpane-textarea-small {\n    height: 75px;\n}\n\n.feedback-taskpane-textarea-tall {\n    height: 200px;\n}", ""]);
             const i = s
         },
         837: (e, t, n) => {
             "use strict";
             n.d(t, {
                 Z: () => i
             });
@@ -8242,11 +8242,11 @@
                     return e[1]
                 }));
             s.push([e.id, "/* Width css tags to be used across project \n   in the format: .w-{number} where number can be any multiple of 5 */\n\n\n.w-5 {\n    width: 5vw;\n}\n\n.w-8 {\n    width: 8vw;\n}\n\n.w-10 {\n    width: 10vw;\n}\n\n.w-15 {\n    width: 15vw;\n}\n\n.w-20 {\n    width: 20vw;\n}\n\n.w-25 {\n    width: 25vw;\n}\n\n.w-30 {\n    width: 30vw;\n}\n\n.w-35 {\n    width: 35vw;\n}\n\n.w-40 {\n    width: 40vw;\n}\n\n.w-45 {\n    width: 45vw;\n}\n\n.w-50 {\n    width: 50vw;\n}\n\n.w-55 {\n    width: 55vw;\n}\n\n.w-60 {\n    width: 60vw;\n}\n\n.w-65 {\n    width: 65vw;\n}\n\n.w-70 {\n    width: 70vw;\n}\n\n.w-75 {\n    width: 75vw;\n}\n\n.w-80 {\n    width: 80vw;\n}\n\n.w-85 {\n    width: 85vw;\n}\n\n.w-90 {\n    width: 90vw;\n}\n\n.w-95 {\n    width: 95vw;\n}\n\n.w-100 {\n    width: 100vw;\n}\n\n.w-90p {\n    width: 90%;\n}\n\n.w-100p {\n    width: 100%;\n}", ""]);
             const i = s
         },
         306: e => {
             "use strict";
-            e.exports = JSON.parse('{"files":["lib/**/*.js","dist/*.js","css/**/*.css","style/index.js"],"jupyterlab":{"outputDir":"mitosheet/labextension","extension":"lib/plugin"},"name":"mitosheet3","license":"Other/Proprietary License","author":{"name":"Mito Sheet","email":"naterush1997@gmail.com"},"bugs":{"url":"https://github.com/mito/mito/issues"},"repository":{"url":"https://github.com/mito/mito","type":"git"},"version":"0.3.91","dependencies":{"@jupyter-widgets/base":"^4","@jupyterlab/notebook":"^3.0.6","@types/fscreen":"^1.0.1","@types/react":"^16.9.49","@types/react-dom":"^17.0.2","ag-grid-community":"^24.0.0","ag-grid-react":"^24.0.0","fscreen":"^1.1.0","react":"^17.0.1","react-dom":"^17.0.1","react-intercom":"^1.0.15"},"scripts":{"test:ga:1":"testcafe chrome tests/1/","test:ga:3":"testcafe chrome tests/3/","test:ga:2":"testcafe chrome tests/2/","test:ga:5":"testcafe chrome tests/5/","test:ga:4":"testcafe chrome tests/4/","test:ga:6":"testcafe chrome tests/6/","deploy:staging":"python3 deployment/deploy.py staging","build:prod":"jlpm run build:lib && jlpm run build:labextension","clean:labextension":"rimraf mitosheet/labextension","deploy:app":"python3 deployment/deploy.py app","build:labextension:dev":"jupyter labextension build --development True .","prepare":"jlpm run clean && jlpm run build:prod","watch:lib":"tsc -w","build:labextension":"jupyter labextension build .","deploy:all":"python3 deployment/deploy.py all","test:local":"export JUPYTER_LAB_LOCAL_TOKEN=`jupyter notebook list | sed -n 2p | cut -d\' \' -f1 | cut -d\'=\' -f2` && export LOCAL_TEST=\\"True\\" && testcafe chrome tests/","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:lib":"tsc","deploy:pypi":"python3 setup.py sdist bdist_wheel upload","clean:nbextension":"rimraf mitosheet/nbextension/static/index.js","build:all":"npm run build:labextension && npm run build:nbextension","lint:check":"eslint src/ --ext .ts,.tsx","watch:nbextension":"webpack --watch","lint":"eslint src/ --ext .ts,.tsx --fix","watch":"run-p watch:src watch:labextension","watch:labextension":"jupyter labextension watch .","install:extension":"jupyter labextension develop --overwrite .","clean:lib":"rimraf lib tsconfig.tsbuildinfo","prepack":"npm run build:lib","test:local:noauth":"testcafe chrome tests/","watch:src":"tsc -w","clean":"jlpm run clean:lib","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","test:remote":"export LOCAL_TEST=\\"False\\"; testcafe chrome tests/"},"keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/expect.js":"^0.3.29","@types/mocha":"^5.2.5","@types/node":"^14.14.35","@typescript-eslint/eslint-plugin":"^4.8.1","@typescript-eslint/parser":"^4.8.1","acorn":"^7.2.0","application":"npm:@lumino/application@^1.13.1","eslint":"^7.14.0","eslint-config-prettier":"^6.15.0","eslint-plugin-office-addins":"^0.1.7","eslint-plugin-prettier":"^3.1.4","eslint-plugin-react":"^7.21.3","expect.js":"^0.3.1","fs-extra":"^7.0.0","mkdirp":"^0.5.1","mocha":"^5.2.0","npm-run-all":"^4.1.5","prettier":"^2.1.1","rimraf":"^3.0.2","testcafe":"^1.9.4","typescript":"~4.1.3","widgets":"npm:@lumino/widgets@^1.16.1"},"main":"lib/index.js","homepage":"https://github.com/mito/mito","types":"./lib/index.d.ts","description":"The Mito Spreadsheet","versions":{"mitosheet":"0.1.301","mitosheet3":"0.3.91"},"resolutions":{"@types/react":"^17.0.2"}}')
+            e.exports = JSON.parse('{"files":["lib/**/*.js","dist/*.js","css/**/*.css","style/index.js"],"jupyterlab":{"outputDir":"mitosheet/labextension","extension":"lib/plugin"},"name":"mitosheet3","license":"Other/Proprietary License","author":{"name":"Mito Sheet","email":"naterush1997@gmail.com"},"bugs":{"url":"https://github.com/mito/mito/issues"},"repository":{"url":"https://github.com/mito/mito","type":"git"},"version":"0.3.92","dependencies":{"@jupyter-widgets/base":"^4","@jupyterlab/notebook":"^3.0.6","@types/fscreen":"^1.0.1","@types/react":"^16.9.49","@types/react-dom":"^17.0.2","ag-grid-community":"^24.0.0","ag-grid-react":"^24.0.0","fscreen":"^1.1.0","react":"^17.0.1","react-dom":"^17.0.1","react-intercom":"^1.0.15"},"scripts":{"test:ga:1":"testcafe chrome tests/1/","test:ga:3":"testcafe chrome tests/3/","test:ga:2":"testcafe chrome tests/2/","test:ga:5":"testcafe chrome tests/5/","test:ga:4":"testcafe chrome tests/4/","test:ga:6":"testcafe chrome tests/6/","deploy:staging":"python3 deployment/deploy.py staging","build:prod":"jlpm run build:lib && jlpm run build:labextension","clean:labextension":"rimraf mitosheet/labextension","deploy:app":"python3 deployment/deploy.py app","build:labextension:dev":"jupyter labextension build --development True .","prepare":"jlpm run clean && jlpm run build:prod","watch:lib":"tsc -w","build:labextension":"jupyter labextension build .","deploy:all":"python3 deployment/deploy.py all","test:local":"export JUPYTER_LAB_LOCAL_TOKEN=`jupyter notebook list | sed -n 2p | cut -d\' \' -f1 | cut -d\'=\' -f2` && export LOCAL_TEST=\\"True\\" && testcafe chrome tests/","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:lib":"tsc","deploy:pypi":"python3 setup.py sdist bdist_wheel upload","clean:nbextension":"rimraf mitosheet/nbextension/static/index.js","build:all":"npm run build:labextension && npm run build:nbextension","lint:check":"eslint src/ --ext .ts,.tsx","watch:nbextension":"webpack --watch","lint":"eslint src/ --ext .ts,.tsx --fix","watch":"run-p watch:src watch:labextension","watch:labextension":"jupyter labextension watch .","install:extension":"jupyter labextension develop --overwrite .","clean:lib":"rimraf lib tsconfig.tsbuildinfo","prepack":"npm run build:lib","test:local:noauth":"testcafe chrome tests/","watch:src":"tsc -w","clean":"jlpm run clean:lib","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","test:remote":"export LOCAL_TEST=\\"False\\"; testcafe chrome tests/"},"keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/expect.js":"^0.3.29","@types/mocha":"^5.2.5","@types/node":"^14.14.35","@typescript-eslint/eslint-plugin":"^4.8.1","@typescript-eslint/parser":"^4.8.1","acorn":"^7.2.0","application":"npm:@lumino/application@^1.13.1","eslint":"^7.14.0","eslint-config-prettier":"^6.15.0","eslint-plugin-office-addins":"^0.1.7","eslint-plugin-prettier":"^3.1.4","eslint-plugin-react":"^7.21.3","expect.js":"^0.3.1","fs-extra":"^7.0.0","mkdirp":"^0.5.1","mocha":"^5.2.0","npm-run-all":"^4.1.5","prettier":"^2.1.1","rimraf":"^3.0.2","testcafe":"^1.9.4","typescript":"~4.1.3","widgets":"npm:@lumino/widgets@^1.16.1"},"main":"lib/index.js","homepage":"https://github.com/mito/mito","types":"./lib/index.d.ts","description":"The Mito Spreadsheet","versions":{"mitosheet":"0.1.302","mitosheet3":"0.3.92"},"resolutions":{"@types/react":"^17.0.2"}}')
         }
     }
 ]);
```

### Comparing `mitosheet3-0.3.91/mitosheet/labextension/static/534.ecfeee9921699bf3929e.js` & `mitosheet3-0.3.92/mitosheet/labextension/static/534.ecfeee9921699bf3929e.js`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/labextension/static/7.a501bf39686c40af057f.js` & `mitosheet3-0.3.92/mitosheet/labextension/static/7.a501bf39686c40af057f.js`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/labextension/static/812.a706af7a2a6413de9561.js` & `mitosheet3-0.3.92/mitosheet/labextension/static/812.a706af7a2a6413de9561.js`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/labextension/static/853.4123dc4d2193c3ad8e88.js` & `mitosheet3-0.3.92/mitosheet/labextension/static/853.4123dc4d2193c3ad8e88.js`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/labextension/static/remoteEntry.25954ef11e950542a78c.js` & `mitosheet3-0.3.92/mitosheet/labextension/static/remoteEntry.84d311aab4baee4ad12b.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -49,29 +49,29 @@
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
         0: "bdbf1960886caa2f64e0",
         7: "a501bf39686c40af057f",
         149: "a955b532a2f6424f09da",
         271: "b12d65aaeb668713705e",
         456: "1c9d5aa965fa68882990",
         461: "cc00aa043b123b43d40d",
-        480: "e084e61bbf78e5e83444",
+        480: "b800b2485bc1f4911b0e",
         534: "ecfeee9921699bf3929e",
         568: "e067c39c389e7e86b7ee",
         812: "a706af7a2a6413de9561",
         853: "4123dc4d2193c3ad8e88",
         856: "3754844c2b5b35b64be1",
         972: "262f36949d3bbf1cb5e6"
     } [e] + ".js?v=" + {
         0: "bdbf1960886caa2f64e0",
         7: "a501bf39686c40af057f",
         149: "a955b532a2f6424f09da",
         271: "b12d65aaeb668713705e",
         456: "1c9d5aa965fa68882990",
         461: "cc00aa043b123b43d40d",
-        480: "e084e61bbf78e5e83444",
+        480: "b800b2485bc1f4911b0e",
         534: "ecfeee9921699bf3929e",
         568: "e067c39c389e7e86b7ee",
         812: "a706af7a2a6413de9561",
         853: "4123dc4d2193c3ad8e88",
         856: "3754844c2b5b35b64be1",
         972: "262f36949d3bbf1cb5e6"
     } [e], w.g = function() {
@@ -131,15 +131,15 @@
                             from: i,
                             eager: !!a
                         })
                     },
                     l = [];
                 switch (t) {
                     case "default":
-                        d("@jupyter-widgets/base", "4.0.0", (() => Promise.all([w.e(534), w.e(856)]).then((() => () => w(3534))))), d("ag-grid-community", "24.1.0", (() => w.e(853).then((() => () => w(853))))), d("ag-grid-react", "24.1.1", (() => Promise.all([w.e(0), w.e(271), w.e(456), w.e(972)]).then((() => () => w(4e3))))), d("fscreen", "1.2.0", (() => w.e(7).then((() => () => w(2007))))), d("mitosheet3", "0.3.91", (() => Promise.all([w.e(812), w.e(271), w.e(456), w.e(480), w.e(568)]).then((() => () => w(1568))))), d("react-intercom", "1.0.15", (() => Promise.all([w.e(271), w.e(149)]).then((() => () => w(8149)))))
+                        d("@jupyter-widgets/base", "4.0.0", (() => Promise.all([w.e(534), w.e(856)]).then((() => () => w(3534))))), d("ag-grid-community", "24.1.0", (() => w.e(853).then((() => () => w(853))))), d("ag-grid-react", "24.1.1", (() => Promise.all([w.e(0), w.e(271), w.e(456), w.e(972)]).then((() => () => w(4e3))))), d("fscreen", "1.2.0", (() => w.e(7).then((() => () => w(2007))))), d("mitosheet3", "0.3.92", (() => Promise.all([w.e(812), w.e(271), w.e(456), w.e(480), w.e(568)]).then((() => () => w(1568))))), d("react-intercom", "1.0.15", (() => Promise.all([w.e(271), w.e(149)]).then((() => () => w(8149)))))
                 }
                 return e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
```

### Comparing `mitosheet3-0.3.91/mitosheet/mito_analytics.py` & `mitosheet3-0.3.92/mitosheet/mito_analytics.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/mito_widget.py` & `mitosheet3-0.3.92/mitosheet/mito_widget.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/parser.py` & `mitosheet3-0.3.92/mitosheet/parser.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/preprocessing/__init__.py` & `mitosheet3-0.3.92/mitosheet/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/preprocessing/preprocess_check_args_type.py` & `mitosheet3-0.3.92/mitosheet/preprocessing/preprocess_check_args_type.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/preprocessing/preprocess_copy.py` & `mitosheet3-0.3.92/mitosheet/preprocessing/preprocess_copy.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/preprocessing/preprocess_read_file_paths.py` & `mitosheet3-0.3.92/mitosheet/preprocessing/preprocess_read_file_paths.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/preprocessing/preprocess_rename_headers.py` & `mitosheet3-0.3.92/mitosheet/preprocessing/preprocess_rename_headers.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/profiling.py` & `mitosheet3-0.3.92/mitosheet/profiling.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/save_utils.py` & `mitosheet3-0.3.92/mitosheet/save_utils.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/saves/__init__.py` & `mitosheet3-0.3.92/mitosheet/saves/__init__.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/saves/mito_simple_raw_import.py` & `mitosheet3-0.3.92/mitosheet/saves/mito_simple_raw_import.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/saves/tutorial_v3/mito_tutorial_checkpoint_2.py` & `mitosheet3-0.3.92/mitosheet/saves/tutorial_v3/mito_tutorial_checkpoint_2.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/saves/tutorial_v3/mito_tutorial_checkpoint_3.py` & `mitosheet3-0.3.92/mitosheet/saves/tutorial_v3/mito_tutorial_checkpoint_3.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/saves/tutorial_v3/mito_tutorial_checkpoint_4.py` & `mitosheet3-0.3.92/mitosheet/saves/tutorial_v3/mito_tutorial_checkpoint_4.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/saves/tutorial_v3/mito_tutorial_checkpoint_5.py` & `mitosheet3-0.3.92/mitosheet/saves/tutorial_v3/mito_tutorial_checkpoint_5.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/saves/tutorial_v3/mito_tutorial_checkpoint_6.py` & `mitosheet3-0.3.92/mitosheet/saves/tutorial_v3/mito_tutorial_checkpoint_6.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/sheet_functions/__init__.py` & `mitosheet3-0.3.92/mitosheet/sheet_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/sheet_functions/control_functions.py` & `mitosheet3-0.3.92/mitosheet/sheet_functions/control_functions.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/sheet_functions/date_functions.py` & `mitosheet3-0.3.92/mitosheet/sheet_functions/date_functions.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/sheet_functions/misc_functions.py` & `mitosheet3-0.3.92/mitosheet/sheet_functions/misc_functions.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/sheet_functions/number_functions.py` & `mitosheet3-0.3.92/mitosheet/sheet_functions/number_functions.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/sheet_functions/sheet_function_utils.py` & `mitosheet3-0.3.92/mitosheet/sheet_functions/sheet_function_utils.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/sheet_functions/string_functions.py` & `mitosheet3-0.3.92/mitosheet/sheet_functions/string_functions.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/sheet_functions/types/__init__.py` & `mitosheet3-0.3.92/mitosheet/sheet_functions/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/sheet_functions/types/decorators.py` & `mitosheet3-0.3.92/mitosheet/sheet_functions/types/decorators.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/sheet_functions/types/to_boolean_series.py` & `mitosheet3-0.3.92/mitosheet/sheet_functions/types/to_boolean_series.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/sheet_functions/types/to_datetime_series.py` & `mitosheet3-0.3.92/mitosheet/sheet_functions/types/to_datetime_series.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/sheet_functions/types/to_number_series.py` & `mitosheet3-0.3.92/mitosheet/sheet_functions/types/to_number_series.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/sheet_functions/types/to_string_series.py` & `mitosheet3-0.3.92/mitosheet/sheet_functions/types/to_string_series.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/sheet_functions/types/utils.py` & `mitosheet3-0.3.92/mitosheet/sheet_functions/types/utils.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/steps/__init__.py` & `mitosheet3-0.3.92/mitosheet/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/steps/column_steps/add_column.py` & `mitosheet3-0.3.92/mitosheet/steps/column_steps/add_column.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/steps/column_steps/change_column_dtype.py` & `mitosheet3-0.3.92/mitosheet/steps/column_steps/change_column_dtype.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/steps/column_steps/delete_column.py` & `mitosheet3-0.3.92/mitosheet/steps/column_steps/delete_column.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/steps/column_steps/rename_column.py` & `mitosheet3-0.3.92/mitosheet/steps/column_steps/rename_column.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/steps/column_steps/reorder_column.py` & `mitosheet3-0.3.92/mitosheet/steps/column_steps/reorder_column.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/steps/column_steps/set_column_formula.py` & `mitosheet3-0.3.92/mitosheet/steps/column_steps/set_column_formula.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/steps/dataframe_steps/dataframe_delete.py` & `mitosheet3-0.3.92/mitosheet/steps/dataframe_steps/dataframe_delete.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/steps/dataframe_steps/dataframe_duplicate.py` & `mitosheet3-0.3.92/mitosheet/steps/dataframe_steps/dataframe_duplicate.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/steps/dataframe_steps/dataframe_rename.py` & `mitosheet3-0.3.92/mitosheet/steps/dataframe_steps/dataframe_rename.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/steps/filter.py` & `mitosheet3-0.3.92/mitosheet/steps/filter.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/steps/import_steps/raw_python_import.py` & `mitosheet3-0.3.92/mitosheet/steps/import_steps/raw_python_import.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/steps/import_steps/simple_import.py` & `mitosheet3-0.3.92/mitosheet/steps/import_steps/simple_import.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/steps/initalize.py` & `mitosheet3-0.3.92/mitosheet/steps/initalize.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/steps/merge.py` & `mitosheet3-0.3.92/mitosheet/steps/merge.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/steps/pivot.py` & `mitosheet3-0.3.92/mitosheet/steps/pivot.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/steps/sort.py` & `mitosheet3-0.3.92/mitosheet/steps/sort.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/tests/conftest.py` & `mitosheet3-0.3.92/mitosheet/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/tests/test_example.py` & `mitosheet3-0.3.92/mitosheet/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/tests/test_execution_errors.py` & `mitosheet3-0.3.92/mitosheet/tests/test_execution_errors.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/tests/test_format.py` & `mitosheet3-0.3.92/mitosheet/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/tests/test_mitosheet_utils.py` & `mitosheet3-0.3.92/mitosheet/tests/test_mitosheet_utils.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/tests/test_parse.py` & `mitosheet3-0.3.92/mitosheet/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/tests/test_save_utils.py` & `mitosheet3-0.3.92/mitosheet/tests/test_save_utils.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/tests/test_step_format.py` & `mitosheet3-0.3.92/mitosheet/tests/test_step_format.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/tests/test_topological_sort.py` & `mitosheet3-0.3.92/mitosheet/tests/test_topological_sort.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/tests/test_transpile.py` & `mitosheet3-0.3.92/mitosheet/tests/test_transpile.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/tests/test_ts_types.py` & `mitosheet3-0.3.92/mitosheet/tests/test_ts_types.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/tests/test_upgrade.py` & `mitosheet3-0.3.92/mitosheet/tests/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/tests/test_utils.py` & `mitosheet3-0.3.92/mitosheet/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/tests/test_widget_state_container.py` & `mitosheet3-0.3.92/mitosheet/tests/test_widget_state_container.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/tests/user/conftest.py` & `mitosheet3-0.3.92/mitosheet/tests/user/conftest.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/tests/user/test_user.py` & `mitosheet3-0.3.92/mitosheet/tests/user/test_user.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/tests/user/test_utils.py` & `mitosheet3-0.3.92/mitosheet/tests/user/test_utils.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/topological_sort.py` & `mitosheet3-0.3.92/mitosheet/topological_sort.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/transpiler/transpile.py` & `mitosheet3-0.3.92/mitosheet/transpiler/transpile.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/updates/__init__.py` & `mitosheet3-0.3.92/mitosheet/updates/__init__.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/updates/append_user_field.py` & `mitosheet3-0.3.92/mitosheet/updates/append_user_field.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/updates/args_update.py` & `mitosheet3-0.3.92/mitosheet/updates/args_update.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/updates/checkout_step_by_idx.py` & `mitosheet3-0.3.92/mitosheet/updates/checkout_step_by_idx.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/updates/delete_saved_analysis.py` & `mitosheet3-0.3.92/mitosheet/updates/delete_saved_analysis.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/updates/rename_saved_analysis.py` & `mitosheet3-0.3.92/mitosheet/updates/rename_saved_analysis.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/updates/replay_analysis.py` & `mitosheet3-0.3.92/mitosheet/updates/replay_analysis.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/updates/save_analysis.py` & `mitosheet3-0.3.92/mitosheet/updates/save_analysis.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/updates/set_user_field_update.py` & `mitosheet3-0.3.92/mitosheet/updates/set_user_field_update.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/updates/undo.py` & `mitosheet3-0.3.92/mitosheet/updates/undo.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/upgrade.py` & `mitosheet3-0.3.92/mitosheet/upgrade.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/user/__init__.py` & `mitosheet3-0.3.92/mitosheet/user/__init__.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/user/create.py` & `mitosheet3-0.3.92/mitosheet/user/create.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/user/db.py` & `mitosheet3-0.3.92/mitosheet/user/db.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/user/schemas.py` & `mitosheet3-0.3.92/mitosheet/user/schemas.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/user/upgrade.py` & `mitosheet3-0.3.92/mitosheet/user/upgrade.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/user/utils.py` & `mitosheet3-0.3.92/mitosheet/user/utils.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/utils.py` & `mitosheet3-0.3.92/mitosheet/utils.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet/widget_state_container.py` & `mitosheet3-0.3.92/mitosheet/widget_state_container.py`

 * *Files identical despite different names*

### Comparing `mitosheet3-0.3.91/mitosheet3.egg-info/PKG-INFO` & `mitosheet3-0.3.92/mitosheet3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitosheet3
-Version: 0.3.91
+Version: 0.3.92
 Summary: The Mito Spreadsheet
 Home-page: https://github.com/mito/mito
 Author: Mito Sheet
 Author-email: naterush1997@gmail.com
 License: Other/Proprietary License
 Description: 
                     To learn more about Mito, checkout out our documentation: https://docs.trymito.io/getting-started/installing-mito
```

### Comparing `mitosheet3-0.3.91/mitosheet3.egg-info/SOURCES.txt` & `mitosheet3-0.3.92/mitosheet3.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,23 +30,23 @@
 mitosheet/api/get_path_join.py
 mitosheet/api/get_saved_analysis_description.py
 mitosheet/labextension/package.json
 mitosheet/labextension/static/0.bdbf1960886caa2f64e0.js
 mitosheet/labextension/static/0.bdbf1960886caa2f64e0.js.LICENSE.txt
 mitosheet/labextension/static/149.a955b532a2f6424f09da.js
 mitosheet/labextension/static/461.cc00aa043b123b43d40d.js
-mitosheet/labextension/static/480.e084e61bbf78e5e83444.js
+mitosheet/labextension/static/480.b800b2485bc1f4911b0e.js
 mitosheet/labextension/static/534.ecfeee9921699bf3929e.js
 mitosheet/labextension/static/534.ecfeee9921699bf3929e.js.LICENSE.txt
 mitosheet/labextension/static/568.e067c39c389e7e86b7ee.js
 mitosheet/labextension/static/7.a501bf39686c40af057f.js
 mitosheet/labextension/static/812.a706af7a2a6413de9561.js
 mitosheet/labextension/static/853.4123dc4d2193c3ad8e88.js
 mitosheet/labextension/static/853.4123dc4d2193c3ad8e88.js.LICENSE.txt
-mitosheet/labextension/static/remoteEntry.25954ef11e950542a78c.js
+mitosheet/labextension/static/remoteEntry.84d311aab4baee4ad12b.js
 mitosheet/labextension/static/style.js
 mitosheet/preprocessing/__init__.py
 mitosheet/preprocessing/preprocess_check_args_type.py
 mitosheet/preprocessing/preprocess_copy.py
 mitosheet/preprocessing/preprocess_read_file_paths.py
 mitosheet/preprocessing/preprocess_rename_headers.py
 mitosheet/saves/__init__.py
```

### Comparing `mitosheet3-0.3.91/setup.py` & `mitosheet3-0.3.92/setup.py`

 * *Files identical despite different names*

