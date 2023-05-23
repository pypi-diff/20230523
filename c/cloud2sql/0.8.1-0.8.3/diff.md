# Comparing `tmp/cloud2sql-0.8.1.tar.gz` & `tmp/cloud2sql-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud2sql-0.8.1.tar", last modified: Fri Apr 14 17:00:15 2023, max compression
+gzip compressed data, was "cloud2sql-0.8.3.tar", last modified: Tue May 23 16:21:14 2023, max compression
```

## Comparing `cloud2sql-0.8.1.tar` & `cloud2sql-0.8.3.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:00:15.832192 cloud2sql-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-04-14 17:00:15.832192 cloud2sql-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:00:15.828192 cloud2sql-0.8.1/cloud2sql/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:00:15.832192 cloud2sql-0.8.1/cloud2sql/arrow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/arrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/arrow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/arrow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/arrow/type_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/arrow/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14034 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/collect_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/show_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/cloud2sql/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:00:15.832192 cloud2sql-0.8.1/cloud2sql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-04-14 17:00:15.000000 cloud2sql-0.8.1/cloud2sql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-14 17:00:15.000000 cloud2sql-0.8.1/cloud2sql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:00:15.000000 cloud2sql-0.8.1/cloud2sql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-14 17:00:15.000000 cloud2sql-0.8.1/cloud2sql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-14 17:00:15.000000 cloud2sql-0.8.1/cloud2sql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 17:00:15.000000 cloud2sql-0.8.1/cloud2sql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/requirements-mysql.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/requirements-parquet.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/requirements-postgresql.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/requirements-snowflake.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-14 17:00:15.832192 cloud2sql-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-14 16:57:00.000000 cloud2sql-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:21:14.374772 cloud2sql-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-05-23 16:21:14.374772 cloud2sql-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:21:14.370772 cloud2sql-0.8.3/cloud2sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:21:14.374772 cloud2sql-0.8.3/cloud2sql/arrow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/arrow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/arrow/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/arrow/type_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/arrow/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/collect_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/remote_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/show_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:21:14.374772 cloud2sql-0.8.3/cloud2sql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-05-23 16:21:14.000000 cloud2sql-0.8.3/cloud2sql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-23 16:21:14.000000 cloud2sql-0.8.3/cloud2sql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:21:14.000000 cloud2sql-0.8.3/cloud2sql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-23 16:21:14.000000 cloud2sql-0.8.3/cloud2sql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-23 16:21:14.000000 cloud2sql-0.8.3/cloud2sql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 16:21:14.000000 cloud2sql-0.8.3/cloud2sql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/requirements-mysql.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/requirements-parquet.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/requirements-postgresql.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/requirements-snowflake.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-23 16:21:14.374772 cloud2sql-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/setup.py
```

### Comparing `cloud2sql-0.8.1/LICENSE` & `cloud2sql-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.1/PKG-INFO` & `cloud2sql-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud2sql
-Version: 0.8.1
+Version: 0.8.3
 Summary: Read infrastructure data from your cloud and export it to a SQL database.
 Home-page: https://github.com/someengineering/cloud2sql
 License: Apache Software License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: all
```

### Comparing `cloud2sql-0.8.1/README.md` & `cloud2sql-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.1/cloud2sql/__main__.py` & `cloud2sql-0.8.3/cloud2sql/__main__.py`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.1/cloud2sql/analytics.py` & `cloud2sql-0.8.3/cloud2sql/analytics.py`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.1/cloud2sql/arrow/config.py` & `cloud2sql-0.8.3/cloud2sql/arrow/config.py`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.1/cloud2sql/arrow/model.py` & `cloud2sql-0.8.3/cloud2sql/arrow/model.py`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.1/cloud2sql/arrow/type_converter.py` & `cloud2sql-0.8.3/cloud2sql/arrow/type_converter.py`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.1/cloud2sql/arrow/writer.py` & `cloud2sql-0.8.3/cloud2sql/arrow/writer.py`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.1/cloud2sql/collect_plugins.py` & `cloud2sql-0.8.3/cloud2sql/collect_plugins.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 import re
 
 
 from cloud2sql.analytics import AnalyticsEventSender
 from cloud2sql.arrow.config import ArrowOutputConfig
 from cloud2sql.show_progress import CollectInfo
 from cloud2sql.sql import SqlUpdater, sql_updater
