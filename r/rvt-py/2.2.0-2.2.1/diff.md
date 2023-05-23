# Comparing `tmp/rvt_py-2.2.0.tar.gz` & `tmp/rvt_py-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rvt_py-2.2.0.tar", last modified: Mon May 22 19:15:45 2023, max compression
+gzip compressed data, was "rvt_py-2.2.1.tar", last modified: Tue May 23 18:20:32 2023, max compression
```

## Comparing `rvt_py-2.2.0.tar` & `rvt_py-2.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 19:15:45.835048 rvt_py-2.2.0/
--rw-rw-rw-   0        0        0    11567 2021-01-08 07:43:58.000000 rvt_py-2.2.0/LICENSE
--rw-rw-rw-   0        0        0     5875 2023-05-22 19:15:45.835048 rvt_py-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4792 2023-05-21 19:08:15.000000 rvt_py-2.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 19:15:45.812049 rvt_py-2.2.0/rvt/
--rw-rw-rw-   0        0        0      484 2023-05-21 19:08:15.000000 rvt_py-2.2.0/rvt/__init__.py
--rw-rw-rw-   0        0        0    74233 2023-05-21 19:08:15.000000 rvt_py-2.2.0/rvt/blend.py
--rw-rw-rw-   0        0        0    19373 2023-05-21 20:29:49.000000 rvt_py-2.2.0/rvt/blend_func.py
--rw-rw-rw-   0        0        0   156675 2023-05-21 19:08:15.000000 rvt_py-2.2.0/rvt/default.py
--rw-rw-rw-   0        0        0    23080 2023-05-21 19:08:15.000000 rvt_py-2.2.0/rvt/tile.py
--rw-rw-rw-   0        0        0    68259 2023-05-21 20:03:46.000000 rvt_py-2.2.0/rvt/vis.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:15:45.833049 rvt_py-2.2.0/rvt_py.egg-info/
--rw-rw-rw-   0        0        0     5875 2023-05-22 19:15:45.000000 rvt_py-2.2.0/rvt_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-22 19:15:45.000000 rvt_py-2.2.0/rvt_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 19:15:45.000000 rvt_py-2.2.0/rvt_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-22 19:15:45.000000 rvt_py-2.2.0/rvt_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-22 19:15:45.000000 rvt_py-2.2.0/rvt_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      876 2023-05-22 19:15:45.838051 rvt_py-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1441 2023-05-22 19:15:35.000000 rvt_py-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 18:20:32.443253 rvt_py-2.2.1/
+-rw-rw-rw-   0        0        0    11567 2021-01-08 07:43:58.000000 rvt_py-2.2.1/LICENSE
+-rw-rw-rw-   0        0        0     5875 2023-05-23 18:20:32.443253 rvt_py-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4792 2023-05-21 19:08:15.000000 rvt_py-2.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 18:20:32.411574 rvt_py-2.2.1/rvt/
+-rw-rw-rw-   0        0        0      484 2023-05-21 19:08:15.000000 rvt_py-2.2.1/rvt/__init__.py
+-rw-rw-rw-   0        0        0    74237 2023-05-23 18:18:33.000000 rvt_py-2.2.1/rvt/blend.py
+-rw-rw-rw-   0        0        0    19373 2023-05-21 20:29:49.000000 rvt_py-2.2.1/rvt/blend_func.py
+-rw-rw-rw-   0        0        0   156675 2023-05-21 19:08:15.000000 rvt_py-2.2.1/rvt/default.py
+-rw-rw-rw-   0        0        0    23080 2023-05-21 19:08:15.000000 rvt_py-2.2.1/rvt/tile.py
+-rw-rw-rw-   0        0        0    68259 2023-05-21 20:03:46.000000 rvt_py-2.2.1/rvt/vis.py
+drwxrwxrwx   0        0        0        0 2023-05-23 18:20:32.443253 rvt_py-2.2.1/rvt_py.egg-info/
+-rw-rw-rw-   0        0        0     5875 2023-05-23 18:20:32.000000 rvt_py-2.2.1/rvt_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-23 18:20:32.000000 rvt_py-2.2.1/rvt_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 18:20:32.000000 rvt_py-2.2.1/rvt_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-23 18:20:32.000000 rvt_py-2.2.1/rvt_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-23 18:20:32.000000 rvt_py-2.2.1/rvt_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      876 2023-05-23 18:20:32.443253 rvt_py-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1441 2023-05-23 18:19:48.000000 rvt_py-2.2.1/setup.py
```

### Comparing `rvt_py-2.2.0/LICENSE` & `rvt_py-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rvt_py-2.2.0/PKG-INFO` & `rvt_py-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rvt_py
-Version: 2.2.0
+Version: 2.2.1
 Summary: Relief Visualization Toolbox Python library. It helps scientist visualize raster elevation model datasets. 
 Home-page: https://github.com/EarthObservation/RVT_py
 Author: ZRC SAZU and University of Ljubljana (UL FGG)
 Author-email: ziga.kokalj@zrc-sazu.si
 Project-URL: Documentation, https://rvt-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/EarthObservation/RVT_py
 Project-URL: Old RVT, https://iaps.zrc-sazu.si/en/rvt#v
