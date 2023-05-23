# Comparing `tmp/qsonic-0.6.1.tar.gz` & `tmp/qsonic-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsonic-0.6.1.tar", last modified: Wed May 17 21:41:20 2023, max compression
+gzip compressed data, was "qsonic-0.6.2.tar", last modified: Tue May 23 15:21:02 2023, max compression
```

## Comparing `qsonic-0.6.1.tar` & `qsonic-0.6.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:41:20.536775 qsonic-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-17 21:41:07.000000 qsonic-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-17 21:41:20.536775 qsonic-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-17 21:41:07.000000 qsonic-0.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:41:20.532775 qsonic-0.6.1/py/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:41:20.536775 qsonic-0.6.1/py/qsonic/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/mathtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/mpi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    49929 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/picca_continuum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:41:20.536775 qsonic-0.6.1/py/qsonic/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/scripts/qsonic_calib.py
--rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/scripts/qsonic_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    25509 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:41:20.536775 qsonic-0.6.1/py/qsonic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-17 21:41:20.000000 qsonic-0.6.1/py/qsonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-17 21:41:20.000000 qsonic-0.6.1/py/qsonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:41:20.000000 qsonic-0.6.1/py/qsonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-17 21:41:20.000000 qsonic-0.6.1/py/qsonic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-17 21:41:20.000000 qsonic-0.6.1/py/qsonic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 21:41:20.000000 qsonic-0.6.1/py/qsonic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 21:41:07.000000 qsonic-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-17 21:41:07.000000 qsonic-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-17 21:41:20.536775 qsonic-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 21:41:07.000000 qsonic-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:41:20.536775 qsonic-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-17 21:41:07.000000 qsonic-0.6.1/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-05-17 21:41:07.000000 qsonic-0.6.1/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-17 21:41:07.000000 qsonic-0.6.1/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-17 21:41:07.000000 qsonic-0.6.1/tests/test_mathtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-17 21:41:07.000000 qsonic-0.6.1/tests/test_mpi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-05-17 21:41:07.000000 qsonic-0.6.1/tests/test_picca_continuum.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-17 21:41:07.000000 qsonic-0.6.1/tests/test_qsonic_calib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-17 21:41:07.000000 qsonic-0.6.1/tests/test_spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:21:02.929183 qsonic-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-23 15:20:44.000000 qsonic-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-23 15:21:02.929183 qsonic-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-23 15:20:44.000000 qsonic-0.6.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:21:02.925182 qsonic-0.6.2/py/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:21:02.929183 qsonic-0.6.2/py/qsonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/mathtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/mpi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49929 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/picca_continuum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:21:02.929183 qsonic-0.6.2/py/qsonic/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/scripts/qsonic_calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/scripts/qsonic_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25509 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:21:02.929183 qsonic-0.6.2/py/qsonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-23 15:21:02.000000 qsonic-0.6.2/py/qsonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-23 15:21:02.000000 qsonic-0.6.2/py/qsonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:21:02.000000 qsonic-0.6.2/py/qsonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-23 15:21:02.000000 qsonic-0.6.2/py/qsonic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-23 15:21:02.000000 qsonic-0.6.2/py/qsonic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 15:21:02.000000 qsonic-0.6.2/py/qsonic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-23 15:20:44.000000 qsonic-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-23 15:20:44.000000 qsonic-0.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-23 15:21:02.929183 qsonic-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 15:20:44.000000 qsonic-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:21:02.929183 qsonic-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-23 15:20:44.000000 qsonic-0.6.2/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-05-23 15:20:44.000000 qsonic-0.6.2/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-23 15:20:44.000000 qsonic-0.6.2/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-23 15:20:44.000000 qsonic-0.6.2/tests/test_mathtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-23 15:20:44.000000 qsonic-0.6.2/tests/test_mpi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-05-23 15:20:44.000000 qsonic-0.6.2/tests/test_picca_continuum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-23 15:20:44.000000 qsonic-0.6.2/tests/test_qsonic_calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-23 15:20:44.000000 qsonic-0.6.2/tests/test_spectrum.py
```

### Comparing `qsonic-0.6.1/LICENSE` & `qsonic-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.1/PKG-INFO` & `qsonic-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: qsonic
-Version: 0.6.1
+Version: 0.6.2
 Summary: Quasar continuum fitter for DESI
 Author: Naim Goksel Karacayli
 Author-email: ngokselk@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/p-slash/qsonic/issues
 Project-URL: Documentation, http://qsonic.readthedocs.io/
 Project-URL: Source, https://github.com/p-slash/qsonic
