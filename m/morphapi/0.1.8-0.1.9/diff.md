# Comparing `tmp/morphapi-0.1.8.tar.gz` & `tmp/morphapi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphapi-0.1.8.tar", last modified: Fri Feb  3 14:54:42 2023, max compression
+gzip compressed data, was "morphapi-0.1.9.tar", last modified: Tue May 23 07:32:54 2023, max compression
```

## Comparing `morphapi-0.1.8.tar` & `morphapi-0.1.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:42.326296 morphapi-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-03 14:54:36.000000 morphapi-0.1.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:42.318296 morphapi-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:42.318296 morphapi-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-02-03 14:54:36.000000 morphapi-0.1.8/.github/workflows/build_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-02-03 14:54:36.000000 morphapi-0.1.8/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-02-03 14:54:36.000000 morphapi-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-03 14:54:36.000000 morphapi-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-03 14:54:36.000000 morphapi-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-02-03 14:54:42.326296 morphapi-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-02-03 14:54:36.000000 morphapi-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:42.318296 morphapi-0.1.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:42.318296 morphapi-0.1.8/examples/download/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-02-03 14:54:36.000000 morphapi-0.1.8/examples/download/allen_morphology_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-02-03 14:54:36.000000 morphapi-0.1.8/examples/download/mouselight_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-02-03 14:54:36.000000 morphapi-0.1.8/examples/download/mpin_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-02-03 14:54:36.000000 morphapi-0.1.8/examples/download/neuromorpho_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:42.322296 morphapi-0.1.8/examples/example_files/
--rw-r--r--   0 runner    (1001) docker     (123)   126929 2023-02-03 14:54:36.000000 morphapi-0.1.8/examples/example_files/example1.swc
--rw-r--r--   0 runner    (1001) docker     (123)   333147 2023-02-03 14:54:36.000000 morphapi-0.1.8/examples/example_files/example2.swc
--rw-r--r--   0 runner    (1001) docker     (123)   221587 2023-02-03 14:54:36.000000 morphapi-0.1.8/examples/example_files/example3.swc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:42.322296 morphapi-0.1.8/examples/visualise/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-02-03 14:54:36.000000 morphapi-0.1.8/examples/visualise/visualise_swc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:42.322296 morphapi-0.1.8/media/
--rw-r--r--   0 runner    (1001) docker     (123)   132923 2023-02-03 14:54:36.000000 morphapi-0.1.8/media/exampleneuron.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:42.322296 morphapi-0.1.8/morphapi/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 14:54:36.000000 morphapi-0.1.8/morphapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:42.322296 morphapi-0.1.8/morphapi/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:36.000000 morphapi-0.1.8/morphapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-02-03 14:54:36.000000 morphapi-0.1.8/morphapi/api/allenmorphology.py
--rw-r--r--   0 runner    (1001) docker     (123)    16871 2023-02-03 14:54:36.000000 morphapi-0.1.8/morphapi/api/mouselight.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-02-03 14:54:36.000000 morphapi-0.1.8/morphapi/api/mpin_celldb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-02-03 14:54:36.000000 morphapi-0.1.8/morphapi/api/neuromorphorg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:42.322296 morphapi-0.1.8/morphapi/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:36.000000 morphapi-0.1.8/morphapi/morphology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-02-03 14:54:36.000000 morphapi-0.1.8/morphapi/morphology/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-02-03 14:54:36.000000 morphapi-0.1.8/morphapi/morphology/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-02-03 14:54:36.000000 morphapi-0.1.8/morphapi/paths_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:42.322296 morphapi-0.1.8/morphapi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:36.000000 morphapi-0.1.8/morphapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-02-03 14:54:36.000000 morphapi-0.1.8/morphapi/utils/data_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-02-03 14:54:36.000000 morphapi-0.1.8/morphapi/utils/webqueries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:42.322296 morphapi-0.1.8/morphapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-02-03 14:54:42.000000 morphapi-0.1.8/morphapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-02-03 14:54:42.000000 morphapi-0.1.8/morphapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 14:54:42.000000 morphapi-0.1.8/morphapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 14:54:42.000000 morphapi-0.1.8/morphapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-02-03 14:54:42.000000 morphapi-0.1.8/morphapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-03 14:54:42.000000 morphapi-0.1.8/morphapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-02-03 14:54:36.000000 morphapi-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-03 14:54:36.000000 morphapi-0.1.8/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-03 14:54:42.326296 morphapi-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-02-03 14:54:36.000000 morphapi-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:42.322296 morphapi-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:36.000000 morphapi-0.1.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:42.326296 morphapi-0.1.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   126929 2023-02-03 14:54:36.000000 morphapi-0.1.8/tests/data/example1.swc
--rw-r--r--   0 runner    (1001) docker     (123)   333147 2023-02-03 14:54:36.000000 morphapi-0.1.8/tests/data/example2.swc
--rw-r--r--   0 runner    (1001) docker     (123)   221587 2023-02-03 14:54:36.000000 morphapi-0.1.8/tests/data/example3.swc
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-02-03 14:54:36.000000 morphapi-0.1.8/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-02-03 14:54:36.000000 morphapi-0.1.8/tests/test_neuron.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-02-03 14:54:36.000000 morphapi-0.1.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:32:54.353454 morphapi-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 07:32:48.000000 morphapi-0.1.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:32:54.341454 morphapi-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:32:54.345454 morphapi-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-23 07:32:48.000000 morphapi-0.1.9/.github/workflows/build_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-23 07:32:48.000000 morphapi-0.1.9/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-23 07:32:48.000000 morphapi-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-23 07:32:48.000000 morphapi-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 07:32:48.000000 morphapi-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-23 07:32:54.357455 morphapi-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-23 07:32:48.000000 morphapi-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:32:54.341454 morphapi-0.1.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:32:54.349454 morphapi-0.1.9/examples/download/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-23 07:32:48.000000 morphapi-0.1.9/examples/download/allen_morphology_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-23 07:32:48.000000 morphapi-0.1.9/examples/download/mouselight_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-23 07:32:48.000000 morphapi-0.1.9/examples/download/mpin_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-23 07:32:48.000000 morphapi-0.1.9/examples/download/neuromorpho_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:32:54.349454 morphapi-0.1.9/examples/example_files/
+-rw-r--r--   0 runner    (1001) docker     (123)   126929 2023-05-23 07:32:48.000000 morphapi-0.1.9/examples/example_files/example1.swc
+-rw-r--r--   0 runner    (1001) docker     (123)   333147 2023-05-23 07:32:48.000000 morphapi-0.1.9/examples/example_files/example2.swc
+-rw-r--r--   0 runner    (1001) docker     (123)   221587 2023-05-23 07:32:48.000000 morphapi-0.1.9/examples/example_files/example3.swc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:32:54.349454 morphapi-0.1.9/examples/visualise/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-23 07:32:48.000000 morphapi-0.1.9/examples/visualise/visualise_swc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:32:54.349454 morphapi-0.1.9/media/
+-rw-r--r--   0 runner    (1001) docker     (123)   132923 2023-05-23 07:32:48.000000 morphapi-0.1.9/media/exampleneuron.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:32:54.349454 morphapi-0.1.9/morphapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:32:48.000000 morphapi-0.1.9/morphapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:32:54.353454 morphapi-0.1.9/morphapi/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:32:48.000000 morphapi-0.1.9/morphapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-05-23 07:32:48.000000 morphapi-0.1.9/morphapi/api/allenmorphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16873 2023-05-23 07:32:48.000000 morphapi-0.1.9/morphapi/api/mouselight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-05-23 07:32:48.000000 morphapi-0.1.9/morphapi/api/mpin_celldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-23 07:32:48.000000 morphapi-0.1.9/morphapi/api/neuromorphorg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:32:54.353454 morphapi-0.1.9/morphapi/morphology/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:32:48.000000 morphapi-0.1.9/morphapi/morphology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-05-23 07:32:48.000000 morphapi-0.1.9/morphapi/morphology/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-05-23 07:32:48.000000 morphapi-0.1.9/morphapi/morphology/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-23 07:32:48.000000 morphapi-0.1.9/morphapi/paths_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:32:54.353454 morphapi-0.1.9/morphapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:32:48.000000 morphapi-0.1.9/morphapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-23 07:32:48.000000 morphapi-0.1.9/morphapi/utils/data_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-23 07:32:48.000000 morphapi-0.1.9/morphapi/utils/webqueries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:32:54.349454 morphapi-0.1.9/morphapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-23 07:32:54.000000 morphapi-0.1.9/morphapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-23 07:32:54.000000 morphapi-0.1.9/morphapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:32:54.000000 morphapi-0.1.9/morphapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:32:54.000000 morphapi-0.1.9/morphapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-23 07:32:54.000000 morphapi-0.1.9/morphapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-23 07:32:54.000000 morphapi-0.1.9/morphapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-23 07:32:48.000000 morphapi-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-23 07:32:48.000000 morphapi-0.1.9/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-23 07:32:54.357455 morphapi-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-23 07:32:48.000000 morphapi-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:32:54.353454 morphapi-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:32:48.000000 morphapi-0.1.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:32:54.353454 morphapi-0.1.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   126929 2023-05-23 07:32:48.000000 morphapi-0.1.9/tests/data/example1.swc
+-rw-r--r--   0 runner    (1001) docker     (123)   333147 2023-05-23 07:32:48.000000 morphapi-0.1.9/tests/data/example2.swc
+-rw-r--r--   0 runner    (1001) docker     (123)   221587 2023-05-23 07:32:48.000000 morphapi-0.1.9/tests/data/example3.swc
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-23 07:32:48.000000 morphapi-0.1.9/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-23 07:32:48.000000 morphapi-0.1.9/tests/test_neuron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-23 07:32:48.000000 morphapi-0.1.9/tox.ini
```

### Comparing `morphapi-0.1.8/.github/workflows/build_and_publish.yml` & `morphapi-0.1.9/.github/workflows/build_and_publish.yml`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/.github/workflows/run-tests.yml` & `morphapi-0.1.9/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/.gitignore` & `morphapi-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/LICENSE` & `morphapi-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/PKG-INFO` & `morphapi-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphapi
-Version: 0.1.8
+Version: 0.1.9
 Summary: A lightweight python package to download neuronal morphologies
 Home-page: https://github.com/brainglobe/morphapi
 Author: Federico Claudi
 License: UNKNOWN
 Description: # morphapi
         
         ## Overview
```

