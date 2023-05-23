# Comparing `tmp/itscalledsoccer-0.2.0.tar.gz` & `tmp/itscalledsoccer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itscalledsoccer-0.2.0.tar", last modified: Fri Apr 15 04:14:07 2022, max compression
+gzip compressed data, was "itscalledsoccer-1.0.0.tar", last modified: Tue May 23 01:18:23 2023, max compression
```

## Comparing `itscalledsoccer-0.2.0.tar` & `itscalledsoccer-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 04:14:07.191004 itscalledsoccer-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-04-15 04:13:54.000000 itscalledsoccer-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2951 2022-04-15 04:14:07.191004 itscalledsoccer-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-04-15 04:13:54.000000 itscalledsoccer-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 04:14:07.191004 itscalledsoccer-0.2.0/itscalledsoccer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-15 04:13:54.000000 itscalledsoccer-0.2.0/itscalledsoccer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3885 2022-04-15 04:13:54.000000 itscalledsoccer-0.2.0/itscalledsoccer/classes.py
--rw-r--r--   0 runner    (1001) docker     (121)    39306 2022-04-15 04:13:54.000000 itscalledsoccer-0.2.0/itscalledsoccer/client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 04:14:07.191004 itscalledsoccer-0.2.0/itscalledsoccer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2951 2022-04-15 04:14:07.000000 itscalledsoccer-0.2.0/itscalledsoccer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-04-15 04:14:07.000000 itscalledsoccer-0.2.0/itscalledsoccer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-15 04:14:07.000000 itscalledsoccer-0.2.0/itscalledsoccer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-04-15 04:14:07.000000 itscalledsoccer-0.2.0/itscalledsoccer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-04-15 04:14:07.000000 itscalledsoccer-0.2.0/itscalledsoccer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-15 04:14:07.191004 itscalledsoccer-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-04-15 04:13:54.000000 itscalledsoccer-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:18:23.420781 itscalledsoccer-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-23 01:18:12.000000 itscalledsoccer-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-23 01:18:23.420781 itscalledsoccer-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-23 01:18:12.000000 itscalledsoccer-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:18:23.420781 itscalledsoccer-1.0.0/itscalledsoccer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:18:12.000000 itscalledsoccer-1.0.0/itscalledsoccer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-23 01:18:12.000000 itscalledsoccer-1.0.0/itscalledsoccer/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39482 2023-05-23 01:18:12.000000 itscalledsoccer-1.0.0/itscalledsoccer/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:18:23.420781 itscalledsoccer-1.0.0/itscalledsoccer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-23 01:18:23.000000 itscalledsoccer-1.0.0/itscalledsoccer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-23 01:18:23.000000 itscalledsoccer-1.0.0/itscalledsoccer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 01:18:23.000000 itscalledsoccer-1.0.0/itscalledsoccer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-23 01:18:23.000000 itscalledsoccer-1.0.0/itscalledsoccer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 01:18:23.000000 itscalledsoccer-1.0.0/itscalledsoccer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 01:18:23.420781 itscalledsoccer-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-23 01:18:12.000000 itscalledsoccer-1.0.0/setup.py
```

### Comparing `itscalledsoccer-0.2.0/LICENSE` & `itscalledsoccer-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `itscalledsoccer-0.2.0/PKG-INFO` & `itscalledsoccer-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 Metadata-Version: 2.1
 Name: itscalledsoccer
-Version: 0.2.0
+Version: 1.0.0
 Summary: Programmatically interact with the American Soccer Analysis API
 Home-page: https://github.com/American-Soccer-Analysis/itscalledsoccer
 Author: American Soccer Analysis
 Author-email: americansocceranalysis@gmail.com
-License: UNKNOWN
 Keywords: stats soccer api american machine learning football
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# itscalledsoccer 
+# itscalledsoccer
 
-<img src="https://raw.githubusercontent.com/American-Soccer-Analysis/itscalledsoccer/main/R-package/man/figures/logo.png" align="right" height="175"/>
+<img src="https://raw.githubusercontent.com/American-Soccer-Analysis/itscalledsoccer-r/main/man/figures/logo.png" align="right" height="175"/>
 
 <!-- badges: start -->
 [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
 ![PyPi Version](https://img.shields.io/pypi/v/itscalledsoccer.svg)
 ![Python tests](https://github.com/American-Soccer-Analysis/itscalledsoccer/actions/workflows/python-tests.yml/badge.svg)
-[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 <!-- badges: end -->
 
+---
+
+:warning: **`itscalledsoccer` has been split up into multiple repositories. If you're looking for the R or JavaScript version, check out the links below** :warning::
+
+- [itscalledsoccer-r](https://github.com/American-Soccer-Analysis/itscalledsoccer-r)
+- [itscalledsoccer-js](https://github.com/American-Soccer-Analysis/itscalledsoccer-js)
+
+---
+
 ## Table of Contents
 
 - [itscalledsoccer](#itscalledsoccer)
   - [Table of Contents](#table-of-contents)
   - [Background](#background)
   - [Install](#install)
   - [Usage](#usage)
@@ -72,9 +80,7 @@
 ## Contributing
 
 Feel free to open an issue or submit a pull request.
 
 ## License
 
 MIT © itscalledsoccer authors
-
-
```

