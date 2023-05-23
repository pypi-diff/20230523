# Comparing `tmp/NREL-rex-0.2.81.tar.gz` & `tmp/NREL-rex-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NREL-rex-0.2.81.tar", last modified: Tue May 23 17:35:49 2023, max compression
+gzip compressed data, was "dist/NREL-rex-0.2.9.tar", last modified: Fri Aug 14 21:16:10 2020, max compression
```

## Comparing `NREL-rex-0.2.81.tar` & `NREL-rex-0.2.9.tar`

### file list

```diff
@@ -1,62 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:35:49.636529 NREL-rex-0.2.81/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:35:49.624529 NREL-rex-0.2.81/NREL_rex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-05-23 17:35:49.000000 NREL-rex-0.2.81/NREL_rex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-23 17:35:49.000000 NREL-rex-0.2.81/NREL_rex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:35:49.000000 NREL-rex-0.2.81/NREL_rex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-23 17:35:49.000000 NREL-rex-0.2.81/NREL_rex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:35:49.000000 NREL-rex-0.2.81/NREL_rex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-23 17:35:49.000000 NREL-rex-0.2.81/NREL_rex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-23 17:35:49.000000 NREL-rex-0.2.81/NREL_rex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-05-23 17:35:49.636529 NREL-rex-0.2.81/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:35:49.628529 NREL-rex-0.2.81/rex/
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:35:49.628529 NREL-rex-0.2.81/rex/joint_pd/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/joint_pd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/joint_pd/joint_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/joint_pd/wind_rose_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21161 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/multi_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    13459 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/multi_res_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    29037 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/multi_time_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/multi_year_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    35431 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:35:49.628529 NREL-rex-0.2.81/rex/rechunk_h5/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/rechunk_h5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/rechunk_h5/chunk_size.py
--rw-r--r--   0 runner    (1001) docker     (123)    15969 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/rechunk_h5/combine_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/rechunk_h5/combine_h5_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/rechunk_h5/rechunk_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    29800 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/rechunk_h5/rechunk_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)    59425 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/renewable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    51837 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:35:49.632529 NREL-rex-0.2.81/rex/resource_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/resource_extraction/US_wave_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/resource_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/resource_extraction/multi_year_resource_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/resource_extraction/nsrdb_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/resource_extraction/resource_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    64401 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/resource_extraction/resource_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/resource_extraction/wave_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/resource_extraction/wind_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    37820 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/sam_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:35:49.632529 NREL-rex-0.2.81/rex/temporal_stats/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/temporal_stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44547 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/temporal_stats/temporal_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/temporal_stats/temporal_stats_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:35:49.636529 NREL-rex-0.2.81/rex/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/utilities/cli_dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/utilities/downscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18013 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/utilities/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/utilities/fun_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26590 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/utilities/hpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17983 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/utilities/loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/utilities/parse_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/utilities/solar_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/utilities/toml_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    27271 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/utilities/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/rex/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 17:35:49.636529 NREL-rex-0.2.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-23 17:35:34.000000 NREL-rex-0.2.81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-14 21:16:10.575921 NREL-rex-0.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-14 21:16:10.571921 NREL-rex-0.2.9/NREL_rex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     5190 2020-08-14 21:16:10.000000 NREL-rex-0.2.9/NREL_rex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1010 2020-08-14 21:16:10.000000 NREL-rex-0.2.9/NREL_rex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-14 21:16:10.000000 NREL-rex-0.2.9/NREL_rex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      315 2020-08-14 21:16:10.000000 NREL-rex-0.2.9/NREL_rex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-14 21:16:10.000000 NREL-rex-0.2.9/NREL_rex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      159 2020-08-14 21:16:10.000000 NREL-rex-0.2.9/NREL_rex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        4 2020-08-14 21:16:10.000000 NREL-rex-0.2.9/NREL_rex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     5190 2020-08-14 21:16:10.575921 NREL-rex-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     3631 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-14 21:16:10.575921 NREL-rex-0.2.9/rex/
+-rw-r--r--   0 runner    (1001) docker     (116)     1230 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    28774 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/multi_year_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-14 21:16:10.575921 NREL-rex-0.2.9/rex/rechunk_h5/
+-rw-r--r--   0 runner    (1001) docker     (116)      104 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/rechunk_h5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2455 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/rechunk_h5/rechunk_cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25248 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/rechunk_h5/rechunk_h5.py
+-rw-r--r--   0 runner    (1001) docker     (116)    43525 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/renewable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (116)    35981 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-14 21:16:10.575921 NREL-rex-0.2.9/rex/resource_extraction/
+-rw-r--r--   0 runner    (1001) docker     (116)      323 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/resource_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6430 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/resource_extraction/multi_year_resource_cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5745 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/resource_extraction/nsrdb_cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9434 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/resource_extraction/resource_cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)    32651 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/resource_extraction/resource_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5405 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/resource_extraction/wave_cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7337 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/resource_extraction/wind_cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)    26809 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/sam_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-14 21:16:10.575921 NREL-rex-0.2.9/rex/utilities/
+-rw-r--r--   0 runner    (1001) docker     (116)      358 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5491 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/utilities/cli_dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5316 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/utilities/downscale.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1416 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    36923 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/utilities/execution.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8673 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/utilities/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (116)      931 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/utilities/parse_keys.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11859 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/utilities/solar_position.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2070 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/utilities/toml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11766 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/utilities/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (116)       48 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/rex/version.py
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-08-14 21:16:10.575921 NREL-rex-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     2532 2020-08-14 21:15:57.000000 NREL-rex-0.2.9/setup.py
```

### Comparing `NREL-rex-0.2.81/README.rst` & `NREL-rex-0.2.9/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-**********************************************
-Welcome to The REsource eXtraction (rex) tool!
-**********************************************
+***
+rex
+***
 
 .. image:: https://github.com/NREL/rex/workflows/Documentation/badge.svg
     :target: https://nrel.github.io/rex/
 
 .. image:: https://github.com/NREL/rex/workflows/Pytests/badge.svg
     :target: https://github.com/NREL/rex/actions?query=workflow%3A%22Pytests%22
 
@@ -19,58 +19,56 @@
 
 .. image:: https://anaconda.org/nrel/nrel-rex/badges/version.svg
     :target: https://anaconda.org/nrel/nrel-rex
 
 .. image:: https://anaconda.org/nrel/nrel-rex/badges/license.svg
     :target: https://anaconda.org/nrel/nrel-rex
 
-.. image:: https://codecov.io/gh/nrel/rex/branch/main/graph/badge.svg?token=WQ95L11SRS
-    :target: https://codecov.io/gh/nrel/rex
-
-.. image:: https://zenodo.org/badge/253541811.svg
-   :target: https://zenodo.org/badge/latestdoi/253541811
+The REsource eXtraction (rex) tool
 
 .. inclusion-intro
 
 rex command line tools
 ======================
 
-- `rex <https://nrel.github.io/rex/_cli/rex.html#rex>`_
-- `NSRDBX <https://nrel.github.io/rex/_cli/NSRDBX.html#NSRDBX>`_
-- `WINDX <https://nrel.github.io/rex/_cli/WINDX.html#WINDX>`_
-- `US-wave <https://nrel.github.io/rex/_cli/US-wave.html#US-wave>`_
-- `WaveX <https://nrel.github.io/rex/_cli/WaveX.html#Wavex>`_
-- `MultiYearX <https://nrel.github.io/rex/_cli/MultiYearX.html#MultiYearX>`_
-- `rechunk <https://nrel.github.io/rex/_cli/rechunk.html#rechunk>`_
-- `temporal-stats <https://nrel.github.io/rex/_cli/temporal-stats.html#temporal-stats>`_
-- `wind-rose <https://nrel.github.io/rex/_cli/wind-rose.html#wind-rose>`_
+- `rex <https://nrel.github.io/rex/rex/rex.resource_extraction.resource_cli.html#rex>`_
+- `NSRDBX <https://nrel.github.io/rex/rex/rex.resource_extraction.nsrdb_cli.html#nsrdbx>`_
+- `WINDX <https://nrel.github.io/rex/rex/rex.resource_extraction.wind_cli.html#windx>`_
+- `WaveX <https://nrel.github.io/rex/rex/rex.resource_extraction.wave_cli.html#wavex>`_
+- `MultiYearX <https://nrel.github.io/rex/rex/rex.resource_extraction.multi_year_resource_cli.html#multiyearx>`_
+- `rechunk <https://nrel.github.io/rex/rex/rex.rechunk_h5.rechunk_cli.html#rechunk>`_
 
-Using Eagle Env
-===============
+Using Eagle Env / Module
+========================
 
 If you would like to run `rex` on Eagle (NREL's HPC) you can use a pre-compiled
 conda env:
 
 .. code-block:: bash
 
-    conda activate /shared-projects/rev/modulefiles/conda/envs/rev/
+    conda activate /datasets/modulefiles/conda_env
 
 or
 
 .. code-block:: bash
 
-    source activate /shared-projects/rev/modulefiles/conda/envs/rev/
+    source activate /datasets/modulefiles/conda_env
+
+or module:
+
+.. code-block:: bash
+
+    module use /datasets/modulefiles
+    module load rex
+
+**NOTE: Loading the rex module can take several minutes**
 
 Installing rex
 ==============
 
-NOTE: The installation instruction below assume that you have python installed
-on your machine and are using `conda <https://docs.conda.io/en/latest/index.html>`_
-as your package/environment manager.
-
 Option 1: Install from PIP or Conda (recommended for analysts):
 ---------------------------------------------------------------
 
 1. Create a new environment:
     ``conda create --name rex``
 
 2. Activate directory:
@@ -82,36 +80,34 @@
 
        - NOTE: If you install using conda and want to use `HSDS <https://github.com/NREL/hsds-examples>`_
          you will also need to install h5pyd manually: ``pip install h5pyd``
 
 Option 2: Clone repo (recommended for developers)
 -------------------------------------------------
 
-1. from home dir, ``git clone git@github.com:NREL/rex.git``
-
-2. Create ``rex`` environment and install package
-    1) Create a conda env: ``conda create -n rex``
-    2) Run the command: ``conda activate rex``
-    3) cd into the repo cloned in 1.
-    4) prior to running ``pip`` below, make sure the branch is correct (install
-       from main!)
-    5) Install ``rex`` and its dependencies by running:
-       ``pip install .`` (or ``pip install -e .`` if running a dev branch
+1. from home dir, ``git clone https://github.com/NREL/rex.git``
+    1) enter github username
+    2) enter github password
+
+2. Install reV environment and modules (using conda)
+    1) cd into reV repo cloned above
+    2) cd into ``bin/$OS/``
+    3) run the command: ``conda env create -f rex.yml``. If conda can't find
+       any packages, try removing them from the yml file.
+
+    4) run the command: ``conda activate rex``
+    5) prior to running ``pip`` below, make sure the branch is correct (install
+       from master!)
+
+    6) cd back to the rex repo (where setup.py is located)
+    7) install pre-commit: ``pre-commit install``
+    8) run ``pip install .`` (or ``pip install -e .`` if running a dev branch
        or working on the source code)
 
-3. Check that ``rex`` was installed successfully
+3. Check that rev was installed successfully
     1) From any directory, run the following commands. This should return the
        help pages for the CLI's.
 
         - ``rex``
-        - ``NSRDBX``
-        - ``WINDX``
-        - ``US-wave``
-
-Recommended Citation
-====================
-
-Update with current version and DOI:
-
-Michael Rossol, Grant Buster. The REsource Extraction Tool (rex).
-https://github.com/NREL/rex (version v0.2.43), 2021.
-https://doi.org/10.5281/zenodo.4499033.
+        - ``NSRDB``
+        - ``WIND``
+        - ``rechunk``
```

### Comparing `NREL-rex-0.2.81/rex/multi_time_resource.py` & `NREL-rex-0.2.9/rex/multi_year_resource.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,435 +1,356 @@
 # -*- coding: utf-8 -*-
 """
-Classes to handle resource data stored over multiple files
+Classes to handle multiple years of resource data
 """
-import pandas as pd
-from glob import glob
-from fnmatch import fnmatch
 import numpy as np
 import os
+from warnings import warn
 
-from rex.resource import Resource
 from rex.renewable_resource import (NSRDB, SolarResource, WindResource,
                                     WaveResource)
+from rex.resource import MultiH5, Resource
+from rex.utilities.exceptions import ResourceKeyError, ResourceWarning
 from rex.utilities.parse_keys import parse_keys, parse_slice
-from rex.utilities.exceptions import FileInputError
+from rex.utilities.utilities import parse_year
 
 
-class MultiTimeH5:
+class MultiYearH5:
     """
-    Class to handle h5 Resources stored over multiple temporal files
+    Class to handle multiple years of h5 Resources
     """
 
-    def __init__(self, h5_path, res_cls=Resource, hsds=False, hsds_kwargs=None,
-                 **res_cls_kwargs):
+    def __init__(self, h5_dir, prefix='', suffix='.h5', res_cls=Resource,
+                 hsds=False, **res_cls_kwargs):
         """
         Parameters
         ----------
-        h5_path : str | list
-            Unix shell style pattern path with * wildcards to multi-file
-            resource file sets. Files must have the same coordinates
-            but can have different datasets or time indexes. Can also be an
-            explicit list of multi time files.
+        h5_dir : str
+            Path to directory containing 5min .h5 files
+        prefix : str
+            Prefix for resource .h5 files
+        suffix : str
+            Suffix for resource .h5 files
         res_cls : obj
             Resource class to use to open and access resource data
         hsds : bool
             Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
             behind HSDS
-        hsds_kwargs : dict, optional
-            Dictionary of optional kwargs for h5pyd, e.g., bucket, username,
-            password, by default None
-        res_cls_kwargs : dict, optional
-            Kwargs for `res_cls`
-        """
-        self.h5_path = h5_path
-        self._file_paths = self._get_file_paths(h5_path, hsds=hsds,
-                                                hsds_kwargs=hsds_kwargs)
+        """
+        self.h5_dir = h5_dir
+        self._year_map = self._map_file_years(h5_dir, prefix=prefix,
+                                              suffix=suffix, hsds=hsds)
         res_cls_kwargs.update({'hsds': hsds})
-        self._h5_map = self._map_file_instances(self._file_paths,
+        self._h5_map = self._map_file_instances(set(self._year_map.values()),
                                                 res_cls=res_cls,
                                                 **res_cls_kwargs)
-
         self._datasets = None
         self._shape = None
         self._time_index = None
-        self._time_slice_map = []
         self._i = 0
 
     def __repr__(self):
-        msg = ("{} for {}:\n Contains data from {} files"
-               .format(self.__class__.__name__, self.h5_path, len(self)))
+        msg = ("{} for {}:\n Contains data for {} year"
+               .format(self.__class__.__name__, self.h5_dir, len(self)))
         return msg
 
-    def __getitem__(self, file):
-        fn_fp_map = {os.path.basename(fp): fp for fp in self._file_paths}
-        if file in self._h5_map['fp']:
-            iloc = np.where(self._h5_map['fp'] == file)[0][0]
-            h5 = self._h5_map.at[iloc, 'h5']
-        elif file in fn_fp_map:
-            iloc = np.where(self._h5_map['fp'] == fn_fp_map[file])[0][0]
-            h5 = self._h5_map.at[iloc, 'h5']
+    def __len__(self):
+        return len(self.years)
+
+    def __getitem__(self, year):
+        if isinstance(year, str):
+            year = int(year)
+
+        if year in self.years:
+            path = self._year_map[year]
+            h5 = self._h5_map[path]
         else:
             raise ValueError('{} is invalid, must be one of: {}'
-                             .format(file, self._file_paths))
+                             .format(year, self.years))
 
         return h5
 
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        if self._i >= len(self.years):
+            self._i = 0
+            raise StopIteration
+
+        year = self.years[self._i]
+        self._i += 1
+
+        return year
+
+    def __contains__(self, year):
+
+        return year in self.years
+
     @property
     def attrs(self):
         """
         Global .h5 file attributes sourced from first .h5 file
 
         Returns
         -------
         attrs : dict
+            .h5 file attributes sourced from first .h5 file
         """
         attrs = dict(self.h5.attrs)
-
         return attrs
 
     @property
-    def files(self):
+    def years(self):
         """
-        Available file paths
+        Available years
 
         Returns
         -------
         list
+            List of dataset present in .h5 files
         """
-        return sorted(self._file_paths)
+        return sorted(self._year_map)
 
     @property
     def h5_files(self):
         """
         .h5 files data is being sourced from
 
         Returns
         -------
         list
+            List of .h5 files data is being sourced form
         """
-        return sorted(self._h5_map['fp'])
+        return sorted(self._h5_map)
 
     @property
     def h5(self):
         """
         open h5 file handler for a single .h5 file
 
         Returns
         -------
-        h5py.File
+        [type]
+            [description]
         """
-        return self._h5_map['h5'].values[0]
+        return self._h5_map[self.h5_files[0]]
 
     @property
     def datasets(self):
         """
         Available datasets
 
         Returns
         -------
         list
+            List of available datasets
         """
         if self._datasets is None:
-            all_dsets = self._h5_map['dsets'].values.tolist()
-            dsets = [d for sub in all_dsets for d in sub]
-            self._datasets = list(set(dsets))
+            self._datasets = self.h5.datasets
 
         return self._datasets
 
     @property
-    def resource_datasets(self):
-        """
-        Available resource datasets
-
-        Returns
-        -------
-        list
-        """
-        res_dsets = [ds for ds in self.datasets
-                     if ds not in ['meta', 'time_index', 'coordinates']]
-
-        return res_dsets
-
-    @property
     def shape(self):
         """
         Dataset shape (time, sites)
 
         Returns
         -------
         tuple
         """
         if self._shape is None:
-            self._shape = (len(self.time_index), self.h5.shape[1])
+            self._shape = (len(self.time_index), len(self.h5))
 
         return self._shape
 
     @property
     def time_index(self):
         """
         Multi-year datetime index
 
         Returns
         -------
         pandas.DatatimeIndex
         """
         if self._time_index is None:
-            time_slice_map = []
-            for _, row in self._h5_map.iterrows():
-                h5 = row['h5']
-                fp = row['fp']
-                ti = h5.time_index
-                time_slice_map.append(np.full(len(ti), os.path.basename(fp)))
+            for year in self.years:
+                path = self._year_map[year]
+                h5 = self._h5_map[path]
                 if self._time_index is None:
-                    self._time_index = ti
+                    self._time_index = h5.time_index
                 else:
-                    self._time_index = self._time_index.append(ti)
-
-            if len(self._time_index) != len(np.unique(self._time_index)):
-                unique, duplicates = np.unique(self._time_index,
-                                               return_counts=True)
-                duplicates = np.where(duplicates > 1)[0]
-                duplicates = unique[duplicates]
-                msg = ('The combined time_index has {} duplicate values:\n{}'
-                       .format(len(duplicates), duplicates))
-                raise RuntimeError(msg)
-
-            self._time_slice_map = np.concatenate(time_slice_map, axis=0)
+                    self._time_index = self._time_index.append(h5.time_index)
 
         return self._time_index
 
     @staticmethod
-    def _get_hsds_file_paths(h5_path, hsds_kwargs=None):
+    def _map_local_files(h5_dir, prefix='', suffix='.h5'):
         """
-        Get a list of h5 filepaths matching the h5_path specification from HSDS
+        Map local file paths to year for which it contains data
 
         Parameters
         ----------
-        h5_path : str
-            Unix shell style pattern path with * wildcards to multi-file
-            resource file sets. Files must have the same coordinates
-            but can have different datasets or time indexes.
-        hsds_kwargs : dict, optional
-            Dictionary of optional kwargs for h5pyd, e.g., bucket, username,
-            password, by default None
+        h5_dir : str
+            Path to directory containing Resource .h5 files
+        prefix : str
+            Prefix for resource .h5 files
+        suffix : str
+            Suffix for resource .h5 files
 
         Returns
         -------
-        file_paths : list
-            List of filepaths for this handler to handle.
-        """
-        import h5pyd
-
-        if hsds_kwargs is None:
-            hsds_kwargs = {}
-
-        hsds_dir = os.path.dirname(h5_path)
-        fn = os.path.basename(h5_path)
-
-        if '*' in hsds_dir:
-            msg = ('HSDS path specifications cannot handle wildcards in the '
-                   'directory name! The directory must be explicit but the '
-                   'filename can have wildcards. This HSDS h5_path input '
-                   'cannot be used: {}'.format(h5_path))
-            raise FileNotFoundError(msg)
-
-        if not fn:
-            msg = ('h5_path must be a unix shell style pattern with '
-                   'wildcard * in order to find files, but received '
-                   'directory specification: {}'.format(h5_path))
-            raise FileInputError(msg)
+        year_map : dict
+            Dictionary mapping years to file paths
+        """
+        year_map = {}
+        for file in sorted(os.listdir(h5_dir)):
+            if file.startswith(prefix) and file.endswith(suffix):
+                try:
+                    year = parse_year(file)
+                    path = os.path.join(h5_dir, file)
+                    if year not in year_map:
+                        year_map[year] = path
+                    else:
+                        msg = ('WARNING: Skipping {} as {} has already been '
+                               'parsed'.format(path, year))
+                        warn(msg, ResourceWarning)
+                except RuntimeError:
+                    msg = ('WARNING: Could not find a valid year in {}'
+                           .format(file))
+                    warn(msg, ResourceWarning)
 
-        with h5pyd.Folder(hsds_dir + '/', **hsds_kwargs) as f:
-            file_paths = [f'{hsds_dir}/{fn}' for fn in f
-                          if fnmatch(f'{hsds_dir}/{fn}', h5_path)]
+        return year_map
 
-        return file_paths
-
-    @classmethod
-    def _get_file_paths(cls, h5_path, hsds=False, hsds_kwargs=None):
+    @staticmethod
+    def _map_hsds_files(hsds_dir, prefix='', suffix='.h5'):
         """
-        Get a file list based on the h5_path specification.
+        Map hsds file paths to year for which it contains data
 
         Parameters
         ----------
-        h5_path : str | list
-            Unix shell style pattern path with * wildcards to multi-file
-            resource file sets. Files must have the same coordinates
-            but can have different datasets or time indexes. Can also be an
-            explicit list of multi time files.
-        hsds : bool
-            Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
-            behind HSDS
-        hsds_kwargs : dict, optional
-            Dictionary of optional kwargs for h5pyd, e.g., bucket, username,
-            password, by default None
+        hsds_dir : str
+            HSDS directory containing Resource .h5 files
+        prefix : str
+            Prefix for resource .h5 files
+        suffix : str
+            Suffix for resource .h5 files
 
         Returns
         -------
-        file_paths : list
-            List of filepaths for this handler to handle.
+        year_map : dict
+            Dictionary mapping years to file paths
         """
+        import h5pyd
 
-        if hsds:
-            file_paths = cls._get_hsds_file_paths(h5_path,
-                                                  hsds_kwargs=hsds_kwargs)
-        elif isinstance(h5_path, (list, tuple)):
-            for fp in h5_path:
-                msg = 'Does not exist: {}'.format(fp)
-                assert os.path.exists(fp), msg
-            file_paths = h5_path
-        elif os.path.isdir(h5_path):
-            msg = ('h5_path must be a unix shell style pattern with '
-                   'wildcard * in order to find files, but received '
-                   'directory specification: {}'.format(h5_path))
-            raise FileInputError(msg)
-        elif isinstance(h5_path, str):
-            file_paths = glob(h5_path)
-
-        if not any(file_paths):
-            msg = ('Could not find any file paths with pattern: {}'
-                   .format(h5_path))
-            raise FileInputError(msg)
+        year_map = {}
+        with h5pyd.Folder(hsds_dir + '/') as f:
+            for file in f:
+                if file.startswith(prefix) and file.endswith(suffix):
+                    try:
+                        year = parse_year(file)
+                        path = os.path.join(hsds_dir, file)
+                        if year not in year_map:
+                            year_map[year] = path
+                        else:
+                            msg = ('WARNING: Skipping {} as {} has already '
+                                   ' been parsed'.format(path, year))
+                            warn(msg, ResourceWarning)
+                    except RuntimeError:
+                        msg = ('WARNING: Could not find a valid year in {}'
+                               .format(file))
+                        warn(msg, ResourceWarning)
 
-        return file_paths
+        return year_map
 
     @staticmethod
-    def _map_file_instances(file_paths, res_cls=Resource, **res_cls_kwargs):
+    def _map_file_years(h5_dir, prefix='', suffix='.h5', hsds=False):
         """
-        Open all .h5 files and map the open h5py instances to the
-        associated file paths
+        Map file paths to year for which it contains data
 
         Parameters
         ----------
-        file_paths : list
-            List of filepaths for this handler to handle.
+        h5_dir : str
+            Path to directory containing Resource .h5 files
+        prefix : str
+            Prefix for resource .h5 files
+        suffix : str
+            Suffix for resource .h5 files
 
         Returns
         -------
-        h5_map : pd.DataFrame
-            DataFrame mapping file paths to open resource instances and
-            datasets per file (columns: fp, h5, and dsets)
+        year_map : dict
+            Dictionary mapping years to file paths
         """
-        h5_map = pd.DataFrame({'fp': file_paths, 'h5': None,
-                               't0': None, 't1': None})
-        for i, f_path in enumerate(file_paths):
-            h5_map.at[i, 'h5'] = res_cls(f_path, **res_cls_kwargs)
-            h5_map.at[i, 't0'] = h5_map.at[i, 'h5'].time_index.values[0]
-            h5_map.at[i, 't1'] = h5_map.at[i, 'h5'].time_index.values[1]
+        if hsds:
+            year_map = MultiYearH5._map_hsds_files(h5_dir, prefix=prefix,
+                                                   suffix=suffix)
+        else:
+            year_map = MultiYearH5._map_local_files(h5_dir, prefix=prefix,
+                                                    suffix=suffix)
 
-        h5_map['dsets'] = [h5.dsets for h5 in h5_map['h5'].values]
-        h5_map = h5_map.sort_values('t0').reset_index(drop=True)
-
-        return h5_map
+        return year_map
 
     @staticmethod
-    def _check_time_slice(time_slice):
+    def _map_file_instances(h5_files, res_cls=Resource, **res_cls_kwargs):
         """
-        Check to see if time positions can be represented as a slice
-
+        Open all .h5 files and map the open h5py instances to the
+        associated file paths
         Parameters
         ----------
-        time_slice : ndarray | list
-            List of temporal positions
-
+        h5_files : list
+            List of .h5 files to open
         Returns
         -------
-        time_slice : ndarray | list | slice
-            Slice covering range of positions to extract if possible
+        h5_map : dict
+            Dictionary mapping file paths to open resource instances
         """
-        s = time_slice[0]
-        e = time_slice[-1] + 1
-        if (e - s) == len(time_slice):
-            time_slice = slice(s, e, None)
+        h5_map = {}
+        for f_path in h5_files:
+            h5_map[f_path] = res_cls(f_path, **res_cls_kwargs)
 
-        return time_slice
+        return h5_map
 
-    def _map_time_slice(self, time_slice):
+    def year_index(self, year):
         """
-        Map timeslices to files
+        Extract time_index for a specific year
 
         Parameters
         ----------
-        time_slice : int | list | slice
-            tuple describing slice of dataset array to extract
+        year : int
+            Year to extract time_index for
 
         Returns
         -------
-        file_times : dict
-            Dictionary mapping files to the time_slices to extract
-        """
-        time_index = self.time_index[time_slice]
-        files = self._time_slice_map[time_slice]
-        file_times = {}
-        for file in np.unique(files):
-            ti = self[file].time_index
-            file_slice = np.where(ti.isin(time_index))[0]
-            file_slice = self._check_time_slice(file_slice)
-            file_times[file] = file_slice
-
-        return file_times
-
-    def _get_ds(self, ds_name, ds_slice):
+        time_index : pandas.DatetimeIndex
+            Resource datetime index for desired year
         """
-        Extract data from given dataset
-
-        Parameters
-        ----------
-        ds_name : str
-            Variable dataset to be extracted
-        ds_slice : int | list | slice
-            tuple describing slice of dataset array to extract
-
-        Returns
-        -------
-        out : ndarray
-            ndarray of variable timeseries data
-            If unscale, returned in native units else in scaled units
-        """
-        ds_slice = parse_slice(ds_slice)
-        out = []
-        time_slice = ds_slice[0]
-        if isinstance(time_slice, (int, np.integer)):
-            time_step = self.time_index[time_slice]
-            file = self._time_slice_map[time_slice]
-            time_index = self[file].time_index
-            time_slice = np.where(time_step == time_index)[0][0]
-            file_slice = (time_slice, ) + ds_slice[1:]
-            out = self[file]._get_ds(ds_name, file_slice)
-        else:
-            file_times = self._map_time_slice(ds_slice[0])
-            for file, time_slice in file_times.items():
-                file_slice = (time_slice, ) + ds_slice[1:]
-                out.append(self[file]._get_ds(ds_name, file_slice))
-
-            out = np.concatenate(out, axis=0)
-
-        return out
+        return self.time_index[self.time_index.year == year]
 
     def close(self):
         """
         Close all h5py.File instances
         """
-        for f in self._h5_map['h5']:
+        for f in self._h5_map.values():
             f.close()
 
 
-class MultiTimeResource:
+class MultiYearResource:
     """
-    Class to handle resource data stored temporally accross multiple
+    Class to handle multiple years of resource data stored accross multiple
     .h5 files
 
     Examples
     --------
 
     Extracting the resource's Datetime Index
 
     >>> path = '$TESTDATADIR/nsrdb/ri_100_nsrdb_*.h5'
-    >>> with MultiTimeResource(path) as res:
+    >>> with MultiYearResource(path) as res:
     >>>     ti = res.time_index
     >>>
     >>> ti
     DatetimeIndex(['2012-01-01 00:00:00', '2012-01-01 00:30:00',
                    '2012-01-01 01:00:00', '2012-01-01 01:30:00',
                    '2012-01-01 02:00:00', '2012-01-01 02:30:00',
                    '2012-01-01 03:00:00', '2012-01-01 03:30:00',
@@ -440,322 +361,273 @@
                    '2013-12-31 21:00:00', '2013-12-31 21:30:00',
                    '2013-12-31 22:00:00', '2013-12-31 22:30:00',
                    '2013-12-31 23:00:00', '2013-12-31 23:30:00'],
                   dtype='datetime64[ns]', length=35088, freq=None)
 
     NOTE: time_index covers data from 2012 and 2013
 
-    >>> with MultiTimeResource(path) as res:
+    >>> with MultiYearResource(path) as res:
     >>>     print(res.h5_files)
 
     ['/Users/mrossol/Git_Repos/rex/tests/data/nsrdb/ri_100_nsrdb_2012.h5',
      '/Users/mrossol/Git_Repos/rex/tests/data/nsrdb/ri_100_nsrdb_2013.h5']
 
     Data slicing works the same as with "Resource" except axis 0 now covers
     2012 and 2013
 
-    >>> with MultiTimeResource(path) as res:
+    >>> with MultiYearResource(path) as res:
     >>>     temperature = res['air_temperature']
     >>>
     >>> temperature
     [[ 4.  5.  5. ...  4.  3.  4.]
      [ 4.  4.  5. ...  4.  3.  4.]
      [ 4.  4.  5. ...  4.  3.  4.]
      ...
      [-1. -1.  0. ... -2. -3. -2.]
      [-1. -1.  0. ... -2. -3. -2.]
      [-1. -1.  0. ... -2. -3. -2.]]
     >>> temperature.shape
     (35088, 100)
 
-    >>> with MultiTimeResource(path) as res:
+    >>> with MultiYearResource(path) as res:
     >>>     temperature = res['air_temperature', ::100] # every 100th timestep
     >>>
     >>> temperature
     [[ 4.  5.  5. ...  4.  3.  4.]
      [ 1.  1.  2. ...  0.  0.  1.]
      [-2. -1. -1. ... -2. -4. -2.]
      ...
      [-3. -2. -2. ... -3. -4. -3.]
      [ 0.  0.  1. ...  0. -1.  0.]
      [ 3.  3.  3. ...  2.  2.  3.]]
     >>> temperature.shape
     (351, 100)
+
+    You can also request a specific year of data using a string representation
+    of the year of interest
+    NOTE: you can also request a list of years using strings
+
+    >>> with MultiYearResource(path) as res:
+    >>>     temperature = res['air_temperature', '2012'] # every 100th timestep
+    >>>
+    >>> temperature
+    [[4. 5. 5. ... 4. 3. 4.]
+     [4. 4. 5. ... 4. 3. 4.]
+     [4. 4. 5. ... 4. 3. 4.]
+     ...
+     [1. 1. 2. ... 0. 0. 0.]
+     [1. 1. 2. ... 0. 0. 1.]
+     [1. 1. 2. ... 0. 0. 1.]]
+    >>> temperature.shape
+    (17520, 100)
     """
+    PREFIX = ''
+    SUFFIX = '.h5'
 
-    def __init__(self, h5_path, unscale=True, str_decode=True,
-                 res_cls=Resource, hsds=False, hsds_kwargs=None):
+    def __init__(self, h5_path, unscale=True, str_decode=True, hsds=False,
+                 res_cls=Resource):
         """
         Parameters
         ----------
-        h5_path : str | list
-            Unix shell style pattern path with * wildcards to multi-file
-            resource file sets. Files must have the same coordinates
-            but can have different datasets or time indexes. Can also be an
-            explicit list of multi time files.
+        h5_path : str
+            Path to directory containing multi-file resource file sets.
+            Available formats:
+                /h5_dir/
+                /h5_dir/prefix*suffix
         unscale : bool
             Boolean flag to automatically unscale variables on extraction
         str_decode : bool
             Boolean flag to decode the bytestring meta data into normal
             strings. Setting this to False will speed up the meta data read.
+        hsds : bool
+            Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
+            behind HSDS
         res_cls : obj
             Resource handler to us to open individual .h5 files
-        hsds : bool, optional
-            Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
-            behind HSDS, by default False
-        hsds_kwargs : dict, optional
-            Dictionary of optional kwargs for h5pyd, e.g., bucket, username,
-            password, by default None
         """
+        self.h5_dir, prefix, suffix = MultiH5.multi_file_args(h5_path)
+        if prefix is None:
+            prefix = self.PREFIX
+
+        if suffix is None:
+            suffix = self.SUFFIX
 
-        self.h5_path = h5_path
+        self._meta = None
         self._time_index = None
+        self._coords = None
         # Map variables to their .h5 files
         cls_kwargs = {'unscale': unscale, 'str_decode': str_decode,
-                      'hsds': hsds, 'hsds_kwargs': hsds_kwargs}
-        self._h5 = MultiTimeH5(self.h5_path, res_cls=res_cls, **cls_kwargs)
+                      'hsds': hsds}
+        self._h5 = MultiYearH5(self.h5_dir, prefix=prefix, suffix=suffix,
+                               res_cls=res_cls, **cls_kwargs)
         self.h5_files = self._h5.h5_files
         self.h5_file = self.h5_files[0]
         self._i = 0
 
     def __repr__(self):
-        msg = "{} for {}".format(self.__class__.__name__, self.h5_path)
+        msg = "{} for {}".format(self.__class__.__name__, self.h5_dir)
         return msg
 
     def __enter__(self):
         return self
 
     def __exit__(self, type, value, traceback):
         self.close()
 
         if type is not None:
             raise
 
     def __len__(self):
-        return len(self.h5.time_index)
+        return self.h5.shape[0]
+
+    def __getitem__(self, keys):
+        ds, ds_slice = parse_keys(keys)
+
+        if ds.endswith('time_index'):
+            out = self._get_time_index(ds_slice)
+        elif ds.endswith('meta'):
+            out = self._get_meta(ds, ds_slice)
+        elif ds.endswith('coordinates'):
+            out = self._get_coords(ds, ds_slice)
+        else:
+            out = self._get_ds(ds, ds_slice)
+
+        return out
 
     def __iter__(self):
         return self
 
     def __next__(self):
         if self._i >= len(self.datasets):
             self._i = 0
             raise StopIteration
 
         dset = self.datasets[self._i]
         self._i += 1
 
         return dset
 
-    def __getitem__(self, keys):
-        ds, ds_slice = parse_keys(keys)
-
-        if ds.endswith('time_index'):
-            out = self.h5.h5._get_time_index(ds_slice)
-        elif ds.endswith('meta'):
-            out = self.h5.h5._get_meta(ds, ds_slice)
-        elif ds.endswith('coordinates'):
-            out = self.h5.h5._get_coords(ds, ds_slice)
-        else:
-            out = self.h5._get_ds(ds, ds_slice)
-
-        return out
-
     def __contains__(self, dset):
         return dset in self.datasets
 
     @property
     def h5(self):
         """
-        Open class instance that handles all .h5 files that data is to
-        be extracted from
+        Open h5py File instance. If _group is not None return open Group
 
         Returns
         -------
-        h5 : MultiTimeH5 | MultiYearH5
+        h5 : h5py.File | h5py.Group
+            Open h5py File or Group instance
         """
-        return self._h5
+        h5 = self._h5
+
+        return h5
 
     @property
     def datasets(self):
         """
         Datasets available
 
         Returns
         -------
         list
+            List of datasets
         """
-        return self.h5.datasets
+        return self._h5.datasets
 
     @property
     def dsets(self):
         """
         Datasets available
 
         Returns
         -------
         list
+            List of datasets
         """
         return self.datasets
 
     @property
