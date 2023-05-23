# Comparing `tmp/simcardems-2023.4.2.tar.gz` & `tmp/simcardems-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simcardems-2023.4.2.tar", last modified: Mon May 22 19:01:17 2023, max compression
+gzip compressed data, was "simcardems-2023.5.0.tar", last modified: Tue May 23 19:15:48 2023, max compression
```

## Comparing `simcardems-2023.4.2.tar` & `simcardems-2023.5.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:01:17.577035 simcardems-2023.4.2/
--rw-r--r--   0 root         (0) root         (0)    26526 2023-05-22 18:51:36.000000 simcardems-2023.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3845 2023-05-22 19:01:17.577035 simcardems-2023.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3141 2023-05-22 18:51:36.000000 simcardems-2023.4.2/README.md
--rw-r--r--   0 root         (0) root         (0)     1831 2023-05-22 19:01:17.581035 simcardems-2023.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      296 2023-05-22 18:51:36.000000 simcardems-2023.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:01:17.569035 simcardems-2023.4.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:01:17.573035 simcardems-2023.4.2/src/simcardems/
--rw-r--r--   0 root         (0) root         (0)     3453 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2388 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/benchmark.py
--rw-r--r--   0 root         (0) root         (0)     5423 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/boundary_conditions.py
--rw-r--r--   0 root         (0) root         (0)     9241 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/cli.py
--rw-r--r--   0 root         (0) root         (0)     1919 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/config.py
--rw-r--r--   0 root         (0) root         (0)    18669 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/datacollector.py
--rw-r--r--   0 root         (0) root         (0)    10019 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/ep_model.py
--rw-r--r--   0 root         (0) root         (0)    17148 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/geometry.py
--rw-r--r--   0 root         (0) root         (0)    11745 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/gui.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/lvgeometry.py
--rw-r--r--   0 root         (0) root         (0)    11482 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/mechanics_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:01:17.577035 simcardems-2023.4.2/src/simcardems/models/
--rw-r--r--   0 root         (0) root         (0)      703 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      333 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/cell_model.py
--rw-r--r--   0 root         (0) root         (0)     6841 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:01:17.577035 simcardems-2023.4.2/src/simcardems/models/explicit_ORdmm_Land/
--rw-r--r--   0 root         (0) root         (0)      819 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/explicit_ORdmm_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60760 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/explicit_ORdmm_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)    14164 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/explicit_ORdmm_Land/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:01:17.577035 simcardems-2023.4.2/src/simcardems/models/fully_coupled_ORdmm_Land/
--rw-r--r--   0 root         (0) root         (0)      567 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6993 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py
--rw-r--r--   0 root         (0) root         (0)    60344 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)    12046 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:01:17.577035 simcardems-2023.4.2/src/simcardems/models/fully_coupled_Tor_Land/
--rw-r--r--   0 root         (0) root         (0)      559 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/fully_coupled_Tor_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6989 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/fully_coupled_Tor_Land/active_model.py
--rw-r--r--   0 root         (0) root         (0)    70634 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)    12043 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/fully_coupled_Tor_Land/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:01:17.577035 simcardems-2023.4.2/src/simcardems/models/pureEP_ORdmm_Land/
--rw-r--r--   0 root         (0) root         (0)      419 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/pureEP_ORdmm_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60636 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)     5012 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/models/pureEP_ORdmm_Land/em_model.py
--rw-r--r--   0 root         (0) root         (0)     5730 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/newton_solver.py
--rw-r--r--   0 root         (0) root         (0)    21621 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/postprocess.py
--rw-r--r--   0 root         (0) root         (0)     7156 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/runner.py
--rw-r--r--   0 root         (0) root         (0)     6485 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/save_load_functions.py
--rw-r--r--   0 root         (0) root         (0)     4515 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/slabgeometry.py
--rw-r--r--   0 root         (0) root         (0)     2642 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/time_stepper.py
--rw-r--r--   0 root         (0) root         (0)     5462 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/utils.py
--rw-r--r--   0 root         (0) root         (0)     4826 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/value_extractor.py
--rw-r--r--   0 root         (0) root         (0)       25 2023-05-22 18:51:36.000000 simcardems-2023.4.2/src/simcardems/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:01:17.573035 simcardems-2023.4.2/src/simcardems.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3845 2023-05-22 19:01:17.000000 simcardems-2023.4.2/src/simcardems.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2052 2023-05-22 19:01:17.000000 simcardems-2023.4.2/src/simcardems.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 19:01:17.000000 simcardems-2023.4.2/src/simcardems.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-05-22 19:01:17.000000 simcardems-2023.4.2/src/simcardems.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 18:51:58.000000 simcardems-2023.4.2/src/simcardems.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      337 2023-05-22 19:01:17.000000 simcardems-2023.4.2/src/simcardems.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-22 19:01:17.000000 simcardems-2023.4.2/src/simcardems.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:01:17.577035 simcardems-2023.4.2/tests/
--rw-r--r--   0 root         (0) root         (0)      523 2023-05-22 18:51:36.000000 simcardems-2023.4.2/tests/test_boundary_conditions.py
--rw-r--r--   0 root         (0) root         (0)     3454 2023-05-22 18:51:36.000000 simcardems-2023.4.2/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     2974 2023-05-22 18:51:36.000000 simcardems-2023.4.2/tests/test_datacollector.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-05-22 18:51:36.000000 simcardems-2023.4.2/tests/test_geometry.py
--rw-r--r--   0 root         (0) root         (0)     3507 2023-05-22 18:51:36.000000 simcardems-2023.4.2/tests/test_mechanics_model.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-05-22 18:51:36.000000 simcardems-2023.4.2/tests/test_models.py
--rw-r--r--   0 root         (0) root         (0)     2793 2023-05-22 18:51:36.000000 simcardems-2023.4.2/tests/test_postprocessing.py
--rw-r--r--   0 root         (0) root         (0)     1956 2023-05-22 18:51:36.000000 simcardems-2023.4.2/tests/test_runner.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-05-22 18:51:36.000000 simcardems-2023.4.2/tests/test_save_load_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:15:48.834749 simcardems-2023.5.0/
+-rw-r--r--   0 root         (0) root         (0)    26526 2023-05-23 19:05:37.000000 simcardems-2023.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3845 2023-05-23 19:15:48.834749 simcardems-2023.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3141 2023-05-23 19:05:37.000000 simcardems-2023.5.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-05-23 19:15:48.834749 simcardems-2023.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      296 2023-05-23 19:05:37.000000 simcardems-2023.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:15:48.826749 simcardems-2023.5.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:15:48.830749 simcardems-2023.5.0/src/simcardems/
+-rw-r--r--   0 root         (0) root         (0)     3453 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     9954 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/benchmark.py
+-rw-r--r--   0 root         (0) root         (0)     5423 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/boundary_conditions.py
+-rw-r--r--   0 root         (0) root         (0)     9241 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/config.py
+-rw-r--r--   0 root         (0) root         (0)    18669 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/datacollector.py
+-rw-r--r--   0 root         (0) root         (0)    10019 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/ep_model.py
+-rw-r--r--   0 root         (0) root         (0)    17148 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/geometry.py
+-rw-r--r--   0 root         (0) root         (0)    11745 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/gui.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/lvgeometry.py
+-rw-r--r--   0 root         (0) root         (0)    11482 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/mechanics_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:15:48.830749 simcardems-2023.5.0/src/simcardems/models/
+-rw-r--r--   0 root         (0) root         (0)      703 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      333 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/models/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)     6841 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/models/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:15:48.834749 simcardems-2023.5.0/src/simcardems/models/explicit_ORdmm_Land/
+-rw-r--r--   0 root         (0) root         (0)      819 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/models/explicit_ORdmm_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60760 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/models/explicit_ORdmm_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)    14164 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/models/explicit_ORdmm_Land/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:15:48.834749 simcardems-2023.5.0/src/simcardems/models/fully_coupled_ORdmm_Land/
+-rw-r--r--   0 root         (0) root         (0)      567 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6993 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py
+-rw-r--r--   0 root         (0) root         (0)    60344 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)    12046 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:15:48.834749 simcardems-2023.5.0/src/simcardems/models/fully_coupled_Tor_Land/
+-rw-r--r--   0 root         (0) root         (0)      559 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/models/fully_coupled_Tor_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6989 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/models/fully_coupled_Tor_Land/active_model.py
+-rw-r--r--   0 root         (0) root         (0)    70634 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)    12043 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/models/fully_coupled_Tor_Land/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:15:48.834749 simcardems-2023.5.0/src/simcardems/models/pureEP_ORdmm_Land/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/models/pureEP_ORdmm_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60636 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)     5012 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/models/pureEP_ORdmm_Land/em_model.py
+-rw-r--r--   0 root         (0) root         (0)     5730 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/newton_solver.py
+-rw-r--r--   0 root         (0) root         (0)    21874 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/postprocess.py
+-rw-r--r--   0 root         (0) root         (0)     7156 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/runner.py
+-rw-r--r--   0 root         (0) root         (0)     6485 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/save_load_functions.py
+-rw-r--r--   0 root         (0) root         (0)     4515 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/slabgeometry.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/time_stepper.py
+-rw-r--r--   0 root         (0) root         (0)     5462 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4826 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/value_extractor.py
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-23 19:05:37.000000 simcardems-2023.5.0/src/simcardems/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:15:48.830749 simcardems-2023.5.0/src/simcardems.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3845 2023-05-23 19:15:48.000000 simcardems-2023.5.0/src/simcardems.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-05-23 19:15:48.000000 simcardems-2023.5.0/src/simcardems.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 19:15:48.000000 simcardems-2023.5.0/src/simcardems.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-05-23 19:15:48.000000 simcardems-2023.5.0/src/simcardems.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 19:05:59.000000 simcardems-2023.5.0/src/simcardems.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      337 2023-05-23 19:15:48.000000 simcardems-2023.5.0/src/simcardems.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-23 19:15:48.000000 simcardems-2023.5.0/src/simcardems.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:15:48.834749 simcardems-2023.5.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      523 2023-05-23 19:05:37.000000 simcardems-2023.5.0/tests/test_boundary_conditions.py
+-rw-r--r--   0 root         (0) root         (0)     3454 2023-05-23 19:05:37.000000 simcardems-2023.5.0/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     2974 2023-05-23 19:05:37.000000 simcardems-2023.5.0/tests/test_datacollector.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-05-23 19:05:37.000000 simcardems-2023.5.0/tests/test_geometry.py
+-rw-r--r--   0 root         (0) root         (0)     3507 2023-05-23 19:05:37.000000 simcardems-2023.5.0/tests/test_mechanics_model.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-05-23 19:05:37.000000 simcardems-2023.5.0/tests/test_models.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2023-05-23 19:05:37.000000 simcardems-2023.5.0/tests/test_postprocessing.py
+-rw-r--r--   0 root         (0) root         (0)     1956 2023-05-23 19:05:37.000000 simcardems-2023.5.0/tests/test_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-05-23 19:05:37.000000 simcardems-2023.5.0/tests/test_save_load_functions.py
```

### Comparing `simcardems-2023.4.2/LICENSE` & `simcardems-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/PKG-INFO` & `simcardems-2023.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simcardems
-Version: 2023.4.2
+Version: 2023.5.0
 Summary: Simula Cardiac electromechanics solver
 Home-page: https://github.com/ComputationalPhysiology/simcardems
 Author: Henrik Finsberg, Ilsbeth van Herck, Cécile Daversin-Catty
 Author-email: henriknf@simula.no
 License: LGPL-2.1
 Keywords: action potential,cardiac mechanics,electrophysiology,electromechanics
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
```

### Comparing `simcardems-2023.4.2/README.md` & `simcardems-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/setup.cfg` & `simcardems-2023.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/__init__.py` & `simcardems-2023.5.0/src/simcardems/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/boundary_conditions.py` & `simcardems-2023.5.0/src/simcardems/boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/cli.py` & `simcardems-2023.5.0/src/simcardems/cli.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/config.py` & `simcardems-2023.5.0/src/simcardems/config.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/datacollector.py` & `simcardems-2023.5.0/src/simcardems/datacollector.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/ep_model.py` & `simcardems-2023.5.0/src/simcardems/ep_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/geometry.py` & `simcardems-2023.5.0/src/simcardems/geometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/gui.py` & `simcardems-2023.5.0/src/simcardems/gui.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/lvgeometry.py` & `simcardems-2023.5.0/src/simcardems/lvgeometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/mechanics_model.py` & `simcardems-2023.5.0/src/simcardems/mechanics_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/models/__init__.py` & `simcardems-2023.5.0/src/simcardems/models/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/models/em_model.py` & `simcardems-2023.5.0/src/simcardems/models/em_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/models/explicit_ORdmm_Land/__init__.py` & `simcardems-2023.5.0/src/simcardems/models/explicit_ORdmm_Land/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/models/explicit_ORdmm_Land/cell_model.py` & `simcardems-2023.5.0/src/simcardems/models/explicit_ORdmm_Land/cell_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/models/explicit_ORdmm_Land/em_model.py` & `simcardems-2023.5.0/src/simcardems/models/explicit_ORdmm_Land/em_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py` & `simcardems-2023.5.0/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py` & `simcardems-2023.5.0/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py` & `simcardems-2023.5.0/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py` & `simcardems-2023.5.0/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/models/fully_coupled_Tor_Land/__init__.py` & `simcardems-2023.5.0/src/simcardems/models/fully_coupled_Tor_Land/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/models/fully_coupled_Tor_Land/active_model.py` & `simcardems-2023.5.0/src/simcardems/models/fully_coupled_Tor_Land/active_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py` & `simcardems-2023.5.0/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/models/fully_coupled_Tor_Land/em_model.py` & `simcardems-2023.5.0/src/simcardems/models/fully_coupled_Tor_Land/em_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py` & `simcardems-2023.5.0/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/models/pureEP_ORdmm_Land/em_model.py` & `simcardems-2023.5.0/src/simcardems/models/pureEP_ORdmm_Land/em_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/newton_solver.py` & `simcardems-2023.5.0/src/simcardems/newton_solver.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/postprocess.py` & `simcardems-2023.5.0/src/simcardems/postprocess.py`

 * *Files 7% similar despite different names*

```diff
@@ -352,56 +352,76 @@
         end = len(time)
 
     if return_interval:
         return lastbeat.y, lastbeat.t, (start, end)
     return lastbeat.y, lastbeat.t
 
 
