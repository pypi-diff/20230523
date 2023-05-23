# Comparing `tmp/planetmapper-1.7.0.tar.gz` & `tmp/planetmapper-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmapper-1.7.0.tar", last modified: Tue May  2 13:21:03 2023, max compression
+gzip compressed data, was "planetmapper-1.7.1.tar", last modified: Tue May 23 15:24:52 2023, max compression
```

## Comparing `planetmapper-1.7.0.tar` & `planetmapper-1.7.1.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:21:03.983509 planetmapper-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-02 13:21:03.983509 planetmapper-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-02 13:20:42.000000 planetmapper-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:21:03.979509 planetmapper-1.7.0/planetmapper/
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    75150 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/body.py
--rw-r--r--   0 runner    (1001) docker     (123)   110519 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:21:03.979509 planetmapper-1.7.0/planetmapper/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/data/rings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   116259 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/kernel_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    45504 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-05-02 13:20:42.000000 planetmapper-1.7.0/planetmapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:21:03.979509 planetmapper-1.7.0/planetmapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-02 13:21:03.000000 planetmapper-1.7.0/planetmapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-02 13:21:03.000000 planetmapper-1.7.0/planetmapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:21:03.000000 planetmapper-1.7.0/planetmapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-02 13:21:03.000000 planetmapper-1.7.0/planetmapper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-02 13:21:03.000000 planetmapper-1.7.0/planetmapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 13:21:03.000000 planetmapper-1.7.0/planetmapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 13:20:42.000000 planetmapper-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 13:21:03.983509 planetmapper-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-02 13:20:42.000000 planetmapper-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:21:03.983509 planetmapper-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-05-02 13:20:42.000000 planetmapper-1.7.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-02 13:20:42.000000 planetmapper-1.7.0/tests/test_basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-05-02 13:20:42.000000 planetmapper-1.7.0/tests/test_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    25986 2023-05-02 13:20:42.000000 planetmapper-1.7.0/tests/test_body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-02 13:20:42.000000 planetmapper-1.7.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-02 13:20:42.000000 planetmapper-1.7.0/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-02 13:20:42.000000 planetmapper-1.7.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    19129 2023-05-02 13:20:42.000000 planetmapper-1.7.0/tests/test_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-05-02 13:20:42.000000 planetmapper-1.7.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:24:52.612048 planetmapper-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-23 15:24:52.612048 planetmapper-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-23 15:24:38.000000 planetmapper-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:24:52.608048 planetmapper-1.7.1/planetmapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80314 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112086 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:24:52.608048 planetmapper-1.7.1/planetmapper/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/data/ring_aliases.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/data/rings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118001 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/kernel_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46384 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-05-23 15:24:38.000000 planetmapper-1.7.1/planetmapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:24:52.608048 planetmapper-1.7.1/planetmapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-23 15:24:52.000000 planetmapper-1.7.1/planetmapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-23 15:24:52.000000 planetmapper-1.7.1/planetmapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:24:52.000000 planetmapper-1.7.1/planetmapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-23 15:24:52.000000 planetmapper-1.7.1/planetmapper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-23 15:24:52.000000 planetmapper-1.7.1/planetmapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 15:24:52.000000 planetmapper-1.7.1/planetmapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-23 15:24:38.000000 planetmapper-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 15:24:52.612048 planetmapper-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-23 15:24:38.000000 planetmapper-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:24:52.612048 planetmapper-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17369 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28382 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29709 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_kernel_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20963 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-23 15:24:38.000000 planetmapper-1.7.1/tests/test_utils.py
```

### Comparing `planetmapper-1.7.0/PKG-INFO` & `planetmapper-1.7.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.7.0
+Version: 1.7.1
 Summary: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
 Project-URL: GitHub, https://github.com/ortk95/planetmapper
 Keywords: planetmapper,astronomy,space,science,spice,ephemeris,planetary-science
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 
 # PlanetMapper
 
 [![PyPI](https://img.shields.io/pypi/v/planetmapper?label=PyPi&logo=python&logoColor=silver)](https://pypi.org/project/planetmapper/)
-[![Upload Python Package](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml)
+[![Upload Package](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml)
 [![Pylint](https://github.com/ortk95/planetmapper/actions/workflows/pylint.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/pylint.yml)
-[![Black](https://github.com/ortk95/planetmapper/actions/workflows/black.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/black.yml)
-[![Tests](https://github.com/ortk95/planetmapper/actions/workflows/unittest.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/unittest.yml)
+[![Format](https://github.com/ortk95/planetmapper/actions/workflows/format.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/format.yml)
+[![Tests](https://github.com/ortk95/planetmapper/actions/workflows/test.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/test.yml)
+[![Coverage Status](https://img.shields.io/coverallsCoverage/github/ortk95/planetmapper)](https://coveralls.io/github/ortk95/planetmapper)
 [![Documentation Status](https://readthedocs.org/projects/planetmapper/badge/?version=latest)](https://planetmapper.readthedocs.io/en/latest/?badge=latest)
 
 
 A Python module for visualising, navigating and mapping Solar System observations.
 
 ## [Documentation](https://planetmapper.readthedocs.io)
 For full documentation and [API reference](https://planetmapper.readthedocs.io/en/latest/documentation.html), visit [planetmapper.readthedocs.io](https://planetmapper.readthedocs.io/en/latest/index.html)
@@ -32,15 +33,15 @@
 ```
 pip install planetmapper --upgrade
 ```
 
 _Requires Python 3.10+_
 
 ## Key features
-### [Fit and map observations using a full featured user interface](https://planetmapper.readthedocs.io/en/latest/user_interface.html)
+### [Fit and map astronomical observations using a full featured user interface](https://planetmapper.readthedocs.io/en/latest/user_interface.html)
 ![PlanetMapper graphical user interface](https://github.com/ortk95/planetmapper/blob/main/docs/images/gui_fitting.png?raw=true)
 
 ### [Easily visualise solar system observations with just a few lines of code](https://planetmapper.readthedocs.io/en/latest/general_python_api.html#wireframe-plots)
 
 ```python
 body = planetmapper.Body('saturn', '2020-01-01')
 body.plot_wireframe_radec()
```

### Comparing `planetmapper-1.7.0/README.md` & `planetmapper-1.7.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # PlanetMapper
 
 [![PyPI](https://img.shields.io/pypi/v/planetmapper?label=PyPi&logo=python&logoColor=silver)](https://pypi.org/project/planetmapper/)
-[![Upload Python Package](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml)
+[![Upload Package](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml)
 [![Pylint](https://github.com/ortk95/planetmapper/actions/workflows/pylint.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/pylint.yml)
-[![Black](https://github.com/ortk95/planetmapper/actions/workflows/black.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/black.yml)
-[![Tests](https://github.com/ortk95/planetmapper/actions/workflows/unittest.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/unittest.yml)
+[![Format](https://github.com/ortk95/planetmapper/actions/workflows/format.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/format.yml)
+[![Tests](https://github.com/ortk95/planetmapper/actions/workflows/test.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/test.yml)
+[![Coverage Status](https://img.shields.io/coverallsCoverage/github/ortk95/planetmapper)](https://coveralls.io/github/ortk95/planetmapper)
 [![Documentation Status](https://readthedocs.org/projects/planetmapper/badge/?version=latest)](https://planetmapper.readthedocs.io/en/latest/?badge=latest)
 
 
 A Python module for visualising, navigating and mapping Solar System observations.
 
 ## [Documentation](https://planetmapper.readthedocs.io)
 For full documentation and [API reference](https://planetmapper.readthedocs.io/en/latest/documentation.html), visit [planetmapper.readthedocs.io](https://planetmapper.readthedocs.io/en/latest/index.html)
@@ -18,15 +19,15 @@
 ```
 pip install planetmapper --upgrade
 ```
 
 _Requires Python 3.10+_
 
 ## Key features
-### [Fit and map observations using a full featured user interface](https://planetmapper.readthedocs.io/en/latest/user_interface.html)
+### [Fit and map astronomical observations using a full featured user interface](https://planetmapper.readthedocs.io/en/latest/user_interface.html)
 ![PlanetMapper graphical user interface](https://github.com/ortk95/planetmapper/blob/main/docs/images/gui_fitting.png?raw=true)
 
 ### [Easily visualise solar system observations with just a few lines of code](https://planetmapper.readthedocs.io/en/latest/general_python_api.html#wireframe-plots)
 
 ```python
 body = planetmapper.Body('saturn', '2020-01-01')
 body.plot_wireframe_radec()
```

### Comparing `planetmapper-1.7.0/planetmapper/__init__.py` & `planetmapper-1.7.1/planetmapper/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,24 +70,21 @@
 
 .. warning::
 
     This code is in active development, so may contain bugs! Any issues, bugs and 
     suggestions can be 
     `reported on GitHub <https://github.com/ortk95/planetmapper/issues/new>`__.
 """
-from .common import __version__, __author__, __url__
-from .base import SpiceBase, set_kernel_path, get_kernel_path
-from .body import Body, DEFAULT_WIREFRAME_FORMATTING
+from . import data_loader, gui, kernel_downloader, utils
+from .base import SpiceBase, get_kernel_path, set_kernel_path
+from .basic_body import BasicBody
+from .body import DEFAULT_WIREFRAME_FORMATTING, Body
 from .body_xy import Backplane, BodyXY
+from .common import __author__, __url__, __version__
 from .observation import Observation
-from .basic_body import BasicBody
-from . import gui
-from . import utils
-from . import kernel_downloader
-from . import data_loader
 
 __all__ = [
     'set_kernel_path',
     'get_kernel_path',
     'SpiceBase',
     'Body',
     'Backplane',
@@ -100,8 +97,9 @@
     'data_loader',
     'DEFAULT_WIREFRAME_FORMATTING',
 ]
 
 
 def main():
     """:meta private:"""
+    # pylint: disable-next=protected-access
     gui._main()
```

### Comparing `planetmapper-1.7.0/planetmapper/body.py` & `planetmapper-1.7.1/planetmapper/body.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 import datetime
 from collections import defaultdict
-from typing import Callable, Literal, cast, TypedDict, Any
+from typing import Any, Callable, Literal, TypedDict, cast, overload
 
 try:
     from typing import Unpack
 except ImportError:
     from typing_extensions import Unpack
+try:
+    from typing import Self
+except ImportError:
+    from typing_extensions import Self
 
 import matplotlib.patheffects as path_effects
 import matplotlib.pyplot as plt
 import matplotlib.transforms
 import numpy as np
 import spiceypy as spice
 from matplotlib.axes import Axes
 from spiceypy.utils.exceptions import (
     NotFoundError,
+    SpiceBODIESNOTDISTINCT,
     SpiceKERNELVARNOTFOUND,
     SpiceSPKINSUFFDATA,
 )
 
 from . import data_loader, utils
-from .base import SpiceBase, Numeric
+from .base import BodyBase, Numeric
 from .basic_body import BasicBody
 
 _WireframeComponent = Literal[
     'all',
     'grid',
     'equator',
     'prime_meridian',
@@ -33,26 +38,32 @@
     'terminator',
     'ring',
     'pole',
     'coordinate_of_interest_lonlat',
     'coordinate_of_interest_radec',
     'other_body_of_interest_marker',
     'other_body_of_interest_label',
+    'hidden_other_body_of_interest_marker',
+    'hidden_other_body_of_interest_label',
     'map_boundary',
 ]
 
 
 class _WireframeKwargs(TypedDict, total=False):
     label_poles: bool
     add_title: bool
     grid_interval: float
     indicate_equator: bool
     indicate_prime_meridian: bool
     formatting: dict[_WireframeComponent, dict[str, Any]] | None
+
+    # Hints for common formatting parameters to make type checking/autocomplete happy
     color: str | tuple[float, float, float]
+    alpha: float
+    zorder: float
 
 
 DEFAULT_WIREFRAME_FORMATTING: dict[_WireframeComponent, dict[str, Any]] = {
     'all': dict(color='k'),
     'grid': dict(alpha=0.5, linestyle=':'),
     'equator': dict(linestyle='-'),
     'prime_meridian': dict(linestyle='-'),
@@ -77,19 +88,21 @@
     'other_body_of_interest_label': dict(
         size='small',
         ha='center',
         va='center',
         alpha=0.5,
         clip_on=True,
     ),
+    'hidden_other_body_of_interest_marker': dict(alpha=0.333),
+    'hidden_other_body_of_interest_label': dict(),
     'map_boundary': dict(),
 }
 
 
-class Body(SpiceBase):
+class Body(BodyBase):
     """
     Class representing an astronomical body observed at a specific time.
 
     Generally only `target`, `utc` and `observer` need to be changed. The additional
     parameters allow customising the exact settings used in the internal SPICE
     functions. Similarly, some methods (e.g. :func:`terminator_radec`) have parameters
     that are passed to SPICE functions which can almost always be left as their default
@@ -98,14 +111,16 @@
     for more details about possible parameter values.
 
     The `target` and `observer` names are passed to
     :func:`SpiceBase.standardise_body_name`, so a variety of formats are acceptable. For
     example `'jupiter'`, `'JUPITER'`, `' Jupiter '`, `'599'` and `599` will
     all resolve to `'JUPITER'`.
 
+    :class:`Body` instances are hashable, so can be used as dictionary keys.
+
     This class inherits from :class:`SpiceBase` so the methods described above are also
     available.
 
     Args:
         target: Name of target body.
         utc: Time of observation. This can be provided in a variety of formats and is
             assumed to be UTC unless otherwise specified. The accepted formats are: any
@@ -136,15 +151,22 @@
         aberration_correction: str = 'CN',
         observer_frame: str = 'J2000',
         illumination_source: str = 'SUN',
         subpoint_method: str = 'INTERCEPT/ELLIPSOID',
         surface_method: str = 'ELLIPSOID',
         **kwargs,
     ) -> None:
-        super().__init__(**kwargs)
+        super().__init__(
+            target=target,
+            utc=utc,
+            observer=observer,
+            aberration_correction=aberration_correction,
+            observer_frame=observer_frame,
+            **kwargs,
+        )
 
         # Document instance variables
         self.et: float
         """Ephemeris time of the observation corresponding to `utc`."""
         self.dtm: datetime.datetime
         """Python timezone aware datetime of the observation corresponding to `utc`."""
         self.target_body_id: int
@@ -246,47 +268,23 @@
         self.other_bodies_of_interest: list[Body | BasicBody]
         """
         List of other bodies of interest to mark when plotting. Add to this list using 
         :func:`add_other_bodies_of_interest`.
         """
 
         # Process inputs
-        if isinstance(utc, float):
-            utc = self.mjd2dtm(utc)
-        if utc is None:
-            utc = datetime.datetime.now(datetime.timezone.utc)
-        if isinstance(utc, datetime.datetime):
-            # convert input datetime to UTC, then to a string compatible with spice
-            utc = utc.replace(tzinfo=datetime.timezone.utc)
-            utc = utc.strftime(self._DEFAULT_DTM_FORMAT_STRING)
-
-        self.target = self.standardise_body_name(target)
-        self.observer = self.standardise_body_name(observer)
-        self.observer_frame = observer_frame
         self.illumination_source = illumination_source
-        self.aberration_correction = aberration_correction
         self.subpoint_method = subpoint_method
         self.surface_method = surface_method
 
-        # Encode strings which are regularly passed to spice (for speed)
-        self._target_encoded = self._encode_str(self.target)
-        self._observer_encoded = self._encode_str(self.observer)
-        self._observer_frame_encoded = self._encode_str(self.observer_frame)
         self._illumination_source_encoded = self._encode_str(self.illumination_source)
-        self._aberration_correction_encoded = self._encode_str(
-            self.aberration_correction
-        )
         self._subpoint_method_encoded = self._encode_str(self.subpoint_method)
         self._surface_method_encoded = self._encode_str(self.surface_method)
 
         # Get target properties and state
-        self.et = spice.utc2et(utc)
-        self.dtm: datetime.datetime = self.et2dtm(self.et)
-        self.utc = self.dtm.strftime(self._DEFAULT_DTM_FORMAT_STRING)
-        self.target_body_id: int = spice.bodn2c(self.target)
         self.target_frame = 'IAU_' + self.target
         self._target_frame_encoded = self._encode_str(self.target_frame)
 
         self.radii = spice.bodvar(self.target_body_id, 'RADII', 3)
         self.r_eq = self.radii[0]
         self.r_polar = self.radii[2]
         self.flattening = (self.r_eq - self.r_polar) / self.r_eq
@@ -300,45 +298,28 @@
         if self.prograde and self.target_body_id not in {10, 301, 399}:
             # {10, 301, 399} accounts for special cases of SUN, MOON and EARTH which are
             # positive east even though they are prograde.
             self.positive_longitude_direction = 'W'
         else:
             self.positive_longitude_direction = 'E'
 
-        starg, lt = spice.spkezr(
-            self._target_encoded,  # type: ignore
-            self.et,
-            self._observer_frame_encoded,  # type: ignore
-            self._aberration_correction_encoded,  # type: ignore
-            self._observer_encoded,  # type: ignore
-        )
-        self._target_obsvec = cast(np.ndarray, starg)[:3]
-        self.target_light_time = cast(float, lt)
-        # cast() calls are only here to make type checking play nicely with spice.spkezr
-        self.target_distance = self.target_light_time * self.speed_of_light()
-        self._target_ra_radians, self._target_dec_radians = self._obsvec2radec_radians(
-            self._target_obsvec
-        )
-        self.target_ra, self.target_dec = self._radian_pair2degrees(
-            self._target_ra_radians, self._target_dec_radians
-        )
         self.target_diameter_arcsec = (
             60 * 60 * np.rad2deg(np.arcsin(2 * self.r_eq / self.target_distance))
         )
 
         # Find sub observer point
         self._subpoint_targvec, self._subpoint_et, self._subpoint_rayvec = spice.subpnt(
             self._subpoint_method_encoded,  # type: ignore
             self._target_encoded,  # type: ignore
             self.et,
             self._target_frame_encoded,  # type: ignore
             self._aberration_correction_encoded,  # type: ignore
             self._observer_encoded,  # type: ignore
         )
-        self.subpoint_distance = np.linalg.norm(self._subpoint_rayvec)
+        self.subpoint_distance = float(np.linalg.norm(self._subpoint_rayvec))
         self.subpoint_lon, self.subpoint_lat = self.targvec2lonlat(
             self._subpoint_targvec
         )
         self._subpoint_obsvec = self._rayvec2obsvec(
             self._subpoint_rayvec, self._subpoint_et
         )
         self._subpoint_ra, self._subpoint_dec = self._radian_pair2degrees(
@@ -376,25 +357,48 @@
                     self.ring_radii.add(r)
 
     def __repr__(self) -> str:
         return f'Body({self.target!r}, {self.utc!r}, observer={self.observer!r})'
 
     def _get_equality_tuple(self) -> tuple:
         return (
-            self.target,
-            self.utc,
-            self.observer,
-            self.observer_frame,
             self.illumination_source,
-            self.aberration_correction,
             self.subpoint_method,
             self.surface_method,
             super()._get_equality_tuple(),
         )
 
+    def _get_kwargs(self) -> dict[str, Any]:
+        return super()._get_kwargs() | dict(
+            illumination_source=self.illumination_source,
+            subpoint_method=self.subpoint_method,
+            surface_method=self.surface_method,
+        )
+
+    def _copy_options_to_other(self, other: Self) -> None:
+        super()._copy_options_to_other(other)
+        other.other_bodies_of_interest = self.other_bodies_of_interest.copy()
+        other.coordinates_of_interest_lonlat = (
+            self.coordinates_of_interest_lonlat.copy()
+        )
+        other.coordinates_of_interest_radec = self.coordinates_of_interest_radec.copy()
+        other.ring_radii = self.ring_radii.copy()
+
+    @overload
+    def create_other_body(
+        self, other_target: str | int, fallback_to_basic_body: Literal[False]
+    ) -> 'Body':
+        ...
+
+    @overload
+    def create_other_body(
+        self, other_target: str | int, fallback_to_basic_body: bool = True
+    ) -> 'Body|BasicBody':
+        ...
+
     def create_other_body(
         self, other_target: str | int, fallback_to_basic_body: bool = True
     ) -> 'Body|BasicBody':
         """
         Create a :class:`Body` instance using identical parameters but just with a
         different target. For example, the `europa` body created here will have
         identical parameters (see below) to the `jupiter` body, just with a different
@@ -440,15 +444,17 @@
                 utc=self.utc,
                 observer=self.observer,
                 observer_frame=self.observer_frame,
                 aberration_correction=self.aberration_correction,
             )
 
     # Stuff to customise wireframe plots
-    def add_other_bodies_of_interest(self, *other_targets: str | int) -> None:
+    def add_other_bodies_of_interest(
+        self, *other_targets: str | int, only_visible: bool = False
+    ) -> None:
         """
         Add targets to the list of :attr:`other_bodies_of_interest` of interest to mark
         when plotting. The other targets are created using :func:`create_other_body`.
         For example, to add the Galilean moons as other targets to a Jupiter body,
         use ::
 
             body = planetmapper.Body('Jupiter')
@@ -462,72 +468,106 @@
             # Uranus' satellites have ID codes 701, 702, 703 etc, so this adds 10 moons
             # with a single function call
 
         See also :func:`add_satellites_to_bodies_of_interest`.
 
         Args:
             *other_targets: Names of the other targets, passed to :class:`Body`
+            only_visible: If `True`, other targets which are hidden behind the target
+                will not be added to :attr:`other_bodies_of_interest`.
         """
         for other_target in other_targets:
-            self.other_bodies_of_interest.append(self.create_other_body(other_target))
+            body = self.create_other_body(other_target)
+            if only_visible and not self.test_if_other_body_visible(body):
+                continue
+            if body not in self.other_bodies_of_interest:
+                self.other_bodies_of_interest.append(body)
+
+    def _get_all_satellite_bodies(
+        self, skip_insufficient_data: bool = False, only_visible: bool = False
+    ) -> 'list[Body | BasicBody]':
+        out: 'list[Body | BasicBody]' = []
+        id_base = (self.target_body_id // 100) * 100
+        for other_target in range(id_base + 1, id_base + 99):
+            try:
+                body = self.create_other_body(other_target)
+                if only_visible and not self.test_if_other_body_visible(body):
+                    continue
+                out.append(body)
+            except SpiceSPKINSUFFDATA:
+                if skip_insufficient_data:
+                    continue
+                raise
+            except NotFoundError:
+                continue
+        return out
 
     def add_satellites_to_bodies_of_interest(
-        self, skip_insufficient_data: bool = False
+        self, skip_insufficient_data: bool = False, only_visible: bool = False
     ) -> None:
         """
         Automatically add all satellites in the target planetary system to
         :attr:`other_bodies_of_interest`.
 
         This uses the NAIF ID codes to identify the satellites. For example, Uranus has
         an ID of 799, and its satellites have codes 701, 702, 703..., so any object with
         a code in the range 701 to 798 is added for Uranus.
 
         See also :func:`add_other_bodies_of_interest`.
 
         Args:
             skip_insufficient_data: If True, satellites with insufficient data in the
                 SPICE kernel will be skipped. If False, an exception will be raised.
+            only_visible: If `True`, satellites which are hidden behind the target body
+                will not be added.
         """
-        id_base = (self.target_body_id // 100) * 100
-        for other_target in range(id_base + 1, id_base + 99):
-            try:
-                self.other_bodies_of_interest.append(
-                    self.create_other_body(other_target)
-                )
-            except SpiceSPKINSUFFDATA:
-                if skip_insufficient_data:
-                    continue
-                else:
-                    raise
-            except NotFoundError:
-                continue
+        satellites = self._get_all_satellite_bodies(
+            skip_insufficient_data=skip_insufficient_data, only_visible=only_visible
+        )
+        for satellite in satellites:
+            if satellite not in self.other_bodies_of_interest:
+                self.other_bodies_of_interest.append(satellite)
+
+    @staticmethod
+    def _standardise_ring_name(name: str) -> str:
+        name = name.casefold().strip().removesuffix('ring')
+        for a, b in data_loader.get_ring_aliases().items():
+            name = name.replace(a, b)
+        return name.casefold().strip()
 
     def ring_radii_from_name(self, name: str) -> list[float]:
         """
         Get list of ring radii in km for a named ring.
 
         This is a convenience function to load data from :attr:`named_ring_data`.
 
         Args:
-            name: Name of ring. This is case insensitive.
+            name: Name of ring. This is case insensitive and, "ring" suffix is
+                optional and non-ASCII versions are allowed. For example, `'liberte'`
+                will load the `'Liberté'` ring radii for Uranus and `'amalthea'` will
+                load the `'Amalthea Ring'` radii for Jupiter.
 
         Raises:
             ValueError: if no ring with the provided name is found.
 
         Returns:
             List of ring radii in km. If the length of this list is 2, then the values
             give the inner and outer radii of the ring respectively. Otherwise, the
             length should be 1, meaning the ring has a single radius.
         """
-        standardise = lambda name: name.casefold().strip().removesuffix('ring').strip()
-        name = standardise(name.casefold().strip())
+        name = self._standardise_ring_name(name)
         for n, radii in self.named_ring_data.items():
-            if name == standardise(n):
+            if name == self._standardise_ring_name(n):
                 return radii
-        raise ValueError(f'No rings found named {name!r} in named_ring_data')
+        raise ValueError(
+            f'No rings found named {name!r} in named_ring_data.'
+            + '\nValid names: {}'.format(
+                [self._standardise_ring_name(n) for n in self.named_ring_data.keys()]
+            )
+        )
 
     def add_named_rings(self, *names: str) -> None:
         """
         Add named rings to :attr:`ring_radii` so that they appear when creating
         wireframe plots. If no arguments are provided (i.e. calling
         `body.add_named_rings()`), then all rings in :attr:`named_ring_data` are added
         to :attr:`ring_radii`.
@@ -563,17 +603,15 @@
 
     def _targvec2obsvec(self, targvec: np.ndarray) -> np.ndarray:
         """
         Transform rectangular vector in target frame to rectangular vector in observer
         frame.
         """
         # Get the target vector from the subpoint to the point of interest
-        targvec_offset = targvec - self._subpoint_targvec  # type: ignore
-        # ^ ignoring type warning due to numpy bug (TODO remove type: ingore in future)
-        # https://github.com/numpy/numpy/issues/22437
+        targvec_offset = targvec - self._subpoint_targvec
 
         # Calculate the difference in LOS distance between observer<->subpoint and
         # observer<->point of interest
         dist_offset = (
             np.linalg.norm(self._subpoint_rayvec + targvec_offset)
             - self.subpoint_distance
         )
@@ -585,15 +623,15 @@
 
         # Create the transform matrix converting between the target vector at the time
         # the ray left the point of interest -> the observer vector at the time the ray
         # hit the detector
         transform_matrix = spice.pxfrm2(
             self._target_frame_encoded,  # type: ignore
             self._observer_frame_encoded,  # type: ignore
-            targvec_et,
+            targvec_et,  #  type: ignore
             self.et,
         )
 
         # Use the transform matrix to perform the actual transformation
         return self._subpoint_obsvec + np.matmul(transform_matrix, targvec_offset)
 
     def _rayvec2obsvec(self, rayvec: np.ndarray, et: float) -> np.ndarray:
@@ -605,37 +643,28 @@
             self._target_frame_encoded,  # type: ignore
             self._observer_frame_encoded,  # type: ignore
             et,
             self.et,
         )
         return np.matmul(px, rayvec)
 
-    def _obsvec2radec_radians(self, obsvec: np.ndarray) -> tuple[float, float]:
-        """
-        Transform rectangular vector in observer frame to observer ra/dec coordinates.
-        """
-        dst, ra, dec = spice.recrad(obsvec)
-        return ra, dec
-
     # Coordinate transformations observer -> target direction
     def _radec2obsvec_norm_radians(self, ra: float, dec: float) -> np.ndarray:
         return spice.radrec(1, ra, dec)
 
     def _obsvec2targvec(self, obsvec: np.ndarray) -> np.ndarray:
         """
         Transform rectangular vector in observer frame to rectangular vector in target
         frame.
 
         Based on inverse of _targvec2obsvec
         """
 
         # Get the target vector from the subpoint to the point of interest
-        obsvec_offset = obsvec - self._subpoint_obsvec  # type: ignore
-        # ^ ignoring type warning due to numpy bug (TODO remove type: ingore in future)
-        # https://github.com/numpy/numpy/issues/22437
+        obsvec_offset = obsvec - self._subpoint_obsvec
 
         # Calculate the difference in LOS distance between observer<->subpoint and
         # observer<->point of interest
         dist_offset = (
             np.linalg.norm(-self._subpoint_rayvec + obsvec_offset)
             - self.subpoint_distance
         )
@@ -648,23 +677,23 @@
         # Create the transform matrix converting between the target vector at the time
         # the ray left the point of interest -> the observer vector at the time the ray
         # hit the detector
         transform_matrix = spice.pxfrm2(
             self._observer_frame_encoded,  # type: ignore
             self._target_frame_encoded,  # type: ignore
             self.et,
-            obsvec_et,
+            obsvec_et,  # type: ignore
         )
 
         # Use the transform matrix to perform the actual transformation
         return self._subpoint_targvec + np.matmul(transform_matrix, obsvec_offset)
 
     def _obsvec_norm2targvec(self, obsvec_norm: np.ndarray) -> np.ndarray:
         """TODO add note about raising NotFoundError"""
-        spoint, trgepc, srfvec = spice.sincpt(
+        spoint, *_ = spice.sincpt(
             self._surface_method_encoded,
             self._target_encoded,
             self.et,
             self._target_frame_encoded,
             self._aberration_correction_encoded,
             self._observer_encoded,
             self._observer_frame_encoded,
@@ -943,15 +972,15 @@
         Returns:
             Matplotlib transformation from `radec` to `km` coordinates.
         """
         if self._mpl_transform_radec2km is None:
             transform_rad2deg = matplotlib.transforms.Affine2D().scale(np.deg2rad(1))
             self._mpl_transform_radec2km = (
                 transform_rad2deg + self._get_matplotlib_radec2km_transform_radians()
-            )  #  type: ignore
+            )
         transform = self._mpl_transform_radec2km
         if ax:
             transform = transform + ax.transData
         return transform
 
     def matplotlib_km2radec_transform(
         self, ax: Axes | None = None
@@ -1080,14 +1109,116 @@
             lat: Latitude of point on target body.
 
         Returns:
             True if the point is visible from the observer, otherwise False.
         """
         return self._test_if_targvec_visible(self.lonlat2targvec(lon, lat))
 
+    def other_body_los_intercept(
+        self, other: 'str | int | Body | BasicBody'
+    ) -> None | Literal['transit', 'hidden', 'part transit', 'part hidden', 'same']:
+        """
+        Test for line-of-sight intercept between the target body and another body.
+
+        This can be used to test for if another body (e.g. a moon) is in front of or
+        behind the target body (e.g. a planet).
+
+        See also :func:`test_if_other_body_visible`.
+
+        .. warning::
+
+            This method does not perform any checks to ensure that any input
+            :class:`Body` or :class:`BasicBody` instances have a consistent observer
+            location and observation time as the target body.
+
+        Args:
+            other: Other body to test for intercept with. Can be a :class`Body` (or
+                :class:`BasicBody`) instance, or a string/integer NAIF ID code which is
+                passed to :func:`create_other_body`.
+
+        Returns:
+            `None` if there is no intercept, otherwise a string indicating the type of
+            intercept. For example, with `jupiter.other_body_los_intercept('europa')`,
+            the possible return values mean:
+
+                - `None` - there is no intercept, meaning that Europa and Jupiter do not
+                  overlap in the sky.
+                - `'hidden'` - all of Europa's disk is hidden behind Jupiter.
+                - `'part hidden'` - part of Europa's disk is hidden behind Jupiter and
+                  part is visible.
+                - `'transit'` - all of Europa's disk is in front of Jupiter.
+                - `'part transit'` - part of Europa's disk is in front of Jupiter.
+
+            The return value can also be `'same'`, which means that the other body is
+            the same object as the target body (or has an identical location).
+        """
+        if not isinstance(other, BodyBase):
+            other = self.create_other_body(other)
+
+        if isinstance(other, BasicBody):
+            try:
+                self.radec2lonlat(
+                    other.target_ra, other.target_dec, not_found_nan=False
+                )
+            except NotFoundError:
+                return None  # No intercept with the target body
+            if other.target_distance == self.target_distance:
+                return 'same'
+            elif other.target_distance - self.target_distance > 0:
+                return 'hidden'
+            else:
+                return 'transit'
+
+        try:
+            occultation = spice.occult(
+                self.target,
+                'ELLIPSOID',
+                self.target_frame,
+                other.target,
+                'ELLIPSOID',
+                other.target_frame,
+                self.aberration_correction,
+                self.observer,
+                self.et,
+            )
+        except SpiceBODIESNOTDISTINCT:
+            return 'same'
+
+        match occultation:
+            case 3:
+                return 'hidden'
+            case 1 | 2:
+                return 'part hidden'
+            case 0:
+                return None
+            case -1 | -3:
+                return 'part transit'
+            case -2:
+                return 'transit'
+        raise ValueError(f'Unknown occultation code: {occultation}')
+
+    def test_if_other_body_visible(self, other: 'str | int | Body | BasicBody') -> bool:
+        """
+        Test if another body is visible, or is hidden behind the target body.
+
+        This is a convenience method equivalent to: ::
+
+            body.other_body_los_intercept(other) != 'hidden'
+
+        Args:
+            other: Other body to test for visibility, passed to
+                :func:`other_body_los_intercept`.
+
+        Returns:
+            `False` if the other body is hidden behind the target body, otherwise
+            `True`. If any part of the other body is visible, this method will return
+            `True`.
+        """
+        return self.other_body_los_intercept(other) != 'hidden'
+
     # Illumination
     def _illumination_angles_from_targvec_radians(
         self, targvec: np.ndarray
     ) -> tuple[float, float, float]:
         phase, incdnc, emissn, visibl, lit = self._illumf_from_targvec_radians(targvec)
         return phase, incdnc, emissn
 
@@ -1692,18 +1823,31 @@
         for radius in self.ring_radii:
             ra, dec = self.ring_radec(radius)
             ax.plot(ra, dec, **kwargs['ring'])
 
         for body in self.other_bodies_of_interest:
             ra = body.target_ra
             dec = body.target_dec
+            label = body.target
+            hidden = not self.test_if_other_body_visible(body)
+            if hidden:
+                label = f'({label})'
             ax.text(
-                ra, dec, body.target + '\n', **kwargs['other_body_of_interest_label']
+                ra,
+                dec,
+                label + '\n',
+                **kwargs['other_body_of_interest_label']
+                | (kwargs['hidden_other_body_of_interest_label'] if hidden else {}),
+            )
+            ax.scatter(
+                ra,
+                dec,
+                **kwargs['other_body_of_interest_marker']
+                | (kwargs['hidden_other_body_of_interest_marker'] if hidden else {}),
             )
-            ax.scatter(ra, dec, **kwargs['other_body_of_interest_marker'])
 
         if add_title:
             ax.set_title(self.get_description(multiline=True))
         return ax
 
     def plot_wireframe_radec(
         self,
@@ -1797,15 +1941,17 @@
                 `color` of the plotted rings to red, you could use::
 
                     body.plot_wireframe_radec(formatting={'ring': {'color': 'r'}})
 
                 The following components can be formatted: `grid`, `equator`,
                 `prime_meridian`, `limb`, `limb_illuminated`, `terminator`, `ring`,
                 `pole`, `coordinate_of_interest_lonlat`, `coordinate_of_interest_radec`,
-                `other_body_of_interest_marker`, `other_body_of_interest_label`.
+                `other_body_of_interest_marker`, `other_body_of_interest_label`,
+                `hidden_other_body_of_interest_marker`,
+                `hidden_other_body_of_interest_label`.
 
             **kwargs: Additional arguments are passed to Matplotlib plotting functions
                 for all components. This is useful for specifying properties like
                 `color` to customise the entire wireframe rather than a single
                 component. For example, to make the entire wireframe red, you could
                 use::
```

### Comparing `planetmapper-1.7.0/planetmapper/body_xy.py` & `planetmapper-1.7.1/planetmapper/body_xy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,128 +1,45 @@
 import datetime
+import io
 import math
 import warnings
-import functools
-import io
 from typing import (
-    cast,
     Any,
     Callable,
-    Concatenate,
     Iterable,
     Literal,
     NamedTuple,
-    ParamSpec,
     Protocol,
-    TypeVar,
     TypedDict,
+    cast,
 )
 
 try:
     from typing import Unpack
 except ImportError:
     from typing_extensions import Unpack
+try:
+    from typing import Self
+except ImportError:
+    from typing_extensions import Self
 
 import matplotlib.patches
 import matplotlib.pyplot as plt
 import matplotlib.transforms
 import numpy as np
 import pyproj
 import scipy.interpolate
 from matplotlib.axes import Axes
 from matplotlib.collections import QuadMesh
 from spiceypy.utils.exceptions import NotFoundError
 
-from .body import (
-    Body,
-    _WireframeKwargs,
-    _WireframeComponent,
-    DEFAULT_WIREFRAME_FORMATTING,
-)
+from .base import _cache_clearable_result, _cache_stable_result
+from .body import Body, _WireframeComponent, _WireframeKwargs
 from .progress import progress_decorator
 
-T = TypeVar('T')
-S = TypeVar('S')
-P = ParamSpec('P')
-
-
-def _cache_clearable_result(
-    fn: Callable[Concatenate[S, P], T]
-) -> Callable[Concatenate[S, P], T]:
-    """
-    Decorator to cache the output of a method call with variable arguments.
-
-    This requires that the class has a `self._cache` dict which can be used to store
-    the cached result. The dictionary key is derived from the name of the decorated
-    function.
-
-    The results cached by this decorator can be cleared using `self._cache.clear()`, so
-    this is useful for results which need to be invalidated (i.e. backplane images
-    which are invalidated the moment the disc params are changed). If the result is
-    stable (i.e. backplane maps) then use `_cache_stable_result` instead.
-
-    Note that any numpy arguments will be converted to (nested) tuples.
-    """
-
-    @functools.wraps(fn)
-    def decorated(self, *args_in: P.args, **kwargs_in: P.kwargs):
-        args, kwargs = _replace_np_arrr_args_with_tuples(args_in, kwargs_in)
-        k = (fn.__name__, args, frozenset(kwargs.items()))
-        if k not in self._cache:
-            self._cache[k] = fn(self, *args, **kwargs)  # type: ignore
-        return self._cache[k]
-
-    return decorated
-
-
-def _cache_stable_result(
-    fn: Callable[Concatenate[S, P], T]
-) -> Callable[Concatenate[S, P], T]:
-    """
-    Decorator to cache stable result
-
-    Very roughly, this is a type-hinted version of `functools.lru_cache` that doesn't
-    cache self.
-
-    See _cache_clearable_result for more details.
-    """
-
-    @functools.wraps(fn)
-    def decorated(self, *args_in: P.args, **kwargs_in: P.kwargs):
-        args, kwargs = _replace_np_arrr_args_with_tuples(args_in, kwargs_in)
-        k = (fn.__name__, args, frozenset(kwargs.items()))
-        if k not in self._stable_cache:
-            self._stable_cache[k] = fn(self, *args, **kwargs)  # type: ignore
-        return self._stable_cache[k]
-
-    return decorated
-
-
-def _replace_np_arrr_args_with_tuples(args, kwargs) -> tuple[tuple, dict[str, Any]]:
-    args = tuple(_maybe_np_arr_to_tuple(a) for a in args)
-    kwargs = {k: _maybe_np_arr_to_tuple(v) for k, v in kwargs.items()}
-    return args, kwargs
-
-
-def _maybe_np_arr_to_tuple(o: Any) -> Any:
-    if isinstance(o, np.ndarray):
-        return _to_tuple(o)
-    return o
-
-
-def _to_tuple(arr: np.ndarray):
-    if arr.ndim > 1:
-        return tuple(_to_tuple(a) for a in arr)
-    elif arr.ndim == 1:
-        return tuple(arr)
-    elif arr.ndim == 0:
-        return float(arr)
-    else:
-        raise ValueError(f'Error converting arr {arr!r} to tuple')
-
 
 class _MapKwargs(TypedDict, total=False):
     projection: str
     degree_interval: float
     lon: float
     lat: float
     size: int
@@ -222,14 +139,18 @@
     If `nx` and `ny` are equal (i.e. the image is square), then the parameter `sz` can
     be used instead to set both `nx` and `ny`, where `BodyXY(..., sz=50)` is equivalent
     to `BodyXY(..., nx=50, ny=50)`.
 
     If `nx` and `ny` are not set, then some functionality (such as generating backplane
     images) will not be available and will raise a `ValueError` if called.
 
+    :class:`BodyXY` instances are mutable and therefore not hashable, meaning that they
+    cannot be used as dictionary keys. :func:`to_body` can be used to create a
+    :class:`Body` instance which is hashable.
+
     Args:
         target: Name of target body, passed to :class:`Body`.
         utc: Time of observation, passed to :class:`Body`.
         observer: Name of observing body, passed to :class:`Body`.
         nx: Number of pixels in the x dimension of the image.
         ny: Number of pixels in the y dimension of the image.
         sz: Convenience parameter to set both `nx` and `ny` to the same value.
@@ -304,17 +225,14 @@
         produce a different image.
 
         This dictionary is used to define the backplanes saved to the output FITS file
         in :func:`Observation.save`.
         """
 
         # Run setup
-        self._cache = {}
-        self._stable_cache = {}
-
         self._nx: int = nx
         self._ny: int = ny
 
         self._x0: float = 0
         self._y0: float = 0
         self._r0: float = 10
         self._rotation_radians: float = 0
@@ -330,35 +248,76 @@
         self._mpl_transform_radec2xy_radians: matplotlib.transforms.Affine2D | None = (
             None
         )
 
         self.backplanes = {}
         self._register_default_backplanes()
 
+    @classmethod
+    def from_body(
+        cls, body: Body, nx: int = 0, ny: int = 0, *, sz: int | None = None
+    ) -> Self:
+        """
+        Create a :class:`BodyXY` instance with the same parameters as a :class:`Body`
+        instance.
+
+        Args:
+            body: :class:`Body` instance to convert.
+            nx: Number of pixels in the x dimension of the image.
+            ny: Number of pixels in the y dimension of the image.
+            sz: Convenience parameter to set both `nx` and `ny` to the same value.
+
+        Returns:
+            :class:`BodyXY` instance with the same parameters as the input :class:`Body`
+            instance and the specified image dimensions.
+        """
+        # pylint: disable=protected-access
+        new = cls(**body._get_kwargs(), nx=nx, ny=ny, sz=sz)
+        body._copy_options_to_other(new)
+        return new
+
+    def to_body(self) -> Body:
+        """
+        Create a :class:`Body` instance from a :class:`BodyXY` instance.
+
+        Returns:
+            :class:`Body` instance with the same parameters as the input :class:`BodyXY`
+            instance.
+        """
+        new = Body(**Body._get_kwargs(self))
+        Body._copy_options_to_other(self, new)
+        return new
+
     def __repr__(self) -> str:
         return f'BodyXY({self.target!r}, {self.utc!r}, {self._nx!r}, {self._ny!r}, observer={self.observer!r})'
 
+    __hash__ = None  # type: ignore
+
     def _get_equality_tuple(self) -> tuple:
         return (
             self._nx,
             self._ny,
             self._x0,
             self._y0,
             self._r0,
             self._rotation_radians,
             super()._get_equality_tuple(),
         )
 
-    # Cache management
-    def _clear_cache(self):
-        """
-        Clear cached results from `_cache_result`.
-        """
-        # TODO document cache clearing (incl stable cache)
-        self._cache.clear()
+    def _get_kwargs(self) -> dict[str, Any]:
+        return super()._get_kwargs() | dict(
+            nx=self._nx,
+            ny=self._ny,
+        )
+
+    def _copy_options_to_other(self, other: Self) -> None:
+        super()._copy_options_to_other(other)
+        other.set_img_size(*self.get_img_size())
+        other.set_disc_params(*self.get_disc_params())
+        other.set_disc_method(self.get_disc_method())
 
     # Coordinate transformations
     @_cache_clearable_result
     def _get_xy2radec_matrix_radians(self) -> np.ndarray:
         r_km = self.r_eq
         r_radians = np.arcsin(r_km / self.target_distance)
         s = r_radians / self.get_r0()
@@ -761,14 +720,72 @@
         """
         dra = dra_arcsec / 3600
         ddec = ddec_arcsec / 3600
         ra0, dec0 = self.xy2radec(0, 0)
         dx, dy = self.radec2xy(ra0 + dra, dec0 + ddec)
         self.adjust_disc_params(dx=dx, dy=dy)
 
+    # Limit getters
+    def _get_xy_corner_coordinates(self) -> list[tuple[float, float]]:
+        return [
+            (-0.5, -0.5),
+            (-0.5, self._ny - 0.5),
+            (self._nx - 0.5, -0.5),
+            (self._nx - 0.5, self._ny - 0.5),
+        ]
+
+    def _get_img_limits(
+        self, func: Callable[[float, float], tuple[float, float]]
+    ) -> tuple[tuple[float, float], tuple[float, float]]:
+        xy_lim = [func(x, y) for x, y in self._get_xy_corner_coordinates()]
+        xlim = (min(x for x, _ in xy_lim), max(x for x, _ in xy_lim))
+        ylim = (min(y for _, y in xy_lim), max(y for _, y in xy_lim))
+        return xlim, ylim
+
+    def get_img_limits_radec(self) -> tuple[tuple[float, float], tuple[float, float]]:
+        """
+        Get the limits of the image coordinates in the RA/Dec coordinate system.
+
+        This can be used to set the axis limits of a plot, for example: ::
+
+            xlim, ylim = obs.get_img_limits_radec()
+            plt.xlim(*xlim)
+            plt.ylim(*ylim)
+
+        See also :func:`get_img_limits_km` and :func:`get_img_limits_xy`.
+
+        Returns:
+            `(ra_left, ra_right), (dec_min, dec_max)` tuple containing the minimum and
+            maximum RA and Dec coordinates of the pixels in the image respectively.
+        """
+        xlim, ylim = self._get_img_limits(self.xy2radec)
+        return xlim[::-1], ylim  # flip xlim because RA increases to the left
+
+    def get_img_limits_km(self) -> tuple[tuple[float, float], tuple[float, float]]:
+        """
+        Get the limits of the image coordinates in the target centred plane. See
+        :func:`get_img_limits_radec` for more details.
+
+        Returns:
+            `(km_x_min, km_x_max), (km_y_min, km_y_max)` tuple containing the minimum
+            and maximum target plane distance coordinates of the pixels in the image.
+        """
+        return self._get_img_limits(self.xy2km)
+
+    def get_img_limits_xy(self) -> tuple[tuple[float, float], tuple[float, float]]:
+        """
+        Get the limits of the image coordinates. See :func:`get_img_limits_radec` for
+        more details.
+
+        Returns:
+            `(x_min, x_max), (y_min, y_max)` tuple containing the minimum and maximum
+            pixel coordinates of the pixels in the image.
+        """
+        return self._get_img_limits(lambda x, y: (x, y))
+
     # Illumination functions etc.
     def limb_xy(self, **kwargs) -> tuple[np.ndarray, np.ndarray]:
         """
         Pixel coordinate version of :func:`Body.limb_radec`.
 
         Args:
             **kwargs: Passed to :func:`Body.limb_radec`.
@@ -1264,14 +1281,15 @@
         Returns:
             Handle returned by Matplotlib's `pcolormesh`.
         """
         if ax is None:
             fig, ax = plt.subplots()
 
         map_kwargs = {}
+        # pylint: disable-next=no-member
         for k in set(_MapKwargs.__optional_keys__) | set(_MapKwargs.__required_keys__):
             if k in kwargs:
                 map_kwargs[k] = kwargs.pop(k)
 
         _, _, xx, yy, _, _ = self.generate_map_coordinates(**map_kwargs)
         h = ax.pcolormesh(xx, yy, map_img, **kwargs)
         self.plot_map_wireframe(ax=ax, **(wireframe_kwargs or {}), **map_kwargs)
@@ -1454,17 +1472,17 @@
                 add_axis_labels=False,
                 add_title=False,
                 **(plot_kwargs or {}) | dict(common_formatting=dict(color='k')),
                 **map_kwargs,
             )
             # Add dx/dy to the limits to ensure the wireframe covers all of each pixel
             # as the xx and yy coordinates only give the centre of each pixel
-            dx = abs(xx[0][1] - xx[0][0])/2
+            dx = abs(xx[0][1] - xx[0][0]) / 2
             ax.set_xlim(np.nanmin(xx) - dx, np.nanmax(xx) + dx)
-            dy = abs(yy[1][0] - yy[0][0])/2
+            dy = abs(yy[1][0] - yy[0][0]) / 2
             ax.set_ylim(np.nanmin(yy) - dy, np.nanmax(yy) + dy)
 
         return self._get_wireframe_overlay(
             output_size=output_size, dpi=dpi, nx=nx, ny=ny, rgba=rgba, plot_fn=plot_fn
         )
 
     # Backplane management
@@ -1550,21 +1568,21 @@
 
         Raises:
             BackplaneNotFoundError: if `name` is not registered as a backplane.
         """
         name = self.standardise_backplane_name(name)
         try:
             return self.backplanes[name]
-        except:
+        except KeyError as exc:
             raise BackplaneNotFoundError(
                 '{n!r} not found. Currently registered backplanes are: {r}.'.format(
                     n=name,
                     r=', '.join([repr(n) for n in self.backplanes.keys()]),
                 )
-            )
+            ) from exc
 
     def get_backplane_img(self, name: str) -> np.ndarray:
         """
         Generate backplane image.
 
         Note that a generated backplane image will depend on the disc parameters
         `(x0, y0, r0, rotation)` at the time this function is called. Generating the
@@ -2795,14 +2813,15 @@
 
 class BackplaneNotFoundError(Exception):
     pass
 
 
 def _make_backplane_documentation_str() -> str:
     class _BodyXY_ForDocumentation(BodyXY):
+        # pylint: disable-next=super-init-not-called
         def __init__(self):
             self.backplanes = {}
             self.positive_longitude_direction = 'W'
             self._register_default_backplanes()
 
     body = _BodyXY_ForDocumentation()
```

### Comparing `planetmapper-1.7.0/planetmapper/data/rings.json` & `planetmapper-1.7.1/planetmapper/data/rings.json`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.0/planetmapper/gui.py` & `planetmapper-1.7.1/planetmapper/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,75 +1,71 @@
+# pylint: disable=attribute-defined-outside-init,protected-access
 import math
 import os
 import tkinter as tk
 import tkinter.colorchooser
 import tkinter.filedialog
 import tkinter.messagebox
 import tkinter.scrolledtext
 import traceback
 from collections import defaultdict
 from tkinter import ttk
 from typing import Any, Callable, Literal, TypeVar
-from functools import lru_cache
 
+import matplotlib as mpl
 import matplotlib.cm
 import matplotlib.colors
 import matplotlib.markers
 import matplotlib.patheffects as path_effects
 import matplotlib.pyplot as plt
 import numpy as np
 import spiceypy as spice
 from astropy.io import fits
 from matplotlib.artist import Artist
+from matplotlib.backend_bases import MouseButton, MouseEvent
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg, NavigationToolbar2Tk
-from matplotlib.backend_bases import MouseEvent, MouseButton
 from matplotlib.text import Text
-import matplotlib as mpl
 
-from matplotlib.backends._backend_tk import NavigationToolbar2Tk  # TODO delete this?
-
-from . import base, common, data_loader, utils
-from .body import Body, BasicBody, NotFoundError
+from . import base, common, data_loader, progress, utils
+from .body import BasicBody, Body, NotFoundError
 from .body_xy import _MapKwargs
 from .observation import Observation
-from . import progress
-
 
 Widget = TypeVar('Widget', bound=tk.Widget)
-SETTER_KEY = Literal[
+SetterKey = Literal[
     'x0', 'y0', 'r0', 'rotation', 'step', 'plate_scale_arcsec', 'plate_scale_km'
 ]
-PLOT_KEY = Literal[
+PlotKey = Literal[
     'image',
+    'grid',
     'limb',
-    'limb_dayside',
+    'limb_illuminated',
     'terminator',
-    'grid',
-    'rings',
-    'poles',
-    'coordinates_lonlat',
-    'coordinates_radec',
-    'other_bodies',
-    'other_bodies_labels',
+    'ring',
+    'pole',
+    'coordinate_of_interest_lonlat',
+    'coordinate_of_interest_radec',
+    'other_body_of_interest_marker',
+    'other_body_of_interest_label',
     'marked_coord',
     '_',
 ]
-IMAGE_MODE = Literal['sum', 'single', 'rgb']
+ImageMode = Literal['sum', 'single', 'rgb']
 
-DEFAULT_PLOT_SETTINGS: dict[PLOT_KEY, dict] = {
+DEFAULT_PLOT_SETTINGS: dict[PlotKey, dict] = {
     'grid': dict(zorder=3.1, color='#333', linewidth=1, linestyle='dotted'),
     'terminator': dict(zorder=3.2, color='w', linewidth=1, linestyle='dashed'),
     'limb': dict(zorder=3.3, color='w', linewidth=0.5, linestyle='solid'),
-    'limb_dayside': dict(zorder=3.31, color='w', linewidth=1, linestyle='solid'),
-    'rings': dict(zorder=3.4, color='w', linewidth=0.5, linestyle='solid'),
-    'poles': dict(zorder=3.5, color='k', outline_color='w'),
-    'coordinates_lonlat': dict(zorder=3.6, marker='x', color='k', s=36),
-    'coordinates_radec': dict(zorder=3.7, marker='+', color='k', s=36),
-    'other_bodies': dict(zorder=3.8, marker='+', color='w', s=36),
-    'other_bodies_labels': dict(zorder=3.81, color='grey'),
+    'limb_illuminated': dict(zorder=3.31, color='w', linewidth=1, linestyle='solid'),
+    'ring': dict(zorder=3.4, color='w', linewidth=0.5, linestyle='solid'),
+    'pole': dict(zorder=3.5, color='k', outline_color='w'),
+    'coordinate_of_interest_lonlat': dict(zorder=3.6, marker='x', color='k', s=36),
+    'coordinate_of_interest_radec': dict(zorder=3.7, marker='+', color='k', s=36),
+    'other_body_of_interest_marker': dict(zorder=3.8, marker='+', color='w', s=36),
+    'other_body_of_interest_label': dict(zorder=3.81, color='grey'),
     'marked_coord': dict(zorder=4, color='cyan', linewidth=0.5, linestyle='dotted'),
     'image': dict(zorder=0.9, cmap='inferno'),
     '_': dict(
         grid_interval=30,
         image_mode='single',
         image_idx_single=0,
         image_idx_r=0,
@@ -79,19 +75,19 @@
         image_vmin=0,
         image_vmax=100,
         image_limit_type='absolute',
     ),
 }
 
 
-LINESTYLES = ['solid', 'dashed', 'dotted', 'dashdot']
-MARKERS = ['x', '+', 'o', '.', '*', 'v', '^', '<', '>', ',', 'D', 'd', '|', '_']
-GRID_INTERVALS = ['10', '30', '45', '90']
-CMAPS = ['gray', 'viridis', 'plasma', 'inferno', 'magma', 'cividis']
-LIMIT_TYPES = ['absolute', 'percentile']
+LINESTYLES = ('solid', 'dashed', 'dotted', 'dashdot')
+MARKERS = ('x', '+', 'o', '.', '*', 'v', '^', '<', '>', ',', 'D', 'd', '|', '_')
+GRID_INTERVALS = ('10', '30', '45', '90')
+CMAPS = ('gray', 'viridis', 'plasma', 'inferno', 'magma', 'cividis')
+LIMIT_TYPES = ('absolute', 'percentile')
 
 MAP_INTERPOLATIONS = ('nearest', 'linear', 'quadratic', 'cubic')
 MAP_PROJECTIONS = ('rectangular', 'orthographic', 'azimuthal')
 
 DEFAULT_HINT = ''
 
 
@@ -100,15 +96,15 @@
 # XQuartz was producing when trying to run planetmapper over SSH on mac. This is a bit
 # of a hack and produces an uglier UI, but is better than always crashing.
 # TODO remove this when the bug is fixed in XQuartz
 # https://github.com/ortk95/planetmapper/issues/145
 try:
     USE_X11_FONT_BUGFIX = bool(os.environ['PLANETMAPPER_USE_X11_FONT_BUGFIX'])
 except KeyError:
-    USE_X11_FONT_BUGFIX = False
+    USE_X11_FONT_BUGFIX = False  # pyright: ignore[reportConstantRedefinition]
 X11_FONT_BUGRIX_TRANSLATIONS = str.maketrans(
     {
         '↖': None,
         '↑': '^',
         '↗': None,
         '←': '<',
         '→': '>',
@@ -180,46 +176,46 @@
             self.save_button: ['<Control-s>'],
             self.load_observation: ['<Control-o>'],
             self.copy_machine_coord_values: ['<Control-c>'],
         }
         self.shortcuts_to_keep_in_entry = ['<Control-s>', '<Control-o>']
 
         self.setter_callbacks: defaultdict[
-            SETTER_KEY, list[Callable[[float], Any]]
+            SetterKey, list[Callable[[float], Any]]
         ] = defaultdict(
             list,
             {
                 'x0': [lambda f: self.get_observation().set_x0(f)],
                 'y0': [lambda f: self.get_observation().set_y0(f)],
                 'r0': [lambda f: self.get_observation().set_r0(f)],
                 'rotation': [lambda f: self.get_observation().set_rotation(f)],
-                'step': [lambda f: self.set_step(f)],
+                'step': [self.set_step],
                 'plate_scale_arcsec': [
                     lambda f: self.get_observation().set_plate_scale_arcsec(f)
                 ],
                 'plate_scale_km': [
                     lambda f: self.get_observation().set_plate_scale_km(f)
                 ],
             },
         )
         self.ui_callbacks: defaultdict[
-            SETTER_KEY | None, set[Callable[[], Any]]
+            SetterKey | None, set[Callable[[], Any]]
         ] = defaultdict(set)
 
-        self.getters: dict[SETTER_KEY, Callable[[], float]] = {
+        self.getters: dict[SetterKey, Callable[[], float]] = {
             'x0': lambda: self.get_observation().get_x0(),
             'y0': lambda: self.get_observation().get_y0(),
             'r0': lambda: self.get_observation().get_r0(),
             'rotation': lambda: self.get_observation().get_rotation(),
             'step': lambda: self.step_size,
             'plate_scale_arcsec': lambda: self.get_observation().get_plate_scale_arcsec(),
             'plate_scale_km': lambda: self.get_observation().get_plate_scale_km(),
         }
-        self.plot_handles: defaultdict[PLOT_KEY, list[Artist]] = defaultdict(list)
-        self.plot_settings: defaultdict[PLOT_KEY, dict] = defaultdict(dict)
+        self.plot_handles: defaultdict[PlotKey, list[Artist]] = defaultdict(list)
+        self.plot_settings: defaultdict[PlotKey, dict] = defaultdict(dict)
         for k, v in DEFAULT_PLOT_SETTINGS.items():
             self.plot_settings[k] = v.copy()
 
         self.disc_finding_routines: dict[
             str, list[tuple[Callable[[], None], str, str]]
         ] = {
             'Reset position': [
@@ -279,15 +275,15 @@
 
         self.delayed_actions: dict[str, tuple[Callable[[], Any], str]] = {}
 
         self.event_time_to_ignore = None
         self.gui_built = False
 
     def __repr__(self) -> str:
-        return f'InteractiveObservation()'
+        return 'InteractiveObservation()'
 
     def run(self) -> None:
         """
         Run the GUI.
         """
         print('Running user interface...')
         try:
@@ -322,15 +318,15 @@
             gui.run()
 
         Args:
             observation: Observation to fit.
         """
         self._observation = observation
 
-        self.image_modes: dict[IMAGE_MODE, tuple[Callable[[], np.ndarray], str]] = {
+        self.image_modes: dict[ImageMode, tuple[Callable[[], np.ndarray], str]] = {
             'single': (self.image_single, 'Single wavelength'),
             'sum': (self.image_sum, 'Sum all wavelengths'),
             'rgb': (self.image_rgb, 'RGB composite'),
         }
         n_wavl = self.get_observation().data.shape[0]
         if n_wavl < 2:
             del self.image_modes['sum']
@@ -517,18 +513,18 @@
     def build_main_controls_section(
         self,
         frame: ttk.Frame,
         label: str,
         buttons: list[tuple[str, str, Callable[[], None], int, int]],
         button_tooltip_base: str,
         entry_tooltip: str,
-        numeric_entries: list[SETTER_KEY | tuple[SETTER_KEY, str]],
+        numeric_entries: list[SetterKey | tuple[SetterKey, str]],
         ipadx=30,
         ipady=1,
-        add_callbacks: list[SETTER_KEY] | None = None,
+        add_callbacks: list[SetterKey] | None = None,
         **kw,
     ) -> None:
         label_frame = ttk.LabelFrame(frame, text=label)
         label_frame.pack(fill='x', pady=3, ipadx=1, ipady=1)
 
         button_frame = ttk.Frame(label_frame)
         button_frame.pack()
@@ -581,15 +577,15 @@
         frame = ttk.LabelFrame(menu, text='Plotted features')
         frame.pack(fill='x', pady=5)
         frame.grid_columnconfigure(0, weight=1)
         PlotLineSetting(self, frame, 'limb', label='Limb', hint='the target\'s limb')
         PlotLineSetting(
             self,
             frame,
-            'limb_dayside',
+            'limb_illuminated',
             label='Limb (dayside)',
             hint='the illuminated part of the target\'s limb',
         )
         PlotLineSetting(
             self,
             frame,
             'terminator',
@@ -603,30 +599,30 @@
             label='Gridlines',
             hint='the longitude/latitude grid on the target',
             callbacks=[self.replot_grid],
         )
         PlotRingsSetting(
             self,
             frame,
-            'rings',
+            'ring',
             label='Rings',
             hint='rings around the target (click Edit to define ring radii)',
             callbacks=[self.replot_rings],
         )
         PlotOutlinedTextSetting(
             self,
             frame,
-            'poles',
+            'pole',
             label='Poles',
             hint='the target\'s poles',
         )
         PlotCoordinatesSetting(
             self,
             frame,
-            'coordinates_lonlat',
+            'coordinate_of_interest_lonlat',
             label='Lon/Lat POI',
             hint='points of interest on the surface of the target (click Edit to define POI)',
             callbacks=[self.replot_coordinates_lonlat],
             coordinate_list=self.get_observation().coordinates_of_interest_lonlat,
             menu_label='\n'.join(
                 [
                     'List of Lon/Lat points of interest.',
@@ -635,15 +631,15 @@
                     'coordinate pair on a new line:',
                 ]
             ),
         )
         PlotCoordinatesSetting(
             self,
             frame,
-            'coordinates_radec',
+            'coordinate_of_interest_radec',
             label='RA/Dec POI',
             hint='points of interest in the sky (click Edit to define POI)',
             callbacks=[self.replot_coordinates_radec],
             coordinate_list=self.get_observation().coordinates_of_interest_radec,
             menu_label='\n'.join(
                 [
                     'List of RA/Dec points of interest.',
@@ -652,23 +648,23 @@
                     'coordinate pair on a new line:',
                 ]
             ),
         )
         PlotOtherBodyScatterSetting(
             self,
             frame,
-            'other_bodies',
-            label='Other bodies',
+            'other_body_of_interest_marker',
+            label='Other bodies (e.g. moons)',
             hint='other bodies of interest (click Edit to specify other bodies to show, e.g. moons)',
             callbacks=[self.replot_other_bodies],
         )
         PlotOtherBodyTextSetting(
             self,
             frame,
-            'other_bodies_labels',
+            'other_body_of_interest_label',
             label='Other body labels',
             hint='labels for other bodies of interest (click Edit to specify other bodies to show, e.g. moons)',
             callbacks=[self.replot_other_bodies],
         )
 
         # Marked coords
         frame = ttk.LabelFrame(menu, text='Marked coords')
@@ -946,16 +942,17 @@
 
     def figure_click_callback(self, event: MouseEvent) -> None:
         if not event.inaxes or event.dblclick:
             return
 
         try:
             # Disable when panning/zooming
-            if self.toolbar.mode._navigate_mode is not None:  #  type: ignore
+            if self.toolbar.mode._navigate_mode is not None:
                 return
+        # pylint: disable-next=bare-except
         except:
             pass
 
         if event.button == MouseButton.RIGHT:
             self.clear_click_location()
 
         if event.button == MouseButton.LEFT:
@@ -1076,15 +1073,15 @@
 
         mode = self.plot_settings['_'].setdefault('image_mode', 'single')
         vmin = self.plot_settings['_'].setdefault('image_vmin', 0)
         vmax = self.plot_settings['_'].setdefault('image_vmax', 1)
         limit_type = self.plot_settings['_'].setdefault('image_limit_type', 'absolute')
 
         with utils.ignore_warnings('All-NaN slice encountered'):
-            image = self.image_modes[mode][0]()  # type: ignore
+            image = self.image_modes[mode][0]()
             if limit_type == 'percentile':
                 vmin = np.nanpercentile(image, vmin)
                 vmax = np.nanpercentile(image, vmax)
 
         self.plot_handles['image'].append(
             self.ax.imshow(
                 image,
@@ -1093,64 +1090,64 @@
                 vmax=vmax,
                 **self.plot_settings['image'],
             )
         )
 
     def replot_limb(self):
         self.remove_artists('limb')
-        self.remove_artists('limb_dayside')
+        self.remove_artists('limb_illuminated')
         self.plot_handles['limb'].extend(
             self.ax.plot(
                 *self.get_observation().limb_radec(),
                 transform=self.transform,
                 **self.plot_settings['limb'],
             )
         )
         (
             ra_day,
             dec_day,
             ra_night,
             dec_night,
         ) = self.get_observation().limb_radec_by_illumination()
-        self.plot_handles['limb_dayside'].extend(
+        self.plot_handles['limb_illuminated'].extend(
             self.ax.plot(
                 ra_day,
                 dec_day,
                 transform=self.transform,
-                **self.plot_settings['limb_dayside'],
+                **self.plot_settings['limb_illuminated'],
             )
         )
 
     def replot_terminator(self):
         self.remove_artists('terminator')
         self.plot_handles['terminator'].extend(
             self.ax.plot(
                 *self.get_observation().terminator_radec(),
                 transform=self.transform,
                 **self.plot_settings['terminator'],
             )
         )
 
     def replot_poles(self):
-        self.remove_artists('poles')
+        self.remove_artists('pole')
         for lon, lat, s in self.get_observation().get_poles_to_plot():
             ra, dec = self.get_observation().lonlat2radec(lon, lat)
-            self.plot_handles['poles'].append(
+            self.plot_handles['pole'].append(
                 self.ax.add_artist(
                     OutlinedText(
                         ra,
                         dec,
                         s,
                         ha='center',
                         va='center',
                         weight='bold',
                         size='small',
                         transform=self.transform,
                         clip_on=True,
-                        **self.plot_settings['poles'],
+                        **self.plot_settings['pole'],
                     )
                 )
             )
 
     def replot_grid(self) -> None:
         self.remove_artists('grid')
         interval = self.plot_settings['_'].setdefault('grid_interval', 30)
@@ -1161,93 +1158,97 @@
                     dec,
                     transform=self.transform,
                     **self.plot_settings['grid'],
                 )
             )
 
     def replot_coordinates_lonlat(self) -> None:
-        self.remove_artists('coordinates_lonlat')
+        self.remove_artists('coordinate_of_interest_lonlat')
         for lon, lat in self.get_observation().coordinates_of_interest_lonlat:
             if self.get_observation().test_if_lonlat_visible(lon, lat):
                 ra, dec = self.get_observation().lonlat2radec(lon, lat)
-                self.plot_handles['coordinates_lonlat'].append(
+                self.plot_handles['coordinate_of_interest_lonlat'].append(
                     self.ax.scatter(
                         ra,
                         dec,
                         transform=self.transform,
-                        **self.plot_settings['coordinates_lonlat'],
+                        **self.plot_settings['coordinate_of_interest_lonlat'],
                     )
                 )
 
     def replot_coordinates_radec(self) -> None:
-        self.remove_artists('coordinates_radec')
+        self.remove_artists('coordinate_of_interest_radec')
         for ra, dec in self.get_observation().coordinates_of_interest_radec:
-            self.plot_handles['coordinates_radec'].append(
+            self.plot_handles['coordinate_of_interest_radec'].append(
                 self.ax.scatter(
                     ra,
                     dec,
                     transform=self.transform,
-                    **self.plot_settings['coordinates_radec'],
+                    **self.plot_settings['coordinate_of_interest_radec'],
                 )
             )
 
     def replot_rings(self) -> None:
-        self.remove_artists('rings')
+        self.remove_artists('ring')
         for radius in self.get_observation().ring_radii:
             ra, dec = self.get_observation().ring_radec(radius)
-            self.plot_handles['rings'].extend(
+            self.plot_handles['ring'].extend(
                 self.ax.plot(
                     ra,
                     dec,
                     transform=self.transform,
-                    **self.plot_settings['rings'],
+                    **self.plot_settings['ring'],
                 )
             )
 
     def replot_other_bodies(self) -> None:
-        self.remove_artists('other_bodies_labels')
-        self.remove_artists('other_bodies')
+        self.remove_artists('other_body_of_interest_label')
+        self.remove_artists('other_body_of_interest_marker')
         for body in self.get_observation().other_bodies_of_interest:
             ra = body.target_ra
             dec = body.target_dec
-
-            self.plot_handles['other_bodies_labels'].append(
+            label = body.target
+            hidden = not self.get_observation().test_if_other_body_visible(body)
+            if hidden:
+                label = f'({label})'
+            self.plot_handles['other_body_of_interest_label'].append(
                 self.ax.text(
                     ra,
                     dec,
-                    body.target + '\n',
+                    label + '\n',
                     size='small',
                     ha='center',
                     va='center',
                     transform=self.transform,
                     clip_on=True,
-                    **self.plot_settings['other_bodies_labels'],
+                    **self.plot_settings['other_body_of_interest_label'],
                 )
             )
-            self.plot_handles['other_bodies'].append(
+            self.plot_handles['other_body_of_interest_marker'].append(
                 self.ax.scatter(
                     ra,
                     dec,
                     transform=self.transform,
-                    **self.plot_settings['other_bodies'],
+                    alpha=0.5 if hidden else 1,
+                    **self.plot_settings['other_body_of_interest_marker'],
                 )
             )
 
     def replot_marked_coord(self) -> None:
         self.remove_artists('marked_coord')
         if self.last_click_location is not None:
             x, y = self.last_click_location
             self.plot_handles['marked_coord'].append(
                 self.ax.axvline(x, **self.plot_settings['marked_coord'])
             )
             self.plot_handles['marked_coord'].append(
                 self.ax.axhline(y, **self.plot_settings['marked_coord'])
             )
 
-    def remove_artists(self, key: PLOT_KEY) -> None:
+    def remove_artists(self, key: PlotKey) -> None:
         while self.plot_handles[key]:
             self.plot_handles[key].pop().remove()
 
     # Delayed actions
     def add_delayed_action(self, name: str, ms: int, func: Callable[[], Any]) -> None:
         self.cancel_delayed_action(name)
         self.delayed_actions[name] = (
@@ -1312,17 +1313,15 @@
         for k, callbacks in self.ui_callbacks.items():
             all_callbacks.update(callbacks)
         for fn in all_callbacks:
             fn()
         if update_plot:
             self.update_plot()
 
-    def set_value(
-        self, key: SETTER_KEY, value: float, update_plot: bool = True
-    ) -> None:
+    def set_value(self, key: SetterKey, value: float, update_plot: bool = True) -> None:
         for fn in self.setter_callbacks[key]:
             fn(value)
         for fn in self.ui_callbacks[key]:
             fn()
         if update_plot:
             self.update_plot()
 
@@ -1629,14 +1628,15 @@
 
     def path_changed(self, *_) -> None:
         path = self.stringvars['path'].get()
         kwargs = {}
         if any(path.endswith(ext) for ext in Observation.FITS_FILE_EXTENSIONS):
             try:
                 with fits.open(path) as hdul:
+                    # pylint: disable-next=no-member
                     header = hdul[0].header  # type: ignore
                 Observation._add_kw_from_header(kwargs, header)
             except FileNotFoundError:
                 pass
         for k, v in kwargs.items():
             try:
                 if v:
@@ -1670,63 +1670,67 @@
 
         string = self.kernel_txt.get('1.0', 'end')
         kernels = [k.strip() for k in string.splitlines()]
         base.load_kernels(*kernels, clear_before=True)
 
         kernel_help = 'Check for typos and make sure you have listed all the required SPICE kernels'
 
-        sb = base.SpiceBase(load_kernels=False)
+        sb = base.SpiceBase(auto_load_kernels=False)
         try:
             target = sb.standardise_body_name(kwargs['target'])
+        # pylint: disable-next=bare-except
         except:
             tkinter.messagebox.showwarning(
-                title=f'Error parsing target',
+                title='Error parsing target',
                 message='Target name {!r} not recognised\n{}'.format(
                     kwargs['target'], kernel_help
                 ),
             )
             return False
 
         try:
             observer = sb.standardise_body_name(kwargs['observer'])
+        # pylint: disable-next=bare-except
         except:
             tkinter.messagebox.showwarning(
-                title=f'Error parsing observer',
+                title='Error parsing observer',
                 message='Observer name {!r} not recognised\n{}'.format(
                     kwargs['observer'], kernel_help
                 ),
             )
             return False
 
         if target == observer:
             tkinter.messagebox.showwarning(
-                title=f'Target and observer identical',
+                title='Target and observer identical',
                 message='Target and observer must correspond to different bodies',
             )
             return False
 
         try:
             kwargs['utc'] = float(kwargs['utc'])  #  type: ignore
         except ValueError:
             try:
                 spice.utc2et(kwargs['utc'])
+            # pylint: disable-next=bare-except
             except:
                 tkinter.messagebox.showwarning(
-                    title=f'Error parsing utc',
+                    title='Error parsing utc',
                     message='Could not parse {!r}\n{}'.format(
                         kwargs['utc'], kernel_help
                     ),
                 )
                 return False
         try:
-            observation = Observation(**kwargs, load_kernels=False)
+            observation = Observation(**kwargs, auto_load_kernels=False)
+        # pylint: disable-next=broad-except
         except Exception as e:
             traceback.print_exc()
             tkinter.messagebox.showwarning(
-                title=f'Error processing inputs',
+                title='Error processing inputs',
                 message=f'Error: {e}' + '\n\nSee terminal for more details',
             )
             return False
         self.gui.set_observation(observation)
         self.gui.kernels = kernels
         return True
 
@@ -2045,16 +2049,16 @@
 
         keep_open = bool(self.keep_open.get())
 
         interpolation = 'linear'
 
         if (save_nav and len(path_nav) == 0) or (save_map and len(path_map) == 0):
             tkinter.messagebox.showwarning(
-                title=f'Error saving file',
-                message=f'File paths must not be empty',
+                title='Error saving file',
+                message='File paths must not be empty',
             )
             return False
 
         try:
             if save_map:
                 interpolation = self.map_interpolation.get()
                 map_kw['projection'] = self.map_projection.get()
@@ -2096,18 +2100,19 @@
             path_map=path_map,
             interpolation=interpolation,
             map_kw=map_kw,
             keep_open=keep_open,
         )
         try:
             saving_process.run_save()
+        # pylint: disable-next=broad-except
         except Exception as e:
             traceback.print_exc()
             tkinter.messagebox.showwarning(
-                title=f'Error saving files',
+                title='Error saving files',
                 message=f'Error: {e}' + '\n\nSee terminal for more details',
             )
             return False
         finally:
             self.gui.get_observation()._remove_progress_hook()
 
         self.gui.set_help_hint(
@@ -2224,15 +2229,15 @@
     def destroy(self) -> None:
         self.window.destroy()
         self.parent.gui.get_observation()._remove_progress_hook()
         self.parent.saving_progress_window = None
 
 
 # Progress hooks
-class SaveProgressHookGUI(progress.SaveProgressHook):
+class SaveProgressHookGUI(progress._SaveProgressHook):
     def __init__(
         self,
         label: ttk.Label,
         bar: ttk.Progressbar,
         message: ttk.Label,
         *args,
         **kwargs,
@@ -2248,38 +2253,36 @@
             self.message.configure(text='Complete')
         else:
             self.bar['value'] = self.overall_progress * 100
             self.message.configure(text=format(self.overall_progress, '.0%'))
         self.bar.update_idletasks()
 
 
-class SaveNavProgressHookGUI(progress.SaveNavProgressHook, SaveProgressHookGUI):
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
+class SaveNavProgressHookGUI(progress._SaveNavProgressHook, SaveProgressHookGUI):
+    pass
 
 
-class SaveMapProgressHookGUI(progress.SaveMapProgressHook, SaveProgressHookGUI):
-    def __init__(self, n_wavelengths: int, *args, **kwargs) -> None:
-        super().__init__(n_wavelengths, *args, **kwargs)
+class SaveMapProgressHookGUI(progress._SaveMapProgressHook, SaveProgressHookGUI):
+    pass
 
 
 # Artist settings popups
 class ArtistSetting(Popup):
     def __init__(
         self,
         gui: GUI,
         parent: tk.Widget,
-        key: PLOT_KEY,
+        key: PlotKey,
         label: str | None = None,
         hint: str | None = None,
         callbacks: list[Callable[[], None]] | None = None,
         row: int | None = None,
     ):
         self.parent = parent
-        self.key: PLOT_KEY = key
+        self.key: PlotKey = key
         self.gui = gui
         self._enable_callback = True
         if label is None:
             label = key
         self.label = label
         self.callbacks = callbacks
 
@@ -2409,15 +2412,15 @@
 class PlotImageSetting(ArtistSetting):
     REPLOT_DELAY_MS = 100
 
     def __init__(
         self,
         gui: GUI,
         parent: tk.Widget,
-        key: PLOT_KEY,
+        key: PlotKey,
         label: str | None = None,
         hint: str | None = None,
         callbacks: list[Callable[[], None]] | None = None,
         row: int | None = None,
     ):
         super().__init__(gui, parent, key, label, hint, callbacks, row)
 
@@ -2582,15 +2585,15 @@
                     from_=0,
                     to=idx_max,
                     increment=1,
                     width=10,
                 )
 
         self.grid: list[
-            tuple[tk.Widget, tk.Widget, set[IMAGE_MODE | Literal['_readonly']]]
+            tuple[tk.Widget, tk.Widget, set[ImageMode | Literal['_readonly']]]
         ] = [
             (
                 ttk.Label(frame, text='Wavelength index (single): '),
                 IndexInput(self.image_idx_single),
                 {'single'},
             ),
             (
@@ -2735,15 +2738,15 @@
                 )
                 general_settings['image_vmax'] = self.get_float(
                     self.image_vmax, 'vmax', positive=False
                 )
                 if general_settings['image_vmin'] >= general_settings['image_vmax']:
                     tkinter.messagebox.showwarning(
                         title='Error parsing limits',
-                        message=f'vmin must be less than vmax',
+                        message='vmin must be less than vmax',
                     )
                     return False
         except ValueError:
             return False
 
         if image_mode in {'single', 'sum'}:
             try:
@@ -2978,15 +2981,15 @@
 
 
 class PlotCoordinatesSetting(PlotScatterSetting):
     def __init__(
         self,
         gui: GUI,
         parent: tk.Widget,
-        key: PLOT_KEY,
+        key: PlotKey,
         coordinate_list: list[tuple[float, float]],
         menu_label: str,
         label: str | None = None,
         hint: str | None = None,
         callbacks: list[Callable[[], None]] | None = None,
         **kwargs,
     ):
@@ -3008,15 +3011,15 @@
             string = self.txt.get('1.0', 'end')
             for line in string.splitlines():
                 line = line.strip().lstrip('(').rstrip(')')
                 if line:
                     coordinates = line.split(',')
                     if len(coordinates) != 2:
                         tkinter.messagebox.showwarning(
-                            title=f'Error parsing coordinates',
+                            title='Error parsing coordinates',
                             message=f'Line {line!r} must have exactly two values separated by a comma',
                         )
                         return False
                     values.append(
                         tuple(
                             self.get_float(c, 'coordinate', positive=False)
                             for c in coordinates
@@ -3077,47 +3080,80 @@
     def apply_settings(self) -> bool:
         settings = self.gui.plot_settings[self.key]
         settings['color'] = self.color.get()
         settings['outline_color'] = self.outline_color.get()
         return True
 
 
+# pylint: disable-next=abstract-method
 class GenericOtherBodySetting(ArtistSetting):
     def add_other_body_menu_setting(self):
-        value = '\n'.join(
-            b.target for b in self.gui.get_observation().other_bodies_of_interest
-        )
         label = '\n'.join(
             [
                 'List other bodies of interest to',
                 'mark (e.g. moons). Body names should',
                 'be recognisable by SPICE (e.g "Europa"',
                 'or "502") with each body listed on a',
                 'new line:',
             ]
         )
         ttk.Label(self.menu_frame, text='\n' + label).pack(fill='x')
         self.txt = tkinter.scrolledtext.ScrolledText(self.menu_frame)
         self.txt.pack(fill='both')
+
+        self.button_frame = ttk.Frame(self.menu_frame)
+        self.button_frame.pack(fill='x', pady=3)
+        self.add_satellites_button = ttk.Button(
+            self.button_frame,
+            text='Add all visible satellites in target system',
+            command=self.add_satellites,
+        )
+        self.add_satellites_button.pack()
+
+        self.populate_text_box()
+
+    def populate_text_box(
+        self, bodies: list[Body | BasicBody] | None = None, append: bool = False
+    ) -> None:
+        if bodies is None:
+            bodies = self.gui.get_observation().other_bodies_of_interest
+        bodies = sorted((b for b in bodies), key=lambda b: b.target_body_id)
+
+        if append:
+            lines = [l for l in self.txt.get('1.0', 'end').splitlines() if l.strip()]
+        else:
+            lines = []
+
+        for b in bodies:
+            line = b.target
+            if line not in lines:
+                lines.append(line)
+        value = '\n'.join(lines)
+        self.txt.delete('1.0', 'end')
         self.txt.insert('1.0', value)
 
+    def add_satellites(self) -> None:
+        bodies = self.gui.get_observation()._get_all_satellite_bodies(
+            skip_insufficient_data=True, only_visible=True
+        )
+        self.populate_text_box(bodies, append=True)
+
     def apply_other_body_setting(self) -> bool:
         bodies: list[Body | BasicBody] = []
         string = self.txt.get('1.0', 'end')
-        for line in string.splitlines():
-            line = line.strip()
-            if line:
-                try:
-                    bodies.append(self.gui.get_observation().create_other_body(line))
-                except NotFoundError:
-                    tkinter.messagebox.showwarning(
-                        title=f'Error parsing target name',
-                        message=f'Target {line!r} is not recognised by SPICE',
-                    )
-                    return False
+        lines = [l for line in string.splitlines() if (l := line.strip())]
+        for line in set(lines):
+            try:
+                bodies.append(self.gui.get_observation().create_other_body(line))
+            except NotFoundError:
+                tkinter.messagebox.showwarning(
+                    title='Error parsing target name',
+                    message=f'Target {line!r} is not recognised by SPICE',
+                )
+                return False
         self.gui.get_observation().other_bodies_of_interest.clear()
         self.gui.get_observation().other_bodies_of_interest[:] = bodies
         return True
 
     def get_window_size(self) -> str:
         return '350x600'
 
@@ -3168,22 +3204,22 @@
 
 
 class NumericEntry:
     def __init__(
         self,
         gui: GUI,
         parent: tk.Widget,
-        key: SETTER_KEY,
+        key: SetterKey,
         label: str | None = None,
         row: int | None = None,
-        add_callbacks: list[SETTER_KEY] | None = None,
+        add_callbacks: list[SetterKey] | None = None,
         **kw,
     ):
         self.parent = parent
-        self.key: SETTER_KEY = key
+        self.key: SetterKey = key
         self.gui = gui
         self._enable_callback = True
 
         if label is None:
             label = key
         self.label = ttk.Label(parent, text=label + ': ')
 
@@ -3272,20 +3308,22 @@
             ('Pan', None, 'move', 'pan'),
             ('Zoom', None, 'zoom_to_rect', 'zoom'),
             (None, None, None, None),
             ('Save', None, 'filesave', 'save_figure'),
         )
         super().__init__(canvas, window, pack_toolbar=pack_toolbar)
         try:
-            self._message_label.configure(foreground='#666666')  # type: ignore
+            self._message_label.configure(foreground='#666666')
+        # pylint: disable-next=bare-except
         except:
             pass
         try:
-            for name, button in self._buttons.items():  # type: ignore
+            for name, button in self._buttons.items():
                 # Get default tooltips from super() and use them
                 for text, tooltip_text, image_file, callback in super().toolitems:
                     if text == name:
                         hint = tooltip_text.replace('\n', ', ')
                         gui.add_tooltip(button, hint)
                         break
+        # pylint: disable-next=bare-except
         except:
             pass
```

### Comparing `planetmapper-1.7.0/planetmapper/kernel_downloader.py` & `planetmapper-1.7.1/planetmapper/kernel_downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     """
     kp = _get_kernel_path(url)
     print(f'{note}Checking {kp}')
     if _check_kernel_exists_locally(url):
         if force_download:
             print('  Kernel already exists, downloading anyway')
         else:
-            print('  ✅ Kernel already exists locally')
+            print('  OK - Kernel already exists locally')
             return
     local_path = _convert_url_to_local_path(url)
     print(f'  Downloading to {local_path}')
     download_file(url, local_path)
     print('    Done')
 
 
@@ -118,14 +118,15 @@
 
     Args:
         index_url: URL of webpage.
 
     Returns:
         List of URL strings corresponding to kernels on the webpage.
     """
+    # pylint: disable=consider-using-with
     assert index_url.startswith(URL_ROOT), f'URL must begin with {URL_ROOT}'
     webpage = urllib.request.urlopen(index_url).read().decode()
     data = webpage.split('<!--start data_content-->')[1].split('</table>')[0]
     lines = data.splitlines()  # get lines from table
     paths = []
     for l in lines:
         if not l.startswith('<img src="/icons/'):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `planetmapper-1.7.0/planetmapper/observation.py` & `planetmapper-1.7.1/planetmapper/observation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import datetime
 import os
 import warnings
-from typing import ParamSpec, TypeVar, Callable, Any, Literal
+from typing import Any, Callable, Literal, ParamSpec, TypeVar
 
 import astropy.wcs
 import numpy as np
 import photutils.aperture
 import PIL.Image
 import scipy.ndimage
 from astropy.io import fits
 from astropy.utils.exceptions import AstropyWarning
 
 from . import common, utils
-from .body_xy import BodyXY, _MapKwargs, Unpack, _cache_clearable_result
-from .progress import progress_decorator, SaveMapProgressHookCLI, SaveNavProgressHookCLI
+from .base import _cache_clearable_result
+from .body_xy import BodyXY, Unpack, _MapKwargs
+from .progress import SaveMapProgressHookCLI, SaveNavProgressHookCLI, progress_decorator
 
 T = TypeVar('T')
 S = TypeVar('S')
 P = ParamSpec('P')
 
 
 class Observation(BodyXY):
@@ -83,14 +84,18 @@
         self,
         path: str | None = None,
         *,
         data: np.ndarray | None = None,
         header: fits.Header | None = None,
         **kwargs,
     ) -> None:
+        self._path_arg = path
+        self._data_arg = data
+        self._header_arg = header
+
         # Add docstrings
         self.data: np.ndarray
         """Observed data."""
         self.header: fits.Header
         """
         FITS header containing data about the observation. If this is not provided, then
         a basic header will be produced containing data derived from the `target` and 
@@ -144,35 +149,51 @@
             except ValueError:
                 self.centre_disc()
 
     def __repr__(self) -> str:
         return f'Observation({self.path!r})'
 
     def _get_equality_tuple(self) -> tuple:
+        # Use nan_to_num to convert NaNs to zeros, so that NaNs in the data don't
+        # cause the equality check to fail. Then use isnan to compare the NaN masks
+        # to ensure e.g. [1, NaN] != [1, 0]. Compare .data to get booleans rather
+        # than numpy's array of booleans.
         return (
             self.path,
-            self.data.data,
+            np.nan_to_num(self.data).data,
+            np.isnan(self.data).data,
             self.header,
             super()._get_equality_tuple(),
         )
 
+    def _get_kwargs(self) -> dict[str, Any]:
+        kw = super()._get_kwargs() | dict(
+            path=self._path_arg,
+            data=self._data_arg,
+            header=self._header_arg,
+        )
+        kw.pop('nx')
+        kw.pop('ny')
+        return kw
+
     def _load_data_from_path(self):
         assert self.path is not None
         if any(self.path.endswith(ext) for ext in self.FITS_FILE_EXTENSIONS):
             self._load_fits_data()
         else:
             self._load_image_data()
 
     def _load_fits_data(self):
         assert self.path is not None
         with fits.open(self.path, memmap=False) as hdul:
             for idx, hdu in enumerate(hdul):
                 if hdu.data is not None:
                     data = hdu.data
                     if idx:
+                        # pylint: disable-next=no-member
                         header = hdul[0].header.copy()  # type: ignore
                         header.update(hdu.header.copy())
                     else:
                         header = hdu.header.copy()
                     break
             else:
                 raise ValueError('No data found in provided FITS file')
@@ -227,19 +248,19 @@
                 # If the header has a MJD value for the start and end of the
                 # observation, average them and use astropy to convert this
                 # mid-observation MJD into a fits format time string
                 beg = float(header['MJD-BEG'])  #  type: ignore
                 end = float(header['MJD-END'])  #  type: ignore
                 mjd = (beg + end) / 2
                 kw['utc'] = mjd
-            except:
+            except (KeyError, TypeError, ValueError):
                 pass
             if 'utc' not in kw:
                 try:
-                    kw['utc'] = header['DATE-OBS'] + ' ' + header['TIME-OBS']
+                    kw['utc'] = header['DATE-OBS'] + ' ' + header['TIME-OBS']  # type: ignore
                 except KeyError:
                     pass
             _try_get_header_value(
                 kw,
                 header,
                 'utc',
                 ['DATE-OBS', 'DATE-BEG', 'DATE-END', 'MJD-BEG', 'MJD-END'],
@@ -282,16 +303,16 @@
         try:
             self.set_disc_params(
                 x0=self.header[self._make_fits_kw('DISC X0')],  # type: ignore
                 y0=self.header[self._make_fits_kw('DISC Y0')],  # type: ignore
                 r0=self.header[self._make_fits_kw('DISC R0')],  # type: ignore
                 rotation=self.header[self._make_fits_kw('DISC ROT')],  # type: ignore
             )
-        except KeyError:
-            raise ValueError('No disc parameters found in FITS header')
+        except KeyError as exc:
+            raise ValueError('No disc parameters found in FITS header') from exc
 
     def _get_wcs_from_header(self, suppress_warnings: bool = False) -> astropy.wcs.WCS:
         with warnings.catch_warnings():
             if suppress_warnings:
                 warnings.simplefilter('ignore', category=AstropyWarning)
             return astropy.wcs.WCS(self.header).celestial
 
@@ -1156,14 +1177,15 @@
             `planetmapper` from the command line or create and run a user interface
             manually using :func:`planetmapper.gui.GUI.run`.
 
         Returns:
             List of `(x, y)` pixel coordinate tuples corresponding to where the user
             clicked on the plot window to mark a location.
         """
+        # pylint: disable=cyclic-import
         from .gui import GUI  # Prevent circular imports
 
         gui = GUI(allow_open=False)
         gui.set_observation(self)
         gui.run()
         return gui.click_locations
```

### Comparing `planetmapper-1.7.0/planetmapper/progress.py` & `planetmapper-1.7.1/planetmapper/progress.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
+import time
 from functools import wraps
-from typing import TypeVar, ParamSpec, Concatenate, Callable, TYPE_CHECKING
+from typing import TYPE_CHECKING, Callable, Concatenate, ParamSpec, TypeVar
+
 import tqdm
-import time
-import numpy as np
-import warnings
+
 if TYPE_CHECKING:
     from .base import SpiceBase
 
 T = TypeVar('T')
 S = TypeVar('S')
 P = ParamSpec('P')
 
 
 def progress_decorator(
     fn: Callable[Concatenate[S, P], T]
 ) -> Callable[Concatenate[S, P], T]:
+    # pylint: disable=protected-access
     @wraps(fn)
     def decorated(self: 'SpiceBase', *args: P.args, **kwargs: P.kwargs):
         if self._progress_hook is None:
             return fn(self, *args, **kwargs)  # type: ignore
         else:
             self._progress_call_stack.append(fn.__qualname__)
             self._update_progress_hook(0)
@@ -43,16 +44,16 @@
 
 
 class CLIProgressHook(ProgressHook):
     """
     General progress hook to display progress of each decorated function individually.
     """
 
-    def __init__(self, leave: bool | None = None, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
+    def __init__(self, leave: bool | None = None, **kwargs) -> None:
+        super().__init__(**kwargs)
         self.leave = leave
         self.bars: dict[tuple[str, ...], tqdm.tqdm] = {}
 
     def __call__(self, progress: float, stack: list[str]) -> None:
         key = tuple(stack)
         if key not in self.bars:
             try:
@@ -86,22 +87,22 @@
         if key not in self.start_times:
             self.start_times[key] = time.time()
         if progress == 1:
             full_diration = time.time() - self.start_times[key]
             self_duration = full_diration
             for k, v in self.self_durations.items():
                 if len(k) > len(key) and k[: len(key)] == key:
-                    self_duration -= self.self_durations[k]
+                    self_duration -= v
             self.self_durations[key] = self_duration
             desc = '> ' * (len(key) - 1) + key[-1]
             print(f'{full_diration:5.2f} {self_duration:5.2f}  {desc}')
 
 
 # Specific progress hooks for use in saving
-class SaveProgressHook(ProgressHook):
+class _SaveProgressHook(ProgressHook):
     """
     Base class for progress hook to use when saving data.
 
     The subclasses attempt to roughly work out the overall progress by using some
     very quick benchmarks I've manually thrown together (`weights`). These are not
     accurate at all, but do give a better idea of the progress level than just giving
     e.g. the number of backplanes generated. It could definitely be improved by e.g.
@@ -142,15 +143,16 @@
     def update_bar(self, progress_change: float) -> None:
         raise NotImplementedError
 
     def get_description(self) -> str:
         return ''
 
 
-class SaveNavProgressHook(SaveProgressHook):
+# pylint: disable-next=abstract-method
+class _SaveNavProgressHook(_SaveProgressHook):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.weights: dict[str, float] = {
             'BodyXY._get_targvec_img': 100,
             'BodyXY._get_lonlat_img': 50,
             'BodyXY._get_radec_img': 5,
             'BodyXY._get_lonlat_centric_img': 5,
@@ -162,15 +164,16 @@
         }
         self.default_key = 'Observation.save_observation'
 
     def get_description(self) -> str:
         return 'Saving observation'
 
 
-class SaveMapProgressHook(SaveProgressHook):
+# pylint: disable-next=abstract-method
+class _SaveMapProgressHook(_SaveProgressHook):
     def __init__(self, n_wavelengths: int, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.n_wavelengths = n_wavelengths
         self.weights: dict[str, float] = {
             'Observation._get_mapped_data': n_wavelengths * 5,
             'BodyXY._get_targvec_map': 10,
             'BodyXY._get_illumf_map': 5,
@@ -184,34 +187,32 @@
         }
         self.default_key = 'Observation.save_mapped_observation'
 
     def get_description(self) -> str:
         return 'Saving map'
 
 
-class SaveProgressHookCLI(SaveProgressHook):
+class _SaveProgressHookCLI(_SaveProgressHook):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.bar = tqdm.tqdm(
             total=100,
             desc=self.get_description(),
             unit='%',
             bar_format='{l_bar}{bar}| [{elapsed}<{remaining}, {rate_fmt}{postfix}]',
             leave=True,
         )
 
     def update_bar(self, progress_change: float) -> None:
-        # * 0.99999 to ensure floating point errros don't accumulate to >100%
-        self.bar.update(progress_change * 100 *0.99999)
+        # * 0.99999 to ensure floating point errros don't accumulate to >100%
+        self.bar.update(progress_change * 100 * 0.99999)
         if self.progress_parts.get(self.default_key, 0) >= 1:
             self.bar.update(100 - self.overall_progress * 100)
             self.bar.close()
 
 
-class SaveNavProgressHookCLI(SaveNavProgressHook, SaveProgressHookCLI):
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
+class SaveNavProgressHookCLI(_SaveNavProgressHook, _SaveProgressHookCLI):
+    pass
 
 
-class SaveMapProgressHookCLI(SaveMapProgressHook, SaveProgressHookCLI):
-    def __init__(self, n_wavelengths: int, *args, **kwargs) -> None:
-        super().__init__(n_wavelengths, *args, **kwargs)
+class SaveMapProgressHookCLI(_SaveMapProgressHook, _SaveProgressHookCLI):
+    pass
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `planetmapper-1.7.0/planetmapper.egg-info/PKG-INFO` & `planetmapper-1.7.1/planetmapper.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.7.0
+Version: 1.7.1
 Summary: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
 Project-URL: GitHub, https://github.com/ortk95/planetmapper
 Keywords: planetmapper,astronomy,space,science,spice,ephemeris,planetary-science
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 
 # PlanetMapper
 
 [![PyPI](https://img.shields.io/pypi/v/planetmapper?label=PyPi&logo=python&logoColor=silver)](https://pypi.org/project/planetmapper/)
-[![Upload Python Package](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml)
+[![Upload Package](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml)
 [![Pylint](https://github.com/ortk95/planetmapper/actions/workflows/pylint.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/pylint.yml)
-[![Black](https://github.com/ortk95/planetmapper/actions/workflows/black.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/black.yml)
-[![Tests](https://github.com/ortk95/planetmapper/actions/workflows/unittest.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/unittest.yml)
+[![Format](https://github.com/ortk95/planetmapper/actions/workflows/format.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/format.yml)
+[![Tests](https://github.com/ortk95/planetmapper/actions/workflows/test.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/test.yml)
+[![Coverage Status](https://img.shields.io/coverallsCoverage/github/ortk95/planetmapper)](https://coveralls.io/github/ortk95/planetmapper)
 [![Documentation Status](https://readthedocs.org/projects/planetmapper/badge/?version=latest)](https://planetmapper.readthedocs.io/en/latest/?badge=latest)
 
 
 A Python module for visualising, navigating and mapping Solar System observations.
 
 ## [Documentation](https://planetmapper.readthedocs.io)
 For full documentation and [API reference](https://planetmapper.readthedocs.io/en/latest/documentation.html), visit [planetmapper.readthedocs.io](https://planetmapper.readthedocs.io/en/latest/index.html)
@@ -32,15 +33,15 @@
 ```
 pip install planetmapper --upgrade
 ```
 
 _Requires Python 3.10+_
 
 ## Key features
-### [Fit and map observations using a full featured user interface](https://planetmapper.readthedocs.io/en/latest/user_interface.html)
+### [Fit and map astronomical observations using a full featured user interface](https://planetmapper.readthedocs.io/en/latest/user_interface.html)
 ![PlanetMapper graphical user interface](https://github.com/ortk95/planetmapper/blob/main/docs/images/gui_fitting.png?raw=true)
 
 ### [Easily visualise solar system observations with just a few lines of code](https://planetmapper.readthedocs.io/en/latest/general_python_api.html#wireframe-plots)
 
 ```python
 body = planetmapper.Body('saturn', '2020-01-01')
 body.plot_wireframe_radec()
```

### Comparing `planetmapper-1.7.0/planetmapper.egg-info/SOURCES.txt` & `planetmapper-1.7.1/planetmapper.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,17 +15,21 @@
 planetmapper/utils.py
 planetmapper.egg-info/PKG-INFO
 planetmapper.egg-info/SOURCES.txt
 planetmapper.egg-info/dependency_links.txt
 planetmapper.egg-info/entry_points.txt
 planetmapper.egg-info/requires.txt
 planetmapper.egg-info/top_level.txt
+planetmapper/data/ring_aliases.json
 planetmapper/data/rings.json
 tests/test_base.py
 tests/test_basic_body.py
 tests/test_body.py
 tests/test_body_xy.py
 tests/test_common.py
+tests/test_data_loader.py
 tests/test_gui.py
 tests/test_init.py
+tests/test_kernel_downloader.py
 tests/test_observation.py
+tests/test_progress.py
 tests/test_utils.py
```

### Comparing `planetmapper-1.7.0/setup.py` & `planetmapper-1.7.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 import sys
+
 import setuptools
 
 root = os.path.abspath(os.path.dirname(__file__))
 sys.path.append(os.path.join(root, 'planetmapper'))
-import common  #  type: ignore
+# pylint: disable-next=import-error
+import common  # type: ignore
 
-with open(os.path.join(root, 'README.md'), 'r') as f:
+with open(os.path.join(root, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='planetmapper',
     version=common.__version__,
     author=common.__author__,
     author_email='oliver.king95@gmail.com',
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `planetmapper-1.7.0/tests/test_basic_body.py` & `planetmapper-1.7.1/tests/test_basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.0/tests/test_body.py` & `planetmapper-1.7.1/tests/test_body.py`

 * *Files 20% similar despite different names*

```diff
@@ -64,14 +64,18 @@
             },
         )
         self.assertEqual(self.body.ring_radii, set())
         self.assertEqual(self.body.coordinates_of_interest_lonlat, [])
         self.assertEqual(self.body.coordinates_of_interest_radec, [])
         self.assertEqual(self.body.other_bodies_of_interest, [])
 
+        moon = Body('moon', '2005-01-01')
+        self.assertEqual(moon.positive_longitude_direction, 'E')
+        self.assertTrue(moon.prograde)
+
     def test_repr(self):
         self.assertEqual(
             repr(self.body),
             "Body('JUPITER', '2005-01-01T00:00:00.000000', observer='HST')",
         )
 
     def test_eq(self):
@@ -102,14 +106,72 @@
                 'Jupiter',
                 observer='HST',
                 utc='2005-01-01T00:00:00',
                 aberration_correction='CN+S',
             ),
         )
 
+    def test_hash(self):
+        self.assertEqual(
+            hash(self.body),
+            hash(Body('Jupiter', observer='HST', utc='2005-01-01T00:00:00')),
+        )
+        times = [
+            '2005-01-01T00:00:00',
+            '2005-01-01T00:00:00',
+            '2005-01-01T00:00:00',
+            '2005-01-01T00:00:01',
+            '2005-01-01T00:00:02',
+        ]
+        d = {}
+        for time in times:
+            d[Body('Jupiter', observer='HST', utc=time)] = time
+        self.assertEqual(len(d), 3)
+
+    def test_get_kwargs(self):
+        self.assertEqual(
+            self.body._get_kwargs(),
+            {
+                'optimize_speed': True,
+                'target': 'JUPITER',
+                'utc': '2005-01-01T00:00:00.000000',
+                'observer': 'HST',
+                'aberration_correction': 'CN',
+                'observer_frame': 'J2000',
+                'illumination_source': 'SUN',
+                'subpoint_method': 'INTERCEPT/ELLIPSOID',
+                'surface_method': 'ELLIPSOID',
+            },
+        )
+
+    def test_copy(self):
+        body = Body('Jupiter', observer='HST', utc='2005-01-01T00:00:00')
+        body.add_other_bodies_of_interest('amalthea')
+        body.coordinates_of_interest_lonlat.append((0, 0))
+        body.coordinates_of_interest_radec.extend([(1, 2), (3, 4)])
+        body.add_named_rings()
+
+        copy = body.copy()
+        self.assertEqual(body, copy)
+        self.assertIsNot(body, copy)
+        self.assertEqual(body._get_kwargs(), copy._get_kwargs())
+        self.assertEqual(body.other_bodies_of_interest, copy.other_bodies_of_interest)
+        self.assertEqual(
+            body.coordinates_of_interest_lonlat, copy.coordinates_of_interest_lonlat
+        )
+        self.assertEqual(
+            body.coordinates_of_interest_radec, copy.coordinates_of_interest_radec
+        )
+        self.assertEqual(body.ring_radii, copy.ring_radii)
+
+        body.coordinates_of_interest_lonlat.append((5, 6))
+        self.assertNotEqual(
+            body.coordinates_of_interest_lonlat, copy.coordinates_of_interest_lonlat
+        )
+
     def test_create_other_body(self):
         self.assertEqual(
             self.body.create_other_body('amalthea'),
             Body('AMALTHEA', observer='HST', utc='2005-01-01T00:00:00'),
         )
 
     def test_add_other_bodies_of_interest(self):
@@ -126,14 +188,31 @@
                 Body('METIS', observer='HST', utc='2005-01-01T00:00:00'),
                 Body('THEBE', observer='HST', utc='2005-01-01T00:00:00'),
             ],
         )
         self.body.other_bodies_of_interest.clear()
         self.assertEqual(self.body.other_bodies_of_interest, [])
 
+        utc = '2005-01-01 04:00:00'
+        jupiter = planetmapper.Body('Jupiter', utc)
+        jupiter.add_other_bodies_of_interest('THEBE', only_visible=True)
+        self.assertEqual(jupiter.other_bodies_of_interest, [])
+
+        jupiter.add_other_bodies_of_interest('AMALTHEA', 'THEBE', only_visible=True)
+        self.assertEqual(jupiter.other_bodies_of_interest, [Body('AMALTHEA', utc)])
+
+        jupiter.other_bodies_of_interest.clear()
+        self.assertEqual(jupiter.other_bodies_of_interest, [])
+
+        jupiter.add_other_bodies_of_interest('AMALTHEA', 'THEBE')
+        self.assertEqual(
+            jupiter.other_bodies_of_interest,
+            [Body('AMALTHEA', utc), Body('THEBE', utc)],
+        )
+
     def test_add_satellites_to_bodies_of_interest(self):
         self.body.other_bodies_of_interest.clear()
         with self.assertRaises(SpiceSPKINSUFFDATA):
             self.body.add_satellites_to_bodies_of_interest()
 
         self.body.other_bodies_of_interest.clear()
         self.body.add_satellites_to_bodies_of_interest(skip_insufficient_data=True)
@@ -145,36 +224,88 @@
                 Body('ADRASTEA', '2005-01-01T00:00:00.000000', 'HST'),
                 Body('METIS', '2005-01-01T00:00:00.000000', 'HST'),
             ],
         )
         self.body.other_bodies_of_interest.clear()
         self.assertEqual(self.body.other_bodies_of_interest, [])
 
-    def test_ring_raddii_from_name(self):
+        utc = '2005-01-01 04:00:00'
+        jupiter = planetmapper.Body('Jupiter', utc)
+        jupiter.add_satellites_to_bodies_of_interest(
+            skip_insufficient_data=True, only_visible=True
+        )
+        self.assertEqual(
+            jupiter.other_bodies_of_interest,
+            [Body('AMALTHEA', utc), Body('ADRASTEA', utc), Body('METIS', utc)],
+        )
+        jupiter.other_bodies_of_interest.clear()
+        self.assertEqual(jupiter.other_bodies_of_interest, [])
+
+        jupiter.add_satellites_to_bodies_of_interest(skip_insufficient_data=True)
+        self.assertEqual(
+            jupiter.other_bodies_of_interest,
+            [
+                Body('AMALTHEA', utc),
+                Body('THEBE', utc),
+                Body('ADRASTEA', utc),
+                Body('METIS', utc),
+            ],
+        )
+        jupiter.other_bodies_of_interest.clear()
+        self.assertEqual(jupiter.other_bodies_of_interest, [])
+
+    def test_standardise_ring_name(self):
+        pairs = [
+            ('a', 'a'),
+            ('A', 'a'),
+            ('  a  ', 'a'),
+            (' c  RiNg ', 'c'),
+            ('liberte', 'liberté'),
+            ('égalité', 'egalité'),
+            ('égalité', 'egalité'),
+            (' FrAternitE ring ', 'fraternité'),
+        ]
+        for name, expected in pairs:
+            with self.subTest(name=name):
+                self.assertEqual(self.body._standardise_ring_name(name), expected)
+
+    def test_ring_radii_from_name(self):
         self.assertEqual(self.body.ring_radii_from_name('Halo'), [89400.0, 123000.0])
         self.assertEqual(
             self.body.ring_radii_from_name('   MaIn rinG         '),
             [123000.0, 128940.0],
         )
         self.assertEqual(self.body.ring_radii_from_name('main'), [123000.0, 128940.0])
         with self.assertRaises(ValueError):
             self.body.ring_radii_from_name('spam')
 
     def test_add_named_rings(self):
         self.body.ring_radii.clear()
         self.assertEqual(self.body.ring_radii, set())
 
-        self.body.add_named_rings('halo', 'main')
+        self.body.add_named_rings('halo', '   MaIn rinG ')
         self.assertEqual(self.body.ring_radii, {89400.0, 123000.0, 128940.0})
 
         self.body.add_named_rings('thebe extension')
         self.assertEqual(
             self.body.ring_radii, {89400.0, 123000.0, 128940.0, 221900.0, 280000.0}
         )
 
+        with self.assertRaises(ValueError):
+            self.body.add_named_rings('<<<< test ring name >>>>')
+
+        self.body.ring_radii.clear()
+        self.assertEqual(self.body.ring_radii, set())
+
+        self.body.add_named_rings()
+        self.assertEqual(
+            self.body.ring_radii,
+            {280000.0, 181350.0, 128940.0, 221900.0, 89400.0, 123000.0},
+        )
+
         self.body.ring_radii.clear()
         self.assertEqual(self.body.ring_radii, set())
 
     def test_lonlat2radec(self):
         pairs = [
             [(0, 90), (196.37390490466322, -5.561534444253404)],
             [(0, 0), (196.36982789576643, -5.565060944053696)],
@@ -336,14 +467,50 @@
                     array([nan, nan, nan, 196.36782109, 196.36828846, nan]),
                     array([nan, nan, nan, -5.56817191, -5.56246245, nan]),
                 ),
                 equal_nan=True,
             )
         )
 
+    def test_other_body_los_intercept(self):
+        utc = '2005-01-01 04:00:00'
+        jupiter = planetmapper.Body('Jupiter', utc)
+
+        intercepts: list[tuple[str, str | None, bool]] = [
+            ('thebe', 'hidden', False),
+            ('metis', 'transit', True),
+            ('amalthea', None, True),
+            ('adrastea', None, True),
+            ('jupiter', 'same', True),
+        ]
+
+        for moon, intercept, visible in intercepts:
+            body = jupiter.create_other_body(moon)
+            arguments = [
+                moon,
+                body,
+                body.target_body_id,
+                planetmapper.BasicBody(moon, utc),
+            ]
+            for arg in arguments:
+                with self.subTest(moon=moon, arg=arg):
+                    self.assertEqual(jupiter.other_body_los_intercept(arg), intercept)
+                    self.assertEqual(
+                        jupiter.test_if_other_body_visible(arg),
+                        visible,
+                    )
+
+        body = planetmapper.Body('Jupiter', '2005-01-01 00:35:24')
+        self.assertEqual(body.other_body_los_intercept('amalthea'), 'part hidden')
+        self.assertEqual(body.test_if_other_body_visible('amalthea'), True)
+
+        body = planetmapper.Body('Jupiter', '2005-01-01 06:34:05')
+        self.assertEqual(body.other_body_los_intercept('amalthea'), 'part transit')
+        self.assertEqual(body.test_if_other_body_visible('amalthea'), True)
+
     def test_illimination_angles_from_lonlat(self):
         self.assertTrue(
             np.allclose(
                 self.body.illumination_angles_from_lonlat(0, 0),
                 (10.31594976458697, 163.2795134457034, 152.99822832991876),
             )
         )
@@ -370,14 +537,25 @@
                     array([nan, nan, nan, 196.36784184, 196.36838618, nan]),
                     array([nan, nan, nan, -5.56815505, -5.56246241, nan]),
                 ),
                 equal_nan=True,
             )
         )
 
+    def test_if_lonlat_illuminated(self):
+        pairs: list[tuple[tuple[float, float], bool]] = [
+            ((0, 0), False),
+            ((180, 12), True),
+        ]
+        for (lon, lat), illuminated in pairs:
+            with self.subTest(lon=lon, lat=lat):
+                self.assertEqual(
+                    self.body.test_if_lonlat_illuminated(lon, lat), illuminated
+                )
+
     def test_ring_plane_coordinates(self):
         self.assertTrue(
             np.allclose(
                 self.body.ring_plane_coordinates(
                     196.37198562427025, -5.565793847134351
                 ),
                 (nan, nan, nan),
@@ -541,7 +719,39 @@
     def test_plot_wireframe(self):
         fig, ax = plt.subplots()
         self.body.plot_wireframe_radec(ax, color='red')
         plt.close(fig)
 
         ax = self.body.plot_wireframe_km()
         plt.close(ax.figure)
+
+        self.body.add_named_rings()
+        self.body.coordinates_of_interest_lonlat.extend(
+            [(0, 0), (90, 0), (180, 0), (270, 0)]
+        )
+        self.body.coordinates_of_interest_radec.append(
+            (self.body.target_ra, self.body.target_dec)
+        )
+        self.body.add_other_bodies_of_interest('amalthea')
+        fig, ax = plt.subplots()
+        self.body.plot_wireframe_km(
+            ax,
+            label_poles=False,
+            add_axis_labels=False,
+            aspect_adjustable='box',
+            add_title=False,
+            grid_interval=43,
+            indicate_equator=True,
+            indicate_prime_meridian=True,
+        )
+        plt.close(fig)
+        self.body.ring_radii.clear()
+        self.body.coordinates_of_interest_lonlat.clear()
+        self.body.coordinates_of_interest_radec.clear()
+        self.body.other_bodies_of_interest.clear()
+
+        # Test hidden other bodies
+        jupiter = planetmapper.Body('jupiter', utc='2005-01-01T04:00')
+        jupiter.add_other_bodies_of_interest('thebe', 'metis', 'amalthea', 'adrastea')
+        fig, ax = plt.subplots()
+        jupiter.plot_wireframe_radec(ax)
+        plt.close(fig)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `planetmapper-1.7.0/tests/test_body_xy.py` & `planetmapper-1.7.1/tests/test_body_xy.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 import numpy as np
 from numpy import array, nan
 
 import planetmapper
 import planetmapper.base
 import planetmapper.progress
 from planetmapper import BodyXY
-from planetmapper.body_xy import (
-    BackplaneNotFoundError,
-    Backplane,
-    _cache_clearable_result,
-    _cache_stable_result,
-)
+from planetmapper.body_xy import Backplane, BackplaneNotFoundError
+
+
+class TestFunctions(unittest.TestCase):
+    def test_make_backplane_documentation_str(self):
+        self.assertIsInstance(
+            planetmapper.body_xy._make_backplane_documentation_str(), str
+        )
 
 
 class TestBodyXY(unittest.TestCase):
     def setUp(self):
         planetmapper.set_kernel_path(common_testing.KERNEL_PATH)
         self.body = BodyXY(
             'Jupiter', observer='HST', utc='2005-01-01T00:00:00', nx=15, ny=10
@@ -37,14 +39,73 @@
 
     def test_attributes(self):
         self.assertEqual(self.body._nx, 15)
         self.assertEqual(self.body._ny, 10)
         self.assertEqual(self.body_zero_size._nx, 0)
         self.assertEqual(self.body_zero_size._ny, 0)
 
+    def test_from_body(self):
+        body = planetmapper.Body('Jupiter', observer='HST', utc='2005-01-01T00:00:00')
+        body.add_other_bodies_of_interest('amalthea')
+        body.coordinates_of_interest_lonlat.append((0, 0))
+        body.coordinates_of_interest_radec.extend([(0, 0), (1, 1)])
+        body.add_named_rings()
+
+        body_xy = BodyXY.from_body(body, nx=15, ny=10)
+        self.assertEqual(
+            body_xy,
+            BodyXY('Jupiter', observer='HST', utc='2005-01-01T00:00:00', nx=15, ny=10),
+        )
+
+        self.assertEqual(body.target, body_xy.target)
+        self.assertEqual(body.utc, body_xy.utc)
+        self.assertEqual(body.observer, body_xy.observer)
+        self.assertEqual(
+            body.coordinates_of_interest_lonlat, body_xy.coordinates_of_interest_lonlat
+        )
+        self.assertEqual(
+            body.coordinates_of_interest_radec, body_xy.coordinates_of_interest_radec
+        )
+        self.assertEqual(body.ring_radii, body_xy.ring_radii)
+
+        body.coordinates_of_interest_radec.clear()
+        self.assertNotEqual(
+            body.coordinates_of_interest_radec, body_xy.coordinates_of_interest_radec
+        )
+
+    def test_to_body(self):
+        body_xy = BodyXY('Jupiter', observer='HST', utc='2005-01-01T00:00:00', sz=10)
+        body_xy.add_other_bodies_of_interest('amalthea')
+        body_xy.coordinates_of_interest_lonlat.append((0, 0))
+        body_xy.coordinates_of_interest_radec.extend([(0, 0), (1, 1)])
+
+        body = body_xy.to_body()
+        self.assertEqual(
+            body,
+            planetmapper.Body('Jupiter', observer='HST', utc='2005-01-01T00:00:00'),
+        )
+
+        self.assertEqual(body.target, body_xy.target)
+        self.assertEqual(body.utc, body_xy.utc)
+        self.assertEqual(body.observer, body_xy.observer)
+        self.assertEqual(
+            body.coordinates_of_interest_lonlat, body_xy.coordinates_of_interest_lonlat
+        )
+        self.assertEqual(
+            body.coordinates_of_interest_radec, body_xy.coordinates_of_interest_radec
+        )
+        self.assertEqual(body.ring_radii, body_xy.ring_radii)
+
+        body.coordinates_of_interest_radec.clear()
+        self.assertNotEqual(
+            body.coordinates_of_interest_radec, body_xy.coordinates_of_interest_radec
+        )
+
+        self.assertEqual(BodyXY.from_body(body, sz=10), body_xy)
+
     def test_repr(self):
         self.assertEqual(
             repr(self.body),
             "BodyXY('JUPITER', '2005-01-01T00:00:00.000000', 15, 10, observer='HST')",
         )
         self.assertEqual(
             repr(self.body_zero_size),
@@ -67,14 +128,70 @@
         self.assertNotEqual(
             self.body, BodyXY('Jupiter', utc='2005-01-01T00:00:00', nx=14, ny=10)
         )
         self.assertNotEqual(
             self.body, BodyXY('Jupiter', utc='2005-01-01T00:00:00', nx=15, ny=11)
         )
 
+    def test_hash(self):
+        with self.assertRaises(TypeError):
+            hash(self.body)
+        with self.assertRaises(TypeError):
+            hash(self.body_zero_size)
+        with self.assertRaises(TypeError):
+            d = {self.body: 1}
+
+    def test_get_kwargs(self):
+        self.assertEqual(
+            self.body._get_kwargs(),
+            {
+                'optimize_speed': True,
+                'target': 'JUPITER',
+                'utc': '2005-01-01T00:00:00.000000',
+                'observer': 'HST',
+                'aberration_correction': 'CN',
+                'observer_frame': 'J2000',
+                'illumination_source': 'SUN',
+                'subpoint_method': 'INTERCEPT/ELLIPSOID',
+                'surface_method': 'ELLIPSOID',
+                'nx': 15,
+                'ny': 10,
+            },
+        )
+
+    def test_copy(self):
+        body = BodyXY(
+            'Jupiter', observer='HST', utc='2005-01-01T00:00:00', nx=15, ny=10
+        )
+        body.add_other_bodies_of_interest('amalthea')
+        body.coordinates_of_interest_lonlat.append((0, 0))
+        body.coordinates_of_interest_radec.extend([(1, 2), (3, 4)])
+        body.add_named_rings()
+        body.set_disc_params(1, 2, 3, 4)
+
+        copy = body.copy()
+        self.assertEqual(body, copy)
+        self.assertIsNot(body, copy)
+        self.assertEqual(body._get_kwargs(), copy._get_kwargs())
+        self.assertEqual(body.other_bodies_of_interest, copy.other_bodies_of_interest)
+        self.assertEqual(
+            body.coordinates_of_interest_lonlat, copy.coordinates_of_interest_lonlat
+        )
+        self.assertEqual(
+            body.coordinates_of_interest_radec, copy.coordinates_of_interest_radec
+        )
+        self.assertEqual(body.ring_radii, copy.ring_radii)
+        self.assertEqual(body.get_img_size(), copy.get_img_size())
+        self.assertEqual(body.get_disc_params(), copy.get_disc_params())
+        self.assertEqual(body.get_disc_method(), copy.get_disc_method())
+
+        body.set_x0(-99)
+        self.assertNotEqual(body, copy)
+        self.assertNotEqual(body.get_x0(), copy.get_x0())
+
     def test_cache(self):
         self.body._cache[' test '] = None
         self.body._clear_cache()
         self.assertEqual(len(self.body._cache), 0)
 
         for fn in (
             self.body.set_x0,
@@ -152,28 +269,33 @@
                     if not any(np.isnan(lonlat)):
                         self.assertTrue(
                             np.allclose(body.lonlat2xy(*lonlat), xy, equal_nan=True)
                         )
                     self.assertTrue(np.allclose(body.km2xy(*km), xy, equal_nan=True))
 
     def test_set_disc_params(self):
-        with self.subTest('args'):
-            x0, y0, r0, rotation = [1.1, 2.2, 3.3, 4.4]
-            self.body.set_disc_params(x0, y0, r0, rotation)
-            self.assertEqual(self.body.get_x0(), x0)
-            self.assertEqual(self.body.get_y0(), y0)
-            self.assertEqual(self.body.get_r0(), r0)
-            self.assertAlmostEqual(self.body.get_rotation(), rotation)
-        with self.subTest('kwargs'):
-            x0, y0, r0, rotation = [1.11, 2.22, 3.33, 4.44]
-            self.body.set_disc_params(x0=x0, y0=y0, r0=r0, rotation=rotation)
-            self.assertEqual(self.body.get_x0(), x0)
-            self.assertEqual(self.body.get_y0(), y0)
-            self.assertEqual(self.body.get_r0(), r0)
-            self.assertAlmostEqual(self.body.get_rotation(), rotation)
+        x0, y0, r0, rotation = [1.1, 2.2, 3.3, 4.4]
+        self.body.set_disc_params(x0, y0, r0, rotation)
+        self.assertEqual(self.body.get_x0(), x0)
+        self.assertEqual(self.body.get_y0(), y0)
+        self.assertEqual(self.body.get_r0(), r0)
+        self.assertAlmostEqual(self.body.get_rotation(), rotation)
+
+        self.body.set_disc_params()
+        self.assertEqual(self.body.get_x0(), x0)
+        self.assertEqual(self.body.get_y0(), y0)
+        self.assertEqual(self.body.get_r0(), r0)
+        self.assertAlmostEqual(self.body.get_rotation(), rotation)
+
+        x0, y0, r0, rotation = [1.11, 2.22, 3.33, 4.44]
+        self.body.set_disc_params(x0=x0, y0=y0, r0=r0, rotation=rotation)
+        self.assertEqual(self.body.get_x0(), x0)
+        self.assertEqual(self.body.get_y0(), y0)
+        self.assertEqual(self.body.get_r0(), r0)
+        self.assertAlmostEqual(self.body.get_rotation(), rotation)
 
     def test_disc_params(self):
         with self.subTest('args'):
             self.body.set_disc_params(0, 0, 1, 0)
             x0, y0, r0, rotation = [11.1, 12.2, 13.3, 14.4]
             self.body.adjust_disc_params(x0, y0, r0, rotation)
             self.assertEqual(self.body.get_x0(), x0)
@@ -232,14 +354,20 @@
             body.set_disc_params(0, 0, 1, 0)
 
         self.assertEqual(self.body.get_img_size(), (15, 10))
         self.assertEqual(self.body_zero_size.get_img_size(), (0, 0))
 
         self.body_zero_size.set_img_size(3, 4)
         self.assertEqual(self.body_zero_size.get_img_size(), (3, 4))
+        self.body_zero_size.set_img_size()
+        self.assertEqual(self.body_zero_size.get_img_size(), (3, 4))
+        self.body_zero_size.set_img_size(nx=5)
+        self.assertEqual(self.body_zero_size.get_img_size(), (5, 4))
+        self.body_zero_size.set_img_size(ny=5)
+        self.assertEqual(self.body_zero_size.get_img_size(), (5, 5))
 
         self.body_zero_size.set_img_size(15, 10)
         self.assertEqual(self.body, self.body_zero_size)
         self.assertTrue(self.body_zero_size._test_if_img_size_valid())
 
         self.body_zero_size.set_img_size(0, 0)
         self.assertEqual(self.body_zero_size.get_img_size(), (0, 0))
@@ -274,14 +402,35 @@
         self.assertTrue(
             np.allclose(
                 self.body.get_disc_params(),
                 (-0.05532064212457044, 0.11116537556358708, 1.0, 0.0),
             )
         )
 
+    def test_img_limits(self):
+        self.assertEqual(self.body.get_img_limits_xy(), ((-0.5, 14.5), (-0.5, 9.5)))
+        self.assertTrue(
+            np.allclose(
+                self.body.get_img_limits_radec(),
+                (
+                    (196.38091225891438, 196.36417481895663),
+                    (-5.571901975157448, -5.560796287842726),
+                ),
+            )
+        )
+        self.assertTrue(
+            np.allclose(
+                self.body.get_img_limits_km(),
+                (
+                    (-151773.3647184372, 130762.09502601624),
+                    (-125352.05899906158, 117394.22356271744),
+                ),
+            )
+        )
+
     def test_limb_xy(self):
         self.body.set_disc_params(5, 8, 10, 45)
         self.assertTrue(
             np.allclose(
                 self.body.limb_xy(npts=5),
                 (
                     array(
@@ -390,15 +539,15 @@
         fig, ax = plt.subplots()
         self.body.plot_map_wireframe(ax=ax, projection='orthographic', lat=56)
         plt.close(fig)
 
         fig, ax = plt.subplots()
         self.body.plot_map_wireframe(ax=ax, projection='azimuthal', lat=-90)
         plt.close(fig)
-    
+
     def test_get_wireframe_overlay(self):
         img = self.body.get_wireframe_overlay_img(output_size=100)
         self.assertEqual(max(img.shape), 100)
         self.assertEqual(len(img.shape), 2)
 
         img = self.body.get_wireframe_overlay_map(output_size=100)
         self.assertEqual(max(img.shape), 100)
@@ -506,14 +655,46 @@
 
     def test_standardise_backplane_name(self):
         self.assertEqual(self.body.standardise_backplane_name('EMISSION'), 'EMISSION')
         self.assertEqual(self.body.standardise_backplane_name(' EMISSION '), 'EMISSION')
         self.assertEqual(self.body.standardise_backplane_name('emission'), 'EMISSION')
         self.assertEqual(self.body.standardise_backplane_name('EmIsSiOn'), 'EMISSION')
 
+    def test_register_backplane(self):
+        name = '<<<TEST>>>'
+        description = 'A test backplane'
+        get_img = lambda: None
+        get_map = lambda: None
+
+        self.body.register_backplane(
+            name,
+            description,
+            get_img,  #  type: ignore
+            get_map,  #  type: ignore
+        )
+
+        backplane = self.body.get_backplane(name)
+        self.assertEqual(backplane.name, name)
+        self.assertEqual(backplane.description, description)
+        self.assertEqual(backplane.get_img, get_img)
+        self.assertEqual(backplane.get_map, get_map)
+
+        with self.assertRaises(ValueError):
+            self.body.register_backplane(
+                name,
+                description,
+                get_img=get_img,  #  type: ignore
+                get_map=get_map,  #  type: ignore
+            )
+
+        del self.body.backplanes[name]
+
+        with self.assertRaises(planetmapper.body_xy.BackplaneNotFoundError):
+            self.body.get_backplane(name)
+
     def test_backplane_summary_string(self):
         lines = [
             'LON-GRAPHIC: Planetographic longitude, positive W [deg]',
             'LAT-GRAPHIC: Planetographic latitude [deg]',
             'LON-CENTRIC: Planetocentric longitude [deg]',
             'LAT-CENTRIC: Planetocentric latitude [deg]',
             'RA: Right ascension [deg]',
@@ -598,78 +779,7 @@
 
     def test_plot_map(self):
         fig, ax = plt.subplots()
         self.body.plot_map(np.ones((180, 360)), ax=ax)
         plt.close(fig)
 
     # Backplane contents tested against FITS reference in test_observation
-
-
-class TestCache(unittest.TestCase):
-    def setUp(self):
-        self._cache = {}
-        self._stable_cache = {}
-        self.functions_called = []
-
-    @_cache_clearable_result
-    def f_clearable(self, a, b=1):
-        self.functions_called.append('f_clearable')
-        return ('f_clearable', a * b)
-
-    @_cache_stable_result
-    def f_stable(self, a, b=1):
-        self.functions_called.append('f_stable')
-        return ('f_stable', a * b)
-
-    def test_clearable_cache(self):
-        self.functions_called = []
-        for attempt in range(3):
-            with self.subTest(attempt=attempt):
-                self._cache.clear()
-                self.functions_called = []
-
-                self.assertEqual(self.f_clearable(1), ('f_clearable', 1))
-                self.assertEqual(self.functions_called, ['f_clearable'])
-                self.assertEqual(self.f_clearable(1), ('f_clearable', 1))
-                self.assertEqual(self.functions_called, ['f_clearable'])
-
-                self.assertEqual(self.f_clearable(2), ('f_clearable', 2))
-                self.assertEqual(self.functions_called, ['f_clearable'] * 2)
-                self.assertEqual(self.f_clearable(2), ('f_clearable', 2))
-                self.assertEqual(self.functions_called, ['f_clearable'] * 2)
-
-                self.assertEqual(self.f_clearable(2, b=2), ('f_clearable', 4))
-                self.assertEqual(self.functions_called, ['f_clearable'] * 3)
-                self.assertEqual(self.f_clearable(2, b=2), ('f_clearable', 4))
-                self.assertEqual(self.functions_called, ['f_clearable'] * 3)
-
-                self.assertEqual(self.f_clearable(1), ('f_clearable', 1))
-                self.assertEqual(self.f_clearable(2), ('f_clearable', 2))
-                self.assertEqual(self.f_clearable(2, b=2), ('f_clearable', 4))
-                self.assertEqual(self.functions_called, ['f_clearable'] * 3)
-
-                self.assertEqual(len(self._cache), 3)
-
-    def test_stable_cache(self):
-        self.functions_called = []
-
-        self.assertEqual(self.f_stable(1), ('f_stable', 1))
-        self.assertEqual(self.functions_called, ['f_stable'])
-        self.assertEqual(self.f_stable(1), ('f_stable', 1))
-        self.assertEqual(self.functions_called, ['f_stable'])
-
-        self.assertEqual(self.f_stable(2), ('f_stable', 2))
-        self.assertEqual(self.functions_called, ['f_stable'] * 2)
-        self.assertEqual(self.f_stable(2), ('f_stable', 2))
-        self.assertEqual(self.functions_called, ['f_stable'] * 2)
-
-        self.assertEqual(self.f_stable(2, b=2), ('f_stable', 4))
-        self.assertEqual(self.functions_called, ['f_stable'] * 3)
-        self.assertEqual(self.f_stable(2, b=2), ('f_stable', 4))
-        self.assertEqual(self.functions_called, ['f_stable'] * 3)
-
-        self.assertEqual(self.f_stable(1), ('f_stable', 1))
-        self.assertEqual(self.f_stable(2), ('f_stable', 2))
-        self.assertEqual(self.f_stable(2, b=2), ('f_stable', 4))
-        self.assertEqual(self.functions_called, ['f_stable'] * 3)
-
-        self.assertEqual(len(self._stable_cache), 3)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `planetmapper-1.7.0/tests/test_init.py` & `planetmapper-1.7.1/tests/test_init.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import unittest
-import planetmapper
+
 import common_testing
 from packaging import version
 
+import planetmapper
+
 
 class TestInit(unittest.TestCase):
     def test_init(self):
         self.assertEqual(planetmapper.__author__, 'Oliver King')
         self.assertEqual(planetmapper.__url__, 'https://github.com/ortk95/planetmapper')
 
     def test_version(self):
```

### Comparing `planetmapper-1.7.0/tests/test_observation.py` & `planetmapper-1.7.1/tests/test_observation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-import unittest
+import fnmatch
 import os
+import unittest
+
 import common_testing
 import numpy as np
 from astropy.io import fits
+
 import planetmapper
 import planetmapper.base
 import planetmapper.progress
 from planetmapper import Observation
-import fnmatch
 
 
 class TestObservation(unittest.TestCase):
     def setUp(self) -> None:
         planetmapper.set_kernel_path(common_testing.KERNEL_PATH)
         self.path = os.path.join(common_testing.DATA_PATH, 'inputs', 'test.fits')
         self.observation = Observation(self.path)
@@ -35,25 +37,29 @@
             path = os.path.join(common_testing.DATA_PATH, 'inputs', 'image.png')
             obs = Observation(
                 path,
                 target='Jupiter',
                 observer='hst',
                 utc='2005-01-01T00:00:00',
             )
+            self.assertEqual(obs, obs)
+            self.assertNotEqual(obs, self.observation)
             self.assertEqual(obs.path, path)
             self.assertEqual(obs.target, 'JUPITER')
             self.assertEqual(obs.header['OBJECT'], 'JUPITER')
             self.assertEqual(obs.observer, 'HST')
             self.assertEqual(obs.utc, '2005-01-01T00:00:00.000000')
             self.assertEqual(obs.header['DATE-OBS'], '2005-01-01T00:00:00.000000')
             self.assertTrue(np.array_equal(obs.data, 100 * np.ones((4, 10, 5))))
 
         with self.subTest('planmap.fits'):
             path = os.path.join(common_testing.DATA_PATH, 'inputs', 'planmap.fits')
             obs = Observation(path)
+            self.assertEqual(obs, obs)
+            self.assertNotEqual(obs, self.observation)
             self.assertEqual(obs.path, path)
             self.assertEqual(obs.target, 'JUPITER')
             self.assertEqual(obs.observer, 'HST')
             self.assertEqual(obs.utc, '2005-01-01T12:00:00.000000')
             self.assertTrue(
                 np.array_equal(
                     obs.data,
@@ -64,14 +70,16 @@
             self.assertAlmostEqual(obs.get_y0(), 2.2)
             self.assertAlmostEqual(obs.get_r0(), 3.3)
             self.assertAlmostEqual(obs.get_rotation(), 4.4)
 
         with self.subTest('planmap.fits+override'):
             path = os.path.join(common_testing.DATA_PATH, 'inputs', 'planmap.fits')
             obs = Observation(path, observer='EARTH', utc='2005-01-01')
+            self.assertEqual(obs, obs)
+            self.assertNotEqual(obs, self.observation)
             self.assertEqual(obs.path, path)
             self.assertEqual(obs.target, 'JUPITER')
             self.assertEqual(obs.observer, 'EARTH')
             self.assertEqual(obs.utc, '2005-01-01T00:00:00.000000')
             self.assertTrue(
                 np.array_equal(
                     obs.data,
@@ -82,26 +90,30 @@
             self.assertAlmostEqual(obs.get_y0(), 2.2)
             self.assertAlmostEqual(obs.get_r0(), 3.3)
             self.assertAlmostEqual(obs.get_rotation(), 4.4)
 
         with self.subTest('wcs.fits'):
             path = os.path.join(common_testing.DATA_PATH, 'inputs', 'wcs.fits')
             obs = Observation(path)
+            self.assertEqual(obs, obs)
+            self.assertNotEqual(obs, self.observation)
             self.assertEqual(obs.path, path)
             self.assertEqual(obs.target, 'JUPITER')
             self.assertEqual(obs.observer, 'HST')
             self.assertEqual(obs.utc, '2005-01-01T00:00:00.000000')
             self.assertAlmostEqual(obs.get_x0(), 198.87871682168858, delta=0.2)
             self.assertAlmostEqual(obs.get_y0(), -31.89770255438151, delta=0.2)
             self.assertAlmostEqual(obs.get_r0(), 164.4473594677842, delta=0.2)
             self.assertAlmostEqual(obs.get_rotation(), 260.32237572846986, delta=0.2)
 
         with self.subTest('extended.fits'):
             path = os.path.join(common_testing.DATA_PATH, 'inputs', 'extended.fits')
             obs = Observation(path)
+            self.assertEqual(obs, obs)
+            self.assertNotEqual(obs, self.observation)
             self.assertEqual(obs.path, path)
             self.assertEqual(obs.target, 'JUPITER')
             self.assertEqual(obs.observer, 'HST')
             self.assertEqual(obs.utc, '2005-01-01T12:00:00.000000')
             self.assertTrue(
                 np.array_equal(
                     obs.data,
@@ -113,14 +125,16 @@
             data = np.ones((5, 6, 7))
             obs = Observation(
                 data=data,
                 target='Jupiter',
                 observer='hst',
                 utc='2005-01-01T00:00:00',
             )
+            self.assertEqual(obs, obs)
+            self.assertNotEqual(obs, self.observation)
             self.assertIsNone(obs.path)
             self.assertEqual(obs.target, 'JUPITER')
             self.assertEqual(obs.observer, 'HST')
             self.assertEqual(obs.utc, '2005-01-01T00:00:00.000000')
             self.assertTrue(np.array_equal(obs.data, data))
 
         with self.subTest('data+header+target+observer+utc'):
@@ -129,14 +143,16 @@
             obs = Observation(
                 data=data,
                 header=header,
                 target='Jupiter',
                 observer='hst',
                 utc='2005-01-01T00:00:00',
             )
+            self.assertEqual(obs, obs)
+            self.assertNotEqual(obs, self.observation)
             self.assertIsNone(obs.path)
             self.assertEqual(obs.target, 'JUPITER')
             self.assertEqual(obs.observer, 'HST')
             self.assertEqual(obs.utc, '2005-01-01T00:00:00.000000')
             self.assertEqual(obs.header, header)
             self.assertTrue(np.array_equal(obs.data, data))
 
@@ -145,14 +161,16 @@
             header = fits.Header(
                 {'OBJECT': 'jupiter', 'TELESCOP': 'HST', 'DATE-OBS': '2005-01-01'}
             )
             obs = Observation(
                 data=data,
                 header=header,
             )
+            self.assertEqual(obs, obs)
+            self.assertNotEqual(obs, self.observation)
             self.assertIsNone(obs.path)
             self.assertEqual(obs.target, 'JUPITER')
             self.assertEqual(obs.observer, 'HST')
             self.assertEqual(obs.utc, '2005-01-01T00:00:00.000000')
             self.assertEqual(obs.header, header)
             data_expected = data[np.newaxis, :, :]
             self.assertTrue(np.array_equal(obs.data, data_expected))
@@ -162,14 +180,16 @@
             header = fits.Header(
                 {'OBJECT': 'jupiter', 'TELESCOP': 'HST', 'DATE-OBS': '2005-01-01'}
             )
             obs = Observation(
                 data=data,
                 header=header,
             )
+            self.assertEqual(obs, obs)
+            self.assertNotEqual(obs, self.observation)
             self.assertIsNone(obs.path)
             self.assertEqual(obs.target, 'JUPITER')
             self.assertEqual(obs.observer, 'HST')
             self.assertEqual(obs.utc, '2005-01-01T00:00:00.000000')
             self.assertEqual(obs.header, header)
             self.assertTrue(np.array_equal(obs.data, data))
 
@@ -177,14 +197,16 @@
             data = np.ones((5, 6, 7))
             header = fits.Header({'OBJECT': 'jupiter', 'DATE-OBS': '2005-01-01'})
             obs = Observation(
                 data=data,
                 header=header,
                 observer='HST',
             )
+            self.assertEqual(obs, obs)
+            self.assertNotEqual(obs, self.observation)
             self.assertIsNone(obs.path)
             self.assertEqual(obs.target, 'JUPITER')
             self.assertEqual(obs.observer, 'HST')
             self.assertEqual(obs.utc, '2005-01-01T00:00:00.000000')
             self.assertEqual(obs.header, header)
             self.assertTrue(np.array_equal(obs.data, data))
 
@@ -194,14 +216,16 @@
                 {'OBJECT': 'mars', 'TELESCOP': 'HST', 'DATE-OBS': '2005-01-01'}
             )
             obs = Observation(
                 data=data,
                 header=header,
                 target='jupiter',
             )
+            self.assertEqual(obs, obs)
+            self.assertNotEqual(obs, self.observation)
             self.assertIsNone(obs.path)
             self.assertEqual(obs.target, 'JUPITER')
             self.assertEqual(obs.observer, 'HST')
             self.assertEqual(obs.utc, '2005-01-01T00:00:00.000000')
             self.assertEqual(obs.header, header)
             self.assertTrue(np.array_equal(obs.data, data))
 
@@ -212,14 +236,28 @@
         self.assertEqual(self.observation.utc, '2005-01-01T00:00:00.000000')
         self.assertEqual(self.observation._nx, 7)
         self.assertEqual(self.observation._ny, 10)
 
     def test_repr(self):
         self.assertEqual(repr(self.observation), f'Observation({self.path!r})')
 
+    def test_hash(self):
+        with self.assertRaises(TypeError):
+            hash(self.observation)
+
+    def test_eq(self):
+        self.assertEqual(self.observation, self.observation)
+        self.assertEqual(self.observation, Observation(self.path))
+
+    def test_copy(self):
+        copy = self.observation.copy()
+        self.assertEqual(copy.path, self.observation.path)
+        self.assertEqual(repr(copy), repr(self.observation))
+        self.assertEqual(copy, self.observation)
+
     def test_disc_from_header(self):
         with self.assertRaises(ValueError):
             self.observation.disc_from_header()
 
         path = os.path.join(common_testing.DATA_PATH, 'inputs', 'planmap.fits')
         obs = Observation(path)
         self.assertAlmostEqual(obs.get_x0(), 1.1)
@@ -354,26 +392,34 @@
 
     def test_save_observation(self):
         self.observation.set_disc_params(2.5, 3.1, 3.9, 123.456)
         self.observation.set_disc_method('<<<test>>>')
 
         path = os.path.join(common_testing.TEMP_PATH, 'test_nav.fits')
 
+        # test print info here
+        self.observation.save_observation(
+            path, print_info=True, wireframe_kwargs=dict(output_size=20, dpi=20)
+        )
+        self.compare_fits_to_reference(path)
+
         # test progress bar here too
         self.observation.save_observation(
             path, show_progress=True, wireframe_kwargs=dict(output_size=20, dpi=20)
         )
         self.compare_fits_to_reference(path)
 
     def test_save_mapped_observation(self):
         self.observation.set_disc_params(2.5, 3.1, 3.9, 123.456)
         self.observation.set_disc_method('<<<test>>>')
 
         map_kwargs = {
-            'rectangular-nearest': dict(degree_interval=30, interpolation='nearest'),
+            'rectangular-nearest': dict(
+                degree_interval=30, interpolation='nearest', show_progress=True
+            ),
             'rectangular-linear': dict(
                 degree_interval=30, interpolation='linear', include_wireframe=False
             ),
             'rectangular-quadratic': dict(
                 degree_interval=30,
                 interpolation='quadratic',
                 include_backplanes=False,
@@ -442,16 +488,18 @@
                     self.assertEqual(data.shape, data_ref.shape)
 
                     # Significantly increase tolerance for wireframe as it is generated
                     # from a Matplotlib plot, so is sensitive to the OS/environment
                     # (e.g. fonts available), and is only a cosmetic backplane anyway
                     # so the actual values don't matter anywhere near as much as the
                     # other backplanes.
-                    atol = 64 if extname == 'WIREFRAME' else 1e-8 # 1e-8 is the default
-                    self.assertTrue(np.allclose(data, data_ref, atol=atol, equal_nan=True))
+                    atol = 64 if extname == 'WIREFRAME' else 1e-8  # 1e-8 is the default
+                    self.assertTrue(
+                        np.allclose(data, data_ref, atol=atol, equal_nan=True)
+                    )
 
                 header = hdu.header
                 header_ref = hdu_ref.header
                 with self.subTest(filename=filename, extname=extname):
                     self.assertEqual(set(header.keys()), set(header_ref.keys()))
 
                 keys_to_skip = {'*DATE*', '*VERSION*'}
```

### Comparing `planetmapper-1.7.0/tests/test_utils.py` & `planetmapper-1.7.1/tests/test_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,68 @@
-import unittest
+import datetime
 import os
+import unittest
+import warnings
+
 import common_testing
 import matplotlib.pyplot as plt
 import numpy as np
-from numpy import array, nan
 from astropy.io import fits
-import warnings
+from numpy import array, nan
+
 import planetmapper
 from planetmapper import utils
-import datetime
 
 
 class TestUtils(unittest.TestCase):
     def setUp(self) -> None:
         planetmapper.set_kernel_path(common_testing.KERNEL_PATH)
 
     def test_format_radec_axes(self):
         fig, ax = plt.subplots()
         utils.format_radec_axes(ax, 45)
         self.assertAlmostEqual(ax.get_aspect(), 1 / 0.7071067811865476)  #  type: ignore
         self.assertTrue(ax.xaxis_inverted())
         plt.close(fig)
 
+        fig, ax = plt.subplots()
+        ax.invert_xaxis()
+        utils.format_radec_axes(
+            ax, 0, dms_ticks=False, add_axis_labels=False, aspect_adjustable='box'
+        )
+        self.assertAlmostEqual(ax.get_aspect(), 1.0)  # type: ignore
+        self.assertTrue(ax.xaxis_inverted())
+        plt.close(fig)
+
+        fig, ax = plt.subplots()
+        utils.format_radec_axes(ax, 30)
+
+        limits: list[tuple[float, float]] = [
+            (-1, 1),
+            (20.12, 20.123),
+            (-42.01, -42.010001),
+            (0.001, 0.005),
+            (-20, 30.1),
+            (42, 42.5),
+        ]
+        for limit in limits:
+            ax.set_xlim(*limit)
+            ax.set_ylim(*limit)
+            fig.canvas.draw()
+        plt.close(fig)
+
     def test_decimal_degrees_to_dms(self):
         pairs = [
             [0, (0, 0, 0)],
             [1, (1, 0, 0)],
             [1.23456789, (1, 14, 4.444404)],
             [-123.456, (-123, 27, 21.6)],
             [360, (360, 0, 0)],
+            [-0.1, (0, -6, 0)],
+            [-0.001, (0, 0, -3.6)],
         ]
         for decimal_degrees, dms in pairs:
             with self.subTest(decimal_degrees=decimal_degrees):
                 d, m, s = utils.decimal_degrees_to_dms(decimal_degrees)
                 self.assertEqual(d, dms[0])
                 self.assertEqual(m, dms[1])
                 self.assertAlmostEqual(s, dms[2])
@@ -110,14 +140,22 @@
             [[[nan, -99], [1.23, 45.6]], array([[nan, 0.0], [0.69315353, 1.0]])],
             [[1, 1, 1], array([0, 0, 0])],
         ]
         for a, b in pairs:
             with self.subTest(a):
                 self.assertTrue(np.allclose(utils.normalise(a), b, equal_nan=True))
 
+        self.assertTrue(
+            np.allclose(
+                utils.normalise([1, 1, 1], single_value=42),
+                np.array([42, 42, 42]),
+                equal_nan=True,
+            )
+        )
+
     def test_check_path(self):
         path = os.path.join(
             common_testing.TEMP_PATH,
             datetime.datetime.now().strftime('TEST1_%Y%m%d%H%M%S%f'),
         )
         utils.check_path(path)
         self.assertTrue(os.path.exists(path))
@@ -127,7 +165,9 @@
         path = os.path.join(
             common_testing.TEMP_PATH,
             datetime.datetime.now().strftime('TEST2_%Y%m%d%H%M%S%f'),
         )
         utils.check_path(os.path.join(path, 'test_file.txt'))
         self.assertTrue(os.path.exists(path))
         os.rmdir(path)
+
+        utils.check_path('')
```

