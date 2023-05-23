# Comparing `tmp/etl_jobs-0.1.4.tar.gz` & `tmp/etl_jobs-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_jobs-0.1.4.tar", max compression
+gzip compressed data, was "etl_jobs-0.1.5.tar", max compression
```

## Comparing `etl_jobs-0.1.4.tar` & `etl_jobs-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-05-10 15:39:00.637598 etl_jobs-0.1.4/etl_jobs/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 15:06:18.864612 etl_jobs-0.1.4/etl_jobs/configuration/api_raw_data/__init__.py
--rw-r--r--   0        0        0      781 2023-05-19 15:58:55.374031 etl_jobs-0.1.4/etl_jobs/configuration/api_raw_data/apis.py
--rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.4/etl_jobs/jobs/extract/__init__.py
--rw-r--r--   0        0        0      741 2023-05-19 15:59:22.196896 etl_jobs-0.1.4/etl_jobs/jobs/extract/extract_data_api.py
--rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.4/etl_jobs/util/extract/__init__.py
--rw-r--r--   0        0        0      362 2023-05-19 15:08:39.349430 etl_jobs-0.1.4/etl_jobs/util/extract/api.py
--rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.4/etl_jobs/util/load/__init__.py
--rw-r--r--   0        0        0      308 2023-05-23 14:23:41.412186 etl_jobs-0.1.4/etl_jobs/util/load/delta_local.py
--rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.4/etl_jobs/util/transform/__init__.py
--rw-r--r--   0        0        0      444 2023-05-19 15:10:37.021525 etl_jobs-0.1.4/etl_jobs/util/transform/polar_bear.py
--rw-r--r--   0        0        0      499 2023-05-23 14:24:10.489626 etl_jobs-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 15:39:00.637598 etl_jobs-0.1.4/README.md
--rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 etl_jobs-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-10 15:39:00.637598 etl_jobs-0.1.5/etl_jobs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 15:06:18.864612 etl_jobs-0.1.5/etl_jobs/configuration/api_raw_data/__init__.py
+-rw-r--r--   0        0        0      781 2023-05-19 15:58:55.374031 etl_jobs-0.1.5/etl_jobs/configuration/api_raw_data/apis.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.5/etl_jobs/jobs/extract/__init__.py
+-rw-r--r--   0        0        0      828 2023-05-23 15:00:27.257099 etl_jobs-0.1.5/etl_jobs/jobs/extract/extract_data_api.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.5/etl_jobs/util/extract/__init__.py
+-rw-r--r--   0        0        0      362 2023-05-19 15:08:39.349430 etl_jobs-0.1.5/etl_jobs/util/extract/api.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.5/etl_jobs/util/load/__init__.py
+-rw-r--r--   0        0        0      308 2023-05-23 14:23:41.412186 etl_jobs-0.1.5/etl_jobs/util/load/delta_local.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.5/etl_jobs/util/transform/__init__.py
+-rw-r--r--   0        0        0      444 2023-05-19 15:10:37.021525 etl_jobs-0.1.5/etl_jobs/util/transform/polar_bear.py
+-rw-r--r--   0        0        0      499 2023-05-23 14:58:56.257660 etl_jobs-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-10 15:39:00.637598 etl_jobs-0.1.5/README.md
+-rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 etl_jobs-0.1.5/PKG-INFO
```

### Comparing `etl_jobs-0.1.4/etl_jobs/configuration/api_raw_data/apis.py` & `etl_jobs-0.1.5/etl_jobs/configuration/api_raw_data/apis.py`

 * *Files identical despite different names*

### Comparing `etl_jobs-0.1.4/etl_jobs/jobs/extract/extract_data_api.py` & `etl_jobs-0.1.5/etl_jobs/jobs/extract/extract_data_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,17 +12,19 @@
     """
     fill in
     """
     # spark = SparkSession \
     #    .builder \
     #    .appName("Schema App") \
     #    .getOrCreate()
-    base_location = "/dbfs/tmp/dev/"
     for api in Apis:
         raw = get_api_data(api.url, "56c5cc10")
-        transformed = transform_machine_bronze(raw)
-        location = base_location + api.name
-        append_table(transformed, location)
+        location = "/user/hive/warehouse/dev.db/" + api.name
+        if api.name == "bronze_maine_raw":
+            transformed = transform_machine_bronze(raw)
+            append_table(transformed, location)
+        else:
+            append_table(raw, location)
 
 
 if __name__ == "__main__":
     extract_data_api()
```

