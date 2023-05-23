# Comparing `tmp/autotraders-1.1.1.tar.gz` & `tmp/autotraders-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.1.1.tar", last modified: Mon May 22 18:59:49 2023, max compression
+gzip compressed data, was "autotraders-1.1.2.tar", last modified: Mon May 22 19:50:41 2023, max compression
```

## Comparing `autotraders-1.1.1.tar` & `autotraders-1.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:49.153979 autotraders-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-22 18:59:35.000000 autotraders-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-22 18:59:49.153979 autotraders-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-22 18:59:35.000000 autotraders-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:49.149979 autotraders-1.1.1/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:49.149979 autotraders-1.1.1/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:49.149979 autotraders-1.1.1/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:49.149979 autotraders-1.1.1/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:49.149979 autotraders-1.1.1/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/shared_models/trait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:49.149979 autotraders-1.1.1/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:49.149979 autotraders-1.1.1/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-22 18:59:49.000000 autotraders-1.1.1/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-22 18:59:49.000000 autotraders-1.1.1/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 18:59:49.000000 autotraders-1.1.1/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 18:59:49.000000 autotraders-1.1.1/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-22 18:59:35.000000 autotraders-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 18:59:49.153979 autotraders-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:49.153979 autotraders-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:35.000000 autotraders-1.1.1/tests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-22 18:59:35.000000 autotraders-1.1.1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-22 18:59:35.000000 autotraders-1.1.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:50:41.440876 autotraders-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-22 19:50:26.000000 autotraders-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-22 19:50:41.440876 autotraders-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-22 19:50:26.000000 autotraders-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:50:41.436876 autotraders-1.1.2/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-22 19:50:26.000000 autotraders-1.1.2/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-22 19:50:26.000000 autotraders-1.1.2/autotraders/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:50:41.436876 autotraders-1.1.2/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-22 19:50:26.000000 autotraders-1.1.2/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-22 19:50:26.000000 autotraders-1.1.2/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:50:41.436876 autotraders-1.1.2/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:50:26.000000 autotraders-1.1.2/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-22 19:50:26.000000 autotraders-1.1.2/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-22 19:50:26.000000 autotraders-1.1.2/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:50:41.436876 autotraders-1.1.2/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-22 19:50:26.000000 autotraders-1.1.2/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-22 19:50:26.000000 autotraders-1.1.2/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-22 19:50:26.000000 autotraders-1.1.2/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-22 19:50:26.000000 autotraders-1.1.2/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-22 19:50:26.000000 autotraders-1.1.2/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:50:41.436876 autotraders-1.1.2/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-22 19:50:26.000000 autotraders-1.1.2/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-22 19:50:26.000000 autotraders-1.1.2/autotraders/shared_models/trait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:50:41.436876 autotraders-1.1.2/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-05-22 19:50:26.000000 autotraders-1.1.2/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-22 19:50:26.000000 autotraders-1.1.2/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-22 19:50:26.000000 autotraders-1.1.2/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-22 19:50:26.000000 autotraders-1.1.2/autotraders/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-22 19:50:26.000000 autotraders-1.1.2/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:50:41.436876 autotraders-1.1.2/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-22 19:50:41.000000 autotraders-1.1.2/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-22 19:50:41.000000 autotraders-1.1.2/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:50:41.000000 autotraders-1.1.2/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 19:50:41.000000 autotraders-1.1.2/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-22 19:50:26.000000 autotraders-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 19:50:41.440876 autotraders-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:50:41.440876 autotraders-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:50:26.000000 autotraders-1.1.2/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-22 19:50:26.000000 autotraders-1.1.2/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-22 19:50:26.000000 autotraders-1.1.2/tests/test_util.py
```

### Comparing `autotraders-1.1.1/LICENSE` & `autotraders-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.1/PKG-INFO` & `autotraders-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.1.1
+Version: 1.1.2
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.1.1/README.md` & `autotraders-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.1/autotraders/agent.py` & `autotraders-1.1.2/autotraders/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         self.ships = None
         self.headquarters = None
         super().__init__(session, update, session.base_url + "my/agent")
 
     def update(self, data=None):
         """Uses 3 API requests to get all agent details"""
         if data is None:
-            data = self.get("")["data"]
+            data = self.get()["data"]
         self.account_id = data["accountId"]
         self.symbol = data["symbol"]
         self.headquarters = data["headquarters"]
         self.credits = data["credits"]
         self.starting_faction = data["startingFaction"]
         self.ships = get_all_ships(self.session)
         self.contracts = get_all_contracts(self.session)
```

### Comparing `autotraders-1.1.1/autotraders/faction/__init__.py` & `autotraders-1.1.2/autotraders/faction/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.description = None
         self.name = None
         self.symbol = symbol
         super().__init__(session, update, session.base_url + "factions/" + self.symbol)
 
     def update(self, data=None):
         if data is None:
-            data = self.get("")["data"]
+            data = self.get()["data"]
         self.name = data["name"]
         self.description = data["description"]
         self.headquarters = MapSymbol(data["headquarters"])
         self.traits = []
         for trait in data["traits"]:
             self.traits.append(Trait(trait))
         self.is_recruting = data["isRecruiting"]
```

### Comparing `autotraders-1.1.1/autotraders/faction/contract.py` & `autotraders-1.1.2/autotraders/faction/contract.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.1/autotraders/map/system.py` & `autotraders-1.1.2/autotraders/map/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         self.star_type = None
         super().__init__(
             session, update, session.base_url + "systems/" + str(self.symbol) + "/"
         )
 
     def update(self, data=None):
         if data is None:
-            data = self.get("")["data"]
+            data = self.get()["data"]
         self.waypoints = []
         self.x = data["x"]
         self.y = data["y"]
         self.factions = data["factions"]
         self.star_type = data["type"]
         for w in data["waypoints"]:
             waypoint = Waypoint(w["symbol"], self.session, False)
```

### Comparing `autotraders-1.1.1/autotraders/map/waypoint.py` & `autotraders-1.1.2/autotraders/map/waypoint.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.1/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.1.2/autotraders/map/waypoint_types/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.1/autotraders/map/waypoint_types/jumpgate.py` & `autotraders-1.1.2/autotraders/map/waypoint_types/jumpgate.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,11 +8,11 @@
     def __init__(self, waypoint: str, session: AutoTradersSession, update=True):
         self.faction_symbol = ""
         self.jump_range = math.nan
         super().__init__(waypoint, "jump-gate", session, update)
 
     def update(self, data: dict = None):
         if data is None:
-            data = self.get("")["data"]
+            data = self.get()["data"]
         self.jump_range = data["jumpRange"]
         if "factionSymbol" in data:
             self.faction_symbol = data["factionSymbol"]
```

### Comparing `autotraders-1.1.1/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.1.2/autotraders/map/waypoint_types/marketplace.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.1/autotraders/map/waypoint_types/shipyard.py` & `autotraders-1.1.2/autotraders/map/waypoint_types/shipyard.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.1/autotraders/session.py` & `autotraders-1.1.2/autotraders/session.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.1/autotraders/shared_models/map_symbol.py` & `autotraders-1.1.2/autotraders/shared_models/map_symbol.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,22 +5,25 @@
         """Your input must be a valid symbol for a sector, system, or waypoint. or a value error might be raised.
         :param s: The symbol
         """
         if type(s) is MapSymbol:
             s = str(s)
         split = s.split("-")
         self.sector = split[0]
-        if len(split) == 2:
+        if len(split) > 1:
             self.system = split[0] + "-" + split[1]
-        if len(split) == 3:
+        if len(split) > 2:
             self.waypoint = split[0] + "-" + split[1] + "-" + split[2]
         if len(split) > 3:
             raise ValueError("Invalid map symbol")
         self.raw = s
 
     def __str__(self):
         """Returns the input that was passed as a string."""
         return self.raw
 
     def __div__(self, other):
-        """Concatenates with a "-", TODO: sanity checks"""
+        """Concatenates with a '-'"""
+        assert isinstance(other, str)
+        if other[0] == "-":
+            other = other[1:]
         return MapSymbol(str(self) + "-" + other)
