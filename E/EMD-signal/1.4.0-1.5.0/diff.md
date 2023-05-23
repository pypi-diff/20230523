# Comparing `tmp/EMD-signal-1.4.0.tar.gz` & `tmp/EMD-signal-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EMD-signal-1.4.0.tar", last modified: Mon Dec 19 23:51:39 2022, max compression
+gzip compressed data, was "EMD-signal-1.5.0.tar", last modified: Tue May 23 21:46:01 2023, max compression
```

## Comparing `EMD-signal-1.4.0.tar` & `EMD-signal-1.5.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 23:51:39.734841 EMD-signal-1.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 23:51:39.726840 EMD-signal-1.4.0/EMD_signal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2022-12-19 23:51:39.000000 EMD-signal-1.4.0/EMD_signal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2022-12-19 23:51:39.000000 EMD-signal-1.4.0/EMD_signal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 23:51:39.000000 EMD-signal-1.4.0/EMD_signal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      203 2022-12-19 23:51:39.000000 EMD-signal-1.4.0/EMD_signal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-19 23:51:39.000000 EMD-signal-1.4.0/EMD_signal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      187 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2022-12-19 23:51:39.734841 EMD-signal-1.4.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 23:51:39.730841 EMD-signal-1.4.0/PyEMD/
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/BEMD.py
--rw-r--r--   0 runner    (1001) docker     (123)    15219 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/CEEMDAN.py
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/EEMD.py
--rw-r--r--   0 runner    (1001) docker     (123)    37466 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/EMD.py
--rw-r--r--   0 runner    (1001) docker     (123)    14028 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/EMD2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    23496 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/EMD_matlab.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/compact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 23:51:39.730841 EMD-signal-1.4.0/PyEMD/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34772 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/experimental/jitemd.py
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/splines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 23:51:39.734841 EMD-signal-1.4.0/PyEMD/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/tests/test_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/tests/test_bemd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/tests/test_ceemdan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/tests/test_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/tests/test_eemd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7366 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/tests/test_emd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/tests/test_emd2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10448 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/tests/test_extrema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/tests/test_splines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/tests/test_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/PyEMD/visualisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 23:51:39.734841 EMD-signal-1.4.0/example/
--rw-r--r--   0 runner    (1001) docker     (123)      924 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/example/eemd_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/example/emd_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/example/hht_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/example/image_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/example/jit_eemd_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/example/jit_emd_class_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/example/jit_emd_function_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/example/simple_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-19 23:51:22.000000 EMD-signal-1.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2022-12-19 23:51:39.734841 EMD-signal-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:46:01.102456 EMD-signal-1.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:46:01.094456 EMD-signal-1.5.0/EMD_signal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-05-23 21:46:01.000000 EMD-signal-1.5.0/EMD_signal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-23 21:46:01.000000 EMD-signal-1.5.0/EMD_signal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:46:01.000000 EMD-signal-1.5.0/EMD_signal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-23 21:46:01.000000 EMD-signal-1.5.0/EMD_signal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 21:46:01.000000 EMD-signal-1.5.0/EMD_signal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-05-23 21:46:01.102456 EMD-signal-1.5.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:46:01.094456 EMD-signal-1.5.0/PyEMD/
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/BEMD.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/CEEMDAN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/EEMD.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37661 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/EMD.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14025 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/EMD2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23480 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/EMD_matlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/compact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:46:01.094456 EMD-signal-1.5.0/PyEMD/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34760 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/experimental/jitemd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/splines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:46:01.098456 EMD-signal-1.5.0/PyEMD/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/tests/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/tests/test_bemd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/tests/test_ceemdan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/tests/test_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/tests/test_eemd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/tests/test_emd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/tests/test_emd2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10448 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/tests/test_extrema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/tests/test_splines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/tests/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/PyEMD/visualisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:46:01.102456 EMD-signal-1.5.0/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/example/eemd_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/example/emd_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/example/example_spline_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/example/hht_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/example/image_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/example/jit_eemd_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/example/jit_emd_class_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/example/jit_emd_function_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/example/simple_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 21:45:47.000000 EMD-signal-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-23 21:46:01.102456 EMD-signal-1.5.0/setup.cfg
```

### Comparing `EMD-signal-1.4.0/EMD_signal.egg-info/PKG-INFO` & `EMD-signal-1.5.0/EMD_signal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EMD-signal
-Version: 1.4.0
+Version: 1.5.0
 Summary: Implementation of the Empirical Mode Decomposition (EMD) and its variations
 Home-page: https://github.com/laszukdawid/PyEMD
 Author: Dawid Laszuk
 Author-email: pyemd@dawid.lasz.uk
 License: Apache-2.0
 Keywords: signal decomposition data analysis
 Classifier: Intended Audience :: Information Technology
@@ -32,15 +32,15 @@
 
 - Online documentation: <https://pyemd.readthedocs.org>
 - Issue tracker: <https://github.com/laszukdawid/pyemd/issues>
 - Source code repository: <https://github.com/laszukdawid/pyemd>
 
 ## Introduction
 
