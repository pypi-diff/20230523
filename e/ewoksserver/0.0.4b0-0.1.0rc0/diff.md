# Comparing `tmp/ewoksserver-0.0.4b0.tar.gz` & `tmp/ewoksserver-0.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksserver-0.0.4b0.tar", last modified: Thu Sep 15 11:30:46 2022, max compression
+gzip compressed data, was "dist/ewoksserver-0.1.0rc0.tar", last modified: Tue May 23 16:58:12 2023, max compression
```

## Comparing `ewoksserver-0.0.4b0.tar` & `ewoksserver-0.1.0rc0.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2211 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1479 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1475 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/src/ewoksserver/
--rw-rw-rw-   0 root         (0) root         (0)       27 2022-09-15 11:26:58.000000 ewoksserver-0.0.4b0/src/ewoksserver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/src/ewoksserver/events/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-15 11:30:39.000000 ewoksserver-0.0.4b0/src/ewoksserver/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/events/ewoks_events.py
--rw-rw-rw-   0 root         (0) root         (0)     2415 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/events/websocket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/
--rw-rw-rw-   0 root         (0) root         (0)      731 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9671 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/binary/
--rw-rw-rw-   0 root         (0) root         (0)      413 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/binary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1140 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/binary/icons.py
--rw-rw-rw-   0 root         (0) root         (0)     3834 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/binary/resource.py
--rw-rw-rw-   0 root         (0) root         (0)     3472 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/binary/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/data/
--rw-rw-rw-   0 root         (0) root         (0)       74 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/data/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-15 11:30:39.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/data/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/data/icons/default.png
--rw-rw-rw-   0 root         (0) root         (0)      133 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/data/icons/graphInput.svg
--rw-rw-rw-   0 root         (0) root         (0)      149 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/data/icons/graphOutput.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/data/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-15 11:30:39.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/data/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/data/tasks/ewokscore.tests.examples.tasks.sumlist.SumList.json
--rw-rw-rw-   0 root         (0) root         (0)      304 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/data/tasks/ewokscore.tests.examples.tasks.sumtask.SumTask.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/data/workflows/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-15 11:30:39.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/data/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12315 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/data/workflows/demo.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/events/
--rw-rw-rw-   0 root         (0) root         (0)      360 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      732 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/events/resource.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/json/
--rw-rw-rw-   0 root         (0) root         (0)      952 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/json/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4691 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/json/resource.py
--rw-rw-rw-   0 root         (0) root         (0)     2933 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/json/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     3332 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/json/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3371 2022-09-15 11:26:58.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/json/workflows.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/resources/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5319 2022-09-15 11:26:58.000000 ewoksserver-0.0.4b0/src/ewoksserver/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/src/ewoksserver/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-15 11:30:39.000000 ewoksserver-0.0.4b0/src/ewoksserver/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3053 2022-09-15 11:26:58.000000 ewoksserver-0.0.4b0/src/ewoksserver/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/src/ewoksserver/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)      292 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/tests/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2730 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/tests/data/icon1.png
--rw-rw-rw-   0 root         (0) root         (0)      133 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/tests/data/icon1.svg
--rw-rw-rw-   0 root         (0) root         (0)     1698 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/tests/data/icon2.png
--rw-rw-rw-   0 root         (0) root         (0)      493 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/tests/data/icon2.svg
--rw-rw-rw-   0 root         (0) root         (0)       91 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/tests/dummy_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2041 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/tests/test_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3137 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/tests/test_events.py
--rw-rw-rw-   0 root         (0) root         (0)     1797 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/tests/test_execute.py
--rw-rw-rw-   0 root         (0) root         (0)     2612 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/tests/test_icons.py
--rw-rw-rw-   0 root         (0) root         (0)     5632 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/tests/test_websocket_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     4013 2022-09-15 07:03:18.000000 ewoksserver-0.0.4b0/src/ewoksserver/tests/test_workflows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/src/ewoksserver.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2211 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/src/ewoksserver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2176 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/src/ewoksserver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/src/ewoksserver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/src/ewoksserver.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      316 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/src/ewoksserver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-09-15 11:30:46.000000 ewoksserver-0.0.4b0/src/ewoksserver.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1468 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1439 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-05-23 16:55:36.000000 ewoksserver-0.1.0rc0/src/ewoksserver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/events/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 16:58:06.000000 ewoksserver-0.1.0rc0/src/ewoksserver/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/events/ewoks_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/events/websocket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      731 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9807 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/binary/
+-rw-rw-rw-   0 root         (0) root         (0)      413 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/binary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/binary/icons.py
+-rw-rw-rw-   0 root         (0) root         (0)     3834 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/binary/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     3472 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/binary/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 16:58:06.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/icons/default.png
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/icons/graphInput.svg
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/icons/graphOutput.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3070 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/icons/sum.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 16:58:06.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/tasks/ewokscore.tests.examples.tasks.sumlist.SumList.json
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/tasks/ewokscore.tests.examples.tasks.sumtask.SumTask.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 16:58:06.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12315 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/workflows/demo.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/events/
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      880 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/events/resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4691 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     3052 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3332 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3371 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/resources/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5963 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 16:58:06.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3053 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2730 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/data/icon1.png
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/data/icon1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1698 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/data/icon2.png
+-rw-rw-rw-   0 root         (0) root         (0)      493 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/data/icon2.svg
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/dummy_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2040 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3137 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2612 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_icons.py
+-rw-rw-rw-   0 root         (0) root         (0)     5844 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_websocket_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     4013 2023-05-23 07:03:09.000000 ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_workflows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2221 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      355 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-23 16:58:12.000000 ewoksserver-0.1.0rc0/src/ewoksserver.egg-info/top_level.txt
```

### Comparing `ewoksserver-0.0.4b0/LICENSE.md` & `ewoksserver-0.1.0rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.0.4b0/PKG-INFO` & `ewoksserver-0.1.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksserver
-Version: 0.0.4b0
+Version: 0.1.0rc0
 Summary: Backend for ewoksweb
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksserver
 Author: ESRF
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksserver
 Project-URL: Documentation, https://workflow.gitlab-pages.esrf.fr/ewoks/ewoksserver
 Project-URL: Tracker, https://gitlab.esrf.fr/workflow/ewoks/ewoksserver/issues
