# Comparing `tmp/tvb-bids-monitor-2.7.2.tar.gz` & `tmp/tvb-bids-monitor-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvb-bids-monitor-2.7.2.tar", last modified: Wed Jan  4 06:21:51 2023, max compression
+gzip compressed data, was "tvb-bids-monitor-2.8.1.tar", last modified: Tue May 23 12:09:36 2023, max compression
```

## Comparing `tvb-bids-monitor-2.7.2.tar` & `tvb-bids-monitor-2.8.1.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:51.072865 tvb-bids-monitor-2.7.2/
--rw-r--r--   0 root         (0) root         (0)     1759 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/AUTHORS
--rw-r--r--   0 root         (0) root         (0)    36777 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      403 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/MANIFEST_bids_monitor.in
--rw-r--r--   0 root         (0) root         (0)     4158 2023-01-04 06:21:51.072865 tvb-bids-monitor-2.7.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4235 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/README.rst
--rw-r--r--   0 root         (0) root         (0)     3656 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/README_bids_monitor.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-04 06:21:51.072865 tvb-bids-monitor-2.7.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2989 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:51.064864 tvb-bids-monitor-2.7.2/tvb/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:51.065864 tvb-bids-monitor-2.7.2/tvb/config/
--rw-r--r--   0 root         (0) root         (0)     3095 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/config/algorithm_categories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:51.066865 tvb-bids-monitor-2.7.2/tvb/config/init/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/config/init/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:51.066865 tvb-bids-monitor-2.7.2/tvb/config/init/alembic/
--rw-r--r--   0 root         (0) root         (0)     2389 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/config/init/alembic/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:51.067865 tvb-bids-monitor-2.7.2/tvb/config/init/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     2466 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/config/init/alembic/versions/32d4bf9f8cab_update_db_002.py
--rw-r--r--   0 root         (0) root         (0)     2262 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/config/init/alembic/versions/32d4bf9f8def_update_db_003.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/config/init/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12427 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/config/init/alembic/versions/ec2859bb9114_update_db_001.py
--rw-r--r--   0 root         (0) root         (0)     9934 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/config/init/datatypes_registry.py
--rw-r--r--   0 root         (0) root         (0)     9460 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/config/init/initializer.py
--rw-r--r--   0 root         (0) root         (0)     6604 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/config/init/introspector_registry.py
--rw-r--r--   0 root         (0) root         (0)     5505 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/config/init/model_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:51.068865 tvb-bids-monitor-2.7.2/tvb/config/logger/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/config/logger/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3176 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/config/logger/cluster_handler.py
--rw-r--r--   0 root         (0) root         (0)     3131 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/config/logger/dev_logger_config.conf
--rw-r--r--   0 root         (0) root         (0)     2794 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/config/logger/logger_config.conf
--rw-r--r--   0 root         (0) root         (0)     5741 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/config/profile_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:51.068865 tvb-bids-monitor-2.7.2/tvb/interfaces/
--rw-r--r--   0 root         (0) root         (0)     1374 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:51.063864 tvb-bids-monitor-2.7.2/tvb/interfaces/rest/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:51.069865 tvb-bids-monitor-2.7.2/tvb/interfaces/rest/bids_monitor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/interfaces/rest/bids_monitor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10489 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/interfaces/rest/bids_monitor/bids_data_builder.py
--rw-r--r--   0 root         (0) root         (0)     8764 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/interfaces/rest/bids_monitor/bids_dir_monitor.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/interfaces/rest/bids_monitor/launch_bids_monitor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:51.069865 tvb-bids-monitor-2.7.2/tvb/interfaces/rest/bids_monitor/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/interfaces/rest/bids_monitor/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10056 2023-01-04 05:55:06.000000 tvb-bids-monitor-2.7.2/tvb/interfaces/rest/bids_monitor/tests/bids_monitor_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:51.071865 tvb-bids-monitor-2.7.2/tvb_bids_monitor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4158 2023-01-04 06:21:50.000000 tvb-bids-monitor-2.7.2/tvb_bids_monitor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1315 2023-01-04 06:21:50.000000 tvb-bids-monitor-2.7.2/tvb_bids_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-04 06:21:50.000000 tvb-bids-monitor-2.7.2/tvb_bids_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-01-04 06:21:50.000000 tvb-bids-monitor-2.7.2/tvb_bids_monitor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-01-04 06:21:50.000000 tvb-bids-monitor-2.7.2/tvb_bids_monitor.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.683415 tvb-bids-monitor-2.8.1/
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)    36777 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      403 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/MANIFEST_bids_monitor.in
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-05-23 12:09:36.683415 tvb-bids-monitor-2.8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4235 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)     3656 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/README_bids_monitor.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 12:09:36.683415 tvb-bids-monitor-2.8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2989 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.671414 tvb-bids-monitor-2.8.1/tvb/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.672414 tvb-bids-monitor-2.8.1/tvb/config/
+-rw-r--r--   0 root         (0) root         (0)     2391 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/algorithm_categories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.674414 tvb-bids-monitor-2.8.1/tvb/config/init/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/init/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.674414 tvb-bids-monitor-2.8.1/tvb/config/init/alembic/
+-rw-r--r--   0 root         (0) root         (0)     2238 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/init/alembic/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.676414 tvb-bids-monitor-2.8.1/tvb/config/init/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     2466 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/init/alembic/versions/32d4bf9f8cab_update_db_002.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/init/alembic/versions/32d4bf9f8def_update_db_003.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/init/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12427 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/init/alembic/versions/ec2859bb9114_update_db_001.py
+-rw-r--r--   0 root         (0) root         (0)     9934 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/init/datatypes_registry.py
+-rw-r--r--   0 root         (0) root         (0)     9460 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/init/initializer.py
+-rw-r--r--   0 root         (0) root         (0)     6604 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/init/introspector_registry.py
+-rw-r--r--   0 root         (0) root         (0)     5505 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/init/model_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.677414 tvb-bids-monitor-2.8.1/tvb/config/logger/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3176 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/logger/cluster_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3465 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/logger/dev_logger_config.conf
+-rw-r--r--   0 root         (0) root         (0)     5445 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/logger/elasticsearch_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3130 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/logger/logger_config.conf
+-rw-r--r--   0 root         (0) root         (0)     5820 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/profile_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.678414 tvb-bids-monitor-2.8.1/tvb/interfaces/
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.678414 tvb-bids-monitor-2.8.1/tvb/interfaces/rest/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/interfaces/rest/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.679414 tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10489 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/bids_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)     8764 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/bids_dir_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/launch_bids_monitor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.680414 tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10056 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/tests/bids_monitor_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.682414 tvb-bids-monitor-2.8.1/tvb_bids_monitor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-05-23 12:09:36.000000 tvb-bids-monitor-2.8.1/tvb_bids_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-05-23 12:09:36.000000 tvb-bids-monitor-2.8.1/tvb_bids_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 12:09:36.000000 tvb-bids-monitor-2.8.1/tvb_bids_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-23 12:09:36.000000 tvb-bids-monitor-2.8.1/tvb_bids_monitor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-23 12:09:36.000000 tvb-bids-monitor-2.8.1/tvb_bids_monitor.egg-info/top_level.txt
```

### Comparing `tvb-bids-monitor-2.7.2/AUTHORS` & `tvb-bids-monitor-2.8.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.7.2/LICENSE` & `tvb-bids-monitor-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.7.2/PKG-INFO` & `tvb-bids-monitor-2.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-bids-monitor
-Version: 2.7.2
+Version: 2.8.1
 Summary: A helper package containing BIDS directory monitor module
 Home-page: http://www.thevirtualbrain.org
 Download-URL: https://github.com/the-virtual-brain/tvb-root
 Author: Akash Upadhyay, Paula Prodan
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb rest client brain simulator neuroscience human animal neuronal dynamics models delay
```

### Comparing `tvb-bids-monitor-2.7.2/README.rst` & `tvb-bids-monitor-2.8.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                 |
                 |
             tvb.config.init
                 |
                 |
             tvb.interfaces
 
