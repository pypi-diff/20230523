# Comparing `tmp/Signal8-1.7.tar.gz` & `tmp/Signal8-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-1.7.tar", last modified: Fri May 19 20:00:02 2023, max compression
+gzip compressed data, was "Signal8-1.8.tar", last modified: Mon May 22 23:15:27 2023, max compression
```

## Comparing `Signal8-1.7.tar` & `Signal8-1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 20:00:02.033506 Signal8-1.7/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-1.7/LICENSE
--rw-rw-rw-   0        0        0     4364 2023-05-19 20:00:02.032508 Signal8-1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3876 2023-05-19 19:25:10.000000 Signal8-1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 20:00:01.972507 Signal8-1.7/Signal8/
--rw-rw-rw-   0        0        0     6519 2023-05-19 19:59:38.000000 Signal8-1.7/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-1.7/Signal8/__init__.py
--rw-rw-rw-   0        0        0      130 2023-05-19 19:25:12.000000 Signal8-1.7/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-05-19 20:00:02.027544 Signal8-1.7/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-1.7/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     7867 2023-05-19 19:40:29.000000 Signal8-1.7/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2423 2023-05-19 19:25:16.000000 Signal8-1.7/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-1.7/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12174 2023-05-19 19:30:46.000000 Signal8-1.7/Signal8/utils/simple_env.py
-drwxrwxrwx   0        0        0        0 2023-05-19 20:00:02.001507 Signal8-1.7/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4364 2023-05-19 20:00:01.000000 Signal8-1.7/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-05-19 20:00:01.000000 Signal8-1.7/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 20:00:01.000000 Signal8-1.7/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-19 20:00:01.000000 Signal8-1.7/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 20:00:02.034507 Signal8-1.7/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-05-19 19:59:53.000000 Signal8-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 23:15:19.644830 Signal8-1.8/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-1.8/LICENSE
+-rw-rw-rw-   0        0        0     4356 2023-05-22 23:15:27.502308 Signal8-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3868 2023-05-22 23:14:08.000000 Signal8-1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 23:15:19.570831 Signal8-1.8/Signal8/
+-rw-rw-rw-   0        0        0     6519 2023-05-19 19:59:38.000000 Signal8-1.8/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-1.8/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      130 2023-05-19 19:25:12.000000 Signal8-1.8/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-05-22 23:15:19.631832 Signal8-1.8/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-1.8/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     7867 2023-05-19 19:40:29.000000 Signal8-1.8/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2407 2023-05-22 23:12:51.000000 Signal8-1.8/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-1.8/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12174 2023-05-19 19:30:46.000000 Signal8-1.8/Signal8/utils/simple_env.py
+drwxrwxrwx   0        0        0        0 2023-05-22 23:15:27.490306 Signal8-1.8/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4356 2023-05-22 23:15:27.000000 Signal8-1.8/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-05-22 23:15:27.000000 Signal8-1.8/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 23:15:27.000000 Signal8-1.8/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-22 23:15:27.000000 Signal8-1.8/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 23:15:27.513305 Signal8-1.8/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-05-22 23:14:59.000000 Signal8-1.8/setup.py
```

### Comparing `Signal8-1.7/LICENSE` & `Signal8-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-1.7/PKG-INFO` & `Signal8-1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 1.7
+Version: 1.8
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
@@ -35,23 +35,23 @@
 env = Signal8.env(dynamic_obstacles=True)
 env.reset(options={"problem_name": "v_cluster"}))
 ```
 
 ## List of Problem Scenarios
 
 |     Names     | Description                                                                                                                                                                                          |
-| :------------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-|  `Cluster`  | The environment features a central square formed by four obstacles, with the start on the left and the goal on the right side.                                                                       |
-|  `L-Shaped`  | The environment showcases a central L-shaped configuration of four obstacles, with the starting point on the left boundary and the goal situated at the inner elbow of the L.                        |
-|  `Vertical`  | Four obstacles are aligned vertically in the environment's center, with the starting point on the left boundary and the goal on the right boundary.                                                  |
-| `Horizontal` | Four obstacles are arranged in a horizontal line at the environment's midsection, with the start on the left boundary and the goal on the right boundary.                                            |
-|    `Top`    | Four obstacles are placed at the top of the environment, while the start is situated in the bottom half on the left boundary and the goal is in the bottom half on the right boundary.               |
-|   `Bottom`   | Four obstacles are placed at the bottom of the environment, while the start is situated in the topÂ half on the left boundary and the goal is in the top half on the right boundary.                 |
-|   `Right`   | Four obstacles are situated on the right side of the environment, with the start positioned in the left half along the bottom boundary and the goal located in the left half along the top boundary. |
-|    `Left`    | Four obstacles are situated on the left side of the environment, with the start positioned in the right half along the bottom boundary and the goal located in the left half along the top boundary. |
+| :-----------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `v_cluster` | The environment features a central square formed by four obstacles, with the start on the left and the goal on the right side.                                                                       |
+| ``h_cluster`` | The environment showcases a central L-shaped configuration of four obstacles, with the starting point on the left boundary and the goal situated at the inner elbow of the L.                        |
+|  `v_wall`  | Four obstacles are aligned vertically in the environment's center, with the starting point on the left boundary and the goal on the right boundary.                                                  |
+|  `h_wall`  | Four obstacles are arranged in a horizontal line at the environment's midsection, with the start on the left boundary and the goal on the right boundary.                                            |
+|    `top`    | Four obstacles are placed at the top of the environment, while the start is situated in the bottom half on the left boundary and the goal is in the bottom half on the right boundary.               |
+|  `bottom`  | Four obstacles are placed at the bottom of the environment, while the start is situated in the topÂ half on the left boundary and the goal is in the top half on the right boundary.                 |
+|   `right`   | Four obstacles are situated on the right side of the environment, with the start positioned in the left half along the bottom boundary and the goal located in the left half along the top boundary. |
+|   `left`   | Four obstacles are situated on the left side of the environment, with the start positioned in the right half along the bottom boundary and the goal located in the left half along the top boundary. |
 
 ## Paper Citation
 
 If you used this environment for your experiments or found it helpful, consider citing the following papers:
 
 Environments in this repo:
```

