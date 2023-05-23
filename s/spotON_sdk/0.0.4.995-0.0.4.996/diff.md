# Comparing `tmp/spotON_sdk-0.0.4.995.tar.gz` & `tmp/spotON_sdk-0.0.4.996.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.4.995.tar", last modified: Tue May 23 17:28:41 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.4.996.tar", last modified: Tue May 23 17:31:21 2023, max compression
```

## Comparing `spotON_sdk-0.0.4.995.tar` & `spotON_sdk-0.0.4.996.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     6184 2023-05-21 14:30:18.248848 spotON_sdk-0.0.4.995/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.4.995/LICENSE
--rw-r--r--   0        0        0      355 2023-05-21 15:19:16.024161 spotON_sdk-0.0.4.995/pyproject.toml
--rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.4.995/spotON_sdk/Logic/Feedback/Feedback.py
--rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.4.995/spotON_sdk/Logic/Feedback/Sensors.py
--rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.4.995/spotON_sdk/Logic/Feedback/Units.py
--rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.4.995/spotON_sdk/Logic/Feedback/__init__.py
--rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.4.995/spotON_sdk/Logic/Output/Switchtypes.py
--rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.4.995/spotON_sdk/Logic/Output/__init__.py
--rw-r--r--   0        0        0     2102 2023-05-23 17:15:32.150907 spotON_sdk-0.0.4.995/spotON_sdk/Logic/Price/Price_Logic.py
--rw-r--r--   0        0        0      208 2023-05-23 09:21:46.713502 spotON_sdk-0.0.4.995/spotON_sdk/Logic/Price/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.4.995/spotON_sdk/Logic/Price/bidding_zones.py
--rw-r--r--   0        0        0     4709 2023-05-22 09:10:42.883983 spotON_sdk-0.0.4.995/spotON_sdk/Logic/Price/countries.py
--rw-r--r--   0        0        0     2248 2023-05-23 14:09:38.854446 spotON_sdk-0.0.4.995/spotON_sdk/Logic/Price/markets.py
--rw-r--r--   0        0        0     6957 2023-05-17 21:52:50.903007 spotON_sdk-0.0.4.995/spotON_sdk/Logic/Price/spotON_Areas.py
--rw-r--r--   0        0        0     1616 2023-05-23 17:11:37.969467 spotON_sdk-0.0.4.995/spotON_sdk/Logic/Price/timeframes.py
--rw-r--r--   0        0        0      144 2023-05-22 18:00:58.368103 spotON_sdk-0.0.4.995/spotON_sdk/Logic/__init__.py
--rw-r--r--   0        0        0      461 2023-05-23 17:28:36.076204 spotON_sdk-0.0.4.995/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.4.995/spotON_sdk/data_helpers/BestHour.py
--rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.4.995/spotON_sdk/data_helpers/__init__.py
--rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.4.995/spotON_sdk/data_helpers/dataframe_modifier.py
--rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.4.995/spotON_sdk/spotON_controller.py
--rw-r--r--   0        0        0      252 1970-01-01 00:00:00.000000 spotON_sdk-0.0.4.995/PKG-INFO
+-rw-r--r--   0        0        0     6184 2023-05-21 14:30:18.248848 spotON_sdk-0.0.4.996/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.4.996/LICENSE
+-rw-r--r--   0        0        0      355 2023-05-21 15:19:16.024161 spotON_sdk-0.0.4.996/pyproject.toml
+-rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.4.996/spotON_sdk/Logic/Feedback/Feedback.py
+-rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.4.996/spotON_sdk/Logic/Feedback/Sensors.py
+-rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.4.996/spotON_sdk/Logic/Feedback/Units.py
+-rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.4.996/spotON_sdk/Logic/Feedback/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.4.996/spotON_sdk/Logic/Output/Switchtypes.py
+-rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.4.996/spotON_sdk/Logic/Output/__init__.py
+-rw-r--r--   0        0        0     2102 2023-05-23 17:15:32.150907 spotON_sdk-0.0.4.996/spotON_sdk/Logic/Price/Price_Logic.py
+-rw-r--r--   0        0        0      208 2023-05-23 09:21:46.713502 spotON_sdk-0.0.4.996/spotON_sdk/Logic/Price/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.4.996/spotON_sdk/Logic/Price/bidding_zones.py
+-rw-r--r--   0        0        0     4709 2023-05-22 09:10:42.883983 spotON_sdk-0.0.4.996/spotON_sdk/Logic/Price/countries.py
+-rw-r--r--   0        0        0     2248 2023-05-23 14:09:38.854446 spotON_sdk-0.0.4.996/spotON_sdk/Logic/Price/markets.py
+-rw-r--r--   0        0        0     6957 2023-05-17 21:52:50.903007 spotON_sdk-0.0.4.996/spotON_sdk/Logic/Price/spotON_Areas.py
+-rw-r--r--   0        0        0     1707 2023-05-23 17:31:16.945257 spotON_sdk-0.0.4.996/spotON_sdk/Logic/Price/timeframes.py
+-rw-r--r--   0        0        0      144 2023-05-22 18:00:58.368103 spotON_sdk-0.0.4.996/spotON_sdk/Logic/__init__.py
+-rw-r--r--   0        0        0      461 2023-05-23 17:30:43.451503 spotON_sdk-0.0.4.996/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.4.996/spotON_sdk/data_helpers/BestHour.py
+-rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.4.996/spotON_sdk/data_helpers/__init__.py
+-rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.4.996/spotON_sdk/data_helpers/dataframe_modifier.py
+-rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.4.996/spotON_sdk/spotON_controller.py
+-rw-r--r--   0        0        0      252 1970-01-01 00:00:00.000000 spotON_sdk-0.0.4.996/PKG-INFO
```

### Comparing `spotON_sdk-0.0.4.995/.gitignore` & `spotON_sdk-0.0.4.996/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.995/LICENSE` & `spotON_sdk-0.0.4.996/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.995/spotON_sdk/Logic/Price/Price_Logic.py` & `spotON_sdk-0.0.4.996/spotON_sdk/Logic/Price/Price_Logic.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.995/spotON_sdk/Logic/Price/bidding_zones.py` & `spotON_sdk-0.0.4.996/spotON_sdk/Logic/Price/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.995/spotON_sdk/Logic/Price/countries.py` & `spotON_sdk-0.0.4.996/spotON_sdk/Logic/Price/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.995/spotON_sdk/Logic/Price/markets.py` & `spotON_sdk-0.0.4.996/spotON_sdk/Logic/Price/markets.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.995/spotON_sdk/Logic/Price/spotON_Areas.py` & `spotON_sdk-0.0.4.996/spotON_sdk/Logic/Price/spotON_Areas.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.995/spotON_sdk/Logic/Price/timeframes.py` & `spotON_sdk-0.0.4.996/spotON_sdk/Logic/Price/timeframes.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 
 
     def add_timeframe(self, start: int, end: int):
         self.timeframes.append(Timeframe(start=start, end=end))
 
     def remove_timeframe(self, start: int, end: int):
         self.timeframes = [timeframe for timeframe in self.timeframes if not (timeframe.start == start and timeframe.end == end)]
+    
+    def remove_initial_timeframe(self):
+        self.timeframes = self.timeframes[1:]
 
     def set_whole_day(self):
         self.timeframes.append(Timeframe(start=0, end=23))
 
     def set_morning(self):
         self.timeframes.append(Timeframe(start=5, end=12))
```

### Comparing `spotON_sdk-0.0.4.995/spotON_sdk/data_helpers/BestHour.py` & `spotON_sdk-0.0.4.996/spotON_sdk/data_helpers/BestHour.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.995/spotON_sdk/data_helpers/dataframe_modifier.py` & `spotON_sdk-0.0.4.996/spotON_sdk/data_helpers/dataframe_modifier.py`

 * *Files identical despite different names*

