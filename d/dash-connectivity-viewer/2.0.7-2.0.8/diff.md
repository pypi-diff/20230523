# Comparing `tmp/dash-connectivity-viewer-2.0.7.tar.gz` & `tmp/dash-connectivity-viewer-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash-connectivity-viewer-2.0.7.tar", last modified: Thu May 18 22:44:43 2023, max compression
+gzip compressed data, was "dash-connectivity-viewer-2.0.8.tar", last modified: Tue May 23 21:40:20 2023, max compression
```

## Comparing `dash-connectivity-viewer-2.0.7.tar` & `dash-connectivity-viewer-2.0.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-18 22:44:43.024444 dash-connectivity-viewer-2.0.7/
--rw-r--r--   0 caseysm    (501) staff       (20)     1842 2023-05-09 18:49:42.000000 dash-connectivity-viewer-2.0.7/LICENSE.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       71 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.7/MANIFEST.in
--rw-r--r--   0 caseysm    (501) staff       (20)      525 2023-05-18 22:44:43.024247 dash-connectivity-viewer-2.0.7/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)      216 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.7/README.md
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-18 22:44:43.009168 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/
--rw-r--r--   0 caseysm    (501) staff       (20)       22 2023-05-18 22:44:29.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/__init__.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-18 22:44:43.013706 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_connectivity/
--rw-r--r--   0 caseysm    (501) staff       (20)      568 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_connectivity/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    24594 2023-05-13 00:17:14.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_connectivity/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)     5453 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_connectivity/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3461 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py
--rw-r--r--   0 caseysm    (501) staff       (20)     6156 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py
--rw-r--r--   0 caseysm    (501) staff       (20)       82 2023-03-18 18:57:32.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_connectivity/external_stylesheets.py
--rw-r--r--   0 caseysm    (501) staff       (20)    20408 2023-05-14 19:13:50.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_connectivity/layout.py
--rw-r--r--   0 caseysm    (501) staff       (20)     4439 2023-05-12 23:41:48.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-18 22:44:43.015789 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_table/
--rw-r--r--   0 caseysm    (501) staff       (20)      711 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_table/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    14472 2023-05-14 19:13:28.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_table/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1347 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_table/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)      210 2023-02-08 23:15:09.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_table/ct_utils.py
--rw-r--r--   0 caseysm    (501) staff       (20)    14841 2023-05-14 19:13:16.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_table/layout.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-18 22:44:43.020681 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/
--rw-r--r--   0 caseysm    (501) staff       (20)       17 2023-04-13 06:43:13.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)     5184 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     2914 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/dash_url_helper.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-18 22:44:43.021501 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/data/
--rw-r--r--   0 caseysm    (501) staff       (20)      144 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/data/height_bounds_v1.npy
--rw-r--r--   0 caseysm    (501) staff       (20)      168 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/data/layer_bounds_v1.npy
--rw-r--r--   0 caseysm    (501) staff       (20)    10170 2023-05-18 22:41:24.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/dataframe_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)      294 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/external_stylesheets.py
--rw-r--r--   0 caseysm    (501) staff       (20)    13477 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/link_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3942 2023-05-14 20:42:12.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/lookup_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)    11370 2023-05-12 23:38:23.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/neuron_data_base.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3756 2023-04-25 19:21:22.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/schema_utils.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3950 2023-05-14 19:10:55.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/table_lookup.py
--rw-r--r--   0 caseysm    (501) staff       (20)      762 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/transform_utils.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-18 22:44:43.023703 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/connectivity_table/
--rw-r--r--   0 caseysm    (501) staff       (20)      591 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/connectivity_table/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    13817 2023-05-14 19:07:55.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/connectivity_table/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)      523 2023-02-08 23:15:09.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/connectivity_table/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     9093 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/connectivity_table/layout.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-18 22:44:43.010181 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer.egg-info/
--rw-r--r--   0 caseysm    (501) staff       (20)      525 2023-05-18 22:44:43.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer.egg-info/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)     1990 2023-05-18 22:44:43.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-05-18 22:44:43.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      180 2023-05-18 22:44:43.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer.egg-info/requires.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       25 2023-05-18 22:44:43.000000 dash-connectivity-viewer-2.0.7/dash_connectivity_viewer.egg-info/top_level.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      179 2023-05-18 22:42:04.000000 dash-connectivity-viewer-2.0.7/requirements.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-05-18 22:44:43.024508 dash-connectivity-viewer-2.0.7/setup.cfg
--rw-r--r--   0 caseysm    (501) staff       (20)     1153 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.7/setup.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-23 21:40:20.171553 dash-connectivity-viewer-2.0.8/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1842 2023-05-09 18:49:42.000000 dash-connectivity-viewer-2.0.8/LICENSE.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       71 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.8/MANIFEST.in
+-rw-r--r--   0 caseysm    (501) staff       (20)      525 2023-05-23 21:40:20.171285 dash-connectivity-viewer-2.0.8/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)      216 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.8/README.md
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-23 21:40:20.078952 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/
+-rw-r--r--   0 caseysm    (501) staff       (20)       22 2023-05-23 21:40:05.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/__init__.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-23 21:40:20.105138 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/
+-rw-r--r--   0 caseysm    (501) staff       (20)      568 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    24594 2023-05-13 00:17:14.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     5453 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3461 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     6156 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py
+-rw-r--r--   0 caseysm    (501) staff       (20)       82 2023-03-18 18:57:32.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/external_stylesheets.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    20408 2023-05-14 19:13:50.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/layout.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     4439 2023-05-12 23:41:48.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-23 21:40:20.128114 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_table/
+-rw-r--r--   0 caseysm    (501) staff       (20)      711 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_table/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    14472 2023-05-14 19:13:28.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_table/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     1347 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_table/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      210 2023-02-08 23:15:09.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_table/ct_utils.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    14841 2023-05-14 19:13:16.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_table/layout.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-23 21:40:20.153782 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/
+-rw-r--r--   0 caseysm    (501) staff       (20)       17 2023-04-13 06:43:13.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     5184 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     2914 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/dash_url_helper.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-23 21:40:20.155417 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/data/
+-rw-r--r--   0 caseysm    (501) staff       (20)      144 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/data/height_bounds_v1.npy
+-rw-r--r--   0 caseysm    (501) staff       (20)      168 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/data/layer_bounds_v1.npy
+-rw-r--r--   0 caseysm    (501) staff       (20)    10170 2023-05-18 22:41:24.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/dataframe_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      294 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/external_stylesheets.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    13477 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/link_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3942 2023-05-14 20:42:12.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/lookup_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    11370 2023-05-12 23:38:23.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/neuron_data_base.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3825 2023-05-23 21:02:51.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/schema_utils.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3950 2023-05-14 19:10:55.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/table_lookup.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      762 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/transform_utils.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-23 21:40:20.169647 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/connectivity_table/
+-rw-r--r--   0 caseysm    (501) staff       (20)      591 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/connectivity_table/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    13817 2023-05-14 19:07:55.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/connectivity_table/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      523 2023-02-08 23:15:09.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/connectivity_table/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     9093 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/connectivity_table/layout.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-23 21:40:20.080234 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer.egg-info/
+-rw-r--r--   0 caseysm    (501) staff       (20)      525 2023-05-23 21:40:20.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)     1990 2023-05-23 21:40:20.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-05-23 21:40:20.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      180 2023-05-23 21:40:20.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer.egg-info/requires.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       25 2023-05-23 21:40:20.000000 dash-connectivity-viewer-2.0.8/dash_connectivity_viewer.egg-info/top_level.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      179 2023-05-18 22:42:04.000000 dash-connectivity-viewer-2.0.8/requirements.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-05-23 21:40:20.171610 dash-connectivity-viewer-2.0.8/setup.cfg
+-rw-r--r--   0 caseysm    (501) staff       (20)     1153 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.8/setup.py
```

### Comparing `dash-connectivity-viewer-2.0.7/LICENSE.txt` & `dash-connectivity-viewer-2.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/PKG-INFO` & `dash-connectivity-viewer-2.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-connectivity-viewer
-Version: 2.0.7
+Version: 2.0.8
 Summary: Dash connectivity viewer for CAVE data
 Home-page: https://github.com/ceesem/dash-connectivity-viewer
 Author: Casey Schneider-Mizell
 Author-email: caseysm@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_connectivity/__init__.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/__init__.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_connectivity/callbacks.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/callbacks.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_connectivity/config.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/config.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_connectivity/layout.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/layout.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_table/__init__.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_table/__init__.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_table/callbacks.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_table/callbacks.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_table/config.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_table/config.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/cell_type_table/layout.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/cell_type_table/layout.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/config.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/config.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/dash_url_helper.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/dash_url_helper.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/dataframe_utilities.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/dataframe_utilities.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/link_utilities.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/link_utilities.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/lookup_utilities.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/lookup_utilities.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/neuron_data_base.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/neuron_data_base.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/schema_utils.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/schema_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 def split_pt_position(pt_position):
     return [f"{pt_position}_{suf}" for suf in SPLIT_SUFFIXES]
 
 _schema_cache = TTLCache(maxsize=128, ttl=86_400)
 def _schema_key(schema_name, client, **kwargs):
     allow_types = kwargs.get('allow_types', ALLOW_COLUMN_TYPES)
