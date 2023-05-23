# Comparing `tmp/etl_jobs-0.1.6.tar.gz` & `tmp/etl_jobs-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_jobs-0.1.6.tar", max compression
+gzip compressed data, was "etl_jobs-0.1.7.tar", max compression
```

## Comparing `etl_jobs-0.1.6.tar` & `etl_jobs-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0        0 2023-05-10 15:39:00.637598 etl_jobs-0.1.6/etl_jobs/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 15:06:18.864612 etl_jobs-0.1.6/etl_jobs/configuration/api_raw_data/__init__.py
--rw-r--r--   0        0        0      783 2023-05-23 15:37:16.223682 etl_jobs-0.1.6/etl_jobs/configuration/api_raw_data/apis.py
--rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.6/etl_jobs/jobs/extract/__init__.py
--rw-r--r--   0        0        0      965 2023-05-23 15:34:59.303942 etl_jobs-0.1.6/etl_jobs/jobs/extract/extract_data_api.py
--rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.6/etl_jobs/util/extract/__init__.py
--rw-r--r--   0        0        0      362 2023-05-19 15:08:39.349430 etl_jobs-0.1.6/etl_jobs/util/extract/api.py
--rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.6/etl_jobs/util/load/__init__.py
--rw-r--r--   0        0        0      308 2023-05-23 14:23:41.412186 etl_jobs-0.1.6/etl_jobs/util/load/delta_local.py
--rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.6/etl_jobs/util/transform/__init__.py
--rw-r--r--   0        0        0      444 2023-05-19 15:10:37.021525 etl_jobs-0.1.6/etl_jobs/util/transform/polar_bear.py
--rw-r--r--   0        0        0      499 2023-05-23 15:38:58.115064 etl_jobs-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 15:39:00.637598 etl_jobs-0.1.6/README.md
--rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 etl_jobs-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-10 15:39:00.637598 etl_jobs-0.1.7/etl_jobs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 15:06:18.864612 etl_jobs-0.1.7/etl_jobs/configuration/api_raw_data/__init__.py
+-rw-r--r--   0        0        0      783 2023-05-23 15:37:16.223682 etl_jobs-0.1.7/etl_jobs/configuration/api_raw_data/apis.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.7/etl_jobs/jobs/extract/__init__.py
+-rw-r--r--   0        0        0      773 2023-05-23 15:58:58.819126 etl_jobs-0.1.7/etl_jobs/jobs/extract/extract_data_api.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.7/etl_jobs/util/extract/__init__.py
+-rw-r--r--   0        0        0      362 2023-05-19 15:08:39.349430 etl_jobs-0.1.7/etl_jobs/util/extract/api.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.7/etl_jobs/util/load/__init__.py
+-rw-r--r--   0        0        0      308 2023-05-23 14:23:41.412186 etl_jobs-0.1.7/etl_jobs/util/load/delta_local.py
+-rw-r--r--   0        0        0      349 2023-05-23 15:52:29.507750 etl_jobs-0.1.7/etl_jobs/util/load/delta_spark.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.7/etl_jobs/util/transform/__init__.py
+-rw-r--r--   0        0        0      444 2023-05-19 15:10:37.021525 etl_jobs-0.1.7/etl_jobs/util/transform/polar_bear.py
+-rw-r--r--   0        0        0      499 2023-05-23 15:59:23.746066 etl_jobs-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-10 15:39:00.637598 etl_jobs-0.1.7/README.md
+-rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 etl_jobs-0.1.7/PKG-INFO
```

### Comparing `etl_jobs-0.1.6/etl_jobs/configuration/api_raw_data/apis.py` & `etl_jobs-0.1.7/etl_jobs/configuration/api_raw_data/apis.py`

 * *Files identical despite different names*

### Comparing `etl_jobs-0.1.6/etl_jobs/jobs/extract/extract_data_api.py` & `etl_jobs-0.1.7/etl_jobs/jobs/extract/extract_data_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 """
 fill in
 
 """
 from etl_jobs.configuration.api_raw_data.apis import Apis
 from etl_jobs.util.extract.api import get_api_data
-from etl_jobs.util.load.delta_local import append_table
+from etl_jobs.util.load.delta_spark import append_table
 from etl_jobs.util.transform.polar_bear import transform_machine_bronze
 
 
 def extract_data_api():
     """
     fill in
     """
     # spark = SparkSession \
     #    .builder \
     #    .appName("Schema App") \
     #    .getOrCreate()
     for api in Apis:
         raw = get_api_data(api.url, "56c5cc10")
-        location = "/user/hive/warehouse/dev.db/" + api.name
         if api.name == "bronze_maine_raw":
-            append_table(transformed, location)
             transformed = transform_machine_bronze(raw)
-            location
-            append_table(transformed, location)
-        else:
-            location = "/user/hive/warehouse/dev.db/" + api.name
-            append_table(raw, location)
+            append_table(transformed, api.name.replace("bronze", "gold"))
+        append_table(raw, api.name)
 
 
 if __name__ == "__main__":
     extract_data_api()
```

