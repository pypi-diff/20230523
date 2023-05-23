# Comparing `tmp/fdtd-0.2.8.tar.gz` & `tmp/fdtd-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdtd-0.2.8.tar", last modified: Mon Mar 27 14:33:29 2023, max compression
+gzip compressed data, was "fdtd-0.3.0.tar", last modified: Tue May 23 13:13:51 2023, max compression
```

## Comparing `fdtd-0.2.8.tar` & `fdtd-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 flaport   (1000) flaport   (1000)        0 2023-03-27 14:33:29.193811 fdtd-0.2.8/
--rw-r--r--   0 flaport   (1000) flaport   (1000)     1086 2023-03-27 14:31:49.000000 fdtd-0.2.8/LICENSE
--rw-r--r--   0 flaport   (1000) flaport   (1000)       34 2023-03-27 14:31:49.000000 fdtd-0.2.8/MANIFEST.in
--rw-r--r--   0 flaport   (1000) flaport   (1000)    27988 2023-03-27 14:33:29.193811 fdtd-0.2.8/PKG-INFO
--rw-r--r--   0 flaport   (1000) flaport   (1000)    27380 2023-03-27 14:31:49.000000 fdtd-0.2.8/README.md
-drwxr-xr-x   0 flaport   (1000) flaport   (1000)        0 2023-03-27 14:33:29.190477 fdtd-0.2.8/fdtd/
--rw-r--r--   0 flaport   (1000) flaport   (1000)      500 2023-03-27 14:33:01.000000 fdtd-0.2.8/fdtd/__init__.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)    12989 2023-03-27 14:31:49.000000 fdtd-0.2.8/fdtd/backend.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)    23779 2023-03-27 14:31:49.000000 fdtd-0.2.8/fdtd/boundaries.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)      423 2023-03-27 14:31:49.000000 fdtd-0.2.8/fdtd/constants.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)     1317 2023-03-27 14:31:49.000000 fdtd-0.2.8/fdtd/conversions.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)    16983 2023-03-27 14:31:49.000000 fdtd-0.2.8/fdtd/detectors.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)    12796 2023-03-27 14:31:49.000000 fdtd-0.2.8/fdtd/fourier.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)    16692 2023-03-27 14:31:49.000000 fdtd-0.2.8/fdtd/grid.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)     8756 2023-03-27 14:32:15.000000 fdtd-0.2.8/fdtd/objects.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)    23028 2023-03-27 14:31:49.000000 fdtd-0.2.8/fdtd/sources.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)      444 2023-03-27 14:31:49.000000 fdtd-0.2.8/fdtd/typing_.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)    18226 2023-03-27 14:31:49.000000 fdtd-0.2.8/fdtd/visualization.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)     1623 2023-03-27 14:31:49.000000 fdtd-0.2.8/fdtd/waveforms.py
-drwxr-xr-x   0 flaport   (1000) flaport   (1000)        0 2023-03-27 14:33:29.190477 fdtd-0.2.8/fdtd.egg-info/
--rw-r--r--   0 flaport   (1000) flaport   (1000)    27988 2023-03-27 14:33:29.000000 fdtd-0.2.8/fdtd.egg-info/PKG-INFO
--rw-r--r--   0 flaport   (1000) flaport   (1000)      675 2023-03-27 14:33:29.000000 fdtd-0.2.8/fdtd.egg-info/SOURCES.txt
--rw-r--r--   0 flaport   (1000) flaport   (1000)        1 2023-03-27 14:33:29.000000 fdtd-0.2.8/fdtd.egg-info/dependency_links.txt
--rw-r--r--   0 flaport   (1000) flaport   (1000)      160 2023-03-27 14:33:29.000000 fdtd-0.2.8/fdtd.egg-info/requires.txt
--rw-r--r--   0 flaport   (1000) flaport   (1000)        5 2023-03-27 14:33:29.000000 fdtd-0.2.8/fdtd.egg-info/top_level.txt
--rw-r--r--   0 flaport   (1000) flaport   (1000)      232 2023-03-27 14:31:49.000000 fdtd-0.2.8/pyproject.toml
--rw-r--r--   0 flaport   (1000) flaport   (1000)      817 2023-03-27 14:33:29.193811 fdtd-0.2.8/setup.cfg
-drwxr-xr-x   0 flaport   (1000) flaport   (1000)        0 2023-03-27 14:33:29.193811 fdtd-0.2.8/tests/
--rw-r--r--   0 flaport   (1000) flaport   (1000)     4049 2023-03-27 14:31:49.000000 fdtd-0.2.8/tests/test_antenna_impedance.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)      512 2023-03-27 14:31:49.000000 fdtd-0.2.8/tests/test_backend.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)     2034 2023-03-27 14:31:49.000000 fdtd-0.2.8/tests/test_boundaries.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)     3601 2023-03-27 14:31:49.000000 fdtd-0.2.8/tests/test_detectors.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)     1692 2023-03-27 14:31:49.000000 fdtd-0.2.8/tests/test_fft.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)     5299 2023-03-27 14:31:49.000000 fdtd-0.2.8/tests/test_grid.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)      298 2023-03-27 14:31:49.000000 fdtd-0.2.8/tests/test_objects.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)     1268 2023-03-27 14:31:49.000000 fdtd-0.2.8/tests/test_sources.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)       85 2023-03-27 14:31:49.000000 fdtd-0.2.8/tests/test_typing.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)       85 2023-03-27 14:31:49.000000 fdtd-0.2.8/tests/test_visualization.py
--rw-r--r--   0 flaport   (1000) flaport   (1000)      566 2023-03-27 14:31:49.000000 fdtd-0.2.8/tests/test_waveforms.py
+drwxr-xr-x   0 flaport   (1000) flaport   (1000)        0 2023-05-23 13:13:51.354970 fdtd-0.3.0/
+-rw-r--r--   0 flaport   (1000) flaport   (1000)     1086 2023-03-27 14:31:49.000000 fdtd-0.3.0/LICENSE
+-rw-r--r--   0 flaport   (1000) flaport   (1000)       34 2023-03-27 14:31:49.000000 fdtd-0.3.0/MANIFEST.in
+-rw-r--r--   0 flaport   (1000) flaport   (1000)    27988 2023-05-23 13:13:51.354970 fdtd-0.3.0/PKG-INFO
+-rw-r--r--   0 flaport   (1000) flaport   (1000)    27380 2023-03-27 14:31:49.000000 fdtd-0.3.0/README.md
+drwxr-xr-x   0 flaport   (1000) flaport   (1000)        0 2023-05-23 13:13:51.348303 fdtd-0.3.0/fdtd/
+-rw-r--r--   0 flaport   (1000) flaport   (1000)      500 2023-05-23 13:12:35.000000 fdtd-0.3.0/fdtd/__init__.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)    13226 2023-05-23 13:12:28.000000 fdtd-0.3.0/fdtd/backend.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)    24194 2023-05-23 13:12:28.000000 fdtd-0.3.0/fdtd/boundaries.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)      423 2023-03-27 14:31:49.000000 fdtd-0.3.0/fdtd/constants.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)     1317 2023-03-27 14:31:49.000000 fdtd-0.3.0/fdtd/conversions.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)    16983 2023-03-27 14:31:49.000000 fdtd-0.3.0/fdtd/detectors.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)    12796 2023-03-27 14:31:49.000000 fdtd-0.3.0/fdtd/fourier.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)    16935 2023-05-23 13:12:28.000000 fdtd-0.3.0/fdtd/grid.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)     9051 2023-05-23 13:12:28.000000 fdtd-0.3.0/fdtd/objects.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)    23028 2023-03-27 14:31:49.000000 fdtd-0.3.0/fdtd/sources.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)      444 2023-03-27 14:31:49.000000 fdtd-0.3.0/fdtd/typing_.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)    18231 2023-05-23 13:12:28.000000 fdtd-0.3.0/fdtd/visualization.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)     1623 2023-03-27 14:31:49.000000 fdtd-0.3.0/fdtd/waveforms.py
+drwxr-xr-x   0 flaport   (1000) flaport   (1000)        0 2023-05-23 13:13:51.351637 fdtd-0.3.0/fdtd.egg-info/
+-rw-r--r--   0 flaport   (1000) flaport   (1000)    27988 2023-05-23 13:13:51.000000 fdtd-0.3.0/fdtd.egg-info/PKG-INFO
+-rw-r--r--   0 flaport   (1000) flaport   (1000)      675 2023-05-23 13:13:51.000000 fdtd-0.3.0/fdtd.egg-info/SOURCES.txt
+-rw-r--r--   0 flaport   (1000) flaport   (1000)        1 2023-05-23 13:13:51.000000 fdtd-0.3.0/fdtd.egg-info/dependency_links.txt
+-rw-r--r--   0 flaport   (1000) flaport   (1000)      160 2023-05-23 13:13:51.000000 fdtd-0.3.0/fdtd.egg-info/requires.txt
+-rw-r--r--   0 flaport   (1000) flaport   (1000)        5 2023-05-23 13:13:51.000000 fdtd-0.3.0/fdtd.egg-info/top_level.txt
+-rw-r--r--   0 flaport   (1000) flaport   (1000)      232 2023-03-27 14:31:49.000000 fdtd-0.3.0/pyproject.toml
+-rw-r--r--   0 flaport   (1000) flaport   (1000)      817 2023-05-23 13:13:51.354970 fdtd-0.3.0/setup.cfg
+drwxr-xr-x   0 flaport   (1000) flaport   (1000)        0 2023-05-23 13:13:51.354970 fdtd-0.3.0/tests/
+-rw-r--r--   0 flaport   (1000) flaport   (1000)     4049 2023-03-27 14:31:49.000000 fdtd-0.3.0/tests/test_antenna_impedance.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)      512 2023-03-27 14:31:49.000000 fdtd-0.3.0/tests/test_backend.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)     2034 2023-03-27 14:31:49.000000 fdtd-0.3.0/tests/test_boundaries.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)     3601 2023-03-27 14:31:49.000000 fdtd-0.3.0/tests/test_detectors.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)     1692 2023-03-27 14:31:49.000000 fdtd-0.3.0/tests/test_fft.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)     5299 2023-03-27 14:31:49.000000 fdtd-0.3.0/tests/test_grid.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)      298 2023-03-27 14:31:49.000000 fdtd-0.3.0/tests/test_objects.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)     1268 2023-03-27 14:31:49.000000 fdtd-0.3.0/tests/test_sources.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)       85 2023-03-27 14:31:49.000000 fdtd-0.3.0/tests/test_typing.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)       85 2023-03-27 14:31:49.000000 fdtd-0.3.0/tests/test_visualization.py
+-rw-r--r--   0 flaport   (1000) flaport   (1000)      566 2023-03-27 14:31:49.000000 fdtd-0.3.0/tests/test_waveforms.py
```

### Comparing `fdtd-0.2.8/LICENSE` & `fdtd-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fdtd-0.2.8/PKG-INFO` & `fdtd-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdtd
-Version: 0.2.8
+Version: 0.3.0
 Summary: a 3D electromagnetic FDTD simulator written in Python
 Home-page: http://github.com/flaport/fdtd
 Author: Floris Laporte
 Author-email: floris.laporte@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `fdtd-0.2.8/README.md` & `fdtd-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fdtd-0.2.8/fdtd/backend.py` & `fdtd-0.3.0/fdtd/backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,17 @@
 
     # types
     int = numpy.int64
     """ integer type for array"""
 
     float = numpy.float64
     """ floating type for array """
+    
+    complex = numpy.complex128
+    """ complex type for array """
 
     # methods
     asarray = _replace_float(numpy.asarray)
 
     exp = staticmethod(numpy.exp)
     """ exponential of all elements in array """
 
@@ -197,14 +200,20 @@
         # types
         int = torch.int64
         """ integer type for array"""
 
         float = torch.get_default_dtype()
         """ floating type for array """
 
+        if float is torch.float32:
+            complex = torch.complex64
+        else:
+            complex = torch.complex128
+        """ complex type for array """
+
         # methods
         asarray = staticmethod(torch.as_tensor)
         """ create an array """
 
         exp = staticmethod(torch.exp)
         """ exponential of all elements in array """
```

