# Comparing `tmp/spotON_sdk-0.0.4.96.tar.gz` & `tmp/spotON_sdk-0.0.4.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.4.96.tar", last modified: Mon May 22 20:36:19 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.4.97.tar", last modified: Mon May 22 20:41:38 2023, max compression
```

## Comparing `spotON_sdk-0.0.4.96.tar` & `spotON_sdk-0.0.4.97.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     6184 2023-05-21 14:30:18.248848 spotON_sdk-0.0.4.96/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.4.96/LICENSE
--rw-r--r--   0        0        0      355 2023-05-21 15:19:16.024161 spotON_sdk-0.0.4.96/pyproject.toml
--rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Feedback/Feedback.py
--rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Feedback/Sensors.py
--rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Feedback/Units.py
--rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Feedback/__init__.py
--rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Output/Switchtypes.py
--rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Output/__init__.py
--rw-r--r--   0        0        0     3782 2023-05-22 20:31:00.223696 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/Price_Logic.py
--rw-r--r--   0        0        0      182 2023-05-22 17:37:25.105808 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/bidding_zones.py
--rw-r--r--   0        0        0     4709 2023-05-22 09:10:42.883983 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/countries.py
--rw-r--r--   0        0        0     2282 2023-05-22 09:10:36.501033 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/markets.py
--rw-r--r--   0        0        0     6957 2023-05-17 21:52:50.903007 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/spotON_Areas.py
--rw-r--r--   0        0        0      144 2023-05-22 18:00:58.368103 spotON_sdk-0.0.4.96/spotON_sdk/Logic/__init__.py
--rw-r--r--   0        0        0      460 2023-05-22 20:36:14.746669 spotON_sdk-0.0.4.96/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.4.96/spotON_sdk/data_helpers/BestHour.py
--rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.4.96/spotON_sdk/data_helpers/__init__.py
--rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.4.96/spotON_sdk/data_helpers/dataframe_modifier.py
--rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.4.96/spotON_sdk/spotON_controller.py
--rw-r--r--   0        0        0      251 1970-01-01 00:00:00.000000 spotON_sdk-0.0.4.96/PKG-INFO
+-rw-r--r--   0        0        0     6184 2023-05-21 14:30:18.248848 spotON_sdk-0.0.4.97/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.4.97/LICENSE
+-rw-r--r--   0        0        0      355 2023-05-21 15:19:16.024161 spotON_sdk-0.0.4.97/pyproject.toml
+-rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.4.97/spotON_sdk/Logic/Feedback/Feedback.py
+-rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.4.97/spotON_sdk/Logic/Feedback/Sensors.py
+-rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.4.97/spotON_sdk/Logic/Feedback/Units.py
+-rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.4.97/spotON_sdk/Logic/Feedback/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.4.97/spotON_sdk/Logic/Output/Switchtypes.py
+-rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.4.97/spotON_sdk/Logic/Output/__init__.py
+-rw-r--r--   0        0        0     3797 2023-05-22 20:41:22.144767 spotON_sdk-0.0.4.97/spotON_sdk/Logic/Price/Price_Logic.py
+-rw-r--r--   0        0        0      182 2023-05-22 17:37:25.105808 spotON_sdk-0.0.4.97/spotON_sdk/Logic/Price/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.4.97/spotON_sdk/Logic/Price/bidding_zones.py
+-rw-r--r--   0        0        0     4709 2023-05-22 09:10:42.883983 spotON_sdk-0.0.4.97/spotON_sdk/Logic/Price/countries.py
+-rw-r--r--   0        0        0     2282 2023-05-22 09:10:36.501033 spotON_sdk-0.0.4.97/spotON_sdk/Logic/Price/markets.py
+-rw-r--r--   0        0        0     6957 2023-05-17 21:52:50.903007 spotON_sdk-0.0.4.97/spotON_sdk/Logic/Price/spotON_Areas.py
+-rw-r--r--   0        0        0      144 2023-05-22 18:00:58.368103 spotON_sdk-0.0.4.97/spotON_sdk/Logic/__init__.py
+-rw-r--r--   0        0        0      460 2023-05-22 20:41:31.231852 spotON_sdk-0.0.4.97/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.4.97/spotON_sdk/data_helpers/BestHour.py
+-rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.4.97/spotON_sdk/data_helpers/__init__.py
+-rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.4.97/spotON_sdk/data_helpers/dataframe_modifier.py
+-rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.4.97/spotON_sdk/spotON_controller.py
+-rw-r--r--   0        0        0      251 1970-01-01 00:00:00.000000 spotON_sdk-0.0.4.97/PKG-INFO
```

### Comparing `spotON_sdk-0.0.4.96/.gitignore` & `spotON_sdk-0.0.4.97/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.96/LICENSE` & `spotON_sdk-0.0.4.97/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/Price_Logic.py` & `spotON_sdk-0.0.4.97/spotON_sdk/Logic/Price/Price_Logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,40 +32,40 @@
             loop_Hours(start,25)
             loop_Hours(0,end)
 
 class Wholeday(Timeframe):
     possibel_hours : List[int] = Field(default_factory=lambda :  [*range(0,24)],init=False)
 
 
-class On_Hours(BaseModel):
+'''class On_Hours(BaseModel):
     timeframes_list : List[Timeframe] = Field(default_factory=list)
     first_timeframe : Timeframe = Field(default_factory=lambda: Wholeday())
 
     # add root validator that adds a variable first_timeframe that retrieves the first timeframe in the timeframes_list
     @root_validator(pre=True)
     def set_first_timeframe(cls, values):
         values["first_timeframe"] = values["timeframes_list"][0]
         return values
     
-    pass
+    pass'''
 
 class Pricefinding(BaseModel):
     pass
 
 class Interrupted(Pricefinding):
     pass
 
 class Continuous(Pricefinding):
     week :int = Field(default=None)
     bestHour :int = Field(default=None)
 
 class Price_Logic(BaseModel):
     nr_of_hours_on: int
     market: Union[str, Market] 
-    on_hours: On_Hours = Field(default_factory=lambda: On_Hours())
+    on_hours: List[Timeframe] = Field(default_factory=lambda: [Wholeday()])
     pricefinding : Continuous | Interrupted = Field(default_factory=lambda: Interrupted())
 
     resolution: float = Field(default=1)
     timeframe_longer_than_nr_of_hours_on :bool = Field(default=False)
     # root validator to set the market to the correct market object if it is a string
     @root_validator(pre=True)
     def set_market_to_market_object(cls, values):
```

### Comparing `spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/bidding_zones.py` & `spotON_sdk-0.0.4.97/spotON_sdk/Logic/Price/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/countries.py` & `spotON_sdk-0.0.4.97/spotON_sdk/Logic/Price/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/markets.py` & `spotON_sdk-0.0.4.97/spotON_sdk/Logic/Price/markets.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/spotON_Areas.py` & `spotON_sdk-0.0.4.97/spotON_sdk/Logic/Price/spotON_Areas.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.96/spotON_sdk/data_helpers/BestHour.py` & `spotON_sdk-0.0.4.97/spotON_sdk/data_helpers/BestHour.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.96/spotON_sdk/data_helpers/dataframe_modifier.py` & `spotON_sdk-0.0.4.97/spotON_sdk/data_helpers/dataframe_modifier.py`

 * *Files identical despite different names*