-    def resource_datasets(self):
-        """
-        Available resource datasets
-
-        Returns
-        -------
-        list
-        """
-        return self.h5.resource_datasets
-
-    @property
-    def res_dsets(self):
-        """
-        Available resource datasets
-
-        Returns
-        -------
-        list
-        """
-        return self.resource_datasets
-
-    @property
     def shape(self):
         """
         Resource shape (timesteps, sites)
         shape = (len(time_index), len(meta))
 
         Returns
         -------
         shape : tuple
+            Shape of resource variable arrays (timesteps, sites)
         """
         return self.h5.shape
 
     @property
     def meta(self):
         """
-        Resource meta data DataFrame
+        Meta data DataFrame
 
         Returns
         -------
         meta : pandas.DataFrame
+            Resource Meta Data
         """
+        if self._meta is None:
+            if 'meta' in self:
+                self._meta = self._get_meta('meta', slice(None))
+            else:
+                raise ResourceKeyError("'meta' is not a valid dataset")
 
-        return self.h5.h5.meta
+        return self._meta
 
     @property
     def time_index(self):
         """
-        Resource DatetimeIndex
+        DatetimeIndex
 
         Returns
         -------
         time_index : pandas.DatetimeIndex
+            Resource datetime index
         """
-        return self.h5.time_index
-
-    @property
-    def lat_lon(self):
-        """
-        Extract (latitude, longitude) pairs
+        if self._time_index is None:
+            if 'time_index' in self:
+                self._time_index = self._get_time_index(slice(None))
+            else:
+                raise ResourceKeyError("'time_index' is not a valid dataset!")
 
-        Returns
-        -------
-        lat_lon : ndarray
-        """
-        return self.h5.h5.lat_lon
+        return self._time_index
 
     @property
     def coordinates(self):
         """
         Coordinates: (lat, lon) pairs
 
         Returns
         -------
-        lat_lon : ndarray
+        coords : ndarray
+            Array of (lat, lon) pairs for each site in meta
         """
-        return self.lat_lon
+        if self._coords is None:
+            if 'coordinates' in self:
+                self._coords = self._get_coords('coordinates', slice(None))
+            else:
+                raise ResourceKeyError("'coordinates' is not a valid dataset!")
+
+        return self._coords
 
     @property
     def global_attrs(self):
         """
         Global (file) attributes
 
         Returns
         -------
         global_attrs : dict
         """
-        return self.get_attrs()
-
-    @property
-    def attrs(self):
-        """
-        Dictionary of all dataset attributes
-
-        Returns
-        -------
-        attrs : dict
-        """
-        return self.h5.h5.attrs
-
-    @property
-    def shapes(self):
-        """
-        Dictionary of all dataset shapes
-
-        Returns
-        -------
-        shapes : dict
-        """
-        return self.h5.h5.shapes
-
-    @property
-    def dtypes(self):
-        """
-        Dictionary of all dataset dtypes
-
-        Returns
-        -------
-        dtypes : dict
-        """
-        return self.h5.h5.dtypes
-
-    @property
-    def chunks(self):
-        """
-        Dictionary of all dataset chunk sizes
-
-        Returns
-        -------
-        chunks : dict
-        """
-        return self.h5.h5.chunks
-
-    @property
-    def scale_factors(self):
-        """
-        Dictionary of all dataset scale factors
-
-        Returns
-        -------
-        scale_factors : dict
-        """
-        return self.h5.h5.scale_factors
-
-    @property
-    def units(self):
-        """
-        Dictionary of all dataset units
-
-        Returns
-        -------
-        units : dict
-        """
-        return self.h5.h5.units
+        return dict(self.h5.attrs)
 
     def get_attrs(self, dset=None):
         """
         Get h5 attributes either from file or dataset
 
         Parameters
         ----------
@@ -763,15 +635,20 @@
             Dataset to get attributes for, if None get file (global) attributes
 
         Returns
         -------
         attrs : dict
             Dataset or file attributes
         """
-        return self.h5.h5.get_attrs(dset=dset)
+        if dset is None:
+            attrs = dict(self.h5.attrs)
+        else:
+            attrs = dict(self.h5.h5[dset].attrs)
+
+        return attrs
 
     def get_dset_properties(self, dset):
         """
         Get dataset properties (shape, dtype, chunks)
 
         Parameters
         ----------
@@ -783,31 +660,36 @@
         shape : tuple
             Dataset array shape
         dtype : str
             Dataset array dtype
         chunks : tuple
             Dataset chunk size
         """
-        return self.h5.h5.get_dset_properties(dset)
+        ds = self.h5.h5[dset]
+        shape, dtype, chunks = ds.shape, ds.dtype, ds.chunks
+        if isinstance(chunks, dict):
+            chunks = tuple(chunks.get('dims', None))
+
+        return shape, dtype, chunks
 
-    def get_scale_factor(self, dset):
+    def get_scale(self, dset):
         """
         Get dataset scale factor
 
         Parameters
         ----------
         dset : str
             Dataset to get scale factor for
 
         Returns
         -------
         float
             Dataset scale factor, used to unscale int values to floats
         """
-        return self.h5.h5.get_scale_factor(dset)
+        return self.h5.h5[dset].attrs.get('scale_factor', 1)
 
     def get_units(self, dset):
         """
         Get dataset units
 
         Parameters
         ----------
@@ -815,15 +697,15 @@
             Dataset to get units for
 
         Returns
         -------
         str
             Dataset units, None if not defined
         """
-        return self.h5.h5.get_units(dset)
+        return self.h5.h5[dset].attrs.get('units', None)
 
     def get_meta_arr(self, rec_name, rows=slice(None)):
         """Get a meta array by name (faster than DataFrame extraction).
 
         Parameters
         ----------
         rec_name : str
@@ -836,146 +718,299 @@
         meta_arr : np.ndarray
             Extracted array from the meta data record name.
         """
         meta_arr = self.h5.h5.get_meta_arr(rec_name, rows=rows)
 
         return meta_arr
 
+    def _get_time_index(self, ds_slice):
+        """
+        Extract and convert time_index to pandas Datetime Index
+
+        Parameters
+        ----------
+        ds_name : str
+            Dataset to extract time_index from
+        ds_slice : int | list | slice
+            tuple describing slice of time_index to extract
+
+        Returns
+        -------
+        time_index : pandas.DatetimeIndex
+            Vector of datetime stamps
+        """
+        ds_slice = parse_slice(ds_slice)
+        time_index = self.h5.time_index[ds_slice[0]]
+
+        return time_index
+
+    def _get_meta(self, ds_name, ds_slice):
+        """
+        Extract and convert meta to a pandas DataFrame
+
+        Parameters
+        ----------
+        ds_name : str
+            Dataset to extract meta from
+        ds_slice : int | list | slice
+            Pandas slicing describing which sites and columns to extract
+
+        Returns
+        -------
+        meta : pandas.Dataframe
+            Dataframe of location meta data
+        """
+        meta = self.h5.h5._get_meta(ds_name, ds_slice)
+
+        return meta
+
+    def _get_coords(self, ds_name, ds_slice):
+        """
+        Extract coordinates (lat, lon) pairs
+
+        Parameters
+        ----------
+        ds_name : str
+            Dataset to extract coordinates from
+        ds_slice : int | list | slice
+            tuple describing slice of coordinates to extract
+
+        Returns
+        -------
+        coords : ndarray
+            Array of (lat, lon) pairs for each site in meta
+        """
+        coords = self.h5.h5._get_coords(ds_name, ds_slice)
+
+        return coords
+
+    def _get_year_ds(self, ds_name, year, year_slice):
+        """
+        Extract dataset data for given year
+
+        Parameters
+        ----------
+        ds_name : str
+            Variable dataset to be extracted
+        year : int
+            Year to extract data for
+        year_slice : int | list | slice
+            tuple describing slice of dataset array to extract
+
+        Returns
+        -------
+        out : ndarray
+            ndarray of variable timeseries data
+            If unscale, returned in native units else in scaled units
+        """
+        out = self.h5[year]._get_ds(ds_name, year_slice)
+
+        return out
+
+    @staticmethod
+    def _check_year_slice(year_slice):
+        """
+        Check to see if year positions can be represented as a slice
+
+        Parameters
+        ----------
+        year_slice : ndarray | list
+            List of temporal positions
+
+        Returns
+        -------
+        year_slice : ndarray | list | slice
+            Slice covering range of positions to extract if possible
+        """
+        s = year_slice[0]
+        e = year_slice[-1] + 1
+        if (e - s) == len(year_slice):
+            year_slice = slice(s, e, None)
+
+        return year_slice
+
+    @staticmethod
+    def _check_for_years(time_slice):
+        """
+        Check to see if temporal slice is a year (str) or list of years (strs)
+        to extract data for
+
+        Parameters
+        ----------
+        time_slice : list | slice | int | str
+            Temporal slice to extract
+
+        Returns
+        -------
+        check : bool
+            True if temporal slice is a year (str) or list of years (strs),
+            else False
+        """
+        check = False
+        if isinstance(time_slice, (list, tuple)):
+            time_slice = time_slice[0]
+
+        if isinstance(time_slice, str):
+            check = True
+
+        return check
+
+    def _get_ds(self, ds_name, ds_slice):
+        """
+        Extract data from given dataset
+
+        Parameters
+        ----------
+        ds_name : str
+            Variable dataset to be extracted
+        ds_slice : int | list | slice
+            tuple describing slice of dataset array to extract
+
+        Returns
+        -------
+        out : ndarray
+            ndarray of variable timeseries data
+            If unscale, returned in native units else in scaled units
+        """
+        ds_slice = parse_slice(ds_slice)
+        out = []
+        if self._check_for_years(ds_slice[0]):
+            years = ds_slice[0]
+            year_slice = (slice(None), ) + ds_slice[1:]
+            if isinstance(years, str):
+                years = [years]
+
+            for year in years:
+                year = int(year)
+                out.append(self._get_year_ds(ds_name, year, year_slice))
+
+        else:
+            time_index = self.h5.time_index[ds_slice[0]]
+            year_map = time_index.year
+            for year in year_map.unique():
+                year_index = self.h5.year_index(year)
+                year_slice = \
+                    np.where(year_index.isin(time_index[year_map == year]))[0]
+                year_slice = \
+                    (self._check_year_slice(year_slice), ) + ds_slice[1:]
+                out.append(self._get_year_ds(ds_name, year, year_slice))
+
+        return np.concatenate(out, axis=0)
+
     def close(self):
         """
         Close h5 instance
         """
         self._h5.close()
 
 
-class MultiTimeSolarResource:
+class MultiYearSolarResource:
     """
-    Class to handle solar resource data stored temporaly accross multiple .h5
-    files
+    Class to handle multiple years of solar resource data stored accross
+    multiple .h5 files
     """
-
-    def __init__(self, h5_path, unscale=True, str_decode=True, hsds=False,
-                 hsds_kwargs=None):
+    def __init__(self, h5_path, unscale=True, str_decode=True, hsds=False):
         """
         Parameters
         ----------
-        h5_path : str | list
-            Unix shell style pattern path with * wildcards to multi-file
-            resource file sets. Files must have the same coordinates
-            but can have different datasets or time indexes. Can also be an
-            explicit list of multi time files.
+        h5_path : str
+            Path to directory containing multi-file resource file sets.
+            Available formats:
+                /h5_dir/
+                /h5_dir/prefix*suffix
         unscale : bool
             Boolean flag to automatically unscale variables on extraction
         str_decode : bool
             Boolean flag to decode the bytestring meta data into normal
             strings. Setting this to False will speed up the meta data read.
-        hsds : bool, optional
+        hsds : bool
             Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
-            behind HSDS, by default False
-        hsds_kwargs : dict, optional
-            Dictionary of optional kwargs for h5pyd, e.g., bucket, username,
-            password, by default None
+            behind HSDS
         """
         super().__init__(h5_path, unscale=unscale, hsds=hsds,
-                         hsds_kwargs=hsds_kwargs, str_decode=str_decode,
-                         res_cls=SolarResource)
+                         str_decode=str_decode, res_cls=SolarResource)
 
 
-class MultiTimeNSRDB(MultiTimeResource):
+class MultiYearNSRDB(MultiYearResource):
     """
-    Class to handle NSRDB data stored temporaly accross multiple .h5
-    files
+    Class to handle multiple years of NSRDB data stored accross
+    multiple .h5 files
     """
     PREFIX = 'nsrdb'
 
-    def __init__(self, h5_path, unscale=True, str_decode=True, hsds=False,
-                 hsds_kwargs=None):
+    def __init__(self, h5_path, unscale=True, str_decode=True, hsds=False):
         """
         Parameters
         ----------
-        h5_path : str | list
-            Unix shell style pattern path with * wildcards to multi-file
-            resource file sets. Files must have the same coordinates
-            but can have different datasets or time indexes. Can also be an
-            explicit list of multi time files.
+        h5_path : str
+            Path to directory containing multi-file resource file sets.
+            Available formats:
+                /h5_dir/
+                /h5_dir/prefix*suffix
         unscale : bool
             Boolean flag to automatically unscale variables on extraction
         str_decode : bool
             Boolean flag to decode the bytestring meta data into normal
             strings. Setting this to False will speed up the meta data read.
-        hsds : bool, optional
+        hsds : bool
             Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
-            behind HSDS, by default False
-        hsds_kwargs : dict, optional
-            Dictionary of optional kwargs for h5pyd, e.g., bucket, username,
-            password, by default None
+            behind HSDS
         """
         super().__init__(h5_path, unscale=unscale, hsds=hsds,
-                         hsds_kwargs=hsds_kwargs, str_decode=str_decode,
-                         res_cls=NSRDB)
+                         str_decode=str_decode, res_cls=NSRDB)
 
 
-class MultiTimeWindResource(MultiTimeResource):
+class MultiYearWindResource(MultiYearResource):
     """
-    Class to handle wind resource data stored temporaly accross multiple .h5
-    files
+    Class to handle multiple years of wind resource data stored accross
+    multiple .h5 files
     """
     PREFIX = 'wtk'
 
-    def __init__(self, h5_path, unscale=True, str_decode=True, hsds=False,
-                 hsds_kwargs=None):
+    def __init__(self, h5_path, unscale=True, str_decode=True, hsds=False):
         """
         Parameters
         ----------
-        h5_path : str | list
-            Unix shell style pattern path with * wildcards to multi-file
-            resource file sets. Files must have the same coordinates
-            but can have different datasets or time indexes. Can also be an
-            explicit list of multi time files.
+        h5_path : str
+            Path to directory containing multi-file resource file sets.
+            Available formats:
+                /h5_dir/
+                /h5_dir/prefix*suffix
         unscale : bool
             Boolean flag to automatically unscale variables on extraction
         str_decode : bool
             Boolean flag to decode the bytestring meta data into normal
             strings. Setting this to False will speed up the meta data read.
-        hsds : bool, optional
+        hsds : bool
             Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
-            behind HSDS, by default False
-        hsds_kwargs : dict, optional
-            Dictionary of optional kwargs for h5pyd, e.g., bucket, username,
-            password, by default None
+            behind HSDS
         """
         super().__init__(h5_path, unscale=unscale, hsds=hsds,
-                         hsds_kwargs=hsds_kwargs, str_decode=str_decode,
-                         res_cls=WindResource)
+                         str_decode=str_decode, res_cls=WindResource)
 
 
-class MultiTimeWaveResource(MultiTimeResource):
+class MultiYearWaveResource:
     """
-    Class to handle wave resource data stored temporaly accross multiple .h5
-    files
+    Class to handle multiple years of wave resource data stored accross
+    multiple .h5 files
     """
 
-    def __init__(self, h5_path, unscale=True, str_decode=True, hsds=False,
-                 hsds_kwargs=None):
+    def __init__(self, h5_path, unscale=True, str_decode=True, hsds=False):
         """
         Parameters
         ----------
-        h5_path : str | list
-            Unix shell style pattern path with * wildcards to multi-file
-            resource file sets. Files must have the same coordinates
-            but can have different datasets or time indexes. Can also be an
-            explicit list of multi time files.
+        h5_path : str
+            Path to directory containing multi-file resource file sets.
+            Available formats:
+                /h5_dir/
+                /h5_dir/prefix*suffix
         unscale : bool
             Boolean flag to automatically unscale variables on extraction
         str_decode : bool
             Boolean flag to decode the bytestring meta data into normal
             strings. Setting this to False will speed up the meta data read.
-        hsds : bool, optional
+        hsds : bool
             Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
-            behind HSDS, by default False
-        hsds_kwargs : dict, optional
-            Dictionary of optional kwargs for h5pyd, e.g., bucket, username,
-            password, by default None
+            behind HSDS
         """
         super().__init__(h5_path, unscale=unscale, hsds=hsds,
-                         hsds_kwargs=hsds_kwargs, str_decode=str_decode,
-                         res_cls=WaveResource)
+                         str_decode=str_decode, res_cls=WaveResource)
```

### Comparing `NREL-rex-0.2.81/rex/rechunk_h5/combine_h5_cli.py` & `NREL-rex-0.2.9/rex/rechunk_h5/rechunk_cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,69 @@
 # -*- coding: utf-8 -*-
 """
-Combined h5 command line interface
+Rechunk h5 command line interface
 """
 import click
-import logging
 import os
 
-from rex.rechunk_h5.combine_h5 import CombineH5
-from rex.utilities.cli_dtypes import INT
+from rex.rechunk_h5.rechunk_h5 import RechunkH5
 from rex.utilities.loggers import init_logger
-from rex import __version__
 
-logger = logging.getLogger(__name__)
 
-
-@click.command()
-@click.version_option(version=__version__)
-@click.option('--combined_h5', '-comb', type=click.Path(), required=True,
-              help="Path to save combined .h5 file to")
-@click.option('--source_h5', '-src', type=click.Path(exists=True),
-              required=True, multiple=True,
-              help="Path to source .h5 file, may supply multiple")
-@click.option('--axis', '-ax', type=int, default=1, show_default=True,
-              help='axis to combine datasets along, by default 1')
-@click.option('--overwrite', '-rm', is_flag=True,
-              help="Flag to overwrite an existing h5_dst file")
-@click.option('--process_size', '-s', default=None, type=INT,
-              show_default=True,
+@click.group(invoke_without_command=True)
+@click.option('--src_h5', '-src', type=click.Path(exists=True), required=True,
+              help="Source .h5 file path")
+@click.option('--dst_h5', '-dst', type=click.Path(), required=False,
+              help="Destination path for rechunked .h5 file")
+@click.option('--var_attrs_path', '-vap', type=click.Path(exists=True),
+              required=True,
+              help=".json containing variable attributes")
+@click.option('--version', '-ver', default=None,
+              help="File version number")
+@click.option('--meta', '-m', default=None, type=click.Path(exists=True),
+              help=("Path to .csv or .npy file containing meta to load into "
+                    "rechunked .h5 file"))
+@click.option('--process_size', '-s', default=None, type=int,
               help="Size of each chunk to be processed")
+@click.option('--check_dset_attrs', '-cda', is_flag=True,
+              help='Flag to compare source and specified dataset attributes')
+@click.option('--resolution', '-res', default=None, type=str,
+              help='New time resolution')
 @click.option('--log_file', '-log', default=None, type=click.Path(),
-              show_default=True,
-              help='Path to .log file, if None only log to stdout')
+              help='Path to .log file')
 @click.option('--verbose', '-v', is_flag=True,
               help='If used upgrade logging to DEBUG')
-def main(combined_h5, source_h5, axis, overwrite, process_size, log_file,
-         verbose):
+@click.pass_context
+def main(ctx, src_h5, dst_h5, var_attrs_path, version, meta, process_size,
+         check_dset_attrs, resolution, log_file, verbose):
     """
-    CombineH5 CLI entry point
+    RechunkH5 CLI entry point
     """
+    ctx.ensure_object(dict)
+
     if verbose:
         log_level = 'DEBUG'
     else:
         log_level = 'INFO'
 
     if log_file is not None:
         log_dir = os.path.dirname(log_file)
         if not os.path.exists(log_dir):
             os.makedirs(log_dir)
 
-    init_logger('rex', log_file=log_file, log_level=log_level)
+    init_logger('rex.rechunk_h5.rechunk_h5', log_file=log_file,
+                log_level=log_level)
 
-    dst_dir = os.path.dirname(combined_h5)
+    dst_dir = os.path.dirname(dst_h5)
     if not os.path.exists(dst_dir):
         os.makedirs(dst_dir)
 
-    CombineH5.run(combined_h5, *source_h5, axis=axis, overwrite=overwrite,
-                  process_size=process_size)
+    RechunkH5.run(src_h5, dst_h5, var_attrs_path,
+                  version=version, meta=meta, process_size=process_size,
+                  check_dset_attrs=check_dset_attrs, resolution=resolution)
 
 
 if __name__ == '__main__':
     try:
         main(obj={})
     except Exception:
-        logger.exception('Error running Combined H5')
         raise
```

### Comparing `NREL-rex-0.2.81/rex/rechunk_h5/rechunk_h5.py` & `NREL-rex-0.2.9/rex/rechunk_h5/rechunk_h5.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,139 +1,184 @@
 """
 Module to rechunk existing .h5 files
 """
 import h5py
 import logging
 import numpy as np
 import pandas as pd
+from pandas.api.types import CategoricalDtype
 import time
 from warnings import warn
 
-from rex.rechunk_h5.chunk_size import TimeseriesChunkSize, ArrayChunkSize
-from rex.utilities.loggers import log_versions
-from rex.utilities.utilities import (get_chunk_ranges, to_records_array,
-                                     pd_date_range)
-
 logger = logging.getLogger(__name__)
 
 
-def get_dataset_attributes(h5_file, out_json=None, chunk_size=2,
-                           weeks_per_chunk=None):
+def get_dataset_attributes(h5_file, out_json=None):
     """
     Extact attributes, dtype, and chunk size for all datasets in .h5 file
 
     Parameters
     ----------
     h5_file : str
         Path to source h5 file to scrape dataset data from
-    chunk_size : int, optional
-        Chunk size in MB, by default 2
-    weeks_per_chunk : int, optional
-        Number of weeks per time chunk, if None scale weeks based on 8
-        weeks for hourly data, by default None
     out_json : str, optional
         Path to output json to save DataFrame of dataset attributes to,
         by default None
 
     Returns
     -------
     ds_attrs : pandas.DataFrame
-        Attributes (attrs, dtype, shape, chunks) for all datasets in
-        source .h5 file
+        Attributes (attrs, dtype, chunks) for all datasets in source .h5 file
     """
     attrs_list = []
     with h5py.File(h5_file, 'r') as f:
-        global_attrs = dict(f.attrs)
-
-        for ds_name in f:
+        datasets = list(f)
+        for ds_name in datasets:
             ds = f[ds_name]
             try:
-                arr_size = ds_name in ['meta', 'coordinates', 'time_index']
-                arr_size |= len(ds.shape) < 2
-                if arr_size:
-                    chunks = ArrayChunkSize.compute(ds, chunk_size=chunk_size)
-                else:
-                    chunks = TimeseriesChunkSize.compute(
-                        ds.shape, ds.dtype,
-                        chunk_size=chunk_size,
-                        weeks_per_chunk=weeks_per_chunk)
-
                 attrs = dict(ds.attrs)
                 if not attrs:
-                    attrs = {}
+                    attrs = None
 
                 ds_attrs = {'attrs': attrs,
                             'dtype': ds.dtype.name,
-                            'shape': ds.shape,
-                            'chunks': chunks}
+                            'chunks': ds.chunks}
                 ds_attrs = pd.Series(ds_attrs)
                 ds_attrs.name = ds_name
                 attrs_list.append(ds_attrs.to_frame().T)
-            except Exception as ex:
-                msg = ('Could not extract attributes for {}: {}'
-                       .format(ds_name, ex))
-                logger.warning(msg)
-                warn(msg)
+            except Exception:
+                pass
 
     ds_attrs = pd.concat(attrs_list)
-    if global_attrs:
-        ds_attrs.loc['global'] = None
-        ds_attrs.at['global', 'attrs'] = global_attrs
-
     if out_json is not None:
         ds_attrs.to_json(out_json)
 
     return ds_attrs
 
 
+def get_chunk_slices(ds_dim, chunk_size):
+    """
+    Create list of chunk slices [(s_i, e_i), ...]
+
+    Parameters
+    ----------
+    ds_len : 'int'
+        Length of dataset axis to chunk
+    chunk_size : 'int'
+        Size of chunks
+
+    Returns
+    -------
+    chunks : 'list'
+        List of chunk start and end positions
+        [(s_i, e_i), (s_i+1, e_i+1), ...]
+    """
+    chunks = list(range(0, ds_dim, chunk_size))
+    if chunks[-1] < ds_dim:
+        chunks.append(ds_dim)
+    else:
+        chunks[-1] = ds_dim
+
+    chunks = list(zip(chunks[:-1], chunks[1:]))
+
+    return chunks
+
+
+def get_dtype(col):
+    """
+    Get column dtype for converstion to records array
+
+    Parameters
+    ----------
+    col : pandas.Series
+        Column from pandas DataFrame
+
+    Returns
+    -------
+    out : str
+        String representation of converted dtype for column:
+        -  float = float32
+        -  int = int16 or int32 depending on data range
+        -  object/str = U* max length of strings in col
+    """
+    dtype = col.dtype
+
+    if isinstance(dtype, CategoricalDtype):
+        col = col.astype(type(col.values[0]))
+        out = get_dtype(col)
+    elif np.issubdtype(dtype, np.floating):
+        out = 'float32'
+    elif np.issubdtype(dtype, np.integer):
+        if col.max() < 32767:
+            out = 'int16'
+        else:
+            out = 'int32'
+    elif np.issubdtype(dtype, np.object_):
+        size = int(col.astype(str).str.len().max())
+        out = 'S{:}'.format(size)
+    else:
+        out = dtype
+
+    return out
+
+
+def to_records_array(df):
+    """
+    Convert pandas DataFrame to numpy Records Array
+
+    Parameters
+    ----------
+    df : pandas.DataFrame
+        Pandas DataFrame to be converted
+
+    Returns
+    -------
+    numpy.rec.array
+        Records array of input df
+    """
+    meta_arrays = []
+    dtypes = []
+    for c_name, c_data in df.iteritems():
+        dtype = get_dtype(c_data)
+
+        if np.issubdtype(dtype, np.bytes_):
+            data = c_data.astype(str).str.encode('utf-8').values
+        else:
+            data = c_data.values
+
+        arr = np.array(data, dtype=dtype)
+        meta_arrays.append(arr)
+        dtypes.append((c_name, dtype))
+
+    return np.core.records.fromarrays(meta_arrays, dtype=dtypes)
+
+
 class RechunkH5:
     """
     Class to create new .h5 file with new chunking
     """
-    # None time-series
-    NON_TS_DSETS = ('meta', 'coordinates', 'time_index')
-
-    def __init__(self, h5_src, h5_dst, var_attrs=None, hub_height=None,
-                 chunk_size=2, weeks_per_chunk=None, overwrite=True):
+    def __init__(self, h5_src, h5_dst, version=None):
         """
         Initalize class object
 
         Parameters
         ----------
         h5_src : str
             Source .h5 file path
         h5_dst : str
             Destination path for rechunked .h5 file
-        var_attrs : str | pandas.DataFrame, optional
-            DataFrame of variable attributes or .json containing variable
-            attributes, by default None
-        hub_height : int | None, optional
-            Rechunk specific hub_height, by default None
-        chunk_size : int, optional
-            Chunk size in MB, by default 2
-        weeks_per_chunk : int, optional
-            Number of weeks per time chunk, if None scale weeks based on 8
-            weeks for hourly data, by default None
-        overwrite : bool, optional
-            Flag to overwrite an existing h5_dst file, by default True
+        version : str
+            File version number
         """
-        log_versions(logger)
         self._src_path = h5_src
         self._src_dsets = None
         self._dst_path = h5_dst
-        self._dst_h5 = h5py.File(h5_dst, mode='w' if overwrite else 'w-')
-
-        self._rechunk_attrs = self._get_var_attrs(
-            var_attrs=var_attrs,
-            hub_height=hub_height,
-            chunk_size=chunk_size,
-            weeks_per_chunk=weeks_per_chunk)
-        if self.global_attrs is not None:
-            for k, v in self.global_attrs['attrs'].items():
-                self._dst_h5.attrs[k] = v
+        self._dst_h5 = h5py.File(h5_dst, 'w')
+        if version:
+            self._dst_h5.attrs['version'] = version
 
         self._time_slice = None
 
     def __enter__(self):
         return self
 
     def __exit__(self, type, value, traceback):
@@ -182,115 +227,14 @@
 
         Returns
         -------
         slice
         """
         return self._time_slice
 
-    @property
-    def rechunk_attrs(self):
-        """
-        Attributes for rechunked files, includes dataset and global attrs
-
-        Returns
-        -------
-        pandas.DataFrame
-        """
-        return self._rechunk_attrs
-
-    @property
-    def global_attrs(self):
-        """
-        Global attributes
-
-        Returns
-        -------
-        pandas.Series
-        """
-        return self._get_attrs('global')
-
-    @property
-    def time_index_attrs(self):
-        """
-        Time index attributes
-
-        Returns
-        -------
-        pandas.Series
-        """
-        return self._get_attrs('time_index')
-
-    @property
-    def meta_attrs(self):
-        """
-        Meta attributes
-
-        Returns
-        -------
-        pandas.Series
-        """
-        return self._get_attrs('meta')
-
-    @property
-    def coordinates_attrs(self):
-        """
-        Coordinates attributes
-
-        Returns
-        -------
-        pandas.Series
-        """
-        return self._get_attrs('coordinates')
-
-    @property
-    def variable_attrs(self):
-        """
-        Variable attributes
-
-        Returns
-        -------
-        pandas.Series
-        """
-        return self._get_attrs('variables')
-
-    @classmethod
-    def _get_hub_height_attrs(cls, var_attrs, hub_height):
-        """
-        Extract attributes for variables at given hub height
-
-        Parameters
-        ----------
-        var_attrs : pandas.DataFrame
-            All variable attributes
-        hub_height : int
-            Hub height of interest
-
-        Returns
-        -------
-        var_attrs : pandas.DataFrame
-            Variable attributes associated with given hub height
-        """
-        variables = var_attrs.index
-        h_flag = '_{}m'.format(hub_height)
-        file_vars = [v for v in variables if h_flag in v]
-        if h_flag == '_0m':
-            for v in variables:
-                check = (v not in cls.NON_TS_DSETS
-                         and not v.endswith(('0m', '2m')))
-                if check:
-                    file_vars.append(v)
-
-        for v in variables:
-            if v in cls.NON_TS_DSETS:
-                file_vars.append(v)
-
-        var_attrs = var_attrs.loc[file_vars]
-
-        return var_attrs
-
     @staticmethod
     def _check_dtype(ds_in, dset_attrs):
         """
         Check dataset dtype against source dataset dtype
 
         Parameters
         ----------
@@ -321,15 +265,15 @@
                     logger.warning(msg)
                     warn(msg)
             elif int_to_float:
                 msg = ('Cannot scale up an {} to a {}'
                        .format(ds_in.dtype, dtype))
                 logger.error(msg)
                 raise RuntimeError(msg)
-            elif np.dtype(dtype).itemsize > ds_in.dtype.itemsize:
+            elif not np.issubdtype(dtype, ds_in.dtype):
                 msg = ('Output dtype ({}) has greater precision than input '
                        'dtype ({}), using input dtype'
                        .format(dtype, ds_in.dtype))
                 logger.warning(msg)
                 warn(msg)
 
                 dset_attrs['dtype'] = ds_in.dtype
@@ -362,34 +306,34 @@
                     logger.warning(msg)
                     warn(msg)
 
                     dset_attrs['attrs'][key] = src_value
 
         return dset_attrs
 
-    @classmethod
-    def check_dset_attrs(cls, ds_in, dset_attrs, check_attrs=False):
+    @staticmethod
+    def check_dset_attrs(ds_in, dset_attrs, check_attrs=False):
         """
         Check dataset attributes (dtype, scale_factor, units) against source
         Dataset
 
         Parameters
         ----------
         ds_in : h5py.Dataset
             Source h5 Dataset
         dset_attrs : dict
             Dictionary of dataset attributes (dtype, chunk, attrs)
         check_attrs : bool, optional
             Flag to compare source and specified dataset attributes,
             by default False
         """
-        dset_attrs = cls._check_dtype(ds_in, dset_attrs)
+        dset_attrs = RechunkH5._check_dtype(ds_in, dset_attrs)
 
         if check_attrs:
-            dset_attrs = cls._check_attrs(ds_in, dset_attrs)
+            dset_attrs = RechunkH5._check_attrs(ds_in, dset_attrs)
 
         return dset_attrs
 
     @staticmethod
     def _check_data(data, dset_attrs):
         """
         Check data dtype and scale if needed
@@ -422,122 +366,14 @@
             if np.issubdtype(dtype, np.integer):
                 data = np.round(data)
 
             data = data.astype(dtype)
 
         return data
 
-    @staticmethod
-    def _check_chunks(chunks, shape):
-        """
-        Check chunks to ensure they are properly formatted:
-        - None or a tuple
-        - same shape as dset_shape
-        - contain all integer values
-
-        Parameters
-        ----------
-        chunks : list | tuple | None
-            Dataset chunks
-        shape : tuple
-            Dataset shape
-
-        Returns
-        -------
-        chunks : tuple | None
-            Updated chunks if "None" was supplied for either axis.
-        """
-        if chunks is not None:
-            if not isinstance(chunks, tuple):
-                chunks = tuple(chunks)
-
-            msg = ("Chunks {} do not match dataset shape {}!"
-                   .format(chunks, shape))
-            assert len(chunks) == len(shape), msg
-
-            if None in chunks:
-                chunk_sizes = chunks
-                chunks = ()
-                for i, c in enumerate(chunk_sizes):
-                    if c is None:
-                        chunks += (shape[i], )
-                    else:
-                        chunks += (c, )
-
-        return chunks
-
-    def _get_var_attrs(self, var_attrs=None, hub_height=None, chunk_size=2,
-                       weeks_per_chunk=None):
-        """
-        Parse variable attributes from file if needed
-
-        Parameters
-        ----------
-        var_attrs : str | pandas.DataFrame, optional
-            DataFrame of variable attributes or .json containing variable
-            attributes, if None build from source .h5 file, by default None
-        hub_height : int | None, optional
-            Rechunk specific hub_height, by default None
-
-        Returns
-        -------
-        var_attrs : pandas.DataFrame
-            DataFrame mapping variable (dataset) name to .h5 attributes
-        """
-        if var_attrs is None:
-            var_attrs = get_dataset_attributes(self._src_path,
-                                               chunk_size=chunk_size,
-                                               weeks_per_chunk=weeks_per_chunk)
-
-        if isinstance(var_attrs, str):
-            var_attrs = pd.read_json(var_attrs)
-        elif not isinstance(var_attrs, pd.DataFrame):
-            msg = ("Variable attributes are expected as a .json file or a "
-                   "pandas DataFrame, but a {} was provided!"
-                   .format(type(var_attrs)))
-            logger.error(msg)
-            raise TypeError(msg)
-
-        var_attrs = var_attrs.where(var_attrs.notnull(), None)
-
-        if hub_height is not None:
-            var_attrs = self._get_hub_height_attrs(var_attrs, hub_height)
-            logger.debug('Reducing variable attributes to variables at hub '
-                         'height {}m:\n{}'.format(hub_height, var_attrs.index))
-
-        return var_attrs
-
-    def _get_attrs(self, index):
-        """
-        Extract attributes for desired dataset(s)
-
-        Parameters
-        ----------
-        index : str
-            rechunk_attrs index to extract. To extract variable attrs, use
-            'variables'
-
-        Returns
-        -------
-        pandas.Series
-            Attributes for given index value(s)
-        """
-        non_ts_attrs = self.NON_TS_DSETS + ('global', )
-        if index in self.rechunk_attrs.index:
-            attrs = self.rechunk_attrs.loc[index]
-        elif index.lower().startswith('variable'):
-            variables = [idx for idx in self.rechunk_attrs.index
-                         if (idx in self.src_dsets)
-                         and (idx not in non_ts_attrs)]
-            attrs = self.rechunk_attrs.loc[variables]
-        else:
-            attrs = None
-
-        return attrs
-
     def init_dset(self, dset_name, dset_shape, dset_attrs):
         """
         Create dataset and add attributes and load data if needed
 
         Parameters
         ----------
         dset_name : str
@@ -549,36 +385,31 @@
 
         Returns
         -------
         ds : h5py.Dataset
             Initalized h5py Dataset instance
         """
         dtype = dset_attrs['dtype']
+        chunks = dset_attrs['chunks']
         attrs = dset_attrs['attrs']
-        chunks = self._check_chunks(dset_attrs['chunks'], dset_shape)
-
         name = dset_attrs.get('name', None)
         if name is not None:
-            if name is not str:
-                msg = ("dataset attribute `name` (value: {}, type: {}) must "
-                       "be a string. Check the attributes of the dataset "
-                       "({}). If using an external json file for variable "
-                       "attributes, it might be using `null` for the name."
-                       .format(name, type(name), dset_name))
-                logger.error(msg)
-                raise RuntimeError(msg)
             dset_name = name
 
+        if chunks:
+            chunks = tuple(chunks)
+
         logger.debug('Creating {} with shape: {}, dtype: {}, chunks: {}'
                      .format(dset_name, dset_shape, dtype, chunks))
         ds = self._dst_h5.create_dataset(dset_name, shape=dset_shape,
                                          dtype=dtype, chunks=chunks)
         if attrs:
             for attr, value in attrs.items():
-                ds.attrs[attr] = value
+                if attr not in ['freq', 'start']:
+                    ds.attrs[attr] = value
 
         logger.info('- {} initialized'.format(dset_name))
 
         return ds
 
     def load_time_index(self, attrs, resolution=None):
         """
