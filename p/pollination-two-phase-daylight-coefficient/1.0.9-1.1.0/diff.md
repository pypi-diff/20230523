# Comparing `tmp/pollination-two-phase-daylight-coefficient-1.0.9.tar.gz` & `tmp/pollination-two-phase-daylight-coefficient-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-two-phase-daylight-coefficient-1.0.9.tar", last modified: Tue Nov  8 11:09:17 2022, max compression
+gzip compressed data, was "dist/pollination-two-phase-daylight-coefficient-1.1.0.tar", last modified: Tue May 23 18:16:25 2023, max compression
```

## Comparing `pollination-two-phase-daylight-coefficient-1.0.9.tar` & `pollination-two-phase-daylight-coefficient-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3426 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (121)     5748 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      940 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4299 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/_prepare_folder.py
--rw-r--r--   0 runner    (1001) docker     (121)     6344 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/two_phase/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/two_phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4596 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/two_phase/_raytracing.py
--rw-r--r--   0 runner    (1001) docker     (121)     5269 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/two_phase/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination_two_phase_daylight_coefficient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      940 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination_two_phase_daylight_coefficient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination_two_phase_daylight_coefficient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination_two_phase_daylight_coefficient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 11:08:27.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination_two_phase_daylight_coefficient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination_two_phase_daylight_coefficient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination_two_phase_daylight_coefficient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/tests/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/_prepare_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/two_phase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/two_phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/two_phase/_raytracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/two_phase/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination_two_phase_daylight_coefficient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination_two_phase_daylight_coefficient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination_two_phase_daylight_coefficient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination_two_phase_daylight_coefficient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:15:37.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination_two_phase_daylight_coefficient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination_two_phase_daylight_coefficient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination_two_phase_daylight_coefficient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/tests/validation_test.py
```

### Comparing `pollination-two-phase-daylight-coefficient-1.0.9/.github/workflows/ci.yaml` & `pollination-two-phase-daylight-coefficient-1.1.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.0.9/.github/workflows/tests.yaml` & `pollination-two-phase-daylight-coefficient-1.1.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.0.9/LICENSE` & `pollination-two-phase-daylight-coefficient-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.0.9/PKG-INFO` & `pollination-two-phase-daylight-coefficient-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pollination-two-phase-daylight-coefficient
-Version: 1.0.9
+Version: 1.1.0
 Summary: Two phase daylight coefficient recipe for Pollination.
 Home-page: https://github.com/pollination/two-phase-daylight-coefficient
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mikkel, ladybug-tools
 Maintainer-email: mikkel@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
 Project-URL: icon, https://raw.githubusercontent.com/ladybug-tools/artwork/master/icons_components/honeybee/png/annualrecipe.png
 Project-URL: docker, https://hub.docker.com/r/ladybugtools/honeybee-radiance
-Description: # two-phase-daylight-coefficient
-        Two phase daylight coefficient recipe for Pollination
-        
 Keywords: honeybee,radiance,ladybug-tools,daylight,annual-daylight
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# two-phase-daylight-coefficient
+
+Two phase daylight coefficient recipe for Pollination. It is unlikely that you may want to use this recipe directly.
```

### Comparing `pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/entry.py` & `pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/entry.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from dataclasses import dataclass
 from pollination_dsl.dag import Inputs, DAG, task, Outputs
-from pollination.honeybee_radiance.multiphase import PrepareMultiphase
 
 # input/output alias
 from pollination.alias.inputs.model import hbjson_model_grid_input
 from pollination.alias.inputs.wea import wea_input_timestep_check
 from pollination.alias.inputs.north import north_input
 from pollination.alias.inputs.radiancepar import rad_par_annual_input
 from pollination.alias.inputs.grid import grid_filter_input, \
