# Comparing `tmp/unyts-0.5.8.tar.gz` & `tmp/unyts-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unyts-0.5.8.tar", last modified: Wed Jan 18 18:22:55 2023, max compression
+gzip compressed data, was "unyts-0.5.9.tar", last modified: Wed Jan 18 21:40:44 2023, max compression
```

## Comparing `unyts-0.5.8.tar` & `unyts-0.5.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-01-18 18:22:55.360000 unyts-0.5.8/
--rw-rw-rw-   0        0        0     1077 2020-11-01 00:39:44.000000 unyts-0.5.8/LICENSE
--rw-rw-rw-   0        0        0     6258 2023-01-18 18:22:56.000000 unyts-0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     4206 2023-01-18 18:16:50.000000 unyts-0.5.8/README.md
--rw-rw-rw-   0        0        0      890 2023-01-18 18:16:50.000000 unyts-0.5.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-18 18:22:56.000000 unyts-0.5.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-18 18:22:55.360000 unyts-0.5.8/src/
-drwxrwxrwx   0        0        0        0 2023-01-18 18:22:55.360000 unyts-0.5.8/src/unyts/
--rw-rw-rw-   0        0        0      687 2023-01-18 18:16:50.000000 unyts-0.5.8/src/unyts/__init__.py
--rw-rw-rw-   0        0        0    18092 2023-01-17 21:17:22.000000 unyts-0.5.8/src/unyts/converter.py
--rw-rw-rw-   0        0        0    40910 2023-01-15 22:49:36.000000 unyts-0.5.8/src/unyts/database.py
--rw-rw-rw-   0        0        0    19751 2023-01-18 18:16:50.000000 unyts-0.5.8/src/unyts/dictionaries.py
--rw-rw-rw-   0        0        0      862 2022-12-29 13:49:38.000000 unyts-0.5.8/src/unyts/errors.py
-drwxrwxrwx   0        0        0        0 2023-01-18 18:22:55.370000 unyts-0.5.8/src/unyts/helpers/
--rw-rw-rw-   0        0        0      158 2022-09-20 21:54:58.000000 unyts-0.5.8/src/unyts/helpers/__init__.py
--rw-rw-rw-   0        0        0     7072 2022-12-31 14:19:22.000000 unyts-0.5.8/src/unyts/helpers/caster.py
--rw-rw-rw-   0        0        0     1275 2023-01-13 00:37:54.000000 unyts-0.5.8/src/unyts/helpers/common_classes.py
--rw-rw-rw-   0        0        0      841 2022-12-29 12:31:02.000000 unyts-0.5.8/src/unyts/helpers/is_number.py
--rw-rw-rw-   0        0        0     1127 2022-12-31 14:19:22.000000 unyts-0.5.8/src/unyts/helpers/is_unit.py
--rw-rw-rw-   0        0        0     1987 2023-01-17 21:17:22.000000 unyts-0.5.8/src/unyts/helpers/multi_split.py
--rw-rw-rw-   0        0        0     3442 2023-01-17 21:17:22.000000 unyts-0.5.8/src/unyts/helpers/unit_string_tools.py
--rw-rw-rw-   0        0        0     4688 2022-12-31 14:46:52.000000 unyts-0.5.8/src/unyts/network.py
--rw-rw-rw-   0        0        0    10713 2023-01-17 21:17:22.000000 unyts-0.5.8/src/unyts/operations.py
--rw-rw-rw-   0        0        0     4761 2023-01-13 00:37:54.000000 unyts-0.5.8/src/unyts/parameters.py
--rw-rw-rw-   0        0        0     2082 2022-12-31 14:37:54.000000 unyts-0.5.8/src/unyts/searches.py
--rw-rw-rw-   0        0        0    28075 2023-01-17 21:17:22.000000 unyts-0.5.8/src/unyts/unit_class.py
-drwxrwxrwx   0        0        0        0 2023-01-18 18:22:55.370000 unyts-0.5.8/src/unyts/units/
--rw-rw-rw-   0        0        0     1491 2023-01-18 18:16:50.000000 unyts-0.5.8/src/unyts/units/Energy.py
--rw-rw-rw-   0        0        0     1030 2023-01-18 18:16:52.000000 unyts-0.5.8/src/unyts/units/Temperature.py
--rw-rw-rw-   0        0        0      648 2023-01-18 18:16:52.000000 unyts-0.5.8/src/unyts/units/Time.py
--rw-rw-rw-   0        0        0      129 2022-09-08 15:55:48.000000 unyts-0.5.8/src/unyts/units/__init__.py
--rw-rw-rw-   0        0        0     1021 2023-01-13 00:37:54.000000 unyts-0.5.8/src/unyts/units/custom.py
--rw-rw-rw-   0        0        0     2158 2023-01-18 18:16:50.000000 unyts-0.5.8/src/unyts/units/define.py
--rw-rw-rw-   0        0        0     1285 2023-01-18 18:16:52.000000 unyts-0.5.8/src/unyts/units/force.py
--rw-rw-rw-   0        0        0     1220 2023-01-18 18:16:52.000000 unyts-0.5.8/src/unyts/units/geometry.py
--rw-rw-rw-   0        0        0     1028 2023-01-18 18:16:52.000000 unyts-0.5.8/src/unyts/units/rates.py
--rw-rw-rw-   0        0        0     1650 2023-01-18 18:16:52.000000 unyts-0.5.8/src/unyts/units/ratios.py
--rw-rw-rw-   0        0        0     2441 2023-01-18 18:16:52.000000 unyts-0.5.8/src/unyts/units/unitless.py
-drwxrwxrwx   0        0        0        0 2023-01-18 18:22:55.360000 unyts-0.5.8/src/unyts.egg-info/
--rw-rw-rw-   0        0        0     6258 2023-01-18 18:22:56.000000 unyts-0.5.8/src/unyts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      992 2023-01-18 18:22:56.000000 unyts-0.5.8/src/unyts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-18 18:22:56.000000 unyts-0.5.8/src/unyts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-01-18 18:22:56.000000 unyts-0.5.8/src/unyts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-01-18 21:40:44.290000 unyts-0.5.9/
+-rw-rw-rw-   0        0        0     1077 2020-11-01 00:39:44.000000 unyts-0.5.9/LICENSE
+-rw-rw-rw-   0        0        0     6258 2023-01-18 21:40:46.000000 unyts-0.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4206 2023-01-18 18:16:50.000000 unyts-0.5.9/README.md
+-rw-rw-rw-   0        0        0      890 2023-01-18 21:37:24.000000 unyts-0.5.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-01-18 21:40:46.000000 unyts-0.5.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-01-18 21:40:44.300000 unyts-0.5.9/src/
+drwxrwxrwx   0        0        0        0 2023-01-18 21:40:44.300000 unyts-0.5.9/src/unyts/
+-rw-rw-rw-   0        0        0      675 2023-01-18 21:37:24.000000 unyts-0.5.9/src/unyts/__init__.py
+-rw-rw-rw-   0        0        0    18082 2023-01-18 21:37:24.000000 unyts-0.5.9/src/unyts/converter.py
+-rw-rw-rw-   0        0        0    40895 2023-01-18 21:37:24.000000 unyts-0.5.9/src/unyts/database.py
+-rw-rw-rw-   0        0        0    19746 2023-01-18 21:37:24.000000 unyts-0.5.9/src/unyts/dictionaries.py
+-rw-rw-rw-   0        0        0      862 2022-12-29 13:49:38.000000 unyts-0.5.9/src/unyts/errors.py
+drwxrwxrwx   0        0        0        0 2023-01-18 21:40:44.310000 unyts-0.5.9/src/unyts/helpers/
+-rw-rw-rw-   0        0        0      158 2022-09-20 21:54:58.000000 unyts-0.5.9/src/unyts/helpers/__init__.py
+-rw-rw-rw-   0        0        0     7057 2023-01-18 21:37:24.000000 unyts-0.5.9/src/unyts/helpers/caster.py
+-rw-rw-rw-   0        0        0     1271 2023-01-18 21:37:24.000000 unyts-0.5.9/src/unyts/helpers/common_classes.py
+-rw-rw-rw-   0        0        0      841 2022-12-29 12:31:02.000000 unyts-0.5.9/src/unyts/helpers/is_number.py
+-rw-rw-rw-   0        0        0     1142 2023-01-18 21:37:24.000000 unyts-0.5.9/src/unyts/helpers/is_unit.py
+-rw-rw-rw-   0        0        0     1987 2023-01-17 21:17:22.000000 unyts-0.5.9/src/unyts/helpers/multi_split.py
+-rw-rw-rw-   0        0        0     3429 2023-01-18 21:37:24.000000 unyts-0.5.9/src/unyts/helpers/unit_string_tools.py
+-rw-rw-rw-   0        0        0     4688 2022-12-31 14:46:52.000000 unyts-0.5.9/src/unyts/network.py
+-rw-rw-rw-   0        0        0    10688 2023-01-18 21:37:24.000000 unyts-0.5.9/src/unyts/operations.py
+-rw-rw-rw-   0        0        0     4761 2023-01-13 00:37:54.000000 unyts-0.5.9/src/unyts/parameters.py
+-rw-rw-rw-   0        0        0     2082 2022-12-31 14:37:54.000000 unyts-0.5.9/src/unyts/searches.py
+-rw-rw-rw-   0        0        0    28062 2023-01-18 21:37:24.000000 unyts-0.5.9/src/unyts/unit_class.py
+drwxrwxrwx   0        0        0        0 2023-01-18 21:40:44.310000 unyts-0.5.9/src/unyts/units/
+-rw-rw-rw-   0        0        0     1479 2023-01-18 21:37:24.000000 unyts-0.5.9/src/unyts/units/Energy.py
+-rw-rw-rw-   0        0        0     1018 2023-01-18 21:37:24.000000 unyts-0.5.9/src/unyts/units/Temperature.py
+-rw-rw-rw-   0        0        0      636 2023-01-18 21:37:24.000000 unyts-0.5.9/src/unyts/units/Time.py
+-rw-rw-rw-   0        0        0      129 2022-09-08 15:55:48.000000 unyts-0.5.9/src/unyts/units/__init__.py
+-rw-rw-rw-   0        0        0     1009 2023-01-18 21:37:24.000000 unyts-0.5.9/src/unyts/units/custom.py
+-rw-rw-rw-   0        0        0     2047 2023-01-18 21:37:24.000000 unyts-0.5.9/src/unyts/units/define.py
+-rw-rw-rw-   0        0        0     1273 2023-01-18 21:37:24.000000 unyts-0.5.9/src/unyts/units/force.py
+-rw-rw-rw-   0        0        0     1208 2023-01-18 21:37:24.000000 unyts-0.5.9/src/unyts/units/geometry.py
+-rw-rw-rw-   0        0        0     1016 2023-01-18 21:37:24.000000 unyts-0.5.9/src/unyts/units/rates.py
+-rw-rw-rw-   0        0        0     1638 2023-01-18 21:37:24.000000 unyts-0.5.9/src/unyts/units/ratios.py
+-rw-rw-rw-   0        0        0     2421 2023-01-18 21:37:24.000000 unyts-0.5.9/src/unyts/units/unitless.py
+drwxrwxrwx   0        0        0        0 2023-01-18 21:40:44.300000 unyts-0.5.9/src/unyts.egg-info/
+-rw-rw-rw-   0        0        0     6258 2023-01-18 21:40:46.000000 unyts-0.5.9/src/unyts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      992 2023-01-18 21:40:46.000000 unyts-0.5.9/src/unyts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-18 21:40:46.000000 unyts-0.5.9/src/unyts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-01-18 21:40:46.000000 unyts-0.5.9/src/unyts.egg-info/top_level.txt
```

### Comparing `unyts-0.5.8/LICENSE` & `unyts-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `unyts-0.5.8/PKG-INFO` & `unyts-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unyts
-Version: 0.5.8
+Version: 0.5.9
 Summary: a unit converter based on graph network and classes to operate with units.
 Author-email: Martin Carlos Araya <martinaraya@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Martín Carlos Araya
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `unyts-0.5.8/README.md` & `unyts-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `unyts-0.5.8/pyproject.toml` & `unyts-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 733e 3d36 312e 3022 5d0d  uptools>=61.0"].
 00000030: 0a62 7569 6c64 2d62 6163 6b65 6e64 203d  .build-backend =
 00000040: 2022 7365 7475 7074 6f6f 6c73 2e62 7569   "setuptools.bui
 00000050: 6c64 5f6d 6574 6122 0d0a 0d0a 5b70 726f  ld_meta"....[pro
 00000060: 6a65 6374 5d0d 0a6e 616d 6520 3d20 2275  ject]..name = "u
 00000070: 6e79 7473 220d 0a76 6572 7369 6f6e 203d  nyts"..version =
-00000080: 2022 302e 352e 3822 0d0a 6175 7468 6f72   "0.5.8"..author
+00000080: 2022 302e 352e 3922 0d0a 6175 7468 6f72   "0.5.9"..author
 00000090: 7320 3d20 5b0d 0a20 207b 206e 616d 653d  s = [..  { name=
 000000a0: 224d 6172 7469 6e20 4361 726c 6f73 2041  "Martin Carlos A
 000000b0: 7261 7961 222c 2065 6d61 696c 3d22 6d61  raya", email="ma
 000000c0: 7274 696e 6172 6179 6140 676d 6169 6c2e  rtinaraya@gmail.
 000000d0: 636f 6d22 207d 2c0d 0a5d 0d0a 6465 7363  com" },..]..desc
 000000e0: 7269 7074 696f 6e20 3d20 2261 2075 6e69  ription = "a uni
 000000f0: 7420 636f 6e76 6572 7465 7220 6261 7365  t converter base
```