### Comparing `fdtd-0.2.8/fdtd/boundaries.py` & `fdtd-0.3.0/fdtd/boundaries.py`

 * *Files 7% similar despite different names*

```diff
@@ -99,14 +99,25 @@
 
     def update_H(self):
         """ Update magnetic field of the grid
 
         Note:
             this method is called *after* the grid fields are updated
         """
+    def promote_dtypes_to_complex(self):
+        self.phi_E = bd.complex(self.phi_E)
+        self.phi_H = bd.complex(self.phi_H)
+
+        self.psi_Ex = bd.complex(self.psi_Ex)
+        self.psi_Ey = bd.complex(self.psi_Ey)
+        self.psi_Ez = bd.complex(self.psi_Ez)
+        
+        self.psi_Hx = bd.complex(self.psi_Hx)
+        self.psi_Hy = bd.complex(self.psi_Hy)
+        self.psi_Hz = bd.complex(self.psi_Hz)
 
     def __repr__(self):
         return f"PML(name={repr(self.name)})"
 
     def __str__(self):
         s = "    " + repr(self) + "\n"
```

### Comparing `fdtd-0.2.8/fdtd/conversions.py` & `fdtd-0.3.0/fdtd/conversions.py`

 * *Files identical despite different names*

### Comparing `fdtd-0.2.8/fdtd/detectors.py` & `fdtd-0.3.0/fdtd/detectors.py`

 * *Files identical despite different names*

