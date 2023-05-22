# Comparing `tmp/bosch-control-panel-cc880p-3.1.4.tar.gz` & `tmp/bosch-control-panel-cc880p-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bosch-control-panel-cc880p-3.1.4.tar", last modified: Sat May 20 17:38:26 2023, max compression
+gzip compressed data, was "bosch-control-panel-cc880p-4.0.0.tar", last modified: Mon May 22 23:20:10 2023, max compression
```

## Comparing `bosch-control-panel-cc880p-3.1.4.tar` & `bosch-control-panel-cc880p-4.0.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:26.009485 bosch-control-panel-cc880p-3.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-20 17:38:26.009485 bosch-control-panel-cc880p-3.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20428 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-20 17:38:26.009485 bosch-control-panel-cc880p-3.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:26.001485 bosch-control-panel-cc880p-3.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:26.001485 bosch-control-panel-cc880p-3.1.4/src/bosch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:26.001485 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:26.005485 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:26.005485 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/cli/cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    18926 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/cp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:26.005485 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/models/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/models/cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/models/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/models/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:26.009485 bosch-control-panel-cc880p-3.1.4/src/bosch_control_panel_cc880p.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-20 17:38:25.000000 bosch-control-panel-cc880p-3.1.4/src/bosch_control_panel_cc880p.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-20 17:38:26.000000 bosch-control-panel-cc880p-3.1.4/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 17:38:25.000000 bosch-control-panel-cc880p-3.1.4/src/bosch_control_panel_cc880p.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-20 17:38:25.000000 bosch-control-panel-cc880p-3.1.4/src/bosch_control_panel_cc880p.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 17:38:25.000000 bosch-control-panel-cc880p-3.1.4/src/bosch_control_panel_cc880p.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 17:38:25.000000 bosch-control-panel-cc880p-3.1.4/src/bosch_control_panel_cc880p.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:20:10.105130 bosch-control-panel-cc880p-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-22 23:19:59.000000 bosch-control-panel-cc880p-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-22 23:20:10.105130 bosch-control-panel-cc880p-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20428 2023-05-22 23:19:59.000000 bosch-control-panel-cc880p-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-22 23:19:59.000000 bosch-control-panel-cc880p-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-22 23:20:10.109130 bosch-control-panel-cc880p-4.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:20:10.101129 bosch-control-panel-cc880p-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:20:10.101129 bosch-control-panel-cc880p-4.0.0/src/bosch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:20:10.101129 bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:20:10.105130 bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 23:19:59.000000 bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:20:10.105130 bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 23:19:59.000000 bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-22 23:19:59.000000 bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-22 23:19:59.000000 bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/cli/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-22 23:19:59.000000 bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22427 2023-05-22 23:19:59.000000 bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/cp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:20:10.105130 bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 23:19:59.000000 bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-22 23:19:59.000000 bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-22 23:19:59.000000 bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/models/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-22 23:19:59.000000 bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/models/cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-22 23:19:59.000000 bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-22 23:19:59.000000 bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/models/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-22 23:19:59.000000 bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/models/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-22 23:19:59.000000 bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/models/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-22 23:19:59.000000 bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 23:19:59.000000 bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:20:10.105130 bosch-control-panel-cc880p-4.0.0/src/bosch_control_panel_cc880p.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-22 23:20:10.000000 bosch-control-panel-cc880p-4.0.0/src/bosch_control_panel_cc880p.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-22 23:20:10.000000 bosch-control-panel-cc880p-4.0.0/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 23:20:10.000000 bosch-control-panel-cc880p-4.0.0/src/bosch_control_panel_cc880p.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-22 23:20:10.000000 bosch-control-panel-cc880p-4.0.0/src/bosch_control_panel_cc880p.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-22 23:20:10.000000 bosch-control-panel-cc880p-4.0.0/src/bosch_control_panel_cc880p.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 23:20:10.000000 bosch-control-panel-cc880p-4.0.0/src/bosch_control_panel_cc880p.egg-info/top_level.txt
```

### Comparing `bosch-control-panel-cc880p-3.1.4/LICENSE` & `bosch-control-panel-cc880p-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.4/PKG-INFO` & `bosch-control-panel-cc880p-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bosch-control-panel-cc880p
-Version: 3.1.4
+Version: 4.0.0
 Summary: Library to interface with the old CC880p Bosch COntrol Panels
 Home-page: https://github.com/hgomes88/bosch-control-panel-cc880p
 Author: Hugo Gomes
 Author-email: hgomes88@gmail.com
 Project-URL: Tracker, https://github.com/hgomes88/bosch-control-panel-cc880p/issues
 Project-URL: Download, https://pypi.org/project/bosch-control-panel-cc880p/
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 3.1.4 Summary:
+Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 4.0.0 Summary:
 Library to interface with the old CC880p Bosch COntrol Panels Home-page: https:
 //github.com/hgomes88/bosch-control-panel-cc880p Author: Hugo Gomes Author-
 email: hgomes88@gmail.com Project-URL: Tracker, https://github.com/hgomes88/
 bosch-control-panel-cc880p/issues Project-URL: Download, https://pypi.org/
 project/bosch-control-panel-cc880p/ Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
```

### Comparing `bosch-control-panel-cc880p-3.1.4/README.md` & `bosch-control-panel-cc880p-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.4/setup.cfg` & `bosch-control-panel-cc880p-4.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/cli/cli.py` & `bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/cli/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,102 +2,111 @@
 import asyncio
 import logging
 
 from bosch.control_panel.cc880p.cli.cmds import handle_command
 from bosch.control_panel.cc880p.cli.parser import Args
 from bosch.control_panel.cc880p.cli.parser import get_args
 from bosch.control_panel.cc880p.cp import CP
+from bosch.control_panel.cc880p.models.constants import Id
 from bosch.control_panel.cc880p.models.cp import Area
 from bosch.control_panel.cc880p.models.cp import Availability