@@ -26,15 +26,15 @@
 It serves as a backend for [ewoksweb](https://ewoksweb.readthedocs.io/) and emits ewoks execution events over websocket.
 
 ## Development
 
 Install from source
 
 ```bash
-python3 -m pip install -e .[dev]
+pip install -e .[dev]
 ```
 
 Run tests
 
 ```bash
 pytest
 ```
```

### Comparing `ewoksserver-0.0.4b0/README.md` & `ewoksserver-0.1.0rc0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 It serves as a backend for [ewoksweb](https://ewoksweb.readthedocs.io/) and emits ewoks execution events over websocket.
 
 ## Development
 
 Install from source
 
 ```bash
-python3 -m pip install -e .[dev]
+pip install -e .[dev]
 ```
 
 Run tests
 
 ```bash
 pytest
 ```
```

### Comparing `ewoksserver-0.0.4b0/setup.cfg` & `ewoksserver-0.1.0rc0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -21,18 +21,19 @@
 	=src
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	flask
 	flask-restful
 	flask-cors
-	flask-socketio <=5.2  #until MR1877 is deployed
+	flask-socketio
 	flask-apispec
+	werkzeug <2.3  # until flask-socketio issue #1982 is solved
 	simple-websocket
-	ewokscore >=0.1.1
+	ewokscore >=0.3.2
 	ewoksjob[worker]
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = *.png, *.svg, *.json
@@ -47,25 +48,21 @@
 dev = 
 	%(test)s
 	black >=22
 	flake8 >=4
 doc = 
 	%(test)s
 	sphinx >=4.5
+	sphinx-autodoc-typehints >=1.16
 	sphinxcontrib-redoc
 
 [options.entry_points]
 console_scripts = 
 	ewoks-server=ewoksserver.server:main
 
-[build_sphinx]
-project = ewoksserver
-version = attr: ewoksserver.__version__
-source-dir = ./doc
-
 [flake8]
 ignore = E501, E203, W503
 max-line-length = 88
 exclude = 
 	.eggs
 
 [coverage:run]
```

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/events/ewoks_events.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/events/ewoks_events.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/events/websocket.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/events/websocket.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from datetime import datetime
 import threading
+from typing import Optional
 
 import flask
 from flask import copy_current_request_context
 from flask_socketio import SocketIO
 from flask_socketio import emit
 
 from .ewoks_events import reader_context
@@ -47,47 +48,53 @@
 
 class EwoksEventEmitter:
     def __init__(self) -> None:
         self._stop_event = threading.Event()
         self._thread = None
         self._counter = 0
 
-    def connect(self):
+    def connect(self) -> None:
         self._counter += 1
         self.start()
 
-    def disconnect(self):
+    def disconnect(self) -> None:
         self._counter = max(self._counter - 1, 0)
         if self._counter == 0:
             self.stop(timeout=3)
 
-    def is_running(self):
-        return self._thread is not None
+    def is_running(self) -> bool:
+        return self._is_running(self._thread)
 
-    def start(self):
-        if self._thread is not None:
+    @staticmethod
+    def _is_running(thread: Optional[threading.Thread] = None) -> bool:
+        return thread is not None and thread.is_alive()
+
+    def start(self) -> None:
+        if self.is_running():
             return
 
         # Flask context's have thread affinity
         @copy_current_request_context
         @copy_current_app_context
         def main():
             self._main()
 
         self._stop_event.clear()
-        self._thread = threading.Thread(target=main, daemon=True)
-        self._thread.start()
-
-    def stop(self, timeout: float = None):
-        if self._thread is None:
+        thread = threading.Thread(target=main, daemon=True)
+        thread.start()
+        self._thread = thread
+
+    def stop(self, timeout: Optional[float] = None) -> None:
+        thread = self._thread
+        if not self._is_running(thread):
             return
         self._stop_event.set()
-        self._thread.join(timeout=timeout)
+        thread.join(timeout=timeout)
 
-    def _main(self):
+    def _main(self) -> None:
         try:
             with reader_context() as reader:
                 if reader is None:
                     return
                 starttime = datetime.now().astimezone()
                 for event in reader.wait_events(
                     starttime=starttime, stop_event=self._stop_event
```

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/resources/__init__.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/resources/api.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/resources/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,14 +301,19 @@
         func = marshal_with(
             ErrorSchema,
             code=403,
             description=f"no permission to write the {resource_type}",
         )(func)
         func = marshal_with(
             ErrorSchema,
+            code=404,
+            description="module not found",
+        )(func)
+        func = marshal_with(
+            ErrorSchema,
             code=409,
             description=f"requested {resource_type} already exists",
         )(func)
         return func
 
     return wrapper
```

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/resources/binary/icons.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/resources/binary/icons.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/resources/binary/resource.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/resources/binary/resource.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/resources/binary/utils.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/resources/binary/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/resources/data/icons/default.png` & `ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/icons/default.png`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/resources/data/workflows/demo.json` & `ewoksserver-0.1.0rc0/src/ewoksserver/resources/data/workflows/demo.json`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/resources/events/resource.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/resources/events/resource.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 from typing import List
+
+from ewoksutils import event_utils
+
 from ..utils import Resource
 from .. import api
 from ...events.ewoks_events import reader_context
 
 
 class ExecutionEvents(Resource):
     @api.get_ewoks_events()
@@ -14,9 +17,11 @@
             if reader is None:
                 raise RuntimeError("server not configured for ewoks events")
             for event in reader.get_events(**filters):
                 if event["job_id"] != job_id:
                     job_id = event["job_id"]
                     job = list()
                     jobs.append(job)
+                if "engine" in event_utils.FIELD_TYPES:
+                    event["binding"] = event["engine"]
                 job.append(event)
         return {"jobs": jobs}, 200
```

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/resources/json/__init__.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/resources/json/resource.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/resource.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/resources/json/tasks.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,20 @@
     def get_identifier(
         self, resource: resource.ResourceContentType
     ) -> resource.ResourceIdentifierType:
         return resource["task_identifier"]
 
     @api.discover_resources("task")
     def post(self, modules=None, task_type="class"):
-        tasks = list(
-            task_discovery.discover_tasks_from_modules(*modules, task_type=task_type)
-        )
+        try:
+            tasks = task_discovery.discover_tasks_from_modules(
+                *modules, task_type=task_type
+            )
+        except ModuleNotFoundError as e:
+            return self.make_response(404, message=str(e))
         for _resource in tasks:
             self._default_task_properties(_resource)
             response, code = self.save_resource(_resource, error_on_exists=True)
             if code != 200:
                 return response, code
         tasks = [desc["task_identifier"] for desc in tasks]
         return self.make_response(200, identifiers=tasks)
```

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/resources/json/utils.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/resources/json/workflows.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/resources/json/workflows.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/server.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,18 +74,29 @@
     adict = app.config.get("EWOKS")
     if adict:
         print(f"\nEWOKS:\n {pformat(adict)}\n")
     else:
         print("\nEWOKS:\n Not configured (no ewoks execution events)\n")
 
 
+def print_serve_message(app, port: Optional[int] = None) -> None:
+    host = "127.0.0.1"
+    if port is None:
+        server_name = app.config["SERVER_NAME"]
+        if server_name and ":" in server_name:
+            port = int(server_name.rsplit(":", 1)[1])
+        else:
+            port = 5000
+    print("\nTo start editing workflows, open this link in a browser:\n")
+    print(f"    http://{host}:{port}\n")
+
+
 def set_log_level(app: Optional[flask.Flask] = None, log_level=logging.WARNING):
-    if app is None:
-        logging.basicConfig(level=log_level)
-    else:
+    logging.basicConfig(level=log_level)
+    if app is not None:
         app.logger.setLevel(log_level)
 
 
 def add_socket(app: flask.Flask) -> SocketIO:
     socketio = SocketIO(app, cors_allowed_origins="*")
     add_events(socketio)
     return socketio
@@ -173,26 +184,35 @@
     parser.add_argument(
         "-s",
         "--spec-filename",
         dest="spec_filename",
         type=str,
         help="Save the Swagger docs as JSON",
     )
+    parser.add_argument(
+        "--without-events",
+        action="store_true",
+        help="Without websocket events",
+    )
 
     args = parser.parse_args(argv[1:])
     log_level = getattr(logging, args.log_level)
 
     app, _, apidoc = create_app(
         configuration=args.configuration, resource_directory=args.resource_directory
     )
     if args.spec_filename:
         save_apidoc(apidoc, args.spec_filename)
         return
-    socketio = add_socket(app)
+    if args.without_events:
+        socketio = None
+    else:
+        socketio = add_socket(app)
     set_log_level(log_level=log_level)
 
     print_config(app)
+    print_serve_message(app, port=args.port)
     run_app(app, socketio=socketio, port=args.port)
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/tests/conftest.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/tests/data/icon1.png` & `ewoksserver-0.1.0rc0/src/ewoksserver/tests/data/icon1.png`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/tests/data/icon2.png` & `ewoksserver-0.1.0rc0/src/ewoksserver/tests/data/icon2.png`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/tests/test_data.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         default_workflow_identifiers,
     )
 
 
 def assert_resource_fallback(
     utils, user_root, category, existing, nonexisting, user, extension, all_resources
 ):
-    user_root = Path(user_root).absolute()
+    user_root = Path(user_root).resolve()
     user_icons_root = utils.root_url(user_root, category)
     default_icons_root = utils.root_url(DEFAULT_ROOT, category)
 
     source = (default_icons_root / existing).with_suffix(extension)
     dest = (user_icons_root / user).with_suffix(extension)
     user_icons_root.mkdir()
     shutil.copyfile(source, dest)
```

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/tests/test_events.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/tests/test_execute.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/tests/test_icons.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_icons.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/tests/test_tasks.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -144,14 +144,19 @@
     assert set(data["identifiers"]) == expected
 
     response = rest_client.post("/tasks/discover", json={"modules": [module]})
     data = response.get_json()
     assert response.status_code == 409, data
     assert "already exists" in data["message"]
 
+    response = rest_client.post("/tasks/discover", json={"modules": ["not_a_module"]})
+    data = response.get_json()
+    assert response.status_code == 404, data
+    assert "No module named" in data["message"]
+
 
 def test_task_descriptions(rest_client, default_task_identifiers):
     response = rest_client.get("/tasks/descriptions")
     data = response.get_json()
     assert response.status_code == 200
     default_descriptions = [
         desc
```

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/tests/test_websocket_connection.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver/tests/test_workflows.py` & `ewoksserver-0.1.0rc0/src/ewoksserver/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver.egg-info/PKG-INFO` & `ewoksserver-0.1.0rc0/src/ewoksserver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksserver
-Version: 0.0.4b0
+Version: 0.1.0rc0
 Summary: Backend for ewoksweb
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksserver
 Author: ESRF
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksserver
 Project-URL: Documentation, https://workflow.gitlab-pages.esrf.fr/ewoks/ewoksserver
 Project-URL: Tracker, https://gitlab.esrf.fr/workflow/ewoks/ewoksserver/issues
@@ -26,15 +26,15 @@
 It serves as a backend for [ewoksweb](https://ewoksweb.readthedocs.io/) and emits ewoks execution events over websocket.
 
 ## Development
 
 Install from source
 
 ```bash
-python3 -m pip install -e .[dev]
+pip install -e .[dev]
 ```
 
 Run tests
 
 ```bash
 pytest
 ```
```

### Comparing `ewoksserver-0.0.4b0/src/ewoksserver.egg-info/SOURCES.txt` & `ewoksserver-0.1.0rc0/src/ewoksserver.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 src/ewoksserver/resources/binary/resource.py
 src/ewoksserver/resources/binary/utils.py
 src/ewoksserver/resources/data/__init__.py
 src/ewoksserver/resources/data/icons/__init__.py
 src/ewoksserver/resources/data/icons/default.png
 src/ewoksserver/resources/data/icons/graphInput.svg
 src/ewoksserver/resources/data/icons/graphOutput.svg
+src/ewoksserver/resources/data/icons/sum.png
 src/ewoksserver/resources/data/tasks/__init__.py
 src/ewoksserver/resources/data/tasks/ewokscore.tests.examples.tasks.sumlist.SumList.json
 src/ewoksserver/resources/data/tasks/ewokscore.tests.examples.tasks.sumtask.SumTask.json
 src/ewoksserver/resources/data/workflows/__init__.py
 src/ewoksserver/resources/data/workflows/demo.json
 src/ewoksserver/resources/events/__init__.py
 src/ewoksserver/resources/events/resource.py
```

