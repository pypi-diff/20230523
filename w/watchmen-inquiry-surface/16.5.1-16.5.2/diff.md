# Comparing `tmp/watchmen_inquiry_surface-16.5.1.tar.gz` & `tmp/watchmen_inquiry_surface-16.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_inquiry_surface-16.5.1.tar", max compression
+gzip compressed data, was "watchmen_inquiry_surface-16.5.2.tar", max compression
```

## Comparing `watchmen_inquiry_surface-16.5.1.tar` & `watchmen_inquiry_surface-16.5.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1061 2023-04-25 10:52:45.984220 watchmen_inquiry_surface-16.5.1/LICENSE
--rw-r--r--   0        0        0     1304 2023-04-25 10:52:45.984220 watchmen_inquiry_surface-16.5.1/pyproject.toml
--rw-r--r--   0        0        0       46 2023-04-25 10:52:45.984220 watchmen_inquiry_surface-16.5.1/src/watchmen_inquiry_surface/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 10:52:45.984220 watchmen_inquiry_surface-16.5.1/src/watchmen_inquiry_surface/data/__init__.py
--rw-r--r--   0        0        0     9852 2023-04-25 10:52:45.984220 watchmen_inquiry_surface-16.5.1/src/watchmen_inquiry_surface/data/data_router.py
--rw-r--r--   0        0        0      176 2023-04-25 10:52:45.984220 watchmen_inquiry_surface-16.5.1/src/watchmen_inquiry_surface/main.py
--rw-r--r--   0        0        0      476 2023-04-25 10:52:45.984220 watchmen_inquiry_surface-16.5.1/src/watchmen_inquiry_surface/settings.py
--rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 watchmen_inquiry_surface-16.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-23 07:54:10.412670 watchmen_inquiry_surface-16.5.2/LICENSE
+-rw-r--r--   0        0        0     1304 2023-05-23 07:54:10.412670 watchmen_inquiry_surface-16.5.2/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-05-23 07:54:10.412670 watchmen_inquiry_surface-16.5.2/src/watchmen_inquiry_surface/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 07:54:10.412670 watchmen_inquiry_surface-16.5.2/src/watchmen_inquiry_surface/data/__init__.py
+-rw-r--r--   0        0        0     9998 2023-05-23 07:54:10.412670 watchmen_inquiry_surface-16.5.2/src/watchmen_inquiry_surface/data/data_router.py
+-rw-r--r--   0        0        0      176 2023-05-23 07:54:10.412670 watchmen_inquiry_surface-16.5.2/src/watchmen_inquiry_surface/main.py
+-rw-r--r--   0        0        0      476 2023-05-23 07:54:10.412670 watchmen_inquiry_surface-16.5.2/src/watchmen_inquiry_surface/settings.py
+-rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 watchmen_inquiry_surface-16.5.2/PKG-INFO
```

### Comparing `watchmen_inquiry_surface-16.5.1/LICENSE` & `watchmen_inquiry_surface-16.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_surface-16.5.1/pyproject.toml` & `watchmen_inquiry_surface-16.5.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "watchmen-inquiry-surface"
-version = "16.5.1"
+version = "16.5.2"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_inquiry_surface", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-inquiry-kernel = "16.5.1"
-watchmen-rest = "16.5.1"
-watchmen-inquiry-trino = { version = "16.5.1", optional = true }
-watchmen-storage-mysql = { version = "16.5.1", optional = true }
-watchmen-storage-oracle = { version = "16.5.1", optional = true }
-watchmen-storage-mongodb = { version = "16.5.1", optional = true }
-watchmen-storage-mssql = { version = "16.5.1", optional = true }
-watchmen-storage-postgresql = { version = "16.5.1", optional = true }
-watchmen-storage-oss = { version = "16.5.1", optional = true }
-watchmen-storage-s3 = { version = "16.5.1", optional = true }
+watchmen-inquiry-kernel = "16.5.2"
+watchmen-rest = "16.5.2"
+watchmen-inquiry-trino = { version = "16.5.2", optional = true }
+watchmen-storage-mysql = { version = "16.5.2", optional = true }
+watchmen-storage-oracle = { version = "16.5.2", optional = true }
+watchmen-storage-mongodb = { version = "16.5.2", optional = true }
+watchmen-storage-mssql = { version = "16.5.2", optional = true }
+watchmen-storage-postgresql = { version = "16.5.2", optional = true }
+watchmen-storage-oss = { version = "16.5.2", optional = true }
+watchmen-storage-s3 = { version = "16.5.2", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 trino = ["watchmen-inquiry-trino"]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
```

### Comparing `watchmen_inquiry_surface-16.5.1/src/watchmen_inquiry_surface/data/data_router.py` & `watchmen_inquiry_surface-16.5.2/src/watchmen_inquiry_surface/data/data_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,16 @@
 		dataset_column = subject_column_map.get(name)
 		if dataset_column is None:
 			raise_400(f'Cannot find column[name={name}] from subject.')
 
 		arithmetic = ReportIndicatorArithmetic.NONE
 		if indicator.arithmetic == SubjectDatasetCriteriaIndicatorArithmetic.COUNT:
 			arithmetic = ReportIndicatorArithmetic.COUNT
+		elif indicator.arithmetic == SubjectDatasetCriteriaIndicatorArithmetic.DISTINCT_COUNT:
+			arithmetic = ReportIndicatorArithmetic.DISTINCT_COUNT
 		elif indicator.arithmetic == SubjectDatasetCriteriaIndicatorArithmetic.SUMMARY:
 			arithmetic = ReportIndicatorArithmetic.SUMMARY
 		elif indicator.arithmetic == SubjectDatasetCriteriaIndicatorArithmetic.AVERAGE:
 			arithmetic = ReportIndicatorArithmetic.AVERAGE
 		elif indicator.arithmetic == SubjectDatasetCriteriaIndicatorArithmetic.MAXIMUM:
 			arithmetic = ReportIndicatorArithmetic.MAXIMUM
 		elif indicator.arithmetic == SubjectDatasetCriteriaIndicatorArithmetic.MINIMUM:
```

### Comparing `watchmen_inquiry_surface-16.5.1/PKG-INFO` & `watchmen_inquiry_surface-16.5.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-inquiry-surface
-Version: 16.5.1
+Version: 16.5.2
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,17 +15,17 @@
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
 Provides-Extra: trino
-Requires-Dist: watchmen-inquiry-kernel (==16.5.1)
-Requires-Dist: watchmen-inquiry-trino (==16.5.1) ; extra == "trino"
-Requires-Dist: watchmen-rest (==16.5.1)
-Requires-Dist: watchmen-storage-mongodb (==16.5.1) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.1) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.1) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.1) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.1) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.1) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.1) ; extra == "s3"
+Requires-Dist: watchmen-inquiry-kernel (==16.5.2)
+Requires-Dist: watchmen-inquiry-trino (==16.5.2) ; extra == "trino"
+Requires-Dist: watchmen-rest (==16.5.2)
+Requires-Dist: watchmen-storage-mongodb (==16.5.2) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.2) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.2) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.2) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.2) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.2) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.2) ; extra == "s3"
```

