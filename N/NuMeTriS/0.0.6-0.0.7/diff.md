# Comparing `tmp/NuMeTriS-0.0.6.tar.gz` & `tmp/NuMeTriS-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NuMeTriS-0.0.6.tar", last modified: Tue May 23 08:10:14 2023, max compression
+gzip compressed data, was "NuMeTriS-0.0.7.tar", last modified: Tue May 23 08:17:33 2023, max compression
```

## Comparing `NuMeTriS-0.0.6.tar` & `NuMeTriS-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 08:10:14.238474 NuMeTriS-0.0.6/
--rw-rw-r--   0 mars      (1000) mars      (1000)    35149 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/LICENSE
--rw-rw-r--   0 mars      (1000) mars      (1000)     9557 2023-05-23 08:10:14.238474 NuMeTriS-0.0.6/PKG-INFO
--rw-rw-r--   0 mars      (1000) mars      (1000)     8571 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/README.md
--rw-rw-r--   0 mars      (1000) mars      (1000)     1380 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/pyproject.toml
--rw-rw-r--   0 mars      (1000) mars      (1000)       38 2023-05-23 08:10:14.238474 NuMeTriS-0.0.6/setup.cfg
--rw-rw-r--   0 mars      (1000) mars      (1000)      136 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/setup.py
-drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 08:10:14.238474 NuMeTriS-0.0.6/src/
-drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 08:10:14.238474 NuMeTriS-0.0.6/src/NuMeTriS/
--rw-rw-r--   0 mars      (1000) mars      (1000)    23127 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/src/NuMeTriS/Graph_Class.py
--rw-rw-r--   0 mars      (1000) mars      (1000)    69485 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/src/NuMeTriS/Utility_Functions.py
--rw-rw-r--   0 mars      (1000) mars      (1000)      183 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/src/NuMeTriS/__init__.py
-drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 08:10:14.238474 NuMeTriS-0.0.6/src/NuMeTriS.egg-info/
--rw-rw-r--   0 mars      (1000) mars      (1000)     9557 2023-05-23 08:10:14.000000 NuMeTriS-0.0.6/src/NuMeTriS.egg-info/PKG-INFO
--rw-rw-r--   0 mars      (1000) mars      (1000)      395 2023-05-23 08:10:14.000000 NuMeTriS-0.0.6/src/NuMeTriS.egg-info/SOURCES.txt
--rw-rw-r--   0 mars      (1000) mars      (1000)        1 2023-05-23 08:10:14.000000 NuMeTriS-0.0.6/src/NuMeTriS.egg-info/dependency_links.txt
--rw-rw-r--   0 mars      (1000) mars      (1000)       94 2023-05-23 08:10:14.000000 NuMeTriS-0.0.6/src/NuMeTriS.egg-info/requires.txt
--rw-rw-r--   0 mars      (1000) mars      (1000)        9 2023-05-23 08:10:14.000000 NuMeTriS-0.0.6/src/NuMeTriS.egg-info/top_level.txt
-drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 08:10:14.238474 NuMeTriS-0.0.6/tests/
--rw-rw-r--   0 mars      (1000) mars      (1000)      693 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/tests/test_DBCM.py
--rw-rw-r--   0 mars      (1000) mars      (1000)      703 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/tests/test_DBCM_CReMa.py
--rw-rw-r--   0 mars      (1000) mars      (1000)      693 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/tests/test_RBCM.py
--rw-rw-r--   0 mars      (1000) mars      (1000)      703 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/tests/test_RBCM_CRWCM.py
+drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 08:17:33.229567 NuMeTriS-0.0.7/
+-rw-rw-r--   0 mars      (1000) mars      (1000)    35149 2023-05-23 08:15:44.000000 NuMeTriS-0.0.7/LICENSE
+-rw-rw-r--   0 mars      (1000) mars      (1000)     9560 2023-05-23 08:17:33.229567 NuMeTriS-0.0.7/PKG-INFO
+-rw-rw-r--   0 mars      (1000) mars      (1000)     8574 2023-05-23 08:15:44.000000 NuMeTriS-0.0.7/README.md
+-rw-rw-r--   0 mars      (1000) mars      (1000)     1380 2023-05-23 08:15:44.000000 NuMeTriS-0.0.7/pyproject.toml
+-rw-rw-r--   0 mars      (1000) mars      (1000)       38 2023-05-23 08:17:33.229567 NuMeTriS-0.0.7/setup.cfg
+-rw-rw-r--   0 mars      (1000) mars      (1000)      136 2023-05-23 08:15:44.000000 NuMeTriS-0.0.7/setup.py
+drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 08:17:33.229567 NuMeTriS-0.0.7/src/
+drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 08:17:33.229567 NuMeTriS-0.0.7/src/NuMeTriS/
+-rw-rw-r--   0 mars      (1000) mars      (1000)    23127 2023-05-23 08:15:44.000000 NuMeTriS-0.0.7/src/NuMeTriS/Graph_Class.py
+-rw-rw-r--   0 mars      (1000) mars      (1000)    69485 2023-05-23 08:15:44.000000 NuMeTriS-0.0.7/src/NuMeTriS/Utility_Functions.py
+-rw-rw-r--   0 mars      (1000) mars      (1000)      183 2023-05-23 08:15:44.000000 NuMeTriS-0.0.7/src/NuMeTriS/__init__.py
+drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 08:17:33.229567 NuMeTriS-0.0.7/src/NuMeTriS.egg-info/
+-rw-rw-r--   0 mars      (1000) mars      (1000)     9560 2023-05-23 08:17:33.000000 NuMeTriS-0.0.7/src/NuMeTriS.egg-info/PKG-INFO
+-rw-rw-r--   0 mars      (1000) mars      (1000)      395 2023-05-23 08:17:33.000000 NuMeTriS-0.0.7/src/NuMeTriS.egg-info/SOURCES.txt
+-rw-rw-r--   0 mars      (1000) mars      (1000)        1 2023-05-23 08:17:33.000000 NuMeTriS-0.0.7/src/NuMeTriS.egg-info/dependency_links.txt
+-rw-rw-r--   0 mars      (1000) mars      (1000)       94 2023-05-23 08:17:33.000000 NuMeTriS-0.0.7/src/NuMeTriS.egg-info/requires.txt
+-rw-rw-r--   0 mars      (1000) mars      (1000)        9 2023-05-23 08:17:33.000000 NuMeTriS-0.0.7/src/NuMeTriS.egg-info/top_level.txt
+drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 08:17:33.229567 NuMeTriS-0.0.7/tests/
+-rw-rw-r--   0 mars      (1000) mars      (1000)      693 2023-05-23 08:15:44.000000 NuMeTriS-0.0.7/tests/test_DBCM.py
+-rw-rw-r--   0 mars      (1000) mars      (1000)      703 2023-05-23 08:15:44.000000 NuMeTriS-0.0.7/tests/test_DBCM_CReMa.py
+-rw-rw-r--   0 mars      (1000) mars      (1000)      693 2023-05-23 08:15:44.000000 NuMeTriS-0.0.7/tests/test_RBCM.py
+-rw-rw-r--   0 mars      (1000) mars      (1000)      703 2023-05-23 08:15:44.000000 NuMeTriS-0.0.7/tests/test_RBCM_CRWCM.py
```

### Comparing `NuMeTriS-0.0.6/LICENSE` & `NuMeTriS-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.6/PKG-INFO` & `NuMeTriS-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NuMeTriS
-Version: 0.0.6
+Version: 0.0.7
 Summary: NuMeTris is a package for Maximum-Entropy models for triadic pattern detection. It contains known models such as DBCM and RBCM for binary motif analysis, and contain mixture models such as DBCM+CReMa and RBCM+CRWCM for weighted triadic motif analysis. The models are solved and routine are present for numeric ensemble generation and the computation of the triadic z-scores for triadic sub-graph occurrence, average flux and intensity.
 Author-email: Marzio Di Vece <marzio.divece@imtlucca.it>
 Project-URL: Homepage, https://github.com/MarsMDK/NuMeTriS
 Keywords: maximum entropy methods,network motifs,pattern detection,graph,network,entropy
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -167,15 +167,15 @@
 
 It plots triadic occurrences (if a binary model is used) or occurrences, fluxes and intensities (if a mixture model is used).
 It is possible to plot z-scores using the argument type='z-scores', significance profiles using argument type='significance' or both, using type='both'.
 
 
 
 ## Documentation
