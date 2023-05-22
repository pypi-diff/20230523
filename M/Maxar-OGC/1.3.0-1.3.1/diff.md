# Comparing `tmp/Maxar_OGC-1.3.0.tar.gz` & `tmp/Maxar_OGC-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\ty027972\Desktop\marianas-team\marianas-team\SDKs\Python\2.0\ogc-sdk\dist\.tmp-p60a5wdm\Maxar_OGC-1.3.0.tar", last modified: Fri Jan  6 21:57:06 2023, max compression
+gzip compressed data, was "C:\Users\ty027972\Desktop\marianas-team\marianas-team\SDKs\Python\2.0\ogc-sdk\dist\.tmp-po2paudp\Maxar_OGC-1.3.1.tar", last modified: Mon May 22 22:14:53 2023, max compression
```

## Comparing `Maxar_OGC-1.3.0.tar` & `Maxar_OGC-1.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-01-06 21:57:06.000000 Maxar_OGC-1.3.0/
--rw-rw-rw-   0        0        0    15959 2023-01-03 20:19:06.000000 Maxar_OGC-1.3.0/LICENSE
--rw-rw-rw-   0        0        0    15959 2023-01-03 20:19:06.000000 Maxar_OGC-1.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2715 2023-01-06 21:57:06.000000 Maxar_OGC-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1822 2023-01-03 20:19:06.000000 Maxar_OGC-1.3.0/README.md
--rw-rw-rw-   0        0        0      102 2023-01-03 20:19:06.000000 Maxar_OGC-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-01-06 21:57:06.000000 Maxar_OGC-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1689 2023-01-06 20:07:30.000000 Maxar_OGC-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-06 21:57:06.000000 Maxar_OGC-1.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-01-06 21:57:06.000000 Maxar_OGC-1.3.0/src/Maxar_OGC/
--rw-rw-rw-   0        0        0       34 2023-01-03 20:19:06.000000 Maxar_OGC-1.3.0/src/Maxar_OGC/__init__.py
--rw-rw-rw-   0        0        0     4581 2023-01-06 19:35:00.000000 Maxar_OGC-1.3.0/src/Maxar_OGC/auth.py
--rw-rw-rw-   0        0        0    10366 2023-01-03 20:19:06.000000 Maxar_OGC-1.3.0/src/Maxar_OGC/cli_commands.py
--rw-rw-rw-   0        0        0    41855 2023-01-06 19:35:00.000000 Maxar_OGC-1.3.0/src/Maxar_OGC/interface.py
--rw-rw-rw-   0        0        0    15323 2023-01-06 19:34:53.000000 Maxar_OGC-1.3.0/src/Maxar_OGC/process.py
--rw-rw-rw-   0        0        0     3956 2023-01-06 19:34:53.000000 Maxar_OGC-1.3.0/src/Maxar_OGC/wcs.py
--rw-rw-rw-   0        0        0     5457 2023-01-06 19:34:53.000000 Maxar_OGC-1.3.0/src/Maxar_OGC/wfs.py
--rw-rw-rw-   0        0        0     3491 2023-01-06 19:34:53.000000 Maxar_OGC-1.3.0/src/Maxar_OGC/wms.py
--rw-rw-rw-   0        0        0     6409 2023-01-06 19:34:53.000000 Maxar_OGC-1.3.0/src/Maxar_OGC/wmts.py
-drwxrwxrwx   0        0        0        0 2023-01-06 21:57:06.000000 Maxar_OGC-1.3.0/src/Maxar_OGC.egg-info/
--rw-rw-rw-   0        0        0     2715 2023-01-06 21:57:06.000000 Maxar_OGC-1.3.0/src/Maxar_OGC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2023-01-06 21:57:06.000000 Maxar_OGC-1.3.0/src/Maxar_OGC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-06 21:57:06.000000 Maxar_OGC-1.3.0/src/Maxar_OGC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      292 2023-01-06 21:57:06.000000 Maxar_OGC-1.3.0/src/Maxar_OGC.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       65 2023-01-06 21:57:06.000000 Maxar_OGC-1.3.0/src/Maxar_OGC.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-01-06 21:57:06.000000 Maxar_OGC-1.3.0/src/Maxar_OGC.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 22:14:53.000000 Maxar_OGC-1.3.1/
+-rw-rw-rw-   0        0        0    15959 2023-05-22 20:40:20.000000 Maxar_OGC-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0    15959 2023-05-22 20:40:20.000000 Maxar_OGC-1.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2715 2023-05-22 22:14:53.000000 Maxar_OGC-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1822 2023-05-22 20:40:20.000000 Maxar_OGC-1.3.1/README.md
+-rw-rw-rw-   0        0        0      102 2023-05-22 20:40:20.000000 Maxar_OGC-1.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-05-22 22:14:53.000000 Maxar_OGC-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1689 2023-05-22 22:05:47.000000 Maxar_OGC-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 22:14:53.000000 Maxar_OGC-1.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 22:14:53.000000 Maxar_OGC-1.3.1/src/Maxar_OGC/
+-rw-rw-rw-   0        0        0       34 2023-05-22 20:40:20.000000 Maxar_OGC-1.3.1/src/Maxar_OGC/__init__.py
+-rw-rw-rw-   0        0        0     4581 2023-05-22 22:05:47.000000 Maxar_OGC-1.3.1/src/Maxar_OGC/auth.py
+-rw-rw-rw-   0        0        0    10366 2023-05-22 20:40:20.000000 Maxar_OGC-1.3.1/src/Maxar_OGC/cli_commands.py
+-rw-rw-rw-   0        0        0    42171 2023-05-22 21:42:46.000000 Maxar_OGC-1.3.1/src/Maxar_OGC/interface.py
+-rw-rw-rw-   0        0        0    15421 2023-05-22 20:40:20.000000 Maxar_OGC-1.3.1/src/Maxar_OGC/process.py
+-rw-rw-rw-   0        0        0     3960 2023-05-22 20:40:20.000000 Maxar_OGC-1.3.1/src/Maxar_OGC/wcs.py
+-rw-rw-rw-   0        0        0     5459 2023-05-22 20:40:20.000000 Maxar_OGC-1.3.1/src/Maxar_OGC/wfs.py
+-rw-rw-rw-   0        0        0     3493 2023-05-22 20:40:20.000000 Maxar_OGC-1.3.1/src/Maxar_OGC/wms.py
+-rw-rw-rw-   0        0        0     6379 2023-05-22 20:40:20.000000 Maxar_OGC-1.3.1/src/Maxar_OGC/wmts.py
+drwxrwxrwx   0        0        0        0 2023-05-22 22:14:53.000000 Maxar_OGC-1.3.1/src/Maxar_OGC.egg-info/
+-rw-rw-rw-   0        0        0     2715 2023-05-22 22:14:53.000000 Maxar_OGC-1.3.1/src/Maxar_OGC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2023-05-22 22:14:53.000000 Maxar_OGC-1.3.1/src/Maxar_OGC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 22:14:53.000000 Maxar_OGC-1.3.1/src/Maxar_OGC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      292 2023-05-22 22:14:53.000000 Maxar_OGC-1.3.1/src/Maxar_OGC.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       65 2023-05-22 22:14:53.000000 Maxar_OGC-1.3.1/src/Maxar_OGC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-22 22:14:53.000000 Maxar_OGC-1.3.1/src/Maxar_OGC.egg-info/top_level.txt
```

### Comparing `Maxar_OGC-1.3.0/LICENSE` & `Maxar_OGC-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Maxar_OGC-1.3.0/LICENSE.txt` & `Maxar_OGC-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Maxar_OGC-1.3.0/PKG-INFO` & `Maxar_OGC-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Maxar_OGC
-Version: 1.3.0
+Version: 1.3.1
 Summary: SDK for interacting with Maxar imagery platforms
 Author: GCS Marianas Team
 Author-email: DL-GCS-Marianas@digitalglobe.com
 License: MIT
 Project-URL: Documentation, https://cloudservices.readthedocs.io/en/latest/index.html
 Project-URL: Source, https://github.com/DigitalGlobe/CloudServices
 Keywords: OGC,WMS,WFS,WMTS,WCS,MAXAR,IMAGERY,GIS
