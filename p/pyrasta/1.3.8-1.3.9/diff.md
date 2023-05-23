# Comparing `tmp/pyrasta-1.3.8.tar.gz` & `tmp/pyrasta-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyrasta-1.3.8.tar", last modified: Wed Aug  4 14:08:03 2021, max compression
+gzip compressed data, was "dist/pyrasta-1.3.9.tar", last modified: Fri Aug 20 13:07:08 2021, max compression
```

## Comparing `pyrasta-1.3.8.tar` & `pyrasta-1.3.9.tar`

### file list

```diff
@@ -1,39 +1,44 @@
-drwxrwxr-x   0 benjamin  (1001) benjamin  (1001)        0 2021-08-04 14:08:03.000000 pyrasta-1.3.8/
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)       90 2021-07-01 08:40:35.000000 pyrasta-1.3.8/MANIFEST.in
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)       38 2021-08-04 14:08:03.000000 pyrasta-1.3.8/setup.cfg
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)     3600 2021-08-04 14:08:03.000000 pyrasta-1.3.8/PKG-INFO
-drwxrwxr-x   0 benjamin  (1001) benjamin  (1001)        0 2021-08-04 14:08:03.000000 pyrasta-1.3.8/pyrasta.egg-info/
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)      729 2021-08-04 14:08:03.000000 pyrasta-1.3.8/pyrasta.egg-info/SOURCES.txt
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)        8 2021-08-04 14:08:03.000000 pyrasta-1.3.8/pyrasta.egg-info/top_level.txt
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)     3600 2021-08-04 14:08:03.000000 pyrasta-1.3.8/pyrasta.egg-info/PKG-INFO
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)       79 2021-08-04 14:08:03.000000 pyrasta-1.3.8/pyrasta.egg-info/requires.txt
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)        1 2021-08-04 14:08:03.000000 pyrasta-1.3.8/pyrasta.egg-info/dependency_links.txt
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)        1 2021-06-24 13:34:44.000000 pyrasta-1.3.8/pyrasta.egg-info/not-zip-safe
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)      735 2021-07-01 08:40:35.000000 pyrasta-1.3.8/setup.py
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)       78 2021-07-19 13:21:20.000000 pyrasta-1.3.8/requirements.txt
-drwxrwxr-x   0 benjamin  (1001) benjamin  (1001)        0 2021-08-04 14:08:03.000000 pyrasta-1.3.8/pyrasta/
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)      880 2021-06-18 19:23:26.000000 pyrasta-1.3.8/pyrasta/raster.py
-drwxrwxr-x   0 benjamin  (1001) benjamin  (1001)        0 2021-08-04 14:08:03.000000 pyrasta-1.3.8/pyrasta/io_/
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)      121 2021-06-18 19:23:26.000000 pyrasta-1.3.8/pyrasta/io_/__init__.py
--rwxrwxr-x   0 benjamin  (1001) benjamin  (1001)     1570 2021-07-01 15:10:56.000000 pyrasta-1.3.8/pyrasta/io_/files.py
--rwxrwxr-x   0 benjamin  (1001) benjamin  (1001)    21963 2021-08-02 09:04:48.000000 pyrasta-1.3.8/pyrasta/base.py
--rwxrwxr-x   0 benjamin  (1001) benjamin  (1001)     2190 2021-07-27 09:28:09.000000 pyrasta-1.3.8/pyrasta/crs.py
--rwxrwxr-x   0 benjamin  (1001) benjamin  (1001)     4127 2021-07-29 15:00:57.000000 pyrasta-1.3.8/pyrasta/utils.py
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)      184 2021-06-18 19:23:26.000000 pyrasta-1.3.8/pyrasta/exceptions.py
--rwxrwxr-x   0 benjamin  (1001) benjamin  (1001)      183 2021-08-04 14:06:51.000000 pyrasta-1.3.8/pyrasta/__init__.py
-drwxrwxr-x   0 benjamin  (1001) benjamin  (1001)        0 2021-08-04 14:08:03.000000 pyrasta-1.3.8/pyrasta/tools/
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)     1094 2021-07-27 09:28:09.000000 pyrasta-1.3.8/pyrasta/tools/filters.py
--rwxrwxr-x   0 benjamin  (1001) benjamin  (1001)     9398 2021-07-08 15:44:49.000000 pyrasta-1.3.8/pyrasta/tools/windows.py
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)     2258 2021-08-04 14:06:10.000000 pyrasta-1.3.8/pyrasta/tools/mask.py
--rwxrwxr-x   0 benjamin  (1001) benjamin  (1001)     8337 2021-07-27 09:28:09.000000 pyrasta-1.3.8/pyrasta/tools/conversion.py
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)     2573 2021-07-27 09:28:09.000000 pyrasta-1.3.8/pyrasta/tools/rasterize.py
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)     5643 2021-08-04 14:06:10.000000 pyrasta-1.3.8/pyrasta/tools/calculator.py
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)      793 2021-07-27 09:28:09.000000 pyrasta-1.3.8/pyrasta/tools/mapping.py
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)     1144 2021-06-18 19:23:26.000000 pyrasta-1.3.8/pyrasta/tools/dem.py
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)     3013 2021-06-18 19:23:26.000000 pyrasta-1.3.8/pyrasta/tools/clip.py
--rwxrwxr-x   0 benjamin  (1001) benjamin  (1001)     4679 2021-08-02 09:04:48.000000 pyrasta-1.3.8/pyrasta/tools/stats.py
--rwxrwxr-x   0 benjamin  (1001) benjamin  (1001)     5497 2021-07-07 16:22:08.000000 pyrasta-1.3.8/pyrasta/tools/merge.py
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)     1424 2021-07-27 10:35:41.000000 pyrasta-1.3.8/pyrasta/tools/polygonize.py
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)     3246 2021-07-07 16:22:08.000000 pyrasta-1.3.8/pyrasta/tools/srtm.py
--rwxrwxr-x   0 benjamin  (1001) benjamin  (1001)     2781 2021-08-02 14:46:44.000000 pyrasta-1.3.8/pyrasta/tools/__init__.py
--rw-rw-r--   0 benjamin  (1001) benjamin  (1001)     2716 2021-07-27 09:28:09.000000 pyrasta-1.3.8/README.md
+drwxrwxr-x   0 benjamin  (1001) benjamin  (1001)        0 2021-08-20 13:07:08.000000 pyrasta-1.3.9/
+-rw-rw-r--   0 benjamin  (1001) benjamin  (1001)     3600 2021-08-20 13:07:08.000000 pyrasta-1.3.9/PKG-INFO
+-rw-rw-r--   0 benjamin  (1001) benjamin  (1001)     2716 2021-07-23 18:29:27.000000 pyrasta-1.3.9/README.md
+drwxrwxr-x   0 benjamin  (1001) benjamin  (1001)        0 2021-08-20 13:07:08.000000 pyrasta-1.3.9/docs/
+-rw-rw-r--   0 benjamin  (1001) benjamin  (1001)    88938 2021-06-16 10:12:51.000000 pyrasta-1.3.9/docs/espace-dev-ird.png
+-rw-rw-r--   0 benjamin  (1001) benjamin  (1001)       78 2021-07-23 10:23:47.000000 pyrasta-1.3.9/requirements.txt
+-rw-rw-r--   0 benjamin  (1001) benjamin  (1001)       38 2021-08-20 13:07:08.000000 pyrasta-1.3.9/setup.cfg
+drwxrwxr-x   0 benjamin  (1001) benjamin  (1001)        0 2021-08-20 13:07:08.000000 pyrasta-1.3.9/pyrasta.egg-info/
+-rw-r--r--   0 benjamin  (1001) benjamin  (1001)     3600 2021-08-20 13:07:08.000000 pyrasta-1.3.9/pyrasta.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin  (1001) benjamin  (1001)        8 2021-08-20 13:07:08.000000 pyrasta-1.3.9/pyrasta.egg-info/top_level.txt
+-rw-r--r--   0 benjamin  (1001) benjamin  (1001)      781 2021-08-20 13:07:08.000000 pyrasta-1.3.9/pyrasta.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin  (1001) benjamin  (1001)       79 2021-08-20 13:07:08.000000 pyrasta-1.3.9/pyrasta.egg-info/requires.txt
+-rw-r--r--   0 benjamin  (1001) benjamin  (1001)        1 2021-08-20 13:07:08.000000 pyrasta-1.3.9/pyrasta.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin  (1001) benjamin  (1001)        1 2021-03-10 11:41:17.000000 pyrasta-1.3.9/pyrasta.egg-info/not-zip-safe
+-rw-rw-r--   0 benjamin  (1001) benjamin  (1001)      735 2021-06-17 13:13:56.000000 pyrasta-1.3.9/setup.py
+-rw-r--r--   0 benjamin  (1001) benjamin  (1001)     1078 2020-11-21 21:17:47.000000 pyrasta-1.3.9/LICENCE
+-rw-rw-r--   0 benjamin  (1001) benjamin  (1001)       90 2021-06-17 13:13:56.000000 pyrasta-1.3.9/MANIFEST.in
+drwxrwxr-x   0 benjamin  (1001) benjamin  (1001)        0 2021-08-20 13:07:08.000000 pyrasta-1.3.9/pyrasta/
+-rwxrwxr-x   0 benjamin  (1001) benjamin  (1001)     2246 2021-08-20 11:05:02.000000 pyrasta-1.3.9/pyrasta/crs.py
+drwxrwxr-x   0 benjamin  (1001) benjamin  (1001)        0 2021-08-20 13:07:08.000000 pyrasta-1.3.9/pyrasta/io_/
+-rwxrwxr-x   0 benjamin  (1001) benjamin  (1001)     1570 2021-07-02 09:46:14.000000 pyrasta-1.3.9/pyrasta/io_/files.py
+-rw-rw-r--   0 benjamin  (1001) benjamin  (1001)      121 2021-03-11 15:48:04.000000 pyrasta-1.3.9/pyrasta/io_/__init__.py
+-rwxrwxr-x   0 benjamin  (1001) benjamin  (1001)     4127 2021-07-31 19:06:47.000000 pyrasta-1.3.9/pyrasta/utils.py
+-rw-r--r--   0 benjamin  (1001) benjamin  (1001)      184 2021-03-10 12:00:35.000000 pyrasta-1.3.9/pyrasta/exceptions.py
+drwxrwxr-x   0 benjamin  (1001) benjamin  (1001)        0 2021-08-20 13:07:08.000000 pyrasta-1.3.9/pyrasta/tools/
+-rw-r--r--   0 benjamin  (1001) benjamin  (1001)     3246 2021-07-02 15:09:55.000000 pyrasta-1.3.9/pyrasta/tools/srtm.py
+-rw-rw-r--   0 benjamin  (1001) benjamin  (1001)     1200 2021-08-20 11:05:02.000000 pyrasta-1.3.9/pyrasta/tools/dem.py
+-rwxrwxr-x   0 benjamin  (1001) benjamin  (1001)     9398 2021-07-08 18:51:00.000000 pyrasta-1.3.9/pyrasta/tools/windows.py
+-rw-rw-r--   0 benjamin  (1001) benjamin  (1001)     1151 2021-08-20 11:05:02.000000 pyrasta-1.3.9/pyrasta/tools/filters.py
+-rwxrwxr-x   0 benjamin  (1001) benjamin  (1001)     8363 2021-08-20 11:05:02.000000 pyrasta-1.3.9/pyrasta/tools/conversion.py
+-rw-rw-r--   0 benjamin  (1001) benjamin  (1001)      793 2021-07-23 11:16:35.000000 pyrasta-1.3.9/pyrasta/tools/mapping.py
+-rw-rw-r--   0 benjamin  (1001) benjamin  (1001)     2630 2021-08-20 11:05:02.000000 pyrasta-1.3.9/pyrasta/tools/rasterize.py
+-rwxrwxr-x   0 benjamin  (1001) benjamin  (1001)      989 2021-08-20 11:05:02.000000 pyrasta-1.3.9/pyrasta/tools/merge.py
+-rw-rw-r--   0 benjamin  (1001) benjamin  (1001)     3069 2021-08-20 11:05:02.000000 pyrasta-1.3.9/pyrasta/tools/clip.py
+-rw-rw-r--   0 benjamin  (1001) benjamin  (1001)     1477 2021-08-20 11:05:02.000000 pyrasta-1.3.9/pyrasta/tools/polygonize.py
+-rw-rw-r--   0 benjamin  (1001) benjamin  (1001)     5699 2021-08-20 11:05:02.000000 pyrasta-1.3.9/pyrasta/tools/calculator.py
+-rwxrwxr-x   0 benjamin  (1001) benjamin  (1001)     4679 2021-07-31 19:06:47.000000 pyrasta-1.3.9/pyrasta/tools/stats.py
+-rwxrwxr-x   0 benjamin  (1001) benjamin  (1001)     2837 2021-08-20 11:05:02.000000 pyrasta-1.3.9/pyrasta/tools/__init__.py
+-rw-rw-r--   0 benjamin  (1001) benjamin  (1001)     1407 2021-08-20 11:05:02.000000 pyrasta-1.3.9/pyrasta/tools/mask.py
+-rw-r--r--   0 benjamin  (1001) benjamin  (1001)      880 2021-03-15 21:38:18.000000 pyrasta-1.3.9/pyrasta/raster.py
+-rwxrwxr-x   0 benjamin  (1001) benjamin  (1001)      183 2021-08-20 11:06:40.000000 pyrasta-1.3.9/pyrasta/__init__.py
+-rwxrwxr-x   0 benjamin  (1001) benjamin  (1001)    22028 2021-08-20 11:05:02.000000 pyrasta-1.3.9/pyrasta/base.py
+-rw-rw-r--   0 benjamin  (1001) benjamin  (1001)       29 2021-03-10 11:43:10.000000 pyrasta-1.3.9/.gitignore
+-rw-r--r--   0 benjamin  (1001) benjamin  (1001)     2427 2021-03-15 21:38:18.000000 pyrasta-1.3.9/tests.py
```

### Comparing `pyrasta-1.3.8/PKG-INFO` & `pyrasta-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrasta
-Version: 1.3.8
+Version: 1.3.9
 Summary: Some tools for fast and easy raster processing
 Home-page: https://framagit.org/benjaminpillot/pyrasta
 Author: Benjamin Pillot
 Author-email: benjaminpillot@riseup.net
 License: MIT
 Description: # PyRasta
