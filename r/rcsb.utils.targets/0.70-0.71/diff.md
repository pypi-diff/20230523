# Comparing `tmp/rcsb.utils.targets-0.70.tar.gz` & `tmp/rcsb.utils.targets-0.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.targets-0.70.tar", last modified: Mon May  8 17:44:53 2023, max compression
+gzip compressed data, was "rcsb.utils.targets-0.71.tar", last modified: Tue May 23 16:25:31 2023, max compression
```

## Comparing `rcsb.utils.targets-0.70.tar` & `rcsb.utils.targets-0.71.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-08 17:44:53.818546 rcsb.utils.targets-0.70/
--rw-r--r--   0 vsts      (1001) docker     (122)     5977 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1645 2023-05-08 17:44:53.818546 rcsb.utils.targets-0.70/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      953 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-08 17:44:53.814546 rcsb.utils.targets-0.70/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-08 17:44:53.818546 rcsb.utils.targets-0.70/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-08 17:44:53.818546 rcsb.utils.targets-0.70/rcsb/utils/targets/
--rw-r--r--   0 vsts      (1001) docker     (122)     9301 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/CARDTargetAnnotationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7017 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/CARDTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8021 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/CARDTargetOntologyProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10102 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/CARDTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19228 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/ChEMBLTargetActivityProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13181 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5330 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8904 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/ChEMBLTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9171 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/DrugBankTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12661 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/DrugBankTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9505 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/IMGTTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    20738 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/IMGTTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10451 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/PharosTargetActivityProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12770 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/PharosTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9154 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/PharosTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8898 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/SAbDabTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9689 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/SAbDabTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/rcsb/utils/targets/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-08 17:44:53.818546 rcsb.utils.targets-0.70/rcsb.utils.targets.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1645 2023-05-08 17:44:53.000000 rcsb.utils.targets-0.70/rcsb.utils.targets.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1209 2023-05-08 17:44:53.000000 rcsb.utils.targets-0.70/rcsb.utils.targets.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-08 17:44:53.000000 rcsb.utils.targets-0.70/rcsb.utils.targets.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-08 17:32:15.000000 rcsb.utils.targets-0.70/rcsb.utils.targets.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      216 2023-05-08 17:44:53.000000 rcsb.utils.targets-0.70/rcsb.utils.targets.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-08 17:44:53.000000 rcsb.utils.targets-0.70/rcsb.utils.targets.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-05-08 17:44:53.818546 rcsb.utils.targets-0.70/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     2273 2023-05-08 17:31:08.000000 rcsb.utils.targets-0.70/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:25:31.408550 rcsb.utils.targets-0.71/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6044 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1645 2023-05-23 16:25:31.408550 rcsb.utils.targets-0.71/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      953 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:25:31.400550 rcsb.utils.targets-0.71/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:25:31.404550 rcsb.utils.targets-0.71/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:25:31.408550 rcsb.utils.targets-0.71/rcsb/utils/targets/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9301 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/CARDTargetAnnotationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7017 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/CARDTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8021 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/CARDTargetOntologyProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10102 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/CARDTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19228 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/ChEMBLTargetActivityProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13181 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5330 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8904 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/ChEMBLTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9171 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/DrugBankTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12661 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/DrugBankTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9505 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/IMGTTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    20738 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/IMGTTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10451 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/PharosTargetActivityProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12770 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/PharosTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9154 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/PharosTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8898 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/SAbDabTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9689 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/SAbDabTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:25:31.404550 rcsb.utils.targets-0.71/rcsb.utils.targets.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1645 2023-05-23 16:25:31.000000 rcsb.utils.targets-0.71/rcsb.utils.targets.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1209 2023-05-23 16:25:31.000000 rcsb.utils.targets-0.71/rcsb.utils.targets.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-23 16:25:31.000000 rcsb.utils.targets-0.71/rcsb.utils.targets.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-23 16:12:21.000000 rcsb.utils.targets-0.71/rcsb.utils.targets.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      216 2023-05-23 16:25:31.000000 rcsb.utils.targets-0.71/rcsb.utils.targets.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-23 16:25:31.000000 rcsb.utils.targets-0.71/rcsb.utils.targets.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-05-23 16:25:31.408550 rcsb.utils.targets-0.71/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     2273 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/setup.py
```

### Comparing `rcsb.utils.targets-0.70/HISTORY.txt` & `rcsb.utils.targets-0.71/HISTORY.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,7 +56,8 @@
   13-Mar-2023  - V0.64 Add CARDTargetAnnotationProvider (to replace CARDTargetFeatureProvider)
   22-Mar-2023  - V0.65 Add timeout to IMGT data file fetch, and update py-rcsb_exdb_assets locators
   24-Mar-2023  - V0.66 In PharosTargetProvider(), download sql file to separate dir
   11-Apr-2023  - V0.67 Fix issue with CARD lineage tree building--handle cases with two parents at same depth; Add treeNodeList building and exporting
   27-Apr-2023  - V0.68 Update CARD treeNodeList building
    2-May-2023  - V0.69 Remove depth field from CARD lineage tree
    5-May-2023  - V0.70 Actually check cache files exist in PharosTargetProvider testCache()
