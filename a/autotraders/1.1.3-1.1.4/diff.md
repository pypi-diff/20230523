# Comparing `tmp/autotraders-1.1.3.tar.gz` & `tmp/autotraders-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.1.3.tar", last modified: Tue May 23 04:40:53 2023, max compression
+gzip compressed data, was "autotraders-1.1.4.tar", last modified: Tue May 23 21:25:04 2023, max compression
```

## Comparing `autotraders-1.1.3.tar` & `autotraders-1.1.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:53.204525 autotraders-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-23 04:40:40.000000 autotraders-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-23 04:40:53.204525 autotraders-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-23 04:40:40.000000 autotraders-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:53.200525 autotraders-1.1.3/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-23 04:40:40.000000 autotraders-1.1.3/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-23 04:40:40.000000 autotraders-1.1.3/autotraders/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:53.200525 autotraders-1.1.3/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-23 04:40:40.000000 autotraders-1.1.3/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-23 04:40:40.000000 autotraders-1.1.3/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:53.200525 autotraders-1.1.3/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:40.000000 autotraders-1.1.3/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-23 04:40:40.000000 autotraders-1.1.3/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-23 04:40:40.000000 autotraders-1.1.3/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:53.200525 autotraders-1.1.3/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-23 04:40:40.000000 autotraders-1.1.3/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-23 04:40:40.000000 autotraders-1.1.3/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-23 04:40:40.000000 autotraders-1.1.3/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-23 04:40:40.000000 autotraders-1.1.3/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-23 04:40:40.000000 autotraders-1.1.3/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:53.200525 autotraders-1.1.3/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-23 04:40:40.000000 autotraders-1.1.3/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-23 04:40:40.000000 autotraders-1.1.3/autotraders/shared_models/trait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:53.204525 autotraders-1.1.3/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)     9225 2023-05-23 04:40:40.000000 autotraders-1.1.3/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-23 04:40:40.000000 autotraders-1.1.3/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-23 04:40:40.000000 autotraders-1.1.3/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-23 04:40:40.000000 autotraders-1.1.3/autotraders/space_traders_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-23 04:40:40.000000 autotraders-1.1.3/autotraders/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 04:40:40.000000 autotraders-1.1.3/autotraders/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-23 04:40:40.000000 autotraders-1.1.3/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:53.200525 autotraders-1.1.3/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-23 04:40:53.000000 autotraders-1.1.3/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-23 04:40:53.000000 autotraders-1.1.3/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 04:40:53.000000 autotraders-1.1.3/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 04:40:53.000000 autotraders-1.1.3/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-23 04:40:40.000000 autotraders-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 04:40:53.204525 autotraders-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:53.204525 autotraders-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:40.000000 autotraders-1.1.3/tests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-23 04:40:40.000000 autotraders-1.1.3/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-23 04:40:40.000000 autotraders-1.1.3/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:25:04.915694 autotraders-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-23 21:24:49.000000 autotraders-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-23 21:25:04.915694 autotraders-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-23 21:24:49.000000 autotraders-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:25:04.911694 autotraders-1.1.4/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-23 21:24:49.000000 autotraders-1.1.4/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-23 21:24:49.000000 autotraders-1.1.4/autotraders/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:25:04.911694 autotraders-1.1.4/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-23 21:24:49.000000 autotraders-1.1.4/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-23 21:24:49.000000 autotraders-1.1.4/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:25:04.911694 autotraders-1.1.4/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:24:49.000000 autotraders-1.1.4/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-23 21:24:49.000000 autotraders-1.1.4/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-23 21:24:49.000000 autotraders-1.1.4/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:25:04.915694 autotraders-1.1.4/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-23 21:24:49.000000 autotraders-1.1.4/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-23 21:24:49.000000 autotraders-1.1.4/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-23 21:24:49.000000 autotraders-1.1.4/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-23 21:24:49.000000 autotraders-1.1.4/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-23 21:24:49.000000 autotraders-1.1.4/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:25:04.915694 autotraders-1.1.4/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-23 21:24:49.000000 autotraders-1.1.4/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-23 21:24:49.000000 autotraders-1.1.4/autotraders/shared_models/trait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:25:04.915694 autotraders-1.1.4/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-05-23 21:24:49.000000 autotraders-1.1.4/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-23 21:24:49.000000 autotraders-1.1.4/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-23 21:24:49.000000 autotraders-1.1.4/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-23 21:24:49.000000 autotraders-1.1.4/autotraders/space_traders_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-23 21:24:49.000000 autotraders-1.1.4/autotraders/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 21:24:49.000000 autotraders-1.1.4/autotraders/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-23 21:24:49.000000 autotraders-1.1.4/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:25:04.911694 autotraders-1.1.4/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-23 21:25:04.000000 autotraders-1.1.4/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-23 21:25:04.000000 autotraders-1.1.4/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:25:04.000000 autotraders-1.1.4/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 21:25:04.000000 autotraders-1.1.4/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-23 21:24:49.000000 autotraders-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 21:25:04.915694 autotraders-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:25:04.915694 autotraders-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:24:49.000000 autotraders-1.1.4/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-23 21:24:49.000000 autotraders-1.1.4/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-23 21:24:49.000000 autotraders-1.1.4/tests/test_util.py
```

### Comparing `autotraders-1.1.3/LICENSE` & `autotraders-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.3/PKG-INFO` & `autotraders-1.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.1.3
+Version: 1.1.4
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.1.3/README.md` & `autotraders-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.3/autotraders/agent.py` & `autotraders-1.1.4/autotraders/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import math
-
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.faction.contract import get_all_contracts
 from autotraders.session import AutoTradersSession
 from autotraders.ship import get_all_ships
 
 
 class Agent(SpaceTradersEntity):