-    key = keys.hashkey(schema_name, str(allow_types))
+    key = keys.hashkey(schema_name, str(allow_types), client.datastack_name)
     return key
 
 @cached(cache=_schema_cache, key=_schema_key)
 def get_col_info(schema_name, client, spatial_point='BoundSpatialPoint', allow_types=ALLOW_COLUMN_TYPES, omit_fields=[]):
     schema = client.schema.schema_definition(schema_name)
     sp_name = f"#/definitions/{spatial_point}"
     n_sp = 0
@@ -80,29 +80,29 @@
         _, extra_cols = get_col_info(meta['schema'], client, allow_types=allow_types, omit_fields=['target_id'])
     pt, add_cols = get_col_info(schema, client, allow_types=allow_types)
     cols = add_cols + extra_cols
     return pt, cols
 
 _metadata_cache = TTLCache(maxsize=128, ttl=86_400)
 def _metadata_key(tn, client, **kwargs):
-    key = keys.hashkey(tn)
+    key = keys.hashkey(tn, client.datastack_name)
     return key
 
 @cached(cache=_metadata_cache, key=_metadata_key)
 def table_metadata(table_name, client, meta=None):
     "Caches getting table metadata"
     if meta is None:
         meta = client.materialize.get_table_metadata(table_name)
     if "schema" not in meta:
         meta["schema"] = meta.get('schema_type')
     return meta
 
 _table_list_cache = TTLCache(maxsize=64, ttl=86_400)
 def _table_list_key(tables, client):