```

### Comparing `Maxar_OGC-1.3.0/README.md` & `Maxar_OGC-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `Maxar_OGC-1.3.0/setup.py` & `Maxar_OGC-1.3.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent.resolve()
 
 README = (HERE / "README.md").read_text()
 
 setup(
   name = 'Maxar_OGC',
-  version = '1.3.0',
+  version = '1.3.1',
   license='MIT',
   description = 'SDK for interacting with Maxar imagery platforms',
   long_description=README,
   long_description_content_type="text/markdown",
   author = 'GCS Marianas Team',
   author_email = 'DL-GCS-Marianas@digitalglobe.com',
   project_urls = {
```

### Comparing `Maxar_OGC-1.3.0/src/Maxar_OGC/auth.py` & `Maxar_OGC-1.3.1/src/Maxar_OGC/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     """
 
     def __init__(self, base_url=None, connectid=None, username=None, password=None):
         self.base_url = base_url  # host name "https://securewatch.maxar.com/"
         self.connect_id = connectid
         self.username = username
         self.password = password
-        self.version = 'python_2.0_1.3.0'
+        self.version = 'python_2.0_1.3.1'
 
         if not self.base_url:
             dir_path = os.path.expanduser('~')
             file = '.ogc-config'
             full_path = os.path.join(dir_path, file)
             if os.path.isfile(full_path):
                 self.base_url, self.connect_id, self.username, self.password = self._get_environment(full_path)
