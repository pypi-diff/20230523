# Comparing `tmp/pyanalyze-0.8.0.tar.gz` & `tmp/pyanalyze-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyanalyze-0.8.0.tar", last modified: Sun Nov  6 04:20:21 2022, max compression
+gzip compressed data, was "pyanalyze-0.9.0.tar", last modified: Mon Jan 16 21:55:00 2023, max compression
```

## Comparing `pyanalyze-0.8.0.tar` & `pyanalyze-0.9.0.tar`

### file list

```diff
@@ -1,101 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 04:20:21.967749 pyanalyze-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    10173 2022-11-06 04:20:11.000000 pyanalyze-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8081 2022-11-06 04:20:21.967749 pyanalyze-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7385 2022-11-06 04:20:11.000000 pyanalyze-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 04:20:21.963749 pyanalyze-0.8.0/pyanalyze/
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-11-06 04:20:11.000000 pyanalyze-0.8.0/pyanalyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-11-06 04:20:11.000000 pyanalyze-0.8.0/pyanalyze/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4933 2022-11-06 04:20:11.000000 pyanalyze-0.8.0/pyanalyze/analysis_lib.py
--rw-r--r--   0 runner    (1001) docker     (121)    48652 2022-11-06 04:20:11.000000 pyanalyze-0.8.0/pyanalyze/annotations.py
--rw-r--r--   0 runner    (1001) docker     (121)    33157 2022-11-06 04:20:11.000000 pyanalyze-0.8.0/pyanalyze/arg_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     5716 2022-11-06 04:20:11.000000 pyanalyze-0.8.0/pyanalyze/ast_annotator.py
--rw-r--r--   0 runner    (1001) docker     (121)     8927 2022-11-06 04:20:11.000000 pyanalyze-0.8.0/pyanalyze/asynq_checker.py
--rw-r--r--   0 runner    (1001) docker     (121)    18389 2022-11-06 04:20:11.000000 pyanalyze-0.8.0/pyanalyze/attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)     6989 2022-11-06 04:20:11.000000 pyanalyze-0.8.0/pyanalyze/boolability.py
--rw-r--r--   0 runner    (1001) docker     (121)    16160 2022-11-06 04:20:11.000000 pyanalyze-0.8.0/pyanalyze/checker.py
--rw-r--r--   0 runner    (1001) docker     (121)     9318 2022-11-06 04:20:11.000000 pyanalyze-0.8.0/pyanalyze/error_code.py
--rw-r--r--   0 runner    (1001) docker     (121)    17258 2022-11-06 04:20:11.000000 pyanalyze-0.8.0/pyanalyze/extensions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7792 2022-11-06 04:20:11.000000 pyanalyze-0.8.0/pyanalyze/find_unused.py
--rw-r--r--   0 runner    (1001) docker     (121)    25440 2022-11-06 04:20:11.000000 pyanalyze-0.8.0/pyanalyze/format_strings.py
--rw-r--r--   0 runner    (1001) docker     (121)    17204 2022-11-06 04:20:11.000000 pyanalyze-0.8.0/pyanalyze/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    67985 2022-11-06 04:20:11.000000 pyanalyze-0.8.0/pyanalyze/implementation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-11-06 04:20:11.000000 pyanalyze-0.8.0/pyanalyze/importer.py
--rw-r--r--   0 runner    (1001) docker     (121)   207303 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/name_check_visitor.py
--rw-r--r--   0 runner    (1001) docker     (121)    41313 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/node_visitor.py
--rw-r--r--   0 runner    (1001) docker     (121)    14305 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/options.py
--rw-r--r--   0 runner    (1001) docker     (121)    17781 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/patma.py
--rw-r--r--   0 runner    (1001) docker     (121)     3888 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/predicates.py
--rw-r--r--   0 runner    (1001) docker     (121)     2325 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/reexport.py
--rw-r--r--   0 runner    (1001) docker     (121)     5124 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/safe.py
--rw-r--r--   0 runner    (1001) docker     (121)     1784 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/shared_options.py
--rw-r--r--   0 runner    (1001) docker     (121)   102490 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/signature.py
--rw-r--r--   0 runner    (1001) docker     (121)    60664 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/stacked_scopes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 04:20:21.955748 pyanalyze-0.8.0/pyanalyze/stubs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 04:20:21.967749 pyanalyze-0.8.0/pyanalyze/stubs/_pyanalyze_tests-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/stubs/_pyanalyze_tests-stubs/aliases.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/stubs/_pyanalyze_tests-stubs/args.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/stubs/_pyanalyze_tests-stubs/contextmanager.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/stubs/_pyanalyze_tests-stubs/evaluated.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      725 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/stubs/_pyanalyze_tests-stubs/initnew.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/stubs/_pyanalyze_tests-stubs/overloaded.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/stubs/_pyanalyze_tests-stubs/recursion.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/stubs/_pyanalyze_tests-stubs/self.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/stubs/_pyanalyze_tests-stubs/typeddict.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 04:20:21.967749 pyanalyze-0.8.0/pyanalyze/stubs/pyanalyze-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)      850 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/stubs/pyanalyze-stubs/extensions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8717 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/suggested_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_analysis_lib.py
--rw-r--r--   0 runner    (1001) docker     (121)    55524 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_annotations.py
--rw-r--r--   0 runner    (1001) docker     (121)    11903 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_arg_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     2305 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_ast_annotator.py
--rw-r--r--   0 runner    (1001) docker     (121)     7937 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_async_await.py
--rw-r--r--   0 runner    (1001) docker     (121)     6824 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_asynq.py
--rw-r--r--   0 runner    (1001) docker     (121)    13392 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_asynq_checker.py
--rw-r--r--   0 runner    (1001) docker     (121)    10398 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)     6720 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_boolability.py
--rw-r--r--   0 runner    (1001) docker     (121)     3570 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2617 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_error_code.py
--rw-r--r--   0 runner    (1001) docker     (121)     2332 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (121)    15859 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_format_strings.py
--rw-r--r--   0 runner    (1001) docker     (121)     6467 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (121)    44124 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_implementation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2121 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_inference_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_literal_string.py
--rw-r--r--   0 runner    (1001) docker     (121)    67077 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_name_check_visitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_never.py
--rw-r--r--   0 runner    (1001) docker     (121)    13520 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_node_visitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     8346 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (121)     7217 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_patma.py
--rw-r--r--   0 runner    (1001) docker     (121)     4517 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_pep673.py
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_self.py
--rw-r--r--   0 runner    (1001) docker     (121)    40499 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_signature.py
--rw-r--r--   0 runner    (1001) docker     (121)    56685 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_stacked_scopes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1927 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_suggested_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     2367 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_thrift_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)    19019 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_type_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (121)    10201 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_type_object.py
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_typeddict.py
--rw-r--r--   0 runner    (1001) docker     (121)    24683 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_typeshed.py
--rw-r--r--   0 runner    (1001) docker     (121)     9877 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_typevar.py
--rw-r--r--   0 runner    (1001) docker     (121)    21394 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_value.py
--rw-r--r--   0 runner    (1001) docker     (121)    23799 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/test_yield_checker.py
--rw-r--r--   0 runner    (1001) docker     (121)     4552 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)    29430 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/type_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (121)     8166 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/type_object.py
--rw-r--r--   0 runner    (1001) docker     (121)    42506 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/typeshed.py
--rw-r--r--   0 runner    (1001) docker     (121)     4714 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/typevar.py
--rw-r--r--   0 runner    (1001) docker     (121)    95319 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/value.py
--rw-r--r--   0 runner    (1001) docker     (121)    25490 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyanalyze/yield_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 04:20:21.963749 pyanalyze-0.8.0/pyanalyze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8081 2022-11-06 04:20:21.000000 pyanalyze-0.8.0/pyanalyze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2704 2022-11-06 04:20:21.000000 pyanalyze-0.8.0/pyanalyze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-06 04:20:21.000000 pyanalyze-0.8.0/pyanalyze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-06 04:20:21.000000 pyanalyze-0.8.0/pyanalyze.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-11-06 04:20:21.000000 pyanalyze-0.8.0/pyanalyze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-06 04:20:21.000000 pyanalyze-0.8.0/pyanalyze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-06 04:20:21.967749 pyanalyze-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1608 2022-11-06 04:20:12.000000 pyanalyze-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 21:55:00.000862 pyanalyze-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-01-16 21:55:00.000862 pyanalyze-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 21:54:59.996862 pyanalyze-0.9.0/pyanalyze/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/analysis_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49907 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34784 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/arg_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/ast_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/asynq_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19964 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/boolability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16160 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/find_unused.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25440 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/format_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17035 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69009 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   219445 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/name_check_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41319 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/node_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14305 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17929 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/patma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/reexport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/shared_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107402 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60664 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/stacked_scopes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 21:54:59.972862 pyanalyze-0.9.0/pyanalyze/stubs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 21:55:00.000862 pyanalyze-0.9.0/pyanalyze/stubs/_pyanalyze_tests-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/stubs/_pyanalyze_tests-stubs/aliases.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/stubs/_pyanalyze_tests-stubs/args.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/stubs/_pyanalyze_tests-stubs/contextmanager.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/stubs/_pyanalyze_tests-stubs/deprecated.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/stubs/_pyanalyze_tests-stubs/evaluated.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/stubs/_pyanalyze_tests-stubs/initnew.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/stubs/_pyanalyze_tests-stubs/overloaded.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/stubs/_pyanalyze_tests-stubs/recursion.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/stubs/_pyanalyze_tests-stubs/self.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/stubs/_pyanalyze_tests-stubs/typeddict.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 21:55:00.000862 pyanalyze-0.9.0/pyanalyze/stubs/pyanalyze-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/stubs/pyanalyze-stubs/extensions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/suggested_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_analysis_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57669 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_arg_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_ast_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_async_await.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_asynq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_asynq_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_boolability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_format_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44124 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_inference_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_literal_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65109 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_name_check_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_never.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_node_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_patma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_pep673.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_recursion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_self.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42456 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56676 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_stacked_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_suggested_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_thrift_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_try.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19019 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_type_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_type_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_typeddict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24690 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_typeshed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_typevar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21394 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23799 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/test_yield_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29490 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/type_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8166 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/type_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43867 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/typeshed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/typevar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97428 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25490 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyanalyze/yield_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 21:54:59.996862 pyanalyze-0.9.0/pyanalyze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-01-16 21:54:59.000000 pyanalyze-0.9.0/pyanalyze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-01-16 21:54:59.000000 pyanalyze-0.9.0/pyanalyze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 21:54:59.000000 pyanalyze-0.9.0/pyanalyze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-16 21:54:59.000000 pyanalyze-0.9.0/pyanalyze.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-16 21:54:59.000000 pyanalyze-0.9.0/pyanalyze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-16 21:54:59.000000 pyanalyze-0.9.0/pyanalyze.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-16 21:55:00.000862 pyanalyze-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-01-16 21:54:45.000000 pyanalyze-0.9.0/setup.py
```

### Comparing `pyanalyze-0.8.0/LICENSE` & `pyanalyze-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/PKG-INFO` & `pyanalyze-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyanalyze
-Version: 0.8.0
+Version: 0.9.0
 Summary: A static analyzer for Python
 Home-page: https://github.com/quora/pyanalyze
 Author: Quora, Inc.
 Author-email: jelle@quora.com
 License: Apache Software License
 Keywords: quora static analysis
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyanalyze-0.8.0/README.md` & `pyanalyze-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/__init__.py` & `pyanalyze-0.9.0/pyanalyze/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 used(extensions.overload)
 used(extensions.evaluated)
 used(extensions.is_provided)
 used(extensions.is_keyword)
 used(extensions.is_positional)
 used(extensions.is_of_type)
 used(extensions.show_error)
+used(extensions.has_extra_keys)
 used(value.UNRESOLVED_VALUE)  # keeping it around for now just in case
 used(reexport)
 used(patma)
 used(checker)
 used(suggested_type)
 used(options)
 used(shared_options)
```

### Comparing `pyanalyze-0.8.0/pyanalyze/analysis_lib.py` & `pyanalyze-0.9.0/pyanalyze/analysis_lib.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/annotations.py` & `pyanalyze-0.9.0/pyanalyze/annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,21 @@
 from collections.abc import Callable, Hashable, Iterable
 from dataclasses import dataclass, field, InitVar
 from typing import (
     Any,
     cast,
     Container,
     ContextManager,
+    Generator,
     Mapping,
     NamedTuple,
     NewType,
     Optional,
     Sequence,
+    Set,
     Tuple,
     TYPE_CHECKING,
     TypeVar,
     Union,
 )
 
 import qcore
@@ -57,14 +59,15 @@
     AsynqCallable,
     CustomCheck,
     ExternalType,
     HasAttrGuard,
     NoReturnGuard,
     ParameterTypeGuard,
     TypeGuard,