### Comparing `morphapi-0.1.8/examples/download/allen_morphology_api.py` & `morphapi-0.1.9/examples/download/allen_morphology_api.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/examples/download/mouselight_api.py` & `morphapi-0.1.9/examples/download/mouselight_api.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/examples/download/mpin_api.py` & `morphapi-0.1.9/examples/download/mpin_api.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/examples/download/neuromorpho_api.py` & `morphapi-0.1.9/examples/download/neuromorpho_api.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/examples/example_files/example1.swc` & `morphapi-0.1.9/examples/example_files/example1.swc`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/examples/example_files/example2.swc` & `morphapi-0.1.9/examples/example_files/example2.swc`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/examples/example_files/example3.swc` & `morphapi-0.1.9/examples/example_files/example3.swc`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/examples/visualise/visualise_swc.py` & `morphapi-0.1.9/examples/visualise/visualise_swc.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/media/exampleneuron.png` & `morphapi-0.1.9/media/exampleneuron.png`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/morphapi/api/allenmorphology.py` & `morphapi-0.1.9/morphapi/api/allenmorphology.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/morphapi/api/mouselight.py` & `morphapi-0.1.9/morphapi/api/mouselight.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 from morphapi.utils.webqueries import mouselight_base_url
 from morphapi.utils.webqueries import post_mouselight
 
 logger = logging.getLogger(__name__)
 
 
 """
-    Collections of functions to query http://ml-neuronbrowser.janelia.org/ and get data about either the status of the API,
+    Collections of functions to query https://ml-neuronbrowser.janelia.org/ and get data about either the status of the API,
     the brain regions or the neurons available.
-    Queries are sent by sending POST requests to http://ml-neuronbrowser.janelia.org/graphql
+    Queries are sent by sending POST requests to https://ml-neuronbrowser.janelia.org/graphql
     with a string query.
 """
 
 # ---------------------------------------------------------------------------- #
 #                                  QUERY UTILS                                 #
 # ---------------------------------------------------------------------------- #
