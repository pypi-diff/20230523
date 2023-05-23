# Comparing `tmp/pyinflux3-cli-0.9.0.tar.gz` & `tmp/pyinflux3-cli-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinflux3-cli-0.9.0.tar", last modified: Mon May 22 12:56:39 2023, max compression
+gzip compressed data, was "pyinflux3-cli-0.9.1.tar", last modified: Tue May 23 11:36:15 2023, max compression
```

## Comparing `pyinflux3-cli-0.9.0.tar` & `pyinflux3-cli-0.9.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:39.098388 pyinflux3-cli-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-22 12:56:39.098388 pyinflux3-cli-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-22 12:56:32.000000 pyinflux3-cli-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:39.098388 pyinflux3-cli-0.9.0/influxdb_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:32.000000 pyinflux3-cli-0.9.0/influxdb_cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7638 2023-05-22 12:56:32.000000 pyinflux3-cli-0.9.0/influxdb_cli/influx3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:39.098388 pyinflux3-cli-0.9.0/pyinflux3_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-22 12:56:39.000000 pyinflux3-cli-0.9.0/pyinflux3_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-22 12:56:39.000000 pyinflux3-cli-0.9.0/pyinflux3_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 12:56:39.000000 pyinflux3-cli-0.9.0/pyinflux3_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-22 12:56:39.000000 pyinflux3-cli-0.9.0/pyinflux3_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-22 12:56:39.000000 pyinflux3-cli-0.9.0/pyinflux3_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 12:56:39.000000 pyinflux3-cli-0.9.0/pyinflux3_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-22 12:56:32.000000 pyinflux3-cli-0.9.0/setup-cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 12:56:39.098388 pyinflux3-cli-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:36:15.128013 pyinflux3-cli-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-23 11:36:15.128013 pyinflux3-cli-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-23 11:36:07.000000 pyinflux3-cli-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:36:15.128013 pyinflux3-cli-0.9.1/influxdb_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:36:07.000000 pyinflux3-cli-0.9.1/influxdb_cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7638 2023-05-23 11:36:07.000000 pyinflux3-cli-0.9.1/influxdb_cli/influx3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:36:15.128013 pyinflux3-cli-0.9.1/pyinflux3_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-23 11:36:15.000000 pyinflux3-cli-0.9.1/pyinflux3_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-23 11:36:15.000000 pyinflux3-cli-0.9.1/pyinflux3_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 11:36:15.000000 pyinflux3-cli-0.9.1/pyinflux3_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-23 11:36:15.000000 pyinflux3-cli-0.9.1/pyinflux3_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-23 11:36:15.000000 pyinflux3-cli-0.9.1/pyinflux3_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 11:36:15.000000 pyinflux3-cli-0.9.1/pyinflux3_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-23 11:36:07.000000 pyinflux3-cli-0.9.1/setup-cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 11:36:15.128013 pyinflux3-cli-0.9.1/setup.cfg
```

### Comparing `pyinflux3-cli-0.9.0/PKG-INFO` & `pyinflux3-cli-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3-cli
-Version: 0.9.0
+Version: 0.9.1
 Summary: Community Python client for InfluxDB IOx (CLI)
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyinflux3-cli-0.9.0/README.md` & `pyinflux3-cli-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pyinflux3-cli-0.9.0/influxdb_cli/influx3.py` & `pyinflux3-cli-0.9.1/influxdb_cli/influx3.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-cli-0.9.0/pyinflux3_cli.egg-info/PKG-INFO` & `pyinflux3-cli-0.9.1/pyinflux3_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3-cli
-Version: 0.9.0
+Version: 0.9.1
 Summary: Community Python client for InfluxDB IOx (CLI)
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyinflux3-cli-0.9.0/setup-cli.py` & `pyinflux3-cli-0.9.1/setup-cli.py`

 * *Files identical despite different names*