+    deprecated,
 )
 from .find_unused import used
 from .functions import FunctionDefNode
 from .node_visitor import ErrorContext
 from .safe import is_instance_of_typing_name, is_typing_name
 from .signature import (
     ELLIPSIS_PARAM,
@@ -134,19 +137,37 @@
 
     The base implementation does very little. Subclass this to do something more useful.
 
     """
 
     should_suppress_undefined_names: bool = field(default=False, init=False)
     """While this is True, no errors are shown for undefined names."""
+    _being_evaluated: Set[int] = field(default_factory=set, init=False)
 
     def suppress_undefined_names(self) -> ContextManager[None]:
         """Temporarily suppress errors about undefined names."""
         return qcore.override(self, "should_suppress_undefined_names", True)
 
+    def is_being_evaluted(self, obj: object) -> bool:
+        return id(obj) in self._being_evaluated
+
+    @contextlib.contextmanager
+    def add_evaluation(self, obj: object) -> Generator[None, None, None]:
+        """Temporarily add an object to the set of objects being evaluated.
+
+        This is used to prevent infinite recursion when evaluating forward references.
+
+        """
+        obj_id = id(obj)
+        self._being_evaluated.add(obj_id)
+        try:
+            yield
+        finally:
+            self._being_evaluated.remove(obj_id)
+
     def show_error(
         self,
         message: str,
         error_code: ErrorCode = ErrorCode.invalid_annotation,
         node: Optional[ast.AST] = None,
     ) -> None:
         """Show an error found while evaluating an annotation."""
@@ -425,19 +446,24 @@
             )
     elif is_instance_of_typing_name(val, "_TypedDictMeta"):
         required_keys = getattr(val, "__required_keys__", None)
         # 3.8's typing.TypedDict doesn't have __required_keys__. With
         # inheritance, this makes it apparently impossible to figure out which
         # keys are required at runtime.
         total = getattr(val, "__total__", True)
+        if hasattr(val, "__extra_keys__"):
+            extra_keys = _type_from_runtime(val.__extra_keys__, ctx)
+        else:
+            extra_keys = None
         return TypedDictValue(
             {
                 key: _get_typeddict_value(value, ctx, key, required_keys, total)
                 for key, value in val.__annotations__.items()
-            }
+            },
+            extra_keys=extra_keys,
         )
     elif val is InitVar:
         # On 3.6 and 3.7, InitVar[T] just returns InitVar at runtime, so we can't
         # get the actual type out.
         return AnyValue(AnySource.inference)
     elif isinstance(val, InitVar):
         # val.type exists only on 3.8+, but on earlier versions
@@ -504,25 +530,23 @@
         return AnyValue(AnySource.incomplete_annotation)
     elif typing_inspect.is_classvar(val) or typing_inspect.is_final_type(val):
         typ = val.__args__[0]
         return _type_from_runtime(typ, ctx)
     elif is_instance_of_typing_name(val, "_ForwardRef") or is_instance_of_typing_name(
         val, "ForwardRef"
     ):
-        # This has issues because the forward ref may be defined in a different file, in
-        # which case we don't know which names are valid in it.
-        with ctx.suppress_undefined_names():
-            try:
-                code = ast.parse(val.__forward_arg__)
-            except SyntaxError:
-                ctx.show_error(
-                    f"Syntax error in forward reference: {val.__forward_arg__}"
+        if ctx.is_being_evaluted(val):
+            return AnyValue(AnySource.inference)
+        with ctx.add_evaluation(val):
+            # This is necessary because the forward ref may be defined in a different file, in
+            # which case we don't know which names are valid in it.
+            with ctx.suppress_undefined_names():
+                return _eval_forward_ref(
+                    val.__forward_arg__, ctx, is_typeddict=is_typeddict
                 )
-                return AnyValue(AnySource.error)
-            return _type_from_ast(code.body[0], ctx, is_typeddict=is_typeddict)
     elif val is Ellipsis:
         # valid in Callable[..., ]
         return AnyValue(AnySource.explicit)
     elif is_instance_of_typing_name(val, "_TypeAlias"):
         # typing.Pattern and Match, which are not normal generic types for some reason
         return GenericValue(val.impl_type, [_type_from_runtime(val.type_var, ctx)])
     elif isinstance(val, TypeGuard):
@@ -922,14 +946,20 @@
 
 @dataclass
 class Pep655Value(Value):
     required: bool
     value: Value
 
 
+@dataclass
+class DecoratorValue(Value):
+    decorator: object
+    args: Tuple[Value, ...]
+
+
 class _Visitor(ast.NodeVisitor):
     def __init__(self, ctx: Context) -> None:
         self.ctx = ctx
 
     def generic_visit(self, node: ast.AST) -> None:
         raise NotImplementedError(f"no visitor implemented for {node!r}")
 
@@ -1073,14 +1103,22 @@
                 )
                 return None
             for name, _ in kwarg_values:
                 self.ctx.show_error(f"Unrecognized ParamSpec kwarg {name}", node=node)
                 return None
             tv = ParamSpec(name_val.val)
             return TypeVarValue(tv, is_paramspec=True)
+        elif is_typing_name(func.val, "deprecated") or func.val is deprecated:
+            if node.keywords:
+                self.ctx.show_error(
+                    "deprecated() does not accept keyword arguments", node=node
+                )
+                return None
+            arg_values = tuple(self.visit(arg) for arg in node.args)
+            return DecoratorValue(deprecated, arg_values)
         elif isinstance(func.val, type):
             if func.val is object:
                 return AnyValue(AnySource.inference)
             return TypedValue(func.val)
         else:
             return None
```

### Comparing `pyanalyze-0.8.0/pyanalyze/arg_spec.py` & `pyanalyze-0.9.0/pyanalyze/arg_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import contextlib
 import enum
 import inspect
 import sys
 import textwrap
 from dataclasses import dataclass, replace
 from types import FunctionType, MethodType, ModuleType
+import typing
 from typing import (
     Any,
     Callable,
     Generic,
     Iterator,
     List,
     Mapping,
@@ -32,25 +33,32 @@
 import typing_inspect
 from typing_extensions import is_typeddict
 
 import pyanalyze
 from . import implementation
 from .analysis_lib import is_positional_only_arg_name
 from .annotations import Context, RuntimeEvaluator, type_from_runtime
-from .extensions import CustomCheck, get_overloads, get_type_evaluations, TypeGuard
+from .extensions import (
+    CustomCheck,
+    get_overloads as pyanalyze_get_overloads,
+    get_type_evaluations,
+    TypeGuard,
+)
 from .find_unused import used
 from .functions import translate_vararg_type
 from .options import Options, PyObjectSequenceOption
 from .safe import (
     all_of_type,
     get_fully_qualified_name,
     hasattr_static,
     is_newtype,
     is_typing_name,
     safe_equals,
+    safe_getattr,
+    safe_hasattr,
     safe_isinstance,
     safe_issubclass,
 )
 from .signature import (
     ANY_SIGNATURE,
     ConcreteSignature,
     ELLIPSIS_PARAM,
@@ -79,14 +87,27 @@
     SubclassValue,
     TypedDictValue,
     TypedValue,
     TypeVarValue,
     Value,
 )
 
+_GET_OVERLOADS = []
+
+try:
+    from typing_extensions import get_overloads
+except ImportError:
+    pass
+else:
+    _GET_OVERLOADS.append(get_overloads)
+if sys.version_info >= (3, 11):
+    # TODO: support version checks
+    # static analysis: ignore[undefined_attribute]
+    _GET_OVERLOADS.append(typing.get_overloads)
+
 # types.MethodWrapperType in 3.7+
 MethodWrapperType = type(object().__str__)
 
 _ENUM_CALL = enum.Enum.__call__.__func__
 
 
 @used  # exposed as an API
@@ -574,26 +595,31 @@
                 obj.__func__, impl, is_asynq, in_overload_resolution
             )
             return make_bound_method(argspec, Composite(KnownValue(obj.__self__)))
 
         # Must be after the check for bound methods, because otherwise we
         # won't bind self correctly.
         if not in_overload_resolution:
+            for get_overloads_func in _GET_OVERLOADS:
+                inner_obj = safe_getattr(obj, "__func__", obj)
+                if safe_hasattr(inner_obj, "__module__") and safe_hasattr(
+                    inner_obj, "__qualname__"
+                ):
+                    sig = self._maybe_make_overloaded_signature(
+                        get_overloads_func(inner_obj), impl, is_asynq
+                    )
+                    if sig is not None:
+                        return sig
             fq_name = get_fully_qualified_name(obj)
             if fq_name is not None:
-                overloads = get_overloads(fq_name)
-                if overloads:
-                    sigs = [
-                        self._cached_get_argspec(
-                            overload, impl, is_asynq, in_overload_resolution=True
-                        )
-                        for overload in overloads
-                    ]
-                    if all_of_type(sigs, Signature):
-                        return OverloadedSignature(sigs)
+                sig = self._maybe_make_overloaded_signature(
+                    pyanalyze_get_overloads(fq_name), impl, is_asynq
+                )
+                if sig is not None:
+                    return sig
                 evaluator_sig = self._maybe_make_evaluator_sig(obj, impl, is_asynq)
                 if evaluator_sig is not None:
                     return evaluator_sig
 
         if hasattr_static(obj, "fn") or hasattr_static(obj, "original_fn"):
             is_asynq = is_asynq or hasattr_static(obj, "asynq")
             # many decorators put the original function in the .fn attribute
@@ -649,15 +675,24 @@
                         key,
                         ParameterKind.KEYWORD_ONLY,
                         default=None if required else KnownValue(...),
                         annotation=value,
                     )
                     for key, (required, value) in td_type.items.items()
                 ]
-                return Signature.make(params, td_type)
+                if td_type.extra_keys is not None:
+                    annotation = GenericValue(
+                        dict, [TypedValue(str), td_type.extra_keys]
+                    )
+                    params.append(
+                        SigParameter(
+                            "%kwargs", ParameterKind.VAR_KEYWORD, annotation=annotation
+                        )
+                    )
+                return Signature.make(params, td_type, callable=obj)
 
         if is_newtype(obj):
             assert hasattr(obj, "__supertype__")
             return Signature.make(
                 [
                     SigParameter(
                         "x",
@@ -777,14 +812,32 @@
             # we could get an argspec here in some cases, but it's impossible to figure out
             # the argspec for some builtin methods (e.g., dict.__init__), and no way to detect
             # these with inspect, so just give up.
             return self._make_any_sig(obj)
 
         return None
 
+    def _maybe_make_overloaded_signature(
+        self,
+        overloads: Sequence[Callable[..., Any]],
+        impl: Optional[Impl],
+        is_asynq: bool,
+    ) -> Optional[OverloadedSignature]:
+        if not overloads:
+            return None
+        sigs = [
+            self._cached_get_argspec(
+                overload, impl, is_asynq, in_overload_resolution=True
+            )
+            for overload in overloads
+        ]
+        if not all_of_type(sigs, Signature):
+            return None
+        return OverloadedSignature(sigs)
+
     def _make_any_sig(self, obj: object) -> Signature:
         if FunctionsSafeToCall.contains(obj, self.options):
             return Signature.make(
                 [ELLIPSIS_PARAM],
                 AnyValue(AnySource.inference),
                 is_asynq=True,
                 allow_call=True,
```

### Comparing `pyanalyze-0.8.0/pyanalyze/ast_annotator.py` & `pyanalyze-0.9.0/pyanalyze/ast_annotator.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/asynq_checker.py` & `pyanalyze-0.9.0/pyanalyze/asynq_checker.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/attributes.py` & `pyanalyze-0.9.0/pyanalyze/attributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -187,14 +187,44 @@
 
     @classmethod
     def should_treat_as_any(cls, val: object, options: Options) -> bool:
         option_value = options.get_value_for(cls)
         return any(func(val) for func in option_value)
 
 
+_CAT = Callable[[object], Optional[Tuple[Value, Value]]]
+
+
+class ClassAttributeTransformer(PyObjectSequenceOption[_CAT]):
+    """Transform certain class attributes.
+
+    Instances of this option are callables that take an object found among
+    a class's attributes and return either None (if the value should not
+    be transformed) or a pair of a get and set type. To disallow setting
+    the value, return :data:`pyanalyze.value.NO_RETURN_VALUE`.
+
+    If multiple transformers match an object, the first one is used.
+
+    TODO: The set type is currently ignored.
+
+    """
+
+    default_value: Sequence[_CAT] = []
+    name = "class_attribute_transformers"
+
+    @classmethod
+    def transform_attribute(cls, val: object, options: Options) -> Optional[Value]:
+        option_value = options.get_value_for(cls)
+        for transformer in option_value:
+            result = transformer(val)
+            if result is not None:
+                return result[0]
+        return None
+
+
 def _unwrap_value_from_subclass(result: Value, ctx: AttrContext) -> Value:
     if not isinstance(result, KnownValue) or ctx.skip_unwrap:
         return result
     cls_val = result.val
     if (
         qcore.inspection.is_classmethod(cls_val)
         or inspect.ismethod(cls_val)
@@ -211,14 +241,19 @@
         # static or class method
         return KnownValue(cls_val)
     elif _static_hasattr(cls_val, "__get__"):
         return AnyValue(AnySource.inference)  # can't figure out what this will return
     elif TreatClassAttributeAsAny.should_treat_as_any(cls_val, ctx.options):
         return AnyValue(AnySource.error)
     else:
+        transformed = ClassAttributeTransformer.transform_attribute(
+            cls_val, ctx.options
+        )
+        if transformed is not None:
+            return transformed
         return KnownValue(cls_val)
 
 
 def _get_attribute_from_synthetic_type(
     fq_name: str, generic_args: Sequence[Value], ctx: AttrContext
 ) -> Value:
     # First check values that are special in Python
@@ -324,14 +359,19 @@
         typeshed_type = ctx.get_attribute_from_typeshed(typ, on_class=False)
         if typeshed_type is not UNINITIALIZED_VALUE:
             return typeshed_type
         return AnyValue(AnySource.inference)
     elif TreatClassAttributeAsAny.should_treat_as_any(cls_val, ctx.options):
         return AnyValue(AnySource.error)
     else:
+        transformed = ClassAttributeTransformer.transform_attribute(
+            cls_val, ctx.options
+        )
+        if transformed is not None:
+            return transformed
         return result
 
 
 def _get_attribute_from_known(obj: object, ctx: AttrContext) -> Value:
     ctx.record_attr_read(type(obj))
 
     if (obj is None or obj is NoneType) and ctx.should_ignore_none_attributes():
@@ -427,69 +467,70 @@
         else:
             attr_type = type_from_annotations(
                 annotations, ctx.attr, ctx=AnnotationsContext(ctx, typ)
             )
             if attr_type is not None:
                 return (attr_type, typ, False)
 
-    try:
-        mro = list(typ.mro())
-    except Exception:
-        # broken mro method
-        pass
-    else:
-        for base_cls in mro:
-            if ctx.skip_mro and base_cls is not typ:
-                continue
-
-            typeshed_type = ctx.get_attribute_from_typeshed(
-                base_cls, on_class=on_class or ctx.skip_unwrap
-            )
-            if typeshed_type is not UNINITIALIZED_VALUE:
-                if ctx.prefer_typeshed:
-                    return typeshed_type, base_cls, False
-                # If it's a callable, we'll probably do better
-                # getting the attribute from the type ourselves,
-                # because we may have our own implementation.
-                if not isinstance(typeshed_type, CallableValue):
-                    return typeshed_type, base_cls, False
+    if safe_isinstance(typ, type):
+        try:
+            mro = list(type.mro(typ))
+        except Exception:
+            # broken mro method
+            pass
+        else:
+            for base_cls in mro:
+                if ctx.skip_mro and base_cls is not typ:
+                    continue
 
-            try:
-                base_dict = base_cls.__dict__
-            except Exception:
-                continue
-
-            try:
-                # Make sure to use only __annotations__ that are actually on this
-                # class, not ones inherited from a base class.
-                annotations = base_dict["__annotations__"]
-            except Exception:
-                pass
-            else:
-                attr_type = type_from_annotations(
-                    annotations, ctx.attr, ctx=AnnotationsContext(ctx, base_cls)
+                typeshed_type = ctx.get_attribute_from_typeshed(
+                    base_cls, on_class=on_class or ctx.skip_unwrap
                 )
-                if attr_type is not None:
-                    return (attr_type, base_cls, False)
+                if typeshed_type is not UNINITIALIZED_VALUE:
+                    if ctx.prefer_typeshed:
+                        return typeshed_type, base_cls, False
+                    # If it's a callable, we'll probably do better
+                    # getting the attribute from the type ourselves,
+                    # because we may have our own implementation.
+                    if not isinstance(typeshed_type, CallableValue):
+                        return typeshed_type, base_cls, False
+
+                try:
+                    base_dict = base_cls.__dict__
+                except Exception:
+                    continue
 
-            try:
-                # Make sure we use only the object from this class, but do invoke
-                # the descriptor protocol with getattr.
-                base_dict[ctx.attr]
-            except Exception:
-                pass
-            else:
                 try:
-                    val = KnownValue(getattr(typ, ctx.attr))
+                    # Make sure to use only __annotations__ that are actually on this
+                    # class, not ones inherited from a base class.
+                    annotations = base_dict["__annotations__"]
                 except Exception:
-                    val = AnyValue(AnySource.inference)
-                return val, base_cls, True
+                    pass
+                else:
+                    attr_type = type_from_annotations(
+                        annotations, ctx.attr, ctx=AnnotationsContext(ctx, base_cls)
+                    )
+                    if attr_type is not None:
+                        return (attr_type, base_cls, False)
 
-            if typeshed_type is not UNINITIALIZED_VALUE:
-                return typeshed_type, base_cls, False
+                try:
+                    # Make sure we use only the object from this class, but do invoke
+                    # the descriptor protocol with getattr.
+                    base_dict[ctx.attr]
+                except Exception:
+                    pass
+                else:
+                    try:
+                        val = KnownValue(getattr(typ, ctx.attr))
+                    except Exception:
+                        val = AnyValue(AnySource.inference)
+                    return val, base_cls, True
+
+                if typeshed_type is not UNINITIALIZED_VALUE:
+                    return typeshed_type, base_cls, False
 
     attrs_type = get_attrs_attribute(typ, ctx)
     if attrs_type is not None:
         return attrs_type, typ, False
 
     if not ctx.skip_mro:
         # Even if we didn't find it any __dict__, maybe getattr() finds it directly.
```

### Comparing `pyanalyze-0.8.0/pyanalyze/boolability.py` & `pyanalyze-0.9.0/pyanalyze/boolability.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/checker.py` & `pyanalyze-0.9.0/pyanalyze/checker.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/error_code.py` & `pyanalyze-0.9.0/pyanalyze/error_code.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,14 +95,17 @@
     bad_match = 75
     bad_evaluator = 76
     implicit_any = 77
     already_declared = 78
     invalid_annotated_assignment = 79
     unused_assignment = 80
     incompatible_yield = 81
+    invalid_import = 82
+    too_many_positional_args = 83
+    deprecated = 84
 
 
 # Allow testing unannotated functions without too much fuss
 DISABLED_IN_TESTS = {
     ErrorCode.missing_return_annotation,
     ErrorCode.missing_parameter_annotation,
     ErrorCode.suggested_return_type,
@@ -115,14 +118,15 @@
     *DISABLED_IN_TESTS,
     ErrorCode.method_first_arg,
     ErrorCode.value_always_true,
     ErrorCode.use_fstrings,
     ErrorCode.unused_ignore,
     ErrorCode.missing_f,
     ErrorCode.bare_ignore,
+    ErrorCode.too_many_positional_args,
     # TODO: turn this on
     ErrorCode.implicit_reexport,
     ErrorCode.incompatible_override,
 }
 
 ERROR_DESCRIPTION = {
     ErrorCode.bad_star_import: '"from ... import *" within a function.',
@@ -215,14 +219,19 @@
     ErrorCode.bad_match: "Invalid type in match statement",
     ErrorCode.bad_evaluator: "Invalid code in type evaluator",
     ErrorCode.implicit_any: "Value is inferred as Any",
     ErrorCode.already_declared: "Name is already declared",
     ErrorCode.invalid_annotated_assignment: "Invalid annotated assignment",
     ErrorCode.unused_assignment: "Assigned value is never used",
     ErrorCode.incompatible_yield: "Incompatible yield type",
+    ErrorCode.deprecated: "Use of deprecated feature",
+    ErrorCode.invalid_import: "Invalid import",
+    ErrorCode.too_many_positional_args: (
+        "Call with many positional arguments should use keyword arguments"
+    ),
 }
 
 
 @used  # exposed as an API
 def register_error_code(name: str, description: str) -> ErrorCode:
     """Register an additional error code. For use in extensions."""
     value = max(member.value for member in ErrorCode) + 1
```

### Comparing `pyanalyze-0.8.0/pyanalyze/extensions.py` & `pyanalyze-0.9.0/pyanalyze/extensions.py`

 * *Files 3% similar despite different names*

```diff
@@ -379,15 +379,15 @@
     """Inspect the inferred type of an expression.
 
     Calling this function will make pyanalyze print out the argument's
     inferred value in a human-readable format. At runtime it does nothing.
 
     This is automatically exposed as a global during type checking, so in
     code that is not run at import, `reveal_type()` can be used without
-    being impoorted.
+    being imported.
 
     Example::
 
         def f(x: int) -> None:
             reveal_type(x)  # Revealed type is "int"
 
     At runtime this returns the argument unchanged.
@@ -442,14 +442,48 @@
         with assert_error():  # error: no error found in this block
             1 + 1
 
     """
     yield
 
 
+def deprecated(__msg: str) -> typing.Callable[[_T], _T]:
+    """Indicate that a class, function or overload is deprecated.
+
+    Usage::
+
+        @deprecated("Use B instead")
+        class A:
+            pass
+        @deprecated("Use g instead")
+        def f():
+            pass
+        @deprecated("int support is deprecated")
+        @overload
+        def g(x: int) -> int: ...
+        @overload
+        def g(x: str) -> int: ...
+
+    When this decorator is applied to an object, the type checker
+    will generate a diagnostic on usage of the deprecated object.
+
+    No runtime warning is issued. The decorator sets the ``__deprecated__``
+    attribute on the decorated object to the deprecation message
+    passed to the decorator.
+
+    See PEP 702 for details.
+    """
+
+    def decorator(__arg: _T) -> _T:
+        __arg.__deprecated__ = __msg
+        return __arg
+
+    return decorator
+
+
 _overloads: Dict[str, List[Callable[..., Any]]] = defaultdict(list)
 _type_evaluations: Dict[str, List[Callable[..., Any]]] = defaultdict(list)
 
 
 def get_overloads(fully_qualified_name: str) -> List[Callable[..., Any]]:
     """Return all defined runtime overloads for this fully qualified name."""
     return _overloads[fully_qualified_name]
@@ -465,15 +499,15 @@
 
 else:
 
     def overload(func: Callable[..., Any]) -> Callable[..., Any]:
         """A version of `typing.overload` that is inspectable at runtime.
 
         If this decorator is used for a function `some_module.some_function`, calling
-        :func:`pyanalyze.extensiions.get_overloads("some_module.some_function")` will
+        :func:`pyanalyze.extensions.get_overloads("some_module.some_function")` will
         return all the runtime overloads.
 
         """
         key = get_fully_qualified_name(func)
         if key is not None:
             _overloads[key].append(func)
         return real_overload(func)
@@ -547,7 +581,32 @@
 
     May not be called at runtime.
 
     """
     raise NotImplementedError(
         "show_error() may only be called in type evaluation functions"
     )
+
+
+def has_extra_keys(value_type: object = Any) -> Callable[[_T], _T]:
+    """Decorator for ``TypedDict`` types, indicating that the dict
+    has additional keys of the given type.
+
+    This is an experimental feature.
+
+    Example usage::
+
+        @has_extra_keys(str)
+        class TD(TypedDict):
+            a: int
+
+        def f(x: TD) -> None:
+            assert_type(x["a"], int)
+            assert_type(x["arbitrary_key"], str)
+
+    """
+
+    def decorator(cls: _T) -> _T:
+        cls.__extra_keys__ = value_type
+        return cls
+
+    return decorator
```

### Comparing `pyanalyze-0.8.0/pyanalyze/find_unused.py` & `pyanalyze-0.9.0/pyanalyze/find_unused.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/format_strings.py` & `pyanalyze-0.9.0/pyanalyze/format_strings.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/functions.py` & `pyanalyze-0.9.0/pyanalyze/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 
 from .error_code import ErrorCode
 from .extensions import evaluated, overload, real_overload
 from .node_visitor import ErrorContext
 from .options import Options, PyObjectSequenceOption
 from .signature import ParameterKind, Signature, SigParameter
 from .stacked_scopes import Composite
-from .typevar import resolve_bounds_map
 from .value import (
     AnySource,
     AnyValue,
     CallableValue,
     CanAssignContext,
     CanAssignError,
     GenericValue,
     get_tv_map,
     KnownValue,
+    is_iterable,
     make_coro_type,
     SubclassValue,
     TypedValue,
     TypeVarValue,
     unite_values,
     UnpackedValue,
     Value,
@@ -45,15 +45,14 @@
 FunctionDefNode = Union[ast.FunctionDef, ast.AsyncFunctionDef]
 FunctionNode = Union[FunctionDefNode, ast.Lambda]
 IMPLICIT_CLASSMETHODS = ("__init_subclass__", "__new__")
 
 YieldT = TypeVar("YieldT")
 SendT = TypeVar("SendT")
 ReturnT = TypeVar("ReturnT")
-IterableValue = GenericValue(collections.abc.Iterable, [TypeVarValue(YieldT)])
 GeneratorValue = GenericValue(
     collections.abc.Generator,
     [TypeVarValue(YieldT), TypeVarValue(SendT), TypeVarValue(ReturnT)],
 )
 
 
 class AsyncFunctionKind(enum.Enum):
@@ -89,43 +88,42 @@
     params: Sequence[ParamInfo]
     return_annotation: Optional[Value]
     potential_function: Optional[object]
 
     def get_generator_yield_type(self, ctx: CanAssignContext) -> Value:
         if self.return_annotation is None:
             return AnyValue(AnySource.unannotated)
-        can_assign = IterableValue.can_assign(self.return_annotation, ctx)
-        if isinstance(can_assign, CanAssignError):
+        iterable_val = is_iterable(self.return_annotation, ctx)
+        if isinstance(iterable_val, CanAssignError):
             return AnyValue(AnySource.error)
-        tv_map, _ = resolve_bounds_map(can_assign, ctx)
-        return tv_map.get(YieldT, AnyValue(AnySource.generic_argument))
+        return iterable_val
 
     def get_generator_send_type(self, ctx: CanAssignContext) -> Value:
         if self.return_annotation is None:
             return AnyValue(AnySource.unannotated)
         tv_map = get_tv_map(GeneratorValue, self.return_annotation, ctx)
         if not isinstance(tv_map, CanAssignError):
             return tv_map.get(SendT, AnyValue(AnySource.generic_argument))
         # If the return annotation is a non-Generator Iterable, assume the send
         # type is None.
-        can_assign = IterableValue.can_assign(self.return_annotation, ctx)
-        if isinstance(can_assign, CanAssignError):
+        iterable_val = is_iterable(self.return_annotation, ctx)
+        if isinstance(iterable_val, CanAssignError):
             return AnyValue(AnySource.error)
         return KnownValue(None)
 
     def get_generator_return_type(self, ctx: CanAssignContext) -> Value:
         if self.return_annotation is None:
             return AnyValue(AnySource.unannotated)
         tv_map = get_tv_map(GeneratorValue, self.return_annotation, ctx)
         if not isinstance(tv_map, CanAssignError):
             return tv_map.get(ReturnT, AnyValue(AnySource.generic_argument))
         # If the return annotation is a non-Generator Iterable, assume the return
         # type is None.
-        can_assign = IterableValue.can_assign(self.return_annotation, ctx)
-        if isinstance(can_assign, CanAssignError):
+        iterable_val = is_iterable(self.return_annotation, ctx)
+        if isinstance(iterable_val, CanAssignError):
             return AnyValue(AnySource.error)
         return KnownValue(None)
 
 
 @dataclass
 class FunctionResult:
     """Computed after visiting a function."""
@@ -325,16 +323,18 @@
                 arg.annotation, allow_unpack=kind.allow_unpack()
             )
             if default is not None:
                 tv_map = value.can_assign(default, ctx)
                 if isinstance(tv_map, CanAssignError):
                     ctx.show_error(
                         arg,
-                        f"Default value for argument {arg.arg} incompatible"
-                        f" with declared type {value}",
+                        (
+                            f"Default value for argument {arg.arg} incompatible"
+                            f" with declared type {value}"
+                        ),
                         error_code=ErrorCode.incompatible_default,
                         detail=tv_map.display(),
                     )
         elif is_self:
             assert enclosing_class is not None
             if is_classmethod or getattr(node, "name", None) in IMPLICIT_CLASSMETHODS:
                 value = SubclassValue(enclosing_class)
