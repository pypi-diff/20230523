# Comparing `tmp/bio-aid-0.2.2.tar.gz` & `tmp/bio-aid-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio-aid-0.2.2.tar", last modified: Tue Apr 25 21:36:29 2023, max compression
+gzip compressed data, was "bio-aid-0.3.0.tar", last modified: Tue May 23 20:58:31 2023, max compression
```

## Comparing `bio-aid-0.2.2.tar` & `bio-aid-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 21:36:29.083058 bio-aid-0.2.2/
-drwxrwxrwx   0        0        0        0 2023-04-25 21:36:29.057922 bio-aid-0.2.2/BioAid/
--rw-rw-rw-   0        0        0     2304 2023-04-25 21:07:27.000000 bio-aid-0.2.2/BioAid/Kmers.py
-drwxrwxrwx   0        0        0        0 2023-04-25 21:36:29.057922 bio-aid-0.2.2/BioAid/MMBSearchTK/
--rw-rw-rw-   0        0        0     7151 2023-03-01 22:48:52.000000 bio-aid-0.2.2/BioAid/MMBSearchTK/AnnoMMBS.py
--rw-rw-rw-   0        0        0      269 2023-03-01 22:48:19.000000 bio-aid-0.2.2/BioAid/MMBSearchTK/__init__.py
--rw-rw-rw-   0        0        0     1372 2023-03-01 22:49:16.000000 bio-aid-0.2.2/BioAid/MMBSearchTK/makeMMBSearchRef.py
--rw-rw-rw-   0        0        0      500 2023-03-01 22:45:30.000000 bio-aid-0.2.2/BioAid/__init__.py
--rw-rw-rw-   0        0        0     6676 2023-04-25 21:18:57.000000 bio-aid-0.2.2/BioAid/base.py
--rw-rw-rw-   0        0        0     4862 2023-03-01 22:41:08.000000 bio-aid-0.2.2/BioAid/complexity.py
-drwxrwxrwx   0        0        0        0 2023-04-25 21:36:29.066109 bio-aid-0.2.2/BioAid/deepSeqInsH/
--rw-rw-rw-   0        0        0      193 2023-03-01 22:49:33.000000 bio-aid-0.2.2/BioAid/deepSeqInsH/__init__.py
--rw-rw-rw-   0        0        0     2693 2023-04-25 21:33:33.000000 bio-aid-0.2.2/BioAid/deepSeqInsH/annoInsH.py
--rw-rw-rw-   0        0        0     1505 2023-04-25 21:06:56.000000 bio-aid-0.2.2/BioAid/diluter.py
--rw-rw-rw-   0        0        0     1202 2023-03-01 22:53:18.000000 bio-aid-0.2.2/BioAid/makeMMBSearchRef.py
--rw-rw-rw-   0        0        0     2062 2023-04-25 21:08:23.000000 bio-aid-0.2.2/BioAid/paralleltools.py
--rw-rw-rw-   0        0        0      870 2023-03-01 22:43:38.000000 bio-aid-0.2.2/BioAid/popDub.py
--rw-rw-rw-   0        0        0     5169 2023-03-01 22:44:42.000000 bio-aid-0.2.2/BioAid/repeatSearch.py
-drwxrwxrwx   0        0        0        0 2023-04-25 21:36:29.066248 bio-aid-0.2.2/BioAid/variantTK/
--rw-rw-rw-   0        0        0      193 2023-03-01 22:45:37.000000 bio-aid-0.2.2/BioAid/variantTK/__init__.py
--rw-rw-rw-   0        0        0    10973 2023-03-01 22:48:01.000000 bio-aid-0.2.2/BioAid/variantTK/variants.py
--rw-rw-rw-   0        0        0     1101 2023-03-01 22:53:18.000000 bio-aid-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      612 2023-04-25 21:36:29.083058 bio-aid-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3164 2023-03-01 22:53:18.000000 bio-aid-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 21:36:29.083058 bio-aid-0.2.2/bio_aid.egg-info/
--rw-rw-rw-   0        0        0      612 2023-04-25 21:36:28.000000 bio-aid-0.2.2/bio_aid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2023-04-25 21:36:28.000000 bio-aid-0.2.2/bio_aid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 21:36:28.000000 bio-aid-0.2.2/bio_aid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-25 21:36:28.000000 bio-aid-0.2.2/bio_aid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-25 21:36:28.000000 bio-aid-0.2.2/bio_aid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 21:36:29.083058 bio-aid-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      994 2023-04-25 21:36:07.000000 bio-aid-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 20:58:31.626261 bio-aid-0.3.0/
+drwxrwxrwx   0        0        0        0 2023-05-23 20:58:31.597419 bio-aid-0.3.0/BioAid/
+-rw-rw-rw-   0        0        0     3178 2023-05-23 20:54:59.000000 bio-aid-0.3.0/BioAid/Kmers.py
+drwxrwxrwx   0        0        0        0 2023-05-23 20:58:31.597419 bio-aid-0.3.0/BioAid/MMBSearchTK/
+-rw-rw-rw-   0        0        0     7151 2023-03-01 22:48:52.000000 bio-aid-0.3.0/BioAid/MMBSearchTK/AnnoMMBS.py
+-rw-rw-rw-   0        0        0      269 2023-03-01 22:48:19.000000 bio-aid-0.3.0/BioAid/MMBSearchTK/__init__.py
+-rw-rw-rw-   0        0        0     1372 2023-03-01 22:49:16.000000 bio-aid-0.3.0/BioAid/MMBSearchTK/makeMMBSearchRef.py
+-rw-rw-rw-   0        0        0      500 2023-03-01 22:45:30.000000 bio-aid-0.3.0/BioAid/__init__.py
+-rw-rw-rw-   0        0        0    10755 2023-05-23 19:48:02.000000 bio-aid-0.3.0/BioAid/base.py
+-rw-rw-rw-   0        0        0     7471 2023-05-23 20:04:40.000000 bio-aid-0.3.0/BioAid/complexity.py
+drwxrwxrwx   0        0        0        0 2023-05-23 20:58:31.597419 bio-aid-0.3.0/BioAid/deepSeqInsH/
+-rw-rw-rw-   0        0        0      193 2023-03-01 22:49:33.000000 bio-aid-0.3.0/BioAid/deepSeqInsH/__init__.py
+-rw-rw-rw-   0        0        0     2693 2023-04-25 21:33:33.000000 bio-aid-0.3.0/BioAid/deepSeqInsH/annoInsH.py
+-rw-rw-rw-   0        0        0     3048 2023-05-23 20:10:39.000000 bio-aid-0.3.0/BioAid/diluter.py
+-rw-rw-rw-   0        0        0     2045 2023-05-23 20:13:32.000000 bio-aid-0.3.0/BioAid/makeMMBSearchRef.py
+-rw-rw-rw-   0        0        0     2903 2023-05-23 20:19:13.000000 bio-aid-0.3.0/BioAid/paralleltools.py
+-rw-rw-rw-   0        0        0     1436 2023-05-23 20:21:48.000000 bio-aid-0.3.0/BioAid/popDub.py
+-rw-rw-rw-   0        0        0     9456 2023-05-23 20:49:05.000000 bio-aid-0.3.0/BioAid/repeatSearch.py
+drwxrwxrwx   0        0        0        0 2023-05-23 20:58:31.597419 bio-aid-0.3.0/BioAid/variantTK/
+-rw-rw-rw-   0        0        0      193 2023-03-01 22:45:37.000000 bio-aid-0.3.0/BioAid/variantTK/__init__.py
+-rw-rw-rw-   0        0        0    10973 2023-03-01 22:48:01.000000 bio-aid-0.3.0/BioAid/variantTK/variants.py
+-rw-rw-rw-   0        0        0     1101 2023-03-01 22:53:18.000000 bio-aid-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      615 2023-05-23 20:58:31.617248 bio-aid-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3164 2023-03-01 22:53:18.000000 bio-aid-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 20:58:31.617248 bio-aid-0.3.0/bio_aid.egg-info/
+-rw-rw-rw-   0        0        0      615 2023-05-23 20:58:31.000000 bio-aid-0.3.0/bio_aid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-05-23 20:58:31.000000 bio-aid-0.3.0/bio_aid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 20:58:31.000000 bio-aid-0.3.0/bio_aid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-23 20:58:31.000000 bio-aid-0.3.0/bio_aid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-23 20:58:31.000000 bio-aid-0.3.0/bio_aid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 20:58:31.626261 bio-aid-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      997 2023-05-23 20:57:20.000000 bio-aid-0.3.0/setup.py
```

### Comparing `bio-aid-0.2.2/BioAid/MMBSearchTK/AnnoMMBS.py` & `bio-aid-0.3.0/BioAid/MMBSearchTK/AnnoMMBS.py`

 * *Files identical despite different names*

### Comparing `bio-aid-0.2.2/BioAid/MMBSearchTK/makeMMBSearchRef.py` & `bio-aid-0.3.0/BioAid/MMBSearchTK/makeMMBSearchRef.py`

 * *Files identical despite different names*

### Comparing `bio-aid-0.2.2/BioAid/deepSeqInsH/annoInsH.py` & `bio-aid-0.3.0/BioAid/deepSeqInsH/annoInsH.py`

 * *Files identical despite different names*

### Comparing `bio-aid-0.2.2/BioAid/popDub.py` & `bio-aid-0.3.0/BioAid/popDub.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # This code was developed and authored by Jerzy Twarowski in Malkova Lab at the University of Iowa 
 # Contact: jerzymateusz-twarowski@uiowa.edu, tvarovski1@gmail.com
 