```

### Comparing `Maxar_OGC-1.3.0/src/Maxar_OGC/cli_commands.py` & `Maxar_OGC-1.3.1/src/Maxar_OGC/cli_commands.py`

 * *Files identical despite different names*

### Comparing `Maxar_OGC-1.3.0/src/Maxar_OGC/interface.py` & `Maxar_OGC-1.3.1/src/Maxar_OGC/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import os
+import sys
 
 from Maxar_OGC.auth import Auth
 from Maxar_OGC.wms import WMS
 from Maxar_OGC.wfs import WFS
 from Maxar_OGC.wmts import WMTS
 from Maxar_OGC.wcs import WCS
 import Maxar_OGC.process as process
 import requests
 import warnings
+import csv
 from concurrent.futures import as_completed
 from PIL import Image
 from bs4 import BeautifulSoup as bs
 
 
 warnings.filterwarnings("ignore")
 
@@ -58,16 +60,16 @@
         Kwargs:
             featureprofile (string) = The desired stacking profile. Defaults to account Default
             typename (string) = The typename of the desired feature type. Defaults to FinishedFeature. Example input
             MaxarCatalogMosaicProducts
         Returns:
             Response is either a list of features or a shapefile of all features and associated metdata.
         """
-        if filter:
-            process.cql_checker(filter)
+        # if filter:
+        #     process.cql_checker(filter)
         if shapefile:
             result = self.wfs.search(bbox=bbox, filter=filter, srsname=srsname, outputformat='shape-zip', **kwargs)
         elif csv:
             result = self.wfs.search(bbox=bbox, filter=filter, srsname=srsname, outputformat='csv', **kwargs)
         else:
             result = self.wfs.search(bbox=bbox, filter=filter, srsname=srsname, **kwargs)
         if bbox:
@@ -386,15 +388,15 @@
         kwargs:
             outputdirectory (string) = Desired output location for tiles
             image_format (string) = Desired image format (png or jpeg)
         Returns:
             None
         """
 
-        if bbox:
+        if bbox is not None:
             process._validate_bbox(bbox, srsname=srsname)
         filter = "featureId='{}'".format(featureid)
         wfs_request = self.search(filter=filter, srsname=srsname)
         image_bbox = wfs_request[0]['geometry']['coordinates'][0]
         x_coords = [x[0] for x in image_bbox]
         y_coords = [y[1] for y in image_bbox]
 
