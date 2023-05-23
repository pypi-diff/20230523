# Comparing `tmp/ssb_sgis-0.2.0.tar.gz` & `tmp/ssb_sgis-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_sgis-0.2.0.tar", max compression
+gzip compressed data, was "ssb_sgis-0.2.1.tar", max compression
```

## Comparing `ssb_sgis-0.2.0.tar` & `ssb_sgis-0.2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1074 2023-05-16 11:10:02.287542 ssb_sgis-0.2.0/LICENSE
--rw-r--r--   0        0        0     7543 2023-05-16 11:10:02.287542 ssb_sgis-0.2.0/README.md
--rw-r--r--   0        0        0     2539 2023-05-16 11:10:18.679628 ssb_sgis-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2230 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/__init__.py
--rw-r--r--   0        0        0     3243 2023-05-16 11:10:18.679628 ssb_sgis-0.2.0/src/sgis/dapla.py
--rw-r--r--   0        0        0      666 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/geopandas_tools/__init__.py
--rw-r--r--   0        0        0     8028 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/geopandas_tools/buffer_dissolve_explode.py
--rw-r--r--   0        0        0    23937 2023-05-16 11:10:18.679628 ssb_sgis-0.2.0/src/sgis/geopandas_tools/general.py
--rw-r--r--   0        0        0     5480 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/geopandas_tools/geometry_types.py
--rw-r--r--   0        0        0    14520 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/geopandas_tools/neighbors.py
--rw-r--r--   0        0        0    11815 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/geopandas_tools/overlay.py
--rw-r--r--   0        0        0     6888 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/geopandas_tools/point_operations.py
--rw-r--r--   0        0        0    10556 2023-05-16 11:10:18.679628 ssb_sgis-0.2.0/src/sgis/geopandas_tools/polygon_operations.py
--rw-r--r--   0        0        0     9722 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/geopandas_tools/to_geodataframe.py
--rw-r--r--   0        0        0     2674 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/helpers.py
--rw-r--r--   0        0        0        0 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/maps/__init__.py
--rw-r--r--   0        0        0    20212 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/maps/explore.py
--rw-r--r--   0        0        0     1938 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/maps/httpserver.py
--rw-r--r--   0        0        0    20499 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/maps/legend.py
--rw-r--r--   0        0        0    17556 2023-05-16 11:10:18.679628 ssb_sgis-0.2.0/src/sgis/maps/map.py
--rw-r--r--   0        0        0    16124 2023-05-16 11:10:18.679628 ssb_sgis-0.2.0/src/sgis/maps/maps.py
--rw-r--r--   0        0        0    14132 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/maps/thematicmap.py
--rw-r--r--   0        0        0        0 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/__init__.py
--rw-r--r--   0        0        0     6218 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/_get_route.py
--rw-r--r--   0        0        0     2017 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/_od_cost_matrix.py
--rw-r--r--   0        0        0     4206 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/_points.py
--rw-r--r--   0        0        0     4487 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/_service_area.py
--rw-r--r--   0        0        0    12433 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/closing_network_holes.py
--rw-r--r--   0        0        0    11984 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/cutting_lines.py
--rw-r--r--   0        0        0     9375 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/directednetwork.py
--rw-r--r--   0        0        0     3359 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/finding_isolated_networks.py
--rw-r--r--   0        0        0     7686 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/network.py
--rw-r--r--   0        0        0    66761 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/networkanalysis.py
--rw-r--r--   0        0        0    12643 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/networkanalysisrules.py
--rw-r--r--   0        0        0     6740 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/nodes.py
--rw-r--r--   0        0        0        0 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/py.typed
--rw-r--r--   0        0        0     3774 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/read_parquet.py
--rw-r--r--   0        0        0     8831 1970-01-01 00:00:00.000000 ssb_sgis-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-23 16:35:45.984323 ssb_sgis-0.2.1/LICENSE
+-rw-r--r--   0        0        0     7543 2023-05-23 16:35:45.984323 ssb_sgis-0.2.1/README.md
+-rw-r--r--   0        0        0     2539 2023-05-23 16:36:01.756300 ssb_sgis-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2230 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/__init__.py
+-rw-r--r--   0        0        0     3243 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/dapla.py
+-rw-r--r--   0        0        0      576 2023-05-23 16:36:01.756300 ssb_sgis-0.2.1/src/sgis/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/geopandas_tools/__init__.py
+-rw-r--r--   0        0        0     8028 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/geopandas_tools/buffer_dissolve_explode.py
+-rw-r--r--   0        0        0    23937 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/geopandas_tools/general.py
+-rw-r--r--   0        0        0     5480 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/geopandas_tools/geometry_types.py
+-rw-r--r--   0        0        0    14520 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/geopandas_tools/neighbors.py
+-rw-r--r--   0        0        0    11815 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/geopandas_tools/overlay.py
+-rw-r--r--   0        0        0     6888 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/geopandas_tools/point_operations.py
+-rw-r--r--   0        0        0    13790 2023-05-23 16:36:01.756300 ssb_sgis-0.2.1/src/sgis/geopandas_tools/polygon_operations.py
+-rw-r--r--   0        0        0     9722 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/geopandas_tools/to_geodataframe.py
+-rw-r--r--   0        0        0     2674 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/helpers.py
+-rw-r--r--   0        0        0        0 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/maps/__init__.py
+-rw-r--r--   0        0        0    20484 2023-05-23 16:36:01.756300 ssb_sgis-0.2.1/src/sgis/maps/explore.py
+-rw-r--r--   0        0        0     1938 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/maps/httpserver.py
+-rw-r--r--   0        0        0    20499 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/maps/legend.py
+-rw-r--r--   0        0        0    17448 2023-05-23 16:36:01.756300 ssb_sgis-0.2.1/src/sgis/maps/map.py
+-rw-r--r--   0        0        0    16009 2023-05-23 16:36:01.756300 ssb_sgis-0.2.1/src/sgis/maps/maps.py
+-rw-r--r--   0        0        0    14132 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/maps/thematicmap.py
+-rw-r--r--   0        0        0        0 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/networkanalysis/__init__.py
+-rw-r--r--   0        0        0     6218 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/networkanalysis/_get_route.py
+-rw-r--r--   0        0        0     2017 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/networkanalysis/_od_cost_matrix.py
+-rw-r--r--   0        0        0     4206 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/networkanalysis/_points.py
+-rw-r--r--   0        0        0     4487 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/networkanalysis/_service_area.py
+-rw-r--r--   0        0        0    12433 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/networkanalysis/closing_network_holes.py
+-rw-r--r--   0        0        0    11984 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/networkanalysis/cutting_lines.py
+-rw-r--r--   0        0        0     9375 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/networkanalysis/directednetwork.py
+-rw-r--r--   0        0        0     3359 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/networkanalysis/finding_isolated_networks.py
+-rw-r--r--   0        0        0     7686 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/networkanalysis/network.py
+-rw-r--r--   0        0        0    66761 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/networkanalysis/networkanalysis.py
+-rw-r--r--   0        0        0    12643 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/networkanalysis/networkanalysisrules.py
+-rw-r--r--   0        0        0     6740 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/networkanalysis/nodes.py
+-rw-r--r--   0        0        0        0 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/py.typed
+-rw-r--r--   0        0        0     3774 2023-05-23 16:35:46.020323 ssb_sgis-0.2.1/src/sgis/read_parquet.py
+-rw-r--r--   0        0        0     8831 1970-01-01 00:00:00.000000 ssb_sgis-0.2.1/PKG-INFO
```

### Comparing `ssb_sgis-0.2.0/LICENSE` & `ssb_sgis-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/README.md` & `ssb_sgis-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/pyproject.toml` & `ssb_sgis-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-sgis"
-version = "0.2.0"
+version = "0.2.1"
 description = "GIS functions used at Statistics Norway."
 authors = ["Statistics Norway <ort@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "sgis", from = "src"}]
 homepage = "https://github.com/statisticsnorway/ssb-sgis"
 repository = "https://github.com/statisticsnorway/ssb-sgis"
```

### Comparing `ssb_sgis-0.2.0/src/sgis/__init__.py` & `ssb_sgis-0.2.1/src/sgis/__init__.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/dapla.py` & `ssb_sgis-0.2.1/src/sgis/dapla.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/exceptions.py` & `ssb_sgis-0.2.1/src/sgis/exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,11 +15,7 @@
             f"No {self.what} within specified 'search_tolerance' "
             f"of {self.search_tolerance}"
         )
 
 
 class ZeroLinesError(Exception):
     """DataFrame has 0 rows."""