```

### Comparing `pyrasta-1.3.8/pyrasta.egg-info/SOURCES.txt` & `pyrasta-1.3.9/pyrasta.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+.gitignore
+LICENCE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
+tests.py
+docs/espace-dev-ird.png
 pyrasta/__init__.py
 pyrasta/base.py
 pyrasta/crs.py
 pyrasta/exceptions.py
 pyrasta/raster.py
 pyrasta/utils.py
 pyrasta.egg-info/PKG-INFO
```

### Comparing `pyrasta-1.3.8/pyrasta.egg-info/PKG-INFO` & `pyrasta-1.3.9/pyrasta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrasta
-Version: 1.3.8
+Version: 1.3.9
 Summary: Some tools for fast and easy raster processing
 Home-page: https://framagit.org/benjaminpillot/pyrasta
 Author: Benjamin Pillot
 Author-email: benjaminpillot@riseup.net
 License: MIT
 Description: # PyRasta
```

### Comparing `pyrasta-1.3.8/setup.py` & `pyrasta-1.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyrasta-1.3.8/pyrasta/raster.py` & `pyrasta-1.3.9/pyrasta/raster.py`

 * *Files identical despite different names*

### Comparing `pyrasta-1.3.8/pyrasta/io_/files.py` & `pyrasta-1.3.9/pyrasta/io_/files.py`

 * *Files identical despite different names*

### Comparing `pyrasta-1.3.8/pyrasta/base.py` & `pyrasta-1.3.9/pyrasta/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 More detailed description.
 """
 
 import multiprocessing as mp
 
 import numpy as np
-import ogr
 import pyproj
 from pyrasta.io_.files import _copy_to_file
 from pyrasta.tools.calculator import _op, _raster_calculation, _log, _log10
 from pyrasta.tools.clip import _clip_raster_by_extent, _clip_raster_by_mask
 from pyrasta.tools.conversion import _resample_raster, _padding, _rescale_raster, \
     _align_raster, _extract_bands, _merge_bands, _read_array, _xy_to_2d_index, _read_value_at, \
     _project_raster, _array_to_raster, _set_no_data, _set_data_type
@@ -22,15 +21,19 @@
 from pyrasta.tools.merge import _merge
 from pyrasta.tools.polygonize import _polygonize
 from pyrasta.tools.rasterize import _rasterize
 from pyrasta.tools.stats import _histogram, _zonal_stats
 from pyrasta.tools.windows import _windowing
 from pyrasta.utils import lazyproperty, grid, MP_CHUNK_SIZE
 
-import gdal
+try:
+    from osgeo import gdal, ogr
+except ImportError:
+    import gdal
+    import ogr
 
 gdal.UseExceptions()
 
 
 class RasterBase:
 
     def __init__(self, src_file):
```

### Comparing `pyrasta-1.3.8/pyrasta/crs.py` & `pyrasta-1.3.9/pyrasta/crs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # -*- coding: utf-8 -*-
 
 """ Functions related to CRS conversion and computation
 
 More detailed description.
 """
 
-import osr
+try:
+    from osgeo import osr
+except ImportError:
+    import osr
+
 import pyproj
 
 
 def is_equal_proj(proj1, proj2):
     """ Compare 2 projections
 
     Parameters
