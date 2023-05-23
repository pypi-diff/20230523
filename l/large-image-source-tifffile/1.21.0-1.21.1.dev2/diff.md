# Comparing `tmp/large-image-source-tifffile-1.21.0.tar.gz` & `tmp/large-image-source-tifffile-1.21.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-tifffile-1.21.0.tar", last modified: Tue May 23 14:22:05 2023, max compression
+gzip compressed data, was "large-image-source-tifffile-1.21.1.dev2.tar", last modified: Tue May 23 18:53:26 2023, max compression
```

## Comparing `large-image-source-tifffile-1.21.0.tar` & `large-image-source-tifffile-1.21.1.dev2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 14:22:05.357571 large-image-source-tifffile-1.21.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-05-23 14:22:05.000000 large-image-source-tifffile-1.21.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      870 2023-05-23 14:22:05.357571 large-image-source-tifffile-1.21.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-05-23 14:22:05.000000 large-image-source-tifffile-1.21.0/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 14:22:05.357571 large-image-source-tifffile-1.21.0/large_image_source_tifffile/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19914 2023-05-23 14:19:58.000000 large-image-source-tifffile-1.21.0/large_image_source_tifffile/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2023-05-23 14:19:58.000000 large-image-source-tifffile-1.21.0/large_image_source_tifffile/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 14:22:05.357571 large-image-source-tifffile-1.21.0/large_image_source_tifffile.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      870 2023-05-23 14:22:05.000000 large-image-source-tifffile-1.21.0/large_image_source_tifffile.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-05-23 14:22:05.000000 large-image-source-tifffile-1.21.0/large_image_source_tifffile.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-23 14:22:05.000000 large-image-source-tifffile-1.21.0/large_image_source_tifffile.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-05-23 14:22:05.000000 large-image-source-tifffile-1.21.0/large_image_source_tifffile.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-05-23 14:22:05.000000 large-image-source-tifffile-1.21.0/large_image_source_tifffile.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-05-23 14:22:05.000000 large-image-source-tifffile-1.21.0/large_image_source_tifffile.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-23 14:22:05.357571 large-image-source-tifffile-1.21.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2694 2023-05-23 14:19:58.000000 large-image-source-tifffile-1.21.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 18:53:26.393592 large-image-source-tifffile-1.21.1.dev2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-05-23 18:53:26.000000 large-image-source-tifffile-1.21.1.dev2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      875 2023-05-23 18:53:26.393592 large-image-source-tifffile-1.21.1.dev2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-05-23 18:53:26.000000 large-image-source-tifffile-1.21.1.dev2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 18:53:26.393592 large-image-source-tifffile-1.21.1.dev2/large_image_source_tifffile/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20913 2023-05-23 18:51:23.000000 large-image-source-tifffile-1.21.1.dev2/large_image_source_tifffile/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2023-05-23 18:51:23.000000 large-image-source-tifffile-1.21.1.dev2/large_image_source_tifffile/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 18:53:26.393592 large-image-source-tifffile-1.21.1.dev2/large_image_source_tifffile.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      875 2023-05-23 18:53:26.000000 large-image-source-tifffile-1.21.1.dev2/large_image_source_tifffile.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-05-23 18:53:26.000000 large-image-source-tifffile-1.21.1.dev2/large_image_source_tifffile.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-23 18:53:26.000000 large-image-source-tifffile-1.21.1.dev2/large_image_source_tifffile.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-05-23 18:53:26.000000 large-image-source-tifffile-1.21.1.dev2/large_image_source_tifffile.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      212 2023-05-23 18:53:26.000000 large-image-source-tifffile-1.21.1.dev2/large_image_source_tifffile.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-05-23 18:53:26.000000 large-image-source-tifffile-1.21.1.dev2/large_image_source_tifffile.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-23 18:53:26.393592 large-image-source-tifffile-1.21.1.dev2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2694 2023-05-23 18:51:23.000000 large-image-source-tifffile-1.21.1.dev2/setup.py
```

### Comparing `large-image-source-tifffile-1.21.0/LICENSE` & `large-image-source-tifffile-1.21.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.21.0/PKG-INFO` & `large-image-source-tifffile-1.21.1.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-tifffile
-Version: 1.21.0
+Version: 1.21.1.dev2
 Summary: A tifffile tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-tifffile-1.21.0/README.rst` & `large-image-source-tifffile-1.21.1.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.21.0/large_image_source_tifffile/__init__.py` & `large-image-source-tifffile-1.21.1.dev2/large_image_source_tifffile/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import logging
 import math
 import os
 import threading
 
 import numpy
 import zarr
@@ -72,14 +73,15 @@
         'image/scn': SourcePriority.PREFERRED,
     }
 
     # Fallback for non-tiled or oddly tiled sources
     _tileSize = 512
     _minImageSize = 128
     _minTileSize = 128