### Comparing `unyts-0.5.8/src/unyts/__init__.py` & `unyts-0.5.9/src/unyts/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat Oct 24 18:24:20 2020
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
-__version__ = '0.5.8'
+__version__ = '0.5.9'
 __release__ = 2023018
 __all__ = ['units', 'convert', 'Unit', 'is_Unit']
 
-import unyts.parameters
-from unyts.parameters import print_path, reload, raise_error, cache
-from unyts.units.define import units
-from unyts.converter import convert
-from unyts.unit_class import Unit, is_Unit
+# import unyts.parameters
+from .parameters import unyts_parameters_, print_path, reload, raise_error, cache
+from .units.define import units
+from .converter import convert
+from .unit_class import Unit, is_Unit
 
-if unyts.parameters.unyts_parameters_.show_version_:
+if unyts_parameters_.show_version_:
     print("loaded unyts version", __version__)
-    unyts.parameters.unyts_parameters_.show_version_ = False
-    unyts.parameters.unyts_parameters_.save_params()
+    # unyts.parameters.unyts_parameters_.show_version_ = False
+    # unyts.parameters.unyts_parameters_.save_params()
```

### Comparing `unyts-0.5.8/src/unyts/converter.py` & `unyts-0.5.9/src/unyts/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 """
 Created on Sat Oct 24 15:57:27 2020
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
 __version__ = '0.5.3'
-__release__ = 20230117
+__release__ = 20230118
 __all__ = ['convert', 'convertible']
 
-from unyts.database import unitsNetwork
+from .database import unitsNetwork
 from unyts.dictionaries import dictionary, temperatureRatioConversions
 from unyts.searches import BFS, print_path
 from unyts.errors import NoConversionFoundError
 from unyts.parameters import unyts_parameters_
 from unyts.helpers.unit_string_tools import split_unit as _split_unit, reduce_parentheses as _reduce_parentheses
 from functools import reduce
 from warnings import warn
@@ -368,15 +368,15 @@
     if value is not None and not isinstance(value, numeric):
         raise ValueError("value must be numeric.")
     if type(value) in [list, tuple]:
         raise TypeError("`value` can not be a list or tuple if NumPy is not installed.")
 
     print_conversion_path = _clean_print_conversion_path(print_conversion_path)
 
-    from unyts.unit_class import Unit
+    from .unit_class import Unit
     if isinstance(from_unit, Unit):
         from_unit = from_unit.get_unit()
     if isinstance(to_unit, Unit):
         to_unit = to_unit.get_unit()
 
     if type(from_unit) is str and from_unit not in ('"', "'"):
         from_unit = from_unit.strip("( ')").strip('( ")').strip("'")
```

### Comparing `unyts-0.5.8/src/unyts/database.py` & `unyts-0.5.9/src/unyts/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 """
 Created on Sat Oct 24 12:36:48 2020
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
 __version__ = '0.5.3'