-**tvb-data** should be installed from **Zenodo**: https://zenodo.org/record/4263723/files/tvb_data.zip?download=1.
+**tvb-data** should be installed from **Zenodo**: https://zenodo.org/record/7574266/files/tvb_data.zip?download=1.
 After download, unzip and execute `python setup.py develop` in the correct env.
 
 Usage
 -----
 
 To use TVB code, clone from GitHub (https://github.com/the-virtual-brain/tvb-root), or get from Pypi::
```

### Comparing `tvb-bids-monitor-2.7.2/README_bids_monitor.rst` & `tvb-bids-monitor-2.8.1/README_bids_monitor.rst`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.7.2/setup.py` & `tvb-bids-monitor-2.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 import shutil
 
 import setuptools
 from setuptools.command.egg_info import manifest_maker
 
 manifest_maker.template = 'MANIFEST_bids_monitor.in'
 
-VERSION = "2.7.2"
+VERSION = "2.8.1"
 
 TVB_TEAM = "Akash Upadhyay, Paula Prodan"
 
 TVB_INSTALL_REQUIREMENTS = ["tvb-rest-client", "watchdog"]
 
 # Packaging bids-monitor
 with open(os.path.join(os.path.dirname(__file__), 'README_bids_monitor.rst')) as fd:
```

### Comparing `tvb-bids-monitor-2.7.2/tvb/__init__.py` & `tvb-bids-monitor-2.8.1/tvb/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.7.2/tvb/config/__init__.py` & `tvb-bids-monitor-2.8.1/tvb/config/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,26 +29,17 @@
 
 E.g. Scientific libraries modules are plugged, to avoid close dependencies.
 E.g. A list with all the modules where adapters are implemented.
 """
 # There are kept here for being used inside tvb.core
 # We can not move all these in IntrospectovRegistry, due to circular dependencies
 
-from collections import OrderedDict
-# Import metrics here, so that Traits will find them and return them as known subclasses
-from tvb.analyzers.metric_kuramoto_index import compute_kuramoto_index_metric
-from tvb.analyzers.metric_proxy_metastability import compute_proxy_metastability_metric
-from tvb.analyzers.metric_variance_global import compute_variance_global_metric
-from tvb.analyzers.metric_variance_of_node_variance import compute_variance_of_node_variance_metric
-
-ALGORITHMS = {'GlobalVariance': compute_variance_global_metric,
-              'KuramotoIndex': compute_kuramoto_index_metric,
-              'ProxyMetastabilitySynchrony': compute_proxy_metastability_metric,
-              'VarianceNodeVariance': compute_variance_of_node_variance_metric}
+from tvb.analyzers import METRICS
 
+ALGORITHMS = METRICS
 
 SIMULATION_DATATYPE_CLASS = "SimulationState"
 
 TVB_IMPORTER_MODULE = "tvb.adapters.uploaders.tvb_importer"
 TVB_IMPORTER_CLASS = "TVBImporter"
 
 SIMULATOR_MODULE = "tvb.adapters.simulator.simulator_adapter"
```

### Comparing `tvb-bids-monitor-2.7.2/tvb/config/algorithm_categories.py` & `tvb-bids-monitor-2.8.1/tvb/config/algorithm_categories.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.7.2/tvb/config/init/alembic/env.py` & `tvb-bids-monitor-2.8.1/tvb/config/init/alembic/env.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,28 +7,33 @@
 from sqlalchemy import pool
 from alembic import context
 
 # this is the Alembic Config object, which provides
 # access to the values within the .ini file in use.
 config = context.config
 
+# Interpret the config file for Python logging.
+# This line sets up loggers basically.
+if config.config_file_name is not None:
+    fileConfig(config.config_file_name)
+
 # add your model's MetaData object here
 # for 'autogenerate' support
 # from myapp import mymodel
 # target_metadata = mymodel.Base.metadata
 from tvb.core.neotraits.db import Base
 target_metadata = Base.metadata
 
 # other values from the config, defined by the needs of env.py,
 # can be acquired:
 # my_important_option = config.get_main_option("my_important_option")
 # ... etc.
 
 
-def run_migrations_offline():
+def run_migrations_offline() -> None:
     """Run migrations in 'offline' mode.
 
     This configures the context with just a URL
     and not an Engine, though an Engine is acceptable
     here as well.  By skipping the Engine creation
     we don't even need a DBAPI to be available.
 
@@ -44,38 +49,30 @@
         dialect_opts={"paramstyle": "named"},
     )
 
     with context.begin_transaction():
         context.run_migrations()
 
 
