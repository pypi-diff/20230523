# Comparing `tmp/geocube-0.4.0.tar.gz` & `tmp/geocube-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocube-0.4.0.tar", last modified: Fri Mar  3 20:44:54 2023, max compression
+gzip compressed data, was "geocube-0.4.1.tar", last modified: Tue May 23 17:37:39 2023, max compression
```

## Comparing `geocube-0.4.0.tar` & `geocube-0.4.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:44:54.798224 geocube-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-03-03 20:44:39.000000 geocube-0.4.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-03-03 20:44:39.000000 geocube-0.4.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-03-03 20:44:39.000000 geocube-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-03 20:44:39.000000 geocube-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-03-03 20:44:54.798224 geocube-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-03-03 20:44:39.000000 geocube-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:44:54.794224 geocube-0.4.0/geocube/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-03 20:44:39.000000 geocube-0.4.0/geocube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-03-03 20:44:39.000000 geocube-0.4.0/geocube/_show_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-03 20:44:39.000000 geocube-0.4.0/geocube/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:44:54.794224 geocube-0.4.0/geocube/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 20:44:39.000000 geocube-0.4.0/geocube/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-03-03 20:44:39.000000 geocube-0.4.0/geocube/api/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:44:54.798224 geocube-0.4.0/geocube/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 20:44:39.000000 geocube-0.4.0/geocube/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:44:54.798224 geocube-0.4.0/geocube/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-03 20:44:39.000000 geocube-0.4.0/geocube/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-03-03 20:44:39.000000 geocube-0.4.0/geocube/cli/commands/make_geocube.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-03-03 20:44:39.000000 geocube-0.4.0/geocube/cli/geocube.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-03 20:44:39.000000 geocube-0.4.0/geocube/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:44:54.798224 geocube-0.4.0/geocube/geo_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-03 20:44:39.000000 geocube-0.4.0/geocube/geo_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-03-03 20:44:39.000000 geocube-0.4.0/geocube/geo_utils/geobox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-03-03 20:44:39.000000 geocube-0.4.0/geocube/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 20:44:39.000000 geocube-0.4.0/geocube/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-03-03 20:44:39.000000 geocube-0.4.0/geocube/rasterize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-03-03 20:44:39.000000 geocube-0.4.0/geocube/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    14643 2023-03-03 20:44:39.000000 geocube-0.4.0/geocube/vector_to_cube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:44:54.798224 geocube-0.4.0/geocube/xarray_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 20:44:39.000000 geocube-0.4.0/geocube/xarray_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-03-03 20:44:39.000000 geocube-0.4.0/geocube/xarray_extensions/vectorxarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:44:54.794224 geocube-0.4.0/geocube.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-03-03 20:44:54.000000 geocube-0.4.0/geocube.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-03 20:44:54.000000 geocube-0.4.0/geocube.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 20:44:54.000000 geocube-0.4.0/geocube.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-03 20:44:54.000000 geocube-0.4.0/geocube.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 20:44:54.000000 geocube-0.4.0/geocube.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-03-03 20:44:54.000000 geocube-0.4.0/geocube.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-03 20:44:54.000000 geocube-0.4.0/geocube.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-03 20:44:39.000000 geocube-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-03-03 20:44:54.798224 geocube-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-03 20:44:39.000000 geocube-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:39.933418 geocube-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-23 17:37:18.000000 geocube-0.4.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-23 17:37:18.000000 geocube-0.4.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-23 17:37:18.000000 geocube-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-23 17:37:18.000000 geocube-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-23 17:37:39.933418 geocube-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-23 17:37:18.000000 geocube-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:39.933418 geocube-0.4.1/geocube/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-23 17:37:18.000000 geocube-0.4.1/geocube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-23 17:37:18.000000 geocube-0.4.1/geocube/_show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-23 17:37:18.000000 geocube-0.4.1/geocube/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:39.933418 geocube-0.4.1/geocube/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:18.000000 geocube-0.4.1/geocube/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-23 17:37:18.000000 geocube-0.4.1/geocube/api/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:39.933418 geocube-0.4.1/geocube/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:18.000000 geocube-0.4.1/geocube/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:39.933418 geocube-0.4.1/geocube/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-23 17:37:18.000000 geocube-0.4.1/geocube/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-23 17:37:18.000000 geocube-0.4.1/geocube/cli/commands/make_geocube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-23 17:37:18.000000 geocube-0.4.1/geocube/cli/geocube.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-23 17:37:18.000000 geocube-0.4.1/geocube/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:39.933418 geocube-0.4.1/geocube/geo_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-23 17:37:18.000000 geocube-0.4.1/geocube/geo_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-05-23 17:37:18.000000 geocube-0.4.1/geocube/geo_utils/geobox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-23 17:37:18.000000 geocube-0.4.1/geocube/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:18.000000 geocube-0.4.1/geocube/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-05-23 17:37:18.000000 geocube-0.4.1/geocube/rasterize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-23 17:37:18.000000 geocube-0.4.1/geocube/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-05-23 17:37:18.000000 geocube-0.4.1/geocube/vector_to_cube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:39.933418 geocube-0.4.1/geocube/xarray_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:18.000000 geocube-0.4.1/geocube/xarray_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-05-23 17:37:18.000000 geocube-0.4.1/geocube/xarray_extensions/vectorxarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:39.933418 geocube-0.4.1/geocube.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-23 17:37:39.000000 geocube-0.4.1/geocube.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-23 17:37:39.000000 geocube-0.4.1/geocube.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:37:39.000000 geocube-0.4.1/geocube.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-23 17:37:39.000000 geocube-0.4.1/geocube.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:37:39.000000 geocube-0.4.1/geocube.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-23 17:37:39.000000 geocube-0.4.1/geocube.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 17:37:39.000000 geocube-0.4.1/geocube.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-23 17:37:18.000000 geocube-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-23 17:37:39.937418 geocube-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 17:37:18.000000 geocube-0.4.1/setup.py
```

### Comparing `geocube-0.4.0/AUTHORS.rst` & `geocube-0.4.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `geocube-0.4.0/CONTRIBUTING.rst` & `geocube-0.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `geocube-0.4.0/LICENSE` & `geocube-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geocube-0.4.0/PKG-INFO` & `geocube-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocube
-Version: 0.4.0
+Version: 0.4.1
 Summary: Tool to convert geopandas vector data into rasterized xarray data.
 Home-page: https://github.com/corteva/geocube
 Download-URL: http://python.org/pypi/geocube
 Author: geocube Contributors
 Author-email: alansnow21@gmail.com
 License: BSD license
 Keywords: geocube,GDAL,rasterize,vector