### Comparing `fdtd-0.2.8/fdtd/fourier.py` & `fdtd-0.3.0/fdtd/fourier.py`

 * *Files identical despite different names*

### Comparing `fdtd-0.2.8/fdtd/grid.py` & `fdtd-0.3.0/fdtd/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     Args:
         E: Electric field to take the curl of (E-type field located on the
            edges of the grid cell [integer gridpoints])
 
     Returns:
         The curl of E (H-type field located on the faces of the grid [half-integer grid points])
     """
-    curl = bd.zeros(E.shape)
+    curl = bd.zeros(E.shape,dtype=E.dtype)
 
     curl[:, :-1, :, 0] += E[:, 1:, :, 2] - E[:, :-1, :, 2]
     curl[:, :, :-1, 0] -= E[:, :, 1:, 1] - E[:, :, :-1, 1]
 
     curl[:, :, :-1, 1] += E[:, :, 1:, 0] - E[:, :, :-1, 0]
     curl[:-1, :, :, 1] -= E[1:, :, :, 2] - E[:-1, :, :, 2]
 
@@ -58,15 +58,15 @@
     Args:
         H: Magnetic field to take the curl of (H-type field located on half-integer grid points)
 
     Returns:
         The curl of H (E-type field located on the edges of the grid [integer grid points])
 
     """
