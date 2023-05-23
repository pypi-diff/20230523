# Comparing `tmp/openstef_dbc-3.6.8a2.tar.gz` & `tmp/openstef_dbc-3.6.8a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstef_dbc-3.6.8a2.tar", last modified: Mon May 22 08:43:22 2023, max compression
+gzip compressed data, was "openstef_dbc-3.6.8a4.tar", last modified: Tue May 23 14:28:28 2023, max compression
```

## Comparing `openstef_dbc-3.6.8a2.tar` & `openstef_dbc-3.6.8a4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:43:22.118004 openstef_dbc-3.6.8a2/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-22 08:43:22.118004 openstef_dbc-3.6.8a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:43:22.114004 openstef_dbc-3.6.8a2/openstef_dbc/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/data_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/ktp_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:43:22.114004 openstef_dbc-3.6.8a2/openstef_dbc/log/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/log/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/log/processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:43:22.114004 openstef_dbc-3.6.8a2/openstef_dbc/models/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/models/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/models/switch_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:43:22.118004 openstef_dbc-3.6.8a2/openstef_dbc/services/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/services/ems.py
--rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/services/model_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/services/prediction_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/services/predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/services/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/services/splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/services/systems.py
--rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/services/weather.py
--rw-r--r--   0 runner    (1001) docker     (123)    16002 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/services/write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/openstef_dbc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:43:22.114004 openstef_dbc-3.6.8a2/openstef_dbc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-22 08:43:22.000000 openstef_dbc-3.6.8a2/openstef_dbc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-22 08:43:22.000000 openstef_dbc-3.6.8a2/openstef_dbc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:43:22.000000 openstef_dbc-3.6.8a2/openstef_dbc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-22 08:43:22.000000 openstef_dbc-3.6.8a2/openstef_dbc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 08:43:22.000000 openstef_dbc-3.6.8a2/openstef_dbc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-22 08:43:22.118004 openstef_dbc-3.6.8a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-22 08:43:07.000000 openstef_dbc-3.6.8a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:28:28.921095 openstef_dbc-3.6.8a4/
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-23 14:28:28.921095 openstef_dbc-3.6.8a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:28:28.917095 openstef_dbc-3.6.8a4/openstef_dbc/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/data_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/ktp_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:28:28.917095 openstef_dbc-3.6.8a4/openstef_dbc/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/log/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/log/processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:28:28.917095 openstef_dbc-3.6.8a4/openstef_dbc/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/models/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/models/switch_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:28:28.921095 openstef_dbc-3.6.8a4/openstef_dbc/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/services/ems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/services/model_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/services/prediction_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/services/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/services/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/services/splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/services/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/services/weather.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16596 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/services/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/openstef_dbc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:28:28.917095 openstef_dbc-3.6.8a4/openstef_dbc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-23 14:28:28.000000 openstef_dbc-3.6.8a4/openstef_dbc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-23 14:28:28.000000 openstef_dbc-3.6.8a4/openstef_dbc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:28:28.000000 openstef_dbc-3.6.8a4/openstef_dbc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-23 14:28:28.000000 openstef_dbc-3.6.8a4/openstef_dbc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 14:28:28.000000 openstef_dbc-3.6.8a4/openstef_dbc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-23 14:28:28.921095 openstef_dbc-3.6.8a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-23 14:28:16.000000 openstef_dbc-3.6.8a4/setup.py
```

### Comparing `openstef_dbc-3.6.8a2/LICENSE` & `openstef_dbc-3.6.8a4/LICENSE`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a2/PKG-INFO` & `openstef_dbc-3.6.8a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef_dbc
-Version: 3.6.8a2
+Version: 3.6.8a4
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openstef_dbc-3.6.8a2/README.md` & `openstef_dbc-3.6.8a4/README.md`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a2/openstef_dbc/__init__.py` & `openstef_dbc-3.6.8a4/openstef_dbc/__init__.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a2/openstef_dbc/data_interface.py` & `openstef_dbc-3.6.8a4/openstef_dbc/data_interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -175,14 +175,26 @@
 
         # Check if a value is nan
         if True in df.isna().values:
             nan_columns = df.columns[df.isna().any()].tolist()
             raise ValueError(
                 f"Dataframe contains NaN's. Found NaN's in columns: {nan_columns}"
             )
