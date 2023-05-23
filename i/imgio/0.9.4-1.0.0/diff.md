# Comparing `tmp/imgio-0.9.4.tar.gz` & `tmp/imgio-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgio-0.9.4.tar", last modified: Fri May 12 14:01:55 2023, max compression
+gzip compressed data, was "imgio-1.0.0.tar", last modified: Tue May 23 14:49:39 2023, max compression
```

## Comparing `imgio-0.9.4.tar` & `imgio-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-12 14:01:55.728345 imgio-0.9.4/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 imgio-0.9.4/LICENSE
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       87 2023-03-13 15:45:56.000000 imgio-0.9.4/MANIFEST.in
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      253 2023-05-12 14:01:55.728345 imgio-0.9.4/PKG-INFO
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      661 2023-03-14 15:37:15.000000 imgio-0.9.4/README.md
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-12 14:01:55.724345 imgio-0.9.4/imgio/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      312 2023-05-12 13:56:46.000000 imgio-0.9.4/imgio/__init__.py
--rwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)    29811 2023-05-12 13:11:45.000000 imgio-0.9.4/imgio/imgio.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     4209 2023-05-12 14:00:48.000000 imgio-0.9.4/imgio/pfm.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     4518 2023-05-12 13:56:12.000000 imgio-0.9.4/imgio/pnm.py
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-12 14:01:55.728345 imgio-0.9.4/imgio/test-images/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    62336 2023-03-13 15:45:56.000000 imgio-0.9.4/imgio/test-images/GrayRampsDiagonal.exr
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   139435 2023-03-13 15:45:56.000000 imgio-0.9.4/imgio/test-images/landscape_1.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   137359 2023-03-13 15:45:56.000000 imgio-0.9.4/imgio/test-images/landscape_2.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   140965 2023-03-13 15:45:56.000000 imgio-0.9.4/imgio/test-images/landscape_3.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   140588 2023-03-13 15:45:56.000000 imgio-0.9.4/imgio/test-images/landscape_4.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   137611 2023-03-13 15:45:56.000000 imgio-0.9.4/imgio/test-images/landscape_5.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   137628 2023-03-13 15:45:56.000000 imgio-0.9.4/imgio/test-images/landscape_6.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   140645 2023-03-13 15:45:56.000000 imgio-0.9.4/imgio/test-images/landscape_7.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   141286 2023-03-13 15:45:56.000000 imgio-0.9.4/imgio/test-images/landscape_8.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   129059 2023-03-13 15:45:56.000000 imgio-0.9.4/imgio/test-images/portrait_1.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   136072 2023-03-13 15:45:56.000000 imgio-0.9.4/imgio/test-images/portrait_2.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   135813 2023-03-13 15:45:56.000000 imgio-0.9.4/imgio/test-images/portrait_3.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   131520 2023-03-13 15:45:56.000000 imgio-0.9.4/imgio/test-images/portrait_4.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   133715 2023-03-13 15:45:56.000000 imgio-0.9.4/imgio/test-images/portrait_5.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   136257 2023-03-13 15:45:56.000000 imgio-0.9.4/imgio/test-images/portrait_6.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   135366 2023-03-13 15:45:56.000000 imgio-0.9.4/imgio/test-images/portrait_7.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   132543 2023-03-13 15:45:56.000000 imgio-0.9.4/imgio/test-images/portrait_8.jpg
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-12 14:01:55.724345 imgio-0.9.4/imgio.egg-info/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      253 2023-05-12 14:01:55.000000 imgio-0.9.4/imgio.egg-info/PKG-INFO
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      872 2023-05-12 14:01:55.000000 imgio-0.9.4/imgio.egg-info/SOURCES.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-05-12 14:01:55.000000 imgio-0.9.4/imgio.egg-info/dependency_links.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-05-12 14:01:55.000000 imgio-0.9.4/imgio.egg-info/not-zip-safe
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       40 2023-05-12 14:01:55.000000 imgio-0.9.4/imgio.egg-info/requires.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        6 2023-05-12 14:01:55.000000 imgio-0.9.4/imgio.egg-info/top_level.txt
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       46 2023-03-14 15:16:06.000000 imgio-0.9.4/requirements.txt
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      128 2023-05-12 14:01:55.728345 imgio-0.9.4/setup.cfg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      605 2023-03-13 15:45:56.000000 imgio-0.9.4/setup.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-23 14:49:39.905876 imgio-1.0.0/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 imgio-1.0.0/LICENSE
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       87 2023-03-13 15:45:56.000000 imgio-1.0.0/MANIFEST.in
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      253 2023-05-23 14:49:39.905876 imgio-1.0.0/PKG-INFO
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      661 2023-03-14 15:37:15.000000 imgio-1.0.0/README.md
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-23 14:49:39.901876 imgio-1.0.0/imgio/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      312 2023-05-23 14:45:06.000000 imgio-1.0.0/imgio/__init__.py
+-rwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)    31404 2023-05-23 14:44:41.000000 imgio-1.0.0/imgio/imgio.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     4209 2023-05-12 14:00:48.000000 imgio-1.0.0/imgio/pfm.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     4518 2023-05-12 13:56:12.000000 imgio-1.0.0/imgio/pnm.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-23 14:49:39.905876 imgio-1.0.0/imgio/test-images/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    62336 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/GrayRampsDiagonal.exr
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   139435 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/landscape_1.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   137359 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/landscape_2.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   140965 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/landscape_3.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   140588 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/landscape_4.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   137611 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/landscape_5.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   137628 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/landscape_6.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   140645 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/landscape_7.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   141286 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/landscape_8.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   129059 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/portrait_1.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   136072 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/portrait_2.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   135813 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/portrait_3.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   131520 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/portrait_4.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   133715 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/portrait_5.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   136257 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/portrait_6.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   135366 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/portrait_7.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   132543 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/portrait_8.jpg
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-23 14:49:39.901876 imgio-1.0.0/imgio.egg-info/
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      253 2023-05-23 14:49:39.000000 imgio-1.0.0/imgio.egg-info/PKG-INFO
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      872 2023-05-23 14:49:39.000000 imgio-1.0.0/imgio.egg-info/SOURCES.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-05-23 14:49:39.000000 imgio-1.0.0/imgio.egg-info/dependency_links.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-05-23 14:49:39.000000 imgio-1.0.0/imgio.egg-info/not-zip-safe
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       40 2023-05-23 14:49:39.000000 imgio-1.0.0/imgio.egg-info/requires.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        6 2023-05-23 14:49:39.000000 imgio-1.0.0/imgio.egg-info/top_level.txt
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       46 2023-03-14 15:16:06.000000 imgio-1.0.0/requirements.txt
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      128 2023-05-23 14:49:39.905876 imgio-1.0.0/setup.cfg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      605 2023-03-13 15:45:56.000000 imgio-1.0.0/setup.py
```

### Comparing `imgio-0.9.4/LICENSE` & `imgio-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/README.md` & `imgio-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/imgio/imgio.py` & `imgio-1.0.0/imgio/imgio.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 
 ######################################################################################
 #
 #  P U B L I C   A P I
 #
 ######################################################################################
 
