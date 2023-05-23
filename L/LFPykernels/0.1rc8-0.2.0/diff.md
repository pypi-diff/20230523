# Comparing `tmp/LFPykernels-0.1rc8.tar.gz` & `tmp/LFPykernels-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LFPykernels-0.1rc8.tar", last modified: Tue Jun 28 19:39:49 2022, max compression
+gzip compressed data, was "LFPykernels-0.2.0.tar", last modified: Tue May 23 09:24:35 2023, max compression
```

## Comparing `LFPykernels-0.1rc8.tar` & `LFPykernels-0.2.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 19:39:49.323962 LFPykernels-0.1rc8/
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/CITATION.cff
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 19:39:49.319962 LFPykernels-0.1rc8/LFPykernels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15909 2022-06-28 19:39:49.000000 LFPykernels-0.1rc8/LFPykernels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-06-28 19:39:49.000000 LFPykernels-0.1rc8/LFPykernels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 19:39:49.000000 LFPykernels-0.1rc8/LFPykernels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 19:39:44.000000 LFPykernels-0.1rc8/LFPykernels.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-06-28 19:39:49.000000 LFPykernels-0.1rc8/LFPykernels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-06-28 19:39:49.000000 LFPykernels-0.1rc8/LFPykernels.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      525 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    15909 2022-06-28 19:39:49.323962 LFPykernels-0.1rc8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14824 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 19:39:49.319962 LFPykernels-0.1rc8/doc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 19:39:49.319962 LFPykernels-0.1rc8/doc/source/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/doc/source/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     2391 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/doc/source/environment.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/doc/source/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/doc/source/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 19:39:49.323962 LFPykernels-0.1rc8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/examples/BallAndSticksTemplate.hoc
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/examples/BallAndSticks_E.hoc
--rw-r--r--   0 runner    (1001) docker     (121)      806 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/examples/BallAndSticks_I.hoc
--rw-r--r--   0 runner    (1001) docker     (121)     1536 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/examples/FIR_filter.nestml
--rw-r--r--   0 runner    (1001) docker     (121)   438267 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/examples/LIF_net_forward_model_predictions.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     2058 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    28610 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/examples/README_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    12178 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/examples/example_network_methods.py
--rw-r--r--   0 runner    (1001) docker     (121)     6929 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/examples/example_network_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 19:39:49.323962 LFPykernels-0.1rc8/examples/mod/
--rw-r--r--   0 runner    (1001) docker     (121)      940 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/examples/mod/Ih_linearized_v2_frozen.mod
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/examples/mod/NaTa_t_frozen.mod
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/examples/mod/SKv3_1_frozen.mod
--rwxr-xr-x   0 runner    (1001) docker     (121)      687 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/examples/mod/exp2synI.mod
--rw-r--r--   0 runner    (1001) docker     (121)     4170 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/examples/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 19:39:49.323962 LFPykernels-0.1rc8/lfpykernels/
--rw-r--r--   0 runner    (1001) docker     (121)     1593 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/lfpykernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28121 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/lfpykernels/kernel_approximator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 19:39:49.323962 LFPykernels-0.1rc8/lfpykernels/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/lfpykernels/tests/BallAndSticksTemplate.hoc
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/lfpykernels/tests/BallAndSticks_E.hoc
--rwxr-xr-x   0 runner    (1001) docker     (121)      687 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/lfpykernels/tests/exp2synI.mod
--rw-r--r--   0 runner    (1001) docker     (121)     7592 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/lfpykernels/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/lfpykernels/version.py
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-06-28 19:39:49.323962 LFPykernels-0.1rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3045 2022-06-28 19:39:35.000000 LFPykernels-0.1rc8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:24:35.235303 LFPykernels-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/CITATION.cff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:24:35.231303 LFPykernels-0.2.0/LFPykernels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-05-23 09:24:35.000000 LFPykernels-0.2.0/LFPykernels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-23 09:24:35.000000 LFPykernels-0.2.0/LFPykernels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:24:35.000000 LFPykernels-0.2.0/LFPykernels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:24:27.000000 LFPykernels-0.2.0/LFPykernels.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-23 09:24:35.000000 LFPykernels-0.2.0/LFPykernels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 09:24:35.000000 LFPykernels-0.2.0/LFPykernels.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-05-23 09:24:35.235303 LFPykernels-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14472 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:24:35.227303 LFPykernels-0.2.0/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:24:35.231303 LFPykernels-0.2.0/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/doc/source/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/doc/source/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/doc/source/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/doc/source/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:24:35.235303 LFPykernels-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/examples/BallAndSticksTemplate.hoc
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/examples/BallAndSticks_E.hoc
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/examples/BallAndSticks_I.hoc
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/examples/FIR_filter.nestml
+-rw-r--r--   0 runner    (1001) docker     (123)   438267 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/examples/LIF_net_forward_model_predictions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    52679 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/examples/README_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12178 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/examples/example_network_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/examples/example_network_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:24:35.235303 LFPykernels-0.2.0/examples/mod/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/examples/mod/Ih_linearized_v2_frozen.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/examples/mod/NaTa_t_frozen.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/examples/mod/SKv3_1_frozen.mod
+-rwxr-xr-x   0 runner    (1001) docker     (123)      687 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/examples/mod/exp2synI.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/examples/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:24:35.235303 LFPykernels-0.2.0/lfpykernels/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/lfpykernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29138 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/lfpykernels/kernel_approximator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:24:35.235303 LFPykernels-0.2.0/lfpykernels/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/lfpykernels/tests/BallAndSticksTemplate.hoc
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/lfpykernels/tests/BallAndSticks_E.hoc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      687 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/lfpykernels/tests/exp2synI.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/lfpykernels/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/lfpykernels/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 09:24:35.235303 LFPykernels-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-23 09:24:16.000000 LFPykernels-0.2.0/setup.py
```

### Comparing `LFPykernels-0.1rc8/LFPykernels.egg-info/PKG-INFO` & `LFPykernels-0.2.0/LFPykernels.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: LFPykernels
-Version: 0.1rc8
+Version: 0.2.0
 Summary: Causal spike-signal impulse response functions for finite-sized neuronal network models
 Home-page: https://github.com/LFPy/LFPykernels
 Author: LFPy-team
 Author-email: lfpy@users.noreply.github.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -28,112 +26,106 @@
 License-File: LICENSE
 
 # LFPykernels
 
 The ``LFPykernels`` package incorporates forward-model based calculations of causal spike-signal
 impulse response functions for finite-sized neuronal network models.
 
