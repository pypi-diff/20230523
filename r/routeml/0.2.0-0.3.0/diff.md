# Comparing `tmp/routeml-0.2.0.tar.gz` & `tmp/routeml-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routeml-0.2.0.tar", last modified: Fri May 19 21:00:49 2023, max compression
+gzip compressed data, was "routeml-0.3.0.tar", last modified: Tue May 23 18:45:10 2023, max compression
```

## Comparing `routeml-0.2.0.tar` & `routeml-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-19 21:00:49.459669 routeml-0.2.0/
--rw-r--r--   0 samuelchin   (502) staff       (20)      525 2023-05-19 21:00:49.459449 routeml-0.2.0/PKG-INFO
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.2.0/README.md
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-19 21:00:49.454727 routeml-0.2.0/routeml/
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.2.0/routeml/__init__.py
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.2.0/routeml/cvrp.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     8405 2023-05-19 20:49:05.000000 routeml-0.2.0/routeml/utils.py
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-19 21:00:49.455323 routeml-0.2.0/routeml.egg-info/
--rw-r--r--   0 samuelchin   (502) staff       (20)      525 2023-05-19 21:00:49.000000 routeml-0.2.0/routeml.egg-info/PKG-INFO
--rw-r--r--   0 samuelchin   (502) staff       (20)      664 2023-05-19 21:00:49.000000 routeml-0.2.0/routeml.egg-info/SOURCES.txt
--rw-r--r--   0 samuelchin   (502) staff       (20)        1 2023-05-19 21:00:49.000000 routeml-0.2.0/routeml.egg-info/dependency_links.txt
--rw-r--r--   0 samuelchin   (502) staff       (20)       14 2023-05-19 21:00:49.000000 routeml-0.2.0/routeml.egg-info/top_level.txt
--rw-r--r--   0 samuelchin   (502) staff       (20)       38 2023-05-19 21:00:49.459722 routeml-0.2.0/setup.cfg
--rw-r--r--   0 samuelchin   (502) staff       (20)      725 2023-05-19 20:54:43.000000 routeml-0.2.0/setup.py
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-19 21:00:49.455592 routeml-0.2.0/tests/
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.2.0/tests/__init__.py
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-19 21:00:49.455842 routeml-0.2.0/tests/integration/
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-19 15:17:17.000000 routeml-0.2.0/tests/integration/__init__.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1559 2023-05-19 16:01:42.000000 routeml-0.2.0/tests/integration/test_vrplib_cost_integration.py
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.2.0/tests/test_cvrp.py
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-19 21:00:49.456335 routeml-0.2.0/tests/unit/
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-19 15:17:06.000000 routeml-0.2.0/tests/unit/__init__.py
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-19 21:00:49.459048 routeml-0.2.0/tests/unit/utils/
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 20:08:10.000000 routeml-0.2.0/tests/unit/utils/__init__.py
--rw-r--r--   0 samuelchin   (502) staff       (20)      995 2023-05-19 15:15:01.000000 routeml-0.2.0/tests/unit/utils/test_get_cvrp_cost.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1431 2023-05-19 20:48:08.000000 routeml-0.2.0/tests/unit/utils/test_get_is_feasible.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1594 2023-05-19 19:51:57.000000 routeml-0.2.0/tests/unit/utils/test_get_route_demand.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1503 2023-05-18 21:14:17.000000 routeml-0.2.0/tests/unit/utils/test_parse_vrplib_file.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1088 2023-05-19 14:54:10.000000 routeml-0.2.0/tests/unit/utils/test_parse_vrplib_solution.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1133 2023-05-18 20:16:06.000000 routeml-0.2.0/tests/unit/utils/test_routes_to_solution.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1089 2023-05-18 20:17:28.000000 routeml-0.2.0/tests/unit/utils/test_solution_to_routes.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-23 18:45:10.838252 routeml-0.3.0/
+-rw-r--r--   0 samuelchin   (502) staff       (20)      525 2023-05-23 18:45:10.838030 routeml-0.3.0/PKG-INFO
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.3.0/README.md
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-23 18:45:10.832926 routeml-0.3.0/routeml/
+-rw-r--r--   0 samuelchin   (502) staff       (20)      106 2023-05-23 18:43:33.000000 routeml-0.3.0/routeml/__init__.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.3.0/routeml/cvrp.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)      684 2023-05-19 23:34:51.000000 routeml-0.3.0/routeml/draw.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1109 2023-05-19 23:36:17.000000 routeml-0.3.0/routeml/solvers.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     9421 2023-05-19 22:58:18.000000 routeml-0.3.0/routeml/utils.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-23 18:45:10.833902 routeml-0.3.0/routeml.egg-info/
+-rw-r--r--   0 samuelchin   (502) staff       (20)      525 2023-05-23 18:45:10.000000 routeml-0.3.0/routeml.egg-info/PKG-INFO
+-rw-r--r--   0 samuelchin   (502) staff       (20)      772 2023-05-23 18:45:10.000000 routeml-0.3.0/routeml.egg-info/SOURCES.txt
+-rw-r--r--   0 samuelchin   (502) staff       (20)        1 2023-05-23 18:45:10.000000 routeml-0.3.0/routeml.egg-info/dependency_links.txt
+-rw-r--r--   0 samuelchin   (502) staff       (20)       30 2023-05-23 18:45:10.000000 routeml-0.3.0/routeml.egg-info/requires.txt
+-rw-r--r--   0 samuelchin   (502) staff       (20)       14 2023-05-23 18:45:10.000000 routeml-0.3.0/routeml.egg-info/top_level.txt
+-rw-r--r--   0 samuelchin   (502) staff       (20)       38 2023-05-23 18:45:10.838305 routeml-0.3.0/setup.cfg
+-rw-r--r--   0 samuelchin   (502) staff       (20)      798 2023-05-23 18:44:57.000000 routeml-0.3.0/setup.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-23 18:45:10.834208 routeml-0.3.0/tests/
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.3.0/tests/__init__.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-23 18:45:10.835010 routeml-0.3.0/tests/integration/
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-19 15:17:17.000000 routeml-0.3.0/tests/integration/__init__.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)      882 2023-05-22 14:35:44.000000 routeml-0.3.0/tests/integration/test_draw_integration.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1559 2023-05-19 16:01:42.000000 routeml-0.3.0/tests/integration/test_vrplib_cost_integration.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.3.0/tests/test_cvrp.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-23 18:45:10.835373 routeml-0.3.0/tests/unit/
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-19 15:17:06.000000 routeml-0.3.0/tests/unit/__init__.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-23 18:45:10.837635 routeml-0.3.0/tests/unit/utils/
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 20:08:10.000000 routeml-0.3.0/tests/unit/utils/__init__.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)      995 2023-05-19 15:15:01.000000 routeml-0.3.0/tests/unit/utils/test_get_cvrp_cost.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1431 2023-05-19 20:48:08.000000 routeml-0.3.0/tests/unit/utils/test_get_is_feasible.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1594 2023-05-19 19:51:57.000000 routeml-0.3.0/tests/unit/utils/test_get_route_demand.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1580 2023-05-19 22:37:04.000000 routeml-0.3.0/tests/unit/utils/test_parse_vrplib_file.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1088 2023-05-19 14:54:10.000000 routeml-0.3.0/tests/unit/utils/test_parse_vrplib_solution.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1133 2023-05-18 20:16:06.000000 routeml-0.3.0/tests/unit/utils/test_routes_to_solution.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1089 2023-05-18 20:17:28.000000 routeml-0.3.0/tests/unit/utils/test_solution_to_routes.py
```

### Comparing `routeml-0.2.0/PKG-INFO` & `routeml-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routeml
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python package for CVRP utilities
 Home-page: https://github.com/jkschin/routeml
 Author: Your Name
 Author-email: jkschin@mit.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `routeml-0.2.0/routeml/utils.py` & `routeml-0.3.0/routeml/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import re
 import requests
 import math
+import random
+import numpy as np
 
 def routes_to_solution(routes):
     """
     Converts a list of routes into a solution (list of routes).
 
     Args:
         routes (list): List of routes, where each route is a list of nodes.
@@ -117,33 +119,32 @@
     if edge_weight_type_match:
         data['edge_weight_type'] = edge_weight_type_match.group(1)
 
     capacity_match = re.search(r'CAPACITY\s*:\s*(\d+)', content)
     if capacity_match:
         data['capacity'] = int(capacity_match.group(1))
 
-    # Extracting node coordinates
     node_coords_match = re.search(r'NODE_COORD_SECTION\s*(.+?)\s*DEMAND_SECTION', content, re.DOTALL)
     if node_coords_match:
         node_coords_str = node_coords_match.group(1).strip()
-        node_coords = {}
+        node_coords = []
         for line in node_coords_str.split('\n'):
             node_id, x, y = re.findall(r'(\d+)\s+([-+]?\d*\.?\d+)\s+([-+]?\d*\.?\d+)', line)[0]
-            node_coords[int(node_id) - 1] = (float(x), float(y))
-        data['node_coords'] = node_coords
+            node_coords.append([float(x), float(y)])
+        data['node_coords'] = np.array(node_coords)
 
     # Extracting demand information
     demand_section_match = re.search(r'DEMAND_SECTION\s*(.+?)\s*DEPOT_SECTION', content, re.DOTALL)
     if demand_section_match:
         demand_section_str = demand_section_match.group(1).strip()
-        demand = {}
+        demand = []
         for line in demand_section_str.split('\n'):
             node_id, demand_val = re.findall(r'(\d+)\s+(-?\d+)', line)[0]
-            demand[int(node_id) - 1] = int(demand_val)
-        data['demand'] = demand
+            demand.append(int(demand_val))
+        data['demand'] = np.array(demand)
 
     # Extracting depot information
     depot_section_match = re.search(r'DEPOT_SECTION\s*(.+?)\s*EOF', content, re.DOTALL)
     if depot_section_match:
         depot_section_str = depot_section_match.group(1).strip()
         depot_ids = [int(node_id) for node_id in re.findall(r'(\d+)\s*[^-0-9]', depot_section_str)]
         data['depot_ids'] = depot_ids
@@ -189,15 +190,15 @@
 
 def get_cvrp_cost(routes_or_solution, coordinates, uchoa=False):
     """
     Compute the total cost of a CVRP solution.
 
     Args:
         routes_or_solution (list or solution): List of routes or a solution.
-        coordinates (dict): Dictionary containing node IDs as keys and corresponding coordinates as values.
+        coordinates (np.array): Array of node coordinates with shape (n_nodes, 2).
         uchoa (bool): Whether to round the distances to the nearest integer. Follows the 2014 paper.
 
     Returns:
         float: Total cost of the CVRP solution.
     """
     if isinstance(routes_or_solution, list) and isinstance(routes_or_solution[0], list):
         solution = routes_to_solution(routes_or_solution)
@@ -263,8 +264,44 @@
     for route in routes:
         total_demand = sum(demand[node] for node in route)
         if total_demand > capacity:
             return False
 
     return True
 
+def get_cvrp_problem(num_nodes):
+    """
+    Generate a random CVRP problem.
+    Follows: "https://arxiv.org/pdf/1802.04240.pdf"
+
+    Args:
+        num_nodes (int): Number of nodes in the problem. Excluding depot.
+
+    Returns:
+        tuple: Tuple containing the node coordinates (np.ndarray) and the demand (np.ndarray).
+    """
+    # Generate depot
+    depot_id = 0
+    depot_coords = np.array([random.uniform(0, 1), random.uniform(0, 1)])
+    depot_demand = np.array([0])
+
+    # Generate node coordinates array
+    node_coords = np.empty((num_nodes + 1, 2))
+    node_coords[depot_id] = depot_coords
+
+    # Generate demand array
+    demands = np.empty((num_nodes + 1))
+    demands[depot_id] = depot_demand
+
+    # Generate node coordinates and demand
+    for node_id in range(1, num_nodes + 1):
+        x = random.uniform(0, 1)
+        y = random.uniform(0, 1)
+        demand_val = random.randint(1, 9)
+        node_coords[node_id] = np.array([float(x), float(y)])
+        demands[node_id] = int(demand_val)
+
+    return node_coords, demands
+
+
+
```

