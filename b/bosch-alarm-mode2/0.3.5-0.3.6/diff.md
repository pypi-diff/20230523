# Comparing `tmp/bosch_alarm_mode2-0.3.5.tar.gz` & `tmp/bosch_alarm_mode2-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bosch_alarm_mode2-0.3.5.tar", max compression
+gzip compressed data, was "bosch_alarm_mode2-0.3.6.tar", max compression
```

## Comparing `bosch_alarm_mode2-0.3.5.tar` & `bosch_alarm_mode2-0.3.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       48 2023-05-21 02:31:10.469944 bosch_alarm_mode2-0.3.5/bosch_alarm_mode2/__init__.py
--rw-r--r--   0        0        0     2330 2023-05-21 03:21:31.913252 bosch_alarm_mode2-0.3.5/bosch_alarm_mode2/connection.py
--rw-r--r--   0        0        0     4239 2023-05-23 09:09:59.112062 bosch_alarm_mode2-0.3.5/bosch_alarm_mode2/const.py
--rw-r--r--   0        0        0    18904 2023-05-23 09:41:01.625380 bosch_alarm_mode2-0.3.5/bosch_alarm_mode2/panel.py
--rw-r--r--   0        0        0      262 2023-05-23 09:42:41.498713 bosch_alarm_mode2-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 bosch_alarm_mode2-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0       48 2023-05-21 02:31:10.469944 bosch_alarm_mode2-0.3.6/bosch_alarm_mode2/__init__.py
+-rw-r--r--   0        0        0     2330 2023-05-21 03:21:31.913252 bosch_alarm_mode2-0.3.6/bosch_alarm_mode2/connection.py
+-rw-r--r--   0        0        0     4640 2023-05-23 10:37:29.185352 bosch_alarm_mode2-0.3.6/bosch_alarm_mode2/const.py
+-rw-r--r--   0        0        0    19547 2023-05-23 10:37:54.568685 bosch_alarm_mode2-0.3.6/bosch_alarm_mode2/panel.py
+-rw-r--r--   0        0        0      262 2023-05-23 10:38:07.872018 bosch_alarm_mode2-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 bosch_alarm_mode2-0.3.6/PKG-INFO
```

### Comparing `bosch_alarm_mode2-0.3.5/bosch_alarm_mode2/connection.py` & `bosch_alarm_mode2-0.3.6/bosch_alarm_mode2/connection.py`

 * *Files identical despite different names*

### Comparing `bosch_alarm_mode2-0.3.5/bosch_alarm_mode2/const.py` & `bosch_alarm_mode2-0.3.6/bosch_alarm_mode2/const.py`

 * *Files 18% similar despite different names*

```diff
@@ -57,14 +57,47 @@
     0xA4: "B5512 (US1B)",
     0xA6: "B8512G (US1A)",
     0xA7: "B9512G (US1A)",
     0xA8: "B3512 (US1B)",
     0xA9: "B6512 (US1B)",
 }
 
+PANEL_AREAS_MAX = {
+    0x20: 2,
+    0x21: 2,
+    0x22: 2,
+    0x23: 8,
+    0x24: 16,
+    0x79: 8,
+    0x84: 32,
+    0xA0: 2,
+    0xA4: 4,
+    0xA6: 8,
+    0xA7: 32,
+    0xA8: 1,
+    0xA9: 6,
+}
+
+PANEL_ZONES_MAX = {
+    0x20: 8,
+    0x21: 16,
+    0x22: 8,
+    0x23: 32,
+    0x24: 64,
+    0x79: 75,
+    0x84: 246,
+    0xA0: 28,
+    0xA4: 48,
+    0xA6: 99,
+    0xA7: 599,
+    0xA8: 16,
+    0xA9: 96,
+}
+
+
 AREA_STATUS_UNKNOWN = 0x00
 AREA_STATUS_DISARMED = 0x04
 AREA_STATUS_ARMING = [0x07, 0x08, 0x0D]
 AREA_STATUS_PENDING = [0x05, 0x06, 0x0E]
 AREA_STATUS_PART_ARMED = [0x02, 0x03]
 AREA_STATUS_ALL_ARMED = [0x01, 0x09, 0x0C]
```

### Comparing `bosch_alarm_mode2-0.3.5/bosch_alarm_mode2/panel.py` & `bosch_alarm_mode2-0.3.6/bosch_alarm_mode2/panel.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,18 +124,22 @@
         self._poll_task = None
 
         self.model = None
         self.protocol_version = None
         self.serial_number = None
         self.areas = {}
         self.points = {}
+        self.max_areas = 0
+        self.max_zones = 0
         self._part_arming_type = AREA_ARMING_PERIMETER_DELAY
         self._all_arming_type = AREA_ARMING_MASTER_DELAY
         self._featureProtocol02 = False
+        self._featureCommandRequestAreaTextCF01 = False
         self._featureCommandRequestAreaTextCF03 = False
+        self._featureCommandRequestConfiguredPointsCF01 = False
 
     LOAD_BASIC_INFO = 1 << 0
     LOAD_ENTITIES = 1 << 1
     LOAD_STATUS = 1 << 2
     LOAD_ALL = LOAD_BASIC_INFO | LOAD_ENTITIES | LOAD_STATUS
 
     async def connect(self, load_selector = LOAD_ALL):
