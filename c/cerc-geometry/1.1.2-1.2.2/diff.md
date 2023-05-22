# Comparing `tmp/cerc-geometry-1.1.2.tar.gz` & `tmp/cerc-geometry-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/peteryefi/Desktop/dompark/geometry/dist/.tmp-_wn4m695/cerc-geometry-1.1.2.tar", last modified: Fri May 19 00:06:57 2023, max compression
+gzip compressed data, was "/Users/peteryefi/Desktop/dompark/geometry/dist/.tmp-py5a9jq4/cerc-geometry-1.2.2.tar", last modified: Mon May 22 23:23:31 2023, max compression
```

## Comparing `cerc-geometry-1.1.2.tar` & `cerc-geometry-1.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-19 00:06:57.519708 cerc-geometry-1.1.2/
--rw-rw-rw-   0 peteryefi   (501) staff       (20)     7431 2023-05-11 00:53:33.000000 cerc-geometry-1.1.2/LICENSE.md
--rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-19 00:06:57.519377 cerc-geometry-1.1.2/PKG-INFO
--rw-r--r--   0 peteryefi   (501) staff       (20)      522 2023-05-12 17:30:08.000000 cerc-geometry-1.1.2/README.md
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-19 00:06:57.509289 cerc-geometry-1.1.2/cerc_geometry.egg-info/
--rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-19 00:06:57.000000 cerc-geometry-1.1.2/cerc_geometry.egg-info/PKG-INFO
--rw-r--r--   0 peteryefi   (501) staff       (20)      535 2023-05-19 00:06:57.000000 cerc-geometry-1.1.2/cerc_geometry.egg-info/SOURCES.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)        1 2023-05-19 00:06:57.000000 cerc-geometry-1.1.2/cerc_geometry.egg-info/dependency_links.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)       48 2023-05-19 00:06:57.000000 cerc-geometry-1.1.2/cerc_geometry.egg-info/requires.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)        9 2023-05-19 00:06:57.000000 cerc-geometry-1.1.2/cerc_geometry.egg-info/top_level.txt
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-19 00:06:57.515579 cerc-geometry-1.1.2/geometry/
--rw-r--r--   0 peteryefi   (501) staff       (20)      200 2023-05-19 00:02:34.000000 cerc-geometry-1.1.2/geometry/__init__.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     5398 2023-05-16 00:05:51.000000 cerc-geometry-1.1.2/geometry/helper.py
--rw-r--r--   0 peteryefi   (501) staff       (20)    11268 2023-05-18 23:49:06.000000 cerc-geometry-1.1.2/geometry/library.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      574 2023-05-18 23:39:06.000000 cerc-geometry-1.1.2/geometry/location.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      707 2023-05-18 23:38:20.000000 cerc-geometry-1.1.2/geometry/map_point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     2168 2023-05-15 23:21:05.000000 cerc-geometry-1.1.2/geometry/plane.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1002 2023-05-15 23:21:05.000000 cerc-geometry-1.1.2/geometry/point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)    14604 2023-05-16 00:05:51.000000 cerc-geometry-1.1.2/geometry/polygon.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     6590 2023-05-15 23:21:05.000000 cerc-geometry-1.1.2/geometry/polyhedron.py
--rw-r--r--   0 peteryefi   (501) staff       (20)       99 2023-05-15 23:40:38.000000 cerc-geometry-1.1.2/pyproject.toml
--rw-r--r--   0 peteryefi   (501) staff       (20)       37 2023-05-18 23:51:47.000000 cerc-geometry-1.1.2/requirements.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)       38 2023-05-19 00:06:57.519820 cerc-geometry-1.1.2/setup.cfg
--rw-r--r--   0 peteryefi   (501) staff       (20)     1320 2023-05-19 00:06:23.000000 cerc-geometry-1.1.2/setup.py
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-19 00:06:57.518821 cerc-geometry-1.1.2/tests/
--rw-r--r--   0 peteryefi   (501) staff       (20)     1961 2023-05-16 00:05:50.000000 cerc-geometry-1.1.2/tests/test_helper.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      736 2023-05-16 00:05:50.000000 cerc-geometry-1.1.2/tests/test_plane.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      842 2023-05-16 00:05:50.000000 cerc-geometry-1.1.2/tests/test_point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1513 2023-05-16 00:05:50.000000 cerc-geometry-1.1.2/tests/test_polygon.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1076 2023-05-16 00:05:50.000000 cerc-geometry-1.1.2/tests/test_polyhedron.py
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-22 23:23:31.718396 cerc-geometry-1.2.2/
+-rw-rw-rw-   0 peteryefi   (501) staff       (20)     7431 2023-05-11 00:53:33.000000 cerc-geometry-1.2.2/LICENSE.md
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-22 23:23:31.718065 cerc-geometry-1.2.2/PKG-INFO
+-rw-r--r--   0 peteryefi   (501) staff       (20)      522 2023-05-12 17:30:08.000000 cerc-geometry-1.2.2/README.md
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-22 23:23:31.707310 cerc-geometry-1.2.2/cerc_geometry.egg-info/
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-22 23:23:31.000000 cerc-geometry-1.2.2/cerc_geometry.egg-info/PKG-INFO
+-rw-r--r--   0 peteryefi   (501) staff       (20)      535 2023-05-22 23:23:31.000000 cerc-geometry-1.2.2/cerc_geometry.egg-info/SOURCES.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)        1 2023-05-22 23:23:31.000000 cerc-geometry-1.2.2/cerc_geometry.egg-info/dependency_links.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)       48 2023-05-22 23:23:31.000000 cerc-geometry-1.2.2/cerc_geometry.egg-info/requires.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)        9 2023-05-22 23:23:31.000000 cerc-geometry-1.2.2/cerc_geometry.egg-info/top_level.txt
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-22 23:23:31.713589 cerc-geometry-1.2.2/geometry/
+-rw-r--r--   0 peteryefi   (501) staff       (20)      200 2023-05-19 00:02:34.000000 cerc-geometry-1.2.2/geometry/__init__.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     5398 2023-05-16 00:05:51.000000 cerc-geometry-1.2.2/geometry/helper.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)    11135 2023-05-22 23:18:20.000000 cerc-geometry-1.2.2/geometry/library.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      574 2023-05-18 23:39:06.000000 cerc-geometry-1.2.2/geometry/location.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      707 2023-05-18 23:38:20.000000 cerc-geometry-1.2.2/geometry/map_point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     2168 2023-05-15 23:21:05.000000 cerc-geometry-1.2.2/geometry/plane.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1002 2023-05-15 23:21:05.000000 cerc-geometry-1.2.2/geometry/point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)    14604 2023-05-16 00:05:51.000000 cerc-geometry-1.2.2/geometry/polygon.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     6590 2023-05-15 23:21:05.000000 cerc-geometry-1.2.2/geometry/polyhedron.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)       99 2023-05-15 23:40:38.000000 cerc-geometry-1.2.2/pyproject.toml
+-rw-r--r--   0 peteryefi   (501) staff       (20)       37 2023-05-18 23:51:47.000000 cerc-geometry-1.2.2/requirements.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)       38 2023-05-22 23:23:31.718519 cerc-geometry-1.2.2/setup.cfg
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1320 2023-05-22 23:18:57.000000 cerc-geometry-1.2.2/setup.py
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-22 23:23:31.717393 cerc-geometry-1.2.2/tests/
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1961 2023-05-16 00:05:50.000000 cerc-geometry-1.2.2/tests/test_helper.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      736 2023-05-16 00:05:50.000000 cerc-geometry-1.2.2/tests/test_plane.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      842 2023-05-16 00:05:50.000000 cerc-geometry-1.2.2/tests/test_point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1513 2023-05-16 00:05:50.000000 cerc-geometry-1.2.2/tests/test_polygon.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1076 2023-05-16 00:05:50.000000 cerc-geometry-1.2.2/tests/test_polyhedron.py
```

### Comparing `cerc-geometry-1.1.2/LICENSE.md` & `cerc-geometry-1.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.1.2/PKG-INFO` & `cerc-geometry-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-geometry
-Version: 1.1.2
+Version: 1.2.2
 Summary: CERC Geometry Library with different modules to manipulate geometric objects
 Home-page: https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Author: CERC
 Author-email:  cerc@concordia.ca
 Project-URL: Repository, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Project-URL: Bug Tracker, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cerc-geometry-1.1.2/README.md` & `cerc-geometry-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.1.2/cerc_geometry.egg-info/PKG-INFO` & `cerc-geometry-1.2.2/cerc_geometry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-geometry