### Comparing `routeml-0.2.0/routeml.egg-info/PKG-INFO` & `routeml-0.3.0/routeml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routeml
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python package for CVRP utilities
 Home-page: https://github.com/jkschin/routeml
 Author: Your Name
 Author-email: jkschin@mit.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `routeml-0.2.0/routeml.egg-info/SOURCES.txt` & `routeml-0.3.0/routeml.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 README.md
 setup.py
 routeml/__init__.py
 routeml/cvrp.py
+routeml/draw.py
+routeml/solvers.py
 routeml/utils.py
 routeml.egg-info/PKG-INFO
 routeml.egg-info/SOURCES.txt
 routeml.egg-info/dependency_links.txt
+routeml.egg-info/requires.txt
 routeml.egg-info/top_level.txt
 tests/__init__.py
 tests/test_cvrp.py
 tests/integration/__init__.py
+tests/integration/test_draw_integration.py
 tests/integration/test_vrplib_cost_integration.py
 tests/unit/__init__.py
 tests/unit/utils/__init__.py
 tests/unit/utils/test_get_cvrp_cost.py
 tests/unit/utils/test_get_is_feasible.py
 tests/unit/utils/test_get_route_demand.py
 tests/unit/utils/test_parse_vrplib_file.py
```

### Comparing `routeml-0.2.0/setup.py` & `routeml-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='routeml',
-    version='0.2.0',
+    version='0.3.0',
     description='Python package for CVRP utilities',
     author='Your Name',
     author_email='jkschin@mit.edu',
     url='https://github.com/jkschin/routeml',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
