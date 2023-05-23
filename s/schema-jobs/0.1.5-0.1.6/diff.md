# Comparing `tmp/schema_jobs-0.1.5.tar.gz` & `tmp/schema_jobs-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schema_jobs-0.1.5.tar", max compression
+gzip compressed data, was "schema_jobs-0.1.6.tar", max compression
```

## Comparing `schema_jobs-0.1.5.tar` & `schema_jobs-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      460 2023-05-18 14:28:10.609980 schema_jobs-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 15:32:59.929513 schema_jobs-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-05-10 15:32:59.929513 schema_jobs-0.1.5/schema_jobs/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.5/schema_jobs/jobs/__init__.py
--rw-r--r--   0        0        0      192 2023-05-18 13:18:38.390862 schema_jobs-0.1.5/schema_jobs/jobs/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358473 schema_jobs-0.1.5/schema_jobs/jobs/configuration/__init__.py
--rw-r--r--   0        0        0      184 2023-05-18 13:27:25.274846 schema_jobs-0.1.5/schema_jobs/jobs/configuration/database_configuration.py
--rw-r--r--   0        0        0      917 2023-05-16 18:03:06.305152 schema_jobs-0.1.5/schema_jobs/jobs/configuration/table_configs.py
--rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.5/schema_jobs/jobs/deploy/__init__.py
--rw-r--r--   0        0        0      600 2023-05-18 13:46:35.012146 schema_jobs-0.1.5/schema_jobs/jobs/deploy/deploy_database_tables.py
--rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.5/schema_jobs/jobs/migration/__init__.py
--rw-r--r--   0        0        0      232 2023-05-16 18:15:04.261246 schema_jobs-0.1.5/schema_jobs/jobs/migration/deploy_migration.py
--rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.5/schema_jobs/jobs/utility/__init__.py
--rw-r--r--   0        0        0      200 2023-05-18 13:18:38.408301 schema_jobs-0.1.5/schema_jobs/jobs/utility/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.5/schema_jobs/jobs/utility/schema/__init__.py
--rw-r--r--   0        0        0      207 2023-05-18 13:18:38.429925 schema_jobs-0.1.5/schema_jobs/jobs/utility/schema/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      587 2023-05-18 13:18:38.438950 schema_jobs-0.1.5/schema_jobs/jobs/utility/schema/__pycache__/database.cpython-39.pyc
--rw-r--r--   0        0        0      306 2023-05-18 13:55:36.742899 schema_jobs-0.1.5/schema_jobs/jobs/utility/schema/database.py
--rw-r--r--   0        0        0       62 2023-05-16 18:12:06.405926 schema_jobs-0.1.5/schema_jobs/jobs/utility/schema/migration.py
--rw-r--r--   0        0        0     1769 2023-05-17 18:22:00.078921 schema_jobs-0.1.5/schema_jobs/jobs/utility/schema/schemas.py
--rw-r--r--   0        0        0      112 2023-05-17 18:46:35.559107 schema_jobs-0.1.5/schema_jobs/jobs/utility/schema/sql.py
--rw-r--r--   0        0        0      354 2023-05-18 14:28:05.653613 schema_jobs-0.1.5/schema_jobs/jobs/utility/schema/table.py
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 schema_jobs-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      483 2023-05-23 14:58:24.982793 schema_jobs-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-10 15:32:59.929513 schema_jobs-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 15:32:59.929513 schema_jobs-0.1.6/schema_jobs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.6/schema_jobs/jobs/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-18 13:18:38.390862 schema_jobs-0.1.6/schema_jobs/jobs/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358473 schema_jobs-0.1.6/schema_jobs/jobs/configuration/__init__.py
+-rw-r--r--   0        0        0      288 2023-05-18 16:00:44.839885 schema_jobs-0.1.6/schema_jobs/jobs/configuration/database_configuration.py
+-rw-r--r--   0        0        0     1232 2023-05-23 14:57:56.216277 schema_jobs-0.1.6/schema_jobs/jobs/configuration/table_configs.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.6/schema_jobs/jobs/deploy/__init__.py
+-rw-r--r--   0        0        0      649 2023-05-18 15:51:28.746729 schema_jobs-0.1.6/schema_jobs/jobs/deploy/deploy_database_tables.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.6/schema_jobs/jobs/migration/__init__.py
+-rw-r--r--   0        0        0      278 2023-05-18 15:57:39.738142 schema_jobs-0.1.6/schema_jobs/jobs/migration/deploy_migration.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.6/schema_jobs/jobs/utility/__init__.py
+-rw-r--r--   0        0        0      200 2023-05-18 13:18:38.408301 schema_jobs-0.1.6/schema_jobs/jobs/utility/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.6/schema_jobs/jobs/utility/schema/__init__.py
+-rw-r--r--   0        0        0      207 2023-05-18 13:18:38.429925 schema_jobs-0.1.6/schema_jobs/jobs/utility/schema/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      587 2023-05-18 13:18:38.438950 schema_jobs-0.1.6/schema_jobs/jobs/utility/schema/__pycache__/database.cpython-39.pyc
+-rw-r--r--   0        0        0      374 2023-05-18 16:09:08.982762 schema_jobs-0.1.6/schema_jobs/jobs/utility/schema/database.py
+-rw-r--r--   0        0        0      108 2023-05-18 15:58:01.773993 schema_jobs-0.1.6/schema_jobs/jobs/utility/schema/migration.py
+-rw-r--r--   0        0        0     2164 2023-05-18 16:06:29.334473 schema_jobs-0.1.6/schema_jobs/jobs/utility/schema/schemas.py
+-rw-r--r--   0        0        0      169 2023-05-18 15:53:55.019901 schema_jobs-0.1.6/schema_jobs/jobs/utility/schema/sql.py
+-rw-r--r--   0        0        0      422 2023-05-18 16:09:08.990666 schema_jobs-0.1.6/schema_jobs/jobs/utility/schema/table.py
+-rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 schema_jobs-0.1.6/PKG-INFO
```

### Comparing `schema_jobs-0.1.5/schema_jobs/jobs/configuration/table_configs.py` & `schema_jobs-0.1.6/schema_jobs/jobs/configuration/table_configs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,80 @@
-from dataclasses import dataclass
-
-from schema_jobs.jobs.utility.schema.schemas import bronze_machine_raw, bronze_sap_bseg, bronze_sales, gold_sales
+"""
+fill in
+"""
 
 import abc