```

### Comparing `pyanalyze-0.8.0/pyanalyze/implementation.py` & `pyanalyze-0.9.0/pyanalyze/implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -371,15 +371,15 @@
 def _sequence_getitem_impl(ctx: CallContext, typ: type) -> ImplReturn:
     def inner(key: Value) -> Value:
         self_value = replace_known_sequence_value(ctx.vars["self"])
         if not isinstance(self_value, TypedValue):
             return AnyValue(AnySource.error)  # shouldn't happen
         key = replace_known_sequence_value(key)
         if not TypedValue(slice).is_assignable(key, ctx.visitor):
-            key = ctx.visitor._check_dunder_call(
+            key, _ = ctx.visitor._check_dunder_call(
                 ctx.ast_for_arg("obj"), Composite(key), "__index__", [], allow_call=True
             )
 
         if isinstance(key, KnownValue):
             if isinstance(key.val, int):
                 if isinstance(self_value, SequenceValue):
                     members = self_value.get_member_sequence()
@@ -475,30 +475,35 @@
 ) -> None:
     if not isinstance(key, KnownValue) or not isinstance(key.val, str):
         ctx.show_error(
             f"TypedDict key must be a string literal (got {key})",
             ErrorCode.invalid_typeddict_key,
             arg="k",
         )
-    elif key.val not in self_value.items:
-        ctx.show_error(
-            f"Key {key.val!r} does not exist in {self_value}",
-            ErrorCode.invalid_typeddict_key,
-            arg="k",
-        )
-    else:
-        _, expected_type = self_value.items[key.val]
-        tv_map = expected_type.can_assign(value, ctx.visitor)
-        if isinstance(tv_map, CanAssignError):
+        return
+    if key.val not in self_value.items:
+        if self_value.extra_keys is None:
             ctx.show_error(
-                f"Value for key {key.val!r} must be {expected_type}, not {value}",
-                ErrorCode.incompatible_argument,
-                arg="v",
-                detail=str(tv_map),
+                f"Key {key.val!r} does not exist in {self_value}",
+                ErrorCode.invalid_typeddict_key,
+                arg="k",
             )