@@ -405,15 +407,15 @@
             maxx = max(x_coords) + 0.0054932
         else:
             miny = min(y_coords)
             maxy = max(y_coords) + 468.1536
             minx = min(x_coords)
             maxx = max(x_coords) + 468.1536
 
-        if bbox:
+        if bbox is not None:
             bbox_order = bbox.split(',')
             if srsname == "EPSG:4326":
                 miny = max(miny, float(bbox_order[0]))
                 maxy = min(maxy, float(bbox_order[2])) + 0.0042176
                 minx = max(minx, float(bbox_order[1]))
                 maxx = min(maxx, float(bbox_order[3])) + 0.0054932
             else:
@@ -485,28 +487,34 @@
                                                                                                   x_list[x + 1],
                                                                                                   y_list[y + 1])
 
         print("Started full image download process...")
 
         #This section deletes bboxes that don't cover the image from Tiles
         wfs_Response = self.wfs.search(filter=filter, srsname=srsname)
+
+        if bbox is not None:
+            if process.aoi_coverage(bbox, wfs_Response)['features'][0]['bbox_coverage'] == 0:
+                raise Exception("Bounding box is outside of desired feature's AOI")
+
         keysToDel = []
-        for tile, bbox in tiles.items():
+        for tile, tile_bbox in tiles.items():
             if srsname == "EPSG:4326":
-                bbox_coverage = process.aoi_coverage(bbox, wfs_Response)['features'][0]['coverage']
+                bbox_coverage = process.aoi_coverage(tile_bbox, wfs_Response)['features'][0]['coverage']
             else:
-                bbox_list = [i for i in bbox.split(',')]
-                bbox = ",".join([bbox_list[1], bbox_list[0], bbox_list[3], bbox_list[2], srsname])
-                bbox_coverage = process.aoi_coverage(bbox + ",{}".format(srsname), wfs_Response)['features'][0]['coverage']
+                tile_bbox_list = [i for i in tile_bbox.split(',')]
+                sub_bbox = ",".join([tile_bbox_list[1], tile_bbox_list[0], tile_bbox_list[3], tile_bbox_list[2], srsname])
+                bbox_coverage = process.aoi_coverage(sub_bbox + ",{}".format(srsname), wfs_Response)['features'][0]['coverage']
             if bbox_coverage == 0.0:
                 keysToDel.append(tile)
 
         for tileKey in keysToDel:
             del tiles[tileKey]
 
+
         url = self.wms.base_url
         headers = self.wms.headers
         querstring = self.wms.querystring
         querstring['crs'] = srsname
         querstring['width'] = img_size
         querstring['height'] = img_size
         querstring['coverage_cql_filter'] = "featureId='{}'".format(featureid)
```

### Comparing `Maxar_OGC-1.3.0/src/Maxar_OGC/process.py` & `Maxar_OGC-1.3.1/src/Maxar_OGC/process.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
-import pyproj
+from pyproj import Transformer
 import shapely.ops as ops
 from shapely.geometry.polygon import Polygon
 import shapely.geometry
 import shapely.wkt
-from functools import partial
 import random
 import string
 import queue
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime
 
 
@@ -45,41 +44,35 @@
     xmin = float(bboxlst[1])
     xmax = float(bboxlst[3])
 
     if srsname == "EPSG:4326":
 
         geom = Polygon([(xmin, ymin), (xmin, ymax), (xmax, ymax), (xmax, ymin)])
 
+        transformer = Transformer.from_crs(
+            "EPSG:4326",
+            f"+proj=aea +lat_1={geom.bounds[1]} +lat_2={geom.bounds[3]}",
+            always_xy=True)
+
         geom_area = ops.transform(
-        partial(
-            pyproj.transform,
-            pyproj.Proj(init='EPSG:4326'),
-            pyproj.Proj(
-                proj='aea',
-                lat_1=geom.bounds[1],
-                lat_2=geom.bounds[3]
-            )
-        ),
-        geom)
+            transformer.transform,
+            geom)
 
     else:
 
         geom = Polygon([(xmin, ymin), (xmin, ymax), (xmax, ymax), (xmax, ymin), (xmin, ymin)])
 