-def run_migrations_online():
+def run_migrations_online() -> None:
     """Run migrations in 'online' mode.
 
     In this scenario we need to create an Engine
     and associate a connection with the context.
 
     """
-    connectable = config.attributes.get('connection', None)
-
-    if connectable is None:
-        # only create Engine if we don't have a Connection
-        # from the outside
-        connectable = engine_from_config(
-            config.get_section(config.config_ini_section),
-            prefix="sqlalchemy.",
-            poolclass=pool.NullPool,
-        )
-
-        # when connectable is already a Connection object, calling
-        # connect() gives us a *branched connection*.
+    connectable = engine_from_config(
+        config.get_section(config.config_ini_section, {}),
+        prefix="sqlalchemy.",
+        poolclass=pool.NullPool,
+    )
 
     with connectable.connect() as connection:
         context.configure(
-            connection=connection, target_metadata=target_metadata, render_as_batch=True
+            connection=connection, target_metadata=target_metadata
         )
 
         with context.begin_transaction():
             context.run_migrations()
 
 
 if context.is_offline_mode():
```

### Comparing `tvb-bids-monitor-2.7.2/tvb/config/init/alembic/versions/32d4bf9f8cab_update_db_002.py` & `tvb-bids-monitor-2.8.1/tvb/config/init/alembic/versions/32d4bf9f8cab_update_db_002.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.7.2/tvb/config/init/alembic/versions/32d4bf9f8def_update_db_003.py` & `tvb-bids-monitor-2.8.1/tvb/config/init/alembic/versions/32d4bf9f8def_update_db_003.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.7.2/tvb/config/init/alembic/versions/ec2859bb9114_update_db_001.py` & `tvb-bids-monitor-2.8.1/tvb/config/init/alembic/versions/ec2859bb9114_update_db_001.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.7.2/tvb/config/init/datatypes_registry.py` & `tvb-bids-monitor-2.8.1/tvb/config/init/datatypes_registry.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.7.2/tvb/config/init/initializer.py` & `tvb-bids-monitor-2.8.1/tvb/config/init/initializer.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.7.2/tvb/config/init/introspector_registry.py` & `tvb-bids-monitor-2.8.1/tvb/config/init/introspector_registry.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.7.2/tvb/config/init/model_manager.py` & `tvb-bids-monitor-2.8.1/tvb/config/init/model_manager.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.7.2/tvb/config/logger/cluster_handler.py` & `tvb-bids-monitor-2.8.1/tvb/config/logger/cluster_handler.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.7.2/tvb/config/logger/dev_logger_config.conf` & `tvb-bids-monitor-2.8.1/tvb/config/logger/dev_logger_config.conf`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ############################################
 ## TVB - logging configuration. ##
 ############################################
 [loggers]
-keys=root, tvb, tvb_trace_user, tvb_core_entities_file, tvb_simulator, cherrypy, sqlalchemy, sqlalchemyEcho, rst2pdf, numba, matplotlib
+keys=root, tvb, tvb_trace_user, tvb_core_entities_file, tvb_simulator, cherrypy, sqlalchemy, sqlalchemyEcho, rst2pdf, numba, matplotlib, elastic_transport
 
 [handlers]
-keys=consoleHandler,fileHandler,cherrypyFileHandler,sqlalchemyFileHandler, traceUserFileHandler
+keys=consoleHandler,fileHandler,cherrypyFileHandler,sqlalchemyFileHandler, traceUserFileHandler, elasticSearchHandler
 
 [formatters]
 keys=simpleFormatter
 
 [logger_root]
 level=DEBUG
 handlers=consoleHandler, fileHandler
@@ -22,15 +22,15 @@
 level=DEBUG
 handlers=consoleHandler, fileHandler
 qualname=tvb
 propagate=0
 
 [logger_tvb_trace_user]
 level=NOTSET
-handlers=traceUserFileHandler
+handlers=traceUserFileHandler, elasticSearchHandler
 qualname=tvb_user_actions
 propagate=0
 
 [logger_tvb_core_entities_file]
 level=INFO
 handlers=consoleHandler, fileHandler
 qualname=tvb.core.entities.file
@@ -78,14 +78,20 @@
 
 [logger_matplotlib]
 level=ERROR
 handlers=consoleHandler, fileHandler
 qualname=matplotlib
 propagate=0
 
+[logger_elastic_transport]
+level=ERROR
+handlers=consoleHandler, fileHandler
+qualname=elastic_transport
+propagate=0
+
 ############################################
 ## Handlers                               ##
 ############################################
 
 [handler_consoleHandler]
 class=StreamHandler
 level=INFO
@@ -115,14 +121,20 @@
 [handler_sqlalchemyFileHandler]
 class=tvb.basic.logger.simple_handler.SimpleTimedRotatingFileHandler
 level=INFO
 formatter=simpleFormatter
 # Generate a new file every midnight and keep logs for 1 day
 args=('sqlalchemy.log', 'midnight', 1, 1)
 
+
+[handler_elasticSearchHandler]
+class=tvb.config.logger.elasticsearch_handler.ElasticQueueHandler
+level=NOTSET
+formatter=simpleFormatter
+
 ############################################
 ## Formatters                             ##
 ############################################
 
 [formatter_simpleFormatter]
 format=%(asctime)s - %(levelname)s - %(name)s - %(message)s
-datefmt=
+datefmt=%Y-%m-%dT%H:%M:%S
```

