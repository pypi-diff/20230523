# Comparing `tmp/pollination-alias-0.9.8.tar.gz` & `tmp/pollination-alias-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-alias-0.9.8.tar", last modified: Wed Sep 29 12:40:16 2021, max compression
+gzip compressed data, was "dist/pollination-alias-0.9.9.tar", last modified: Thu Oct  7 23:56:44 2021, max compression
```

## Comparing `pollination-alias-0.9.8.tar` & `pollination-alias-0.9.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 12:40:16.000000 pollination-alias-0.9.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 12:40:15.000000 pollination-alias-0.9.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 12:40:16.000000 pollination-alias-0.9.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      169 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      275 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      843 2021-09-29 12:40:16.000000 pollination-alias-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      196 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 12:40:15.000000 pollination-alias-0.9.8/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 12:40:16.000000 pollination-alias-0.9.8/pollination/alias/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/pollination/alias/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 12:40:16.000000 pollination-alias-0.9.8/pollination/alias/inputs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/pollination/alias/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6275 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/pollination/alias/inputs/bool_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     5257 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/pollination/alias/inputs/comfort.py
--rw-r--r--   0 runner    (1001) docker     (121)      597 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/pollination/alias/inputs/ddy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1316 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/pollination/alias/inputs/grid.py
--rw-r--r--   0 runner    (1001) docker     (121)     6462 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/pollination/alias/inputs/model.py
--rw-r--r--   0 runner    (1001) docker     (121)      735 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/pollination/alias/inputs/north.py
--rw-r--r--   0 runner    (1001) docker     (121)     1452 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/pollination/alias/inputs/pit.py
--rw-r--r--   0 runner    (1001) docker     (121)     2629 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/pollination/alias/inputs/radiancepar.py
--rw-r--r--   0 runner    (1001) docker     (121)      619 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/pollination/alias/inputs/runperiod.py
--rw-r--r--   0 runner    (1001) docker     (121)      888 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/pollination/alias/inputs/schedule.py
--rw-r--r--   0 runner    (1001) docker     (121)     3169 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/pollination/alias/inputs/simulation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/pollination/alias/inputs/wea.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 12:40:16.000000 pollination-alias-0.9.8/pollination/alias/outputs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/pollination/alias/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9482 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/pollination/alias/outputs/comfort.py
--rw-r--r--   0 runner    (1001) docker     (121)    17711 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/pollination/alias/outputs/daylight.py
--rw-r--r--   0 runner    (1001) docker     (121)      587 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/pollination/alias/outputs/eui.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 12:40:16.000000 pollination-alias-0.9.8/pollination_alias.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      843 2021-09-29 12:40:15.000000 pollination-alias-0.9.8/pollination_alias.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2021-09-29 12:40:15.000000 pollination-alias-0.9.8/pollination_alias.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-29 12:40:15.000000 pollination-alias-0.9.8/pollination_alias.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-29 12:40:15.000000 pollination-alias-0.9.8/pollination_alias.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-09-29 12:40:15.000000 pollination-alias-0.9.8/pollination_alias.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-09-29 12:40:15.000000 pollination-alias-0.9.8/pollination_alias.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      102 2021-09-29 12:40:16.000000 pollination-alias-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2021-09-29 12:39:26.000000 pollination-alias-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 23:56:44.000000 pollination-alias-0.9.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 23:56:44.000000 pollination-alias-0.9.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 23:56:44.000000 pollination-alias-0.9.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1084 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      843 2021-10-07 23:56:44.000000 pollination-alias-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 23:56:44.000000 pollination-alias-0.9.9/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 23:56:44.000000 pollination-alias-0.9.9/pollination/alias/
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/pollination/alias/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 23:56:44.000000 pollination-alias-0.9.9/pollination/alias/inputs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/pollination/alias/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6275 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/pollination/alias/inputs/bool_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5257 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/pollination/alias/inputs/comfort.py
+-rw-r--r--   0 runner    (1001) docker     (121)      597 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/pollination/alias/inputs/ddy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2477 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/pollination/alias/inputs/grid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6462 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/pollination/alias/inputs/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)      735 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/pollination/alias/inputs/north.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1452 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/pollination/alias/inputs/pit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2629 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/pollination/alias/inputs/radiancepar.py
+-rw-r--r--   0 runner    (1001) docker     (121)      619 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/pollination/alias/inputs/runperiod.py
+-rw-r--r--   0 runner    (1001) docker     (121)      888 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/pollination/alias/inputs/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3169 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/pollination/alias/inputs/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1196 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/pollination/alias/inputs/wea.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 23:56:44.000000 pollination-alias-0.9.9/pollination/alias/outputs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/pollination/alias/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9482 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/pollination/alias/outputs/comfort.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17711 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/pollination/alias/outputs/daylight.py
+-rw-r--r--   0 runner    (1001) docker     (121)      587 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/pollination/alias/outputs/eui.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 23:56:44.000000 pollination-alias-0.9.9/pollination_alias.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      843 2021-10-07 23:56:44.000000 pollination-alias-0.9.9/pollination_alias.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1022 2021-10-07 23:56:44.000000 pollination-alias-0.9.9/pollination_alias.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-07 23:56:44.000000 pollination-alias-0.9.9/pollination_alias.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-07 23:56:44.000000 pollination-alias-0.9.9/pollination_alias.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-10-07 23:56:44.000000 pollination-alias-0.9.9/pollination_alias.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-10-07 23:56:44.000000 pollination-alias-0.9.9/pollination_alias.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2021-10-07 23:56:44.000000 pollination-alias-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1058 2021-10-07 23:55:57.000000 pollination-alias-0.9.9/setup.py
```

### Comparing `pollination-alias-0.9.8/.github/workflows/ci.yaml` & `pollination-alias-0.9.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-alias-0.9.8/LICENSE` & `pollination-alias-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-alias-0.9.8/PKG-INFO` & `pollination-alias-0.9.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-alias
-Version: 0.9.8
+Version: 0.9.9
 Summary: Collection of alias inputs and outputs for Pollination recipes.
 Home-page: https://github.com/pollination/pollination-alias
 Author: Pollination
 Author-email: info@pollination.cloud
 License: Apache-2.0 License
 Description: # pollination-alias
         A collection of input and output aliases for Pollination Recipe's inputs and outputs.