-def calculatePopulationDoublings(initial_population, final_population_ml, final_culture_volume):
+def calculatePopulationDoublings(initial_population: int|float, final_population_ml: int|float, final_culture_volume: int|float) -> None:
+    """
+    Calculates the number of population doublings required to reach a final population size.
+
+    Args:
+        initial_population (int|float): The initial population size.
+        final_population_ml (int|float): The final population size in milliliters.
+        final_culture_volume (int|float): The final culture volume in milliliters.
+
+    Returns:
+        None: This function does not return anything, but prints the number of population doublings required to reach the final population size.
+    """
     final_population = final_population_ml * final_culture_volume
     doubling_cycle_size = final_population
     doublings = 0
     while doubling_cycle_size > initial_population:
         if doubling_cycle_size < initial_population*2:
             doublings = doublings + (doubling_cycle_size-initial_population)/initial_population
             break
```

### Comparing `bio-aid-0.2.2/BioAid/variantTK/variants.py` & `bio-aid-0.3.0/BioAid/variantTK/variants.py`

 * *Files identical despite different names*

### Comparing `bio-aid-0.2.2/LICENSE` & `bio-aid-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bio-aid-0.2.2/PKG-INFO` & `bio-aid-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bio-aid
-Version: 0.2.2
+Version: 0.3.0
 Summary: Genetic Analysis Tools
 Author: tvarovski (Jerzy Twarowski)
 Author-email: <tvarovski1@gmail.com>
 Keywords: python,biology,bio,genetics,genomics,NGS
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 A package that contains tools for the analysis of genetic sequence and sequencing related data
```

### Comparing `bio-aid-0.2.2/README.md` & `bio-aid-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bio-aid-0.2.2/bio_aid.egg-info/PKG-INFO` & `bio-aid-0.3.0/bio_aid.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bio-aid
-Version: 0.2.2
+Version: 0.3.0
 Summary: Genetic Analysis Tools
 Author: tvarovski (Jerzy Twarowski)
 Author-email: <tvarovski1@gmail.com>
 Keywords: python,biology,bio,genetics,genomics,NGS
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 A package that contains tools for the analysis of genetic sequence and sequencing related data
```

### Comparing `bio-aid-0.2.2/bio_aid.egg-info/SOURCES.txt` & `bio-aid-0.3.0/bio_aid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bio-aid-0.2.2/setup.py` & `bio-aid-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.2.2'
+VERSION = '0.3.0'
 DESCRIPTION = 'Genetic Analysis Tools'
 LONG_DESCRIPTION = 'A package that contains tools for the analysis of genetic sequence and sequencing related data'
 
 # Setting up
 setup(
     name="bio-aid",
     version=VERSION,
@@ -17,13 +17,13 @@
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=['pandas', 'numpy', 'matplotlib', 'seaborn', 'regex', 'pyensembl', 'natsort'],
     keywords=['python', 'biology', 'bio', 'genetics', 'genomics', 'NGS'],
     classifiers=[
         "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.10",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