```

### Comparing `autotraders-1.1.3/autotraders/faction/__init__.py` & `autotraders-1.1.4/autotraders/faction/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.3/autotraders/faction/contract.py` & `autotraders-1.1.4/autotraders/faction/contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import math
-
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.util import parse_time
 
 
 class Deliver:
@@ -21,15 +19,17 @@
         self.fulfilled = None
         self.deadline = None
         self.accept_deadline = None
         self.contract_type = None
         self.on_fulfilled = None
         self.on_accepted = None
         self.contract_id = contract_id
-        super().__init__(session, update, session.base_url + "my/contracts/" + self.contract_id)
+        super().__init__(
+            session, update, session.base_url + "my/contracts/" + self.contract_id
+        )
 
     def update(self, data=None):
         if data is None:
             data = self.get()["data"]
         self.on_accepted = data["terms"]["payment"]["onAccepted"]
         self.on_fulfilled = data["terms"]["payment"]["onFulfilled"]
         self.accepted = data["accepted"]
@@ -41,17 +41,18 @@
             self.contract_data = [Deliver(d) for d in data["terms"]["deliver"]]
 
     def accept(self):
         j = self.post("accept")
         self.update(j["data"]["contract"])
 
     def deliver(self, symbol, cargo_symbol, amount):
-        j = self.post("deliver",
-                      data={"shipSymbol": symbol, "tradeSymbol": cargo_symbol, "units": amount},
-                      )
+        j = self.post(
+            "deliver",
+            data={"shipSymbol": symbol, "tradeSymbol": cargo_symbol, "units": amount},
+        )
         self.update(j["data"]["contract"])
 
     def negotiate(self, ship_symbol, session):
         j = session.post(
             self.session.base_url + "my/ships/" + ship_symbol + "/negotiate/contract"
         ).json()
         if "error" in j:
```

### Comparing `autotraders-1.1.3/autotraders/map/system.py` & `autotraders-1.1.4/autotraders/map/system.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import math
-
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.session import AutoTradersSession
 from autotraders.map.waypoint import Waypoint
 from autotraders.shared_models.map_symbol import MapSymbol
 
 
 class System(SpaceTradersEntity):
@@ -38,10 +36,13 @@
         systems = []
         for system in j:
             s = System(system["symbol"], session, False)
             s.update(system)
             systems.append(s)
         return systems, r.json()["meta"]["total"]
 
+    def __eq__(self, other):
+        return self.symbol == other.symbol
+
 
 def list_systems(session, page=1) -> (list[System], int):
     System.all(session, page)
```

### Comparing `autotraders-1.1.3/autotraders/map/waypoint.py` & `autotraders-1.1.4/autotraders/map/waypoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import math
-
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.trait import Trait
 
 from autotraders.shared_models.map_symbol import MapSymbol
 
 
 class Waypoint:
@@ -56,10 +54,13 @@
         waypoints = []
         for w in data:
             waypoint = Waypoint(w["symbol"], session, False)
             waypoint.update(w)
             waypoints.append(waypoint)
         return waypoints
 
+    def __eq__(self, other):
+        return self.symbol == other.symbol
+
 
 def get_all_waypoints(system, session):
     return Waypoint.all(system, session)
```

### Comparing `autotraders-1.1.3/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.1.4/autotraders/map/waypoint_types/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.3/autotraders/map/waypoint_types/jumpgate.py` & `autotraders-1.1.4/autotraders/map/waypoint_types/jumpgate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import math
-
 from autotraders.map.waypoint_types import WaypointType
 from autotraders.session import AutoTradersSession
 
 
 class JumpGate(WaypointType):
     def __init__(self, waypoint: str, session: AutoTradersSession, update=True):
         self.faction_symbol = ""
```

### Comparing `autotraders-1.1.3/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.1.4/autotraders/map/waypoint_types/marketplace.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.3/autotraders/map/waypoint_types/shipyard.py` & `autotraders-1.1.4/autotraders/map/waypoint_types/shipyard.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.3/autotraders/session.py` & `autotraders-1.1.4/autotraders/session.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.3/autotraders/ship/__init__.py` & `autotraders-1.1.4/autotraders/ship/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,17 +30,17 @@
             self.current += symbol["units"]
 
 
 class Route:
     def __init__(self, data):
         self.destination = MapSymbol(data["destination"]["symbol"])
         self.departure = MapSymbol(data["departure"]["symbol"])