+from dataclasses import dataclass
+
+from schema_jobs.jobs.utility.schema.schemas import (
+    bronze_machine_raw,
+    bronze_sales,
+    bronze_sap_bseg,
+    gold_sales,
+)
 
 
 class TableConfig(abc.ABC):
-    pass
+    """
+    fill in
+
+    """
+
+    table_name = ""
+    database_name = ""
+    schema = ""
 
 
 @dataclass
 class TableConfigBronzeMachineRaw(TableConfig):
-    table_name = "machine_raw"
+    """
+    fill in
+
+    """
+
+    table_name = "bronze_maine_raw"
     database_name = "dev"
     schema = bronze_machine_raw()
 
 
 @dataclass
 class TableConfigBronzSapBseg(TableConfig):
-    table_name = "sap_bseg"
+    """
+    fill in
+
+    """
+
+    table_name = "bronze_sap_bseg"
     database_name = "dev"
     schema = bronze_sap_bseg()
 
 
 @dataclass
 class TableConfigBronzeSales(TableConfig):
-    table_name = "sales"
+    """
+    fill in
+
+    """
+
+    table_name = "bronze_sales"
     database_name = "dev"
     schema = bronze_sales()
 
 
 @dataclass
 class TableConfigGoldSales(TableConfig):
+    """
+    fill in
+
+    """
+
     table_name = "gold_sales"
     database_name = "dev"
     schema = gold_sales()
 
 
-tables = [TableConfigBronzeMachineRaw, TableConfigBronzSapBseg, TableConfigBronzeSales, TableConfigGoldSales]
+tables = [
+    TableConfigBronzeMachineRaw,
+    TableConfigBronzSapBseg,
+    TableConfigBronzeSales,
+    TableConfigGoldSales,
+]
```

### Comparing `schema_jobs-0.1.5/schema_jobs/jobs/deploy/deploy_database_tables.py` & `schema_jobs-0.1.6/schema_jobs/jobs/deploy/deploy_database_tables.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,23 @@
+"""
+fill in
+
+"""
+
 from schema_jobs.jobs.configuration.database_configuration import DatabaseConfiguration
+from schema_jobs.jobs.configuration.table_configs import tables
 from schema_jobs.jobs.utility.schema.database import deploy_database
 from schema_jobs.jobs.utility.schema.table import deploy_table
-from schema_jobs.jobs.configuration.table_configs import tables
+
 
 def deploy_database_tables():