-    curl = bd.zeros(H.shape)
+    curl = bd.zeros(H.shape,dtype=H.dtype)
 
     curl[:, 1:, :, 0] += H[:, 1:, :, 2] - H[:, :-1, :, 2]
     curl[:, :, 1:, 0] -= H[:, :, 1:, 1] - H[:, :, :-1, 1]
 
     curl[:, :, 1:, 1] += H[:, :, 1:, 0] - H[:, :, :-1, 0]
     curl[1:, :, :, 1] -= H[1:, :, :, 2] - H[:-1, :, :, 2]
 
@@ -259,15 +259,15 @@
         if isinstance(total_time, float):
             total_time /= self.time_step
         time = range(0, int(total_time), 1)
         if progress_bar:
             time = tqdm(time)
         for _ in time:
             self.step()
-
+    
     def step(self):
         """do a single FDTD step by first updating the electric field and then
         updating the magnetic field
         """
         self.update_E()
         self.update_H()
         self.time_steps_passed += 1
@@ -345,14 +345,19 @@
         detector._register_grid(self)
         self.detectors[name] = detector
 
     def add_object(self, name, obj):
         """add an object to the grid"""
         obj._register_grid(self)
         self.objects[name] = obj
+    
+    def promote_dtypes_to_complex(self):
+        self.E = self.E.astype(bd.complex)
+        self.H = self.H.astype(bd.complex)
+        [boundary.promote_dtypes_to_complex() for boundary in self.boundaries]
 
     def __setitem__(self, key, attr):
         if not isinstance(key, tuple):
             x, y, z = key, slice(None), slice(None)
         elif len(key) == 1:
             x, y, z = key[0], slice(None), slice(None)
         elif len(key) == 2:
```

### Comparing `fdtd-0.2.8/fdtd/objects.py` & `fdtd-0.3.0/fdtd/objects.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,18 @@
             grid: the grid to register the object into
             x: the x-location of the object in the grid
             y: the y-location of the object in the grid
             z: the z-location of the object in the grid
         """
         self.grid = grid
         self.grid.objects.append(self)
+
+        if self.permittivity.dtype is bd.complex().dtype:
+            self.grid.promote_dtypes_to_complex()
+
         if self.name is not None:
             if not hasattr(grid, self.name):
                 setattr(grid, self.name, self)
             else:
                 raise ValueError(
                     f"The grid already has an attribute with name {self.name}"
                 )
@@ -62,15 +66,15 @@
         self.Ny = abs(self.y.stop - self.y.start)
         self.Nz = abs(self.z.stop - self.z.start)
 
         # set the permittivity of the object
         if bd.is_array(self.permittivity) and len(self.permittivity.shape) == 3:
             self.permittivity = self.permittivity[:, :, :, None]
         self.inverse_permittivity = (
-            bd.ones((self.Nx, self.Ny, self.Nz, 3)) / self.permittivity
+            bd.ones((self.Nx, self.Ny, self.Nz, 3),dtype=self.permittivity.dtype) / self.permittivity
         )
 
         # set the permittivity values of the object at its border to be equal
         # to the grid permittivity. This way, the object is made symmetric.
         if self.Nx > 1:
             self.inverse_permittivity[-1, :, :, 0] = self.grid.inverse_permittivity[
                 -1, self.y, self.z, 0
@@ -114,25 +118,29 @@
         """custom update equations for inside the object
 
         Args:
             curl_H: the curl of magnetic field in the grid.
 
         """
         loc = (self.x, self.y, self.z)
-        self.grid.E[loc] += (
+
+        self.grid.E[loc] = self.grid.E[loc] +(
             self.grid.courant_number * self.inverse_permittivity * curl_H[loc]
-        )
+            )
 
     def update_H(self, curl_E):
         """custom update equations for inside the object
 
         Args:
             curl_E: the curl of electric field in the grid.
 
         """
+    # def promote_dtypes_to_complex(self):
+    #     self.E = self.E.astype(bd.complex)
+    #     self.H = self.H.astype(bd.complex)
 
     def __repr__(self):
         return f"{self.__class__.__name__}(name={repr(self.name)})"
 
     def __str__(self):
         s = "    " + repr(self) + "\n"
```

### Comparing `fdtd-0.2.8/fdtd/sources.py` & `fdtd-0.3.0/fdtd/sources.py`

 * *Files identical despite different names*

### Comparing `fdtd-0.2.8/fdtd/visualization.py` & `fdtd-0.3.0/fdtd/visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,15 @@
         )
         plt.gca().add_patch(patch)
 
     # visualize the energy in the grid
     cmap_norm = None
     if norm == "log":
         cmap_norm = LogNorm(vmin=1e-4, vmax=grid_energy.max() + 1e-4)
-    plt.imshow(bd.numpy(grid_energy), cmap=cmap, interpolation="sinc", norm=cmap_norm)
+    plt.imshow(abs(bd.numpy(grid_energy)), cmap=cmap, interpolation="sinc", norm=cmap_norm)
 
     # finalize the plot
     plt.ylabel(xlabel)
     plt.xlabel(ylabel)
     plt.ylim(Nx, -1)
     plt.xlim(-1, Ny)
     plt.figlegend()
```

### Comparing `fdtd-0.2.8/fdtd/waveforms.py` & `fdtd-0.3.0/fdtd/waveforms.py`

 * *Files identical despite different names*

### Comparing `fdtd-0.2.8/fdtd.egg-info/PKG-INFO` & `fdtd-0.3.0/fdtd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdtd
-Version: 0.2.8
+Version: 0.3.0
 Summary: a 3D electromagnetic FDTD simulator written in Python
 Home-page: http://github.com/flaport/fdtd
 Author: Floris Laporte
 Author-email: floris.laporte@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `fdtd-0.2.8/fdtd.egg-info/SOURCES.txt` & `fdtd-0.3.0/fdtd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fdtd-0.2.8/setup.cfg` & `fdtd-0.3.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fdtd
-version = 0.2.8
+version = 0.3.0
 description = a 3D electromagnetic FDTD simulator written in Python
 author = Floris Laporte
 author_email = floris.laporte@gmail.com
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://github.com/flaport/fdtd
 classifiers =
```

### Comparing `fdtd-0.2.8/tests/test_antenna_impedance.py` & `fdtd-0.3.0/tests/test_antenna_impedance.py`

 * *Files identical despite different names*

### Comparing `fdtd-0.2.8/tests/test_backend.py` & `fdtd-0.3.0/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `fdtd-0.2.8/tests/test_boundaries.py` & `fdtd-0.3.0/tests/test_boundaries.py`

 * *Files identical despite different names*

### Comparing `fdtd-0.2.8/tests/test_detectors.py` & `fdtd-0.3.0/tests/test_detectors.py`

 * *Files identical despite different names*

### Comparing `fdtd-0.2.8/tests/test_fft.py` & `fdtd-0.3.0/tests/test_fft.py`

 * *Files identical despite different names*

### Comparing `fdtd-0.2.8/tests/test_grid.py` & `fdtd-0.3.0/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `fdtd-0.2.8/tests/test_sources.py` & `fdtd-0.3.0/tests/test_sources.py`

 * *Files identical despite different names*

### Comparing `fdtd-0.2.8/tests/test_waveforms.py` & `fdtd-0.3.0/tests/test_waveforms.py`

 * *Files identical despite different names*

