# Comparing `tmp/schema_jobs-0.1.8.tar.gz` & `tmp/schema_jobs-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schema_jobs-0.1.8.tar", max compression
+gzip compressed data, was "schema_jobs-0.1.9.tar", max compression
```

## Comparing `schema_jobs-0.1.8.tar` & `schema_jobs-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      483 2023-05-23 15:59:54.761127 schema_jobs-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 15:32:59.929513 schema_jobs-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-05-10 15:32:59.929513 schema_jobs-0.1.8/schema_jobs/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.8/schema_jobs/jobs/__init__.py
--rw-r--r--   0        0        0      192 2023-05-18 13:18:38.390862 schema_jobs-0.1.8/schema_jobs/jobs/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358473 schema_jobs-0.1.8/schema_jobs/jobs/configuration/__init__.py
--rw-r--r--   0        0        0      288 2023-05-18 16:00:44.839885 schema_jobs-0.1.8/schema_jobs/jobs/configuration/database_configuration.py
--rw-r--r--   0        0        0     1234 2023-05-23 15:37:25.290101 schema_jobs-0.1.8/schema_jobs/jobs/configuration/table_configs.py
--rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.8/schema_jobs/jobs/deploy/__init__.py
--rw-r--r--   0        0        0      649 2023-05-18 15:51:28.746729 schema_jobs-0.1.8/schema_jobs/jobs/deploy/deploy_database_tables.py
--rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.8/schema_jobs/jobs/migration/__init__.py
--rw-r--r--   0        0        0      278 2023-05-18 15:57:39.738142 schema_jobs-0.1.8/schema_jobs/jobs/migration/deploy_migration.py
--rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.8/schema_jobs/jobs/utility/__init__.py
--rw-r--r--   0        0        0      200 2023-05-18 13:18:38.408301 schema_jobs-0.1.8/schema_jobs/jobs/utility/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.8/schema_jobs/jobs/utility/schema/__init__.py
--rw-r--r--   0        0        0      207 2023-05-18 13:18:38.429925 schema_jobs-0.1.8/schema_jobs/jobs/utility/schema/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      587 2023-05-18 13:18:38.438950 schema_jobs-0.1.8/schema_jobs/jobs/utility/schema/__pycache__/database.cpython-39.pyc
--rw-r--r--   0        0        0      374 2023-05-18 16:09:08.982762 schema_jobs-0.1.8/schema_jobs/jobs/utility/schema/database.py
--rw-r--r--   0        0        0      108 2023-05-18 15:58:01.773993 schema_jobs-0.1.8/schema_jobs/jobs/utility/schema/migration.py
--rw-r--r--   0        0        0     2164 2023-05-18 16:06:29.334473 schema_jobs-0.1.8/schema_jobs/jobs/utility/schema/schemas.py
--rw-r--r--   0        0        0      169 2023-05-18 15:53:55.019901 schema_jobs-0.1.8/schema_jobs/jobs/utility/schema/sql.py
--rw-r--r--   0        0        0      422 2023-05-18 16:09:08.990666 schema_jobs-0.1.8/schema_jobs/jobs/utility/schema/table.py
--rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 schema_jobs-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      483 2023-05-23 16:39:53.508697 schema_jobs-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-10 15:32:59.929513 schema_jobs-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 15:32:59.929513 schema_jobs-0.1.9/schema_jobs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.9/schema_jobs/jobs/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-18 13:18:38.390862 schema_jobs-0.1.9/schema_jobs/jobs/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358473 schema_jobs-0.1.9/schema_jobs/jobs/configuration/__init__.py
+-rw-r--r--   0        0        0      288 2023-05-18 16:00:44.839885 schema_jobs-0.1.9/schema_jobs/jobs/configuration/database_configuration.py
+-rw-r--r--   0        0        0     1477 2023-05-23 16:39:41.304290 schema_jobs-0.1.9/schema_jobs/jobs/configuration/table_configs.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.9/schema_jobs/jobs/deploy/__init__.py
+-rw-r--r--   0        0        0      649 2023-05-18 15:51:28.746729 schema_jobs-0.1.9/schema_jobs/jobs/deploy/deploy_database_tables.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.9/schema_jobs/jobs/migration/__init__.py
+-rw-r--r--   0        0        0      278 2023-05-18 15:57:39.738142 schema_jobs-0.1.9/schema_jobs/jobs/migration/deploy_migration.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.9/schema_jobs/jobs/utility/__init__.py
+-rw-r--r--   0        0        0      200 2023-05-18 13:18:38.408301 schema_jobs-0.1.9/schema_jobs/jobs/utility/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.9/schema_jobs/jobs/utility/schema/__init__.py
+-rw-r--r--   0        0        0      207 2023-05-18 13:18:38.429925 schema_jobs-0.1.9/schema_jobs/jobs/utility/schema/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      587 2023-05-18 13:18:38.438950 schema_jobs-0.1.9/schema_jobs/jobs/utility/schema/__pycache__/database.cpython-39.pyc
+-rw-r--r--   0        0        0      374 2023-05-18 16:09:08.982762 schema_jobs-0.1.9/schema_jobs/jobs/utility/schema/database.py
+-rw-r--r--   0        0        0      108 2023-05-18 15:58:01.773993 schema_jobs-0.1.9/schema_jobs/jobs/utility/schema/migration.py
+-rw-r--r--   0        0        0     2164 2023-05-18 16:06:29.334473 schema_jobs-0.1.9/schema_jobs/jobs/utility/schema/schemas.py
+-rw-r--r--   0        0        0      169 2023-05-18 15:53:55.019901 schema_jobs-0.1.9/schema_jobs/jobs/utility/schema/sql.py
+-rw-r--r--   0        0        0      422 2023-05-18 16:09:08.990666 schema_jobs-0.1.9/schema_jobs/jobs/utility/schema/table.py
+-rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 schema_jobs-0.1.9/PKG-INFO
```

### Comparing `schema_jobs-0.1.8/schema_jobs/jobs/configuration/table_configs.py` & `schema_jobs-0.1.9/schema_jobs/jobs/configuration/table_configs.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import abc
 from dataclasses import dataclass
 
 from schema_jobs.jobs.utility.schema.schemas import (
     bronze_machine_raw,
     bronze_sales,
     bronze_sap_bseg,
-    gold_sales,
+    gold_sales, silver_machine_raw,
 )
 
 
 class TableConfig(abc.ABC):
     """
     fill in
 
@@ -32,14 +32,25 @@
     """
 
     table_name = "bronze_machine_raw"
     database_name = "dev"
     schema = bronze_machine_raw()
 
 