-__release__ = 20230115
+__release__ = 20230118
 __all__ = ['unitsNetwork']
 
-from unyts.dictionaries import SI, SI_order, OGF, OGF_order, DATA, DATA_order, dictionary, StandardAirDensity, \
+from .dictionaries import SI, SI_order, OGF, OGF_order, DATA, DATA_order, dictionary, StandardAirDensity, \
     StandardEarthGravity
-from unyts.network import UDigraph, UNode, Conversion
-from unyts.parameters import unyts_parameters_, dir_path
+from .network import UDigraph, UNode, Conversion
+from .parameters import unyts_parameters_, dir_path
 from os.path import isfile
 from json import dump as json_dump
 from warnings import warn
 
 try:
     from cloudpickle import dump as cloudpickle_dump, load as cloudpickle_load
     _cloudpickle_ = True
```

### Comparing `unyts-0.5.8/src/unyts/dictionaries.py` & `unyts-0.5.9/src/unyts/dictionaries.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 """
 Created on Sat Oct 24 12:14:51 2020
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
 __version__ = '0.5.8'
-__release__ = 20230115
+__release__ = 20230118
 __all__ = ['dictionary', 'SI', 'OGF', 'DATA', 'StandardAirDensity', 'StandardEarthGravity', 'unitless_names']
 
 from json import load as json_load
 from pickle import load as pickle_load, dump as pickle_dump
 from os.path import isfile
-from unyts.parameters import unyts_parameters_, dir_path
+from .parameters import unyts_parameters_, dir_path
 
 StandardAirDensity = 1.225  # Kg/m3 or g/cc
 StandardEarthGravity = 9.80665  # m/s2 or 980.665 cm/s2 from
 
 # Sistema Internacional
 SI = {
     'Y': (lambda X: X * 1E+24, lambda X: X * 1E+48, lambda X: X * 1E+72),  # yotta
```

### Comparing `unyts-0.5.8/src/unyts/errors.py` & `unyts-0.5.9/src/unyts/errors.py`

 * *Files identical despite different names*

### Comparing `unyts-0.5.8/src/unyts/helpers/caster.py` & `unyts-0.5.9/src/unyts/helpers/caster.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 """
 Created on Wed Aug  3 21:14:44 2022
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
 __version__ = '0.4.9'