-
-
-class NotInJupyterError(Exception):
-    """This functionality only works in Jupyter."""
```

### Comparing `ssb_sgis-0.2.0/src/sgis/geopandas_tools/buffer_dissolve_explode.py` & `ssb_sgis-0.2.1/src/sgis/geopandas_tools/buffer_dissolve_explode.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/geopandas_tools/general.py` & `ssb_sgis-0.2.1/src/sgis/geopandas_tools/general.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/geopandas_tools/geometry_types.py` & `ssb_sgis-0.2.1/src/sgis/geopandas_tools/geometry_types.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/geopandas_tools/neighbors.py` & `ssb_sgis-0.2.1/src/sgis/geopandas_tools/neighbors.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/geopandas_tools/overlay.py` & `ssb_sgis-0.2.1/src/sgis/geopandas_tools/overlay.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/geopandas_tools/point_operations.py` & `ssb_sgis-0.2.1/src/sgis/geopandas_tools/point_operations.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/geopandas_tools/polygon_operations.py` & `ssb_sgis-0.2.1/src/sgis/geopandas_tools/polygon_operations.py`

 * *Files 20% similar despite different names*

```diff
@@ -40,14 +40,88 @@
         cluster_col: Name of the resulting cluster column.
         explode: Whether to explode the geometries to singlepart before the spatial
             join. Defaults to True. Index will be preserved.
 
     Returns:
         One or more GeoDataFrames (same amount as was given) with a new cluster column.
 
