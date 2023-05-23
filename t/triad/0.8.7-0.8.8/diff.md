# Comparing `tmp/triad-0.8.7.tar.gz` & `tmp/triad-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triad-0.8.7.tar", last modified: Thu May  4 06:59:47 2023, max compression
+gzip compressed data, was "triad-0.8.8.tar", last modified: Tue May 23 06:36:43 2023, max compression
```

## Comparing `triad-0.8.7.tar` & `triad-0.8.8.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:47.371417 triad-0.8.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-04 06:59:09.000000 triad-0.8.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-05-04 06:59:47.371417 triad-0.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-04 06:59:09.000000 triad-0.8.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-04 06:59:47.371417 triad-0.8.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-04 06:59:09.000000 triad-0.8.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:47.367417 triad-0.8.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:09.000000 triad-0.8.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:47.367417 triad-0.8.7/tests/collections/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 06:59:09.000000 triad-0.8.7/tests/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-04 06:59:09.000000 triad-0.8.7/tests/collections/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-05-04 06:59:09.000000 triad-0.8.7/tests/collections/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-04 06:59:09.000000 triad-0.8.7/tests/collections/test_function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-05-04 06:59:09.000000 triad-0.8.7/tests/collections/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:47.367417 triad-0.8.7/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/convert_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:47.367417 triad-0.8.7/tests/utils/dispatcher_examples/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/dispatcher_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/dispatcher_examples/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/dispatcher_examples/invalid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_class_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_pandas_like.py
--rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_pyarrow_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_threading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:47.367417 triad-0.8.7/triad/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-04 06:59:09.000000 triad-0.8.7/triad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:47.371417 triad-0.8.7/triad/collections/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-04 06:59:09.000000 triad-0.8.7/triad/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-05-04 06:59:09.000000 triad-0.8.7/triad/collections/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-04 06:59:09.000000 triad-0.8.7/triad/collections/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11058 2023-05-04 06:59:09.000000 triad-0.8.7/triad/collections/function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-05-04 06:59:09.000000 triad-0.8.7/triad/collections/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-04 06:59:09.000000 triad-0.8.7/triad/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-04 06:59:09.000000 triad-0.8.7/triad/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:47.371417 triad-0.8.7/triad/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/class_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    17472 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/pandas_like.py
--rw-r--r--   0 runner    (1001) docker     (123)    24206 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:47.371417 triad-0.8.7/triad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-05-04 06:59:47.000000 triad-0.8.7/triad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-04 06:59:47.000000 triad-0.8.7/triad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 06:59:47.000000 triad-0.8.7/triad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-04 06:59:47.000000 triad-0.8.7/triad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 06:59:47.000000 triad-0.8.7/triad.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:47.371417 triad-0.8.7/triad_version/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-04 06:59:09.000000 triad-0.8.7/triad_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:43.625054 triad-0.8.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-23 06:36:03.000000 triad-0.8.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-23 06:36:43.625054 triad-0.8.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-23 06:36:03.000000 triad-0.8.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-23 06:36:43.625054 triad-0.8.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-23 06:36:03.000000 triad-0.8.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:43.621054 triad-0.8.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:03.000000 triad-0.8.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:43.621054 triad-0.8.8/tests/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 06:36:03.000000 triad-0.8.8/tests/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-23 06:36:03.000000 triad-0.8.8/tests/collections/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-05-23 06:36:03.000000 triad-0.8.8/tests/collections/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-23 06:36:03.000000 triad-0.8.8/tests/collections/test_function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-05-23 06:36:03.000000 triad-0.8.8/tests/collections/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:43.621054 triad-0.8.8/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/convert_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:43.621054 triad-0.8.8/tests/utils/dispatcher_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/dispatcher_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/dispatcher_examples/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/dispatcher_examples/invalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_class_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_pandas_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21182 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_pyarrow_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-23 06:36:03.000000 triad-0.8.8/tests/utils/test_threading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:43.625054 triad-0.8.8/triad/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-23 06:36:03.000000 triad-0.8.8/triad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:43.625054 triad-0.8.8/triad/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 06:36:03.000000 triad-0.8.8/triad/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-05-23 06:36:03.000000 triad-0.8.8/triad/collections/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-23 06:36:03.000000 triad-0.8.8/triad/collections/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11058 2023-05-23 06:36:03.000000 triad-0.8.8/triad/collections/function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-05-23 06:36:03.000000 triad-0.8.8/triad/collections/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-23 06:36:03.000000 triad-0.8.8/triad/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-23 06:36:03.000000 triad-0.8.8/triad/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:43.625054 triad-0.8.8/triad/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/class_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17472 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/pandas_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29571 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-23 06:36:03.000000 triad-0.8.8/triad/utils/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:43.625054 triad-0.8.8/triad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-23 06:36:43.000000 triad-0.8.8/triad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-23 06:36:43.000000 triad-0.8.8/triad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:36:43.000000 triad-0.8.8/triad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 06:36:43.000000 triad-0.8.8/triad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-23 06:36:43.000000 triad-0.8.8/triad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:36:43.625054 triad-0.8.8/triad_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 06:36:03.000000 triad-0.8.8/triad_version/__init__.py
```

### Comparing `triad-0.8.7/LICENSE` & `triad-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/PKG-INFO` & `triad-0.8.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triad
-Version: 0.8.7
+Version: 0.8.8
 Summary: A collection of python utils for Fugue projects
 Home-page: http://github.com/fugue-project/triad
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Triad
         