```

### Comparing `pyrasta-1.3.8/pyrasta/utils.py` & `pyrasta-1.3.9/pyrasta/utils.py`

 * *Files identical despite different names*

### Comparing `pyrasta-1.3.8/pyrasta/tools/filters.py` & `pyrasta-1.3.9/pyrasta/tools/filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # -*- coding: utf-8 -*-
 
 """ Module summary description.
 
 More detailed description.
 """
-import gdal
 from pyrasta.tools import _clone_gdal_dataset, _return_raster
 from pyrasta.utils import gdal_progress_bar
 
+try:
+    from osgeo import gdal
+except ImportError:
+    import gdal
+
 
 @_return_raster
 def _sieve(raster, out_file, threshold, connectedness, progress_bar):
     """ Apply sieve filter to raster
 
     Parameters
     ----------
```

### Comparing `pyrasta-1.3.8/pyrasta/tools/windows.py` & `pyrasta-1.3.9/pyrasta/tools/windows.py`

 * *Files identical despite different names*

### Comparing `pyrasta-1.3.8/pyrasta/tools/conversion.py` & `pyrasta-1.3.9/pyrasta/tools/conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 
 More detailed description.
 """
 from pyrasta.crs import srs_from
 from pyrasta.io_.files import VrtTempFile, _copy_to_file
 from pyrasta.tools import _gdal_temp_dataset, _return_raster, _clone_gdal_dataset
 
