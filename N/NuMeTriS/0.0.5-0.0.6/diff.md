# Comparing `tmp/NuMeTriS-0.0.5.tar.gz` & `tmp/NuMeTriS-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NuMeTriS-0.0.5.tar", last modified: Tue May 23 07:54:23 2023, max compression
+gzip compressed data, was "NuMeTriS-0.0.6.tar", last modified: Tue May 23 08:10:14 2023, max compression
```

## Comparing `NuMeTriS-0.0.5.tar` & `NuMeTriS-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 07:54:23.764381 NuMeTriS-0.0.5/
--rw-rw-r--   0 mars      (1000) mars      (1000)    35149 2023-05-23 07:51:06.000000 NuMeTriS-0.0.5/LICENSE
--rw-rw-r--   0 mars      (1000) mars      (1000)     9527 2023-05-23 07:54:23.764381 NuMeTriS-0.0.5/PKG-INFO
--rw-rw-r--   0 mars      (1000) mars      (1000)     8541 2023-05-23 07:51:06.000000 NuMeTriS-0.0.5/README.md
--rw-rw-r--   0 mars      (1000) mars      (1000)     1380 2023-05-23 07:51:06.000000 NuMeTriS-0.0.5/pyproject.toml
--rw-rw-r--   0 mars      (1000) mars      (1000)       38 2023-05-23 07:54:23.764381 NuMeTriS-0.0.5/setup.cfg
--rw-rw-r--   0 mars      (1000) mars      (1000)      136 2023-05-23 07:51:06.000000 NuMeTriS-0.0.5/setup.py
-drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 07:54:23.764381 NuMeTriS-0.0.5/src/
-drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 07:54:23.764381 NuMeTriS-0.0.5/src/NuMeTriS/
--rw-rw-r--   0 mars      (1000) mars      (1000)    23127 2023-05-23 07:51:06.000000 NuMeTriS-0.0.5/src/NuMeTriS/Graph_Class.py
--rw-rw-r--   0 mars      (1000) mars      (1000)    69485 2023-05-23 07:51:06.000000 NuMeTriS-0.0.5/src/NuMeTriS/Utility_Functions.py
--rw-rw-r--   0 mars      (1000) mars      (1000)      183 2023-05-23 07:51:06.000000 NuMeTriS-0.0.5/src/NuMeTriS/__init__.py
-drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 07:54:23.764381 NuMeTriS-0.0.5/src/NuMeTriS.egg-info/
--rw-rw-r--   0 mars      (1000) mars      (1000)     9527 2023-05-23 07:54:23.000000 NuMeTriS-0.0.5/src/NuMeTriS.egg-info/PKG-INFO
--rw-rw-r--   0 mars      (1000) mars      (1000)      395 2023-05-23 07:54:23.000000 NuMeTriS-0.0.5/src/NuMeTriS.egg-info/SOURCES.txt
--rw-rw-r--   0 mars      (1000) mars      (1000)        1 2023-05-23 07:54:23.000000 NuMeTriS-0.0.5/src/NuMeTriS.egg-info/dependency_links.txt
--rw-rw-r--   0 mars      (1000) mars      (1000)       94 2023-05-23 07:54:23.000000 NuMeTriS-0.0.5/src/NuMeTriS.egg-info/requires.txt
--rw-rw-r--   0 mars      (1000) mars      (1000)        9 2023-05-23 07:54:23.000000 NuMeTriS-0.0.5/src/NuMeTriS.egg-info/top_level.txt
-drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 07:54:23.764381 NuMeTriS-0.0.5/tests/
--rw-rw-r--   0 mars      (1000) mars      (1000)      693 2023-05-23 07:51:06.000000 NuMeTriS-0.0.5/tests/test_DBCM.py
--rw-rw-r--   0 mars      (1000) mars      (1000)      703 2023-05-23 07:51:06.000000 NuMeTriS-0.0.5/tests/test_DBCM_CReMa.py
--rw-rw-r--   0 mars      (1000) mars      (1000)      693 2023-05-23 07:51:06.000000 NuMeTriS-0.0.5/tests/test_RBCM.py
--rw-rw-r--   0 mars      (1000) mars      (1000)      703 2023-05-23 07:51:06.000000 NuMeTriS-0.0.5/tests/test_RBCM_CRWCM.py
+drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 08:10:14.238474 NuMeTriS-0.0.6/
+-rw-rw-r--   0 mars      (1000) mars      (1000)    35149 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/LICENSE
+-rw-rw-r--   0 mars      (1000) mars      (1000)     9557 2023-05-23 08:10:14.238474 NuMeTriS-0.0.6/PKG-INFO
+-rw-rw-r--   0 mars      (1000) mars      (1000)     8571 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/README.md
+-rw-rw-r--   0 mars      (1000) mars      (1000)     1380 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/pyproject.toml
+-rw-rw-r--   0 mars      (1000) mars      (1000)       38 2023-05-23 08:10:14.238474 NuMeTriS-0.0.6/setup.cfg
+-rw-rw-r--   0 mars      (1000) mars      (1000)      136 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/setup.py
+drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 08:10:14.238474 NuMeTriS-0.0.6/src/
+drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 08:10:14.238474 NuMeTriS-0.0.6/src/NuMeTriS/
+-rw-rw-r--   0 mars      (1000) mars      (1000)    23127 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/src/NuMeTriS/Graph_Class.py
+-rw-rw-r--   0 mars      (1000) mars      (1000)    69485 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/src/NuMeTriS/Utility_Functions.py
+-rw-rw-r--   0 mars      (1000) mars      (1000)      183 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/src/NuMeTriS/__init__.py
+drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 08:10:14.238474 NuMeTriS-0.0.6/src/NuMeTriS.egg-info/
+-rw-rw-r--   0 mars      (1000) mars      (1000)     9557 2023-05-23 08:10:14.000000 NuMeTriS-0.0.6/src/NuMeTriS.egg-info/PKG-INFO
+-rw-rw-r--   0 mars      (1000) mars      (1000)      395 2023-05-23 08:10:14.000000 NuMeTriS-0.0.6/src/NuMeTriS.egg-info/SOURCES.txt
+-rw-rw-r--   0 mars      (1000) mars      (1000)        1 2023-05-23 08:10:14.000000 NuMeTriS-0.0.6/src/NuMeTriS.egg-info/dependency_links.txt
+-rw-rw-r--   0 mars      (1000) mars      (1000)       94 2023-05-23 08:10:14.000000 NuMeTriS-0.0.6/src/NuMeTriS.egg-info/requires.txt
+-rw-rw-r--   0 mars      (1000) mars      (1000)        9 2023-05-23 08:10:14.000000 NuMeTriS-0.0.6/src/NuMeTriS.egg-info/top_level.txt
+drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 08:10:14.238474 NuMeTriS-0.0.6/tests/
+-rw-rw-r--   0 mars      (1000) mars      (1000)      693 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/tests/test_DBCM.py
+-rw-rw-r--   0 mars      (1000) mars      (1000)      703 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/tests/test_DBCM_CReMa.py
+-rw-rw-r--   0 mars      (1000) mars      (1000)      693 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/tests/test_RBCM.py
+-rw-rw-r--   0 mars      (1000) mars      (1000)      703 2023-05-23 08:08:31.000000 NuMeTriS-0.0.6/tests/test_RBCM_CRWCM.py
```

### Comparing `NuMeTriS-0.0.5/LICENSE` & `NuMeTriS-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.5/PKG-INFO` & `NuMeTriS-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NuMeTriS
-Version: 0.0.5
+Version: 0.0.6
 Summary: NuMeTris is a package for Maximum-Entropy models for triadic pattern detection. It contains known models such as DBCM and RBCM for binary motif analysis, and contain mixture models such as DBCM+CReMa and RBCM+CRWCM for weighted triadic motif analysis. The models are solved and routine are present for numeric ensemble generation and the computation of the triadic z-scores for triadic sub-graph occurrence, average flux and intensity.
 Author-email: Marzio Di Vece <marzio.divece@imtlucca.it>
 Project-URL: Homepage, https://github.com/MarsMDK/NuMeTriS
 Keywords: maximum entropy methods,network motifs,pattern detection,graph,network,entropy
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -16,19 +16,19 @@
 ![PyPI](https://img.shields.io/badge/pypi-v2.1.1-blue)  [![License:GPLv3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Python Version](https://img.shields.io/badge/Python-3.9%20%7C%203.10-blue) [![arXiv](https://img.shields.io/badge/arXiv-2305.12179-orange)](https://arxiv.org/abs/2305.12179)
 
 # NuMeTriS: NUll ModEls for TRIadic Structures
 
 NuMeTriS is a package developed on python3 for Pattern Detection of the 13 triadic connected sub-graphs using maximum-entropy models using direected and reciprocated constraints on network data.
 
 NuMeTriS provides solvers for the binary models DBCM and RBCM, and the conditional weighted models CReMa and CRWCM.
-All of these models are explained in [1](forthcoming on ArXiv).
+All of these models are explained in [[1](https://arxiv.org/abs/2305.12179)].
 The use of DBCM and CReMa enable the user to explicitly constrain network properties based on direction, such as out-degree, in-degree (binary) and out-strength and in-strength (weighted).
 In contrast, the use of RBCM and CRWCM enable the user to constrain network properties based on both direction and reciprocity, such as the reciprocated and non-reciprocated degrees and the reciprocated and non-reciprocated strengths.
 
-Moreover, after solving the models it is possible to generate the related ensembles and compute triadic occurrences, the arithmetic mean of the weights on triadic structures (average fluxes) and their geometric mean (intensities). While triadic occurrences and fluxes are explained in [1](forthcoming on ArXiv), the triadic intensity is the geometric mean of the weights in triadic structures, as explained in [2](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.71.065103) but here defined for all 13 sub-graphs.
+Moreover, after solving the models it is possible to generate the related ensembles and compute triadic occurrences, the arithmetic mean of the weights on triadic structures (average fluxes) and their geometric mean (intensities). While triadic occurrences and fluxes are explained in [[1](https://arxiv.org/abs/2305.12179)], the triadic intensity is the geometric mean of the weights in triadic structures, as explained in [[2](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.71.065103)] but here defined for all 13 sub-graphs.
 
 To explore Maximum-Entropy modeling on networks, checkout [Maximum Entropy Hub](https://meh.imtlucca.it/).
 
 When using the module for your scientific research please consider citing:
 
 
 ```
```

### Comparing `NuMeTriS-0.0.5/README.md` & `NuMeTriS-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ![PyPI](https://img.shields.io/badge/pypi-v2.1.1-blue)  [![License:GPLv3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Python Version](https://img.shields.io/badge/Python-3.9%20%7C%203.10-blue) [![arXiv](https://img.shields.io/badge/arXiv-2305.12179-orange)](https://arxiv.org/abs/2305.12179)
 
 # NuMeTriS: NUll ModEls for TRIadic Structures
 
 NuMeTriS is a package developed on python3 for Pattern Detection of the 13 triadic connected sub-graphs using maximum-entropy models using direected and reciprocated constraints on network data.
 
 NuMeTriS provides solvers for the binary models DBCM and RBCM, and the conditional weighted models CReMa and CRWCM.
-All of these models are explained in [1](forthcoming on ArXiv).
+All of these models are explained in [[1](https://arxiv.org/abs/2305.12179)].
 The use of DBCM and CReMa enable the user to explicitly constrain network properties based on direction, such as out-degree, in-degree (binary) and out-strength and in-strength (weighted).
 In contrast, the use of RBCM and CRWCM enable the user to constrain network properties based on both direction and reciprocity, such as the reciprocated and non-reciprocated degrees and the reciprocated and non-reciprocated strengths.
 
-Moreover, after solving the models it is possible to generate the related ensembles and compute triadic occurrences, the arithmetic mean of the weights on triadic structures (average fluxes) and their geometric mean (intensities). While triadic occurrences and fluxes are explained in [1](forthcoming on ArXiv), the triadic intensity is the geometric mean of the weights in triadic structures, as explained in [2](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.71.065103) but here defined for all 13 sub-graphs.
+Moreover, after solving the models it is possible to generate the related ensembles and compute triadic occurrences, the arithmetic mean of the weights on triadic structures (average fluxes) and their geometric mean (intensities). While triadic occurrences and fluxes are explained in [[1](https://arxiv.org/abs/2305.12179)], the triadic intensity is the geometric mean of the weights in triadic structures, as explained in [[2](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.71.065103)] but here defined for all 13 sub-graphs.
 
 To explore Maximum-Entropy modeling on networks, checkout [Maximum Entropy Hub](https://meh.imtlucca.it/).
 
 When using the module for your scientific research please consider citing:
 
 
 ```
```

### Comparing `NuMeTriS-0.0.5/pyproject.toml` & `NuMeTriS-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NuMeTriS"
-version = "0.0.5"
+version = "0.0.6"
 description = "NuMeTris is a package for Maximum-Entropy models for triadic pattern detection. It contains known models such as DBCM and RBCM for binary motif analysis, and contain mixture models such as DBCM+CReMa and RBCM+CRWCM for weighted triadic motif analysis. The models are solved and routine are present for numeric ensemble generation and the computation of the triadic z-scores for triadic sub-graph occurrence, average flux and intensity."
 readme = "README.md"
 license = {file = "GNU General Public License v3"}
 authors = [{ name = "Marzio Di Vece", email = "marzio.divece@imtlucca.it" }]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3.9",
```

### Comparing `NuMeTriS-0.0.5/src/NuMeTriS/Graph_Class.py` & `NuMeTriS-0.0.6/src/NuMeTriS/Graph_Class.py`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.5/src/NuMeTriS/Utility_Functions.py` & `NuMeTriS-0.0.6/src/NuMeTriS/Utility_Functions.py`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.5/src/NuMeTriS.egg-info/PKG-INFO` & `NuMeTriS-0.0.6/src/NuMeTriS.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NuMeTriS
-Version: 0.0.5
+Version: 0.0.6
 Summary: NuMeTris is a package for Maximum-Entropy models for triadic pattern detection. It contains known models such as DBCM and RBCM for binary motif analysis, and contain mixture models such as DBCM+CReMa and RBCM+CRWCM for weighted triadic motif analysis. The models are solved and routine are present for numeric ensemble generation and the computation of the triadic z-scores for triadic sub-graph occurrence, average flux and intensity.
 Author-email: Marzio Di Vece <marzio.divece@imtlucca.it>
 Project-URL: Homepage, https://github.com/MarsMDK/NuMeTriS
 Keywords: maximum entropy methods,network motifs,pattern detection,graph,network,entropy
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -16,19 +16,19 @@
 ![PyPI](https://img.shields.io/badge/pypi-v2.1.1-blue)  [![License:GPLv3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Python Version](https://img.shields.io/badge/Python-3.9%20%7C%203.10-blue) [![arXiv](https://img.shields.io/badge/arXiv-2305.12179-orange)](https://arxiv.org/abs/2305.12179)
 
 # NuMeTriS: NUll ModEls for TRIadic Structures
 
 NuMeTriS is a package developed on python3 for Pattern Detection of the 13 triadic connected sub-graphs using maximum-entropy models using direected and reciprocated constraints on network data.
 
 NuMeTriS provides solvers for the binary models DBCM and RBCM, and the conditional weighted models CReMa and CRWCM.
-All of these models are explained in [1](forthcoming on ArXiv).
+All of these models are explained in [[1](https://arxiv.org/abs/2305.12179)].
 The use of DBCM and CReMa enable the user to explicitly constrain network properties based on direction, such as out-degree, in-degree (binary) and out-strength and in-strength (weighted).
 In contrast, the use of RBCM and CRWCM enable the user to constrain network properties based on both direction and reciprocity, such as the reciprocated and non-reciprocated degrees and the reciprocated and non-reciprocated strengths.
 
-Moreover, after solving the models it is possible to generate the related ensembles and compute triadic occurrences, the arithmetic mean of the weights on triadic structures (average fluxes) and their geometric mean (intensities). While triadic occurrences and fluxes are explained in [1](forthcoming on ArXiv), the triadic intensity is the geometric mean of the weights in triadic structures, as explained in [2](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.71.065103) but here defined for all 13 sub-graphs.
+Moreover, after solving the models it is possible to generate the related ensembles and compute triadic occurrences, the arithmetic mean of the weights on triadic structures (average fluxes) and their geometric mean (intensities). While triadic occurrences and fluxes are explained in [[1](https://arxiv.org/abs/2305.12179)], the triadic intensity is the geometric mean of the weights in triadic structures, as explained in [[2](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.71.065103)] but here defined for all 13 sub-graphs.
 
 To explore Maximum-Entropy modeling on networks, checkout [Maximum Entropy Hub](https://meh.imtlucca.it/).
 
 When using the module for your scientific research please consider citing:
 
 
 ```
```

### Comparing `NuMeTriS-0.0.5/tests/test_DBCM.py` & `NuMeTriS-0.0.6/tests/test_DBCM.py`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.5/tests/test_DBCM_CReMa.py` & `NuMeTriS-0.0.6/tests/test_DBCM_CReMa.py`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.5/tests/test_RBCM.py` & `NuMeTriS-0.0.6/tests/test_RBCM.py`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.5/tests/test_RBCM_CRWCM.py` & `NuMeTriS-0.0.6/tests/test_RBCM_CRWCM.py`

 * *Files identical despite different names*