@@ -24,14 +24,18 @@
         ```bash
         pip install triad
         ```
         
         
         ## Release History
         
+        ### 0.8.8
+        
+        * Add type replacement utils for pyarrow
+        
         ### 0.8.7
         
         * Fix pandas 2.0 warnings
         
         ### 0.8.6
         
         * Fixed timestamp conversion for pandas 2.0
```

### Comparing `triad-0.8.7/README.md` & `triad-0.8.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 ```bash
 pip install triad
 ```
 
 
 ## Release History
 
+### 0.8.8
+
+* Add type replacement utils for pyarrow
+
 ### 0.8.7
 
 * Fix pandas 2.0 warnings
 
 ### 0.8.6
 
 * Fixed timestamp conversion for pandas 2.0
```

### Comparing `triad-0.8.7/setup.py` & `triad-0.8.8/setup.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/tests/collections/test_dict.py` & `triad-0.8.8/tests/collections/test_dict.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/tests/collections/test_fs.py` & `triad-0.8.8/tests/collections/test_fs.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/tests/collections/test_function_wrapper.py` & `triad-0.8.8/tests/collections/test_function_wrapper.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/tests/collections/test_schema.py` & `triad-0.8.8/tests/collections/test_schema.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/tests/utils/test_assertion.py` & `triad-0.8.8/tests/utils/test_assertion.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/tests/utils/test_class_extension.py` & `triad-0.8.8/tests/utils/test_class_extension.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/tests/utils/test_convert.py` & `triad-0.8.8/tests/utils/test_convert.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/tests/utils/test_dispatcher.py` & `triad-0.8.8/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/tests/utils/test_hash.py` & `triad-0.8.8/tests/utils/test_hash.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/tests/utils/test_iter.py` & `triad-0.8.8/tests/utils/test_iter.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/tests/utils/test_pandas_like.py` & `triad-0.8.8/tests/utils/test_pandas_like.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/tests/utils/test_pyarrow_convert.py` & `triad-0.8.8/tests/utils/test_pyarrow_convert.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/tests/utils/test_rename.py` & `triad-0.8.8/tests/utils/test_rename.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/tests/utils/test_schema.py` & `triad-0.8.8/tests/utils/test_schema.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/tests/utils/test_string.py` & `triad-0.8.8/tests/utils/test_string.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/tests/utils/test_threading.py` & `triad-0.8.8/tests/utils/test_threading.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/triad/collections/dict.py` & `triad-0.8.8/triad/collections/dict.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/triad/collections/fs.py` & `triad-0.8.8/triad/collections/fs.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/triad/collections/function_wrapper.py` & `triad-0.8.8/triad/collections/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/triad/collections/schema.py` & `triad-0.8.8/triad/collections/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,14 +197,16 @@
             is_supported(value.type), SchemaError(f"{value} is not supported")
         )
         super().__setitem__(name, value, *args, **kwds)  # type: ignore
 
     def __eq__(self, other: Any) -> bool:
         if other is None:
             return False
+        if other is self:
+            return True
         if isinstance(other, Schema):
             return super().__eq__(other)
         if isinstance(other, str):
             return self.__repr__() == other
         return self == Schema(other)
 
     def __contains__(self, key: Any) -> bool:  # noqa: C901