```

### Comparing `morphapi-0.1.8/morphapi/api/mpin_celldb.py` & `morphapi-0.1.9/morphapi/api/mpin_celldb.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/morphapi/api/neuromorphorg.py` & `morphapi-0.1.9/morphapi/api/neuromorphorg.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,19 +37,26 @@
             "Neuron Fields"
         ]
 
     def get_fields_values(self, field):
         """
         Returns the list of allowed values for a given query field
         """
-        return list(
-            request_no_ssl(self._base_url + f"/fields/{field}").json()[
-                "fields"
-            ]
-        )
+        current_page = 0
+        max_page = 1
+        values = []
+        while current_page < max_page:
+            req = request_no_ssl(
+                self._base_url
+                + f"/fields/{field}?&size=1000&page={current_page}"
+            ).json()
+            values.extend(req["fields"])
+            max_page = req.get("page", {}).get("totalPages", max_page)
+            current_page += 1
+        return values
 
     def get_neurons_metadata(self, size=100, page=0, **criteria):
         """
         Uses the neuromorpho API to download metadata about neurons.
         Criteri can be used to restrict the search to neurons of interest/
         https://neuromorpho.org/apiReference.html
 
@@ -125,24 +132,33 @@
     def build_filepath(self, neuron_id):
         """
         Build a filepath from a neuron ID.
         """
         return os.path.join(self.neuromorphorg_cache, f"{neuron_id}.swc")
 
     def download_neurons(
-        self, neurons, _name=None, load_neurons=True, **kwargs
+        self,
+        neurons,
+        _name=None,
+        load_neurons=True,
+        use_neuron_names=False,
+        **kwargs,
     ):
         """
         Downloads neuronal morphological data and saves it to .swc files.
         It then returns a list of Neuron instances with morphological data for each neuron.
 
         :param neurons: list of neurons metadata (as returned by one of the functions
-                    used to fetch metadata)
+            used to fetch metadata)
         :param _name: used internally to save cached neurons with a different prefix when the