-__release__ = 20221231
+__release__ = 20230118
 __all__ = ['caster', 'to_number']
 
-
-from unyts.helpers.common_classes import number
+from .common_classes import number
 
 
 def caster(string: str) -> number:
     """
     Helper function to try to cast the string to number
 
     Parameters
```

### Comparing `unyts-0.5.8/src/unyts/helpers/common_classes.py` & `unyts-0.5.9/src/unyts/helpers/common_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 """
 Created on Sat Oct 24 14:34:59 2020
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
 __version__ = '0.5.4'
-__release__ = 20230112
+__release__ = 20230118
 __all__ = ['array_like', 'number', 'numeric', 'unit_or_str']
 
-from unyts.unit_class import Unit
+from ..unit_class import Unit
 try:
     from numpy import ndarray, int64, float64, int32, float32
     _numpy_ = True
 except ModuleNotFoundError:
     _numpy_ = False
 try:
     from pandas import Series, DataFrame
```

### Comparing `unyts-0.5.8/src/unyts/helpers/is_number.py` & `unyts-0.5.9/src/unyts/helpers/is_number.py`

 * *Files identical despite different names*

### Comparing `unyts-0.5.8/src/unyts/helpers/is_unit.py` & `unyts-0.5.9/src/unyts/helpers/is_unit.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 """
 Created on Sat Oct 24 14:46:04 2020
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
 __version__ = '0.4.9'
-__release__ = 20221231
+__release__ = 20230118
 __all__ = ['is_unit']
 
-from unyts.dictionaries import dictionary
+from ..dictionaries import dictionary as _dictionary
 
 
 def is_unit(unit: str) -> bool:
     if type(unit) is str:
         unit = unit.strip()
     else:
         raise TypeError("unit must be a string.")
 
-    for each in list(dictionary.keys()):
+    for each in list(_dictionary.keys()):
         if '_' not in each:
-            is_u = unit in list(dictionary[each])
+            is_u = unit in list(_dictionary[each])
             if is_u:
                 return True
 
     if '/' in unit or '*' in unit:
         unit_split = []
         for each in unit.split('/'):
             unit_split += each.split('*')
         ret = [False] * len(unit_split)
-        for each in list(dictionary.keys()):
+        for each in list(_dictionary.keys()):
             if '_' not in each:
                 for sub_u in range(len(unit_split)):
-                    if unit_split[sub_u] in list(dictionary[each]):
+                    if unit_split[sub_u] in list(_dictionary[each]):
                         ret[sub_u] = True
         for each in ret:
             if not each:
                 return False
         return True
     return False
```

### Comparing `unyts-0.5.8/src/unyts/helpers/multi_split.py` & `unyts-0.5.9/src/unyts/helpers/multi_split.py`

 * *Files identical despite different names*

### Comparing `unyts-0.5.8/src/unyts/helpers/unit_string_tools.py` & `unyts-0.5.9/src/unyts/helpers/unit_string_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 """
 Created on Sat Oct 24 15:57:27 2020
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
 __version__ = '0.5.2'