+        transformer = Transformer.from_crs(
+            srsname,
+            f"+proj=aea +lat_1={geom.bounds[1]} +lat_2={geom.bounds[3]}",
+            always_xy=True)
+
         geom_area = ops.transform(
-        partial(
-            pyproj.transform,
-            pyproj.Proj(init=srsname),
-            pyproj.Proj(
-                proj='aea',
-                lat_1=geom.bounds[1],
-                lat_2=geom.bounds[3]
-            )
-        ),
-        geom)
+            transformer.transform,
+            geom)
 
     # Print the area in sqkm^2
 
     geomareasqkm = geom_area.area/(10**6)
     return geomareasqkm
 
 
@@ -249,105 +242,105 @@
 def _check_typeName(typename):
     acceptable_types = ['FinishedFeature', 'TileMatrixFeature', 'ImageInMosaicFeature', 'MaxarCatalogMosaicProducts',
                         'MaxarCatalogMosaicSeamlines', 'MaxarCatalogMosaicTiles', 'PCMChangePolygons']
     if typename not in acceptable_types:
         raise Exception('{} is not an acceptable TypeName. Please use one of the following {}'.format(typename, acceptable_types))
 
 
-def cql_checker(cql_filter):
-    """
-    Function checks for the validity of a passed in cql filter
-    Args:
-        cql_filter: string representation of cql filter
-    """
-    string_list = ['featureId', 'sourceUnit', 'productType', 'groundSampleDistanceUnits', 'dataLayer', 'product_line_item',
-                   'legacyDescription', 'colorBandOrder', 'assetName', 'assetType', 'legacyId',
-                   'factoryOrderNumber', 'layer', 'crsFromPixels', 'url', 'spatialAccuracy', 'catalogIdentifier',
-                   'tileMatrixSet', 'tileMatrix', 'product_name', 'product_id', 'acquisitionTime']
-    string_date_list = ['acquisitionDate', 'ingestDate', 'collect_date_min']
-    float_list = ['groundSampleDistance', 'perPixelX', 'perPixelY', 'CE90Accuracy', 'RMSEAccuracy']
-    boolean_list = ['outputMosaic']
-    integer_list = ['ageDays', 'row', 'column']
-    source_list = ["'WV01'", "'WV02'", "'WV03_VNIR'", "'WV03'", "'WV04'", "'GE01'", "'QB02'", "'KS3'", "'KS3A'",
-                   "'WV03_SWIR'", "'KS5'", "'RS2'", "'IK02'", "'LG01'", "'LG02'"]
-    _0_360_list = ['sunAzimuth', 'offNadirAngle', 'sunElevation']
-    _0_1_list = ['cloudCover']
-    error_list = []
-    if cql_filter is None:
-        error_list.append('filter can not be None type')
-        raise Exception('CQL Filter Error:', error_list)
-    if cql_filter.find(')') < cql_filter.find('(') or cql_filter.count('(') != cql_filter.count(')'):
-        error_list.append('Incorrect parenthesis')
-    temp_list = [x.split('AND') for x in [i for i in cql_filter.split('OR')]]
-    cql_parse = [item.replace('(', '').replace(')', '') for sublist in temp_list for item in sublist]
-    for item in cql_parse:
-        if item.find('>=') > 0:
-            key, value = item.split('>=')
-        elif item.find('<=') > 0:
-            key, value = item.split('<=')
-        elif item.find('=') > 0:
-            key, value = item.split('=')
-        elif item.find('<') > 0:
-            key, value = item.split('<')
-        elif item.find('>') > 0:
-            key, value = item.split('>')
-        else:
-            error_list.append('No comparison operator e.g. < > =')
-        if key == 'source':
-            if value not in source_list:
-                error_list.append(f'{value} should be {source_list}')
-        elif key in float_list:
-            try:
-                float(value)
-            except:
-                error_list.append(f'{value} Not a float')
-        elif key in boolean_list:
-            if value != 'FALSE' and value != 'TRUE':
-                error_list.append(f'{value} should be either TRUE or FALSE')
-        elif key in integer_list:
-            try:
-                int(value)
-            except:
-                error_list.append(f'{value} Not an integer')
-        elif key in string_date_list:
-            if value[0] != "'" or value[-1] != "'":
-                error_list.append(f'{value} Need single quotes around dates')
-            value = value.replace("'", "")
-            try:
-                format_data = "%Y-%m-%d %H:%M:%S.%f"
-                datetime.strptime(value, format_data)
-            except:
-                try:
-                    format_data_2 = "%Y-%m-%d"
-                    datetime.strptime(value, format_data_2)
-                except:
-                    error_list.append(f'{value} Not a valid date')
-        elif key in string_list:
-            if value[0] != "'" or value[-1] != "'":
-                error_list.append(f'{value} Need single quotes around value')
-            if not isinstance(value, str):
-                error_list.append(f'{value} Not a valid string value')
-        elif key in _0_1_list:
-            try:
-                value = float(value)
-            except:
-                error_list.append(f'{value} Not a float')
-            if not (0 <= value <= 1):
-                error_list.append(f'{value} must be between 0 and 1')
-        elif key in _0_360_list:
-            try:
-                value = float(value)
-            except:
-                error_list.append(f'{value} Not a float')
-            if not (0 <= value <= 360):
-                error_list.append(f'{value} must be between 0 and 360')
-        else:
-            error_list.append(f'{key, value} Not a valid parameter')
-    if len(error_list) > 0:
-        raise Exception('CQL Filter Error:', error_list)
+# def cql_checker(cql_filter):
+#     """
+#     Function checks for the validity of a passed in cql filter
+#     Args:
+#         cql_filter: string representation of cql filter
+#     """
+#     string_list = ['featureId', 'sourceUnit', 'productType', 'groundSampleDistanceUnits', 'dataLayer', 'product_line_item',
+#                    'legacyDescription', 'colorBandOrder', 'assetName', 'assetType', 'legacyId',
+#                    'factoryOrderNumber', 'layer', 'crsFromPixels', 'url', 'spatialAccuracy', 'catalogIdentifier',
+#                    'tileMatrixSet', 'tileMatrix', 'product_name', 'product_id', 'acquisitionTime']
+#     string_date_list = ['acquisitionDate', 'ingestDate', 'collect_date_min']
+#     float_list = ['groundSampleDistance', 'perPixelX', 'perPixelY', 'CE90Accuracy', 'RMSEAccuracy']
+#     boolean_list = ['outputMosaic']
+#     integer_list = ['ageDays', 'row', 'column']
+#     source_list = ["'WV01'", "'WV02'", "'WV03_VNIR'", "'WV03'", "'WV04'", "'GE01'", "'QB02'", "'KS3'", "'KS3A'",
+#                    "'WV03_SWIR'", "'KS5'", "'RS2'", "'IK02'", "'LG01'", "'LG02'"]
+#     _0_360_list = ['sunAzimuth', 'offNadirAngle', 'sunElevation']
+#     _0_1_list = ['cloudCover']
+#     error_list = []
+#     if cql_filter is None:
+#         error_list.append('filter can not be None type')
+#         raise Exception('CQL Filter Error:', error_list)
+#     if cql_filter.find(')') < cql_filter.find('(') or cql_filter.count('(') != cql_filter.count(')'):
+#         error_list.append('Incorrect parenthesis')
+#     temp_list = [x.split('AND') for x in [i for i in cql_filter.split('OR')]]
+#     cql_parse = [item.replace('(', '').replace(')', '') for sublist in temp_list for item in sublist]
+#     for item in cql_parse:
+#         if item.find('>=') > 0:
+#             key, value = item.split('>=')
+#         elif item.find('<=') > 0:
+#             key, value = item.split('<=')
+#         elif item.find('=') > 0:
+#             key, value = item.split('=')
+#         elif item.find('<') > 0:
+#             key, value = item.split('<')
+#         elif item.find('>') > 0:
+#             key, value = item.split('>')
+#         else:
+#             error_list.append('No comparison operator e.g. < > =')
+#         if key == 'source':
+#             if value not in source_list:
+#                 error_list.append(f'{value} should be {source_list}')
+#         elif key in float_list:
+#             try:
+#                 float(value)
+#             except:
+#                 error_list.append(f'{value} Not a float')
+#         elif key in boolean_list:
+#             if value != 'FALSE' and value != 'TRUE':
+#                 error_list.append(f'{value} should be either TRUE or FALSE')
+#         elif key in integer_list:
+#             try:
+#                 int(value)
+#             except:
+#                 error_list.append(f'{value} Not an integer')
+#         elif key in string_date_list:
+#             if value[0] != "'" or value[-1] != "'":
+#                 error_list.append(f'{value} Need single quotes around dates')
+#             value = value.replace("'", "")
+#             try:
+#                 format_data = "%Y-%m-%d %H:%M:%S.%f"
+#                 datetime.strptime(value, format_data)
+#             except:
+#                 try:
+#                     format_data_2 = "%Y-%m-%d"
+#                     datetime.strptime(value, format_data_2)
+#                 except:
+#                     error_list.append(f'{value} Not a valid date')
+#         elif key in string_list:
+#             if value[0] != "'" or value[-1] != "'":
+#                 error_list.append(f'{value} Need single quotes around value')
+#             if not isinstance(value, str):
+#                 error_list.append(f'{value} Not a valid string value')
+#         elif key in _0_1_list:
+#             try:
+#                 value = float(value)
+#             except:
+#                 error_list.append(f'{value} Not a float')
+#             if not (0 <= value <= 1):
+#                 error_list.append(f'{value} must be between 0 and 1')
+#         elif key in _0_360_list:
+#             try:
+#                 value = float(value)
+#             except:
+#                 error_list.append(f'{value} Not a float')
+#             if not (0 <= value <= 360):
+#                 error_list.append(f'{value} must be between 0 and 360')
+#         else:
+#             error_list.append(f'{key, value} Not a valid parameter')
+#     if len(error_list) > 0:
+#         raise Exception('CQL Filter Error:', error_list)
 
 
 class BoundedThreadPoolExecutor(ThreadPoolExecutor):
 
     def __init__(self, *args, **kwargs):
         super(BoundedThreadPoolExecutor, self).__init__(*args, **kwargs)
         self._work_queue = queue.Queue()