-RW_FORMATS = [".pnm", ".pgm", ".ppm", ".pfm", ".png", ".jpg", ".jpeg", ".tif", ".tiff", ".insp", ".npy", ".raw"]
-RO_FORMATS = RW_FORMATS + [".exr", ".bmp"]
+RW_FORMATS = [".pnm", ".pgm", ".ppm", ".pfm", ".png", ".jpg", ".jpeg", ".tif", ".tiff", ".insp", ".npy", ".raw", ".exr"]
+RO_FORMATS = RW_FORMATS + [".bmp"]
 
 def imread(filespec, width=None, height=None, bpp=None, raw_header_size=None, verbose=False):
     """
     Reads the given image file from disk and returns it as a NumPy array.
     Grayscale images are returned as 2D arrays of shape H x W, color images
     as 3D arrays of shape H x W x 3.
     """
@@ -118,14 +118,17 @@
         _enforce(packed is False, "packed Bayer RAW images are not yet supported.")
         _enforce(image.ndim == 2, "image.shape must be (m, n) for a Bayer RAW; was %s."%(str(image.shape)))
         _reraise(lambda: _write_raw(filespec, image, maxval, packed, verbose))
     elif filetype == ".pfm":
         _disallow(image.ndim == 3 and image.shape[2] != 3, "image.shape must be (m, n) or (m, n, 3); was %s."%(str(image.shape)))
         _enforce(maxval >= 0.0, "maxval (scale) must be non-negative; was %s."%(repr(maxval)))
         _reraise(lambda: pfm.write(filespec, image, maxval, little_endian=True, verbose=verbose))
