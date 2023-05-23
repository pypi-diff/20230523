# Comparing `tmp/watchmen_collector_kernel-16.5.1.tar.gz` & `tmp/watchmen_collector_kernel-16.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_collector_kernel-16.5.1.tar", max compression
+gzip compressed data, was "watchmen_collector_kernel-16.5.2.tar", max compression
```

## Comparing `watchmen_collector_kernel-16.5.1.tar` & `watchmen_collector_kernel-16.5.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1061 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/LICENSE
--rw-r--r--   0        0        0     1197 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/__init__.py
--rw-r--r--   0        0        0      263 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/common/__init__.py
--rw-r--r--   0        0        0      302 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/common/constants.py
--rw-r--r--   0        0        0      697 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/common/settings.py
--rw-r--r--   0        0        0      666 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/model/__init__.py
--rw-r--r--   0        0        0      495 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/model/change_data_json.py
--rw-r--r--   0        0        0       99 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/model/change_data_json_history.py
--rw-r--r--   0        0        0      330 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/model/change_data_record.py
--rw-r--r--   0        0        0      106 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/model/change_data_record_history.py
--rw-r--r--   0        0        0      288 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/model/collector_model_config.py
--rw-r--r--   0        0        0     2143 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/model/collector_table_config.py
--rw-r--r--   0        0        0      264 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/model/competitive_lock.py
--rw-r--r--   0        0        0     1942 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/model/condition.py
--rw-r--r--   0        0        0     1362 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/model/scheduled_task.py
--rw-r--r--   0        0        0       93 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/model/scheduled_task_history.py
--rw-r--r--   0        0        0      251 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/model/trigger_event.py
--rw-r--r--   0        0        0      175 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/model/trigger_model.py
--rw-r--r--   0        0        0      229 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/model/trigger_table.py
--rw-r--r--   0        0        0      426 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/service/__init__.py
--rw-r--r--   0        0        0     2360 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/service/criteria_builder.py
--rw-r--r--   0        0        0     2873 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/service/data_capture.py
--rw-r--r--   0        0        0     2928 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/service/extract_source.py
--rw-r--r--   0        0        0     2452 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/service/extract_utils.py
--rw-r--r--   0        0        0     1142 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/service/lock_clean.py
--rw-r--r--   0        0        0      842 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/service/lock_helper.py
--rw-r--r--   0        0        0     1673 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/service/task_housekeeping.py
--rw-r--r--   0        0        0     3634 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/service/task_service.py
--rw-r--r--   0        0        0     6790 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/service/trigger_collector.py
--rw-r--r--   0        0        0     1173 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/__init__.py
--rw-r--r--   0        0        0     1774 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/change_data_json_history_service.py
--rw-r--r--   0        0        0     8464 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/change_data_json_service.py
--rw-r--r--   0        0        0     1845 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/change_data_record_history_service.py
--rw-r--r--   0        0        0     7953 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/change_data_record_service.py
--rw-r--r--   0        0        0     3830 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/collector_model_config_service.py
--rw-r--r--   0        0        0     5659 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/collector_table_config_service.py
--rw-r--r--   0        0        0     2534 2023-04-25 10:52:45.968219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/competitive_lock_service.py
--rw-r--r--   0        0        0     1586 2023-04-25 10:52:45.972219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/scheduled_task_history_service.py
--rw-r--r--   0        0        0     6825 2023-04-25 10:52:45.972219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/scheduled_task_service.py
--rw-r--r--   0        0        0     3099 2023-04-25 10:52:45.972219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/trigger_event_service.py
--rw-r--r--   0        0        0     3219 2023-04-25 10:52:45.972219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/trigger_model_service.py
--rw-r--r--   0        0        0     3779 2023-04-25 10:52:45.972219 watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/trigger_table_service.py
--rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 watchmen_collector_kernel-16.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-23 07:54:10.396669 watchmen_collector_kernel-16.5.2/LICENSE
+-rw-r--r--   0        0        0     1197 2023-05-23 07:54:10.396669 watchmen_collector_kernel-16.5.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-23 07:54:10.396669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/__init__.py
+-rw-r--r--   0        0        0      263 2023-05-23 07:54:10.396669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/common/__init__.py
+-rw-r--r--   0        0        0      302 2023-05-23 07:54:10.396669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/common/constants.py
+-rw-r--r--   0        0        0      697 2023-05-23 07:54:10.396669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/common/settings.py
+-rw-r--r--   0        0        0      666 2023-05-23 07:54:10.396669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/__init__.py
+-rw-r--r--   0        0        0      495 2023-05-23 07:54:10.396669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/change_data_json.py
+-rw-r--r--   0        0        0       99 2023-05-23 07:54:10.396669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/change_data_json_history.py
+-rw-r--r--   0        0        0      330 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/change_data_record.py
+-rw-r--r--   0        0        0      106 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/change_data_record_history.py
+-rw-r--r--   0        0        0      288 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/collector_model_config.py
+-rw-r--r--   0        0        0     2143 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/collector_table_config.py
+-rw-r--r--   0        0        0      264 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/competitive_lock.py
+-rw-r--r--   0        0        0     1942 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/condition.py
+-rw-r--r--   0        0        0     1362 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/scheduled_task.py
+-rw-r--r--   0        0        0       93 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/scheduled_task_history.py
+-rw-r--r--   0        0        0      251 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/trigger_event.py
+-rw-r--r--   0        0        0      175 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/trigger_model.py
+-rw-r--r--   0        0        0      229 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/trigger_table.py
+-rw-r--r--   0        0        0      426 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/__init__.py
+-rw-r--r--   0        0        0     2360 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/criteria_builder.py
+-rw-r--r--   0        0        0     2873 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/data_capture.py
+-rw-r--r--   0        0        0     2928 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/extract_source.py
+-rw-r--r--   0        0        0     2452 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/extract_utils.py
+-rw-r--r--   0        0        0     1142 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/lock_clean.py
+-rw-r--r--   0        0        0      842 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/lock_helper.py
+-rw-r--r--   0        0        0     1673 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/task_housekeeping.py
+-rw-r--r--   0        0        0     3634 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/task_service.py
+-rw-r--r--   0        0        0     6790 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/trigger_collector.py
+-rw-r--r--   0        0        0     1173 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/__init__.py
+-rw-r--r--   0        0        0     1774 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/change_data_json_history_service.py
+-rw-r--r--   0        0        0     8464 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/change_data_json_service.py
+-rw-r--r--   0        0        0     1845 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/change_data_record_history_service.py
+-rw-r--r--   0        0        0     7953 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/change_data_record_service.py
+-rw-r--r--   0        0        0     3830 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/collector_model_config_service.py
+-rw-r--r--   0        0        0     5659 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/collector_table_config_service.py
+-rw-r--r--   0        0        0     2534 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/competitive_lock_service.py
+-rw-r--r--   0        0        0     1586 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/scheduled_task_history_service.py
+-rw-r--r--   0        0        0     6825 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/scheduled_task_service.py
+-rw-r--r--   0        0        0     3099 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/trigger_event_service.py
+-rw-r--r--   0        0        0     3219 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/trigger_model_service.py
+-rw-r--r--   0        0        0     3779 2023-05-23 07:54:10.400669 watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/trigger_table_service.py
+-rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 watchmen_collector_kernel-16.5.2/PKG-INFO
```

### Comparing `watchmen_collector_kernel-16.5.1/LICENSE` & `watchmen_collector_kernel-16.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/pyproject.toml` & `watchmen_collector_kernel-16.5.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "watchmen-collector-kernel"
-version = "16.5.1"
+version = "16.5.2"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_collector_kernel", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.23.3"
-watchmen-data-kernel = "16.5.1"
-watchmen-storage-mysql = { version = "16.5.1", optional = true }
-watchmen-storage-oracle = { version = "16.5.1", optional = true }
-watchmen-storage-mongodb = { version = "16.5.1", optional = true }
-watchmen-storage-mssql = { version = "16.5.1", optional = true }
-watchmen-storage-postgresql = { version = "16.5.1", optional = true }
-watchmen-storage-oss = { version = "16.5.1", optional = true }
-watchmen-storage-s3 = { version = "16.5.1", optional = true }
+watchmen-data-kernel = "16.5.2"
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

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/common/settings.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/common/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/model/__init__.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/model/collector_table_config.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/collector_table_config.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/model/condition.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/condition.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/model/scheduled_task.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/model/scheduled_task.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/service/criteria_builder.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/criteria_builder.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/service/data_capture.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/data_capture.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/service/extract_source.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/extract_source.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/service/extract_utils.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/extract_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/service/lock_clean.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/lock_clean.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/service/lock_helper.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/lock_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/service/task_housekeeping.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/task_housekeeping.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/service/task_service.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/task_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/service/trigger_collector.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/service/trigger_collector.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/__init__.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/change_data_json_history_service.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/change_data_json_history_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/change_data_json_service.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/change_data_json_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/change_data_record_history_service.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/change_data_record_history_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/change_data_record_service.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/change_data_record_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/collector_model_config_service.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/collector_model_config_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/collector_table_config_service.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/collector_table_config_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/competitive_lock_service.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/competitive_lock_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/scheduled_task_history_service.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/scheduled_task_history_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/scheduled_task_service.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/scheduled_task_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/trigger_event_service.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/trigger_event_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/trigger_model_service.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/trigger_model_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/src/watchmen_collector_kernel/storage/trigger_table_service.py` & `watchmen_collector_kernel-16.5.2/src/watchmen_collector_kernel/storage/trigger_table_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.1/PKG-INFO` & `watchmen_collector_kernel-16.5.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-collector-kernel
-Version: 16.5.1
+Version: 16.5.2
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
 Requires-Dist: numpy (>=1.23.3,<2.0.0)
-Requires-Dist: watchmen-data-kernel (==16.5.1)
-Requires-Dist: watchmen-storage-mongodb (==16.5.1) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.1) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.1) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.1) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.1) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.1) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.1) ; extra == "s3"
+Requires-Dist: watchmen-data-kernel (==16.5.2)
+Requires-Dist: watchmen-storage-mongodb (==16.5.2) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.2) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.2) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.2) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.2) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.2) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.2) ; extra == "s3"
```