```

### Comparing `Maxar_OGC-1.3.0/src/Maxar_OGC/wcs.py` & `Maxar_OGC-1.3.1/src/Maxar_OGC/wcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         Returns:
             requests response object of desired image
         """
 
         self.querystring = self._init_querystring()
         keys = list(kwargs.keys())
         process._validate_bbox(bbox, srsname=srsname)
-        if 'filter' in kwargs:
-            process.cql_checker(kwargs.get('filter'))
+        # if 'filter' in kwargs:
+        #     process.cql_checker(kwargs.get('filter'))
         self.querystring.update({'boundingbox': bbox})
         self.querystring.update({'identifier': identifier})
         self.querystring.update({'gridoffsets': gridoffsets})
         if srsname != "EPSG:4326":
             self.querystring['gridcrs'] = "urn:ogc:def:crs:EPSG::{}".format(srsname[5:])
             self.querystring.update({'gridbasecrs': 'urn:ogc:def:crs:EPSG::{}'.format(srsname[5:])})
             bbox_list = [i for i in bbox.split(',')]
```

### Comparing `Maxar_OGC-1.3.0/src/Maxar_OGC/wfs.py` & `Maxar_OGC-1.3.1/src/Maxar_OGC/wfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         """
 
         self.querystring = self._init_querystring()
         process._check_typeName(typename)
         self.querystring.update({'typename': 'DigitalGlobe:{}'.format(typename)})
         keys = list(kwargs.keys())
         if 'filter' in keys and kwargs['filter']:
