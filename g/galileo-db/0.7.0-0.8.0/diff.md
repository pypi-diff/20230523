# Comparing `tmp/galileo-db-0.7.0.tar.gz` & `tmp/galileo-db-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/galileo-db-0.7.0.tar", last modified: Thu Nov  5 22:08:01 2020, max compression
+gzip compressed data, was "dist/galileo-db-0.8.0.tar", last modified: Fri Dec  4 18:35:30 2020, max compression
```

## Comparing `galileo-db-0.7.0.tar` & `galileo-db-0.8.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-11-05 22:08:01.949397 galileo-db-0.7.0/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1050 2020-11-05 22:08:01.949397 galileo-db-0.7.0/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      521 2020-06-26 10:59:16.000000 galileo-db-0.7.0/README.md
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-11-05 22:08:01.945397 galileo-db-0.7.0/galileo_db.egg-info/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1050 2020-11-05 22:08:01.000000 galileo-db-0.7.0/galileo_db.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1196 2020-11-05 22:08:01.000000 galileo-db-0.7.0/galileo_db.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2020-11-05 22:08:01.000000 galileo-db-0.7.0/galileo_db.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      111 2020-11-05 22:08:01.000000 galileo-db-0.7.0/galileo_db.egg-info/entry_points.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       58 2020-11-05 22:08:01.000000 galileo-db-0.7.0/galileo_db.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       16 2020-11-05 22:08:01.000000 galileo-db-0.7.0/galileo_db.egg-info/top_level.txt
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-11-05 22:08:01.945397 galileo-db-0.7.0/galileodb/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      215 2020-06-03 11:09:36.000000 galileo-db-0.7.0/galileodb/__init__.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-11-05 22:08:01.945397 galileo-db-0.7.0/galileodb/cli/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2020-06-03 11:09:36.000000 galileo-db-0.7.0/galileodb/cli/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1651 2020-10-11 21:49:48.000000 galileo-db-0.7.0/galileodb/cli/manager.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2552 2020-10-18 01:10:54.000000 galileo-db-0.7.0/galileodb/cli/recorder.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1971 2020-10-18 02:10:57.000000 galileo-db-0.7.0/galileodb/db.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1653 2020-11-05 21:44:39.000000 galileo-db-0.7.0/galileodb/factory.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2020 2020-10-18 01:10:54.000000 galileo-db-0.7.0/galileodb/model.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-11-05 22:08:01.945397 galileo-db-0.7.0/galileodb/recorder/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      363 2020-06-03 11:09:36.000000 galileo-db-0.7.0/galileodb/recorder/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3433 2020-10-18 01:10:54.000000 galileo-db-0.7.0/galileodb/recorder/events.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1207 2020-10-26 20:23:51.000000 galileo-db-0.7.0/galileodb/recorder/recorder.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2170 2020-06-03 11:09:36.000000 galileo-db-0.7.0/galileodb/recorder/telemetry.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3559 2020-10-26 20:23:51.000000 galileo-db-0.7.0/galileodb/recorder/traces.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-11-05 22:08:01.945397 galileo-db-0.7.0/galileodb/reporter/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2020-06-03 11:09:36.000000 galileo-db-0.7.0/galileodb/reporter/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      401 2020-06-03 11:09:36.000000 galileo-db-0.7.0/galileodb/reporter/events.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      357 2020-06-03 11:09:36.000000 galileo-db-0.7.0/galileodb/reporter/telemetry.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1015 2020-10-18 01:10:54.000000 galileo-db-0.7.0/galileodb/reporter/traces.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-11-05 22:08:01.945397 galileo-db-0.7.0/galileodb/sql/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2020-06-03 11:09:36.000000 galileo-db-0.7.0/galileodb/sql/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10200 2020-11-05 21:53:03.000000 galileo-db-0.7.0/galileodb/sql/adapter.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-11-05 22:08:01.945397 galileo-db-0.7.0/galileodb/sql/driver/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2020-06-03 11:09:36.000000 galileo-db-0.7.0/galileodb/sql/driver/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1026 2020-06-03 11:09:36.000000 galileo-db-0.7.0/galileodb/sql/driver/mysql.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      208 2020-06-03 11:09:36.000000 galileo-db-0.7.0/galileodb/sql/driver/sqlite.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1291 2020-10-19 13:20:24.000000 galileo-db-0.7.0/galileodb/sql/schema.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5337 2020-11-05 19:42:22.000000 galileo-db-0.7.0/galileodb/trace.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2020-11-05 22:08:01.949397 galileo-db-0.7.0/setup.cfg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1421 2020-11-05 22:06:47.000000 galileo-db-0.7.0/setup.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-11-05 22:08:01.945397 galileo-db-0.7.0/tests/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2020-06-03 11:09:36.000000 galileo-db-0.7.0/tests/__init__.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-11-05 22:08:01.949397 galileo-db-0.7.0/tests/recorder/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2020-06-03 11:09:36.000000 galileo-db-0.7.0/tests/recorder/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4539 2020-06-26 10:59:16.000000 galileo-db-0.7.0/tests/recorder/test_events.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2484 2020-11-05 22:03:51.000000 galileo-db-0.7.0/tests/recorder/test_telemetry.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3082 2020-10-26 20:23:51.000000 galileo-db-0.7.0/tests/recorder/test_traces.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-11-05 22:08:01.949397 galileo-db-0.7.0/tests/reporter/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2020-10-18 01:10:54.000000 galileo-db-0.7.0/tests/reporter/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2125 2020-10-18 01:10:54.000000 galileo-db-0.7.0/tests/reporter/test_traces.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-11-05 22:08:01.949397 galileo-db-0.7.0/tests/sql/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2020-06-03 11:09:36.000000 galileo-db-0.7.0/tests/sql/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3446 2020-10-11 21:49:48.000000 galileo-db-0.7.0/tests/sql/adapter.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-11-05 22:08:01.949397 galileo-db-0.7.0/tests/sql/driver/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2020-06-03 11:09:36.000000 galileo-db-0.7.0/tests/sql/driver/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      583 2020-06-03 11:09:36.000000 galileo-db-0.7.0/tests/sql/driver/test_sqlite.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6968 2020-11-05 20:19:57.000000 galileo-db-0.7.0/tests/test_db.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6266 2020-10-18 02:53:06.000000 galileo-db-0.7.0/tests/test_trace.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2949 2020-10-18 01:10:54.000000 galileo-db-0.7.0/tests/testutils.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-12-04 18:35:30.891009 galileo-db-0.8.0/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1353 2020-12-04 18:35:30.891009 galileo-db-0.8.0/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      808 2020-12-04 18:16:43.000000 galileo-db-0.8.0/README.md
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-12-04 18:35:30.887009 galileo-db-0.8.0/galileo_db.egg-info/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1353 2020-12-04 18:35:30.000000 galileo-db-0.8.0/galileo_db.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1196 2020-12-04 18:35:30.000000 galileo-db-0.8.0/galileo_db.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2020-12-04 18:35:30.000000 galileo-db-0.8.0/galileo_db.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      111 2020-12-04 18:35:30.000000 galileo-db-0.8.0/galileo_db.egg-info/entry_points.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       58 2020-12-04 18:35:30.000000 galileo-db-0.8.0/galileo_db.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       16 2020-12-04 18:35:30.000000 galileo-db-0.8.0/galileo_db.egg-info/top_level.txt
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-12-04 18:35:30.887009 galileo-db-0.8.0/galileodb/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      215 2020-06-03 11:09:36.000000 galileo-db-0.8.0/galileodb/__init__.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-12-04 18:35:30.887009 galileo-db-0.8.0/galileodb/cli/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2020-06-03 11:09:36.000000 galileo-db-0.8.0/galileodb/cli/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1651 2020-10-11 21:49:48.000000 galileo-db-0.8.0/galileodb/cli/manager.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2552 2020-10-18 01:10:54.000000 galileo-db-0.8.0/galileodb/cli/recorder.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1971 2020-10-18 02:10:57.000000 galileo-db-0.8.0/galileodb/db.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1653 2020-11-05 21:44:39.000000 galileo-db-0.8.0/galileodb/factory.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2046 2020-12-04 17:47:49.000000 galileo-db-0.8.0/galileodb/model.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-12-04 18:35:30.887009 galileo-db-0.8.0/galileodb/recorder/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      363 2020-06-03 11:09:36.000000 galileo-db-0.8.0/galileodb/recorder/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3433 2020-10-18 01:10:54.000000 galileo-db-0.8.0/galileodb/recorder/events.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1207 2020-10-26 20:23:51.000000 galileo-db-0.8.0/galileodb/recorder/recorder.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2092 2020-12-04 17:50:36.000000 galileo-db-0.8.0/galileodb/recorder/telemetry.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3559 2020-10-26 20:23:51.000000 galileo-db-0.8.0/galileodb/recorder/traces.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-12-04 18:35:30.887009 galileo-db-0.8.0/galileodb/reporter/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2020-06-03 11:09:36.000000 galileo-db-0.8.0/galileodb/reporter/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      401 2020-06-03 11:09:36.000000 galileo-db-0.8.0/galileodb/reporter/events.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      440 2020-12-04 17:52:06.000000 galileo-db-0.8.0/galileodb/reporter/telemetry.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1015 2020-10-18 01:10:54.000000 galileo-db-0.8.0/galileodb/reporter/traces.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-12-04 18:35:30.887009 galileo-db-0.8.0/galileodb/sql/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2020-06-03 11:09:36.000000 galileo-db-0.8.0/galileodb/sql/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10200 2020-11-05 21:53:03.000000 galileo-db-0.8.0/galileodb/sql/adapter.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-12-04 18:35:30.887009 galileo-db-0.8.0/galileodb/sql/driver/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2020-06-03 11:09:36.000000 galileo-db-0.8.0/galileodb/sql/driver/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1026 2020-06-03 11:09:36.000000 galileo-db-0.8.0/galileodb/sql/driver/mysql.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      208 2020-06-03 11:09:36.000000 galileo-db-0.8.0/galileodb/sql/driver/sqlite.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1320 2020-12-04 17:47:16.000000 galileo-db-0.8.0/galileodb/sql/schema.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5337 2020-11-05 19:42:22.000000 galileo-db-0.8.0/galileodb/trace.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2020-12-04 18:35:30.891009 galileo-db-0.8.0/setup.cfg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1421 2020-12-04 18:33:45.000000 galileo-db-0.8.0/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-12-04 18:35:30.891009 galileo-db-0.8.0/tests/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2020-06-03 11:09:36.000000 galileo-db-0.8.0/tests/__init__.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-12-04 18:35:30.891009 galileo-db-0.8.0/tests/recorder/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2020-06-03 11:09:36.000000 galileo-db-0.8.0/tests/recorder/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4539 2020-06-26 10:59:16.000000 galileo-db-0.8.0/tests/recorder/test_events.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2665 2020-12-04 17:55:52.000000 galileo-db-0.8.0/tests/recorder/test_telemetry.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3082 2020-10-26 20:23:51.000000 galileo-db-0.8.0/tests/recorder/test_traces.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-12-04 18:35:30.891009 galileo-db-0.8.0/tests/reporter/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2020-10-18 01:10:54.000000 galileo-db-0.8.0/tests/reporter/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2125 2020-10-18 01:10:54.000000 galileo-db-0.8.0/tests/reporter/test_traces.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-12-04 18:35:30.891009 galileo-db-0.8.0/tests/sql/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2020-06-03 11:09:36.000000 galileo-db-0.8.0/tests/sql/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3446 2020-10-11 21:49:48.000000 galileo-db-0.8.0/tests/sql/adapter.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2020-12-04 18:35:30.891009 galileo-db-0.8.0/tests/sql/driver/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2020-06-03 11:09:36.000000 galileo-db-0.8.0/tests/sql/driver/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      583 2020-06-03 11:09:36.000000 galileo-db-0.8.0/tests/sql/driver/test_sqlite.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7128 2020-12-04 17:58:27.000000 galileo-db-0.8.0/tests/test_db.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6266 2020-10-18 02:53:06.000000 galileo-db-0.8.0/tests/test_trace.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2949 2020-10-18 01:10:54.000000 galileo-db-0.8.0/tests/testutils.py
```

### Comparing `galileo-db-0.7.0/galileo_db.egg-info/SOURCES.txt` & `galileo-db-0.8.0/galileo_db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galileo-db-0.7.0/galileodb/cli/manager.py` & `galileo-db-0.8.0/galileodb/cli/manager.py`

 * *Files identical despite different names*

### Comparing `galileo-db-0.7.0/galileodb/cli/recorder.py` & `galileo-db-0.8.0/galileodb/cli/recorder.py`

 * *Files identical despite different names*

### Comparing `galileo-db-0.7.0/galileodb/db.py` & `galileo-db-0.8.0/galileodb/db.py`

 * *Files identical despite different names*

### Comparing `galileo-db-0.7.0/galileodb/factory.py` & `galileo-db-0.8.0/galileodb/factory.py`

 * *Files identical despite different names*

### Comparing `galileo-db-0.7.0/galileodb/model.py` & `galileo-db-0.8.0/galileodb/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
 class Telemetry(NamedTuple):
     timestamp: float
     metric: str
     node: str
     value: float
     exp_id: str
