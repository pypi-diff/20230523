# Comparing `tmp/sbmlcore-0.2.0.tar.gz` & `tmp/sbmlcore-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbmlcore-0.2.0.tar", last modified: Tue May  9 13:33:56 2023, max compression
+gzip compressed data, was "sbmlcore-0.2.3.tar", last modified: Tue May 23 20:45:41 2023, max compression
```

## Comparing `sbmlcore-0.2.0.tar` & `sbmlcore-0.2.3.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 fowler     (503) staff       (20)        0 2023-05-09 13:33:56.780476 sbmlcore-0.2.0/
--rw-r--r--   0 fowler     (503) staff       (20)     1072 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/LICENSE
--rw-r--r--   0 fowler     (503) staff       (20)     3911 2023-05-09 13:33:56.780562 sbmlcore-0.2.0/PKG-INFO
--rw-r--r--   0 fowler     (503) staff       (20)     2939 2023-05-09 13:13:03.000000 sbmlcore-0.2.0/README.md
--rw-r--r--   0 fowler     (503) staff       (20)        6 2023-05-09 13:30:29.000000 sbmlcore-0.2.0/VERSION
--rw-r--r--   0 fowler     (503) staff       (20)      116 2023-05-09 13:29:27.000000 sbmlcore-0.2.0/pyproject.toml
-drwxr-xr-x   0 fowler     (503) staff       (20)        0 2023-05-09 13:33:56.774311 sbmlcore-0.2.0/sbmlcore/
--rw-r--r--   0 fowler     (503) staff       (20)     6161 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/sbmlcore/AminoAcidProperties.py
--rw-r--r--   0 fowler     (503) staff       (20)     3915 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/sbmlcore/DeepDDG.py
--rw-r--r--   0 fowler     (503) staff       (20)    16192 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/sbmlcore/ExternalCode.py
--rw-r--r--   0 fowler     (503) staff       (20)     2282 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/sbmlcore/FeaturesDataFrame.py
--rw-r--r--   0 fowler     (503) staff       (20)      426 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/sbmlcore/Misc.py
--rw-r--r--   0 fowler     (503) staff       (20)     3238 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/sbmlcore/RaSP.py
--rw-r--r--   0 fowler     (503) staff       (20)     2840 2023-01-06 14:07:50.000000 sbmlcore-0.2.0/sbmlcore/ResidueDepth.py
--rw-r--r--   0 fowler     (503) staff       (20)     6194 2022-10-05 09:39:59.000000 sbmlcore-0.2.0/sbmlcore/StructuralDistances.py
--rw-r--r--   0 fowler     (503) staff       (20)     3791 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/sbmlcore/TempFactors.py
--rw-r--r--   0 fowler     (503) staff       (20)    17544 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/sbmlcore/TrajectoryDihedrals.py
--rw-r--r--   0 fowler     (503) staff       (20)     9895 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/sbmlcore/TrajectoryDistances.py
--rw-r--r--   0 fowler     (503) staff       (20)     1207 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/sbmlcore/__init__.py
-drwxr-xr-x   0 fowler     (503) staff       (20)        0 2023-05-09 13:33:56.775076 sbmlcore-0.2.0/sbmlcore.egg-info/
--rw-r--r--   0 fowler     (503) staff       (20)     3911 2023-05-09 13:33:56.000000 sbmlcore-0.2.0/sbmlcore.egg-info/PKG-INFO
--rw-r--r--   0 fowler     (503) staff       (20)      935 2023-05-09 13:33:56.000000 sbmlcore-0.2.0/sbmlcore.egg-info/SOURCES.txt
--rw-r--r--   0 fowler     (503) staff       (20)        1 2023-05-09 13:33:56.000000 sbmlcore-0.2.0/sbmlcore.egg-info/dependency_links.txt
--rw-r--r--   0 fowler     (503) staff       (20)       55 2023-05-09 13:33:56.000000 sbmlcore-0.2.0/sbmlcore.egg-info/requires.txt
--rw-r--r--   0 fowler     (503) staff       (20)        9 2023-05-09 13:33:56.000000 sbmlcore-0.2.0/sbmlcore.egg-info/top_level.txt
--rw-r--r--   0 fowler     (503) staff       (20)     1119 2023-05-09 13:33:56.780935 sbmlcore-0.2.0/setup.cfg
-drwxr-xr-x   0 fowler     (503) staff       (20)        0 2023-05-09 13:33:56.780327 sbmlcore-0.2.0/tests/
--rw-r--r--   0 fowler     (503) staff       (20)      234 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_MDAnalysis.py
--rw-r--r--   0 fowler     (503) staff       (20)      753 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_MW.py
--rw-r--r--   0 fowler     (503) staff       (20)      757 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_Pi.py
--rw-r--r--   0 fowler     (503) staff       (20)      786 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_aminoacidvolumechange.py
--rw-r--r--   0 fowler     (503) staff       (20)     3807 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_deep_ddg.py
--rw-r--r--   0 fowler     (503) staff       (20)     1201 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_dssp.py
--rw-r--r--   0 fowler     (503) staff       (20)     2412 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_freesasa.py
--rw-r--r--   0 fowler     (503) staff       (20)     1617 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_hydropathy.py
--rw-r--r--   0 fowler     (503) staff       (20)      677 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_rasp.py
--rw-r--r--   0 fowler     (503) staff       (20)      330 2023-01-06 15:36:46.000000 sbmlcore-0.2.0/tests/test_residuedepth.py
--rw-r--r--   0 fowler     (503) staff       (20)      349 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_rogov.py
--rw-r--r--   0 fowler     (503) staff       (20)     1916 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_snap2.py
--rw-r--r--   0 fowler     (503) staff       (20)     1168 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_stride.py
--rw-r--r--   0 fowler     (503) staff       (20)     2782 2023-05-09 13:20:53.000000 sbmlcore-0.2.0/tests/test_structuraldistances.py
--rw-r--r--   0 fowler     (503) staff       (20)      665 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_tempfactor.py
--rw-r--r--   0 fowler     (503) staff       (20)     9512 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_trajectorydihedrals.py
--rw-r--r--   0 fowler     (503) staff       (20)     6544 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_trajectorydistances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:45:41.492861 sbmlcore-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-23 20:45:41.492861 sbmlcore-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:45:41.484861 sbmlcore-0.2.3/sbmlcore/
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/sbmlcore/AminoAcidProperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/sbmlcore/DeepDDG.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/sbmlcore/ExternalCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/sbmlcore/FeaturesDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/sbmlcore/Misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/sbmlcore/RaSP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/sbmlcore/ResidueDepth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/sbmlcore/StructuralDistances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/sbmlcore/TempFactors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/sbmlcore/TrajectoryDihedrals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/sbmlcore/TrajectoryDistances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/sbmlcore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:45:41.488861 sbmlcore-0.2.3/sbmlcore/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/sbmlcore/data/rogov.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:45:41.488861 sbmlcore-0.2.3/sbmlcore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-23 20:45:41.000000 sbmlcore-0.2.3/sbmlcore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-23 20:45:41.000000 sbmlcore-0.2.3/sbmlcore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:45:41.000000 sbmlcore-0.2.3/sbmlcore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-23 20:45:41.000000 sbmlcore-0.2.3/sbmlcore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 20:45:41.000000 sbmlcore-0.2.3/sbmlcore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-23 20:45:41.492861 sbmlcore-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:45:41.492861 sbmlcore-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/tests/test_MDAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/tests/test_MW.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/tests/test_Pi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/tests/test_aminoacidvolumechange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/tests/test_deep_ddg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/tests/test_dssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/tests/test_freesasa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/tests/test_hydropathy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/tests/test_rasp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/tests/test_residuedepth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/tests/test_rogov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/tests/test_snap2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/tests/test_stride.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/tests/test_structuraldistances.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/tests/test_tempfactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/tests/test_trajectorydihedrals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-05-23 20:42:36.000000 sbmlcore-0.2.3/tests/test_trajectorydistances.py
```

### Comparing `sbmlcore-0.2.0/LICENSE` & `sbmlcore-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/PKG-INFO` & `sbmlcore-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbmlcore
-Version: 0.2.0
+Version: 0.2.3
 Summary: Constructs core features table for the application to machine learning models
 Home-page: https://github.com/fowler-lab/sbmlcore
 Author: Philip W Fowler and Charlotte I Lynch and Dylan Adlard
 Author-email: philip.fowler@ndm.ox.ac.uk
 License: MIT
 Project-URL: Documentation, https://github.com/fowler-lab/sbmlcore
 Project-URL: CI, https://github.com/fowler-lab/sbmlcore/actions