-                class is used to download neurons for other APIs
+            class is used to download neurons for other APIs
+        :param load_neurons: if set to True, the neurons are loaded into a
+            `morphapi.morphology.morphology.Neuron` object and returned
+        :param use_neuron_names: if set to True, the filenames use the names of the neurons instead
+            of their IDs
         """
         if not isinstance(neurons, (list, tuple)):
             neurons = [neurons]
 
         to_return = []
         for neuron in neurons:
             if not isinstance(neuron, dict):
@@ -150,15 +166,20 @@
 
             try:
                 neuron["status"] == 500  # download went wrong
                 continue
             except KeyError:
                 pass
 
-            filepath = self.build_filepath(neuron["neuron_id"])
+            if use_neuron_names:
+                filepath = self.build_filepath(
+                    neuron.get("neuron_name", neuron["neuron_id"])
+                )
+            else:
+                filepath = self.build_filepath(neuron["neuron_id"])
             load_current_neuron = load_neurons
 
             if not os.path.isfile(filepath):
                 # Download and write to file
                 if self._version == "CNG version":
                     url = f"https://neuromorpho.org/dableFiles/{neuron['archive'].lower()}/CNG version/{neuron['neuron_name']}.CNG.swc"
                 else:
```

### Comparing `morphapi-0.1.8/morphapi/morphology/cache.py` & `morphapi-0.1.9/morphapi/morphology/cache.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/morphapi/morphology/morphology.py` & `morphapi-0.1.9/morphapi/morphology/morphology.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/morphapi/paths_manager.py` & `morphapi-0.1.9/morphapi/paths_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         :param kwargs: use the name of a folder as key and a path as argument to specify the path of individual subfolders
         """
         # Get and make base directory
 
         if base_dir is None:
             self.base_dir = Path.home() / ".morphapi"
         else:
-            self.base_dir = base_dir
+            self.base_dir = Path(base_dir)
 
         self.base_dir.mkdir(exist_ok=True)
 
         for fld_name, folder in default_paths.items():
             # Check if user provided a path for this folder, otherwise use default
 
             path = self.base_dir / kwargs.pop(fld_name, folder)
```

### Comparing `morphapi-0.1.8/morphapi/utils/data_io.py` & `morphapi-0.1.9/morphapi/utils/data_io.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/morphapi/utils/webqueries.py` & `morphapi-0.1.9/morphapi/utils/webqueries.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/morphapi.egg-info/PKG-INFO` & `morphapi-0.1.9/morphapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphapi
-Version: 0.1.8
+Version: 0.1.9
 Summary: A lightweight python package to download neuronal morphologies
 Home-page: https://github.com/brainglobe/morphapi
 Author: Federico Claudi
 License: UNKNOWN
 Description: # morphapi
         
         ## Overview
