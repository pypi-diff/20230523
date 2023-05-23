# Comparing `tmp/LasBuildSeg-0.1.19.tar.gz` & `tmp/LasBuildSeg-0.1.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LasBuildSeg-0.1.19.tar", last modified: Mon May 22 16:39:47 2023, max compression
+gzip compressed data, was "LasBuildSeg-0.1.20.tar", last modified: Tue May 23 07:46:00 2023, max compression
```

## Comparing `LasBuildSeg-0.1.19.tar` & `LasBuildSeg-0.1.20.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 16:39:47.020337 LasBuildSeg-0.1.19/
--rw-rw-rw-   0        0        0      149 2023-05-22 16:37:51.000000 LasBuildSeg-0.1.19/CHANGELOG.txt
--rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.1.19/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-05-22 16:39:46.965520 LasBuildSeg-0.1.19/LasBuildSeg/
-drwxrwxrwx   0        0        0        0 2023-05-22 16:39:47.014364 LasBuildSeg-0.1.19/LasBuildSeg/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0    11872 2023-05-10 09:29:06.000000 LasBuildSeg-0.1.19/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py
--rw-rw-rw-   0        0        0    15767 2023-05-22 16:38:43.000000 LasBuildSeg-0.1.19/LasBuildSeg/LasBuildSeg.py
--rw-rw-rw-   0        0        0      519 2023-05-22 16:07:43.000000 LasBuildSeg-0.1.19/LasBuildSeg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:39:47.010370 LasBuildSeg-0.1.19/LasBuildSeg.egg-info/
--rw-rw-rw-   0        0        0     3076 2023-05-22 16:39:45.000000 LasBuildSeg-0.1.19/LasBuildSeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-05-22 16:39:46.000000 LasBuildSeg-0.1.19/LasBuildSeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 16:39:45.000000 LasBuildSeg-0.1.19/LasBuildSeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-05-22 16:39:45.000000 LasBuildSeg-0.1.19/LasBuildSeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-22 16:39:45.000000 LasBuildSeg-0.1.19/LasBuildSeg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       51 2023-05-10 09:31:40.000000 LasBuildSeg-0.1.19/MANIFEST.in
--rw-rw-rw-   0        0        0     3076 2023-05-22 16:39:47.017354 LasBuildSeg-0.1.19/PKG-INFO
--rw-rw-rw-   0        0        0     2146 2023-05-22 16:39:08.000000 LasBuildSeg-0.1.19/README.md
--rw-rw-rw-   0        0        0     1496 2023-05-22 16:37:57.000000 LasBuildSeg-0.1.19/Setup.py
--rw-rw-rw-   0        0        0      123 2023-05-17 11:16:46.000000 LasBuildSeg-0.1.19/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 16:39:47.021333 LasBuildSeg-0.1.19/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 07:46:00.212826 LasBuildSeg-0.1.20/
+-rw-rw-rw-   0        0        0      109 2023-05-23 07:44:56.000000 LasBuildSeg-0.1.20/CHANGELOG.txt
+-rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.1.20/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 07:46:00.105736 LasBuildSeg-0.1.20/LasBuildSeg/
+drwxrwxrwx   0        0        0        0 2023-05-23 07:46:00.205849 LasBuildSeg-0.1.20/LasBuildSeg/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0    11872 2023-05-10 09:29:06.000000 LasBuildSeg-0.1.20/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py
+-rw-rw-rw-   0        0        0    15745 2023-05-23 07:44:15.000000 LasBuildSeg-0.1.20/LasBuildSeg/LasBuildSeg.py
+-rw-rw-rw-   0        0        0      519 2023-05-22 16:07:43.000000 LasBuildSeg-0.1.20/LasBuildSeg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:46:00.174959 LasBuildSeg-0.1.20/LasBuildSeg.egg-info/
+-rw-rw-rw-   0        0        0     3076 2023-05-23 07:45:58.000000 LasBuildSeg-0.1.20/LasBuildSeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-05-23 07:45:59.000000 LasBuildSeg-0.1.20/LasBuildSeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 07:45:58.000000 LasBuildSeg-0.1.20/LasBuildSeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-05-23 07:45:58.000000 LasBuildSeg-0.1.20/LasBuildSeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-23 07:45:58.000000 LasBuildSeg-0.1.20/LasBuildSeg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       51 2023-05-10 09:31:40.000000 LasBuildSeg-0.1.20/MANIFEST.in
+-rw-rw-rw-   0        0        0     3076 2023-05-23 07:46:00.210832 LasBuildSeg-0.1.20/PKG-INFO
+-rw-rw-rw-   0        0        0     2146 2023-05-22 16:39:08.000000 LasBuildSeg-0.1.20/README.md
+-rw-rw-rw-   0        0        0     1496 2023-05-23 07:44:55.000000 LasBuildSeg-0.1.20/Setup.py
+-rw-rw-rw-   0        0        0      123 2023-05-17 11:16:46.000000 LasBuildSeg-0.1.20/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 07:46:00.213824 LasBuildSeg-0.1.20/setup.cfg
```

### Comparing `LasBuildSeg-0.1.19/LICENSE.txt` & `LasBuildSeg-0.1.20/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.19/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py` & `LasBuildSeg-0.1.20/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.19/LasBuildSeg/LasBuildSeg.py` & `LasBuildSeg-0.1.20/LasBuildSeg/LasBuildSeg.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,19 +118,19 @@
     mesh_x, mesh_y = np.meshgrid(np.arange(min_x, max_x, resolution), np.arange(min_y, max_y, resolution))
 
     # Interpolate the z values of the ground points onto the mesh grid
     ground_values = ground_tree.query(np.vstack((mesh_x.ravel(), mesh_y.ravel())).T)[0]
     mesh_z = ground_values.reshape(mesh_x.shape)
 
     # Load the point cloud