-            process.cql_checker(kwargs.get('filter'))
+            # process.cql_checker(kwargs.get('filter'))
             if 'bbox' in keys and kwargs['bbox']:
                 if srsname == "EPSG:4326":
                     process._validate_bbox(kwargs['bbox'], srsname=srsname)
                     self._combine_bbox_and_filter(kwargs['filter'], kwargs['bbox'], typename)
                     del (kwargs['filter'])
                     del (kwargs['bbox'])
                 else:
```

### Comparing `Maxar_OGC-1.3.0/src/Maxar_OGC/wms.py` & `Maxar_OGC-1.3.1/src/Maxar_OGC/wms.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                 bbox_list = [i for i in kwargs['bbox'].split(',')]
                 kwargs['bbox'] = ",".join([bbox_list[1], bbox_list[0], bbox_list[3], bbox_list[2]])
                 self.querystring['crs'] = kwargs['srsname']
             self.querystring.update({'bbox': kwargs['bbox']})
         else:
             raise Exception('Search function must have a BBOX.')
         if 'filter' in keys:
-            process.cql_checker(kwargs.get('filter'))
+            # process.cql_checker(kwargs.get('filter'))
             self.querystring.update({'coverage_cql_filter': kwargs['filter']})
             del (kwargs['filter'])
         del (kwargs['srsname'])
         for key, value in kwargs.items():
             self.querystring[key] = value
 
         request = requests.get(self.base_url, headers=self.headers, params=self.querystring)