### Comparing `Signal8-1.7/README.md` & `Signal8-1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,23 +23,23 @@
 env = Signal8.env(dynamic_obstacles=True)
 env.reset(options={"problem_name": "v_cluster"}))
 ```
 
 ## List of Problem Scenarios
 
 |     Names     | Description                                                                                                                                                                                          |
-| :------------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-|  `Cluster`  | The environment features a central square formed by four obstacles, with the start on the left and the goal on the right side.                                                                       |
-|  `L-Shaped`  | The environment showcases a central L-shaped configuration of four obstacles, with the starting point on the left boundary and the goal situated at the inner elbow of the L.                        |
-|  `Vertical`  | Four obstacles are aligned vertically in the environment's center, with the starting point on the left boundary and the goal on the right boundary.                                                  |
-| `Horizontal` | Four obstacles are arranged in a horizontal line at the environment's midsection, with the start on the left boundary and the goal on the right boundary.                                            |
-|    `Top`    | Four obstacles are placed at the top of the environment, while the start is situated in the bottom half on the left boundary and the goal is in the bottom half on the right boundary.               |
-|   `Bottom`   | Four obstacles are placed at the bottom of the environment, while the start is situated in the top half on the left boundary and the goal is in the top half on the right boundary.                 |
-|   `Right`   | Four obstacles are situated on the right side of the environment, with the start positioned in the left half along the bottom boundary and the goal located in the left half along the top boundary. |
-|    `Left`    | Four obstacles are situated on the left side of the environment, with the start positioned in the right half along the bottom boundary and the goal located in the left half along the top boundary. |
+| :-----------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `v_cluster` | The environment features a central square formed by four obstacles, with the start on the left and the goal on the right side.                                                                       |
+| ``h_cluster`` | The environment showcases a central L-shaped configuration of four obstacles, with the starting point on the left boundary and the goal situated at the inner elbow of the L.                        |
+|  `v_wall`  | Four obstacles are aligned vertically in the environment's center, with the starting point on the left boundary and the goal on the right boundary.                                                  |
+|  `h_wall`  | Four obstacles are arranged in a horizontal line at the environment's midsection, with the start on the left boundary and the goal on the right boundary.                                            |
+|    `top`    | Four obstacles are placed at the top of the environment, while the start is situated in the bottom half on the left boundary and the goal is in the bottom half on the right boundary.               |
+|  `bottom`  | Four obstacles are placed at the bottom of the environment, while the start is situated in the top half on the left boundary and the goal is in the top half on the right boundary.                 |
+|   `right`   | Four obstacles are situated on the right side of the environment, with the start positioned in the left half along the bottom boundary and the goal located in the left half along the top boundary. |
+|   `left`   | Four obstacles are situated on the left side of the environment, with the start positioned in the right half along the bottom boundary and the goal located in the left half along the top boundary. |
 
 ## Paper Citation
 
 If you used this environment for your experiments or found it helpful, consider citing the following papers:
 
 Environments in this repo:
```