-    dsm_data = laspy.read('updated_file.las')
-    dsm_points = np.vstack((dsm_data.x, dsm_data.y, dsm_data.z)).T
+    dtm_data = las_data
+    dtm_points = np.vstack((dtm_data.x, dtm_data.y, dtm_data.z)).T
 
     # Classify points as non-ground (not class 2)
-    non_ground_points = dsm_points[dsm_data.classification != 2]
+    non_ground_points = dtm_points[dtm_data.classification != 2]
 
     # Interpolate the non-ground points onto the mesh grid
     non_ground_z = griddata(non_ground_points[:, :2], non_ground_points[:, 2], (mesh_x, mesh_y), method=interpolation_method)
 
     # Subtract the interpolated non-ground values from the interpolated ground values also enhancge the contrast by using ground_multiplier
     dtm = ground_multiplier * mesh_z - non_ground_z
```

### Comparing `LasBuildSeg-0.1.19/LasBuildSeg/__init__.py` & `LasBuildSeg-0.1.20/LasBuildSeg/__init__.py`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.19/LasBuildSeg.egg-info/PKG-INFO` & `LasBuildSeg-0.1.20/LasBuildSeg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.1.19
+Version: 0.1.20
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `LasBuildSeg-0.1.19/PKG-INFO` & `LasBuildSeg-0.1.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.1.19
+Version: 0.1.20
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `LasBuildSeg-0.1.19/README.md` & `LasBuildSeg-0.1.20/README.md`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.19/Setup.py` & `LasBuildSeg-0.1.20/Setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     INSTALL_REQUIRES = []
 else:
     with open("requirements.txt") as f:
         INSTALL_REQUIRES = [line.strip() for line in f.readlines()]
         
 setup(
   name='LasBuildSeg',
-  version='0.1.19',
+  version='0.1.20',
   description='Building Footrprint Extraction from Aerial LiDAR data',
   long_description=long_description,
   long_description_content_type='text/markdown',  
   url='',  
   author='MertcanErdem',
   author_email='merak908@gmail.com',
   license='GNU General Public License v2.0',
```

