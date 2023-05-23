# Comparing `tmp/soos-sca-1.7.9.tar.gz` & `tmp/soos-sca-1.7.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soos-sca-1.7.9.tar", last modified: Wed Mar  8 14:39:23 2023, max compression
+gzip compressed data, was "soos-sca-1.7.9rc1.tar", last modified: Mon Mar  6 17:15:54 2023, max compression
```

## Comparing `soos-sca-1.7.9.tar` & `soos-sca-1.7.9rc1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 14:39:23.233555 soos-sca-1.7.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-08 14:39:04.000000 soos-sca-1.7.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-03-08 14:39:23.233555 soos-sca-1.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-03-08 14:39:04.000000 soos-sca-1.7.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-08 14:39:04.000000 soos-sca-1.7.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-08 14:39:23.233555 soos-sca-1.7.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-08 14:39:04.000000 soos-sca-1.7.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 14:39:23.229555 soos-sca-1.7.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 14:39:23.233555 soos-sca-1.7.9/src/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-08 14:39:04.000000 soos-sca-1.7.9/src/cli/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-08 14:39:04.000000 soos-sca-1.7.9/src/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    77178 2023-03-08 14:39:04.000000 soos-sca-1.7.9/src/cli/soos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 14:39:23.233555 soos-sca-1.7.9/src/soos_sca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-03-08 14:39:23.000000 soos-sca-1.7.9/src/soos_sca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-08 14:39:23.000000 soos-sca-1.7.9/src/soos_sca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 14:39:23.000000 soos-sca-1.7.9/src/soos_sca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-08 14:39:23.000000 soos-sca-1.7.9/src/soos_sca.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-08 14:39:23.000000 soos-sca-1.7.9/src/soos_sca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-08 14:39:23.000000 soos-sca-1.7.9/src/soos_sca.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 14:39:23.233555 soos-sca-1.7.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-03-08 14:39:04.000000 soos-sca-1.7.9/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:15:54.760060 soos-sca-1.7.9rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-06 17:15:37.000000 soos-sca-1.7.9rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-03-06 17:15:54.764060 soos-sca-1.7.9rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-03-06 17:15:37.000000 soos-sca-1.7.9rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-06 17:15:37.000000 soos-sca-1.7.9rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-06 17:15:54.764060 soos-sca-1.7.9rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-06 17:15:37.000000 soos-sca-1.7.9rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:15:54.760060 soos-sca-1.7.9rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:15:54.760060 soos-sca-1.7.9rc1/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-06 17:15:37.000000 soos-sca-1.7.9rc1/src/cli/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-06 17:15:37.000000 soos-sca-1.7.9rc1/src/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77178 2023-03-06 17:15:37.000000 soos-sca-1.7.9rc1/src/cli/soos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:15:54.760060 soos-sca-1.7.9rc1/src/soos_sca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-03-06 17:15:54.000000 soos-sca-1.7.9rc1/src/soos_sca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-06 17:15:54.000000 soos-sca-1.7.9rc1/src/soos_sca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 17:15:54.000000 soos-sca-1.7.9rc1/src/soos_sca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-06 17:15:54.000000 soos-sca-1.7.9rc1/src/soos_sca.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-06 17:15:54.000000 soos-sca-1.7.9rc1/src/soos_sca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-06 17:15:54.000000 soos-sca-1.7.9rc1/src/soos_sca.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:15:54.760060 soos-sca-1.7.9rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-03-06 17:15:37.000000 soos-sca-1.7.9rc1/tests/tests.py
```

### Comparing `soos-sca-1.7.9/LICENSE` & `soos-sca-1.7.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `soos-sca-1.7.9/PKG-INFO` & `soos-sca-1.7.9rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soos-sca
-Version: 1.7.9
+Version: 1.7.9rc1
 Summary: Software security, simplified.
 Home-page: https://github.com/soos-io/soos-ci-analysis-python
 Author: SOOS
 Author-email: dev@soos.io
 Project-URL: Issues, https://github.com/soos-io/soos-ci-analysis-python/issues
 Project-URL: Source, https://github.com/soos-io/soos-ci-analysis-python
 Project-URL: About, https://soos.io
```

### Comparing `soos-sca-1.7.9/README.md` & `soos-sca-1.7.9rc1/README.md`

 * *Files identical despite different names*

### Comparing `soos-sca-1.7.9/setup.cfg` & `soos-sca-1.7.9rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `soos-sca-1.7.9/setup.py` & `soos-sca-1.7.9rc1/setup.py`

 * *Files identical despite different names*

### Comparing `soos-sca-1.7.9/src/cli/soos.py` & `soos-sca-1.7.9rc1/src/cli/soos.py`

 * *Files identical despite different names*

### Comparing `soos-sca-1.7.9/src/soos_sca.egg-info/PKG-INFO` & `soos-sca-1.7.9rc1/src/soos_sca.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soos-sca
-Version: 1.7.9
+Version: 1.7.9rc1
 Summary: Software security, simplified.
 Home-page: https://github.com/soos-io/soos-ci-analysis-python
 Author: SOOS
 Author-email: dev@soos.io
 Project-URL: Issues, https://github.com/soos-io/soos-ci-analysis-python/issues
 Project-URL: Source, https://github.com/soos-io/soos-ci-analysis-python
 Project-URL: About, https://soos.io
```

### Comparing `soos-sca-1.7.9/tests/tests.py` & `soos-sca-1.7.9rc1/tests/tests.py`

 * *Files identical despite different names*

