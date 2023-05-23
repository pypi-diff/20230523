# Comparing `tmp/openstef_dbc-3.6.8a4.tar.gz` & `tmp/openstef_dbc-3.6.8a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstef_dbc-3.6.8a4.tar", last modified: Tue May 23 14:28:28 2023, max compression
+gzip compressed data, was "openstef_dbc-3.6.8a5.tar", last modified: Tue May 23 15:43:37 2023, max compression
```

## Comparing `openstef_dbc-3.6.8a4.tar` & `openstef_dbc-3.6.8a5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:28:28.921095 openstef_dbc-3.6.8a4/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-23 14:28:28.921095 openstef_dbc-3.6.8a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:28:28.917095 openstef_dbc-3.6.8a4/openstef_dbc/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/data_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/ktp_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:28:28.917095 openstef_dbc-3.6.8a4/openstef_dbc/log/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/log/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/log/processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:28:28.917095 openstef_dbc-3.6.8a4/openstef_dbc/models/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/models/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/models/switch_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:28:28.921095 openstef_dbc-3.6.8a4/openstef_dbc/services/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/services/ems.py
--rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/services/model_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/services/prediction_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/services/predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/services/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/services/splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/services/systems.py
--rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/services/weather.py
--rw-r--r--   0 runner    (1001) docker     (123)    16596 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/services/write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:28:28.917095 openstef_dbc-3.6.8a4/openstef_dbc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-23 14:28:28.000000 openstef_dbc-3.6.8a4/openstef_dbc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-23 14:28:28.000000 openstef_dbc-3.6.8a4/openstef_dbc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:28:28.000000 openstef_dbc-3.6.8a4/openstef_dbc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-23 14:28:28.000000 openstef_dbc-3.6.8a4/openstef_dbc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 14:28:28.000000 openstef_dbc-3.6.8a4/openstef_dbc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-23 14:28:28.921095 openstef_dbc-3.6.8a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:43:37.148440 openstef_dbc-3.6.8a5/
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-23 15:43:37.148440 openstef_dbc-3.6.8a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:43:37.144439 openstef_dbc-3.6.8a5/openstef_dbc/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/data_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/ktp_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:43:37.148440 openstef_dbc-3.6.8a5/openstef_dbc/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/log/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/log/processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:43:37.148440 openstef_dbc-3.6.8a5/openstef_dbc/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/models/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/models/switch_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:43:37.148440 openstef_dbc-3.6.8a5/openstef_dbc/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/services/ems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/services/model_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/services/prediction_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/services/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/services/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/services/splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/services/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/services/weather.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/services/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/openstef_dbc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:43:37.144439 openstef_dbc-3.6.8a5/openstef_dbc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-23 15:43:37.000000 openstef_dbc-3.6.8a5/openstef_dbc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-23 15:43:37.000000 openstef_dbc-3.6.8a5/openstef_dbc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:43:37.000000 openstef_dbc-3.6.8a5/openstef_dbc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-23 15:43:37.000000 openstef_dbc-3.6.8a5/openstef_dbc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 15:43:37.000000 openstef_dbc-3.6.8a5/openstef_dbc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-23 15:43:37.148440 openstef_dbc-3.6.8a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-23 15:43:23.000000 openstef_dbc-3.6.8a5/setup.py
```

### Comparing `openstef_dbc-3.6.8a4/LICENSE` & `openstef_dbc-3.6.8a5/LICENSE`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a4/PKG-INFO` & `openstef_dbc-3.6.8a5/openstef_dbc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openstef_dbc
-Version: 3.6.8a4
+Name: openstef-dbc
+Version: 3.6.8a5
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openstef_dbc-3.6.8a4/README.md` & `openstef_dbc-3.6.8a5/README.md`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a4/openstef_dbc/__init__.py` & `openstef_dbc-3.6.8a5/openstef_dbc/__init__.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a4/openstef_dbc/data_interface.py` & `openstef_dbc-3.6.8a5/openstef_dbc/data_interface.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a4/openstef_dbc/database.py` & `openstef_dbc-3.6.8a5/openstef_dbc/database.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a4/openstef_dbc/ktp_api.py` & `openstef_dbc-3.6.8a5/openstef_dbc/ktp_api.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a4/openstef_dbc/log/logging.py` & `openstef_dbc-3.6.8a5/openstef_dbc/log/logging.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a4/openstef_dbc/log/processors.py` & `openstef_dbc-3.6.8a5/openstef_dbc/log/processors.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a4/openstef_dbc/models/measurement.py` & `openstef_dbc-3.6.8a5/openstef_dbc/models/measurement.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a4/openstef_dbc/services/ems.py` & `openstef_dbc-3.6.8a5/openstef_dbc/services/ems.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a4/openstef_dbc/services/model_input.py` & `openstef_dbc-3.6.8a5/openstef_dbc/services/model_input.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a4/openstef_dbc/services/prediction_job.py` & `openstef_dbc-3.6.8a5/openstef_dbc/services/prediction_job.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a4/openstef_dbc/services/predictions.py` & `openstef_dbc-3.6.8a5/openstef_dbc/services/predictions.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a4/openstef_dbc/services/predictor.py` & `openstef_dbc-3.6.8a5/openstef_dbc/services/predictor.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a4/openstef_dbc/services/splitting.py` & `openstef_dbc-3.6.8a5/openstef_dbc/services/splitting.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a4/openstef_dbc/services/systems.py` & `openstef_dbc-3.6.8a5/openstef_dbc/services/systems.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a4/openstef_dbc/services/weather.py` & `openstef_dbc-3.6.8a5/openstef_dbc/services/weather.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a4/openstef_dbc/services/write.py` & `openstef_dbc-3.6.8a5/openstef_dbc/services/write.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,21 +101,22 @@
         }
         # Generate casting dict for available quantiles
         p = re.compile(r"quantile_P\d\d")
         quantile_columns = [s for s in field_columns if p.match(s)]
         casting_dict.update(dict.fromkeys(quantile_columns, np.float64))
 
         # Check if we have all columns and not some extra
