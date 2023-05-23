# Comparing `tmp/mathphys-2.8.0.tar.gz` & `tmp/mathphys-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathphys-2.8.0.tar", last modified: Tue May 23 18:59:23 2023, max compression
+gzip compressed data, was "mathphys-2.8.1.tar", last modified: Tue May 23 20:21:51 2023, max compression
```

## Comparing `mathphys-2.8.0.tar` & `mathphys-2.8.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:59:23.985159 mathphys-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-05-23 18:59:10.000000 mathphys-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-23 18:59:10.000000 mathphys-2.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-05-23 18:59:23.985159 mathphys-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1107 2023-05-23 18:59:10.000000 mathphys-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:59:23.985159 mathphys-2.8.0/mathphys/
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-23 18:59:22.000000 mathphys-2.8.0/mathphys/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)      577 2023-05-23 18:59:10.000000 mathphys-2.8.0/mathphys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-05-23 18:59:10.000000 mathphys-2.8.0/mathphys/base_units.py
--rw-r--r--   0 runner    (1001) docker     (122)     2385 2023-05-23 18:59:10.000000 mathphys-2.8.0/mathphys/beam_optics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-05-23 18:59:10.000000 mathphys-2.8.0/mathphys/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     6242 2023-05-23 18:59:10.000000 mathphys-2.8.0/mathphys/functions.py
--rw-r--r--   0 runner    (1001) docker     (122)    55472 2023-05-23 18:59:10.000000 mathphys-2.8.0/mathphys/imgproc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1774 2023-05-23 18:59:10.000000 mathphys-2.8.0/mathphys/units.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:59:23.985159 mathphys-2.8.0/mathphys.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-05-23 18:59:23.000000 mathphys-2.8.0/mathphys.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      412 2023-05-23 18:59:23.000000 mathphys-2.8.0/mathphys.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 18:59:23.000000 mathphys-2.8.0/mathphys.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 18:59:23.000000 mathphys-2.8.0/mathphys.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-23 18:59:23.000000 mathphys-2.8.0/mathphys.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-23 18:59:23.000000 mathphys-2.8.0/mathphys.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-23 18:59:10.000000 mathphys-2.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 18:59:23.985159 mathphys-2.8.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1204 2023-05-23 18:59:10.000000 mathphys-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 20:21:51.848339 mathphys-2.8.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-05-23 20:21:41.000000 mathphys-2.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-23 20:21:41.000000 mathphys-2.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-05-23 20:21:51.848339 mathphys-2.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1107 2023-05-23 20:21:41.000000 mathphys-2.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 20:21:51.848339 mathphys-2.8.1/mathphys/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-23 20:21:50.000000 mathphys-2.8.1/mathphys/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)      577 2023-05-23 20:21:41.000000 mathphys-2.8.1/mathphys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-05-23 20:21:41.000000 mathphys-2.8.1/mathphys/base_units.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2385 2023-05-23 20:21:41.000000 mathphys-2.8.1/mathphys/beam_optics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-05-23 20:21:41.000000 mathphys-2.8.1/mathphys/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6242 2023-05-23 20:21:41.000000 mathphys-2.8.1/mathphys/functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    55511 2023-05-23 20:21:41.000000 mathphys-2.8.1/mathphys/imgproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1774 2023-05-23 20:21:41.000000 mathphys-2.8.1/mathphys/units.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 20:21:51.848339 mathphys-2.8.1/mathphys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-05-23 20:21:51.000000 mathphys-2.8.1/mathphys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      412 2023-05-23 20:21:51.000000 mathphys-2.8.1/mathphys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 20:21:51.000000 mathphys-2.8.1/mathphys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 20:21:51.000000 mathphys-2.8.1/mathphys.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-23 20:21:51.000000 mathphys-2.8.1/mathphys.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-23 20:21:51.000000 mathphys-2.8.1/mathphys.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-23 20:21:41.000000 mathphys-2.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 20:21:51.848339 mathphys-2.8.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1204 2023-05-23 20:21:41.000000 mathphys-2.8.1/setup.py
```

### Comparing `mathphys-2.8.0/LICENSE` & `mathphys-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mathphys-2.8.0/PKG-INFO` & `mathphys-2.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathphys
-Version: 2.8.0
+Version: 2.8.1
 Summary: LNLS Math and Physics Utilities
 Home-page: https://github.com/lnls-fac/mathphys
 Download-URL: https://github.com/lnls-fac/mathphys
 Author: lnls-fac
 Author-email: xresende@gmail.com
 License: MIT License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mathphys-2.8.0/README.md` & `mathphys-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `mathphys-2.8.0/mathphys/__init__.py` & `mathphys-2.8.1/mathphys/__init__.py`

 * *Files identical despite different names*

