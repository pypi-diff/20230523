# Comparing `tmp/watchmen_data_surface-16.5.1.tar.gz` & `tmp/watchmen_data_surface-16.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_data_surface-16.5.1.tar", max compression
+gzip compressed data, was "watchmen_data_surface-16.5.2.tar", max compression
```

## Comparing `watchmen_data_surface-16.5.1.tar` & `watchmen_data_surface-16.5.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-04-25 10:52:45.976220 watchmen_data_surface-16.5.1/LICENSE
--rw-r--r--   0        0        0     1195 2023-04-25 10:52:45.976220 watchmen_data_surface-16.5.1/pyproject.toml
--rw-r--r--   0        0        0       43 2023-04-25 10:52:45.976220 watchmen_data_surface-16.5.1/src/watchmen_data_surface/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 10:52:45.976220 watchmen_data_surface-16.5.1/src/watchmen_data_surface/cache/__init__.py
--rw-r--r--   0        0        0     2237 2023-04-25 10:52:45.976220 watchmen_data_surface-16.5.1/src/watchmen_data_surface/cache/cache_router.py
--rw-r--r--   0        0        0        0 2023-04-25 10:52:45.976220 watchmen_data_surface-16.5.1/src/watchmen_data_surface/data/__init__.py
--rw-r--r--   0        0        0     9814 2023-04-25 10:52:45.976220 watchmen_data_surface-16.5.1/src/watchmen_data_surface/data/topic_data_router.py
--rw-r--r--   0        0        0      240 2023-04-25 10:52:45.976220 watchmen_data_surface-16.5.1/src/watchmen_data_surface/main.py
--rw-r--r--   0        0        0      462 2023-04-25 10:52:45.976220 watchmen_data_surface-16.5.1/src/watchmen_data_surface/settings.py
--rw-r--r--   0        0        0     1171 1970-01-01 00:00:00.000000 watchmen_data_surface-16.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-23 07:54:10.404670 watchmen_data_surface-16.5.2/LICENSE
+-rw-r--r--   0        0        0     1195 2023-05-23 07:54:10.404670 watchmen_data_surface-16.5.2/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-05-23 07:54:10.404670 watchmen_data_surface-16.5.2/src/watchmen_data_surface/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 07:54:10.404670 watchmen_data_surface-16.5.2/src/watchmen_data_surface/cache/__init__.py
+-rw-r--r--   0        0        0     2237 2023-05-23 07:54:10.404670 watchmen_data_surface-16.5.2/src/watchmen_data_surface/cache/cache_router.py
+-rw-r--r--   0        0        0        0 2023-05-23 07:54:10.404670 watchmen_data_surface-16.5.2/src/watchmen_data_surface/data/__init__.py
+-rw-r--r--   0        0        0     9814 2023-05-23 07:54:10.404670 watchmen_data_surface-16.5.2/src/watchmen_data_surface/data/topic_data_router.py
+-rw-r--r--   0        0        0      240 2023-05-23 07:54:10.404670 watchmen_data_surface-16.5.2/src/watchmen_data_surface/main.py
+-rw-r--r--   0        0        0      462 2023-05-23 07:54:10.404670 watchmen_data_surface-16.5.2/src/watchmen_data_surface/settings.py
+-rw-r--r--   0        0        0     1171 1970-01-01 00:00:00.000000 watchmen_data_surface-16.5.2/PKG-INFO
```

### Comparing `watchmen_data_surface-16.5.1/LICENSE` & `watchmen_data_surface-16.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_data_surface-16.5.1/pyproject.toml` & `watchmen_data_surface-16.5.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "watchmen-data-surface"
-version = "16.5.1"
+version = "16.5.2"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_data_surface", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-data-kernel = "16.5.1"
-watchmen-rest = "16.5.1"
-watchmen-storage-mysql = { version = "16.5.1", optional = true }
-watchmen-storage-oracle = { version = "16.5.1", optional = true }
-watchmen-storage-mongodb = { version = "16.5.1", optional = true }
-watchmen-storage-mssql = { version = "16.5.1", optional = true }
-watchmen-storage-postgresql = { version = "16.5.1", optional = true }
-watchmen-storage-oss = { version = "16.5.1", optional = true }
-watchmen-storage-s3 = { version = "16.5.1", optional = true }
+watchmen-data-kernel = "16.5.2"
+watchmen-rest = "16.5.2"
+watchmen-storage-mysql = { version = "16.5.2", optional = true }
+watchmen-storage-oracle = { version = "16.5.2", optional = true }
+watchmen-storage-mongodb = { version = "16.5.2", optional = true }
+watchmen-storage-mssql = { version = "16.5.2", optional = true }
+watchmen-storage-postgresql = { version = "16.5.2", optional = true }
+watchmen-storage-oss = { version = "16.5.2", optional = true }
+watchmen-storage-s3 = { version = "16.5.2", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
 mongodb = ["watchmen-storage-mongodb"]
```

### Comparing `watchmen_data_surface-16.5.1/src/watchmen_data_surface/cache/cache_router.py` & `watchmen_data_surface-16.5.2/src/watchmen_data_surface/cache/cache_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_surface-16.5.1/src/watchmen_data_surface/data/topic_data_router.py` & `watchmen_data_surface-16.5.2/src/watchmen_data_surface/data/topic_data_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_surface-16.5.1/PKG-INFO` & `watchmen_data_surface-16.5.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-data-surface
-Version: 16.5.1
+Version: 16.5.2
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,16 +14,16 @@
 Provides-Extra: mongodb
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
-Requires-Dist: watchmen-data-kernel (==16.5.1)
-Requires-Dist: watchmen-rest (==16.5.1)
-Requires-Dist: watchmen-storage-mongodb (==16.5.1) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.1) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.1) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.1) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.1) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.1) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.1) ; extra == "s3"
+Requires-Dist: watchmen-data-kernel (==16.5.2)
+Requires-Dist: watchmen-rest (==16.5.2)
+Requires-Dist: watchmen-storage-mongodb (==16.5.2) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.2) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.2) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.2) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.2) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.2) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.2) ; extra == "s3"
```