+from cloud2sql.remote_graph import RemoteGraphCollector
 
 try:
     from cloud2sql.arrow.model import ArrowModel
     from cloud2sql.arrow.writer import ArrowWriter
     from cloud2sql.arrow.config import FileDestination, CloudBucketDestination, S3Bucket, GCSBucket
 except ImportError:
     pass
@@ -61,18 +62,26 @@
     config: Config = Config  # type: ignore
     for entry_point in pkg_resources.iter_entry_points("resoto.plugins"):
         plugin_class = entry_point.load()
         if issubclass(plugin_class, BaseCollectorPlugin) and plugin_class.cloud in raw_config:
             log.info(f"Found collector {plugin_class.cloud} ({plugin_class.__name__})")
             plugin_class.add_config(config)
             plugin = plugin_class()
-            if hasattr(plugin, "core_feedback"):
-                setattr(plugin, "core_feedback", feedback.with_context(plugin.cloud))
             result[plugin_class.cloud] = plugin
 
+    # lookup local plugins
+    if RemoteGraphCollector.cloud in raw_config:
+        log.info(f"Found collector {RemoteGraphCollector.cloud} ({RemoteGraphCollector.__name__})")
+        result[RemoteGraphCollector.cloud] = RemoteGraphCollector()
+        RemoteGraphCollector.add_config(config)
+
+    for plugin in result.values():
+        if hasattr(plugin, "core_feedback"):
+            setattr(plugin, "core_feedback", feedback.with_context(plugin.cloud))
+
     Config.init_default_config()
     Config.running_config.data = {**Config.running_config.data, **Config.read_config(raw_config)}
     return result
 
 
 def configure(path_to_config: Optional[str]) -> Json:
     # at least one key should be present
```

### Comparing `cloud2sql-0.8.1/cloud2sql/schema_utils.py` & `cloud2sql-0.8.3/cloud2sql/schema_utils.py`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.1/cloud2sql/show_progress.py` & `cloud2sql-0.8.3/cloud2sql/show_progress.py`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.1/cloud2sql/snowflake.py` & `cloud2sql-0.8.3/cloud2sql/snowflake.py`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.1/cloud2sql/sql.py` & `cloud2sql-0.8.3/cloud2sql/sql.py`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.1/cloud2sql/util.py` & `cloud2sql-0.8.3/cloud2sql/util.py`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.1/cloud2sql.egg-info/PKG-INFO` & `cloud2sql-0.8.3/cloud2sql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud2sql
-Version: 0.8.1
+Version: 0.8.3
 Summary: Read infrastructure data from your cloud and export it to a SQL database.
 Home-page: https://github.com/someengineering/cloud2sql
 License: Apache Software License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: all
```

### Comparing `cloud2sql-0.8.1/cloud2sql.egg-info/SOURCES.txt` & `cloud2sql-0.8.3/cloud2sql.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 requirements.txt
 setup.cfg
 setup.py
 cloud2sql/__init__.py
 cloud2sql/__main__.py
 cloud2sql/analytics.py
 cloud2sql/collect_plugins.py
+cloud2sql/remote_graph.py
 cloud2sql/schema_utils.py
 cloud2sql/show_progress.py
 cloud2sql/snowflake.py
 cloud2sql/sql.py
 cloud2sql/util.py
 cloud2sql.egg-info/PKG-INFO
 cloud2sql.egg-info/SOURCES.txt
```

### Comparing `cloud2sql-0.8.1/setup.py` & `cloud2sql-0.8.3/setup.py`

 * *Files identical despite different names*