-    key = keys.hashkey('_'.join(tables))
+    key = keys.hashkey('_'.join(tables), client.datastack_name)
     return key
 
 @cached(cache=_table_list_cache, key=_table_list_key)
 def populate_metadata_cache(tables, client):
     all_meta = client.materialize.get_tables_metadata()
     for tn, meta in zip(tables, all_meta):
         table_metadata(tn, client, meta=meta)
```

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/table_lookup.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/table_lookup.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/common/transform_utils.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/common/transform_utils.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/connectivity_table/__init__.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/connectivity_table/__init__.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/connectivity_table/callbacks.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/connectivity_table/callbacks.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/connectivity_table/config.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/connectivity_table/config.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer/connectivity_table/layout.py` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer/connectivity_table/layout.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer.egg-info/PKG-INFO` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-connectivity-viewer
-Version: 2.0.7
+Version: 2.0.8
 Summary: Dash connectivity viewer for CAVE data
 Home-page: https://github.com/ceesem/dash-connectivity-viewer
 Author: Casey Schneider-Mizell
 Author-email: caseysm@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `dash-connectivity-viewer-2.0.7/dash_connectivity_viewer.egg-info/SOURCES.txt` & `dash-connectivity-viewer-2.0.8/dash_connectivity_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.7/setup.py` & `dash-connectivity-viewer-2.0.8/setup.py`

 * *Files identical despite different names*

