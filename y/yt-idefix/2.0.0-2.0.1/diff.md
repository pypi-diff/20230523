# Comparing `tmp/yt_idefix-2.0.0.tar.gz` & `tmp/yt_idefix-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_idefix-2.0.0.tar", last modified: Mon May  1 13:30:43 2023, max compression
+gzip compressed data, was "yt_idefix-2.0.1.tar", last modified: Tue May 23 10:05:25 2023, max compression
```

## Comparing `yt_idefix-2.0.0.tar` & `yt_idefix-2.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:30:43.108076 yt_idefix-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-01 13:30:27.000000 yt_idefix-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-01 13:30:43.108076 yt_idefix-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-05-01 13:30:27.000000 yt_idefix-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-01 13:30:27.000000 yt_idefix-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 13:30:43.108076 yt_idefix-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:30:43.108076 yt_idefix-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/tests/test_C_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/tests/test_dmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/tests/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/tests/test_vtk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/tests/test_xdmf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:30:43.108076 yt_idefix-2.0.0/yt_idefix/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/_backports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:30:43.108076 yt_idefix-2.0.0/yt_idefix/_io/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/_io/C_io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/_io/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/_io/dmp_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/_io/h5_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/_io/vtk_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    34811 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:30:43.108076 yt_idefix-2.0.0/yt_idefix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-01 13:30:43.000000 yt_idefix-2.0.0/yt_idefix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-01 13:30:43.000000 yt_idefix-2.0.0/yt_idefix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 13:30:43.000000 yt_idefix-2.0.0/yt_idefix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-01 13:30:43.000000 yt_idefix-2.0.0/yt_idefix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-01 13:30:43.000000 yt_idefix-2.0.0/yt_idefix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 13:30:43.000000 yt_idefix-2.0.0/yt_idefix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:05:25.445487 yt_idefix-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-23 10:05:15.000000 yt_idefix-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-23 10:05:25.445487 yt_idefix-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-05-23 10:05:15.000000 yt_idefix-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-23 10:05:15.000000 yt_idefix-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 10:05:25.445487 yt_idefix-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:05:25.445487 yt_idefix-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/tests/test_C_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/tests/test_dmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/tests/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/tests/test_vtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/tests/test_xdmf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:05:25.445487 yt_idefix-2.0.1/yt_idefix/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/_backports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:05:25.445487 yt_idefix-2.0.1/yt_idefix/_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/_io/C_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/_io/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/_io/dmp_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/_io/h5_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/_io/vtk_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35099 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:05:25.445487 yt_idefix-2.0.1/yt_idefix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-23 10:05:25.000000 yt_idefix-2.0.1/yt_idefix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-23 10:05:25.000000 yt_idefix-2.0.1/yt_idefix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 10:05:25.000000 yt_idefix-2.0.1/yt_idefix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-23 10:05:25.000000 yt_idefix-2.0.1/yt_idefix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-23 10:05:25.000000 yt_idefix-2.0.1/yt_idefix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 10:05:25.000000 yt_idefix-2.0.1/yt_idefix.egg-info/top_level.txt
```

### Comparing `yt_idefix-2.0.0/LICENSE` & `yt_idefix-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.0/PKG-INFO` & `yt_idefix-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt_idefix
-Version: 2.0.0
+Version: 2.0.1
 Summary: An extension module for yt, adding a frontend for Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Documentation, https://yt-project.org/docs/dev/
 Project-URL: Source, https://github.com/neutrinoceros/yt_idefix
 Project-URL: Tracker, https://github.com/neutrinoceros/yt_idefix/issues