+class TableConfigSilverMachineRaw(TableConfig):
+    """
+    fill in
+
+    """
+
+    table_name = "bronze_machine_raw"
+    database_name = "dev"
+    schema = silver_machine_raw()
+
+
 @dataclass
 class TableConfigBronzSapBseg(TableConfig):
     """
     fill in
 
     """
 
@@ -72,9 +83,10 @@
     schema = gold_sales()
 
 
 tables = [
     TableConfigBronzeMachineRaw,
     TableConfigBronzSapBseg,
     TableConfigBronzeSales,
+    TableConfigSilverMachineRaw,
     TableConfigGoldSales,
 ]
```

### Comparing `schema_jobs-0.1.8/schema_jobs/jobs/deploy/deploy_database_tables.py` & `schema_jobs-0.1.9/schema_jobs/jobs/deploy/deploy_database_tables.py`

 * *Files identical despite different names*

### Comparing `schema_jobs-0.1.8/schema_jobs/jobs/utility/schema/__pycache__/database.cpython-39.pyc` & `schema_jobs-0.1.9/schema_jobs/jobs/utility/schema/__pycache__/database.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `schema_jobs-0.1.8/schema_jobs/jobs/utility/schema/schemas.py` & `schema_jobs-0.1.9/schema_jobs/jobs/utility/schema/schemas.py`

 * *Files identical despite different names*

