# Comparing `tmp/python_json_log_formatter-3.0.2.tar.gz` & `tmp/python_json_log_formatter-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_json_log_formatter-3.0.2.tar", last modified: Sat Jan 21 16:29:27 2023, max compression
+gzip compressed data, was "python_json_log_formatter-3.2.0.tar", last modified: Tue May 23 12:59:55 2023, max compression
```

## Comparing `python_json_log_formatter-3.0.2.tar` & `python_json_log_formatter-3.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-01-21 16:29:27.163790 python_json_log_formatter-3.0.2/
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)    11358 2022-11-24 16:19:23.000000 python_json_log_formatter-3.0.2/LICENSE
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)     3044 2023-01-21 16:29:27.163611 python_json_log_formatter-3.0.2/PKG-INFO
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)     2413 2022-11-28 21:08:13.000000 python_json_log_formatter-3.0.2/README.md
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)      941 2022-12-13 12:36:44.000000 python_json_log_formatter-3.0.2/pyproject.toml
-drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-01-21 16:29:27.162587 python_json_log_formatter-3.0.2/python_json_log_formatter/
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)     1110 2022-12-15 13:46:18.000000 python_json_log_formatter-3.0.2/python_json_log_formatter/__init__.py
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)       92 2022-12-13 12:36:44.000000 python_json_log_formatter-3.0.2/python_json_log_formatter/__init__.pyi
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)     7690 2023-01-21 16:27:05.000000 python_json_log_formatter-3.0.2/python_json_log_formatter/context_filter.py
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)      273 2022-12-13 12:36:44.000000 python_json_log_formatter-3.0.2/python_json_log_formatter/context_filter.pyi
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)        0 2022-12-13 12:36:44.000000 python_json_log_formatter-3.0.2/python_json_log_formatter/py.typed
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)     3808 2023-01-21 16:28:45.000000 python_json_log_formatter-3.0.2/python_json_log_formatter/python_json_log_formatter.py
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)      319 2022-12-13 12:36:44.000000 python_json_log_formatter-3.0.2/python_json_log_formatter/python_json_log_formatter.pyi
-drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-01-21 16:29:27.163395 python_json_log_formatter-3.0.2/python_json_log_formatter.egg-info/
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)     3044 2023-01-21 16:29:27.000000 python_json_log_formatter-3.0.2/python_json_log_formatter.egg-info/PKG-INFO
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)      540 2023-01-21 16:29:27.000000 python_json_log_formatter-3.0.2/python_json_log_formatter.egg-info/SOURCES.txt
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)        1 2023-01-21 16:29:27.000000 python_json_log_formatter-3.0.2/python_json_log_formatter.egg-info/dependency_links.txt
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)       26 2023-01-21 16:29:27.000000 python_json_log_formatter-3.0.2/python_json_log_formatter.egg-info/top_level.txt
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)       38 2023-01-21 16:29:27.163836 python_json_log_formatter-3.0.2/setup.cfg
+drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-05-23 12:59:55.490592 python_json_log_formatter-3.2.0/
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)    11358 2022-11-24 16:19:23.000000 python_json_log_formatter-3.2.0/LICENSE
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)     3400 2023-05-23 12:59:55.490423 python_json_log_formatter-3.2.0/PKG-INFO
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)     2769 2023-05-23 12:59:38.000000 python_json_log_formatter-3.2.0/README.md
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)      941 2022-12-13 12:36:44.000000 python_json_log_formatter-3.2.0/pyproject.toml
+drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-05-23 12:59:55.489254 python_json_log_formatter-3.2.0/python_json_log_formatter/
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)     1110 2022-12-15 13:46:18.000000 python_json_log_formatter-3.2.0/python_json_log_formatter/__init__.py
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)       92 2022-12-13 12:36:44.000000 python_json_log_formatter-3.2.0/python_json_log_formatter/__init__.pyi
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)    11953 2023-05-23 12:59:38.000000 python_json_log_formatter-3.2.0/python_json_log_formatter/context_filter.py
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)      553 2023-05-23 12:59:38.000000 python_json_log_formatter-3.2.0/python_json_log_formatter/context_filter.pyi
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)        0 2022-12-13 12:36:44.000000 python_json_log_formatter-3.2.0/python_json_log_formatter/py.typed
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)     5305 2023-05-23 12:59:38.000000 python_json_log_formatter-3.2.0/python_json_log_formatter/python_json_log_formatter.py
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)      658 2023-05-23 12:59:38.000000 python_json_log_formatter-3.2.0/python_json_log_formatter/python_json_log_formatter.pyi
+drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-05-23 12:59:55.490194 python_json_log_formatter-3.2.0/python_json_log_formatter.egg-info/
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)     3400 2023-05-23 12:59:55.000000 python_json_log_formatter-3.2.0/python_json_log_formatter.egg-info/PKG-INFO
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)      540 2023-05-23 12:59:55.000000 python_json_log_formatter-3.2.0/python_json_log_formatter.egg-info/SOURCES.txt
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)        1 2023-05-23 12:59:55.000000 python_json_log_formatter-3.2.0/python_json_log_formatter.egg-info/dependency_links.txt
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)       26 2023-05-23 12:59:55.000000 python_json_log_formatter-3.2.0/python_json_log_formatter.egg-info/top_level.txt
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)       38 2023-05-23 12:59:55.490638 python_json_log_formatter-3.2.0/setup.cfg
```

### Comparing `python_json_log_formatter-3.0.2/LICENSE` & `python_json_log_formatter-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_json_log_formatter-3.0.2/PKG-INFO` & `python_json_log_formatter-3.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_json_log_formatter
-Version: 3.0.2
+Version: 3.2.0
 Summary: Supplements a default formatter configuration for machine-readable JSON logging and applies it
 Author-email: Niels Korschinsky <niels.korschinsky@ibm.com>
 Project-URL: Homepage, https://github.com/IBM/python-json-log-formatter
 Project-URL: Bug Tracker, https://github.com/IBM/python-json-log-formatter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -63,8 +63,13 @@
 ## Features
 
 Sets the logging format for the root logger and thus for every child logger.
 In EVERY file where logging happens, please use `LOGGER = logging.getLogger(__name__)` to get an individual logger.
 Allows printing exception information on any logging level, not only on the `EXCEPTION` level but also for `INFO` or `DEBUG`.
 Supply `exec_info` to print these.
 