@@ -14,10 +14,14 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     install_requires=[
+        "numpy",
+        "scipy",
+        "matplotlib",
+        "hygese"
         # Add any dependencies required by your package
     ],
 )
```

### Comparing `routeml-0.2.0/tests/integration/test_vrplib_cost_integration.py` & `routeml-0.3.0/tests/integration/test_vrplib_cost_integration.py`

 * *Files identical despite different names*

### Comparing `routeml-0.2.0/tests/unit/utils/test_get_cvrp_cost.py` & `routeml-0.3.0/tests/unit/utils/test_get_cvrp_cost.py`

 * *Files identical despite different names*

### Comparing `routeml-0.2.0/tests/unit/utils/test_get_is_feasible.py` & `routeml-0.3.0/tests/unit/utils/test_get_is_feasible.py`

 * *Files identical despite different names*

### Comparing `routeml-0.2.0/tests/unit/utils/test_get_route_demand.py` & `routeml-0.3.0/tests/unit/utils/test_get_route_demand.py`

 * *Files identical despite different names*

### Comparing `routeml-0.2.0/tests/unit/utils/test_parse_vrplib_file.py` & `routeml-0.3.0/tests/unit/utils/test_parse_vrplib_file.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,16 +25,17 @@
             # Perform assertions on the parsed data
             self.assertEqual(parsed_data['name'], "X-n101-k25")
             self.assertEqual(parsed_data['type'], "CVRP")
             self.assertEqual(parsed_data['dimension'], 101)
             self.assertEqual(parsed_data['edge_weight_type'], "EUC_2D")
             self.assertEqual(parsed_data['capacity'], 206)
 
-            self.assertEqual(len(parsed_data['node_coords']), 101)
-            self.assertEqual(len(parsed_data['demand']), 101)
+            self.assertEqual(parsed_data['node_coords'].shape[0], 101)
+            self.assertEqual(parsed_data['node_coords'].shape[1], 2)
+            self.assertEqual(parsed_data['demand'].shape[0], 101)
             self.assertEqual(len(parsed_data['depot_ids']), 1)
 
             # Additional assertions or validations on the parsed data
 
             print("VRPLIB file parsed successfully!")
```

### Comparing `routeml-0.2.0/tests/unit/utils/test_parse_vrplib_solution.py` & `routeml-0.3.0/tests/unit/utils/test_parse_vrplib_solution.py`

 * *Files identical despite different names*

### Comparing `routeml-0.2.0/tests/unit/utils/test_routes_to_solution.py` & `routeml-0.3.0/tests/unit/utils/test_routes_to_solution.py`

 * *Files identical despite different names*

### Comparing `routeml-0.2.0/tests/unit/utils/test_solution_to_routes.py` & `routeml-0.3.0/tests/unit/utils/test_solution_to_routes.py`

 * *Files identical despite different names*