### Comparing `Signal8-1.7/Signal8/Signal8.py` & `Signal8-1.8/Signal8/Signal8.py`

 * *Files identical despite different names*

### Comparing `Signal8-1.7/Signal8/utils/core.py` & `Signal8-1.8/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-1.7/Signal8/utils/problems.py` & `Signal8-1.8/Signal8/utils/problems.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,20 +45,20 @@
     return list(problems.keys())
 
 def get_problem(scenario_name, dynamic_obstacles):
     static_scenario = problems[scenario_name]
     
     if dynamic_obstacles:
         dynamic_elements = {
-            'v_cluster': {'dynamic_obs': (((-1, 1), (-0.5, -0.35)), ((-1, 1), (0.35, 0.5)))},
-            'h_cluster': {'dynamic_obs': (((-0.5, -0.35), (-1, 1)), ((0.35, 0.5), (-1, 1)))},
-            'v_wall': {'dynamic_obs': (((-1, 1), (-0.25, -0.075)), ((-1, 1), (0.075, 0.25)))},
-            'h_wall': {'dynamic_obs': (((-0.25, -0.075), (-1, 1)), ((0.075, 0.25), (-1, 1)))},
-            'left': {'dynamic_obs': (((-1, 0.5), (-0.45, -0.55)), ((-1, 0.5), (0.45, 0.55)))},
-            'right': {'dynamic_obs': (((-0.5, 1), (-0.45, -0.55)), ((-0.5, 1), (0.45, 0.55)))},
-            'top': {'dynamic_obs': (((-0.45, -0.55), (-0.5, 1)), ((0.45, 0.55), (-0.5, 1)))},
-            'bottom': {'dynamic_obs': (((-0.45, -0.55), (-1, 0.5)), ((0.45, 0.55), (-1, 0.5)))},
+            'v_cluster': {'dynamic_obs': (((-1, 1), (-0.45, -0.40)), ((-1, 1), (0.40, 0.45)))},
+            'h_cluster': {'dynamic_obs': (((-0.45, -0.40), (-1, 1)), ((0.40, 0.45), (-1, 1)))},
+            'v_wall': {'dynamic_obs': (((-1, 1), (-0.25, -0.20)), ((-1, 1), (0.20, 0.25)))},
+            'h_wall': {'dynamic_obs': (((-0.45, -0.40), (-1, 1)), ((0.40, 0.45), (-1, 1)))},
+            'left': {'dynamic_obs': (((-1, 1), (-0.40, -0.45)), ((-1, 1), (0.40, 0.45)))},
+            'right': {'dynamic_obs': (((-1, 1), (-0.40, -0.45)), ((-1, 1), (0.40, 0.45)))},
+            'top': {'dynamic_obs': (((-0.40, -0.45), (-1, 1)), ((0.40, 0.45), (-1, 1)))},
+            'bottom': {'dynamic_obs': (((-0.40, -0.45), (-1, 1)), ((0.40, 0.45), (-1, 1)))},
         }
         dynamic_scenario = {**static_scenario, **dynamic_elements[scenario_name]}
         return dynamic_scenario
         
     return static_scenario
