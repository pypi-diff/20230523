# Comparing `tmp/shipyard_templates-0.1.3.tar.gz` & `tmp/shipyard_templates-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_templates-0.1.3.tar", max compression
+gzip compressed data, was "shipyard_templates-0.1.4.tar", max compression
```

## Comparing `shipyard_templates-0.1.3.tar` & `shipyard_templates-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-04-18 15:33:24.335210 shipyard_templates-0.1.3/README.md
--rw-r--r--   0        0        0      342 2023-05-18 23:19:33.669964 shipyard_templates-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      358 2023-05-16 23:00:51.355646 shipyard_templates-0.1.3/shipyard_templates/__init__.py
--rw-r--r--   0        0        0      552 2023-04-18 15:33:24.336079 shipyard_templates-0.1.3/shipyard_templates/cloudstorage.py
--rw-r--r--   0        0        0     1965 2023-04-18 15:33:24.336218 shipyard_templates-0.1.3/shipyard_templates/database.py
--rw-r--r--   0        0        0      267 2023-04-18 15:33:24.336346 shipyard_templates-0.1.3/shipyard_templates/datavisualization.py
--rw-r--r--   0        0        0     1093 2023-04-18 15:33:24.336748 shipyard_templates-0.1.3/shipyard_templates/etl.py
--rw-r--r--   0        0        0      245 2023-04-18 15:33:24.336885 shipyard_templates-0.1.3/shipyard_templates/messaging.py
--rw-r--r--   0        0        0      235 2023-04-18 15:33:24.337013 shipyard_templates-0.1.3/shipyard_templates/notebooks.py
--rw-r--r--   0        0        0      753 2023-05-16 23:00:51.355840 shipyard_templates-0.1.3/shipyard_templates/projectmanagement.py
--rw-r--r--   0        0        0      543 2023-05-17 19:10:59.029455 shipyard_templates-0.1.3/shipyard_templates/shipyard_logger.py
--rw-r--r--   0        0        0      280 2023-04-18 15:33:24.337469 shipyard_templates-0.1.3/shipyard_templates/spreadsheets.py
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 shipyard_templates-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:21.819295 shipyard_templates-0.1.4/README.md
+-rw-r--r--   0        0        0      342 2023-05-23 14:13:44.147230 shipyard_templates-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      358 2023-05-16 19:54:06.644392 shipyard_templates-0.1.4/shipyard_templates/__init__.py
+-rw-r--r--   0        0        0      552 2023-05-12 18:48:21.819618 shipyard_templates-0.1.4/shipyard_templates/cloudstorage.py
+-rw-r--r--   0        0        0     1965 2023-05-12 18:48:21.819681 shipyard_templates-0.1.4/shipyard_templates/database.py
+-rw-r--r--   0        0        0      267 2023-05-12 18:48:21.819750 shipyard_templates-0.1.4/shipyard_templates/datavisualization.py
+-rw-r--r--   0        0        0     1093 2023-05-12 18:48:21.819815 shipyard_templates-0.1.4/shipyard_templates/etl.py
+-rw-r--r--   0        0        0      245 2023-05-12 18:48:21.819876 shipyard_templates-0.1.4/shipyard_templates/messaging.py
+-rw-r--r--   0        0        0      235 2023-05-12 18:48:21.819939 shipyard_templates-0.1.4/shipyard_templates/notebooks.py
+-rw-r--r--   0        0        0      753 2023-05-23 14:13:00.186819 shipyard_templates-0.1.4/shipyard_templates/projectmanagement.py
+-rw-r--r--   0        0        0      543 2023-05-23 01:46:27.306492 shipyard_templates-0.1.4/shipyard_templates/shipyard_logger.py
+-rw-r--r--   0        0        0      280 2023-05-12 18:48:21.820063 shipyard_templates-0.1.4/shipyard_templates/spreadsheets.py
+-rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 shipyard_templates-0.1.4/PKG-INFO
```

### Comparing `shipyard_templates-0.1.3/shipyard_templates/cloudstorage.py` & `shipyard_templates-0.1.4/shipyard_templates/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.1.3/shipyard_templates/database.py` & `shipyard_templates-0.1.4/shipyard_templates/database.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.1.3/shipyard_templates/etl.py` & `shipyard_templates-0.1.4/shipyard_templates/etl.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.1.3/shipyard_templates/projectmanagement.py` & `shipyard_templates-0.1.4/shipyard_templates/projectmanagement.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.1.3/shipyard_templates/shipyard_logger.py` & `shipyard_templates-0.1.4/shipyard_templates/shipyard_logger.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.1.3/PKG-INFO` & `shipyard_templates-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-templates
-Version: 0.1.3
+Version: 0.1.4
 Summary: Super classes for blueprint development
 License: Apache-2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