-This is yet another Python implementation of Empirical Mode
+Python implementation of the Empirical Mode
 Decomposition (EMD). The package contains multiple EMD variations and
 intends to deliver more in time.
 
 ### EMD variations
 
 -  Ensemble EMD (EEMD),
 -  "Complete Ensemble EMD" (CEEMDAN)
@@ -51,15 +51,17 @@
 *PyEMD* allows you to use different splines for envelopes, stopping criteria
 and extrema interpolations.
 
 ### Available splines
 
 -  Natural cubic (**default**)
 -  Pointwise cubic
+-  Hermite cubic
 -  Akima
+-  PChip
 -  Linear
 
 ### Available stopping criteria
 
 -  Cauchy convergence (**default**)
 -  Fixed number of iterations
 -  Number of consecutive proto-imfs
```

### Comparing `EMD-signal-1.4.0/EMD_signal.egg-info/SOURCES.txt` & `EMD-signal-1.5.0/EMD_signal.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -36,13 +36,14 @@
 PyEMD/tests/test_emd2d.py
 PyEMD/tests/test_extrema.py
 PyEMD/tests/test_splines.py
 PyEMD/tests/test_utils.py
 PyEMD/tests/test_visualization.py
 example/eemd_example.py
 example/emd_comparison.py
+example/example_spline_capabilities.py
 example/hht_example.py
 example/image_example.py
 example/jit_eemd_example.py
 example/jit_emd_class_example.py
 example/jit_emd_function_example.py
 example/simple_example.py
```

### Comparing `EMD-signal-1.4.0/LICENSE.md` & `EMD-signal-1.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `EMD-signal-1.4.0/PKG-INFO` & `EMD-signal-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EMD-signal
-Version: 1.4.0
+Version: 1.5.0
 Summary: Implementation of the Empirical Mode Decomposition (EMD) and its variations
 Home-page: https://github.com/laszukdawid/PyEMD
 Author: Dawid Laszuk
 Author-email: pyemd@dawid.lasz.uk
 License: Apache-2.0
 Keywords: signal decomposition data analysis
 Classifier: Intended Audience :: Information Technology
@@ -32,15 +32,15 @@
 
 - Online documentation: <https://pyemd.readthedocs.org>
 - Issue tracker: <https://github.com/laszukdawid/pyemd/issues>
 - Source code repository: <https://github.com/laszukdawid/pyemd>
 
 ## Introduction
 
-This is yet another Python implementation of Empirical Mode
+Python implementation of the Empirical Mode
 Decomposition (EMD). The package contains multiple EMD variations and
 intends to deliver more in time.
 
 ### EMD variations
 
 -  Ensemble EMD (EEMD),
 -  "Complete Ensemble EMD" (CEEMDAN)
@@ -51,15 +51,17 @@
 *PyEMD* allows you to use different splines for envelopes, stopping criteria
 and extrema interpolations.
 
 ### Available splines
 
 -  Natural cubic (**default**)
 -  Pointwise cubic
+-  Hermite cubic
 -  Akima
+-  PChip
 -  Linear
 
 ### Available stopping criteria
 
 -  Cauchy convergence (**default**)
 -  Fixed number of iterations
 -  Number of consecutive proto-imfs
```

### Comparing `EMD-signal-1.4.0/PyEMD/BEMD.py` & `EMD-signal-1.5.0/PyEMD/BEMD.py`

 * *Files identical despite different names*

### Comparing `EMD-signal-1.4.0/PyEMD/CEEMDAN.py` & `EMD-signal-1.5.0/PyEMD/CEEMDAN.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,14 @@
     """
 
     logger = logging.getLogger(__name__)
 
     noise_kinds_all = ["normal", "uniform"]
 
     def __init__(self, trials: int = 100, epsilon: float = 0.005, ext_EMD=None, parallel: bool = False, **kwargs):
-
         # Ensemble constants
         self.trials = trials
         self.epsilon = epsilon
         self.noise_scale = float(kwargs.get("noise_scale", 1.0))
         self.range_thr = float(kwargs.get("range_thr", 0.01))
         self.total_power_thr = float(kwargs.get("total_power_thr", 0.05))
```

### Comparing `EMD-signal-1.4.0/PyEMD/EEMD.py` & `EMD-signal-1.5.0/PyEMD/EEMD.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
     """
 
     logger = logging.getLogger(__name__)
 
     noise_kinds_all = ["normal", "uniform"]
 
     def __init__(self, trials: int = 100, noise_width: float = 0.05, ext_EMD=None, parallel: bool = False, **kwargs):
-
         # Ensemble constants
         self.trials = trials
         self.noise_width = noise_width
         self.separate_trends = bool(kwargs.get("separate_trends", False))
 
         self.random = np.random.RandomState()
         self.noise_kind = kwargs.get("noise_kind", "normal")
@@ -190,16 +189,15 @@
         all_IMFs = map_pool(self._trial_update, range(self.trials))
 
         if self.parallel:
             map_pool.close()
 
         self._all_imfs = defaultdict(list)
         it = iter if not progress else lambda x: tqdm(x, desc="EEMD", total=self.trials)