```

### Comparing `Signal8-1.7/Signal8/utils/simple_env.py` & `Signal8-1.8/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-1.7/Signal8.egg-info/PKG-INFO` & `Signal8-1.8/Signal8.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 1.7
+Version: 1.8
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
@@ -35,23 +35,23 @@
 env = Signal8.env(dynamic_obstacles=True)
 env.reset(options={"problem_name": "v_cluster"}))
 ```
 
 ## List of Problem Scenarios
 
 |     Names     | Description                                                                                                                                                                                          |
-| :------------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-|  `Cluster`  | The environment features a central square formed by four obstacles, with the start on the left and the goal on the right side.                                                                       |
-|  `L-Shaped`  | The environment showcases a central L-shaped configuration of four obstacles, with the starting point on the left boundary and the goal situated at the inner elbow of the L.                        |
-|  `Vertical`  | Four obstacles are aligned vertically in the environment's center, with the starting point on the left boundary and the goal on the right boundary.                                                  |
-| `Horizontal` | Four obstacles are arranged in a horizontal line at the environment's midsection, with the start on the left boundary and the goal on the right boundary.                                            |
-|    `Top`    | Four obstacles are placed at the top of the environment, while the start is situated in the bottom half on the left boundary and the goal is in the bottom half on the right boundary.               |
-|   `Bottom`   | Four obstacles are placed at the bottom of the environment, while the start is situated in the topÂ half on the left boundary and the goal is in the top half on the right boundary.                 |
-|   `Right`   | Four obstacles are situated on the right side of the environment, with the start positioned in the left half along the bottom boundary and the goal located in the left half along the top boundary. |
-|    `Left`    | Four obstacles are situated on the left side of the environment, with the start positioned in the right half along the bottom boundary and the goal located in the left half along the top boundary. |
+| :-----------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `v_cluster` | The environment features a central square formed by four obstacles, with the start on the left and the goal on the right side.                                                                       |
+| ``h_cluster`` | The environment showcases a central L-shaped configuration of four obstacles, with the starting point on the left boundary and the goal situated at the inner elbow of the L.                        |
+|  `v_wall`  | Four obstacles are aligned vertically in the environment's center, with the starting point on the left boundary and the goal on the right boundary.                                                  |
+|  `h_wall`  | Four obstacles are arranged in a horizontal line at the environment's midsection, with the start on the left boundary and the goal on the right boundary.                                            |
+|    `top`    | Four obstacles are placed at the top of the environment, while the start is situated in the bottom half on the left boundary and the goal is in the bottom half on the right boundary.               |
+|  `bottom`  | Four obstacles are placed at the bottom of the environment, while the start is situated in the topÂ half on the left boundary and the goal is in the top half on the right boundary.                 |
+|   `right`   | Four obstacles are situated on the right side of the environment, with the start positioned in the left half along the bottom boundary and the goal located in the left half along the top boundary. |
+|   `left`   | Four obstacles are situated on the left side of the environment, with the start positioned in the right half along the bottom boundary and the goal located in the left half along the top boundary. |
 
 ## Paper Citation
 
 If you used this environment for your experiments or found it helpful, consider citing the following papers:
 
 Environments in this repo:
```

### Comparing `Signal8-1.7/setup.py` & `Signal8-1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="1.7",
+    version="1.8",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