-# from osgeo import gdal_array
-
 import affine
-import gdal
 from pyrasta.tools.mapping import NUMPY_TO_GDAL
 
 
+try:
+    from osgeo import gdal
+except ImportError:
+    import gdal
+
+
 @_return_raster
 def _align_raster(in_raster, out_file, on_raster):
     """ Align raster on other raster
 
     """
     out_ds = _gdal_temp_dataset(out_file, in_raster._gdal_driver,
                                 on_raster._gdal_dataset.GetProjection(),
```

### Comparing `pyrasta-1.3.8/pyrasta/tools/rasterize.py` & `pyrasta-1.3.9/pyrasta/tools/rasterize.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,21 @@
 
 More detailed description.
 """
 from pyrasta.io_ import ESRI_DRIVER
 from pyrasta.io_.files import ShapeTempFile
 from pyrasta.tools import _gdal_temp_dataset, _return_raster
 
-import gdal
 from pyrasta.utils import gdal_progress_bar
 
+try:
+    from osgeo import gdal
+except ImportError:
+    import gdal
+
 
 @_return_raster
 def _rasterize(raster_class, out_file, gdal_driver, geodataframe,
                burn_values, attribute, projection, x_size, y_size,
                nb_band, geo_transform, data_type, no_data, all_touched,
                progress_bar):
     """ Rasterize geographic layer
```

### Comparing `pyrasta-1.3.8/pyrasta/tools/calculator.py` & `pyrasta-1.3.9/pyrasta/tools/calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 
 from pyrasta.tools import _gdal_temp_dataset, _return_raster, _clone_gdal_dataset
 from pyrasta.tools.mapping import GDAL_TO_NUMPY
 from pyrasta.tools.windows import get_block_windows, get_xy_block_windows
 from pyrasta.utils import split_into_chunks
 from tqdm import tqdm
 
-import gdal
+try:
+    from osgeo import gdal
+except ImportError:
+    import gdal
 
 OP_WINDOW_SIZE = 1000
 
 
 @_return_raster
 def _log(raster, out_file):
```

### Comparing `pyrasta-1.3.8/pyrasta/tools/mapping.py` & `pyrasta-1.3.9/pyrasta/tools/mapping.py`

 * *Files identical despite different names*

### Comparing `pyrasta-1.3.8/pyrasta/tools/dem.py` & `pyrasta-1.3.9/pyrasta/tools/dem.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 
 """ Digital Elevation Model functions
 
 More detailed description.
 """
 from pyrasta.tools import _return_raster
 
-import gdal
+try:
+    from osgeo import gdal
+except ImportError:
+    import gdal
 
 
 @_return_raster
 def _slope(dem, out_file, slope_format, scale):
     """ Compute DEM slope
 
     Parameters
```

### Comparing `pyrasta-1.3.8/pyrasta/tools/clip.py` & `pyrasta-1.3.9/pyrasta/tools/clip.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 
 More detailed description.
 """
 from pyrasta.io_ import ESRI_DRIVER
 from pyrasta.io_.files import RasterTempFile, ShapeTempFile
 from pyrasta.tools import _return_raster, _gdal_temp_dataset
 
-import gdal
+try:
+    from osgeo import gdal
+except ImportError:
+    import gdal
 
 
 @_return_raster
 def _clip_raster_by_extent(raster, out_file, bounds, no_data):
     """ Clip raster by extent
 
     Parameters
```

### Comparing `pyrasta-1.3.8/pyrasta/tools/stats.py` & `pyrasta-1.3.9/pyrasta/tools/stats.py`

 * *Files identical despite different names*

### Comparing `pyrasta-1.3.8/pyrasta/tools/polygonize.py` & `pyrasta-1.3.9/pyrasta/tools/polygonize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # -*- coding: utf-8 -*-
 
 """ Module summary description.
 
 More detailed description.
 """
-import math
-
-import gdal
-import ogr
 from pyrasta.crs import srs_from
 from pyrasta.utils import gdal_progress_bar
 
+try:
+    from osgeo import gdal, ogr
+except ImportError:
+    import gdal
+    import ogr
+
 
 def _polygonize(raster, filename, band, layer_name,
                 field_name, ogr_driver, is_8_connected,
                 progress_bar):
     """ Polygonize raster
 
     Parameters
```

### Comparing `pyrasta-1.3.8/pyrasta/tools/srtm.py` & `pyrasta-1.3.9/pyrasta/tools/srtm.py`

 * *Files identical despite different names*

### Comparing `pyrasta-1.3.8/pyrasta/tools/__init__.py` & `pyrasta-1.3.9/pyrasta/tools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 More detailed description.
 """
 
 from functools import wraps
 
 from pyrasta.io_.files import RasterTempFile
 
-import gdal
+try:
+    from osgeo import gdal
+except ImportError:
+    import gdal
 
 
 def _return_raster(function):
     @wraps(function)
     def return_raster(raster, *args, **kwargs):
         try:
             with RasterTempFile(raster._gdal_driver.GetMetadata()['DMD_EXTENSION']) as out_file:
```

### Comparing `pyrasta-1.3.8/README.md` & `pyrasta-1.3.9/README.md`

 * *Files identical despite different names*