### Comparing `mathphys-2.8.0/mathphys/beam_optics.py` & `mathphys-2.8.1/mathphys/beam_optics.py`

 * *Files identical despite different names*

### Comparing `mathphys-2.8.0/mathphys/constants.py` & `mathphys-2.8.1/mathphys/constants.py`

 * *Files identical despite different names*

### Comparing `mathphys-2.8.0/mathphys/functions.py` & `mathphys-2.8.1/mathphys/functions.py`

 * *Files identical despite different names*

### Comparing `mathphys-2.8.0/mathphys/imgproc.py` & `mathphys-2.8.1/mathphys/imgproc.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,15 +521,15 @@
 
         return _np.sum(self.data)
 
     @property
     def is_saturated(self):
         """Check if image is saturated."""
         return self._is_saturated
-    
+
     @property
     def is_with_image(self):
         """Check if image has signal."""
         return self._is_with_image
 
     def imshow(self, fig=None, axes=None, cropx=None, cropy=None):
         """."""
@@ -1248,15 +1248,15 @@
         # print('u', u)
         # print('vt', vt)
         axis1, axis2 = vt.T
         axis1, axis2 = u.T
         if axis1[0] < 0:
             axis1 *= -1
         # print('axis1', axis1)
-        angle = _np.arctan2(axis1[1], axis1[0]) * 180 / _np.pi
+        angle = - _np.arctan2(axis1[1], axis1[0]) * 180 / _np.pi
 
         return angle, sigma1, sigma2
 
     @staticmethod
     def calc_rotated_sigma(angle, sigma1, sigma2):
         """Convert normal sigmas to sigmas in rotated axes give angle [deg]."""
         angle *= _np.pi / 180
@@ -1277,15 +1277,15 @@
         #   (mean ± std. dev. of 7 runs, 1000 loops each)
 
         self._roi_mean = None
         self._roi_sigma = None
         self._roi_amp = None
         self._roi_fit = None
         self._roi_fit_error = None
-        self._fitgauss = fitgauss or FitGaussian
+        self._fitgauss = fitgauss or FitGaussianScipy()
         super().__init__(*args, **kwargs)
         self._update_image_roi(*args, **kwargs)
 
     @property
     def roi_sigma(self):
         """Image roiy fitted gaussian sigma."""
         return self._roi_sigma
@@ -1392,15 +1392,15 @@
 
         self._use_svd4theta = use_svd4theta
         self._fitx = None
         self._fity = None
         self._angle = None
         self._sigma1 = None
         self._sigma2 = None
-        self._fitgauss = fitgauss or FitGaussian
+        self._fitgauss = fitgauss or FitGaussianScipy()
         super().__init__(*args, **kwargs)
         self._update_image_fit(roix=roix, roiy=roiy)
 
     @property
     def use_svd4theta(self):
         """Return whether SVD of 2nd-moment matrix is used for theta calc."""
         return self._use_svd4theta
@@ -1601,14 +1601,16 @@
                 lw=2, label='roiy_fit')
 
         axes.legend()
         axes.grid()
         axes.set_ylabel('ROI pixel indices')
         axes.set_ylabel('Projection Intensity')
 
+        return fig, axes
+
     def __str__(self):
         """."""
         res = super().__str__()
         res += '\n--- fitx ---\n'
         res += self.fitx.__str__()
         res += f'\nroi_amplitude   : {self.fitx.roi_amplitude}'
         res += f'\nroi_mean        : {self.fitx.roi_mean}'
@@ -1635,14 +1637,15 @@
         return roix, roiy
 
     def _update_image_fit(self, roix=None, roiy=None):
         """."""
         # fit projections
         roix, roiy = Image2D.update_roi(self.data, roix, roiy)
         data = self.project_image(self._data, 0)
+
         self._fity = Image1D_Fit(
             data=data, roi=roiy, fitgauss=self._fitgauss)
         self._fity.set_saturation_flag(self.is_saturated)
         data = self.project_image(self._data, 1)
         self._fitx = Image1D_Fit(
             data=data, roi=roix, fitgauss=self._fitgauss)
         self._fitx.set_saturation_flag(self.is_saturated)
```

### Comparing `mathphys-2.8.0/mathphys/units.py` & `mathphys-2.8.1/mathphys/units.py`

 * *Files identical despite different names*

### Comparing `mathphys-2.8.0/mathphys.egg-info/PKG-INFO` & `mathphys-2.8.1/mathphys.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathphys
-Version: 2.8.0
+Version: 2.8.1
 Summary: LNLS Math and Physics Utilities
 Home-page: https://github.com/lnls-fac/mathphys
 Download-URL: https://github.com/lnls-fac/mathphys
 Author: lnls-fac
 Author-email: xresende@gmail.com
 License: MIT License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mathphys-2.8.0/setup.py` & `mathphys-2.8.1/setup.py`

 * *Files identical despite different names*