+        # Check if a value is inf
+        if True in df.isinf().values:
+            nan_columns = df.columns[df.isinf().any()].tolist()
+            raise ValueError(
+                f"Dataframe contains Inf's. Found Inf's in columns: {nan_columns}"
+            )
+
+        if True in df.isnull().values:
+            nan_columns = df.columns[df.isinf().any()].tolist()
+            raise ValueError(
+                f"Dataframe contains missing values. Found missing values in columns: {nan_columns}"
+            )
 
         try:
             self.influx_write_api.write(
                 record=df,
                 data_frame_measurement_name=measurement,
                 bucket=f"{database}/autogen",
                 data_frame_tag_columns=tag_columns,
```

### Comparing `openstef_dbc-3.6.8a2/openstef_dbc/database.py` & `openstef_dbc-3.6.8a4/openstef_dbc/database.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a2/openstef_dbc/ktp_api.py` & `openstef_dbc-3.6.8a4/openstef_dbc/ktp_api.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a2/openstef_dbc/log/logging.py` & `openstef_dbc-3.6.8a4/openstef_dbc/log/logging.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a2/openstef_dbc/log/processors.py` & `openstef_dbc-3.6.8a4/openstef_dbc/log/processors.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a2/openstef_dbc/models/measurement.py` & `openstef_dbc-3.6.8a4/openstef_dbc/models/measurement.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a2/openstef_dbc/services/ems.py` & `openstef_dbc-3.6.8a4/openstef_dbc/services/ems.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a2/openstef_dbc/services/model_input.py` & `openstef_dbc-3.6.8a4/openstef_dbc/services/model_input.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a2/openstef_dbc/services/prediction_job.py` & `openstef_dbc-3.6.8a4/openstef_dbc/services/prediction_job.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a2/openstef_dbc/services/predictions.py` & `openstef_dbc-3.6.8a4/openstef_dbc/services/predictions.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a2/openstef_dbc/services/predictor.py` & `openstef_dbc-3.6.8a4/openstef_dbc/services/predictor.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a2/openstef_dbc/services/splitting.py` & `openstef_dbc-3.6.8a4/openstef_dbc/services/splitting.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a2/openstef_dbc/services/systems.py` & `openstef_dbc-3.6.8a4/openstef_dbc/services/systems.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a2/openstef_dbc/services/weather.py` & `openstef_dbc-3.6.8a4/openstef_dbc/services/weather.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a2/openstef_dbc/services/write.py` & `openstef_dbc-3.6.8a4/openstef_dbc/services/write.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-FileCopyrightText: 2017-2022 Contributors to the OpenSTEF project <korte.termijn.prognoses@alliander.com>
 #
 # SPDX-License-Identifier: MPL-2.0
 
 from typing import Tuple, List
 from datetime import datetime
 import time
+import re
 
 import numpy as np
 import pandas as pd
 
 from openstef_dbc.data_interface import _DataInterface
 from openstef_dbc.log import logging
 
@@ -79,40 +80,58 @@
         # Write DataFrame to influx database
         # Find tag columns
         tag_columns = ["pid", "type", "customer"]
         # Specify field columns
         field_columns = [x for x in forecast.columns if x not in tag_columns]
 
         # Cast columns to correct type, as influx is extremely picky
-        casting_dict = {"prediction": float, "stdev": float}
-        for col, cast in casting_dict.items():
-            if col in field_columns:
-                forecast = forecast.astype({col: cast})
-
-        try:
-            result = _DataInterface.get_instance().exec_influx_write(
-                forecast.copy(),
-                database=dbname,
-                measurement=influxtable,
-                tag_columns=tag_columns,
-                field_columns=field_columns,
-                time_precision="s",
-            )
-        except Exception as e:
-            forecast = forecast.rename(columns={"created": "created_temp"})
-            field_columns = [x for x in forecast.columns if x not in tag_columns]
-            result = _DataInterface.get_instance().exec_influx_write(
-                forecast.copy(),
-                database=dbname,
-                measurement=influxtable,
-                tag_columns=tag_columns,
-                field_columns=field_columns,
-                time_precision="s",
+        casting_dict = {
+            "prediction": np.float64,
+            "stdev": np.float64,
+            "pid": np.int64,
+            "type": str,
+            "customer": str,
+            "created": np.int64,
+            "algtype": str,
+            "description": str,
+            "forecast_solar": np.float64,
+            "forecast_wind_on_shore": np.float64,
+            "forecast_other": np.float64,
+            "forecast": np.float64,
+            "quality": str,
+        }
+        # Generate casting dict for available quantiles
+        p = re.compile(r"quantile_P\d\d")
+        quantile_columns = [s for s in field_columns if p.match(s)]
+        casting_dict.update(dict.fromkeys(quantile_columns, np.float64))
+
+        # Check if we have all columns and not some extra
+        for k in casting_dict.keys():
+            # Remove any casting dict entries that are not in the dataframe
+            if k not in forecast.columns:
+                casting_dict.pop(k, None)
+
+        if (
+            casting_dict.keys() != forecast.columns.to_list()
+        ):  # Check if we have a type description for every column, if not raise an error
+            raise ValueError(
+                "Got unexpected columns, unable to cast these columns in the correct datatype."
             )
 
+        forecast = forecast.astype(casting_dict)
+
+        result = _DataInterface.get_instance().exec_influx_write(
+            forecast.copy(),
+            database=dbname,
+            measurement=influxtable,
+            tag_columns=tag_columns,
+            field_columns=field_columns,
+            time_precision="s",
+        )
+
         message = ""
 
         if result:
             num_rows = str(len(forecast))
             self.logger.info(
                 "Succesfully written Forecast to database",
                 num_rows=num_rows,
```

### Comparing `openstef_dbc-3.6.8a2/openstef_dbc/utils.py` & `openstef_dbc-3.6.8a4/openstef_dbc/utils.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a2/openstef_dbc.egg-info/PKG-INFO` & `openstef_dbc-3.6.8a4/openstef_dbc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef-dbc
-Version: 3.6.8a2
+Version: 3.6.8a4
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openstef_dbc-3.6.8a2/openstef_dbc.egg-info/SOURCES.txt` & `openstef_dbc-3.6.8a4/openstef_dbc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a2/setup.py` & `openstef_dbc-3.6.8a4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def read_long_description_from_readme():
     with open("README.md", "r", encoding="utf-8") as fh:
         return fh.read()
 
 
 setup(
     name="openstef_dbc",
-    version="3.6.8a2",
+    version="3.6.8a4",
     packages=find_packages(include=["openstef_dbc", "openstef_dbc.*"]),
     description="Database Connection for OpenSTEF",
     long_description=read_long_description_from_readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/openstef/openstef-dbc",
     author="Alliander N.V",
     author_email="korte.termijn.prognoses@alliander.com",
```

