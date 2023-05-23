# Comparing `tmp/PyFibreBundle-1.3.tar.gz` & `tmp/PyFibreBundle-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFibreBundle-1.3.tar", last modified: Wed May 17 12:22:49 2023, max compression
+gzip compressed data, was "PyFibreBundle-1.3.1.tar", last modified: Tue May 23 11:13:37 2023, max compression
```

## Comparing `PyFibreBundle-1.3.tar` & `PyFibreBundle-1.3.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:22:49.298095 PyFibreBundle-1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-17 12:22:33.000000 PyFibreBundle-1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-17 12:22:49.298095 PyFibreBundle-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-17 12:22:33.000000 PyFibreBundle-1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-17 12:22:33.000000 PyFibreBundle-1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:22:49.298095 PyFibreBundle-1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:22:49.294095 PyFibreBundle-1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:22:49.294095 PyFibreBundle-1.3/src/PyFibreBundle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-17 12:22:49.000000 PyFibreBundle-1.3/src/PyFibreBundle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-17 12:22:49.000000 PyFibreBundle-1.3/src/PyFibreBundle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:22:49.000000 PyFibreBundle-1.3/src/PyFibreBundle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-17 12:22:49.000000 PyFibreBundle-1.3/src/PyFibreBundle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 12:22:49.000000 PyFibreBundle-1.3/src/PyFibreBundle.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:22:49.298095 PyFibreBundle-1.3/src/pybundle/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-17 12:22:33.000000 PyFibreBundle-1.3/src/pybundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-17 12:22:33.000000 PyFibreBundle-1.3/src/pybundle/bundle_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10163 2023-05-17 12:22:33.000000 PyFibreBundle-1.3/src/pybundle/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    17007 2023-05-17 12:22:33.000000 PyFibreBundle-1.3/src/pybundle/core_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-05-17 12:22:33.000000 PyFibreBundle-1.3/src/pybundle/core_interpolation_numba.py
--rw-r--r--   0 runner    (1001) docker     (123)    21812 2023-05-17 12:22:33.000000 PyFibreBundle-1.3/src/pybundle/mosaic.py
--rw-r--r--   0 runner    (1001) docker     (123)    24147 2023-05-17 12:22:33.000000 PyFibreBundle-1.3/src/pybundle/pybundle.py
--rw-r--r--   0 runner    (1001) docker     (123)    24243 2023-05-17 12:22:33.000000 PyFibreBundle-1.3/src/pybundle/super_res.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-17 12:22:33.000000 PyFibreBundle-1.3/src/pybundle/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:22:49.298095 PyFibreBundle-1.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-17 12:22:34.000000 PyFibreBundle-1.3/test/test_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-17 12:22:34.000000 PyFibreBundle-1.3/test/test_find_cores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-17 12:22:34.000000 PyFibreBundle-1.3/test/test_loc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-17 12:22:34.000000 PyFibreBundle-1.3/test/test_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-17 12:22:34.000000 PyFibreBundle-1.3/test/test_masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-17 12:22:34.000000 PyFibreBundle-1.3/test/test_masking_col.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-17 12:22:34.000000 PyFibreBundle-1.3/test/test_mosaic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-17 12:22:34.000000 PyFibreBundle-1.3/test/test_mosaic_col.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-17 12:22:34.000000 PyFibreBundle-1.3/test/test_pybundle_oop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-17 12:22:34.000000 PyFibreBundle-1.3/test/test_recon_tri_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-17 12:22:34.000000 PyFibreBundle-1.3/test/test_recon_tri_interp_col.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-17 12:22:34.000000 PyFibreBundle-1.3/test/test_simple_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-17 12:22:34.000000 PyFibreBundle-1.3/test/test_simple_processing_col.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-17 12:22:34.000000 PyFibreBundle-1.3/test/test_sr_sort_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-17 12:22:34.000000 PyFibreBundle-1.3/test/test_super_res.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-17 12:22:34.000000 PyFibreBundle-1.3/test/test_super_res_oop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:13:37.986429 PyFibreBundle-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-23 11:13:37.986429 PyFibreBundle-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 11:13:37.986429 PyFibreBundle-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:13:37.974429 PyFibreBundle-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:13:37.978429 PyFibreBundle-1.3.1/src/PyFibreBundle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-23 11:13:37.000000 PyFibreBundle-1.3.1/src/PyFibreBundle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-23 11:13:37.000000 PyFibreBundle-1.3.1/src/PyFibreBundle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 11:13:37.000000 PyFibreBundle-1.3.1/src/PyFibreBundle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-23 11:13:37.000000 PyFibreBundle-1.3.1/src/PyFibreBundle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 11:13:37.000000 PyFibreBundle-1.3.1/src/PyFibreBundle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:13:37.982429 PyFibreBundle-1.3.1/src/pybundle/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/src/pybundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/src/pybundle/bundle_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13352 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/src/pybundle/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17767 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/src/pybundle/core_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/src/pybundle/core_interpolation_numba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24572 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/src/pybundle/mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28182 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/src/pybundle/pybundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25481 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/src/pybundle/super_res.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-23 11:13:23.000000 PyFibreBundle-1.3.1/src/pybundle/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:13:37.986429 PyFibreBundle-1.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_find_cores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_loc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_masking_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_mosaic_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_processing_im_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_pybundle_oop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_recon_tri_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_recon_tri_interp_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_simple_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_simple_processing_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_sr_sort_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_super_res.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-23 11:13:24.000000 PyFibreBundle-1.3.1/test/test_super_res_oop.py
```

### Comparing `PyFibreBundle-1.3/LICENSE` & `PyFibreBundle-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3/PKG-INFO` & `PyFibreBundle-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFibreBundle
-Version: 1.3
+Version: 1.3.1
 Summary: Image processing of images acquired through fibre imaging bundle, including core removal, mosaicing and super-resolution..
 Author-email: Michael Hughes <m.r.hughes@kent.ac.uk>
 License: MIT License
         
         Copyright (c) [2022] [Michael Hughes]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `PyFibreBundle-1.3/README.md` & `PyFibreBundle-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3/pyproject.toml` & `PyFibreBundle-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyFibreBundle"
-version = "1.3"
+version = "1.3.1"
 description = "Image processing of images acquired through fibre imaging bundle, including core removal, mosaicing and super-resolution.."
 readme = "README.md"
 authors = [{ name = "Michael Hughes", email = "m.r.hughes@kent.ac.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `PyFibreBundle-1.3/src/PyFibreBundle.egg-info/PKG-INFO` & `PyFibreBundle-1.3.1/src/PyFibreBundle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFibreBundle
-Version: 1.3
+Version: 1.3.1
 Summary: Image processing of images acquired through fibre imaging bundle, including core removal, mosaicing and super-resolution..
 Author-email: Michael Hughes <m.r.hughes@kent.ac.uk>
 License: MIT License
         
         Copyright (c) [2022] [Michael Hughes]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `PyFibreBundle-1.3/src/PyFibreBundle.egg-info/SOURCES.txt` & `PyFibreBundle-1.3.1/src/PyFibreBundle.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 test/test_find_cores.py
 test/test_loc.py
 test/test_mask.py
 test/test_masking.py
 test/test_masking_col.py
 test/test_mosaic.py
 test/test_mosaic_col.py
+test/test_processing_im_type.py
 test/test_pybundle_oop.py
 test/test_recon_tri_interp.py
 test/test_recon_tri_interp_col.py
 test/test_simple_processing.py
 test/test_simple_processing_col.py
 test/test_sr_sort_stack.py
 test/test_super_res.py
```

### Comparing `PyFibreBundle-1.3/src/pybundle/__init__.py` & `PyFibreBundle-1.3.1/src/pybundle/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3/src/pybundle/bundle_calibration.py` & `PyFibreBundle-1.3.1/src/pybundle/bundle_calibration.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 fibre bundle images.
 
 
 BundleCalibration class stores the results of calibration for triangualar
 linear interpretation.
 
 
-@author: Mike Hughes
-Applied Optics Group, University of Kent
-https://github.com/mikehugheskent
+@author: Mike Hughes, Applied Optics Group, University of Kent
 """
 
 class BundleCalibration:
     
             
     coreX = None
     coreY = None
```

### Comparing `PyFibreBundle-1.3/src/pybundle/core.py` & `PyFibreBundle-1.3.1/src/pybundle/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,76 +3,144 @@
 PyFibreBundle is an open source Python package for image processing of
 fibre bundle images.
 
 This file contains core functions for locating the fibre bundle, masking
 and cropping the bundle, and simple methods for removing the core structure
 by spatial filtering.
 
-@author: Mike Hughes
-Applied Optics Group, University of Kent
-https://github.com/mikehugheskent
+@author: Mike Hughes, Applied Optics Group, University of Kent
 """
 
 import numpy as np
 import scipy.fft
 import math
 import time
 
-
 import cv2 as cv
 
 import pybundle
 from pybundle.bundle_calibration import BundleCalibration
-from pybundle.utility import average_channels, max_channels
+from pybundle.utility import average_channels, max_channels, extract_central
+
+
+def normalise_image(img, normImg, outputType = None):
+    """Normalise image by dividing pixelwise by a reference image. 
+    
+    Returns the normalised image as a 2D/3D numpy array. 
+    
+    If the image is 3D (colour) then the reference image can either by 2D 
+    (in which case it will be applied to each colour plane) or 3D.
+    
+    Optionally specify an output type to cast to. If no output type is 
+    specified, the output image will be float32. If uint8 or uint16 is 
+    specified, the image will be scaled to use the full range of that data
+    type.
+    
+    Arguments:
+        img     : 2D/3D numpy array, input image
+        normImg : 2D/3D numpy array, reference image to divide by
+        
+    Keyword Arguments:
+        outputType : str, if specified, output image will be cast to this type
+                     Default is None, in which case it will be returned as
+                     a float32.
+    """
+  
+        
+    # Slight speed advantage over float64
+    normImg = normImg.astype('float32')
+    img = img.astype('float32')
+
+    # If the normalisation image is 2D but image is 3D, we apply normalisation
+    # image to each plane
+    if img.ndim == 3 and normImg.ndim == 2:
+        normImg = np.expand_dims(normImg, 2)
+    
+    # Divide, avoiding division by zero  
+    out = np.divide(img, normImg, where=normImg!=0)
+  
+    # Below we adjust the output type if request using the optional
+    # keyword. If it is an integer type we normalise to use the full
+    # range
+    if outputType == 'uint8':
+        normImg = normImg / np.max(normImg) * 256
+    
+    if outputType == 'uint16':
+        normImg = normImg / np.max(normImg) * 65536
+        
+    if outputType is not None:
+        if normImg.dtype != outputType:
+            normImg = normImg.astype(outputType)   
+    
+    return out
 
-def normalise_image(img, normImg):
-    """Normalise image by dividing by a reference image
-    :param img: input image as 2D numpy array
-    :param normImg: reference image as 2D numpy array
-    :return: normalised image as 2D numpy array
-    """
-    img = img.astype('float64')
-    normImg = normImg.astype('float64')
-    normImg = np.divide(img, normImg, out=np.zeros_like(img).astype('float64'), where=normImg!=0)
-    return normImg
+    
 
+def g_filter(img, filterSize, kernelSize = None):
+    """ Applies 2D Gaussian filter to image. By default
+    the kernel size is 4 times the filter_size (sigma).
+    
+    Returns filtered image as numpy array.
     
+    Arguments:        
+        img          : input image as 2D/3D numpy array
+        filterSize   : float, sigma of Gaussian filter
+   
+    Keyword Arguments:   
+        kernelSize   : int, size of convolution kernal
 
-def g_filter(img, filter_size):
-    """ Applies 2D Gaussian filter to image. The kernel size is 8 times sigma.
-    :param img: input image as 2D numpy array
-    :param filter_size: sigma of Gaussian filter
-    :return: filtered image as 2D numpy array
-    """
-    kernel_size = round(filter_size * 8)              # Kernal size needs to be larger than sigma
-    kernel_size = kernel_size + 1 - kernel_size % 2   # Kernel size must be odd
-    img_filt = cv.GaussianBlur(img,(kernel_size,kernel_size), filter_size)
+    """
+    
+    # Kernal size needs to be larger than sigma
+    if kernelSize is None:
+        kernelSize = round(filterSize * 4)             
+    
+    # Force kernel size to be odd
+    kernelSize = kernelSize + 1 - kernelSize % 2       
+    
+    img_filt = cv.GaussianBlur(img,(kernelSize, kernelSize), filterSize)
+    
     return img_filt
 
 
-def median_filter(img, filter_size):
-    """Apply median filter to an image
-    :param img: input image as 2D numpy array
-    :param filter_size: filter size in pixels (filter is square)
+def median_filter(img, filterSize):
+    """ Applies 2D median filter to an image.
+    
+    Returns the filtered image as a 2D numpy array.
+    
+    Arguments:        
+        img          : input image as 2D/3D numpy array
+        filterSize   : float, sigma of Gaussian filter
+   
     """
-    imgFilt = cv.medianBlur(img, filter_size)
+    
+    imgFilt = cv.medianBlur(img, filterSize)
+   
     return imgFilt
 
 
 def find_core_spacing(img):
-    """ Estimate fibre bundle core spacing using peak in 2D Fourier transform. 
-    :param img: input image showing bundle as 2D numpy array
-    :return: estimated core spacing in pixels
+    """ Estimates fibre bundle core spacing using peak in 2D Fourier transform. 
+    
+    If the image is not square, a square will be cropped from the centre. 
+    It is therefore usually best to crop the image to the bundle 
+    before passing it to this function.
+    
+    Returns core spacing as float.
+    
+    Arguments: 
+        img  : input image showing bundle as 2D/3D numpy array
+        
     """
     
+    # If colour image, we take the mean across the channels
     imgAv = average_channels(img)
     
     # Ensure image is square
-    size = np.min(np.shape(imgAv))
-    imgAv = imgAv[:size,:size]
+    imgAv = extract_central(imgAv)
     
     # Look at log-scaled 2D FFT
     fd = np.log(np.abs(np.fft.fftshift(np.fft.fft2(imgAv))))
    
     # Average radial profile     
     rad = pybundle.radial_profile(fd, (np.shape(fd)[0] / 2, np.shape(fd)[1] / 2))
     
@@ -85,77 +153,94 @@
     # Find the point of fastest drop
     firstMinRange = np.round(np.shape(radDiff)[0] / 10).astype(int)
     firstMin = np.argmin(radDiff[0:firstMinRange]).astype(int)
     
     # Find point after fastest drop where gradient is positive    
     startReg = int((np.argwhere(radDiff[firstMin:] >0)[0] + firstMin))
     peakPos = np.argmax(radDiff[startReg:]) + startReg
-    coreSpacing = size / peakPos 
-
+    coreSpacing = np.shape(imgAv)[0] / peakPos 
+    
     return coreSpacing
 
 
 
 def edge_filter(imgSize, edgePos, skinThickness):
