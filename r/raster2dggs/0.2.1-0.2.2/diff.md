# Comparing `tmp/raster2dggs-0.2.1.tar.gz` & `tmp/raster2dggs-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster2dggs-0.2.1.tar", max compression
+gzip compressed data, was "raster2dggs-0.2.2.tar", max compression
```

## Comparing `raster2dggs-0.2.1.tar` & `raster2dggs-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     8424 2023-05-19 04:54:29.612237 raster2dggs-0.2.1/README.md
--rw-r--r--   0        0        0     1091 2023-05-19 04:54:52.024349 raster2dggs-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       27 2023-05-03 02:59:48.530270 raster2dggs-0.2.1/raster2dggs/__init__.py
--rw-r--r--   0        0        0      599 2023-05-03 02:59:13.750096 raster2dggs-0.2.1/raster2dggs/cli.py
--rw-r--r--   0        0        0    15766 2023-05-19 04:52:32.967656 raster2dggs-0.2.1/raster2dggs/h3.py
--rw-r--r--   0        0        0     9843 1970-01-01 00:00:00.000000 raster2dggs-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     8424 2023-05-22 23:16:34.972155 raster2dggs-0.2.2/README.md
+-rw-r--r--   0        0        0     1091 2023-05-22 23:16:41.480189 raster2dggs-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-05-03 02:59:48.530270 raster2dggs-0.2.2/raster2dggs/__init__.py
+-rw-r--r--   0        0        0      599 2023-05-03 02:59:13.750096 raster2dggs-0.2.2/raster2dggs/cli.py
+-rw-r--r--   0        0        0    16047 2023-05-22 23:16:08.684017 raster2dggs-0.2.2/raster2dggs/h3.py
+-rw-r--r--   0        0        0     9843 1970-01-01 00:00:00.000000 raster2dggs-0.2.2/PKG-INFO
```

### Comparing `raster2dggs-0.2.1/README.md` & `raster2dggs-0.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -148,17 +148,17 @@
 ## Citation
 
 ```bibtex
 @software{raster2dggs,
   title={{raster2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/raster2dggs},
-  version={0.2.1},
+  version={0.2.2},
   date={2023-02-09}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). raster2dggs (0.2.1) [Computer software]. https://github.com/manaakiwhenua/raster2dggs 
+> Ardo, J., & Law, R. (2023). raster2dggs (0.2.2) [Computer software]. https://github.com/manaakiwhenua/raster2dggs 
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/raster2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

### Comparing `raster2dggs-0.2.1/pyproject.toml` & `raster2dggs-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "raster2dggs"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["James Ardo <ardoj@landcareresearch.co.nz>"]
 maintainers = ["Richard Law <lawr@landcareresearch.co.nz>"]
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 repository = "https://github.com/manaakiwhenua/raster2dggs"
 keywords = ["dggs", "raster", "h3", "cli"]
```

### Comparing `raster2dggs-0.2.1/raster2dggs/cli.py` & `raster2dggs-0.2.2/raster2dggs/cli.py`

 * *Files identical despite different names*

### Comparing `raster2dggs-0.2.1/raster2dggs/h3.py` & `raster2dggs-0.2.2/raster2dggs/h3.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import multiprocessing
 from numbers import Number
 import numpy as np
 from pathlib import Path
 import tempfile
 import threading
-from typing import Tuple, Union
+from typing import Callable, Tuple, Union
 from urllib.parse import urlparse
 
 import click
 import click_log
 import dask
 import dask.dataframe as dd
 import h3pandas  # Necessary import despite lack of explicit use
@@ -215,15 +215,15 @@
 
             LOGGER.debug("Stage 1 (primary indexing) complete")
             return _address_boundary_issues(
                 tmpdir, output, resolution, parent_res, **kwargs
             )
 
 
-def _h3_parent_groupby(df, resolution: int, aggfunc: str, decimals: int):
+def _h3_parent_groupby(df, resolution: int, aggfunc: Union[str, Callable], decimals: int):
     """
     Function for aggregating the h3 resolution values per parent partition. Each partition will be run through with a
     pandas .groupby function. This step is to ensure there are no duplicate h3 values, which will happen when indexing a
     high resolution raster at a coarser h3 resolution.
     """
     if decimals > 0:
         return df.groupby(f"h3_{resolution:02}").agg(aggfunc).round(decimals)
@@ -338,15 +338,15 @@
     help="Number of threads to use when running in parallel. The default is determined based dynamically as the total number of available cores, minus one.",
 )
 @click.option(
     "-a",
     "--aggfunc",
     default=DEFAULTS["aggfunc"],
     type=click.Choice(
-        ["count", "mean", "sum", "prod", "std", "var", "min", "max", "median"]
+        ["count", "mean", "sum", "prod", "std", "var", "min", "max", "median", "mode"]
     ),
     help="Numpy aggregate function to apply when aggregating cell values after DGGS indexing, in case of multiple pixels mapping to the same DGGS cell.",
 )
 @click.option(
     "-d",
     "--decimals",
     default=DEFAULTS["decimals"],
@@ -390,16 +390,15 @@
 ):
     """
     Ingest a raster image and index it to the H3 DGGS.
 
     RASTER_INPUT is the path to input raster data; prepend with protocol like s3:// or hdfs:// for remote data.
     OUTPUT_DIRECTORY should be a directory, not a file, as it will be the write location for an Apache Parquet data store, with partitions equivalent to parent cells of target cells at a fixed offset. However, this can also be remote (use the appropriate prefix, e.g. s3://).
     """
-    tempfile.tempdir = tempdir
-    print(tempfile.tempdir)
+    tempfile.tempdir = tempdir if tempdir is not None else tempfile.tempdir
     if parent_res is not None and not int(parent_res) < int(resolution):
         raise ParentResolutionException(
             "Parent resolution ({pr}) must be less than target resolution ({r})".format(
                 pr=parent_res, r=resolution
             )
         )
     if not Path(raster_input).exists():
@@ -417,14 +416,17 @@
     warp_args: dict = {
         "resampling": Resampling._member_map_[resampling],
         "crs": crs.CRS.from_epsg(
             4326
         ),  # Input raster must be converted to WGS84 (4326) for H3 indexing
         "warp_mem_limit": warp_mem_limit,
     }
+    if aggfunc == 'mode':
+        logging.warning('Mode aggregation: arbitrary behaviour: if there is more than one mode when aggregating, only the first value will be recorded.')
+        aggfunc = lambda x: pd.Series.mode(x)[0]
     kwargs = {
         "upscale": upscale,
         "compression": compression,
         "threads": threads,
         "aggfunc": aggfunc,
         "decimals": decimals,
         "warp_mem_limit": warp_mem_limit,
```

### Comparing `raster2dggs-0.2.1/PKG-INFO` & `raster2dggs-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster2dggs
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Home-page: https://github.com/manaakiwhenua/raster2dggs
 License: LGPL-3.0-or-later
 Keywords: dggs,raster,h3,cli
 Author: James Ardo
 Author-email: ardoj@landcareresearch.co.nz
 Maintainer: Richard Law
@@ -183,18 +183,18 @@
 ## Citation
 
 ```bibtex
 @software{raster2dggs,
   title={{raster2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/raster2dggs},
-  version={0.2.1},
+  version={0.2.2},
   date={2023-02-09}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). raster2dggs (0.2.1) [Computer software]. https://github.com/manaakiwhenua/raster2dggs 
+> Ardo, J., & Law, R. (2023). raster2dggs (0.2.2) [Computer software]. https://github.com/manaakiwhenua/raster2dggs 
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/raster2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