-Version: 1.1.2
+Version: 1.2.2
 Summary: CERC Geometry Library with different modules to manipulate geometric objects
 Home-page: https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Author: CERC
 Author-email:  cerc@concordia.ca
 Project-URL: Repository, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Project-URL: Bug Tracker, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cerc-geometry-1.1.2/cerc_geometry.egg-info/SOURCES.txt` & `cerc-geometry-1.2.2/cerc_geometry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.1.2/geometry/helper.py` & `cerc-geometry-1.2.2/geometry/helper.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.1.2/geometry/library.py` & `cerc-geometry-1.2.2/geometry/library.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
   def __init__(self, delta=0, area_delta=0):
     self._delta = delta
     self._area_delta = area_delta
 
   @staticmethod
   def coordinate_to_map_point(coordinate, city):
-    factor = GeometryHelper.factor()
+    factor = Library.factor()
     return MapPoint(((coordinate[0] - city.lower_corner[0]) * factor), ((coordinate[1] - city.lower_corner[1]) * factor))
 
   @staticmethod
   def city_mapping(city, building_names=None, plot=False):
 
     """
 
@@ -49,15 +49,15 @@
     {
      "building_name" : [{line: 0 coordinate_1: [x,y,z], coordinate_2:[x, y, z], points: 0}]
     }
     """
     lines_information = {}
     if building_names is None:
       building_names = [b.name for b in city.buildings]