```

### Comparing `sbmlcore-0.2.0/README.md` & `sbmlcore-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/sbmlcore/AminoAcidProperties.py` & `sbmlcore-0.2.3/sbmlcore/AminoAcidProperties.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/sbmlcore/DeepDDG.py` & `sbmlcore-0.2.3/sbmlcore/DeepDDG.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/sbmlcore/ExternalCode.py` & `sbmlcore-0.2.3/sbmlcore/ExternalCode.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/sbmlcore/FeaturesDataFrame.py` & `sbmlcore-0.2.3/sbmlcore/FeaturesDataFrame.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/sbmlcore/RaSP.py` & `sbmlcore-0.2.3/sbmlcore/RaSP.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/sbmlcore/ResidueDepth.py` & `sbmlcore-0.2.3/sbmlcore/ResidueDepth.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/sbmlcore/StructuralDistances.py` & `sbmlcore-0.2.3/sbmlcore/StructuralDistances.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/sbmlcore/TempFactors.py` & `sbmlcore-0.2.3/sbmlcore/TempFactors.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/sbmlcore/TrajectoryDihedrals.py` & `sbmlcore-0.2.3/sbmlcore/TrajectoryDihedrals.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/sbmlcore/TrajectoryDistances.py` & `sbmlcore-0.2.3/sbmlcore/TrajectoryDistances.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/sbmlcore/__init__.py` & `sbmlcore-0.2.3/sbmlcore/__init__.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/sbmlcore.egg-info/PKG-INFO` & `sbmlcore-0.2.3/sbmlcore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbmlcore
-Version: 0.2.0
+Version: 0.2.3
 Summary: Constructs core features table for the application to machine learning models
 Home-page: https://github.com/fowler-lab/sbmlcore
 Author: Philip W Fowler and Charlotte I Lynch and Dylan Adlard
 Author-email: philip.fowler@ndm.ox.ac.uk
 License: MIT
 Project-URL: Documentation, https://github.com/fowler-lab/sbmlcore
 Project-URL: CI, https://github.com/fowler-lab/sbmlcore/actions
