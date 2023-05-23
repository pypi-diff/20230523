# Comparing `tmp/ecoengine-0.0.5.tar.gz` & `tmp/ecoengine-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoengine-0.0.5.tar", last modified: Tue May 16 20:16:06 2023, max compression
+gzip compressed data, was "ecoengine-0.0.6.tar", last modified: Tue May 23 19:02:04 2023, max compression
```

## Comparing `ecoengine-0.0.5.tar` & `ecoengine-0.0.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:16:06.776467 ecoengine-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-16 20:15:31.000000 ecoengine-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-16 20:16:06.776467 ecoengine-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-16 20:15:31.000000 ecoengine-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 20:15:31.000000 ecoengine-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-16 20:16:06.776467 ecoengine-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 20:15:31.000000 ecoengine-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:16:06.768467 ecoengine-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:16:06.772467 ecoengine-0.0.5/src/ecoengine/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:16:06.772467 ecoengine-0.0.5/src/ecoengine/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/constants/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:16:06.772467 ecoengine-0.0.5/src/ecoengine/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:16:06.772467 ecoengine-0.0.5/src/ecoengine/data/load_shapes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/apartment.json
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/elementary_school.json
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/food_service_a.json
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/food_service_b.json
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/junior_high.json
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/mens_dorm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/motel.json
--rw-r--r--   0 runner    (1001) docker     (123)    47218 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/multi_family.json
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/nursing_home.json
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/office_building.json
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/senior_high.json
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/womens_dorm.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:16:06.772467 ecoengine-0.0.5/src/ecoengine/engine/
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/engine/BuildingCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/engine/EcosizerEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/engine/SystemCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:16:06.772467 ecoengine-0.0.5/src/ecoengine/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/objects/Building.py
--rw-r--r--   0 runner    (1001) docker     (123)    23658 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/objects/SystemConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/objects/systemConfigUtils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:16:06.772467 ecoengine-0.0.5/src/ecoengine/objects/systems/
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/objects/systems/ParallelLoopTank.py
--rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/objects/systems/SwingTank.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/objects/systems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:16:06.772467 ecoengine-0.0.5/src/ecoengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-16 20:16:06.000000 ecoengine-0.0.5/src/ecoengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-16 20:16:06.000000 ecoengine-0.0.5/src/ecoengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:16:06.000000 ecoengine-0.0.5/src/ecoengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-16 20:16:06.000000 ecoengine-0.0.5/src/ecoengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 20:16:06.000000 ecoengine-0.0.5/src/ecoengine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:02:04.918220 ecoengine-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 19:01:31.000000 ecoengine-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-23 19:02:04.918220 ecoengine-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-23 19:01:31.000000 ecoengine-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 19:01:31.000000 ecoengine-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-23 19:02:04.918220 ecoengine-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 19:01:31.000000 ecoengine-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:02:04.914220 ecoengine-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:02:04.914220 ecoengine-0.0.6/src/ecoengine/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:02:04.914220 ecoengine-0.0.6/src/ecoengine/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/constants/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:02:04.914220 ecoengine-0.0.6/src/ecoengine/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:02:04.918220 ecoengine-0.0.6/src/ecoengine/data/load_shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/apartment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/elementary_school.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/food_service_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/food_service_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/junior_high.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/mens_dorm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/motel.json
+-rw-r--r--   0 runner    (1001) docker     (123)    47218 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/multi_family.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/nursing_home.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/office_building.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/senior_high.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/womens_dorm.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:02:04.918220 ecoengine-0.0.6/src/ecoengine/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/engine/BuildingCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/engine/EcosizerEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/engine/SystemCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:02:04.918220 ecoengine-0.0.6/src/ecoengine/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/objects/Building.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36036 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/objects/SystemConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/objects/systemConfigUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:02:04.918220 ecoengine-0.0.6/src/ecoengine/objects/systems/
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/objects/systems/ParallelLoopTank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/objects/systems/SwingTank.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/objects/systems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:02:04.914220 ecoengine-0.0.6/src/ecoengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-23 19:02:04.000000 ecoengine-0.0.6/src/ecoengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-23 19:02:04.000000 ecoengine-0.0.6/src/ecoengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 19:02:04.000000 ecoengine-0.0.6/src/ecoengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-23 19:02:04.000000 ecoengine-0.0.6/src/ecoengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 19:02:04.000000 ecoengine-0.0.6/src/ecoengine.egg-info/top_level.txt
```

### Comparing `ecoengine-0.0.5/PKG-INFO` & `ecoengine-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoengine
-Version: 0.0.5
+Version: 0.0.6
 Summary: A software for sizing Heat Pump Water Heaters for buildings
 Home-page: https://ecosizer.ecotope.com/sizer/
 Author: Nolan
 Author-email: nolan@ecotope.com
 Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecoengine-0.0.5/README.md` & `ecoengine-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.5/setup.cfg` & `ecoengine-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ecoengine
-version = 0.0.5
+version = 0.0.6
 author = Nolan
 author_email = nolan@ecotope.com
 description = A software for sizing Heat Pump Water Heaters for buildings
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://ecosizer.ecotope.com/sizer/
 project_urls =
```

### Comparing `ecoengine-0.0.5/src/ecoengine/__init__.py` & `ecoengine-0.0.6/src/ecoengine/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.5/src/ecoengine/data/load_shapes/apartment.json` & `ecoengine-0.0.6/src/ecoengine/data/load_shapes/apartment.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.5/src/ecoengine/data/load_shapes/elementary_school.json` & `ecoengine-0.0.6/src/ecoengine/data/load_shapes/elementary_school.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.5/src/ecoengine/data/load_shapes/food_service_a.json` & `ecoengine-0.0.6/src/ecoengine/data/load_shapes/food_service_a.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.5/src/ecoengine/data/load_shapes/food_service_b.json` & `ecoengine-0.0.6/src/ecoengine/data/load_shapes/food_service_b.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.5/src/ecoengine/data/load_shapes/junior_high.json` & `ecoengine-0.0.6/src/ecoengine/data/load_shapes/junior_high.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.5/src/ecoengine/data/load_shapes/mens_dorm.json` & `ecoengine-0.0.6/src/ecoengine/data/load_shapes/mens_dorm.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.5/src/ecoengine/data/load_shapes/motel.json` & `ecoengine-0.0.6/src/ecoengine/data/load_shapes/motel.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.5/src/ecoengine/data/load_shapes/multi_family.json` & `ecoengine-0.0.6/src/ecoengine/data/load_shapes/multi_family.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.5/src/ecoengine/data/load_shapes/nursing_home.json` & `ecoengine-0.0.6/src/ecoengine/data/load_shapes/nursing_home.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.5/src/ecoengine/data/load_shapes/office_building.json` & `ecoengine-0.0.6/src/ecoengine/data/load_shapes/office_building.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.5/src/ecoengine/data/load_shapes/senior_high.json` & `ecoengine-0.0.6/src/ecoengine/data/load_shapes/senior_high.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.5/src/ecoengine/data/load_shapes/womens_dorm.json` & `ecoengine-0.0.6/src/ecoengine/data/load_shapes/womens_dorm.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.5/src/ecoengine/engine/BuildingCreator.py` & `ecoengine-0.0.6/src/ecoengine/engine/BuildingCreator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.5/src/ecoengine/engine/EcosizerEngine.py` & `ecoengine-0.0.6/src/ecoengine/engine/EcosizerEngine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 from .BuildingCreator import *
 from .SystemCreator import *
 
 print("EcosizerEngine Copyright (C) 2023  Ecotope Inc.")
 print("This program comes with ABSOLUTELY NO WARRANTY. This is free software, and you are welcome to redistribute under certain conditions; details check GNU AFFERO GENERAL PUBLIC LICENSE_08102020.docx.")
 
 class EcosizerEngine:
-
     """
     Initializes and sizes the HPWH system for a building based on the given parameters.
 
     Attributes
     ----------
     incomingT_F : float 
         The incoming city water temperature on the design day. [°F]
-    magnitudeStat : int or list
+    magnitude_stat : int or list
         a number that will be used to assess the magnitude of the building based on the building type
     supplyT_F : float
         The hot water supply temperature.[°F]
     storageT_F : float 
         The hot water storage temperature. [°F]
     percentUseable : float
         The fraction of the storage volume that can be filled with hot water.
     aquaFract: float
-        The fraction of the total hieght of the primary hot water tanks at which the Aquastat is located.
+        The fraction of the total height of the primary hot water tanks at which the Aquastat is located.
     schematic : String
         Indicates schematic type. Valid values are 'swingtank', 'paralleltank', and 'primary'
-    buildingType : string or list
+    building_type : string or list
         a string indicating the type of building we are sizing for (e.g. "multi_family", "office_building", etc.)
     loadShape : ndarray
         defaults to design load shape for building type.
     avgLoadShape : ndarray
         defaults to average load shape for building type.
     loadShiftSchedule : array_like
-        List or array of 0's and 1's for don't run and run respectively. Used for load shifting
+        List or array of 0's, 1's used for load shifting, 0 indicates system is off. 
+    loadUpHours : float
+        Number of hours spent loading up for first shed.
+    aquaFractLoadUp : float
+        The fraction of the total height of the primary hot water tanks at which the load up aquastat is located.
+    aquaFractShed : float
+        The fraction of the total height of the primary hot water tanks at which the shed aquastat is located.
+    loadUpT_F : float
+        The hot water storage temperature between the normal and load up aquastat. [°F]
     loadShiftPercent: float
         Percentage of days the load shift will be met
     returnT_F : float 
         The water temperature returning from the recirculation loop. [°F]
-    flowRate : float 
+    flow_rate : float 
         The pump flow rate of the recirculation loop. (GPM)
     gpdpp : float
         The volume of water in gallons at 120F each person uses per dat.[°F]
     nBR : array_like
         A list of the number of units by size in the order 0 bedroom units,
         1 bedroom units, 2 bedroom units, 3 bedroom units, 4 bedroom units,
         5 bedroom units.
@@ -59,54 +66,58 @@
         Set to true if doing loadshift
     setpointTM_F : float
         The setpoint of the temprature maintence tank. Defaults to 130 °F.
     TMonTemp_F : float
         The temperature where parallel loop tank will turn on.
         Defaults to 120 °F.
     offTime_hr: integer
-        Maximum hours per day the temperature maintenance equipment can run
-    standardGPD : string
-        indicates whether to use a standard gpdpp specification for multi-family buildings. Set to None if not using a standard gpdpp.
+        Maximum hours per day the temperature maintenance equipment can run.
+
     """
 