+    subsystem: str = None
 
 
 class NodeInfo(NamedTuple):
     node: str
     data: Dict[str, str]
     exp_id: str
```

### Comparing `galileo-db-0.7.0/galileodb/recorder/events.py` & `galileo-db-0.8.0/galileodb/recorder/events.py`

 * *Files identical despite different names*

### Comparing `galileo-db-0.7.0/galileodb/recorder/recorder.py` & `galileo-db-0.8.0/galileodb/recorder/recorder.py`

 * *Files identical despite different names*

### Comparing `galileo-db-0.7.0/galileodb/recorder/telemetry.py` & `galileo-db-0.8.0/galileodb/recorder/telemetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,19 +43,15 @@
             # than having the try/except block
             if t.metric == 'status':
                 val = 1 if t.value == 'true' else 0
             else:
                 logger.error('Could not convert value "%s" of metric "%s"', t.value, t.metric)
                 return
 
-        metric = t.metric
-        if t.subsystem:
-            metric += '/' + t.subsystem
-
-        self.buffer.append(GalileoTelemetry(float(t.timestamp), t.metric, t.node, val, self.exp_id))
+        self.buffer.append(GalileoTelemetry(float(t.timestamp), t.metric, t.node, val, self.exp_id, t.subsystem))
 
         self.i = (self.i + 1) % self.flush_every
         if self.i == 0:
             self._flush()
 
     def _flush(self):
         if not self.buffer:
