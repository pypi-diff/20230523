# Comparing `tmp/coolpandas-0.3.1.tar.gz` & `tmp/coolpandas-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolpandas-0.3.1.tar", last modified: Tue May 16 11:59:29 2023, max compression
+gzip compressed data, was "coolpandas-0.3.2.tar", last modified: Tue May 23 18:40:42 2023, max compression
```

## Comparing `coolpandas-0.3.1.tar` & `coolpandas-0.3.2.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:59:29.000074 coolpandas-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-16 11:59:15.000000 coolpandas-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-16 11:59:29.000074 coolpandas-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-16 11:59:15.000000 coolpandas-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:59:28.992074 coolpandas-0.3.1/coolpandas/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:59:28.996074 coolpandas-0.3.1/coolpandas/eda/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/eda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/eda/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/eda/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/eda/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/eda/features_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/eda/geo_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/eda/missing_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/eda/random_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/eda/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/eda/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/eda/value_counts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:59:28.996074 coolpandas-0.3.1/coolpandas/evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/evaluate/confusion_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:59:28.996074 coolpandas-0.3.1/coolpandas/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/plot/barplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/plot/boxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/plot/distplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/plot/geoplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/plot/lineplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/plot/mapplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/plot/style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:59:28.996074 coolpandas-0.3.1/coolpandas/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/transform/bin.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/transform/epoch.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/transform/missing_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/transform/outliers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:59:29.000074 coolpandas-0.3.1/coolpandas/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-16 11:59:15.000000 coolpandas-0.3.1/coolpandas/utils/random_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:59:28.996074 coolpandas-0.3.1/coolpandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-16 11:59:28.000000 coolpandas-0.3.1/coolpandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-16 11:59:28.000000 coolpandas-0.3.1/coolpandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 11:59:28.000000 coolpandas-0.3.1/coolpandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-16 11:59:28.000000 coolpandas-0.3.1/coolpandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-16 11:59:28.000000 coolpandas-0.3.1/coolpandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-16 11:59:15.000000 coolpandas-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 11:59:29.000074 coolpandas-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:40:42.396992 coolpandas-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-23 18:40:31.000000 coolpandas-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-23 18:40:42.396992 coolpandas-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-23 18:40:31.000000 coolpandas-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:40:42.388992 coolpandas-0.3.2/coolpandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:40:42.392992 coolpandas-0.3.2/coolpandas/connect/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/connect/redshift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:40:42.392992 coolpandas-0.3.2/coolpandas/eda/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/features_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/geo_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/missing_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/random_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/eda/value_counts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:40:42.392992 coolpandas-0.3.2/coolpandas/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/evaluate/confusion_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:40:42.392992 coolpandas-0.3.2/coolpandas/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/plot/barplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/plot/boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/plot/distplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/plot/geoplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/plot/lineplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/plot/mapplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/plot/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:40:42.396992 coolpandas-0.3.2/coolpandas/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/transform/bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/transform/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/transform/missing_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/transform/outliers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:40:42.396992 coolpandas-0.3.2/coolpandas/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-23 18:40:31.000000 coolpandas-0.3.2/coolpandas/utils/random_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:40:42.392992 coolpandas-0.3.2/coolpandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-23 18:40:42.000000 coolpandas-0.3.2/coolpandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-23 18:40:42.000000 coolpandas-0.3.2/coolpandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:40:42.000000 coolpandas-0.3.2/coolpandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-23 18:40:42.000000 coolpandas-0.3.2/coolpandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 18:40:42.000000 coolpandas-0.3.2/coolpandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-23 18:40:31.000000 coolpandas-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 18:40:42.396992 coolpandas-0.3.2/setup.cfg
```

### Comparing `coolpandas-0.3.1/LICENSE` & `coolpandas-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/PKG-INFO` & `coolpandas-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coolpandas
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python package for Exploratory Data Analysis.
 Author-email: Avel Docquin <adocquin@outlook.com>
 Project-URL: Homepage, https://github.com/adocquin/coolpandas
 Project-URL: Bug Tracker, https://github.com/adocquin/coolpandas/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `coolpandas-0.3.1/README.md` & `coolpandas-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas/eda/__init__.py` & `coolpandas-0.3.2/coolpandas/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas/eda/correlation.py` & `coolpandas-0.3.2/coolpandas/eda/correlation.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas/eda/distribution.py` & `coolpandas-0.3.2/coolpandas/eda/distribution.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas/eda/duplicates.py` & `coolpandas-0.3.2/coolpandas/eda/duplicates.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas/eda/features_type.py` & `coolpandas-0.3.2/coolpandas/eda/features_type.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas/eda/geo_distance.py` & `coolpandas-0.3.2/coolpandas/eda/geo_distance.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas/eda/missing_values.py` & `coolpandas-0.3.2/coolpandas/eda/missing_values.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas/eda/shape.py` & `coolpandas-0.3.2/coolpandas/eda/shape.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas/eda/summary.py` & `coolpandas-0.3.2/coolpandas/eda/summary.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas/eda/value_counts.py` & `coolpandas-0.3.2/coolpandas/eda/value_counts.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas/evaluate/confusion_matrix.py` & `coolpandas-0.3.2/coolpandas/evaluate/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas/plot/barplot.py` & `coolpandas-0.3.2/coolpandas/plot/barplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas/plot/boxplot.py` & `coolpandas-0.3.2/coolpandas/plot/boxplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas/plot/distplot.py` & `coolpandas-0.3.2/coolpandas/plot/distplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas/plot/geoplot.py` & `coolpandas-0.3.2/coolpandas/plot/geoplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas/plot/lineplot.py` & `coolpandas-0.3.2/coolpandas/plot/lineplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas/plot/mapplot.py` & `coolpandas-0.3.2/coolpandas/plot/mapplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas/plot/style.py` & `coolpandas-0.3.2/coolpandas/plot/style.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas/transform/bin.py` & `coolpandas-0.3.2/coolpandas/transform/bin.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas/transform/missing_values.py` & `coolpandas-0.3.2/coolpandas/transform/missing_values.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas/transform/outliers.py` & `coolpandas-0.3.2/coolpandas/transform/outliers.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.3.1/coolpandas.egg-info/PKG-INFO` & `coolpandas-0.3.2/coolpandas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coolpandas
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python package for Exploratory Data Analysis.
 Author-email: Avel Docquin <adocquin@outlook.com>
 Project-URL: Homepage, https://github.com/adocquin/coolpandas
 Project-URL: Bug Tracker, https://github.com/adocquin/coolpandas/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `coolpandas-0.3.1/coolpandas.egg-info/SOURCES.txt` & `coolpandas-0.3.2/coolpandas.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 pyproject.toml
 coolpandas/__init__.py
 coolpandas.egg-info/PKG-INFO
 coolpandas.egg-info/SOURCES.txt
 coolpandas.egg-info/dependency_links.txt
 coolpandas.egg-info/requires.txt
 coolpandas.egg-info/top_level.txt
+coolpandas/connect/__init__.py
+coolpandas/connect/redshift.py
 coolpandas/eda/__init__.py
 coolpandas/eda/correlation.py
 coolpandas/eda/distribution.py
 coolpandas/eda/duplicates.py
 coolpandas/eda/features_type.py
 coolpandas/eda/geo_distance.py
 coolpandas/eda/missing_values.py
```

### Comparing `coolpandas-0.3.1/pyproject.toml` & `coolpandas-0.3.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coolpandas"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="Avel Docquin", email="adocquin@outlook.com" },
   ]
 description = "A Python package for Exploratory Data Analysis."
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
@@ -40,14 +40,15 @@
 [project.urls]
 "Homepage" = "https://github.com/adocquin/coolpandas"
 "Bug Tracker" = "https://github.com/adocquin/coolpandas/issues"
 
 [tool.setuptools]
 packages = [
   "coolpandas",
+  "coolpandas.connect",
   "coolpandas.eda",
   "coolpandas.evaluate",
   "coolpandas.plot",
   "coolpandas.transform",
   "coolpandas.utils",
   ]
```

