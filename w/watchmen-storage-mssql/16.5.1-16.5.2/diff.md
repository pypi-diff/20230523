# Comparing `tmp/watchmen_storage_mssql-16.5.1.tar.gz` & `tmp/watchmen_storage_mssql-16.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_mssql-16.5.1.tar", max compression
+gzip compressed data, was "watchmen_storage_mssql-16.5.2.tar", max compression
```

## Comparing `watchmen_storage_mssql-16.5.1.tar` & `watchmen_storage_mssql-16.5.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-04-25 10:52:46.012223 watchmen_storage_mssql-16.5.1/LICENSE
--rw-r--r--   0        0        0      460 2023-04-25 10:52:46.016223 watchmen_storage_mssql-16.5.1/pyproject.toml
--rw-r--r--   0        0        0      259 2023-04-25 10:52:46.016223 watchmen_storage_mssql-16.5.1/src/watchmen_storage_mssql/__init__.py
--rw-r--r--   0        0        0     2294 2023-04-25 10:52:46.016223 watchmen_storage_mssql-16.5.1/src/watchmen_storage_mssql/data_source_mssql.py
--rw-r--r--   0        0        0     2450 2023-04-25 10:52:46.016223 watchmen_storage_mssql-16.5.1/src/watchmen_storage_mssql/script_builder_mssql.py
--rw-r--r--   0        0        0     7773 2023-04-25 10:52:46.016223 watchmen_storage_mssql-16.5.1/src/watchmen_storage_mssql/storage_mssql.py
--rw-r--r--   0        0        0     2085 2023-04-25 10:52:46.016223 watchmen_storage_mssql-16.5.1/src/watchmen_storage_mssql/storage_mssql_configuration.py
--rw-r--r--   0        0        0     7971 2023-04-25 10:52:46.016223 watchmen_storage_mssql-16.5.1/src/watchmen_storage_mssql/table_creator.py
--rw-r--r--   0        0        0    12465 2023-04-25 10:52:46.016223 watchmen_storage_mssql-16.5.1/src/watchmen_storage_mssql/where_build.py
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 watchmen_storage_mssql-16.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-23 07:54:10.436672 watchmen_storage_mssql-16.5.2/LICENSE
+-rw-r--r--   0        0        0      460 2023-05-23 07:54:10.436672 watchmen_storage_mssql-16.5.2/pyproject.toml
+-rw-r--r--   0        0        0      259 2023-05-23 07:54:10.436672 watchmen_storage_mssql-16.5.2/src/watchmen_storage_mssql/__init__.py
+-rw-r--r--   0        0        0     2294 2023-05-23 07:54:10.436672 watchmen_storage_mssql-16.5.2/src/watchmen_storage_mssql/data_source_mssql.py
+-rw-r--r--   0        0        0     2450 2023-05-23 07:54:10.436672 watchmen_storage_mssql-16.5.2/src/watchmen_storage_mssql/script_builder_mssql.py
+-rw-r--r--   0        0        0     7773 2023-05-23 07:54:10.436672 watchmen_storage_mssql-16.5.2/src/watchmen_storage_mssql/storage_mssql.py
+-rw-r--r--   0        0        0     2085 2023-05-23 07:54:10.436672 watchmen_storage_mssql-16.5.2/src/watchmen_storage_mssql/storage_mssql_configuration.py
+-rw-r--r--   0        0        0     7971 2023-05-23 07:54:10.436672 watchmen_storage_mssql-16.5.2/src/watchmen_storage_mssql/table_creator.py
+-rw-r--r--   0        0        0    12465 2023-05-23 07:54:10.436672 watchmen_storage_mssql-16.5.2/src/watchmen_storage_mssql/where_build.py
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 watchmen_storage_mssql-16.5.2/PKG-INFO
```

### Comparing `watchmen_storage_mssql-16.5.1/LICENSE` & `watchmen_storage_mssql-16.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mssql-16.5.1/src/watchmen_storage_mssql/data_source_mssql.py` & `watchmen_storage_mssql-16.5.2/src/watchmen_storage_mssql/data_source_mssql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mssql-16.5.1/src/watchmen_storage_mssql/script_builder_mssql.py` & `watchmen_storage_mssql-16.5.2/src/watchmen_storage_mssql/script_builder_mssql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mssql-16.5.1/src/watchmen_storage_mssql/storage_mssql.py` & `watchmen_storage_mssql-16.5.2/src/watchmen_storage_mssql/storage_mssql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mssql-16.5.1/src/watchmen_storage_mssql/storage_mssql_configuration.py` & `watchmen_storage_mssql-16.5.2/src/watchmen_storage_mssql/storage_mssql_configuration.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mssql-16.5.1/src/watchmen_storage_mssql/table_creator.py` & `watchmen_storage_mssql-16.5.2/src/watchmen_storage_mssql/table_creator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mssql-16.5.1/src/watchmen_storage_mssql/where_build.py` & `watchmen_storage_mssql-16.5.2/src/watchmen_storage_mssql/where_build.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mssql-16.5.1/PKG-INFO` & `watchmen_storage_mssql-16.5.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-mssql
-Version: 16.5.1
+Version: 16.5.2
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyodbc (>=4.0.32,<5.0.0)
-Requires-Dist: watchmen-storage-rds (==16.5.1)
+Requires-Dist: watchmen-storage-rds (==16.5.2)
```