-Sets `pipeline_status` and `job_status` to `failed` on `ERROR` or `CRITICAL`, supports minor logging levels (41, etc).
+Sets `pipeline_status` and `job_status` to `failed` on `CRITICAL`, supports minor logging levels (41, etc).
+
+To disable the logging on local machines, supply `disable_log_formatting=True` when configuring the logger.
+Alternatively, without code changes, you can supply the ENV var `DISABLE_LOG_FORMATTING"=True` to generally disable it.
+
+Every attribute of the LogRecord will be included in the formatted message unless specified in the `excluded_logging_context_keys` list.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python_json_log_formatter Version: 3.0.2 Summary:
+Metadata-Version: 2.1 Name: python_json_log_formatter Version: 3.2.0 Summary:
 Supplements a default formatter configuration for machine-readable JSON logging
 and applies it Author-email: Niels Korschinsky
 korschinsky@ibm.com> Project-URL: Homepage, https://github.com/IBM/python-json-
 log-formatter Project-URL: Bug Tracker, https://github.com/IBM/python-json-log-
 formatter/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
@@ -29,9 +29,14 @@
 VERSION = "1.0.0 (2022/11/24)" PythonLogger.setup_logger(VERSION,
 logging.DEBUG) LOGGER = logging.getLogger(__name__) ``` ## Features Sets the
 logging format for the root logger and thus for every child logger. In EVERY
 file where logging happens, please use `LOGGER = logging.getLogger(__name__)`
 to get an individual logger. Allows printing exception information on any
 logging level, not only on the `EXCEPTION` level but also for `INFO` or
 `DEBUG`. Supply `exec_info` to print these. Sets `pipeline_status` and
-`job_status` to `failed` on `ERROR` or `CRITICAL`, supports minor logging
-levels (41, etc).
+`job_status` to `failed` on `CRITICAL`, supports minor logging levels (41,
+etc). To disable the logging on local machines, supply
+`disable_log_formatting=True` when configuring the logger. Alternatively,
+without code changes, you can supply the ENV var `DISABLE_LOG_FORMATTING"=True`
+to generally disable it. Every attribute of the LogRecord will be included in
+the formatted message unless specified in the `excluded_logging_context_keys`
+list.
```

### Comparing `python_json_log_formatter-3.0.2/pyproject.toml` & `python_json_log_formatter-3.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_json_log_formatter-3.0.2/python_json_log_formatter/__init__.py` & `python_json_log_formatter-3.2.0/python_json_log_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `python_json_log_formatter-3.0.2/python_json_log_formatter.egg-info/PKG-INFO` & `python_json_log_formatter-3.2.0/python_json_log_formatter.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-json-log-formatter
-Version: 3.0.2
+Version: 3.2.0
 Summary: Supplements a default formatter configuration for machine-readable JSON logging and applies it
 Author-email: Niels Korschinsky <niels.korschinsky@ibm.com>
 Project-URL: Homepage, https://github.com/IBM/python-json-log-formatter
 Project-URL: Bug Tracker, https://github.com/IBM/python-json-log-formatter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -63,8 +63,13 @@
 ## Features
 
 Sets the logging format for the root logger and thus for every child logger.
 In EVERY file where logging happens, please use `LOGGER = logging.getLogger(__name__)` to get an individual logger.
 Allows printing exception information on any logging level, not only on the `EXCEPTION` level but also for `INFO` or `DEBUG`.
 Supply `exec_info` to print these.
 
-Sets `pipeline_status` and `job_status` to `failed` on `ERROR` or `CRITICAL`, supports minor logging levels (41, etc).
+Sets `pipeline_status` and `job_status` to `failed` on `CRITICAL`, supports minor logging levels (41, etc).
+
+To disable the logging on local machines, supply `disable_log_formatting=True` when configuring the logger.
+Alternatively, without code changes, you can supply the ENV var `DISABLE_LOG_FORMATTING"=True` to generally disable it.
+
+Every attribute of the LogRecord will be included in the formatted message unless specified in the `excluded_logging_context_keys` list.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-json-log-formatter Version: 3.0.2 Summary:
+Metadata-Version: 2.1 Name: python-json-log-formatter Version: 3.2.0 Summary:
 Supplements a default formatter configuration for machine-readable JSON logging
 and applies it Author-email: Niels Korschinsky
 korschinsky@ibm.com> Project-URL: Homepage, https://github.com/IBM/python-json-
 log-formatter Project-URL: Bug Tracker, https://github.com/IBM/python-json-log-
 formatter/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