-from bosch.control_panel.cc880p.models.cp import ControlPanelEntity
 from bosch.control_panel.cc880p.models.cp import CpVersion
-from bosch.control_panel.cc880p.models.cp import Id
 from bosch.control_panel.cc880p.models.cp import Output
 from bosch.control_panel.cc880p.models.cp import Siren
 from bosch.control_panel.cc880p.models.cp import Time
 from bosch.control_panel.cc880p.models.cp import Zone
+from bosch.control_panel.cc880p.models.errors import Error
+from bosch.control_panel.cc880p.models.listener import BaseControlPanelListener
 from bosch.control_panel.cc880p.utils import to_hex
 
-logging.basicConfig(level=logging.WARNING)
+logging.basicConfig(level=logging.DEBUG)
 
 prev_data = None
 
 
-async def data_listener(data: bytes) -> bool:
-    """Listen of any control panel change."""
-    global prev_data
-    if prev_data and prev_data[:-2] != data[:-2]:
-        print('\nDifference:')
-        print(f'\tBefore:\t{to_hex(prev_data)}')
-        print(f'\tAfter:\t{to_hex(data)}')
-    else:
-        print('\nNo Changes:')
-        print(to_hex(data))
-    prev_data = data
-    return True
-
-
-async def cp_listener(id: Id, cp: ControlPanelEntity) -> bool:
-    """Control panel listener."""
-    if isinstance(cp, Zone):
-        print(f'Zone {id} updated: {cp}')
-    elif isinstance(cp, Output):
-        print(f'Output {id} updated: {cp}')
-    elif isinstance(cp, Siren):
-        print(f'Siren updated: {cp}')
-    elif isinstance(cp, Area):
-        print(f'Area {id} updated: {cp}')
-    elif isinstance(cp, Availability):
-        print(f'Control Panel availability is: {cp}')
-    elif isinstance(cp, Time):
-        print(f'Control Panel time is: {cp}')
-
-    return True
-
-
-async def _wait_for_connection(cp: CP):
-    while not cp.connected:
-        await asyncio.sleep(1.0)
+class Listener(BaseControlPanelListener):
+    """Lister class implementing all events of interest."""
+
+    def __init__(self, cp: CP):
+        """Init."""
+        self._cp = cp
+
+    async def on_availability_changed(self, entity: Availability):
+        """On availability changed."""
+        print(f'Control Panel availability is: {entity}')
+
+    async def on_area_changed(self, entity: Area):
+        """On area changed."""
+        print(f'Area {id} updated: {entity}')
+
+    async def on_siren_changed(self, entity: Siren):
+        """On siren changed."""
+        print(f'Siren updated: {entity}')
+
+    async def on_zone_changed(self, id: Id, entity: Zone):
+        """On zone changed."""
+        print(f'Zone {id} updated: {entity}')
+
+    async def on_time_changed(self, entity: Time):
+        """On time changed."""
+        print('Time changed to:', entity)
+
+    async def on_output_changed(self, id: Id, entity: Output):
+        """On output changed."""
+        print(f'Output {id} updated: {entity}')
+
+    async def on_data(self, data: bytes):
+        """On data changed."""
+        global prev_data
+        if prev_data and prev_data[:-2] != data[:-2]:
+            print('\nDifference:')
+            print(f'\tBefore:\t{to_hex(prev_data)}')
+            print(f'\tAfter:\t{to_hex(data)}')
+        else:
+            print('\nNo Changes:')
+            print(to_hex(data))
+        prev_data = data
 
 
 async def run_listen_mode(cp: CP):
     """Run the control panel in listen mode."""
-    cp.add_data_listener(data_listener)
-    cp.add_control_panel_listener(cp_listener)
+    cp.add_listener(Listener(cp))
     while True:
-        try:
-            await asyncio.wait_for(_wait_for_connection(cp), timeout=3.0)
-            await cp.get_status()
-        except BaseException:
-            logging.exception('Error:')
-        finally:
-            await asyncio.sleep(1)
+        await asyncio.sleep(1)
 
 
 async def run_cmd_mode(cp: CP, args):
     """Run mode command."""
-    await handle_command(cp, args)
+    resp = await handle_command(cp, args)
+    print('Resp:', resp)
 
 
 async def run(loop):
     """Run the control panel command line."""
     args: Args = get_args()
 
     cp = CP(
         ip=args.connect,
         port=args.port,
         model=CpVersion.S16_V14.model(),
         installer_code=args.code,
+        poll_period=3,
         loop=loop,
     )
 
     await cp.start()
 
     if args.cmd:
-        await run_cmd_mode(cp, args)
+        try:
+            await run_cmd_mode(cp, args)
+        except Error as exc:
+            logging.error(f'Error: {repr(exc)}')
+        except BaseException:
+            logging.exception('Unknown error:')
+
     else:
         await run_listen_mode(cp)
 
     await cp.stop()
 
 
 def main():
```

### Comparing `bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/cli/cmds.py` & `bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/cli/cmds.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,67 +12,67 @@
 def cmd(cp: CP, obj: Any = None):
     """Fetch the control panel status after any change."""
     def inner(func):
         async def wrapper(*args, **kwargs):
             # await cp.get_status()
             if obj is not None:
                 print(f'Before: {obj}')
-            await func(*args, **kwargs)
+            return await func(*args, **kwargs)
             # await cp.get_status()
             if obj is not None:
                 print(f'After: {obj}')
         return wrapper
     return inner
 
 
 async def set_mode_arming(cp: CP, arm: bool):
     """Handle the arming mode command."""
-    await cmd(cp, cp.control_panel.areas[1])(cp.set_arming)(arm=arm)
+    return await cmd(cp, cp.control_panel.areas[1])(cp.set_arming)(arm=arm)
 
 
 async def handle_mode_command(cp: CP, mode: str):
     """Handle the mode command."""
     if mode == 'arm':