-    """ Create a 2D edge filter with cosine smoothing
-    :param imgSize: size of (sqaure) images which will be processed 
-    :param edgePos: spatial frequency of cut-off
-    :param skinThickness: slope of edge
-    :return mask: spatial frequency domain filter as a 2D numpy array
+    """ Creates a 2D edge filter with cosine smoothing.
+    
+    Returns the filter in spatial frequency domain filter as a 2D numpy array.
+   
+    Arguments: 
+        imgSize       : size of (square) images which will be processed, and
+                        size of filter output
+        edgePos       : spatial frequency of cut-off
+        skinThickness : slope of edge, the distance, in spatial frequency, over 
+                        which it goes from 90% to 10%                        
     """
 
     circleRadius = imgSize / edgePos
     thickness = circleRadius * skinThickness
 
     innerRad = circleRadius - thickness / 2
     xM, yM = np.meshgrid(range(imgSize),range(imgSize))
     imgRad = np.sqrt( (xM - imgSize/2) **2 + (yM - imgSize/2) **2)
     mask =  np.cos(math.pi / (2 * thickness) * (imgRad - innerRad))**2
     mask[imgRad < innerRad ] = 1
     mask[imgRad > innerRad + thickness] = 0
+    
     return mask        
 
 
 def filter_image(img, filt):
-    """ Apply a Fourier domain filter to an image. Filter must be same size as image.
-    :param img: input image (spatial domain), 2D numpy array
-    :param filt: spatial frequency domain representation of filter, 2D numpy array
-    :return: filtered image, 2D numpy array
+    """ Applies a Fourier domain filter to an image, such as created by
+    edge_filter(). Filter must be same size as image (x and y) but not
+    multi-channel (i.e. a 2D array).
+    
+    Returns filtered image as 2D/3D numpy array.
+    
+    Arguments: 
+        img    : input image (spatial domain), 2D/3D numpy array
+        filt   : spatial frequency domain representation of filter, 2D numpy array        
     """
 
     fd = scipy.fft.fftshift(scipy.fft.fft2(img, axes = (0,1)),axes = (0,1))
     if img.ndim == 2:
         fd = fd * filt
     elif img.ndim == 3:
         fd = fd * np.expand_dims(filt, 2)  
         
     return np.abs(scipy.fft.ifft2(scipy.fft.fftshift(fd, axes = (0,1)), axes = (0,1)))
 
 
 def find_bundle(img, **kwargs):
     """ Locate fibre bundle by thresholding and searching for largest
-    connected region. Returns tuple of (centreX, centreY, radius)
-    :param img: input image of fibre bundle, 2D numpy array
-    :param filterSize: sigma of Gaussian filter applied to remove core pattern, default to 4
-    :return: tuple of (centreX, centreY, radius)
+    connected region. 
+    
+    Returns tuple of (centreX, centreY, radius).
+    
+    Arguments: 
+
+        img        : input image of fibre bundle, 2D numpy array
+        
+    Keyword Arguments:   
+   
+        filterSize : sigma of Gaussian filter applied to remove core pattern, 
+                     defaults to 4
     """
     
     filterSize = kwargs.get('filterSize', 4)
     
-    #imgFilt = average_channels(img)
+    # If we have a colour image, take max value across channels
     imgFilt = max_channels(img)
     
     # Filter to minimise effects of structure in bundle
     imgFilt = g_filter(imgFilt, filterSize)
     imgFilt = (imgFilt / np.max(imgFilt) * 255).astype('uint8')
     
     # Threshold to binarise and then look for connected regions
     thres, imgBinary = cv.threshold(imgFilt,0,1,cv.THRESH_BINARY+cv.THRESH_OTSU)
-    #plt.imshow(imgBinary)
-
     num_labels, labels, stats, centroid  = cv.connectedComponentsWithStats(imgBinary, 8, cv.CV_32S)
     
     # Region 0 is background, so find largest of other regions
     sizes = stats[1:,4]
     biggestRegion = sizes.argmax() + 1
     
     # Find distance from centre to each edge and take minimum as safe value for radius
@@ -170,108 +255,157 @@
     return centreX, centreY, radius
 
 
 
 ################ MASKING AND CROPPING ###################################
     
 
-def crop_rect(img,loc):
+def crop_rect(img, loc):
     """Extracts a square around the bundle using specified co-ordinates.
-    :param img: input image as 2D numpy array
-    :param loc: location to crop, specified as bundle location tuple of (centreX, centreY, radius)
-    :return: tuple of (cropped image as 2D numpy array, new location tuple)
+    
+    Returns tuple of (cropped image as 2D numpy array, new location tuple)
+
+    Arguments:  
+        img  : input image as 2D numpy array
+        loc  : location to crop, specified as bundle location tuple of 
+               (centreX, centreY, radius)
     """
+    
     cx,cy, rad = loc
     imgCrop = img[cy-rad:cy+ rad, cx-rad:cx+rad]
     
     # Correct the co-ordinates of the bundle so that they
     # are correct for new cropped image
     newLoc = [rad,rad,loc[2]]
    
     return imgCrop, newLoc
 
 
 
 
 def get_mask(img, loc):
-    """ Returns a circular mask, 1 inside bundle, 0 outside bundle using specified
-    bundle co-ordinates. Mask image has same dimensions as input image.
-    :param img: img used to determine size of mask, 2D numpy array
-    :param loc: location of bundle used to determine location of mask, tuple of (centreX, centreY, radius)
-    :return: mask as 2D numpy array
+    """ Returns a circular mask, 1 inside bundle, 0 outside bundle, using specified
+    bundle co-ordinates. Mask image has same dimensions as first two
+    dimensions of input image (i.e. does not return a mask for each colour plane).
+    
+    Returns mask as 2D numpy array.
+    
+    Arguments:  
+         img  : img used to determine size of mask, 2D numpy array
+         loc  : location of bundle used to determine location of mask, 
+                tuple of (centreX, centreY, radius)
     """
     cx, cy, rad = loc
  
-    mY,mX = np.meshgrid(range(img.shape[0]),range(img.shape[1]))
+    mY,mX = np.meshgrid(range(img.shape[0]), range(img.shape[1]))
    
     m = np.square(mX - cx) +  np.square(mY - cy)   
     imgMask = np.transpose(m < rad**2)
      
     return imgMask
 
     
 def apply_mask(img, mask):
-    """Sets all pixels outside bundle to 0 using a pre-defined mask. 
-    :param img: input image as 2D numpy array
-    :param mask: mask as 2D numy array with same dimensions as img, with areas to be kept as 1 and areas to be masked as0.
+    """Sets all pixels outside bundle to 0 using a pre-defined mask. If the
+    image is 3D, the mask will be applied to each colour plane.
+    
+    Arguments:  
+         img   : input image as 2D numpy array
+         mask  : mask as 2D numy array with same dimensions as img, 
+                 with areas to be kept as 1 and areas to be masked as 0.
     """
+    
     if img.ndim == 3:
         m = np.expand_dims(mask, 2)
-        #imgMasked = np.multiply(img, np.repeat(mask, np.shape(img)[2], 2))
     else:
         m = mask
     imgMasked = np.multiply(img, m)
     
     return imgMasked
   
 
-def auto_mask(img, **kwargs):
-    """ Locates bundle and sets pixels outside to 0   
-    :param img: input image as 2D numpy array
-    :param loc: optional location of bundle as tuple of (centreX, centreY, radius), defaults to determining this using find_bundle
-    :return: masked image as 2D numpy array
+def auto_mask(img, loc = None, **kwargs):
+    """ Locates bundle and sets pixels outside to 0 .
+    
+    Arguments:  
+        img  : input image as 2D numpy array
+    
+    Keyword Arguments:
+        loc    : optional location of bundle as tuple of (centreX, centreY, radius), 
+                 defaults to determining this using find_bundle
+        Others : if loc is not specified, other optional keyword arguments will
+                 be passed to find_bundle.
+
+
     """
-    loc = pybundle.find_bundle(img, **kwargs)
+    if loc is None:
+        loc = pybundle.find_bundle(img, **kwargs)
     mask = pybundle.get_mask(img, loc)
     imgMasked = pybundle.apply_mask(img, mask)
+    
     return imgMasked
 
     
-def auto_mask_crop(img, **kwargs):
-    """ Locates bundle, sets pixels outside to 0 and returns cropped image
-    around bundle
-    :param img: input image as 2D numpy array
-    :param loc: optional location of bundle as tuple of (centreX, centreY, radius), defaults to determining this using find_bundle
-    :return: masked and cropped image as 2D numpy array
+def auto_mask_crop(img, loc = None, **kwargs):
+    """ Locates bundle, sets pixels outside to 0, and returns cropped image
+    around bundle.
+    
+    Arguments:  
+
+        img:  input image as 2D numpy array
+        
+    Keyword Arguments:
+    
+        loc:     optional location of bundle as tuple of (centreX, centreY, radius), 
+                 defaults to determining this using find_bundle
+        Others : if loc is not specified, other optional keyword arguments will
+                 be passed to find_bundle.
     """
-    loc = pybundle.find_bundle(img, **kwargs)
+    
+    if loc is None:
+        loc = pybundle.find_bundle(img, **kwargs)
     imgMasked = pybundle.auto_mask(img)
     imgCropped = pybundle.crop_rect(imgMasked, loc)
+    
     return imgCropped            
 
 
 
-def crop_filter_mask(img, loc, mask, filterSize, **kwargs):
+def crop_filter_mask(img, loc, mask, filterSize, resize = False, **kwargs):
     """ For convenient quick processing of images. Sequentially crops image to 
     bundle, applies Gaussian filter and then sets pixels outside bundle to 0.
-    Set loc to None to automatically locate bundle. Optional parameter resize
-    allows the output images to be rescaled. If using autolocate, can
-    optionally specify find_bundle options as additional arguments.    
-    :param img: input image, 2D numpy array
-    :param loc: location of bundle as tuple of (centreX, centreY, radius), set to None to determining this using find_bundle
-    :param mask: 2D numpy array with value of 1 inside bundle and 0 outside bundle
-    :param filterSize: sigma of Gaussian filter
-    :param resize: optional size to rescale output image to, if not specified there will be no resize
-    :return: output image as 2D numpy array
+    Set loc to None to automatically locate bundle. Optional parameter 'resize'
+    allows the output images to be rescaled. If using auto-locate, can
+    optionally specify find_bundle() options as additional keyword arguments. 
+    
+    Returns output image as 2D/3D numpy array
+    
+    Arguments:  
+
+        img        : input image, 2D/3D numpy array
+        loc        : location of bundle as tuple of (centreX, centreY, radius), 
+                      set to None to determining this using find_bundle
+        mask       : 2D numpy array with value of 1 inside bundle and 0 outside bundle
+        filterSize : sigma of Gaussian filter
+        
+    Keyword Arguments:
+    
+        resize     : size to rescale output image to, default is no resize
+        Others     : if loc is not specified, other optional keyword arguments will
+                    be passed to find_bundle.
+        
     """
     
-    resize = kwargs.get('resize', False)
     if loc is None:
         loc = pybundle.find_bundle(img, **kwargs)
+    
     img = pybundle.g_filter(img, filterSize)
+    
     img = pybundle.apply_mask(img, mask)
+    
     img, newLoc = pybundle.crop_rect(img, loc)
+    
     if resize is not False:
         img = cv.resize(img, (resize,resize))        
     
     return img
```

### Comparing `PyFibreBundle-1.3/src/pybundle/core_interpolation.py` & `PyFibreBundle-1.3.1/src/pybundle/core_interpolation.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 """
 PyFibreBundle is an open source Python package for image processing of
 fibre bundle images.
 
 This file contains functions related to triangular linear interpolation 
 between cores, including functions for finding cores.
 
-@author: Mike Hughes
-Applied Optics Group, University of Kent
-https://github.com/mikehugheskent
+@author: Mike Hughes, Applied Optics Group, University of Kent
 """
 
 
 import numpy as np
 import math
 import time
 
@@ -35,16 +33,22 @@
     numbaAvailable = True
 except:
     numbaAvailable = False
  
 
 def find_cores(img, coreSpacing):
      """ Find cores in bundle image using regional maxima. Generally fast and
-     accurate. CoreSpacing is an estimate of the separation between cores in
-     pixels.
+     accurate. 
+     
+     Returns tuple of (x_pos, y_pos) where x_pos and y_pos are 1D numpy arrays.
+     
+     Arguments:
+         img         : 2D/3D numpy array
+         coreSpacing : float, estimate of the separation between cores in
+                       pixels.
      """
      # Pre-filtering helps to minimse noise and reduce efffect of
      # multimodal patterns
      imgF = pybundle.g_filter(img, coreSpacing/5)
 
      # If a colour image, convert to greyscale by taking the maximum value across the channels
      imgF = pybundle.max_channels(imgF)
@@ -95,24 +99,29 @@
      return cx, cy
 
 
 def core_values(img, coreX, coreY, filterSize, **kwargs):
     """ Extract intensity of each core in fibre bundle image. First applies a
     Gaussian filter unless filterSize is None. Supports JIT acceleration
     if numba is installed.
-    :param coreX: 1D numpy array giving x co-ordinates of core centres
-    :param coreY: 1D numpy array giving y co-ordinates of core centres
-    :param filterSize: sigma of Gaussian filter
-    :param numba: optional, if true numba JIT used for faster execution, defaults to False.
+    
+    Arguments:
+        coreX      : 1D numpy array giving x co-ordinates of core centres
+        coreY      : 1D numpy array giving y co-ordinates of core centres
+        filterSize : float, sigma of Gaussian filter
+    
+    Keyword Arguments:    
+
+        numba  : optional, if true numba JIT used for faster execution, defaults to False.
     """
     numba = kwargs.get('numba', False)
     
     if filterSize is not None:
         img = pybundle.g_filter(img, filterSize)
-
+        
     if numba and numbaAvailable:
         cInt = core_value_extract_numba(img, coreX, coreY)
     else:
         cInt = img[coreY, coreX]
         
     return cInt
  
@@ -120,45 +129,49 @@
 def calib_tri_interp(img, coreSize, gridSize, **kwargs):
     """ Performs calibration to allow subsequent core removal by triangular linear interpolation.
     Reconstructed images will be of size (gridSize, gridSize). 'coreSize' is used by
     the core finding routine, and should be an estimate of the core spacing. This function
     returns the entire calibration as an instance of BundleCalibration which can subsequently by used 
     by recon_tri_interp. If background and/or normalisation images are specified, subsequent 
     reconstructions will have background subtraction and/or normalisation respectively.
+    
+    Returns an instance of BundleCalibration
+
         
     Thanks to Cheng Yong Xin, Joseph, who collaborated in implementation of this function.
     
-    :param img: calibration image of bundle as 2D (mono) or 3D (colour) numpy array
-    :param coreSize: estimate of average spacing between cores
-    :param gridSize: output size of image, supply a single value, image will be square
-    :param centreX: optional, x centre location of bundle, if not specified will be determined automatically
-    :param centreY: optional, y centre location of bundle, if not specified will be determined automatically
-    :param radius: optional, radius of bundle, if not specified will be determined automatically
-    :param filterSize: optional, sigma of Gaussian filter applied, defaults to  0 (no filter)
-    :param background: optional, image used for background subtractionn as 2D numpy array
-    :param normalise: optional, image used for normalisation, as 2D numpy array. Can be same as 
-                      calibration image, defaults to no normalisation
-    :param autoMask: optional, boolean, if true the calibration image will be masked to prevent 
+    Arguments:
+        img        : calibration image of bundle as 2D (mono) or 3D (colour) numpy array
+        coreSize   : float, estimate of average spacing between cores
+        gridSize   : int, output size of image, supply a single value, image will be square
+        
+    Keyword Arguments:    
+        centreX    : int, optional, x centre location of bundle, if not specified will be determined automatically
+        centreY    : int, optional, y centre location of bundle, if not specified will be determined automatically
+        radius     : int, optional, radius of bundle, if not specified will be determined automatically
+        filterSize : float, optional, sigma of Gaussian filter applied, defaults to  0 (no filter)
+        background : optional, image used for background subtraction as 2D numpy array
+        normalise  : optional, image used for normalisation, as 2D numpy array. Can be same as 
+                     calibration image, defaults to no normalisation
+        autoMask   : optional, boolean, if true the calibration image will be masked to prevent 
                      spurious core detections outside of bundle, defualts to True
-    :param mask: optional, boolean, when reconstructing output image will be masked outside of 
-                 bundle, defaults to True
-    :return: instance of BundleCalibration
+        mask       : optional, boolean, when reconstructing output image will be masked outside of 
+                     bundle, defaults to True
     """
 
     centreX = kwargs.get('centreX', -1)
     centreY = kwargs.get('centreY', -1)
     radius = kwargs.get('radius', -1)
     filterSize = kwargs.get('filterSize', 0)
     normalise = kwargs.get('normalise', None)
     autoMask = kwargs.get('autoMask', True)
     mask = kwargs.get('mask', True)
     background = kwargs.get('background', None)
     if autoMask:
         img = pybundle.auto_mask(img)