-__release__ = 20230117
+__release__ = 20230118
 __all__ = ['split_ratio', 'split_product', 'split_unit', 'reduce_parentheses', 'reduce_units']
 
-from unyts.helpers.multi_split import multi_split
+from .multi_split import multi_split
 
 
 def split_ratio(unit: str) -> tuple:  # tuple[str]
     return list(map(str.strip, unit.split('/')))
 
 
 def split_product(unit: str) -> tuple:  # tuple[str]
```

### Comparing `unyts-0.5.8/src/unyts/network.py` & `unyts-0.5.9/src/unyts/network.py`

 * *Files identical despite different names*

### Comparing `unyts-0.5.8/src/unyts/operations.py` & `unyts-0.5.9/src/unyts/operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 """
 Created on Sat Oct 24 14:38:58 2020
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
 __version__ = '0.5.2'
-__release__ = 20230116
+__release__ = 20230118
 __all__ = ['unit_product', 'unit_division', 'unit_base_power', 'unit_power', 'unit_addition', 'unit_inverse']
 
-from unyts.dictionaries import dictionary, unitless_names
-from unyts.converter import convertible
-from unyts.helpers.is_number import is_number
-from unyts.helpers.unit_string_tools import reduce_units
-from unyts.helpers.multi_split import multi_split
+from .dictionaries import dictionary, unitless_names
+from .converter import convertible
+from .helpers.is_number import is_number
+from .helpers.unit_string_tools import reduce_units
+from .helpers.multi_split import multi_split
 
 
 def unit_split(unit_string: str) -> str:
     us = multi_split(unit_string)
     return us
```

### Comparing `unyts-0.5.8/src/unyts/parameters.py` & `unyts-0.5.9/src/unyts/parameters.py`

 * *Files identical despite different names*

### Comparing `unyts-0.5.8/src/unyts/searches.py` & `unyts-0.5.9/src/unyts/searches.py`

 * *Files identical despite different names*

### Comparing `unyts-0.5.8/src/unyts/unit_class.py` & `unyts-0.5.9/src/unyts/unit_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
 __version__ = '0.5.7'
 __release__ = 20230117
 __all__ = ['Unit', 'is_Unit']
 
-from unyts.errors import WrongUnitsError, WrongValueError, NoConversionFoundError
-from unyts.operations import unit_product as _unit_product, unit_division as _unit_division, unit_base_power as _unit_base_power
-from unyts.helpers.unit_string_tools import reduce_units as _reduce_units
-from unyts.converter import convert as _convert, convertible as _convertible
+from .errors import WrongUnitsError, WrongValueError, NoConversionFoundError
+from .operations import unit_product as _unit_product, unit_division as _unit_division, \
+    unit_base_power as _unit_base_power
+from .helpers.unit_string_tools import reduce_units as _reduce_units
+from .converter import convert as _convert, convertible as _convertible
 from numbers import Number
 
 
 try:
     import numpy as np
     from numpy import ndarray, int64, float64, int32, float32
     _numpy_ = True
```

### Comparing `unyts-0.5.8/src/unyts/units/Energy.py` & `unyts-0.5.9/src/unyts/units/Energy.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
 __version__ = '0.5.3'
 __release__ = 20230118
 __all__ = ['Energy', 'Power']
 
-from unyts.dictionaries import dictionary as _dictionary
-from unyts.unit_class import Unit
-from unyts.helpers.common_classes import unit_or_str, numeric
+from ..dictionaries import dictionary as _dictionary
+from ..unit_class import Unit
+from ..helpers.common_classes import unit_or_str, numeric
 
 
 class Energy(Unit):
     classUnits = _dictionary['Energy']
 
     def __init__(self, value: numeric, unit: unit_or_str):
         self.name = 'energy'
```

### Comparing `unyts-0.5.8/src/unyts/units/Temperature.py` & `unyts-0.5.9/src/unyts/units/Temperature.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
 __version__ = '0.5.3'
 __release__ = 20230118
 __all__ = ['Temperature', 'TemperatureGradient']
 
-from unyts.dictionaries import dictionary as _dictionary
-from unyts.unit_class import Unit
-from unyts.helpers.common_classes import unit_or_str, numeric
+from ..dictionaries import dictionary as _dictionary
+from ..unit_class import Unit
+from ..helpers.common_classes import unit_or_str, numeric
 
 
 class Temperature(Unit):
     classUnits = _dictionary['Temperature']
 
     def __init__(self, value: numeric, units: unit_or_str):
         self.name = 'temperature'
```

### Comparing `unyts-0.5.8/src/unyts/units/Time.py` & `unyts-0.5.9/src/unyts/units/Time.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
 __version__ = '0.5.3'
 __release__ = 20230118
 __all__ = ['Time']
 
-from unyts.dictionaries import dictionary as _dictionary
-from unyts.unit_class import Unit
-from unyts.helpers.common_classes import unit_or_str, numeric
+from ..dictionaries import dictionary as _dictionary
+from ..unit_class import Unit
+from ..helpers.common_classes import unit_or_str, numeric
 
 
 class Time(Unit):
     classUnits = _dictionary['Time']
 
     def __init__(self, value: numeric, units: unit_or_str):
         self.name = 'time'
```

### Comparing `unyts-0.5.8/src/unyts/units/custom.py` & `unyts-0.5.9/src/unyts/units/custom.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 """
 Created on Sat Oct 24 14:34:59 2020
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
 __version__ = '0.5.2'