```

### Comparing `geocube-0.4.0/README.rst` & `geocube-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `geocube-0.4.0/geocube/_show_versions.py` & `geocube-0.4.1/geocube/_show_versions.py`

 * *Files identical despite different names*

### Comparing `geocube-0.4.0/geocube/api/core.py` & `geocube-0.4.1/geocube/api/core.py`

 * *Files identical despite different names*

### Comparing `geocube-0.4.0/geocube/cli/commands/make_geocube.py` & `geocube-0.4.1/geocube/cli/commands/make_geocube.py`

 * *Files identical despite different names*

### Comparing `geocube-0.4.0/geocube/cli/geocube.py` & `geocube-0.4.1/geocube/cli/geocube.py`

 * *Files identical despite different names*

### Comparing `geocube-0.4.0/geocube/geo_utils/geobox.py` & `geocube-0.4.1/geocube/geo_utils/geobox.py`

 * *Files identical despite different names*

### Comparing `geocube-0.4.0/geocube/logger.py` & `geocube-0.4.1/geocube/logger.py`

 * *Files identical despite different names*

### Comparing `geocube-0.4.0/geocube/rasterize.py` & `geocube-0.4.1/geocube/rasterize.py`

 * *Files identical despite different names*

### Comparing `geocube-0.4.0/geocube/vector.py` & `geocube-0.4.1/geocube/vector.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,18 +34,19 @@
 
     Returns
     -------
     geopandas.GeoDataFrame
     """
     # nodata mask
     mask = None
-    if numpy.isnan(data_array.rio.nodata):
-        mask = ~data_array.isnull()
-    elif data_array.rio.nodata is not None:
-        mask = data_array != data_array.rio.nodata
+    if data_array.rio.nodata is not None:
+        if numpy.isnan(data_array.rio.nodata):
+            mask = ~data_array.isnull()
+        else:
+            mask = data_array != data_array.rio.nodata
 
     # vectorize generator
     vectorized_data = (
         (value, shapely.geometry.shape(polygon))
         for polygon, value in rasterio.features.shapes(
             data_array,
             transform=data_array.rio.transform(),
```

### Comparing `geocube-0.4.0/geocube/vector_to_cube.py` & `geocube-0.4.1/geocube/vector_to_cube.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,17 +148,20 @@
             )
         # reproject vector data to the projection of the output raster
         if self._geobox.crs is not None:
             vector_data = self._vector_data.to_crs(self._geobox.crs)
 
         # convert to datetime
         for datetime_measurement in self._datetime_measurements:  # type: ignore
-            vector_data[datetime_measurement] = pandas.to_datetime(
-                vector_data[datetime_measurement]
-            ).astype("datetime64[ns]")
+            vector_data[datetime_measurement] = (
+                pandas.to_datetime(vector_data[datetime_measurement])
+                .dt.tz_convert("UTC")
+                .dt.tz_localize(None)
+                .astype("datetime64[ns]")
+            )
 
         # get categorical enumerations if they exist
         self._categorical_enums = {}
         for categorical_column in vector_data.select_dtypes(["category"]).columns:
             self._categorical_enums[categorical_column] = vector_data[
                 categorical_column
             ].cat.categories
```

### Comparing `geocube-0.4.0/geocube/xarray_extensions/vectorxarray.py` & `geocube-0.4.1/geocube/xarray_extensions/vectorxarray.py`

 * *Files identical despite different names*

### Comparing `geocube-0.4.0/geocube.egg-info/PKG-INFO` & `geocube-0.4.1/geocube.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocube
-Version: 0.4.0
+Version: 0.4.1
 Summary: Tool to convert geopandas vector data into rasterized xarray data.
 Home-page: https://github.com/corteva/geocube
 Download-URL: http://python.org/pypi/geocube
 Author: geocube Contributors
 Author-email: alansnow21@gmail.com
 License: BSD license
 Keywords: geocube,GDAL,rasterize,vector
```

### Comparing `geocube-0.4.0/geocube.egg-info/SOURCES.txt` & `geocube-0.4.1/geocube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geocube-0.4.0/setup.cfg` & `geocube-0.4.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 author = geocube Contributors
 author_email = alansnow21@gmail.com
 name = geocube
-version = 0.4.0
+version = 0.4.1
 description = Tool to convert geopandas vector data into rasterized xarray data.
 keywords = geocube, GDAL, rasterize, vector
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 license = BSD license
 license_files = LICENSE
 platform = any
```

