# Comparing `tmp/bosch_alarm_mode2-0.3.3.tar.gz` & `tmp/bosch_alarm_mode2-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bosch_alarm_mode2-0.3.3.tar", max compression
+gzip compressed data, was "bosch_alarm_mode2-0.3.4.tar", max compression
```

## Comparing `bosch_alarm_mode2-0.3.3.tar` & `bosch_alarm_mode2-0.3.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       48 2023-05-21 02:31:10.469944 bosch_alarm_mode2-0.3.3/bosch_alarm_mode2/__init__.py
--rw-r--r--   0        0        0     2330 2023-05-21 03:21:31.913252 bosch_alarm_mode2-0.3.3/bosch_alarm_mode2/connection.py
--rw-r--r--   0        0        0     4265 2023-05-23 08:22:59.035419 bosch_alarm_mode2-0.3.3/bosch_alarm_mode2/const.py
--rw-r--r--   0        0        0    18725 2023-05-23 08:51:06.615405 bosch_alarm_mode2-0.3.3/bosch_alarm_mode2/panel.py
--rw-r--r--   0        0        0      262 2023-05-23 08:51:34.388738 bosch_alarm_mode2-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 bosch_alarm_mode2-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       48 2023-05-21 02:31:10.469944 bosch_alarm_mode2-0.3.4/bosch_alarm_mode2/__init__.py
+-rw-r--r--   0        0        0     2330 2023-05-21 03:21:31.913252 bosch_alarm_mode2-0.3.4/bosch_alarm_mode2/connection.py
+-rw-r--r--   0        0        0     4265 2023-05-23 08:22:59.035419 bosch_alarm_mode2-0.3.4/bosch_alarm_mode2/const.py
+-rw-r--r--   0        0        0    18877 2023-05-23 08:53:54.805404 bosch_alarm_mode2-0.3.4/bosch_alarm_mode2/panel.py
+-rw-r--r--   0        0        0      262 2023-05-23 08:54:39.298737 bosch_alarm_mode2-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 bosch_alarm_mode2-0.3.4/PKG-INFO
```

### Comparing `bosch_alarm_mode2-0.3.3/bosch_alarm_mode2/connection.py` & `bosch_alarm_mode2-0.3.4/bosch_alarm_mode2/connection.py`

 * *Files identical despite different names*

### Comparing `bosch_alarm_mode2-0.3.3/bosch_alarm_mode2/const.py` & `bosch_alarm_mode2-0.3.4/bosch_alarm_mode2/const.py`

 * *Files identical despite different names*

### Comparing `bosch_alarm_mode2-0.3.3/bosch_alarm_mode2/panel.py` & `bosch_alarm_mode2-0.3.4/bosch_alarm_mode2/panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,31 +343,35 @@
             data = await self._connection.send_command(name_cmd, request)
             name = data.split(b'\x00', 1)[0]
             if not name: break
             names[id] = name.decode('ascii')
         print(names)
         return names
 
-    async def _load_names(self, name_cmd, config_cmd, type) -> dict[int, str]:
-        if self._featureCommandRequestAreaTextCF03:
-            return await self._load_names_cf03(name_cmd)
-        
-        # CF01 will return names, even ones we don't have authrority over. This will give us a list of all
-        # Supported names and then we can update the names if cf01 is available
+    async def _load_configured_names(self, config_cmd, type):
         data = await self._connection.send_command(config_cmd)
         names = {}
         index = 0
         while data:
             b = data.pop(0)
             for i in range(8):
                 id = index + (8 - i)
                 if b & 1 != 0:
                     names[id] = f"{type}{id}"
                 b >>= 1
             index+=8
+        return names
+    async def _load_names(self, name_cmd, config_cmd, type) -> dict[int, str]:
+        if self._featureCommandRequestAreaTextCF03:
+            return await self._load_names_cf03(name_cmd)
+        
+        # CF01 will return names, even ones we don't have authrority over. This will give us a list of all
+        # Supported names and then we can update the names if cf01 is available
+        names = await self._load_configured_names(config_cmd, type)
+
         if self._featureCommandRequestAreaTextCF01:
             return await self._load_names_cf01(name_cmd, names)
 
         # And then if CF01 isn't available, we can just return a list of names
         return names
 
     async def _get_alarms_for_priority(self, priority, last_area=None, last_point=None):
```