@@ -287,46 +291,49 @@
         else:
             await self._authenticate_automation()
 
     async def _model(self):
         data = await self._connection.send_command(CMD.WHAT_ARE_YOU)
         self.model = PANEL_MODEL[data[0]]
         self.protocol_version = 'v%d.%d' % (data[5], data[6])
-        # Solution and IMAX panels use one set of arming types, B series panels use another.
+        # Solution and AMAX panels use one set of arming types, B series panels use another.
         if data[0] <= 0x24:
             self._part_arming_type = AREA_ARMING_STAY1
             self._all_arming_type = AREA_ARMING_AWAY
         else:
             self._part_arming_type = AREA_ARMING_PERIMETER_DELAY
             self._all_arming_type = AREA_ARMING_MASTER_DELAY
-
+        
     async def _basicinfo(self):
         commandformat = bytearray()
         commandformat.append(3)
         
         data = await self._connection.send_command(CMD.WHAT_ARE_YOU, commandformat)
         self.model = PANEL_MODEL[data[0]]
+        self.max_zones = PANEL_ZONES_MAX[data[0]]
+        self.max_areas = PANEL_AREAS_MAX[data[0]]
         self.protocol_version = 'v%d.%d' % (data[5], data[6])
         if data[13]: LOG.warning('busy flag: %d', data[13])
         bitmask = data[23:].ljust(33, b'\0')
         self._featureProtocol02 = (bitmask[0] & 0x40) != 0
         self._featureCommandRequestAreaTextCF01 = (bitmask[7] & 0x20) != 0
         self._featureCommandRequestAreaTextCF03 = (bitmask[7] & 0x08) != 0
+        self._featureCommandRequestConfiguredPointsCF01 = (bitmask[12] & 0x80) != 0
         # Check if serial read command is supported before sending it
         if (bitmask[11] & 0x04) != 0:
             data = await self._connection.send_command(
                     CMD.PRODUCT_SERIAL, b'\x00\x00')
             self.serial_number = int.from_bytes(data[0:6], 'big')
 
     async def _load_areas(self):
-        names = await self._load_names(CMD.AREA_TEXT, CMD.REQUEST_CONFIGURED_AREAS, "AREA")
+        names = await self._load_names(CMD.AREA_TEXT, CMD.REQUEST_CONFIGURED_AREAS, "AREA", self.max_areas)
         self.areas = {id: Area(name) for id, name in names.items()}
 
     async def _load_points(self):
-        names = await self._load_names(CMD.POINT_TEXT, CMD.REQUEST_CONFIGURED_POINTS, "POINT")
+        names = await self._load_names(CMD.POINT_TEXT, CMD.REQUEST_CONFIGURED_POINTS, "ZONE", self.max_zones)
         self.points = {id: Point(name) for id, name in names.items()}
 
     async def _load_names_cf03(self, name_cmd) -> dict[int, str]:
         names = {}
         id = 0
         while True:
             request = bytearray(id.to_bytes(2, 'big'))
@@ -358,24 +365,31 @@
             for i in range(8):
                 id = index + (8 - i)
                 if b & 1 != 0:
                     names[id] = f"{type}{id}"
                 b >>= 1
             index+=8
         return names
-    async def _load_names(self, name_cmd, config_cmd, type) -> dict[int, str]:
+    
+    async def _load_names(self, name_cmd, config_cmd, type, max) -> dict[int, str]:
         if self._featureCommandRequestAreaTextCF03:
             return await self._load_names_cf03(name_cmd)
         
-        names = await self._load_configured_names(config_cmd, type)
+        names = {}
+        
+        if self._featureCommandRequestConfiguredPointsCF01:
+            names = await self._load_configured_names(config_cmd, type)
 
         if self._featureCommandRequestAreaTextCF01:
             return await self._load_names_cf01(name_cmd, names)
+        
+        # If none of the above methods work, then we just have to hardcode it
+        if not self._featureCommandRequestConfiguredPointsCF01:
+            names = [f"{type}{x}" for x in range(1, 1 + max)]
 
-        # And then if CF01 isn't available, we can just return a list of names
         return names
 
     async def _get_alarms_for_priority(self, priority, last_area=None, last_point=None):
         request = bytearray([priority])
         if last_area and last_point:
             request.append(last_area.to_bytes(2, 'big'))
             request.append(last_point.to_bytes(2, 'big'))
@@ -409,15 +423,15 @@
         for id in entities.keys(): request.extend(id.to_bytes(2, 'big'))
         response = await self._connection.send_command(status_cmd, request)
         while response:
             entities[_get_int16(response)].status = response[2]
             response = response[3:]
 
     async def _area_arm(self, area_id, arm_type, code):
-        if self._arming_code != None and code != self._arming_code:
+        if self._arming_code != None and int(code) != int(self._arming_code):
             return
         request = bytearray([arm_type])
         # bitmask with only i-th bit from the left being 1 (section 3.1.4)
         request.extend(bytearray((area_id-1)//8)) # leading 0 bytes
         request.append(1<<(7-((area_id-1) % 8))) # i%8-th bit from the left (top) set
         await self._connection.send_command(CMD.AREA_ARM, request)
```