+    elif filetype == ".exr":
+        _enforce(pyexr is not None, "OpenEXR support not installed")
+        _reraise(lambda: _write_exr(filespec, image, verbose))
     elif filetype == ".npy":
         _reraise(lambda: _write_npy(filespec, image, verbose))
     elif filetype in [".pnm", ".pgm", ".ppm"]:
         _reraise(lambda: pnm.write(filespec, image, maxval, verbose))
     elif filetype in [".png", ".tif", ".tiff", ".jpg", ".jpeg", ".insp"]:
         _disallow(image.ndim == 3 and image.shape[2] != 3, "image.shape must be (m, n) or (m, n, 3); was %s."%(str(image.shape)))
         _disallow(filetype in [".jpg", ".jpeg"] and maxval != 255, "maxval must be 255 for a JPEG; was %d."%(maxval))
@@ -194,33 +197,41 @@
     if orientation in exif_to_rot90:
         rot90_ccw_steps = exif_to_rot90[orientation]
         img = np.rot90(img, rot90_ccw_steps)  # 0/90/180/270 CCW
     return img
 
 def _read_exr(filespec, verbose=False):
     exr = pyexr.open(filespec)
-    data = exr.get()
+    precision = list(exr.channel_precision.values())[0]
+    data = exr.get(precision=precision)
     maxval = np.max(data)
     w, h, ch, dt = exr.width, exr.height, len(exr.channels), data.dtype
     _print(verbose, "Reading OpenEXR file %s (w=%d, h=%d, c=%d, %s)"%(filespec, w, h, ch, dt))
     return data, maxval
 
+def _write_exr(filespec, image, verbose=False):
+    h, w = image.shape[:2]
+    ch = image.shape[2] if image.ndim == 3 else 1
+    dt = pyexr.HALF if image.dtype == np.float16 else pyexr.FLOAT
+    channels = [f"ch{idx:02d}" for idx in range(ch)] if ch >= 5 else None
+    pyexr.write(filespec, image, precision=dt, channel_names=channels)
+    _print(verbose, "Writing OpenEXR file %s (w=%d, h=%d, c=%d, %s)"%(filespec, w, h, ch, image.dtype))
+
 def _read_npy(filespec, verbose=False):
     data = np.load(filespec)
     _enforce(data.ndim == 3, "NumPy file %s image has unsupported shape %s"%(filespec, str(data.shape)))
     maxval = np.max(data)
     h, w, ch = data.shape
     _print(verbose, "Reading NumPy file %s (w=%d, h=%d, c=%d, %s)"%(filespec, w, h, ch, data.dtype))
     return data, maxval
 
 def _write_npy(filespec, image, verbose=False):
     _enforce(image.ndim == 3, "image.shape must be (m, n, c) for .npy; was %s."%(str(image.shape)))
     h, w, ch = image.shape
-    if verbose:
-        print("Writing file %s (w=%d, h=%d, c=%d, %s)"%(filespec, w, h, ch, image.dtype))
+    _print(verbose, "Writing NumPy file %s (w=%d, h=%d, c=%d, %s)"%(filespec, w, h, ch, image.dtype))
     np.save(filespec, image)
 
 def _read_raw(filespec, width, height, bpp, header_size=None, verbose=False):
     # Warning: hardcoded endianness (x86)
     with open(filespec, "rb") as infile:
         buf = infile.read()
         shape = (height, width)