### Comparing `tvb-bids-monitor-2.7.2/tvb/config/logger/logger_config.conf` & `tvb-bids-monitor-2.8.1/tvb/config/logger/logger_config.conf`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ############################################
 ## TVB - logging configuration. ##
 ############################################
 [loggers]
-keys=root, tvb, tvb_trace_user, tvb_core_entities_file, tvb_simulator, tvb_traits, cherrypy, sqlalchemy, rst2pdf, numba, matplotlib
+keys=root, tvb, tvb_trace_user, tvb_core_entities_file, tvb_simulator, tvb_traits, cherrypy, sqlalchemy, rst2pdf, numba, matplotlib, elastic_transport
 
 [handlers]
-keys=consoleHandler,fileHandler,cherrypyFileHandler, traceUserFileHandler
+keys=consoleHandler,fileHandler,cherrypyFileHandler, traceUserFileHandler, elasticSearchHandler
 
 [formatters]
 keys=simpleFormatter
 
 [logger_root]
 level=WARNING
 handlers=fileHandler
@@ -22,15 +22,15 @@
 level=INFO
 handlers=fileHandler
 qualname=tvb
 propagate=0
 
 [logger_tvb_trace_user]
 level=NOTSET
-handlers=traceUserFileHandler
+handlers=traceUserFileHandler, elasticSearchHandler
 qualname=tvb_user_actions
 propagate=0
 
 [logger_tvb_core_entities_file]
 level=WARNING
 handlers=fileHandler
 qualname=tvb.core.entities.file