```

### Comparing `autotraders-1.1.1/autotraders/ship/__init__.py` & `autotraders-1.1.2/autotraders/ship/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 
 from autotraders import SpaceTradersEntity
+from autotraders.map.system import System
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.ship.ship_components import Frame, Reactor, Engine, Module, Mount
 from autotraders.ship.survey import Survey
 from autotraders.util import parse_time
 from autotraders.map.waypoint import Waypoint
 
@@ -70,15 +71,15 @@
         self.crew = None
         super().__init__(
             session, update, session.base_url + "my/ships/" + self.symbol + "/"
         )
 
     def update(self, data: dict = None, hard=False):
         if data is None:
-            data = self.get("")["data"]  # TODO: This is a hack (sort of)
+            data = self.get()["data"]
         if self.crew is None and not hard:
             self.crew = Crew(data["crew"])
         if self.frame is None and not hard:
             self.frame = Frame(data["frame"])
         if self.reactor is None and not hard:
             self.reactor = Reactor(data["reactor"])
         if self.engine is None and not hard:
@@ -114,15 +115,15 @@
         """
         j = self.post("navigate", data={"waypointSymbol": waypoint})
         self.update(j["data"])
 
     def patch_navigation(self, new_flight_mode):
         r = self.session.patch(
             self.session.base_url + "my/ships/" + self.symbol + "/nav",
-            data={"flightMode": new_flight_mode},  # TODO: Test
+            data={"flightMode": new_flight_mode}
         )
         j = r.json()
         if "error" in j:
             raise IOError(j["error"]["message"])
         self.update({"nav": j["data"]})
 
     def dock(self):
@@ -197,49 +198,53 @@
         j = self.post(
             "jettison",
             data={"symbol": cargo_symbol, "units": quantity},
         )
         self.update(j["data"])
 
     def refine(self, output_symbol: str):
-        j = self.post(  # TODO: Fix
+        j = self.post(
             "refine",
             data={"produce": output_symbol},
         )
         self.update(j["data"])
         self.reactor.cooldown = parse_time(j["cooldown"]["expiration"])
 
     def chart(self) -> Waypoint:
         """
         Charts the current waypoint
         :return: The info about the waypoint that has been charted
         """
         j = self.post("chart")
         w = Waypoint(j["data"]["waypoint"]["symbol"], self.session, False)
         w.update(j["data"]["waypoint"])
-        self.update()  # TODO: Fix
         return w
 
     def survey(self) -> list[Survey]:
         j = self.post("survey")
         surveys = []
         for s in j["data"]["surveys"]:
             surveys.append(Survey(s))
         self.reactor.cooldown = parse_time(j["cooldown"]["expiration"])
         return surveys
 
     def scan_systems(self):
         j = self.post("scan/systems")
+        systems = []
+        for system in j["systems"]:
+            s = System(system["symbol"], self.session, False)
+            s.update(system)
+            systems.append(s)
         self.reactor.cooldown = parse_time(j["cooldown"]["expiration"])
-        raise NotImplementedError  # TODO: Fix
+        return systems
 
     def scan_waypoints(self):
         j = self.post("scan/waypoints")
         waypoints = []
-        for waypoint in j["systems"]:
+        for waypoint in j["waypoints"]:
             s = Waypoint(waypoint["symbol"], self.session, False)
             s.update(waypoint)
             waypoints.append(s)
         self.reactor.cooldown = parse_time(j["cooldown"]["expiration"])
         return waypoints
 
     def scan_ships(self):
```

### Comparing `autotraders-1.1.1/autotraders/ship/ship_components.py` & `autotraders-1.1.2/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.1/autotraders.egg-info/PKG-INFO` & `autotraders-1.1.2/autotraders.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.1.1
+Version: 1.1.2
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.1.1/autotraders.egg-info/SOURCES.txt` & `autotraders-1.1.2/autotraders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.1/pyproject.toml` & `autotraders-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `autotraders-1.1.1/tests/test_init.py` & `autotraders-1.1.2/tests/test_init.py`

 * *Files identical despite different names*

