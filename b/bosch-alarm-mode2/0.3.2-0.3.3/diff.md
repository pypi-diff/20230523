# Comparing `tmp/bosch_alarm_mode2-0.3.2.tar.gz` & `tmp/bosch_alarm_mode2-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bosch_alarm_mode2-0.3.2.tar", max compression
+gzip compressed data, was "bosch_alarm_mode2-0.3.3.tar", max compression
```

## Comparing `bosch_alarm_mode2-0.3.2.tar` & `bosch_alarm_mode2-0.3.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       48 2023-05-21 02:31:10.469944 bosch_alarm_mode2-0.3.2/bosch_alarm_mode2/__init__.py
--rw-r--r--   0        0        0     2330 2023-05-21 03:21:31.913252 bosch_alarm_mode2-0.3.2/bosch_alarm_mode2/connection.py
--rw-r--r--   0        0        0     4220 2023-05-22 09:16:58.475238 bosch_alarm_mode2-0.3.2/bosch_alarm_mode2/const.py
--rw-r--r--   0        0        0    17857 2023-05-22 22:49:25.036597 bosch_alarm_mode2-0.3.2/bosch_alarm_mode2/panel.py
--rw-r--r--   0        0        0      262 2023-05-23 07:21:43.112117 bosch_alarm_mode2-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 bosch_alarm_mode2-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0       48 2023-05-21 02:31:10.469944 bosch_alarm_mode2-0.3.3/bosch_alarm_mode2/__init__.py
+-rw-r--r--   0        0        0     2330 2023-05-21 03:21:31.913252 bosch_alarm_mode2-0.3.3/bosch_alarm_mode2/connection.py
+-rw-r--r--   0        0        0     4265 2023-05-23 08:22:59.035419 bosch_alarm_mode2-0.3.3/bosch_alarm_mode2/const.py
+-rw-r--r--   0        0        0    18725 2023-05-23 08:51:06.615405 bosch_alarm_mode2-0.3.3/bosch_alarm_mode2/panel.py
+-rw-r--r--   0        0        0      262 2023-05-23 08:51:34.388738 bosch_alarm_mode2-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 bosch_alarm_mode2-0.3.3/PKG-INFO
```

### Comparing `bosch_alarm_mode2-0.3.2/bosch_alarm_mode2/connection.py` & `bosch_alarm_mode2-0.3.3/bosch_alarm_mode2/connection.py`

 * *Files identical despite different names*

### Comparing `bosch_alarm_mode2-0.3.2/bosch_alarm_mode2/const.py` & `bosch_alarm_mode2-0.3.3/bosch_alarm_mode2/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,16 @@
 
 class CMD:
     # Unauthenticated commands
     WHAT_ARE_YOU = 0x01
     AUTHENTICATE = 0x06
     LOGIN_REMOTE_USER = 0x3E
     # Area / Point Counts
-    PANEL_CAPACITIES = 0x1F
+    REQUEST_CONFIGURED_AREAS = 0x24
+    REQUEST_CONFIGURED_POINTS = 0x35
     # Alarm memory details
     ALARM_MEMORY_SUMMARY = 0x08
     ALARM_MEMORY_DETAIL = 0x23
     # Area group
     AREA_STATUS = 0x26
     AREA_ARM = 0x27
     AREA_TEXT = 0x29
```

### Comparing `bosch_alarm_mode2-0.3.2/bosch_alarm_mode2/panel.py` & `bosch_alarm_mode2-0.3.3/bosch_alarm_mode2/panel.py`

 * *Files 6% similar despite different names*

```diff
@@ -301,27 +301,28 @@
         
         data = await self._connection.send_command(CMD.WHAT_ARE_YOU, commandformat)
         self.model = PANEL_MODEL[data[0]]
         self.protocol_version = 'v%d.%d' % (data[5], data[6])
         if data[13]: LOG.warning('busy flag: %d', data[13])
         bitmask = data[23:].ljust(33, b'\0')
         self._featureProtocol02 = (bitmask[0] & 0x40) != 0
+        self._featureCommandRequestAreaTextCF01 = (bitmask[7] & 0x20) != 0
         self._featureCommandRequestAreaTextCF03 = (bitmask[7] & 0x08) != 0
         # Check if serial read command is supported before sending it
         if (bitmask[11] & 0x04) != 0:
             data = await self._connection.send_command(
                     CMD.PRODUCT_SERIAL, b'\x00\x00')
             self.serial_number = int.from_bytes(data[0:6], 'big')
 
     async def _load_areas(self):
-        names = await self._load_names(CMD.AREA_TEXT)
+        names = await self._load_names(CMD.AREA_TEXT, CMD.REQUEST_CONFIGURED_AREAS, "AREA")
         self.areas = {id: Area(name) for id, name in names.items()}
 
     async def _load_points(self):
-        names = await self._load_names(CMD.POINT_TEXT)
+        names = await self._load_names(CMD.POINT_TEXT, CMD.REQUEST_CONFIGURED_POINTS, "POINT")
         self.points = {id: Point(name) for id, name in names.items()}
 
     async def _load_names_cf03(self, name_cmd) -> dict[int, str]:
         names = {}
         id = 0
         while True:
             request = bytearray(id.to_bytes(2, 'big'))
@@ -331,30 +332,47 @@
             if not data: break
             while data:
                 id = _get_int16(data)
                 name, data = data[2:].split(b'\x00', 1)
                 names[id] = name.decode('ascii')
         return names
 
-    async def _load_names_cf01(self, name_cmd) -> dict[int, str]:
-        names = {}
-        for id in range(1, 255):
+    async def _load_names_cf01(self, name_cmd, names) -> dict[int, str]:
+        for id in names.keys():
             request = bytearray(id.to_bytes(2, 'big'))
             request.append(0x00)  # primary language
             data = await self._connection.send_command(name_cmd, request)
             name = data.split(b'\x00', 1)[0]
             if not name: break
             names[id] = name.decode('ascii')
+        print(names)
         return names
 
-    async def _load_names(self, name_cmd) -> dict[int, str]:
+    async def _load_names(self, name_cmd, config_cmd, type) -> dict[int, str]:
         if self._featureCommandRequestAreaTextCF03:
             return await self._load_names_cf03(name_cmd)
         
-        return await self._load_names_cf01(name_cmd)
+        # CF01 will return names, even ones we don't have authrority over. This will give us a list of all
+        # Supported names and then we can update the names if cf01 is available
+        data = await self._connection.send_command(config_cmd)
+        names = {}
+        index = 0
+        while data:
+            b = data.pop(0)
+            for i in range(8):
+                id = index + (8 - i)
+                if b & 1 != 0:
+                    names[id] = f"{type}{id}"
+                b >>= 1
+            index+=8
+        if self._featureCommandRequestAreaTextCF01:
+            return await self._load_names_cf01(name_cmd, names)
+
+        # And then if CF01 isn't available, we can just return a list of names
+        return names
 
     async def _get_alarms_for_priority(self, priority, last_area=None, last_point=None):
         request = bytearray([priority])
         if last_area and last_point:
             request.append(last_area.to_bytes(2, 'big'))
             request.append(last_point.to_bytes(2, 'big'))
         response_detail = await self._connection.send_command(CMD.ALARM_MEMORY_DETAIL, request)
```