-    ""
-    #spark = SparkSession \
+    """
+    fill in
+    """
+    # spark = SparkSession \
     #    .builder \
     #    .appName("Schema App") \
     #    .getOrCreate()
     deploy_database(DatabaseConfiguration)
     for table in tables:
         deploy_table(table)
```

### Comparing `schema_jobs-0.1.5/schema_jobs/jobs/utility/schema/__pycache__/database.cpython-39.pyc` & `schema_jobs-0.1.6/schema_jobs/jobs/utility/schema/__pycache__/database.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `schema_jobs-0.1.5/schema_jobs/jobs/utility/schema/schemas.py` & `schema_jobs-0.1.6/schema_jobs/jobs/utility/schema/schemas.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,91 @@
-from pyspark.sql.types import StructType,FloatType,BinaryType, StructField, StringType, IntegerType
+"""
+fill in
+"""
+
+from pyspark.sql.types import (
+    BinaryType,
+    FloatType,
+    IntegerType,
+    StringType,
+    StructField,
+    StructType,
+)
 
 
 def bronze_machine_raw():
-    schema = StructType([
-        StructField("N8j2", FloatType(), True),
-        StructField("42mj", FloatType(), True),
-        StructField("6tk3", BinaryType(), True),
-        ])
+    """
+    fill in
+    """
+    schema = StructType(
+        [
+            StructField("N8j2", FloatType(), True),
+            StructField("42mj", FloatType(), True),
+            StructField("6tk3", BinaryType(), True),
+        ]
+    )
     return schema
 
 
 def silver_machine_raw():
-    schema = StructType([
-        StructField("N8j2", FloatType(), True),
-        StructField("42mj", FloatType(), True),
-        StructField("6tk3", BinaryType(), True),
-        StructField("engine_type", StringType(), True)
-        ])
+    """
+    fill in
+    """
+    schema = StructType(
+        [
+            StructField("N8j2", FloatType(), True),
+            StructField("42mj", FloatType(), True),
+            StructField("6tk3", BinaryType(), True),
+            StructField("engine_type", StringType(), True),
+        ]
+    )
     return schema
 
 
 def bronze_sap_bseg():
-    schema = StructType([
-        StructField("MANDT", StringType(), True),
-        StructField("BUKRS", StringType(), True),
-        StructField("BELNR", StringType(), True),
-        StructField("GJAHR", FloatType(), True),
-        StructField("BUZEI", FloatType(), True)
-        ])
+    """
+    fill in
+    """
+    schema = StructType(
+        [
+            StructField("MANDT", StringType(), True),
+            StructField("BUKRS", StringType(), True),
+            StructField("BELNR", StringType(), True),
+            StructField("GJAHR", FloatType(), True),
+            StructField("BUZEI", FloatType(), True),
+        ]
+    )
     return schema
 
 
 def bronze_sales():
-    schema = StructType([
-        StructField("ORDERNUMBER", IntegerType(), True),
-        StructField("SALE", FloatType(), True),
-        StructField("ORDERDATE", IntegerType(), True),
-        StructField("STATUS", BinaryType(), True),
-        StructField("CUSTOMERNAME", StringType(), True),
-        StructField("ADDRESSLINE", IntegerType(), True),
-        StructField("CITY", StringType(), True),
-        StructField("STATE", StringType(), True),
-        StructField("STORE", StringType(), True)
-        ])
+    """
+    fill in
+    """
+    schema = StructType(
+        [
+            StructField("ORDERNUMBER", IntegerType(), True),
+            StructField("SALE", FloatType(), True),
+            StructField("ORDERDATE", IntegerType(), True),
+            StructField("STATUS", BinaryType(), True),
+            StructField("CUSTOMERNAME", StringType(), True),
+            StructField("ADDRESSLINE", IntegerType(), True),
+            StructField("CITY", StringType(), True),
+            StructField("STATE", StringType(), True),
+            StructField("STORE", StringType(), True),
+        ]
+    )
     return schema
 
+
 def gold_sales():
-    schema = StructType([
-        StructField("CUSTOMERNAME", StringType(), True),
-        StructField("AVG", FloatType(), True),
-        StructField("TOTAL", FloatType(), True),
-        ])
+    """
+    fill in
+    """
+    schema = StructType(
+        [
+            StructField("CUSTOMERNAME", StringType(), True),
+            StructField("AVG", FloatType(), True),
+            StructField("TOTAL", FloatType(), True),
+        ]
+    )
     return schema
```

