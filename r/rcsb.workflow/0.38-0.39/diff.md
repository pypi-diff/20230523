# Comparing `tmp/rcsb.workflow-0.38.tar.gz` & `tmp/rcsb.workflow-0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.workflow-0.38.tar", last modified: Tue May  9 18:04:08 2023, max compression
+gzip compressed data, was "rcsb.workflow-0.39.tar", last modified: Tue May 23 16:05:39 2023, max compression
```

## Comparing `rcsb.workflow-0.38.tar` & `rcsb.workflow-0.39.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 18:04:08.958278 rcsb.workflow-0.38/
--rw-r--r--   0 vsts      (1001) docker     (122)     2275 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      106 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1839 2023-05-09 18:04:08.958278 rcsb.workflow-0.38/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1143 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 18:04:08.950277 rcsb.workflow-0.38/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 18:04:08.954277 rcsb.workflow-0.38/rcsb/workflow/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/rcsb/workflow/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 18:04:08.954277 rcsb.workflow-0.38/rcsb/workflow/chem/
--rw-r--r--   0 vsts      (1001) docker     (122)     3781 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/rcsb/workflow/chem/ChemCompFileWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5191 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/rcsb/workflow/chem/ChemCompImageWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3928 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/rcsb/workflow/chem/ChemCompSearchIndexWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/rcsb/workflow/chem/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 18:04:08.958278 rcsb.workflow-0.38/rcsb/workflow/targets/
--rw-r--r--   0 vsts      (1001) docker     (122)    10335 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/rcsb/workflow/targets/ProteinTargetSequenceExecutionWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)    28640 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/rcsb/workflow/targets/ProteinTargetSequenceWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/rcsb/workflow/targets/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 18:04:08.950277 rcsb.workflow-0.38/rcsb.workflow.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1839 2023-05-09 18:04:08.000000 rcsb.workflow-0.38/rcsb.workflow.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      661 2023-05-09 18:04:08.000000 rcsb.workflow-0.38/rcsb.workflow.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-09 18:04:08.000000 rcsb.workflow-0.38/rcsb.workflow.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-09 18:04:07.000000 rcsb.workflow-0.38/rcsb.workflow.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      196 2023-05-09 18:04:08.000000 rcsb.workflow-0.38/rcsb.workflow.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-09 18:04:08.000000 rcsb.workflow-0.38/rcsb.workflow.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      230 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-05-09 18:04:08.958278 rcsb.workflow-0.38/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2447 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:05:39.299165 rcsb.workflow-0.39/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2340 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      106 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1839 2023-05-23 16:05:39.299165 rcsb.workflow-0.39/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1143 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:05:39.295165 rcsb.workflow-0.39/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:05:39.299165 rcsb.workflow-0.39/rcsb/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/rcsb/workflow/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:05:39.299165 rcsb.workflow-0.39/rcsb/workflow/chem/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3781 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/rcsb/workflow/chem/ChemCompFileWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5191 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/rcsb/workflow/chem/ChemCompImageWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3928 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/rcsb/workflow/chem/ChemCompSearchIndexWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/rcsb/workflow/chem/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:05:39.299165 rcsb.workflow-0.39/rcsb/workflow/targets/
+-rw-r--r--   0 vsts      (1001) docker     (122)    10335 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/rcsb/workflow/targets/ProteinTargetSequenceExecutionWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    28640 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/rcsb/workflow/targets/ProteinTargetSequenceWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/rcsb/workflow/targets/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:05:39.299165 rcsb.workflow-0.39/rcsb.workflow.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1839 2023-05-23 16:05:39.000000 rcsb.workflow-0.39/rcsb.workflow.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      661 2023-05-23 16:05:39.000000 rcsb.workflow-0.39/rcsb.workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-23 16:05:39.000000 rcsb.workflow-0.39/rcsb.workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-23 16:05:38.000000 rcsb.workflow-0.39/rcsb.workflow.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      196 2023-05-23 16:05:39.000000 rcsb.workflow-0.39/rcsb.workflow.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-23 16:05:39.000000 rcsb.workflow-0.39/rcsb.workflow.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      230 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-05-23 16:05:39.299165 rcsb.workflow-0.39/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2447 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/setup.py
```

### Comparing `rcsb.workflow-0.38/HISTORY.txt` & `rcsb.workflow-0.39/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 29-Jul-2021 - V0.31 Broaden cache policy for cofactor providers.
 26-Aug-2021 - V0.32 Update dependencies
 27-Jun-2022 - V0.33 Change the molBuildType value from "model-xyz" to "connection-table" in ChemCompImageWorkflow()
  9-Jan-2023 - V0.34 Configuration changes to support tox 4
  3-Mar-2023 - V0.35 Standardize args in ProteinTargetSequenceExecutionWorkflow
 14-Mar-2023 - V0.36 Generate CARD annotations instead of features during ProteinTargetSequenceExecutionWorkflow
 21-Mar-2023 - V0.37 Allow backing up Pharos-targets to stash
- 5-May-2023 - V0.38 Add fromDbPharos and reloadPharos parameters to ProteinTargetSequenceExecutionWorkflow.exportFasta()
+ 5-May-2023 - V0.38 Add fromDbPharos and reloadPharos parameters to ProteinTargetSequenceExecutionWorkflow.exportFasta()
+22-May-2023 - V0.39 Add retries to tox task for MMseqs2 download
```

### Comparing `rcsb.workflow-0.38/LICENSE` & `rcsb.workflow-0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.38/PKG-INFO` & `rcsb.workflow-0.39/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.workflow
-Version: 0.38
+Version: 0.39
 Summary: RCSB Python data processing and ETL/ELT workflow entry points
 Home-page: https://github.com/rcsb/py-rcsb_workflow
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.workflow-0.38/README.md` & `rcsb.workflow-0.39/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.38/rcsb/workflow/chem/ChemCompFileWorkflow.py` & `rcsb.workflow-0.39/rcsb/workflow/chem/ChemCompFileWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.38/rcsb/workflow/chem/ChemCompImageWorkflow.py` & `rcsb.workflow-0.39/rcsb/workflow/chem/ChemCompImageWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.38/rcsb/workflow/chem/ChemCompSearchIndexWorkflow.py` & `rcsb.workflow-0.39/rcsb/workflow/chem/ChemCompSearchIndexWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.38/rcsb/workflow/targets/ProteinTargetSequenceExecutionWorkflow.py` & `rcsb.workflow-0.39/rcsb/workflow/targets/ProteinTargetSequenceExecutionWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.38/rcsb/workflow/targets/ProteinTargetSequenceWorkflow.py` & `rcsb.workflow-0.39/rcsb/workflow/targets/ProteinTargetSequenceWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.38/rcsb.workflow.egg-info/PKG-INFO` & `rcsb.workflow-0.39/rcsb.workflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.workflow
-Version: 0.38
+Version: 0.39
 Summary: RCSB Python data processing and ETL/ELT workflow entry points
 Home-page: https://github.com/rcsb/py-rcsb_workflow
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.workflow-0.38/rcsb.workflow.egg-info/SOURCES.txt` & `rcsb.workflow-0.39/rcsb.workflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.38/setup.py` & `rcsb.workflow-0.39/setup.py`

 * *Files identical despite different names*