```

### Comparing `galileo-db-0.7.0/galileodb/recorder/traces.py` & `galileo-db-0.8.0/galileodb/recorder/traces.py`

 * *Files identical despite different names*

### Comparing `galileo-db-0.7.0/galileodb/reporter/traces.py` & `galileo-db-0.8.0/galileodb/reporter/traces.py`

 * *Files identical despite different names*

### Comparing `galileo-db-0.7.0/galileodb/sql/adapter.py` & `galileo-db-0.8.0/galileodb/sql/adapter.py`

 * *Files identical despite different names*

### Comparing `galileo-db-0.7.0/galileodb/sql/driver/mysql.py` & `galileo-db-0.8.0/galileodb/sql/driver/mysql.py`

 * *Files identical despite different names*

### Comparing `galileo-db-0.7.0/galileodb/sql/schema.sql` & `galileo-db-0.8.0/galileodb/sql/schema.sql`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 );
 
 CREATE TABLE IF NOT EXISTS telemetry
 (
     EXP_ID    VARCHAR(100) NOT NULL,
     TIMESTAMP DOUBLE       NOT NULL,
     METRIC    varchar(100) NOT NULL,
-    NODE      varchar(50) NOT NULL,
+    SUBSYSTEM varchar(100),
+    NODE      varchar(50)  NOT NULL,
     VALUE     DOUBLE       NOT NULL
 );
 
 CREATE TABLE IF NOT EXISTS events
 (
     EXP_ID      VARCHAR(100) NOT NULL,
     TIMESTAMP   DOUBLE       NOT NULL,
```