-    def __init__(self, incomingT_F, magnitudeStat, supplyT_F, storageT_F, percentUseable, aquaFract, 
-                            schematic, buildingType, loadshape = None, avgLoadshape = None, loadShiftSchedule = None, loadShiftPercent = 1,
+    def __init__(self, incomingT_F, magnitudeStat, supplyT_F, storageT_F, percentUseable, aquaFract,
+                            schematic, buildingType, loadshape = None, avgLoadshape = None, loadShiftSchedule = None, loadUpHours = None,
+                            aquaFractLoadUp = None, aquaFractShed = None, loadUpT_F = None, loadShiftPercent = 1,
                             returnT_F = 0, flowRate = 0, gpdpp = 0, nBR = None, safetyTM = 1.75,
                             defrostFactor = 1, compRuntime_hr = 16, nApt = 0, Wapt = 0, doLoadShift = False,
                             setpointTM_F = 135, TMonTemp_F = 120, offTime_hr = 0.333, standardGPD = None):
         
-        building = createBuilding(  incomingT_F     = incomingT_F,
-                                    magnitudeStat   = magnitudeStat, 
+        building = createBuilding( incomingT_F     = incomingT_F,
+                                    magnitudeStat  = magnitudeStat, 
                                     supplyT_F       = supplyT_F, 
-                                    buildingType    = buildingType,
+                                    buildingType   = buildingType,
                                     loadshape       = loadshape,
                                     avgLoadshape    = avgLoadshape,
                                     returnT_F       = returnT_F, 
                                     flowRate       = flowRate,
                                     gpdpp           = gpdpp,
                                     nBR             = nBR,
                                     nApt            = nApt,
                                     Wapt            = Wapt,
-                                    standardGPD     = standardGPD
+                                    standardGPD = standardGPD
         )
 
         system = createSystem(  schematic, 
                                 building, 
                                 storageT_F, 
                                 defrostFactor, 
                                 percentUseable, 
                                 compRuntime_hr, 
                                 aquaFract, 
-                                doLoadShift         = doLoadShift, 
-                                loadShiftPercent    = loadShiftPercent, 
-                                loadShiftSchedule   = loadShiftSchedule, 
-                                safetyTM            = safetyTM, 
-                                setpointTM_F        = setpointTM_F, 
-                                TMonTemp_F          = TMonTemp_F, 
-                                offTime_hr          = offTime_hr
+                                aquaFractLoadUp = aquaFractLoadUp,
+                                aquaFractShed = aquaFractShed,
+                                loadUpT_F = loadUpT_F,
+                                doLoadShift = doLoadShift, 
+                                loadShiftPercent = loadShiftPercent, 
+                                loadShiftSchedule = loadShiftSchedule, 
+                                loadUpHours = loadUpHours,
+                                safetyTM = safetyTM, 
+                                setpointTM_F = setpointTM_F, 
+                                TMonTemp_F = TMonTemp_F, 
+                                offTime_hr = offTime_hr
         )
  
         self.system = system
     
     def getSizingResults(self):
         """
         Returns the minimum primary volume and heating capacity sizing results
@@ -124,15 +135,15 @@
         fraction is too small for system and cuts the return arrays to match cutoff point.
 
         Returns
         -------
         volN : array
             Array of volume in the tank at each hour.
 
-        primaryHeatHrs2kBTUHR : array
+        sHrs2kBTUHR : array
             Array of heating capacity in kBTU/hr
             
         heatHours : array
             Array of running hours per day corresponding to primaryHeatHrs2kBTUHR
             
         recIndex : int
             The index of the recommended heating rate. 
@@ -152,14 +163,30 @@
         Returns
         -------
         div/fig
             plot_div
         """
         return self.system.plotStorageLoadSim(return_as_div)
     
+    def lsSizedPoints(self):
+        """
+        Returns combinations of storage and capacity based on number of 
+        load up hours
+
+        Returns 
+        -------
+        volN : array
+            Array of storage volume for each number of load up hours.
+        CapN : array
+            Array of heating capacity for each number of load up hours.
+        N : array
+            Array of load up hours tested. Goes from 1 to hour before first shed.
+        """
+        return self.system.lsSizedPoints()
+
     def getHWMagnitude(self):
         """
         Returns the total daily hot water for the building the HPWH is being sized for.
         
         Returns
         -------
         magnitude : Float
```

### Comparing `ecoengine-0.0.5/src/ecoengine/engine/SystemCreator.py` & `ecoengine-0.0.6/src/ecoengine/engine/SystemCreator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from ecoengine.objects.SystemConfig import *
 from ecoengine.objects.systems.SwingTank import *
 from ecoengine.objects.systems.ParallelLoopTank import *
 
 def createSystem(schematic, building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, doLoadShift = False, 
-                 loadShiftPercent = 1, loadShiftSchedule = None, safetyTM = 1.75, setpointTM_F = 135, TMonTemp_F = 120, offTime_hr = 0.333):
+                 aquaFractLoadUp = None, aquaFractShed = None, loadUpT_F = None, loadShiftPercent = 1, loadShiftSchedule = None, loadUpHours = None, safetyTM = 1.75, 
+                 setpointTM_F = 135, TMonTemp_F = 120, offTime_hr = 0.333):
+
     """
     Initializes and sizes the HPWH system. Both primary and tempurature maintenance (for parrallel loop and swing tank) are set up in this function.
 
     Attributes
     ----------
     schematic : String
         Indicates schematic type. Valid values are 'swingtank', 'paralleltank', and 'primary'
@@ -18,21 +20,29 @@
     defrostFactor : float 
         A multipier used to account for defrost in the final heating capacity. Default equals 1.
     percentUseable : float
         The fraction of the storage volume that can be filled with hot water.
     compRuntime_hr : float
         The number of hours the compressor will run on the design day. [Hr]
     aquaFract: float
-        The fraction of the total hieght of the primary hot water tanks at which the Aquastat is located.
+        The fraction of the total height of the primary hot water tanks at which the Aquastat is located.
     doLoadShift : boolean
         Set to true if doing loadshift
+    aquaFractLoadUp : float
+        The fraction of the total height of the primary hot water tanks at which the load up aquastat is located.
+    aquaFractShed : float
+        The fraction of the total height of the primary hot water tanks at which the shed aquastat is located.
+    loadUpT_F : float
+        The hot water storage temperature between the normal and load up aquastat. [°F]
     loadShiftPercent: float
         Percentage of days the load shift will be met
     loadShiftSchedule : array_like
-        List or array of 0's and 1's for don't run and run respectively. Used for load shifting
+        List or array of 0's and 1's for don't run and run respectively. Used for load shifting 
+    loadUpHours : float
+        Number of hours spent loading up for first shed.
     safetyTM : float
         The saftey factor for the temperature maintenance system.
     setpointTM_F : float
         The setpoint of the temprature maintence tank. Defaults to 130 °F.
     TMonTemp_F : float
         The temperature where parallel loop tank will turn on.
         Defaults to 120 °F.
@@ -44,16 +54,17 @@
     Exception: Error if schematic is not in list of valid schematic names.
 
     """
     
     match schematic:
         case 'swingtank':
             return SwingTank(safetyTM, building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, 
-                             doLoadShift, loadShiftPercent, loadShiftSchedule)        
+                             doLoadShift, loadShiftPercent, loadShiftSchedule, loadUpHours, aquaFractLoadUp, aquaFractShed, loadUpT_F)        
         case 'paralleltank':
             return ParallelLoopTank(safetyTM, setpointTM_F, TMonTemp_F, offTime_hr, building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, 
-                 doLoadShift, loadShiftPercent, loadShiftSchedule)
+                 doLoadShift, loadShiftPercent, loadShiftSchedule, loadUpHours, aquaFractLoadUp, aquaFractShed, loadUpT_F)
         case 'primary':
-            return Primary(building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, doLoadShift, loadShiftPercent, loadShiftSchedule)
+            return Primary(building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, doLoadShift, loadShiftPercent, loadShiftSchedule, loadUpHours,
+                           aquaFractLoadUp, aquaFractShed, loadUpT_F)
         case _:
             raise Exception("Unknown system schematic type.")
```

### Comparing `ecoengine-0.0.5/src/ecoengine/engine/__init__.py` & `ecoengine-0.0.6/src/ecoengine/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.5/src/ecoengine/objects/Building.py` & `ecoengine-0.0.6/src/ecoengine/objects/Building.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.5/src/ecoengine/objects/SystemConfig.py` & `ecoengine-0.0.6/src/ecoengine/objects/SystemConfig.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,58 +4,59 @@
 from scipy.stats import norm #lognorm
 from plotly.graph_objs import Figure, Scatter
 from plotly.offline import plot
 from .systemConfigUtils import roundList, mixVolume, hrToMinList, getPeakIndices, checkLiqudWater, checkHeatHours
 
 class SystemConfig:
     def __init__(self, building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, 
-                 doLoadShift = False, loadShiftPercent = 1, loadShiftSchedule = None):
-        # check inputs. LoadShiftSchedule not checked because it is checked elsewhere
+                 doLoadShift = False, loadShiftPercent = 1, loadShiftSchedule = None, loadUpHours = None, aquaFractLoadUp = None, 
+                 aquaFractShed = None, loadUpT_F = None):
+        # check inputs. Schedule not checked because it is checked elsewhere
         self._checkInputs(building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, doLoadShift, loadShiftPercent)
-        
         self.doLoadShift = doLoadShift
         self.building = building        
-        # self.totalHWLoad = self.building.magnitude
         self.storageT_F = storageT_F
         self.defrostFactor = defrostFactor
         self.percentUseable = percentUseable
         self.compRuntime_hr = compRuntime_hr
         self.aquaFract = aquaFract
+        self.loadUpHours = None
 
         if doLoadShift and not loadShiftSchedule is None:
-            self._setLoadShift(loadShiftSchedule, loadShiftPercent)
+            self._setLoadShift(loadShiftSchedule, loadUpHours, aquaFract, aquaFractLoadUp, aquaFractShed, storageT_F, loadUpT_F, loadShiftPercent)
+        
         else:
             self.loadShiftSchedule = [1] * 24
             self.fract_total_vol = 1 # fraction of total volume for for load shifting, or 1 if no load shifting
 
         #Check if need to increase sizing to meet lower runtimes for load shift
         self.maxDayRun_hr = min(self.compRuntime_hr, sum(self.loadShiftSchedule))
 
         #size system
-        self.PVol_G_atStorageT, self.effSwingFract = self.sizePrimaryTankVolume(self.maxDayRun_hr)
-        self.PCap_kBTUhr = self._primaryHeatHrs2kBTUHR(self.maxDayRun_hr, self.effSwingFract )
+        self.PVol_G_atStorageT, self.effSwingFract = self.sizePrimaryTankVolume(self.maxDayRun_hr, self.loadUpHours)
+        self.PCap_kBTUhr = self._primaryHeatHrs2kBTUHR(heathours = self.maxDayRun_hr, loadUpHours = self.loadUpHours, effSwingVolFract = self.effSwingFract, primaryCurve = False)[0]
 
     def _checkInputs(self, building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, doLoadShift, loadShiftPercent):
         if not isinstance(building, Building):
             raise Exception("Error: Building is not valid.")
-        if not (isinstance(storageT_F, int) or isinstance(storageT_F, float)) or not checkLiqudWater(storageT_F):
+        if not (isinstance(storageT_F, int) or isinstance(storageT_F, float)) or not checkLiqudWater(storageT_F): 
             raise Exception('Invalid input given for Storage temp, it must be between 32 and 212F.')
         if not (isinstance(defrostFactor, int) or isinstance(defrostFactor, float)) or defrostFactor < 0 or defrostFactor > 1:
             raise Exception("Invalid input given for Defrost Factor, must be a number between 0 and 1.")
         if not (isinstance(percentUseable, int) or isinstance(percentUseable, float)) or percentUseable > 1 or percentUseable < 0:
             raise Exception("Invalid input given for percentUseable, must be a number between 0 and 1.")
         if not isinstance(compRuntime_hr, int) or compRuntime_hr <= 0 or compRuntime_hr > 24:
             raise Exception("Invalid input given for compRuntime_hr, must be an integer between 0 and 24.")
         if not (isinstance(aquaFract, int) or isinstance(aquaFract, float)) or aquaFract > 1 or aquaFract <= 0:
             raise Exception("Invalid input given for aquaFract must, be a number between 0 and 1.")
         if not (isinstance(loadShiftPercent, int) or isinstance(loadShiftPercent, float)) or loadShiftPercent > 1 or loadShiftPercent < 0:
             raise Exception("Invalid input given for loadShiftPercent, must be a number between 0 and 1.")
         if not isinstance(doLoadShift, bool):
             raise Exception("Invalid input given for doLoadShift, must be a boolean.")
-
+              
     def getSizingResults(self):
         """
         Returns the minimum primary volume and heating capacity sizing results. Implimented seperatly in Temp Maintenence systems.
 
         Returns
         -------
         list
@@ -89,28 +90,31 @@
         D_hw : list 
             The hot water demand with time at the tsupply temperature
         prun : list 
             The actual output in gallons of the HPWH with time
         """
 
         G_hw, D_hw, V0, Vtrig, pV, pheating = self._getInitialSimulationValues(Pcapacity, Pvolume)
-
+       
         hw_outSwing = [0] * (len(G_hw))
         hw_outSwing[0] = D_hw[0]
         prun = [0] * (len(G_hw))
 
         if initPV:
             pV[0] = initPV
 
+        #get mixed storage temp
+        mixedStorT_F = self._mixStorageTemps(pV[0])[0]
+
         # Run the "simulation"
         for i in range(1, len(G_hw)):
-            mixedDHW = mixVolume(D_hw[i], self.storageT_F, self.building.incomingT_F, self.building.supplyT_F)
-            mixedGHW = mixVolume(G_hw[i], self.storageT_F, self.building.incomingT_F, self.building.supplyT_F)
-            pheating, pV[i], prun[i] = self.runOnePrimaryStep(pheating, V0, Vtrig, pV[i-1], mixedDHW, mixedGHW)
-
+            mixedDHW = mixVolume(D_hw[i], mixedStorT_F, self.building.incomingT_F, self.building.supplyT_F) 
+            mixedGHW = mixVolume(G_hw[i], mixedStorT_F, self.building.incomingT_F, self.building.supplyT_F)
+            pheating, pV[i], prun[i] = self.runOnePrimaryStep(pheating, V0, Vtrig[i], pV[i-1], mixedDHW, mixedGHW) 
+            
         return [roundList(pV, 3),
                 roundList(G_hw, 3),
                 roundList(D_hw, 3),
                 roundList(prun, 3)]
 
     def _getInitialSimulationValues(self, Pcapacity=None, Pvolume=None):
         """
@@ -130,92 +134,140 @@
         list [ G_hw, D_hw, V0, V, run, pheating ]
         G_hw : list
             The generation of HW with time at the supply temperature
         D_hw : list
             The hot water demand with time at the tsupply temperature
         V0 : float
             The storage volume of the primary system at the storage temperature
-        Vtrig : float
+        Vtrig : list
             The remaining volume of the primary storage volume when heating is
-            triggered, note this equals V0*(1 - aquaFract) TODO is that true tho?
+            triggered, note this equals V0*(1 - aquaFract[i]) 
         pV : list 
-            Volume of HW in the tank with time at the strorage temperature. Initialized to array of 0s with pV[0] set to V0
+            Volume of HW in the tank with time at the storage temperature. Initialized to array of 0s with pV[0] set to V0
         pheating : boolean 
             set to false. Simulation starts with a full tank so primary heating starts off
         """
         if not Pcapacity:
             Pcapacity =  self.PCap_kBTUhr
 
         if not Pvolume:
             Pvolume =  self.PVol_G_atStorageT
-
+        
         loadShapeN = self.building.loadshape
         if self.doLoadShift:
             loadShapeN = self.building.avgLoadshape
-
+        
         # Get the generation rate from the primary capacity
         G_hw = 1000 * Pcapacity / rhoCp / (self.building.supplyT_F - self.building.incomingT_F) \
-               * self.defrostFactor * np.tile(self.loadShiftSchedule,3)
+               * self.defrostFactor * np.tile(self.loadShiftSchedule, 3)
+
         
         # Define the use of DHW with the normalized load shape
         D_hw = self.building.magnitude * self.fract_total_vol * np.tile(loadShapeN, 3)
 
+        # Init the "simulation"
+        V0 = np.ceil(Pvolume * self.percentUseable) 
+        
+        Vtrig = np.tile(np.ceil(Pvolume * (1 - self.aquaFract)) + 1, 24) # To prevent negatives with any of that rounding math. TODO Nolan and I don't think we need this mysterious + 1
+        
+        if self.doLoadShift:
+            
+            Vtrig = [Pvolume * (1 - self.aquaFractShed) if x == 0 else Pvolume * (1 - self.aquaFract) for x in self.loadShiftSchedule]
+            
+            #set load up hours pre-shed 1
+            shedHours = [i for i in range(len(self.loadShiftSchedule)) if self.loadShiftSchedule[i] == 0] 
+            Vtrig = [Pvolume * (1 - self.aquaFractLoadUp) if shedHours[0] - self.loadUpHours <= i <= shedHours[0] - 1 else Vtrig[i] for i, x in enumerate(Vtrig)]
+            
+            #check if there are two sheds, if so set all hours inbetween to load up
+            try:
+                secondShed = [[shedHours[i-1], shedHours[i]] for i in range(1, len(shedHours)) if shedHours[i] - shedHours[i-1] > 1][0]
+                Vtrig = [Pvolume * (1 - self.aquaFractLoadUp) if secondShed[0] <= i <= secondShed[1] - 1 else Vtrig[i] for i, x in enumerate(Vtrig)]
+            
+            except IndexError:
+                pass
+        
         # To per minute from per hour
         G_hw = np.array(hrToMinList(G_hw)) / 60
         D_hw = np.array(hrToMinList(D_hw)) / 60
+        Vtrig = np.array(hrToMinList(np.tile(Vtrig, 3))) 
 
-        # Init the "simulation"
-        V0 = np.ceil(Pvolume * self.percentUseable)
-        Vtrig = np.ceil(Pvolume * (1 - self.aquaFract)) + 1 # To prevent negatives with any of that rounding math. TODO Nolan is sus of that +1
         pV = [V0] + [0] * (len(G_hw) - 1)
 
         pheating = False
-
+    
         return G_hw, D_hw, V0, Vtrig, pV, pheating
     
-    def _setLoadShift(self, loadShiftSchedule, loadShiftPercent=1):
+    def _setLoadShift(self, loadShiftSchedule, loadUpHours, aquaFract, aquaFractLoadUp, aquaFractShed, storageT_F, loadUpT_F, loadShiftPercent=1):
         """
         Sets the load shifting schedule from input loadShiftSchedule
 
         Parameters
         ----------
         loadShiftSchedule : array_like
-            List or array of 0's and 1's for don't run and run.
-
+            List or array of 0's, 1's used for load shifting, 0 indicates system is off. 
+        loadUpHours : float
+            Number of hours spent loading up for first shed.
+        aquaFract: float
+            The fraction of the total height of the primary hot water tanks at which the Aquastat is located.
+        aquaFractLoadUp : float
+            The fraction of the total height of the primary hot water tanks at which the load up aquastat is located.
+        aquaFractShed : float
+            The fraction of the total height of the primary hot water tanks at which the shed aquastat is located.
+        storageT_F : float 
+            The hot water storage temperature. [°F]
+        loadUpT_F : float
+            The hot water storage temperature between the normal and load up aquastat. [°F]
         loadShiftPercent : float
             Percentile of days which need to be covered by load shifting
 
         """
         # Check
-        if len(loadShiftSchedule) != 24 : #TODO ensure loadShiftSchedule is valid and add load up
-            raise Exception("loadshift is not of length 24 but instead has length of "+str(len(loadShiftSchedule))+".")
+        if not(isinstance(loadShiftSchedule, list)):
+            raise Exception("Invalid input given for schedule, must be an array of length 24.")
+        if len(loadShiftSchedule) != 24: 
+            raise Exception("Load shift is not of length 24 but instead has length of "+str(len(loadShiftSchedule))+".")
+        if not all(i in [0,1] for i in loadShiftSchedule):
+            raise Exception("Loadshift schedule must be comprised of 0s, 1s, and 2s for shed, normal, and load up operation.")
         if sum(loadShiftSchedule) == 0 :
             raise Exception("When using Load shift the HPWH's must run for at least 1 hour each day.")
         if loadShiftPercent < 0.25 :
             raise Exception("Load shift only available for above 25 percent of days.")
         if loadShiftPercent > 1 :
             raise Exception("Cannot load shift for more than 100 percent of days")
+        if not (isinstance(aquaFractLoadUp, int) or isinstance(aquaFractLoadUp, float)) or aquaFractLoadUp > aquaFract or aquaFractLoadUp <= 0:
+            raise Exception("Invalid input given for load up aquastat fraction, must be a number between 0 and normal aquastat fraction.")
+        if not (isinstance(aquaFractShed, int) or isinstance(aquaFractShed, float)) or aquaFractShed >= 1 or aquaFractShed < aquaFract:
+            raise Exception("Invalid input given for shed aquastat fraction, must be a number between normal aquastat fraction and 1.")
+        if not (isinstance(loadUpT_F, int) or isinstance(loadUpT_F, float)) or loadUpT_F < storageT_F or not checkLiqudWater(loadUpT_F):
+            raise Exception("Invalid input given for load up storage temp, it must be a number between normal storage temp and 212F.")
+        if not (isinstance(loadUpHours, int)) or loadUpHours > loadShiftSchedule.index(0): #make sure there are not more load up hours than nhours before first shed
+            raise Exception("Invalid input given for load up hours, must be an integer less than or equal to hours in day before first shed period.") 
 
         self.loadShiftSchedule = loadShiftSchedule
-        self.loadshift = np.array(loadShiftSchedule, dtype = float)# Coerce to numpy array of data type float
-
-        # adjust for loadShiftPercent
+        self.loadUpHours = loadUpHours
+        self.aquaFractLoadUp = aquaFractLoadUp
+        self.aquaFractShed = aquaFractShed
+        self.loadUpT_F = loadUpT_F
+        self.loadshift = np.array(loadShiftSchedule, dtype = float) # Coerce to numpy array of data type float
+        
+        # adjust for cdf_shift
         if loadShiftPercent == 1: # meaing 100% of days covered by load shift
             self.fract_total_vol = 1
+            
         else:
             # calculate fraction total hot water required to meet load shift days
             fract = norm_mean + norm_std * norm.ppf(loadShiftPercent) #TODO norm_mean and std are currently from multi-family, need other types eventually. For now, loadshifting will only be available for multi-family
             self.fract_total_vol = fract if fract <= 1. else 1.
         
         self.doLoadShift = True
 
-    # SwingTank has it's own implimentation
-    def _primaryHeatHrs2kBTUHR(self, heathours, effSwingVolFract=1):
+    def _primaryHeatHrs2kBTUHR(self, heathours, loadUpHours, primaryCurve = False, effSwingVolFract=1):
         """
-        Converts from hours of heating in a day to heating capacity.
+        Converts from hours of heating in a day to heating capacity. If loadshifting compares this method to capacity needed to load up
+        and takes maximum.
 
         Implimented seperatly in Swing Tank systems
 
         Parameters
         ----------
         heathours : float or numpy.ndarray
             The number of hours primary heating equipment can run.
@@ -224,28 +276,50 @@
             The fractional adjustment to the total hot water load for the
             primary system. Only used in a swing tank system.
 
         Returns
         -------
         heatCap
             The heating capacity in [btu/hr].
+        genRate
+            The generation rate in [gal/hr] when the heat pump is on. 
+            If loadshifting this is the maximum between normal calculation
+            and what is necessary to complete first load up.
         """
         checkHeatHours(heathours)
-        heatCap = self.building.magnitude / heathours * rhoCp * \
-            (self.building.supplyT_F - self.building.incomingT_F) / self.defrostFactor /1000.
-        return heatCap
+        genRate = self.building.magnitude * effSwingVolFract / heathours
+        
+        if self.doLoadShift and not primaryCurve:
+            Vshift, VconsumedLU = self._calcPrelimVol(loadUpHours) 
+            Vload = Vshift * (self.aquaFract - self.aquaFractLoadUp) / (self.aquaFractShed - self.aquaFractLoadUp) #volume in 'load up' portion of tank
+            LUgenRate = (Vload + VconsumedLU) / loadUpHours #rate needed to load up tank and offset use during load up period
+            
+            #compare with original genRate
+            genRate = max(LUgenRate, genRate)
+            
+        heatCap = genRate * rhoCp * \
+            (self.building.supplyT_F - self.building.incomingT_F) / self.defrostFactor / 1000
+       
+        return heatCap, genRate
     
-    def sizePrimaryTankVolume(self, heatHrs):
+
+    def sizePrimaryTankVolume(self, heatHrs, loadUpHours, primaryCurve = False):
         """
-        Calculates the primary storage using the Ecotope sizing methodology
+        Calculates the primary storage using the Ecotope sizing methodology. Function is also used
+        to generate primary sizing curve, which creates a curve with no load shifting and points
+        with varying numbers of load up hours.
 
         Parameters
         ----------
         heatHrs : float
             The number of hours primary heating equipment can run in a day.
+        primaryCurve : 
+            Indicates that function is being called to generate the priamry
+            sizing curve. This overrides LS sizing and sizes with "normal"
+            sizing (default = False)
         
         Raises
         ------
         ValueError: aquastat fraction is too low.
         ValueError: The minimum aquastat fraction is greater than 1.
 
         Returns
@@ -253,48 +327,63 @@
         totalVolMax : float
             The total storage volume in gallons adjusted to the storage tempreature
         effMixFract : float
             The fractional adjustment to the total hot water load for the
             primary system. Only used in a swing tank system.
         
         """
+       
+
         if heatHrs <= 0 or heatHrs > 24:
             raise Exception("Heat hours is not within 1 - 24 hours")
         # Fraction used for adjusting swing tank volume.
         effMixFract = 1.
 
         # Running vol
         runningVol_G, effMixFract = self._calcRunningVol(heatHrs, np.ones(24), self.building.loadshape, effMixFract)
+        totalVolAtStorage = self._getTotalVolAtStorage(runningVol_G)
+        totalVolAtStorage *=  thermalStorageSF
 
-        # If doing load shift, solve for the runningVol_G and take the larger volume
-        if self.doLoadShift:
-            LSrunningVol_G = 0
-            LSeffMixFract = 0
-            # calculate loadshift sizing with avg loadshape (see page 19 of methodology documentation)
-            LSrunningVol_G, LSeffMixFract = self._calcRunningVol(heatHrs, self.loadShiftSchedule, self.building.avgLoadshape, LSeffMixFract)
-            LSrunningVol_G *= self.fract_total_vol
+        if self.doLoadShift and not primaryCurve:
+            LSrunningVol_G, LSeffMixFract = self._calcRunningVolLS(loadUpHours, effMixFract)
+            LSrunningVol_G *= self.fract_total_vol 
 
             # Get total volume from max of primary method or load shift method
             if LSrunningVol_G > runningVol_G:
                 runningVol_G = LSrunningVol_G
                 effMixFract = LSeffMixFract
+                
+                #get the average tank volume
+                totalVolAtStorage = self._mixStorageTemps(runningVol_G)[1]
+                
+                #multiply computed storage by efficiency safety factor (currently set to 1)
+                totalVolAtStorage *=  thermalStorageSF 
+        
+            # Check the Cycling Volume 
+            LUcyclingVol_G = totalVolAtStorage * (self.aquaFractLoadUp - (1 - self.percentUseable))
+            minRunVol_G = pCompMinimumRunTime * (self.building.magnitude / heatHrs) # (generation rate - no usage) #REMOVED EFFMIXFRACT
+            
+            if minRunVol_G > LUcyclingVol_G:
+                min_AF = minRunVol_G / totalVolAtStorage + (1 - self.percentUseable)
+                if min_AF < 1:
+                    raise ValueError("01", "The load up aquastat fraction is too low in the storge system recommend increasing the maximum run hours in the day or increasing to a minimum of: ", round(min_AF,3))
+                raise ValueError("02", "The minimum aquastat fraction is greater than 1. This is due to the storage efficency and/or the maximum run hours in the day may be too low. Try increasing these values, we reccomend 0.8 and 16 hours for these variables respectively." )
 
-        totalVolAtStorage = self._getTotalVolAtStorage(runningVol_G)
-
-        # Check the Cycling Volume ############################################
         cyclingVol_G = totalVolAtStorage * (self.aquaFract - (1 - self.percentUseable))
-        minRunVol_G = pCompMinimumRunTime * (self.building.magnitude * effMixFract / heatHrs) # (generation rate - no usage)
+        minRunVol_G = pCompMinimumRunTime * (self.building.magnitude / heatHrs) # (generation rate - no usage)  #REMOVED EFFMIXFRACT
 
         if minRunVol_G > cyclingVol_G:
             min_AF = minRunVol_G / totalVolAtStorage + (1 - self.percentUseable)
             if min_AF < 1:
                 raise ValueError("01", "The aquastat fraction is too low in the storge system recommend increasing the maximum run hours in the day or increasing to a minimum of: ", round(min_AF,3))
             raise ValueError("02", "The minimum aquastat fraction is greater than 1. This is due to the storage efficency and/or the maximum run hours in the day may be too low. Try increasing these values, we reccomend 0.8 and 16 hours for these variables respectively." )
 
+        
         # Return the temperature adjusted total volume ########################
+        
         return totalVolAtStorage, effMixFract
     
     def _calcRunningVol(self, heatHrs, onOffArr, loadshape, effMixFract = 0):
         """
         Function to find the running volume for the hot water storage tank, which
         is needed for calculating the total volume for primary sizing and in the event of load shift sizing
         represents the entire volume.
@@ -310,55 +399,98 @@
         loadshape : ndarray
             normalized array of length 24 representing the daily loadshape for this calculation.
         effMixFract: Int
             unused value in this instance of the function. Used in Swing Tank implimentation
 
         Raises
         ------
-        Exception: Error if oversizeing system.
+        Exception: Error if oversizing system.
 
         Returns
         -------
         runV_G : float
-            The running volume in gallons
+            The running volume in gallons at supply temp.
         effMixFract: int
-            returns same value from parameter. Needed for Swing Tank implimentation. Not actually used in this function instance 
+            Needed for swing tank implementation.
         """          
-        genrate = np.tile(onOffArr,2) / heatHrs #hourly
-        diffN = genrate - np.tile(loadshape,2) #hourly
+        genRate = np.tile(onOffArr,2) / heatHrs #hourly
+        diffN = genRate - np.tile(loadshape,2) #hourly
         diffInd = getPeakIndices(diffN[0:24]) #Days repeat so just get first day!
         diffN *= self.building.magnitude
+        
         # Get the running volume ##############################################
         if len(diffInd) == 0:
             #TODO but what if it is undersized? Also can this ever be hit? users currently do not have power to change num hours from interface
             raise Exception("ERROR ID 03","The heating rate is greater than the peak volume the system is oversized! Try increasing the hours the heat pump runs in a day",)
         runV_G = 0
         for peakInd in diffInd:
             #Get the rest of the day from the start of the peak
             diffCum = np.cumsum(diffN[peakInd:])  #hourly
             runV_G = max(runV_G, -min(diffCum[diffCum<0.])) #Minimum value less than 0 or 0.
-
         return runV_G, effMixFract
     
+    def _calcRunningVolLS(self, loadUpHours, effMixFract = 1):
+        """
+        Function to calculate the running volume if load shifting. Using the max generation rate between normal sizing
+        and preliminary volume, the deficit between generation and hot water use is then added to the preliminary volume.
+
+        Implemented separately for swing tank system.
+
+        Parameters
+        ------   
+        loadUpHours : float
+            Number of hours of scheduled load up before first shed. If sizing, this is set by user. If creating sizing
+            plot, number may vary.   
+        effMixFract : float
+            Only used in swing tank implementation.
+
+        Returns
+        ------
+        LSrunV_G : float
+            Volume needed between primary shed aquastat and load up aquastat at supply temp.
+        effMixFract : float
+            Used for swing tank implementation.
+        """
+        Vshift = self._calcPrelimVol(loadUpHours)[0] #volume to make it through first shed
+        
+        genRateON = self._primaryHeatHrs2kBTUHR(self.maxDayRun_hr, loadUpHours, effSwingVolFract = effMixFract, primaryCurve = False)[1] #max generation rate from both methods
+        genRate = [genRateON if x != 0 else 0 for x in self.loadShiftSchedule] #set generation rate during shed to 0
+        
+        diffN = np.tile(genRate, 2) - np.tile(self.building.avgLoadshape,2) * self.building.magnitude
+        
+        #get first index after shed
+        shedEnd = [i for i,x in enumerate(genRate[1:],1) if x > genRate[i-1]][0] #start at beginning of first shed, fully loaded up equivalent to starting at the end of shed completely "empty"
+        diffCum = np.cumsum(diffN[shedEnd:]) 
+        LSrunV_G = -min(diffCum[diffCum<0.], default = 0) #numbers less than 0 are a hot water deficit, find the biggest deficit. if no deficit then 0.
+        
+        #add running volume to preliminary shifted volume
+        LSrunV_G += Vshift
+        
+        return LSrunV_G, effMixFract 
+
     def _getTotalVolAtStorage(self, runningVol_G):
         """
-        Calculates the maximum primary storage using the Ecotope sizing methodology. Swing Tanks implement sperately
+        Calculates the maximum primary storage using the Ecotope sizing methodology. Swing Tanks implement sperately.
 
         Parameters
         ----------
         runningVol_G : float
             The running volume in gallons
+        avgStorageT_F : float
+            Average storage temperature. If not load shifting this is the storage temp. If load shifting this is the 
+            average between load up and normal setpoint based on aquastat locations.
 
         Returns
         -------
         totalVolMax : float
-            The total storage volume in gallons adjusted to the storage tempreature
+            The total storage volume in gallons adjusted to the storage tempreature.
         
         """
-        return mixVolume(runningVol_G, self.storageT_F, self.building.incomingT_F, self.building.supplyT_F) / (1-self.aquaFract)
+        
+        return mixVolume(runningVol_G, self.storageT_F, self.building.incomingT_F, self.building.supplyT_F) / (1 - self.aquaFract)
     
     def primaryCurve(self):
         """
         Sizes the primary system curve. Will catch the point at which the aquatstat
         fraction is too small for system and cuts the return arrays to match cutoff point.
 
         Returns
@@ -374,32 +506,60 @@
             
         recIndex : int
             The index of the recommended heating rate. 
         """
         # Define the heating hours we'll check
         delta = -0.25
         maxHeatHours = 1/(max(self.building.loadshape))*1.001   
-        
-        arr1 = np.arange(24, self.maxDayRun_hr, delta)
+        arr1 = np.arange(24, self.maxDayRun_hr, delta) #TODO why are we going all the way to 24 hours ???
         recIndex = len(arr1)
         heatHours = np.concatenate((arr1, np.arange(self.maxDayRun_hr, maxHeatHours, delta)))
         
         volN = np.zeros(len(heatHours))
         effMixFract = np.ones(len(heatHours))
         for i in range(0,len(heatHours)):
             try:
-                volN[i], effMixFract[i] = self.sizePrimaryTankVolume(heatHours[i])
+                volN[i], effMixFract[i] = self.sizePrimaryTankVolume(heatHours[i], self.loadUpHours, primaryCurve = True)
+                
             except ValueError:
                 break
         # Cut to the point the aquastat fraction was too small
         volN        = volN[:i]
         heatHours   = heatHours[:i]
         effMixFract = effMixFract[:i]
 
-        return [volN, self._primaryHeatHrs2kBTUHR(heatHours, effMixFract), heatHours, recIndex]
+        return [volN, self._primaryHeatHrs2kBTUHR(heatHours, self.loadUpHours, effSwingVolFract = effMixFract, primaryCurve = True)[0], heatHours, recIndex]
+
+    def lsSizedPoints(self):
+        """
+        Creates points for sizing curve plot based on number of hours in first load up period. If "regular" sizing 
+        drives algorithmn, regular sizing will be used. This prevents user from oversizing system by putting 
+        ill-informed number of load up hours.
+
+        Returns
+        lsSizingCombos : array
+            Array of volume and capacity combinations sized based on the number of load up hours.
+        """
+        
+        volN = np.zeros(5)
+        capN = np.zeros(5)
+        effMixN = np.zeros(5)
+        N = np.zeros(5)
+
+        #load up hours to loop through
+        for i in range(1, 6): #arbitrary stopping point, anything more than this will not result in different sizing
+            #size the primary system based on the number of load up hours
+            volN[i-1], effMixN[i-1] = self.sizePrimaryTankVolume(heatHrs = self.maxDayRun_hr, loadUpHours = i, primaryCurve = False)
+            capN[i-1] = self._primaryHeatHrs2kBTUHR(heathours = self.maxDayRun_hr, loadUpHours = i, effSwingVolFract = effMixN[i-1], primaryCurve = False)[0]
+            N[i-1] = i
+
+        volN, capN = zip(*set(zip(volN, capN)))
+        N = N[:len(volN)]
+    
+        return [volN, capN, N]
 
     
     def runOnePrimaryStep(self, pheating, V0, Vtrig, Vcurr, hw_out, hw_in):
         """
         Runs one step on the primary system. This changes the volume of the primary system
         by assuming there is hot water removed at a volume of hw_out and hot water
         generated or added at a volume of hw_in. This is assuming the system is perfectly
@@ -434,30 +594,29 @@
         """
         did_run = 0
         Vnew = 0
         if pheating:
             Vnew = Vcurr + hw_in - hw_out # If heating, generate HW and lose HW
             did_run = hw_in
 
-        else:  # Else not heating,
+        else:  # Else not heating, REMOVED TIME MISSED HERE
             Vnew = Vcurr - hw_out # So lose HW
             if Vnew < Vtrig: # If should heat
-                time_missed = (Vtrig - Vnew)/hw_out # Volume below turn on / rate of draw gives time below tigger (aquastat)
-                Vnew += hw_in * time_missed # Start heating
-                did_run = hw_in * time_missed
+                Vnew += hw_in # # Start heating
+                did_run = hw_in 
                 pheating = True
 
         if Vnew > V0: # If overflow
             time_over = (Vnew - V0) / (hw_in - hw_out) # Volume over generated / rate of generation gives time above full
             Vnew = V0 - hw_out * time_over # Make full with missing volume
             did_run = hw_in * (1-time_over)
             pheating = False # Stop heating
 
         if Vnew < 0:
-           raise Exception("Primary storage ran out of Volume!")
+           raise Exception("Primary storage ran out of Volume!") 
 
         return pheating, Vnew, did_run
     
     def plotStorageLoadSim(self, return_as_div=True):
         """
         Returns a plot of the of the simulation for the minimum sized primary
         system as a div or plotly figure. Can plot the minute level simulation
@@ -471,24 +630,24 @@
 
         Returns
         -------
         div/fig
             plot_div
         """
         [V, G_hw, D_hw, run] = self.simulate()
-
+        
         hrind_fromback = 24 # Look at the last 24 hours of the simulation not the whole thing
         run = np.array(run[-(60*hrind_fromback):])*60
         G_hw = np.array(G_hw[-(60*hrind_fromback):])*60
         D_hw = np.array(D_hw[-(60*hrind_fromback):])*60
         V = np.array(V[-(60*hrind_fromback):])
 
         if any(i < 0 for i in V):
-            raise Exception("Primary storage ran out of Volume!")
-
+            raise Exception("Primary storage ran out of Volume!") 
+        
         fig = Figure()
 
         # Do primary components
         x_data = list(range(len(V)))
 
         if self.doLoadShift:
             ls_off = [int(not x)* max(V)*2 for x in G_hw]
@@ -516,14 +675,74 @@
 
         if return_as_div:
             plot_div = plot(fig, output_type='div', show_link=False, link_text="",
                         include_plotlyjs = False)
             return plot_div
         return fig
     
+    def _calcPrelimVol(self, loadUpHours):
+        '''
+        Function to calculate volume shifted during first shed period, which is used to calculated generation rate
+        needed for load up.
+
+        Parameters
+        ----------
+        loadUpHours : float
+            Number of hours of scheduled load up before first shed. If sizing, this is set by user. If creating sizing
+            plot, number may vary. 
+
+        Returns 
+        ----------
+        Vshift : float
+            Volume at supply temp between normal and load up AQ fract needed to make it through first shed period.
+        VconsumedLU : float
+            Volume at supply temp consumed during first load up period.
+        '''
+        shedHours = [i for i in range(len(self.loadShiftSchedule)) if self.loadShiftSchedule[i] == 0] #get all scheduled shed hours
+        firstShed = [x for i,x in enumerate(shedHours) if x == shedHours[0] + i] #get first shed
+        Vshift = sum([self.building.avgLoadshape[i]*self.building.magnitude for i in firstShed])#calculate vol used during first shed
+        VconsumedLU = sum(self.building.avgLoadshape[firstShed[0] - loadUpHours : firstShed[0]]) * self.building.magnitude
+        
+        return Vshift, VconsumedLU 
+        
+        
+
+    def _mixStorageTemps(self, runningVol_G):
+        """
+        Calculates average tank temperature using load up and normal setpoints according to locations of aquastats. 
+        Used for load shifting when there are two setpoints. Returns normal storage setpoint if load up and normal
+        setpoint are equal or if not loadshifting.
+
+        Parameters
+        ----------
+        runningVol_G : float
+            Volume of water to be mixed. 
+
+        Returns
+        ----------
+        mixStorageT_F: float
+            Average storage temperature calcuated with normal setpoint and load up setpoint.
+        totalVolMax : float
+            The total storage volume in gallons adjusted to the average storage temperature.
+        """
+        mixStorageT_F = self.storageT_F
+
+        if self.doLoadShift:
+            f = (self.aquaFract - self.aquaFractLoadUp) / (self.aquaFractShed - self.aquaFractLoadUp) 
+            normV = (1 - f) * runningVol_G
+            loadV = f * runningVol_G
+
+            mixStorageT_F = (self.storageT_F * normV + self.loadUpT_F * loadV) / (normV + loadV)
+
+            return mixStorageT_F, mixVolume(runningVol_G, mixStorageT_F, self.building.incomingT_F, self.building.supplyT_F) / (self.aquaFractShed - self.aquaFractLoadUp)
+        
+        return [mixStorageT_F]
+
     
 class Primary(SystemConfig):
     def __init__(self, building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, 
-                 doLoadShift = False, loadShiftPercent = 1, loadShiftSchedule = None):
+                 doLoadShift = False, loadShiftPercent = 1, loadShiftSchedule = None, loadUpHours = None, aquaFractLoadUp = None, 
+                 aquaFractShed = None, loadUpT_F = None):
         super().__init__(building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, 
-                 doLoadShift, loadShiftPercent, loadShiftSchedule)
+                 doLoadShift, loadShiftPercent, loadShiftSchedule, loadUpHours, aquaFractLoadUp, aquaFractShed, loadUpT_F)
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ecoengine-0.0.5/src/ecoengine/objects/__init__.py` & `ecoengine-0.0.6/src/ecoengine/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.5/src/ecoengine/objects/systemConfigUtils.py` & `ecoengine-0.0.6/src/ecoengine/objects/systemConfigUtils.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.5/src/ecoengine/objects/systems/ParallelLoopTank.py` & `ecoengine-0.0.6/src/ecoengine/objects/systems/ParallelLoopTank.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 import numpy as np
 from ecoengine.objects.Building import Building
 from ecoengine.constants.Constants import *
 from ecoengine.objects.systemConfigUtils import checkLiqudWater
 
 class ParallelLoopTank(SystemConfig):
     def __init__(self, safetyTM, setpointTM_F, TMonTemp_F, offTime_hr, building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, 
-                 doLoadShift = False, loadShiftPercent = 1, loadShiftSchedule = None):
+                 doLoadShift = False, loadShiftPercent = 1, loadShiftSchedule = None, loadUpHours = None, aquaFractLoadUp = None, aquaFractShed = None, loadUpT_F = None):
+
 
         if TMonTemp_F == 0:
             TMonTemp_F = building.incomingT_F + 2
         
         super().__init__(building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, 
-                 doLoadShift, loadShiftPercent, loadShiftSchedule)
+                 doLoadShift, loadShiftPercent, loadShiftSchedule, loadUpHours, aquaFractLoadUp, aquaFractShed, loadUpT_F)
         
         self._checkParallelLoopInputs(safetyTM, offTime_hr, setpointTM_F, TMonTemp_F)
         self.setpointTM_F = setpointTM_F
         self.TMonTemp_F = TMonTemp_F
         self.offTime_hr = offTime_hr # Hour
         self.safetyTM = safetyTM # Safety factor
```

### Comparing `ecoengine-0.0.5/src/ecoengine.egg-info/PKG-INFO` & `ecoengine-0.0.6/src/ecoengine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoengine
-Version: 0.0.5
+Version: 0.0.6
 Summary: A software for sizing Heat Pump Water Heaters for buildings
 Home-page: https://ecosizer.ecotope.com/sizer/
 Author: Nolan
 Author-email: nolan@ecotope.com
 Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecoengine-0.0.5/src/ecoengine.egg-info/SOURCES.txt` & `ecoengine-0.0.6/src/ecoengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

