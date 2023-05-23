# Comparing `tmp/apache-airflow-providers-sktvane-0.1.4.tar.gz` & `tmp/apache-airflow-providers-sktvane-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-sktvane-0.1.4.tar", last modified: Tue May 16 06:34:03 2023, max compression
+gzip compressed data, was "apache-airflow-providers-sktvane-0.1.5.tar", last modified: Tue May 23 04:40:37 2023, max compression
```

## Comparing `apache-airflow-providers-sktvane-0.1.4.tar` & `apache-airflow-providers-sktvane-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:34:03.848683 apache-airflow-providers-sktvane-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-16 06:34:03.848683 apache-airflow-providers-sktvane-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-16 06:33:53.000000 apache-airflow-providers-sktvane-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:34:03.836683 apache-airflow-providers-sktvane-0.1.4/airflow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:34:03.836683 apache-airflow-providers-sktvane-0.1.4/airflow/providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:34:03.840683 apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 06:33:53.000000 apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:34:03.844683 apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/macros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 06:33:53.000000 apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-16 06:33:53.000000 apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/macros/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-16 06:33:53.000000 apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/macros/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-16 06:33:53.000000 apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/macros/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-16 06:33:53.000000 apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/macros/slack_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-16 06:33:53.000000 apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/macros/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:34:03.844683 apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 06:33:53.000000 apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-16 06:33:53.000000 apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/operators/nes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:34:03.844683 apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 06:33:53.000000 apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-16 06:33:53.000000 apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/sensors/gcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:34:03.844683 apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 06:33:53.000000 apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 06:33:53.000000 apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:34:03.848683 apache-airflow-providers-sktvane-0.1.4/apache_airflow_providers_sktvane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-16 06:34:03.000000 apache-airflow-providers-sktvane-0.1.4/apache_airflow_providers_sktvane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-16 06:34:03.000000 apache-airflow-providers-sktvane-0.1.4/apache_airflow_providers_sktvane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 06:34:03.000000 apache-airflow-providers-sktvane-0.1.4/apache_airflow_providers_sktvane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 06:34:03.000000 apache-airflow-providers-sktvane-0.1.4/apache_airflow_providers_sktvane.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 06:34:03.000000 apache-airflow-providers-sktvane-0.1.4/apache_airflow_providers_sktvane.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 06:34:03.848683 apache-airflow-providers-sktvane-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-16 06:33:53.000000 apache-airflow-providers-sktvane-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:37.150298 apache-airflow-providers-sktvane-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-23 04:40:37.150298 apache-airflow-providers-sktvane-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:37.150298 apache-airflow-providers-sktvane-0.1.5/airflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:37.150298 apache-airflow-providers-sktvane-0.1.5/airflow/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:37.150298 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:37.150298 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/slack_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:37.150298 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/operators/nes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:37.150298 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/sensors/gcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:37.150298 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:37.150298 apache-airflow-providers-sktvane-0.1.5/apache_airflow_providers_sktvane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-23 04:40:37.000000 apache-airflow-providers-sktvane-0.1.5/apache_airflow_providers_sktvane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-23 04:40:37.000000 apache-airflow-providers-sktvane-0.1.5/apache_airflow_providers_sktvane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 04:40:37.000000 apache-airflow-providers-sktvane-0.1.5/apache_airflow_providers_sktvane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-23 04:40:37.000000 apache-airflow-providers-sktvane-0.1.5/apache_airflow_providers_sktvane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 04:40:37.000000 apache-airflow-providers-sktvane-0.1.5/apache_airflow_providers_sktvane.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-23 04:40:37.154298 apache-airflow-providers-sktvane-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/setup.py
```

### Comparing `apache-airflow-providers-sktvane-0.1.4/PKG-INFO` & `apache-airflow-providers-sktvane-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sktvane
-Version: 0.1.4
+Version: 0.1.5
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt
 Home-page: https://github.com/sktaiflow/sktvane-airflow-providers
 Author: aidp
 Author-email: aidp@sktai.io
 License: MIT
 Download-URL: https://github.com/sktaiflow/sktvane-airflow-providers
 Keywords: airflow,sktvane
```

### Comparing `apache-airflow-providers-sktvane-0.1.4/README.md` & `apache-airflow-providers-sktvane-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/macros/date.py` & `apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/date.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,14 +19,26 @@
 def ym_nodash_add_month(ds, months, prev_ds=True):
     ds = datetime.strptime(ds, "%Y%m%d")
     time_delta = timedelta(-1) if prev_ds else timedelta(0)
     ds = ds + time_delta + relativedelta(months=months)
     return ds.strftime("%Y%m")
 
 
+def first_day_of_last_month(ds):
+    date = datetime.strptime(ds, "%Y%m%d")
+    dt = date.replace(month=date.month, day=1) - timedelta(days=1)
+    return dt.replace(month=dt.month, day=1).strftime("%Y%m%d")
+
+
+def last_day_of_last_month(ds):
+    date = datetime.strptime(ds, "%Y%m%d")
+    dt = date.replace(month=date.month, day=1) - timedelta(days=1)
+    return dt.strftime("%Y%m%d")
+
+
 def first_day_of_this_month(ds):
     date = datetime.strptime(ds, "%Y%m%d")
     dt = date.replace(month=date.month, day=1)
     return dt.strftime("%Y%m%d")
 
 
 def last_day_of_this_month(ds):
```

### Comparing `apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/macros/gcp.py` & `apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/gcp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/macros/slack.py` & `apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/macros/slack_notifier.py` & `apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/operators/nes.py` & `apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/operators/nes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.4/airflow/providers/sktvane/sensors/gcp.py` & `apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/sensors/gcp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.4/apache_airflow_providers_sktvane.egg-info/PKG-INFO` & `apache-airflow-providers-sktvane-0.1.5/apache_airflow_providers_sktvane.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sktvane
-Version: 0.1.4
+Version: 0.1.5
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt
 Home-page: https://github.com/sktaiflow/sktvane-airflow-providers
 Author: aidp
 Author-email: aidp@sktai.io
 License: MIT
 Download-URL: https://github.com/sktaiflow/sktvane-airflow-providers
 Keywords: airflow,sktvane
```

### Comparing `apache-airflow-providers-sktvane-0.1.4/apache_airflow_providers_sktvane.egg-info/SOURCES.txt` & `apache-airflow-providers-sktvane-0.1.5/apache_airflow_providers_sktvane.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.4/setup.py` & `apache-airflow-providers-sktvane-0.1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="apache-airflow-providers-sktvane",
-    version="0.1.4",
+    version="0.1.5",
     author="aidp",
     author_email="aidp@sktai.io",
     description="Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["airflow", "sktvane"],
     license="MIT",
```