-        for (imfs, trend) in it(all_IMFs):
-
+        for imfs, trend in it(all_IMFs):
             # A bit of explanation here.
             # If the `trend` is not None, that means it was intentionally separated in the decomp process.
             # This might due to `separate_trends` flag which means that trends are summed up separately
             # and treated as the last component. Since `proto_eimfs` is a dict, that `-1` is treated literally
             # and **not** as the *last position*. We can then use that `-1` to always add it as the last pos
             # in the actual eIMF, which indicates the trend.
             if trend is not None:
@@ -273,15 +271,14 @@
         """Pointwise standard deviation over computed ensemble."""
         return np.array([imfs.std(axis=0) for imfs in self._all_imfs.values()])
 
 
 ###################################################
 # Beginning of program
 if __name__ == "__main__":
-
     import pylab as plt
 
     E_imfNo = np.zeros(50, dtype=np.int)
 
     # Logging options
     logging.basicConfig(level=logging.INFO)
```

### Comparing `EMD-signal-1.4.0/PyEMD/EMD.py` & `EMD-signal-1.5.0/PyEMD/EMD.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import logging
 from typing import Optional, Tuple
 
 import numpy as np
 from scipy.interpolate import interp1d
 
-from PyEMD.splines import akima, cubic_spline_3pts
+from PyEMD.splines import akima, cubic_spline_3pts, cubic, pchip, cubic_hermite
 from PyEMD.utils import get_timeline
 
 FindExtremaOutput = Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray]
 
 
 class EMD:
     """
@@ -477,18 +477,24 @@
         t = T[np.r_[T >= extrema[0, 0]] & np.r_[T <= extrema[0, -1]]]
 
         if kind == "akima":
             return t, akima(extrema[0], extrema[1], t)
 
         elif kind == "cubic":
             if extrema.shape[1] > 3:
-                return t, interp1d(extrema[0], extrema[1], kind=kind)(t)
+                return t, cubic(extrema[0], extrema[1], t)
             else:
                 return cubic_spline_3pts(extrema[0], extrema[1], t)
 
+        elif kind == "pchip":
+            return t, pchip(extrema[0], extrema[1], t)
+
+        elif kind == "cubic_hermite":
+            return t, cubic_hermite(extrema[0], extrema[1], t)
+
         elif kind in ["slinear", "quadratic", "linear"]:
             return T, interp1d(extrema[0], extrema[1], kind=kind)(t).astype(self.DTYPE)
 
         else:
             raise ValueError("No such interpolation method!")
 
     @staticmethod
@@ -580,15 +586,15 @@
         # a = Sn + Sp - 2*S0
         # b = 2*(Tn+Tp)*S0 - ((Tn+T0)*Sp+(T0+Tp)*Sn)
         # c = Sp*T0*Tn -2*Tp*S0*Tn + Tp*T0*Sn
         TnTp, T0Tn, TpT0 = Tn - Tp, T0 - Tn, Tp - T0
         scale = Tp * Tn * Tn + Tp * Tp * T0 + T0 * T0 * Tn - Tp * Tp * Tn - Tp * T0 * T0 - T0 * Tn * Tn
 
         a = T0Tn * Sp + TnTp * S0 + TpT0 * Sn
-        b = (S0 - Sn) * Tp ** 2 + (Sn - Sp) * T0 ** 2 + (Sp - S0) * Tn ** 2
+        b = (S0 - Sn) * Tp**2 + (Sn - Sp) * T0**2 + (Sp - S0) * Tn**2
         c = T0 * Tn * T0Tn * Sp + Tn * Tp * TnTp * S0 + Tp * T0 * TpT0 * Sn
 
         a = a / scale
         b = b / scale
         c = c / scale
         a[a == 0] = 1e-14
         tVertex = -0.5 * b / a
@@ -630,15 +636,14 @@
         d = np.diff(S)
         d1, d2 = d[:-1], d[1:]
         indmin = np.nonzero(np.r_[d1 * d2 < 0] & np.r_[d1 < 0])[0] + 1
         indmax = np.nonzero(np.r_[d1 * d2 < 0] & np.r_[d1 > 0])[0] + 1
 
         # When two or more points have the same value
         if np.any(d == 0):
-
             imax, imin = [], []
 
             bad = d == 0
             dd = np.diff(np.append(np.append(0, bad), 0))
             debs = np.nonzero(dd == 1)[0]
             fins = np.nonzero(dd == -1)[0]
             if debs[0] == 1:
@@ -727,15 +732,15 @@
         in a significant manner.
         """
         # local max are >0 and local min are <0
         if np.any(eMax[1] < 0) or np.any(eMin[1] > 0):
             return False
 
         # Convergence
-        if np.sum(imf_new ** 2) < 1e-10:
+        if np.sum(imf_new**2) < 1e-10:
             return False
 
         # Precompute values
         imf_diff = imf_new - imf_old
         imf_diff_sqrd_sum = np.sum(imf_diff * imf_diff)
 
         # Scaled variance test
@@ -846,15 +851,14 @@
 
                 ext_res = self.find_extrema(T, imf)
                 max_pos, min_pos, indzer = ext_res[0], ext_res[2], ext_res[4]
                 extNo = len(min_pos) + len(max_pos)
                 nzm = len(indzer)
 
                 if extNo > 2:
