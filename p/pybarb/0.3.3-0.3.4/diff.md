# Comparing `tmp/pybarb-0.3.3.tar.gz` & `tmp/pybarb-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybarb-0.3.3.tar", last modified: Fri May 12 12:43:08 2023, max compression
+gzip compressed data, was "pybarb-0.3.4.tar", last modified: Tue May 23 20:14:06 2023, max compression
```

## Comparing `pybarb-0.3.3.tar` & `pybarb-0.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-12 12:43:08.877211 pybarb-0.3.3/
--rw-r--r--   0 simon_business   (501) staff       (20)      245 2023-05-12 12:43:08.876983 pybarb-0.3.3/PKG-INFO
--rw-r--r--   0 simon_business   (501) staff       (20)     2744 2023-04-25 15:40:48.000000 pybarb-0.3.3/README.md
-drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-12 12:43:08.874796 pybarb-0.3.3/pybarb/
--rw-r--r--   0 simon_business   (501) staff       (20)       21 2023-05-12 12:41:57.000000 pybarb-0.3.3/pybarb/__init__.py
--rw-r--r--   0 simon_business   (501) staff       (20)    23770 2023-04-25 15:18:38.000000 pybarb-0.3.3/pybarb/pybarb.py
-drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-12 12:43:08.876606 pybarb-0.3.3/pybarb.egg-info/
--rw-r--r--   0 simon_business   (501) staff       (20)      245 2023-05-12 12:43:08.000000 pybarb-0.3.3/pybarb.egg-info/PKG-INFO
--rw-r--r--   0 simon_business   (501) staff       (20)      203 2023-05-12 12:43:08.000000 pybarb-0.3.3/pybarb.egg-info/SOURCES.txt
--rw-r--r--   0 simon_business   (501) staff       (20)        1 2023-05-12 12:43:08.000000 pybarb-0.3.3/pybarb.egg-info/dependency_links.txt
--rw-r--r--   0 simon_business   (501) staff       (20)       34 2023-05-12 12:43:08.000000 pybarb-0.3.3/pybarb.egg-info/requires.txt
--rw-r--r--   0 simon_business   (501) staff       (20)        7 2023-05-12 12:43:08.000000 pybarb-0.3.3/pybarb.egg-info/top_level.txt
--rw-r--r--   0 simon_business   (501) staff       (20)       38 2023-05-12 12:43:08.877304 pybarb-0.3.3/setup.cfg
--rw-r--r--   0 simon_business   (501) staff       (20)      404 2023-05-12 12:42:25.000000 pybarb-0.3.3/setup.py
+drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-23 20:14:06.785958 pybarb-0.3.4/
+-rw-r--r--   0 simon_business   (501) staff       (20)      245 2023-05-23 20:14:06.785727 pybarb-0.3.4/PKG-INFO
+-rw-r--r--   0 simon_business   (501) staff       (20)     2743 2023-05-23 20:06:36.000000 pybarb-0.3.4/README.md
+drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-23 20:14:06.783137 pybarb-0.3.4/pybarb/
+-rw-r--r--   0 simon_business   (501) staff       (20)       21 2023-05-12 12:41:57.000000 pybarb-0.3.4/pybarb/__init__.py
+-rw-r--r--   0 simon_business   (501) staff       (20)    24060 2023-05-23 19:59:41.000000 pybarb-0.3.4/pybarb/pybarb.py
+drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-23 20:14:06.785276 pybarb-0.3.4/pybarb.egg-info/
+-rw-r--r--   0 simon_business   (501) staff       (20)      245 2023-05-23 20:14:06.000000 pybarb-0.3.4/pybarb.egg-info/PKG-INFO
+-rw-r--r--   0 simon_business   (501) staff       (20)      203 2023-05-23 20:14:06.000000 pybarb-0.3.4/pybarb.egg-info/SOURCES.txt
+-rw-r--r--   0 simon_business   (501) staff       (20)        1 2023-05-23 20:14:06.000000 pybarb-0.3.4/pybarb.egg-info/dependency_links.txt
+-rw-r--r--   0 simon_business   (501) staff       (20)       34 2023-05-23 20:14:06.000000 pybarb-0.3.4/pybarb.egg-info/requires.txt
+-rw-r--r--   0 simon_business   (501) staff       (20)        7 2023-05-23 20:14:06.000000 pybarb-0.3.4/pybarb.egg-info/top_level.txt
+-rw-r--r--   0 simon_business   (501) staff       (20)       38 2023-05-23 20:14:06.786054 pybarb-0.3.4/setup.cfg
+-rw-r--r--   0 simon_business   (501) staff       (20)      404 2023-05-23 20:13:35.000000 pybarb-0.3.4/setup.py
```

### Comparing `pybarb-0.3.3/README.md` & `pybarb-0.3.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# barb_api
+# pybarb
+
 A python package for interacting with [BARB's web API](https://barb-api.co.uk/api-docs).
 
 ## About Barb
 
 Barb is the industry’s standard for understanding what people watch.
 
 Barb's hybrid approach integrates people-based panel data with census-level online viewing data. Barb's methodology enables them to deliver inclusive measurement of total identified viewing across all broadcast, VOD and video-sharing platforms, delivered onto and consumed via multiple platforms and devices.
```

### Comparing `pybarb-0.3.3/pybarb/pybarb.py` & `pybarb-0.3.4/pybarb/pybarb.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,15 +109,17 @@
 
             Returns:
                 ProgrammeRatingsResultSet: The programme ratings result set.
         """
 
         # The query parameters
         params = {"min_transmission_date": min_transmission_date, "max_transmission_date": max_transmission_date,
-                  "station_code": self.get_station_code(station), "panel_code": self.get_panel_code(panel), "consolidated": consolidated, "last_updated_greater_than": last_updated_greater_than, "use_reporting_days": use_reporting_days, "limit": limit}
+                  "station_code":  None if station is None else self.get_station_code(station),
+                  "panel_code":  None if panel is None else self.get_panel_code(panel),
+                  "consolidated": consolidated, "last_updated_greater_than": last_updated_greater_than, "use_reporting_days": use_reporting_days, "limit": limit}
 
         api_response_data = self.query_event_endpoint(
             "programme_ratings", params)
 
         return ProgrammeRatingsResultSet(api_response_data)
 
     def advertising_spots(self, min_transmission_date, max_transmission_date, station=None, panel=None, advertiser=None,
@@ -141,15 +143,16 @@
 
             Returns:
                 AdvertisingSpotsResultSet: The advertising spots result set.
         """
 
         # The query parameters
         params = {"min_transmission_date": min_transmission_date, "max_transmission_date": max_transmission_date,
-                  "station_code": self.get_station_code(station), "panel_code": self.get_panel_code(panel),
+                  "station_code": None if station is None else self.get_station_code(station), 
+                  "panel_code": None if panel is None else self.get_panel_code(panel),
                   "advertiser": advertiser, "buyer": buyer, "consolidated": consolidated,
                   "standardise_audiences": standardise_audiences, "use_reporting_days": use_reporting_days, "last_updated_greater_than": last_updated_greater_than,
                   "limit": limit}
 
         api_response_data = self.query_event_endpoint(
             "advertising_spots", params)
 
@@ -174,15 +177,16 @@
 
             Returns:
                 AudiencesByTimeResultSet: The audiences by time result set.
         """
 
         # The query parameters
         params = {"min_transmission_date": min_transmission_date, "max_transmission_date": max_transmission_date,
-                  "station_code": self.get_station_code(station), "panel_code": self.get_panel_code(panel),
+                  "station_code":  None if station is None else self.get_station_code(station),
+                  "panel_code":  None if panel is None else self.get_panel_code(panel),
                   "time_period_length": time_period_length, "viewing_status": viewing_status,
                   "use_polling_days": use_polling_days, "last_updated_greater_than": last_updated_greater_than,
                   "limit": limit}
 
         api_response_data = self.query_event_endpoint(
             "audiences_by_time", params)
 
@@ -205,17 +209,16 @@
         api_response_data = {"endpoint": "programme_ratings",
                              "events": r_json["events"],
                              "audience_categories": r_json["audience_categories"]}
         while r.headers.__contains__("X-Next"):
             x_next_url = r.headers["X-Next"]
             r = requests.get(url=x_next_url, headers=self.headers)
             r_json = r.json()
-            api_response_data["events"].append(r_json["events"])
-            api_response_data["audience_categories"].append(
-                r_json["audience_categories"])
+            api_response_data["events"] = api_response_data["events"] + r_json["events"]
+            api_response_data["audience_categories"] = api_response_data["audience_categories"]  + r_json["audience_categories"]
 
         return api_response_data
     
     def list_stations(self, regex_filter=None):
         """
         Lists the stations available in the API.
```

