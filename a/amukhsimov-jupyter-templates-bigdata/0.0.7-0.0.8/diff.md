# Comparing `tmp/amukhsimov-jupyter-templates-bigdata-0.0.7.tar.gz` & `tmp/amukhsimov-jupyter-templates-bigdata-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amukhsimov-jupyter-templates-bigdata-0.0.7.tar", last modified: Tue May 23 13:30:53 2023, max compression
+gzip compressed data, was "amukhsimov-jupyter-templates-bigdata-0.0.8.tar", last modified: Tue May 23 13:40:54 2023, max compression
```

## Comparing `amukhsimov-jupyter-templates-bigdata-0.0.7.tar` & `amukhsimov-jupyter-templates-bigdata-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 13:30:53.012127 amukhsimov-jupyter-templates-bigdata-0.0.7/
--rw-r--r--   0 amukhsimov   (502) staff       (20)      412 2023-05-23 13:30:53.011938 amukhsimov-jupyter-templates-bigdata-0.0.7/PKG-INFO
--rw-r--r--   0 amukhsimov   (502) staff       (20)     1998 2023-05-23 10:23:41.000000 amukhsimov-jupyter-templates-bigdata-0.0.7/README.md
--rw-r--r--   0 amukhsimov   (502) staff       (20)       38 2023-05-23 13:30:53.012179 amukhsimov-jupyter-templates-bigdata-0.0.7/setup.cfg
--rw-r--r--   0 amukhsimov   (502) staff       (20)      944 2023-05-23 13:30:41.000000 amukhsimov-jupyter-templates-bigdata-0.0.7/setup.py
-drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 13:30:53.009791 amukhsimov-jupyter-templates-bigdata-0.0.7/src/
-drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 13:30:53.010753 amukhsimov-jupyter-templates-bigdata-0.0.7/src/amukhsimov_jupyter_templates_bigdata/
--rw-r--r--   0 amukhsimov   (502) staff       (20)       79 2023-05-23 13:05:45.000000 amukhsimov-jupyter-templates-bigdata-0.0.7/src/amukhsimov_jupyter_templates_bigdata/__init__.py
--rw-r--r--   0 amukhsimov   (502) staff       (20)     9788 2023-05-23 13:30:34.000000 amukhsimov-jupyter-templates-bigdata-0.0.7/src/amukhsimov_jupyter_templates_bigdata/connectors.py
--rw-r--r--   0 amukhsimov   (502) staff       (20)      808 2023-05-23 08:22:13.000000 amukhsimov-jupyter-templates-bigdata-0.0.7/src/amukhsimov_jupyter_templates_bigdata/crypto.py
-drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 13:30:53.011736 amukhsimov-jupyter-templates-bigdata-0.0.7/src/amukhsimov_jupyter_templates_bigdata.egg-info/
--rw-r--r--   0 amukhsimov   (502) staff       (20)      412 2023-05-23 13:30:52.000000 amukhsimov-jupyter-templates-bigdata-0.0.7/src/amukhsimov_jupyter_templates_bigdata.egg-info/PKG-INFO
--rw-r--r--   0 amukhsimov   (502) staff       (20)      496 2023-05-23 13:30:52.000000 amukhsimov-jupyter-templates-bigdata-0.0.7/src/amukhsimov_jupyter_templates_bigdata.egg-info/SOURCES.txt
--rw-r--r--   0 amukhsimov   (502) staff       (20)        1 2023-05-23 13:30:52.000000 amukhsimov-jupyter-templates-bigdata-0.0.7/src/amukhsimov_jupyter_templates_bigdata.egg-info/dependency_links.txt
--rw-r--r--   0 amukhsimov   (502) staff       (20)       54 2023-05-23 13:30:52.000000 amukhsimov-jupyter-templates-bigdata-0.0.7/src/amukhsimov_jupyter_templates_bigdata.egg-info/requires.txt
--rw-r--r--   0 amukhsimov   (502) staff       (20)       37 2023-05-23 13:30:52.000000 amukhsimov-jupyter-templates-bigdata-0.0.7/src/amukhsimov_jupyter_templates_bigdata.egg-info/top_level.txt
+drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 13:40:54.033609 amukhsimov-jupyter-templates-bigdata-0.0.8/
+-rw-r--r--   0 amukhsimov   (502) staff       (20)      412 2023-05-23 13:40:54.033424 amukhsimov-jupyter-templates-bigdata-0.0.8/PKG-INFO
+-rw-r--r--   0 amukhsimov   (502) staff       (20)     1998 2023-05-23 10:23:41.000000 amukhsimov-jupyter-templates-bigdata-0.0.8/README.md
+-rw-r--r--   0 amukhsimov   (502) staff       (20)       38 2023-05-23 13:40:54.033662 amukhsimov-jupyter-templates-bigdata-0.0.8/setup.cfg
+-rw-r--r--   0 amukhsimov   (502) staff       (20)      944 2023-05-23 13:40:45.000000 amukhsimov-jupyter-templates-bigdata-0.0.8/setup.py
+drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 13:40:54.031531 amukhsimov-jupyter-templates-bigdata-0.0.8/src/
+drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 13:40:54.032449 amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata/
+-rw-r--r--   0 amukhsimov   (502) staff       (20)       79 2023-05-23 13:05:45.000000 amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata/__init__.py
+-rw-r--r--   0 amukhsimov   (502) staff       (20)     9788 2023-05-23 13:40:30.000000 amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata/connectors.py
+-rw-r--r--   0 amukhsimov   (502) staff       (20)      808 2023-05-23 08:22:13.000000 amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata/crypto.py
+drwxr-xr-x   0 amukhsimov   (502) staff       (20)        0 2023-05-23 13:40:54.033222 amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata.egg-info/
+-rw-r--r--   0 amukhsimov   (502) staff       (20)      412 2023-05-23 13:40:53.000000 amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata.egg-info/PKG-INFO
+-rw-r--r--   0 amukhsimov   (502) staff       (20)      496 2023-05-23 13:40:53.000000 amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata.egg-info/SOURCES.txt
+-rw-r--r--   0 amukhsimov   (502) staff       (20)        1 2023-05-23 13:40:53.000000 amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata.egg-info/dependency_links.txt
+-rw-r--r--   0 amukhsimov   (502) staff       (20)       54 2023-05-23 13:40:53.000000 amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata.egg-info/requires.txt
+-rw-r--r--   0 amukhsimov   (502) staff       (20)       37 2023-05-23 13:40:53.000000 amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata.egg-info/top_level.txt
```

### Comparing `amukhsimov-jupyter-templates-bigdata-0.0.7/README.md` & `amukhsimov-jupyter-templates-bigdata-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `amukhsimov-jupyter-templates-bigdata-0.0.7/setup.py` & `amukhsimov-jupyter-templates-bigdata-0.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'amukhsimov-jupyter-templates-bigdata'
 LONG_DESCRIPTION = 'No description'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="amukhsimov-jupyter-templates-bigdata",
```