```

### Comparing `pollination-alias-0.9.8/pollination/alias/inputs/bool_options.py` & `pollination-alias-0.9.9/pollination/alias/inputs/bool_options.py`

 * *Files identical despite different names*

### Comparing `pollination-alias-0.9.8/pollination/alias/inputs/comfort.py` & `pollination-alias-0.9.9/pollination/alias/inputs/comfort.py`

 * *Files identical despite different names*

### Comparing `pollination-alias-0.9.8/pollination/alias/inputs/ddy.py` & `pollination-alias-0.9.9/pollination/alias/inputs/ddy.py`

 * *Files identical despite different names*

### Comparing `pollination-alias-0.9.8/pollination/alias/inputs/grid.py` & `pollination-alias-0.9.9/pollination/alias/inputs/grid.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from queenbee.io.common import IOAliasHandler
 
 
 """Alias for text that filters the simulated radiance grids."""
 grid_filter_input = [
     InputAlias.str(
         name='grid_filter',
-        description='Text for a grid identifer or a pattern to filter the sensor grids '
+        description='Text for a grid identifier or a pattern to filter the sensor grids '
         'of the model that are simulated. For instance, first_floor_* will simulate '
         'only the sensor grids that have an identifier that starts with '
         'first_floor_. By default, all grids in the model will be simulated.',
         default='*',
         platform=['grasshopper']
     )
 ]
@@ -26,7 +26,34 @@
         'this can mean a faster simulation on machines with several CPUs. However ,'
         'If the number is too low, the overhad of splitting the grid will not be worth '
         'the time gained through parallelization. (Default: 200).',
         default=200,
         platform=['grasshopper']
     )
 ]