-__release__ = 20230107
+__release__ = 20230118
 __all__ = ['CustomUnits', 'UserUnits', 'OtherUnits']
 
-from unyts.dictionaries import dictionary
-from unyts.unit_class import Unit
-from unyts.helpers.common_classes import unit_or_str, numeric
+from ..dictionaries import dictionary
+from ..unit_class import Unit
+from ..helpers.common_classes import unit_or_str, numeric
 
 
 def CustomUnits(value: numeric, units: unit_or_str) -> Unit:
     return UserUnits(value, units)
 
 
 def OtherUnits(value: numeric, units: unit_or_str) -> Unit:
```

### Comparing `unyts-0.5.8/src/unyts/units/define.py` & `unyts-0.5.9/src/unyts/units/define.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
 __version__ = '0.5.0'
 __release__ = 20230118
 __all__ = ['units']
 
-from unyts.dictionaries import dictionary as _dictionary
-from unyts.units.custom import UserUnits, OtherUnits
-from unyts.units.force import Pressure, Weight, Compressibility
-from unyts.units.geometry import Length, Area, Volume
-from unyts.units.temperature import Temperature, TemperatureGradient
-from unyts.units.time import Time
-from unyts.units.unitless import Dimensionless, Percentage
-from unyts.units.ratios import Density, VolumeRatio, ProductivityIndex, PressureGradient
-from unyts.units.rates import Rate, Speed, Velocity
-from unyts.units.energy import Energy, Power
-from unyts.unit_class import Unit
-from unyts.helpers.common_classes import unit_or_str as unit_or_str, numeric as numeric
+from ..dictionaries import dictionary as _dictionary
+from .custom import UserUnits, OtherUnits
+from .force import Pressure, Weight, Compressibility
+from .geometry import Length, Area, Volume
+from .temperature import Temperature, TemperatureGradient
+from .time import Time
+from .unitless import Dimensionless, Percentage
+from .ratios import Density, VolumeRatio, ProductivityIndex, PressureGradient
+from .rates import Rate, Speed, Velocity
+from .energy import Energy, Power
+from ..unit_class import Unit
+from ..helpers.common_classes import unit_or_str as unit_or_str, numeric as numeric
 
 
 def units(value: numeric, unit: unit_or_str = None) -> Unit:
     """
     return an instance of units with the provided value and units.
 
     Parameters
```

### Comparing `unyts-0.5.8/src/unyts/units/force.py` & `unyts-0.5.9/src/unyts/units/force.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
 __version__ = '0.5.3'
 __release__ = 20230118
 __all__ = ['Pressure', 'Weight', 'Compressibility']
 
-from unyts.dictionaries import dictionary as _dictionary
-from unyts.unit_class import Unit
-from unyts.helpers.common_classes import unit_or_str, numeric
+from ..dictionaries import dictionary as _dictionary
+from ..unit_class import Unit
+from ..helpers.common_classes import unit_or_str, numeric
 
 
 class Pressure(Unit):
     classUnits = _dictionary['Pressure']
 
     def __init__(self, value: numeric, units: unit_or_str):
         self.name = 'pressure'
```

### Comparing `unyts-0.5.8/src/unyts/units/geometry.py` & `unyts-0.5.9/src/unyts/units/geometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
 __version__ = '0.5.3'
 __release__ = 20230118
 __all__ = ['Length', 'Area', 'Volume']
 
-from unyts.dictionaries import dictionary as _dictionary
-from unyts.unit_class import Unit
-from unyts.helpers.common_classes import unit_or_str, numeric
+from ..dictionaries import dictionary as _dictionary
+from ..unit_class import Unit
+from ..helpers.common_classes import unit_or_str, numeric
 
 
 class Length(Unit):
     classUnits = _dictionary['Length']
 
     def __init__(self, value: numeric, units: unit_or_str):
         self.name = 'length'
```

### Comparing `unyts-0.5.8/src/unyts/units/rates.py` & `unyts-0.5.9/src/unyts/units/rates.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
 __version__ = '0.5.3'
 __release__ = 20230118
 __all__ = ['Rate', 'Speed', 'Velocity']
 
-from unyts.dictionaries import dictionary as _dictionary
-from unyts.unit_class import Unit
-from unyts.helpers.common_classes import unit_or_str, numeric
+from ..dictionaries import dictionary as _dictionary
+from ..unit_class import Unit
+from ..helpers.common_classes import unit_or_str, numeric
 
 
 class Rate(Unit):
     classUnits = _dictionary['Rate']
 
     def __init__(self, value: numeric, units: unit_or_str):
         self.name = 'rate'
```

### Comparing `unyts-0.5.8/src/unyts/units/ratios.py` & `unyts-0.5.9/src/unyts/units/ratios.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
 __version__ = '0.5.3'
 __release__ = 20230118
 __all__ = ['Density', 'VolumeRatio', 'ProductivityIndex', 'PressureGradient']
 
-from unyts.dictionaries import dictionary as _dictionary
-from unyts.unit_class import Unit
-from unyts.helpers.common_classes import unit_or_str, numeric
+from ..dictionaries import dictionary as _dictionary
+from ..unit_class import Unit
+from ..helpers.common_classes import unit_or_str, numeric
 
 
 class Density(Unit):
     classUnits = _dictionary['Density']
 
     def __init__(self, value: numeric, units: unit_or_str):
         self.name = 'density'
```

### Comparing `unyts-0.5.8/src/unyts/units/unitless.py` & `unyts-0.5.9/src/unyts/units/unitless.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
 __version__ = '0.5.3'
 __release__ = 20230118
 __all__ = ['Dimensionless', 'Percentage', 'unitless_names']
 
-from unyts.dictionaries import dictionary as _dictionary
-from unyts.unit_class import Unit
-from unyts.errors import WrongUnitsError
-from unyts.helpers.common_classes import unit_or_str, numeric
-from unyts.dictionaries import unitless_names
+from ..dictionaries import dictionary as _dictionary
+from ..unit_class import Unit
+from ..errors import WrongUnitsError
+from ..helpers.common_classes import unit_or_str, numeric
+from ..dictionaries import unitless_names
 
 
 class Dimensionless(Unit):
     classUnits = _dictionary['Dimensionless']
 
     def __init__(self, value: numeric, units: unit_or_str = None):
         self.name = 'dimensionless'
```

### Comparing `unyts-0.5.8/src/unyts.egg-info/PKG-INFO` & `unyts-0.5.9/src/unyts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unyts
-Version: 0.5.8
+Version: 0.5.9
 Summary: a unit converter based on graph network and classes to operate with units.
 Author-email: Martin Carlos Araya <martinaraya@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Martín Carlos Araya
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `unyts-0.5.8/src/unyts.egg-info/SOURCES.txt` & `unyts-0.5.9/src/unyts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