-
                     max_env, min_env, eMax, eMin = self.extract_max_min_spline(T, imf)
                     mean[:] = 0.5 * (max_env + min_env)
 
                     imf_old = imf.copy()
                     imf[:] = imf - mean
 
                     # Fix number of iterations
@@ -982,15 +986,15 @@
     DTYPE = np.float64
 
     # Signal options
     N = 400
     tMin, tMax = 0, 2 * np.pi
     T = np.linspace(tMin, tMax, N, dtype=DTYPE)
 
-    S = np.sin(20 * T * (1 + 0.2 * T)) + T ** 2 + np.sin(13 * T)
+    S = np.sin(20 * T * (1 + 0.2 * T)) + T**2 + np.sin(13 * T)
     S = S.astype(DTYPE)
     print("Input S.dtype: " + str(S.dtype))
 
     # Prepare and run EMD
     emd = EMD()
     emd.FIXE_H = 5
     emd.nbsym = 2
```

### Comparing `EMD-signal-1.4.0/PyEMD/EMD2d.py` & `EMD-signal-1.5.0/PyEMD/EMD2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,15 +321,14 @@
                 n += 1
                 self.logger.debug("Iteration: " + str(n))
 
                 min_peaks, max_peaks = self.find_extrema(imf)
 
                 self.logger.debug("min_peaks = %i  |  max_peaks = %i", len(min_peaks[0]), len(max_peaks[0]))
                 if len(min_peaks[0]) > 4 and len(max_peaks[0]) > 4:
-
                     imf_old = imf.copy()
                     imf = imf - mean_env
 
                     min_env, max_env = self.extract_max_min_spline(imf)
 
                     mean_env = 0.5 * (min_env + max_env)
 
@@ -340,29 +339,27 @@
                     if self.FIXE:
                         if n >= self.FIXE + 1:
                             stop_sifting = True
 
                     # Fix number of iterations after number of zero-crossings
                     # and extrema differ at most by one.
                     elif self.FIXE_H:
-
                         if n == 1:
                             continue
                         if self.check_proto_imf(imf, imf_old, mean_env):
                             n_h += 1
                         else:
                             n_h = 0
 
                         # STOP if enough n_h
                         if n_h >= self.FIXE_H:
                             stop_sifting = True
 
                     # Stops after default stopping criteria are met
                     else:
-
                         if self.check_proto_imf(imf, imf_old, mean_env):
                             stop_sifting = True
 
                 else:
                     notFinished = False
                     stop_sifting = True