+
+
+"""Alias for inputs that set the minimum number of sensors in split sensor grids."""
+min_sensor_count_input = [
+    InputAlias.int(
+        name='min_sen_count',
+        description='Positive integer for the minimum number of sensors in each '
+        'grid after redistributing the sensors based on cpu_count. This value takes '
+        'precedence over the cpu_count and can be used to ensure that the '
+        'parallelization does not result in generating unnecessarily small '
+        'sensor grids that increase overhead. (Default: 200).',
+        default=200,
+        platform=['grasshopper']
+    )
+]
+
+
+"""Alias for inputs that set the CPU count by splittin sensor grids."""
+cpu_count = Inputs.int(
+    default=50,
+    description='The maximum number of CPUs for parallel execution. For local '
+    'simulation, this value is ignored and the cpu_count is automatically set to '
+    'be equal to the number of workers tasked to the run. For cloud-based runs, '
+    'this input can be used to control the resources used for the simulation and, '
+    'if unspecified, the default value of 50 will be used.',
+    spec={'type': 'integer', 'minimum': 1}
+)
```

### Comparing `pollination-alias-0.9.8/pollination/alias/inputs/model.py` & `pollination-alias-0.9.9/pollination/alias/inputs/model.py`

 * *Files identical despite different names*

### Comparing `pollination-alias-0.9.8/pollination/alias/inputs/north.py` & `pollination-alias-0.9.9/pollination/alias/inputs/north.py`

 * *Files identical despite different names*

### Comparing `pollination-alias-0.9.8/pollination/alias/inputs/pit.py` & `pollination-alias-0.9.9/pollination/alias/inputs/pit.py`

 * *Files identical despite different names*

### Comparing `pollination-alias-0.9.8/pollination/alias/inputs/radiancepar.py` & `pollination-alias-0.9.9/pollination/alias/inputs/radiancepar.py`

 * *Files identical despite different names*

### Comparing `pollination-alias-0.9.8/pollination/alias/inputs/runperiod.py` & `pollination-alias-0.9.9/pollination/alias/inputs/runperiod.py`

 * *Files identical despite different names*

### Comparing `pollination-alias-0.9.8/pollination/alias/inputs/schedule.py` & `pollination-alias-0.9.9/pollination/alias/inputs/schedule.py`

 * *Files identical despite different names*

### Comparing `pollination-alias-0.9.8/pollination/alias/inputs/simulation.py` & `pollination-alias-0.9.9/pollination/alias/inputs/simulation.py`

 * *Files identical despite different names*

### Comparing `pollination-alias-0.9.8/pollination/alias/inputs/wea.py` & `pollination-alias-0.9.9/pollination/alias/inputs/wea.py`

 * *Files identical despite different names*

### Comparing `pollination-alias-0.9.8/pollination/alias/outputs/comfort.py` & `pollination-alias-0.9.9/pollination/alias/outputs/comfort.py`

 * *Files identical despite different names*

### Comparing `pollination-alias-0.9.8/pollination/alias/outputs/daylight.py` & `pollination-alias-0.9.9/pollination/alias/outputs/daylight.py`

 * *Files identical despite different names*

### Comparing `pollination-alias-0.9.8/pollination/alias/outputs/eui.py` & `pollination-alias-0.9.9/pollination/alias/outputs/eui.py`

 * *Files identical despite different names*

### Comparing `pollination-alias-0.9.8/pollination_alias.egg-info/PKG-INFO` & `pollination-alias-0.9.9/pollination_alias.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-alias
-Version: 0.9.8
+Version: 0.9.9
 Summary: Collection of alias inputs and outputs for Pollination recipes.
 Home-page: https://github.com/pollination/pollination-alias
 Author: Pollination
 Author-email: info@pollination.cloud
 License: Apache-2.0 License
 Description: # pollination-alias
         A collection of input and output aliases for Pollination Recipe's inputs and outputs.
```

### Comparing `pollination-alias-0.9.8/pollination_alias.egg-info/SOURCES.txt` & `pollination-alias-0.9.9/pollination_alias.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-alias-0.9.8/setup.py` & `pollination-alias-0.9.9/setup.py`

 * *Files identical despite different names*