```

### Comparing `sbmlcore-0.2.0/sbmlcore.egg-info/SOURCES.txt` & `sbmlcore-0.2.3/sbmlcore.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 sbmlcore/TrajectoryDistances.py
 sbmlcore/__init__.py
 sbmlcore.egg-info/PKG-INFO
 sbmlcore.egg-info/SOURCES.txt
 sbmlcore.egg-info/dependency_links.txt
 sbmlcore.egg-info/requires.txt
 sbmlcore.egg-info/top_level.txt
+sbmlcore/data/rogov.csv
 tests/test_MDAnalysis.py
 tests/test_MW.py
 tests/test_Pi.py
 tests/test_aminoacidvolumechange.py
 tests/test_deep_ddg.py
 tests/test_dssp.py
 tests/test_freesasa.py
```

### Comparing `sbmlcore-0.2.0/setup.cfg` & `sbmlcore-0.2.3/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -32,11 +32,14 @@
 	pandas
 	MDAnalysis
 	freesasa
 	pytest
 	pytest-cov
 	BioPython
 
+[options.package_data]
+sbmlcore = data/*csv
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sbmlcore-0.2.0/tests/test_MW.py` & `sbmlcore-0.2.3/tests/test_MW.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/tests/test_Pi.py` & `sbmlcore-0.2.3/tests/test_Pi.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/tests/test_aminoacidvolumechange.py` & `sbmlcore-0.2.3/tests/test_aminoacidvolumechange.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/tests/test_deep_ddg.py` & `sbmlcore-0.2.3/tests/test_deep_ddg.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/tests/test_dssp.py` & `sbmlcore-0.2.3/tests/test_dssp.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/tests/test_freesasa.py` & `sbmlcore-0.2.3/tests/test_freesasa.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/tests/test_hydropathy.py` & `sbmlcore-0.2.3/tests/test_hydropathy.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/tests/test_rasp.py` & `sbmlcore-0.2.3/tests/test_rasp.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/tests/test_snap2.py` & `sbmlcore-0.2.3/tests/test_snap2.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/tests/test_stride.py` & `sbmlcore-0.2.3/tests/test_stride.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/tests/test_structuraldistances.py` & `sbmlcore-0.2.3/tests/test_structuraldistances.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/tests/test_tempfactor.py` & `sbmlcore-0.2.3/tests/test_tempfactor.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/tests/test_trajectorydihedrals.py` & `sbmlcore-0.2.3/tests/test_trajectorydihedrals.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.2.0/tests/test_trajectorydistances.py` & `sbmlcore-0.2.3/tests/test_trajectorydistances.py`

 * *Files identical despite different names*