+            return
+        else:
+            expected_type = self_value.extra_keys
+    else:
+        _, expected_type = self_value.items[key.val]
+    tv_map = expected_type.can_assign(value, ctx.visitor)
+    if isinstance(tv_map, CanAssignError):
+        ctx.show_error(
+            f"Value for key {key.val!r} must be {expected_type}, not {value}",
+            ErrorCode.incompatible_argument,
+            arg="v",
+            detail=str(tv_map),
+        )
 
 
 def _check_dict_key_hashability(key: Value, ctx: CallContext, arg: str) -> bool:
     hashability = check_hashability(key, ctx.visitor)
     if isinstance(hashability, CanAssignError):
         ctx.show_error(
             "Dictionary key is not hashable",
@@ -548,20 +553,29 @@
             elif isinstance(key, KnownValue):
                 try:
                     _, value = self_value.items[key.val]
                     return value
                 # probably KeyError, but catch anything in case it's an
                 # unhashable str subclass or something
                 except Exception:
-                    # No error here; TypedDicts may have additional keys at runtime.
-                    pass
-            # TODO strictly we should throw an error for any non-Literal or unknown key:
-            # https://www.python.org/dev/peps/pep-0589/#supported-and-unsupported-operations
-            # Don't do that yet because it may cause too much disruption.
-            return AnyValue(AnySource.inference)
+                    if self_value.extra_keys is None:
+                        ctx.show_error(
+                            f"Unknown TypedDict key {key}",
+                            ErrorCode.invalid_typeddict_key,
+                            arg="k",
+                        )
+                        return AnyValue(AnySource.error)
+            if self_value.extra_keys is not None:
+                return self_value.extra_keys
+            ctx.show_error(
+                f"TypedDict key must be a literal, not {key}",
+                ErrorCode.invalid_typeddict_key,
+                arg="k",
+            )
+            return AnyValue(AnySource.error)
         elif isinstance(self_value, DictIncompleteValue):
             val = self_value.get_value(key, ctx.visitor)
             if val is UNINITIALIZED_VALUE:
                 # No error here, the key may have been added where we couldn't see it.
                 # TODO try out changing this
                 return AnyValue(AnySource.error)
             return val
@@ -611,25 +625,34 @@
                 return AnyValue(AnySource.error)
             elif isinstance(key, KnownValue):
                 try:
                     required, value = self_value.items[key.val]
                 # probably KeyError, but catch anything in case it's an
                 # unhashable str subclass or something
                 except Exception:
-                    # No error here; TypedDicts may have additional keys at runtime.
-                    pass
+                    if self_value.extra_keys is None:
+                        ctx.show_error(
+                            f"Unknown TypedDict key {key.val!r}",
+                            ErrorCode.invalid_typeddict_key,
+                            arg="k",
+                        )
+                        return AnyValue(AnySource.error)
                 else:
                     if required:
                         return value
                     else:
                         return value | default
-            # TODO strictly we should throw an error for any non-Literal or unknown key:
-            # https://www.python.org/dev/peps/pep-0589/#supported-and-unsupported-operations
-            # Don't do that yet because it may cause too much disruption.
-            return default
+            if self_value.extra_keys is not None:
+                return self_value.extra_keys | default
+            ctx.show_error(
+                f"TypedDict key must be a literal, not {key}",
+                ErrorCode.invalid_typeddict_key,
+                arg="k",
+            )
+            return AnyValue(AnySource.error)
         elif isinstance(self_value, DictIncompleteValue):
             val = self_value.get_value(key, ctx.visitor)
             if val is UNINITIALIZED_VALUE:
                 return default
             return val | default
         elif isinstance(self_value, TypedValue):
             key_type = self_value.get_generic_arg_for_type(dict, ctx.visitor, 0)
@@ -677,14 +700,16 @@
                 if is_required:
                     ctx.show_error(
                         f"Cannot pop required TypedDict key {key}",
                         error_code=ErrorCode.incompatible_argument,
                         arg="key",
                     )
                 return ImplReturn(_maybe_unite(expected_type, default))
+        if self_value.extra_keys is not None:
+            return ImplReturn(_maybe_unite(self_value.extra_keys, default))
         ctx.show_error(
             f"Key {key} does not exist in TypedDict",
             ErrorCode.invalid_typeddict_key,
             arg="key",
         )
         return ImplReturn(default)
     elif isinstance(self_value, DictIncompleteValue):
@@ -757,20 +782,24 @@
             # unhashable str subclass or something
             except Exception:
                 pass
             else:
                 tv_map = expected_type.can_assign(default, ctx.visitor)
                 if isinstance(tv_map, CanAssignError):
                     ctx.show_error(
-                        f"TypedDict key {key.val} expected value of type"
-                        f" {expected_type}, not {default}",
+                        (
+                            f"TypedDict key {key.val} expected value of type"
+                            f" {expected_type}, not {default}"
+                        ),
                         ErrorCode.incompatible_argument,
                         arg="default",
                     )
                 return ImplReturn(expected_type)
+        if self_value.extra_keys is not None:
+            return ImplReturn(self_value.extra_keys | default)
         ctx.show_error(
             f"Key {key} does not exist in TypedDict",
             ErrorCode.invalid_typeddict_key,
             arg="key",
         )
         return ImplReturn(default)
     elif isinstance(self_value, DictIncompleteValue):
@@ -1083,16 +1112,18 @@
 def _assert_is_value_impl(ctx: CallContext) -> Value:
     if not ctx.visitor._is_checking():
         return KnownValue(None)
     obj = ctx.vars["obj"]
     expected_value = ctx.vars["value"]
     if not isinstance(expected_value, KnownValue):
         ctx.show_error(
-            "Value argument to assert_is_value must be a KnownValue (got"
-            f" {expected_value!r}; object is {obj!r})",
+            (
+                "Value argument to assert_is_value must be a KnownValue (got"
+                f" {expected_value!r}; object is {obj!r})"
+            ),
             ErrorCode.inference_failure,
             arg="value",
         )
     else:
         if _remove_annotated(ctx.vars["skip_annotated"]) == KnownValue(True):
             obj = _remove_annotated(obj)
         if obj != expected_value.val:
@@ -1176,16 +1207,18 @@
         ctx.show_error(message, error_code=ErrorCode.incompatible_call)
         return TypedValue(str)
     for field in parsed.iter_replacement_fields():
         # TODO validate conversion specifiers, attributes, etc.
         if field.arg_name is None:
             if current_index >= len(args):
                 ctx.show_error(
-                    "Too few arguments to format string (expected at least"
-                    f" {current_index})",
+                    (
+                        "Too few arguments to format string (expected at least"
+                        f" {current_index})"
+                    ),
                     error_code=ErrorCode.incompatible_call,
                 )
             used_indices.add(current_index)
             current_index += 1
         elif isinstance(field.arg_name, int):
             index = field.arg_name
             if index >= len(args):
```

### Comparing `pyanalyze-0.8.0/pyanalyze/importer.py` & `pyanalyze-0.9.0/pyanalyze/importer.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/name_check_visitor.py` & `pyanalyze-0.9.0/pyanalyze/name_check_visitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,30 +6,25 @@
 type inference. It is the central object that invokes other parts of
 the system.
 
 """
 import abc
 import ast
 import asyncio
-import builtins
 import collections
 import collections.abc
 import contextlib
 import enum
 import itertools
 import logging
 import operator
 import os
 import os.path
 import pickle
-import random
-import re
-import string
 import sys
-import tempfile
 import traceback
 import types
 from argparse import ArgumentParser
 from dataclasses import dataclass
 from itertools import chain
 from pathlib import Path
 from typing import (
@@ -51,15 +46,14 @@
     TypeVar,
     Union,
 )
 
 import asynq
 import qcore
 import typeshed_client
-from ast_decompiler import decompile
 from typing_extensions import Annotated, Protocol
 
 from . import attributes, format_strings, importer, node_visitor, type_evaluation
 from .analysis_lib import get_attribute_path
 from .annotations import (
     is_context_manager_type,
     is_instance_of_typing_name,
@@ -81,15 +75,14 @@
     compute_value_of_function,
     FunctionDefNode,
     FunctionInfo,
     FunctionNode,
     FunctionResult,
     GeneratorValue,
     IMPLICIT_CLASSMETHODS,
-    IterableValue,
     ReturnT,
     SendT,
     YieldT,
 )
 from .options import (
     add_arguments,
     BooleanOption,
@@ -100,15 +93,22 @@
     Options,
     PyObjectSequenceOption,
     StringSequenceOption,
 )
 from .patma import PatmaVisitor
 from .predicates import EqualsPredicate
 from .reexport import ImplicitReexportTracker
-from .safe import is_dataclass_type, is_hashable, safe_getattr, safe_issubclass
+from .safe import (
+    is_dataclass_type,
+    is_hashable,
+    safe_getattr,
+    safe_hasattr,
+    safe_isinstance,
+    safe_issubclass,
+)
 from .shared_options import EnforceNoUnused, ImportPaths, Paths
 from .signature import (
     ANY_SIGNATURE,
     ARGS,
     ConcreteSignature,
     KWARGS,
     MaybeSignature,
@@ -149,39 +149,44 @@
     display_suggested_type,
     prepare_type,
     should_suggest_type,
 )
 from .type_object import get_mro, TypeObject
 from .value import (
     AlwaysPresentExtension,
+    DeprecatedExtension,
+    SkipDeprecatedExtension,
     annotate_value,
     AnnotatedValue,
     AnySource,
     AnyValue,
     AssertErrorExtension,
     AsyncTaskIncompleteValue,
+    CallableValue,
     CanAssign,
     CanAssignError,
     check_hashability,
     concrete_values_from_iterable,
     ConstraintExtension,
     DictIncompleteValue,
     flatten_values,
     GenericBases,
     GenericValue,
     get_tv_map,
+    is_iterable,
     is_union,
     KnownValue,
     kv_pairs_from_mapping,
     KVPair,
     make_coro_type,
     MultiValuedValue,
     NO_RETURN_VALUE,
     NoReturnConstraintExtension,
     ReferencingValue,
+    replace_known_sequence_value,
     SequenceValue,
     set_self,
     SubclassValue,
     TypedValue,
     TypeVarValue,
     unannotate_value,
     UnboundMethodValue,
@@ -201,14 +206,28 @@
 
 try:
     from ast import Match
 except ImportError:
     # 3.9 and lower
     Match = Any
 
+try:
+    from ast import TryStar
+    from builtins import BaseExceptionGroup, ExceptionGroup
+except ImportError:
+    # 3.10 and lower
+    TryStar = Any
+
+    class BaseExceptionGroup:
+        pass
+
+    class ExceptionGroup:
+        pass
+
+
 T = TypeVar("T")
 U = TypeVar("U")
 AwaitableValue = GenericValue(collections.abc.Awaitable, [TypeVarValue(T)])
 KnownNone = KnownValue(None)
 ExceptionValue = TypedValue(BaseException) | SubclassValue(TypedValue(BaseException))
 ExceptionOrNone = ExceptionValue | KnownNone
 
@@ -1408,16 +1427,18 @@
         else:
             declared_type = current_scope.get_declared_type(varname)
             if declared_type is not None:
                 can_assign = declared_type.can_assign(value, self)
                 if isinstance(can_assign, CanAssignError):
                     self._show_error_if_checking(
                         node,
-                        f"Incompatible assignment: expected {declared_type}, got"
-                        f" {value}",
+                        (
+                            f"Incompatible assignment: expected {declared_type}, got"
+                            f" {value}"
+                        ),
                         error_code=ErrorCode.incompatible_assignment,
                         detail=can_assign.display(),
                     )
             if current_scope.is_final(varname):
                 self._show_error_if_checking(
                     node,
                     f"Cannot assign to final name {varname}",
@@ -2189,25 +2210,134 @@
                         name
                     ),
                     error_code=ErrorCode.bad_nonlocal,
                 )
                 defining_scope = self.scopes.module_scope()
             self._set_name_in_scope(name, node, ReferencingValue(defining_scope, name))
 
+    def check_deprecation(self, node: ast.AST, value: Value) -> bool:
+        if isinstance(value, AnnotatedValue):
+            if value.has_metadata_of_type(SkipDeprecatedExtension):
+                return False
+            for metadata in value.get_metadata_of_type(DeprecatedExtension):
+                self._show_error_if_checking(
+                    node,
+                    f"{value} is deprecated: {metadata.deprecation_message}",
+                    error_code=ErrorCode.deprecated,
+                )
+                return True
+            return self.check_deprecation(node, value.value)
+        if isinstance(value, UnboundMethodValue):
+            method = value.get_method()
+            if method is None:
+                return False
+            return self.check_deprecation(node, KnownValue(method))
+        if isinstance(value, CallableValue):
+            if not isinstance(value.signature, Signature):
+                return False
+            if value.signature.deprecated is None:
+                return False
+            deprecated = value.signature.deprecated
+        elif isinstance(value, KnownValue):
+            deprecated = safe_getattr(value.val, "__deprecated__", None)
+            if deprecated is None:
+                return False
+        else:
+            return False
+        if not safe_isinstance(deprecated, str):
+            # happens with Mock objects
+            return False
+        self._show_error_if_checking(
+            node,
+            f"{value} is deprecated: {deprecated}",
+            error_code=ErrorCode.deprecated,
+        )
+        return True
+
     # Imports
 
     def visit_Import(self, node: ast.Import) -> None:
         self.generic_visit(node)
         if self.scopes.scope_type() == ScopeType.module_scope:
-            self._handle_imports(node.names)
-
             for name in node.names:
                 self.import_name_to_node[name.name] = node
+
+        for alias in node.names:
+            self._try_to_import(alias.name)
+            # "import a.b" sets the name "a", but "import a.b as c" sets "c" to the value "a.b"
+            varname = (
+                alias.name if alias.asname is not None else alias.name.split(".")[0]
+            )
+            mod = self._get_module(varname, node)
+            self._set_alias_in_scope(alias, mod, node=node)
+
+    def _set_alias_in_scope(
+        self,
+        alias: ast.alias,
+        value: Value,
+        *,
+        force_public: bool = False,
+        node: ast.AST,
+    ) -> None:
+        # aliases only have a lineno attached in 3.10+
+        if sys.version_info >= (3, 10):
+            error_node = alias
+        else:
+            error_node = node
+        if self.check_deprecation(error_node, value):
+            value = annotate_value(value, [SkipDeprecatedExtension()])
+        if alias.asname is not None:
+            self._set_name_in_scope(
+                alias.asname,
+                alias,
+                value,
+                private=not force_public and alias.asname != alias.name,
+            )
         else:
-            self._simulate_import(node)
+            self._set_name_in_scope(
+                alias.name.split(".")[0], alias, value, private=not force_public
+            )
+
+    def _get_module(self, name: str, node: ast.AST) -> Value:
+        if name not in sys.modules:
+            self._try_to_import(name)
+        if name in sys.modules:
+            # import a.b.c only succeeds if a.b.c is a module that
+            # exists, but it doesn't return the module a.b.c, it
+            # follows the attribute chain. But this isn't true for
+            # ImportFrom.
+            if isinstance(node, ast.ImportFrom):
+                return KnownValue(sys.modules[name])
+            pieces = name.split(".")
+            base_module = sys.modules.get(pieces[0])
+            for piece in pieces[1:]:
+                if not safe_hasattr(base_module, piece):
+                    self._show_error_if_checking(
+                        node,
+                        (
+                            f"Cannot import {name} because {piece} is not an attribute"
+                            f" of {base_module!r}"
+                        ),
+                        error_code=ErrorCode.import_failed,
+                    )
+                    return AnyValue(AnySource.unresolved_import)
+                base_module = getattr(base_module, piece)
+            return KnownValue(base_module)
+        else:
+            # TODO: Maybe get the module from stubs?
+            self._show_error_if_checking(
+                node, f"Cannot import {name}", error_code=ErrorCode.import_failed
+            )
+            return AnyValue(AnySource.unresolved_import)
+
+    def _try_to_import(self, module_name: str) -> None:
+        try:
+            __import__(module_name)
+        except Exception:
+            pass
 
     def visit_ImportFrom(self, node: ast.ImportFrom) -> None:
         self.generic_visit(node)
         # this is used to decide where to add additional imports (after the first import), so
         # exclude __future__ imports
         if (
             self.scopes.scope_type() == ScopeType.module_scope
@@ -2217,25 +2347,128 @@
             self.import_name_to_node[node.module] = node
         if node.module == "__future__":
             for name in node.names:
                 self.future_imports.add(name.name)
 
         self._maybe_record_usages_from_import(node)
 
-        is_star_import = len(node.names) == 1 and node.names[0].name == "*"
-        force_public = self.filename.endswith("/__init__.py") and node.level == 1
-        if force_public and node.module is not None:
-            # from .a import b implicitly sets a in the parent module's namespace.
-            # We allow relying on this behavior.
-            self._set_name_in_scope(node.module, node)
-        if self.scopes.scope_type() == ScopeType.module_scope and not is_star_import:
-            self._handle_imports(node.names, force_public=force_public)
+        # See if we can get the names from the stub instead
+        if (
+            node.module is not None
+            and node.level == 0
+            # pyanalyze.extensions has a stub only for the purpose of other stubs
+            # it shouldn't be used for runtime imports
+            and node.module != "pyanalyze.extensions"
+        ):
+            path = typeshed_client.ModulePath(tuple(node.module.split(".")))
+            finder = self.checker.ts_finder
+            mod = finder.resolver.get_module(path)
+            if mod.exists:
+                for alias in node.names:
+                    val = finder.resolve_name(node.module, alias.name)
+                    if val is UNINITIALIZED_VALUE:
+                        self._show_error_if_checking(
+                            node,
+                            f"Cannot import name {alias.name!r} from {node.module!r}",
+                            ErrorCode.import_failed,
+                        )
+                        val = AnyValue(AnySource.error)
+                    self._set_alias_in_scope(alias, val, node=node)
+                return
+
+        is_init = self.filename.endswith("/__init__.py")
+        source_module = self._get_import_from_module(node)
+
+        # from .a import b implicitly sets a in the parent module's namespace.
+        # We allow relying on this behavior.
+        if (
+            is_init
+            and node.module is not None
+            and "." not in node.module
+            and node.level == 1
+        ):
+            self._set_name_in_scope(node.module, node, source_module, private=False)
+
+        for alias in node.names:
+            if alias.name == "*":
+                if isinstance(source_module, KnownValue) and isinstance(
+                    source_module.val, types.ModuleType
+                ):
+                    for name, val in source_module.val.__dict__.items():
+                        if name.startswith("_"):
+                            continue
+                        self._set_name_in_scope(
+                            name, alias, KnownValue(val), private=False
+                        )
+                else:
+                    self._show_error_if_checking(
+                        node,
+                        f"Cannot import * from unresolved module {node.module!r}",
+                        ErrorCode.invalid_import,
+                    )
+                continue
+            val = self._get_import_from_value(source_module, alias.name, node)
+            self._set_alias_in_scope(
+                alias, val, force_public=is_init and node.level == 1, node=node
+            )
+
+    def _get_import_from_value(
+        self, source_module: Value, alias_name: str, node: ast.ImportFrom
+    ) -> Value:
+        val = self.get_attribute_from_value(source_module, alias_name)
+        if val is not UNINITIALIZED_VALUE:
+            return val
+        if isinstance(source_module, KnownValue) and isinstance(
+            source_module.val, types.ModuleType
+        ):
+            name = f"{source_module.val.__name__}.{alias_name}"
+            self._try_to_import(name)
+            val = self.get_attribute_from_value(source_module, alias_name)
+            if val is not UNINITIALIZED_VALUE:
+                return val
+
+        self._show_error_if_checking(
+            node,
+            f"Cannot import name {alias_name!r} from {node.module!r}",
+            ErrorCode.import_failed,
+        )
+        return AnyValue(AnySource.error)
+
+    def _get_import_from_module(self, node: ast.ImportFrom) -> Value:
+        if node.level > 0:
+            if self.module is None:
+                return AnyValue(AnySource.unresolved_import)
+            level = node.level
+            if self.filename.endswith("/__init__.py"):
+                level -= 1
+
+            current_module_path: List[str] = self.module.__name__.split(".")
+            if level >= len(current_module_path):
+                self._show_error_if_checking(
+                    node,
+                    "Attempted relative import beyond top-level package",
+                    error_code=ErrorCode.invalid_import,
+                )
+                return AnyValue(AnySource.error)
+            if level:
+                current_module_path = current_module_path[:-level]
+            if node.module is not None:
+                current_module_path.append(node.module)
+            module_name = ".".join(current_module_path)
         else:
-            # For now we always treat star imports as public. We might revisit this later.
-            self._simulate_import(node, force_public=True)
+            # Should be disallowed by the AST
+            if node.module is None:
+                self._show_error_if_checking(
+                    node,
+                    "Attempted absolute import without module name",
+                    error_code=ErrorCode.invalid_import,
+                )
+                return AnyValue(AnySource.error)
+            module_name = node.module
+        return self._get_module(module_name, node)
 
     def _maybe_record_usages_from_import(self, node: ast.ImportFrom) -> None:
         if self.unused_finder is None or self.module is None:
             return
         if self._is_unimportable_module(node):
             return
         if node.level == 0:
@@ -2269,138 +2502,14 @@
         if isinstance(node, ast.ImportFrom):
             # the split is needed for cases like "from foo.bar import baz" if foo is unimportable
             return node.module is not None and node.module.split(".")[0] in unimportable
         else:
             # need the split if the code is "import foo.bar as bar" if foo is unimportable
             return any(name.name.split(".")[0] in unimportable for name in node.names)
 
-    def _simulate_import(
-        self, node: Union[ast.ImportFrom, ast.Import], *, force_public: bool = False
-    ) -> None:
-        """Set the names retrieved from an import node in nontrivial situations.
-
-        For simple imports (module-global imports that are not "from ... import *"), we can just
-        retrieve the imported names from the module dictionary, but this is not possible with
-        import * or when the import is within a function.
-
-        To figure out what names would be imported in these cases, we create a fake module
-        consisting of just the import statement, eval it, and set all the names in its __dict__
-        in the current module scope.
-
-        TODO: Replace this with code that just evaluates the import without going
-        through this exec shenanigans.
-
-        """
-        if self.module is None:
-            self._handle_imports(node.names, force_public=force_public)
-            return
-
-        # See if we can get the names from the stub instead
-        if (
-            isinstance(node, ast.ImportFrom)
-            and node.module is not None
-            and node.level == 0
-        ):
-            path = typeshed_client.ModulePath(tuple(node.module.split(".")))
-            finder = self.checker.ts_finder
-            mod = finder.resolver.get_module(path)
-            if mod.exists:
-                for alias in node.names:
-                    val = finder.resolve_name(node.module, alias.name)
-                    if val is UNINITIALIZED_VALUE:
-                        self._show_error_if_checking(
-                            node,
-                            f"Cannot import name {alias.name!r} from {node.module!r}",
-                            ErrorCode.import_failed,
-                        )
-                        val = AnyValue(AnySource.error)
-                    self._set_name_in_scope(
-                        alias.asname or alias.name, alias, val, private=not force_public
-                    )
-                return
-
-        source_code = decompile(node)
-
-        if self._is_unimportable_module(node):
-            self._handle_imports(node.names, force_public=force_public)
-            self.log(logging.INFO, "Ignoring import node", source_code)
-            return
-
-        # create a pseudo-module and examine its dictionary to figure out what this imports
-        # default to the current __file__ if necessary
-        module_file = safe_getattr(self.module, "__file__", __file__)
-        random_suffix = "".join(
-            random.choice(string.ascii_lowercase) for _ in range(10)
-        )
-        pseudo_module_file = re.sub(r"\.pyc?$", random_suffix + ".py", module_file)
-        is_init = os.path.basename(module_file) in ("__init__.py", "__init__.pyc")
-        if is_init:
-            pseudo_module_name = self.module.__name__ + "." + random_suffix
-        else:
-            pseudo_module_name = self.module.__name__ + random_suffix
-
-        # Apparently doing 'from file_in_package import *' in an __init__.py also adds
-        # file_in_package to the module's scope.
-        if (
-            isinstance(node, ast.ImportFrom)
-            and is_init
-            and node.module is not None
-            and "." not in node.module
-        ):  # not in the package
-            if node.level == 1 or (node.level == 0 and node.module not in sys.modules):
-                self._set_name_in_scope(
-                    node.module,
-                    node,
-                    TypedValue(types.ModuleType),
-                    private=not force_public,
-                )
-
-        with tempfile.NamedTemporaryFile(suffix=".py") as f:
-            f.write(source_code.encode("utf-8"))
-            f.flush()
-            f.seek(0)
-            try:
-                pseudo_module = importer.import_module(pseudo_module_name, Path(f.name))
-            except Exception:
-                # sets the name of the imported module to Any so we don't get further
-                # errors
-                self._handle_imports(node.names, force_public=force_public)
-                return
-            finally:
-                # clean up pyc file
-                try:
-                    os.unlink(pseudo_module_file + "c")
-                except OSError:
-                    pass
-                if pseudo_module_name in sys.modules:
-                    del sys.modules[pseudo_module_name]
-
-        for name, value in pseudo_module.__dict__.items():
-            if name.startswith("__") or (
-                hasattr(builtins, name) and value == getattr(builtins, name)
-            ):
-                continue
-            self._set_name_in_scope(
-                name,
-                node,
-                KnownValue(value),
-                private=not force_public,
-                lookup_node=(node, name),
-            )
-
-    def _handle_imports(
-        self, names: Iterable[ast.alias], *, force_public: bool = False
-    ) -> None:
-        for node in names:
-            if node.asname is not None:
-                self._set_name_in_scope(node.asname, node)
-            else:
-                varname = node.name.split(".")[0]
-                self._set_name_in_scope(varname, node, private=not force_public)
-
     # Comprehensions
 
     def visit_DictComp(self, node: ast.DictComp) -> Value:
         return self._visit_sequence_comp(node, dict)
 
     def visit_ListComp(self, node: ast.ListComp) -> Value:
         return self._visit_sequence_comp(node, list)
@@ -2560,19 +2669,85 @@
         # Returning a SequenceValue here instead of a GenericValue allows
         # later code to modify this container.
         return SequenceValue(typ, [(True, member_value)])
 
     # Literals and displays
 
     def visit_JoinedStr(self, node: ast.JoinedStr) -> Value:
-        # JoinedStr is the node type for f-strings.
-        # Not too much to check here. Perhaps we can add checks that format specifiers
-        # are valid.
-        self._generic_visit_list(node.values)
-        return TypedValue(str)
+        elements = self._generic_visit_list(node.values)
+        limit = self.options.get_value_for(UnionSimplificationLimit)
+        possible_values: List[List[str]] = [[]]
+        for elt in elements:
+            subvals = list(flatten_values(elt))
+            # Bail out if the list of possible values gets too long.
+            if len(possible_values) * len(subvals) > limit:
+                return TypedValue(str)
+            to_add = []
+            for subval in subvals:
+                if not isinstance(subval, KnownValue):
+                    return TypedValue(str)
+                if not isinstance(subval.val, str):
+                    return TypedValue(str)
+                to_add.append(subval.val)
+            possible_values = [
+                lst + [new_elt] for lst in possible_values for new_elt in to_add
+            ]
+        return unite_values(*[KnownValue("".join(lst)) for lst in possible_values])
+
+    def visit_FormattedValue(self, node: ast.FormattedValue) -> Value:
+        val = self.visit(node.value)
+        format_spec_val = (
+            self.visit(node.format_spec) if node.format_spec else KnownValue("")
+        )
+        if isinstance(format_spec_val, KnownValue) and isinstance(
+            format_spec_val.val, str
+        ):
+            format_spec = format_spec_val.val
+        else:
+            # TODO: statically check whether the format specifier is valid.
+            return TypedValue(str)
+        possible_vals = []
+        for subval in flatten_values(val):
+            possible_vals.append(
+                self._visit_single_formatted_value(subval, node, format_spec)
+            )
+        return unite_and_simplify(
+            *possible_vals, limit=self.options.get_value_for(UnionSimplificationLimit)
+        )
+
+    def _visit_single_formatted_value(
+        self, val: Value, node: ast.FormattedValue, format_spec: str
+    ) -> Value:
+        if not isinstance(val, KnownValue):
+            return TypedValue(str)
+        output = val.val
+        if node.conversion != -1:
+            unsupported_conversion = False
+            try:
+                if node.conversion == ord("a"):
+                    output = ascii(output)
+                elif node.conversion == ord("s"):
+                    output = str(output)
+                elif node.conversion == ord("r"):
+                    output = repr(output)
+                else:
+                    unsupported_conversion = True
+            except Exception:
+                # str/repr/ascii failed
+                return TypedValue(str)
+            if unsupported_conversion:
+                raise NotImplementedError(
+                    f"Unsupported converion specifier {node.conversion}"
+                )
+        try:
+            output = format(output, format_spec)
+        except Exception:
+            # format failed
+            return TypedValue(str)
+        return KnownValue(output)
 
     def visit_Constant(self, node: ast.Constant) -> Value:
         # replaces Num, Str, etc. in 3.8+
         if isinstance(node.value, str):
             self._maybe_show_missing_f_error(node, node.value)
         return KnownValue(node.value)
 
@@ -3055,15 +3230,15 @@
                 val = KnownValue(True)
             else:
                 val = TypedValue(bool)
             return annotate_with_constraint(val, constraint.invert())
         else:
             operand = self.composite_from_node(node.operand)
             _, method = UNARY_OPERATION_TO_DESCRIPTION_AND_METHOD[type(node.op)]
-            val = self._check_dunder_call(node, operand, method, [], allow_call=True)
+            val, _ = self._check_dunder_call(node, operand, method, [], allow_call=True)
             return val
 
     def visit_BinOp(self, node: ast.BinOp) -> Value:
         left = self.composite_from_node(node.left)
         right = self.composite_from_node(node.right)
         return self._visit_binop_internal(
             node.left, left, node.op, node.right, right, node
@@ -3120,15 +3295,18 @@
         allow_call = allow_call and method not in self.options.get_value_for(
             DisallowCallsToDunders
         )
 
         if is_inplace:
             assert imethod is not None, f"no inplace method available for {op}"
             with self.catch_errors() as inplace_errors:
-                inplace_result = self._check_dunder_call(
+                # Not _check_dunder_call_or_catch because if the call doesn't
+                # typecheck it normally returns NotImplemented and we try the
+                # non-inplace method next.
+                inplace_result, _ = self._check_dunder_call(
                     source_node,
                     left_composite,
                     imethod,
                     [right_composite],
                     allow_call=allow_call,
                 )
             if not inplace_errors:
@@ -3156,33 +3334,72 @@
     ) -> Value:
         left = left_composite.value
         right = right_composite.value
         (description, method, _, rmethod) = BINARY_OPERATION_TO_DESCRIPTION_AND_METHOD[
             type(op)
         ]
         if rmethod is None:
-            return self._check_dunder_call(
+            # "in" falls back to __iter__ and then to __getitem__ if __contains__ is not defined
+            if method == "__contains__":
+                contains_result_or_errors = self._check_dunder_call_or_catch(
+                    source_node,
+                    left_composite,
+                    method,
+                    [right_composite],
+                    allow_call=allow_call,
+                )
+                if isinstance(contains_result_or_errors, Value):
+                    return contains_result_or_errors
+
+                iterable_type = is_iterable(left, self)
+                if isinstance(iterable_type, Value):
+                    can_assign = iterable_type.can_assign(right, self)
+                    if isinstance(can_assign, CanAssignError):
+                        self._show_error_if_checking(
+                            source_node,
+                            "Unsupported operand for 'in'",
+                            ErrorCode.incompatible_argument,
+                            detail=str(can_assign),
+                        )
+                        return TypedValue(bool)
+                    else:
+                        return TypedValue(bool)
+
+                getitem_result = self._check_dunder_call_or_catch(
+                    source_node,
+                    left_composite,
+                    "__getitem__",
+                    [right_composite],
+                    allow_call=allow_call,
+                )
+                if isinstance(getitem_result, Value):
+                    return TypedValue(bool)  # Always returns a bool
+                self.show_caught_errors(contains_result_or_errors)
+                return TypedValue(bool)
+
+            result, _ = self._check_dunder_call(
                 source_node,
                 left_composite,
                 method,
                 [right_composite],
                 allow_call=allow_call,
             )
+            return result
 
         with self.catch_errors() as left_errors:
-            left_result = self._check_dunder_call(
+            left_result, _ = self._check_dunder_call(
                 source_node,
                 left_composite,
                 method,
                 [right_composite],
                 allow_call=allow_call,
             )
 
         with self.catch_errors() as right_errors:
-            right_result = self._check_dunder_call(
+            right_result, _ = self._check_dunder_call(
                 source_node,
                 right_composite,
                 rmethod,
                 [left_composite],
                 allow_call=allow_call,
             )
         if left_errors:
@@ -3253,42 +3470,41 @@
         if return_value is NO_RETURN_VALUE:
             self._set_name_in_scope(LEAVES_SCOPE, node, AnyValue(AnySource.marker))
         return return_value
 
     def unpack_awaitable(self, composite: Composite, node: ast.AST) -> Value:
         tv_map = get_tv_map(AwaitableValue, composite.value, self)
         if isinstance(tv_map, CanAssignError):
-            return self._check_dunder_call(node, composite, "__await__", [])
+            result, _ = self._check_dunder_call(node, composite, "__await__", [])
+            return result
         else:
             return tv_map.get(T, AnyValue(AnySource.generic_argument))
 
     def visit_YieldFrom(self, node: ast.YieldFrom) -> Value:
         self.is_generator = True
         value = self.visit(node.value)
         tv_map = get_tv_map(GeneratorValue, value, self)
         if isinstance(tv_map, CanAssignError):
             can_assign = get_tv_map(AwaitableValue, value, self)
             if not isinstance(can_assign, CanAssignError):
                 tv_map = {
                     ReturnT: can_assign.get(T, AnyValue(AnySource.generic_argument))
                 }
             else:
-                can_assign = get_tv_map(IterableValue, value, self)
-                if isinstance(can_assign, CanAssignError):
+                iterable_type = is_iterable(value, self)
+                if isinstance(iterable_type, CanAssignError):
                     self._show_error_if_checking(
                         node,
                         f"Cannot use {value} in yield from",
                         error_code=ErrorCode.bad_yield_from,
                         detail=can_assign.display(),
                     )
                     tv_map = {ReturnT: AnyValue(AnySource.error)}
                 else:
-                    tv_map = {
-                        YieldT: can_assign.get(T, AnyValue(AnySource.generic_argument))
-                    }
+                    tv_map = {YieldT: iterable_type}
 
         if self.current_function_info is not None:
             expected_yield = self.current_function_info.get_generator_yield_type(self)
             yield_type = tv_map.get(YieldT, AnyValue(AnySource.generic_argument))
             can_assign = expected_yield.can_assign(yield_type, self)
             if isinstance(can_assign, CanAssignError):
                 self._show_error_if_checking(
@@ -3300,16 +3516,18 @@
 
             expected_send = self.current_function_info.get_generator_send_type(self)
             send_type = tv_map.get(SendT, AnyValue(AnySource.generic_argument))
             can_assign = send_type.can_assign(expected_send, self)
             if isinstance(can_assign, CanAssignError):
                 self._show_error_if_checking(
                     node,
-                    f"Cannot send {send_type} to a generator (expected"
-                    f" {expected_send})",
+                    (
+                        f"Cannot send {send_type} to a generator (expected"
+                        f" {expected_send})"
+                    ),
                     error_code=ErrorCode.incompatible_yield,
                     detail=can_assign.display(),
                 )
 
         return tv_map.get(ReturnT, AnyValue(AnySource.generic_argument))
 
     def visit_Yield(self, node: ast.Yield) -> Value:
@@ -3341,16 +3559,18 @@
         if self.current_function_info is None:
             return AnyValue(AnySource.inference)
         yield_type = self.current_function_info.get_generator_yield_type(self)
         can_assign = yield_type.can_assign(value, self)
         if isinstance(can_assign, CanAssignError):
             self._show_error_if_checking(
                 node,
-                f"Cannot assign value of type {value} to yield expression of type"
-                f" {yield_type}",
+                (
+                    f"Cannot assign value of type {value} to yield expression of type"
+                    f" {yield_type}"
+                ),
                 error_code=ErrorCode.incompatible_yield,
                 detail=can_assign.display(),
             )
         return self.current_function_info.get_generator_send_type(self)
 
     def _unwrap_yield_result(self, node: ast.AST, value: Value) -> Value:
         if isinstance(value, AsyncTaskIncompleteValue):
@@ -3443,16 +3663,18 @@
                         detail=can_assign.display(),
                     )
         elif self.expected_return_value is not None:
             can_assign = self.expected_return_value.can_assign(value, self)
             if isinstance(can_assign, CanAssignError):
                 self._show_error_if_checking(
                     node,
-                    f"Declared return type {self.expected_return_value} is incompatible"
-                    f" with actual return type {value}",
+                    (
+                        f"Declared return type {self.expected_return_value} is"
+                        f" incompatible with actual return type {value}"
+                    ),
                     error_code=ErrorCode.incompatible_return_value,
                     detail=can_assign.display(),
                 )
         if (
             self.expected_return_value == KnownNone
             and value != KnownNone
             and value is not NO_RETURN_VALUE
@@ -3627,16 +3849,16 @@
         Returns a tuple of two values:
         - A Value object representing a member of the iterator.
         - The number of elements in the iterator, or None if the number is unknown.
 
         """
         composite = self.composite_from_node(node)
         if is_async:
-            iterator = self._check_dunder_call(node, composite, "__aiter__", [])
-            anext = self._check_dunder_call(
+            iterator, _ = self._check_dunder_call(node, composite, "__aiter__", [])
+            anext, _ = self._check_dunder_call(
                 node, Composite(iterator, None, node), "__anext__", []
             )
             return self.unpack_awaitable(Composite(anext), node)
         iterated = composite.value
         result = concrete_values_from_iterable(iterated, self)
         if isinstance(result, CanAssignError):
             self._show_error_if_checking(
@@ -3720,15 +3942,17 @@
                 # assume it does not suppress exceptions.
                 can_suppress = False
         if node.optional_vars is not None:
             with qcore.override(self, "being_assigned", assigned):
                 self.visit(node.optional_vars)
         return can_suppress
 
-    def visit_try_except(self, node: ast.Try) -> None:
+    def visit_try_except(
+        self, node: Union[ast.Try, TryStar], *, is_try_star: bool = False
+    ) -> None:
         with self.scopes.subscope():
             with self.scopes.subscope() as dummy_scope:
                 pass
 
             with self.scopes.subscope() as failure_scope:
                 with self.scopes.suppressing_subscope() as success_scope:
                     self._generic_visit_list(node.body)
@@ -3741,73 +3965,119 @@
             except_scopes = []
             for handler in node.handlers:
                 with self.scopes.subscope() as except_scope:
                     except_scopes.append(except_scope)
                     # reset yield checks between branches to avoid incorrect errors when we yield
                     # both in the try and the except block
                     self.yield_checker.reset_yield_checks()
-                    self.scopes.combine_subscopes([dummy_scope, failure_scope])
+                    # With except*, multiple except* blocks may run, so we need
+                    # to combine not just the failure scope, but also the previous
+                    # except_scopes.
+                    if is_try_star:
+                        subscopes = [dummy_scope, failure_scope, *except_scopes]
+                    else:
+                        subscopes = [dummy_scope, failure_scope]
+                    self.scopes.combine_subscopes(subscopes)
                     self.visit(handler)
 
         self.scopes.combine_subscopes([else_scope, *except_scopes])
 
-    def visit_Try(self, node: ast.Try) -> None:
-        # py3 combines the Try and Try/Finally nodes
+    def visit_Try(
+        self, node: Union[ast.Try, TryStar], *, is_try_star: bool = False
+    ) -> None:
         if node.finalbody:
             with self.scopes.subscope() as failure_scope:
                 with self.scopes.suppressing_subscope() as success_scope:
-                    self.visit_try_except(node)
+                    self.visit_try_except(node, is_try_star=is_try_star)
 
             # If the try block fails
             with self.scopes.subscope():
                 self.scopes.combine_subscopes([failure_scope])
                 self._generic_visit_list(node.finalbody)
 
             # For the case where execution continues after the try-finally
             self.scopes.combine_subscopes([success_scope])
             self._generic_visit_list(node.finalbody)
         else:
             # Life is much simpler without finally
-            self.visit_try_except(node)
+            self.visit_try_except(node, is_try_star=is_try_star)
         self.yield_checker.reset_yield_checks()
 
+    def visit_TryStar(self, node: TryStar) -> None:
+        self.visit_Try(node, is_try_star=True)
+
     def visit_ExceptHandler(self, node: ast.ExceptHandler) -> None:
         if node.type is not None:
             typ = self.visit(node.type)
-            if isinstance(typ, KnownValue):
-                val = typ.val
-                if isinstance(val, tuple):
-                    if all(self._check_valid_exception_class(cls, node) for cls in val):
-                        to_assign = unite_values(*[TypedValue(cls) for cls in val])
-                    else:
-                        to_assign = TypedValue(BaseException)
-                else:
-                    if self._check_valid_exception_class(val, node):
-                        to_assign = TypedValue(val)
-                    else:
-                        to_assign = TypedValue(BaseException)
-            else:
-                # maybe this should be an error, exception classes should virtually always be
-                # statically findable
-                to_assign = TypedValue(BaseException)
+            is_try_star = not isinstance(self.node_context.contexts[-2], ast.Try)
+            possible_types = self._extract_exception_types(
+                typ, node, is_try_star=is_try_star
+            )
             if node.name is not None:
+                to_assign = unite_values(*[typ for _, typ in possible_types])
+                if is_try_star:
+                    if all(is_exception for is_exception, _ in possible_types):
+                        base = ExceptionGroup
+                    else:
+                        base = BaseExceptionGroup
+                    to_assign = GenericValue(base, [to_assign])
                 self._set_name_in_scope(node.name, node, value=to_assign, private=True)
 
         self._generic_visit_list(node.body)
 
-    def _check_valid_exception_class(self, val: object, node: ast.AST) -> bool:
-        if not (isinstance(val, type) and issubclass(val, BaseException)):
-            self._show_error_if_checking(
-                node,
-                f"{val!r} is not an exception class",
-                error_code=ErrorCode.bad_except_handler,
-            )
-            return False
-        else:
-            return True
+    def _extract_exception_types(
+        self, typ: Value, node: ast.AST, is_try_star: bool = False
+    ) -> List[Tuple[bool, Value]]:
+        possible_types = []
+        for subval in flatten_values(typ, unwrap_annotated=True):
+            subval = replace_known_sequence_value(subval)
+            if isinstance(subval, SequenceValue) and subval.typ is tuple:
+                for _, elt in subval.members:
+                    possible_types += self._extract_exception_types(
+                        elt, node, is_try_star=is_try_star
+                    )
+                continue
+            elif isinstance(subval, GenericValue) and subval.typ is tuple:
+                possible_types += self._extract_exception_types(
+                    subval.args[0], node, is_try_star=is_try_star
+                )
+                continue
+            elif (
+                isinstance(subval, SubclassValue)
+                and isinstance(subval.typ, TypedValue)
+                and isinstance(subval.typ.typ, type)
+            ):
+                subval = KnownValue(subval.typ.typ)
+            if isinstance(subval, KnownValue):
+                if isinstance(subval.val, type) and issubclass(
+                    subval.val, BaseException
+                ):
+                    if is_try_star and issubclass(subval.val, BaseExceptionGroup):
+                        self._show_error_if_checking(
+                            node,
+                            (
+                                "ExceptionGroup cannot be used as the type in an"
+                                f" except* clause: {subval.val!r}"
+                            ),
+                            error_code=ErrorCode.bad_except_handler,
+                        )
+                    is_exception = issubclass(subval.val, Exception)
+                    possible_types.append((is_exception, TypedValue(subval.val)))
+                else:
+                    self._show_error_if_checking(
+                        node,
+                        f"{subval!r} is not an exception class",
+                        error_code=ErrorCode.bad_except_handler,
+                    )
+                    possible_types.append((False, TypedValue(BaseException)))
+            else:
+                # TODO consider raising an error for except classes
+                # that cannot be statically resolved.
+                possible_types.append((False, TypedValue(BaseException)))
+        return possible_types
 
     def visit_If(self, node: ast.If) -> None:
         _, constraint = self.constraint_from_condition(node.test)
         # reset yield checks to avoid incorrect errors when we yield in both the condition and one
         # of the blocks
         self.yield_checker.reset_yield_checks()
         with self.scopes.subscope() as body_scope:
@@ -3975,16 +4245,18 @@
             value = self.visit(node.value)
 
             if expected_type is not None:
                 can_assign = expected_type.can_assign(value, self)
                 if isinstance(can_assign, CanAssignError):
                     self._show_error_if_checking(
                         node,
-                        f"Incompatible assignment: expected {expected_type}, got"
-                        f" {value}",
+                        (
+                            f"Incompatible assignment: expected {expected_type}, got"
+                            f" {value}"
+                        ),
                         error_code=ErrorCode.incompatible_assignment,
                         detail=can_assign.display(),
                     )
                 # We set the declared type on initial assignment, so that the
                 # annotation can be used to adjust pyanalyze's type inference.
                 value = expected_type
 
@@ -4026,14 +4298,15 @@
     ) -> Composite:
         if force_read or self._is_read_ctx(node.ctx):
             self.yield_checker.record_usage(node.id, node)
             value, origin = self.resolve_name(node)
             varname_value = self.checker.maybe_get_variable_name_value(node.id)
             if varname_value is not None and self._should_use_varname_value(value):
                 value = varname_value
+            self.check_deprecation(node, value)
             return Composite(value, VarnameWithOrigin(node.id, origin), node)
         elif self._is_write_ctx(node.ctx):
             if self._name_node_to_statement is not None:
                 statement = self.node_context.nearest_enclosing(
                     (ast.stmt, ast.comprehension)
                 )
                 self._name_node_to_statement[node] = statement
@@ -4206,17 +4479,18 @@
                 local_value = self._get_composite(
                     composite_var.get_varname(), node, return_value
                 )
                 if local_value is not UNINITIALIZED_VALUE:
                     return_value = local_value
             return return_value
         elif isinstance(node.ctx, ast.Del):
-            return self._check_dunder_call(
+            result, _ = self._check_dunder_call(
                 node.value, root_composite, "__delitem__", [index_composite]
             )
+            return result
         else:
             self.show_error(
                 node,
                 f"Unexpected subscript context: {node.ctx}",
                 ErrorCode.unexpected_node,
             )
             return AnyValue(AnySource.error)
@@ -4233,56 +4507,93 @@
             self.show_error(
                 node,
                 f"Object of type {callee_val} does not support {method_name!r}",
                 error_code=ErrorCode.unsupported_operation,
             )
         return method_object
 
+    def _check_dunder_call_or_catch(
+        self,
+        node: ast.AST,
+        callee_composite: Composite,
+        method_name: str,
+        args: Iterable[Composite],
+        allow_call: bool = False,
+    ) -> Union[Value, List[node_visitor.Error]]:
+        """Use this for checking a dunder call that may fall back to another.
+
+        There are three cases:
+        - The dunder does not exist. We want to defer the error, in case the fallback
+          exists.
+        - The dunder exists and the call typechecks. We want to return its result.
+        - The dunder exists, but the call doesn't typecheck. We want to show the error
+          immediately and return Any.
+
+        """
+        with self.catch_errors() as errors:
+            result, exists = self._check_dunder_call(
+                node, callee_composite, method_name, args, allow_call=allow_call
+            )
+        if not errors:
+            return result
+        elif exists:
+            # Inplace method exists, but it doesn't accept these arguments
+            self.show_caught_errors(errors)
+            return result
+        else:
+            return errors
+
     def _check_dunder_call(
         self,
         node: ast.AST,
         callee_composite: Composite,
         method_name: str,
         args: Iterable[Composite],
         allow_call: bool = False,
-    ) -> Value:
+    ) -> Tuple[Value, bool]:
         if isinstance(callee_composite.value, MultiValuedValue):
             composites = [
                 Composite(val, callee_composite.varname, callee_composite.node)
                 for val in callee_composite.value.vals
             ]
             with qcore.override(self, "in_union_decomposition", True):
-                values = [
+                values_and_exists = [
                     self._check_dunder_call_no_mvv(
                         node, composite, method_name, args, allow_call
                     )
                     for composite in composites
                 ]
-            return unite_and_simplify(
-                *values, limit=self.options.get_value_for(UnionSimplificationLimit)
+            values = [value for value, _ in values_and_exists]
+            # TODO: We should do something more complex when unions are involved.
+            exists = all(exists for _, exists in values_and_exists)
+            return (
+                unite_and_simplify(
+                    *values, limit=self.options.get_value_for(UnionSimplificationLimit)
+                ),
+                exists,
             )
         return self._check_dunder_call_no_mvv(
             node, callee_composite, method_name, args, allow_call
         )
 
     def _check_dunder_call_no_mvv(
         self,
         node: ast.AST,
         callee_composite: Composite,
         method_name: str,
         args: Iterable[Composite],
         allow_call: bool = False,
-    ) -> Value:
+    ) -> Tuple[Value, bool]:
         method_object = self._get_dunder(node, callee_composite.value, method_name)
         if method_object is UNINITIALIZED_VALUE:
-            return AnyValue(AnySource.error)
+            return AnyValue(AnySource.error), False
         return_value = self.check_call(
             node, method_object, [callee_composite, *args], allow_call=allow_call
         )
-        return return_value
+        return return_value, True
 
     def _get_composite(self, composite: Varname, node: ast.AST, value: Value) -> Value:
         local_value, _ = self.scopes.current_scope().get_local(
             composite, node, self.state, fallback_value=value
         )
         if isinstance(local_value, MultiValuedValue):
             vals = [val for val in local_value.vals if val is not UNINITIALIZED_VALUE]
@@ -4350,14 +4661,15 @@
             value = self.get_attribute(
                 root_composite,
                 node.attr,
                 node,
                 use_fallback=True,
                 ignore_none=self.options.get_value_for(IgnoreNoneAttributes),
             )
+            self.check_deprecation(node, value)
             if self._should_use_varname_value(value):
                 varname_value = self.checker.maybe_get_variable_name_value(node.attr)
                 if varname_value is not None:
                     return Composite(varname_value, composite, node)
             if (
                 composite is not None
                 and self.scopes.scope_type() == ScopeType.function_scope
@@ -5018,21 +5330,14 @@
                     }
                 )
         if attribute_checker is not None:
             all_failures += attribute_checker.all_failures
         return all_failures
 
     @classmethod
-    def _should_ignore_module(cls, module_name: str) -> bool:
-        """Override this to ignore some modules."""
-        # exclude test modules for now to avoid spurious failures
-        # TODO(jelle): enable for test modules too
-        return module_name.split(".")[-1].startswith("test")
-
-    @classmethod
     def check_file_in_worker(
         cls,
         filename: str,
         attribute_checker: Optional[ClassAttributeChecker] = None,
         **kwargs: Any,
     ) -> Tuple[List[node_visitor.Failure], Any]:
         failures = cls.check_file(
```

### Comparing `pyanalyze-0.8.0/pyanalyze/node_visitor.py` & `pyanalyze-0.9.0/pyanalyze/node_visitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 import codemod
 import qcore
 from ast_decompiler import decompile
 from typing_extensions import NotRequired, Protocol, TypedDict
 
 from . import analysis_lib
 
+Error = Dict[str, Any]
+
 
 @dataclass(frozen=True)
 class _FakeNode:
     lineno: int
     col_offset: int
 
 
@@ -537,20 +539,20 @@
             return None
         else:
             return {
                 code: cls.is_enabled_by_default(code) for code in cls.error_code_enum
             }
 
     @contextmanager
-    def catch_errors(self) -> Iterator[List[Dict[str, Any]]]:
+    def catch_errors(self) -> Iterator[List[Error]]:
         caught_errors = []
         with qcore.override(self, "caught_errors", caught_errors):
             yield caught_errors
 
-    def show_caught_errors(self, errors: Iterable[Dict[str, Any]]) -> None:
+    def show_caught_errors(self, errors: Iterable[Error]) -> None:
         for error in errors:
             self.show_error(**error)
 
     def is_enabled(self, error_code: Enum) -> bool:
         if self.settings is not None:
             return self.settings.get(error_code, True)
         return True
```

### Comparing `pyanalyze-0.8.0/pyanalyze/options.py` & `pyanalyze-0.9.0/pyanalyze/options.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/patma.py` & `pyanalyze-0.9.0/pyanalyze/patma.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,16 +268,18 @@
                 kv_pairs, key_val, self.visitor, optional_pairs, removed_pairs
             )
             optional_pairs |= new_optional_pairs
             removed_pairs |= new_removed_pairs
             if value is UNINITIALIZED_VALUE:
                 self.visitor.show_error(
                     node,
-                    f"Impossible pattern: {self.visitor.match_subject.value} has no key"
-                    f" {key_val}",
+                    (
+                        f"Impossible pattern: {self.visitor.match_subject.value} has no"
+                        f" key {key_val}"
+                    ),
                     ErrorCode.impossible_pattern,
                 )
                 value = AnyValue(AnySource.error)
             with qcore.override(self.visitor, "match_subject", Composite(value)):
                 constraints.append(self.visit(pattern))
         if node.rest is not None:
             new_kv_pairs = []
@@ -326,16 +328,18 @@
                     ErrorCode.bad_match,
                     detail=str(match_args),
                 )
                 match_args = [SpecialPositionalMatch.error for _ in node.patterns]
             if len(node.patterns) > len(match_args):
                 self.visitor.show_error(
                     node.cls,
-                    f"{cls} takes at most {len(match_args)} positional subpatterns, but"
-                    f" {len(match_args)} were provided",
+                    (
+                        f"{cls} takes at most {len(match_args)} positional subpatterns,"
+                        f" but {len(match_args)} were provided"
+                    ),
                     ErrorCode.bad_match,
                     detail=str(match_args),
                 )
                 match_args = [SpecialPositionalMatch.error for _ in node.patterns]
             patterns = [*zip(match_args, node.patterns), *patterns]
 
         seen_names = set()
@@ -409,16 +413,18 @@
             return NULL_CONSTRAINT
         return Constraint(varname, typ, True, value)
 
     def check_impossible_pattern(self, node: ast.AST, value: Value) -> None:
         if not is_overlapping(self.visitor.match_subject.value, value, self.visitor):
             self.visitor.show_error(
                 node,
-                f"Impossible pattern: {self.visitor.match_subject.value} can never be"
-                f" {value}",
+                (
+                    f"Impossible pattern: {self.visitor.match_subject.value} can never"
+                    f" be {value}"
+                ),
                 ErrorCode.impossible_pattern,
             )
 
 
 def index_of(elts: Sequence[T], pred: Callable[[T], bool]) -> Optional[int]:
     for i, elt in enumerate(elts):
         if pred(elt):
```

### Comparing `pyanalyze-0.8.0/pyanalyze/predicates.py` & `pyanalyze-0.9.0/pyanalyze/predicates.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/reexport.py` & `pyanalyze-0.9.0/pyanalyze/reexport.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/safe.py` & `pyanalyze-0.9.0/pyanalyze/safe.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/shared_options.py` & `pyanalyze-0.9.0/pyanalyze/shared_options.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/signature.py` & `pyanalyze-0.9.0/pyanalyze/signature.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 
 import asynq
 import qcore
 from qcore.helpers import safe_str
 from typing_extensions import assert_never, Literal, Protocol, Self
 
 from .error_code import ErrorCode
+from .safe import safe_getattr
+from .node_visitor import Replacement
+from .options import IntegerOption
 from .stacked_scopes import (
     AbstractConstraint,
     AndConstraint,
     Composite,
     Constraint,
     ConstraintType,
     NULL_CONSTRAINT,
@@ -84,14 +87,15 @@
     MultiValuedValue,
     NO_RETURN_VALUE,
     NoReturnConstraintExtension,
     NoReturnGuardExtension,
     ParameterTypeGuardExtension,
     ParamSpecArgsValue,
     ParamSpecKwargsValue,
+    is_iterable,
     replace_known_sequence_value,
     SequenceValue,
     stringify_object,
     TypedDictValue,
     TypedValue,
     TypeGuardExtension,
     TypeVarLike,
@@ -112,14 +116,22 @@
 ELLIPSIS = qcore.MarkerObject("ellipsis")
 ELLIPSIS_COMPOSITE = Composite(AnyValue(AnySource.ellipsis_callable))
 
 # TODO turn on
 USE_CHECK_CALL_FOR_CAN_ASSIGN = False
 
 
+class MaximumPositionalArgs(IntegerOption):
+    """If calls have more than this many positional arguments, attempt to
+    turn them into keyword arguments."""
+
+    default_value = 10
+    name = "maximum_positional_args"
+
+
 class InvalidSignature(Exception):
     """Raised when an invalid signature is encountered."""
 
 
 @dataclass
 class PossibleArg:
     # Label used for arguments that may not be present at runtiime.
@@ -149,23 +161,26 @@
 ]
 
 # Arguments bound to a call
 BoundArgs = Dict[str, Tuple[Position, Composite]]
 
 
 class CheckCallContext(Protocol):
-    visitor: Optional["NameCheckVisitor"]
+    @property
+    def visitor(self) -> Optional["NameCheckVisitor"]:
+        raise NotImplementedError
 
     def on_error(
         self,
         __message: str,
         *,
         code: ErrorCode = ...,
         node: Optional[ast.AST] = ...,
         detail: Optional[str] = ...,
+        replacement: Optional[Replacement] = ...,
     ) -> object:
         raise NotImplementedError
 
     @property
     def can_assign_ctx(self) -> CanAssignContext:
         raise NotImplementedError
 
@@ -179,14 +194,15 @@
     def on_error(
         self,
         message: str,
         *,
         code: ErrorCode = ErrorCode.incompatible_call,
         node: Optional[ast.AST] = None,
         detail: Optional[str] = ...,
+        replacement: Optional[Replacement] = ...,
     ) -> object:
         self.errors.append(message)
         return None
 
 
 @dataclass
 class _VisitorBasedContext:
@@ -200,20 +216,23 @@
     def on_error(
         self,
         message: str,
         *,
         code: ErrorCode = ErrorCode.incompatible_call,
         node: Optional[ast.AST] = None,
         detail: Optional[str] = ...,
+        replacement: Optional[Replacement] = None,
     ) -> None:
         if node is None:
             node = self.node
         if node is None:
             return
-        self.visitor.show_error(node, message, code, detail=detail)
+        self.visitor.show_error(
+            node, message, code, detail=detail, replacement=replacement
+        )
 
 
 @dataclass
 class ActualArguments:
     """Represents the actual arguments to a call.
 
     Before creating this class, we decompose ``*args`` and ``**kwargs`` arguments
@@ -240,14 +259,16 @@
 
     This returns data that is useful for overload resolution.
 
     """
 
     return_value: Value
     """The return value of the function."""
+    sig: "Signature"
+    """Signature that was used for this call."""
     is_error: bool = False
     """Whether there was an error in this call. Used only for overload resolutioon."""
     used_any_for_match: bool = False
     """Whether Any was used for this match. Used only for overload resolution."""
     remaining_arguments: Optional[ActualArguments] = None
     """Arguments that still need to be processed. Used only for overload resolution."""
 
@@ -518,14 +539,16 @@
     is_asynq: bool = False
     """Whether this signature represents an asynq function."""
     has_return_annotation: bool = True
     allow_call: bool = False
     """Whether type checking can call the actual function to retrieve a precise return value."""
     evaluator: Optional[Evaluator] = None
     """Type evaluator for this function."""
+    deprecated: Optional[str] = None
+    """Deprecation message for this callable."""
     typevars_of_params: Dict[str, List[TypeVarLike]] = field(
         init=False, default_factory=dict, repr=False, compare=False, hash=False
     )
     all_typevars: Set[TypeVarLike] = field(
         init=False, default_factory=set, repr=False, compare=False, hash=False
     )
 
@@ -631,16 +654,18 @@
                     if is_overload:
                         triple = decompose_union(
                             param_typ, composite.value, ctx.can_assign_ctx
                         )
                         if triple is not None:
                             return triple
                     ctx.on_error(
-                        f"Incompatible argument type for {param.name}: expected"
-                        f" {param_typ} but got {composite.value}",
+                        (
+                            f"Incompatible argument type for {param.name}: expected"
+                            f" {param_typ} but got {composite.value}"
+                        ),
                         code=bounds_map.get_error_code()
                         or ErrorCode.incompatible_argument,
                         node=composite.node if composite.node is not None else None,
                         detail=str(bounds_map),
                     )
                     return None, False, None
             return bounds_map, used_any, None
@@ -763,30 +788,34 @@
         param_spec_consumed = False
 
         for param in self.parameters.values():
             if param.kind is ParameterKind.POSITIONAL_ONLY:
                 if positional_index < len(actual_args.positionals):
                     if positional_index in actual_args.pos_or_keyword_params:
                         self.show_call_error(
-                            f"Positional parameter {positional_index} should be"
-                            " positional-or-keyword",
+                            (
+                                f"Positional parameter {positional_index} should be"
+                                " positional-or-keyword"
+                            ),
                             ctx,
                         )
                         return None
                     definitely_provided, composite = actual_args.positionals[
                         positional_index
                     ]
                     if (
                         not definitely_provided
                         and param.default is None
                         and not actual_args.ellipsis
                     ):
                         self.show_call_error(
-                            f"Parameter '{param.name}' may not be provided by this"
-                            " call",
+                            (
+                                f"Parameter '{param.name}' may not be provided by this"
+                                " call"
+                            ),
                             ctx,
                         )
                         return None
                     bound_args[param.name] = (positional_index, composite)
                     positional_index += 1
                 elif actual_args.star_args is not None:
                     if param.default is None:
@@ -816,36 +845,42 @@
                     ]
                     if (
                         not definitely_provided
                         and param.default is None
                         and not actual_args.ellipsis
                     ):
                         self.show_call_error(
-                            f"Parameter '{param.name}' may not be provided by this"
-                            " call",
+                            (
+                                f"Parameter '{param.name}' may not be provided by this"
+                                " call"
+                            ),
                             ctx,
                         )
                         return None
                     bound_args[param.name] = (positional_index, composite)
                     positional_index += 1
                     if param.name in actual_args.keywords:
                         if param.name in actual_args.pos_or_keyword_params:
                             keywords_consumed.add(param.name)
                         else:
                             self.show_call_error(
-                                f"Parameter '{param.name}' provided as both a"
-                                " positional and a keyword argument",
+                                (
+                                    f"Parameter '{param.name}' provided as both a"
+                                    " positional and a keyword argument"
+                                ),
                                 ctx,
                             )
                             return None
                 elif actual_args.star_args is not None:
                     if param.name in actual_args.keywords:
                         self.show_call_error(
-                            f"Parameter '{param.name}' may be filled from both *args"
-                            " and a keyword argument",
+                            (
+                                f"Parameter '{param.name}' may be filled from both"
+                                " *args and a keyword argument"
+                            ),
                             ctx,
                         )
                         return None
                     star_args_consumed = True
                     if param.default is None:
                         position = ARGS
                     else:
@@ -864,16 +899,18 @@
                     definitely_provided, composite = actual_args.keywords[param.name]
                     if (
                         not definitely_provided
                         and param.default is None
                         and not actual_args.ellipsis
                     ):
                         self.show_call_error(
-                            f"Parameter '{param.name}' may not be provided by this"
-                            " call",
+                            (
+                                f"Parameter '{param.name}' may not be provided by this"
+                                " call"
+                            ),
                             ctx,
                         )
                         return None
                     bound_args[param.name] = param.name, composite
                     keywords_consumed.add(param.name)
                 elif actual_args.star_kwargs is not None:
                     if param.default is None:
@@ -893,28 +930,32 @@
                         f"Missing required argument '{param.name}'", ctx
                     )
                     return None
             elif param.kind is ParameterKind.KEYWORD_ONLY:
                 if param.name in actual_args.keywords:
                     if param.name in actual_args.pos_or_keyword_params:
                         self.show_call_error(
-                            f"Keyword parameter {param.name} should be"
-                            " positional-or-keyword",
+                            (
+                                f"Keyword parameter {param.name} should be"
+                                " positional-or-keyword"
+                            ),
                             ctx,
                         )
                         return None
                     definitely_provided, composite = actual_args.keywords[param.name]
                     if (
                         not definitely_provided
                         and param.default is None
                         and not actual_args.ellipsis
                     ):
                         self.show_call_error(
-                            f"Parameter '{param.name}' may not be provided by this"
-                            " call",
+                            (
+                                f"Parameter '{param.name}' may not be provided by this"
+                                " call"
+                            ),
                             ctx,
                         )
                         return None
                     bound_args[param.name] = param.name, composite
                     keywords_consumed.add(param.name)
                 elif actual_args.star_kwargs is not None:
                     if param.default is None:
@@ -1024,16 +1065,18 @@
                     self.show_call_error("Callable requires a ParamSpec argument", ctx)
                     return None
             else:
                 assert False, f"unhandled param {param.kind}"
 
         if not star_args_consumed and positional_index != len(actual_args.positionals):
             self.show_call_error(
-                f"Takes {positional_index} positional arguments but"
-                f" {len(actual_args.positionals)} were given",
+                (
+                    f"Takes {positional_index} positional arguments but"
+                    f" {len(actual_args.positionals)} were given"
+                ),
                 ctx,
             )
             return None
         if not star_kwargs_consumed:
             extra_kwargs = set(actual_args.keywords) - keywords_consumed
             if extra_kwargs:
                 extra_kwargs_str = ", ".join(map(repr, extra_kwargs))
@@ -1070,15 +1113,15 @@
         ctx.on_error(message, node=node, detail=detail)
 
     def get_default_return(self, source: AnySource = AnySource.error) -> CallReturn:
         return_value = self.return_value
         if self._return_key in self.typevars_of_params:
             typevar_values = {tv: AnyValue(source) for tv in self.all_typevars}
             return_value = return_value.substitute_typevars(typevar_values)
-        return CallReturn(return_value, is_error=True)
+        return CallReturn(return_value, is_error=True, sig=self)
 
     def check_call(
         self,
         args: Iterable[Argument],
         visitor: "NameCheckVisitor",
         node: Optional[ast.AST],
     ) -> Value:
@@ -1089,26 +1132,76 @@
 
         """
         args = list(args)
         ctx = _VisitorBasedContext(visitor, node)
         preprocessed = preprocess_args(args, ctx)
         if preprocessed is None:
             return self.get_default_return().return_value
-        return self.check_call_preprocessed(preprocessed, ctx).return_value
+        return self.check_call_preprocessed(
+            preprocessed, ctx, original_args=args, node=node
+        ).return_value
+
+    def maybe_show_too_many_pos_args_error(
+        self,
+        *,
+        args: Sequence[Argument],
+        bound_args: BoundArgs,
+        ctx: CheckCallContext,
+        node: ast.Call,
+    ) -> None:
+        """Show an error if the call to this Signature has too many positional arguments.
+        """
+        if ctx.visitor is None:
+            return
+        if len(node.args) < ctx.visitor.options.get_value_for(MaximumPositionalArgs):
+            return
+        composite_to_name = {}
+        for name, (kind, composite) in bound_args.items():
+            if isinstance(kind, int):
+                composite_to_name[composite] = name
+        node_to_composite = {}
+        for unbound_arg, kind in args:
+            if kind is None and unbound_arg.node is not None:
+                node_to_composite[unbound_arg.node] = unbound_arg
+
+        new_args = []
+        new_keywords = []
+        for arg in node.args:
+            if arg not in node_to_composite:
+                return
+            composite = node_to_composite[arg]
+            if composite not in composite_to_name:
+                return
+            name = composite_to_name[composite]
+            new_keywords.append(ast.keyword(arg=name, value=arg))
+        new_keywords += node.keywords
+        new_node = ast.Call(func=node.func, args=new_args, keywords=new_keywords)
+        ctx.visitor.show_error(
+            node,
+            f"Too many positional arguments for {stringify_object(self.callable)}",
+            error_code=ErrorCode.too_many_positional_args,
+            replacement=ctx.visitor.replace_node(node, new_node),
+        )
 
     def check_call_preprocessed(
         self,
         preprocessed: ActualArguments,
         ctx: CheckCallContext,
         *,
         is_overload: bool = False,
+        original_args: Optional[Sequence[Argument]] = None,
+        node: Optional[ast.AST] = None,
     ) -> CallReturn:
         bound_args = self.bind_arguments(preprocessed, ctx)
         if bound_args is None:
             return self.get_default_return()
+        if original_args is not None and isinstance(node, ast.Call):
+            self.maybe_show_too_many_pos_args_error(
+                args=original_args, bound_args=bound_args, ctx=ctx, node=node
+            )
         return self.check_call_with_bound_args(
             preprocessed, bound_args, ctx, is_overload=is_overload
         )
 
     def check_call_with_bound_args(
         self,
         preprocessed: ActualArguments,
@@ -1239,14 +1332,15 @@
                     return_value = runtime_return
         ret = self._apply_annotated_constraints(return_value, composites)
         return CallReturn(
             ret,
             is_error=had_error,
             used_any_for_match=used_any,
             remaining_arguments=new_args,
+            sig=self,
         )
 
     def _maybe_perform_call(
         self, actual_args: ActualArguments, ctx: CheckCallContext
     ) -> Optional[Value]:
         if self.callable is None or not callable(self.callable):
             return None
@@ -1376,16 +1470,18 @@
                             f"positional-only param {my_param.name!r} has no default"
                         )
 
                     their_annotation = their_params[i].get_annotation()
                     tv_map = their_annotation.can_assign(my_annotation, ctx)
                     if isinstance(tv_map, CanAssignError):
                         return CanAssignError(
-                            f"type of positional-only parameter {my_param.name!r} is"
-                            " incompatible",
+                            (
+                                "type of positional-only parameter"
+                                f" {my_param.name!r} is incompatible"
+                            ),
                             [tv_map],
                         )
                     tv_maps.append(tv_map)
                     consumed_positional.add(their_params[i].name)
                 elif args_annotation is not None:
                     new_tv_maps = can_assign_var_positional(
                         my_param, args_annotation, i - their_args_index, ctx
@@ -1491,16 +1587,18 @@
                         ParameterKind.POSITIONAL_OR_KEYWORD,
                     )
                 ]
                 for extra_param in extra_positional:
                     tv_map = extra_param.get_annotation().can_assign(my_annotation, ctx)
                     if isinstance(tv_map, CanAssignError):
                         return CanAssignError(
-                            f"type of param {extra_param.name!r} is incompatible with "
-                            "*args type",
+                            (
+                                f"type of param {extra_param.name!r} is incompatible"
+                                " with *args type"
+                            ),
                             [tv_map],
                         )
                     tv_maps.append(tv_map)
             elif my_param.kind is ParameterKind.VAR_KEYWORD:
                 if kwargs_annotation is None:
                     return CanAssignError("**kwargs are not accepted")
                 tv_map = kwargs_annotation.can_assign(my_annotation, ctx)
@@ -1514,16 +1612,18 @@
                     and param.kind
                     in (ParameterKind.KEYWORD_ONLY, ParameterKind.POSITIONAL_OR_KEYWORD)
                 ]
                 for extra_param in extra_keyword:
                     tv_map = extra_param.get_annotation().can_assign(my_annotation, ctx)
                     if isinstance(tv_map, CanAssignError):
                         return CanAssignError(
-                            f"type of param {extra_param.name!r} is incompatible with "
-                            "**kwargs type",
+                            (
+                                f"type of param {extra_param.name!r} is incompatible"
+                                " with **kwargs type"
+                            ),
                             [tv_map],
                         )
                     tv_maps.append(tv_map)
             elif my_param.kind is ParameterKind.PARAM_SPEC:
                 remaining = [
                     param
                     for param in other.parameters.values()
@@ -1677,14 +1777,15 @@
         *,
         impl: Optional[Impl] = None,
         callable: Optional[object] = None,
         has_return_annotation: bool = True,
         is_asynq: bool = False,
         allow_call: bool = False,
         evaluator: Optional[Evaluator] = None,
+        deprecated: Optional[str] = None,
     ) -> "Signature":
         """Create a :class:`Signature` object.
 
         This is more convenient to use than the constructor
         because it abstracts away the creation of the underlying
         :class:`inspect.Signature`.
 
@@ -1716,26 +1817,39 @@
                     param_dict[name] = SigParameter(
                         name,
                         ParameterKind.KEYWORD_ONLY,
                         annotation=value,
                         default=None if is_required else AnyValue(AnySource.marker),
                     )
                     i += 1
+                if param.annotation.extra_keys is not None:
+                    name = f"%kwargs{i}"
+                    param_dict[name] = SigParameter(
+                        name,
+                        ParameterKind.VAR_KEYWORD,
+                        annotation=GenericValue(
+                            dict, [TypedValue(str), param.annotation.extra_keys]
+                        ),
+                    )
+                    i += 1
             else:
                 param_dict[param.name] = param
                 i += 1
+        if deprecated is None and callable is not None:
+            deprecated = safe_getattr(callable, "__deprecated__", None)
         return cls(
             param_dict,
             return_value=return_annotation,
             impl=impl,
             callable=callable,
             has_return_annotation=has_return_annotation,
             is_asynq=is_asynq,
             allow_call=allow_call,
             evaluator=evaluator,
+            deprecated=deprecated,
         )
 
     def __str__(self) -> str:
         param_str = ", ".join(self._render_parameters())
         asynq_str = "@asynq " if self.is_asynq else ""
         rendered = f"{asynq_str}({param_str}) -> {self.return_value}"
         if self.impl:
@@ -2196,21 +2310,30 @@
                 else:
                     union_rets.append(ret)
                 actual_args = ret.remaining_arguments
             elif ret.used_any_for_match:
                 any_rets.append(ret)
             else:
                 # We got a clean match!
-                return self._unite_rets(any_rets, union_and_any_rets, union_rets, ret)
+                return self._unite_rets(
+                    any_rets,
+                    union_and_any_rets,
+                    union_rets,
+                    ret,
+                    visitor=visitor,
+                    node=node,
+                )
 
         if any_rets:
             # We don't do this if we have union_rets, because if we got here, we
             # didn't get any clean matches. Therefore, we must have some remaining
             # union members we haven't handled.
-            return self._unite_rets(any_rets, union_and_any_rets, union_rets)
+            return self._unite_rets(
+                any_rets, union_and_any_rets, union_rets, visitor=visitor, node=node
+            )
 
         # None of the signatures matched
         errors = list(itertools.chain.from_iterable(errors_per_overload))
         codes = {error["error_code"] for error in errors}
         if len(codes) == 1:
             (error_code,) = codes
         else:
@@ -2223,33 +2346,45 @@
 
     def _unite_rets(
         self,
         any_rets: Sequence[CallReturn],
         union_and_any_rets: Sequence[CallReturn],
         union_rets: Sequence[CallReturn],
         clean_ret: Optional[CallReturn] = None,
+        *,
+        visitor: "NameCheckVisitor",
+        node: Optional[ast.AST],
     ) -> Value:
         if any_rets or union_and_any_rets:
             deduped = {ret.return_value for ret in any_rets}
             if (
                 len(deduped) == 1
                 and not union_rets
                 and not union_and_any_rets
                 and clean_ret is None
             ):
-                return any_rets[0].return_value
-            return AnyValue(AnySource.multiple_overload_matches)
+                rets = any_rets
+            else:
+                return AnyValue(AnySource.multiple_overload_matches)
         elif union_rets:
             if clean_ret is not None:
                 rets = [*union_rets, clean_ret]
             else:
                 rets = union_rets
-            return unite_values(*[r.return_value for r in rets])
-        assert clean_ret is not None
-        return clean_ret.return_value
+        else:
+            assert clean_ret is not None
+            rets = [clean_ret]
+        for ret in rets:
+            if ret.sig.deprecated is not None:
+                visitor.show_error(
+                    node,
+                    f"Use of deprecated overload {ret.sig}: {ret.sig.deprecated}",
+                    ErrorCode.deprecated,
+                )
+        return unite_values(*[r.return_value for r in rets])
 
     def _make_detail(
         self,
         errors_per_overload: Sequence[Sequence[Dict[str, Any]]],
         sigs: Sequence[Signature],
     ) -> CanAssignError:
         details = []
@@ -2403,16 +2538,14 @@
         if return_override is None:
             return_override = argspec.return_override
         return BoundMethodSignature(argspec.signature, self_composite, return_override)
     else:
         assert_never(argspec)
 
 
-T = TypeVar("T")
-IterableValue = GenericValue(collections.abc.Iterable, [TypeVarValue(T)])
 K = TypeVar("K")
 V = TypeVar("V")
 MappingValue = GenericValue(collections.abc.Mapping, [TypeVarValue(K), TypeVarValue(V)])
 
 
 def can_assign_var_positional(
     my_param: SigParameter, args_annotation: Value, idx: int, ctx: CanAssignContext
@@ -2427,29 +2560,34 @@
                     f"parameter {my_param.name!r} is not accepted;"
                     f" {args_annotation} only accepts {length} values"
                 )
             their_annotation = members[idx]
             can_assign = their_annotation.can_assign(my_annotation, ctx)
             if isinstance(can_assign, CanAssignError):
                 return CanAssignError(
-                    f"type of parameter {my_param.name!r} is incompatible: *args[{idx}]"
-                    " type is incompatible",
+                    (
+                        f"type of parameter {my_param.name!r} is incompatible:"
+                        f" *args[{idx}] type is incompatible"
+                    ),
                     [can_assign],
                 )
             return [can_assign]
 