@@ -304,14 +315,15 @@
         self.assertRaisesRegex(ImageIOError, "^Failed to read", imread, "nonexisting/.ppm")
         self.assertRaisesRegex(ImageIOError, "^Failed to read", imread, "nonexisting/invalidfilename")
         self.assertRaisesRegex(ImageIOError, "^Failed to read", imread, "nonexisting.jpg")
         self.assertRaisesRegex(ImageIOError, "^Failed to read", imread, "nonexisting.png")
         self.assertRaisesRegex(ImageIOError, "^Failed to read", imread, "nonexisting.ppm")
         self.assertRaisesRegex(ImageIOError, "^Failed to read", imread, "nonexisting.pgm")
         self.assertRaisesRegex(ImageIOError, "^Failed to read", imread, "nonexisting.pfm")
+        self.assertRaisesRegex(ImageIOError, "^Failed to read", imread, "nonexisting.exr")
         self.assertRaisesRegex(ImageIOError, "^Failed to read", imread, "nonexisting.bmp")
         self.assertRaisesRegex(ImageIOError, "^Failed to read", imread, "invalidformat.pfm")
         self.assertRaisesRegex(ImageIOError, "^Failed to read", imread, "invalidformat.jpg")
         self.assertRaisesRegex(ImageIOError, "^Failed to read", imread, "invalidformat.ppm")
         self.assertRaisesRegex(ImageIOError, "^Failed to read.*verbose", imread, "validimage.ppm", verbose="foo")
         self.assertRaisesRegex(ImageIOError, "^Failed to write", imwrite, "invalidfilename", pixels8b, 255)
         self.assertRaisesRegex(ImageIOError, "^Failed to write", imwrite, "invalidtype.bmp", pixels8b, 255)
@@ -429,27 +441,42 @@
             self.assertEqual(result.dtype, np.float32)
             self.assertEqual(result.shape, shape)
             self.assertTrue(np.allclose(result, pixels))
             os.remove(tempfile)
 
     def test_npy(self):
         for dt in ["float16", "float32"]:
-            for shape in [(1, 1, 2), (1, 1, 9), (7, 11, 3), (9, 13, 31), (123, 321, 3)]:
+            for shape in [(1, 1, 1), (1, 1, 2), (1, 1, 9), (7, 11, 3), (9, 13, 31), (123, 321, 3)]:
                 scale = 3.141
                 tempfile = "imgio.test.npy"
                 print("Testing NPY reading & writing in %s mode, shape=%s..."%(dt, repr(shape)))
                 pixels = np.random.random(shape)  # float64 pixels
                 pixels = pixels.astype(dt)  # convert to float16/32
                 imwrite(tempfile, pixels, maxval=scale, verbose=False)
                 result, resscale = imread(tempfile, verbose=False)
                 self.assertEqual(result.dtype, dt)
                 self.assertEqual(result.shape, shape)
                 self.assertTrue(np.allclose(result, pixels))
                 os.remove(tempfile)
 
+    def test_exr(self):
+        for dt in ["float16", "float32"]:
+            for shape in [(1, 1, 1), (1, 1, 2), (1, 1, 9), (7, 11, 3), (9, 13, 31), (123, 321, 3)]:
+                scale = 3.141
+                tempfile = "imgio.test.exr"
+                print("Testing EXR reading & writing in %s mode, shape=%s..."%(dt, repr(shape)))
+                pixels = np.random.random(shape)  # float64 pixels
+                pixels = pixels.astype(dt)  # convert to float16/32
+                imwrite(tempfile, pixels, maxval=scale, verbose=False)
+                result, resscale = imread(tempfile, verbose=False)
+                self.assertEqual(result.dtype, dt)
+                self.assertEqual(result.shape, shape)
+                self.assertTrue(np.allclose(result, pixels))
+                os.remove(tempfile)
+
     def test_exif(self):
         print("Testing EXIF orientation handling...")
         thispath = os.path.dirname(os.path.abspath(__file__))
         for orientation in ["landscape", "portrait"]:
             reffile = "%s_1.jpg"%(orientation)
             filespec = os.path.join(thispath, "test-images", reffile)
             refimg, refmax = imread(filespec)
