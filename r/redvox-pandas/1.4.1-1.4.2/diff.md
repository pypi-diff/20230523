# Comparing `tmp/redvox-pandas-1.4.1.tar.gz` & `tmp/redvox-pandas-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redvox-pandas-1.4.1.tar", last modified: Fri Apr 28 19:56:54 2023, max compression
+gzip compressed data, was "redvox-pandas-1.4.2.tar", last modified: Tue May 23 20:16:35 2023, max compression
```

## Comparing `redvox-pandas-1.4.1.tar` & `redvox-pandas-1.4.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 19:56:54.304577 redvox-pandas-1.4.1/
--rw-rw-r--   0 opq       (1000) opq       (1000)    11359 2021-07-02 00:27:05.000000 redvox-pandas-1.4.1/LICENSE
--rw-r--r--   0 opq       (1000) opq       (1000)    15648 2023-04-28 19:56:54.304577 redvox-pandas-1.4.1/PKG-INFO
--rw-r--r--   0 opq       (1000) opq       (1000)     2266 2023-04-27 21:26:24.000000 redvox-pandas-1.4.1/README.md
--rw-r--r--   0 opq       (1000) opq       (1000)      882 2023-04-28 19:55:00.000000 redvox-pandas-1.4.1/pyproject.toml
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 19:56:54.303577 redvox-pandas-1.4.1/redpandas/
--rw-rw-r--   0 opq       (1000) opq       (1000)      305 2022-07-07 20:44:53.000000 redvox-pandas-1.4.1/redpandas/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    19300 2023-04-27 21:26:25.000000 redvox-pandas-1.4.1/redpandas/redpd_build_station.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    15456 2022-07-07 20:44:53.000000 redvox-pandas-1.4.1/redpandas/redpd_cohere.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     6751 2021-08-03 22:13:07.000000 redvox-pandas-1.4.1/redpandas/redpd_config.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4051 2022-07-07 20:44:53.000000 redvox-pandas-1.4.1/redpandas/redpd_datawin.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4981 2023-04-27 21:26:25.000000 redvox-pandas-1.4.1/redpandas/redpd_df.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    14773 2022-07-07 20:44:53.000000 redvox-pandas-1.4.1/redpandas/redpd_dq.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    16853 2021-08-03 22:13:07.000000 redvox-pandas-1.4.1/redpandas/redpd_ensonify.py
--rw-rw-r--   0 opq       (1000) opq       (1000)      403 2021-10-18 19:57:34.000000 redvox-pandas-1.4.1/redpandas/redpd_errors.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    26898 2021-10-18 19:57:34.000000 redvox-pandas-1.4.1/redpandas/redpd_filter.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     8524 2022-07-07 20:44:53.000000 redvox-pandas-1.4.1/redpandas/redpd_geospatial.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4200 2022-07-07 20:44:53.000000 redvox-pandas-1.4.1/redpandas/redpd_gravity.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3790 2022-07-07 20:44:53.000000 redvox-pandas-1.4.1/redpandas/redpd_iterator.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     7874 2022-07-07 20:44:53.000000 redvox-pandas-1.4.1/redpandas/redpd_orientation.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 19:56:54.303577 redvox-pandas-1.4.1/redpandas/redpd_plot/
--rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-08-03 22:13:07.000000 redvox-pandas-1.4.1/redpandas/redpd_plot/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4423 2021-08-03 22:13:07.000000 redvox-pandas-1.4.1/redpandas/redpd_plot/coherence.py
--rw-r--r--   0 opq       (1000) opq       (1000)    33263 2023-04-27 21:26:25.000000 redvox-pandas-1.4.1/redpandas/redpd_plot/mesh.py
--rw-rw-r--   0 opq       (1000) opq       (1000)      467 2021-10-18 19:57:34.000000 redvox-pandas-1.4.1/redpandas/redpd_plot/parameters.py
--rw-r--r--   0 opq       (1000) opq       (1000)    35442 2023-04-27 21:26:25.000000 redvox-pandas-1.4.1/redpandas/redpd_plot/wiggles.py
--rw-r--r--   0 opq       (1000) opq       (1000)    15627 2023-04-27 21:26:25.000000 redvox-pandas-1.4.1/redpandas/redpd_preprocess.py
--rw-r--r--   0 opq       (1000) opq       (1000)     8703 2023-04-27 21:26:25.000000 redvox-pandas-1.4.1/redpandas/redpd_report.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1482 2022-07-07 20:44:53.000000 redvox-pandas-1.4.1/redpandas/redpd_scales.py
--rw-rw-r--   0 opq       (1000) opq       (1000)       80 2022-07-07 20:44:53.000000 redvox-pandas-1.4.1/redpandas/redpd_state.py
--rw-r--r--   0 opq       (1000) opq       (1000)    15899 2023-04-27 21:26:25.000000 redvox-pandas-1.4.1/redpandas/redpd_tfr.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    21018 2022-07-07 20:44:53.000000 redvox-pandas-1.4.1/redpandas/redpd_xcorr.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 19:56:54.304577 redvox-pandas-1.4.1/redvox_pandas.egg-info/
--rw-rw-r--   0 opq       (1000) opq       (1000)    15648 2023-04-28 19:56:54.000000 redvox-pandas-1.4.1/redvox_pandas.egg-info/PKG-INFO
--rw-rw-r--   0 opq       (1000) opq       (1000)      908 2023-04-28 19:56:54.000000 redvox-pandas-1.4.1/redvox_pandas.egg-info/SOURCES.txt
--rw-rw-r--   0 opq       (1000) opq       (1000)        1 2023-04-28 19:56:54.000000 redvox-pandas-1.4.1/redvox_pandas.egg-info/dependency_links.txt
--rw-rw-r--   0 opq       (1000) opq       (1000)       96 2023-04-28 19:56:54.000000 redvox-pandas-1.4.1/redvox_pandas.egg-info/requires.txt
--rw-rw-r--   0 opq       (1000) opq       (1000)       10 2023-04-28 19:56:54.000000 redvox-pandas-1.4.1/redvox_pandas.egg-info/top_level.txt
--rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-04-28 19:56:54.304577 redvox-pandas-1.4.1/setup.cfg
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-05-23 20:16:35.862973 redvox-pandas-1.4.2/
+-rw-rw-r--   0 opq       (1000) opq       (1000)    11359 2021-07-02 00:27:05.000000 redvox-pandas-1.4.2/LICENSE
+-rw-r--r--   0 opq       (1000) opq       (1000)    15648 2023-05-23 20:16:35.862973 redvox-pandas-1.4.2/PKG-INFO
+-rw-r--r--   0 opq       (1000) opq       (1000)     2266 2023-04-27 21:26:24.000000 redvox-pandas-1.4.2/README.md
+-rw-r--r--   0 opq       (1000) opq       (1000)      882 2023-05-23 20:16:28.000000 redvox-pandas-1.4.2/pyproject.toml
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-05-23 20:16:35.861973 redvox-pandas-1.4.2/redpandas/
+-rw-rw-r--   0 opq       (1000) opq       (1000)      305 2022-07-07 20:44:53.000000 redvox-pandas-1.4.2/redpandas/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    19300 2023-04-27 21:26:25.000000 redvox-pandas-1.4.2/redpandas/redpd_build_station.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    15456 2022-07-07 20:44:53.000000 redvox-pandas-1.4.2/redpandas/redpd_cohere.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     6751 2021-08-03 22:13:07.000000 redvox-pandas-1.4.2/redpandas/redpd_config.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4051 2022-07-07 20:44:53.000000 redvox-pandas-1.4.2/redpandas/redpd_datawin.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     4981 2023-04-27 21:26:25.000000 redvox-pandas-1.4.2/redpandas/redpd_df.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    14773 2022-07-07 20:44:53.000000 redvox-pandas-1.4.2/redpandas/redpd_dq.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    16853 2021-08-03 22:13:07.000000 redvox-pandas-1.4.2/redpandas/redpd_ensonify.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)      403 2021-10-18 19:57:34.000000 redvox-pandas-1.4.2/redpandas/redpd_errors.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    26898 2021-10-18 19:57:34.000000 redvox-pandas-1.4.2/redpandas/redpd_filter.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     8524 2022-07-07 20:44:53.000000 redvox-pandas-1.4.2/redpandas/redpd_geospatial.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4200 2022-07-07 20:44:53.000000 redvox-pandas-1.4.2/redpandas/redpd_gravity.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     3790 2022-07-07 20:44:53.000000 redvox-pandas-1.4.2/redpandas/redpd_iterator.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     7874 2022-07-07 20:44:53.000000 redvox-pandas-1.4.2/redpandas/redpd_orientation.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-05-23 20:16:35.861973 redvox-pandas-1.4.2/redpandas/redpd_plot/
+-rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-08-03 22:13:07.000000 redvox-pandas-1.4.2/redpandas/redpd_plot/__init__.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4423 2021-08-03 22:13:07.000000 redvox-pandas-1.4.2/redpandas/redpd_plot/coherence.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    33263 2023-04-27 21:26:25.000000 redvox-pandas-1.4.2/redpandas/redpd_plot/mesh.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)      467 2021-10-18 19:57:34.000000 redvox-pandas-1.4.2/redpandas/redpd_plot/parameters.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    35442 2023-04-27 21:26:25.000000 redvox-pandas-1.4.2/redpandas/redpd_plot/wiggles.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    15627 2023-04-27 21:26:25.000000 redvox-pandas-1.4.2/redpandas/redpd_preprocess.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     8703 2023-04-27 21:26:25.000000 redvox-pandas-1.4.2/redpandas/redpd_report.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     1482 2022-07-07 20:44:53.000000 redvox-pandas-1.4.2/redpandas/redpd_scales.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)       80 2022-07-07 20:44:53.000000 redvox-pandas-1.4.2/redpandas/redpd_state.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    15899 2023-04-27 21:26:25.000000 redvox-pandas-1.4.2/redpandas/redpd_tfr.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    21018 2022-07-07 20:44:53.000000 redvox-pandas-1.4.2/redpandas/redpd_xcorr.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-05-23 20:16:35.862973 redvox-pandas-1.4.2/redvox_pandas.egg-info/
+-rw-rw-r--   0 opq       (1000) opq       (1000)    15648 2023-05-23 20:16:35.000000 redvox-pandas-1.4.2/redvox_pandas.egg-info/PKG-INFO
+-rw-rw-r--   0 opq       (1000) opq       (1000)      908 2023-05-23 20:16:35.000000 redvox-pandas-1.4.2/redvox_pandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 opq       (1000) opq       (1000)        1 2023-05-23 20:16:35.000000 redvox-pandas-1.4.2/redvox_pandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 opq       (1000) opq       (1000)       96 2023-05-23 20:16:35.000000 redvox-pandas-1.4.2/redvox_pandas.egg-info/requires.txt
+-rw-rw-r--   0 opq       (1000) opq       (1000)       10 2023-05-23 20:16:35.000000 redvox-pandas-1.4.2/redvox_pandas.egg-info/top_level.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-05-23 20:16:35.862973 redvox-pandas-1.4.2/setup.cfg
```

### Comparing `redvox-pandas-1.4.1/LICENSE` & `redvox-pandas-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/PKG-INFO` & `redvox-pandas-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redvox-pandas
-Version: 1.4.1
+Version: 1.4.2
 Summary: Library to streamline preprocessing of RedVox API 900 and API 1000 data
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `redvox-pandas-1.4.1/README.md` & `redvox-pandas-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/pyproject.toml` & `redvox-pandas-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # See:
 # - https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 # - https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 
 [project]
 name = "redvox-pandas"
-version = "1.4.1"
+version = "1.4.2"
 authors = [
     { name = "RedVox, Inc", email = "support@redvox.io" }
 ]
 description = "Library to streamline preprocessing of RedVox API 900 and API 1000 data"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 
 dependencies = [
     "obspy==1.4.0",
     "pymap3d==3.0.1",
-    "redvox==3.4.0",
+    "redvox==3.4.2",
     "redvox-base[matplotlib,numpy,pandas,scipy]==2023.4.27"
 ]
 
 [project.urls]
 homepage = "https://github.com/RedVoxInc/redpandas"
 PyPI = "https://pypi.org/project/redpandas/"
```