@@ -602,15 +433,15 @@
             if timezone is not None:
                 if time_index.tz is not None:
                     time_index = time_index.tz_convert(timezone)
                 else:
                     time_index = time_index.tz_localize(timezone)
 
             if resolution is not None:
-                resample = pd_date_range(time_index.min(), time_index.max(),
+                resample = pd.date_range(time_index.min(), time_index.max(),
                                          freq=resolution)
                 if len(resample) > len(time_index):
                     msg = ("Resolution ({}) must be > time_index resolution "
                            "({})".format(resolution, time_index.freq))
                     logger.error(msg)
                     raise RuntimeError(msg)
 
@@ -671,15 +502,15 @@
         attrs : pandas.Series
             Dataset attributes associated with coordinates
         """
         ts = time.time()
         logger.info('Rechunking coordinates')
         meta_data = self._dst_h5['meta'][...]
         coords = np.dstack((meta_data['latitude'], meta_data['longitude']))[0]
-        attrs['dtype'] = 'float32'
+        attrs['dtype'] = coords.dtype
 
         if isinstance(attrs['chunks'], int):
             attrs['chunks'] = (attrs['chunks'], 2)
 
         ds = self.init_dset('coordinates', coords.shape, attrs)
         ds[...] = coords
         logger.info('- coordinates transfered')
@@ -713,15 +544,15 @@
             chunks = ds_in.chunks
             if isinstance(chunks, tuple):
                 sites = shape[1]
             else:
                 by_rows = True
                 sites = shape[0]
 
-            slice_map = get_chunk_ranges(sites, process_size)
+            slice_map = get_chunk_slices(sites, process_size)
             for s, e in slice_map:
                 if by_rows:
                     ds_out[s:e] = self._check_data(ds_in[s:e], dset_attrs)
                 else:
                     data = ds_in[:, s:e]
                     if reduce:
                         data = data[self.time_slice]
@@ -785,109 +616,168 @@
             logger.info('- {} transfered'.format(dset_name))
             tt = (time.time() - ts) / 60
             logger.debug('\t- {:.2f} minutes'.format(tt))
         else:
             logger.warning('{} already exists in {}'
                            .format(dset_name, self._dst_path))
 
-    def rechunk(self, meta=None, process_size=None,
+    @staticmethod
+    def pop_dset_attrs(var_attrs, dset):
+        """
+        Pop attributres for given dataset from dataset attributes DataFrame
+
+        Parameters
+        ----------
+        dset_attrs : pandas.DataFrame
+            DataFrame of dataset attributes (dtype, chunks, attrs)
+        dset : str
+            Dataset of interest
+
+        Returns
+        -------
+        dset_attrs : pandas.DataFrame
+            Updated DataFrame of dataset attributes (dtype, chunks, attrs)
+        attrs : pandas.Series
+            Series of attributes for given dataset
+        """
+        attrs = var_attrs.loc[dset]
+        var_attrs = var_attrs.drop(dset)
+
+        return var_attrs, attrs
+
+    @staticmethod
+    def _parse_var_attrs(var_attrs):
+        """
+        Parse variable attributes from file if needed
+
+        Parameters
+        ----------
+        var_attrs : str | pandas.DataFrame
+            DataFrame of variable attributes or .json containing variable
+            attributes
+
+        Returns
+        -------
+        var_attrs : pandas.DataFrame
+            DataFrame mapping variable (dataset) name to .h5 attributes
+        """
+        if isinstance(var_attrs, str):
+            var_attrs = pd.read_json(var_attrs)
+        elif not isinstance(var_attrs, pd.DataFrame):
+            msg = ("Variable attributes are expected as a .json file or a "
+                   "pandas DataFrame, but a {} was provided!"
+                   .format(type(var_attrs)))
+            logger.error(msg)
+            raise TypeError(msg)
+
+        var_attrs = var_attrs.where(var_attrs.notnull(), None)
+
+        return var_attrs
+
+    def rechunk(self, var_attrs, meta=None, process_size=None,
                 check_dset_attrs=False, resolution=None):
         """
         Rechunk all variables in given variable attributes json
 
         Parameters
         ----------
-        meta : str, optional
+        var_attrs : str | pandas.DataFrame
+            DataFrame of variable attributes or .json containing variable
+            attributes
+        meta : str
             Path to .csv or .npy file containing meta to load into
-            rechunked .h5 file, by default None
-        process_size : int, optional
-            Size of each chunk to be processed at a time, by default None
+            rechunked .h5 file
+        process_size : int
+            Size of each chunk to be processed at a time
         check_dset_attrs : bool, optional
             Flag to compare source and specified dataset attributes,
             by default False
         resolution : str, optional
             New time resolution, by default None
         """
         try:
             ts = time.time()
             with h5py.File(self._src_path, 'r') as f_in:
                 for k, v in f_in.attrs.items():
                     logger.debug('Transfering global attribute {}'
                                  .format(k))
                     self._dst_h5.attrs[k] = v
-                # Process time_index
-            if self.time_index_attrs is not None:
-                self.load_time_index(self.time_index_attrs,
+
+            var_attrs = self._parse_var_attrs(var_attrs)
+            if 'global' in var_attrs.index:
+                var_attrs, global_attrs = self.pop_dset_attrs(var_attrs,
+                                                              'global')
+
+                for k, v in global_attrs['attrs'].items():
+                    self._dst_h5.attrs[k] = v
+
+            # Process time_index
+            if 'time_index' in var_attrs.index:
+                var_attrs, time_index_attrs = self.pop_dset_attrs(var_attrs,
+                                                                  'time_index')
+                self.load_time_index(time_index_attrs,
                                      resolution=resolution)
 
             # Process meta
-            if self.meta_attrs is not None:
-                self.load_meta(self.meta_attrs, meta_path=meta)
+            if 'meta' in var_attrs.index:
+                var_attrs, meta_attrs = self.pop_dset_attrs(var_attrs, 'meta')
+                self.load_meta(meta_attrs, meta_path=meta)
 
             # Process coordinates
-            if self.coordinates_attrs is not None:
-                self.load_coords(self.coordinates_attrs)
-
-            for dset_name, dset_attrs in self.variable_attrs.iterrows():
+            if 'coordinates' in var_attrs.index:
+                var_attrs, coords_attrs = self.pop_dset_attrs(var_attrs,
+                                                              'coordinates')
+                self.load_coords(coords_attrs)
+
+            mask = var_attrs.index.isin(self.src_dsets)
+            var_attrs = var_attrs.loc[mask]
+            for dset_name, dset_attrs in var_attrs.iterrows():
                 self.load_dset(dset_name, dset_attrs,
                                process_size=process_size,
                                check_attrs=check_dset_attrs)
 
             tt = (time.time() - ts) / 60
             logger.debug('\t- {:} created in {:.2f} minutes'
                          .format(self._dst_path, tt))
         except Exception:
             logger.exception('Error creating {:}'.format(self._dst_path))
-            raise
 
     @classmethod
-    def run(cls, h5_src, h5_dst, var_attrs=None, hub_height=None,
-            chunk_size=2, weeks_per_chunk=None, overwrite=True, meta=None,
+    def run(cls, h5_src, h5_dst, var_attrs, version=None, meta=None,
             process_size=None, check_dset_attrs=False, resolution=None):
         """
         Rechunk h5_src to h5_dst using given attributes
 
         Parameters
         ----------
         h5_src : str
             Source .h5 file path
         h5_dst : str
             Destination path for rechunked .h5 file
         var_attrs : str | pandas.DataFrame
             DataFrame of variable attributes or .json containing variable
             attributes
-        hub_height : int | None, optional
-            Rechunk specific hub_height, by default None
-        chunk_size : int, optional
-            Chunk size in MB, by default 2
-        weeks_per_chunk : int, optional
-            Number of weeks per time chunk, if None scale weeks based on 8
-            weeks for hourly data, by default None
-        overwrite : bool, optional
-            Flag to overwrite an existing h5_dst file, by default True
-        meta : str, optional
+        version : str
+            File version number
+        meta : str
             Path to .csv or .npy file containing meta to load into
-            rechunked .h5 file, by default None
-        process_size : int, optional
-            Size of each chunk to be processed at a time, by default None
+            rechunked .h5 file
+        process_size : int
+            Size of each chunk to be processed at a time
         check_dset_attrs : bool, optional
             Flag to compare source and specified dataset attributes,
             by default False
         resolution : str, optional
             New time resolution, by default None
         """
         logger.info('Rechunking {} to {} using chunks given in {}'
                     .format(h5_src, h5_dst, var_attrs))
         try:
-            kwargs = {'hub_height': hub_height,
-                      'chunk_size': chunk_size,
-                      'weeks_per_chunk': weeks_per_chunk,
-                      'overwrite': overwrite}
-            with cls(h5_src, h5_dst, var_attrs, **kwargs) as r:
-                r.rechunk(meta=meta, process_size=process_size,
+            with cls(h5_src, h5_dst, version=version) as r:
+                r.rechunk(var_attrs, meta=meta, process_size=process_size,
                           check_dset_attrs=check_dset_attrs,
                           resolution=resolution)
 
             logger.info('{} complete'.format(h5_dst))
         except Exception:
             logger.exception("Error rechunking {}".format(h5_src))
             raise
```

### Comparing `NREL-rex-0.2.81/rex/renewable_resource.py` & `NREL-rex-0.2.9/rex/renewable_resource.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,38 @@
 # -*- coding: utf-8 -*-
-# pylint: disable=no-member
 """
 Classes to handle renewable resource data
 """
-import re
-from abc import abstractmethod
 import numpy as np
-import os
 import pandas as pd
 import warnings
-import logging
 
-from rex.resource import BaseResource
+from rex.resource import Resource, MultiFileResource
 from rex.sam_resource import SAMResource
 from rex.utilities.exceptions import (ResourceValueError, ExtrapolationWarning,
-                                      ResourceWarning, ResourceRuntimeError,
-                                      ResourceKeyError,
+                                      ResourceWarning,
                                       MoninObukhovExtrapolationError)
-from rex.utilities.parse_keys import parse_keys
 
 
-logger = logging.getLogger(__name__)
-
-
-class WaveResource(BaseResource):
+class SolarResource(Resource):
     """
-    Class to handle Wave BaseResource .h5 files
+    Class to handle Solar Resource .h5 files
 
     See Also
     --------
-    resource.BaseResource : Parent class
+    resource.Resource : Parent class
     """
-
-    def get_SAM_df(self, site):
+    def _get_SAM_df(self, ds_name, site):
         """
-        Get SAM wave resource DataFrame for given site
+        Get SAM solar resource DataFrame for given site
 
         Parameters
         ----------
+        ds_name : str
+            'Dataset' name == SAM
         site : int
             Site to extract SAM DataFrame for
 
         Returns
         -------
         res_df : pandas.DataFrame
             time-series DataFrame of resource variables needed to run SAM
@@ -55,858 +46,231 @@
                                'Hour': self.time_index.hour})
         if len(self) > 8784:
             res_df['Minute'] = self.time_index.minute
 
         time_zone = self.meta.loc[site, 'timezone']
         time_interval = len(self.time_index) // 8760
 
-        for var in ['significant_wave_height', 'energy_period']:
-            ds_slice = (slice(None), site)
-            var_array = self._get_ds(var, ds_slice)
-            var_array = SAMResource.roll_timeseries(var_array, time_zone,
-                                                    time_interval)
-            res_df[var] = var_array
-
-        col_map = {'significant_wave_height': 'wave_height',
-                   'energy_period': 'wave_period'}
-        res_df = res_df.rename(columns=col_map)
-        res_df.name = "SAM_-{}".format(site)
-
-        return res_df
-
-    @staticmethod
-    def _preload_SAM(res, sites, means=False, time_index_step=None):
-        """
-        Pre-load project_points for SAM
-
-        Parameters
-        ----------
-        res : rex.Resource
-            rex Resource handler or similar (NSRDB, WindResource,
-            MultiFileResource, etc...)
-        sites : list
-            List of sites to be provided to SAM
-        means : bool
-            Boolean flag to compute mean resource when res_array is set
-        time_index_step: int, optional
-            Step size for time_index, used to reduce temporal resolution,
-            by default None
-
-        Returns
-        -------
-        SAM_res : SAMResource
-            Instance of SAMResource pre-loaded with Wave resource for sites
-            in project_points
-        """
-        SAM_res = super()._preload_SAM(res, sites, 'wave', means=means,
-                                       time_index_step=time_index_step)
-
-        return SAM_res
-
-    @classmethod
-    def preload_SAM(cls, h5_file, sites, unscale=True, str_decode=True,
-                    group=None, hsds=False, hsds_kwargs=None, means=False,
-                    time_index_step=None):
-        """
-        Pre-load project_points for SAM
-
-        Parameters
-        ----------
-        h5_file : str
-            h5_file to extract resource from
-        sites : list
-            List of sites to be provided to SAM
-        unscale : bool
-            Boolean flag to automatically unscale variables on extraction
-        str_decode : bool
-            Boolean flag to decode the bytestring meta data into normal
-            strings. Setting this to False will speed up the meta data read.
-        group : str
-            Group within .h5 resource file to open
-        hsds : bool, optional
-            Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
-            behind HSDS, by default False
-        hsds_kwargs : dict, optional
-            Dictionary of optional kwargs for h5pyd, e.g., bucket, username,
-            password, by default None
-        means : bool
-            Boolean flag to compute mean resource when res_array is set
-        time_index_step: int, optional
-            Step size for time_index, used to reduce temporal resolution,
-            by default None
-
-        Returns
-        -------
-        SAM_res : SAMResource
-            Instance of SAMResource pre-loaded with Wave resource for sites
-            in project_points
-        """
-        kwargs = {"unscale": unscale, "hsds": hsds, 'hsds_kwargs': hsds_kwargs,
-                  "str_decode": str_decode, "group": group}
-        with cls(h5_file, **kwargs) as res:
-            SAM_res = res._preload_SAM(res, sites, means=means,
-                                       time_index_step=time_index_step)
-
-        return SAM_res
-
-
-class AbstractInterpolatedResource(BaseResource):
-    """Class to handle resource dataset interpolation.
-
-    Default type of interpolation is linear.
-
-    Pressure and Temperature lapse rates are used if p and t are only given at
-    a single hub height. The lapse rates are from the International Standard
-    Atmosphere (ISA) or ICAO Standard Atmosphere:
-    (https://www.faa.gov/regulations_policies/handbooks_manuals/aviation/
-     phak/media/06_phak_ch4.pdf)
-    """
-
-    LAPSE_RATES = {'temperature': 6.56, 'pressure': 11_109}
-    """Air Temperature and Pressure lapse rate in C/km and Pa/km"""
-
-    def __init__(self, h5_file, mode='r', unscale=True, str_decode=True,
-                 group=None, use_lapse_rate=True, hsds=False,
-                 hsds_kwargs=None):
-        """
-        Parameters
-        ----------
-        h5_file : str
-            Path to .h5 resource file
-        mode : str, optional
-            Mode to instantiate h5py.File instance, by default 'r'
-        unscale : bool
-            Boolean flag to automatically unscale variables on extraction
-        str_decode : bool
-            Boolean flag to decode the bytestring meta data into normal
-            strings. Setting this to False will speed up the meta data read.
-        group : str
-            Group within .h5 resource file to open
-        use_lapse_rate : bool
-            If a dataset is only available at a single hub-height and this flag
-            value is set to `True`, pressure / temperature values will be
-            calculated using linear lapse rate adjustment from the available
-            hub height to the requested one. If the flag value is set to
-            `False`, the value of these variables at the single available
-            hub-height will be returned for *all* requested heights. This
-            option has no effect if data is available at multiple hub-heights.
-        hsds : bool, optional
-            Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
-            behind HSDS, by default False
-        hsds_kwargs : dict, optional
-            Dictionary of optional kwargs for h5pyd, e.g., bucket, username,
-            password, by default None
-        """
-        self._interp_var = None
-        self._use_lapse = use_lapse_rate
-        super().__init__(h5_file, unscale=unscale, str_decode=str_decode,
-                         group=group, hsds=hsds, mode=mode,
-                         hsds_kwargs=hsds_kwargs)
-
-        # this is where self.heights or self.depths gets set
-        self._interpolation_variable = self._parse_interp_var(self.datasets)
-        prop_name = "{}s".format(self.VARIABLE_NAME)
-        setattr(self, prop_name, self._interpolation_variable)
-
-    @classmethod
-    def _parse_interp_var(cls, datasets):
-        """Extract available interpolation variable values for the
-        interpolable datasets. Used for interpolation/extrapolation.
-
-        Parameters
-        ----------
-        datasets : list
-            List of dataset names that will be parsed for interpolation value
-            suffixes like "windspeed_100m" -> windspeed at 100 meters
-
-        Returns
-        -------
-        dict
-            Dictionary of available interpolation variable values for
-            the interpolable datasets. For example, this could be:
-            {'windspeed': [10, 100, 200]}
-        """
-        interp_var = {dset: [] for dset in cls.INTERPOLABLE_DSETS}
-        ignore = ['meta', 'time_index', 'coordinates']
-        for ds in datasets:
-            if ds not in ignore:
-                ds_name, val = cls._parse_name(ds)
-                if ds_name in interp_var and val is not None:
-                    interp_var[ds_name].append(val)
-
-        return interp_var
-
-    @classmethod
-    def _parse_name(cls, ds_name):
-        """Extract dataset name and interpolation variable value from
-        dataset name.
-
-        Parameters
-        ----------
-        ds_name : str
-            Dataset name
-
-        Returns
-        -------
-        name : str
-            Dataset name without interpolation value.
-        val : int | float
-            Variable value.
-        """
-
-        regex = "_-?[0-9]+(.[0-9]+)?{}$".format(cls.VARIABLE_UNIT)
-        regex = re.search(regex, ds_name)
-        if regex:
-            val = regex.group()
-            name = ds_name.rstrip(val)
-            val = val.lstrip('_').rstrip(cls.VARIABLE_UNIT)
-
-            try:
-                val = int(val)
-            except ValueError:
-                val = float(val)
-
-            return name, val
-
-        return ds_name, None
-
-    @classmethod
-    def _get_nearest_val(cls, val, vals):
-        """
-        Get two nearest two values in `vals`.
-        Determine if val is inside or outside the range of vals
-        (requiring extrapolation instead of interpolation)
-
-        Parameters
-        ----------
-        val : int | float
-            Value of interest.
-        vals : list
-            List of available values.
-
-        Returns
-        -------
-        nearest_val : list
-            List of 1st and 2nd nearest val in vals.
-        extrapolate : bool
-            Flag as to whether val is inside or outside vals range
-        """
-
-        vals_arr = np.array(vals, dtype='float32')
-        dist = np.abs(vals_arr - val)
-        pos = dist.argsort()[:2]
-        nearest_d = sorted([vals[p] for p in pos])
-        extrapolate = np.all(val < vals_arr) or np.all(val > vals_arr)
-
-        if extrapolate:
-            v_min, v_max = np.sort(vals)[[0, -1]]
-            msg = ('{} is outside the {} range'.format(val, cls.VARIABLE_NAME),
-                   '({}, {}).'.format(v_min, v_max),
-                   'Extrapolation to be used.')
-            warnings.warn(' '.join(msg), ExtrapolationWarning)
-
-        return nearest_d, extrapolate
-
-    def _get_closest_existing_dset_name(self, dset):
-        """Get the name of an existing dataset closest to interp value. """
-
-        var_name, val = self._parse_name(dset)
-        if val is not None and var_name in self._interpolation_variable:
-            available_vals = self._interpolation_variable[var_name]
-            (val, _), _ = self._get_nearest_val(val, available_vals)
-            dset = '{}_{}{}'.format(var_name, val, self.VARIABLE_UNIT)
-
-        return dset
-
-    def get_dset_properties(self, dset):
-        """
-        Get dataset properties (shape, dtype, chunks)
-
-        Parameters
-        ----------
-        dset : str
-            Dataset to get scale factor for
-
-        Returns
-        -------
-        shape : tuple
-            Dataset array shape
-        dtype : str
-            Dataset array dtype
-        chunks : tuple
-            Dataset chunk size
-        """
-        dset = self._get_closest_existing_dset_name(dset)
-        return super().get_dset_properties(dset)
-
-    def get_attrs(self, dset=None):
-        """
-        Get h5 attributes either from file or dataset
-
-        Parameters
-        ----------
-        dset : str
-            Dataset to get attributes for, if None get file (global) attributes
-
-        Returns
-        -------
-        attrs : dict
-            Dataset or file attributes
-        """
-        if dset is None:
-            attrs = dict(self.h5.attrs)
-        else:
-            dset = self._get_closest_existing_dset_name(dset)
-            attrs = super().get_attrs(dset=dset)
-
-        return attrs
-
-    def _get_ds(self, ds_name, ds_slice):
-        """
-        Extract data from given dataset
-
-        Parameters
-        ----------
-        ds_name : str
-            Variable dataset to be extracted
-        ds_slice : tuple
-            Tuple of (int, slice, list, ndarray) of what to extract from
-            ds, each arg is for a sequential axis
-
-        Returns
-        -------
-        out : ndarray
-            ndarray of variable timeseries data
-            If unscale, returned in native units else in scaled units
-        """
-        var_name, val = self._parse_name(ds_name)
-        if val is not None and var_name in self._interpolation_variable:
-            out = self._get_ds_interpolated(ds_name, ds_slice)
-        else:
-            out = super()._get_ds(ds_name, ds_slice)
-
-        return out
-
-    def _get_ds_interpolated(self, ds_name, ds_slice):
-        """Extract data from given dataset at desired interpolation value.
-
-        Data is interpolated or extrapolated as needed.
-
-        Parameters
-        ----------
-        ds_name : str
-            Variable dataset to be extracted
-        ds_slice : tuple
-            Tuple of (int, slice, list, ndarray) of what to extract
-            from ds, each arg is for a sequential axis
-
-        Returns
-        -------
-        out : ndarray
-            ndarray of variable timeseries data
-            If unscale, returned in native units else in scaled units
-        """
-        var_name, val = self._parse_name(ds_name)
-        interpolation_values = self._interpolation_variable[var_name]
-
-        if not interpolation_values:
-            warnings.warn('No {0} info available for {1!r}, returning '
-                          'single {2!r} value for requested {0} {3}{4}'
-                          .format(self.VARIABLE_NAME, ds_name, var_name, val,
-                                  self.VARIABLE_UNIT), ResourceWarning)
-            out = super()._get_ds(var_name, ds_slice)
-
-        elif val in interpolation_values:
-            ds_name = '{}_{}{}'.format(var_name, int(val), self.VARIABLE_UNIT)
-            out = super()._get_ds(ds_name, ds_slice)
-
-        elif (len(interpolation_values) == 1
-              and self._use_lapse
-              and var_name in self.LAPSE_RATES):
-            out = self._get_ds_lapse(ds_name, ds_slice)
-
-        elif len(interpolation_values) == 1:
-            val = interpolation_values[0]
-            ds_name = '{}_{}{}'.format(var_name, int(val), self.VARIABLE_UNIT)
-            warnings.warn('Only one {} available, returning {!r}'
-                          .format(self.VARIABLE_NAME, ds_name),
-                          ResourceWarning)
-            out = super()._get_ds(ds_name, ds_slice)
-
-        else:
-            out = self._get_calculated_ds(val, ds_name, var_name, ds_slice)
-
-        return out
-
-    def _get_ds_lapse(self, ds_name, ds_slice,
-                      valid_units=('pa', 'pascals',
-                                   'c', 'celsius',
-                                   'k', 'kelvin')):
-        """Extract data from given dataset where there is only temperature or
-        pressure data at a single elevation and a lapse rate must be used to
-        adjust to a new elevation.
-
-        Parameters
-        ----------
-        ds_name : str
-            Variable dataset to be extracted
-        ds_slice : tuple
-            Tuple of (int, slice, list, ndarray) of what to extract
-            from ds, each arg is for a sequential axis
-        valid_units : tuple
-            Tuple of valid lower-case units that can be lapse-rate adjusted. If
-            the dataset doesnt have units in this list, a warning will be
-            raised.
-
-        Returns
-        -------
-        out : ndarray
-            ndarray of variable timeseries data
-            If unscale, returned in native units else in scaled units
-        """
-
-        var_name, val = self._parse_name(ds_name)
-        interpolation_values = self._interpolation_variable[var_name]
-        ds_name = '{}_{}{}'.format(var_name, int(interpolation_values[0]),
-                                   self.VARIABLE_UNIT)
-        lapse_rate = self.LAPSE_RATES[var_name]
-
-        if self.VARIABLE_UNIT != 'm':
-            msg = ('Cannot use temperature/pressure lapse rate when vertical '
-                   'interpolation unit is not "m": {}'
-                   .format(self.VARIABLE_UNIT))
-            logger.error(msg)
-            raise RuntimeError(msg)
-
-        logger.info('Only one {} available for {} at {}, using '
-                    'lapse rate of {} to get to {}'
-                    .format(self.VARIABLE_NAME, var_name,
-                            interpolation_values[0], lapse_rate, val))
-
-        ds_units = str(self.units.get(ds_name, None))
-        if ds_units.lower() not in valid_units:
-            msg = ('Dataset "{}" is being adjusted to elevation {} via lapse '
-                   'rate but valid units not found: {} (must be Pa or C). '
-                   'Proceeding, but if this is not the desired behavior, set '
-                   'use_lapse_rate=False'.format(ds_name, val, ds_units))
-            logger.warning(msg)
-            warnings.warn(msg, ResourceWarning)
-
-        out = super()._get_ds(ds_name, ds_slice)
-        delta_h = (interpolation_values[0] - val) / 1000  # to kilometers
-        lapse = delta_h * lapse_rate
-        return out + lapse
-
-    def _get_calculated_ds(self, val, ds_name, var_name, ds_slice):
-        """Get interpolated/extrapolated values for the dataset. """
-        vals = self._interpolation_variable[var_name]
-        (v1, v2), extrapolate = self._get_nearest_val(val, vals)
-
-        if extrapolate:
-            msg = ('Extrapolating {} using linear extrapolation'
-                   .format(ds_name))
-            warnings.warn(msg, ExtrapolationWarning)
-
-        dset_name_1 = '{}_{}{}'.format(var_name, v1, self.VARIABLE_UNIT)
-        ts1 = super()._get_ds(dset_name_1, ds_slice)
-        dset_name_2 = '{}_{}{}'.format(var_name, v2, self.VARIABLE_UNIT)
-        ts2 = super()._get_ds(dset_name_2, ds_slice)
-
-        out = linear_interp(ts1, v1, ts2, v2, val)
-        return out
-
-    @staticmethod
-    def _set_sam_res(res, values, dsets, SAM_res, time_slice, sites):
-        """
-        Set the resource for individual sites at various values
-        (i.e. hub-heights, depths, etc).
-
-        Parameters
-        ----------
-        res : rex.Resource
-            rex Resource handler or similar (NSRDB, WindResource,
-            MultiFileResource, etc...)
-        values : list | int
-            List of interpolation values e.g. hub heights or geothermal depths
-        dsets : list
-            List of dataset names to set
-        SAM_res : SAMResource
-            SAMResource object to load resource data into
-        time_slice : slice
-            Slice object representing any temporal subsampling
-        sites : list | slice
-            Spatial indices to load.
-        """
-
-        if isinstance(values, (int, float)):
-            SAM_res.load_rex_resource(res, dsets, time_slice, sites,
-                                      hh=values, hh_unit=res.VARIABLE_UNIT)
-
-        else:
-            _, unique_index = np.unique(values, return_inverse=True)
-            unique_values = sorted(list(set(values)))
-            for dset in dsets:
-                for index, value in enumerate(unique_values):
-                    pos = np.where(unique_index == index)[0]
-                    sites = np.array(SAM_res.sites)[pos]
-                    ds_name = '{}_{}{}'.format(dset, value, res.VARIABLE_UNIT)
-                    SAM_res[dset, :, pos] = res[ds_name, time_slice, sites]
-
-    @property
-    @abstractmethod
-    def INTERPOLABLE_DSETS(self):
-        """
-        list: Names of the datasets allowed to be interpolated/extrapolated.
-        """
-        raise NotImplementedError
-
-    @property
-    @abstractmethod
-    def VARIABLE_NAME(self):
-        """
-        str: Name of the variable to interpolate over (e.g. "height").
-        """
-        raise NotImplementedError
-
-    @property
-    @abstractmethod
-    def VARIABLE_UNIT(self):
-        """
-        str: Abbreviation used in dataset names for the interpolation
-        variable unit  (e.g. "m").
-        """
-        raise NotImplementedError
-
-
-class SolarResource(AbstractInterpolatedResource):
-    """
-    Class to handle Solar BaseResource .h5 files
-
-    See Also
-    --------
-    resource.BaseResource : Parent class
-    """
-
-    INTERPOLABLE_DSETS = ["temperature", "windspeed"]
-    VARIABLE_NAME = "height"
-    VARIABLE_UNIT = "m"
-
-    def get_SAM_df(self, site, extra_cols=None):
-        """
-        Get SAM solar resource DataFrame for given site
-
-        Parameters
-        ----------
-        site : int
-            Site to extract SAM DataFrame for.
-        extra_cols : dict, optional
-            A dictionary where they keys are extra columns
-            to extract from the SAM solar resource DataFrame
-            and the values are the names the new columns should
-            have (e.g. extra_cols={'surface_albedo': 'Surface
-            Albedo'} will extract the 'surface_albedo' from the
-            resource file and call it 'Surface Albedo' in the output).
-
-        Returns
-        -------
-        res_df : pandas.DataFrame
-            time-series DataFrame of resource variables needed to run SAM
-        """
-        if not self._unscale:
-            raise ResourceValueError("SAM requires unscaled values")
-
-        res_df = pd.DataFrame({'Year': self.time_index.year,
-                               'Month': self.time_index.month,
-                               'Day': self.time_index.day,
-                               'Hour': self.time_index.hour})
-
-        if len(self) > 8784 or (self.time_index.minute != 0).any():
-            res_df['Minute'] = self.time_index.minute
-
-        time_zone = self.meta.loc[site, 'timezone']
-        time_interval = len(self.time_index) // 8760
-
-        main_cols = ['dni', 'dhi', 'wind_speed', 'air_temperature']
-        extra_cols = extra_cols or {}
-        for var in main_cols + list(extra_cols):
+        for var in ['dni', 'dhi', 'wind_speed', 'air_temperature']:
             ds_slice = (slice(None), site)
             var_array = self._get_ds(var, ds_slice)
             var_array = SAMResource.roll_timeseries(var_array, time_zone,
                                                     time_interval)
             res_df[var] = SAMResource.check_units(var, var_array,
-                                                  tech='pvwattsv8')
+                                                  tech='pvwattsv7')
 
         col_map = {'dni': 'DNI', 'dhi': 'DHI', 'wind_speed': 'Wind Speed',
                    'air_temperature': 'Temperature'}
-        col_map.update(extra_cols)
         res_df = res_df.rename(columns=col_map)
-        res_df.name = "SAM_-{}".format(site)
+        res_df.name = "{}-{}".format(ds_name, site)
 
         return res_df
 
-    @staticmethod
-    def _preload_SAM(res, sites, tech='pvwattsv8', time_index_step=None,
-                     means=False, clearsky=False, bifacial=False):
+    def _preload_SAM(self, sites, tech='pvwattsv7', clearsky=False,
+                     means=False):
         """
         Pre-load project_points for SAM
 
         Parameters
         ----------
-        res : rex.Resource
-            rex Resource handler or similar (NSRDB, WindResource,
-            MultiFileResource, etc...)
         sites : list
             List of sites to be provided to SAM
         tech : str, optional
-            SAM technology string, by default 'pvwattsv8'
-        time_index_step: int, optional
-            Step size for time_index, used to reduce temporal resolution,
-            by default None
-        means : bool, optional
-            Boolean flag to compute mean resource when res_array is set,
-            by default False
+            SAM technology string, by default 'pvwattsv7'
         clearsky : bool
             Boolean flag to pull clearsky instead of real irradiance
-        bifacial : bool
-            Boolean flag to pull surface albedo for bifacial modeling.
+        means : bool
+            Boolean flag to compute mean resource when res_array is set
 
         Returns
         -------
         SAM_res : SAMResource
             Instance of SAMResource pre-loaded with Solar resource for sites
             in project_points
         """
-        time_slice = slice(None, None, time_index_step)
-        SAM_res = SAMResource(sites, tech, res['time_index', time_slice],
-                              means=means)
+        SAM_res = SAMResource(sites, tech, self.time_index, means=means)
         sites = SAM_res.sites_slice
-        SAM_res['meta'] = res['meta', sites]
-
+        SAM_res['meta'] = self['meta', sites]
         if clearsky:
             SAM_res.set_clearsky()
 
-        if bifacial and 'surface_albedo' not in SAM_res.var_list:
-            SAM_res._var_list.append('surface_albedo')
+        SAM_res.check_irradiance_datasets(self.datasets, clearsky=clearsky)
+        for var in SAM_res.var_list:
+            if var in self.datasets:
+                SAM_res[var] = self[var, :, sites]
 
-        SAM_res.check_irradiance_datasets(res.datasets, clearsky=clearsky)
-        SAM_res.load_rex_resource(res, SAM_res.var_list, time_slice, sites,
-                                  hh=2)
         SAM_res.compute_irradiance(clearsky=clearsky)
 
         return SAM_res
 
     @classmethod
-    def preload_SAM(cls, h5_file, sites, unscale=True, str_decode=True,
-                    group=None, hsds=False, hsds_kwargs=None,
-                    tech='pvwattsv8', time_index_step=None, means=False,
-                    clearsky=False, bifacial=False):
+    def preload_SAM(cls, h5_file, sites, unscale=True, hsds=False,
+                    str_decode=True, group=None, tech='pvwattsv7',
+                    clearsky=False, means=False):
         """
         Pre-load project_points for SAM
 
         Parameters
         ----------
         h5_file : str
             h5_file to extract resource from
         sites : list
             List of sites to be provided to SAM
         unscale : bool
             Boolean flag to automatically unscale variables on extraction
+        hsds : bool
+            Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
+            behind HSDS
         str_decode : bool
             Boolean flag to decode the bytestring meta data into normal
             strings. Setting this to False will speed up the meta data read.
         group : str
             Group within .h5 resource file to open
-        hsds : bool, optional
-            Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
-            behind HSDS, by default False
-        hsds_kwargs : dict, optional
-            Dictionary of optional kwargs for h5pyd, e.g., bucket, username,
-            password, by default None
         tech : str, optional
-            SAM technology string, by default 'pvwattsv8'
-        time_index_step: int, optional
-            Step size for time_index, used to reduce temporal resolution,
-            by default None
-        means : bool, optional
-            Boolean flag to compute mean resource when res_array is set,
-            by default False
+            SAM technology string, by default 'pvwattsv7'
         clearsky : bool
             Boolean flag to pull clearsky instead of real irradiance
-        bifacial : bool
-            Boolean flag to pull surface albedo for bifacial modeling.
+        means : bool
+            Boolean flag to compute mean resource when res_array is set
 
         Returns
         -------
         SAM_res : SAMResource
             Instance of SAMResource pre-loaded with Solar resource for sites
             in project_points
         """