-
     # Find the cores in the calibration image
     coreX, coreY = pybundle.find_cores(img, coreSize)
     coreX = np.round(coreX).astype('uint16')
     coreY = np.round(coreY).astype('uint16')
 
     # Default values
     if centreX < 0:
@@ -180,42 +193,46 @@
     return calib
 
  
 def init_tri_interp(img, coreX, coreY, centreX, centreY, radius, gridSize, **kwargs):
     """ Used by calib_tri_interp to perform Delaunay triangulation of core positions, 
     and find each pixel of reconstruction grid in barycentric co-ordinates w.r.t. 
     enclosing triangle.
-    :param img: calibration image as 2D (mono) or 3D (colour) numpy array
-    :param coreX: x centre of each core as 1D numpy array
-    :param coreY: y centre of each core as 1D numpy array
-    :param centreX: x centre location of bundle (reconstruction will be centred on this)
-    :param centreY: y centre location of bundle (reconstruction will be centred on this)
-    :param radius: radius of bundle (reconstruction will cover a square out to this radius)
-    :param gridSize: output size of image, supply a single value, image will be square
-    :param filterSize: optional, sigma of Gaussian filter applied, defaults to no filter
-    :param background: optional, image used for background subtractionn as 2D numpy array
-    :param normalise: optional, image used for normalisation, as 2D numpy array. Can be same as 
-                      calibration image, defaults to no normalisation
-    :param mask: optional, boolean, when reconstructing output image will be masked outside 
-                 of bundle, defaults to True
-    :return: instance of BundleCalibration
     
+    Returns instance of BundleCalibration.
+    
+    Arguments:
+         img     : calibration image as 2D (mono) or 3D (colour) numpy array
+         coreX   : x centre of each core as 1D numpy array
+         coreY   : y centre of each core as 1D numpy array
+         centreX : x centre location of bundle (reconstruction will be centred on this)
+         centreY : y centre location of bundle (reconstruction will be centred on this)
+         radius  : radius of bundle (reconstruction will cover a square out to this radius)
+    
+    Keyword Arguments:    
+         gridSize   : output size of image, supply a single value, image will be square
+         filterSize : optional, sigma of Gaussian filter applied, defaults to no filter
+         background : optional, image used for background subtractionn as 2D numpy array
+         normalise  : optional, image used for normalisation, as 2D numpy array. Can be same as 
+                      calibration image, defaults to no normalisation
+         mask       : optional, boolean, when reconstructing output image will be masked outside 
+                      of bundle, defaults to True    
     """
+    
     filterSize = kwargs.get('filterSize', None)
     normalise = kwargs.get('normalise', None)
     background = kwargs.get('background', None)
     mask = kwargs.get('mask', True)
     numba = kwargs.get('numba', True)
 
     if img.ndim > 2:    # Colour image if we have a third dimension to image
         col = True
     else:
         col = False
 
-
     # Delaunay triangulation over core centre locations
     points = np.vstack((coreX, coreY)).T
     #t1 = time.perf_counter()
     tri = Delaunay(points)
     #print("Delauany time ", str(time.perf_counter() - t1))
 
     # Make a vector of all the pixels in the reconstruction grid
@@ -279,19 +296,21 @@
 
     return calib
 
 
 def barycentric(nPixels, tri, mapping, interpPoints):
     """ Converts a set of Cartesian co-ordinates to barycentric co-ordinates.
     Assumes a prior Delaunay triangulation and simplex stored in mapping.
-    :param nPixels : Number of pixels in grid 
-    :param tri     : Delaunay triangulation
-    :param mapping : Output from Delaunay.find_simplex, records the co-ordinates of the
-                     three triangle vertices surrounding each point
-    :param interpPoints : Cartesian grid co-ordinates
+    
+    Arguments:
+         nPixels      : Number of pixels in grid 
+         tri          : Delaunay triangulation
+         mapping      : Output from Delaunay.find_simplex, records the co-ordinates of the
+                        three triangle vertices surrounding each point
+         interpPoints : Cartesian grid co-ordinates
     """
     # Left here as could try numba optimisation in future
     # baryCoords = np.zeros([nPixels, 3])
     #  c = np.zeros([3,2,nPixels])
     # for i in range(nPixels):
     #     c[:,:,i] = tri.transform[mapping[i]]
                                                  
@@ -300,18 +319,21 @@
     baryCoords = np.c_[b0, 1 - b0.sum(axis=1)]                                              
                                                   
     return baryCoords
 
 
 def tri_interp_normalise(calibIn, normalise):
     """ Updates a calibration with a new normalisation without requiring
-    full recalibration
-    :param calibIn: input calibration, instance of BundleCalibration
-    :param normalise: normalisation image as 2D/3D numpy array, or None to remove normalisation
-    :return: updated instance of BundleCalibration
+    full recalibration.
+    
+    Returns updated instance of BundleCalibration
+    
+    Arguments:
+         calibIn   : input calibration, instance of BundleCalibration
+         normalise : normalisation image as 2D/3D numpy array, or None to remove normalisation
     """
     calibOut = calibIn
 
     if normalise is not None:
         calibOut.normaliseVals = pybundle.core_values(normalise, calibOut.coreX, calibOut.coreY,calibOut.filterSize).astype('double')
         calibOut.normalise = normalise
 
@@ -320,18 +342,23 @@
         calibOut.normalise = None
     
     return calibOut
 
 
 def tri_interp_background(calibIn, background):
      """ Updates a calibration with a new background without requiring
-     full recalibration
-     :param calibIn: bundle calibration, instance of BundleCalibration
-     :param background: background image as 2D/3D numpy array
+     full recalibration.
+     
+     Returns updated instance of BundleCalibration
+
+     Arguments:
+          calibIn: bundle calibration, instance of BundleCalibration
+          background: background image as 2D/3D numpy array
      """
+     
      calibOut = calibIn
 
      if background is not None:
          calibOut.backgroundVals = pybundle.core_values(background, calibOut.coreX, calibOut.coreY,calibOut.filterSize).astype('double')
          calibOut.background = background
 
      else:
@@ -339,26 +366,31 @@
          calibOut.background = None
          
      return calibOut
 
 
 def recon_tri_interp(img, calib, **kwargs):
      """ Removes core pattern using triangular linear interpolation. Requires an initial
-     calibration using calib_tri_interp
-     :param img: raw image to be reconstructed as 2D (mono) or 3D (colour) numpy array
-     :param calib: bundle calibration as instance of BundleCalibration
-     :param numba: optional, if true use JIT acceleration using Numba, default to False
-     :return: reconstructed image as 2D/3D numpy array
+     calibration using calib_tri_interp.
+     
+     Returns reconstructed image as 2D/3D numpy array.
+
+     Arguments:
+          img: raw image to be reconstructed as 2D (mono) or 3D (colour) numpy array
+          calib: bundle calibration as instance of BundleCalibration
+          
+     Keyword Arguments:     
+          numba: optional, if true use JIT acceleration using Numba, default is False
      """
     
      numba = kwargs.get('numba', True)
 
      # Extract intensity from each core
      cVals = pybundle.core_values(
-         img, calib.coreX, calib.coreY, calib.filterSize, **kwargs).astype('double')
+         img, calib.coreX, calib.coreY, calib.filterSize, **kwargs).astype('float64')
 
      if calib.background is not None:
          cVals = cVals - calib.backgroundVals    
       
      if calib.normalise is not None:
          cVals = (cVals / calib.normaliseVals * 255)    
 
@@ -391,21 +423,26 @@
     """Produces pixel values based on linear interpolation between supplied
     surrounding triangle vertex core intensity values. The core values, cVals, 
     are supplied as a 1D numpy array, giving the intensity extraacted from each core.
     The indices of the three cores surrounding each pixel in the reconstruction
     grid are given by coreIdx, a 2D  numpy array. The mapping, which provides
     the tringle index for each reconstruction grid pixel, is used here purely
     for intentifying pixels which lie outside the complex hull of the bundle, so
-    that these can be set to 0.  
-    :param baryCoords: barycentric co-ordinates of each pixel in reconstruction grid
-        as 2D numpy array of size (3, num_pixels)
-    :param cVals: intensity values from each core as 1D numpy array
-    :param coreIdx: the indices of the three cores making up the enclosing triangle
-        for each reconstruction grid pixel, as 2D numpy array of size (3, num_pixels)
-    :return: value of each pixel in the reconstruction grid, as 1D numpy array
+    that these can be set to 0. 
+    
+    Returns value of each pixel in the reconstruction grid, as 1D numpy array
+
+    Arguments:
+         baryCoords  : barycentric co-ordinates of each pixel in reconstruction grid
+                       as 2D numpy array of size (3, num_pixels)
+         cVals       : intensity values from each core as 1D numpy array
+         coreIdx     : the indices of the three cores making up the enclosing triangle
+                       for each reconstruction grid pixel, as 2D numpy array of 
+                       size (3, num_pixels)
+         mapping     : pixel to triangle mapping, as generated by init_tri_interp              
     """
    
     if cVals.ndim == 2:
         pixelVal = np.zeros((np.shape(baryCoords)[0], np.shape(cVals)[1]))
         for iChannel in range(np.shape(cVals)[1]):
             val = baryCoords * cVals[:, iChannel][coreIdx]
             pixelVal[:,iChannel] = np.sum(val, 1)
```

### Comparing `PyFibreBundle-1.3/src/pybundle/core_interpolation_numba.py` & `PyFibreBundle-1.3.1/src/pybundle/core_interpolation_numba.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 PyFibreBundle is an open source Python package for image processing of
 fibre bundle images.
 
 This file contains functions related to triangular linear interpolation 
 between cores which are accelerated using the JIT functionality of the numba
 package.
 
-@author: Mike Hughes
-Applied Optics Group, University of Kent
-https://github.com/mikehugheskent
+@author: Mike Hughes, Applied Optics Group, University of Kent
 """
 
 
 import numba
 from numba import jit, njit
 import numpy as np
 
 @jit(nopython = True)   
 def core_value_extract_numba(img, coreX, coreY):
-    """ Extract intensity of each core in fibre bundle image using JIT compiler
+    """ Extract intensity of each core in fibre bundle image using JIT compiler.
     
-    :param coreX: 1D numpy array giving x co-ordinates of core centres
-    :param coreY: 1D numpy array giving y co-ordinates of core centres
-    :param filterSize: sigma of Gaussian filter
-    :param numba: optional, if true numba JIT used for faster executio, defaults to False.
-    :return: core intensity values as 1D numpy array 
+    Returns core intensity values as 1D numpy array 
+    
+    Arguments:
+           coreX      : 1D numpy array giving x co-ordinates of core centres
+           coreY      : 1D numpy array giving y co-ordinates of core centres
+           filterSize : float, sigma of Gaussian filter
+     
     """
     if img.ndim == 2:
         nCores = np.shape(coreX)[0]
         cInt = np.zeros((nCores),dtype=numba.int64)
         for i in range(nCores):
             cInt[i] = (img[coreY[i], coreX[i]])
     elif img.ndim == 3:
@@ -49,30 +49,34 @@
     surrounding triangle vertex core intensity values. The core values, cVals, 
     are supplied as a 1D numpy array, giving the intensity extraacted from each core.
     The indices of the three cores surrounding each pixel in the reconstruction
     grid are given by coreIdx, a 2D  numpy array. The mapping, which provides
     the tringle index for each reconstruction grid pixel, is used here purely
     for intentying pixels which lie outside the complex hull of the bundle, so
     that these can be set to 0.  
-    :param baryCoords: barycentric co-ordinates of each pixel in reconstruction grid
-        as 2D numpy array of size (3, num_pixels)
-    :param cVals: intensity values from each core as 1D numpy array
-    :param coreIdx: the indices of the three cores making up the enclosing triangle
-        for each reconstruction grid pixel, as 2D numpy array of size (3, num_pixels)
-    :return: value of each pixel in the reconstruction grid, as 1D numpy array
+    
+    Returns value of each pixel in the reconstruction grid, as 1D numpy array
+
+           baryCoords : barycentric co-ordinates of each pixel in reconstruction grid
+                        as 2D numpy array of size (3, num_pixels)
+           cVals      : intensity values from each core as 1D numpy array
+           coreIdx    : the indices of the three cores making up the enclosing triangle
+                        for each reconstruction grid pixel, as 2D numpy array 
+                        of size (3, num_pixels)
+           mapping    : as output in BundleCalibration from calib_tri_interp()
+           mask       : mask to apply 2D numpy array of 1s and 0.
+                        
     """
     
     assert (cVal.ndim == 1 or cVal.ndim == 2), "Pixel Values in cVal must be 1D (mono) or 2D (colour)"
     
     if cVal.ndim == 2:
         pixelVal = np.zeros((np.shape(baryCoords)[0], np.shape(cVal)[1]))
     else:
-        pixelVal = np.zeros((np.shape(baryCoords)[0]))
-
-         
+        pixelVal = np.zeros((np.shape(baryCoords)[0]))         
 
     if cVal.ndim == 2:   # Colour
         if mask is None:
             for i in range(np.shape(baryCoords)[0]):
                 for c in range(np.shape(cVal)[1]):
                     pixelVal[i,c] =  baryCoords[i,0] * cVal[coreIdx[i,0],c] + baryCoords[i,1] * cVal[coreIdx[i,1],c] + baryCoords[i,2] * cVal[coreIdx[i,2],c]
         else:
@@ -92,19 +96,23 @@
     pixelVal[mapping < 0] = 0
         
     return pixelVal   
   
     
 @jit(nopython=True)
 def apply_mask_numba(img, mask):
-    """ Numba optimised version of apply_mask. Applies a mask to an input image. 
-    :param img: input image as 2D numpy array
-    :param mask: mask image, 2D numpy array with 1 for pixels to keep and 0 for
-      pixels to set to 0. Must be same size as img
-    :return: masked image as 2D numpy array
+    """ Numba optimised version of apply_mask. Applies a mask to an input image.
+    
+    Returns the masked image as a 2D numpy array.
+
+    
+    Arguments:
+           img  : input image as 2D numpy array
+           mask : mask image, 2D numpy array with 1 for pixels to keep and 0 for
+                  pixels to set to 0. Must be same size as img
     """
     w,h = np.shape(img)
    
     for x in range(w):
         for y in range(h):
             img[x,y] = img[x,y] * mask[x,y]
```

### Comparing `PyFibreBundle-1.3/src/pybundle/mosaic.py` & `PyFibreBundle-1.3.1/src/pybundle/mosaic.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,91 @@
 # -*- coding: utf-8 -*-
 """
 PyFibreBundle is an open source Python package for image processing of
 fibre bundle images.
 
-
 Mosaic class provides mosaicing functionality.
 
-
-@author: Mike Hughes
-Applied Optics Group, University of Kent
-https://github.com/mikehugheskent
+@author: Mike Hughes, Applied Optics Group, University of Kent
 """
     
 import numpy as np
 import math
 import time