-Requires-Python: >=3.7
+Requires-Python: <3.11,>=3.7
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: pub
 License-File: LICENSE
 
 ======
 QSOnic
```

### Comparing `qsonic-0.6.1/README.rst` & `qsonic-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.1/py/qsonic/calibration.py` & `qsonic-0.6.2/py/qsonic/calibration.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.1/py/qsonic/catalog.py` & `qsonic-0.6.2/py/qsonic/catalog.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.1/py/qsonic/io.py` & `qsonic-0.6.2/py/qsonic/io.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.1/py/qsonic/masks.py` & `qsonic-0.6.2/py/qsonic/masks.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.1/py/qsonic/mathtools.py` & `qsonic-0.6.2/py/qsonic/mathtools.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.1/py/qsonic/mpi_utils.py` & `qsonic-0.6.2/py/qsonic/mpi_utils.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.1/py/qsonic/picca_continuum.py` & `qsonic-0.6.2/py/qsonic/picca_continuum.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.1/py/qsonic/scripts/qsonic_calib.py` & `qsonic-0.6.2/py/qsonic/scripts/qsonic_calib.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.1/py/qsonic/scripts/qsonic_fit.py` & `qsonic-0.6.2/py/qsonic/scripts/qsonic_fit.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.1/py/qsonic/spectrum.py` & `qsonic-0.6.2/py/qsonic/spectrum.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.1/py/qsonic.egg-info/PKG-INFO` & `qsonic-0.6.2/py/qsonic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: qsonic
-Version: 0.6.1
+Version: 0.6.2
 Summary: Quasar continuum fitter for DESI
 Author: Naim Goksel Karacayli
 Author-email: ngokselk@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/p-slash/qsonic/issues
 Project-URL: Documentation, http://qsonic.readthedocs.io/
 Project-URL: Source, https://github.com/p-slash/qsonic
-Requires-Python: >=3.7
+Requires-Python: <3.11,>=3.7
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: pub
 License-File: LICENSE
 
 ======
 QSOnic
```

### Comparing `qsonic-0.6.1/py/qsonic.egg-info/SOURCES.txt` & `qsonic-0.6.2/py/qsonic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.1/setup.cfg` & `qsonic-0.6.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.6.1
+current_version = 0.6.2
 commit = True
 tag = True
 
 [bumpversion:file:py/qsonic/__init__.py]
 search = __version__ = '{current_version}'
 replace = __version__ = '{new_version}'
 
@@ -20,15 +20,15 @@
 	Documentation=http://qsonic.readthedocs.io/
 	Source=https://github.com/p-slash/qsonic
 
 [options]
 package_dir = 
 	=py
 packages = find_namespace:
-python_requires = >=3.7
+python_requires = >=3.7, <3.11
 install_requires = file: requirements.txt
 
 [options.packages.find]
 where = py
 
 [options.entry_points]
 console_scripts =
```

### Comparing `qsonic-0.6.1/tests/test_catalog.py` & `qsonic-0.6.2/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.1/tests/test_io.py` & `qsonic-0.6.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.1/tests/test_masks.py` & `qsonic-0.6.2/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.1/tests/test_mathtools.py` & `qsonic-0.6.2/tests/test_mathtools.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.1/tests/test_mpi_utils.py` & `qsonic-0.6.2/tests/test_mpi_utils.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.1/tests/test_picca_continuum.py` & `qsonic-0.6.2/tests/test_picca_continuum.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.1/tests/test_qsonic_calib.py` & `qsonic-0.6.2/tests/test_qsonic_calib.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.1/tests/test_spectrum.py` & `qsonic-0.6.2/tests/test_spectrum.py`

 * *Files identical despite different names*

