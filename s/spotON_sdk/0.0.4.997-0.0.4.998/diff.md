# Comparing `tmp/spotON_sdk-0.0.4.997.tar.gz` & `tmp/spotON_sdk-0.0.4.998.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.4.997.tar", last modified: Tue May 23 18:22:55 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.4.998.tar", last modified: Tue May 23 18:27:51 2023, max compression
```

## Comparing `spotON_sdk-0.0.4.997.tar` & `spotON_sdk-0.0.4.998.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     6184 2023-05-21 14:30:18.248848 spotON_sdk-0.0.4.997/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.4.997/LICENSE
--rw-r--r--   0        0        0      355 2023-05-21 15:19:16.024161 spotON_sdk-0.0.4.997/pyproject.toml
--rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.4.997/spotON_sdk/Logic/Feedback/Feedback.py
--rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.4.997/spotON_sdk/Logic/Feedback/Sensors.py
--rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.4.997/spotON_sdk/Logic/Feedback/Units.py
--rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.4.997/spotON_sdk/Logic/Feedback/__init__.py
--rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.4.997/spotON_sdk/Logic/Output/Switchtypes.py
--rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.4.997/spotON_sdk/Logic/Output/__init__.py
--rw-r--r--   0        0        0     1993 2023-05-23 18:22:07.766571 spotON_sdk-0.0.4.997/spotON_sdk/Logic/Price/Price_Logic.py
--rw-r--r--   0        0        0      208 2023-05-23 09:21:46.713502 spotON_sdk-0.0.4.997/spotON_sdk/Logic/Price/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.4.997/spotON_sdk/Logic/Price/bidding_zones.py
--rw-r--r--   0        0        0     4709 2023-05-22 09:10:42.883983 spotON_sdk-0.0.4.997/spotON_sdk/Logic/Price/countries.py
--rw-r--r--   0        0        0     2248 2023-05-23 14:09:38.854446 spotON_sdk-0.0.4.997/spotON_sdk/Logic/Price/markets.py
--rw-r--r--   0        0        0     6957 2023-05-17 21:52:50.903007 spotON_sdk-0.0.4.997/spotON_sdk/Logic/Price/spotON_Areas.py
--rw-r--r--   0        0        0     1707 2023-05-23 17:31:16.945257 spotON_sdk-0.0.4.997/spotON_sdk/Logic/Price/timeframes.py
--rw-r--r--   0        0        0      144 2023-05-22 18:00:58.368103 spotON_sdk-0.0.4.997/spotON_sdk/Logic/__init__.py
--rw-r--r--   0        0        0      461 2023-05-23 18:22:46.242654 spotON_sdk-0.0.4.997/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.4.997/spotON_sdk/data_helpers/BestHour.py
--rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.4.997/spotON_sdk/data_helpers/__init__.py
--rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.4.997/spotON_sdk/data_helpers/dataframe_modifier.py
--rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.4.997/spotON_sdk/spotON_controller.py
--rw-r--r--   0        0        0      252 1970-01-01 00:00:00.000000 spotON_sdk-0.0.4.997/PKG-INFO
+-rw-r--r--   0        0        0     6184 2023-05-21 14:30:18.248848 spotON_sdk-0.0.4.998/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.4.998/LICENSE
+-rw-r--r--   0        0        0      355 2023-05-21 15:19:16.024161 spotON_sdk-0.0.4.998/pyproject.toml
+-rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.4.998/spotON_sdk/Logic/Feedback/Feedback.py
+-rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.4.998/spotON_sdk/Logic/Feedback/Sensors.py
+-rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.4.998/spotON_sdk/Logic/Feedback/Units.py
+-rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.4.998/spotON_sdk/Logic/Feedback/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.4.998/spotON_sdk/Logic/Output/Switchtypes.py
+-rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.4.998/spotON_sdk/Logic/Output/__init__.py
+-rw-r--r--   0        0        0     1947 2023-05-23 18:27:13.051697 spotON_sdk-0.0.4.998/spotON_sdk/Logic/Price/Price_Logic.py
+-rw-r--r--   0        0        0      208 2023-05-23 09:21:46.713502 spotON_sdk-0.0.4.998/spotON_sdk/Logic/Price/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.4.998/spotON_sdk/Logic/Price/bidding_zones.py
+-rw-r--r--   0        0        0     4709 2023-05-22 09:10:42.883983 spotON_sdk-0.0.4.998/spotON_sdk/Logic/Price/countries.py
+-rw-r--r--   0        0        0     2248 2023-05-23 14:09:38.854446 spotON_sdk-0.0.4.998/spotON_sdk/Logic/Price/markets.py
+-rw-r--r--   0        0        0     6957 2023-05-17 21:52:50.903007 spotON_sdk-0.0.4.998/spotON_sdk/Logic/Price/spotON_Areas.py
+-rw-r--r--   0        0        0     1707 2023-05-23 17:31:16.945257 spotON_sdk-0.0.4.998/spotON_sdk/Logic/Price/timeframes.py
+-rw-r--r--   0        0        0      144 2023-05-22 18:00:58.368103 spotON_sdk-0.0.4.998/spotON_sdk/Logic/__init__.py
+-rw-r--r--   0        0        0      461 2023-05-23 18:27:45.813958 spotON_sdk-0.0.4.998/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.4.998/spotON_sdk/data_helpers/BestHour.py
+-rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.4.998/spotON_sdk/data_helpers/__init__.py
+-rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.4.998/spotON_sdk/data_helpers/dataframe_modifier.py
+-rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.4.998/spotON_sdk/spotON_controller.py
+-rw-r--r--   0        0        0      252 1970-01-01 00:00:00.000000 spotON_sdk-0.0.4.998/PKG-INFO
```

### Comparing `spotON_sdk-0.0.4.997/.gitignore` & `spotON_sdk-0.0.4.998/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.997/LICENSE` & `spotON_sdk-0.0.4.998/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.997/spotON_sdk/Logic/Price/Price_Logic.py` & `spotON_sdk-0.0.4.998/spotON_sdk/Logic/Price/Price_Logic.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,22 @@
 from mimetypes import init
 from os import name
 from typing import List, Union
 from pydantic import BaseModel, Field, validator, root_validator
 from .timeframes import Timeframes,Timeframe
 from .markets import Market, Markets
 