+
 import cv2 as cv
+
 from pybundle import pybundle
+from pybundle.utility import extract_central
 
 ##############################################################################        
 class Mosaic:
+    """ The Mosaic class is used for producing mosaics from a sequence of
+    images. After instantiating a Mosaic object, use add() to add in images
+    and get_mosaic to obtain the current mosaic image.
+    
+    Arguments:
+        mosaicSize    : int, square size of mosaic image
+        
+    Keyword Arguments:
+        resize         : int, images will be resized to a square this size,
+                         default is None meaning no resize.
+        templateSize   : int, size of square to extract to use as template
+                         for shift detection. Default is 1/4 image size.
+        refSize        : int, size of square to extract to use as image
+                         to compare template to for shift detection. 
+                         Default is 1/2 image size.
+        cropSize       : int, input images are cropped to a circle of this 
+                         diameter before insertion. (default is 
+                         0.9 x size of first image added)
+        imageType      : str, data type for mosaic, default is the same
+                         as first image added
+        blend          : boolean, if True (default), images will be added blended,
+                         otherwise they are added dead-leaf
+        blendDist      : int, distance in pixels from edge of inserted 
+                         image to blend with mosaic, default is 40
+        minDistforAdd  : int, minimum distance moved before an image
+                         will be added to the mosaic, default is 25
+        initialX       : int, starting positon of mosaic, default is centre
+        initialY       : int, starting positon of mosaic, default is centre  
+        boundaryMethod : method to deal with reaching edge: CROP, SCROLL or
+                         EXPAND, default is CROP
+        expandStep     : int, amount to expand by if EXPAND boundaryMethod
+                         is used
+        resetThresh    : float, mosaic will reset if correlation peak is
+                         below this, default is None (ignore)
+        resetIntensity : float, mosaic will reset if mean image value is
+                         below this value, default is None (ignore)
+        resetSharpness : float, mosaic will reset if image sharpness (mean
+                         of gradient) drops below this value, default is None (ignore)                
+        
+    """
     
     # Constants for method of dealing with reaching the edge of the mosaic image
     CROP = 0
     EXPAND = 1
     SCROLL = 2
     
     # Constants for direction of images reaching the edge of the mosaic image
     LEFT = 0
     TOP = 1
     RIGHT = 2
     BOTTOM = 3  
     
     lastImageAdded = None
           
-    def __init__(self, mosaicSize, **kwargs):
-        """ Initisialise Mosaic object, used for high speed mosaicing
-        of fibre bundle images.
-        """
+    def __init__(self, mosaicSize, **kwargs):        
+        
         
         self.mosaicSize = mosaicSize
         self.prevImg = []
 
         # If None is used for the following
         # sensible values will be selected after the first image
-        # is received
+        # is received and __initialise_mosaic() is called
         self.resize = kwargs.get('resize', None)
         self.templateSize = kwargs.get('templateSize', None)
         self.refSize = kwargs.get('refSize', None)
         self.cropSize = kwargs.get('cropSize', None)
         self.imageType = kwargs.get('imageType', None)
         
         # Blending control
@@ -78,212 +115,223 @@
         self.lastShift = [0,0]
         self.lastXAdded = 0
         self.lastYAdded = 0
         self.nImages = 0        
         self.imSize = None  # None tells us to read this from the first image        
         
         self.col = False   # Assume monochrome
-        return
-        
-       
-    def initialise(self, img):
-        """ Choose sensible values for non-specified parameters.
-        :param img: input image to used to choose sensible parameters, 2D/3D numpy array
-        :return None:
-        """
-        
-        if img.ndim == 3:
-            self.col = True
-            self.nChannels = np.shape(img)[2]
-        else:
-            self.col = False
         
-        if self.imSize is None:
-            if self.resize is None:
-                self.imSize = min(img.shape[0:2])
-            else:
-                self.imSize = self.resize
-
-        if self.cropSize is None:
-            self.cropSize = round(self.imSize * .9)            
-        
-        if self.templateSize is None:
-            self.templateSize = round(self.imSize / 4)
-            
-        if self.refSize is None:
-            self.refSize = round(self.imSize / 2)
-            
-        if self.imageType is None:
-            self.imageType = img.dtype
+        return
         
-        if np.size(self.mask) == 0:
-            self.mask = pybundle.get_mask(np.zeros([self.imSize,self.imSize]),(self.imSize/2,self.imSize/2,self.cropSize / 2))
        
-        if self.col:
-            self.mosaic = np.zeros((self.mosaicSize, self.mosaicSize, self.nChannels), dtype = self.imageType)
-        else:
-            self.mosaic = np.zeros((self.mosaicSize, self.mosaicSize), dtype = self.imageType)
-
-        self.currentX = self.initialX
-        self.currentY = self.initialY
-        
-        self.nImages = 0
-        
-        return 
-    
     
     # Add image to current mosaic
     def add(self, img):
         """ Add image to current mosaic.
-        :param img: image as 2D numpy array
-        :return: None
+        
+        Arguments:
+            img    : image as 2D/3D numpy array
         """
 
         # Before we have first image we can't choose sensible default values, so
         # initialisation is called here if we are on the first image
         if self.nImages == 0:
-            self.initialise(img) 
-
+            self.__initialise_mosaic(img) 
+          
                   
         if self.resize is not None: 
             imgResized = cv.resize(img, (self.resize, self.resize))
         else:
             imgResized = img
             
         if self.nImages > 0:
             
-            self.lastShift, self.shiftConf = Mosaic.find_shift(self.prevImg, imgResized, self.templateSize, self.refSize)
+            self.lastShift, self.shiftConf = Mosaic.__find_shift(self.prevImg, imgResized, self.templateSize, self.refSize)
            
+            # reset mosaic if correlation between two images below threshold
             if self.resetThresh is not None:
                 if self.shiftConf < self.resetThresh:
-                    self.initialise(img)
-                    Mosaic.insert_into_mosaic(self.mosaic, imgResized, self.mask, (self.currentX, self.currentY))
+                   
+                    self.__initialise_mosaic(img)
+                    Mosaic.__insert_into_mosaic(self.mosaic, imgResized, self.mask, (self.currentX, self.currentY))
 
                     return
-            
+                
+            # reset mosaic if image intensity below threshold
             if self.resetIntensity is not None:
                 if np.mean(imgResized) < self.resetIntensity:
-                    self.initialise(img)
-                    Mosaic.insert_into_mosaic(self.mosaic, imgResized, self.mask, (self.currentX, self.currentY))
+                    self.__initialise_mosaic(img)
+                    Mosaic.__insert_into_mosaic(self.mosaic, imgResized, self.mask, (self.currentX, self.currentY))
 
                     return
                 
+            # reset mosaic if image sharpness below threshold  
             if self.resetSharpness is not None:
                 refIm = pybundle.extract_central(imgResized, self.refSize)
                 
-                if refIm.ndim == 3:
+                if refIm.ndim == 3:  # colour
                     gx, gy = np.gradient(refIm, axis = (0,1))
                     gx = np.mean(gx,2)
                     gy = np.mean(gy,2)
                     
-                else:
+                else:                # monochrome
                     gx, gy = np.gradient(refIm)
                    
                 gnorm = np.sqrt(gx**2 + gy**2)
                 gav = np.mean(gnorm)
                 if gav < self.resetSharpness:   
-                    self.initialise(img)
-                    Mosaic.insert_into_mosaic(self.mosaic, imgResized, self.mask, (self.currentX, self.currentY))
+                    self.__initialise_mosaic(img)
+                    Mosaic.__insert_into_mosaic(self.mosaic, imgResized, self.mask, (self.currentX, self.currentY))
                     return
 
             self.currentX = self.currentX + self.lastShift[1]
             self.currentY = self.currentY + self.lastShift[0]
             
             distMoved = math.sqrt( (self.currentX - self.lastXAdded)**2 + (self.currentY - self.lastYAdded)**2)
             
             if distMoved >= self.minDistForAdd:
                 self.lastXAdded = self.currentX
                 self.lastYAdded = self.currentY
                 
                 for i in range(2):
-                    outside, direction, outsideBy = Mosaic.is_outside_mosaic(self.mosaic, imgResized, (self.currentX, self.currentY))
+                    outside, direction, outsideBy = Mosaic.__is_outside_mosaic(self.mosaic, imgResized, (self.currentX, self.currentY))
     
                     if outside == True:
                         if self.boundaryMethod == self.EXPAND: 
-                            self.mosaic, self.mosaicWidth, self.mosaicHeight, self.currentX, self.currentY = Mosaic.expand_mosaic(self.mosaic, max(outsideBy, self.expandStep), direction, self.currentX, self.currentY)
+                            self.mosaic, self.mosaicWidth, self.mosaicHeight, self.currentX, self.currentY = Mosaic.__expand_mosaic(self.mosaic, max(outsideBy, self.expandStep), direction, self.currentX, self.currentY)
                             outside = False
                         elif self.boundaryMethod == self.SCROLL:
-                            self.mosaic, self.currentX, self.currentY = Mosaic.scroll_mosaic(self.mosaic, outsideBy, direction, self.currentX, self.currentY)
+                            self.mosaic, self.currentX, self.currentY = Mosaic.__scroll_mosaic(self.mosaic, outsideBy, direction, self.currentX, self.currentY)
                             outside = False
                     
                 if outside == False:
                     if self.blend:
-                        Mosaic.insert_into_mosaic_blended(self.mosaic, imgResized, self.mask, self.blendMask, self.cropSize, self.blendDist, (self.currentX, self.currentY))
+                        Mosaic.__insert_into_mosaic_blended(self.mosaic, imgResized, self.mask, self.blendMask, self.cropSize, self.blendDist, (self.currentX, self.currentY))
                     else:
-                        Mosaic.insert_into_mosaic(self.mosaic, imgResized, self.mask, (self.currentX, self.currentY))
+                        Mosaic.__insert_into_mosaic(self.mosaic, imgResized, self.mask, (self.currentX, self.currentY))
                             
         else:  
             # 1st image goes straight into mosaic
-            Mosaic.insert_into_mosaic(self.mosaic, imgResized, self.mask, (self.currentX, self.currentY))
+            Mosaic.__insert_into_mosaic(self.mosaic, imgResized, self.mask, (self.currentX, self.currentY))
             self.lastXAdded = self.currentX
             self.lastYAdded = self.currentY
 
         self.prevImg = imgResized
         self.nImages = self.nImages + 1
 
 
 
     def get_mosaic(self):
-        """ Obtain current mosaic image.
-        :return: mosaic image as 2D numpy array
+        """ Returns current mosaic image as 2D/3D numpy array
         """
         return self.mosaic
+    
         
-
-
     def reset(self):
-        """ Called when mosaic is restarted.
-        :return: None
+        """ Call to reset mosaic, clearing image. The mosaic will only
+        be fully reset once a new image is added. Note that parameters that
+        were already initialised will not be reset. 
         """
         self.nImages = 0
+
+    
+    def __initialise_mosaic(self, img):
+        """ Choose sensible values for non-specified parameters.
+        
+        Arguments:
+            img  : input image to used to choose sensible parameters for 
+                    mosaicing, 2D/3D numpy array
+        """
+        
+        if img.ndim == 3:
+            self.col = True
+            self.nChannels = np.shape(img)[2]
+        else:
+            self.col = False
+        
+        if self.imSize is None:
+            if self.resize is None:
+                self.imSize = min(img.shape[0:2])
+            else:
+                self.imSize = self.resize
+    
+        if self.cropSize is None:
+            self.cropSize = round(self.imSize * .9)            
+        
+        if self.templateSize is None:
+            self.templateSize = round(self.imSize / 4)
             
+        if self.refSize is None:
+            self.refSize = round(self.imSize / 2)
+            
+        if self.imageType is None:
+            self.imageType = img.dtype
+        
+        if np.size(self.mask) == 0:
+            self.mask = pybundle.get_mask(np.zeros([self.imSize,self.imSize]),(self.imSize/2,self.imSize/2,self.cropSize / 2))
+       
+        if self.col:
+            self.mosaic = np.zeros((self.mosaicSize, self.mosaicSize, self.nChannels), dtype = self.imageType)
+        else:
+            self.mosaic = np.zeros((self.mosaicSize, self.mosaicSize), dtype = self.imageType)
+    
+        self.currentX = self.initialX
+        self.currentY = self.initialY
+        
+        self.nImages = 0
         
-    def insert_into_mosaic(mosaic, img, mask, position):
+        return 
+    
+    
+
+    @staticmethod    
+    def __insert_into_mosaic(mosaic, img, mask, position):
         """ Dead leaf insertion of image into a mosaic at specified position. 
         Only pixels for which mask == 1 are copied.
-        :param mosaic: current mosaic image, 2D numpy array
-        :param img: img to insert, 2D numpy array
-        :param mask: 2D numpy array with values of 1 for pixels to be copied
-            and 0 for pixels not to be copied. Must be same size as img.
-        :param position: position of insertion as tuple of (x,y). This is the
-            pixel the centre of the image will be at.
+        
+        Arguments:
+            mosaic   : current mosaic image, 2D/3D numpy array
+            img      : img to insert, 2D/3D numpy array
+            mask     : 2D numpy array with values of 1 for pixels to be copied
+                       and 0 for pixels not to be copied. Must be same size as img.
+            position : position of insertion as tuple of (x,y). This is the
+                       pixel the centre of the image will be at.
         
         """
         px = math.floor(position[0] - np.shape(img)[0] / 2)
         py = math.floor(position[1] - np.shape(img)[1] / 2)        
         
         oldRegion = mosaic[px:px + np.shape(img)[0] , py :py + np.shape(img)[1]]
-
         
         oldRegion[np.array(mask)] = img[np.array(mask)]
         mosaic[px:px + np.shape(img)[0] , py :py + np.shape(img)[1]] = oldRegion
         
         return
     
-                
-    def insert_into_mosaic_blended(mosaic, img, mask, blendMask, cropSize, blendDist, position):
+    @staticmethod            
+    def __insert_into_mosaic_blended(mosaic, img, mask, blendMask, cropSize, blendDist, position):
         """ Insertion of image into a mosaic with cosine window blending. Only pixels from
         image for which mask == 1 are copied. Pixels within blendDist of edge of mosaic
-        (i.e. radius of cropSize/2) are blended with existing mosaic pixel values    
-        :param mosaic: current mosaic image, 2D numpy array
-        param img: img to insert, 2D numpy array
-        :param mask: 2D numpy array with values of 1 for pixels to be copied
-            and 0 for pixels not to be copied. Must be same size as img.
-        :param blendMask: the cosine window blending mask with weighted pixel values. If passed empty []
-            this will be created
-        :param cropSize: size of input image.
-        :param blendDist: number which control the sptial extent of the blending
-        :param position: position of insertion as tuple of (x,y). This is the
-            pixel the centre of the image will be at.
-        :return: None
+        (i.e. radius of cropSize/2) are blended with existing mosaic pixel values  
+        
+        Arguments:
+           mosaic    : current mosaic image, 2D/3D numpy array
+           img       : img to insert, 2D/3D numpy array
+           mask      : 2D numpy array with values of 1 for pixels to be copied
+                       and 0 for pixels not to be copied. Must be same size as img.           
+           blendMask : the cosine window blending mask with weighted pixel values. If passed empty []
+                       this will be created
+           cropSize  : size of input image.
+           blendDist : number which controls the sptial extent of the blending
+           position  : position of insertion as tuple of (x,y). This is the
+                       pixel the centre of the image will be at.
         
         """
         px = math.floor(position[0] - np.shape(img)[0] / 2)