+    Examples
+    --------
+
+    Create polygon geometries where row 0, 1 and 2 overlap, 3 and 4 overlap
+    and 6 is on its own.
+
+    >>> import sgis as sg
+    >>> gdf = sg.to_gdf([(0, 0), (1, 1), (0, 1), (4, 4), (4, 3), (7, 7)])
+    >>> buffered = sg.buff(gdf, 1)
+    >>> gdf
+                                                geometry
+    0  POLYGON ((1.00000 0.00000, 0.99951 -0.03141, 0...
+    1  POLYGON ((2.00000 1.00000, 1.99951 0.96859, 1....
+    2  POLYGON ((1.00000 1.00000, 0.99951 0.96859, 0....
+    3  POLYGON ((5.00000 4.00000, 4.99951 3.96859, 4....
+    4  POLYGON ((5.00000 3.00000, 4.99951 2.96859, 4....
+    5  POLYGON ((8.00000 7.00000, 7.99951 6.96859, 7....
+
+    This will add a cluster column to the GeoDataFrame:
+
+    >>> gdf = sg.get_polygon_clusters(gdf, cluster_col="cluster")
+    >>> gdf
+       cluster                                           geometry
+    0        0  POLYGON ((1.00000 0.00000, 0.99951 -0.03141, 0...
+    1        0  POLYGON ((2.00000 1.00000, 1.99951 0.96859, 1....
+    2        0  POLYGON ((1.00000 1.00000, 0.99951 0.96859, 0....
+    3        1  POLYGON ((5.00000 4.00000, 4.99951 3.96859, 4....
+    4        1  POLYGON ((5.00000 3.00000, 4.99951 2.96859, 4....
+    5        2  POLYGON ((8.00000 7.00000, 7.99951 6.96859, 7....
+
+    If multiple GeoDataFrames are given, all are returned with common
+    cluster values.
+
+    >>> gdf2 = sg.to_gdf([(0, 0), (7, 7)])
+    >>> gdf, gdf2 = sg.get_polygon_clusters(gdf, gdf2, cluster_col="cluster")
+    >>> gdf2
+    cluster                 geometry
+    0        0  POINT (0.00000 0.00000)
+    1        2  POINT (7.00000 7.00000)
+    >>> gdf
+       cluster                                           geometry
+    0        0  POLYGON ((1.00000 0.00000, 0.99951 -0.03141, 0...
+    1        0  POLYGON ((2.00000 1.00000, 1.99951 0.96859, 1....
+    2        0  POLYGON ((1.00000 1.00000, 0.99951 0.96859, 0....
+    3        1  POLYGON ((5.00000 4.00000, 4.99951 3.96859, 4....
+    4        1  POLYGON ((5.00000 3.00000, 4.99951 2.96859, 4....
+    5        2  POLYGON ((8.00000 7.00000, 7.99951 6.96859, 7....
+
+    Dissolving 'by' the cluster column will make the dissolve much
+    faster if there are a lot of non-overlapping polygons.
+
+    >>> dissolved = gdf.dissolve(by="cluster", as_index=False)
+    >>> dissolved
+       cluster                                           geometry
+    0        0  POLYGON ((0.99951 -0.03141, 0.99803 -0.06279, ...
+    1        1  POLYGON ((4.99951 2.96859, 4.99803 2.93721, 4....
+    2        2  POLYGON ((8.00000 7.00000, 7.99951 6.96859, 7....
+
+    Which is equivelen to this in straigt geopandas:
+
+    >>> dissolved2 = gdf.dissolve().explode(ignore_index=True).assign(cluster=lambda x: x.index)
+    >>> dissolved2
+       cluster                                           geometry
+    0        0  POLYGON ((0.99803 -0.06279, 0.99556 -0.09411, ...
+    1        1  POLYGON ((4.99803 2.93721, 4.99556 2.90589, 4....
+    2        2  POLYGON ((7.99556 6.90589, 7.99211 6.87467, 7....
+
+    Note that the order of the coordinates is different, and there is
+    some deviations in the rounding on microscopic levels.
+
+    >>> dissolved.area.sum()
+    15.016909720698278
+    >>> dissolved2.area.sum()
+    15.016909720698285
     """
     if isinstance(gdfs[-1], str):
         *gdfs, cluster_col = gdfs
 
     concated = pd.DataFrame()
     for i, gdf in enumerate(gdfs):
         if isinstance(gdf, GeoSeries):
```

### Comparing `ssb_sgis-0.2.0/src/sgis/geopandas_tools/to_geodataframe.py` & `ssb_sgis-0.2.1/src/sgis/geopandas_tools/to_geodataframe.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/helpers.py` & `ssb_sgis-0.2.1/src/sgis/helpers.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/maps/explore.py` & `ssb_sgis-0.2.1/src/sgis/maps/explore.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import branca as bc
 import folium
 import matplotlib
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame
+from IPython.core.display import display
 from shapely.geometry import LineString
 
 from ..geopandas_tools.general import clean_geoms, random_points_in_polygons
 from ..geopandas_tools.geometry_types import get_geom_type
 from ..geopandas_tools.to_geodataframe import to_gdf
 from .httpserver import run_html_server
 from .map import Map
@@ -62,27 +63,29 @@
 class Explore(Map):
     def __init__(
         self,
         *gdfs,
         column: str | None = None,
         popup: bool = True,
         max_zoom: int = 30,
+        smooth_factor: 2.5,
         browser: bool = False,
         **kwargs,
     ):
         self.browser = browser
         if not self.browser and "show_in_browser" in kwargs:
             self.browser = kwargs.pop("show_in_browser")
         if not self.browser and "in_browser" in kwargs:
             self.browser = kwargs.pop("in_browser")
 
         super().__init__(*gdfs, column=column, **kwargs)
 
         self.popup = popup
         self.max_zoom = max_zoom
+        self.smooth_factor = smooth_factor
 
         self._to_single_geom_type()
 
         if self._is_categorical:
             if len(self.gdfs) == 1:
                 self._split_categories()
         else:
@@ -242,29 +245,32 @@
             popup=self.popup,
             **self.kwargs,
         )
 
         for gdf, label in zip(self._gdfs, self.labels, strict=True):
             if not len(gdf):
                 continue
+
             f = folium.FeatureGroup(name=label)
 
             gjs = self._explore_return(
                 gdf,
                 color=gdf["color"],
                 return_="geojson",
                 tooltip=self._tooltip_cols(gdf),
+                popup=self.popup,
                 **{
                     key: value
                     for key, value in self.kwargs.items()
                     if key not in ["title"]
                 },
             )
             f.add_child(gjs)
             self.map.add_child(f)
+
         _categorical_legend(
             self.map,
             self._column,
             self._categories_colors_dict.keys(),
             self._categories_colors_dict.values(),
         )
         folium.TileLayer("stamentoner").add_to(self.map)
@@ -289,15 +295,14 @@
 
         colorbar = bc.colormap.StepColormap(
             unique_colors,
             vmin=self._gdf[self._column].min(),
             vmax=self._gdf[self._column].max(),
             caption=self._column,
             index=self.bins,
-            #  **colormap_kwds,
         )
 
         for gdf, label in zip(self._gdfs, self.labels, strict=True):
             if not len(gdf):
                 continue
             f = folium.FeatureGroup(name=label)
 
@@ -305,14 +310,15 @@
             colorarray = unique_colors[classified]
 
             gjs = self._explore_return(
                 gdf,
                 tooltip=self._tooltip_cols(gdf),
                 color=colorarray,
                 return_="geojson",
+                popup=self.popup,
                 **{key: value for key, value in self.kwargs.items() if key != "title"},
             )
             f.add_child(gjs)
             self.map.add_child(f)
 
         self.map.add_child(colorbar)
         folium.TileLayer("stamentoner").add_to(self.map)
@@ -412,14 +418,16 @@
 
             if isinstance(tiles, xyzservices.TileProvider):
                 attr = attr if attr else tiles.html_attribution
                 map_kwds["min_zoom"] = tiles.get("min_zoom", 0)
                 map_kwds["max_zoom"] = tiles.get("max_zoom", 30)
                 tiles = tiles.build_url(scale_factor="{r}")
 
+            map_kwds["zoom_start"] = self.kwargs.get("zoom_start", 15)
+
             m = folium.Map(
                 location=location,
                 control_scale=control_scale,
                 tiles=tiles,
                 attr=attr,
                 width=width,
                 height=height,
@@ -518,14 +526,15 @@
             gjs = folium.GeoJson(
                 gdf.__geo_interface__,
                 tooltip=tooltip,
                 popup=popup,
                 marker=marker,
                 style_function=style_function,
                 highlight_function=highlight_function,
+                smooth_factor=self.smooth_factor,
                 **kwargs,
             )
             return gjs
 
         return m
```

### Comparing `ssb_sgis-0.2.0/src/sgis/maps/httpserver.py` & `ssb_sgis-0.2.1/src/sgis/maps/httpserver.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/maps/legend.py` & `ssb_sgis-0.2.1/src/sgis/maps/legend.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/maps/map.py` & `ssb_sgis-0.2.1/src/sgis/maps/map.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,26 +27,24 @@
 
 # custom default colors for non-numeric data, because the geopandas default has very
 # similar colors. The palette is like the "Set2" cmap from matplotlib, but with more
 # colors. If more than 14 categories, the geopandas default cmap is used.
 _CATEGORICAL_CMAP = {
     0: "#4576ff",
     1: "#ff455e",
-    2: "#59d45f",
-    3: "#b51d8b",
-    4: "#ffa514",
-    5: "#f2dc4e",
-    6: "#ff8cc9",
-    7: "#6bf2eb",
-    8: "#916209",
-    9: "#008d94",
-    10: "#8a030a",
-    11: "#9c65db",
-    12: "#228000",
-    13: "#80ff00",
+    2: "#ffa617",
+    3: "#ff8cc9",
+    4: "#804e00",
+    5: "#99ff00",
+    6: "#fff700",
+    7: "#00ffee",
+    8: "#36d19b",
+    9: "#94006b",
+    10: "#750000",
+    11: "#1c6b00",
 }
 
 
 class Map:
     """Base class that prepares one or more GeoDataFrames for mapping.
 
     The class has no public methods.
@@ -231,15 +229,14 @@
 
         if self.scheme is None:
             return
 
         if not self.bins:
             self.bins = self._create_bins(self._gdf, self._column)
             if len(self.bins) <= self._k and len(self.bins) != len(self._unique_values):
-                warnings.warn(f"Could not create {self._k} classes.")
                 self._k = len(self.bins)
         else:
             self.bins = self._add_minmax_to_bins(self.bins)
             if len(self._unique_values) <= len(self.bins):
                 self._k = len(self.bins)  # - 1
 
     def _get_labels(self, gdfs: tuple[GeoDataFrame]) -> None:
```

### Comparing `ssb_sgis-0.2.0/src/sgis/maps/maps.py` & `ssb_sgis-0.2.1/src/sgis/maps/maps.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,56 +7,42 @@
 The 'qtm' function shows a simple static map of one or more GeoDataFrames.
 """
 from numbers import Number
 
 from geopandas import GeoDataFrame, GeoSeries
 from shapely import Geometry
 
-from ..exceptions import NotInJupyterError
 from ..geopandas_tools.general import clean_clip, random_points_in_polygons, to_gdf
 from ..geopandas_tools.geometry_types import get_geom_type
 from ..helpers import make_namedict
 from .explore import Explore
 from .map import Map
 from .thematicmap import ThematicMap
 
 
-def _check_if_jupyter_is_needed(explore, browser):
-    if explore and not browser:
-        try:
-            display
-        except NameError as e:
-            raise NotInJupyterError(
-                "Cannot display interactive map. Try setting "
-                "'browser' to True, or 'explore' to False."
-            ) from e
-
-
-def _get_mask(kwargs: dict, crs) -> tuple[GeoDataFrame, dict | None, dict]:
+def _get_mask(kwargs: dict, crs) -> tuple[GeoDataFrame | None, dict]:
     masks = {
         "bygdoy": (10.6976899, 59.9081695),
-        "Bygdoy": (10.6976899, 59.9081695),
         "kongsvinger": (12.0035242, 60.1875279),
-        "Kongsvinger": (12.0035242, 60.1875279),
         "stavanger": (5.6960601, 58.8946196),
-        "Stavanger": (5.6960601, 58.8946196),
     }
 
     if "size" in kwargs and kwargs["size"] is not None:
         size = kwargs["size"]
     else:
         size = 1000
 
     for key, value in kwargs.items():
-        if key in masks:
+        if key.lower() in masks:
             mask = masks[key]
             kwargs.pop(key)
             if isinstance(value, Number) and value > 1:
                 size = value
-            return to_gdf([mask], crs=4326).to_crs(crs).buffer(size), kwargs
+            the_mask = to_gdf([mask], crs=4326).to_crs(crs).buffer(size)
+            return the_mask, kwargs
 
     return None, kwargs
 
 
 def explore(
     *gdfs: GeoDataFrame,
     column: str | None = None,
@@ -121,37 +107,56 @@
     With additional arguments.
 
     >>> roads["meters"] = roads.length
     >>> points["meters"] = points.length
     >>> explore(roads, points, column="meters", cmap="plasma", max_zoom=60)
     """
     mask, kwargs = _get_mask(kwargs | {"size": size}, crs=gdfs[0].crs)
+
     kwargs.pop("size", None)
+
     if mask is not None:
         return clipmap(
             *gdfs,
             column=column,
             mask=mask,
             labels=labels,
             browser=browser,
             max_zoom=max_zoom,
             **kwargs,
         )
 
+    if center is not None:
+        size = size if size else 1000
+        if not isinstance(center, GeoDataFrame):
+            mask = to_gdf(center, crs=gdfs[0].crs).buffer(size)
+        elif get_geom_type(center) == "point":
+            mask = center.buffer(size)
+
+        return clipmap(
+            *gdfs,
+            column=column,
+            mask=mask,
+            labels=labels,
+            browser=browser,
+            max_zoom=max_zoom,
+            **kwargs,
+        )
+
     m = Explore(
         *gdfs,
         column=column,
         labels=labels,
         browser=browser,
         max_zoom=max_zoom,
         smooth_factor=smooth_factor,
         **kwargs,
     )
 
-    m.explore(center=center, size=size)
+    m.explore()
 
 
 def samplemap(
     *gdfs: GeoDataFrame,
     column: str | None = None,
     size: int = 1000,
     sample_from_first: bool = True,
@@ -214,15 +219,14 @@
     >>> samplemap(roads, points)
 
     Sample area with a radius of 5 kilometers.
 
     >>> samplemap(roads, points, size=5_000, column="meters")
 
     """
-    _check_if_jupyter_is_needed(explore, browser)
 
     if not size and isinstance(gdfs[-1], (float, int)):
         *gdfs, size = gdfs
 
     mask, kwargs = _get_mask(kwargs | {"size": size}, crs=gdfs[0].crs)
     kwargs.pop("size")
 
@@ -313,15 +317,15 @@
 def clipmap(
     *gdfs: GeoDataFrame,
     column: str | None = None,
     mask: GeoDataFrame | GeoSeries | Geometry = None,
     labels: tuple[str] | None = None,
     explore: bool = True,
     max_zoom: int = 30,
-    smooth_factor: int = 1.5,
+    smooth_factor: int | float = 1.5,
     browser: bool = False,
     **kwargs,
 ) -> None:
     """Shows an interactive map of a of GeoDataFrames clipped to the mask extent.
 
     It takes all the GeoDataFrames specified, clips them to the extent of the mask,
     and displays the resulting geometries in an interactive map with a common legends.
@@ -354,16 +358,14 @@
 
     See also
     --------
     explore: same functionality, but shows the entire area of the geometries.
     samplemap: same functionality, but shows only a random area of a given size.
     """
 
-    _check_if_jupyter_is_needed(explore, browser)
-
     gdfs, column = Explore._separate_args(gdfs, column)
 
     clipped, kwargs = _prepare_clipmap(
         *gdfs,
         mask=mask,
         labels=labels,
         **kwargs,
```

### Comparing `ssb_sgis-0.2.0/src/sgis/maps/thematicmap.py` & `ssb_sgis-0.2.1/src/sgis/maps/thematicmap.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/networkanalysis/_get_route.py` & `ssb_sgis-0.2.1/src/sgis/networkanalysis/_get_route.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/networkanalysis/_od_cost_matrix.py` & `ssb_sgis-0.2.1/src/sgis/networkanalysis/_od_cost_matrix.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/networkanalysis/_points.py` & `ssb_sgis-0.2.1/src/sgis/networkanalysis/_points.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/networkanalysis/_service_area.py` & `ssb_sgis-0.2.1/src/sgis/networkanalysis/_service_area.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/networkanalysis/closing_network_holes.py` & `ssb_sgis-0.2.1/src/sgis/networkanalysis/closing_network_holes.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/networkanalysis/cutting_lines.py` & `ssb_sgis-0.2.1/src/sgis/networkanalysis/cutting_lines.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/networkanalysis/directednetwork.py` & `ssb_sgis-0.2.1/src/sgis/networkanalysis/directednetwork.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/networkanalysis/finding_isolated_networks.py` & `ssb_sgis-0.2.1/src/sgis/networkanalysis/finding_isolated_networks.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/networkanalysis/network.py` & `ssb_sgis-0.2.1/src/sgis/networkanalysis/network.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/networkanalysis/networkanalysis.py` & `ssb_sgis-0.2.1/src/sgis/networkanalysis/networkanalysis.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/networkanalysis/networkanalysisrules.py` & `ssb_sgis-0.2.1/src/sgis/networkanalysis/networkanalysisrules.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/networkanalysis/nodes.py` & `ssb_sgis-0.2.1/src/sgis/networkanalysis/nodes.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/src/sgis/read_parquet.py` & `ssb_sgis-0.2.1/src/sgis/read_parquet.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.0/PKG-INFO` & `ssb_sgis-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-sgis
-Version: 0.2.0
+Version: 0.2.1
 Summary: GIS functions used at Statistics Norway.
 Home-page: https://github.com/statisticsnorway/ssb-sgis
 License: MIT
 Author: Statistics Norway
 Author-email: ort@ssb.no
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 3 - Alpha
```