-    factor = GeometryHelper.factor()
+    factor = Library.factor()
     x = math.ceil((city.upper_corner[0] - city.lower_corner[0]) * factor) + 1
     y = math.ceil((city.upper_corner[1] - city.lower_corner[1]) * factor) + 1
     city_map = [['' for _ in range(y + 1)] for _ in range(x + 1)]
     map_info = [[{} for _ in range(y + 1)] for _ in range(x + 1)]
     img = Image.new('RGB', (x + 1, y + 1), "black")  # create a new black image
     city_image = img.load()  # create the pixel map
     for building_name in building_names:
@@ -67,40 +67,40 @@
         length = len(ground.perimeter_polygon.coordinates) - 1
         for i, coordinate in enumerate(ground.perimeter_polygon.coordinates):
 
           j = i + 1
           if i == length:
             j = 0
           next_coordinate = ground.perimeter_polygon.coordinates[j]
-          distance = GeometryHelper.distance_between_points(coordinate, next_coordinate)
+          distance = Library.distance_between_points(coordinate, next_coordinate)
           steps = int(distance * factor * 2)
           if steps == 0:
             continue
           delta_x = (next_coordinate[0] - coordinate[0]) / steps
           delta_y = (next_coordinate[1] - coordinate[1]) / steps
 
           for k in range(0, steps):
             new_coordinate = (coordinate[0] + (delta_x * k), coordinate[1] + (delta_y * k))
-            point = GeometryHelper.coordinate_to_map_point(new_coordinate, city)
+            point = Library.coordinate_to_map_point(new_coordinate, city)
             x = point.x
             y = point.y
             if city_map[x][y] == '':
               city_map[x][y] = building.name
               map_info[x][y] = {
                 'line_start': (coordinate[0], coordinate[1]),
                 'line_end': (next_coordinate[0], next_coordinate[1]),
               }
               city_image[x, y] = (100, 0, 0)
             elif city_map[x][y] != building.name:
               neighbour = city.city_object(city_map[x][y])
               neighbour_info = map_info[x][y]
 
               # prepare the keys