```

### Comparing `triad-0.8.7/triad/utils/assertion.py` & `triad-0.8.8/triad/utils/assertion.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/triad/utils/class_extension.py` & `triad-0.8.8/triad/utils/class_extension.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/triad/utils/convert.py` & `triad-0.8.8/triad/utils/convert.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/triad/utils/dispatcher.py` & `triad-0.8.8/triad/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/triad/utils/entry_points.py` & `triad-0.8.8/triad/utils/entry_points.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/triad/utils/hash.py` & `triad-0.8.8/triad/utils/hash.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/triad/utils/iter.py` & `triad-0.8.8/triad/utils/iter.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/triad/utils/json.py` & `triad-0.8.8/triad/utils/json.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/triad/utils/pandas_like.py` & `triad-0.8.8/triad/utils/pandas_like.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/triad/utils/pyarrow.py` & `triad-0.8.8/triad/utils/pyarrow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import pickle
 from datetime import date, datetime
 from functools import partial
-from typing import Any, Callable, Dict, Iterable, List, Optional, Set, Tuple
+from typing import Any, Callable, Dict, Iterable, List, Optional, Set, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 from pandas.core.dtypes.base import ExtensionDtype
 
 from triad.constants import TRIAD_VAR_QUOTE
@@ -15,14 +15,21 @@
 from .iter import EmptyAwareIterable, Slicer
 from .json import loads_no_dup
 from .schema import move_to_unquoted, quote_name, unquote_name
 
 TRIAD_DEFAULT_TIMESTAMP_UNIT = "us"
 TRIAD_DEFAULT_TIMESTAMP = pa.timestamp(TRIAD_DEFAULT_TIMESTAMP_UNIT)
 