-        await set_mode_arming(cp, True)
+        return await set_mode_arming(cp, True)
     elif mode == 'disarm':
-        await set_mode_arming(cp, False)
+        return await set_mode_arming(cp, False)
 
 
 async def handle_siren_command(cp: CP, status: bool):
     """Handle the siren command."""
-    await cmd(cp, cp.control_panel.siren)(cp.set_siren)(on=status)
+    return await cmd(cp, cp.control_panel.siren)(cp.set_siren)(on=status)
 
 
 async def handle_out_command(cp: CP, out: int, status: bool):
     """Handle outputs command."""
-    await cmd(cp, cp.control_panel.outputs[out])(cp.set_output)(
+    return await cmd(cp, cp.control_panel.outputs[out])(cp.set_output)(
         id=out,
         on=status
     )
 
 
 async def handle_time_command(cp: CP, time: datetime):
     """Handle the set time command."""
-    await cmd(cp, cp.control_panel.time)(cp.set_time)(time=time)
+    return await cmd(cp, cp.control_panel.time)(cp.set_time)(time=time)
 
 
 async def handle_keys_command(cp: CP, keys: List[str]):
     """Handle the keys sending."""
     keys = [i for ele in keys for i in ele]
-    await cmd(cp)(cp.send_keys)(keys=keys)
-    await cmd(cp, cp.control_panel.areas)(cp.get_status)()
+    return await cmd(cp)(cp.send_keys)(keys=keys)
+    return await cmd(cp, cp.control_panel.areas)(cp.get_status)()
 
 
 async def handle_raw_command(cp: CP, raw: bytes):
     """Handle raw commands."""
     # Add the checksum calculated to the data
     _raw = raw + bytes([checksum(raw)])
     print(f'Sending: {_raw.hex()}')
     # Send the command and wait for the response
-    resp = await (cp.send_command)(message=_raw)
+    resp = await (cp.send_command)(request=_raw)
 
     # Split the response checksum from its data
     resp_checksum = resp[-1]
     resp_data = resp[0:-1]
     # Calculate the checksum
     calc_checksum = checksum(resp_data)
 
@@ -84,23 +84,24 @@
     else:
         print(
             f'[INVALID CHECKSUM] received: {hex(resp_checksum)} | calculated: '
             f'{hex(calc_checksum)}'
         )
 
     print(resp.hex())
+    return resp
 
 
 async def handle_command(cp: CP, args: Args):
     """Handle the control panel commands."""
     if args.cmd == Commands.SetMode:
-        await handle_mode_command(cp, args.mode)
+        return await handle_mode_command(cp, args.mode)
     if args.cmd == Commands.SetSiren:
-        await handle_siren_command(cp, args.status)
+        return await handle_siren_command(cp, args.status)
     if args.cmd == Commands.SetTime:
-        await handle_time_command(cp, args.time)
+        return await handle_time_command(cp, args.time)
     if args.cmd == Commands.SetOutput:
-        await handle_out_command(cp, args.out, args.status)
+        return await handle_out_command(cp, args.out, args.status)
     if args.cmd == Commands.SendKeys:
-        await handle_keys_command(cp, args.keys)
+        return await handle_keys_command(cp, args.keys)
     if args.cmd == Commands.SendRaw:
-        await handle_raw_command(cp, args.raw)
+        return await handle_raw_command(cp, args.raw)
```

### Comparing `bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/cli/parser.py` & `bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/cli/parser.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/cp.py` & `bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/cp.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,48 +5,52 @@
 import logging
 from asyncio import AbstractEventLoop
 from asyncio import Task
 from asyncio.exceptions import CancelledError
 from enum import Enum
 from typing import List
 from typing import Optional
-from typing import Type
 from typing import Union
 
-from bosch.control_panel.cc880p.models.callbacks import ControlPanelListener
-from bosch.control_panel.cc880p.models.callbacks import DataListener
+from bosch.control_panel.cc880p.models import errors
 from bosch.control_panel.cc880p.models.constants import Id
 from bosch.control_panel.cc880p.models.constants import MAX_KEYS
+from bosch.control_panel.cc880p.models.constants import MAX_POLL_PERIOD_S
 from bosch.control_panel.cc880p.models.cp import ArmingMode
 from bosch.control_panel.cc880p.models.cp import ControlPanel
 from bosch.control_panel.cc880p.models.cp import CpModel
+from bosch.control_panel.cc880p.models.listener import BaseControlPanelListener
+from bosch.control_panel.cc880p.models.listener import EventProducer
 from bosch.control_panel.cc880p.models.requests import KeysRequest
 from bosch.control_panel.cc880p.models.requests import Request
 from bosch.control_panel.cc880p.models.requests import SetArmingRequest
 from bosch.control_panel.cc880p.models.requests import SetOutRequest
 from bosch.control_panel.cc880p.models.requests import SetSirenRequest
 from bosch.control_panel.cc880p.models.requests import SetTimeRequest
 from bosch.control_panel.cc880p.models.requests import StatusRequest
 from bosch.control_panel.cc880p.models.responses import Response
 from bosch.control_panel.cc880p.models.responses import StatusResponse
-from bosch.control_panel.cc880p.utils import checksum
-from bosch.control_panel.cc880p.utils import to_hex
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class CP:
     """Alarm control panel object representation."""
 
+    ###########################################################################
+    # Init
+    ###########################################################################
+
     def __init__(
         self,
         ip: str,
         port: int,
         model: CpModel,
         installer_code: str = None,
+        poll_period: float = 1.0,
         loop: Optional[AbstractEventLoop] = None,
     ):
         """Initialize the Control Panel object to interface through TCP.
 
         Args:
             ip (str):
                 IP of the control panel
@@ -67,33 +71,37 @@
         self._installer_code = installer_code
 
         # IP of the control panel
         self._ip = ip
         # Port of the control panel
         self._port = port
 
+        self._init_poll_period = poll_period
+        self._poll_period = self._init_poll_period
+
         # Streamreader
         self._reader: Optional[asyncio.StreamReader] = None
         # Streamwriter
         self._writer: Optional[asyncio.StreamWriter] = None
         # Connected
         self._connected: bool = False
         # Reconnection task
         self._conn_task: Optional[Task] = None
 
         # Lock
         self._lock = asyncio.Lock()
 
-        # Listeners to be called whenever the control panel state is changed
-        self._control_panel_listeners: List[ControlPanelListener] = []
-        # Listeners to be called whenever the there's new data
-        self._data_listeners: List[DataListener] = []
+        self._listeners: List[BaseControlPanelListener] = []
 
         self._control_panel = ControlPanel.build(self._model)
 
+        self._evt = EventProducer(self._control_panel)
+
+        self._update_last_request()
+
     def __repr__(self):
         """Representation of control panel."""
         return str(self._control_panel)
 
     @property
     def __dict__(self):
         """Return a dict representation of control panel."""
@@ -116,427 +124,501 @@
         return self._control_panel
 
     @property
     def connected(self) -> bool:
         """Report whether the connection to the alarm is established."""
         return self._connected
 
+    async def _set_connected(self, connected=True):
+        if connected != self._connected:
+            self._connected = connected
+            self.control_panel.availability.available = self._connected
+            await self._evt.notify_availability_changed()
+
     async def start(self) -> 'CP':
         """Establish the connection to the control panel."""
-        await self._start_connection_task()
+        await self._connect()
         return self
 
     async def stop(self) -> 'CP':
         """Stop the connection to the control panel."""
-        await self._stop_connection_task()
+        await self._disconnect()
         return self
 
-    def add_control_panel_listener(self, listener: ControlPanelListener):
-        """Add a listener function to listen for any change in the alarm."""
-        self._control_panel_listeners.append(listener)
-
-    def add_data_listener(self, listener: DataListener):
-        """Add a listener function to listen for any incoming data."""
-        self._data_listeners.append(listener)
+    ###########################################################################
+    # Connection
+    ###########################################################################
+
+    async def _connect(self):
+        connected = False
+        _LOGGER.info('Connecting')
+        try:
+            # Start the connection
+            await self._open_connection()
+            # Ensure the connection is established by requesting for its status
+            await self._get_status()
+            # Set the connection state to connected
+            connected = True
+        except errors.Error as exc:
+            _LOGGER.error(f'Error: {repr(exc)}')
+        except BaseException:
+            _LOGGER.exception('Unknown error:')
+        else:
+            _LOGGER.info('Connected')
+        finally:
+            # Always update the connection state
+            await self._set_connected(connected)
+            # Always create the connection task if not created yet
+            await self._create_connection_task()
+
+    async def _open_connection(self):
+        """Open the stream connection to the alarm."""
+        async with self._lock:
+            try:
+                self._reader, self._writer = await asyncio.open_connection(
+                    self._ip,
+                    self._port
+                )
+            except ConnectionRefusedError as exc:
+                raise ConnectionError from exc
+            except OSError as exc:
+                if exc.errno == 113:
+                    raise errors.ConnectionError from exc
+                else:
+                    raise
+
+    async def _create_connection_task(self):
+        if not self._conn_task:
+            self._conn_task = asyncio.create_task(self._connection_task())
+
+    async def _disconnect(self):
+        # Cancel any connection related task
+        await self._cancel_connection_task()
+        # Ensure any previous connection is closed
+        await self._close_connection()
+        # Set the connection state to disconnected
+        await self._set_connected(False)
+
+    async def _cancel_connection_task(self):
+        if self._conn_task:
+            self._conn_task.cancel()
+            self._conn_task = None
+
+    async def _close_connection(self):
+        async with self._lock:
+            if self._reader:
+                if not self._reader.at_eof():
+                    self._reader.feed_eof()
+            if self._writer:
+                self._writer.close()
+                await self._writer.wait_closed()
+
+            self._reader = None
+            self._writer = None
+
+    async def _connection_task(self):
+        period = self._retry_period(init=True)
+        while True:
+            try:
+                if not self.connected:
+                    _LOGGER.info('Reconnecting')
+                    await self._close_connection()
+                    await self._connect()
+                    if self.connected:
+                        _LOGGER.info('Reconnected')
+                        period = self._retry_period(init=True)
+                    else:
+                        period = self._retry_period()
+                        _LOGGER.error(
+                            f'Reconnection failed. Retrying in {period} '
+                            'seconds.'
+                        )
+                else:
+                    # Ask for status to check if connection with the control
+                    # panel is still available
+                    now = datetime.datetime.now()
+                    if abs(
+                        now - self.last_request_time
+                    ).total_seconds() >= self._init_poll_period:
+                        _LOGGER.debug('Polling Status')
+                        await self.get_status()
+            except CancelledError:
+                raise
+            except errors.Error as exc:
+                _LOGGER.error(f'Error: {repr(exc)}')
+                self._retry_period()
+            except BaseException:
+                _LOGGER.exception('Unknown error:')
+                self._retry_period()
+
+            try:
+                await asyncio.sleep(period)
+            except CancelledError:
+                raise
+
+    def _retry_period(self, init=False):
+        if init:
+            self._poll_period = self._init_poll_period
+        else:
+            self._poll_period = self._poll_period * 2
+
+        if self._poll_period > MAX_POLL_PERIOD_S:
+            self._poll_period = MAX_POLL_PERIOD_S
+
+        return self._poll_period
+
+    ###########################################################################
+    # Listeners
+    ###########################################################################
+
+    def add_listener(self, listener: BaseControlPanelListener):
+        """Add a listener to listen for change events."""
+        self._evt.add_listener(listener)
+
+    def remove_listener(self, listener: BaseControlPanelListener):
+        """Remove a listener."""
+        self._evt.remove_listener(listener)
+
+    def clear_listeners(self):
+        """Remove all the listeners."""
+        self._evt.clear_listeners()
+
+    ###########################################################################
+    # Commands
+    ###########################################################################
+
+    def _command(func):
+        async def wrapper(self, *args, **kwargs):
+            if self.connected:
+                return await func(self, *args, **kwargs)
+            raise errors.ConnectionError('Not connected')
+        return wrapper
 
+    @_command  # type: ignore
+    async def get_status(self):
+        """Get the control panel status."""
+        return await self._get_status()
+
+    async def _get_status(self):
+        """Get the control panel status."""
+        status_request = StatusRequest(installer_code=self._installer_code)
+        status_response = await self._send_request(
+            status_request,
+            StatusResponse
+        )
+        await self._handle_status_msg(status_response)
+        return status_response
+
+    @_command  # type: ignore
     async def send_keys(
         self,
         keys: Union[str, List[str]],
     ):
         """Simulate a keypad, allowing sending multiple keys."""
         encoded_keys = self._encode_keys(keys)
 
         for i in range(0, len(encoded_keys), MAX_KEYS):
             # Get the next keys subset
             keys_subset = encoded_keys[i: i + MAX_KEYS]
             # Build the request
             request = KeysRequest(keys=keys_subset, zone=0)
             # Send the request
-            await self.send_request(request, StatusResponse)
+            status_response = await self._send_request(request, StatusResponse)
 
-    async def set_output(self, id: Id, on: bool):
+        await self._handle_status_msg(status_response)
+
+    def _encode_keys(self, keys: Union[str, List[str]]) -> bytes:
+        return bytes(self._encode_key(key) for key in list(keys))
+
+    def _encode_key(self, key: str) -> int:
+        # Is a number between 0 and 9
+        if key.isdigit() and int(key) in range(0, 10):
+            return int(key)
+        elif key == '*':
+            return 0x1B
+        elif key == '#':
+            return 0x1A
+        else:
+            msg = 'Unrecognized key %s', key
+            _LOGGER.error(msg)
+            raise errors.ValueError(msg)
+
+    @_command  # type: ignore
+    async def set_output(self, id: Id, on: bool) -> bool:
         """Set output."""
-        try:
-            if id not in self.control_panel.outputs:
-                raise ValueError(f"The output with {id} doesn't exist")
+        if id not in self.control_panel.outputs:
+            raise errors.ValueError(f"The output with {id} doesn't exist")
 
-            if self._control_panel.outputs[id].on != on:
-                request = SetOutRequest(id, on)
-                await self.send_request(request, StatusResponse)
-        except Exception as ex:
-            _LOGGER.error(f'Error setting the output: {ex}')
-            raise
+        if self._control_panel.outputs[id].on != on:
+            request = SetOutRequest(id, on)
+            status_response = await self._send_request(request, StatusResponse)
+            await self._handle_status_msg(status_response)
+
+        return self._control_panel.outputs[id].on
 
+    @_command  # type: ignore
     async def set_arming(
         self,
         id: Id = 1,
         arm: bool = False
-    ):
+    ) -> bool:
         """Set arming."""
+        request = None
+
         if arm and self._control_panel.areas[id].mode == ArmingMode.DISARMED:
             request = SetArmingRequest(id, arm)
-            await self.send_request(request, StatusResponse)
 
         elif not arm and \
                 self._control_panel.areas[id].mode != ArmingMode.DISARMED:
             request = SetArmingRequest(id, arm)
-            await self.send_request(request, StatusResponse)
 
+        if request:
+            status_response = await self._send_request(request, StatusResponse)
+            await self._handle_status_msg(status_response)
+
+        # Arming takes some time, so request again for the status
+        await self.get_status()
+
+        return self._control_panel.areas[id].mode != ArmingMode.DISARMED
+
+    @_command  # type: ignore
     async def set_siren(self, on: bool = False):
         """Set siren on or off.."""
+        request = None
         if on and self._control_panel.siren.on != on:
             # Switch on the siren
-            await self.send_request(SetSirenRequest(on), StatusResponse)
+            request = SetSirenRequest(on)
         elif not on and self._control_panel.siren.on != on:
             # Switch of the siren
-            await self.send_request(SetSirenRequest(on), StatusResponse)
+            request = SetSirenRequest(on)
 
-    async def set_time(self, time: datetime.datetime = None):
-        """Set time."""
-        # Set the time in the alarm
-        await self.send_request(SetTimeRequest(time), StatusResponse)
+        if request:
+            status_response = await self._send_request(request, StatusResponse)
+            await self._handle_status_msg(status_response)
 
-    async def get_status(self):
-        """Command to request the status of the alarm."""
-        request = StatusRequest(installer_code=self._installer_code)
-        await self.send_request(request, StatusResponse)
+        return self._control_panel.siren.on
 
-    async def send_request(
-            self,
-            request: Request,
-            resp_type: Optional[Type[Response]] = None
-    ):
-        """Send a new request."""
-        n_resp_bytes = resp_type.size if resp_type else 1
-        resp = await self.send_command(
-            message=request.encode(),
-            n_resp_bytes=n_resp_bytes,
-            timeout=3
+    @_command  # type: ignore
+    async def set_time(self, time: datetime.datetime = None) -> datetime.time:
+        """Set time."""
+        # Set the time in the alarm
+        status_response = await self._send_request(
+            SetTimeRequest(time),
+            StatusResponse
         )
-        if resp_type:
-            size_resp = len(resp) if resp else 0
-            if size_resp != resp_type.size:
-                raise ValueError(
-                    f'The size of the frame should be {resp_type.size}'
-                    f' but is {size_resp}'
-                )
-        self._handle_data(resp)
+        await self._handle_status_msg(status_response)
+        return self._control_panel.time.time
 
-    async def send_command(
-        self,
-        message: bytes,
-        n_resp_bytes=0,
-        timeout=3
-    ) -> Optional[bytes]:
-        """Send a command to the alarm and returns its response.
-
-        Args:
-            message (bytes):
-                Message to send to the control panel
+    ###########################################################################
+    # Write/Read
+    ###########################################################################
 
-        Returns:
-            bytes:
-                Response of the message sent to the control panel or None
-                otherwise
-        """
-        resp = None
-        available = False
+    async def _send_request(
+        self,
+        request: Request,
+        response: Optional[Response]
+    ) -> Union[Response, Optional[bytes]]:
+        """Send a new request."""
+        try:
+            resp = await self._send(
+                message=request.encode(),
+                resp_size=response.size if response else 0,
+                timeout=3
+            )
+            await self._evt.notify_data(resp)
+        except BaseException:
+            await self._set_connected(False)
+            raise
+        finally:
+            self._update_last_request()
 
-        if self.connected:
-            async with self._lock:
-                try:
-                    resp = await self._send(message, n_resp_bytes, timeout)
-                except asyncio.exceptions.TimeoutError:
-                    _LOGGER.warning('Message not received on time')
-                    raise
-                except asyncio.IncompleteReadError:
-                    _LOGGER.warning('Message not received.')
-                    raise
-                except EOFError:
-                    _LOGGER.warning('Connection EOF')
-                    raise
-                except (OSError):
-                    _LOGGER.warning('Connection failed')
-                    await self._close_connection()
-                    raise
-                except BaseException:
-                    _LOGGER.exception('Unexpected Error:')
-                    raise
-                else:
-                    available = True
-                    return resp
-                finally:
-                    await self._update_availability(available)
+        if response and self._valid_response(resp, response):
+            resp = response.decode(resp, self._model)
         else:
-            await self._update_availability(available)
-            raise ConnectionError('Not Connected')
-
-    async def _update_availability(self, available: bool = True):
-        if self.control_panel.availability.available != available:
-            self.control_panel.availability.available = available
-            for listener in self._control_panel_listeners:
-                asyncio.create_task(
-                    listener(0, self.control_panel.availability)
-                )
-
-    async def _connect(self):
-        async with self._lock:
-            _LOGGER.info('Connecting to control panel...')
-            try:
-                await self._close_connection()
-                await self._open_connection()
-            except asyncio.TimeoutError:
-                _LOGGER.error('Connection to control panel timed out')
-                raise
-            except (OSError):
-                _LOGGER.error('Connection to control panel failed')
-                raise
-            except BaseException:
-                _LOGGER.error(
-                    'Connection to control panel failed with unknown error')
-                raise
-
-    async def _close_connection(self):
-        """Close the stream connection to the alarm."""
-        if self._reader:
-            if not self._reader.at_eof():
-                self._reader.feed_eof()
-        if self._writer:
-            self._writer.close()
-            await self._writer.wait_closed()
-
-        self._reader = None
-        self._writer = None
+            raise errors.MessageError(
+                'Invalid response. Expected to be a frame of type '
+                f'{type(response)} but the message is {resp!r}'
+            )
+        return resp
 
-        self._connected = False
+    def _valid_response(
+            self,
+            raw_resp: Optional[bytes],
+            response: Response) -> bool:
+        valid = False
+
+        if raw_resp and len(raw_resp) == response.size:
+            if bytes([raw_resp[0]]) == bytes.fromhex(response.code):
+                valid = True
 
-    async def _open_connection(self):
-        """Open the stream connection to the alarm."""
-        self._reader, self._writer = await asyncio.open_connection(
-            self._ip,
-            self._port
-        )
-        self._connected = True
+        return valid
 
     async def _send(
         self,
         message: bytes,
-        n_resp_bytes: int = 0,
+        resp_size: int = 0,
         timeout=3
-    ) -> bytes:
+    ) -> Optional[bytes]:
         """Send a binary stream to the control panel and waits for its response.
 
         Args:
             message (bytes): Message to send to the control panel
 
         Returns:
             bytes: Response of the message sent to the control panel
         """
-        if self.connected and self._writer and self._reader:
+        if not self._writer:
+            raise errors.ConnectionError('Writer is not open')
+        elif not self._reader:
+            raise errors.ConnectionError('Reader is not open')
+
+        async with self._lock:
             # Ensure a clean buffer
             self._reader._buffer.clear()  # type: ignore
-
             # Send the command
-            self._writer.write(message)
-            await self._writer.drain()
-
+            await self._write(message)
             # Wait for a response
-            if not self._reader.at_eof():
-                if n_resp_bytes:
-                    data = await asyncio.wait_for(
-                        self._reader.readexactly(n_resp_bytes),
-                        timeout=timeout
-                    )
-                else:
-                    data = await asyncio.wait_for(
-                        self._reader.read(32), timeout=timeout
-                    )
-                if not data:
-                    raise asyncio.IncompleteReadError(data, 32)
-                return data
-            else:
-                raise EOFError()
-        else:
-            raise ConnectionError('Not Connected')
-
-    def _encode_key(self, key: str) -> int:
-        # Is a number between 0 and 9
-        if key.isdigit() and int(key) in range(0, 10):
-            return int(key)
-        elif key == '*':
-            return 0x1B
-        elif key == '#':
-            return 0x1A
-        else:
-            _LOGGER.error('Unrecognized key %s', key)
-            raise ValueError('Unrecognized key %s', key)
-
-    def _encode_keys(self, keys: Union[str, List[str]]) -> bytes:
-        return bytes(self._encode_key(key) for key in list(keys))
-
-    def _validate_data(self, data: Optional[bytes]):
-        if data:
-            cs = checksum(data[0:-1])
-            if cs != data[-1]:
-                raise ValueError(
-                    f'Data with invalid checksum. Received: {hex(data[-1])}, '
-                    f'Calculated: {hex(cs)} ({data.hex()})'
-                )
-        else:
-            raise RuntimeError('Checksum cannot be calculated without data')
-
-    def _handle_data(self, data: Optional[bytes]):
-        if data:
-
-            self._validate_data(data)
+            return await self._read(resp_size, timeout)
 
-            _LOGGER.debug('New Data: %s', to_hex(data))
-
-            if self._is_status_msg(data):
-                self._handle_status_msg(data)
+    async def _write(self, message: bytes):
+        if self._writer:
+            try:
+                self._writer.write(message)
+                await self._writer.drain()
+                return
+            except ConnectionRefusedError as exc:
+                raise errors.ConnectionError from exc
+            except OSError as exc:
+                if exc.errno == 113:
+                    raise errors.ConnectionError from exc
+                else:
+                    raise
 
-            for listener in self._data_listeners:
-                asyncio.create_task(listener(data))
-        else:
-            _LOGGER.warning('No Data Received!!!')
+        raise errors.ConnectionError('Writer is not open')
 
-    @classmethod
-    def _is_status_msg(cls, data: bytes):
+    async def _read(
+        self,
+        read_size: int = 0,
+        timeout: float = 3
+    ) -> Optional[bytes]:
 
-        if bytes([data[0]]) != bytes.fromhex(StatusResponse.code):
-            return False
+        data: Optional[bytes] = None
 
-        if len(data) != StatusResponse.size:
-            raise ValueError(
-                f'The size of the frame should be {StatusResponse.size}'
-                f' but is {len(data)}'
-            )
+        if self._reader:
+            if not self._reader.at_eof():
+                try:
+                    if read_size:
+                        data = await asyncio.wait_for(
+                            self._reader.readexactly(read_size),
+                            timeout=timeout
+                        )
+                    else:
+                        data = await asyncio.wait_for(
+                            self._reader.read(32), timeout=timeout
+                        )
+                    return data
+                except asyncio.exceptions.TimeoutError as exc:
+                    raise errors.TimeoutError from exc
+                except asyncio.exceptions.IncompleteReadError as exc:
+                    raise errors.MessageError from exc
+                except ConnectionRefusedError as exc:
+                    raise errors.ConnectionError from exc
+                except OSError as exc:
+                    if exc.errno == 113:
+                        raise errors.ConnectionError from exc
+                    else:
+                        raise
+            else:
+                raise errors.MessageError('EOF')
 
-        return True
+        raise errors.ConnectionError('Reader is not open')
 
-    def _handle_status_msg(self, data: bytes):
-        resp = StatusResponse.decode(data, self._model)
+    def _update_last_request(self):
+        self._last_request = datetime.datetime.now()
 
-        self._update_siren_status(resp.siren)
-        self._update_output_status(resp.outs)
-        self._update_area_status(resp.areas)
-        self._update_zone_status(resp.zones)
-        self.update_zone_enabled(resp.zones_en)
-        self._update_time(resp.time)
+    @property
+    def last_request_time(self) -> datetime.datetime:
+        """Get the last request time."""
+        return self._last_request
+
+    ###########################################################################
+    # Response Handlers
+    ###########################################################################
+
+    async def _handle_status_msg(self, status: StatusResponse):
+        await self._update_siren_status(status.siren)
+        await self._update_output_status(status.outs)
+        await self._update_area_status(status.areas)
+        await self._update_zone_status(status.zones)
+        await self.update_zone_enabled(status.zones_en)
+        await self._update_time(status.time)
 
-    def _update_zone_status(self, zones: List[bool]):
+    async def _update_zone_status(self, zones: List[bool]):
         for i in range(self._model.n_zones):
             zone_number: Id = i + 1
             zone = self._control_panel.zones[zone_number]
-
             if zone.triggered != zones[i]:
                 zone.triggered = zones[i]
-
-                for listener in self._control_panel_listeners:
-                    asyncio.create_task(listener(zone_number, zone))
-
+                await self._evt.notify_zone_trigger_changed(zone_number)
                 _LOGGER.info(
                     'Status of Zone %d changed to %d',
                     zone_number,
                     zone.triggered
                 )
 
-    def update_zone_enabled(self, zones_en: List[bool]):
+    async def update_zone_enabled(self, zones_en: List[bool]):
         """Update zone enabled."""
         for i in range(self._model.n_zones):
             zone_number = i + 1
             zone = self._control_panel.zones[zone_number]
-
             if zone.enabled != zones_en[i]:
                 zone.enabled = zones_en[i]
-
-                for listener in self._control_panel_listeners:
-                    asyncio.create_task(listener(zone_number, zone))
-
+                await self._evt.notify_zone_enabling_changed(zone_number)
                 _LOGGER.info(
                     'Zone enabling of Zone %d changed to %d',
                     zone_number,
                     zone.enabled
                 )
 
-    def _update_siren_status(self, status: bool):
+    async def _update_siren_status(self, status: bool):
         if self._control_panel.siren.on != status:
             self._control_panel.siren.on = status
-
-            for listener in self._control_panel_listeners:
-                asyncio.create_task(listener(0, self._control_panel.siren))
-
+            await self._evt.notify_siren_changed()
             _LOGGER.info('Siren changed to %d', self._control_panel.siren.on)
 
-    def _update_output_status(self, outs: List[bool]):
+    async def _update_output_status(self, outs: List[bool]):
         for i in range(self._model.n_outputs):
             out_number: Id = i + 1
             out = self._control_panel.outputs[out_number]
-
             if out.on != outs[i]:
                 out.on = outs[i]
-
-                for listener in self._control_panel_listeners:
-                    asyncio.create_task(listener(out_number, out))
-
+                await self._evt.notify_output_changed(out_number)
                 _LOGGER.info('The output %d changed to %d', out_number, out.on)
 
-    def _update_area_status(self, areas: List[ArmingMode]):
-
+    async def _update_area_status(self, areas: List[ArmingMode]):
         for i in range(self._model.n_areas):
             area_number: Id = i + 1
             area = self._control_panel.areas[area_number]
             status_changed = False
-
             if areas[i] is ArmingMode.DISARMED:
                 if area.mode is not ArmingMode.DISARMED:
                     area.mode = ArmingMode.DISARMED
                     status_changed = True
             elif areas[i] is ArmingMode.ARMED_AWAY:
                 if area.mode is not ArmingMode.ARMED_AWAY:
                     status_changed = True
                     area.mode = ArmingMode.ARMED_AWAY
             elif areas[i] is not ArmingMode.ARMED_STAY:
                 if area.mode is not ArmingMode.ARMED_STAY:
                     status_changed = True
                     area.mode = ArmingMode.ARMED_STAY
-
             if status_changed:
-                for listener in self._control_panel_listeners:
-                    asyncio.create_task(listener(area_number, area))
-
+                await self._evt.notify_area_changed()
                 _LOGGER.info(
                     'Status of Area %d changed to %s', area_number, area.mode
                 )
 
-    def _update_time(self, time: datetime.time):
-
+    async def _update_time(self, time: datetime.time):
         if self._control_panel.time.time != time:
             self._control_panel.time.time = time
-
-            for listener in self._control_panel_listeners:
-                asyncio.create_task(listener(0, self._control_panel.time))
-
+            await self._evt.notify_time_changed()
             _LOGGER.info('Time updated %s', self._control_panel.time)
-
-    async def _start_connection_task(self):
-        self._conn_task = asyncio.create_task(self._connection_task())
-
-    async def _stop_connection_task(self):
-        if self._conn_task:
-            self._conn_task.cancel()
-            self._conn_task = None
-        async with self._lock:
-            await self._close_connection()
-
-    async def _connection_task(self):
-        while True:
-            try:
-                if not self.connected:
-                    _LOGGER.info('Connecting')
-                    await self._connect()
-            except CancelledError:
-                break
-            except BaseException:
-                _LOGGER.error('Connection failed')
-            finally:
-                await asyncio.sleep(3)
```

### Comparing `bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/models/cp.py` & `bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/models/cp.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/models/requests.py` & `bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/models/requests.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/models/responses.py` & `bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/models/responses.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,31 +19,36 @@
 @dataclass
 class Response:
     """Response base object."""
 
     code: str
     size: int
 
+    @classmethod
+    def decode(cls, data: bytes, cp: CpModel):
+        """Abstract method to decode a response."""
+        raise NotImplementedError
+
 
 @dataclass
-class StatusResponse:
+class StatusResponse(Response):
     """Status response object."""
 
     code: str = field(init=False, default=ResponsesProps.StatusCode.value)
     size: int = field(init=False, default=ResponsesProps.StatusSize.value)
     time: datetime.time
     siren: bool
     outs: List[bool]
     areas: List[ArmingMode]
     zones: List[bool]
     zones_en: List[bool]
 
     @classmethod
     def decode(cls, data: bytes, cp: CpModel):
-        """Decode a status response."""
+        """Implement of decode method."""
         time = cls._decode_time(data)
         siren = cls._decode_siren_status(data)
         outs = cls._decode_outputs(data, cp.n_outputs)
         areas = cls._decode_areas(data, cp.n_areas)
         zones = cls._decode_zones(data, cp.n_zones)
         zones_en = cls._decode_zones_en(data, cp.n_zones, areas[0])
```

### Comparing `bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/utils.py` & `bosch-control-panel-cc880p-4.0.0/src/bosch/control_panel/cc880p/utils.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.4/src/bosch_control_panel_cc880p.egg-info/PKG-INFO` & `bosch-control-panel-cc880p-4.0.0/src/bosch_control_panel_cc880p.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bosch-control-panel-cc880p
-Version: 3.1.4
+Version: 4.0.0
 Summary: Library to interface with the old CC880p Bosch COntrol Panels
 Home-page: https://github.com/hgomes88/bosch-control-panel-cc880p
 Author: Hugo Gomes
 Author-email: hgomes88@gmail.com
 Project-URL: Tracker, https://github.com/hgomes88/bosch-control-panel-cc880p/issues
 Project-URL: Download, https://pypi.org/project/bosch-control-panel-cc880p/
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 3.1.4 Summary:
+Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 4.0.0 Summary:
 Library to interface with the old CC880p Bosch COntrol Panels Home-page: https:
 //github.com/hgomes88/bosch-control-panel-cc880p Author: Hugo Gomes Author-
 email: hgomes88@gmail.com Project-URL: Tracker, https://github.com/hgomes88/
 bosch-control-panel-cc880p/issues Project-URL: Download, https://pypi.org/
 project/bosch-control-panel-cc880p/ Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
```

### Comparing `bosch-control-panel-cc880p-3.1.4/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt` & `bosch-control-panel-cc880p-4.0.0/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 src/bosch/control_panel/cc880p/cli/cli.py
 src/bosch/control_panel/cc880p/cli/cmds.py
 src/bosch/control_panel/cc880p/cli/parser.py
 src/bosch/control_panel/cc880p/models/__init__.py
 src/bosch/control_panel/cc880p/models/callbacks.py
 src/bosch/control_panel/cc880p/models/constants.py
 src/bosch/control_panel/cc880p/models/cp.py
+src/bosch/control_panel/cc880p/models/errors.py
+src/bosch/control_panel/cc880p/models/listener.py
 src/bosch/control_panel/cc880p/models/requests.py
 src/bosch/control_panel/cc880p/models/responses.py
 src/bosch_control_panel_cc880p.egg-info/PKG-INFO
 src/bosch_control_panel_cc880p.egg-info/SOURCES.txt
 src/bosch_control_panel_cc880p.egg-info/dependency_links.txt
 src/bosch_control_panel_cc880p.egg-info/entry_points.txt
 src/bosch_control_panel_cc880p.egg-info/requires.txt
```