@@ -72,88 +71,62 @@
         description='Wea file.',
         extensions=['wea'],
         alias=wea_input_timestep_check
     )
 
     @task(template=TwoPhasePrepareFolder)
     def prepare_folder_annual_daylight(
-        self, north=north, grid_filter=grid_filter, model=model, wea=wea
+        self, north=north, cpu_count=cpu_count, min_sensor_count=min_sensor_count,
+        grid_filter=grid_filter, model=model, wea=wea
         ):
         return [
             {
                 'from': TwoPhasePrepareFolder()._outputs.model_folder,
                 'to': 'model'
             },
             {
                 'from': TwoPhasePrepareFolder()._outputs.resources,
                 'to': 'resources'
             },
             {
                 'from': TwoPhasePrepareFolder()._outputs.results,
                 'to': 'results'
-            }
-        ]
-
-    @task(
-        template=PrepareMultiphase,
-        needs=[prepare_folder_annual_daylight],
-        sub_paths={
-            'sunpath': 'sunpath.mtx'
-        }
-    )
-    def prepare_multiphase(
-        self, model=prepare_folder_annual_daylight._outputs.model_folder,
-        sunpath=prepare_folder_annual_daylight._outputs.resources, phase=2,
-        cpu_count=cpu_count, cpus_per_grid=3,
-        min_sensor_count=min_sensor_count, static='include'
-    ):
-        return [
-            {
-                'from': PrepareMultiphase()._outputs.scene_folder,
-                'to': 'resources/dynamic/octree'
             },
             {
-                'from': PrepareMultiphase()._outputs.grid_folder,
-                'to': 'resources/dynamic/grid'
-            },
-            {
-                'from': PrepareMultiphase()._outputs.two_phase_info
-            },
-            {   'from': PrepareMultiphase()._outputs.grid_states_file,
-                'to': 'results/grid_states.json'
+                'from': TwoPhasePrepareFolder()._outputs.two_phase_info
             }
         ]
 
     @task(
         template=TwoPhaseSimulation,
-        loop=prepare_multiphase._outputs.two_phase_info,
-        needs=[prepare_folder_annual_daylight, prepare_multiphase],
+        loop=prepare_folder_annual_daylight._outputs.two_phase_info,
+        needs=[prepare_folder_annual_daylight],
         sub_folder='calcs/2_phase/{{item.identifier}}',
         sub_paths={
-            'octree_file': '{{item.octree}}',
-            'octree_file_direct': '{{item.octree_direct}}',
-            'octree_file_with_suns': '{{item.octree_direct_sun}}',
-            'sensor_grids_folder': '{{item.sensor_grids_folder}}',
+            'octree_file': 'dynamic/octree/{{item.octree}}',
+            'octree_file_direct': 'dynamic/octree/{{item.octree_direct}}',
+            'octree_file_with_suns': 'dynamic/octree/{{item.octree_direct_sun}}',
+            'sensor_grids_folder': 'dynamic/grid/{{item.sensor_grids_folder}}',
             'sky_dome': 'sky.dome',
             'total_sky': 'sky.mtx',
             'direct_sky': 'sky_direct.mtx',
             'sun_modifiers': 'suns.mod',
             'bsdf_folder': 'bsdf'
         }
     )
     def calculate_two_phase_matrix(
         self,
         identifier='{{item.identifier}}',
         light_path='{{item.light_path}}',
         radiance_parameters=radiance_parameters,
         sensor_grids_info='{{item.sensor_grids_info}}',
-        sensor_grids_folder=prepare_multiphase._outputs.grid_folder,
-        octree_file=prepare_multiphase._outputs.scene_folder,
-        octree_file_direct=prepare_multiphase._outputs.scene_folder,
-        octree_file_with_suns=prepare_multiphase._outputs.scene_folder,
+        sensor_grids_folder=prepare_folder_annual_daylight._outputs.resources,
+        octree_file=prepare_folder_annual_daylight._outputs.resources,
+        octree_file_direct=prepare_folder_annual_daylight._outputs.resources,
+        octree_file_with_suns=prepare_folder_annual_daylight._outputs.resources,
         sky_dome=prepare_folder_annual_daylight._outputs.resources,
         total_sky=prepare_folder_annual_daylight._outputs.resources,
         direct_sky=prepare_folder_annual_daylight._outputs.resources,
         sun_modifiers=prepare_folder_annual_daylight._outputs.resources,
         bsdf_folder=prepare_folder_annual_daylight._outputs.model_folder,
         results_folder='../../../results'
     ):
```

### Comparing `pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/two_phase/_raytracing.py` & `pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/two_phase/_raytracing.py`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/two_phase/entry.py` & `pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/two_phase/entry.py`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.0.9/pollination_two_phase_daylight_coefficient.egg-info/PKG-INFO` & `pollination-two-phase-daylight-coefficient-1.1.0/pollination_two_phase_daylight_coefficient.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pollination-two-phase-daylight-coefficient
-Version: 1.0.9
+Version: 1.1.0
 Summary: Two phase daylight coefficient recipe for Pollination.
 Home-page: https://github.com/pollination/two-phase-daylight-coefficient
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mikkel, ladybug-tools
 Maintainer-email: mikkel@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
 Project-URL: icon, https://raw.githubusercontent.com/ladybug-tools/artwork/master/icons_components/honeybee/png/annualrecipe.png
 Project-URL: docker, https://hub.docker.com/r/ladybugtools/honeybee-radiance
-Description: # two-phase-daylight-coefficient
-        Two phase daylight coefficient recipe for Pollination
-        
 Keywords: honeybee,radiance,ladybug-tools,daylight,annual-daylight
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# two-phase-daylight-coefficient
+
+Two phase daylight coefficient recipe for Pollination. It is unlikely that you may want to use this recipe directly.
```

### Comparing `pollination-two-phase-daylight-coefficient-1.0.9/pollination_two_phase_daylight_coefficient.egg-info/SOURCES.txt` & `pollination-two-phase-daylight-coefficient-1.1.0/pollination_two_phase_daylight_coefficient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.0.9/setup.py` & `pollination-two-phase-daylight-coefficient-1.1.0/setup.py`

 * *Files identical despite different names*