```

### Comparing `rvt_py-2.2.0/README.md` & `rvt_py-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `rvt_py-2.2.0/rvt/blend.py` & `rvt_py-2.2.1/rvt/blend.py`

 * *Files 0% similar despite different names*

```diff
@@ -585,15 +585,15 @@
             max_colormap_cut = self.layers[i_img].max_colormap_cut
             if colormap is not None and len(image.shape) < 3:
                 norm_image = gray_scale_to_color_ramp(gray_scale=norm_image, colormap=colormap, output_8bit=False,
                                                       min_colormap_cut=min_colormap_cut,
                                                       max_colormap_cut=max_colormap_cut)
 
             # Blend current layer with background layer
-            if not rendered_image:
+            if rendered_image is None:
                 # if current layer has visualization applied, but there has been no rendering
                 # of images yet, than current layer will be the initial value of rendered_image
                 rendered_image = norm_image
                 continue
             else:
                 active = norm_image
                 background = rendered_image
```

### Comparing `rvt_py-2.2.0/rvt/blend_func.py` & `rvt_py-2.2.1/rvt/blend_func.py`

 * *Files identical despite different names*

### Comparing `rvt_py-2.2.0/rvt/default.py` & `rvt_py-2.2.1/rvt/default.py`

 * *Files identical despite different names*

### Comparing `rvt_py-2.2.0/rvt/tile.py` & `rvt_py-2.2.1/rvt/tile.py`

 * *Files identical despite different names*

### Comparing `rvt_py-2.2.0/rvt/vis.py` & `rvt_py-2.2.1/rvt/vis.py`

 * *Files identical despite different names*

### Comparing `rvt_py-2.2.0/rvt_py.egg-info/PKG-INFO` & `rvt_py-2.2.1/rvt_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rvt-py
-Version: 2.2.0
+Version: 2.2.1
 Summary: Relief Visualization Toolbox Python library. It helps scientist visualize raster elevation model datasets. 
 Home-page: https://github.com/EarthObservation/RVT_py
 Author: ZRC SAZU and University of Ljubljana (UL FGG)
 Author-email: ziga.kokalj@zrc-sazu.si
 Project-URL: Documentation, https://rvt-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/EarthObservation/RVT_py
 Project-URL: Old RVT, https://iaps.zrc-sazu.si/en/rvt#v
```

### Comparing `rvt_py-2.2.0/setup.cfg` & `rvt_py-2.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `rvt_py-2.2.0/setup.py` & `rvt_py-2.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rvt_py",
-    version="2.2.0",
+    version="2.2.1",
     author="ZRC SAZU and University of Ljubljana (UL FGG)",
     author_email="ziga.kokalj@zrc-sazu.si",
     description="Relief Visualization Toolbox Python library. "
                 "It helps scientist visualize raster elevation model datasets. ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EarthObservation/RVT_py",
```