-              neighbour_start_coordinate = f'{GeometryHelper.coordinate_to_map_point(neighbour_info["line_start"], city)}'
-              building_start_coordinate = f'{GeometryHelper.coordinate_to_map_point(coordinate, city)}'
+              neighbour_start_coordinate = f'{Library.coordinate_to_map_point(neighbour_info["line_start"], city)}'
+              building_start_coordinate = f'{Library.coordinate_to_map_point(coordinate, city)}'
               neighbour_key = f'{neighbour.name}_{neighbour_start_coordinate}_{building_start_coordinate}'
               building_key = f'{building.name}_{building_start_coordinate}_{neighbour_start_coordinate}'
 
               # Add my neighbour info to my shared lines
               if building.name in lines_information.keys() and neighbour_key in lines_information[building.name]:
                 shared_points = int(lines_information[building.name][neighbour_key]['shared_points'])
                 lines_information[building.name][neighbour_key]['shared_points'] = shared_points + 1
@@ -109,18 +109,18 @@
                   lines_information[building.name] = {}
                 lines_information[building.name][neighbour_key] = {
                   'neighbour_name': neighbour.name,
                   'line_start': (coordinate[0], coordinate[1]),
                   'line_end': (next_coordinate[0], next_coordinate[1]),
                   'neighbour_line_start': neighbour_info['line_start'],
                   'neighbour_line_end': neighbour_info['line_end'],
-                  'coordinate_start': f"{GeometryHelper.coordinate_to_map_point(coordinate, city)}",
-                  'coordinate_end': f"{GeometryHelper.coordinate_to_map_point(next_coordinate, city)}",
-                  'neighbour_start': f"{GeometryHelper.coordinate_to_map_point(neighbour_info['line_start'], city)}",
-                  'neighbour_end': f"{GeometryHelper.coordinate_to_map_point(neighbour_info['line_end'], city)}",
+                  'coordinate_start': f"{Library.coordinate_to_map_point(coordinate, city)}",
+                  'coordinate_end': f"{Library.coordinate_to_map_point(next_coordinate, city)}",
+                  'neighbour_start': f"{Library.coordinate_to_map_point(neighbour_info['line_start'], city)}",
+                  'neighbour_end': f"{Library.coordinate_to_map_point(neighbour_info['line_end'], city)}",
                   'shared_points': 1
                 }
 
               # Add my info to my neighbour shared lines
               if neighbour.name in lines_information.keys() and building_key in lines_information[neighbour.name]:
                 shared_points = int(lines_information[neighbour.name][building_key]['shared_points'])
                 lines_information[neighbour.name][building_key]['shared_points'] = shared_points + 1
@@ -129,18 +129,18 @@
                   lines_information[neighbour.name] = {}
                 lines_information[neighbour.name][building_key] = {
                   'neighbour_name': building.name,
                   'line_start': neighbour_info['line_start'],
                   'line_end': neighbour_info['line_end'],
                   'neighbour_line_start': (coordinate[0], coordinate[1]),
                   'neighbour_line_end': (next_coordinate[0], next_coordinate[1]),
-                  'neighbour_start': f"{GeometryHelper.coordinate_to_map_point(coordinate, city)}",
-                  'neighbour_end': f"{GeometryHelper.coordinate_to_map_point(next_coordinate, city)}",
-                  'coordinate_start': f"{GeometryHelper.coordinate_to_map_point(neighbour_info['line_start'], city)}",
-                  'coordinate_end': f"{GeometryHelper.coordinate_to_map_point(neighbour_info['line_end'], city)}",
+                  'neighbour_start': f"{Library.coordinate_to_map_point(coordinate, city)}",
+                  'neighbour_end': f"{Library.coordinate_to_map_point(next_coordinate, city)}",
+                  'coordinate_start': f"{Library.coordinate_to_map_point(neighbour_info['line_start'], city)}",
+                  'coordinate_end': f"{Library.coordinate_to_map_point(neighbour_info['line_end'], city)}",
                   'shared_points': 1
                 }
 
               if building.neighbours is None:
                 building.neighbours = [neighbour]
               elif neighbour not in building.neighbours:
                 building.neighbours.append(neighbour)