-
 ## Build Status
 
 [![DOI](https://zenodo.org/badge/424143558.svg)](https://zenodo.org/badge/latestdoi/424143558)
 [![Coverage Status](https://coveralls.io/repos/github/LFPy/LFPykernels/badge.svg?branch=main)](https://coveralls.io/github/LFPy/LFPykernels?branch=main)
 [![Documentation Status](https://readthedocs.org/projects/lfpykernels/badge/?version=latest)](https://lfpykernels.readthedocs.io/en/latest/?badge=latest)
 [![flake8 lint](https://github.com/LFPy/LFPykernels/actions/workflows/flake8.yml/badge.svg)](https://github.com/LFPy/LFPykernels/actions/workflows/flake8.yml)
 [![Python application](https://github.com/LFPy/LFPykernels/workflows/Python%20application/badge.svg)](https://github.com/LFPy/LFPykernels/actions?query=workflow%3A%22Python+application%22)
 [![Upload Python Package](https://github.com/LFPy/LFPykernels/workflows/Upload%20Python%20Package/badge.svg)](https://pypi.org/project/LFPykernels)
-[![Conda Recipe](https://img.shields.io/badge/recipe-lfpykernels-green.svg)](https://anaconda.org/conda-forge/lfpykernels)
-[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/lfpykernels.svg)](https://anaconda.org/conda-forge/lfpykernels)
-[![Conda Version](https://img.shields.io/conda/vn/conda-forge/lfpykernels.svg)](https://anaconda.org/conda-forge/lfpykernels)
-[![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/lfpykernels.svg)](https://anaconda.org/conda-forge/lfpykernels)
 [![License](http://img.shields.io/:license-GPLv3+-green.svg)](http://www.gnu.org/licenses/gpl-3.0.html)
 
-
 ## Citation
 
-If you use this software, please cite it as (change version accordingly):
+These codes correspond to results shown in the peer-reviewed manuscript:
+
+Hagen E, Magnusson SH, Ness TV, Halnes G, Babu PN, et al. (2022)
+Brain signal predictions from multi-scale networks using a linearized framework.
+PLOS Computational Biology 18(8): e1010353. <https://doi.org/10.1371/journal.pcbi.1010353>
 
-    Hagen, Espen. (2021). LFPykernels (version/git-SHA/git-tag). Zenodo. https://doi.org/10.5281/zenodo.5720619
+Bibtex format:
+
+    @article{10.1371/journal.pcbi.1010353,
+        doi = {10.1371/journal.pcbi.1010353},
+        author = {Hagen, Espen AND Magnusson, Steinn H. AND Ness, Torbjørn V. AND Halnes, Geir AND Babu, Pooja N. AND Linssen, Charl AND Morrison, Abigail AND Einevoll, Gaute T.},
+        journal = {PLOS Computational Biology},
+        publisher = {Public Library of Science},
+        title = {Brain signal predictions from multi-scale networks using a linearized framework},
+        year = {2022},
+        month = {08},
+        volume = {18},
+        url = {https://doi.org/10.1371/journal.pcbi.1010353},
+        pages = {1-51},
+        number = {8},
+    }
 
+If you use this software, please cite it as (change `<version>/<git-SHA>/<git-tag>` accordingly):
+
+    Hagen, Espen. (2021). LFPykernels (<version>/<git-SHA>/<git-tag>). Zenodo. https://doi.org/10.5281/zenodo.5720619
 
 BibTex format:
 
     @software{hagen_espen_2021_5720619,
       author       = {Hagen, Espen},
       title        = {LFPykernels},
       month        = nov,
       year         = 2021,
       note         = {If you use this software, please cite it as below.},
       publisher    = {Zenodo},
-      version      = {version/git-SHA/git-tag},
+      version      = {<version>/<git-SHA>/<git-tag>},
       doi          = {10.5281/zenodo.5720619},
       url          = {https://doi.org/10.5281/zenodo.5720619}
     }
 
-
-These codes correspond to results shown in the preprint manuscript:
-
-    Brain signal predictions from multi-scale networks using a linearized framework
-    Espen Hagen, Steinn H. Magnusson, Torbjørn V. Ness, Geir Halnes, Pooja N. Babu, Charl Linssen, Abigail Morrison, Gaute T. Einevoll
-    bioRxiv 2022.02.28.482256; doi: https://doi.org/10.1101/2022.02.28.482256
-
-
-Bibtex format:
-
-    @article {Hagen2022.02.28.482256,
-    	author = {Hagen, Espen and Magnusson, Steinn H. and Ness, Torbjørn V. and Halnes, Geir and Babu, Pooja N. and Linssen, Charl and Morrison, Abigail and Einevoll, Gaute T.},
-    	title = {Brain signal predictions from multi-scale networks using a linearized framework},
-    	elocation-id = {2022.02.28.482256},
-    	year = {2022},
-    	doi = {10.1101/2022.02.28.482256},
-    	publisher = {Cold Spring Harbor Laboratory},
-    	URL = {https://www.biorxiv.org/content/early/2022/03/02/2022.02.28.482256},
-    	eprint = {https://www.biorxiv.org/content/early/2022/03/02/2022.02.28.482256.full.pdf},
-    	journal = {bioRxiv}
-    }
-
 If you use or refer to this work, please cite it as above.
 Adaptations or modifications of this work should comply with the provided `LICENSE` file provided with this repository.  
 
-
 ## Features
 
 The ``LFPykernels`` package incorporates forward-model based calculations of causal spike-signal
 impulse response functions for finite-sized neuronal network models.
 The signals considered are low-frequency extracellular potentials ("local field potential" - LFP)
 or current dipole moments (and by extension EEG and MEG like signals) that are
 thought to mainly stem from synaptic currents and associated return currents.
 The basic idea is that the effect of any spike event in each presynaptic
 population on each signal type can be captured by single linearised multicompartment neuron
 models representative of each population and simultaneously accounting for known distributions of
 cells and synapses in space, distributions of delays, synaptic currents and associated return currents.
 
-A scientific publication describing the present methodology in detail is planned.
+The present methodology is described in detail by [Hagen E et al., 2022](https://doi.org/10.1371/journal.pcbi.1010353).
 The intended use for filter kernels predicted using ``LFPykernels`` is forward-model based signal predictions
 from neuronal network simulation frameworks using simplified neuron representations like leaky integrate-and-fire
-point neurons or rate-based neurons.
-Let ``nu_X(t)`` describe presynaptic population spike rates in units of spikes/dt
-and ``H_YX(r, tau)`` predicted spike-signal kernels for the connections between presynaptic populations ``X`` and
-postsynaptic populations ``Y`` the full signal may then be computed via the sum over linear convolutions
-```
-V(r, t) = sum_X sum_Y conv(nu_X, H_YX)(r, t)
+point neurons or rate-based neurons, but can also be used with biophysically detailed network models.
+
+Let `$\nu_X(t)$` describe presynaptic population spike rates in units of spikes/dt
+and `$H_{YX}(\mathbf{R}, \tau)$` predicted spike-signal kernels for the connections between presynaptic populations `$X$` and
+postsynaptic populations `$Y$` the full signal may then be computed via the sum over linear convolutions:
+
+``` math
+V(\mathbf{R}, t) = \sum_X \sum_Y (\nu_X \ast H_{YX})(\mathbf{R}, t)
 ```
 
 A more elaborate example combining kernel predictions with a spiking point-neuron network simulation is provided in the example notebook
-https://github.com/LFPy/LFPykernels/blob/main/examples/LIF_net_forward_model_predictions.ipynb
-
-For questions, please raise an issue at https://github.com/LFPy/LFPykernels/issues.
+<https://github.com/LFPy/LFPykernels/blob/main/examples/LIF_net_forward_model_predictions.ipynb>
 
+For questions, please raise an issue at <https://github.com/LFPy/LFPykernels/issues>.
 
 ## Usage
 
-Example prediction of kernel function ``H`` mapping spike events of a
-presynaptic inhibitory population ``X=='I'`` to extracellular potential contributions by a
-postsynaptic excitatory population ``Y=='E'`` (see https://github.com/LFPy/LFPykernels/blob/main/examples/README_example.ipynb):
+Example prediction of kernel function `$H(\mathbf{R},\tau)$` mapping spike events of a
+presynaptic inhibitory population `$X==\mathrm{I}$` to extracellular potential contributions by a
+postsynaptic excitatory population `$Y==\mathrm{E}$` (see <https://github.com/LFPy/LFPykernels/blob/main/examples/README_example.ipynb>):
 
+    import os
     import matplotlib.pyplot as plt
     import scipy.stats as st
     import numpy as np
     from lfpykernels import GaussCylinderPotential, KernelApprox
     import neuron
 
     # recompile mod files if needed
@@ -240,15 +232,14 @@
 
     # make kernel predictions for connection from populations X='I' onto Y='E'
     H = kernel.get_kernel(
         probes=[probe],
         Vrest=Vrest, dt=dt, X='I', t_X=t_X, tau=tau,
         g_eff=g_eff)
 
-
 ## Physical units
 
 Notes on physical units used in `LFPykernels`:
 
 - There are no explicit checks for physical units
 
 - Transmembrane currents are assumed to be in units of (nA)
@@ -263,115 +254,95 @@
 
 - Magnetic fields are assumed to be in units of (nA/µm)
 
 - Simulation times are assumed to be in units of (ms) with step size ∆t
 
 - Spike rates are assumed to be in units of (# spikes / ∆t)
 
-
 ## Documentation
 
 The online Documentation of `LFPykernels` can be found here:
-https://lfpykernels.readthedocs.io/en/latest
-
+<https://lfpykernels.readthedocs.io/en/latest>
 
 ## Dependencies
 
 `LFPykernels` is implemented in Python and is written (and continuously tested) for `Python >= 3.7` (older versions may or may not work).
-The main `LFPykernels` module depends on ``LFPy`` (https://github.com/LFPy/LFPy, https://LFPy.readthedocs.io).
+The main `LFPykernels` module depends on ``LFPy`` (<https://github.com/LFPy/LFPy>, <https://LFPy.readthedocs.io>).
 
 Running all unit tests and example files may in addition require `py.test`, `matplotlib`,
 `LFPy`.
 
-
 ## Installation
 
-### From development sources (https://github.com/LFPy/LFPykernels)
+### From development sources (<https://github.com/LFPy/LFPykernels>)
 
-Install the current development version on https://GitHub.com using `git` (https://git-scm.com):
+Install the current development version on <https://GitHub.com> using `git` (<https://git-scm.com>):
 
-    $ git clone https://github.com/LFPy/LFPykernels.git
-    $ cd LFPykernels
-    $ python setup.py install  # --user optional
+    git clone https://github.com/LFPy/LFPykernels.git
+    cd LFPykernels
+    python setup.py install  # --user optional
 
 or using `pip`:
 
-    $ pip install .  # --user optional
+    pip install .  # --user optional
 
 For active development, link the repository location
 
-    $ pip install -e .  # --user optional
+    pip install -e .  # --user optional
 
-### Installation of stable releases on PyPI.org (https://www.pypi.org)
+### Installation of stable releases on PyPI.org (<https://www.pypi.org>)
 
-Installing stable releases from the Python Package Index (https://www.pypi.org/project/lfpykernels):
+Installing stable releases from the Python Package Index (<https://www.pypi.org/project/lfpykernels>):
 
-    $ pip install lfpykernels  # --user optional
+    pip install lfpykernels  # --user optional
 
 To upgrade the installation using pip:
 
-    $ pip install --upgrade --no-deps lfpykernels
-
-
-### Installation of stable releases on conda-forge (https://conda-forge.org)
-
-Installing `lfpykernels` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:
-
-    $ conda config --add channels conda-forge
-
-Once the `conda-forge` channel has been enabled, `lfpykernels` can be installed with:
-
-    $ conda install lfpykernels
-
-It is possible to list all of the versions of `lfpykernels` available on your platform with:
-
-    $ conda search lfpykernels --channel conda-forge
-
+    pip install --upgrade --no-deps lfpykernels
 
 ## Docker
 
-We provide a Docker (https://www.docker.com) container recipe file with LFPykernels etc.
+We provide a Docker (<https://www.docker.com>) container recipe file with LFPykernels etc.
 To get started, install Docker and issue either:
 
     # build Dockerfile from GitHub
-    $ docker build -t lfpykernels https://raw.githubusercontent.com/LFPy/LFPykernels/main/Dockerfile
-    $ docker run -it -p 5000:5000 lfpykernels
-
+    docker build -t lfpykernels https://raw.githubusercontent.com/LFPy/LFPykernels/main/Dockerfile
+    docker run -it -p 5000:5000 lfpykernels
 
 or
 
     # build local Dockerfile (obtained by cloning repo, checkout branch etc.)
-    $ docker build -t lfpykernels - < Dockerfile
-    $ docker run -it -p 5000:5000 lfpykernels
-
+    docker build -t lfpykernels - < Dockerfile
+    docker run -it -p 5000:5000 lfpykernels
 
 If the docker file should fail for some reason it is possible to store the build log and avoid build caches by issuing
 
-    $ docker build --no-cache --progress=plain -t lfpykernels - < Dockerfile 2>&1 | tee lfpykernels.log
-
+    docker build --no-cache --progress=plain -t lfpykernels - < Dockerfile 2>&1 | tee lfpykernels.log
 
 For successful builds, the ``--mount`` option can be used to mount a folder on the host to a target folder as:
 
-    $ docker run --mount type=bind,source="$(pwd)",target=/opt/data -it -p 5000:5000 lfpykernels
-
+    docker run --mount type=bind,source="$(pwd)",target=/opt/data -it -p 5000:5000 lfpykernels
 
 which mounts the present working dirctory (``$(pwd)``) to the ``/opt/data`` directory of the container.
 Try mounting the ``LFPykernels`` source directory for example (by setting ``source="<path-to-LFPykernels>"``).
 Various example files can then be found in the folder ``/opt/data/examples/``
 when the container is running.
 
 Jupyter notebook servers running from within the
 container can be accessed after invoking them by issuing:
 
-    $ cd /opt/data/examples/
-    $ jupyter-notebook --ip 0.0.0.0 --port=5000 --no-browser --allow-root
-
+    cd /opt/data/examples/
+    jupyter-notebook --ip 0.0.0.0 --port=5000 --no-browser --allow-root
 
 and opening the resulting URL in a browser on the host computer, similar to:
-http://127.0.0.1:5000/?token=dcf8f859f859740fc858c568bdd5b015e0cf15bfc2c5b0c1
-
+<http://127.0.0.1:5000/?token=dcf8f859f859740fc858c568bdd5b015e0cf15bfc2c5b0c1>
 
 ## Acknowledgements
 
-This work was supported by the European Union Horizon 2020 Research and Innovation Programme under Grant Agreement No. 785907 and No. 945539 Human Brain Project (HBP) SGA2 and SGA3.
-
-
+This work was supported by the European Union Horizon 2020 Research and
+Innovation Programme under Grant Agreement No. 785907 and No. 945539 Human Brain Project (HBP) SGA2 and SGA3.
+We also acknowledge the use of Fenix Infrastructure resources,
+which are partially funded from the European Union’s Horizon 2020 Research and Innovation Programme
+through the ICEI Project under the Grant Agreement No. 800858; The Helmholtz Alliance through the Initiative and
+Networking Fund of the Helmholtz Association and the Helmholtz Portfolio theme Supercomputing
+and Modeling for the Human Brain; and The Excellence Strategy of the Federal Government and
+the La¨nder [G:(DE-82)EXS-PF-JARA-SDS005, G: (DE-82)EXS-SF-neuroIC002].
```

### Comparing `LFPykernels-0.1rc8/LFPykernels.egg-info/SOURCES.txt` & `LFPykernels-0.2.0/LFPykernels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LFPykernels-0.1rc8/LICENSE` & `LFPykernels-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LFPykernels-0.1rc8/MANIFEST.in` & `LFPykernels-0.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `LFPykernels-0.1rc8/PKG-INFO` & `LFPykernels-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: LFPykernels
-Version: 0.1rc8
+Version: 0.2.0
 Summary: Causal spike-signal impulse response functions for finite-sized neuronal network models
 Home-page: https://github.com/LFPy/LFPykernels
 Author: LFPy-team
 Author-email: lfpy@users.noreply.github.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -28,112 +26,106 @@
 License-File: LICENSE
 
 # LFPykernels
 
 The ``LFPykernels`` package incorporates forward-model based calculations of causal spike-signal
 impulse response functions for finite-sized neuronal network models.
 
-
 ## Build Status
 
 [![DOI](https://zenodo.org/badge/424143558.svg)](https://zenodo.org/badge/latestdoi/424143558)
 [![Coverage Status](https://coveralls.io/repos/github/LFPy/LFPykernels/badge.svg?branch=main)](https://coveralls.io/github/LFPy/LFPykernels?branch=main)
 [![Documentation Status](https://readthedocs.org/projects/lfpykernels/badge/?version=latest)](https://lfpykernels.readthedocs.io/en/latest/?badge=latest)
 [![flake8 lint](https://github.com/LFPy/LFPykernels/actions/workflows/flake8.yml/badge.svg)](https://github.com/LFPy/LFPykernels/actions/workflows/flake8.yml)
 [![Python application](https://github.com/LFPy/LFPykernels/workflows/Python%20application/badge.svg)](https://github.com/LFPy/LFPykernels/actions?query=workflow%3A%22Python+application%22)
 [![Upload Python Package](https://github.com/LFPy/LFPykernels/workflows/Upload%20Python%20Package/badge.svg)](https://pypi.org/project/LFPykernels)
-[![Conda Recipe](https://img.shields.io/badge/recipe-lfpykernels-green.svg)](https://anaconda.org/conda-forge/lfpykernels)
-[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/lfpykernels.svg)](https://anaconda.org/conda-forge/lfpykernels)
-[![Conda Version](https://img.shields.io/conda/vn/conda-forge/lfpykernels.svg)](https://anaconda.org/conda-forge/lfpykernels)
-[![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/lfpykernels.svg)](https://anaconda.org/conda-forge/lfpykernels)
 [![License](http://img.shields.io/:license-GPLv3+-green.svg)](http://www.gnu.org/licenses/gpl-3.0.html)
 
-
 ## Citation
 
-If you use this software, please cite it as (change version accordingly):
+These codes correspond to results shown in the peer-reviewed manuscript:
+
+Hagen E, Magnusson SH, Ness TV, Halnes G, Babu PN, et al. (2022)
+Brain signal predictions from multi-scale networks using a linearized framework.
+PLOS Computational Biology 18(8): e1010353. <https://doi.org/10.1371/journal.pcbi.1010353>
 
-    Hagen, Espen. (2021). LFPykernels (version/git-SHA/git-tag). Zenodo. https://doi.org/10.5281/zenodo.5720619
+Bibtex format:
+
+    @article{10.1371/journal.pcbi.1010353,
+        doi = {10.1371/journal.pcbi.1010353},
+        author = {Hagen, Espen AND Magnusson, Steinn H. AND Ness, Torbjørn V. AND Halnes, Geir AND Babu, Pooja N. AND Linssen, Charl AND Morrison, Abigail AND Einevoll, Gaute T.},
+        journal = {PLOS Computational Biology},
+        publisher = {Public Library of Science},
+        title = {Brain signal predictions from multi-scale networks using a linearized framework},
+        year = {2022},
+        month = {08},
+        volume = {18},
+        url = {https://doi.org/10.1371/journal.pcbi.1010353},
+        pages = {1-51},
+        number = {8},
+    }
 
+If you use this software, please cite it as (change `<version>/<git-SHA>/<git-tag>` accordingly):
+
+    Hagen, Espen. (2021). LFPykernels (<version>/<git-SHA>/<git-tag>). Zenodo. https://doi.org/10.5281/zenodo.5720619
 
 BibTex format:
 
     @software{hagen_espen_2021_5720619,
       author       = {Hagen, Espen},
       title        = {LFPykernels},
       month        = nov,
       year         = 2021,
       note         = {If you use this software, please cite it as below.},
       publisher    = {Zenodo},
-      version      = {version/git-SHA/git-tag},
+      version      = {<version>/<git-SHA>/<git-tag>},
       doi          = {10.5281/zenodo.5720619},
       url          = {https://doi.org/10.5281/zenodo.5720619}
     }
 
-
-These codes correspond to results shown in the preprint manuscript:
-
-    Brain signal predictions from multi-scale networks using a linearized framework
-    Espen Hagen, Steinn H. Magnusson, Torbjørn V. Ness, Geir Halnes, Pooja N. Babu, Charl Linssen, Abigail Morrison, Gaute T. Einevoll
-    bioRxiv 2022.02.28.482256; doi: https://doi.org/10.1101/2022.02.28.482256
-
-
-Bibtex format:
-
-    @article {Hagen2022.02.28.482256,
-    	author = {Hagen, Espen and Magnusson, Steinn H. and Ness, Torbjørn V. and Halnes, Geir and Babu, Pooja N. and Linssen, Charl and Morrison, Abigail and Einevoll, Gaute T.},
-    	title = {Brain signal predictions from multi-scale networks using a linearized framework},
-    	elocation-id = {2022.02.28.482256},
-    	year = {2022},
-    	doi = {10.1101/2022.02.28.482256},
-    	publisher = {Cold Spring Harbor Laboratory},
-    	URL = {https://www.biorxiv.org/content/early/2022/03/02/2022.02.28.482256},
-    	eprint = {https://www.biorxiv.org/content/early/2022/03/02/2022.02.28.482256.full.pdf},
-    	journal = {bioRxiv}
-    }
-
 If you use or refer to this work, please cite it as above.
 Adaptations or modifications of this work should comply with the provided `LICENSE` file provided with this repository.  
 
-
 ## Features
 
 The ``LFPykernels`` package incorporates forward-model based calculations of causal spike-signal
 impulse response functions for finite-sized neuronal network models.
 The signals considered are low-frequency extracellular potentials ("local field potential" - LFP)
 or current dipole moments (and by extension EEG and MEG like signals) that are
 thought to mainly stem from synaptic currents and associated return currents.
 The basic idea is that the effect of any spike event in each presynaptic
 population on each signal type can be captured by single linearised multicompartment neuron
 models representative of each population and simultaneously accounting for known distributions of
 cells and synapses in space, distributions of delays, synaptic currents and associated return currents.
 
-A scientific publication describing the present methodology in detail is planned.
+The present methodology is described in detail by [Hagen E et al., 2022](https://doi.org/10.1371/journal.pcbi.1010353).
 The intended use for filter kernels predicted using ``LFPykernels`` is forward-model based signal predictions
 from neuronal network simulation frameworks using simplified neuron representations like leaky integrate-and-fire
-point neurons or rate-based neurons.
-Let ``nu_X(t)`` describe presynaptic population spike rates in units of spikes/dt
-and ``H_YX(r, tau)`` predicted spike-signal kernels for the connections between presynaptic populations ``X`` and
-postsynaptic populations ``Y`` the full signal may then be computed via the sum over linear convolutions
-```
-V(r, t) = sum_X sum_Y conv(nu_X, H_YX)(r, t)
+point neurons or rate-based neurons, but can also be used with biophysically detailed network models.
+
+Let `$\nu_X(t)$` describe presynaptic population spike rates in units of spikes/dt
+and `$H_{YX}(\mathbf{R}, \tau)$` predicted spike-signal kernels for the connections between presynaptic populations `$X$` and
+postsynaptic populations `$Y$` the full signal may then be computed via the sum over linear convolutions:
+
+``` math
+V(\mathbf{R}, t) = \sum_X \sum_Y (\nu_X \ast H_{YX})(\mathbf{R}, t)
 ```
 
 A more elaborate example combining kernel predictions with a spiking point-neuron network simulation is provided in the example notebook
-https://github.com/LFPy/LFPykernels/blob/main/examples/LIF_net_forward_model_predictions.ipynb
-
-For questions, please raise an issue at https://github.com/LFPy/LFPykernels/issues.
+<https://github.com/LFPy/LFPykernels/blob/main/examples/LIF_net_forward_model_predictions.ipynb>
 
+For questions, please raise an issue at <https://github.com/LFPy/LFPykernels/issues>.
 
 ## Usage
 
-Example prediction of kernel function ``H`` mapping spike events of a
-presynaptic inhibitory population ``X=='I'`` to extracellular potential contributions by a
-postsynaptic excitatory population ``Y=='E'`` (see https://github.com/LFPy/LFPykernels/blob/main/examples/README_example.ipynb):
+Example prediction of kernel function `$H(\mathbf{R},\tau)$` mapping spike events of a
+presynaptic inhibitory population `$X==\mathrm{I}$` to extracellular potential contributions by a
+postsynaptic excitatory population `$Y==\mathrm{E}$` (see <https://github.com/LFPy/LFPykernels/blob/main/examples/README_example.ipynb>):
 
+    import os
     import matplotlib.pyplot as plt
     import scipy.stats as st
     import numpy as np
     from lfpykernels import GaussCylinderPotential, KernelApprox
     import neuron
 
     # recompile mod files if needed
@@ -240,15 +232,14 @@
 
     # make kernel predictions for connection from populations X='I' onto Y='E'
     H = kernel.get_kernel(
         probes=[probe],
         Vrest=Vrest, dt=dt, X='I', t_X=t_X, tau=tau,
         g_eff=g_eff)
 
-
 ## Physical units
 
 Notes on physical units used in `LFPykernels`:
 
 - There are no explicit checks for physical units
 
 - Transmembrane currents are assumed to be in units of (nA)
@@ -263,115 +254,95 @@
 
 - Magnetic fields are assumed to be in units of (nA/µm)
 
 - Simulation times are assumed to be in units of (ms) with step size ∆t
 
 - Spike rates are assumed to be in units of (# spikes / ∆t)
 
-
 ## Documentation
 
 The online Documentation of `LFPykernels` can be found here:
-https://lfpykernels.readthedocs.io/en/latest
-
+<https://lfpykernels.readthedocs.io/en/latest>
 
 ## Dependencies
 
 `LFPykernels` is implemented in Python and is written (and continuously tested) for `Python >= 3.7` (older versions may or may not work).
-The main `LFPykernels` module depends on ``LFPy`` (https://github.com/LFPy/LFPy, https://LFPy.readthedocs.io).
+The main `LFPykernels` module depends on ``LFPy`` (<https://github.com/LFPy/LFPy>, <https://LFPy.readthedocs.io>).
 
 Running all unit tests and example files may in addition require `py.test`, `matplotlib`,
 `LFPy`.
 
-
 ## Installation
 
-### From development sources (https://github.com/LFPy/LFPykernels)
+### From development sources (<https://github.com/LFPy/LFPykernels>)
 
-Install the current development version on https://GitHub.com using `git` (https://git-scm.com):
+Install the current development version on <https://GitHub.com> using `git` (<https://git-scm.com>):
 
-    $ git clone https://github.com/LFPy/LFPykernels.git
-    $ cd LFPykernels
-    $ python setup.py install  # --user optional
+    git clone https://github.com/LFPy/LFPykernels.git
+    cd LFPykernels
+    python setup.py install  # --user optional
 
 or using `pip`:
 
-    $ pip install .  # --user optional
+    pip install .  # --user optional
 
 For active development, link the repository location
 
-    $ pip install -e .  # --user optional
+    pip install -e .  # --user optional
 
-### Installation of stable releases on PyPI.org (https://www.pypi.org)
+### Installation of stable releases on PyPI.org (<https://www.pypi.org>)
 
-Installing stable releases from the Python Package Index (https://www.pypi.org/project/lfpykernels):
+Installing stable releases from the Python Package Index (<https://www.pypi.org/project/lfpykernels>):
 
-    $ pip install lfpykernels  # --user optional
+    pip install lfpykernels  # --user optional
 
 To upgrade the installation using pip:
 
-    $ pip install --upgrade --no-deps lfpykernels
-
-
-### Installation of stable releases on conda-forge (https://conda-forge.org)
-
-Installing `lfpykernels` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:
-
-    $ conda config --add channels conda-forge
-
-Once the `conda-forge` channel has been enabled, `lfpykernels` can be installed with:
-
-    $ conda install lfpykernels
-
-It is possible to list all of the versions of `lfpykernels` available on your platform with:
-
-    $ conda search lfpykernels --channel conda-forge
-
+    pip install --upgrade --no-deps lfpykernels
 
 ## Docker
 
-We provide a Docker (https://www.docker.com) container recipe file with LFPykernels etc.
+We provide a Docker (<https://www.docker.com>) container recipe file with LFPykernels etc.
 To get started, install Docker and issue either:
 
     # build Dockerfile from GitHub
-    $ docker build -t lfpykernels https://raw.githubusercontent.com/LFPy/LFPykernels/main/Dockerfile
-    $ docker run -it -p 5000:5000 lfpykernels
-
+    docker build -t lfpykernels https://raw.githubusercontent.com/LFPy/LFPykernels/main/Dockerfile
+    docker run -it -p 5000:5000 lfpykernels
 
 or
 
     # build local Dockerfile (obtained by cloning repo, checkout branch etc.)
-    $ docker build -t lfpykernels - < Dockerfile
-    $ docker run -it -p 5000:5000 lfpykernels
-
+    docker build -t lfpykernels - < Dockerfile
+    docker run -it -p 5000:5000 lfpykernels
 
 If the docker file should fail for some reason it is possible to store the build log and avoid build caches by issuing
 
-    $ docker build --no-cache --progress=plain -t lfpykernels - < Dockerfile 2>&1 | tee lfpykernels.log
-
+    docker build --no-cache --progress=plain -t lfpykernels - < Dockerfile 2>&1 | tee lfpykernels.log
 
 For successful builds, the ``--mount`` option can be used to mount a folder on the host to a target folder as:
 
-    $ docker run --mount type=bind,source="$(pwd)",target=/opt/data -it -p 5000:5000 lfpykernels
-
+    docker run --mount type=bind,source="$(pwd)",target=/opt/data -it -p 5000:5000 lfpykernels
 
 which mounts the present working dirctory (``$(pwd)``) to the ``/opt/data`` directory of the container.
 Try mounting the ``LFPykernels`` source directory for example (by setting ``source="<path-to-LFPykernels>"``).
 Various example files can then be found in the folder ``/opt/data/examples/``
 when the container is running.
 
 Jupyter notebook servers running from within the
 container can be accessed after invoking them by issuing:
 
-    $ cd /opt/data/examples/
-    $ jupyter-notebook --ip 0.0.0.0 --port=5000 --no-browser --allow-root
-
+    cd /opt/data/examples/
+    jupyter-notebook --ip 0.0.0.0 --port=5000 --no-browser --allow-root
 
 and opening the resulting URL in a browser on the host computer, similar to:
-http://127.0.0.1:5000/?token=dcf8f859f859740fc858c568bdd5b015e0cf15bfc2c5b0c1
-
+<http://127.0.0.1:5000/?token=dcf8f859f859740fc858c568bdd5b015e0cf15bfc2c5b0c1>
 
 ## Acknowledgements
 
-This work was supported by the European Union Horizon 2020 Research and Innovation Programme under Grant Agreement No. 785907 and No. 945539 Human Brain Project (HBP) SGA2 and SGA3.
-
-
+This work was supported by the European Union Horizon 2020 Research and
+Innovation Programme under Grant Agreement No. 785907 and No. 945539 Human Brain Project (HBP) SGA2 and SGA3.
+We also acknowledge the use of Fenix Infrastructure resources,
+which are partially funded from the European Union’s Horizon 2020 Research and Innovation Programme
+through the ICEI Project under the Grant Agreement No. 800858; The Helmholtz Alliance through the Initiative and
+Networking Fund of the Helmholtz Association and the Helmholtz Portfolio theme Supercomputing
+and Modeling for the Human Brain; and The Excellence Strategy of the Federal Government and
+the La¨nder [G:(DE-82)EXS-PF-JARA-SDS005, G: (DE-82)EXS-SF-neuroIC002].
```

### Comparing `LFPykernels-0.1rc8/README.md` & `LFPykernels-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,110 +1,104 @@
 # LFPykernels
 
 The ``LFPykernels`` package incorporates forward-model based calculations of causal spike-signal
 impulse response functions for finite-sized neuronal network models.
 
-
 ## Build Status
 
 [![DOI](https://zenodo.org/badge/424143558.svg)](https://zenodo.org/badge/latestdoi/424143558)
 [![Coverage Status](https://coveralls.io/repos/github/LFPy/LFPykernels/badge.svg?branch=main)](https://coveralls.io/github/LFPy/LFPykernels?branch=main)
 [![Documentation Status](https://readthedocs.org/projects/lfpykernels/badge/?version=latest)](https://lfpykernels.readthedocs.io/en/latest/?badge=latest)
 [![flake8 lint](https://github.com/LFPy/LFPykernels/actions/workflows/flake8.yml/badge.svg)](https://github.com/LFPy/LFPykernels/actions/workflows/flake8.yml)
 [![Python application](https://github.com/LFPy/LFPykernels/workflows/Python%20application/badge.svg)](https://github.com/LFPy/LFPykernels/actions?query=workflow%3A%22Python+application%22)
 [![Upload Python Package](https://github.com/LFPy/LFPykernels/workflows/Upload%20Python%20Package/badge.svg)](https://pypi.org/project/LFPykernels)
-[![Conda Recipe](https://img.shields.io/badge/recipe-lfpykernels-green.svg)](https://anaconda.org/conda-forge/lfpykernels)
-[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/lfpykernels.svg)](https://anaconda.org/conda-forge/lfpykernels)
-[![Conda Version](https://img.shields.io/conda/vn/conda-forge/lfpykernels.svg)](https://anaconda.org/conda-forge/lfpykernels)
-[![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/lfpykernels.svg)](https://anaconda.org/conda-forge/lfpykernels)
 [![License](http://img.shields.io/:license-GPLv3+-green.svg)](http://www.gnu.org/licenses/gpl-3.0.html)
 
-
 ## Citation
 
-If you use this software, please cite it as (change version accordingly):
+These codes correspond to results shown in the peer-reviewed manuscript:
+
+Hagen E, Magnusson SH, Ness TV, Halnes G, Babu PN, et al. (2022)
+Brain signal predictions from multi-scale networks using a linearized framework.
+PLOS Computational Biology 18(8): e1010353. <https://doi.org/10.1371/journal.pcbi.1010353>
+
+Bibtex format:
+
+    @article{10.1371/journal.pcbi.1010353,
+        doi = {10.1371/journal.pcbi.1010353},
+        author = {Hagen, Espen AND Magnusson, Steinn H. AND Ness, Torbjørn V. AND Halnes, Geir AND Babu, Pooja N. AND Linssen, Charl AND Morrison, Abigail AND Einevoll, Gaute T.},
+        journal = {PLOS Computational Biology},
+        publisher = {Public Library of Science},
+        title = {Brain signal predictions from multi-scale networks using a linearized framework},
+        year = {2022},
+        month = {08},
+        volume = {18},
+        url = {https://doi.org/10.1371/journal.pcbi.1010353},
+        pages = {1-51},
+        number = {8},
+    }
 
-    Hagen, Espen. (2021). LFPykernels (version/git-SHA/git-tag). Zenodo. https://doi.org/10.5281/zenodo.5720619
+If you use this software, please cite it as (change `<version>/<git-SHA>/<git-tag>` accordingly):
 
+    Hagen, Espen. (2021). LFPykernels (<version>/<git-SHA>/<git-tag>). Zenodo. https://doi.org/10.5281/zenodo.5720619
 
 BibTex format:
 
     @software{hagen_espen_2021_5720619,
       author       = {Hagen, Espen},
       title        = {LFPykernels},
       month        = nov,
       year         = 2021,
       note         = {If you use this software, please cite it as below.},
       publisher    = {Zenodo},
-      version      = {version/git-SHA/git-tag},
+      version      = {<version>/<git-SHA>/<git-tag>},
       doi          = {10.5281/zenodo.5720619},
       url          = {https://doi.org/10.5281/zenodo.5720619}
     }
 
-
-These codes correspond to results shown in the preprint manuscript:
-
-    Brain signal predictions from multi-scale networks using a linearized framework
-    Espen Hagen, Steinn H. Magnusson, Torbjørn V. Ness, Geir Halnes, Pooja N. Babu, Charl Linssen, Abigail Morrison, Gaute T. Einevoll
-    bioRxiv 2022.02.28.482256; doi: https://doi.org/10.1101/2022.02.28.482256
-
-
-Bibtex format:
-
-    @article {Hagen2022.02.28.482256,
-    	author = {Hagen, Espen and Magnusson, Steinn H. and Ness, Torbjørn V. and Halnes, Geir and Babu, Pooja N. and Linssen, Charl and Morrison, Abigail and Einevoll, Gaute T.},
-    	title = {Brain signal predictions from multi-scale networks using a linearized framework},
-    	elocation-id = {2022.02.28.482256},
-    	year = {2022},
-    	doi = {10.1101/2022.02.28.482256},
-    	publisher = {Cold Spring Harbor Laboratory},
-    	URL = {https://www.biorxiv.org/content/early/2022/03/02/2022.02.28.482256},
-    	eprint = {https://www.biorxiv.org/content/early/2022/03/02/2022.02.28.482256.full.pdf},
-    	journal = {bioRxiv}
-    }
-
 If you use or refer to this work, please cite it as above.
 Adaptations or modifications of this work should comply with the provided `LICENSE` file provided with this repository.  
 
-
 ## Features
 
 The ``LFPykernels`` package incorporates forward-model based calculations of causal spike-signal
 impulse response functions for finite-sized neuronal network models.
 The signals considered are low-frequency extracellular potentials ("local field potential" - LFP)
 or current dipole moments (and by extension EEG and MEG like signals) that are
 thought to mainly stem from synaptic currents and associated return currents.
 The basic idea is that the effect of any spike event in each presynaptic
 population on each signal type can be captured by single linearised multicompartment neuron
 models representative of each population and simultaneously accounting for known distributions of
 cells and synapses in space, distributions of delays, synaptic currents and associated return currents.
 
-A scientific publication describing the present methodology in detail is planned.
+The present methodology is described in detail by [Hagen E et al., 2022](https://doi.org/10.1371/journal.pcbi.1010353).
 The intended use for filter kernels predicted using ``LFPykernels`` is forward-model based signal predictions
 from neuronal network simulation frameworks using simplified neuron representations like leaky integrate-and-fire
-point neurons or rate-based neurons.
-Let ``nu_X(t)`` describe presynaptic population spike rates in units of spikes/dt
-and ``H_YX(r, tau)`` predicted spike-signal kernels for the connections between presynaptic populations ``X`` and
-postsynaptic populations ``Y`` the full signal may then be computed via the sum over linear convolutions
-```
-V(r, t) = sum_X sum_Y conv(nu_X, H_YX)(r, t)
+point neurons or rate-based neurons, but can also be used with biophysically detailed network models.
+
+Let `$\nu_X(t)$` describe presynaptic population spike rates in units of spikes/dt
+and `$H_{YX}(\mathbf{R}, \tau)$` predicted spike-signal kernels for the connections between presynaptic populations `$X$` and
+postsynaptic populations `$Y$` the full signal may then be computed via the sum over linear convolutions:
+
+``` math
+V(\mathbf{R}, t) = \sum_X \sum_Y (\nu_X \ast H_{YX})(\mathbf{R}, t)
 ```
 
 A more elaborate example combining kernel predictions with a spiking point-neuron network simulation is provided in the example notebook
-https://github.com/LFPy/LFPykernels/blob/main/examples/LIF_net_forward_model_predictions.ipynb
-
-For questions, please raise an issue at https://github.com/LFPy/LFPykernels/issues.
+<https://github.com/LFPy/LFPykernels/blob/main/examples/LIF_net_forward_model_predictions.ipynb>
 
+For questions, please raise an issue at <https://github.com/LFPy/LFPykernels/issues>.
 
 ## Usage
 
-Example prediction of kernel function ``H`` mapping spike events of a
-presynaptic inhibitory population ``X=='I'`` to extracellular potential contributions by a
-postsynaptic excitatory population ``Y=='E'`` (see https://github.com/LFPy/LFPykernels/blob/main/examples/README_example.ipynb):
+Example prediction of kernel function `$H(\mathbf{R},\tau)$` mapping spike events of a
+presynaptic inhibitory population `$X==\mathrm{I}$` to extracellular potential contributions by a
+postsynaptic excitatory population `$Y==\mathrm{E}$` (see <https://github.com/LFPy/LFPykernels/blob/main/examples/README_example.ipynb>):
 
+    import os
     import matplotlib.pyplot as plt
     import scipy.stats as st
     import numpy as np
     from lfpykernels import GaussCylinderPotential, KernelApprox
     import neuron
 
     # recompile mod files if needed
@@ -211,15 +205,14 @@
 
     # make kernel predictions for connection from populations X='I' onto Y='E'
     H = kernel.get_kernel(
         probes=[probe],
         Vrest=Vrest, dt=dt, X='I', t_X=t_X, tau=tau,
         g_eff=g_eff)
 
-
 ## Physical units
 
 Notes on physical units used in `LFPykernels`:
 
 - There are no explicit checks for physical units
 
 - Transmembrane currents are assumed to be in units of (nA)
@@ -234,113 +227,95 @@
 
 - Magnetic fields are assumed to be in units of (nA/µm)
 
 - Simulation times are assumed to be in units of (ms) with step size ∆t
 
 - Spike rates are assumed to be in units of (# spikes / ∆t)
 
-
 ## Documentation
 
 The online Documentation of `LFPykernels` can be found here:
-https://lfpykernels.readthedocs.io/en/latest
-
+<https://lfpykernels.readthedocs.io/en/latest>
 
 ## Dependencies
 
 `LFPykernels` is implemented in Python and is written (and continuously tested) for `Python >= 3.7` (older versions may or may not work).
-The main `LFPykernels` module depends on ``LFPy`` (https://github.com/LFPy/LFPy, https://LFPy.readthedocs.io).
+The main `LFPykernels` module depends on ``LFPy`` (<https://github.com/LFPy/LFPy>, <https://LFPy.readthedocs.io>).
 
 Running all unit tests and example files may in addition require `py.test`, `matplotlib`,
 `LFPy`.
 
-
 ## Installation
 
-### From development sources (https://github.com/LFPy/LFPykernels)
+### From development sources (<https://github.com/LFPy/LFPykernels>)
 
-Install the current development version on https://GitHub.com using `git` (https://git-scm.com):
+Install the current development version on <https://GitHub.com> using `git` (<https://git-scm.com>):
 
-    $ git clone https://github.com/LFPy/LFPykernels.git
-    $ cd LFPykernels
-    $ python setup.py install  # --user optional
+    git clone https://github.com/LFPy/LFPykernels.git
+    cd LFPykernels
+    python setup.py install  # --user optional
 
 or using `pip`:
 
-    $ pip install .  # --user optional
+    pip install .  # --user optional
 
 For active development, link the repository location
 
-    $ pip install -e .  # --user optional
+    pip install -e .  # --user optional
 
-### Installation of stable releases on PyPI.org (https://www.pypi.org)
+### Installation of stable releases on PyPI.org (<https://www.pypi.org>)
 
-Installing stable releases from the Python Package Index (https://www.pypi.org/project/lfpykernels):
+Installing stable releases from the Python Package Index (<https://www.pypi.org/project/lfpykernels>):
 
-    $ pip install lfpykernels  # --user optional
+    pip install lfpykernels  # --user optional
 
 To upgrade the installation using pip:
 
-    $ pip install --upgrade --no-deps lfpykernels
-
-
-### Installation of stable releases on conda-forge (https://conda-forge.org)
-
-Installing `lfpykernels` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:
-
-    $ conda config --add channels conda-forge
-
-Once the `conda-forge` channel has been enabled, `lfpykernels` can be installed with:
-
-    $ conda install lfpykernels
-
-It is possible to list all of the versions of `lfpykernels` available on your platform with:
-
-    $ conda search lfpykernels --channel conda-forge
-
+    pip install --upgrade --no-deps lfpykernels
 
 ## Docker
 
-We provide a Docker (https://www.docker.com) container recipe file with LFPykernels etc.
+We provide a Docker (<https://www.docker.com>) container recipe file with LFPykernels etc.
 To get started, install Docker and issue either:
 
     # build Dockerfile from GitHub
-    $ docker build -t lfpykernels https://raw.githubusercontent.com/LFPy/LFPykernels/main/Dockerfile
-    $ docker run -it -p 5000:5000 lfpykernels
-
+    docker build -t lfpykernels https://raw.githubusercontent.com/LFPy/LFPykernels/main/Dockerfile
+    docker run -it -p 5000:5000 lfpykernels
 
 or
 
     # build local Dockerfile (obtained by cloning repo, checkout branch etc.)
-    $ docker build -t lfpykernels - < Dockerfile
-    $ docker run -it -p 5000:5000 lfpykernels
-
+    docker build -t lfpykernels - < Dockerfile
+    docker run -it -p 5000:5000 lfpykernels
 
 If the docker file should fail for some reason it is possible to store the build log and avoid build caches by issuing
 
-    $ docker build --no-cache --progress=plain -t lfpykernels - < Dockerfile 2>&1 | tee lfpykernels.log
-
+    docker build --no-cache --progress=plain -t lfpykernels - < Dockerfile 2>&1 | tee lfpykernels.log
 
 For successful builds, the ``--mount`` option can be used to mount a folder on the host to a target folder as:
 
-    $ docker run --mount type=bind,source="$(pwd)",target=/opt/data -it -p 5000:5000 lfpykernels
-
+    docker run --mount type=bind,source="$(pwd)",target=/opt/data -it -p 5000:5000 lfpykernels
 
 which mounts the present working dirctory (``$(pwd)``) to the ``/opt/data`` directory of the container.
 Try mounting the ``LFPykernels`` source directory for example (by setting ``source="<path-to-LFPykernels>"``).
 Various example files can then be found in the folder ``/opt/data/examples/``
 when the container is running.
 
 Jupyter notebook servers running from within the
 container can be accessed after invoking them by issuing:
 
-    $ cd /opt/data/examples/
-    $ jupyter-notebook --ip 0.0.0.0 --port=5000 --no-browser --allow-root
-
+    cd /opt/data/examples/
+    jupyter-notebook --ip 0.0.0.0 --port=5000 --no-browser --allow-root
 
 and opening the resulting URL in a browser on the host computer, similar to:
-http://127.0.0.1:5000/?token=dcf8f859f859740fc858c568bdd5b015e0cf15bfc2c5b0c1
-
+<http://127.0.0.1:5000/?token=dcf8f859f859740fc858c568bdd5b015e0cf15bfc2c5b0c1>
 
 ## Acknowledgements
 
-This work was supported by the European Union Horizon 2020 Research and Innovation Programme under Grant Agreement No. 785907 and No. 945539 Human Brain Project (HBP) SGA2 and SGA3.
+This work was supported by the European Union Horizon 2020 Research and
+Innovation Programme under Grant Agreement No. 785907 and No. 945539 Human Brain Project (HBP) SGA2 and SGA3.
+We also acknowledge the use of Fenix Infrastructure resources,
+which are partially funded from the European Union’s Horizon 2020 Research and Innovation Programme
+through the ICEI Project under the Grant Agreement No. 800858; The Helmholtz Alliance through the Initiative and
+Networking Fund of the Helmholtz Association and the Helmholtz Portfolio theme Supercomputing
+and Modeling for the Human Brain; and The Excellence Strategy of the Federal Government and
+the La¨nder [G:(DE-82)EXS-PF-JARA-SDS005, G: (DE-82)EXS-SF-neuroIC002].
```

### Comparing `LFPykernels-0.1rc8/doc/source/Makefile` & `LFPykernels-0.2.0/doc/source/Makefile`

 * *Files identical despite different names*

### Comparing `LFPykernels-0.1rc8/doc/source/conf.py` & `LFPykernels-0.2.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `LFPykernels-0.1rc8/doc/source/index.rst` & `LFPykernels-0.2.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `LFPykernels-0.1rc8/doc/source/make.bat` & `LFPykernels-0.2.0/doc/source/make.bat`

 * *Files identical despite different names*

### Comparing `LFPykernels-0.1rc8/examples/BallAndSticks_E.hoc` & `LFPykernels-0.2.0/examples/BallAndSticks_E.hoc`

 * *Files identical despite different names*

### Comparing `LFPykernels-0.1rc8/examples/BallAndSticks_I.hoc` & `LFPykernels-0.2.0/examples/BallAndSticks_I.hoc`

 * *Files identical despite different names*

### Comparing `LFPykernels-0.1rc8/examples/FIR_filter.nestml` & `LFPykernels-0.2.0/examples/FIR_filter.nestml`

 * *Files identical despite different names*

### Comparing `LFPykernels-0.1rc8/examples/LIF_net_forward_model_predictions.ipynb` & `LFPykernels-0.2.0/examples/LIF_net_forward_model_predictions.ipynb`

 * *Files identical despite different names*

### Comparing `LFPykernels-0.1rc8/examples/README.md` & `LFPykernels-0.2.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `LFPykernels-0.1rc8/examples/example_network_methods.py` & `LFPykernels-0.2.0/examples/example_network_methods.py`

 * *Files identical despite different names*

### Comparing `LFPykernels-0.1rc8/examples/example_network_parameters.py` & `LFPykernels-0.2.0/examples/example_network_parameters.py`

 * *Files identical despite different names*

### Comparing `LFPykernels-0.1rc8/examples/mod/Ih_linearized_v2_frozen.mod` & `LFPykernels-0.2.0/examples/mod/Ih_linearized_v2_frozen.mod`

 * *Files identical despite different names*

### Comparing `LFPykernels-0.1rc8/examples/mod/NaTa_t_frozen.mod` & `LFPykernels-0.2.0/examples/mod/NaTa_t_frozen.mod`

 * *Files identical despite different names*

### Comparing `LFPykernels-0.1rc8/examples/mod/SKv3_1_frozen.mod` & `LFPykernels-0.2.0/examples/mod/SKv3_1_frozen.mod`

 * *Files identical despite different names*

### Comparing `LFPykernels-0.1rc8/examples/mod/exp2synI.mod` & `LFPykernels-0.2.0/examples/mod/exp2synI.mod`

 * *Files identical despite different names*

### Comparing `LFPykernels-0.1rc8/examples/plotting.py` & `LFPykernels-0.2.0/examples/plotting.py`

 * *Files identical despite different names*

### Comparing `LFPykernels-0.1rc8/lfpykernels/__init__.py` & `LFPykernels-0.2.0/lfpykernels/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
         from presynaptic spiking activity and resulting postsynaptic currents
   * GaussCylinderPotential:
         Compute electric potential of electric sources that are treated as
         inhomogeneous current source density cylinders that are Gaussian along
         the vertical z-axis and constant within a fixed radius in the radial
         directions (xy-plane).
   * KernelApproxCurrentDipoleMoment:
-        Modified ``lfpykit.CurrentDipoleMoment`` class that ignores contributions
-        to the current dipole moment in the the x- and y-directions
-        due to rotational symmetry around the z-axis.
+        Modified ``lfpykit.CurrentDipoleMoment`` class that ignores
+        contributions to the current dipole moment in the the x- and
+        y-directions due to rotational symmetry around the z-axis.
 
 
 :Modules:
   * kernel_approx
   * version
 """
```

### Comparing `LFPykernels-0.1rc8/lfpykernels/kernel_approximator.py` & `LFPykernels-0.2.0/lfpykernels/kernel_approximator.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,29 +43,29 @@
     """
     tp = (tau_1 * tau_2) / (tau_2 - tau_1) * np.log(tau_2 / tau_1)
     u = np.exp(-tp / tau_2) - np.exp(-tp / tau_1)
     return (tau_2 - tau_1) / u
 
 
 class KernelApprox(object):
-    '''Class for computing linear spike-to-signal filter kernels resulting
+    """Class for computing linear spike-to-signal filter kernels resulting
     from presynaptic spiking activity and resulting postsynaptic currents
 
     Parameters
     ----------
     X: list of str
         presynaptic populations
     Y: str
         postsynaptic population
     N_X: array of int
         presynaptic population sizes
     N_Y: int
         postsynaptic population size
     C_YX: array of float
-        pairwise connection probabilities betwen populations X and Y
+        pairwise connection probabilities between populations X and Y
     multapseFunction: callable
         ``scipy.stats.rv_discrete`` or ``scipy.stats.rv_continuous`` like
         function for determining mean number of synapse
         instances per connection between populations X and Y.
         Default is ``scipy.stats.truncnorm``.
     multapseParameters: list of dict
         kwargs for ``multapseFunction``
@@ -95,15 +95,18 @@
         across morphology
     nu_ext: float
         activation rate of extrinsic synapses (1/s)
     n_ext: float
         number of extrinsic synapses
     nu_X: dict of floats
         presynaptic population rates (1/s)
-    '''
+    conductance_based: bool
+        ``True`` (default) if the original network model has conductance-based
+        synapses, ``False`` if it uses current-based synapses
+    """
 
     def __init__(
             self,
             X=['E'],
             Y='E',
             N_X=np.array([1024]),
             N_Y=1024,
@@ -123,15 +126,16 @@
                                                     dict(loc=750., scale=100.)
                                                     ],
                                            funweights=[0.5, 1.])],
             extSynapseParameters=dict(syntype='Exp2Syn', weight=0.0005,
                                       tau1=0.2, tau2=1.8, e=0.0),
             nu_ext=40.,
             n_ext=128.,
-            nu_X=dict(E=1.)
+            nu_X=dict(E=1.),
+            conductance_based=True
     ):
         # set attributes
         self.X = X
         self.Y = Y
         self.N_X = N_X
         self.N_Y = N_Y
         self.C_YX = C_YX
@@ -144,17 +148,18 @@
         self.delayParameters = delayParameters
         self.synapseParameters = synapseParameters
         self.synapsePositionArguments = synapsePositionArguments
         self.extSynapseParameters = extSynapseParameters
         self.nu_ext = nu_ext
         self.n_ext = n_ext
         self.nu_X = nu_X
+        self.conductance_based = conductance_based
 
     def get_delay(self, X, dt, tau):
-        '''Get normalized transfer function for conduction delay distribution
+        """Get normalized transfer function for conduction delay distribution
         for connections between population X and Y
 
         Parameters
         ----------
         X: str
             presynaptic population name
         dt: float
@@ -163,15 +168,15 @@
             time lag
 
         Returns
         -------
         h_delta: ndarray
             shape (2 * tau // dt + 1) array with transfer function for delay
             distribution
-        '''
+        """
         t = np.linspace(-tau, tau, int(2 * tau // dt + 1))
         [i] = np.where(np.array(self.X) == X)[0]
         h_delay = self.delayFunction(**self.delayParameters[i]).pdf(t)
         return h_delay / h_delay.sum()
 
     def draw_rand_pos(self, SIZE, radius, loc, scale, cap=None):
         """
@@ -343,37 +348,38 @@
                 + ' or scipy.stats.rv_continuous')
 
         return multapsedist
 
     def get_kernel(self, probes, Vrest=-65, dt=2**-4,
                    X='E', t_X=200, tau=50,
                    g_eff=True, fir=False):
-        '''Compute linear spike-to-signal filter kernel mapping presynaptic
+        """Compute linear spike-to-signal filter kernel mapping presynaptic
         population firing rates/spike trains to signal measurement, e.g., LFP.
 
         Parameters
         ----------
         probes: list of objects
             list of ``LFPykit.models`` like instances
             (should be instantiated with cell=None).
-        Vrest: float of list of float
+        Vrest: float or list of float
             Mean/Expectation value of postsynaptic membrane voltage used
             for linearization of synapse conductances.
             If list of length equal to the number of compartments, the
             corresponding synapse current magnitude will be computed on a per
             compartment basis.
         dt: float
             temporal resolution (ms)
         X: str
             presynaptic population for kernel, must be element in
             ``<KernelApprox instance>.X``
         t_X: float
             time of presynaptic event (ms)
         tau: float
-            half-duration of filter kernel -- full duration is (2 * tau + dt)
+            half-duration of filter kernel -- full duration
+            is ``(2 * tau + dt)`` if ``fir==False``
         g_eff: bool
             if True (default), account for contributions by synaptic
             conductances to the effective membrane time constant from
             presynaptic populations X and extrinsic connections.
         fir: bool
             if True, return only filter coefficients corresponding to time lags
             greater than zero on the interval [dt, tau] corresponding to that
@@ -381,15 +387,20 @@
             the full set of coefficients on the interval [-tau, tau] is
             returned.
 
         Returns
         -------
         H_YX: dict of ndarray
             shape (n_channels, 2 * tau // dt + 1) linear response kernel
-        '''
+        """
+
+        mssg = "g_eff is True but conductance_based is False." + \
+               "This probably makes no sense...?"
+        assert not (g_eff and (not self.conductance_based)), mssg
+
         # get conduction delay transfer function for connections from X to Y
         h_delta = self.get_delay(X, dt, tau)
 
         # assess index of presynaptic population in X
         (X_i, ) = np.where(np.array(self.X) == X)[0]
 
         # estimate number of connections as in Potjans&Diesmann2014
@@ -410,26 +421,30 @@
 
         # per neuron outdegree
         k_YX_out = K_YX / self.N_X
 
         # class NetworkCell parameters:
         cellParameters = deepcopy(self.cellParameters)
         cellParameters.update(dict(
-            dt=dt,
-            tstop=t_X + tau,
-            delete_sections=True
-        )
+                dt=dt,
+                tstop=t_X + tau,
+                delete_sections=True
+            )
         )
 
         # Create Cell object representative of whole population
         cell = TemplateCell(**cellParameters)
 
+        self.cell = cell  # saving cell for debugging and plotting
         # set cell rotation
         cell.set_rotation(**self.rotationParameters)
 
+        # set cell position
+        cell.set_pos(z=self.populationParameters['loc'])
+
         # need lists of segment references for each cell in order to shift
         # g_pas per segment
         cell.allseglist = neuron.h.List()
         for sec in cell.allseclist:
             for seg in sec:
                 cell.allseglist.append(seg)
 
@@ -477,19 +492,19 @@
             # mean (z_mean + u_mean) and st.dev sqrt(z_std^2 + u_std^2)
             syn_pos = deepcopy(self.synapsePositionArguments[iii])
 
             for h, funarg in enumerate(syn_pos['funargs']):
                 # NOTE: ignoring shifting synapse placements by the mean
                 # somatic depth, which may be implemented as:
                 # syn_pos['funargs'][h]['loc'] = \
-                #     funarg['loc'] + self.populationParameters['loc']
+                #    funarg['loc'] + self.populationParameters['loc']
+
                 syn_pos['funargs'][h]['scale'] = \
                     np.sqrt(funarg['scale']**2 +
                             self.populationParameters['scale']**2)
-
             # per-compartment connection probability
             p = self.get_rand_idx_area_and_distribution_prob(
                 cell,
                 **syn_pos)
 
             # synapses per compartment for each connection.
             # Distinguish between input densities and outdegrees as
@@ -518,28 +533,35 @@
                     errmsg = '{} not supported'.format(extPar['syntype'])
                     raise NotImplementedError(errmsg)
 
             if iii == X_i:
                 # modify synapse parameters to account for current-based
                 # synapses linearized around Vrest
                 d = self.synapseParameters[iii].copy()
-                if isinstance(Vrest, (int, float)):
-                    w = [- d['weight'] * (Vrest - d['e'])] * cell.totnsegs
-                    # d['weight'] = - d['weight'] * (Vrest - d['e'])
+
+                if self.conductance_based:
+                    if isinstance(Vrest, (int, float)):
+                        w = [- d['weight'] * (Vrest - d['e'])] * cell.totnsegs
+                        # d['weight'] = - d['weight'] * (Vrest - d['e'])
+                    else:
+                        w = [- d['weight'] * (Vr - d['e']) for Vr in Vrest]
+                    del d['e']  # no longer needed
+                    d['syntype'] = d['syntype'] + 'I'
                 else:
-                    w = [- d['weight'] * (Vr - d['e']) for Vr in Vrest]
-                del d['e']  # no longer needed
-                d['syntype'] = d['syntype'] + 'I'
+                    w = [d['weight']] * cell.totnsegs
 
                 # create current synapses activated by spike time of
                 # presynaptic population X
                 # setting weight scaled by synapses per compartment
+                # saving comp_weight for debugging purposes
+                self.comp_weight = np.zeros(cell.totnsegs)
                 for idx, w_idx in enumerate(w):
                     di = d.copy()
                     di['weight'] = w_idx * rho_YX_out[idx]
+                    self.comp_weight[idx] = di['weight']
                     # di['weight'] = di['weight'] * rho_YX_out[idx]
                     syn = Synapse(cell, idx=idx, **di)
                     syn.set_spike_times(np.array([t_X]))
 
         # simulate and record transmembrane currents
         cell.simulate(rec_imem=True)
 
@@ -547,14 +569,15 @@
         if fir:
             inds = (cell.tvec > t_X) & (cell.tvec <= (t_X + tau))
         else:
             inds = (cell.tvec >= (t_X - tau)) & (cell.tvec <= (t_X + tau))
         H_YX = dict()
         for probe in probes:
             probe.cell = cell
+
             if probe.__class__.__name__ in ['PointSourcePotential',
                                             'LineSourcePotential']:
                 warn('results are non-deterministic for ' +
                      f'probe {probe.__class__.__name__}.' +
                      'Support may be deprecated in the future.')
                 # draw offsets from the distribution of cells in space
                 # with homogeneous density
@@ -586,15 +609,16 @@
             data = M @ cell.imem
 
             # apply delay distribution function
             for h, d in enumerate(data):
                 data[h, ] = np.convolve(d, h_delta, 'same')
 
             # subtract kernel offsets at tau == 0:
-            data = data - data[:, cell.tvec == t_X]
+            t_idx_ = np.argmin(np.abs(cell.tvec - t_X))
+            data = data - data[:, t_idx_, None]
 
             # force negative time lags to be zero
             data[:, cell.tvec < t_X] = 0
 
             # extract kernel
             H_YX[probe.__class__.__name__] = data[:, inds]
 
@@ -650,27 +674,27 @@
         return np.exp(-(z / self.sigma_z)**2 / 2) / (
             self.sigma_z * np.sqrt(2 * np.pi))
 
     def _func(self, z, z_e=0, z_i=0):
         return self._f(z_e - z, z_i) * self._g(z)
 
     def get_transformation_matrix(self):
-        '''
+        """
         Get linear response matrix
 
         Returns
         -------
         response_matrix: ndarray
             shape (n_coords, n_seg) ndarray
 
         Raises
         ------
         AttributeError
             if ``cell is None``
-        '''
+        """
         if self.cell is None:
             raise AttributeError(
                 '{}.cell is None'.format(self.__class__.__name__))
         M = np.empty((self.z.size, self.cell.totnsegs))
         for j, z_e in enumerate(self.z):
             for i in range(self.cell.totnsegs):
                 M[j, i], _ = si.quad(self._func, -np.inf, np.inf,
@@ -679,15 +703,15 @@
         M /= (np.pi * self.R**2)  # Distribute current evenly across surface
 
         return M
 
 
 class KernelApproxCurrentDipoleMoment(lfpykit.CurrentDipoleMoment):
     """Modified ``lfpykit.CurrentDipoleMoment`` like class that ignores
-    contributions to the current dipole moment in the the x- and y-directions
+    contributions to the current dipole moment in the x- and y-directions
     due to rotational symmetry around the z-axis.
 
     Parameters
     ----------
     cell: object
         ``CellGeometry`` object or similar
     """
```

### Comparing `LFPykernels-0.1rc8/lfpykernels/tests/BallAndSticks_E.hoc` & `LFPykernels-0.2.0/lfpykernels/tests/BallAndSticks_E.hoc`

 * *Files identical despite different names*

### Comparing `LFPykernels-0.1rc8/lfpykernels/tests/exp2synI.mod` & `LFPykernels-0.2.0/lfpykernels/tests/exp2synI.mod`

 * *Files identical despite different names*

### Comparing `LFPykernels-0.1rc8/lfpykernels/tests/test_module.py` & `LFPykernels-0.2.0/lfpykernels/tests/test_module.py`

 * *Files 20% similar despite different names*

```diff
@@ -41,14 +41,77 @@
                                 y=np.array([[0.] * 2] * n_seg),
                                 z=np.array([[1. * x, 1. * (x + 1)]
                                             for x in range(n_seg)]),
                                 d=np.array([1.] * n_seg))
     return cell
 
 
+def set_passive(cell, Vrest):
+    """Insert passive leak channel across all sections
+
+    Parameters
+    ----------
+    cell: object
+        LFPy.NetworkCell like object
+    Vrest: float
+        Steady state potential
+    """
+    for sec in cell.template.all:
+        sec.insert('pas')
+        sec.g_pas = 0.0003  # (S/cm2)
+        sec.e_pas = Vrest  # (mV)
+
+
+def check_kernelApprox(dt, tau, Vrest, params):
+    # instantiate object
+    kernel = lfpykernels.KernelApprox(
+        **params
+    )
+
+    # check delay distribution
+    delay = kernel.get_delay('E', dt=dt, tau=tau)
+    assert delay.shape == (int(tau // dt) * 2 + 1, )
+    assert delay.min() == 0
+    assert np.all(delay[:int(tau // dt) + 1] == 0)
+    np.testing.assert_almost_equal(delay.sum(), 1)
+
+    # check get_rand_idx_area_and_distribution_prob method with
+    # a uniform distribution
+    cell = LFPy.TemplateCell(**params['cellParameters'])
+    p = kernel.get_rand_idx_area_and_distribution_prob(
+        cell,
+        section='allsec',
+        fun=st.uniform,
+        funargs=dict(loc=-1E3, scale=2E3))
+    np.testing.assert_allclose(p, cell.area / cell.area.sum())
+
+    # check kernel predictions using two different forward models
+    z = np.linspace(-500, 500, 11)
+    gauss = lfpykernels.GaussCylinderPotential(
+        cell=None, z=z, sigma=0.3, R=100, sigma_z=100
+    )
+
+    cdm = lfpykernels.KernelApproxCurrentDipoleMoment(cell=None)
+
+    H_EE = kernel.get_kernel(probes=(gauss, cdm), Vrest=Vrest, X='E',
+                             dt=dt, tau=tau, t_X=200, g_eff=True)
+
+    assert (H_EE['GaussCylinderPotential'].shape
+            == (z.size, int(2 * tau // dt) + 1))
+    assert np.all(H_EE['GaussCylinderPotential'][:, :int(tau // dt) + 1]
+                  == 0)
+    assert (H_EE['KernelApproxCurrentDipoleMoment'].shape
+            == (3, int(2 * tau // dt) + 1))
+    assert np.all(
+        H_EE['KernelApproxCurrentDipoleMoment'][:, :int(tau // dt) + 1]
+        == 0)
+
+    return H_EE
+
+
 class TestSuite(unittest.TestCase):
     """
     test methods and modules
     """
 
     def test_TestSuite_00(self):
         '''test TestSuite'''
@@ -103,43 +166,79 @@
         )
 
         np.testing.assert_allclose(point.get_transformation_matrix(),
                                    gauss.get_transformation_matrix())
 
     def test_KernelApprox_00(self):
         '''test that the basic methods of the KernelApprox class works'''
+        # parameters
+        Vrest = -65.
+        dt = 2**-4
+        tau = 100.
+
+        cellParameters = dict(
+            templatefile=os.path.join(lfpykernels.__path__[0], 'tests',
+                                      'BallAndSticksTemplate.hoc'),
+            templatename='BallAndSticksTemplate',
+            custom_fun=[set_passive],
+            custom_fun_args=[{'Vrest': Vrest}],
+            templateargs=None,
+            delete_sections=True,
+            morphology=os.path.join(lfpykernels.__path__[0], 'tests',
+                                    'BallAndSticks_E.hoc')
+        )
 
-        def set_passive(cell, Vrest):
-            """Insert passive leak channel across all sections
+        populationParameters = dict(radius=100, loc=0, scale=50)
+
+        params = dict(
+            X=['E'],
+            Y='E',
+            N_X=np.array([1024]),
+            N_Y=1024,
+            C_YX=np.array([0.1]),
+            cellParameters=cellParameters,
+            populationParameters=populationParameters,
+            rotationParameters=dict(x=0., y=0.),
+            multapseFunction=st.truncnorm,
+            multapseParameters=[dict(a=-0.2, b=1.6, loc=2, scale=5)],
+            delayFunction=st.truncnorm,
+            delayParameters=[dict(a=-4.0, b=np.inf, loc=1.5, scale=0.3)],
+            synapseParameters=[dict(weight=0.001, syntype='Exp2Syn',
+                                    tau1=0.2, tau2=1.8, e=0.)],
+            synapsePositionArguments=[dict(section=['soma', 'apic'],
+                                           fun=[st.norm, st.norm],
+                                           funargs=[dict(loc=0., scale=100.),
+                                                    dict(loc=750., scale=100.)
+                                                    ],
+                                           funweights=[0.5, 1.])],
+            extSynapseParameters=dict(syntype='Exp2Syn', weight=0.0005,
+                                      tau1=0.2, tau2=1.8, e=0.0),
+            nu_ext=40.,
+            n_ext=128.,
+            nu_X=dict(E=1.)
+        )
 
-            Parameters
-            ----------
-            cell: object
-                LFPy.NetworkCell like object
-            Vrest: float
-                Steady state potential
-            """
-            for sec in cell.template.all:
-                sec.insert('pas')
-                sec.g_pas = 0.0003  # (S/cm2)
-                sec.e_pas = Vrest  # (mV)
+        _ = check_kernelApprox(dt, tau, Vrest, params)
 
+    def test_KernelApprox_01(self):
+        '''test that the basic methods of the KernelApprox class works
+        with offset cell positions along z-axis'''
         # parameters
         Vrest = -65.
         dt = 2**-4
         tau = 100.
 
         cellParameters = dict(
             templatefile=os.path.join(lfpykernels.__path__[0], 'tests',
                                       'BallAndSticksTemplate.hoc'),
             templatename='BallAndSticksTemplate',
             custom_fun=[set_passive],
             custom_fun_args=[{'Vrest': Vrest}],
             templateargs=None,
-            delete_sections=False,
+            delete_sections=True,
             morphology=os.path.join(lfpykernels.__path__[0], 'tests',
                                     'BallAndSticks_E.hoc')
         )
 
         populationParameters = dict(radius=100, loc=0, scale=50)
 
         params = dict(
@@ -166,49 +265,48 @@
             extSynapseParameters=dict(syntype='Exp2Syn', weight=0.0005,
                                       tau1=0.2, tau2=1.8, e=0.0),
             nu_ext=40.,
             n_ext=128.,
             nu_X=dict(E=1.)
         )
 
-        # instantiate object
-        kernel = lfpykernels.KernelApprox(
-            **params
-        )
-
-        # check delay distribution
-        delay = kernel.get_delay('E', dt=dt, tau=tau)
-        assert delay.shape == (int(tau // dt) * 2 + 1, )
-        assert delay.min() == 0
-        assert np.all(delay[:int(tau // dt) + 1] == 0)
-        np.testing.assert_almost_equal(delay.sum(), 1)
-
-        # check get_rand_idx_area_and_distribution_prob method with
-        # a uniform distribution
-        cell = LFPy.TemplateCell(**cellParameters)
-        p = kernel.get_rand_idx_area_and_distribution_prob(
-            cell,
-            section='allsec',
-            fun=st.uniform,
-            funargs=dict(loc=-1E3, scale=2E3))
-        np.testing.assert_allclose(p, cell.area / cell.area.sum())
+        H_EE = check_kernelApprox(dt, tau, Vrest, params)
 
-        # check kernel predictions using two different forward models
-        z = np.linspace(-500, 500, 11)
-        gauss = lfpykernels.GaussCylinderPotential(
-            cell=None, z=z, sigma=0.3, R=100, sigma_z=100
-        )
+        # offset by 200µm along z-axis
+        populationParameters = dict(radius=100, loc=200, scale=50)
 
-        cdm = lfpykernels.KernelApproxCurrentDipoleMoment(cell=None)
+        params = dict(
+            X=['E'],
+            Y='E',
+            N_X=np.array([1024]),
+            N_Y=1024,
+            C_YX=np.array([0.1]),
+            cellParameters=cellParameters,
+            populationParameters=populationParameters,
+            rotationParameters=dict(x=0., y=0.),
+            multapseFunction=st.truncnorm,
+            multapseParameters=[dict(a=-0.2, b=1.6, loc=2, scale=5)],
+            delayFunction=st.truncnorm,
+            delayParameters=[dict(a=-4.0, b=np.inf, loc=1.5, scale=0.3)],
+            synapseParameters=[dict(weight=0.001, syntype='Exp2Syn',
+                                    tau1=0.2, tau2=1.8, e=0.)],
+            synapsePositionArguments=[
+                dict(section=['soma', 'apic'],
+                     fun=[st.norm, st.norm],
+                     funargs=[dict(loc=0. + populationParameters['loc'],
+                                   scale=100.),
+                              dict(loc=750. + populationParameters['loc'],
+                                   scale=100.)
+                              ],
+                     funweights=[0.5, 1.])],
+            extSynapseParameters=dict(syntype='Exp2Syn', weight=0.0005,
+                                      tau1=0.2, tau2=1.8, e=0.0),
+            nu_ext=40.,
+            n_ext=128.,
+            nu_X=dict(E=1.)
+        )
 
-        H_EE = kernel.get_kernel(probes=(gauss, cdm), Vrest=Vrest, X='E',
-                                 dt=dt, tau=tau, t_X=200, g_eff=True)
+        H_EE_offset = check_kernelApprox(dt, tau, Vrest, params)
 
-        assert (H_EE['GaussCylinderPotential'].shape
-                == (z.size, int(2 * tau // dt) + 1))
-        assert np.all(H_EE['GaussCylinderPotential'][:, :int(tau // dt) + 1]
-                      == 0)
-        assert (H_EE['KernelApproxCurrentDipoleMoment'].shape
-                == (3, int(2 * tau // dt) + 1))
-        assert np.all(
-            H_EE['KernelApproxCurrentDipoleMoment'][:, :int(tau // dt) + 1]
-            == 0)
+        # check that results translated by 200µm vertically match
+        np.testing.assert_allclose(H_EE['GaussCylinderPotential'][:-2, ],
+                                   H_EE_offset['GaussCylinderPotential'][2:, ])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `LFPykernels-0.1rc8/setup.py` & `LFPykernels-0.2.0/setup.py`

 * *Files identical despite different names*