+LARGE_TYPES_REPLACEMENT: List[Tuple[Any, Any]] = [
+    (pa.large_string(), pa.string()),
+    (pa.large_binary(), pa.binary()),
+    (pa.large_utf8(), pa.utf8()),
+    (pa.types.is_large_list, lambda t: pa.list_(t.value_field)),
+]
+
 _TYPE_EXPRESSION_MAPPING: Dict[str, pa.DataType] = {
     "null": pa.null(),
     "str": pa.string(),
     "string": pa.string(),
     "bool": pa.bool_(),
     "boolean": pa.bool_(),
     "int8": pa.int8(),
@@ -282,25 +289,177 @@
         return pa.Table.from_arrays(cols, names=names)
 
     if same:
         return lambda x: x
     return partial(_alter, params=params)
 
 
+def replace_types_in_table(
+    df: pa.Table,
+    pairs: List[
+        Tuple[
+            Union[Callable[[pa.DataType], bool], pa.DataType],
+            Union[Callable[[pa.DataType], pa.DataType], pa.DataType],
+        ]
+    ],
+    recursive: bool = True,
+    safe: bool = True,
+) -> pa.Table:
+    """Replace(cast) types in a table
+
+    :param df: the table
+    :param pairs: a list of (is_type, convert_type) pairs
+    :param recursive: whether to do recursive replacement in nested types
+    :param safe: whether to check for conversion errors such as overflow
+
+    :return: the new table
+    """
+    old_schema = df.schema
+    new_schema = replace_types_in_schema(old_schema, pairs, recursive)
+    if old_schema is new_schema:
+        return df
+    func = get_alter_func(old_schema, new_schema, safe=safe)
+    return func(df)
+
+
+def replace_types_in_schema(
+    schema: pa.Schema,
+    pairs: List[
+        Tuple[
+            Union[Callable[[pa.DataType], bool], pa.DataType],
+            Union[Callable[[pa.DataType], pa.DataType], pa.DataType],
+        ]
+    ],
+    recursive: bool = True,
+) -> pa.Schema:
+    """Replace types in a schema
+
+    :param schema: the schema
+    :param pairs: a list of (is_type, convert_type) pairs
+    :param recursive: whether to do recursive replacement in nested types
+    :return: the new schema
+    """
+    fields = []
+    changed = False
+    for f in schema:
+        new_type = f.type
+        for is_type, convert_type in pairs:
+            _is_type = is_type if callable(is_type) else lambda t: t == is_type  # noqa
+            _convert_type = (
+                convert_type
+                if callable(convert_type)
+                else lambda t: convert_type  # noqa
+            )
+            new_type = replace_type(
+                new_type, _is_type, _convert_type, recursive=recursive
+            )
+        if f.type is new_type or f.type == new_type:
+            fields.append(f)
+        else:
+            changed = True
+            fields.append(pa.field(f.name, new_type))
+    if not changed:
+        return schema
+    return pa.schema(fields)
+
+
+def replace_type(  # noqa: C901
+    current_type: pa.DataType,
+    is_type: Callable[[pa.DataType], bool],
+    convert_type: Callable[[pa.DataType], pa.DataType],
+    recursive: bool = True,
+) -> pa.DataType:
+    """Replace ``current_type`` or if it is nested, replace in the nested
+    types
+
+    :param current_type: the current type
+    :param is_type: the function to check if the type is the type to replace
+    :param convert_type: the function to convert the type
+    :param recursive: whether to do recursive replacement in nested types
+    :return: the new type
+    """
+    if not pa.types.is_nested(current_type) and is_type(current_type):
+        return convert_type(current_type)
+    if recursive:
+        if pa.types.is_struct(current_type):
+            old_fields = list(current_type)
+            fields = [
+                _replace_field(f, is_type, convert_type, recursive=recursive)
+                for f in old_fields
+            ]
+            if all(a is b for a, b in zip(fields, old_fields)):
+                return current_type
+            return pa.struct(fields)
+        if pa.types.is_list(current_type) or pa.types.is_large_list(current_type):
+            old_f = current_type.value_field
+            f = _replace_field(old_f, is_type, convert_type, recursive=recursive)
+            if f is old_f:
+                res = current_type
+            elif pa.types.is_large_list(current_type):
+                res = pa.large_list(f)
+            else:
+                res = pa.list_(f)
+            if is_type(res):
+                return convert_type(res)
+            return res
+        if pa.types.is_map(current_type):
+            old_k, old_v = current_type.key_field, current_type.item_field
+            k, v = _replace_field(
+                old_k, is_type, convert_type, recursive=recursive
+            ), _replace_field(old_v, is_type, convert_type, recursive=recursive)
+            if k is old_k and v is old_v:
+                return current_type
+            return pa.map_(k, v)
+    return current_type
+
+
+def _replace_field(
+    field: pa.Field,
+    is_type: Callable[[pa.DataType], bool],
+    convert_type: Callable[[pa.DataType], pa.DataType],
+    recursive: bool,
+):
+    old_type = field.type
+    new_type = replace_type(old_type, is_type, convert_type, recursive=recursive)
+    if old_type is new_type or old_type == new_type:
+        return field
+    return pa.field(
+        field.name, new_type, nullable=field.nullable, metadata=field.metadata
+    )
+
+
 def schemas_equal(
-    a: pa.Schema, b: pa.Schema, check_order: bool = True, check_metadata: bool = True
+    a: pa.Schema,
+    b: pa.Schema,
+    check_order: bool = True,
+    check_metadata: bool = True,
+    ignore: Optional[
+        List[
+            Tuple[
+                Union[Callable[[pa.DataType], bool], pa.DataType],
+                Union[Callable[[pa.DataType], pa.DataType], pa.DataType],
+            ]
+        ]
+    ] = None,
 ) -> bool:
     """check if two schemas are equal
 
     :param a: first pyarrow schema
     :param b: second pyarrow schema
     :param compare_order: whether to compare order
     :param compare_order: whether to compare metadata
+    :param ignore: a list of (is_type, convert_type) pairs to
+        ignore differences on, defaults to None
     :return: if the two schema equal
     """
+    if a is b:
+        return True
+    if ignore is not None:
+        a = replace_types_in_schema(a, ignore, recursive=True)
+        b = replace_types_in_schema(b, ignore, recursive=True)
     if check_order:
         return a.equals(b, check_metadata=check_metadata)
     if check_metadata and a.metadata != b.metadata:
         return False
     da = {k: a.field(k) for k in a.names}
     db = {k: b.field(k) for k in b.names}
     return da == db
```

### Comparing `triad-0.8.7/triad/utils/rename.py` & `triad-0.8.8/triad/utils/rename.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/triad/utils/schema.py` & `triad-0.8.8/triad/utils/schema.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/triad/utils/string.py` & `triad-0.8.8/triad/utils/string.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/triad/utils/threading.py` & `triad-0.8.8/triad/utils/threading.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.7/triad.egg-info/PKG-INFO` & `triad-0.8.8/triad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triad
-Version: 0.8.7
+Version: 0.8.8
 Summary: A collection of python utils for Fugue projects
 Home-page: http://github.com/fugue-project/triad
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Triad
         
@@ -24,14 +24,18 @@
         ```bash
         pip install triad
         ```
         
         
         ## Release History
         
+        ### 0.8.8
+        
+        * Add type replacement utils for pyarrow
+        
         ### 0.8.7
         
         * Fix pandas 2.0 warnings
         
         ### 0.8.6
         
         * Fixed timestamp conversion for pandas 2.0
```

### Comparing `triad-0.8.7/triad.egg-info/SOURCES.txt` & `triad-0.8.8/triad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