@@ -162,19 +162,19 @@
     # todo: trimesh has a method for this
     line_points = [lines[0][0], lines[0][1]]
     lines.remove(lines[0])
     while len(lines) > 1:
       i = 0
       for line in lines:
         i += 1
-        if GeometryHelper.distance_between_points(line[0], line_points[len(line_points) - 1]) < 1e-8:
+        if Library.distance_between_points(line[0], line_points[len(line_points) - 1]) < 1e-8:
           line_points.append(line[1])
           lines.pop(i - 1)
           break
-        if GeometryHelper.distance_between_points(line[1], line_points[len(line_points) - 1]) < 1e-8:
+        if Library.distance_between_points(line[1], line_points[len(line_points) - 1]) < 1e-8:
           line_points.append(line[0])
           lines.pop(i - 1)
           break
     polyhedron = Polyhedron(Polygon(line_points).triangles)
     trimesh = Trimesh(polyhedron.vertices, polyhedron.faces)
     return trimesh
 
@@ -219,21 +219,21 @@
     for i in range(0, len(normal_plane)):
       normal_plane_opp[i] = - normal_plane[i]
 
     section_1 = intersections.slice_mesh_plane(trimesh, normal_plane, point_plane)
     if section_1 is None:
       return [trimesh]
     lines = list(intersections.mesh_plane(trimesh, normal_plane, point_plane))
-    cap = GeometryHelper.segment_list_to_trimesh(lines)
-    trimesh_1 = GeometryHelper._merge_meshes(section_1, cap)
+    cap = Library.segment_list_to_trimesh(lines)
+    trimesh_1 = Library._merge_meshes(section_1, cap)
 
     section_2 = intersections.slice_mesh_plane(trimesh, normal_plane_opp, point_plane)
     if section_2 is None:
       return [trimesh_1]
-    trimesh_2 = GeometryHelper._merge_meshes(section_2, cap)
+    trimesh_2 = Library._merge_meshes(section_2, cap)
 
     return [trimesh_1, trimesh_2]
 
   @staticmethod
   def get_location(latitude, longitude) -> Location:
     """
     Get Location from latitude and longitude
```

### Comparing `cerc-geometry-1.1.2/geometry/location.py` & `cerc-geometry-1.2.2/geometry/location.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.1.2/geometry/map_point.py` & `cerc-geometry-1.2.2/geometry/map_point.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.1.2/geometry/plane.py` & `cerc-geometry-1.2.2/geometry/plane.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.1.2/geometry/point.py` & `cerc-geometry-1.2.2/geometry/point.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.1.2/geometry/polygon.py` & `cerc-geometry-1.2.2/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.1.2/geometry/polyhedron.py` & `cerc-geometry-1.2.2/geometry/polyhedron.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.1.2/setup.py` & `cerc-geometry-1.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     for requirement
     in pkg_resources.parse_requirements(r)
   ]
 install_requires.append('setuptools')
 
 setuptools.setup(
   name="cerc-geometry",
-  version="1.1.2",
+  version="1.2.2",
   author="CERC",
   author_email=" cerc@concordia.ca",
   description="CERC Geometry Library with different modules to manipulate geometric objects",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry",
   project_urls={
```

### Comparing `cerc-geometry-1.1.2/tests/test_helper.py` & `cerc-geometry-1.2.2/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.1.2/tests/test_plane.py` & `cerc-geometry-1.2.2/tests/test_plane.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.1.2/tests/test_point.py` & `cerc-geometry-1.2.2/tests/test_point.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.1.2/tests/test_polygon.py` & `cerc-geometry-1.2.2/tests/test_polygon.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.1.2/tests/test_polyhedron.py` & `cerc-geometry-1.2.2/tests/test_polyhedron.py`

 * *Files identical despite different names*

