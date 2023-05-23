# Comparing `tmp/watchmen_storage_oss-16.5.1.tar.gz` & `tmp/watchmen_storage_oss-16.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_oss-16.5.1.tar", max compression
+gzip compressed data, was "watchmen_storage_oss-16.5.2.tar", max compression
```

## Comparing `watchmen_storage_oss-16.5.1.tar` & `watchmen_storage_oss-16.5.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-04-25 10:52:46.024223 watchmen_storage_oss-16.5.1/LICENSE
--rw-r--r--   0        0        0      449 2023-04-25 10:52:46.024223 watchmen_storage_oss-16.5.1/pyproject.toml
--rw-r--r--   0        0        0      112 2023-04-25 10:52:46.024223 watchmen_storage_oss-16.5.1/src/watchmen_storage_oss/__init__.py
--rw-r--r--   0        0        0     1299 2023-04-25 10:52:46.024223 watchmen_storage_oss-16.5.1/src/watchmen_storage_oss/data_source_oss.py
--rw-r--r--   0        0        0      495 2023-04-25 10:52:46.024223 watchmen_storage_oss-16.5.1/src/watchmen_storage_oss/object_defs_oss.py
--rw-r--r--   0        0        0     1657 2023-04-25 10:52:46.024223 watchmen_storage_oss-16.5.1/src/watchmen_storage_oss/object_storage_service.py
--rw-r--r--   0        0        0     8903 2023-04-25 10:52:46.024223 watchmen_storage_oss-16.5.1/src/watchmen_storage_oss/storage_oss.py
--rw-r--r--   0        0        0     1836 2023-04-25 10:52:46.024223 watchmen_storage_oss-16.5.1/src/watchmen_storage_oss/storage_oss_configuration.py
--rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 watchmen_storage_oss-16.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-23 07:54:10.444672 watchmen_storage_oss-16.5.2/LICENSE
+-rw-r--r--   0        0        0      449 2023-05-23 07:54:10.444672 watchmen_storage_oss-16.5.2/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-05-23 07:54:10.444672 watchmen_storage_oss-16.5.2/src/watchmen_storage_oss/__init__.py
+-rw-r--r--   0        0        0     1299 2023-05-23 07:54:10.444672 watchmen_storage_oss-16.5.2/src/watchmen_storage_oss/data_source_oss.py
+-rw-r--r--   0        0        0      495 2023-05-23 07:54:10.444672 watchmen_storage_oss-16.5.2/src/watchmen_storage_oss/object_defs_oss.py
+-rw-r--r--   0        0        0     1657 2023-05-23 07:54:10.444672 watchmen_storage_oss-16.5.2/src/watchmen_storage_oss/object_storage_service.py
+-rw-r--r--   0        0        0     8903 2023-05-23 07:54:10.444672 watchmen_storage_oss-16.5.2/src/watchmen_storage_oss/storage_oss.py
+-rw-r--r--   0        0        0     1836 2023-05-23 07:54:10.444672 watchmen_storage_oss-16.5.2/src/watchmen_storage_oss/storage_oss_configuration.py
+-rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 watchmen_storage_oss-16.5.2/PKG-INFO
```

### Comparing `watchmen_storage_oss-16.5.1/LICENSE` & `watchmen_storage_oss-16.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.5.1/src/watchmen_storage_oss/data_source_oss.py` & `watchmen_storage_oss-16.5.2/src/watchmen_storage_oss/data_source_oss.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.5.1/src/watchmen_storage_oss/object_storage_service.py` & `watchmen_storage_oss-16.5.2/src/watchmen_storage_oss/object_storage_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.5.1/src/watchmen_storage_oss/storage_oss.py` & `watchmen_storage_oss-16.5.2/src/watchmen_storage_oss/storage_oss.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.5.1/src/watchmen_storage_oss/storage_oss_configuration.py` & `watchmen_storage_oss-16.5.2/src/watchmen_storage_oss/storage_oss_configuration.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.5.1/PKG-INFO` & `watchmen_storage_oss-16.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-oss
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
 Requires-Dist: oss2 (==2.15.0)
-Requires-Dist: watchmen-storage (==16.5.1)
+Requires-Dist: watchmen-storage (==16.5.2)
```

