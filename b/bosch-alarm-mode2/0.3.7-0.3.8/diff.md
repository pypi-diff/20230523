# Comparing `tmp/bosch_alarm_mode2-0.3.7.tar.gz` & `tmp/bosch_alarm_mode2-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bosch_alarm_mode2-0.3.7.tar", max compression
+gzip compressed data, was "bosch_alarm_mode2-0.3.8.tar", max compression
```

## Comparing `bosch_alarm_mode2-0.3.7.tar` & `bosch_alarm_mode2-0.3.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       48 2023-05-21 02:31:10.469944 bosch_alarm_mode2-0.3.7/bosch_alarm_mode2/__init__.py
--rw-r--r--   0        0        0     2330 2023-05-21 03:21:31.913252 bosch_alarm_mode2-0.3.7/bosch_alarm_mode2/connection.py
--rw-r--r--   0        0        0     4700 2023-05-23 11:18:15.221998 bosch_alarm_mode2-0.3.7/bosch_alarm_mode2/const.py
--rw-r--r--   0        0        0    20319 2023-05-23 11:25:59.905327 bosch_alarm_mode2-0.3.7/bosch_alarm_mode2/panel.py
--rw-r--r--   0        0        0      262 2023-05-23 11:26:55.791994 bosch_alarm_mode2-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 bosch_alarm_mode2-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0       48 2023-05-21 02:31:10.469944 bosch_alarm_mode2-0.3.8/bosch_alarm_mode2/__init__.py
+-rw-r--r--   0        0        0     2330 2023-05-21 03:21:31.913252 bosch_alarm_mode2-0.3.8/bosch_alarm_mode2/connection.py
+-rw-r--r--   0        0        0     4700 2023-05-23 11:18:15.221998 bosch_alarm_mode2-0.3.8/bosch_alarm_mode2/const.py
+-rw-r--r--   0        0        0    20324 2023-05-23 12:06:52.689999 bosch_alarm_mode2-0.3.8/bosch_alarm_mode2/panel.py
+-rw-r--r--   0        0        0      262 2023-05-23 12:07:38.703332 bosch_alarm_mode2-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 bosch_alarm_mode2-0.3.8/PKG-INFO
```

### Comparing `bosch_alarm_mode2-0.3.7/bosch_alarm_mode2/connection.py` & `bosch_alarm_mode2-0.3.8/bosch_alarm_mode2/connection.py`

 * *Files identical despite different names*

### Comparing `bosch_alarm_mode2-0.3.7/bosch_alarm_mode2/const.py` & `bosch_alarm_mode2-0.3.8/bosch_alarm_mode2/const.py`

 * *Files identical despite different names*

### Comparing `bosch_alarm_mode2-0.3.7/bosch_alarm_mode2/panel.py` & `bosch_alarm_mode2-0.3.8/bosch_alarm_mode2/panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,27 +329,27 @@
     async def _load_areas(self):
         names = await self._load_names(CMD.AREA_TEXT, CMD.REQUEST_CONFIGURED_AREAS, "AREA")
         if not names:
             if self._featureCommandRequestAreaAuthorityCF01:
                 names = await self._load_configured_names(CMD.AREA_AUTHORITY, "AREA")
             # If none of the above methods work, then we just have to hardcode it
             else:
-                names = [f"AREA{x}" for x in range(1, 1 + self.max_areas)]
+                names = {x: f"AREA{x}" for x in range(1, 1 + self.max_areas)}
         self.areas = {id: Area(name) for id, name in names.items()}
 
     async def _load_points(self):
         names = await self._load_names(CMD.POINT_TEXT, CMD.REQUEST_CONFIGURED_POINTS, "ZONE")
         if not names:
             # Request points from all areas we have authority over
             if self._featureCommandRequestPointsInAreaCF01:
                 for area in self.areas.keys():
                     names.update(await self._load_configured_names(CMD.REQUEST_POINTS_IN_AREA, "ZONE", bytearray(area.to_bytes(2, 'big'))))
             # If none of the above methods work, then we just have to hardcode it
             else:
-                names = [f"ZONE{x}" for x in range(1, 1 + self.max_zones)]
+                names = {x:f"ZONE{x}" for x in range(1, 1 + self.max_zones)}
         self.points = {id: Point(name) for id, name in names.items()}
 
     async def _load_names_cf03(self, name_cmd) -> dict[int, str]:
         names = {}
         id = 0
         while True:
             request = bytearray(id.to_bytes(2, 'big'))
```