-        py = math.floor(position[1] - np.shape(img)[1] / 2)
-        
+        py = math.floor(position[1] - np.shape(img)[1] / 2)        
                
         # Region of mosaic we are going to work on
         oldRegion = mosaic[px:px + np.shape(img)[0] , py :py + np.shape(img)[1]]
 
         # Only do blending on non-zero valued pixels of mosaic, otherwise we 
         # blend into nothing
         blendingMask = np.where(oldRegion>0,1,0)
@@ -292,15 +340,15 @@
         # the colour channels
         if blendingMask.ndim > 2:
             blendingMask = np.max(blendingMask,2)
 
         # If first time, create blend mask giving weights to apply for each pixel
         if blendMask == []:
             maskRad = cropSize / 2
-            blendImageMask = Mosaic.cosine_window(np.shape(oldRegion)[0], maskRad, blendDist) 
+            blendImageMask = Mosaic.__cosine_window(np.shape(oldRegion)[0], maskRad, blendDist) 
 
 
         imgMask = blendImageMask.copy()
         imgMask[blendingMask == 0] = 1   # For pixels where mosaic == 0 use original pixel values from image 
         imgMask = imgMask * mask
         mosaicMask = 1- imgMask    
         
@@ -312,94 +360,91 @@
         oldRegion = oldRegion * mosaicMask + img * imgMask       
 
         # Insert it back in
         mosaic[px:px + np.shape(img)[0] , py :py + np.shape(img)[1]] = oldRegion
        
         return
    
-    
-    def find_shift(img1, img2, templateSize, refSize):
+    @staticmethod
+    def __find_shift(img1, img2, templateSize, refSize):
         """ Calculates how far img2 has shifted relative to img1 using
-        normalised cross correlation
-        :param img1: reference image as 2D/3D numpy array
-        :param img2: template image as 2D/3D numpy array
-        :param templateSize: a square of this size is extracted from img as the template
-        :param refSize: a sqaure of this size is extracted from refSize as the template. 
-           Must be bigger than templateSize and the maximum shift detectable is 
-           (refSize - templateSize)/2
-        :return: tuples of (shift, max_val) where shift is a tuple of (x_shift, y_shift) and 
-           max_val is the normalised cross correlation peak value. Returns None if the shift
-           cannot be calculated.
+        normalised cross correlation.
+        
+        Returns tuple of (shift, max_val) where shift is a tuple of (x_shift, y_shift) and 
+        max_val is the normalised cross correlation peak value. Returns None if the shift
+        cannot be calculated.
+           
+        Arguments:  
+            img1         : reference image as 2D/3D numpy array
+            img2         : template image as 2D/3D numpy array
+            templateSize : int, a square of this size is extracted from img as 
+                           the template
+            refSize      : int, a square of this size is extracted from refSize 
+                           as the template. 
+                           Must be bigger than templateSize and the maximum 
+                           shift detectable is (refSize - templateSize)/2
+        
         """
+        
         if refSize < templateSize or min(np.shape(img1)[0:2]) < refSize or min(np.shape(img2)[0:2]) < refSize:
              return None
         else:
              template = pybundle.extract_central(img2, templateSize)  
              refIm = pybundle.extract_central(img1, refSize)
 
              res = cv.matchTemplate(pybundle.to8bit(template), pybundle.to8bit(refIm), cv.TM_CCORR_NORMED)
              min_val, max_val, min_loc, max_loc = cv.minMaxLoc(res)
              shift = [max_loc[0] - (refSize - templateSize), max_loc[1] - (refSize - templateSize)]
-             #shift = 0
              return shift, max_val
             
     
-    def extract_central(img, boxSize):
-        """ Extracts square of size boxSize from centre of img.
-        :param img: input image as 2D numpy array
-        :param boxSize: size of sqaure
-        :return: cropped image as 2D numpy array
-        """
-
-        w = np.shape(img)[0]
-        h = np.shape(img)[1]
-
-        cx = w/2
-        cy = h/2
-        boxSemiSize = min(cx,cy,boxSize)
-        
-        img = img[math.floor(cx - boxSemiSize):math.floor(cx + boxSemiSize), math.ceil(cy- boxSemiSize): math.ceil(cy + boxSemiSize)]
-        return img    
-    
-    
-    def cosine_window(imgSize, circleSize, circleSmooth):
+    @staticmethod   
+    def __cosine_window(imgSize, circleSize, circleSmooth):
         """ Produce a circular cosine window mask on grid of imgSize * imgSize. Mask
-        is 0 for radius > circleSize and 1 for radius < (circleSize - cicleSmooth)
+        is 0 for radius > circleSize and 1 for radius < (circleSize - circleSmooth).
         The intermediate region is a smooth cosine function.
-        :param imgSize: size of square mask to generate
-        :param circleSize: radius of mask (mask pixels outside here are 0)
-        :param circleSmooth: size of smoothing region at the inside edge of the circle. 
-            (mask pixels with a radius less than this are 1)
-        :return: mask as 2D numpy array.           
+        
+        Returns mask as 2D numpy array.           
+        
+        Arguments: 
+            imgSize      : int, size of square mask to generate
+            circleSize   : int, radius of mask (mask pixels outside here are 0)
+            circleSmooth : int, size of smoothing region at the inside edge of the circle. 
+                                (mask pixels with a radius less than this are 1)
         """
         
         innerRad = circleSize - circleSmooth
         xM, yM = np.meshgrid(range(imgSize),range(imgSize))
         imgRad = np.sqrt( (xM - imgSize/2) **2 + (yM - imgSize/2) **2)
         mask =  np.cos(math.pi / (2 * circleSmooth) * (imgRad - innerRad))**2
         mask[imgRad < innerRad ] = 1
         mask[imgRad > innerRad + circleSmooth] = 0
+        
         return mask    
     
-    
-    def is_outside_mosaic(mosaic, img, position):
+    @staticmethod
+    def __is_outside_mosaic(mosaic, img, position):
         """ Checks if position of image to insert into mosaic will result in 
-        # part of inserted image being outside of mosaic. Returns tuple of 
-        # boolean (true if outside), side it leaves (using consts defined above)
-        # and distance is has strayed over the edge. e.g. (True, Mosaic.Top, 20).
-        :param mosaic: mosaic image (strictly can be any numpy array the same size as the mosaic)
-        :param img: image to be inserted as 2D numpy array
-        :param position: position of insertion as tuple of (x,y). This is the
-            pixel the centre of the image will be at.        
-        :return: tuple of (ouside, side, distance)
-            where: - outside is True if part of image is outside mosaic
-                   - side is (one of the) side(s) it has strayed out of, one of Mosaic.Top, 
-                   Mosaic.Bottom, Mosaic.Left or Mosaic.Right or -1 if outside == False
-                   - distance is distance it has strayed outside mosaic in the direction specified
-                   in size. (0 if outside == False)
+        part of inserted image being outside of mosaic. Returns tuple of 
+        boolean (true if outside), side it leaves (using consts defined above)
+        and distance is has strayed over the edge. e.g. (True, Mosaic.Top, 20).
+        
+        Returns tuple of (ouside, side, distance), where outside is True if 
+        part of image, side is (one of the) side(s) it has strayed out of, 
+        one of Mosaic.Top, Mosaic.Bottom, Mosaic.Left or Mosaic.Right or -1 if 
+        outside == False, distance is distance it has strayed outside mosaic in 
+        the direction specified in size (0 if outside == False).
+        
+        Arguments:
+            
+            mosaic   : mosaic image (strictly can be any numpy array the same size as the mosaic)
+            img      : image to be inserted as 2D numpy array
+            position : position of insertion as tuple of (x,y). This is the
+                       pixel the centre of the image will be at.        
+        
             """
         
         imgW = np.shape(img)[0] 
         imgH = np.shape(img)[1] 
         
         mosaicW = np.shape(mosaic)[0]
         mosaicH = np.shape(mosaic)[1]        
@@ -417,31 +462,34 @@
         elif right > mosaicW:
             return True, Mosaic.RIGHT, right - mosaicW        
         elif bottom > mosaicH:
             return True, Mosaic.BOTTOM, bottom - mosaicH
         else:
             return False, -1, 0        
      
-  
-    def expand_mosaic(mosaic, distance, direction, currentX, currentY):
+    @staticmethod
+    def __expand_mosaic(mosaic, distance, direction, currentX, currentY):
         """ Increase size of mosaic image by 'distance' in direction 'direction'. Supply
         currentX and currentY position so that these can be modified to be correct
         for new mosaic size. 
-        :param mosaic: input mosaic image as 2D numpy array
-        :param distance: pixels to expand by
-        :param direction: side to expand, one of Mosaic.Top, Mosaic.Bottom, 
-            Mosaic.Left or Mosaic.Right
-        :param currentX: x position of last image insertion into mosaic
-        :param currentY: y position of last image insertion into mosaic
-        :return: tuple of (newMosaic, width, height, newX, newY)
-            where -newMosaic is the larger mosaic image as 2D numpy array
-                  -width is the x-size of the new mosaic
-                  -height is the y-size of the new mosaic
-                  -newX is the x position of the last image insertion in the new mosaic
-                  -newT is the y position of the last image insertion in the new mosaic
+        
+        Returns tuple of (newMosaic, width, height, newX, newY), where newMosaic 
+        is the larger mosaic image as 2D numpy array, width is the x-size of 
+        the new mosaic, height is the y-size of the new mosaic, newX is the x 
+        position of the last image insertion in the new mosaic, newY is the y 
+        position of the last image insertion in the new mosaic.
+        
+        Arguments:            
+            mosaic    : input mosaic image as 2D numpy array
+            distance  : pixels to expand by
+            direction : side to expand, one of Mosaic.Top, Mosaic.Bottom, 
+                         Mosaic.Left or Mosaic.Right
+            currentX  : x position of last image insertion into mosaic
+            currentY  : y position of last image insertion into mosaic
+        
         """          
         mosaicWidth = np.shape(mosaic)[0]
         mosaicHeight = np.shape(mosaic)[1]
         if mosaic.ndim > 2:
             mosaicChannels = np.shape(mosaic)[2]
         else:
             mosaicChannels = 1
@@ -466,31 +514,34 @@
         
         if direction == Mosaic.BOTTOM:
             newMosaicHeight = mosaicHeight + distance
             newMosaic = np.squeeze(np.zeros((mosaicWidth, newMosaicHeight, mosaicChannels), mosaic.dtype))
             newMosaic[:, 0:mosaicHeight ] = mosaic
             return newMosaic, mosaicWidth, newMosaicHeight,  currentX , currentY 
         
-    
-    def scroll_mosaic(mosaic, distance, direction, currentX, currentY):
+    @staticmethod
+    def __scroll_mosaic(mosaic, distance, direction, currentX, currentY):
         """ Scroll mosaic to allow mosaicing to continue past edge of mosaic. Pixel 
         values will be lost. Supply currentX and currentY position so that these
-        can be modified to be correct for new mosaic size
-        :param mosaic: input mosaic image as 2D numpy array
-        :param distance: pixels to expand by
-        :param direction: side to expand, one of Mosaic.Top, Mosaic.Bottom, 
-            Mosaic.Left or Mosaic.Right
-        :param currentX: x position of last image insertion into mosaic
-        :param currentY: y position of last image insertion into mosaic
-        :return: tuple of (newMosaic, width, height, newX, newY)
-            where -newMosaic is the larger mosaic image as 2D numpy array
-                  -width is the x-size of the new mosaic
-                  -height is the y-size of the new mosaic
-                  -newX is the x position of the last image insertion in the new mosaic
-                  -newT is the y position of the last image insertion in the new mosaic
+        can be modified to be correct for new mosaic size.
+        
+        Return: tuple of (newMosaic, width, height, newX, newY), where 
+        newMosaic is the larger mosaic image as 2D numpy array, width is the 
+        x-size of the new mosaic, height is the y-size of the new mosaic, newX 
+        is the x position of the last image insertion in the new mosaic, newY 
+        is the y position of the last image insertion in the new mosaic.
+        
+        Arguments:
+            mosaic    : input mosaic image as 2D numpy array
+            distance  : pixels to expand by
+            direction : side to expand, one of Mosaic.Top, Mosaic.Bottom, 
+                        Mosaic.Left or Mosaic.Right
+            currentX  : x position of last image insertion into mosaic
+            currentY  : y position of last image insertion into mosaic        
+        
         """
         mosaicWidth = np.shape(mosaic)[0]
         mosaicHeight = np.shape(mosaic)[1]
 
         if direction == Mosaic.LEFT:       
             newMosaic = np.roll(mosaic,distance,0)
             newMosaic[0:distance:,:] = 0
```

### Comparing `PyFibreBundle-1.3/src/pybundle/pybundle.py` & `PyFibreBundle-1.3.1/src/pybundle/pybundle.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 
 
 import numpy as np
 import math
 import time
 
 import cv2 as cv
+import pybundle
 
 from pybundle.core_interpolation import *    
 from pybundle.bundle_calibration import BundleCalibration
+from pybundle.core import normalise_image
 
 
 class PyBundle:
        
     coreMethod = None
 
     background = None
@@ -37,15 +39,15 @@
     applyMask = False
     
     crop = False
     
     filterSize = None
     
     autoContrast = False
-    outputType = 'float'
+    outputType = 'float64'
     
     edgeFilter = None
     edgeFilterShape = None
     
     calibImage = None
     coreSize = 3
     gridSize  = 512
@@ -119,67 +121,106 @@
         self.srMultiNormalisation = kwargs.get('srMultiNormalisation' ,self.srMultiNormalisation )
         self.srDarkFrame = kwargs.get('srDarkFrame', self.srDarkFrame)
         self.srUseLut = kwargs.get('srUseLut', self.srUseLut)
         
                
 
     def set_filter_size(self, filterSize):
-        """ Set the size of Gaussian filter used if filtering method employed"""
+        """ Set the size of Gaussian filter used if filtering method employed.
+        
+        Arguments:
+            filterSize : float, sigma of Gaussian filter
+        """
         self.filterSize = filterSize
         
     
     def set_loc(self, loc):
-        """ Store the location of the bundle, requires tuple of (centreX, centreY, radius)."""
+        """ Store the location of the bundle. This will also set autoLoc = False.
+        
+        Arguments:
+            loc : bundle location, tuple of (centreX, centreY, radius)
+        """
+        
         self.loc = loc
         self.autoLoc = False   # We don't want to automatically find it if we have been given it
         
     
     def set_core_method(self, coreMethod):
-        """ Set the method to use to remove cores, FILTER, TRILIN or EDGE_FILTER"""
+        """ Set the method to use to remove cores, FILTER, TRILIN or EDGE_FILTER
+        
+        Arguments:
+            coreMethod: PyBundle.FILTER, PyBundle.TRILIN or PyBundle.EDGE_FILTER
+        """
         self.coreMethod = coreMethod
         
         
     def set_core_size(self, coreSize):
-        """ Set the estimated centre-centre core spacing used to help find cores as part of TRILIN method"""
+        """ Set the estimated centre-centre core spacing used to help find 
+        cores as part of TRILIN method.
+        
+        Arguments:
+            coreSize : float, estimate core spacing
+        """
         self.coreSize = coreSize
         
     
     def set_mask(self, mask):
-        """ Provide a mask to be used. Mask must be a 2D numpy array of same size as images to be processed"""
+        """ Provide a mask to be used. Mask must be a 2D numpy array of same 
+        size as images to be processed
+        
+        Arguments:
+            mask : 2D numpy array, 1 inside bundle, 0 inside bundle. Must be
+                   same size as image to be processed.
+        """
         self.mask = mask
         self.autoMask = False  # We don't want to automatically find it if we have been given it
         
     
     def set_auto_contrast(self, ac):
