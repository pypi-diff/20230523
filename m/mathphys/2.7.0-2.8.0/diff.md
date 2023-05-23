# Comparing `tmp/mathphys-2.7.0.tar.gz` & `tmp/mathphys-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathphys-2.7.0.tar", last modified: Mon Feb  6 13:22:44 2023, max compression
+gzip compressed data, was "mathphys-2.8.0.tar", last modified: Tue May 23 18:59:23 2023, max compression
```

## Comparing `mathphys-2.7.0.tar` & `mathphys-2.8.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 13:22:44.781397 mathphys-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-02-06 13:22:29.000000 mathphys-2.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-02-06 13:22:29.000000 mathphys-2.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-02-06 13:22:44.781397 mathphys-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1107 2023-02-06 13:22:29.000000 mathphys-2.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 13:22:44.777397 mathphys-2.7.0/mathphys/
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-02-06 13:22:42.000000 mathphys-2.7.0/mathphys/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)      529 2023-02-06 13:22:29.000000 mathphys-2.7.0/mathphys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-02-06 13:22:29.000000 mathphys-2.7.0/mathphys/base_units.py
--rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-02-06 13:22:29.000000 mathphys-2.7.0/mathphys/beam_optics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1928 2023-02-06 13:22:29.000000 mathphys-2.7.0/mathphys/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     6242 2023-02-06 13:22:29.000000 mathphys-2.7.0/mathphys/functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1774 2023-02-06 13:22:29.000000 mathphys-2.7.0/mathphys/units.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 13:22:44.777397 mathphys-2.7.0/mathphys.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-02-06 13:22:44.000000 mathphys-2.7.0/mathphys.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      392 2023-02-06 13:22:44.000000 mathphys-2.7.0/mathphys.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-06 13:22:44.000000 mathphys-2.7.0/mathphys.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-06 13:22:44.000000 mathphys-2.7.0/mathphys.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-02-06 13:22:44.000000 mathphys-2.7.0/mathphys.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-02-06 13:22:44.000000 mathphys-2.7.0/mathphys.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-02-06 13:22:29.000000 mathphys-2.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-06 13:22:44.781397 mathphys-2.7.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1204 2023-02-06 13:22:29.000000 mathphys-2.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:59:23.985159 mathphys-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-05-23 18:59:10.000000 mathphys-2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-23 18:59:10.000000 mathphys-2.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-05-23 18:59:23.985159 mathphys-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1107 2023-05-23 18:59:10.000000 mathphys-2.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:59:23.985159 mathphys-2.8.0/mathphys/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-23 18:59:22.000000 mathphys-2.8.0/mathphys/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)      577 2023-05-23 18:59:10.000000 mathphys-2.8.0/mathphys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-05-23 18:59:10.000000 mathphys-2.8.0/mathphys/base_units.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2385 2023-05-23 18:59:10.000000 mathphys-2.8.0/mathphys/beam_optics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-05-23 18:59:10.000000 mathphys-2.8.0/mathphys/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6242 2023-05-23 18:59:10.000000 mathphys-2.8.0/mathphys/functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    55472 2023-05-23 18:59:10.000000 mathphys-2.8.0/mathphys/imgproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1774 2023-05-23 18:59:10.000000 mathphys-2.8.0/mathphys/units.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:59:23.985159 mathphys-2.8.0/mathphys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-05-23 18:59:23.000000 mathphys-2.8.0/mathphys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      412 2023-05-23 18:59:23.000000 mathphys-2.8.0/mathphys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 18:59:23.000000 mathphys-2.8.0/mathphys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 18:59:23.000000 mathphys-2.8.0/mathphys.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-23 18:59:23.000000 mathphys-2.8.0/mathphys.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-23 18:59:23.000000 mathphys-2.8.0/mathphys.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-23 18:59:10.000000 mathphys-2.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 18:59:23.985159 mathphys-2.8.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1204 2023-05-23 18:59:10.000000 mathphys-2.8.0/setup.py
```

### Comparing `mathphys-2.7.0/LICENSE` & `mathphys-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mathphys-2.7.0/PKG-INFO` & `mathphys-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathphys
-Version: 2.7.0
+Version: 2.8.0
 Summary: LNLS Math and Physics Utilities
 Home-page: https://github.com/lnls-fac/mathphys
 Download-URL: https://github.com/lnls-fac/mathphys
 Author: lnls-fac
 Author-email: xresende@gmail.com
 License: MIT License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mathphys-2.7.0/README.md` & `mathphys-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `mathphys-2.7.0/mathphys/beam_optics.py` & `mathphys-2.8.0/mathphys/beam_optics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Beam Optics functions."""
 
 import math as _math
 import numpy as _np
+
 from mathphys import constants as _c
 from mathphys import units as _u
 
 
 # NOTE: This function is used in siriuspy!
 def beam_rigidity(**kwargs):
     """Beam rigidity."""
```

### Comparing `mathphys-2.7.0/mathphys/constants.py` & `mathphys-2.8.0/mathphys/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Constants module.
 
 https://en.wikipedia.org/wiki/International_System_of_Units
 """
 
 import math as _math
+
 from . import base_units as _u
 
 
 # temporary auxiliary derived units
 _volt = (_u.kilogram * _u.meter**2) / (_u.ampere * _u.second**2)
 _coulomb = _u.second * _u.ampere
 _joule = _u.kilogram * _u.meter**2 / _u.second**2
```

### Comparing `mathphys-2.7.0/mathphys/functions.py` & `mathphys-2.8.0/mathphys/functions.py`

 * *Files identical despite different names*

### Comparing `mathphys-2.7.0/mathphys/units.py` & `mathphys-2.8.0/mathphys/units.py`

 * *Files identical despite different names*

### Comparing `mathphys-2.7.0/mathphys.egg-info/PKG-INFO` & `mathphys-2.8.0/mathphys.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathphys
-Version: 2.7.0
+Version: 2.8.0
 Summary: LNLS Math and Physics Utilities
 Home-page: https://github.com/lnls-fac/mathphys
 Download-URL: https://github.com/lnls-fac/mathphys
 Author: lnls-fac
 Author-email: xresende@gmail.com
 License: MIT License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mathphys-2.7.0/setup.py` & `mathphys-2.8.0/setup.py`

 * *Files identical despite different names*