### Comparing `redvox-pandas-1.4.1/redpandas/redpd_build_station.py` & `redvox-pandas-1.4.2/redpandas/redpd_build_station.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/redpandas/redpd_cohere.py` & `redvox-pandas-1.4.2/redpandas/redpd_cohere.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/redpandas/redpd_config.py` & `redvox-pandas-1.4.2/redpandas/redpd_config.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/redpandas/redpd_datawin.py` & `redvox-pandas-1.4.2/redpandas/redpd_datawin.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/redpandas/redpd_df.py` & `redvox-pandas-1.4.2/redpandas/redpd_df.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/redpandas/redpd_dq.py` & `redvox-pandas-1.4.2/redpandas/redpd_dq.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/redpandas/redpd_ensonify.py` & `redvox-pandas-1.4.2/redpandas/redpd_ensonify.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/redpandas/redpd_filter.py` & `redvox-pandas-1.4.2/redpandas/redpd_filter.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/redpandas/redpd_geospatial.py` & `redvox-pandas-1.4.2/redpandas/redpd_geospatial.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/redpandas/redpd_gravity.py` & `redvox-pandas-1.4.2/redpandas/redpd_gravity.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/redpandas/redpd_iterator.py` & `redvox-pandas-1.4.2/redpandas/redpd_iterator.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/redpandas/redpd_orientation.py` & `redvox-pandas-1.4.2/redpandas/redpd_orientation.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/redpandas/redpd_plot/coherence.py` & `redvox-pandas-1.4.2/redpandas/redpd_plot/coherence.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/redpandas/redpd_plot/mesh.py` & `redvox-pandas-1.4.2/redpandas/redpd_plot/mesh.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/redpandas/redpd_plot/wiggles.py` & `redvox-pandas-1.4.2/redpandas/redpd_plot/wiggles.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/redpandas/redpd_preprocess.py` & `redvox-pandas-1.4.2/redpandas/redpd_preprocess.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/redpandas/redpd_report.py` & `redvox-pandas-1.4.2/redpandas/redpd_report.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/redpandas/redpd_scales.py` & `redvox-pandas-1.4.2/redpandas/redpd_scales.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/redpandas/redpd_tfr.py` & `redvox-pandas-1.4.2/redpandas/redpd_tfr.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/redpandas/redpd_xcorr.py` & `redvox-pandas-1.4.2/redpandas/redpd_xcorr.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.1/redvox_pandas.egg-info/PKG-INFO` & `redvox-pandas-1.4.2/redvox_pandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redvox-pandas
-Version: 1.4.1
+Version: 1.4.2
 Summary: Library to streamline preprocessing of RedVox API 900 and API 1000 data
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `redvox-pandas-1.4.1/redvox_pandas.egg-info/SOURCES.txt` & `redvox-pandas-1.4.2/redvox_pandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