-        """ Determines whether images are scaled to be between 0-255. Boolean"""
+        """ Determines whether images are scaled to be between 0-255. 
+        
+        Arguments:
+            ac : boolean, True to autocontrast 
+        """
+
         self.autoContrast = ac
         
         
     def set_crop(self, crop):
         """ Determines whether images are cropped to size of bundle 
         for FILTER, EDGE_FILTER methods. crop is Boolean.
+        
+        Arguments:
+            crop : boolean, True to crop
         """
+        
         self.crop = crop    
     
     
     def set_apply_mask(self, applyMask):
         """ Determines whether areas outside the bundle are set to zero 
-        for FILTER and EDGE_FILTER method. applyMask is Boolean.
+        for FILTER and EDGE_FILTER method. 
+        
+        Arguments:
+            applyMask: boolean, True to apply mask, False to not apply mask
         """
         self.apply_mask = applyMask
         
     
     def set_auto_mask(self, img, **kwargs):
         """ Set whether to automically create mask using pre-determined bundle 
         location.
         
         It is also possible to provide an image as a 2D numpy array, in which
         case the mask will be generated of the correct size for this image, but
-        this is deprecates, use calibrate() instead. Optionally provide a 
+        this is deprecated, use calibrate() instead. Optionally provide a 
         radius rather than using radius of determined bundle location.
+        
+        Arguments:
+            img: boolean, True to automically create mask
        
         """       
         if type(img) is bool:
             if img is True:
                 self.mask = None
                 self.autoMask = True     
             
@@ -195,31 +236,38 @@
     
         
         
     def create_and_set_mask(self, img, **kwargs):
         """ Determine mask from provided calibration image and set as mask
         Optionally provide a radius rather than using radius of determined
         bundle location.
-        :param img: calibration image from which size of mask is determined
-        :param radius, optional radius of mask
+        
+        Arguments:
+            img: calibration image from which size of mask is determined
+            
+        Keyword Arguments:            
+            radius : radius of mask, default is to determine this automtically
         """    
         if img is not None:
             self.set_auto_loc(img)
             
             if self.loc is not None:
                 self.set_auto_mask(img, **kwargs)    
         
         
     def set_auto_loc(self, img):
         """ Sets whether the bundle is automatically located for cropping and masking,
-        if these are turned on.
+        if these are turned on, depending on boolean value passed.
         
         It is also possible to pass an image as a 2D numpy array instead of a Boolean,
         in which case the bundle location will be determined from this image. However,
-        this is not deprecated in favour of setting calibImg and then calling calibrate.
+        this is noq deprecated in favour of setting calibImg and then calling calibrate.
+        
+        Arguments:
+            img : boolean, True to auto-locate bundle, False to not.
         """      
         
         if type(img) is bool:
             if img is True:
                 self.loc = None
                 self.autoLoc = True
         elif type(img) is np.ndarray:        
@@ -227,154 +275,235 @@
             self.autoLoc  = False
                     
         
     def set_background(self, background):
         """ Store an image to be used as background. If TRILIN is being used and a 
         calibration has already been performed, the background will be added to the
         calibration.
-        :param background: background image as 2D numpy array. Set as None to removed background.
+
+        Arguments:
+
+            backgroundImage : background image as 2D/3D numpy array. Set as 
+                              None to remove background.        
         """
+        
         if background is not None:
             self.background = background.astype('float')
         else:
             self.background = None
         if self.calibration is not None:
             self.calibration = pybundle.tri_interp_background(self.calibration, self.background)
             
         
     def set_normalise_image(self, normaliseImage):
         """ Store an image to be used for normalisation. If TRILIN is being used and a 
         calibration has already been performed, the normalisation will be added to the
         calibration.
-        :param normaliseImage: normalisation image as 2D numpy array. Set as None to removed normalisation.
+        
+        Arguments:
+
+            normaliseImage : normalisation image as 2D/3D numpy array. Set as 
+                             None to remove normalisation.
         """
         if normaliseImage is not None:
             self.normaliseImage = normaliseImage.astype('float')
         else:
             self.normaliseImage = None
         if self.calibration is not None:
             self.calibration = pybundle.tri_interp_normalise(self.calibration, self.normaliseImage)
             
         
     def set_output_type(self, outputType):
-        """ Specify the data type of input images from 'process'. If not called, 
-        default of 'uint8' will be used.
-        :param outputType: one of 'uint8', 'unit16' or 'float'
-        :return: True if type was valid, otherwise False
+        """ Specify the data type of input images returned from 'process'. 
+        Returns False if type not valid.
+        
+        Arguments:
+
+            outputType : str, one of 'uint8', 'unit16' or 'float'
         """
-        if outputType == 'uint8' or outputType == 'uint16' or outputType == 'float':
+        if outputType == 'uint8' or outputType == 'uint16' or outputType == 'float' or outputType == 'float32' or outputType == 'float64':
             self.outputType = outputType
             return True
         else:
             return False
         
             
     def set_calib_image(self, calibImg):
-        """ Set image to be used for calibration if TRLIN method used.
-        :param calibImg: calibration image as 2D numpy array
+        """ Set image to be used for calibration.
+        
+        Arguments:
+            calibImg : calibration image as 2D/3D numpy array
         """
         self.calibImage = calibImg.astype('float')
         
         
         
     def set_grid_size(self, gridSize):
-        """ Set output image size if TRLIN method used. If not called prior to calling 'calibrate', the default value of 512 will be used.
-        :param gridSize: size of square image output size
+        """ Sets output image size if TRLIN method used. If not called prior 
+        to calling 'calibrate', the default value of 512 will be used.
+        
+        Arguments:
+            gridSize : int, size of square image output 
         """
         self.gridSize = gridSize
         
         
     def set_edge_filter_shape(self, edgePos, edgeSlope):  
-        """ Create filter if EDGE_FILTER method is to be used.
-        :param edgePos: spatial frequency of edge in pixels of FFT of image
-        :param edgeSlope: steepness of slope (range from 10% to 90%) in pixels of FFT of image
+        """ Creates and stores filter for EDGE_FILTER method.
+        
+        Arguments:
+            edgePos   : float, spatial frequency of edge in pixels of FFT of image
+            edgeSlope : float, steepness of slope (range from 10% to 90%) in pixels of FFT of image
         """
+        
         self.edgeFilterShape  = (edgePos, edgeSlope)
         
         
     def set_use_numba(self, useNumba):
-        """ Sets whether Numba should be used for JIT compiler acceleration for functionality which support this. Boolean"""
+        """ Sets whether Numba should be used for JIT compiler acceleration for 
+        functionality which supports this.
+
+        Arguments:
+            useNumba : boolean, True to use Numba, False to not.
+        """
+        
         self.useNumba = useNumba  
 
     def set_sr_calib_images(self, calibImages):
-        """ Provides the calibration images, a stack of shifted images used to determine shifts between images for super-resolution
+        """ Provides the calibration images, a stack of shifted images used to 
+        determine shifts between images for super-resolution
+        
+        Arguments:
+            calibImages : 3D numpy array, stack of shifted images.
+            
         """
         self.srCalibImages = calibImages
         
         
     def set_sr_norm_to_images(self, normToImages):
-        """ Sets whether super-resolution recon should normalise each input image to have the same mean intensity. Boolean"""
+        """ Sets whether super-resolution recon should normalise each input 
+        image to have the same mean intensity. 
+        
+        Arguments:
+            normToImages : boolean, True to normalise, False to not
+        
+        """
 
         self.srNormToImages = normToImages         
         
         
     def set_sr_norm_to_backgrounds(self, normToBackgrounds):
-        """ Sets whether super-resolution recon should normalise each input image w.r.t. a stack of backgrounds in srBackgrounds to have the same mean intensity. Boolean"""
+        """ Sets whether super-resolution recon should normalise each input 
+        image w.r.t. a stack of backgrounds in srBackgrounds to have the same 
+        mean intensity. 
+        
+        Arguments:
+            normToBackgrounds : boolean, True to normalise, False to not
+        
+        """
         self.srNormToBackgrounds = normToBackgrounds  
         
     
     def set_sr_multi_backgrounds(self, mb):
-        """ Sets whether super-resolution should normalise each core in each image"""
+        """ Sets whether super-resolution should use individual backgrounds for each
+        each shifted image.
+        
+        Arguments:
+            mb : boolean, True to use multiple backgrounds, False to not
+            
+        """
         self.srMultiBackgrounds = mb
         
         
     def set_sr_multi_normalisation(self, mn):
+        """ Sets whether super-resolution should normalise to each core in each image
+        
+        Arguments:
+            mn : boolean, True to normalise each core in each image, False to not
+            
+        """
         self.srMultiNormalisation = mn
 
         
     def set_sr_backgrounds(self, backgrounds):
-        """ Provide a set of background images for background correction of each SR shifted image.
+        """ Provide a set of background images for background correction of 
+        each SR shifted image.
+        
+        Arguments:
+            backgrounds : 3D numpy array, stack of background images
+            
         """
         self.srBackgrounds = backgrounds  
        
         
     def set_sr_normalisation_images(self, normalisationImages):
-        """ Provide a set of normalisation images for normalising intensity of each SR shifted image.
+        """ Provide a set of normalisation images for normalising intensity of 
+        each SR shifted image.
+        
+        Arguments:
+            normalisationImages : 3D numpy array, stack of images
+            
         """
         self.srNormalisationImgs = normalisationImages
         
 
     def set_sr_shifts(self, shifts):
-        """ Provide shifts between SR images"""
+        """ Provide shifts between SR images. If this is set then no registration
+        will be performed. 
+        
+        Arguments:
+            shifts : 2D numpy array, shifts for each image relative to first
+                     image. 1st axis is image number, 2nd axis is (x,y)
+        """
         self.srShifts = shifts
      
      
     def set_sr_dark_frame(self, darkFrame):
-        """ Provide a dark frame for super-resolution calibration"""
+        """ Provide a dark frame for super-resolution calibration.
+        
+        Arguments:
+            darkFrame : 2D numpy array, dark frame
+        
+        """
         self.srDarkFrame = darkFrame
         
         
     def set_sr_param_value(self, val):
-        """ Sets the current value of the parameter on which the shifts dependent for SR reconstruction """
+        """ Sets the current value of the parameter on which the shifts
+        dependent for SR reconstruction.
+        
+        Arguments:
+            val : parameter value
+        
+        """
         self.srParamValue = val
                 
         
     def calibrate(self):
         """ Peforms calibraion steps appropriate to chosen method. A calibration 
         image must have been set prior to calling this.
         
-        For TRILIN, creates inerpolation calibration.
+        For TRILIN, creates interpolation calibration.
         
-        FOR FILTER, EDGE_FILTER the bundle will be located if autoLoc has been set.
+        For FILTER, EDGE_FILTER the bundle will be located if autoLoc has been set.
         
-        FOR FILTER, EDGE_FILTER the mask will be located if autoMask has been set.
-
+        For FILTER, EDGE_FILTER the mask will be located if autoMask has been set.
         
         """
-       
         assert self.calibImage is not None, "Calibration requires calibration image, use set_calib_image()."
         
         if self.coreMethod == self.TRILIN:
             if self.calibImage is not None:
 
                 self.calibration = pybundle.calib_tri_interp(self.calibImage, self.coreSize, self.gridSize, 
                                                          background = self.background, 
                                                          normalise = self.normaliseImage,
-                                                         filterSize = self.filterSize)
-        
+                                                         filterSize = self.filterSize,
+                                                         mask = True,
+                                                         autoMask = True)
         else:
             
             if self.autoLoc and self.calibImage is not None:
                 self.loc = pybundle.find_bundle(self.calibImage)
                 self.autoLoc = False    
             
             if self.autoMask and self.calibImage is not None and self.loc is not None:
@@ -384,15 +513,18 @@
         if self.coreMethod == self.EDGE_FILTER:
              assert self.loc is not None, "Calibration for edge filter requires the bundle location."
              assert type(self.edgeFilterShape) is tuple, "Edge filter shape not defined."
              self.edgeFilter = pybundle.edge_filter(self.loc[2] *2 , self.edgeFilterShape[0], self.edgeFilterShape[1])
             
     
     def calibrate_sr(self):
-        """ Creates calibration for TRILIN SR method. A calibration image, set of super-res shift images, coreSize and griSize must have been set prior to calling this."""
+        """ Creates calibration for TRILIN SR method. A calibration image, 
+        set of super-res shift images, coreSize and gridSize must have been 
+        set prior to calling this.
+        """
         
         if self.srCalibImages is not None or self.srShifts is not None:
             self.calibrationSR = pybundle.SuperRes.calib_multi_tri_interp(
                 self.calibImage, self.srCalibImages,                                                                           
                 self.coreSize, self.gridSize, 
                 background = self.background, 
                 normalise = self.normaliseImage,
@@ -404,17 +536,21 @@
                 multiBackgrounds = self.srMultiBackgrounds,
                 multiNormalisation = self.srMultiNormalisation,
                 darkFrame = self.srDarkFrame,
                 filterSize = self.filterSize)
 
     
     def process(self, img):
-        """ Process fibre bundle image using current settings .
-        :param img: input image as 2D numpy array
-        :return: processing image as 2D numpy array
+        """ Process fibre bundle image using current settings.
+        
+        Returns processed image as 2D/3D numpy array.
+        
+        Arguments:
+            img: input image as 2D/3D numpy array
+            
         """
         
         method = self.coreMethod  # to insulate against a change during processing
         
         imgOut = img        
         
         
@@ -449,23 +585,26 @@
             mask = self.mask
             
             
         # Background subtraction (This is handled separately for TRILIN)     
         if method == self.FILTER or method == self.EDGE_FILTER:
             if self.background is not None:
                 imgOut = imgOut - self.background
+                
         
+        # Normalisation (This is handled separately for TRILIN)     
+        if method == self.FILTER or method == self.EDGE_FILTER:
+            if self.normaliseImage is not None:
+                imgOut = normalise_image(imgOut, self.normaliseImage)              
+
         
         # Gaussian Filter
         if method == self.FILTER and self.filterSize is not None:
-            imgOut = pybundle.g_filter(imgOut, self.filterSize)
-            
-                
-       
-            
+            imgOut = pybundle.g_filter(imgOut, self.filterSize)            
+                  
                 
         # Masking
         if (method == self.FILTER or method == self.EDGE_FILTER) and mask is not None:
             imgOut = pybundle.apply_mask(imgOut, mask)
        
         
         # Cropping
@@ -528,17 +667,19 @@
             imgOut = imgOut / np.max(imgOut)
             if self.outputType == 'uint8':
                 imgOut = imgOut * 255
             elif self.outputType == 'uint16':
                 imgOut = imgOut * (2**16 - 1)
             elif self.outputType == 'float':
                 imgOut = imgOut
-        
+                
+                
         # Type casting