@@ -29,9 +29,14 @@
 VERSION = "1.0.0 (2022/11/24)" PythonLogger.setup_logger(VERSION,
 logging.DEBUG) LOGGER = logging.getLogger(__name__) ``` ## Features Sets the
 logging format for the root logger and thus for every child logger. In EVERY
 file where logging happens, please use `LOGGER = logging.getLogger(__name__)`
 to get an individual logger. Allows printing exception information on any
 logging level, not only on the `EXCEPTION` level but also for `INFO` or
 `DEBUG`. Supply `exec_info` to print these. Sets `pipeline_status` and
-`job_status` to `failed` on `ERROR` or `CRITICAL`, supports minor logging
-levels (41, etc).
+`job_status` to `failed` on `CRITICAL`, supports minor logging levels (41,
+etc). To disable the logging on local machines, supply
+`disable_log_formatting=True` when configuring the logger. Alternatively,
+without code changes, you can supply the ENV var `DISABLE_LOG_FORMATTING"=True`
+to generally disable it. Every attribute of the LogRecord will be included in
+the formatted message unless specified in the `excluded_logging_context_keys`
+list.
```

### Comparing `python_json_log_formatter-3.0.2/python_json_log_formatter.egg-info/SOURCES.txt` & `python_json_log_formatter-3.2.0/python_json_log_formatter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