### Comparing `galileo-db-0.7.0/galileodb/trace.py` & `galileo-db-0.8.0/galileodb/trace.py`

 * *Files identical despite different names*

### Comparing `galileo-db-0.7.0/setup.py` & `galileo-db-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     with open("requirements.txt", "r") as fh:
         install_requires = [line for line in fh.read().split(os.linesep) if line and not line.startswith('git')]
 except FileNotFoundError:
     install_requires = []
 
 setuptools.setup(
     name="galileo-db",
-    version="0.7.0",
+    version="0.8.0",
     author="Thomas Rausch",
     author_email="t.rausch@dsg.tuwien.ac.at",
     description="Galileo DB: Gateway and client tools for the Galileo Experiment DB",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/edgerun/galileo-db",
     packages=setuptools.find_packages(),
```

### Comparing `galileo-db-0.7.0/tests/recorder/test_events.py` & `galileo-db-0.8.0/tests/recorder/test_events.py`

 * *Files identical despite different names*

### Comparing `galileo-db-0.7.0/tests/recorder/test_telemetry.py` & `galileo-db-0.8.0/tests/recorder/test_telemetry.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,21 @@
 
     @timeout_decorator.timeout(5)
     def test_recorder_records_correctly(self):
         recorder = ExperimentTelemetryRecorder(self.redis_resource.rds, self.db_resource.db, 'unittest', flush_every=1)
 
         recorder._record(Telemetry('1.0', '31', 'node1', 'cpu'))
         recorder._record(Telemetry('2.0', '32', 'node2', 'cpu'))
+        recorder._record(Telemetry('3.0', '33', 'node2', 'rx', 'eth0'))
 
         records = self.db_resource.sql.fetchall('SELECT * FROM `telemetry` WHERE EXP_ID = "unittest"')
-        self.assertEqual(2, len(records))
-        self.assertEqual(('unittest', 1.0, 'cpu', 'node1', 31.0), records[0])
-        self.assertEqual(('unittest', 2.0, 'cpu', 'node2', 32.0), records[1])
+        self.assertEqual(3, len(records))
+        self.assertEqual(('unittest', 1.0, 'cpu', None, 'node1', 31.0), records[0])
+        self.assertEqual(('unittest', 2.0, 'cpu', None, 'node2', 32.0), records[1])
+        self.assertEqual(('unittest', 3.0, 'rx', 'eth0', 'node2', 33.0), records[2])
 
     @timeout_decorator.timeout(5)
     def test_publish_non_float_value_does_not_break_recorder(self):
         recorder = ExperimentTelemetryRecorder(self.redis_resource.rds, self.db_resource.db, 'unittest')
         recorder.start()
         time.sleep(0.5)
 
@@ -53,13 +55,13 @@
             self.reporter.report(Telemetry('7', '37', 'node2', 'cpu'))
         finally:
             time.sleep(0.5)
             recorder.stop(timeout=2)
 
         records = self.db_resource.sql.fetchall('SELECT * FROM `telemetry` WHERE EXP_ID = "unittest"')
         self.assertEqual(2, len(records))
-        self.assertEqual(('unittest', 5.0, 'cpu', 'node1', 35.0), records[0])
-        self.assertEqual(('unittest', 7.0, 'cpu', 'node2', 37.0), records[1])
+        self.assertEqual(('unittest', 5.0, 'cpu', None, 'node1', 35.0), records[0])
+        self.assertEqual(('unittest', 7.0, 'cpu', None, 'node2', 37.0), records[1])
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `galileo-db-0.7.0/tests/recorder/test_traces.py` & `galileo-db-0.8.0/tests/recorder/test_traces.py`

 * *Files identical despite different names*

### Comparing `galileo-db-0.7.0/tests/reporter/test_traces.py` & `galileo-db-0.8.0/tests/reporter/test_traces.py`

 * *Files identical despite different names*

### Comparing `galileo-db-0.7.0/tests/sql/adapter.py` & `galileo-db-0.8.0/tests/sql/adapter.py`

 * *Files identical despite different names*

### Comparing `galileo-db-0.7.0/tests/sql/driver/test_sqlite.py` & `galileo-db-0.8.0/tests/sql/driver/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `galileo-db-0.7.0/tests/test_db.py` & `galileo-db-0.8.0/tests/test_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,32 +79,35 @@
         self.assertEqual(self.db.get_experiment('expid8').end, 100)
 
     def test_save_and_get_telemetry(self):
         telemetry = [
             Telemetry(1, 'cpu', 'n1', 32, 'expid1'),
             Telemetry(2, 'cpu', 'n1', 33, 'expid1'),
             Telemetry(3, 'cpu', 'n1', 31, 'expid2'),
+            Telemetry(4, 'rx', 'n1', 32, 'expid2', 'eth0'),
         ]
 
         self.db.save_telemetry(telemetry)
 
         actual = self.db.get_telemetry('expid1')
         self.assertEqual(2, len(actual))
         self.assertEqual(telemetry[0], actual[0])
         self.assertEqual(telemetry[1], actual[1])
 
         actual = self.db.get_telemetry('expid2')
-        self.assertEqual(1, len(actual))
+        self.assertEqual(2, len(actual))
         self.assertEqual(telemetry[2], actual[0])
+        self.assertEqual(telemetry[3], actual[1])
 
         actual = self.db.get_telemetry()
-        self.assertEqual(3, len(actual))
+        self.assertEqual(4, len(actual))
         self.assertEqual(telemetry[0], actual[0])
         self.assertEqual(telemetry[1], actual[1])
         self.assertEqual(telemetry[2], actual[2])
+        self.assertEqual(telemetry[3], actual[3])
 
     def test_save_and_touch_and_get_traces(self):
         traces = [
             RequestTrace('req1', 'c1', 's1', 1.1, 1.2, 1.3, server='h1', status=200),
             RequestTrace('req2', 'c2', 's2', 2.1, 2.2, 2.3, server='h2', status=200),
             RequestTrace('req3', 'c3', 's1', 3.1, 3.2, 3.3, server='h1', status=200, response='time=123'),
             RequestTrace('req4', 'c1', 's1', 4.1, 4.2, 4.3, server='h1', status=200),
```

### Comparing `galileo-db-0.7.0/tests/test_trace.py` & `galileo-db-0.8.0/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `galileo-db-0.7.0/tests/testutils.py` & `galileo-db-0.8.0/tests/testutils.py`

 * *Files identical despite different names*