-        imgOut = imgOut.astype(self.outputType)        
+        if imgOut.dtype != self.outputType:
+            imgOut = imgOut.astype(self.outputType)        
         
         return imgOut
     
 
     def get_pixel_scale(self):
         """ Returns the scaling factor between the pixel size in the raw image
         and the pixel size in the processed image. If the TRILIN method is
@@ -563,24 +704,42 @@
                 else:
                     return None
         else:    
             return 1  
         
         
     def set_super_res(self, sr):
-        """ Enables or disables super resoution, sr is boolean"""
+        """ Enables or disables super resolution.
+        
+        Arguments:
+            sr : boolean, True to use super-resolution.
+        """
         self.superRes = sr
         
         
     def set_sr_use_lut(self, useLUT):
-        """ Enables or disables use of calibration LUT for super resoution, useLUT is boolean"""
+        """ Enables or disables use of calibration LUT for super resoution.
+        
+        Arguments:
+            useLUT : boolean, True to use calibration LUT.
+            
+        """
         self.srUseLut = useLUT
         
     def calibrate_sr_lut(self, paramCalib, paramRange, nCalibrations) :   
-        """ Creates calibration LUT for TRILIN SR method. A calibration image, set of super-res shift images, coreSize and griSize must have been set prior to calling this."""
+        """ Creates calibration LUT for TRILIN SR method. A calibration image, 
+        set of super-res shift images, coreSize and griSize must have been 
+        set prior to calling this.
+        
+        Arguments:
+            paramCalib   :  parameter shift calibration, as generated by calib_param_shift()
+            paramRange   :  tuple of (min, max) defining range of parameter values to generate for
+            nCalibration : int, number of parameter values to generate for
+            
+        """
    
         if self.srCalibImages is not None or self.srShifts is not None:
             self.srCalibrationLUT = pybundle.calibrationLUT(
                 self.calibImage, self.srCalibImages,                                                                           
                 self.coreSize, self.gridSize, 
                 paramCalib, paramRange, nCalibrations,
                 background = self.background,
```

### Comparing `PyFibreBundle-1.3/src/pybundle/super_res.py` & `PyFibreBundle-1.3.1/src/pybundle/super_res.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 This file contains the SuperRes class which has functions for improving
 resolution of fibre bundle images by combining multiple images of the 
 object shifted with respect to the bundle core pattern.
 
 The preferred way to use the functionality is via the PyBundle class rather 
 than calling these functions directly.
 
-@author: Mike Hughes
-Applied Optics Group
-University of Kent
+@author: Mike Hughes, Applied Optics Group, University of Kent
 """
 
 import pybundle
 import time
 
 import numpy as np
 
@@ -37,41 +35,48 @@
 
 class SuperRes:
 
     def calib_multi_tri_interp(calibImg, imgs, coreSize, gridSize, **kwargs):
         """ Calibration step for super-resolution reconstruction. Either specify the
         known shifts between images, or provide an example set of images
         which the shifts will be calculated from. 
+        
+        Returns instance of BundleCalibration.
+        
+        Arguments:
 
-        :param calibImg: calibration image of fibre bundle, 2D numpy array
-        :param imgs: example set of images with the same set of mutual shifts as the images to
-            later be used to recover an enhanced resolution image from. 3D numpy array.
-            Can be None if 'shifts' is specified instead.
-        :param coreSize: estimate of average spacing between cores
-        :param gridSize: output size of image, supply a single value, image will be square
-        :param normalise: optional, image used for normalisation, as 2D numpy array. Can be same as calibration image, defaults to no normalisation
-        :param background: image used for calibration and , optionally, for background subtraction, as 2D numpy array, defaults to no background
-        :param shifts: optional, known x and y shifts between images as 2D numpy array of size (numImages,2). 
-                       Will override 'imgs' if specified as anything other than None.
-        :param centreX: optional, x centre location of bundle, if not specified will be determined automatically
-        :param centreY: optional, y centre location of bundle, if not specified will be determined automatically
-        :param radius: optional, radius of bundle, if not specified will be determined automatically
-        :param filterSize: optional, sigma of Gaussian filter applied when finding cores, defaults to no filter
-        :param normToImage: optional, if True each image will be normalised to have the same mean intensity. Defaults to False.
-        :param normToBackground: optional, if true, each image will be normalised with respect to the corresponding 
-                       background image from a stack of background images (one for each shift position) provided in backgroundImgs. 
-                       Defaults to False.
-        :param backgroundImgs: optional, stack of images, same size as imgs which are used to normalise or for image by image background subtraction. Defaults to None.
-        :param multiBackgrounds: boolean, if True and backgroundImgs is defined, each image will have its own background image subtracted rather than using backgroundImg
-        :param imageScaleFactor: If normToBackground and normToImage are False (default), use this to specify the normalisation factors for each image. Provide a 1D array the same size as the number of shifted images. Each image will be multiplied by the corresponding factor prior to reconstruction. Default is None (i.e. no scaling).
-        :param autoMask: optional, mask pixels outside bundle when searching for cores. Defualts to True.
-        :param mask: optional, boolean, when reconstructing output image will be masked outside of bundle. Defaults to True
-        :return: instance of BundleCalibration
+               calibImg   : calibration image of fibre bundle, 2D numpy array
+               imgs       : example set of images with the same set of mutual shifts as the images to
+                            later be used to recover an enhanced resolution image from. 3D numpy array.
+                            Can be None if 'shifts' is specified instead.
+               coreSize   : float, estimate of average spacing between cores
+               gridSize   : int, output size of image, supply a single value, image will be square
+               
+        Keyword Arguments:       
+              
+               normalise  : image used for normalisation, as 2D numpy array. Can be same as calibration image, defaults to no normalisation
+               background : image used for background subtraction, as 2D numpy array, defaults to no background
+               shifts     : known x and y shifts between images as 2D numpy array of size (numImages,2). 
+                            Will override doing registration of 'imgs' if specified as anything other than None.
+               centreX    : int, x centre location of bundle, if not specified will be determined automatically
+               centreY    : int, y centre location of bundle, if not specified will be determined automatically
+               radius     : int, radius of bundle, if not specified will be determined automatically
+               filterSize : float, sigma of Gaussian filter applied when finding cores, defaults to no filter
+               normToImage: boolean, if True each image will be normalised to have the same mean intensity. Defaults to False.
+               normToBackground : optional, if true, each image will be normalised with respect to the corresponding 
+                                  background image from a stack of background images (one for each shift position) provided in backgroundImgs. 
+                                  Defaults to False.
+               backgroundImgs   : stack of images, same size as imgs which are used to normalise or for image by image background subtraction. Defaults to None.
+               multiBackgrounds : boolean, if True and backgroundImgs is defined, each image will have its own background image subtracted rather than using backgroundImg
+               imageScaleFactor : If normToBackground and normToImage are False (default), use this to specify the normalisation factors for each image. Provide a 1D array the same size as the number of shifted images. Each image will be multiplied by the corresponding factor prior to reconstruction. Default is None (i.e. no scaling).
+               autoMask         : boolean, mask pixels outside bundle when searching for cores. Defualts to True.
+               mask:            : boolean, when reconstructing output image will be masked outside of bundle. Defaults to True
 
         """
+        
         shifts = kwargs.get('shifts', None)
         centreX = kwargs.get('centreX', None)
         centreY = kwargs.get('centreY', None)
         radius = kwargs.get('radius', None)
         filterSize = kwargs.get('filterSize', None)
         normToImage = kwargs.get('normToImage', False)
         normToBackground = kwargs.get('normToBackground', False)
@@ -187,17 +192,15 @@
             multiNormalisationVals = np.zeros((calib.nCores, nImages))
 
             for idx in range(nImages):
                 multiNormalisationVals[:, idx] = pybundle.core_values(normalisationImgs[:,:,idx], singleCalib.coreX, singleCalib.coreY, filterSize).astype('double') - darkVals
         
             calib.multiNormalisationVals = multiNormalisationVals
 
-       
-            
-            
+          
         # Have to set 'background' and 'normalise' to None in previous line as the cores are the shifted
         # positions in the full set from all the images and not the actual core position in each images.
         # We later copy across the background/normalise values from the single image calibration.
 
         calib.coreXShifted = calib.coreX
         calib.coreYShifted = calib.coreY
         
@@ -227,23 +230,29 @@
                 np.zeros((gridSize, gridSize)), (gridSize/2, gridSize/2, gridSize/2))
         else:
             calib.mask = None
 
         return calib
     
 
-    def recon_multi_tri_interp(imgs, calib, **kwargs):
-        """ Reconstruct image with super-resolution from set of shifted image. Requires calibration
-        to have been performed and stored in 'calib' as instance of BundleCalibration.
-        :param imgs: set of shifted images
-        :param calib: calibration, instance of BundleCalibration (must be
-            created by calib_multi_tri_interp and not calib_tri_interp).
-        :return: reconstructed image as 2D numpy array
+    def recon_multi_tri_interp(imgs, calib, numba = True):
+        """ Reconstruct image with super-resolution from set of shifted image. 
+        Requires calibration to have been performed and stored in 'calib' as 
+        instance of BundleCalibration.
+        
+        Returns reconstructed image as 2D numpy array
+        
+        Arguments:
+            imgs     : set of shifted images
+            calib    : calibration, instance of BundleCalibration (must be
+                    created by calib_multi_tri_interp and not calib_tri_interp).
+            
+        Keyword Arguments:
+            numba    : boolean, if True Numba JIT will be used (default).
         """
-        numba = kwargs.get('numba', True)
 
         nImages = np.shape(imgs)[2]
 
         cVals = []
         #print("recon filter", str(calib.filterSize))
         for i in range(nImages):
 
@@ -296,27 +305,35 @@
 
         if calib.mask is not None:
             imgOut = pybundle.apply_mask(imgOut, calib.mask)
 
         return imgOut
 
 
-    def get_shifts(imgs, **kwargs):
+    def get_shifts(imgs, templateSize = None, refSize = None, upsample = 2, **kwargs):
         """ Determines the shift of each image in a stack w.r.t. first image
-        :param imgs: stack of images as 3D numpy array
-        :param templateSize: a square of this size is extracted from imgs as the template
-        :param refSize: a sqaure of this size is extracted from first image as the reference image. 
-           Must be bigger than templateSize and the maximum shift detectable is 
-           (refSize - templateSize)/2        
-        :param upSample: upsampleing factor for images before shift detection for sub-pixel accuracy
-        :return: shifts as 2D numpy array
+        
+        Return shifts as 2D numpy array.
+        
+        Arguments:
+            
+            imgs         : stack of images as 3D numpy array
+            
+        Keyword Arguments:
+            
+            templateSize : int, a square of this size is extracted from imgs 
+                           as the template, default is 1/4 image size
+            refSize      : int, a square of this size is extracted from first 
+                           image as the reference image, default is 1/2 image
+                           size. Must be bigger than  
+                           templateSize and the maximum shift detectable is 
+                           (refSize - templateSize)/2   
+            upSample     : upsampling factor for images before shift detection  
+                           for sub-pixel accuracy, default is 2.
         """
-        templateSize = kwargs.get('templateSize', None)
-        refSize = kwargs.get('refSize', None)
-        upsample = kwargs.get('upSample', 2)
 
         imgSize = np.min(np.shape(imgs[:, :, 0]))
 
         if templateSize is None:
             templateSize = imgSize / 4
 
         if refSize is None:
@@ -332,28 +349,39 @@
 
             shifts[iImage, 0] = thisShift[0]
             shifts[iImage, 1] = thisShift[1]
 
         return shifts
     
 
-    def find_shift(img1, img2, templateSize, refSize, upsample, **kwargs):
-        """ Determines shift between two images by Normalised Cross Correlation (NCC). A sqaure template extracted
-        from the centre of img2 is compared with a sqaure region extracted from the reference image img1. The size 
-        of the template (templateSize) must be less than the size of the reference (refSize). The maximum
-        detectable shift is the (refSize - templateSize) / 2.
-        : param img1 : image as 2D numpy array
-        : param img2 : image as 2D numpy array
-        : param templateSize : size of square region of img2 to use as template. 
-        : param refSize : size of square region of img1 to template match with
-        : upsample : factor to scale images by prior to template matching to
-                     allow for sub-pixel registration.        
+    def find_shift(img1, img2, templateSize, refSize, upsample, returnMax = False):
+        """ Determines shift between two images by Normalised Cross 
+        Correlation (NCC). A square template extracted from the centre of img2 
+        is compared with a square region extracted from the reference image 
+        img1. The size of the template (templateSize) must be less than the 
+        size of the reference (refSize). The maximum detectable shift is 
+        (refSize - templateSize) / 2.
+        
+        If returnMax is False, returns shift as a tuple of (x_shift, y_shift).
+        If returnMax is True, returns tuple of (shift, cc. peak value).
+        
+        Arguments:
+            img1         : image as 2D numpy array
+            img2         : image as 2D numpy array
+            templateSize : int, size of square region of img2 to use as template. 
+            refSize      : int, size of square region of img1 to template match with
+            upsample     : int, factor to scale images by prior to template matching to
+                           allow for sub-pixel registration.  
+                           
+        Keyword Arguments:
+            returnMax    : boolean, if true returns cc.peak value as well
+                           as shift, default is False. 
+                   
         """
         
-        returnMax = kwargs.get('returnMax', False)
 
         if refSize < templateSize or min(np.shape(img1)) < refSize or min(np.shape(img2)) < refSize:
             return -1
         else:
 
             template = pybundle.extract_central(img2, templateSize).astype('float32')
             refIm = pybundle.extract_central(img1, refSize).astype('float32')
@@ -369,32 +397,42 @@
             min_val, max_val, min_loc, max_loc = cv.minMaxLoc(res)
             shift = [(max_loc[0] - (refSize - templateSize) * upsample)/upsample,
                      (max_loc[1] - (refSize - templateSize) * upsample)/upsample]
             if returnMax:
                 return shift, max_val
             else:
                 return shift
+            
 
     def sort_sr_stack(stack, stackLength):
         """ Takes a stack of images and extracts an ordered set
         of images relative to a reference 'blank' frame which is much lower intensity than
         the other frames. 
 
         The blank frame can be anywhere in the stack, and the output stack will be formed cyclically
         from frames before and after the blank frame. For example, if we have frames:
-           1  2  3  B  4  5
+        
+        1  2  3  B  4  5
+        
         where B is the blank frame, the function will return a stack in the following order:
-           4  5  1  2  3
+        
+        4  5  1  2  3
                    
         The input stack, 'stack' should should have (stackLength + 1)  frames to ensure that a 
         and there must be stackLength + 1 images in each cycle
         (i.e. stackLength useful images plus one blank reference image).
         The blank reference image is not returned, i.e the returned stack has stackLength frames.
         
         Input stack should have frame number in third dimension.
+        
+        Arguments:
+            
+             stack       : 3D numpy array (y,x, image_number)
+             stackLength : number of image after blank frame
+             
         """
         
         meanVal = np.mean(np.mean(stack,1),0)        
         blankFrame = np.argmin(meanVal)
         
         outOrder = np.arange(blankFrame + 1, blankFrame + 1 + stackLength)
         
@@ -406,19 +444,23 @@
         for idx in range(stackLength):
             
             outStack[:,:,idx] = stack[:,:,outOrderWrapped[idx]] 
     
         return outStack
     
         
-    def multi_tri_backgrounds(calibIn, backgrounds) :
+    def multi_tri_backgrounds(calibIn, backgrounds):
          """ Updates a multi_tri calibration with a new set of backgrounds without requiring
-         full recalibration
-         :param calibIn: bundle calibration, instance of BundleCalibration
-         :param background: background image as 2D numpy array
+         full recalibration.
+         
+         Returns instance of BundleCalibration.
+         
+         Arguments:
+             calibIn    : bundle calibration, instance of BundleCalibration
+             background : background image as 2D numpy array
          """
          calibOut = calibIn
     
          if background is not None:
              calibOut.backgroundVals = pybundle.core_values(background, calibOut.coreX, calibOut.coreY,calibOut.filterSize).astype('double')
              calibOut.background = background
     