-def extract_biomarkers(V, Ta, time, Ca, lmbda, inv_lmbda, u):
+def extract_biomarkers(
+    *,
+    V: np.ndarray,
+    time: np.ndarray,
+    Ca: np.ndarray,
+    Ta: Optional[np.ndarray] = None,
+    lmbda: Optional[np.ndarray] = None,
+    inv_lmbda: Optional[np.ndarray] = None,
+    u: Optional[np.ndarray] = None,
+) -> Dict[str, float]:
     d = {}
-    d["maxTa"] = np.max(Ta)
-    d["ampTa"] = np.max(Ta) - np.min(Ta)
-    d["APD40"] = find_duration(V, time, 40)
-    d["APD50"] = find_duration(V, time, 50)
-    d["APD90"] = find_duration(V, time, 90)
-    d["triangulation"] = d["APD90"] - d["APD40"]
+
+    V_beat = apf.Beat(y=V, t=time)
+    Ca_beat = apf.Beat(y=Ca, t=time)
+
+    d["APD40"] = V_beat.apd(40)
+    d["APD50"] = V_beat.apd(50)
+    d["APD90"] = V_beat.apd(90)
+    d["triangulation"] = V_beat.triangulation(high=90, low=40)
     d["Vpeak"] = np.max(V)
     d["Vmin"] = np.min(V)