### Comparing `amukhsimov-jupyter-templates-bigdata-0.0.7/src/amukhsimov_jupyter_templates_bigdata/connectors.py` & `amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata/connectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 
 class Connector:
     def __init__(self):
         pass
 
     def get_spark_connector(self, use_local_spark: bool, app_name: str):
-        if not use_local_spark:
+        if use_local_spark:
             spark = SparkSession.builder \
                 .config("spark.executor.memory", LOCAL_SPARK_EXECUTOR_MEMORY) \
                 .config("spark.driver.memory", LOCAL_SPARK_DRIVER_MEMORY) \
                 .config("spark.driver.maxResultsSize", LOCAL_SPARK_DRIVE_MAX_RESULTS_SIZE)
 
             if LOCAL_SPARK_DRIVER_EXTRA_CLASS_PATH is not None:
                 spark = spark.config("spark.driver.extraClassPath", LOCAL_SPARK_DRIVER_EXTRA_CLASS_PATH)
@@ -82,16 +82,16 @@
 
             spark = SparkSession.builder \
                 .config("spark.executor.memory", REMOTE_SPARK_EXECUTOR_MEMORY) \
                 .config("spark.driver.memory", REMOTE_SPARK_DRIVER_MEMORY) \
                 .config("spark.driver.maxResultsSize", REMOTE_SPARK_DRIVE_MAX_RESULTS_SIZE) \
                 .master(REMOTE_SPARK_MASTER)
 
-            if LOCAL_SPARK_DRIVER_EXTRA_CLASS_PATH is not None:
-                spark = spark.config("spark.driver.extraClassPath", LOCAL_SPARK_DRIVER_EXTRA_CLASS_PATH)
+            # if LOCAL_SPARK_DRIVER_EXTRA_CLASS_PATH is not None:
+            #     spark = spark.config("spark.driver.extraClassPath", LOCAL_SPARK_DRIVER_EXTRA_CLASS_PATH)
             if REMOTE_SPARK_HADOOP_FS_DEFAULT_FS is not None:
                 spark = spark.config("spark.hadoop.fs.defaultFS", REMOTE_SPARK_HADOOP_FS_DEFAULT_FS)
             if REMOTE_SPARK_SQL_WAREHOUSE_DIR is not None:
                 spark = spark.config("spark.sql.warehouse.dir", REMOTE_SPARK_SQL_WAREHOUSE_DIR)
 
             return spark.appName(app_name).getOrCreate()
```

### Comparing `amukhsimov-jupyter-templates-bigdata-0.0.7/src/amukhsimov_jupyter_templates_bigdata/crypto.py` & `amukhsimov-jupyter-templates-bigdata-0.0.8/src/amukhsimov_jupyter_templates_bigdata/crypto.py`

 * *Files identical despite different names*