-        for k in casting_dict.keys():
+        casting_dict_columns = list(casting_dict.keys())
+        for k in casting_dict_columns:
             # Remove any casting dict entries that are not in the dataframe
             if k not in forecast.columns:
                 casting_dict.pop(k, None)
 
-        if (
-            casting_dict.keys() != forecast.columns.to_list()
+        if set(casting_dict.keys()) != set(
+            forecast.columns.to_list()
         ):  # Check if we have a type description for every column, if not raise an error
             raise ValueError(
                 "Got unexpected columns, unable to cast these columns in the correct datatype."
             )
 
         forecast = forecast.astype(casting_dict)
```

### Comparing `openstef_dbc-3.6.8a4/openstef_dbc/utils.py` & `openstef_dbc-3.6.8a5/openstef_dbc/utils.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a4/openstef_dbc.egg-info/PKG-INFO` & `openstef_dbc-3.6.8a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openstef-dbc
-Version: 3.6.8a4
+Name: openstef_dbc
+Version: 3.6.8a5
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openstef_dbc-3.6.8a4/openstef_dbc.egg-info/SOURCES.txt` & `openstef_dbc-3.6.8a5/openstef_dbc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a4/setup.py` & `openstef_dbc-3.6.8a5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def read_long_description_from_readme():
     with open("README.md", "r", encoding="utf-8") as fh:
         return fh.read()
 
 
 setup(
     name="openstef_dbc",
-    version="3.6.8a4",
+    version="3.6.8a5",
     packages=find_packages(include=["openstef_dbc", "openstef_dbc.*"]),
     description="Database Connection for OpenSTEF",
     long_description=read_long_description_from_readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/openstef/openstef-dbc",
     author="Alliander N.V",
     author_email="korte.termijn.prognoses@alliander.com",
```