-        kwargs = {"unscale": unscale, "hsds": hsds, 'hsds_kwargs': hsds_kwargs,
+        kwargs = {"unscale": unscale, "hsds": hsds,
                   "str_decode": str_decode, "group": group}
         with cls(h5_file, **kwargs) as res:
-            SAM_res = res._preload_SAM(res, sites, tech=tech,
-                                       time_index_step=time_index_step,
-                                       means=means, clearsky=clearsky,
-                                       bifacial=bifacial)
+            SAM_res = res._preload_SAM(sites, tech=tech, clearsky=clearsky,
+                                       means=means)
 
         return SAM_res
 
 
 class NSRDB(SolarResource):
     """
     Class to handle NSRDB .h5 files
 
     See Also
     --------
-    resource.BaseResource : Parent class
+    resource.Resource : Parent class
     """
-    ADD_ATTR = ['add_offset', 'psm_add_offset']
-    SCALE_ATTR = ['scale_factor', 'psm_scale_factor']
-    UNIT_ATTR = ['units', 'psm_units']
+    ADD_ATTR = 'psm_add_offset'
+    SCALE_ATTR = 'psm_scale_factor'
+    UNIT_ATTR = 'psm_units'
 
-    @staticmethod
-    def _preload_SAM(res, sites, tech='pvwattsv8', time_index_step=None,
-                     means=False, clearsky=False, bifacial=False,
-                     downscale=None):
+    def _preload_SAM(self, sites, tech='pvwattsv7', clearsky=False,
+                     downscale=None, means=False):
         """
         Pre-load project_points for SAM
 
         Parameters
         ----------
-        res : rex.Resource
-            rex Resource handler or similar (NSRDB, WindResource,
-            MultiFileResource, etc...)
         sites : list
             List of sites to be provided to SAM
         tech : str, optional
-            SAM technology string, by default 'pvwattsv8'
-        time_index_step: int, optional
-            Step size for time_index, used to reduce temporal resolution,
-            by default None
-        means : bool, optional
-            Boolean flag to compute mean resource when res_array is set,
-            by default False
+            SAM technology string, by default 'pvwattsv7'
         clearsky : bool
             Boolean flag to pull clearsky instead of real irradiance
-        bifacial : bool
-            Boolean flag to pull surface albedo for bifacial modeling.
-        downscale : NoneType | dict
+        downscale : NoneType | str
             Option for NSRDB resource downscaling to higher temporal
-            resolution. Expects a dict of downscaling kwargs with a minimum
-            requirement of the desired frequency e.g. 'frequency': '5min'
-            and an option to add "variability_kwargs".
+            resolution. Expects a string in the Pandas frequency format,
+            e.g. '5min'.
+        means : bool
+            Boolean flag to compute mean resource when res_array is set
 
         Returns
         -------
         SAM_res : SAMResource
             Instance of SAMResource pre-loaded with Solar resource for sites
             in project_points
         """
-        time_slice = slice(None, None, time_index_step)
-        SAM_res = SAMResource(sites, tech, res['time_index', time_slice],
-                              means=means)
+        SAM_res = SAMResource(sites, tech, self.time_index, means=means)
         sites = SAM_res.sites_slice
-        SAM_res['meta'] = res['meta', sites]
+        SAM_res['meta'] = self['meta', sites]
 
         if clearsky:
             SAM_res.set_clearsky()
 
-        if bifacial and 'surface_albedo' not in SAM_res.var_list:
-            SAM_res._var_list.append('surface_albedo')
-
-        SAM_res.check_irradiance_datasets(res.datasets, clearsky=clearsky)
+        SAM_res.check_irradiance_datasets(self.datasets, clearsky=clearsky)
         if not downscale:
-            SAM_res.load_rex_resource(res, SAM_res.var_list, time_slice,
-                                      sites, hh=2)
+            for var in SAM_res.var_list:
+                if var in self.datasets:
+                    SAM_res[var] = self[var, :, sites]
+
             SAM_res.compute_irradiance(clearsky=clearsky)
         else:
             # contingent import to avoid dependencies
             from rex.utilities.downscale import downscale_nsrdb
-            frequency = downscale.pop('frequency')
-            SAM_res = downscale_nsrdb(SAM_res, res, sam_vars=SAM_res.var_list,
-                                      frequency=frequency,
-                                      variability_kwargs=downscale)
+            SAM_res = downscale_nsrdb(SAM_res, self, downscale,
+                                      sam_vars=SAM_res.var_list)
 
         return SAM_res
 
     @classmethod
-    def preload_SAM(cls, h5_file, sites, unscale=True, str_decode=True,
-                    group=None, hsds=False, hsds_kwargs=None,
-                    tech='pvwattsv8', time_index_step=None, means=False,
-                    clearsky=False, bifacial=False, downscale=None):
+    def preload_SAM(cls, h5_file, sites, unscale=True, hsds=False,
+                    str_decode=True, group=None, tech='pvwattsv7',
+                    clearsky=False, downscale=None, means=False):
         """
         Pre-load project_points for SAM
 
         Parameters
         ----------
         h5_file : str
             h5_file to extract resource from
         sites : list
             List of sites to be provided to SAM
         unscale : bool
             Boolean flag to automatically unscale variables on extraction
+        hsds : bool
+            Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
+            behind HSDS
         str_decode : bool
             Boolean flag to decode the bytestring meta data into normal
             strings. Setting this to False will speed up the meta data read.
         group : str
             Group within .h5 resource file to open
-        hsds : bool, optional
-            Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
-            behind HSDS, by default False
-        hsds_kwargs : dict, optional
-            Dictionary of optional kwargs for h5pyd, e.g., bucket, username,
-            password, by default None
         tech : str, optional
-            SAM technology string, by default 'pvwattsv8'
-       time_index_step: int, optional
-            Step size for time_index, used to reduce temporal resolution,
-            by default None
-        means : bool, optional
-            Boolean flag to compute mean resource when res_array is set,
-            by default False
+            SAM technology string, by default 'pvwattsv7'
         clearsky : bool
             Boolean flag to pull clearsky instead of real irradiance
-        bifacial : bool
-            Boolean flag to pull surface albedo for bifacial modeling.
-        downscale : NoneType | dict
+        downscale : NoneType | str
             Option for NSRDB resource downscaling to higher temporal
-            resolution. Expects a dict of downscaling kwargs with a minimum
-            requirement of the desired frequency e.g. 'frequency': '5min'
-            and an option to add "variability_kwargs".
+            resolution. Expects a string in the Pandas frequency format,
+            e.g. '5min'.
+        means : bool
+            Boolean flag to compute mean resource when res_array is set
 
         Returns
         -------
         SAM_res : SAMResource
             Instance of SAMResource pre-loaded with Solar resource for sites
             in project_points
         """
-        kwargs = {"unscale": unscale, "hsds": hsds, 'hsds_kwargs': hsds_kwargs,
+        kwargs = {"unscale": unscale, "hsds": hsds,
                   "str_decode": str_decode, "group": group}
         with cls(h5_file, **kwargs) as res:
-            SAM_res = res._preload_SAM(res, sites, tech=tech,
-                                       time_index_step=time_index_step,
-                                       means=means, clearsky=clearsky,
-                                       bifacial=bifacial, downscale=downscale)
+            SAM_res = res._preload_SAM(sites, tech=tech, clearsky=clearsky,
+                                       downscale=downscale, means=means)
 
         return SAM_res
 
 
-class WindResource(AbstractInterpolatedResource):
+class WindResource(Resource):
     """
-    Class to handle Wind BaseResource .h5 files
+    Class to handle Wind Resource .h5 files
 
     See Also
     --------
-    resource.AbstractInterpolatedResource : Parent class
+    resource.Resource : Parent class
 
     Examples
     --------
-    >>> import os
-    >>> from rex import TESTDATADIR, WindResource
-    >>> file = os.path.join(TESTDATADIR, 'wtk/ri_100_wtk_2012.h5')
+    >>> file = '$TESTDATADIR/wtk/ri_100_wtk_2012.h5'
     >>> with WindResource(file) as res:
     >>>     print(res.datasets)
     ['meta', 'pressure_0m', 'pressure_100m', 'pressure_200m',
     'temperature_100m', 'temperature_80m', 'time_index', 'winddirection_100m',
     'winddirection_80m', 'windspeed_100m', 'windspeed_80m']
 
     WindResource can interpolate between available hub-heights (80 & 100)
@@ -936,37 +300,160 @@
      [10.5515785  9.804363   9.770399  ...  8.026898   8.468434   8.67222  ]
      ...
      [ 9.079792   9.170363   9.634542  ... 13.472508  13.7102585 14.004617 ]
      [10.710078  10.710078  10.698757  ... 14.468795  14.514081  14.6386175]
      [10.698757  10.857258  11.174257  ... 16.585903  16.676476  16.653833 ]]
     """
 
-    INTERPOLABLE_DSETS = ["temperature", "pressure", "windspeed",
-                          "winddirection"]
-    VARIABLE_NAME = "height"
-    VARIABLE_UNIT = "m"
-
-    def __getitem__(self, keys):
-        ds, ds_slice = parse_keys(keys)
-        _, ds_name = os.path.split(ds)
-        if 'SAM' in ds_name:
-            site = ds_slice[0]
-            if isinstance(site, (int, np.integer)):
-                _, height = self._parse_name(ds_name)
-                out = self.get_SAM_df(site, height)
+    def __init__(self, h5_file, unscale=True, hsds=False, str_decode=True,
+                 group=None):
+        """
+        Parameters
+        ----------
+        h5_file : str
+            Path to .h5 resource file
+        unscale : bool
+            Boolean flag to automatically unscale variables on extraction
+        hsds : bool
+            Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
+            behind HSDS
+        str_decode : bool
+            Boolean flag to decode the bytestring meta data into normal
+            strings. Setting this to False will speed up the meta data read.
+        group : str
+            Group within .h5 resource file to open
+        """
+        self._heights = None
+        super().__init__(h5_file, unscale=unscale, hsds=hsds,
+                         str_decode=str_decode, group=group)
+
+    @staticmethod
+    def _parse_hub_height(name):
+        """
+        Extract hub height from given string
+
+        Parameters
+        ----------
+        name : str
+            String to parse hub height from
+
+        Returns
+        -------
+        h : int | float
+            Hub Height as a numeric value
+        """
+        h = name.strip('m')
+        try:
+            h = int(h)
+        except ValueError:
+            h = float(h)
+
+        return h
+
+    @staticmethod
+    def _parse_name(ds_name):
+        """
+        Extract dataset name and height from dataset name
+
+        Parameters
+        ----------
+        ds_name : str
+            Dataset name
+
+        Returns
+        -------
+        name : str
+            Variable name
+        h : int | float
+            Height of variable
+        """
+        try:
+            if ds_name.endswith('m'):
+                name, h = ds_name.split('_')
+                h = WindResource._parse_hub_height(h)
             else:
-                msg = "Can only extract SAM DataFrame for a single site"
-                raise ResourceRuntimeError(msg)
-        else:
-            out = super().__getitem__(keys)
+                raise ValueError('{} does not end with "_hm"'
+                                 .format(ds_name))
+        except Exception as ex:
+            name = ds_name
+            h = None
+            msg = ('Could not extract hub-height from {}:\n{}'
+                   .format(ds_name, ex))
+            warnings.warn(msg)
 
-        return out
+        return name, h
 
-    @classmethod
-    def monin_obukhov_extrapolation(cls, ts_1, h_1, z0, L, h):
+    @property
+    def heights(self):
+        """
+        Extract available heights for pressure, temperature, windspeed, precip,
+        and winddirection variables. Used for interpolation/extrapolation.
+
+        Returns
+        -------
+        self._heights : list
+            List of available heights for:
+            windspeed, winddirection, temperature, and pressure
+        """
+        if self._heights is None:
+            heights = {'pressure': [],
+                       'temperature': [],
+                       'windspeed': [],
+                       'winddirection': []}
+
+            ignore = ['meta', 'time_index', 'coordinates']
+            for ds in self.datasets:
+                if ds not in ignore:
+                    ds_name, h = self._parse_name(ds)
+                    if ds_name in heights.keys():
+                        heights[ds_name].append(h)
+
+            self._heights = heights
+
+        return self._heights
+
+    @staticmethod
+    def get_nearest_h(h, heights):
+        """
+        Get two nearest h values in heights.
+        Determine if h is inside or outside the range of heights
+        (requiring extrapolation instead of interpolation)
+
+        Parameters
+        ----------
+        h : int | float
+            Height value of interest
+        heights : list
+            List of available heights
+
+        Returns
+        -------
+        nearest_h : list
+            list of 1st and 2nd nearest height in heights
+        extrapolate : bool
+            Flag as to whether h is inside or outside heights range
+        """
+
+        heights_arr = np.array(heights, dtype='float32')
+        dist = np.abs(heights_arr - h)
+        pos = dist.argsort()[:2]
+        nearest_h = sorted([heights[p] for p in pos])
+        extrapolate = np.all(h < heights_arr) or np.all(h > heights_arr)
+
+        if extrapolate:
+            h_min, h_max = np.sort(heights)[[0, -1]]
+            msg = ('{} is outside the height range'.format(h),
+                   '({}, {}).'.format(h_min, h_max),
+                   'Extrapolation to be used.')
+            warnings.warn(' '.join(msg), ExtrapolationWarning)
+
+        return nearest_h, extrapolate
+
+    @staticmethod
+    def monin_obukhov_extrapolation(ts_1, h_1, z0, L, h):
         """
         Monin-Obukhov extrapolation
 
         Parameters
         ----------
          ts_1 : ndarray
             Time-series array at height h_1
@@ -981,19 +468,19 @@
 
         Returns
         -------
         ndarray
             new wind speed from MO extrapolation.
         """
         # Non dimensional stability parameter at h
-        zeta = cls.stability_function(h / L)
+        zeta = WindResource.stability_function(h / L)
         # Non dimensional stability parameter at z0
-        zeta_0 = cls.stability_function(z0 / L)
+        zeta_0 = WindResource.stability_function(z0 / L)
         # Non dimensional stability parameter at h_1
-        zeta_1 = cls.stability_function(h_1 / L)
+        zeta_1 = WindResource.stability_function(h_1 / L)
 
         # Logarithmic extrapolation equation
         out = (ts_1 * (np.log(h / z0) - zeta + zeta_0)
                / (np.log(h_1 / z0) - zeta_1 + zeta_0))
 
         return out
 
@@ -1090,14 +577,50 @@
             alpha[alpha > 0.6] = 0.6
 
         out = ts_1 * (h / h_1)**alpha
 
         return out
 
     @staticmethod
+    def linear_interp(ts_1, h_1, ts_2, h_2, h):
+        """
+        Linear interpolate/extrapolate time-series data to height h
+
+        Parameters
+        ----------
+        ts_1 : ndarray
+            Time-series array at height h_1
+        h_1 : int | float
+            Height corresponding to time-seris ts_1
+        ts_2 : ndarray
+            Time-series array at height h_2
+        h_2 : int | float
+            Height corresponding to time-seris ts_2
+        h : int | float
+            Height of desired time-series
+
+        Returns
+        -------
+        out : ndarray
+            Time-series array at height h
+        """
+        if h_1 > h_2:
+            h_1, h_2 = h_2, h_1
+            ts_1, ts_2 = ts_2, ts_1
+
+        # Calculate slope for every posiiton in variable arrays
+        m = (ts_2 - ts_1) / (h_2 - h_1)
+        # Calculate intercept for every position in variable arrays
+        b = ts_2 - m * h_2
+
+        out = m * h + b
+
+        return out
+
+    @staticmethod
     def shortest_angle(a0, a1):
         """
         Calculate the shortest angle distance between a0 and a1
 
         Parameters
         ----------
         a0 : int | float
@@ -1109,16 +632,16 @@
         -------
         da : int | float
             shortest angle distance between a0 and a1
         """
         da = (a1 - a0) % 360
         return 2 * da % 360 - da
 
-    @classmethod
-    def circular_interp(cls, ts_1, h_1, ts_2, h_2, h):
+    @staticmethod
+    def circular_interp(ts_1, h_1, ts_2, h_2, h):
         """
         Circular interpolate/extrapolate time-series data to height h
 
         Parameters
         ----------
         ts_1 : ndarray
             Time-series array at height h_1
@@ -1134,169 +657,182 @@
         Returns
         -------
         out : ndarray
             Time-series array at height h
         """
         h_f = (h - h_1) / (h_2 - h_1)
 
-        da = cls.shortest_angle(ts_1, ts_2) * h_f
+        da = WindResource.shortest_angle(ts_1, ts_2) * h_f
         da = np.sign(da) * (np.abs(da) % 360)
 
         out = (ts_2 + da) % 360
 
         return out
 
-    @staticmethod
-    def _check_hub_height(heights, h):
+    def _check_hub_height(self, h):
         """
         Check requested hub-height against available windspeed hub-heights
         If only one hub-height is available change request to match available
         hub-height
 
         Parameters
         ----------
-        heights : dict
-            Dictionary of available interpolation variable values for
-            the interpolable datasets. For example, this could be:
-            {'windspeed': [10, 100, 200]}
         h : int | float
             Requested hub-height
 
         Returns
         -------
         h : int | float
             Hub-height to extract
         """
-        heights = heights['windspeed']
+        heights = self.heights['windspeed']
         if len(heights) == 1:
             h = heights[0]
             warnings.warn('Wind speed is only available at {h}m, '
                           'all variables will be extracted at {h}m'
                           .format(h=h), ResourceWarning)
 
         return h
 
     def _try_monin_obukhov_extrapolation(self, ts_1, ds_slice, h_1, h):
         rmol = 'inversemoninobukhovlength_2m'
         if rmol not in self:
             msg = ("{} is needed to run monin obukhov extrapolation"
                    .format(rmol))
+            warnings.warn(msg)
             raise MoninObukhovExtrapolationError(msg)
 
         if 'roughness_length' in self:
             z0 = self._get_ds('roughness_length', ds_slice)
         elif 'z0' in self.meta:
             z0 = self.meta['z0']
         else:
             msg = ("roughness length ('z0') is needed to run monin obukhov"
                    "extrapolation")
+            warnings.warn(msg, ExtrapolationWarning)
             raise MoninObukhovExtrapolationError(msg)
 
         L = 1 / self._get_ds(rmol, ds_slice)
 
         out = self.monin_obukhov_extrapolation(ts_1, h_1, z0, L, h)
 
         return out
 
-    def _get_ds_interpolated(self, ds_name, ds_slice):
-        """Extract data from given dataset at desired interpolation value.
-
-        Data is interpolated or extrapolated as needed.
+    def _get_ds_height(self, ds_name, ds_slice):
+        """
+        Extract data from given dataset at desired height, interpolate or
+        extrapolate if neede
 
         Parameters
         ----------
         ds_name : str
             Variable dataset to be extracted
-        ds_slice : tuple
-            Tuple of (int, slice, list, ndarray) of what to extract
-            from ds, each arg is for a sequential axis
+        ds_slice : tuple of int | list | slice
+            tuple describing list ds_slice to extract
 
         Returns
         -------
         out : ndarray
             ndarray of variable timeseries data
             If unscale, returned in native units else in scaled units
         """
-        var_name, __ = self._parse_name(ds_name)
+        var_name, h = self._parse_name(ds_name)
         heights = self.heights[var_name]
+        if len(heights) == 1:
+            h = heights[0]
+            ds_name = '{}_{}m'.format(var_name, h)
+            warnings.warn('Only one hub-height available, returning {}'
+                          .format(ds_name), ResourceWarning)
+
+        if h in heights:
+            ds_name = '{}_{}m'.format(var_name, int(h))
+            out = super()._get_ds(ds_name, ds_slice)
+        else:
+            (h1, h2), extrapolate = self.get_nearest_h(h, heights)
+            if extrapolate:
+                warnings.warn('Extrapolating {}'.format(ds_name),
+                              ExtrapolationWarning)
+
+            ts1 = super()._get_ds('{}_{}m'.format(var_name, h1), ds_slice)
+            ts2 = super()._get_ds('{}_{}m'.format(var_name, h2), ds_slice)
+
+            if (var_name == 'windspeed') and extrapolate:
+                if h < h1:
+                    try:
+                        self._try_monin_obukhov_extrapolation(ts1, ds_slice,
+                                                              h1, h)
+                        warnings.warn('\t- Using Monin Obukhov '
+                                      'Extrapolation',
+                                      ExtrapolationWarning)
+                    except MoninObukhovExtrapolationError:
+                        out = self.power_law_interp(ts1, h1, ts2, h2, h)
+                        warnings.warn('\t- Using Power Law Extrapolation',
+                                      ExtrapolationWarning)
+                else:
+                    out = self.power_law_interp(ts1, h1, ts2, h2, h)
+                    warnings.warn('\t- Using Power Law Extrapolation',
+                                  ExtrapolationWarning)
+            elif var_name == 'winddirection':
+                out = self.circular_interp(ts1, h1, ts2, h2, h)
+            else:
+                out = self.linear_interp(ts1, h1, ts2, h2, h)
 
-        if not heights:
-            msg = ("Missing height info for dataset '{}' in {}"
-                   .format(var_name, self.h5_file))
-            logger.error(msg)
-            raise ResourceKeyError(msg)
-
-        return super()._get_ds_interpolated(ds_name, ds_slice)
-
-    def _get_calculated_ds(self, val, ds_name, var_name, ds_slice):
-        """Get interpolated/extrapolated values for the dataset. """
-        heights = self._interpolation_variable[var_name]
-        (h1, h2), extrapolate = self._get_nearest_val(val, heights)
+        return out
 
-        if extrapolate:
-            msg = 'Extrapolating {}'.format(ds_name)
+    def _get_ds(self, ds_name, ds_slice):
+        """
+        Extract data from given dataset
 
-        dset_name_1 = '{}_{}{}'.format(var_name, h1, self.VARIABLE_UNIT)
-        ts1 = super()._get_ds(dset_name_1, ds_slice)
-        dset_name_2 = '{}_{}{}'.format(var_name, h2, self.VARIABLE_UNIT)
-        ts2 = super()._get_ds(dset_name_2, ds_slice)
-
-        if (var_name == 'windspeed') and extrapolate:
-            if val < h1:
-                try:
-                    out = self._try_monin_obukhov_extrapolation(ts1,
-                                                                ds_slice,
-                                                                h1, val)
-                    msg += ' using Monin Obukhov Extrapolation'
-                    warnings.warn(msg, ExtrapolationWarning)
-                except MoninObukhovExtrapolationError:
-                    out = self.power_law_interp(ts1, h1, ts2, h2, val)
-                    msg += ' using Power Law Extrapolation'
-                    warnings.warn(msg, ExtrapolationWarning)
-            else:
-                out = self.power_law_interp(ts1, h1, ts2, h2, val)
-                msg += ' using Power Law Extrapolation'
-                warnings.warn(msg, ExtrapolationWarning)
-        elif var_name == 'winddirection':
-            out = self.circular_interp(ts1, h1, ts2, h2, val)
+        Parameters
+        ----------
+        ds_name : str
+            Variable dataset to be extracted
+        ds_slice : tuple of int | list | slice
+            tuple describing list ds_slice to extract
+
+        Returns
+        -------
+        out : ndarray
+            ndarray of variable timeseries data
+            If unscale, returned in native units else in scaled units
+        """
+        var_name, h = self._parse_name(ds_name)
+        if h is not None and var_name in self.heights:
+            out = self._get_ds_height(ds_name, ds_slice)
         else:
-            out = linear_interp(ts1, h1, ts2, h2, val)
+            out = super()._get_ds(ds_name, ds_slice)
+
         return out
 
-    def get_SAM_df(self, site, height, require_wind_dir=False, icing=False,
-                   add_header=False):
+    def _get_SAM_df(self, ds_name, site, require_wind_dir=False,
+                    icing=False):
         """
         Get SAM wind resource DataFrame for given site
 
         Parameters
         ----------
+        ds_name : str
+            'Dataset' name == SAM
         site : int
             Site to extract SAM DataFrame for
-        height : int
-            Hub height to extract SAM variables at
-        require_wind_dir : bool, optional
-            Boolean flag as to whether wind direction will be loaded,
-            by default False
-        icing : bool, optional
-            Boolean flag to include relativehumitidy for icing calculation,
-            by default False
-        add_header : bool, optional
-            Add units and hub_height below variable names, needed for SAM .csv,
-            by default False
+        require_wind_dir : bool
+            Boolean flag as to whether wind direction will be loaded.
+        icing : bool
+            Boolean flag to include relativehumitidy for icing calculation
 
         Returns
         -------
         res_df : pandas.DataFrame
             time-series DataFrame of resource variables needed to run SAM
         """
         if not self._unscale:
             raise ResourceValueError("SAM requires unscaled values")
 
-        height = self._check_hub_height(self.heights, height)
-        units = ['year', 'month', 'day', 'hour']
+        _, h = self._parse_name(ds_name)
+        h = self._check_hub_height(h)
         res_df = pd.DataFrame({'Year': self.time_index.year,
                                'Month': self.time_index.month,
                                'Day': self.time_index.day,
                                'Hour': self.time_index.hour})
         if len(self) > 8784:
             res_df['Minute'] = self.time_index.minute
 
@@ -1304,337 +840,431 @@
         time_interval = len(self.time_index) // 8760
 
         variables = ['pressure', 'temperature', 'winddirection', 'windspeed']
         if not require_wind_dir:
             variables.remove('winddirection')
 
         if icing:
-            variables.append('relativehumidity_2m')
+            variables.append('relativehumidity')
 
         for var in variables:
-            var_name = "{}_{}m".format(var, height)
+            var_name = "{}_{}m".format(var, h)
             ds_slice = (slice(None), site)
             var_array = self._get_ds(var_name, ds_slice)
             var_array = SAMResource.roll_timeseries(var_array, time_zone,
                                                     time_interval)
             res_df[var] = SAMResource.check_units(var, var_array,
                                                   tech='windpower')
             res_df[var] = SAMResource.enforce_arr_range(
                 var, res_df[var],
                 SAMResource.WIND_DATA_RANGES[var], [site])
 
         col_map = {'pressure': 'Pressure', 'temperature': 'Temperature',
                    'windspeed': 'Speed', 'winddirection': 'Direction',
-                   'relativehumidity_2m': 'Relative Humidity'}
+                   'relativehumidity': 'Relative Humidity'}
         res_df = res_df.rename(columns=col_map)
-        res_df.name = "SAM_{}m-{}".format(height, site)
-
-        if add_header:
-            header = pd.DataFrame(columns=res_df.columns)
-            header_units = units + [self.get_units(v) for v in variables]
-            header_heights = [height] * len(header_units)
-            header = pd.DataFrame([header_units, header_heights],
-                                  columns=res_df.columns)
-            res_df = pd.concat((header, res_df)).reset_index(drop=True)
+        res_df.name = "{}-{}".format(ds_name, site)
 
         return res_df
 
-    @staticmethod
-    def _preload_SAM(res, sites, hub_heights, time_index_step=None,
-                     means=False, require_wind_dir=False,
-                     precip_rate=False, icing=False):
+    def _preload_SAM(self, sites, hub_heights, require_wind_dir=False,
+                     precip_rate=False, icing=False, means=False):
         """
         Pre-load project_points for SAM
 
         Parameters
         ----------
-        res : rex.Resource
-            rex Resource handler or similar (NSRDB, WindResource,
-            MultiFileResource, etc...)
         sites : list
             List of sites to be provided to SAM
         hub_heights : int | float | list
             Hub heights to extract for SAM
-        time_index_step: int, optional
-            Step size for time_index, used to reduce temporal resolution,
-            by default None
-        means : bool, optional
-            Boolean flag to compute mean resource when res_array is set,
-            by default False
-        require_wind_dir : bool, optional
-            Boolean flag as to whether wind direction will be loaded,
-            by default False
-        precip_rate : bool, optional
-            Boolean flag as to whether precipitationrate_0m will be preloaded,
-            by default False
-        icing : bool, optional
+        require_wind_dir : bool
+            Boolean flag as to whether wind direction will be loaded.
+        precip_rate : bool
+            Boolean flag as to whether precipitationrate_0m will be preloaded
+        icing : bool
             Boolean flag as to whether icing is analyzed.
-            This will preload relative humidity, by default False
+            This will preload relative humidity.
+        means : bool
+            Boolean flag to compute mean resource when res_array is set
 
         Returns
         -------
         SAM_res : SAMResource
             Instance of SAMResource pre-loaded with Solar resource for sites
             in project_points
         """
-
-        time_slice = slice(None, None, time_index_step)
-        SAM_res = SAMResource(sites, 'windpower',
-                              res['time_index', time_slice],
+        SAM_res = SAMResource(sites, 'windpower', self.time_index,
                               hub_heights=hub_heights,
                               require_wind_dir=require_wind_dir,
                               means=means)
-
         sites = SAM_res.sites_slice
-        SAM_res['meta'] = res['meta', sites]
+        SAM_res['meta'] = self['meta', sites]
         var_list = SAM_res.var_list
         if not require_wind_dir:
             var_list.remove('winddirection')
 
-        h = res._check_hub_height(res.heights, SAM_res.h)
-        res._set_sam_res(res, h, var_list, SAM_res, time_slice, sites)
+        h = self._check_hub_height(SAM_res.h)
+        if isinstance(h, (int, float)):
+            for var in var_list:
+                ds_name = "{}_{}m".format(var, h)
+                SAM_res[var] = self[ds_name, :, sites]
+        else:
+            _, unq_idx = np.unique(h, return_inverse=True)
+            unq_h = sorted(list(set(h)))
+
+            site_list = np.array(SAM_res.sites)
+            height_slices = {}
+            for i, h_i in enumerate(unq_h):
+                pos = np.where(unq_idx == i)[0]
+                height_slices[h_i] = (site_list[pos], pos)
+
+            for var in var_list:
+                for h_i, (h_pos, sam_pos) in height_slices.items():
+                    ds_name = '{}_{}m'.format(var, h_i)
+                    SAM_res[var, :, sam_pos] = self[ds_name, :, h_pos]
 
         if precip_rate:
             var = 'precipitationrate'
             ds_name = '{}_0m'.format(var)
             SAM_res.append_var_list(var)
-            SAM_res[var] = res[ds_name, time_slice, sites]
+            SAM_res[var] = self[ds_name, :, sites]
 
         if icing:
             var = 'rh'
             ds_name = 'relativehumidity_2m'
             SAM_res.append_var_list(var)
-            SAM_res[var] = res[ds_name, time_slice, sites]
+            SAM_res[var] = self[ds_name, :, sites]
 
         return SAM_res
 
     @classmethod
     def preload_SAM(cls, h5_file, sites, hub_heights, unscale=True,
-                    str_decode=True, group=None, hsds=False, hsds_kwargs=None,
-                    time_index_step=None, means=False,
-                    require_wind_dir=False, precip_rate=False, icing=False):
+                    hsds=False, str_decode=True, group=None,
+                    require_wind_dir=False, precip_rate=False, icing=False,
+                    means=False):
         """
         Placeholder for classmethod that will pre-load project_points for SAM
 
         Parameters
         ----------
         h5_file : str
             h5_file to extract resource from
         sites : list
             List of sites to be provided to SAM
         hub_heights : int | float | list
             Hub heights to extract for SAM
         unscale : bool
             Boolean flag to automatically unscale variables on extraction
+        hsds : bool
+            Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
+            behind HSDS
         str_decode : bool
             Boolean flag to decode the bytestring meta data into normal
             strings. Setting this to False will speed up the meta data read.
         group : str
             Group within .h5 resource file to open
-        hsds : bool, optional
-            Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
-            behind HSDS, by default False
-        hsds_kwargs : dict, optional
-            Dictionary of optional kwargs for h5pyd, e.g., bucket, username,
-            password, by default None
-        time_index_step: int, optional
-            Step size for time_index, used to reduce temporal resolution,
-            by default None
-        means : bool, optional
-            Boolean flag to compute mean resource when res_array is set,
-            by default False
-        require_wind_dir : bool, optional
-            Boolean flag as to whether wind direction will be loaded,
-            by default False
-        precip_rate : bool, optional
-            Boolean flag as to whether precipitationrate_0m will be preloaded,
-            by default False
-        icing : bool, optional
+        require_wind_dir : bool
+            Boolean flag as to whether wind direction will be loaded.
+        precip_rate : bool
+            Boolean flag as to whether precipitationrate_0m will be preloaded
+        icing : bool
             Boolean flag as to whether icing is analyzed.
-            This will preload relative humidity, by default False
+            This will preload relative humidity.
+        means : bool
+            Boolean flag to compute mean resource when res_array is set
 
         Returns
         -------
         SAM_res : SAMResource
             Instance of SAMResource pre-loaded with Solar resource for sites
             in project_points
         """
-        kwargs = {"unscale": unscale, "hsds": hsds, 'hsds_kwargs': hsds_kwargs,
+        kwargs = {"unscale": unscale, "hsds": hsds,
                   "str_decode": str_decode, "group": group}
         with cls(h5_file, **kwargs) as res:
-            SAM_res = res._preload_SAM(res, sites, hub_heights,
+            SAM_res = res._preload_SAM(sites, hub_heights,
                                        require_wind_dir=require_wind_dir,
                                        precip_rate=precip_rate, icing=icing,
-                                       means=means,
-                                       time_index_step=time_index_step)
+                                       means=means)
 
         return SAM_res
 
 
-class GeothermalResource(AbstractInterpolatedResource):
+class WaveResource(Resource):
     """
-    Class to handle Geothermal Resource .h5 files
+    Class to handle Wave Resource .h5 files
 
     See Also
     --------
-    resource.AbstractInterpolatedResource : Parent class
+    resource.Resource : Parent class
+    """
 
-    Examples
-    --------
-    >>> file = '$TESTDATADIR/geo/template_geo_data.h5'
-    >>> with GeothermalResource(file) as res:
-    >>>     print(res.datasets)
-    ['meta', 'temperature_3500m', 'temperature_4500m']
+    def _get_SAM_df(self, ds_name, site):
+        """
+        Get SAM wave resource DataFrame for given site
 
-    GeothermalResource can linearly interpolate between available depths
-    (3.5km & 4.5km).
+        Parameters
+        ----------
+        ds_name : str
+            'Dataset' name == SAM
+        site : int
+            Site to extract SAM DataFrame for
 
-    >>> with GeothermalResource(file) as res:
-    >>>     temp_4km = res['temperature_4000m']
-    >>>
-    >>> temp_4km
-    [450.5, 434. , 383.5, 422. , 387. , 316.5, 438. , 419. , 424. ,
-     438.5]
+        Returns
+        -------
+        res_df : pandas.DataFrame
+            time-series DataFrame of resource variables needed to run SAM
+        """
+        if not self._unscale:
+            raise ResourceValueError("SAM requires unscaled values")
 
-    GeothermalResource can also linearly extrapolate beyond available depths
+        res_df = pd.DataFrame({'Year': self.time_index.year,
+                               'Month': self.time_index.month,
+                               'Day': self.time_index.day,
+                               'Hour': self.time_index.hour})
+        if len(self) > 8784:
+            res_df['Minute'] = self.time_index.minute
 
-    >>> with GeothermalResource(file) as res:
-    >>>     temp_5km = res['temperature_5000m']
-    >>>
-    >>> temp_5km
-    ExtrapolationWarning: 5000 is outside the depth range (3500, 4500).
-    Extrapolation to be used.
-    [501.5, 338. , 428.5, 548. , 405. , 301.5, 440. , 565. , 446. ,
-     341.5]
-    """
+        time_zone = self.meta.loc[site, 'timezone']
+        time_interval = len(self.time_index) // 8760
 
-    LAPSE_RATES = {}
-    INTERPOLABLE_DSETS = ["temperature", "potential_MW"]
-    VARIABLE_NAME = "depth"
-    VARIABLE_UNIT = "m"
+        for var in ['significant_wave_height', 'peak_period']:
+            ds_slice = (slice(None), site)
+            var_array = self._get_ds(var, ds_slice)
+            var_array = SAMResource.roll_timeseries(var_array, time_zone,
+                                                    time_interval)
+            res_df[var] = SAMResource.check_units(var, var_array,
+                                                  tech='pvwattsv7')
 
-    @staticmethod
-    def _preload_SAM(res, sites, depths, time_index_step=None,
-                     means=False):
+        col_map = {'significant_wave_height': 'Hs', 'peak_period': 'Tp'}
+        res_df = res_df.rename(columns=col_map)
+        res_df.name = "{}-{}".format(ds_name, site)
+
+        return res_df
+
+    def _preload_SAM(self, sites, means=False):
         """
         Pre-load project_points for SAM
 
         Parameters
         ----------
-        res : rex.Resource
-            rex Resource handler or similar (NSRDB, WindResource,
-            MultiFileResource, etc...)
         sites : list
             List of sites to be provided to SAM
-        depths :  int | float | list
-            Depths to extract for SAM
-        time_index_step: int, optional
-            Step size for time_index, used to reduce temporal resolution,
-            by default None
-        means : bool, optional
-            Boolean flag to compute mean resource when res_array is set,
-            by default False
+        means : bool
+            Boolean flag to compute mean resource when res_array is set
 
         Returns
         -------
         SAM_res : SAMResource
-            Instance of SAMResource pre-loaded with Solar resource for sites
+            Instance of SAMResource pre-loaded with Wave resource for sites
             in project_points
         """
-        time_slice = slice(None, None, time_index_step)
-        SAM_res = SAMResource(sites, "geothermal",
-                              res['time_index', time_slice],
-                              depths=depths, means=means)
+        SAM_res = SAMResource(sites, 'wave', self.time_index, means=means)
         sites = SAM_res.sites_slice
-        SAM_res['meta'] = res['meta', sites]
-        res._set_sam_res(res, SAM_res.d, SAM_res.var_list, SAM_res, time_slice,
-                         sites)
+        SAM_res['meta'] = self['meta', sites]
+        for var in SAM_res.var_list:
+            if var in self.datasets:
+                SAM_res[var] = self[var, :, sites]
 
         return SAM_res
 
     @classmethod
-    def preload_SAM(cls, h5_file, sites, depths, unscale=True, str_decode=True,
-                    group=None, hsds=False, hsds_kwargs=None,
-                    time_index_step=None, means=False):
+    def preload_SAM(cls, h5_file, sites, unscale=True, hsds=False,
+                    str_decode=True, group=None, means=False):
         """
         Pre-load project_points for SAM
 
         Parameters
         ----------
         h5_file : str
             h5_file to extract resource from
         sites : list
             List of sites to be provided to SAM
-        depths :  int | float | list
-            Depths to extract for SAM
         unscale : bool
             Boolean flag to automatically unscale variables on extraction
+        hsds : bool
+            Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
+            behind HSDS
         str_decode : bool
             Boolean flag to decode the bytestring meta data into normal
             strings. Setting this to False will speed up the meta data read.
         group : str
             Group within .h5 resource file to open
-        hsds : bool, optional
-            Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
-            behind HSDS, by default False
-        hsds_kwargs : dict, optional
-            Dictionary of optional kwargs for h5pyd, e.g., bucket, username,
-            password, by default None
-        tech : str, optional
-            SAM technology string, by default 'geothermal'
-        time_index_step: int, optional
-            Step size for time_index, used to reduce temporal resolution,
-            by default None
-        means : bool, optional
-            Boolean flag to compute mean resource when res_array is set,
-            by default False
+        means : bool
+            Boolean flag to compute mean resource when res_array is set
 
         Returns
         -------
         SAM_res : SAMResource
-            Instance of SAMResource pre-loaded with Solar resource for sites
+            Instance of SAMResource pre-loaded with Wave resource for sites
             in project_points
         """
-        kwargs = {"unscale": unscale, "hsds": hsds, 'hsds_kwargs': hsds_kwargs,
+        kwargs = {"unscale": unscale, "hsds": hsds,
                   "str_decode": str_decode, "group": group}
         with cls(h5_file, **kwargs) as res:
-            SAM_res = res._preload_SAM(res, sites, depths,
-                                       time_index_step=time_index_step,
-                                       means=means)
+            SAM_res = res._preload_SAM(sites, means=means)
 
         return SAM_res
 
 
-def linear_interp(ts_1, h_1, ts_2, h_2, h):
+class MultiFileNSRDB(MultiFileResource, NSRDB):
     """
-    Linear interpolate/extrapolate time-series data to height h
+    Class to handle 2018 and beyond NSRDB data that is at 2km and
+    sub 30 min resolution
 
-    Parameters
-    ----------
-    ts_1 : ndarray
-        Time-series array at height h_1
-    h_1 : int | float
-        Height corresponding to time-seris ts_1
-    ts_2 : ndarray
-        Time-series array at height h_2
-    h_2 : int | float
-        Height corresponding to time-seris ts_2
-    h : int | float
-        Height of desired time-series
-
-    Returns
-    -------
-    out : ndarray
-        Time-series array at height h
+    See Also
+    --------
+    resource.MultiFileResource : Parent class
+    resource.NSRDB : Parent class
     """
-    if h_1 > h_2:
-        h_1, h_2 = h_2, h_1
-        ts_1, ts_2 = ts_2, ts_1
-
-    # Calculate slope for every position in variable arrays
-    m = (ts_2 - ts_1) / (h_2 - h_1)
-    # Calculate intercept for every position in variable arrays
-    b = ts_2 - m * h_2
+    @classmethod
+    def preload_SAM(cls, h5_path, sites, unscale=True, str_decode=True,
+                    tech='pvwattsv7', clearsky=False, downscale=None,
+                    means=False):
+        """
+        Pre-load project_points for SAM
 
-    out = m * h + b
+        Parameters
+        ----------
+        h5_path : str
+            Path to directory containing multi-file resource file sets.
+            Available formats:
+                /h5_dir/
+                /h5_dir/prefix*suffix
+        sites : list
+            List of sites to be provided to SAM
+        unscale : bool
+            Boolean flag to automatically unscale variables on extraction
+        str_decode : bool
+            Boolean flag to decode the bytestring meta data into normal
+            strings. Setting this to False will speed up the meta data read.
+        tech : str, optional
+            SAM technology string, by default 'pvwattsv7'
+        clearsky : bool
+            Boolean flag to pull clearsky instead of real irradiance
+        downscale : NoneType | str
+            Option for NSRDB resource downscaling to higher temporal
+            resolution. Expects a string in the Pandas frequency format,
+            e.g. '5min'.
+        means : bool
+            Boolean flag to compute mean resource when res_array is set
+
+        Returns
+        -------
+        SAM_res : SAMResource
+            Instance of SAMResource pre-loaded with Solar resource for sites
+            in project_points
+        """
+        with cls(h5_path, unscale=unscale, str_decode=str_decode) as res:
+            # pylint: disable=assignment-from-no-return
+            SAM_res = res._preload_SAM(sites, tech=tech, clearsky=clearsky,
+                                       downscale=downscale, means=means)
+
+        return SAM_res
+
+
+class MultiFileWTK(MultiFileResource, WindResource):
+    """
+    Class to handle 5min WIND Toolkit data
+
+    See Also
+    --------
+    resource.MultiFileResource : Parent class
+    resource.WindResource : Parent class
+
+    Examples
+    --------
+    MultiFileWTK automatically searches for files of the form *m.h5
+
+    >>> file = '$TESTDATADIR/wtk'
+    >>> with MultiFileWTK(file) as res:
+    >>>     print(list(res._h5_files)
+    >>>     print(res.datasets)
+    ['$TESTDATADIR/wtk_2010_200m.h5',
+     '$TESTDATADIR/wtk_2010_100m.h5']
+    ['coordinates', 'meta', 'pressure_100m', 'pressure_200m',
+     'temperature_100m', 'temperature_200m', 'time_index',
+     'winddirection_100m', 'winddirection_200m', 'windspeed_100m',
+     'windspeed_200m']
+
+    MultiFileWTK, like WindResource can interpolate / extrapolate hub-heights
+
+    >>> with MultiFileWTK(file) as res:
+    >>>     wspd = res['windspeed_150m']
+    >>>
+    >>> wspd
+    [[16.19     16.25     16.305    ... 16.375    16.39     16.39    ]
+     [16.15     16.205    16.255001 ... 16.35     16.365    16.39    ]
+     [16.154999 16.195    16.23     ... 16.335    16.32     16.34    ]
+     ...
+     [10.965    11.675    12.08     ... 15.18     14.805    14.42    ]
+     [11.66     11.91     12.535    ... 13.31     12.23     12.335   ]
+     [12.785    13.295    14.014999 ... 12.205    11.360001 11.64    ]]
+    """
+    SUFFIX = 'm.h5'
+
+    def __init__(self, h5_path, unscale=True, str_decode=True):
+        """
+        Parameters
+        ----------
+        h5_path : str
+            Path to directory containing multi-file resource file sets.
+            Available formats:
+                /h5_dir/
+                /h5_dir/prefix*suffix
+        unscale : bool
+            Boolean flag to automatically unscale variables on extraction
+        str_decode : bool
+            Boolean flag to decode the bytestring meta data into normal
+            strings. Setting this to False will speed up the meta data read.
+        """
+        super().__init__(h5_path, unscale=unscale, str_decode=str_decode)
+        self._heights = None
+
+    @classmethod
+    def preload_SAM(cls, h5_path, sites, hub_heights, unscale=True,
+                    str_decode=True, require_wind_dir=False,
+                    precip_rate=False, icing=False, means=False):
+        """
+        Placeholder for classmethod that will pre-load project_points for SAM
+
+        Parameters
+        ----------
+        h5_path : str
+            Path to directory containing multi-file resource file sets.
+            Available formats:
+                /h5_dir/
+                /h5_dir/prefix*suffix
+        sites : list
+            List of sites to be provided to SAM
+        hub_heights : int | float | list
+            Hub heights to extract for SAM
+        unscale : bool
+            Boolean flag to automatically unscale variables on extraction
+        str_decode : bool
+            Boolean flag to decode the bytestring meta data into normal
+            strings. Setting this to False will speed up the meta data read.
+        require_wind_dir : bool
+            Boolean flag as to whether wind direction will be loaded.
+        precip_rate : bool
+            Boolean flag as to whether precipitationrate_0m will be preloaded
+        icing : bool
+            Boolean flag as to whether icing is analyzed.
+            This will preload relative humidity.
+        means : bool
+            Boolean flag to compute mean resource when res_array is set
+
+        Returns
+        -------
+        SAM_res : SAMResource
+            Instance of SAMResource pre-loaded with Solar resource for sites
+            in project_points
+        """
+        with cls(h5_path, unscale=unscale, str_decode=str_decode) as res:
+            # pylint: disable=assignment-from-no-return
+            SAM_res = res._preload_SAM(sites, hub_heights,
+                                       require_wind_dir=require_wind_dir,
+                                       precip_rate=precip_rate, icing=icing,
+                                       means=means)
 
-    return out
+        return SAM_res
```

### Comparing `NREL-rex-0.2.81/rex/resource.py` & `NREL-rex-0.2.9/rex/resource.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,123 +1,99 @@
 # -*- coding: utf-8 -*-
 """
 Classes to handle resource data
 """
-from abc import ABC
 import h5py
 import numpy as np
 import os
 import pandas as pd
-import dateutil
-from warnings import warn
 
-from rex.sam_resource import SAMResource
 from rex.utilities.parse_keys import parse_keys, parse_slice
-from rex.utilities.exceptions import ResourceKeyError, ResourceRuntimeError
-from rex.utilities.utilities import check_tz, get_lat_lon_cols
+from rex.utilities.exceptions import (ResourceKeyError, ResourceRuntimeError)
 
 
 class ResourceDataset:
     """
     h5py.Dataset wrapper for Resource .h5 files
     """
-
     def __init__(self, ds, scale_attr='scale_factor', add_attr='add_offset',
                  unscale=True):
         """
         Parameters
         ----------
         ds : h5py.dataset
             Open .h5 dataset instance to extract data from
-        scale_attr : str | list | optional
-            Name of scale factor attribute, by default 'scale_factor'. Can also
-            be a prioritized list of scale factor names.
-        add_attr : str | list | optional
-            Name of add offset attribute, by default 'add_offset'. Can also
-            be a prioritized list of add offset names.
+        scale_attr : str, optional
+            Name of scale factor attribute, by default 'scale_factor'
+        add_attr : str, optional
+            Name of add offset attribute, by default 'add_offset'
         unscale : bool, optional
             Flag to unscale dataset data, by default True
         """
         self._ds = ds
-
-        self._scale_factor = self._parse_scale_add_attrs(scale_attr, 1)
-        self._adder = self._parse_scale_add_attrs(add_attr, 0)
-
+        self._scale_factor = self._ds.attrs.get(scale_attr, 1)
+        self._adder = self._ds.attrs.get(add_attr, 0)
         self._unscale = unscale
-        if self._scale_factor == 1 and self._adder == 0:
-            self._unscale = False
 
     def __repr__(self):
-        msg = "{} for {}".format(self.__class__.__name__, self.ds.name)
+        msg = "{} for {}".format(self.__class__.__name__, self._ds.name)
 
         return msg
 
     def __getitem__(self, ds_slice):
         ds_slice = parse_slice(ds_slice)
+        out = self._extract_ds_slice(ds_slice)
+        if self._unscale:
+            out = self._unscale_data(out)
 
-        return self._get_ds_slice(ds_slice)
-
-    @property
-    def ds(self):
-        """
-        Open Dataset instance
-
-        Returns
-        -------
-        h5py(d).Dataset
-        """
-        return self._ds
+        return out
 
     @property
     def shape(self):
         """
         Dataset shape
 
         Returns
         -------
         tuple
         """
-        return self.ds.shape
+        return self._ds.shape
 
     @property
     def size(self):
         """
         Dataset size
 
         Returns
         -------
         int
         """
-        return self.ds.size
+        return self._ds.size
 
     @property
     def dtype(self):
         """
         Dataset dtype
 
         Returns
         -------
         str | numpy.dtype
         """
-        return self.ds.dtype
+        return self._ds.dtype
 
     @property
     def chunks(self):
         """
         Dataset chunk size
 
         Returns
         -------
         tuple
         """
-        chunks = self.ds.chunks
-        if isinstance(chunks, dict):
-            chunks = tuple(chunks.get('dims', None))
-
-        return chunks
+        return self._ds.chunks
 
     @property
     def scale_factor(self):
         """
         Dataset scale factor
 
         Returns
@@ -133,360 +109,67 @@
 
         Returns
         -------
         float
         """
         return self._adder
 
-    def _parse_scale_add_attrs(self, attr, default):
-        """Get the scale and add offset factors using one or more prioritized
-        scale/add attribute names.
-
-        Parameters
-        ----------
-        attr : str | list | optional
-            Name of scale factor or adder attribute. Can also
-            be a prioritized list of attr names.
-        default : float
-            Default factor if attr is not found
-
-        Returns
-        -------
-        factor : float
-            Multiplicative or adder scale factor retrieved from dataset
-            attributes.
-        """
-
-        factor = default
-
-        if isinstance(attr, str):
-            attr = [attr]
-
-        for name in attr:
-            if name in self.ds.attrs:
-                factor = self.ds.attrs[name]
-                break
-
-        return factor
-
     @staticmethod
     def _check_slice(ds_slice):
         """
-        Check ds_slice for lists, ensure lists are of the same len
-
-        Parameters
-        ----------
-        ds_slice : tuple
-            Tuple of (int, slice, list, ndarray) of what to extract from ds,
-            each arg is for a sequential axis
-
-        Returns
-        -------
-        list_len : int | None
-            List lenght, None if none of the args are a list | ndarray
-        multi_list : bool
-            Flag if multiple list are provided in ds_slice
-        """
-        multi_list = False
-        list_len = []
-        for s in ds_slice:
-            if isinstance(s, (list, np.ndarray)):
-                list_len.append(len(s))
-
-        if list_len:
-            if len(list_len) > 1:
-                multi_list = True
-
-            list_len = list(set(list_len))
-            if len(list_len) > 1:
-                msg = ('shape mismatch: indexing arrays could not be '
-                       'broadcast together with shapes {}'
-                       .format(['({},)'.format(ln) for ln in list_len]))
-                raise IndexError(msg)
-            else:
-                list_len = list_len[0]
-        else:
-            list_len = None
-
-        return list_len, multi_list
-
-    @staticmethod
-    def _make_list_slices(ds_slice, list_len):
-        """
-        Duplicate slice arguements to enable zipping of list slices with
-        non-list slices
-
-        Parameters
-        ----------
-        ds_slice : tuple
-            Tuple of (int, slice, list, ndarray) of what to extract from ds,
-            each arg is for a sequential axis
-        list_len : int
-            List lenght
-
-        Returns
-        -------
-        zip_slices : list
-            List of slices to extract for each entry in list slice
-        """
-        zip_slices = []
-        for s in ds_slice:
-            if not isinstance(s, (list, np.ndarray)):
-                zip_slices.append([s] * list_len)
-            else:
-                zip_slices.append(s)
-
-        return zip_slices
-
-    @staticmethod
-    def _list_to_slice(ds_slice):
-        """
         Check ds_slice to see if it is an int, slice, or list. Return
         pieces required for fancy indexing based on input type.
 
         Parameters
         ----------
-        ds_slice : tuple
-            Tuple of (int, slice, list, ndarray) of what to extract from ds,
-            each arg is for a sequential axis
+        ds_slice : slice | list | ndarray
+            slice, list, or vector of points to extract
 
         Returns
         -------
         ds_slice : slice
             Slice that encompasses the entire range
         ds_idx : ndarray
             Adjusted list to extract points of interest from sliced array
         """
         ds_idx = None
         if isinstance(ds_slice, (list, np.ndarray)):
             in_slice = np.array(ds_slice)
-            if np.issubdtype(in_slice.dtype, np.dtype(bool)):
-                in_slice = np.where(in_slice)[0]
-
             s = in_slice.min()
             e = in_slice.max() + 1
             ds_slice = slice(s, e, None)
             ds_idx = in_slice - s
         elif isinstance(ds_slice, slice):
             ds_idx = slice(None)
 
         return ds_slice, ds_idx
 
-    @staticmethod
-    def _get_out_arr_slice(arr_slice, start):
-        """
-        Determine slice of pre-build output array that is being filled
-
-        Parameters
-        ----------
-        arr_slice : tuple
-            Tuple of (int, slice, list, ndarray) for section of output array
-            being extracted
-        start : int
-            Start of slice, used for list gets
-
-        Returns
-        -------
-        out_slice : tuple
-            Slice arguments of portion of output array to insert arr_slice
-            into
-        stop : int
-            Stop of slice, used for list gets, will be new start upon
-            iteration
-        """
-        out_slice = ()
-        int_slice = ()
-        int_start = start
-        int_stop = start
-        stop = start
-        for s in arr_slice:
-            if isinstance(s, slice):
-                out_slice += (slice(None), )
-                int_slice += (slice(None), )
-            elif isinstance(s, (int, np.integer)):
-                if int_start == int_stop:
-                    int_slice += (int_start, )
-                    int_stop += 1
-            elif isinstance(s, (list, tuple, np.ndarray)):
-                list_len = len(s)
-                if list_len == 1:
-                    stop += 1
-                    out_slice += ([start], )
-                else:
-                    stop += len(s)
-                    out_slice += (slice(start, stop), )
-
-        if not out_slice:
-            out_slice += (start, )
-            stop += 1
-        elif all(s == slice(None) for s in out_slice):
-            out_slice = int_slice
-            stop = int_stop
-
-        return out_slice, stop
-
-    def _get_out_arr_shape(self, ds_slice):
-        """
-        Determine shape of output array
-
-        Parameters
-        ----------
-        ds_slice : tuple
-            Tuple of (int, slice, list, ndarray) of what to extract from ds,
-            each arg is for a sequential axis
-
-        Returns
-        -------
-        out_shape : tuple
-            Shape of output array
-        """
-        ds_shape = self.shape
-        out_shape = ()
-        contains_list = False
-
-        ds_slice += (slice(None), ) * (len(ds_shape) - len(ds_slice))
-        for i, ax_slice in enumerate(ds_slice):
-            if isinstance(ax_slice, slice):
-                stop = ax_slice.stop
-                if stop is None:
-                    stop = ds_shape[i]
-
-                out_shape += (len(range(*ax_slice.indices(stop))), )
-
-            if isinstance(ax_slice, (list, tuple, np.ndarray)):
-                if not contains_list:
-                    out_shape += (len(ax_slice), )
-
-                contains_list = True
-
-        return out_shape
-
-    def _extract_list_slice(self, ds_slice):
-        """
-        Optimize and extract list slice request along a single dimension. This
-        function checks if sequential gid requests are more than one chunk size
-        apart and then splits them into multiple separate requests (more
-        efficient to do multipl reads than to read all gids in-between).
-
-        Parameters
-        ----------
-        ds_slice : tuple
-            Tuple of (int, slice, list, ndarray) of what to extract from ds,
-            each arg is for a sequential axis
-
-        Returns
-        -------
-        out : ndarray
-            Extracted array of data from ds
-        """
-        out_slices = []
-        chunks = self.chunks
-        sort_idx = []
-        list_len = None
-        if chunks:
-            for i, ax_slice in enumerate(ds_slice):
-                c = chunks[i]
-                if isinstance(ax_slice, (list, np.ndarray)):
-                    if not isinstance(ax_slice, np.ndarray):
-                        ax_slice = np.array(ax_slice)
-
-                    idx = np.argsort(ax_slice)
-                    sort_idx.append(np.argsort(idx))
-                    ax_slice = ax_slice[idx]
-
-                    # this checks if sequential gid requests are more than one
-                    # chunk size apart and then splits them into multiple
-                    # separate requests
-                    diff = np.diff(ax_slice) > c
-                    if np.any(diff):
-                        pos = np.where(diff)[0] + 1
-                        ax_slice = np.split(ax_slice, pos)
-                        list_len = len(ax_slice)
-                elif isinstance(ax_slice, slice):
-                    sort_idx.append(slice(None))
-
-                out_slices.append(ax_slice)
-        else:
-            out_slices = ds_slice
-
-        if list_len is not None:
-            out_shape = self._get_out_arr_shape(ds_slice)
-            out_slices = self._make_list_slices(out_slices, list_len)
-
-            out = np.zeros(out_shape, dtype=self.dtype)
-            start = 0
-            for s in zip(*out_slices):
-                arr_slice, stop = self._get_out_arr_slice(s, start)
-                out[arr_slice] = self._extract_ds_slice(s)
-                start = stop
-
-            out = out[tuple(sort_idx)]
-        else:
-            out = self._extract_ds_slice(ds_slice)
-
-        return out
-
-    def _extract_multi_list_slice(self, ds_slice, list_len):
-        """
-        Extract ds_slice that has multiple lists
-
-        Parameters
-        ----------
-        ds_slice : tuple
-            Tuple of (int, slice, list, ndarray) of what to extract from ds,
-            each arg is for a sequential axis
-        list_len : int
-            List lenght
-
-        Returns
-        -------
-        out : ndarray
-            Extracted array of data from ds
-        """
-        zip_slices = self._make_list_slices(ds_slice, list_len)
-
-        out_shape = self._get_out_arr_shape(ds_slice)
-
-        out = np.zeros(out_shape, dtype=self.dtype)
-        start = 0
-        for s in zip(*zip_slices):
-            arr_slice, stop = self._get_out_arr_slice(s, start)
-            arr = self._extract_ds_slice(s)
-            out[arr_slice] = arr
-
-            start = stop
-
-        return out
-
     def _extract_ds_slice(self, ds_slice):
         """
-        Extact ds_slice from ds using slices where possible
+        Extact ds_slice from ds as efficiently as possible.
 
         Parameters
         ----------
-        ds_slice : tuple
-            Tuple of (int, slice, list, ndarray) of what to extract from ds,
-            each arg is for a sequential axis
+        ds_slice : int | slice | list | ndarray
+            What to extract from ds, each arg is for a sequential axis
 
         Returns
         -------
         out : ndarray
             Extracted array of data from ds
         """
         slices = ()
         idx_slice = ()
         for ax_slice in ds_slice:
-            ax_slice, ax_idx = self._list_to_slice(ax_slice)
+            ax_slice, ax_idx = ResourceDataset._check_slice(ax_slice)
             slices += (ax_slice,)
             if ax_idx is not None:
                 idx_slice += (ax_idx,)
 
-        out = self.ds[slices]
-
-        # check to see if idx_slice needs to be applied
+        out = self._ds[slices]
         if any(s != slice(None) if isinstance(s, slice) else True
                for s in idx_slice):
             out = out[idx_slice]
 
         return out
 
     def _unscale_data(self, data):
@@ -509,131 +192,249 @@
             data *= self.scale_factor
             data += self.adder
         else:
             data /= self.scale_factor
 
         return data
 
-    def _get_ds_slice(self, ds_slice):
-        """
-        Get ds_slice from ds as efficiently as possible, unscale if desired
-
-        Parameters
-        ----------
-        ds_slice : tuple
-            Tuple of (int, slice, list, ndarray) of what to extract from ds,
-            each arg is for a sequential axis
-
-        Returns
-        -------
-        out : ndarray
-            Extracted array of data from ds
-        """
-        list_len, multi_list = self._check_slice(ds_slice)
-        if list_len is not None:
-            if multi_list:
-                out = self._extract_multi_list_slice(ds_slice, list_len)
-            else:
-                out = self._extract_list_slice(ds_slice)
-        else:
-            out = self._extract_ds_slice(ds_slice)
-
-        if self._unscale:
-            out = self._unscale_data(out)
-
-        return out
-
     @classmethod
     def extract(cls, ds, ds_slice, scale_attr='scale_factor',
                 add_attr='add_offset', unscale=True):
         """
         Extract data from Resource Dataset
 
         Parameters
         ----------
         ds : h5py.dataset
             Open .h5 dataset instance to extract data from
-        ds_slice : tuple
-            Tuple of (int, slice, list, ndarray) of what to extract from ds,
-            each arg is for a sequential axis
+        ds_slice : slice | list | ndarray
+            slice, list, or vector of points to extract
         scale_attr : str, optional
             Name of scale factor attribute, by default 'scale_factor'
         add_attr : str, optional
             Name of add offset attribute, by default 'add_offset'
         unscale : bool, optional
             Flag to unscale dataset data, by default True
         """
         dset = cls(ds, scale_attr=scale_attr, add_attr=add_attr,
                    unscale=unscale)
 
         return dset[ds_slice]
 
 
-class BaseResource(ABC):
+class Resource:
     """
-    Abstract Base class to handle resource .h5 files
+    Base class to handle resource .h5 files
+
+    Examples
+    --------
+
+    Extracting the resource's Datetime Index
+
+    >>> file = '$TESTDATADIR/nsrdb/ri_100_nsrdb_2012.h5'
+    >>> with Resource(file) as res:
+    >>>     ti = res.time_index
+    >>>
+    >>> ti
+    DatetimeIndex(['2012-01-01 00:00:00', '2012-01-01 00:30:00',
+                   '2012-01-01 01:00:00', '2012-01-01 01:30:00',
+                   '2012-01-01 02:00:00', '2012-01-01 02:30:00',
+                   '2012-01-01 03:00:00', '2012-01-01 03:30:00',
+                   '2012-01-01 04:00:00', '2012-01-01 04:30:00',
+                   ...
+                   '2012-12-31 19:00:00', '2012-12-31 19:30:00',
+                   '2012-12-31 20:00:00', '2012-12-31 20:30:00',
+                   '2012-12-31 21:00:00', '2012-12-31 21:30:00',
+                   '2012-12-31 22:00:00', '2012-12-31 22:30:00',
+                   '2012-12-31 23:00:00', '2012-12-31 23:30:00'],
+                  dtype='datetime64[ns]', length=17568, freq=None)
+
+    Efficient slicing of the Datetime Index
+
+    >>> with Resource(file) as res:
+    >>>     ti = res['time_index', 1]
+    >>>
+    >>> ti
+    2012-01-01 00:30:00
+
+    >>> with Resource(file) as res:
+    >>>     ti = res['time_index', :10]
+    >>>
+    >>> ti
+    DatetimeIndex(['2012-01-01 00:00:00', '2012-01-01 00:30:00',
+                   '2012-01-01 01:00:00', '2012-01-01 01:30:00',
+                   '2012-01-01 02:00:00', '2012-01-01 02:30:00',
+                   '2012-01-01 03:00:00', '2012-01-01 03:30:00',
+                   '2012-01-01 04:00:00', '2012-01-01 04:30:00'],
+                  dtype='datetime64[ns]', freq=None)
+
+    >>> with Resource(file) as res:
+    >>>     ti = res['time_index', [1, 2, 4, 8, 9]
+    >>>
+    >>> ti
+    DatetimeIndex(['2012-01-01 00:30:00', '2012-01-01 01:00:00',
+                   '2012-01-01 02:00:00', '2012-01-01 04:00:00',
+                   '2012-01-01 04:30:00'],
+                  dtype='datetime64[ns]', freq=None)
+
+    Extracting resource's site metadata
+
+    >>> with Resource(file) as res:
+    >>>     meta = res.meta
+    >>>
+    >>> meta
+            latitude  longitude   elevation  timezone    country ...
+    0      41.29     -71.86    0.000000        -5           None ...
+    1      41.29     -71.82    0.000000        -5           None ...
+    2      41.25     -71.82    0.000000        -5           None ...
+    3      41.33     -71.82   15.263158        -5  United States ...
+    4      41.37     -71.82   25.360000        -5  United States ...
+    ..       ...        ...         ...       ...            ... ...
+    95     41.25     -71.66    0.000000        -5           None ...
+    96     41.89     -71.66  153.720000        -5  United States ...
+    97     41.45     -71.66   35.440000        -5  United States ...
+    98     41.61     -71.66  140.200000        -5  United States ...
+    99     41.41     -71.66   35.160000        -5  United States ...
+    [100 rows x 10 columns]
+
+    Efficient slicing of the metadata
+
+    >>> with Resource(file) as res:
+    >>>     meta = res['meta', 1]
+    >>>
+    >>> meta
+       latitude  longitude  elevation  timezone country state county urban ...
+    1     41.29     -71.82        0.0        -5    None  None   None  None ...
+
+    >>> with Resource(file) as res:
+    >>>     meta = res['meta', :5]
+    >>>
+    >>> meta
+       latitude  longitude  elevation  timezone        country ...
+    0     41.29     -71.86   0.000000        -5           None ...
+    1     41.29     -71.82   0.000000        -5           None ...
+    2     41.25     -71.82   0.000000        -5           None ...
+    3     41.33     -71.82  15.263158        -5  United States ...
+    4     41.37     -71.82  25.360000        -5  United States ...
+
+    >>> with Resource(file) as res:
+    >>>     tz = res['meta', :, 'timezone']
+    >>>
+    >>> tz
+    0    -5
+    1    -5
+    2    -5
+    3    -5
+    4    -5
+         ..
+    95   -5
+    96   -5
+    97   -5
+    98   -5
+    99   -5
+    Name: timezone, Length: 100, dtype: int64
+
+    >>> with Resource(file) as res:
+    >>>     lat_lon = res['meta', :, ['latitude', 'longitude']]
+    >>>
+    >>> lat_lon
+        latitude  longitude
+    0      41.29     -71.86
+    1      41.29     -71.82
+    2      41.25     -71.82
+    3      41.33     -71.82
+    4      41.37     -71.82
+    ..       ...        ...
+    95     41.25     -71.66
+    96     41.89     -71.66
+    97     41.45     -71.66
+    98     41.61     -71.66
+    99     41.41     -71.66
+    [100 rows x 2 columns]
+
+    Extracting resource variables (datasets)
+
+    >>> with Resource(file) as res:
+    >>>     wspd = res['wind_speed']
+    >>>
+    >>> wspd
+    [[12. 12. 12. ... 12. 12. 12.]
+     [12. 12. 12. ... 12. 12. 12.]
+     [12. 12. 12. ... 12. 12. 12.]
+     ...
+     [14. 14. 14. ... 14. 14. 14.]
+     [15. 15. 15. ... 15. 15. 15.]
+     [15. 15. 15. ... 15. 15. 15.]]
+
+    Efficient slicing of variables
+
+    >>> with Resource(file) as res:
+    >>>     wspd = res['wind_speed', :2]
+    >>>
+    >>> wspd
+    [[12. 12. 12. 12. 12. 12. 53. 53. 53. 53. 53. 12. 53.  1.  1. 12. 12. 12.
+       1.  1. 12. 53. 53. 53. 12. 12. 12. 12. 12.  1. 12. 12.  1. 12. 12. 53.
+      12. 53.  1. 12.  1. 53. 53. 12. 12. 12. 12.  1.  1.  1. 12. 12.  1.  1.
+      12. 12. 53. 53. 53. 12. 12. 53. 53. 12. 12. 12. 12. 12. 12.  1. 53.  1.
+      53. 12. 12. 53. 53.  1.  1.  1. 53. 12.  1.  1. 53. 53. 53. 12. 12. 12.
+      12. 12. 12. 12.  1. 12.  1. 12. 12. 12.]
+     [12. 12. 12. 12. 12. 12. 53. 53. 53. 53. 53. 12. 53.  1.  1. 12. 12. 12.
+       1.  1. 12. 53. 53. 53. 12. 12. 12. 12. 12.  1. 12. 12.  1. 12. 12. 53.
+      12. 53.  1. 12.  1. 53. 53. 12. 12. 12. 12.  1.  1.  1. 12. 12.  1.  1.
+      12. 12. 53. 53. 53. 12. 12. 53. 53. 12. 12. 12. 12. 12. 12.  1. 53.  1.
+      53. 12. 12. 53. 53.  1.  1.  1. 53. 12.  1.  1. 53. 53. 53. 12. 12. 12.
+      12. 12. 12. 12.  1. 12.  1. 12. 12. 12.]]
+
+    >>> with Resource(file) as res:
+    >>>     wspd = res['wind_speed', :, [2, 3]]
+    >>>
+    >>> wspd
+    [[12. 12.]
+     [12. 12.]
+     [12. 12.]
+     ...
+     [14. 14.]
+     [15. 15.]
+     [15. 15.]]
     """
     SCALE_ATTR = 'scale_factor'
     ADD_ATTR = 'add_offset'
     UNIT_ATTR = 'units'
 
-    def __init__(self, h5_file, mode='r', unscale=True, str_decode=True,
-                 group=None, hsds=False, hsds_kwargs=None):
+    def __init__(self, h5_file, unscale=True, hsds=False, str_decode=True,
+                 group=None):
         """
         Parameters
         ----------
         h5_file : str
             Path to .h5 resource file
-        mode : str, optional
-            Mode to instantiate h5py.File instance, by default 'r'
-        unscale : bool, optional
-            Boolean flag to automatically unscale variables on extraction,
-            by default True
-        str_decode : bool, optional
-            Boolean flag to decode the bytestring meta data into normal
-            strings. Setting this to False will speed up the meta data read,
-            by default True
-        group : str, optional
-            Group within .h5 resource file to open, by default None
-        hsds : bool, optional
+        unscale : bool
+            Boolean flag to automatically unscale variables on extraction
+        hsds : bool
             Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
-            behind HSDS, by default False
-        hsds_kwargs : dict, optional
-            Dictionary of optional kwargs for h5pyd, e.g., bucket, username,
-            password, by default None
+            behind HSDS
+        str_decode : bool
+            Boolean flag to decode the bytestring meta data into normal
+            strings. Setting this to False will speed up the meta data read.
+        group : str
+            Group within .h5 resource file to open
         """
         self.h5_file = h5_file
         if hsds:
-            if mode != 'r':
-                raise IOError('Cannot write to files accessed vias HSDS!')
-
             import h5pyd
-            if hsds_kwargs is None:
-                hsds_kwargs = {}
-
-            self._h5 = h5pyd.File(self.h5_file, mode='r', use_cache=False,
-                                  **hsds_kwargs)
+            self._h5 = h5pyd.File(self.h5_file, 'r')
         else:
-            try:
-                self._h5 = h5py.File(self.h5_file, mode=mode)
-            except Exception as e:
-                msg = ('Could not open file in mode "{}": "{}"'
-                       .format(mode, self.h5_file))
-                raise IOError(msg) from e
+            self._h5 = h5py.File(self.h5_file, 'r')
 
         self._group = group
         self._unscale = unscale
         self._meta = None
         self._time_index = None
-        self._lat_lon = None
+        self._coords = None
         self._str_decode = str_decode
-        self._attrs = None
-        self._shapes = None
-        self._chunks = None
-        self._dtypes = None
         self._i = 0
 
     def __repr__(self):
         msg = "{} for {}".format(self.__class__.__name__, self.h5_file)
 
         return msg
 
@@ -643,37 +444,32 @@
     def __exit__(self, type, value, traceback):
         self.close()
 
         if type is not None:
             raise
 
     def __len__(self):
-        return self.h5['time_index'].shape[0]
+        return self.h5['meta'].shape[0]
 
     def __getitem__(self, keys):
         ds, ds_slice = parse_keys(keys)
-        _, ds_name = os.path.split(ds)
 
-        if ds_name.startswith('time_index'):
+        if ds.endswith('time_index'):
             out = self._get_time_index(ds, ds_slice)
-
-        elif ds_name.startswith('meta'):
+        elif ds.endswith('meta'):
             out = self._get_meta(ds, ds_slice)
-
-        elif ds_name.startswith('coordinates'):
+        elif ds.endswith('coordinates'):
             out = self._get_coords(ds, ds_slice)
-
-        elif 'SAM' in ds_name:
+        elif 'SAM' in ds:
             site = ds_slice[0]
-            if isinstance(site, (int, np.integer)):
-                out = self.get_SAM_df(site)  # pylint: disable=E1111
+            if isinstance(site, int):
+                out = self._get_SAM_df(ds, site)  # pylint: disable=E1111
             else:
                 msg = "Can only extract SAM DataFrame for a single site"
                 raise ResourceRuntimeError(msg)
-
         else:
             out = self._get_ds(ds, ds_slice)
 
         return out
 
     def __iter__(self):
         return self
@@ -687,16 +483,16 @@
         self._i += 1
 
         return dset
 
     def __contains__(self, dset):
         return dset in self.datasets
 
-    @classmethod
-    def _get_datasets(cls, h5_obj, group=None):
+    @staticmethod
+    def _get_datasets(h5_obj, group=None):
         """
         Search h5 file instance for Datasets
 
         Parameters
         ----------
         h5_obj : h5py.File | h5py.Group
             Open h5py File or Group instance to search
@@ -706,15 +502,15 @@
         dsets : list
             List of datasets in h5_obj
         """
         dsets = []
         for name in h5_obj:
             sub_obj = h5_obj[name]
             if isinstance(sub_obj, h5py.Group):
-                dsets.extend(cls._get_datasets(sub_obj, group=name))
+                dsets.extend(Resource._get_datasets(sub_obj, group=name))
             else:
                 dset_name = name
                 if group is not None:
                     dset_name = "{}/{}".format(group, dset_name)
 
                 dsets.append(dset_name)
 
@@ -724,14 +520,15 @@
     def h5(self):
         """
         Open h5py File instance. If _group is not None return open Group
 
         Returns
         -------
         h5 : h5py.File | h5py.Group
+            Open h5py File or Group instance
         """
         h5 = self._h5
         if self._group is not None:
             h5 = h5[self._group]
 
         return h5
 
@@ -739,54 +536,31 @@
     def datasets(self):
         """
         Datasets available
 
         Returns
         -------
         list
+            List of datasets
         """
         return self._get_datasets(self.h5)
 
     @property
     def dsets(self):
         """
         Datasets available
 
         Returns
         -------
         list
+            List of datasets
         """
         return self.datasets
 
     @property
-    def resource_datasets(self):
-        """
-        Available resource datasets
-
-        Returns
-        -------
-        list
-        """
-        dsets = [ds for ds in self.datasets
-                 if ds not in ['meta', 'time_index', 'coordinates']]
-
-        return dsets
-
-    @property
-    def res_dsets(self):
-        """
-        Available resource datasets
-
-        Returns
-        -------
-        list
-        """
-        return self.resource_datasets
-
-    @property
     def groups(self):
         """
         Groups available
 
         Returns
         -------
         groups : list
@@ -804,44 +578,46 @@
         """
         Resource shape (timesteps, sites)
         shape = (len(time_index), len(meta))
 
         Returns
         -------
         shape : tuple
+            Shape of resource variable arrays (timesteps, sites)
         """
-        shape = (self.h5['time_index'].shape[0], self.h5['meta'].shape[0])
-
-        return shape
+        _shape = (self.h5['time_index'].shape[0], self.h5['meta'].shape[0])
+        return _shape
 
     @property
     def meta(self):
         """
-        Resource meta data DataFrame
+        Meta data DataFrame
 
         Returns
         -------
         meta : pandas.DataFrame
+            Resource Meta Data
         """
         if self._meta is None:
             if 'meta' in self.h5:
                 self._meta = self._get_meta('meta', slice(None))
             else:
                 raise ResourceKeyError("'meta' is not a valid dataset")
 
         return self._meta
 
     @property
     def time_index(self):
         """
-        Resource DatetimeIndex
+        DatetimeIndex
 
         Returns
         -------
         time_index : pandas.DatetimeIndex
+            Resource datetime index
         """
         if self._time_index is None:
             if 'time_index' in self.h5:
                 self._time_index = self._get_time_index('time_index',
                                                         slice(None))
             else:
                 raise ResourceKeyError("'time_index' is not a valid dataset!")
@@ -851,46 +627,24 @@
     @property
     def coordinates(self):
         """
         Coordinates: (lat, lon) pairs
 
         Returns
         -------
-        lat_lon : ndarray
-        """
-        return self.lat_lon
-
-    @property
-    def lat_lon(self):
-        """
-        Extract (latitude, longitude) pairs
-
-        Returns
-        -------
-        lat_lon : ndarray
+        coords : ndarray
+            Array of (lat, lon) pairs for each site in meta
         """
-        if self._lat_lon is None:
-            if 'coordinates' in self:
-                self._lat_lon = self._get_coords('coordinates', slice(None))
+        if self._coords is None:
+            if 'coordinates' in self.h5:
+                self._coords = self._get_coords('coordinates', slice(None))
             else:
-                lat_lon_cols = get_lat_lon_cols(self.meta)
-                self._lat_lon = self.meta[lat_lon_cols].values
-
-        return self._lat_lon
-
-    @property
-    def data_version(self):
-        """
-        Get the version attribute of the data. None if not available.
+                raise ResourceKeyError("'coordinates' is not a valid dataset!")
 
-        Returns
-        -------
-        version : str | None
-        """
-        return self.global_attrs.get('version', None)
+        return self._coords
 
     @property
     def global_attrs(self):
         """
         Global (file) attributes
 
         Returns
@@ -898,159 +652,22 @@
         global_attrs : dict
         """
         return dict(self.h5.attrs)
 
     @property
     def attrs(self):
         """
-        Dictionary of all dataset attributes
+        Global (file) attributes
 
         Returns
         -------
         attrs : dict
+            .h5 file attributes sourced from first .h5 file
         """
-        if self._attrs is None:
-            self._attrs = {}
-            for dset in self.datasets:
-                self._attrs[dset] = dict(self.h5[dset].attrs)
-
-        return self._attrs
-
-    @property
-    def shapes(self):
-        """
-        Dictionary of all dataset shapes
-
-        Returns
-        -------
-        shapes : dict
-        """
-        if self._shapes is None:
-            self._shapes = {}
-            for dset in self.datasets:
-                self._shapes[dset] = self.h5[dset].shape
-
-        return self._shapes
-
-    @property
-    def dtypes(self):
-        """
-        Dictionary of all dataset dtypes
-
-        Returns
-        -------
-        dtypes : dict
-        """
-        if self._dtypes is None:
-            self._dtypes = {}
-            for dset in self.datasets:
-                self._dtypes[dset] = self.h5[dset].dtype
-
-        return self._dtypes
-
-    @property
-    def chunks(self):
-        """
-        Dictionary of all dataset chunk sizes
-
-        Returns
-        -------
-        chunks : dict
-        """
-        if self._chunks is None:
-            self._chunks = {}
-            for dset in self.datasets:
-                self._chunks[dset] = self._check_chunks(self.h5[dset].chunks)
-
-        return self._chunks
-
-    @property
-    def adders(self):
-        """
-        Dictionary of all dataset add offset factors
-
-        Returns
-        -------
-        adders : dict
-        """
-        return self._parse_attr_names(self.ADD_ATTR, 0)
-
-    @property
-    def scale_factors(self):
-        """
-        Dictionary of all dataset scale factors
-
-        Returns
-        -------
-        scale_factors : dict
-        """
-        return self._parse_attr_names(self.SCALE_ATTR, 1)
-
-    @property
-    def units(self):
-        """
-        Dictionary of all dataset units
-
-        Returns
-        -------
-        units : dict
-        """
-        return self._parse_attr_names(self.UNIT_ATTR, None)
-
-    def _parse_attr_names(self, attr_names, default):
-        """Retrieve an attribute from all dataset attributes.
-
-        Parameters
-        ----------
-        attr_names : str | list
-            Single or prioritized list of attribute names to retrieve, e.g.
-            "scale_factor" or ["scale_factor", "psm_scale_factor"]
-        default : None | int | float
-            Default value if attr_names not found in any given dataset.
-
-        Returns
-        -------
-        out : dict
-            Dictionary mapping datasets (keys) to attribute values (values),
-            e.g. if attr_names="scale_factor", out would be:
-            {"windspeed_10m": 10, "misc": 1}
-        """
-
-        if isinstance(attr_names, str):
-            attr_names = [attr_names]
-
-        out = {}
-        for dset, attrs in self.attrs.items():
-            out[dset] = default
-            for name in attr_names:
-                if name in attrs:
-                    out[dset] = attrs[name]
-                    break
-
-        return out
-
-    @staticmethod
-    def _check_chunks(chunks):
-        """
-        Check to see if chunks is an HSDS dictionary, if so convert to a tuple
-
-        Parameters
-        ----------
-        chunks : tuple | dict | None
-            tuple of chunk size, None, or HSDS chunk dictionary
-
-        Returns
-        -------
-        chunks : tuple
-            Tuple of chunk size along all axes
-        """
-        if isinstance(chunks, dict):
-            chunks = tuple(chunks.get('dims', None))
-
-        return chunks
+        return self.global_attrs
 
     @staticmethod
     def df_str_decode(df):
         """Decode a dataframe with byte string columns into ordinary str cols.
 
         Parameters
         ----------
@@ -1129,55 +746,50 @@
         dtype : str
             Dataset array dtype
         chunks : tuple
             Dataset chunk size
         """
         ds = self.h5[dset]
         shape, dtype, chunks = ds.shape, ds.dtype, ds.chunks
+        if isinstance(chunks, dict):
+            chunks = tuple(chunks.get('dims', None))
 
-        return shape, dtype, self._check_chunks(chunks)
+        return shape, dtype, chunks
 
-    def get_scale_factor(self, dset):
+    def get_scale(self, dset):
         """
         Get dataset scale factor
 
         Parameters
         ----------
         dset : str
             Dataset to get scale factor for
 
         Returns
         -------
         float
             Dataset scale factor, used to unscale int values to floats
         """
-        return self.scale_factors[dset]
+        return self.h5[dset].attrs.get(self.SCALE_ATTR, 1)
 
-    # pylint: disable=redefined-argument-from-local
     def get_units(self, dset):
         """
         Get dataset units
 
         Parameters
         ----------
         dset : str
             Dataset to get units for
 
         Returns
         -------
         str
             Dataset units, None if not defined
         """
-        if dset not in self:
-            name = dset.split('_')[0]
-            for dset in self.resource_datasets:
-                if dset.startswith(name):
-                    break
-
-        return self.units[dset]
+        return self.h5[dset].attrs.get(self.UNIT_ATTR, None)
 
     def get_meta_arr(self, rec_name, rows=slice(None)):
         """Get a meta array by name (faster than DataFrame extraction).
 
         Parameters
         ----------
         rec_name : str
@@ -1203,70 +815,60 @@
         """
         Extract and convert time_index to pandas Datetime Index
 
         Parameters
         ----------
         ds_name : str
             Dataset to extract time_index from
-        ds_slice : tuple
-            Tuple of (int, slice, list, ndarray) of what to extract from
-            time_index
+        ds_slice : int | list | slice
+            tuple describing slice of time_index to extract
 
         Returns
         -------
         time_index : pandas.DatetimeIndex
             Vector of datetime stamps
         """
         ds_slice = parse_slice(ds_slice)
         time_index = self.h5[ds_name]
         time_index = ResourceDataset.extract(time_index, ds_slice[0],
                                              unscale=False)
-        try:
-            datetime_index = pd.to_datetime(time_index.astype(str))
-        except (pd.errors.OutOfBoundsDatetime, dateutil.parser.ParserError):
-            return time_index
-
-        return check_tz(datetime_index)
+        # time_index: np.array
+        return pd.to_datetime(time_index.astype(str))
 
     def _get_meta(self, ds_name, ds_slice):
         """
         Extract and convert meta to a pandas DataFrame
 
         Parameters
         ----------
         ds_name : str
             Dataset to extract meta from
-        ds_slice : tuple
-            Tuple of (int, slice, list, ndarray, str) of what sites and columns
-            to extract from meta
+        ds_slice : int | list | slice
+            Pandas slicing describing which sites and columns to extract
 
         Returns
         -------
         meta : pandas.Dataframe
             Dataframe of location meta data
         """
         ds_slice = parse_slice(ds_slice)
         sites = ds_slice[0]
-        if isinstance(sites, (int, np.integer)):
+        if isinstance(sites, int):
             sites = slice(sites, sites + 1)
 
         meta = self.h5[ds_name]
         meta = ResourceDataset.extract(meta, sites, unscale=False)
 
         if isinstance(sites, slice):
-            stop = sites.stop
-            if stop is None:
-                stop = len(meta)
-
-            sites = list(range(*sites.indices(stop)))
+            if sites.stop:
+                sites = list(range(*sites.indices(sites.stop)))
+            else:
+                sites = list(range(len(meta)))
 
         meta = pd.DataFrame(meta, index=sites)
-        if 'gid' not in meta:
-            meta.index.name = 'gid'
-
         if self._str_decode:
             meta = self.df_str_decode(meta)
 
         if len(ds_slice) == 2:
             meta = meta[ds_slice[1]]
 
         return meta
@@ -1275,482 +877,399 @@
         """
         Extract coordinates (lat, lon) pairs
 
         Parameters
         ----------
         ds_name : str
             Dataset to extract coordinates from
-        ds_slice : tuple
-            Tuple of (int, slice, list, ndarray) of what to extract from
-            coordinates, each arg is for a sequential axis
+        ds_slice : int | list | slice
+            tuple describing slice of coordinates to extract
 
         Returns
         -------
         coords : ndarray
             Array of (lat, lon) pairs for each site in meta
         """
         ds_slice = parse_slice(ds_slice)
         coords = self.h5[ds_name]
         coords = ResourceDataset.extract(coords, ds_slice[0],
                                          unscale=False)
         return coords
 
-    # pylint: disable=unused-argument
-    def get_SAM_df(self, site):
+    def _get_SAM_df(self, ds_name, site):
         """
         Placeholder for get_SAM_df method that it resource specific
 
         Parameters
         ----------
+        ds_name : str
+            'Dataset' name == SAM
         site : int
             Site to extract SAM DataFrame for
         """
-        msg = ('Method to retrieve SAM dataframe not implemented for vanilla '
-               'Resource handler. Use an NSRDB or WTK handler instead.')
-        raise NotImplementedError(msg)
 
     def _get_ds(self, ds_name, ds_slice):
         """
         Extract data from given dataset
 
         Parameters
         ----------
         ds_name : str
             Variable dataset to be extracted
-        ds_slice : tuple
-            Tuple of (int, slice, list, ndarray) of what to extract from ds,
-            each arg is for a sequential axis
+        ds_slice : int | list | slice
+            tuple describing slice of dataset array to extract
 
         Returns
         -------
         out : ndarray
             ndarray of variable timeseries data
             If unscale, returned in native units else in scaled units
         """
         if ds_name not in self.datasets:
             raise ResourceKeyError('{} not in {}'
                                    .format(ds_name, self.datasets))
 
         ds = self.h5[ds_name]
         ds_slice = parse_slice(ds_slice)
-        if len(ds_slice) > len(ds.shape):
-            return self._get_ds_with_repeated_values(ds, ds_name, ds_slice)
-        return ResourceDataset.extract(ds, ds_slice,
-                                       scale_attr=self.SCALE_ATTR,
-                                       add_attr=self.ADD_ATTR,
-                                       unscale=self._unscale)
-
-    def _get_ds_with_repeated_values(self, ds, ds_name, ds_slice):
-        """
-        Extract 1D data using 2D slice by repeating the 1D data along
-        the spatial or temporal dimension
-
-        Parameters
-        ----------
-        ds : h5py.dataset
-            Open .h5 dataset instance to extract data from
-        ds_name : str
-            Variable dataset to be extracted
-        ds_slice : tuple
-            Tuple of (int, slice, list, ndarray) of what to extract from ds,
-            each arg is for a sequential axis
-
-        Returns
-        -------
-        out : ndarray
-            ndarray of variable timeseries data
-            If unscale, returned in native units else in scaled units
-        """
-        ti_shape = self.shapes.get('time_index')
-        meta_shape = self.shapes.get('meta')
-        if ti_shape == meta_shape:
-            msg = ("Attempting to use a 2D slice on a 1D dataset when the "
-                   "meta and time index have the same shape - unable to "
-                   "disambiguate the slice dimensions. Please either update "
-                   "the length of the meta and/or index, set the shape of "
-                   "{!r} to be 2-dimensional (current shape: {!r}), or use a "
-                   "1-dimensional slice.".format(ds_name, ds.shape))
-            raise ResourceRuntimeError(msg)
-
-        if ds.shape == ti_shape:
-            return self._get_ds_with_spatial_repeat(ds, ds_name, ds_slice)
-        if ds.shape == meta_shape:
-            return self._get_ds_with_temporal_repeat(ds, ds_name, ds_slice)
-
-        msg = ("Attempting to use a 2D slice on a 1D dataset ({0!r}) when "
-               "the shape of the dataset {1!r} does not match the shape "
-               "of the meta {2!r})or the time index {3!r}. Please either "
-               "update the length of ({0!r}) to match either the meta or "
-               "index, or use a 1-dimensional slice."
-               .format(ds_name, ds.shape, meta_shape, ti_shape))
-        raise ResourceRuntimeError(msg)
-
-    def _get_ds_with_spatial_repeat(self, ds, ds_name, ds_slice):
-        """
-        Extract 1D data using 2D slice by repeating the 1D data along
-        the spatial dimension
-
-        Parameters
-        ----------
-        ds : h5py.dataset
-            Open .h5 dataset instance to extract data from
-        ds_name : str
-            Variable dataset to be extracted
-        ds_slice : tuple
-            Tuple of (int, slice, list, ndarray) of what to extract from ds,
-            each arg is for a sequential axis
-
-        Returns
-        -------
-        out : ndarray
-            ndarray of variable timeseries data
-            If unscale, returned in native units else in scaled units
-        """
-        msg = ("Attempting to use a 2D slice on a 1D dataset ({!r}). 1D "
-               "dataset values will be repeated along the spatial dimension"
-               .format(ds_name))
-        warn(msg)
-
-        out = ResourceDataset.extract(ds, ds_slice[:1],
-                                      scale_attr=self.SCALE_ATTR,
-                                      add_attr=self.ADD_ATTR,
-                                      unscale=self._unscale)
-        if not isinstance(out, np.ndarray):
-            out *= np.ones(self.shapes['meta'], dtype=np.float32)
-            out = out[ds_slice[1]]
-        else:
-            out = np.repeat(out[:, None], self.shapes['meta'][0], axis=1)
-            out = out[:, ds_slice[1]]
-
-        return out.astype(np.float32)
-
-    def _get_ds_with_temporal_repeat(self, ds, ds_name, ds_slice):
-        """
-        Extract 1D data using 2D slice by repeating the 1D data along
-        the temporal dimension
-
-        Parameters
-        ----------
-        ds : h5py.dataset
-            Open .h5 dataset instance to extract data from
-        ds_name : str
-            Variable dataset to be extracted
-        ds_slice : tuple
-            Tuple of (int, slice, list, ndarray) of what to extract from ds,
-            each arg is for a sequential axis
-
-        Returns
-        -------
-        out : ndarray
-            ndarray of variable timeseries data
-            If unscale, returned in native units else in scaled units
-        """
-        msg = ("Attempting to use a 2D slice on a 1D dataset ({!r}). 1D "
-               "dataset values will be repeated along the temporal dimension"
-               .format(ds_name))
-        warn(msg)
-
-        out = ResourceDataset.extract(ds, ds_slice[1:],
-                                      scale_attr=self.SCALE_ATTR,
+        out = ResourceDataset.extract(ds, ds_slice, scale_attr=self.SCALE_ATTR,
                                       add_attr=self.ADD_ATTR,
                                       unscale=self._unscale)
 
-        if not isinstance(out, np.ndarray):
-            out *= np.ones(self.shapes['time_index'], dtype=np.float32)
-        else:
-            out = np.ones((self.shapes['time_index'][0], len(out))) * out
-
-        return out[ds_slice[0]].astype(np.float32)
+        return out
 
     def close(self):
         """
         Close h5 instance
         """
         self._h5.close()
 
-    @staticmethod
-    def _preload_SAM(res, sites, tech, time_index_step=None, means=False):
+    def _preload_SAM(self, sites, tech, **kwargs):
         """
         Placeholder method to pre-load project_points for SAM
 
         Parameters
         ----------
-        res : rex.Resource
-            rex Resource handler or similar (NSRDB, WindResource,
-            MultiFileResource, etc...)
         sites : list
             List of sites to be provided to SAM
         tech : str
             Technology to be run by SAM
-        time_index_step: int, optional
-            Step size for time_index, used to reduce temporal resolution,
-            by default None
-        means : bool, optional
-            Boolean flag to compute mean resource when res_array is set,
-            by default False
-        """
-        time_slice = slice(None, None, time_index_step)
-        SAM_res = SAMResource(sites, tech, res['time_index', time_slice],
-                              means=means)
-        sites = SAM_res.sites_slice
-        SAM_res['meta'] = res['meta', sites]
-
-        SAM_res.load_rex_resource(res, SAM_res.var_list, time_slice, sites)
-
-        return SAM_res
+        kwargs : dict
+            internal kwargs
+        """
 
     @classmethod
-    def preload_SAM(cls, h5_file, sites, tech, unscale=True, str_decode=True,
-                    group=None, hsds=False, hsds_kwargs=None,
-                    time_index_step=None, means=False):
+    def preload_SAM(cls, h5_file, sites, tech, **kwargs):
         """
-        Pre-load project_points for SAM
+        Placeholder for classmethod that will pre-load project_points for SAM
 
         Parameters
         ----------
         h5_file : str
             h5_file to extract resource from
         sites : list
             List of sites to be provided to SAM
         tech : str
             Technology to be run by SAM
-        unscale : bool
-            Boolean flag to automatically unscale variables on extraction
-        str_decode : bool
-            Boolean flag to decode the bytestring meta data into normal
-            strings. Setting this to False will speed up the meta data read.
-        group : str
-            Group within .h5 resource file to open
-        hsds : bool, optional
-            Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
-            behind HSDS, by default False
-        hsds_kwargs : dict, optional
-            Dictionary of optional kwargs for h5pyd, e.g., bucket, username,
-            password, by default None
-        time_index_step: int, optional
-            Step size for time_index, used to reduce temporal resolution,
-            by default None
-        means : bool, optional
-            Boolean flag to compute mean resource when res_array is set,
-            by default False
+        kwargs : dict
+            kwargs to init resource class
+        """
 
-        Returns
-        -------
-        SAM_res : SAMResource
-            Instance of SAMResource pre-loaded with Solar resource for sites
-            in project_points
-        """
-        kwargs = {"unscale": unscale, "hsds": hsds, 'hsds_kwargs': hsds_kwargs,
-                  "str_decode": str_decode, "group": group}
-        with cls(h5_file, **kwargs) as res:
-            SAM_res = res._preload_SAM(res, sites, tech,
-                                       time_index_step=time_index_step,
-                                       means=means)
 
-        return SAM_res
+class MultiH5:
+    """
+    Class to handle multiple h5 file Resources
+    """
 
+    def __init__(self, h5_dir, prefix='', suffix='.h5'):
+        """
+        Parameters
+        ----------
+        h5_dir : str
+            Path to directory containing 5min .h5 files
+        prefix : str
+            Prefix for resource .h5 files
+        suffix : str
+            Suffix for resource .h5 files
+        """
+        self.h5_dir = h5_dir
+        self._dset_map = self._map_file_dsets(h5_dir, prefix=prefix,
+                                              suffix=suffix)
+        self._h5_map = self._map_file_instances(set(self._dset_map.values()))
 
-class Resource(BaseResource):
-    """
-    Base class to handle resource .h5 files
+        self._i = 0
 
-    Examples
-    --------
+    def __repr__(self):
+        msg = ("{} for {}:\n Contains {} files and {} datasets"
+               .format(self.__class__.__name__, self.h5_dir,
+                       len(self), len(self._dset_map)))
+        return msg
 
-    Extracting the resource's Datetime Index
+    def __len__(self):
+        return len(self._h5_map)
 
-    >>> file = '$TESTDATADIR/nsrdb/ri_100_nsrdb_2012.h5'
-    >>> with Resource(file) as res:
-    >>>     ti = res.time_index
-    >>>
-    >>> ti
-    DatetimeIndex(['2012-01-01 00:00:00', '2012-01-01 00:30:00',
-                   '2012-01-01 01:00:00', '2012-01-01 01:30:00',
-                   '2012-01-01 02:00:00', '2012-01-01 02:30:00',
-                   '2012-01-01 03:00:00', '2012-01-01 03:30:00',
-                   '2012-01-01 04:00:00', '2012-01-01 04:30:00',
-                   ...
-                   '2012-12-31 19:00:00', '2012-12-31 19:30:00',
-                   '2012-12-31 20:00:00', '2012-12-31 20:30:00',
-                   '2012-12-31 21:00:00', '2012-12-31 21:30:00',
-                   '2012-12-31 22:00:00', '2012-12-31 22:30:00',
-                   '2012-12-31 23:00:00', '2012-12-31 23:30:00'],
-                  dtype='datetime64[ns]', length=17568, freq=None)
+    def __getitem__(self, dset):
+        if dset in self:
+            path = self._dset_map[dset]
+            h5 = self._h5_map[path]
+            ds = h5[dset]
+        else:
+            raise ValueError('{} is invalid must be one of: {}'
+                             .format(dset, self.datasets))
 
-    Efficient slicing of the Datetime Index
+        return ds
 
-    >>> with Resource(file) as res:
-    >>>     ti = res['time_index', 1]
-    >>>
-    >>> ti
-    2012-01-01 00:30:00
+    def __iter__(self):
+        return self
 
-    >>> with Resource(file) as res:
-    >>>     ti = res['time_index', :10]
-    >>>
-    >>> ti
-    DatetimeIndex(['2012-01-01 00:00:00', '2012-01-01 00:30:00',
-                   '2012-01-01 01:00:00', '2012-01-01 01:30:00',
-                   '2012-01-01 02:00:00', '2012-01-01 02:30:00',
-                   '2012-01-01 03:00:00', '2012-01-01 03:30:00',
-                   '2012-01-01 04:00:00', '2012-01-01 04:30:00'],
-                  dtype='datetime64[ns]', freq=None)
+    def __next__(self):
+        if self._i >= len(self.datasets):
+            self._i = 0
+            raise StopIteration
 
-    >>> with Resource(file) as res:
-    >>>     ti = res['time_index', [1, 2, 4, 8, 9]
-    >>>
-    >>> ti
-    DatetimeIndex(['2012-01-01 00:30:00', '2012-01-01 01:00:00',
-                   '2012-01-01 02:00:00', '2012-01-01 04:00:00',
-                   '2012-01-01 04:30:00'],
-                  dtype='datetime64[ns]', freq=None)
+        dset = self.datasets[self._i]
+        self._i += 1
 
-    Extracting resource's site metadata
+        return dset
 
-    >>> with Resource(file) as res:
-    >>>     meta = res.meta
-    >>>
-    >>> meta
-            latitude  longitude   elevation  timezone    country ...
-    0      41.29     -71.86    0.000000        -5           None ...
-    1      41.29     -71.82    0.000000        -5           None ...
-    2      41.25     -71.82    0.000000        -5           None ...
-    3      41.33     -71.82   15.263158        -5  United States ...
-    4      41.37     -71.82   25.360000        -5  United States ...
-    ..       ...        ...         ...       ...            ... ...
-    95     41.25     -71.66    0.000000        -5           None ...
-    96     41.89     -71.66  153.720000        -5  United States ...
-    97     41.45     -71.66   35.440000        -5  United States ...
-    98     41.61     -71.66  140.200000        -5  United States ...
-    99     41.41     -71.66   35.160000        -5  United States ...
-    [100 rows x 10 columns]
+    def __contains__(self, dset):
+        return dset in self.datasets
 
-    Efficient slicing of the metadata
+    @property
+    def attrs(self):
+        """
+        Global .h5 file attributes sourced from first .h5 file
+        Returns
+        -------
+        attrs : dict
+            .h5 file attributes sourced from first .h5 file
+        """
+        path = self.h5_files[0]
+        attrs = dict(self._h5_map[path].attrs)
+        return attrs
 
-    >>> with Resource(file) as res:
-    >>>     meta = res['meta', 1]
-    >>>
-    >>> meta
-       latitude  longitude  elevation  timezone country state county urban ...
-    1     41.29     -71.82        0.0        -5    None  None   None  None ...
+    @property
+    def datasets(self):
+        """
+        Available datasets
+        Returns
+        -------
+        list
+            List of dataset present in .h5 files
+        """
+        return sorted(self._dset_map)
 
-    >>> with Resource(file) as res:
-    >>>     meta = res['meta', :5]
-    >>>
-    >>> meta
-       latitude  longitude  elevation  timezone        country ...
-    0     41.29     -71.86   0.000000        -5           None ...
-    1     41.29     -71.82   0.000000        -5           None ...
-    2     41.25     -71.82   0.000000        -5           None ...
-    3     41.33     -71.82  15.263158        -5  United States ...
-    4     41.37     -71.82  25.360000        -5  United States ...
+    @property
+    def h5_files(self):
+        """
+        .h5 files data is being sourced from
+        Returns
+        -------
+        list
+            List of .h5 files data is being sourced form
+        """
+        return sorted(self._h5_map)
 
-    >>> with Resource(file) as res:
-    >>>     tz = res['meta', :, 'timezone']
-    >>>
-    >>> tz
-    0    -5
-    1    -5
-    2    -5
-    3    -5
-    4    -5
-         ..
-    95   -5
-    96   -5
-    97   -5
-    98   -5
-    99   -5
-    Name: timezone, Length: 100, dtype: int64
+    @staticmethod
+    def _get_dsets(h5_path):
+        """
+        Get datasets in given .h5 file
+        Parameters
+        ----------
+        h5_path : str
+            Path to .h5 file to get variables for
+        Returns
+        -------
+        unique_dsets : list
+            List of unique datasets in .h5 file
+        shared_dsets : list
+            List of shared datasets in .h5 file
+        """
+        unique_dsets = []
+        shared_dsets = []
+        with h5py.File(h5_path, mode='r') as f:
+            for dset in f:
+                if dset not in ['meta', 'time_index', 'coordinates']:
+                    unique_dsets.append(dset)
+                else:
+                    shared_dsets.append(dset)
 
-    >>> with Resource(file) as res:
-    >>>     lat_lon = res['meta', :, ['latitude', 'longitude']]
-    >>>
-    >>> lat_lon
-        latitude  longitude
-    0      41.29     -71.86
-    1      41.29     -71.82
-    2      41.25     -71.82
-    3      41.33     -71.82
-    4      41.37     -71.82
-    ..       ...        ...
-    95     41.25     -71.66
-    96     41.89     -71.66
-    97     41.45     -71.66
-    98     41.61     -71.66
-    99     41.41     -71.66
-    [100 rows x 2 columns]
+        return unique_dsets, shared_dsets
 
-    Extracting resource variables (datasets)
+    @staticmethod
+    def _map_file_dsets(h5_dir, prefix='', suffix='.h5'):
+        """
+        Map 5min variables to their .h5 files in given directory
+        Parameters
+        ----------
+        h5_dir : str
+            Path to directory containing 5min .h5 files
+        prefix : str
+            Prefix for resource .h5 files
+        suffix : str
+            Suffix for resource .h5 files
+        Returns
+        -------
+        dset_map : dict
+            Dictionary mapping datasets to file paths
+        """
+        dset_map = {}
+        for file in sorted(os.listdir(h5_dir)):
+            if file.startswith(prefix) and file.endswith(suffix):
+                path = os.path.join(h5_dir, file)
+                unique_dsets, shared_dsets = MultiH5._get_dsets(path)
+                for dset in shared_dsets:
+                    if dset not in dset_map:
+                        dset_map[dset] = path
 
-    >>> with Resource(file) as res:
-    >>>     wspd = res['wind_speed']
-    >>>
-    >>> wspd
-    [[12. 12. 12. ... 12. 12. 12.]
-     [12. 12. 12. ... 12. 12. 12.]
-     [12. 12. 12. ... 12. 12. 12.]
-     ...
-     [14. 14. 14. ... 14. 14. 14.]
-     [15. 15. 15. ... 15. 15. 15.]
-     [15. 15. 15. ... 15. 15. 15.]]
+                for dset in unique_dsets:
+                    dset_map[dset] = path
 
-    Efficient slicing of variables
+        return dset_map
 
-    >>> with Resource(file) as res:
-    >>>     wspd = res['wind_speed', :2]
-    >>>
-    >>> wspd
-    [[12. 12. 12. 12. 12. 12. 53. 53. 53. 53. 53. 12. 53.  1.  1. 12. 12. 12.
-       1.  1. 12. 53. 53. 53. 12. 12. 12. 12. 12.  1. 12. 12.  1. 12. 12. 53.
-      12. 53.  1. 12.  1. 53. 53. 12. 12. 12. 12.  1.  1.  1. 12. 12.  1.  1.
-      12. 12. 53. 53. 53. 12. 12. 53. 53. 12. 12. 12. 12. 12. 12.  1. 53.  1.
-      53. 12. 12. 53. 53.  1.  1.  1. 53. 12.  1.  1. 53. 53. 53. 12. 12. 12.
-      12. 12. 12. 12.  1. 12.  1. 12. 12. 12.]
-     [12. 12. 12. 12. 12. 12. 53. 53. 53. 53. 53. 12. 53.  1.  1. 12. 12. 12.
-       1.  1. 12. 53. 53. 53. 12. 12. 12. 12. 12.  1. 12. 12.  1. 12. 12. 53.
-      12. 53.  1. 12.  1. 53. 53. 12. 12. 12. 12.  1.  1.  1. 12. 12.  1.  1.
-      12. 12. 53. 53. 53. 12. 12. 53. 53. 12. 12. 12. 12. 12. 12.  1. 53.  1.
-      53. 12. 12. 53. 53.  1.  1.  1. 53. 12.  1.  1. 53. 53. 53. 12. 12. 12.
-      12. 12. 12. 12.  1. 12.  1. 12. 12. 12.]]
+    @staticmethod
+    def _map_file_instances(h5_files):
+        """
+        Open all .h5 files and map the open h5py instances to the
+        associated file paths
+        Parameters
+        ----------
+        h5_files : list
+            List of .h5 files to open
+        Returns
+        -------
+        h5_map : dict
+            Dictionary mapping file paths to open resource instances
+        """
+        h5_map = {}
+        for f_path in h5_files:
+            h5_map[f_path] = h5py.File(f_path, mode='r')
 
-    >>> with Resource(file) as res:
-    >>>     wspd = res['wind_speed', :, [2, 3]]
+        return h5_map
+
+    @staticmethod
+    def multi_file_args(h5_path):
+        """
+        Get multi-h5 directory arguments for multi file resource paths.
+        Parameters
+        ----------
+        h5_path : str
+            Path to directory containing multi-file resource file sets.
+            Available formats:
+                /h5_dir/
+                /h5_dir/prefix*suffix
+        Returns
+        -------
+        h5_dir : str
+            Directory containing multi-file resource files.
+        prefix : str
+            File prefix for files in h5_dir.
+        suffix : str
+            File suffix for files in h5_dir.
+        """
+        h5_dir = h5_path
+        prefix = None
+        suffix = None
+
+        if '*' in h5_path:
+            h5_dir, fn = os.path.split(h5_path)
+            prefix, suffix = fn.split('*')
+        elif os.path.isfile(h5_path):
+            raise RuntimeError("MultiFileResource cannot handle a single file"
+                               " use Resource instead.")
+
+        return h5_dir, prefix, suffix
+
+    def close(self):
+        """
+        Close all h5py.File instances
+        """
+        for f in self._h5_map.values():
+            f.close()
+
+
+class MultiFileResource(Resource):
+    """
+    Class to handle fine spatial resolution resource data stored in
+    multiple .h5 files
+    See Also
+    --------
+    resource.Resource : Parent class
+    Examples
+    --------
+    Due to the size of the 2018 NSRDB and 5min WTK, datasets are stored in
+    multiple files. MultiFileResource and it's sub-classes allow for
+    interaction with all datasets as if they are in a single file.
+    MultiFileResource can take a directory containing all files to source
+    data from, or a filepath with a wildcard (*) indicating the filename
+    format.
+    >>> file = '$TESTDATADIR/wtk/wtk_2010_*m.h5'
+    >>> with MultiFileResource(file) as res:
+    >>>     print(self._h5_files)
+    ['$TESTDATADIR/wtk_2010_200m.h5',
+     '$TESTDATADIR/wtk_2010_100m.h5']
+    >>> file_100m = '$TESTDATADIR/wtk_2010_100m.h5'
+    >>> with Resource(file_100m) as res:
+    >>>     print(res.datasets)
+    ['coordinates', 'meta', 'pressure_100m', 'temperature_100m', 'time_index',
+     'winddirection_100m', 'windspeed_100m']
+    >>> file_200m = '$TESTDATADIR/wtk_2010_200m.h5'
+    >>> with Resource(file_200m) as res:
+    >>>     print(res.datasets)
+    ['coordinates', 'meta', 'pressure_200m', 'temperature_200m', 'time_index',
+     'winddirection_200m', 'windspeed_200m']
+    >>> with MultiFileResource(file) as res:
+    >>>     print(res.datasets)
+    ['coordinates', 'meta', 'pressure_100m', 'pressure_200m',
+     'temperature_100m', 'temperature_200m', 'time_index',
+     'winddirection_100m', 'winddirection_200m', 'windspeed_100m',
+     'windspeed_200m']
+    >>> with MultiFileResource(file) as res:
+    >>>     wspd = res['windspeed_100m']
     >>>
     >>> wspd
-    [[12. 12.]
-     [12. 12.]
-     [12. 12.]
+    [[15.13 15.17 15.21 ... 15.3  15.32 15.31]
+     [15.09 15.13 15.16 ... 15.26 15.29 15.31]
+     [15.09 15.12 15.15 ... 15.24 15.23 15.26]
      ...
-     [14. 14.]
-     [15. 15.]
-     [15. 15.]]
+     [10.29 11.08 11.51 ... 14.43 14.41 14.19]
+     [11.   11.19 11.79 ... 13.27 11.93 11.8 ]
+     [12.16 12.44 13.09 ... 11.94 10.88 11.12]]
     """
-    SCALE_ATTR = 'scale_factor'
-    ADD_ATTR = 'add_offset'
-    UNIT_ATTR = 'units'
+    PREFIX = ''
+    SUFFIX = '.h5'
 
-    def __init__(self, h5_file, unscale=True, str_decode=True, group=None,
-                 hsds=False, hsds_kwargs=None):
+    def __init__(self, h5_path, unscale=True, str_decode=True):
         """
         Parameters
         ----------
-        h5_file : str
-            Path to .h5 resource file
-        unscale : bool, optional
-            Boolean flag to automatically unscale variables on extraction,
-            by default True
-        str_decode : bool, optional
+        h5_path : str
+            Path to directory containing multi-file resource file sets.
+            Available formats:
+                /h5_dir/
+                /h5_dir/prefix*suffix
+        unscale : bool
+            Boolean flag to automatically unscale variables on extraction
+        str_decode : bool
             Boolean flag to decode the bytestring meta data into normal
-            strings. Setting this to False will speed up the meta data read,
-            by default True
-        group : str, optional
-            Group within .h5 resource file to open, by default None
-        hsds : bool, optional
-            Boolean flag to use h5pyd to handle .h5 'files' hosted on AWS
-            behind HSDS, by default False
-        hsds_kwargs : dict, optional
-            Dictionary of optional kwargs for h5pyd, e.g., bucket, username,
-            password, by default None
-        """
-        super().__init__(h5_file, unscale=unscale, str_decode=str_decode,
-                         group=group, mode='r', hsds=hsds,
-                         hsds_kwargs=hsds_kwargs)
+            strings. Setting this to False will speed up the meta data read.
+        """
+        self.h5_dir, prefix, suffix = MultiH5.multi_file_args(h5_path)
+        if prefix is None:
+            prefix = self.PREFIX
+
+        if suffix is None:
+            suffix = self.SUFFIX
+
+        self._unscale = unscale
+        self._meta = None
+        self._time_index = None
+        self._coords = None
+        self._str_decode = str_decode
+        self._group = None
+        # Map variables to their .h5 files
+        self._h5 = MultiH5(self.h5_dir, prefix=prefix, suffix=suffix)
+        self._h5_files = self._h5.h5_files
+        self.h5_file = self._h5_files[0]
+
+    def __repr__(self):
+        msg = "{} for {}".format(self.__class__.__name__, self.h5_dir)
+        return msg
```

### Comparing `NREL-rex-0.2.81/rex/resource_extraction/US_wave_cli.py` & `NREL-rex-0.2.9/rex/resource_extraction/multi_year_resource_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,207 +1,176 @@
 # -*- coding: utf-8 -*-
-# pylint: disable=all
 """
-US Wave Command Line Interface
+Multi Year ResourceX Command Line Interface
 """
 import click
 import logging
 import os
 
-from rex.resource_extraction.resource_cli import box as box_cmd
-from rex.resource_extraction.resource_cli import dataset as dataset_grp
-from rex.resource_extraction.resource_cli import multi_site as multi_site_cmd
-from rex.resource_extraction.resource_cli import region as region_cmd
-from rex.resource_extraction.resource_cli import site as site_cmd
-from rex.resource_extraction.multi_year_resource_cli \
-    import map_means as means_grp
-from rex.resource_extraction.multi_year_resource_cli \
-    import year as yr_means_cmd
-from rex.resource_extraction.multi_year_resource_cli \
-    import multi_year as multi_yr_means_cmd
-from rex.resource_extraction.resource_extraction import MultiYearWaveX
-from rex.utilities.cli_dtypes import STRLIST, INTLIST
-from rex.utilities.loggers import init_logger
-from rex import __version__
+from rex.resource_extraction.resource_cli import dataset as dataset_ctx
+from rex.resource_extraction.resource_cli import multi_site as multi_site_ctx
+from rex.resource_extraction.resource_cli import region as region_ctx
+from rex.resource_extraction.resource_cli import site as site_ctx
+from rex.resource_extraction.resource_extraction import (MultiYearResourceX,
+                                                         MultiYearNSRDBX,
+                                                         MultiYearWindX,
+                                                         MultiYearWaveX)
+from rex.utilities.cli_dtypes import STRLIST
+from rex.utilities.loggers import init_mult
 
 logger = logging.getLogger(__name__)
 
 
 @click.group()
-@click.version_option(version=__version__)
-@click.option('--domain', '-d', required=True,
-              type=click.Choice(['West_Coast', 'Hawaii'],
-                                case_sensitive=False),
-              help=('Geospatial domain to extract data from'))
+@click.option('--resource_path', '-h5', required=True,
+              type=click.Path(),
+              help=('Path to Resource .h5 files'))
 @click.option('--out_dir', '-o', required=True, type=click.Path(),
               help='Directory to dump output files')
-@click.option('--years', '-yrs', type=INTLIST, default=None,
-              show_default=True,
-              help='List of years to access, by default None')
-@click.option('--buoy', '-b', is_flag=True,
-              help="Boolean flag to use access virtual buoy data")
-@click.option('--eagle', '-hpc', is_flag=True,
-              help="Boolean flag to use access data on NRELs HPC vs. via HSDS")
-@click.option('--log_file', '-log', default=None, type=click.Path(),
-              show_default=True,
-              help='Path to .log file, if None only log to stdout')
+@click.option('--res_cls', '-res',
+              type=click.Choice(['Resource', 'NSRDB', 'Wind', 'Wave'],
+                                case_sensitive=False),
+              default='Resource',
+              help='Resource type')
 @click.option('-v', '--verbose', is_flag=True,
               help='Flag to turn on debug logging. Default is not verbose.')
 @click.pass_context
-def main(ctx, domain, out_dir, years, buoy, eagle, log_file, verbose):
+def main(ctx, resource_path, res_cls, out_dir, verbose):
     """
-    US Wave Command Line Interface
+    ResourceX Command Line Interface
     """
     ctx.ensure_object(dict)
-    if eagle:
-        path = '/datasets/US_wave/v1.0.0'
-        hsds = False
-    else:
-        path = '/nrel/US_wave'
-        hsds = True
-
-    if buoy:
-        path = os.path.join(path, 'virtual_buoy', domain)
-    else:
-        path = os.path.join(path, domain)
-
-    ctx.obj['H5'] = path
+    ctx.obj['H5'] = resource_path
+    ctx.obj['OUT_DIR'] = out_dir
+    ctx.obj['CLS_KWARGS'] = {}
 
-    if not os.path.exists(out_dir):
-        os.makedirs(out_dir)
+    if res_cls == 'Resource':
+        ctx.obj['CLS'] = MultiYearResourceX
+    elif res_cls == 'NSRDB':
+        ctx.obj['CLS'] = MultiYearNSRDBX
+    elif res_cls == 'Wind':
+        ctx.obj['CLS'] = MultiYearWindX
+    elif res_cls == 'Wave':
+        ctx.obj['CLS'] = MultiYearWaveX
+
+    name = os.path.splitext(os.path.basename(resource_path))[0]
+    init_mult(name, out_dir, verbose=verbose, node=True,
+              modules=[__name__, 'rex.resource_extraction',
+                       'rex.multi_year_resource'])
 
-    ctx.obj['OUT_DIR'] = out_dir
-    ctx.obj['CLS_KWARGS'] = {'years': years, 'hsds': hsds}
-    ctx.obj['CLS'] = MultiYearWaveX
+    logger.info('Extracting Resource data from {}'.format(resource_path))
+    logger.info('Outputs to be stored in: {}'.format(out_dir))
 
-    if verbose:
-        log_level = 'DEBUG'
-    else:
-        log_level = 'INFO'
-
-    if log_file is not None:
-        log_dir = os.path.dirname(log_file)
-        if not os.path.exists(log_dir):
-            os.makedirs(log_dir)
 
-    init_logger('rex', log_file=log_file, log_level=log_level)
+@main.command()
+@click.option('--year', '-yr', type=str, required=True,
+              help='Year to average')
+@click.option('--dataset', '-d', type=str, required=True,
+              help='Dataset to extract')
+@click.option('--region_col', '-col', type=str, default='state',
+              help='Meta column to search for region')
+@click.option('--region', '-r', type=str, default=None,
+              help='Region to extract')
+@click.pass_context
+def year(ctx, year, dataset, region_col, region):
+    """
+    Average a single dataset for a given year
+    Extract only pixels in region if given.
+    """
+    with ctx.obj['CLS'](ctx.obj['H5'], **ctx.obj['CLS_KWARGS']) as f:
+        map_df = f.get_means_map(dataset, year, region=region,
+                                 region_col=region_col)
 
-    logger.info('Extracting US wave data for {} from {}'.format(domain, path))
-    logger.info('Outputs to be stored in: {}'.format(out_dir))
+    out_path = "{}-{}.csv".format(dataset, year)
+    out_path = os.path.join(ctx.obj['OUT_DIR'], out_path)
+    logger.info('Saving data to {}'.format(out_path))
+    map_df.to_csv(out_path)
 
 
-@main.group()
+@main.command()
+@click.option('--years', '-yrs', type=STRLIST, required=True,
+              help='List of Years to average')
 @click.option('--dataset', '-d', type=str, required=True,
               help='Dataset to extract')
+@click.option('--region_col', '-col', type=str, default='state',
+              help='Meta column to search for region')
+@click.option('--region', '-r', type=str, default=None,
+              help='Region to extract')
 @click.pass_context
-def dataset(ctx, dataset):
+def years(ctx, years, dataset, region_col, region):
     """
-    Extract a single dataset
+    Average a single dataset for a given years
+    Extract only pixels in region if given.
     """
-    ctx.invoke(dataset_grp, dataset=dataset)
+    with ctx.obj['CLS'](ctx.obj['H5'], **ctx.obj['CLS_KWARGS']) as f:
+        map_df = f.get_means_map(dataset, years, region=region,
+                                 region_col=region_col)
 
+    out_path = "{}_{}-{}.csv".format(dataset, years[0], years[-1])
+    out_path = os.path.join(ctx.obj['OUT_DIR'], out_path)
+    logger.info('Saving data to {}'.format(out_path))
+    map_df.to_csv(out_path)
 
-@dataset.command()
-@click.option('--lat_lon', '-ll', nargs=2, type=float,
-              default=None, show_default=True,
+
+@main.command()
+@click.option('--dataset', '-d', type=str, required=True,
+              help='Dataset to extract')
+@click.option('--lat_lon', '-ll', nargs=2, type=click.Tuple([float, float]),
+              default=None,
               help='(lat, lon) coordinates of interest')
-@click.option('--gid', '-gid', type=int, default=None, show_default=True,
+@click.option('--gid', '-g', type=int, default=None,
               help='Resource gid of interest')
 @click.pass_context
-def site(ctx, lat_lon, gid):
+def site(ctx, dataset, lat_lon, gid):
     """
-    Extract the nearest pixel to the given (lat, lon) coordinates
-    OR the given resource gid
+    Extract a single dataset for the nearest pixel to the given (lat, lon)
+    coordinates OR the given resource gid
     """
-    ctx.invoke(site_cmd, lat_lon=lat_lon, gid=gid)
+    ctx.invoke(site_ctx, dataset=dataset, lat_lon=lat_lon, gid=gid)
 
 
-@dataset.command()
+@main.command()
+@click.option('--dataset', '-d', type=str, required=True,
+              help='Dataset to extract')
 @click.option('--region', '-r', type=str, required=True,
               help='Region to extract')
 @click.option('--region_col', '-col', type=str, default='state',
               help='Meta column to search for region')
-@click.option('--timestep', '-ts', type=str, default=None,
-              help='Timestep to extract')
-@click.pass_context
-def region(ctx, region, region_col, timestep):
-    """
-    Extract a single dataset for all gids in the given region
-    """
-    ctx.invoke(region_cmd, region=region, region_col=region_col,
-               timestep=timestep)
-
-
-@dataset.command()
-@click.option('--lat_lon_1', '-ll1', nargs=2, type=float,
-              required=True,
-              help='One corner of the bounding box')
-@click.option('--lat_lon_2', '-ll2', nargs=2, type=float,
-              required=True,
-              help='The other corner of the bounding box')
-@click.option('--timestep', '-ts', type=str, default=None, show_default=True,
-              help='Timestep to extract')
-@click.option('--file_suffix', '-fs', default=None, show_default=True,
-              help='File name suffix')
 @click.pass_context
-def box(ctx, lat_lon_1, lat_lon_2, timestep, file_suffix):
+def region(ctx, dataset, region, region_col):
     """
-    Extract all pixels in the given bounding box
+    Extract a single dataset for all pixels in the given region
     """
-    ctx.invoke(box_cmd, lat_lon_1=lat_lon_1, lat_lon_2=lat_lon_2,
-               file_suffix=file_suffix, timestep=timestep)
+    ctx.invoke(region_ctx, dataset=dataset, region=region,
+               region_col=region_col)
 
 
-@dataset.command()
+@main.group()
 @click.option('--sites', '-s', type=click.Path(exists=True), required=True,
               help=('.csv or .json file with columns "latitude", "longitude" '
                     'OR "gid"'))
 @click.pass_context
 def multi_site(ctx, sites):
     """
     Extract multiple sites given in '--sites' .csv or .json as
     "latitude", "longitude" pairs OR "gid"s
     """
-    ctx.invoke(multi_site_cmd, sites=sites)
-
+    ctx.invoke(multi_site_ctx, sites=sites)
 
-@dataset.group()
-@click.option('--region', '-r', type=str, default=None, show_default=True,
-              help='Region to extract')
-@click.option('--region_col', '-col', type=str, default='state',
-              show_default=True,
-              help='Meta column to search for region')
-def map_means(ctx, region, region_col):
-    """
-    Map means for given dataset in region if given.
-    """
-    ctx.invoke(means_grp, region=region, region_col=region_col)
 
-
-@map_means.command()
-@click.option('--year', '-yr', type=str, required=True,
-              help='Year to average')
-@click.pass_context
-def year(ctx, year):
-    """
-    Map means for a given year
-    """
-    ctx.invoke(yr_means_cmd, year=year)
-
-
-@map_means.command()
-@click.option('--years', '-yrs', type=STRLIST, required=True,
-              help='List of Years to average')
+@multi_site.command()
+@click.option('--dataset', '-d', type=str, required=True,
+              help='Dataset to extract')
 @click.pass_context
-def multi_year(ctx, years):
+def dataset(ctx, dataset):
     """
-    Map means for a given year
+    Extract given dataset for all sites
     """
-    ctx.invoke(multi_yr_means_cmd, years=years)
+    ctx.invoke(dataset_ctx, dataset=dataset)
 
 
 if __name__ == '__main__':
     try:
         main(obj={})
     except Exception:
-        logger.exception('Error running US_wave CLI')
+        logger.exception('Error running MultiYearResourceX CLI')
         raise
```

### Comparing `NREL-rex-0.2.81/rex/resource_extraction/multi_year_resource_cli.py` & `NREL-rex-0.2.9/rex/resource_extraction/resource_cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,236 +1,272 @@
 # -*- coding: utf-8 -*-
-# pylint: disable=all
 """
-Multi Year ResourceX Command Line Interface
+ResourceX Command Line Interface
 """
 import click
 import logging
 import os
+import pandas as pd
 
-from rex.resource_extraction.resource_cli import box as box_cmd
-from rex.resource_extraction.resource_cli import dataset as dataset_grp
-from rex.resource_extraction.resource_cli import multi_site as multi_site_cmd
-from rex.resource_extraction.resource_cli import region as region_cmd
-from rex.resource_extraction.resource_cli import site as site_cmd
-from rex.resource_extraction.resource_extraction import (MultiYearResourceX,
-                                                         MultiYearNSRDBX,
-                                                         MultiYearWindX,
-                                                         MultiYearWaveX)
-from rex.utilities.cli_dtypes import STRLIST, INTLIST
-from rex.utilities.loggers import init_logger
-from rex import __version__
+from rex.resource_extraction.resource_extraction import (ResourceX,
+                                                         MultiFileResourceX)
+from rex.utilities.loggers import init_mult
+from rex.utilities.utilities import check_res_file
 
 logger = logging.getLogger(__name__)
 
 
 @click.group()
-@click.version_option(version=__version__)
-@click.option('--resource_path', '-h5', required=True,
+@click.option('--resource_h5', '-h5', required=True,
               type=click.Path(),
-              help=('Path to Resource .h5 files'))
+              help=('Path to Resource .h5 file'))
 @click.option('--out_dir', '-o', required=True, type=click.Path(),
               help='Directory to dump output files')
-@click.option('--years', '-yrs', type=INTLIST, default=None,
-              show_default=True,
-              help='List of years to access, by default None')
-@click.option('--hsds', '-hsds', is_flag=True,
-              help=("Boolean flag to use h5pyd to handle .h5 'files' hosted "
-                    "on AWS behind HSDS"))
-@click.option('--res_cls', '-res',
-              type=click.Choice(['Resource', 'NSRDB', 'Wind', 'Wave'],
-                                case_sensitive=False),
-              default='Resource', show_default=True,
-              help='Resource type')
-@click.option('--log_file', '-log', default=None, type=click.Path(),
-              show_default=True,
-              help='Path to .log file, if None only log to stdout')
 @click.option('-v', '--verbose', is_flag=True,
               help='Flag to turn on debug logging. Default is not verbose.')
 @click.pass_context
-def main(ctx, resource_path, out_dir, years, hsds, res_cls, log_file,
-         verbose):
+def main(ctx, resource_h5, out_dir, verbose):
     """
-    Multi-year ResourceX Command Line Interface
+    ResourceX Command Line Interface
     """
     ctx.ensure_object(dict)
-    ctx.obj['H5'] = resource_path
+    ctx.obj['H5'] = resource_h5
     ctx.obj['OUT_DIR'] = out_dir
-    ctx.obj['CLS_KWARGS'] = {'years': years, 'hsds': hsds}
+    ctx.obj['CLS_KWARGS'] = {}
 
-    if res_cls == 'Resource':
-        ctx.obj['CLS'] = MultiYearResourceX
-    elif res_cls == 'NSRDB':
-        ctx.obj['CLS'] = MultiYearNSRDBX
-    elif res_cls == 'Wind':
-        ctx.obj['CLS'] = MultiYearWindX
-    elif res_cls == 'Wave':
-        ctx.obj['CLS'] = MultiYearWaveX
-
-    if verbose:
-        log_level = 'DEBUG'
+    multi_h5_res, hsds = check_res_file(resource_h5)
+    if multi_h5_res:
+        assert os.path.exists(os.path.dirname(resource_h5))
+        ctx.obj['CLS'] = MultiFileResourceX
     else:
-        log_level = 'INFO'
-
-    if log_file is not None:
-        log_dir = os.path.dirname(log_file)
-        if not os.path.exists(log_dir):
-            os.makedirs(log_dir)
+        if hsds:
+            ctx.obj['CLS_KWARGS']['hsds'] = hsds
+        else:
+            assert os.path.exists(resource_h5)
+
+        ctx.obj['CLS'] = ResourceX
+
+    name = os.path.splitext(os.path.basename(resource_h5))[0]
+    init_mult(name, out_dir, verbose=verbose, node=True,
+              modules=[__name__, 'rex.resource_extraction',
+                       'rex.resource'])
 
-    init_logger('rex', log_file=log_file, log_level=log_level)
-
-    logger.info('Extracting Resource data from {}'.format(resource_path))
+    logger.info('Extracting Resource data from {}'.format(resource_h5))
     logger.info('Outputs to be stored in: {}'.format(out_dir))
 
 
-@main.group()
-@click.option('--dataset', '-d', type=str, required=True,
-              help='Dataset to extract')
+@main.command()
+@click.option('--lat_lon', '-ll', nargs=2, type=click.Tuple([float, float]),
+              default=None,
+              help='(lat, lon) coordinates of interest')
+@click.option('--gid', '-g', type=int, default=None,
+              help='Resource gid of interest')
 @click.pass_context
-def dataset(ctx, dataset):
+def sam_file(ctx, lat_lon, gid):
     """
-    Extract a single dataset
+    Extract all datasets needed for SAM for the nearest pixel to the given
+    (lat, lon) coordinates OR the given resource gid
     """
-    ctx.invoke(dataset_grp, dataset=dataset)
+    if lat_lon is None and gid is None:
+        click.echo("Must supply '--lat-lon' OR '--gid'!")
+        raise click.Abort()
+    elif lat_lon and gid:
+        click.echo("You must only supply '--lat-lon' OR '--gid'!")
+        raise click.Abort()
+
+    logger.info('Saving data to {}'.format(ctx.obj['OUT_DIR']))
+    with ctx.obj['CLS'](ctx.obj['H5'], **ctx.obj['CLS_KWARGS']) as f:
+        if lat_lon is not None:
+            f.get_SAM_lat_lon(lat_lon, out_path=ctx.obj['OUT_DIR'])
+        elif gid is not None:
+            gid = f._get_nearest(lat_lon)
+            f.get_SAM_gid(gid, out_path=ctx.obj['OUT_DIR'])
 
 
-@dataset.command()
-@click.option('--lat_lon', '-ll', nargs=2, type=float,
-              default=None, show_default=True,
+@main.command()
+@click.option('--dataset', '-d', type=str, required=True,
+              help='Dataset to extract')
+@click.option('--lat_lon', '-ll', nargs=2, type=click.Tuple([float, float]),
+              default=None,
               help='(lat, lon) coordinates of interest')
-@click.option('--gid', '-gid', type=int, default=None, show_default=True,
+@click.option('--gid', '-g', type=int, default=None,
               help='Resource gid of interest')
 @click.pass_context
-def site(ctx, lat_lon, gid):
+def site(ctx, dataset, lat_lon, gid):
     """
-    Extract the nearest pixel to the given (lat, lon) coordinates
-    OR the given resource gid
+    Extract a single dataset for the nearest pixel to the given (lat, lon)
+    coordinates OR the given resource gid
     """
-    ctx.invoke(site_cmd, lat_lon=lat_lon, gid=gid)
+    if lat_lon is None and gid is None:
+        click.echo("Must supply '--lat-lon' OR '--gid'!")
+        raise click.Abort()
+    elif lat_lon and gid:
+        click.echo("You must only supply '--lat-lon' OR '--gid'!")
+        raise click.Abort()
+
+    with ctx.obj['CLS'](ctx.obj['H5'], **ctx.obj['CLS_KWARGS']) as f:
+        if lat_lon is not None:
+            site_df = f.get_lat_lon_df(dataset, lat_lon)
+        elif gid is not None:
+            site_df = f.get_gid_df(dataset, gid)
 
+    gid = site_df.name
+    out_path = "{}-{}.csv".format(dataset, gid)
+    out_path = os.path.join(ctx.obj['OUT_DIR'], out_path)
+    logger.info('Saving data to {}'.format(out_path))
+    site_df.to_csv(out_path)
 
-@dataset.command()
+
+@main.command()
+@click.option('--dataset', '-d', type=str, required=True,
+              help='Dataset to extract')
 @click.option('--region', '-r', type=str, required=True,
               help='Region to extract')
 @click.option('--region_col', '-col', type=str, default='state',
-              show_default=True,
               help='Meta column to search for region')
-@click.option('--timestep', '-ts', type=str, default=None,
-              show_default=True,
-              help='Timestep to extract')
 @click.pass_context
-def region(ctx, region, region_col, timestep):
+def region(ctx, dataset, region, region_col):
     """
-    Extract a single dataset for all gids in the given region
+    Extract a single dataset for all pixels in the given region
     """
-    ctx.invoke(region_cmd, region=region, region_col=region_col,
-               timestep=timestep)
+    with ctx.obj['CLS'](ctx.obj['H5'], **ctx.obj['CLS_KWARGS']) as f:
+        region_df = f.get_region_df(dataset, region, region_col=region_col)
+        meta = f['meta']
+
+    out_path = "{}-{}.csv".format(dataset, region)
+    out_path = os.path.join(ctx.obj['OUT_DIR'], out_path)
+    logger.info('Saving data to {}'.format(out_path))
+    region_df.to_csv(out_path)
+
+    out_path = "{}-meta.csv".format(region)
+    out_path = os.path.join(ctx.obj['OUT_DIR'], out_path)
+    meta = meta.loc[region_df.columns]
+    meta.index.name = 'gid'
+    logger.info('Saving meta data to {}'.format(out_path))
+    meta.to_csv(out_path)
 
 
-@dataset.command()
-@click.option('--lat_lon_1', '-ll1', nargs=2, type=float,
-              required=True,
-              help='One corner of the bounding box')
-@click.option('--lat_lon_2', '-ll2', nargs=2, type=float,
-              required=True,
-              help='The other corner of the bounding box')
-@click.option('--file_suffix', '-fs', default=None,
-              show_default=True,
-              help='File name suffix')
-@click.option('--timestep', '-ts', type=str, default=None,
-              show_default=True,
+@main.command()
+@click.option('--timestep', '-ts', type=str, required=True,
               help='Timestep to extract')
+@click.option('--dataset', '-d', type=str, required=True,
+              help='Dataset to extract')
+@click.option('--region_col', '-col', type=str, default='state',
+              help='Meta column to search for region')
+@click.option('--region', '-r', type=str, default=None,
+              help='Region to extract')
 @click.pass_context
-def box(ctx, lat_lon_1, lat_lon_2, file_suffix, timestep):
+def timestep(ctx, timestep, dataset, region_col, region):
     """
-    Extract all pixels in the given bounding box
+    Extract a single dataset for a single timestep
+    Extract only pixels in region if given.
     """
-    ctx.invoke(box_cmd, lat_lon_1=lat_lon_1, lat_lon_2=lat_lon_2,
-               file_suffix=file_suffix, timestep=timestep)
+    with ctx.obj['CLS'](ctx.obj['H5'], **ctx.obj['CLS_KWARGS']) as f:
+        map_df = f.get_timestep_map(dataset, timestep, region=region,
+                                    region_col=region_col)
+
+    out_path = "{}-{}.csv".format(dataset, timestep)
+    out_path = os.path.join(ctx.obj['OUT_DIR'], out_path)
+    logger.info('Saving data to {}'.format(out_path))
+    map_df.to_csv(out_path)
 
 
-@dataset.command()
+@main.group()
 @click.option('--sites', '-s', type=click.Path(exists=True), required=True,
               help=('.csv or .json file with columns "latitude", "longitude" '
                     'OR "gid"'))
 @click.pass_context
 def multi_site(ctx, sites):
     """
     Extract multiple sites given in '--sites' .csv or .json as
     "latitude", "longitude" pairs OR "gid"s
     """
-    ctx.invoke(multi_site_cmd, sites=sites)
-
-
-@dataset.group(invoke_without_command=True)
-@click.option('--region', '-r', type=str, default=None,
-              show_default=True,
-              help='Region to extract')
-@click.option('--region_col', '-col', type=str, default='state',
-              show_default=True,
-              help='Meta column to search for region')
-def map_means(ctx, region, region_col):
-    """
-    Map temporal means for given dataset in region if given.
-    """
-    logger = ctx.obj["LOGGER"]
-    if ctx.invoked_subcommand is None:
-        with ctx.obj['CLS'](ctx.obj['H5'], **ctx.obj['CLS_KWARGS']) as f:
-            map_df = f.get_means_map(ctx.obj["DATASET"], year=None,
-                                     region=region,
-                                     region_col=region_col)
+    name = os.path.splitext(os.path.basename(sites))[0]
+    ctx.obj['NAME'] = name
+    if sites.endswith('.csv'):
+        sites = pd.read_csv(sites)
+    elif sites.endswith('.json'):
+        sites = pd.read_json(sites)
+    else:
+        click.echo("'--sites' must be a .csv or .json file!")
+        click.Abort()
 
-        out_path = "{}-means.csv".format(dataset)
-        out_path = os.path.join(ctx.obj['OUT_DIR'], out_path)
-        logger.info('Saving data to {}'.format(out_path))
-        map_df.to_csv(out_path)
+    if 'gid' in sites:
+        ctx.obj['GID'] = sites['gid'].values
+        ctx.obj['LAT_LON'] = None
+    elif 'latitude' in sites and 'longitude' in sites:
+        ctx.obj['GID'] = None
+        ctx.obj['LAT_LON'] = sites[['latitude', 'longitude']].values
     else:
-        ctx.obj['REGION'] = region
-        ctx.obj['REGION_COL'] = region_col
+        click.echo('Must supply site "gid"s or "latitude" and "longitude" '
+                   'as columns in "--sites" file')
 
 
-@map_means.command()
-@click.option('--year', '-yr', type=str, required=True,
-              help='Year to average')
+@multi_site.command()
+@click.option('--dataset', '-d', type=str, required=True,
+              help='Dataset to extract')
 @click.pass_context
-def year(ctx, year):
+def dataset(ctx, dataset):
     """
-    Map means for a given year
+    Extract given dataset for all sites
     """
-    logger = ctx.obj["LOGGER"]
+    gid = ctx.obj['GID']
+    lat_lon = ctx.obj['LAT_LON']
     with ctx.obj['CLS'](ctx.obj['H5'], **ctx.obj['CLS_KWARGS']) as f:
-        map_df = f.get_means_map(ctx.obj["DATASET"], year=year,
-                                 region=ctx.obj['REGION'],
-                                 region_col=ctx.obj["REGION_COL"])
+        meta = f['meta']
+        if lat_lon is not None:
+            site_df = f.get_lat_lon_df(dataset, lat_lon)
+        elif gid is not None:
+            site_df = f.get_gid_df(dataset, gid)
 
-    out_path = "{}-{}.csv".format(dataset, year)
+    name = ctx.obj['NAME']
+    out_path = "{}-{}.csv".format(dataset, name)
     out_path = os.path.join(ctx.obj['OUT_DIR'], out_path)
     logger.info('Saving data to {}'.format(out_path))
-    map_df.to_csv(out_path)
+    site_df.to_csv(out_path)
+
+    out_path = "{}-meta.csv".format(name)
+    out_path = os.path.join(ctx.obj['OUT_DIR'], out_path)
+    meta = meta.loc[site_df.columns]
+    meta.index.name = 'gid'
+    logger.info('Saving meta data to {}'.format(out_path))
+    meta.to_csv(out_path)
 
 
-@map_means.command()
-@click.option('--years', '-yrs', type=STRLIST, required=True,
-              help='List of Years to average')
+@multi_site.command()
 @click.pass_context
-def multi_year(ctx, years):
+def sam(ctx):
     """
-    Map means for a given subset of years
+    Extract SAM variables
     """
-    logger = ctx.obj["LOGGER"]
+    gid = ctx.obj['GID']
+    lat_lon = ctx.obj['LAT_LON']
     with ctx.obj['CLS'](ctx.obj['H5'], **ctx.obj['CLS_KWARGS']) as f:
-        map_df = f.get_means_map(ctx.obj["DATASET"], year=years,
-                                 region=ctx.obj['REGION'],
-                                 region_col=ctx.obj["REGION_COL"])
+        meta = f['meta']
+        if lat_lon is not None:
+            SAM_df = f.get_SAM_lat_lon(lat_lon)
+        elif gid is not None:
+            SAM_df = f.get_SAM_gid(gid)
+
+    name = ctx.obj['NAME']
+    gids = []
+    for df in SAM_df:
+        gids.append(int(df.name.split('-')[-1]))
+        out_path = "{}-{}.csv".format(df.name, name)
+        out_path = os.path.join(ctx.obj['OUT_DIR'], out_path)
+        logger.info('Saving data to {}'.format(out_path))
+        df.to_csv(out_path)
 
-    out_path = "{}_{}-{}.csv".format(dataset, years[0], years[-1])
+    out_path = "{}-meta.csv".format(name)
     out_path = os.path.join(ctx.obj['OUT_DIR'], out_path)
-    logger.info('Saving data to {}'.format(out_path))
-    map_df.to_csv(out_path)
+    meta = meta.loc[gids]
+    meta.index.name = 'gid'
+    logger.info('Saving meta data to {}'.format(out_path))
+    meta.to_csv(out_path)
 
 
 if __name__ == '__main__':
     try:
         main(obj={})
     except Exception:
-        logger.exception('Error running MultiYearResourceX CLI')
+        logger.exception('Error running ResourceX CLI')
         raise
```

### Comparing `NREL-rex-0.2.81/rex/resource_extraction/nsrdb_cli.py` & `NREL-rex-0.2.9/rex/resource_extraction/nsrdb_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,182 +1,170 @@
 # -*- coding: utf-8 -*-
-# pylint: disable=all
 """
 NSRDBX Command Line Interface
 """
 import click
 import logging
 import os
 
 from rex.resource_extraction.resource_extraction import (NSRDBX, SolarX,
                                                          MultiFileNSRDBX)
-from rex.resource_extraction.resource_cli import box as box_cmd
-from rex.resource_extraction.resource_cli import dataset as dataset_grp
-from rex.resource_extraction.resource_cli import multi_site as multi_site_cmd
+from rex.resource_extraction.resource_cli import dataset as dataset_cmd
+from rex.resource_extraction.resource_cli import multi_site as multi_site_grp
 from rex.resource_extraction.resource_cli import region as region_cmd
-from rex.resource_extraction.resource_cli import sam_datasets as sam_cmd
+from rex.resource_extraction.resource_cli import sam as sam_cmd
+from rex.resource_extraction.resource_cli import sam_file as sam_file_cmd
 from rex.resource_extraction.resource_cli import site as site_cmd
-from rex.utilities.loggers import init_logger
+from rex.resource_extraction.resource_cli import timestep as timestep_cmd
+from rex.utilities.loggers import init_mult
 from rex.utilities.utilities import check_res_file
-from rex import __version__
 
 logger = logging.getLogger(__name__)
 
 
 @click.group()
-@click.version_option(version=__version__)
 @click.option('--solar_h5', '-h5', required=True,
               type=click.Path(),
               help=('Path to Resource .h5 file'))
 @click.option('--out_dir', '-o', required=True, type=click.Path(exists=True),
               help='Directory to dump output files')
-@click.option('--log_file', '-log', default=None, type=click.Path(),
-              show_default=True,
-              help='Path to .log file, if None only log to stdout')
 @click.option('-v', '--verbose', is_flag=True,
               help='Flag to turn on debug logging. Default is not verbose.')
 @click.pass_context
-def main(ctx, solar_h5, out_dir, log_file, verbose):
+def main(ctx, solar_h5, out_dir, verbose):
     """
     NSRDBX Command Line Interface
     """
     ctx.ensure_object(dict)
-    if not os.path.exists(out_dir):
-        os.makedirs(out_dir)
-
     ctx.obj['H5'] = solar_h5
     ctx.obj['OUT_DIR'] = out_dir
     ctx.obj['CLS_KWARGS'] = {}
 
     multi_h5_res, hsds = check_res_file(solar_h5)
     name = os.path.splitext(os.path.basename(solar_h5))[0]
-    if 'nsrdb' in name:
-        ctx.obj['CLS'] = NSRDBX
-    else:
-        ctx.obj['CLS'] = SolarX
-
-    if multi_h5_res and not hsds:
+    if multi_h5_res:
         assert os.path.exists(os.path.dirname(solar_h5))
         ctx.obj['CLS'] = MultiFileNSRDBX
-    elif hsds:
-        ctx.obj['CLS_KWARGS']['hsds'] = hsds
     else:
-        assert os.path.exists(solar_h5)
-
-    if verbose:
-        log_level = 'DEBUG'
-    else:
-        log_level = 'INFO'
-
-    if log_file is not None:
-        log_dir = os.path.dirname(log_file)
-        if not os.path.exists(log_dir):
-            os.makedirs(log_dir)
-
-    init_logger('rex', log_file=log_file, log_level=log_level)
+        if hsds:
+            ctx.obj['CLS_KWARGS']['hsds'] = hsds
+        else:
+            assert os.path.exists(solar_h5)
+
+        if 'nsrdb' in name:
+            ctx.obj['CLS'] = NSRDBX
+        else:
+            ctx.obj['CLS'] = SolarX
+
+    init_mult(name, out_dir, verbose=verbose, node=True,
+              modules=[__name__, 'rex.resource_extraction',
+                       'rex.renewable_resource'])
 
     logger.info('Extracting solar data from {}'.format(solar_h5))
     logger.info('Outputs to be stored in: {}'.format(out_dir))
 
 
 @main.command()
-@click.option('--lat_lon', '-ll', nargs=2, type=float,
-              default=None, show_default=True,
+@click.option('--lat_lon', '-ll', nargs=2, type=click.Tuple([float, float]),
+              default=None,
               help='(lat, lon) coordinates of interest')
-@click.option('--gid', '-gid', type=int, default=None,
-              show_default=True,
+@click.option('--gid', '-g', type=int, default=None,
               help='Resource gid of interest')
-@click.option('--sites', '-s', type=click.Path(exists=True), default=None,
-              show_default=True,
-              help=('.csv or .json file with columns "latitude", "longitude" '
-                    'OR "gid"'))
 @click.pass_context
-def sam_datasets(ctx, lat_lon, gid, sites):
+def sam_file(ctx, lat_lon, gid):
     """
-    Extract all datasets needed for SAM for the nearest pixel(s) to the given
-    (lat, lon) coordinates, the given resource gid, or the give sites
+    Extract all datasets needed for SAM for the nearest pixel to the given
+    (lat, lon) coordinates OR the given resource gid
     """
-    ctx.invoke(sam_cmd, lat_lon=lat_lon, gid=gid, sites=sites)
+    ctx.invoke(sam_file_cmd, lat_lon=lat_lon, gid=gid)
 
 
-@main.group()
+@main.command()
 @click.option('--dataset', '-d', type=str, required=True,
               help='Dataset to extract')
-@click.pass_context
-def dataset(ctx, dataset):
-    """
-    Extract a single dataset
-    """
-    ctx.invoke(dataset_grp, dataset=dataset)
-
-
-@dataset.command()
-@click.option('--lat_lon', '-ll', nargs=2, type=float,
-              default=None, show_default=True,
+@click.option('--lat_lon', '-ll', nargs=2, type=click.Tuple([float, float]),
+              default=None,
               help='(lat, lon) coordinates of interest')
-@click.option('--gid', '-gid', type=int, default=None, show_default=True,
+@click.option('--gid', '-g', type=int, default=None,
               help='Resource gid of interest')
 @click.pass_context
-def site(ctx, lat_lon, gid):
+def site(ctx, dataset, lat_lon, gid):
     """
-    Extract the nearest pixel to the given (lat, lon) coordinates OR the given
-    resource gid
+    Extract a single dataset for the nearest pixel to the given (lat, lon)
+    coordinates OR the given resource gid
     """
-    ctx.invoke(site_cmd, lat_lon=lat_lon, gid=gid)
+    ctx.invoke(site_cmd, dataset=dataset, lat_lon=lat_lon, gid=gid)
 
 
-@dataset.command()
+@main.command()
+@click.option('--dataset', '-d', type=str, required=True,
+              help='Dataset to extract')
 @click.option('--region', '-r', type=str, required=True,
               help='Region to extract')
 @click.option('--region_col', '-col', type=str, default='state',
-              show_default=True,
               help='Meta column to search for region')
-@click.option('--timestep', '-ts', type=str, default=None,
-              show_default=True,
-              help='Timestep to extract')
 @click.pass_context
-def region(ctx, region, region_col, timestep):
+def region(ctx, dataset, region, region_col):
     """
     Extract a single dataset for all pixels in the given region
     """
-    ctx.invoke(region_cmd, region=region, region_col=region_col,
-               timestep=timestep)
+    ctx.invoke(region_cmd, dataset=dataset, region=region,
+               region_col=region_col)
 
 
-@dataset.command()
-@click.option('--lat_lon_1', '-ll1', nargs=2, type=float,
-              required=True,
-              help='One corner of the bounding box')
-@click.option('--lat_lon_2', '-ll2', nargs=2, type=float,
-              required=True,
-              help='The other corner of the bounding box')
-@click.option('--file_suffix', '-fs', default=None, show_default=True,
-              help='Filename suffix')
-@click.option('--timestep', '-ts', type=str, default=None, show_default=True,
+@main.command()
+@click.option('--timestep', '-ts', type=str, required=True,
               help='Timestep to extract')
+@click.option('--dataset', '-d', type=str, required=True,
+              help='Dataset to extract')
+@click.option('--region', '-r', type=str, default=None,
+              help='Region to extract')
+@click.option('--region_col', '-col', type=str, default='state',
+              help='Meta column to search for region')
 @click.pass_context
-def box(ctx, lat_lon_1, lat_lon_2, file_suffix, timestep):
+def timestep(ctx, timestep, dataset, region, region_col):
     """
-    Extract all gids in the given bounding box
+    Extract a single dataset for a single timestep
+    Extract only pixels in region if given.
     """
-    ctx.invoke(box_cmd, lat_lon_1=lat_lon_1, lat_lon_2=lat_lon_2,
-               file_suffix=file_suffix, timestep=timestep)
+    ctx.invoke(timestep_cmd, dataset=dataset, timestep=timestep,
+               region=region, region_col=region_col)
 
 
-@dataset.command()
+@main.group()
 @click.option('--sites', '-s', type=click.Path(exists=True), required=True,
               help=('.csv or .json file with columns "latitude", "longitude" '
                     'OR "gid"'))
 @click.pass_context
 def multi_site(ctx, sites):
     """
     Extract multiple sites given in '--sites' .csv or .json as
     "latitude", "longitude" pairs OR "gid"s
     """
-    ctx.invoke(multi_site_cmd, sites=sites)
+    ctx.invoke(multi_site_grp, sites=sites)
+
+
+@multi_site.command()
+@click.option('--dataset', '-d', type=str, required=True,
+              help='Dataset to extract')
+@click.pass_context
+def dataset(ctx, dataset):
+    """
+    Extract given dataset for all sites
+    """
+    ctx.invoke(dataset_cmd, dataset=dataset)
+
+
+@multi_site.command()
+@click.pass_context
+def sam(ctx):
+    """
+    Extract SAM variables
+    """
+    ctx.invoke(sam_cmd)
 
 
 if __name__ == '__main__':
     try:
         main(obj={})
     except Exception:
         logger.exception('Error running NSRDBX CLI')
```

### Comparing `NREL-rex-0.2.81/rex/resource_extraction/wave_cli.py` & `NREL-rex-0.2.9/rex/resource_extraction/wave_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,170 +1,161 @@
 # -*- coding: utf-8 -*-
-# pylint: disable=all
 """
 WaveX Command Line Interface
 """
 import click
 import logging
 import os
 
 from rex.resource_extraction.resource_extraction import WaveX
-from rex.resource_extraction.resource_cli import box as box_cmd
-from rex.resource_extraction.resource_cli import dataset as dataset_grp
-from rex.resource_extraction.resource_cli import multi_site as multi_site_cmd
+from rex.resource_extraction.resource_cli import dataset as dataset_cmd
+from rex.resource_extraction.resource_cli import multi_site as multi_site_grp
 from rex.resource_extraction.resource_cli import region as region_cmd
-from rex.resource_extraction.resource_cli import sam_datasets as sam_cmd
+from rex.resource_extraction.resource_cli import sam as sam_cmd
+from rex.resource_extraction.resource_cli import sam_file as sam_file_cmd
 from rex.resource_extraction.resource_cli import site as site_cmd
-from rex.utilities.loggers import init_logger
+from rex.resource_extraction.resource_cli import timestep as timestep_cmd
+from rex.utilities.loggers import init_mult
 from rex.utilities.utilities import check_res_file
-from rex import __version__
 
 logger = logging.getLogger(__name__)
 
 
 @click.group()
-@click.version_option(version=__version__)
 @click.option('--wave_h5', '-h5', required=True,
               type=click.Path(),
               help=('Path to Resource .h5 file'))
 @click.option('--out_dir', '-o', required=True, type=click.Path(exists=True),
               help='Directory to dump output files')
 @click.option('-v', '--verbose', is_flag=True,
               help='Flag to turn on debug logging. Default is not verbose.')
 @click.pass_context
-def main(ctx, wave_h5, out_dir, log_file, verbose):
+def main(ctx, wave_h5, out_dir, verbose):
     """
     WaveX Command Line Interface
     """
     ctx.ensure_object(dict)
-    if not os.path.exists(out_dir):
-        os.makedirs(out_dir)
-
     ctx.obj['H5'] = wave_h5
     ctx.obj['OUT_DIR'] = out_dir
     ctx.obj['CLS_KWARGS'] = {}
     ctx.obj['CLS'] = WaveX
 
     _, hsds = check_res_file(wave_h5)
+    name = os.path.splitext(os.path.basename(wave_h5))[0]
     if hsds:
         ctx.obj['CLS_KWARGS']['hsds'] = hsds
     else:
         assert os.path.exists(wave_h5)
 
-    if verbose:
-        log_level = 'DEBUG'
-    else:
-        log_level = 'INFO'
-
-    if log_file is not None:
-        log_dir = os.path.dirname(log_file)
-        if not os.path.exists(log_dir):
-            os.makedirs(log_dir)
-
-    init_logger('rex', log_file=log_file, log_level=log_level)
+    init_mult(name, out_dir, verbose=verbose, node=True,
+              modules=[__name__, 'rex.resource_extraction',
+                       'rex.renewable_resource'])
 
     logger.info('Extracting wave data from {}'.format(wave_h5))
     logger.info('Outputs to be stored in: {}'.format(out_dir))
 
 
-@main.command()
-@click.option('--lat_lon', '-ll', nargs=2, type=float,
-              default=None, show_default=True,
-              help='(lat, lon) coordinates of interest')
-@click.option('--gid', '-gid', type=int, default=None, show_default=True,
-              help='Resource gid of interest')
-@click.option('--sites', '-s', type=click.Path(exists=True), default=None,
-              show_default=True,
+@main.group()
+@click.option('--sites', '-s', type=click.Path(exists=True), required=True,
               help=('.csv or .json file with columns "latitude", "longitude" '
                     'OR "gid"'))
 @click.pass_context
-def sam_datasets(ctx, lat_lon, gid, sites):
+def multi_site(ctx, sites):
     """
-    Extract all datasets needed for SAM for the nearest pixel(s) to the given
-    (lat, lon) coordinates, the given resource gid, or the give sites
+    Extract multiple sites given in '--sites' .csv or .json as
+    "latitude", "longitude" pairs OR "gid"s
     """
-    ctx.invoke(sam_cmd, lat_lon=lat_lon, gid=gid, sites=sites)
+    ctx.invoke(multi_site_grp, sites=sites)
 
 
-@main.group()
+@multi_site.command()
 @click.option('--dataset', '-d', type=str, required=True,
               help='Dataset to extract')
 @click.pass_context
 def dataset(ctx, dataset):
     """
-    Extract a single dataset
+    Extract given dataset for all sites
     """
-    ctx.invoke(dataset_grp, dataset=dataset)
+    ctx.invoke(dataset_cmd, dataset=dataset)
 
 
-@dataset.command()
-@click.option('--lat_lon', '-ll', nargs=2, type=float,
-              default=None, show_default=True,
+@multi_site.command()
+@click.pass_context
+def sam(ctx):
+    """
+    Extract SAM variables
+    """
+    ctx.invoke(sam_cmd)
+
+
+@main.command()
+@click.option('--lat_lon', '-ll', nargs=2, type=click.Tuple([float, float]),
+              default=None,
               help='(lat, lon) coordinates of interest')
-@click.option('--gid', '-gid', type=int, default=None, show_default=True,
+@click.option('--gid', '-g', type=int, default=None,
               help='Resource gid of interest')
 @click.pass_context
-def site(ctx, lat_lon, gid):
+def sam_file(ctx, lat_lon, gid):
     """
-    Extract the nearest pixel to the given (lat, lon) coordinates
-    OR the given resource gid
+    Extract all datasets needed for SAM for the nearest pixel to the given
+    (lat, lon) coordinates OR the given resource gid
     """
-    ctx.invoke(site_cmd, lat_lon=lat_lon, gid=gid)
+    ctx.invoke(sam_file_cmd, lat_lon=lat_lon, gid=gid)
 
 
-@dataset.command()
-@click.option('--region', '-r', type=str, required=True,
-              help='Region to extract')
-@click.option('--region_col', '-col', type=str, default='state',
-              show_default=True,
-              help='Meta column to search for region')
-@click.option('--timestep', '-ts', type=str, default=None, show_default=True,
-              help='Timestep to extract')
+@main.command()
+@click.option('--dataset', '-d', type=str, required=True,
+              help='Dataset to extract')
+@click.option('--lat_lon', '-ll', nargs=2, type=click.Tuple([float, float]),
+              default=None,
+              help='(lat, lon) coordinates of interest')
+@click.option('--gid', '-g', type=int, default=None,
+              help='Resource gid of interest')
 @click.pass_context
-def region(ctx, region, region_col, timestep):
+def site(ctx, dataset, lat_lon, gid):
     """
-    Extract a single dataset for all gids in the given region
+    Extract a single dataset for the nearest pixel to the given (lat, lon)
+    coordinates OR the given resource gid
     """
-
-    ctx.invoke(region_cmd, region=region, region_col=region_col,
-               timestep=timestep)
+    ctx.invoke(site_cmd, dataset=dataset, lat_lon=lat_lon, gid=gid)
 
 
-@dataset.command()
-@click.option('--lat_lon_1', '-ll1', nargs=2, type=float,
-              required=True,
-              help='One corner of the bounding box')
-@click.option('--lat_lon_2', '-ll2', nargs=2, type=float,
-              required=True,
-              help='The other corner of the bounding box')
-@click.option('--file_suffix', '-fs', default=None, show_default=True,
-              help='File name suffix')
-@click.option('--timestep', '-ts', type=str, default=None, show_default=True,
-              help='Timestep to extract')
+@main.command()
+@click.option('--dataset', '-d', type=str, required=True,
+              help='Dataset to extract')
+@click.option('--region', '-r', type=str, required=True,
+              help='Region to extract')
+@click.option('--region_col', '-col', type=str, default='state',
+              help='Meta column to search for region')
 @click.pass_context
-def box(ctx, lat_lon_1, lat_lon_2, file_suffix, timestep):
+def region(ctx, dataset, region, region_col):
     """
-    Extract all pixels in the given bounding box
+    Extract a single dataset for all pixels in the given region
     """
-    ctx.invoke(box_cmd, lat_lon_1=lat_lon_1, lat_lon_2=lat_lon_2,
-               file_suffix=file_suffix, timestep=timestep)
+    ctx.invoke(region_cmd, dataset=dataset, region=region,
+               region_col=region_col)
 
 
-@dataset.command()
-@click.option('--sites', '-s', type=click.Path(exists=True), required=True,
-              help=('.csv or .json file with columns "latitude", "longitude" '
-                    'OR "gid"'))
+@main.command()
+@click.option('--timestep', '-ts', type=str, required=True,
+              help='Timestep to extract')
+@click.option('--dataset', '-d', type=str, required=True,
+              help='Dataset to extract')
+@click.option('--region', '-r', type=str, default=None,
+              help='Region to extract')
+@click.option('--region_col', '-col', type=str, default='state',
+              help='Meta column to search for region')
 @click.pass_context
-def multi_site(ctx, sites):
+def timestep(ctx, timestep, dataset, region, region_col):
     """
-    Extract multiple sites given in '--sites' .csv or .json as
-    "latitude", "longitude" pairs OR "gid"s
-
+    Extract a single dataset for a single timestep
+    Extract only pixels in region if given.
     """
-    ctx.invoke(multi_site_cmd, sites=sites)
+    ctx.invoke(timestep_cmd, dataset=dataset, timestep=timestep,
+               region=region, region_col=region_col)
 
 
 if __name__ == '__main__':
     try:
         main(obj={})
     except Exception:
         logger.exception('Error running WaveX CLI')
```

### Comparing `NREL-rex-0.2.81/rex/resource_extraction/wind_cli.py` & `NREL-rex-0.2.9/rex/resource_extraction/wind_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,229 +1,211 @@
 # -*- coding: utf-8 -*-
-# pylint: disable=all
 """
 WindX Command Line Interface
 """
 import click
 import logging
 import os
 
 from rex.resource_extraction.resource_extraction import WindX, MultiFileWindX
-from rex.resource_extraction.resource_cli import box as box_cmd
-from rex.resource_extraction.resource_cli import dataset as dataset_grp
-from rex.resource_extraction.resource_cli import multi_site as multi_site_cmd
-from rex.resource_extraction.resource_cli import _parse_sites
+from rex.resource_extraction.resource_cli import dataset as dataset_cmd
+from rex.resource_extraction.resource_cli import multi_site as multi_site_grp
 from rex.resource_extraction.resource_cli import region as region_cmd
 from rex.resource_extraction.resource_cli import site as site_cmd
-from rex.utilities.loggers import init_logger
+from rex.resource_extraction.resource_cli import timestep as timestep_cmd
+from rex.utilities.loggers import init_mult
 from rex.utilities.utilities import check_res_file
-from rex import __version__
 
 logger = logging.getLogger(__name__)
 
 
 @click.group()
-@click.version_option(version=__version__)
 @click.option('--wind_h5', '-h5', required=True,
               type=click.Path(),
               help=('Path to Resource .h5 file'))
-@click.option('--out_dir', '-o', required=True, type=click.Path(),
+@click.option('--out_dir', '-o', required=True, type=click.Path(exists=True),
               help='Directory to dump output files')
-@click.option('--log_file', '-log', default=None, type=click.Path(),
-              show_default=True,
-              help='Path to .log file, if None only log to stdout')
 @click.option('-v', '--verbose', is_flag=True,
               help='Flag to turn on debug logging. Default is not verbose.')
 @click.pass_context
-def main(ctx, wind_h5, out_dir, log_file, verbose):
+def main(ctx, wind_h5, out_dir, verbose):
     """
     WindX Command Line Interface
     """
     ctx.ensure_object(dict)
-    if not os.path.exists(out_dir):
-        os.makedirs(out_dir)
-
     ctx.obj['H5'] = wind_h5
     ctx.obj['OUT_DIR'] = out_dir
     ctx.obj['CLS_KWARGS'] = {}
 
     multi_h5_res, hsds = check_res_file(wind_h5)
-    if multi_h5_res and not hsds:
+    if multi_h5_res:
         assert os.path.exists(os.path.dirname(wind_h5))
         ctx.obj['CLS'] = MultiFileWindX
-    elif hsds:
-        ctx.obj['CLS_KWARGS']['hsds'] = hsds
     else:
-        assert os.path.exists(wind_h5)
+        if hsds:
+            ctx.obj['CLS_KWARGS']['hsds'] = hsds
+        else:
+            assert os.path.exists(wind_h5)
 
         ctx.obj['CLS'] = WindX
 
-    if verbose:
-        log_level = 'DEBUG'
-    else:
-        log_level = 'INFO'
-
-    if log_file is not None:
-        log_dir = os.path.dirname(log_file)
-        if not os.path.exists(log_dir):
-            os.makedirs(log_dir)
-
-    init_logger('rex', log_file=log_file, log_level=log_level)
+    name = os.path.splitext(os.path.basename(wind_h5))[0]
+    init_mult(name, out_dir, verbose=verbose, node=True,
+              modules=[__name__, 'rex.resource_extraction',
+                       'rex.renewable_resource'])
 
     logger.info('Extracting Wind data from {}'.format(wind_h5))
     logger.info('Outputs to be stored in: {}'.format(out_dir))
 
 
 @main.command()
 @click.option('--hub_height', '-h', type=int, required=True,
               help='Hub height to extract SAM variables at')
-@click.option('--lat_lon', '-ll', nargs=2, type=float,
-              default=None, show_default=True,
+@click.option('--lat_lon', '-ll', nargs=2, type=click.Tuple([float, float]),
+              default=None,
               help='(lat, lon) coordinates of interest')
-@click.option('--gid', '-gid', type=int, default=None, show_default=True,
+@click.option('--gid', '-g', type=int, default=None,
               help='Resource gid of interest')
-@click.option('--sites', '-s', type=click.Path(exists=True), default=None,
-              show_default=True,
-              help=('.csv or .json file with columns "latitude", "longitude" '
-                    'OR "gid"'))
 @click.pass_context
-def sam_datasets(ctx, hub_height, lat_lon, gid, sites):
-    """
-    Extract all datasets needed for SAM for the nearest pixel(s) to the given
-    (lat, lon) coordinates, the given resource gid, or the give sites
+def sam_file(ctx, hub_height, lat_lon, gid):
     """
-    if not lat_lon:
-        lat_lon = None
+    Extract all datasets at the given hub height needed for SAM for
+    nearest pixel to the given (lat, lon) coordinates OR the given
+    resource gid
+    """
+    if lat_lon is None and gid is None:
+        click.echo("Must supply '--lat-lon' OR '--gid'!")
+        raise click.Abort()
+    elif lat_lon and gid:
+        click.echo("You must only supply '--lat-lon' OR '--gid'!")
+        raise click.Abort()
+
+    with ctx.obj['CLS'](ctx.obj['H5'], compute_tree=ctx.obj['TREE']) as f:
+        if lat_lon is not None:
+            SAM_df = f.get_SAM_lat_lon(hub_height, lat_lon)
+        elif gid is not None:
+            SAM_df = f.get_SAM_gid(hub_height, lat_lon)
+
+    SAM_df['winddirection_{}m'.format(hub_height)] = 0
+
+    out_path = "{}.csv".format(SAM_df.name)
+    out_path = os.path.join(ctx.obj['OUT_DIR'], out_path)
+    logger.info('Saving data to {}'.format(out_path))
+    SAM_df.to_csv(out_path)
 
-    inputs = set((lat_lon, gid, sites))
-    if len(inputs) == 1:
-        msg = "Must supply '--lat-lon', '--gid', or '--sites'!"
-        click.echo(msg)
-        raise click.Abort(msg)
-    elif len(inputs) > 2:
-        msg = ("You must only supply one of '--lat-lon', '--gid', or "
-               "'--sites'!")
-        click.echo(msg)
-        raise click.Abort(msg)
-
-    if lat_lon or gid:
-        logger.info('Saving data to {}'.format(ctx.obj['OUT_DIR']))
-        with ctx.obj['CLS'](ctx.obj['H5'], **ctx.obj['CLS_KWARGS']) as f:
-            if lat_lon is not None:
-                out_path = os.path.join(ctx.obj['OUT_DIR'],
-                                        'SAM_{}.csv'.format(lat_lon))
-                f.get_SAM_lat_lon(hub_height, lat_lon,
-                                  out_path=out_path)
-            elif gid is not None:
-                out_path = os.path.join(ctx.obj['OUT_DIR'],
-                                        'SAM_{}.csv'.format(gid))
-                f.get_SAM_gid(hub_height, gid, out_path=out_path)
 
-    else:
-        name, gid, lat_lon = _parse_sites(sites)
-        with ctx.obj['CLS'](ctx.obj['H5'], **ctx.obj['CLS_KWARGS']) as f:
-            meta = f['meta']
-            if lat_lon is not None:
-                SAM_df = f.get_SAM_lat_lon(hub_height, lat_lon)
-            elif gid is not None:
-                SAM_df = f.get_SAM_gid(hub_height, gid)
-
-        gids = []
-        for df in SAM_df:
-            gids.append(int(df.name.split('-')[-1]))
-            out_path = "{}-{}.csv".format(df.name, name)
-            out_path = os.path.join(ctx.obj['OUT_DIR'], out_path)
-            logger.info('Saving data to {}'.format(out_path))
-            df.to_csv(out_path)
-
-        out_path = "{}-meta.csv".format(name)
-        out_path = os.path.join(ctx.obj['OUT_DIR'], out_path)
-        meta = meta.loc[gids]
-        logger.info('Saving meta data to {}'.format(out_path))
-        meta.to_csv(out_path)
-
-
-@main.group()
+@main.command()
 @click.option('--dataset', '-d', type=str, required=True,
               help='Dataset to extract')
-@click.pass_context
-def dataset(ctx, dataset):
-    """
-    Extract a single dataset
-    """
-    ctx.invoke(dataset_grp, dataset=dataset)
-
-
-@dataset.command()
-@click.option('--lat_lon', '-ll', nargs=2, type=float,
-              default=None, show_default=True,
-              help='(lat, lon) coordinates of interest')
-@click.option('--gid', '-gid', type=int, default=None, show_default=True,
+@click.option('--gid', '-g', type=int, default=None,
               help='Resource gid of interest')
+@click.option('--lat_lon', '-ll', nargs=2, type=click.Tuple([float, float]),
+              default=None,
+              help='(lat, lon) coordinates of interest')
 @click.pass_context
-def site(ctx, lat_lon, gid):
+def site(ctx, dataset, gid, lat_lon):
     """
-    Extract the nearest pixel to the given (lat, lon) coordinates OR the
-    given resource gid
+    Extract a single dataset for the nearest pixel to the given (lat, lon)
+    coordinates OR the given resource gid
     """
-
-    ctx.invoke(site_cmd, lat_lon=lat_lon, gid=gid)
+    ctx.invoke(site_cmd, dataset=dataset, lat_lon=lat_lon, gid=gid)
 
 
-@dataset.command()
-@click.option('--region', '-r', type=str, required=True,
+@main.command()
+@click.option('--dataset', '-d', type=str, required=True,
+              help='Dataset to extract')
+@click.option('--timestep', '-ts', type=str, required=True,
+              help='Timestep to extract')
+@click.option('--region', '-r', type=str, default=None,
               help='Region to extract')
 @click.option('--region_col', '-col', type=str, default='state',
-              show_default=True,
               help='Meta column to search for region')
-@click.option('--timestep', '-ts', type=str, default=None, show_default=True,
-              help='Time-step to extract')
 @click.pass_context
-def region(ctx, region, region_col, timestep):
+def timestep(ctx, dataset, timestep, region, region_col):
     """
-    Extract a single dataset for all gids in the given region
+    Extract a single dataset for a single timestep
+    Extract only pixels in region if given.
     """
-
-    ctx.invoke(region_cmd, region=region, region_col=region_col,
-               timestep=timestep)
+    ctx.invoke(timestep_cmd, dataset=dataset, timestep=timestep, region=region,
+               region_col=region_col)
 
 
-@dataset.command()
-@click.option('--lat_lon_1', '-ll1', nargs=2, type=float,
-              required=True,
-              help='One corner of the bounding box')
-@click.option('--lat_lon_2', '-ll2', nargs=2, type=float,
-              required=True,
-              help='The other corner of the bounding box')
-@click.option('--file_suffix', '-fs', default=None, show_default=True,
-              help='Filename suffix')
-@click.option('--timestep', '-ts', type=str, default=None, show_default=True,
-              help='Timestep to extract')
+@main.command()
+@click.option('--dataset', '-d', type=str, required=True,
+              help='Dataset to extract')
+@click.option('--region', '-r', type=str, required=True,
+              help='Region to extract')
+@click.option('--region_col', '-col', type=str, default='state',
+              help='Meta column to search for region')
 @click.pass_context
-def box(ctx, lat_lon_1, lat_lon_2, file_suffix, timestep):
+def region(ctx, dataset, region, region_col):
     """
-    Extract all pixels in the given bounding box
+    Extract a single dataset for all pixels in the given region
     """
-
-    ctx.invoke(box_cmd, lat_lon_1=lat_lon_1, lat_lon_2=lat_lon_2,
-               file_suffix=file_suffix, timestep=timestep)
+    ctx.invoke(region_cmd, dataset=dataset, region=region,
+               region_col=region_col)
 
 
-@dataset.command()
+@main.group()
 @click.option('--sites', '-s', type=click.Path(exists=True), required=True,
               help=('.csv or .json file with columns "latitude", "longitude" '
                     'OR "gid"'))
 @click.pass_context
 def multi_site(ctx, sites):
     """
     Extract multiple sites given in '--sites' .csv or .json as
     "latitude", "longitude" pairs OR "gid"s
+    """
+    ctx.invoke(multi_site_grp, sites=sites)
+
 
+@multi_site.command()
+@click.option('--hub_height', '-h', type=int, required=True,
+              help='Hub height to extract SAM variables at')
+@click.pass_context
+def sam(ctx, hub_height):
+    """
+    Extract SAM variables
+    """
+    gid = ctx.obj['GID']
+    lat_lon = ctx.obj['LAT_LON']
+    with ctx.obj['CLS'](ctx.obj['H5'], compute_tree=ctx.obj['TREE']) as f:
+        meta = f['meta']
+        if lat_lon is not None:
+            SAM_df = f.get_SAM_lat_lon(hub_height, lat_lon)
+        elif gid is not None:
+            SAM_df = f.get_SAM_gid(hub_height, gid)
+
+    name = ctx.obj['NAME']
+    gids = []
+    for df in SAM_df:
+        out_path = "{}-{}.csv".format(df.name, name)
+        out_path = os.path.join(ctx.obj['OUT_DIR'], out_path)
+        df['winddirection_{}m'.format(hub_height)] = 0
+        gids.append(int(df.name.split('-')[-1]))
+        logger.info('Saving data to {}'.format(out_path))
+        df.to_csv(out_path)
+
+    out_path = "{}-meta.csv".format(name)
+    out_path = os.path.join(ctx.obj['OUT_DIR'], out_path)
+    meta = meta.loc[gids]
+    meta.index.name = 'gid'
+    logger.info('Saving meta data to {}'.format(out_path))
+    meta.to_csv(out_path)
+
+
+@multi_site.command()
+@click.option('--dataset', '-d', type=str, required=True,
+              help='Dataset to extract')
+@click.pass_context
+def dataset(ctx, dataset):
+    """
+    Extract given dataset for all sites
     """
-    ctx.invoke(multi_site_cmd, sites=sites)
+    ctx.invoke(dataset_cmd, dataset=dataset)
 
 
 if __name__ == '__cli__':
     try:
         main(obj={})
     except Exception:
         logger.exception('Error running WindX CLI')
```

### Comparing `NREL-rex-0.2.81/rex/utilities/cli_dtypes.py` & `NREL-rex-0.2.9/rex/utilities/cli_dtypes.py`

 * *Files 10% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         return x
 
     def convert(self, value, param, ctx):
         """Convert string to list."""
         if isinstance(value, str):
             value = sanitize_str(value, subs=['=', '(', ')', ' ', '[', ']',
                                               '"', "'"])
-            if value.lower() == 'none':
+            if value == 'None':
                 return None
             list0 = value.split(',')
             return [self.dtype(x) for x in list0]
         elif isinstance(value, list):
             return value
         elif isinstance(value, type(None)):
             return value
@@ -159,15 +159,15 @@
         self._click_path_type = click.types.Path(**kwargs)
 
     def convert(self, value, param, ctx):
         """Convert string to list."""
         if isinstance(value, str):
             value = sanitize_str(value, subs=['=', '(', ')', ' ', '[', ']',
                                               '"', "'"])
-            if value.lower() == 'none':
+            if value == 'None':
                 return None
             list0 = value.split(',')
             return [self.path(x, param, ctx) for x in list0]
         elif isinstance(value, list):
             return value
         elif isinstance(value, type(None)):
             return value
@@ -176,48 +176,15 @@
                       .format(value, type(value)), param, ctx)
 
     def path(self, value, param, ctx):
         """Enforce a homogeneous string datatype."""
         return self._click_path_type.convert(value, param, ctx)
 
 
-class StrOrListType(click.ParamType):
-    """Flexible type for string or list of strings."""
-    name = 'str_or_list'
-
-    @staticmethod
-    def dtype(x):
-        """Enforce a homogeneous string datatype."""
-        return str(x)
-
-    def convert(self, value, param, ctx):
-        """Convert string to list."""
-        if isinstance(value, str):
-            if (('(' in value and ')' in value)
-                    or ('[' in value and ']' in value)):
-                value = sanitize_str(value, subs=['=', '(', ')', ' ', '[', ']',
-                                                  '"', "'"])
-                list0 = value.split(',')
-                return [self.dtype(x) for x in list0]
-            else:
-                if value.lower() == 'none':
-                    return None
-                else:
-                    return value
-        elif isinstance(value, list):
-            return value
-        elif isinstance(value, type(None)):
-            return value
-        else:
-            self.fail('Cannot recognize list type: {} {}'
-                      .format(value, type(value)), param, ctx)
-
-
 INT = IntType()
 FLOAT = FloatType()
 STR = StrType()
 STRFLOAT = StrFloatType()
 INTLIST = IntListType()
 FLOATLIST = FloatListType()
 STRLIST = StrListType()
 PATHLIST = PathListType()
-STR_OR_LIST = StrOrListType()
```

### Comparing `NREL-rex-0.2.81/rex/utilities/downscale.py` & `NREL-rex-0.2.9/rex/utilities/downscale.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,48 +6,40 @@
 @author: gbuster
 """
 import numpy as np
 import pandas as pd
 import logging
 
 from rex.utilities.solar_position import SolarPosition
-from rex.utilities.utilities import get_lat_lon_cols, pd_date_range
 
 from nsrdb.all_sky import CLEAR_TYPES
 from nsrdb.all_sky.all_sky import all_sky
 from nsrdb.utilities.interpolation import temporal_lin, temporal_step
 
 
 logger = logging.getLogger(__name__)
 
 
-def make_time_index(year, frequency, set_timezone=True):
+def make_time_index(year, frequency):
     """Make the NSRDB target time index.
 
     Parameters
     ----------
     year : int
         Year for time index.
     frequency : str
         String in the Pandas frequency format, e.g. '5min'.
-    set_timezone : bool
-        Flag to set a timezone-aware time index. will be set to UTC with
-        zero offset.
 
     Returns
     -------
     ti : pd.DatetimeIndex
         Pandas datetime index for a full year at the requested resolution.
     """
-    ti = pd_date_range('1-1-{y}'.format(y=year), '1-1-{y}'.format(y=year + 1),
+    ti = pd.date_range('1-1-{y}'.format(y=year), '1-1-{y}'.format(y=year + 1),
                        freq=frequency)[:-1]
-
-    if set_timezone:
-        ti = ti.tz_localize('UTC')
-
     return ti
 
 
 def interp_cld_props(data, ti_native, ti_new,
                      var_list=('cld_reff_dcomp', 'cld_opd_dcomp')):
     """Interpolate missing cloud properties (NOT CLOUD TYPE).
 
@@ -83,39 +75,34 @@
 
         # set clear timesteps cloud props to zero for better transitions
         data[var].values[np.isin(data['cloud_type'], CLEAR_TYPES)] = 0.0
 
         # interpolate empty values
         data[var] = data[var].interpolate(method='linear', axis=0).values
 
-        logger.debug('Downscaled array for "{}" has shape {} and {} NaN values'
-                     .format(var, data[var].shape, np.isnan(data[var]).sum()))
-
     return data
 
 
-def downscale_nsrdb(SAM_res, res, frequency='5min',
+def downscale_nsrdb(SAM_res, res, frequency,
                     sam_vars=('dhi', 'dni', 'wind_speed', 'air_temperature'),
-                    variability_kwargs=None):
+                    ghi_variability=0.05):
     """Downscale the NSRDB resource and return the preloaded SAM_res.
 
     Parameters
     ----------
     SAM_res : SAMResource
         SAM resource object.
     res : NSRDB
         NSRDB resource handler.
     frequency : str
         String in the Pandas frequency format, e.g. '5min'.
     sam_vars : tuple | list
         Variables to save to SAM resource handler before returning.
-    variability_kwargs : Nonetype | dict
-        Downscaling kwargs to the NSRDB all sky method call. Should include
-        maximum GHI synthetic variability fraction ("var_frac") which
-        will be set to 0.05 (5%) if variability_kwargs is None.
+    ghi_variability : float
+        Maximum GHI synthetic variability fraction.
 
     Returns
     -------
     SAM_res : SAMResource
         SAM resource object with downscaled solar resource data loaded.
         Time index and shape are also updated.
     """
@@ -137,51 +124,35 @@
     sites_slice = SAM_res.sites_slice
 
     # get downscaled time_index
     time_index = make_time_index(res.time_index.year[0], frequency)
     SAM_res._time_index = time_index
     SAM_res._shape = (len(time_index), len(SAM_res.sites))
 
-    logger.debug('Native resource time index has length {}: \n{}'
-                 .format(len(res.time_index), res.time_index))
-    logger.debug('Target resource time index has length {}: \n{}'
-                 .format(len(time_index), time_index))
-
     # downscale variables into an all-sky input variable namespace
     all_sky_ins = {'time_index': time_index}
     for var in var_list:
-        arr = res[var, :, sites_slice]
-        arr = temporal_lin(res[var, :, sites_slice], res.time_index,
-                           time_index)
-        all_sky_ins[var] = arr
-        logger.debug('Downscaled array for "{}" has shape {} and {} NaN values'
-                     .format(var, arr.shape, np.isnan(arr).sum()))
+        all_sky_ins[var] = temporal_lin(res[var, :, sites_slice],
+                                        res.time_index, time_index)
 
     # calculate downscaled solar zenith angle
-    lat_lon_cols = get_lat_lon_cols(res.meta)
-    lat_lon = res.meta.loc[SAM_res.sites, lat_lon_cols]\
+    lat_lon = res.meta.loc[SAM_res.sites, ['latitude', 'longitude']]\
         .values.astype(np.float32)
-    sza = SolarPosition(time_index, lat_lon).zenith
-    all_sky_ins['solar_zenith_angle'] = sza
-    logger.debug('Downscaled array for "solar_zenith_angle" '
-                 'has shape {} and {} NaN values'
-                 .format(sza.shape, np.isnan(sza).sum()))
+    all_sky_ins['solar_zenith_angle'] = SolarPosition(time_index,
+                                                      lat_lon).zenith
 
     # get downscaled cloud properties
     all_sky_ins['cloud_type'] = temporal_step(
         res['cloud_type', :, sites_slice], res.time_index, time_index)
     all_sky_ins['cld_opd_dcomp'] = res['cld_opd_dcomp', :, sites_slice]
     all_sky_ins['cld_reff_dcomp'] = res['cld_reff_dcomp', :, sites_slice]
     all_sky_ins = interp_cld_props(all_sky_ins, res.time_index, time_index)
 
-    # add all sky kwargs such as variability
-    if variability_kwargs is None:
-        variability_kwargs = {'var_frac': 0.05}
-
-    all_sky_ins['variability_kwargs'] = variability_kwargs
+    # add variability
+    all_sky_ins['ghi_variability'] = ghi_variability
 
     # run all-sky
     logger.debug('Running all-sky for "{}".'.format(SAM_res))
     all_sky_outs = all_sky(**all_sky_ins)
 
     # set downscaled data to sam resource handler
     for k, v in all_sky_outs.items():
```

### Comparing `NREL-rex-0.2.81/rex/utilities/exceptions.py` & `NREL-rex-0.2.9/rex/utilities/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,26 +18,14 @@
 
 class ExecutionError(Exception):
     """
     Error for execution failure
     """
 
 
-class HpcError(Exception):
-    """
-    Error for HPC failure
-    """
-
-
-class SlurmError(Exception):
-    """
-    Error for SLURM failure
-    """
-
-
 class ExtrapolationWarning(Warning):
     """
     Warning for when value will be extrapolated
     """
 
 
 class MoninObukhovExtrapolationError(Exception):
@@ -78,20 +66,14 @@
 
 class ParallelExecutionWarning(Warning):
     """
     Warning for parallel job execution.
     """
 
 
-class PbsWarning(Warning):
-    """
-    Warning for PBS errors/warnings
-    """
-
-
 class SlurmWarning(Warning):
     """
     Warning for SLURM errors/warnings
     """
 
 
 class ResourceWarning(Warning):
@@ -106,24 +88,7 @@
     """
 
 
 class SAMInputWarning(Warning):
     """
     Warning for bad SAM inputs
     """
-
-
-class LoggerWarning(Warning):
-    """
-    Warning for bad logger inputs
-    """
-
-class HandlerRuntimeError(Exception):
-    """
-    RuntimeError for Handlers
-    """
-
-
-class HandlerValueError(Exception):
-    """
-    ValueError for Handlers
-    """
```

### Comparing `NREL-rex-0.2.81/rex/utilities/parse_keys.py` & `NREL-rex-0.2.9/rex/utilities/parse_keys.py`

 * *Files identical despite different names*

### Comparing `NREL-rex-0.2.81/rex/utilities/solar_position.py` & `NREL-rex-0.2.9/rex/utilities/solar_position.py`

 * *Files identical despite different names*

### Comparing `NREL-rex-0.2.81/rex/utilities/toml_parser.py` & `NREL-rex-0.2.9/rex/utilities/toml_parser.py`

 * *Files identical despite different names*

### Comparing `NREL-rex-0.2.81/setup.py` & `NREL-rex-0.2.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -58,34 +58,28 @@
     entry_points={
         "console_scripts": [
             "rex=rex.resource_extraction.resource_cli:main",
             "NSRDBX=rex.resource_extraction.nsrdb_cli:main",
             "WINDX=rex.resource_extraction.wind_cli:main",
             "WaveX=rex.resource_extraction.wave_cli:main",
             "MultiYearX=rex.resource_extraction.multi_year_resource_cli:main",
-            "US-wave=rex.resource_extraction.US_wave_cli:main",
-            "rechunk=rex.rechunk_h5.rechunk_cli:main",
-            "combine-h5=rex.rechunk_h5.combine_h5_cli:main",
-            "temporal-stats=rex.temporal_stats.temporal_stats_cli:main",
-            "wind-rose=rex.jpd.wind_rose_cli:main"
-        ],
+            "rechunk=rex.rechunk_h5.rechunk_cli:main"],
     },
     include_package_data=True,
     license="BSD 3-Clause",
     zip_safe=False,
     keywords="rex",
-    python_requires='>=3.8',
+    python_requires='>=3.7',
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
     ],
     test_suite="tests",
     install_requires=install_requires,
     extras_require={
         "test": test_requires,
         "dev": test_requires + ["flake8", "pre-commit", "pylint"],
     },
```