+  22-May-2023  - V0.71 Add retries to tox task for MMseqs2 download
```

### Comparing `rcsb.utils.targets-0.70/LICENSE` & `rcsb.utils.targets-0.71/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.70/PKG-INFO` & `rcsb.utils.targets-0.71/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.targets
-Version: 0.70
+Version: 0.71
 Summary: RCSB Python Wrapper Module for Target Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_targets
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.targets-0.70/README.md` & `rcsb.utils.targets-0.71/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.70/rcsb/utils/targets/CARDTargetAnnotationProvider.py` & `rcsb.utils.targets-0.71/rcsb/utils/targets/CARDTargetAnnotationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.70/rcsb/utils/targets/CARDTargetFeatureProvider.py` & `rcsb.utils.targets-0.71/rcsb/utils/targets/CARDTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.70/rcsb/utils/targets/CARDTargetOntologyProvider.py` & `rcsb.utils.targets-0.71/rcsb/utils/targets/CARDTargetOntologyProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.70/rcsb/utils/targets/CARDTargetProvider.py` & `rcsb.utils.targets-0.71/rcsb/utils/targets/CARDTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.70/rcsb/utils/targets/ChEMBLTargetActivityProvider.py` & `rcsb.utils.targets-0.71/rcsb/utils/targets/ChEMBLTargetActivityProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.70/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py` & `rcsb.utils.targets-0.71/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.70/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py` & `rcsb.utils.targets-0.71/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.70/rcsb/utils/targets/ChEMBLTargetProvider.py` & `rcsb.utils.targets-0.71/rcsb/utils/targets/ChEMBLTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.70/rcsb/utils/targets/DrugBankTargetCofactorProvider.py` & `rcsb.utils.targets-0.71/rcsb/utils/targets/DrugBankTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.70/rcsb/utils/targets/DrugBankTargetProvider.py` & `rcsb.utils.targets-0.71/rcsb/utils/targets/DrugBankTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.70/rcsb/utils/targets/IMGTTargetFeatureProvider.py` & `rcsb.utils.targets-0.71/rcsb/utils/targets/IMGTTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.70/rcsb/utils/targets/IMGTTargetProvider.py` & `rcsb.utils.targets-0.71/rcsb/utils/targets/IMGTTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.70/rcsb/utils/targets/PharosTargetActivityProvider.py` & `rcsb.utils.targets-0.71/rcsb/utils/targets/PharosTargetActivityProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.70/rcsb/utils/targets/PharosTargetCofactorProvider.py` & `rcsb.utils.targets-0.71/rcsb/utils/targets/PharosTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.70/rcsb/utils/targets/PharosTargetProvider.py` & `rcsb.utils.targets-0.71/rcsb/utils/targets/PharosTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.70/rcsb/utils/targets/SAbDabTargetFeatureProvider.py` & `rcsb.utils.targets-0.71/rcsb/utils/targets/SAbDabTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.70/rcsb/utils/targets/SAbDabTargetProvider.py` & `rcsb.utils.targets-0.71/rcsb/utils/targets/SAbDabTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.70/rcsb.utils.targets.egg-info/PKG-INFO` & `rcsb.utils.targets-0.71/rcsb.utils.targets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.targets
-Version: 0.70
+Version: 0.71
 Summary: RCSB Python Wrapper Module for Target Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_targets
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.targets-0.70/rcsb.utils.targets.egg-info/SOURCES.txt` & `rcsb.utils.targets-0.71/rcsb.utils.targets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.70/setup.py` & `rcsb.utils.targets-0.71/setup.py`

 * *Files identical despite different names*