```

### Comparing `Maxar_OGC-1.3.0/src/Maxar_OGC/wmts.py` & `Maxar_OGC-1.3.1/src/Maxar_OGC/wmts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import xml.etree.ElementTree as ET
 import Maxar_OGC.process as process
 import math
-from pyproj import transform, Proj
+from pyproj import Transformer
 
 class WMTS:
     def __init__(self, session):
         self.base_url = session['base_url'] + "earthservice/wmtsaccess"
         self.headers = session['headers']
         self.connect_id = session['connectid']
         self.response = None
@@ -40,17 +40,16 @@
                             matrixwidth = TileMatrixSet[i][5].text
                             matrixheight = TileMatrixSet[i][6].text
             if not matrixwidth or not matrixheight:
                 raise Exception('Unable to determine Matrix dimensions from input coordinates')
 
             return str(round((float(longx) + 180) * (int(matrixwidth)/360))), str(round((90 - float(laty)) * (int(matrixheight)/180)))
         else:
-            inProj = Proj(init=crs)
-            outProj = Proj(init='epsg:4326')
-            x2, y2 = transform(inProj, outProj, longx, laty)
+            transform = Transformer.from_crs(crs, "EPSG:4326")
+            x2, y2 = transform.transform(longx, laty)
 
             def deg2num(lat_deg, lon_deg, zoom):
                 lat_rad = math.radians(lat_deg)
                 n = 2.0 ** zoom
                 xtile = int((lon_deg + 180.0) / 360.0 * n)
                 ytile = int((1.0 - math.asinh(math.tan(lat_rad)) / math.pi) / 2.0 * n)
                 return (str(xtile), str(ytile))
```

### Comparing `Maxar_OGC-1.3.0/src/Maxar_OGC.egg-info/PKG-INFO` & `Maxar_OGC-1.3.1/src/Maxar_OGC.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Maxar-OGC
-Version: 1.3.0
+Version: 1.3.1
 Summary: SDK for interacting with Maxar imagery platforms
 Author: GCS Marianas Team
 Author-email: DL-GCS-Marianas@digitalglobe.com
 License: MIT
 Project-URL: Documentation, https://cloudservices.readthedocs.io/en/latest/index.html
 Project-URL: Source, https://github.com/DigitalGlobe/CloudServices
 Keywords: OGC,WMS,WFS,WMTS,WCS,MAXAR,IMAGERY,GIS
```