-    d["dvdt"] = (V[1] - V[0]) / 2.0
+    d["dvdt_max"] = V_beat.maximum_upstroke_velocity()
     d["maxCa"] = np.max(Ca)
     d["ampCa"] = np.max(Ca) - np.min(Ca)
-    d["CaTD50"] = find_duration(Ca, time, 50)
-    d["CaTD80"] = find_duration(Ca, time, 80)
-    d["CaTD90"] = find_duration(Ca, time, 90)
-    d["ttp_Ta"] = find_ttp(Ta, time)
-    d["rt50_Ta"] = find_decaytime(Ta, time, 50)
-    d["rt95_Ta"] = find_decaytime(Ta, time, 5)
-    d["maxlmbda"] = np.max(lmbda)
-    d["minlmbda"] = np.min(lmbda)
-    d["ttplmbda"] = find_ttp(inv_lmbda, time)
-    d["lmbdaD50"] = find_duration(inv_lmbda, time, 50)
-    d["lmbdaD80"] = find_duration(inv_lmbda, time, 80)
-    d["lmbdaD90"] = find_duration(inv_lmbda, time, 90)
-    d["rt50_lmbda"] = find_decaytime(inv_lmbda, time, 50)
-    d["rt95_lmbda"] = find_decaytime(inv_lmbda, time, 5)
-
-    u_norm = np.linalg.norm(u, axis=1)
-    ux, uy, uz = u.T
-    for name, arr in zip(["norm", "x", "y", "z"], [u_norm, ux, uy, uz]):
-        d[f"max_displacement_{name}"] = np.abs(np.max(arr))
-        d[f"rel_max_displacement_{name}"] = np.abs(
-            np.min(arr) - np.max(arr),
-        )
-        d[f"max_displacement_perc_{name}"] = d[f"max_displacement_{name}"] * 100 / 20.0
-        d[f"rel_max_displacement_perc_{name}"] = (
-            d[f"rel_max_displacement_{name}"] * 100 / (20.0 - np.abs(np.max(arr)))
-        )
-        d[f"time_to_max_displacement_{name}"] = (
-            time[np.where(arr == np.min(arr))[0][0]] % 1000
-        )
+    d["CaTD50"] = Ca_beat.apd(50)
+    d["CaTD80"] = Ca_beat.apd(80)
+
+    if Ta is not None:
+        Ta_beat = apf.Beat(Ta)
+        d["maxTa"] = np.max(Ta.y)
+        d["ampTa"] = np.max(Ta.y) - np.min(Ta.y)
+        d["ttp_Ta"] = Ta_beat.ttp()
+        d["rt50_Ta"] = Ta_beat.tau(50)
+        d["rt95_Ta"] = Ta_beat.tau(5)
+    if lmbda is not None:
+        d["maxlmbda"] = np.max(lmbda)
+        d["minlmbda"] = np.min(lmbda)
+
+    if inv_lmbda is not None:
+        inv_lmbda_beat = apf.Beat(y=inv_lmbda, t=time)
+        d["ttplmbda"] = inv_lmbda_beat.ttp()
+        d["lmbdaD50"] = inv_lmbda_beat.apd(50)
+        d["lmbdaD80"] = inv_lmbda_beat.apd(80)
+        d["lmbdaD90"] = inv_lmbda_beat.apd(90)
+        d["rt50_lmbda"] = inv_lmbda_beat.tau(50)
+        d["rt95_lmbda"] = inv_lmbda_beat.tau(5)
+
+    if u is not None:
+        u_norm = np.linalg.norm(u, axis=1)
+        ux, uy, uz = u.T
+        for name, arr in zip(["norm", "x", "y", "z"], [u_norm, ux, uy, uz]):
+            d[f"max_displacement_{name}"] = np.max(arr)
+            d[f"min_displacement_{name}"] = np.min(arr)
+            d[f"time_to_max_displacement_{name}"] = apf.features.time_to_peak(
+                y=arr,
+                x=time,
+            )
+            d[f"time_to_min_displacement_{name}"] = apf.features.time_to_peak(
+                y=-arr,
+                x=time,
+            )
+
     return d
 
 
 def get_biomarkers(results, outdir, num_models):
     biomarker_dict = {}
     fig, ax = plt.subplots()
     for PoMm in range(1, num_models + 1):
