# Comparing `tmp/etl_jobs-0.1.8.tar.gz` & `tmp/etl_jobs-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_jobs-0.1.8.tar", max compression
+gzip compressed data, was "etl_jobs-0.1.9.tar", max compression
```

## Comparing `etl_jobs-0.1.8.tar` & `etl_jobs-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2023-05-10 15:39:00.637598 etl_jobs-0.1.8/etl_jobs/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 15:06:18.864612 etl_jobs-0.1.8/etl_jobs/configuration/api_raw_data/__init__.py
--rw-r--r--   0        0        0      783 2023-05-23 15:37:16.223682 etl_jobs-0.1.8/etl_jobs/configuration/api_raw_data/apis.py
--rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.8/etl_jobs/jobs/extract/__init__.py
--rw-r--r--   0        0        0      773 2023-05-23 15:58:58.819126 etl_jobs-0.1.8/etl_jobs/jobs/extract/extract_data_api.py
--rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.8/etl_jobs/util/extract/__init__.py
--rw-r--r--   0        0        0      362 2023-05-19 15:08:39.349430 etl_jobs-0.1.8/etl_jobs/util/extract/api.py
--rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.8/etl_jobs/util/load/__init__.py
--rw-r--r--   0        0        0      308 2023-05-23 14:23:41.412186 etl_jobs-0.1.8/etl_jobs/util/load/delta_local.py
--rw-r--r--   0        0        0      349 2023-05-23 15:52:29.507750 etl_jobs-0.1.8/etl_jobs/util/load/delta_spark.py
--rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.8/etl_jobs/util/transform/__init__.py
--rw-r--r--   0        0        0      209 2023-05-23 16:17:14.072059 etl_jobs-0.1.8/etl_jobs/util/transform/gold_sales.py
--rw-r--r--   0        0        0      444 2023-05-19 15:10:37.021525 etl_jobs-0.1.8/etl_jobs/util/transform/polar_bear.py
--rw-r--r--   0        0        0      519 2023-05-23 16:18:46.713118 etl_jobs-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 15:39:00.637598 etl_jobs-0.1.8/README.md
--rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 etl_jobs-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-10 15:39:00.637598 etl_jobs-0.1.9/etl_jobs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 15:06:18.864612 etl_jobs-0.1.9/etl_jobs/configuration/api_raw_data/__init__.py
+-rw-r--r--   0        0        0      783 2023-05-23 15:37:16.223682 etl_jobs-0.1.9/etl_jobs/configuration/api_raw_data/apis.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.9/etl_jobs/jobs/extract/__init__.py
+-rw-r--r--   0        0        0     1072 2023-05-23 17:37:54.605716 etl_jobs-0.1.9/etl_jobs/jobs/extract/elt_data_api.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.9/etl_jobs/util/extract/__init__.py
+-rw-r--r--   0        0        0      362 2023-05-19 15:08:39.349430 etl_jobs-0.1.9/etl_jobs/util/extract/api.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.9/etl_jobs/util/load/__init__.py
+-rw-r--r--   0        0        0      308 2023-05-23 14:23:41.412186 etl_jobs-0.1.9/etl_jobs/util/load/delta_local.py
+-rw-r--r--   0        0        0      674 2023-05-23 18:36:08.946298 etl_jobs-0.1.9/etl_jobs/util/load/delta_spark.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.9/etl_jobs/util/transform/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-23 16:17:14.072059 etl_jobs-0.1.9/etl_jobs/util/transform/gold_sales.py
+-rw-r--r--   0        0        0      444 2023-05-19 15:10:37.021525 etl_jobs-0.1.9/etl_jobs/util/transform/polar_bear.py
+-rw-r--r--   0        0        0      519 2023-05-23 19:01:33.635903 etl_jobs-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-10 15:39:00.637598 etl_jobs-0.1.9/README.md
+-rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 etl_jobs-0.1.9/PKG-INFO
```

### Comparing `etl_jobs-0.1.8/etl_jobs/configuration/api_raw_data/apis.py` & `etl_jobs-0.1.9/etl_jobs/configuration/api_raw_data/apis.py`

 * *Files identical despite different names*

### Comparing `etl_jobs-0.1.8/pyproject.toml` & `etl_jobs-0.1.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "etl-jobs"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Brian L <bclipp770@gmail.com>"]
 readme = "README.md"
 packages = [{include = "etl_jobs"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `etl_jobs-0.1.8/PKG-INFO` & `etl_jobs-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl-jobs
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Brian L
 Author-email: bclipp770@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

