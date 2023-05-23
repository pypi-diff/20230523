# Comparing `tmp/bodo_platform_utils-0.0.8.tar.gz` & `tmp/bodo_platform_utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodo_platform_utils-0.0.8.tar", last modified: Mon Apr 17 17:38:03 2023, max compression
+gzip compressed data, was "bodo_platform_utils-0.0.9.tar", last modified: Tue May 23 21:04:51 2023, max compression
```

## Comparing `bodo_platform_utils-0.0.8.tar` & `bodo_platform_utils-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:38:03.881700 bodo_platform_utils-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-17 17:38:03.881700 bodo_platform_utils-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:38:03.881700 bodo_platform_utils-0.0.8/bodo_platform_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/bodo_platform_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-17 17:38:03.881700 bodo_platform_utils-0.0.8/bodo_platform_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/bodo_platform_utils/bodosqlwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/bodo_platform_utils/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/bodo_platform_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/bodo_platform_utils/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/bodo_platform_utils/utils_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:38:03.881700 bodo_platform_utils-0.0.8/bodo_platform_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-17 17:38:03.000000 bodo_platform_utils-0.0.8/bodo_platform_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-17 17:38:03.000000 bodo_platform_utils-0.0.8/bodo_platform_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:38:03.000000 bodo_platform_utils-0.0.8/bodo_platform_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-17 17:38:03.000000 bodo_platform_utils-0.0.8/bodo_platform_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-17 17:38:03.000000 bodo_platform_utils-0.0.8/bodo_platform_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-17 17:38:03.881700 bodo_platform_utils-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:04:51.657964 bodo_platform_utils-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-23 21:03:06.000000 bodo_platform_utils-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-23 21:03:06.000000 bodo_platform_utils-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-23 21:04:51.657964 bodo_platform_utils-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-23 21:03:06.000000 bodo_platform_utils-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:04:51.661964 bodo_platform_utils-0.0.9/bodo_platform_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-23 21:03:06.000000 bodo_platform_utils-0.0.9/bodo_platform_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-23 21:04:51.661964 bodo_platform_utils-0.0.9/bodo_platform_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-05-23 21:03:06.000000 bodo_platform_utils-0.0.9/bodo_platform_utils/bodosqlwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-23 21:03:06.000000 bodo_platform_utils-0.0.9/bodo_platform_utils/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-23 21:03:06.000000 bodo_platform_utils-0.0.9/bodo_platform_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-23 21:03:06.000000 bodo_platform_utils-0.0.9/bodo_platform_utils/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-23 21:03:06.000000 bodo_platform_utils-0.0.9/bodo_platform_utils/utils_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:04:51.657964 bodo_platform_utils-0.0.9/bodo_platform_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-23 21:04:51.000000 bodo_platform_utils-0.0.9/bodo_platform_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-23 21:04:51.000000 bodo_platform_utils-0.0.9/bodo_platform_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:04:51.000000 bodo_platform_utils-0.0.9/bodo_platform_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-23 21:04:51.000000 bodo_platform_utils-0.0.9/bodo_platform_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 21:04:51.000000 bodo_platform_utils-0.0.9/bodo_platform_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-23 21:04:51.661964 bodo_platform_utils-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-23 21:03:06.000000 bodo_platform_utils-0.0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-05-23 21:03:06.000000 bodo_platform_utils-0.0.9/versioneer.py
```

### Comparing `bodo_platform_utils-0.0.8/LICENSE` & `bodo_platform_utils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bodo_platform_utils-0.0.8/PKG-INFO` & `bodo_platform_utils-0.0.9/bodo_platform_utils.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bodo_platform_utils
-Version: 0.0.8
+Name: bodo-platform-utils
+Version: 0.0.9
 Summary: This is package contains utility functions to retrieve data from Cloud Providers for platform
 Home-page: https://github.com/Bodo-inc/bodo-platform-utils
 Author: Bodo Inc
 Author-email: noreply@bodo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bodo_platform_utils-0.0.8/bodo_platform_utils/bodosqlwrapper.py` & `bodo_platform_utils-0.0.9/bodo_platform_utils/bodosqlwrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 from .catalog import get_data
 
 import bodosql
 
 import bodo
 import bodo.utils.tracing as tracing
 
+# Turn verbose mode on
+bodo.set_verbose_level(2)
+
 @bodo.jit(cache=True)
 def run_sql_query(
     query_str, bc, pq_out_filename, sf_out_table_name, sf_write_conn, print_output
 ):
     """Boilerplate function to execute a query string.
 
     Args:
```

### Comparing `bodo_platform_utils-0.0.8/bodo_platform_utils/catalog.py` & `bodo_platform_utils-0.0.9/bodo_platform_utils/catalog.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_utils-0.0.8/bodo_platform_utils/config.py` & `bodo_platform_utils-0.0.9/bodo_platform_utils/config.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_utils-0.0.8/bodo_platform_utils/secrets.py` & `bodo_platform_utils-0.0.9/bodo_platform_utils/secrets.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_utils-0.0.8/bodo_platform_utils.egg-info/PKG-INFO` & `bodo_platform_utils-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bodo-platform-utils
-Version: 0.0.8
+Name: bodo_platform_utils
+Version: 0.0.9
 Summary: This is package contains utility functions to retrieve data from Cloud Providers for platform
 Home-page: https://github.com/Bodo-inc/bodo-platform-utils
 Author: Bodo Inc
 Author-email: noreply@bodo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bodo_platform_utils-0.0.8/setup.py` & `bodo_platform_utils-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_utils-0.0.8/versioneer.py` & `bodo_platform_utils-0.0.9/versioneer.py`

 * *Files identical despite different names*