```

### Comparing `simcardems-2023.4.2/src/simcardems/runner.py` & `simcardems-2023.5.0/src/simcardems/runner.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/save_load_functions.py` & `simcardems-2023.5.0/src/simcardems/save_load_functions.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/slabgeometry.py` & `simcardems-2023.5.0/src/simcardems/slabgeometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/time_stepper.py` & `simcardems-2023.5.0/src/simcardems/time_stepper.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/utils.py` & `simcardems-2023.5.0/src/simcardems/utils.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems/value_extractor.py` & `simcardems-2023.5.0/src/simcardems/value_extractor.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/src/simcardems.egg-info/PKG-INFO` & `simcardems-2023.5.0/src/simcardems.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simcardems
-Version: 2023.4.2
+Version: 2023.5.0
 Summary: Simula Cardiac electromechanics solver
 Home-page: https://github.com/ComputationalPhysiology/simcardems
 Author: Henrik Finsberg, Ilsbeth van Herck, Cécile Daversin-Catty
 Author-email: henriknf@simula.no
 License: LGPL-2.1
 Keywords: action potential,cardiac mechanics,electrophysiology,electromechanics
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
```

### Comparing `simcardems-2023.4.2/src/simcardems.egg-info/SOURCES.txt` & `simcardems-2023.5.0/src/simcardems.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/tests/test_boundary_conditions.py` & `simcardems-2023.5.0/tests/test_boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/tests/test_cli.py` & `simcardems-2023.5.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/tests/test_datacollector.py` & `simcardems-2023.5.0/tests/test_datacollector.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/tests/test_geometry.py` & `simcardems-2023.5.0/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/tests/test_mechanics_model.py` & `simcardems-2023.5.0/tests/test_mechanics_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/tests/test_models.py` & `simcardems-2023.5.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/tests/test_postprocessing.py` & `simcardems-2023.5.0/tests/test_postprocessing.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/tests/test_runner.py` & `simcardems-2023.5.0/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.2/tests/test_save_load_functions.py` & `simcardems-2023.5.0/tests/test_save_load_functions.py`

 * *Files identical despite different names*