@@ -79,14 +79,20 @@
 
 [logger_matplotlib]
 level=ERROR
 handlers=consoleHandler, fileHandler
 qualname=matplotlib
 propagate=0
 
+[logger_elastic_transport]
+level=ERROR
+handlers=consoleHandler, fileHandler
+qualname=elastic_transport
+propagate=0
+
 ############################################
 ## Handlers                               ##
 ############################################
 
 [handler_consoleHandler]
 class=StreamHandler
 level=ERROR
@@ -108,14 +114,22 @@
 
 [handler_traceUserFileHandler]
 class=tvb.basic.logger.simple_handler.SimpleTimedRotatingFileHandler
 level=NOTSET
 formatter=simpleFormatter
 # Generate a new file every midnight and keep logs for 30 days
 args=('trace_user.log', 'midnight', 1, 30)
+
+
+[handler_elasticSearchHandler]
+class=tvb.config.logger.elasticsearch_handler.ElasticQueueHandler
+level=NOTSET
+formatter=simpleFormatter
+
+
 ############################################
 ## Formatters                             ##
 ############################################
 
 [formatter_simpleFormatter]
 format=%(asctime)s - %(levelname)s - %(name)s - %(message)s
-datefmt=
+datefmt=%Y-%m-%dT%H:%M:%S
```

### Comparing `tvb-bids-monitor-2.7.2/tvb/config/profile_settings.py` & `tvb-bids-monitor-2.8.1/tvb/config/profile_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 TVB global configurations are predefined/read from here, for working with Framework.
 
 .. moduleauthor:: Lia Domide <lia.domide@codemart.ro>
 """
 
 import os
 import sys
+import tvb.config.init
 from tvb.basic.config import stored
 from tvb.basic.config.profile_settings import BaseSettingsProfile
 from tvb.basic.config.settings import DBSettings
 from tvb.basic.logger import builder
 from tvb.basic.logger.builder import LoggerBuilder
 from tvb.config.init.datatypes_registry import populate_datatypes_registry
 
@@ -60,15 +61,16 @@
 
     def initialize_for_deployment(self):
         """
         Specific initialization for deployment and framework settings
         """
         super(WebSettingsProfile, self).initialize_for_deployment()
 
-        inside_static_folder = os.path.join(self.EXTERNALS_FOLDER_PARENT, 'tvb')
+        inside_static_folder = os.path.dirname(os.path.dirname(os.path.dirname(
+            os.path.abspath(tvb.config.init.__file__))))
         self.web.CHERRYPY_CONFIGURATION['/statichelp']['tools.staticdir.root'] = inside_static_folder
 
         # We want to disable warnings we get from sqlalchemy for traited attributes when we are in deployment mode.
         import warnings
         from sqlalchemy import exc as sa_exc
 
         warnings.simplefilter("ignore", category=sa_exc.SAWarning)
```

### Comparing `tvb-bids-monitor-2.7.2/tvb/interfaces/__init__.py` & `tvb-bids-monitor-2.8.1/tvb/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.7.2/tvb/interfaces/rest/bids_monitor/bids_data_builder.py` & `tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/bids_data_builder.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.7.2/tvb/interfaces/rest/bids_monitor/bids_dir_monitor.py` & `tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/bids_dir_monitor.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.7.2/tvb/interfaces/rest/bids_monitor/launch_bids_monitor.py` & `tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/launch_bids_monitor.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.7.2/tvb/interfaces/rest/bids_monitor/tests/bids_monitor_test.py` & `tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/tests/bids_monitor_test.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.7.2/tvb_bids_monitor.egg-info/PKG-INFO` & `tvb-bids-monitor-2.8.1/tvb_bids_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-bids-monitor
-Version: 2.7.2
+Version: 2.8.1
 Summary: A helper package containing BIDS directory monitor module
 Home-page: http://www.thevirtualbrain.org
 Download-URL: https://github.com/the-virtual-brain/tvb-root
 Author: Akash Upadhyay, Paula Prodan
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb rest client brain simulator neuroscience human animal neuronal dynamics models delay
```

### Comparing `tvb-bids-monitor-2.7.2/tvb_bids_monitor.egg-info/SOURCES.txt` & `tvb-bids-monitor-2.8.1/tvb_bids_monitor.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,16 +17,18 @@
 tvb/config/init/alembic/versions/32d4bf9f8cab_update_db_002.py
 tvb/config/init/alembic/versions/32d4bf9f8def_update_db_003.py
 tvb/config/init/alembic/versions/__init__.py
 tvb/config/init/alembic/versions/ec2859bb9114_update_db_001.py
 tvb/config/logger/__init__.py
 tvb/config/logger/cluster_handler.py
 tvb/config/logger/dev_logger_config.conf
+tvb/config/logger/elasticsearch_handler.py
 tvb/config/logger/logger_config.conf
 tvb/interfaces/__init__.py
+tvb/interfaces/rest/__init__.py
 tvb/interfaces/rest/bids_monitor/__init__.py
 tvb/interfaces/rest/bids_monitor/bids_data_builder.py
 tvb/interfaces/rest/bids_monitor/bids_dir_monitor.py
 tvb/interfaces/rest/bids_monitor/launch_bids_monitor.py
 tvb/interfaces/rest/bids_monitor/tests/__init__.py
 tvb/interfaces/rest/bids_monitor/tests/bids_monitor_test.py
 tvb_bids_monitor.egg-info/PKG-INFO
```