```

### Comparing `EMD-signal-1.4.0/PyEMD/EMD_matlab.py` & `EMD-signal-1.5.0/PyEMD/EMD_matlab.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         Decomposition and its algorithms", IEEE-EURASIP Workshop on
         Nonlinear Signal and Image Processing NSIP-03, Grado (I), June 2003
     """
 
     logger = logging.getLogger(__name__)
 
     def __init__(self):
-
         self.splineKind = "cubic"
 
         self.nbsym = 2
         self.reduceScale = 1.0
         self.maxIteration = 500
         self.scaleFactor = 100
 
@@ -342,15 +341,14 @@
         d = np.diff(s)
         d1, d2 = d[:-1], d[1:]
         indmin = np.nonzero(np.r_[d1 * d2 < 0] & np.r_[d1 < 0])[0] + 1
         indmax = np.nonzero(np.r_[d1 * d2 < 0] & np.r_[d1 > 0])[0] + 1
 
         # When two or more points have the same value
         if np.any(d == 0):
-
             imax, imin = [], []
 
             bad = d == 0
             dd = np.diff(np.append(np.append(0, bad), 0))
             debs = np.nonzero(dd == 1)[0]
             fins = np.nonzero(dd == -1)[0]
             if debs[0] == 1:
@@ -427,15 +425,14 @@
         if (not (f1 or f2)) and f3:
             return True
         else:
             return False
 
     @staticmethod
     def _common_dtype(x, y):
-
         dtype = np.find_common_type([x.dtype, y.dtype], [])
         if x.dtype != dtype:
             x = x.astype(dtype)
         if y.dtype != dtype:
             y = y.astype(dtype)
 
         return x, y
@@ -528,15 +525,14 @@
                 MP, mP = ext_res[0], ext_res[2]
                 indzer = ext_res[4]
 
                 extNo = len(mP) + len(MP)
                 nzm = len(indzer)
 
                 if extNo > 2:
-
                     # Plotting. Either into file, or on-screen display.
                     imfOld = imf.copy()
                     imf = imf - self.reduceScale * mean
 
                     env_ext = self.extractMaxMinSpline(T, imf)
                     maxEnv, minEnv = env_ext[0], env_ext[1]
 
@@ -564,15 +560,14 @@
                     if self.FIXE:
                         if n >= self.FIXE + 1:
                             break
 
                     # Fix number of iterations after number of zero-crossings
                     # and extrema differ at most by one.
                     elif self.FIXE_H:
-
                         ext_res = self.findExtrema(T, imf)
                         mP, MP, indzer = ext_res[0], ext_res[2], ext_res[4]
                         extNo = len(mP) + len(MP)
                         nzm = len(indzer)
 
                         if n == 1:
                             continue
@@ -583,15 +578,14 @@
 
                         # STOP
                         if n_h >= self.FIXE_H:
                             break
 
                     # Stops after default stopping criteria are meet.
                     else:
-
                         mP, _, MP, _, indzer = self.findExtrema(T, imf)
                         extNo = len(mP) + len(MP)
                         nzm = len(indzer)
 
                         f1 = self.stop_sifting(imf, maxEnv, minEnv, mean, extNo)
                         f2 = abs(extNo - nzm) < 2
 
@@ -627,30 +621,29 @@
         return IMF, EXT, ITER, imfNo
 
 
 ###################################################
 # Beginning of program
 
 if __name__ == "__main__":
-
     import pylab as plt
 
     # Logging options
     logging.basicConfig(level=logging.DEBUG)
 
     # EMD options
     maxImf = -1
     DTYPE = np.float64
 
     # Signal options
     N = 1000
     tMin, tMax = 0, 1
     T = np.linspace(tMin, tMax, N, dtype=DTYPE)
 
-    S = 6 * T + np.cos(8 * np.pi ** T) + 0.5 * np.cos(40 * np.pi * T)
+    S = 6 * T + np.cos(8 * np.pi**T) + 0.5 * np.cos(40 * np.pi * T)
     S = S.astype(DTYPE)
 
     # Prepare and run EMD
     emd = EMD()
     emd.FIXE_H = 5
     # ~ emd.FIXE = 10
     emd.nbsym = 2
```

### Comparing `EMD-signal-1.4.0/PyEMD/checks.py` & `EMD-signal-1.5.0/PyEMD/checks.py`

 * *Files 8% similar despite different names*

```diff
@@ -113,20 +113,23 @@
     elif test_name == "aposteriori":
         scaling_imf_mean_period = math.log(mean_period(IMFs[rescaling_imf - 1]))
         scaling_imf_energy_density = math.log(energy(IMFs[rescaling_imf - 1]) / N)
 
         k = abs(stats.norm.ppf((1 - alpha) / 2))
         up_limit = -scaling_imf_mean_period + (k * math.sqrt(2 / N) * math.exp(scaling_imf_mean_period) / 2)
 
-        scaling_factor = up_limit - scaling_imf_energy_density
+        scaling_factor = math.exp(up_limit)
 
         for idx, imf in enumerate(IMFs):
             log_T = math.log(mean_period(imf))
-            energy_density = math.log(energy(imf) / N)
-            scaled_energy_density = energy_density + scaling_factor
+            if idx != rescaling_imf - 1:
+                scaled_energy_density = math.log((energy(imf) / N) / scaling_factor)
+            else:
+                scaled_energy_density = math.log(scaling_factor)
+
             sig_aposteriori = significance_aposteriori(scaled_energy_density, log_T, N, alpha)
 
             output[idx + 1] = int(sig_aposteriori)
 
     else:
         raise AssertionError("Only 'apriori' and 'aposteriori' are allowed")
```

### Comparing `EMD-signal-1.4.0/PyEMD/compact.py` & `EMD-signal-1.5.0/PyEMD/compact.py`

 * *Files identical despite different names*

### Comparing `EMD-signal-1.4.0/PyEMD/experimental/jitemd.py` & `EMD-signal-1.5.0/PyEMD/experimental/jitemd.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
     # a = Sn + Sp - 2*S0
     # b = 2*(Tn+Tp)*S0 - ((Tn+T0)*Sp+(T0+Tp)*Sn)
     # c = Sp*T0*Tn -2*Tp*S0*Tn + Tp*T0*Sn
     TnTp, T0Tn, TpT0 = Tn - Tp, T0 - Tn, Tp - T0
     scale = Tp * Tn * Tn + Tp * Tp * T0 + T0 * T0 * Tn - Tp * Tp * Tn - Tp * T0 * T0 - T0 * Tn * Tn
 
     a = T0Tn * Sp + TnTp * S0 + TpT0 * Sn
-    b = (S0 - Sn) * Tp ** 2 + (Sn - Sp) * T0 ** 2 + (Sp - S0) * Tn ** 2
+    b = (S0 - Sn) * Tp**2 + (Sn - Sp) * T0**2 + (Sp - S0) * Tn**2
     c = T0 * Tn * T0Tn * Sp + Tn * Tp * TnTp * S0 + Tp * T0 * TpT0 * Sn
 
     a = a / scale
     b = b / scale
     c = c / scale
     a[a == 0] = 1e-14
     tVertex = -0.5 * b / a
@@ -730,15 +730,15 @@
     """
     # local max are >0 and local min are <0
     # if np.any(eMax[1] < 0) or np.any(eMin[1] > 0):
     if np.sum(eMax[1] < 0) + np.sum(eMin[1] > 0) > 0:
         return False
 
     # Convergence
-    if np.sum(imf_new ** 2) < 1e-10:
+    if np.sum(imf_new**2) < 1e-10:
         return False
 
     # Precompute values
     imf_diff = imf_new - imf_old
     imf_diff_sqrd_sum = np.sum(imf_diff * imf_diff)
 
     # Scaled variance test
@@ -851,15 +851,14 @@
 
             ext_res = find_extrema(T, imf, extrema_detection)
             max_pos, min_pos, indzer = ext_res[0], ext_res[2], ext_res[4]
             extNo = len(min_pos) + len(max_pos)
             nzm = len(indzer)
 
             if extNo > 2:
-
                 max_extrema, min_extrema = extract_max_min_extrema(T, imf, nbsym, extrema_detection)
                 _, max_env = spline_points(T, max_extrema, spline_kind)
                 _, min_env = spline_points(T, min_extrema, spline_kind)
                 mean = 0.5 * (max_env + min_env)
 
                 imf_old = imf.copy()
                 imf = imf - mean
@@ -993,15 +992,15 @@
     DTYPE = np.float64
 
     # Signal options
     N = 400
     tMin, tMax = 0, 2 * np.pi
     T = np.linspace(tMin, tMax, N, dtype=DTYPE)
 
-    S = np.sin(20 * T * (1 + 0.2 * T)) + T ** 2 + np.sin(13 * T)
+    S = np.sin(20 * T * (1 + 0.2 * T)) + T**2 + np.sin(13 * T)
     S = S.astype(DTYPE)
     print("Input S.dtype: " + str(S.dtype))
 
     # Prepare and run EMD
     config = EmdConfig()
     imfs = emd(config, S, T, max_imf)
     imfNo = imfs.shape[0]
```

### Comparing `EMD-signal-1.4.0/PyEMD/tests/test_bemd.py` & `EMD-signal-1.5.0/PyEMD/tests/test_bemd.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,14 @@
         image = self._sin(x_f=[3, 5], y_f=[2])
         IMFs = self.bemd(image)
 
         # One of the reasons this algorithm isn't the preferred one
         self.assertTrue(IMFs.shape[0] == 7, "Depending on spline, there should be an IMF and possibly trend")
 
     def test_bemd_limitImfNo(self):
-
         # Create image
         rows, cols = 64, 64
         linear_background = 0.2 * self._generate_linear_image(rows, cols)
 
         # Sinusoidal IMF
         X = np.arange(cols)[None, :].T
         Y = np.arange(rows)
```

### Comparing `EMD-signal-1.4.0/PyEMD/tests/test_ceemdan.py` & `EMD-signal-1.5.0/PyEMD/tests/test_ceemdan.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,15 +108,14 @@
     def test_ceemdan_noiseKind_unknown(self):
         ceemdan = CEEMDAN()
         ceemdan.noise_kind = "bernoulli"
         with self.assertRaises(ValueError):
             ceemdan.generate_noise(1.0, 100)
 
     def test_ceemdan_passingCustomEMD(self):
-
         spline_kind = "linear"
         params = {"spline_kind": spline_kind}
 
         ceemdan = CEEMDAN()
         self.assertFalse(
             ceemdan.EMD.spline_kind == spline_kind,
             "Not" + self.cmp_msg(ceemdan.EMD.spline_kind, spline_kind),
@@ -130,15 +129,15 @@
         self.assertTrue(
             ceemdan.EMD.spline_kind == spline_kind,
             self.cmp_msg(ceemdan.EMD.spline_kind, spline_kind),
         )
 
     def test_ceemdan_noiseSeed(self):
         T = np.linspace(0, 1, 100)
-        S = np.sin(2 * np.pi * T + 4 ** T) + np.cos((T - 0.4) ** 2)
+        S = np.sin(2 * np.pi * T + 4**T) + np.cos((T - 0.4) ** 2)
 
         # Compare up to machine epsilon
         def cmpMachEps(x, y):
             return np.abs(x - y) <= 2 * np.finfo(x.dtype).eps
 
         ceemdan = CEEMDAN(trials=10)
 
@@ -160,15 +159,15 @@
 
         # Using same seeds, thus expecting same results
         msg_true = "Used same seed, expected same results"
         self.assertTrue(np.all(cmpMachEps(cIMF2, cIMF3)), msg_true)
 
     def test_ceemdan_originalSignal(self):
         T = np.linspace(0, 1, 100)
-        S = 2 * np.cos(3 * np.pi * T) + np.cos(2 * np.pi * T + 4 ** T)
+        S = 2 * np.cos(3 * np.pi * T) + np.cos(2 * np.pi * T + 4**T)
 
         # Make a copy of S for comparsion
         Scopy = np.copy(S)
 
         # Compare up to machine epsilon
         def cmpMachEps(x, y):
             return np.abs(x - y) <= 2 * np.finfo(x.dtype).eps
```

### Comparing `EMD-signal-1.4.0/PyEMD/tests/test_checks.py` & `EMD-signal-1.5.0/PyEMD/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `EMD-signal-1.4.0/PyEMD/tests/test_compact.py` & `EMD-signal-1.5.0/PyEMD/tests/test_compact.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
         # Do NOT modify this function! If you do, the following can happen:
         # -- Possible test errors for filter (tolerace of np.allclose).
         # -- Error in the derivative test (analytical derivative is hardcoded)
         t = np.linspace(0.0, np.pi, 200)
         return 0.1 * np.cos(2.0 * np.pi * t)
 
     def test_TDMA(self):
-
         diags = np.array([0.5 * np.ones(10), 1.0 * np.ones(10), 0.5 * np.ones(10)])
         positions = [-1, 0, 1]
         tridiag = sp.sparse.spdiags(diags, positions, 10, 10).todense()
 
         # change some diagonal values to make sure it is working
         diags[0][3] = 2.0
         diags[1][1] = 2.0
```

### Comparing `EMD-signal-1.4.0/PyEMD/tests/test_eemd.py` & `EMD-signal-1.5.0/PyEMD/tests/test_eemd.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,14 @@
         noise_kind = "whoever_supports_this_is_wrong"
         eemd = EEMD(noise_kind=noise_kind)
 
         with self.assertRaises(ValueError):
             eemd.generate_noise(1.0, 100)
 
     def test_eemd_passingCustomEMD(self):
-
         spline_kind = "linear"
         params = {"spline_kind": spline_kind}
 
         eemd = EEMD()
         self.assertFalse(eemd.EMD.spline_kind == spline_kind, "Not" + self.cmp_msg(eemd.EMD.spline_kind, spline_kind))
 
         from PyEMD import EMD
@@ -98,15 +97,15 @@
         emd = EMD(**params)
 
         eemd = EEMD(ext_EMD=emd)
         self.assertTrue(eemd.EMD.spline_kind == spline_kind, self.cmp_msg(eemd.EMD.spline_kind, spline_kind))
 
     def test_eemd_noiseSeed(self):
         T = np.linspace(0, 1, 100)
-        S = np.sin(2 * np.pi * T + 4 ** T) + np.cos((T - 0.4) ** 2)
+        S = np.sin(2 * np.pi * T + 4**T) + np.cos((T - 0.4) ** 2)
 
         # Compare up to machine epsilon
         def cmpMachEps(x, y):
             return np.abs(x - y) <= 2 * np.finfo(x.dtype).eps
 
         config = {"processes": 1}
         eemd = EEMD(trials=10, **config)
```

### Comparing `EMD-signal-1.4.0/PyEMD/tests/test_emd.py` & `EMD-signal-1.5.0/PyEMD/tests/test_emd.py`

 * *Files identical despite different names*

### Comparing `EMD-signal-1.4.0/PyEMD/tests/test_emd2d.py` & `EMD-signal-1.5.0/PyEMD/tests/test_emd2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,23 +281,21 @@
             np.allclose(IMFs[0], comp_2d, atol=1.0), "Output: \n" + str(IMFs[0]) + "\nInput: \n" + str(comp_2d)
         )
 
         # Second IMF should be linear trend
         self.assertTrue(np.allclose(IMFs[1], linear_background, atol=1.0))
 
     def test_emd2d_passArgsViaDict(self):