-        self.moving = self.destination == self.departure
+        self.moving = self.destination != self.departure
         if self.moving:
-            self.depature_time = parse_time(data["departure_time"])
+            self.departure_time = parse_time(data["departureTime"])
             self.arrival = parse_time(data["arrival"])
 
 
 class Nav:
     def __init__(self, data):
         self.status = data["status"]
         self.location = MapSymbol(data["waypointSymbol"])
@@ -72,25 +72,29 @@
         super().__init__(
             session, update, session.base_url + "my/ships/" + self.symbol + "/"
         )
 
     def update(self, data: dict = None, hard=False):
         if data is None:
             data = self.get()["data"]
-        if self.crew is None and not hard:
+
+        def go_for_update(d, s):
+            return s in data and (d is None or hard)
+
+        if go_for_update(self.crew, "crew"):
             self.crew = Crew(data["crew"])
-        if self.frame is None and not hard:
+        if go_for_update(self.frame, "frame"):
             self.frame = Frame(data["frame"])
-        if self.reactor is None and not hard:
+        if go_for_update(self.reactor, "reactor"):
             self.reactor = Reactor(data["reactor"])
-        if self.engine is None and not hard:
+        if go_for_update(self.engine, "engine"):
             self.engine = Engine(data["engine"])
-        if self.modules is None and not hard:
+        if go_for_update(self.modules, "modules"):
             self.modules = [Module(d) for d in data["modules"]]
-        if self.mounts is None and not hard:
+        if go_for_update(self.mounts, "mounts"):
             self.mounts = [Mount(d) for d in data["mounts"]]
         if "nav" in data:
             self.nav = Nav(data["nav"])
         if "fuel" in data:
             self.fuel = Fuel(data["fuel"]["current"], data["fuel"]["capacity"])
         if "cargo" in data:
             self.cargo = Cargo(data["cargo"])
@@ -115,15 +119,15 @@
         """
         j = self.post("navigate", data={"waypointSymbol": waypoint})
         self.update(j["data"])
 
     def patch_navigation(self, new_flight_mode):
         r = self.session.patch(
             self.session.base_url + "my/ships/" + self.symbol + "/nav",
-            data={"flightMode": new_flight_mode}
+            data={"flightMode": new_flight_mode},
         )
         j = r.json()
         if "error" in j:
             raise IOError(j["error"]["message"])
         self.update({"nav": j["data"]})
 
     def dock(self):
```

### Comparing `autotraders-1.1.3/autotraders/ship/ship_components.py` & `autotraders-1.1.4/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.3/autotraders/space_traders_entity.py` & `autotraders-1.1.4/autotraders/space_traders_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         if self.action_url[-1] != "/":
             self.action_url += "/"
         if update:
             self.update()
 
     def get(self, action: str = None) -> dict:
         if action is None:
-            r = self.session.get(self.action_url[0: len(self.action_url) - 1])
+            r = self.session.get(self.action_url[0 : len(self.action_url) - 1]) # noqa E203
         else:
             r = self.session.get(
                 self.action_url + action,
             )
         j = r.json()
         if "error" in j:
             raise IOError(j["error"]["message"])
```

### Comparing `autotraders-1.1.3/autotraders/status.py` & `autotraders-1.1.4/autotraders/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,12 +54,14 @@
     s.reset_date = j["resetDate"]
     s.description = j["description"]
     s.stats = j["stats"]
     s.next_reset = j["serverResets"]["nextReset"]
     s.reset_frequency = j["serverResets"]["frequency"]
     s.announcements = []
     for announcement in j["announcements"]:
-        s.announcements.append(Announcement(title=announcement["title"], body=announcement["body"]))
+        s.announcements.append(
+            Announcement(title=announcement["title"], body=announcement["body"])
+        )
     s.links = []
     for link in j["links"]:
         s.links.append(Link(name=link["name"], url=link["url"]))
     return s
```

### Comparing `autotraders-1.1.3/autotraders.egg-info/PKG-INFO` & `autotraders-1.1.4/autotraders.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.1.3
+Version: 1.1.4
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.1.3/autotraders.egg-info/SOURCES.txt` & `autotraders-1.1.4/autotraders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.3/pyproject.toml` & `autotraders-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `autotraders-1.1.3/tests/test_init.py` & `autotraders-1.1.4/tests/test_init.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
 
 from autotraders.agent import Agent
 from autotraders.session import get_session
+from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.ship import Ship
 from autotraders.faction.contract import Contract
 
 
 @pytest.fixture
 def session():
     s = get_session("BLANK")
@@ -30,11 +31,19 @@
 
 def test_ship(session):
     s = Ship("TEST", session)
     s.dock()
     s.orbit()
     s.refuel()
 
+
 def test_contact(session):
     c = Contract("blah", session)
     c.accept()
     c.fulfill()
+
+def test_map_symbol():
+    s = MapSymbol("X1-TEST")
+    s1 = MapSymbol("X1-TEST2")
+    s2 = MapSymbol("X1-TEST")
+    assert s != s1
+    assert s == s2
```