-You can find the complete documentation of the DyGyS library in [documentation](https://numetris.readthedocs.io/en/latest/index.html)
+You can find the complete documentation of the NuMeTriS library in [documentation](https://numetris.readthedocs.io/en/latest/index.html)
 
 ## Credits
 
 *Author*:
 
 [Marzio Di Vece](https://www.imtlucca.it/it/marzio.divece) (a.k.a. [MarsMDK](https://github.com/MarsMDK))
```

### Comparing `NuMeTriS-0.0.6/README.md` & `NuMeTriS-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
 It plots triadic occurrences (if a binary model is used) or occurrences, fluxes and intensities (if a mixture model is used).
 It is possible to plot z-scores using the argument type='z-scores', significance profiles using argument type='significance' or both, using type='both'.
 
 
 
 ## Documentation
-You can find the complete documentation of the DyGyS library in [documentation](https://numetris.readthedocs.io/en/latest/index.html)
+You can find the complete documentation of the NuMeTriS library in [documentation](https://numetris.readthedocs.io/en/latest/index.html)
 
 ## Credits
 
 *Author*:
 
 [Marzio Di Vece](https://www.imtlucca.it/it/marzio.divece) (a.k.a. [MarsMDK](https://github.com/MarsMDK))
```

### Comparing `NuMeTriS-0.0.6/pyproject.toml` & `NuMeTriS-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NuMeTriS"
-version = "0.0.6"
+version = "0.0.7"
 description = "NuMeTris is a package for Maximum-Entropy models for triadic pattern detection. It contains known models such as DBCM and RBCM for binary motif analysis, and contain mixture models such as DBCM+CReMa and RBCM+CRWCM for weighted triadic motif analysis. The models are solved and routine are present for numeric ensemble generation and the computation of the triadic z-scores for triadic sub-graph occurrence, average flux and intensity."
 readme = "README.md"
 license = {file = "GNU General Public License v3"}
 authors = [{ name = "Marzio Di Vece", email = "marzio.divece@imtlucca.it" }]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3.9",
```

### Comparing `NuMeTriS-0.0.6/src/NuMeTriS/Graph_Class.py` & `NuMeTriS-0.0.7/src/NuMeTriS/Graph_Class.py`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.6/src/NuMeTriS/Utility_Functions.py` & `NuMeTriS-0.0.7/src/NuMeTriS/Utility_Functions.py`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.6/src/NuMeTriS.egg-info/PKG-INFO` & `NuMeTriS-0.0.7/src/NuMeTriS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NuMeTriS
-Version: 0.0.6
+Version: 0.0.7
 Summary: NuMeTris is a package for Maximum-Entropy models for triadic pattern detection. It contains known models such as DBCM and RBCM for binary motif analysis, and contain mixture models such as DBCM+CReMa and RBCM+CRWCM for weighted triadic motif analysis. The models are solved and routine are present for numeric ensemble generation and the computation of the triadic z-scores for triadic sub-graph occurrence, average flux and intensity.
 Author-email: Marzio Di Vece <marzio.divece@imtlucca.it>
 Project-URL: Homepage, https://github.com/MarsMDK/NuMeTriS
 Keywords: maximum entropy methods,network motifs,pattern detection,graph,network,entropy
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -167,15 +167,15 @@
 
 It plots triadic occurrences (if a binary model is used) or occurrences, fluxes and intensities (if a mixture model is used).
 It is possible to plot z-scores using the argument type='z-scores', significance profiles using argument type='significance' or both, using type='both'.
 
 
 
 ## Documentation
-You can find the complete documentation of the DyGyS library in [documentation](https://numetris.readthedocs.io/en/latest/index.html)
+You can find the complete documentation of the NuMeTriS library in [documentation](https://numetris.readthedocs.io/en/latest/index.html)
 
 ## Credits
 
 *Author*:
 
 [Marzio Di Vece](https://www.imtlucca.it/it/marzio.divece) (a.k.a. [MarsMDK](https://github.com/MarsMDK))
```

### Comparing `NuMeTriS-0.0.6/tests/test_DBCM.py` & `NuMeTriS-0.0.7/tests/test_DBCM.py`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.6/tests/test_DBCM_CReMa.py` & `NuMeTriS-0.0.7/tests/test_DBCM_CReMa.py`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.6/tests/test_RBCM.py` & `NuMeTriS-0.0.7/tests/test_RBCM.py`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.6/tests/test_RBCM_CRWCM.py` & `NuMeTriS-0.0.7/tests/test_RBCM_CRWCM.py`

 * *Files identical despite different names*