@@ -34,15 +34,15 @@
 [![PyPI](https://img.shields.io/badge/requires-Python%20≥%203.8-blue?logo=python&logoColor=white)](https://pypi.org/project/yt_idefix/)
 [![yt-project](https://img.shields.io/static/v1?label="works%20with"&message="yt"&color="blueviolet")](https://yt-project.org)
 
 <!--- Tests and style --->
 [![CI](https://github.com/neutrinoceros/yt_idefix/actions/workflows/ci.yml/badge.svg)](https://github.com/neutrinoceros/yt_idefix/actions/workflows/ci.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/yt_idefix/main.svg)](https://results.pre-commit.ci/latest/github/neutrinoceros/yt_idefix/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 A maturing yt frontend for Idefix and Pluto, packaged as an extension for yt.
 
 ## Installation
 
 ```shell
 python -m pip install yt_idefix
```

### Comparing `yt_idefix-2.0.0/README.md` & `yt_idefix-2.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![PyPI](https://img.shields.io/badge/requires-Python%20≥%203.8-blue?logo=python&logoColor=white)](https://pypi.org/project/yt_idefix/)
 [![yt-project](https://img.shields.io/static/v1?label="works%20with"&message="yt"&color="blueviolet")](https://yt-project.org)
 
 <!--- Tests and style --->
 [![CI](https://github.com/neutrinoceros/yt_idefix/actions/workflows/ci.yml/badge.svg)](https://github.com/neutrinoceros/yt_idefix/actions/workflows/ci.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/yt_idefix/main.svg)](https://results.pre-commit.ci/latest/github/neutrinoceros/yt_idefix/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 A maturing yt frontend for Idefix and Pluto, packaged as an extension for yt.
 
 ## Installation
 
 ```shell
 python -m pip install yt_idefix
```

### Comparing `yt_idefix-2.0.0/pyproject.toml` & `yt_idefix-2.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yt_idefix"
-version = "2.0.0"
+version = "2.0.1"
 description = "An extension module for yt, adding a frontend for Idefix"
 authors = [
     { name = "C.M.T. Robert" },
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
@@ -80,14 +80,15 @@
     "*/api.py",
     "*/__init__.py",
 ]
 select = [
     "E",
     "F",
     "W",
+    "C4",   # flake8-comprehensions
     "B",    # flake8-bugbear
     "G",    # flake8-logging-format
     "YTT",  # flake8-2020
     "UP",   # pyupgrade
     "I",    # isort
 ]
 ignore = [
```

### Comparing `yt_idefix-2.0.0/tests/test_C_io.py` & `yt_idefix-2.0.1/tests/test_C_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.0/tests/test_dmp.py` & `yt_idefix-2.0.1/tests/test_dmp.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.0/tests/test_loading.py` & `yt_idefix-2.0.1/tests/test_loading.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.0/tests/test_vtk.py` & `yt_idefix-2.0.1/tests/test_vtk.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.0/tests/test_xdmf.py` & `yt_idefix-2.0.1/tests/test_xdmf.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.0/yt_idefix/_backports.py` & `yt_idefix-2.0.1/yt_idefix/_backports.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.0/yt_idefix/_io/commons.py` & `yt_idefix-2.0.1/yt_idefix/_io/commons.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.0/yt_idefix/_io/dmp_io.py` & `yt_idefix-2.0.1/yt_idefix/_io/dmp_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.0/yt_idefix/_io/h5_io.py` & `yt_idefix-2.0.1/yt_idefix/_io/h5_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.0/yt_idefix/_io/vtk_io.py` & `yt_idefix-2.0.1/yt_idefix/_io/vtk_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.0/yt_idefix/data_structures.py` & `yt_idefix-2.0.1/yt_idefix/data_structures.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from abc import ABC, abstractmethod
 from functools import cached_property
 from pathlib import Path
 from typing import TYPE_CHECKING, Final, Literal
 
 import inifix
 import numpy as np
+import numpy.testing as npt
 
 from yt.data_objects.index_subobjects.stretched_grid import StretchedGrid
 from yt.data_objects.static_output import Dataset
 from yt.funcs import setdefaultattr
 from yt.geometry.grid_geometry_handler import GridIndex
 from yt.utilities.lib.misc_utilities import (  # type: ignore [import]
     _obtain_coords_and_widths,
@@ -181,46 +182,50 @@
             cell_edges = vtk_io.read_grid_coordinates(fh, geometry=self.ds.geometry)
 
         dims = self.ds.domain_dimensions
         length_unit = self.ds.quan(1, "code_length")
 
         cell_widths: tuple[XSpans, YSpans, ZSpans]
         cell_widths = (
-            np.empty(max(dims[0], 2), dtype="float64") * length_unit,
-            np.empty(max(dims[1], 2), dtype="float64") * length_unit,
-            np.empty(max(dims[2], 2), dtype="float64") * length_unit,
+            np.full(max(dims[0], 2), -1, dtype="float64") * length_unit,
+            np.full(max(dims[1], 2), -1, dtype="float64") * length_unit,
+            np.full(max(dims[2], 2), -1, dtype="float64") * length_unit,
         )
 
         for idir, edges in enumerate(cell_edges[:3]):
             if dims[idir] > 1:
                 cell_widths[idir][:] = np.ediff1d(edges)
             else:
                 cell_widths[idir][:] = self.ds.domain_width[idir]
+            npt.assert_array_less(0, cell_widths[idir])
+
         return cell_widths
 
     @cached_property
     def _cell_centers(self) -> tuple[XCoords, YCoords, ZCoords]:
         with open(self.index_filename, "rb") as fh:
             cell_edges = vtk_io.read_grid_coordinates(fh, geometry=self.ds.geometry)
 
         dims = self.ds.domain_dimensions
         length_unit = self.ds.quan(1, "code_length")
 
         cell_centers: tuple[XCoords, YCoords, ZCoords]
         cell_centers = (
-            np.empty(max(dims[0], 2), dtype="float64") * length_unit,
-            np.empty(max(dims[1], 2), dtype="float64") * length_unit,
-            np.empty(max(dims[2], 2), dtype="float64") * length_unit,
+            np.full(max(dims[0], 2), -1, dtype="float64") * length_unit,
+            np.full(max(dims[1], 2), -1, dtype="float64") * length_unit,
+            np.full(max(dims[2], 2), -1, dtype="float64") * length_unit,
         )
 
         for idir, edges in enumerate(cell_edges[:3]):
             if dims[idir] > 1:
                 cell_centers[idir][:] = 0.5 * (edges[1:] + edges[:-1])
             else:
                 cell_centers[idir][:] = edges[0]
+            npt.assert_array_less(0, cell_centers[idir])
+
         return cell_centers
 
 
 class IdefixDmpHierarchy(FieldOffsetHierarchy):
     def _get_field_offset_index(self) -> dict[str, int]:
         with open(self.index_filename, "rb") as fh:
             return dmp_io.get_field_offset_index(fh)
@@ -254,47 +259,51 @@
         )
 
         dims = self.ds.domain_dimensions
         length_unit = self.ds.quan(1, "code_length")
 
         cell_widths: tuple[XSpans, YSpans, ZSpans]
         cell_widths = (
-            np.empty(max(dims[0], 2), dtype="float64") * length_unit,
-            np.empty(max(dims[1], 2), dtype="float64") * length_unit,
-            np.empty(max(dims[2], 2), dtype="float64") * length_unit,
+            np.full(max(dims[0], 2), -1, dtype="float64") * length_unit,
+            np.full(max(dims[1], 2), -1, dtype="float64") * length_unit,
+            np.full(max(dims[2], 2), -1, dtype="float64") * length_unit,
         )
 
         for idir, edges in enumerate(cell_edges[:3]):
             if dims[idir] > 1:
                 cell_widths[idir][:] = np.ediff1d(edges)
             else:
                 cell_widths[idir][:] = self.ds.domain_width[idir]
+            npt.assert_array_less(0, cell_widths[idir])
+
         return cell_widths
 
     @cached_property
     def _cell_centers(self) -> tuple[XCoords, YCoords, ZCoords]:
         cell_edges = h5_io.read_grid_coordinates(
             self.index_filename, geometry=self.ds.geometry
         )
 
         dims = self.ds.domain_dimensions
         length_unit = self.ds.quan(1, "code_length")
 
         cell_centers: tuple[XCoords, YCoords, ZCoords]
         cell_centers = (
-            np.empty(max(dims[0], 2), dtype="float64") * length_unit,
-            np.empty(max(dims[1], 2), dtype="float64") * length_unit,
-            np.empty(max(dims[2], 2), dtype="float64") * length_unit,
+            np.full(max(dims[0], 2), -1, dtype="float64") * length_unit,
+            np.full(max(dims[1], 2), -1, dtype="float64") * length_unit,
+            np.full(max(dims[2], 2), -1, dtype="float64") * length_unit,
         )
 
         for idir, edges in enumerate(cell_edges[:3]):
             if dims[idir] > 1:
                 cell_centers[idir][:] = 0.5 * (edges[1:] + edges[:-1])
             else:
                 cell_centers[idir][:] = edges[0]
+            npt.assert_array_less(0, cell_centers)
+
         return cell_centers
 
 
 class GoodboyDataset(Dataset, ABC):
     """
     Abstract class that defines interfaces common to all concrete dataset classes in this module
     """
```

### Comparing `yt_idefix-2.0.0/yt_idefix/definitions.py` & `yt_idefix-2.0.1/yt_idefix/definitions.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.0/yt_idefix/fields.py` & `yt_idefix-2.0.1/yt_idefix/fields.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.0/yt_idefix/io.py` & `yt_idefix-2.0.1/yt_idefix/io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.0/yt_idefix.egg-info/PKG-INFO` & `yt_idefix-2.0.1/yt_idefix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-idefix
-Version: 2.0.0
+Version: 2.0.1
 Summary: An extension module for yt, adding a frontend for Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Documentation, https://yt-project.org/docs/dev/
 Project-URL: Source, https://github.com/neutrinoceros/yt_idefix
 Project-URL: Tracker, https://github.com/neutrinoceros/yt_idefix/issues
@@ -34,15 +34,15 @@
 [![PyPI](https://img.shields.io/badge/requires-Python%20≥%203.8-blue?logo=python&logoColor=white)](https://pypi.org/project/yt_idefix/)
 [![yt-project](https://img.shields.io/static/v1?label="works%20with"&message="yt"&color="blueviolet")](https://yt-project.org)
 
 <!--- Tests and style --->
 [![CI](https://github.com/neutrinoceros/yt_idefix/actions/workflows/ci.yml/badge.svg)](https://github.com/neutrinoceros/yt_idefix/actions/workflows/ci.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/yt_idefix/main.svg)](https://results.pre-commit.ci/latest/github/neutrinoceros/yt_idefix/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 A maturing yt frontend for Idefix and Pluto, packaged as an extension for yt.
 
 ## Installation
 
 ```shell
 python -m pip install yt_idefix
```

### Comparing `yt_idefix-2.0.0/yt_idefix.egg-info/SOURCES.txt` & `yt_idefix-2.0.1/yt_idefix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

