# Comparing `tmp/wom_py-0.4.0.tar.gz` & `tmp/wom_py-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wom_py-0.4.0.tar", max compression
+gzip compressed data, was "wom_py-0.4.1.tar", max compression
```

## Comparing `wom_py-0.4.0.tar` & `wom_py-0.4.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1074 2023-05-13 21:57:03.117573 wom_py-0.4.0/LICENSE
--rw-r--r--   0        0        0     2712 2023-05-13 21:57:03.117573 wom_py-0.4.0/README.md
--rw-r--r--   0        0        0     2138 2023-05-13 21:57:03.117573 wom_py-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4385 2023-05-13 21:57:03.221574 wom_py-0.4.0/wom/__init__.py
--rw-r--r--   0        0        0     1324 2023-05-13 21:57:03.117573 wom_py-0.4.0/wom/__main__.py
--rw-r--r--   0        0        0     1808 2023-05-13 21:57:03.117573 wom_py-0.4.0/wom/_cli.py
--rw-r--r--   0        0        0     8648 2023-05-13 21:57:03.117573 wom_py-0.4.0/wom/client.py
--rw-r--r--   0        0        0     1447 2023-05-13 21:57:03.117573 wom_py-0.4.0/wom/constants.py
--rw-r--r--   0        0        0     7008 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/enums.py
--rw-r--r--   0        0        0     1729 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/errors.py
--rw-r--r--   0        0        0     3228 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/__init__.py
--rw-r--r--   0        0        0     1557 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/base.py
--rw-r--r--   0        0        0     1673 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/competitions/__init__.py
--rw-r--r--   0        0        0     1591 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/competitions/enums.py
--rw-r--r--   0        0        0     7413 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/competitions/models.py
--rw-r--r--   0        0        0     1289 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/deltas/__init__.py
--rw-r--r--   0        0        0     1824 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/deltas/models.py
--rw-r--r--   0        0        0     1716 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/groups/__init__.py
--rw-r--r--   0        0        0     7780 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/groups/enums.py
--rw-r--r--   0        0        0     9139 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/groups/models.py
--rw-r--r--   0        0        0     1738 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/http.py
--rw-r--r--   0        0        0     1471 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/names/__init__.py
--rw-r--r--   0        0        0     1793 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/names/enums.py
--rw-r--r--   0        0        0     5289 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/names/models.py
--rw-r--r--   0        0        0     1754 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/players/__init__.py
--rw-r--r--   0        0        0     5664 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/players/enums.py
--rw-r--r--   0        0        0    11907 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/players/models.py
--rw-r--r--   0        0        0     1300 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/records/__init__.py
--rw-r--r--   0        0        0     2217 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/records/models.py
--rw-r--r--   0        0        0        0 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/py.typed
--rw-r--r--   0        0        0     5561 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/result.py
--rw-r--r--   0        0        0     6505 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/routes.py
--rw-r--r--   0        0        0    34101 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/serializer.py
--rw-r--r--   0        0        0     1709 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/services/__init__.py
--rw-r--r--   0        0        0     2050 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/services/base.py
--rw-r--r--   0        0        0    21170 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/services/competitions.py
--rw-r--r--   0        0        0     3528 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/services/deltas.py
--rw-r--r--   0        0        0     3688 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/services/efficiency.py
--rw-r--r--   0        0        0    24099 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/services/groups.py
--rw-r--r--   0        0        0     5772 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/services/http.py
--rw-r--r--   0        0        0     4031 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/services/names.py
--rw-r--r--   0        0        0    18088 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/services/players.py
--rw-r--r--   0        0        0     3506 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/services/records.py
--rw-r--r--   0        0        0     4030 1970-01-01 00:00:00.000000 wom_py-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-23 00:08:59.093807 wom_py-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2712 2023-05-23 00:08:59.093807 wom_py-0.4.1/README.md
+-rw-r--r--   0        0        0     2138 2023-05-23 00:08:59.093807 wom_py-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4385 2023-05-23 00:08:59.173811 wom_py-0.4.1/wom/__init__.py
+-rw-r--r--   0        0        0     1324 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/__main__.py
+-rw-r--r--   0        0        0     1808 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/_cli.py
+-rw-r--r--   0        0        0     8648 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/client.py
+-rw-r--r--   0        0        0     1447 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/constants.py
+-rw-r--r--   0        0        0     7010 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/enums.py
+-rw-r--r--   0        0        0     1729 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/errors.py
+-rw-r--r--   0        0        0     3228 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/__init__.py
+-rw-r--r--   0        0        0     1557 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/base.py
+-rw-r--r--   0        0        0     1673 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/competitions/__init__.py
+-rw-r--r--   0        0        0     1591 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/competitions/enums.py
+-rw-r--r--   0        0        0     7413 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/competitions/models.py
+-rw-r--r--   0        0        0     1289 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/deltas/__init__.py
+-rw-r--r--   0        0        0     1824 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/deltas/models.py
+-rw-r--r--   0        0        0     1716 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/groups/__init__.py
+-rw-r--r--   0        0        0     7780 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/groups/enums.py
+-rw-r--r--   0        0        0     9275 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/groups/models.py
+-rw-r--r--   0        0        0     1738 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/http.py
+-rw-r--r--   0        0        0     1471 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/names/__init__.py
+-rw-r--r--   0        0        0     1793 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/names/enums.py
+-rw-r--r--   0        0        0     5138 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/names/models.py
+-rw-r--r--   0        0        0     1754 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/players/__init__.py
+-rw-r--r--   0        0        0     5664 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/players/enums.py
+-rw-r--r--   0        0        0    11907 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/players/models.py
+-rw-r--r--   0        0        0     1300 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/records/__init__.py
+-rw-r--r--   0        0        0     2217 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/records/models.py
+-rw-r--r--   0        0        0        0 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/py.typed
+-rw-r--r--   0        0        0     5561 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/result.py
+-rw-r--r--   0        0        0     6505 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/routes.py
+-rw-r--r--   0        0        0    34477 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/serializer.py
+-rw-r--r--   0        0        0     1709 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/services/__init__.py
+-rw-r--r--   0        0        0     2050 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/services/base.py
+-rw-r--r--   0        0        0    21170 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/services/competitions.py
+-rw-r--r--   0        0        0     3528 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/services/deltas.py
+-rw-r--r--   0        0        0     3688 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/services/efficiency.py
+-rw-r--r--   0        0        0    24099 2023-05-23 00:08:59.101808 wom_py-0.4.1/wom/services/groups.py
+-rw-r--r--   0        0        0     5772 2023-05-23 00:08:59.101808 wom_py-0.4.1/wom/services/http.py
+-rw-r--r--   0        0        0     4031 2023-05-23 00:08:59.101808 wom_py-0.4.1/wom/services/names.py
+-rw-r--r--   0        0        0    18088 2023-05-23 00:08:59.101808 wom_py-0.4.1/wom/services/players.py
+-rw-r--r--   0        0        0     3506 2023-05-23 00:08:59.101808 wom_py-0.4.1/wom/services/records.py
+-rw-r--r--   0        0        0     3828 1970-01-01 00:00:00.000000 wom_py-0.4.1/PKG-INFO
```

### Comparing `wom_py-0.4.0/LICENSE` & `wom_py-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/README.md` & `wom_py-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/pyproject.toml` & `wom_py-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wom.py"
-version = "0.4.0"
+version = "0.4.1"
 description = "An asynchronous wrapper for the Wise Old Man API."
 authors = ["Jonxslays"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jonxslays/wom.py"
 repository = "https://github.com/Jonxslays/wom.py"
 documentation = "https://jonxslays.github.io/wom.py"
```

### Comparing `wom_py-0.4.0/wom/__init__.py` & `wom_py-0.4.1/wom/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,23 +28,23 @@
 """
 
 from __future__ import annotations
 
 from typing import Final
 
 __packagename__: Final[str] = "wom.py"
-__version__: Final[str] = "0.4.0"
+__version__: Final[str] = "0.4.1"
 __author__: Final[str] = "Jonxslays"
 __copyright__: Final[str] = "2023-present Jonxslays"
 __description__: Final[str] = "An asynchronous wrapper for the Wise Old Man API."
 __url__: Final[str] = "https://github.com/Jonxslays/wom.py"
 __docs__: Final[str] = "https://jonxslays.github.io/wom.py"
 __repository__: Final[str] = __url__
 __license__: Final[str] = "MIT"
-__git_sha__: Final[str] = "[47bafd3]"
+__git_sha__: Final[str] = "[c7d71ca]"
 
 from . import client
 from . import constants
 from . import enums
 from . import errors
 from . import models
 from . import result
```

### Comparing `wom_py-0.4.0/wom/__main__.py` & `wom_py-0.4.1/wom/__main__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/_cli.py` & `wom_py-0.4.1/wom/_cli.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/client.py` & `wom_py-0.4.1/wom/client.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/constants.py` & `wom_py-0.4.1/wom/constants.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/enums.py` & `wom_py-0.4.1/wom/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,58 +176,58 @@
 class Bosses(Metric):
     """Bosses from OSRS."""
 
     AbyssalSire = "abyssal_sire"
     AlchemicalHydra = "alchemical_hydra"
     Artio = "artio"
     BarrowsChests = "barrows_chests"
-    Brophyta = "bryophyta"
+    Bryophyta = "bryophyta"
     Callisto = "callisto"
     Calvarion = "calvarion"
     Cerberus = "cerberus"
     ChambersOfXeric = "chambers_of_xeric"
     ChambersOfXericChallenge = "chambers_of_xeric_challenge_mode"
     ChaosElemental = "chaos_elemental"
     ChaosFanatic = "chaos_fanatic"
     CommanderZilyana = "commander_zilyana"
     CorporealBeast = "corporeal_beast"
     CrazyArchaeologist = "crazy_archaeologist"
-    DagganothPrime = "dagannoth_prime"
-    DagganothRex = "dagannoth_rex"
-    DagganothSupreme = "dagannoth_supreme"
+    DagannothPrime = "dagannoth_prime"
+    DagannothRex = "dagannoth_rex"
+    DagannothSupreme = "dagannoth_supreme"
     DerangedArchaeologist = "deranged_archaeologist"
     GeneralGraardor = "general_graardor"
     GiantMole = "giant_mole"
     GrotesqueGuardians = "grotesque_guardians"
     Hespori = "hespori"
     KalphiteQueen = "kalphite_queen"
     KingBlackDragon = "king_black_dragon"
     Kraken = "kraken"
     Kreearra = "kreearra"
-    KrilTsutaroth = "kril_tsutsaroth"
+    KrilTsutsaroth = "kril_tsutsaroth"
     Mimic = "mimic"
     Nex = "nex"
     Nightmare = "nightmare"
     PhosanisNightmare = "phosanis_nightmare"
     Obor = "obor"
     PhantomMuspah = "phantom_muspah"
     Sarachnis = "sarachnis"
     Scorpia = "scorpia"
     Skotizo = "skotizo"
     Spindel = "spindel"
     Tempoross = "tempoross"
-    TheGuantlet = "the_gauntlet"
+    TheGauntlet = "the_gauntlet"
     TheCorruptedGauntlet = "the_corrupted_gauntlet"
     TheatreOfBlood = "theatre_of_blood"
     TheatreOfBloodHard = "theatre_of_blood_hard_mode"
     ThermonuclearSmokeDevil = "thermonuclear_smoke_devil"
     TombsOfAmascut = "tombs_of_amascut"
     TombsOfAmascutExpert = "tombs_of_amascut_expert"
-    TzkalZuk = "tzkal_zuk"
-    TztokJad = "tztok_jad"
+    TzKalZuk = "tzkal_zuk"
+    TzTokJad = "tztok_jad"
     Venenatis = "venenatis"
     Vetion = "vetion"
     Vorkath = "vorkath"
     Wintertodt = "wintertodt"
     Zalcano = "zalcano"
     Zulrah = "zulrah"
```

### Comparing `wom_py-0.4.0/wom/errors.py` & `wom_py-0.4.1/wom/errors.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/models/__init__.py` & `wom_py-0.4.1/wom/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/models/base.py` & `wom_py-0.4.1/wom/models/base.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/models/competitions/__init__.py` & `wom_py-0.4.1/wom/models/competitions/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/models/competitions/enums.py` & `wom_py-0.4.1/wom/models/competitions/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/models/competitions/models.py` & `wom_py-0.4.1/wom/models/competitions/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/models/deltas/__init__.py` & `wom_py-0.4.1/wom/models/deltas/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/models/deltas/models.py` & `wom_py-0.4.1/wom/models/deltas/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/models/groups/__init__.py` & `wom_py-0.4.1/wom/models/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/models/groups/enums.py` & `wom_py-0.4.1/wom/models/groups/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/models/groups/models.py` & `wom_py-0.4.1/wom/models/groups/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,16 +253,16 @@
 
     level: int
     """The players level in the skill."""
 
     experience: int
     """The players experience in the skill."""
 
-    player: Player
-    """The player leading in this metric."""
+    player: t.Optional[Player]
+    """The player leading in this metric, or `None` if none do."""
 
 
 @attrs.define(init=False)
 class BossLeader(BaseModel):
     """Represents a leader in a particular boss."""
 
     metric: enums.Bosses
@@ -270,16 +270,16 @@
 
     rank: int
     """The players rank in killing the boss."""
 
     kills: int
     """The number of kills the player has."""
 
-    player: Player
-    """The player leading in this metric."""
+    player: t.Optional[Player]
+    """The player leading in this metric, or `None` if none do."""
 
 
 @attrs.define(init=False)
 class ActivityLeader(BaseModel):
     """Represents a leader in a particular activity."""
 
     metric: enums.Activities
@@ -287,16 +287,16 @@
 
     rank: int
     """The players rank in the activity."""
 
     score: int
     """The players score in the activity."""
 
-    player: Player
-    """The player leading in this metric."""
+    player: t.Optional[Player]
+    """The player leading in this metric, or `None` if none do."""
 
 
 @attrs.define(init=False)
 class ComputedMetricLeader(BaseModel):
     """Represents a leader in a particular computed metric."""
 
     metric: enums.ComputedMetrics
@@ -306,16 +306,16 @@
 
     rank: int
     """The players rank in the computed metric."""
 
     value: int
     """The value of the computed metric."""
 
-    player: Player
-    """The player leading in this metric."""
+    player: t.Optional[Player]
+    """The player leading in this metric, or `None` if none do."""
 
 
 @attrs.define(init=False)
 class MetricLeaders(BaseModel):
     """The leaders for each metric in a group."""
 
     skills: t.Dict[enums.Skills, SkillLeader]
```

### Comparing `wom_py-0.4.0/wom/models/http.py` & `wom_py-0.4.1/wom/models/http.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/models/names/__init__.py` & `wom_py-0.4.1/wom/models/names/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/models/names/enums.py` & `wom_py-0.4.1/wom/models/names/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/models/names/models.py` & `wom_py-0.4.1/wom/models/names/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,16 +70,16 @@
         NameChangeReviewReason.NewNameNotFound,
         NameChangeReviewReason.NegativeGains,
     ]
     """The reason this name change was denied."""
 
     negative_gains: t.Optional[t.Dict[enums.Metric, int]]
     """The negative gains that were observed, if there were any. Only populated
-    when the reason is
-    [`NegativeGains`][wom.NameChangeReviewReason.NegativeGains]"""
+    when the reason is [`NegativeGains`][wom.NameChangeReviewReason].
+    """
 
 
 @attrs.define(init=False)
 class SkippedNameChangeReviewContext(NameChangeReviewContext):  # type: ignore[override]
     """The review context for a name change that was skipped."""
 
     reason: t.Literal[
@@ -87,47 +87,41 @@
         NameChangeReviewReason.ExcessiveGains,
         NameChangeReviewReason.TotalLevelTooLow,
     ]
     """The reason this name change was denied."""
 
     max_hours_diff: t.Optional[int]
     """The max number of hours in the transition period. Only populated when
-    reason is
-    [`TransitionTooLong`][wom.NameChangeReviewReason.TransitionTooLong].
+    reason is [`TransitionTooLong`][wom.NameChangeReviewReason].
     """
 
     hours_diff: t.Optional[int]
     """The actual number of hours in the transition period. Only populated when
-    reason is
-    [`TransitionTooLong`][wom.NameChangeReviewReason.TransitionTooLong]
-    or [`ExcessiveGains`][wom.NameChangeReviewReason.ExcessiveGains].
+    reason is [`TransitionTooLong`][wom.NameChangeReviewReason] or
+    [`ExcessiveGains`][wom.NameChangeReviewReason].
     """
 
     ehp_diff: t.Optional[int]
     """The number difference between the old and new names ehp. Only populated
-    when the reason is
-    [`ExcessiveGains`][wom.NameChangeReviewReason.ExcessiveGains].
+    when the reason is [`ExcessiveGains`][wom.NameChangeReviewReason].
     """
 
     ehb_diff: t.Optional[int]
     """The number difference between the old and new names ehb. Only populated
-    when the reason is
-    [`ExcessiveGains`][wom.NameChangeReviewReason.ExcessiveGains].
+    when the reason is [`ExcessiveGains`][wom.NameChangeReviewReason].
     """
 
     min_total_level: t.Optional[int]
     """The minimum total level allowed for this name change. Only populated
-    when the reason is
-    [`TotalLevelTooLow`][wom.NameChangeReviewReason.TotalLevelTooLow].
+    when the reason is [`TotalLevelTooLow`][wom.NameChangeReviewReason].
     """
 
     total_level: t.Optional[int]
     """The number difference between the old and new names ehb. Only populated
-    when the reason is
-    [`TotalLevelTooLow`][wom.NameChangeReviewReason.TotalLevelTooLow].
+    when the reason is [`TotalLevelTooLow`][wom.NameChangeReviewReason].
     """
 
 
 @attrs.define(init=False)
 class NameChange(BaseModel):
     """Represents a player name change."""
```

### Comparing `wom_py-0.4.0/wom/models/players/__init__.py` & `wom_py-0.4.1/wom/models/players/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/models/players/enums.py` & `wom_py-0.4.1/wom/models/players/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/models/players/models.py` & `wom_py-0.4.1/wom/models/players/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/models/records/__init__.py` & `wom_py-0.4.1/wom/models/records/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/models/records/models.py` & `wom_py-0.4.1/wom/models/records/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/result.py` & `wom_py-0.4.1/wom/result.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/routes.py` & `wom_py-0.4.1/wom/routes.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/serializer.py` & `wom_py-0.4.1/wom/serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -939,61 +939,81 @@
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         leader = models.SkillLeader()
         leader.metric = enums.Skills.from_str(data["metric"])
-        leader.player = self.deserialize_player(data["player"])
         self._set_attrs(leader, data, "experience", "rank", "level")
+
+        if player := data.get("player", None):
+            leader.player = self.deserialize_player(player)
+        else:
+            leader.player = player
+
         return leader
 
     def deserialize_boss_leader(self, data: DictT) -> models.BossLeader:
         """Deserializes the data into a boss leader model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         leader = models.BossLeader()
         leader.metric = enums.Bosses.from_str(data["metric"])
-        leader.player = self.deserialize_player(data["player"])
         self._set_attrs(leader, data, "kills", "rank")
+
+        if player := data.get("player", None):
+            leader.player = self.deserialize_player(player)
+        else:
+            leader.player = player
+
         return leader
 
     def deserialize_activity_leader(self, data: DictT) -> models.ActivityLeader:
         """Deserializes the data into an activity leader model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         leader = models.ActivityLeader()
         leader.metric = enums.Activities.from_str(data["metric"])
-        leader.player = self.deserialize_player(data["player"])
         self._set_attrs(leader, data, "score", "rank")
+
+        if player := data.get("player", None):
+            leader.player = self.deserialize_player(player)
+        else:
+            leader.player = player
+
         return leader
 
     def deserialize_computed_leader(self, data: DictT) -> models.ComputedMetricLeader:
         """Deserializes the data into a computed metric leader model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         leader = models.ComputedMetricLeader()
         leader.metric = enums.ComputedMetrics.from_str(data["metric"])
-        leader.player = self.deserialize_player(data["player"])
         self._set_attrs(leader, data, "value", "rank")
+
+        if player := data.get("player", None):
+            leader.player = self.deserialize_player(player)
+        else:
+            leader.player = player
+
         return leader
 
     def deserialize_metric_leaders(self, data: DictT) -> models.MetricLeaders:
         """Deserializes the data into a metric leaders model.
 
         Args:
             data: The JSON payload.
```

### Comparing `wom_py-0.4.0/wom/services/__init__.py` & `wom_py-0.4.1/wom/services/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/services/base.py` & `wom_py-0.4.1/wom/services/base.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/services/competitions.py` & `wom_py-0.4.1/wom/services/competitions.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/services/deltas.py` & `wom_py-0.4.1/wom/services/deltas.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/services/efficiency.py` & `wom_py-0.4.1/wom/services/efficiency.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/services/groups.py` & `wom_py-0.4.1/wom/services/groups.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/services/http.py` & `wom_py-0.4.1/wom/services/http.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/services/names.py` & `wom_py-0.4.1/wom/services/names.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/services/players.py` & `wom_py-0.4.1/wom/services/players.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/wom/services/records.py` & `wom_py-0.4.1/wom/services/records.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.0/PKG-INFO` & `wom_py-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wom-py
-Version: 0.4.0
+Version: 0.4.1
 Summary: An asynchronous wrapper for the Wise Old Man API.
 Home-page: https://github.com/Jonxslays/wom.py
 License: MIT
 Author: Jonxslays
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
@@ -13,18 +13,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: aiohttp (>3.8.1)
 Requires-Dist: attrs (>=22)
 Project-URL: Documentation, https://jonxslays.github.io/wom.py
 Project-URL: Repository, https://github.com/Jonxslays/wom.py
```

#### html2text {}

```diff
@@ -1,25 +1,22 @@
-Metadata-Version: 2.1 Name: wom-py Version: 0.4.0 Summary: An asynchronous
+Metadata-Version: 2.1 Name: wom-py Version: 0.4.1 Summary: An asynchronous
 wrapper for the Wise Old Man API. Home-page: https://github.com/Jonxslays/
 wom.py License: MIT Author: Jonxslays Requires-Python: >=3.8 Classifier:
 Development Status :: 4 - Beta Classifier: Framework :: AsyncIO Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Topic :: Software Development ::
-Libraries Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Classifier: Typing :: Typed Requires-Dist: aiohttp (>3.8.1) Requires-
-Dist: attrs (>=22) Project-URL: Documentation, https://jonxslays.github.io/
-wom.py Project-URL: Repository, https://github.com/Jonxslays/wom.py
-Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Classifier: Typing :: Typed Requires-Dist: aiohttp
+(>3.8.1) Requires-Dist: attrs (>=22) Project-URL: Documentation, https://
+jonxslays.github.io/wom.py Project-URL: Repository, https://github.com/
+Jonxslays/wom.py Description-Content-Type: text/markdown
                              ****** wom.py ******
    [Stable_version] [License] [Python_versions] [Maintainability] [Coverage]
 An asynchronous wrapper for the [Wise Old Man API](https://docs.wiseoldman.net/
 ). The library aims to make it easy to interact with the Wise Old Man API by
 providing service methods matching all available endpoints and model classes
 for data consistency. ## Documentation - [Stable](https://jonxslays.github.io/
 wom.py/) - [Development](https://jonxslays.github.io/wom.py/dev/) ##
```

