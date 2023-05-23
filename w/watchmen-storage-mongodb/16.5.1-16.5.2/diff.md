# Comparing `tmp/watchmen_storage_mongodb-16.5.1.tar.gz` & `tmp/watchmen_storage_mongodb-16.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_mongodb-16.5.1.tar", max compression
+gzip compressed data, was "watchmen_storage_mongodb-16.5.2.tar", max compression
```

## Comparing `watchmen_storage_mongodb-16.5.1.tar` & `watchmen_storage_mongodb-16.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1061 2023-04-25 10:52:46.008222 watchmen_storage_mongodb-16.5.1/LICENSE
--rw-r--r--   0        0        0      460 2023-04-25 10:52:46.012223 watchmen_storage_mongodb-16.5.1/pyproject.toml
--rw-r--r--   0        0        0      210 2023-04-25 10:52:46.012223 watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/__init__.py
--rw-r--r--   0        0        0      703 2023-04-25 10:52:46.012223 watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/codes_options.py
--rw-r--r--   0        0        0     1308 2023-04-25 10:52:46.012223 watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/data_source_mongo.py
--rw-r--r--   0        0        0     2540 2023-04-25 10:52:46.012223 watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/document_defs_helper.py
--rw-r--r--   0        0        0    17650 2023-04-25 10:52:46.012223 watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/document_defs_mongo.py
--rw-r--r--   0        0        0     2541 2023-04-25 10:52:46.012223 watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/document_mongo.py
--rw-r--r--   0        0        0     5220 2023-04-25 10:52:46.012223 watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/engine_mongo.py
--rw-r--r--   0        0        0      509 2023-04-25 10:52:46.012223 watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/sort_build.py
--rw-r--r--   0        0        0    21084 2023-04-25 10:52:46.012223 watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/storage_mongo.py
--rw-r--r--   0        0        0     1899 2023-04-25 10:52:46.012223 watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/storage_mongo_configuration.py
--rw-r--r--   0        0        0    11657 2023-04-25 10:52:46.012223 watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/topic_document_generate.py
--rw-r--r--   0        0        0    24666 2023-04-25 10:52:46.012223 watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/where_build.py
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 watchmen_storage_mongodb-16.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-23 07:54:10.432671 watchmen_storage_mongodb-16.5.2/LICENSE
+-rw-r--r--   0        0        0      460 2023-05-23 07:54:10.432671 watchmen_storage_mongodb-16.5.2/pyproject.toml
+-rw-r--r--   0        0        0      210 2023-05-23 07:54:10.432671 watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/__init__.py
+-rw-r--r--   0        0        0      703 2023-05-23 07:54:10.432671 watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/codes_options.py
+-rw-r--r--   0        0        0     1308 2023-05-23 07:54:10.432671 watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/data_source_mongo.py
+-rw-r--r--   0        0        0     2540 2023-05-23 07:54:10.432671 watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/document_defs_helper.py
+-rw-r--r--   0        0        0    17673 2023-05-23 07:54:10.432671 watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/document_defs_mongo.py
+-rw-r--r--   0        0        0     2541 2023-05-23 07:54:10.432671 watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/document_mongo.py
+-rw-r--r--   0        0        0     5220 2023-05-23 07:54:10.432671 watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/engine_mongo.py
+-rw-r--r--   0        0        0      509 2023-05-23 07:54:10.432671 watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/sort_build.py
+-rw-r--r--   0        0        0    21084 2023-05-23 07:54:10.436672 watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/storage_mongo.py
+-rw-r--r--   0        0        0     1899 2023-05-23 07:54:10.436672 watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/storage_mongo_configuration.py
+-rw-r--r--   0        0        0    11657 2023-05-23 07:54:10.436672 watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/topic_document_generate.py
+-rw-r--r--   0        0        0    24666 2023-05-23 07:54:10.436672 watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/where_build.py
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 watchmen_storage_mongodb-16.5.2/PKG-INFO
```

### Comparing `watchmen_storage_mongodb-16.5.1/LICENSE` & `watchmen_storage_mongodb-16.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/codes_options.py` & `watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/codes_options.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/data_source_mongo.py` & `watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/data_source_mongo.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/document_defs_helper.py` & `watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/document_defs_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/document_defs_mongo.py` & `watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/document_defs_mongo.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
 )
 # admin
 table_users = MongoDocument(
 	name='users',
 	columns=[
 		create_pk('user_id'),
 		create_str('name', False), create_str('nickname'), create_str('password'),
+		create_str('email'),
 		create_bool('is_active'), create_json('group_ids'), create_str('role'),
 		create_tenant_id(), *create_tuple_audit_columns(), create_optimistic_lock()
 	]
 )
 table_user_groups = MongoDocument(
 	name='user_groups',
 	columns=[
```

### Comparing `watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/document_mongo.py` & `watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/document_mongo.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/engine_mongo.py` & `watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/engine_mongo.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/storage_mongo.py` & `watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/storage_mongo.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/storage_mongo_configuration.py` & `watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/storage_mongo_configuration.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/topic_document_generate.py` & `watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/topic_document_generate.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.5.1/src/watchmen_storage_mongodb/where_build.py` & `watchmen_storage_mongodb-16.5.2/src/watchmen_storage_mongodb/where_build.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.5.1/PKG-INFO` & `watchmen_storage_mongodb-16.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-mongodb
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
 Requires-Dist: pymongo (>=4.1.0,<5.0.0)
-Requires-Dist: watchmen-storage (==16.5.1)
+Requires-Dist: watchmen-storage (==16.5.2)
```