+    _singleTileSize = 1024
     _maxTileSize = 2048
     _minAssociatedImageSize = 64
     _maxAssociatedImageSize = 8192
 
     def __init__(self, path, **kwargs):
         """
         Initialize the tile class.  See the base class for other available
@@ -98,14 +100,16 @@
             if not os.path.isfile(self._largeImagePath):
                 raise TileSourceFileNotFoundError(self._largeImagePath) from None
             raise TileSourceError('File cannot be opened via tifffile.')
         maxseries, maxsamples = self._biggestSeries()
         self.tileWidth = self.tileHeight = self._tileSize
         s = self._tf.series[maxseries]
         self._baseSeries = s
+        if len(s.levels) == 1:
+            self.tileWidth = self.tileHeight = self._singleTileSize
         page = s.pages[0]
         if ('TileWidth' in page.tags and
                 self._minTileSize <= page.tags['TileWidth'].value <= self._maxTileSize):
             self.tileWidth = page.tags['TileWidth'].value
         if ('TileLength' in page.tags and
                 self._minTileSize <= page.tags['TileLength'].value <= self._maxTileSize):
             self.tileHeight = page.tags['TileLength'].value
@@ -239,14 +243,23 @@
                 entry['width'] = s.shape[s.axes.index('X')]
                 entry['height'] = s.shape[s.axes.index('Y')]
                 if (id not in self._associatedImages and
                         max(entry['width'], entry['height']) <= self._maxAssociatedImageSize and
                         max(entry['width'], entry['height']) >= self._minAssociatedImageSize):
                     self._associatedImages[id] = entry
 
+    def _handle_imagej(self):
+        try:
+            ijm = self._tf.pages[0].tags['IJMetadata'].value
+            if (ijm['Labels'] and len(ijm['Labels']) == self._framecount and
+                    not getattr(self, '_channels', None)):
+                self._channels = ijm['Labels']
+        except Exception:
+            pass
+
     def _handle_scn(self):  # noqa
         """
         For SCN files, parse the xml and possibly adjust how associated images
         are labelled.
         """
         import xml.etree.ElementTree
 
@@ -355,23 +368,31 @@
         """
         result = {}
         pages = [s.pages[0] for s in self._tf.series]
         pagesInSeries = [p for s in self._tf.series for ll in s.pages.levels for p in ll.pages]
         pages.extend([page for page in self._tf.pages if page not in pagesInSeries])
         for page in pages:
             for tag in getattr(page, 'tags', []):
-                if tag.dtype_name == 'ASCII' and tag.value:
+                if (tag.dtype_name == 'ASCII' or (
+                        tag.dtype_name == 'BYTE' and isinstance(tag.value, dict))) and tag.value:
                     key = basekey = tag.name
                     suffix = 0
                     while key in result:
                         if result[key] == tag.value:
                             break
                         suffix += 1
                         key = '%s_%d' % (basekey, suffix)
                     result[key] = tag.value
+                    if isinstance(result[key], dict):
+                        result[key] = result[key].copy()
+                        for subkey in list(result[key]):
+                            try:
+                                json.dumps(result[key][subkey])
+                            except Exception:
+                                del result[key][subkey]
         if hasattr(self, '_xml') and 'xml' not in result:
             result.pop('ImageDescription', None)
             result['xml'] = self._xml
         if hasattr(self, '_channelInfo'):
             result['channelInfo'] = self._channelInfo
         result['tifffileKind'] = self._baseSeries.kind
         return result
@@ -416,19 +437,21 @@
         else:
             sidx = 0
         series = self._tf.series[self._series[sidx]]
         with self._zarrlock:
             if sidx not in self._zarrcache:
                 if len(self._zarrcache) > 10:
                     self._zarrcache = {}
-                self._zarrcache[sidx] = zarr.open(series.aszarr(), mode='r')
-            za = self._zarrcache[sidx]
+                za = zarr.open(series.aszarr(), mode='r')
+                hasgbs = hasattr(za[0], 'get_basic_selection')
+                self._zarrcache[sidx] = (za, hasgbs)
+            za, hasgbs = self._zarrcache[sidx]
         xidx = series.axes.index('X')
         yidx = series.axes.index('Y')
-        if hasattr(za[0], 'get_basic_selection'):
+        if hasgbs:
             bza = za[0]
             # we could cache this
             for ll in range(len(series.levels) - 1, 0, -1):
                 scale = round(max(za[0].shape[xidx] / za[ll].shape[xidx],
                                   za[0].shape[yidx] / za[ll].shape[yidx]))
                 if scale <= step and step // scale == step / scale:
                     bza = za[ll]
```

### Comparing `large-image-source-tifffile-1.21.0/large_image_source_tifffile/girder_source.py` & `large-image-source-tifffile-1.21.1.dev2/large_image_source_tifffile/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.21.0/large_image_source_tifffile.egg-info/PKG-INFO` & `large-image-source-tifffile-1.21.1.dev2/large_image_source_tifffile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-tifffile
-Version: 1.21.0
+Version: 1.21.1.dev2
 Summary: A tifffile tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-tifffile-1.21.0/setup.py` & `large-image-source-tifffile-1.21.1.dev2/setup.py`

 * *Files identical despite different names*