-
         FIXE = 10
         params = {"FIXE": FIXE}
         emd2D = EMD2D(**params)
 
         self.assertTrue(emd2D.FIXE == FIXE, "Received {}, Expceted {}".format(emd2D.FIXE, FIXE))
 
     def test_emd2d_limitImfNo(self):
-
         # Create image
         rows, cols = 128, 128
         linear_background = 0.2 * self._generate_linear_image(rows, cols)
 
         # Sinusoidal IMF
         X = np.arange(cols)[None, :].T
         Y = np.arange(rows)
```

### Comparing `EMD-signal-1.4.0/PyEMD/tests/test_extrema.py` & `EMD-signal-1.5.0/PyEMD/tests/test_extrema.py`

 * *Files identical despite different names*

### Comparing `EMD-signal-1.4.0/PyEMD/tests/test_splines.py` & `EMD-signal-1.5.0/PyEMD/tests/test_splines.py`

 * *Files identical despite different names*

### Comparing `EMD-signal-1.4.0/PyEMD/tests/test_utils.py` & `EMD-signal-1.5.0/PyEMD/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `EMD-signal-1.4.0/PyEMD/tests/test_visualization.py` & `EMD-signal-1.5.0/PyEMD/tests/test_visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def test_instantiation(self):
         emd = EMD()
         with self.assertRaises(ValueError):
             Visualisation(emd)
 
     def test_instantiation2(self):
         t = np.linspace(0, 1, 50)
-        S = t + np.cos(np.cos(4.0 * t ** 2))
+        S = t + np.cos(np.cos(4.0 * t**2))
         emd = EMD()
         emd.emd(S, t)
         imfs, res = emd.get_imfs_and_residue()
         vis = Visualisation(emd)
         self.assertTrue(np.alltrue(vis.imfs == imfs))
         self.assertTrue(np.alltrue(vis.residue == res))
 
@@ -47,15 +47,15 @@
         vis = Visualisation()
         imfs = np.arange(50).reshape(2, 25)
         with self.assertRaises(AttributeError):
             vis._check_imfs(imfs, None, True)
 
     def test_check_imfs5(self):
         t = np.linspace(0, 1, 50)
-        S = t + np.cos(np.cos(4.0 * t ** 2))
+        S = t + np.cos(np.cos(4.0 * t**2))
         emd = EMD()
         emd.emd(S, t)
         imfs, res = emd.get_imfs_and_residue()
         vis = Visualisation(emd)
         imfs2, res2 = vis._check_imfs(imfs, res, False)
         self.assertTrue(np.alltrue(imfs == imfs2))
         self.assertTrue(np.alltrue(res == res2))
@@ -78,42 +78,42 @@
         sig = np.arange(10)
         vis = Visualisation()
         phase = vis._calc_inst_phase(sig, None)
         assert len(sig) == len(phase)
 
     def test_calc_instant_phase2(self):
         t = np.linspace(0, 1, 50)
-        S = t + np.cos(np.cos(4.0 * t ** 2))
+        S = t + np.cos(np.cos(4.0 * t**2))
         emd = EMD()
         imfs = emd.emd(S, t)
         vis = Visualisation()
         phase = vis._calc_inst_phase(imfs, 0.4)
         assert len(imfs) == len(phase)
 
     def test_calc_instant_phase3(self):
         t = np.linspace(0, 1, 50)
-        S = t + np.cos(np.cos(4.0 * t ** 2))
+        S = t + np.cos(np.cos(4.0 * t**2))
         emd = EMD()
         imfs = emd.emd(S, t)
         vis = Visualisation()
         with self.assertRaises(AssertionError):
             _ = vis._calc_inst_phase(imfs, 0.8)
 
     def test_calc_instant_freq_alphaNone(self):
         t = np.linspace(0, 1, 50)
-        S = t + np.cos(np.cos(4.0 * t ** 2))
+        S = t + np.cos(np.cos(4.0 * t**2))
         emd = EMD()
         imfs = emd.emd(S, t)
         vis = Visualisation()
         freqs = vis._calc_inst_freq(imfs, t, False, None)
         self.assertEqual(imfs.shape, freqs.shape)
 
     def test_calc_instant_freq(self):
         t = np.linspace(0, 1, 50)
-        S = t + np.cos(np.cos(4.0 * t ** 2))
+        S = t + np.cos(np.cos(4.0 * t**2))
         emd = EMD()
         imfs = emd.emd(S, t)
         vis = Visualisation()
         freqs = vis._calc_inst_freq(imfs, t, False, 0.4)
         self.assertEqual(imfs.shape, freqs.shape)
 
     def test_plot_instant_freq(self):
```