@@ -428,18 +470,21 @@
              
          return calibOut 
 
         
     def calib_param_shift(param, images, calibration):
         """ For use when the shifts between the images are linearly dependent on some other parameter. 
         Provide a TRILIN calibration and a 4D stack of images of (x, y, shift, parameter), i.e. an extra 
-        dimensions to provide examples of shifts for differentvalues of the parameter. The values of the parameter
+        dimension to provide examples of shifts for different values of the parameter. The values of the parameter
         corresponding to each set of images is provided in param, i.e. the fourth dimension of images should be
         the same length as param.
+        
         Returns a 3D array of calibration factors, giving the gradient and offset of x and y shifts of each image with respect to the parameter.
+        
+        
         """
         nSets = np.shape(images)[3]
         nShifts = np.shape(images)[2]
         imgRecon = np.zeros((calibration.gridSize, calibration.gridSize, nShifts))
         shifts = np.zeros((nShifts, 2, nSets))
         shiftFit = np.zeros((nShifts, 2, 2))    # 2 dimensions (x,y) and 2 params of linear fit
         assert len(param) == nSets
@@ -474,16 +519,15 @@
          singleCalib = pyb.calib_multi_ti_interp(calibImg, coreSize, gridSize, **kwargs)
          for idx in range(np.shape(shiftsSet)[2]):
              kwargs.update({'shifts': shiftsSet[:,:,idx]})    # Add this set of shifts a calibrate
              calib = SuperRes.calib_multi_tri_interp(calibImg, imgs, coreSize, gridSize, singleCalib = singleCalib, **kwargs)
              calibrationSRs.append(calib)
     
     
-class calibrationLUT:
-    
+class calibrationLUT:   
     
     """ Creates and stores a SR calibration look up table (LUT) containing SR calibrations for different 
     values of some parameter on which the image shift is linearly dependent. paramRange is a tuple of (min, max) values of the parameters, and nCalibrations
     calibration will be generated equally spaced within this range. paramCalib is the output from a 
     calib_param_shift that allows the shifts for a specific.
     """
     def __init__(self, calibImg, imgs, coreSize, gridSize, paramCalib, paramRange, nCalibrations, **kwargs):
```

### Comparing `PyFibreBundle-1.3/test/test_all.py` & `PyFibreBundle-1.3.1/test/test_all.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 @author: Mike Hughes, Applied Optics Group, University of Kent
 """
 
 print("\ntest_simple_processing")
 print("-------------------------")
 import test_simple_processing
 
+print("\ntest_simple_processing_col")
+print("-------------------------")
+import test_simple_processing_col
+
 print("\ntest_masking (low-level)")
 print("-------------------------")
 import test_masking
 
 print("\ntest_masking (class)")
 print("-------------------------")
 import test_mask
@@ -29,14 +33,18 @@
 print("-------------------------")
 import test_mosaic
 
 print("\ntest_pybundle_oop")
 print("-------------------------")
 import test_pybundle_oop
 
+print("\ntest_image_types_oop")
+print("-------------------------")
+import test_processing_im_type
+
 print("\ntest_recon_tri_interp")
 print("-------------------------")
 import test_recon_tri_interp
 
 print("\ntest_super_res")
 print("-------------------------")
-import test_super_res
+import test_super_res_oop
```

### Comparing `PyFibreBundle-1.3/test/test_find_cores.py` & `PyFibreBundle-1.3.1/test/test_find_cores.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3/test/test_loc.py` & `PyFibreBundle-1.3.1/test/test_loc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-
+# -*- coding: utf-8 -*-
 """
 Tests the location find routines
 
 @author: Mike Hughes, Applied Optics Group, University of Kent
 """
 from matplotlib import pyplot as plt
 import numpy as np
 import os
 import time
+from pathlib import Path
 
 from PIL import Image
 
 import context    # Add relative path to get pybundle
 
 from pybundle import PyBundle 
 import pybundle
 
-from pathlib import Path
-
 
 img = np.array(Image.open(Path('data/usaf1.tif')))
 calibImg = np.array(Image.open(Path('data/usaf1_background.tif')))
 
 
-
 pyb = PyBundle(coreMethod = PyBundle.FILTER, filterSize = 2)
 imgProc = pyb.process(img)
 #plt.figure(dpi = 150); plt.title('Default'); plt.imshow(imgProc, cmap = 'gray')
 
 assert np.shape(imgProc)[0] != np.shape(imgProc)[1] 
 
 
@@ -53,14 +51,17 @@
 pyb = PyBundle(coreMethod = PyBundle.FILTER, filterSize = 2, crop = True, autoLoc = False, loc = (200,200,100) )
 imgProc = pyb.process(img)
 #plt.figure(dpi = 150); plt.title('crop = True, autoLoc default loc set'); plt.imshow(imgProc, cmap = 'gray')
 
 assert np.shape(imgProc) == (200,200)
 
 
+
+
+
 pyb = PyBundle(coreMethod = PyBundle.FILTER, filterSize = 2, crop = True, autoLoc = True, loc = (200,200,100) )
 imgProc = pyb.process(img)
 #plt.figure(dpi = 150); plt.title('crop = True, autoLoc = True, loc set'); plt.imshow(imgProc, cmap = 'gray')
 
 assert np.shape(imgProc) != (200,200)
 assert np.shape(imgProc)[0] == np.shape(imgProc)[1]
```

### Comparing `PyFibreBundle-1.3/test/test_mask.py` & `PyFibreBundle-1.3.1/test/test_mask.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3/test/test_masking.py` & `PyFibreBundle-1.3.1/test/test_masking.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 Tests the cropping and mask functionality of pybundle
 
-@author: Mike Hughes
-Applied Optics Group
-University of Kent
+@author: Mike Hughes, Applied Optics Group, University of Kent
 """
 
 from matplotlib import pyplot as plt
 from PIL import Image
 import numpy as np
 
 import context
```

### Comparing `PyFibreBundle-1.3/test/test_masking_col.py` & `PyFibreBundle-1.3.1/test/test_masking_col.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # -*- coding: utf-8 -*-
 """
-Tests the cropping and mask functionality of pybundle
+Tests the cropping and mask functionality of pybundle with colour images
 
-@author: Mike Hughes
-Applied Optics Group
-University of Kent
+@author: Mike Hughes, Applied Optics Group, University of Kent
 """
 
 from matplotlib import pyplot as plt
 from PIL import Image
 import numpy as np
 
 import context
```

### Comparing `PyFibreBundle-1.3/test/test_mosaic.py` & `PyFibreBundle-1.3.1/test/test_mosaic.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3/test/test_mosaic_col.py` & `PyFibreBundle-1.3.1/test/test_mosaic_col.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,27 +32,26 @@
 calibImg = calibImg[:,:,::-1]
 
 # Create PyBundle object for core removal
 pyb = PyBundle(coreMethod = PyBundle.TRILIN,  # Set to remove core pattern by trianglar linear interpolation
                coreSize = 3,                  # Providing an estimate of the core spacing in pixels help to identify core locations robustly
                calibImage = calibImg,
                normaliseImage = calibImg,
-               outputType = 'uint16',
                autoContrast = False)
 pyb.calibrate()
 
 
 # Create mosaic object
 mosaic = Mosaic(1000, resize = 250)
 
 # Read in one image and process
 ret, img = cap.read()
 img = img[:,:,::-1]
 imgProc = pyb.process(img)
-imgStack = np.zeros([nFrames, 512, 512, 3 ], dtype='uint8' ) 
+imgStack = np.zeros([nFrames, 512, 512, 3 ], dtype='uint16' ) 
 imgStack[0,:,:,:] = imgProc
 
 
 # Load video frames
 for i in range(1,nFrames):
     cap.set(cv.CAP_PROP_POS_FRAMES, i)
     ret, img = cap.read()
@@ -66,20 +65,20 @@
 # it is passed here as 'mosaic' with a 'description' used to label the output
 def test_mosaic(mosaic, description):
    
     mosaic.reset()
     t0 = time.time()
     for i in range(nFrames):   
         img = imgStack[i,:,:,:]
+       
         mosaic.add(img)   
         mosaicImage = mosaic.get_mosaic()
-        #cv.imshow('ImageWindow',cv.resize(mosaicImage,(400,400)).astype('uint8'))
-        #cv.waitKey(1)
+
     plt.figure()
-    plt.imshow(mosaicImage, cmap = 'gray') 
+    plt.imshow(mosaicImage / np.max(mosaicImage), cmap = 'gray') 
     plt.title(description)
  
     print(f"{description}: Average time to add a frame to mosaic: {str(1000 * round( (time.time() - t0)/nFrames,3))} ms.")
 
 
 # The tests
 
@@ -88,17 +87,14 @@
 
 mosaic = Mosaic(1000, blend = False)
 test_mosaic(mosaic, "Default, no blend")
 
 mosaic = Mosaic(1000, resize = 250)
 test_mosaic(mosaic, "Default with resize to 250")
 
-mosaic = Mosaic(10000, resize = 250)
-test_mosaic(mosaic, "Default with 10k x 10k image, resize to 250")
-
 mosaic = Mosaic(1000, resize = 250, blend = False)
 test_mosaic(mosaic, "No Blend")
 
 mosaic = Mosaic(1000, resize = 250, blend = True)
 test_mosaic(mosaic, "Blend")
 
 mosaic = Mosaic(1000, resize = 250, blend = True, blendDist = 5)
```

### Comparing `PyFibreBundle-1.3/test/test_pybundle_oop.py` & `PyFibreBundle-1.3.1/test/test_pybundle_oop.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3/test/test_recon_tri_interp.py` & `PyFibreBundle-1.3.1/test/test_recon_tri_interp.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3/test/test_recon_tri_interp_col.py` & `PyFibreBundle-1.3.1/test/test_recon_tri_interp_col.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # -*- coding: utf-8 -*-
 """
-Test removal of fibre bundle core pattern by 
+Test removal of fibre bundle core pattern for colour images by 
 Delaunay triangulation and triangular linear interpolation.
 
 This also tests the faster numba-based option. 
 
-@author: Mike Hughes
-Applied Optics Group
-University of Kent
+@author: Mike Hughes, Applied Optics Group, University of Kent
 """
 
 from matplotlib import pyplot as plt
 import numpy as np
 import time
 
 from PIL import Image
 
 import context    # Add relative path to get PyBundle
 import os
 import cv2 as cv
+
 import pybundle
 
 # We load in two images, an image with uniform illumination for calibation
 # and an image of a USAF resolution target to demonstrate core removal
 img = np.array(Image.open("data\\bundle_colour_1.tif"))
 calibImg = np.array(Image.open("data\\bundle_colour_1_background.tif"))
```

### Comparing `PyFibreBundle-1.3/test/test_simple_processing.py` & `PyFibreBundle-1.3.1/test/test_simple_processing.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3/test/test_simple_processing_col.py` & `PyFibreBundle-1.3.1/test/test_simple_processing_col.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3/test/test_sr_sort_stack.py` & `PyFibreBundle-1.3.1/test/test_sr_sort_stack.py`

 * *Files identical despite different names*

### Comparing `PyFibreBundle-1.3/test/test_super_res.py` & `PyFibreBundle-1.3.1/test/test_super_res.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,29 +56,29 @@
 plt.figure(dpi = 150)
 plt.imshow(reconSingle, cmap='gray')
 plt.title('Single Image')
  
 
 """ Super Resolution Recon """
 t1 = time.perf_counter()
-calib = SuperRes.calib_multi_tri_interp(calibImg, imgs, coreSize, gridSize, filterSize = filterSize, background = calibImg, normalise = calibImg, autoMask = True)
+calib = SuperRes.calib_multi_tri_interp(calibImg, imgs, coreSize, gridSize, filterSize = filterSize, normalise = calibImg, autoMask = True)
 print("Calibration time:", round(time.perf_counter() - t1, 3))
 
 t1 = time.perf_counter()
 reconImg = SuperRes.recon_multi_tri_interp(imgs, calib)
 print("Reconstruction time:", round(time.perf_counter() - t1, 3))
 
 plt.figure(dpi = 150)
 plt.imshow(reconImg, cmap='gray')
 plt.title('SR Image')
 
 
 """ Super Resolution Recon with Intensity Normalisation"""
 t1 = time.perf_counter()
-calib = SuperRes.calib_multi_tri_interp(calibImg, imgs, coreSize, gridSize, filterSize = filterSize, background = calibImg, normalise = calibImg, normToImage = True, autoMask = True)
+calib = SuperRes.calib_multi_tri_interp(calibImg, imgs, coreSize, gridSize, filterSize = filterSize, normalise = calibImg, normToImage = True)
 print("Calibration time:", round(time.perf_counter() - t1, 3))
 
 t1 = time.perf_counter()
 reconImg = SuperRes.recon_multi_tri_interp(imgs, calib)
 print("Reconstruction time:", round(time.perf_counter() - t1, 3))
 
 plt.figure(dpi = 150)
@@ -92,15 +92,15 @@
                    [-24.75892784, -12.66735843],
                    [-28.21366196, -21.87998274],
                    [ -2.8789451 , -10.93999137],
                    [ -4.60631216, -16.69788157],
                    [ -9.78841333, -30.51681804],
                    [-17.27367059, -27.06208392]])
 t1 = time.perf_counter()
-calib = SuperRes.calib_multi_tri_interp(calibImg, None, coreSize, gridSize,  shifts = shifts, filterSize = filterSize, background = calibImg, normalise = calibImg, autoMask = True)
+calib = SuperRes.calib_multi_tri_interp(calibImg, None, coreSize, gridSize,  shifts = shifts, filterSize = filterSize, normalise = calibImg)
 print(f"Calibration time: {round(time.perf_counter() - t1, 3)} s")
 
 t1 = time.perf_counter()
 reconImg = SuperRes.recon_multi_tri_interp(imgs, calib)
 print(f"Reconstruction time: {round(time.perf_counter() - t1, 3)} s")
 
 plt.figure(dpi = 150)
```

### Comparing `PyFibreBundle-1.3/test/test_super_res_oop.py` & `PyFibreBundle-1.3.1/test/test_super_res_oop.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,16 +41,16 @@
 
 for idx, fName in enumerate(files[:nImages]):
     img = Image.open(fName)
     imgs[:,:,idx] = np.array(img)
 
 calibImg = np.array(Image.open(backFile))
 
-pyb = PyBundle(coreMethod = PyBundle.TRILIN, gridSize = gridSize, autoContrast = True, 
-               calibImage = calibImg, backgroundImage = calibImg, normaliseImage = calibImg)
+pyb = PyBundle(coreMethod = PyBundle.TRILIN, gridSize = gridSize, autoContrast = False, 
+               calibImage = calibImg, normaliseImage = calibImg, backgroundImage = calibImg)
 
 
 """ Single image recon for comparison """
 pyb.calibrate()
 reconSingle = pyb.process(imgs[:,:,0])
 
 """ Super Resolution Recon """
@@ -75,16 +75,16 @@
                     [-24.75892784, -12.66735843],
                     [-28.21366196, -21.87998274],
                     [ -2.8789451 , -10.93999137],
                     [ -4.60631216, -16.69788157],
                     [ -9.78841333, -30.51681804],
                     [-17.27367059, -27.06208392] ])
     
-pyb = PyBundle(coreMethod = PyBundle.TRILIN, superRes = True, gridSize = gridSize, autoContrast = True, 
-               calibImage = calibImg, backgroundImage = calibImg, normaliseImage = calibImg)
+pyb = PyBundle(coreMethod = PyBundle.TRILIN, superRes = True, gridSize = gridSize, autoContrast = False, 
+               calibImage = calibImg, normaliseImage = calibImg)
 
 pyb.set_sr_shifts(shifts)
 pyb.calibrate_sr()
 
 reconSR = pyb.process(imgs)
 
 plt.figure(dpi = 150)
```