### Comparing `itscalledsoccer-0.2.0/README.md` & `itscalledsoccer-1.0.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,27 @@
-# itscalledsoccer 
+# itscalledsoccer
 
-<img src="https://raw.githubusercontent.com/American-Soccer-Analysis/itscalledsoccer/main/R-package/man/figures/logo.png" align="right" height="175"/>
+<img src="https://raw.githubusercontent.com/American-Soccer-Analysis/itscalledsoccer-r/main/man/figures/logo.png" align="right" height="175"/>
 
 <!-- badges: start -->
 [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
 ![PyPi Version](https://img.shields.io/pypi/v/itscalledsoccer.svg)
 ![Python tests](https://github.com/American-Soccer-Analysis/itscalledsoccer/actions/workflows/python-tests.yml/badge.svg)
-[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 <!-- badges: end -->
 
+---
+
+:warning: **`itscalledsoccer` has been split up into multiple repositories. If you're looking for the R or JavaScript version, check out the links below** :warning::
+
+- [itscalledsoccer-r](https://github.com/American-Soccer-Analysis/itscalledsoccer-r)
+- [itscalledsoccer-js](https://github.com/American-Soccer-Analysis/itscalledsoccer-js)
+
+---
+
 ## Table of Contents
 
 - [itscalledsoccer](#itscalledsoccer)
   - [Table of Contents](#table-of-contents)
   - [Background](#background)
   - [Install](#install)
   - [Usage](#usage)
```

### Comparing `itscalledsoccer-0.2.0/itscalledsoccer/classes.py` & `itscalledsoccer-1.0.0/itscalledsoccer/classes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import List, Optional
 
 
 class Game:
     def __init__(
         self,
         game_id: str,
         date_time_utc: str,
@@ -54,16 +54,16 @@
         birth_date: str,
         height_ft: int,
         height_in: int,
         weight_lb: int,
         nationality: str,
         primary_broad_position: str,
         primary_general_position: str,
-        secondary_broad_position: str = None,
-        secondary_general_position: str = None,
+        secondary_broad_position: Optional[str] = None,
+        secondary_general_position: Optional[str] = None,
         season_name: List[str] = [],
     ) -> None:
         self.player_id = player_id
         self.player_name = player_name
         self.birth_date = birth_date
         self.height_ft = height_ft
         self.height_in = height_in
@@ -84,27 +84,27 @@
 
 
 class Stadium:
     def __init__(
         self,
         stadium_id: str,
         stadium_name: str,
-        capacity: int = None,
-        year_built: int = None,
-        roof: bool = None,
-        turf: bool = None,
-        street: str = None,
-        city: str = None,
-        province: str = None,
-        country: str = None,
-        postal_code: str = None,
-        latitude: float = None,
-        longitude: float = None,
-        field_x: int = None,
-        field_y: int = None,
+        capacity: Optional[int] = None,
+        year_built: Optional[int] = None,
+        roof: Optional[bool] = None,
+        turf: Optional[bool] = None,
+        street: Optional[str] = None,
+        city: Optional[str] = None,
+        province: Optional[str] = None,
+        country: Optional[str] = None,
+        postal_code: Optional[str] = None,
+        latitude: Optional[float] = None,
+        longitude: Optional[float] = None,
+        field_x: Optional[int] = None,
+        field_y: Optional[int] = None,
     ) -> None:
         self.stadium_id = stadium_id
         self.stadium_name = stadium_name
         self.capacity = capacity
         self.year_built = year_built
         self.roof = roof
         self.turf = turf
```

### Comparing `itscalledsoccer-0.2.0/itscalledsoccer/client.py` & `itscalledsoccer-1.0.0/itscalledsoccer/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         plural_type = f"{type}s" if type != "stadia" else f"{type}"
         print(f"Gathering all {plural_type}")
         df = pd.DataFrame([])
         for league in self.LEAGUES:
             url = f"{self.BASE_URL}{league}/{plural_type}"
             resp_df = self._execute_query(url, {})
             resp_df = resp_df.assign(competition=league)
-            df = df.append(resp_df)
+            df = pd.concat([df, resp_df], ignore_index=True)
         return df
 
     def _convert_name_to_id(self, type: str, name: str) -> str:
         """Converts the name of a player, manager, stadium, referee or team
         to their corresponding id.
 
         :param type: type of name to convert
@@ -244,15 +244,15 @@
 
         if isinstance(response, pd.DataFrame):
             offset = self.MAX_API_LIMIT
 
             while len(temp_response.index) == self.MAX_API_LIMIT:
                 params["offset"] = str(offset)
                 temp_response = self._single_request(url, params)
-                response = response.append(temp_response)
+                response = pd.concat([response, temp_response], ignore_index=True)
                 offset = offset + self.MAX_API_LIMIT
 
         return response
 
     def _single_request(
         self, url: str, params: Dict[str, Union[str, List[str], None]]
     ) -> pd.DataFrame:
@@ -339,100 +339,100 @@
 
                 stats = pd.concat([stats, response])
 
         return stats
 
     def get_stadia(
         self,
-        leagues: Union[str, List[str]] = None,
-        ids: Union[str, List[str]] = None,
-        names: Union[str, List[str]] = None,
+        leagues: Union[str, List[str], None] = None,
+        ids: Union[str, List[str], None] = None,
+        names: Union[str, List[str], None] = None,
     ) -> pd.DataFrame:
         """Get information associated with stadia
 
         :param leagues: league abbreviation or a list of league abbreviations
         :param ids: a single stadium id or a list of stadia ids (optional)
         :param names: a single stadium name or a list of stadia names (optional)
         :returns: Dataframe
         """
         stadia = self._filter_entity(self.stadia, "stadium", leagues, ids, names)
         return stadia
 
     def get_referees(
         self,
-        leagues: Union[str, List[str]] = None,
-        ids: Union[str, List[str]] = None,
-        names: Union[str, List[str]] = None,
+        leagues: Union[str, List[str], None] = None,
+        ids: Union[str, List[str], None] = None,
+        names: Union[str, List[str], None] = None,
     ) -> pd.DataFrame:
         """Get information associated with referees
 
         :param leagues: league abbreviation or a list of league abbreviations
         :param ids: a single referee id or a list of referee ids (optional)
         :param names: a single referee name or a list of referee names (optional)
         :returns: Dataframe
         """
         referees = self._filter_entity(self.referees, "referee", leagues, ids, names)
         return referees
 
     def get_managers(
         self,
-        leagues: Union[str, List[str]] = None,
-        ids: Union[str, List[str]] = None,
-        names: Union[str, List[str]] = None,
+        leagues: Union[str, List[str], None] = None,
+        ids: Union[str, List[str], None] = None,
+        names: Union[str, List[str], None] = None,
     ) -> pd.DataFrame:
         """Get information associated with managers
 
         :param leagues: league abbreviation or a list of league abbreviations
         :param ids: a single referee id or a list of referee ids (optional)
         :param names: a single referee name or a list of referee names (optional)
         :returns: Dataframe
         """
         managers = self._filter_entity(self.managers, "manager", leagues, ids, names)
         return managers
 
     def get_teams(
         self,
-        leagues: Union[str, List[str]] = None,
-        ids: Union[str, List[str]] = None,
-        names: Union[str, List[str]] = None,
+        leagues: Union[str, List[str], None] = None,
+        ids: Union[str, List[str], None] = None,
+        names: Union[str, List[str], None] = None,
     ) -> pd.DataFrame:
         """Get information associated with teams
 
         :param leagues: league abbreviation or a list of league abbreviations
         :param ids: a single team id or a list of team ids (optional)
         :param names: a single team name or a list of team names (optional)
         :returns: Dataframe
         """
         teams = self._filter_entity(self.teams, "team", leagues, ids, names)
         return teams
 
     def get_players(
         self,
-        leagues: Union[str, List[str]] = None,
-        ids: Union[str, List[str]] = None,
-        names: Union[str, List[str]] = None,
+        leagues: Union[str, List[str], None] = None,
+        ids: Union[str, List[str], None] = None,
+        names: Union[str, List[str], None] = None,
     ) -> pd.DataFrame:
         """Get information associated with players
 
         :param league: league abbreviation or a list of league abbreviations
         :param ids: a single player id or a list of player ids (optional)
         :param names: a single player name or a list of player names (optional)
         :returns: Dataframe
         """
         players = self._filter_entity(self.players, "player", leagues, ids, names)
         return players
 
     def get_games(
         self,
-        leagues: Union[str, List[str]] = None,
-        game_ids: Union[str, List[str]] = None,
-        team_ids: Union[str, List[str]] = None,
-        team_names: Union[str, List[str]] = None,
-        seasons: Union[str, List[str]] = None,
-        stages: Union[str, List[str]] = None,
+        leagues: Union[str, List[str], None] = None,
+        game_ids: Union[str, List[str], None] = None,
+        team_ids: Union[str, List[str], None] = None,
+        team_names: Union[str, List[str], None] = None,
+        seasons: Union[str, List[str], None] = None,
+        stages: Union[str, List[str], None] = None,
     ) -> pd.DataFrame:
         """Get information related to games
 
         :param leagues: league abbreviation or a list of league abbreviations
         :param game_ids: a single game id or a list of game ids
         :param team_ids: a single team id or a list of team ids
         :param team_names: a single team name or a list of team names
```

### Comparing `itscalledsoccer-0.2.0/itscalledsoccer.egg-info/PKG-INFO` & `itscalledsoccer-1.0.0/itscalledsoccer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 Metadata-Version: 2.1
 Name: itscalledsoccer
-Version: 0.2.0
+Version: 1.0.0
 Summary: Programmatically interact with the American Soccer Analysis API
 Home-page: https://github.com/American-Soccer-Analysis/itscalledsoccer
 Author: American Soccer Analysis
 Author-email: americansocceranalysis@gmail.com
-License: UNKNOWN
 Keywords: stats soccer api american machine learning football
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# itscalledsoccer 
+# itscalledsoccer
 
-<img src="https://raw.githubusercontent.com/American-Soccer-Analysis/itscalledsoccer/main/R-package/man/figures/logo.png" align="right" height="175"/>
+<img src="https://raw.githubusercontent.com/American-Soccer-Analysis/itscalledsoccer-r/main/man/figures/logo.png" align="right" height="175"/>
 
 <!-- badges: start -->
 [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
 ![PyPi Version](https://img.shields.io/pypi/v/itscalledsoccer.svg)
 ![Python tests](https://github.com/American-Soccer-Analysis/itscalledsoccer/actions/workflows/python-tests.yml/badge.svg)
-[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 <!-- badges: end -->
 
+---
+
+:warning: **`itscalledsoccer` has been split up into multiple repositories. If you're looking for the R or JavaScript version, check out the links below** :warning::
+
+- [itscalledsoccer-r](https://github.com/American-Soccer-Analysis/itscalledsoccer-r)
+- [itscalledsoccer-js](https://github.com/American-Soccer-Analysis/itscalledsoccer-js)
+
+---
+
 ## Table of Contents
 
 - [itscalledsoccer](#itscalledsoccer)
   - [Table of Contents](#table-of-contents)
   - [Background](#background)
   - [Install](#install)
   - [Usage](#usage)
@@ -72,9 +80,7 @@
 ## Contributing
 
 Feel free to open an issue or submit a pull request.
 
 ## License
 
 MIT © itscalledsoccer authors
-
-
```

### Comparing `itscalledsoccer-0.2.0/setup.py` & `itscalledsoccer-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,30 +2,31 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="itscalledsoccer",
     packages=find_packages(exclude=["tests", "tests.*"]),
-    version="0.2.0",
+    version="1.0.0",
     description="Programmatically interact with the American Soccer Analysis API",
     long_description=long_description,
-    long_description_content_type = "text/markdown",
+    long_description_content_type="text/markdown",
     author="American Soccer Analysis",
     author_email="americansocceranalysis@gmail.com",
     url="https://github.com/American-Soccer-Analysis/itscalledsoccer",
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     keywords="stats soccer api american machine learning football",
     install_requires=[
-        "requests==2.25.1",
-        "CacheControl==0.12.6",
-        "rapidfuzz==1.9.1",
-        "pandas==1.3.1"
-    ]
+        "requests==2.31.0",
+        "CacheControl==0.12.11",
+        "rapidfuzz==3.0.0",
+        "pandas==2.0.1",
+    ],
 )
```