@@ -459,21 +486,21 @@
                 filespec = os.path.join(thispath, "test-images", filename)
                 testimg, testmax = imread(filespec, verbose=False)
                 epsdiff = np.isclose(refimg, testimg, atol=5.0, rtol=0.2)
                 self.assertEqual(refmax, testmax)
                 self.assertEqual(refimg.shape, testimg.shape)
                 self.assertGreater(np.sum(epsdiff), 0.5 * epsdiff.size)
 
-    def test_exr(self):
+    def test_exr_read(self):
         print("Testing EXR reading...")
         thispath = os.path.dirname(os.path.abspath(__file__))
         filespec = os.path.join(thispath, "test-images", "GrayRampsDiagonal.exr")
         img, maxval = imread(filespec)
         self.assertEqual(img.shape, (800, 800, 1))
-        self.assertEqual(img.dtype, np.float32)
+        self.assertEqual(img.dtype, np.float16)
         self.assertEqual(maxval, np.max(img))
 
     def test_raw(self):
         for packed in [False]:
             for shape in [(1, 1), (7, 11)]:
                 for bpp in [1, 5, 7, 8, 10, 12, 13, 16]:
                     maxval = 2**bpp - 1
```

### Comparing `imgio-0.9.4/imgio/pfm.py` & `imgio-1.0.0/imgio/pfm.py`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/imgio/pnm.py` & `imgio-1.0.0/imgio/pnm.py`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/imgio/test-images/GrayRampsDiagonal.exr` & `imgio-1.0.0/imgio/test-images/GrayRampsDiagonal.exr`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/imgio/test-images/landscape_1.jpg` & `imgio-1.0.0/imgio/test-images/landscape_1.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/imgio/test-images/landscape_2.jpg` & `imgio-1.0.0/imgio/test-images/landscape_2.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/imgio/test-images/landscape_3.jpg` & `imgio-1.0.0/imgio/test-images/landscape_3.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/imgio/test-images/landscape_4.jpg` & `imgio-1.0.0/imgio/test-images/landscape_4.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/imgio/test-images/landscape_5.jpg` & `imgio-1.0.0/imgio/test-images/landscape_5.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/imgio/test-images/landscape_6.jpg` & `imgio-1.0.0/imgio/test-images/landscape_6.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/imgio/test-images/landscape_7.jpg` & `imgio-1.0.0/imgio/test-images/landscape_7.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/imgio/test-images/landscape_8.jpg` & `imgio-1.0.0/imgio/test-images/landscape_8.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/imgio/test-images/portrait_1.jpg` & `imgio-1.0.0/imgio/test-images/portrait_1.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/imgio/test-images/portrait_2.jpg` & `imgio-1.0.0/imgio/test-images/portrait_2.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/imgio/test-images/portrait_3.jpg` & `imgio-1.0.0/imgio/test-images/portrait_3.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/imgio/test-images/portrait_4.jpg` & `imgio-1.0.0/imgio/test-images/portrait_4.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/imgio/test-images/portrait_5.jpg` & `imgio-1.0.0/imgio/test-images/portrait_5.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/imgio/test-images/portrait_6.jpg` & `imgio-1.0.0/imgio/test-images/portrait_6.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/imgio/test-images/portrait_7.jpg` & `imgio-1.0.0/imgio/test-images/portrait_7.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/imgio/test-images/portrait_8.jpg` & `imgio-1.0.0/imgio/test-images/portrait_8.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/imgio.egg-info/SOURCES.txt` & `imgio-1.0.0/imgio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imgio-0.9.4/setup.py` & `imgio-1.0.0/setup.py`

 * *Files identical despite different names*