-class Pricefinding(BaseModel):
-    pass
 
 
-class Interrupted_On_Time(Pricefinding):
+class Interrupted_On_Time(BaseModel):
     name: str = Field(default="Interrupted_On_Time",init = False)
     pass
 
 
-class Continuous_On_Time(Pricefinding):
+class Continuous_On_Time(BaseModel):
     name: str = Field(default="Continuous_On_Time",init = False)
     week: int = Field(default=None)
     best_hour: int = Field(default=None)
 
 
 class Price_Logic(BaseModel):
     nr_of_hours_on: int
```

### Comparing `spotON_sdk-0.0.4.997/spotON_sdk/Logic/Price/bidding_zones.py` & `spotON_sdk-0.0.4.998/spotON_sdk/Logic/Price/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.997/spotON_sdk/Logic/Price/countries.py` & `spotON_sdk-0.0.4.998/spotON_sdk/Logic/Price/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.997/spotON_sdk/Logic/Price/markets.py` & `spotON_sdk-0.0.4.998/spotON_sdk/Logic/Price/markets.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.997/spotON_sdk/Logic/Price/spotON_Areas.py` & `spotON_sdk-0.0.4.998/spotON_sdk/Logic/Price/spotON_Areas.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.997/spotON_sdk/Logic/Price/timeframes.py` & `spotON_sdk-0.0.4.998/spotON_sdk/Logic/Price/timeframes.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.997/spotON_sdk/data_helpers/BestHour.py` & `spotON_sdk-0.0.4.998/spotON_sdk/data_helpers/BestHour.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.997/spotON_sdk/data_helpers/dataframe_modifier.py` & `spotON_sdk-0.0.4.998/spotON_sdk/data_helpers/dataframe_modifier.py`

 * *Files identical despite different names*

