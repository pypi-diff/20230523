# Comparing `tmp/tidytcells-1.7.0.tar.gz` & `tmp/tidytcells-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidytcells-1.7.0.tar", last modified: Sat May 20 20:39:04 2023, max compression
+gzip compressed data, was "tidytcells-1.8.0.tar", last modified: Tue May 23 16:25:09 2023, max compression
```

## Comparing `tidytcells-1.7.0.tar` & `tidytcells-1.8.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.522236 tidytcells-1.7.0/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1068 2022-11-05 19:14:55.000000 tidytcells-1.7.0/LICENSE.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       19 2022-11-06 20:07:03.000000 tidytcells-1.7.0/MANIFEST.in
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2052 2023-05-20 20:39:04.522236 tidytcells-1.7.0/PKG-INFO
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1433 2023-03-05 13:54:54.000000 tidytcells-1.7.0/README.md
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        5 2023-05-20 20:34:56.000000 tidytcells-1.7.0/VERSION.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       38 2023-05-20 20:39:04.522236 tidytcells-1.7.0/setup.cfg
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1287 2023-03-05 13:54:54.000000 tidytcells-1.7.0/setup.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.511236 tidytcells-1.7.0/src/
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.513236 tidytcells-1.7.0/src/tidytcells/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       90 2023-03-11 19:32:17.000000 tidytcells-1.7.0/src/tidytcells/__init__.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.518236 tidytcells-1.7.0/src/tidytcells/_resources/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1109 2023-05-20 20:06:21.000000 tidytcells-1.7.0/src/tidytcells/_resources/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)   611997 2023-02-24 16:40:58.000000 tidytcells-1.7.0/src/tidytcells/_resources/homosapiens_mhc.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1295 2023-02-24 16:40:58.000000 tidytcells-1.7.0/src/tidytcells/_resources/homosapiens_mhc_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    14382 2023-05-20 18:54:56.000000 tidytcells-1.7.0/src/tidytcells/_resources/homosapiens_tcr.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    59200 2023-05-20 19:36:11.000000 tidytcells-1.7.0/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     6476 2023-05-20 18:54:57.000000 tidytcells-1.7.0/src/tidytcells/_resources/homosapiens_tcr_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1031 2023-02-24 20:05:06.000000 tidytcells-1.7.0/src/tidytcells/_resources/musmusculus_mhc.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     5344 2023-02-24 20:05:06.000000 tidytcells-1.7.0/src/tidytcells/_resources/musmusculus_mhc_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    16802 2023-02-24 16:40:58.000000 tidytcells-1.7.0/src/tidytcells/_resources/musmusculus_tcr.json
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.519236 tidytcells-1.7.0/src/tidytcells/_utils/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        0 2023-02-24 16:40:58.000000 tidytcells-1.7.0/src/tidytcells/_utils/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     4336 2023-05-20 20:12:43.000000 tidytcells-1.7.0/src/tidytcells/_utils/abstract_functions.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     3081 2023-03-05 13:54:54.000000 tidytcells-1.7.0/src/tidytcells/_utils/gene_query_engines.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    10869 2023-03-05 13:54:54.000000 tidytcells-1.7.0/src/tidytcells/_utils/gene_standardisers.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      553 2023-03-05 13:54:54.000000 tidytcells-1.7.0/src/tidytcells/_utils/warnings.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.519236 tidytcells-1.7.0/src/tidytcells/aa/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      246 2023-03-11 19:32:17.000000 tidytcells-1.7.0/src/tidytcells/aa/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1290 2023-03-11 19:32:17.000000 tidytcells-1.7.0/src/tidytcells/aa/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.520236 tidytcells-1.7.0/src/tidytcells/junction/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      248 2023-03-11 19:32:17.000000 tidytcells-1.7.0/src/tidytcells/junction/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2671 2023-03-11 19:32:17.000000 tidytcells-1.7.0/src/tidytcells/junction/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.520236 tidytcells-1.7.0/src/tidytcells/mhc/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      403 2023-03-05 13:54:54.000000 tidytcells-1.7.0/src/tidytcells/mhc/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     9648 2023-03-11 23:17:03.000000 tidytcells-1.7.0/src/tidytcells/mhc/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.521236 tidytcells-1.7.0/src/tidytcells/tcr/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      260 2023-05-20 20:15:47.000000 tidytcells-1.7.0/src/tidytcells/tcr/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8313 2023-05-20 20:17:45.000000 tidytcells-1.7.0/src/tidytcells/tcr/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.514236 tidytcells-1.7.0/src/tidytcells.egg-info/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2052 2023-05-20 20:39:04.000000 tidytcells-1.7.0/src/tidytcells.egg-info/PKG-INFO
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1244 2023-05-20 20:39:04.000000 tidytcells-1.7.0/src/tidytcells.egg-info/SOURCES.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        1 2023-05-20 20:39:04.000000 tidytcells-1.7.0/src/tidytcells.egg-info/dependency_links.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       89 2023-05-20 20:39:04.000000 tidytcells-1.7.0/src/tidytcells.egg-info/requires.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       11 2023-05-20 20:39:04.000000 tidytcells-1.7.0/src/tidytcells.egg-info/top_level.txt
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.521236 tidytcells-1.7.0/tests/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1231 2023-03-11 19:32:17.000000 tidytcells-1.7.0/tests/test_aa.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2021 2023-03-11 19:32:17.000000 tidytcells-1.7.0/tests/test_junction.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8969 2023-03-05 13:54:54.000000 tidytcells-1.7.0/tests/test_mhc.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     7811 2023-05-20 20:32:03.000000 tidytcells-1.7.0/tests/test_tcr.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.854359 tidytcells-1.8.0/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1068 2022-12-06 13:03:03.000000 tidytcells-1.8.0/LICENSE.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       19 2022-12-06 13:03:03.000000 tidytcells-1.8.0/MANIFEST.in
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2052 2023-05-23 16:25:09.854359 tidytcells-1.8.0/PKG-INFO
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1433 2023-05-23 15:08:38.000000 tidytcells-1.8.0/README.md
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        5 2023-05-23 16:21:15.000000 tidytcells-1.8.0/VERSION.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       38 2023-05-23 16:25:09.854359 tidytcells-1.8.0/setup.cfg
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1287 2023-05-23 16:19:34.000000 tidytcells-1.8.0/setup.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.845358 tidytcells-1.8.0/src/
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.846358 tidytcells-1.8.0/src/tidytcells/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       90 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/__init__.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.850358 tidytcells-1.8.0/src/tidytcells/_resources/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1283 2023-05-23 16:14:45.000000 tidytcells-1.8.0/src/tidytcells/_resources/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)   611997 2023-03-02 13:53:55.000000 tidytcells-1.8.0/src/tidytcells/_resources/homosapiens_mhc.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1295 2023-03-02 13:53:55.000000 tidytcells-1.8.0/src/tidytcells/_resources/homosapiens_mhc_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    14382 2023-05-23 16:03:07.000000 tidytcells-1.8.0/src/tidytcells/_resources/homosapiens_tcr.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    88302 2023-05-23 16:03:08.000000 tidytcells-1.8.0/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     6476 2023-05-23 16:03:08.000000 tidytcells-1.8.0/src/tidytcells/_resources/homosapiens_tcr_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1031 2023-03-02 13:53:55.000000 tidytcells-1.8.0/src/tidytcells/_resources/musmusculus_mhc.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     5344 2023-03-02 13:53:55.000000 tidytcells-1.8.0/src/tidytcells/_resources/musmusculus_mhc_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    16802 2023-03-02 13:53:55.000000 tidytcells-1.8.0/src/tidytcells/_resources/musmusculus_tcr.json
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.851359 tidytcells-1.8.0/src/tidytcells/_utils/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        0 2023-03-02 13:53:55.000000 tidytcells-1.8.0/src/tidytcells/_utils/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     4336 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/_utils/abstract_functions.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     3081 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/_utils/gene_query_engines.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    10869 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/_utils/gene_standardisers.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      553 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/_utils/warnings.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.852358 tidytcells-1.8.0/src/tidytcells/aa/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      246 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/aa/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1290 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/aa/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.852358 tidytcells-1.8.0/src/tidytcells/junction/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      248 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/junction/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2671 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/junction/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.852358 tidytcells-1.8.0/src/tidytcells/mhc/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      403 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/mhc/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     9648 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/mhc/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.853358 tidytcells-1.8.0/src/tidytcells/tcr/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      260 2023-05-23 15:08:38.000000 tidytcells-1.8.0/src/tidytcells/tcr/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8425 2023-05-23 16:22:37.000000 tidytcells-1.8.0/src/tidytcells/tcr/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.847359 tidytcells-1.8.0/src/tidytcells.egg-info/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2052 2023-05-23 16:25:09.000000 tidytcells-1.8.0/src/tidytcells.egg-info/PKG-INFO
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1244 2023-05-23 16:25:09.000000 tidytcells-1.8.0/src/tidytcells.egg-info/SOURCES.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        1 2023-05-23 16:25:09.000000 tidytcells-1.8.0/src/tidytcells.egg-info/dependency_links.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       89 2023-05-23 16:25:09.000000 tidytcells-1.8.0/src/tidytcells.egg-info/requires.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       11 2023-05-23 16:25:09.000000 tidytcells-1.8.0/src/tidytcells.egg-info/top_level.txt
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-23 16:25:09.853358 tidytcells-1.8.0/tests/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1231 2023-05-23 15:08:38.000000 tidytcells-1.8.0/tests/test_aa.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2021 2023-05-23 15:08:38.000000 tidytcells-1.8.0/tests/test_junction.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8969 2023-05-23 15:08:38.000000 tidytcells-1.8.0/tests/test_mhc.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8072 2023-05-23 16:10:54.000000 tidytcells-1.8.0/tests/test_tcr.py
```

### Comparing `tidytcells-1.7.0/LICENSE.txt` & `tidytcells-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tidytcells-1.7.0/PKG-INFO` & `tidytcells-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: tidytcells
-Version: 1.7.0
+Version: 1.8.0
 Summary: Standardise TCR/MHC data.
 Author: Yuta Nagano
 Author-email: yutanagano51@proton.me
 Keywords: immunology,bioinformatics,TCR,MHC,HLA,T cell,IMGT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # tidytcells
 
 ![Tests](https://github.com/yutanagano/tidytcells/actions/workflows/tests.yaml/badge.svg)
```

### Comparing `tidytcells-1.7.0/README.md` & `tidytcells-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `tidytcells-1.7.0/setup.py` & `tidytcells-1.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
     keywords="immunology, bioinformatics, TCR, MHC, HLA, T cell, IMGT",
     package_dir={"": "src"},
     packages=find_packages("src"),
     package_data={"tidytcells": ["_resources/*"]},
-    python_requires=">=3.6",
+    python_requires=">=3.9",
     extras_require={
         "dev": [
             "build",
             "odfpy>=1.4.1",
             "pandas>=1.1.5",
             "pip",
             "pytest>=7",
```

### Comparing `tidytcells-1.7.0/src/tidytcells/_resources/homosapiens_mhc.json` & `tidytcells-1.8.0/src/tidytcells/_resources/homosapiens_mhc.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.7.0/src/tidytcells/_resources/homosapiens_mhc_synonyms.json` & `tidytcells-1.8.0/src/tidytcells/_resources/homosapiens_mhc_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.7.0/src/tidytcells/_resources/homosapiens_tcr.json` & `tidytcells-1.8.0/src/tidytcells/_resources/homosapiens_tcr.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.7.0/src/tidytcells/_resources/homosapiens_tcr_synonyms.json` & `tidytcells-1.8.0/src/tidytcells/_resources/homosapiens_tcr_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.7.0/src/tidytcells/_resources/musmusculus_mhc.json` & `tidytcells-1.8.0/src/tidytcells/_resources/musmusculus_mhc.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.7.0/src/tidytcells/_resources/musmusculus_mhc_synonyms.json` & `tidytcells-1.8.0/src/tidytcells/_resources/musmusculus_mhc_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.7.0/src/tidytcells/_resources/musmusculus_tcr.json` & `tidytcells-1.8.0/src/tidytcells/_resources/musmusculus_tcr.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.7.0/src/tidytcells/_utils/abstract_functions.py` & `tidytcells-1.8.0/src/tidytcells/_utils/abstract_functions.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.7.0/src/tidytcells/_utils/gene_query_engines.py` & `tidytcells-1.8.0/src/tidytcells/_utils/gene_query_engines.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.7.0/src/tidytcells/_utils/gene_standardisers.py` & `tidytcells-1.8.0/src/tidytcells/_utils/gene_standardisers.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.7.0/src/tidytcells/_utils/warnings.py` & `tidytcells-1.8.0/src/tidytcells/_utils/warnings.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.7.0/src/tidytcells/aa/_main.py` & `tidytcells-1.8.0/src/tidytcells/aa/_main.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.7.0/src/tidytcells/junction/_main.py` & `tidytcells-1.8.0/src/tidytcells/junction/_main.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.7.0/src/tidytcells/mhc/_main.py` & `tidytcells-1.8.0/src/tidytcells/mhc/_main.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.7.0/src/tidytcells/tcr/_main.py` & `tidytcells-1.8.0/src/tidytcells/tcr/_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
         ``Dict[str, str]``
 
     .. topic:: Example usage
 
         Get amino acid sequence information about the human V gene TRBV2*01.
 
         >>> tt.tcr.get_aa_sequence(gene="TRBV2*01", species="homosapiens")
-        {'CDR1-IMGT': 'SNHLY', 'CDR2-IMGT': 'FYNNEI', 'FR1-IMGT': 'EPEVTQTPSHQVTQMGQEVILRCVPI', 'FR2-IMGT': 'FYWYRQILGQKVEFLVS', 'FR3-IMGT': 'SEKSEIFDDQFSVERPDGSNFTLKIRSTKLEDSAMYFC'}
+        {'CDR1-IMGT': 'SNHLY', 'CDR2-IMGT': 'FYNNEI', 'FR1-IMGT': 'EPEVTQTPSHQVTQMGQEVILRCVPI', 'FR2-IMGT': 'FYWYRQILGQKVEFLVS', 'FR3-IMGT': 'SEKSEIFDDQFSVERPDGSNFTLKIRSTKLEDSAMYFC', 'V-REGION': 'EPEVTQTPSHQVTQMGQEVILRCVPISNHLYFYWYRQILGQKVEFLVSFYNNEISEKSEIFDDQFSVERPDGSNFTLKIRSTKLEDSAMYFCASSE'}
     """
     # Type checks
     if type(gene) != str:
         raise TypeError(f"gene must be type str, got {gene} ({type(gene)}).")
     if type(species) != str:
         raise TypeError(f"species must be type str, got {species} ({type(species)}).")
```

### Comparing `tidytcells-1.7.0/src/tidytcells.egg-info/PKG-INFO` & `tidytcells-1.8.0/src/tidytcells.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: tidytcells
-Version: 1.7.0
+Version: 1.8.0
 Summary: Standardise TCR/MHC data.
 Author: Yuta Nagano
 Author-email: yutanagano51@proton.me
 Keywords: immunology,bioinformatics,TCR,MHC,HLA,T cell,IMGT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # tidytcells
 
 ![Tests](https://github.com/yutanagano/tidytcells/actions/workflows/tests.yaml/badge.svg)
```

### Comparing `tidytcells-1.7.0/src/tidytcells.egg-info/SOURCES.txt` & `tidytcells-1.8.0/src/tidytcells.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tidytcells-1.7.0/tests/test_aa.py` & `tidytcells-1.8.0/tests/test_aa.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.7.0/tests/test_junction.py` & `tidytcells-1.8.0/tests/test_junction.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.7.0/tests/test_mhc.py` & `tidytcells-1.8.0/tests/test_mhc.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.7.0/tests/test_tcr.py` & `tidytcells-1.8.0/tests/test_tcr.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,24 +222,26 @@
                 "TRBV2*01",
                 {
                     "CDR1-IMGT": "SNHLY",
                     "CDR2-IMGT": "FYNNEI",
                     "FR1-IMGT": "EPEVTQTPSHQVTQMGQEVILRCVPI",
                     "FR2-IMGT": "FYWYRQILGQKVEFLVS",
                     "FR3-IMGT": "SEKSEIFDDQFSVERPDGSNFTLKIRSTKLEDSAMYFC",
+                    "V-REGION": "EPEVTQTPSHQVTQMGQEVILRCVPISNHLYFYWYRQILGQKVEFLVSFYNNEISEKSEIFDDQFSVERPDGSNFTLKIRSTKLEDSAMYFCASSE",
                 },
             ),
             (
                 "TRAV10*02",
                 {
                     "CDR1-IMGT": "VSPFSN",
                     "CDR2-IMGT": "MTFSENT",
                     "FR1-IMGT": "KNQVEQSPQSLIILEGKNCTLQCNYT",
                     "FR2-IMGT": "LRWYKQDTGRGPVSLTI",
                     "FR3-IMGT": "KSNGRYTATLDADTKQSSLHITASQLSDSASYIC",
+                    "V-REGION": "KNQVEQSPQSLIILEGKNCTLQCNYTVSPFSNLRWYKQDTGRGPVSLTIMTFSENTKSNGRYTATLDADTKQSSLHITASQLSDSASYICVVS",
                 },
             ),
         ),
     )
     def test_get_aa_sequence(self, gene, expected):
         result = tcr.get_aa_sequence(gene=gene)
```