### Comparing `EMD-signal-1.4.0/PyEMD/utils.py` & `EMD-signal-1.5.0/PyEMD/utils.py`

 * *Files identical despite different names*

### Comparing `EMD-signal-1.4.0/PyEMD/visualisation.py` & `EMD-signal-1.5.0/PyEMD/visualisation.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 
 
 if __name__ == "__main__":
     from PyEMD import EMD
 
     # Simple signal example
     t = np.arange(0, 3, 0.01)
-    S = np.sin(13 * t + 0.2 * t ** 1.4) - np.cos(3 * t)
+    S = np.sin(13 * t + 0.2 * t**1.4) - np.cos(3 * t)
 
     emd = EMD()
     emd.emd(S)
     imfs, res = emd.get_imfs_and_residue()
 
     # Initiate visualisation with emd instance
     vis = Visualisation(emd)
```

### Comparing `EMD-signal-1.4.0/README.md` & `EMD-signal-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 - Online documentation: <https://pyemd.readthedocs.org>
 - Issue tracker: <https://github.com/laszukdawid/pyemd/issues>
 - Source code repository: <https://github.com/laszukdawid/pyemd>
 
 ## Introduction
 
-This is yet another Python implementation of Empirical Mode
+Python implementation of the Empirical Mode
 Decomposition (EMD). The package contains multiple EMD variations and
 intends to deliver more in time.
 
 ### EMD variations
 
 -  Ensemble EMD (EEMD),
 -  "Complete Ensemble EMD" (CEEMDAN)
@@ -29,15 +29,17 @@
 *PyEMD* allows you to use different splines for envelopes, stopping criteria
 and extrema interpolations.
 
 ### Available splines
 
 -  Natural cubic (**default**)
 -  Pointwise cubic
+-  Hermite cubic
 -  Akima
+-  PChip
 -  Linear
 
 ### Available stopping criteria
 
 -  Cauchy convergence (**default**)
 -  Fixed number of iterations
 -  Number of consecutive proto-imfs
```

### Comparing `EMD-signal-1.4.0/example/eemd_example.py` & `EMD-signal-1.5.0/example/eemd_example.py`

 * *Files identical despite different names*

### Comparing `EMD-signal-1.4.0/example/emd_comparison.py` & `EMD-signal-1.5.0/example/emd_comparison.py`

 * *Files identical despite different names*

### Comparing `EMD-signal-1.4.0/example/hht_example.py` & `EMD-signal-1.5.0/example/hht_example.py`

 * *Files identical despite different names*

### Comparing `EMD-signal-1.4.0/example/image_example.py` & `EMD-signal-1.5.0/example/image_example.py`

 * *Files identical despite different names*

### Comparing `EMD-signal-1.4.0/example/simple_example.py` & `EMD-signal-1.5.0/example/simple_example.py`

 * *Files identical despite different names*

### Comparing `EMD-signal-1.4.0/setup.cfg` & `EMD-signal-1.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 	sphinx
 	sphinx_rtd_theme
 	numpydoc
 jit = 
 	numba==0.56.*
 dev = 
 	pycodestyle==2.8.*
-	black==21.10b0
+	black==23.3.*
 	isort==5.10.*
 	click==8.0.4
 test = 
 	pytest
 	codecov
 
 [pycodestyle]
```