-    tv_map = get_tv_map(IterableValue, args_annotation, ctx)
-    if isinstance(tv_map, CanAssignError):
-        return CanAssignError(f"{args_annotation} is not an iterable type", [tv_map])
-    iterable_arg = tv_map.get(T, AnyValue(AnySource.generic_argument))
+    iterable_arg = is_iterable(args_annotation, ctx)
+    if isinstance(iterable_arg, CanAssignError):
+        return CanAssignError(
+            f"{args_annotation} is not an iterable type", [iterable_arg]
+        )
     bounds_map = iterable_arg.can_assign(my_annotation, ctx)
     if isinstance(bounds_map, CanAssignError):
         return CanAssignError(
-            f"type of parameter {my_param.name!r} is incompatible: "
-            "*args type is incompatible",
+            (
+                f"type of parameter {my_param.name!r} is incompatible: "
+                "*args type is incompatible"
+            ),
             [bounds_map],
         )
     return [bounds_map]
 
 
 def can_assign_var_keyword(
     my_param: SigParameter, kwargs_annotation: Value, ctx: CanAssignContext
@@ -2461,16 +2599,18 @@
             return CanAssignError(
                 f"parameter {my_param.name!r} is not accepted by {kwargs_annotation}"
             )
         their_annotation = kwargs_annotation.items[my_param.name][1]
         can_assign = their_annotation.can_assign(my_annotation, ctx)
         if isinstance(can_assign, CanAssignError):
             return CanAssignError(
-                f"type of parameter {my_param.name!r} is incompatible:"
-                f" *kwargs[{my_param.name!r}] type is incompatible",
+                (
+                    f"type of parameter {my_param.name!r} is incompatible:"
+                    f" *kwargs[{my_param.name!r}] type is incompatible"
+                ),
                 [can_assign],
             )
         bounds_maps.append(can_assign)
     else:
         mapping_tv_map = get_tv_map(MappingValue, kwargs_annotation, ctx)
         if isinstance(mapping_tv_map, CanAssignError):
             return CanAssignError(
@@ -2484,16 +2624,18 @@
                 [can_assign],
             )
         bounds_maps.append(can_assign)
         value_arg = mapping_tv_map.get(V, AnyValue(AnySource.generic_argument))
         can_assign = value_arg.can_assign(my_annotation, ctx)
         if isinstance(can_assign, CanAssignError):
             return CanAssignError(
-                f"type of parameter {my_param.name!r} is incompatible: **kwargs type"
-                " is incompatible",
+                (
+                    f"type of parameter {my_param.name!r} is incompatible: **kwargs"
+                    " type is incompatible"
+                ),
                 [can_assign],
             )
         bounds_maps.append(can_assign)
     return bounds_maps
 
 
 def decompose_union(
```

### Comparing `pyanalyze-0.8.0/pyanalyze/stacked_scopes.py` & `pyanalyze-0.9.0/pyanalyze/stacked_scopes.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/stubs/_pyanalyze_tests-stubs/initnew.pyi` & `pyanalyze-0.9.0/pyanalyze/stubs/_pyanalyze_tests-stubs/initnew.pyi`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/stubs/pyanalyze-stubs/extensions.pyi` & `pyanalyze-0.9.0/pyanalyze/stubs/pyanalyze-stubs/extensions.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 def overload(func: Callable[..., Any]) -> Callable[..., Any]: ...
 def evaluated(func: Callable[..., Any]) -> Callable[..., Any]: ...
 def is_provided(arg: Any) -> bool: ...
 def is_positional(arg: Any) -> bool: ...
 def is_keyword(arg: Any) -> bool: ...
 def is_of_type(arg: Any, type: Any, *, exclude_any: bool = ...) -> bool: ...
 def show_error(message: str, *, argument: Optional[Any] = ...) -> bool: ...
+def deprecated(__message: str) -> Callable[..., Any]: ...
 def __getattr__(self, __arg: str) -> Any: ...
```

### Comparing `pyanalyze-0.8.0/pyanalyze/suggested_type.py` & `pyanalyze-0.9.0/pyanalyze/suggested_type.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_analysis_lib.py` & `pyanalyze-0.9.0/pyanalyze/test_analysis_lib.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_annotations.py` & `pyanalyze-0.9.0/pyanalyze/test_annotations.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,15 @@
             assert_is_value(Capybara(), TypedValue(Capybara))
             assert_is_value(mara(), KnownValue(None))
 
     @assert_passes()
     def test_annotations_function(self):
         def caviidae() -> None:
             x = int
+
             # tests that annotations in a nested functions are not evaluated in a context where
             # they don't exist
             def capybara(a: x, *b: x, c: x, d: x = 3, **kwargs: x):
                 pass
 
             capybara(1, c=1)
             capybara(1, c="x")  # E: incompatible_argument
@@ -362,29 +363,70 @@
             assert_is_value(z, t_str_int)
             assert_is_value(omega, t_str_int | KnownValue(None))
             assert_is_value(empty, SequenceValue(tuple, []))
 
     @skip_before((3, 9))
     @assert_passes()
     def test_builtin_tuples(self):
+        from collections.abc import Iterable
         from typing import Union
 
+        def returner() -> Iterable[tuple[str, int]]:
+            yield ("a", 1)
+
         def capybara(
             x: tuple[int, ...],
             y: tuple[int],
             z: tuple[str, int],
             omega: Union[tuple[str, int], None],
             empty: tuple[()],
+            kappa: Iterable[tuple[str, int]],
         ) -> None:
             assert_is_value(x, GenericValue(tuple, [TypedValue(int)]))
             assert_is_value(y, make_simple_sequence(tuple, [TypedValue(int)]))
             t_str_int = make_simple_sequence(tuple, [TypedValue(str), TypedValue(int)])
             assert_is_value(z, t_str_int)
             assert_is_value(omega, t_str_int | KnownValue(None))
             assert_is_value(empty, SequenceValue(tuple, []))
+            for t in kappa:
+                assert_is_value(t, t_str_int)
+            for elt in returner():
+                assert_is_value(elt, t_str_int)
+
+    @skip_before((3, 9))
+    def test_builtin_tuples_string(self):
+        self.assert_passes(
+            """
+            from __future__ import annotations
+            from collections.abc import Iterable
+            from typing import Union
+
+            def returner() -> Iterable[tuple[str, int]]:
+                yield ("a", 1)
+
+            def capybara(
+                x: tuple[int, ...],
+                y: tuple[int],
+                z: tuple[str, int],
+                omega: Union[tuple[str, int], None],
+                empty: tuple[()],
+                kappa: Iterable[tuple[str, int]],
+            ) -> None:
+                assert_is_value(x, GenericValue(tuple, [TypedValue(int)]))
+                assert_is_value(y, make_simple_sequence(tuple, [TypedValue(int)]))
+                t_str_int = make_simple_sequence(tuple, [TypedValue(str), TypedValue(int)])
+                assert_is_value(z, t_str_int)
+                assert_is_value(omega, t_str_int | KnownValue(None))
+                assert_is_value(empty, SequenceValue(tuple, []))
+                for t in kappa:
+                    assert_is_value(t, t_str_int)
+                for elt in returner():
+                    assert_is_value(elt, t_str_int)
+            """
+        )
 
     @assert_passes()
     def test_invalid_annotation(self):
         def not_an_annotation(x: 1):  # E: invalid_annotation
             pass
 
         def forward_ref_undefined(x: "NoSuchType"):  # E: undefined_name
@@ -509,14 +551,32 @@
         self.assert_passes(
             """
             from __future__ import annotations
 
             def capybara(x: int | None, y: int | str) -> None:
                 assert_is_value(x, MultiValuedValue([TypedValue(int), KnownValue(None)]))
                 assert_is_value(y, MultiValuedValue([TypedValue(int), TypedValue(str)]))
+
+            def caller():
+                capybara(1, 2)
+                capybara(None, "x")
+            """
+        )
+
+    @skip_before((3, 10))
+    def test_pep604_runtime(self):
+        self.assert_passes(
+            """
+            def capybara(x: int | None, y: int | str) -> None:
+                assert_is_value(x, MultiValuedValue([TypedValue(int), KnownValue(None)]))
+                assert_is_value(y, MultiValuedValue([TypedValue(int), TypedValue(str)]))
+
+            def caller():
+                capybara(1, 2)
+                capybara(None, "x")
             """
         )
 
     @assert_passes()
     def test_stringified_ops(self):
         from typing_extensions import Literal
```

### Comparing `pyanalyze-0.8.0/pyanalyze/test_arg_spec.py` & `pyanalyze-0.9.0/pyanalyze/test_arg_spec.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_ast_annotator.py` & `pyanalyze-0.9.0/pyanalyze/test_ast_annotator.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_async_await.py` & `pyanalyze-0.9.0/pyanalyze/test_async_await.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_asynq.py` & `pyanalyze-0.9.0/pyanalyze/test_asynq.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_asynq_checker.py` & `pyanalyze-0.9.0/pyanalyze/test_asynq_checker.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_attributes.py` & `pyanalyze-0.9.0/pyanalyze/test_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,16 @@
             assert_is_value(Unhashable().prop, AnyValue(AnySource.inference))
 
     @assert_passes()
     def test_tuple_subclass_with_getattr(self):
         # Inspired by pyspark.sql.types.Row
         class Row(tuple):
             def __getattr__(self, attr):
+                if attr.startswith("__"):
+                    raise AttributeError(attr)
                 return attr.upper()
 
         def capybara():
             x = Row()
             return x.capybaras
 
     @assert_passes()
@@ -360,7 +362,19 @@
             def types(cls):
                 return []
 
         def capybara(x: X) -> None:
             cls = X
             if hasattr(cls, "types"):  # E: value_always_true
                 assert_is_value(cls.types(), AnyValue(AnySource.unannotated))
+
+
+class TestClassAttributeTransformer(TestNameCheckVisitorBase):
+    @assert_passes()
+    def test(self):
+        from pyanalyze.test_config import StringField
+
+        class Capybara:
+            foo = StringField()
+
+        def capybara(c: Capybara):
+            assert_is_value(c.foo, TypedValue(str))
```

### Comparing `pyanalyze-0.8.0/pyanalyze/test_boolability.py` & `pyanalyze-0.9.0/pyanalyze/test_boolability.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_config.py` & `pyanalyze-0.9.0/pyanalyze/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 
 Configuration file specific to tests.
 
 """
 from pathlib import Path
-from typing import Dict, Optional
+from typing import Dict, Optional, Tuple
 
 from . import tests, value
 from .arg_spec import ArgSpecCache
 from .error_code import ErrorCode, register_error_code
 from .find_unused import used
 
 from .options import Options
@@ -108,9 +108,23 @@
         and issubclass(cls, tests.Wrapper)
         and cls is not tests.Wrapper
     ):
         return cls.base
     return cls
 
 
+class StringField:
+    pass
+
+
+@used  # in test.toml
+def transform_class_attribute(
+    attr: object,
+) -> Optional[Tuple[value.Value, value.Value]]:
+    """Transforms a StringField attribute."""
+    if isinstance(attr, StringField):
+        return value.TypedValue(str), value.NO_RETURN_VALUE
+    return None
+
+
 CONFIG_PATH = Path(__file__).parent / "test.toml"
 TEST_OPTIONS = Options.from_option_list(config_file_path=CONFIG_PATH)
```

### Comparing `pyanalyze-0.8.0/pyanalyze/test_enum.py` & `pyanalyze-0.9.0/pyanalyze/test_enum.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_extensions.py` & `pyanalyze-0.9.0/pyanalyze/test_extensions.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_format_strings.py` & `pyanalyze-0.9.0/pyanalyze/test_format_strings.py`

 * *Files 12% similar despite different names*

```diff
@@ -474,7 +474,34 @@
         def capybara(x):
             "foo %f" % x
 
     @assert_passes()
     def test_complicated_expression(self):
         def capybara(x):
             "foo %s" % len(x)
+
+
+class TestFStringLiteral(TestNameCheckVisitorBase):
+    @assert_passes()
+    def test_basic(self):
+        from typing_extensions import Literal, assert_type
+
+        def capybara(a: Literal["a"], ab: Literal["a", "b"]):
+            assert_type(f"a{a}", Literal["aa"])
+            assert_type(f"a{ab}", Literal["aa", "ab"])
+            assert_type(f"a{ab}b{ab}", Literal["aaba", "aabb", "abba", "abbb"])
+            # Make sure we don't infer a 2**16-size union
+            assert_type(
+                f"{ab}{ab}{ab}{ab}{ab}{ab}{ab}{ab}{ab}{ab}{ab}{ab}{ab}{ab}{ab}{ab}", str
+            )
+
+    @assert_passes()
+    def test_conversions(self):
+        from typing_extensions import Literal, assert_type
+
+        def capybara(a: Literal["á"], ab: Literal["á", "ê"]):
+            assert_type(f"a{a!r}", Literal["a'á'"])
+            assert_type(f"a{ab!r}", Literal["a'á'", "a'ê'"])
+            assert_type(f"a{a!s}", Literal["aá"])
+            assert_type(f"a{ab!s}", Literal["aá", "aê"])
+            assert_type(f"a{a!a}", Literal["a'\\xe1'"])
+            assert_type(f"a{ab!a}", Literal["a'\\xe1'", "a'\\xea'"])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyanalyze-0.8.0/pyanalyze/test_functions.py` & `pyanalyze-0.9.0/pyanalyze/test_functions.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_generators.py` & `pyanalyze-0.9.0/pyanalyze/test_generators.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_implementation.py` & `pyanalyze-0.9.0/pyanalyze/test_implementation.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_inference_helpers.py` & `pyanalyze-0.9.0/pyanalyze/test_inference_helpers.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_literal_string.py` & `pyanalyze-0.9.0/pyanalyze/test_literal_string.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_name_check_visitor.py` & `pyanalyze-0.9.0/pyanalyze/test_name_check_visitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,18 +288,15 @@
             pass
 
         def run():
             print(cavy.call_count)
 
     @assert_passes()
     def test_mock_attr(self):
-        try:
-            from unittest import mock
-        except ImportError:
-            import mock
+        from unittest import mock
 
         class X:
             a = mock.MagicMock()
 
         class Y:
             def __init__(self):
                 self.x = X()
@@ -1744,83 +1741,14 @@
 
     @assert_passes()
     def test_undefined_name(self):
         def capybara():
             return f"{x}"  # E: undefined_name
 
 
-class TestTypedDict(TestNameCheckVisitorBase):
-    @assert_passes()
-    def test_basic(self):
-        from mypy_extensions import TypedDict as METypedDict
-        from typing_extensions import TypedDict as TETypedDict
-
-        T = METypedDict("T", {"a": int, "b": str})
-        T2 = TETypedDict("T2", {"a": int, "b": str})
-
-        def capybara(x: T, y: T2):
-            assert_is_value(
-                x,
-                TypedDictValue(
-                    {"a": (True, TypedValue(int)), "b": (True, TypedValue(str))}
-                ),
-            )
-            assert_is_value(x["a"], TypedValue(int))
-            assert_is_value(
-                y,
-                TypedDictValue(
-                    {"a": (True, TypedValue(int)), "b": (True, TypedValue(str))}
-                ),
-            )
-            assert_is_value(y["a"], TypedValue(int))
-
-    @assert_passes()
-    def test_unknown_key_unresolved(self):
-        from mypy_extensions import TypedDict
-
-        T = TypedDict("T", {"a": int, "b": str})
-
-        def capybara(x: T):
-            assert_is_value(x["not a key"], AnyValue(AnySource.inference))
-
-    @assert_passes()
-    def test_invalid_key(self):
-        from mypy_extensions import TypedDict
-
-        T = TypedDict("T", {"a": int, "b": str})
-
-        def capybara(x: T):
-            x[0]  # E: invalid_typeddict_key
-
-    @assert_passes()
-    def test_total(self):
-        from typing_extensions import TypedDict
-
-        class TD(TypedDict, total=False):
-            a: int
-            b: str
-
-        class TD2(TD):
-            c: float
-
-        def f(td: TD) -> None:
-            pass
-
-        def g(td2: TD2) -> None:
-            pass
-
-        def caller() -> None:
-            f({})
-            f({"a": 1})
-            f({"a": 1, "b": "c"})
-            f({"a": "a"})  # E: incompatible_argument
-            g({"c": 1.0})
-            g({})  # E: incompatible_argument
-
-
 _AnnotSettings = {
     ErrorCode.missing_parameter_annotation: True,
     ErrorCode.missing_return_annotation: True,
 }
 
 
 class TestRequireAnnotations(TestNameCheckVisitorBase):
```

### Comparing `pyanalyze-0.8.0/pyanalyze/test_never.py` & `pyanalyze-0.9.0/pyanalyze/test_never.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_node_visitor.py` & `pyanalyze-0.9.0/pyanalyze/test_node_visitor.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_operations.py` & `pyanalyze-0.9.0/pyanalyze/test_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -228,14 +228,35 @@
             i < s  # E: unsupported_operation
             s >= f  # E: unsupported_operation
             # TODO: These don't throw errors because None.__lt__ exists at runtime.
             s > None
             s > os
 
     @assert_passes()
+    def test_contains(self):
+        from typing import Iterator, Iterable
+
+        class OnlyGetitem:
+            def __getitem__(self, x: int) -> int:
+                return x
+
+        class OnlyIter:
+            def __iter__(self) -> Iterator[int]:
+                yield 1
+
+        def capybara(x: int, ogi: OnlyGetitem, oi: OnlyIter, it: Iterable[int]):
+            1 in x  # E: unsupported_operation
+            1 in ogi
+            "x" in ogi  # E: incompatible_argument
+            1 in oi
+            "1" in oi  # E: incompatible_argument
+            1 in it
+            "1" in it  # E: incompatible_argument
+
+    @assert_passes()
     def test_failing_eq(self):
         class FlakyCapybara:
             def __eq__(self, other: object) -> bool:
                 raise IndentationError
 
         fc = FlakyCapybara()
```

### Comparing `pyanalyze-0.8.0/pyanalyze/test_patma.py` & `pyanalyze-0.9.0/pyanalyze/test_patma.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_pep673.py` & `pyanalyze-0.9.0/pyanalyze/test_pep673.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_signature.py` & `pyanalyze-0.9.0/pyanalyze/test_signature.py`

 * *Files 2% similar despite different names*

```diff
@@ -431,16 +431,18 @@
     @assert_passes()
     def test_error_location(self):
         def two_args(x: str, y: int) -> None:
             pass
 
         def capybara():
             two_args(
-                "one very long string so long that it goes on its own line is this"
-                " enough",
+                (
+                    "one very long string so long that it goes on its own line is this"
+                    " enough"
+                ),
                 "not an int",  # E: incompatible_argument
             )
 
     @assert_passes()
     def test_too_few_args(self):
         def fn(x, y):
             return x + y
@@ -906,15 +908,15 @@
         def capybara():
             assert_is_value(overloaded(), TypedValue(int))
             assert_is_value(overloaded("x"), TypedValue(str))
             overloaded(1)  # E: incompatible_argument
             overloaded("x", "y")  # E: incompatible_call
 
     @assert_passes()
-    def test_runtime(self):
+    def test_pyanalyze_extensions(self):
         from typing import Union
 
         from pyanalyze.extensions import overload
 
         @overload
         def overloaded() -> int:
             raise NotImplementedError
@@ -930,15 +932,43 @@
                 return args[0]
             else:
                 raise TypeError("too many arguments")
 
         def capybara():
             assert_is_value(overloaded(), TypedValue(int))
             assert_is_value(overloaded("x"), TypedValue(str))
-            overloaded(1)  # E: incompatible_call
+            overloaded(1)  # E: incompatible_argument
+            overloaded("a", "b")  # E: incompatible_call
+
+    @assert_passes()
+    def test_typing_extensions(self):
+        from typing import Union
+
+        from typing_extensions import overload
+
+        @overload
+        def overloaded() -> int:
+            raise NotImplementedError
+
+        @overload
+        def overloaded(x: str) -> str:
+            raise NotImplementedError
+
+        def overloaded(*args: str) -> Union[int, str]:
+            if not args:
+                return 0
+            elif len(args) == 1:
+                return args[0]
+            else:
+                raise TypeError("too many arguments")
+
+        def capybara():
+            assert_is_value(overloaded(), TypedValue(int))
+            assert_is_value(overloaded("x"), TypedValue(str))
+            overloaded(1)  # E: incompatible_argument
             overloaded("a", "b")  # E: incompatible_call
 
     @assert_passes()
     def test_list_any(self):
         from typing import Any, List, Union
 
         from typing_extensions import Literal
@@ -1242,7 +1272,47 @@
         from typing_extensions import Unpack
 
         def unpack_that_int(*args: Unpack[int]) -> None:  # E: invalid_annotation
             assert_is_value(args, AnyValue(AnySource.error))
 
         def bad_kwargs(**kwargs: Unpack[None]) -> None:  # E: invalid_annotation
             assert_is_value(kwargs, AnyValue(AnySource.error))
+
+
+class TestTooManyPosArgs(TestNameCheckVisitorBase):
+    def test_basic(self):
+        self.assert_is_changed(
+            """
+            def f(a, b, c, d, e, f, g, h, i, j, k):
+                pass
+
+            def capybara():
+                f(1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11)
+            """,
+            """
+            def f(a, b, c, d, e, f, g, h, i, j, k):
+                pass
+
+            def capybara():
+                f(a=1, b=2, c=3, d=4, e=5, f=6, g=7, h=8, i=9, j=10, k=11)
+            """,
+        )
+
+    def test_method(self):
+        self.assert_is_changed(
+            """
+            class X:
+                def f(self, a, b, c, d, e, f, g, h, i, j, k):
+                    pass
+
+            def capybara(x: X):
+                x.f(1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11)
+            """,
+            """
+            class X:
+                def f(self, a, b, c, d, e, f, g, h, i, j, k):
+                    pass
+
+            def capybara(x: X):
+                x.f(a=1, b=2, c=3, d=4, e=5, f=6, g=7, h=8, i=9, j=10, k=11)
+            """,
+        )
```

### Comparing `pyanalyze-0.8.0/pyanalyze/test_stacked_scopes.py` & `pyanalyze-0.9.0/pyanalyze/test_stacked_scopes.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,21 +18,21 @@
     SequenceValue,
     TypedValue,
     UNINITIALIZED_VALUE,
 )
 
 
 # just used for its __dict__
-class Module(object):
+class Module:
     foo = 1
     bar = None
 
 
-class TestStackedScopes(object):
-    def setup(self):
+class TestStackedScopes:
+    def setup_method(self):
         self.scopes = build_stacked_scopes(Module)
 
     def test_scope_type(self):
         assert ScopeType.module_scope == self.scopes.scope_type()
 
         with self.scopes.add_scope(ScopeType.function_scope, scope_node=None):
             assert ScopeType.function_scope == self.scopes.scope_type()
```

### Comparing `pyanalyze-0.8.0/pyanalyze/test_suggested_type.py` & `pyanalyze-0.9.0/pyanalyze/test_suggested_type.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_thrift_enum.py` & `pyanalyze-0.9.0/pyanalyze/test_thrift_enum.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_type_evaluation.py` & `pyanalyze-0.9.0/pyanalyze/test_type_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_type_object.py` & `pyanalyze-0.9.0/pyanalyze/test_type_object.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_typeshed.py` & `pyanalyze-0.9.0/pyanalyze/test_typeshed.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,15 @@
 
 
 class GenericChild(Parent[T]):
     pass
 
 
 class TestGetGenericBases:
-    def setup(self) -> None:
+    def setup_method(self) -> None:
         checker = Checker()
         self.get_generic_bases = checker.arg_spec_cache.get_generic_bases
 
     def test_runtime(self):
         assert {
             Parent: {T: AnyValue(AnySource.generic_argument)}
         } == self.get_generic_bases(Parent)
```

### Comparing `pyanalyze-0.8.0/pyanalyze/test_typevar.py` & `pyanalyze-0.9.0/pyanalyze/test_typevar.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_value.py` & `pyanalyze-0.9.0/pyanalyze/test_value.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/test_yield_checker.py` & `pyanalyze-0.9.0/pyanalyze/test_yield_checker.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/tests.py` & `pyanalyze-0.9.0/pyanalyze/tests.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/type_evaluation.py` & `pyanalyze-0.9.0/pyanalyze/type_evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -500,16 +500,18 @@
             if mod == KnownValue(sys):
                 if node.left.attr == "platform":
                     left_operand = sys.platform
                 elif node.left.attr == "version_info":
                     left_operand = sys.version_info
                 else:
                     return self.return_invalid(
-                        "Only comparisons on sys.platform and sys.version_info are"
-                        " supported",
+                        (
+                            "Only comparisons on sys.platform and sys.version_info are"
+                            " supported"
+                        ),
                         node.left,
                     )
                 data = _OP_TO_DATA[type(op)]
                 try:
                     result = data.impl(left_operand, right_operand.val)
                 except Exception:
                     return self.return_invalid(
```

### Comparing `pyanalyze-0.8.0/pyanalyze/type_object.py` & `pyanalyze-0.9.0/pyanalyze/type_object.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/typeshed.py` & `pyanalyze-0.9.0/pyanalyze/typeshed.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,21 +35,27 @@
 from typing_extensions import Protocol, TypedDict
 
 from pyanalyze.functions import translate_vararg_type
 from .analysis_lib import is_positional_only_arg_name
 from .annotations import (
     Context,
     make_type_var_value,
+    DecoratorValue,
     Pep655Value,
     SyntheticEvaluator,
     type_from_value,
     value_from_ast,
 )
 from .error_code import ErrorCode
-from .extensions import evaluated, overload, real_overload
+from .extensions import (
+    evaluated,
+    overload,
+    real_overload,
+    deprecated as deprecated_decorator,
+)
 from .node_visitor import Failure
 from .options import Options, PathSequenceOption
 from .safe import all_of_type, hasattr_static, is_typing_name, safe_isinstance
 from .signature import (
     ConcreteSignature,
     make_bound_method,
     OverloadedSignature,
@@ -59,14 +65,17 @@
 )
 from .stacked_scopes import Composite, uniq_chain
 from .value import (
     AnySource,
     AnyValue,
     CallableValue,
     CanAssignContext,
+    DeprecatedExtension,
+    Extension,
+    annotate_value,
     extract_typevars,
     GenericValue,
     KnownValue,
     make_coro_type,
     SubclassValue,
     TypedDictValue,
     TypedValue,
@@ -791,14 +800,15 @@
         mod: str,
         objclass: Optional[type] = None,
         *,
         autobind: bool = False,
         allow_call: bool = False,
     ) -> Optional[Signature]:
         is_classmethod = is_staticmethod = is_evaluated = False
+        deprecated = None
         for decorator_ast in node.decorator_list:
             decorator = self._parse_expr(decorator_ast, mod)
             if (
                 decorator == KnownValue(abstractmethod)
                 or decorator == KnownValue(overload)
                 or decorator == KnownValue(real_overload)
             ):
@@ -810,16 +820,22 @@
             elif decorator == KnownValue(staticmethod):
                 is_staticmethod = True
                 if autobind:  # TODO support staticmethods otherwise
                     continue
             elif decorator == KnownValue(evaluated):
                 is_evaluated = True
                 continue
-            # might be @overload or something else we don't recognize
-            return None
+            elif (
+                isinstance(decorator, DecoratorValue)
+                and decorator.decorator is deprecated_decorator
+            ):
+                arg = decorator.args[0]
+                if isinstance(arg, KnownValue) and isinstance(arg.val, str):
+                    deprecated = arg.val
+            # something we don't recognize; ignore it
         if node.returns is None:
             return_value = AnyValue(AnySource.unannotated)
         else:
             return_value = self._parse_type(node.returns, mod)
         # ignore self type for class and static methods
         if node.decorator_list:
             objclass = None
@@ -872,14 +888,15 @@
             cleaned_arguments,
             callable=obj,
             return_annotation=make_coro_type(return_value)
             if isinstance(node, ast.AsyncFunctionDef)
             else return_value,
             allow_call=allow_call,
             evaluator=evaluator,
+            deprecated=deprecated,
         )
 
     def _parse_param_list(
         self,
         args: Iterable[ast.arg],
         defaults: Iterable[Optional[ast.AST]],
         module: str,
@@ -978,26 +995,46 @@
         if not isinstance(info.ast, ast.Assign) or not isinstance(
             info.ast.value, ast.Call
         ):
             return AnyValue(AnySource.inference)
         ctx = _AnnotationContext(finder=self, module=module)
         return value_from_ast(info.ast.value, ctx=ctx)
 
+    def _extract_metadata(self, module: str, node: ast.ClassDef) -> Sequence[Extension]:
+        metadata = []
+        for decorator in node.decorator_list:
+            decorator_val = self._parse_expr(decorator, module)
+            if (
+                isinstance(decorator_val, DecoratorValue)
+                and decorator_val.decorator is deprecated_decorator
+            ):
+                arg = decorator_val.args[0]
+                if isinstance(arg, KnownValue) and isinstance(arg.val, str):
+                    metadata.append(DeprecatedExtension(arg.val))
+        return metadata
+
     def make_synthetic_type(self, module: str, info: typeshed_client.NameInfo) -> Value:
         fq_name = f"{module}.{info.name}"
         bases = self._get_bases_from_info(info, module, fq_name)
         typ = TypedValue(fq_name)
+        if isinstance(info.ast, ast.ClassDef):
+            metadata = self._extract_metadata(module, info.ast)
+        else:
+            metadata = []
         if bases is not None:
             if any(
                 (isinstance(base, KnownValue) and is_typing_name(base.val, "TypedDict"))
                 or isinstance(base, TypedDictValue)
                 for base in bases
             ):
                 typ = self._make_typeddict(module, info, bases)
-        return SubclassValue(typ, exactly=True)
+        val = SubclassValue(typ, exactly=True)
+        if metadata:
+            return annotate_value(val, metadata)
+        return val
 
     def _make_typeddict(
         self, module: str, info: typeshed_client.NameInfo, bases: Sequence[Value]
     ) -> TypedDictValue:
         total = True
         if isinstance(info.ast, ast.ClassDef):
             for keyword in info.ast.keywords:
@@ -1030,15 +1067,16 @@
         else:
             return (total, field)
 
     def _value_from_info(
         self, info: typeshed_client.resolver.ResolvedName, module: str
     ) -> Value:
         # This guard against infinite recursion if a type refers to itself
-        # (real-world example: os._ScandirIterator).
+        # (real-world example: os._ScandirIterator). Needs to change in
+        # order to support recursive types.
         if info in self._active_infos:
             return AnyValue(AnySource.inference)
         self._active_infos.append(info)
         try:
             return self._value_from_info_inner(info, module)
         finally:
             self._active_infos.pop()
```

### Comparing `pyanalyze-0.8.0/pyanalyze/typevar.py` & `pyanalyze-0.9.0/pyanalyze/typevar.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze/value.py` & `pyanalyze-0.9.0/pyanalyze/value.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,14 +355,16 @@
     """Marker object used internally."""
     incomplete_annotation = 11
     """A special form like ClassVar without a type argument."""
     multiple_overload_matches = 12
     """Multiple matching overloads."""
     ellipsis_callable = 13
     """Callable using an ellipsis."""
+    unresolved_import = 14
+    """An unresolved import."""
 
 
 @dataclass(frozen=True)
 class AnyValue(Value):
     """An unknown value, equivalent to ``typing.Any``."""
 
     source: AnySource
@@ -1143,22 +1145,35 @@
 class TypedDictValue(GenericValue):
     """Equivalent to ``typing.TypedDict``; a dictionary with a known set of string keys.
     """
 
     items: Dict[str, Tuple[bool, Value]]
     """The items of the ``TypedDict``. Required items are represented as (True, value) and optional
     ones as (False, value)."""
+    extra_keys: Optional[Value] = None
+    """The type of unknown keys, if any."""
 
-    def __init__(self, items: Dict[str, Tuple[bool, Value]]) -> None:
+    def __init__(
+        self, items: Dict[str, Tuple[bool, Value]], extra_keys: Optional[Value] = None
+    ) -> None:
+        value_types = []
         if items:
-            value_type = unite_values(*[val for _, val in items.values()])
-        else:
-            value_type = AnyValue(AnySource.unreachable)
-        super().__init__(dict, (TypedValue(str), value_type))
+            value_types += [val for _, val in items.values()]
+        if extra_keys is not None:
+            value_types.append(extra_keys)
+        value_type = (
+            unite_values(*value_types)
+            if value_types
+            else AnyValue(AnySource.unreachable)
+        )
+        # The key type must be str so dict[str, Any] is compatible with a TypedDict
+        key_type = TypedValue(str)
+        super().__init__(dict, (key_type, value_type))
         self.items = items
+        self.extra_keys = extra_keys
 
     def num_required_keys(self) -> int:
         return sum(1 for required, _ in self.items.values() if required)
 
     def all_keys_required(self) -> bool:
         return all(required for required, _ in self.items.values())
 
@@ -1189,14 +1204,22 @@
                     can_assign = value.can_assign(other.items[key][1], ctx)
                     if isinstance(can_assign, CanAssignError):
                         return CanAssignError(
                             f"Types for key {key} are incompatible",
                             children=[can_assign],
                         )
                     bounds_maps.append(can_assign)
+            # TODO: What if only one of the two has extra keys?
+            if self.extra_keys is not None and other.extra_keys is not None:
+                can_assign = self.extra_keys.can_assign(other.extra_keys, ctx)
+                if isinstance(can_assign, CanAssignError):
+                    return CanAssignError(
+                        "Types for extra keys are incompatible", children=[can_assign]
+                    )
+                bounds_maps.append(can_assign)
             return unify_bounds_maps(bounds_maps)
         elif isinstance(other, KnownValue) and isinstance(other.val, dict):
             bounds_maps = []
             for key, (is_required, value) in self.items.items():
                 if key not in other.val:
                     if is_required:
                         return CanAssignError(f"Key {key} is missing in {other}")
@@ -1212,15 +1235,18 @@
         return super().can_assign(other, ctx)
 
     def substitute_typevars(self, typevars: TypeVarMap) -> "TypedDictValue":
         return TypedDictValue(
             {
                 key: (is_required, value.substitute_typevars(typevars))
                 for key, (is_required, value) in self.items.items()
-            }
+            },
+            extra_keys=self.extra_keys.substitute_typevars(typevars)
+            if self.extra_keys is not None
+            else None,
         )
 
     def __str__(self) -> str:
         items = [
             f'"{key}": {value if required else "NotRequired[" + str(value) + "]"}'
             for key, (required, value) in self.items.items()
         ]
@@ -1896,14 +1922,26 @@
 
 @dataclass(frozen=True)
 class AssertErrorExtension(Extension):
     """Used for the implementation of :func:`pyanalyze.extensions.assert_error`."""
 
 
 @dataclass(frozen=True)
+class SkipDeprecatedExtension(Extension):
+    """Indicates that use of this value should not trigger deprecation errors."""
+
+
+@dataclass(frozen=True)
+class DeprecatedExtension(Extension):
+    """Indicates that use of this value should trigger a deprecation error."""
+
+    deprecation_message: str
+
+
+@dataclass(frozen=True)
 class AnnotatedValue(Value):
     """Value representing a `PEP 593 <https://www.python.org/dev/peps/pep-0593/>`_ Annotated object.
 
     Pyanalyze uses ``Annotated`` types to represent types with some extra
     information added to them in the form of :class:`Extension` objects.
 
     """
@@ -2284,30 +2322,35 @@
         return unite_values(*value_subvals, *chain.from_iterable(seq_subvals))
     if isinstance(value, SequenceValue):
         members = value.get_member_sequence()
         if members is None:
             return value.args[0]
         return members
     elif isinstance(value, TypedDictValue):
-        if all(required for required, _ in value.items.items()):
+        if value.extra_keys is None and all(
+            required for required, _ in value.items.items()
+        ):
             return [KnownValue(key) for key in value.items]
-        return MultiValuedValue([KnownValue(key) for key in value.items])
+        possibilities = [KnownValue(key) for key in value.items]
+        if value.extra_keys is not None:
+            possibilities.append(TypedValue(str))
+        return MultiValuedValue(possibilities)
     elif isinstance(value, DictIncompleteValue):
         if all(pair.is_required and not pair.is_many for pair in value.kv_pairs):
             return [pair.key for pair in value.kv_pairs]
     elif isinstance(value, KnownValue):
         if isinstance(value.val, (str, bytes, range)):
             if len(value.val) < ITERATION_LIMIT:
                 return [KnownValue(c) for c in value.val]
             is_nonempty = True
     elif value is NO_RETURN_VALUE:
         return NO_RETURN_VALUE
-    iter_tv_map = get_tv_map(IterableValue, value, ctx)
-    if not isinstance(iter_tv_map, CanAssignError):
-        val = iter_tv_map.get(T, AnyValue(AnySource.generic_argument))
+    iterable_type = is_iterable(value, ctx)
+    if isinstance(iterable_type, Value):
+        val = iterable_type
     else:
         getitem_tv_map = get_tv_map(GetItemProtoValue, value, ctx)
         if not isinstance(getitem_tv_map, CanAssignError):
             val = getitem_tv_map.get(T, AnyValue(AnySource.generic_argument))
         # Hack to support iteration over StrEnum. A better solution would have to
         # handle descriptors better in attribute assignment and Protocol compatibility.
         elif (
@@ -2316,15 +2359,15 @@
             and isinstance(value.typ.typ, type)
             and safe_issubclass(value.typ.typ, enum.Enum)
         ):
             return value.typ
         else:
             # We return the error from the __iter__ check because the __getitem__
             # check is more arcane.
-            return iter_tv_map
+            return iterable_type
     if is_nonempty:
         return annotate_value(val, [AlwaysPresentExtension()])
     return val
 
 
 K = TypeVar("K")
 V = TypeVar("V")
@@ -2367,18 +2410,28 @@
             return [
                 KVPair(pair.key, pair.value, pair.is_many, is_required=False)
                 for pair in pairs
             ]
     if isinstance(value_val, DictIncompleteValue):
         return value_val.kv_pairs
     elif isinstance(value_val, TypedDictValue):
-        return [
+        pairs = [
             KVPair(KnownValue(key), value, is_required=required)
             for key, (required, value) in value_val.items.items()
         ]
+        if value_val.extra_keys is not None:
+            pairs.append(
+                KVPair(
+                    TypedValue(str),
+                    value_val.extra_keys,
+                    is_many=True,
+                    is_required=False,
+                )
+            )
+        return pairs
     else:
         # Ideally we should only need to check ProtocolMappingValue, but if
         # we do that we can't infer the right types for dict, so try the
         # nominal Mapping first.
         can_assign = get_tv_map(NominalMappingValue, value_val, ctx)
         if isinstance(can_assign, CanAssignError):
             can_assign = get_tv_map(ProtocolMappingValue, value_val, ctx)
@@ -2486,19 +2539,26 @@
         if value.typ is tuple:
             return _unpack_sequence_value(value, target_length, post_starred_length)
         elif value.typ is list:
             vals = _unpack_sequence_value(value, target_length, post_starred_length)
             if not isinstance(vals, CanAssignError):
                 return vals
 
+    iterable_type = is_iterable(value, ctx)
+    if isinstance(iterable_type, CanAssignError):
+        return iterable_type
+    return _create_unpacked_list(iterable_type, target_length, post_starred_length)
+
+
+def is_iterable(value: Value, ctx: CanAssignContext) -> Union[CanAssignError, Value]:
+    """Check whether a value is iterable."""
     tv_map = get_tv_map(IterableValue, value, ctx)
     if isinstance(tv_map, CanAssignError):
         return tv_map
-    iterable_type = tv_map.get(T, AnyValue(AnySource.generic_argument))
-    return _create_unpacked_list(iterable_type, target_length, post_starred_length)
+    return tv_map.get(T, AnyValue(AnySource.generic_argument))
 
 
 def _create_unpacked_list(
     iterable_type: Value, target_length: int, post_starred_length: Optional[int]
 ) -> List[Value]:
     if post_starred_length is not None:
         return [
```

### Comparing `pyanalyze-0.8.0/pyanalyze/yield_checker.py` & `pyanalyze-0.9.0/pyanalyze/yield_checker.py`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/pyanalyze.egg-info/PKG-INFO` & `pyanalyze-0.9.0/pyanalyze.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyanalyze
-Version: 0.8.0
+Version: 0.9.0
 Summary: A static analyzer for Python
 Home-page: https://github.com/quora/pyanalyze
 Author: Quora, Inc.
 Author-email: jelle@quora.com
 License: Apache Software License
 Keywords: quora static analysis
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyanalyze-0.8.0/pyanalyze.egg-info/SOURCES.txt` & `pyanalyze-0.9.0/pyanalyze.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -37,34 +37,38 @@
 pyanalyze/test_ast_annotator.py
 pyanalyze/test_async_await.py
 pyanalyze/test_asynq.py
 pyanalyze/test_asynq_checker.py
 pyanalyze/test_attributes.py
 pyanalyze/test_boolability.py
 pyanalyze/test_config.py
+pyanalyze/test_deprecated.py
 pyanalyze/test_enum.py
 pyanalyze/test_error_code.py
 pyanalyze/test_extensions.py
 pyanalyze/test_format_strings.py
 pyanalyze/test_functions.py
 pyanalyze/test_generators.py
 pyanalyze/test_implementation.py
+pyanalyze/test_import.py
 pyanalyze/test_inference_helpers.py
 pyanalyze/test_literal_string.py
 pyanalyze/test_name_check_visitor.py
 pyanalyze/test_never.py
 pyanalyze/test_node_visitor.py
 pyanalyze/test_operations.py
 pyanalyze/test_patma.py
 pyanalyze/test_pep673.py
+pyanalyze/test_recursion.py
 pyanalyze/test_self.py
 pyanalyze/test_signature.py
 pyanalyze/test_stacked_scopes.py
 pyanalyze/test_suggested_type.py
 pyanalyze/test_thrift_enum.py
+pyanalyze/test_try.py
 pyanalyze/test_type_evaluation.py
 pyanalyze/test_type_object.py
 pyanalyze/test_typeddict.py
 pyanalyze/test_typeshed.py
 pyanalyze/test_typevar.py
 pyanalyze/test_value.py
 pyanalyze/test_yield_checker.py
@@ -80,14 +84,15 @@
 pyanalyze.egg-info/dependency_links.txt
 pyanalyze.egg-info/entry_points.txt
 pyanalyze.egg-info/requires.txt
 pyanalyze.egg-info/top_level.txt
 pyanalyze/stubs/_pyanalyze_tests-stubs/aliases.pyi
 pyanalyze/stubs/_pyanalyze_tests-stubs/args.pyi
 pyanalyze/stubs/_pyanalyze_tests-stubs/contextmanager.pyi
+pyanalyze/stubs/_pyanalyze_tests-stubs/deprecated.pyi
 pyanalyze/stubs/_pyanalyze_tests-stubs/evaluated.pyi
 pyanalyze/stubs/_pyanalyze_tests-stubs/initnew.pyi
 pyanalyze/stubs/_pyanalyze_tests-stubs/overloaded.pyi
 pyanalyze/stubs/_pyanalyze_tests-stubs/recursion.pyi
 pyanalyze/stubs/_pyanalyze_tests-stubs/self.pyi
 pyanalyze/stubs/_pyanalyze_tests-stubs/typeddict.pyi
 pyanalyze/stubs/pyanalyze-stubs/extensions.pyi
```

### Comparing `pyanalyze-0.8.0/pyproject.toml` & `pyanalyze-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyanalyze-0.8.0/setup.py` & `pyanalyze-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from setuptools import setup
 
 
-version = "0.8.0"
+version = "0.9.0"
 package_data = ["test.toml", "stubs/*/*.pyi"]
 
 
 if __name__ == "__main__":
     setup(
         name="pyanalyze",
         version=version,
@@ -31,15 +31,15 @@
         packages=["pyanalyze"],
         install_requires=[
             "asynq",
             "qcore>=0.5.1",
             "ast_decompiler>=0.4.0",
             "typeshed_client>=2.1.0",
             "typing_inspect>=0.7.0",
-            "typing_extensions>=4.0.0",
+            "typing_extensions>=4.1.0",
             "aenum>=2.2.3",
             "codemod",
             "tomli>=1.1.0",
         ],
         # These are useful for unit tests of pyanalyze extensions
         # outside the package.
         package_data={"pyanalyze": package_data},
```