```

### Comparing `morphapi-0.1.8/morphapi.egg-info/SOURCES.txt` & `morphapi-0.1.9/morphapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/setup.py` & `morphapi-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/tests/data/example1.swc` & `morphapi-0.1.9/tests/data/example1.swc`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/tests/data/example2.swc` & `morphapi-0.1.9/tests/data/example2.swc`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/tests/data/example3.swc` & `morphapi-0.1.9/tests/data/example3.swc`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/tests/test_download.py` & `morphapi-0.1.9/tests/test_download.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,71 @@
+from pathlib import Path
+
 from morphapi.api.allenmorphology import AllenMorphology
 from morphapi.api.mouselight import MouseLightAPI
 from morphapi.api.neuromorphorg import NeuroMorpOrgAPI
 
 
-def test_neuromorpho_download():
-    api = NeuroMorpOrgAPI()
+def test_neuromorpho_download(tmpdir):
+    api = NeuroMorpOrgAPI(base_dir=tmpdir)
+    cache_path = Path(api.neuromorphorg_cache)
+
     metadata, _ = api.get_neurons_metadata(
         size=2,  # Can get the metadata for up to 500 neurons at the time
         species="mouse",
         cell_type="pyramidal",
         brain_region="neocortex",
     )
 
     if len(metadata) != 2:
         raise ValueError("Incorrect metadata length")
 
+    assert len(list(cache_path.iterdir())) == 0
     neurons = api.download_neurons(metadata)
 
-    if len(neurons) != len(metadata):
-        raise ValueError
+    assert len(neurons) == len(metadata)
+    assert len(list(cache_path.iterdir())) == 2
 
     neurons = [neuron.create_mesh()[1] for neuron in neurons]
 
     # Test no load
     assert api.download_neurons(metadata, load_neurons=False)[0].points is None
+    assert len(list(cache_path.iterdir())) == 2
+
+    # Test using neuron names
+    assert (
+        api.download_neurons(
+            metadata, load_neurons=False, use_neuron_names=True
+        )[0].points
+        is None
+    )
+    assert len(list(cache_path.iterdir())) == 4
+
+    cache_files = list(cache_path.iterdir())
+    assert sorted([i.name for i in cache_files]) == [
+        "10075.swc",
+        "10076.swc",
+        "C1q-Cell7-40x.swc",
+        "Ctrl-Cell3-40x.swc",
+    ]
 
     # Test failure
     metadata[0]["neuron_id"] = "BAD ID"
     metadata[0]["neuron_name"] = "BAD NAME"
     neurons = api.download_neurons([metadata[0]])
 
     assert neurons[0].data_file.name == "BAD ID.swc"
     assert neurons[0].points is None
 
+    # Test get_fields_values
+    assert len(api.get_fields_values("strain")) > 1000
+
 
-def test_mouselight_download():
-    mlapi = MouseLightAPI()
+def test_mouselight_download(tmpdir):
+    mlapi = MouseLightAPI(base_dir=tmpdir)
 
     neurons_metadata = mlapi.fetch_neurons_metadata(
         filterby="soma", filter_regions=["MOs"]
     )
     neurons_metadata = sorted(neurons_metadata, key=lambda x: x["idString"])
 
     neurons = mlapi.download_neurons(neurons_metadata[0])
@@ -83,16 +109,16 @@
             i["brainArea_acronym"] == "MOs6b"
             for i in filtered_neurons_metadata_atlas
         ]
     )
     assert filtered_neurons_metadata == filtered_neurons_metadata_atlas
 
 
-def test_allen_morphology_download():
-    am = AllenMorphology()
+def test_allen_morphology_download(tmpdir):
+    am = AllenMorphology(base_dir=tmpdir)
 
     # Select some mouse neurons in the primary visual cortex
     neurons_df = am.neurons.loc[
         (am.neurons.species == "Mus musculus")
         & (am.neurons.structure_area_abbrev == "VISp")
     ].loc[[2, 120, 505]]
```

### Comparing `morphapi-0.1.8/tests/test_neuron.py` & `morphapi-0.1.9/tests/test_neuron.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.1.8/tox.ini` & `morphapi-0.1.9/tox.ini`

 * *Files identical despite different names*

